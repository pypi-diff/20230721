# Comparing `tmp/OpenTEA-3.5.0.tar.gz` & `tmp/OpenTEA-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OpenTEA-3.5.0.tar", last modified: Thu Feb  2 12:36:35 2023, max compression
+gzip compressed data, was "OpenTEA-3.6.0.tar", last modified: Fri Jul 21 12:25:47 2023, max compression
```

## Comparing `OpenTEA-3.5.0.tar` & `OpenTEA-3.6.0.tar`

### file list

```diff
@@ -1,156 +1,197 @@
-drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-02-02 12:36:35.141886 OpenTEA-3.5.0/
--rw-r--r--   0 dauptain   (502) staff       (20)     1630 2022-07-08 08:58:25.000000 OpenTEA-3.5.0/LICENSE
--rw-r--r--   0 dauptain   (502) staff       (20)        9 2022-07-08 08:58:25.000000 OpenTEA-3.5.0/MANIFEST.in
--rw-r--r--   0 dauptain   (502) staff       (20)     4937 2023-02-02 12:36:35.142152 OpenTEA-3.5.0/PKG-INFO
--rw-r--r--   0 dauptain   (502) staff       (20)     4010 2022-07-08 08:58:25.000000 OpenTEA-3.5.0/README.md
--rw-r--r--   0 dauptain   (502) staff       (20)     1358 2023-02-02 12:36:35.143551 OpenTEA-3.5.0/setup.cfg
--rw-r--r--   0 dauptain   (502) staff       (20)       38 2022-07-08 08:58:25.000000 OpenTEA-3.5.0/setup.py
-drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-02-02 12:36:34.788223 OpenTEA-3.5.0/src/
-drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-02-02 12:36:34.801780 OpenTEA-3.5.0/src/OpenTEA.egg-info/
--rw-r--r--   0 dauptain   (502) staff       (20)     4937 2023-02-02 12:36:34.000000 OpenTEA-3.5.0/src/OpenTEA.egg-info/PKG-INFO
--rw-r--r--   0 dauptain   (502) staff       (20)     5603 2023-02-02 12:36:34.000000 OpenTEA-3.5.0/src/OpenTEA.egg-info/SOURCES.txt
--rw-r--r--   0 dauptain   (502) staff       (20)        1 2023-02-02 12:36:34.000000 OpenTEA-3.5.0/src/OpenTEA.egg-info/dependency_links.txt
--rw-r--r--   0 dauptain   (502) staff       (20)       50 2023-02-02 12:36:34.000000 OpenTEA-3.5.0/src/OpenTEA.egg-info/entry_points.txt
--rw-r--r--   0 dauptain   (502) staff       (20)        1 2022-07-08 11:41:40.000000 OpenTEA-3.5.0/src/OpenTEA.egg-info/not-zip-safe
--rw-r--r--   0 dauptain   (502) staff       (20)      196 2023-02-02 12:36:34.000000 OpenTEA-3.5.0/src/OpenTEA.egg-info/requires.txt
--rw-r--r--   0 dauptain   (502) staff       (20)       19 2023-02-02 12:36:34.000000 OpenTEA-3.5.0/src/OpenTEA.egg-info/top_level.txt
-drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-02-02 12:36:34.802681 OpenTEA-3.5.0/src/gallery/
--rw-r--r--   0 dauptain   (502) staff       (20)    41511 2022-07-08 08:58:25.000000 OpenTEA-3.5.0/src/gallery/trivial.png
-drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-02-02 12:36:34.814471 OpenTEA-3.5.0/src/opentea/
--rw-r--r--   0 dauptain   (502) staff       (20)     6148 2022-09-20 13:11:24.000000 OpenTEA-3.5.0/src/opentea/.DS_Store
--rw-r--r--   0 dauptain   (502) staff       (20)      139 2022-12-06 16:11:33.000000 OpenTEA-3.5.0/src/opentea/__init__.py
-drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-02-02 12:36:34.818858 OpenTEA-3.5.0/src/opentea/__pycache__/
--rw-r--r--   0 dauptain   (502) staff       (20)      270 2022-12-16 22:10:43.000000 OpenTEA-3.5.0/src/opentea/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)     1943 2022-10-04 23:03:12.000000 OpenTEA-3.5.0/src/opentea/__pycache__/cli.cpython-39.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)     3785 2022-07-08 11:42:15.000000 OpenTEA-3.5.0/src/opentea/__pycache__/process_utils.cpython-39.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)     1958 2022-10-04 23:02:48.000000 OpenTEA-3.5.0/src/opentea/cli.py
-drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-02-02 12:36:34.820004 OpenTEA-3.5.0/src/opentea/examples/
-drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-02-02 12:36:34.828132 OpenTEA-3.5.0/src/opentea/examples/calculator/
--rw-r--r--   0 dauptain   (502) staff       (20)        0 2022-07-08 08:58:25.000000 OpenTEA-3.5.0/src/opentea/examples/calculator/__init__.py
-drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-02-02 12:36:34.831260 OpenTEA-3.5.0/src/opentea/examples/calculator/__pycache__/
--rw-r--r--   0 dauptain   (502) staff       (20)      165 2022-07-08 11:41:55.000000 OpenTEA-3.5.0/src/opentea/examples/calculator/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)      871 2022-10-05 13:51:24.000000 OpenTEA-3.5.0/src/opentea/examples/calculator/__pycache__/startup.cpython-39.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)      937 2022-07-08 08:58:25.000000 OpenTEA-3.5.0/src/opentea/examples/calculator/callback_tab1.py
--rw-r--r--   0 dauptain   (502) staff       (20)     1613 2022-07-08 08:58:25.000000 OpenTEA-3.5.0/src/opentea/examples/calculator/dataset_from_gui.yml
--rw-r--r--   0 dauptain   (502) staff       (20)    15092 2022-09-23 09:25:53.000000 OpenTEA-3.5.0/src/opentea/examples/calculator/schema_calculator.yaml
--rw-r--r--   0 dauptain   (502) staff       (20)      669 2022-10-04 23:05:42.000000 OpenTEA-3.5.0/src/opentea/examples/calculator/startup.py
--rw-r--r--   0 dauptain   (502) staff       (20)      982 2022-07-08 08:58:25.000000 OpenTEA-3.5.0/src/opentea/examples/calculator/updatde3dscene_1.py
--rw-r--r--   0 dauptain   (502) staff       (20)     1070 2022-07-08 08:58:25.000000 OpenTEA-3.5.0/src/opentea/examples/dataset_to_gui.yml
-drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-02-02 12:36:34.850719 OpenTEA-3.5.0/src/opentea/examples/simple/
--rw-r--r--   0 dauptain   (502) staff       (20)      483 2022-07-08 08:58:25.000000 OpenTEA-3.5.0/src/opentea/examples/simple/.tmp_docu.html
--rw-r--r--   0 dauptain   (502) staff       (20)        0 2022-07-08 08:58:25.000000 OpenTEA-3.5.0/src/opentea/examples/simple/__init__.py
-drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-02-02 12:36:34.860794 OpenTEA-3.5.0/src/opentea/examples/simple/__pycache__/
--rw-r--r--   0 dauptain   (502) staff       (20)      161 2022-07-08 11:41:55.000000 OpenTEA-3.5.0/src/opentea/examples/simple/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)      842 2022-10-04 22:57:36.000000 OpenTEA-3.5.0/src/opentea/examples/simple/__pycache__/startup.cpython-39.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)      701 2022-07-08 08:58:25.000000 OpenTEA-3.5.0/src/opentea/examples/simple/process_controleifreq.py
--rw-r--r--   0 dauptain   (502) staff       (20)     4821 2022-07-08 08:58:25.000000 OpenTEA-3.5.0/src/opentea/examples/simple/schema_simple.yaml
--rw-r--r--   0 dauptain   (502) staff       (20)      638 2022-10-04 22:56:26.000000 OpenTEA-3.5.0/src/opentea/examples/simple/startup.py
--rw-r--r--   0 dauptain   (502) staff       (20)    29085 2022-07-08 08:58:25.000000 OpenTEA-3.5.0/src/opentea/examples/simple/test-pattern-tv.jpg
--rw-r--r--   0 dauptain   (502) staff       (20)     3118 2022-07-08 08:58:25.000000 OpenTEA-3.5.0/src/opentea/examples/simple/test.png
--rw-r--r--   0 dauptain   (502) staff       (20)      547 2022-07-08 08:58:25.000000 OpenTEA-3.5.0/src/opentea/examples/simple/test.py
--rw-r--r--   0 dauptain   (502) staff       (20)    26843 2022-07-08 08:58:25.000000 OpenTEA-3.5.0/src/opentea/examples/simple/vegetable-icon-png-16.png
-drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-02-02 12:36:34.881977 OpenTEA-3.5.0/src/opentea/examples/trivial/
--rw-r--r--   0 dauptain   (502) staff       (20)        0 2022-07-08 08:58:25.000000 OpenTEA-3.5.0/src/opentea/examples/trivial/__init__.py
-drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-02-02 12:36:34.885334 OpenTEA-3.5.0/src/opentea/examples/trivial/__pycache__/
--rw-r--r--   0 dauptain   (502) staff       (20)      162 2022-07-08 11:41:52.000000 OpenTEA-3.5.0/src/opentea/examples/trivial/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)      854 2022-10-04 22:57:34.000000 OpenTEA-3.5.0/src/opentea/examples/trivial/__pycache__/startup.cpython-39.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)      671 2022-07-08 08:58:25.000000 OpenTEA-3.5.0/src/opentea/examples/trivial/custom_callback.py
--rw-r--r--   0 dauptain   (502) staff       (20)       95 2022-07-08 08:58:25.000000 OpenTEA-3.5.0/src/opentea/examples/trivial/dataset_from_gui.yml
--rw-r--r--   0 dauptain   (502) staff       (20)       96 2022-07-08 08:58:25.000000 OpenTEA-3.5.0/src/opentea/examples/trivial/dataset_to_gui.yml
--rw-r--r--   0 dauptain   (502) staff       (20)      834 2022-07-08 08:58:25.000000 OpenTEA-3.5.0/src/opentea/examples/trivial/schema_trivial.yaml
--rw-r--r--   0 dauptain   (502) staff       (20)      657 2022-10-04 22:56:33.000000 OpenTEA-3.5.0/src/opentea/examples/trivial/startup.py
-drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-02-02 12:36:34.905207 OpenTEA-3.5.0/src/opentea/gui_forms/
--rw-r--r--   0 dauptain   (502) staff       (20)        0 2022-07-08 08:58:25.000000 OpenTEA-3.5.0/src/opentea/gui_forms/__init__.py
-drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-02-02 12:36:34.925569 OpenTEA-3.5.0/src/opentea/gui_forms/__pycache__/
--rw-r--r--   0 dauptain   (502) staff       (20)      155 2022-07-08 11:41:52.000000 OpenTEA-3.5.0/src/opentea/gui_forms/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)     6220 2022-09-26 15:02:15.000000 OpenTEA-3.5.0/src/opentea/gui_forms/__pycache__/_base.cpython-39.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)      562 2022-07-08 11:41:53.000000 OpenTEA-3.5.0/src/opentea/gui_forms/__pycache__/_exceptions.cpython-39.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)     2924 2022-09-26 13:47:04.000000 OpenTEA-3.5.0/src/opentea/gui_forms/__pycache__/constants.cpython-39.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)     9015 2022-09-21 09:29:14.000000 OpenTEA-3.5.0/src/opentea/gui_forms/__pycache__/generic_widgets.cpython-39.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)    44454 2023-02-02 11:22:47.000000 OpenTEA-3.5.0/src/opentea/gui_forms/__pycache__/leaf_widgets.cpython-39.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)     7287 2022-09-26 13:30:12.000000 OpenTEA-3.5.0/src/opentea/gui_forms/__pycache__/menus.cpython-39.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)    44357 2022-12-16 22:10:43.000000 OpenTEA-3.5.0/src/opentea/gui_forms/__pycache__/node_widgets.cpython-39.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)     1918 2022-09-26 13:47:04.000000 OpenTEA-3.5.0/src/opentea/gui_forms/__pycache__/otinker.cpython-39.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)     8903 2022-11-21 10:04:50.000000 OpenTEA-3.5.0/src/opentea/gui_forms/__pycache__/root_widget.cpython-39.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)     1438 2022-12-29 14:26:49.000000 OpenTEA-3.5.0/src/opentea/gui_forms/__pycache__/soundboard.cpython-39.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)     4090 2022-09-23 09:27:48.000000 OpenTEA-3.5.0/src/opentea/gui_forms/__pycache__/utils.cpython-39.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)     1297 2022-11-18 13:00:02.000000 OpenTEA-3.5.0/src/opentea/gui_forms/__pycache__/viewer_2d.cpython-39.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)     2204 2022-11-18 13:00:02.000000 OpenTEA-3.5.0/src/opentea/gui_forms/__pycache__/viewer_3d.cpython-39.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)     6384 2022-09-26 14:58:57.000000 OpenTEA-3.5.0/src/opentea/gui_forms/_base.py
--rw-r--r--   0 dauptain   (502) staff       (20)      189 2022-07-08 08:58:25.000000 OpenTEA-3.5.0/src/opentea/gui_forms/_exceptions.py
--rw-r--r--   0 dauptain   (502) staff       (20)     3577 2022-09-26 13:44:47.000000 OpenTEA-3.5.0/src/opentea/gui_forms/constants.py
--rw-r--r--   0 dauptain   (502) staff       (20)     9139 2022-09-21 08:22:26.000000 OpenTEA-3.5.0/src/opentea/gui_forms/generic_widgets.py
-drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-02-02 12:36:34.956785 OpenTEA-3.5.0/src/opentea/gui_forms/images/
--rw-r--r--   0 dauptain   (502) staff       (20)      670 2022-07-08 08:58:25.000000 OpenTEA-3.5.0/src/opentea/gui_forms/images/about_icon.gif
--rw-r--r--   0 dauptain   (502) staff       (20)      161 2022-07-08 08:58:25.000000 OpenTEA-3.5.0/src/opentea/gui_forms/images/docu_icon.gif
--rw-r--r--   0 dauptain   (502) staff       (20)      670 2022-07-08 08:58:25.000000 OpenTEA-3.5.0/src/opentea/gui_forms/images/help_icon.gif
--rw-r--r--   0 dauptain   (502) staff       (20)      691 2022-07-08 08:58:25.000000 OpenTEA-3.5.0/src/opentea/gui_forms/images/invalid_icon.gif
--rw-r--r--   0 dauptain   (502) staff       (20)     1026 2022-07-08 08:58:25.000000 OpenTEA-3.5.0/src/opentea/gui_forms/images/load_icon.gif
--rw-r--r--   0 dauptain   (502) staff       (20)    10783 2022-07-08 08:58:25.000000 OpenTEA-3.5.0/src/opentea/gui_forms/images/logo_opentea.gif
--rw-r--r--   0 dauptain   (502) staff       (20)     5303 2022-07-08 08:58:25.000000 OpenTEA-3.5.0/src/opentea/gui_forms/images/logo_project_large.gif
--rw-r--r--   0 dauptain   (502) staff       (20)      188 2022-07-08 08:58:25.000000 OpenTEA-3.5.0/src/opentea/gui_forms/images/minus_icon.gif
--rw-r--r--   0 dauptain   (502) staff       (20)     1062 2022-07-08 08:58:25.000000 OpenTEA-3.5.0/src/opentea/gui_forms/images/new_icon.gif
--rw-r--r--   0 dauptain   (502) staff       (20)      197 2022-07-08 08:58:25.000000 OpenTEA-3.5.0/src/opentea/gui_forms/images/plus_icon.gif
--rw-r--r--   0 dauptain   (502) staff       (20)      129 2022-07-08 08:58:25.000000 OpenTEA-3.5.0/src/opentea/gui_forms/images/quit_icon.gif
--rw-r--r--   0 dauptain   (502) staff       (20)     1109 2022-07-08 08:58:25.000000 OpenTEA-3.5.0/src/opentea/gui_forms/images/save_icon.gif
--rw-r--r--   0 dauptain   (502) staff       (20)      202 2022-07-08 08:58:25.000000 OpenTEA-3.5.0/src/opentea/gui_forms/images/tree_icon.gif
--rw-r--r--   0 dauptain   (502) staff       (20)      670 2022-07-08 08:58:25.000000 OpenTEA-3.5.0/src/opentea/gui_forms/images/unknown_icon.gif
--rw-r--r--   0 dauptain   (502) staff       (20)      686 2022-07-08 08:58:25.000000 OpenTEA-3.5.0/src/opentea/gui_forms/images/valid_icon.gif
--rw-r--r--   0 dauptain   (502) staff       (20)     1684 2022-07-08 08:58:25.000000 OpenTEA-3.5.0/src/opentea/gui_forms/images/wait_2_icon.gif
--rw-r--r--   0 dauptain   (502) staff       (20)    43085 2023-02-02 12:02:09.000000 OpenTEA-3.5.0/src/opentea/gui_forms/leaf_widgets.py
--rw-r--r--   0 dauptain   (502) staff       (20)     6132 2022-09-26 13:20:22.000000 OpenTEA-3.5.0/src/opentea/gui_forms/menus.py
--rw-r--r--   0 dauptain   (502) staff       (20)    51257 2022-12-06 16:04:49.000000 OpenTEA-3.5.0/src/opentea/gui_forms/node_widgets.py
--rw-r--r--   0 dauptain   (502) staff       (20)     1976 2022-09-26 13:35:52.000000 OpenTEA-3.5.0/src/opentea/gui_forms/otinker.py
--rw-r--r--   0 dauptain   (502) staff       (20)     9384 2022-11-21 09:14:22.000000 OpenTEA-3.5.0/src/opentea/gui_forms/root_widget.py
--rw-r--r--   0 dauptain   (502) staff       (20)      572 2022-12-29 14:26:43.000000 OpenTEA-3.5.0/src/opentea/gui_forms/soundboard.py
--rw-r--r--   0 dauptain   (502) staff       (20)     4229 2022-09-23 09:27:37.000000 OpenTEA-3.5.0/src/opentea/gui_forms/utils.py
--rw-r--r--   0 dauptain   (502) staff       (20)      817 2022-11-18 12:59:42.000000 OpenTEA-3.5.0/src/opentea/gui_forms/viewer_2d.py
--rw-r--r--   0 dauptain   (502) staff       (20)     2367 2022-11-18 12:59:55.000000 OpenTEA-3.5.0/src/opentea/gui_forms/viewer_3d.py
-drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-02-02 12:36:35.006777 OpenTEA-3.5.0/src/opentea/gui_forms/wav/
--rw-r--r--   0 dauptain   (502) staff       (20)     4239 2022-09-21 08:22:26.000000 OpenTEA-3.5.0/src/opentea/gui_forms/wav/dsbdcls.wav
--rw-r--r--   0 dauptain   (502) staff       (20)     4225 2022-09-21 08:22:26.000000 OpenTEA-3.5.0/src/opentea/gui_forms/wav/dsbdopn.wav
--rw-r--r--   0 dauptain   (502) staff       (20)    13926 2022-09-21 08:22:26.000000 OpenTEA-3.5.0/src/opentea/gui_forms/wav/dsdorcls.wav
--rw-r--r--   0 dauptain   (502) staff       (20)    13860 2022-09-21 08:22:26.000000 OpenTEA-3.5.0/src/opentea/gui_forms/wav/dsdoropn.wav
--rw-r--r--   0 dauptain   (502) staff       (20)     2307 2022-09-21 08:22:26.000000 OpenTEA-3.5.0/src/opentea/gui_forms/wav/dsitemup.wav
--rw-r--r--   0 dauptain   (502) staff       (20)     3954 2022-09-21 08:22:26.000000 OpenTEA-3.5.0/src/opentea/gui_forms/wav/dsoof.wav
--rw-r--r--   0 dauptain   (502) staff       (20)    15196 2022-09-21 08:22:26.000000 OpenTEA-3.5.0/src/opentea/gui_forms/wav/dsplpain.wav
--rw-r--r--   0 dauptain   (502) staff       (20)     6299 2022-09-21 08:22:26.000000 OpenTEA-3.5.0/src/opentea/gui_forms/wav/dsswtchn.wav
-drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-02-02 12:36:35.025445 OpenTEA-3.5.0/src/opentea/noob/
--rw-r--r--   0 dauptain   (502) staff       (20)        0 2022-07-08 08:58:25.000000 OpenTEA-3.5.0/src/opentea/noob/__init__.py
-drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-02-02 12:36:35.043804 OpenTEA-3.5.0/src/opentea/noob/__pycache__/
--rw-r--r--   0 dauptain   (502) staff       (20)      150 2022-07-08 11:41:52.000000 OpenTEA-3.5.0/src/opentea/noob/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)     4542 2022-07-08 11:41:55.000000 OpenTEA-3.5.0/src/opentea/noob/__pycache__/asciigraph.cpython-39.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)     4656 2022-07-08 11:41:52.000000 OpenTEA-3.5.0/src/opentea/noob/__pycache__/check_schema.cpython-39.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)     5029 2022-07-08 11:41:55.000000 OpenTEA-3.5.0/src/opentea/noob/__pycache__/inferdefault.cpython-39.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)     8033 2022-07-08 11:41:52.000000 OpenTEA-3.5.0/src/opentea/noob/__pycache__/noob.cpython-39.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)      877 2022-07-08 11:41:55.000000 OpenTEA-3.5.0/src/opentea/noob/__pycache__/schema.cpython-39.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)      426 2022-11-18 10:08:58.000000 OpenTEA-3.5.0/src/opentea/noob/__pycache__/utils.cpython-39.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)     4034 2022-11-18 10:08:58.000000 OpenTEA-3.5.0/src/opentea/noob/__pycache__/validate_light.cpython-39.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)     8493 2022-07-08 11:41:55.000000 OpenTEA-3.5.0/src/opentea/noob/__pycache__/validation.cpython-39.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)     4694 2022-07-08 08:58:25.000000 OpenTEA-3.5.0/src/opentea/noob/asciigraph.py
--rw-r--r--   0 dauptain   (502) staff       (20)     5898 2022-07-08 08:58:25.000000 OpenTEA-3.5.0/src/opentea/noob/check_schema.py
--rw-r--r--   0 dauptain   (502) staff       (20)     8641 2022-07-08 08:58:25.000000 OpenTEA-3.5.0/src/opentea/noob/inferdefault.py
--rw-r--r--   0 dauptain   (502) staff       (20)     8877 2022-07-08 08:58:25.000000 OpenTEA-3.5.0/src/opentea/noob/noob.py
--rw-r--r--   0 dauptain   (502) staff       (20)    80506 2022-07-08 08:58:25.000000 OpenTEA-3.5.0/src/opentea/noob/schema.json
--rw-r--r--   0 dauptain   (502) staff       (20)      777 2022-07-08 08:58:25.000000 OpenTEA-3.5.0/src/opentea/noob/schema.py
--rw-r--r--   0 dauptain   (502) staff       (20)      397 2022-07-08 08:58:25.000000 OpenTEA-3.5.0/src/opentea/noob/utils.py
--rw-r--r--   0 dauptain   (502) staff       (20)     5560 2022-11-18 09:50:02.000000 OpenTEA-3.5.0/src/opentea/noob/validate_light.py
--rw-r--r--   0 dauptain   (502) staff       (20)    12531 2022-07-08 08:58:25.000000 OpenTEA-3.5.0/src/opentea/noob/validation.py
--rw-r--r--   0 dauptain   (502) staff       (20)     4061 2022-07-08 08:58:25.000000 OpenTEA-3.5.0/src/opentea/process_utils.py
-drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-02-02 12:36:35.057304 OpenTEA-3.5.0/src/opentea/tools/
--rw-r--r--   0 dauptain   (502) staff       (20)        0 2022-07-08 08:58:25.000000 OpenTEA-3.5.0/src/opentea/tools/__init__.py
-drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-02-02 12:36:35.133839 OpenTEA-3.5.0/src/opentea/tools/__pycache__/
--rw-r--r--   0 dauptain   (502) staff       (20)      151 2022-09-23 08:40:49.000000 OpenTEA-3.5.0/src/opentea/tools/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)     8419 2022-09-23 08:40:49.000000 OpenTEA-3.5.0/src/opentea/tools/__pycache__/proxy_h5.cpython-39.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)     3877 2022-09-23 08:40:49.000000 OpenTEA-3.5.0/src/opentea/tools/__pycache__/schema2md.cpython-39.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)     3277 2022-11-18 10:08:58.000000 OpenTEA-3.5.0/src/opentea/tools/__pycache__/visit_h5.cpython-39.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)     7781 2022-07-08 08:58:25.000000 OpenTEA-3.5.0/src/opentea/tools/proxy_h5.py
--rw-r--r--   0 dauptain   (502) staff       (20)     4607 2022-07-08 08:58:25.000000 OpenTEA-3.5.0/src/opentea/tools/schema2md.py
--rw-r--r--   0 dauptain   (502) staff       (20)     2943 2022-07-08 08:58:25.000000 OpenTEA-3.5.0/src/opentea/tools/visit_h5.py
-drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-02-02 12:36:35.138088 OpenTEA-3.5.0/src/tkhtmlview/
--rw-r--r--   0 dauptain   (502) staff       (20)      264 2022-07-08 08:58:25.000000 OpenTEA-3.5.0/src/tkhtmlview/README.md
--rwxr-xr-x   0 dauptain   (502) staff       (20)     4517 2022-07-08 08:58:25.000000 OpenTEA-3.5.0/src/tkhtmlview/__init__.py
-drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-02-02 12:36:35.140681 OpenTEA-3.5.0/src/tkhtmlview/__pycache__/
--rw-r--r--   0 dauptain   (502) staff       (20)     4192 2022-07-08 11:41:53.000000 OpenTEA-3.5.0/src/tkhtmlview/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)    17079 2022-07-08 11:41:53.000000 OpenTEA-3.5.0/src/tkhtmlview/__pycache__/html_parser.cpython-39.pyc
--rwxr-xr-x   0 dauptain   (502) staff       (20)    26203 2022-07-08 08:58:25.000000 OpenTEA-3.5.0/src/tkhtmlview/html_parser.py
+drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-07-21 12:25:47.189061 OpenTEA-3.6.0/
+-rw-r--r--   0 dauptain   (502) staff       (20)     1630 2022-07-08 08:58:25.000000 OpenTEA-3.6.0/LICENSE
+-rw-r--r--   0 dauptain   (502) staff       (20)        9 2022-07-08 08:58:25.000000 OpenTEA-3.6.0/MANIFEST.in
+-rw-r--r--   0 dauptain   (502) staff       (20)     4937 2023-07-21 12:25:47.189141 OpenTEA-3.6.0/PKG-INFO
+-rw-r--r--   0 dauptain   (502) staff       (20)     4010 2022-07-08 08:58:25.000000 OpenTEA-3.6.0/README.md
+-rw-r--r--   0 dauptain   (502) staff       (20)     1422 2023-07-21 12:25:47.189648 OpenTEA-3.6.0/setup.cfg
+-rw-r--r--   0 dauptain   (502) staff       (20)       38 2022-07-08 08:58:25.000000 OpenTEA-3.6.0/setup.py
+drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-07-21 12:25:47.142130 OpenTEA-3.6.0/src/
+drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-07-21 12:25:47.144856 OpenTEA-3.6.0/src/OpenTEA.egg-info/
+-rw-r--r--   0 dauptain   (502) staff       (20)     4937 2023-07-21 12:25:47.000000 OpenTEA-3.6.0/src/OpenTEA.egg-info/PKG-INFO
+-rw-r--r--   0 dauptain   (502) staff       (20)     7690 2023-07-21 12:25:47.000000 OpenTEA-3.6.0/src/OpenTEA.egg-info/SOURCES.txt
+-rw-r--r--   0 dauptain   (502) staff       (20)        1 2023-07-21 12:25:47.000000 OpenTEA-3.6.0/src/OpenTEA.egg-info/dependency_links.txt
+-rw-r--r--   0 dauptain   (502) staff       (20)       50 2023-07-21 12:25:47.000000 OpenTEA-3.6.0/src/OpenTEA.egg-info/entry_points.txt
+-rw-r--r--   0 dauptain   (502) staff       (20)        1 2022-07-08 11:41:40.000000 OpenTEA-3.6.0/src/OpenTEA.egg-info/not-zip-safe
+-rw-r--r--   0 dauptain   (502) staff       (20)      212 2023-07-21 12:25:47.000000 OpenTEA-3.6.0/src/OpenTEA.egg-info/requires.txt
+-rw-r--r--   0 dauptain   (502) staff       (20)       19 2023-07-21 12:25:47.000000 OpenTEA-3.6.0/src/OpenTEA.egg-info/top_level.txt
+drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-07-21 12:25:47.145050 OpenTEA-3.6.0/src/gallery/
+-rw-r--r--   0 dauptain   (502) staff       (20)    41511 2022-07-08 08:58:25.000000 OpenTEA-3.6.0/src/gallery/trivial.png
+drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-07-21 12:25:47.146495 OpenTEA-3.6.0/src/opentea/
+-rw-r--r--   0 dauptain   (502) staff       (20)     6148 2022-09-20 13:11:24.000000 OpenTEA-3.6.0/src/opentea/.DS_Store
+-rw-r--r--   0 dauptain   (502) staff       (20)      139 2023-07-21 12:23:42.000000 OpenTEA-3.6.0/src/opentea/__init__.py
+drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-07-21 12:25:47.148654 OpenTEA-3.6.0/src/opentea/__pycache__/
+-rw-r--r--   0 dauptain   (502) staff       (20)      297 2023-03-17 16:31:17.000000 OpenTEA-3.6.0/src/opentea/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)      270 2022-12-16 22:10:43.000000 OpenTEA-3.6.0/src/opentea/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     3019 2023-07-17 13:25:07.000000 OpenTEA-3.6.0/src/opentea/__pycache__/cli.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     1943 2022-10-04 23:03:12.000000 OpenTEA-3.6.0/src/opentea/__pycache__/cli.cpython-39.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     5505 2023-03-21 16:38:55.000000 OpenTEA-3.6.0/src/opentea/__pycache__/process_utils.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     3785 2022-07-08 11:42:15.000000 OpenTEA-3.6.0/src/opentea/__pycache__/process_utils.cpython-39.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     1958 2022-10-04 23:02:48.000000 OpenTEA-3.6.0/src/opentea/cli.py
+drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-07-21 12:25:47.148913 OpenTEA-3.6.0/src/opentea/examples/
+drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-07-21 12:25:47.150535 OpenTEA-3.6.0/src/opentea/examples/calculator/
+-rw-r--r--   0 dauptain   (502) staff       (20)        0 2022-07-08 08:58:25.000000 OpenTEA-3.6.0/src/opentea/examples/calculator/__init__.py
+drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-07-21 12:25:47.151482 OpenTEA-3.6.0/src/opentea/examples/calculator/__pycache__/
+-rw-r--r--   0 dauptain   (502) staff       (20)      183 2023-07-17 13:25:18.000000 OpenTEA-3.6.0/src/opentea/examples/calculator/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)      165 2022-07-08 11:41:55.000000 OpenTEA-3.6.0/src/opentea/examples/calculator/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     1694 2023-07-17 13:25:18.000000 OpenTEA-3.6.0/src/opentea/examples/calculator/__pycache__/startup.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)      871 2022-10-05 13:51:24.000000 OpenTEA-3.6.0/src/opentea/examples/calculator/__pycache__/startup.cpython-39.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)      937 2022-07-08 08:58:25.000000 OpenTEA-3.6.0/src/opentea/examples/calculator/callback_tab1.py
+-rw-r--r--   0 dauptain   (502) staff       (20)     1613 2022-07-08 08:58:25.000000 OpenTEA-3.6.0/src/opentea/examples/calculator/dataset_from_gui.yml
+-rw-r--r--   0 dauptain   (502) staff       (20)    15092 2022-09-23 09:25:53.000000 OpenTEA-3.6.0/src/opentea/examples/calculator/schema_calculator.yaml
+-rw-r--r--   0 dauptain   (502) staff       (20)      669 2022-10-04 23:05:42.000000 OpenTEA-3.6.0/src/opentea/examples/calculator/startup.py
+-rw-r--r--   0 dauptain   (502) staff       (20)      982 2022-07-08 08:58:25.000000 OpenTEA-3.6.0/src/opentea/examples/calculator/updatde3dscene_1.py
+-rw-r--r--   0 dauptain   (502) staff       (20)     1070 2022-07-08 08:58:25.000000 OpenTEA-3.6.0/src/opentea/examples/dataset_to_gui.yml
+drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-07-21 12:25:47.153472 OpenTEA-3.6.0/src/opentea/examples/simple/
+-rw-r--r--   0 dauptain   (502) staff       (20)      483 2022-07-08 08:58:25.000000 OpenTEA-3.6.0/src/opentea/examples/simple/.tmp_docu.html
+-rw-r--r--   0 dauptain   (502) staff       (20)        0 2022-07-08 08:58:25.000000 OpenTEA-3.6.0/src/opentea/examples/simple/__init__.py
+drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-07-21 12:25:47.154308 OpenTEA-3.6.0/src/opentea/examples/simple/__pycache__/
+-rw-r--r--   0 dauptain   (502) staff       (20)      179 2023-07-17 13:25:18.000000 OpenTEA-3.6.0/src/opentea/examples/simple/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)      161 2022-07-08 11:41:55.000000 OpenTEA-3.6.0/src/opentea/examples/simple/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     1660 2023-07-17 13:25:18.000000 OpenTEA-3.6.0/src/opentea/examples/simple/__pycache__/startup.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)      842 2022-10-04 22:57:36.000000 OpenTEA-3.6.0/src/opentea/examples/simple/__pycache__/startup.cpython-39.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)      701 2022-07-08 08:58:25.000000 OpenTEA-3.6.0/src/opentea/examples/simple/process_controleifreq.py
+-rw-r--r--   0 dauptain   (502) staff       (20)     4821 2022-07-08 08:58:25.000000 OpenTEA-3.6.0/src/opentea/examples/simple/schema_simple.yaml
+-rw-r--r--   0 dauptain   (502) staff       (20)      638 2022-10-04 22:56:26.000000 OpenTEA-3.6.0/src/opentea/examples/simple/startup.py
+-rw-r--r--   0 dauptain   (502) staff       (20)    29085 2022-07-08 08:58:25.000000 OpenTEA-3.6.0/src/opentea/examples/simple/test-pattern-tv.jpg
+-rw-r--r--   0 dauptain   (502) staff       (20)     3118 2022-07-08 08:58:25.000000 OpenTEA-3.6.0/src/opentea/examples/simple/test.png
+-rw-r--r--   0 dauptain   (502) staff       (20)      547 2022-07-08 08:58:25.000000 OpenTEA-3.6.0/src/opentea/examples/simple/test.py
+-rw-r--r--   0 dauptain   (502) staff       (20)    26843 2022-07-08 08:58:25.000000 OpenTEA-3.6.0/src/opentea/examples/simple/vegetable-icon-png-16.png
+drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-07-21 12:25:47.155448 OpenTEA-3.6.0/src/opentea/examples/trivial/
+-rw-r--r--   0 dauptain   (502) staff       (20)        0 2022-07-08 08:58:25.000000 OpenTEA-3.6.0/src/opentea/examples/trivial/__init__.py
+drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-07-21 12:25:47.156228 OpenTEA-3.6.0/src/opentea/examples/trivial/__pycache__/
+-rw-r--r--   0 dauptain   (502) staff       (20)      180 2023-07-17 13:25:17.000000 OpenTEA-3.6.0/src/opentea/examples/trivial/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)      162 2022-07-08 11:41:52.000000 OpenTEA-3.6.0/src/opentea/examples/trivial/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     1676 2023-07-17 13:25:17.000000 OpenTEA-3.6.0/src/opentea/examples/trivial/__pycache__/startup.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)      854 2022-10-04 22:57:34.000000 OpenTEA-3.6.0/src/opentea/examples/trivial/__pycache__/startup.cpython-39.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)      671 2022-07-08 08:58:25.000000 OpenTEA-3.6.0/src/opentea/examples/trivial/custom_callback.py
+-rw-r--r--   0 dauptain   (502) staff       (20)       95 2022-07-08 08:58:25.000000 OpenTEA-3.6.0/src/opentea/examples/trivial/dataset_from_gui.yml
+-rw-r--r--   0 dauptain   (502) staff       (20)       96 2022-07-08 08:58:25.000000 OpenTEA-3.6.0/src/opentea/examples/trivial/dataset_to_gui.yml
+-rw-r--r--   0 dauptain   (502) staff       (20)      834 2022-07-08 08:58:25.000000 OpenTEA-3.6.0/src/opentea/examples/trivial/schema_trivial.yaml
+-rw-r--r--   0 dauptain   (502) staff       (20)      657 2022-10-04 22:56:33.000000 OpenTEA-3.6.0/src/opentea/examples/trivial/startup.py
+drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-07-21 12:25:47.160297 OpenTEA-3.6.0/src/opentea/gui_forms/
+-rw-r--r--   0 dauptain   (502) staff       (20)        0 2022-07-08 08:58:25.000000 OpenTEA-3.6.0/src/opentea/gui_forms/__init__.py
+drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-07-21 12:25:47.169370 OpenTEA-3.6.0/src/opentea/gui_forms/__pycache__/
+-rw-r--r--   0 dauptain   (502) staff       (20)      173 2023-03-17 16:31:17.000000 OpenTEA-3.6.0/src/opentea/gui_forms/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)      155 2022-07-08 11:41:52.000000 OpenTEA-3.6.0/src/opentea/gui_forms/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     9065 2023-03-17 16:31:17.000000 OpenTEA-3.6.0/src/opentea/gui_forms/__pycache__/_base.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     6220 2022-09-26 15:02:15.000000 OpenTEA-3.6.0/src/opentea/gui_forms/__pycache__/_base.cpython-39.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)      705 2023-03-17 16:31:17.000000 OpenTEA-3.6.0/src/opentea/gui_forms/__pycache__/_exceptions.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)      562 2022-07-08 11:41:53.000000 OpenTEA-3.6.0/src/opentea/gui_forms/__pycache__/_exceptions.cpython-39.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     5874 2023-07-20 14:52:02.000000 OpenTEA-3.6.0/src/opentea/gui_forms/__pycache__/constants.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     2924 2022-09-26 13:47:04.000000 OpenTEA-3.6.0/src/opentea/gui_forms/__pycache__/constants.cpython-39.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)    17086 2023-03-17 16:31:17.000000 OpenTEA-3.6.0/src/opentea/gui_forms/__pycache__/generic_widgets.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     9015 2022-09-21 09:29:14.000000 OpenTEA-3.6.0/src/opentea/gui_forms/__pycache__/generic_widgets.cpython-39.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)    74702 2023-03-17 16:31:17.000000 OpenTEA-3.6.0/src/opentea/gui_forms/__pycache__/leaf_widgets.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)    44415 2023-02-15 15:35:08.000000 OpenTEA-3.6.0/src/opentea/gui_forms/__pycache__/leaf_widgets.cpython-39.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)    12660 2023-07-20 13:35:06.000000 OpenTEA-3.6.0/src/opentea/gui_forms/__pycache__/menus.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     7287 2022-09-26 13:30:12.000000 OpenTEA-3.6.0/src/opentea/gui_forms/__pycache__/menus.cpython-39.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)    83421 2023-07-20 20:07:11.000000 OpenTEA-3.6.0/src/opentea/gui_forms/__pycache__/node_widgets.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)    44357 2022-12-16 22:10:43.000000 OpenTEA-3.6.0/src/opentea/gui_forms/__pycache__/node_widgets.cpython-39.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     3086 2023-07-11 10:48:35.000000 OpenTEA-3.6.0/src/opentea/gui_forms/__pycache__/otinker.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     1918 2022-09-26 13:47:04.000000 OpenTEA-3.6.0/src/opentea/gui_forms/__pycache__/otinker.cpython-39.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)    14518 2023-03-17 16:31:17.000000 OpenTEA-3.6.0/src/opentea/gui_forms/__pycache__/root_widget.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     8903 2022-11-21 10:04:50.000000 OpenTEA-3.6.0/src/opentea/gui_forms/__pycache__/root_widget.cpython-39.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     1923 2023-03-17 16:31:17.000000 OpenTEA-3.6.0/src/opentea/gui_forms/__pycache__/soundboard.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     1438 2022-12-29 14:26:49.000000 OpenTEA-3.6.0/src/opentea/gui_forms/__pycache__/soundboard.cpython-39.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     6547 2023-03-17 16:31:17.000000 OpenTEA-3.6.0/src/opentea/gui_forms/__pycache__/utils.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     4090 2022-09-23 09:27:48.000000 OpenTEA-3.6.0/src/opentea/gui_forms/__pycache__/utils.cpython-39.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     2027 2023-03-17 16:31:17.000000 OpenTEA-3.6.0/src/opentea/gui_forms/__pycache__/viewer_2d.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     1297 2022-11-18 13:00:02.000000 OpenTEA-3.6.0/src/opentea/gui_forms/__pycache__/viewer_2d.cpython-39.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     4225 2023-07-11 11:14:13.000000 OpenTEA-3.6.0/src/opentea/gui_forms/__pycache__/viewer_3d.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     2204 2022-11-18 13:00:02.000000 OpenTEA-3.6.0/src/opentea/gui_forms/__pycache__/viewer_3d.cpython-39.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     6384 2022-09-26 14:58:57.000000 OpenTEA-3.6.0/src/opentea/gui_forms/_base.py
+-rw-r--r--   0 dauptain   (502) staff       (20)      189 2022-07-08 08:58:25.000000 OpenTEA-3.6.0/src/opentea/gui_forms/_exceptions.py
+-rw-r--r--   0 dauptain   (502) staff       (20)     3903 2023-07-20 14:42:12.000000 OpenTEA-3.6.0/src/opentea/gui_forms/constants.py
+-rw-r--r--   0 dauptain   (502) staff       (20)     9139 2022-09-21 08:22:26.000000 OpenTEA-3.6.0/src/opentea/gui_forms/generic_widgets.py
+drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-07-21 12:25:47.172893 OpenTEA-3.6.0/src/opentea/gui_forms/images/
+-rw-r--r--   0 dauptain   (502) staff       (20)      670 2022-07-08 08:58:25.000000 OpenTEA-3.6.0/src/opentea/gui_forms/images/about_icon.gif
+-rw-r--r--   0 dauptain   (502) staff       (20)      161 2022-07-08 08:58:25.000000 OpenTEA-3.6.0/src/opentea/gui_forms/images/docu_icon.gif
+-rw-r--r--   0 dauptain   (502) staff       (20)      670 2022-07-08 08:58:25.000000 OpenTEA-3.6.0/src/opentea/gui_forms/images/help_icon.gif
+-rw-r--r--   0 dauptain   (502) staff       (20)      691 2022-07-08 08:58:25.000000 OpenTEA-3.6.0/src/opentea/gui_forms/images/invalid_icon.gif
+-rw-r--r--   0 dauptain   (502) staff       (20)     1026 2022-07-08 08:58:25.000000 OpenTEA-3.6.0/src/opentea/gui_forms/images/load_icon.gif
+-rw-r--r--   0 dauptain   (502) staff       (20)    10783 2022-07-08 08:58:25.000000 OpenTEA-3.6.0/src/opentea/gui_forms/images/logo_opentea.gif
+-rw-r--r--   0 dauptain   (502) staff       (20)     5303 2022-07-08 08:58:25.000000 OpenTEA-3.6.0/src/opentea/gui_forms/images/logo_project_large.gif
+-rw-r--r--   0 dauptain   (502) staff       (20)      188 2022-07-08 08:58:25.000000 OpenTEA-3.6.0/src/opentea/gui_forms/images/minus_icon.gif
+-rw-r--r--   0 dauptain   (502) staff       (20)     1062 2022-07-08 08:58:25.000000 OpenTEA-3.6.0/src/opentea/gui_forms/images/new_icon.gif
+-rw-r--r--   0 dauptain   (502) staff       (20)      197 2022-07-08 08:58:25.000000 OpenTEA-3.6.0/src/opentea/gui_forms/images/plus_icon.gif
+-rw-r--r--   0 dauptain   (502) staff       (20)      129 2022-07-08 08:58:25.000000 OpenTEA-3.6.0/src/opentea/gui_forms/images/quit_icon.gif
+-rw-r--r--   0 dauptain   (502) staff       (20)     1109 2022-07-08 08:58:25.000000 OpenTEA-3.6.0/src/opentea/gui_forms/images/save_icon.gif
+-rw-r--r--   0 dauptain   (502) staff       (20)      202 2022-07-08 08:58:25.000000 OpenTEA-3.6.0/src/opentea/gui_forms/images/tree_icon.gif
+-rw-r--r--   0 dauptain   (502) staff       (20)      670 2022-07-08 08:58:25.000000 OpenTEA-3.6.0/src/opentea/gui_forms/images/unknown_icon.gif
+-rw-r--r--   0 dauptain   (502) staff       (20)      686 2022-07-08 08:58:25.000000 OpenTEA-3.6.0/src/opentea/gui_forms/images/valid_icon.gif
+-rw-r--r--   0 dauptain   (502) staff       (20)     1684 2022-07-08 08:58:25.000000 OpenTEA-3.6.0/src/opentea/gui_forms/images/wait_2_icon.gif
+-rw-r--r--   0 dauptain   (502) staff       (20)    43085 2023-02-02 12:02:09.000000 OpenTEA-3.6.0/src/opentea/gui_forms/leaf_widgets.py
+-rw-r--r--   0 dauptain   (502) staff       (20)     6481 2023-07-20 13:33:16.000000 OpenTEA-3.6.0/src/opentea/gui_forms/menus.py
+-rw-r--r--   0 dauptain   (502) staff       (20)    52214 2023-07-20 20:07:02.000000 OpenTEA-3.6.0/src/opentea/gui_forms/node_widgets.py
+-rw-r--r--   0 dauptain   (502) staff       (20)     2026 2023-07-11 10:40:51.000000 OpenTEA-3.6.0/src/opentea/gui_forms/otinker.py
+-rw-r--r--   0 dauptain   (502) staff       (20)     9384 2022-11-21 09:14:22.000000 OpenTEA-3.6.0/src/opentea/gui_forms/root_widget.py
+-rw-r--r--   0 dauptain   (502) staff       (20)      572 2022-12-29 14:26:43.000000 OpenTEA-3.6.0/src/opentea/gui_forms/soundboard.py
+-rw-r--r--   0 dauptain   (502) staff       (20)     4229 2022-09-23 09:27:37.000000 OpenTEA-3.6.0/src/opentea/gui_forms/utils.py
+-rw-r--r--   0 dauptain   (502) staff       (20)      817 2022-11-18 12:59:42.000000 OpenTEA-3.6.0/src/opentea/gui_forms/viewer_2d.py
+-rw-r--r--   0 dauptain   (502) staff       (20)     2470 2023-07-11 11:13:59.000000 OpenTEA-3.6.0/src/opentea/gui_forms/viewer_3d.py
+drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-07-21 12:25:47.174889 OpenTEA-3.6.0/src/opentea/gui_forms/wav/
+-rw-r--r--   0 dauptain   (502) staff       (20)     4239 2022-09-21 08:22:26.000000 OpenTEA-3.6.0/src/opentea/gui_forms/wav/dsbdcls.wav
+-rw-r--r--   0 dauptain   (502) staff       (20)     4225 2022-09-21 08:22:26.000000 OpenTEA-3.6.0/src/opentea/gui_forms/wav/dsbdopn.wav
+-rw-r--r--   0 dauptain   (502) staff       (20)    13926 2022-09-21 08:22:26.000000 OpenTEA-3.6.0/src/opentea/gui_forms/wav/dsdorcls.wav
+-rw-r--r--   0 dauptain   (502) staff       (20)    13860 2022-09-21 08:22:26.000000 OpenTEA-3.6.0/src/opentea/gui_forms/wav/dsdoropn.wav
+-rw-r--r--   0 dauptain   (502) staff       (20)     2307 2022-09-21 08:22:26.000000 OpenTEA-3.6.0/src/opentea/gui_forms/wav/dsitemup.wav
+-rw-r--r--   0 dauptain   (502) staff       (20)     3954 2022-09-21 08:22:26.000000 OpenTEA-3.6.0/src/opentea/gui_forms/wav/dsoof.wav
+-rw-r--r--   0 dauptain   (502) staff       (20)    15196 2022-09-21 08:22:26.000000 OpenTEA-3.6.0/src/opentea/gui_forms/wav/dsplpain.wav
+-rw-r--r--   0 dauptain   (502) staff       (20)     6299 2022-09-21 08:22:26.000000 OpenTEA-3.6.0/src/opentea/gui_forms/wav/dsswtchn.wav
+drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-07-21 12:25:47.177477 OpenTEA-3.6.0/src/opentea/noob/
+-rw-r--r--   0 dauptain   (502) staff       (20)        0 2022-07-08 08:58:25.000000 OpenTEA-3.6.0/src/opentea/noob/__init__.py
+drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-07-21 12:25:47.181588 OpenTEA-3.6.0/src/opentea/noob/__pycache__/
+-rw-r--r--   0 dauptain   (502) staff       (20)      168 2023-03-17 16:31:17.000000 OpenTEA-3.6.0/src/opentea/noob/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)      150 2022-07-08 11:41:52.000000 OpenTEA-3.6.0/src/opentea/noob/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     6621 2023-03-17 16:31:17.000000 OpenTEA-3.6.0/src/opentea/noob/__pycache__/asciigraph.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     4542 2022-07-08 11:41:55.000000 OpenTEA-3.6.0/src/opentea/noob/__pycache__/asciigraph.cpython-39.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     8641 2023-07-17 13:25:07.000000 OpenTEA-3.6.0/src/opentea/noob/__pycache__/check_schema.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     4656 2022-07-08 11:41:52.000000 OpenTEA-3.6.0/src/opentea/noob/__pycache__/check_schema.cpython-39.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     8869 2023-03-17 16:31:17.000000 OpenTEA-3.6.0/src/opentea/noob/__pycache__/inferdefault.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     5029 2022-07-08 11:41:55.000000 OpenTEA-3.6.0/src/opentea/noob/__pycache__/inferdefault.cpython-39.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)    12344 2023-03-17 16:31:17.000000 OpenTEA-3.6.0/src/opentea/noob/__pycache__/noob.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     8033 2022-07-08 11:41:52.000000 OpenTEA-3.6.0/src/opentea/noob/__pycache__/noob.cpython-39.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     1075 2023-03-17 16:31:17.000000 OpenTEA-3.6.0/src/opentea/noob/__pycache__/schema.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)      877 2022-07-08 11:41:55.000000 OpenTEA-3.6.0/src/opentea/noob/__pycache__/schema.cpython-39.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)      426 2022-11-18 10:08:58.000000 OpenTEA-3.6.0/src/opentea/noob/__pycache__/utils.cpython-39.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     6863 2023-07-11 10:55:18.000000 OpenTEA-3.6.0/src/opentea/noob/__pycache__/validate_light.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     4034 2022-11-18 10:08:58.000000 OpenTEA-3.6.0/src/opentea/noob/__pycache__/validate_light.cpython-39.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)    14882 2023-07-11 10:54:55.000000 OpenTEA-3.6.0/src/opentea/noob/__pycache__/validation.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     8493 2022-07-08 11:41:55.000000 OpenTEA-3.6.0/src/opentea/noob/__pycache__/validation.cpython-39.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     4694 2022-07-08 08:58:25.000000 OpenTEA-3.6.0/src/opentea/noob/asciigraph.py
+-rw-r--r--   0 dauptain   (502) staff       (20)     5898 2022-07-08 08:58:25.000000 OpenTEA-3.6.0/src/opentea/noob/check_schema.py
+-rw-r--r--   0 dauptain   (502) staff       (20)     8641 2022-07-08 08:58:25.000000 OpenTEA-3.6.0/src/opentea/noob/inferdefault.py
+-rw-r--r--   0 dauptain   (502) staff       (20)     8877 2022-07-08 08:58:25.000000 OpenTEA-3.6.0/src/opentea/noob/noob.py
+-rw-r--r--   0 dauptain   (502) staff       (20)    80506 2022-07-08 08:58:25.000000 OpenTEA-3.6.0/src/opentea/noob/schema.json
+-rw-r--r--   0 dauptain   (502) staff       (20)      777 2022-07-08 08:58:25.000000 OpenTEA-3.6.0/src/opentea/noob/schema.py
+-rw-r--r--   0 dauptain   (502) staff       (20)      397 2022-07-08 08:58:25.000000 OpenTEA-3.6.0/src/opentea/noob/utils.py
+-rw-r--r--   0 dauptain   (502) staff       (20)     5615 2023-07-11 10:55:15.000000 OpenTEA-3.6.0/src/opentea/noob/validate_light.py
+-rw-r--r--   0 dauptain   (502) staff       (20)    12543 2023-07-11 10:54:44.000000 OpenTEA-3.6.0/src/opentea/noob/validation.py
+-rw-r--r--   0 dauptain   (502) staff       (20)     4061 2022-07-08 08:58:25.000000 OpenTEA-3.6.0/src/opentea/process_utils.py
+drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-07-21 12:25:47.182297 OpenTEA-3.6.0/src/opentea/tools/
+-rw-r--r--   0 dauptain   (502) staff       (20)        0 2022-07-08 08:58:25.000000 OpenTEA-3.6.0/src/opentea/tools/__init__.py
+drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-07-21 12:25:47.183482 OpenTEA-3.6.0/src/opentea/tools/__pycache__/
+-rw-r--r--   0 dauptain   (502) staff       (20)      151 2022-09-23 08:40:49.000000 OpenTEA-3.6.0/src/opentea/tools/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     8419 2022-09-23 08:40:49.000000 OpenTEA-3.6.0/src/opentea/tools/__pycache__/proxy_h5.cpython-39.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     3877 2022-09-23 08:40:49.000000 OpenTEA-3.6.0/src/opentea/tools/__pycache__/schema2md.cpython-39.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     3277 2022-11-18 10:08:58.000000 OpenTEA-3.6.0/src/opentea/tools/__pycache__/visit_h5.cpython-39.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     7781 2022-07-08 08:58:25.000000 OpenTEA-3.6.0/src/opentea/tools/proxy_h5.py
+-rw-r--r--   0 dauptain   (502) staff       (20)     4607 2022-07-08 08:58:25.000000 OpenTEA-3.6.0/src/opentea/tools/schema2md.py
+-rw-r--r--   0 dauptain   (502) staff       (20)     2943 2022-07-08 08:58:25.000000 OpenTEA-3.6.0/src/opentea/tools/visit_h5.py
+drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-07-21 12:25:47.184328 OpenTEA-3.6.0/src/tkhtmlview/
+-rw-r--r--   0 dauptain   (502) staff       (20)      264 2022-07-08 08:58:25.000000 OpenTEA-3.6.0/src/tkhtmlview/README.md
+-rwxr-xr-x   0 dauptain   (502) staff       (20)     4517 2022-07-08 08:58:25.000000 OpenTEA-3.6.0/src/tkhtmlview/__init__.py
+drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-07-21 12:25:47.186444 OpenTEA-3.6.0/src/tkhtmlview/__pycache__/
+-rw-r--r--   0 dauptain   (502) staff       (20)     8313 2023-03-17 16:31:17.000000 OpenTEA-3.6.0/src/tkhtmlview/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     4192 2022-07-08 11:41:53.000000 OpenTEA-3.6.0/src/tkhtmlview/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)    39975 2023-03-17 16:31:17.000000 OpenTEA-3.6.0/src/tkhtmlview/__pycache__/html_parser.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)    17079 2022-07-08 11:41:53.000000 OpenTEA-3.6.0/src/tkhtmlview/__pycache__/html_parser.cpython-39.pyc
+-rwxr-xr-x   0 dauptain   (502) staff       (20)    26203 2022-07-08 08:58:25.000000 OpenTEA-3.6.0/src/tkhtmlview/html_parser.py
+drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-07-21 12:25:47.188831 OpenTEA-3.6.0/tests/
+-rw-r--r--   0 dauptain   (502) staff       (20)      527 2022-09-21 08:22:26.000000 OpenTEA-3.6.0/tests/test_guiform.py
+-rw-r--r--   0 dauptain   (502) staff       (20)     1115 2022-07-08 08:58:25.000000 OpenTEA-3.6.0/tests/test_infer.py
+-rw-r--r--   0 dauptain   (502) staff       (20)     2546 2022-07-08 08:58:25.000000 OpenTEA-3.6.0/tests/test_noob.py
+-rw-r--r--   0 dauptain   (502) staff       (20)      289 2022-07-08 08:58:25.000000 OpenTEA-3.6.0/tests/test_proxyh5.py
+-rw-r--r--   0 dauptain   (502) staff       (20)      347 2022-07-08 08:58:25.000000 OpenTEA-3.6.0/tests/test_schema2md.py
+-rw-r--r--   0 dauptain   (502) staff       (20)      991 2022-11-15 13:01:22.000000 OpenTEA-3.6.0/tests/test_units.py
+-rw-r--r--   0 dauptain   (502) staff       (20)     1952 2022-07-08 08:58:25.000000 OpenTEA-3.6.0/tests/test_validate.py
```

### Comparing `OpenTEA-3.5.0/LICENSE` & `OpenTEA-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/PKG-INFO` & `OpenTEA-3.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenTEA
-Version: 3.5.0
+Version: 3.6.0
 Summary: Graphical User Interface engine based upon Schema
 Home-page: https://gitlab.com/cerfacs/opentea3
 Author: Antoine Dauptain, Aimad Er-raiy, L. F. Pereira
 Author-email: coop@cerfacs.com
 Project-URL: Homepage, https://gitlab.com/cerfacs/opentea3
 Project-URL: Documentation, https://opentea.readthedocs.io/en/latest/
 Project-URL: Bug Tracker, https://gitlab.com/cerfacs/opentea3/-/issues
```

### Comparing `OpenTEA-3.5.0/README.md` & `OpenTEA-3.6.0/README.md`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/setup.cfg` & `OpenTEA-3.6.0/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -27,17 +27,19 @@
 package_dir = 
 	= src
 packages = find:
 python_requires = >= 3.6
 install_requires = 
 	numpy>=1.16.2
 	h5py>=2.6.0
-	jsonschema
+	loguru   # excellent logger
+	colorama # To colorize log output
 	markdown
 	Pillow>=5.4.1
+	jsonschema
 	PyYAML>=3.13
 	nob>=0.4.1
 	nobvisual
 	requests
 	click
 	tiny_3d_engine>=0.2
 	tiny_2d_engine
```

### Comparing `OpenTEA-3.5.0/src/OpenTEA.egg-info/PKG-INFO` & `OpenTEA-3.6.0/src/OpenTEA.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenTEA
-Version: 3.5.0
+Version: 3.6.0
 Summary: Graphical User Interface engine based upon Schema
 Home-page: https://gitlab.com/cerfacs/opentea3
 Author: Antoine Dauptain, Aimad Er-raiy, L. F. Pereira
 Author-email: coop@cerfacs.com
 Project-URL: Homepage, https://gitlab.com/cerfacs/opentea3
 Project-URL: Documentation, https://opentea.readthedocs.io/en/latest/
 Project-URL: Bug Tracker, https://gitlab.com/cerfacs/opentea3/-/issues
```

### Comparing `OpenTEA-3.5.0/src/OpenTEA.egg-info/SOURCES.txt` & `OpenTEA-3.6.0/src/OpenTEA.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -11,44 +11,53 @@
 src/OpenTEA.egg-info/requires.txt
 src/OpenTEA.egg-info/top_level.txt
 src/gallery/trivial.png
 src/opentea/.DS_Store
 src/opentea/__init__.py
 src/opentea/cli.py
 src/opentea/process_utils.py
+src/opentea/__pycache__/__init__.cpython-311.pyc
 src/opentea/__pycache__/__init__.cpython-39.pyc
+src/opentea/__pycache__/cli.cpython-311.pyc
 src/opentea/__pycache__/cli.cpython-39.pyc
+src/opentea/__pycache__/process_utils.cpython-311.pyc
 src/opentea/__pycache__/process_utils.cpython-39.pyc
 src/opentea/examples/dataset_to_gui.yml
 src/opentea/examples/calculator/__init__.py
 src/opentea/examples/calculator/callback_tab1.py
 src/opentea/examples/calculator/dataset_from_gui.yml
 src/opentea/examples/calculator/schema_calculator.yaml
 src/opentea/examples/calculator/startup.py
 src/opentea/examples/calculator/updatde3dscene_1.py
+src/opentea/examples/calculator/__pycache__/__init__.cpython-311.pyc
 src/opentea/examples/calculator/__pycache__/__init__.cpython-39.pyc
+src/opentea/examples/calculator/__pycache__/startup.cpython-311.pyc
 src/opentea/examples/calculator/__pycache__/startup.cpython-39.pyc
 src/opentea/examples/simple/.tmp_docu.html
 src/opentea/examples/simple/__init__.py
 src/opentea/examples/simple/process_controleifreq.py
 src/opentea/examples/simple/schema_simple.yaml
 src/opentea/examples/simple/startup.py
 src/opentea/examples/simple/test-pattern-tv.jpg
 src/opentea/examples/simple/test.png
 src/opentea/examples/simple/test.py
 src/opentea/examples/simple/vegetable-icon-png-16.png
+src/opentea/examples/simple/__pycache__/__init__.cpython-311.pyc
 src/opentea/examples/simple/__pycache__/__init__.cpython-39.pyc
+src/opentea/examples/simple/__pycache__/startup.cpython-311.pyc
 src/opentea/examples/simple/__pycache__/startup.cpython-39.pyc
 src/opentea/examples/trivial/__init__.py
 src/opentea/examples/trivial/custom_callback.py
 src/opentea/examples/trivial/dataset_from_gui.yml
 src/opentea/examples/trivial/dataset_to_gui.yml
 src/opentea/examples/trivial/schema_trivial.yaml
 src/opentea/examples/trivial/startup.py
+src/opentea/examples/trivial/__pycache__/__init__.cpython-311.pyc
 src/opentea/examples/trivial/__pycache__/__init__.cpython-39.pyc
+src/opentea/examples/trivial/__pycache__/startup.cpython-311.pyc
 src/opentea/examples/trivial/__pycache__/startup.cpython-39.pyc
 src/opentea/gui_forms/__init__.py
 src/opentea/gui_forms/_base.py
 src/opentea/gui_forms/_exceptions.py
 src/opentea/gui_forms/constants.py
 src/opentea/gui_forms/generic_widgets.py
 src/opentea/gui_forms/leaf_widgets.py
@@ -56,27 +65,41 @@
 src/opentea/gui_forms/node_widgets.py
 src/opentea/gui_forms/otinker.py
 src/opentea/gui_forms/root_widget.py
 src/opentea/gui_forms/soundboard.py
 src/opentea/gui_forms/utils.py
 src/opentea/gui_forms/viewer_2d.py
 src/opentea/gui_forms/viewer_3d.py
+src/opentea/gui_forms/__pycache__/__init__.cpython-311.pyc
 src/opentea/gui_forms/__pycache__/__init__.cpython-39.pyc
+src/opentea/gui_forms/__pycache__/_base.cpython-311.pyc
 src/opentea/gui_forms/__pycache__/_base.cpython-39.pyc
+src/opentea/gui_forms/__pycache__/_exceptions.cpython-311.pyc
 src/opentea/gui_forms/__pycache__/_exceptions.cpython-39.pyc
+src/opentea/gui_forms/__pycache__/constants.cpython-311.pyc
 src/opentea/gui_forms/__pycache__/constants.cpython-39.pyc
+src/opentea/gui_forms/__pycache__/generic_widgets.cpython-311.pyc
 src/opentea/gui_forms/__pycache__/generic_widgets.cpython-39.pyc
+src/opentea/gui_forms/__pycache__/leaf_widgets.cpython-311.pyc
 src/opentea/gui_forms/__pycache__/leaf_widgets.cpython-39.pyc
+src/opentea/gui_forms/__pycache__/menus.cpython-311.pyc
 src/opentea/gui_forms/__pycache__/menus.cpython-39.pyc
+src/opentea/gui_forms/__pycache__/node_widgets.cpython-311.pyc
 src/opentea/gui_forms/__pycache__/node_widgets.cpython-39.pyc
+src/opentea/gui_forms/__pycache__/otinker.cpython-311.pyc
 src/opentea/gui_forms/__pycache__/otinker.cpython-39.pyc
+src/opentea/gui_forms/__pycache__/root_widget.cpython-311.pyc
 src/opentea/gui_forms/__pycache__/root_widget.cpython-39.pyc
+src/opentea/gui_forms/__pycache__/soundboard.cpython-311.pyc
 src/opentea/gui_forms/__pycache__/soundboard.cpython-39.pyc
+src/opentea/gui_forms/__pycache__/utils.cpython-311.pyc
 src/opentea/gui_forms/__pycache__/utils.cpython-39.pyc
+src/opentea/gui_forms/__pycache__/viewer_2d.cpython-311.pyc
 src/opentea/gui_forms/__pycache__/viewer_2d.cpython-39.pyc
+src/opentea/gui_forms/__pycache__/viewer_3d.cpython-311.pyc
 src/opentea/gui_forms/__pycache__/viewer_3d.cpython-39.pyc
 src/opentea/gui_forms/images/about_icon.gif
 src/opentea/gui_forms/images/docu_icon.gif
 src/opentea/gui_forms/images/help_icon.gif
 src/opentea/gui_forms/images/invalid_icon.gif
 src/opentea/gui_forms/images/load_icon.gif
 src/opentea/gui_forms/images/logo_opentea.gif
@@ -104,29 +127,46 @@
 src/opentea/noob/inferdefault.py
 src/opentea/noob/noob.py
 src/opentea/noob/schema.json
 src/opentea/noob/schema.py
 src/opentea/noob/utils.py
 src/opentea/noob/validate_light.py
 src/opentea/noob/validation.py
+src/opentea/noob/__pycache__/__init__.cpython-311.pyc
 src/opentea/noob/__pycache__/__init__.cpython-39.pyc
+src/opentea/noob/__pycache__/asciigraph.cpython-311.pyc
 src/opentea/noob/__pycache__/asciigraph.cpython-39.pyc
+src/opentea/noob/__pycache__/check_schema.cpython-311.pyc
 src/opentea/noob/__pycache__/check_schema.cpython-39.pyc
+src/opentea/noob/__pycache__/inferdefault.cpython-311.pyc
 src/opentea/noob/__pycache__/inferdefault.cpython-39.pyc
+src/opentea/noob/__pycache__/noob.cpython-311.pyc
 src/opentea/noob/__pycache__/noob.cpython-39.pyc
+src/opentea/noob/__pycache__/schema.cpython-311.pyc
 src/opentea/noob/__pycache__/schema.cpython-39.pyc
 src/opentea/noob/__pycache__/utils.cpython-39.pyc
+src/opentea/noob/__pycache__/validate_light.cpython-311.pyc
 src/opentea/noob/__pycache__/validate_light.cpython-39.pyc
+src/opentea/noob/__pycache__/validation.cpython-311.pyc
 src/opentea/noob/__pycache__/validation.cpython-39.pyc
 src/opentea/tools/__init__.py
 src/opentea/tools/proxy_h5.py
 src/opentea/tools/schema2md.py
 src/opentea/tools/visit_h5.py
 src/opentea/tools/__pycache__/__init__.cpython-39.pyc
 src/opentea/tools/__pycache__/proxy_h5.cpython-39.pyc
 src/opentea/tools/__pycache__/schema2md.cpython-39.pyc
 src/opentea/tools/__pycache__/visit_h5.cpython-39.pyc
 src/tkhtmlview/README.md
 src/tkhtmlview/__init__.py
 src/tkhtmlview/html_parser.py
+src/tkhtmlview/__pycache__/__init__.cpython-311.pyc
 src/tkhtmlview/__pycache__/__init__.cpython-39.pyc
-src/tkhtmlview/__pycache__/html_parser.cpython-39.pyc
+src/tkhtmlview/__pycache__/html_parser.cpython-311.pyc
+src/tkhtmlview/__pycache__/html_parser.cpython-39.pyc
+tests/test_guiform.py
+tests/test_infer.py
+tests/test_noob.py
+tests/test_proxyh5.py
+tests/test_schema2md.py
+tests/test_units.py
+tests/test_validate.py
```

### Comparing `OpenTEA-3.5.0/src/gallery/trivial.png` & `OpenTEA-3.6.0/src/gallery/trivial.png`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/.DS_Store` & `OpenTEA-3.6.0/src/opentea/.DS_Store`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/__pycache__/cli.cpython-39.pyc` & `OpenTEA-3.6.0/src/opentea/__pycache__/cli.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/__pycache__/process_utils.cpython-39.pyc` & `OpenTEA-3.6.0/src/opentea/__pycache__/process_utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/cli.py` & `OpenTEA-3.6.0/src/opentea/cli.py`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/examples/calculator/__pycache__/startup.cpython-39.pyc` & `OpenTEA-3.6.0/src/opentea/examples/calculator/__pycache__/startup.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/examples/calculator/callback_tab1.py` & `OpenTEA-3.6.0/src/opentea/examples/calculator/callback_tab1.py`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/examples/calculator/dataset_from_gui.yml` & `OpenTEA-3.6.0/src/opentea/examples/calculator/dataset_from_gui.yml`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/examples/calculator/schema_calculator.yaml` & `OpenTEA-3.6.0/src/opentea/examples/calculator/schema_calculator.yaml`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/examples/calculator/startup.py` & `OpenTEA-3.6.0/src/opentea/examples/calculator/startup.py`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/examples/calculator/updatde3dscene_1.py` & `OpenTEA-3.6.0/src/opentea/examples/calculator/updatde3dscene_1.py`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/examples/dataset_to_gui.yml` & `OpenTEA-3.6.0/src/opentea/examples/dataset_to_gui.yml`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/examples/simple/__pycache__/startup.cpython-39.pyc` & `OpenTEA-3.6.0/src/opentea/examples/simple/__pycache__/startup.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/examples/simple/process_controleifreq.py` & `OpenTEA-3.6.0/src/opentea/examples/simple/process_controleifreq.py`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/examples/simple/schema_simple.yaml` & `OpenTEA-3.6.0/src/opentea/examples/simple/schema_simple.yaml`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/examples/simple/startup.py` & `OpenTEA-3.6.0/src/opentea/examples/simple/startup.py`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/examples/simple/test-pattern-tv.jpg` & `OpenTEA-3.6.0/src/opentea/examples/simple/test-pattern-tv.jpg`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/examples/simple/test.png` & `OpenTEA-3.6.0/src/opentea/examples/simple/test.png`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/examples/simple/test.py` & `OpenTEA-3.6.0/src/opentea/examples/simple/test.py`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/examples/simple/vegetable-icon-png-16.png` & `OpenTEA-3.6.0/src/opentea/examples/simple/vegetable-icon-png-16.png`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/examples/trivial/__pycache__/startup.cpython-39.pyc` & `OpenTEA-3.6.0/src/opentea/examples/trivial/__pycache__/startup.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/examples/trivial/custom_callback.py` & `OpenTEA-3.6.0/src/opentea/examples/trivial/custom_callback.py`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/examples/trivial/schema_trivial.yaml` & `OpenTEA-3.6.0/src/opentea/examples/trivial/schema_trivial.yaml`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/examples/trivial/startup.py` & `OpenTEA-3.6.0/src/opentea/examples/trivial/startup.py`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/gui_forms/__pycache__/_base.cpython-39.pyc` & `OpenTEA-3.6.0/src/opentea/gui_forms/__pycache__/_base.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/gui_forms/__pycache__/_exceptions.cpython-39.pyc` & `OpenTEA-3.6.0/src/opentea/gui_forms/__pycache__/_exceptions.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/gui_forms/__pycache__/constants.cpython-39.pyc` & `OpenTEA-3.6.0/src/opentea/gui_forms/__pycache__/constants.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/gui_forms/__pycache__/generic_widgets.cpython-39.pyc` & `OpenTEA-3.6.0/src/opentea/gui_forms/__pycache__/generic_widgets.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/gui_forms/__pycache__/leaf_widgets.cpython-39.pyc` & `OpenTEA-3.6.0/src/opentea/gui_forms/__pycache__/leaf_widgets.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Feb  2 11:22:40 2023 UTC, .py size: 43168 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 009d db63 a0a8 0000  a..........c....
+00000000: 610d 0d0a 0000 0000 41a6 db63 4da8 0000  a.......A..cM...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 4002 0000 6400  .....@...s@...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6403 6c04 6d05 5a05 6d06 5a06  Z.d.d.l.m.Z.m.Z.
 00000060: 6d07 5a07 6d08 5a08 6d09 5a09 6d0a 5a0a  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e  m.Z.m.Z.m.Z.m.Z.
@@ -565,16 +565,16 @@
 00002340: 5300 2913 4ee9 0200 0000 a901 7231 0000  S.).N.......r1..
 00002350: 0072 3b00 0000 727b 0000 0072 4000 0000  .r;...r{...r@...
 00002360: da02 7365 fa0d 6e6f 2073 7461 7475 7320  ..se..no status 
 00002370: 7965 74fa 0d53 7461 7475 732e 544c 6162  yet..Status.TLab
 00002380: 656c da04 6c65 6674 a903 723c 0000 00da  el..left..r<....
 00002390: 0573 7479 6c65 da08 636f 6d70 6f75 6e64  .style..compound
 000023a0: da07 6d69 6e69 6d75 6dda 0369 6e66 da07  ..minimum..inf..
-000023b0: 6d61 7869 6d75 6d5a 1065 7863 6c75 7369  maximumZ.exclusi
-000023c0: 7665 4d69 6e69 6d75 6d46 5a10 6578 636c  veMinimumFZ.excl
+000023b0: 6d61 7869 6d75 6dda 1065 7863 6c75 7369  maximum..exclusi
+000023c0: 7665 4d69 6e69 6d75 6d46 da10 6578 636c  veMinimumF..excl
 000023d0: 7573 6976 654d 6178 696d 756d 727a 0000  usiveMaximumrz..
 000023e0: 0072 3f00 0000 290e 7245 0000 00da 0663  .r?...).rE.....c
 000023f0: 6f6e 6669 6772 1300 0000 727e 0000 0072  onfigr....r~...r
 00002400: 4b00 0000 724a 0000 0072 0200 0000 7248  K...rJ...r....rH
 00002410: 0000 00da 0b5f 7374 6174 7573 5f6c 626c  ....._status_lbl
 00002420: 7220 0000 0072 2100 0000 da05 666c 6f61  r ...r!.....floa
 00002430: 74da 075f 626f 756e 6473 da11 5f65 7863  t.._bounds.._exc
@@ -585,15 +585,15 @@
 00002480: ff06 020c 010c ff06 037a 245f 4f54 4e75  .........z$_OTNu
 00002490: 6d65 7269 6345 6e74 7279 2e5f 636f 6e66  mericEntry._conf
 000024a0: 6967 5f73 7461 7475 735f 6c61 6265 6c63  ig_status_labelc
 000024b0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
 000024c0: 0400 0000 4300 0000 7314 0000 007c 006a  ....C...s....|.j
 000024d0: 006a 0164 0164 0164 028d 0201 0064 0053  .j.d.d.d.....d.S
 000024e0: 0029 034e 7254 0000 00a9 0272 3c00 0000  .).NrT.....r<...
-000024f0: da05 696d 6167 6529 0272 9700 0000 7296  ..image).r....r.
+000024f0: da05 696d 6167 6529 0272 9900 0000 7298  ..image).r....r.
 00002500: 0000 0072 4d00 0000 722e 0000 0072 2e00  ...rM...r....r..
 00002510: 0000 722f 0000 00da 135f 7265 7365 745f  ..r/....._reset_
 00002520: 7374 6174 7573 5f6c 6162 656c 3101 0000  status_label1...
 00002530: 7302 0000 0000 017a 235f 4f54 4e75 6d65  s......z#_OTNume
 00002540: 7269 6345 6e74 7279 2e5f 7265 7365 745f  ricEntry._reset_
 00002550: 7374 6174 7573 5f6c 6162 656c 6301 0000  status_labelc...
 00002560: 0000 0000 0000 0000 0002 0000 0004 0000  ................
@@ -607,15 +607,15 @@
 000025e0: 6a00 6408 1900 7d01 7c00 6a02 6406 1900  j.d...}.|.j.d...
 000025f0: 7294 7c00 6a03 6405 6b02 728c 7c01 6406  r.|.j.d.k.r.|.d.
 00002600: 3800 7d01 6e08 7c01 6409 3900 7d01 7c01  8.}.n.|.d.9.}.|.
 00002610: 5300 290a 4e72 5300 0000 723e 0000 0072  S.).NrS...r>...r
 00002620: 9300 0000 7201 0000 00da 0769 6e74 6567  ....r......integ
 00002630: 6572 7234 0000 0067 9a99 9999 9999 f13f  err4...g.......?
 00002640: 7295 0000 00e7 cdcc cccc cccc ec3f 2904  r............?).
-00002650: 7220 0000 0072 2100 0000 729a 0000 00da  r ...r!...r.....
+00002650: 7220 0000 0072 2100 0000 729c 0000 00da  r ...r!...r.....
 00002660: 055f 7479 7065 7271 0000 0072 2e00 0000  ._typerq...r....
 00002670: 722e 0000 0072 2f00 0000 7252 0000 0034  r....r/...rR...4
 00002680: 0100 0073 2200 0000 0001 0e02 0801 0403  ...s"...........
 00002690: 0401 0a01 0a01 0a01 0a01 0a02 0a01 0a01  ................
 000026a0: 0a01 0a01 0a01 0a02 0802 7a1c 5f4f 544e  ..........z._OTN
 000026b0: 756d 6572 6963 456e 7472 792e 5f67 6574  umericEntry._get
 000026c0: 5f64 6566 6175 6c74 6302 0000 0000 0000  _defaultc.......
@@ -626,38 +626,38 @@
 00002710: 7065 4d01 0000 7302 0000 0000 027a 185f  peM...s......z._
 00002720: 4f54 4e75 6d65 7269 6345 6e74 7279 2e73  OTNumericEntry.s
 00002730: 7472 3274 7970 6563 0100 0000 0000 0000  tr2typec........
 00002740: 0000 0000 0100 0000 0200 0000 0300 0000  ................
 00002750: 7320 0000 0074 0083 00a0 01a1 0001 007c  s ...t.........|
 00002760: 006a 0264 016b 0572 1c7c 00a0 03a1 0001  .j.d.k.r.|......
 00002770: 0064 0053 0029 024e 7201 0000 0029 0472  .d.S.).Nr....).r
-00002780: 1e00 0000 725f 0000 0072 5700 0000 729d  ....r_...rW...r.
+00002780: 1e00 0000 725f 0000 0072 5700 0000 729f  ....r_...rW...r.
 00002790: 0000 0072 4d00 0000 722c 0000 0072 2e00  ...rM...r,...r..
 000027a0: 0000 722f 0000 0072 5f00 0000 5101 0000  ..r/...r_...Q...
 000027b0: 7306 0000 0000 010a 010a 017a 205f 4f54  s..........z _OT
 000027c0: 4e75 6d65 7269 6345 6e74 7279 2e6f 6e5f  NumericEntry.on_
 000027d0: 7570 6461 7465 5f73 7461 7475 7363 0100  update_statusc..
 000027e0: 0000 0000 0000 0000 0000 0100 0000 0800  ................
 000027f0: 0000 4300 0000 7330 0000 007a 127c 00a0  ..C...s0...z.|..
 00002800: 007c 006a 01a0 02a1 00a1 0157 0053 0004  .|.j.......W.S..
 00002810: 0074 0379 2a01 0001 0001 0074 0483 0082  .t.y*......t....
 00002820: 0159 006e 0230 0064 0053 0072 4c00 0000  .Y.n.0.d.S.rL...
-00002830: a905 72a1 0000 0072 6d00 0000 7221 0000  ..r....rm...r!..
+00002830: a905 72a3 0000 0072 6d00 0000 7221 0000  ..r....rm...r!..
 00002840: 00da 0a56 616c 7565 4572 726f 7272 0f00  ...ValueErrorr..
 00002850: 0000 724d 0000 0072 2e00 0000 722e 0000  ..rM...r....r...
 00002860: 0072 2f00 0000 7221 0000 0056 0100 0073  .r/...r!...V...s
 00002870: 0800 0000 0001 0201 1201 0c01 7a13 5f4f  ............z._O
 00002880: 544e 756d 6572 6963 456e 7472 792e 6765  TNumericEntry.ge
 00002890: 7463 0200 0000 0000 0000 0000 0000 0200  tc..............
 000028a0: 0000 0800 0000 4300 0000 7338 0000 007a  ......C...s8...z
 000028b0: 1a7c 00a0 007c 01a1 017d 017c 006a 01a0  .|...|...}.|.j..
 000028c0: 027c 01a1 0101 0057 006e 1804 0074 0379  .|.....W.n...t.y
 000028d0: 3201 0001 0001 0074 0483 0082 0159 006e  2......t.....Y.n
-000028e0: 0230 0064 0053 0072 4c00 0000 2905 72a1  .0.d.S.rL...).r.
-000028f0: 0000 0072 6d00 0000 7251 0000 0072 a300  ...rm...rQ...r..
+000028e0: 0230 0064 0053 0072 4c00 0000 2905 72a3  .0.d.S.rL...).r.
+000028f0: 0000 0072 6d00 0000 7251 0000 0072 a500  ...rm...rQ...r..
 00002900: 0000 7210 0000 0072 7100 0000 722e 0000  ..r....rq...r...
 00002910: 0072 2e00 0000 722f 0000 0072 5100 0000  .r....r/...rQ...
 00002920: 5c01 0000 730a 0000 0000 0102 010a 0110  \...s...........
 00002930: 020c 017a 135f 4f54 4e75 6d65 7269 6345  ...z._OTNumericE
 00002940: 6e74 7279 2e73 6574 6301 0000 0000 0000  ntry.setc.......
 00002950: 0000 0000 0003 0000 0003 0000 0047 0000  .............G..
 00002960: 0073 4a00 0000 7c00 a000 a100 7d02 7c02  .sJ...|.....}.|.
@@ -684,26 +684,26 @@
 00002ab0: 6e02 3000 6400 5300 a903 4e7a 0f49 6e76  n.0.d.S...Nz.Inv
 00002ac0: 616c 6964 2069 6e70 7574 2022 fa01 2229  alid input "..")
 00002ad0: 0472 2100 0000 720f 0000 0072 7e00 0000  .r!...r....r~...
 00002ae0: da1c 5f75 7064 6174 655f 696e 7661 6c69  .._update_invali
 00002af0: 645f 7374 6174 7573 5f6c 6162 656c a902  d_status_label..
 00002b00: 7229 0000 00da 0965 7272 6f72 5f6d 7367  r).....error_msg
 00002b10: 722e 0000 0072 2e00 0000 722f 0000 0072  r....r....r/...r
-00002b20: a400 0000 7701 0000 730c 0000 0000 0302  ....w...s.......
+00002b20: a600 0000 7701 0000 730c 0000 0000 0302  ....w...s.......
 00002b30: 010a 010c 0112 0110 027a 1b5f 4f54 4e75  .........z._OTNu
 00002b40: 6d65 7269 6345 6e74 7279 2e5f 6368 6563  mericEntry._chec
 00002b50: 6b5f 7479 7065 6302 0000 0000 0000 0000  k_typec.........
 00002b60: 0000 0003 0000 0003 0000 0043 0000 0073  ...........C...s
 00002b70: 2000 0000 7c00 a000 7c01 a101 7d02 7c02   ...|...|...}.|.
 00002b80: 721c 7c00 a001 7c02 a101 0100 6401 5300  r.|...|.....d.S.
 00002b90: 6402 5300 2903 4e46 5429 02da 0d5f 6368  d.S.).NFT)..._ch
-00002ba0: 6563 6b5f 626f 756e 6473 72a9 0000 0029  eck_boundsr....)
-00002bb0: 0372 2900 0000 7272 0000 0072 ab00 0000  .r)...rr...r....
+00002ba0: 6563 6b5f 626f 756e 6473 72ab 0000 0029  eck_boundsr....)
+00002bb0: 0372 2900 0000 7272 0000 0072 ad00 0000  .r)...rr...r....
 00002bc0: 722e 0000 0072 2e00 0000 722f 0000 0072  r....r....r/...r
-00002bd0: a600 0000 8201 0000 730a 0000 0000 020a  ........s.......
+00002bd0: a800 0000 8201 0000 730a 0000 0000 020a  ........s.......
 00002be0: 0104 010a 0104 027a 1f5f 4f54 4e75 6d65  .......z._OTNume
 00002bf0: 7269 6345 6e74 7279 2e5f 7661 6c69 6461  ricEntry._valida
 00002c00: 7465 5f76 616c 7565 6302 0000 0000 0000  te_valuec.......
 00002c10: 0000 0000 0008 0000 0005 0000 0043 0000  .............C..
 00002c20: 0073 6e00 0000 6401 6402 6702 7d02 7400  .sn...d.d.g.}.t.
 00002c30: 6a01 7400 6a02 6702 7d03 7403 7c00 6a04  j.t.j.g.}.t.|.j.
 00002c40: 7c00 6a05 7c03 7c02 8304 4400 5d42 5c04  |.j.|.|...D.]B\.
@@ -712,83 +712,83 @@
 00002c70: 6403 7c05 7254 6404 6e02 6405 9b00 7c07  d.|.rTd.n.d...|.
 00002c80: 9b00 7c04 9b00 9d04 0200 0100 5300 7126  ..|.........S.q&
 00002c90: 6405 5300 2906 7a1a 5661 6c69 6461 7465  d.S.).z.Validate
 00002ca0: 2072 756c 6573 206f 6e20 656e 7472 6965   rules on entrie
 00002cb0: 732e fa01 3cfa 013e 7a09 496e 7661 6c69  s...<..>z.Invali
 00002cc0: 643a 20fa 013d 7254 0000 0029 06da 086f  d: ..=rT...)...o
 00002cd0: 7065 7261 746f 72da 026c 65da 0267 65da  perator..le..ge.
-00002ce0: 037a 6970 7299 0000 0072 9a00 0000 2908  .zipr....r....).
+00002ce0: 037a 6970 729b 0000 0072 9c00 0000 2908  .zipr....r....).
 00002cf0: 7229 0000 0072 7200 0000 5a0d 7374 725f  r)...rr...Z.str_
-00002d00: 6f70 6572 6174 6f72 735a 096f 7065 7261  operatorsZ.opera
-00002d10: 746f 7273 5a03 6c69 6d5a 0965 7863 6c75  torsZ.limZ.exclu
+00002d00: 6f70 6572 6174 6f72 73da 096f 7065 7261  operators..opera
+00002d10: 746f 7273 da03 6c69 6dda 0965 7863 6c75  tors..lim..exclu
 00002d20: 7369 7665 5a09 6f70 6572 6174 6f72 5f5a  siveZ.operator_Z
 00002d30: 0c73 7472 5f6f 7065 7261 746f 7272 2e00  .str_operatorr..
-00002d40: 0000 722e 0000 0072 2f00 0000 72ac 0000  ..r....r/...r...
+00002d40: 0000 722e 0000 0072 2f00 0000 72ae 0000  ..r....r/...r...
 00002d50: 008b 0100 0073 1400 0000 0002 0801 0c01  .....s..........
 00002d60: 0201 0cff 1002 0a01 0c01 0202 2002 7a1d  ............ .z.
 00002d70: 5f4f 544e 756d 6572 6963 456e 7472 792e  _OTNumericEntry.
 00002d80: 5f63 6865 636b 5f62 6f75 6e64 7363 0200  _check_boundsc..
 00002d90: 0000 0000 0000 0000 0000 0200 0000 0400  ................
 00002da0: 0000 4300 0000 731e 0000 007c 006a 006a  ..C...s....|.j.j
 00002db0: 017c 0174 0264 0119 0064 028d 0201 0064  .|.t.d...d.....d
 00002dc0: 037c 005f 0364 0053 0029 044e da07 696e  .|._.d.S.).N..in
-00002dd0: 7661 6c69 6472 9b00 0000 e9ff ffff ff29  validr.........)
-00002de0: 0472 9700 0000 7296 0000 0072 1400 0000  .r....r....r....
-00002df0: 7257 0000 0072 aa00 0000 722e 0000 0072  rW...r....r....r
-00002e00: 2e00 0000 722f 0000 0072 a900 0000 9901  ....r/...r......
+00002dd0: 7661 6c69 6472 9d00 0000 e9ff ffff ff29  validr.........)
+00002de0: 0472 9900 0000 7298 0000 0072 1400 0000  .r....r....r....
+00002df0: 7257 0000 0072 ac00 0000 722e 0000 0072  rW...r....r....r
+00002e00: 2e00 0000 722f 0000 0072 ab00 0000 9901  ....r/...r......
 00002e10: 0000 7308 0000 0000 0106 0108 ff06 027a  ..s............z
 00002e20: 2c5f 4f54 4e75 6d65 7269 6345 6e74 7279  ,_OTNumericEntry
 00002e30: 2e5f 7570 6461 7465 5f69 6e76 616c 6964  ._update_invalid
 00002e40: 5f73 7461 7475 735f 6c61 6265 6c29 1372  _status_label).r
 00002e50: 6300 0000 7264 0000 0072 6500 0000 7226  c...rd...re...r&
-00002e60: 0000 0072 8900 0000 729d 0000 0072 5200  ...r....r....rR.
+00002e60: 0000 0072 8900 0000 729f 0000 0072 5200  ...r....r....rR.
 00002e70: 0000 da03 6162 63da 0e61 6273 7472 6163  ....abc..abstrac
-00002e80: 746d 6574 686f 6472 a100 0000 725f 0000  tmethodr....r_..
+00002e80: 746d 6574 686f 6472 a300 0000 725f 0000  tmethodr....r_..
 00002e90: 0072 2100 0000 7251 0000 0072 5c00 0000  .r!...rQ...r\...
-00002ea0: 72a4 0000 0072 a600 0000 72ac 0000 0072  r....r....r....r
-00002eb0: a900 0000 7267 0000 0072 2e00 0000 722e  ....rg...r....r.
+00002ea0: 72a6 0000 0072 a800 0000 72ae 0000 0072  r....r....r....r
+00002eb0: ab00 0000 7267 0000 0072 2e00 0000 722e  ....rg...r....r.
 00002ec0: 0000 0072 2c00 0000 722f 0000 0072 8800  ...r,...r/...r..
 00002ed0: 0000 1b01 0000 731c 0000 0008 020c 0408  ......s.........
 00002ee0: 1008 0308 1904 010a 030c 0508 0608 0808  ................
 00002ef0: 1308 0b08 0908 0e72 8800 0000 6300 0000  .......r....c...
 00002f00: 0000 0000 0000 0000 0000 0000 0002 0000  ................
 00002f10: 0040 0000 0073 1400 0000 6500 5a01 6400  .@...s....e.Z.d.
 00002f20: 5a02 6401 6402 8400 5a03 6403 5300 2904  Z.d.d...Z.d.S.).
 00002f30: da09 4f54 496e 7465 6765 7263 0200 0000  ..OTIntegerc....
 00002f40: 0000 0000 0000 0000 0200 0000 0200 0000  ................
 00002f50: 4300 0000 7308 0000 0074 007c 0183 0153  C...s....t.|...S
 00002f60: 0072 4c00 0000 2901 7249 0000 0072 7100  .rL...).rI...rq.
 00002f70: 0000 722e 0000 0072 2e00 0000 722f 0000  ..r....r....r/..
-00002f80: 0072 a100 0000 a101 0000 7302 0000 0000  .r........s.....
+00002f80: 0072 a300 0000 a101 0000 7302 0000 0000  .r........s.....
 00002f90: 017a 124f 5449 6e74 6567 6572 2e73 7472  .z.OTInteger.str
 00002fa0: 3274 7970 654e a904 7263 0000 0072 6400  2typeN..rc...rd.
-00002fb0: 0000 7265 0000 0072 a100 0000 722e 0000  ..re...r....r...
+00002fb0: 0000 7265 0000 0072 a300 0000 722e 0000  ..re...r....r...
 00002fc0: 0072 2e00 0000 722e 0000 0072 2f00 0000  .r....r....r/...
-00002fd0: 72b8 0000 009f 0100 0073 0200 0000 0802  r........s......
-00002fe0: 72b8 0000 0063 0000 0000 0000 0000 0000  r....c..........
+00002fd0: 72bd 0000 009f 0100 0073 0200 0000 0802  r........s......
+00002fe0: 72bd 0000 0063 0000 0000 0000 0000 0000  r....c..........
 00002ff0: 0000 0000 0000 0100 0000 4000 0000 730c  ..........@...s.
 00003000: 0000 0065 005a 0164 005a 0264 0153 0029  ...e.Z.d.Z.d.S.)
 00003010: 02da 084f 5453 7472 696e 674e 2903 7263  ...OTStringN).rc
 00003020: 0000 0072 6400 0000 7265 0000 0072 2e00  ...rd...re...r..
 00003030: 0000 722e 0000 0072 2e00 0000 722f 0000  ..r....r....r/..
-00003040: 0072 ba00 0000 a501 0000 7302 0000 0008  .r........s.....
-00003050: 0172 ba00 0000 6300 0000 0000 0000 0000  .r....c.........
+00003040: 0072 bf00 0000 a501 0000 7302 0000 0008  .r........s.....
+00003050: 0172 bf00 0000 6300 0000 0000 0000 0000  .r....c.........
 00003060: 0000 0000 0000 0002 0000 0040 0000 0073  ...........@...s
 00003070: 1400 0000 6500 5a01 6400 5a02 6401 6402  ....e.Z.d.Z.d.d.
 00003080: 8400 5a03 6403 5300 2904 da08 4f54 4e75  ..Z.d.S.)...OTNu
 00003090: 6d62 6572 6302 0000 0000 0000 0000 0000  mberc...........
 000030a0: 0002 0000 0002 0000 0043 0000 0073 0800  .........C...s..
 000030b0: 0000 7400 7c01 8301 5300 724c 0000 0029  ..t.|...S.rL...)
-000030c0: 0172 9800 0000 7271 0000 0072 2e00 0000  .r....rq...r....
-000030d0: 722e 0000 0072 2f00 0000 72a1 0000 00ab  r....r/...r.....
+000030c0: 0172 9a00 0000 7271 0000 0072 2e00 0000  .r....rq...r....
+000030d0: 722e 0000 0072 2f00 0000 72a3 0000 00ab  r....r/...r.....
 000030e0: 0100 0073 0200 0000 0001 7a11 4f54 4e75  ...s......z.OTNu
-000030f0: 6d62 6572 2e73 7472 3274 7970 654e 72b9  mber.str2typeNr.
+000030f0: 6d62 6572 2e73 7472 3274 7970 654e 72be  mber.str2typeNr.
 00003100: 0000 0072 2e00 0000 722e 0000 0072 2e00  ...r....r....r..
-00003110: 0000 722f 0000 0072 bb00 0000 a901 0000  ..r/...r........
-00003120: 7302 0000 0008 0272 bb00 0000 6300 0000  s......r....c...
+00003110: 0000 722f 0000 0072 c000 0000 a901 0000  ..r/...r........
+00003120: 7302 0000 0008 0272 c000 0000 6300 0000  s......r....c...
 00003130: 0000 0000 0000 0000 0000 0000 0002 0000  ................
 00003140: 0040 0000 0073 3c00 0000 6500 5a01 6400  .@...s<...e.Z.d.
 00003150: 5a02 6401 6402 8400 5a03 6403 6404 8400  Z.d.d...Z.d.d...
 00003160: 5a04 6405 6406 8400 5a05 6407 6408 8400  Z.d.d...Z.d.d...
 00003170: 5a06 6409 640a 8400 5a07 640b 640c 8400  Z.d.d...Z.d.d...
 00003180: 5a08 640d 5300 290e da09 4f54 426f 6f6c  Z.d.S.)...OTBool
 00003190: 6561 6e63 0100 0000 0000 0000 0000 0000  eanc............
@@ -832,15 +832,15 @@
 000033f0: 0000 0000 017a 0d4f 5442 6f6f 6c65 616e  .....z.OTBoolean
 00003400: 2e67 6574 6302 0000 0000 0000 0000 0000  .getc...........
 00003410: 0002 0000 0008 0000 0043 0000 0073 3200  .........C...s2.
 00003420: 0000 7a14 7c00 6a00 a001 7402 7c01 8301  ..z.|.j...t.|...
 00003430: a101 0100 5700 6e18 0400 7403 792c 0100  ....W.n...t.y,..
 00003440: 0100 0100 7404 8300 8201 5900 6e02 3000  ....t.....Y.n.0.
 00003450: 6400 5300 724c 0000 0029 0572 6d00 0000  d.S.rL...).rm...
-00003460: 7251 0000 00da 0462 6f6f 6c72 a300 0000  rQ.....boolr....
+00003460: 7251 0000 00da 0462 6f6f 6c72 a500 0000  rQ.....boolr....
 00003470: 7210 0000 0072 7100 0000 722e 0000 0072  r....rq...r....r
 00003480: 2e00 0000 722f 0000 0072 5100 0000 c201  ....r/...rQ.....
 00003490: 0000 7308 0000 0000 0102 0114 010c 017a  ..s............z
 000034a0: 0d4f 5442 6f6f 6c65 616e 2e73 6574 6301  .OTBoolean.setc.
 000034b0: 0000 0000 0000 0000 0000 0002 0000 0003  ................
 000034c0: 0000 0043 0000 0073 2400 0000 7c00 6a00  ...C...s$...|.j.
 000034d0: 6401 6b03 720e 6402 6e02 6403 7d01 7c00  d.k.r.d.n.d.}.|.
@@ -853,17 +853,17 @@
 00003540: 0000 722f 0000 0072 5e00 0000 c801 0000  ..r/...r^.......
 00003550: 7304 0000 0000 0112 017a 1f4f 5442 6f6f  s........z.OTBoo
 00003560: 6c65 616e 2e5f 7570 6461 7465 5f77 6964  lean._update_wid
 00003570: 6765 7473 5f73 7479 6c65 4e29 0972 6300  gets_styleN).rc.
 00003580: 0000 7264 0000 0072 6500 0000 7225 0000  ..rd...re...r%..
 00003590: 0072 2600 0000 7252 0000 0072 2100 0000  .r&...rR...r!...
 000035a0: 7251 0000 0072 5e00 0000 722e 0000 0072  rQ...r^...r....r
-000035b0: 2e00 0000 722e 0000 0072 2f00 0000 72bc  ....r....r/...r.
+000035b0: 2e00 0000 722e 0000 0072 2f00 0000 72c1  ....r....r/...r.
 000035c0: 0000 00af 0100 0073 0c00 0000 0802 0804  .......s........
-000035d0: 0807 0803 0803 0806 72bc 0000 0063 0000  ........r....c..
+000035d0: 0807 0803 0803 0806 72c1 0000 0063 0000  ........r....c..
 000035e0: 0000 0000 0000 0000 0000 0000 0000 0300  ................
 000035f0: 0000 0000 0000 734a 0000 0065 005a 0164  ......sJ...e.Z.d
 00003600: 005a 0287 0066 0164 0164 0284 085a 0364  .Z...f.d.d...Z.d
 00003610: 0364 0484 005a 0465 056a 0664 0564 0684  .d...Z.e.j.d.d..
 00003620: 0083 015a 0764 0764 0884 005a 0864 0964  ...Z.d.d...Z.d.d
 00003630: 0a84 005a 0964 0b64 0c84 005a 0a87 0004  ...Z.d.d...Z....
 00003640: 005a 0b53 0029 0dda 115f 4f54 4368 6f69  .Z.S.)..._OTChoi
@@ -918,51 +918,51 @@
 00003950: 0043 0000 0073 1000 0000 7c00 6a00 a001  .C...s....|.j...
 00003960: 7c01 a101 0100 6400 5300 724c 0000 0072  |.....d.S.rL...r
 00003970: 7000 0000 7271 0000 0072 2e00 0000 722e  p...rq...r....r.
 00003980: 0000 0072 2f00 0000 7251 0000 00e7 0100  ...r/...rQ......
 00003990: 0073 0200 0000 0001 7a15 5f4f 5443 686f  .s......z._OTCho
 000039a0: 6963 6541 6273 7472 6163 742e 7365 7429  iceAbstract.set)
 000039b0: 0c72 6300 0000 7264 0000 0072 6500 0000  .rc...rd...re...
-000039c0: 721f 0000 0072 2500 0000 72b6 0000 0072  r....r%...r....r
-000039d0: b700 0000 7226 0000 0072 5200 0000 7221  ....r&...rR...r!
+000039c0: 721f 0000 0072 2500 0000 72bb 0000 0072  r....r%...r....r
+000039d0: bc00 0000 7226 0000 0072 5200 0000 7221  ....r&...rR...r!
 000039e0: 0000 0072 5100 0000 7267 0000 0072 2e00  ...rQ...rg...r..
 000039f0: 0000 722e 0000 0072 2c00 0000 722f 0000  ..r....r,...r/..
-00003a00: 0072 c400 0000 cd01 0000 730e 0000 0008  .r........s.....
-00003a10: 030c 0408 0404 010a 0308 0808 0372 c400  .............r..
+00003a00: 0072 c900 0000 cd01 0000 730e 0000 0008  .r........s.....
+00003a10: 030c 0408 0404 010a 0308 0808 0372 c900  .............r..
 00003a20: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
 00003a30: 0000 0002 0000 0040 0000 0073 1400 0000  .......@...s....
 00003a40: 6500 5a01 6400 5a02 6401 6402 8400 5a03  e.Z.d.Z.d.d...Z.
 00003a50: 6403 5300 2904 da08 4f54 4368 6f69 6365  d.S.)...OTChoice
 00003a60: 6305 0000 0000 0000 0000 0000 0005 0000  c...............
 00003a70: 0005 0000 0043 0000 0073 5000 0000 6401  .....C...sP...d.
 00003a80: 7c01 7600 7236 7400 7c01 6401 1900 8301  |.v.r6t.|.d.....
 00003a90: 6402 6b04 7226 7401 7c01 7c02 7c03 7c04  d.k.r&t.|.|.|.|.
 00003aa0: 8304 5300 7402 7c01 7c02 7c03 7c04 8304  ..S.t.|.|.|.|...
 00003ab0: 5300 6e16 6403 7c01 7600 724c 7403 7c01  S.n.d.|.v.rLt.|.
 00003ac0: 7c02 7c03 7c04 8304 5300 6400 5300 2904  |.|.|...S.d.S.).
-00003ad0: 4e72 c600 0000 e905 0000 00da 0d6f 745f  Nr...........ot_
+00003ad0: 4e72 cb00 0000 e905 0000 00da 0d6f 745f  Nr...........ot_
 00003ae0: 6479 6e5f 6368 6f69 6365 2904 da03 6c65  dyn_choice)...le
 00003af0: 6eda 0e5f 4f54 4368 6f69 6365 436f 6d62  n.._OTChoiceComb
 00003b00: 6fda 0e5f 4f54 4368 6f69 6365 5261 6469  o.._OTChoiceRadi
 00003b10: 6fda 105f 4f54 4368 6f69 6365 4479 6e61  o.._OTChoiceDyna
 00003b20: 6d69 6372 2800 0000 722e 0000 0072 2e00  micr(...r....r..
 00003b30: 0000 722f 0000 00da 075f 5f6e 6577 5f5f  ..r/.....__new__
 00003b40: ed01 0000 730c 0000 0000 0208 0110 010e  ....s...........
 00003b50: 0210 0108 017a 104f 5443 686f 6963 652e  .....z.OTChoice.
 00003b60: 5f5f 6e65 775f 5f4e 2904 7263 0000 0072  __new__N).rc...r
-00003b70: 6400 0000 7265 0000 0072 ce00 0000 722e  d...re...r....r.
+00003b70: 6400 0000 7265 0000 0072 d300 0000 722e  d...re...r....r.
 00003b80: 0000 0072 2e00 0000 722e 0000 0072 2f00  ...r....r....r/.
-00003b90: 0000 72c7 0000 00eb 0100 0073 0200 0000  ..r........s....
-00003ba0: 0802 72c7 0000 0063 0000 0000 0000 0000  ..r....c........
+00003b90: 0000 72cc 0000 00eb 0100 0073 0200 0000  ..r........s....
+00003ba0: 0802 72cc 0000 0063 0000 0000 0000 0000  ..r....c........
 00003bb0: 0000 0000 0000 0000 0300 0000 0000 0000  ................
 00003bc0: 7344 0000 0065 005a 0164 005a 0287 0066  sD...e.Z.d.Z...f
 00003bd0: 0164 0164 0284 085a 0364 0364 0484 005a  .d.d...Z.d.d...Z
 00003be0: 0464 0564 0684 005a 0564 0764 0884 005a  .d.d...Z.d.d...Z
 00003bf0: 0664 0964 0a84 005a 0764 0b64 0c84 005a  .d.d...Z.d.d...Z
-00003c00: 0887 0004 005a 0953 0029 0d72 cc00 0000  .....Z.S.).r....
+00003c00: 0887 0004 005a 0953 0029 0d72 d100 0000  .....Z.S.).r....
 00003c10: 6305 0000 0000 0000 0000 0000 0005 0000  c...............
 00003c20: 0006 0000 0003 0000 0073 1c00 0000 6900  .........s....i.
 00003c30: 7c00 5f00 7401 8300 a002 7c01 7c02 7c03  |._.t.....|.|.|.
 00003c40: 7c04 a104 0100 6400 5300 724c 0000 0029  |.....d.S.rL...)
 00003c50: 03da 0872 6164 5f62 746e 7372 1e00 0000  ...rad_btnsr....
 00003c60: 721f 0000 0072 2800 0000 722c 0000 0072  r....r(...r,...r
 00003c70: 2e00 0000 722f 0000 0072 1f00 0000 fa01  ....r/...r......
@@ -990,1790 +990,1787 @@
 00003dd0: 7c03 6408 6409 8d03 0100 7c07 7c00 6a0d  |.d.d.....|.|.j.
 00003de0: 7c05 3c00 7c03 7c02 3700 7d03 715a 7c00  |.<.|.|.7.}.qZ|.
 00003df0: 6a03 6a0e 640a 640b 640c 8d02 0100 7c00  j.j.d.d.d.....|.
 00003e00: 6a0f 6a0c 6407 7410 6407 7c03 1400 8301  j.j.d.t.d.|.....
 00003e10: 640d 6409 8d03 0100 640e 5300 290f 7a21  d.d.....d.S.).z!
 00003e20: 5261 6469 6f62 7574 746f 6e20 7665 7273  Radiobutton vers
 00003e30: 696f 6e20 6f66 2074 6865 2077 6964 6765  ion of the widge
-00003e40: 7472 c600 0000 7234 0000 0072 8b00 0000  tr....r4...r....
-00003e50: 727a 0000 00da 0b65 6e75 6d5f 7469 746c  rz.....enum_titl
-00003e60: 6573 2904 723c 0000 0072 7200 0000 72be  es).r<...rr...r.
-00003e70: 0000 0072 bf00 0000 723b 0000 0072 7b00  ...r....r;...r{.
+00003e40: 7472 cb00 0000 7234 0000 0072 8b00 0000  tr....r4...r....
+00003e50: 727a 0000 005a 0b65 6e75 6d5f 7469 746c  rz...Z.enum_titl
+00003e60: 6573 2904 723c 0000 0072 7200 0000 72c3  es).r<...rr...r.
+00003e70: 0000 0072 c400 0000 723b 0000 0072 7b00  ...r....r;...r{.
 00003e80: 0000 7240 0000 00da 0673 756e 6b65 6e72  ..r@.....sunkenr
 00003e90: 8a00 0000 2902 da06 7265 6c69 6566 da07  ....)...relief..
-00003ea0: 7061 6464 696e 6772 bd00 0000 4e29 11da  paddingr....N)..
-00003eb0: 036d 6178 72ca 0000 0072 2000 0000 7245  .maxr....r ...rE
-00003ec0: 0000 0072 9600 0000 7213 0000 0072 2100  ...r....r....r!.
-00003ed0: 0000 72b3 0000 0072 0200 0000 da0b 5261  ..r....r......Ra
+00003ea0: 7061 6464 696e 6772 c200 0000 4e29 11da  paddingr....N)..
+00003eb0: 036d 6178 72cf 0000 0072 2000 0000 7245  .maxr....r ...rE
+00003ec0: 0000 0072 9800 0000 7213 0000 0072 2100  ...r....r....r!.
+00003ed0: 0000 72b5 0000 0072 0200 0000 da0b 5261  ..r....r......Ra
 00003ee0: 6469 6f62 7574 746f 6e72 6d00 0000 7218  diobuttonrm...r.
-00003ef0: 0000 0072 4b00 0000 72cf 0000 0072 8400  ...rK...r....r..
+00003ef0: 0000 0072 4b00 0000 72d4 0000 0072 8400  ...rK...r....r..
 00003f00: 0000 724a 0000 0072 4900 0000 2908 7229  ..rJ...rI...).r)
-00003f10: 0000 00da 076e 5f6c 696e 6573 5a08 7265  .....n_linesZ.re
+00003f10: 0000 00da 076e 5f6c 696e 6573 da08 7265  .....n_lines..re
 00003f20: 6c5f 7374 6570 5a0c 6375 7272 656e 745f  l_stepZ.current_
 00003f30: 7265 6c79 da06 7469 746c 6573 7272 0000  rely..titlesrr..
 00003f40: 0072 1a00 0000 da07 7261 645f 6274 6e72  .r......rad_btnr
-00003f50: 2e00 0000 722e 0000 0072 2f00 0000 72d0  ....r....r/...r.
+00003f50: 2e00 0000 722e 0000 0072 2f00 0000 72d5  ....r....r/...r.
 00003f60: 0000 0001 0200 0073 2c00 0000 0002 1401  .......s,.......
 00003f70: 1201 0801 0803 1402 1801 0401 0401 0201  ................
 00003f80: 0201 0401 02fb 0607 0401 0201 0201 02fd  ................
-00003f90: 0604 0a01 0a02 1001 7a26 5f4f 5443 686f  ........z&_OTCho
+00003f90: 0604 0a01 0a02 1002 7a26 5f4f 5443 686f  ........z&_OTCho
 00003fa0: 6963 6552 6164 696f 2e5f 7061 636b 5f77  iceRadio._pack_w
 00003fb0: 6974 685f 7261 6469 6f62 7574 746f 6e73  ith_radiobuttons
 00003fc0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
 00003fd0: 0002 0000 0043 0000 0073 2000 0000 7c00  .....C...s ...|.
 00003fe0: 6a00 6401 6b02 7214 7c00 a001 a100 0100  j.d.k.r.|.......
 00003ff0: 6e08 7c00 a002 a100 0100 6400 5300 725d  n.|.......d.S.r]
 00004000: 0000 0029 0372 5700 0000 da17 5f72 6573  ...).rW....._res
 00004010: 6574 5f62 6163 6b67 726f 756e 645f 636f  et_background_co
 00004020: 6c6f 72da 1b5f 6869 6768 6c69 6768 745f  lor.._highlight_
 00004030: 6261 636b 6772 6f75 6e64 5f63 6f6c 6f72  background_color
 00004040: 724d 0000 0072 2e00 0000 722e 0000 0072  rM...r....r....r
-00004050: 2f00 0000 725e 0000 001e 0200 0073 0600  /...r^.......s..
+00004050: 2f00 0000 725e 0000 001f 0200 0073 0600  /...r^.......s..
 00004060: 0000 0001 0a01 0a02 7a24 5f4f 5443 686f  ........z$_OTCho
 00004070: 6963 6552 6164 696f 2e5f 7570 6461 7465  iceRadio._update
 00004080: 5f77 6964 6765 7473 5f73 7479 6c65 6301  _widgets_stylec.
 00004090: 0000 0000 0000 0000 0000 0005 0000 0004  ................
 000040a0: 0000 0043 0000 0073 3c00 0000 7c00 a000  ...C...s<...|...
 000040b0: a100 7d01 7c00 6a01 a002 a100 4400 5d24  ..}.|.j.....D.]$
 000040c0: 5c02 7d02 7d03 7c02 7c01 6b02 7226 6401  \.}.}.|.|.k.r&d.
 000040d0: 6e02 6402 7d04 7c03 6a03 7c04 6403 8d01  n.d.}.|.j.|.d...
 000040e0: 0100 7112 6400 5300 2904 4e7a 1848 6967  ..q.d.S.).Nz.Hig
 000040f0: 686c 6967 6874 6564 2e54 5261 6469 6f62  hlighted.TRadiob
 00004100: 7574 746f 6eda 0c54 5261 6469 6f62 7574  utton..TRadiobut
-00004110: 746f 6e72 c200 0000 2904 7221 0000 0072  tonr....).r!...r
-00004120: cf00 0000 da05 6974 656d 7372 8400 0000  ......itemsr....
+00004110: 746f 6e72 c700 0000 2904 7221 0000 0072  tonr....).r!...r
+00004120: d400 0000 da05 6974 656d 7372 8400 0000  ......itemsr....
 00004130: 2905 7229 0000 00da 0376 616c 7222 0000  ).r).....valr"..
-00004140: 0072 d900 0000 7291 0000 0072 2e00 0000  .r....r....r....
-00004150: 722e 0000 0072 2f00 0000 72db 0000 0024  r....r/...r....$
+00004140: 0072 de00 0000 7291 0000 0072 2e00 0000  .r....r....r....
+00004150: 722e 0000 0072 2f00 0000 72e0 0000 0025  r....r/...r....%
 00004160: 0200 0073 0800 0000 0001 0801 1201 1001  ...s............
 00004170: 7a2a 5f4f 5443 686f 6963 6552 6164 696f  z*_OTChoiceRadio
 00004180: 2e5f 6869 6768 6c69 6768 745f 6261 636b  ._highlight_back
 00004190: 6772 6f75 6e64 5f63 6f6c 6f72 6301 0000  ground_colorc...
 000041a0: 0000 0000 0000 0000 0002 0000 0004 0000  ................
 000041b0: 0043 0000 0073 2000 0000 7c00 6a00 a001  .C...s ...|.j...
 000041c0: a100 4400 5d10 7d01 7c01 6a02 6401 6402  ..D.].}.|.j.d.d.
-000041d0: 8d01 0100 710a 6400 5300 2903 4e72 dc00  ....q.d.S.).Nr..
-000041e0: 0000 72c2 0000 0029 0372 cf00 0000 da06  ..r....).r......
+000041d0: 8d01 0100 710a 6400 5300 2903 4e72 e100  ....q.d.S.).Nr..
+000041e0: 0000 72c7 0000 0029 0372 d400 0000 da06  ..r....).r......
 000041f0: 7661 6c75 6573 7284 0000 0029 0272 2900  valuesr....).r).
-00004200: 0000 72d9 0000 0072 2e00 0000 722e 0000  ..r....r....r...
-00004210: 0072 2f00 0000 72da 0000 002a 0200 0073  .r/...r....*...s
+00004200: 0000 72de 0000 0072 2e00 0000 722e 0000  ..r....r....r...
+00004210: 0072 2f00 0000 72df 0000 002b 0200 0073  .r/...r....+...s
 00004220: 0400 0000 0001 0e01 7a26 5f4f 5443 686f  ........z&_OTCho
 00004230: 6963 6552 6164 696f 2e5f 7265 7365 745f  iceRadio._reset_
 00004240: 6261 636b 6772 6f75 6e64 5f63 6f6c 6f72  background_color
 00004250: 290a 7263 0000 0072 6400 0000 7265 0000  ).rc...rd...re..
-00004260: 0072 1f00 0000 7226 0000 0072 d000 0000  .r....r&...r....
-00004270: 725e 0000 0072 db00 0000 72da 0000 0072  r^...r....r....r
+00004260: 0072 1f00 0000 7226 0000 0072 d500 0000  .r....r&...r....
+00004270: 725e 0000 0072 e000 0000 72df 0000 0072  r^...r....r....r
 00004280: 6700 0000 722e 0000 0072 2e00 0000 722c  g...r....r....r,
-00004290: 0000 0072 2f00 0000 72cc 0000 00f8 0100  ...r/...r.......
-000042a0: 0073 0c00 0000 0802 0c04 0803 081d 0806  .s..............
-000042b0: 0806 72cc 0000 0063 0000 0000 0000 0000  ..r....c........
+00004290: 0000 0072 2f00 0000 72d1 0000 00f8 0100  ...r/...r.......
+000042a0: 0073 0c00 0000 0802 0c04 0803 081e 0806  .s..............
+000042b0: 0806 72d1 0000 0063 0000 0000 0000 0000  ..r....c........
 000042c0: 0000 0000 0000 0000 0200 0000 4000 0000  ............@...
 000042d0: 7328 0000 0065 005a 0164 005a 0264 015a  s(...e.Z.d.Z.d.Z
 000042e0: 0364 0264 0384 005a 0464 0464 0584 005a  .d.d...Z.d.d...Z
 000042f0: 0564 0664 0784 005a 0664 0853 0029 0972  .d.d...Z.d.S.).r
-00004300: cb00 0000 7a12 4f54 2063 686f 6963 6573  ....z.OT choices
+00004300: d000 0000 7a12 4f54 2063 686f 6963 6573  ....z.OT choices
 00004310: 2077 6964 6765 742e 6301 0000 0000 0000   widget.c.......
-00004320: 0000 0000 0003 0000 0005 0000 0043 0000  .............C..
-00004330: 0073 3000 0000 7c00 6a00 a001 6401 a101  .s0...|.j...d...
-00004340: 7d01 7c00 6a00 a001 6402 7c00 6a00 6401  }.|.j...d.|.j.d.
-00004350: 1900 a102 7d02 7c00 a002 7c01 7c02 a102  ....}.|...|.|...
-00004360: 0100 6400 5300 2903 4e72 c600 0000 72d1  ..d.S.).Nr....r.
-00004370: 0000 0029 0372 2000 0000 7221 0000 00da  ...).r ...r!....
-00004380: 135f 7061 636b 5f77 6974 685f 636f 6d62  ._pack_with_comb
-00004390: 6f62 6f78 2903 7229 0000 00da 076f 7074  obox).r).....opt
-000043a0: 696f 6e73 72d8 0000 0072 2e00 0000 722e  ionsr....r....r.
-000043b0: 0000 0072 2f00 0000 7226 0000 0032 0200  ...r/...r&...2..
-000043c0: 0073 0600 0000 0001 0c01 1401 7a1e 5f4f  .s..........z._O
-000043d0: 5443 686f 6963 6543 6f6d 626f 2e5f 6372  TChoiceCombo._cr
-000043e0: 6561 7465 5f77 6964 6765 7473 6303 0000  eate_widgetsc...
-000043f0: 0000 0000 0000 0000 0003 0000 0007 0000  ................
-00004400: 0043 0000 0073 3000 0000 7400 6a01 7c00  .C...s0...t.j.|.
-00004410: 6a02 7c01 7c00 6a03 6401 7404 6402 8d05  j.|.|.j.d.t.d...
-00004420: 7c00 5f05 7c00 6a05 6a06 6403 6404 6405  |._.|.j.j.d.d.d.
-00004430: 6406 8d03 0100 6407 5300 2908 7a1e 436f  d.....d.S.).z.Co
-00004440: 6d62 6f62 6f78 2076 6572 7369 6f6e 206f  mbobox version o
-00004450: 6620 7468 6520 7769 6467 6574 da08 7265  f the widget..re
-00004460: 6164 6f6e 6c79 2904 72df 0000 0072 7500  adonly).r....ru.
-00004470: 0000 721c 0000 005a 0b70 6f73 7463 6f6d  ..r....Z.postcom
-00004480: 6d61 6e64 723b 0000 0072 3400 0000 727b  mandr;...r4...r{
-00004490: 0000 0072 4000 0000 4e29 0772 0200 0000  ...r@...N).r....
-000044a0: da08 436f 6d62 6f62 6f78 7245 0000 0072  ..ComboboxrE...r
-000044b0: 6d00 0000 7218 0000 00da 0563 6f6d 626f  m...r......combo
-000044c0: 724b 0000 0029 0372 2900 0000 da06 6f70  rK...).r).....op
-000044d0: 7469 6f6e 72d8 0000 0072 2e00 0000 722e  tionr....r....r.
-000044e0: 0000 0072 2f00 0000 72e0 0000 0037 0200  ...r/...r....7..
-000044f0: 0073 1000 0000 0003 0401 0401 0201 0401  .s..............
-00004500: 0201 02fb 0806 7a22 5f4f 5443 686f 6963  ......z"_OTChoic
-00004510: 6543 6f6d 626f 2e5f 7061 636b 5f77 6974  eCombo._pack_wit
-00004520: 685f 636f 6d62 6f62 6f78 6301 0000 0000  h_comboboxc.....
-00004530: 0000 0000 0000 0002 0000 0003 0000 0043  ...............C
-00004540: 0000 0073 2400 0000 7c00 6a00 6401 6b02  ...s$...|.j.d.k.
-00004550: 720e 6402 6e02 6403 7d01 7c00 6a01 6a02  r.d.n.d.}.|.j.j.
-00004560: 7c01 6404 8d01 0100 6400 5300 2905 4e72  |.d.....d.S.).Nr
-00004570: 3400 0000 da09 5443 6f6d 626f 626f 787a  4.....TComboboxz
-00004580: 1548 6967 686c 6967 6874 6564 2e54 436f  .Highlighted.TCo
-00004590: 6d62 6f62 6f78 72c2 0000 0029 0372 5700  mboboxr....).rW.
-000045a0: 0000 72e4 0000 0072 8400 0000 72c3 0000  ..r....r....r...
-000045b0: 0072 2e00 0000 722e 0000 0072 2f00 0000  .r....r....r/...
-000045c0: 725e 0000 0042 0200 0073 0400 0000 0001  r^...B...s......
-000045d0: 1201 7a24 5f4f 5443 686f 6963 6543 6f6d  ..z$_OTChoiceCom
-000045e0: 626f 2e5f 7570 6461 7465 5f77 6964 6765  bo._update_widge
-000045f0: 7473 5f73 7479 6c65 4e29 0772 6300 0000  ts_styleN).rc...
-00004600: 7264 0000 0072 6500 0000 7266 0000 0072  rd...re...rf...r
-00004610: 2600 0000 72e0 0000 0072 5e00 0000 722e  &...r....r^...r.
-00004620: 0000 0072 2e00 0000 722e 0000 0072 2f00  ...r....r....r/.
-00004630: 0000 72cb 0000 002f 0200 0073 0800 0000  ..r..../...s....
-00004640: 0801 0402 0805 080b 72cb 0000 0063 0000  ........r....c..
-00004650: 0000 0000 0000 0000 0000 0000 0000 0300  ................
-00004660: 0000 0000 0000 7356 0000 0065 005a 0164  ......sV...e.Z.d
-00004670: 005a 0287 0066 0164 0164 0284 085a 0364  .Z...f.d.d...Z.d
-00004680: 0364 0484 005a 0464 0564 0684 005a 0564  .d...Z.d.d...Z.d
-00004690: 0764 0884 005a 0664 1264 0a64 0b84 015a  .d...Z.d.d.d...Z
-000046a0: 0764 0c64 0d84 005a 0864 0e64 0f84 005a  .d.d...Z.d.d...Z
-000046b0: 0964 1064 1184 005a 0a87 0004 005a 0b53  .d.d...Z.....Z.S
-000046c0: 0029 13da 0d4f 5446 696c 6542 726f 7773  .)...OTFileBrows
-000046d0: 6572 6305 0000 0000 0000 0000 0000 0008  erc.............
-000046e0: 0000 0006 0000 0003 0000 0073 6c00 0000  ...........sl...
-000046f0: 7400 8300 a001 7c01 7c02 7c03 7c04 a104  t.....|.|.|.|...
-00004700: 0100 6700 7c00 5f02 6401 7c00 5f03 6402  ..g.|._.d.|._.d.
-00004710: 7c01 7600 7268 7c01 6402 1900 7d05 6403  |.v.rh|.d...}.d.
-00004720: 7c05 7600 723e 6404 7c00 5f03 6e2a 7c05  |.v.r>d.|._.n*|.
-00004730: 4400 5d24 7d06 7c06 9b00 6405 9d02 6406  D.]$}.|...d...d.
-00004740: 7c06 9b00 9d02 6602 7d07 7c00 6a02 a004  |.....f.}.|.j...
-00004750: 7c07 a101 0100 7142 6407 5300 2908 faa9  |.....qBd.S.)...
-00004760: 5374 6172 7475 7020 636c 6173 732e 0a0a  Startup class...
-00004770: 2020 2020 2020 2020 496e 7075 7473 203a          Inputs :
-00004780: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-00004790: 2d0a 2020 2020 2020 2020 7363 6865 6d61  -.        schema
-000047a0: 203a 2061 2073 6368 656d 6120 6173 2061   : a schema as a
-000047b0: 206e 6573 7465 6420 6f62 6a65 6374 0a20   nested object. 
-000047c0: 2020 2020 2020 2072 6f6f 745f 6672 616d         root_fram
-000047d0: 6520 3a20 2061 2054 6b20 6f62 6a65 6374  e :  a Tk object
-000047e0: 2077 6572 6520 7468 6520 7769 6467 6574   were the widget
-000047f0: 2077 696c 6c20 6265 2067 7261 6674 6564   will be grafted
-00004800: 0a20 2020 2020 2020 2046 5a09 6f74 5f66  .        FZ.ot_f
-00004810: 696c 7465 72da 0964 6972 6563 746f 7279  ilter..directory
-00004820: 547a 0620 6669 6c65 737a 022a 2e4e 2905  Tz. filesz.*.N).
-00004830: 721e 0000 0072 1f00 0000 da07 5f66 696c  r....r......_fil
-00004840: 7465 72da 0c5f 6973 6469 7265 6374 6f72  ter.._isdirector
-00004850: 79da 0661 7070 656e 6429 0872 2900 0000  y..append).r)...
-00004860: 7220 0000 0072 2a00 0000 7222 0000 0072  r ...r*...r"...r
-00004870: 2b00 0000 da07 6669 6c74 6572 73da 0365  +.....filters..e
-00004880: 7874 5a08 6669 6c65 7479 7065 722c 0000  xtZ.filetyper,..
-00004890: 0072 2e00 0000 722f 0000 0072 1f00 0000  .r....r/...r....
-000048a0: 4902 0000 7314 0000 0000 0812 0206 0106  I...s...........
-000048b0: 0208 0108 0108 0108 0208 0114 017a 164f  .............z.O
-000048c0: 5446 696c 6542 726f 7773 6572 2e5f 5f69  TFileBrowser.__i
-000048d0: 6e69 745f 5f63 0100 0000 0000 0000 0000  nit__c..........
-000048e0: 0000 0100 0000 0400 0000 4300 0000 731c  ..........C...s.
-000048f0: 0000 0074 0083 007c 005f 017c 006a 01a0  ...t...|._.|.j..
-00004900: 0264 017c 006a 03a1 0201 0064 0053 0072  .d.|.j.....d.S.r
-00004910: 6a00 0000 72c5 0000 0072 4d00 0000 722e  j...r....rM...r.
-00004920: 0000 0072 2e00 0000 722f 0000 0072 2500  ...r....r/...r%.
-00004930: 0000 5f02 0000 7304 0000 0000 0108 017a  .._...s........z
-00004940: 194f 5446 696c 6542 726f 7773 6572 2e5f  .OTFileBrowser._
-00004950: 6465 6669 6e65 5f76 6172 6301 0000 0000  define_varc.....
-00004960: 0000 0000 0000 0001 0000 0008 0000 0043  ...............C
-00004970: 0000 0073 c800 0000 7c00 6a00 6a01 6401  ...s....|.j.j.d.
-00004980: 6401 6402 6403 8d03 0100 7c00 6a02 6a03  d.d.d.....|.j.j.
-00004990: 6404 7404 1400 6405 8d01 0100 7405 6a06  d.t...d.....t.j.
-000049a0: 7c00 6a02 7c00 6a07 6406 6407 6408 6409  |.j.|.j.d.d.d.d.
-000049b0: 8d05 7c00 5f08 7c00 6a08 6a01 6401 6401  ..|._.|.j.j.d.d.
-000049c0: 640a 640b 640c 8d04 0100 7405 6a09 7c00  d.d.d.....t.j.|.
-000049d0: 6a02 640d 7c00 6a0a 640e 8d03 7c00 5f0b  j.d.|.j.d...|._.
-000049e0: 7c00 6a0b 6a01 6401 6401 640a 640f 640c  |.j.j.d.d.d.d.d.
-000049f0: 8d04 0100 7c00 6a08 6a0c 7c00 6a0b 6a0d  ....|.j.j.|.j.j.
-00004a00: 6410 8d01 0100 7405 6a0e 7c00 6a02 740f  d.....t.j.|.j.t.
-00004a10: 6411 1900 6412 7410 1400 6413 6414 7c00  d...d.t...d.d.|.
-00004a20: 6a11 6415 8d06 7c00 5f12 7c00 6a12 6a01  j.d...|._.|.j.j.
-00004a30: 6416 6401 6417 6403 8d03 0100 6400 5300  d.d.d.d.....d.S.
-00004a40: 2918 4e72 3b00 0000 72bd 0000 0072 4000  ).Nr;...r....r@.
-00004a50: 0000 728a 0000 0072 8b00 0000 727c 0000  ..r....r....r|..
-00004a60: 0072 7400 0000 da05 7269 6768 7429 0472  .rt.....right).r
-00004a70: 7500 0000 721c 0000 0072 7800 0000 da07  u...r....rx.....
-00004a80: 6a75 7374 6966 7967 9a99 9999 9999 d93f  justifyg.......?
-00004a90: 727b 0000 0029 0472 4100 0000 7242 0000  r{...).rA...rB..
-00004aa0: 00da 0872 656c 7769 6474 6872 4300 0000  ...relwidthrC...
-00004ab0: da0a 686f 7269 7a6f 6e74 616c 2902 da06  ..horizontal)...
-00004ac0: 6f72 6965 6e74 72bf 0000 00da 026e 7729  orientr......nw)
-00004ad0: 01da 0e78 7363 726f 6c6c 636f 6d6d 616e  ...xscrollcomman
-00004ae0: 64da 046c 6f61 6467 9a99 9999 9999 b93f  d..loadg.......?
-00004af0: 728f 0000 00fa 0b63 6c61 6d2e 544c 6162  r......clam.TLab
-00004b00: 656c 2905 729c 0000 0072 3000 0000 7292  el).r....r0...r.
-00004b10: 0000 0072 9100 0000 72bf 0000 0072 9f00  ...r....r....r..
-00004b20: 0000 726b 0000 0029 1372 4a00 0000 724b  ..rk...).rJ...rK
-00004b30: 0000 0072 4500 0000 7296 0000 0072 1300  ...rE...r....r..
-00004b40: 0000 7202 0000 0072 0800 0000 726d 0000  ..r....r....rm..
-00004b50: 0072 7e00 0000 da09 5363 726f 6c6c 6261  .r~.....Scrollba
-00004b60: 72da 1d5f 4f54 4669 6c65 4272 6f77 7365  r.._OTFileBrowse
-00004b70: 725f 5f73 6372 6f6c 6c48 616e 646c 6572  r__scrollHandler
-00004b80: 5a07 5f73 6372 6f6c 6c72 8400 0000 7251  Z._scrollr....rQ
-00004b90: 0000 00da 0642 7574 746f 6e72 1400 0000  .....Buttonr....
-00004ba0: 7212 0000 00da 075f 6272 6f77 7365 da04  r......_browse..
-00004bb0: 5f62 746e 724d 0000 0072 2e00 0000 722e  _btnrM...r....r.
-00004bc0: 0000 0072 2f00 0000 7226 0000 0063 0200  ...r/...r&...c..
-00004bd0: 0073 2800 0000 0002 1201 1202 0801 0401  .s(.............
-00004be0: 0201 0201 02fc 0805 1402 1601 1401 1202  ................
-00004bf0: 0801 0601 0601 0201 0201 04fb 0807 7a1d  ..............z.
-00004c00: 4f54 4669 6c65 4272 6f77 7365 722e 5f63  OTFileBrowser._c
-00004c10: 7265 6174 655f 7769 6467 6574 7363 0100  reate_widgetsc..
-00004c20: 0000 0000 0000 0000 0000 0500 0000 0400  ................
-00004c30: 0000 4700 0000 734a 0000 007c 0164 0119  ..G...sJ...|.d..
-00004c40: 007c 0164 0219 0002 007d 027d 037c 0264  .|.d.....}.}.|.d
-00004c50: 036b 0272 327c 0164 0419 007d 047c 006a  .k.r2|.d...}.|.j
-00004c60: 00a0 017c 037c 04a1 0201 006e 147c 0264  ...|.|.....n.|.d
-00004c70: 056b 0272 467c 006a 00a0 027c 03a1 0101  .k.rF|.j...|....
-00004c80: 0064 0653 0029 077a 1d43 616c 6c62 6163  .d.S.).z.Callbac
-00004c90: 6b20 666f 7220 656e 7472 7920 7363 726f  k for entry scro
-00004ca0: 6c6c 6261 7220 7201 0000 0072 3400 0000  llbar r....r4...
-00004cb0: da06 7363 726f 6c6c 728a 0000 00da 066d  ..scrollr......m
-00004cc0: 6f76 6574 6f4e 2903 727e 0000 00da 0c78  ovetoN).r~.....x
-00004cd0: 7669 6577 5f73 6372 6f6c 6cda 0c78 7669  view_scroll..xvi
-00004ce0: 6577 5f6d 6f76 6574 6f29 0572 2900 0000  ew_moveto).r)...
-00004cf0: da01 4cda 026f 705a 0768 6f77 4d61 6e79  ..L..opZ.howMany
-00004d00: da05 756e 6974 7372 2e00 0000 722e 0000  ..unitsr....r...
-00004d10: 0072 2f00 0000 5a0f 5f5f 7363 726f 6c6c  .r/...Z.__scroll
-00004d20: 4861 6e64 6c65 727c 0200 0073 0c00 0000  Handler|...s....
-00004d30: 0002 1201 0801 0801 1001 0801 7a1d 4f54  ............z.OT
-00004d40: 4669 6c65 4272 6f77 7365 722e 5f5f 7363  FileBrowser.__sc
-00004d50: 726f 6c6c 4861 6e64 6c65 724e 6302 0000  rollHandlerNc...
-00004d60: 0000 0000 0000 0000 0004 0000 0004 0000  ................
-00004d70: 0043 0000 0073 6000 0000 7c00 a000 a100  .C...s`...|.....
-00004d80: 7d02 7c00 6a01 721e 7402 6a03 7c00 6a04  }.|.j.r.t.j.|.j.
-00004d90: 6401 8d01 7d03 6e12 7402 6a05 7c00 6a04  d...}.n.t.j.|.j.
-00004da0: 7c00 6a06 6402 8d02 7d03 7c03 6403 6b02  |.j.d...}.|.d.k.
-00004db0: 723c 6404 5300 7407 6a08 a009 7c03 a101  r<d.S.t.j...|...
-00004dc0: 7d03 7c03 7c02 6b03 725c 7c00 6a0a a00b  }.|.|.k.r\|.j...
-00004dd0: 7c03 a101 0100 6404 5300 2905 7a1a 4272  |.....d.S.).z.Br
-00004de0: 6f77 7365 2064 6972 6563 746f 7279 206f  owse directory o
-00004df0: 7220 6669 6c65 732e 2901 721a 0000 0029  r files.).r....)
-00004e00: 0272 1a00 0000 da09 6669 6c65 7479 7065  .r......filetype
-00004e10: 7372 5400 0000 4e29 0c72 2100 0000 72eb  srT...N).r!...r.
-00004e20: 0000 0072 0a00 0000 da0c 6173 6b64 6972  ...r......askdir
-00004e30: 6563 746f 7279 721a 0000 00da 0f61 736b  ectoryr......ask
-00004e40: 6f70 656e 6669 6c65 6e61 6d65 72ea 0000  openfilenamer...
-00004e50: 00da 026f 73da 0470 6174 68da 0772 656c  ...os..path..rel
-00004e60: 7061 7468 726d 0000 0072 5100 0000 2904  pathrm...rQ...).
-00004e70: 7229 0000 00da 0565 7665 6e74 5a08 6375  r).....eventZ.cu
-00004e80: 725f 7061 7468 7208 0100 0072 2e00 0000  r_pathr....r....
-00004e90: 722e 0000 0072 2f00 0000 72fb 0000 0085  r....r/...r.....
-00004ea0: 0200 0073 1600 0000 0002 0802 0601 1002  ...s............
-00004eb0: 0801 04ff 0603 0801 0402 0c01 0801 7a15  ..............z.
-00004ec0: 4f54 4669 6c65 4272 6f77 7365 722e 5f62  OTFileBrowser._b
-00004ed0: 726f 7773 6563 0100 0000 0000 0000 0000  rowsec..........
-00004ee0: 0000 0200 0000 0300 0000 4300 0000 7324  ..........C...s$
-00004ef0: 0000 007c 006a 0064 016b 0272 0e64 026e  ...|.j.d.k.r.d.n
-00004f00: 0264 037d 017c 006a 016a 027c 0164 048d  .d.}.|.j.j.|.d..
-00004f10: 0101 0064 0053 0029 054e 7234 0000 00da  ...d.S.).Nr4....
-00004f20: 0654 456e 7472 79fa 1248 6967 686c 6967  .TEntry..Highlig
-00004f30: 6874 6564 2e54 456e 7472 7972 c200 0000  hted.TEntryr....
-00004f40: 2903 7257 0000 0072 7e00 0000 7284 0000  ).rW...r~...r...
-00004f50: 0072 c300 0000 722e 0000 0072 2e00 0000  .r....r....r....
-00004f60: 722f 0000 0072 5e00 0000 9602 0000 7304  r/...r^.......s.
-00004f70: 0000 0000 0112 017a 234f 5446 696c 6542  .......z#OTFileB
-00004f80: 726f 7773 6572 2e5f 7570 6461 7465 5f77  rowser._update_w
-00004f90: 6964 6765 7473 5f73 7479 6c65 6301 0000  idgets_stylec...
-00004fa0: 0000 0000 0000 0000 0001 0000 0002 0000  ................
-00004fb0: 0043 0000 0073 0a00 0000 7c00 6a00 a001  .C...s....|.j...
-00004fc0: a100 5300 724c 0000 0072 6f00 0000 724d  ..S.rL...ro...rM
-00004fd0: 0000 0072 2e00 0000 722e 0000 0072 2f00  ...r....r....r/.
-00004fe0: 0000 7221 0000 009a 0200 0073 0200 0000  ..r!.......s....
-00004ff0: 0001 7a11 4f54 4669 6c65 4272 6f77 7365  ..z.OTFileBrowse
-00005000: 722e 6765 7463 0200 0000 0000 0000 0000  r.getc..........
-00005010: 0000 0200 0000 0300 0000 4300 0000 7310  ..........C...s.
-00005020: 0000 007c 006a 00a0 017c 01a1 0101 0064  ...|.j...|.....d
-00005030: 0053 0072 4c00 0000 7270 0000 0072 7100  .S.rL...rp...rq.
-00005040: 0000 722e 0000 0072 2e00 0000 722f 0000  ..r....r....r/..
-00005050: 0072 5100 0000 9d02 0000 7302 0000 0000  .rQ.......s.....
-00005060: 017a 114f 5446 696c 6542 726f 7773 6572  .z.OTFileBrowser
-00005070: 2e73 6574 2901 4e29 0c72 6300 0000 7264  .set).N).rc...rd
-00005080: 0000 0072 6500 0000 721f 0000 0072 2500  ...re...r....r%.
-00005090: 0000 7226 0000 0072 f900 0000 72fb 0000  ..r&...r....r...
-000050a0: 0072 5e00 0000 7221 0000 0072 5100 0000  .r^...r!...rQ...
-000050b0: 7267 0000 0072 2e00 0000 722e 0000 0072  rg...r....r....r
-000050c0: 2c00 0000 722f 0000 0072 e700 0000 4702  ,...r/...r....G.
-000050d0: 0000 7310 0000 0008 020c 1608 0408 1908  ..s.............
-000050e0: 090a 1108 0408 0372 e700 0000 6300 0000  .......r....c...
-000050f0: 0000 0000 0000 0000 0000 0000 0003 0000  ................
-00005100: 0000 0000 0073 2000 0000 6500 5a01 6400  .....s ...e.Z.d.
-00005110: 5a02 6401 5a03 8700 6601 6402 6403 8408  Z.d.Z...f.d.d...
-00005120: 5a04 8700 0400 5a05 5300 2904 72cd 0000  Z.....Z.S.).r...
-00005130: 007a 9654 6869 7320 7061 7274 6963 756c  .z.This particul
-00005140: 6172 2063 6c61 7373 2069 7320 666f 7220  ar class is for 
-00005150: 6368 6f6f 7369 6e67 2061 6d6f 6e67 2061  choosing among a
-00005160: 2076 6172 6961 626c 6520 7365 7420 6f66   variable set of
-00005170: 206f 7074 696f 6e0a 2020 2020 0a20 2020   option.    .   
-00005180: 2045 7861 6d70 6c65 3a20 7365 6c65 6374   Example: select
-00005190: 2061 2070 6174 6368 206e 616d 6520 616d   a patch name am
-000051a0: 6f6e 6720 6120 6c69 7374 2066 6f75 6e64  ong a list found
-000051b0: 2069 6e20 616e 2065 7874 6572 6e61 6c20   in an external 
-000051c0: 6669 6c65 0a20 2020 2063 0200 0000 0000  file.    c......
-000051d0: 0000 0000 0000 0500 0000 0300 0000 0300  ................
-000051e0: 0000 7342 0000 0074 007c 006a 01a0 02a1  ..sB...t.|.j....
-000051f0: 0083 017d 027c 006a 0364 0119 007d 037c  ...}.|.j.d...}.|
-00005200: 027c 0319 0064 0264 0285 0219 007d 047c  .|...d.d.....}.|
-00005210: 00a0 047c 04a1 0101 0074 0583 00a0 067c  ...|.....t.....|
-00005220: 01a1 0101 0064 0253 0029 037a 2052 6563  .....d.S.).z Rec
-00005230: 6f6e 6669 6775 7265 2074 6865 206f 7074  onfigure the opt
-00005240: 696f 6e73 2077 6865 6e20 7365 7472 c900  ions when setr..
-00005250: 0000 4e29 0772 0d00 0000 da12 6d79 5f72  ..N).r......my_r
-00005260: 6f6f 745f 7461 625f 7769 6467 6574 7221  oot_tab_widgetr!
-00005270: 0000 0072 2000 0000 72e0 0000 0072 1e00  ...r ...r....r..
-00005280: 0000 7251 0000 0029 0572 2900 0000 7272  ..rQ...).r)...rr
-00005290: 0000 00da 0474 7265 65da 036b 6579 72e1  .....tree..keyr.
-000052a0: 0000 0072 2c00 0000 722e 0000 0072 2f00  ...r,...r....r/.
-000052b0: 0000 7251 0000 00a7 0200 0073 0a00 0000  ..rQ.......s....
-000052c0: 0002 0e01 0a01 1001 0a01 7a14 5f4f 5443  ..........z._OTC
-000052d0: 686f 6963 6544 796e 616d 6963 2e73 6574  hoiceDynamic.set
-000052e0: 2906 7263 0000 0072 6400 0000 7265 0000  ).rc...rd...re..
-000052f0: 0072 6600 0000 7251 0000 0072 6700 0000  .rf...rQ...rg...
-00005300: 722e 0000 0072 2e00 0000 722c 0000 0072  r....r....r,...r
-00005310: 2f00 0000 72cd 0000 00a1 0200 0073 0400  /...r........s..
-00005320: 0000 0801 0405 72cd 0000 0063 0000 0000  ......r....c....
-00005330: 0000 0000 0000 0000 0000 0000 0300 0000  ................
-00005340: 0000 0000 734e 0000 0065 005a 0164 005a  ....sN...e.Z.d.Z
-00005350: 0287 0066 0164 0164 0284 085a 0364 0364  ...f.d.d...Z.d.d
-00005360: 0484 005a 0464 0564 0684 005a 0564 0764  ...Z.d.d...Z.d.d
-00005370: 0884 005a 0664 1064 0a64 0b84 015a 0764  ...Z.d.d.d...Z.d
-00005380: 0c64 0d84 005a 0864 0e64 0f84 005a 0987  .d...Z.d.d...Z..
-00005390: 0004 005a 0a53 0029 11da 064f 5444 6f63  ...Z.S.)...OTDoc
-000053a0: 7563 0500 0000 0000 0000 0000 0000 0500  uc..............
-000053b0: 0000 0600 0000 0300 0000 7326 0000 0074  ..........s&...t
-000053c0: 0083 00a0 017c 017c 027c 037c 04a1 0401  .....|.|.|.|....
-000053d0: 0074 027c 0483 017c 005f 0364 017c 005f  .t.|...|._.d.|._
-000053e0: 0464 0153 0029 0272 e800 0000 4e29 0572  .d.S.).r....N).r
-000053f0: 1e00 0000 721f 0000 0072 1700 0000 da04  ....r....r......
-00005400: 726f 6f74 da07 5f64 6961 6c6f 6772 2800  root.._dialogr(.
-00005410: 0000 722c 0000 0072 2e00 0000 722f 0000  ..r,...r....r/..
-00005420: 0072 1f00 0000 b302 0000 7306 0000 0000  .r........s.....
-00005430: 0812 010a 027a 0f4f 5444 6f63 752e 5f5f  .....z.OTDocu.__
-00005440: 696e 6974 5f5f 6301 0000 0000 0000 0000  init__c.........
-00005450: 0000 0001 0000 0004 0000 0043 0000 0073  ...........C...s
-00005460: 1c00 0000 7400 8300 7c00 5f01 7c00 6a01  ....t...|._.|.j.
-00005470: a002 6401 7c00 6a03 a102 0100 6400 5300  ..d.|.j.....d.S.
-00005480: 726a 0000 0072 c500 0000 724d 0000 0072  rj...r....rM...r
-00005490: 2e00 0000 722e 0000 0072 2f00 0000 7225  ....r....r/...r%
-000054a0: 0000 00c0 0200 0073 0400 0000 0002 0801  .......s........
-000054b0: 7a12 4f54 446f 6375 2e5f 6465 6669 6e65  z.OTDocu._define
-000054c0: 5f76 6172 6301 0000 0000 0000 0000 0000  _varc...........
-000054d0: 0001 0000 0008 0000 0043 0000 0073 4a00  .........C...sJ.
-000054e0: 0000 7400 6a01 7c00 6a02 6401 7403 1400  ..t.j.|.j.d.t...
-000054f0: 6402 7404 6403 1900 6404 7c00 6a05 6405  d.t.d...d.|.j.d.
-00005500: 8d06 7c00 5f06 7c00 6a06 6a07 6406 6407  ..|._.|.j.j.d.d.
-00005510: 6402 6408 8d03 0100 7c00 6a02 6a08 6409  d.d.....|.j.j.d.
-00005520: 640a 640b 8d02 0100 6400 5300 290c 4e67  d.d.....d.S.).Ng
-00005530: 7b14 ae47 e17a 843f da06 6365 6e74 6572  {..G.z.?..center
-00005540: da04 646f 6375 72f7 0000 0029 0572 3000  ..docur....).r0.
-00005550: 0000 7292 0000 0072 9c00 0000 7291 0000  ..r....r....r...
-00005560: 0072 bf00 0000 729f 0000 0072 3b00 0000  .r....r....r;...
-00005570: 7240 0000 00da 0662 6f74 746f 6d72 3800  r@.....bottomr8.
-00005580: 0000 7239 0000 0029 0972 0200 0000 72fa  ..r9...).r....r.
-00005590: 0000 0072 4500 0000 7212 0000 0072 1400  ...rE...r....r..
-000055a0: 0000 da0d 5f70 6f70 7570 5f64 6961 6c6f  ...._popup_dialo
-000055b0: 6772 fc00 0000 724b 0000 00da 0e70 6163  gr....rK.....pac
-000055c0: 6b5f 636f 6e66 6967 7572 6572 4d00 0000  k_configurerM...
-000055d0: 722e 0000 0072 2e00 0000 722f 0000 0072  r....r....r/...r
-000055e0: 2600 0000 c502 0000 7312 0000 0000 0108  &.......s.......
-000055f0: 0106 0102 0106 0102 0104 fb08 0612 017a  ...............z
-00005600: 164f 5444 6f63 752e 5f63 7265 6174 655f  .OTDocu._create_
-00005610: 7769 6467 6574 7363 0100 0000 0000 0000  widgetsc........
-00005620: 0000 0000 0400 0000 0700 0000 4300 0000  ............C...
-00005630: 7328 0100 0074 007c 006a 0183 017c 005f  s(...t.|.j...|._
-00005640: 027c 006a 02a0 037c 006a 01a1 0101 007c  .|.j...|.j.....|
-00005650: 006a 02a0 0464 01a1 0101 007c 006a 02a0  .j...d.....|.j..
-00005660: 05a1 0001 007c 006a 02a0 0664 027c 006a  .....|.j...d.|.j
-00005670: 07a1 0201 007c 006a 02a0 0664 037c 006a  .....|.j...d.|.j
-00005680: 07a1 0201 007c 006a 02a0 0864 047c 006a  .....|.j...d.|.j
-00005690: 07a1 0201 0074 096a 0a7c 006a 0264 0574  .....t.j.|.j.d.t
-000056a0: 0b14 0064 0574 0b14 0064 068d 037d 017c  ...d.t...d...}.|
-000056b0: 016a 0c64 0764 0864 0964 0a8d 0301 007c  .j.d.d.d.d.....|
-000056c0: 01a0 0d64 0ba1 0101 007c 016a 0e64 0c64  ...d.....|.j.d.d
-000056d0: 0d64 0e8d 0201 007c 016a 0f64 0c64 0d64  .d.....|.j.d.d.d
-000056e0: 0e8d 0201 0074 09a0 107c 01a1 017d 027c  .....t...|...}.|
-000056f0: 026a 0c64 0f64 1064 118d 0201 0074 117c  .j.d.d.d.....t.|
-00005700: 0164 127c 026a 1264 1374 0b14 0064 1464  .d.|.j.d.t...d.d
-00005710: 158d 057d 037c 036a 1364 1664 1764 188d  ...}.|.j.d.d.d..
-00005720: 0201 007c 03a0 1464 197c 006a 15a0 16a1  ...|...d.|.j....
-00005730: 0064 16a1 0301 007c 036a 1764 1a64 1b8d  .d.....|.j.d.d..
-00005740: 0101 007c 03a0 0ca1 0001 007c 026a 177c  ...|.......|.j.|
-00005750: 036a 1864 1c8d 0101 0064 1d53 0029 1e7a  .j.d.....d.S.).z
-00005760: 2844 6973 706c 6179 2063 6f6e 7465 6e74  (Display content
-00005770: 206f 6620 646f 6375 6d65 6e74 6174 696f   of documentatio
-00005780: 6e20 7374 7269 6e67 2e5a 0d44 6f63 756d  n string.Z.Docum
-00005790: 656e 7461 7469 6f6e 7a0b 3c43 6f6e 7472  entationz.<Contr
-000057a0: 6f6c 2d77 3e7a 083c 4573 6361 7065 3eda  ol-w>z.<Escape>.
-000057b0: 1057 4d5f 4445 4c45 5445 5f57 494e 444f  .WM_DELETE_WINDO
-000057c0: 57e9 0300 0000 2902 7230 0000 0072 3100  W.....).r0...r1.
-000057d0: 0000 7235 0000 00da 0462 6f74 6854 2903  ..r5.....bothT).
-000057e0: 7237 0000 0072 3a00 0000 da06 6578 7061  r7...r:.....expa
-000057f0: 6e64 4672 0100 0000 7234 0000 0029 01da  ndFr....r4...)..
-00005800: 0677 6569 6768 7472 ef00 0000 da01 7972  .weightr......yr
-00005810: 3900 0000 da04 776f 7264 677b 14ae 47e1  9.....wordg{..G.
-00005820: 7a94 3f72 d200 0000 2904 da04 7772 6170  z.?r....)...wrap
-00005830: da0e 7973 6372 6f6c 6c63 6f6d 6d61 6e64  ..yscrollcommand
-00005840: 7276 0000 0072 d300 0000 da04 626f 6c64  rv...r......bold
-00005850: 2903 5a05 5469 6d65 73e9 0e00 0000 721d  ).Z.Times.....r.
-00005860: 0000 0029 01da 0466 6f6e 74da 0365 6e64  ...)...font..end
-00005870: 727c 0000 00a9 0172 1c00 0000 a901 72bf  r|.....r......r.
-00005880: 0000 004e 2919 7206 0000 0072 1101 0000  ...N).r....r....
-00005890: 7212 0100 00da 0974 7261 6e73 6965 6e74  r......transient
-000058a0: 721a 0000 00da 0867 7261 625f 7365 74da  r......grab_set.
-000058b0: 0462 696e 64da 0f5f 6465 7374 726f 795f  .bind.._destroy_
-000058c0: 6469 616c 6f67 da08 7072 6f74 6f63 6f6c  dialog..protocol
-000058d0: 7202 0000 0072 4400 0000 7212 0000 0072  r....rD...r....r
-000058e0: 4700 0000 da0e 6772 6964 5f70 726f 7061  G.....grid_propa
-000058f0: 6761 7465 da11 6772 6964 5f72 6f77 636f  gate..grid_rowco
-00005900: 6e66 6967 7572 65da 1467 7269 645f 636f  nfigure..grid_co
-00005910: 6c75 6d6e 636f 6e66 6967 7572 6572 f800  lumnconfigurer..
-00005920: 0000 7207 0000 0072 5100 0000 da0d 7461  ..r....rQ.....ta
-00005930: 675f 636f 6e66 6967 7572 65da 0669 6e73  g_configure..ins
-00005940: 6572 7472 6d00 0000 7221 0000 0072 9600  ertrm...r!...r..
-00005950: 0000 da05 7976 6965 7729 0472 2900 0000  ....yview).r)...
-00005960: 5a09 646c 675f 6672 616d 65da 0973 6372  Z.dlg_frame..scr
-00005970: 6f6c 6c62 6172 5a07 7465 7874 5f77 6472  ollbarZ.text_wdr
-00005980: 2e00 0000 722e 0000 0072 2f00 0000 7216  ....r....r/...r.
-00005990: 0100 00cf 0200 0073 3a00 0000 0003 0c01  .......s:.......
-000059a0: 0e01 0c01 0a02 1001 1001 1002 0801 0601  ................
-000059b0: 06fe 0603 1001 0a01 0e01 0e02 0a01 0e02  ................
-000059c0: 0201 0201 0201 0401 0601 02fb 0608 0e01  ................
-000059d0: 1401 0c01 0801 7a14 4f54 446f 6375 2e5f  ......z.OTDocu._
-000059e0: 706f 7075 705f 6469 616c 6f67 4e63 0200  popup_dialogNc..
-000059f0: 0000 0000 0000 0000 0000 0200 0000 0200  ................
-00005a00: 0000 4300 0000 731e 0000 007c 006a 00a0  ..C...s....|.j..
-00005a10: 01a1 0001 007c 006a 02a0 03a1 0001 0064  .....|.j.......d
-00005a20: 017c 005f 0264 0153 0029 027a 1244 6573  .|._.d.S.).z.Des
-00005a30: 7472 6f79 696e 6720 6469 616c 6f67 2e4e  troying dialog.N
-00005a40: 2904 7211 0100 00da 0966 6f63 7573 5f73  ).r......focus_s
-00005a50: 6574 7212 0100 0072 6100 0000 a902 7229  etr....ra.....r)
-00005a60: 0000 0072 0a01 0000 722e 0000 0072 2e00  ...r....r....r..
-00005a70: 0000 722f 0000 0072 2a01 0000 f402 0000  ..r/...r*.......
-00005a80: 7306 0000 0000 020a 010a 017a 164f 5444  s..........z.OTD
-00005a90: 6f63 752e 5f64 6573 7472 6f79 5f64 6961  ocu._destroy_dia
-00005aa0: 6c6f 6763 0100 0000 0000 0000 0000 0000  logc............
-00005ab0: 0100 0000 0200 0000 4300 0000 730a 0000  ........C...s...
-00005ac0: 007c 006a 00a0 01a1 0053 0029 017a 0c56  .|.j.....S.).z.V
-00005ad0: 6f69 6420 7265 7475 726e 2e72 6f00 0000  oid return.ro...
-00005ae0: 724d 0000 0072 2e00 0000 722e 0000 0072  rM...r....r....r
-00005af0: 2f00 0000 7221 0000 00fa 0200 0073 0200  /...r!.......s..
-00005b00: 0000 0002 7a0a 4f54 446f 6375 2e67 6574  ....z.OTDocu.get
-00005b10: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-00005b20: 0003 0000 0043 0000 0073 1000 0000 7c00  .....C...s....|.
-00005b30: 6a00 a001 7c01 a101 0100 6401 5300 2902  j...|.....d.S.).
-00005b40: 7a23 5365 7420 7661 6c75 6520 746f 2064  z#Set value to d
-00005b50: 6f63 756d 656e 7461 7469 6f6e 2063 6f6e  ocumentation con
-00005b60: 7465 6e74 2e4e 7270 0000 0072 7100 0000  tent.Nrp...rq...
-00005b70: 722e 0000 0072 2e00 0000 722f 0000 0072  r....r....r/...r
-00005b80: 5100 0000 fe02 0000 7302 0000 0000 027a  Q.......s......z
-00005b90: 0a4f 5444 6f63 752e 7365 7429 014e 290b  .OTDocu.set).N).
-00005ba0: 7263 0000 0072 6400 0000 7265 0000 0072  rc...rd...re...r
-00005bb0: 1f00 0000 7225 0000 0072 2600 0000 7216  ....r%...r&...r.
-00005bc0: 0100 0072 2a01 0000 7221 0000 0072 5100  ...r*...r!...rQ.
-00005bd0: 0000 7267 0000 0072 2e00 0000 722e 0000  ..rg...r....r...
-00005be0: 0072 2c00 0000 722f 0000 0072 1001 0000  .r,...r/...r....
-00005bf0: b102 0000 730e 0000 0008 020c 0d08 0508  ....s...........
-00005c00: 0a08 250a 0608 0472 1001 0000 6300 0000  ..%....r....c...
-00005c10: 0000 0000 0000 0000 0000 0000 0003 0000  ................
-00005c20: 0000 0000 0073 3c00 0000 6500 5a01 6400  .....s<...e.Z.d.
-00005c30: 5a02 8700 6601 6401 6402 8408 5a03 6403  Z...f.d.d...Z.d.
-00005c40: 6404 8400 5a04 6405 6406 8400 5a05 6407  d...Z.d.d...Z.d.
-00005c50: 6408 8400 5a06 6409 640a 8400 5a07 8700  d...Z.d.d...Z...
-00005c60: 0400 5a08 5300 290b da0d 4f54 4465 7363  ..Z.S.)...OTDesc
-00005c70: 7269 7074 696f 6e63 0500 0000 0000 0000  riptionc........
-00005c80: 0000 0000 0500 0000 0600 0000 0300 0000  ................
-00005c90: 7326 0000 0074 0083 00a0 017c 017c 027c  s&...t.....|.|.|
-00005ca0: 037c 04a1 0401 007c 006a 026a 0364 0164  .|.....|.j.j.d.d
-00005cb0: 0264 038d 0201 0064 0453 0029 0572 e800  .d.....d.S.).r..
-00005cc0: 0000 7215 0100 0072 3800 0000 7239 0000  ..r....r8...r9..
-00005cd0: 004e 2904 721e 0000 0072 1f00 0000 7245  .N).r....r....rE
-00005ce0: 0000 0072 1701 0000 7228 0000 0072 2c00  ...r....r(...r,.
-00005cf0: 0000 722e 0000 0072 2f00 0000 721f 0000  ..r....r/...r...
-00005d00: 0005 0300 0073 0400 0000 0008 1201 7a16  .....s........z.
-00005d10: 4f54 4465 7363 7269 7074 696f 6e2e 5f5f  OTDescription.__
-00005d20: 696e 6974 5f5f 6301 0000 0000 0000 0000  init__c.........
-00005d30: 0000 0001 0000 0004 0000 0043 0000 0073  ...........C...s
-00005d40: 1c00 0000 7400 8300 7c00 5f01 7c00 6a01  ....t...|._.|.j.
-00005d50: a002 6401 7c00 6a03 a102 0100 6400 5300  ..d.|.j.....d.S.
-00005d60: 726a 0000 0072 c500 0000 724d 0000 0072  rj...r....rM...r
-00005d70: 2e00 0000 722e 0000 0072 2f00 0000 7225  ....r....r/...r%
-00005d80: 0000 0010 0300 0073 0400 0000 0002 0801  .......s........
-00005d90: 7a19 4f54 4465 7363 7269 7074 696f 6e2e  z.OTDescription.
-00005da0: 5f64 6566 696e 655f 7661 7263 0100 0000  _define_varc....
-00005db0: 0000 0000 0000 0000 0100 0000 0500 0000  ................
-00005dc0: 4300 0000 732a 0000 007c 006a 006a 0164  C...s*...|.j.j.d
-00005dd0: 017c 006a 0274 0364 0214 0064 038d 0301  .|.j.t.d...d....
-00005de0: 007c 006a 006a 0464 0464 058d 0101 0064  .|.j.j.d.d.....d
-00005df0: 0053 0029 064e 728f 0000 0067 9a99 9999  .S.).Nr....g....
-00005e00: 9999 e93f 2903 72f0 0000 0072 7500 0000  ...?).r....ru...
-00005e10: 723d 0000 0072 1501 0000 a901 7237 0000  r=...r......r7..
-00005e20: 0029 0572 4a00 0000 7296 0000 0072 6d00  .).rJ...r....rm.
-00005e30: 0000 7212 0000 0072 4700 0000 724d 0000  ..r....rG...rM..
-00005e40: 0072 2e00 0000 722e 0000 0072 2f00 0000  .r....r....r/...
-00005e50: 7226 0000 0015 0300 0073 0a00 0000 0001  r&.......s......
-00005e60: 0801 0401 06fe 0603 7a1d 4f54 4465 7363  ........z.OTDesc
-00005e70: 7269 7074 696f 6e2e 5f63 7265 6174 655f  ription._create_
-00005e80: 7769 6467 6574 7363 0100 0000 0000 0000  widgetsc........
-00005e90: 0000 0000 0100 0000 0200 0000 4300 0000  ............C...
-00005ea0: 730a 0000 007c 006a 00a0 01a1 0053 0072  s....|.j.....S.r
-00005eb0: 4c00 0000 726f 0000 0072 4d00 0000 722e  L...ro...rM...r.
-00005ec0: 0000 0072 2e00 0000 722f 0000 0072 2100  ...r....r/...r!.
-00005ed0: 0000 1b03 0000 7302 0000 0000 017a 114f  ......s......z.O
-00005ee0: 5444 6573 6372 6970 7469 6f6e 2e67 6574  TDescription.get
-00005ef0: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-00005f00: 0003 0000 0043 0000 0073 1000 0000 7c00  .....C...s....|.
-00005f10: 6a00 a001 7c01 a101 0100 6400 5300 724c  j...|.....d.S.rL
-00005f20: 0000 0072 7000 0000 7271 0000 0072 2e00  ...rp...rq...r..
-00005f30: 0000 722e 0000 0072 2f00 0000 7251 0000  ..r....r/...rQ..
-00005f40: 001e 0300 0073 0200 0000 0001 7a11 4f54  .....s......z.OT
-00005f50: 4465 7363 7269 7074 696f 6e2e 7365 7429  Description.set)
-00005f60: 0972 6300 0000 7264 0000 0072 6500 0000  .rc...rd...re...
-00005f70: 721f 0000 0072 2500 0000 7226 0000 0072  r....r%...r&...r
-00005f80: 2100 0000 7251 0000 0072 6700 0000 722e  !...rQ...rg...r.
-00005f90: 0000 0072 2e00 0000 722c 0000 0072 2f00  ...r....r,...r/.
-00005fa0: 0000 7235 0100 0003 0300 0073 0a00 0000  ..r5.......s....
-00005fb0: 0802 0c0b 0805 0806 0803 7235 0100 0063  ..........r5...c
-00005fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00005fd0: 0300 0000 0000 0000 7354 0000 0065 005a  ........sT...e.Z
-00005fe0: 0164 005a 0287 0066 0164 0164 0284 085a  .d.Z...f.d.d...Z
-00005ff0: 0364 0364 0484 005a 0464 0564 0684 005a  .d.d...Z.d.d...Z
-00006000: 0564 0764 0884 005a 0664 0964 0a84 005a  .d.d...Z.d.d...Z
-00006010: 0764 0b64 0c84 005a 0864 0d64 0e84 005a  .d.d...Z.d.d...Z
-00006020: 0964 0f64 1084 005a 0a87 0004 005a 0b53  .d.d...Z.....Z.S
-00006030: 0029 11da 094f 5443 6f6d 6d65 6e74 6305  .)...OTCommentc.
-00006040: 0000 0000 0000 0000 0000 0006 0000 0006  ................
-00006050: 0000 0003 0000 0073 5c00 0000 7c01 a000  .......s\...|...
-00006060: 6401 6402 a102 7d05 7c05 6403 6b02 7c00  d.d...}.|.d.k.|.
-00006070: 5f01 7402 8300 a003 7c01 7c02 7c03 7c04  _.t.....|.|.|.|.
-00006080: a104 0100 7c00 6a04 6a05 6404 6405 6406  ....|.j.j.d.d.d.
-00006090: 8d02 0100 7c00 6a04 a006 6407 7c00 6a07  ....|.j...d.|.j.
-000060a0: a102 0100 7c00 6a04 a006 6408 7c00 6a08  ....|.j...d.|.j.
-000060b0: a102 0100 6409 5300 290a 72e8 0000 0072  ....d.S.).r....r
-000060c0: 1c00 0000 721d 0000 0072 7c00 0000 7235  ....r....r|...r5
-000060d0: 0000 0072 3800 0000 7239 0000 00fa 073c  ...r8...r9.....<
-000060e0: 456e 7465 723e fa07 3c4c 6561 7665 3e4e  Enter>..<Leave>N
-000060f0: 2909 7221 0000 0072 7c00 0000 721e 0000  ).r!...r|...r...
-00006100: 0072 1f00 0000 7245 0000 0072 1701 0000  .r....rE...r....
-00006110: 7229 0100 00da 155f 756e 6269 6e64 5f67  r)....._unbind_g
-00006120: 6c6f 6261 6c5f 7363 726f 6c6c da13 5f62  lobal_scroll.._b
-00006130: 696e 645f 676c 6f62 616c 5f73 6372 6f6c  ind_global_scrol
-00006140: 6c29 0672 2900 0000 7220 0000 0072 2a00  l).r)...r ...r*.
-00006150: 0000 7222 0000 0072 2b00 0000 721c 0000  ..r"...r+...r...
-00006160: 0072 2c00 0000 722e 0000 0072 2f00 0000  .r,...r....r/...
-00006170: 721f 0000 0024 0300 0073 0c00 0000 0008  r....$...s......
-00006180: 0c01 0a02 1202 1002 1001 7a12 4f54 436f  ..........z.OTCo
-00006190: 6d6d 656e 742e 5f5f 696e 6974 5f5f 6301  mment.__init__c.
-000061a0: 0000 0000 0000 0000 0000 0001 0000 0004  ................
-000061b0: 0000 0043 0000 0073 1c00 0000 7400 8300  ...C...s....t...
-000061c0: 7c00 5f01 7c00 6a01 a002 6401 7c00 6a03  |._.|.j...d.|.j.
-000061d0: a102 0100 6400 5300 726a 0000 0072 c500  ....d.S.rj...r..
-000061e0: 0000 724d 0000 0072 2e00 0000 722e 0000  ..rM...r....r...
-000061f0: 0072 2f00 0000 7225 0000 0036 0300 0073  .r/...r%...6...s
-00006200: 0400 0000 0001 0801 7a15 4f54 436f 6d6d  ........z.OTComm
-00006210: 656e 742e 5f64 6566 696e 655f 7661 7263  ent._define_varc
-00006220: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00006230: 0700 0000 4300 0000 732c 0000 007c 006a  ....C...s,...|.j
-00006240: 00a0 0164 0164 02a1 027d 0174 027c 006a  ...d.d...}.t.|.j
-00006250: 037c 006a 047c 0164 037c 006a 0564 048d  .|.j.|.d.|.j.d..
-00006260: 057c 005f 0664 0053 0029 054e 7231 0000  .|._.d.S.).Nr1..
-00006270: 00e9 0600 0000 e90a 0000 0029 0372 3100  ...........).r1.
-00006280: 0000 7230 0000 0072 7c00 0000 2907 7220  ..r0...r|...).r 
-00006290: 0000 0072 2100 0000 7215 0000 0072 4500  ...r!...r....rE.
-000062a0: 0000 726d 0000 0072 7c00 0000 da0c 7465  ..rm...r|.....te
-000062b0: 7874 5f63 6f6e 736f 6c65 2902 7229 0000  xt_console).r)..
-000062c0: 0072 3100 0000 722e 0000 0072 2e00 0000  .r1...r....r....
-000062d0: 722f 0000 0072 2600 0000 3a03 0000 730e  r/...r&...:...s.
-000062e0: 0000 0000 010e 0206 0104 0102 0102 0104  ................
-000062f0: fc7a 194f 5443 6f6d 6d65 6e74 2e5f 6372  .z.OTComment._cr
-00006300: 6561 7465 5f77 6964 6765 7473 6301 0000  eate_widgetsc...
-00006310: 0000 0000 0000 0000 0002 0000 0003 0000  ................
-00006320: 0047 0000 0073 1000 0000 7c00 6a00 a001  .G...s....|.j...
-00006330: 6401 a101 0100 6400 5300 2902 4efa 163c  d.....d.S.).N..<
-00006340: 3c62 696e 645f 676c 6f62 616c 5f73 6372  <bind_global_scr
-00006350: 6f6c 6c3e 3ea9 0272 4500 0000 da0e 6576  oll>>..rE.....ev
-00006360: 656e 745f 6765 6e65 7261 7465 725a 0000  ent_generaterZ..
-00006370: 0072 2e00 0000 722e 0000 0072 2f00 0000  .r....r....r/...
-00006380: 723b 0100 0043 0300 0073 0200 0000 0001  r;...C...s......
-00006390: 7a1d 4f54 436f 6d6d 656e 742e 5f62 696e  z.OTComment._bin
-000063a0: 645f 676c 6f62 616c 5f73 6372 6f6c 6c63  d_global_scrollc
-000063b0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-000063c0: 0300 0000 4700 0000 7310 0000 007c 006a  ....G...s....|.j
-000063d0: 00a0 0164 01a1 0101 0064 0053 0029 024e  ...d.....d.S.).N
-000063e0: fa18 3c3c 756e 6269 6e64 5f67 6c6f 6261  ..<<unbind_globa
-000063f0: 6c5f 7363 726f 6c6c 3e3e 7240 0100 0072  l_scroll>>r@...r
-00006400: 5a00 0000 722e 0000 0072 2e00 0000 722f  Z...r....r....r/
-00006410: 0000 0072 3a01 0000 4603 0000 7302 0000  ...r:...F...s...
-00006420: 0000 017a 1f4f 5443 6f6d 6d65 6e74 2e5f  ...z.OTComment._
-00006430: 756e 6269 6e64 5f67 6c6f 6261 6c5f 7363  unbind_global_sc
-00006440: 726f 6c6c 6301 0000 0000 0000 0000 0000  rollc...........
-00006450: 0001 0000 0002 0000 0043 0000 0073 0e00  .........C...s..
-00006460: 0000 7c00 6a00 a001 a100 a002 a100 5300  ..|.j.........S.
-00006470: 724c 0000 0029 0372 6d00 0000 7221 0000  rL...).rm...r!..
-00006480: 00da 0672 7374 7269 7072 4d00 0000 722e  ...rstriprM...r.
-00006490: 0000 0072 2e00 0000 722f 0000 0072 2100  ...r....r/...r!.
-000064a0: 0000 4903 0000 7302 0000 0000 017a 0d4f  ..I...s......z.O
-000064b0: 5443 6f6d 6d65 6e74 2e67 6574 6302 0000  TComment.getc...
-000064c0: 0000 0000 0000 0000 0002 0000 0003 0000  ................
-000064d0: 0043 0000 0073 1000 0000 7c00 6a00 a001  .C...s....|.j...
-000064e0: 7c01 a101 0100 6400 5300 724c 0000 0029  |.....d.S.rL...)
-000064f0: 0272 3e01 0000 da08 7365 745f 7465 7874  .r>.....set_text
-00006500: 7271 0000 0072 2e00 0000 722e 0000 0072  rq...r....r....r
-00006510: 2f00 0000 7251 0000 004c 0300 0073 0200  /...rQ...L...s..
-00006520: 0000 0001 7a0d 4f54 436f 6d6d 656e 742e  ....z.OTComment.
-00006530: 7365 7463 0100 0000 0000 0000 0000 0000  setc............
-00006540: 0300 0000 0300 0000 4300 0000 7356 0000  ........C...sV..
-00006550: 007c 006a 0072 0a64 0053 007c 006a 0164  .|.j.r.d.S.|.j.d
-00006560: 016b 0272 1864 026e 0674 0264 0319 007d  .k.r.d.n.t.d...}
-00006570: 017c 006a 0164 016b 0272 2e64 046e 0674  .|.j.d.k.r.d.n.t
-00006580: 0264 0519 007d 027c 006a 036a 047c 0164  .d...}.|.j.j.|.d
-00006590: 068d 0101 007c 006a 036a 047c 0264 078d  .....|.j.j.|.d..
-000065a0: 0101 0064 0053 0029 084e 7234 0000 0072  ...d.S.).Nr4...r
-000065b0: 8500 0000 7286 0000 0072 7400 0000 7281  ....r....rt...r.
-000065c0: 0000 0072 8700 0000 2901 7278 0000 0029  ...r....).rx...)
-000065d0: 0572 7c00 0000 7257 0000 0072 1100 0000  .r|...rW...r....
-000065e0: 723e 0100 0072 8400 0000 2903 7229 0000  r>...r....).r)..
-000065f0: 005a 0762 6763 6f6c 6f72 5a07 6667 636f  .Z.bgcolorZ.fgco
-00006600: 6c6f 7272 2e00 0000 722e 0000 0072 2f00  lorr....r....r/.
-00006610: 0000 725e 0000 004f 0300 0073 0c00 0000  ..r^...O...s....
-00006620: 0001 0601 0402 1601 1601 0e01 7a1f 4f54  ............z.OT
-00006630: 436f 6d6d 656e 742e 5f75 7064 6174 655f  Comment._update_
-00006640: 7769 6467 6574 735f 7374 796c 6529 0c72  widgets_style).r
-00006650: 6300 0000 7264 0000 0072 6500 0000 721f  c...rd...re...r.
-00006660: 0000 0072 2500 0000 7226 0000 0072 3b01  ...r%...r&...r;.
-00006670: 0000 723a 0100 0072 2100 0000 7251 0000  ..r:...r!...rQ..
-00006680: 0072 5e00 0000 7267 0000 0072 2e00 0000  .r^...rg...r....
-00006690: 722e 0000 0072 2c00 0000 722f 0000 0072  r....r,...r/...r
-000066a0: 3701 0000 2203 0000 7310 0000 0008 020c  7..."...s.......
-000066b0: 1208 0408 0908 0308 0308 0308 0372 3701  .............r7.
-000066c0: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-000066d0: 0000 0002 0000 0040 0000 0073 2800 0000  .......@...s(...
-000066e0: 6500 5a01 6400 5a02 6401 5a03 6402 6403  e.Z.d.Z.d.Z.d.d.
-000066f0: 8400 5a04 6404 6405 8400 5a05 6406 6407  ..Z.d.d...Z.d.d.
-00006700: 8400 5a06 6408 5300 2909 da07 4f54 456d  ..Z.d.S.)...OTEm
-00006710: 7074 797a 224f 5420 7769 6467 6574 2066  ptyz"OT widget f
-00006720: 6f72 2075 6e69 6d70 6c65 6d65 6e74 6564  or unimplemented
-00006730: 2074 7970 6573 2e63 0100 0000 0000 0000   types.c........
-00006740: 0000 0000 0300 0000 0700 0000 4300 0000  ............C...
-00006750: 7382 0000 0064 017c 005f 007c 006a 01a0  s....d.|._.|.j..
-00006760: 0264 0264 00a1 0264 036b 0372 1c64 0053  .d.d...d.k.r.d.S
-00006770: 0067 007d 0164 0444 005d 287d 027c 027c  .g.}.d.D.](}.|.|
-00006780: 006a 0176 0072 247c 01a0 037c 029b 0064  .j.v.r$|...|...d
-00006790: 057c 006a 017c 0219 009b 009d 03a1 0101  .|.j.|..........
-000067a0: 0071 247c 006a 046a 0564 06a0 067c 01a1  .q$|.j.j.d...|..
-000067b0: 0164 078d 0101 007c 006a 046a 0764 0864  .d.....|.j.j.d.d
-000067c0: 0964 0964 0a8d 0301 007c 006a 08a0 09a1  .d.d.....|.j....
-000067d0: 0001 0064 0053 0029 0b4e 7201 0000 00da  ...d.S.).Nr.....
-000067e0: 076f 745f 7479 7065 da04 766f 6964 2904  .ot_type..void).
-000067f0: 7222 0000 0072 1a00 0000 da04 7479 7065  r"...r......type
-00006800: 7246 0100 007a 0320 3d20 da01 0aa9 0172  rF...z. = .....r
-00006810: 3c00 0000 7235 0000 0072 8a00 0000 2903  <...r5...r....).
-00006820: 7237 0000 00da 0470 6164 78da 0470 6164  r7.....padx..pad
-00006830: 7929 0a72 5700 0000 7220 0000 0072 2100  y).rW...r ...r!.
-00006840: 0000 72ec 0000 0072 4a00 0000 7284 0000  ..r....rJ...r...
-00006850: 00da 046a 6f69 6e72 4700 0000 7245 0000  ...joinrG...rE..
-00006860: 00da 0666 6f72 6765 7429 0372 2900 0000  ...forget).r)...
-00006870: da04 696e 666f da04 6974 656d 722e 0000  ..info..itemr...
-00006880: 0072 2e00 0000 722f 0000 0072 2600 0000  .r....r/...r&...
-00006890: 5c03 0000 7314 0000 0000 0106 0112 0104  \...s...........
-000068a0: 0204 0108 010a 011c 0214 0112 027a 174f  .............z.O
-000068b0: 5445 6d70 7479 2e5f 6372 6561 7465 5f77  TEmpty._create_w
-000068c0: 6964 6765 7473 6301 0000 0000 0000 0000  idgetsc.........
-000068d0: 0000 0001 0000 0001 0000 0043 0000 0073  ...........C...s
-000068e0: 0400 0000 6400 5300 724c 0000 0072 2e00  ....d.S.rL...r..
-000068f0: 0000 724d 0000 0072 2e00 0000 722e 0000  ..rM...r....r...
-00006900: 0072 2f00 0000 7221 0000 006b 0300 0073  .r/...r!...k...s
-00006910: 0200 0000 0001 7a0b 4f54 456d 7074 792e  ......z.OTEmpty.
-00006920: 6765 7463 0100 0000 0000 0000 0000 0000  getc............
-00006930: 0300 0000 0100 0000 4f00 0000 7304 0000  ........O...s...
-00006940: 0064 0053 0072 4c00 0000 722e 0000 0029  .d.S.rL...r....)
-00006950: 0372 2900 0000 725b 0000 00da 066b 7761  .r)...r[.....kwa
-00006960: 7267 7372 2e00 0000 722e 0000 0072 2f00  rgsr....r....r/.
-00006970: 0000 7251 0000 006e 0300 0073 0200 0000  ..rQ...n...s....
-00006980: 0001 7a0b 4f54 456d 7074 792e 7365 744e  ..z.OTEmpty.setN
-00006990: 2907 7263 0000 0072 6400 0000 7265 0000  ).rc...rd...re..
-000069a0: 0072 6600 0000 7226 0000 0072 2100 0000  .rf...r&...r!...
-000069b0: 7251 0000 0072 2e00 0000 722e 0000 0072  rQ...r....r....r
-000069c0: 2e00 0000 722f 0000 0072 4501 0000 5903  ....r/...rE...Y.
-000069d0: 0000 7308 0000 0008 0104 0208 0f08 0372  ..s............r
-000069e0: 4501 0000 6300 0000 0000 0000 0000 0000  E...c...........
-000069f0: 0000 0000 0003 0000 0040 0000 0073 6600  .........@...sf.
-00006a00: 0000 6500 5a01 6400 5a02 6401 5a03 6402  ..e.Z.d.Z.d.Z.d.
-00006a10: 6403 8400 5a04 6404 6405 8400 5a05 6406  d...Z.d.d...Z.d.
-00006a20: 6407 8400 5a06 6408 6409 8400 5a07 6508  d...Z.d.d...Z.e.
-00006a30: 6a09 640a 640b 8400 8301 5a0a 640c 640d  j.d.d.....Z.d.d.
-00006a40: 8400 5a0b 640e 640f 8400 5a0c 6410 6411  ..Z.d.d...Z.d.d.
-00006a50: 8400 5a0d 6412 6413 8400 5a0e 6414 6415  ..Z.d.d...Z.d.d.
-00006a60: 8400 5a0f 6416 5300 2917 da0f 5f4f 5441  ..Z.d.S.)..._OTA
-00006a70: 6273 7472 6163 744c 6973 747a cd43 6c61  bstractListz.Cla
-00006a80: 7373 2074 6f20 6861 6e64 6c65 204c 4953  ss to handle LIS
-00006a90: 5453 0a20 2020 200a 2020 2020 496e 2074  TS.    .    In t
-00006aa0: 6865 206d 656d 6f72 7920 6120 6c69 7374  he memory a list
-00006ab0: 2069 7320 6120 5079 7468 6f6e 204c 6973   is a Python Lis
-00006ac0: 7473 0a20 2020 2042 7574 2066 6f72 2074  ts.    But for t
-00006ad0: 6865 2047 5549 2c20 7468 6520 6c69 7374  he GUI, the list
-00006ae0: 2063 6f6e 7461 696e 6573 2073 7562 6c65   containes suble
-00006af0: 6176 6573 2077 6974 6820 7370 6563 6966  aves with specif
-00006b00: 6963 2062 6568 6176 696f 720a 2020 2020  ic behavior.    
-00006b10: 5765 206c 6f6f 7365 2068 6572 6520 7468  We loose here th
-00006b20: 6520 7573 7561 6c20 7065 7266 6563 7420  e usual perfect 
-00006b30: 6d61 7070 696e 6720 6274 7720 6d65 6d6f  mapping btw memo
-00006b40: 7279 2061 6e64 2047 5549 6301 0000 0000  ry and GUIc.....
-00006b50: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
-00006b60: 0000 0073 0a00 0000 6700 7c00 5f00 6400  ...s....g.|._.d.
-00006b70: 5300 724c 0000 0072 4e00 0000 724d 0000  S.rL...rN...rM..
-00006b80: 0072 2e00 0000 722e 0000 0072 2f00 0000  .r....r....r/...
-00006b90: 7223 0000 0079 0300 0073 0200 0000 0001  r#...y...s......
-00006ba0: 7a24 5f4f 5441 6273 7472 6163 744c 6973  z$_OTAbstractLis
-00006bb0: 742e 5f69 6e69 745f 7072 6576 696f 7573  t._init_previous
-00006bc0: 5f76 616c 7565 6301 0000 0000 0000 0000  _valuec.........
-00006bd0: 0000 0001 0000 0006 0000 0043 0000 0073  ...........C...s
-00006be0: 2e00 0000 7400 a001 7c00 6a02 a101 7c00  ....t...|.j...|.
-00006bf0: 5f03 7c00 6a03 6a04 6401 6401 6402 6403  _.|.j.j.d.d.d.d.
-00006c00: 6404 8d04 0100 7c00 a005 a100 0100 6400  d.....|.......d.
-00006c10: 5300 2905 4e72 3b00 0000 723e 0000 0072  S.).Nr;...r>...r
-00006c20: f400 0000 a904 72f1 0000 0072 4100 0000  ......r....rA...
-00006c30: 7242 0000 0072 4300 0000 2906 7202 0000  rB...rC...).r...
-00006c40: 0072 4400 0000 7245 0000 00da 0f65 6e74  .rD...rE.....ent
-00006c50: 7279 6c69 7374 686f 6c64 6572 724b 0000  rylistholderrK..
-00006c60: 00da 155f 636f 6e66 6967 7572 655f 706f  ..._configure_po
-00006c70: 7075 705f 6d65 6e75 724d 0000 0072 2e00  pup_menurM...r..
-00006c80: 0000 722e 0000 0072 2f00 0000 7226 0000  ..r....r/...r&..
-00006c90: 007c 0300 0073 1000 0000 0001 0e01 0601  .|...s..........
-00006ca0: 0201 0201 0201 02fc 0606 7a1f 5f4f 5441  ..........z._OTA
-00006cb0: 6273 7472 6163 744c 6973 742e 5f63 7265  bstractList._cre
-00006cc0: 6174 655f 7769 6467 6574 7363 0100 0000  ate_widgetsc....
-00006cd0: 0000 0000 0000 0000 0500 0000 0600 0000  ................
-00006ce0: 4300 0000 7374 0000 007c 006a 0064 0119  C...st...|.j.d..
-00006cf0: 00a0 0164 02a1 017d 017c 006a 0064 0119  ...d...}.|.j.d..
-00006d00: 00a0 0164 0364 00a1 027d 027c 0264 0075  ...d.d...}.|.d.u
-00006d10: 0072 4264 0464 0564 0664 079c 037d 037c  .rBd.d.d.d...}.|
-00006d20: 037c 0119 007c 027c 013c 0074 0264 087c  .|...|.|.<.t.d.|
-00006d30: 006a 00a0 0164 0964 08a1 0283 027d 0474  .j...d.d.....}.t
-00006d40: 037c 047c 006a 00a0 0164 0a64 08a1 0283  .|.|.j...d.d....
-00006d50: 027d 047c 0267 017c 0414 0053 0029 0b4e  .}.|.g.|...S.).N
-00006d60: 72dd 0000 0072 4801 0000 7253 0000 0072  r....rH...rS...r
-00006d70: 5400 0000 723e 0000 0072 0100 0000 2903  T...r>...r....).
-00006d80: da06 7374 7269 6e67 da06 6e75 6d62 6572  ..string..number
-00006d90: 729e 0000 0072 3400 0000 da08 6d61 7849  r....r4.....maxI
-00006da0: 7465 6d73 da08 6d69 6e49 7465 6d73 2904  tems..minItems).
-00006db0: 7220 0000 0072 2100 0000 da03 6d69 6e72  r ...r!.....minr
-00006dc0: d500 0000 2905 7229 0000 00da 0969 7465  ....).r).....ite
-00006dd0: 6d5f 7479 7065 7272 0000 005a 0874 7970  m_typerr...Z.typ
-00006de0: 6532 7661 6c5a 066e 5f72 6570 7372 2e00  e2valZ.n_repsr..
-00006df0: 0000 722e 0000 0072 2f00 0000 7252 0000  ..r....r/...rR..
-00006e00: 0086 0300 0073 1600 0000 0004 1001 1202  .....s..........
-00006e10: 0803 0201 0201 02fe 0603 0c03 1401 1402  ................
-00006e20: 7a1c 5f4f 5441 6273 7472 6163 744c 6973  z._OTAbstractLis
-00006e30: 742e 5f67 6574 5f64 6566 6175 6c74 6301  t._get_defaultc.
-00006e40: 0000 0000 0000 0000 0000 0001 0000 0004  ................
-00006e50: 0000 0043 0000 0073 3c00 0000 7400 7c00  ...C...s<...t.|.
-00006e60: 6a01 6401 6402 8d02 7c00 5f02 7c00 a003  j.d.d...|._.|...
-00006e70: a100 0100 7c00 6a01 a004 6403 7c00 6a05  ....|.j...d.|.j.
-00006e80: a102 0100 7c00 6a01 a004 6404 7c00 6a06  ....|.j...d.|.j.
-00006e90: a102 0100 6400 5300 2905 4e46 2901 da07  ....d.S.).NF)...
-00006ea0: 7465 6172 6f66 6672 3801 0000 7239 0100  tearoffr8...r9..
-00006eb0: 0029 0772 0b00 0000 7254 0100 00da 0a70  .).r....rT.....p
-00006ec0: 6f70 7570 5f6d 656e 75da 135f 6164 645f  opup_menu.._add_
-00006ed0: 706f 7075 705f 636f 6d6d 616e 6473 7229  popup_commandsr)
-00006ee0: 0100 00da 0f5f 6163 7469 7661 7465 5f70  ....._activate_p
-00006ef0: 6f70 7570 da11 5f64 6561 6374 6976 6174  opup.._deactivat
-00006f00: 655f 706f 7075 7072 4d00 0000 722e 0000  e_popuprM...r...
-00006f10: 0072 2e00 0000 722f 0000 0072 5501 0000  .r....r/...rU...
-00006f20: 9b03 0000 7308 0000 0000 0110 0208 0210  ....s...........
-00006f30: 017a 255f 4f54 4162 7374 7261 6374 4c69  .z%_OTAbstractLi
-00006f40: 7374 2e5f 636f 6e66 6967 7572 655f 706f  st._configure_po
-00006f50: 7075 705f 6d65 6e75 6301 0000 0000 0000  pup_menuc.......
-00006f60: 0000 0000 0001 0000 0001 0000 0043 0000  .............C..
-00006f70: 0073 0400 0000 6400 5300 724c 0000 0072  .s....d.S.rL...r
-00006f80: 2e00 0000 724d 0000 0072 2e00 0000 722e  ....rM...r....r.
-00006f90: 0000 0072 2f00 0000 725e 0100 00a3 0300  ...r/...r^......
-00006fa0: 0073 0200 0000 0002 7a23 5f4f 5441 6273  .s......z#_OTAbs
-00006fb0: 7472 6163 744c 6973 742e 5f61 6464 5f70  tractList._add_p
-00006fc0: 6f70 7570 5f63 6f6d 6d61 6e64 7363 0100  opup_commandsc..
-00006fd0: 0000 0000 0000 0000 0000 0200 0000 0400  ................
-00006fe0: 0000 4700 0000 7314 0000 007c 006a 00a0  ..G...s....|.j..
-00006ff0: 0164 017c 006a 02a1 0201 0064 0053 00a9  .d.|.j.....d.S..
-00007000: 024e 7a0a 3c42 7574 746f 6e2d 323e 2903  .Nz.<Button-2>).
-00007010: 7254 0100 00da 0862 696e 645f 616c 6cda  rT.....bind_all.
-00007020: 0e6f 6e5f 7269 6768 745f 636c 6963 6b72  .on_right_clickr
-00007030: 5a00 0000 722e 0000 0072 2e00 0000 722f  Z...r....r....r/
-00007040: 0000 0072 5f01 0000 a703 0000 7302 0000  ...r_.......s...
-00007050: 0000 017a 1f5f 4f54 4162 7374 7261 6374  ...z._OTAbstract
-00007060: 4c69 7374 2e5f 6163 7469 7661 7465 5f70  List._activate_p
-00007070: 6f70 7570 6301 0000 0000 0000 0000 0000  opupc...........
-00007080: 0002 0000 0003 0000 0047 0000 0073 1000  .........G...s..
-00007090: 0000 7c00 6a00 a001 6401 a101 0100 6400  ..|.j...d.....d.
-000070a0: 5300 7261 0100 0029 0272 5401 0000 da0a  S.ra...).rT.....
-000070b0: 756e 6269 6e64 5f61 6c6c 725a 0000 0072  unbind_allrZ...r
-000070c0: 2e00 0000 722e 0000 0072 2f00 0000 7260  ....r....r/...r`
-000070d0: 0100 00aa 0300 0073 0200 0000 0001 7a21  .......s......z!
-000070e0: 5f4f 5441 6273 7472 6163 744c 6973 742e  _OTAbstractList.
-000070f0: 5f64 6561 6374 6976 6174 655f 706f 7075  _deactivate_popu
-00007100: 7063 0200 0000 0000 0000 0000 0000 0200  pc..............
-00007110: 0000 0400 0000 4300 0000 7316 0000 007c  ......C...s....|
-00007120: 006a 00a0 017c 016a 027c 016a 03a1 0201  .j...|.j.|.j....
-00007130: 0064 0053 0072 4c00 0000 2904 725d 0100  .d.S.rL...).r]..
-00007140: 00da 0874 6b5f 706f 7075 70da 0678 5f72  ...tk_popup..x_r
-00007150: 6f6f 74da 0679 5f72 6f6f 7472 3401 0000  oot..y_rootr4...
-00007160: 722e 0000 0072 2e00 0000 722f 0000 0072  r....r....r/...r
-00007170: 6301 0000 ad03 0000 7302 0000 0000 017a  c.......s......z
-00007180: 1e5f 4f54 4162 7374 7261 6374 4c69 7374  ._OTAbstractList
-00007190: 2e6f 6e5f 7269 6768 745f 636c 6963 6b63  .on_right_clickc
-000071a0: 0100 0000 0000 0000 0000 0000 0400 0000  ................
-000071b0: 0500 0000 4700 0000 7338 0000 0064 01a0  ....G...s8...d..
-000071c0: 0064 0264 0384 007c 00a0 01a1 0044 0083  .d.d...|.....D..
-000071d0: 01a1 017d 0274 027c 006a 0383 017d 037c  ...}.t.|.j...}.|
-000071e0: 03a0 04a1 0001 007c 03a0 057c 02a1 0101  .......|...|....
-000071f0: 0064 0053 0029 044e 7a02 2c20 6301 0000  .d.S.).Nz., c...
-00007200: 0000 0000 0000 0000 0002 0000 0004 0000  ................
-00007210: 0053 0000 0073 1400 0000 6700 7c00 5d0c  .S...s....g.|.].
-00007220: 7d01 7400 7c01 8301 9102 7104 5300 722e  }.t.|.....q.S.r.
-00007230: 0000 0029 01da 0373 7472 a902 da02 2e30  ...)...str.....0
-00007240: 7272 0000 0072 2e00 0000 722e 0000 0072  rr...r....r....r
-00007250: 2f00 0000 da0a 3c6c 6973 7463 6f6d 703e  /.....<listcomp>
-00007260: b103 0000 f300 0000 007a 2b5f 4f54 4162  .........z+_OTAb
-00007270: 7374 7261 6374 4c69 7374 2e6f 6e5f 636f  stractList.on_co
-00007280: 7079 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  py.<locals>.<lis
-00007290: 7463 6f6d 703e 2906 724d 0100 0072 2100  tcomp>).rM...r!.
-000072a0: 0000 7217 0000 0072 4500 0000 da0f 636c  ..r....rE.....cl
-000072b0: 6970 626f 6172 645f 636c 6561 72da 1063  ipboard_clear..c
-000072c0: 6c69 7062 6f61 7264 5f61 7070 656e 6429  lipboard_append)
-000072d0: 0472 2900 0000 725b 0000 005a 0863 6f70  .r)...r[...Z.cop
-000072e0: 795f 7374 7272 1101 0000 722e 0000 0072  y_strr....r....r
-000072f0: 2e00 0000 722f 0000 00da 076f 6e5f 636f  ....r/.....on_co
-00007300: 7079 b003 0000 7308 0000 0000 0118 010a  py....s.........
-00007310: 0108 017a 175f 4f54 4162 7374 7261 6374  ...z._OTAbstract
-00007320: 4c69 7374 2e6f 6e5f 636f 7079 6302 0000  List.on_copyc...
-00007330: 0000 0000 0000 0000 0002 0000 0003 0000  ................
-00007340: 0043 0000 0073 1600 0000 7c00 6a00 6a01  .C...s....|.j.j.
-00007350: 7c01 7402 1400 6401 8d01 0100 6400 5300  |.t...d.....d.S.
-00007360: 2902 4e72 8b00 0000 2903 7245 0000 0072  ).Nr....).rE...r
-00007370: 9600 0000 7213 0000 00a9 0272 2900 0000  ....r......r)...
-00007380: 72d7 0000 0072 2e00 0000 722e 0000 0072  r....r....r....r
-00007390: 2f00 0000 da0e 5f72 6573 697a 655f 686f  /....._resize_ho
-000073a0: 6c64 6572 b603 0000 7302 0000 0000 017a  lder....s......z
-000073b0: 1e5f 4f54 4162 7374 7261 6374 4c69 7374  ._OTAbstractList
-000073c0: 2e5f 7265 7369 7a65 5f68 6f6c 6465 724e  ._resize_holderN
-000073d0: 2910 7263 0000 0072 6400 0000 7265 0000  ).rc...rd...re..
-000073e0: 0072 6600 0000 7223 0000 0072 2600 0000  .rf...r#...r&...
-000073f0: 7252 0000 0072 5501 0000 72b6 0000 0072  rR...rU...r....r
-00007400: b700 0000 725e 0100 0072 5f01 0000 7260  ....r^...r_...r`
-00007410: 0100 0072 6301 0000 726f 0100 0072 7101  ...rc...ro...rq.
-00007420: 0000 722e 0000 0072 2e00 0000 722e 0000  ..r....r....r...
-00007430: 0072 2f00 0000 7252 0100 0072 0300 0073  .r/...rR...r...s
-00007440: 1800 0000 0801 0406 0803 080a 0815 0808  ................
-00007450: 0401 0a03 0803 0803 0803 0806 7252 0100  ............rR..
-00007460: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00007470: 0000 0400 0000 0000 0000 738e 0000 0065  ..........s....e
-00007480: 005a 0164 005a 0264 015a 0364 1f87 0066  .Z.d.Z.d.Z.d...f
-00007490: 0164 0364 0484 095a 0464 0564 0684 005a  .d.d...Z.d.d...Z
-000074a0: 0564 0764 0884 005a 0664 0964 0a84 005a  .d.d...Z.d.d...Z
-000074b0: 0764 0b64 0c84 005a 0864 0d64 0e84 005a  .d.d...Z.d.d...Z
-000074c0: 0965 0a64 0f64 1084 0083 015a 0b64 1164  .e.d.d.....Z.d.d
-000074d0: 1284 005a 0c64 1364 1484 005a 0d64 1564  ...Z.d.d...Z.d.d
-000074e0: 1684 005a 0e64 1764 1884 005a 0f64 1964  ...Z.d.d...Z.d.d
-000074f0: 1a84 005a 1064 1b64 1c84 005a 1164 1d64  ...Z.d.d...Z.d.d
-00007500: 1e84 005a 1287 0004 005a 1353 0029 20da  ...Z.....Z.S.) .
-00007510: 0a5f 4c69 7374 456e 7472 797a 4f54 6865  ._ListEntryzOThe
-00007520: 2064 6566 6175 6c74 2053 5542 7769 6467   default SUBwidg
-00007530: 6574 2065 6e74 7279 2066 6f72 206c 6973  et entry for lis
-00007540: 7473 0a20 2020 200a 2020 2020 5468 6973  ts.    .    This
-00007550: 2069 7320 7061 636b 6564 2049 6e73 6964   is packed Insid
-00007560: 6520 616e 204f 544c 6973 742e 4e63 0500  e an OTList.Nc..
-00007570: 0000 0000 0000 0000 0000 0500 0000 0600  ................
-00007580: 0000 0300 0000 7322 0000 007c 047c 005f  ......s"...|.|._
-00007590: 007c 037c 005f 0174 0283 00a0 037c 017c  .|.|._.t.....|.|
-000075a0: 0264 017c 03a1 0401 0064 0153 0029 027a  .d.|.....d.S.).z
-000075b0: 1e41 6464 6974 696f 6e73 2074 6f20 5f4c  .Additions to _L
-000075c0: 6561 6657 6964 6765 7420 696e 6974 204e  eafWidget init N
-000075d0: 2904 da0f 5f70 7265 7669 6f75 735f 7661  )..._previous_va
-000075e0: 6c75 6572 4500 0000 721e 0000 0072 1f00  luerE...r....r..
-000075f0: 0000 2905 7229 0000 0072 2000 0000 722a  ..).r)...r ...r*
-00007600: 0000 00da 0668 6f6c 6465 7272 4f00 0000  .....holderrO...
-00007610: 722c 0000 0072 2e00 0000 722f 0000 0072  r,...r....r/...r
-00007620: 1f00 0000 bf03 0000 7306 0000 0000 0206  ........s.......
-00007630: 0106 017a 135f 4c69 7374 456e 7472 792e  ...z._ListEntry.
-00007640: 5f5f 696e 6974 5f5f 6301 0000 0000 0000  __init__c.......
-00007650: 0000 0000 0001 0000 0005 0000 0043 0000  .............C..
-00007660: 0073 3800 0000 7400 6a01 7c00 6a02 7c00  .s8...t.j.|.j.|.
-00007670: 6a03 6401 6402 8d03 7c00 5f04 7c00 6a04  j.d.d...|._.|.j.
-00007680: 6a05 6403 6404 8d01 0100 7c00 6a04 a006  j.d.d.....|.j...
-00007690: 6405 7c00 6a07 a102 0100 6406 5300 2907  d.|.j.....d.S.).
-000076a0: fa3d 5245 6465 6669 6e65 2057 4954 484f  .=REdefine WITHO
-000076b0: 5554 2072 6563 616c 6c69 6e67 205f 6372  UT recalling _cr
-000076c0: 6561 7465 5f77 6964 6765 7473 2829 2066  eate_widgets() f
-000076d0: 726f 6d20 4c65 6166 5769 6467 6574 2146  rom LeafWidget!F
-000076e0: 2902 7275 0000 0072 7700 0000 7235 0000  ).ru...rw...r5..
-000076f0: 0072 3601 0000 7a09 3c46 6f63 7573 496e  .r6...z.<FocusIn
-00007700: 3e4e 2908 7202 0000 0072 0800 0000 7245  >N).r....r....rE
-00007710: 0000 0072 6d00 0000 da05 656e 7472 7972  ...rm.....entryr
-00007720: 4700 0000 7229 0100 00da 0e6f 6e5f 656e  G...r).....on_en
-00007730: 7472 795f 666f 6375 7372 4d00 0000 722e  try_focusrM...r.
-00007740: 0000 0072 2e00 0000 722f 0000 0072 2600  ...r....r/...r&.
-00007750: 0000 c603 0000 730a 0000 0000 030c 0102  ......s.........
-00007760: ff08 020e 027a 1a5f 4c69 7374 456e 7472  .....z._ListEntr
-00007770: 792e 5f63 7265 6174 655f 7769 6467 6574  y._create_widget
-00007780: 7363 0100 0000 0000 0000 0000 0000 0200  sc..............
-00007790: 0000 0300 0000 4300 0000 7324 0000 007c  ......C...s$...|
-000077a0: 006a 0064 016b 0272 0e64 026e 0264 037d  .j.d.k.r.d.n.d.}
-000077b0: 017c 006a 016a 027c 0164 048d 0101 0064  .|.j.j.|.d.....d
-000077c0: 0553 0029 0672 7501 0000 7234 0000 0072  .S.).ru...r4...r
-000077d0: 0b01 0000 720c 0100 0072 c200 0000 4e29  ....r....r....N)
-000077e0: 0372 5700 0000 7276 0100 0072 8400 0000  .rW...rv...r....
-000077f0: 72c3 0000 0072 2e00 0000 722e 0000 0072  r....r....r....r
-00007800: 2f00 0000 725e 0000 00cf 0300 0073 0400  /...r^.......s..
-00007810: 0000 0003 1201 7a20 5f4c 6973 7445 6e74  ......z _ListEnt
-00007820: 7279 2e5f 7570 6461 7465 5f77 6964 6765  ry._update_widge
-00007830: 7473 5f73 7479 6c65 6301 0000 0000 0000  ts_stylec.......
-00007840: 0000 0000 0001 0000 0003 0000 0043 0000  .............C..
-00007850: 0073 1200 0000 6401 7c00 6a00 a001 a100  .s....d.|.j.....
-00007860: 9b00 6402 9d03 5300 72a7 0000 0029 0272  ..d...S.r....).r
-00007870: 7601 0000 7221 0000 0072 4d00 0000 722e  v...r!...rM...r.
-00007880: 0000 0072 2e00 0000 722f 0000 00da 155f  ...r....r/....._
-00007890: 6765 745f 7374 6174 7573 5f65 7272 6f72  get_status_error
-000078a0: 5f6d 7367 d503 0000 7302 0000 0000 017a  _msg....s......z
-000078b0: 205f 4c69 7374 456e 7472 792e 5f67 6574   _ListEntry._get
-000078c0: 5f73 7461 7475 735f 6572 726f 725f 6d73  _status_error_ms
-000078d0: 6763 0200 0000 0000 0000 0000 0000 0200  gc..............
-000078e0: 0000 0400 0000 4300 0000 732a 0000 007c  ......C...s*...|
-000078f0: 006a 0064 016b 0272 1c7c 006a 01a0 027c  .j.d.k.r.|.j...|
-00007900: 00a0 03a1 00a1 0101 006e 0a7c 006a 01a0  .........n.|.j..
-00007910: 04a1 0001 0064 0253 0029 037a 7c49 6620  .....d.S.).z|If 
-00007920: 7573 6572 2066 6f63 7573 206f 6e20 6120  user focus on a 
-00007930: 6365 6c6c 2c20 0a20 2020 2020 2020 200a  cell, .        .
-00007940: 2020 2020 2020 2020 616e 6420 6365 6c6c          and cell
-00007950: 2069 7320 696e 7661 6c69 642c 2075 7064   is invalid, upd
-00007960: 6174 6520 4c69 7374 2065 7272 6f72 206d  ate List error m
-00007970: 6573 7361 6765 0a20 2020 2020 2020 2065  essage.        e
-00007980: 6c73 6520 6d61 6b65 2069 7420 766f 6964  lse make it void
-00007990: 0a20 2020 2020 2020 2072 b500 0000 4e29  .        r....N)
-000079a0: 0572 5700 0000 722a 0000 0072 a900 0000  .rW...r*...r....
-000079b0: 7278 0100 00da 145f 7570 6461 7465 5f73  rx....._update_s
-000079c0: 7461 7475 735f 6c61 6265 6c72 3401 0000  tatus_labelr4...
-000079d0: 722e 0000 0072 2e00 0000 722f 0000 0072  r....r....r/...r
-000079e0: 7701 0000 d803 0000 7306 0000 0000 060a  w.......s.......
-000079f0: 0112 027a 195f 4c69 7374 456e 7472 792e  ...z._ListEntry.
-00007a00: 6f6e 5f65 6e74 7279 5f66 6f63 7573 6301  on_entry_focusc.
-00007a10: 0000 0000 0000 0000 0000 0002 0000 0001  ................
-00007a20: 0000 0047 0000 0073 0400 0000 6401 5300  ...G...s....d.S.
-00007a30: 2902 7a24 5265 6d6f 7665 2074 6865 2075  ).z$Remove the u
-00007a40: 7375 616c 2063 7265 6174 696f 6e20 6f66  sual creation of
-00007a50: 2077 6964 6765 7473 4e72 2e00 0000 725a   widgetsNr....rZ
-00007a60: 0000 0072 2e00 0000 722e 0000 0072 2f00  ...r....r....r/.
-00007a70: 0000 7224 0000 00e7 0300 0073 0200 0000  ..r$.......s....
-00007a80: 0002 7a26 5f4c 6973 7445 6e74 7279 2e5f  ..z&_ListEntry._
-00007a90: 6372 6561 7465 5f63 6f6d 6d6f 6e5f 6c65  create_common_le
-00007aa0: 6166 5f77 6964 6765 7473 6301 0000 0000  af_widgetsc.....
-00007ab0: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
-00007ac0: 0000 0073 0a00 0000 7c00 6a00 6401 1900  ...s....|.j.d...
-00007ad0: 5300 2902 4e72 4801 0000 2901 7220 0000  S.).NrH...).r ..
-00007ae0: 0072 4d00 0000 722e 0000 0072 2e00 0000  .rM...r....r....
-00007af0: 722f 0000 0072 5b01 0000 ec03 0000 7302  r/...r[.......s.
-00007b00: 0000 0000 027a 145f 4c69 7374 456e 7472  .....z._ListEntr
-00007b10: 792e 6974 656d 5f74 7970 6563 0100 0000  y.item_typec....
-00007b20: 0000 0000 0000 0000 0100 0000 0200 0000  ................
-00007b30: 4300 0000 730c 0000 007c 006a 007c 005f  C...s....|.j.|._
-00007b40: 0164 0053 0072 4c00 0000 2902 7273 0100  .d.S.rL...).rs..
-00007b50: 0072 4f00 0000 724d 0000 0072 2e00 0000  .rO...rM...r....
-00007b60: 722e 0000 0072 2f00 0000 7223 0000 00f0  r....r/...r#....
-00007b70: 0300 0073 0200 0000 0001 7a1f 5f4c 6973  ...s......z._Lis
-00007b80: 7445 6e74 7279 2e5f 696e 6974 5f70 7265  tEntry._init_pre
-00007b90: 7669 6f75 735f 7661 6c75 6563 0200 0000  vious_valuec....
-00007ba0: 0000 0000 0000 0000 0200 0000 0200 0000  ................
-00007bb0: 4300 0000 7330 0000 007c 006a 0064 016b  C...s0...|.j.d.k
-00007bc0: 0272 1274 017c 0183 0153 007c 006a 0064  .r.t.|...S.|.j.d
-00007bd0: 026b 0272 2474 027c 0183 0153 0074 037c  .k.r$t.|...S.t.|
-00007be0: 0183 0153 0064 0353 0029 047a 2b53 7472  ...S.d.S.).z+Str
-00007bf0: 6f6e 676c 7920 7479 7065 2074 6865 2076  ongly type the v
-00007c00: 616c 7565 2065 6e74 6572 6564 2062 7920  alue entered by 
-00007c10: 7468 6520 7573 6572 7257 0100 0072 9e00  the userrW...r..
-00007c20: 0000 4e29 0472 5b01 0000 7298 0000 0072  ..N).r[...r....r
-00007c30: 4900 0000 7268 0100 0072 7100 0000 722e  I...rh...rq...r.
-00007c40: 0000 0072 2e00 0000 722f 0000 0072 a100  ...r....r/...r..
-00007c50: 0000 f303 0000 730a 0000 0000 020a 0108  ......s.........
-00007c60: 010a 0108 027a 135f 4c69 7374 456e 7472  .....z._ListEntr
-00007c70: 792e 7374 7232 7479 7065 6301 0000 0000  y.str2typec.....
-00007c80: 0000 0000 0000 0001 0000 0004 0000 0043  ...............C
-00007c90: 0000 0073 1c00 0000 7400 8300 7c00 5f01  ...s....t...|._.
-00007ca0: 7c00 6a01 a002 6401 7c00 6a03 a102 0100  |.j...d.|.j.....
-00007cb0: 6400 5300 726a 0000 0072 6c00 0000 724d  d.S.rj...rl...rM
-00007cc0: 0000 0072 2e00 0000 722e 0000 0072 2f00  ...r....r....r/.
-00007cd0: 0000 7225 0000 00fc 0300 0073 0400 0000  ..r%.......s....
-00007ce0: 0002 0801 7a16 5f4c 6973 7445 6e74 7279  ....z._ListEntry
-00007cf0: 2e5f 6465 6669 6e65 5f76 6172 6301 0000  ._define_varc...
-00007d00: 0000 0000 0000 0000 0003 0000 0008 0000  ................
-00007d10: 0047 0000 0073 5200 0000 7a24 7c00 a000  .G...sR...z$|...
-00007d20: a100 7d02 7c00 6a01 7c02 6b02 721c 6401  ..}.|.j.|.k.r.d.
-00007d30: 7c00 5f02 6e06 6402 7c00 5f02 5700 6e28  |._.n.d.|._.W.n(
-00007d40: 0400 7403 794c 0100 0100 0100 6403 7c00  ..t.yL......d.|.
-00007d50: 5f02 7c00 6a04 a005 7c00 a006 a100 a101  _.|.j...|.......
-00007d60: 0100 5900 6e02 3000 6404 5300 2905 7a18  ..Y.n.0.d.S.).z.
-00007d70: 4361 6c6c 6261 636b 2069 6620 7661 6c75  Callback if valu
-00007d80: 6520 6368 616e 6765 7234 0000 0072 0100  e changer4...r..
-00007d90: 0000 72b5 0000 004e 2907 7221 0000 0072  ..r....N).r!...r
-00007da0: 4f00 0000 7257 0000 0072 0f00 0000 722a  O...rW...r....r*
-00007db0: 0000 0072 a900 0000 7278 0100 0029 0372  ...r....rx...).r
-00007dc0: 2900 0000 725b 0000 0072 7200 0000 722e  )...r[...rr...r.
-00007dd0: 0000 0072 2e00 0000 722f 0000 0072 5c00  ...r....r/...r\.
-00007de0: 0000 0104 0000 7310 0000 0000 0302 0108  ......s.........
-00007df0: 010a 0108 020a 020c 0106 017a 1a5f 4c69  ...........z._Li
-00007e00: 7374 456e 7472 792e 6f6e 5f76 616c 7565  stEntry.on_value
-00007e10: 5f63 6861 6e67 6563 0100 0000 0000 0000  _changec........
-00007e20: 0000 0000 0100 0000 0800 0000 4300 0000  ............C...
-00007e30: 7330 0000 007a 127c 00a0 007c 006a 01a0  s0...z.|...|.j..
-00007e40: 02a1 00a1 0157 0053 0004 0074 0379 2a01  .....W.S...t.y*.
-00007e50: 0001 0001 0074 0483 0082 0159 006e 0230  .....t.....Y.n.0
-00007e60: 0064 0153 0029 027a 126f 7065 6e74 6561  .d.S.).z.opentea
-00007e70: 2047 4554 206d 6574 686f 644e 72a2 0000   GET methodNr...
-00007e80: 0072 4d00 0000 722e 0000 0072 2e00 0000  .rM...r....r....
-00007e90: 722f 0000 0072 2100 0000 1204 0000 7308  r/...r!.......s.
-00007ea0: 0000 0000 0202 0112 010c 017a 0e5f 4c69  ...........z._Li
-00007eb0: 7374 456e 7472 792e 6765 7463 0200 0000  stEntry.getc....
-00007ec0: 0000 0000 0000 0000 0200 0000 0800 0000  ................
-00007ed0: 4300 0000 7334 0000 007a 167c 006a 00a0  C...s4...z.|.j..
-00007ee0: 017c 00a0 027c 01a1 01a1 0101 0057 006e  .|...|.......W.n
-00007ef0: 1804 0074 0379 2e01 0001 0001 0074 0483  ...t.y.......t..
-00007f00: 0082 0159 006e 0230 0064 0153 0029 027a  ...Y.n.0.d.S.).z
-00007f10: 126f 7065 6e74 6561 2053 4554 206d 6574  .opentea SET met
-00007f20: 686f 644e 2905 726d 0000 0072 5100 0000  hodN).rm...rQ...
-00007f30: 72a1 0000 0072 a300 0000 7210 0000 0072  r....r....r....r
-00007f40: 7100 0000 722e 0000 0072 2e00 0000 722f  q...r....r....r/
-00007f50: 0000 0072 5100 0000 1904 0000 7308 0000  ...rQ.......s...
-00007f60: 0000 0302 0116 010c 017a 0e5f 4c69 7374  .........z._List
-00007f70: 456e 7472 792e 7365 7463 0100 0000 0000  Entry.setc......
-00007f80: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
-00007f90: 0000 7318 0000 007c 00a0 0064 01a1 0101  ..s....|...d....
-00007fa0: 007c 006a 01a0 02a1 0001 0064 0053 0072  .|.j.......d.S.r
-00007fb0: 5d00 0000 2903 7260 0000 0072 7601 0000  ]...).r`...rv...
-00007fc0: 7261 0000 0072 4d00 0000 722e 0000 0072  ra...rM...r....r
-00007fd0: 2e00 0000 722f 0000 0072 6100 0000 2204  ....r/...ra...".
-00007fe0: 0000 7304 0000 0000 010a 027a 125f 4c69  ..s........z._Li
-00007ff0: 7374 456e 7472 792e 6465 7374 726f 7929  stEntry.destroy)
-00008000: 014e 2914 7263 0000 0072 6400 0000 7265  .N).rc...rd...re
-00008010: 0000 0072 6600 0000 721f 0000 0072 2600  ...rf...r....r&.
-00008020: 0000 725e 0000 0072 7801 0000 7277 0100  ..r^...rx...rw..
-00008030: 0072 2400 0000 da08 7072 6f70 6572 7479  .r$.....property
-00008040: 725b 0100 0072 2300 0000 72a1 0000 0072  r[...r#...r....r
-00008050: 2500 0000 725c 0000 0072 2100 0000 7251  %...r\...r!...rQ
-00008060: 0000 0072 6100 0000 7267 0000 0072 2e00  ...ra...rg...r..
-00008070: 0000 722e 0000 0072 2c00 0000 722f 0000  ..r....r,...r/..
-00008080: 0072 7201 0000 ba03 0000 7320 0000 0008  .rr.......s ....
-00008090: 0104 040e 0708 0908 0608 0308 0f08 0502  ................
-000080a0: 010a 0308 0308 0908 0508 1108 0708 0972  ...............r
-000080b0: 7201 0000 6300 0000 0000 0000 0000 0000  r...c...........
-000080c0: 0000 0000 0003 0000 0000 0000 0073 f800  .............s..
-000080d0: 0000 6500 5a01 6400 5a02 6401 5a03 8700  ..e.Z.d.Z.d.Z...
-000080e0: 6601 6402 6403 8408 5a04 8700 6601 6404  f.d.d...Z...f.d.
-000080f0: 6405 8408 5a05 6506 6406 6407 8400 8301  d...Z.e.d.d.....
-00008100: 5a07 6408 6409 8400 5a08 640a 640b 8400  Z.d.d...Z.d.d...
-00008110: 5a09 640c 640d 8400 5a0a 8700 6601 640e  Z.d.d...Z...f.d.
-00008120: 640f 8408 5a0b 6410 6411 8400 5a0c 6412  d...Z.d.d...Z.d.
-00008130: 6413 8400 5a0d 6414 6415 8400 5a0e 6416  d...Z.d.d...Z.d.
-00008140: 6417 8400 5a0f 6418 6419 8400 5a10 641a  d...Z.d.d...Z.d.
-00008150: 641b 8400 5a11 641c 641d 8400 5a12 641e  d...Z.d.d...Z.d.
-00008160: 641f 8400 5a13 6420 6421 8400 5a14 6422  d...Z.d d!..Z.d"
-00008170: 6423 8400 5a15 6424 6425 8400 5a16 6437  d#..Z.d$d%..Z.d7
-00008180: 6427 6428 8401 5a17 6438 6429 642a 8401  d'd(..Z.d8d)d*..
-00008190: 5a18 642b 642c 8400 5a19 642d 642e 8400  Z.d+d,..Z.d-d...
-000081a0: 5a1a 642f 6430 8400 5a1b 6431 6432 8400  Z.d/d0..Z.d1d2..
-000081b0: 5a1c 6433 6434 8400 5a1d 6435 6436 8400  Z.d3d4..Z.d5d6..
-000081c0: 5a1e 8700 0400 5a1f 5300 2939 da0d 4f54  Z.....Z.S.)9..OT
-000081d0: 4479 6e61 6d69 634c 6973 747a 1b4c 6973  DynamicListz.Lis
-000081e0: 7420 636f 6e74 726f 6c6c 6564 2062 7920  t controlled by 
-000081f0: 7468 6520 7573 6572 6305 0000 0000 0000  the userc.......
-00008200: 0000 0000 0005 0000 0006 0000 0003 0000  ................
-00008210: 0073 5a00 0000 6401 7c00 5f00 6401 7c00  .sZ...d.|._.d.|.
-00008220: 5f01 6402 7c00 5f02 7c01 6403 1900 6404  _.d.|._.|.d...d.
-00008230: 1900 7c00 5f03 7c01 a004 6405 7405 6406  ..|._.|...d.t.d.
-00008240: 8301 a102 7c00 5f06 7c01 a004 6407 7405  ....|._.|...d.t.
-00008250: 6408 8301 a102 7c00 5f07 7408 8300 a009  d.....|._.t.....
-00008260: 7c01 7c02 7c03 7c04 a104 0100 6402 5300  |.|.|.|.....d.S.
-00008270: 2909 7adc 5374 6172 7475 7020 636c 6173  ).z.Startup clas
-00008280: 732e 0a0a 2020 2020 2020 2020 496e 7075  s...        Inpu
-00008290: 7473 203a 0a20 2020 2020 2020 202d 2d2d  ts :.        ---
-000082a0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 7363  -----.        sc
-000082b0: 6865 6d61 203a 2061 2073 6368 656d 6120  hema : a schema 
-000082c0: 6173 2061 206e 6573 7465 6420 6f62 6a65  as a nested obje
-000082d0: 6374 0a20 2020 2020 2020 2070 6172 656e  ct.        paren
-000082e0: 743a 203f 3f3f 0a20 2020 2020 2020 206e  t: ???.        n
-000082f0: 616d 653a 206e 616d 6520 746f 2062 6520  ame: name to be 
-00008300: 6164 6465 640a 2020 2020 2020 2020 726f  added.        ro
-00008310: 6f74 5f66 7261 6d65 203a 2020 6120 546b  ot_frame :  a Tk
-00008320: 206f 626a 6563 7420 7765 7265 2074 6865   object were the
-00008330: 2077 6964 6765 7420 7769 6c6c 2062 6520   widget will be 
-00008340: 6772 6166 7465 640a 2020 2020 2020 2020  grafted.        
-00008350: 7201 0000 004e 72dd 0000 0072 4801 0000  r....Nr....rH...
-00008360: 7259 0100 007a 042d 696e 6672 5801 0000  rY...z.-infrX...
-00008370: 7294 0000 0029 0ada 0f5f 7374 6174 7573  r....)..._status
-00008380: 5f69 6e76 616c 6964 da0c 5f73 7461 7475  _invalid.._statu
-00008390: 735f 7465 6d70 da0c 656d 7074 795f 7769  s_temp..empty_wi
-000083a0: 6467 6574 725b 0100 0072 2100 0000 7298  dgetr[...r!...r.
-000083b0: 0000 00da 096d 696e 5f69 7465 6d73 da09  .....min_items..
-000083c0: 6d61 785f 6974 656d 7372 1e00 0000 721f  max_itemsr....r.
-000083d0: 0000 0072 2800 0000 722c 0000 0072 2e00  ...r(...r,...r..
-000083e0: 0000 722f 0000 0072 1f00 0000 2b04 0000  ..r/...r....+...
-000083f0: 730e 0000 0000 0a06 0106 0306 030e 0212  s...............
-00008400: 0112 027a 164f 5444 796e 616d 6963 4c69  ...z.OTDynamicLi
-00008410: 7374 2e5f 5f69 6e69 745f 5f63 0100 0000  st.__init__c....
-00008420: 0000 0000 0000 0000 0100 0000 0200 0000  ................
-00008430: 0300 0000 731e 0000 0074 0083 00a0 01a1  ....s....t......
-00008440: 0001 007c 00a0 02a1 0001 007c 00a0 03a1  ...|.......|....
-00008450: 0001 0064 0153 0029 027a 2b41 6464 206d  ...d.S.).z+Add m
-00008460: 6f72 6520 746f 205f 4f54 4162 7374 7261  ore to _OTAbstra
-00008470: 6374 4c69 7374 2e5f 6372 6561 7465 5f77  ctList._create_w
-00008480: 6964 6765 7473 4e29 0472 1e00 0000 7226  idgetsN).r....r&
-00008490: 0000 0072 8900 0000 da0f 5f63 6f6e 6669  ...r......_confi
-000084a0: 675f 6275 7474 6f6e 7372 4d00 0000 722c  g_buttonsrM...r,
-000084b0: 0000 0072 2e00 0000 722f 0000 0072 2600  ...r....r/...r&.
-000084c0: 0000 4404 0000 7306 0000 0000 020a 0108  ..D...s.........
-000084d0: 017a 1d4f 5444 796e 616d 6963 4c69 7374  .z.OTDynamicList
-000084e0: 2e5f 6372 6561 7465 5f77 6964 6765 7473  ._create_widgets
-000084f0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00008500: 0002 0000 0043 0000 0073 0c00 0000 7c00  .....C...s....|.
-00008510: 6a00 7c00 6a01 6b03 5300 2901 7a1c 5472  j.|.j.k.S.).z.Tr
-00008520: 7565 2069 6620 6c69 7374 2063 616e 2063  ue if list can c
-00008530: 6861 6e67 6520 7369 7a65 2902 727f 0100  hange size).r...
-00008540: 0072 8001 0000 724d 0000 0072 2e00 0000  .r....rM...r....
-00008550: 722e 0000 0072 2f00 0000 da09 7265 7369  r....r/.....resi
-00008560: 7a61 626c 654a 0400 0073 0200 0000 0003  zableJ...s......
-00008570: 7a17 4f54 4479 6e61 6d69 634c 6973 742e  z.OTDynamicList.
-00008580: 7265 7369 7a61 626c 6563 0100 0000 0000  resizablec......
-00008590: 0000 0000 0000 0200 0000 0600 0000 4300  ..............C.
-000085a0: 0000 733a 0000 0074 006a 017c 006a 0264  ..s:...t.j.|.j.d
-000085b0: 0164 0264 0364 048d 047c 005f 037c 006a  .d.d.d...|._.|.j
-000085c0: 0472 2064 056e 0264 067d 017c 006a 036a  .r d.n.d.}.|.j.j
-000085d0: 057c 0164 0664 0764 088d 0301 0064 0053  .|.d.d.d.....d.S
-000085e0: 0029 094e 728d 0000 0072 8e00 0000 728f  .).Nr....r....r.
-000085f0: 0000 0072 9000 0000 729f 0000 0072 7a00  ...r....r....rz.
-00008600: 0000 728c 0000 0072 4000 0000 2906 7202  ..r....r@...).r.
-00008610: 0000 0072 4800 0000 7245 0000 0072 9700  ...rH...rE...r..
-00008620: 0000 7282 0100 0072 4b00 0000 2902 7229  ..r....rK...).r)
-00008630: 0000 0072 4100 0000 722e 0000 0072 2e00  ...rA...r....r..
-00008640: 0000 722f 0000 0072 8900 0000 4f04 0000  ..r/...r....O...
-00008650: 730c 0000 0000 0104 0108 0102 fe08 030e  s...............
-00008660: 017a 224f 5444 796e 616d 6963 4c69 7374  .z"OTDynamicList
-00008670: 2e5f 636f 6e66 6967 5f73 7461 7475 735f  ._config_status_
-00008680: 6c61 6265 6c63 0100 0000 0000 0000 0000  labelc..........
-00008690: 0000 0100 0000 0600 0000 4300 0000 7362  ..........C...sb
-000086a0: 0000 007c 006a 0073 0a64 0153 0074 016a  ...|.j.s.d.S.t.j
-000086b0: 027c 006a 0364 027c 006a 0464 038d 037c  .|.j.d.|.j.d...|
-000086c0: 005f 0574 016a 027c 006a 0364 047c 006a  ._.t.j.|.j.d.|.j
-000086d0: 0664 038d 037c 005f 077c 006a 056a 0864  .d...|._.|.j.j.d
-000086e0: 0564 0664 0764 0864 098d 0401 007c 006a  .d.d.d.d.....|.j
-000086f0: 076a 0864 0564 0a64 0764 0864 098d 0401  .j.d.d.d.d.d....
-00008700: 0064 0153 0029 0b7a 1149 6e69 7469 616c  .d.S.).z.Initial
-00008710: 6973 6520 656e 7472 792e 4efa 012b 2902  ise entry.N..+).
-00008720: 723c 0000 0072 bf00 0000 da01 2d67 9a99  r<...r......-g..
-00008730: 9999 9999 a93f 6766 6666 6666 66ee 3f72  .....?gffffff.?r
-00008740: 7a00 0000 728c 0000 0072 5301 0000 7234  z...r....rS...r4
-00008750: 0000 0029 0972 8201 0000 7202 0000 0072  ...).r....r....r
-00008760: fa00 0000 7245 0000 00da 0b6f 6e5f 6164  ....rE.....on_ad
-00008770: 645f 6974 656d 5a0a 6164 6469 7465 6d5f  d_itemZ.additem_
-00008780: 6274 da0b 6f6e 5f64 656c 5f69 7465 6d5a  bt..on_del_itemZ
-00008790: 0a64 656c 6974 656d 5f62 7472 4b00 0000  .delitem_btrK...
-000087a0: 724d 0000 0072 2e00 0000 722e 0000 0072  rM...r....r....r
-000087b0: 2f00 0000 7281 0100 0056 0400 0073 2400  /...r....V...s$.
-000087c0: 0000 0002 0601 0402 0801 0201 04fe 0803  ................
-000087d0: 0801 0201 04fe 0804 0801 0201 04fe 0603  ................
-000087e0: 0801 0201 04fe 7a1d 4f54 4479 6e61 6d69  ......z.OTDynami
-000087f0: 634c 6973 742e 5f63 6f6e 6669 675f 6275  cList._config_bu
-00008800: 7474 6f6e 7363 0100 0000 0000 0000 0000  ttonsc..........
-00008810: 0000 0100 0000 0400 0000 4300 0000 7328  ..........C...s(
-00008820: 0000 007c 006a 006a 0164 017c 006a 0264  ...|.j.j.d.|.j.d
-00008830: 028d 0201 007c 006a 006a 0164 037c 006a  .....|.j.j.d.|.j
-00008840: 0364 028d 0201 0064 0453 0029 05fa 2652  .d.....d.S.)..&R
-00008850: 652d 6465 6669 6e65 205f 4f54 4162 7374  e-define _OTAbst
-00008860: 7261 6374 4c69 7374 2076 6f69 6420 6d65  ractList void me
-00008870: 7468 6f64 20da 0443 6f70 79a9 02da 056c  thod ..Copy....l
-00008880: 6162 656c 72bf 0000 005a 0550 6173 7465  abelr....Z.Paste
-00008890: 4e29 0472 5d01 0000 da0b 6164 645f 636f  N).r].....add_co
-000088a0: 6d6d 616e 6472 6f01 0000 da08 6f6e 5f70  mmandro.....on_p
-000088b0: 6173 7465 724d 0000 0072 2e00 0000 722e  asterM...r....r.
-000088c0: 0000 0072 2f00 0000 725e 0100 0069 0400  ...r/...r^...i..
-000088d0: 0073 0400 0000 0002 1201 7a21 4f54 4479  .s........z!OTDy
-000088e0: 6e61 6d69 634c 6973 742e 5f61 6464 5f70  namicList._add_p
-000088f0: 6f70 7570 5f63 6f6d 6d61 6e64 7363 0100  opup_commandsc..
-00008900: 0000 0000 0000 0000 0000 0200 0000 0500  ................
-00008910: 0000 0300 0000 7332 0000 0074 0064 0164  ......s2...t.d.d
-00008920: 0274 017c 006a 0283 0117 0083 027d 017c  .t.|.j.......}.|
-00008930: 006a 0372 227c 0164 0337 007d 0174 0483  .j.r"|.d.7.}.t..
-00008940: 00a0 057c 01a1 0101 0064 0453 0029 057a  ...|.....d.S.).z
-00008950: 2541 646a 7573 7420 686f 6c64 6572 2073  %Adjust holder s
-00008960: 697a 6520 746f 2069 6e74 6572 6e20 7661  ize to intern va
-00008970: 7269 6162 6c65 728a 0000 0072 3400 0000  riabler....r4...
-00008980: 723b 0000 004e 2906 72d5 0000 0072 ca00  r;...N).r....r..
-00008990: 0000 da09 7661 7269 6162 6c65 7372 8201  ....variablesr..
-000089a0: 0000 721e 0000 0072 7101 0000 7270 0100  ..r....rq...rp..
-000089b0: 0072 2c00 0000 722e 0000 0072 2f00 0000  .r,...r....r/...
-000089c0: 7271 0100 006e 0400 0073 0800 0000 0002  rq...n...s......
-000089d0: 1401 0601 0801 7a1c 4f54 4479 6e61 6d69  ......z.OTDynami
-000089e0: 634c 6973 742e 5f72 6573 697a 655f 686f  cList._resize_ho
-000089f0: 6c64 6572 6301 0000 0000 0000 0000 0000  lderc...........
-00008a00: 0002 0000 0004 0000 0043 0000 0073 3400  .........C...s4.
-00008a10: 0000 7c00 6a00 6401 7501 720e 6401 5300  ..|.j.d.u.r.d.S.
-00008a20: 7401 6a02 7c00 6a03 6402 6403 8d02 7d01  t.j.|.j.d.d...}.
-00008a30: 7c01 6a04 6404 6405 8d01 0100 7c01 7c00  |.j.d.d.....|.|.
-00008a40: 5f00 6401 5300 2906 7a17 4164 6420 6e65  _.d.S.).z.Add ne
-00008a50: 7720 656e 7472 7920 746f 2068 6f6c 6465  w entry to holde
-00008a60: 724e 7247 0100 0072 4a01 0000 7235 0000  rNrG...rJ...r5..
-00008a70: 0072 3601 0000 2905 727e 0100 0072 0200  .r6...).r~...r..
-00008a80: 0000 7248 0000 0072 5401 0000 7247 0000  ..rH...rT...rG..
-00008a90: 0029 0272 2900 0000 728a 0100 0072 2e00  .).r)...r....r..
-00008aa0: 0000 722e 0000 0072 2f00 0000 da11 6372  ..r....r/.....cr
-00008ab0: 6561 7465 5f76 6f69 645f 656e 7472 7975  eate_void_entryu
-00008ac0: 0400 0073 0a00 0000 0002 0a01 0402 1001  ...s............
-00008ad0: 0c01 7a1f 4f54 4479 6e61 6d69 634c 6973  ..z.OTDynamicLis
-00008ae0: 742e 6372 6561 7465 5f76 6f69 645f 656e  t.create_void_en
-00008af0: 7472 7963 0100 0000 0000 0000 0000 0000  tryc............
-00008b00: 0700 0000 0900 0000 4700 0000 73cc 0000  ........G...s...
-00008b10: 007a 1274 007c 006a 0183 01a0 02a1 007d  .z.t.|.j.......}
-00008b20: 0257 006e 1a04 0074 036a 046a 0579 2c01  .W.n...t.j.j.y,.
-00008b30: 0001 0001 0064 017d 0259 006e 0230 007c  .....d.}.Y.n.0.|
-00008b40: 0273 4274 066a 0764 0264 038d 0101 0064  .sBt.j.d.d.....d
-00008b50: 0453 0064 0564 0684 007c 02a0 0864 07a1  .S.d.d...|...d..
-00008b60: 0144 0083 017d 037c 006a 0972 667c 006a  .D...}.|.j.rf|.j
-00008b70: 0964 0819 006e 0e74 0a7c 007c 006a 0b7c  .d...n.t.|.|.j.|
-00008b80: 006a 0c83 037d 047c 0344 005d 427d 057a  .j...}.|.D.]B}.z
-00008b90: 0e7c 04a0 0d7c 05a1 0101 0057 0071 7a04  .|...|.....W.qz.
-00008ba0: 0074 0e79 ba01 0001 0001 0064 097c 029b  .t.y.......d.|..
-00008bb0: 0064 0a9d 037d 0674 066a 077c 0664 038d  .d...}.t.j.|.d..
-00008bc0: 0101 0059 0001 0064 0453 0030 0071 7a7c  ...Y...d.S.0.qz|
-00008bd0: 00a0 0f7c 03a1 0101 0064 0453 0029 0b7a  ...|.....d.S.).z
-00008be0: 1143 616c 6c62 6163 6b20 6f6e 2070 6173  .Callback on pas
-00008bf0: 7465 7254 0000 007a 104e 6f74 6869 6e67  terT...z.Nothing
-00008c00: 2074 6f20 7061 7374 6529 01da 076d 6573   to paste)...mes
-00008c10: 7361 6765 4e63 0100 0000 0000 0000 0000  sageNc..........
-00008c20: 0000 0200 0000 0400 0000 5300 0000 7314  ..........S...s.
-00008c30: 0000 0067 007c 005d 0c7d 017c 01a0 00a1  ...g.|.].}.|....
-00008c40: 0091 0271 0453 0072 2e00 0000 2901 da05  ...q.S.r....)...
-00008c50: 7374 7269 7072 6901 0000 722e 0000 0072  stripri...r....r
-00008c60: 2e00 0000 722f 0000 0072 6b01 0000 8a04  ....r/...rk.....
-00008c70: 0000 726c 0100 007a 2a4f 5444 796e 616d  ..rl...z*OTDynam
-00008c80: 6963 4c69 7374 2e6f 6e5f 7061 7374 652e  icList.on_paste.
-00008c90: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
-00008ca0: 6d70 3efa 012c 7201 0000 007a 1449 6e76  mp>..,r....z.Inv
-00008cb0: 616c 6964 2063 6c69 7062 6f61 7264 3a0a  alid clipboard:.
-00008cc0: 27fa 0127 2910 7217 0000 0072 4500 0000  '..').r....rE...
-00008cd0: da0d 636c 6970 626f 6172 645f 6765 74da  ..clipboard_get.
-00008ce0: 0774 6b69 6e74 6572 da08 5f74 6b69 6e74  .tkinter.._tkint
-00008cf0: 6572 da08 5463 6c45 7272 6f72 720c 0000  er..TclErrorr...
-00008d00: 00da 0b73 686f 7777 6172 6e69 6e67 da05  ...showwarning..
-00008d10: 7370 6c69 7472 8d01 0000 7272 0100 0072  splitr....rr...r
-00008d20: 5401 0000 725b 0100 0072 a100 0000 72a3  T...r[...r....r.
-00008d30: 0000 0072 5100 0000 2907 7229 0000 0072  ...rQ...).r)...r
-00008d40: 5b00 0000 5a09 7061 7374 655f 7374 725a  [...Z.paste_strZ
-00008d50: 0870 6173 7465 5f6c 73da 0376 6172 7272  .paste_ls..varrr
-00008d60: 0000 0072 8f01 0000 722e 0000 0072 2e00  ...r....r....r..
-00008d70: 0000 722f 0000 0072 8c01 0000 7f04 0000  ..r/...r........
-00008d80: 7326 0000 0000 0202 0112 0110 010a 0204  s&..............
-00008d90: 010c 0104 0214 0412 010a ff04 0208 0102  ................
-00008da0: 010e 010c 010c 010c 010c 037a 164f 5444  ...........z.OTD
-00008db0: 796e 616d 6963 4c69 7374 2e6f 6e5f 7061  ynamicList.on_pa
-00008dc0: 7374 6563 0100 0000 0000 0000 0000 0000  stec............
-00008dd0: 0100 0000 0200 0000 4300 0000 7320 0000  ........C...s ..
-00008de0: 0074 007c 006a 0183 017c 006a 026b 0272  .t.|.j...|.j.k.r
-00008df0: 1464 0153 007c 00a0 03a1 0001 0064 0153  .d.S.|.......d.S
-00008e00: 0029 027a 3663 616c 6c62 6163 6b20 4164  .).z6callback Ad
-00008e10: 6420 616e 2069 7465 6d20 6174 2074 6865  d an item at the
-00008e20: 2065 6e64 206f 6620 7468 6520 6172 7261   end of the arra
-00008e30: 792e 0a20 2020 2020 2020 204e 2904 72ca  y..        N).r.
-00008e40: 0000 0072 8d01 0000 7280 0100 00da 095f  ...r....r......_
-00008e50: 6164 645f 6974 656d 724d 0000 0072 2e00  add_itemrM...r..
-00008e60: 0000 722e 0000 0072 2f00 0000 7285 0100  ..r....r/...r...
-00008e70: 009b 0400 0073 0600 0000 0004 1001 0402  .....s..........
-00008e80: 7a19 4f54 4479 6e61 6d69 634c 6973 742e  z.OTDynamicList.
-00008e90: 6f6e 5f61 6464 5f69 7465 6d63 0100 0000  on_add_itemc....
-00008ea0: 0000 0000 0000 0000 0100 0000 0300 0000  ................
-00008eb0: 4300 0000 7322 0000 0074 007c 006a 0183  C...s"...t.|.j..
-00008ec0: 017c 006a 026b 0272 1464 0153 007c 00a0  .|.j.k.r.d.S.|..
-00008ed0: 0364 02a1 0101 0064 0153 0029 037a 3643  .d.....d.S.).z6C
-00008ee0: 616c 6c62 6163 6b20 4465 6c65 7465 2069  allback Delete i
-00008ef0: 7465 6d20 6174 2074 6865 2065 6e64 206f  tem at the end o
-00008f00: 6620 7468 6520 6172 7261 792e 0a20 2020  f the array..   
-00008f10: 2020 2020 204e 7234 0000 0029 0472 ca00       Nr4...).r..
-00008f20: 0000 728d 0100 0072 7f01 0000 da0c 7265  ..r....r......re
-00008f30: 6d6f 7665 5f69 7465 6d73 724d 0000 0072  move_itemsrM...r
-00008f40: 2e00 0000 722e 0000 0072 2f00 0000 7286  ....r....r/...r.
-00008f50: 0100 00a4 0400 0073 0600 0000 0003 1001  .......s........
-00008f60: 0402 7a19 4f54 4479 6e61 6d69 634c 6973  ..z.OTDynamicLis
-00008f70: 742e 6f6e 5f64 656c 5f69 7465 6d63 0200  t.on_del_itemc..
-00008f80: 0000 0000 0000 0000 0000 0200 0000 0400  ................
-00008f90: 0000 4300 0000 7318 0000 007c 006a 006a  ..C...s....|.j.j
-00008fa0: 017c 0174 0264 0119 0064 028d 0201 0064  .|.t.d...d.....d
-00008fb0: 0053 0029 034e 72b4 0000 0072 9b00 0000  .S.).Nr....r....
-00008fc0: 2903 7297 0000 0072 9600 0000 7214 0000  ).r....r....r...
-00008fd0: 0072 aa00 0000 722e 0000 0072 2e00 0000  .r....r....r....
-00008fe0: 722f 0000 0072 a900 0000 ac04 0000 7308  r/...r........s.
-00008ff0: 0000 0000 0106 0102 0106 fe7a 2a4f 5444  ...........z*OTD
-00009000: 796e 616d 6963 4c69 7374 2e5f 7570 6461  ynamicList._upda
-00009010: 7465 5f69 6e76 616c 6964 5f73 7461 7475  te_invalid_statu
-00009020: 735f 6c61 6265 6c63 0100 0000 0000 0000  s_labelc........
-00009030: 0000 0000 0300 0000 0400 0000 4300 0000  ............C...
-00009040: 733c 0000 007c 00a0 00a1 007d 017c 0164  s<...|.....}.|.d
-00009050: 016b 0272 227c 006a 016a 0264 0264 0264  .k.r"|.j.j.d.d.d
-00009060: 038d 0201 006e 1664 047c 019b 0064 059d  .....n.d.|...d..
-00009070: 037d 027c 00a0 037c 02a1 0101 0064 0053  .}.|...|.....d.S
-00009080: 0029 064e 7201 0000 0072 5400 0000 729b  .).Nr....rT...r.
-00009090: 0000 007a 0943 6f6e 7461 696e 7320 7a11  ...z.Contains z.
-000090a0: 2069 6e76 616c 6964 2069 6e70 7574 2873   invalid input(s
-000090b0: 2929 04da 155f 6765 745f 6e75 6d62 6572  ))..._get_number
-000090c0: 5f6f 665f 6572 726f 7273 7297 0000 0072  _of_errorsr....r
-000090d0: 9600 0000 72a9 0000 0029 0372 2900 0000  ....r....).r)...
-000090e0: 5a05 6e5f 6572 7272 ab00 0000 722e 0000  Z.n_errr....r...
-000090f0: 0072 2e00 0000 722f 0000 0072 7901 0000  .r....r/...ry...
-00009100: b104 0000 730a 0000 0000 0108 0108 0112  ....s...........
-00009110: 020c 017a 224f 5444 796e 616d 6963 4c69  ...z"OTDynamicLi
-00009120: 7374 2e5f 7570 6461 7465 5f73 7461 7475  st._update_statu
-00009130: 735f 6c61 6265 6c63 0100 0000 0000 0000  s_labelc........
-00009140: 0000 0000 0100 0000 0200 0000 4300 0000  ............C...
-00009150: 730a 0000 0067 007c 005f 0064 0053 0072  s....g.|._.d.S.r
-00009160: 4c00 0000 a901 728d 0100 0072 4d00 0000  L.....r....rM...
-00009170: 722e 0000 0072 2e00 0000 722f 0000 0072  r....r....r/...r
-00009180: 2500 0000 bb04 0000 7302 0000 0000 017a  %.......s......z
-00009190: 194f 5444 796e 616d 6963 4c69 7374 2e5f  .OTDynamicList._
-000091a0: 6465 6669 6e65 5f76 6172 6301 0000 0000  define_varc.....
-000091b0: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
-000091c0: 0000 0073 2000 0000 7c00 6a00 720a 6401  ...s ...|.j.r.d.
-000091d0: 5300 7c00 6a01 7318 7c00 a002 a100 731c  S.|.j.s.|.....s.
-000091e0: 6402 5300 6403 5300 2904 7a10 5265 7475  d.S.d.S.).z.Retu
-000091f0: 726e 2073 7461 7475 7320 4944 72b5 0000  rn status IDr...
-00009200: 0072 0100 0000 7234 0000 0029 0372 7c01  .r....r4...).r|.
-00009210: 0000 727d 0100 00da 155f 6368 6563 6b5f  ..r}....._check_
-00009220: 7072 6576 696f 7573 5f76 616c 7565 724d  previous_valuerM
-00009230: 0000 0072 2e00 0000 722e 0000 0072 2f00  ...r....r....r/.
-00009240: 0000 da0b 5f67 6574 5f73 7461 7475 73be  ...._get_status.
-00009250: 0400 0073 0a00 0000 0002 0601 0402 0e01  ...s............
-00009260: 0402 7a19 4f54 4479 6e61 6d69 634c 6973  ..z.OTDynamicLis
-00009270: 742e 5f67 6574 5f73 7461 7475 7363 0100  t._get_statusc..
-00009280: 0000 0000 0000 0000 0000 0400 0000 0300  ................
-00009290: 0000 4300 0000 7346 0000 007c 00a0 00a1  ..C...sF...|....
-000092a0: 007d 0174 017c 006a 0283 0174 017c 0183  .}.t.|.j...t.|..
-000092b0: 016b 0372 1e64 0153 0074 037c 006a 027c  .k.r.d.S.t.|.j.|
-000092c0: 0183 0244 005d 165c 027d 027d 037c 027c  ...D.].\.}.}.|.|
-000092d0: 036b 0372 2a01 0064 0153 0071 2a64 0253  .k.r*..d.S.q*d.S
-000092e0: 0029 037a 3420 5472 7565 2069 6620 636f  .).z4 True if co
-000092f0: 6e74 656e 7420 6f66 206d 656d 6f72 7920  ntent of memory 
-00009300: 6571 7561 6c73 2074 6f20 7072 6576 696f  equals to previo
-00009310: 7573 2076 616c 7565 7346 5429 0472 2100  us valuesFT).r!.
-00009320: 0000 72ca 0000 0072 4f00 0000 72b3 0000  ..r....rO...r...
-00009330: 0029 0472 2900 0000 72df 0000 0072 de00  .).r)...r....r..
-00009340: 0000 5a07 636d 705f 7661 6c72 2e00 0000  ..Z.cmp_valr....
-00009350: 722e 0000 0072 2f00 0000 729e 0100 00c8  r....r/...r.....
-00009360: 0400 0073 0e00 0000 0002 0802 1201 0402  ...s............
-00009370: 1401 0801 0802 7a23 4f54 4479 6e61 6d69  ......z#OTDynami
-00009380: 634c 6973 742e 5f63 6865 636b 5f70 7265  cList._check_pre
-00009390: 7669 6f75 735f 7661 6c75 6563 0100 0000  vious_valuec....
-000093a0: 0000 0000 0000 0000 0100 0000 0200 0000  ................
-000093b0: 4300 0000 7322 0000 007c 006a 0064 0175  C...s"...|.j.d.u
-000093c0: 0072 0e64 0153 007c 006a 00a0 01a1 0001  .r.d.S.|.j......
-000093d0: 0064 017c 005f 0064 0153 0029 027a 1352  .d.|._.d.S.).z.R
-000093e0: 656d 6f76 6520 656d 7074 7920 7769 6467  emove empty widg
-000093f0: 6574 4e29 0272 7e01 0000 7261 0000 0072  etN).r~...ra...r
-00009400: 4d00 0000 722e 0000 0072 2e00 0000 722f  M...r....r....r/
-00009410: 0000 00da 1263 6c65 6172 5f65 6d70 7479  .....clear_empty
-00009420: 5f77 6964 6765 74d6 0400 0073 0800 0000  _widget....s....
-00009430: 0002 0a01 0402 0a01 7a20 4f54 4479 6e61  ........z OTDyna
-00009440: 6d69 634c 6973 742e 636c 6561 725f 656d  micList.clear_em
-00009450: 7074 795f 7769 6467 6574 6302 0000 0000  pty_widgetc.....
-00009460: 0000 0000 0000 0002 0000 0008 0000 0043  ...............C
-00009470: 0000 0073 2600 0000 7a0c 7c00 6a00 7c01  ...s&...z.|.j.|.
-00009480: 1900 5700 5300 0400 7401 7920 0100 0100  ..W.S...t.y ....
-00009490: 0100 5900 6401 5300 3000 6401 5300 2902  ..Y.d.S.0.d.S.).
-000094a0: 7a27 5265 7475 726e 2070 7265 7669 6f75  z'Return previou
-000094b0: 7320 7661 6c75 6520 6f66 206f 6e65 206c  s value of one l
-000094c0: 6973 7420 656e 7472 794e 2902 724f 0000  ist entryN).rO..
-000094d0: 00da 0a49 6e64 6578 4572 726f 7229 0272  ...IndexError).r
-000094e0: 2900 0000 da05 696e 6465 7872 2e00 0000  ).....indexr....
-000094f0: 722e 0000 0072 2f00 0000 da18 5f67 6574  r....r/....._get
-00009500: 5f70 7265 7669 6f75 735f 6974 656d 5f76  _previous_item_v
-00009510: 616c 7565 de04 0000 7308 0000 0000 0202  alue....s.......
-00009520: 010c 010c 017a 264f 5444 796e 616d 6963  .....z&OTDynamic
-00009530: 4c69 7374 2e5f 6765 745f 7072 6576 696f  List._get_previo
-00009540: 7573 5f69 7465 6d5f 7661 6c75 654e 6302  us_item_valueNc.
-00009550: 0000 0000 0000 0000 0000 0004 0000 0005  ................
-00009560: 0000 0043 0000 0073 4c00 0000 7c00 a000  ...C...sL...|...
-00009570: 7401 7c00 6a02 8301 a101 7d02 7403 7c00  t.|.j.....}.t.|.
-00009580: 6a04 6401 1900 7c00 7c00 6a05 7c02 8304  j.d...|.|.j.|...
-00009590: 7d03 7c01 6402 7501 7238 7c03 a006 7c01  }.|.d.u.r8|...|.
-000095a0: a101 0100 7c00 a007 a100 0100 7c00 a008  ....|.......|...
-000095b0: a100 0100 6402 5300 2903 7a16 4164 6420  ....d.S.).z.Add 
-000095c0: 616e 2069 7465 6d20 696e 7465 726e 616c  an item internal
-000095d0: 6c79 72dd 0000 004e 2909 72a3 0100 0072  lyr....N).r....r
-000095e0: ca00 0000 728d 0100 0072 7201 0000 7220  ....r....rr...r 
-000095f0: 0000 0072 5401 0000 7251 0000 0072 a001  ...rT...rQ...r..
-00009600: 0000 7271 0100 0029 0472 2900 0000 7272  ..rq...).r)...rr
-00009610: 0000 0072 4f00 0000 5a09 6e65 775f 656e  ...rO...Z.new_en
-00009620: 7472 7972 2e00 0000 722e 0000 0072 2f00  tryr....r....r/.
-00009630: 0000 729a 0100 00e5 0400 0073 1000 0000  ..r........s....
-00009640: 0004 1001 1001 02ff 0402 0801 0a02 0801  ................
-00009650: 7a17 4f54 4479 6e61 6d69 634c 6973 742e  z.OTDynamicList.
-00009660: 5f61 6464 5f69 7465 6d63 0200 0000 0000  _add_itemc......
-00009670: 0000 0000 0000 0400 0000 0200 0000 4300  ..............C.
-00009680: 0000 7366 0000 007c 006a 0073 0a64 0153  ..sf...|.j.s.d.S
-00009690: 007c 0164 0175 0072 1c74 017c 006a 0083  .|.d.u.r.t.|.j..
-000096a0: 017d 0164 027d 027c 027c 016b 0072 447c  .}.d.}.|.|.k.rD|
-000096b0: 006a 00a0 02a1 007d 037c 03a0 03a1 0001  .j.....}.|......
-000096c0: 007c 0264 0337 007d 0271 207c 00a0 04a1  .|.d.7.}.q |....
-000096d0: 0001 0074 017c 006a 0083 0164 026b 0272  ...t.|.j...d.k.r
-000096e0: 627c 00a0 05a1 0001 0064 0153 0029 047a  b|.......d.S.).z
-000096f0: 4344 656c 6574 6520 736f 6d65 2069 7465  CDelete some ite
-00009700: 6d73 0a20 2020 2020 2020 200a 2020 2020  ms.        .    
-00009710: 2020 2020 6465 6c20 616c 6c20 6974 656d      del all item
-00009720: 7320 6966 206e 5f69 7465 6d73 2069 7320  s if n_items is 
-00009730: 4e6f 6e65 4e72 0100 0000 7234 0000 0029  NoneNr....r4...)
-00009740: 0672 8d01 0000 72ca 0000 00da 0370 6f70  .r....r......pop
-00009750: 7261 0000 0072 7101 0000 728e 0100 0029  ra...rq...r....)
-00009760: 0472 2900 0000 5a07 6e5f 6974 656d 73da  .r)...Z.n_items.
-00009770: 0169 7299 0100 0072 2e00 0000 722e 0000  .ir....r....r...
-00009780: 0072 2f00 0000 729b 0100 00f2 0400 0073  .r/...r........s
-00009790: 1800 0000 0005 0601 0402 0801 0a02 0401  ................
-000097a0: 0801 0a01 0801 0a02 0802 0e01 7a1a 4f54  ............z.OT
-000097b0: 4479 6e61 6d69 634c 6973 742e 7265 6d6f  DynamicList.remo
-000097c0: 7665 5f69 7465 6d73 6301 0000 0000 0000  ve_itemsc.......
-000097d0: 0000 0000 0001 0000 0001 0000 0043 0000  .............C..
-000097e0: 0073 0600 0000 7c00 6a00 5300 2901 7a21  .s....|.j.S.).z!
-000097f0: 4865 6d2c 2072 656d 6f76 655f 6974 656d  Hem, remove_item
-00009800: 7320 6973 206e 6220 6f66 2065 7272 6f72  s is nb of error
-00009810: 7329 0172 7c01 0000 724d 0000 0072 2e00  s).r|...rM...r..
-00009820: 0000 722e 0000 0072 2f00 0000 729c 0100  ..r....r/...r...
-00009830: 0008 0500 0073 0200 0000 0002 7a23 4f54  .....s......z#OT
-00009840: 4479 6e61 6d69 634c 6973 742e 5f67 6574  DynamicList._get
-00009850: 5f6e 756d 6265 725f 6f66 5f65 7272 6f72  _number_of_error
-00009860: 7363 0100 0000 0000 0000 0000 0000 0100  sc..............
-00009870: 0000 0400 0000 4300 0000 7324 0000 007c  ......C...s$...|
-00009880: 00a0 00a1 0001 007c 006a 0164 016b 0372  .......|.j.d.k.r
-00009890: 207c 00a0 027c 00a0 03a1 00a1 0101 0064   |...|.........d
-000098a0: 0253 00a9 037a 5243 616c 6c62 6163 6b20  .S...zRCallback 
-000098b0: 6966 2073 7461 7475 7320 6973 2075 7064  if status is upd
-000098c0: 6174 6564 0a20 2020 2020 2020 200a 2020  ated.        .  
-000098d0: 2020 2020 2020 5741 524e 494e 473a 2074        WARNING: t
-000098e0: 7269 6767 6572 2064 6570 7065 6e64 656e  rigger deppenden
-000098f0: 6379 2073 6574 7465 7272 b500 0000 4e29  cy setterr....N)
-00009900: 0472 7901 0000 7257 0000 0072 a500 0000  .ry...rW...r....
-00009910: 7221 0000 0072 4d00 0000 722e 0000 0072  r!...rM...r....r
-00009920: 2e00 0000 722f 0000 0072 5f00 0000 0c05  ....r/...r_.....
-00009930: 0000 7306 0000 0000 0408 020a 017a 1e4f  ..s..........z.O
-00009940: 5444 796e 616d 6963 4c69 7374 2e6f 6e5f  TDynamicList.on_
-00009950: 7570 6461 7465 5f73 7461 7475 7363 0200  update_statusc..
-00009960: 0000 0000 0000 0000 0000 0200 0000 0300  ................
-00009970: 0000 4300 0000 7310 0000 007c 006a 00a0  ..C...s....|.j..
-00009980: 017c 01a1 0101 0064 0153 0029 027a 114e  .|.....d.S.).z.N
-00009990: 6577 2063 6869 6c64 2074 6f20 6c69 7374  ew child to list
-000099a0: 4e29 0272 8d01 0000 72ec 0000 0029 0272  N).r....r....).r
-000099b0: 2900 0000 da05 6368 696c 6472 2e00 0000  ).....childr....
-000099c0: 722e 0000 0072 2f00 0000 da09 6164 645f  r....r/.....add_
-000099d0: 6368 696c 6415 0500 0073 0200 0000 0002  child....s......
-000099e0: 7a17 4f54 4479 6e61 6d69 634c 6973 742e  z.OTDynamicList.
-000099f0: 6164 645f 6368 696c 6463 0200 0000 0000  add_childc......
-00009a00: 0000 0000 0000 0900 0000 0500 0000 4300  ..............C.
-00009a10: 0000 73b8 0000 0074 007c 0183 017d 027c  ..s....t.|...}.|
-00009a20: 027c 006a 016b 0072 3274 027c 006a 017c  .|.j.k.r2t.|.j.|
-00009a30: 0218 0083 0144 005d 0e7d 037c 01a0 0364  .....D.].}.|...d
-00009a40: 01a1 0101 0071 206e 187c 027c 006a 046b  .....q n.|.|.j.k
-00009a50: 0472 4a7c 0164 017c 006a 0485 0219 007d  .rJ|.d.|.j.....}
-00009a60: 0174 007c 0183 017d 0274 007c 006a 0583  .t.|...}.t.|.j..
-00009a70: 017d 047c 047c 026b 0472 767c 047c 0218  .}.|.|.k.rv|.|..
-00009a80: 007d 057c 00a0 067c 05a1 0101 0074 077c  .}.|...|.....t.|
-00009a90: 006a 057c 0183 0244 005d 125c 027d 067d  .j.|...D.].\.}.}
-00009aa0: 077c 06a0 087c 07a1 0101 0071 8274 027c  .|...|.....q.t.|
-00009ab0: 047c 0283 0244 005d 127d 087c 00a0 097c  .|...D.].}.|...|
-00009ac0: 017c 0819 00a1 0101 0071 a064 0153 0029  .|.......q.d.S.)
-00009ad0: 027a 124f 7065 6e74 6561 2053 4554 206d  .z.Opentea SET m
-00009ae0: 6574 686f 644e 290a 72ca 0000 0072 7f01  ethodN).r....r..
-00009af0: 0000 da05 7261 6e67 6572 ec00 0000 7280  ....ranger....r.
-00009b00: 0100 0072 8d01 0000 729b 0100 0072 b300  ...r....r....r..
-00009b10: 0000 7251 0000 0072 9a01 0000 2909 7229  ..rQ...r....).r)
-00009b20: 0000 0072 df00 0000 5a0b 6e5f 7365 745f  ...r....Z.n_set_
-00009b30: 656c 656d 73da 015f 5a06 6e5f 7661 7273  elems.._Z.n_vars
-00009b40: 5a05 6e5f 6465 6c72 be00 0000 7272 0000  Z.n_delr....rr..
-00009b50: 0072 a501 0000 722e 0000 0072 2e00 0000  .r....r....r....
-00009b60: 722f 0000 0072 5100 0000 1a05 0000 731e  r/...rQ.......s.
-00009b70: 0000 0000 0208 010a 0112 010e 020a 010e  ................
-00009b80: 0208 010a 0808 0108 010a 0314 010c 030e  ................
-00009b90: 017a 114f 5444 796e 616d 6963 4c69 7374  .z.OTDynamicList
-00009ba0: 2e73 6574 6301 0000 0000 0000 0000 0000  .setc...........
-00009bb0: 0001 0000 0002 0000 0043 0000 0073 1000  .........C...s..
-00009bc0: 0000 6401 6402 8400 7c00 6a00 4400 8301  ..d.d...|.j.D...
-00009bd0: 5300 2903 fa12 4f70 656e 7465 6120 4745  S.)...Opentea GE
-00009be0: 5420 6d65 7468 6f64 6301 0000 0000 0000  T methodc.......
-00009bf0: 0000 0000 0002 0000 0004 0000 0053 0000  .............S..
-00009c00: 0073 1400 0000 6700 7c00 5d0c 7d01 7c01  .s....g.|.].}.|.
-00009c10: a000 a100 9102 7104 5300 722e 0000 0029  ......q.S.r....)
-00009c20: 0172 2100 0000 2902 726a 0100 0072 9901  .r!...).rj...r..
-00009c30: 0000 722e 0000 0072 2e00 0000 722f 0000  ..r....r....r/..
-00009c40: 0072 6b01 0000 3c05 0000 726c 0100 007a  .rk...<...rl...z
-00009c50: 254f 5444 796e 616d 6963 4c69 7374 2e67  %OTDynamicList.g
-00009c60: 6574 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  et.<locals>.<lis
-00009c70: 7463 6f6d 703e 729d 0100 0072 4d00 0000  tcomp>r....rM...
-00009c80: 722e 0000 0072 2e00 0000 722f 0000 0072  r....r....r/...r
-00009c90: 2100 0000 3905 0000 7302 0000 0000 037a  !...9...s......z
-00009ca0: 114f 5444 796e 616d 6963 4c69 7374 2e67  .OTDynamicList.g
-00009cb0: 6574 6301 0000 0000 0000 0000 0000 0002  etc.............
-00009cc0: 0000 0003 0000 0043 0000 0073 3600 0000  .......C...s6...
-00009cd0: 7c00 6a00 6401 6b03 720e 6402 5300 7c00  |.j.d.k.r.d.S.|.
-00009ce0: a001 a100 7c00 5f02 7c00 6a03 4400 5d0a  ....|._.|.j.D.].
-00009cf0: 7d01 6403 7c01 5f00 711e 7c00 a004 a100  }.d.|._.q.|.....
-00009d00: 0100 6402 5300 2904 7a17 4f70 656e 7465  ..d.S.).z.Opente
-00009d10: 6120 5641 4c49 4441 5445 206d 6574 686f  a VALIDATE metho
-00009d20: 6472 0100 0000 4e72 3400 0000 2905 7257  dr....Nr4...).rW
-00009d30: 0000 0072 2100 0000 724f 0000 0072 8d01  ...r!...rO...r..
-00009d40: 0000 7258 0000 0029 0272 2900 0000 7299  ..rX...).r)...r.
-00009d50: 0100 0072 2e00 0000 722e 0000 0072 2f00  ...r....r....r/.
-00009d60: 0000 7259 0000 003e 0500 0073 0c00 0000  ..rY...>...s....
-00009d70: 0003 0a01 0402 0a02 0a01 0802 7a16 4f54  ............z.OT
-00009d80: 4479 6e61 6d69 634c 6973 742e 7661 6c69  DynamicList.vali
-00009d90: 6461 7465 2901 4e29 014e 2920 7263 0000  date).N).N) rc..
-00009da0: 0072 6400 0000 7265 0000 0072 6600 0000  .rd...re...rf...
-00009db0: 721f 0000 0072 2600 0000 727a 0100 0072  r....r&...rz...r
-00009dc0: 8201 0000 7289 0000 0072 8101 0000 725e  ....r....r....r^
-00009dd0: 0100 0072 7101 0000 728e 0100 0072 8c01  ...rq...r....r..
-00009de0: 0000 7285 0100 0072 8601 0000 72a9 0000  ..r....r....r...
-00009df0: 0072 7901 0000 7225 0000 0072 9f01 0000  .ry...r%...r....
-00009e00: 729e 0100 0072 a001 0000 72a3 0100 0072  r....r....r....r
-00009e10: 9a01 0000 729b 0100 0072 9c01 0000 725f  ....r....r....r_
-00009e20: 0000 0072 a801 0000 7251 0000 0072 2100  ...r....rQ...r!.
-00009e30: 0000 7259 0000 0072 6700 0000 722e 0000  ..rY...rg...r...
-00009e40: 0072 2e00 0000 722c 0000 0072 2f00 0000  .r....r,...r/...
-00009e50: 727b 0100 0028 0400 0073 3800 0000 0801  r{...(...s8.....
-00009e60: 0402 0c19 0c06 0201 0a04 0807 0813 0805  ................
-00009e70: 0c07 080a 081c 0809 0808 0805 080a 0803  ................
-00009e80: 080a 080e 0808 0807 0a0d 0a16 0804 0809  ................
-00009e90: 0805 081f 0805 727b 0100 0063 0000 0000  ......r{...c....
-00009ea0: 0000 0000 0000 0000 0000 0000 0300 0000  ................
-00009eb0: 0000 0000 7392 0000 0065 005a 0164 005a  ....s....e.Z.d.Z
-00009ec0: 0264 015a 0364 0264 0384 005a 0464 0464  .d.Z.d.d...Z.d.d
-00009ed0: 0584 005a 0564 0664 0784 005a 0664 0864  ...Z.d.d...Z.d.d
-00009ee0: 0984 005a 0764 0a64 0b84 005a 0887 0066  ...Z.d.d...Z...f
-00009ef0: 0164 0c64 0d84 085a 0965 0a64 0e64 0f84  .d.d...Z.e.d.d..
-00009f00: 0083 015a 0b65 0b6a 0c64 1064 0f84 0083  ...Z.e.j.d.d....
-00009f10: 015a 0b64 1164 1284 005a 0d64 1364 1484  .Z.d.d...Z.d.d..
-00009f20: 005a 0e64 1564 1684 005a 0f64 1764 1884  .Z.d.d...Z.d.d..
-00009f30: 005a 1064 1964 1a84 005a 1164 1b64 1c84  .Z.d.d...Z.d.d..
-00009f40: 005a 1287 0004 005a 1353 0029 1dda 0c4f  .Z.....Z.S.)...O
-00009f50: 5453 7461 7469 634c 6973 747a 4b4c 6973  TStaticListzKLis
-00009f60: 7420 4e4f 5420 636f 6e74 726f 6c6c 6564  t NOT controlled
-00009f70: 2062 6279 2074 6865 2075 7365 720a 2020   bby the user.  
-00009f80: 2020 0a20 2020 2063 7265 6174 6564 2069    .    created i
-00009f90: 6620 6f74 5f72 6571 7569 7265 206f 7220  f ot_require or 
-00009fa0: 6469 7361 626c 6564 6301 0000 0000 0000  disabledc.......
-00009fb0: 0000 0000 0003 0000 0006 0000 0043 0000  .............C..
-00009fc0: 0073 a600 0000 6401 7d01 7c00 a000 7c01  .s....d.}.|...|.
-00009fd0: a101 0100 7401 6a02 7c00 6a03 6402 6403  ....t.j.|.j.d.d.
-00009fe0: 8d02 7d02 7404 7c00 6a03 7c01 7c02 6a05  ..}.t.|.j.|.|.j.
-00009ff0: 6404 8d03 7c00 5f06 7c00 6a06 6a07 6405  d...|._.|.j.j.d.
-0000a000: 7408 6406 1900 7408 6406 1900 7408 6407  t.d...t.d...t.d.
-0000a010: 1900 6408 8d04 0100 7c02 6a09 7c00 6a06  ..d.....|.j.|.j.
-0000a020: 6a0a 6409 8d01 0100 7c02 6a0b 640a 640b  j.d.....|.j.d.d.
-0000a030: 640c 8d02 0100 7c00 6a06 6a0b 640d 640e  d.....|.j.j.d.d.
-0000a040: 640f 6410 8d03 0100 7c00 6a06 a00c 6411  d.d.....|.j...d.
-0000a050: 7c00 6a0d a102 0100 7c00 6a06 a00c 6412  |.j.....|.j...d.
-0000a060: 7c00 6a0e a102 0100 6413 5300 2914 7a10  |.j.....d.S.).z.
-0000a070: 5061 636b 696e 6720 656c 656d 656e 7473  Packing elements
-0000a080: 723c 0100 00da 0876 6572 7469 6361 6c29  r<.....vertical)
-0000a090: 0172 f300 0000 2902 7231 0000 0072 2001  .r....).r1...r .
-0000a0a0: 0000 727c 0000 0072 8000 0000 7281 0000  ..r|...r....r...
-0000a0b0: 0029 0472 1c00 0000 7282 0000 0072 7900  .).r....r....ry.
-0000a0c0: 0000 7283 0000 0072 2601 0000 72ef 0000  ..r....r&...r...
-0000a0d0: 0072 1d01 0000 7239 0000 0072 3500 0000  .r....r9...r5...
-0000a0e0: 721a 0100 0072 8a00 0000 2903 7237 0000  r....r....).r7..
-0000a0f0: 0072 3a00 0000 724c 0100 0072 3801 0000  .r:...rL...r8...
-0000a100: 7239 0100 004e 290f 7271 0100 0072 0200  r9...N).rq...r..
-0000a110: 0000 72f8 0000 0072 5401 0000 7209 0000  ..r....rT...r...
-0000a120: 0072 5100 0000 da03 6c62 7872 8400 0000  .rQ.....lbxr....
-0000a130: 7211 0000 0072 9600 0000 7231 0100 0072  r....r....r1...r
-0000a140: 4700 0000 7229 0100 0072 3a01 0000 723b  G...r)...r:...r;
-0000a150: 0100 0029 0372 2900 0000 da06 6e6c 696e  ...).r).....nlin
-0000a160: 6573 7232 0100 0072 2e00 0000 722e 0000  esr2...r....r...
-0000a170: 0072 2f00 0000 da12 5f63 6f6e 6669 6775  .r/....._configu
-0000a180: 7265 5f6c 6973 7462 6f78 5305 0000 7326  re_listboxS...s&
-0000a190: 0000 0000 0204 010a 0210 0202 0104 0102  ................
-0000a1a0: 0104 fd08 0406 0102 0106 0106 0106 fc06  ................
-0000a1b0: 0610 010e 0112 0110 017a 1f4f 5453 7461  .........z.OTSta
-0000a1c0: 7469 634c 6973 742e 5f63 6f6e 6669 6775  ticList._configu
-0000a1d0: 7265 5f6c 6973 7462 6f78 6301 0000 0000  re_listboxc.....
-0000a1e0: 0000 0000 0000 0002 0000 0003 0000 0047  ...............G
-0000a1f0: 0000 0073 1000 0000 7c00 6a00 a001 6401  ...s....|.j...d.
-0000a200: a101 0100 6402 5300 2903 7a22 456e 6162  ....d.S.).z"Enab
-0000a210: 6c65 2073 6372 6f6c 6c20 6966 2070 6f69  le scroll if poi
-0000a220: 6e74 6572 2069 6e20 7769 6467 6574 723f  nter in widgetr?
-0000a230: 0100 004e a902 72ae 0100 0072 4101 0000  ...N..r....rA...
-0000a240: 725a 0000 0072 2e00 0000 722e 0000 0072  rZ...r....r....r
-0000a250: 2f00 0000 723b 0100 006a 0500 0073 0200  /...r;...j...s..
-0000a260: 0000 0002 7a20 4f54 5374 6174 6963 4c69  ....z OTStaticLi
-0000a270: 7374 2e5f 6269 6e64 5f67 6c6f 6261 6c5f  st._bind_global_
-0000a280: 7363 726f 6c6c 6301 0000 0000 0000 0000  scrollc.........
-0000a290: 0000 0002 0000 0003 0000 0047 0000 0073  ...........G...s
-0000a2a0: 1000 0000 7c00 6a00 a001 6401 a101 0100  ....|.j...d.....
-0000a2b0: 6402 5300 2903 7a23 4469 7361 626c 6520  d.S.).z#Disable 
-0000a2c0: 7363 726f 6c6c 2069 6620 706f 696e 7465  scroll if pointe
-0000a2d0: 7220 696e 2077 6964 6765 7472 4201 0000  r in widgetrB...
-0000a2e0: 4e72 b101 0000 725a 0000 0072 2e00 0000  Nr....rZ...r....
-0000a2f0: 722e 0000 0072 2f00 0000 723a 0100 006e  r....r/...r:...n
-0000a300: 0500 0073 0200 0000 0002 7a22 4f54 5374  ...s......z"OTSt
-0000a310: 6174 6963 4c69 7374 2e5f 756e 6269 6e64  aticList._unbind
-0000a320: 5f67 6c6f 6261 6c5f 7363 726f 6c6c 6301  _global_scrollc.
-0000a330: 0000 0000 0000 0000 0000 0002 0000 0005  ................
-0000a340: 0000 0043 0000 0073 4800 0000 7c00 6a00  ...C...sH...|.j.
-0000a350: 6a01 6401 6402 8d01 0100 7c00 6a00 a002  j.d.d.....|.j...
-0000a360: 6403 6404 a102 0100 7c00 6a03 4400 5d12  d.d.....|.j.D.].
-0000a370: 7d01 7c00 6a00 a004 6404 7c01 a102 0100  }.|.j...d.|.....
-0000a380: 7122 7c00 6a00 6a01 6405 6402 8d01 0100  q"|.j.j.d.d.....
-0000a390: 6406 5300 2907 7a30 4368 616e 6765 2061  d.S.).z0Change a
-0000a3a0: 7070 6561 7265 6e63 6520 6163 636f 7264  ppearence accord
-0000a3b0: 696e 6720 746f 2069 6e74 6572 6e61 6c20  ing to internal 
-0000a3c0: 7661 7269 6162 6c65 721d 0000 0072 2501  variabler....r%.
-0000a3d0: 0000 7201 0000 0072 2401 0000 727c 0000  ..r....r$...r|..
-0000a3e0: 004e 2905 72ae 0100 0072 8400 0000 da06  .N).r....r......
-0000a3f0: 6465 6c65 7465 72be 0000 0072 3001 0000  deleter....r0...
-0000a400: 2902 7229 0000 0072 5001 0000 722e 0000  ).r)...rP...r...
-0000a410: 0072 2e00 0000 722f 0000 00da 0f5f 7570  .r....r/....._up
-0000a420: 6461 7465 5f6c 6973 7462 6f78 7205 0000  date_listboxr...
-0000a430: 730a 0000 0000 020e 020e 010a 0110 027a  s..............z
-0000a440: 1c4f 5453 7461 7469 634c 6973 742e 5f75  .OTStaticList._u
-0000a450: 7064 6174 655f 6c69 7374 626f 7863 0100  pdate_listboxc..
-0000a460: 0000 0000 0000 0000 0000 0100 0000 0200  ................
-0000a470: 0000 4300 0000 730a 0000 0067 007c 005f  ..C...s....g.|._
-0000a480: 0064 0053 0072 4c00 0000 a901 da09 5f76  .d.S.rL......._v
-0000a490: 6172 6961 626c 6572 4d00 0000 722e 0000  ariablerM...r...
-0000a4a0: 0072 2e00 0000 722f 0000 0072 2500 0000  .r....r/...r%...
-0000a4b0: 7d05 0000 7302 0000 0000 017a 184f 5453  }...s......z.OTS
-0000a4c0: 7461 7469 634c 6973 742e 5f64 6566 696e  taticList._defin
-0000a4d0: 655f 7661 7263 0100 0000 0000 0000 0000  e_varc..........
-0000a4e0: 0000 0100 0000 0200 0000 0300 0000 7316  ..............s.
-0000a4f0: 0000 0074 0083 00a0 01a1 0001 007c 00a0  ...t.........|..
-0000a500: 02a1 0001 0064 0153 0029 027a 1641 6464  .....d.S.).z.Add
-0000a510: 2074 6f20 5f63 7265 6174 655f 7769 6467   to _create_widg
-0000a520: 6574 734e 2903 721e 0000 0072 2600 0000  etsN).r....r&...
-0000a530: 72b0 0100 0072 4d00 0000 722c 0000 0072  r....rM...r,...r
-0000a540: 2e00 0000 722f 0000 0072 2600 0000 8005  ....r/...r&.....
-0000a550: 0000 7304 0000 0000 020a 017a 1c4f 5453  ..s........z.OTS
-0000a560: 7461 7469 634c 6973 742e 5f63 7265 6174  taticList._creat
-0000a570: 655f 7769 6467 6574 7363 0100 0000 0000  e_widgetsc......
-0000a580: 0000 0000 0000 0100 0000 0100 0000 4300  ..............C.
-0000a590: 0000 7306 0000 007c 006a 0053 0072 4c00  ..s....|.j.S.rL.
-0000a5a0: 0000 72b4 0100 0072 4d00 0000 722e 0000  ..r....rM...r...
-0000a5b0: 0072 2e00 0000 722f 0000 0072 be00 0000  .r....r/...r....
-0000a5c0: 8505 0000 7302 0000 0000 027a 154f 5453  ....s......z.OTS
-0000a5d0: 7461 7469 634c 6973 742e 7661 7269 6162  taticList.variab
-0000a5e0: 6c65 6302 0000 0000 0000 0000 0000 0002  lec.............
-0000a5f0: 0000 0004 0000 0043 0000 0073 2c00 0000  .......C...s,...
-0000a600: 7400 7c00 a001 7c01 a101 8301 7c00 5f02  t.|...|.....|._.
-0000a610: 7c01 7c00 5f03 7c00 a004 a100 0100 7c00  |.|._.|.......|.
-0000a620: a005 7c01 a101 0100 6401 5300 2902 7a31  ..|.....d.S.).z1
-0000a630: 4164 6420 6164 6469 7469 6f6e 616c 2062  Add additional b
-0000a640: 6568 6176 696f 7220 746f 2074 6865 2073  ehavior to the s
-0000a650: 6574 7465 7220 6f66 2076 6172 6961 626c  etter of variabl
-0000a660: 654e 2906 7249 0000 00da 115f 636f 6d70  eN).rI....._comp
-0000a670: 6172 655f 7072 6576 696f 7573 7257 0000  are_previousrW..
-0000a680: 0072 b501 0000 72b3 0100 0072 a500 0000  .r....r....r....
-0000a690: 2902 7229 0000 0072 df00 0000 722e 0000  ).r)...r....r...
-0000a6a0: 0072 2e00 0000 722f 0000 0072 be00 0000  .r....r/...r....
-0000a6b0: 8905 0000 7308 0000 0000 0310 0206 0108  ....s...........
-0000a6c0: 0163 0200 0000 0000 0000 0000 0000 0400  .c..............
-0000a6d0: 0000 0300 0000 4300 0000 733e 0000 0074  ......C...s>...t
-0000a6e0: 007c 0183 0174 007c 006a 0183 016b 0372  .|...t.|.j...k.r
-0000a6f0: 1664 0153 0074 027c 006a 017c 0183 0244  .d.S.t.|.j.|...D
-0000a700: 005d 165c 027d 027d 037c 027c 036b 0372  .].\.}.}.|.|.k.r
-0000a710: 2201 0064 0153 0071 2264 0253 0029 037a  "..d.S.q"d.S.).z
-0000a720: 2b54 7275 6520 6966 2076 616c 7565 7320  +True if values 
-0000a730: 6964 656e 7469 6361 6c20 746f 2070 7265  identical to pre
-0000a740: 7669 6f75 7320 7661 6c75 6573 4654 2903  vious valuesFT).
-0000a750: 72ca 0000 0072 4f00 0000 72b3 0000 0029  r....rO...r....)
-0000a760: 0472 2900 0000 72df 0000 0072 de00 0000  .r)...r....r....
-0000a770: da07 6e65 775f 7661 6c72 2e00 0000 722e  ..new_valr....r.
-0000a780: 0000 0072 2f00 0000 72b6 0100 0092 0500  ...r/...r.......
-0000a790: 0073 0c00 0000 0002 1201 0401 1401 0801  .s..............
-0000a7a0: 0801 7a1e 4f54 5374 6174 6963 4c69 7374  ..z.OTStaticList
-0000a7b0: 2e5f 636f 6d70 6172 655f 7072 6576 696f  ._compare_previo
-0000a7c0: 7573 6301 0000 0000 0000 0000 0000 0001  usc.............
-0000a7d0: 0000 0004 0000 0043 0000 0073 1600 0000  .......C...s....
-0000a7e0: 7c00 6a00 6a01 6401 7c00 6a02 6402 8d02  |.j.j.d.|.j.d...
-0000a7f0: 0100 6403 5300 2904 7287 0100 0072 8801  ..d.S.).r....r..
-0000a800: 0000 7289 0100 004e 2903 725d 0100 0072  ..r....N).r]...r
-0000a810: 8b01 0000 726f 0100 0072 4d00 0000 722e  ....ro...rM...r.
-0000a820: 0000 0072 2e00 0000 722f 0000 0072 5e01  ...r....r/...r^.
-0000a830: 0000 9c05 0000 7302 0000 0000 027a 204f  ......s......z O
-0000a840: 5453 7461 7469 634c 6973 742e 5f61 6464  TStaticList._add
-0000a850: 5f70 6f70 7570 5f63 6f6d 6d61 6e64 7363  _popup_commandsc
-0000a860: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-0000a870: 0400 0000 4300 0000 731c 0000 007c 006a  ....C...s....|.j
-0000a880: 0064 016b 0372 187c 00a0 017c 00a0 02a1  .d.k.r.|...|....
-0000a890: 00a1 0101 0064 0253 0072 a601 0000 2903  .....d.S.r....).
-0000a8a0: 7257 0000 0072 a500 0000 7221 0000 0072  rW...r....r!...r
-0000a8b0: 4d00 0000 722e 0000 0072 2e00 0000 722f  M...r....r....r/
-0000a8c0: 0000 0072 5f00 0000 a105 0000 7304 0000  ...r_.......s...
-0000a8d0: 0000 050a 017a 1d4f 5453 7461 7469 634c  .....z.OTStaticL
-0000a8e0: 6973 742e 6f6e 5f75 7064 6174 655f 7374  ist.on_update_st
-0000a8f0: 6174 7573 6301 0000 0000 0000 0000 0000  atusc...........
-0000a900: 0001 0000 0001 0000 0043 0000 0073 0600  .........C...s..
-0000a910: 0000 7c00 6a00 5300 2901 72ab 0100 0029  ..|.j.S.).r....)
-0000a920: 0172 be00 0000 724d 0000 0072 2e00 0000  .r....rM...r....
-0000a930: 722e 0000 0072 2f00 0000 7221 0000 00aa  r....r/...r!....
-0000a940: 0500 0073 0200 0000 0002 7a10 4f54 5374  ...s......z.OTSt
-0000a950: 6174 6963 4c69 7374 2e67 6574 6302 0000  aticList.getc...
-0000a960: 0000 0000 0000 0000 0002 0000 0002 0000  ................
-0000a970: 0043 0000 0073 0e00 0000 7400 7c01 8301  .C...s....t.|...
-0000a980: 7c00 5f01 6401 5300 2902 7a54 4f70 656e  |._.d.S.).zTOpen
-0000a990: 7465 6120 5345 5420 6d65 7468 6f64 0a20  tea SET method. 
-0000a9a0: 2020 2020 2020 2042 7920 6173 7369 676e         By assign
-0000a9b0: 696e 6720 7765 2074 7269 6767 6572 2074  ing we trigger t
-0000a9c0: 6865 2076 6172 6961 626c 6520 5f5f 7365  he variable __se
-0000a9d0: 7474 6572 5f5f 200a 2020 2020 2020 2020  tter__ .        
-0000a9e0: 4e29 02da 046c 6973 7472 be00 0000 7271  N)...listr....rq
-0000a9f0: 0000 0072 2e00 0000 722e 0000 0072 2f00  ...r....r....r/.
-0000aa00: 0000 7251 0000 00ae 0500 0073 0200 0000  ..rQ.......s....
-0000aa10: 0004 7a10 4f54 5374 6174 6963 4c69 7374  ..z.OTStaticList
-0000aa20: 2e73 6574 6301 0000 0000 0000 0000 0000  .setc...........
-0000aa30: 0001 0000 0002 0000 0043 0000 0073 2a00  .........C...s*.
-0000aa40: 0000 7c00 6a00 6401 6b03 720e 6400 5300  ..|.j.d.k.r.d.S.
-0000aa50: 7c00 a001 a100 7c00 5f02 6402 7c00 5f00  |.....|._.d.|._.
-0000aa60: 7c00 a003 a100 0100 6400 5300 7256 0000  |.......d.S.rV..
-0000aa70: 0029 0472 5700 0000 7221 0000 0072 4f00  .).rW...r!...rO.
-0000aa80: 0000 7258 0000 0072 4d00 0000 722e 0000  ..rX...rM...r...
-0000aa90: 0072 2e00 0000 722f 0000 0072 5900 0000  .r....r/...rY...
-0000aaa0: b405 0000 730a 0000 0000 010a 0104 020a  ....s...........
-0000aab0: 0106 017a 154f 5453 7461 7469 634c 6973  ...z.OTStaticLis
-0000aac0: 742e 7661 6c69 6461 7465 2914 7263 0000  t.validate).rc..
-0000aad0: 0072 6400 0000 7265 0000 0072 6600 0000  .rd...re...rf...
-0000aae0: 72b0 0100 0072 3b01 0000 723a 0100 0072  r....r;...r:...r
-0000aaf0: b301 0000 7225 0000 0072 2600 0000 727a  ....r%...r&...rz
-0000ab00: 0100 0072 be00 0000 da06 7365 7474 6572  ...r......setter
-0000ab10: 72b6 0100 0072 5e01 0000 725f 0000 0072  r....r^...r_...r
-0000ab20: 2100 0000 7251 0000 0072 5900 0000 7267  !...rQ...rY...rg
-0000ab30: 0000 0072 2e00 0000 722e 0000 0072 2c00  ...r....r....r,.
-0000ab40: 0000 722f 0000 0072 ac01 0000 4d05 0000  ..r/...r....M...
-0000ab50: 7322 0000 0008 0104 0508 1708 0408 0408  s"..............
-0000ab60: 0b08 030c 0502 010a 0304 010a 0808 0a08  ................
-0000ab70: 0508 0908 0408 0672 ac01 0000 293a 7266  .......r....):rf
-0000ab80: 0000 0072 0701 0000 72b0 0000 0072 b600  ...r....r....r..
-0000ab90: 0000 7294 0100 0072 0200 0000 7203 0000  ..r....r....r...
-0000aba0: 0072 0400 0000 7205 0000 0072 0600 0000  .r....r....r....
-0000abb0: 7207 0000 0072 0800 0000 7209 0000 0072  r....r....r....r
-0000abc0: 0a00 0000 720b 0000 0072 0c00 0000 da03  ....r....r......
-0000abd0: 6e6f 6272 0d00 0000 da17 6f70 656e 7465  nobr......opente
-0000abe0: 612e 6775 695f 666f 726d 732e 5f62 6173  a.gui_forms._bas
-0000abf0: 6572 0e00 0000 da1d 6f70 656e 7465 612e  er......opentea.
-0000ac00: 6775 695f 666f 726d 732e 5f65 7863 6570  gui_forms._excep
-0000ac10: 7469 6f6e 7372 0f00 0000 7210 0000 00da  tionsr....r.....
-0000ac20: 1b6f 7065 6e74 6561 2e67 7569 5f66 6f72  .opentea.gui_for
-0000ac30: 6d73 2e63 6f6e 7374 616e 7473 7211 0000  ms.constantsr...
-0000ac40: 0072 1200 0000 7213 0000 0072 1400 0000  .r....r....r....
-0000ac50: da21 6f70 656e 7465 612e 6775 695f 666f  .!opentea.gui_fo
-0000ac60: 726d 732e 6765 6e65 7269 635f 7769 6467  rms.generic_widg
-0000ac70: 6574 7372 1500 0000 da17 6f70 656e 7465  etsr......opente
-0000ac80: 612e 6775 695f 666f 726d 732e 7574 696c  a.gui_forms.util
-0000ac90: 7372 1600 0000 7217 0000 00da 1c6f 7065  sr....r......ope
-0000aca0: 6e74 6561 2e67 7569 5f66 6f72 6d73 2e73  ntea.gui_forms.s
-0000acb0: 6f75 6e64 626f 6172 6472 1800 0000 da07  oundboardr......
-0000acc0: 4142 434d 6574 6172 1900 0000 7269 0000  ABCMetar....ri..
-0000acd0: 0072 7300 0000 7288 0000 0072 b800 0000  .rs...r....r....
-0000ace0: 72ba 0000 0072 bb00 0000 72bc 0000 0072  r....r....r....r
-0000acf0: c400 0000 72c7 0000 0072 cc00 0000 72cb  ....r....r....r.
-0000ad00: 0000 0072 e700 0000 72cd 0000 0072 1001  ...r....r....r..
-0000ad10: 0000 7235 0100 0072 3701 0000 7245 0100  ..r5...r7...rE..
-0000ad20: 0072 5201 0000 7272 0100 0072 7b01 0000  .rR...rr...r{...
-0000ad30: 72ac 0100 0072 2e00 0000 722e 0000 0072  r....r....r....r
-0000ad40: 2e00 0000 722f 0000 00da 083c 6d6f 6475  ....r/.....<modu
-0000ad50: 6c65 3e01 0000 0073 4a00 0000 0443 0801  le>....sJ....C..
-0000ad60: 0801 0802 0801 340e 0c02 0c01 1004 1807  ......4.........
-0000ad70: 0c01 1004 0c0b 1665 1015 162c 167f 0005  .......e...,....
-0000ad80: 1006 1004 1006 101e 161e 0e0d 1037 1018  .............7..
-0000ad90: 105a 1010 1052 101f 1037 1019 1648 106e  .Z...R...7...H.n
-0000ada0: 107f 007f 0027                           .....'
+00004320: 0000 0000 0002 0000 0003 0000 0043 0000  .............C..
+00004330: 0073 1a00 0000 7c00 6a00 a001 6401 a101  .s....|.j...d...
+00004340: 7d01 7c00 a002 7c01 a101 0100 6400 5300  }.|...|.....d.S.
+00004350: 2902 4e72 cb00 0000 2903 7220 0000 0072  ).Nr....).r ...r
+00004360: 2100 0000 da13 5f70 6163 6b5f 7769 7468  !....._pack_with
+00004370: 5f63 6f6d 626f 626f 7829 0272 2900 0000  _combobox).r)...
+00004380: da07 6f70 7469 6f6e 7372 2e00 0000 722e  ..optionsr....r.
+00004390: 0000 0072 2f00 0000 7226 0000 0033 0200  ...r/...r&...3..
+000043a0: 0073 0400 0000 0001 0c01 7a1e 5f4f 5443  .s........z._OTC
+000043b0: 686f 6963 6543 6f6d 626f 2e5f 6372 6561  hoiceCombo._crea
+000043c0: 7465 5f77 6964 6765 7473 6302 0000 0000  te_widgetsc.....
+000043d0: 0000 0000 0000 0002 0000 0007 0000 0043  ...............C
+000043e0: 0000 0073 3000 0000 7400 6a01 7c00 6a02  ...s0...t.j.|.j.
+000043f0: 7c01 7c00 6a03 6401 7404 6402 8d05 7c00  |.|.j.d.t.d...|.
+00004400: 5f05 7c00 6a05 6a06 6403 6404 6405 6406  _.|.j.j.d.d.d.d.
+00004410: 8d03 0100 6407 5300 2908 7a1e 436f 6d62  ....d.S.).z.Comb
+00004420: 6f62 6f78 2076 6572 7369 6f6e 206f 6620  obox version of 
+00004430: 7468 6520 7769 6467 6574 da08 7265 6164  the widget..read
+00004440: 6f6e 6c79 2904 72e4 0000 0072 7500 0000  only).r....ru...
+00004450: 721c 0000 005a 0b70 6f73 7463 6f6d 6d61  r....Z.postcomma
+00004460: 6e64 723b 0000 0072 3400 0000 727b 0000  ndr;...r4...r{..
+00004470: 0072 4000 0000 4e29 0772 0200 0000 da08  .r@...N).r......
+00004480: 436f 6d62 6f62 6f78 7245 0000 0072 6d00  ComboboxrE...rm.
+00004490: 0000 7218 0000 00da 0563 6f6d 626f 724b  ..r......comborK
+000044a0: 0000 0029 0272 2900 0000 da06 6f70 7469  ...).r).....opti
+000044b0: 6f6e 722e 0000 0072 2e00 0000 722f 0000  onr....r....r/..
+000044c0: 0072 e500 0000 3702 0000 7310 0000 0000  .r....7...s.....
+000044d0: 0304 0104 0102 0104 0102 0102 fb08 067a  ...............z
+000044e0: 225f 4f54 4368 6f69 6365 436f 6d62 6f2e  "_OTChoiceCombo.
+000044f0: 5f70 6163 6b5f 7769 7468 5f63 6f6d 626f  _pack_with_combo
+00004500: 626f 7863 0100 0000 0000 0000 0000 0000  boxc............
+00004510: 0200 0000 0300 0000 4300 0000 7324 0000  ........C...s$..
+00004520: 007c 006a 0064 016b 0272 0e64 026e 0264  .|.j.d.k.r.d.n.d
+00004530: 037d 017c 006a 016a 027c 0164 048d 0101  .}.|.j.j.|.d....
+00004540: 0064 0053 0029 054e 7234 0000 00da 0954  .d.S.).Nr4.....T
+00004550: 436f 6d62 6f62 6f78 7a15 4869 6768 6c69  Comboboxz.Highli
+00004560: 6768 7465 642e 5443 6f6d 626f 626f 7872  ghted.TComboboxr
+00004570: c700 0000 2903 7257 0000 0072 e900 0000  ....).rW...r....
+00004580: 7284 0000 0072 c800 0000 722e 0000 0072  r....r....r....r
+00004590: 2e00 0000 722f 0000 0072 5e00 0000 4202  ....r/...r^...B.
+000045a0: 0000 7304 0000 0000 0112 017a 245f 4f54  ..s........z$_OT
+000045b0: 4368 6f69 6365 436f 6d62 6f2e 5f75 7064  ChoiceCombo._upd
+000045c0: 6174 655f 7769 6467 6574 735f 7374 796c  ate_widgets_styl
+000045d0: 654e 2907 7263 0000 0072 6400 0000 7265  eN).rc...rd...re
+000045e0: 0000 0072 6600 0000 7226 0000 0072 e500  ...rf...r&...r..
+000045f0: 0000 725e 0000 0072 2e00 0000 722e 0000  ..r^...r....r...
+00004600: 0072 2e00 0000 722f 0000 0072 d000 0000  .r....r/...r....
+00004610: 3002 0000 7308 0000 0008 0104 0208 0408  0...s...........
+00004620: 0b72 d000 0000 6300 0000 0000 0000 0000  .r....c.........
+00004630: 0000 0000 0000 0003 0000 0000 0000 0073  ...............s
+00004640: 5600 0000 6500 5a01 6400 5a02 8700 6601  V...e.Z.d.Z...f.
+00004650: 6401 6402 8408 5a03 6403 6404 8400 5a04  d.d...Z.d.d...Z.
+00004660: 6405 6406 8400 5a05 6407 6408 8400 5a06  d.d...Z.d.d...Z.
+00004670: 6412 640a 640b 8401 5a07 640c 640d 8400  d.d.d...Z.d.d...
+00004680: 5a08 640e 640f 8400 5a09 6410 6411 8400  Z.d.d...Z.d.d...
+00004690: 5a0a 8700 0400 5a0b 5300 2913 da0d 4f54  Z.....Z.S.)...OT
+000046a0: 4669 6c65 4272 6f77 7365 7263 0500 0000  FileBrowserc....
+000046b0: 0000 0000 0000 0000 0800 0000 0600 0000  ................
+000046c0: 0300 0000 736c 0000 0074 0083 00a0 017c  ....sl...t.....|
+000046d0: 017c 027c 037c 04a1 0401 0067 007c 005f  .|.|.|.....g.|._
+000046e0: 0264 017c 005f 0364 027c 0176 0072 687c  .d.|._.d.|.v.rh|
+000046f0: 0164 0219 007d 0564 037c 0576 0072 3e64  .d...}.d.|.v.r>d
+00004700: 047c 005f 036e 2a7c 0544 005d 247d 067c  .|._.n*|.D.]$}.|
+00004710: 069b 0064 059d 0264 067c 069b 009d 0266  ...d...d.|.....f
+00004720: 027d 077c 006a 02a0 047c 07a1 0101 0071  .}.|.j...|.....q
+00004730: 4264 0753 0029 08fa a953 7461 7274 7570  Bd.S.)...Startup
+00004740: 2063 6c61 7373 2e0a 0a20 2020 2020 2020   class...       
+00004750: 2049 6e70 7574 7320 3a0a 2020 2020 2020   Inputs :.      
+00004760: 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020    --------.     
+00004770: 2020 2073 6368 656d 6120 3a20 6120 7363     schema : a sc
+00004780: 6865 6d61 2061 7320 6120 6e65 7374 6564  hema as a nested
+00004790: 206f 626a 6563 740a 2020 2020 2020 2020   object.        
+000047a0: 726f 6f74 5f66 7261 6d65 203a 2020 6120  root_frame :  a 
+000047b0: 546b 206f 626a 6563 7420 7765 7265 2074  Tk object were t
+000047c0: 6865 2077 6964 6765 7420 7769 6c6c 2062  he widget will b
+000047d0: 6520 6772 6166 7465 640a 2020 2020 2020  e grafted.      
+000047e0: 2020 465a 096f 745f 6669 6c74 6572 da09    FZ.ot_filter..
+000047f0: 6469 7265 6374 6f72 7954 7a06 2066 696c  directoryTz. fil
+00004800: 6573 7a02 2a2e 4e29 0572 1e00 0000 721f  esz.*.N).r....r.
+00004810: 0000 00da 075f 6669 6c74 6572 da0c 5f69  ....._filter.._i
+00004820: 7364 6972 6563 746f 7279 da06 6170 7065  sdirectory..appe
+00004830: 6e64 2908 7229 0000 0072 2000 0000 722a  nd).r)...r ...r*
+00004840: 0000 0072 2200 0000 722b 0000 00da 0766  ...r"...r+.....f
+00004850: 696c 7465 7273 da03 6578 74da 0866 696c  ilters..ext..fil
+00004860: 6574 7970 6572 2c00 0000 722e 0000 0072  etyper,...r....r
+00004870: 2f00 0000 721f 0000 0049 0200 0073 1400  /...r....I...s..
+00004880: 0000 0008 1202 0601 0602 0801 0801 0801  ................
+00004890: 0802 0801 1401 7a16 4f54 4669 6c65 4272  ......z.OTFileBr
+000048a0: 6f77 7365 722e 5f5f 696e 6974 5f5f 6301  owser.__init__c.
+000048b0: 0000 0000 0000 0000 0000 0001 0000 0004  ................
+000048c0: 0000 0043 0000 0073 1c00 0000 7400 8300  ...C...s....t...
+000048d0: 7c00 5f01 7c00 6a01 a002 6401 7c00 6a03  |._.|.j...d.|.j.
+000048e0: a102 0100 6400 5300 726a 0000 0072 ca00  ....d.S.rj...r..
+000048f0: 0000 724d 0000 0072 2e00 0000 722e 0000  ..rM...r....r...
+00004900: 0072 2f00 0000 7225 0000 005f 0200 0073  .r/...r%..._...s
+00004910: 0400 0000 0001 0801 7a19 4f54 4669 6c65  ........z.OTFile
+00004920: 4272 6f77 7365 722e 5f64 6566 696e 655f  Browser._define_
+00004930: 7661 7263 0100 0000 0000 0000 0000 0000  varc............
+00004940: 0100 0000 0800 0000 4300 0000 73c8 0000  ........C...s...
+00004950: 007c 006a 006a 0164 0164 0164 0264 038d  .|.j.j.d.d.d.d..
+00004960: 0301 007c 006a 026a 0364 0474 0414 0064  ...|.j.j.d.t...d
+00004970: 058d 0101 0074 056a 067c 006a 027c 006a  .....t.j.|.j.|.j
+00004980: 0764 0664 0764 0864 098d 057c 005f 087c  .d.d.d.d...|._.|
+00004990: 006a 086a 0164 0164 0164 0a64 0b64 0c8d  .j.j.d.d.d.d.d..
+000049a0: 0401 0074 056a 097c 006a 0264 0d7c 006a  ...t.j.|.j.d.|.j
+000049b0: 0a64 0e8d 037c 005f 0b7c 006a 0b6a 0164  .d...|._.|.j.j.d
+000049c0: 0164 0164 0a64 0f64 0c8d 0401 007c 006a  .d.d.d.d.....|.j
+000049d0: 086a 0c7c 006a 0b6a 0d64 108d 0101 0074  .j.|.j.j.d.....t
+000049e0: 056a 0e7c 006a 0274 0f64 1119 0064 1274  .j.|.j.t.d...d.t
+000049f0: 1014 0064 1364 147c 006a 1164 158d 067c  ...d.d.|.j.d...|
+00004a00: 005f 127c 006a 126a 0164 1664 0164 1764  ._.|.j.j.d.d.d.d
+00004a10: 038d 0301 0064 0053 0029 184e 723b 0000  .....d.S.).Nr;..
+00004a20: 0072 c200 0000 7240 0000 0072 8a00 0000  .r....r@...r....
+00004a30: 728b 0000 0072 7c00 0000 7274 0000 00da  r....r|...rt....
+00004a40: 0572 6967 6874 2904 7275 0000 0072 1c00  .right).ru...r..
+00004a50: 0000 7278 0000 00da 076a 7573 7469 6679  ..rx.....justify
+00004a60: 679a 9999 9999 99d9 3f72 7b00 0000 2904  g.......?r{...).
+00004a70: 7241 0000 0072 4200 0000 da08 7265 6c77  rA...rB.....relw
+00004a80: 6964 7468 7243 0000 00da 0a68 6f72 697a  idthrC.....horiz
+00004a90: 6f6e 7461 6c29 02da 066f 7269 656e 7472  ontal)...orientr
+00004aa0: c400 0000 da02 6e77 2901 da0e 7873 6372  ......nw)...xscr
+00004ab0: 6f6c 6c63 6f6d 6d61 6e64 da04 6c6f 6164  ollcommand..load
+00004ac0: 679a 9999 9999 99b9 3f72 8f00 0000 fa0b  g.......?r......
+00004ad0: 636c 616d 2e54 4c61 6265 6c29 0572 9e00  clam.TLabel).r..
+00004ae0: 0000 7230 0000 0072 9200 0000 7291 0000  ..r0...r....r...
+00004af0: 0072 c400 0000 72a1 0000 0072 6b00 0000  .r....r....rk...
+00004b00: 2913 724a 0000 0072 4b00 0000 7245 0000  ).rJ...rK...rE..
+00004b10: 0072 9800 0000 7213 0000 0072 0200 0000  .r....r....r....
+00004b20: 7208 0000 0072 6d00 0000 727e 0000 00da  r....rm...r~....
+00004b30: 0953 6372 6f6c 6c62 6172 da1d 5f4f 5446  .Scrollbar.._OTF
+00004b40: 696c 6542 726f 7773 6572 5f5f 7363 726f  ileBrowser__scro
+00004b50: 6c6c 4861 6e64 6c65 725a 075f 7363 726f  llHandlerZ._scro
+00004b60: 6c6c 7284 0000 0072 5100 0000 da06 4275  llr....rQ.....Bu
+00004b70: 7474 6f6e 7214 0000 0072 1200 0000 da07  ttonr....r......
+00004b80: 5f62 726f 7773 65da 045f 6274 6e72 4d00  _browse.._btnrM.
+00004b90: 0000 722e 0000 0072 2e00 0000 722f 0000  ..r....r....r/..
+00004ba0: 0072 2600 0000 6302 0000 7328 0000 0000  .r&...c...s(....
+00004bb0: 0212 0112 0208 0104 0102 0102 0102 fc08  ................
+00004bc0: 0514 0216 0114 0112 0208 0106 0106 0102  ................
+00004bd0: 0102 0104 fb08 077a 1d4f 5446 696c 6542  .......z.OTFileB
+00004be0: 726f 7773 6572 2e5f 6372 6561 7465 5f77  rowser._create_w
+00004bf0: 6964 6765 7473 6301 0000 0000 0000 0000  idgetsc.........
+00004c00: 0000 0005 0000 0004 0000 0047 0000 0073  ...........G...s
+00004c10: 4a00 0000 7c01 6401 1900 7c01 6402 1900  J...|.d...|.d...
+00004c20: 0200 7d02 7d03 7c02 6403 6b02 7232 7c01  ..}.}.|.d.k.r2|.
+00004c30: 6404 1900 7d04 7c00 6a00 a001 7c03 7c04  d...}.|.j...|.|.
+00004c40: a102 0100 6e14 7c02 6405 6b02 7246 7c00  ....n.|.d.k.rF|.
+00004c50: 6a00 a002 7c03 a101 0100 6406 5300 2907  j...|.....d.S.).
+00004c60: 7a1d 4361 6c6c 6261 636b 2066 6f72 2065  z.Callback for e
+00004c70: 6e74 7279 2073 6372 6f6c 6c62 6172 2072  ntry scrollbar r
+00004c80: 0100 0000 7234 0000 00da 0673 6372 6f6c  ....r4.....scrol
+00004c90: 6c72 8a00 0000 da06 6d6f 7665 746f 4e29  lr......movetoN)
+00004ca0: 0372 7e00 0000 da0c 7876 6965 775f 7363  .r~.....xview_sc
+00004cb0: 726f 6c6c da0c 7876 6965 775f 6d6f 7665  roll..xview_move
+00004cc0: 746f 2905 7229 0000 00da 014c da02 6f70  to).r).....L..op
+00004cd0: 5a07 686f 774d 616e 79da 0575 6e69 7473  Z.howMany..units
+00004ce0: 722e 0000 0072 2e00 0000 722f 0000 005a  r....r....r/...Z
+00004cf0: 0f5f 5f73 6372 6f6c 6c48 616e 646c 6572  .__scrollHandler
+00004d00: 7c02 0000 730c 0000 0000 0212 0108 0108  |...s...........
+00004d10: 0110 0108 017a 1d4f 5446 696c 6542 726f  .....z.OTFileBro
+00004d20: 7773 6572 2e5f 5f73 6372 6f6c 6c48 616e  wser.__scrollHan
+00004d30: 646c 6572 4e63 0200 0000 0000 0000 0000  dlerNc..........
+00004d40: 0000 0400 0000 0400 0000 4300 0000 7360  ..........C...s`
+00004d50: 0000 007c 00a0 00a1 007d 027c 006a 0172  ...|.....}.|.j.r
+00004d60: 1e74 026a 037c 006a 0464 018d 017d 036e  .t.j.|.j.d...}.n
+00004d70: 1274 026a 057c 006a 047c 006a 0664 028d  .t.j.|.j.|.j.d..
+00004d80: 027d 037c 0364 036b 0272 3c64 0453 0074  .}.|.d.k.r<d.S.t
+00004d90: 076a 08a0 097c 03a1 017d 037c 037c 026b  .j...|...}.|.|.k
+00004da0: 0372 5c7c 006a 0aa0 0b7c 03a1 0101 0064  .r\|.j...|.....d
+00004db0: 0453 0029 057a 1a42 726f 7773 6520 6469  .S.).z.Browse di
+00004dc0: 7265 6374 6f72 7920 6f72 2066 696c 6573  rectory or files
+00004dd0: 2e29 0172 1a00 0000 2902 721a 0000 00da  .).r....).r.....
+00004de0: 0966 696c 6574 7970 6573 7254 0000 004e  .filetypesrT...N
+00004df0: 290c 7221 0000 0072 f000 0000 720a 0000  ).r!...r....r...
+00004e00: 00da 0c61 736b 6469 7265 6374 6f72 7972  ...askdirectoryr
+00004e10: 1a00 0000 da0f 6173 6b6f 7065 6e66 696c  ......askopenfil
+00004e20: 656e 616d 6572 ef00 0000 da02 6f73 da04  enamer......os..
+00004e30: 7061 7468 da07 7265 6c70 6174 6872 6d00  path..relpathrm.
+00004e40: 0000 7251 0000 0029 0472 2900 0000 da05  ..rQ...).r).....
+00004e50: 6576 656e 745a 0863 7572 5f70 6174 6872  eventZ.cur_pathr
+00004e60: 0e01 0000 722e 0000 0072 2e00 0000 722f  ....r....r....r/
+00004e70: 0000 0072 0101 0000 8502 0000 7316 0000  ...r........s...
+00004e80: 0000 0208 0206 0110 0208 0104 ff06 0308  ................
+00004e90: 0104 020c 0108 017a 154f 5446 696c 6542  .......z.OTFileB
+00004ea0: 726f 7773 6572 2e5f 6272 6f77 7365 6301  rowser._browsec.
+00004eb0: 0000 0000 0000 0000 0000 0002 0000 0003  ................
+00004ec0: 0000 0043 0000 0073 2400 0000 7c00 6a00  ...C...s$...|.j.
+00004ed0: 6401 6b02 720e 6402 6e02 6403 7d01 7c00  d.k.r.d.n.d.}.|.
+00004ee0: 6a01 6a02 7c01 6404 8d01 0100 6400 5300  j.j.|.d.....d.S.
+00004ef0: 2905 4e72 3400 0000 da06 5445 6e74 7279  ).Nr4.....TEntry
+00004f00: fa12 4869 6768 6c69 6768 7465 642e 5445  ..Highlighted.TE
+00004f10: 6e74 7279 72c7 0000 0029 0372 5700 0000  ntryr....).rW...
+00004f20: 727e 0000 0072 8400 0000 72c8 0000 0072  r~...r....r....r
+00004f30: 2e00 0000 722e 0000 0072 2f00 0000 725e  ....r....r/...r^
+00004f40: 0000 0096 0200 0073 0400 0000 0001 1201  .......s........
+00004f50: 7a23 4f54 4669 6c65 4272 6f77 7365 722e  z#OTFileBrowser.
+00004f60: 5f75 7064 6174 655f 7769 6467 6574 735f  _update_widgets_
+00004f70: 7374 796c 6563 0100 0000 0000 0000 0000  stylec..........
+00004f80: 0000 0100 0000 0200 0000 4300 0000 730a  ..........C...s.
+00004f90: 0000 007c 006a 00a0 01a1 0053 0072 4c00  ...|.j.....S.rL.
+00004fa0: 0000 726f 0000 0072 4d00 0000 722e 0000  ..ro...rM...r...
+00004fb0: 0072 2e00 0000 722f 0000 0072 2100 0000  .r....r/...r!...
+00004fc0: 9a02 0000 7302 0000 0000 017a 114f 5446  ....s......z.OTF
+00004fd0: 696c 6542 726f 7773 6572 2e67 6574 6302  ileBrowser.getc.
+00004fe0: 0000 0000 0000 0000 0000 0002 0000 0003  ................
+00004ff0: 0000 0043 0000 0073 1000 0000 7c00 6a00  ...C...s....|.j.
+00005000: a001 7c01 a101 0100 6400 5300 724c 0000  ..|.....d.S.rL..
+00005010: 0072 7000 0000 7271 0000 0072 2e00 0000  .rp...rq...r....
+00005020: 722e 0000 0072 2f00 0000 7251 0000 009d  r....r/...rQ....
+00005030: 0200 0073 0200 0000 0001 7a11 4f54 4669  ...s......z.OTFi
+00005040: 6c65 4272 6f77 7365 722e 7365 7429 014e  leBrowser.set).N
+00005050: 290c 7263 0000 0072 6400 0000 7265 0000  ).rc...rd...re..
+00005060: 0072 1f00 0000 7225 0000 0072 2600 0000  .r....r%...r&...
+00005070: 72ff 0000 0072 0101 0000 725e 0000 0072  r....r....r^...r
+00005080: 2100 0000 7251 0000 0072 6700 0000 722e  !...rQ...rg...r.
+00005090: 0000 0072 2e00 0000 722c 0000 0072 2f00  ...r....r,...r/.
+000050a0: 0000 72ec 0000 0047 0200 0073 1000 0000  ..r....G...s....
+000050b0: 0802 0c16 0804 0819 0809 0a11 0804 0803  ................
+000050c0: 72ec 0000 0063 0000 0000 0000 0000 0000  r....c..........
+000050d0: 0000 0000 0000 0300 0000 0000 0000 7320  ..............s 
+000050e0: 0000 0065 005a 0164 005a 0264 015a 0387  ...e.Z.d.Z.d.Z..
+000050f0: 0066 0164 0264 0384 085a 0487 0004 005a  .f.d.d...Z.....Z
+00005100: 0553 0029 0472 d200 0000 7a96 5468 6973  .S.).r....z.This
+00005110: 2070 6172 7469 6375 6c61 7220 636c 6173   particular clas
+00005120: 7320 6973 2066 6f72 2063 686f 6f73 696e  s is for choosin
+00005130: 6720 616d 6f6e 6720 6120 7661 7269 6162  g among a variab
+00005140: 6c65 2073 6574 206f 6620 6f70 7469 6f6e  le set of option
+00005150: 0a20 2020 200a 2020 2020 4578 616d 706c  .    .    Exampl
+00005160: 653a 2073 656c 6563 7420 6120 7061 7463  e: select a patc
+00005170: 6820 6e61 6d65 2061 6d6f 6e67 2061 206c  h name among a l
+00005180: 6973 7420 666f 756e 6420 696e 2061 6e20  ist found in an 
+00005190: 6578 7465 726e 616c 2066 696c 650a 2020  external file.  
+000051a0: 2020 6302 0000 0000 0000 0000 0000 0005    c.............
+000051b0: 0000 0003 0000 0003 0000 0073 4200 0000  ...........sB...
+000051c0: 7400 7c00 6a01 a002 a100 8301 7d02 7c00  t.|.j.......}.|.
+000051d0: 6a03 6401 1900 7d03 7c02 7c03 1900 6402  j.d...}.|.|...d.
+000051e0: 6402 8502 1900 7d04 7c00 a004 7c04 a101  d.....}.|...|...
+000051f0: 0100 7405 8300 a006 7c01 a101 0100 6402  ..t.....|.....d.
+00005200: 5300 2903 7a20 5265 636f 6e66 6967 7572  S.).z Reconfigur
+00005210: 6520 7468 6520 6f70 7469 6f6e 7320 7768  e the options wh
+00005220: 656e 2073 6574 72ce 0000 004e 2907 720d  en setr....N).r.
+00005230: 0000 00da 126d 795f 726f 6f74 5f74 6162  .....my_root_tab
+00005240: 5f77 6964 6765 7472 2100 0000 7220 0000  _widgetr!...r ..
+00005250: 0072 e500 0000 721e 0000 0072 5100 0000  .r....r....rQ...
+00005260: 2905 7229 0000 0072 7200 0000 da04 7472  ).r)...rr.....tr
+00005270: 6565 da03 6b65 7972 e600 0000 722c 0000  ee..keyr....r,..
+00005280: 0072 2e00 0000 722f 0000 0072 5100 0000  .r....r/...rQ...
+00005290: a702 0000 730a 0000 0000 020e 010a 0110  ....s...........
+000052a0: 010a 017a 145f 4f54 4368 6f69 6365 4479  ...z._OTChoiceDy
+000052b0: 6e61 6d69 632e 7365 7429 0672 6300 0000  namic.set).rc...
+000052c0: 7264 0000 0072 6500 0000 7266 0000 0072  rd...re...rf...r
+000052d0: 5100 0000 7267 0000 0072 2e00 0000 722e  Q...rg...r....r.
+000052e0: 0000 0072 2c00 0000 722f 0000 0072 d200  ...r,...r/...r..
+000052f0: 0000 a102 0000 7304 0000 0008 0104 0572  ......s........r
+00005300: d200 0000 6300 0000 0000 0000 0000 0000  ....c...........
+00005310: 0000 0000 0003 0000 0000 0000 0073 4e00  .............sN.
+00005320: 0000 6500 5a01 6400 5a02 8700 6601 6401  ..e.Z.d.Z...f.d.
+00005330: 6402 8408 5a03 6403 6404 8400 5a04 6405  d...Z.d.d...Z.d.
+00005340: 6406 8400 5a05 6407 6408 8400 5a06 6410  d...Z.d.d...Z.d.
+00005350: 640a 640b 8401 5a07 640c 640d 8400 5a08  d.d...Z.d.d...Z.
+00005360: 640e 640f 8400 5a09 8700 0400 5a0a 5300  d.d...Z.....Z.S.
+00005370: 2911 da06 4f54 446f 6375 6305 0000 0000  )...OTDocuc.....
+00005380: 0000 0000 0000 0005 0000 0006 0000 0003  ................
+00005390: 0000 0073 2600 0000 7400 8300 a001 7c01  ...s&...t.....|.
+000053a0: 7c02 7c03 7c04 a104 0100 7402 7c04 8301  |.|.|.....t.|...
+000053b0: 7c00 5f03 6401 7c00 5f04 6401 5300 2902  |._.d.|._.d.S.).
+000053c0: 72ed 0000 004e 2905 721e 0000 0072 1f00  r....N).r....r..
+000053d0: 0000 7217 0000 00da 0472 6f6f 74da 075f  ..r......root.._
+000053e0: 6469 616c 6f67 7228 0000 0072 2c00 0000  dialogr(...r,...
+000053f0: 722e 0000 0072 2f00 0000 721f 0000 00b3  r....r/...r.....
+00005400: 0200 0073 0600 0000 0008 1201 0a02 7a0f  ...s..........z.
+00005410: 4f54 446f 6375 2e5f 5f69 6e69 745f 5f63  OTDocu.__init__c
+00005420: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00005430: 0400 0000 4300 0000 731c 0000 0074 0083  ....C...s....t..
+00005440: 007c 005f 017c 006a 01a0 0264 017c 006a  .|._.|.j...d.|.j
+00005450: 03a1 0201 0064 0053 0072 6a00 0000 72ca  .....d.S.rj...r.
+00005460: 0000 0072 4d00 0000 722e 0000 0072 2e00  ...rM...r....r..
+00005470: 0000 722f 0000 0072 2500 0000 c002 0000  ..r/...r%.......
+00005480: 7304 0000 0000 0208 017a 124f 5444 6f63  s........z.OTDoc
+00005490: 752e 5f64 6566 696e 655f 7661 7263 0100  u._define_varc..
+000054a0: 0000 0000 0000 0000 0000 0100 0000 0800  ................
+000054b0: 0000 4300 0000 734a 0000 0074 006a 017c  ..C...sJ...t.j.|
+000054c0: 006a 0264 0174 0314 0064 0274 0464 0319  .j.d.t...d.t.d..
+000054d0: 0064 047c 006a 0564 058d 067c 005f 067c  .d.|.j.d...|._.|
+000054e0: 006a 066a 0764 0664 0764 0264 088d 0301  .j.j.d.d.d.d....
+000054f0: 007c 006a 026a 0864 0964 0a64 0b8d 0201  .|.j.j.d.d.d....
+00005500: 0064 0053 0029 0c4e 677b 14ae 47e1 7a84  .d.S.).Ng{..G.z.
+00005510: 3fda 0663 656e 7465 72da 0464 6f63 7572  ?..center..docur
+00005520: fd00 0000 2905 7230 0000 0072 9200 0000  ....).r0...r....
+00005530: 729e 0000 0072 9100 0000 72c4 0000 0072  r....r....r....r
+00005540: a100 0000 723b 0000 0072 4000 0000 da06  ....r;...r@.....
+00005550: 626f 7474 6f6d 7238 0000 0072 3900 0000  bottomr8...r9...
+00005560: 2909 7202 0000 0072 0001 0000 7245 0000  ).r....r....rE..
+00005570: 0072 1200 0000 7214 0000 00da 0d5f 706f  .r....r......_po
+00005580: 7075 705f 6469 616c 6f67 7202 0100 0072  pup_dialogr....r
+00005590: 4b00 0000 da0e 7061 636b 5f63 6f6e 6669  K.....pack_confi
+000055a0: 6775 7265 724d 0000 0072 2e00 0000 722e  gurerM...r....r.
+000055b0: 0000 0072 2f00 0000 7226 0000 00c5 0200  ...r/...r&......
+000055c0: 0073 1200 0000 0001 0801 0601 0201 0601  .s..............
+000055d0: 0201 04fb 0806 1201 7a16 4f54 446f 6375  ........z.OTDocu
+000055e0: 2e5f 6372 6561 7465 5f77 6964 6765 7473  ._create_widgets
+000055f0: 6301 0000 0000 0000 0000 0000 0004 0000  c...............
+00005600: 0007 0000 0043 0000 0073 2801 0000 7400  .....C...s(...t.
+00005610: 7c00 6a01 8301 7c00 5f02 7c00 6a02 a003  |.j...|._.|.j...
+00005620: 7c00 6a01 a101 0100 7c00 6a02 a004 6401  |.j.....|.j...d.
+00005630: a101 0100 7c00 6a02 a005 a100 0100 7c00  ....|.j.......|.
+00005640: 6a02 a006 6402 7c00 6a07 a102 0100 7c00  j...d.|.j.....|.
+00005650: 6a02 a006 6403 7c00 6a07 a102 0100 7c00  j...d.|.j.....|.
+00005660: 6a02 a008 6404 7c00 6a07 a102 0100 7409  j...d.|.j.....t.
+00005670: 6a0a 7c00 6a02 6405 740b 1400 6405 740b  j.|.j.d.t...d.t.
+00005680: 1400 6406 8d03 7d01 7c01 6a0c 6407 6408  ..d...}.|.j.d.d.
+00005690: 6409 640a 8d03 0100 7c01 a00d 640b a101  d.d.....|...d...
+000056a0: 0100 7c01 6a0e 640c 640d 640e 8d02 0100  ..|.j.d.d.d.....
+000056b0: 7c01 6a0f 640c 640d 640e 8d02 0100 7409  |.j.d.d.d.....t.
+000056c0: a010 7c01 a101 7d02 7c02 6a0c 640f 6410  ..|...}.|.j.d.d.
+000056d0: 6411 8d02 0100 7411 7c01 6412 7c02 6a12  d.....t.|.d.|.j.
+000056e0: 6413 740b 1400 6414 6415 8d05 7d03 7c03  d.t...d.d...}.|.
+000056f0: 6a13 6416 6417 6418 8d02 0100 7c03 a014  j.d.d.d.....|...
+00005700: 6419 7c00 6a15 a016 a100 6416 a103 0100  d.|.j.....d.....
+00005710: 7c03 6a17 641a 641b 8d01 0100 7c03 a00c  |.j.d.d.....|...
+00005720: a100 0100 7c02 6a17 7c03 6a18 641c 8d01  ....|.j.|.j.d...
+00005730: 0100 641d 5300 291e 7a28 4469 7370 6c61  ..d.S.).z(Displa
+00005740: 7920 636f 6e74 656e 7420 6f66 2064 6f63  y content of doc
+00005750: 756d 656e 7461 7469 6f6e 2073 7472 696e  umentation strin
+00005760: 672e 5a0d 446f 6375 6d65 6e74 6174 696f  g.Z.Documentatio
+00005770: 6e7a 0b3c 436f 6e74 726f 6c2d 773e 7a08  nz.<Control-w>z.
+00005780: 3c45 7363 6170 653e da10 574d 5f44 454c  <Escape>..WM_DEL
+00005790: 4554 455f 5749 4e44 4f57 e903 0000 0029  ETE_WINDOW.....)
+000057a0: 0272 3000 0000 7231 0000 0072 3500 0000  .r0...r1...r5...
+000057b0: da04 626f 7468 5429 0372 3700 0000 723a  ..bothT).r7...r:
+000057c0: 0000 00da 0665 7870 616e 6446 7201 0000  .....expandFr...
+000057d0: 0072 3400 0000 2901 da06 7765 6967 6874  .r4...)...weight
+000057e0: 72f5 0000 00da 0179 7239 0000 00da 0477  r......yr9.....w
+000057f0: 6f72 6467 7b14 ae47 e17a 943f 72d6 0000  ordg{..G.z.?r...
+00005800: 0029 04da 0477 7261 70da 0e79 7363 726f  .)...wrap..yscro
+00005810: 6c6c 636f 6d6d 616e 6472 7600 0000 72d7  llcommandrv...r.
+00005820: 0000 00da 0462 6f6c 6429 035a 0554 696d  .....bold).Z.Tim
+00005830: 6573 e90e 0000 0072 1d00 0000 2901 da04  es.....r....)...
+00005840: 666f 6e74 da03 656e 6472 7c00 0000 a901  font..endr|.....
+00005850: 721c 0000 00a9 0172 c400 0000 4e29 1972  r......r....N).r
+00005860: 0600 0000 7217 0100 0072 1801 0000 da09  ....r....r......
+00005870: 7472 616e 7369 656e 7472 1a00 0000 da08  transientr......
+00005880: 6772 6162 5f73 6574 da04 6269 6e64 da0f  grab_set..bind..
+00005890: 5f64 6573 7472 6f79 5f64 6961 6c6f 67da  _destroy_dialog.
+000058a0: 0870 726f 746f 636f 6c72 0200 0000 7244  .protocolr....rD
+000058b0: 0000 0072 1200 0000 7247 0000 00da 0e67  ...r....rG.....g
+000058c0: 7269 645f 7072 6f70 6167 6174 65da 1167  rid_propagate..g
+000058d0: 7269 645f 726f 7763 6f6e 6669 6775 7265  rid_rowconfigure
+000058e0: da14 6772 6964 5f63 6f6c 756d 6e63 6f6e  ..grid_columncon
+000058f0: 6669 6775 7265 72fe 0000 0072 0700 0000  figurer....r....
+00005900: 7251 0000 00da 0d74 6167 5f63 6f6e 6669  rQ.....tag_confi
+00005910: 6775 7265 da06 696e 7365 7274 726d 0000  gure..insertrm..
+00005920: 0072 2100 0000 7298 0000 00da 0579 7669  .r!...r......yvi
+00005930: 6577 2904 7229 0000 005a 0964 6c67 5f66  ew).r)...Z.dlg_f
+00005940: 7261 6d65 da09 7363 726f 6c6c 6261 725a  rame..scrollbarZ
+00005950: 0774 6578 745f 7764 722e 0000 0072 2e00  .text_wdr....r..
+00005960: 0000 722f 0000 0072 1c01 0000 cf02 0000  ..r/...r........
+00005970: 733a 0000 0000 030c 010e 010c 010a 0210  s:..............
+00005980: 0110 0110 0208 0106 0106 fe06 0310 010a  ................
+00005990: 010e 010e 020a 010e 0202 0102 0102 0104  ................
+000059a0: 0106 0102 fb06 080e 0114 010c 0108 017a  ...............z
+000059b0: 144f 5444 6f63 752e 5f70 6f70 7570 5f64  .OTDocu._popup_d
+000059c0: 6961 6c6f 674e 6302 0000 0000 0000 0000  ialogNc.........
+000059d0: 0000 0002 0000 0002 0000 0043 0000 0073  ...........C...s
+000059e0: 1e00 0000 7c00 6a00 a001 a100 0100 7c00  ....|.j.......|.
+000059f0: 6a02 a003 a100 0100 6401 7c00 5f02 6401  j.......d.|._.d.
+00005a00: 5300 2902 7a12 4465 7374 726f 7969 6e67  S.).z.Destroying
+00005a10: 2064 6961 6c6f 672e 4e29 0472 1701 0000   dialog.N).r....
+00005a20: da09 666f 6375 735f 7365 7472 1801 0000  ..focus_setr....
+00005a30: 7261 0000 00a9 0272 2900 0000 7210 0100  ra.....r)...r...
+00005a40: 0072 2e00 0000 722e 0000 0072 2f00 0000  .r....r....r/...
+00005a50: 7230 0100 00f4 0200 0073 0600 0000 0002  r0.......s......
+00005a60: 0a01 0a01 7a16 4f54 446f 6375 2e5f 6465  ....z.OTDocu._de
+00005a70: 7374 726f 795f 6469 616c 6f67 6301 0000  stroy_dialogc...
+00005a80: 0000 0000 0000 0000 0001 0000 0002 0000  ................
+00005a90: 0043 0000 0073 0a00 0000 7c00 6a00 a001  .C...s....|.j...
+00005aa0: a100 5300 2901 7a0c 566f 6964 2072 6574  ..S.).z.Void ret
+00005ab0: 7572 6e2e 726f 0000 0072 4d00 0000 722e  urn.ro...rM...r.
+00005ac0: 0000 0072 2e00 0000 722f 0000 0072 2100  ...r....r/...r!.
+00005ad0: 0000 fa02 0000 7302 0000 0000 027a 0a4f  ......s......z.O
+00005ae0: 5444 6f63 752e 6765 7463 0200 0000 0000  TDocu.getc......
+00005af0: 0000 0000 0000 0200 0000 0300 0000 4300  ..............C.
+00005b00: 0000 7310 0000 007c 006a 00a0 017c 01a1  ..s....|.j...|..
+00005b10: 0101 0064 0153 0029 027a 2353 6574 2076  ...d.S.).z#Set v
+00005b20: 616c 7565 2074 6f20 646f 6375 6d65 6e74  alue to document
+00005b30: 6174 696f 6e20 636f 6e74 656e 742e 4e72  ation content.Nr
+00005b40: 7000 0000 7271 0000 0072 2e00 0000 722e  p...rq...r....r.
+00005b50: 0000 0072 2f00 0000 7251 0000 00fe 0200  ...r/...rQ......
+00005b60: 0073 0200 0000 0002 7a0a 4f54 446f 6375  .s......z.OTDocu
+00005b70: 2e73 6574 2901 4e29 0b72 6300 0000 7264  .set).N).rc...rd
+00005b80: 0000 0072 6500 0000 721f 0000 0072 2500  ...re...r....r%.
+00005b90: 0000 7226 0000 0072 1c01 0000 7230 0100  ..r&...r....r0..
+00005ba0: 0072 2100 0000 7251 0000 0072 6700 0000  .r!...rQ...rg...
+00005bb0: 722e 0000 0072 2e00 0000 722c 0000 0072  r....r....r,...r
+00005bc0: 2f00 0000 7216 0100 00b1 0200 0073 0e00  /...r........s..
+00005bd0: 0000 0802 0c0d 0805 080a 0825 0a06 0804  ...........%....
+00005be0: 7216 0100 0063 0000 0000 0000 0000 0000  r....c..........
+00005bf0: 0000 0000 0000 0300 0000 0000 0000 733c  ..............s<
+00005c00: 0000 0065 005a 0164 005a 0287 0066 0164  ...e.Z.d.Z...f.d
+00005c10: 0164 0284 085a 0364 0364 0484 005a 0464  .d...Z.d.d...Z.d
+00005c20: 0564 0684 005a 0564 0764 0884 005a 0664  .d...Z.d.d...Z.d
+00005c30: 0964 0a84 005a 0787 0004 005a 0853 0029  .d...Z.....Z.S.)
+00005c40: 0bda 0d4f 5444 6573 6372 6970 7469 6f6e  ...OTDescription
+00005c50: 6305 0000 0000 0000 0000 0000 0005 0000  c...............
+00005c60: 0006 0000 0003 0000 0073 2600 0000 7400  .........s&...t.
+00005c70: 8300 a001 7c01 7c02 7c03 7c04 a104 0100  ....|.|.|.|.....
+00005c80: 7c00 6a02 6a03 6401 6402 6403 8d02 0100  |.j.j.d.d.d.....
+00005c90: 6404 5300 2905 72ed 0000 0072 1b01 0000  d.S.).r....r....
+00005ca0: 7238 0000 0072 3900 0000 4e29 0472 1e00  r8...r9...N).r..
+00005cb0: 0000 721f 0000 0072 4500 0000 721d 0100  ..r....rE...r...
+00005cc0: 0072 2800 0000 722c 0000 0072 2e00 0000  .r(...r,...r....
+00005cd0: 722f 0000 0072 1f00 0000 0503 0000 7304  r/...r........s.
+00005ce0: 0000 0000 0812 017a 164f 5444 6573 6372  .......z.OTDescr
+00005cf0: 6970 7469 6f6e 2e5f 5f69 6e69 745f 5f63  iption.__init__c
+00005d00: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00005d10: 0400 0000 4300 0000 731c 0000 0074 0083  ....C...s....t..
+00005d20: 007c 005f 017c 006a 01a0 0264 017c 006a  .|._.|.j...d.|.j
+00005d30: 03a1 0201 0064 0053 0072 6a00 0000 72ca  .....d.S.rj...r.
+00005d40: 0000 0072 4d00 0000 722e 0000 0072 2e00  ...rM...r....r..
+00005d50: 0000 722f 0000 0072 2500 0000 1003 0000  ..r/...r%.......
+00005d60: 7304 0000 0000 0208 017a 194f 5444 6573  s........z.OTDes
+00005d70: 6372 6970 7469 6f6e 2e5f 6465 6669 6e65  cription._define
+00005d80: 5f76 6172 6301 0000 0000 0000 0000 0000  _varc...........
+00005d90: 0001 0000 0005 0000 0043 0000 0073 2a00  .........C...s*.
+00005da0: 0000 7c00 6a00 6a01 6401 7c00 6a02 7403  ..|.j.j.d.|.j.t.
+00005db0: 6402 1400 6403 8d03 0100 7c00 6a00 6a04  d...d.....|.j.j.
+00005dc0: 6404 6405 8d01 0100 6400 5300 2906 4e72  d.d.....d.S.).Nr
+00005dd0: 8f00 0000 679a 9999 9999 99e9 3f29 0372  ....g.......?).r
+00005de0: f600 0000 7275 0000 0072 3d00 0000 721b  ....ru...r=...r.
+00005df0: 0100 00a9 0172 3700 0000 2905 724a 0000  .....r7...).rJ..
+00005e00: 0072 9800 0000 726d 0000 0072 1200 0000  .r....rm...r....
+00005e10: 7247 0000 0072 4d00 0000 722e 0000 0072  rG...rM...r....r
+00005e20: 2e00 0000 722f 0000 0072 2600 0000 1503  ....r/...r&.....
+00005e30: 0000 730a 0000 0000 0108 0104 0106 fe06  ..s.............
+00005e40: 037a 1d4f 5444 6573 6372 6970 7469 6f6e  .z.OTDescription
+00005e50: 2e5f 6372 6561 7465 5f77 6964 6765 7473  ._create_widgets
+00005e60: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00005e70: 0002 0000 0043 0000 0073 0a00 0000 7c00  .....C...s....|.
+00005e80: 6a00 a001 a100 5300 724c 0000 0072 6f00  j.....S.rL...ro.
+00005e90: 0000 724d 0000 0072 2e00 0000 722e 0000  ..rM...r....r...
+00005ea0: 0072 2f00 0000 7221 0000 001b 0300 0073  .r/...r!.......s
+00005eb0: 0200 0000 0001 7a11 4f54 4465 7363 7269  ......z.OTDescri
+00005ec0: 7074 696f 6e2e 6765 7463 0200 0000 0000  ption.getc......
+00005ed0: 0000 0000 0000 0200 0000 0300 0000 4300  ..............C.
+00005ee0: 0000 7310 0000 007c 006a 00a0 017c 01a1  ..s....|.j...|..
+00005ef0: 0101 0064 0053 0072 4c00 0000 7270 0000  ...d.S.rL...rp..
+00005f00: 0072 7100 0000 722e 0000 0072 2e00 0000  .rq...r....r....
+00005f10: 722f 0000 0072 5100 0000 1e03 0000 7302  r/...rQ.......s.
+00005f20: 0000 0000 017a 114f 5444 6573 6372 6970  .....z.OTDescrip
+00005f30: 7469 6f6e 2e73 6574 2909 7263 0000 0072  tion.set).rc...r
+00005f40: 6400 0000 7265 0000 0072 1f00 0000 7225  d...re...r....r%
+00005f50: 0000 0072 2600 0000 7221 0000 0072 5100  ...r&...r!...rQ.
+00005f60: 0000 7267 0000 0072 2e00 0000 722e 0000  ..rg...r....r...
+00005f70: 0072 2c00 0000 722f 0000 0072 3b01 0000  .r,...r/...r;...
+00005f80: 0303 0000 730a 0000 0008 020c 0b08 0508  ....s...........
+00005f90: 0608 0372 3b01 0000 6300 0000 0000 0000  ...r;...c.......
+00005fa0: 0000 0000 0000 0000 0003 0000 0000 0000  ................
+00005fb0: 0073 5400 0000 6500 5a01 6400 5a02 8700  .sT...e.Z.d.Z...
+00005fc0: 6601 6401 6402 8408 5a03 6403 6404 8400  f.d.d...Z.d.d...
+00005fd0: 5a04 6405 6406 8400 5a05 6407 6408 8400  Z.d.d...Z.d.d...
+00005fe0: 5a06 6409 640a 8400 5a07 640b 640c 8400  Z.d.d...Z.d.d...
+00005ff0: 5a08 640d 640e 8400 5a09 640f 6410 8400  Z.d.d...Z.d.d...
+00006000: 5a0a 8700 0400 5a0b 5300 2911 da09 4f54  Z.....Z.S.)...OT
+00006010: 436f 6d6d 656e 7463 0500 0000 0000 0000  Commentc........
+00006020: 0000 0000 0600 0000 0600 0000 0300 0000  ................
+00006030: 735c 0000 007c 01a0 0064 0164 02a1 027d  s\...|...d.d...}
+00006040: 057c 0564 036b 027c 005f 0174 0283 00a0  .|.d.k.|._.t....
+00006050: 037c 017c 027c 037c 04a1 0401 007c 006a  .|.|.|.|.....|.j
+00006060: 046a 0564 0464 0564 068d 0201 007c 006a  .j.d.d.d.....|.j
+00006070: 04a0 0664 077c 006a 07a1 0201 007c 006a  ...d.|.j.....|.j
+00006080: 04a0 0664 087c 006a 08a1 0201 0064 0953  ...d.|.j.....d.S
+00006090: 0029 0a72 ed00 0000 721c 0000 0072 1d00  .).r....r....r..
+000060a0: 0000 727c 0000 0072 3500 0000 7238 0000  ..r|...r5...r8..
+000060b0: 0072 3900 0000 fa07 3c45 6e74 6572 3efa  .r9.....<Enter>.
+000060c0: 073c 4c65 6176 653e 4e29 0972 2100 0000  .<Leave>N).r!...
+000060d0: 727c 0000 0072 1e00 0000 721f 0000 0072  r|...r....r....r
+000060e0: 4500 0000 721d 0100 0072 2f01 0000 da15  E...r....r/.....
+000060f0: 5f75 6e62 696e 645f 676c 6f62 616c 5f73  _unbind_global_s
+00006100: 6372 6f6c 6cda 135f 6269 6e64 5f67 6c6f  croll.._bind_glo
+00006110: 6261 6c5f 7363 726f 6c6c 2906 7229 0000  bal_scroll).r)..
+00006120: 0072 2000 0000 722a 0000 0072 2200 0000  .r ...r*...r"...
+00006130: 722b 0000 0072 1c00 0000 722c 0000 0072  r+...r....r,...r
+00006140: 2e00 0000 722f 0000 0072 1f00 0000 2403  ....r/...r....$.
+00006150: 0000 730c 0000 0000 080c 010a 0212 0210  ..s.............
+00006160: 0210 017a 124f 5443 6f6d 6d65 6e74 2e5f  ...z.OTComment._
+00006170: 5f69 6e69 745f 5f63 0100 0000 0000 0000  _init__c........
+00006180: 0000 0000 0100 0000 0400 0000 4300 0000  ............C...
+00006190: 731c 0000 0074 0083 007c 005f 017c 006a  s....t...|._.|.j
+000061a0: 01a0 0264 017c 006a 03a1 0201 0064 0053  ...d.|.j.....d.S
+000061b0: 0072 6a00 0000 72ca 0000 0072 4d00 0000  .rj...r....rM...
+000061c0: 722e 0000 0072 2e00 0000 722f 0000 0072  r....r....r/...r
+000061d0: 2500 0000 3603 0000 7304 0000 0000 0108  %...6...s.......
+000061e0: 017a 154f 5443 6f6d 6d65 6e74 2e5f 6465  .z.OTComment._de
+000061f0: 6669 6e65 5f76 6172 6301 0000 0000 0000  fine_varc.......
+00006200: 0000 0000 0002 0000 0007 0000 0043 0000  .............C..
+00006210: 0073 2c00 0000 7c00 6a00 a001 6401 6402  .s,...|.j...d.d.
+00006220: a102 7d01 7402 7c00 6a03 7c00 6a04 7c01  ..}.t.|.j.|.j.|.
+00006230: 6403 7c00 6a05 6404 8d05 7c00 5f06 6400  d.|.j.d...|._.d.
+00006240: 5300 2905 4e72 3100 0000 e906 0000 00e9  S.).Nr1.........
+00006250: 0a00 0000 2903 7231 0000 0072 3000 0000  ....).r1...r0...
+00006260: 727c 0000 0029 0772 2000 0000 7221 0000  r|...).r ...r!..
+00006270: 0072 1500 0000 7245 0000 0072 6d00 0000  .r....rE...rm...
+00006280: 727c 0000 00da 0c74 6578 745f 636f 6e73  r|.....text_cons
+00006290: 6f6c 6529 0272 2900 0000 7231 0000 0072  ole).r)...r1...r
+000062a0: 2e00 0000 722e 0000 0072 2f00 0000 7226  ....r....r/...r&
+000062b0: 0000 003a 0300 0073 0e00 0000 0001 0e02  ...:...s........
+000062c0: 0601 0401 0201 0201 04fc 7a19 4f54 436f  ..........z.OTCo
+000062d0: 6d6d 656e 742e 5f63 7265 6174 655f 7769  mment._create_wi
+000062e0: 6467 6574 7363 0100 0000 0000 0000 0000  dgetsc..........
+000062f0: 0000 0200 0000 0300 0000 4700 0000 7310  ..........G...s.
+00006300: 0000 007c 006a 00a0 0164 01a1 0101 0064  ...|.j...d.....d
+00006310: 0053 0029 024e fa16 3c3c 6269 6e64 5f67  .S.).N..<<bind_g
+00006320: 6c6f 6261 6c5f 7363 726f 6c6c 3e3e a902  lobal_scroll>>..
+00006330: 7245 0000 00da 0e65 7665 6e74 5f67 656e  rE.....event_gen
+00006340: 6572 6174 6572 5a00 0000 722e 0000 0072  eraterZ...r....r
+00006350: 2e00 0000 722f 0000 0072 4101 0000 4303  ....r/...rA...C.
+00006360: 0000 7302 0000 0000 017a 1d4f 5443 6f6d  ..s......z.OTCom
+00006370: 6d65 6e74 2e5f 6269 6e64 5f67 6c6f 6261  ment._bind_globa
+00006380: 6c5f 7363 726f 6c6c 6301 0000 0000 0000  l_scrollc.......
+00006390: 0000 0000 0002 0000 0003 0000 0047 0000  .............G..
+000063a0: 0073 1000 0000 7c00 6a00 a001 6401 a101  .s....|.j...d...
+000063b0: 0100 6400 5300 2902 4efa 183c 3c75 6e62  ..d.S.).N..<<unb
+000063c0: 696e 645f 676c 6f62 616c 5f73 6372 6f6c  ind_global_scrol
+000063d0: 6c3e 3e72 4601 0000 725a 0000 0072 2e00  l>>rF...rZ...r..
+000063e0: 0000 722e 0000 0072 2f00 0000 7240 0100  ..r....r/...r@..
+000063f0: 0046 0300 0073 0200 0000 0001 7a1f 4f54  .F...s......z.OT
+00006400: 436f 6d6d 656e 742e 5f75 6e62 696e 645f  Comment._unbind_
+00006410: 676c 6f62 616c 5f73 6372 6f6c 6c63 0100  global_scrollc..
+00006420: 0000 0000 0000 0000 0000 0100 0000 0200  ................
+00006430: 0000 4300 0000 730e 0000 007c 006a 00a0  ..C...s....|.j..
+00006440: 01a1 00a0 02a1 0053 0072 4c00 0000 2903  .......S.rL...).
+00006450: 726d 0000 0072 2100 0000 da06 7273 7472  rm...r!.....rstr
+00006460: 6970 724d 0000 0072 2e00 0000 722e 0000  iprM...r....r...
+00006470: 0072 2f00 0000 7221 0000 0049 0300 0073  .r/...r!...I...s
+00006480: 0200 0000 0001 7a0d 4f54 436f 6d6d 656e  ......z.OTCommen
+00006490: 742e 6765 7463 0200 0000 0000 0000 0000  t.getc..........
+000064a0: 0000 0200 0000 0300 0000 4300 0000 7310  ..........C...s.
+000064b0: 0000 007c 006a 00a0 017c 01a1 0101 0064  ...|.j...|.....d
+000064c0: 0053 0072 4c00 0000 2902 7244 0100 00da  .S.rL...).rD....
+000064d0: 0873 6574 5f74 6578 7472 7100 0000 722e  .set_textrq...r.
+000064e0: 0000 0072 2e00 0000 722f 0000 0072 5100  ...r....r/...rQ.
+000064f0: 0000 4c03 0000 7302 0000 0000 017a 0d4f  ..L...s......z.O
+00006500: 5443 6f6d 6d65 6e74 2e73 6574 6301 0000  TComment.setc...
+00006510: 0000 0000 0000 0000 0003 0000 0003 0000  ................
+00006520: 0043 0000 0073 5600 0000 7c00 6a00 720a  .C...sV...|.j.r.
+00006530: 6400 5300 7c00 6a01 6401 6b02 7218 6402  d.S.|.j.d.k.r.d.
+00006540: 6e06 7402 6403 1900 7d01 7c00 6a01 6401  n.t.d...}.|.j.d.
+00006550: 6b02 722e 6404 6e06 7402 6405 1900 7d02  k.r.d.n.t.d...}.
+00006560: 7c00 6a03 6a04 7c01 6406 8d01 0100 7c00  |.j.j.|.d.....|.
+00006570: 6a03 6a04 7c02 6407 8d01 0100 6400 5300  j.j.|.d.....d.S.
+00006580: 2908 4e72 3400 0000 7285 0000 0072 8600  ).Nr4...r....r..
+00006590: 0000 7274 0000 0072 8100 0000 7287 0000  ..rt...r....r...
+000065a0: 0029 0172 7800 0000 2905 727c 0000 0072  .).rx...).r|...r
+000065b0: 5700 0000 7211 0000 0072 4401 0000 7284  W...r....rD...r.
+000065c0: 0000 0029 0372 2900 0000 5a07 6267 636f  ...).r)...Z.bgco
+000065d0: 6c6f 725a 0766 6763 6f6c 6f72 722e 0000  lorZ.fgcolorr...
+000065e0: 0072 2e00 0000 722f 0000 0072 5e00 0000  .r....r/...r^...
+000065f0: 4f03 0000 730c 0000 0000 0106 0104 0216  O...s...........
+00006600: 0116 010e 017a 1f4f 5443 6f6d 6d65 6e74  .....z.OTComment
+00006610: 2e5f 7570 6461 7465 5f77 6964 6765 7473  ._update_widgets
+00006620: 5f73 7479 6c65 290c 7263 0000 0072 6400  _style).rc...rd.
+00006630: 0000 7265 0000 0072 1f00 0000 7225 0000  ..re...r....r%..
+00006640: 0072 2600 0000 7241 0100 0072 4001 0000  .r&...rA...r@...
+00006650: 7221 0000 0072 5100 0000 725e 0000 0072  r!...rQ...r^...r
+00006660: 6700 0000 722e 0000 0072 2e00 0000 722c  g...r....r....r,
+00006670: 0000 0072 2f00 0000 723d 0100 0022 0300  ...r/...r=..."..
+00006680: 0073 1000 0000 0802 0c12 0804 0809 0803  .s..............
+00006690: 0803 0803 0803 723d 0100 0063 0000 0000  ......r=...c....
+000066a0: 0000 0000 0000 0000 0000 0000 0200 0000  ................
+000066b0: 4000 0000 7328 0000 0065 005a 0164 005a  @...s(...e.Z.d.Z
+000066c0: 0264 015a 0364 0264 0384 005a 0464 0464  .d.Z.d.d...Z.d.d
+000066d0: 0584 005a 0564 0664 0784 005a 0664 0853  ...Z.d.d...Z.d.S
+000066e0: 0029 09da 074f 5445 6d70 7479 7a22 4f54  .)...OTEmptyz"OT
+000066f0: 2077 6964 6765 7420 666f 7220 756e 696d   widget for unim
+00006700: 706c 656d 656e 7465 6420 7479 7065 732e  plemented types.
+00006710: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
+00006720: 0007 0000 0043 0000 0073 8200 0000 6401  .....C...s....d.
+00006730: 7c00 5f00 7c00 6a01 a002 6402 6400 a102  |._.|.j...d.d...
+00006740: 6403 6b03 721c 6400 5300 6700 7d01 6404  d.k.r.d.S.g.}.d.
+00006750: 4400 5d28 7d02 7c02 7c00 6a01 7600 7224  D.](}.|.|.j.v.r$
+00006760: 7c01 a003 7c02 9b00 6405 7c00 6a01 7c02  |...|...d.|.j.|.
+00006770: 1900 9b00 9d03 a101 0100 7124 7c00 6a04  ..........q$|.j.
+00006780: 6a05 6406 a006 7c01 a101 6407 8d01 0100  j.d...|...d.....
+00006790: 7c00 6a04 6a07 6408 6409 6409 640a 8d03  |.j.j.d.d.d.d...
+000067a0: 0100 7c00 6a08 a009 a100 0100 6400 5300  ..|.j.......d.S.
+000067b0: 290b 4e72 0100 0000 da07 6f74 5f74 7970  ).Nr......ot_typ
+000067c0: 65da 0476 6f69 6429 0472 2200 0000 721a  e..void).r"...r.
+000067d0: 0000 00da 0474 7970 6572 4c01 0000 7a03  .....typerL...z.
+000067e0: 203d 20da 010a a901 723c 0000 0072 3500   = .....r<...r5.
+000067f0: 0000 728a 0000 0029 0372 3700 0000 da04  ..r....).r7.....
+00006800: 7061 6478 da04 7061 6479 290a 7257 0000  padx..pady).rW..
+00006810: 0072 2000 0000 7221 0000 0072 f100 0000  .r ...r!...r....
+00006820: 724a 0000 0072 8400 0000 da04 6a6f 696e  rJ...r......join
+00006830: 7247 0000 0072 4500 0000 da06 666f 7267  rG...rE.....forg
+00006840: 6574 2903 7229 0000 00da 0469 6e66 6fda  et).r).....info.
+00006850: 0469 7465 6d72 2e00 0000 722e 0000 0072  .itemr....r....r
+00006860: 2f00 0000 7226 0000 005c 0300 0073 1400  /...r&...\...s..
+00006870: 0000 0001 0601 1201 0402 0401 0801 0a01  ................
+00006880: 1c02 1401 1202 7a17 4f54 456d 7074 792e  ......z.OTEmpty.
+00006890: 5f63 7265 6174 655f 7769 6467 6574 7363  _create_widgetsc
+000068a0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+000068b0: 0100 0000 4300 0000 7304 0000 0064 0053  ....C...s....d.S
+000068c0: 0072 4c00 0000 722e 0000 0072 4d00 0000  .rL...r....rM...
+000068d0: 722e 0000 0072 2e00 0000 722f 0000 0072  r....r....r/...r
+000068e0: 2100 0000 6b03 0000 7302 0000 0000 017a  !...k...s......z
+000068f0: 0b4f 5445 6d70 7479 2e67 6574 6301 0000  .OTEmpty.getc...
+00006900: 0000 0000 0000 0000 0003 0000 0001 0000  ................
+00006910: 004f 0000 0073 0400 0000 6400 5300 724c  .O...s....d.S.rL
+00006920: 0000 0072 2e00 0000 2903 7229 0000 0072  ...r....).r)...r
+00006930: 5b00 0000 da06 6b77 6172 6773 722e 0000  [.....kwargsr...
+00006940: 0072 2e00 0000 722f 0000 0072 5100 0000  .r....r/...rQ...
+00006950: 6e03 0000 7302 0000 0000 017a 0b4f 5445  n...s......z.OTE
+00006960: 6d70 7479 2e73 6574 4e29 0772 6300 0000  mpty.setN).rc...
+00006970: 7264 0000 0072 6500 0000 7266 0000 0072  rd...re...rf...r
+00006980: 2600 0000 7221 0000 0072 5100 0000 722e  &...r!...rQ...r.
+00006990: 0000 0072 2e00 0000 722e 0000 0072 2f00  ...r....r....r/.
+000069a0: 0000 724b 0100 0059 0300 0073 0800 0000  ..rK...Y...s....
+000069b0: 0801 0402 080f 0803 724b 0100 0063 0000  ........rK...c..
+000069c0: 0000 0000 0000 0000 0000 0000 0000 0300  ................
+000069d0: 0000 4000 0000 7366 0000 0065 005a 0164  ..@...sf...e.Z.d
+000069e0: 005a 0264 015a 0364 0264 0384 005a 0464  .Z.d.Z.d.d...Z.d
+000069f0: 0464 0584 005a 0564 0664 0784 005a 0664  .d...Z.d.d...Z.d
+00006a00: 0864 0984 005a 0765 086a 0964 0a64 0b84  .d...Z.e.j.d.d..
+00006a10: 0083 015a 0a64 0c64 0d84 005a 0b64 0e64  ...Z.d.d...Z.d.d
+00006a20: 0f84 005a 0c64 1064 1184 005a 0d64 1264  ...Z.d.d...Z.d.d
+00006a30: 1384 005a 0e64 1464 1584 005a 0f64 1653  ...Z.d.d...Z.d.S
+00006a40: 0029 17da 0f5f 4f54 4162 7374 7261 6374  .)..._OTAbstract
+00006a50: 4c69 7374 7acd 436c 6173 7320 746f 2068  Listz.Class to h
+00006a60: 616e 646c 6520 4c49 5354 530a 2020 2020  andle LISTS.    
+00006a70: 0a20 2020 2049 6e20 7468 6520 6d65 6d6f  .    In the memo
+00006a80: 7279 2061 206c 6973 7420 6973 2061 2050  ry a list is a P
+00006a90: 7974 686f 6e20 4c69 7374 730a 2020 2020  ython Lists.    
+00006aa0: 4275 7420 666f 7220 7468 6520 4755 492c  But for the GUI,
+00006ab0: 2074 6865 206c 6973 7420 636f 6e74 6169   the list contai
+00006ac0: 6e65 7320 7375 626c 6561 7665 7320 7769  nes subleaves wi
+00006ad0: 7468 2073 7065 6369 6669 6320 6265 6861  th specific beha
+00006ae0: 7669 6f72 0a20 2020 2057 6520 6c6f 6f73  vior.    We loos
+00006af0: 6520 6865 7265 2074 6865 2075 7375 616c  e here the usual
+00006b00: 2070 6572 6665 6374 206d 6170 7069 6e67   perfect mapping
+00006b10: 2062 7477 206d 656d 6f72 7920 616e 6420   btw memory and 
+00006b20: 4755 4963 0100 0000 0000 0000 0000 0000  GUIc............
+00006b30: 0100 0000 0200 0000 4300 0000 730a 0000  ........C...s...
+00006b40: 0067 007c 005f 0064 0053 0072 4c00 0000  .g.|._.d.S.rL...
+00006b50: 724e 0000 0072 4d00 0000 722e 0000 0072  rN...rM...r....r
+00006b60: 2e00 0000 722f 0000 0072 2300 0000 7903  ....r/...r#...y.
+00006b70: 0000 7302 0000 0000 017a 245f 4f54 4162  ..s......z$_OTAb
+00006b80: 7374 7261 6374 4c69 7374 2e5f 696e 6974  stractList._init
+00006b90: 5f70 7265 7669 6f75 735f 7661 6c75 6563  _previous_valuec
+00006ba0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00006bb0: 0600 0000 4300 0000 732e 0000 0074 00a0  ....C...s....t..
+00006bc0: 017c 006a 02a1 017c 005f 037c 006a 036a  .|.j...|._.|.j.j
+00006bd0: 0464 0164 0164 0264 0364 048d 0401 007c  .d.d.d.d.d.....|
+00006be0: 00a0 05a1 0001 0064 0053 0029 054e 723b  .......d.S.).Nr;
+00006bf0: 0000 0072 3e00 0000 72fa 0000 00a9 0472  ...r>...r......r
+00006c00: f700 0000 7241 0000 0072 4200 0000 7243  ....rA...rB...rC
+00006c10: 0000 0029 0672 0200 0000 7244 0000 0072  ...).r....rD...r
+00006c20: 4500 0000 da0f 656e 7472 796c 6973 7468  E.....entrylisth
+00006c30: 6f6c 6465 7272 4b00 0000 da15 5f63 6f6e  olderrK....._con
+00006c40: 6669 6775 7265 5f70 6f70 7570 5f6d 656e  figure_popup_men
+00006c50: 7572 4d00 0000 722e 0000 0072 2e00 0000  urM...r....r....
+00006c60: 722f 0000 0072 2600 0000 7c03 0000 7310  r/...r&...|...s.
+00006c70: 0000 0000 010e 0106 0102 0102 0102 0102  ................
+00006c80: fc06 067a 1f5f 4f54 4162 7374 7261 6374  ...z._OTAbstract
+00006c90: 4c69 7374 2e5f 6372 6561 7465 5f77 6964  List._create_wid
+00006ca0: 6765 7473 6301 0000 0000 0000 0000 0000  getsc...........
+00006cb0: 0005 0000 0006 0000 0043 0000 0073 7400  .........C...st.
+00006cc0: 0000 7c00 6a00 6401 1900 a001 6402 a101  ..|.j.d.....d...
+00006cd0: 7d01 7c00 6a00 6401 1900 a001 6403 6400  }.|.j.d.....d.d.
+00006ce0: a102 7d02 7c02 6400 7500 7242 6404 6405  ..}.|.d.u.rBd.d.
+00006cf0: 6406 6407 9c03 7d03 7c03 7c01 1900 7c02  d.d...}.|.|...|.
+00006d00: 7c01 3c00 7402 6408 7c00 6a00 a001 6409  |.<.t.d.|.j...d.
+00006d10: 6408 a102 8302 7d04 7403 7c04 7c00 6a00  d.....}.t.|.|.j.
+00006d20: a001 640a 6408 a102 8302 7d04 7c02 6701  ..d.d.....}.|.g.
+00006d30: 7c04 1400 5300 290b 4e72 e200 0000 724e  |...S.).Nr....rN
+00006d40: 0100 0072 5300 0000 7254 0000 0072 3e00  ...rS...rT...r>.
+00006d50: 0000 7201 0000 0029 03da 0673 7472 696e  ..r....)...strin
+00006d60: 67da 066e 756d 6265 7272 a000 0000 7234  g..numberr....r4
+00006d70: 0000 00da 086d 6178 4974 656d 73da 086d  .....maxItems..m
+00006d80: 696e 4974 656d 7329 0472 2000 0000 7221  inItems).r ...r!
+00006d90: 0000 00da 036d 696e 72d9 0000 0029 0572  .....minr....).r
+00006da0: 2900 0000 da09 6974 656d 5f74 7970 6572  ).....item_typer
+00006db0: 7200 0000 5a08 7479 7065 3276 616c 5a06  r...Z.type2valZ.
+00006dc0: 6e5f 7265 7073 722e 0000 0072 2e00 0000  n_repsr....r....
+00006dd0: 722f 0000 0072 5200 0000 8603 0000 7316  r/...rR.......s.
+00006de0: 0000 0000 0410 0112 0208 0302 0102 0102  ................
+00006df0: fe06 030c 0314 0114 027a 1c5f 4f54 4162  .........z._OTAb
+00006e00: 7374 7261 6374 4c69 7374 2e5f 6765 745f  stractList._get_
+00006e10: 6465 6661 756c 7463 0100 0000 0000 0000  defaultc........
+00006e20: 0000 0000 0100 0000 0400 0000 4300 0000  ............C...
+00006e30: 733c 0000 0074 007c 006a 0164 0164 028d  s<...t.|.j.d.d..
+00006e40: 027c 005f 027c 00a0 03a1 0001 007c 006a  .|._.|.......|.j
+00006e50: 01a0 0464 037c 006a 05a1 0201 007c 006a  ...d.|.j.....|.j
+00006e60: 01a0 0464 047c 006a 06a1 0201 0064 0053  ...d.|.j.....d.S
+00006e70: 0029 054e 4629 01da 0774 6561 726f 6666  .).NF)...tearoff
+00006e80: 723e 0100 0072 3f01 0000 2907 720b 0000  r>...r?...).r...
+00006e90: 0072 5a01 0000 da0a 706f 7075 705f 6d65  .rZ.....popup_me
+00006ea0: 6e75 da13 5f61 6464 5f70 6f70 7570 5f63  nu.._add_popup_c
+00006eb0: 6f6d 6d61 6e64 7372 2f01 0000 da0f 5f61  ommandsr/....._a
+00006ec0: 6374 6976 6174 655f 706f 7075 70da 115f  ctivate_popup.._
+00006ed0: 6465 6163 7469 7661 7465 5f70 6f70 7570  deactivate_popup
+00006ee0: 724d 0000 0072 2e00 0000 722e 0000 0072  rM...r....r....r
+00006ef0: 2f00 0000 725b 0100 009b 0300 0073 0800  /...r[.......s..
+00006f00: 0000 0001 1002 0802 1001 7a25 5f4f 5441  ..........z%_OTA
+00006f10: 6273 7472 6163 744c 6973 742e 5f63 6f6e  bstractList._con
+00006f20: 6669 6775 7265 5f70 6f70 7570 5f6d 656e  figure_popup_men
+00006f30: 7563 0100 0000 0000 0000 0000 0000 0100  uc..............
+00006f40: 0000 0100 0000 4300 0000 7304 0000 0064  ......C...s....d
+00006f50: 0053 0072 4c00 0000 722e 0000 0072 4d00  .S.rL...r....rM.
+00006f60: 0000 722e 0000 0072 2e00 0000 722f 0000  ..r....r....r/..
+00006f70: 0072 6401 0000 a303 0000 7302 0000 0000  .rd.......s.....
+00006f80: 027a 235f 4f54 4162 7374 7261 6374 4c69  .z#_OTAbstractLi
+00006f90: 7374 2e5f 6164 645f 706f 7075 705f 636f  st._add_popup_co
+00006fa0: 6d6d 616e 6473 6301 0000 0000 0000 0000  mmandsc.........
+00006fb0: 0000 0002 0000 0004 0000 0047 0000 0073  ...........G...s
+00006fc0: 1400 0000 7c00 6a00 a001 6401 7c00 6a02  ....|.j...d.|.j.
+00006fd0: a102 0100 6400 5300 a902 4e7a 0a3c 4275  ....d.S...Nz.<Bu
+00006fe0: 7474 6f6e 2d32 3e29 0372 5a01 0000 da08  tton-2>).rZ.....
+00006ff0: 6269 6e64 5f61 6c6c da0e 6f6e 5f72 6967  bind_all..on_rig
+00007000: 6874 5f63 6c69 636b 725a 0000 0072 2e00  ht_clickrZ...r..
+00007010: 0000 722e 0000 0072 2f00 0000 7265 0100  ..r....r/...re..
+00007020: 00a7 0300 0073 0200 0000 0001 7a1f 5f4f  .....s......z._O
+00007030: 5441 6273 7472 6163 744c 6973 742e 5f61  TAbstractList._a
+00007040: 6374 6976 6174 655f 706f 7075 7063 0100  ctivate_popupc..
+00007050: 0000 0000 0000 0000 0000 0200 0000 0300  ................
+00007060: 0000 4700 0000 7310 0000 007c 006a 00a0  ..G...s....|.j..
+00007070: 0164 01a1 0101 0064 0053 0072 6701 0000  .d.....d.S.rg...
+00007080: 2902 725a 0100 00da 0a75 6e62 696e 645f  ).rZ.....unbind_
+00007090: 616c 6c72 5a00 0000 722e 0000 0072 2e00  allrZ...r....r..
+000070a0: 0000 722f 0000 0072 6601 0000 aa03 0000  ..r/...rf.......
+000070b0: 7302 0000 0000 017a 215f 4f54 4162 7374  s......z!_OTAbst
+000070c0: 7261 6374 4c69 7374 2e5f 6465 6163 7469  ractList._deacti
+000070d0: 7661 7465 5f70 6f70 7570 6302 0000 0000  vate_popupc.....
+000070e0: 0000 0000 0000 0002 0000 0004 0000 0043  ...............C
+000070f0: 0000 0073 1600 0000 7c00 6a00 a001 7c01  ...s....|.j...|.
+00007100: 6a02 7c01 6a03 a102 0100 6400 5300 724c  j.|.j.....d.S.rL
+00007110: 0000 0029 0472 6301 0000 da08 746b 5f70  ...).rc.....tk_p
+00007120: 6f70 7570 da06 785f 726f 6f74 da06 795f  opup..x_root..y_
+00007130: 726f 6f74 723a 0100 0072 2e00 0000 722e  rootr:...r....r.
+00007140: 0000 0072 2f00 0000 7269 0100 00ad 0300  ...r/...ri......
+00007150: 0073 0200 0000 0001 7a1e 5f4f 5441 6273  .s......z._OTAbs
+00007160: 7472 6163 744c 6973 742e 6f6e 5f72 6967  tractList.on_rig
+00007170: 6874 5f63 6c69 636b 6301 0000 0000 0000  ht_clickc.......
+00007180: 0000 0000 0004 0000 0005 0000 0047 0000  .............G..
+00007190: 0073 3800 0000 6401 a000 6402 6403 8400  .s8...d...d.d...
+000071a0: 7c00 a001 a100 4400 8301 a101 7d02 7402  |.....D.....}.t.
+000071b0: 7c00 6a03 8301 7d03 7c03 a004 a100 0100  |.j...}.|.......
+000071c0: 7c03 a005 7c02 a101 0100 6400 5300 2904  |...|.....d.S.).
+000071d0: 4e7a 022c 2063 0100 0000 0000 0000 0000  Nz., c..........
+000071e0: 0000 0200 0000 0400 0000 5300 0000 7314  ..........S...s.
+000071f0: 0000 0067 007c 005d 0c7d 0174 007c 0183  ...g.|.].}.t.|..
+00007200: 0191 0271 0453 0072 2e00 0000 2901 da03  ...q.S.r....)...
+00007210: 7374 72a9 02da 022e 3072 7200 0000 722e  str.....0rr...r.
+00007220: 0000 0072 2e00 0000 722f 0000 00da 0a3c  ...r....r/.....<
+00007230: 6c69 7374 636f 6d70 3eb1 0300 00f3 0000  listcomp>.......
+00007240: 0000 7a2b 5f4f 5441 6273 7472 6163 744c  ..z+_OTAbstractL
+00007250: 6973 742e 6f6e 5f63 6f70 792e 3c6c 6f63  ist.on_copy.<loc
+00007260: 616c 733e 2e3c 6c69 7374 636f 6d70 3e29  als>.<listcomp>)
+00007270: 0672 5301 0000 7221 0000 0072 1700 0000  .rS...r!...r....
+00007280: 7245 0000 00da 0f63 6c69 7062 6f61 7264  rE.....clipboard
+00007290: 5f63 6c65 6172 da10 636c 6970 626f 6172  _clear..clipboar
+000072a0: 645f 6170 7065 6e64 2904 7229 0000 0072  d_append).r)...r
+000072b0: 5b00 0000 5a08 636f 7079 5f73 7472 7217  [...Z.copy_strr.
+000072c0: 0100 0072 2e00 0000 722e 0000 0072 2f00  ...r....r....r/.
+000072d0: 0000 da07 6f6e 5f63 6f70 79b0 0300 0073  ....on_copy....s
+000072e0: 0800 0000 0001 1801 0a01 0801 7a17 5f4f  ............z._O
+000072f0: 5441 6273 7472 6163 744c 6973 742e 6f6e  TAbstractList.on
+00007300: 5f63 6f70 7963 0200 0000 0000 0000 0000  _copyc..........
+00007310: 0000 0200 0000 0300 0000 4300 0000 7316  ..........C...s.
+00007320: 0000 007c 006a 006a 017c 0174 0214 0064  ...|.j.j.|.t...d
+00007330: 018d 0101 0064 0053 0029 024e 728b 0000  .....d.S.).Nr...
+00007340: 0029 0372 4500 0000 7298 0000 0072 1300  .).rE...r....r..
+00007350: 0000 a902 7229 0000 0072 db00 0000 722e  ....r)...r....r.
+00007360: 0000 0072 2e00 0000 722f 0000 00da 0e5f  ...r....r/....._
+00007370: 7265 7369 7a65 5f68 6f6c 6465 72b6 0300  resize_holder...
+00007380: 0073 0200 0000 0001 7a1e 5f4f 5441 6273  .s......z._OTAbs
+00007390: 7472 6163 744c 6973 742e 5f72 6573 697a  tractList._resiz
+000073a0: 655f 686f 6c64 6572 4e29 1072 6300 0000  e_holderN).rc...
+000073b0: 7264 0000 0072 6500 0000 7266 0000 0072  rd...re...rf...r
+000073c0: 2300 0000 7226 0000 0072 5200 0000 725b  #...r&...rR...r[
+000073d0: 0100 0072 bb00 0000 72bc 0000 0072 6401  ...r....r....rd.
+000073e0: 0000 7265 0100 0072 6601 0000 7269 0100  ..re...rf...ri..
+000073f0: 0072 7501 0000 7277 0100 0072 2e00 0000  .ru...rw...r....
+00007400: 722e 0000 0072 2e00 0000 722f 0000 0072  r....r....r/...r
+00007410: 5801 0000 7203 0000 7318 0000 0008 0104  X...r...s.......
+00007420: 0608 0308 0a08 1508 0804 010a 0308 0308  ................
+00007430: 0308 0308 0672 5801 0000 6300 0000 0000  .....rX...c.....
+00007440: 0000 0000 0000 0000 0000 0004 0000 0000  ................
+00007450: 0000 0073 8e00 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
+00007460: 6401 5a03 641f 8700 6601 6403 6404 8409  d.Z.d...f.d.d...
+00007470: 5a04 6405 6406 8400 5a05 6407 6408 8400  Z.d.d...Z.d.d...
+00007480: 5a06 6409 640a 8400 5a07 640b 640c 8400  Z.d.d...Z.d.d...
+00007490: 5a08 640d 640e 8400 5a09 650a 640f 6410  Z.d.d...Z.e.d.d.
+000074a0: 8400 8301 5a0b 6411 6412 8400 5a0c 6413  ....Z.d.d...Z.d.
+000074b0: 6414 8400 5a0d 6415 6416 8400 5a0e 6417  d...Z.d.d...Z.d.
+000074c0: 6418 8400 5a0f 6419 641a 8400 5a10 641b  d...Z.d.d...Z.d.
+000074d0: 641c 8400 5a11 641d 641e 8400 5a12 8700  d...Z.d.d...Z...
+000074e0: 0400 5a13 5300 2920 da0a 5f4c 6973 7445  ..Z.S.) .._ListE
+000074f0: 6e74 7279 7a4f 5468 6520 6465 6661 756c  ntryzOThe defaul
+00007500: 7420 5355 4277 6964 6765 7420 656e 7472  t SUBwidget entr
+00007510: 7920 666f 7220 6c69 7374 730a 2020 2020  y for lists.    
+00007520: 0a20 2020 2054 6869 7320 6973 2070 6163  .    This is pac
+00007530: 6b65 6420 496e 7369 6465 2061 6e20 4f54  ked Inside an OT
+00007540: 4c69 7374 2e4e 6305 0000 0000 0000 0000  List.Nc.........
+00007550: 0000 0005 0000 0006 0000 0003 0000 0073  ...............s
+00007560: 2200 0000 7c04 7c00 5f00 7c03 7c00 5f01  "...|.|._.|.|._.
+00007570: 7402 8300 a003 7c01 7c02 6401 7c03 a104  t.....|.|.d.|...
+00007580: 0100 6401 5300 2902 7a1e 4164 6469 7469  ..d.S.).z.Additi
+00007590: 6f6e 7320 746f 205f 4c65 6166 5769 6467  ons to _LeafWidg
+000075a0: 6574 2069 6e69 7420 4e29 04da 0f5f 7072  et init N)..._pr
+000075b0: 6576 696f 7573 5f76 616c 7565 7245 0000  evious_valuerE..
+000075c0: 0072 1e00 0000 721f 0000 0029 0572 2900  .r....r....).r).
+000075d0: 0000 7220 0000 0072 2a00 0000 da06 686f  ..r ...r*.....ho
+000075e0: 6c64 6572 724f 0000 0072 2c00 0000 722e  lderrO...r,...r.
+000075f0: 0000 0072 2f00 0000 721f 0000 00bf 0300  ...r/...r.......
+00007600: 0073 0600 0000 0002 0601 0601 7a13 5f4c  .s..........z._L
+00007610: 6973 7445 6e74 7279 2e5f 5f69 6e69 745f  istEntry.__init_
+00007620: 5f63 0100 0000 0000 0000 0000 0000 0100  _c..............
+00007630: 0000 0500 0000 4300 0000 7338 0000 0074  ......C...s8...t
+00007640: 006a 017c 006a 027c 006a 0364 0164 028d  .j.|.j.|.j.d.d..
+00007650: 037c 005f 047c 006a 046a 0564 0364 048d  .|._.|.j.j.d.d..
+00007660: 0101 007c 006a 04a0 0664 057c 006a 07a1  ...|.j...d.|.j..
+00007670: 0201 0064 0653 0029 07fa 3d52 4564 6566  ...d.S.)..=REdef
+00007680: 696e 6520 5749 5448 4f55 5420 7265 6361  ine WITHOUT reca
+00007690: 6c6c 696e 6720 5f63 7265 6174 655f 7769  lling _create_wi
+000076a0: 6467 6574 7328 2920 6672 6f6d 204c 6561  dgets() from Lea
+000076b0: 6657 6964 6765 7421 4629 0272 7500 0000  fWidget!F).ru...
+000076c0: 7277 0000 0072 3500 0000 723c 0100 007a  rw...r5...r<...z
+000076d0: 093c 466f 6375 7349 6e3e 4e29 0872 0200  .<FocusIn>N).r..
+000076e0: 0000 7208 0000 0072 4500 0000 726d 0000  ..r....rE...rm..
+000076f0: 00da 0565 6e74 7279 7247 0000 0072 2f01  ...entryrG...r/.
+00007700: 0000 da0e 6f6e 5f65 6e74 7279 5f66 6f63  ....on_entry_foc
+00007710: 7573 724d 0000 0072 2e00 0000 722e 0000  usrM...r....r...
+00007720: 0072 2f00 0000 7226 0000 00c6 0300 0073  .r/...r&.......s
+00007730: 0a00 0000 0003 0c01 02ff 0802 0e02 7a1a  ..............z.
+00007740: 5f4c 6973 7445 6e74 7279 2e5f 6372 6561  _ListEntry._crea
+00007750: 7465 5f77 6964 6765 7473 6301 0000 0000  te_widgetsc.....
+00007760: 0000 0000 0000 0002 0000 0003 0000 0043  ...............C
+00007770: 0000 0073 2400 0000 7c00 6a00 6401 6b02  ...s$...|.j.d.k.
+00007780: 720e 6402 6e02 6403 7d01 7c00 6a01 6a02  r.d.n.d.}.|.j.j.
+00007790: 7c01 6404 8d01 0100 6405 5300 2906 727b  |.d.....d.S.).r{
+000077a0: 0100 0072 3400 0000 7211 0100 0072 1201  ...r4...r....r..
+000077b0: 0000 72c7 0000 004e 2903 7257 0000 0072  ..r....N).rW...r
+000077c0: 7c01 0000 7284 0000 0072 c800 0000 722e  |...r....r....r.
+000077d0: 0000 0072 2e00 0000 722f 0000 0072 5e00  ...r....r/...r^.
+000077e0: 0000 cf03 0000 7304 0000 0000 0312 017a  ......s........z
+000077f0: 205f 4c69 7374 456e 7472 792e 5f75 7064   _ListEntry._upd
+00007800: 6174 655f 7769 6467 6574 735f 7374 796c  ate_widgets_styl
+00007810: 6563 0100 0000 0000 0000 0000 0000 0100  ec..............
+00007820: 0000 0300 0000 4300 0000 7312 0000 0064  ......C...s....d
+00007830: 017c 006a 00a0 01a1 009b 0064 029d 0353  .|.j.......d...S
+00007840: 0072 a900 0000 2902 727c 0100 0072 2100  .r....).r|...r!.
+00007850: 0000 724d 0000 0072 2e00 0000 722e 0000  ..rM...r....r...
+00007860: 0072 2f00 0000 da15 5f67 6574 5f73 7461  .r/....._get_sta
+00007870: 7475 735f 6572 726f 725f 6d73 67d5 0300  tus_error_msg...
+00007880: 0073 0200 0000 0001 7a20 5f4c 6973 7445  .s......z _ListE
+00007890: 6e74 7279 2e5f 6765 745f 7374 6174 7573  ntry._get_status
+000078a0: 5f65 7272 6f72 5f6d 7367 6302 0000 0000  _error_msgc.....
+000078b0: 0000 0000 0000 0002 0000 0004 0000 0043  ...............C
+000078c0: 0000 0073 2a00 0000 7c00 6a00 6401 6b02  ...s*...|.j.d.k.
+000078d0: 721c 7c00 6a01 a002 7c00 a003 a100 a101  r.|.j...|.......
+000078e0: 0100 6e0a 7c00 6a01 a004 a100 0100 6402  ..n.|.j.......d.
+000078f0: 5300 2903 7a7c 4966 2075 7365 7220 666f  S.).z|If user fo
+00007900: 6375 7320 6f6e 2061 2063 656c 6c2c 200a  cus on a cell, .
+00007910: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00007920: 2061 6e64 2063 656c 6c20 6973 2069 6e76   and cell is inv
+00007930: 616c 6964 2c20 7570 6461 7465 204c 6973  alid, update Lis
+00007940: 7420 6572 726f 7220 6d65 7373 6167 650a  t error message.
+00007950: 2020 2020 2020 2020 656c 7365 206d 616b          else mak
+00007960: 6520 6974 2076 6f69 640a 2020 2020 2020  e it void.      
+00007970: 2020 72ba 0000 004e 2905 7257 0000 0072    r....N).rW...r
+00007980: 2a00 0000 72ab 0000 0072 7e01 0000 da14  *...r....r~.....
+00007990: 5f75 7064 6174 655f 7374 6174 7573 5f6c  _update_status_l
+000079a0: 6162 656c 723a 0100 0072 2e00 0000 722e  abelr:...r....r.
+000079b0: 0000 0072 2f00 0000 727d 0100 00d8 0300  ...r/...r}......
+000079c0: 0073 0600 0000 0006 0a01 1202 7a19 5f4c  .s..........z._L
+000079d0: 6973 7445 6e74 7279 2e6f 6e5f 656e 7472  istEntry.on_entr
+000079e0: 795f 666f 6375 7363 0100 0000 0000 0000  y_focusc........
+000079f0: 0000 0000 0200 0000 0100 0000 4700 0000  ............G...
+00007a00: 7304 0000 0064 0153 0029 027a 2452 656d  s....d.S.).z$Rem
+00007a10: 6f76 6520 7468 6520 7573 7561 6c20 6372  ove the usual cr
+00007a20: 6561 7469 6f6e 206f 6620 7769 6467 6574  eation of widget
+00007a30: 734e 722e 0000 0072 5a00 0000 722e 0000  sNr....rZ...r...
+00007a40: 0072 2e00 0000 722f 0000 0072 2400 0000  .r....r/...r$...
+00007a50: e703 0000 7302 0000 0000 027a 265f 4c69  ....s......z&_Li
+00007a60: 7374 456e 7472 792e 5f63 7265 6174 655f  stEntry._create_
+00007a70: 636f 6d6d 6f6e 5f6c 6561 665f 7769 6467  common_leaf_widg
+00007a80: 6574 7363 0100 0000 0000 0000 0000 0000  etsc............
+00007a90: 0100 0000 0200 0000 4300 0000 730a 0000  ........C...s...
+00007aa0: 007c 006a 0064 0119 0053 0029 024e 724e  .|.j.d...S.).NrN
+00007ab0: 0100 0029 0172 2000 0000 724d 0000 0072  ...).r ...rM...r
+00007ac0: 2e00 0000 722e 0000 0072 2f00 0000 7261  ....r....r/...ra
+00007ad0: 0100 00ec 0300 0073 0200 0000 0002 7a14  .......s......z.
+00007ae0: 5f4c 6973 7445 6e74 7279 2e69 7465 6d5f  _ListEntry.item_
+00007af0: 7479 7065 6301 0000 0000 0000 0000 0000  typec...........
+00007b00: 0001 0000 0002 0000 0043 0000 0073 0c00  .........C...s..
+00007b10: 0000 7c00 6a00 7c00 5f01 6400 5300 724c  ..|.j.|._.d.S.rL
+00007b20: 0000 0029 0272 7901 0000 724f 0000 0072  ...).ry...rO...r
+00007b30: 4d00 0000 722e 0000 0072 2e00 0000 722f  M...r....r....r/
+00007b40: 0000 0072 2300 0000 f003 0000 7302 0000  ...r#.......s...
+00007b50: 0000 017a 1f5f 4c69 7374 456e 7472 792e  ...z._ListEntry.
+00007b60: 5f69 6e69 745f 7072 6576 696f 7573 5f76  _init_previous_v
+00007b70: 616c 7565 6302 0000 0000 0000 0000 0000  aluec...........
+00007b80: 0002 0000 0002 0000 0043 0000 0073 3000  .........C...s0.
+00007b90: 0000 7c00 6a00 6401 6b02 7212 7401 7c01  ..|.j.d.k.r.t.|.
+00007ba0: 8301 5300 7c00 6a00 6402 6b02 7224 7402  ..S.|.j.d.k.r$t.
+00007bb0: 7c01 8301 5300 7403 7c01 8301 5300 6403  |...S.t.|...S.d.
+00007bc0: 5300 2904 7a2b 5374 726f 6e67 6c79 2074  S.).z+Strongly t
+00007bd0: 7970 6520 7468 6520 7661 6c75 6520 656e  ype the value en
+00007be0: 7465 7265 6420 6279 2074 6865 2075 7365  tered by the use
+00007bf0: 7272 5d01 0000 72a0 0000 004e 2904 7261  rr]...r....N).ra
+00007c00: 0100 0072 9a00 0000 7249 0000 0072 6e01  ...r....rI...rn.
+00007c10: 0000 7271 0000 0072 2e00 0000 722e 0000  ..rq...r....r...
+00007c20: 0072 2f00 0000 72a3 0000 00f3 0300 0073  .r/...r........s
+00007c30: 0a00 0000 0002 0a01 0801 0a01 0802 7a13  ..............z.
+00007c40: 5f4c 6973 7445 6e74 7279 2e73 7472 3274  _ListEntry.str2t
+00007c50: 7970 6563 0100 0000 0000 0000 0000 0000  ypec............
+00007c60: 0100 0000 0400 0000 4300 0000 731c 0000  ........C...s...
+00007c70: 0074 0083 007c 005f 017c 006a 01a0 0264  .t...|._.|.j...d
+00007c80: 017c 006a 03a1 0201 0064 0053 0072 6a00  .|.j.....d.S.rj.
+00007c90: 0000 726c 0000 0072 4d00 0000 722e 0000  ..rl...rM...r...
+00007ca0: 0072 2e00 0000 722f 0000 0072 2500 0000  .r....r/...r%...
+00007cb0: fc03 0000 7304 0000 0000 0208 017a 165f  ....s........z._
+00007cc0: 4c69 7374 456e 7472 792e 5f64 6566 696e  ListEntry._defin
+00007cd0: 655f 7661 7263 0100 0000 0000 0000 0000  e_varc..........
+00007ce0: 0000 0300 0000 0800 0000 4700 0000 7352  ..........G...sR
+00007cf0: 0000 007a 247c 00a0 00a1 007d 027c 006a  ...z$|.....}.|.j
+00007d00: 017c 026b 0272 1c64 017c 005f 026e 0664  .|.k.r.d.|._.n.d
+00007d10: 027c 005f 0257 006e 2804 0074 0379 4c01  .|._.W.n(..t.yL.
+00007d20: 0001 0001 0064 037c 005f 027c 006a 04a0  .....d.|._.|.j..
+00007d30: 057c 00a0 06a1 00a1 0101 0059 006e 0230  .|.........Y.n.0
+00007d40: 0064 0453 0029 057a 1843 616c 6c62 6163  .d.S.).z.Callbac
+00007d50: 6b20 6966 2076 616c 7565 2063 6861 6e67  k if value chang
+00007d60: 6572 3400 0000 7201 0000 0072 ba00 0000  er4...r....r....
+00007d70: 4e29 0772 2100 0000 724f 0000 0072 5700  N).r!...rO...rW.
+00007d80: 0000 720f 0000 0072 2a00 0000 72ab 0000  ..r....r*...r...
+00007d90: 0072 7e01 0000 2903 7229 0000 0072 5b00  .r~...).r)...r[.
+00007da0: 0000 7272 0000 0072 2e00 0000 722e 0000  ..rr...r....r...
+00007db0: 0072 2f00 0000 725c 0000 0001 0400 0073  .r/...r\.......s
+00007dc0: 1000 0000 0003 0201 0801 0a01 0802 0a02  ................
+00007dd0: 0c01 0601 7a1a 5f4c 6973 7445 6e74 7279  ....z._ListEntry
+00007de0: 2e6f 6e5f 7661 6c75 655f 6368 616e 6765  .on_value_change
+00007df0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00007e00: 0008 0000 0043 0000 0073 3000 0000 7a12  .....C...s0...z.
+00007e10: 7c00 a000 7c00 6a01 a002 a100 a101 5700  |...|.j.......W.
+00007e20: 5300 0400 7403 792a 0100 0100 0100 7404  S...t.y*......t.
+00007e30: 8300 8201 5900 6e02 3000 6401 5300 2902  ....Y.n.0.d.S.).
+00007e40: 7a12 6f70 656e 7465 6120 4745 5420 6d65  z.opentea GET me
+00007e50: 7468 6f64 4e72 a400 0000 724d 0000 0072  thodNr....rM...r
+00007e60: 2e00 0000 722e 0000 0072 2f00 0000 7221  ....r....r/...r!
+00007e70: 0000 0012 0400 0073 0800 0000 0002 0201  .......s........
+00007e80: 1201 0c01 7a0e 5f4c 6973 7445 6e74 7279  ....z._ListEntry
+00007e90: 2e67 6574 6302 0000 0000 0000 0000 0000  .getc...........
+00007ea0: 0002 0000 0008 0000 0043 0000 0073 3400  .........C...s4.
+00007eb0: 0000 7a16 7c00 6a00 a001 7c00 a002 7c01  ..z.|.j...|...|.
+00007ec0: a101 a101 0100 5700 6e18 0400 7403 792e  ......W.n...t.y.
+00007ed0: 0100 0100 0100 7404 8300 8201 5900 6e02  ......t.....Y.n.
+00007ee0: 3000 6401 5300 2902 7a12 6f70 656e 7465  0.d.S.).z.opente
+00007ef0: 6120 5345 5420 6d65 7468 6f64 4e29 0572  a SET methodN).r
+00007f00: 6d00 0000 7251 0000 0072 a300 0000 72a5  m...rQ...r....r.
+00007f10: 0000 0072 1000 0000 7271 0000 0072 2e00  ...r....rq...r..
+00007f20: 0000 722e 0000 0072 2f00 0000 7251 0000  ..r....r/...rQ..
+00007f30: 0019 0400 0073 0800 0000 0003 0201 1601  .....s..........
+00007f40: 0c01 7a0e 5f4c 6973 7445 6e74 7279 2e73  ..z._ListEntry.s
+00007f50: 6574 6301 0000 0000 0000 0000 0000 0001  etc.............
+00007f60: 0000 0003 0000 0043 0000 0073 1800 0000  .......C...s....
+00007f70: 7c00 a000 6401 a101 0100 7c00 6a01 a002  |...d.....|.j...
+00007f80: a100 0100 6400 5300 725d 0000 0029 0372  ....d.S.r]...).r
+00007f90: 6000 0000 727c 0100 0072 6100 0000 724d  `...r|...ra...rM
+00007fa0: 0000 0072 2e00 0000 722e 0000 0072 2f00  ...r....r....r/.
+00007fb0: 0000 7261 0000 0022 0400 0073 0400 0000  ..ra..."...s....
+00007fc0: 0001 0a02 7a12 5f4c 6973 7445 6e74 7279  ....z._ListEntry
+00007fd0: 2e64 6573 7472 6f79 2901 4e29 1472 6300  .destroy).N).rc.
+00007fe0: 0000 7264 0000 0072 6500 0000 7266 0000  ..rd...re...rf..
+00007ff0: 0072 1f00 0000 7226 0000 0072 5e00 0000  .r....r&...r^...
+00008000: 727e 0100 0072 7d01 0000 7224 0000 00da  r~...r}...r$....
+00008010: 0870 726f 7065 7274 7972 6101 0000 7223  .propertyra...r#
+00008020: 0000 0072 a300 0000 7225 0000 0072 5c00  ...r....r%...r\.
+00008030: 0000 7221 0000 0072 5100 0000 7261 0000  ..r!...rQ...ra..
+00008040: 0072 6700 0000 722e 0000 0072 2e00 0000  .rg...r....r....
+00008050: 722c 0000 0072 2f00 0000 7278 0100 00ba  r,...r/...rx....
+00008060: 0300 0073 2000 0000 0801 0404 0e07 0809  ...s ...........
+00008070: 0806 0803 080f 0805 0201 0a03 0803 0809  ................
+00008080: 0805 0811 0807 0809 7278 0100 0063 0000  ........rx...c..
+00008090: 0000 0000 0000 0000 0000 0000 0000 0300  ................
+000080a0: 0000 0000 0000 73f8 0000 0065 005a 0164  ......s....e.Z.d
+000080b0: 005a 0264 015a 0387 0066 0164 0264 0384  .Z.d.Z...f.d.d..
+000080c0: 085a 0487 0066 0164 0464 0584 085a 0565  .Z...f.d.d...Z.e
+000080d0: 0664 0664 0784 0083 015a 0764 0864 0984  .d.d.....Z.d.d..
+000080e0: 005a 0864 0a64 0b84 005a 0964 0c64 0d84  .Z.d.d...Z.d.d..
+000080f0: 005a 0a87 0066 0164 0e64 0f84 085a 0b64  .Z...f.d.d...Z.d
+00008100: 1064 1184 005a 0c64 1264 1384 005a 0d64  .d...Z.d.d...Z.d
+00008110: 1464 1584 005a 0e64 1664 1784 005a 0f64  .d...Z.d.d...Z.d
+00008120: 1864 1984 005a 1064 1a64 1b84 005a 1164  .d...Z.d.d...Z.d
+00008130: 1c64 1d84 005a 1264 1e64 1f84 005a 1364  .d...Z.d.d...Z.d
+00008140: 2064 2184 005a 1464 2264 2384 005a 1564   d!..Z.d"d#..Z.d
+00008150: 2464 2584 005a 1664 3764 2764 2884 015a  $d%..Z.d7d'd(..Z
+00008160: 1764 3864 2964 2a84 015a 1864 2b64 2c84  .d8d)d*..Z.d+d,.
+00008170: 005a 1964 2d64 2e84 005a 1a64 2f64 3084  .Z.d-d...Z.d/d0.
+00008180: 005a 1b64 3164 3284 005a 1c64 3364 3484  .Z.d1d2..Z.d3d4.
+00008190: 005a 1d64 3564 3684 005a 1e87 0004 005a  .Z.d5d6..Z.....Z
+000081a0: 1f53 0029 39da 0d4f 5444 796e 616d 6963  .S.)9..OTDynamic
+000081b0: 4c69 7374 7a1b 4c69 7374 2063 6f6e 7472  Listz.List contr
+000081c0: 6f6c 6c65 6420 6279 2074 6865 2075 7365  olled by the use
+000081d0: 7263 0500 0000 0000 0000 0000 0000 0500  rc..............
+000081e0: 0000 0600 0000 0300 0000 735a 0000 0064  ..........sZ...d
+000081f0: 017c 005f 0064 017c 005f 0164 027c 005f  .|._.d.|._.d.|._
+00008200: 027c 0164 0319 0064 0419 007c 005f 037c  .|.d...d...|._.|
+00008210: 01a0 0464 0574 0564 0683 01a1 027c 005f  ...d.t.d.....|._
+00008220: 067c 01a0 0464 0774 0564 0883 01a1 027c  .|...d.t.d.....|
+00008230: 005f 0774 0883 00a0 097c 017c 027c 037c  ._.t.....|.|.|.|
+00008240: 04a1 0401 0064 0253 0029 097a dc53 7461  .....d.S.).z.Sta
+00008250: 7274 7570 2063 6c61 7373 2e0a 0a20 2020  rtup class...   
+00008260: 2020 2020 2049 6e70 7574 7320 3a0a 2020       Inputs :.  
+00008270: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20        --------. 
+00008280: 2020 2020 2020 2073 6368 656d 6120 3a20         schema : 
+00008290: 6120 7363 6865 6d61 2061 7320 6120 6e65  a schema as a ne
+000082a0: 7374 6564 206f 626a 6563 740a 2020 2020  sted object.    
+000082b0: 2020 2020 7061 7265 6e74 3a20 3f3f 3f0a      parent: ???.
+000082c0: 2020 2020 2020 2020 6e61 6d65 3a20 6e61          name: na
+000082d0: 6d65 2074 6f20 6265 2061 6464 6564 0a20  me to be added. 
+000082e0: 2020 2020 2020 2072 6f6f 745f 6672 616d         root_fram
+000082f0: 6520 3a20 2061 2054 6b20 6f62 6a65 6374  e :  a Tk object
+00008300: 2077 6572 6520 7468 6520 7769 6467 6574   were the widget
+00008310: 2077 696c 6c20 6265 2067 7261 6674 6564   will be grafted
+00008320: 0a20 2020 2020 2020 2072 0100 0000 4e72  .        r....Nr
+00008330: e200 0000 724e 0100 0072 5f01 0000 7a04  ....rN...r_...z.
+00008340: 2d69 6e66 725e 0100 0072 9400 0000 290a  -infr^...r....).
+00008350: da0f 5f73 7461 7475 735f 696e 7661 6c69  .._status_invali
+00008360: 64da 0c5f 7374 6174 7573 5f74 656d 70da  d.._status_temp.
+00008370: 0c65 6d70 7479 5f77 6964 6765 7472 6101  .empty_widgetra.
+00008380: 0000 7221 0000 0072 9a00 0000 da09 6d69  ..r!...r......mi
+00008390: 6e5f 6974 656d 73da 096d 6178 5f69 7465  n_items..max_ite
+000083a0: 6d73 721e 0000 0072 1f00 0000 7228 0000  msr....r....r(..
+000083b0: 0072 2c00 0000 722e 0000 0072 2f00 0000  .r,...r....r/...
+000083c0: 721f 0000 002b 0400 0073 0e00 0000 000a  r....+...s......
+000083d0: 0601 0603 0603 0e02 1201 1202 7a16 4f54  ............z.OT
+000083e0: 4479 6e61 6d69 634c 6973 742e 5f5f 696e  DynamicList.__in
+000083f0: 6974 5f5f 6301 0000 0000 0000 0000 0000  it__c...........
+00008400: 0001 0000 0002 0000 0003 0000 0073 1e00  .............s..
+00008410: 0000 7400 8300 a001 a100 0100 7c00 a002  ..t.........|...
+00008420: a100 0100 7c00 a003 a100 0100 6401 5300  ....|.......d.S.
+00008430: 2902 7a2b 4164 6420 6d6f 7265 2074 6f20  ).z+Add more to 
+00008440: 5f4f 5441 6273 7472 6163 744c 6973 742e  _OTAbstractList.
+00008450: 5f63 7265 6174 655f 7769 6467 6574 734e  _create_widgetsN
+00008460: 2904 721e 0000 0072 2600 0000 7289 0000  ).r....r&...r...
+00008470: 00da 0f5f 636f 6e66 6967 5f62 7574 746f  ..._config_butto
+00008480: 6e73 724d 0000 0072 2c00 0000 722e 0000  nsrM...r,...r...
+00008490: 0072 2f00 0000 7226 0000 0044 0400 0073  .r/...r&...D...s
+000084a0: 0600 0000 0002 0a01 0801 7a1d 4f54 4479  ..........z.OTDy
+000084b0: 6e61 6d69 634c 6973 742e 5f63 7265 6174  namicList._creat
+000084c0: 655f 7769 6467 6574 7363 0100 0000 0000  e_widgetsc......
+000084d0: 0000 0000 0000 0100 0000 0200 0000 4300  ..............C.
+000084e0: 0000 730c 0000 007c 006a 007c 006a 016b  ..s....|.j.|.j.k
+000084f0: 0353 0029 017a 1c54 7275 6520 6966 206c  .S.).z.True if l
+00008500: 6973 7420 6361 6e20 6368 616e 6765 2073  ist can change s
+00008510: 697a 6529 0272 8501 0000 7286 0100 0072  ize).r....r....r
+00008520: 4d00 0000 722e 0000 0072 2e00 0000 722f  M...r....r....r/
+00008530: 0000 00da 0972 6573 697a 6162 6c65 4a04  .....resizableJ.
+00008540: 0000 7302 0000 0000 037a 174f 5444 796e  ..s......z.OTDyn
+00008550: 616d 6963 4c69 7374 2e72 6573 697a 6162  amicList.resizab
+00008560: 6c65 6301 0000 0000 0000 0000 0000 0002  lec.............
+00008570: 0000 0006 0000 0043 0000 0073 3a00 0000  .......C...s:...
+00008580: 7400 6a01 7c00 6a02 6401 6402 6403 6404  t.j.|.j.d.d.d.d.
+00008590: 8d04 7c00 5f03 7c00 6a04 7220 6405 6e02  ..|._.|.j.r d.n.
+000085a0: 6406 7d01 7c00 6a03 6a05 7c01 6406 6407  d.}.|.j.j.|.d.d.
+000085b0: 6408 8d03 0100 6400 5300 2909 4e72 8d00  d.....d.S.).Nr..
+000085c0: 0000 728e 0000 0072 8f00 0000 7290 0000  ..r....r....r...
+000085d0: 0072 a100 0000 727a 0000 0072 8c00 0000  .r....rz...r....
+000085e0: 7240 0000 0029 0672 0200 0000 7248 0000  r@...).r....rH..
+000085f0: 0072 4500 0000 7299 0000 0072 8801 0000  .rE...r....r....
+00008600: 724b 0000 0029 0272 2900 0000 7241 0000  rK...).r)...rA..
+00008610: 0072 2e00 0000 722e 0000 0072 2f00 0000  .r....r....r/...
+00008620: 7289 0000 004f 0400 0073 0c00 0000 0001  r....O...s......
+00008630: 0401 0801 02fe 0803 0e01 7a22 4f54 4479  ..........z"OTDy
+00008640: 6e61 6d69 634c 6973 742e 5f63 6f6e 6669  namicList._confi
+00008650: 675f 7374 6174 7573 5f6c 6162 656c 6301  g_status_labelc.
+00008660: 0000 0000 0000 0000 0000 0001 0000 0006  ................
+00008670: 0000 0043 0000 0073 6200 0000 7c00 6a00  ...C...sb...|.j.
+00008680: 730a 6401 5300 7401 6a02 7c00 6a03 6402  s.d.S.t.j.|.j.d.
+00008690: 7c00 6a04 6403 8d03 7c00 5f05 7401 6a02  |.j.d...|._.t.j.
+000086a0: 7c00 6a03 6404 7c00 6a06 6403 8d03 7c00  |.j.d.|.j.d...|.
+000086b0: 5f07 7c00 6a05 6a08 6405 6406 6407 6408  _.|.j.j.d.d.d.d.
+000086c0: 6409 8d04 0100 7c00 6a07 6a08 6405 640a  d.....|.j.j.d.d.
+000086d0: 6407 6408 6409 8d04 0100 6401 5300 290b  d.d.d.....d.S.).
+000086e0: 7a11 496e 6974 6961 6c69 7365 2065 6e74  z.Initialise ent
+000086f0: 7279 2e4e fa01 2b29 0272 3c00 0000 72c4  ry.N..+).r<...r.
+00008700: 0000 00da 012d 679a 9999 9999 99a9 3f67  .....-g.......?g
+00008710: 6666 6666 6666 ee3f 727a 0000 0072 8c00  ffffff.?rz...r..
+00008720: 0000 7259 0100 0072 3400 0000 2909 7288  ..rY...r4...).r.
+00008730: 0100 0072 0200 0000 7200 0100 0072 4500  ...r....r....rE.
+00008740: 0000 da0b 6f6e 5f61 6464 5f69 7465 6d5a  ....on_add_itemZ
+00008750: 0a61 6464 6974 656d 5f62 74da 0b6f 6e5f  .additem_bt..on_
+00008760: 6465 6c5f 6974 656d 5a0a 6465 6c69 7465  del_itemZ.delite
+00008770: 6d5f 6274 724b 0000 0072 4d00 0000 722e  m_btrK...rM...r.
+00008780: 0000 0072 2e00 0000 722f 0000 0072 8701  ...r....r/...r..
+00008790: 0000 5604 0000 7324 0000 0000 0206 0104  ..V...s$........
+000087a0: 0208 0102 0104 fe08 0308 0102 0104 fe08  ................
+000087b0: 0408 0102 0104 fe06 0308 0102 0104 fe7a  ...............z
+000087c0: 1d4f 5444 796e 616d 6963 4c69 7374 2e5f  .OTDynamicList._
+000087d0: 636f 6e66 6967 5f62 7574 746f 6e73 6301  config_buttonsc.
+000087e0: 0000 0000 0000 0000 0000 0001 0000 0004  ................
+000087f0: 0000 0043 0000 0073 2800 0000 7c00 6a00  ...C...s(...|.j.
+00008800: 6a01 6401 7c00 6a02 6402 8d02 0100 7c00  j.d.|.j.d.....|.
+00008810: 6a00 6a01 6403 7c00 6a03 6402 8d02 0100  j.j.d.|.j.d.....
+00008820: 6404 5300 2905 fa26 5265 2d64 6566 696e  d.S.)..&Re-defin
+00008830: 6520 5f4f 5441 6273 7472 6163 744c 6973  e _OTAbstractLis
+00008840: 7420 766f 6964 206d 6574 686f 6420 da04  t void method ..
+00008850: 436f 7079 a902 da05 6c61 6265 6c72 c400  Copy....labelr..
+00008860: 0000 5a05 5061 7374 654e 2904 7263 0100  ..Z.PasteN).rc..
+00008870: 00da 0b61 6464 5f63 6f6d 6d61 6e64 7275  ...add_commandru
+00008880: 0100 00da 086f 6e5f 7061 7374 6572 4d00  .....on_pasterM.
+00008890: 0000 722e 0000 0072 2e00 0000 722f 0000  ..r....r....r/..
+000088a0: 0072 6401 0000 6904 0000 7304 0000 0000  .rd...i...s.....
+000088b0: 0212 017a 214f 5444 796e 616d 6963 4c69  ...z!OTDynamicLi
+000088c0: 7374 2e5f 6164 645f 706f 7075 705f 636f  st._add_popup_co
+000088d0: 6d6d 616e 6473 6301 0000 0000 0000 0000  mmandsc.........
+000088e0: 0000 0002 0000 0005 0000 0003 0000 0073  ...............s
+000088f0: 3200 0000 7400 6401 6402 7401 7c00 6a02  2...t.d.d.t.|.j.
+00008900: 8301 1700 8302 7d01 7c00 6a03 7222 7c01  ......}.|.j.r"|.
+00008910: 6403 3700 7d01 7404 8300 a005 7c01 a101  d.7.}.t.....|...
+00008920: 0100 6404 5300 2905 7a25 4164 6a75 7374  ..d.S.).z%Adjust
+00008930: 2068 6f6c 6465 7220 7369 7a65 2074 6f20   holder size to 
+00008940: 696e 7465 726e 2076 6172 6961 626c 6572  intern variabler
+00008950: 8a00 0000 7234 0000 0072 3b00 0000 4e29  ....r4...r;...N)
+00008960: 0672 d900 0000 72cf 0000 00da 0976 6172  .r....r......var
+00008970: 6961 626c 6573 7288 0100 0072 1e00 0000  iablesr....r....
+00008980: 7277 0100 0072 7601 0000 722c 0000 0072  rw...rv...r,...r
+00008990: 2e00 0000 722f 0000 0072 7701 0000 6e04  ....r/...rw...n.
+000089a0: 0000 7308 0000 0000 0214 0106 0108 017a  ..s............z
+000089b0: 1c4f 5444 796e 616d 6963 4c69 7374 2e5f  .OTDynamicList._
+000089c0: 7265 7369 7a65 5f68 6f6c 6465 7263 0100  resize_holderc..
+000089d0: 0000 0000 0000 0000 0000 0200 0000 0400  ................
+000089e0: 0000 4300 0000 7334 0000 007c 006a 0064  ..C...s4...|.j.d
+000089f0: 0175 0172 0e64 0153 0074 016a 027c 006a  .u.r.d.S.t.j.|.j
+00008a00: 0364 0264 038d 027d 017c 016a 0464 0464  .d.d...}.|.j.d.d
+00008a10: 058d 0101 007c 017c 005f 0064 0153 0029  .....|.|._.d.S.)
+00008a20: 067a 1741 6464 206e 6577 2065 6e74 7279  .z.Add new entry
+00008a30: 2074 6f20 686f 6c64 6572 4e72 4d01 0000   to holderNrM...
+00008a40: 7250 0100 0072 3500 0000 723c 0100 0029  rP...r5...r<...)
+00008a50: 0572 8401 0000 7202 0000 0072 4800 0000  .r....r....rH...
+00008a60: 725a 0100 0072 4700 0000 2902 7229 0000  rZ...rG...).r)..
+00008a70: 0072 9001 0000 722e 0000 0072 2e00 0000  .r....r....r....
+00008a80: 722f 0000 00da 1163 7265 6174 655f 766f  r/.....create_vo
+00008a90: 6964 5f65 6e74 7279 7504 0000 730a 0000  id_entryu...s...
+00008aa0: 0000 020a 0104 0210 010c 017a 1f4f 5444  ...........z.OTD
+00008ab0: 796e 616d 6963 4c69 7374 2e63 7265 6174  ynamicList.creat
+00008ac0: 655f 766f 6964 5f65 6e74 7279 6301 0000  e_void_entryc...
+00008ad0: 0000 0000 0000 0000 0007 0000 0009 0000  ................
+00008ae0: 0047 0000 0073 cc00 0000 7a12 7400 7c00  .G...s....z.t.|.
+00008af0: 6a01 8301 a002 a100 7d02 5700 6e1a 0400  j.......}.W.n...
+00008b00: 7403 6a04 6a05 792c 0100 0100 0100 6401  t.j.j.y,......d.
+00008b10: 7d02 5900 6e02 3000 7c02 7342 7406 6a07  }.Y.n.0.|.sBt.j.
+00008b20: 6402 6403 8d01 0100 6404 5300 6405 6406  d.d.....d.S.d.d.
+00008b30: 8400 7c02 a008 6407 a101 4400 8301 7d03  ..|...d...D...}.
+00008b40: 7c00 6a09 7266 7c00 6a09 6408 1900 6e0e  |.j.rf|.j.d...n.
+00008b50: 740a 7c00 7c00 6a0b 7c00 6a0c 8303 7d04  t.|.|.j.|.j...}.
+00008b60: 7c03 4400 5d42 7d05 7a0e 7c04 a00d 7c05  |.D.]B}.z.|...|.
+00008b70: a101 0100 5700 717a 0400 740e 79ba 0100  ....W.qz..t.y...
+00008b80: 0100 0100 6409 7c02 9b00 640a 9d03 7d06  ....d.|...d...}.
+00008b90: 7406 6a07 7c06 6403 8d01 0100 5900 0100  t.j.|.d.....Y...
+00008ba0: 6404 5300 3000 717a 7c00 a00f 7c03 a101  d.S.0.qz|...|...
+00008bb0: 0100 6404 5300 290b 7a11 4361 6c6c 6261  ..d.S.).z.Callba
+00008bc0: 636b 206f 6e20 7061 7374 6572 5400 0000  ck on pasterT...
+00008bd0: 7a10 4e6f 7468 696e 6720 746f 2070 6173  z.Nothing to pas
+00008be0: 7465 2901 da07 6d65 7373 6167 654e 6301  te)...messageNc.
+00008bf0: 0000 0000 0000 0000 0000 0002 0000 0004  ................
+00008c00: 0000 0053 0000 0073 1400 0000 6700 7c00  ...S...s....g.|.
+00008c10: 5d0c 7d01 7c01 a000 a100 9102 7104 5300  ].}.|.......q.S.
+00008c20: 722e 0000 0029 01da 0573 7472 6970 726f  r....)...stripro
+00008c30: 0100 0072 2e00 0000 722e 0000 0072 2f00  ...r....r....r/.
+00008c40: 0000 7271 0100 008a 0400 0072 7201 0000  ..rq.......rr...
+00008c50: 7a2a 4f54 4479 6e61 6d69 634c 6973 742e  z*OTDynamicList.
+00008c60: 6f6e 5f70 6173 7465 2e3c 6c6f 6361 6c73  on_paste.<locals
+00008c70: 3e2e 3c6c 6973 7463 6f6d 703e fa01 2c72  >.<listcomp>..,r
+00008c80: 0100 0000 7a14 496e 7661 6c69 6420 636c  ....z.Invalid cl
+00008c90: 6970 626f 6172 643a 0a27 fa01 2729 1072  ipboard:.'..').r
+00008ca0: 1700 0000 7245 0000 00da 0d63 6c69 7062  ....rE.....clipb
+00008cb0: 6f61 7264 5f67 6574 da07 746b 696e 7465  oard_get..tkinte
+00008cc0: 72da 085f 746b 696e 7465 72da 0854 636c  r.._tkinter..Tcl
+00008cd0: 4572 726f 7272 0c00 0000 da0b 7368 6f77  Errorr......show
+00008ce0: 7761 726e 696e 67da 0573 706c 6974 7293  warning..splitr.
+00008cf0: 0100 0072 7801 0000 725a 0100 0072 6101  ...rx...rZ...ra.
+00008d00: 0000 72a3 0000 0072 a500 0000 7251 0000  ..r....r....rQ..
+00008d10: 0029 0772 2900 0000 725b 0000 005a 0970  .).r)...r[...Z.p
+00008d20: 6173 7465 5f73 7472 5a08 7061 7374 655f  aste_strZ.paste_
+00008d30: 6c73 da03 7661 7272 7200 0000 7295 0100  ls..varrr...r...
+00008d40: 0072 2e00 0000 722e 0000 0072 2f00 0000  .r....r....r/...
+00008d50: 7292 0100 007f 0400 0073 2600 0000 0002  r........s&.....
+00008d60: 0201 1201 1001 0a02 0401 0c01 0402 1404  ................
+00008d70: 1201 0aff 0402 0801 0201 0e01 0c01 0c01  ................
+00008d80: 0c01 0c03 7a16 4f54 4479 6e61 6d69 634c  ....z.OTDynamicL
+00008d90: 6973 742e 6f6e 5f70 6173 7465 6301 0000  ist.on_pastec...
+00008da0: 0000 0000 0000 0000 0001 0000 0002 0000  ................
+00008db0: 0043 0000 0073 2000 0000 7400 7c00 6a01  .C...s ...t.|.j.
+00008dc0: 8301 7c00 6a02 6b02 7214 6401 5300 7c00  ..|.j.k.r.d.S.|.
+00008dd0: a003 a100 0100 6401 5300 2902 7a36 6361  ......d.S.).z6ca
+00008de0: 6c6c 6261 636b 2041 6464 2061 6e20 6974  llback Add an it
+00008df0: 656d 2061 7420 7468 6520 656e 6420 6f66  em at the end of
+00008e00: 2074 6865 2061 7272 6179 2e0a 2020 2020   the array..    
+00008e10: 2020 2020 4e29 0472 cf00 0000 7293 0100      N).r....r...
+00008e20: 0072 8601 0000 da09 5f61 6464 5f69 7465  .r......_add_ite
+00008e30: 6d72 4d00 0000 722e 0000 0072 2e00 0000  mrM...r....r....
+00008e40: 722f 0000 0072 8b01 0000 9b04 0000 7306  r/...r........s.
+00008e50: 0000 0000 0410 0104 027a 194f 5444 796e  .........z.OTDyn
+00008e60: 616d 6963 4c69 7374 2e6f 6e5f 6164 645f  amicList.on_add_
+00008e70: 6974 656d 6301 0000 0000 0000 0000 0000  itemc...........
+00008e80: 0001 0000 0003 0000 0043 0000 0073 2200  .........C...s".
+00008e90: 0000 7400 7c00 6a01 8301 7c00 6a02 6b02  ..t.|.j...|.j.k.
+00008ea0: 7214 6401 5300 7c00 a003 6402 a101 0100  r.d.S.|...d.....
+00008eb0: 6401 5300 2903 7a36 4361 6c6c 6261 636b  d.S.).z6Callback
+00008ec0: 2044 656c 6574 6520 6974 656d 2061 7420   Delete item at 
+00008ed0: 7468 6520 656e 6420 6f66 2074 6865 2061  the end of the a
+00008ee0: 7272 6179 2e0a 2020 2020 2020 2020 4e72  rray..        Nr
+00008ef0: 3400 0000 2904 72cf 0000 0072 9301 0000  4...).r....r....
+00008f00: 7285 0100 00da 0c72 656d 6f76 655f 6974  r......remove_it
+00008f10: 656d 7372 4d00 0000 722e 0000 0072 2e00  emsrM...r....r..
+00008f20: 0000 722f 0000 0072 8c01 0000 a404 0000  ..r/...r........
+00008f30: 7306 0000 0000 0310 0104 027a 194f 5444  s..........z.OTD
+00008f40: 796e 616d 6963 4c69 7374 2e6f 6e5f 6465  ynamicList.on_de
+00008f50: 6c5f 6974 656d 6302 0000 0000 0000 0000  l_itemc.........
+00008f60: 0000 0002 0000 0004 0000 0043 0000 0073  ...........C...s
+00008f70: 1800 0000 7c00 6a00 6a01 7c01 7402 6401  ....|.j.j.|.t.d.
+00008f80: 1900 6402 8d02 0100 6400 5300 2903 4e72  ..d.....d.S.).Nr
+00008f90: b900 0000 729d 0000 0029 0372 9900 0000  ....r....).r....
+00008fa0: 7298 0000 0072 1400 0000 72ac 0000 0072  r....r....r....r
+00008fb0: 2e00 0000 722e 0000 0072 2f00 0000 72ab  ....r....r/...r.
+00008fc0: 0000 00ac 0400 0073 0800 0000 0001 0601  .......s........
+00008fd0: 0201 06fe 7a2a 4f54 4479 6e61 6d69 634c  ....z*OTDynamicL
+00008fe0: 6973 742e 5f75 7064 6174 655f 696e 7661  ist._update_inva
+00008ff0: 6c69 645f 7374 6174 7573 5f6c 6162 656c  lid_status_label
+00009000: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
+00009010: 0004 0000 0043 0000 0073 3c00 0000 7c00  .....C...s<...|.
+00009020: a000 a100 7d01 7c01 6401 6b02 7222 7c00  ....}.|.d.k.r"|.
+00009030: 6a01 6a02 6402 6402 6403 8d02 0100 6e16  j.j.d.d.d.....n.
+00009040: 6404 7c01 9b00 6405 9d03 7d02 7c00 a003  d.|...d...}.|...
+00009050: 7c02 a101 0100 6400 5300 2906 4e72 0100  |.....d.S.).Nr..
+00009060: 0000 7254 0000 0072 9d00 0000 7a09 436f  ..rT...r....z.Co
+00009070: 6e74 6169 6e73 207a 1120 696e 7661 6c69  ntains z. invali
+00009080: 6420 696e 7075 7428 7329 2904 da15 5f67  d input(s))..._g
+00009090: 6574 5f6e 756d 6265 725f 6f66 5f65 7272  et_number_of_err
+000090a0: 6f72 7372 9900 0000 7298 0000 0072 ab00  orsr....r....r..
+000090b0: 0000 2903 7229 0000 005a 056e 5f65 7272  ..).r)...Z.n_err
+000090c0: 72ad 0000 0072 2e00 0000 722e 0000 0072  r....r....r....r
+000090d0: 2f00 0000 727f 0100 00b1 0400 0073 0a00  /...r........s..
+000090e0: 0000 0001 0801 0801 1202 0c01 7a22 4f54  ............z"OT
+000090f0: 4479 6e61 6d69 634c 6973 742e 5f75 7064  DynamicList._upd
+00009100: 6174 655f 7374 6174 7573 5f6c 6162 656c  ate_status_label
+00009110: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00009120: 0002 0000 0043 0000 0073 0a00 0000 6700  .....C...s....g.
+00009130: 7c00 5f00 6400 5300 724c 0000 00a9 0172  |._.d.S.rL.....r
+00009140: 9301 0000 724d 0000 0072 2e00 0000 722e  ....rM...r....r.
+00009150: 0000 0072 2f00 0000 7225 0000 00bb 0400  ...r/...r%......
+00009160: 0073 0200 0000 0001 7a19 4f54 4479 6e61  .s......z.OTDyna
+00009170: 6d69 634c 6973 742e 5f64 6566 696e 655f  micList._define_
+00009180: 7661 7263 0100 0000 0000 0000 0000 0000  varc............
+00009190: 0100 0000 0200 0000 4300 0000 7320 0000  ........C...s ..
+000091a0: 007c 006a 0072 0a64 0153 007c 006a 0173  .|.j.r.d.S.|.j.s
+000091b0: 187c 00a0 02a1 0073 1c64 0253 0064 0353  .|.....s.d.S.d.S
+000091c0: 0029 047a 1052 6574 7572 6e20 7374 6174  .).z.Return stat
+000091d0: 7573 2049 4472 ba00 0000 7201 0000 0072  us IDr....r....r
+000091e0: 3400 0000 2903 7282 0100 0072 8301 0000  4...).r....r....
+000091f0: da15 5f63 6865 636b 5f70 7265 7669 6f75  .._check_previou
+00009200: 735f 7661 6c75 6572 4d00 0000 722e 0000  s_valuerM...r...
+00009210: 0072 2e00 0000 722f 0000 00da 0b5f 6765  .r....r/....._ge
+00009220: 745f 7374 6174 7573 be04 0000 730a 0000  t_status....s...
+00009230: 0000 0206 0104 020e 0104 027a 194f 5444  ...........z.OTD
+00009240: 796e 616d 6963 4c69 7374 2e5f 6765 745f  ynamicList._get_
+00009250: 7374 6174 7573 6301 0000 0000 0000 0000  statusc.........
+00009260: 0000 0004 0000 0003 0000 0043 0000 0073  ...........C...s
+00009270: 4600 0000 7c00 a000 a100 7d01 7401 7c00  F...|.....}.t.|.
+00009280: 6a02 8301 7401 7c01 8301 6b03 721e 6401  j...t.|...k.r.d.
+00009290: 5300 7403 7c00 6a02 7c01 8302 4400 5d16  S.t.|.j.|...D.].
+000092a0: 5c02 7d02 7d03 7c02 7c03 6b03 722a 0100  \.}.}.|.|.k.r*..
+000092b0: 6401 5300 712a 6402 5300 2903 7a34 2054  d.S.q*d.S.).z4 T
+000092c0: 7275 6520 6966 2063 6f6e 7465 6e74 206f  rue if content o
+000092d0: 6620 6d65 6d6f 7279 2065 7175 616c 7320  f memory equals 
+000092e0: 746f 2070 7265 7669 6f75 7320 7661 6c75  to previous valu
+000092f0: 6573 4654 2904 7221 0000 0072 cf00 0000  esFT).r!...r....
+00009300: 724f 0000 0072 b500 0000 2904 7229 0000  rO...r....).r)..
+00009310: 0072 e400 0000 72e3 0000 005a 0763 6d70  .r....r....Z.cmp
+00009320: 5f76 616c 722e 0000 0072 2e00 0000 722f  _valr....r....r/
+00009330: 0000 0072 a401 0000 c804 0000 730e 0000  ...r........s...
+00009340: 0000 0208 0212 0104 0214 0108 0108 027a  ...............z
+00009350: 234f 5444 796e 616d 6963 4c69 7374 2e5f  #OTDynamicList._
+00009360: 6368 6563 6b5f 7072 6576 696f 7573 5f76  check_previous_v
+00009370: 616c 7565 6301 0000 0000 0000 0000 0000  aluec...........
+00009380: 0001 0000 0002 0000 0043 0000 0073 2200  .........C...s".
+00009390: 0000 7c00 6a00 6401 7500 720e 6401 5300  ..|.j.d.u.r.d.S.
+000093a0: 7c00 6a00 a001 a100 0100 6401 7c00 5f00  |.j.......d.|._.
+000093b0: 6401 5300 2902 7a13 5265 6d6f 7665 2065  d.S.).z.Remove e
+000093c0: 6d70 7479 2077 6964 6765 744e 2902 7284  mpty widgetN).r.
+000093d0: 0100 0072 6100 0000 724d 0000 0072 2e00  ...ra...rM...r..
+000093e0: 0000 722e 0000 0072 2f00 0000 da12 636c  ..r....r/.....cl
+000093f0: 6561 725f 656d 7074 795f 7769 6467 6574  ear_empty_widget
+00009400: d604 0000 7308 0000 0000 020a 0104 020a  ....s...........
+00009410: 017a 204f 5444 796e 616d 6963 4c69 7374  .z OTDynamicList
+00009420: 2e63 6c65 6172 5f65 6d70 7479 5f77 6964  .clear_empty_wid
+00009430: 6765 7463 0200 0000 0000 0000 0000 0000  getc............
+00009440: 0200 0000 0800 0000 4300 0000 7326 0000  ........C...s&..
+00009450: 007a 0c7c 006a 007c 0119 0057 0053 0004  .z.|.j.|...W.S..
+00009460: 0074 0179 2001 0001 0001 0059 0064 0153  .t.y ......Y.d.S
+00009470: 0030 0064 0153 0029 027a 2752 6574 7572  .0.d.S.).z'Retur
+00009480: 6e20 7072 6576 696f 7573 2076 616c 7565  n previous value
+00009490: 206f 6620 6f6e 6520 6c69 7374 2065 6e74   of one list ent
+000094a0: 7279 4e29 0272 4f00 0000 da0a 496e 6465  ryN).rO.....Inde
+000094b0: 7845 7272 6f72 2902 7229 0000 00da 0569  xError).r).....i
+000094c0: 6e64 6578 722e 0000 0072 2e00 0000 722f  ndexr....r....r/
+000094d0: 0000 00da 185f 6765 745f 7072 6576 696f  ....._get_previo
+000094e0: 7573 5f69 7465 6d5f 7661 6c75 65de 0400  us_item_value...
+000094f0: 0073 0800 0000 0002 0201 0c01 0c01 7a26  .s............z&
+00009500: 4f54 4479 6e61 6d69 634c 6973 742e 5f67  OTDynamicList._g
+00009510: 6574 5f70 7265 7669 6f75 735f 6974 656d  et_previous_item
+00009520: 5f76 616c 7565 4e63 0200 0000 0000 0000  _valueNc........
+00009530: 0000 0000 0400 0000 0500 0000 4300 0000  ............C...
+00009540: 734c 0000 007c 00a0 0074 017c 006a 0283  sL...|...t.|.j..
+00009550: 01a1 017d 0274 037c 006a 0464 0119 007c  ...}.t.|.j.d...|
+00009560: 007c 006a 057c 0283 047d 037c 0164 0275  .|.j.|...}.|.d.u
+00009570: 0172 387c 03a0 067c 01a1 0101 007c 00a0  .r8|...|.....|..
+00009580: 07a1 0001 007c 00a0 08a1 0001 0064 0253  .....|.......d.S
+00009590: 0029 037a 1641 6464 2061 6e20 6974 656d  .).z.Add an item
+000095a0: 2069 6e74 6572 6e61 6c6c 7972 e200 0000   internallyr....
+000095b0: 4e29 0972 a901 0000 72cf 0000 0072 9301  N).r....r....r..
+000095c0: 0000 7278 0100 0072 2000 0000 725a 0100  ..rx...r ...rZ..
+000095d0: 0072 5100 0000 72a6 0100 0072 7701 0000  .rQ...r....rw...
+000095e0: 2904 7229 0000 0072 7200 0000 724f 0000  ).r)...rr...rO..
+000095f0: 005a 096e 6577 5f65 6e74 7279 722e 0000  .Z.new_entryr...
+00009600: 0072 2e00 0000 722f 0000 0072 a001 0000  .r....r/...r....
+00009610: e504 0000 7310 0000 0000 0410 0110 0102  ....s...........
+00009620: ff04 0208 010a 0208 017a 174f 5444 796e  .........z.OTDyn
+00009630: 616d 6963 4c69 7374 2e5f 6164 645f 6974  amicList._add_it
+00009640: 656d 6302 0000 0000 0000 0000 0000 0004  emc.............
+00009650: 0000 0002 0000 0043 0000 0073 6600 0000  .......C...sf...
+00009660: 7c00 6a00 730a 6401 5300 7c01 6401 7500  |.j.s.d.S.|.d.u.
+00009670: 721c 7401 7c00 6a00 8301 7d01 6402 7d02  r.t.|.j...}.d.}.
+00009680: 7c02 7c01 6b00 7244 7c00 6a00 a002 a100  |.|.k.rD|.j.....
+00009690: 7d03 7c03 a003 a100 0100 7c02 6403 3700  }.|.......|.d.7.
+000096a0: 7d02 7120 7c00 a004 a100 0100 7401 7c00  }.q |.......t.|.
+000096b0: 6a00 8301 6402 6b02 7262 7c00 a005 a100  j...d.k.rb|.....
+000096c0: 0100 6401 5300 2904 7a43 4465 6c65 7465  ..d.S.).zCDelete
+000096d0: 2073 6f6d 6520 6974 656d 730a 2020 2020   some items.    
+000096e0: 2020 2020 0a20 2020 2020 2020 2064 656c      .        del
+000096f0: 2061 6c6c 2069 7465 6d73 2069 6620 6e5f   all items if n_
+00009700: 6974 656d 7320 6973 204e 6f6e 654e 7201  items is NoneNr.
+00009710: 0000 0072 3400 0000 2906 7293 0100 0072  ...r4...).r....r
+00009720: cf00 0000 da03 706f 7072 6100 0000 7277  ......popra...rw
+00009730: 0100 0072 9401 0000 2904 7229 0000 005a  ...r....).r)...Z
+00009740: 076e 5f69 7465 6d73 da01 6972 9f01 0000  .n_items..ir....
+00009750: 722e 0000 0072 2e00 0000 722f 0000 0072  r....r....r/...r
+00009760: a101 0000 f204 0000 7318 0000 0000 0506  ........s.......
+00009770: 0104 0208 010a 0204 0108 010a 0108 010a  ................
+00009780: 0208 020e 017a 1a4f 5444 796e 616d 6963  .....z.OTDynamic
+00009790: 4c69 7374 2e72 656d 6f76 655f 6974 656d  List.remove_item
+000097a0: 7363 0100 0000 0000 0000 0000 0000 0100  sc..............
+000097b0: 0000 0100 0000 4300 0000 7306 0000 007c  ......C...s....|
+000097c0: 006a 0053 0029 017a 2148 656d 2c20 7265  .j.S.).z!Hem, re
+000097d0: 6d6f 7665 5f69 7465 6d73 2069 7320 6e62  move_items is nb
+000097e0: 206f 6620 6572 726f 7273 2901 7282 0100   of errors).r...
+000097f0: 0072 4d00 0000 722e 0000 0072 2e00 0000  .rM...r....r....
+00009800: 722f 0000 0072 a201 0000 0805 0000 7302  r/...r........s.
+00009810: 0000 0000 027a 234f 5444 796e 616d 6963  .....z#OTDynamic
+00009820: 4c69 7374 2e5f 6765 745f 6e75 6d62 6572  List._get_number
+00009830: 5f6f 665f 6572 726f 7273 6301 0000 0000  _of_errorsc.....
+00009840: 0000 0000 0000 0001 0000 0004 0000 0043  ...............C
+00009850: 0000 0073 2400 0000 7c00 a000 a100 0100  ...s$...|.......
+00009860: 7c00 6a01 6401 6b03 7220 7c00 a002 7c00  |.j.d.k.r |...|.
+00009870: a003 a100 a101 0100 6402 5300 a903 7a52  ........d.S...zR
+00009880: 4361 6c6c 6261 636b 2069 6620 7374 6174  Callback if stat
+00009890: 7573 2069 7320 7570 6461 7465 640a 2020  us is updated.  
+000098a0: 2020 2020 2020 0a20 2020 2020 2020 2057        .        W
+000098b0: 4152 4e49 4e47 3a20 7472 6967 6765 7220  ARNING: trigger 
+000098c0: 6465 7070 656e 6465 6e63 7920 7365 7474  deppendency sett
+000098d0: 6572 72ba 0000 004e 2904 727f 0100 0072  err....N).r....r
+000098e0: 5700 0000 72a7 0000 0072 2100 0000 724d  W...r....r!...rM
+000098f0: 0000 0072 2e00 0000 722e 0000 0072 2f00  ...r....r....r/.
+00009900: 0000 725f 0000 000c 0500 0073 0600 0000  ..r_.......s....
+00009910: 0004 0802 0a01 7a1e 4f54 4479 6e61 6d69  ......z.OTDynami
+00009920: 634c 6973 742e 6f6e 5f75 7064 6174 655f  cList.on_update_
+00009930: 7374 6174 7573 6302 0000 0000 0000 0000  statusc.........
+00009940: 0000 0002 0000 0003 0000 0043 0000 0073  ...........C...s
+00009950: 1000 0000 7c00 6a00 a001 7c01 a101 0100  ....|.j...|.....
+00009960: 6401 5300 2902 7a11 4e65 7720 6368 696c  d.S.).z.New chil
+00009970: 6420 746f 206c 6973 744e 2902 7293 0100  d to listN).r...
+00009980: 0072 f100 0000 2902 7229 0000 00da 0563  .r....).r).....c
+00009990: 6869 6c64 722e 0000 0072 2e00 0000 722f  hildr....r....r/
+000099a0: 0000 00da 0961 6464 5f63 6869 6c64 1505  .....add_child..
+000099b0: 0000 7302 0000 0000 027a 174f 5444 796e  ..s......z.OTDyn
+000099c0: 616d 6963 4c69 7374 2e61 6464 5f63 6869  amicList.add_chi
+000099d0: 6c64 6302 0000 0000 0000 0000 0000 0009  ldc.............
+000099e0: 0000 0005 0000 0043 0000 0073 b800 0000  .......C...s....
+000099f0: 7400 7c01 8301 7d02 7c02 7c00 6a01 6b00  t.|...}.|.|.j.k.
+00009a00: 7232 7402 7c00 6a01 7c02 1800 8301 4400  r2t.|.j.|.....D.
+00009a10: 5d0e 7d03 7c01 a003 6401 a101 0100 7120  ].}.|...d.....q 
+00009a20: 6e18 7c02 7c00 6a04 6b04 724a 7c01 6401  n.|.|.j.k.rJ|.d.
+00009a30: 7c00 6a04 8502 1900 7d01 7400 7c01 8301  |.j.....}.t.|...
+00009a40: 7d02 7400 7c00 6a05 8301 7d04 7c04 7c02  }.t.|.j...}.|.|.
+00009a50: 6b04 7276 7c04 7c02 1800 7d05 7c00 a006  k.rv|.|...}.|...
+00009a60: 7c05 a101 0100 7407 7c00 6a05 7c01 8302  |.....t.|.j.|...
+00009a70: 4400 5d12 5c02 7d06 7d07 7c06 a008 7c07  D.].\.}.}.|...|.
+00009a80: a101 0100 7182 7402 7c04 7c02 8302 4400  ....q.t.|.|...D.
+00009a90: 5d12 7d08 7c00 a009 7c01 7c08 1900 a101  ].}.|...|.|.....
+00009aa0: 0100 71a0 6401 5300 2902 7a12 4f70 656e  ..q.d.S.).z.Open
+00009ab0: 7465 6120 5345 5420 6d65 7468 6f64 4e29  tea SET methodN)
+00009ac0: 0a72 cf00 0000 7285 0100 00da 0572 616e  .r....r......ran
+00009ad0: 6765 72f1 0000 0072 8601 0000 7293 0100  ger....r....r...
+00009ae0: 0072 a101 0000 72b5 0000 0072 5100 0000  .r....r....rQ...
+00009af0: 72a0 0100 0029 0972 2900 0000 72e4 0000  r....).r)...r...
+00009b00: 005a 0b6e 5f73 6574 5f65 6c65 6d73 da01  .Z.n_set_elems..
+00009b10: 5fda 066e 5f76 6172 735a 056e 5f64 656c  _..n_varsZ.n_del
+00009b20: 72c3 0000 0072 7200 0000 72ab 0100 0072  r....rr...r....r
+00009b30: 2e00 0000 722e 0000 0072 2f00 0000 7251  ....r....r/...rQ
+00009b40: 0000 001a 0500 0073 1e00 0000 0002 0801  .......s........
+00009b50: 0a01 1201 0e02 0a01 0e02 0801 0a08 0801  ................
+00009b60: 0801 0a03 1401 0c03 0e01 7a11 4f54 4479  ..........z.OTDy
+00009b70: 6e61 6d69 634c 6973 742e 7365 7463 0100  namicList.setc..
+00009b80: 0000 0000 0000 0000 0000 0100 0000 0200  ................
+00009b90: 0000 4300 0000 7310 0000 0064 0164 0284  ..C...s....d.d..
+00009ba0: 007c 006a 0044 0083 0153 0029 03fa 124f  .|.j.D...S.)...O
+00009bb0: 7065 6e74 6561 2047 4554 206d 6574 686f  pentea GET metho
+00009bc0: 6463 0100 0000 0000 0000 0000 0000 0200  dc..............
+00009bd0: 0000 0400 0000 5300 0000 7314 0000 0067  ......S...s....g
+00009be0: 007c 005d 0c7d 017c 01a0 00a1 0091 0271  .|.].}.|.......q
+00009bf0: 0453 0072 2e00 0000 2901 7221 0000 0029  .S.r....).r!...)
+00009c00: 0272 7001 0000 729f 0100 0072 2e00 0000  .rp...r....r....
+00009c10: 722e 0000 0072 2f00 0000 7271 0100 003c  r....r/...rq...<
+00009c20: 0500 0072 7201 0000 7a25 4f54 4479 6e61  ...rr...z%OTDyna
+00009c30: 6d69 634c 6973 742e 6765 742e 3c6c 6f63  micList.get.<loc
+00009c40: 616c 733e 2e3c 6c69 7374 636f 6d70 3e72  als>.<listcomp>r
+00009c50: a301 0000 724d 0000 0072 2e00 0000 722e  ....rM...r....r.
+00009c60: 0000 0072 2f00 0000 7221 0000 0039 0500  ...r/...r!...9..
+00009c70: 0073 0200 0000 0003 7a11 4f54 4479 6e61  .s......z.OTDyna
+00009c80: 6d69 634c 6973 742e 6765 7463 0100 0000  micList.getc....
+00009c90: 0000 0000 0000 0000 0200 0000 0300 0000  ................
+00009ca0: 4300 0000 7336 0000 007c 006a 0064 016b  C...s6...|.j.d.k
+00009cb0: 0372 0e64 0253 007c 00a0 01a1 007c 005f  .r.d.S.|.....|._
+00009cc0: 027c 006a 0344 005d 0a7d 0164 037c 015f  .|.j.D.].}.d.|._
+00009cd0: 0071 1e7c 00a0 04a1 0001 0064 0253 0029  .q.|.......d.S.)
+00009ce0: 047a 174f 7065 6e74 6561 2056 414c 4944  .z.Opentea VALID
+00009cf0: 4154 4520 6d65 7468 6f64 7201 0000 004e  ATE methodr....N
+00009d00: 7234 0000 0029 0572 5700 0000 7221 0000  r4...).rW...r!..
+00009d10: 0072 4f00 0000 7293 0100 0072 5800 0000  .rO...r....rX...
+00009d20: 2902 7229 0000 0072 9f01 0000 722e 0000  ).r)...r....r...
+00009d30: 0072 2e00 0000 722f 0000 0072 5900 0000  .r....r/...rY...
+00009d40: 3e05 0000 730c 0000 0000 030a 0104 020a  >...s...........
+00009d50: 020a 0108 027a 164f 5444 796e 616d 6963  .....z.OTDynamic
+00009d60: 4c69 7374 2e76 616c 6964 6174 6529 014e  List.validate).N
+00009d70: 2901 4e29 2072 6300 0000 7264 0000 0072  ).N) rc...rd...r
+00009d80: 6500 0000 7266 0000 0072 1f00 0000 7226  e...rf...r....r&
+00009d90: 0000 0072 8001 0000 7288 0100 0072 8900  ...r....r....r..
+00009da0: 0000 7287 0100 0072 6401 0000 7277 0100  ..r....rd...rw..
+00009db0: 0072 9401 0000 7292 0100 0072 8b01 0000  .r....r....r....
+00009dc0: 728c 0100 0072 ab00 0000 727f 0100 0072  r....r....r....r
+00009dd0: 2500 0000 72a5 0100 0072 a401 0000 72a6  %...r....r....r.
+00009de0: 0100 0072 a901 0000 72a0 0100 0072 a101  ...r....r....r..
+00009df0: 0000 72a2 0100 0072 5f00 0000 72ae 0100  ..r....r_...r...
+00009e00: 0072 5100 0000 7221 0000 0072 5900 0000  .rQ...r!...rY...
+00009e10: 7267 0000 0072 2e00 0000 722e 0000 0072  rg...r....r....r
+00009e20: 2c00 0000 722f 0000 0072 8101 0000 2804  ,...r/...r....(.
+00009e30: 0000 7338 0000 0008 0104 020c 190c 0602  ..s8............
+00009e40: 010a 0408 0708 1308 050c 0708 0a08 1c08  ................
+00009e50: 0908 0808 0508 0a08 0308 0a08 0e08 0808  ................
+00009e60: 070a 0d0a 1608 0408 0908 0508 1f08 0572  ...............r
+00009e70: 8101 0000 6300 0000 0000 0000 0000 0000  ....c...........
+00009e80: 0000 0000 0003 0000 0000 0000 0073 9200  .............s..
+00009e90: 0000 6500 5a01 6400 5a02 6401 5a03 6402  ..e.Z.d.Z.d.Z.d.
+00009ea0: 6403 8400 5a04 6404 6405 8400 5a05 6406  d...Z.d.d...Z.d.
+00009eb0: 6407 8400 5a06 6408 6409 8400 5a07 640a  d...Z.d.d...Z.d.
+00009ec0: 640b 8400 5a08 8700 6601 640c 640d 8408  d...Z...f.d.d...
+00009ed0: 5a09 650a 640e 640f 8400 8301 5a0b 650b  Z.e.d.d.....Z.e.
+00009ee0: 6a0c 6410 640f 8400 8301 5a0b 6411 6412  j.d.d.....Z.d.d.
+00009ef0: 8400 5a0d 6413 6414 8400 5a0e 6415 6416  ..Z.d.d...Z.d.d.
+00009f00: 8400 5a0f 6417 6418 8400 5a10 6419 641a  ..Z.d.d...Z.d.d.
+00009f10: 8400 5a11 641b 641c 8400 5a12 8700 0400  ..Z.d.d...Z.....
+00009f20: 5a13 5300 291d da0c 4f54 5374 6174 6963  Z.S.)...OTStatic
+00009f30: 4c69 7374 7a4b 4c69 7374 204e 4f54 2063  ListzKList NOT c
+00009f40: 6f6e 7472 6f6c 6c65 6420 6262 7920 7468  ontrolled bby th
+00009f50: 6520 7573 6572 0a20 2020 200a 2020 2020  e user.    .    
+00009f60: 6372 6561 7465 6420 6966 206f 745f 7265  created if ot_re
+00009f70: 7175 6972 6520 6f72 2064 6973 6162 6c65  quire or disable
+00009f80: 6463 0100 0000 0000 0000 0000 0000 0300  dc..............
+00009f90: 0000 0600 0000 4300 0000 73a6 0000 0064  ......C...s....d
+00009fa0: 017d 017c 00a0 007c 01a1 0101 0074 016a  .}.|...|.....t.j
+00009fb0: 027c 006a 0364 0264 038d 027d 0274 047c  .|.j.d.d...}.t.|
+00009fc0: 006a 037c 017c 026a 0564 048d 037c 005f  .j.|.|.j.d...|._
+00009fd0: 067c 006a 066a 0764 0574 0864 0619 0074  .|.j.j.d.t.d...t
+00009fe0: 0864 0619 0074 0864 0719 0064 088d 0401  .d...t.d...d....
+00009ff0: 007c 026a 097c 006a 066a 0a64 098d 0101  .|.j.|.j.j.d....
+0000a000: 007c 026a 0b64 0a64 0b64 0c8d 0201 007c  .|.j.d.d.d.....|
+0000a010: 006a 066a 0b64 0d64 0e64 0f64 108d 0301  .j.j.d.d.d.d....
+0000a020: 007c 006a 06a0 0c64 117c 006a 0da1 0201  .|.j...d.|.j....
+0000a030: 007c 006a 06a0 0c64 127c 006a 0ea1 0201  .|.j...d.|.j....
+0000a040: 0064 1353 0029 147a 1050 6163 6b69 6e67  .d.S.).z.Packing
+0000a050: 2065 6c65 6d65 6e74 7372 4201 0000 da08   elementsrB.....
+0000a060: 7665 7274 6963 616c 2901 72f9 0000 0029  vertical).r....)
+0000a070: 0272 3100 0000 7226 0100 0072 7c00 0000  .r1...r&...r|...
+0000a080: 7280 0000 0072 8100 0000 2904 721c 0000  r....r....).r...
+0000a090: 0072 8200 0000 7279 0000 0072 8300 0000  .r....ry...r....
+0000a0a0: 722c 0100 0072 f500 0000 7223 0100 0072  r,...r....r#...r
+0000a0b0: 3900 0000 7235 0000 0072 2001 0000 728a  9...r5...r ...r.
+0000a0c0: 0000 0029 0372 3700 0000 723a 0000 0072  ...).r7...r:...r
+0000a0d0: 5201 0000 723e 0100 0072 3f01 0000 4e29  R...r>...r?...N)
+0000a0e0: 0f72 7701 0000 7202 0000 0072 fe00 0000  .rw...r....r....
+0000a0f0: 725a 0100 0072 0900 0000 7251 0000 00da  rZ...r....rQ....
+0000a100: 036c 6278 7284 0000 0072 1100 0000 7298  .lbxr....r....r.
+0000a110: 0000 0072 3701 0000 7247 0000 0072 2f01  ...r7...rG...r/.
+0000a120: 0000 7240 0100 0072 4101 0000 2903 7229  ..r@...rA...).r)
+0000a130: 0000 00da 066e 6c69 6e65 7372 3801 0000  .....nlinesr8...
+0000a140: 722e 0000 0072 2e00 0000 722f 0000 00da  r....r....r/....
+0000a150: 125f 636f 6e66 6967 7572 655f 6c69 7374  ._configure_list
+0000a160: 626f 7853 0500 0073 2600 0000 0002 0401  boxS...s&.......
+0000a170: 0a02 1002 0201 0401 0201 04fd 0804 0601  ................
+0000a180: 0201 0601 0601 06fc 0606 1001 0e01 1201  ................
+0000a190: 1001 7a1f 4f54 5374 6174 6963 4c69 7374  ..z.OTStaticList
+0000a1a0: 2e5f 636f 6e66 6967 7572 655f 6c69 7374  ._configure_list
+0000a1b0: 626f 7863 0100 0000 0000 0000 0000 0000  boxc............
+0000a1c0: 0200 0000 0300 0000 4700 0000 7310 0000  ........G...s...
+0000a1d0: 007c 006a 00a0 0164 01a1 0101 0064 0253  .|.j...d.....d.S
+0000a1e0: 0029 037a 2245 6e61 626c 6520 7363 726f  .).z"Enable scro
+0000a1f0: 6c6c 2069 6620 706f 696e 7465 7220 696e  ll if pointer in
+0000a200: 2077 6964 6765 7472 4501 0000 4ea9 0272   widgetrE...N..r
+0000a210: b501 0000 7247 0100 0072 5a00 0000 722e  ....rG...rZ...r.
+0000a220: 0000 0072 2e00 0000 722f 0000 0072 4101  ...r....r/...rA.
+0000a230: 0000 6a05 0000 7302 0000 0000 027a 204f  ..j...s......z O
+0000a240: 5453 7461 7469 634c 6973 742e 5f62 696e  TStaticList._bin
+0000a250: 645f 676c 6f62 616c 5f73 6372 6f6c 6c63  d_global_scrollc
+0000a260: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+0000a270: 0300 0000 4700 0000 7310 0000 007c 006a  ....G...s....|.j
+0000a280: 00a0 0164 01a1 0101 0064 0253 0029 037a  ...d.....d.S.).z
+0000a290: 2344 6973 6162 6c65 2073 6372 6f6c 6c20  #Disable scroll 
+0000a2a0: 6966 2070 6f69 6e74 6572 2069 6e20 7769  if pointer in wi
+0000a2b0: 6467 6574 7248 0100 004e 72b8 0100 0072  dgetrH...Nr....r
+0000a2c0: 5a00 0000 722e 0000 0072 2e00 0000 722f  Z...r....r....r/
+0000a2d0: 0000 0072 4001 0000 6e05 0000 7302 0000  ...r@...n...s...
+0000a2e0: 0000 027a 224f 5453 7461 7469 634c 6973  ...z"OTStaticLis
+0000a2f0: 742e 5f75 6e62 696e 645f 676c 6f62 616c  t._unbind_global
+0000a300: 5f73 6372 6f6c 6c63 0100 0000 0000 0000  _scrollc........
+0000a310: 0000 0000 0200 0000 0500 0000 4300 0000  ............C...
+0000a320: 7348 0000 007c 006a 006a 0164 0164 028d  sH...|.j.j.d.d..
+0000a330: 0101 007c 006a 00a0 0264 0364 04a1 0201  ...|.j...d.d....
+0000a340: 007c 006a 0344 005d 127d 017c 006a 00a0  .|.j.D.].}.|.j..
+0000a350: 0464 047c 01a1 0201 0071 227c 006a 006a  .d.|.....q"|.j.j
+0000a360: 0164 0564 028d 0101 0064 0653 0029 077a  .d.d.....d.S.).z
+0000a370: 3043 6861 6e67 6520 6170 7065 6172 656e  0Change appearen
+0000a380: 6365 2061 6363 6f72 6469 6e67 2074 6f20  ce according to 
+0000a390: 696e 7465 726e 616c 2076 6172 6961 626c  internal variabl
+0000a3a0: 6572 1d00 0000 722b 0100 0072 0100 0000  er....r+...r....
+0000a3b0: 722a 0100 0072 7c00 0000 4e29 0572 b501  r*...r|...N).r..
+0000a3c0: 0000 7284 0000 00da 0664 656c 6574 6572  ..r......deleter
+0000a3d0: c300 0000 7236 0100 0029 0272 2900 0000  ....r6...).r)...
+0000a3e0: 7256 0100 0072 2e00 0000 722e 0000 0072  rV...r....r....r
+0000a3f0: 2f00 0000 da0f 5f75 7064 6174 655f 6c69  /....._update_li
+0000a400: 7374 626f 7872 0500 0073 0a00 0000 0002  stboxr...s......
+0000a410: 0e02 0e01 0a01 1002 7a1c 4f54 5374 6174  ........z.OTStat
+0000a420: 6963 4c69 7374 2e5f 7570 6461 7465 5f6c  icList._update_l
+0000a430: 6973 7462 6f78 6301 0000 0000 0000 0000  istboxc.........
+0000a440: 0000 0001 0000 0002 0000 0043 0000 0073  ...........C...s
+0000a450: 0a00 0000 6700 7c00 5f00 6400 5300 724c  ....g.|._.d.S.rL
+0000a460: 0000 00a9 01da 095f 7661 7269 6162 6c65  ......._variable
+0000a470: 724d 0000 0072 2e00 0000 722e 0000 0072  rM...r....r....r
+0000a480: 2f00 0000 7225 0000 007d 0500 0073 0200  /...r%...}...s..
+0000a490: 0000 0001 7a18 4f54 5374 6174 6963 4c69  ....z.OTStaticLi
+0000a4a0: 7374 2e5f 6465 6669 6e65 5f76 6172 6301  st._define_varc.
+0000a4b0: 0000 0000 0000 0000 0000 0001 0000 0002  ................
+0000a4c0: 0000 0003 0000 0073 1600 0000 7400 8300  .......s....t...
+0000a4d0: a001 a100 0100 7c00 a002 a100 0100 6401  ......|.......d.
+0000a4e0: 5300 2902 7a16 4164 6420 746f 205f 6372  S.).z.Add to _cr
+0000a4f0: 6561 7465 5f77 6964 6765 7473 4e29 0372  eate_widgetsN).r
+0000a500: 1e00 0000 7226 0000 0072 b701 0000 724d  ....r&...r....rM
+0000a510: 0000 0072 2c00 0000 722e 0000 0072 2f00  ...r,...r....r/.
+0000a520: 0000 7226 0000 0080 0500 0073 0400 0000  ..r&.......s....
+0000a530: 0002 0a01 7a1c 4f54 5374 6174 6963 4c69  ....z.OTStaticLi
+0000a540: 7374 2e5f 6372 6561 7465 5f77 6964 6765  st._create_widge
+0000a550: 7473 6301 0000 0000 0000 0000 0000 0001  tsc.............
+0000a560: 0000 0001 0000 0043 0000 0073 0600 0000  .......C...s....
+0000a570: 7c00 6a00 5300 724c 0000 0072 bb01 0000  |.j.S.rL...r....
+0000a580: 724d 0000 0072 2e00 0000 722e 0000 0072  rM...r....r....r
+0000a590: 2f00 0000 72c3 0000 0085 0500 0073 0200  /...r........s..
+0000a5a0: 0000 0002 7a15 4f54 5374 6174 6963 4c69  ....z.OTStaticLi
+0000a5b0: 7374 2e76 6172 6961 626c 6563 0200 0000  st.variablec....
+0000a5c0: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+0000a5d0: 4300 0000 732c 0000 0074 007c 00a0 017c  C...s,...t.|...|
+0000a5e0: 01a1 0183 017c 005f 027c 017c 005f 037c  .....|._.|.|._.|
+0000a5f0: 00a0 04a1 0001 007c 00a0 057c 01a1 0101  .......|...|....
+0000a600: 0064 0153 0029 027a 3141 6464 2061 6464  .d.S.).z1Add add
+0000a610: 6974 696f 6e61 6c20 6265 6861 7669 6f72  itional behavior
+0000a620: 2074 6f20 7468 6520 7365 7474 6572 206f   to the setter o
+0000a630: 6620 7661 7269 6162 6c65 4e29 0672 4900  f variableN).rI.
+0000a640: 0000 da11 5f63 6f6d 7061 7265 5f70 7265  ...._compare_pre
+0000a650: 7669 6f75 7372 5700 0000 72bc 0100 0072  viousrW...r....r
+0000a660: ba01 0000 72a7 0000 0029 0272 2900 0000  ....r....).r)...
+0000a670: 72e4 0000 0072 2e00 0000 722e 0000 0072  r....r....r....r
+0000a680: 2f00 0000 72c3 0000 0089 0500 0073 0800  /...r........s..
+0000a690: 0000 0003 1002 0601 0801 6302 0000 0000  ..........c.....
+0000a6a0: 0000 0000 0000 0004 0000 0003 0000 0043  ...............C
+0000a6b0: 0000 0073 3e00 0000 7400 7c01 8301 7400  ...s>...t.|...t.
+0000a6c0: 7c00 6a01 8301 6b03 7216 6401 5300 7402  |.j...k.r.d.S.t.
+0000a6d0: 7c00 6a01 7c01 8302 4400 5d16 5c02 7d02  |.j.|...D.].\.}.
+0000a6e0: 7d03 7c02 7c03 6b03 7222 0100 6401 5300  }.|.|.k.r"..d.S.
+0000a6f0: 7122 6402 5300 2903 7a2b 5472 7565 2069  q"d.S.).z+True i
+0000a700: 6620 7661 6c75 6573 2069 6465 6e74 6963  f values identic
+0000a710: 616c 2074 6f20 7072 6576 696f 7573 2076  al to previous v
+0000a720: 616c 7565 7346 5429 0372 cf00 0000 724f  aluesFT).r....rO
+0000a730: 0000 0072 b500 0000 2904 7229 0000 0072  ...r....).r)...r
+0000a740: e400 0000 72e3 0000 00da 076e 6577 5f76  ....r......new_v
+0000a750: 616c 722e 0000 0072 2e00 0000 722f 0000  alr....r....r/..
+0000a760: 0072 bd01 0000 9205 0000 730c 0000 0000  .r........s.....
+0000a770: 0212 0104 0114 0108 0108 017a 1e4f 5453  ...........z.OTS
+0000a780: 7461 7469 634c 6973 742e 5f63 6f6d 7061  taticList._compa
+0000a790: 7265 5f70 7265 7669 6f75 7363 0100 0000  re_previousc....
+0000a7a0: 0000 0000 0000 0000 0100 0000 0400 0000  ................
+0000a7b0: 4300 0000 7316 0000 007c 006a 006a 0164  C...s....|.j.j.d
+0000a7c0: 017c 006a 0264 028d 0201 0064 0353 0029  .|.j.d.....d.S.)
+0000a7d0: 0472 8d01 0000 728e 0100 0072 8f01 0000  .r....r....r....
+0000a7e0: 4e29 0372 6301 0000 7291 0100 0072 7501  N).rc...r....ru.
+0000a7f0: 0000 724d 0000 0072 2e00 0000 722e 0000  ..rM...r....r...
+0000a800: 0072 2f00 0000 7264 0100 009c 0500 0073  .r/...rd.......s
+0000a810: 0200 0000 0002 7a20 4f54 5374 6174 6963  ......z OTStatic
+0000a820: 4c69 7374 2e5f 6164 645f 706f 7075 705f  List._add_popup_
+0000a830: 636f 6d6d 616e 6473 6301 0000 0000 0000  commandsc.......
+0000a840: 0000 0000 0001 0000 0004 0000 0043 0000  .............C..
+0000a850: 0073 1c00 0000 7c00 6a00 6401 6b03 7218  .s....|.j.d.k.r.
+0000a860: 7c00 a001 7c00 a002 a100 a101 0100 6402  |...|.........d.
+0000a870: 5300 72ac 0100 0029 0372 5700 0000 72a7  S.r....).rW...r.
+0000a880: 0000 0072 2100 0000 724d 0000 0072 2e00  ...r!...rM...r..
+0000a890: 0000 722e 0000 0072 2f00 0000 725f 0000  ..r....r/...r_..
+0000a8a0: 00a1 0500 0073 0400 0000 0005 0a01 7a1d  .....s........z.
+0000a8b0: 4f54 5374 6174 6963 4c69 7374 2e6f 6e5f  OTStaticList.on_
+0000a8c0: 7570 6461 7465 5f73 7461 7475 7363 0100  update_statusc..
+0000a8d0: 0000 0000 0000 0000 0000 0100 0000 0100  ................
+0000a8e0: 0000 4300 0000 7306 0000 007c 006a 0053  ..C...s....|.j.S
+0000a8f0: 0029 0172 b201 0000 2901 72c3 0000 0072  .).r....).r....r
+0000a900: 4d00 0000 722e 0000 0072 2e00 0000 722f  M...r....r....r/
+0000a910: 0000 0072 2100 0000 aa05 0000 7302 0000  ...r!.......s...
+0000a920: 0000 027a 104f 5453 7461 7469 634c 6973  ...z.OTStaticLis
+0000a930: 742e 6765 7463 0200 0000 0000 0000 0000  t.getc..........
+0000a940: 0000 0200 0000 0200 0000 4300 0000 730e  ..........C...s.
+0000a950: 0000 0074 007c 0183 017c 005f 0164 0153  ...t.|...|._.d.S
+0000a960: 0029 027a 544f 7065 6e74 6561 2053 4554  .).zTOpentea SET
+0000a970: 206d 6574 686f 640a 2020 2020 2020 2020   method.        
+0000a980: 4279 2061 7373 6967 6e69 6e67 2077 6520  By assigning we 
+0000a990: 7472 6967 6765 7220 7468 6520 7661 7269  trigger the vari
+0000a9a0: 6162 6c65 205f 5f73 6574 7465 725f 5f20  able __setter__ 
+0000a9b0: 0a20 2020 2020 2020 204e 2902 da04 6c69  .        N)...li
+0000a9c0: 7374 72c3 0000 0072 7100 0000 722e 0000  str....rq...r...
+0000a9d0: 0072 2e00 0000 722f 0000 0072 5100 0000  .r....r/...rQ...
+0000a9e0: ae05 0000 7302 0000 0000 047a 104f 5453  ....s......z.OTS
+0000a9f0: 7461 7469 634c 6973 742e 7365 7463 0100  taticList.setc..
+0000aa00: 0000 0000 0000 0000 0000 0100 0000 0200  ................
+0000aa10: 0000 4300 0000 732a 0000 007c 006a 0064  ..C...s*...|.j.d
+0000aa20: 016b 0372 0e64 0053 007c 00a0 01a1 007c  .k.r.d.S.|.....|
+0000aa30: 005f 0264 027c 005f 007c 00a0 03a1 0001  ._.d.|._.|......
+0000aa40: 0064 0053 0072 5600 0000 2904 7257 0000  .d.S.rV...).rW..
+0000aa50: 0072 2100 0000 724f 0000 0072 5800 0000  .r!...rO...rX...
+0000aa60: 724d 0000 0072 2e00 0000 722e 0000 0072  rM...r....r....r
+0000aa70: 2f00 0000 7259 0000 00b4 0500 0073 0a00  /...rY.......s..
+0000aa80: 0000 0001 0a01 0402 0a01 0601 7a15 4f54  ............z.OT
+0000aa90: 5374 6174 6963 4c69 7374 2e76 616c 6964  StaticList.valid
+0000aaa0: 6174 6529 1472 6300 0000 7264 0000 0072  ate).rc...rd...r
+0000aab0: 6500 0000 7266 0000 0072 b701 0000 7241  e...rf...r....rA
+0000aac0: 0100 0072 4001 0000 72ba 0100 0072 2500  ...r@...r....r%.
+0000aad0: 0000 7226 0000 0072 8001 0000 72c3 0000  ..r&...r....r...
+0000aae0: 00da 0673 6574 7465 7272 bd01 0000 7264  ...setterr....rd
+0000aaf0: 0100 0072 5f00 0000 7221 0000 0072 5100  ...r_...r!...rQ.
+0000ab00: 0000 7259 0000 0072 6700 0000 722e 0000  ..rY...rg...r...
+0000ab10: 0072 2e00 0000 722c 0000 0072 2f00 0000  .r....r,...r/...
+0000ab20: 72b3 0100 004d 0500 0073 2200 0000 0801  r....M...s".....
+0000ab30: 0405 0817 0804 0804 080b 0803 0c05 0201  ................
+0000ab40: 0a03 0401 0a08 080a 0805 0809 0804 0806  ................
+0000ab50: 72b3 0100 0029 3a72 6600 0000 720d 0100  r....):rf...r...
+0000ab60: 0072 b200 0000 72bb 0000 0072 9a01 0000  .r....r....r....
+0000ab70: 7202 0000 0072 0300 0000 7204 0000 0072  r....r....r....r
+0000ab80: 0500 0000 7206 0000 0072 0700 0000 7208  ....r....r....r.
+0000ab90: 0000 0072 0900 0000 720a 0000 0072 0b00  ...r....r....r..
+0000aba0: 0000 720c 0000 00da 036e 6f62 720d 0000  ..r......nobr...
+0000abb0: 00da 176f 7065 6e74 6561 2e67 7569 5f66  ...opentea.gui_f
+0000abc0: 6f72 6d73 2e5f 6261 7365 720e 0000 00da  orms._baser.....
+0000abd0: 1d6f 7065 6e74 6561 2e67 7569 5f66 6f72  .opentea.gui_for
+0000abe0: 6d73 2e5f 6578 6365 7074 696f 6e73 720f  ms._exceptionsr.
+0000abf0: 0000 0072 1000 0000 da1b 6f70 656e 7465  ...r......opente
+0000ac00: 612e 6775 695f 666f 726d 732e 636f 6e73  a.gui_forms.cons
+0000ac10: 7461 6e74 7372 1100 0000 7212 0000 0072  tantsr....r....r
+0000ac20: 1300 0000 7214 0000 00da 216f 7065 6e74  ....r.....!opent
+0000ac30: 6561 2e67 7569 5f66 6f72 6d73 2e67 656e  ea.gui_forms.gen
+0000ac40: 6572 6963 5f77 6964 6765 7473 7215 0000  eric_widgetsr...
+0000ac50: 00da 176f 7065 6e74 6561 2e67 7569 5f66  ...opentea.gui_f
+0000ac60: 6f72 6d73 2e75 7469 6c73 7216 0000 0072  orms.utilsr....r
+0000ac70: 1700 0000 da1c 6f70 656e 7465 612e 6775  ......opentea.gu
+0000ac80: 695f 666f 726d 732e 736f 756e 6462 6f61  i_forms.soundboa
+0000ac90: 7264 7218 0000 00da 0741 4243 4d65 7461  rdr......ABCMeta
+0000aca0: 7219 0000 0072 6900 0000 7273 0000 0072  r....ri...rs...r
+0000acb0: 8800 0000 72bd 0000 0072 bf00 0000 72c0  ....r....r....r.
+0000acc0: 0000 0072 c100 0000 72c9 0000 0072 cc00  ...r....r....r..
+0000acd0: 0000 72d1 0000 0072 d000 0000 72ec 0000  ..r....r....r...
+0000ace0: 0072 d200 0000 7216 0100 0072 3b01 0000  .r....r....r;...
+0000acf0: 723d 0100 0072 4b01 0000 7258 0100 0072  r=...rK...rX...r
+0000ad00: 7801 0000 7281 0100 0072 b301 0000 722e  x...r....r....r.
+0000ad10: 0000 0072 2e00 0000 722e 0000 0072 2f00  ...r....r....r/.
+0000ad20: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+0000ad30: 734a 0000 0004 4308 0108 0108 0208 0134  sJ....C........4
+0000ad40: 0e0c 020c 0110 0418 070c 0110 040c 0b16  ................
+0000ad50: 6510 1516 2c16 7f00 0510 0610 0410 0610  e...,...........
+0000ad60: 1e16 1e0e 0d10 3810 1710 5a10 1010 5210  ......8...Z...R.
+0000ad70: 1f10 3710 1916 4810 6e10 7f00 7f00 27    ..7...H.n.....'
```

### Comparing `OpenTEA-3.5.0/src/opentea/gui_forms/__pycache__/menus.cpython-39.pyc` & `OpenTEA-3.6.0/src/opentea/gui_forms/__pycache__/menus.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/gui_forms/__pycache__/node_widgets.cpython-39.pyc` & `OpenTEA-3.6.0/src/opentea/gui_forms/__pycache__/node_widgets.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/gui_forms/__pycache__/otinker.cpython-39.pyc` & `OpenTEA-3.6.0/src/opentea/gui_forms/__pycache__/otinker.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/gui_forms/__pycache__/root_widget.cpython-39.pyc` & `OpenTEA-3.6.0/src/opentea/gui_forms/__pycache__/root_widget.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/gui_forms/__pycache__/soundboard.cpython-39.pyc` & `OpenTEA-3.6.0/src/opentea/gui_forms/__pycache__/soundboard.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/gui_forms/__pycache__/utils.cpython-39.pyc` & `OpenTEA-3.6.0/src/opentea/gui_forms/__pycache__/utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/gui_forms/__pycache__/viewer_2d.cpython-39.pyc` & `OpenTEA-3.6.0/src/opentea/gui_forms/__pycache__/viewer_2d.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/gui_forms/__pycache__/viewer_3d.cpython-39.pyc` & `OpenTEA-3.6.0/src/opentea/gui_forms/__pycache__/viewer_3d.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/gui_forms/_base.py` & `OpenTEA-3.6.0/src/opentea/gui_forms/_base.py`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/gui_forms/constants.py` & `OpenTEA-3.6.0/src/opentea/gui_forms/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 import os
 from glob import glob
 import inspect
 import platform
-
+from loguru import logger
 from PIL import (
     ImageTk,
     Image,
 )
 
 
 # BG_COLOR = '#%02x%02x%02x' % (220, 218, 213)
@@ -69,21 +69,30 @@
             bgc[1] - 1,
             bgc[2] + 4,
         )
 
     bgc_dark = tuple([int(0.3 * i) for i in bgc])
     PARAMS["bg_dark"] = "#%02x%02x%02x" % bgc_dark
     PARAMS["hl_bg"] = '#ffe785'  # highlight background color
-
+    PARAMS["verbose_log"] = False
 
 def set_system():
     global PARAMS
     PARAMS["sys"] = platform.system()
 
 
+def toggle_verbose():
+    global PARAMS
+    if PARAMS["verbose_log"] is False:
+        PARAMS["verbose_log"]= True
+        logger.info("Switching verbose mode on...")
+    else:
+        PARAMS["verbose_log"]= False
+        logger.info("Switching verbose mode off...")
+
 # pylint: disable=global-statement
 def load_icons():
     """Load icons.
 
     Load all ./otinker_images/*_icon.gif as icons
 
     Returns :
```

### Comparing `OpenTEA-3.5.0/src/opentea/gui_forms/generic_widgets.py` & `OpenTEA-3.6.0/src/opentea/gui_forms/generic_widgets.py`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/gui_forms/images/about_icon.gif` & `OpenTEA-3.6.0/src/opentea/gui_forms/images/about_icon.gif`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/gui_forms/images/help_icon.gif` & `OpenTEA-3.6.0/src/opentea/gui_forms/images/help_icon.gif`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/gui_forms/images/invalid_icon.gif` & `OpenTEA-3.6.0/src/opentea/gui_forms/images/invalid_icon.gif`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/gui_forms/images/load_icon.gif` & `OpenTEA-3.6.0/src/opentea/gui_forms/images/load_icon.gif`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/gui_forms/images/logo_opentea.gif` & `OpenTEA-3.6.0/src/opentea/gui_forms/images/logo_opentea.gif`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/gui_forms/images/logo_project_large.gif` & `OpenTEA-3.6.0/src/opentea/gui_forms/images/logo_project_large.gif`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/gui_forms/images/new_icon.gif` & `OpenTEA-3.6.0/src/opentea/gui_forms/images/new_icon.gif`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/gui_forms/images/save_icon.gif` & `OpenTEA-3.6.0/src/opentea/gui_forms/images/save_icon.gif`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/gui_forms/images/unknown_icon.gif` & `OpenTEA-3.6.0/src/opentea/gui_forms/images/unknown_icon.gif`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/gui_forms/images/valid_icon.gif` & `OpenTEA-3.6.0/src/opentea/gui_forms/images/valid_icon.gif`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/gui_forms/images/wait_2_icon.gif` & `OpenTEA-3.6.0/src/opentea/gui_forms/images/wait_2_icon.gif`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/gui_forms/leaf_widgets.py` & `OpenTEA-3.6.0/src/opentea/gui_forms/leaf_widgets.py`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/gui_forms/menus.py` & `OpenTEA-3.6.0/src/opentea/gui_forms/menus.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 
 import os
 from abc import ABCMeta
 from abc import abstractmethod
 import tkinter as tk
 from tkinter import filedialog
-
+from loguru import logger
 from nobvisual import visual_treenob
 
 from opentea.noob.asciigraph import nob_asciigraph
 from opentea.gui_forms.utils import quit_dialog
+from opentea.gui_forms.constants import toggle_verbose
 from opentea.gui_forms.generic_widgets import TextConsole
 
 
 # TODO: about in md instead?
 ABOUT = """
 This is GUI FORMS, front ends provided by OpenTEA.
 
@@ -139,18 +140,29 @@
         self.add_command(label="Show tree", image=self.otroot.icons["tree"],
                          compound="left", command=self.on_show_tree)
 
         self.add_command(label="Show circular map", image=self.otroot.icons["tree"],
                          compound="left", command=self.on_show_circular)
         self.add_command(label="Show status map", image=self.otroot.icons["tree"],
                          compound="left", command=self.on_show_status)
+        self.add_command(label="Toggle verbose log",
+                         compound="left", command=self.on_toggle_verbose)
+
 
     def _bind_items(self):
         self.root.bind("<Control-h>", self.on_show_tree)
 
+
+    def on_toggle_verbose(self, event=None):
+        """Toggle verbose mode in terminal
+        """
+        toggle_verbose()
+            
+
+
     def on_show_tree(self, event=None):
         toplevel = tk.Toplevel(self.root)
         toplevel.title("Tree View")
         toplevel.transient(self.root)
 
         memory = tk.StringVar(value=nob_asciigraph(self.otroot.get()))
```

### Comparing `OpenTEA-3.5.0/src/opentea/gui_forms/node_widgets.py` & `OpenTEA-3.6.0/src/opentea/gui_forms/node_widgets.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,16 @@
 """
 
 import os
 import warnings
 import copy
 import time
 import subprocess
-
+from loguru import logger
+import colorama as clrm
 import tkinter as tk
 from tkinter import (
     ttk,
     Menu,
     Entry,
     Frame,
     StringVar,
@@ -296,16 +297,15 @@
             try:
                 if child in dict_:
                     try:
                         self.children[child].set(dict_[child])
                     except SetException:
                         pass
             except TypeError:
-                print("==========================")
-                print("Child not set", child, nob_pprint(self.schema, max_lvl=2))
+                logger.error(f"Child {child} not set\n{nob_pprint(self.schema, max_lvl=2)}")
 
     def validate(self):
 
         if self.status != 0:
             return
 
         self.validate_children()
@@ -656,15 +656,15 @@
             play_item()
         
     def execute(self, script):
         """execute a script"""
         # TODO: execute via import instead of script?
 
         full_script = os.path.join(PARAMS["calling_dir"], script)
-        print("Mem update : Executing in subprocess ", full_script)
+        logger.info("Executing in subprocess :", full_script)
         start = time.time()
         dump = yaml.dump(self.parent.get(), default_flow_style=False)
 
         with open(".dataset_from_gui.yml", "w") as fout:
             fout.writelines(dump)
 
         subp = subprocess.run(
@@ -679,34 +679,30 @@
         duration = str(round(end - start, 3)) + "s"
 
         returnstr = ""
         success = False
         if subp.returncode == 0:
             success = True
 
-            print("Process successful...")
-            print("\n" + subp.stdout.decode("utf-8"))
+            logger.success("Process successful...")
+            #logger.debug("\n" + subp.stdout.decode("utf-8"))
+            logwcolor(subp.stdout.decode("utf-8").split("\n"))
+            
             with open(".dataset_to_gui.yml", "r") as fin:
                 data_in = yaml.load(fin, Loader=yaml.SafeLoader)
                 # main_validate(data_in, self.schema)
                 self.parent.set(data_in)
 
         else:
-            msg_err = "Return code : " + str(subp.returncode)
-            msg_err += "\n" + "### STD-OUT / ERR ###" + "\n"
-            msg_err += subp.stdout.decode("utf-8")
-
-            print("Process failed...")
-            print(msg_err)
-
-            for line in subp.stdout.decode("utf-8").split("\n"):
-                if "Error" in line:
-                    returnstr = line
+            logger.error("Process failed...")
+            logger.debug(f"Return code : {subp.returncode}")
+            returnstr=logwcolor(subp.stdout.decode("utf-8").split("\n"))
+            #logger.error(msg_err)
 
-        print("Process finished in " + duration)
+        logger.info("Process finished in " + duration)
 
         return success, duration, returnstr
 
     def _get_status_icon(self, status):
         status2icon = {0: "unknown", 1: "valid", -1: "invalid"}
         return status2icon[status]
 
@@ -715,14 +711,44 @@
         status_icon = self._get_status_icon(status)
 
         if self._status_icon != status_icon:
             self.parent.notebook.tab(
                 self.tab_id, image=IMAGE_DICT[status_icon], compound="left")
             self._status_icon = status_icon
 
+def logwcolor(text:list)->str:
+
+    returnstr=""
+    clrm.init()
+
+    for line in text:
+        if "Error" in line:
+            returnstr=line
+            
+        if "DEBUG" in line[25:35]:
+            if PARAMS["verbose_log"]:
+                print(clrm.Back.BLACK+clrm.Fore.BLUE+clrm.Style.NORMAL+line[25:])
+        elif "INFO" in line[25:35]:
+            print(clrm.Back.BLACK+clrm.Fore.WHITE+clrm.Style.NORMAL+line[25:])
+        elif "SUCCES" in line[25:35]:
+            print(clrm.Back.BLACK+clrm.Fore.GREEN+clrm.Style.BRIGHT+line[25:])
+        elif "WARNING" in line[25:35]:
+            print(clrm.Back.BLACK+clrm.Fore.YELLOW+clrm.Style.BRIGHT+line[25:])
+        elif "CRITICAL" in line[25:35]:
+            print(clrm.Back.BLACK+clrm.Fore.RED+clrm.Style.BRIGHT+line[25:])
+        else :
+            print(clrm.Back.BLACK+clrm.Fore.CYAN+clrm.Style.NORMAL+line)
+    clrm.reinit()
+    return returnstr
+#2023-07-13 06:47:34.825 | WARNING  | 
+#01234567890123456789012345678901234567
+        
+            
+            
+
 
 class OTMultipleWidget(OTNodeWidget):
     """OT multiple widget."""
     # TODO: break in dependent/non-dependent?
     # TODO: add min and max?
     def __init__(self, schema, parent, name, root_frame):
         """Startup class.
```

### Comparing `OpenTEA-3.5.0/src/opentea/gui_forms/otinker.py` & `OpenTEA-3.6.0/src/opentea/gui_forms/otinker.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 """
 import os
 from tkinter import (
     Tk,
     ttk,
 )
 
-
+from loguru import logger
 import opentea
 from opentea.gui_forms.root_widget import OTRoot
 from opentea.gui_forms.constants import (
     set_constants,
 )
 from opentea.gui_forms.utils import quit_dialog
 from opentea.noob.validation import validate_opentea_schema
@@ -53,33 +53,33 @@
     Outputs :
     ---------
     a tkinter GUI
     """
 
     # global CALLING_DIR
     # CALLING_DIR = calling_dir
-    print(f" (**,) Staring up OpenTEA GUI engine v.{opentea.__version__}...")
+    logger.debug(f" (**,) Staring up OpenTEA GUI engine v.{opentea.__version__}...")
     validate_opentea_schema(schema)
     tksession = Tk()
     tksession.protocol("WM_DELETE_WINDOW", quit_dialog)
 
     sty = ttk.Style()
     sty.theme_use(theme)
 
     set_constants(tksession, calling_dir, theme)
 
     if start_mainloop is False or data_file is None:
         create_voidfile("dummy.yml")
-        print(" (oO,) |No file provided, using dummy.yml for now.")
+        logger.warning(" (oO,) |No file provided, using dummy.yml for now.")
         data_file = "dummy.yml"
 
     data_file = os.path.abspath(data_file)
 
 
-    print(f" (^^,) |Opening {data_file}...")
+    logger.success(f" (^^,) |Opening {data_file}...")
     otroot = OTRoot(
         schema,
         tksession,
         sty,
         data_file=data_file,
         tab_3d=tab_3d,
         tab_2d=tab_2d,
```

### Comparing `OpenTEA-3.5.0/src/opentea/gui_forms/root_widget.py` & `OpenTEA-3.6.0/src/opentea/gui_forms/root_widget.py`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/gui_forms/soundboard.py` & `OpenTEA-3.6.0/src/opentea/gui_forms/soundboard.py`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/gui_forms/utils.py` & `OpenTEA-3.6.0/src/opentea/gui_forms/utils.py`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/gui_forms/viewer_2d.py` & `OpenTEA-3.6.0/src/opentea/gui_forms/viewer_2d.py`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/gui_forms/viewer_3d.py` & `OpenTEA-3.6.0/src/opentea/gui_forms/viewer_3d.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import os
 import subprocess
 from tkinter import ttk
 
+from loguru import logger
 import yaml
-from tiny_3d_engine import (
-    Engine3D,
-    load_file_as_scene,
-)
+from tiny_3d_engine.engine import Engine3D
+from tiny_3d_engine.scene3d import load_file_as_scene
 
 from opentea.gui_forms.constants import PARAMS
 #from opentea.gui_forms.root_widget import OTRoot
 # todo : move this into root module
 
 def add_viewer_3d(otroot):
     title = "3D view"
@@ -36,15 +35,15 @@
         self.otroot = otroot
 
     def update_view(self, script: str):
         """execute a script for 3d view update"""
         # TODO: clean tmp files
 
         full_script = os.path.join(PARAMS["calling_dir"], script)
-        print("3D-view : Executing in subprocess ", full_script)
+        logger.debug("3D-view : Executing in subprocess ", full_script)
 
         try:
             scene_file = ".scene_from_gui.geo"
             self.dump(".scene_from_gui")
         except ValueError:
             scene_file = "no_scene"
 
@@ -58,26 +57,26 @@
             # capture_output=True,  # only for python 3.7
             stdout=subprocess.PIPE,
             stderr=subprocess.STDOUT,
             check=False,
         )
 
         if not os.path.exists(".scene_to_gui.geo"):
-            print('No scene: no 3D update.')
+            logger.debug('No scene: no 3D update.')
             return True
 
         if subp.returncode == 0:
             new_scene = load_file_as_scene(".scene_to_gui.geo")
-            print("3D update...")
-            print("\n" + subp.stdout.decode("utf-8"))
+            logger.debug("3D update...")
+            logger.debug("\n" + subp.stdout.decode("utf-8"))
             self.update(new_scene)
             self.render()
             return True  # success
 
         else:
             msg_err = "Return code : " + str(subp.returncode)
             msg_err += "\n" + "### STD-OUT / ERR ###" + "\n"
             msg_err += subp.stdout.decode("utf-8")
-            print("no 3D update.")
-            print(msg_err)
+            logger.warning("3D update failed")
+            logger.warning(msg_err)
 
             return False
```

### Comparing `OpenTEA-3.5.0/src/opentea/gui_forms/wav/dsbdcls.wav` & `OpenTEA-3.6.0/src/opentea/gui_forms/wav/dsbdcls.wav`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/gui_forms/wav/dsbdopn.wav` & `OpenTEA-3.6.0/src/opentea/gui_forms/wav/dsbdopn.wav`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/gui_forms/wav/dsdorcls.wav` & `OpenTEA-3.6.0/src/opentea/gui_forms/wav/dsdorcls.wav`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/gui_forms/wav/dsdoropn.wav` & `OpenTEA-3.6.0/src/opentea/gui_forms/wav/dsdoropn.wav`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/gui_forms/wav/dsitemup.wav` & `OpenTEA-3.6.0/src/opentea/gui_forms/wav/dsitemup.wav`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/gui_forms/wav/dsoof.wav` & `OpenTEA-3.6.0/src/opentea/gui_forms/wav/dsoof.wav`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/gui_forms/wav/dsplpain.wav` & `OpenTEA-3.6.0/src/opentea/gui_forms/wav/dsplpain.wav`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/gui_forms/wav/dsswtchn.wav` & `OpenTEA-3.6.0/src/opentea/gui_forms/wav/dsswtchn.wav`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/noob/__pycache__/asciigraph.cpython-39.pyc` & `OpenTEA-3.6.0/src/opentea/noob/__pycache__/asciigraph.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/noob/__pycache__/check_schema.cpython-39.pyc` & `OpenTEA-3.6.0/src/opentea/noob/__pycache__/check_schema.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/noob/__pycache__/inferdefault.cpython-39.pyc` & `OpenTEA-3.6.0/src/opentea/noob/__pycache__/inferdefault.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/noob/__pycache__/noob.cpython-39.pyc` & `OpenTEA-3.6.0/src/opentea/noob/__pycache__/noob.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/noob/__pycache__/schema.cpython-39.pyc` & `OpenTEA-3.6.0/src/opentea/noob/__pycache__/schema.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/noob/__pycache__/validate_light.cpython-39.pyc` & `OpenTEA-3.6.0/src/opentea/noob/__pycache__/validate_light.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/noob/__pycache__/validation.cpython-39.pyc` & `OpenTEA-3.6.0/src/opentea/noob/__pycache__/validation.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/noob/asciigraph.py` & `OpenTEA-3.6.0/src/opentea/noob/asciigraph.py`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/noob/check_schema.py` & `OpenTEA-3.6.0/src/opentea/noob/check_schema.py`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/noob/inferdefault.py` & `OpenTEA-3.6.0/src/opentea/noob/inferdefault.py`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/noob/noob.py` & `OpenTEA-3.6.0/src/opentea/noob/noob.py`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/noob/schema.json` & `OpenTEA-3.6.0/src/opentea/noob/schema.json`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/noob/schema.py` & `OpenTEA-3.6.0/src/opentea/noob/schema.py`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/noob/validate_light.py` & `OpenTEA-3.6.0/src/opentea/noob/validate_light.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Lightweight validate from jsonschema"""
 
 import jsonschema
 import numpy as np
 from opentea.noob.noob import nob_pprint
-
+from loguru import logger
 
 class ValidationErrorShort(Exception):
     """Valodation error"""
 
 
 __all__ = ["validate_light"]
 
@@ -115,15 +115,15 @@
         allowed_props = list(schema["properties"].keys())
         for key in list_keys:
             if key in allowed_props:
                 out = validate_base(
                     data[key], schema["properties"][key], path=path + "." + key
                 )
                 if out is not None:
-                    print("KO", path, (path + "." + key))
+                    logger.warning(f"Props not validated {path}, {(path + '.' + key)}")
                     return out
 
         if "additionalProperties" in schema:
             if schema["additionalProperties"] is False:
                 list_keys = list(data.keys())
                 allowed_props = list(schema["properties"].keys())
                 for key in allowed_props:
```

### Comparing `OpenTEA-3.5.0/src/opentea/noob/validation.py` & `OpenTEA-3.6.0/src/opentea/noob/validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Module to operate a trplie layer of validation"""
 
 
 import json
-
+from loguru import logger
 from opentea.noob.noob import (nob_find,
                                # nob_find_unique,
                                nob_node_exist,
                                nob_get,
                                nob_set,
                                nob_pprint)
 from opentea.noob.schema import clean_schema_addresses
@@ -266,16 +266,15 @@
             log += _require_update_data(data,
                                         src_nodename,
                                         tgt_data_address,
                                         tgt_schema,
                                         data_out,
                                         multiple_fill)
 
-    if verbose:
-        print(log)
+    logger.debug(log)
 
     return data_out
 
 #pylint: disable=too-many-arguments
 def _require_update_data(data,
                          src_nodename,
                          tgt_data_address,
```

### Comparing `OpenTEA-3.5.0/src/opentea/process_utils.py` & `OpenTEA-3.6.0/src/opentea/process_utils.py`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/tools/__pycache__/proxy_h5.cpython-39.pyc` & `OpenTEA-3.6.0/src/opentea/tools/__pycache__/proxy_h5.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/tools/__pycache__/schema2md.cpython-39.pyc` & `OpenTEA-3.6.0/src/opentea/tools/__pycache__/schema2md.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/tools/__pycache__/visit_h5.cpython-39.pyc` & `OpenTEA-3.6.0/src/opentea/tools/__pycache__/visit_h5.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/tools/proxy_h5.py` & `OpenTEA-3.6.0/src/opentea/tools/proxy_h5.py`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/tools/schema2md.py` & `OpenTEA-3.6.0/src/opentea/tools/schema2md.py`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/opentea/tools/visit_h5.py` & `OpenTEA-3.6.0/src/opentea/tools/visit_h5.py`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/tkhtmlview/__init__.py` & `OpenTEA-3.6.0/src/tkhtmlview/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/tkhtmlview/__pycache__/__init__.cpython-39.pyc` & `OpenTEA-3.6.0/src/tkhtmlview/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/tkhtmlview/__pycache__/html_parser.cpython-39.pyc` & `OpenTEA-3.6.0/src/tkhtmlview/__pycache__/html_parser.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `OpenTEA-3.5.0/src/tkhtmlview/html_parser.py` & `OpenTEA-3.6.0/src/tkhtmlview/html_parser.py`

 * *Files identical despite different names*

