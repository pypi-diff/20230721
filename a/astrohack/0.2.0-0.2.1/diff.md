# Comparing `tmp/astrohack-0.2.0.tar.gz` & `tmp/astrohack-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astrohack-0.2.0.tar", last modified: Fri Jul 21 19:34:01 2023, max compression
+gzip compressed data, was "astrohack-0.2.1.tar", last modified: Fri Jul 21 19:54:23 2023, max compression
```

## Comparing `astrohack-0.2.0.tar` & `astrohack-0.2.1.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:34:01.247597 astrohack-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-21 19:33:45.000000 astrohack-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 19:33:45.000000 astrohack-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-21 19:34:01.247597 astrohack-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-21 19:33:45.000000 astrohack-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 19:33:45.000000 astrohack-0.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-21 19:33:45.000000 astrohack-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 19:34:01.247597 astrohack-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:34:01.227599 astrohack-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:34:01.235598 astrohack-0.2.0/src/astrohack/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:34:01.239598 astrohack-0.2.0/src/astrohack/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11213 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/_utils/_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/_utils/_combine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/_utils/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/_utils/_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/_utils/_dask_graph_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:34:01.239598 astrohack-0.2.0/src/astrohack/_utils/_dask_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/_utils/_dask_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     9171 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/_utils/_diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (123)    19855 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/_utils/_dio.py
--rw-r--r--   0 runner    (1001) docker     (123)    22280 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/_utils/_extract_holog.py
--rw-r--r--   0 runner    (1001) docker     (123)    12084 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/_utils/_extract_point.py
--rw-r--r--   0 runner    (1001) docker     (123)    25434 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/_utils/_gaussfitter.py
--rw-r--r--   0 runner    (1001) docker     (123)    22627 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/_utils/_holog.py
--rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/_utils/_imaging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:34:01.239598 astrohack-0.2.0/src/astrohack/_utils/_logger/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/_utils/_logger/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5482 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/_utils/_logger/_astrohack_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/_utils/_panel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:34:01.239598 astrohack-0.2.0/src/astrohack/_utils/_panel_classes/
--rw-r--r--   0 runner    (1001) docker     (123)    36145 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/_utils/_panel_classes/antenna_surface.py
--rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/_utils/_panel_classes/base_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/_utils/_panel_classes/polygon_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/_utils/_panel_classes/ring_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/_utils/_panel_classes/telescope.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:34:01.243597 astrohack-0.2.0/src/astrohack/_utils/_param_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/_utils/_param_utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2156 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/_utils/_param_utils/_check_logger_parms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/_utils/_param_utils/_check_parms.py
--rw-r--r--   0 runner    (1001) docker     (123)    27855 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/_utils/_phase_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)    14720 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/_utils/_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     6380 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/astrohack_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/combine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:34:01.227599 astrohack-0.2.0/src/astrohack/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:34:01.243597 astrohack-0.2.0/src/astrohack/data/.file_meta_data/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/data/.file_meta_data/J1924-2914.ms.calibrated.split.SPW3.json
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after_fixed.split.json
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before_fixed_split.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:34:01.243597 astrohack-0.2.0/src/astrohack/data/telescopes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/data/telescopes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:34:01.243597 astrohack-0.2.0/src/astrohack/data/telescopes/aca_7m.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/data/telescopes/aca_7m.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/data/telescopes/aca_7m.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/data/telescopes/aca_7m.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:34:01.243597 astrohack-0.2.0/src/astrohack/data/telescopes/alma_da.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/data/telescopes/alma_da.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/data/telescopes/alma_da.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/data/telescopes/alma_da.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:34:01.243597 astrohack-0.2.0/src/astrohack/data/telescopes/alma_dv.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/data/telescopes/alma_dv.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/data/telescopes/alma_dv.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/data/telescopes/alma_dv.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:34:01.243597 astrohack-0.2.0/src/astrohack/data/telescopes/alma_tp.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/data/telescopes/alma_tp.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/data/telescopes/alma_tp.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/data/telescopes/alma_tp.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:34:01.247597 astrohack-0.2.0/src/astrohack/data/telescopes/vla.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/data/telescopes/vla.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/data/telescopes/vla.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/data/telescopes/vla.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:34:01.247597 astrohack-0.2.0/src/astrohack/data/telescopes/vlba.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/data/telescopes/vlba.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/data/telescopes/vlba.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/data/telescopes/vlba.zarr/.zmetadata
--rw-r--r--   0 runner    (1001) docker     (123)     8448 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/dio.py
--rw-r--r--   0 runner    (1001) docker     (123)    28650 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/extract_holog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/extract_pointing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/gdown_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/holog.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/locit.py
--rw-r--r--   0 runner    (1001) docker     (123)    42610 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/mds.py
--rw-r--r--   0 runner    (1001) docker     (123)    11058 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/profiling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:34:01.247597 astrohack-0.2.0/src/astrohack/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/visualization/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:34:01.235598 astrohack-0.2.0/src/astrohack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-21 19:34:01.000000 astrohack-0.2.0/src/astrohack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-07-21 19:34:01.000000 astrohack-0.2.0/src/astrohack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 19:34:01.000000 astrohack-0.2.0/src/astrohack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-21 19:34:01.000000 astrohack-0.2.0/src/astrohack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-21 19:34:01.000000 astrohack-0.2.0/src/astrohack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:54:23.466200 astrohack-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-21 19:54:08.000000 astrohack-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 19:54:08.000000 astrohack-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-21 19:54:23.466200 astrohack-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-21 19:54:08.000000 astrohack-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 19:54:08.000000 astrohack-0.2.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-21 19:54:08.000000 astrohack-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 19:54:23.466200 astrohack-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:54:23.454200 astrohack-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:54:23.458200 astrohack-0.2.1/src/astrohack/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:54:23.462200 astrohack-0.2.1/src/astrohack/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11213 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/_utils/_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/_utils/_combine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/_utils/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/_utils/_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/_utils/_dask_graph_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:54:23.462200 astrohack-0.2.1/src/astrohack/_utils/_dask_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/_utils/_dask_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9171 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/_utils/_diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19855 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/_utils/_dio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22280 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/_utils/_extract_holog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12084 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/_utils/_extract_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25434 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/_utils/_gaussfitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22627 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/_utils/_holog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/_utils/_imaging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:54:23.462200 astrohack-0.2.1/src/astrohack/_utils/_logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/_utils/_logger/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5482 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/_utils/_logger/_astrohack_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/_utils/_panel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:54:23.462200 astrohack-0.2.1/src/astrohack/_utils/_panel_classes/
+-rw-r--r--   0 runner    (1001) docker     (123)    36145 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/_utils/_panel_classes/antenna_surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/_utils/_panel_classes/base_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/_utils/_panel_classes/polygon_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/_utils/_panel_classes/ring_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/_utils/_panel_classes/telescope.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:54:23.462200 astrohack-0.2.1/src/astrohack/_utils/_param_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/_utils/_param_utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2156 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/_utils/_param_utils/_check_logger_parms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/_utils/_param_utils/_check_parms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27855 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/_utils/_phase_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14720 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/_utils/_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6380 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/astrohack_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/combine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:54:23.454200 astrohack-0.2.1/src/astrohack/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:54:23.462200 astrohack-0.2.1/src/astrohack/data/.file_meta_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/data/.file_meta_data/J1924-2914.ms.calibrated.split.SPW3.json
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after_fixed.split.json
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before_fixed_split.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:54:23.462200 astrohack-0.2.1/src/astrohack/data/telescopes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/data/telescopes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:54:23.462200 astrohack-0.2.1/src/astrohack/data/telescopes/aca_7m.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/data/telescopes/aca_7m.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/data/telescopes/aca_7m.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/data/telescopes/aca_7m.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:54:23.466200 astrohack-0.2.1/src/astrohack/data/telescopes/alma_da.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/data/telescopes/alma_da.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/data/telescopes/alma_da.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/data/telescopes/alma_da.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:54:23.466200 astrohack-0.2.1/src/astrohack/data/telescopes/alma_dv.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/data/telescopes/alma_dv.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/data/telescopes/alma_dv.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/data/telescopes/alma_dv.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:54:23.466200 astrohack-0.2.1/src/astrohack/data/telescopes/alma_tp.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/data/telescopes/alma_tp.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/data/telescopes/alma_tp.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/data/telescopes/alma_tp.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:54:23.466200 astrohack-0.2.1/src/astrohack/data/telescopes/vla.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/data/telescopes/vla.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/data/telescopes/vla.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/data/telescopes/vla.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:54:23.466200 astrohack-0.2.1/src/astrohack/data/telescopes/vlba.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/data/telescopes/vlba.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/data/telescopes/vlba.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/data/telescopes/vlba.zarr/.zmetadata
+-rw-r--r--   0 runner    (1001) docker     (123)     8448 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/dio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28650 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/extract_holog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/extract_pointing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/gdown_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/holog.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/locit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42610 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/mds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11058 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/profiling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:54:23.466200 astrohack-0.2.1/src/astrohack/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/visualization/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:54:23.458200 astrohack-0.2.1/src/astrohack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-21 19:54:23.000000 astrohack-0.2.1/src/astrohack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-07-21 19:54:23.000000 astrohack-0.2.1/src/astrohack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 19:54:23.000000 astrohack-0.2.1/src/astrohack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-21 19:54:23.000000 astrohack-0.2.1/src/astrohack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-21 19:54:23.000000 astrohack-0.2.1/src/astrohack.egg-info/top_level.txt
```

### Comparing `astrohack-0.2.0/LICENSE` & `astrohack-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.0/PKG-INFO` & `astrohack-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astrohack
-Version: 0.2.0
+Version: 0.2.1
 Summary: Holography Antenna Commissioning Kit
 Author-email: Jan-Willem Steeb <jsteeb@nrao.edu>, Joshua Hoskins <jhoskins@nrao.edu>, Victor de Souza Magalhaes <vdesouza@nrao.edu>
 Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 License-File: LICENSE
```

### Comparing `astrohack-0.2.0/README.md` & `astrohack-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.0/pyproject.toml` & `astrohack-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "astrohack"
-version = "0.2.0"
+version = "0.2.1"
 description = "Holography Antenna Commissioning Kit"
 authors = [
     {name = "Jan-Willem Steeb", email="jsteeb@nrao.edu"},
     {name = "Joshua Hoskins", email="jhoskins@nrao.edu"}, 
     {name = "Victor de Souza Magalhaes", email="vdesouza@nrao.edu"}
 ]
 license = {file = "LICENSE.txt"}
```

### Comparing `astrohack-0.2.0/src/astrohack/_utils/_algorithms.py` & `astrohack-0.2.1/src/astrohack/_utils/_algorithms.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.0/src/astrohack/_utils/_combine.py` & `astrohack-0.2.1/src/astrohack/_utils/_combine.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.0/src/astrohack/_utils/_constants.py` & `astrohack-0.2.1/src/astrohack/_utils/_constants.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.0/src/astrohack/_utils/_conversion.py` & `astrohack-0.2.1/src/astrohack/_utils/_conversion.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.0/src/astrohack/_utils/_dask_graph_tools.py` & `astrohack-0.2.1/src/astrohack/_utils/_dask_graph_tools.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.0/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py` & `astrohack-0.2.1/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.0/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py` & `astrohack-0.2.1/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.0/src/astrohack/_utils/_diagnostics.py` & `astrohack-0.2.1/src/astrohack/_utils/_diagnostics.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.0/src/astrohack/_utils/_dio.py` & `astrohack-0.2.1/src/astrohack/_utils/_dio.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.0/src/astrohack/_utils/_extract_holog.py` & `astrohack-0.2.1/src/astrohack/_utils/_extract_holog.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.0/src/astrohack/_utils/_extract_point.py` & `astrohack-0.2.1/src/astrohack/_utils/_extract_point.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.0/src/astrohack/_utils/_gaussfitter.py` & `astrohack-0.2.1/src/astrohack/_utils/_gaussfitter.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.0/src/astrohack/_utils/_holog.py` & `astrohack-0.2.1/src/astrohack/_utils/_holog.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.0/src/astrohack/_utils/_imaging.py` & `astrohack-0.2.1/src/astrohack/_utils/_imaging.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.0/src/astrohack/_utils/_logger/_astrohack_logger.py` & `astrohack-0.2.1/src/astrohack/_utils/_logger/_astrohack_logger.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.0/src/astrohack/_utils/_panel.py` & `astrohack-0.2.1/src/astrohack/_utils/_panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.0/src/astrohack/_utils/_panel_classes/antenna_surface.py` & `astrohack-0.2.1/src/astrohack/_utils/_panel_classes/antenna_surface.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.0/src/astrohack/_utils/_panel_classes/base_panel.py` & `astrohack-0.2.1/src/astrohack/_utils/_panel_classes/base_panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.0/src/astrohack/_utils/_panel_classes/polygon_panel.py` & `astrohack-0.2.1/src/astrohack/_utils/_panel_classes/polygon_panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.0/src/astrohack/_utils/_panel_classes/ring_panel.py` & `astrohack-0.2.1/src/astrohack/_utils/_panel_classes/ring_panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.0/src/astrohack/_utils/_panel_classes/telescope.py` & `astrohack-0.2.1/src/astrohack/_utils/_panel_classes/telescope.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.0/src/astrohack/_utils/_param_utils/_check_logger_parms.py` & `astrohack-0.2.1/src/astrohack/_utils/_param_utils/_check_logger_parms.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.0/src/astrohack/_utils/_param_utils/_check_parms.py` & `astrohack-0.2.1/src/astrohack/_utils/_param_utils/_check_parms.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.0/src/astrohack/_utils/_phase_fitting.py` & `astrohack-0.2.1/src/astrohack/_utils/_phase_fitting.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.0/src/astrohack/_utils/_tools.py` & `astrohack-0.2.1/src/astrohack/_utils/_tools.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.0/src/astrohack/astrohack_client.py` & `astrohack-0.2.1/src/astrohack/astrohack_client.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.0/src/astrohack/combine.py` & `astrohack-0.2.1/src/astrohack/combine.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.0/src/astrohack/data/.file_meta_data/J1924-2914.ms.calibrated.split.SPW3.json` & `astrohack-0.2.1/src/astrohack/data/.file_meta_data/J1924-2914.ms.calibrated.split.SPW3.json`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.0/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after_fixed.split.json` & `astrohack-0.2.1/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after_fixed.split.json`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.0/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before_fixed_split.json` & `astrohack-0.2.1/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before_fixed_split.json`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.0/src/astrohack/data/telescopes/aca_7m.zarr/.zattrs` & `astrohack-0.2.1/src/astrohack/data/telescopes/aca_7m.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.0/src/astrohack/data/telescopes/aca_7m.zarr/.zmetadata` & `astrohack-0.2.1/src/astrohack/data/telescopes/aca_7m.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.0/src/astrohack/data/telescopes/alma_da.zarr/.zattrs` & `astrohack-0.2.1/src/astrohack/data/telescopes/alma_da.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.0/src/astrohack/data/telescopes/alma_da.zarr/.zmetadata` & `astrohack-0.2.1/src/astrohack/data/telescopes/alma_da.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.0/src/astrohack/data/telescopes/alma_dv.zarr/.zattrs` & `astrohack-0.2.1/src/astrohack/data/telescopes/alma_dv.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.0/src/astrohack/data/telescopes/alma_dv.zarr/.zmetadata` & `astrohack-0.2.1/src/astrohack/data/telescopes/alma_dv.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.0/src/astrohack/data/telescopes/alma_tp.zarr/.zattrs` & `astrohack-0.2.1/src/astrohack/data/telescopes/alma_tp.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.0/src/astrohack/data/telescopes/alma_tp.zarr/.zmetadata` & `astrohack-0.2.1/src/astrohack/data/telescopes/alma_tp.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.0/src/astrohack/data/telescopes/vla.zarr/.zattrs` & `astrohack-0.2.1/src/astrohack/data/telescopes/vla.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.0/src/astrohack/data/telescopes/vla.zarr/.zmetadata` & `astrohack-0.2.1/src/astrohack/data/telescopes/vla.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.0/src/astrohack/data/telescopes/vlba.zarr/.zattrs` & `astrohack-0.2.1/src/astrohack/data/telescopes/vlba.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.0/src/astrohack/data/telescopes/vlba.zarr/.zmetadata` & `astrohack-0.2.1/src/astrohack/data/telescopes/vlba.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.0/src/astrohack/dio.py` & `astrohack-0.2.1/src/astrohack/dio.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.0/src/astrohack/extract_holog.py` & `astrohack-0.2.1/src/astrohack/extract_holog.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.0/src/astrohack/extract_pointing.py` & `astrohack-0.2.1/src/astrohack/extract_pointing.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.0/src/astrohack/gdown_utils.py` & `astrohack-0.2.1/src/astrohack/gdown_utils.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.0/src/astrohack/holog.py` & `astrohack-0.2.1/src/astrohack/holog.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.0/src/astrohack/mds.py` & `astrohack-0.2.1/src/astrohack/mds.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.0/src/astrohack/panel.py` & `astrohack-0.2.1/src/astrohack/panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.0/src/astrohack/profiling.py` & `astrohack-0.2.1/src/astrohack/profiling.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.0/src/astrohack/visualization/viewer.py` & `astrohack-0.2.1/src/astrohack/visualization/viewer.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.0/src/astrohack.egg-info/PKG-INFO` & `astrohack-0.2.1/src/astrohack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astrohack
-Version: 0.2.0
+Version: 0.2.1
 Summary: Holography Antenna Commissioning Kit
 Author-email: Jan-Willem Steeb <jsteeb@nrao.edu>, Joshua Hoskins <jhoskins@nrao.edu>, Victor de Souza Magalhaes <vdesouza@nrao.edu>
 Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 License-File: LICENSE
```

### Comparing `astrohack-0.2.0/src/astrohack.egg-info/SOURCES.txt` & `astrohack-0.2.1/src/astrohack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

