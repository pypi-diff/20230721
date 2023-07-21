# Comparing `tmp/astrohack-0.1.8.tar.gz` & `tmp/astrohack-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astrohack-0.1.8.tar", last modified: Mon Jul 10 18:41:42 2023, max compression
+gzip compressed data, was "astrohack-0.2.0.tar", last modified: Fri Jul 21 19:34:01 2023, max compression
```

## Comparing `astrohack-0.1.8.tar` & `astrohack-0.2.0.tar`

### file list

```diff
@@ -1,95 +1,96 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:41:42.006725 astrohack-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-10 18:41:23.000000 astrohack-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 18:41:23.000000 astrohack-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-10 18:41:42.006725 astrohack-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-10 18:41:23.000000 astrohack-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 18:41:23.000000 astrohack-0.1.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-10 18:41:23.000000 astrohack-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 18:41:42.006725 astrohack-0.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:41:41.986724 astrohack-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:41:41.990724 astrohack-0.1.8/src/astrohack/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:41:41.998725 astrohack-0.1.8/src/astrohack/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11224 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/_utils/_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/_utils/_combine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/_utils/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/_utils/_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/_utils/_dask_graph_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:41:41.998725 astrohack-0.1.8/src/astrohack/_utils/_dask_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/_utils/_dask_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     9171 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/_utils/_diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (123)    19864 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/_utils/_dio.py
--rw-r--r--   0 runner    (1001) docker     (123)    22554 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/_utils/_extract_holog.py
--rw-r--r--   0 runner    (1001) docker     (123)    12086 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/_utils/_extract_point.py
--rw-r--r--   0 runner    (1001) docker     (123)    25434 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/_utils/_gaussfitter.py
--rw-r--r--   0 runner    (1001) docker     (123)    22951 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/_utils/_holog.py
--rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/_utils/_imaging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:41:41.998725 astrohack-0.1.8/src/astrohack/_utils/_logger/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/_utils/_logger/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5462 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/_utils/_logger/_astrohack_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/_utils/_panel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:41:41.998725 astrohack-0.1.8/src/astrohack/_utils/_panel_classes/
--rw-r--r--   0 runner    (1001) docker     (123)    36145 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/_utils/_panel_classes/antenna_surface.py
--rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/_utils/_panel_classes/base_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/_utils/_panel_classes/polygon_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/_utils/_panel_classes/ring_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/_utils/_panel_classes/telescope.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:41:42.002725 astrohack-0.1.8/src/astrohack/_utils/_parm_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/_utils/_parm_utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2156 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/_utils/_parm_utils/_check_logger_parms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/_utils/_parm_utils/_check_parms.py
--rw-r--r--   0 runner    (1001) docker     (123)    27855 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/_utils/_phase_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)    14430 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/_utils/_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/astrohack_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/combine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:41:41.986724 astrohack-0.1.8/src/astrohack/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:41:42.002725 astrohack-0.1.8/src/astrohack/data/.file_meta_data/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/data/.file_meta_data/J1924-2914.ms.calibrated.split.SPW3.json
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after_fixed.split.json
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before_fixed_split.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:41:42.002725 astrohack-0.1.8/src/astrohack/data/telescopes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/data/telescopes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:41:42.002725 astrohack-0.1.8/src/astrohack/data/telescopes/aca_7m.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/data/telescopes/aca_7m.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/data/telescopes/aca_7m.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/data/telescopes/aca_7m.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:41:42.002725 astrohack-0.1.8/src/astrohack/data/telescopes/alma_da.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/data/telescopes/alma_da.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/data/telescopes/alma_da.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/data/telescopes/alma_da.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:41:42.002725 astrohack-0.1.8/src/astrohack/data/telescopes/alma_dv.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/data/telescopes/alma_dv.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/data/telescopes/alma_dv.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/data/telescopes/alma_dv.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:41:42.006725 astrohack-0.1.8/src/astrohack/data/telescopes/alma_tp.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/data/telescopes/alma_tp.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/data/telescopes/alma_tp.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/data/telescopes/alma_tp.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:41:42.006725 astrohack-0.1.8/src/astrohack/data/telescopes/vla.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/data/telescopes/vla.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/data/telescopes/vla.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/data/telescopes/vla.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:41:42.006725 astrohack-0.1.8/src/astrohack/data/telescopes/vlba.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/data/telescopes/vlba.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/data/telescopes/vlba.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/data/telescopes/vlba.zarr/.zmetadata
--rw-r--r--   0 runner    (1001) docker     (123)     8448 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/dio.py
--rw-r--r--   0 runner    (1001) docker     (123)    33264 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/extract_holog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/gdown_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11115 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/holog.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/locit.py
--rw-r--r--   0 runner    (1001) docker     (123)    42606 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/mds.py
--rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/profiling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:41:42.006725 astrohack-0.1.8/src/astrohack/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/visualization/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:41:41.994724 astrohack-0.1.8/src/astrohack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-10 18:41:41.000000 astrohack-0.1.8/src/astrohack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-07-10 18:41:41.000000 astrohack-0.1.8/src/astrohack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 18:41:41.000000 astrohack-0.1.8/src/astrohack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-10 18:41:41.000000 astrohack-0.1.8/src/astrohack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-10 18:41:41.000000 astrohack-0.1.8/src/astrohack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:34:01.247597 astrohack-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-21 19:33:45.000000 astrohack-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 19:33:45.000000 astrohack-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-21 19:34:01.247597 astrohack-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-21 19:33:45.000000 astrohack-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 19:33:45.000000 astrohack-0.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-21 19:33:45.000000 astrohack-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 19:34:01.247597 astrohack-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:34:01.227599 astrohack-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:34:01.235598 astrohack-0.2.0/src/astrohack/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:34:01.239598 astrohack-0.2.0/src/astrohack/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11213 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/_utils/_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/_utils/_combine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/_utils/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/_utils/_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/_utils/_dask_graph_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:34:01.239598 astrohack-0.2.0/src/astrohack/_utils/_dask_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/_utils/_dask_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9171 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/_utils/_diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19855 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/_utils/_dio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22280 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/_utils/_extract_holog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12084 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/_utils/_extract_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25434 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/_utils/_gaussfitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22627 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/_utils/_holog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/_utils/_imaging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:34:01.239598 astrohack-0.2.0/src/astrohack/_utils/_logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/_utils/_logger/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5482 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/_utils/_logger/_astrohack_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/_utils/_panel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:34:01.239598 astrohack-0.2.0/src/astrohack/_utils/_panel_classes/
+-rw-r--r--   0 runner    (1001) docker     (123)    36145 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/_utils/_panel_classes/antenna_surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/_utils/_panel_classes/base_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/_utils/_panel_classes/polygon_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/_utils/_panel_classes/ring_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/_utils/_panel_classes/telescope.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:34:01.243597 astrohack-0.2.0/src/astrohack/_utils/_param_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/_utils/_param_utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2156 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/_utils/_param_utils/_check_logger_parms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/_utils/_param_utils/_check_parms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27855 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/_utils/_phase_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14720 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/_utils/_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6380 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/astrohack_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/combine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:34:01.227599 astrohack-0.2.0/src/astrohack/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:34:01.243597 astrohack-0.2.0/src/astrohack/data/.file_meta_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/data/.file_meta_data/J1924-2914.ms.calibrated.split.SPW3.json
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after_fixed.split.json
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before_fixed_split.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:34:01.243597 astrohack-0.2.0/src/astrohack/data/telescopes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/data/telescopes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:34:01.243597 astrohack-0.2.0/src/astrohack/data/telescopes/aca_7m.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/data/telescopes/aca_7m.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/data/telescopes/aca_7m.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/data/telescopes/aca_7m.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:34:01.243597 astrohack-0.2.0/src/astrohack/data/telescopes/alma_da.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/data/telescopes/alma_da.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/data/telescopes/alma_da.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/data/telescopes/alma_da.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:34:01.243597 astrohack-0.2.0/src/astrohack/data/telescopes/alma_dv.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/data/telescopes/alma_dv.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/data/telescopes/alma_dv.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/data/telescopes/alma_dv.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:34:01.243597 astrohack-0.2.0/src/astrohack/data/telescopes/alma_tp.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/data/telescopes/alma_tp.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/data/telescopes/alma_tp.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/data/telescopes/alma_tp.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:34:01.247597 astrohack-0.2.0/src/astrohack/data/telescopes/vla.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/data/telescopes/vla.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/data/telescopes/vla.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/data/telescopes/vla.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:34:01.247597 astrohack-0.2.0/src/astrohack/data/telescopes/vlba.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/data/telescopes/vlba.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/data/telescopes/vlba.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/data/telescopes/vlba.zarr/.zmetadata
+-rw-r--r--   0 runner    (1001) docker     (123)     8448 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/dio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28650 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/extract_holog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/extract_pointing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/gdown_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/holog.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/locit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42610 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/mds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11058 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/profiling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:34:01.247597 astrohack-0.2.0/src/astrohack/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-07-21 19:33:45.000000 astrohack-0.2.0/src/astrohack/visualization/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:34:01.235598 astrohack-0.2.0/src/astrohack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-21 19:34:01.000000 astrohack-0.2.0/src/astrohack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-07-21 19:34:01.000000 astrohack-0.2.0/src/astrohack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 19:34:01.000000 astrohack-0.2.0/src/astrohack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-21 19:34:01.000000 astrohack-0.2.0/src/astrohack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-21 19:34:01.000000 astrohack-0.2.0/src/astrohack.egg-info/top_level.txt
```

### Comparing `astrohack-0.1.8/LICENSE` & `astrohack-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.8/PKG-INFO` & `astrohack-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astrohack
-Version: 0.1.8
+Version: 0.2.0
 Summary: Holography Antenna Commissioning Kit
 Author-email: Jan-Willem Steeb <jsteeb@nrao.edu>, Joshua Hoskins <jhoskins@nrao.edu>, Victor de Souza Magalhaes <vdesouza@nrao.edu>
 Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 License-File: LICENSE
```

### Comparing `astrohack-0.1.8/README.md` & `astrohack-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.8/pyproject.toml` & `astrohack-0.2.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "astrohack"
-version = "0.1.8"
+version = "0.2.0"
 description = "Holography Antenna Commissioning Kit"
 authors = [
     {name = "Jan-Willem Steeb", email="jsteeb@nrao.edu"},
     {name = "Joshua Hoskins", email="jhoskins@nrao.edu"}, 
     {name = "Victor de Souza Magalhaes", email="vdesouza@nrao.edu"}
 ]
 license = {file = "LICENSE.txt"}
@@ -18,14 +18,16 @@
 'gdown',
 'matplotlib',
 'memory_profiler',
 'numba>=0.57.0',
 'numpy',
 'prettytable',
 'pytest',
+'pytest-cov',
+'pytest-html',
 'scikit_image',
 'scipy',
 'xarray',
 'zarr',
 'bokeh',
 'jupyterlab',
 'python_casacore>=3.5.2; sys_platform != "darwin" '
```

### Comparing `astrohack-0.1.8/src/astrohack/_utils/_algorithms.py` & `astrohack-0.2.0/src/astrohack/_utils/_algorithms.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,37 +205,39 @@
         for it0 in range(shape[0]):
             results[it0], variances[it0] = _least_squares_fit_block(system[it0], vector[it0])
     else:
         results, variances, _ = _least_squares_fit(system, vector)
     return results, variances
     
     
-def _get_grid_parms(vis_map_dict,pnt_map_dict, ant_names):
+def _get_grid_parms(vis_map_dict, pnt_map_dict, ant_names):
     
     grid_parms = {}
+
     for ant_index in vis_map_dict.keys():
-        abs_diff = np.abs(np.diff(pnt_map_dict['ant_'+ant_names[ant_index]]['POINTING_OFFSET'],axis=0))
-        
+        abs_diff = np.abs(np.diff(pnt_map_dict['ant_'+ant_names[ant_index]]['POINTING_OFFSET'], axis=0))
+
         max_dis_x = np.max(abs_diff[:,0])/100
         max_dis_y = np.max(abs_diff[:,1])/100
-        
+
         n_pix_x = np.sum([abs_diff[:,0] > max_dis_x]) + 1
         n_pix_y = np.sum([abs_diff[:,1] > max_dis_y]) + 1
         
         cell_size_x = np.mean(abs_diff[abs_diff[:,0] > max_dis_x,0])
         cell_size_y = np.mean(abs_diff[abs_diff[:,1] > max_dis_y,1])
         
         if n_pix_x < n_pix_y:
             n_pix = n_pix_x**2
             cell_size = cell_size_x
+
         else:
             n_pix = n_pix_y**2
             cell_size = cell_size_y
         
-        grid_parms['ant_'+ant_names[ant_index]] = {'n_pix':n_pix,'cell_size':cell_size}
+        grid_parms['ant_'+ant_names[ant_index]] = {'n_pix':n_pix, 'cell_size':cell_size}
 
     return grid_parms
 
 def _significant_digits(x, digits):
     if np.isscalar(x):
         return _significant_digits_scalar(x,digits)
     else:
```

### Comparing `astrohack-0.1.8/src/astrohack/_utils/_combine.py` & `astrohack-0.2.0/src/astrohack/_utils/_combine.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.8/src/astrohack/_utils/_constants.py` & `astrohack-0.2.0/src/astrohack/_utils/_constants.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.8/src/astrohack/_utils/_conversion.py` & `astrohack-0.2.0/src/astrohack/_utils/_conversion.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.8/src/astrohack/_utils/_dask_graph_tools.py` & `astrohack-0.2.0/src/astrohack/_utils/_dask_graph_tools.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.8/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py` & `astrohack-0.2.0/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.8/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py` & `astrohack-0.2.0/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.8/src/astrohack/_utils/_diagnostics.py` & `astrohack-0.2.0/src/astrohack/_utils/_diagnostics.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.8/src/astrohack/_utils/_dio.py` & `astrohack-0.2.0/src/astrohack/_utils/_dio.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,45 @@
 import os
 import json
 import zarr
 import copy
 import datetime
 import shutil
+import inspect
+
 import numpy as np
 import xarray as xr
 
 from astropy.io import fits
 from astrohack import __version__ as code_version
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
-from astrohack._utils._tools import _numpy_to_json, _add_prefix
 
-DIMENSION_KEY = "_ARRAY_DIMENSIONS"
+from astrohack._utils._tools import _add_prefix
+from astrohack._utils._tools import NumpyEncoder
 
+DIMENSION_KEY = "_ARRAY_DIMENSIONS"
+CALLING_FUNCTION=1
 
-def check_if_file_exists(caller, file):
+def _check_if_file_exists(file):
     logger = _get_astrohack_logger()
+    caller = inspect.stack()[CALLING_FUNCTION].function
 
     if os.path.exists(file) is False:
         logger.error(f'[{caller}]: File {file} does not exists.')
         raise FileNotFoundError
 
 
-def check_if_file_will_be_overwritten(caller, file, overwrite):
+def _check_if_file_will_be_overwritten(file, overwrite):
     logger = _get_astrohack_logger()
+    caller=inspect.stack()[CALLING_FUNCTION].function
+    
     if (os.path.exists(file) is True) and (overwrite is False):
         logger.error(f'[{caller}]: {file} already exists. To overwite set overwrite to True, or remove current file.')
-        raise FileExistsError
+        
+        raise FileExistsError("{file} exists.".format(file=file))
         
     elif  (os.path.exists(file) is True) and (overwrite is True):
         if file.endswith(".zarr"):
             logger.warning(f'[{caller}]: {file} will be overwritten.')
             shutil.rmtree(file)
         else:
             logger.warning(f'[{caller}]: {file} may not be valid hack file. Check the file name again.')
@@ -311,15 +319,14 @@
         if dask_load:
             return xr.open_zarr(image_path)
         else:
             return _open_no_dask_zarr(image_path)
     else:
         raise FileNotFoundError("Image file: {} not found".format(image_path))
 
-
 def _read_meta_data(file_name, file_type, origin):
     """Reads dimensional data from holog meta file.
 
     Args:
         file_name (str): astorhack file name.
         file_type (str): astrohack file type
         origin (str, list): Astrohack expected origin(s)
@@ -331,32 +338,41 @@
     
     try:
         with open(f'{file_name}/.{file_type}_attr') as json_file:
             json_dict = json.load(json_file)
 
     except Exception as error:
         logger.error(str(error))
-        raise
-        
-
+        raise Exception   
+    
+    # I don't see the use case for this or the origin in general. This means I need to either look at the
+    # meta data of a file I want to open ahead of time or list all possible unctions that could have made it.
+    
+    
     try:
         metadataorigin = json_dict['origin']
     except KeyError:
         logger.error("[_read_meta_data]: Badly formatted metadata in input file")
+        
         raise Exception('Bad metadata')
+
     if isinstance(origin, str):
         if metadataorigin != origin:
             logger.error(f"[_read_meta_data]: Input file is not an Astrohack {file_type} file")
             logger.error(f"Expected origin was {origin} but got {metadataorigin}")
+            
             raise TypeError('Incorrect file type')
+
     elif isinstance(origin, (list, tuple)):
         if metadataorigin not in origin:
             logger.error(f"[_read_meta_data]: Input file is not an Astrohack {file_type} file")
             logger.error(f"Expected origin was {origin} but got {metadataorigin}")
+            
             raise TypeError('Incorrect file type')
+    
 
     return json_dict
 
 
 def _check_mds_origin(file_name, file_type):
     """
 
@@ -364,14 +380,15 @@
         file_name(str): astrohack file name.
         file_type(str, list): accepted astrohack file type
 
     Returns: origin(str) the origin of the mds file
 
     """
     logger = _get_astrohack_logger()
+
     if isinstance(file_type, str):
         file_type = [file_type]
 
     for ftype in file_type:
         try:
             with open(f'{file_name}/.{ftype}_attr') as json_file:
                 json_dict = json.load(json_file)
@@ -389,43 +406,36 @@
     except KeyError:
         logger.error("[_check_mds_origin]: Badly formatted metadata in input file")
         raise Exception('Bad metadata')
 
     return metadataorigin
 
 
-def _write_meta_data(origin, file_name, input_dict):
+def _write_meta_data(file_name, input_dict):
     """
     Creates a metadata dictionary that is compatible with JSON and writes it to a file
     Args:
         origin: Which function created the mds
         file_name: Output json file name
         input_dict: Dictionary to be included in the metadata
     """
+
     logger = _get_astrohack_logger()
-    metadata = {'version': code_version,
-                'origin': origin}
-    for key in input_dict.keys():
-        if type(input_dict[key]) == np.ndarray:
-            try:
-                for item in range(len(input_dict[key])):
-                    newkey = f'{key}_{item}'
-                    metadata[newkey] = _numpy_to_json(input_dict[key][item])
-            except TypeError:
-                if len(input_dict['grid_size'].shape) == 0:
-                    metadata[key] = "None"
-                else:
-                    metadata[key] = input_dict[key]
-        elif input_dict[key] is None:
-            metadata[key] = "None"
-        else:
-            metadata[key] = input_dict[key]
+
+    meta_data = copy.deepcopy(input_dict)
+
+    meta_data.update({
+        'version': code_version,
+        'origin': inspect.stack()[CALLING_FUNCTION].function
+    })
+
     try:
         with open(file_name, "w") as json_file:
-            json.dump(metadata, json_file)
+            json.dump(meta_data, json_file, cls=NumpyEncoder)
+
     except Exception as error:
         logger.error("[_write_meta_data] {error}".format(error=error))
 
 
 def _read_data_from_holog_json(holog_file, holog_dict, ant_id, ddi_id=None):
     """Read holog file meta data and extract antenna based xds information for each (ddi, holog_map)
 
@@ -445,15 +455,15 @@
 
     try:
         with open(holog_meta_data, "r") as json_file:
             holog_json = json.load(json_file)
 
     except Exception as error:
         logger.error(str(error))
-        raise
+        raise Exception
 
     ant_data_dict = {}
 
     for ddi in holog_json[ant_id_str].keys():
         if "ddi_" in ddi:
             if (ddi_id is not None) and (ddi != ddi_id):
                 continue
```

### Comparing `astrohack-0.1.8/src/astrohack/_utils/_extract_holog.py` & `astrohack-0.2.0/src/astrohack/_utils/_extract_holog.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
 
     map_ant_name_list = list(map(str, map_ant_name_tuple))
 
     map_ant_name_list = ['ant_' + i for i in map_ant_name_list]
 
     pnt_ant_dict = _load_point_file(pnt_name, map_ant_name_list, dask_load=False)
     pnt_map_dict = _extract_pointing_chunk(map_ant_name_list, time_vis, pnt_ant_dict)
-    grid_parms = _get_grid_parms(vis_map_dict,pnt_map_dict, ant_names)
+    grid_parms = _get_grid_parms(vis_map_dict, pnt_map_dict, ant_names)
     
     ### To DO:
     ################### Average multiple repeated samples
     #over_flow_protector_constant = float("%.5g" % time_vis[0])  # For example 5076846059.4 -> 5076800000.0
     #time_vis = time_vis - over_flow_protector_constant
     #from astrohack._utils._algorithms import _average_repeated_pointings
     #time_vis = _average_repeated_pointings(vis_map_dict, weight_map_dict, flagged_mapping_antennas,time_vis,pnt_map_dict,ant_names)
@@ -534,36 +534,41 @@
                                 ant_holog_dict[ant][ddi] = {map:{}}
                     
                             ant_holog_dict[ant][ddi][map] = xds.to_dict(data=False)
                             cell_sizes.append(xds.attrs["grid_parms"]["cell_size"])
                             n_pixs.append(xds.attrs["grid_parms"]["n_pix"])
                             telescope_names.append(xds.attrs['telescope_name'])
     
-    cell_sizes_sigfigs =  _significant_digits(cell_sizes,digits=3)
+    cell_sizes_sigfigs =  _significant_digits(cell_sizes, digits=3)
+
     if not (len(set(cell_sizes_sigfigs)) == 1):
         logger.error('Cell size not consistant: ' + str(cell_sizes))
         raise
         
     if not (len(set(n_pixs)) == 1):
         logger.error('Number of pixels not consistant: ' + str(n_pixs))
         raise
         
     if not (len(set(telescope_names)) == 1):
         logger.error('Telescope name not consistant: ' + str(telescope_names))
         raise
+
     output_meta_file = "{name}/{ext}".format(name=holog_file, ext=".holog_json")
+    
     try:
         with open(output_meta_file, "w") as json_file:
             json.dump(ant_holog_dict, json_file)
 
     except Exception as error:
         logger.error("[_create_holog_meta_data] {error}".format(error=error))
 
-    meta_data = {'cell_size': np.mean(cell_sizes),
-                 'n_pix': n_pixs[0],
-                 'telescope_name': telescope_names[0]}
+    meta_data = {
+        'cell_size': np.mean(cell_sizes),
+        'n_pix': n_pixs[0],
+        'telescope_name': telescope_names[0]
+    }
+
     meta_data.update(input_params)
-    holog_attr_file = "{name}/{ext}".format(name=holog_file, ext=".holog_attr")
-    _write_meta_data('extract_holog', holog_attr_file, meta_data)
-    point_attr_file = "{name}/{ext}".format(name=input_params['point_name'], ext=".point_attr")
-    _write_meta_data('extract_holog', point_attr_file, input_params)
+    
+    return meta_data
+
```

### Comparing `astrohack-0.1.8/src/astrohack/_utils/_extract_point.py` & `astrohack-0.2.0/src/astrohack/_utils/_extract_point.py`

 * *Files 0% similar despite different names*

```diff
@@ -296,9 +296,8 @@
                     if  scan_time_dict[ddi][s][1] < t:
                         scan_time_dict[ddi][s][1] = t
                 else:
                     scan_time_dict[ddi][s] = np.array([t,t])
             else:
                 scan_time_dict[ddi] = {s: np.array([t,t])}
   
-    return scan_time_dict
-
+    return scan_time_dict
```

### Comparing `astrohack-0.1.8/src/astrohack/_utils/_gaussfitter.py` & `astrohack-0.2.0/src/astrohack/_utils/_gaussfitter.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.8/src/astrohack/_utils/_holog.py` & `astrohack-0.2.0/src/astrohack/_utils/_holog.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,22 +37,22 @@
     Args:
         holog_chunk_params (dict): Dictionary containing holography parameters.
     """
     logger = _get_astrohack_logger()
     fname = 'holog'
 
     holog_file, ant_data_dict = _load_holog_file(
-        holog_chunk_params["holog_file"],
+        holog_chunk_params["holog_name"],
         dask_load=False,
         load_pnt_dict=False,
         ant_id=holog_chunk_params["this_ant"],
         ddi_id=holog_chunk_params["this_ddi"]
     )
 
-    meta_data = _read_meta_data(holog_chunk_params["holog_file"], 'holog', 'extract_holog')
+    meta_data = _read_meta_data(holog_chunk_params["holog_name"], 'holog', 'extract_holog')
 
     # Calculate lm coordinates
     l, m = _calc_coords(holog_chunk_params["grid_size"], holog_chunk_params["cell_size"])
     grid_l, grid_m = list(map(np.transpose, np.meshgrid(l, m)))
     
     to_stokes = holog_chunk_params["to_stokes"]
 
@@ -264,21 +264,29 @@
     xds.attrs["aperture_resolution"] = aperture_resolution
     xds.attrs["ant_id"] = holog_chunk_params["this_ant"]
     xds.attrs["ant_name"] = ant_name
     xds.attrs["telescope_name"] = meta_data['telescope_name']
     xds.attrs["time_centroid"] = np.array(time_centroid)
     xds.attrs["ddi"] = ddi
 
-    coords = {"ddi": list(ant_data_dict.keys()), "pol": pol, "l": l, "m": m, "u": u, "v": v, "u_prime": u_prime,
-              "v_prime": v_prime, "chan": freq_chan}
-    #coords["time"] = np.array(time_centroid)
-
+    coords = {
+        "ddi": list(ant_data_dict.keys()), 
+        "pol": pol, 
+        "l": l, 
+        "m": m, 
+        "u": u, 
+        "v": v, 
+        "u_prime": u_prime,
+        "v_prime": v_prime, 
+        "chan": freq_chan
+    }
+    
     xds = xds.assign_coords(coords)
 
-    xds.to_zarr("{name}/{ant}/{ddi}".format(name=holog_chunk_params["image_file"], ant=holog_chunk_params["this_ant"],
+    xds.to_zarr("{name}/{ant}/{ddi}".format(name=holog_chunk_params["image_name"], ant=holog_chunk_params["this_ant"],
                                             ddi=ddi), mode="w", compute=True, consolidated=True)
 
 
 def _create_average_chan_map(freq_chan, chan_tolerance_factor):
     n_chan = len(freq_chan)
     cf_chan_map = np.zeros((n_chan,), dtype=int)
 
@@ -306,25 +314,14 @@
     cf_chan_map = np.zeros((n_chan,), dtype=int)
     for i in range(n_chan):
         cf_chan_map[i], _ = _find_nearest(pb_freq, freq_chan[i])
 
     return cf_chan_map, pb_freq
 
 
-def _create_image_meta_data(image_file, input_params):
-    """
-    Save image meta data to a json file
-    Args:
-        image_file: image file
-        input_params: holog input parameter dictionaire
-    """
-    output_attr_file = "{name}/{ext}".format(name=image_file, ext=".image_attr")
-    _write_meta_data('holog', output_attr_file, input_params)
-
-
 def _export_to_fits_holog_chunk(parm_dict):
     """
     Holog side chunk function for the user facing function export_to_fits
     Args:
         parm_dict: parameter dictionary
     """
     logger = _get_astrohack_logger()
```

### Comparing `astrohack-0.1.8/src/astrohack/_utils/_imaging.py` & `astrohack-0.2.0/src/astrohack/_utils/_imaging.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.8/src/astrohack/_utils/_logger/_astrohack_logger.py` & `astrohack-0.2.0/src/astrohack/_utils/_logger/_astrohack_logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,17 +32,20 @@
     ERROR = "\x1b[32;31m"   #red
     CRITICAL = "\x1b[31;1m" #bold red
 
     start_msg = "%(asctime)s - "
     middle_msg = "%(levelname)-8s"
     end_msg = " - %(name)s - (%(filename)s:%(lineno)d) - %(message)s"
     
+    import inspect
+
+
     FORMATS = {
         logging.DEBUG: start_msg + DEBUG + middle_msg  + reset + end_msg ,
-        logging.INFO:  start_msg + INFO + middle_msg  + reset + end_msg ,
+        logging.INFO:  start_msg + INFO + middle_msg  + reset + end_msg,
         logging.WARNING:  start_msg + WARNING + middle_msg  + reset + end_msg ,
         logging.ERROR:  start_msg + ERROR + middle_msg  + reset + end_msg ,
         logging.CRITICAL:  start_msg + CRITICAL + middle_msg  + reset + end_msg ,
     }
 
     def format(self, record):
         log_fmt = self.FORMATS.get(record.levelno)
```

### Comparing `astrohack-0.1.8/src/astrohack/_utils/_panel.py` & `astrohack-0.2.0/src/astrohack/_utils/_panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.8/src/astrohack/_utils/_panel_classes/antenna_surface.py` & `astrohack-0.2.0/src/astrohack/_utils/_panel_classes/antenna_surface.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.8/src/astrohack/_utils/_panel_classes/base_panel.py` & `astrohack-0.2.0/src/astrohack/_utils/_panel_classes/base_panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.8/src/astrohack/_utils/_panel_classes/polygon_panel.py` & `astrohack-0.2.0/src/astrohack/_utils/_panel_classes/polygon_panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.8/src/astrohack/_utils/_panel_classes/ring_panel.py` & `astrohack-0.2.0/src/astrohack/_utils/_panel_classes/ring_panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.8/src/astrohack/_utils/_panel_classes/telescope.py` & `astrohack-0.2.0/src/astrohack/_utils/_panel_classes/telescope.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.8/src/astrohack/_utils/_parm_utils/_check_logger_parms.py` & `astrohack-0.2.0/src/astrohack/_utils/_param_utils/_check_logger_parms.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.8/src/astrohack/_utils/_parm_utils/_check_parms.py` & `astrohack-0.2.0/src/astrohack/_utils/_param_utils/_check_parms.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.8/src/astrohack/_utils/_phase_fitting.py` & `astrohack-0.2.0/src/astrohack/_utils/_phase_fitting.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.8/src/astrohack/_utils/_tools.py` & `astrohack-0.2.0/src/astrohack/_utils/_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,33 @@
+import json
+
 import numpy as np
+
 from mpl_toolkits.axes_grid1 import make_axes_locatable
 from prettytable import PrettyTable
 from textwrap import fill
 
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
 
+class NumpyEncoder(json.JSONEncoder):
+    def default(self, obj):
+        if isinstance(obj, np.ndarray):
+            return obj.tolist()
+        
+        elif isinstance(obj, np.floating):
+            return float(obj)
+        
+        elif isinstance(obj, np.integer):
+            return int(obj)
+
+        elif isinstance(obj, NoneType):
+            return "None"
+
+
+        return json.JSONEncoder.default(self, obj)
 
 def _well_positioned_colorbar(ax, fig, image, label, location='right', size='5%', pad=0.05):
     """
     Adds a well positioned colorbar to a plot
     Args:
         ax: Axes instance to add the colorbar
         fig: Figure in which the axes are embedded
@@ -34,14 +53,15 @@
         suffix: The suffix to be removed
 
     Returns: the input string minus suffix
 
     """
     if suffix and input_string.endswith(suffix):
         return input_string[:-len(suffix)]
+        
     return input_string
 
 
 def _jsonify(holog_obj):
     """ Convert holog_obs_description dictionay to json format. This just means converting numpy.ndarry
         entries to string lists.
 
@@ -150,24 +170,17 @@
                 msg = f'[{caller}]: cannot interpret parameter {item} of type {type(item)}'
                 logger.error(msg)
                 raise Exception(msg)
     else:
         msg = f'[{caller}] cannot interpret parameter {parm} of type {type(parm)}'
         logger.error(msg)
         raise Exception(msg)
+        
     return oulist
 
-
-def _numpy_to_json(value):
-    if isinstance(value, np.integer):
-        return int(value)
-    if isinstance(value, np.floating):
-        return float(value)
-
-
 def _split_pointing_table(ms_name, antennas):
     """ Split pointing table to contain only specified antennas
 
     :param ms_name: Measurement file
     :type ms_name: str
     :param antennas: List of antennas to sub-select on.
     :type antennas: list (str)
```

### Comparing `astrohack-0.1.8/src/astrohack/astrohack_client.py` & `astrohack-0.2.0/src/astrohack/astrohack_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import warnings, time, os, psutil, multiprocessing, re
 import dask
 import copy
 import os
 import logging
 import astrohack
-from astrohack._utils._parm_utils._check_logger_parms import _check_logger_parms, _check_worker_logger_parms
+from astrohack._utils._param_utils._check_logger_parms import _check_logger_parms, _check_worker_logger_parms
 from astrohack._utils._logger._astrohack_logger import  _setup_astrohack_logger, _get_astrohack_logger
 from astrohack._utils._dask_plugins._astrohack_worker import _astrohack_worker
 
 def astrohack_local_client(cores=None, memory_limit=None, dask_local_dir=None, log_parms={}, worker_log_parms={}):
     """ Setup dask cluster and astrohack logger.
 
     :param cores: Number of cores in Dask cluster, defaults to None
```

### Comparing `astrohack-0.1.8/src/astrohack/combine.py` & `astrohack-0.2.0/src/astrohack/combine.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 
 from astrohack._utils._combine import _combine_chunk
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
-from astrohack._utils._parm_utils._check_parms import _check_parms, _parm_check_passed
+from astrohack._utils._param_utils._check_parms import _check_parms, _parm_check_passed
 from astrohack._utils._tools import _remove_suffix
-from astrohack._utils._dio import check_if_file_will_be_overwritten, check_if_file_exists, _write_meta_data
+from astrohack._utils._dio import _check_if_file_will_be_overwritten, _check_if_file_exists, _write_meta_data
 from astrohack.mds import AstrohackImageFile
 from astrohack._utils._dask_graph_tools import _dask_general_compute
 
 
 def combine(image_name, combine_name=None, ant_id=None, ddi=None, weighted=False, parallel=False, overwrite=False):
     """Combine DDIs in a Holography image to increase SNR
 
@@ -48,25 +48,25 @@
         }
     """
     logger = _get_astrohack_logger()
     fname = 'combine'
     combine_params = _check_combine_parms(fname, image_name, combine_name, ant_id, ddi, weighted, parallel, overwrite)
     input_params = combine_params.copy()
 
-    check_if_file_exists(fname, combine_params['image_file'])
-    check_if_file_will_be_overwritten(fname, combine_params['combine_file'], combine_params['overwrite'])
+    _check_if_file_exists(combine_params['image_file'])
+    _check_if_file_will_be_overwritten(combine_params['combine_file'], combine_params['overwrite'])
 
     image_mds = AstrohackImageFile(combine_params['image_file'])
     image_mds._open()
     combine_params['image_mds'] = image_mds
 
     if _dask_general_compute(fname, image_mds, _combine_chunk, combine_params, ['ant'], parallel=parallel):
         logger.info(f"[{fname}]: Finished processing")
         output_attr_file = "{name}/{ext}".format(name=combine_params['combine_file'], ext=".image_attr")
-        _write_meta_data('combine', output_attr_file, input_params)
+        _write_meta_data(output_attr_file, input_params)
         combine_mds = AstrohackImageFile(combine_params['combine_file'])
         combine_mds._open()
         return combine_mds
     else:
         logger.warning(f"[{fname}]: No data to process")
         return None
```

### Comparing `astrohack-0.1.8/src/astrohack/data/.file_meta_data/J1924-2914.ms.calibrated.split.SPW3.json` & `astrohack-0.2.0/src/astrohack/data/.file_meta_data/J1924-2914.ms.calibrated.split.SPW3.json`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.8/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after_fixed.split.json` & `astrohack-0.2.0/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after_fixed.split.json`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.8/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before_fixed_split.json` & `astrohack-0.2.0/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before_fixed_split.json`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.8/src/astrohack/data/telescopes/aca_7m.zarr/.zattrs` & `astrohack-0.2.0/src/astrohack/data/telescopes/aca_7m.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.8/src/astrohack/data/telescopes/aca_7m.zarr/.zmetadata` & `astrohack-0.2.0/src/astrohack/data/telescopes/aca_7m.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.8/src/astrohack/data/telescopes/alma_da.zarr/.zattrs` & `astrohack-0.2.0/src/astrohack/data/telescopes/alma_da.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.8/src/astrohack/data/telescopes/alma_da.zarr/.zmetadata` & `astrohack-0.2.0/src/astrohack/data/telescopes/alma_da.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.8/src/astrohack/data/telescopes/alma_dv.zarr/.zattrs` & `astrohack-0.2.0/src/astrohack/data/telescopes/alma_dv.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.8/src/astrohack/data/telescopes/alma_dv.zarr/.zmetadata` & `astrohack-0.2.0/src/astrohack/data/telescopes/alma_dv.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.8/src/astrohack/data/telescopes/alma_tp.zarr/.zattrs` & `astrohack-0.2.0/src/astrohack/data/telescopes/alma_tp.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.8/src/astrohack/data/telescopes/alma_tp.zarr/.zmetadata` & `astrohack-0.2.0/src/astrohack/data/telescopes/alma_tp.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.8/src/astrohack/data/telescopes/vla.zarr/.zattrs` & `astrohack-0.2.0/src/astrohack/data/telescopes/vla.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.8/src/astrohack/data/telescopes/vla.zarr/.zmetadata` & `astrohack-0.2.0/src/astrohack/data/telescopes/vla.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.8/src/astrohack/data/telescopes/vlba.zarr/.zattrs` & `astrohack-0.2.0/src/astrohack/data/telescopes/vlba.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.8/src/astrohack/data/telescopes/vlba.zarr/.zmetadata` & `astrohack-0.2.0/src/astrohack/data/telescopes/vlba.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.8/src/astrohack/dio.py` & `astrohack-0.2.0/src/astrohack/dio.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.8/src/astrohack/extract_holog.py` & `astrohack-0.2.0/src/astrohack/extract_holog.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,70 +1,84 @@
 import os
 import dask
 import json
 import copy
+import inspect 
 import numpy as np
 import numbers
+
 from astropy.time import Time
 
 from pprint import pformat
 
 from casacore import tables as ctables
 
 from astrohack._utils._constants import pol_str
 from astrohack._utils._conversion import _convert_ant_name_to_id
 from astrohack._utils._extract_holog import _create_holog_meta_data
 from astrohack._utils._extract_point import _extract_pointing
 from astrohack._utils._dio import _load_point_file
-from astrohack._utils._dio import  check_if_file_will_be_overwritten, check_if_file_exists
+from astrohack._utils._dio import _check_if_file_will_be_overwritten
+from astrohack._utils._dio import _check_if_file_exists
 from astrohack._utils._dio import _load_holog_file
+from astrohack._utils._dio import _write_meta_data
 from astrohack._utils._extract_holog import _extract_holog_chunk
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
-from astrohack._utils._parm_utils._check_parms import _check_parms, _parm_check_passed
+from astrohack._utils._param_utils._check_parms import _check_parms, _parm_check_passed
 from astrohack._utils._tools import _remove_suffix
 from astrohack._utils._tools import _jsonify
 
 from astrohack.mds import AstrohackHologFile
 
+from astrohack.extract_pointing import extract_pointing
+
+CURRENT_FUNCTION=0
+
 def extract_holog(
     ms_name,
-    holog_obs_dict=None,
-    ddi=None,
-    baseline_average_distance=None,
-    baseline_average_nearest=None,
+    point_name,
     holog_name=None,
-    point_name=None,
+    holog_obs_dict=None,
+    ddi='all',
+    baseline_average_distance='all',
+    baseline_average_nearest='all',
     data_column="CORRECTED_DATA",
     parallel=False,
-    reuse_point_zarr=False,
     overwrite=False,
 ):
     """
     Extract holography and optionally pointing data, from measurement set. Creates holography output file.
 
     :param ms_name: Name of input measurement file name.
     :type ms_name: str
+
+    :param point_name: Name of *<point_name>.point.zarr* file to use.
+    :type holog_name: str
+
+    :param holog_name: Name of *<holog_name>.holog.zarr* file to create. Defaults to measurement set name with *holog.zarr* extension.
+    :type holog_name: str, optional
+
     :param holog_obs_dict: The *holog_obs_dict* describes which scan and antenna data to extract from the measurement set. As detailed below, this compound dictionary also includes important meta data needed for preprocessing and extraction of the holography data from the measurement set. If not specified holog_obs_dict will be generated. For auto generation of the holog_obs_dict the assumtion is made that the same antanna beam is not mapped twice in a row (alternating sets of antennas is fine).
     :type holog_obs_dict: dict, optional
+
     :param ddi:  DDI(s) that should be extracted from the measurement set. Defaults to all DDI's in the ms.
     :type ddi: int numpy.ndarray | int list, optional
+
     :param baseline_average_distance: To increase the signal to noise for a mapping antenna mutiple reference antennas can be used. The baseline_average_distance is the acceptable distance (in meters) between a mapping antenna and a reference antenna. The baseline_average_distance is only used if the holog_obs_dict is not specified. If no distance is specified all reference antennas will be used. baseline_average_distance and baseline_average_nearest can not be used together.
     :type baseline_average_distance: float, optional
+
     :param baseline_average_nearest: To increase the signal to noise for a mapping antenna mutiple reference antennas can be used. The baseline_average_nearest is the number of nearest reference antennas to use. The baseline_average_nearest is only used if the holog_obs_dict is not specified.  baseline_average_distance and baseline_average_nearest can not be used together.
     :type baseline_average_nearest: int, optional
-    :param holog_name: Name of *<holog_name>.holog.zarr* file to create. Defaults to measurement set name with *holog.zarr* extension.
-    :type holog_name: str, optional
-    :param point_name: Name of *<point_name>.point.zarr* file to create. Defaults to measurement set name with *point.zarr* extension.
-    :type point_name: str, optional
+
     :param data_column: Determines the data column to pull from the measurement set. Defaults to "CORRECTED_DATA".
     :type data_column: str, optional, ex. DATA, CORRECTED_DATA
+
     :param parallel: Boolean for whether to process in parallel, defaults to False.
     :type parallel: bool, optional
-    :param reuse_point_zarr: If true the point.zarr specified in point_name is reused, defaults to False.
-    :type reuse_point_zarr: bool, optional
+
     :param overwrite: Boolean for whether to overwrite current holog.zarr and point.zarr files, defaults to False.
     :type overwrite: bool, optional
 
     :return: Holography holog object.
     :rtype: AstrohackHologFile
 
     .. _Description:
@@ -123,123 +137,120 @@
                             'DV23', 'DV24', 'DV25'
                         ]
                     }
                 }
             }
 
     """
+    extract_holog_params = locals()
+
     logger = _get_astrohack_logger()
-    
-    fname = 'extract_holog'
+
+    function_name = inspect.stack()[CURRENT_FUNCTION].function
+
     ######### Parameter Checking #########
-    extract_holog_parms = _check_extract_holog_parms(fname,
-                                                     ms_name,
-                                                     holog_obs_dict,
-                                                     ddi,
-                                                     baseline_average_distance,
-                                                     baseline_average_nearest,
-                                                     holog_name,
-                                                     point_name,
-                                                     data_column,
-                                                     parallel,
-                                                     reuse_point_zarr,
-                                                     overwrite)
-    input_params = extract_holog_parms.copy()
-    
-    check_if_file_exists(fname, extract_holog_parms['ms_name'])
-    check_if_file_will_be_overwritten(fname, extract_holog_parms['holog_name'], extract_holog_parms['overwrite'])
-    
-        
-    ############# Extract pointing infromation and save to point.zarr #############
-    if extract_holog_parms["reuse_point_zarr"]:
-        try:
-            pnt_dict = _load_point_file(extract_holog_parms['point_name'])
-        except:
-            logger.warning(f'[{fname}]: Could not find {extract_holog_parms["point_name"]}, creating point new 'f'point.zarr.')
-
-            # If you tried to reuse .pointing and there was a failure, delete old file and recreate
-            check_if_file_will_be_overwritten(fname, extract_holog_parms['point_name'], True)
-            pnt_dict = _extract_pointing(extract_holog_parms['ms_name'], extract_holog_parms['point_name'], parallel=extract_holog_parms['parallel'])
-    else:
+    extract_holog_params = _check_extract_holog_params(function_name=function_name, extract_holog_params=extract_holog_params)
+    
 
-        # If you don't want to reuse .point delete and recreate
-        check_if_file_will_be_overwritten(fname, extract_holog_parms['point_name'], True)
-        pnt_dict = _extract_pointing(extract_holog_parms['ms_name'], extract_holog_parms['point_name'], parallel=extract_holog_parms['parallel'])
+    _check_if_file_exists(extract_holog_params['ms_name'])
+    _check_if_file_will_be_overwritten(extract_holog_params['holog_name'], extract_holog_params['overwrite'])
+
+    if holog_name==None:
         
+        logger.debug('[{caller}]: File {file} does not exists. Extracting ...'.format(caller=function_name, file=holog_name))
+            
+        from astrohack._utils._tools import _remove_suffix
+
+        holog_name = _remove_suffix(ms_name, '.ms') + '.holog.zarr'
+        extract_holog_params['holog_name'] = holog_name
+            
+        logger.debug('[{caller}]: Extracting holog to {output}'.format(caller=function_name, output=holog_name))
+          
+    try:
+        pnt_dict = _load_point_file(extract_holog_params['point_name'])
+    except:
+        logger.warning(f'[{function_name}]: Could not find {extract_holog_params["point_name"]}, creating point new 'f'point.zarr.')        
 
     ######## Get Spectral Windows ########
     ctb = ctables.table(
-        os.path.join(extract_holog_parms['ms_name'], "DATA_DESCRIPTION"),
+        os.path.join(extract_holog_params['ms_name'], "DATA_DESCRIPTION"),
         readonly=True,
         lockoptions={"option": "usernoread"},
         ack=False,
     )
     ddi_spw = ctb.getcol("SPECTRAL_WINDOW_ID")
     ddpol_indexol = ctb.getcol("POLARIZATION_ID")
     ms_ddi = np.arange(len(ddi_spw))
     ctb.close()
 
     ######## Get Antenna IDs and Names ########
     ctb = ctables.table(
-        os.path.join(extract_holog_parms['ms_name'], "ANTENNA"),
+        os.path.join(extract_holog_params['ms_name'], "ANTENNA"),
         readonly=True,
         lockoptions={"option": "usernoread"},
         ack=False,
     )
 
     ant_names = np.array(ctb.getcol("NAME"))
     ant_id = np.arange(len(ant_names))
     ant_pos = ctb.getcol("POSITION")
 
     ctb.close()
     
     ######## Get Antenna IDs that are in the main table########
     ctb = ctables.table(
-        extract_holog_parms['ms_name'],
+        extract_holog_params['ms_name'],
         readonly=True,
         lockoptions={"option": "usernoread"},
         ack=False,
     )
 
     ant1 = np.unique(ctb.getcol("ANTENNA1"))
     ant2 = np.unique(ctb.getcol("ANTENNA2"))
     ant_id_main = np.unique(np.append(ant1,ant2))
     
     ant_names_main = ant_names[ant_id_main]
     ctb.close()
     
     # Create holog_obs_dict or modify user supplied holog_obs_dict.
-    ddi = extract_holog_parms['ddi_sel']
+    ddi = extract_holog_params['ddi']
+
     if holog_obs_dict is None: #Automatically create holog_obs_dict
         from astrohack._utils._extract_holog import _create_holog_obs_dict
-        holog_obs_dict = _create_holog_obs_dict(pnt_dict, extract_holog_parms['baseline_average_distance'],
-                                                extract_holog_parms['baseline_average_nearest'], ant_names, ant_pos,
-                                                ant_names_main)
+        holog_obs_dict = _create_holog_obs_dict(
+            pnt_dict, 
+            extract_holog_params['baseline_average_distance'],
+            extract_holog_params['baseline_average_nearest'], 
+            ant_names, 
+            ant_pos,
+            ant_names_main
+        )
         
         #From the generated holog_obs_dict subselect user supplied ddis.
         if ddi != 'all':
             holog_obs_dict_keys = list(holog_obs_dict.keys())
             for ddi_key in holog_obs_dict_keys:
                 if 'ddi' in ddi_key:
                     ddi_id = int(ddi_key.replace('ddi_',''))
                     if ddi_id not in ddi:
                         del holog_obs_dict[ddi_key]
+
     else:
         #If a user defines a holog_obs_dict it needs to be duplicated for each ddi.
         holog_obs_dict_with_ddi = {}
         if ddi == 'all':
             for ddi_id in ms_ddi:
                 holog_obs_dict_with_ddi['ddi_' + str(ddi_id)] = holog_obs_dict
         else:
             for ddi_id in ddi:
                 holog_obs_dict_with_ddi['ddi_' + str(ddi_id)] = holog_obs_dict
         
         holog_obs_dict = holog_obs_dict_with_ddi
             
-    logger.info(f"[{fname}]: holog_obs_dict: \n%s", pformat(list(holog_obs_dict.values())[0], indent=2, width=2))
+    logger.info(f"[{function_name}]: holog_obs_dict: \n%s", pformat(list(holog_obs_dict.values())[0], indent=2, width=2))
 
 
     outfile_obj = copy.deepcopy(holog_obs_dict)
 
     _jsonify(outfile_obj)
 
     with open(".holog_obs_dict.json", "w") as outfile:
@@ -252,15 +263,15 @@
 
     # 2.61 SubscanIntent (p. 152)
     # MIXED : Pointing measurement, some antennas are on-source, some off-source
     # REFERENCE : reference measurement (used for boresight in holography).
     # Undefined : ?
 
     ctb = ctables.table(
-        os.path.join(extract_holog_parms['ms_name'], "STATE"),
+        os.path.join(extract_holog_params['ms_name'], "STATE"),
         readonly=True,
         lockoptions={"option": "usernoread"},
         ack=False,
     )
 
     # scan intent (with subscan intent) is stored in the OBS_MODE column of the STATE subtable.
     obs_modes = ctb.getcol("OBS_MODE")
@@ -270,42 +281,42 @@
     state_ids = []
 
     for i, mode in enumerate(obs_modes):
         if (scan_intent in mode) and ('REFERENCE' not in mode):
             state_ids.append(i)
 
     spw_ctb = ctables.table(
-        os.path.join(extract_holog_parms['ms_name'], "SPECTRAL_WINDOW"),
+        os.path.join(extract_holog_params['ms_name'], "SPECTRAL_WINDOW"),
         readonly=True,
         lockoptions={"option": "usernoread"},
         ack=False,
     )
     pol_ctb = ctables.table(
-        os.path.join(extract_holog_parms['ms_name'], "POLARIZATION"),
+        os.path.join(extract_holog_params['ms_name'], "POLARIZATION"),
         readonly=True,
         lockoptions={"option": "usernoread"},
         ack=False,
     )
 
     obs_ctb = ctables.table(
-        os.path.join(extract_holog_parms['ms_name'], "OBSERVATION"),
+        os.path.join(extract_holog_params['ms_name'], "OBSERVATION"),
         readonly=True,
         lockoptions={"option": "usernoread"},
         ack=False,
     )
     
     telescope_name = obs_ctb.getcol("TELESCOPE_NAME")[0]
     start_time_unix = obs_ctb.getcol('TIME_RANGE')[0][0] - 3506716800.0
     time = Time(start_time_unix, format='unix').jyear
 
     # If we have an EVLA run from before 2023 the pointing table needs to be fixed.
     if telescope_name == "EVLA" and time < 2023:
         # Convert from casa epoch to unix time
         his_ctb = ctables.table(
-            os.path.join(extract_holog_parms['ms_name'], "HISTORY"),
+            os.path.join(extract_holog_params['ms_name'], "HISTORY"),
             readonly=True,
             lockoptions={"option": "usernoread"},
             ack=False,
         )
     
         assert ("pnt_tbl:fixed" in his_ctb.getcol("MESSAGE")), \
             "Pointing table not corrected, users should apply function astrohack.dio.fix_pointing_table() to " \
@@ -316,200 +327,188 @@
     count = 0
     delayed_list = []
     for ddi_name in holog_obs_dict.keys():
         ddi = int(ddi_name.replace('ddi_',''))
         spw_setup_id = ddi_spw[ddi]
         pol_setup_id = ddpol_indexol[ddi]
         
-        extract_holog_parms["ddi"] = ddi
-        extract_holog_parms["chan_setup"] = {}
-        extract_holog_parms["pol_setup"] = {}
-        extract_holog_parms["chan_setup"]["chan_freq"] = spw_ctb.getcol("CHAN_FREQ", startrow=spw_setup_id, nrow=1)[0, :]
-        extract_holog_parms["chan_setup"]["chan_width"] = spw_ctb.getcol("CHAN_WIDTH", startrow=spw_setup_id, nrow=1)[0, :]
-        extract_holog_parms["chan_setup"]["eff_bw"] = spw_ctb.getcol("EFFECTIVE_BW", startrow=spw_setup_id, nrow=1)[0, :]
-        extract_holog_parms["chan_setup"]["ref_freq"] = spw_ctb.getcol("REF_FREQUENCY", startrow=spw_setup_id, nrow=1)[0]
-        extract_holog_parms["chan_setup"]["total_bw"] = spw_ctb.getcol("TOTAL_BANDWIDTH", startrow=spw_setup_id, nrow=1)[0]
-        extract_holog_parms["pol_setup"]["pol"] = pol_str[pol_ctb.getcol("CORR_TYPE", startrow=pol_setup_id, nrow=1)[0, :]]
+        extract_holog_params["ddi"] = ddi
+        extract_holog_params["chan_setup"] = {}
+        extract_holog_params["pol_setup"] = {}
+        extract_holog_params["chan_setup"]["chan_freq"] = spw_ctb.getcol("CHAN_FREQ", startrow=spw_setup_id, nrow=1)[0, :]
+        extract_holog_params["chan_setup"]["chan_width"] = spw_ctb.getcol("CHAN_WIDTH", startrow=spw_setup_id, nrow=1)[0, :]
+        extract_holog_params["chan_setup"]["eff_bw"] = spw_ctb.getcol("EFFECTIVE_BW", startrow=spw_setup_id, nrow=1)[0, :]
+        extract_holog_params["chan_setup"]["ref_freq"] = spw_ctb.getcol("REF_FREQUENCY", startrow=spw_setup_id, nrow=1)[0]
+        extract_holog_params["chan_setup"]["total_bw"] = spw_ctb.getcol("TOTAL_BANDWIDTH", startrow=spw_setup_id, nrow=1)[0]
+        extract_holog_params["pol_setup"]["pol"] = pol_str[pol_ctb.getcol("CORR_TYPE", startrow=pol_setup_id, nrow=1)[0, :]]
         
-        extract_holog_parms["telescope_name"] = obs_ctb.getcol("TELESCOPE_NAME")[0]
+        extract_holog_params["telescope_name"] = obs_ctb.getcol("TELESCOPE_NAME")[0]
 
         for holog_map_key in holog_obs_dict[ddi_name].keys(): #loop over all beam_scan_ids, a beam_scan_id can conist out of more than one scan in an ms (this is the case for the VLA pointed mosiacs).
 
             if 'map' in holog_map_key:
                 scans = holog_obs_dict[ddi_name][holog_map_key]["scans"]
-                logger.info(f"[{fname}]: Processing ddi: {ddi}, scans: {scans}")
+                logger.info(f"[{function_name}]: Processing ddi: {ddi}, scans: {scans}")
                 
                 if len(list(holog_obs_dict[ddi_name][holog_map_key]['ant'].keys())) != 0:
                     map_ant_list = []
                     ref_ant_per_map_ant_list = []
                     
                     map_ant_name_list = []
                     ref_ant_per_map_ant_name_list = []
                     for map_ant_str in holog_obs_dict[ddi_name][holog_map_key]['ant'].keys():
-                        ref_ant_ids = np.array(_convert_ant_name_to_id(ant_names,list(holog_obs_dict[ddi_name][holog_map_key]['ant'][map_ant_str])))
+                        ref_ant_ids = np.array(_convert_ant_name_to_id(ant_names, list(holog_obs_dict[ddi_name][holog_map_key]['ant'][map_ant_str])))
                         
                         map_ant_id = _convert_ant_name_to_id(ant_names,map_ant_str)[0]
 
                         ref_ant_per_map_ant_list.append(ref_ant_ids)
                         map_ant_list.append(map_ant_id)
                         
                         ref_ant_per_map_ant_name_list.append(list(holog_obs_dict[ddi_name][holog_map_key]['ant'][map_ant_str]))
                         map_ant_name_list.append(map_ant_str)
 
-                    extract_holog_parms["ref_ant_per_map_ant_tuple"] = tuple(ref_ant_per_map_ant_list)
-                    extract_holog_parms["map_ant_tuple"] = tuple(map_ant_list)
+                    extract_holog_params["ref_ant_per_map_ant_tuple"] = tuple(ref_ant_per_map_ant_list)
+                    extract_holog_params["map_ant_tuple"] = tuple(map_ant_list)
                     
-                    extract_holog_parms["ref_ant_per_map_ant_name_tuple"] = tuple(ref_ant_per_map_ant_name_list)
-                    extract_holog_parms["map_ant_name_tuple"] = tuple(map_ant_name_list)
+                    extract_holog_params["ref_ant_per_map_ant_name_tuple"] = tuple(ref_ant_per_map_ant_name_list)
+                    extract_holog_params["map_ant_name_tuple"] = tuple(map_ant_name_list)
                     
-                    extract_holog_parms["scans"] = scans
-                    extract_holog_parms["sel_state_ids"] = state_ids
-                    extract_holog_parms["holog_map_key"] = holog_map_key
-                    extract_holog_parms["ant_names"] = ant_names
+                    extract_holog_params["scans"] = scans
+                    extract_holog_params["sel_state_ids"] = state_ids
+                    extract_holog_params["holog_map_key"] = holog_map_key
+                    extract_holog_params["ant_names"] = ant_names
                     
                     if parallel:
                         delayed_list.append(
                             dask.delayed(_extract_holog_chunk)(
-                                dask.delayed(extract_holog_parms)
+                                dask.delayed(extract_holog_params)
                             )
                         )
                     else:
-                        _extract_holog_chunk(extract_holog_parms)
+                        _extract_holog_chunk(extract_holog_params)
                     count += 1
                 else:
-                    logger.warning(f'[{fname}]: DDI ' + str(ddi) + ' has no holography data to extract.')
+                    logger.warning(f'[{function_name}]: DDI ' + str(ddi) + ' has no holography data to extract.')
 
     spw_ctb.close()
     pol_ctb.close()
     obs_ctb.close()
 
     if parallel:
         dask.compute(delayed_list)    
 
     if count > 0:
-        logger.info(f"[{fname}]: Finished processing")
-        holog_dict = _load_holog_file(holog_file=extract_holog_parms["holog_name"], dask_load=True, load_pnt_dict=False)
-        extract_holog_parms['telescope_name'] = telescope_name
-        _create_holog_meta_data(holog_file=extract_holog_parms['holog_name'], holog_dict=holog_dict,
-                                input_params=input_params)
-        holog_mds = AstrohackHologFile(extract_holog_parms['holog_name'])
+        logger.info(f"[{function_name}]: Finished processing")
+        holog_dict = _load_holog_file(holog_file=extract_holog_params["holog_name"], dask_load=True, load_pnt_dict=False)
+        extract_holog_params['telescope_name'] = telescope_name
+        
+        holog_attr_file = "{name}/{ext}".format(name=extract_holog_params['holog_name'], ext=".holog_attr")
+
+        meta_data = _create_holog_meta_data(
+            holog_file=extract_holog_params['holog_name'], 
+            holog_dict=holog_dict,
+            input_params=extract_holog_params.copy()
+        )
+
+        _write_meta_data(holog_attr_file, meta_data)
+
+        holog_mds = AstrohackHologFile(extract_holog_params['holog_name'])
         holog_mds._open()
+        
         return holog_mds
     else:
-        logger.warning(f"[{fname}]: No data to process")
+        logger.warning(f"[{function_name}]: No data to process")
         return None
 
     holog_mds._open()
 
     return holog_mds
 
-def _check_extract_holog_parms(fname,
-                               ms_name,
-                               holog_obs_dict,
-                               ddi_sel,
-                               baseline_average_distance,
-                               baseline_average_nearest,
-                               holog_name,
-                               point_name,
-                               data_column,
-                               parallel,
-                               reuse_point_zarr,
-                               overwrite):
-
-    extract_holog_parms = {"ms_name": ms_name, "holog_name": holog_name, "ddi_sel": ddi_sel, "point_name": point_name,
-                           "data_column": data_column, "parallel": parallel, "overwrite": overwrite,
-                           "reuse_point_zarr": reuse_point_zarr, "baseline_average_distance": baseline_average_distance,
-                           "baseline_average_nearest": baseline_average_nearest}
+def _check_extract_holog_params(function_name, extract_holog_params):
 
     #### Parameter Checking ####
     logger = _get_astrohack_logger()
     parms_passed = True
     
-    parms_passed = parms_passed and _check_parms(fname, extract_holog_parms, 'ms_name', [str], default=None)
+    parms_passed = parms_passed and _check_parms(function_name, extract_holog_params, 'ms_name', [str], default=None)
 
-    base_name = _remove_suffix(ms_name, '.ms')
-    parms_passed = parms_passed and _check_parms(fname, extract_holog_parms,'holog_name', [str],
-                                                 default=base_name+'.holog.zarr')
-
-    point_base_name = _remove_suffix(extract_holog_parms['holog_name'], '.holog.zarr')
-    parms_passed = parms_passed and _check_parms(fname, extract_holog_parms, 'point_name', [str],
-                                                 default=point_base_name+'.point.zarr')
+    base_name = _remove_suffix(extract_holog_params['ms_name'], '.ms')
     
-    parms_passed = parms_passed and _check_parms(fname, extract_holog_parms, 'ddi_sel', [list, int],
-                                                 list_acceptable_data_types=[int], default='all')
+    parms_passed = parms_passed and _check_parms(function_name, extract_holog_params, 'holog_name', [str], default=base_name+'.holog.zarr')
+    parms_passed = parms_passed and _check_parms(function_name, extract_holog_params, 'point_name', [str], default=None)
+
+    point_base_name = _remove_suffix(extract_holog_params['holog_name'], '.holog.zarr')
+    
+    parms_passed = parms_passed and _check_parms(function_name, extract_holog_params, 'ddi', [list, int, str], list_acceptable_data_types=[int], default='all')
   
     #To Do: special function needed to check holog_obs_dict.
-    parm_check = isinstance(holog_obs_dict,dict) or (holog_obs_dict is None)
+    parm_check = isinstance(extract_holog_params['holog_obs_dict'], dict) or (extract_holog_params['holog_obs_dict'] is None)
     parms_passed = parms_passed and parm_check
+
     if not parm_check:
-        logger.error(f'[{fname}]: Parameter holog_obs_dict must be of type {str(dict)}.')
+        logger.error(f'[{function_name}]: Parameter holog_obs_dict must be of type {str(dict)}.')
         
-    parms_passed = parms_passed and _check_parms(fname, extract_holog_parms, 'baseline_average_distance',
-                                                 [numbers.Number], default='all')
+    parms_passed = parms_passed and _check_parms(function_name, extract_holog_params, 'baseline_average_distance', [numbers.Number, str], default='all')
     
-    parms_passed = parms_passed and _check_parms(fname, extract_holog_parms, 'baseline_average_nearest', [int],
-                                                 default='all')
+    parms_passed = parms_passed and _check_parms(function_name, extract_holog_params, 'baseline_average_nearest', [int, str], default='all')
     
-    if (extract_holog_parms['baseline_average_distance'] != 'all') and \
-            (extract_holog_parms['baseline_average_nearest'] != 'all'):
-        logger.error(f'[{fname}]: baseline_average_distance: {str(baseline_average_distance)} and '
-                     f'baseline_average_nearest: {str(baseline_average_distance)} can not both be specified.')
+    if (extract_holog_params['baseline_average_distance'] != 'all') and (extract_holog_params['baseline_average_nearest'] != 'all'):
+        logger.error(f'[{function_name}]: baseline_average_distance: {str(baseline_average_distance)} and 'f'baseline_average_nearest: {str(baseline_average_distance)} can not both be specified.')
+
         parms_passed = False
  
-    parms_passed = parms_passed and _check_parms(fname, extract_holog_parms, 'data_column', [str],
-                                                 default='CORRECTED_DATA')
+    parms_passed = parms_passed and _check_parms(function_name, extract_holog_params, 'data_column', [str], default='CORRECTED_DATA')
 
-    parms_passed = parms_passed and _check_parms(fname, extract_holog_parms, 'parallel', [bool], default=False)
-    
-    parms_passed = parms_passed and _check_parms(fname, extract_holog_parms, 'reuse_point_zarr', [bool], default=False)
+    parms_passed = parms_passed and _check_parms(function_name, extract_holog_params, 'parallel', [bool], default=False)
 
-    parms_passed = parms_passed and _check_parms(fname, extract_holog_parms, 'overwrite', [bool],default=False)
+    parms_passed = parms_passed and _check_parms(function_name, extract_holog_params, 'overwrite', [bool],default=False)
 
-    _parm_check_passed(fname, parms_passed)
+    _parm_check_passed(function_name, parms_passed)
 
-    return extract_holog_parms
+    return extract_holog_params
 
 def generate_holog_obs_dict(
     ms_name,
-    holog_obs_dict=None,
-    ddi=None,
-    baseline_average_distance=None,
-    baseline_average_nearest=None,
-    holog_name=None,
     point_name=None,
+    ddi='all',
+    baseline_average_distance='all',
+    baseline_average_nearest='all',
     data_column="CORRECTED_DATA",
-    parallel=False,
-    reuse_point_zarr=False
+    overwrite=False,
+    parallel=False
 ):
     """
     Extract holography and optionally pointing data, from measurement set. Creates holography output file.
 
     :param ms_name: Name of input measurement file name.
     :type ms_name: str
-    :param holog_obs_dict: The *holog_obs_dict* describes which scan and antenna data to extract from the measurement set. As detailed below, this compound dictionary also includes important meta data needed for preprocessing and extraction of the holography data from the measurement set. If not specified holog_obs_dict will be generated. For auto generation of the holog_obs_dict the assumtion is made that the same antanna beam is not mapped twice in a row (alternating sets of antennas is fine).
-    :type holog_obs_dict: dict, optional
+    
     :param ddi:  DDI(s) that should be extracted from the measurement set. Defaults to all DDI's in the ms.
     :type ddi: int numpy.ndarray | int list, optional
+
     :param baseline_average_distance: To increase the signal to noise for a mapping antenna mutiple reference antennas can be used. The baseline_average_distance is the acceptable distance between a mapping antenna and a reference antenna. The baseline_average_distance is only used if the holog_obs_dict is not specified. If no distance is specified all reference antennas will be used. baseline_average_distance and baseline_average_nearest can not be used together.
     :type holog_obs_dict: float, optional
+
     :param baseline_average_nearest: To increase the signal to noise for a mapping antenna mutiple reference antennas can be used. The baseline_average_nearest is the number of nearest reference antennas to use. The baseline_average_nearest is only used if the holog_obs_dict is not specified.  baseline_average_distance and baseline_average_nearest can not be used together.
     :type holog_obs_dict: int, optional
-    :param holog_name: Name of *<holog_name>.holog.zarr* file to create. Defaults to measurement set name with *holog.zarr* extension.
-    :type holog_name: str, optional
+
     :param point_name: Name of *<point_name>.point.zarr* file to create. Defaults to measurement set name with *point.zarr* extension.
     :type point_name: str, optional
+
     :param data_column: Determines the data column to pull from the measurement set. Defaults to "CORRECTED_DATA".
     :type data_column: str, optional, ex. DATA, CORRECTED_DATA
+
+    :param overwrite: Boolean for whether to overwrite current holog.zarr and point.zarr files, defaults to False.
+    :type overwrite: bool, optional
+
     :param parallel: Boolean for whether to process in parallel. Defaults to False
     :type parallel: bool, optional
-    :param reuse_point_zarr: If true the point.zarr specified in point_name is reused.
-    :type reuse_point_zarr: bool, optional
 
-    :return: Holography holog object.
-    :rtype: AstrohackHologFile
+    :return: holog observation dictionary
+    :rtype: json
 
     .. _Description:
 
     **AstrohackHologFile**
 
     Holog object allows the user to access holog data via compound dictionary keys with values, in order of depth, `ddi` -> `map` -> `ant`. The holog object also provides a `summary()` helper function to list available keys for each file. An outline of the holog object structure is show below:
 
@@ -527,16 +526,14 @@
             },
             ⋮
             ddi_m: …
         }
 
     **Additional Information**
 
-        This function extracts the holography related information from the given measurement file. The data is restructured into an astrohack file format and saved into a file in the form of *<holog_name>.holog.zarr*. The extension *.holog.zarr* is used for all holography files. In addition, the pointing information is recorded into a holography file of format *<pointing_name>.point.zarr*. The extension *.point.zarr* is used for all holography pointing files. 
-
         **holog_obs_dict[holog_mapping_id] (dict):**
         *holog_mapping_id* is a unique, arbitrary, user-defined integer assigned to the data that describes a single complete mapping of the beam.
         
         .. rubric:: This is needed for two reasons:
         * A complete mapping of the beam can be done over more than one scan (for example the VLA data). 
         * A measurement set can contain more than one mapping of the beam (for example the ALMA data).
     
@@ -563,116 +560,104 @@
                             'DV23', 'DV24', 'DV25'
                         ]
                     }
                 }
             }
 
     """
+    extract_holog_params = locals()
+
     logger = _get_astrohack_logger()
     
-    fname = 'extract_holog'
-    ######### Parameter Checking #########
-    extract_holog_parms = _check_extract_holog_parms(fname,
-                                                     ms_name,
-                                                     holog_obs_dict,
-                                                     ddi,
-                                                     baseline_average_distance,
-                                                     baseline_average_nearest,
-                                                     holog_name,
-                                                     point_name,
-                                                     data_column,
-                                                     parallel,
-                                                     reuse_point_zarr, 
-                                                     False)
-    input_params = extract_holog_parms.copy()
-    
-    check_if_file_exists(fname, extract_holog_parms['ms_name'])
-           
-    ############# Exstract pointing infromation and save to point.zarr #############
-    if extract_holog_parms["reuse_point_zarr"]:
-        try:
-            pnt_dict = _load_point_file(extract_holog_parms['point_name'])
-        except:
-            logger.warning(f'[{fname}]: Could not find {extract_holog_parms["point_name"]}, creating point new '
-                           f'point.zarr.')
-            pnt_dict = _extract_pointing(extract_holog_parms['ms_name'], extract_holog_parms['point_name'],
-                                         parallel=extract_holog_parms['parallel'])
-    else:
-        check_if_file_will_be_overwritten(fname, extract_holog_parms['point_name'], True)
-        pnt_dict = _extract_pointing(extract_holog_parms['ms_name'], extract_holog_parms['point_name'],
-                                     parallel=extract_holog_parms['parallel'])
+    function_name = inspect.stack()[CURRENT_FUNCTION].function
+    
+    _check_if_file_exists(extract_holog_params['ms_name'])
+
+    if os.path.exists(point_name) is False or point_name==None:
+        
+        logger.debug('[{caller}]: File {file} does not exists. Extracting ...'.format(caller=function_name, file=point_name))
+            
+        from astrohack._utils._tools import _remove_suffix
+
+        point_name = _remove_suffix(ms_name, '.ms') + '.point.zarr'
+        extract_holog_params['point_name'] = point_name
+            
+        logger.debug('[{caller}]: Extracting pointing to {output}'.format(caller=function_name, output=point_name))
+        
+
+    pnt_dict = extract_pointing(
+        ms_name=extract_holog_params['ms_name'],
+        point_name=extract_holog_params['point_name'],
+        parallel=extract_holog_params['parallel'],
+        overwrite=extract_holog_params['overwrite']
+    )
 
     ######## Get Spectral Windows ########
     ctb = ctables.table(
-        os.path.join(extract_holog_parms['ms_name'], "DATA_DESCRIPTION"),
+        os.path.join(extract_holog_params['ms_name'], "DATA_DESCRIPTION"),
         readonly=True,
         lockoptions={"option": "usernoread"},
         ack=False,
     )
     ddi_spw = ctb.getcol("SPECTRAL_WINDOW_ID")
     ddpol_indexol = ctb.getcol("POLARIZATION_ID")
     ms_ddi = np.arange(len(ddi_spw))
     ctb.close()
 
     ######## Get Antenna IDs and Names ########
     ctb = ctables.table(
-        os.path.join(extract_holog_parms['ms_name'], "ANTENNA"),
+        os.path.join(extract_holog_params['ms_name'], "ANTENNA"),
         readonly=True,
         lockoptions={"option": "usernoread"},
         ack=False,
     )
 
     ant_names = np.array(ctb.getcol("NAME"))
     ant_id = np.arange(len(ant_names))
     ant_pos = ctb.getcol("POSITION")
 
     ctb.close()
     
     ######## Get Antenna IDs that are in the main table########
     ctb = ctables.table(
-        extract_holog_parms['ms_name'],
+        extract_holog_params['ms_name'],
         readonly=True,
         lockoptions={"option": "usernoread"},
         ack=False,
     )
 
     ant1 = np.unique(ctb.getcol("ANTENNA1"))
     ant2 = np.unique(ctb.getcol("ANTENNA2"))
     ant_id_main = np.unique(np.append(ant1,ant2))
     
     ant_names_main = ant_names[ant_id_main]
     ctb.close()
     
     # Create holog_obs_dict or modify user supplied holog_obs_dict.
-    ddi = extract_holog_parms['ddi_sel']
-    if holog_obs_dict is None: #Automatically create holog_obs_dict
-        from astrohack._utils._extract_holog import _create_holog_obs_dict
-        holog_obs_dict = _create_holog_obs_dict(pnt_dict, extract_holog_parms['baseline_average_distance'],
-                                                extract_holog_parms['baseline_average_nearest'], ant_names, ant_pos,
-                                                ant_names_main)
+    ddi = extract_holog_params['ddi']
+
+    
+    from astrohack._utils._extract_holog import _create_holog_obs_dict
+    holog_obs_dict = _create_holog_obs_dict(
+            pnt_dict, 
+            extract_holog_params['baseline_average_distance'],
+            extract_holog_params['baseline_average_nearest'], 
+            ant_names, 
+            ant_pos,
+            ant_names_main
+    )
         
         #From the generated holog_obs_dict subselect user supplied ddis.
-        if ddi != 'all':
-            holog_obs_dict_keys = list(holog_obs_dict.keys())
-            for ddi_key in holog_obs_dict_keys:
-                if 'ddi' in ddi_key:
-                    ddi_id = int(ddi_key.replace('ddi_',''))
-                    if ddi_id not in ddi:
-                        del holog_obs_dict[ddi_key]
-    else:
-        #If a user defines a holog_obs_dict it needs to be duplicated for each ddi.
-        holog_obs_dict_with_ddi = {}
-        if ddi == 'all':
-            for ddi_id in ms_ddi:
-                holog_obs_dict_with_ddi['ddi_' + str(ddi_id)] = holog_obs_dict
-        else:
-            for ddi_id in ddi:
-                holog_obs_dict_with_ddi['ddi_' + str(ddi_id)] = holog_obs_dict
-        
-        holog_obs_dict = holog_obs_dict_with_ddi
+    if ddi != 'all':
+        holog_obs_dict_keys = list(holog_obs_dict.keys())
+        for ddi_key in holog_obs_dict_keys:
+            if 'ddi' in ddi_key:
+                ddi_id = int(ddi_key.replace('ddi_',''))
+                if ddi_id not in ddi:
+                    del holog_obs_dict[ddi_key]
 
 
     outfile_obj = copy.deepcopy(holog_obs_dict)
 
     _jsonify(outfile_obj)
 
     with open(".holog_obs_dict.json", "w") as outfile:
```

### Comparing `astrohack-0.1.8/src/astrohack/gdown_utils.py` & `astrohack-0.2.0/src/astrohack/gdown_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import os
 import re
 import gdown
 import shutil
 import json
 
+from astrohack._utils._tools import _remove_suffix
+
 from prettytable import PrettyTable
 
 gdown_ids = {
     'ea25_cal_small_before_fixed.split.ms':'1oydlR7kA7F4n0i9KF9HgRc2jq1ziUslt',
     'ea25_cal_small_after_fixed.split.ms':'1TATMxKTFYIEO-l9L3jdYj62lZ8TZex4T',
     'J1924-2914.ms.calibrated.split.SPW3': '1OSDjWM1IskPOlC0w1wVBqsTp8JAbNGzL',
     'extract_holog_verification.json':'1Wd79KCl-wxlUwBRxYFUnofG8mN0Xfzga',
@@ -65,22 +67,24 @@
 
     for file in files:
         assert file in gdown_ids, "File {file} not available. Available files are:".format(file=file) + str(gdown_ids.keys())
 
         id = gdown_ids[file]
         create_folder(folder)
 
-        if unpack: 
-            file = file+'.zip'
-        
         fullname = os.path.join(folder, file)
 
-        if not os.path.exists(fullname):
-            url = 'https://drive.google.com/u/0/uc?id=' + id + '&export=download'
-            gdown.download(url, fullname)
+        if os.path.exists(fullname) or os.path.exists(fullname + '.zip'):
+            continue   
+
+        if unpack:
+            fullname = fullname + '.zip'
+
+        url = 'https://drive.google.com/u/0/uc?id=' + id + '&export=download'
+        gdown.download(url, fullname)
 
         # Unpack results
         if unpack: 
             shutil.unpack_archive(filename=fullname, extract_dir=folder)
 
             # Let's clean up after ourselves
             os.remove(fullname)
```

### Comparing `astrohack-0.1.8/src/astrohack/holog.py` & `astrohack-0.2.0/src/astrohack/holog.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,41 @@
 import json
-import numpy as np
+import inspect
 import numbers
 
-from astrohack._utils._holog import _holog_chunk, _create_image_meta_data
+import numpy as np
+
+from astrohack._utils._holog import _holog_chunk
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
-from astrohack._utils._parm_utils._check_parms import _check_parms, _parm_check_passed
+from astrohack._utils._param_utils._check_parms import _check_parms, _parm_check_passed
 from astrohack._utils._tools import _remove_suffix
-from astrohack._utils._dio import check_if_file_will_be_overwritten, check_if_file_exists, _read_meta_data
+from astrohack._utils._dio import _check_if_file_will_be_overwritten, _check_if_file_exists, _read_meta_data, _write_meta_data
 from astrohack.mds import AstrohackImageFile
 from astrohack._utils._dask_graph_tools import _dask_general_compute
 
+CURRENT_FUNCTION=0
 
-def holog(holog_name, grid_size=None, cell_size=None, image_name=None, padding_factor=50,
-          grid_interpolation_mode="linear", chan_average=True, chan_tolerance_factor=0.005, scan_average=True,
-          ant_id=None, ddi=None, to_stokes=True, apply_mask=True, phase_fit=True, overwrite=False, parallel=False):
+def holog(
+    holog_name, 
+    grid_size=None, 
+    cell_size=None, 
+    image_name=None, 
+    padding_factor=50,
+    grid_interpolation_mode="linear", 
+    chan_average=True, 
+    chan_tolerance_factor=0.005, 
+    scan_average=True,
+    ant_id=None, 
+    ddi=None, 
+    to_stokes=True, 
+    apply_mask=True, 
+    phase_fit=True, 
+    overwrite=False, 
+    parallel=False
+):
     """ Process holography data and derive aperture illumination pattern.
 
     :param holog_name: Name of holography .holog.zarr file to process.
     :type holog_name: str
     :param grid_size: Numpy array specifying the dimensions of the grid used in data gridding. If not specified grid_size is calculated using POINTING_OFFSET in pointing table.
     :type grid_size: numpy.ndarray, dtype int, optional
     :param cell_size: Numpy array defining the cell size of each grid bin. If not specified cell_size is calculated using POINTING_OFFSET in pointing table.
@@ -77,112 +95,114 @@
             },
             ⋮
             ant_n: …
         }
 
     """
     
+    holog_params = locals()
+
     logger = _get_astrohack_logger()
-    fname = 'holog'
-    holog_params = _check_holog_parms(fname, holog_name, grid_size, cell_size, image_name, padding_factor, parallel,
-                                      grid_interpolation_mode, chan_average, chan_tolerance_factor, scan_average,
-                                      ant_id, ddi, to_stokes, apply_mask, phase_fit, overwrite)
-    input_params = holog_params.copy()
+
+    function_name = inspect.stack()[CURRENT_FUNCTION].function
+
+    ######### Parameter Checking #########
+    holog_params = _check_holog_params(function_name=function_name, holog_params=holog_params)
     
-    check_if_file_exists(fname, holog_params['holog_file'])
-    check_if_file_will_be_overwritten(fname, holog_params['image_file'], holog_params['overwrite'])
+    _check_if_file_exists(holog_params['holog_name'])
+    _check_if_file_will_be_overwritten(holog_params['image_name'], holog_params['overwrite'])
+
+    json_data = "/".join((holog_params['holog_name'], ".holog_json"))
 
-    json_data = "/".join((holog_params['holog_file'], ".holog_json"))
     with open(json_data, "r") as json_file:
         holog_json = json.load(json_file)
-    meta_data = _read_meta_data(holog_params['holog_file'], 'holog', 'extract_holog')
+        
+    meta_data = _read_meta_data(holog_params['holog_name'], 'holog', 'extract_holog')
 
     if holog_params["cell_size"] is None:
         cell_size = np.array([-meta_data["cell_size"], meta_data["cell_size"]])
         holog_params["cell_size"] = cell_size
     
     if holog_params["grid_size"] is None:
         n_pix = int(np.sqrt(meta_data["n_pix"]))
         grid_size = np.array([n_pix, n_pix])
         holog_params["grid_size"] = grid_size
 
-    logger.info(f'[{fname}]: Cell size: {str(cell_size)}, Grid size {str(grid_size)}')
+    logger.info(f'[{function_name}]: Cell size: {str(cell_size)}, Grid size {str(grid_size)}')
+    
     json_data = {
             "cell_size": holog_params["cell_size"].tolist(),
             "grid_size": holog_params["grid_size"].tolist()
     }
     
     with open(".holog_diagnostic.json", "w") as out_file:
         json.dump(json_data, out_file)
 
-    if _dask_general_compute(fname, holog_json, _holog_chunk, holog_params, ['ant', 'ddi'], parallel=parallel):
-        _create_image_meta_data(holog_params['image_file'], input_params)
-        image_mds = AstrohackImageFile(holog_params['image_file'])
+    if _dask_general_compute(function_name, holog_json, _holog_chunk, holog_params, ['ant', 'ddi'], parallel=parallel):
+        
+        output_attr_file = "{name}/{ext}".format(name=holog_params['image_name'], ext=".image_attr")
+        _write_meta_data(output_attr_file, holog_params.copy())
+        
+        image_mds = AstrohackImageFile(holog_params['image_name'])
         image_mds._open()
-        logger.info(f'[{fname}]: Finished processing')
+        
+        logger.info(f'[{function_name}]: Finished processing')
+
         return image_mds
     else:
-        logger.warning(f"[{fname}]: No data to process")
+        logger.warning(f"[{function_name}]: No data to process")
         return None
 
 
-def _check_holog_parms(fname, holog_name, grid_size, cell_size, image_name, padding_factor, parallel,
-                       grid_interpolation_mode, chan_average, chan_tolerance_factor, scan_average, ant_id, ddi,
-                       to_stokes, apply_mask, phase_fit, overwrite):
-
-    holog_params = {"holog_file": holog_name, "grid_size": grid_size, "cell_size": cell_size, "image_file": image_name,
-                    "padding_factor": padding_factor, "parallel": parallel,
-                    "grid_interpolation_mode": grid_interpolation_mode, "chan_average": chan_average, "ddi": ddi,
-                    "chan_tolerance_factor": chan_tolerance_factor, "scan_average": scan_average, "ant": ant_id,
-                    "to_stokes": to_stokes, "apply_mask": apply_mask, "phase_fit": phase_fit, "overwrite": overwrite}
+def _check_holog_params(function_name, holog_params):
 
     #### Parameter Checking ####
     parms_passed = True
     
-    parms_passed = parms_passed and _check_parms(fname, holog_params, 'holog_file', [str], default=None)
+    parms_passed = parms_passed and _check_parms(function_name, holog_params, 'holog_name', [str], default=None)
 
-    parms_passed = parms_passed and _check_parms(fname, holog_params, 'grid_size', [list, np.ndarray],
+    parms_passed = parms_passed and _check_parms(function_name, holog_params, 'grid_size', [list, np.ndarray],
                                                  list_acceptable_data_types=[np.int64, int], list_len=2, default='None',
                                                  log_default_setting=False)
     if (isinstance(holog_params['grid_size'], str)) and (holog_params['grid_size'] == 'None'):
         holog_params['grid_size'] = None
     else:
         holog_params['grid_size'] = np.array(holog_params['grid_size'])
 
-    parms_passed = parms_passed and _check_parms(fname, holog_params, 'cell_size', [list, np.ndarray],
+    parms_passed = parms_passed and _check_parms(function_name, holog_params, 'cell_size', [list, np.ndarray],
                                                  list_acceptable_data_types=[numbers.Number], list_len=2,
                                                  default='None', log_default_setting=False)
     if (isinstance(holog_params['cell_size'], str)) and (holog_params['cell_size'] == 'None'):
         holog_params['cell_size'] = None
     else:
         holog_params['cell_size'] = np.array(holog_params['cell_size'])
 
-    base_name = _remove_suffix(holog_params['holog_file'], '.holog.zarr')
-    parms_passed = parms_passed and _check_parms(fname, holog_params, 'image_file', [str],
+    base_name = _remove_suffix(holog_params['holog_name'], '.holog.zarr')
+    parms_passed = parms_passed and _check_parms(function_name, holog_params, 'image_name', [str],
                                                  default=base_name+'.image.zarr')
-    parms_passed = parms_passed and _check_parms(fname, holog_params, 'padding_factor', [int], default=50)
-    parms_passed = parms_passed and _check_parms(fname, holog_params, 'parallel', [bool], default=False)
-    parms_passed = parms_passed and _check_parms(fname, holog_params, 'grid_interpolation_mode', [str],
+    parms_passed = parms_passed and _check_parms(function_name, holog_params, 'padding_factor', [int], default=50)
+    parms_passed = parms_passed and _check_parms(function_name, holog_params, 'parallel', [bool], default=False)
+    parms_passed = parms_passed and _check_parms(function_name, holog_params, 'grid_interpolation_mode', [str],
                                                  acceptable_data=["nearest", "linear", "cubic"], default="nearest")
-    parms_passed = parms_passed and _check_parms(fname, holog_params, 'chan_average', [bool], default=True)
-    parms_passed = parms_passed and _check_parms(fname, holog_params, 'chan_tolerance_factor', [float],
+    parms_passed = parms_passed and _check_parms(function_name, holog_params, 'chan_average', [bool], default=True)
+    parms_passed = parms_passed and _check_parms(function_name, holog_params, 'chan_tolerance_factor', [float],
                                                  acceptable_range=[0, 1], default=0.005)
-    parms_passed = parms_passed and _check_parms(fname, holog_params, 'scan_average', [bool], default=True)
-    parms_passed = parms_passed and _check_parms(fname, holog_params, 'ant', [list, str],
+    parms_passed = parms_passed and _check_parms(function_name, holog_params, 'scan_average', [bool], default=True)
+    parms_passed = parms_passed and _check_parms(function_name, holog_params, 'ant', [list, str],
                                                  list_acceptable_data_types=[str], default='all')
-    parms_passed = parms_passed and _check_parms(fname, holog_params, 'ddi', [list, int],
+    parms_passed = parms_passed and _check_parms(function_name, holog_params, 'ddi', [list, int],
                                                  list_acceptable_data_types=[int], default='all')
-    parms_passed = parms_passed and _check_parms(fname, holog_params, 'to_stokes', [bool], default=True)
+    parms_passed = parms_passed and _check_parms(function_name, holog_params, 'to_stokes', [bool], default=True)
 
     if isinstance(holog_params['phase_fit'], list) or isinstance(holog_params['phase_fit'], type(np.ndarray)):
-        parms_passed = parms_passed and _check_parms(fname, holog_params, 'phase_fit', [list, type(np.ndarray)],
+        parms_passed = parms_passed and _check_parms(function_name, holog_params, 'phase_fit', [list, type(np.ndarray)],
                                                      list_acceptable_data_types=[bool], list_len=5)
     else:
-        parms_passed = parms_passed and _check_parms(fname, holog_params, 'phase_fit', [bool], default=True)
+        parms_passed = parms_passed and _check_parms(function_name, holog_params, 'phase_fit', [bool], default=True)
 
-    parms_passed = parms_passed and _check_parms(fname, holog_params, 'apply_mask', [bool], default=True)
-    parms_passed = parms_passed and _check_parms(fname, holog_params, 'overwrite', [bool], default=False)
+    parms_passed = parms_passed and _check_parms(function_name, holog_params, 'apply_mask', [bool], default=True)
+    parms_passed = parms_passed and _check_parms(function_name, holog_params, 'overwrite', [bool], default=False)
 
-    _parm_check_passed(fname, parms_passed)
+    _parm_check_passed(function_name, parms_passed)
 
     return holog_params
```

### Comparing `astrohack-0.1.8/src/astrohack/mds.py` & `astrohack-0.2.0/src/astrohack/mds.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
 from astrohack._utils._dio import _read_meta_data
 from astrohack._utils._dio import _load_holog_file
 from astrohack._utils._dio import _load_image_file
 from astrohack._utils._dio import _load_panel_file
 from astrohack._utils._dio import _load_point_file
 from astrohack._utils._dio import _create_destination_folder
-from astrohack._utils._parm_utils._check_parms import _check_parms, _parm_check_passed
+from astrohack._utils._param_utils._check_parms import _check_parms, _parm_check_passed
 from astrohack._utils._constants import length_units, trigo_units, plot_types, possible_splits
 from astrohack._utils._dask_graph_tools import _dask_general_compute
 from astrohack._utils._tools import _print_method_list, _print_attributes, _print_data_contents, _print_summary_header
 
 from astrohack._utils._panel import _plot_antenna_chunk, _export_to_fits_panel_chunk, _export_screws_chunk
 from astrohack._utils._holog import _export_to_fits_holog_chunk, _plot_aperture_chunk, _plot_beam_chunk
 from astrohack._utils._diagnostics import _calibration_plot_chunk
@@ -860,15 +860,15 @@
             _load_point_file(file=file, dask_load=dask_load, pnt_dict=self)
             self._file_is_open = True
 
         except Exception as e:
             logger.error("[AstrohackPointFile]: {}".format(e))
             self._file_is_open = False
 
-        self._meta_data = _read_meta_data(file, 'point', 'extract_holog')
+        self._meta_data = _read_meta_data(file, 'point', 'extract_pointing')
 
         return self._file_is_open
 
     def summary(self):
         """ Prints summary of the AstrohackPointFile object, with available data, attributes and available methods
         """
         _print_summary_header(self.file)
```

### Comparing `astrohack-0.1.8/src/astrohack/panel.py` & `astrohack-0.2.0/src/astrohack/panel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import shutil
 
 from astrohack._utils._panel_classes.base_panel import panel_models
-from astrohack._utils._dio import _aips_holog_to_xds, check_if_file_will_be_overwritten, check_if_file_exists, _write_meta_data
+from astrohack._utils._dio import _aips_holog_to_xds, _check_if_file_will_be_overwritten, _check_if_file_exists, _write_meta_data
 from astrohack._utils._panel import _panel_chunk
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
-from astrohack._utils._parm_utils._check_parms import _check_parms, _parm_check_passed
+from astrohack._utils._param_utils._check_parms import _check_parms, _parm_check_passed
 from astrohack._utils._tools import _remove_suffix
 from astrohack._utils._dask_graph_tools import _dask_general_compute
 
 from astrohack.mds import AstrohackPanelFile, AstrohackImageFile
 
 
 def panel(image_name, panel_name=None, cutoff=0.2, panel_model=None, panel_margins=0.2, ant_id=None, ddi=None,
@@ -92,29 +92,29 @@
     logger = _get_astrohack_logger()
     fname = 'panel'
     panel_params = _check_panel_parms(fname, image_name, panel_name, cutoff, panel_model, panel_margins, ant_id, ddi,
                                       parallel, overwrite)
     input_params = panel_params.copy()
     # Doubled this entry for compatibility with the factorized antenna ddi loop
     panel_params['filename'] = panel_params['image_name']
-    check_if_file_exists(fname, panel_params['image_name'])
+    _check_if_file_exists(panel_params['image_name'])
     image_mds = AstrohackImageFile(panel_params['image_name'])
     image_mds._open()
-    check_if_file_will_be_overwritten(fname, panel_params['panel_name'], panel_params['overwrite'])
+    _check_if_file_will_be_overwritten(panel_params['panel_name'], panel_params['overwrite'])
 
     if os.path.exists(panel_params['image_name']+'/.aips'):
         panel_params['origin'] = 'AIPS'
         _panel_chunk(panel_params)
 
     else:
         panel_params['origin'] = 'astrohack'
         if _dask_general_compute(fname, image_mds, _panel_chunk, panel_params, ['ant', 'ddi'], parallel=parallel):
             logger.info(f"[{fname}]: Finished processing")
             output_attr_file = "{name}/{ext}".format(name=panel_params['panel_name'], ext=".panel_attr")
-            _write_meta_data('panel', output_attr_file, input_params)
+            _write_meta_data(output_attr_file, input_params)
             panel_mds = AstrohackPanelFile(panel_params['panel_name'])
             panel_mds._open()
             return panel_mds
         else:
             logger.warning(f"[{fname}]: No data to process")
             return None
 
@@ -131,17 +131,17 @@
     Args:
         amp_image: Full path to amplitude image
         dev_image: Full path to deviation image
         telescope_name: Telescope name to be added to the .zarr file
         holog_name: Name of the output .zarr file
         overwrite: Overwrite previous file of same name?
     """
-    check_if_file_exists(amp_image)
-    check_if_file_exists(dev_image)
-    check_if_file_will_be_overwritten(holog_name, overwrite)
+    _check_if_file_exists(amp_image)
+    _check_if_file_exists(dev_image)
+    _check_if_file_will_be_overwritten(holog_name, overwrite)
 
     xds = _aips_holog_to_xds(amp_image, dev_image)
     xds.attrs['telescope_name'] = telescope_name
     if os.path.exists(holog_name):
         shutil.rmtree(holog_name, ignore_errors=False, onerror=None)
     xds.to_zarr(holog_name, mode='w', compute=True, consolidated=True)
     aips_mark = open(holog_name+'/.aips', 'w')
```

### Comparing `astrohack-0.1.8/src/astrohack/profiling.py` & `astrohack-0.2.0/src/astrohack/profiling.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.8/src/astrohack/visualization/viewer.py` & `astrohack-0.2.0/src/astrohack/visualization/viewer.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.8/src/astrohack.egg-info/PKG-INFO` & `astrohack-0.2.0/src/astrohack.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astrohack
-Version: 0.1.8
+Version: 0.2.0
 Summary: Holography Antenna Commissioning Kit
 Author-email: Jan-Willem Steeb <jsteeb@nrao.edu>, Joshua Hoskins <jhoskins@nrao.edu>, Victor de Souza Magalhaes <vdesouza@nrao.edu>
 Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 License-File: LICENSE
```

### Comparing `astrohack-0.1.8/src/astrohack.egg-info/SOURCES.txt` & `astrohack-0.2.0/src/astrohack.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 README.rst
 pyproject.toml
 src/astrohack/__init__.py
 src/astrohack/astrohack_client.py
 src/astrohack/combine.py
 src/astrohack/dio.py
 src/astrohack/extract_holog.py
+src/astrohack/extract_pointing.py
 src/astrohack/gdown_utils.py
 src/astrohack/holog.py
 src/astrohack/locit.py
 src/astrohack/mds.py
 src/astrohack/panel.py
 src/astrohack/profiling.py
 src/astrohack.egg-info/PKG-INFO
@@ -41,17 +42,17 @@
 src/astrohack/_utils/_logger/__init__.py
 src/astrohack/_utils/_logger/_astrohack_logger.py
 src/astrohack/_utils/_panel_classes/antenna_surface.py
 src/astrohack/_utils/_panel_classes/base_panel.py
 src/astrohack/_utils/_panel_classes/polygon_panel.py
 src/astrohack/_utils/_panel_classes/ring_panel.py
 src/astrohack/_utils/_panel_classes/telescope.py
-src/astrohack/_utils/_parm_utils/__init__.py
-src/astrohack/_utils/_parm_utils/_check_logger_parms.py
-src/astrohack/_utils/_parm_utils/_check_parms.py
+src/astrohack/_utils/_param_utils/__init__.py
+src/astrohack/_utils/_param_utils/_check_logger_parms.py
+src/astrohack/_utils/_param_utils/_check_parms.py
 src/astrohack/data/.file_meta_data/J1924-2914.ms.calibrated.split.SPW3.json
 src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after_fixed.split.json
 src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before_fixed_split.json
 src/astrohack/data/telescopes/__init__.py
 src/astrohack/data/telescopes/aca_7m.zarr/.zattrs
 src/astrohack/data/telescopes/aca_7m.zarr/.zgroup
 src/astrohack/data/telescopes/aca_7m.zarr/.zmetadata
```

