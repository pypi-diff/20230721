# Comparing `tmp/nwbwidgets-0.9.0.tar.gz` & `tmp/nwbwidgets-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nwbwidgets-0.9.0.tar", last modified: Sat Oct  1 16:45:31 2022, max compression
+gzip compressed data, was "nwbwidgets-0.9.1.tar", last modified: Sun Oct  2 15:21:40 2022, max compression
```

## Comparing `nwbwidgets-0.9.0.tar` & `nwbwidgets-0.9.1.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 bendichter   (502) staff       (20)        0 2022-10-01 16:45:31.654055 nwbwidgets-0.9.0/
--rw-r--r--   0 bendichter   (502) staff       (20)       60 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/.coveragerc
-drwxr-xr-x   0 bendichter   (502) staff       (20)        0 2022-10-01 16:45:31.638755 nwbwidgets-0.9.0/.github/
-drwxr-xr-x   0 bendichter   (502) staff       (20)        0 2022-10-01 16:45:31.640978 nwbwidgets-0.9.0/.github/workflows/
--rw-r--r--   0 bendichter   (502) staff       (20)      891 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/.github/workflows/workflow.yml
--rw-r--r--   0 bendichter   (502) staff       (20)     2034 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/.gitignore
--rw-r--r--   0 bendichter   (502) staff       (20)        1 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/CHANGELOG.md
--rw-r--r--   0 bendichter   (502) staff       (20)     3361 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 bendichter   (502) staff       (20)     2407 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/LICENSE
--rw-r--r--   0 bendichter   (502) staff       (20)     3752 2022-10-01 16:45:31.653832 nwbwidgets-0.9.0/PKG-INFO
--rw-r--r--   0 bendichter   (502) staff       (20)     2985 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/README.md
-drwxr-xr-x   0 bendichter   (502) staff       (20)        0 2022-10-01 16:45:31.641426 nwbwidgets-0.9.0/binder/
--rw-r--r--   0 bendichter   (502) staff       (20)      336 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/binder/postBuild
--rw-r--r--   0 bendichter   (502) staff       (20)       10 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/binder/requirements.txt
-drwxr-xr-x   0 bendichter   (502) staff       (20)        0 2022-10-01 16:45:31.641759 nwbwidgets-0.9.0/examples/
--rw-r--r--   0 bendichter   (502) staff       (20)     2728 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/examples/NWBWidgets-modality-demos.ipynb
--rw-r--r--   0 bendichter   (502) staff       (20)     2294 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/examples/YutaMouse41-ephys-viz.ipynb
-drwxr-xr-x   0 bendichter   (502) staff       (20)        0 2022-10-01 16:45:31.644910 nwbwidgets-0.9.0/nwbwidgets/
--rw-r--r--   0 bendichter   (502) staff       (20)      232 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/nwbwidgets/__init__.py
--rw-r--r--   0 bendichter   (502) staff       (20)     3053 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/nwbwidgets/allen.py
-drwxr-xr-x   0 bendichter   (502) staff       (20)        0 2022-10-01 16:45:31.645911 nwbwidgets-0.9.0/nwbwidgets/analysis/
--rw-r--r--   0 bendichter   (502) staff       (20)        0 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/nwbwidgets/analysis/__init__.py
--rw-r--r--   0 bendichter   (502) staff       (20)     5815 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/nwbwidgets/analysis/spikes.py
--rw-r--r--   0 bendichter   (502) staff       (20)    13547 2022-10-01 16:45:00.000000 nwbwidgets-0.9.0/nwbwidgets/base.py
--rw-r--r--   0 bendichter   (502) staff       (20)     6773 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/nwbwidgets/behavior.py
--rw-r--r--   0 bendichter   (502) staff       (20)     7435 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/nwbwidgets/brains.py
-drwxr-xr-x   0 bendichter   (502) staff       (20)        0 2022-10-01 16:45:31.646705 nwbwidgets-0.9.0/nwbwidgets/controllers/
--rw-r--r--   0 bendichter   (502) staff       (20)      203 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/nwbwidgets/controllers/__init__.py
--rw-r--r--   0 bendichter   (502) staff       (20)    13830 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/nwbwidgets/controllers/group_and_sort_controllers.py
--rw-r--r--   0 bendichter   (502) staff       (20)     1298 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/nwbwidgets/controllers/misc.py
--rw-r--r--   0 bendichter   (502) staff       (20)    10237 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/nwbwidgets/controllers/time_window_controllers.py
-drwxr-xr-x   0 bendichter   (502) staff       (20)        0 2022-10-01 16:45:31.647094 nwbwidgets-0.9.0/nwbwidgets/dashboards/
--rw-r--r--   0 bendichter   (502) staff       (20)      377 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/nwbwidgets/dashboards/README.md
--rw-r--r--   0 bendichter   (502) staff       (20)        0 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/nwbwidgets/dashboards/__init__.py
--rw-r--r--   0 bendichter   (502) staff       (20)     8638 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/nwbwidgets/dashboards/allen.py
-drwxr-xr-x   0 bendichter   (502) staff       (20)        0 2022-10-01 16:45:31.647239 nwbwidgets-0.9.0/nwbwidgets/dashboards/images/
--rw-r--r--   0 bendichter   (502) staff       (20)  1454342 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/nwbwidgets/dashboards/images/gif_allen.gif
--rw-r--r--   0 bendichter   (502) staff       (20)     8382 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/nwbwidgets/dynamictablesummary.py
--rw-r--r--   0 bendichter   (502) staff       (20)     5986 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/nwbwidgets/ecephys.py
--rw-r--r--   0 bendichter   (502) staff       (20)     1608 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/nwbwidgets/ephys_viz_interface.py
--rw-r--r--   0 bendichter   (502) staff       (20)     2934 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/nwbwidgets/file.py
--rw-r--r--   0 bendichter   (502) staff       (20)     9701 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/nwbwidgets/icephys.py
--rw-r--r--   0 bendichter   (502) staff       (20)     5500 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/nwbwidgets/image.py
--rw-r--r--   0 bendichter   (502) staff       (20)    43537 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/nwbwidgets/misc.py
--rw-r--r--   0 bendichter   (502) staff       (20)    12893 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/nwbwidgets/ophys.py
--rw-r--r--   0 bendichter   (502) staff       (20)     3701 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/nwbwidgets/spectrum.py
--rw-r--r--   0 bendichter   (502) staff       (20)    32177 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/nwbwidgets/timeseries.py
-drwxr-xr-x   0 bendichter   (502) staff       (20)        0 2022-10-01 16:45:31.650704 nwbwidgets-0.9.0/nwbwidgets/utils/
--rw-r--r--   0 bendichter   (502) staff       (20)        0 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/nwbwidgets/utils/__init__.py
--rw-r--r--   0 bendichter   (502) staff       (20)     3597 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/nwbwidgets/utils/cmaps.py
--rw-r--r--   0 bendichter   (502) staff       (20)     5772 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/nwbwidgets/utils/dynamictable.py
--rw-r--r--   0 bendichter   (502) staff       (20)      345 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/nwbwidgets/utils/functional.py
--rw-r--r--   0 bendichter   (502) staff       (20)     1202 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/nwbwidgets/utils/mpl.py
--rw-r--r--   0 bendichter   (502) staff       (20)     2459 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/nwbwidgets/utils/plotly.py
--rw-r--r--   0 bendichter   (502) staff       (20)      184 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/nwbwidgets/utils/pynwb.py
--rw-r--r--   0 bendichter   (502) staff       (20)      492 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/nwbwidgets/utils/testing.py
--rw-r--r--   0 bendichter   (502) staff       (20)     8240 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/nwbwidgets/utils/timeseries.py
--rw-r--r--   0 bendichter   (502) staff       (20)     5626 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/nwbwidgets/utils/units.py
--rw-r--r--   0 bendichter   (502) staff       (20)     2627 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/nwbwidgets/utils/widgets.py
--rw-r--r--   0 bendichter   (502) staff       (20)       18 2022-10-01 16:45:00.000000 nwbwidgets-0.9.0/nwbwidgets/version.py
--rw-r--r--   0 bendichter   (502) staff       (20)     3328 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/nwbwidgets/view.py
-drwxr-xr-x   0 bendichter   (502) staff       (20)        0 2022-10-01 16:45:31.645674 nwbwidgets-0.9.0/nwbwidgets.egg-info/
--rw-r--r--   0 bendichter   (502) staff       (20)     3752 2022-10-01 16:45:31.000000 nwbwidgets-0.9.0/nwbwidgets.egg-info/PKG-INFO
--rw-r--r--   0 bendichter   (502) staff       (20)     1889 2022-10-01 16:45:31.000000 nwbwidgets-0.9.0/nwbwidgets.egg-info/SOURCES.txt
--rw-r--r--   0 bendichter   (502) staff       (20)        1 2022-10-01 16:45:31.000000 nwbwidgets-0.9.0/nwbwidgets.egg-info/dependency_links.txt
--rw-r--r--   0 bendichter   (502) staff       (20)      196 2022-10-01 16:45:31.000000 nwbwidgets-0.9.0/nwbwidgets.egg-info/requires.txt
--rw-r--r--   0 bendichter   (502) staff       (20)       71 2022-10-01 16:45:31.000000 nwbwidgets-0.9.0/nwbwidgets.egg-info/top_level.txt
--rw-r--r--   0 bendichter   (502) staff       (20)      196 2022-10-01 16:45:00.000000 nwbwidgets-0.9.0/requirements.txt
--rw-r--r--   0 bendichter   (502) staff       (20)       38 2022-10-01 16:45:31.654107 nwbwidgets-0.9.0/setup.cfg
--rw-r--r--   0 bendichter   (502) staff       (20)     1432 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/setup.py
-drwxr-xr-x   0 bendichter   (502) staff       (20)        0 2022-10-01 16:45:31.653572 nwbwidgets-0.9.0/test/
--rw-r--r--   0 bendichter   (502) staff       (20)        0 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/test/__init__.py
--rw-r--r--   0 bendichter   (502) staff       (20)      446 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/test/conftest.py
--rw-r--r--   0 bendichter   (502) staff       (20)     4623 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/test/test_base.py
--rw-r--r--   0 bendichter   (502) staff       (20)     4517 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/test/test_behavior.py
--rw-r--r--   0 bendichter   (502) staff       (20)     3666 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/test/test_controllers.py
--rw-r--r--   0 bendichter   (502) staff       (20)     5407 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/test/test_dynamictablesummary.py
--rw-r--r--   0 bendichter   (502) staff       (20)     3552 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/test/test_ecephys.py
--rw-r--r--   0 bendichter   (502) staff       (20)      651 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/test/test_file.py
--rw-r--r--   0 bendichter   (502) staff       (20)     3781 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/test/test_icephys.py
--rw-r--r--   0 bendichter   (502) staff       (20)     1635 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/test/test_image.py
--rw-r--r--   0 bendichter   (502) staff       (20)     4538 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/test/test_misc.py
--rw-r--r--   0 bendichter   (502) staff       (20)     6054 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/test/test_ophys.py
--rw-r--r--   0 bendichter   (502) staff       (20)     8661 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/test/test_timeseries.py
--rw-r--r--   0 bendichter   (502) staff       (20)      417 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/test/test_utils_cmaps.py
--rw-r--r--   0 bendichter   (502) staff       (20)     1431 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/test/test_utils_dynamictable.py
--rw-r--r--   0 bendichter   (502) staff       (20)      472 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/test/test_utils_mpl.py
--rw-r--r--   0 bendichter   (502) staff       (20)     4786 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/test/test_utils_timeseries.py
--rw-r--r--   0 bendichter   (502) staff       (20)     7186 2022-09-30 18:42:44.000000 nwbwidgets-0.9.0/test/test_utils_units.py
+drwxr-xr-x   0 bendichter   (502) staff       (20)        0 2022-10-02 15:21:40.505312 nwbwidgets-0.9.1/
+-rw-r--r--   0 bendichter   (502) staff       (20)       60 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/.coveragerc
+drwxr-xr-x   0 bendichter   (502) staff       (20)        0 2022-10-02 15:21:40.494853 nwbwidgets-0.9.1/.github/
+drwxr-xr-x   0 bendichter   (502) staff       (20)        0 2022-10-02 15:21:40.496604 nwbwidgets-0.9.1/.github/workflows/
+-rw-r--r--   0 bendichter   (502) staff       (20)      891 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/.github/workflows/workflow.yml
+-rw-r--r--   0 bendichter   (502) staff       (20)     2034 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/.gitignore
+-rw-r--r--   0 bendichter   (502) staff       (20)        1 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/CHANGELOG.md
+-rw-r--r--   0 bendichter   (502) staff       (20)     3361 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 bendichter   (502) staff       (20)     2407 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/LICENSE
+-rw-r--r--   0 bendichter   (502) staff       (20)     3752 2022-10-02 15:21:40.505099 nwbwidgets-0.9.1/PKG-INFO
+-rw-r--r--   0 bendichter   (502) staff       (20)     2985 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/README.md
+drwxr-xr-x   0 bendichter   (502) staff       (20)        0 2022-10-02 15:21:40.496846 nwbwidgets-0.9.1/binder/
+-rw-r--r--   0 bendichter   (502) staff       (20)      336 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/binder/postBuild
+-rw-r--r--   0 bendichter   (502) staff       (20)       10 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/binder/requirements.txt
+drwxr-xr-x   0 bendichter   (502) staff       (20)        0 2022-10-02 15:21:40.497099 nwbwidgets-0.9.1/examples/
+-rw-r--r--   0 bendichter   (502) staff       (20)     2728 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/examples/NWBWidgets-modality-demos.ipynb
+-rw-r--r--   0 bendichter   (502) staff       (20)     2294 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/examples/YutaMouse41-ephys-viz.ipynb
+drwxr-xr-x   0 bendichter   (502) staff       (20)        0 2022-10-02 15:21:40.499097 nwbwidgets-0.9.1/nwbwidgets/
+-rw-r--r--   0 bendichter   (502) staff       (20)      232 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/nwbwidgets/__init__.py
+-rw-r--r--   0 bendichter   (502) staff       (20)     3053 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/nwbwidgets/allen.py
+drwxr-xr-x   0 bendichter   (502) staff       (20)        0 2022-10-02 15:21:40.499874 nwbwidgets-0.9.1/nwbwidgets/analysis/
+-rw-r--r--   0 bendichter   (502) staff       (20)        0 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/nwbwidgets/analysis/__init__.py
+-rw-r--r--   0 bendichter   (502) staff       (20)     5815 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/nwbwidgets/analysis/spikes.py
+-rw-r--r--   0 bendichter   (502) staff       (20)    13620 2022-10-02 15:11:54.000000 nwbwidgets-0.9.1/nwbwidgets/base.py
+-rw-r--r--   0 bendichter   (502) staff       (20)     6773 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/nwbwidgets/behavior.py
+-rw-r--r--   0 bendichter   (502) staff       (20)     7435 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/nwbwidgets/brains.py
+drwxr-xr-x   0 bendichter   (502) staff       (20)        0 2022-10-02 15:21:40.500347 nwbwidgets-0.9.1/nwbwidgets/controllers/
+-rw-r--r--   0 bendichter   (502) staff       (20)      203 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/nwbwidgets/controllers/__init__.py
+-rw-r--r--   0 bendichter   (502) staff       (20)    13830 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/nwbwidgets/controllers/group_and_sort_controllers.py
+-rw-r--r--   0 bendichter   (502) staff       (20)     1298 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/nwbwidgets/controllers/misc.py
+-rw-r--r--   0 bendichter   (502) staff       (20)    10237 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/nwbwidgets/controllers/time_window_controllers.py
+drwxr-xr-x   0 bendichter   (502) staff       (20)        0 2022-10-02 15:21:40.500679 nwbwidgets-0.9.1/nwbwidgets/dashboards/
+-rw-r--r--   0 bendichter   (502) staff       (20)      377 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/nwbwidgets/dashboards/README.md
+-rw-r--r--   0 bendichter   (502) staff       (20)        0 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/nwbwidgets/dashboards/__init__.py
+-rw-r--r--   0 bendichter   (502) staff       (20)     8638 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/nwbwidgets/dashboards/allen.py
+drwxr-xr-x   0 bendichter   (502) staff       (20)        0 2022-10-02 15:21:40.500797 nwbwidgets-0.9.1/nwbwidgets/dashboards/images/
+-rw-r--r--   0 bendichter   (502) staff       (20)  1454342 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/nwbwidgets/dashboards/images/gif_allen.gif
+-rw-r--r--   0 bendichter   (502) staff       (20)     8382 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/nwbwidgets/dynamictablesummary.py
+-rw-r--r--   0 bendichter   (502) staff       (20)     5986 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/nwbwidgets/ecephys.py
+-rw-r--r--   0 bendichter   (502) staff       (20)     1608 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/nwbwidgets/ephys_viz_interface.py
+-rw-r--r--   0 bendichter   (502) staff       (20)     2934 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/nwbwidgets/file.py
+-rw-r--r--   0 bendichter   (502) staff       (20)     9701 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/nwbwidgets/icephys.py
+-rw-r--r--   0 bendichter   (502) staff       (20)     5500 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/nwbwidgets/image.py
+-rw-r--r--   0 bendichter   (502) staff       (20)    43537 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/nwbwidgets/misc.py
+-rw-r--r--   0 bendichter   (502) staff       (20)    12893 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/nwbwidgets/ophys.py
+-rw-r--r--   0 bendichter   (502) staff       (20)     3701 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/nwbwidgets/spectrum.py
+-rw-r--r--   0 bendichter   (502) staff       (20)    32177 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/nwbwidgets/timeseries.py
+drwxr-xr-x   0 bendichter   (502) staff       (20)        0 2022-10-02 15:21:40.502853 nwbwidgets-0.9.1/nwbwidgets/utils/
+-rw-r--r--   0 bendichter   (502) staff       (20)        0 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/nwbwidgets/utils/__init__.py
+-rw-r--r--   0 bendichter   (502) staff       (20)     3597 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/nwbwidgets/utils/cmaps.py
+-rw-r--r--   0 bendichter   (502) staff       (20)     5772 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/nwbwidgets/utils/dynamictable.py
+-rw-r--r--   0 bendichter   (502) staff       (20)      345 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/nwbwidgets/utils/functional.py
+-rw-r--r--   0 bendichter   (502) staff       (20)     1202 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/nwbwidgets/utils/mpl.py
+-rw-r--r--   0 bendichter   (502) staff       (20)     2459 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/nwbwidgets/utils/plotly.py
+-rw-r--r--   0 bendichter   (502) staff       (20)      184 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/nwbwidgets/utils/pynwb.py
+-rw-r--r--   0 bendichter   (502) staff       (20)      492 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/nwbwidgets/utils/testing.py
+-rw-r--r--   0 bendichter   (502) staff       (20)     8240 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/nwbwidgets/utils/timeseries.py
+-rw-r--r--   0 bendichter   (502) staff       (20)     5626 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/nwbwidgets/utils/units.py
+-rw-r--r--   0 bendichter   (502) staff       (20)     2627 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/nwbwidgets/utils/widgets.py
+-rw-r--r--   0 bendichter   (502) staff       (20)       18 2022-10-02 15:12:00.000000 nwbwidgets-0.9.1/nwbwidgets/version.py
+-rw-r--r--   0 bendichter   (502) staff       (20)     3328 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/nwbwidgets/view.py
+drwxr-xr-x   0 bendichter   (502) staff       (20)        0 2022-10-02 15:21:40.499661 nwbwidgets-0.9.1/nwbwidgets.egg-info/
+-rw-r--r--   0 bendichter   (502) staff       (20)     3752 2022-10-02 15:21:40.000000 nwbwidgets-0.9.1/nwbwidgets.egg-info/PKG-INFO
+-rw-r--r--   0 bendichter   (502) staff       (20)     1889 2022-10-02 15:21:40.000000 nwbwidgets-0.9.1/nwbwidgets.egg-info/SOURCES.txt
+-rw-r--r--   0 bendichter   (502) staff       (20)        1 2022-10-02 15:21:40.000000 nwbwidgets-0.9.1/nwbwidgets.egg-info/dependency_links.txt
+-rw-r--r--   0 bendichter   (502) staff       (20)      184 2022-10-02 15:21:40.000000 nwbwidgets-0.9.1/nwbwidgets.egg-info/requires.txt
+-rw-r--r--   0 bendichter   (502) staff       (20)       71 2022-10-02 15:21:40.000000 nwbwidgets-0.9.1/nwbwidgets.egg-info/top_level.txt
+-rw-r--r--   0 bendichter   (502) staff       (20)      183 2022-10-02 15:11:54.000000 nwbwidgets-0.9.1/requirements.txt
+-rw-r--r--   0 bendichter   (502) staff       (20)       38 2022-10-02 15:21:40.505368 nwbwidgets-0.9.1/setup.cfg
+-rw-r--r--   0 bendichter   (502) staff       (20)     1432 2022-10-02 15:12:33.000000 nwbwidgets-0.9.1/setup.py
+drwxr-xr-x   0 bendichter   (502) staff       (20)        0 2022-10-02 15:21:40.504884 nwbwidgets-0.9.1/test/
+-rw-r--r--   0 bendichter   (502) staff       (20)        0 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/test/__init__.py
+-rw-r--r--   0 bendichter   (502) staff       (20)      446 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/test/conftest.py
+-rw-r--r--   0 bendichter   (502) staff       (20)     4623 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/test/test_base.py
+-rw-r--r--   0 bendichter   (502) staff       (20)     4517 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/test/test_behavior.py
+-rw-r--r--   0 bendichter   (502) staff       (20)     3666 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/test/test_controllers.py
+-rw-r--r--   0 bendichter   (502) staff       (20)     5407 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/test/test_dynamictablesummary.py
+-rw-r--r--   0 bendichter   (502) staff       (20)     3552 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/test/test_ecephys.py
+-rw-r--r--   0 bendichter   (502) staff       (20)      651 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/test/test_file.py
+-rw-r--r--   0 bendichter   (502) staff       (20)     3781 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/test/test_icephys.py
+-rw-r--r--   0 bendichter   (502) staff       (20)     1635 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/test/test_image.py
+-rw-r--r--   0 bendichter   (502) staff       (20)     4538 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/test/test_misc.py
+-rw-r--r--   0 bendichter   (502) staff       (20)     6054 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/test/test_ophys.py
+-rw-r--r--   0 bendichter   (502) staff       (20)     8661 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/test/test_timeseries.py
+-rw-r--r--   0 bendichter   (502) staff       (20)      417 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/test/test_utils_cmaps.py
+-rw-r--r--   0 bendichter   (502) staff       (20)     1431 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/test/test_utils_dynamictable.py
+-rw-r--r--   0 bendichter   (502) staff       (20)      472 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/test/test_utils_mpl.py
+-rw-r--r--   0 bendichter   (502) staff       (20)     4786 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/test/test_utils_timeseries.py
+-rw-r--r--   0 bendichter   (502) staff       (20)     7186 2022-09-30 18:42:44.000000 nwbwidgets-0.9.1/test/test_utils_units.py
```

### Comparing `nwbwidgets-0.9.0/.github/workflows/workflow.yml` & `nwbwidgets-0.9.1/.github/workflows/workflow.yml`

 * *Files identical despite different names*

### Comparing `nwbwidgets-0.9.0/.gitignore` & `nwbwidgets-0.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `nwbwidgets-0.9.0/CODE_OF_CONDUCT.md` & `nwbwidgets-0.9.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `nwbwidgets-0.9.0/LICENSE` & `nwbwidgets-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nwbwidgets-0.9.0/PKG-INFO` & `nwbwidgets-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwbwidgets
-Version: 0.9.0
+Version: 0.9.1
 Summary: This is nwbwidgets, widgets for viewing the contents of a NWB-file in Jupyter Notebooks using ipywidgets.
 Home-page: https://github.com/NeurodataWithoutBorders/nwb-jupyter-widgets
 Author: Ben Dichter
 Author-email: ben.dichter@catalystneuro.com
 License: BSD
 Keywords: jupyter,hdf5,notebook,nwb
 Classifier: Operating System :: OS Independent
```

### Comparing `nwbwidgets-0.9.0/README.md` & `nwbwidgets-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `nwbwidgets-0.9.0/examples/NWBWidgets-modality-demos.ipynb` & `nwbwidgets-0.9.1/examples/NWBWidgets-modality-demos.ipynb`

 * *Files identical despite different names*

### Comparing `nwbwidgets-0.9.0/examples/YutaMouse41-ephys-viz.ipynb` & `nwbwidgets-0.9.1/examples/YutaMouse41-ephys-viz.ipynb`

 * *Files identical despite different names*

### Comparing `nwbwidgets-0.9.0/nwbwidgets/allen.py` & `nwbwidgets-0.9.1/nwbwidgets/allen.py`

 * *Files identical despite different names*

### Comparing `nwbwidgets-0.9.0/nwbwidgets/analysis/spikes.py` & `nwbwidgets-0.9.1/nwbwidgets/analysis/spikes.py`

 * *Files identical despite different names*

### Comparing `nwbwidgets-0.9.0/nwbwidgets/base.py` & `nwbwidgets-0.9.1/nwbwidgets/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from collections.abc import Iterable
 from datetime import datetime
 from typing import Union
 
 import pandas as pd
 import matplotlib.pyplot as plt
 
-from ipydatagrid import DataGrid
+# from ipydatagrid import DataGrid re-add when ipywidgets 8 is supported
 from IPython import display
 from ipywidgets import widgets
 from ipywidgets.widgets.interaction import show_inline_matplotlib_plots
 
 import h5py
 from pynwb import ProcessingModule
 from pynwb.core import NWBDataInterface, MultiContainerInterface
@@ -30,21 +30,21 @@
         lbl_val = widgets.Label(str(val), layout=field_lay)
         info.append(widgets.HBox(children=[lbl_key, lbl_val]))
     vbox = widgets.VBox(info)
     return vbox
 
 
 def render_dataframe(dynamic_table: DynamicTable):
-    try:
-        return DataGrid(dynamic_table.to_dataframe())
-    except:
-        out1 = widgets.Output()
-        with out1:
-            display.display(dynamic_table.to_dataframe())
-        return out1
+    # try:
+    #     return DataGrid(dynamic_table.to_dataframe())
+    # except:
+    out1 = widgets.Output()
+    with out1:
+        display.display(dynamic_table.to_dataframe())
+    return out1
 
 
 def show_neurodata_base(
     node: NWBDataInterface, neurodata_vis_spec: dict
 ) -> widgets.Widget:
     """
     Gets a pynwb object and returns a Vertical Box containing textual info and
@@ -325,17 +325,18 @@
 
 
 def show_dset(dset: h5py.Dataset, **kwargs):
     return widgets.VBox(children=[show_dict(dict(dset.attrs)), dataset_to_sheet(dset)])
 
 
 def dataset_to_sheet(dset: h5py.Dataset):
-    if dset.ndim >= 2:
-        return widgets.HTML(print(dset))
-    return DataGrid(pd.DataFrame(dset[:]))
+    # if dset.ndim >= 2:
+    #     return widgets.HTML(print(dset))
+    # return DataGrid(pd.DataFrame(dset[:]))
+    return widgets.HTML(print(dset))
 
 
 def show_dict(in_dict) -> widgets.Widget:
     field_lay = widgets.Layout(
         max_height="40px", max_width="600px", min_height="30px", min_width="130px"
     )
     info = []
```

### Comparing `nwbwidgets-0.9.0/nwbwidgets/behavior.py` & `nwbwidgets-0.9.1/nwbwidgets/behavior.py`

 * *Files identical despite different names*

### Comparing `nwbwidgets-0.9.0/nwbwidgets/brains.py` & `nwbwidgets-0.9.1/nwbwidgets/brains.py`

 * *Files identical despite different names*

### Comparing `nwbwidgets-0.9.0/nwbwidgets/controllers/group_and_sort_controllers.py` & `nwbwidgets-0.9.1/nwbwidgets/controllers/group_and_sort_controllers.py`

 * *Files identical despite different names*

### Comparing `nwbwidgets-0.9.0/nwbwidgets/controllers/misc.py` & `nwbwidgets-0.9.1/nwbwidgets/controllers/misc.py`

 * *Files identical despite different names*

### Comparing `nwbwidgets-0.9.0/nwbwidgets/controllers/time_window_controllers.py` & `nwbwidgets-0.9.1/nwbwidgets/controllers/time_window_controllers.py`

 * *Files identical despite different names*

### Comparing `nwbwidgets-0.9.0/nwbwidgets/dashboards/allen.py` & `nwbwidgets-0.9.1/nwbwidgets/dashboards/allen.py`

 * *Files identical despite different names*

### Comparing `nwbwidgets-0.9.0/nwbwidgets/dashboards/images/gif_allen.gif` & `nwbwidgets-0.9.1/nwbwidgets/dashboards/images/gif_allen.gif`

 * *Files identical despite different names*

### Comparing `nwbwidgets-0.9.0/nwbwidgets/dynamictablesummary.py` & `nwbwidgets-0.9.1/nwbwidgets/dynamictablesummary.py`

 * *Files identical despite different names*

### Comparing `nwbwidgets-0.9.0/nwbwidgets/ecephys.py` & `nwbwidgets-0.9.1/nwbwidgets/ecephys.py`

 * *Files identical despite different names*

### Comparing `nwbwidgets-0.9.0/nwbwidgets/ephys_viz_interface.py` & `nwbwidgets-0.9.1/nwbwidgets/ephys_viz_interface.py`

 * *Files identical despite different names*

### Comparing `nwbwidgets-0.9.0/nwbwidgets/file.py` & `nwbwidgets-0.9.1/nwbwidgets/file.py`

 * *Files identical despite different names*

### Comparing `nwbwidgets-0.9.0/nwbwidgets/icephys.py` & `nwbwidgets-0.9.1/nwbwidgets/icephys.py`

 * *Files identical despite different names*

### Comparing `nwbwidgets-0.9.0/nwbwidgets/image.py` & `nwbwidgets-0.9.1/nwbwidgets/image.py`

 * *Files identical despite different names*

### Comparing `nwbwidgets-0.9.0/nwbwidgets/misc.py` & `nwbwidgets-0.9.1/nwbwidgets/misc.py`

 * *Files identical despite different names*

### Comparing `nwbwidgets-0.9.0/nwbwidgets/ophys.py` & `nwbwidgets-0.9.1/nwbwidgets/ophys.py`

 * *Files identical despite different names*

### Comparing `nwbwidgets-0.9.0/nwbwidgets/spectrum.py` & `nwbwidgets-0.9.1/nwbwidgets/spectrum.py`

 * *Files identical despite different names*

### Comparing `nwbwidgets-0.9.0/nwbwidgets/timeseries.py` & `nwbwidgets-0.9.1/nwbwidgets/timeseries.py`

 * *Files identical despite different names*

### Comparing `nwbwidgets-0.9.0/nwbwidgets/utils/cmaps.py` & `nwbwidgets-0.9.1/nwbwidgets/utils/cmaps.py`

 * *Files identical despite different names*

### Comparing `nwbwidgets-0.9.0/nwbwidgets/utils/dynamictable.py` & `nwbwidgets-0.9.1/nwbwidgets/utils/dynamictable.py`

 * *Files identical despite different names*

### Comparing `nwbwidgets-0.9.0/nwbwidgets/utils/mpl.py` & `nwbwidgets-0.9.1/nwbwidgets/utils/mpl.py`

 * *Files identical despite different names*

### Comparing `nwbwidgets-0.9.0/nwbwidgets/utils/plotly.py` & `nwbwidgets-0.9.1/nwbwidgets/utils/plotly.py`

 * *Files identical despite different names*

### Comparing `nwbwidgets-0.9.0/nwbwidgets/utils/timeseries.py` & `nwbwidgets-0.9.1/nwbwidgets/utils/timeseries.py`

 * *Files identical despite different names*

### Comparing `nwbwidgets-0.9.0/nwbwidgets/utils/units.py` & `nwbwidgets-0.9.1/nwbwidgets/utils/units.py`

 * *Files identical despite different names*

### Comparing `nwbwidgets-0.9.0/nwbwidgets/utils/widgets.py` & `nwbwidgets-0.9.1/nwbwidgets/utils/widgets.py`

 * *Files identical despite different names*

### Comparing `nwbwidgets-0.9.0/nwbwidgets/view.py` & `nwbwidgets-0.9.1/nwbwidgets/view.py`

 * *Files identical despite different names*

### Comparing `nwbwidgets-0.9.0/nwbwidgets.egg-info/PKG-INFO` & `nwbwidgets-0.9.1/nwbwidgets.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwbwidgets
-Version: 0.9.0
+Version: 0.9.1
 Summary: This is nwbwidgets, widgets for viewing the contents of a NWB-file in Jupyter Notebooks using ipywidgets.
 Home-page: https://github.com/NeurodataWithoutBorders/nwb-jupyter-widgets
 Author: Ben Dichter
 Author-email: ben.dichter@catalystneuro.com
 License: BSD
 Keywords: jupyter,hdf5,notebook,nwb
 Classifier: Operating System :: OS Independent
```

### Comparing `nwbwidgets-0.9.0/nwbwidgets.egg-info/SOURCES.txt` & `nwbwidgets-0.9.1/nwbwidgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nwbwidgets-0.9.0/setup.py` & `nwbwidgets-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `nwbwidgets-0.9.0/test/test_base.py` & `nwbwidgets-0.9.1/test/test_base.py`

 * *Files identical despite different names*

### Comparing `nwbwidgets-0.9.0/test/test_behavior.py` & `nwbwidgets-0.9.1/test/test_behavior.py`

 * *Files identical despite different names*

### Comparing `nwbwidgets-0.9.0/test/test_controllers.py` & `nwbwidgets-0.9.1/test/test_controllers.py`

 * *Files identical despite different names*

### Comparing `nwbwidgets-0.9.0/test/test_dynamictablesummary.py` & `nwbwidgets-0.9.1/test/test_dynamictablesummary.py`

 * *Files identical despite different names*

### Comparing `nwbwidgets-0.9.0/test/test_ecephys.py` & `nwbwidgets-0.9.1/test/test_ecephys.py`

 * *Files identical despite different names*

### Comparing `nwbwidgets-0.9.0/test/test_file.py` & `nwbwidgets-0.9.1/test/test_file.py`

 * *Files identical despite different names*

### Comparing `nwbwidgets-0.9.0/test/test_icephys.py` & `nwbwidgets-0.9.1/test/test_icephys.py`

 * *Files identical despite different names*

### Comparing `nwbwidgets-0.9.0/test/test_image.py` & `nwbwidgets-0.9.1/test/test_image.py`

 * *Files identical despite different names*

### Comparing `nwbwidgets-0.9.0/test/test_misc.py` & `nwbwidgets-0.9.1/test/test_misc.py`

 * *Files identical despite different names*

### Comparing `nwbwidgets-0.9.0/test/test_ophys.py` & `nwbwidgets-0.9.1/test/test_ophys.py`

 * *Files identical despite different names*

### Comparing `nwbwidgets-0.9.0/test/test_timeseries.py` & `nwbwidgets-0.9.1/test/test_timeseries.py`

 * *Files identical despite different names*

### Comparing `nwbwidgets-0.9.0/test/test_utils_dynamictable.py` & `nwbwidgets-0.9.1/test/test_utils_dynamictable.py`

 * *Files identical despite different names*

### Comparing `nwbwidgets-0.9.0/test/test_utils_timeseries.py` & `nwbwidgets-0.9.1/test/test_utils_timeseries.py`

 * *Files identical despite different names*

### Comparing `nwbwidgets-0.9.0/test/test_utils_units.py` & `nwbwidgets-0.9.1/test/test_utils_units.py`

 * *Files identical despite different names*

