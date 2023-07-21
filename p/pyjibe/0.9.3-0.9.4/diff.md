# Comparing `tmp/pyjibe-0.9.3.tar.gz` & `tmp/pyjibe-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjibe-0.9.3.tar", last modified: Fri Jul  9 21:22:01 2021, max compression
+gzip compressed data, was "pyjibe-0.9.4.tar", last modified: Tue Aug  3 21:07:43 2021, max compression
```

## Comparing `pyjibe-0.9.3.tar` & `pyjibe-0.9.4.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-07-09 21:22:01.769306 pyjibe-0.9.3/
--rw-r--r--   0 runner     (501) staff       (20)     8193 2021-07-09 21:19:00.000000 pyjibe-0.9.3/CHANGELOG
--rw-r--r--   0 runner     (501) staff       (20)    35149 2021-07-09 21:19:00.000000 pyjibe-0.9.3/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)      162 2021-07-09 21:19:00.000000 pyjibe-0.9.3/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)     2267 2021-07-09 21:22:01.769503 pyjibe-0.9.3/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     1369 2021-07-09 21:19:00.000000 pyjibe-0.9.3/README.rst
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-07-09 21:22:01.745875 pyjibe-0.9.3/pyjibe/
--rw-r--r--   0 runner     (501) staff       (20)       59 2021-07-09 21:19:03.000000 pyjibe-0.9.3/pyjibe/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1297 2021-07-09 21:19:03.000000 pyjibe-0.9.3/pyjibe/__main__.py
--rw-r--r--   0 runner     (501) staff       (20)     7095 2021-07-09 21:19:03.000000 pyjibe-0.9.3/pyjibe/_version.py
--rw-r--r--   0 runner     (501) staff       (20)       82 2021-07-09 21:21:22.000000 pyjibe-0.9.3/pyjibe/_version_save.py
--rw-r--r--   0 runner     (501) staff       (20)      209 2021-07-09 21:19:03.000000 pyjibe-0.9.3/pyjibe/colormap.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-07-09 21:22:01.758275 pyjibe-0.9.3/pyjibe/fd/
--rw-r--r--   0 runner     (501) staff       (20)       48 2021-07-09 21:19:03.000000 pyjibe-0.9.3/pyjibe/fd/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     3063 2021-07-09 21:19:03.000000 pyjibe-0.9.3/pyjibe/fd/dlg_autosave_design.ui
--rw-r--r--   0 runner     (501) staff       (20)     1975 2021-07-09 21:19:03.000000 pyjibe-0.9.3/pyjibe/fd/dlg_export_vals.py
--rw-r--r--   0 runner     (501) staff       (20)     4897 2021-07-09 21:19:03.000000 pyjibe-0.9.3/pyjibe/fd/dlg_export_vals.ui
--rw-r--r--   0 runner     (501) staff       (20)     6649 2021-07-09 21:19:03.000000 pyjibe-0.9.3/pyjibe/fd/export.py
--rw-r--r--   0 runner     (501) staff       (20)    25059 2021-07-09 21:19:03.000000 pyjibe-0.9.3/pyjibe/fd/main.py
--rw-r--r--   0 runner     (501) staff       (20)    22014 2021-07-09 21:19:03.000000 pyjibe-0.9.3/pyjibe/fd/main.ui
--rw-r--r--   0 runner     (501) staff       (20)     4616 2021-07-09 21:19:03.000000 pyjibe-0.9.3/pyjibe/fd/mpl_edelta.py
--rw-r--r--   0 runner     (501) staff       (20)     6401 2021-07-09 21:19:03.000000 pyjibe-0.9.3/pyjibe/fd/mpl_indent.py
--rw-r--r--   0 runner     (501) staff       (20)     9748 2021-07-09 21:19:03.000000 pyjibe-0.9.3/pyjibe/fd/mpl_qmap.py
--rw-r--r--   0 runner     (501) staff       (20)     3040 2021-07-09 21:19:03.000000 pyjibe-0.9.3/pyjibe/fd/rating_base.py
--rw-r--r--   0 runner     (501) staff       (20)     2762 2021-07-09 21:19:03.000000 pyjibe-0.9.3/pyjibe/fd/rating_iface.py
--rw-r--r--   0 runner     (501) staff       (20)     5195 2021-07-09 21:19:03.000000 pyjibe-0.9.3/pyjibe/fd/rating_iface.ui
--rw-r--r--   0 runner     (501) staff       (20)     3428 2021-07-09 21:19:03.000000 pyjibe-0.9.3/pyjibe/fd/tab_edelta.py
--rw-r--r--   0 runner     (501) staff       (20)     4498 2021-07-09 21:19:03.000000 pyjibe-0.9.3/pyjibe/fd/tab_edelta.ui
--rw-r--r--   0 runner     (501) staff       (20)    22156 2021-07-09 21:19:04.000000 pyjibe-0.9.3/pyjibe/fd/tab_fit.py
--rw-r--r--   0 runner     (501) staff       (20)    27923 2021-07-09 21:19:04.000000 pyjibe-0.9.3/pyjibe/fd/tab_fit.ui
--rw-r--r--   0 runner     (501) staff       (20)     3471 2021-07-09 21:19:04.000000 pyjibe-0.9.3/pyjibe/fd/tab_info.py
--rw-r--r--   0 runner     (501) staff       (20)     1551 2021-07-09 21:19:04.000000 pyjibe-0.9.3/pyjibe/fd/tab_info.ui
--rw-r--r--   0 runner     (501) staff       (20)     3352 2021-07-09 21:19:04.000000 pyjibe-0.9.3/pyjibe/fd/tab_preprocess.py
--rw-r--r--   0 runner     (501) staff       (20)     6874 2021-07-09 21:19:04.000000 pyjibe-0.9.3/pyjibe/fd/tab_preprocess.ui
--rw-r--r--   0 runner     (501) staff       (20)     6424 2021-07-09 21:19:04.000000 pyjibe-0.9.3/pyjibe/fd/tab_qmap.py
--rw-r--r--   0 runner     (501) staff       (20)     4384 2021-07-09 21:19:04.000000 pyjibe-0.9.3/pyjibe/fd/tab_qmap.ui
--rw-r--r--   0 runner     (501) staff       (20)     1470 2021-07-09 21:19:04.000000 pyjibe-0.9.3/pyjibe/fd/widget_fdist.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-07-09 21:22:01.761235 pyjibe-0.9.3/pyjibe/head/
--rw-r--r--   0 runner     (501) staff       (20)       39 2021-07-09 21:19:04.000000 pyjibe-0.9.3/pyjibe/head/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-07-09 21:22:01.762874 pyjibe-0.9.3/pyjibe/head/custom_widgets/
--rw-r--r--   0 runner     (501) staff       (20)      275 2021-07-09 21:19:04.000000 pyjibe-0.9.3/pyjibe/head/custom_widgets/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1473 2021-07-09 21:19:04.000000 pyjibe-0.9.3/pyjibe/head/custom_widgets/dirdialog_multiselect.py
--rw-r--r--   0 runner     (501) staff       (20)     3323 2021-07-09 21:19:04.000000 pyjibe-0.9.3/pyjibe/head/custom_widgets/mpl_navigation_toolbar_icons.py
--rw-r--r--   0 runner     (501) staff       (20)     1069 2021-07-09 21:19:04.000000 pyjibe-0.9.3/pyjibe/head/custom_widgets/wait_cursor.py
--rw-r--r--   0 runner     (501) staff       (20)     5669 2021-07-09 21:19:04.000000 pyjibe-0.9.3/pyjibe/head/dlg_tool_convert.py
--rw-r--r--   0 runner     (501) staff       (20)     8182 2021-07-09 21:19:04.000000 pyjibe-0.9.3/pyjibe/head/dlg_tool_convert.ui
--rw-r--r--   0 runner     (501) staff       (20)     2457 2021-07-09 21:19:04.000000 pyjibe-0.9.3/pyjibe/head/infdoubleslider.py
--rw-r--r--   0 runner     (501) staff       (20)     3276 2021-07-09 21:19:04.000000 pyjibe-0.9.3/pyjibe/head/infdoublespinbox.py
--rw-r--r--   0 runner     (501) staff       (20)    10926 2021-07-09 21:19:04.000000 pyjibe-0.9.3/pyjibe/head/main.py
--rw-r--r--   0 runner     (501) staff       (20)     5302 2021-07-09 21:19:04.000000 pyjibe-0.9.3/pyjibe/head/main.ui
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-07-09 21:22:01.764519 pyjibe-0.9.3/pyjibe/img/
--rw-r--r--   0 runner     (501) staff       (20)     2107 2021-07-09 21:19:04.000000 pyjibe-0.9.3/pyjibe/img/icon.png
--rw-r--r--   0 runner     (501) staff       (20)     1159 2021-07-09 21:19:04.000000 pyjibe-0.9.3/pyjibe/img/savedat_large.png
--rw-r--r--   0 runner     (501) staff       (20)     1241 2021-07-09 21:19:04.000000 pyjibe-0.9.3/pyjibe/img/saveimg_large.png
--rw-r--r--   0 runner     (501) staff       (20)    11393 2021-07-09 21:19:04.000000 pyjibe-0.9.3/pyjibe/img/splash.png
--rw-r--r--   0 runner     (501) staff       (20)      347 2021-07-09 21:19:04.000000 pyjibe-0.9.3/pyjibe/registry.py
--rw-r--r--   0 runner     (501) staff       (20)     3084 2021-07-09 21:19:04.000000 pyjibe-0.9.3/pyjibe/units.py
--rw-r--r--   0 runner     (501) staff       (20)      791 2021-07-09 21:19:04.000000 pyjibe-0.9.3/pyjibe/util.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-07-09 21:22:01.748237 pyjibe-0.9.3/pyjibe.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     2267 2021-07-09 21:22:01.000000 pyjibe-0.9.3/pyjibe.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     1719 2021-07-09 21:22:01.000000 pyjibe-0.9.3/pyjibe.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2021-07-09 21:22:01.000000 pyjibe-0.9.3/pyjibe.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)       45 2021-07-09 21:22:01.000000 pyjibe-0.9.3/pyjibe.egg-info/entry_points.txt
--rw-r--r--   0 runner     (501) staff       (20)       53 2021-07-09 21:22:01.000000 pyjibe-0.9.3/pyjibe.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)        7 2021-07-09 21:22:01.000000 pyjibe-0.9.3/pyjibe.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)       73 2021-07-09 21:22:01.770264 pyjibe-0.9.3/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)     1321 2021-07-09 21:19:04.000000 pyjibe-0.9.3/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-07-09 21:22:01.768077 pyjibe-0.9.3/tests/
--rw-r--r--   0 runner     (501) staff       (20)      522 2021-07-09 21:19:04.000000 pyjibe-0.9.3/tests/conftest.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-07-09 21:22:01.768862 pyjibe-0.9.3/tests/data/
--rw-r--r--   0 runner     (501) staff       (20)    11993 2021-07-09 21:19:04.000000 pyjibe-0.9.3/tests/data/invalid_dataset.jpk-force
--rw-r--r--   0 runner     (501) staff       (20)    22266 2021-07-09 21:19:04.000000 pyjibe-0.9.3/tests/data/spot3-0192.jpk-force
--rw-r--r--   0 runner     (501) staff       (20)      417 2021-07-09 21:19:04.000000 pyjibe-0.9.3/tests/helpers.py
--rw-r--r--   0 runner     (501) staff       (20)     2026 2021-07-09 21:19:04.000000 pyjibe-0.9.3/tests/test_fd_base.py
--rw-r--r--   0 runner     (501) staff       (20)    10874 2021-07-09 21:19:04.000000 pyjibe-0.9.3/tests/test_fd_fit.py
--rw-r--r--   0 runner     (501) staff       (20)     5324 2021-07-09 21:19:04.000000 pyjibe-0.9.3/tests/test_fd_fit_model_expr.py
--rw-r--r--   0 runner     (501) staff       (20)      584 2021-07-09 21:19:04.000000 pyjibe-0.9.3/tests/test_fd_qmap.py
--rw-r--r--   0 runner     (501) staff       (20)     1714 2021-07-09 21:19:04.000000 pyjibe-0.9.3/tests/test_fd_rater.py
--rw-r--r--   0 runner     (501) staff       (20)      286 2021-07-09 21:19:04.000000 pyjibe-0.9.3/tests/test_fd_tab_info.py
--rw-r--r--   0 runner     (501) staff       (20)     6095 2021-07-09 21:19:04.000000 pyjibe-0.9.3/tests/test_head.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-08-03 21:07:43.526043 pyjibe-0.9.4/
+-rw-r--r--   0 runner     (501) staff       (20)     8426 2021-08-03 21:06:44.000000 pyjibe-0.9.4/CHANGELOG
+-rw-r--r--   0 runner     (501) staff       (20)    35149 2021-08-03 21:06:44.000000 pyjibe-0.9.4/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)      162 2021-08-03 21:06:44.000000 pyjibe-0.9.4/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)     2267 2021-08-03 21:07:43.526248 pyjibe-0.9.4/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     1369 2021-08-03 21:06:44.000000 pyjibe-0.9.4/README.rst
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-08-03 21:07:43.490798 pyjibe-0.9.4/pyjibe/
+-rw-r--r--   0 runner     (501) staff       (20)       59 2021-08-03 21:06:44.000000 pyjibe-0.9.4/pyjibe/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1297 2021-08-03 21:06:44.000000 pyjibe-0.9.4/pyjibe/__main__.py
+-rw-r--r--   0 runner     (501) staff       (20)     7095 2021-08-03 21:06:44.000000 pyjibe-0.9.4/pyjibe/_version.py
+-rw-r--r--   0 runner     (501) staff       (20)       82 2021-08-03 21:06:54.000000 pyjibe-0.9.4/pyjibe/_version_save.py
+-rw-r--r--   0 runner     (501) staff       (20)      209 2021-08-03 21:06:44.000000 pyjibe-0.9.4/pyjibe/colormap.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-08-03 21:07:43.514055 pyjibe-0.9.4/pyjibe/fd/
+-rw-r--r--   0 runner     (501) staff       (20)       48 2021-08-03 21:06:44.000000 pyjibe-0.9.4/pyjibe/fd/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     3063 2021-08-03 21:06:44.000000 pyjibe-0.9.4/pyjibe/fd/dlg_autosave_design.ui
+-rw-r--r--   0 runner     (501) staff       (20)     1975 2021-08-03 21:06:44.000000 pyjibe-0.9.4/pyjibe/fd/dlg_export_vals.py
+-rw-r--r--   0 runner     (501) staff       (20)     4897 2021-08-03 21:06:44.000000 pyjibe-0.9.4/pyjibe/fd/dlg_export_vals.ui
+-rw-r--r--   0 runner     (501) staff       (20)     6649 2021-08-03 21:06:44.000000 pyjibe-0.9.4/pyjibe/fd/export.py
+-rw-r--r--   0 runner     (501) staff       (20)    25059 2021-08-03 21:06:44.000000 pyjibe-0.9.4/pyjibe/fd/main.py
+-rw-r--r--   0 runner     (501) staff       (20)    22014 2021-08-03 21:06:44.000000 pyjibe-0.9.4/pyjibe/fd/main.ui
+-rw-r--r--   0 runner     (501) staff       (20)     4616 2021-08-03 21:06:44.000000 pyjibe-0.9.4/pyjibe/fd/mpl_edelta.py
+-rw-r--r--   0 runner     (501) staff       (20)     6693 2021-08-03 21:06:44.000000 pyjibe-0.9.4/pyjibe/fd/mpl_indent.py
+-rw-r--r--   0 runner     (501) staff       (20)     9748 2021-08-03 21:06:44.000000 pyjibe-0.9.4/pyjibe/fd/mpl_qmap.py
+-rw-r--r--   0 runner     (501) staff       (20)     3040 2021-08-03 21:06:44.000000 pyjibe-0.9.4/pyjibe/fd/rating_base.py
+-rw-r--r--   0 runner     (501) staff       (20)     2762 2021-08-03 21:06:44.000000 pyjibe-0.9.4/pyjibe/fd/rating_iface.py
+-rw-r--r--   0 runner     (501) staff       (20)     5195 2021-08-03 21:06:44.000000 pyjibe-0.9.4/pyjibe/fd/rating_iface.ui
+-rw-r--r--   0 runner     (501) staff       (20)     3376 2021-08-03 21:06:44.000000 pyjibe-0.9.4/pyjibe/fd/tab_edelta.py
+-rw-r--r--   0 runner     (501) staff       (20)     4498 2021-08-03 21:06:44.000000 pyjibe-0.9.4/pyjibe/fd/tab_edelta.ui
+-rw-r--r--   0 runner     (501) staff       (20)    22411 2021-08-03 21:06:44.000000 pyjibe-0.9.4/pyjibe/fd/tab_fit.py
+-rw-r--r--   0 runner     (501) staff       (20)    27923 2021-08-03 21:06:44.000000 pyjibe-0.9.4/pyjibe/fd/tab_fit.ui
+-rw-r--r--   0 runner     (501) staff       (20)     3471 2021-08-03 21:06:44.000000 pyjibe-0.9.4/pyjibe/fd/tab_info.py
+-rw-r--r--   0 runner     (501) staff       (20)     1551 2021-08-03 21:06:44.000000 pyjibe-0.9.4/pyjibe/fd/tab_info.ui
+-rw-r--r--   0 runner     (501) staff       (20)     3352 2021-08-03 21:06:44.000000 pyjibe-0.9.4/pyjibe/fd/tab_preprocess.py
+-rw-r--r--   0 runner     (501) staff       (20)     6874 2021-08-03 21:06:44.000000 pyjibe-0.9.4/pyjibe/fd/tab_preprocess.ui
+-rw-r--r--   0 runner     (501) staff       (20)     6424 2021-08-03 21:06:44.000000 pyjibe-0.9.4/pyjibe/fd/tab_qmap.py
+-rw-r--r--   0 runner     (501) staff       (20)     4384 2021-08-03 21:06:44.000000 pyjibe-0.9.4/pyjibe/fd/tab_qmap.ui
+-rw-r--r--   0 runner     (501) staff       (20)     1470 2021-08-03 21:06:44.000000 pyjibe-0.9.4/pyjibe/fd/widget_fdist.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-08-03 21:07:43.517122 pyjibe-0.9.4/pyjibe/head/
+-rw-r--r--   0 runner     (501) staff       (20)       39 2021-08-03 21:06:44.000000 pyjibe-0.9.4/pyjibe/head/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-08-03 21:07:43.518657 pyjibe-0.9.4/pyjibe/head/custom_widgets/
+-rw-r--r--   0 runner     (501) staff       (20)      275 2021-08-03 21:06:44.000000 pyjibe-0.9.4/pyjibe/head/custom_widgets/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1473 2021-08-03 21:06:44.000000 pyjibe-0.9.4/pyjibe/head/custom_widgets/dirdialog_multiselect.py
+-rw-r--r--   0 runner     (501) staff       (20)     3323 2021-08-03 21:06:44.000000 pyjibe-0.9.4/pyjibe/head/custom_widgets/mpl_navigation_toolbar_icons.py
+-rw-r--r--   0 runner     (501) staff       (20)     1069 2021-08-03 21:06:44.000000 pyjibe-0.9.4/pyjibe/head/custom_widgets/wait_cursor.py
+-rw-r--r--   0 runner     (501) staff       (20)     5669 2021-08-03 21:06:44.000000 pyjibe-0.9.4/pyjibe/head/dlg_tool_convert.py
+-rw-r--r--   0 runner     (501) staff       (20)     8182 2021-08-03 21:06:44.000000 pyjibe-0.9.4/pyjibe/head/dlg_tool_convert.ui
+-rw-r--r--   0 runner     (501) staff       (20)     2457 2021-08-03 21:06:44.000000 pyjibe-0.9.4/pyjibe/head/infdoubleslider.py
+-rw-r--r--   0 runner     (501) staff       (20)     3276 2021-08-03 21:06:44.000000 pyjibe-0.9.4/pyjibe/head/infdoublespinbox.py
+-rw-r--r--   0 runner     (501) staff       (20)    10926 2021-08-03 21:06:44.000000 pyjibe-0.9.4/pyjibe/head/main.py
+-rw-r--r--   0 runner     (501) staff       (20)     5302 2021-08-03 21:06:44.000000 pyjibe-0.9.4/pyjibe/head/main.ui
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-08-03 21:07:43.520773 pyjibe-0.9.4/pyjibe/img/
+-rw-r--r--   0 runner     (501) staff       (20)     2107 2021-08-03 21:06:44.000000 pyjibe-0.9.4/pyjibe/img/icon.png
+-rw-r--r--   0 runner     (501) staff       (20)     1159 2021-08-03 21:06:44.000000 pyjibe-0.9.4/pyjibe/img/savedat_large.png
+-rw-r--r--   0 runner     (501) staff       (20)     1241 2021-08-03 21:06:44.000000 pyjibe-0.9.4/pyjibe/img/saveimg_large.png
+-rw-r--r--   0 runner     (501) staff       (20)    11393 2021-08-03 21:06:44.000000 pyjibe-0.9.4/pyjibe/img/splash.png
+-rw-r--r--   0 runner     (501) staff       (20)      347 2021-08-03 21:06:44.000000 pyjibe-0.9.4/pyjibe/registry.py
+-rw-r--r--   0 runner     (501) staff       (20)     3084 2021-08-03 21:06:44.000000 pyjibe-0.9.4/pyjibe/units.py
+-rw-r--r--   0 runner     (501) staff       (20)      791 2021-08-03 21:06:44.000000 pyjibe-0.9.4/pyjibe/util.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-08-03 21:07:43.493099 pyjibe-0.9.4/pyjibe.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     2267 2021-08-03 21:07:41.000000 pyjibe-0.9.4/pyjibe.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     1719 2021-08-03 21:07:41.000000 pyjibe-0.9.4/pyjibe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2021-08-03 21:07:41.000000 pyjibe-0.9.4/pyjibe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)       45 2021-08-03 21:07:41.000000 pyjibe-0.9.4/pyjibe.egg-info/entry_points.txt
+-rw-r--r--   0 runner     (501) staff       (20)       53 2021-08-03 21:07:41.000000 pyjibe-0.9.4/pyjibe.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)        7 2021-08-03 21:07:41.000000 pyjibe-0.9.4/pyjibe.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)       73 2021-08-03 21:07:43.526829 pyjibe-0.9.4/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)     1321 2021-08-03 21:06:44.000000 pyjibe-0.9.4/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-08-03 21:07:43.524761 pyjibe-0.9.4/tests/
+-rw-r--r--   0 runner     (501) staff       (20)      522 2021-08-03 21:06:44.000000 pyjibe-0.9.4/tests/conftest.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-08-03 21:07:43.525576 pyjibe-0.9.4/tests/data/
+-rw-r--r--   0 runner     (501) staff       (20)    11993 2021-08-03 21:06:44.000000 pyjibe-0.9.4/tests/data/invalid_dataset.jpk-force
+-rw-r--r--   0 runner     (501) staff       (20)    22266 2021-08-03 21:06:44.000000 pyjibe-0.9.4/tests/data/spot3-0192.jpk-force
+-rw-r--r--   0 runner     (501) staff       (20)      417 2021-08-03 21:06:44.000000 pyjibe-0.9.4/tests/helpers.py
+-rw-r--r--   0 runner     (501) staff       (20)     2026 2021-08-03 21:06:44.000000 pyjibe-0.9.4/tests/test_fd_base.py
+-rw-r--r--   0 runner     (501) staff       (20)    10874 2021-08-03 21:06:44.000000 pyjibe-0.9.4/tests/test_fd_fit.py
+-rw-r--r--   0 runner     (501) staff       (20)     5324 2021-08-03 21:06:44.000000 pyjibe-0.9.4/tests/test_fd_fit_model_expr.py
+-rw-r--r--   0 runner     (501) staff       (20)      584 2021-08-03 21:06:44.000000 pyjibe-0.9.4/tests/test_fd_qmap.py
+-rw-r--r--   0 runner     (501) staff       (20)     1714 2021-08-03 21:06:44.000000 pyjibe-0.9.4/tests/test_fd_rater.py
+-rw-r--r--   0 runner     (501) staff       (20)      286 2021-08-03 21:06:44.000000 pyjibe-0.9.4/tests/test_fd_tab_info.py
+-rw-r--r--   0 runner     (501) staff       (20)     6095 2021-08-03 21:06:44.000000 pyjibe-0.9.4/tests/test_head.py
```

### Comparing `pyjibe-0.9.3/CHANGELOG` & `pyjibe-0.9.4/CHANGELOG`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+0.9.4
+ - enh: only show exact sneddon model "sneddon_spher" in developer
+   mode to avoid confusion
+ - setup: bump afmformats from 0.15.0 to 0.16.0 (improve support for
+   AFM workshop data)
+ - setup: bump nanite from 1.7.6 to 2.0.0
 0.9.3
  - fix: possible fix for TypeError in InfDoubleSpinBox
  - setup: bump afmformats from 0.14.3 to 0.15.0 as well as
    nanite from 1.7.6 to 1.7.8 (requirement for #14)
 0.9.2
  - ref: improve speed when displaying QMap data
  - enh: add developer mode for loading creep-compliance data (#14)
```

### Comparing `pyjibe-0.9.3/LICENSE` & `pyjibe-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjibe-0.9.3/PKG-INFO` & `pyjibe-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pyjibe
-Version: 0.9.3
+Version: 0.9.4
 Summary: Graphical user interface for Bio-AFM analysis
 Home-page: https://github.com/AFM-analysis/PyJibe
 Author: Paul Müller
 Author-email: dev@craban.de
 License: GPL v3
 Description: |PyJibe|
         ========
```

### Comparing `pyjibe-0.9.3/README.rst` & `pyjibe-0.9.4/README.rst`

 * *Files identical despite different names*

### Comparing `pyjibe-0.9.3/pyjibe/__main__.py` & `pyjibe-0.9.4/pyjibe/__main__.py`

 * *Files identical despite different names*

### Comparing `pyjibe-0.9.3/pyjibe/_version.py` & `pyjibe-0.9.4/pyjibe/_version.py`

 * *Files identical despite different names*

### Comparing `pyjibe-0.9.3/pyjibe/fd/dlg_autosave_design.ui` & `pyjibe-0.9.4/pyjibe/fd/dlg_autosave_design.ui`

 * *Files identical despite different names*

### Comparing `pyjibe-0.9.3/pyjibe/fd/dlg_export_vals.py` & `pyjibe-0.9.4/pyjibe/fd/dlg_export_vals.py`

 * *Files identical despite different names*

### Comparing `pyjibe-0.9.3/pyjibe/fd/dlg_export_vals.ui` & `pyjibe-0.9.4/pyjibe/fd/dlg_export_vals.ui`

 * *Files identical despite different names*

### Comparing `pyjibe-0.9.3/pyjibe/fd/export.py` & `pyjibe-0.9.4/pyjibe/fd/export.py`

 * *Files identical despite different names*

### Comparing `pyjibe-0.9.3/pyjibe/fd/main.py` & `pyjibe-0.9.4/pyjibe/fd/main.py`

 * *Files identical despite different names*

### Comparing `pyjibe-0.9.3/pyjibe/fd/main.ui` & `pyjibe-0.9.4/pyjibe/fd/main.ui`

 * *Files identical despite different names*

### Comparing `pyjibe-0.9.3/pyjibe/fd/mpl_edelta.py` & `pyjibe-0.9.4/pyjibe/fd/mpl_edelta.py`

 * *Files identical despite different names*

### Comparing `pyjibe-0.9.3/pyjibe/fd/mpl_indent.py` & `pyjibe-0.9.4/pyjibe/fd/mpl_indent.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+import warnings
+
 from matplotlib.figure import Figure
 import matplotlib.gridspec as gridspec
 from matplotlib.backends.backend_qt5agg import (
     FigureCanvasQTAgg as FigureCanvas)
 import numpy as np
 
-
 from .. import units
 from ..head import custom_widgets
 
 
 class MPLIndentation(object):
     def __init__(self):
         """Matplotlib plot for force-indentation data"""
@@ -72,19 +73,26 @@
         yaxis = "force"
         xscale = units.hrscale(xaxis)
         yscale = units.hrscale(yaxis)
         xunit = units.hrunit(xaxis)
         yunit = units.hrunit(yaxis)
 
         # approach and retract data
-        for segment in ["approach", "retract"]:
-            segment_bool = segment == "retract"
+        if fdist.metadata["segment count"] == 2:
+            segments = ["approach", "retract"]
+        else:
+            segments = ["approach", "intermediate", "retract"]
+        for ii, segment in enumerate(segments):
+            if segment == "intermediate":
+                # Dear future self...
+                warnings.warn("Ignoring 'intermediate' segment!")
+                continue
             self.plots[segment].set_data(
-                fdist[xaxis][fdist["segment"] == segment_bool]*xscale,
-                fdist[yaxis][fdist["segment"] == segment_bool]*yscale)
+                fdist[xaxis][fdist["segment"] == ii]*xscale,
+                fdist[yaxis][fdist["segment"] == ii]*yscale)
 
         self.axis_res.set_xlabel("{} [{}]".format(xaxis, xunit))
         self.axis_res.set_ylabel("residuals [{}]".format(yunit))
         self.axis_main.set_ylabel("{} [{}]".format(yaxis, yunit))
 
         if "fit" in fdist and np.sum(fdist["fit range"]):
             self.plots["residuals"].set_visible(True)
```

### Comparing `pyjibe-0.9.3/pyjibe/fd/mpl_qmap.py` & `pyjibe-0.9.4/pyjibe/fd/mpl_qmap.py`

 * *Files identical despite different names*

### Comparing `pyjibe-0.9.3/pyjibe/fd/rating_base.py` & `pyjibe-0.9.4/pyjibe/fd/rating_base.py`

 * *Files identical despite different names*

### Comparing `pyjibe-0.9.3/pyjibe/fd/rating_iface.py` & `pyjibe-0.9.4/pyjibe/fd/rating_iface.py`

 * *Files identical despite different names*

### Comparing `pyjibe-0.9.3/pyjibe/fd/rating_iface.ui` & `pyjibe-0.9.4/pyjibe/fd/rating_iface.ui`

 * *Files identical despite different names*

### Comparing `pyjibe-0.9.3/pyjibe/fd/tab_edelta.py` & `pyjibe-0.9.4/pyjibe/fd/tab_edelta.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,17 +47,16 @@
     def mpl_edelta_update(self):
         """Update the E(delta) plot"""
         if self.fd.tabs.currentWidget() == self:
             fdist = self.current_curve
             delta_opt = self.fd.tab_fit.sp_range_1.value()
             # Update slider range
             xaxis = self.fd.tab_fit.cb_xaxis.currentText()
-            segment = self.fd.tab_fit.cb_segment.currentText().lower()
-            segment_bool = segment == "retract"
-            segid = fdist["segment"] == segment_bool
+            segment_idx = self.fd.tab_fit.cb_segment.currentIndex()
+            segid = fdist["segment"] == segment_idx
             xdata = fdist[xaxis]
             xscale = units.hrscale(xaxis)
             minx = np.min(xdata[segid])*xscale
             self.delta_slider.blockSignals(True)
             self.delta_slider.setMinimum(minx)
             self.delta_slider.setValue(delta_opt)
             self.delta_slider.blockSignals(False)
```

### Comparing `pyjibe-0.9.3/pyjibe/fd/tab_edelta.ui` & `pyjibe-0.9.4/pyjibe/fd/tab_edelta.ui`

 * *Files identical despite different names*

### Comparing `pyjibe-0.9.3/pyjibe/fd/tab_fit.py` & `pyjibe-0.9.4/pyjibe/fd/tab_fit.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,19 @@
                                                   "tab_fit.ui")
         uic.loadUi(path_ui, self)
 
         # Setup the fitting tab
         id_para = 0
         # Model selection
         models_av = list(nmodel.models_available.keys())
+        # Exact spherical model is only available in developer mode
+        settings = QtCore.QSettings()
+        settings.setIniCodec("utf-8")
+        if not bool(int(settings.value("developer mode", "0"))):
+            models_av.remove("sneddon_spher")
         models_av.sort(key=lambda x: nmodel.models_available[x].model_name)
         for ii, key in enumerate(models_av):
             model = nmodel.models_available[key]
             self.cb_model.addItem(model.model_name, key)
             if key == "hertz_para":
                 id_para = ii
         # Setz Hertz Parabolic as default
```

### Comparing `pyjibe-0.9.3/pyjibe/fd/tab_fit.ui` & `pyjibe-0.9.4/pyjibe/fd/tab_fit.ui`

 * *Files identical despite different names*

### Comparing `pyjibe-0.9.3/pyjibe/fd/tab_info.py` & `pyjibe-0.9.4/pyjibe/fd/tab_info.py`

 * *Files identical despite different names*

### Comparing `pyjibe-0.9.3/pyjibe/fd/tab_info.ui` & `pyjibe-0.9.4/pyjibe/fd/tab_info.ui`

 * *Files identical despite different names*

### Comparing `pyjibe-0.9.3/pyjibe/fd/tab_preprocess.py` & `pyjibe-0.9.4/pyjibe/fd/tab_preprocess.py`

 * *Files identical despite different names*

### Comparing `pyjibe-0.9.3/pyjibe/fd/tab_preprocess.ui` & `pyjibe-0.9.4/pyjibe/fd/tab_preprocess.ui`

 * *Files identical despite different names*

### Comparing `pyjibe-0.9.3/pyjibe/fd/tab_qmap.py` & `pyjibe-0.9.4/pyjibe/fd/tab_qmap.py`

 * *Files identical despite different names*

### Comparing `pyjibe-0.9.3/pyjibe/fd/tab_qmap.ui` & `pyjibe-0.9.4/pyjibe/fd/tab_qmap.ui`

 * *Files identical despite different names*

### Comparing `pyjibe-0.9.3/pyjibe/fd/widget_fdist.py` & `pyjibe-0.9.4/pyjibe/fd/widget_fdist.py`

 * *Files identical despite different names*

### Comparing `pyjibe-0.9.3/pyjibe/head/custom_widgets/dirdialog_multiselect.py` & `pyjibe-0.9.4/pyjibe/head/custom_widgets/dirdialog_multiselect.py`

 * *Files identical despite different names*

### Comparing `pyjibe-0.9.3/pyjibe/head/custom_widgets/mpl_navigation_toolbar_icons.py` & `pyjibe-0.9.4/pyjibe/head/custom_widgets/mpl_navigation_toolbar_icons.py`

 * *Files identical despite different names*

### Comparing `pyjibe-0.9.3/pyjibe/head/custom_widgets/wait_cursor.py` & `pyjibe-0.9.4/pyjibe/head/custom_widgets/wait_cursor.py`

 * *Files identical despite different names*

### Comparing `pyjibe-0.9.3/pyjibe/head/dlg_tool_convert.py` & `pyjibe-0.9.4/pyjibe/head/dlg_tool_convert.py`

 * *Files identical despite different names*

### Comparing `pyjibe-0.9.3/pyjibe/head/dlg_tool_convert.ui` & `pyjibe-0.9.4/pyjibe/head/dlg_tool_convert.ui`

 * *Files identical despite different names*

### Comparing `pyjibe-0.9.3/pyjibe/head/infdoubleslider.py` & `pyjibe-0.9.4/pyjibe/head/infdoubleslider.py`

 * *Files identical despite different names*

### Comparing `pyjibe-0.9.3/pyjibe/head/infdoublespinbox.py` & `pyjibe-0.9.4/pyjibe/head/infdoublespinbox.py`

 * *Files identical despite different names*

### Comparing `pyjibe-0.9.3/pyjibe/head/main.py` & `pyjibe-0.9.4/pyjibe/head/main.py`

 * *Files identical despite different names*

### Comparing `pyjibe-0.9.3/pyjibe/head/main.ui` & `pyjibe-0.9.4/pyjibe/head/main.ui`

 * *Files identical despite different names*

### Comparing `pyjibe-0.9.3/pyjibe/img/icon.png` & `pyjibe-0.9.4/pyjibe/img/icon.png`

 * *Files identical despite different names*

### Comparing `pyjibe-0.9.3/pyjibe/img/savedat_large.png` & `pyjibe-0.9.4/pyjibe/img/savedat_large.png`

 * *Files identical despite different names*

### Comparing `pyjibe-0.9.3/pyjibe/img/saveimg_large.png` & `pyjibe-0.9.4/pyjibe/img/saveimg_large.png`

 * *Files identical despite different names*

### Comparing `pyjibe-0.9.3/pyjibe/img/splash.png` & `pyjibe-0.9.4/pyjibe/img/splash.png`

 * *Files identical despite different names*

### Comparing `pyjibe-0.9.3/pyjibe/units.py` & `pyjibe-0.9.4/pyjibe/units.py`

 * *Files identical despite different names*

### Comparing `pyjibe-0.9.3/pyjibe/util.py` & `pyjibe-0.9.4/pyjibe/util.py`

 * *Files identical despite different names*

### Comparing `pyjibe-0.9.3/pyjibe.egg-info/PKG-INFO` & `pyjibe-0.9.4/pyjibe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pyjibe
-Version: 0.9.3
+Version: 0.9.4
 Summary: Graphical user interface for Bio-AFM analysis
 Home-page: https://github.com/AFM-analysis/PyJibe
 Author: Paul Müller
 Author-email: dev@craban.de
 License: GPL v3
 Description: |PyJibe|
         ========
```

### Comparing `pyjibe-0.9.3/pyjibe.egg-info/SOURCES.txt` & `pyjibe-0.9.4/pyjibe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyjibe-0.9.3/setup.py` & `pyjibe-0.9.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,16 +20,16 @@
     version=version,
     packages=find_packages(),
     package_dir={name: name},
     include_package_data=True,
     license="GPL v3",
     description=description,
     long_description=open('README.rst').read() if exists('README.rst') else '',
-    install_requires=["afmformats>=0.15.0",
-                      "nanite>=1.7.8",
+    install_requires=["afmformats>=0.16.0",
+                      "nanite>=2.0.0",
                       "matplotlib>=3",  # NavigationToolbar2QT mod
                       "pyqt5"],
     python_requires='>=3.6, <4',
     entry_points={"gui_scripts": ['pyjibe = pyjibe.__main__:main']},
     keywords=["atomic force microscopy", "biomechanics"],
     classifiers=[
         'Operating System :: OS Independent',
```

### Comparing `pyjibe-0.9.3/tests/conftest.py` & `pyjibe-0.9.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyjibe-0.9.3/tests/data/invalid_dataset.jpk-force` & `pyjibe-0.9.4/tests/data/invalid_dataset.jpk-force`

 * *Files identical despite different names*

### Comparing `pyjibe-0.9.3/tests/data/spot3-0192.jpk-force` & `pyjibe-0.9.4/tests/data/spot3-0192.jpk-force`

 * *Files identical despite different names*

### Comparing `pyjibe-0.9.3/tests/test_fd_base.py` & `pyjibe-0.9.4/tests/test_fd_base.py`

 * *Files identical despite different names*

### Comparing `pyjibe-0.9.3/tests/test_fd_fit.py` & `pyjibe-0.9.4/tests/test_fd_fit.py`

 * *Files identical despite different names*

### Comparing `pyjibe-0.9.3/tests/test_fd_fit_model_expr.py` & `pyjibe-0.9.4/tests/test_fd_fit_model_expr.py`

 * *Files identical despite different names*

### Comparing `pyjibe-0.9.3/tests/test_fd_qmap.py` & `pyjibe-0.9.4/tests/test_fd_qmap.py`

 * *Files identical despite different names*

### Comparing `pyjibe-0.9.3/tests/test_fd_rater.py` & `pyjibe-0.9.4/tests/test_fd_rater.py`

 * *Files identical despite different names*

### Comparing `pyjibe-0.9.3/tests/test_head.py` & `pyjibe-0.9.4/tests/test_head.py`

 * *Files identical despite different names*

