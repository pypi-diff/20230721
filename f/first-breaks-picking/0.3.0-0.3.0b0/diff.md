# Comparing `tmp/first-breaks-picking-0.3.0.tar.gz` & `tmp/first-breaks-picking-0.3.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "first-breaks-picking-0.3.0.tar", last modified: Fri Jul 21 10:13:23 2023, max compression
+gzip compressed data, was "first-breaks-picking-0.3.0b0.tar", last modified: Wed Jul 19 05:44:41 2023, max compression
```

## Comparing `first-breaks-picking-0.3.0.tar` & `first-breaks-picking-0.3.0b0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-07-21 10:13:22.999121 first-breaks-picking-0.3.0/
--rw-r--r--   0 daloro    (1000) daloro    (1000)    11357 2023-05-10 12:43:20.000000 first-breaks-picking-0.3.0/LICENSE
--rw-rw-r--   0 daloro    (1000) daloro    (1000)    24006 2023-07-21 10:13:22.999121 first-breaks-picking-0.3.0/PKG-INFO
--rw-r--r--   0 daloro    (1000) daloro    (1000)    22791 2023-07-19 05:43:43.000000 first-breaks-picking-0.3.0/README.md
-drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-07-21 10:13:22.995121 first-breaks-picking-0.3.0/first_breaks/
--rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-05-10 12:43:20.000000 first-breaks-picking-0.3.0/first_breaks/__init__.py
-drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-07-21 10:13:22.991121 first-breaks-picking-0.3.0/first_breaks/_pytorch/
-drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-07-21 10:13:22.995121 first-breaks-picking-0.3.0/first_breaks/_pytorch/models/
--rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-07-10 12:37:21.000000 first-breaks-picking-0.3.0/first_breaks/_pytorch/models/__init__.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)     5730 2023-07-10 12:37:21.000000 first-breaks-picking-0.3.0/first_breaks/_pytorch/models/unet3plus.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)      352 2023-06-12 06:38:44.000000 first-breaks-picking-0.3.0/first_breaks/cli.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)     1171 2023-07-10 12:37:21.000000 first-breaks-picking-0.3.0/first_breaks/const.py
-drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-07-21 10:13:22.995121 first-breaks-picking-0.3.0/first_breaks/data_models/
--rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-07-17 07:07:08.000000 first-breaks-picking-0.3.0/first_breaks/data_models/__init__.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)     1701 2023-07-18 13:44:34.000000 first-breaks-picking-0.3.0/first_breaks/data_models/dependent.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)     2090 2023-07-18 17:00:55.000000 first-breaks-picking-0.3.0/first_breaks/data_models/independent.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)      441 2023-07-18 13:44:34.000000 first-breaks-picking-0.3.0/first_breaks/data_models/initialised_defaults.py
-drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-07-21 10:13:22.995121 first-breaks-picking-0.3.0/first_breaks/desktop/
--rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-05-10 12:43:20.000000 first-breaks-picking-0.3.0/first_breaks/desktop/__init__.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)     5525 2023-07-18 16:48:46.000000 first-breaks-picking-0.3.0/first_breaks/desktop/byte_encode_unit_widget.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)     1903 2023-07-18 16:49:22.000000 first-breaks-picking-0.3.0/first_breaks/desktop/combobox_with_mapping.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)    18931 2023-07-18 13:48:53.000000 first-breaks-picking-0.3.0/first_breaks/desktop/graph.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)    20070 2023-07-19 05:38:40.000000 first-breaks-picking-0.3.0/first_breaks/desktop/main_gui.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)     6739 2023-07-10 12:37:21.000000 first-breaks-picking-0.3.0/first_breaks/desktop/picking_widget.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)     2661 2023-07-18 16:49:29.000000 first-breaks-picking-0.3.0/first_breaks/desktop/radioset_widget.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)     3571 2023-07-18 16:49:46.000000 first-breaks-picking-0.3.0/first_breaks/desktop/slider_with_values.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)     2700 2023-07-10 12:37:21.000000 first-breaks-picking-0.3.0/first_breaks/desktop/threads.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)     4238 2023-07-18 16:49:38.000000 first-breaks-picking-0.3.0/first_breaks/desktop/utils.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)     7474 2023-07-18 16:47:54.000000 first-breaks-picking-0.3.0/first_breaks/desktop/visualization_settings_widget.py
-drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-07-21 10:13:22.995121 first-breaks-picking-0.3.0/first_breaks/picking/
--rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-05-30 07:39:18.000000 first-breaks-picking-0.3.0/first_breaks/picking/__init__.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)      955 2023-07-10 12:37:21.000000 first-breaks-picking-0.3.0/first_breaks/picking/ipicker.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)     4952 2023-07-10 12:37:21.000000 first-breaks-picking-0.3.0/first_breaks/picking/picker_onnx.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)     9351 2023-07-18 16:46:26.000000 first-breaks-picking-0.3.0/first_breaks/picking/task.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)     2197 2023-07-18 17:00:56.000000 first-breaks-picking-0.3.0/first_breaks/picking/utils.py
-drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-07-21 10:13:22.995121 first-breaks-picking-0.3.0/first_breaks/sgy/
--rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-05-10 12:43:20.000000 first-breaks-picking-0.3.0/first_breaks/sgy/__init__.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)     8608 2023-07-18 16:49:53.000000 first-breaks-picking-0.3.0/first_breaks/sgy/headers.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)    16232 2023-07-18 16:46:38.000000 first-breaks-picking-0.3.0/first_breaks/sgy/reader.py
-drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-07-21 10:13:22.995121 first-breaks-picking-0.3.0/first_breaks/utils/
--rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-05-10 12:43:20.000000 first-breaks-picking-0.3.0/first_breaks/utils/__init__.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)      635 2023-05-10 12:43:20.000000 first-breaks-picking-0.3.0/first_breaks/utils/debug.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)     5833 2023-07-18 16:46:46.000000 first-breaks-picking-0.3.0/first_breaks/utils/utils.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)     3815 2023-05-26 13:27:32.000000 first-breaks-picking-0.3.0/first_breaks/utils/visualizations.py
-drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-07-21 10:13:22.999121 first-breaks-picking-0.3.0/first_breaks_picking.egg-info/
--rw-rw-r--   0 daloro    (1000) daloro    (1000)    24006 2023-07-21 10:13:22.000000 first-breaks-picking-0.3.0/first_breaks_picking.egg-info/PKG-INFO
--rw-rw-r--   0 daloro    (1000) daloro    (1000)     1683 2023-07-21 10:13:22.000000 first-breaks-picking-0.3.0/first_breaks_picking.egg-info/SOURCES.txt
--rw-rw-r--   0 daloro    (1000) daloro    (1000)        1 2023-07-21 10:13:22.000000 first-breaks-picking-0.3.0/first_breaks_picking.egg-info/dependency_links.txt
--rw-rw-r--   0 daloro    (1000) daloro    (1000)       71 2023-07-21 10:13:22.000000 first-breaks-picking-0.3.0/first_breaks_picking.egg-info/entry_points.txt
--rw-rw-r--   0 daloro    (1000) daloro    (1000)      184 2023-07-21 10:13:22.000000 first-breaks-picking-0.3.0/first_breaks_picking.egg-info/requires.txt
--rw-rw-r--   0 daloro    (1000) daloro    (1000)       19 2023-07-21 10:13:22.000000 first-breaks-picking-0.3.0/first_breaks_picking.egg-info/top_level.txt
--rw-r--r--   0 daloro    (1000) daloro    (1000)      337 2023-07-21 10:13:22.999121 first-breaks-picking-0.3.0/setup.cfg
--rw-rw-r--   0 daloro    (1000) daloro    (1000)     2230 2023-07-21 10:12:38.000000 first-breaks-picking-0.3.0/setup.py
-drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-07-21 10:13:22.999121 first-breaks-picking-0.3.0/tests/
--rw-r--r--   0 daloro    (1000) daloro    (1000)      330 2023-07-10 12:37:21.000000 first-breaks-picking-0.3.0/tests/test_demo_sgy.py
-drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-07-21 10:13:22.999121 first-breaks-picking-0.3.0/tests/test_desktop/
--rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-07-10 12:37:21.000000 first-breaks-picking-0.3.0/tests/test_desktop/__init__.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-07-10 12:37:21.000000 first-breaks-picking-0.3.0/tests/test_desktop/test_graph.py
-drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-07-21 10:13:22.999121 first-breaks-picking-0.3.0/tests/test_picking/
--rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-07-10 12:37:21.000000 first-breaks-picking-0.3.0/tests/test_picking/__init__.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)     1288 2023-07-10 12:37:21.000000 first-breaks-picking-0.3.0/tests/test_picking/test_picker.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)     3329 2023-07-10 12:37:21.000000 first-breaks-picking-0.3.0/tests/test_picking/test_task.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)     1467 2023-07-18 16:41:44.000000 first-breaks-picking-0.3.0/tests/test_readme_examples.py
-drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-07-21 10:13:22.999121 first-breaks-picking-0.3.0/tests/test_sgy/
--rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-07-10 12:37:21.000000 first-breaks-picking-0.3.0/tests/test_sgy/__init__.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)     1859 2023-07-18 12:38:11.000000 first-breaks-picking-0.3.0/tests/test_sgy/test_reader.py
+drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-07-19 05:44:41.852779 first-breaks-picking-0.3.0b0/
+-rw-r--r--   0 daloro    (1000) daloro    (1000)    11357 2023-05-10 12:43:20.000000 first-breaks-picking-0.3.0b0/LICENSE
+-rw-rw-r--   0 daloro    (1000) daloro    (1000)    24007 2023-07-19 05:44:41.852779 first-breaks-picking-0.3.0b0/PKG-INFO
+-rw-r--r--   0 daloro    (1000) daloro    (1000)    22791 2023-07-19 05:43:43.000000 first-breaks-picking-0.3.0b0/README.md
+drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-07-19 05:44:41.852779 first-breaks-picking-0.3.0b0/first_breaks/
+-rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-05-10 12:43:20.000000 first-breaks-picking-0.3.0b0/first_breaks/__init__.py
+drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-07-19 05:44:41.852779 first-breaks-picking-0.3.0b0/first_breaks/_pytorch/
+drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-07-19 05:44:41.852779 first-breaks-picking-0.3.0b0/first_breaks/_pytorch/models/
+-rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-07-10 12:37:21.000000 first-breaks-picking-0.3.0b0/first_breaks/_pytorch/models/__init__.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)     5730 2023-07-10 12:37:21.000000 first-breaks-picking-0.3.0b0/first_breaks/_pytorch/models/unet3plus.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)      352 2023-06-12 06:38:44.000000 first-breaks-picking-0.3.0b0/first_breaks/cli.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)     1171 2023-07-10 12:37:21.000000 first-breaks-picking-0.3.0b0/first_breaks/const.py
+drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-07-19 05:44:41.852779 first-breaks-picking-0.3.0b0/first_breaks/data_models/
+-rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-07-17 07:07:08.000000 first-breaks-picking-0.3.0b0/first_breaks/data_models/__init__.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)     1701 2023-07-18 13:44:34.000000 first-breaks-picking-0.3.0b0/first_breaks/data_models/dependent.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)     2090 2023-07-18 17:00:55.000000 first-breaks-picking-0.3.0b0/first_breaks/data_models/independent.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)      441 2023-07-18 13:44:34.000000 first-breaks-picking-0.3.0b0/first_breaks/data_models/initialised_defaults.py
+drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-07-19 05:44:41.852779 first-breaks-picking-0.3.0b0/first_breaks/desktop/
+-rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-05-10 12:43:20.000000 first-breaks-picking-0.3.0b0/first_breaks/desktop/__init__.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)     5525 2023-07-18 16:48:46.000000 first-breaks-picking-0.3.0b0/first_breaks/desktop/byte_encode_unit_widget.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)     1903 2023-07-18 16:49:22.000000 first-breaks-picking-0.3.0b0/first_breaks/desktop/combobox_with_mapping.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)    18931 2023-07-18 13:48:53.000000 first-breaks-picking-0.3.0b0/first_breaks/desktop/graph.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)    20070 2023-07-19 05:38:40.000000 first-breaks-picking-0.3.0b0/first_breaks/desktop/main_gui.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)     6739 2023-07-10 12:37:21.000000 first-breaks-picking-0.3.0b0/first_breaks/desktop/picking_widget.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)     2661 2023-07-18 16:49:29.000000 first-breaks-picking-0.3.0b0/first_breaks/desktop/radioset_widget.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)     3571 2023-07-18 16:49:46.000000 first-breaks-picking-0.3.0b0/first_breaks/desktop/slider_with_values.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)     2700 2023-07-10 12:37:21.000000 first-breaks-picking-0.3.0b0/first_breaks/desktop/threads.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)     4238 2023-07-18 16:49:38.000000 first-breaks-picking-0.3.0b0/first_breaks/desktop/utils.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)     7474 2023-07-18 16:47:54.000000 first-breaks-picking-0.3.0b0/first_breaks/desktop/visualization_settings_widget.py
+drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-07-19 05:44:41.852779 first-breaks-picking-0.3.0b0/first_breaks/picking/
+-rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-05-30 07:39:18.000000 first-breaks-picking-0.3.0b0/first_breaks/picking/__init__.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)      955 2023-07-10 12:37:21.000000 first-breaks-picking-0.3.0b0/first_breaks/picking/ipicker.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)     4952 2023-07-10 12:37:21.000000 first-breaks-picking-0.3.0b0/first_breaks/picking/picker_onnx.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)     9351 2023-07-18 16:46:26.000000 first-breaks-picking-0.3.0b0/first_breaks/picking/task.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)     2197 2023-07-18 17:00:56.000000 first-breaks-picking-0.3.0b0/first_breaks/picking/utils.py
+drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-07-19 05:44:41.852779 first-breaks-picking-0.3.0b0/first_breaks/sgy/
+-rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-05-10 12:43:20.000000 first-breaks-picking-0.3.0b0/first_breaks/sgy/__init__.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)     8608 2023-07-18 16:49:53.000000 first-breaks-picking-0.3.0b0/first_breaks/sgy/headers.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)    16232 2023-07-18 16:46:38.000000 first-breaks-picking-0.3.0b0/first_breaks/sgy/reader.py
+drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-07-19 05:44:41.852779 first-breaks-picking-0.3.0b0/first_breaks/utils/
+-rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-05-10 12:43:20.000000 first-breaks-picking-0.3.0b0/first_breaks/utils/__init__.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)      635 2023-05-10 12:43:20.000000 first-breaks-picking-0.3.0b0/first_breaks/utils/debug.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)     5833 2023-07-18 16:46:46.000000 first-breaks-picking-0.3.0b0/first_breaks/utils/utils.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)     3815 2023-05-26 13:27:32.000000 first-breaks-picking-0.3.0b0/first_breaks/utils/visualizations.py
+drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-07-19 05:44:41.852779 first-breaks-picking-0.3.0b0/first_breaks_picking.egg-info/
+-rw-rw-r--   0 daloro    (1000) daloro    (1000)    24007 2023-07-19 05:44:41.000000 first-breaks-picking-0.3.0b0/first_breaks_picking.egg-info/PKG-INFO
+-rw-rw-r--   0 daloro    (1000) daloro    (1000)     1683 2023-07-19 05:44:41.000000 first-breaks-picking-0.3.0b0/first_breaks_picking.egg-info/SOURCES.txt
+-rw-rw-r--   0 daloro    (1000) daloro    (1000)        1 2023-07-19 05:44:41.000000 first-breaks-picking-0.3.0b0/first_breaks_picking.egg-info/dependency_links.txt
+-rw-rw-r--   0 daloro    (1000) daloro    (1000)       71 2023-07-19 05:44:41.000000 first-breaks-picking-0.3.0b0/first_breaks_picking.egg-info/entry_points.txt
+-rw-rw-r--   0 daloro    (1000) daloro    (1000)      184 2023-07-19 05:44:41.000000 first-breaks-picking-0.3.0b0/first_breaks_picking.egg-info/requires.txt
+-rw-rw-r--   0 daloro    (1000) daloro    (1000)       19 2023-07-19 05:44:41.000000 first-breaks-picking-0.3.0b0/first_breaks_picking.egg-info/top_level.txt
+-rw-r--r--   0 daloro    (1000) daloro    (1000)      337 2023-07-19 05:44:41.852779 first-breaks-picking-0.3.0b0/setup.cfg
+-rw-rw-r--   0 daloro    (1000) daloro    (1000)     2238 2023-07-18 16:41:29.000000 first-breaks-picking-0.3.0b0/setup.py
+drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-07-19 05:44:41.852779 first-breaks-picking-0.3.0b0/tests/
+-rw-r--r--   0 daloro    (1000) daloro    (1000)      330 2023-07-10 12:37:21.000000 first-breaks-picking-0.3.0b0/tests/test_demo_sgy.py
+drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-07-19 05:44:41.852779 first-breaks-picking-0.3.0b0/tests/test_desktop/
+-rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-07-10 12:37:21.000000 first-breaks-picking-0.3.0b0/tests/test_desktop/__init__.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-07-10 12:37:21.000000 first-breaks-picking-0.3.0b0/tests/test_desktop/test_graph.py
+drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-07-19 05:44:41.852779 first-breaks-picking-0.3.0b0/tests/test_picking/
+-rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-07-10 12:37:21.000000 first-breaks-picking-0.3.0b0/tests/test_picking/__init__.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)     1288 2023-07-10 12:37:21.000000 first-breaks-picking-0.3.0b0/tests/test_picking/test_picker.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)     3329 2023-07-10 12:37:21.000000 first-breaks-picking-0.3.0b0/tests/test_picking/test_task.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)     1467 2023-07-18 16:41:44.000000 first-breaks-picking-0.3.0b0/tests/test_readme_examples.py
+drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-07-19 05:44:41.852779 first-breaks-picking-0.3.0b0/tests/test_sgy/
+-rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-07-10 12:37:21.000000 first-breaks-picking-0.3.0b0/tests/test_sgy/__init__.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)     1859 2023-07-18 12:38:11.000000 first-breaks-picking-0.3.0b0/tests/test_sgy/test_reader.py
```

### Comparing `first-breaks-picking-0.3.0/LICENSE` & `first-breaks-picking-0.3.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.3.0/PKG-INFO` & `first-breaks-picking-0.3.0b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: first-breaks-picking
-Version: 0.3.0
+Version: 0.3.0b0
 Summary: Tool for picking first breaks in seismic gather
 Home-page: https://github.com/DaloroAT/first_breaks_picking
 Author: Aleksei Tarasov
 Author-email: aleksei.v.tarasov@gmail.com
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/DaloroAT/first_breaks_picking
 Keywords: seismic,first-breaks,computer-vision,deep-learning,segmentation,data-science
@@ -17,15 +17,15 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.8,<3.9
 Description-Content-Type: text/markdown
 Provides-Extra: gpu
 License-File: LICENSE
 
 # First breaks picking
 This project is devoted to pick waves that are the first to be detected on a seismogram (first breaks, first arrivals).
 Traditionally, this procedure is performed manually. When processing field data, the number of picks reaches hundreds of
```

### Comparing `first-breaks-picking-0.3.0/README.md` & `first-breaks-picking-0.3.0b0/README.md`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.3.0/first_breaks/_pytorch/models/unet3plus.py` & `first-breaks-picking-0.3.0b0/first_breaks/_pytorch/models/unet3plus.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.3.0/first_breaks/const.py` & `first-breaks-picking-0.3.0b0/first_breaks/const.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.3.0/first_breaks/data_models/dependent.py` & `first-breaks-picking-0.3.0b0/first_breaks/data_models/dependent.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.3.0/first_breaks/data_models/independent.py` & `first-breaks-picking-0.3.0b0/first_breaks/data_models/independent.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.3.0/first_breaks/desktop/byte_encode_unit_widget.py` & `first-breaks-picking-0.3.0b0/first_breaks/desktop/byte_encode_unit_widget.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.3.0/first_breaks/desktop/combobox_with_mapping.py` & `first-breaks-picking-0.3.0b0/first_breaks/desktop/combobox_with_mapping.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.3.0/first_breaks/desktop/graph.py` & `first-breaks-picking-0.3.0b0/first_breaks/desktop/graph.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.3.0/first_breaks/desktop/main_gui.py` & `first-breaks-picking-0.3.0b0/first_breaks/desktop/main_gui.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.3.0/first_breaks/desktop/picking_widget.py` & `first-breaks-picking-0.3.0b0/first_breaks/desktop/picking_widget.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.3.0/first_breaks/desktop/radioset_widget.py` & `first-breaks-picking-0.3.0b0/first_breaks/desktop/radioset_widget.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.3.0/first_breaks/desktop/slider_with_values.py` & `first-breaks-picking-0.3.0b0/first_breaks/desktop/slider_with_values.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.3.0/first_breaks/desktop/threads.py` & `first-breaks-picking-0.3.0b0/first_breaks/desktop/threads.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.3.0/first_breaks/desktop/utils.py` & `first-breaks-picking-0.3.0b0/first_breaks/desktop/utils.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.3.0/first_breaks/desktop/visualization_settings_widget.py` & `first-breaks-picking-0.3.0b0/first_breaks/desktop/visualization_settings_widget.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.3.0/first_breaks/picking/ipicker.py` & `first-breaks-picking-0.3.0b0/first_breaks/picking/ipicker.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.3.0/first_breaks/picking/picker_onnx.py` & `first-breaks-picking-0.3.0b0/first_breaks/picking/picker_onnx.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.3.0/first_breaks/picking/task.py` & `first-breaks-picking-0.3.0b0/first_breaks/picking/task.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.3.0/first_breaks/picking/utils.py` & `first-breaks-picking-0.3.0b0/first_breaks/picking/utils.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.3.0/first_breaks/sgy/headers.py` & `first-breaks-picking-0.3.0b0/first_breaks/sgy/headers.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.3.0/first_breaks/sgy/reader.py` & `first-breaks-picking-0.3.0b0/first_breaks/sgy/reader.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.3.0/first_breaks/utils/debug.py` & `first-breaks-picking-0.3.0b0/first_breaks/utils/debug.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.3.0/first_breaks/utils/utils.py` & `first-breaks-picking-0.3.0b0/first_breaks/utils/utils.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.3.0/first_breaks/utils/visualizations.py` & `first-breaks-picking-0.3.0b0/first_breaks/utils/visualizations.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.3.0/first_breaks_picking.egg-info/PKG-INFO` & `first-breaks-picking-0.3.0b0/first_breaks_picking.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: first-breaks-picking
-Version: 0.3.0
+Version: 0.3.0b0
 Summary: Tool for picking first breaks in seismic gather
 Home-page: https://github.com/DaloroAT/first_breaks_picking
 Author: Aleksei Tarasov
 Author-email: aleksei.v.tarasov@gmail.com
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/DaloroAT/first_breaks_picking
 Keywords: seismic,first-breaks,computer-vision,deep-learning,segmentation,data-science
@@ -17,15 +17,15 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.8,<3.9
 Description-Content-Type: text/markdown
 Provides-Extra: gpu
 License-File: LICENSE
 
 # First breaks picking
 This project is devoted to pick waves that are the first to be detected on a seismogram (first breaks, first arrivals).
 Traditionally, this procedure is performed manually. When processing field data, the number of picks reaches hundreds of
```

### Comparing `first-breaks-picking-0.3.0/first_breaks_picking.egg-info/SOURCES.txt` & `first-breaks-picking-0.3.0b0/first_breaks_picking.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.3.0/setup.py` & `first-breaks-picking-0.3.0b0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 basic_reqs = load_requirements("requirements/basic.txt")
 cpu_reqs = load_requirements("requirements/cpu.txt")
 gpu_extra_reqs = load_requirements("requirements/gpu.txt")
 
 
 setup(
     # technical things
-    version="0.3.0",
+    version="0.3.0b",
     packages=find_packages(exclude=['data', 'docs', 'legacy', 'first_breaks._pytorch', 'tests', "requirements"]),
-    python_requires=">=3.8,<3.11",
+    python_requires=">=3.8,<3.9",  # todo
     install_requires=basic_reqs + cpu_reqs,
     extras_require={'gpu': gpu_extra_reqs},
     long_description=Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     entry_points={
             "console_scripts": [
                 "first-breaks-picking=first_breaks.cli:cli_commands"
```

### Comparing `first-breaks-picking-0.3.0/tests/test_picking/test_picker.py` & `first-breaks-picking-0.3.0b0/tests/test_picking/test_picker.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.3.0/tests/test_picking/test_task.py` & `first-breaks-picking-0.3.0b0/tests/test_picking/test_task.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.3.0/tests/test_readme_examples.py` & `first-breaks-picking-0.3.0b0/tests/test_readme_examples.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.3.0/tests/test_sgy/test_reader.py` & `first-breaks-picking-0.3.0b0/tests/test_sgy/test_reader.py`

 * *Files identical despite different names*

