# Comparing `tmp/napari_matplotlib-1.0.0.tar.gz` & `tmp/napari_matplotlib-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari_matplotlib-1.0.0.tar", last modified: Fri Jun 30 11:33:34 2023, max compression
+gzip compressed data, was "napari_matplotlib-1.0.1.tar", last modified: Fri Jul 21 10:27:20 2023, max compression
```

## Comparing `napari_matplotlib-1.0.0.tar` & `napari_matplotlib-1.0.1.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:33:34.174736 napari_matplotlib-1.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:33:34.158736 napari_matplotlib-1.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:33:34.162736 napari_matplotlib-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/.github/workflows/napari_hub_preview.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:33:34.162736 napari_matplotlib-1.0.0/.napari/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/.napari/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-06-30 11:33:34.174736 napari_matplotlib-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:33:34.162736 napari_matplotlib-1.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:33:34.166736 napari_matplotlib-1.0.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)  1116521 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/docs/_static/hist.png
--rw-r--r--   0 runner    (1001) docker     (123)    52586 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/docs/_static/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/docs/third_party.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/docs/user_guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-06-30 11:33:34.174736 napari_matplotlib-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:33:34.158736 napari_matplotlib-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:33:34.166736 napari_matplotlib-1.0.0/src/napari_matplotlib/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-30 11:33:34.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    11409 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/histogram.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:33:34.158736 napari_matplotlib-1.0.0/src/napari_matplotlib/icons/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:33:34.170736 napari_matplotlib-1.0.0/src/napari_matplotlib/icons/black/
--rw-r--r--   0 runner    (1001) docker     (123)     6919 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/icons/black/Back.png
--rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/icons/black/Customize.png
--rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/icons/black/Forward.png
--rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/icons/black/Home.png
--rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/icons/black/Pan.png
--rw-r--r--   0 runner    (1001) docker     (123)    12383 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/icons/black/Pan_checked.png
--rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/icons/black/Save.png
--rw-r--r--   0 runner    (1001) docker     (123)     7042 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/icons/black/Subplots.png
--rw-r--r--   0 runner    (1001) docker     (123)     8367 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/icons/black/Zoom.png
--rw-r--r--   0 runner    (1001) docker     (123)    12884 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/icons/black/Zoom_checked.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:33:34.170736 napari_matplotlib-1.0.0/src/napari_matplotlib/icons/white/
--rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/icons/white/Back.png
--rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/icons/white/Customize.png
--rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/icons/white/Forward.png
--rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/icons/white/Home.png
--rw-r--r--   0 runner    (1001) docker     (123)     7114 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/icons/white/Pan.png
--rw-r--r--   0 runner    (1001) docker     (123)    11810 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/icons/white/Pan_checked.png
--rw-r--r--   0 runner    (1001) docker     (123)     7381 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/icons/white/Save.png
--rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/icons/white/Subplots.png
--rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/icons/white/Zoom.png
--rw-r--r--   0 runner    (1001) docker     (123)    12372 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/icons/white/Zoom_checked.png
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/napari.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/scatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/slice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:33:34.170736 napari_matplotlib-1.0.0/src/napari_matplotlib/styles/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/styles/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/styles/dark.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/styles/light.mplstyle
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:33:34.174736 napari_matplotlib-1.0.0/src/napari_matplotlib/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:33:34.174736 napari_matplotlib-1.0.0/src/napari_matplotlib/tests/baseline/
--rw-r--r--   0 runner    (1001) docker     (123)    15662 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/tests/baseline/test_custom_theme.png
--rw-r--r--   0 runner    (1001) docker     (123)    28728 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/tests/baseline/test_histogram_2D.png
--rw-r--r--   0 runner    (1001) docker     (123)    20558 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/tests/baseline/test_histogram_3D.png
--rw-r--r--   0 runner    (1001) docker     (123)    34981 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/tests/baseline/test_no_theme_side_effects.png
--rw-r--r--   0 runner    (1001) docker     (123)    21290 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/tests/baseline/test_slice_2D.png
--rw-r--r--   0 runner    (1001) docker     (123)    14698 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/tests/baseline/test_slice_3D.png
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:33:34.174736 napari_matplotlib-1.0.0/src/napari_matplotlib/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/tests/data/test_theme.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/tests/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:33:34.174736 napari_matplotlib-1.0.0/src/napari_matplotlib/tests/scatter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/tests/scatter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:33:34.174736 napari_matplotlib-1.0.0/src/napari_matplotlib/tests/scatter/baseline/
--rw-r--r--   0 runner    (1001) docker     (123)    24951 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/tests/scatter/baseline/test_features_scatter_widget_2D.png
--rw-r--r--   0 runner    (1001) docker     (123)    18537 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/tests/scatter/baseline/test_scatter_2D.png
--rw-r--r--   0 runner    (1001) docker     (123)    17321 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/tests/scatter/baseline/test_scatter_3D.png
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/tests/scatter/test_scatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/tests/scatter/test_scatter_features.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/tests/test_histogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/tests/test_layer_changes.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/tests/test_slice.py
--rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/tests/test_theme.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/tests/test_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/src/napari_matplotlib/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:33:34.166736 napari_matplotlib-1.0.0/src/napari_matplotlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-06-30 11:33:34.000000 napari_matplotlib-1.0.0/src/napari_matplotlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-06-30 11:33:34.000000 napari_matplotlib-1.0.0/src/napari_matplotlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 11:33:34.000000 napari_matplotlib-1.0.0/src/napari_matplotlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-30 11:33:34.000000 napari_matplotlib-1.0.0/src/napari_matplotlib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-30 11:33:34.000000 napari_matplotlib-1.0.0/src/napari_matplotlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 11:33:34.000000 napari_matplotlib-1.0.0/src/napari_matplotlib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-30 11:33:19.000000 napari_matplotlib-1.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:27:20.810291 napari_matplotlib-1.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:27:20.790291 napari_matplotlib-1.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:27:20.794291 napari_matplotlib-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/.github/workflows/napari_hub_preview.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:27:20.794291 napari_matplotlib-1.0.1/.napari/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/.napari/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-07-21 10:27:20.810291 napari_matplotlib-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:27:20.794291 napari_matplotlib-1.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:27:20.798291 napari_matplotlib-1.0.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)  1116521 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/docs/_static/hist.png
+-rw-r--r--   0 runner    (1001) docker     (123)    52586 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/docs/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/docs/third_party.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/docs/user_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-07-21 10:27:20.810291 napari_matplotlib-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:27:20.790291 napari_matplotlib-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:27:20.798291 napari_matplotlib-1.0.1/src/napari_matplotlib/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/src/napari_matplotlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-21 10:27:20.000000 napari_matplotlib-1.0.1/src/napari_matplotlib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11409 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/src/napari_matplotlib/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/src/napari_matplotlib/histogram.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:27:20.790291 napari_matplotlib-1.0.1/src/napari_matplotlib/icons/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:27:20.802291 napari_matplotlib-1.0.1/src/napari_matplotlib/icons/black/
+-rw-r--r--   0 runner    (1001) docker     (123)     6919 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/src/napari_matplotlib/icons/black/Back.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/src/napari_matplotlib/icons/black/Customize.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/src/napari_matplotlib/icons/black/Forward.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/src/napari_matplotlib/icons/black/Home.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/src/napari_matplotlib/icons/black/Pan.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12383 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/src/napari_matplotlib/icons/black/Pan_checked.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/src/napari_matplotlib/icons/black/Save.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7042 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/src/napari_matplotlib/icons/black/Subplots.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8367 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/src/napari_matplotlib/icons/black/Zoom.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12884 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/src/napari_matplotlib/icons/black/Zoom_checked.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:27:20.806291 napari_matplotlib-1.0.1/src/napari_matplotlib/icons/white/
+-rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/src/napari_matplotlib/icons/white/Back.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/src/napari_matplotlib/icons/white/Customize.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/src/napari_matplotlib/icons/white/Forward.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/src/napari_matplotlib/icons/white/Home.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7114 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/src/napari_matplotlib/icons/white/Pan.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11810 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/src/napari_matplotlib/icons/white/Pan_checked.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7381 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/src/napari_matplotlib/icons/white/Save.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/src/napari_matplotlib/icons/white/Subplots.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/src/napari_matplotlib/icons/white/Zoom.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12372 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/src/napari_matplotlib/icons/white/Zoom_checked.png
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/src/napari_matplotlib/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/src/napari_matplotlib/scatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/src/napari_matplotlib/slice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:27:20.806291 napari_matplotlib-1.0.1/src/napari_matplotlib/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/src/napari_matplotlib/styles/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/src/napari_matplotlib/styles/dark.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/src/napari_matplotlib/styles/light.mplstyle
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:27:20.806291 napari_matplotlib-1.0.1/src/napari_matplotlib/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/src/napari_matplotlib/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:27:20.810291 napari_matplotlib-1.0.1/src/napari_matplotlib/tests/baseline/
+-rw-r--r--   0 runner    (1001) docker     (123)    15662 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/src/napari_matplotlib/tests/baseline/test_custom_theme.png
+-rw-r--r--   0 runner    (1001) docker     (123)    28728 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/src/napari_matplotlib/tests/baseline/test_histogram_2D.png
+-rw-r--r--   0 runner    (1001) docker     (123)    20558 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/src/napari_matplotlib/tests/baseline/test_histogram_3D.png
+-rw-r--r--   0 runner    (1001) docker     (123)    34981 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/src/napari_matplotlib/tests/baseline/test_no_theme_side_effects.png
+-rw-r--r--   0 runner    (1001) docker     (123)    21290 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/src/napari_matplotlib/tests/baseline/test_slice_2D.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14698 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/src/napari_matplotlib/tests/baseline/test_slice_3D.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/src/napari_matplotlib/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:27:20.810291 napari_matplotlib-1.0.1/src/napari_matplotlib/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/src/napari_matplotlib/tests/data/test_theme.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/src/napari_matplotlib/tests/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:27:20.810291 napari_matplotlib-1.0.1/src/napari_matplotlib/tests/scatter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/src/napari_matplotlib/tests/scatter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:27:20.810291 napari_matplotlib-1.0.1/src/napari_matplotlib/tests/scatter/baseline/
+-rw-r--r--   0 runner    (1001) docker     (123)    24951 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/src/napari_matplotlib/tests/scatter/baseline/test_features_scatter_widget_2D.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18537 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/src/napari_matplotlib/tests/scatter/baseline/test_scatter_2D.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17321 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/src/napari_matplotlib/tests/scatter/baseline/test_scatter_3D.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/src/napari_matplotlib/tests/scatter/test_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/src/napari_matplotlib/tests/scatter/test_scatter_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/src/napari_matplotlib/tests/test_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/src/napari_matplotlib/tests/test_layer_changes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/src/napari_matplotlib/tests/test_slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/src/napari_matplotlib/tests/test_theme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/src/napari_matplotlib/tests/test_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/src/napari_matplotlib/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/src/napari_matplotlib/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:27:20.802291 napari_matplotlib-1.0.1/src/napari_matplotlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-07-21 10:27:20.000000 napari_matplotlib-1.0.1/src/napari_matplotlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-07-21 10:27:20.000000 napari_matplotlib-1.0.1/src/napari_matplotlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 10:27:20.000000 napari_matplotlib-1.0.1/src/napari_matplotlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-21 10:27:20.000000 napari_matplotlib-1.0.1/src/napari_matplotlib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-21 10:27:20.000000 napari_matplotlib-1.0.1/src/napari_matplotlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-21 10:27:20.000000 napari_matplotlib-1.0.1/src/napari_matplotlib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-21 10:27:07.000000 napari_matplotlib-1.0.1/tox.ini
```

### Comparing `napari_matplotlib-1.0.0/.github/workflows/docs.yml` & `napari_matplotlib-1.0.1/.github/workflows/docs.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 name: Build docs
 
 on:
+
   pull_request:
     branches:
       - main
   push:
     branches:
       - main
+    tags:
+      - "v*" # Push events to matching v*, i.e. v1.0, v20.15.10
 
 jobs:
   build-docs:
     name: Build & Upload Artifact
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
```

### Comparing `napari_matplotlib-1.0.0/.github/workflows/napari_hub_preview.yml` & `napari_matplotlib-1.0.1/.github/workflows/napari_hub_preview.yml`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-1.0.0/.github/workflows/test_and_deploy.yml` & `napari_matplotlib-1.0.1/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-1.0.0/.gitignore` & `napari_matplotlib-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-1.0.0/.pre-commit-config.yaml` & `napari_matplotlib-1.0.1/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     rev: v4.4.0
     hooks:
       - id: check-docstring-first
       - id: end-of-file-fixer
       - id: trailing-whitespace
 
   - repo: https://github.com/asottile/setup-cfg-fmt
-    rev: v2.3.0
+    rev: v2.4.0
     hooks:
       - id: setup-cfg-fmt
 
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black
@@ -25,13 +25,13 @@
     rev: v1.4.1
     hooks:
      - id: mypy
        additional_dependencies: [numpy, matplotlib]
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
     # Ruff version.
-    rev: 'v0.0.275'
+    rev: 'v0.0.276'
     hooks:
       - id: ruff
 
 ci:
   autofix_prs: false
```

### Comparing `napari_matplotlib-1.0.0/LICENSE` & `napari_matplotlib-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-1.0.0/PKG-INFO` & `napari_matplotlib-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari_matplotlib
-Version: 1.0.0
+Version: 1.0.1
 Summary: A plugin to use Matplotlib with napari
 Home-page: https://github.com/matplotlib/napari-matplotlib
 Author: David Stansby
 Author-email: d.stansby@ucl.ac.uk
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/matplotlib/napari-matplotlib/issues
 Project-URL: Documentation, https://napari-matplotlib.github.io
```

### Comparing `napari_matplotlib-1.0.0/README.md` & `napari_matplotlib-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-1.0.0/docs/Makefile` & `napari_matplotlib-1.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-1.0.0/docs/_static/hist.png` & `napari_matplotlib-1.0.1/docs/_static/hist.png`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-1.0.0/docs/_static/logo.png` & `napari_matplotlib-1.0.1/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-1.0.0/docs/changelog.rst` & `napari_matplotlib-1.0.1/docs/changelog.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Changelog
 =========
 
+1.0.1
+-----
+Bug fixes
+~~~~~~~~~
+- Pinned that maximum version of `napari` to 0.4.17, since ``napari-matplotlib``
+  does not yet work with ``napari`` 0.4.18.
+
 1.0.0
 -----
 
 New features
 ~~~~~~~~~~~~
 - Added ``MPLWidget`` as a widget containing just a Matplotlib canvas
   without any association with a napari viewer.
```

### Comparing `napari_matplotlib-1.0.0/docs/conf.py` & `napari_matplotlib-1.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-1.0.0/docs/index.rst` & `napari_matplotlib-1.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-1.0.0/docs/make.bat` & `napari_matplotlib-1.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-1.0.0/docs/third_party.rst` & `napari_matplotlib-1.0.1/docs/third_party.rst`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-1.0.0/docs/user_guide.rst` & `napari_matplotlib-1.0.1/docs/user_guide.rst`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-1.0.0/pyproject.toml` & `napari_matplotlib-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-1.0.0/setup.cfg` & `napari_matplotlib-1.0.1/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 	Source Code = https://github.com/matplotlib/napari-matplotlib
 	User Support = https://github.com/matplotlib/napari-matplotlib/issues
 
 [options]
 packages = find:
 install_requires = 
 	matplotlib
-	napari
+	napari<0.4.18
 	numpy
 	tinycss2
 python_requires = >=3.8
 include_package_data = True
 package_dir = 
 	=src
 setup_requires =
```

### Comparing `napari_matplotlib-1.0.0/src/napari_matplotlib/base.py` & `napari_matplotlib-1.0.1/src/napari_matplotlib/base.py`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-1.0.0/src/napari_matplotlib/histogram.py` & `napari_matplotlib-1.0.1/src/napari_matplotlib/histogram.py`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-1.0.0/src/napari_matplotlib/icons/black/Back.png` & `napari_matplotlib-1.0.1/src/napari_matplotlib/icons/black/Back.png`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-1.0.0/src/napari_matplotlib/icons/black/Customize.png` & `napari_matplotlib-1.0.1/src/napari_matplotlib/icons/black/Customize.png`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-1.0.0/src/napari_matplotlib/icons/black/Forward.png` & `napari_matplotlib-1.0.1/src/napari_matplotlib/icons/black/Forward.png`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-1.0.0/src/napari_matplotlib/icons/black/Home.png` & `napari_matplotlib-1.0.1/src/napari_matplotlib/icons/black/Home.png`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-1.0.0/src/napari_matplotlib/icons/black/Pan.png` & `napari_matplotlib-1.0.1/src/napari_matplotlib/icons/black/Pan.png`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-1.0.0/src/napari_matplotlib/icons/black/Pan_checked.png` & `napari_matplotlib-1.0.1/src/napari_matplotlib/icons/black/Pan_checked.png`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-1.0.0/src/napari_matplotlib/icons/black/Save.png` & `napari_matplotlib-1.0.1/src/napari_matplotlib/icons/black/Save.png`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-1.0.0/src/napari_matplotlib/icons/black/Subplots.png` & `napari_matplotlib-1.0.1/src/napari_matplotlib/icons/black/Subplots.png`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-1.0.0/src/napari_matplotlib/icons/black/Zoom.png` & `napari_matplotlib-1.0.1/src/napari_matplotlib/icons/black/Zoom.png`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-1.0.0/src/napari_matplotlib/icons/black/Zoom_checked.png` & `napari_matplotlib-1.0.1/src/napari_matplotlib/icons/black/Zoom_checked.png`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-1.0.0/src/napari_matplotlib/icons/white/Back.png` & `napari_matplotlib-1.0.1/src/napari_matplotlib/icons/white/Back.png`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-1.0.0/src/napari_matplotlib/icons/white/Customize.png` & `napari_matplotlib-1.0.1/src/napari_matplotlib/icons/white/Customize.png`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-1.0.0/src/napari_matplotlib/icons/white/Forward.png` & `napari_matplotlib-1.0.1/src/napari_matplotlib/icons/white/Forward.png`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-1.0.0/src/napari_matplotlib/icons/white/Home.png` & `napari_matplotlib-1.0.1/src/napari_matplotlib/icons/white/Home.png`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-1.0.0/src/napari_matplotlib/icons/white/Pan.png` & `napari_matplotlib-1.0.1/src/napari_matplotlib/icons/white/Pan.png`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-1.0.0/src/napari_matplotlib/icons/white/Pan_checked.png` & `napari_matplotlib-1.0.1/src/napari_matplotlib/icons/white/Pan_checked.png`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-1.0.0/src/napari_matplotlib/icons/white/Save.png` & `napari_matplotlib-1.0.1/src/napari_matplotlib/icons/white/Save.png`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-1.0.0/src/napari_matplotlib/icons/white/Subplots.png` & `napari_matplotlib-1.0.1/src/napari_matplotlib/icons/white/Subplots.png`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-1.0.0/src/napari_matplotlib/icons/white/Zoom.png` & `napari_matplotlib-1.0.1/src/napari_matplotlib/icons/white/Zoom.png`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-1.0.0/src/napari_matplotlib/icons/white/Zoom_checked.png` & `napari_matplotlib-1.0.1/src/napari_matplotlib/icons/white/Zoom_checked.png`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-1.0.0/src/napari_matplotlib/napari.yaml` & `napari_matplotlib-1.0.1/src/napari_matplotlib/napari.yaml`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-1.0.0/src/napari_matplotlib/scatter.py` & `napari_matplotlib-1.0.1/src/napari_matplotlib/scatter.py`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-1.0.0/src/napari_matplotlib/slice.py` & `napari_matplotlib-1.0.1/src/napari_matplotlib/slice.py`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-1.0.0/src/napari_matplotlib/tests/baseline/test_custom_theme.png` & `napari_matplotlib-1.0.1/src/napari_matplotlib/tests/baseline/test_custom_theme.png`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-1.0.0/src/napari_matplotlib/tests/baseline/test_histogram_2D.png` & `napari_matplotlib-1.0.1/src/napari_matplotlib/tests/baseline/test_histogram_2D.png`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-1.0.0/src/napari_matplotlib/tests/baseline/test_histogram_3D.png` & `napari_matplotlib-1.0.1/src/napari_matplotlib/tests/baseline/test_histogram_3D.png`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-1.0.0/src/napari_matplotlib/tests/baseline/test_no_theme_side_effects.png` & `napari_matplotlib-1.0.1/src/napari_matplotlib/tests/baseline/test_no_theme_side_effects.png`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-1.0.0/src/napari_matplotlib/tests/baseline/test_slice_2D.png` & `napari_matplotlib-1.0.1/src/napari_matplotlib/tests/baseline/test_slice_2D.png`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-1.0.0/src/napari_matplotlib/tests/baseline/test_slice_3D.png` & `napari_matplotlib-1.0.1/src/napari_matplotlib/tests/baseline/test_slice_3D.png`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-1.0.0/src/napari_matplotlib/tests/conftest.py` & `napari_matplotlib-1.0.1/src/napari_matplotlib/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-1.0.0/src/napari_matplotlib/tests/helpers.py` & `napari_matplotlib-1.0.1/src/napari_matplotlib/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-1.0.0/src/napari_matplotlib/tests/scatter/baseline/test_features_scatter_widget_2D.png` & `napari_matplotlib-1.0.1/src/napari_matplotlib/tests/scatter/baseline/test_features_scatter_widget_2D.png`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-1.0.0/src/napari_matplotlib/tests/scatter/baseline/test_scatter_2D.png` & `napari_matplotlib-1.0.1/src/napari_matplotlib/tests/scatter/baseline/test_scatter_2D.png`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-1.0.0/src/napari_matplotlib/tests/scatter/baseline/test_scatter_3D.png` & `napari_matplotlib-1.0.1/src/napari_matplotlib/tests/scatter/baseline/test_scatter_3D.png`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-1.0.0/src/napari_matplotlib/tests/scatter/test_scatter.py` & `napari_matplotlib-1.0.1/src/napari_matplotlib/tests/scatter/test_scatter.py`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-1.0.0/src/napari_matplotlib/tests/scatter/test_scatter_features.py` & `napari_matplotlib-1.0.1/src/napari_matplotlib/tests/scatter/test_scatter_features.py`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-1.0.0/src/napari_matplotlib/tests/test_histogram.py` & `napari_matplotlib-1.0.1/src/napari_matplotlib/tests/test_histogram.py`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-1.0.0/src/napari_matplotlib/tests/test_layer_changes.py` & `napari_matplotlib-1.0.1/src/napari_matplotlib/tests/test_layer_changes.py`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-1.0.0/src/napari_matplotlib/tests/test_slice.py` & `napari_matplotlib-1.0.1/src/napari_matplotlib/tests/test_slice.py`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-1.0.0/src/napari_matplotlib/tests/test_theme.py` & `napari_matplotlib-1.0.1/src/napari_matplotlib/tests/test_theme.py`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-1.0.0/src/napari_matplotlib/tests/test_ui.py` & `napari_matplotlib-1.0.1/src/napari_matplotlib/tests/test_ui.py`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-1.0.0/src/napari_matplotlib/tests/test_util.py` & `napari_matplotlib-1.0.1/src/napari_matplotlib/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-1.0.0/src/napari_matplotlib/util.py` & `napari_matplotlib-1.0.1/src/napari_matplotlib/util.py`

 * *Files identical despite different names*

### Comparing `napari_matplotlib-1.0.0/src/napari_matplotlib.egg-info/PKG-INFO` & `napari_matplotlib-1.0.1/src/napari_matplotlib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-matplotlib
-Version: 1.0.0
+Version: 1.0.1
 Summary: A plugin to use Matplotlib with napari
 Home-page: https://github.com/matplotlib/napari-matplotlib
 Author: David Stansby
 Author-email: d.stansby@ucl.ac.uk
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/matplotlib/napari-matplotlib/issues
 Project-URL: Documentation, https://napari-matplotlib.github.io
```

### Comparing `napari_matplotlib-1.0.0/src/napari_matplotlib.egg-info/SOURCES.txt` & `napari_matplotlib-1.0.1/src/napari_matplotlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

