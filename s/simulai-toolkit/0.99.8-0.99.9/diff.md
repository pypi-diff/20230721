# Comparing `tmp/simulai-toolkit-0.99.8.tar.gz` & `tmp/simulai-toolkit-0.99.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simulai-toolkit-0.99.8.tar", last modified: Fri Jan 20 16:40:29 2023, max compression
+gzip compressed data, was "simulai-toolkit-0.99.9.tar", last modified: Mon Jan 23 17:58:12 2023, max compression
```

## Comparing `simulai-toolkit-0.99.8.tar` & `simulai-toolkit-0.99.9.tar`

### file list

```diff
@@ -1,97 +1,173 @@
-drwxr-xr-x   0 jalmeida  (1000) jalmeida  (1000)        0 2023-01-20 16:40:29.020473 simulai-toolkit-0.99.8/
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)      575 2023-01-18 19:24:16.000000 simulai-toolkit-0.99.8/AUTHORS.rst
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     4354 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.8/CONTRIBUTING.rst
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)      132 2022-12-05 14:53:20.000000 simulai-toolkit-0.99.8/DESCRIPTION.md
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)       89 2022-12-05 14:53:20.000000 simulai-toolkit-0.99.8/HISTORY.rst
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)      628 2022-12-05 14:53:20.000000 simulai-toolkit-0.99.8/LICENSE
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)      262 2022-12-05 14:53:20.000000 simulai-toolkit-0.99.8/MANIFEST.in
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     1324 2023-01-20 16:40:29.019473 simulai-toolkit-0.99.8/PKG-INFO
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     5042 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.8/README.rst
-drwxr-xr-x   0 jalmeida  (1000) jalmeida  (1000)        0 2023-01-20 16:40:28.951472 simulai-toolkit-0.99.8/docs/
-drwxr-xr-x   0 jalmeida  (1000) jalmeida  (1000)        0 2023-01-20 16:40:28.952472 simulai-toolkit-0.99.8/docs/_modules/
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     1937 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.8/docs/_modules/modules.rst
-drwxr-xr-x   0 jalmeida  (1000) jalmeida  (1000)        0 2023-01-20 16:40:28.955472 simulai-toolkit-0.99.8/docs/_package/
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)       99 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.8/docs/_package/main.rst
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     1463 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.8/docs/_package/simulai.math.rst
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     1022 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.8/docs/_package/simulai.utilities.rst
-drwxr-xr-x   0 jalmeida  (1000) jalmeida  (1000)        0 2023-01-20 16:40:28.956472 simulai-toolkit-0.99.8/docs/_templates/
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)      650 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.8/docs/_templates/ISSUE_TEMPLATE.rst
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     2315 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.8/docs/conf.py
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)      281 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.8/docs/index.rst
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     5090 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.8/docs/quickstart.rst
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     1959 2023-01-20 16:40:19.000000 simulai-toolkit-0.99.8/pyproject.toml
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)       38 2023-01-20 16:40:29.020473 simulai-toolkit-0.99.8/setup.cfg
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)      226 2022-12-05 14:53:20.000000 simulai-toolkit-0.99.8/setup.py
-drwxr-xr-x   0 jalmeida  (1000) jalmeida  (1000)        0 2023-01-20 16:40:28.966472 simulai-toolkit-0.99.8/simulai/
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     1032 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.8/simulai/__init__.py
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     3174 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.8/simulai/abstract.py
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     1354 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.8/simulai/activations.py
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)    11653 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.8/simulai/batching.py
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     6466 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.8/simulai/file.py
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)    33914 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.8/simulai/io.py
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     6011 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.8/simulai/mesh.py
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)    28041 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.8/simulai/metrics.py
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)    13622 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.8/simulai/normalization.py
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     2897 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.8/simulai/output.py
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     5864 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.8/simulai/parallel.py
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)    27673 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.8/simulai/simulation.py
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     3144 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.8/simulai/special.py
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     1328 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.8/simulai/tokens.py
-drwxr-xr-x   0 jalmeida  (1000) jalmeida  (1000)        0 2023-01-20 16:40:28.973472 simulai-toolkit-0.99.8/simulai_toolkit.egg-info/
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     1324 2023-01-20 16:40:28.000000 simulai-toolkit-0.99.8/simulai_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     2174 2023-01-20 16:40:28.000000 simulai-toolkit-0.99.8/simulai_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)        1 2023-01-20 16:40:28.000000 simulai-toolkit-0.99.8/simulai_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)      218 2023-01-20 16:40:28.000000 simulai-toolkit-0.99.8/simulai_toolkit.egg-info/requires.txt
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)        8 2023-01-20 16:40:28.000000 simulai-toolkit-0.99.8/simulai_toolkit.egg-info/top_level.txt
-drwxr-xr-x   0 jalmeida  (1000) jalmeida  (1000)        0 2023-01-20 16:40:28.975473 simulai-toolkit-0.99.8/tests/
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)      152 2022-12-05 14:53:20.000000 simulai-toolkit-0.99.8/tests/README.md
-drwxr-xr-x   0 jalmeida  (1000) jalmeida  (1000)        0 2023-01-20 16:40:28.977472 simulai-toolkit-0.99.8/tests/devices/
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     5165 2023-01-18 13:08:53.000000 simulai-toolkit-0.99.8/tests/devices/test_network_devices.py
-drwxr-xr-x   0 jalmeida  (1000) jalmeida  (1000)        0 2023-01-20 16:40:28.984473 simulai-toolkit-0.99.8/tests/math/
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     3277 2023-01-09 15:45:17.000000 simulai-toolkit-0.99.8/tests/math/test_LSODA.py
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     2606 2022-12-05 14:53:20.000000 simulai-toolkit-0.99.8/tests/math/test_RK4.py
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     3945 2023-01-05 19:58:08.000000 simulai-toolkit-0.99.8/tests/math/test_collocation_derivative.py
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)    10326 2023-01-18 13:53:40.000000 simulai-toolkit-0.99.8/tests/math/test_metrics.py
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     1096 2023-01-12 13:30:25.000000 simulai-toolkit-0.99.8/tests/math/test_products.py
-drwxr-xr-x   0 jalmeida  (1000) jalmeida  (1000)        0 2023-01-20 16:40:28.985473 simulai-toolkit-0.99.8/tests/metrics/
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)      556 2022-12-05 14:53:20.000000 simulai-toolkit-0.99.8/tests/metrics/test_mahalanobis.py
-drwxr-xr-x   0 jalmeida  (1000) jalmeida  (1000)        0 2023-01-20 16:40:28.994473 simulai-toolkit-0.99.8/tests/network/
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     5168 2023-01-04 14:20:32.000000 simulai-toolkit-0.99.8/tests/network/test_conv_1d.py
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     5183 2023-01-04 14:20:32.000000 simulai-toolkit-0.99.8/tests/network/test_conv_2d.py
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)    10158 2023-01-20 13:11:28.000000 simulai-toolkit-0.99.8/tests/network/test_deeponet.py
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     7617 2023-01-11 18:27:18.000000 simulai-toolkit-0.99.8/tests/network/test_dense.py
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     2972 2023-01-18 13:08:53.000000 simulai-toolkit-0.99.8/tests/network/test_elm.py
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     5908 2023-01-20 13:25:36.000000 simulai-toolkit-0.99.8/tests/network/test_flexible_deeponet.py
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     5943 2023-01-20 13:25:37.000000 simulai-toolkit-0.99.8/tests/network/test_improved_deeponet.py
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)      402 2023-01-04 14:23:31.000000 simulai-toolkit-0.99.8/tests/network/utils.py
-drwxr-xr-x   0 jalmeida  (1000) jalmeida  (1000)        0 2023-01-20 16:40:28.996473 simulai-toolkit-0.99.8/tests/opinf/
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     3649 2023-01-19 12:58:40.000000 simulai-toolkit-0.99.8/tests/opinf/test_extended_opinf_operators_construction.py
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)    14908 2023-01-20 14:35:19.000000 simulai-toolkit-0.99.8/tests/opinf/test_opinf_operators_construction.py
-drwxr-xr-x   0 jalmeida  (1000) jalmeida  (1000)        0 2023-01-20 16:40:28.997473 simulai-toolkit-0.99.8/tests/parallelism/
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     3510 2023-01-18 13:53:40.000000 simulai-toolkit-0.99.8/tests/parallelism/test_modelpool_affinemapping.py
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)    35168 2023-01-18 13:53:40.000000 simulai-toolkit-0.99.8/tests/parallelism/test_modelpool_esn.py
-drwxr-xr-x   0 jalmeida  (1000) jalmeida  (1000)        0 2023-01-20 16:40:28.998473 simulai-toolkit-0.99.8/tests/postprocessing/
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     3091 2022-12-05 14:53:20.000000 simulai-toolkit-0.99.8/tests/postprocessing/test_batchwise_extrapolation.py
-drwxr-xr-x   0 jalmeida  (1000) jalmeida  (1000)        0 2023-01-20 16:40:29.006473 simulai-toolkit-0.99.8/tests/preprocessing/
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     3588 2023-01-18 13:53:40.000000 simulai-toolkit-0.99.8/tests/preprocessing/test_batch_copy.py
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     1305 2022-12-05 14:53:20.000000 simulai-toolkit-0.99.8/tests/preprocessing/test_batching.py
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     5232 2023-01-18 13:53:40.000000 simulai-toolkit-0.99.8/tests/preprocessing/test_mapvalid.py
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     3789 2023-01-18 13:53:40.000000 simulai-toolkit-0.99.8/tests/preprocessing/test_meanevaluation.py
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)      999 2022-12-05 14:53:20.000000 simulai-toolkit-0.99.8/tests/preprocessing/test_minmax.py
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     3835 2022-12-05 14:53:20.000000 simulai-toolkit-0.99.8/tests/preprocessing/test_moving_window.py
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)    10930 2023-01-18 13:53:40.000000 simulai-toolkit-0.99.8/tests/preprocessing/test_reshaper.py
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     4348 2023-01-18 13:53:40.000000 simulai-toolkit-0.99.8/tests/preprocessing/test_sampler.py
-drwxr-xr-x   0 jalmeida  (1000) jalmeida  (1000)        0 2023-01-20 16:40:29.007473 simulai-toolkit-0.99.8/tests/rbf/
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     1793 2022-12-05 14:53:20.000000 simulai-toolkit-0.99.8/tests/rbf/test_rbf.py
-drwxr-xr-x   0 jalmeida  (1000) jalmeida  (1000)        0 2023-01-20 16:40:29.007473 simulai-toolkit-0.99.8/tests/residuals/
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     5728 2023-01-18 13:08:53.000000 simulai-toolkit-0.99.8/tests/residuals/test_symbolicoperator.py
-drwxr-xr-x   0 jalmeida  (1000) jalmeida  (1000)        0 2023-01-20 16:40:29.018473 simulai-toolkit-0.99.8/tests/rom/
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     5766 2023-01-19 12:23:11.000000 simulai-toolkit-0.99.8/tests/rom/test_cnn_autoencoder.py
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     1970 2022-12-05 14:53:20.000000 simulai-toolkit-0.99.8/tests/rom/test_dmd_decomposition.py
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     3469 2022-12-05 14:53:20.000000 simulai-toolkit-0.99.8/tests/rom/test_gappy_pca_decomposition.py
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     5025 2023-01-12 13:17:44.000000 simulai-toolkit-0.99.8/tests/rom/test_hosvd.py
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     6108 2023-01-18 13:53:40.000000 simulai-toolkit-0.99.8/tests/rom/test_ipca_datapreparer.py
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     9812 2023-01-18 13:53:40.000000 simulai-toolkit-0.99.8/tests/rom/test_ipca_decomposition.py
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     2619 2023-01-19 15:57:55.000000 simulai-toolkit-0.99.8/tests/rom/test_mlp_autoencoder.py
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     5486 2023-01-12 12:48:41.000000 simulai-toolkit-0.99.8/tests/rom/test_pca_decomposition.py
--rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     2563 2023-01-12 16:55:23.000000 simulai-toolkit-0.99.8/tests/rom/test_qqm.py
+drwxr-xr-x   0 jalmeida  (1000) jalmeida  (1000)        0 2023-01-23 17:58:12.884577 simulai-toolkit-0.99.9/
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)      575 2023-01-18 19:24:16.000000 simulai-toolkit-0.99.9/AUTHORS.rst
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     4355 2023-01-20 17:39:11.000000 simulai-toolkit-0.99.9/CONTRIBUTING.rst
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)      132 2022-12-05 14:53:20.000000 simulai-toolkit-0.99.9/DESCRIPTION.md
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)       89 2022-12-05 14:53:20.000000 simulai-toolkit-0.99.9/HISTORY.rst
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)      628 2022-12-05 14:53:20.000000 simulai-toolkit-0.99.9/LICENSE
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)      262 2022-12-05 14:53:20.000000 simulai-toolkit-0.99.9/MANIFEST.in
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     1324 2023-01-23 17:58:12.883577 simulai-toolkit-0.99.9/PKG-INFO
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     5042 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.9/README.rst
+drwxr-xr-x   0 jalmeida  (1000) jalmeida  (1000)        0 2023-01-23 17:58:12.841577 simulai-toolkit-0.99.9/docs/
+drwxr-xr-x   0 jalmeida  (1000) jalmeida  (1000)        0 2023-01-23 17:58:12.845577 simulai-toolkit-0.99.9/docs/_modules/
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)      119 2023-01-23 13:38:04.000000 simulai-toolkit-0.99.9/docs/_modules/simulai.abstract.rst
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)      128 2023-01-23 13:38:04.000000 simulai-toolkit-0.99.9/docs/_modules/simulai.activations.rst
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)      120 2023-01-23 13:38:04.000000 simulai-toolkit-0.99.9/docs/_modules/simulai.batching.rst
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)      107 2023-01-23 13:38:04.000000 simulai-toolkit-0.99.9/docs/_modules/simulai.file.rst
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)      103 2023-01-23 13:38:04.000000 simulai-toolkit-0.99.9/docs/_modules/simulai.io.rst
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)      107 2023-01-23 13:38:04.000000 simulai-toolkit-0.99.9/docs/_modules/simulai.mesh.rst
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)      117 2023-01-23 13:38:04.000000 simulai-toolkit-0.99.9/docs/_modules/simulai.metrics.rst
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)      135 2023-01-23 13:38:04.000000 simulai-toolkit-0.99.9/docs/_modules/simulai.normalization.rst
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)      113 2023-01-23 13:38:04.000000 simulai-toolkit-0.99.9/docs/_modules/simulai.output.rst
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)      119 2023-01-23 13:38:04.000000 simulai-toolkit-0.99.9/docs/_modules/simulai.parallel.rst
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)      125 2023-01-23 13:38:04.000000 simulai-toolkit-0.99.9/docs/_modules/simulai.simulation.rst
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)      116 2023-01-23 13:38:04.000000 simulai-toolkit-0.99.9/docs/_modules/simulai.special.rst
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)      113 2023-01-23 13:38:04.000000 simulai-toolkit-0.99.9/docs/_modules/simulai.tokens.rst
+drwxr-xr-x   0 jalmeida  (1000) jalmeida  (1000)        0 2023-01-23 17:58:12.847577 simulai-toolkit-0.99.9/docs/_package/
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     1442 2023-01-23 13:38:04.000000 simulai-toolkit-0.99.9/docs/_package/simulai.math.rst
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)      183 2023-01-23 13:38:04.000000 simulai-toolkit-0.99.9/docs/_package/simulai.models.rst
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)      777 2023-01-23 13:38:04.000000 simulai-toolkit-0.99.9/docs/_package/simulai.optimization.rst
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     1031 2023-01-23 13:38:04.000000 simulai-toolkit-0.99.9/docs/_package/simulai.regression.rst
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)      231 2023-01-23 13:38:04.000000 simulai-toolkit-0.99.9/docs/_package/simulai.residuals.rst
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)      160 2023-01-23 13:38:04.000000 simulai-toolkit-0.99.9/docs/_package/simulai.rom.rst
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)      235 2023-01-23 13:38:04.000000 simulai-toolkit-0.99.9/docs/_package/simulai.sampling.rst
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     1006 2023-01-23 13:38:04.000000 simulai-toolkit-0.99.9/docs/_package/simulai.utilities.rst
+drwxr-xr-x   0 jalmeida  (1000) jalmeida  (1000)        0 2023-01-23 17:58:12.847577 simulai-toolkit-0.99.9/docs/_templates/
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)      725 2023-01-20 17:39:11.000000 simulai-toolkit-0.99.9/docs/_templates/ISSUES_TEMPLATE.rst
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     2317 2023-01-20 16:55:17.000000 simulai-toolkit-0.99.9/docs/conf.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)      866 2023-01-23 13:38:04.000000 simulai-toolkit-0.99.9/docs/index.rst
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     5092 2023-01-23 13:38:04.000000 simulai-toolkit-0.99.9/docs/quickstart.rst
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     2014 2023-01-23 17:57:56.000000 simulai-toolkit-0.99.9/pyproject.toml
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)       38 2023-01-23 17:58:12.884577 simulai-toolkit-0.99.9/setup.cfg
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)      226 2022-12-05 14:53:20.000000 simulai-toolkit-0.99.9/setup.py
+drwxr-xr-x   0 jalmeida  (1000) jalmeida  (1000)        0 2023-01-23 17:58:12.834576 simulai-toolkit-0.99.9/simulai/
+drwxr-xr-x   0 jalmeida  (1000) jalmeida  (1000)        0 2023-01-23 17:58:12.850577 simulai-toolkit-0.99.9/simulai/math/
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)      935 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.9/simulai/math/__init__.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)    15703 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.9/simulai/math/differentiation.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     5388 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.9/simulai/math/expressions.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)    15368 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.9/simulai/math/filtering.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)    14648 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.9/simulai/math/integration.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)    18177 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.9/simulai/math/kansas.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     2379 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.9/simulai/math/products.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     1505 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.9/simulai/math/progression.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     5348 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.9/simulai/math/quadratures.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     4790 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.9/simulai/math/spaces.py
+drwxr-xr-x   0 jalmeida  (1000) jalmeida  (1000)        0 2023-01-23 17:58:12.850577 simulai-toolkit-0.99.9/simulai/models/
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     1135 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.9/simulai/models/__init__.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)    45556 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.9/simulai/models/_models.py
+drwxr-xr-x   0 jalmeida  (1000) jalmeida  (1000)        0 2023-01-23 17:58:12.852577 simulai-toolkit-0.99.9/simulai/models/_pytorch_models/
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)      262 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.9/simulai/models/_pytorch_models/__init__.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)    28401 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.9/simulai/models/_pytorch_models/_autoencoder.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)    27165 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.9/simulai/models/_pytorch_models/_deeponet.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     6644 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.9/simulai/models/_pytorch_models/_miscellaneous.py
+drwxr-xr-x   0 jalmeida  (1000) jalmeida  (1000)        0 2023-01-23 17:58:12.853577 simulai-toolkit-0.99.9/simulai/optimization/
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)      997 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.9/simulai/optimization/__init__.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     4832 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.9/simulai/optimization/_builtin.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     7794 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.9/simulai/optimization/_builtin_pytorch.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)    46917 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.9/simulai/optimization/_losses.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)    24509 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.9/simulai/optimization/_optimization.py
+drwxr-xr-x   0 jalmeida  (1000) jalmeida  (1000)        0 2023-01-23 17:58:12.855577 simulai-toolkit-0.99.9/simulai/regression/
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     1568 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.9/simulai/regression/__init__.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     5944 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.9/simulai/regression/_affine.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     6050 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.9/simulai/regression/_elm.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)    73087 2023-01-23 12:30:32.000000 simulai-toolkit-0.99.9/simulai/regression/_esn.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     6530 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.9/simulai/regression/_extended_opinf.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)    35955 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.9/simulai/regression/_opinf.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     1445 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.9/simulai/regression/_pinv.py
+drwxr-xr-x   0 jalmeida  (1000) jalmeida  (1000)        0 2023-01-23 17:58:12.858577 simulai-toolkit-0.99.9/simulai/regression/pytorch/
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)      661 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.9/simulai/regression/pytorch/__init__.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     5632 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.9/simulai/regression/pytorch/_conv.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)    13650 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.9/simulai/regression/pytorch/_dense.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)    14336 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.9/simulai/regression/pytorch/_koopman.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     1439 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.9/simulai/regression/pytorch/_numpy.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)    14345 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.9/simulai/regression/pytorch/_opinf.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     7596 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.9/simulai/regression/pytorch/_rbf.py
+drwxr-xr-x   0 jalmeida  (1000) jalmeida  (1000)        0 2023-01-23 17:58:12.858577 simulai-toolkit-0.99.9/simulai/residuals/
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)      879 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.9/simulai/residuals/__init__.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)    14788 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.9/simulai/residuals/_pytorch_residuals.py
+drwxr-xr-x   0 jalmeida  (1000) jalmeida  (1000)        0 2023-01-23 17:58:12.859577 simulai-toolkit-0.99.9/simulai/rom/
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)      931 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.9/simulai/rom/__init__.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)    31649 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.9/simulai/rom/_rom.py
+drwxr-xr-x   0 jalmeida  (1000) jalmeida  (1000)        0 2023-01-23 17:58:12.860577 simulai-toolkit-0.99.9/simulai/sampling/
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)       36 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.9/simulai/sampling/__init__.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     6007 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.9/simulai/sampling/_hamiltonian_sampling.py
+drwxr-xr-x   0 jalmeida  (1000) jalmeida  (1000)        0 2023-01-23 17:58:12.862577 simulai-toolkit-0.99.9/simulai/simulai_toolkit.egg-info/
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     1324 2023-01-23 17:58:12.000000 simulai-toolkit-0.99.9/simulai/simulai_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     4610 2023-01-23 17:58:12.000000 simulai-toolkit-0.99.9/simulai/simulai_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)        1 2023-01-23 17:58:12.000000 simulai-toolkit-0.99.9/simulai/simulai_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)      218 2023-01-23 17:58:12.000000 simulai-toolkit-0.99.9/simulai/simulai_toolkit.egg-info/requires.txt
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)       89 2023-01-23 17:58:12.000000 simulai-toolkit-0.99.9/simulai/simulai_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 jalmeida  (1000) jalmeida  (1000)        0 2023-01-23 17:58:12.864577 simulai-toolkit-0.99.9/simulai/templates/
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)      955 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.9/simulai/templates/__init__.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)    23329 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.9/simulai/templates/_pytorch_network.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     1704 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.9/simulai/templates/_templates.py
+drwxr-xr-x   0 jalmeida  (1000) jalmeida  (1000)        0 2023-01-23 17:58:12.866577 simulai-toolkit-0.99.9/simulai/utilities/
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)      765 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.9/simulai/utilities/__init__.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)      794 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.9/simulai/utilities/_makedirs_to_file.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)      869 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.9/simulai/utilities/_tmp_dir.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     7618 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.9/simulai/utilities/lorenz_solver.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     1298 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.9/simulai/utilities/lotka_volterra_solver.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     3581 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.9/simulai/utilities/opinf_deviation.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     3936 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.9/simulai/utilities/oscillator_solver.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     4473 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.9/simulai/utilities/problem_classes.py
+drwxr-xr-x   0 jalmeida  (1000) jalmeida  (1000)        0 2023-01-23 17:58:12.869577 simulai-toolkit-0.99.9/simulai/workflows/
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     1137 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.9/simulai/workflows/__init__.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     3263 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.9/simulai/workflows/_cloud_object_storage.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)    23351 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.9/simulai/workflows/_esn_modelpool_train.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     4952 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.9/simulai/workflows/_extrapolation.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     1943 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.9/simulai/workflows/_h5_comparison.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)    12556 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.9/simulai/workflows/_h5_ipod.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     1824 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.9/simulai/workflows/_neural_net_timeint.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)    10763 2023-01-20 16:10:46.000000 simulai-toolkit-0.99.9/simulai/workflows/_parametric_hyperopt.py
+drwxr-xr-x   0 jalmeida  (1000) jalmeida  (1000)        0 2023-01-23 17:58:12.870577 simulai-toolkit-0.99.9/tests/
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)      152 2022-12-05 14:53:20.000000 simulai-toolkit-0.99.9/tests/README.md
+drwxr-xr-x   0 jalmeida  (1000) jalmeida  (1000)        0 2023-01-23 17:58:12.871577 simulai-toolkit-0.99.9/tests/devices/
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     5165 2023-01-18 13:08:53.000000 simulai-toolkit-0.99.9/tests/devices/test_network_devices.py
+drwxr-xr-x   0 jalmeida  (1000) jalmeida  (1000)        0 2023-01-23 17:58:12.872577 simulai-toolkit-0.99.9/tests/math/
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     3277 2023-01-09 15:45:17.000000 simulai-toolkit-0.99.9/tests/math/test_LSODA.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     2606 2022-12-05 14:53:20.000000 simulai-toolkit-0.99.9/tests/math/test_RK4.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     3945 2023-01-05 19:58:08.000000 simulai-toolkit-0.99.9/tests/math/test_collocation_derivative.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)    10326 2023-01-18 13:53:40.000000 simulai-toolkit-0.99.9/tests/math/test_metrics.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     1096 2023-01-12 13:30:25.000000 simulai-toolkit-0.99.9/tests/math/test_products.py
+drwxr-xr-x   0 jalmeida  (1000) jalmeida  (1000)        0 2023-01-23 17:58:12.873577 simulai-toolkit-0.99.9/tests/metrics/
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)      556 2022-12-05 14:53:20.000000 simulai-toolkit-0.99.9/tests/metrics/test_mahalanobis.py
+drwxr-xr-x   0 jalmeida  (1000) jalmeida  (1000)        0 2023-01-23 17:58:12.875577 simulai-toolkit-0.99.9/tests/network/
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     5168 2023-01-04 14:20:32.000000 simulai-toolkit-0.99.9/tests/network/test_conv_1d.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     5183 2023-01-04 14:20:32.000000 simulai-toolkit-0.99.9/tests/network/test_conv_2d.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)    10158 2023-01-20 13:11:28.000000 simulai-toolkit-0.99.9/tests/network/test_deeponet.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     7617 2023-01-11 18:27:18.000000 simulai-toolkit-0.99.9/tests/network/test_dense.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     2972 2023-01-18 13:08:53.000000 simulai-toolkit-0.99.9/tests/network/test_elm.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     5908 2023-01-20 13:25:36.000000 simulai-toolkit-0.99.9/tests/network/test_flexible_deeponet.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     5943 2023-01-20 13:25:37.000000 simulai-toolkit-0.99.9/tests/network/test_improved_deeponet.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     7477 2023-01-23 12:52:41.000000 simulai-toolkit-0.99.9/tests/network/test_residual_cnn.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)      402 2023-01-04 14:23:31.000000 simulai-toolkit-0.99.9/tests/network/utils.py
+drwxr-xr-x   0 jalmeida  (1000) jalmeida  (1000)        0 2023-01-23 17:58:12.876577 simulai-toolkit-0.99.9/tests/opinf/
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     3649 2023-01-19 12:58:40.000000 simulai-toolkit-0.99.9/tests/opinf/test_extended_opinf_operators_construction.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)    14908 2023-01-20 14:35:19.000000 simulai-toolkit-0.99.9/tests/opinf/test_opinf_operators_construction.py
+drwxr-xr-x   0 jalmeida  (1000) jalmeida  (1000)        0 2023-01-23 17:58:12.877577 simulai-toolkit-0.99.9/tests/parallelism/
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     3510 2023-01-18 13:53:40.000000 simulai-toolkit-0.99.9/tests/parallelism/test_modelpool_affinemapping.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)    35318 2023-01-23 12:38:20.000000 simulai-toolkit-0.99.9/tests/parallelism/test_modelpool_esn.py
+drwxr-xr-x   0 jalmeida  (1000) jalmeida  (1000)        0 2023-01-23 17:58:12.877577 simulai-toolkit-0.99.9/tests/postprocessing/
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     3091 2022-12-05 14:53:20.000000 simulai-toolkit-0.99.9/tests/postprocessing/test_batchwise_extrapolation.py
+drwxr-xr-x   0 jalmeida  (1000) jalmeida  (1000)        0 2023-01-23 17:58:12.879577 simulai-toolkit-0.99.9/tests/preprocessing/
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     3588 2023-01-18 13:53:40.000000 simulai-toolkit-0.99.9/tests/preprocessing/test_batch_copy.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     1305 2022-12-05 14:53:20.000000 simulai-toolkit-0.99.9/tests/preprocessing/test_batching.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     5232 2023-01-18 13:53:40.000000 simulai-toolkit-0.99.9/tests/preprocessing/test_mapvalid.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     3789 2023-01-18 13:53:40.000000 simulai-toolkit-0.99.9/tests/preprocessing/test_meanevaluation.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)      999 2022-12-05 14:53:20.000000 simulai-toolkit-0.99.9/tests/preprocessing/test_minmax.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     3835 2022-12-05 14:53:20.000000 simulai-toolkit-0.99.9/tests/preprocessing/test_moving_window.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)    10930 2023-01-18 13:53:40.000000 simulai-toolkit-0.99.9/tests/preprocessing/test_reshaper.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     4348 2023-01-18 13:53:40.000000 simulai-toolkit-0.99.9/tests/preprocessing/test_sampler.py
+drwxr-xr-x   0 jalmeida  (1000) jalmeida  (1000)        0 2023-01-23 17:58:12.880577 simulai-toolkit-0.99.9/tests/rbf/
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     1793 2022-12-05 14:53:20.000000 simulai-toolkit-0.99.9/tests/rbf/test_rbf.py
+drwxr-xr-x   0 jalmeida  (1000) jalmeida  (1000)        0 2023-01-23 17:58:12.880577 simulai-toolkit-0.99.9/tests/residuals/
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     5728 2023-01-18 13:08:53.000000 simulai-toolkit-0.99.9/tests/residuals/test_symbolicoperator.py
+drwxr-xr-x   0 jalmeida  (1000) jalmeida  (1000)        0 2023-01-23 17:58:12.883577 simulai-toolkit-0.99.9/tests/rom/
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     5766 2023-01-19 12:23:11.000000 simulai-toolkit-0.99.9/tests/rom/test_cnn_autoencoder.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     1970 2022-12-05 14:53:20.000000 simulai-toolkit-0.99.9/tests/rom/test_dmd_decomposition.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     3469 2022-12-05 14:53:20.000000 simulai-toolkit-0.99.9/tests/rom/test_gappy_pca_decomposition.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     5025 2023-01-12 13:17:44.000000 simulai-toolkit-0.99.9/tests/rom/test_hosvd.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     6108 2023-01-18 13:53:40.000000 simulai-toolkit-0.99.9/tests/rom/test_ipca_datapreparer.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     9812 2023-01-18 13:53:40.000000 simulai-toolkit-0.99.9/tests/rom/test_ipca_decomposition.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     2619 2023-01-19 15:57:55.000000 simulai-toolkit-0.99.9/tests/rom/test_mlp_autoencoder.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     5486 2023-01-12 12:48:41.000000 simulai-toolkit-0.99.9/tests/rom/test_pca_decomposition.py
+-rw-r--r--   0 jalmeida  (1000) jalmeida  (1000)     2563 2023-01-12 16:55:23.000000 simulai-toolkit-0.99.9/tests/rom/test_qqm.py
```

### Comparing `simulai-toolkit-0.99.8/AUTHORS.rst` & `simulai-toolkit-0.99.9/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `simulai-toolkit-0.99.8/CONTRIBUTING.rst` & `simulai-toolkit-0.99.9/CONTRIBUTING.rst`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 If you are reporting a bug, please include:
 
 * Your operating system name and version.
 * Any details about your local setup that might be helpful in troubleshooting.
 * Detailed steps to reproduce the bug.
 
-Be sure to take a look at the template here: https://github.com/IBM/simulai/tree/main/docs/_templates/ISSUE_TEMPLATE.rst
+Be sure to take a look at the template here: https://github.com/IBM/simulai/tree/main/docs/_templates/ISSUES_TEMPLATE.rst
 
 Fix Bugs
 ~~~~~~~~
 
 Look through the GitHub issues for bugs. Anything tagged with "bug" and "help
 wanted" is open to whoever wants to implement it.
```

### Comparing `simulai-toolkit-0.99.8/LICENSE` & `simulai-toolkit-0.99.9/LICENSE`

 * *Files identical despite different names*

### Comparing `simulai-toolkit-0.99.8/PKG-INFO` & `simulai-toolkit-0.99.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simulai-toolkit
-Version: 0.99.8
+Version: 0.99.9
 Summary: A Python package with data-driven pipelines for physics-informed machine learning
 License: Apache License, Version 2.0
 Project-URL: Source, https://github.com/IBM/simulai
 Project-URL: Tracker, https://github.com/IBM/simulai/issues
 Project-URL: Documentation, https://simulai-toolkit.readthedocs.io
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `simulai-toolkit-0.99.8/README.rst` & `simulai-toolkit-0.99.9/README.rst`

 * *Files identical despite different names*

### Comparing `simulai-toolkit-0.99.8/docs/_package/simulai.math.rst` & `simulai-toolkit-0.99.9/docs/_package/simulai.math.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-simulai.math package
-====================
+Math Package
+============
 
 simulai.math.differentiation module
 -----------------------------------
 
 .. automodule:: simulai.math.differentiation
    :members:
    :undoc-members:
@@ -32,15 +32,15 @@
    :members:
    :undoc-members:
    :show-inheritance:
 
 simulai.math.kansas module
 --------------------------
 
-.. automodule:: simulai.:math.expression
+.. automodule:: simulai.math.kansas
    :members:
    :undoc-members:
    :show-inheritance:
 
 simulai.math.products module
 ----------------------------
```

### Comparing `simulai-toolkit-0.99.8/docs/_package/simulai.utilities.rst` & `simulai-toolkit-0.99.9/docs/_package/simulai.utilities.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-simulai.utilities package
-=========================
+Utilities Package
+=================
 
 simulai.utilities.lorenz\_solver module
 ---------------------------------------
 
 .. automodule:: simulai.utilities.lorenz_solver
    :members:
    :undoc-members:
```

### Comparing `simulai-toolkit-0.99.8/docs/conf.py` & `simulai-toolkit-0.99.9/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 import sphinx_theme
 html_theme = 'stanford_theme'
 html_theme_path = [sphinx_theme.get_html_theme_path('stanford-theme')]
 
 # sphinx readthedocs theme
 #html_theme = 'sphinx_rtd_theme'
 
-html_logo = '_static/logo.png'
+html_logo = '../assets/logo.png'
 
 # Below html_theme_options config depends on the theme.
 # For Stanford theme:
 # https://sphinx-rtd-theme.readthedocs.io/en/stable/configuring.html
 html_theme_options = {
     'logo_only': True,
     'display_version': True
```

### Comparing `simulai-toolkit-0.99.8/docs/quickstart.rst` & `simulai-toolkit-0.99.9/docs/quickstart.rst`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
    :target: https://badge.fury.io/py/simulai-toolkit
 .. image:: https://readthedocs.org/projects/simulai-toolkit/badge/?version=latest
    :target: https://simulai-toolkit.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status
 .. image:: ../assets/coverage.svg
    :target: tests/ 
     
-.. image:: _static/logo.png
+.. image:: ../assets/logo.png
 
 A Python package with data-driven pipelines for physics-informed machine learning.
 
 .. image:: ../assets/simulai_diagram.svg
 
 The SimulAI toolkit provides easy access to state-of-the-art models and algorithms for physics-informed machine learning. Currently, it includes the following methods described in the literature:
```

### Comparing `simulai-toolkit-0.99.8/pyproject.toml` & `simulai-toolkit-0.99.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools" ]
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "simulai-toolkit"
-version = "0.99.8"
+version = "0.99.9"
 description = "A Python package with data-driven pipelines for physics-informed machine learning"
 license = { "text" = "Apache License, Version 2.0" }
 readme = { "file" = "DESCRIPTION.md", "content-type" = "text/markdown" }
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: Apache Software License",
@@ -51,25 +51,26 @@
 mpi = ["mpi4py"]
 
 [project.urls]
 Source = "https://github.com/IBM/simulai"
 Tracker = "https://github.com/IBM/simulai/issues"
 Documentation = "https://simulai-toolkit.readthedocs.io"
 
-[tool.setuptools]
-packages = ['simulai']
+#[tool.setuptools]
+#packages = ['simulai']
+
+[tool.setuptools.packages.find]
+where = ["simulai"]
 
 [tool.bumpver]
-current_version = "0.99.8"
-version_pattern = "MAJOR.MINOR.PATCH"
+current_version = "0.99.9"
+version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
     'current_version = "{version}"',
     'version = "{version}"'
 ]
-    
-
```

### Comparing `simulai-toolkit-0.99.8/simulai/__init__.py` & `simulai-toolkit-0.99.9/simulai/math/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,20 +12,9 @@
 #     See the License for the specific language governing permissions and
 #     limitations under the License.
 
 # (C) Copyright IBM Corporation 2017, 2018, 2019
 # U.S. Government Users Restricted Rights:  Use, duplication or disclosure restricted
 # by GSA ADP Schedule Contract with IBM Corp.
 #
-# Author: Joao Lucas S. Almeida <joao.lucas.sousa.almeida@ibm.com>
-
-import os
-
-engine_var = os.environ.get('engine')
-
-if engine_var is not None:
-    engine = engine_var
-else:
-    engine = 'pytorch'
-
-__version__ = '1.3'
-
+# Author: Joao Lucas de Sousa Almeida <joao.lucas.sousa.almeida@ibm.com>
+# Author: Leonardo P. Tizzei <ltizzei@br.ibm.com>
```

### Comparing `simulai-toolkit-0.99.8/simulai/io.py` & `simulai-toolkit-0.99.9/simulai/rom/_rom.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,1030 +8,991 @@
 
 #     Unless required by applicable law or agreed to in writing, software
 #     distributed under the License is distributed on an "AS IS" BASIS,
 #     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #     See the License for the specific language governing permissions and
 #     limitations under the License.
 
-import sys
 import numpy as np
-import torch
-import h5py
-import random
-from typing import Union, Dict, List
-from torch import Tensor
-from numpy.lib import recfunctions
-
-from simulai.batching import batchdomain_constructor
-from simulai.metrics import MemorySizeEval
-from simulai.abstract import DataPreparer
-from simulai.batching import indices_batchdomain_constructor
-from simulai.abstract import Dataset
-
-
-"""
-    BEGIN DataPreparer children
-"""
+import os
+import pickle
+import importlib
+import copy
+from typing import List, Tuple, Union
+
+from sklearn.decomposition import PCA, IncrementalPCA, TruncatedSVD
+import dask.array as da
 
-# This class does nothing
-class ByPassPreparer(DataPreparer):
+from simulai.abstract import ROM
+from simulai.optimization import SpaRSA
 
-    """
-    ByPass class, it fills the DataPreparer blank, but does nothing.
-    """
-    name = "no_preparer"
+class ByPassROM(ROM):
 
-    def __init__(self, channels_last:bool=False) -> None:
+    name = 'no_rom'
+    def __init__(self) -> None:
 
         super().__init__()
 
-        self.channels_last = channels_last
-        self.collapsible_shapes = None
-        self.dtype = None
-
-    def prepare_input_data(self, data:np.ndarray) -> np.ndarray:
-
-        self.collapsible_shapes = data.shape[1:]
-
-        return data
-
-    def prepare_output_data(self, data:np.ndarray) -> np.ndarray:
-
-        return data
+    def __call__(self):
+        pass
 
-    def prepare_input_structured_data(self, data:np.recarray) -> np.ndarray:
+class IByPass(ROM):
 
-        return data
+    """
+    It executes the Incremental Proper Orthogonal Decomposition using the SciKit-learn interface
+    The IncrementalPCA class from SciKit-learn expects a two-dimensional array
+    as input, so it is necessary to reshape the input data before processing it.
+    This class is intended to be used for Big Data purposes.
+    """
 
-    def prepare_output_structured_data(self, data:np.ndarray) -> np.recarray:
+    name = "ibypass"
 
-        return data
+    def __init__(self, config=None, data_mean=None):
 
-# It is used for high-dimensional datasets, in order to convert them to
-# 2D ones
-class Reshaper(DataPreparer):
+        super().__init__()
 
-    name = "reshaper"
+        self.kind = "batchwise"
 
-    def __init__(self, channels_last:bool=False) -> None:
+    def fit(self, data:np.ndarray=None) -> None:
 
         """
+        Output shape: (space_dimension, n_modes)
 
-        Reshaper converts n-dimensional arrays to two-dimensional ones, performing a
-        simple reshaping operation F: (n0, n1, ..., nm) -> (n0, prod(n1, ..., nm))
-
+        :param data:
+        :type data: hdf5.File
         """
+        pass
 
-        super().__init__()
-
-        # Nomenclature: shape = (immutable_shape, *collapsible_shapes)
-        self.channels_last = channels_last
-        self.collapsible_shapes = None
-        self.collapsed_shape = None
-        self.dtype = None
-        self.n_features = None
-
-    def _set_shapes_from_data(self, data:np.ndarray=None) -> None:
-
-        self.collapsible_shapes = data.shape[1:]
-        self.collapsed_shape = np.prod(self.collapsible_shapes).astype(int)
-        self._is_recarray = data.dtype.names is not None
-        if self._is_recarray:
-            self.n_features = len(data.dtype.names)*self.collapsed_shape
-        else:
-            self.n_features = self.collapsed_shape
-
-    def _prepare_input_data(self, data:np.ndarray=None) -> np.ndarray:
-
-        assert len(data.shape) > 1, 'Error! data must have at least two dimensions'
-        return data.reshape((data.shape[0], self.n_features))
-
-    def prepare_input_data(self, data:Union[np.ndarray, np.recarray]) -> np.ndarray:
-
-        self._set_shapes_from_data(data)
-        if self._is_recarray:
-            return self._prepare_input_structured_data(data)
-        else:
-            return self._prepare_input_data(data)
+    def project(self, data:np.ndarray=None) -> np.ndarray:
 
-    def _reshape_to_output(self, data:np.ndarray) -> np.ndarray:
-
-        return data.reshape((data.shape[0],) + self.collapsible_shapes)
-
-    def _prepare_output_data(self, data:np.ndarray=None, single:bool=False) -> np.ndarray:
-
-        if self._is_recarray:
-            return self._prepare_output_structured_data(data)
-        else:
-            return self._reshape_to_output(data)
+        """
+        Output shape: (n_timesteps, n_modes)
+        """
 
-    def prepare_output_data(self, data:np.ndarray, single:bool=False) -> np.ndarray:
+        return data
 
-        return self._prepare_output_data(data)
+    def reconstruct(self, projected_data:np.ndarray=None) -> np.ndarray:
 
-    def _prepare_input_structured_data(self, data:np.recarray=None) -> np.ndarray:
+        """
+        Output shape: (space_dimension, n_timesteps)
+        """
 
-        self.dtype = data.dtype
-        self._set_shapes_from_data(data)
-        data_ = recfunctions.structured_to_unstructured(data)
-        reshaped_data_ = self._prepare_input_data(data_)
-        return reshaped_data_
+        return projected_data
 
-    def prepare_input_structured_data(self, data:np.recarray=None) -> np.ndarray:
+    def save(self, save_path:str=None, model_name:str=None) -> None:
 
-        return self._prepare_input_structured_data(data)
+        """It saves data in a NPZ file
+        :param save_path: path to save the model
+        :type save_path: str
+        :param model_name: name for the saved model
+        :type model_name: str
+        :return: nothing
+        """
 
-    def prepare_output_structured_data(self, data:np.ndarray=None) -> np.recarray:
+        np.savez(os.path.join(save_path, model_name+'.npz'), self.modes, self.data_mean)
 
-        return self._prepare_output_structured_data(data)
+    def restore(self, save_path:str=None, model_name:str=None) -> None:
 
-    def _prepare_output_structured_data(self, data:np.ndarray=None) -> np.recarray:
+        """It saves data in a NPZ file
+        :param save_path: path to save the model
+        :type save_path: str
+        :param model_name: name for the saved model
+        :type model_name: str
+        :return: nothing
+        """
 
-        data = data.reshape((data.shape[0], ) + self.collapsible_shapes + (len(self.dtype), ))
-        output_data = recfunctions.unstructured_to_structured(data, self.dtype)
-        output_data = self._reshape_to_output(output_data)
+        self.modes, self.data_mean = np.load(os.path.join(save_path, model_name + '.npz'))
 
-        return output_data
 
+class ParallelSVD(ROM):
 
-# It is used for high-dimensional datasets, in order to scale and convert them to
-# 2D ones
-class ScalerReshaper(Reshaper):
+    name = 'parallel_svd'
 
-    name = "scalerreshaper"
+    def __init__(self, n_components:int=None, chunks:Tuple[int]=None) -> None:
 
-    def __init__(self, bias:float=0., scale:float=1., channels_last:bool=False) -> None:
+        """Executing SVD using dask
 
         """
+        super().__init__()
 
-        Reshaper converts n-dimensional arrays to two-dimensional ones, performing a
-        simple reshaping operation F: (n0, n1, ..., nm) -> (n0, prod(n1, ..., nm))
-
-        """
+        self.n_components = n_components
+        self.chunks = chunks
+        self.default_chunks_numbers = (10, 10)
+        self.U = None
+        self.s = None
+        self.V = None
 
-        super().__init__(channels_last=channels_last)
+    def _chunk_size_condition(self, size:int, chunk_size:int) -> int:
 
-        # Nomenclature: shape = (immutable_shape, *collapsible_shapes)
-        self.bias = bias
-        self.scale = scale
+        if size // chunk_size == 0:
+            return size
+        else:
+            return size // chunk_size
 
-    def prepare_input_data(self, data:Union[np.ndarray, np.recarray]=None, *args, **kwargs) -> np.ndarray:
+    def fit(self, data:Union[np.ndarray, da.core.Array]=None) -> Union[np.ndarray, da.core.Array]:
 
-        if data.dtype.names is None:
-            return super(ScalerReshaper, self).prepare_input_data((data-self.bias)/self.scale, *args, **kwargs)
+        if self.chunks == None:
+            chunks = [self._chunk_size_condition(size, self.default_chunks_numbers[j])
+                      for j, size in enumerate(data.shape)]
         else:
-            return self.prepare_input_structured_data(data, *args, **kwargs)
+            chunks = self.chunks
 
-    def prepare_output_data(self, data:Union[np.ndarray, np.recarray]=None, *args, **kwargs) -> np.ndarray:
-        if not self._is_recarray:
-            return super(ScalerReshaper, self).prepare_output_data(data*self.scale+self.bias, *args, **kwargs)
+        if isinstance(data, np.ndarray):
+            parallel_data = da.from_array(data, chunks=chunks)
         else:
-            return self.prepare_output_structured_data(data)
-
-    def _get_structured_bias_scale(self, dtype:np.dtype=None) -> (float, float):
-
-        bias = self.bias
-        if isinstance(self.bias, float):
-            bias = {n: self.bias for n in dtype.names}
-        scale = self.scale
-        if isinstance(self.scale, float):
-            scale = {n: self.scale for n in dtype.names}
+            parallel_data = data
 
-        return bias, scale
+        U, s, V = da.linalg.svd_compressed(parallel_data, k=self.n_components)
 
-    def prepare_input_structured_data(self, data:np.recarray=None, *args, **kwargs) -> np.ndarray:
+        self.U = U
+        self.s = s
+        self.V = V
 
-        bias, scale = self._get_structured_bias_scale(data.dtype)
 
-        data = data.copy()
-        names = data.dtype.names
-        for name in names:
-            data[name] = (data[name]-bias[name])/scale[name]
-
-        return super(ScalerReshaper, self).prepare_input_structured_data(data, *args, **kwargs)
-
-    def prepare_output_structured_data(self, data:np.ndarray=None, *args, **kwargs) -> np.recarray:
-
-        bias, scale = self._get_structured_bias_scale(self.dtype)
-        data = super(ScalerReshaper, self).prepare_output_structured_data(data, *args, **kwargs)
-        data = data.copy()
-        for name in self.dtype.names:
-            data[name] = data[name]*scale[name]+bias[name]
-        return data
-
-
-# It is used for datasets in which there are invalid data
-class MapValid(Reshaper):
+class POD(ROM):
 
     """
-    MapValid converts n-dimensional arrays to two-dimensional ones performing a valid values
-    mapping operation F: F: data.shape = (n0, n1, ..., nm) -> data'.shape = (n0, n_valids)
-    n_valids = dim([k in data[0, ...] if k != mask])
-    WARNING: the invalid positions are expected to be static in relation to n0.
+    It executes the classical Proper Orthogonal Decomposition using the SciKit-learn interface.
+    The PCA class from SciKit-learn expects a two-dimensional array
+    as input, so it is necessary to reshape the input data in order to
+    ensure that
     """
 
-    name = "map_valid"
+    name = "pod"
 
-    def __init__(self, config:dict=None, mask=None, channels_last:bool=True) -> None:
+    def __init__(self, config:dict=None, svd_filter:callable=None) -> None:
 
-        """
-
-        :param config: configurations dictionary
+        """Propor Orthogonal Decomposition
+        :param config: configuration dictionary for the POD parameters
         :type config: dict
-        :param mask:  mask to select the invalid values
-        :type: int, np.NaN or np.inf
-
+        :param svd_filter: a filter callable applied to SVD decomposition
+        :type svd_filter: callable
+        :return: nothing
         """
 
         super().__init__()
 
-        # Some default parameters which can be
-        # overwritten by the config content
+        if 'n_components' not in config:
+            config['n_components'] = None
 
-        self.default_dtype = 'float64'
-
-        if mask == 0 or isinstance(mask, int):
-            self.replace_mask_with_large_number = False
+        if 'mean_component' in config:
+            self.mean_component = config.pop('mean_component')
         else:
-            self.replace_mask_with_large_number = True
-
-        self.return_the_same_mask = True
+            self.mean_component = True
 
-        for key, value in config.items():
-            setattr(self, key, value)
-
-        # Default value for very large numbers
-        self.large_number = 1e15
-
-        if not mask or self.replace_mask_with_large_number:
-            self.mask = self.large_number
+        if 'eig_norm' in config:
+            self.eig_norm = config.pop('eig_norm')
         else:
-            self.mask = mask
+            self.eig_norm = False
 
-        self.mask_ = mask
+        self.pca = PCA(**config)
 
-        for key, value in config.items():
-            setattr(self, key, value)
+        self.modes = None
 
-        self.valid_indices = None
-        self.original_dimensions = None
+        self.data_mean = None
 
-        self.channels_last = channels_last
+        self.svd_filter = svd_filter
 
-    def prepare_input_data(self, data:np.ndarray=None) -> np.ndarray:
+    def fit(self, data:np.ndarray=None) -> None:
 
         """
-
-        Internal input data preparer, executed for each label of the structured array
-
         :param data:
         :type data: np.ndarray
-        :return:
-        :rtype: np.ndarray
-
+        :return: nothing
         """
 
-        data = super(MapValid, self).prepare_input_data(data)
+        if self.mean_component:
+            self.data_mean = data.mean(0)
+            data_til = data - self.data_mean
 
-        if self.mask == self.large_number:
-            self.valid_indices_ = np.where(data[0, ...] < self.mask)
-
-        elif not str(self.mask).isnumeric() or isinstance(self.mask, int):
-            self.valid_indices_ = np.where(data[0, ...] != self.mask)
+            mean_contrib = np.linalg.norm(self.data_mean, 2) / np.linalg.norm(data, 2)
 
+            print("Relative contribution of the mean component: {}".format(mean_contrib))
         else:
-            raise Exception("The chosen mask {} does not fit in any supported case".format(self.mask))
+            data_til = data
 
-        samples_dim = data.shape[0]
+        decomp = self.pca.fit(data_til)
 
-        valid_indices = (slice(0, samples_dim), ) + self.valid_indices_
+        self.modes = decomp.components_
+        self.singular_values = decomp.singular_values_
 
-        return data[valid_indices]
+        # Executing SVD filtering over the singular values if necessary
+        if self.svd_filter is not None:
+            self.singular_values_truncated = self.svd_filter.exec(singular_values=self.singular_values,
+                                                                  data_shape=data.shape)
+            n_values = len(self.singular_values_truncated)
+            self.singular_values = self.singular_values_truncated
+            self.modes = self.modes[:n_values, :]
 
-    def prepare_output_data(self, data:np.ndarray=None) -> np.ndarray:
+        else:
+            pass
 
-        """
+        relative_modal_energy = decomp.explained_variance_ratio_.sum()
 
-        Internal output.py data preparer, executed for each label of
-        the structured array
+        print("Relative Modal Energy {}".format(relative_modal_energy))
 
-        :param data:
+    def project(self, data:np.ndarray=None) -> np.ndarray:
+
+        """
+        :param data: array of shape (n_samples, n_features)
         :type data: np.ndarray
-        :return:
+        :return: array of shape (n_samples, n_modes) containing the projection over the POD basis
         :rtype: np.ndarray
-
         """
 
-        immutable_shape = data.shape[0]
+        if self.mean_component:
+            data_til = data - self.data_mean
+        else:
+            data_til = data
 
-        final_shape = (immutable_shape, self.n_features, )
+        if not type(self.modes) == np.ndarray:
+            self.fit(data_til)
 
-        if self.return_the_same_mask:
-            mask = self.mask_
+        if self.eig_norm:
+            return np.sqrt(self.singular_values)[None,:]*(data_til.dot(self.modes.T))
         else:
-            mask = np.NaN  # For practical purposes
-        reshaped_data = np.full(final_shape, mask)
+            return data_til.dot(self.modes.T)
 
-        if not reshaped_data.dtype.type == self.default_dtype:
-            reshaped_data = reshaped_data.astype(self.default_dtype)
+    def reconstruct(self, projected_data:np.ndarray=None) -> np.ndarray:
 
-        samples_dim = data.shape[0]
-        valid_indices = (slice(0, samples_dim),) + self.valid_indices_
+        """
+        :param projected_data: array of shape (n_samples, n_modes)
+        :type projected_data: np.ndarray
+        :return: array of shape (n_samples, n_features)
+        :rtype: np.ndarray
+        """
 
-        reshaped_data[valid_indices] = data
+        n_modes_used = projected_data.shape[-1]
+        n_modes = self.singular_values.shape[0]
 
-        reshaped_data = super(MapValid, self).prepare_output_data(reshaped_data)
+        if n_modes_used < n_modes:
+            print(f"Truncating the number of modes from {n_modes} to {n_modes_used}")
 
-        return reshaped_data
+        if getattr(self, 'eig_norm', False) != False:
+            singular_values = self.singular_values[slice(0, n_modes_used)]
+            projected_data = (1/np.sqrt(singular_values)[None, :])*projected_data
+        else:
+            pass
 
-    def prepare_input_structured_data(self, data:np.recarray=None) -> np.ndarray:
+        '''
+               It is possible to reconstruct using less modes than
+               created during the ROM construction, so we will
+               adjust the size of self.modes according to projected_data
+        '''
 
-        """
+        if self.mean_component:
+            return projected_data.dot(self.modes[slice(0, n_modes_used)]) + self.data_mean
+        else:
+            return projected_data.dot(self.modes[slice(0, n_modes_used)])
 
-        :param data: structured array to be prepared, the default shape is
-        (n_samples, 1, *other_dimensions)
-        The features dimensions is 1 in NumPy structured arrays
-        :type data: np.ndarray
-        :return: np.ndarray
+    def save(self, save_path:str=None, model_name:str=None) -> None:
 
+        """It saves data in a NPZ file
+        :param save_path: path to save the model
+        :type save_path: str
+        :param model_name: name for the saved model
+        :type model_name: str
+        :return: nothing
         """
+        np.savez(os.path.join(save_path, model_name + '.npz'), self.modes, self.data_mean)
 
-        return self.prepare_input_data(data)
-
-    def prepare_output_structured_data(self, data:np.ndarray=None) -> np.ndarray:
+    def restore(self, save_path:str=None, model_name:str=None) -> None:
 
+        """It saves data in a NPZ file
+        :param save_path: path to save the model
+        :type save_path: str
+        :param model_name: name for the saved model
+        :type model_name: str
+        :return: nothing
         """
 
-        :param data: np.ndarray
-        :return: np.ndarray
+        self.modes, self.data_mean = np.load(os.path.join(save_path, model_name + '.npz'))
 
-        """
-        return self.prepare_output_data(data)
+class IPOD(ROM):
 
+    """Incremental Propor Orthogonal Decomposition
+    It executes the Incremental Proper Orthogonal Decomposition using the SciKit-learn interface
+    The IncrementalPCA class from SciKit-learn expects a two-dimensional array
+    as input, so it is necessary to reshape the input data before processing it.
+    This class is intended to be used for Big Data purposes.
+    """
 
-# Sampling (and, optionally, shuffling) datasets
-class Sampling(DataPreparer):
+    name = "ipod"
 
-    name = "sampling"
+    def __init__(self, config:dict=None, data_mean:np.ndarray=None, svd_filter:callable=None) -> None:
 
-    def __init__(self, choices_fraction:float=0.1, shuffling:bool=False) -> None:
+        """
+        :param config: configuration dictionary for the POD parameters
+        :type config: dict
+        :param data_mean: pre-evaluated mean of the dataset
+        :type data_mean: np.ndarray
+        :param svd_filter: a filter callable applied to SVD decomposition
+        :type svd_filter: callable
+        :return: nothing
+        """
 
         super().__init__()
 
-        self.choices_fraction = choices_fraction
-        self.shuffling = shuffling
-
-        self.global_indices = None
-        self.sampled_indices = None
-
-    @property
-    def indices(self) -> list:
-
-        assert self.sampled_indices is not None,\
-        "The indices still were not generate." \
-        "Run prepare_input_data or prepare_input_structured_data for getting them."
+        self.kind = "batchwise"
 
-        return sorted(self.sampled_indices.tolist())
+        if 'n_components' not in config:
+            config['n_components'] = None
 
-    def prepare_input_data(self, data:np.ndarray=None, data_interval:list=None) -> np.ndarray:
-
-        if data_interval is None:
-            data_interval = [0, data.shape[0]]
-        n_samples = data_interval[1] - data_interval[0]
-
-        self.global_indices = np.arange(start=data_interval[0], stop=data_interval[1])
-
-        n_choices = int(self.choices_fraction*n_samples)
+        if 'mean_component' in config:
+            self.mean_component = config.pop('mean_component')
+        else:
+            self.mean_component = True
 
-        self.sampled_indices = self.global_indices.copy()
-        if self.shuffling:
-            np.random.shuffle(self.sampled_indices)
+        if 'eig_norm' in config:
+            self.eig_norm = config.pop('eig_norm')
         else:
-            self.sampled_indices = self.sampled_indices
+            self.eig_norm = False
 
-        self.sampled_indices = np.random.choice(self.sampled_indices, n_choices)
+        self.pca = IncrementalPCA(**config)
 
-        return data[self.sampled_indices]
+        self.modes = None
 
-    def prepare_input_structured_data(self, data:h5py.Dataset=None, data_interval:list=None,
-                                            batch_size:int=None, dump_path:str=None) -> np.recarray:
+        self.data_mean = data_mean
 
-        """
-        :param data: structured array to be prepared, the default shape is
-        (n_samples, 1, *other_dimensions)
-        The features dimensions is 1 in NumPy structured arrays
-        :type data: np.ndarray
-        :return: np.ndarray
-        """
+        self.data_size = None
 
-        if data_interval is None:
-            data_interval = [0, data.shape[0]]
+        self.svd_filter = svd_filter
 
-        n_samples = data_interval[1] - data_interval[0]
-        self.global_indices = np.arange(start=data_interval[0], stop=data_interval[1])
+    def fit(self, data:np.ndarray=None) -> None:
 
-        n_sampled_preserved = int(self.choices_fraction*n_samples)
-        self.sampled_indices = np.random.choice(self.global_indices, n_sampled_preserved, replace=False)
-
-        if isinstance(data, h5py.Dataset):
+        """
+        Output shape: (space_dimension, n_modes)
 
-            if isinstance(batch_size, MemorySizeEval):
-                batch_size = batch_size(max_batches=n_sampled_preserved, shape=data.shape[1:])
+        :param data:
+        :type data: hdf5.File
+        """
+        if self.data_mean is None:
+            if not isinstance(self.data_mean, np.ndarray) and not self.data_size:
+                self.data_mean = data.mean(0)
+                self.data_size = data.shape[0]
             else:
-                pass
-
-            assert dump_path, "Using a h5py.Dataset as input data a dump_path must be provided."
-
-            fp = h5py.File(dump_path, 'w')
-            sampled_data = fp.create_dataset('data', shape=(n_sampled_preserved,) + data.shape[1:],
-                                             dtype=data.dtype)
-
-            # Constructing the normalization  using the reference data
-            batches = indices_batchdomain_constructor(indices=self.sampled_indices, batch_size=batch_size)
-
-            start_ix = 0
-            for batch_id, batch in enumerate(batches):
-                print(f"Sampling batch {batch_id+1}/{len(batches)} batch_size={len(batch)}")
-                finish_ix = start_ix + len(batch)
-                sampled_data[start_ix:finish_ix] = data[sorted(batch)]
-                start_ix = finish_ix
-
-            if self.shuffling:
-                random.shuffle(sampled_data)
+                self.data_mean = (self.data_size*self.data_mean +
+                                  data.shape[0]*data.mean(0))/(self.data_size + data.shape[0])
+                self.data_size += data.shape[0]
+        else:
+            assert len(self.data_mean.shape) == 1,\
+                f"The data_mean array must have dimension 1, but received shape {self.data_mean.shape}"
+
+        if self.mean_component:
+            data_til = data - self.data_mean
+        else:
+            data_til = data
+
+        decomp = self.pca.partial_fit(data_til)
+        self.modes = decomp.components_
+        self.singular_values = decomp.singular_values_
+
+        # Executing SVD filtering over the singular values if necessary
+        if self.svd_filter is not None:
+            self.singular_values_truncated = self.svd_filter.exec(singular_values=self.singular_values,
+                                                                  data_shape=data.shape)
+            n_values = len(self.singular_values_truncated)
+            self.singular_values = self.singular_values_truncated
+            self.modes = self.modes[:n_values, :]
 
         else:
-            raise Exception("Others cases are still not implemented.")
-
-        return sampled_data
-
-"""
-    END DataPreparer and its children
-"""
-
-"""
-    BEGIN Time-series data preparation (MovingWindow, SlidingWindow and BatchExtrapolation)
-"""
-
-class MovingWindow:
+            pass
 
-    """
+        relative_modal_energy = decomp.explained_variance_ratio_.sum()
 
-    MovingWindow is applied over a time-series array (2D array), and it is used for
-    creating the necessary augmented data used for LSTM networks, replicating the training
-    windows for each sample in the dataset.
-
-    See a graphical example:
-
-    batch n
-    ---------|---
-    history  | horizon
-
-        batch n+1
-        ---------|---
-        history  | horizon
-    ----
-    skip
+        print("Relative Modal Energy {}".format(relative_modal_energy))
 
-    """
+        self.relative_modal_energy = relative_modal_energy
 
-    def __init__(self, history_size:int=None, skip_size:int=1, horizon_size:int=None, full_output:bool=True) -> None:
+    def project(self, data:np.ndarray=None) -> np.ndarray:
 
         """
-
-        :param history_size: number of history samples
-        :type history_size: int
-        :param skip_size: number of samples to skip between two windows
-        :type skip_size: int
-        :param horizon_size: number of samples to use as prediction horizon
-        :type horizon_size: int
-
+        :param data: array of shape (n_samples, n_features)
+        :type data: np.ndarray
+        :return: array of shape (n_samples, n_modes) containing the projection over the POD basis
+        :rtype: np.ndarray
         """
 
-        self.history_size = history_size
-        self.skip_size = skip_size
-        self.horizon_size = horizon_size
-        self.full_output = full_output
-
-        if self.full_output == True:
-            self.process_batch = self.bypass
+        if self.mean_component:
+            data_til = data - self.data_mean
         else:
-            self.process_batch = self.get_last_item
-
-        # Verifying if history and horizon sizes was provided
-        assert history_size, f"A value for history_size must be provided, not {history_size}"
-        assert horizon_size, f"A value for horizon_size must be provided, not {horizon_size}"
-
-    def get_last_item(self, batch:np.ndarray) -> np.ndarray:
-
-        return batch[-1:]
+            data_til = data
 
-    def bypass(self, batch:np.ndarray) -> np.ndarray:
+        if not type(self.modes) == np.ndarray:
+            self.fit(data)
 
-        return batch
+        if self.eig_norm:
+            return np.sqrt(self.singular_values)[None, :] * (data_til.dot(self.modes.T))
+        else:
+            return data_til.dot(self.modes.T)
 
-    def __call__(self, input_data:np.ndarray=None, output_data:np.ndarray=None) -> (np.ndarray, np.ndarray):
+    def reconstruct(self, projected_data:np.ndarray=None) -> np.ndarray:
 
         """
-
-        :param input_data: 2D array (time-series) to be used for constructing the history size
-        :type input_data: np.ndarray
-        :param output_data:
-        :type output_data: np.ndarray
-        :return: (np.ndarray, np.ndarray) with shapes
-        (n_samples, n_history, n_features) and (n_samples, n_horizon, n_features)
-
+        :param projected_data: array of shape (n_samples, n_modes)
+        :type projected_data: np.ndarray
+        :return: array of shape (n_samples, n_features)
+        :rtype: np.ndarray
         """
 
-        # It is expected series_data to be a set of time-series with shape
-        # (n_timesteps, n_variables)
+        n_modes_used = projected_data.shape[-1]
 
-        input_batches_list = list()
-        output_batches_list = list()
-        data_size = input_data.shape[0]
+        if getattr(self, 'eig_norm', False) != False:
+            singular_values = self.singular_values[slice(0, n_modes_used)]
+            projected_data = (1 / np.sqrt(singular_values)[None, :]) * projected_data
+        else:
+            pass
 
-        assert input_data.shape[0] == output_data.shape[0]
+        '''
+            It is possible to reconstruct using less modes than
+            created during the ROM construction, so we will
+            adjust the size of self.modes according to projected_data
+        '''
 
-        center = self.history_size
+        if self.mean_component:
+            # We are using the approach of evaluating the mean value incrementally
+            # If this is the best way for doing it, just the experiments will demonstrate
+            return projected_data.dot(self.modes[slice(0, n_modes_used)]) + self.data_mean
+        else:
+            return projected_data.dot(self.modes[slice(0, n_modes_used)])
 
-        # Loop for covering the entire time-series dataset constructing the
-        # training windows
-        while center + self.horizon_size <= data_size:
+    def save(self, save_path:str=None, model_name:str=None) -> None:
 
-            input_batch = input_data[center - self.history_size:center, :]
-            output_batch = output_data[center:center + self.horizon_size, :]
+        """It saves data in a NPZ file
+       :param save_path: path to save the model
+       :type save_path: str
+       :param model_name: name for the saved model
+       :type model_name: str
+       :return: nothing
+       """
 
-            input_batches_list.append(input_batch)
-            output_batches_list.append(self.process_batch(batch=output_batch))
+        np.savez(os.path.join(save_path, model_name+'.npz'), self.modes, self.data_mean)
 
-            center += self.skip_size
+    def restore(self, save_path:str=None, model_name:str=None) -> None:
 
-        input_data = np.stack(input_batches_list, 0)
-        output_data = np.stack(output_batches_list, 0)
+        """It saves data in a NPZ file
+       :param save_path: path to save the model
+       :type save_path: str
+       :param model_name: name for the saved model
+       :type model_name: str
+       :return: nothing
+       """
 
-        return input_data, output_data
+        self.modes, self.data_mean = np.load(os.path.join(save_path, model_name + '.npz'))
 
-class SlidingWindow:
+class HOSVD(ROM):
 
+    """High-Order Singular Value Decomposition
+    It executes the High-Order SVD using a multidimensional array as input.
+    This class is intended to be used for Big Data purposes.
     """
 
-    SlidingWindow is applied over a time-series array (2D array), and it is used for
-    creating the necessary augmented data used for LSTM networks, replicating the training
-    windows for each sample in the dataset. The difference between SlidingWindow and MovingWindow
-    is that here there is no intersection between two sequential batches
-
-    See an graphical example:
-
-    batch n
-    ---------|---
-    history  | horizon
-
-                      batch n+1
-                      ---------|---
-                      history  | horizon
+    name = "hosvd"
 
-    """
-
-    def __init__(self, history_size:int=None, skip_size:int=None) -> None:
+    def __init__(self, n_components:List[int]=None, components_names:List[str]=None, engine:str='sklearn',
+                       limit:str='1 GiB') -> None:
 
         """
-
-        :param history_size: number of history samples
-        :type history_size: int
-        :param skip_size: number of samples to skip between two windows
-        :type skip_size: int
-
+        :param n_components: list with the number of components for each direction
+        :type n_components: List[int]
+        :return: nothing
         """
 
-        self.history_size = history_size
-        self.skip_size = skip_size
-
-        # Verifying if history and horizon sizes was provided
-        assert history_size, f"A value for history_size must be provided, not {history_size}"
-        assert skip_size, f"A value for horizon_size must be provided, not {skip_size}"
-
-    def __call__(self, input_data:np.ndarray=None, output_data:np.ndarray=None) -> (np.ndarray, np.ndarray):
-
-        """
+        super().__init__()
 
-        :param input_data: 2D array (time-series) to be used for constructing the history size
-        :type input_data: np.ndarray
-        :param output_data:
-        :type output_data: np.ndarray
-        :return: (np.ndarray, np.ndarray) with shapes
-        (n_samples, n_history, n_features) and (n_samples, n_horizon, n_features)
+        self.n_components = n_components
 
-        """
+        # Naming the components of the HOSVD decomposition
+        if components_names is None:
+            self.components_names = [f'component_{i}' for i in range(len(self.n_components))]
+        else:
+            assert len(components_names) == len(n_components), "The number of components must be equal" \
+                                                               " to the number of names."
+            self.components_names = components_names
 
-        # It is expected series_data to be a set of time-series with shape
-        # (n_timesteps, n_variables)
+        self.engine = engine
+        self.limit = limit
 
-        input_batches_list = list()
-        output_batches_list = list()
-        data_size = input_data.shape[0]
+        self.svd_classes = self._configure_SVD()
 
-        assert input_data.shape[0] == output_data.shape[0]
+        self.sizelist = None
+        self.shape = None
+        self.n_dims = None
+        self._comp_tag = '_decomp'
+        self.U_list = list()
+        self.S = None
 
-        center = self.history_size
+        self.k_svd = self._k_svd
 
-        # Loop for covering the entire time-series dataset constructing the
-        # training windows
-        while center + self.skip_size <= data_size:
+        if self.engine == 'sklearn':
+            self.lin = np
+        elif self.engine == 'dask':
+            self.lin = da
+        else:
+            raise Exception(f"The engine {self.engine} is not supported.")
 
-            input_batch = input_data[center - self.history_size:center, :]
-            output_batch = output_data[center - self.history_size + self.skip_size:
-                                       center+self.skip_size, :]
+    def _configure_SVD(self) -> Union[List[TruncatedSVD], List[ParallelSVD]]:
 
-            input_batches_list.append(input_batch)
-            output_batches_list.append(output_batch)
+        if self.engine == 'sklearn':
+            return [TruncatedSVD(n_components=n) for n in self.n_components]
+        elif self.engine == 'dask':
+            return [ParallelSVD(n_components=n) for n in self.n_components]
+        else:
+            raise Exception(f"The engine {self.engine} is not supported, it must be in ['sklearn', 'dask'].")
 
-            center += self.skip_size
+    def _set_components(self) -> None:
 
-        input_data = np.stack(input_batches_list, 0)
-        output_data = np.stack(output_batches_list, 0)
+        for j, name in enumerate(self.components_names):
 
-        return input_data, output_data
+            setattr(self, name.upper() + self._comp_tag, self.U_list[j])
 
-class IntersectingBatches:
+    def _k_svd(self, data:np.ndarray=None, k:int=None) -> Union[np.ndarray, da.core.Array]:
 
-    """
+        """SVD applied to the k-mode flattening
+        :param projected_data: array of shape (n_samples, n_features)
+        :type projected_data: np.ndarray
+        :return: Left eigenvectors matrix U
+        :rtype: np.ndarray
+        """
 
-    IntersectingBatches is applied over a time-series array (2D array).
+        self.svd_classes[k].fit(data)
 
-    See a graphical example:
+        if self.engine == 'sklearn':
+            s = self.svd_classes[k].singular_values_ * np.eye(self.n_components[k])
+            VT = self.svd_classes[k].components_
+            SVT = s @ VT
+            U = (np.linalg.pinv(SVT.T) @ data.T).T
 
-    batch n
-    |------------|
-        batch n+1
-        |------------|
-    ----
-    skip
+        else:
+            U = getattr(self.svd_classes[k], 'U')
 
-    """
+        return U
 
-    def __init__(self, skip_size:int=1, batch_size:int=None, full:bool=True) -> None:
+    def _k_flattening(self, data:Union[np.ndarray, da.core.Array]=None, k:int=None) -> Union[np.ndarray, da.core.Array]:
 
+        """k-mode flattening
+        :param projected_data: array of shape (n_1, n_2, ..., n_n)
+        :type projected_data: np.ndarray
+        :return: reshaped array of shape (n_1, n_2*n_3*...*n_n)
+        :rtype: np.ndarray
         """
 
-        :param skip_size: number of samples to skip between two windows
-        :type skip_size: int
-        :param batch_size: number of samples to use in each batch
-        :type batch_size: int
+        sizelist = copy.deepcopy(self.sizelist)
+        sizelist_collapsible = copy.deepcopy(sizelist)
 
-        """
+        sizelist[0] = k
+        sizelist[k] = 0
 
-        # Verifying if history and horizon sizes was provided
-        assert batch_size, f"A value for horizon_size must be provided, not {batch_size}"
+        sizelist_collapsible.pop(k)
+        collapsible_dims = np.prod([self.shape[s] for s in sizelist_collapsible])
 
-        self.skip_size = skip_size
-        self.batch_size = batch_size
-        self.full = full
+        if isinstance(data, da.core.Array):
+            return data.transpose(sizelist).reshape((-1, collapsible_dims), limit=self.limit)
+        else:
+            return data.transpose(sizelist).reshape(-1, collapsible_dims)
 
-    def get_indices(self, dim:int=None) -> np.ndarray:
+    def fit(self, data:Union[np.ndarray, da.core.Array]=None) -> None:
 
+        """Executing High-Order SVD
+        :param data: input array of shape (n_1, n_2, ..., n_n)
+        :type data: np.ndarray
+        :return: nothing
         """
+        import pprint
+        pprinter = pprint.PrettyPrinter(indent=2)
 
-        It gets just the indices of the shifting
+        self.n_dims = len(data.shape)
+        self.shape = data.shape
+        S = data
 
-        :param dim: total dimension
-        :type dim: int
-        :return: the shifted indices
-        :rtype: np.ndarray
+        self.sizelist = np.arange(self.n_dims).tolist()
 
-        """
+        print("Using the SVD classes:\n")
+        pprinter.pprint(self.svd_classes)
+        print('\n')
 
-        center = 0
-        indices = list()
-        indices_m = list()
+        for k in range(self.n_dims):
 
-        # Loop for covering the entire time-series dataset constructing the
-        # training windows
-        while center + self.batch_size < dim:
+            print(f"Executing SVD for the dimension {k}")
 
-            index = center + self.batch_size
+            data_k_flatten = self._k_flattening(data=data, k=k)
+            U = self.k_svd(data=data_k_flatten, k=k)
 
-            indices.append(center)
-            indices_m.append(index)
+            self.U_list.append(U)
 
-            center += self.skip_size
+            S = self.lin.tensordot(S, U, axes=([0],[0]))
 
-        return np.array(indices), np.array(indices_m)
+        self.S = np.array(S)
 
-    def __call__(self, input_data:np.ndarray=None) -> Union[list, np.ndarray]:
+        self._set_components()
 
-        """
-
-        :param input_data: 2D array (time-series) to be used for constructing the history size
-        :type input_data: np.ndarray
-        :param output_data:
-        :type output_data: np.ndarray
-        :return: (np.ndarray, np.ndarray) with shapes
-        (n_samples, n_history, n_features) and (n_samples, n_horizon, n_features)
+    def project(self, data:Union[np.ndarray, da.core.Array]=None) -> Union[np.ndarray, da.core.Array]:
 
+        """Projecting using the SVD basis
+        :param data: input array of shape (n_1, n_2, ..., n_n)
+        :type data: np.ndarray
+        :return: reduced array of shape (n_1', n_2', ..., n_n')
+        :rtype: np.ndarray
         """
 
-        # It is expected series_data to be a set of time-series with shape
-        # (n_timesteps, n_variables)
-
-        input_batches_list = list()
+        assert len(data.shape) == self.n_dims
+        S = data
 
-        data_size = input_data.shape[0]
+        for k in range(self.n_dims):
 
-        center = 0
+            S = np.tensordot(S, self.U_list[k], axes=([0], [0]))
 
-        # Loop for covering the entire time-series dataset constructing the
-        # training windows
-        while center + self.batch_size <= data_size:
+        return S
 
-            input_batch = input_data[center:center + self.batch_size]
+    def reconstruct(self, data:Union[np.ndarray, da.core.Array]=None,
+                          replace_components:dict=None) -> Union[np.ndarray, da.core.Array]:
 
-            input_batches_list.append(input_batch)
-
-            center += self.skip_size
+        """Reconstruction using the pre-existent basis
+        :param data: reduced array of shape (n_1', n_2', ..., n_n')
+        :type data: np.ndarray
+        :return: reconstructed array of shape (n_1, n_2, n_3,..., n_n)
+        :rtype: np.ndarray
+        """
 
-        if self.full == True:
-            return input_batches_list
-        else:
-            return np.vstack([item[-1] for item in input_batches_list])
+        if replace_components is not None:
+            U_list = copy.deepcopy(self.U_list)
 
+            for key, value in replace_components.items():
 
-class BatchwiseExtrapolation:
+                try:
+                    index = self.components_names.index(key)
+                except:
+                    raise Exception(f"The key {key} is not in the list of components.")
 
-    """
+                U_list[index] = value
+        else:
+            U_list = self.U_list
 
-    BatchwiseExtraplation uses a time-series regression model and inputs as generated by
-    MovingWindow to continuously extrapolate a dataset
+        A = data
+        modes = np.arange(self.n_dims).tolist()
 
-    """
+        for k in modes:
 
-    def __init__(self, op:callable=None, auxiliary_data:np.ndarray=None) -> None:
+            A = np.tensordot(U_list[k], A, axes=([1], [k]))
 
-        self.op = op
-        self.auxiliary_data = auxiliary_data
-        self.time_id = 0
+        return A.transpose()
 
-    def _simple_extrapolation(self, extrapolation_dataset:np.ndarray, history_size:int=0) -> np.ndarray:
+        # Saving to disk the complete model
+    def save(self, save_path: str = None, model_name: str = None) -> None:
 
-        return extrapolation_dataset[None, -history_size:, :]
+        """Complete saving
 
-    def _forcing_extrapolation(self, extrapolation_dataset:np.ndarray, history_size:int=0) -> np.ndarray:
+        :param save_path: path to the saving directory
+        :type: str
+        :param model_name: name for the model
+        :type model_name: str
+        :return: nothing
+        """
+        blacklist = ['lin']
+        for el in blacklist:
+            setattr(self, el, None)
 
-        return np.hstack([extrapolation_dataset[-history_size:, :],
-                          self.auxiliary_data[self.time_id-history_size:self.time_id, :]])[None, :, :]
+        path = os.path.join(save_path, model_name + '.pkl')
+        try:
+            with open(path, 'wb') as fp:
+                pickle.dump(self, fp, protocol=4)
+        except Exception as e:
+            print(e, e.args)
 
-    def __call__(self, init_state:np.ndarray=None, history_size:int=None, horizon_size:int=None,
-                       testing_data_size:int=None) -> np.ndarray:
 
-        if isinstance(self.auxiliary_data, np.ndarray):
-            n_series = self.auxiliary_data.shape[-1]
-        else:
-            n_series = 0
+class DMD(ROM):
 
-        current_state = init_state
-        extrapolation_dataset = init_state[0, :, n_series:]
-        self.time_id = history_size
+    def __init__(self, config=None):
 
-        if isinstance(self.auxiliary_data, np.ndarray):
+        """
+        Parameters
+        ----------
+        config
+        """
+        super().__init__()
+        for key, value in config.items():
+            setattr(self, key, value)
 
-            assert self.auxiliary_data.shape[-1] + n_series == init_state.shape[-1], \
-                   "Number of series in the initial state must be {}".format(self.auxiliary_data.shape[-1])
+        self.Lambda = None
+        self.Phi = None
+        self.A_tilde = None
+        self.initial_state = None
 
-            current_state_constructor = self._forcing_extrapolation
+    '''The method fit from DMD receives an array with shape (nt, np.product(*dims))
+       and constructs a model for estimating the state nt+1
+    '''
+    def fit(self, data=None):
 
-        else:
+        data = data.T
 
-            current_state_constructor = self._simple_extrapolation
+        X_aug = np.vstack((data[:, 0:-2], data[:, 1:-1]))
+        X_aug_tilde = np.vstack((data[:, 1:-1], data[:, 2:]))
 
-        while extrapolation_dataset.shape[0] - history_size + horizon_size <= testing_data_size:
+        U, Sig, VT = np.linalg.svd(X_aug, full_matrices=False)
+        A_tilde = U.T @ X_aug_tilde @ VT.T @ np.linalg.inv(np.diag(Sig))
 
-            extrapolation = self.op(current_state)
-            extrapolation_dataset = np.concatenate([extrapolation_dataset, extrapolation[0]], 0)
-            current_state = current_state_constructor(extrapolation_dataset,
-                                                      history_size=history_size)
+        self.A_tilde = A_tilde
 
-            log_str = "Extrapolation {}".format(self.time_id + 1 - history_size)
-            sys.stdout.write("\r" + log_str)
-            sys.stdout.flush()
+        Lambda, W = np.linalg.eig(A_tilde)
 
-            self.time_id += horizon_size
+        self.Lambda = Lambda
 
-        extrapolation_dataset = extrapolation_dataset[history_size:, :]
+        Phi = X_aug_tilde @ VT.T @ np.linalg.inv(np.diag(Sig)) @ W
 
-        return extrapolation_dataset
+        self.Phi = Phi
 
-"""
-    END Time-series data preparation (MovingWindow, SlidingWindow and BatchExtrapolation)
-"""
+        initial_state = np.linalg.inv(Phi.conj().T @ Phi) @ Phi.conj().T @ X_aug_tilde[:, -1]
 
-class BatchCopy:
+        self.initial_state = initial_state
 
-    def __init__(self, channels_last:bool=False) -> None:
+        print('Fitting process concluded.')
 
-        self.channels_last = channels_last
+    def predict(self, step=None):
 
-    def _single_copy(self, data:h5py.Dataset=None, data_interval:list=None,
-                           batch_size:int=None, dump_path:str=None,
-                           transformation:callable=lambda data: data) -> h5py.Dataset:
+        return self.Phi @ np.diag(self.Lambda**(step-1)) @ self.initial_state
 
-        assert isinstance(data, h5py.Dataset), "The input must be h5py.Dataset"
+# Gappy POD
+class GPOD(ROM):
 
-        variables_list = data.dtype.names
-        data_shape = (data_interval[1] - data_interval[0],) + data.shape[1:]
+    def __init__(self, pca_type='pod', pca_config=None, config=None):
 
-        data_file = h5py.File(dump_path, "w")
-        dtype = [(var, '<f8') for var in variables_list]
+        """GPOD
+        :param pca_type: the kind of PCA to be used
+        :type pca_type: str
 
-        dset = data_file.create_dataset("data", shape=data_shape,
-                                        dtype=dtype)
+        """
+        super().__init__()
 
-        if isinstance(batch_size, MemorySizeEval):
-            n_samples = data_interval[1] - data_interval[0]
-            batch_size = batch_size(max_batches=n_samples, shape=data.shape[1:])
-        else:
-            pass
+        this_module = importlib.import_module('simulai.rom')
 
-        # Constructing the normalization  using the reference data
-        batches = batchdomain_constructor(data_interval, batch_size)
-        dset_batches = batchdomain_constructor([0, dset.shape[0]], batch_size)
+        # A PCA instance is used for constructing the basis
+        self.pca_type = pca_type
+        self.config = config
+
+        self.sensors_distribution = None
+        self.n_sensors = None
+        self.sensors_placer = None
 
-        variables_names = data.dtype.names
+        for key, value in config.items():
+            setattr(self, key, value)
 
-        n_variables = len(data.dtype.names)
+        assert self.sensors_distribution, "sensors_distribution must be provided"
 
-        for batch_id, (batch, d_batch) in enumerate(zip(batches, dset_batches)):
+        if not self.sensors_placer or self.sensors_placer != 'extrema':
+            print("As no placement criteria eas provided for the sensor, the extrema method will be used.")
+            self.sensors_placer = 'extrema'
+        else:
+            raise Exception(f"The placement method {self.sensors_placer} is not supported.")
 
-            print(f"Copying batch {batch_id+1}/{len(batches)} batch_size={batch[1]-batch[0]}")
 
-            # The variables dimension is the last one
-            if self.channels_last:
-                # TODO this is a restrictive way of doing it. It must be more flexible.
-                chunk_data = data[slice(*batch)].view((float, len(data.dtype.names)))#.transpose((0, 4, 2, 3, 1))
-            # The variables dimension is the second one
-            else:
-                chunk_data = data[slice(*batch)].view((float, len(data.dtype.names)))
+        if self.sensors_placer == 'extrema':
 
-            chunk_data = np.core.records.fromarrays(np.split(chunk_data[...], n_variables, axis=-1),
-                                                               names=variables_names,
-                                                               formats=','.join(len(variables_names) * ['f8']))
+            assert all([not item%2 for item in self.sensors_distribution]),\
+                "If extrema placement is being used, all the number of sensors must be pair"
 
-            if len(chunk_data.shape) > len(dset.shape):
-                chunk_data = np.squeeze(chunk_data, axis=-1)
-            else:
-                pass
+        self.placer = getattr(self, '_' + self.sensors_placer)
 
-            dset[slice(*d_batch)] = transformation(chunk_data[...])
+        self.n_sensors = sum(self.sensors_distribution)
 
-        return dset
+        self.pca_class = getattr(this_module, self.pca_type.upper())
 
-    def _multiple_copy(self, data:list=None, data_interval:list=None,
-                             batch_size:int=None, dump_path:str=None,
-                             transformation:callable=lambda data: data) -> h5py.Dataset:
+        self.pca = self.pca_class(config=pca_config)
 
-        assert all([isinstance(di, h5py.Dataset) for di in data]), "All inputs must be h5py.Dataset"
+        self.modes = None
+        self.M = None
+        self.M_inv = None
+        self.mask_array = None
 
-        variables_list = sum([list(di.dtype.names) for di in data], [])
-        data_shape = (data_interval[1] - data_interval[0],) + data[0].shape[1:]
+    # It gets the positions related to the n maximum and n minimum values to be used
+    # to locate sensors
+    def _extrema(self):
 
-        data_file = h5py.File(dump_path, "w")
-        dtype = [(var, '<f8') for var in variables_list]
+        locations = list()
+        n_modes = self.modes.shape[0]
 
-        dset = data_file.create_dataset("data", shape=data_shape,
-                                        dtype=dtype)
+        for mode_i in range(n_modes):
 
-        if isinstance(batch_size, MemorySizeEval):
-            n_samples = data_interval[1] - data_interval[0]
-            batch_size = batch_size(max_batches=n_samples, shape=data.shape[1:])
-        else:
-            pass
+            n_sensors = self.sensors_distribution[mode_i]
+            n_minimum = n_maximum = int(n_sensors/2)
 
-        # Constructing the normalization  using the reference data
-        batches = batchdomain_constructor(data_interval, batch_size)
-        dset_batches = batchdomain_constructor([0, dset.shape[0]], batch_size)
+            locations += self.modes[mode_i].argsort()[:n_minimum].tolist()
+            locations += self.modes[mode_i].argsort()[-n_maximum:].tolist()
 
-        variables_names = sum([list(di.dtype.names) for di in data], [])
+        return locations
 
-        n_variables = sum([len(di.dtype.names) for di in data])
+    # The m dot product (a, b)_m = (m*a, m*b), in which m is a mask array
+    def m_dot(self, a, b, mask_array=None):
 
-        for batch_id, (batch, d_batch) in enumerate(zip(batches, dset_batches)):
+        return (mask_array*a).dot((mask_array*b).T)
 
-            print(f"Copying and concatenating the batches {batch_id+1}/{len(batches)} batch_size={batch[1] - batch[0]}")
+    def fit(self, data=None):
 
-            # The variables dimension is the last one
-            if self.channels_last:
-                # TODO this is a restrictive way of doing it. It must be more flexible.
-                chunk_data = np.stack([di[slice(*batch)].view((float, len(di.dtype.names))).transpose((0, 4, 2, 3, 1))
-                                       for di in data], axis=-1)
-            # The variables dimension is the second one
-            else:
-                chunk_data = np.stack([di[slice(*batch)].view((float, len(di.dtype.names))) for di in data], axis=-1)
+        self.pca.fit(data=data)
+        self.modes = self.pca.modes
 
-            chunk_data = np.core.records.fromarrays(np.split(chunk_data[...], n_variables, axis=-1),
-                                                    names=variables_names,
-                                                    formats=','.join(len(variables_names) * ['f8']))
+        n_features = self.modes.shape[1]
 
-            if len(chunk_data.shape) > len(dset.shape):
-                chunk_data = np.squeeze(chunk_data, axis=-1)
-            else:
-                pass
+        sensors_locations = self.placer()
 
-            dset[slice(*d_batch)] = transformation(chunk_data[...])
+        mask_array = np.zeros((1, n_features))
+        mask_array[:, sensors_locations] = 1
 
-        return dset
+        self.mask_array = mask_array
+        self.M = self.m_dot(self.modes, self.modes, mask_array=mask_array)
+        self.M_inv = np.linalg.inv(self.M)
 
-    def copy(self, data:h5py.Dataset=None, data_interval:list=None,
-                   batch_size:int=None, dump_path:str=None,
-                   transformation:callable=lambda data: data) -> h5py.Dataset:
+        print(f'The condition number for the matrix M is {np.linalg.cond(self.M)}')
 
-        if isinstance(data, list):
+    def project(self, data=None):
 
-            return self._multiple_copy(data=data, data_interval=data_interval, batch_size=batch_size,
-                                       dump_path=dump_path, transformation=transformation)
+        data_til = self.mask_array * data
+        f = self.m_dot(data_til, self.modes, mask_array=self.mask_array)
 
-        else:
-            return self._single_copy(data=data, data_interval=data_interval, batch_size=batch_size,
-                                       dump_path=dump_path, transformation=transformation)
+        return f @ self.M_inv.T
 
-class MakeTensor:
+    def reconstruct(self, projected_data=None):
 
-    def __init__(self, input_names=None, output_names=None):
+        return self.pca.reconstruct(projected_data=projected_data)
 
-        self.input_names = input_names
-        self.output_names = output_names
+# Quasi-Quadratic Manifold
+class QQM:
 
-    def _make_tensor(self, input_data:np.ndarray=None, device:str='cpu') -> List[torch.Tensor]:
+    def __init__(self, n_inputs:int=None, alpha_0:float=None, sparsity_tol:float=1e-15,
+                       lambd:float=None, epsilon:float=1e-10, use_mean:bool=False) -> None:
 
-        inputs_list = list(torch.split(input_data, 1, dim=-1))
+        """It extends and enriches the POD approach by determining a quadratic basis for its residual
+        :param n_inputs: number of inputs used in the POD approximation
+        :type n_inputs:int
+        :param alpha_0: regularization parameter used in SparSA algorithm
+        :type alpha_0: float
+        :param sparsity_tol: sparsity tolerance used in SpaRSA
+        :type sparsity_tol: float
+        :param lambd: regularization parameter used in SparSA algorithm
+        :type lambd: float
+        :param epsilon: threshold for zeroing columns in SpaRSA
+        :type epsilon: float
+        :param use_mean: use mean for the SpaRSA loss function of not ?
+        :type use_mean: bool
+        :returns: nothing
+        """
 
-        for vv, var in enumerate(inputs_list):
+        self.alpha_0 = alpha_0
+        self.lambd = lambd
+        self.epsilon = epsilon
+        self.n_inputs = n_inputs
+        self.i_u, self.j_u = np.triu_indices(self.n_inputs)
+        self.V_bar = None
+        self.valid_indices = None
 
-            var.requires_grad = True
-            var = var.to(device)
-            inputs_list[vv] = var
-            #var = var[..., None]
+        self.optimizer = SpaRSA(lambd=self.lambd, alpha_0=alpha_0, use_mean=use_mean, sparsity_tol=sparsity_tol,
+                                epsilon=epsilon, transform=self.W_transform)
 
-        return inputs_list
+    def _kronecker_product(self, a:np.ndarray=None, b:np.ndarray=None) -> np.ndarray:
 
-    def _make_tensor_dict(self, input_data:dict=None, device:str='cpu') -> dict:
+        """It executes a Kronecker dot between two arrays
+        :param a: left array
+        :type a: np.ndarray
+        :param b: right (transposed) array
+        :type b: np.ndarray
+        :returns: the Kronecker output array
+        :rtype: np.ndarray
+        """
 
-        inputs_dict = dict()
+        assert a.shape == b.shape, f"a and b must have the same shape, but received {a.shape} and {b.shape}"
 
-        for key, item in input_data.items():
+        kron_output = np.einsum('bi, bj->bij', a, b)
 
-            item.requires_grad = True
-            item = item.to(device)
-            inputs_dict[key] = item
+        assert np.isnan(kron_output).max() == False, "There are NaN in the Kronecker output"
 
-        return inputs_dict
+        # Checking if the Kronecker output tensor is symmetric or not
+        if np.array_equal(kron_output, kron_output.transpose(0,2,1)):
+            return kron_output[:, self.i_u, self.j_u]
+        else:
+            shapes = kron_output.shape[1:]
+            return kron_output.reshape(-1, np.prod(shapes))
 
-    def __call__(self, input_data:Union[np.ndarray, torch.Tensor,
-                                        Dict[str, np.ndarray]]=None,
-                                         device:str='cpu') -> List[torch.Tensor]:
+    # Each batch in W has n_inputs*(n_inputs + 1)/2 columns
+    def W_transform(self, data:np.ndarray=None) -> np.ndarray:
 
-        if type(input_data) == np.ndarray:
+        """W_transform simply applied Kronecker product for data itself
+        :param data: the data to be W-transformed
+        :type: np.ndarray
+        :returns: the Kronecker product between data and data itself
+        :rtype: np.ndarray
+        """
 
-            input_data = torch.from_numpy(input_data.astype(np.float32))
+        return self._kronecker_product(a=data, b=data)
 
-            inputs_list = self._make_tensor(input_data=input_data, device=device)
+    def fit(self, input_data:np.ndarray=None, target_data:np.ndarray=None, pinv:bool=False) -> None:
 
-            return inputs_list
+        """It executes the fitting process using the chosen optimization algorithm, SpaRSA
+         or Moore-Penrose pseudoinverse
 
-        if type(input_data) == torch.Tensor:
+        :param input_data: in general, the original latent series
+        :type input_data: np.ndarray
+        :param target_data: in general, the residual of the linear approximation
+        :type target_data: np.ndarray
+        :param pinv: use pseudoinverse or not
+        :type pinv: bool
+        :returns: nothing
+        """
 
-            inputs_list = self._make_tensor(input_data=input_data, device=device)
+        if not pinv:
+            self.V_bar = self.optimizer.fit(input_data=input_data, target_data=target_data)
+        else:
+           V_bar = np.linalg.pinv(self.W_transform(data=input_data)) @ target_data
+           self.V_bar = np.where(np.abs(V_bar) < self.optimizer.sparsity_tol, 0, V_bar)
 
-            return inputs_list
+        self.valid_indices = np.argwhere(np.sum(np.abs(self.V_bar), axis=1) > 0).flatten()
 
-        elif type(input_data) == dict:
+        print(f"\n Number of original modes: {self.i_u.size}. Number of modes selected: {self.valid_indices.size}")
 
-            inputs_list = self._make_tensor_dict(input_data=input_data, device=device)
+    def project(self, data:np.ndarray=None) -> np.ndarray:
 
-            return inputs_list
+        """Executes the W-transformation and collects just the valid modes determined
+         by the optimization algorithm
 
-        else:
-            raise Exception(f"The type {type(input_data)} for input_data is not supported.")
+        :param data: the data to be projected
+        :type: np.ndarray
+        :returns: the projection over the selected basis
+        :rtype: np.ndarray
+        """
 
-class GaussianNoise(Dataset):
+        return  self.W_transform(data=data)[:, self.valid_indices]
 
-    def __init__(self, stddev:float=0.01, input_data:Union[np.ndarray, Tensor]=None):
+    def eval(self, data:np.ndarray=None) -> None:
 
-        super(Dataset, self).__init__()
+        """It projects and reconstructs
 
-        self.stddev = stddev
+        :param data: the data to be projected
+        :type: np.ndarray
+        :returns: the approximated data
+        :rtype: np.ndarray
+        """
 
-        if isinstance(input_data, np.ndarray):
-            input_data_ = torch.from_numpy(input_data.astype("float32"))
-        else:
-            input_data_ = input_data
+        return self.W_transform(data=data) @ self.V_bar
 
-        self.input_data = input_data_
+    def save(self, save_path: str = None, model_name: str = None) -> None:
 
-        self.data_shape = tuple(self.input_data.shape)
+        """Complete saving
 
-    def size(self):
+        :param save_path: path to the saving directory
+        :type: str
+        :param model_name: name for the model
+        :type model_name: str
+        :return: nothing
+        """
 
-        return self.data_shape
+        blacklist = ['optimizer']
+        for el in blacklist:
+            setattr(self, el, None)
 
-    def __call__(self):
+        path = os.path.join(save_path, model_name + '.pkl')
+        try:
+            with open(path, 'wb') as fp:
+                pickle.dump(self, fp, protocol=4)
+        except Exception as e:
+            print(e, e.args)
 
-        return (1 + self.stddev*torch.randn(*self.data_shape))*self.input_data
```

### Comparing `simulai-toolkit-0.99.8/simulai_toolkit.egg-info/PKG-INFO` & `simulai-toolkit-0.99.9/simulai/simulai_toolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simulai-toolkit
-Version: 0.99.8
+Version: 0.99.9
 Summary: A Python package with data-driven pipelines for physics-informed machine learning
 License: Apache License, Version 2.0
 Project-URL: Source, https://github.com/IBM/simulai
 Project-URL: Tracker, https://github.com/IBM/simulai/issues
 Project-URL: Documentation, https://simulai-toolkit.readthedocs.io
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `simulai-toolkit-0.99.8/tests/devices/test_network_devices.py` & `simulai-toolkit-0.99.9/tests/devices/test_network_devices.py`

 * *Files identical despite different names*

### Comparing `simulai-toolkit-0.99.8/tests/math/test_LSODA.py` & `simulai-toolkit-0.99.9/tests/math/test_LSODA.py`

 * *Files identical despite different names*

### Comparing `simulai-toolkit-0.99.8/tests/math/test_RK4.py` & `simulai-toolkit-0.99.9/tests/math/test_RK4.py`

 * *Files identical despite different names*

### Comparing `simulai-toolkit-0.99.8/tests/math/test_collocation_derivative.py` & `simulai-toolkit-0.99.9/tests/math/test_collocation_derivative.py`

 * *Files identical despite different names*

### Comparing `simulai-toolkit-0.99.8/tests/math/test_metrics.py` & `simulai-toolkit-0.99.9/tests/math/test_metrics.py`

 * *Files identical despite different names*

### Comparing `simulai-toolkit-0.99.8/tests/math/test_products.py` & `simulai-toolkit-0.99.9/tests/math/test_products.py`

 * *Files identical despite different names*

### Comparing `simulai-toolkit-0.99.8/tests/metrics/test_mahalanobis.py` & `simulai-toolkit-0.99.9/tests/metrics/test_mahalanobis.py`

 * *Files identical despite different names*

### Comparing `simulai-toolkit-0.99.8/tests/network/test_conv_1d.py` & `simulai-toolkit-0.99.9/tests/network/test_conv_1d.py`

 * *Files identical despite different names*

### Comparing `simulai-toolkit-0.99.8/tests/network/test_conv_2d.py` & `simulai-toolkit-0.99.9/tests/network/test_conv_2d.py`

 * *Files identical despite different names*

### Comparing `simulai-toolkit-0.99.8/tests/network/test_deeponet.py` & `simulai-toolkit-0.99.9/tests/network/test_deeponet.py`

 * *Files identical despite different names*

### Comparing `simulai-toolkit-0.99.8/tests/network/test_dense.py` & `simulai-toolkit-0.99.9/tests/network/test_dense.py`

 * *Files identical despite different names*

### Comparing `simulai-toolkit-0.99.8/tests/network/test_elm.py` & `simulai-toolkit-0.99.9/tests/network/test_elm.py`

 * *Files identical despite different names*

### Comparing `simulai-toolkit-0.99.8/tests/network/test_flexible_deeponet.py` & `simulai-toolkit-0.99.9/tests/network/test_flexible_deeponet.py`

 * *Files identical despite different names*

### Comparing `simulai-toolkit-0.99.8/tests/network/test_improved_deeponet.py` & `simulai-toolkit-0.99.9/tests/network/test_improved_deeponet.py`

 * *Files identical despite different names*

### Comparing `simulai-toolkit-0.99.8/tests/opinf/test_extended_opinf_operators_construction.py` & `simulai-toolkit-0.99.9/tests/opinf/test_extended_opinf_operators_construction.py`

 * *Files identical despite different names*

### Comparing `simulai-toolkit-0.99.8/tests/opinf/test_opinf_operators_construction.py` & `simulai-toolkit-0.99.9/tests/opinf/test_opinf_operators_construction.py`

 * *Files identical despite different names*

### Comparing `simulai-toolkit-0.99.8/tests/parallelism/test_modelpool_affinemapping.py` & `simulai-toolkit-0.99.9/tests/parallelism/test_modelpool_affinemapping.py`

 * *Files identical despite different names*

### Comparing `simulai-toolkit-0.99.8/tests/parallelism/test_modelpool_esn.py` & `simulai-toolkit-0.99.9/tests/parallelism/test_modelpool_esn.py`

 * *Files 2% similar despite different names*

```diff
@@ -249,15 +249,16 @@
                 'skip_size': 1
             }
         """
         pool_config = {'template': 'independent_series'}
 
         self.test_case = "independent_series_single_fit"
 
-        self._run_ESN(rc_config, pool_config=pool_config)
+        for model_type in ['EchoStateNetwork', 'DeepEchoStateNetwork', 'WideEchoStateNetwork']:
+            self._run_ESN(rc_config, pool_config=pool_config, model_type=model_type)
 
     ''' Maybe this test is no more useful
     def test_modelpool_ESN_no_parallelism(self):
 
         # Configuration of the sub-networks (in this case, ESN-RC)
         rc_config = {
             'reservoir_dim': 250,
@@ -341,15 +342,15 @@
         field_test_data = Z_field[N_train:, :]
 
         forcings_train_data = Z_forcings[:N_train, :]
         forcings_test_data = Z_forcings[N_train:, :]
 
         return field_train_data, forcings_train_data, field_test_data, forcings_test_data
 
-    def _run_ESN(self, rc_config, pool_config=None, fit=True, model=None, output=False):
+    def _run_ESN(self, rc_config, pool_config=None, fit=True, model=None, model_type:str='EchoStateNetwork', output=False):
 
         field_train_data, forcings_train_data, field_test_data, forcings_test_data = self.get_manufactured_dataset()
 
         input_data = field_train_data[:-1]
         auxiliary_data = forcings_train_data[:-1]
         target_data = field_train_data[1:]
 
@@ -372,15 +373,15 @@
         pool_config['n_outputs'] = n_fields
         pool_config['n_auxiliary'] = n_forcings
         # The dictionary pool_config could be directly declared, but it is done in stages given the
         # characteristics of the function _run_ESN, which is used in multiple different cases
 
         if fit and model is None:
 
-            pool = ModelPool(config=pool_config, model_type='EchoStateNetwork',
+            pool = ModelPool(config=pool_config, model_type=model_type,
                              model_config=rc_config)
 
             if self.test_case is not "independent_series_multi_fit":
                 pool.fit(input_data=input_data, target_data=target_data,
                          auxiliary_data=auxiliary_data)
             else:
                 for group_index in range(n_fields):
```

### Comparing `simulai-toolkit-0.99.8/tests/postprocessing/test_batchwise_extrapolation.py` & `simulai-toolkit-0.99.9/tests/postprocessing/test_batchwise_extrapolation.py`

 * *Files identical despite different names*

### Comparing `simulai-toolkit-0.99.8/tests/preprocessing/test_batch_copy.py` & `simulai-toolkit-0.99.9/tests/preprocessing/test_batch_copy.py`

 * *Files identical despite different names*

### Comparing `simulai-toolkit-0.99.8/tests/preprocessing/test_batching.py` & `simulai-toolkit-0.99.9/tests/preprocessing/test_batching.py`

 * *Files identical despite different names*

### Comparing `simulai-toolkit-0.99.8/tests/preprocessing/test_mapvalid.py` & `simulai-toolkit-0.99.9/tests/preprocessing/test_mapvalid.py`

 * *Files identical despite different names*

### Comparing `simulai-toolkit-0.99.8/tests/preprocessing/test_meanevaluation.py` & `simulai-toolkit-0.99.9/tests/preprocessing/test_meanevaluation.py`

 * *Files identical despite different names*

### Comparing `simulai-toolkit-0.99.8/tests/preprocessing/test_minmax.py` & `simulai-toolkit-0.99.9/tests/preprocessing/test_minmax.py`

 * *Files identical despite different names*

### Comparing `simulai-toolkit-0.99.8/tests/preprocessing/test_moving_window.py` & `simulai-toolkit-0.99.9/tests/preprocessing/test_moving_window.py`

 * *Files identical despite different names*

### Comparing `simulai-toolkit-0.99.8/tests/preprocessing/test_reshaper.py` & `simulai-toolkit-0.99.9/tests/preprocessing/test_reshaper.py`

 * *Files identical despite different names*

### Comparing `simulai-toolkit-0.99.8/tests/preprocessing/test_sampler.py` & `simulai-toolkit-0.99.9/tests/preprocessing/test_sampler.py`

 * *Files identical despite different names*

### Comparing `simulai-toolkit-0.99.8/tests/rbf/test_rbf.py` & `simulai-toolkit-0.99.9/tests/rbf/test_rbf.py`

 * *Files identical despite different names*

### Comparing `simulai-toolkit-0.99.8/tests/residuals/test_symbolicoperator.py` & `simulai-toolkit-0.99.9/tests/residuals/test_symbolicoperator.py`

 * *Files identical despite different names*

### Comparing `simulai-toolkit-0.99.8/tests/rom/test_cnn_autoencoder.py` & `simulai-toolkit-0.99.9/tests/rom/test_cnn_autoencoder.py`

 * *Files identical despite different names*

### Comparing `simulai-toolkit-0.99.8/tests/rom/test_dmd_decomposition.py` & `simulai-toolkit-0.99.9/tests/rom/test_dmd_decomposition.py`

 * *Files identical despite different names*

### Comparing `simulai-toolkit-0.99.8/tests/rom/test_gappy_pca_decomposition.py` & `simulai-toolkit-0.99.9/tests/rom/test_gappy_pca_decomposition.py`

 * *Files identical despite different names*

### Comparing `simulai-toolkit-0.99.8/tests/rom/test_hosvd.py` & `simulai-toolkit-0.99.9/tests/rom/test_hosvd.py`

 * *Files identical despite different names*

### Comparing `simulai-toolkit-0.99.8/tests/rom/test_ipca_datapreparer.py` & `simulai-toolkit-0.99.9/tests/rom/test_ipca_datapreparer.py`

 * *Files identical despite different names*

### Comparing `simulai-toolkit-0.99.8/tests/rom/test_ipca_decomposition.py` & `simulai-toolkit-0.99.9/tests/rom/test_ipca_decomposition.py`

 * *Files identical despite different names*

### Comparing `simulai-toolkit-0.99.8/tests/rom/test_mlp_autoencoder.py` & `simulai-toolkit-0.99.9/tests/rom/test_mlp_autoencoder.py`

 * *Files identical despite different names*

### Comparing `simulai-toolkit-0.99.8/tests/rom/test_pca_decomposition.py` & `simulai-toolkit-0.99.9/tests/rom/test_pca_decomposition.py`

 * *Files identical despite different names*

### Comparing `simulai-toolkit-0.99.8/tests/rom/test_qqm.py` & `simulai-toolkit-0.99.9/tests/rom/test_qqm.py`

 * *Files identical despite different names*

