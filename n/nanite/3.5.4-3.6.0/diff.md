# Comparing `tmp/nanite-3.5.4.tar.gz` & `tmp/nanite-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanite-3.5.4.tar", last modified: Mon Feb 20 21:49:07 2023, max compression
+gzip compressed data, was "nanite-3.6.0.tar", last modified: Fri Jul 21 13:21:02 2023, max compression
```

## Comparing `nanite-3.5.4.tar` & `nanite-3.6.0.tar`

### file list

```diff
@@ -1,122 +1,164 @@
-drwxrwxrwx   0        0        0        0 2023-02-20 21:49:07.877434 nanite-3.5.4/
--rw-rw-rw-   0        0        0     9891 2023-02-20 21:47:41.000000 nanite-3.5.4/CHANGELOG
--rw-rw-rw-   0        0        0    35823 2023-02-20 21:47:41.000000 nanite-3.5.4/LICENSE
--rw-rw-rw-   0        0        0      172 2023-02-20 21:47:41.000000 nanite-3.5.4/MANIFEST.in
--rw-rw-rw-   0        0        0     1910 2023-02-20 21:49:07.877434 nanite-3.5.4/PKG-INFO
--rw-rw-rw-   0        0        0     1056 2023-02-20 21:47:41.000000 nanite-3.5.4/README.rst
-drwxrwxrwx   0        0        0        0 2023-02-20 21:49:07.783678 nanite-3.5.4/nanite/
--rw-rw-rw-   0        0        0      233 2023-02-20 21:47:41.000000 nanite-3.5.4/nanite/__init__.py
--rw-rw-rw-   0        0        0     7292 2023-02-20 21:47:41.000000 nanite-3.5.4/nanite/_version.py
--rw-rw-rw-   0        0        0       85 2023-02-20 21:48:23.000000 nanite-3.5.4/nanite/_version_save.py
-drwxrwxrwx   0        0        0        0 2023-02-20 21:49:07.799305 nanite-3.5.4/nanite/cli/
--rw-rw-rw-   0        0        0      118 2023-02-20 21:47:41.000000 nanite-3.5.4/nanite/cli/__init__.py
--rw-rw-rw-   0        0        0     2120 2023-02-20 21:47:41.000000 nanite-3.5.4/nanite/cli/plotting.py
--rw-rw-rw-   0        0        0     9544 2023-02-20 21:47:41.000000 nanite-3.5.4/nanite/cli/profile.py
--rw-rw-rw-   0        0        0    11842 2023-02-20 21:47:41.000000 nanite-3.5.4/nanite/cli/rating.py
--rw-rw-rw-   0        0        0    23991 2023-02-20 21:47:41.000000 nanite-3.5.4/nanite/fit.py
--rw-rw-rw-   0        0        0     2667 2023-02-20 21:47:41.000000 nanite-3.5.4/nanite/group.py
--rw-rw-rw-   0        0        0    14978 2023-02-20 21:47:41.000000 nanite-3.5.4/nanite/indent.py
-drwxrwxrwx   0        0        0        0 2023-02-20 21:49:07.799305 nanite-3.5.4/nanite/model/
--rw-rw-rw-   0        0        0     3872 2023-02-20 21:47:41.000000 nanite-3.5.4/nanite/model/__init__.py
--rw-rw-rw-   0        0        0    11519 2023-02-20 21:47:41.000000 nanite-3.5.4/nanite/model/core.py
--rw-rw-rw-   0        0        0     2278 2023-02-20 21:47:41.000000 nanite-3.5.4/nanite/model/logic.py
--rw-rw-rw-   0        0        0     2310 2023-02-20 21:47:41.000000 nanite-3.5.4/nanite/model/model_conical_indenter.py
--rw-rw-rw-   0        0        0     3212 2023-02-20 21:47:41.000000 nanite-3.5.4/nanite/model/model_hertz_paraboloidal.py
--rw-rw-rw-   0        0        0     2417 2023-02-20 21:47:41.000000 nanite-3.5.4/nanite/model/model_hertz_three_sided_pyramid.py
--rw-rw-rw-   0        0        0     3808 2023-02-20 21:47:41.000000 nanite-3.5.4/nanite/model/model_sneddon_spherical.pyx
--rw-rw-rw-   0        0        0     3184 2023-02-20 21:47:41.000000 nanite-3.5.4/nanite/model/model_sneddon_spherical_approximation.py
--rw-rw-rw-   0        0        0     3377 2023-02-20 21:47:41.000000 nanite-3.5.4/nanite/model/residuals.py
--rw-rw-rw-   0        0        0      370 2023-02-20 21:47:41.000000 nanite-3.5.4/nanite/model/weight.py
--rw-rw-rw-   0        0        0    16288 2023-02-20 21:47:41.000000 nanite-3.5.4/nanite/poc.py
--rw-rw-rw-   0        0        0    13001 2023-02-20 21:47:41.000000 nanite-3.5.4/nanite/preproc.py
--rw-rw-rw-   0        0        0     2947 2023-02-20 21:47:41.000000 nanite-3.5.4/nanite/qmap.py
-drwxrwxrwx   0        0        0        0 2023-02-20 21:49:07.799305 nanite-3.5.4/nanite/rate/
--rw-rw-rw-   0        0        0       73 2023-02-20 21:47:41.000000 nanite-3.5.4/nanite/rate/__init__.py
--rw-rw-rw-   0        0        0    20028 2023-02-20 21:47:41.000000 nanite-3.5.4/nanite/rate/features.py
--rw-rw-rw-   0        0        0    14360 2023-02-20 21:47:41.000000 nanite-3.5.4/nanite/rate/io.py
--rw-rw-rw-   0        0        0    11602 2023-02-20 21:47:41.000000 nanite-3.5.4/nanite/rate/rater.py
--rw-rw-rw-   0        0        0     1901 2023-02-20 21:47:41.000000 nanite-3.5.4/nanite/rate/regressors.py
-drwxrwxrwx   0        0        0        0 2023-02-20 21:49:07.814961 nanite-3.5.4/nanite/rate/ts_zef18/
--rw-rw-rw-   0        0        0    11320 2023-02-20 21:47:41.000000 nanite-3.5.4/nanite/rate/ts_zef18/train_feat_bin_apr_spikes_count.txt
--rw-rw-rw-   0        0        0    11320 2023-02-20 21:47:41.000000 nanite-3.5.4/nanite/rate/ts_zef18/train_feat_bin_cp_position.txt
--rw-rw-rw-   0        0        0    11320 2023-02-20 21:47:41.000000 nanite-3.5.4/nanite/rate/ts_zef18/train_feat_bin_size.txt
--rw-rw-rw-   0        0        0    11320 2023-02-20 21:47:41.000000 nanite-3.5.4/nanite/rate/ts_zef18/train_feat_con_apr_flatness.txt
--rw-rw-rw-   0        0        0    11320 2023-02-20 21:47:41.000000 nanite-3.5.4/nanite/rate/ts_zef18/train_feat_con_apr_size.txt
--rw-rw-rw-   0        0        0    11320 2023-02-20 21:47:41.000000 nanite-3.5.4/nanite/rate/ts_zef18/train_feat_con_apr_sum.txt
--rw-rw-rw-   0        0        0    11320 2023-02-20 21:47:41.000000 nanite-3.5.4/nanite/rate/ts_zef18/train_feat_con_bln_slope.txt
--rw-rw-rw-   0        0        0    11320 2023-02-20 21:47:41.000000 nanite-3.5.4/nanite/rate/ts_zef18/train_feat_con_bln_variation.txt
--rw-rw-rw-   0        0        0    12260 2023-02-20 21:47:41.000000 nanite-3.5.4/nanite/rate/ts_zef18/train_feat_con_cp_curvature.txt
--rw-rw-rw-   0        0        0    11315 2023-02-20 21:47:41.000000 nanite-3.5.4/nanite/rate/ts_zef18/train_feat_con_cp_magnitude.txt
--rw-rw-rw-   0        0        0    11320 2023-02-20 21:47:41.000000 nanite-3.5.4/nanite/rate/ts_zef18/train_feat_con_idt_maxima_75perc.txt
--rw-rw-rw-   0        0        0    11320 2023-02-20 21:47:41.000000 nanite-3.5.4/nanite/rate/ts_zef18/train_feat_con_idt_monotony.txt
--rw-rw-rw-   0        0        0    11320 2023-02-20 21:47:41.000000 nanite-3.5.4/nanite/rate/ts_zef18/train_feat_con_idt_spike_area.txt
--rw-rw-rw-   0        0        0    11320 2023-02-20 21:47:41.000000 nanite-3.5.4/nanite/rate/ts_zef18/train_feat_con_idt_sum.txt
--rw-rw-rw-   0        0        0    11320 2023-02-20 21:47:41.000000 nanite-3.5.4/nanite/rate/ts_zef18/train_feat_con_idt_sum_75perc.txt
--rw-rw-rw-   0        0        0    11320 2023-02-20 21:47:41.000000 nanite-3.5.4/nanite/rate/ts_zef18/train_response.txt
--rw-rw-rw-   0        0        0     3681 2023-02-20 21:47:41.000000 nanite-3.5.4/nanite/read.py
--rw-rw-rw-   0        0        0     2555 2023-02-20 21:47:41.000000 nanite-3.5.4/nanite/smooth.py
-drwxrwxrwx   0        0        0        0 2023-02-20 21:49:07.783678 nanite-3.5.4/nanite.egg-info/
--rw-rw-rw-   0        0        0     1910 2023-02-20 21:49:07.000000 nanite-3.5.4/nanite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3882 2023-02-20 21:49:07.000000 nanite-3.5.4/nanite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-20 21:49:07.000000 nanite-3.5.4/nanite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      213 2023-02-20 21:49:07.000000 nanite-3.5.4/nanite.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      131 2023-02-20 21:49:07.000000 nanite-3.5.4/nanite.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-02-20 21:49:07.000000 nanite-3.5.4/nanite.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      111 2023-02-20 21:47:41.000000 nanite-3.5.4/pyproject.toml
--rw-rw-rw-   0        0        0      108 2023-02-20 21:49:07.877434 nanite-3.5.4/setup.cfg
--rw-rw-rw-   0        0        0     2439 2023-02-20 21:47:41.000000 nanite-3.5.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-20 21:49:07.846180 nanite-3.5.4/tests/
--rw-rw-rw-   0        0        0     4584 2023-02-20 21:47:41.000000 nanite-3.5.4/tests/common.py
--rw-rw-rw-   0        0        0      544 2023-02-20 21:47:41.000000 nanite-3.5.4/tests/conftest.py
-drwxrwxrwx   0        0        0        0 2023-02-20 21:49:07.877434 nanite-3.5.4/tests/data/
--rw-rw-rw-   0        0        0    68411 2023-02-20 21:47:41.000000 nanite-3.5.4/tests/data/fmt-jpk-cl_calibration_force-save-2015-02-04.jpk-force
--rw-rw-rw-   0        0        0   158553 2023-02-20 21:47:41.000000 nanite-3.5.4/tests/data/fmt-jpk-fd_flipsign_2015.05.22-15.31.49.352.jpk-force
--rw-rw-rw-   0        0        0   497346 2023-02-20 21:47:41.000000 nanite-3.5.4/tests/data/fmt-jpk-fd_map-data-reference-points.jpk-force-map
--rw-rw-rw-   0        0        0   407527 2023-02-20 21:47:41.000000 nanite-3.5.4/tests/data/fmt-jpk-fd_map0d_extracted.jpk-force-map
--rw-rw-rw-   0        0        0  1645418 2023-02-20 21:47:41.000000 nanite-3.5.4/tests/data/fmt-jpk-fd_map1d_2016-11-07.jpk-force-map
--rw-rw-rw-   0        0        0   953060 2023-02-20 21:47:41.000000 nanite-3.5.4/tests/data/fmt-jpk-fd_map2x2_extracted.jpk-force-map
--rw-rw-rw-   0        0        0   401583 2023-02-20 21:47:41.000000 nanite-3.5.4/tests/data/fmt-jpk-fd_map_bad_2013-05-27_1.jpk-force-map
--rw-rw-rw-   0        0        0   400957 2023-02-20 21:47:41.000000 nanite-3.5.4/tests/data/fmt-jpk-fd_map_bad_2013-05-27_2.jpk-force-map
--rw-rw-rw-   0        0        0   193751 2023-02-20 21:47:41.000000 nanite-3.5.4/tests/data/fmt-jpk-fd_single_bad_2017-01-16_1.jpk-force
--rw-rw-rw-   0        0        0   101264 2023-02-20 21:47:41.000000 nanite-3.5.4/tests/data/fmt-jpk-fd_single_bad_2017-01-16_2.jpk-force
--rw-rw-rw-   0        0        0   101240 2023-02-20 21:47:41.000000 nanite-3.5.4/tests/data/fmt-jpk-fd_single_bad_2017-01-16_3.jpk-force
--rw-rw-rw-   0        0        0   103538 2023-02-20 21:47:41.000000 nanite-3.5.4/tests/data/fmt-jpk-fd_single_bad_2017-01-16_4.jpk-force
--rw-rw-rw-   0        0        0   101531 2023-02-20 21:47:41.000000 nanite-3.5.4/tests/data/fmt-jpk-fd_single_bad_2017-01-16_5.jpk-force
--rw-rw-rw-   0        0        0   311042 2023-02-20 21:47:41.000000 nanite-3.5.4/tests/data/fmt-jpk-fd_single_bad_GWAT_2017-10-17.jpk-force
--rw-rw-rw-   0        0        0     6785 2023-02-20 21:47:41.000000 nanite-3.5.4/tests/data/fmt-jpk-fd_single_bad_bead10_2017-04-27.jpk-force
--rw-rw-rw-   0        0        0     6783 2023-02-20 21:47:41.000000 nanite-3.5.4/tests/data/fmt-jpk-fd_single_bad_bead46_2017-04-20.jpk-force
--rw-rw-rw-   0        0        0     6799 2023-02-20 21:47:41.000000 nanite-3.5.4/tests/data/fmt-jpk-fd_single_bad_bead7_2017-04-27.jpk-force
--rw-rw-rw-   0        0        0   596184 2023-02-20 21:47:41.000000 nanite-3.5.4/tests/data/fmt-jpk-fd_single_tilted-baseline-mitotic_2021-01-29.jpk-force
--rw-rw-rw-   0        0        0    22266 2023-02-20 21:47:41.000000 nanite-3.5.4/tests/data/fmt-jpk-fd_spot3-0192.jpk-force
--rw-rw-rw-   0        0        0     1269 2023-02-20 21:47:41.000000 nanite-3.5.4/tests/data/model_external_basic.py
--rw-rw-rw-   0        0        0     1073 2023-02-20 21:47:41.000000 nanite-3.5.4/tests/test_cli_plotting.py
--rw-rw-rw-   0        0        0     2885 2023-02-20 21:47:41.000000 nanite-3.5.4/tests/test_cli_profile.py
--rw-rw-rw-   0        0        0     3031 2023-02-20 21:47:41.000000 nanite-3.5.4/tests/test_cli_rating.py
--rw-rw-rw-   0        0        0     2754 2023-02-20 21:47:41.000000 nanite-3.5.4/tests/test_fit_ancillary.py
--rw-rw-rw-   0        0        0     5915 2023-02-20 21:47:41.000000 nanite-3.5.4/tests/test_fit_base.py
--rw-rw-rw-   0        0        0     4274 2023-02-20 21:47:41.000000 nanite-3.5.4/tests/test_fit_emodulus_search.py
--rw-rw-rw-   0        0        0     1664 2023-02-20 21:47:41.000000 nanite-3.5.4/tests/test_fit_hash.py
--rw-rw-rw-   0        0        0     4440 2023-02-20 21:47:41.000000 nanite-3.5.4/tests/test_fit_properties.py
--rw-rw-rw-   0        0        0     2196 2023-02-20 21:47:41.000000 nanite-3.5.4/tests/test_group.py
--rw-rw-rw-   0        0        0    11518 2023-02-20 21:47:41.000000 nanite-3.5.4/tests/test_indent.py
--rw-rw-rw-   0        0        0     2357 2023-02-20 21:47:41.000000 nanite-3.5.4/tests/test_indent2.py
--rw-rw-rw-   0        0        0     2439 2023-02-20 21:47:41.000000 nanite-3.5.4/tests/test_model.py
--rw-rw-rw-   0        0        0     5177 2023-02-20 21:47:41.000000 nanite-3.5.4/tests/test_model_core.py
--rw-rw-rw-   0        0        0     5264 2023-02-20 21:47:41.000000 nanite-3.5.4/tests/test_model_expr.py
--rw-rw-rw-   0        0        0     3654 2023-02-20 21:47:41.000000 nanite-3.5.4/tests/test_model_hertz_cone.py
--rw-rw-rw-   0        0        0     3420 2023-02-20 21:47:41.000000 nanite-3.5.4/tests/test_model_hertz_parabol.py
--rw-rw-rw-   0        0        0     3554 2023-02-20 21:47:41.000000 nanite-3.5.4/tests/test_model_hertz_pyramid_three.py
--rw-rw-rw-   0        0        0      925 2023-02-20 21:47:41.000000 nanite-3.5.4/tests/test_model_logic.py
--rw-rw-rw-   0        0        0     3658 2023-02-20 21:47:41.000000 nanite-3.5.4/tests/test_model_sneddon_spherical.py
--rw-rw-rw-   0        0        0     2975 2023-02-20 21:47:41.000000 nanite-3.5.4/tests/test_model_sneddon_spherical_approximation.py
--rw-rw-rw-   0        0        0      698 2023-02-20 21:47:41.000000 nanite-3.5.4/tests/test_model_sneddon_spherical_invert_delta.py
--rw-rw-rw-   0        0        0     1871 2023-02-20 21:47:41.000000 nanite-3.5.4/tests/test_model_style.py
--rw-rw-rw-   0        0        0     1405 2023-02-20 21:47:41.000000 nanite-3.5.4/tests/test_open_jpk_variation.py
--rw-rw-rw-   0        0        0     3933 2023-02-20 21:47:41.000000 nanite-3.5.4/tests/test_poc.py
--rw-rw-rw-   0        0        0     5648 2023-02-20 21:47:41.000000 nanite-3.5.4/tests/test_preproc.py
--rw-rw-rw-   0        0        0     7158 2023-02-20 21:47:41.000000 nanite-3.5.4/tests/test_qmap.py
--rw-rw-rw-   0        0        0     5222 2023-02-20 21:47:41.000000 nanite-3.5.4/tests/test_rate_features.py
--rw-rw-rw-   0        0        0     6481 2023-02-20 21:47:41.000000 nanite-3.5.4/tests/test_rate_io.py
--rw-rw-rw-   0        0        0     1781 2023-02-20 21:47:41.000000 nanite-3.5.4/tests/test_rate_training_set.py
--rw-rw-rw-   0        0        0      960 2023-02-20 21:47:41.000000 nanite-3.5.4/tests/test_read.py
--rw-rw-rw-   0        0        0     1970 2023-02-20 21:47:41.000000 nanite-3.5.4/tests/test_smooth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:21:02.731015 nanite-3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-21 13:20:46.000000 nanite-3.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-21 13:20:46.000000 nanite-3.6.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9876 2023-07-21 13:20:46.000000 nanite-3.6.0/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-21 13:20:46.000000 nanite-3.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-21 13:20:46.000000 nanite-3.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-21 13:21:02.731015 nanite-3.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-21 13:20:46.000000 nanite-3.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:21:02.703014 nanite-3.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-21 13:20:46.000000 nanite-3.6.0/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-07-21 13:20:46.000000 nanite-3.6.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:21:02.703014 nanite-3.6.0/docs/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   131520 2023-07-21 13:20:46.000000 nanite-3.6.0/docs/data/force-save-example.jpk-force
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:21:02.703014 nanite-3.6.0/docs/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-07-21 13:20:46.000000 nanite-3.6.0/docs/extensions/fancy_include.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-07-21 13:20:46.000000 nanite-3.6.0/docs/extensions/github_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-21 13:20:46.000000 nanite-3.6.0/docs/extensions/nanite_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-21 13:20:46.000000 nanite-3.6.0/docs/extensions/nanite_preprocs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-07-21 13:20:46.000000 nanite-3.6.0/docs/extensions/simple_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28646 2023-07-21 13:20:46.000000 nanite-3.6.0/docs/fitting_geometry.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14378 2023-07-21 13:20:46.000000 nanite-3.6.0/docs/fitting_geometry.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:21:02.703014 nanite-3.6.0/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    70846 2023-07-21 13:20:46.000000 nanite-3.6.0/docs/img/nanite-fit-example.png
+-rw-r--r--   0 runner    (1001) docker     (123)    86373 2023-07-21 13:20:46.000000 nanite-3.6.0/docs/img/nanite-rate-example.png
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-21 13:20:46.000000 nanite-3.6.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-07-21 13:20:46.000000 nanite-3.6.0/docs/nanite.bib
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-21 13:20:46.000000 nanite-3.6.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-21 13:20:46.000000 nanite-3.6.0/docs/sec_changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-21 13:20:46.000000 nanite-3.6.0/docs/sec_cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-07-21 13:20:46.000000 nanite-3.6.0/docs/sec_code_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9761 2023-07-21 13:20:46.000000 nanite-3.6.0/docs/sec_develop.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-21 13:20:46.000000 nanite-3.6.0/docs/sec_examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10788 2023-07-21 13:20:46.000000 nanite-3.6.0/docs/sec_fitting_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-07-21 13:20:46.000000 nanite-3.6.0/docs/sec_getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-07-21 13:20:46.000000 nanite-3.6.0/docs/sec_rating_workflow.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-21 13:20:46.000000 nanite-3.6.0/docs/sec_z_bib.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:21:02.703014 nanite-3.6.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:21:02.703014 nanite-3.6.0/examples/data/
+-rwxr-xr-x   0 runner    (1001) docker     (123)   159955 2023-07-21 13:20:46.000000 nanite-3.6.0/examples/data/zebrafish-head-section-gray-matter.jpk-force
+-rw-r--r--   0 runner    (1001) docker     (123)    37788 2023-07-21 13:20:46.000000 nanite-3.6.0/examples/fit_and_rate.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-21 13:20:46.000000 nanite-3.6.0/examples/fit_and_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-21 13:20:46.000000 nanite-3.6.0/examples/generate_example_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)   104455 2023-07-21 13:20:46.000000 nanite-3.6.0/examples/model_spherical_indenter.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-07-21 13:20:46.000000 nanite-3.6.0/examples/model_spherical_indenter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:21:02.707014 nanite-3.6.0/nanite/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-21 13:21:02.000000 nanite-3.6.0/nanite/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:21:02.707014 nanite-3.6.0/nanite/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/cli/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9265 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/cli/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11525 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/cli/rating.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23381 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14599 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/indent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:21:02.711014 nanite-3.6.0/nanite/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11218 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/model/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/model/logic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/model/model_conical_indenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/model/model_hertz_paraboloidal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/model/model_hertz_three_sided_pyramid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/model/model_sneddon_spherical.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/model/model_sneddon_spherical_approximation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/model/residuals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/model/weight.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15811 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/poc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12637 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/preproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/qmap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:21:02.711014 nanite-3.6.0/nanite/rate/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/rate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19457 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/rate/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13970 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/rate/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11276 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/rate/rater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/rate/regressors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:21:02.715014 nanite-3.6.0/nanite/rate/ts_zef18/
+-rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/rate/ts_zef18/train_feat_bin_apr_spikes_count.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/rate/ts_zef18/train_feat_bin_cp_position.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/rate/ts_zef18/train_feat_bin_size.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/rate/ts_zef18/train_feat_con_apr_flatness.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/rate/ts_zef18/train_feat_con_apr_size.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/rate/ts_zef18/train_feat_con_apr_sum.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/rate/ts_zef18/train_feat_con_bln_slope.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/rate/ts_zef18/train_feat_con_bln_variation.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/rate/ts_zef18/train_feat_con_cp_curvature.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10183 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/rate/ts_zef18/train_feat_con_cp_magnitude.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/rate/ts_zef18/train_feat_con_idt_maxima_75perc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/rate/ts_zef18/train_feat_con_idt_monotony.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/rate/ts_zef18/train_feat_con_idt_spike_area.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/rate/ts_zef18/train_feat_con_idt_sum.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/rate/ts_zef18/train_feat_con_idt_sum_75perc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/rate/ts_zef18/train_response.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-07-21 13:20:46.000000 nanite-3.6.0/nanite/smooth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:21:02.707014 nanite-3.6.0/nanite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-21 13:21:02.000000 nanite-3.6.0/nanite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-07-21 13:21:02.000000 nanite-3.6.0/nanite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 13:21:02.000000 nanite-3.6.0/nanite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-21 13:21:02.000000 nanite-3.6.0/nanite.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-21 13:21:02.000000 nanite-3.6.0/nanite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-21 13:21:02.000000 nanite-3.6.0/nanite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-07-21 13:20:46.000000 nanite-3.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 13:21:02.731015 nanite-3.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-21 13:20:46.000000 nanite-3.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:21:02.719015 nanite-3.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:21:02.731015 nanite-3.6.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/data/cli-profile-1.7.8.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/data/cli-profile-2.1.0.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    42815 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/data/fmt-afm-workshop-fd_single_2021-10-22_14.16.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    68411 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/data/fmt-jpk-cl_calibration_force-save-2015-02-04.jpk-force
+-rw-r--r--   0 runner    (1001) docker     (123)   158553 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/data/fmt-jpk-fd_flipsign_2015.05.22-15.31.49.352.jpk-force
+-rw-r--r--   0 runner    (1001) docker     (123)   497346 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/data/fmt-jpk-fd_map-data-reference-points.jpk-force-map
+-rw-r--r--   0 runner    (1001) docker     (123)   407527 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/data/fmt-jpk-fd_map0d_extracted.jpk-force-map
+-rwxr-xr-x   0 runner    (1001) docker     (123)  1645418 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/data/fmt-jpk-fd_map1d_2016-11-07.jpk-force-map
+-rw-r--r--   0 runner    (1001) docker     (123)   953060 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/data/fmt-jpk-fd_map2x2_extracted.jpk-force-map
+-rw-r--r--   0 runner    (1001) docker     (123)   401583 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/data/fmt-jpk-fd_map_bad_2013-05-27_1.jpk-force-map
+-rw-r--r--   0 runner    (1001) docker     (123)   400957 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/data/fmt-jpk-fd_map_bad_2013-05-27_2.jpk-force-map
+-rwxr-xr-x   0 runner    (1001) docker     (123)   193751 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/data/fmt-jpk-fd_single_bad_2017-01-16_1.jpk-force
+-rwxr-xr-x   0 runner    (1001) docker     (123)   101264 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/data/fmt-jpk-fd_single_bad_2017-01-16_2.jpk-force
+-rwxr-xr-x   0 runner    (1001) docker     (123)   101240 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/data/fmt-jpk-fd_single_bad_2017-01-16_3.jpk-force
+-rwxr-xr-x   0 runner    (1001) docker     (123)   103538 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/data/fmt-jpk-fd_single_bad_2017-01-16_4.jpk-force
+-rwxr-xr-x   0 runner    (1001) docker     (123)   101531 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/data/fmt-jpk-fd_single_bad_2017-01-16_5.jpk-force
+-rwxr-xr-x   0 runner    (1001) docker     (123)   311042 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/data/fmt-jpk-fd_single_bad_GWAT_2017-10-17.jpk-force
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6785 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/data/fmt-jpk-fd_single_bad_bead10_2017-04-27.jpk-force
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6783 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/data/fmt-jpk-fd_single_bad_bead46_2017-04-20.jpk-force
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6799 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/data/fmt-jpk-fd_single_bad_bead7_2017-04-27.jpk-force
+-rw-r--r--   0 runner    (1001) docker     (123)   596184 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/data/fmt-jpk-fd_single_tilted-baseline-mitotic_2021-01-29.jpk-force
+-rw-r--r--   0 runner    (1001) docker     (123)    22266 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/data/fmt-jpk-fd_spot3-0192.jpk-force
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/data/model_external_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93520 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/data/rate-export_1.7.8.h5
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/test_cli_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/test_cli_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/test_cli_rating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/test_fit_ancillary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/test_fit_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/test_fit_emodulus_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/test_fit_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/test_fit_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/test_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11222 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/test_indent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/test_indent2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/test_model_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/test_model_expr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/test_model_hertz_cone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/test_model_hertz_parabol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/test_model_hertz_pyramid_three.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/test_model_logic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/test_model_sneddon_spherical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/test_model_sneddon_spherical_approximation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/test_model_sneddon_spherical_invert_delta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/test_model_style.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/test_open_jpk_variation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/test_poc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/test_preproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6746 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/test_qmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/test_rate_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/test_rate_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/test_rate_training_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/test_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-07-21 13:20:46.000000 nanite-3.6.0/tests/test_smooth.py
```

### Comparing `nanite-3.5.4/CHANGELOG` & `nanite-3.6.0/CHANGELOG`

 * *Files 14% similar despite different names*

```diff
@@ -1,230 +1,236 @@
-3.5.4
- - setup: drop support for Python 3.7
-3.5.3
- - setup: bump numpy to 1.22.0
-3.5.2
- - build: add wheels for Python up to 3.11
- - ref: fix DeprecationWarnings
- - docs: make docs build on Windows
- - docs: update GH actions badge
- - tests: loosen np.allclose calls
-3.5.1
- - docs: minor update
-3.5.0
- - feat: allow to specify geometric correction factor k during fit
-   (tip position is multiplied by k and contact point is modified
-   directly before and after fit)
-3.4.0
- - feat: allow to load fitting models from external Python files
- - enh: add method to deregister NaniteFitModels
-3.3.1
- - docs: added some clarifications in the model docs
- - enh: check for leading/trailing spaces in models
- - enh: add more checks during loading models
-3.3.0
- - feat: introduce new NaniteFitModel class
- - ref: deprecated get_anc_parms in favor of compute_anc_parms
- - docs: add more information on how to write own model functions
-3.2.1
- - enh: more sensible default parameters for POC estimation fits
-3.2.0
- - feat: allow specifying the minimizer method for fitting (#21)
- - feat: new contact point estimation with linear fit for baseline
-   and polynomial fit for indentation part
- - feat: new contact point estimation with Fréchet distance between
-   curve and direct path in normalized coordinates
- - tests: rename experimental test data files according to
-   afmformats scheme (#20)
-3.1.4
- - docs: preprocessing methods not correctly rendered
-3.1.3
- - fix: make sure that AFM metadata contain the spring constant and
-   raise a MissingMetaDataError if this is not the case
- - ref: deprecate `IndentationPreprocessor` class in favor of a more
-   flat submodule (#17)
-3.1.2
- - docs: add POC table to docs
-3.1.1
- - fix: do not modify preprocessing options when applying them (create
-   a copy of the dictionary)
- - ref: remove `Indentation.reset` in favor of `AFMData.reset_data`
-3.1.0
- - feat: new contact point estimation method "fit_constant_polynomial"
-   which applies a piece-wise constant and polynomial fit
- - feat: contact point estimation methods now return detailed
-   information about the procedure (currently plottable data to
-   understand the process)
- - fix: spatial smoothing not working in some cases (#15)
- - enh: add `steps_optional` in preprocessing to allow fine-grained
-   control about order of application
- - ref: remove "...smoothed" column data (which was never used anyway);
-   instead, apply smoothing directly to AFMData subclass
- - ref: rename `require_steps` to `steps_required` in preprocessing
-   decorator
- - setup: bump afmformats from 0.16.0 to 0.16.4
-3.0.0
- - BREAKING CHANGE: The contact point estimation method "scheme_2020"
-   has been removed, although it has been the default for some time.
-   It turns out that it does not perform so well and there are other
-   more stable methods (to be implemented). Furthermore, some of the
-   contact point estimation methods were improved so that basically
-   many tests had to be updated. This will not break your analysis,
-   it just means your contact points will change.
- - feat: implement options for preprocessing methods
- - feat: the "correct_tip_offset" preprocessing method now
-   accepts the "method" argument (see new poc submodule)
- - fix: contact point estimation with gradient-based method
-   "poc_gradient_zero_crossing" did not really work
- - enh: improve contact point estimation with "fit_constant_line"
- - enh: speed-up contact point estimation with "deviation_from_baseline"
- - ref: CLI profiles now use JSON format by default
-   (old format still supported)
- - ref: move contact point estimation to new 'poc' submodule
-2.0.1
- - enh: implement 'require_steps' in preprocessing to make sure
-   that steps are executed in the correct order
- - enh: add several helper functions for preprocessing
-2.0.0
- - BREAKING CHANGE: segment in FitProperties is now an integer
- - setup: bump afmformats from 0.15.0 to 0.16.0
- - docs: update doc strings for the "sneddon_spher_approx" model
- - docs: remove duplcate docs for model functions
-1.7.8
- - ref: introduce preprocessing_step decorator for managing
-   preprocessing steps
- - ref: explicitly request "force-distance" data from afmformats
-   (can be lifted by ``setting nanite.read.DEFAULT_MODALITY`` to ``None``)
- - setup: bump afmformats from 0.14.3 to 0.15.0 (initial support for
-   loading creep-compliance data)
-1.7.7
- - docs: fix build
-1.7.6
- - setup: bump afmformats from 0.14.1 to 0.14.3 (adjust tests, speed)
-1.7.5
- - ref: migrate `QMap` and `Group` code to afmformats 0.14.1
- - ref: `Indentation` is now a subclass for `afmformats.AFMForceDistance`
- - ref: `QMap` is now a subclass for `afmformats.AFMQMap`
- - ref: `Group` is now a subclass for `afmformats.AFMGroup`
-1.7.4
- - enh: allow passing metadata to the IndentationGroup initializer
- - setup: bump afmformats from 0.10.2 to 0.13.2
- - ref: deprecate get_data_paths in favor of afmformats.find_data
-1.7.3
- - build: move windows pipeline to GH Actions
- - ref: better warning traceback for deprecated weight_cp method
- - ref: DeprecationWarning: np.int from numpy 1.20
-1.7.2
- - build: use oldest-supported-numpy in pyproject.toml
-1.7.1
- - build: migrate to GitHub Actions
-1.7.0
- - enh: simplified writing new model functions by introducing default
-   modeling and residual wrappers
- - ref: improve code readability
-1.6.3
- - tests: fix fails due to tifffile upgrade
- - setup: lift historic pinning of lmfit==0.9.5
-1.6.2
- - tests: improve coverage
- - enh: add sanity checks for models during registration (#5)
-1.6.1
- - enh: if the contact point estimate is not possible, use a fit
-   with a partially constant and linear function
-1.6.0
- - enh: improve contact point estimation by computing the gradient
-   first; resolves issues with tilted baselines (#6)
-   (This may affect fitting results slightly, hence the new minor
-   release)
-1.5.5
- - setup: make tkinter optional for frozen applications
-1.5.4
- - setup: bump scikit-learn from 0.18.0 to 0.23.0 (different
-   model results due to bugfixes, enhancements, or random
-   sampling procedures; the tests have been updated accordingly)
- - setup: bump afmformats from 0.10.0 to 0.10.2
-1.5.3
- - setup: new builds for Python 3.8
-1.5.2
- - enh: be more verbose when tip position cannot be computed
- - setup: bump afmformats from 0.7.0 to 0.10.0
-1.5.1
- - setup: bump afmformats from 0.6.0 to 0.7.0 (metadata fixes)
-1.5.0
- - feat: IndentationGroup.get_enum returns a curve from an enum value
- - setup: bump afmformats from 0.5.0 to 0.6.0 (hdf5 export, improved tab
-   export)
-1.4.1
- - enh: set parameter `baseline` to "vary" for all models
- - fix: make sure that `model_key` is set before `params_initial`
-   when fitting with kwargs (otherwise, `params_initial` might reset)
-1.4.0
- - feat: add function `Indentation.get_rating_parameters`
- - feat: compute additional ancillary parameter "Maximum indentation"
- - feat: new functions `model.get_parm_unit` and updated
-   `model.get_parm_name` to work with ancillary parameters as well
-1.3.0
- - feat: allow to define ancillary parameters for models and use them
-   during fitting by default
- - feat: `Indentation.get_initial_fit_parameters` now automatically
-   computes common and model-related ancillary parameters if no
-   initial parameters are present
- - enh: allow to set the `model_key` in more functions of `Indentation`
- - ref: use `idnt` to represent Indentation instances
- - fix: preprocessing steps not stored in `Indentation.preprocessing`
- - setup: bump afmformats from 0.4.1 to 0.5.0
-1.2.4
- - enh: update boundaries and default values for model parameters
-1.2.3
- - fix: FitProperties did not detect changes in "params_initial"
-1.2.2
- - setup: bump afmformats version from 0.3.0 to 0.4.1
-1.2.1
- - enh: skip computation of tip position if it is already in the
-   dataset and cannot be computed e.g. due to missing spring constant
- - fix: typo in get_data_paths_enum
- - setup: bump afmformats version from 0.2.0 to 0.3.0
-1.2.0
- - tests: np.asscalar is deprecated
- - ref: migrate to afmformats (#1)
- - docs: minor improvements
-1.1.2
- - fix: add ``__version__`` property
- - tests: use time.perf_counter for timing tests
- - docs: improved LaTeX rendering
-1.1.1
- - setup: migrate to PEP 517 (pyproject.toml)
- - docs: minor update
-1.1.0
- - feat: add contact point to available features in qmap visualization
- - fix: avoid two invalid operations when computing features 
-1.0.1
- - fix: invalid operation when loading data with a callback function
-1.0.0
- - docs: minor update
-0.9.3
- - enh: store nanite and h5py library versions in rating container
- - enh: update hyperparameters of rating regressors
- - ref: deprecation in h5py: replace dataset.value by dataset[...]
-0.9.2
- - ref: renamed the mode `model_hertz_parabolic` to
-   `model_hertz_paraboloidal` to be consistent
- - docs: updat code reference and other minor improvements
-0.9.1
- - fix: `preprocessing` keyword not working in `Indentation.fit_model`
- - docs: add another scripting example and minor improvements
- - tests: increase coverage
-0.9.0
- - ref: remove legacy "discrete" feature type
- - ref: renamed kwargs for `Indetation.rate_quality`
- - ref: new method `nanite.load_group` for loading experimental data
- - ref: new class read.data.IndentationData for managing data
- - ref: replace dataset.IndentationDataSet with group.IndentationGroup
-   to avoid ambiguities
- - fix: add missing "zef18" training set
- - fix: sample weight computation failed when a rating level was missing
- - enh: add `nanite-generate-training-set` command line program
- - tests: reduce warnings and increase coverage
- - cleanup: old docs in nanite.rate.io
- - docs: major update using helper extensions
-0.8.0
- - initial release
+3.6.0
+ - tests: make tests less strict and some cleanup
+ - setup: drop support for Python 3.8 and 3.9
+ - setup: bump h5py from 2.8.0 to 3.9.0
+ - build: migrate to pyproject.toml
+ - ci: use cibuildwheel for releases
+3.5.4
+ - setup: drop support for Python 3.7
+3.5.3
+ - setup: bump numpy to 1.22.0
+3.5.2
+ - build: add wheels for Python up to 3.11
+ - ref: fix DeprecationWarnings
+ - docs: make docs build on Windows
+ - docs: update GH actions badge
+ - tests: loosen np.allclose calls
+3.5.1
+ - docs: minor update
+3.5.0
+ - feat: allow to specify geometric correction factor k during fit
+   (tip position is multiplied by k and contact point is modified
+   directly before and after fit)
+3.4.0
+ - feat: allow to load fitting models from external Python files
+ - enh: add method to deregister NaniteFitModels
+3.3.1
+ - docs: added some clarifications in the model docs
+ - enh: check for leading/trailing spaces in models
+ - enh: add more checks during loading models
+3.3.0
+ - feat: introduce new NaniteFitModel class
+ - ref: deprecated get_anc_parms in favor of compute_anc_parms
+ - docs: add more information on how to write own model functions
+3.2.1
+ - enh: more sensible default parameters for POC estimation fits
+3.2.0
+ - feat: allow specifying the minimizer method for fitting (#21)
+ - feat: new contact point estimation with linear fit for baseline
+   and polynomial fit for indentation part
+ - feat: new contact point estimation with Fréchet distance between
+   curve and direct path in normalized coordinates
+ - tests: rename experimental test data files according to
+   afmformats scheme (#20)
+3.1.4
+ - docs: preprocessing methods not correctly rendered
+3.1.3
+ - fix: make sure that AFM metadata contain the spring constant and
+   raise a MissingMetaDataError if this is not the case
+ - ref: deprecate `IndentationPreprocessor` class in favor of a more
+   flat submodule (#17)
+3.1.2
+ - docs: add POC table to docs
+3.1.1
+ - fix: do not modify preprocessing options when applying them (create
+   a copy of the dictionary)
+ - ref: remove `Indentation.reset` in favor of `AFMData.reset_data`
+3.1.0
+ - feat: new contact point estimation method "fit_constant_polynomial"
+   which applies a piece-wise constant and polynomial fit
+ - feat: contact point estimation methods now return detailed
+   information about the procedure (currently plottable data to
+   understand the process)
+ - fix: spatial smoothing not working in some cases (#15)
+ - enh: add `steps_optional` in preprocessing to allow fine-grained
+   control about order of application
+ - ref: remove "...smoothed" column data (which was never used anyway);
+   instead, apply smoothing directly to AFMData subclass
+ - ref: rename `require_steps` to `steps_required` in preprocessing
+   decorator
+ - setup: bump afmformats from 0.16.0 to 0.16.4
+3.0.0
+ - BREAKING CHANGE: The contact point estimation method "scheme_2020"
+   has been removed, although it has been the default for some time.
+   It turns out that it does not perform so well and there are other
+   more stable methods (to be implemented). Furthermore, some of the
+   contact point estimation methods were improved so that basically
+   many tests had to be updated. This will not break your analysis,
+   it just means your contact points will change.
+ - feat: implement options for preprocessing methods
+ - feat: the "correct_tip_offset" preprocessing method now
+   accepts the "method" argument (see new poc submodule)
+ - fix: contact point estimation with gradient-based method
+   "poc_gradient_zero_crossing" did not really work
+ - enh: improve contact point estimation with "fit_constant_line"
+ - enh: speed-up contact point estimation with "deviation_from_baseline"
+ - ref: CLI profiles now use JSON format by default
+   (old format still supported)
+ - ref: move contact point estimation to new 'poc' submodule
+2.0.1
+ - enh: implement 'require_steps' in preprocessing to make sure
+   that steps are executed in the correct order
+ - enh: add several helper functions for preprocessing
+2.0.0
+ - BREAKING CHANGE: segment in FitProperties is now an integer
+ - setup: bump afmformats from 0.15.0 to 0.16.0
+ - docs: update doc strings for the "sneddon_spher_approx" model
+ - docs: remove duplcate docs for model functions
+1.7.8
+ - ref: introduce preprocessing_step decorator for managing
+   preprocessing steps
+ - ref: explicitly request "force-distance" data from afmformats
+   (can be lifted by ``setting nanite.read.DEFAULT_MODALITY`` to ``None``)
+ - setup: bump afmformats from 0.14.3 to 0.15.0 (initial support for
+   loading creep-compliance data)
+1.7.7
+ - docs: fix build
+1.7.6
+ - setup: bump afmformats from 0.14.1 to 0.14.3 (adjust tests, speed)
+1.7.5
+ - ref: migrate `QMap` and `Group` code to afmformats 0.14.1
+ - ref: `Indentation` is now a subclass for `afmformats.AFMForceDistance`
+ - ref: `QMap` is now a subclass for `afmformats.AFMQMap`
+ - ref: `Group` is now a subclass for `afmformats.AFMGroup`
+1.7.4
+ - enh: allow passing metadata to the IndentationGroup initializer
+ - setup: bump afmformats from 0.10.2 to 0.13.2
+ - ref: deprecate get_data_paths in favor of afmformats.find_data
+1.7.3
+ - build: move windows pipeline to GH Actions
+ - ref: better warning traceback for deprecated weight_cp method
+ - ref: DeprecationWarning: np.int from numpy 1.20
+1.7.2
+ - build: use oldest-supported-numpy in pyproject.toml
+1.7.1
+ - build: migrate to GitHub Actions
+1.7.0
+ - enh: simplified writing new model functions by introducing default
+   modeling and residual wrappers
+ - ref: improve code readability
+1.6.3
+ - tests: fix fails due to tifffile upgrade
+ - setup: lift historic pinning of lmfit==0.9.5
+1.6.2
+ - tests: improve coverage
+ - enh: add sanity checks for models during registration (#5)
+1.6.1
+ - enh: if the contact point estimate is not possible, use a fit
+   with a partially constant and linear function
+1.6.0
+ - enh: improve contact point estimation by computing the gradient
+   first; resolves issues with tilted baselines (#6)
+   (This may affect fitting results slightly, hence the new minor
+   release)
+1.5.5
+ - setup: make tkinter optional for frozen applications
+1.5.4
+ - setup: bump scikit-learn from 0.18.0 to 0.23.0 (different
+   model results due to bugfixes, enhancements, or random
+   sampling procedures; the tests have been updated accordingly)
+ - setup: bump afmformats from 0.10.0 to 0.10.2
+1.5.3
+ - setup: new builds for Python 3.8
+1.5.2
+ - enh: be more verbose when tip position cannot be computed
+ - setup: bump afmformats from 0.7.0 to 0.10.0
+1.5.1
+ - setup: bump afmformats from 0.6.0 to 0.7.0 (metadata fixes)
+1.5.0
+ - feat: IndentationGroup.get_enum returns a curve from an enum value
+ - setup: bump afmformats from 0.5.0 to 0.6.0 (hdf5 export, improved tab
+   export)
+1.4.1
+ - enh: set parameter `baseline` to "vary" for all models
+ - fix: make sure that `model_key` is set before `params_initial`
+   when fitting with kwargs (otherwise, `params_initial` might reset)
+1.4.0
+ - feat: add function `Indentation.get_rating_parameters`
+ - feat: compute additional ancillary parameter "Maximum indentation"
+ - feat: new functions `model.get_parm_unit` and updated
+   `model.get_parm_name` to work with ancillary parameters as well
+1.3.0
+ - feat: allow to define ancillary parameters for models and use them
+   during fitting by default
+ - feat: `Indentation.get_initial_fit_parameters` now automatically
+   computes common and model-related ancillary parameters if no
+   initial parameters are present
+ - enh: allow to set the `model_key` in more functions of `Indentation`
+ - ref: use `idnt` to represent Indentation instances
+ - fix: preprocessing steps not stored in `Indentation.preprocessing`
+ - setup: bump afmformats from 0.4.1 to 0.5.0
+1.2.4
+ - enh: update boundaries and default values for model parameters
+1.2.3
+ - fix: FitProperties did not detect changes in "params_initial"
+1.2.2
+ - setup: bump afmformats version from 0.3.0 to 0.4.1
+1.2.1
+ - enh: skip computation of tip position if it is already in the
+   dataset and cannot be computed e.g. due to missing spring constant
+ - fix: typo in get_data_paths_enum
+ - setup: bump afmformats version from 0.2.0 to 0.3.0
+1.2.0
+ - tests: np.asscalar is deprecated
+ - ref: migrate to afmformats (#1)
+ - docs: minor improvements
+1.1.2
+ - fix: add ``__version__`` property
+ - tests: use time.perf_counter for timing tests
+ - docs: improved LaTeX rendering
+1.1.1
+ - setup: migrate to PEP 517 (pyproject.toml)
+ - docs: minor update
+1.1.0
+ - feat: add contact point to available features in qmap visualization
+ - fix: avoid two invalid operations when computing features 
+1.0.1
+ - fix: invalid operation when loading data with a callback function
+1.0.0
+ - docs: minor update
+0.9.3
+ - enh: store nanite and h5py library versions in rating container
+ - enh: update hyperparameters of rating regressors
+ - ref: deprecation in h5py: replace dataset.value by dataset[...]
+0.9.2
+ - ref: renamed the mode `model_hertz_parabolic` to
+   `model_hertz_paraboloidal` to be consistent
+ - docs: updat code reference and other minor improvements
+0.9.1
+ - fix: `preprocessing` keyword not working in `Indentation.fit_model`
+ - docs: add another scripting example and minor improvements
+ - tests: increase coverage
+0.9.0
+ - ref: remove legacy "discrete" feature type
+ - ref: renamed kwargs for `Indetation.rate_quality`
+ - ref: new method `nanite.load_group` for loading experimental data
+ - ref: new class read.data.IndentationData for managing data
+ - ref: replace dataset.IndentationDataSet with group.IndentationGroup
+   to avoid ambiguities
+ - fix: add missing "zef18" training set
+ - fix: sample weight computation failed when a rating level was missing
+ - enh: add `nanite-generate-training-set` command line program
+ - tests: reduce warnings and increase coverage
+ - cleanup: old docs in nanite.rate.io
+ - docs: major update using helper extensions
+0.8.0
+ - initial release
```

### Comparing `nanite-3.5.4/LICENSE` & `nanite-3.6.0/LICENSE`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,674 +1,674 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Use with the GNU Affero General Public License.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<https://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
-<https://www.gnu.org/licenses/why-not-lgpl.html>.
+                    GNU GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The GNU General Public License is a free, copyleft license for
+software and other kinds of works.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+the GNU General Public License is intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.  We, the Free Software Foundation, use the
+GNU General Public License for most of our software; it applies also to
+any other work released this way by its authors.  You can apply it to
+your programs, too.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  To protect your rights, we need to prevent others from denying you
+these rights or asking you to surrender the rights.  Therefore, you have
+certain responsibilities if you distribute copies of the software, or if
+you modify it: responsibilities to respect the freedom of others.
+
+  For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must pass on to the recipients the same
+freedoms that you received.  You must make sure that they, too, receive
+or can get the source code.  And you must show them these terms so they
+know their rights.
+
+  Developers that use the GNU GPL protect your rights with two steps:
+(1) assert copyright on the software, and (2) offer you this License
+giving you legal permission to copy, distribute and/or modify it.
+
+  For the developers' and authors' protection, the GPL clearly explains
+that there is no warranty for this free software.  For both users' and
+authors' sake, the GPL requires that modified versions be marked as
+changed, so that their problems will not be attributed erroneously to
+authors of previous versions.
+
+  Some devices are designed to deny users access to install or run
+modified versions of the software inside them, although the manufacturer
+can do so.  This is fundamentally incompatible with the aim of
+protecting users' freedom to change the software.  The systematic
+pattern of such abuse occurs in the area of products for individuals to
+use, which is precisely where it is most unacceptable.  Therefore, we
+have designed this version of the GPL to prohibit the practice for those
+products.  If such problems arise substantially in other domains, we
+stand ready to extend this provision to those domains in future versions
+of the GPL, as needed to protect the freedom of users.
+
+  Finally, every program is threatened constantly by software patents.
+States should not allow patents to restrict development and use of
+software on general-purpose computers, but in those that do, we wish to
+avoid the special danger that patents applied to a free program could
+make it effectively proprietary.  To prevent this, the GPL assures that
+patents cannot be used to render the program non-free.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU General Public License.
+
+  "Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+  "The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+  To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+  A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+  To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+  To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+  An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+  1. Source Code.
+
+  The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+  A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+  The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+  The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+  The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+  The Corresponding Source for a work in source code form is that
+same work.
+
+  2. Basic Permissions.
+
+  All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+  You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+  Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+  No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+  When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+  4. Conveying Verbatim Copies.
+
+  You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+  You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+  5. Conveying Modified Source Versions.
+
+  You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+  A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+  6. Conveying Non-Source Forms.
+
+  You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+  A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+  A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+  "Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+  If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+  The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+  Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+  7. Additional Terms.
+
+  "Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+  When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+  Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+  All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+  If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+  Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+  8. Termination.
+
+  You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+  However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+  Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+  Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+  9. Acceptance Not Required for Having Copies.
+
+  You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+  10. Automatic Licensing of Downstream Recipients.
+
+  Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+  An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+  You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+  11. Patents.
+
+  A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+  A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+  Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+  In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+  If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+  If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+  A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+  Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+  12. No Surrender of Others' Freedom.
+
+  If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+  13. Use with the GNU Affero General Public License.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU Affero General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the special requirements of the GNU Affero General Public License,
+section 13, concerning interaction through a network will apply to the
+combination as such.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU General Public License from time to time.  Such new versions will
+be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+  Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+  15. Disclaimer of Warranty.
+
+  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. Limitation of Liability.
+
+  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+  17. Interpretation of Sections 15 and 16.
+
+  If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If the program does terminal interaction, make it output a short
+notice like this when it starts in an interactive mode:
+
+    <program>  Copyright (C) <year>  <name of author>
+    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+    This is free software, and you are welcome to redistribute it
+    under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate
+parts of the General Public License.  Of course, your program's commands
+might be different; for a GUI interface, you would use an "about box".
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU GPL, see
+<https://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
+<https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `nanite-3.5.4/PKG-INFO` & `nanite-3.6.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,52 @@
-Metadata-Version: 2.1
-Name: nanite
-Version: 3.5.4
-Summary: Loading, fitting, and rating AFM force-distance data
-Home-page: https://github.com/AFM-analysis/nanite
-Maintainer: Paul Müller
-Maintainer-email: dev@craban.de
-License: GPL v3
-Description: nanite
-        ======
-        
-        |PyPI Version| |Build Status| |Coverage Status| |Docs Status|
-        
-        Loading, fitting, and rating AFM force-distance data.
-        
-        Documentation
-        -------------
-        
-        The documentation, including the code reference and examples, is available at
-        `nanite.readthedocs.io <https://nanite.readthedocs.io/en/stable/>`__.
-        
-        
-        Installation
-        ------------
-        To install the latest release, simply run:
-        
-        ::
-        
-            pip install nanite[CLI]
-        
-        
-        .. |PyPI Version| image:: https://img.shields.io/pypi/v/nanite.svg
-           :target: https://pypi.python.org/pypi/nanite
-        .. |Build Status| image:: https://img.shields.io/github/actions/workflow/status/AFM-analysis/nanite/check.yml
-           :target: https://github.com/AFM-analysis/nanite/actions?query=workflow%3AChecks
-        .. |Coverage Status| image:: https://img.shields.io/codecov/c/github/AFM-analysis/nanite/master.svg
-           :target: https://codecov.io/gh/AFM-analysis/nanite
-        .. |Docs Status| image:: https://readthedocs.org/projects/nanite/badge/?version=latest
-           :target: https://readthedocs.org/projects/nanite/builds/
-        
-Keywords: atomic force microscopy,mechanical phenotyping,tissue analysis
-Platform: ALL
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Scientific/Engineering :: Visualization
-Classifier: Intended Audience :: Science/Research
-Requires-Python: >=3.8, <4
-Provides-Extra: CLI
+Metadata-Version: 2.1
+Name: nanite
+Version: 3.6.0
+Summary: Loading, fitting, and rating AFM force-distance data
+Author: Paul Müller, Shada Abuhattum
+Maintainer-email: Paul Müller <dev@craban.de>
+License: GPL version 3
+Project-URL: source, https://github.com/AFM-Analysis/nanite
+Project-URL: tracker, https://github.com/AFM-Analysis/nanite/issues
+Project-URL: documentation, https://nanite.readthedocs.io/en/stable/
+Project-URL: changelog, https://nanite.readthedocs.io/en/stable/sec_changelog.html
+Keywords: atomic force microscopy,mechanical phenotyping,tissue analysis
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering :: Visualization
+Classifier: Intended Audience :: Science/Research
+Requires-Python: <4,>=3.10
+Description-Content-Type: text/x-rst
+Provides-Extra: CLI
+License-File: LICENSE
+
+nanite
+======
+
+|PyPI Version| |Build Status| |Coverage Status| |Docs Status|
+
+Loading, fitting, and rating AFM force-distance data.
+
+Documentation
+-------------
+
+The documentation, including the code reference and examples, is available at
+`nanite.readthedocs.io <https://nanite.readthedocs.io/en/stable/>`__.
+
+
+Installation
+------------
+To install the latest release, simply run:
+
+::
+
+    pip install nanite[CLI]
+
+
+.. |PyPI Version| image:: https://img.shields.io/pypi/v/nanite.svg
+   :target: https://pypi.python.org/pypi/nanite
+.. |Build Status| image:: https://img.shields.io/github/actions/workflow/status/AFM-analysis/nanite/check.yml
+   :target: https://github.com/AFM-analysis/nanite/actions?query=workflow%3AChecks
+.. |Coverage Status| image:: https://img.shields.io/codecov/c/github/AFM-analysis/nanite/master.svg
+   :target: https://codecov.io/gh/AFM-analysis/nanite
+.. |Docs Status| image:: https://readthedocs.org/projects/nanite/badge/?version=latest
+   :target: https://readthedocs.org/projects/nanite/builds/
```

### Comparing `nanite-3.5.4/README.rst` & `nanite-3.6.0/README.rst`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-nanite
-======
-
-|PyPI Version| |Build Status| |Coverage Status| |Docs Status|
-
-Loading, fitting, and rating AFM force-distance data.
-
-Documentation
--------------
-
-The documentation, including the code reference and examples, is available at
-`nanite.readthedocs.io <https://nanite.readthedocs.io/en/stable/>`__.
-
-
-Installation
-------------
-To install the latest release, simply run:
-
-::
-
-    pip install nanite[CLI]
-
-
-.. |PyPI Version| image:: https://img.shields.io/pypi/v/nanite.svg
-   :target: https://pypi.python.org/pypi/nanite
-.. |Build Status| image:: https://img.shields.io/github/actions/workflow/status/AFM-analysis/nanite/check.yml
-   :target: https://github.com/AFM-analysis/nanite/actions?query=workflow%3AChecks
-.. |Coverage Status| image:: https://img.shields.io/codecov/c/github/AFM-analysis/nanite/master.svg
-   :target: https://codecov.io/gh/AFM-analysis/nanite
-.. |Docs Status| image:: https://readthedocs.org/projects/nanite/badge/?version=latest
-   :target: https://readthedocs.org/projects/nanite/builds/
+nanite
+======
+
+|PyPI Version| |Build Status| |Coverage Status| |Docs Status|
+
+Loading, fitting, and rating AFM force-distance data.
+
+Documentation
+-------------
+
+The documentation, including the code reference and examples, is available at
+`nanite.readthedocs.io <https://nanite.readthedocs.io/en/stable/>`__.
+
+
+Installation
+------------
+To install the latest release, simply run:
+
+::
+
+    pip install nanite[CLI]
+
+
+.. |PyPI Version| image:: https://img.shields.io/pypi/v/nanite.svg
+   :target: https://pypi.python.org/pypi/nanite
+.. |Build Status| image:: https://img.shields.io/github/actions/workflow/status/AFM-analysis/nanite/check.yml
+   :target: https://github.com/AFM-analysis/nanite/actions?query=workflow%3AChecks
+.. |Coverage Status| image:: https://img.shields.io/codecov/c/github/AFM-analysis/nanite/master.svg
+   :target: https://codecov.io/gh/AFM-analysis/nanite
+.. |Docs Status| image:: https://readthedocs.org/projects/nanite/badge/?version=latest
+   :target: https://readthedocs.org/projects/nanite/builds/
```

### Comparing `nanite-3.5.4/nanite/cli/plotting.py` & `nanite-3.6.0/nanite/cli/plotting.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-import matplotlib.pylab as plt
-import numpy as np
-
-
-def plot_data(idnt, figure=None, add_text="", path=None):
-    if figure is None:
-        figure = plt.figure(figsize=(10, 7))
-    else:
-        figure.clear()
-    ax = figure.add_axes([.07, .1, .90, .87])
-    ax.set_xlabel("tip position [µm]")
-    ax.set_ylabel("force [nN]")
-    # overview plot
-    ax.plot(idnt["tip position"] * 1e6, idnt["fit"] * 1e9)
-    ax.plot(idnt["tip position"] * 1e6, idnt["force"] * 1e9)
-    # inset with indentation
-    axin = figure.add_axes([.3, .3, .65, .65])
-    axin.patch.set_alpha(0.5)
-    # inset limits depend on contact point
-    axin.plot(idnt["tip position"] * 1e6, idnt["fit"] * 1e9, label="fit")
-    axin.plot(idnt["tip position"] * 1e6, idnt["force"] * 1e9, label="data")
-    axin.legend(loc="upper right")
-    axin.grid()
-    cp = idnt.fit_properties["params_fitted"]["contact_point"].value * 1e6
-    xmin = idnt["tip position"].min() * 1e6
-    dx = np.abs(cp - xmin)
-    ymin = idnt["force"][idnt["segment"] == 0].min() * 1e9
-    ymax = idnt["force"][idnt["segment"] == 0].max() * 1e9
-    dy = ymax - ymin
-    axin.set_xlim(xmin - dx/7, cp + dx/2)
-    axin.set_ylim(ymin - dy/7, ymax + dy/7)
-    axin.set_xticks([])
-    axin.set_ylabel("close-up")
-    # inset with residuals
-    axin2 = figure.add_axes([.3, .15, .65, .14])
-    axin2.patch.set_alpha(0.5)
-    axin2.plot(idnt["tip position"] * 1e6,
-               idnt["fit residuals"] * 1e9, label="fit")
-    axin2.set_xlim(xmin - dx/7, cp + dx/2)
-    axin2.set_ylabel("fit residuals")
-    axin2.axhline(0, color="gray")
-    axin2.set_ylim(-dy/10, dy/10)
-    # display fitted parameters
-    text = "Fit parameters:\n"
-    text += "model: {}\n".format(idnt.fit_properties["model_key"])
-    params = idnt.fit_properties["params_fitted"]
-    for p in params:
-        text += "{}={:.2e}\n".format(p, params[p].value)
-    text += "\n\n" + add_text
-    axin.text(cp, ymax, text, horizontalalignment="right",
-              verticalalignment="top")
-
-    if path is not None:
-        figure.savefig(path)
-        plt.close()
+import matplotlib.pylab as plt
+import numpy as np
+
+
+def plot_data(idnt, figure=None, add_text="", path=None):
+    if figure is None:
+        figure = plt.figure(figsize=(10, 7))
+    else:
+        figure.clear()
+    ax = figure.add_axes([.07, .1, .90, .87])
+    ax.set_xlabel("tip position [µm]")
+    ax.set_ylabel("force [nN]")
+    # overview plot
+    ax.plot(idnt["tip position"] * 1e6, idnt["fit"] * 1e9)
+    ax.plot(idnt["tip position"] * 1e6, idnt["force"] * 1e9)
+    # inset with indentation
+    axin = figure.add_axes([.3, .3, .65, .65])
+    axin.patch.set_alpha(0.5)
+    # inset limits depend on contact point
+    axin.plot(idnt["tip position"] * 1e6, idnt["fit"] * 1e9, label="fit")
+    axin.plot(idnt["tip position"] * 1e6, idnt["force"] * 1e9, label="data")
+    axin.legend(loc="upper right")
+    axin.grid()
+    cp = idnt.fit_properties["params_fitted"]["contact_point"].value * 1e6
+    xmin = idnt["tip position"].min() * 1e6
+    dx = np.abs(cp - xmin)
+    ymin = idnt["force"][idnt["segment"] == 0].min() * 1e9
+    ymax = idnt["force"][idnt["segment"] == 0].max() * 1e9
+    dy = ymax - ymin
+    axin.set_xlim(xmin - dx/7, cp + dx/2)
+    axin.set_ylim(ymin - dy/7, ymax + dy/7)
+    axin.set_xticks([])
+    axin.set_ylabel("close-up")
+    # inset with residuals
+    axin2 = figure.add_axes([.3, .15, .65, .14])
+    axin2.patch.set_alpha(0.5)
+    axin2.plot(idnt["tip position"] * 1e6,
+               idnt["fit residuals"] * 1e9, label="fit")
+    axin2.set_xlim(xmin - dx/7, cp + dx/2)
+    axin2.set_ylabel("fit residuals")
+    axin2.axhline(0, color="gray")
+    axin2.set_ylim(-dy/10, dy/10)
+    # display fitted parameters
+    text = "Fit parameters:\n"
+    text += "model: {}\n".format(idnt.fit_properties["model_key"])
+    params = idnt.fit_properties["params_fitted"]
+    for p in params:
+        text += "{}={:.2e}\n".format(p, params[p].value)
+    text += "\n\n" + add_text
+    axin.text(cp, ymax, text, horizontalalignment="right",
+              verticalalignment="top")
+
+    if path is not None:
+        figure.savefig(path)
+        plt.close()
```

### Comparing `nanite-3.5.4/nanite/cli/rating.py` & `nanite-3.6.0/nanite/cli/rating.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,317 +1,317 @@
-import argparse
-import io
-from functools import lru_cache
-import getpass
-from os import fspath
-import pathlib
-try:
-    import tkinter as tk
-except (ImportError, FileNotFoundError):
-    TK_AVAILABLE = False
-else:
-    from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg
-    TK_AVAILABLE = True
-
-import types
-
-import afmformats
-from matplotlib.figure import Figure
-import matplotlib.image as mpimg
-import tifffile
-
-from ..indent import Indentation
-from ..group import IndentationGroup
-from ..read import get_data_paths_enum
-from ..rate import io as rio
-
-from .profile import Profile, PROFILE_PATH
-from .plotting import plot_data
-
-
-class RatingGUI:
-    def __init__(self, root, data_paths, h5path):
-        self.data_paths = data_paths
-        self.h5path = h5path
-        self.current_index = 0
-        self.idnt = None
-        self.root = root
-
-        root.wm_protocol("WM_DELETE_WINDOW", self.close)
-        tk.Grid.rowconfigure(root, 0, weight=1)
-        tk.Grid.columnconfigure(root, 0, weight=1)
-
-        root.title("nanite force-distance rater")
-
-        master = tk.Frame(root)
-        master.grid(row=0, column=0, sticky=tk.N+tk.S+tk.E+tk.W)
-        self.master = master
-
-        tk.Grid.rowconfigure(master, 1, weight=1)
-
-        for ii in range(7):
-            tk.Grid.columnconfigure(master, ii, weight=1)
-
-        l1 = tk.Label(master, text="User text!")
-        l1.grid(row=0, column=0, columnspan=6)
-
-        self.figure = Figure(figsize=(10, 7), dpi=100)
-        self.canvas = FigureCanvasTkAgg(self.figure, master=master)
-        self.canvas.get_tk_widget().grid(row=1,
-                                         column=0,
-                                         columnspan=6,
-                                         sticky=tk.N+tk.S+tk.E+tk.W)
-
-        l2 = tk.Label(master, text="user:")
-        l2.grid(row=2, column=0, sticky=tk.E)
-        self.user = tk.Entry(master, text="user:", width=30)
-        self.user.insert(0, getpass.getuser())
-        self.user.grid(row=2, column=1, sticky=tk.W)
-
-        l3 = tk.Label(master, text="rating:")
-        l3.grid(row=2, column=2, sticky=tk.E)
-        self.rating = tk.Spinbox(master, from_=-1, to=10)
-        self.rating.grid(row=2, column=3, sticky=tk.W)
-
-        self.prev_button = tk.Button(master,
-                                     text="Previous (Alt+Left)",
-                                     command=self.previous)
-        root.bind('<Alt-Left>', self.previous)
-        self.prev_button.grid(row=2, column=4, sticky=tk.W+tk.E)
-
-        self.next_button = tk.Button(master,
-                                     text="Next (Alt+Right)",
-                                     command=self.next)
-        root.bind('<Alt-Right>', self.next)
-        self.next_button.grid(row=2, column=5, sticky=tk.W+tk.E)
-
-        l4 = tk.Label(master, text="comment:")
-        l4.grid(row=3, column=0, sticky=tk.E)
-        self.comment = tk.Entry(master, width=100)
-        self.comment.grid(row=3, column=1, columnspan=5, sticky=tk.W+tk.E)
-
-        # skip to first unrated curve
-        while True:
-            fakeidnt = types.SimpleNamespace()
-            fakeidnt.path = self.current_path
-            fakeidnt.enum = self.current_enum
-            rated, _, _ = rio.hdf5_rated(self.h5path, indent=fakeidnt)
-            if not rated:
-                break
-            else:
-                self.current_index += 1
-        self.load()
-
-    @property
-    def current_path(self):
-        return self.data_paths[self.current_index][0]
-
-    @property
-    def current_enum(self):
-        return self.data_paths[self.current_index][1]
-
-    def close(self):
-        self.save()
-        self.root.destroy()
-
-    def next(self, e=None):
-        self.save()
-        self.current_index += 1
-        if self.current_index == len(self.data_paths):
-            self.current_index = 0
-        self.load()
-
-    def previous(self, e=None):
-        self.save()
-        self.current_index -= 1
-        if self.current_index < 0:
-            self.current_index = len(self.data_paths) - 1
-        self.load()
-
-    def load(self):
-        self.set_label_path()
-        path = self.current_path
-        enum = self.current_enum
-        self.idnt = fit_data(path=path, enum=enum)
-        plot_data(self.idnt, figure=self.figure)
-        self.canvas.draw()
-
-        # set rating
-        self.rating.delete(0, tk.END)
-        self.comment.delete(0, tk.END)
-        rated, rating, comment = rio.hdf5_rated(self.h5path, indent=self.idnt)
-        if rated:
-            self.rating.insert(0, "{}".format(rating))
-            self.comment.insert(0, "{}".format(comment))
-
-    def save(self):
-        rating = self.rating.get()
-        if rating:
-            rio.save_hdf5(h5path=self.h5path,
-                          indent=self.idnt,
-                          user_rate=int(rating),
-                          user_name=self.user.get(),
-                          user_comment=self.comment.get(),
-                          h5mode="a")
-
-    def set_label_path(self):
-        if hasattr(self, "label_path"):
-            self.label_path.destroy()
-        self.label_path = tk.Label(self.master,
-                                   text="curve {}/{}: {} - {}".format(
-                                       self.current_index + 1,
-                                       len(self.data_paths),
-                                       self.current_path,
-                                       self.current_enum))
-        self.label_path.grid(row=0, column=0, columnspan=6)
-
-
-def fit():
-    parser = fit_parser()
-    args = parser.parse_args()
-    path = pathlib.Path(args.data_path).resolve()
-    pout = pathlib.Path(args.out_dir).resolve()
-    pout.mkdir(exist_ok=True, parents=True)
-    fit_perform(path, path_results=pout)
-
-
-def fit_perform(path, path_results, profile_path=PROFILE_PATH):
-    path_results = pathlib.Path(path_results)
-    ptsv = path_results / "statistics.tsv"
-    ptif = path_results / "plots.tif"
-    # exported data columns
-    pf = Profile(path=profile_path, create=False)
-    dlist = [["path", lambda x: x.path],
-             ["enum", lambda x: x.enum],
-             ["E", lambda x: x.fit_properties["params_fitted"]["E"].value],
-             ["rating", lambda x: round(x.rate_quality(
-                 training_set=pf["rating training set"],
-                 regressor=pf["rating regressor"]),
-                 ndigits=1)],
-             ]
-    ddict = dict(dlist)
-    header = "\t".join([dd[0] for dd in dlist])
-    with ptsv.open(mode="w") as ts:
-        ts.write(header + "\n")
-    # get all files in path
-    datapaths = afmformats.find_data(path, modality="force-distance")
-    with tifffile.TiffWriter(fspath(ptif), imagej=True) as tf, \
-            ptsv.open(mode="a") as ts:
-        for pp in datapaths:
-            print("Processing: {}".format(pp))
-            grp = IndentationGroup(pp)
-            for idnt in grp:
-                fit_data(idnt, profile_path=profile_path)
-                # save statistics
-                stats = [str(dd[1](idnt)) for dd in dlist]
-                ts.write("\t".join(stats) + "\n")
-                # save plot
-                imio = io.BytesIO()
-                rating_text = "Rating parameters:\n" \
-                    + "regressor: {}\n".format(pf["rating regressor"]) \
-                    + "training set: {}\n".format(pf["rating training set"]) \
-                    + "rating: {:.1f}\n".format(ddict["rating"](idnt))
-                plot_data(idnt,
-                          add_text=rating_text,
-                          path=imio)
-                imio.seek(0)
-                imdat = (mpimg.imread(imio) * 255).astype("uint8")
-                tf.write(imdat, contiguous=True)
-
-
-@lru_cache(maxsize=5)
-def fit_data(path, enum=0, profile_path=PROFILE_PATH):
-    if isinstance(path, Indentation):
-        idnt = path
-    else:
-        idnt = IndentationGroup(path)[enum]
-
-    pf = Profile(path=profile_path, create=False)
-
-    idnt.apply_preprocessing(preprocessing=pf["preprocessing"],
-                             options=pf["preprocessing_options"])
-    params = pf.get_fit_params()
-
-    idnt.fit_model(model_key=pf["model_key"],
-                   params_initial=params,
-                   range_type=pf["range_type"],
-                   range_x=pf["range_x"],
-                   segment=pf["segment"],
-                   weight_cp=pf["weight_cp"],
-                   )
-    return idnt
-
-
-def fit_parser():
-    descr = "Fit AFM force-distance data. Statistics (.tsv file) and " \
-            + "visualizations of the fits (multi-page .tif file) are stored " \
-            + "in the results directory."
-    parser = argparse.ArgumentParser(description=descr)
-    parser.add_argument('data_path', type=str,
-                        help='input folder containing AFM force-distance '
-                             + 'data')
-    parser.add_argument('out_dir', type=str,
-                        help='results directory')
-    return parser
-
-
-def generate_training_set_parser():
-    descr = "Create a training set for usage in nanite from rating " \
-            "containers (.h5 files manually created with `nanite-rate`)."
-    parser = argparse.ArgumentParser(description=descr)
-    parser.add_argument('data_path', type=str,
-                        help='path to a rating container or a folder '
-                             + 'containing rating containers')
-    parser.add_argument('out_dir', type=str,
-                        help='directory where the training set will be '
-                             ' stored')
-    return parser
-
-
-def generate_training_set():
-    parser = generate_training_set_parser()
-    args = parser.parse_args()
-    data_path = pathlib.Path(args.data_path).resolve()
-    out_dir = pathlib.Path(args.out_dir).resolve()
-    name = data_path.stem
-    if data_path.exists():
-        print("Generating training set '{}'.".format(name))
-        rm = rio.RateManager(data_path, verbose=1)
-        rm.export_training_set(out_dir / "ts_{}".format(name))
-    else:
-        print("Path does not exist: '{}'".format(data_path))
-
-
-def rate():
-    parser = rate_parser()
-    args = parser.parse_args()
-    path = pathlib.Path(args.data_path).resolve()
-    h5 = pathlib.Path(args.rating_path).resolve()
-    if not h5.name.endswith(".h5"):
-        h5 = h5.with_name(h5.name + ".h5")
-    # get all files in path
-    enumpaths = get_data_paths_enum(path, skip_errors=True)
-    # for now, only compare single curves
-    enumpaths = [ee for ee in enumpaths if ee[0].suffix == ".jpk-force"]
-    if TK_AVAILABLE:
-        # start GUI
-        root = tk.Tk()
-        RatingGUI(root, data_paths=enumpaths, h5path=h5)
-        root.mainloop()
-    else:
-        raise ValueError("tkinter is not available! (frozen application?)")
-
-
-def rate_parser():
-    descr = "Manually rate (the fit to) AFM force-distance data. " \
-            + "A graphical user interface allows to rate and comment on " \
-            + "each force-distance curve. The fits and the raw data are " \
-            + "stored in a rating container that can then be passed to " \
-            + "`nanite-generate-training-set`."
-    parser = argparse.ArgumentParser(description=descr)
-    parser.add_argument('data_path', type=str,
-                        help='input folder containing AFM force-distance '
-                             + 'data')
-    parser.add_argument('rating_path', type=str,
-                        help='path to the output rating container (will '
-                             + 'be created if it does not already exist)')
-    return parser
+import argparse
+import io
+from functools import lru_cache
+import getpass
+from os import fspath
+import pathlib
+try:
+    import tkinter as tk
+except (ImportError, FileNotFoundError):
+    TK_AVAILABLE = False
+else:
+    from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg
+    TK_AVAILABLE = True
+
+import types
+
+import afmformats
+from matplotlib.figure import Figure
+import matplotlib.image as mpimg
+import tifffile
+
+from ..indent import Indentation
+from ..group import IndentationGroup
+from ..read import get_data_paths_enum
+from ..rate import io as rio
+
+from .profile import Profile, PROFILE_PATH
+from .plotting import plot_data
+
+
+class RatingGUI:
+    def __init__(self, root, data_paths, h5path):
+        self.data_paths = data_paths
+        self.h5path = h5path
+        self.current_index = 0
+        self.idnt = None
+        self.root = root
+
+        root.wm_protocol("WM_DELETE_WINDOW", self.close)
+        tk.Grid.rowconfigure(root, 0, weight=1)
+        tk.Grid.columnconfigure(root, 0, weight=1)
+
+        root.title("nanite force-distance rater")
+
+        master = tk.Frame(root)
+        master.grid(row=0, column=0, sticky=tk.N+tk.S+tk.E+tk.W)
+        self.master = master
+
+        tk.Grid.rowconfigure(master, 1, weight=1)
+
+        for ii in range(7):
+            tk.Grid.columnconfigure(master, ii, weight=1)
+
+        l1 = tk.Label(master, text="User text!")
+        l1.grid(row=0, column=0, columnspan=6)
+
+        self.figure = Figure(figsize=(10, 7), dpi=100)
+        self.canvas = FigureCanvasTkAgg(self.figure, master=master)
+        self.canvas.get_tk_widget().grid(row=1,
+                                         column=0,
+                                         columnspan=6,
+                                         sticky=tk.N+tk.S+tk.E+tk.W)
+
+        l2 = tk.Label(master, text="user:")
+        l2.grid(row=2, column=0, sticky=tk.E)
+        self.user = tk.Entry(master, text="user:", width=30)
+        self.user.insert(0, getpass.getuser())
+        self.user.grid(row=2, column=1, sticky=tk.W)
+
+        l3 = tk.Label(master, text="rating:")
+        l3.grid(row=2, column=2, sticky=tk.E)
+        self.rating = tk.Spinbox(master, from_=-1, to=10)
+        self.rating.grid(row=2, column=3, sticky=tk.W)
+
+        self.prev_button = tk.Button(master,
+                                     text="Previous (Alt+Left)",
+                                     command=self.previous)
+        root.bind('<Alt-Left>', self.previous)
+        self.prev_button.grid(row=2, column=4, sticky=tk.W+tk.E)
+
+        self.next_button = tk.Button(master,
+                                     text="Next (Alt+Right)",
+                                     command=self.next)
+        root.bind('<Alt-Right>', self.next)
+        self.next_button.grid(row=2, column=5, sticky=tk.W+tk.E)
+
+        l4 = tk.Label(master, text="comment:")
+        l4.grid(row=3, column=0, sticky=tk.E)
+        self.comment = tk.Entry(master, width=100)
+        self.comment.grid(row=3, column=1, columnspan=5, sticky=tk.W+tk.E)
+
+        # skip to first unrated curve
+        while True:
+            fakeidnt = types.SimpleNamespace()
+            fakeidnt.path = self.current_path
+            fakeidnt.enum = self.current_enum
+            rated, _, _ = rio.hdf5_rated(self.h5path, indent=fakeidnt)
+            if not rated:
+                break
+            else:
+                self.current_index += 1
+        self.load()
+
+    @property
+    def current_path(self):
+        return self.data_paths[self.current_index][0]
+
+    @property
+    def current_enum(self):
+        return self.data_paths[self.current_index][1]
+
+    def close(self):
+        self.save()
+        self.root.destroy()
+
+    def next(self, e=None):
+        self.save()
+        self.current_index += 1
+        if self.current_index == len(self.data_paths):
+            self.current_index = 0
+        self.load()
+
+    def previous(self, e=None):
+        self.save()
+        self.current_index -= 1
+        if self.current_index < 0:
+            self.current_index = len(self.data_paths) - 1
+        self.load()
+
+    def load(self):
+        self.set_label_path()
+        path = self.current_path
+        enum = self.current_enum
+        self.idnt = fit_data(path=path, enum=enum)
+        plot_data(self.idnt, figure=self.figure)
+        self.canvas.draw()
+
+        # set rating
+        self.rating.delete(0, tk.END)
+        self.comment.delete(0, tk.END)
+        rated, rating, comment = rio.hdf5_rated(self.h5path, indent=self.idnt)
+        if rated:
+            self.rating.insert(0, "{}".format(rating))
+            self.comment.insert(0, "{}".format(comment))
+
+    def save(self):
+        rating = self.rating.get()
+        if rating:
+            rio.save_hdf5(h5path=self.h5path,
+                          indent=self.idnt,
+                          user_rate=int(rating),
+                          user_name=self.user.get(),
+                          user_comment=self.comment.get(),
+                          h5mode="a")
+
+    def set_label_path(self):
+        if hasattr(self, "label_path"):
+            self.label_path.destroy()
+        self.label_path = tk.Label(self.master,
+                                   text="curve {}/{}: {} - {}".format(
+                                       self.current_index + 1,
+                                       len(self.data_paths),
+                                       self.current_path,
+                                       self.current_enum))
+        self.label_path.grid(row=0, column=0, columnspan=6)
+
+
+def fit():
+    parser = fit_parser()
+    args = parser.parse_args()
+    path = pathlib.Path(args.data_path).resolve()
+    pout = pathlib.Path(args.out_dir).resolve()
+    pout.mkdir(exist_ok=True, parents=True)
+    fit_perform(path, path_results=pout)
+
+
+def fit_perform(path, path_results, profile_path=PROFILE_PATH):
+    path_results = pathlib.Path(path_results)
+    ptsv = path_results / "statistics.tsv"
+    ptif = path_results / "plots.tif"
+    # exported data columns
+    pf = Profile(path=profile_path, create=False)
+    dlist = [["path", lambda x: x.path],
+             ["enum", lambda x: x.enum],
+             ["E", lambda x: x.fit_properties["params_fitted"]["E"].value],
+             ["rating", lambda x: round(x.rate_quality(
+                 training_set=pf["rating training set"],
+                 regressor=pf["rating regressor"]),
+                 ndigits=1)],
+             ]
+    ddict = dict(dlist)
+    header = "\t".join([dd[0] for dd in dlist])
+    with ptsv.open(mode="w") as ts:
+        ts.write(header + "\n")
+    # get all files in path
+    datapaths = afmformats.find_data(path, modality="force-distance")
+    with tifffile.TiffWriter(fspath(ptif), imagej=True) as tf, \
+            ptsv.open(mode="a") as ts:
+        for pp in datapaths:
+            print("Processing: {}".format(pp))
+            grp = IndentationGroup(pp)
+            for idnt in grp:
+                fit_data(idnt, profile_path=profile_path)
+                # save statistics
+                stats = [str(dd[1](idnt)) for dd in dlist]
+                ts.write("\t".join(stats) + "\n")
+                # save plot
+                imio = io.BytesIO()
+                rating_text = "Rating parameters:\n" \
+                    + "regressor: {}\n".format(pf["rating regressor"]) \
+                    + "training set: {}\n".format(pf["rating training set"]) \
+                    + "rating: {:.1f}\n".format(ddict["rating"](idnt))
+                plot_data(idnt,
+                          add_text=rating_text,
+                          path=imio)
+                imio.seek(0)
+                imdat = (mpimg.imread(imio) * 255).astype("uint8")
+                tf.write(imdat, contiguous=True)
+
+
+@lru_cache(maxsize=5)
+def fit_data(path, enum=0, profile_path=PROFILE_PATH):
+    if isinstance(path, Indentation):
+        idnt = path
+    else:
+        idnt = IndentationGroup(path)[enum]
+
+    pf = Profile(path=profile_path, create=False)
+
+    idnt.apply_preprocessing(preprocessing=pf["preprocessing"],
+                             options=pf["preprocessing_options"])
+    params = pf.get_fit_params()
+
+    idnt.fit_model(model_key=pf["model_key"],
+                   params_initial=params,
+                   range_type=pf["range_type"],
+                   range_x=pf["range_x"],
+                   segment=pf["segment"],
+                   weight_cp=pf["weight_cp"],
+                   )
+    return idnt
+
+
+def fit_parser():
+    descr = "Fit AFM force-distance data. Statistics (.tsv file) and " \
+            + "visualizations of the fits (multi-page .tif file) are stored " \
+            + "in the results directory."
+    parser = argparse.ArgumentParser(description=descr)
+    parser.add_argument('data_path', type=str,
+                        help='input folder containing AFM force-distance '
+                             + 'data')
+    parser.add_argument('out_dir', type=str,
+                        help='results directory')
+    return parser
+
+
+def generate_training_set_parser():
+    descr = "Create a training set for usage in nanite from rating " \
+            "containers (.h5 files manually created with `nanite-rate`)."
+    parser = argparse.ArgumentParser(description=descr)
+    parser.add_argument('data_path', type=str,
+                        help='path to a rating container or a folder '
+                             + 'containing rating containers')
+    parser.add_argument('out_dir', type=str,
+                        help='directory where the training set will be '
+                             ' stored')
+    return parser
+
+
+def generate_training_set():
+    parser = generate_training_set_parser()
+    args = parser.parse_args()
+    data_path = pathlib.Path(args.data_path).resolve()
+    out_dir = pathlib.Path(args.out_dir).resolve()
+    name = data_path.stem
+    if data_path.exists():
+        print("Generating training set '{}'.".format(name))
+        rm = rio.RateManager(data_path, verbose=1)
+        rm.export_training_set(out_dir / "ts_{}".format(name))
+    else:
+        print("Path does not exist: '{}'".format(data_path))
+
+
+def rate():
+    parser = rate_parser()
+    args = parser.parse_args()
+    path = pathlib.Path(args.data_path).resolve()
+    h5 = pathlib.Path(args.rating_path).resolve()
+    if not h5.name.endswith(".h5"):
+        h5 = h5.with_name(h5.name + ".h5")
+    # get all files in path
+    enumpaths = get_data_paths_enum(path, skip_errors=True)
+    # for now, only compare single curves
+    enumpaths = [ee for ee in enumpaths if ee[0].suffix == ".jpk-force"]
+    if TK_AVAILABLE:
+        # start GUI
+        root = tk.Tk()
+        RatingGUI(root, data_paths=enumpaths, h5path=h5)
+        root.mainloop()
+    else:
+        raise ValueError("tkinter is not available! (frozen application?)")
+
+
+def rate_parser():
+    descr = "Manually rate (the fit to) AFM force-distance data. " \
+            + "A graphical user interface allows to rate and comment on " \
+            + "each force-distance curve. The fits and the raw data are " \
+            + "stored in a rating container that can then be passed to " \
+            + "`nanite-generate-training-set`."
+    parser = argparse.ArgumentParser(description=descr)
+    parser.add_argument('data_path', type=str,
+                        help='input folder containing AFM force-distance '
+                             + 'data')
+    parser.add_argument('rating_path', type=str,
+                        help='path to the output rating container (will '
+                             + 'be created if it does not already exist)')
+    return parser
```

### Comparing `nanite-3.5.4/nanite/fit.py` & `nanite-3.6.0/nanite/fit.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,610 +1,610 @@
-import copy
-import hashlib
-import numbers
-import warnings
-
-import lmfit
-import numpy as np
-import scipy.signal as spsig
-
-from . import model
-
-
-FP_DEFAULT = dict(model_key="hertz_para",
-                  optimal_fit_edelta=False,
-                  optimal_fit_num_samples=100,
-                  params_initial=None,
-                  preprocessing=[],
-                  preprocessing_options={},
-                  range_type="absolute",
-                  range_x=[0, 0],
-                  segment=0,
-                  weight_cp=1e-6,
-                  gcf_k=1.0,
-                  x_axis="tip position",
-                  y_axis="force",
-                  method="leastsq",
-                  method_kws={},
-                  )
-
-FP_RESULTS = ["chi_sqr",
-              "hash",
-              "optimal_fit_delta_array",
-              "optimal_fit_delta",
-              "optimal_fit_E_array",
-              "params_fitted",
-              "success",
-              "xmax",
-              "xmin",
-              ]
-
-
-class FitKeyError(BaseException):
-    pass
-
-
-class FitDataError(BaseException):
-    pass
-
-
-class FitWarning(UserWarning):
-    pass
-
-
-class FitProperties(dict):
-    """Fit property manager class
-
-    Provide convenient access to fit properties as a dictionary
-    and dynamically manage resets due to new initial parameters.
-
-    Dynamic properties include:
-
-    - set "params_initial" to `None` if the "model_key" changes
-    - remove all keys except those in `FP_DEFAULT` if a key that is
-      in `FP_DEFAULT` changes (All other keys are considered to be
-      obsolete fitting results).
-
-    Additional attributes:
-    """
-
-    def __setitem__(self, key, value):
-        if key == "segment":
-            # Since version 1.8.0, nanite uses an integer to identify
-            # the segment. Replace the input accordingly for backwards
-            # compatibility.
-            if value == "approach":
-                value = 0
-            elif value == "retract":
-                value = 1
-        # Proceed with normal checks.
-        if key in FP_DEFAULT:
-            if (key in self
-                and key == "params_initial"
-                    and self["params_initial"] is not None
-                    and value is not None):
-                # check for changed initial parameters
-                for pp in self["params_initial"]:
-                    s1 = self["params_initial"][pp].__getstate__()
-                    s2 = value[pp].__getstate__()
-                    if s1 != s2:
-                        self.reset()
-                        break
-            elif key in self and self[key] == value:
-                # nothing to do, parameters match
-                pass
-            else:
-                if key == "model_key":
-                    # Other model has other parameters.
-                    self["params_initial"] = None
-                elif key == "range_x":
-                    if ("optimal_fit_edelta" in self and
-                        self["optimal_fit_edelta"] and
-                        "range_x" in self and
-                            self["range_x"][1] == value[1]):
-                        # Ignore changes in range[0]
-                        return
-                # Trigger `self.reset`
-                self.reset()
-        elif key not in FP_RESULTS:
-            msg = "Key '{}' not in FP_DEFAULT".format(key)
-            raise FitKeyError(msg)
-        super(FitProperties, self).__setitem__(key, value)
-
-    def reset(self):
-        for key in list(self.keys()):
-            if key not in FP_DEFAULT:
-                self.pop(key)
-
-    def restore(self, props):
-        """update the dictionary without removing any keys"""
-        for key in props:
-            super(FitProperties, self).__setitem__(key, props[key])
-
-
-class IndentationFitter(object):
-    def __init__(self, idnt, **kwargs):
-        """Fit force-distance curves
-
-        Parameters
-        ----------
-        idnt: nanite.indent.Indentation
-            The dataset to fit
-        model_key: str
-            A key referring to a model in
-            `nanite.model.models_available`
-        params_initial: instance of lmfit.Parameters
-            Parameters for fitting. If not given,
-            default parameters are used.
-        range_x: tuple of 2
-            The range for fitting, see `range_type` below.
-        range_type: str
-            One of:
-
-            - absolute:
-                Set the absolute fitting range in values
-                given by the `x_axis`.
-            - relative cp:
-                In some cases it is desired to be able to
-                fit a model only up until a certain indentation
-                depth (tip position) measured from the contact
-                point. Since the contact point is a fit parameter
-                as well, this requires a two-pass fitting.
-        preprocessing: list of str
-            Preprocessing step identifiers
-        preprocessing_options: dict of dicts
-            Preprocessing keyword arguments of steps (if applicable)
-        segment: int
-            Segment index (e.g. 0 for approach)
-        weight_cp: float
-            Weight the contact point region which shows artifacts
-            that are difficult to model with e.g. Hertz.
-        gcf_k: float
-            Geometrical correction factor :math:`k` for non-single-contact
-            data. The measured indentation is multiplied by this factor to
-            correct for experimental geometries during fitting,
-            e.g. ``gcf_k=0.5`` for parallel-place compression.
-        optimal_fit_edelta: bool
-            Search for the optimal fit by varying the maximal
-            indentation depth and determining a plateau in the
-            resulting Young's modulus (fitting parameter "E").
-        optimal_fit_num_samples: int
-            Number of samples to use for searching the optimal fit
-        """
-        # Get initial fit parameters
-        # IMPORTANT:
-        # If there are new additions in the default values,
-        # make sure to take these into account in `FP_DEFAULT`.
-        self.fp = FitProperties(**FP_DEFAULT)
-
-        # Get parameters from dataset
-        # (sorted, such that `model_key` is set before `params_initial`)
-        for key in sorted(idnt.fit_properties.keys()):
-            if key in FP_DEFAULT:
-                self.fp[key] = idnt.fit_properties[key]
-        # Get parameters from kwargs
-        # (sorted, such that `model_key` is set before `params_initial`)
-        for key in sorted(self.fp.keys()):
-            if key in kwargs:
-                if key not in FP_DEFAULT:
-                    msg = "Key '{}' not in FP_DEFAULT".format(key)
-                    raise FitKeyError(msg)
-                self.fp[key] = kwargs[key]
-        # Set initial fitting parameters
-        if self.fp["params_initial"] is None:
-            self.fp["params_initial"] = self.get_initial_parameters(
-                idnt=idnt,
-                model_key=self.fp["model_key"]
-            )
-
-        # Set arrays
-        self.segment = idnt["segment"] == self.fp["segment"]
-        self.segment.setflags(write=False)
-
-        self.x_axis = idnt[self.fp["x_axis"]]
-        self.x_axis.setflags(write=False)
-
-        self.y_axis = idnt[self.fp["y_axis"]]
-        self.y_axis.setflags(write=False)
-
-        self.fit_range = np.zeros_like(self.segment)
-        self.fit_curve = np.zeros_like(self.y_axis)
-        self.fit_residuals = np.zeros_like(self.y_axis)
-
-        # Fitting parameters might be changed due to iterative fitting.
-        # Store them in separate variables to prevent resetting the
-        # `FitPropreties` instance `self.fp`.
-        self.optimal_fit_edelta = self.fp["optimal_fit_edelta"]
-        self.range_type = self.fp["range_type"]
-        self.range_x = list(self.fp["range_x"])
-
-        self.hash = self._hash()
-        self.fp["hash"] = self.hash
-
-        # Perform sanity checks
-        if self.fp["range_type"] not in ["absolute", "relative cp"]:
-            msg = "`range_type` must be  'absolute' or 'relative cp'!"
-            raise FitKeyError(msg)
-        if len(self.fp["range_x"]) != 2:
-            raise FitKeyError("`range_x` must have length 2!")
-        if (np.isnan(self.fp["range_x"][0]) or
-                np.isnan(self.fp["range_x"][1])):
-            raise FitKeyError("`range_x` must not contain NaN!")
-        if not isinstance(self.fp["segment"], numbers.Integral):
-            raise FitKeyError(
-                f"`segment` must be integer, got '{self.fp['segment']}!")
-        if self.fp["model_key"] not in model.models_available:
-            msg = "unknown model '{}'".format(self.fp["model_key"])
-            raise FitKeyError(msg)
-
-        if self.fp["optimal_fit_edelta"]:
-            # Make sure we have emodulus
-            if "E" not in self.fp["params_initial"]:
-                msg = "Search for optimal fit requires the parameter 'E'!"
-                raise FitKeyError(msg)
-            # This only works with absolute range
-            if self.fp["range_type"] != "absolute":
-                msg = "Only absolute range relative to contact point allowed!"
-                raise FitKeyError(msg)
-
-        md_key = self.fp["model_key"]
-        md = model.models_available[md_key]
-        params = md.get_parameter_defaults()
-        for p in params:
-            msg = "Unknown fitting parameter '{}' for model '{}'!"
-            if p not in self.fp["params_initial"]:
-                raise FitKeyError(msg.format(p, md_key))
-
-        if self.fp["range_x"][0] > self.fp["range_x"][1]:
-            msg = "Fitting range is inverted: {}".format(self.fp["range_x"])
-            warnings.warn(msg, FitWarning)
-
-    def compute_emodulus_vs_mindelta(self, callback=None):
-        """Compute elastic modulus vs. minimal indentation curve"""
-        segid = self.segment
-        xseg = self.x_axis[segid]
-        yseg = self.y_axis[segid]
-
-        xmax = np.max(self.fp["range_x"])
-        if np.isinf(xmax):
-            xmax = np.max(xseg)
-        # Disable and remember `optimal_fit_edelta`
-        optimal_fit_edelta = self.optimal_fit_edelta
-        self.optimal_fit_edelta = False
-
-        # We are agnostic concerning the direction of indentation.
-        # `xseg` should start at the baseline.
-        seems_approach = np.average(yseg[:10]) < np.average(yseg[-10:])
-        if seems_approach and self.fp["segment"] == 0:
-            if xseg[0] < xseg[-1]:
-                msg = "Unexpected trend in approach x data!"
-                raise FitDataError(msg)
-        elif seems_approach:
-            msg = "Data appears to be 'approach', but is 'retract'!"
-            raise FitDataError(msg)
-        elif not seems_approach and self.fp["segment"] > 0:
-            if xseg[0] > xseg[-1]:
-                msg = "Unexpected trend in retract x data!"
-                raise FitDataError(msg)
-            msg = "Unexpected trend in retract curve!"
-            raise FitDataError(msg)
-        elif not seems_approach:
-            msg = "Data appears to be 'retract', but is 'approach'!"
-            raise FitDataError(msg)
-
-        # Fit the range of parameters
-        xmin = xseg.min()
-        if xmin >= 0:
-            msg = "No negative values (indentation) found! " \
-                  + "Did you correct for tip offset?"
-            raise FitKeyError(msg)
-        num_samp = self.fp["optimal_fit_num_samples"]
-        indentations = np.linspace(xmin, xmin*.05, num_samp)
-        emoduli = np.zeros_like(indentations)
-        for ii, x0 in enumerate(indentations):
-            # Perform a fit and record the elastic modulus
-            self.range_x = [x0, xmax]
-            self.fit()
-            emoduli[ii] = self.fp["params_fitted"]["E"].value
-            if callback and ii % 5 == 0:
-                callback(emoduli, indentations)
-
-        self.optimal_fit_edelta = optimal_fit_edelta
-
-        return emoduli, indentations
-
-    @staticmethod
-    def compute_opt_mindelta(emoduli, indentations):
-        """Determine the plateau of an emodulus-indentation curve
-
-        The following procedure is performed:
-
-        1. Smooth the emodulus data with a Butterworth filter
-        2. Label sequences that have similar values by binning
-           into ten regions between the min and max.
-        3. Ignore sequences with emodulus that is smaller than
-           the binning size.
-        4. Determine the longest sequence.
-        """
-        # Perform smoothing of the curve
-        # First, perform filtering with butterworth filter
-        nb = 1      # Filter order
-        wb = 0.05    # Cutoff frequency
-        b, a = spsig.butter(nb, wb, output='ba')
-        smooth_e = spsig.filtfilt(b, a, emoduli)
-        # Second, determine the longest sequence of values
-        # that have the same smoothed value.
-        ni = 10
-        ivals, istep = np.linspace(smooth_e.min(), smooth_e.max(), ni,
-                                   endpoint=False, retstep=True)
-        ivals += istep/2
-        labelarray = np.zeros_like(smooth_e, dtype=int)
-        valarray = np.zeros_like(smooth_e, dtype=int)
-        # label each sequence with an individual `idx`
-        for ii in range(smooth_e.shape[0]):
-            valid = np.argmin(np.abs(ivals - smooth_e[ii]))
-            if ii == 0:
-                idx = 0
-            elif valid == valarray[ii-1]:
-                pass
-            else:
-                idx += 1
-            labelarray[ii] = idx
-            valarray[ii] = valid
-        # Determine the longest sequence
-        counts = list(np.bincount(labelarray))
-        # Ignore values that are below cutoff
-
-        for ii in range(len(counts)):
-            labmax = np.argmax(counts)
-            labid = np.where(labelarray == labmax)[0][0]
-            valmax = ivals[valarray[labid]]
-            if valmax > istep:
-                break
-            counts.pop(labmax)
-        else:
-            # Nothing found: select the middle value
-            warnings.warn("Could not find correct plateau.", FitWarning)
-            labmax = 5
-        # Determine the interval in the original array
-        indices = np.where(labelarray == labmax)[0]
-        if len(indices) == 1:
-            dopt = indentations[indices[0]]
-        else:
-            # compute optimal indentation as center
-            dopt = np.average(indentations[indices[0]:indices[-1]])
-        return dopt
-
-    def _fit(self):
-        """Fit a model to the data
-
-        Notes
-        -----
-        This method is private because it requires the array
-        `self.fit_range` before the actual fitting.
-        """
-        model_key = self.fp["model_key"]
-        params_initial = self.fp["params_initial"]
-        # modify contact point with gcf_k
-        cpi = params_initial["contact_point"].value
-        params_initial["contact_point"].set(value=cpi * self.fp["gcf_k"])
-        weight_cp = self.fp["weight_cp"]
-
-        # boolean array indexing the segment
-        segid = self.segment
-        # x: the entire segment (correct with gcf_k)
-        xseg = self.x_axis[segid] * self.fp["gcf_k"]
-        # y: the entire segment
-        yseg = self.y_axis[segid]
-        # x: the values being fitted (correct with gcf_k)
-        x = self.x_axis[self.fit_range] * self.fp["gcf_k"]
-        # y: the values being fitted
-        y = self.y_axis[self.fit_range]
-
-        md = model.models_available[model_key]
-
-        # short reference for better readability
-        fit_cur = self.fit_curve
-        fit_res = self.fit_residuals
-
-        # reset values to nan
-        fit_cur[:] = np.nan
-        fit_res[:] = np.nan
-
-        # Make sure that we can actually fit by comparing variable fitting
-        # parameters and size of x.
-        npvaried = np.sum([p[1].vary for p in list(params_initial.items())])
-        if npvaried < x.shape[0] - 1:
-            # perform fit
-            fit = lmfit.minimize(
-                fcn=md.residual,
-                params=params_initial,
-                method=self.fp["method"],
-                args=(x, y, weight_cp),
-                **self.fp["method_kws"],
-                )
-            # fitted method
-            fit_cur[segid] = md.model(fit.params, xseg)
-            # residuals
-            fit_res[segid] = md.residual(fit.params, xseg, yseg, weight_cp)
-            # inverse contact point correction with gcf_k
-            cpf = fit.params["contact_point"].value
-            fit.params["contact_point"].set(value=cpf / self.fp["gcf_k"])
-            # add fit results to fp dictionary
-            self.fp.update({"params_fitted": fit.params,
-                            "chi_sqr": fit.chisqr,
-                            "xmin": x.min() / self.fp["gcf_k"],
-                            "xmax": x.max() / self.fp["gcf_k"],
-                            "success": True,
-                            })
-        else:
-            self.fp["success"] = False
-
-    def fit(self):
-        """Fit the approach-retract data to a model function
-        """
-        range_type = self.range_type
-        range_x = copy.copy(self.range_x)
-        # Set to True in `self._fit`
-        self.fp["success"] = False
-
-        if self.optimal_fit_edelta:
-            # emodulus-indentation curve:
-            emoduli, indentations = self.compute_emodulus_vs_mindelta()
-            # determine optimal x0
-            dopt = self.compute_opt_mindelta(emoduli, indentations)
-            # add indentations/emoduli to self.fp
-            self.fp["optimal_fit_E_array"] = emoduli
-            self.fp["optimal_fit_delta_array"] = indentations
-            self.fp["optimal_fit_delta"] = dopt
-            # update fitting parameters for final fit
-            self.range_x = [dopt, np.max(self.fp["range_x"])]
-            # perform final fit
-            self.optimal_fit_edelta = False
-            self.fit()
-            self.optimal_fit_edelta = True
-
-        elif self.range_type == "absolute":
-            # This is easy. Simply set the boolean array of fitting values
-            # Exclude data points from other segment
-            if range_x[0] != range_x[1]:
-                x_data = self.x_axis.copy()
-                range_bool = self.segment.copy()
-                rmin, rmax = np.min(range_x), np.max(range_x)
-                range_bool[x_data < rmin] = False
-                range_bool[x_data > rmax] = False
-            else:
-                range_bool = self.segment
-            self.fit_range[:] = range_bool
-            self._fit()
-
-        elif range_type == "relative cp":
-            # Let's try to solve this with four passes
-            # First, get the approximate contact point
-            self.range_type = "absolute"
-            # Set full range to get estimate of cp
-            self.range_x = [0, 0]
-            self.fit()
-            # Do the following three-times.
-            for _i in range(3):
-                # get the fitted contact point
-                cp = self.fp["params_fitted"]["contact_point"].value
-                self.range_x = list(np.array(range_x)+cp)
-                # Second, fit with the new contact point as range parameters
-                self.fit()
-
-        # Reset range data to original values
-        self.range_type = range_type
-        self.range_x = range_x
-
-    def get_initial_parameters(self, idnt=None,
-                               model_key=FP_DEFAULT["model_key"]):
-        """Get initial fit parameters for a specific model
-
-        Parameters
-        ----------
-
-        """
-        if (model_key == self.fp["model_key"] and
-                self.fp["params_initial"] is not None):
-            params = self.fp["params_initial"]
-        else:
-            params = guess_initial_parameters(idnt=idnt, model_key=model_key)
-        return params
-
-    def _hash(self):
-        """Compute hash identifier for current fit
-
-        The hash is computed without applying the fit, making
-        it suitable for caching fits.
-        """
-        hashlist = []
-        # preprocessing
-        hashlist.append(self.fp["preprocessing"])
-        hashlist.append(self.fp["preprocessing_options"])
-        # axes data
-        hashlist.append(self.x_axis)
-        hashlist.append(self.y_axis)
-        # fit parameters
-        for key in FP_DEFAULT:
-            if (key == "range_x" and
-                    self.fp["optimal_fit_edelta"]):
-                # range only partly if "optimal_fit_edelta" is True
-                hashlist.append(self.fp["range_x"][1])
-            elif (key == "optimal_fit_num_samples" and
-                  not self.fp["optimal_fit_edelta"]):
-                # ignore number of samples if optimal fit is not used
-                pass
-            else:
-                hashlist.append(self.fp[key])
-        # join and hash
-        myhash = hashlib.md5(obj2bytes(hashlist)).hexdigest()
-        return myhash
-
-
-def guess_initial_parameters(idnt=None,
-                             model_key=FP_DEFAULT["model_key"],
-                             common_ancillaries=True,
-                             model_ancillaries=True):
-    """Guess initial fitting parameters
-
-    Parameters
-    ----------
-    idnt: nanite.indent.Indentation
-        The dataset to use for guessing initial fitting parameters
-        using ancillary parameters
-    model_key: str
-        The model key
-    common_ancillaries: bool
-        Guess global ancillary parameters (such as contact point)
-    model_ancillaries: bool
-        Use model-related ancillary parameters
-    """
-    md = model.models_available[model_key]
-    params = md.get_parameter_defaults()
-    if common_ancillaries and idnt is not None:
-        # Guess initial contact point from actual tip position
-        # (see `self.compute_tip_position`)
-        # Depending on how the current dataset was pre-processed,
-        # the column "tip position" might already be corrected by
-        # an estimated contact point offset.
-        # (see `self.compute_tip_offset`)
-        if "tip position" in idnt:
-            cpid = idnt.estimate_contact_point_index()
-            cp = idnt["tip position"][cpid]
-            params["contact_point"].set(cp)
-        else:
-            msg = "Cannot estimate contact point, because of missing "\
-                  + "column 'tip position'"
-            warnings.warn(msg, FitWarning)
-    if model_ancillaries and idnt is not None:
-        anc_dict = idnt.get_ancillary_parameters()
-        # set the parameter values
-        for anckey in anc_dict:
-            if anckey in params:
-                if not np.isnan(anc_dict[anckey]):  # ignore nans
-                    params[anckey].set(value=anc_dict[anckey])
-    return params
-
-
-def obj2bytes(obj):
-    """Bytes representation of an object for hashing"""
-    if isinstance(obj, str):
-        return obj.encode("utf-8")
-    elif isinstance(obj, (bool, int, float, np.bool_)):
-        return str(float(obj)).encode("utf-8")
-    elif obj is None:
-        return b"none"
-    elif isinstance(obj, np.ndarray):
-        return obj.tobytes()
-    elif isinstance(obj, tuple):
-        return obj2bytes(list(obj))
-    elif isinstance(obj, list):
-        return b"".join(obj2bytes(o) for o in obj)
-    elif isinstance(obj, dict):
-        return obj2bytes(sorted(obj.items()))
-    elif isinstance(obj, lmfit.parameter.Parameter):
-        return obj2bytes([obj.value, obj.max, obj.min, obj.vary,
-                          obj.expr, obj.name])
-    else:
-        raise ValueError("No rule to convert object '{}' to string.".
-                         format(obj.__class__))
+import copy
+import hashlib
+import numbers
+import warnings
+
+import lmfit
+import numpy as np
+import scipy.signal as spsig
+
+from . import model
+
+
+FP_DEFAULT = dict(model_key="hertz_para",
+                  optimal_fit_edelta=False,
+                  optimal_fit_num_samples=100,
+                  params_initial=None,
+                  preprocessing=[],
+                  preprocessing_options={},
+                  range_type="absolute",
+                  range_x=[0, 0],
+                  segment=0,
+                  weight_cp=1e-6,
+                  gcf_k=1.0,
+                  x_axis="tip position",
+                  y_axis="force",
+                  method="leastsq",
+                  method_kws={},
+                  )
+
+FP_RESULTS = ["chi_sqr",
+              "hash",
+              "optimal_fit_delta_array",
+              "optimal_fit_delta",
+              "optimal_fit_E_array",
+              "params_fitted",
+              "success",
+              "xmax",
+              "xmin",
+              ]
+
+
+class FitKeyError(BaseException):
+    pass
+
+
+class FitDataError(BaseException):
+    pass
+
+
+class FitWarning(UserWarning):
+    pass
+
+
+class FitProperties(dict):
+    """Fit property manager class
+
+    Provide convenient access to fit properties as a dictionary
+    and dynamically manage resets due to new initial parameters.
+
+    Dynamic properties include:
+
+    - set "params_initial" to `None` if the "model_key" changes
+    - remove all keys except those in `FP_DEFAULT` if a key that is
+      in `FP_DEFAULT` changes (All other keys are considered to be
+      obsolete fitting results).
+
+    Additional attributes:
+    """
+
+    def __setitem__(self, key, value):
+        if key == "segment":
+            # Since version 1.8.0, nanite uses an integer to identify
+            # the segment. Replace the input accordingly for backwards
+            # compatibility.
+            if value == "approach":
+                value = 0
+            elif value == "retract":
+                value = 1
+        # Proceed with normal checks.
+        if key in FP_DEFAULT:
+            if (key in self
+                and key == "params_initial"
+                    and self["params_initial"] is not None
+                    and value is not None):
+                # check for changed initial parameters
+                for pp in self["params_initial"]:
+                    s1 = self["params_initial"][pp].__getstate__()
+                    s2 = value[pp].__getstate__()
+                    if s1 != s2:
+                        self.reset()
+                        break
+            elif key in self and self[key] == value:
+                # nothing to do, parameters match
+                pass
+            else:
+                if key == "model_key":
+                    # Other model has other parameters.
+                    self["params_initial"] = None
+                elif key == "range_x":
+                    if ("optimal_fit_edelta" in self and
+                        self["optimal_fit_edelta"] and
+                        "range_x" in self and
+                            self["range_x"][1] == value[1]):
+                        # Ignore changes in range[0]
+                        return
+                # Trigger `self.reset`
+                self.reset()
+        elif key not in FP_RESULTS:
+            msg = "Key '{}' not in FP_DEFAULT".format(key)
+            raise FitKeyError(msg)
+        super(FitProperties, self).__setitem__(key, value)
+
+    def reset(self):
+        for key in list(self.keys()):
+            if key not in FP_DEFAULT:
+                self.pop(key)
+
+    def restore(self, props):
+        """update the dictionary without removing any keys"""
+        for key in props:
+            super(FitProperties, self).__setitem__(key, props[key])
+
+
+class IndentationFitter(object):
+    def __init__(self, idnt, **kwargs):
+        """Fit force-distance curves
+
+        Parameters
+        ----------
+        idnt: nanite.indent.Indentation
+            The dataset to fit
+        model_key: str
+            A key referring to a model in
+            `nanite.model.models_available`
+        params_initial: instance of lmfit.Parameters
+            Parameters for fitting. If not given,
+            default parameters are used.
+        range_x: tuple of 2
+            The range for fitting, see `range_type` below.
+        range_type: str
+            One of:
+
+            - absolute:
+                Set the absolute fitting range in values
+                given by the `x_axis`.
+            - relative cp:
+                In some cases it is desired to be able to
+                fit a model only up until a certain indentation
+                depth (tip position) measured from the contact
+                point. Since the contact point is a fit parameter
+                as well, this requires a two-pass fitting.
+        preprocessing: list of str
+            Preprocessing step identifiers
+        preprocessing_options: dict of dicts
+            Preprocessing keyword arguments of steps (if applicable)
+        segment: int
+            Segment index (e.g. 0 for approach)
+        weight_cp: float
+            Weight the contact point region which shows artifacts
+            that are difficult to model with e.g. Hertz.
+        gcf_k: float
+            Geometrical correction factor :math:`k` for non-single-contact
+            data. The measured indentation is multiplied by this factor to
+            correct for experimental geometries during fitting,
+            e.g. ``gcf_k=0.5`` for parallel-place compression.
+        optimal_fit_edelta: bool
+            Search for the optimal fit by varying the maximal
+            indentation depth and determining a plateau in the
+            resulting Young's modulus (fitting parameter "E").
+        optimal_fit_num_samples: int
+            Number of samples to use for searching the optimal fit
+        """
+        # Get initial fit parameters
+        # IMPORTANT:
+        # If there are new additions in the default values,
+        # make sure to take these into account in `FP_DEFAULT`.
+        self.fp = FitProperties(**FP_DEFAULT)
+
+        # Get parameters from dataset
+        # (sorted, such that `model_key` is set before `params_initial`)
+        for key in sorted(idnt.fit_properties.keys()):
+            if key in FP_DEFAULT:
+                self.fp[key] = idnt.fit_properties[key]
+        # Get parameters from kwargs
+        # (sorted, such that `model_key` is set before `params_initial`)
+        for key in sorted(self.fp.keys()):
+            if key in kwargs:
+                if key not in FP_DEFAULT:
+                    msg = "Key '{}' not in FP_DEFAULT".format(key)
+                    raise FitKeyError(msg)
+                self.fp[key] = kwargs[key]
+        # Set initial fitting parameters
+        if self.fp["params_initial"] is None:
+            self.fp["params_initial"] = self.get_initial_parameters(
+                idnt=idnt,
+                model_key=self.fp["model_key"]
+            )
+
+        # Set arrays
+        self.segment = idnt["segment"] == self.fp["segment"]
+        self.segment.setflags(write=False)
+
+        self.x_axis = idnt[self.fp["x_axis"]]
+        self.x_axis.setflags(write=False)
+
+        self.y_axis = idnt[self.fp["y_axis"]]
+        self.y_axis.setflags(write=False)
+
+        self.fit_range = np.zeros_like(self.segment)
+        self.fit_curve = np.zeros_like(self.y_axis)
+        self.fit_residuals = np.zeros_like(self.y_axis)
+
+        # Fitting parameters might be changed due to iterative fitting.
+        # Store them in separate variables to prevent resetting the
+        # `FitPropreties` instance `self.fp`.
+        self.optimal_fit_edelta = self.fp["optimal_fit_edelta"]
+        self.range_type = self.fp["range_type"]
+        self.range_x = list(self.fp["range_x"])
+
+        self.hash = self._hash()
+        self.fp["hash"] = self.hash
+
+        # Perform sanity checks
+        if self.fp["range_type"] not in ["absolute", "relative cp"]:
+            msg = "`range_type` must be  'absolute' or 'relative cp'!"
+            raise FitKeyError(msg)
+        if len(self.fp["range_x"]) != 2:
+            raise FitKeyError("`range_x` must have length 2!")
+        if (np.isnan(self.fp["range_x"][0]) or
+                np.isnan(self.fp["range_x"][1])):
+            raise FitKeyError("`range_x` must not contain NaN!")
+        if not isinstance(self.fp["segment"], numbers.Integral):
+            raise FitKeyError(
+                f"`segment` must be integer, got '{self.fp['segment']}!")
+        if self.fp["model_key"] not in model.models_available:
+            msg = "unknown model '{}'".format(self.fp["model_key"])
+            raise FitKeyError(msg)
+
+        if self.fp["optimal_fit_edelta"]:
+            # Make sure we have emodulus
+            if "E" not in self.fp["params_initial"]:
+                msg = "Search for optimal fit requires the parameter 'E'!"
+                raise FitKeyError(msg)
+            # This only works with absolute range
+            if self.fp["range_type"] != "absolute":
+                msg = "Only absolute range relative to contact point allowed!"
+                raise FitKeyError(msg)
+
+        md_key = self.fp["model_key"]
+        md = model.models_available[md_key]
+        params = md.get_parameter_defaults()
+        for p in params:
+            msg = "Unknown fitting parameter '{}' for model '{}'!"
+            if p not in self.fp["params_initial"]:
+                raise FitKeyError(msg.format(p, md_key))
+
+        if self.fp["range_x"][0] > self.fp["range_x"][1]:
+            msg = "Fitting range is inverted: {}".format(self.fp["range_x"])
+            warnings.warn(msg, FitWarning)
+
+    def compute_emodulus_vs_mindelta(self, callback=None):
+        """Compute elastic modulus vs. minimal indentation curve"""
+        segid = self.segment
+        xseg = self.x_axis[segid]
+        yseg = self.y_axis[segid]
+
+        xmax = np.max(self.fp["range_x"])
+        if np.isinf(xmax):
+            xmax = np.max(xseg)
+        # Disable and remember `optimal_fit_edelta`
+        optimal_fit_edelta = self.optimal_fit_edelta
+        self.optimal_fit_edelta = False
+
+        # We are agnostic concerning the direction of indentation.
+        # `xseg` should start at the baseline.
+        seems_approach = np.average(yseg[:10]) < np.average(yseg[-10:])
+        if seems_approach and self.fp["segment"] == 0:
+            if xseg[0] < xseg[-1]:
+                msg = "Unexpected trend in approach x data!"
+                raise FitDataError(msg)
+        elif seems_approach:
+            msg = "Data appears to be 'approach', but is 'retract'!"
+            raise FitDataError(msg)
+        elif not seems_approach and self.fp["segment"] > 0:
+            if xseg[0] > xseg[-1]:
+                msg = "Unexpected trend in retract x data!"
+                raise FitDataError(msg)
+            msg = "Unexpected trend in retract curve!"
+            raise FitDataError(msg)
+        elif not seems_approach:
+            msg = "Data appears to be 'retract', but is 'approach'!"
+            raise FitDataError(msg)
+
+        # Fit the range of parameters
+        xmin = xseg.min()
+        if xmin >= 0:
+            msg = "No negative values (indentation) found! " \
+                  + "Did you correct for tip offset?"
+            raise FitKeyError(msg)
+        num_samp = self.fp["optimal_fit_num_samples"]
+        indentations = np.linspace(xmin, xmin*.05, num_samp)
+        emoduli = np.zeros_like(indentations)
+        for ii, x0 in enumerate(indentations):
+            # Perform a fit and record the elastic modulus
+            self.range_x = [x0, xmax]
+            self.fit()
+            emoduli[ii] = self.fp["params_fitted"]["E"].value
+            if callback and ii % 5 == 0:
+                callback(emoduli, indentations)
+
+        self.optimal_fit_edelta = optimal_fit_edelta
+
+        return emoduli, indentations
+
+    @staticmethod
+    def compute_opt_mindelta(emoduli, indentations):
+        """Determine the plateau of an emodulus-indentation curve
+
+        The following procedure is performed:
+
+        1. Smooth the emodulus data with a Butterworth filter
+        2. Label sequences that have similar values by binning
+           into ten regions between the min and max.
+        3. Ignore sequences with emodulus that is smaller than
+           the binning size.
+        4. Determine the longest sequence.
+        """
+        # Perform smoothing of the curve
+        # First, perform filtering with butterworth filter
+        nb = 1      # Filter order
+        wb = 0.05    # Cutoff frequency
+        b, a = spsig.butter(nb, wb, output='ba')
+        smooth_e = spsig.filtfilt(b, a, emoduli)
+        # Second, determine the longest sequence of values
+        # that have the same smoothed value.
+        ni = 10
+        ivals, istep = np.linspace(smooth_e.min(), smooth_e.max(), ni,
+                                   endpoint=False, retstep=True)
+        ivals += istep/2
+        labelarray = np.zeros_like(smooth_e, dtype=int)
+        valarray = np.zeros_like(smooth_e, dtype=int)
+        # label each sequence with an individual `idx`
+        for ii in range(smooth_e.shape[0]):
+            valid = np.argmin(np.abs(ivals - smooth_e[ii]))
+            if ii == 0:
+                idx = 0
+            elif valid == valarray[ii-1]:
+                pass
+            else:
+                idx += 1
+            labelarray[ii] = idx
+            valarray[ii] = valid
+        # Determine the longest sequence
+        counts = list(np.bincount(labelarray))
+        # Ignore values that are below cutoff
+
+        for ii in range(len(counts)):
+            labmax = np.argmax(counts)
+            labid = np.where(labelarray == labmax)[0][0]
+            valmax = ivals[valarray[labid]]
+            if valmax > istep:
+                break
+            counts.pop(labmax)
+        else:
+            # Nothing found: select the middle value
+            warnings.warn("Could not find correct plateau.", FitWarning)
+            labmax = 5
+        # Determine the interval in the original array
+        indices = np.where(labelarray == labmax)[0]
+        if len(indices) == 1:
+            dopt = indentations[indices[0]]
+        else:
+            # compute optimal indentation as center
+            dopt = np.average(indentations[indices[0]:indices[-1]])
+        return dopt
+
+    def _fit(self):
+        """Fit a model to the data
+
+        Notes
+        -----
+        This method is private because it requires the array
+        `self.fit_range` before the actual fitting.
+        """
+        model_key = self.fp["model_key"]
+        params_initial = self.fp["params_initial"]
+        # modify contact point with gcf_k
+        cpi = params_initial["contact_point"].value
+        params_initial["contact_point"].set(value=cpi * self.fp["gcf_k"])
+        weight_cp = self.fp["weight_cp"]
+
+        # boolean array indexing the segment
+        segid = self.segment
+        # x: the entire segment (correct with gcf_k)
+        xseg = self.x_axis[segid] * self.fp["gcf_k"]
+        # y: the entire segment
+        yseg = self.y_axis[segid]
+        # x: the values being fitted (correct with gcf_k)
+        x = self.x_axis[self.fit_range] * self.fp["gcf_k"]
+        # y: the values being fitted
+        y = self.y_axis[self.fit_range]
+
+        md = model.models_available[model_key]
+
+        # short reference for better readability
+        fit_cur = self.fit_curve
+        fit_res = self.fit_residuals
+
+        # reset values to nan
+        fit_cur[:] = np.nan
+        fit_res[:] = np.nan
+
+        # Make sure that we can actually fit by comparing variable fitting
+        # parameters and size of x.
+        npvaried = np.sum([p[1].vary for p in list(params_initial.items())])
+        if npvaried < x.shape[0] - 1:
+            # perform fit
+            fit = lmfit.minimize(
+                fcn=md.residual,
+                params=params_initial,
+                method=self.fp["method"],
+                args=(x, y, weight_cp),
+                **self.fp["method_kws"],
+                )
+            # fitted method
+            fit_cur[segid] = md.model(fit.params, xseg)
+            # residuals
+            fit_res[segid] = md.residual(fit.params, xseg, yseg, weight_cp)
+            # inverse contact point correction with gcf_k
+            cpf = fit.params["contact_point"].value
+            fit.params["contact_point"].set(value=cpf / self.fp["gcf_k"])
+            # add fit results to fp dictionary
+            self.fp.update({"params_fitted": fit.params,
+                            "chi_sqr": fit.chisqr,
+                            "xmin": x.min() / self.fp["gcf_k"],
+                            "xmax": x.max() / self.fp["gcf_k"],
+                            "success": True,
+                            })
+        else:
+            self.fp["success"] = False
+
+    def fit(self):
+        """Fit the approach-retract data to a model function
+        """
+        range_type = self.range_type
+        range_x = copy.copy(self.range_x)
+        # Set to True in `self._fit`
+        self.fp["success"] = False
+
+        if self.optimal_fit_edelta:
+            # emodulus-indentation curve:
+            emoduli, indentations = self.compute_emodulus_vs_mindelta()
+            # determine optimal x0
+            dopt = self.compute_opt_mindelta(emoduli, indentations)
+            # add indentations/emoduli to self.fp
+            self.fp["optimal_fit_E_array"] = emoduli
+            self.fp["optimal_fit_delta_array"] = indentations
+            self.fp["optimal_fit_delta"] = dopt
+            # update fitting parameters for final fit
+            self.range_x = [dopt, np.max(self.fp["range_x"])]
+            # perform final fit
+            self.optimal_fit_edelta = False
+            self.fit()
+            self.optimal_fit_edelta = True
+
+        elif self.range_type == "absolute":
+            # This is easy. Simply set the boolean array of fitting values
+            # Exclude data points from other segment
+            if range_x[0] != range_x[1]:
+                x_data = self.x_axis.copy()
+                range_bool = self.segment.copy()
+                rmin, rmax = np.min(range_x), np.max(range_x)
+                range_bool[x_data < rmin] = False
+                range_bool[x_data > rmax] = False
+            else:
+                range_bool = self.segment
+            self.fit_range[:] = range_bool
+            self._fit()
+
+        elif range_type == "relative cp":
+            # Let's try to solve this with four passes
+            # First, get the approximate contact point
+            self.range_type = "absolute"
+            # Set full range to get estimate of cp
+            self.range_x = [0, 0]
+            self.fit()
+            # Do the following three-times.
+            for _i in range(3):
+                # get the fitted contact point
+                cp = self.fp["params_fitted"]["contact_point"].value
+                self.range_x = list(np.array(range_x)+cp)
+                # Second, fit with the new contact point as range parameters
+                self.fit()
+
+        # Reset range data to original values
+        self.range_type = range_type
+        self.range_x = range_x
+
+    def get_initial_parameters(self, idnt=None,
+                               model_key=FP_DEFAULT["model_key"]):
+        """Get initial fit parameters for a specific model
+
+        Parameters
+        ----------
+
+        """
+        if (model_key == self.fp["model_key"] and
+                self.fp["params_initial"] is not None):
+            params = self.fp["params_initial"]
+        else:
+            params = guess_initial_parameters(idnt=idnt, model_key=model_key)
+        return params
+
+    def _hash(self):
+        """Compute hash identifier for current fit
+
+        The hash is computed without applying the fit, making
+        it suitable for caching fits.
+        """
+        hashlist = []
+        # preprocessing
+        hashlist.append(self.fp["preprocessing"])
+        hashlist.append(self.fp["preprocessing_options"])
+        # axes data
+        hashlist.append(self.x_axis)
+        hashlist.append(self.y_axis)
+        # fit parameters
+        for key in FP_DEFAULT:
+            if (key == "range_x" and
+                    self.fp["optimal_fit_edelta"]):
+                # range only partly if "optimal_fit_edelta" is True
+                hashlist.append(self.fp["range_x"][1])
+            elif (key == "optimal_fit_num_samples" and
+                  not self.fp["optimal_fit_edelta"]):
+                # ignore number of samples if optimal fit is not used
+                pass
+            else:
+                hashlist.append(self.fp[key])
+        # join and hash
+        myhash = hashlib.md5(obj2bytes(hashlist)).hexdigest()
+        return myhash
+
+
+def guess_initial_parameters(idnt=None,
+                             model_key=FP_DEFAULT["model_key"],
+                             common_ancillaries=True,
+                             model_ancillaries=True):
+    """Guess initial fitting parameters
+
+    Parameters
+    ----------
+    idnt: nanite.indent.Indentation
+        The dataset to use for guessing initial fitting parameters
+        using ancillary parameters
+    model_key: str
+        The model key
+    common_ancillaries: bool
+        Guess global ancillary parameters (such as contact point)
+    model_ancillaries: bool
+        Use model-related ancillary parameters
+    """
+    md = model.models_available[model_key]
+    params = md.get_parameter_defaults()
+    if common_ancillaries and idnt is not None:
+        # Guess initial contact point from actual tip position
+        # (see `self.compute_tip_position`)
+        # Depending on how the current dataset was pre-processed,
+        # the column "tip position" might already be corrected by
+        # an estimated contact point offset.
+        # (see `self.compute_tip_offset`)
+        if "tip position" in idnt:
+            cpid = idnt.estimate_contact_point_index()
+            cp = idnt["tip position"][cpid]
+            params["contact_point"].set(cp)
+        else:
+            msg = "Cannot estimate contact point, because of missing "\
+                  + "column 'tip position'"
+            warnings.warn(msg, FitWarning)
+    if model_ancillaries and idnt is not None:
+        anc_dict = idnt.get_ancillary_parameters()
+        # set the parameter values
+        for anckey in anc_dict:
+            if anckey in params:
+                if not np.isnan(anc_dict[anckey]):  # ignore nans
+                    params[anckey].set(value=anc_dict[anckey])
+    return params
+
+
+def obj2bytes(obj):
+    """Bytes representation of an object for hashing"""
+    if isinstance(obj, str):
+        return obj.encode("utf-8")
+    elif isinstance(obj, (bool, int, float, np.bool_)):
+        return str(float(obj)).encode("utf-8")
+    elif obj is None:
+        return b"none"
+    elif isinstance(obj, np.ndarray):
+        return obj.tobytes()
+    elif isinstance(obj, tuple):
+        return obj2bytes(list(obj))
+    elif isinstance(obj, list):
+        return b"".join(obj2bytes(o) for o in obj)
+    elif isinstance(obj, dict):
+        return obj2bytes(sorted(obj.items()))
+    elif isinstance(obj, lmfit.parameter.Parameter):
+        return obj2bytes([obj.value, obj.max, obj.min, obj.vary,
+                          obj.expr, obj.name])
+    else:
+        raise ValueError("No rule to convert object '{}' to string.".
+                         format(obj.__class__))
```

### Comparing `nanite-3.5.4/nanite/group.py` & `nanite-3.6.0/nanite/group.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-import pathlib
-
-import afmformats
-from afmformats.errors import MissingMetaDataError
-
-from .read import get_load_data_modality_kwargs, load_data
-
-
-def load_group(path, callback=None, meta_override=None):
-    """Load indentation data from disk
-
-    Parameters
-    ----------
-    path: path-like
-        Path to experimental data
-    callback: callable
-        function for tracking progress; must accept a float in
-        [0, 1] as an argument.
-    meta_override: dict
-        if specified, contains key-value pairs of metadata that
-        should be used when loading the files
-        (see :data:`afmformats.meta.META_FIELDS`)
-
-    Returns
-    -------
-    group: nanite.IndetationGroup
-        Indentation group with force-distance data
-    """
-    path = pathlib.Path(path)
-    data = load_data(path,
-                     callback=callback,
-                     meta_override=meta_override,
-                     )
-    grp = IndentationGroup()
-    grp += data
-    grp.path = path
-    return grp
-
-
-class IndentationGroup(afmformats.AFMGroup):
-    def __init__(self, path=None, meta_override=None, callback=None):
-        """Group of Indentation
-
-        Parameters
-        ----------
-        path: str or pathlib.Path or None
-            The path to the data file. The data format is determined
-            and the file is loaded using :ref:`afmformats:index`.
-        meta_override: dict
-            if specified, contains key-value pairs of metadata that
-            should be used when loading the files
-            (see :data:`afmformats.meta.META_FIELDS`)
-        callback: callable or None
-            A method that accepts a float between 0 and 1
-            to externally track the process of loading the data.
-        """
-        super(IndentationGroup, self).__init__(
-            path=path,
-            meta_override=meta_override,
-            callback=callback,
-            **get_load_data_modality_kwargs()
-        )
-
-    def append(self, afmdata):
-        """Append a new instance of AFMData
-
-        This subclassed method makes sure that "spring constant" is set
-        if "tip position" has to be computed in the future.
-
-        Parameters
-        ----------
-        afmdata: afmformats.afm_data.AFMData
-            AFM data
-        """
-        if ("spring constant" not in afmdata.metadata
-                and "tip position" not in afmdata):
-            raise MissingMetaDataError(
-                ["spring constant"],
-                "Please specify the spring constant!")
-        # Call the original function
-        super(IndentationGroup, self).append(afmdata)
+import pathlib
+
+import afmformats
+from afmformats.errors import MissingMetaDataError
+
+from .read import get_load_data_modality_kwargs, load_data
+
+
+def load_group(path, callback=None, meta_override=None):
+    """Load indentation data from disk
+
+    Parameters
+    ----------
+    path: path-like
+        Path to experimental data
+    callback: callable
+        function for tracking progress; must accept a float in
+        [0, 1] as an argument.
+    meta_override: dict
+        if specified, contains key-value pairs of metadata that
+        should be used when loading the files
+        (see :data:`afmformats.meta.META_FIELDS`)
+
+    Returns
+    -------
+    group: nanite.IndetationGroup
+        Indentation group with force-distance data
+    """
+    path = pathlib.Path(path)
+    data = load_data(path,
+                     callback=callback,
+                     meta_override=meta_override,
+                     )
+    grp = IndentationGroup()
+    grp += data
+    grp.path = path
+    return grp
+
+
+class IndentationGroup(afmformats.AFMGroup):
+    def __init__(self, path=None, meta_override=None, callback=None):
+        """Group of Indentation
+
+        Parameters
+        ----------
+        path: str or pathlib.Path or None
+            The path to the data file. The data format is determined
+            and the file is loaded using :ref:`afmformats:index`.
+        meta_override: dict
+            if specified, contains key-value pairs of metadata that
+            should be used when loading the files
+            (see :data:`afmformats.meta.META_FIELDS`)
+        callback: callable or None
+            A method that accepts a float between 0 and 1
+            to externally track the process of loading the data.
+        """
+        super(IndentationGroup, self).__init__(
+            path=path,
+            meta_override=meta_override,
+            callback=callback,
+            **get_load_data_modality_kwargs()
+        )
+
+    def append(self, afmdata):
+        """Append a new instance of AFMData
+
+        This subclassed method makes sure that "spring constant" is set
+        if "tip position" has to be computed in the future.
+
+        Parameters
+        ----------
+        afmdata: afmformats.afm_data.AFMData
+            AFM data
+        """
+        if ("spring constant" not in afmdata.metadata
+                and "tip position" not in afmdata):
+            raise MissingMetaDataError(
+                ["spring constant"],
+                "Please specify the spring constant!")
+        # Call the original function
+        super(IndentationGroup, self).append(afmdata)
```

### Comparing `nanite-3.5.4/nanite/indent.py` & `nanite-3.6.0/nanite/indent.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,379 +1,379 @@
-from collections import OrderedDict
-import copy
-import warnings
-
-import afmformats
-import numpy as np
-
-from .fit import IndentationFitter, FitProperties, guess_initial_parameters, \
-    FP_DEFAULT
-from . import model
-from . import poc
-from . import preproc
-from .rate import get_rater
-
-
-class Indentation(afmformats.AFMForceDistance):
-    def __init__(self, data, metadata, diskcache=None):
-        """Additional functionalities for afmformats.AFMForceDistance"""
-        super(Indentation, self).__init__(data=data,
-                                          metadata=metadata,
-                                          diskcache=diskcache)
-        #: Default preprocessing steps,
-        #: see :func:`Indentation.apply_preprocessing`.
-        self.preprocessing = []
-        #: Preprocessing options
-        self.preprocessing_options = {}
-        # preprocessing details (for user convenience)
-        self._preprocessing_details = {}
-        # protected fit properties
-        self._fit_properties = FitProperties()
-
-        # Curve rating (see `self.rate_quality`)
-        self._rating = None
-
-    @property
-    def data(self):
-        warnings.warn("Please use __getitem__ instead!", DeprecationWarning)
-        return self
-
-    @property
-    def fit_properties(self):
-        """Fitting results, see :func:`Indentation.fit_model`)"""
-        return self._fit_properties
-
-    @fit_properties.setter
-    def fit_properties(self, fp):
-        self._fit_properties.update(fp)
-
-    def apply_preprocessing(self, preprocessing=None, options=None,
-                            ret_details=False):
-        """Perform curve preprocessing steps
-
-        Parameters
-        ----------
-        preprocessing: list
-            A list of preprocessing method identifiers that are
-            stored in the `nanite.preproc.PREPROCESSORS` list.
-            If set to `None`, `self.preprocessing` will be
-            used.
-        options: dict of dict
-            Dictionary of keyword arguments for each preprocessing
-            step (if applicable)
-        ret_details:
-            Return preprocessing details dictionary
-        """
-        if preprocessing is None:
-            preprocessing = self.preprocessing
-
-        if options is None:
-            options = self.preprocessing_options
-
-        if "preprocessing" in self.fit_properties:
-            preproc_past = [self.fit_properties["preprocessing"],
-                            self.fit_properties["preprocessing_options"]]
-        else:
-            preproc_past = []
-
-        if ((preproc_past != [preprocessing, options])
-                or (not self._preprocessing_details and ret_details)):
-            # Remember initial fit parameters for user convenience
-            fp = self.fit_properties
-            # Reset fit properties
-            fp.reset()
-            # Set preprocessing options
-            fp["preprocessing"] = preprocessing
-            fp["preprocessing_options"] = options
-            # Reset rating
-            self._rating = None
-            # Apply preprocessing
-            # (This will call `AFMData.reset_data` on self)
-            details = preproc.apply(apret=self,
-                                    identifiers=preprocessing,
-                                    options=options,
-                                    ret_details=ret_details)
-            self._preprocessing_details = details
-            # Check availability of axes
-            for ax in ["x_axis", "y_axis"]:
-                # make sure the fitting axes are defined
-                if ax in fp and not fp[ax] in self:
-                    fp.pop(ax)
-
-        # remember preprocessing
-        self.preprocessing = preprocessing
-        self.preprocessing_options = copy.deepcopy(options)
-
-        return self._preprocessing_details
-
-    def compute_emodulus_mindelta(self, callback=None):
-        """Elastic modulus in dependency of maximum indentation
-
-        The fitting interval is varied such that the maximum
-        indentation depth ranges from the lowest tip position
-        to the estimated contact point. For each interval, the
-        current model is fitted and the elastic modulus is
-        extracted.
-
-        Parameters
-        ----------
-        callback: callable
-            A method that is called with the `emoduli` and
-            `indentations` as the computation proceeds every
-            five steps.
-
-        Returns
-        -------
-        emoduli, indentations: 1d ndarrays
-            The fitted elastic moduli at the corresponding
-            maximal indentation depths.
-
-        Notes
-        -----
-        The information about emodulus and mindelta is also stored in
-        `self.fit_properties` with the keys "optimal_fit_E_array" and
-        "optimal_fit_delta_array", if `self.fit_model` is called with
-        the argument `search_optimal_fit` set to `True`.
-        """
-
-        if "optimal_fit_E_array" in self.fit_properties:
-            emoduli = self.fit_properties["optimal_fit_E_array"]
-            indentations = self.fit_properties["optimal_fit_delta_array"]
-        else:
-            fitter = IndentationFitter(self)
-            emoduli, indentations = fitter.compute_emodulus_vs_mindelta(
-                callback=callback
-            )
-            self.fit_properties["optimal_fit_E_array"] = emoduli
-            self.fit_properties["optimal_fit_delta_array"] = indentations
-        return emoduli, indentations
-
-    def estimate_optimal_mindelta(self):
-        """Estimate the optimal indentation depth
-
-        This is a convenience function that wraps around
-        `compute_emodulus_mindelta` and
-        `IndentationFitter.compute_opt_mindelta`.
-        """
-        emoduli, indentations = self.compute_emodulus_mindelta()
-        dopt = IndentationFitter.compute_opt_mindelta(
-            emoduli=emoduli,
-            indentations=indentations
-        )
-        return dopt
-
-    def estimate_contact_point_index(self, method="deviation_from_baseline"):
-        """Estimate the contact point index
-
-        See the `poc` submodule for more information.
-        """
-        idp = poc.compute_poc(force=np.array(self["force"], copy=True),
-                              method=method)
-        return idp
-
-    def fit_model(self, **kwargs):
-        """Fit the approach-retract data to a model function
-
-        Parameters
-        ----------
-        model_key: str
-            A key referring to a model in
-            `nanite.model.models_available`
-        params_initial: instance of lmfit.Parameters or dict
-            Parameters for fitting. If not given,
-            default parameters are used.
-        range_x: tuple of 2
-            The range for fitting, see `range_type` below.
-        range_type: str
-            One of:
-
-            - absolute:
-                Set the absolute fitting range in values
-                given by the `x_axis`.
-            - relative cp:
-                In some cases it is desired to be able to
-                fit a model only up until a certain indentation
-                depth (tip position) measured from the contact
-                point. Since the contact point is a fit parameter
-                as well, this requires a two-pass fitting.
-        preprocessing: list of str
-            Preprocessing
-        preprocessing_options: list of str
-            Preprocessing
-        segment: str
-            Segment index (e.g. 0 for approach)
-        weight_cp: float
-            Weight the contact point region which shows artifacts
-            that are difficult to model with e.g. Hertz.
-        gcf_k: float
-            Geometrical correction factor :math:`k` for non-single-contact
-            data. The measured indentation is multiplied by this factor to
-            correct for experimental geometries during fitting,
-            e.g. ``gcf_k=0.5`` for parallel-place compression.
-        optimal_fit_edelta: bool
-            Search for the optimal fit by varying the maximal
-            indentation depth and determining a plateau in the
-            resulting Young's modulus (fitting parameter "E").
-        """
-        if "preprocessing" in kwargs:
-            options = kwargs.get("preprocessing_options",
-                                 self.preprocessing_options)
-            self.apply_preprocessing(preprocessing=kwargs["preprocessing"],
-                                     options=options)
-        # self.fit_properties is an instance of FitProperties that
-        # stores previous fit kwargs. If the given kwargs are
-        # different than in the previous fit, the following two
-        # lines will reset the "hash" in the fit properties, triggering
-        # a new fit.
-        # (sorted, such that `model_key` is set before `params_initial`)
-        for arg in sorted(kwargs.keys()):
-            self.fit_properties[arg] = kwargs[arg]
-
-        # set a default model (needed for self.get_initial_fit_parameters)
-        if "model_key" not in self.fit_properties:
-            self.fit_properties["model_key"] = FP_DEFAULT["model_key"]
-
-        # set default initial parameters
-        if ("params_initial" not in self.fit_properties
-                or self.fit_properties["params_initial"] is None):
-            # We need the initial parameters (to modify them).
-            # Guesses common parameters like the contact point that
-            # would have otherwise been done in `IndentationFitter`:
-            fp_guess = self.get_initial_fit_parameters(
-                common_ancillaries=True,
-                model_ancillaries=True)
-            self.fit_properties["params_initial"] = fp_guess
-
-        if "hash" in self.fit_properties:
-            # There is nothing to do, because the initial fit
-            # properties are the same.
-            pass
-        else:
-            fitter = IndentationFitter(self)
-            # Perform fitting
-            # Note: if `fitter.fp["success"]` is `False`, then
-            # the `fit_residuals` and `fit_curve` are `nan`.
-            fitter.fit()
-            self["fit"] = fitter.fit_curve
-            self["fit residuals"] = fitter.fit_residuals
-            self["fit range"] = fitter.fit_range
-            self.fit_properties = fitter.fp
-
-    def get_ancillary_parameters(self, model_key=None):
-        """Compute ancillary parameters for the current model"""
-        if model_key is None:
-            if "model_key" in self.fit_properties:
-                model_key = self.fit_properties["model_key"]
-            else:
-                model_key = FP_DEFAULT["model_key"]
-        return model.compute_anc_parms(idnt=self,
-                                       model_key=model_key)
-
-    def get_initial_fit_parameters(self, model_key=None,
-                                   common_ancillaries=True,
-                                   model_ancillaries=True):
-        """Return the initial fit parameters
-
-        If there are not initial fit parameters set in
-        `self.fit_properties`, then they are computed.
-
-        Parameters
-        ----------
-        model_key: str
-            Optionally set a model key. This will override the
-            "model_key" key in `self.fit_properties`.
-        common_ancillaries: bool
-            Guess global ancillaries such as the contact point.
-        model_ancillaries: bool
-            Guess model-related ancillaries
-
-        Notes
-        -----
-        `global_ancillaries` and `model_ancillaries` only have an
-        effect if self.fit_properties["params_initial"] is set.
-        """
-        if model_key is not None:
-            self.fit_properties["model_key"] = model_key
-        if self.fit_properties.get("params_initial", False):
-            parms = self.fit_properties["params_initial"]
-        elif "model_key" in self.fit_properties:
-            parms = guess_initial_parameters(
-                self,
-                model_key=self.fit_properties["model_key"],
-                model_ancillaries=model_ancillaries,
-                common_ancillaries=common_ancillaries)
-        else:
-            # for user convenience (with default model)
-            parms = guess_initial_parameters(
-                self,
-                model_key=FP_DEFAULT["model_key"],
-                model_ancillaries=model_ancillaries,
-                common_ancillaries=common_ancillaries)
-        return parms
-
-    def get_rating_parameters(self):
-        """Return current rating parameters"""
-        rdict = OrderedDict()
-        if self._rating is None:
-            rt = [np.nan] * 6
-        else:
-            rt = self._rating
-        rdict["Hash"] = rt[0]
-        rdict["Regressor"] = rt[1]
-        rdict["Training set"] = rt[2]
-        rdict["Feature names"] = rt[3]
-        rdict["Linear discriminant analysis"] = rt[4]
-        rdict["Rating"] = rt[5]
-        return rdict
-
-    def rate_quality(self, regressor="Extra Trees", training_set="zef18",
-                     names=None, lda=None):
-        """Compute the quality of the obtained curve
-
-        Uses heuristic approaches to rate a curve.
-
-        Parameters
-        ----------
-        regressor: str
-            The regressor name used for rating.
-        training_set: str
-            A label for a training set shipped with nanite or a
-            path to a training set.
-        names: list of str
-            Only use these features for rating
-        lda: bool
-            Perform linear discriminant analysis
-
-        Returns
-        -------
-        rating: float
-            A value between 0 and 10 where 0 is the lowest rating.
-            If no fit has been performed, a rating of -1 is returned.
-
-        Notes
-        -----
-        The rating is cached based on the fitting hash
-        (see `IndentationFitter._hash`).
-        """
-        if self.fit_properties and "hash" in self.fit_properties:
-            curhash = self.fit_properties["hash"]
-        else:
-            curhash = "none"
-        if regressor.lower() == "none":
-            rt = -1
-        elif (self._rating is None or
-              self._rating[0] != curhash or
-              self._rating[1] != regressor or
-              self._rating[2] != training_set or
-              self._rating[3] != names or
-              self._rating[4] != lda):
-            # Perform rating
-            rater = get_rater(regressor=regressor,
-                              training_set=training_set,
-                              names=names,
-                              lda=lda)
-            rt = rater.rate(datasets=self)[0]
-            self._rating = (curhash, regressor, training_set, names, lda, rt)
-        else:
-            # Use cached rating
-            rt = self._rating[-1]
-        return rt
+from collections import OrderedDict
+import copy
+import warnings
+
+import afmformats
+import numpy as np
+
+from .fit import IndentationFitter, FitProperties, guess_initial_parameters, \
+    FP_DEFAULT
+from . import model
+from . import poc
+from . import preproc
+from .rate import get_rater
+
+
+class Indentation(afmformats.AFMForceDistance):
+    def __init__(self, data, metadata, diskcache=None):
+        """Additional functionalities for afmformats.AFMForceDistance"""
+        super(Indentation, self).__init__(data=data,
+                                          metadata=metadata,
+                                          diskcache=diskcache)
+        #: Default preprocessing steps,
+        #: see :func:`Indentation.apply_preprocessing`.
+        self.preprocessing = []
+        #: Preprocessing options
+        self.preprocessing_options = {}
+        # preprocessing details (for user convenience)
+        self._preprocessing_details = {}
+        # protected fit properties
+        self._fit_properties = FitProperties()
+
+        # Curve rating (see `self.rate_quality`)
+        self._rating = None
+
+    @property
+    def data(self):
+        warnings.warn("Please use __getitem__ instead!", DeprecationWarning)
+        return self
+
+    @property
+    def fit_properties(self):
+        """Fitting results, see :func:`Indentation.fit_model`)"""
+        return self._fit_properties
+
+    @fit_properties.setter
+    def fit_properties(self, fp):
+        self._fit_properties.update(fp)
+
+    def apply_preprocessing(self, preprocessing=None, options=None,
+                            ret_details=False):
+        """Perform curve preprocessing steps
+
+        Parameters
+        ----------
+        preprocessing: list
+            A list of preprocessing method identifiers that are
+            stored in the `nanite.preproc.PREPROCESSORS` list.
+            If set to `None`, `self.preprocessing` will be
+            used.
+        options: dict of dict
+            Dictionary of keyword arguments for each preprocessing
+            step (if applicable)
+        ret_details:
+            Return preprocessing details dictionary
+        """
+        if preprocessing is None:
+            preprocessing = self.preprocessing
+
+        if options is None:
+            options = self.preprocessing_options
+
+        if "preprocessing" in self.fit_properties:
+            preproc_past = [self.fit_properties["preprocessing"],
+                            self.fit_properties["preprocessing_options"]]
+        else:
+            preproc_past = []
+
+        if ((preproc_past != [preprocessing, options])
+                or (not self._preprocessing_details and ret_details)):
+            # Remember initial fit parameters for user convenience
+            fp = self.fit_properties
+            # Reset fit properties
+            fp.reset()
+            # Set preprocessing options
+            fp["preprocessing"] = preprocessing
+            fp["preprocessing_options"] = options
+            # Reset rating
+            self._rating = None
+            # Apply preprocessing
+            # (This will call `AFMData.reset_data` on self)
+            details = preproc.apply(apret=self,
+                                    identifiers=preprocessing,
+                                    options=options,
+                                    ret_details=ret_details)
+            self._preprocessing_details = details
+            # Check availability of axes
+            for ax in ["x_axis", "y_axis"]:
+                # make sure the fitting axes are defined
+                if ax in fp and not fp[ax] in self:
+                    fp.pop(ax)
+
+        # remember preprocessing
+        self.preprocessing = preprocessing
+        self.preprocessing_options = copy.deepcopy(options)
+
+        return self._preprocessing_details
+
+    def compute_emodulus_mindelta(self, callback=None):
+        """Elastic modulus in dependency of maximum indentation
+
+        The fitting interval is varied such that the maximum
+        indentation depth ranges from the lowest tip position
+        to the estimated contact point. For each interval, the
+        current model is fitted and the elastic modulus is
+        extracted.
+
+        Parameters
+        ----------
+        callback: callable
+            A method that is called with the `emoduli` and
+            `indentations` as the computation proceeds every
+            five steps.
+
+        Returns
+        -------
+        emoduli, indentations: 1d ndarrays
+            The fitted elastic moduli at the corresponding
+            maximal indentation depths.
+
+        Notes
+        -----
+        The information about emodulus and mindelta is also stored in
+        `self.fit_properties` with the keys "optimal_fit_E_array" and
+        "optimal_fit_delta_array", if `self.fit_model` is called with
+        the argument `search_optimal_fit` set to `True`.
+        """
+
+        if "optimal_fit_E_array" in self.fit_properties:
+            emoduli = self.fit_properties["optimal_fit_E_array"]
+            indentations = self.fit_properties["optimal_fit_delta_array"]
+        else:
+            fitter = IndentationFitter(self)
+            emoduli, indentations = fitter.compute_emodulus_vs_mindelta(
+                callback=callback
+            )
+            self.fit_properties["optimal_fit_E_array"] = emoduli
+            self.fit_properties["optimal_fit_delta_array"] = indentations
+        return emoduli, indentations
+
+    def estimate_optimal_mindelta(self):
+        """Estimate the optimal indentation depth
+
+        This is a convenience function that wraps around
+        `compute_emodulus_mindelta` and
+        `IndentationFitter.compute_opt_mindelta`.
+        """
+        emoduli, indentations = self.compute_emodulus_mindelta()
+        dopt = IndentationFitter.compute_opt_mindelta(
+            emoduli=emoduli,
+            indentations=indentations
+        )
+        return dopt
+
+    def estimate_contact_point_index(self, method="deviation_from_baseline"):
+        """Estimate the contact point index
+
+        See the `poc` submodule for more information.
+        """
+        idp = poc.compute_poc(force=np.array(self["force"], copy=True),
+                              method=method)
+        return idp
+
+    def fit_model(self, **kwargs):
+        """Fit the approach-retract data to a model function
+
+        Parameters
+        ----------
+        model_key: str
+            A key referring to a model in
+            `nanite.model.models_available`
+        params_initial: instance of lmfit.Parameters or dict
+            Parameters for fitting. If not given,
+            default parameters are used.
+        range_x: tuple of 2
+            The range for fitting, see `range_type` below.
+        range_type: str
+            One of:
+
+            - absolute:
+                Set the absolute fitting range in values
+                given by the `x_axis`.
+            - relative cp:
+                In some cases it is desired to be able to
+                fit a model only up until a certain indentation
+                depth (tip position) measured from the contact
+                point. Since the contact point is a fit parameter
+                as well, this requires a two-pass fitting.
+        preprocessing: list of str
+            Preprocessing
+        preprocessing_options: list of str
+            Preprocessing
+        segment: str
+            Segment index (e.g. 0 for approach)
+        weight_cp: float
+            Weight the contact point region which shows artifacts
+            that are difficult to model with e.g. Hertz.
+        gcf_k: float
+            Geometrical correction factor :math:`k` for non-single-contact
+            data. The measured indentation is multiplied by this factor to
+            correct for experimental geometries during fitting,
+            e.g. ``gcf_k=0.5`` for parallel-place compression.
+        optimal_fit_edelta: bool
+            Search for the optimal fit by varying the maximal
+            indentation depth and determining a plateau in the
+            resulting Young's modulus (fitting parameter "E").
+        """
+        if "preprocessing" in kwargs:
+            options = kwargs.get("preprocessing_options",
+                                 self.preprocessing_options)
+            self.apply_preprocessing(preprocessing=kwargs["preprocessing"],
+                                     options=options)
+        # self.fit_properties is an instance of FitProperties that
+        # stores previous fit kwargs. If the given kwargs are
+        # different than in the previous fit, the following two
+        # lines will reset the "hash" in the fit properties, triggering
+        # a new fit.
+        # (sorted, such that `model_key` is set before `params_initial`)
+        for arg in sorted(kwargs.keys()):
+            self.fit_properties[arg] = kwargs[arg]
+
+        # set a default model (needed for self.get_initial_fit_parameters)
+        if "model_key" not in self.fit_properties:
+            self.fit_properties["model_key"] = FP_DEFAULT["model_key"]
+
+        # set default initial parameters
+        if ("params_initial" not in self.fit_properties
+                or self.fit_properties["params_initial"] is None):
+            # We need the initial parameters (to modify them).
+            # Guesses common parameters like the contact point that
+            # would have otherwise been done in `IndentationFitter`:
+            fp_guess = self.get_initial_fit_parameters(
+                common_ancillaries=True,
+                model_ancillaries=True)
+            self.fit_properties["params_initial"] = fp_guess
+
+        if "hash" in self.fit_properties:
+            # There is nothing to do, because the initial fit
+            # properties are the same.
+            pass
+        else:
+            fitter = IndentationFitter(self)
+            # Perform fitting
+            # Note: if `fitter.fp["success"]` is `False`, then
+            # the `fit_residuals` and `fit_curve` are `nan`.
+            fitter.fit()
+            self["fit"] = fitter.fit_curve
+            self["fit residuals"] = fitter.fit_residuals
+            self["fit range"] = fitter.fit_range
+            self.fit_properties = fitter.fp
+
+    def get_ancillary_parameters(self, model_key=None):
+        """Compute ancillary parameters for the current model"""
+        if model_key is None:
+            if "model_key" in self.fit_properties:
+                model_key = self.fit_properties["model_key"]
+            else:
+                model_key = FP_DEFAULT["model_key"]
+        return model.compute_anc_parms(idnt=self,
+                                       model_key=model_key)
+
+    def get_initial_fit_parameters(self, model_key=None,
+                                   common_ancillaries=True,
+                                   model_ancillaries=True):
+        """Return the initial fit parameters
+
+        If there are not initial fit parameters set in
+        `self.fit_properties`, then they are computed.
+
+        Parameters
+        ----------
+        model_key: str
+            Optionally set a model key. This will override the
+            "model_key" key in `self.fit_properties`.
+        common_ancillaries: bool
+            Guess global ancillaries such as the contact point.
+        model_ancillaries: bool
+            Guess model-related ancillaries
+
+        Notes
+        -----
+        `global_ancillaries` and `model_ancillaries` only have an
+        effect if self.fit_properties["params_initial"] is set.
+        """
+        if model_key is not None:
+            self.fit_properties["model_key"] = model_key
+        if self.fit_properties.get("params_initial", False):
+            parms = self.fit_properties["params_initial"]
+        elif "model_key" in self.fit_properties:
+            parms = guess_initial_parameters(
+                self,
+                model_key=self.fit_properties["model_key"],
+                model_ancillaries=model_ancillaries,
+                common_ancillaries=common_ancillaries)
+        else:
+            # for user convenience (with default model)
+            parms = guess_initial_parameters(
+                self,
+                model_key=FP_DEFAULT["model_key"],
+                model_ancillaries=model_ancillaries,
+                common_ancillaries=common_ancillaries)
+        return parms
+
+    def get_rating_parameters(self):
+        """Return current rating parameters"""
+        rdict = OrderedDict()
+        if self._rating is None:
+            rt = [np.nan] * 6
+        else:
+            rt = self._rating
+        rdict["Hash"] = rt[0]
+        rdict["Regressor"] = rt[1]
+        rdict["Training set"] = rt[2]
+        rdict["Feature names"] = rt[3]
+        rdict["Linear discriminant analysis"] = rt[4]
+        rdict["Rating"] = rt[5]
+        return rdict
+
+    def rate_quality(self, regressor="Extra Trees", training_set="zef18",
+                     names=None, lda=None):
+        """Compute the quality of the obtained curve
+
+        Uses heuristic approaches to rate a curve.
+
+        Parameters
+        ----------
+        regressor: str
+            The regressor name used for rating.
+        training_set: str
+            A label for a training set shipped with nanite or a
+            path to a training set.
+        names: list of str
+            Only use these features for rating
+        lda: bool
+            Perform linear discriminant analysis
+
+        Returns
+        -------
+        rating: float
+            A value between 0 and 10 where 0 is the lowest rating.
+            If no fit has been performed, a rating of -1 is returned.
+
+        Notes
+        -----
+        The rating is cached based on the fitting hash
+        (see `IndentationFitter._hash`).
+        """
+        if self.fit_properties and "hash" in self.fit_properties:
+            curhash = self.fit_properties["hash"]
+        else:
+            curhash = "none"
+        if regressor.lower() == "none":
+            rt = -1
+        elif (self._rating is None or
+              self._rating[0] != curhash or
+              self._rating[1] != regressor or
+              self._rating[2] != training_set or
+              self._rating[3] != names or
+              self._rating[4] != lda):
+            # Perform rating
+            rater = get_rater(regressor=regressor,
+                              training_set=training_set,
+                              names=names,
+                              lda=lda)
+            rt = rater.rate(datasets=self)[0]
+            self._rating = (curhash, regressor, training_set, names, lda, rt)
+        else:
+            # Use cached rating
+            rt = self._rating[-1]
+        return rt
```

### Comparing `nanite-3.5.4/nanite/model/__init__.py` & `nanite-3.6.0/nanite/model/__init__.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,128 +1,128 @@
-import warnings
-
-from . import model_conical_indenter  # noqa: F401
-from . import model_hertz_paraboloidal  # noqa: F401
-from . import model_hertz_three_sided_pyramid  # noqa: F401
-from . import model_sneddon_spherical  # noqa: F401
-from . import model_sneddon_spherical_approximation  # noqa: F401
-
-from .core import NaniteFitModel  # noqa: F401
-from . import residuals  # noqa: F401
-from .logic import models_available, register_model
-from .logic import deregister_model, load_model_from_file  # noqa: F401
-
-
-def compute_anc_parms(idnt, model_key):
-    """Compute ancillary parameters for a force-distance dataset
-
-    Ancillary parameters include parameters that:
-
-    - are unrelated to fitting: They may just be important parameters
-      to the user.
-    - require the entire dataset: They cannot be extracted during
-      fitting, because they require more than just the approach xor
-      retract curve to compute (e.g. hysteresis, jump of retract curve
-      at maximum indentation). They may, additionally, depend on
-      initial fit parameters set by the user.
-    - require a fit: They are dependent on fitting parameters but
-      are not required during fitting.
-
-    Notes
-    -----
-    If an ancillary parameter name matches that of a fitting parameter,
-    then it is assumed that it can be used for fitting. Please see
-    :func:`nanite.indent.Indentation.get_initial_fit_parameters`
-    and :func:`nanite.fit.guess_initial_parameters`.
-
-    Ancillary parameters are set to `np.nan` if they cannot be
-    computed.
-
-    Parameters
-    ----------
-    idnt: nanite.indent.Indentation
-        The force-distance data for which to compute the ancillary
-        parameters
-    model_key: str
-        Name of the model
-
-    Returns
-    -------
-    ancillaries: collections.OrderedDict
-        key-value dictionary of ancillary parameters
-    """
-    md = models_available[model_key]
-    return md.compute_ancillaries(idnt)
-
-
-def get_anc_parms(idnt, model_key):
-    warnings.warn(
-        "Method `get_anc_parms` is deprecated. Please use "
-        + "`compute_anc_parms` instead.",
-        DeprecationWarning)
-    return compute_anc_parms(idnt, model_key)
-
-
-def get_anc_parm_keys(model_key):
-    """Return the key names of a model's ancillary parameters"""
-    md = models_available[model_key]
-    return md.get_anc_parm_keys()
-
-
-def get_init_parms(model_key):
-    """Get initial fit parameters for a model"""
-    md = models_available[model_key]
-    return md.get_parameter_defaults()
-
-
-def get_model_by_name(name):
-    """Convenience function to obtain a model by name instead of by key"""
-    for key in models_available:
-        if models_available[key].model_name == name:
-            return models_available[key]
-    else:
-        raise KeyError("No model with name '{}'!".format(name))
-
-
-def get_parm_name(model_key, parm_key):
-    """Return parameter label
-
-    Parameters
-    ----------
-    model_key: str
-        The model key (e.g. "hertz_cone")
-    parm_key: str
-        The parameter key (e.g. "E")
-
-    Returns
-    -------
-    parm_name: str
-        The parameter label (e.g. "Young's Modulus")
-    """
-    md = models_available[model_key]
-    return md.get_parm_name(parm_key)
-
-
-def get_parm_unit(model_key, parm_key):
-    """Return parameter unit
-
-    Parameters
-    ----------
-    model_key: str
-        The model key (e.g. "hertz_cone")
-    parm_key: str
-        The parameter key (e.g. "E")
-
-    Returns
-    -------
-    parm_unit: str
-        The parameter unit (e.g. "Pa")
-    """
-    md = models_available[model_key]
-    return md.get_parm_unit(parm_key)
-
-
-# Populate list of available fit models
-_loc = locals().copy()
-for _item in _loc:
-    if _item.startswith("model_"):
-        register_model(_loc[_item])
+import warnings
+
+from . import model_conical_indenter  # noqa: F401
+from . import model_hertz_paraboloidal  # noqa: F401
+from . import model_hertz_three_sided_pyramid  # noqa: F401
+from . import model_sneddon_spherical  # noqa: F401
+from . import model_sneddon_spherical_approximation  # noqa: F401
+
+from .core import NaniteFitModel  # noqa: F401
+from . import residuals  # noqa: F401
+from .logic import models_available, register_model
+from .logic import deregister_model, load_model_from_file  # noqa: F401
+
+
+def compute_anc_parms(idnt, model_key):
+    """Compute ancillary parameters for a force-distance dataset
+
+    Ancillary parameters include parameters that:
+
+    - are unrelated to fitting: They may just be important parameters
+      to the user.
+    - require the entire dataset: They cannot be extracted during
+      fitting, because they require more than just the approach xor
+      retract curve to compute (e.g. hysteresis, jump of retract curve
+      at maximum indentation). They may, additionally, depend on
+      initial fit parameters set by the user.
+    - require a fit: They are dependent on fitting parameters but
+      are not required during fitting.
+
+    Notes
+    -----
+    If an ancillary parameter name matches that of a fitting parameter,
+    then it is assumed that it can be used for fitting. Please see
+    :func:`nanite.indent.Indentation.get_initial_fit_parameters`
+    and :func:`nanite.fit.guess_initial_parameters`.
+
+    Ancillary parameters are set to `np.nan` if they cannot be
+    computed.
+
+    Parameters
+    ----------
+    idnt: nanite.indent.Indentation
+        The force-distance data for which to compute the ancillary
+        parameters
+    model_key: str
+        Name of the model
+
+    Returns
+    -------
+    ancillaries: collections.OrderedDict
+        key-value dictionary of ancillary parameters
+    """
+    md = models_available[model_key]
+    return md.compute_ancillaries(idnt)
+
+
+def get_anc_parms(idnt, model_key):
+    warnings.warn(
+        "Method `get_anc_parms` is deprecated. Please use "
+        + "`compute_anc_parms` instead.",
+        DeprecationWarning)
+    return compute_anc_parms(idnt, model_key)
+
+
+def get_anc_parm_keys(model_key):
+    """Return the key names of a model's ancillary parameters"""
+    md = models_available[model_key]
+    return md.get_anc_parm_keys()
+
+
+def get_init_parms(model_key):
+    """Get initial fit parameters for a model"""
+    md = models_available[model_key]
+    return md.get_parameter_defaults()
+
+
+def get_model_by_name(name):
+    """Convenience function to obtain a model by name instead of by key"""
+    for key in models_available:
+        if models_available[key].model_name == name:
+            return models_available[key]
+    else:
+        raise KeyError("No model with name '{}'!".format(name))
+
+
+def get_parm_name(model_key, parm_key):
+    """Return parameter label
+
+    Parameters
+    ----------
+    model_key: str
+        The model key (e.g. "hertz_cone")
+    parm_key: str
+        The parameter key (e.g. "E")
+
+    Returns
+    -------
+    parm_name: str
+        The parameter label (e.g. "Young's Modulus")
+    """
+    md = models_available[model_key]
+    return md.get_parm_name(parm_key)
+
+
+def get_parm_unit(model_key, parm_key):
+    """Return parameter unit
+
+    Parameters
+    ----------
+    model_key: str
+        The model key (e.g. "hertz_cone")
+    parm_key: str
+        The parameter key (e.g. "E")
+
+    Returns
+    -------
+    parm_unit: str
+        The parameter unit (e.g. "Pa")
+    """
+    md = models_available[model_key]
+    return md.get_parm_unit(parm_key)
+
+
+# Populate list of available fit models
+_loc = locals().copy()
+for _item in _loc:
+    if _item.startswith("model_"):
+        register_model(_loc[_item])
```

### Comparing `nanite-3.5.4/nanite/model/core.py` & `nanite-3.6.0/nanite/model/core.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,301 +1,301 @@
-from collections import OrderedDict
-import inspect
-import warnings
-
-import numpy as np
-
-from . import residuals
-
-
-class ModelError(BaseException):
-    pass
-
-
-class ModelIncompleteError(ModelError):
-    pass
-
-
-class ModelImplementationError(ModelError):
-    pass
-
-
-class ModelImportError(ModelError):
-    pass
-
-
-class ModelImplementationWarning(UserWarning):
-    pass
-
-
-class NaniteFitModel:
-    def __init__(self, model_module):
-        """Initialize the model with an imported Python module"""
-        self.module = model_module
-        self._module_check()
-        self._module_autocomplete()
-
-        # propagate all module attributes to this instance
-        # standard parameters
-        self.get_parameter_defaults = self.module.get_parameter_defaults
-        self.model_doc = self.module.model_doc
-        self.model_key = self.module.model_key
-        self.model_name = self.module.model_name
-        self.parameter_keys = self.module.parameter_keys
-        self.parameter_names = self.module.parameter_names
-        self.parameter_units = self.module.parameter_units
-        self.valid_axes_x = self.module.valid_axes_x
-        self.valid_axes_y = self.module.valid_axes_y
-        # optional ancillary parameters
-        if hasattr(self.module, "compute_ancillaries"):
-            self.has_module_ancillaries = True
-            self.parameter_anc_keys = self.module.parameter_anc_keys
-            self.parameter_anc_names = self.module.parameter_anc_names
-            self.parameter_anc_units = self.module.parameter_anc_units
-        else:
-            self.has_module_ancillaries = False
-        # model function
-        self.model = self.module.model
-        # residuals
-        self.residual = self.module.residual
-
-    def __str__(self):
-        return f"NaniteFitModel '{self.model_key}'"
-
-    def __repr__(self):
-        return f"<NaniteFitModel '{self.model_key}' at {hex(id(self))}"
-
-    def _module_autocomplete(self):
-        """Add any missing attributes to the underlying model module"""
-        # check for residuals function
-        if not hasattr(self.module, "residual"):
-            # use the default residual function
-            self.module.residual = residuals.get_default_residuals_wrapper(
-                model_function=self.module.model_func)
-
-        # check for modeling function
-        if not hasattr(self.module, "model"):
-            # use the default residual function
-            self.module.model = residuals.get_default_modeling_wrapper(
-                model_function=self.module.model_func)
-
-    def _module_check(self):
-        """Checks whether the model's module is set up correctly"""
-        # sanity checks
-        missing = []
-        for attr in [
-            "get_parameter_defaults",
-            "model_doc",
-            "model_key",
-            "model_name",
-            "parameter_keys",
-            "parameter_names",
-            "parameter_units",
-            "valid_axes_x",
-            "valid_axes_y",
-             ]:
-            if not hasattr(self.module, attr):
-                missing.append(attr)
-        if missing:
-            raise ModelIncompleteError(
-                f"Model `{self.module}` is missing the following "
-                + f"attributes: {', '.join(missing)}")
-
-        model_key = self.module.model_key
-        # check for completeness of ancillary parameter recipe
-        if hasattr(self.module, "compute_ancillaries"):
-            missing_anc = []
-            for attr in ["parameter_anc_keys",
-                         "parameter_anc_names",
-                         "parameter_anc_units",
-                         ]:
-                if not hasattr(self.module, attr):
-                    missing_anc.append(attr)
-            if missing_anc:
-                raise ModelIncompleteError(
-                    f"Model `{model_key}` is missing the following "
-                    + f"attributes: {', '.join(missing_anc)}")
-
-        # check length of modeling lists
-        if len(self.module.parameter_keys) != len(self.module.parameter_names):
-            raise ModelImplementationError(
-                "'parameter_keys' and 'parameter_names' have different "
-                + f"lengths for model '{model_key}'!")
-        if len(self.module.parameter_keys) != len(self.module.parameter_units):
-            raise ModelImplementationError(
-                "'parameter_keys' and 'parameter_units' have different "
-                + f"lengths for model '{model_key}'!")
-
-        # check for spaces in units
-        if [u.strip() for u in self.module.parameter_units] \
-                != self.module.parameter_units:
-            warnings.warn("The `parameter_units` should not contain leading "
-                          + f"or trailing spaces. Please check {model_key}!",
-                          ModelImplementationWarning)
-
-        if hasattr(self.module, "parameter_anc_units"):
-            if [u.strip() for u in self.module.parameter_anc_units] \
-                    != self.module.parameter_anc_units:
-                warnings.warn(
-                    "The `parameter_anc_units` should not contain leading "
-                    + f"or trailing spaces. Please check {model_key}!",
-                    ModelImplementationWarning)
-
-        # check for label uniqueness
-        if len(self.module.parameter_names) \
-                != len(set(self.module.parameter_names)):
-            raise ModelImplementationError(
-                f"'parameter_names' should be unique for '{model_key}'!")
-
-        # checks for model parameters
-        p_def = list(self.module.get_parameter_defaults().keys())
-        p_arg = list(inspect.signature(
-            self.module.model_func).parameters.keys())
-        for ii, key in enumerate(self.module.parameter_keys):
-            if key != p_def[ii]:
-                raise ModelImplementationError(
-                    "Please check 'parameter_keys' and "
-                    + f"'get_parameter_defaults'  of the model '{model_key}'. "
-                    + f"Keys {key} and {p_def[ii]} are not in order!")
-            if key != p_arg[ii+1]:
-                warnings.warn(
-                    "Please make sure that the parameters of the model "
-                    + "function are in the same order as in 'parameter_keys' "
-                    + f"for the model '{model_key}'! "
-                    + "The abscissa (usually `delta`) should come first. "
-                    + "This warning may become an Exception in the future!",
-                    ModelImplementationWarning)
-
-    def compute_ancillaries(self, fd):
-        """Compute ancillary parameters for a force-distance dataset
-
-        Ancillary parameters include parameters that:
-
-        - are unrelated to fitting: They may just be important parameters
-          to the user.
-        - require the entire dataset: They cannot be extracted during
-          fitting, because they require more than just the approach xor
-          retract curve to compute (e.g. hysteresis, jump of retract curve
-          at maximum indentation). They may, additionally, depend on
-          initial fit parameters set by the user.
-        - require a fit: They are dependent on fitting parameters but
-          are not required during fitting.
-
-        Notes
-        -----
-        If an ancillary parameter name matches that of a fitting parameter,
-        then it is assumed that it can be used for fitting. Please see
-        :func:`nanite.indent.Indentation.get_initial_fit_parameters`
-        and :func:`nanite.fit.guess_initial_parameters`.
-
-        Ancillary parameters are set to `np.nan` if they cannot be
-        computed.
-
-        Parameters
-        ----------
-        fd: nanite.indent.Indentation
-            The force-distance data for which to compute the ancillary
-            parameters
-
-        Returns
-        -------
-        ancillaries: collections.OrderedDict
-            key-value dictionary of ancillary parameters
-        """
-        # TODO:
-        # - ancillaries are not cached yet (some ancillaries might depend on
-        #   fitting interval or other initial parameters - take that into
-        #   account)
-        # - "max_indent" actually belongs to "common_ancillaries" (see fit.py)
-        anc_ord = OrderedDict()
-        # general
-        for key in ANCILLARY_COMMON:
-            gmeth = ANCILLARY_COMMON[key][2]
-            anc_ord[key] = gmeth(fd)
-        # from module
-        if self.has_module_ancillaries:
-            anc_md = self.module.compute_ancillaries(fd)
-            for kk in self.parameter_anc_keys:
-                anc_ord[kk] = anc_md[kk]
-        return anc_ord
-
-    def get_anc_parm_keys(self):
-        """Return the key names of a model's ancillary parameters"""
-        akeys = list(ANCILLARY_COMMON.keys())
-        if self.has_module_ancillaries:
-            akeys += self.parameter_anc_keys
-        return akeys
-
-    def get_parm_name(self, key):
-        """Return parameter label
-
-        Parameters
-        ----------
-        key: str
-            The parameter key (e.g. "E")
-
-        Returns
-        -------
-        parm_name: str
-            The parameter label (e.g. "Young's Modulus")
-        """
-        if key in self.parameter_keys:
-            idx = self.parameter_keys.index(key)
-            return self.parameter_names[idx]
-        elif (self.has_module_ancillaries
-              and key in self.parameter_anc_keys):
-            idx = self.parameter_anc_keys.index(key)
-            return self.parameter_anc_names[idx]
-        elif key in ANCILLARY_COMMON:
-            return ANCILLARY_COMMON[key][0]
-        else:
-            raise KeyError(
-                f"Could not find parameter name for '{key}' in '{self}'!")
-
-    def get_parm_unit(self, key):
-        """Return parameter unit
-
-        Parameters
-        ----------
-        key: str
-            The parameter key (e.g. "E")
-
-        Returns
-        -------
-        parm_unit: str
-            The parameter unit (e.g. "Pa")
-        """
-        if key in self.parameter_keys:
-            idx = self.parameter_keys.index(key)
-            return self.parameter_units[idx]
-        elif (self.has_module_ancillaries
-              and key in self.parameter_anc_keys):
-            idx = self.parameter_anc_keys.index(key)
-            return self.parameter_anc_units[idx]
-        elif key in ANCILLARY_COMMON:
-            return ANCILLARY_COMMON[key][1]
-        else:
-            raise KeyError(
-                f"Could not find parameter unit for '{key}' in '{self}'!")
-
-
-def compute_anc_max_indent(fd):
-    """Compute ancillary parameter 'Maximum indentation'"""
-    # compute maximal indentation
-    if ("tip position" in fd
-        and "fit" in fd
-            and "params_fitted" in fd.fit_properties
-            and "contact_point" in fd.fit_properties["params_fitted"]):
-        cp = fd.fit_properties["params_fitted"]["contact_point"].value
-        idmax = fd.appr["fit"].argmax()
-        mi = fd.appr["tip position"][idmax]
-        mival = (cp-mi)
-    else:
-        mival = np.nan
-    return mival
-
-
-#: Common ancillary parameters
-ANCILLARY_COMMON = OrderedDict()
-ANCILLARY_COMMON["max_indent"] = ("Maximum indentation",
-                                  "m",
-                                  compute_anc_max_indent)
+from collections import OrderedDict
+import inspect
+import warnings
+
+import numpy as np
+
+from . import residuals
+
+
+class ModelError(BaseException):
+    pass
+
+
+class ModelIncompleteError(ModelError):
+    pass
+
+
+class ModelImplementationError(ModelError):
+    pass
+
+
+class ModelImportError(ModelError):
+    pass
+
+
+class ModelImplementationWarning(UserWarning):
+    pass
+
+
+class NaniteFitModel:
+    def __init__(self, model_module):
+        """Initialize the model with an imported Python module"""
+        self.module = model_module
+        self._module_check()
+        self._module_autocomplete()
+
+        # propagate all module attributes to this instance
+        # standard parameters
+        self.get_parameter_defaults = self.module.get_parameter_defaults
+        self.model_doc = self.module.model_doc
+        self.model_key = self.module.model_key
+        self.model_name = self.module.model_name
+        self.parameter_keys = self.module.parameter_keys
+        self.parameter_names = self.module.parameter_names
+        self.parameter_units = self.module.parameter_units
+        self.valid_axes_x = self.module.valid_axes_x
+        self.valid_axes_y = self.module.valid_axes_y
+        # optional ancillary parameters
+        if hasattr(self.module, "compute_ancillaries"):
+            self.has_module_ancillaries = True
+            self.parameter_anc_keys = self.module.parameter_anc_keys
+            self.parameter_anc_names = self.module.parameter_anc_names
+            self.parameter_anc_units = self.module.parameter_anc_units
+        else:
+            self.has_module_ancillaries = False
+        # model function
+        self.model = self.module.model
+        # residuals
+        self.residual = self.module.residual
+
+    def __str__(self):
+        return f"NaniteFitModel '{self.model_key}'"
+
+    def __repr__(self):
+        return f"<NaniteFitModel '{self.model_key}' at {hex(id(self))}"
+
+    def _module_autocomplete(self):
+        """Add any missing attributes to the underlying model module"""
+        # check for residuals function
+        if not hasattr(self.module, "residual"):
+            # use the default residual function
+            self.module.residual = residuals.get_default_residuals_wrapper(
+                model_function=self.module.model_func)
+
+        # check for modeling function
+        if not hasattr(self.module, "model"):
+            # use the default residual function
+            self.module.model = residuals.get_default_modeling_wrapper(
+                model_function=self.module.model_func)
+
+    def _module_check(self):
+        """Checks whether the model's module is set up correctly"""
+        # sanity checks
+        missing = []
+        for attr in [
+            "get_parameter_defaults",
+            "model_doc",
+            "model_key",
+            "model_name",
+            "parameter_keys",
+            "parameter_names",
+            "parameter_units",
+            "valid_axes_x",
+            "valid_axes_y",
+             ]:
+            if not hasattr(self.module, attr):
+                missing.append(attr)
+        if missing:
+            raise ModelIncompleteError(
+                f"Model `{self.module}` is missing the following "
+                + f"attributes: {', '.join(missing)}")
+
+        model_key = self.module.model_key
+        # check for completeness of ancillary parameter recipe
+        if hasattr(self.module, "compute_ancillaries"):
+            missing_anc = []
+            for attr in ["parameter_anc_keys",
+                         "parameter_anc_names",
+                         "parameter_anc_units",
+                         ]:
+                if not hasattr(self.module, attr):
+                    missing_anc.append(attr)
+            if missing_anc:
+                raise ModelIncompleteError(
+                    f"Model `{model_key}` is missing the following "
+                    + f"attributes: {', '.join(missing_anc)}")
+
+        # check length of modeling lists
+        if len(self.module.parameter_keys) != len(self.module.parameter_names):
+            raise ModelImplementationError(
+                "'parameter_keys' and 'parameter_names' have different "
+                + f"lengths for model '{model_key}'!")
+        if len(self.module.parameter_keys) != len(self.module.parameter_units):
+            raise ModelImplementationError(
+                "'parameter_keys' and 'parameter_units' have different "
+                + f"lengths for model '{model_key}'!")
+
+        # check for spaces in units
+        if [u.strip() for u in self.module.parameter_units] \
+                != self.module.parameter_units:
+            warnings.warn("The `parameter_units` should not contain leading "
+                          + f"or trailing spaces. Please check {model_key}!",
+                          ModelImplementationWarning)
+
+        if hasattr(self.module, "parameter_anc_units"):
+            if [u.strip() for u in self.module.parameter_anc_units] \
+                    != self.module.parameter_anc_units:
+                warnings.warn(
+                    "The `parameter_anc_units` should not contain leading "
+                    + f"or trailing spaces. Please check {model_key}!",
+                    ModelImplementationWarning)
+
+        # check for label uniqueness
+        if len(self.module.parameter_names) \
+                != len(set(self.module.parameter_names)):
+            raise ModelImplementationError(
+                f"'parameter_names' should be unique for '{model_key}'!")
+
+        # checks for model parameters
+        p_def = list(self.module.get_parameter_defaults().keys())
+        p_arg = list(inspect.signature(
+            self.module.model_func).parameters.keys())
+        for ii, key in enumerate(self.module.parameter_keys):
+            if key != p_def[ii]:
+                raise ModelImplementationError(
+                    "Please check 'parameter_keys' and "
+                    + f"'get_parameter_defaults'  of the model '{model_key}'. "
+                    + f"Keys {key} and {p_def[ii]} are not in order!")
+            if key != p_arg[ii+1]:
+                warnings.warn(
+                    "Please make sure that the parameters of the model "
+                    + "function are in the same order as in 'parameter_keys' "
+                    + f"for the model '{model_key}'! "
+                    + "The abscissa (usually `delta`) should come first. "
+                    + "This warning may become an Exception in the future!",
+                    ModelImplementationWarning)
+
+    def compute_ancillaries(self, fd):
+        """Compute ancillary parameters for a force-distance dataset
+
+        Ancillary parameters include parameters that:
+
+        - are unrelated to fitting: They may just be important parameters
+          to the user.
+        - require the entire dataset: They cannot be extracted during
+          fitting, because they require more than just the approach xor
+          retract curve to compute (e.g. hysteresis, jump of retract curve
+          at maximum indentation). They may, additionally, depend on
+          initial fit parameters set by the user.
+        - require a fit: They are dependent on fitting parameters but
+          are not required during fitting.
+
+        Notes
+        -----
+        If an ancillary parameter name matches that of a fitting parameter,
+        then it is assumed that it can be used for fitting. Please see
+        :func:`nanite.indent.Indentation.get_initial_fit_parameters`
+        and :func:`nanite.fit.guess_initial_parameters`.
+
+        Ancillary parameters are set to `np.nan` if they cannot be
+        computed.
+
+        Parameters
+        ----------
+        fd: nanite.indent.Indentation
+            The force-distance data for which to compute the ancillary
+            parameters
+
+        Returns
+        -------
+        ancillaries: collections.OrderedDict
+            key-value dictionary of ancillary parameters
+        """
+        # TODO:
+        # - ancillaries are not cached yet (some ancillaries might depend on
+        #   fitting interval or other initial parameters - take that into
+        #   account)
+        # - "max_indent" actually belongs to "common_ancillaries" (see fit.py)
+        anc_ord = OrderedDict()
+        # general
+        for key in ANCILLARY_COMMON:
+            gmeth = ANCILLARY_COMMON[key][2]
+            anc_ord[key] = gmeth(fd)
+        # from module
+        if self.has_module_ancillaries:
+            anc_md = self.module.compute_ancillaries(fd)
+            for kk in self.parameter_anc_keys:
+                anc_ord[kk] = anc_md[kk]
+        return anc_ord
+
+    def get_anc_parm_keys(self):
+        """Return the key names of a model's ancillary parameters"""
+        akeys = list(ANCILLARY_COMMON.keys())
+        if self.has_module_ancillaries:
+            akeys += self.parameter_anc_keys
+        return akeys
+
+    def get_parm_name(self, key):
+        """Return parameter label
+
+        Parameters
+        ----------
+        key: str
+            The parameter key (e.g. "E")
+
+        Returns
+        -------
+        parm_name: str
+            The parameter label (e.g. "Young's Modulus")
+        """
+        if key in self.parameter_keys:
+            idx = self.parameter_keys.index(key)
+            return self.parameter_names[idx]
+        elif (self.has_module_ancillaries
+              and key in self.parameter_anc_keys):
+            idx = self.parameter_anc_keys.index(key)
+            return self.parameter_anc_names[idx]
+        elif key in ANCILLARY_COMMON:
+            return ANCILLARY_COMMON[key][0]
+        else:
+            raise KeyError(
+                f"Could not find parameter name for '{key}' in '{self}'!")
+
+    def get_parm_unit(self, key):
+        """Return parameter unit
+
+        Parameters
+        ----------
+        key: str
+            The parameter key (e.g. "E")
+
+        Returns
+        -------
+        parm_unit: str
+            The parameter unit (e.g. "Pa")
+        """
+        if key in self.parameter_keys:
+            idx = self.parameter_keys.index(key)
+            return self.parameter_units[idx]
+        elif (self.has_module_ancillaries
+              and key in self.parameter_anc_keys):
+            idx = self.parameter_anc_keys.index(key)
+            return self.parameter_anc_units[idx]
+        elif key in ANCILLARY_COMMON:
+            return ANCILLARY_COMMON[key][1]
+        else:
+            raise KeyError(
+                f"Could not find parameter unit for '{key}' in '{self}'!")
+
+
+def compute_anc_max_indent(fd):
+    """Compute ancillary parameter 'Maximum indentation'"""
+    # compute maximal indentation
+    if ("tip position" in fd
+        and "fit" in fd
+            and "params_fitted" in fd.fit_properties
+            and "contact_point" in fd.fit_properties["params_fitted"]):
+        cp = fd.fit_properties["params_fitted"]["contact_point"].value
+        idmax = fd.appr["fit"].argmax()
+        mi = fd.appr["tip position"][idmax]
+        mival = (cp-mi)
+    else:
+        mival = np.nan
+    return mival
+
+
+#: Common ancillary parameters
+ANCILLARY_COMMON = OrderedDict()
+ANCILLARY_COMMON["max_indent"] = ("Maximum indentation",
+                                  "m",
+                                  compute_anc_max_indent)
```

### Comparing `nanite-3.5.4/nanite/model/logic.py` & `nanite-3.6.0/nanite/model/logic.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-import importlib
-import pathlib
-import sys
-import warnings
-
-from .core import ModelImportError, NaniteFitModel
-
-#: currently available models
-models_available = {}
-
-
-def load_model_from_file(path, register=False):
-    """Import a fit model file and return the module
-
-    This is intended for loading custom models or for model
-    development.
-
-    Parameters
-    ----------
-    path: str or Path
-        pathname to a Python script conaining a fit model
-    register: bool
-        whether to register the model after import
-
-    Returns
-    -------
-    model: NaniteFitModel
-        nanite fit model object
-
-    Raises
-    ------
-    ModelImportError
-        If the model cannot be imported
-    """
-    path = pathlib.Path(path)
-    try:
-        # insert the plugin directory to sys.path so we can import it
-        sys.path.insert(-1, str(path.parent))
-        sys.dont_write_bytecode = True
-        module = importlib.import_module(path.stem)
-    except ModuleNotFoundError:
-        raise ModelImportError(f"Could not import '{path}'!")
-    finally:
-        # undo our path insertion
-        sys.path.pop(0)
-        sys.dont_write_bytecode = False
-
-        mod = NaniteFitModel(module)
-
-        if register:
-            register_model(module)
-
-        return mod
-
-
-def register_model(module, *args):
-    """Register a fitting model
-
-    Parameters
-    ----------
-    module: Python module or NaniteFitModel
-        the model to register
-
-    Returns
-    -------
-    model: NaniteFitModel
-        the corresponding NaniteFitModel instance
-    """
-    if args:
-        warnings.warn("Please only pass the module to `register_model`!",
-                      DeprecationWarning)
-    global models_available  # this is not necessary, but clarifies things
-    # add model
-    if isinstance(module, NaniteFitModel):
-        # we already have a fit model
-        md = module
-    else:
-        md = NaniteFitModel(module)
-    # the actual registration
-    models_available[module.model_key] = md
-    return md
-
-
-def deregister_model(model):
-    """Deregister a NaniteFitModel"""
-    global models_available  # this is not necessary, but clarifies things
-    models_available.pop(model.model_key)
+import importlib
+import pathlib
+import sys
+import warnings
+
+from .core import ModelImportError, NaniteFitModel
+
+#: currently available models
+models_available = {}
+
+
+def load_model_from_file(path, register=False):
+    """Import a fit model file and return the module
+
+    This is intended for loading custom models or for model
+    development.
+
+    Parameters
+    ----------
+    path: str or Path
+        pathname to a Python script conaining a fit model
+    register: bool
+        whether to register the model after import
+
+    Returns
+    -------
+    model: NaniteFitModel
+        nanite fit model object
+
+    Raises
+    ------
+    ModelImportError
+        If the model cannot be imported
+    """
+    path = pathlib.Path(path)
+    try:
+        # insert the plugin directory to sys.path so we can import it
+        sys.path.insert(-1, str(path.parent))
+        sys.dont_write_bytecode = True
+        module = importlib.import_module(path.stem)
+    except ModuleNotFoundError:
+        raise ModelImportError(f"Could not import '{path}'!")
+    finally:
+        # undo our path insertion
+        sys.path.pop(0)
+        sys.dont_write_bytecode = False
+
+        mod = NaniteFitModel(module)
+
+        if register:
+            register_model(module)
+
+        return mod
+
+
+def register_model(module, *args):
+    """Register a fitting model
+
+    Parameters
+    ----------
+    module: Python module or NaniteFitModel
+        the model to register
+
+    Returns
+    -------
+    model: NaniteFitModel
+        the corresponding NaniteFitModel instance
+    """
+    if args:
+        warnings.warn("Please only pass the module to `register_model`!",
+                      DeprecationWarning)
+    global models_available  # this is not necessary, but clarifies things
+    # add model
+    if isinstance(module, NaniteFitModel):
+        # we already have a fit model
+        md = module
+    else:
+        md = NaniteFitModel(module)
+    # the actual registration
+    models_available[module.model_key] = md
+    return md
+
+
+def deregister_model(model):
+    """Deregister a NaniteFitModel"""
+    global models_available  # this is not necessary, but clarifies things
+    models_available.pop(model.model_key)
```

### Comparing `nanite-3.5.4/nanite/model/model_conical_indenter.py` & `nanite-3.6.0/nanite/model/model_hertz_three_sided_pyramid.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,84 +1,82 @@
-import lmfit
-import numpy as np
-from numpy import pi
-
-
-def get_parameter_defaults():
-    """Return the default model parameters"""
-    # The order of the parameters must match the order
-    # of ´parameter_names´ and ´parameter_keys´.
-    params = lmfit.Parameters()
-    params.add("E", value=3e3, min=0)
-    params.add("alpha", value=25, min=0, max=90, vary=False)
-    params.add("nu", value=.5, min=0, max=0.5, vary=False)
-    params.add("contact_point", value=0)
-    params.add("baseline", value=0)
-    return params
-
-
-def hertz_conical(delta, E, alpha, nu, contact_point=0, baseline=0):
-    r"""Hertz model for a conical indenter
-
-    .. math::
-
-        F = \frac{2\tan\alpha}{\pi}
-            \frac{E}{1-\nu^2}
-            \delta^2
-
-    Parameters
-    ----------
-    delta: 1d ndarray
-        Indentation [m]
-    E: float
-        Young's modulus [N/m²]
-    alpha: float
-        Half cone angle [degrees]
-    nu: float
-        Poisson's ratio
-    contact_point: float
-        Indentation offset [m]
-    baseline: float
-        Force offset [N]
-
-    Returns
-    -------
-    F: float
-        Force [N]
-
-    Notes
-    -----
-    These approximations are made by the Hertz model:
-
-    - The sample is isotropic.
-    - The sample is a linear elastic solid.
-    - The sample is extended infinitely in one half space.
-    - The indenter is not deformable.
-    - There are no additional interactions between sample and indenter.
-
-    Additional assumptions:
-
-    - infinitely sharp probe
-
-    References
-    ==========
-    Love (1939) :cite:`Love1939`,
-    Sneddon (1965) :cite:`Sneddon1965` (equation 6.4)
-    """
-    aa = 2*np.tan(alpha*pi/180)/pi * E/(1-nu**2)
-    root = contact_point-delta
-    pos = root > 0
-    bb = np.zeros_like(delta)
-    bb[pos] = root[pos]**2
-    return aa*bb + baseline
-
-
-model_doc = hertz_conical.__doc__
-model_func = hertz_conical
-model_key = "hertz_cone"
-model_name = "conical indenter (Hertz)"
-parameter_keys = ["E", "alpha", "nu", "contact_point", "baseline"]
-parameter_names = ["Young's Modulus", "Half Cone Angle",
-                   "Poisson's Ratio", "Contact Point", "Force Baseline"]
-parameter_units = ["Pa", "°", "", "m", "N"]
-valid_axes_x = ["tip position"]
-valid_axes_y = ["force"]
+import lmfit
+import numpy as np
+from numpy import pi
+
+
+def get_parameter_defaults():
+    """Return the default model parameters"""
+    # The order of the parameters must match the order
+    # of ´parameter_names´ and ´parameter_keys´.
+    params = lmfit.Parameters()
+    params.add("E", value=3e3, min=0)
+    params.add("alpha", value=5, min=0, max=30, vary=False)
+    params.add("nu", value=.5, min=0, max=0.5, vary=False)
+    params.add("contact_point", value=0)
+    params.add("baseline", value=0)
+    return params
+
+
+def hertz_three_sided_pyramid(delta, E, alpha, nu, contact_point=0,
+                              baseline=0):
+    r"""Hertz model for three sided pyramidal indenter
+
+    .. math::
+
+        F = 0.887 \tan\alpha
+            \cdot \frac{E}{1-\nu^2}
+            \delta^2
+
+    Parameters
+    ----------
+    delta: 1d ndarray
+        Indentation [m]
+    E: float
+        Young's modulus [N/m²]
+    alpha: float
+        Inclination angle of the pyramidal face [degrees]
+    nu: float
+        Poisson's ratio
+    contact_point: float
+        Indentation offset [m]
+    baseline: float
+        Force offset [N]
+
+    Returns
+    -------
+    F: float
+        Force [N]
+
+    Notes
+    -----
+    These approximations are made by the Hertz model:
+
+    - The sample is isotropic.
+    - The sample is a linear elastic solid.
+    - The sample is extended infinitely in one half space.
+    - The indenter is not deformable.
+    - There are no additional interactions between sample and indenter.
+    - The inclination angle of the pyramidal face (in radians)
+      must be close to zero.
+
+    References
+    ----------
+    Bilodeau et al. 1992 :cite:`Bilodeau:1992`
+    """
+    aa = 0.8887*np.tan(alpha*pi/180) * E/(1-nu**2)
+    root = contact_point-delta
+    pos = root > 0
+    bb = np.zeros_like(delta)
+    bb[pos] = (root[pos])**(2)
+    return aa*bb + baseline
+
+
+model_doc = hertz_three_sided_pyramid.__doc__
+model_func = hertz_three_sided_pyramid
+model_key = "hertz_pyr3s"
+model_name = "pyramidal indenter, three-sided (Hertz)"
+parameter_keys = ["E", "alpha", "nu", "contact_point", "baseline"]
+parameter_names = ["Young's Modulus", "Face Angle",
+                   "Poisson's Ratio", "Contact Point", "Force Baseline"]
+parameter_units = ["Pa", "°", "", "m", "N"]
+valid_axes_x = ["tip position"]
+valid_axes_y = ["force"]
```

### Comparing `nanite-3.5.4/nanite/model/model_hertz_paraboloidal.py` & `nanite-3.6.0/nanite/model/model_hertz_paraboloidal.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,112 +1,112 @@
-import lmfit
-import numpy as np
-
-
-def get_parameter_defaults():
-    """Return the default model parameters"""
-    # The order of the parameters must match the order
-    # of ´parameter_names´ and ´parameter_keys´.
-    params = lmfit.Parameters()
-    params.add("E", value=3e3, min=0)
-    params.add("R", value=10e-6, min=0, vary=False)
-    params.add("nu", value=.5, min=0, max=0.5, vary=False)
-    params.add("contact_point", value=0)
-    params.add("baseline", value=0)
-    return params
-
-
-def hertz_paraboloidal(delta, E, R, nu, contact_point=0, baseline=0):
-    r"""Hertz model for a paraboloidal indenter
-
-    .. math::
-
-        F = \frac{4}{3}
-            \frac{E}{1-\nu^2}
-            \sqrt{R}
-            \delta^{3/2}
-
-    Parameters
-    ----------
-    delta: 1d ndarray
-        Indentation [m]
-    E: float
-        Young's modulus [N/m²]
-    R: float
-        Tip radius [m]
-    nu: float
-        Poisson's ratio
-    contact_point: float
-        Indentation offset [m]
-    baseline: float
-        Force offset [N]
-
-    Returns
-    -------
-    F: float
-        Force [N]
-
-    Notes
-    -----
-    The derivation in :cite:`Sneddon1965` reads
-
-    .. math::
-
-        F = \frac{4}{3}
-            \frac{E}{1-\nu^2}
-            \sqrt{2k}
-            \delta^{3/2},
-
-    where :math:`k` is defined by the paraboloid equation
-
-    .. math::
-
-        \rho^2 = 4kz.
-
-    As follows from the derivations in :cite:`LandauLifshitz`, this
-    model is valid for either of the two cases:
-
-    - Indentation of a plane (infinite radius) with Young's modulus
-      :math:`E` by a sphere with infinite Young's modulus and radius
-      :math:`R`, or
-    - Indentation of a sphere with radius :math:`R` and Young's modulus
-      :math:`E` by a plane (infinite radius) with infinite Young's modulus.
-
-
-    These approximations are made by the Hertz model:
-
-    - The sample is isotropic.
-    - The sample is a linear elastic solid.
-    - The sample is extended infinitely in one half space.
-    - The indenter is not deformable.
-    - There are no additional interactions between sample and indenter.
-
-    Additional assumptions:
-
-    - no surface forces
-    - If the indenter is spherical, then its radius :math:`R` is much
-      larger than the indentation depth :math:`\delta`.
-
-    References
-    ----------
-    Sneddon (1965) :cite:`Sneddon1965` (equation 6.9),
-    Theory of Elasticity by Landau and Lifshitz (1959)
-    :cite:`LandauLifshitz` (§9 Solid bodies in contact, equation 9.14)
-    """
-    aa = 4/3 * E/(1-nu**2)*np.sqrt(R)
-    root = contact_point-delta
-    pos = root > 0
-    bb = np.zeros_like(delta)
-    bb[pos] = (root[pos])**(3/2)
-    return aa*bb + baseline
-
-
-model_doc = hertz_paraboloidal.__doc__
-model_func = hertz_paraboloidal
-model_key = "hertz_para"
-model_name = "parabolic indenter (Hertz)"
-parameter_keys = ["E", "R", "nu", "contact_point", "baseline"]
-parameter_names = ["Young's Modulus", "Tip Radius",
-                   "Poisson's Ratio", "Contact Point", "Force Baseline"]
-parameter_units = ["Pa", "m", "", "m", "N"]
-valid_axes_x = ["tip position"]
-valid_axes_y = ["force"]
+import lmfit
+import numpy as np
+
+
+def get_parameter_defaults():
+    """Return the default model parameters"""
+    # The order of the parameters must match the order
+    # of ´parameter_names´ and ´parameter_keys´.
+    params = lmfit.Parameters()
+    params.add("E", value=3e3, min=0)
+    params.add("R", value=10e-6, min=0, vary=False)
+    params.add("nu", value=.5, min=0, max=0.5, vary=False)
+    params.add("contact_point", value=0)
+    params.add("baseline", value=0)
+    return params
+
+
+def hertz_paraboloidal(delta, E, R, nu, contact_point=0, baseline=0):
+    r"""Hertz model for a paraboloidal indenter
+
+    .. math::
+
+        F = \frac{4}{3}
+            \frac{E}{1-\nu^2}
+            \sqrt{R}
+            \delta^{3/2}
+
+    Parameters
+    ----------
+    delta: 1d ndarray
+        Indentation [m]
+    E: float
+        Young's modulus [N/m²]
+    R: float
+        Tip radius [m]
+    nu: float
+        Poisson's ratio
+    contact_point: float
+        Indentation offset [m]
+    baseline: float
+        Force offset [N]
+
+    Returns
+    -------
+    F: float
+        Force [N]
+
+    Notes
+    -----
+    The derivation in :cite:`Sneddon1965` reads
+
+    .. math::
+
+        F = \frac{4}{3}
+            \frac{E}{1-\nu^2}
+            \sqrt{2k}
+            \delta^{3/2},
+
+    where :math:`k` is defined by the paraboloid equation
+
+    .. math::
+
+        \rho^2 = 4kz.
+
+    As follows from the derivations in :cite:`LandauLifshitz`, this
+    model is valid for either of the two cases:
+
+    - Indentation of a plane (infinite radius) with Young's modulus
+      :math:`E` by a sphere with infinite Young's modulus and radius
+      :math:`R`, or
+    - Indentation of a sphere with radius :math:`R` and Young's modulus
+      :math:`E` by a plane (infinite radius) with infinite Young's modulus.
+
+
+    These approximations are made by the Hertz model:
+
+    - The sample is isotropic.
+    - The sample is a linear elastic solid.
+    - The sample is extended infinitely in one half space.
+    - The indenter is not deformable.
+    - There are no additional interactions between sample and indenter.
+
+    Additional assumptions:
+
+    - no surface forces
+    - If the indenter is spherical, then its radius :math:`R` is much
+      larger than the indentation depth :math:`\delta`.
+
+    References
+    ----------
+    Sneddon (1965) :cite:`Sneddon1965` (equation 6.9),
+    Theory of Elasticity by Landau and Lifshitz (1959)
+    :cite:`LandauLifshitz` (§9 Solid bodies in contact, equation 9.14)
+    """
+    aa = 4/3 * E/(1-nu**2)*np.sqrt(R)
+    root = contact_point-delta
+    pos = root > 0
+    bb = np.zeros_like(delta)
+    bb[pos] = (root[pos])**(3/2)
+    return aa*bb + baseline
+
+
+model_doc = hertz_paraboloidal.__doc__
+model_func = hertz_paraboloidal
+model_key = "hertz_para"
+model_name = "parabolic indenter (Hertz)"
+parameter_keys = ["E", "R", "nu", "contact_point", "baseline"]
+parameter_names = ["Young's Modulus", "Tip Radius",
+                   "Poisson's Ratio", "Contact Point", "Force Baseline"]
+parameter_units = ["Pa", "m", "", "m", "N"]
+valid_axes_x = ["tip position"]
+valid_axes_y = ["force"]
```

### Comparing `nanite-3.5.4/nanite/model/model_hertz_three_sided_pyramid.py` & `nanite-3.6.0/nanite/model/model_conical_indenter.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,82 +1,84 @@
-import lmfit
-import numpy as np
-from numpy import pi
-
-
-def get_parameter_defaults():
-    """Return the default model parameters"""
-    # The order of the parameters must match the order
-    # of ´parameter_names´ and ´parameter_keys´.
-    params = lmfit.Parameters()
-    params.add("E", value=3e3, min=0)
-    params.add("alpha", value=5, min=0, max=30, vary=False)
-    params.add("nu", value=.5, min=0, max=0.5, vary=False)
-    params.add("contact_point", value=0)
-    params.add("baseline", value=0)
-    return params
-
-
-def hertz_three_sided_pyramid(delta, E, alpha, nu, contact_point=0,
-                              baseline=0):
-    r"""Hertz model for three sided pyramidal indenter
-
-    .. math::
-
-        F = 0.887 \tan\alpha
-            \cdot \frac{E}{1-\nu^2}
-            \delta^2
-
-    Parameters
-    ----------
-    delta: 1d ndarray
-        Indentation [m]
-    E: float
-        Young's modulus [N/m²]
-    alpha: float
-        Inclination angle of the pyramidal face [degrees]
-    nu: float
-        Poisson's ratio
-    contact_point: float
-        Indentation offset [m]
-    baseline: float
-        Force offset [N]
-
-    Returns
-    -------
-    F: float
-        Force [N]
-
-    Notes
-    -----
-    These approximations are made by the Hertz model:
-
-    - The sample is isotropic.
-    - The sample is a linear elastic solid.
-    - The sample is extended infinitely in one half space.
-    - The indenter is not deformable.
-    - There are no additional interactions between sample and indenter.
-    - The inclination angle of the pyramidal face (in radians)
-      must be close to zero.
-
-    References
-    ----------
-    Bilodeau et al. 1992 :cite:`Bilodeau:1992`
-    """
-    aa = 0.8887*np.tan(alpha*pi/180) * E/(1-nu**2)
-    root = contact_point-delta
-    pos = root > 0
-    bb = np.zeros_like(delta)
-    bb[pos] = (root[pos])**(2)
-    return aa*bb + baseline
-
-
-model_doc = hertz_three_sided_pyramid.__doc__
-model_func = hertz_three_sided_pyramid
-model_key = "hertz_pyr3s"
-model_name = "pyramidal indenter, three-sided (Hertz)"
-parameter_keys = ["E", "alpha", "nu", "contact_point", "baseline"]
-parameter_names = ["Young's Modulus", "Face Angle",
-                   "Poisson's Ratio", "Contact Point", "Force Baseline"]
-parameter_units = ["Pa", "°", "", "m", "N"]
-valid_axes_x = ["tip position"]
-valid_axes_y = ["force"]
+import lmfit
+import numpy as np
+from numpy import pi
+
+
+def get_parameter_defaults():
+    """Return the default model parameters"""
+    # The order of the parameters must match the order
+    # of ´parameter_names´ and ´parameter_keys´.
+    params = lmfit.Parameters()
+    params.add("E", value=3e3, min=0)
+    params.add("alpha", value=25, min=0, max=90, vary=False)
+    params.add("nu", value=.5, min=0, max=0.5, vary=False)
+    params.add("contact_point", value=0)
+    params.add("baseline", value=0)
+    return params
+
+
+def hertz_conical(delta, E, alpha, nu, contact_point=0, baseline=0):
+    r"""Hertz model for a conical indenter
+
+    .. math::
+
+        F = \frac{2\tan\alpha}{\pi}
+            \frac{E}{1-\nu^2}
+            \delta^2
+
+    Parameters
+    ----------
+    delta: 1d ndarray
+        Indentation [m]
+    E: float
+        Young's modulus [N/m²]
+    alpha: float
+        Half cone angle [degrees]
+    nu: float
+        Poisson's ratio
+    contact_point: float
+        Indentation offset [m]
+    baseline: float
+        Force offset [N]
+
+    Returns
+    -------
+    F: float
+        Force [N]
+
+    Notes
+    -----
+    These approximations are made by the Hertz model:
+
+    - The sample is isotropic.
+    - The sample is a linear elastic solid.
+    - The sample is extended infinitely in one half space.
+    - The indenter is not deformable.
+    - There are no additional interactions between sample and indenter.
+
+    Additional assumptions:
+
+    - infinitely sharp probe
+
+    References
+    ==========
+    Love (1939) :cite:`Love1939`,
+    Sneddon (1965) :cite:`Sneddon1965` (equation 6.4)
+    """
+    aa = 2*np.tan(alpha*pi/180)/pi * E/(1-nu**2)
+    root = contact_point-delta
+    pos = root > 0
+    bb = np.zeros_like(delta)
+    bb[pos] = root[pos]**2
+    return aa*bb + baseline
+
+
+model_doc = hertz_conical.__doc__
+model_func = hertz_conical
+model_key = "hertz_cone"
+model_name = "conical indenter (Hertz)"
+parameter_keys = ["E", "alpha", "nu", "contact_point", "baseline"]
+parameter_names = ["Young's Modulus", "Half Cone Angle",
+                   "Poisson's Ratio", "Contact Point", "Force Baseline"]
+parameter_units = ["Pa", "°", "", "m", "N"]
+valid_axes_x = ["tip position"]
+valid_axes_y = ["force"]
```

### Comparing `nanite-3.5.4/nanite/model/model_sneddon_spherical.pyx` & `nanite-3.6.0/nanite/model/model_sneddon_spherical.pyx`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,134 +1,134 @@
-# cython: language_level=3
-# cython: binding=True
-import lmfit
-import numpy as np
-cimport numpy as np
-
-
-def get_parameter_defaults():
-    """Return the default model parameters"""
-    # The order of the parameters must match the order 
-    # of ´parameter_names´ and ´parameter_keys´.
-    params = lmfit.Parameters()
-    params.add("E", value=3e3, min=0)
-    params.add("R", value=10e-6, min=0, vary=False)
-    params.add("nu", value=.5, min=0, max=0.5, vary=False)
-    params.add("contact_point", value=0)
-    params.add("baseline", value=0)
-    return params
-
-
-def hertz_spherical(delta, double E, double R, double nu,
-                    double contact_point=0, double baseline=0):
-    r"""Hertz model for Spherical indenter - modified by Sneddon
-
-
-    .. math::
-
-        F &= \frac{E}{1-\nu^2} \left( \frac{R^2+a^2}{2} \ln \! \left(
-             \frac{R+a}{R-a}\right) -aR  \right)\\
-        \delta &= \frac{a}{2} \ln
-             \! \left(\frac{R+a}{R-a}\right)
-
-    (:math:`a` is the radius of the circular contact area between bead
-    and sample.)
-
-    Parameters
-    ----------
-    delta: 1d ndarray
-        Indentation [m]
-    E: float
-        Young's modulus [N/m²]
-    R: float
-        Tip radius [m]
-    nu: float
-        Poisson's ratio
-    contact_point: float
-        Indentation offset [m]
-    baseline: float
-        Force offset [N]
-
-    Returns
-    -------
-    F: float
-        Force [N]
-
-    Notes
-    -----
-    These approximations are made by the Hertz model:
-
-    - The sample is isotropic.
-    - The sample is a linear elastic solid.
-    - The sample is extended infinitely in one half space.
-    - The indenter is not deformable.
-    - There are no additional interactions between sample and indenter.
-
-    Additional assumptions:
-
-    - no surface forces
-
-    References
-    ----------
-    Sneddon (1965) :cite:`Sneddon1965` (equations 6.13 and 6.15)
-    """
-    cdef double a
-    cdef int ii
-    FF = np.zeros_like(delta)
-    root = delta-contact_point
-    root[root >0]=0
-    root=-1*root
-    for ii in range(root.shape[0]):
-        if root[ii]==0:
-            FF[ii]=0
-        else:
-            a=_get_a(R, root[ii])
-            FF[ii]=E/(1-nu**2)*((R**2+a**2)/2*np.log((R+a)/(R-a))-a*R) 
-    return FF + baseline
-
-
-cdef double _get_a(double R, double delta, double accuracy=1e-12):
-    cdef double a_left, a_center, a_right, d_delta, delta_predict
-    a_left=0
-    a_center=0.5*R
-    a_right=R
-    d_delta=1e200 #np.inf
-    while d_delta>accuracy:
-        delta_predict=_delta_of_a(a_center, R)
-        if delta_predict>delta:
-            a_left,a_right=a_left,a_center
-            a_center=a_left+(a_right-a_left)/2
-        elif delta_predict<delta:
-            a_left,a_right=a_center,a_right
-            a_center=a_left+(a_right-a_left)/2
-        else:
-            break
-        d_delta=abs((delta_predict-delta)/delta)
-    return a_center
-
-
-def get_a(R, delta, accuracy=1e-12):
-    """Compute the contact area radius (wrapper)"""
-    return _get_a(R, delta, accuracy)
-
-
-cdef double _delta_of_a(double a, double R):
-    cdef double delta
-    delta=a/2*np.log((R+a)/(R-a))
-    return delta
-
-
-def delta_of_a(a, R):
-    """Compute indentation from contact area radius (wrapper)"""
-    return _delta_of_a(a, R)
-
-
-model_doc = hertz_spherical.__doc__
-model_func = hertz_spherical
-model_key = "sneddon_spher"
-model_name = "spherical indenter (Sneddon)"
-parameter_keys = ["E", "R", "nu", "contact_point", "baseline"]
-parameter_names = ["Young's Modulus", "Tip Radius",
-                   "Poisson's Ratio", "Contact Point", "Force Baseline"]
-parameter_units = ["Pa", "m", "", "m", "N"]
-valid_axes_x = ["tip position"]
-valid_axes_y = ["force"]
+# cython: language_level=3
+# cython: binding=True
+import lmfit
+import numpy as np
+cimport numpy as np
+
+
+def get_parameter_defaults():
+    """Return the default model parameters"""
+    # The order of the parameters must match the order 
+    # of ´parameter_names´ and ´parameter_keys´.
+    params = lmfit.Parameters()
+    params.add("E", value=3e3, min=0)
+    params.add("R", value=10e-6, min=0, vary=False)
+    params.add("nu", value=.5, min=0, max=0.5, vary=False)
+    params.add("contact_point", value=0)
+    params.add("baseline", value=0)
+    return params
+
+
+def hertz_spherical(delta, double E, double R, double nu,
+                    double contact_point=0, double baseline=0):
+    r"""Hertz model for Spherical indenter - modified by Sneddon
+
+
+    .. math::
+
+        F &= \frac{E}{1-\nu^2} \left( \frac{R^2+a^2}{2} \ln \! \left(
+             \frac{R+a}{R-a}\right) -aR  \right)\\
+        \delta &= \frac{a}{2} \ln
+             \! \left(\frac{R+a}{R-a}\right)
+
+    (:math:`a` is the radius of the circular contact area between bead
+    and sample.)
+
+    Parameters
+    ----------
+    delta: 1d ndarray
+        Indentation [m]
+    E: float
+        Young's modulus [N/m²]
+    R: float
+        Tip radius [m]
+    nu: float
+        Poisson's ratio
+    contact_point: float
+        Indentation offset [m]
+    baseline: float
+        Force offset [N]
+
+    Returns
+    -------
+    F: float
+        Force [N]
+
+    Notes
+    -----
+    These approximations are made by the Hertz model:
+
+    - The sample is isotropic.
+    - The sample is a linear elastic solid.
+    - The sample is extended infinitely in one half space.
+    - The indenter is not deformable.
+    - There are no additional interactions between sample and indenter.
+
+    Additional assumptions:
+
+    - no surface forces
+
+    References
+    ----------
+    Sneddon (1965) :cite:`Sneddon1965` (equations 6.13 and 6.15)
+    """
+    cdef double a
+    cdef int ii
+    FF = np.zeros_like(delta)
+    root = delta-contact_point
+    root[root >0]=0
+    root=-1*root
+    for ii in range(root.shape[0]):
+        if root[ii]==0:
+            FF[ii]=0
+        else:
+            a=_get_a(R, root[ii])
+            FF[ii]=E/(1-nu**2)*((R**2+a**2)/2*np.log((R+a)/(R-a))-a*R) 
+    return FF + baseline
+
+
+cdef double _get_a(double R, double delta, double accuracy=1e-12):
+    cdef double a_left, a_center, a_right, d_delta, delta_predict
+    a_left=0
+    a_center=0.5*R
+    a_right=R
+    d_delta=1e200 #np.inf
+    while d_delta>accuracy:
+        delta_predict=_delta_of_a(a_center, R)
+        if delta_predict>delta:
+            a_left,a_right=a_left,a_center
+            a_center=a_left+(a_right-a_left)/2
+        elif delta_predict<delta:
+            a_left,a_right=a_center,a_right
+            a_center=a_left+(a_right-a_left)/2
+        else:
+            break
+        d_delta=abs((delta_predict-delta)/delta)
+    return a_center
+
+
+def get_a(R, delta, accuracy=1e-12):
+    """Compute the contact area radius (wrapper)"""
+    return _get_a(R, delta, accuracy)
+
+
+cdef double _delta_of_a(double a, double R):
+    cdef double delta
+    delta=a/2*np.log((R+a)/(R-a))
+    return delta
+
+
+def delta_of_a(a, R):
+    """Compute indentation from contact area radius (wrapper)"""
+    return _delta_of_a(a, R)
+
+
+model_doc = hertz_spherical.__doc__
+model_func = hertz_spherical
+model_key = "sneddon_spher"
+model_name = "spherical indenter (Sneddon)"
+parameter_keys = ["E", "R", "nu", "contact_point", "baseline"]
+parameter_names = ["Young's Modulus", "Tip Radius",
+                   "Poisson's Ratio", "Contact Point", "Force Baseline"]
+parameter_units = ["Pa", "m", "", "m", "N"]
+valid_axes_x = ["tip position"]
+valid_axes_y = ["force"]
```

### Comparing `nanite-3.5.4/nanite/model/model_sneddon_spherical_approximation.py` & `nanite-3.6.0/nanite/model/model_sneddon_spherical_approximation.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,101 +1,101 @@
-import lmfit
-import numpy as np
-
-
-def get_parameter_defaults():
-    """Return the default model parameters"""
-    # The order of the parameters must match the order
-    # of ´parameter_names´ and ´parameter_keys´.
-    params = lmfit.Parameters()
-    params.add("E", value=3e3, min=0)
-    params.add("R", value=10e-6, min=0, vary=False)
-    params.add("nu", value=.5, min=0, max=0.5, vary=False)
-    params.add("contact_point", value=0)
-    params.add("baseline", value=0)
-    return params
-
-
-def hertz_sneddon_spherical_approx(delta, E, R, nu, contact_point=0,
-                                   baseline=0):
-    r"""Hertz model for Spherical indenter - approximation
-
-    .. math::
-
-        F = \frac{4}{3} \frac{E}{1-\nu^2} \sqrt{R} \delta^{3/2}
-            \left(1
-             - \frac{1}{10} \frac{\delta}{R}
-             - \frac{1}{840} \left(\frac{\delta}{R}\right)^2
-             + \frac{11}{15120} \left(\frac{\delta}{R}\right)^3
-             + \frac{1357}{6652800} \left(\frac{\delta}{R}\right)^4
-             \right)
-
-    Parameters
-    ----------
-    delta: 1d ndarray
-        Indentation [m]
-    E: float
-        Young's modulus [N/m²]
-    R: float
-        Tip radius [m]
-    nu: float
-        Poisson's ratio
-    contact_point: float
-        Indentation offset [m]
-    baseline: float
-        Force offset [N]
-
-    Returns
-    -------
-    F: float
-        Force [N]
-
-    Notes
-    -----
-    These approximations are made by the Hertz model:
-
-    - The sample is isotropic.
-    - The sample is a linear elastic solid.
-    - The sample is extended infinitely in one half space.
-    - The indenter is not deformable.
-    - There are no additional interactions between sample and indenter.
-
-    Additional assumptions:
-
-    - no surface forces
-
-    Truncated power series approximation:
-
-    This model is a truncated power series approximation of
-    :ref:`sec_ref_model_sneddon_spher`. The expected error is more
-    than four magnitues lower than the signal (see e.g.
-    :ref:`example_model_spherical_indenter`). The Bio-AFM analysis software
-    by JPK/Bruker uses the same model.
-
-    References
-    ----------
-    Sneddon (1965) :cite:`Sneddon1965` (equations 6.13 and 6.15),
-    Dobler (personal communication, 2018) :cite:`Dobler`
-    """
-    aa = 4/3 * E/(1-nu**2)*np.sqrt(R)
-    root = contact_point-delta
-    pos = root > 0
-    bb = np.zeros_like(delta)
-    bb[pos] = (root[pos])**(3/2)*(
-        + 1
-        - 1/10*(root[pos]/R)
-        - 1/840*(root[pos]/R)**2
-        + 11/15120*(root[pos]/R)**3
-        + 1357/6652800*(root[pos]/R)**4)
-    return aa*bb + baseline
-
-
-model_doc = hertz_sneddon_spherical_approx.__doc__
-model_func = hertz_sneddon_spherical_approx
-model_key = "sneddon_spher_approx"
-model_name = "spherical indenter (Sneddon, truncated power series)"
-parameter_keys = ["E", "R", "nu", "contact_point", "baseline"]
-parameter_names = ["Young's Modulus", "Tip Radius",
-                   "Poisson's Ratio", "Contact Point", "Force Baseline"]
-parameter_units = ["Pa", "m", "", "m", "N"]
-valid_axes_x = ["tip position"]
-valid_axes_y = ["force"]
+import lmfit
+import numpy as np
+
+
+def get_parameter_defaults():
+    """Return the default model parameters"""
+    # The order of the parameters must match the order
+    # of ´parameter_names´ and ´parameter_keys´.
+    params = lmfit.Parameters()
+    params.add("E", value=3e3, min=0)
+    params.add("R", value=10e-6, min=0, vary=False)
+    params.add("nu", value=.5, min=0, max=0.5, vary=False)
+    params.add("contact_point", value=0)
+    params.add("baseline", value=0)
+    return params
+
+
+def hertz_sneddon_spherical_approx(delta, E, R, nu, contact_point=0,
+                                   baseline=0):
+    r"""Hertz model for Spherical indenter - approximation
+
+    .. math::
+
+        F = \frac{4}{3} \frac{E}{1-\nu^2} \sqrt{R} \delta^{3/2}
+            \left(1
+             - \frac{1}{10} \frac{\delta}{R}
+             - \frac{1}{840} \left(\frac{\delta}{R}\right)^2
+             + \frac{11}{15120} \left(\frac{\delta}{R}\right)^3
+             + \frac{1357}{6652800} \left(\frac{\delta}{R}\right)^4
+             \right)
+
+    Parameters
+    ----------
+    delta: 1d ndarray
+        Indentation [m]
+    E: float
+        Young's modulus [N/m²]
+    R: float
+        Tip radius [m]
+    nu: float
+        Poisson's ratio
+    contact_point: float
+        Indentation offset [m]
+    baseline: float
+        Force offset [N]
+
+    Returns
+    -------
+    F: float
+        Force [N]
+
+    Notes
+    -----
+    These approximations are made by the Hertz model:
+
+    - The sample is isotropic.
+    - The sample is a linear elastic solid.
+    - The sample is extended infinitely in one half space.
+    - The indenter is not deformable.
+    - There are no additional interactions between sample and indenter.
+
+    Additional assumptions:
+
+    - no surface forces
+
+    Truncated power series approximation:
+
+    This model is a truncated power series approximation of
+    :ref:`sec_ref_model_sneddon_spher`. The expected error is more
+    than four magnitues lower than the signal (see e.g.
+    :ref:`example_model_spherical_indenter`). The Bio-AFM analysis software
+    by JPK/Bruker uses the same model.
+
+    References
+    ----------
+    Sneddon (1965) :cite:`Sneddon1965` (equations 6.13 and 6.15),
+    Dobler (personal communication, 2018) :cite:`Dobler`
+    """
+    aa = 4/3 * E/(1-nu**2)*np.sqrt(R)
+    root = contact_point-delta
+    pos = root > 0
+    bb = np.zeros_like(delta)
+    bb[pos] = (root[pos])**(3/2)*(
+        + 1
+        - 1/10*(root[pos]/R)
+        - 1/840*(root[pos]/R)**2
+        + 11/15120*(root[pos]/R)**3
+        + 1357/6652800*(root[pos]/R)**4)
+    return aa*bb + baseline
+
+
+model_doc = hertz_sneddon_spherical_approx.__doc__
+model_func = hertz_sneddon_spherical_approx
+model_key = "sneddon_spher_approx"
+model_name = "spherical indenter (Sneddon, truncated power series)"
+parameter_keys = ["E", "R", "nu", "contact_point", "baseline"]
+parameter_names = ["Young's Modulus", "Tip Radius",
+                   "Poisson's Ratio", "Contact Point", "Force Baseline"]
+parameter_units = ["Pa", "m", "", "m", "N"]
+valid_axes_x = ["tip position"]
+valid_axes_y = ["force"]
```

### Comparing `nanite-3.5.4/nanite/model/residuals.py` & `nanite-3.6.0/nanite/model/residuals.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,108 +1,108 @@
-import numpy as np
-
-
-def get_default_residuals_wrapper(model_function):
-    """Return a wrapper around the default nanite residual function"""
-    default_modeling_wrapper = get_default_modeling_wrapper(model_function)
-
-    def default_residuals_wrapper(params, delta, force, weight_cp=5e-7):
-        return residual(params=params,
-                        delta=delta,
-                        force=force,
-                        model=default_modeling_wrapper,
-                        weight_cp=weight_cp)
-
-    return default_residuals_wrapper
-
-
-def get_default_modeling_wrapper(model_function):
-    """Return a wrapper around the default nanite modeling function"""
-    def default_modeling_wrapper(params, delta):
-        return model_direction_agnostic(model_function=model_function,
-                                        params=params,
-                                        delta=delta)
-    return default_modeling_wrapper
-
-
-def model_direction_agnostic(model_function, params, delta):
-    """Call `model_function` while making sure that data are in correct order
-
-    TODO: Re-evaluate usefulness of this method.
-    """
-    if delta[0] < delta[-1]:
-        revert = True
-    else:
-        revert = False
-    if revert:
-        delta = delta[::-1]
-
-    mf = model_function(delta=delta, **params.valuesdict())
-
-    if revert:
-        return mf[::-1]
-    else:
-        return mf
-
-
-def residual(params, delta, force, model, weight_cp=5e-7):
-    """Compute residuals for fitting
-
-    Parameters
-    ----------
-    params: lmfit.Parameters
-        The fitting parameters for `model`
-    delta: 1D ndarray of lenght M
-        The indentation distances
-    force: 1D ndarray of length M
-        The corresponding force data
-    model: callable
-        A model function accepting the arguments ``params``
-        and ``delta``
-    weight_cp: positive float or zero/False
-        The distance from the contact point until which
-        linear weights will be applied. Set to zero to
-        disable weighting.
-    """
-    md = model(params, delta)
-    resid = force - md
-
-    if weight_cp:
-        # weight the curve so that the data around the contact_point do
-        # not affect the fit so much.
-        weights = compute_contact_point_weights(
-            cp=params["contact_point"].value,
-            delta=delta,
-            weight_dist=weight_cp)
-        resid *= weights
-    return resid
-
-
-def compute_contact_point_weights(cp, delta, weight_dist=5e-7):
-    """Compute contact point weights
-
-    Parameters
-    ----------
-    cp: float
-        Fitted contact point value
-    delta: 1d ndarray of length N
-        The indentation array along which weights will be computed.
-    weight_width: float
-        The distance from `cp` until which weights will be applied.
-
-    Returns
-    -------
-    weights: 1d ndarray of length N
-        The weights.
-
-    Notes
-    -----
-    All variables should be given in the same units. The weights increase
-    linearly from increasing distances of `delta-cp` from 0 to 1 and are
-    1 outside of the weight width `abs(delta-cp)>weight_width`.
-    """
-    # weights are proportional to distance from contact point
-    # normalized by weight_width.
-    x = np.abs(delta-cp)
-    x /= weight_dist
-    x[x > 1] = 1
-    return x
+import numpy as np
+
+
+def get_default_residuals_wrapper(model_function):
+    """Return a wrapper around the default nanite residual function"""
+    default_modeling_wrapper = get_default_modeling_wrapper(model_function)
+
+    def default_residuals_wrapper(params, delta, force, weight_cp=5e-7):
+        return residual(params=params,
+                        delta=delta,
+                        force=force,
+                        model=default_modeling_wrapper,
+                        weight_cp=weight_cp)
+
+    return default_residuals_wrapper
+
+
+def get_default_modeling_wrapper(model_function):
+    """Return a wrapper around the default nanite modeling function"""
+    def default_modeling_wrapper(params, delta):
+        return model_direction_agnostic(model_function=model_function,
+                                        params=params,
+                                        delta=delta)
+    return default_modeling_wrapper
+
+
+def model_direction_agnostic(model_function, params, delta):
+    """Call `model_function` while making sure that data are in correct order
+
+    TODO: Re-evaluate usefulness of this method.
+    """
+    if delta[0] < delta[-1]:
+        revert = True
+    else:
+        revert = False
+    if revert:
+        delta = delta[::-1]
+
+    mf = model_function(delta=delta, **params.valuesdict())
+
+    if revert:
+        return mf[::-1]
+    else:
+        return mf
+
+
+def residual(params, delta, force, model, weight_cp=5e-7):
+    """Compute residuals for fitting
+
+    Parameters
+    ----------
+    params: lmfit.Parameters
+        The fitting parameters for `model`
+    delta: 1D ndarray of lenght M
+        The indentation distances
+    force: 1D ndarray of length M
+        The corresponding force data
+    model: callable
+        A model function accepting the arguments ``params``
+        and ``delta``
+    weight_cp: positive float or zero/False
+        The distance from the contact point until which
+        linear weights will be applied. Set to zero to
+        disable weighting.
+    """
+    md = model(params, delta)
+    resid = force - md
+
+    if weight_cp:
+        # weight the curve so that the data around the contact_point do
+        # not affect the fit so much.
+        weights = compute_contact_point_weights(
+            cp=params["contact_point"].value,
+            delta=delta,
+            weight_dist=weight_cp)
+        resid *= weights
+    return resid
+
+
+def compute_contact_point_weights(cp, delta, weight_dist=5e-7):
+    """Compute contact point weights
+
+    Parameters
+    ----------
+    cp: float
+        Fitted contact point value
+    delta: 1d ndarray of length N
+        The indentation array along which weights will be computed.
+    weight_width: float
+        The distance from `cp` until which weights will be applied.
+
+    Returns
+    -------
+    weights: 1d ndarray of length N
+        The weights.
+
+    Notes
+    -----
+    All variables should be given in the same units. The weights increase
+    linearly from increasing distances of `delta-cp` from 0 to 1 and are
+    1 outside of the weight width `abs(delta-cp)>weight_width`.
+    """
+    # weights are proportional to distance from contact point
+    # normalized by weight_width.
+    x = np.abs(delta-cp)
+    x /= weight_dist
+    x[x > 1] = 1
+    return x
```

### Comparing `nanite-3.5.4/nanite/poc.py` & `nanite-3.6.0/nanite/poc.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,477 +1,477 @@
-"""Methods for estimating the point of contact (POC)"""
-import lmfit
-import numpy as np
-from scipy.ndimage import uniform_filter1d
-
-
-#: List of all methods available for contact point estimation
-POC_METHODS = []
-
-
-def compute_preproc_clip_approach(force):
-    """Clip the approach part (discard the retract part)
-
-    This POC preprocessing method may be applied before
-    applying the POC estimation method.
-    """
-    # get data
-    fg0 = np.array(force, copy=True)
-    # Only use the (initial) approach part of the curve.
-    idmax = np.argmax(fg0)
-    fg = fg0[:idmax]
-    return fg
-
-
-def compute_poc(force, method="deviation_from_baseline", ret_details=False):
-    """Compute the contact point from force data
-
-    Parameters
-    ----------
-    force: 1d ndarray
-        Force data
-    method: str
-        Name of the method for computing the POC (see :const:`POC_METHODS`)
-    ret_details: bool
-        Whether or not to return a dictionary with details alongside the
-        POC estimate.
-
-    Notes
-    -----
-    If the POC method returns np.nan, then the center of the
-    force data is returned (to allow fitting algorithms to proceed).
-    """
-    # compute POC according to method chosen
-    for mfunc in POC_METHODS:
-        if mfunc.identifier == method:
-            if "clip_approach" in mfunc.preprocessing:
-                force = compute_preproc_clip_approach(force)
-            data = mfunc(force, ret_details=ret_details)
-            if ret_details:
-                cp, details = data
-                details["method"] = method
-            else:
-                cp, details = data, None
-            break
-    else:
-        raise ValueError(f"Undefined POC method '{method}'!")
-    if np.isnan(cp):
-        cp = force.size // 2
-    if ret_details:
-        return cp, details
-    else:
-        return cp
-
-
-def poc(identifier, name, preprocessing):
-    """Decorator for point of contact (POC) methods
-
-    The name and identifier are stored as a property of the wrapped
-    function.
-
-    Parameters
-    ----------
-    identifier: str
-        identifier of the POC method (e.g. "baseline_deviation")
-    name: str
-        human-readble name of the POC method
-        (e.g. "Deviation from baseline")
-    preprocessing: list of str
-        list of preprocessing methods that should be applied;
-        may contain ["clip_approach"].
-    """
-    def attribute_setter(func):
-        """Decorator that sets the necessary attributes
-
-        The outer decorator is used to obtain the attributes.
-        This inner decorator returns the actual function that
-        wraps the preprocessor.
-        """
-        POC_METHODS.append(func)
-        func.identifier = identifier
-        func.name = name
-        func.preprocessing = preprocessing
-        return func
-
-    return attribute_setter
-
-
-@poc(identifier="deviation_from_baseline",
-     name="Deviation from baseline",
-     preprocessing=["clip_approach"])
-def poc_deviation_from_baseline(force, ret_details=False):
-    """Deviation from baseline
-
-    1. Obtain the baseline (initial 10% of the gradient curve)
-    2. Compute average and maximum deviation of the baseline
-    3. The CP is the index of the curve where it exceeds
-       twice of the maximum deviation
-    """
-    cp = np.nan
-    details = {}
-    # Crop the slow approach trace (10% of the curve)
-    baseline = force[:int(force.size * .1)]
-    if baseline.size:
-        bl_avg = np.average(baseline)
-        bl_rng = np.max(np.abs(baseline - bl_avg)) * 2
-        bl_dev = (force - bl_avg) > bl_rng
-        # argmax gets the first largest value
-        maxid = np.argmax(bl_dev)
-        if bl_dev[maxid]:
-            cp = maxid
-        if ret_details:
-            x = [0, force.size-1]
-            details["plot force"] = [np.arange(force.size), force]
-            details["plot baseline mean"] = [x, [bl_avg, bl_avg]]
-            details["plot baseline threshold"] = [x, [bl_avg + bl_rng,
-                                                      bl_avg + bl_rng]]
-            details["plot poc"] = [[cp, cp],
-                                   [force.min(), force.max()]]
-
-    if ret_details:
-        return cp, details
-    else:
-        return cp
-
-
-@poc(identifier="fit_constant_line",
-     name="Piecewise fit with constant and line",
-     preprocessing=["clip_approach"])
-def poc_fit_constant_line(force, ret_details=False):
-    r"""Piecewise fit with constant and line
-
-    Fit a piecewise function (constant+linear) to the baseline
-    and indentation part:
-
-    .. math::
-
-       F = \text{max}(d, m\delta + d)
-
-    The point of contact is the intersection of a horizontal line
-    at :math:`d` (baseline) and a linear function with slope :math:`m`
-    for the indentation part.
-
-    The point of contact is defined as :math:`\delta=0` (It's another
-    fitting parameter).
-    """
-    def model(params, x):
-        d = params["d"]
-        x0 = params["x0"]
-        m = params["m"]
-        one = d
-        two = m * (x - x0) + d
-        return np.maximum(one, two)
-
-    def residual(params, x, data):
-        return data - model(params, x)
-
-    y = np.array(force, copy=True)
-    cp = np.nan
-    details = {}
-    if y.size > 4:  # 3 fit parameters
-        ymin, ymax = np.min(y), np.max(y)
-        y = (y - ymin) / (ymax - ymin)
-        x = np.arange(y.size)
-        x0 = poc_frechet_direct_path(force)
-        if np.isnan(x0):
-            x0 = y.size // 2
-        params = lmfit.Parameters()
-        params.add('d', value=np.mean(y[:10]))
-        params.add('x0', value=x0)
-        params.add('m', value=(1 - y[x0])/(x.size - x0))
-
-        out = lmfit.minimize(residual, params, args=(x, y), method="nelder")
-        if out.success:
-            cp = int(out.params["x0"])
-            if ret_details:
-                details["plot force"] = [x, y]
-                details["plot fit"] = [np.arange(force.size),
-                                       model(out.params, x)]
-                details["plot poc"] = [[cp, cp],
-                                       [y.min(), y.max()]]
-
-    if ret_details:
-        return cp, details
-    else:
-        return cp
-
-
-@poc(identifier="fit_constant_polynomial",
-     name="Piecewise fit with constant and polynomial",
-     preprocessing=["clip_approach"])
-def poc_fit_constant_polynomial(force, ret_details=False):
-    r"""Piecewise fit with constant and polynomial
-
-    Fit a piecewise function (constant + polynomial) to the baseline
-    and indentation part.
-
-    .. math::
-
-       F = \frac{\delta^3}{a\delta^2 + b\delta + c} + d
-
-    This function is defined for all :math:`\delta>0`. For all
-    :math:`\delta<0` the model evaluates to :math:`d` (baseline).
-
-    I'm not sure where this has been described initially, but it is
-    used e.g. in :cite:`Rusaczonek19`.
-
-    For small indentations, this function exhibits a cubic behavior:
-
-    .. math::
-
-       y \approx \delta^3/c + d
-
-    And for large indentations, this function is linear:
-
-    .. math::
-
-       y \approx \delta/a
-
-    The point of contact is defined as :math:`\delta=0` (It's another
-    fitting parameter).
-    """
-    def model(params, x):
-        d = params["d"].value
-        x0 = params["x0"].value
-        a = params["a"].value
-        b = params["b"].value
-        c = params["c"].value
-        x1 = x - x0
-        curve = x1**3 / (a*x1**2 + b*x1 + c) + d
-        curve[x1 <= 0] = d
-        return curve
-
-    def residual(params, x, data):
-        curve = model(params, x)
-        return data - curve
-
-    y = np.array(force, copy=True)
-    cp = np.nan
-    details = {}
-    if y.size > 6:  # 5 fit parameters
-        ymin, ymax = np.min(y), np.max(y)
-        y = (y - ymin) / (ymax - ymin)
-        x = np.arange(y.size)
-        x0 = poc_frechet_direct_path(force)
-        if np.isnan(x0):
-            x0 = y.size // 2
-        params = lmfit.Parameters()
-        params.add('d', value=np.mean(y[:10]))
-        params.add('x0', value=x0)
-        # The polynomial fitting parameters are supposed to be
-        # greater than zero (source?). We set the minimum to 1e-3 so
-        # the fitting algorithm becomes more stable. Also, the initial
-        # values for b and c are more or less arbitrary (this is a heuristic
-        # approach).
-        # for larger x, a is something like an inverse slope. Since we
-        # normalized the y-values to 1, we just take the x-difference.
-        params.add('a', value=(y.size-x0), min=1e-3, max=100*(y.size-x0))
-        params.add('b', value=y.size, min=1e-3)
-        params.add('c', value=.5, min=1e-3)
-
-        out = lmfit.minimize(residual, params, args=(x, y), method="nelder")
-
-        if out.success:
-            cp = int(out.params["x0"])
-            if ret_details:
-                details["plot force"] = [x, y]
-                details["plot fit"] = [np.arange(force.size),
-                                       model(out.params, x)]
-                details["plot poc"] = [[cp, cp],
-                                       [y.min(), y.max()]]
-
-    if ret_details:
-        return cp, details
-    else:
-        return cp
-
-
-@poc(identifier="fit_line_polynomial",
-     name="Piecewise fit with line and polynomial",
-     preprocessing=["clip_approach"])
-def poc_fit_line_polynomial(force, ret_details=False):
-    r"""Piecewise fit with line and polynomial
-
-    Fit a piecewise function (line + polynomial) to the baseline
-    and indentation part.
-
-    The linear basline (:math:`\delta<0`) is modeled with:
-
-    .. math::
-
-       F = m \delta + d
-
-    The indentation part (:math:`\delta>0`) is modeled with:
-
-    .. math::
-
-       F = \frac{\delta^3}{a\delta^2 + b\delta + c} + m \delta  + d
-
-    For small indentations, this function exhibits a linear and
-    only slightly cubic behavior:
-
-    .. math::
-
-       y \approx \delta^3/c + m \delta + d
-
-    And for large indentations, this function is linear:
-
-    .. math::
-
-       y \approx \left( \frac{1}{a} + m \right) \delta
-
-    The point of contact is defined as :math:`\delta=0` (It's another
-    fitting parameter).
-
-
-    See Also
-    --------
-    poc_fit_constant_polynomial: polynomial-only version
-    """
-    def model(params, x):
-        d = params["d"].value
-        x0 = params["x0"].value
-        m = params["m"].value
-        a = params["a"].value
-        b = params["b"].value
-        c = params["c"].value
-        x1 = x - x0
-        curve = m * x1 + d
-        curve[x1 > 0] += x1[x1 > 0]**3 / (a*x1[x1 > 0]**2 + b*x1[x1 > 0] + c)
-        return curve
-
-    def residual(params, x, data):
-        curve = model(params, x)
-        return data - curve
-
-    y = np.array(force, copy=True)
-    cp = np.nan
-    details = {}
-    if y.size > 7:  # 6 fit parameters
-        ymin, ymax = np.min(y), np.max(y)
-        y = (y - ymin) / (ymax - ymin)
-        x = np.arange(y.size)
-        x0 = poc_frechet_direct_path(force)
-        if np.isnan(x0):
-            x0 = y.size // 2
-        params = lmfit.Parameters()
-        params.add('d', value=np.mean(y[:10]))
-        params.add('x0', value=x0)
-        # slope
-        params.add('m', value=y[x0]/x0)
-        # The polynomial fitting parameters are supposed to be
-        # greater than zero (source?). We set the minimum to 1e-3 so
-        # the fitting algorithm becomes more stable. Also, the initial
-        # values for b and c are more or less arbitrary (this is a heuristic
-        # approach).
-        # for larger x, a is something like an inverse slope. Since we
-        # normalized the y-values to 1, we just take the x-difference.
-        params.add('a', value=(y.size-x0), min=1e-3, max=100*(y.size-x0))
-        params.add('b', value=y.size, min=1e-3)
-        params.add('c', value=.5, min=1e-3)
-
-        out = lmfit.minimize(residual, params, args=(x, y), method="nelder")
-
-        if out.success:
-            cp = int(out.params["x0"])
-            if ret_details:
-                details["plot force"] = [x, y]
-                details["plot fit"] = [np.arange(force.size),
-                                       model(out.params, x)]
-                details["plot poc"] = [[cp, cp],
-                                       [y.min(), y.max()]]
-                print(cp, y.min(), y.max())
-
-    if ret_details:
-        return cp, details
-    else:
-        return cp
-
-
-@poc(identifier="frechet_direct_path",
-     name="Fréchet distance to direct path",
-     preprocessing=["clip_approach"])
-def poc_frechet_direct_path(force, ret_details=False):
-    """Fréchet distance to direct path
-
-    The indentation part is transformed to normalized coordinates
-    (force and corresponding x in range [0, 1]). The point with the
-    largest distance to the line from (0, 0) to (1, 1) is the contact
-    point.
-
-    This method is robust with regard to tilted baselines and is a
-    good initial guess for fitting-based POC estimation approaches.
-
-    Note that the length of the baseline influences the returned
-    contact point. For shorter baselines, the contact point will
-    be closer to the point of maximum indentation.
-    """
-    x = np.linspace(0, 1, len(force), endpoint=True)
-    y = (force - force.min()) / (force.max() - force.min())
-
-    # rotate the curve towards x
-    # (computation of Frechet distance with curve is now just distance
-    # from x-axis, i.e. minimum)
-    alpha = - np.pi / 4
-    yr = x * np.sin(alpha) + y * np.cos(alpha)
-    cp = np.argmin(yr)
-
-    if ret_details:
-        details = {"plot normalized rotated force": [np.arange(len(force)),
-                                                     yr],
-                   "plot poc": [[cp, cp],
-                                [yr.min(), yr.max()]]}
-        return cp, details
-    else:
-        return cp
-
-
-@poc(identifier="gradient_zero_crossing",
-     name="Gradient zero-crossing of indentation part",
-     preprocessing=["clip_approach"])
-def poc_gradient_zero_crossing(force, ret_details=False):
-    """Gradient zero-crossing of indentation part
-
-    1. Apply a moving average filter to the curve
-    2. Compute the gradient
-    3. Cut off gradient at maximum with a 10 point reserve
-    4. Apply a moving average filter to the gradient
-    5. The POC is the index of the averaged gradient curve where
-       the values are below 1% of the gradient maximum, measured
-       from the indentation maximum (not from baseline).
-    """
-    cp = np.nan
-    details = {}
-    # Perform a median filter to smooth the array
-    filtsize = max(5, int(force.size*.01))
-    y = uniform_filter1d(force, size=filtsize)
-    if y.size > 1:
-        # Cutoff at maximum plus some reserve
-        cutoff = y.size - np.argmax(y) + 10
-        grad = np.gradient(y)[:-cutoff]
-        if grad.size > 50:
-            # Use the point where the gradient becomes small enough.
-            gradn = uniform_filter1d(grad, size=filtsize)
-            thresh = 0.01 * np.max(gradn)
-            gradpos = gradn <= thresh
-            if np.sum(gradpos):
-                # The gradient contains positive values.
-                # Flip `gradpos`, because we want the first value from the
-                # end of the array.
-                # Weight with two times "filtsize//2", because we actually
-                # want the rolling median filter from the edge and not at the
-                # center of the array (and two times, because we did two
-                # filter operations).
-                cp = y.size - np.where(gradpos[::-1])[0][0] - cutoff + filtsize
-
-                if ret_details:
-                    x = np.arange(gradn.size)
-                    details["plot force gradient"] = [x, gradn]
-                    details["plot threshold"] = [[x[0], x[-1]],
-                                                 [thresh, thresh]]
-                    details["plot poc"] = [[cp, cp],
-                                           [gradn.min(), gradn.max()]]
-
-    if ret_details:
-        return cp, details
-    else:
-        return cp
+"""Methods for estimating the point of contact (POC)"""
+import lmfit
+import numpy as np
+from scipy.ndimage import uniform_filter1d
+
+
+#: List of all methods available for contact point estimation
+POC_METHODS = []
+
+
+def compute_preproc_clip_approach(force):
+    """Clip the approach part (discard the retract part)
+
+    This POC preprocessing method may be applied before
+    applying the POC estimation method.
+    """
+    # get data
+    fg0 = np.array(force, copy=True)
+    # Only use the (initial) approach part of the curve.
+    idmax = np.argmax(fg0)
+    fg = fg0[:idmax]
+    return fg
+
+
+def compute_poc(force, method="deviation_from_baseline", ret_details=False):
+    """Compute the contact point from force data
+
+    Parameters
+    ----------
+    force: 1d ndarray
+        Force data
+    method: str
+        Name of the method for computing the POC (see :const:`POC_METHODS`)
+    ret_details: bool
+        Whether or not to return a dictionary with details alongside the
+        POC estimate.
+
+    Notes
+    -----
+    If the POC method returns np.nan, then the center of the
+    force data is returned (to allow fitting algorithms to proceed).
+    """
+    # compute POC according to method chosen
+    for mfunc in POC_METHODS:
+        if mfunc.identifier == method:
+            if "clip_approach" in mfunc.preprocessing:
+                force = compute_preproc_clip_approach(force)
+            data = mfunc(force, ret_details=ret_details)
+            if ret_details:
+                cp, details = data
+                details["method"] = method
+            else:
+                cp, details = data, None
+            break
+    else:
+        raise ValueError(f"Undefined POC method '{method}'!")
+    if np.isnan(cp):
+        cp = force.size // 2
+    if ret_details:
+        return cp, details
+    else:
+        return cp
+
+
+def poc(identifier, name, preprocessing):
+    """Decorator for point of contact (POC) methods
+
+    The name and identifier are stored as a property of the wrapped
+    function.
+
+    Parameters
+    ----------
+    identifier: str
+        identifier of the POC method (e.g. "baseline_deviation")
+    name: str
+        human-readble name of the POC method
+        (e.g. "Deviation from baseline")
+    preprocessing: list of str
+        list of preprocessing methods that should be applied;
+        may contain ["clip_approach"].
+    """
+    def attribute_setter(func):
+        """Decorator that sets the necessary attributes
+
+        The outer decorator is used to obtain the attributes.
+        This inner decorator returns the actual function that
+        wraps the preprocessor.
+        """
+        POC_METHODS.append(func)
+        func.identifier = identifier
+        func.name = name
+        func.preprocessing = preprocessing
+        return func
+
+    return attribute_setter
+
+
+@poc(identifier="deviation_from_baseline",
+     name="Deviation from baseline",
+     preprocessing=["clip_approach"])
+def poc_deviation_from_baseline(force, ret_details=False):
+    """Deviation from baseline
+
+    1. Obtain the baseline (initial 10% of the gradient curve)
+    2. Compute average and maximum deviation of the baseline
+    3. The CP is the index of the curve where it exceeds
+       twice of the maximum deviation
+    """
+    cp = np.nan
+    details = {}
+    # Crop the slow approach trace (10% of the curve)
+    baseline = force[:int(force.size * .1)]
+    if baseline.size:
+        bl_avg = np.average(baseline)
+        bl_rng = np.max(np.abs(baseline - bl_avg)) * 2
+        bl_dev = (force - bl_avg) > bl_rng
+        # argmax gets the first largest value
+        maxid = np.argmax(bl_dev)
+        if bl_dev[maxid]:
+            cp = maxid
+        if ret_details:
+            x = [0, force.size-1]
+            details["plot force"] = [np.arange(force.size), force]
+            details["plot baseline mean"] = [x, [bl_avg, bl_avg]]
+            details["plot baseline threshold"] = [x, [bl_avg + bl_rng,
+                                                      bl_avg + bl_rng]]
+            details["plot poc"] = [[cp, cp],
+                                   [force.min(), force.max()]]
+
+    if ret_details:
+        return cp, details
+    else:
+        return cp
+
+
+@poc(identifier="fit_constant_line",
+     name="Piecewise fit with constant and line",
+     preprocessing=["clip_approach"])
+def poc_fit_constant_line(force, ret_details=False):
+    r"""Piecewise fit with constant and line
+
+    Fit a piecewise function (constant+linear) to the baseline
+    and indentation part:
+
+    .. math::
+
+       F = \text{max}(d, m\delta + d)
+
+    The point of contact is the intersection of a horizontal line
+    at :math:`d` (baseline) and a linear function with slope :math:`m`
+    for the indentation part.
+
+    The point of contact is defined as :math:`\delta=0` (It's another
+    fitting parameter).
+    """
+    def model(params, x):
+        d = params["d"]
+        x0 = params["x0"]
+        m = params["m"]
+        one = d
+        two = m * (x - x0) + d
+        return np.maximum(one, two)
+
+    def residual(params, x, data):
+        return data - model(params, x)
+
+    y = np.array(force, copy=True)
+    cp = np.nan
+    details = {}
+    if y.size > 4:  # 3 fit parameters
+        ymin, ymax = np.min(y), np.max(y)
+        y = (y - ymin) / (ymax - ymin)
+        x = np.arange(y.size)
+        x0 = poc_frechet_direct_path(force)
+        if np.isnan(x0):
+            x0 = y.size // 2
+        params = lmfit.Parameters()
+        params.add('d', value=np.mean(y[:10]))
+        params.add('x0', value=x0)
+        params.add('m', value=(1 - y[x0])/(x.size - x0))
+
+        out = lmfit.minimize(residual, params, args=(x, y), method="nelder")
+        if out.success:
+            cp = int(out.params["x0"])
+            if ret_details:
+                details["plot force"] = [x, y]
+                details["plot fit"] = [np.arange(force.size),
+                                       model(out.params, x)]
+                details["plot poc"] = [[cp, cp],
+                                       [y.min(), y.max()]]
+
+    if ret_details:
+        return cp, details
+    else:
+        return cp
+
+
+@poc(identifier="fit_constant_polynomial",
+     name="Piecewise fit with constant and polynomial",
+     preprocessing=["clip_approach"])
+def poc_fit_constant_polynomial(force, ret_details=False):
+    r"""Piecewise fit with constant and polynomial
+
+    Fit a piecewise function (constant + polynomial) to the baseline
+    and indentation part.
+
+    .. math::
+
+       F = \frac{\delta^3}{a\delta^2 + b\delta + c} + d
+
+    This function is defined for all :math:`\delta>0`. For all
+    :math:`\delta<0` the model evaluates to :math:`d` (baseline).
+
+    I'm not sure where this has been described initially, but it is
+    used e.g. in :cite:`Rusaczonek19`.
+
+    For small indentations, this function exhibits a cubic behavior:
+
+    .. math::
+
+       y \approx \delta^3/c + d
+
+    And for large indentations, this function is linear:
+
+    .. math::
+
+       y \approx \delta/a
+
+    The point of contact is defined as :math:`\delta=0` (It's another
+    fitting parameter).
+    """
+    def model(params, x):
+        d = params["d"].value
+        x0 = params["x0"].value
+        a = params["a"].value
+        b = params["b"].value
+        c = params["c"].value
+        x1 = x - x0
+        curve = x1**3 / (a*x1**2 + b*x1 + c) + d
+        curve[x1 <= 0] = d
+        return curve
+
+    def residual(params, x, data):
+        curve = model(params, x)
+        return data - curve
+
+    y = np.array(force, copy=True)
+    cp = np.nan
+    details = {}
+    if y.size > 6:  # 5 fit parameters
+        ymin, ymax = np.min(y), np.max(y)
+        y = (y - ymin) / (ymax - ymin)
+        x = np.arange(y.size)
+        x0 = poc_frechet_direct_path(force)
+        if np.isnan(x0):
+            x0 = y.size // 2
+        params = lmfit.Parameters()
+        params.add('d', value=np.mean(y[:10]))
+        params.add('x0', value=x0)
+        # The polynomial fitting parameters are supposed to be
+        # greater than zero (source?). We set the minimum to 1e-3 so
+        # the fitting algorithm becomes more stable. Also, the initial
+        # values for b and c are more or less arbitrary (this is a heuristic
+        # approach).
+        # for larger x, a is something like an inverse slope. Since we
+        # normalized the y-values to 1, we just take the x-difference.
+        params.add('a', value=(y.size-x0), min=1e-3, max=100*(y.size-x0))
+        params.add('b', value=y.size, min=1e-3)
+        params.add('c', value=.5, min=1e-3)
+
+        out = lmfit.minimize(residual, params, args=(x, y), method="nelder")
+
+        if out.success:
+            cp = int(out.params["x0"])
+            if ret_details:
+                details["plot force"] = [x, y]
+                details["plot fit"] = [np.arange(force.size),
+                                       model(out.params, x)]
+                details["plot poc"] = [[cp, cp],
+                                       [y.min(), y.max()]]
+
+    if ret_details:
+        return cp, details
+    else:
+        return cp
+
+
+@poc(identifier="fit_line_polynomial",
+     name="Piecewise fit with line and polynomial",
+     preprocessing=["clip_approach"])
+def poc_fit_line_polynomial(force, ret_details=False):
+    r"""Piecewise fit with line and polynomial
+
+    Fit a piecewise function (line + polynomial) to the baseline
+    and indentation part.
+
+    The linear basline (:math:`\delta<0`) is modeled with:
+
+    .. math::
+
+       F = m \delta + d
+
+    The indentation part (:math:`\delta>0`) is modeled with:
+
+    .. math::
+
+       F = \frac{\delta^3}{a\delta^2 + b\delta + c} + m \delta  + d
+
+    For small indentations, this function exhibits a linear and
+    only slightly cubic behavior:
+
+    .. math::
+
+       y \approx \delta^3/c + m \delta + d
+
+    And for large indentations, this function is linear:
+
+    .. math::
+
+       y \approx \left( \frac{1}{a} + m \right) \delta
+
+    The point of contact is defined as :math:`\delta=0` (It's another
+    fitting parameter).
+
+
+    See Also
+    --------
+    poc_fit_constant_polynomial: polynomial-only version
+    """
+    def model(params, x):
+        d = params["d"].value
+        x0 = params["x0"].value
+        m = params["m"].value
+        a = params["a"].value
+        b = params["b"].value
+        c = params["c"].value
+        x1 = x - x0
+        curve = m * x1 + d
+        curve[x1 > 0] += x1[x1 > 0]**3 / (a*x1[x1 > 0]**2 + b*x1[x1 > 0] + c)
+        return curve
+
+    def residual(params, x, data):
+        curve = model(params, x)
+        return data - curve
+
+    y = np.array(force, copy=True)
+    cp = np.nan
+    details = {}
+    if y.size > 7:  # 6 fit parameters
+        ymin, ymax = np.min(y), np.max(y)
+        y = (y - ymin) / (ymax - ymin)
+        x = np.arange(y.size)
+        x0 = poc_frechet_direct_path(force)
+        if np.isnan(x0):
+            x0 = y.size // 2
+        params = lmfit.Parameters()
+        params.add('d', value=np.mean(y[:10]))
+        params.add('x0', value=x0)
+        # slope
+        params.add('m', value=y[x0]/x0)
+        # The polynomial fitting parameters are supposed to be
+        # greater than zero (source?). We set the minimum to 1e-3 so
+        # the fitting algorithm becomes more stable. Also, the initial
+        # values for b and c are more or less arbitrary (this is a heuristic
+        # approach).
+        # for larger x, a is something like an inverse slope. Since we
+        # normalized the y-values to 1, we just take the x-difference.
+        params.add('a', value=(y.size-x0), min=1e-3, max=100*(y.size-x0))
+        params.add('b', value=y.size, min=1e-3)
+        params.add('c', value=.5, min=1e-3)
+
+        out = lmfit.minimize(residual, params, args=(x, y), method="nelder")
+
+        if out.success:
+            cp = int(out.params["x0"])
+            if ret_details:
+                details["plot force"] = [x, y]
+                details["plot fit"] = [np.arange(force.size),
+                                       model(out.params, x)]
+                details["plot poc"] = [[cp, cp],
+                                       [y.min(), y.max()]]
+                print(cp, y.min(), y.max())
+
+    if ret_details:
+        return cp, details
+    else:
+        return cp
+
+
+@poc(identifier="frechet_direct_path",
+     name="Fréchet distance to direct path",
+     preprocessing=["clip_approach"])
+def poc_frechet_direct_path(force, ret_details=False):
+    """Fréchet distance to direct path
+
+    The indentation part is transformed to normalized coordinates
+    (force and corresponding x in range [0, 1]). The point with the
+    largest distance to the line from (0, 0) to (1, 1) is the contact
+    point.
+
+    This method is robust with regard to tilted baselines and is a
+    good initial guess for fitting-based POC estimation approaches.
+
+    Note that the length of the baseline influences the returned
+    contact point. For shorter baselines, the contact point will
+    be closer to the point of maximum indentation.
+    """
+    x = np.linspace(0, 1, len(force), endpoint=True)
+    y = (force - force.min()) / (force.max() - force.min())
+
+    # rotate the curve towards x
+    # (computation of Frechet distance with curve is now just distance
+    # from x-axis, i.e. minimum)
+    alpha = - np.pi / 4
+    yr = x * np.sin(alpha) + y * np.cos(alpha)
+    cp = np.argmin(yr)
+
+    if ret_details:
+        details = {"plot normalized rotated force": [np.arange(len(force)),
+                                                     yr],
+                   "plot poc": [[cp, cp],
+                                [yr.min(), yr.max()]]}
+        return cp, details
+    else:
+        return cp
+
+
+@poc(identifier="gradient_zero_crossing",
+     name="Gradient zero-crossing of indentation part",
+     preprocessing=["clip_approach"])
+def poc_gradient_zero_crossing(force, ret_details=False):
+    """Gradient zero-crossing of indentation part
+
+    1. Apply a moving average filter to the curve
+    2. Compute the gradient
+    3. Cut off gradient at maximum with a 10 point reserve
+    4. Apply a moving average filter to the gradient
+    5. The POC is the index of the averaged gradient curve where
+       the values are below 1% of the gradient maximum, measured
+       from the indentation maximum (not from baseline).
+    """
+    cp = np.nan
+    details = {}
+    # Perform a median filter to smooth the array
+    filtsize = max(5, int(force.size*.01))
+    y = uniform_filter1d(force, size=filtsize)
+    if y.size > 1:
+        # Cutoff at maximum plus some reserve
+        cutoff = y.size - np.argmax(y) + 10
+        grad = np.gradient(y)[:-cutoff]
+        if grad.size > 50:
+            # Use the point where the gradient becomes small enough.
+            gradn = uniform_filter1d(grad, size=filtsize)
+            thresh = 0.01 * np.max(gradn)
+            gradpos = gradn <= thresh
+            if np.sum(gradpos):
+                # The gradient contains positive values.
+                # Flip `gradpos`, because we want the first value from the
+                # end of the array.
+                # Weight with two times "filtsize//2", because we actually
+                # want the rolling median filter from the edge and not at the
+                # center of the array (and two times, because we did two
+                # filter operations).
+                cp = y.size - np.where(gradpos[::-1])[0][0] - cutoff + filtsize
+
+                if ret_details:
+                    x = np.arange(gradn.size)
+                    details["plot force gradient"] = [x, gradn]
+                    details["plot threshold"] = [[x[0], x[-1]],
+                                                 [thresh, thresh]]
+                    details["plot poc"] = [[cp, cp],
+                                           [gradn.min(), gradn.max()]]
+
+    if ret_details:
+        return cp, details
+    else:
+        return cp
```

### Comparing `nanite-3.5.4/nanite/qmap.py` & `nanite-3.6.0/nanite/qmap.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,85 +1,85 @@
-import warnings
-
-import afmformats
-from afmformats.afm_qmap import qmap_feature
-import numpy as np
-
-from .read import get_load_data_modality_kwargs
-
-
-class DataMissingWarning(UserWarning):
-    pass
-
-
-class QMap(afmformats.AFMQMap):
-    def __init__(self, path_or_group, meta_override=None, callback=None):
-        """Quantitative force spectroscopy map handling
-
-        Parameters
-        ----------
-        path_or_group: str or pathlib.Path or afmformats.afm_group.AFMGroup
-            The path to the data file or an instance of `AFMGroup`
-        meta_override: dict
-            Dictionary with metadata that is used when loading the data
-            in `path`.
-        callback: callable or None
-            A method that accepts a float between 0 and 1
-            to externally track the process of loading the data.
-        """
-        super(QMap, self).__init__(
-            path_or_group=path_or_group,
-            meta_override=meta_override,
-            callback=callback,
-            **get_load_data_modality_kwargs()
-        )
-
-    @staticmethod
-    @qmap_feature(name="fit: contact point",
-                  unit="nm",
-                  cache=False)
-    def feat_fit_contact_point(idnt):
-        """Contact point of the fit"""
-        if idnt.fit_properties.get("success", False):
-            # use cached contact point
-            params = idnt.fit_properties["params_fitted"]
-            value = params["contact_point"].value * 1e9
-        else:
-            msg = "The experimental data has not been fitted. Please call " \
-                  + "`idnt.fit_model` manually for {}!".format(idnt)
-            warnings.warn(msg, DataMissingWarning)
-            value = np.nan
-
-        return value
-
-    @staticmethod
-    @qmap_feature(name="fit: Young's modulus",
-                  unit="Pa",
-                  cache=False)
-    def feat_fit_youngs_modulus(idnt):
-        """Young's modulus"""
-        if idnt.fit_properties.get("success", False):
-            # use cached young's modulus
-            value = idnt.fit_properties["params_fitted"]["E"].value
-        else:
-            msg = "The experimental data has not been fitted. Please call " \
-                  + "`idnt.fit_model` manually for {}!".format(idnt)
-            warnings.warn(msg, DataMissingWarning)
-            value = np.nan
-
-        return value
-
-    @staticmethod
-    @qmap_feature(name="fit: rating",
-                  unit="",
-                  cache=False)
-    def feat_meta_rating(idnt):
-        """Rating"""
-        if idnt._rating is None:
-            msg = "The experimental data has not been rated. Please call " \
-                  + "`idnt.rate_quality` manually for {}!".format(idnt)
-            warnings.warn(msg, DataMissingWarning)
-            value = np.nan
-        else:
-            # use cached rating
-            value = idnt._rating[-1]
-        return value
+import warnings
+
+import afmformats
+from afmformats.afm_qmap import qmap_feature
+import numpy as np
+
+from .read import get_load_data_modality_kwargs
+
+
+class DataMissingWarning(UserWarning):
+    pass
+
+
+class QMap(afmformats.AFMQMap):
+    def __init__(self, path_or_group, meta_override=None, callback=None):
+        """Quantitative force spectroscopy map handling
+
+        Parameters
+        ----------
+        path_or_group: str or pathlib.Path or afmformats.afm_group.AFMGroup
+            The path to the data file or an instance of `AFMGroup`
+        meta_override: dict
+            Dictionary with metadata that is used when loading the data
+            in `path`.
+        callback: callable or None
+            A method that accepts a float between 0 and 1
+            to externally track the process of loading the data.
+        """
+        super(QMap, self).__init__(
+            path_or_group=path_or_group,
+            meta_override=meta_override,
+            callback=callback,
+            **get_load_data_modality_kwargs()
+        )
+
+    @staticmethod
+    @qmap_feature(name="fit: contact point",
+                  unit="nm",
+                  cache=False)
+    def feat_fit_contact_point(idnt):
+        """Contact point of the fit"""
+        if idnt.fit_properties.get("success", False):
+            # use cached contact point
+            params = idnt.fit_properties["params_fitted"]
+            value = params["contact_point"].value * 1e9
+        else:
+            msg = "The experimental data has not been fitted. Please call " \
+                  + "`idnt.fit_model` manually for {}!".format(idnt)
+            warnings.warn(msg, DataMissingWarning)
+            value = np.nan
+
+        return value
+
+    @staticmethod
+    @qmap_feature(name="fit: Young's modulus",
+                  unit="Pa",
+                  cache=False)
+    def feat_fit_youngs_modulus(idnt):
+        """Young's modulus"""
+        if idnt.fit_properties.get("success", False):
+            # use cached young's modulus
+            value = idnt.fit_properties["params_fitted"]["E"].value
+        else:
+            msg = "The experimental data has not been fitted. Please call " \
+                  + "`idnt.fit_model` manually for {}!".format(idnt)
+            warnings.warn(msg, DataMissingWarning)
+            value = np.nan
+
+        return value
+
+    @staticmethod
+    @qmap_feature(name="fit: rating",
+                  unit="",
+                  cache=False)
+    def feat_meta_rating(idnt):
+        """Rating"""
+        if idnt._rating is None:
+            msg = "The experimental data has not been rated. Please call " \
+                  + "`idnt.rate_quality` manually for {}!".format(idnt)
+            warnings.warn(msg, DataMissingWarning)
+            value = np.nan
+        else:
+            # use cached rating
+            value = idnt._rating[-1]
+        return value
```

### Comparing `nanite-3.5.4/nanite/rate/features.py` & `nanite-3.6.0/nanite/rate/features.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,571 +1,571 @@
-import inspect
-
-import numpy as np
-from scipy import ndimage
-
-#: Valid keyword arguments for feature types
-VALID_FEATURE_TYPES = ["all", "binary", "continuous"]
-
-
-class IndentationFeatures(object):
-    def __init__(self, dataset=None):
-        #: current dataset from which features are computed
-        self.dataset = dataset
-
-    @property
-    def is_fitted(self):
-        if self.is_valid:
-            return self.dataset.fit_properties["success"]
-        else:
-            return False
-
-    @property
-    def is_valid(self):
-        return bool(self.dataset.fit_properties)
-
-    @property
-    def has_contact_point(self):
-        if self.is_fitted:
-            pint = self.dataset.fit_properties["params_fitted"]
-            return "contact_point" in pint
-        else:
-            return False
-
-    @property
-    def contact_point(self):
-        if self.has_contact_point:
-            pint = self.dataset.fit_properties["params_fitted"]
-            return pint["contact_point"].value
-        else:
-            raise ValueError("No contact point in data!")
-
-    @property
-    def datafit_apr(self):
-        seg = self.dataset["segment"] == 0
-        f = self.dataset["fit"][seg].copy()
-        return f
-
-    @property
-    def datares_apr(self):
-        return self.datafit_apr - self.datay_apr
-
-    @property
-    def datax_apr(self):
-        xaxis = self.dataset.fit_properties["x_axis"]
-        seg = self.dataset["segment"] == 0
-        x = self.dataset[xaxis][seg].copy()
-        # Make sure everything is ok
-        assert x[0] > x[-1], "Approach from large distances towards lower"
-        return x
-
-    @property
-    def datay_apr(self):
-        yaxis = self.dataset.fit_properties["y_axis"]
-        seg = self.dataset["segment"] == 0
-        y = self.dataset[yaxis][seg].copy()
-        return y
-
-    @property
-    def meta(self):
-        return self.dataset.metadata
-
-    @staticmethod
-    def compute_features(idnt, which_type="all", names=None,
-                         ret_names=False):
-        """Compute the features for a data set
-
-        Parameters
-        ----------
-        idnt: nanite.Indentation
-            A dataset to rate
-        names: list of str
-            The names of the rating methods to use,
-            e.g. ["rate_apr_bumps", "rate_apr_mon_incr"].
-            If None (default), all available rating methods are
-            used.
-
-        Notes
-        -----
-        `names` may include features that are excluded by `which_type`.
-        E.g. if a "bool" feature is in `names` but `which_type` is
-        "float", then the "bool" feature will be silently ignored.
-        """
-        inst = IndentationFeatures(idnt)
-        # make sure to keep the order of `names`, i.e. only compute
-        # names if they are not given.
-        if names is None or which_type != "all":
-            names = IndentationFeatures.get_feature_names(
-                which_type=which_type, names=names)
-        samples = []
-        for nameii in names:
-            sii = float(getattr(inst, nameii)())
-            samples.append(sii)
-        samples = np.array(samples, dtype=float).flatten()
-        if ret_names:
-            return samples, names
-        else:
-            return samples
-
-    @classmethod
-    def get_feature_funcs(cls, which_type="all", names=None):
-        """Return functions that compute features from a dataset
-
-        Parameters
-        ----------
-        names: list of str
-            The names of the rating methods to use,
-            e.g. ["rate_apr_bumps", "rate_apr_mon_incr"].
-            If None (default), all available rating methods are
-            returned.
-        which_type: str
-            Which features to return: ["all", "bool", "float"].
-
-        Returns
-        -------
-        raters: list of tuples (name, callable)
-            Each item in the list consists contains the name
-            of the rating method and the corresponding rating
-            method.
-        """
-        fnames = cls.get_feature_names(which_type=which_type, names=names)
-        ffuncs = [(ff, getattr(cls, ff)) for ff in fnames]
-        return ffuncs
-
-    @classmethod
-    def get_feature_names(cls, which_type="all", names=None,
-                          ret_indices=False):
-        """Get features names
-
-        Parameters
-        ----------
-        which_type: str or list of str
-            Return only features that are of a certain type.
-            See `VALID_FEATURE_TYPES` for valid strings.
-        names: list of str
-            Return only features that are in this list.
-        ret_indices: bool
-            If True, also return the internal feature indices.
-
-        Returns
-        -------
-        name_list: list of str
-            List of feature names (callables of this class)
-        """
-        if isinstance(which_type, (list, tuple)):
-            # recurse
-            fnames = []
-            for wt in which_type:
-                fnames += cls.get_feature_names(which_type=wt)
-        else:
-            if which_type not in VALID_FEATURE_TYPES:
-                msg = "`which_type` must be one of {}, got '{}'".format(
-                    VALID_FEATURE_TYPES, which_type)
-                raise ValueError(msg)
-            if which_type == "all":
-                fstart = "feat_"
-            elif which_type == "binary":
-                fstart = "feat_bin_"
-            elif which_type == "continuous":
-                fstart = "feat_con_"
-            ffuncs = inspect.getmembers(cls, lambda a: (inspect.isroutine(a)))
-            fnames = [ff[0] for ff in ffuncs if ff[0].startswith(fstart)]
-        # keep only names requested by the user
-        if names:
-            # convenience: make sure the requested feature names all exists
-            refnames = cls.get_feature_names()
-            unknown = [nn for nn in names if nn not in refnames]
-            if unknown:
-                msg = "Unknown feature names: '{}'".format(",".join(unknown))
-                raise ValueError(msg)
-            # only use selected features
-            fnames = [ff for ff in fnames if ff in names]
-        fnames = sorted(fnames)
-        if ret_indices:
-            # return the internal index
-            allnames = cls.get_feature_names()
-            indices = []
-            for ii, aff in enumerate(allnames):
-                if aff in fnames:
-                    indices.append(ii)
-            return fnames, np.array(indices, dtype=int)
-        else:
-            return fnames
-
-    # for bool features, 1 means good and 0 means bad
-    def feat_bin_apr_spikes_count(self):
-        """spikes during IDT
-
-        Sudden spikes in indentation curve
-        """
-        if self.has_contact_point:
-            cp = self.contact_point
-            # indentation part
-            indidx = self.datax_apr < cp
-            diff = self.datares_apr[indidx]
-            diff = diff[~np.isnan(diff)]
-            if len(diff) > 50:
-                # find regions with peaks
-                diff_smooth = ndimage.gaussian_filter1d(diff, sigma=11)
-                delta1 = diff - diff_smooth
-                diff_smooth2 = ndimage.gaussian_filter1d(diff, sigma=1)
-                delta2 = diff_smooth2 - diff_smooth
-                std = np.std(delta1)
-                peakarray = np.diff(np.abs(delta2) > 3*std)
-                npeaks = np.sum(peakarray)
-                value = npeaks <= 5
-            else:
-                value = np.nan
-        else:
-            value = np.nan
-        return value
-
-    def feat_bin_cp_position(self):
-        """CP outside of data range
-
-        Contact point position outside of range
-        """
-        if self.has_contact_point:
-            cp = self.contact_point
-            x = self.datax_apr
-            if cp < np.min(x) or cp > np.max(x):
-                value = False
-            else:
-                value = True
-            return value
-        else:
-            return np.nan
-
-    def feat_bin_size(self):
-        """dataset too small
-
-        Number of points in indentation curve
-        """
-        if self.is_valid:
-            a_ind = self.datay_apr
-            num = a_ind.shape[0]
-            if num < 600:
-                value = False
-            else:
-                value = True
-        else:
-            value = np.nan
-        return value
-
-    def feat_con_apr_flatness(self):
-        """flatness of APR residuals
-
-        fraction of the positive-gradient residuals in the approach part
-        """
-        if self.has_contact_point:
-            cp = self.contact_point
-            # baseline indices of approach curve
-            # (approaches from pos values)
-            blidx = self.datax_apr > cp
-            # get residuals of approach curve
-            r_bl = self.datares_apr[blidx]
-            r_bl = r_bl[~np.isnan(r_bl)]
-            # perform gaussian blur
-            sigma = max(5, (int(r_bl.shape[0]/120)//2)*2+1)
-            y = ndimage.gaussian_filter1d(r_bl, sigma=sigma)
-            if len(y) > 2:
-                grad = np.gradient(y)
-                pos = np.sum(grad > 0)
-                neg = np.sum(grad < 0)
-                value = pos/(pos + neg)
-            else:
-                value = np.nan
-        else:
-            value = np.nan
-        return value
-
-    def feat_con_apr_sum(self):
-        """residuals of APR
-
-        absolute sum of the residuals in the approach part
-        """
-        if self.has_contact_point:
-            cp = self.contact_point
-            # indentation part
-            indidx = self.datax_apr > cp
-            diff = self.datares_apr[indidx]
-            diff = diff[~np.isnan(diff)]
-            xin = self.datax_apr
-            yin = self.datay_apr
-
-            norm = xin.size * np.max(yin)
-            value = np.sum(np.abs(diff)) / norm * 100
-            value = np.log(1+value)
-        else:
-            value = np.nan
-        return value
-
-    def feat_con_apr_size(self):
-        """relative APR size
-
-        length of the approach part relative to the indentation part
-        """
-        if self.has_contact_point:
-            cp = self.contact_point
-            # baseline indices of approach curve
-            # (approaches from pos values)
-            x = self.datax_apr
-            aprsize = np.sum(x > cp)
-            tolsize = x.shape[0]
-            value = 1 - aprsize/tolsize
-            return value
-        else:
-            return np.nan
-
-    def feat_con_bln_slope(self):
-        """slope of BLN
-
-        slope obtained from a linear least-squares fit to the baseline
-        """
-        if self.has_contact_point:
-            cp = self.contact_point
-            x = self.datax_apr
-            y = self.datares_apr
-            # break point is between xmax and cp
-            breakp = (np.max(x) + cp) / 2
-            # left of break point and no nans
-            valid = (x > breakp) * (~np.isnan(x))
-
-            # slope range
-            x_sl = x[valid]
-            y_sl = y[valid]
-
-            if x_sl.size > 20:
-                # fit a line to the data
-                A = np.vstack([x_sl, np.ones(len(x_sl))]).T
-                m, _c = np.linalg.lstsq(A, y_sl, rcond=None)[0]
-                # normalize with maximum force
-                value = m / np.max(self.datay_apr)
-                value = np.log(1 + np.abs(value)) / 10
-            else:
-                value = np.nan
-        else:
-            value = np.nan
-        return value
-
-    def feat_con_bln_variation(self):
-        """variation in BLN
-
-        comparison of the forces at the beginning and at the end
-        of the baseline
-        """
-        if self.has_contact_point:
-            cp = self.contact_point
-            r_bl = self.datares_apr[self.datax_apr > cp]
-            r_bl = r_bl[~np.isnan(r_bl)]
-            # skip 10%
-            offset = int(r_bl.shape[0]*.1)
-            if offset:
-                r_bl = r_bl[:-offset]
-            if r_bl.shape[0] > 20:
-                avg1 = np.average(r_bl[:10])
-                avg2 = np.average(r_bl[-10:])
-                # normalize with maximum force and multiply by 1000
-                maxforce = np.max(self.datay_apr)
-                value = np.abs(avg1-avg2)/maxforce * 1e3
-                value = np.log(1 + value) / 5
-            else:
-                value = np.nan
-            return value
-        else:
-            return np.nan
-
-    def feat_con_cp_curvature(self):
-        """curvature at CP
-
-        curvature of the force-distance data at the contact point
-        """
-        if self.has_contact_point:
-            cp = self.contact_point
-            x = self.datax_apr
-            y = self.datay_apr
-            # 10 % of indentation is range
-            cpid = np.argmin(np.abs(x - cp))
-            maxid = np.argmax(y)
-            incl = np.abs(maxid - cpid) // 10
-            if incl > 5:
-                reg = y[cpid - incl:cpid + incl]
-                if len(reg):
-                    lin = np.linspace(reg.min(), reg.max(), reg.size)
-                    diff = np.sum(reg-lin)
-                    value = diff / y.max() * 10
-                    value = np.log(1 + np.abs(value)) * np.sign(value) / 4
-                else:
-                    value = np.nan
-            else:
-                value = np.nan
-        else:
-            value = np.nan
-        return value
-
-    def feat_con_cp_magnitude(self):
-        """residuals at CP
-
-        mean value of the residuals around the contact point
-        """
-        if self.has_contact_point:
-            cp = self.contact_point
-            # use 10% of the indentation part as size
-            r_range = int(np.sum(self.datax_apr < cp) * .1)
-            cpidx = np.nanargmin(np.abs(self.datax_apr-cp))
-            rat_range = np.abs(
-                self.datares_apr[cpidx - r_range:cpidx + r_range])
-            # normalization with setpoint of curve gives us a number
-            if len(rat_range):
-                value = np.nansum(rat_range) / np.max(self.datay_apr) / 100
-            else:
-                value = np.nan
-            return value
-        else:
-            return np.nan
-
-    def feat_con_idt_maxima_75perc(self):
-        """maxima in IDT residuals
-
-        sum of the indentation residuals' maxima in three intervals
-        in-between 25% and 100% relative to the maximum indentation
-        """
-        if self.has_contact_point:
-            yin = self.datay_apr
-            fit = self.datafit_apr
-            xin = self.datax_apr
-            cp = self.contact_point
-            id100 = np.argmin(xin)
-            id000 = np.argmin(np.abs(xin - cp))
-            id025 = int(id000 + .25 * (id100 - id000))
-            idmin, idmax = min(id025, id100), max(id025, id100)
-            if idmin != idmax:
-                # find zeros
-                idcen = idmin + (idmax - idmin) // 2
-                smooth = ndimage.gaussian_filter1d(yin - fit, sigma=11)
-                idzero1 = idmin + np.argmin(np.abs(smooth[idmin:idcen]))
-                idzero2 = idcen + np.argmin(np.abs(smooth[idcen:idmax]))
-                # change of sign in 1st, 2nd, and 3rd part of indentation
-                ydiffs = []
-                if idmin != idzero1:
-                    y1 = np.max(np.abs((yin - fit)[idmin:idzero1]))
-                    ydiffs.append(y1)
-                if idzero1 != idzero2:
-                    y2 = np.max(np.abs((yin - fit)[idzero1:idzero2]))
-                    ydiffs.append(y2)
-                if idzero2 != idmax:
-                    y3 = np.max(np.abs((yin - fit)[idzero2:idmax]))
-                    ydiffs.append(y3)
-                if ydiffs:
-                    # combine the changes (ydiff2 has different sign)
-                    ydiff = np.sum(ydiffs)
-                    ydiff /= yin.max()
-                    value = np.log(1 + ydiff) * 2
-                else:
-                    value = np.nan
-            else:
-                value = np.nan
-        else:
-            value = np.nan
-        return value
-
-    def feat_con_idt_monotony(self):
-        """monotony of IDT
-
-        change of the gradient in the indentation part
-        """
-        if self.has_contact_point:
-            cp = self.contact_point
-            # indentation part
-            indidx = self.datax_apr < cp
-            # get approach curve
-            a_ind = self.datay_apr[indidx]
-            # perform gaussian blur
-            y = ndimage.gaussian_filter1d(a_ind, sigma=2)
-            if len(y) > 2:
-                grad = np.gradient(y)
-                gz = np.abs(np.sum(grad[grad > 0]))
-                lz = np.abs(np.sum(grad[grad < 0]))
-                value = np.sum(indidx) * lz / gz
-                value = np.log(1 + value) / 10
-            else:
-                value = np.nan
-        else:
-            value = np.nan
-        return value
-
-    def feat_con_idt_sum(self):
-        """overall IDT residuals
-
-        sum of the residuals in the indentation part
-        """
-        if self.has_contact_point:
-            cp = self.contact_point
-            x = self.datax_apr
-            y = self.datay_apr
-            f = self.datafit_apr
-            idind = x < cp
-            diff = (y - f)[idind]
-            if diff.size:
-                area = np.nansum(np.abs(diff))/diff.size
-                norm = np.abs(y.max() - y.min())/2
-                value = area/norm
-                value = np.log(1 + value) * 5
-            else:
-                value = np.nan
-        else:
-            value = np.nan
-        return value
-
-    def feat_con_idt_sum_75perc(self):
-        """residuals in 75% IDT
-
-        sum of the residuals in the indentation part in-between
-        25% and 100% relative to the maximum indentation
-        """
-        if self.has_contact_point:
-            yin = self.datay_apr
-            fit = self.datafit_apr
-            xin = self.datax_apr
-            cp = self.contact_point
-            id100 = np.argmin(xin)
-            id000 = np.argmin(np.abs(xin - cp))
-            id025 = int(id000 + .25 * (id100 - id000))
-            idmin, idmax = min(id025, id100), max(id025, id100)
-            ydiff = np.sum(np.abs(yin - fit)[idmin:idmax])
-            xnorm = np.abs(xin[idmin] - xin[idmax])
-            # area under the curve (normalization with absolute x interval)
-            area = ydiff * xnorm
-            # normalize by max force and multiply by 1e6 to get values around 1
-            value = area / np.max(yin) * 1e6
-            value = np.log(1+value) / 8
-        else:
-            value = np.nan
-        return value
-
-    def feat_con_idt_spike_area(self):
-        """area of IDT spikes
-
-        area of spikes appearing in the indentation part
-        """
-        if self.has_contact_point:
-            cp = self.contact_point
-            # indentation part
-            indidx = self.datax_apr < cp
-            diff = self.datares_apr[indidx]
-            diff = diff[~np.isnan(diff)]
-            if len(diff) > 20:
-                # find regions with peaks
-                diff_smooth = ndimage.gaussian_filter1d(diff, sigma=11)
-                delta1 = diff - diff_smooth
-                diff_smooth2 = ndimage.gaussian_filter1d(diff, sigma=1)
-                delta2 = np.abs(diff_smooth2 - diff_smooth)
-                std = np.std(delta1)
-                peaks = np.sum(delta2[delta1 > 3*std])
-                # add SD to avoid too many zero-valued samples
-                value = (std + peaks) / np.max(self.datay_apr)
-                value = np.log(1 + value) * 20
-            else:
-                value = np.nan
-        else:
-            value = np.nan
-        return value
+import inspect
+
+import numpy as np
+from scipy import ndimage
+
+#: Valid keyword arguments for feature types
+VALID_FEATURE_TYPES = ["all", "binary", "continuous"]
+
+
+class IndentationFeatures(object):
+    def __init__(self, dataset=None):
+        #: current dataset from which features are computed
+        self.dataset = dataset
+
+    @property
+    def is_fitted(self):
+        if self.is_valid:
+            return self.dataset.fit_properties["success"]
+        else:
+            return False
+
+    @property
+    def is_valid(self):
+        return bool(self.dataset.fit_properties)
+
+    @property
+    def has_contact_point(self):
+        if self.is_fitted:
+            pint = self.dataset.fit_properties["params_fitted"]
+            return "contact_point" in pint
+        else:
+            return False
+
+    @property
+    def contact_point(self):
+        if self.has_contact_point:
+            pint = self.dataset.fit_properties["params_fitted"]
+            return pint["contact_point"].value
+        else:
+            raise ValueError("No contact point in data!")
+
+    @property
+    def datafit_apr(self):
+        seg = self.dataset["segment"] == 0
+        f = self.dataset["fit"][seg].copy()
+        return f
+
+    @property
+    def datares_apr(self):
+        return self.datafit_apr - self.datay_apr
+
+    @property
+    def datax_apr(self):
+        xaxis = self.dataset.fit_properties["x_axis"]
+        seg = self.dataset["segment"] == 0
+        x = self.dataset[xaxis][seg].copy()
+        # Make sure everything is ok
+        assert x[0] > x[-1], "Approach from large distances towards lower"
+        return x
+
+    @property
+    def datay_apr(self):
+        yaxis = self.dataset.fit_properties["y_axis"]
+        seg = self.dataset["segment"] == 0
+        y = self.dataset[yaxis][seg].copy()
+        return y
+
+    @property
+    def meta(self):
+        return self.dataset.metadata
+
+    @staticmethod
+    def compute_features(idnt, which_type="all", names=None,
+                         ret_names=False):
+        """Compute the features for a data set
+
+        Parameters
+        ----------
+        idnt: nanite.Indentation
+            A dataset to rate
+        names: list of str
+            The names of the rating methods to use,
+            e.g. ["rate_apr_bumps", "rate_apr_mon_incr"].
+            If None (default), all available rating methods are
+            used.
+
+        Notes
+        -----
+        `names` may include features that are excluded by `which_type`.
+        E.g. if a "bool" feature is in `names` but `which_type` is
+        "float", then the "bool" feature will be silently ignored.
+        """
+        inst = IndentationFeatures(idnt)
+        # make sure to keep the order of `names`, i.e. only compute
+        # names if they are not given.
+        if names is None or which_type != "all":
+            names = IndentationFeatures.get_feature_names(
+                which_type=which_type, names=names)
+        samples = []
+        for nameii in names:
+            sii = float(getattr(inst, nameii)())
+            samples.append(sii)
+        samples = np.array(samples, dtype=float).flatten()
+        if ret_names:
+            return samples, names
+        else:
+            return samples
+
+    @classmethod
+    def get_feature_funcs(cls, which_type="all", names=None):
+        """Return functions that compute features from a dataset
+
+        Parameters
+        ----------
+        names: list of str
+            The names of the rating methods to use,
+            e.g. ["rate_apr_bumps", "rate_apr_mon_incr"].
+            If None (default), all available rating methods are
+            returned.
+        which_type: str
+            Which features to return: ["all", "bool", "float"].
+
+        Returns
+        -------
+        raters: list of tuples (name, callable)
+            Each item in the list consists contains the name
+            of the rating method and the corresponding rating
+            method.
+        """
+        fnames = cls.get_feature_names(which_type=which_type, names=names)
+        ffuncs = [(ff, getattr(cls, ff)) for ff in fnames]
+        return ffuncs
+
+    @classmethod
+    def get_feature_names(cls, which_type="all", names=None,
+                          ret_indices=False):
+        """Get features names
+
+        Parameters
+        ----------
+        which_type: str or list of str
+            Return only features that are of a certain type.
+            See `VALID_FEATURE_TYPES` for valid strings.
+        names: list of str
+            Return only features that are in this list.
+        ret_indices: bool
+            If True, also return the internal feature indices.
+
+        Returns
+        -------
+        name_list: list of str
+            List of feature names (callables of this class)
+        """
+        if isinstance(which_type, (list, tuple)):
+            # recurse
+            fnames = []
+            for wt in which_type:
+                fnames += cls.get_feature_names(which_type=wt)
+        else:
+            if which_type not in VALID_FEATURE_TYPES:
+                msg = "`which_type` must be one of {}, got '{}'".format(
+                    VALID_FEATURE_TYPES, which_type)
+                raise ValueError(msg)
+            if which_type == "all":
+                fstart = "feat_"
+            elif which_type == "binary":
+                fstart = "feat_bin_"
+            elif which_type == "continuous":
+                fstart = "feat_con_"
+            ffuncs = inspect.getmembers(cls, lambda a: (inspect.isroutine(a)))
+            fnames = [ff[0] for ff in ffuncs if ff[0].startswith(fstart)]
+        # keep only names requested by the user
+        if names:
+            # convenience: make sure the requested feature names all exists
+            refnames = cls.get_feature_names()
+            unknown = [nn for nn in names if nn not in refnames]
+            if unknown:
+                msg = "Unknown feature names: '{}'".format(",".join(unknown))
+                raise ValueError(msg)
+            # only use selected features
+            fnames = [ff for ff in fnames if ff in names]
+        fnames = sorted(fnames)
+        if ret_indices:
+            # return the internal index
+            allnames = cls.get_feature_names()
+            indices = []
+            for ii, aff in enumerate(allnames):
+                if aff in fnames:
+                    indices.append(ii)
+            return fnames, np.array(indices, dtype=int)
+        else:
+            return fnames
+
+    # for bool features, 1 means good and 0 means bad
+    def feat_bin_apr_spikes_count(self):
+        """spikes during IDT
+
+        Sudden spikes in indentation curve
+        """
+        if self.has_contact_point:
+            cp = self.contact_point
+            # indentation part
+            indidx = self.datax_apr < cp
+            diff = self.datares_apr[indidx]
+            diff = diff[~np.isnan(diff)]
+            if len(diff) > 50:
+                # find regions with peaks
+                diff_smooth = ndimage.gaussian_filter1d(diff, sigma=11)
+                delta1 = diff - diff_smooth
+                diff_smooth2 = ndimage.gaussian_filter1d(diff, sigma=1)
+                delta2 = diff_smooth2 - diff_smooth
+                std = np.std(delta1)
+                peakarray = np.diff(np.abs(delta2) > 3*std)
+                npeaks = np.sum(peakarray)
+                value = npeaks <= 5
+            else:
+                value = np.nan
+        else:
+            value = np.nan
+        return value
+
+    def feat_bin_cp_position(self):
+        """CP outside of data range
+
+        Contact point position outside of range
+        """
+        if self.has_contact_point:
+            cp = self.contact_point
+            x = self.datax_apr
+            if cp < np.min(x) or cp > np.max(x):
+                value = False
+            else:
+                value = True
+            return value
+        else:
+            return np.nan
+
+    def feat_bin_size(self):
+        """dataset too small
+
+        Number of points in indentation curve
+        """
+        if self.is_valid:
+            a_ind = self.datay_apr
+            num = a_ind.shape[0]
+            if num < 600:
+                value = False
+            else:
+                value = True
+        else:
+            value = np.nan
+        return value
+
+    def feat_con_apr_flatness(self):
+        """flatness of APR residuals
+
+        fraction of the positive-gradient residuals in the approach part
+        """
+        if self.has_contact_point:
+            cp = self.contact_point
+            # baseline indices of approach curve
+            # (approaches from pos values)
+            blidx = self.datax_apr > cp
+            # get residuals of approach curve
+            r_bl = self.datares_apr[blidx]
+            r_bl = r_bl[~np.isnan(r_bl)]
+            # perform gaussian blur
+            sigma = max(5, (int(r_bl.shape[0]/120)//2)*2+1)
+            y = ndimage.gaussian_filter1d(r_bl, sigma=sigma)
+            if len(y) > 2:
+                grad = np.gradient(y)
+                pos = np.sum(grad > 0)
+                neg = np.sum(grad < 0)
+                value = pos/(pos + neg)
+            else:
+                value = np.nan
+        else:
+            value = np.nan
+        return value
+
+    def feat_con_apr_sum(self):
+        """residuals of APR
+
+        absolute sum of the residuals in the approach part
+        """
+        if self.has_contact_point:
+            cp = self.contact_point
+            # indentation part
+            indidx = self.datax_apr > cp
+            diff = self.datares_apr[indidx]
+            diff = diff[~np.isnan(diff)]
+            xin = self.datax_apr
+            yin = self.datay_apr
+
+            norm = xin.size * np.max(yin)
+            value = np.sum(np.abs(diff)) / norm * 100
+            value = np.log(1+value)
+        else:
+            value = np.nan
+        return value
+
+    def feat_con_apr_size(self):
+        """relative APR size
+
+        length of the approach part relative to the indentation part
+        """
+        if self.has_contact_point:
+            cp = self.contact_point
+            # baseline indices of approach curve
+            # (approaches from pos values)
+            x = self.datax_apr
+            aprsize = np.sum(x > cp)
+            tolsize = x.shape[0]
+            value = 1 - aprsize/tolsize
+            return value
+        else:
+            return np.nan
+
+    def feat_con_bln_slope(self):
+        """slope of BLN
+
+        slope obtained from a linear least-squares fit to the baseline
+        """
+        if self.has_contact_point:
+            cp = self.contact_point
+            x = self.datax_apr
+            y = self.datares_apr
+            # break point is between xmax and cp
+            breakp = (np.max(x) + cp) / 2
+            # left of break point and no nans
+            valid = (x > breakp) * (~np.isnan(x))
+
+            # slope range
+            x_sl = x[valid]
+            y_sl = y[valid]
+
+            if x_sl.size > 20:
+                # fit a line to the data
+                A = np.vstack([x_sl, np.ones(len(x_sl))]).T
+                m, _c = np.linalg.lstsq(A, y_sl, rcond=None)[0]
+                # normalize with maximum force
+                value = m / np.max(self.datay_apr)
+                value = np.log(1 + np.abs(value)) / 10
+            else:
+                value = np.nan
+        else:
+            value = np.nan
+        return value
+
+    def feat_con_bln_variation(self):
+        """variation in BLN
+
+        comparison of the forces at the beginning and at the end
+        of the baseline
+        """
+        if self.has_contact_point:
+            cp = self.contact_point
+            r_bl = self.datares_apr[self.datax_apr > cp]
+            r_bl = r_bl[~np.isnan(r_bl)]
+            # skip 10%
+            offset = int(r_bl.shape[0]*.1)
+            if offset:
+                r_bl = r_bl[:-offset]
+            if r_bl.shape[0] > 20:
+                avg1 = np.average(r_bl[:10])
+                avg2 = np.average(r_bl[-10:])
+                # normalize with maximum force and multiply by 1000
+                maxforce = np.max(self.datay_apr)
+                value = np.abs(avg1-avg2)/maxforce * 1e3
+                value = np.log(1 + value) / 5
+            else:
+                value = np.nan
+            return value
+        else:
+            return np.nan
+
+    def feat_con_cp_curvature(self):
+        """curvature at CP
+
+        curvature of the force-distance data at the contact point
+        """
+        if self.has_contact_point:
+            cp = self.contact_point
+            x = self.datax_apr
+            y = self.datay_apr
+            # 10 % of indentation is range
+            cpid = np.argmin(np.abs(x - cp))
+            maxid = np.argmax(y)
+            incl = np.abs(maxid - cpid) // 10
+            if incl > 5:
+                reg = y[cpid - incl:cpid + incl]
+                if len(reg):
+                    lin = np.linspace(reg.min(), reg.max(), reg.size)
+                    diff = np.sum(reg-lin)
+                    value = diff / y.max() * 10
+                    value = np.log(1 + np.abs(value)) * np.sign(value) / 4
+                else:
+                    value = np.nan
+            else:
+                value = np.nan
+        else:
+            value = np.nan
+        return value
+
+    def feat_con_cp_magnitude(self):
+        """residuals at CP
+
+        mean value of the residuals around the contact point
+        """
+        if self.has_contact_point:
+            cp = self.contact_point
+            # use 10% of the indentation part as size
+            r_range = int(np.sum(self.datax_apr < cp) * .1)
+            cpidx = np.nanargmin(np.abs(self.datax_apr-cp))
+            rat_range = np.abs(
+                self.datares_apr[cpidx - r_range:cpidx + r_range])
+            # normalization with setpoint of curve gives us a number
+            if len(rat_range):
+                value = np.nansum(rat_range) / np.max(self.datay_apr) / 100
+            else:
+                value = np.nan
+            return value
+        else:
+            return np.nan
+
+    def feat_con_idt_maxima_75perc(self):
+        """maxima in IDT residuals
+
+        sum of the indentation residuals' maxima in three intervals
+        in-between 25% and 100% relative to the maximum indentation
+        """
+        if self.has_contact_point:
+            yin = self.datay_apr
+            fit = self.datafit_apr
+            xin = self.datax_apr
+            cp = self.contact_point
+            id100 = np.argmin(xin)
+            id000 = np.argmin(np.abs(xin - cp))
+            id025 = int(id000 + .25 * (id100 - id000))
+            idmin, idmax = min(id025, id100), max(id025, id100)
+            if idmin != idmax:
+                # find zeros
+                idcen = idmin + (idmax - idmin) // 2
+                smooth = ndimage.gaussian_filter1d(yin - fit, sigma=11)
+                idzero1 = idmin + np.argmin(np.abs(smooth[idmin:idcen]))
+                idzero2 = idcen + np.argmin(np.abs(smooth[idcen:idmax]))
+                # change of sign in 1st, 2nd, and 3rd part of indentation
+                ydiffs = []
+                if idmin != idzero1:
+                    y1 = np.max(np.abs((yin - fit)[idmin:idzero1]))
+                    ydiffs.append(y1)
+                if idzero1 != idzero2:
+                    y2 = np.max(np.abs((yin - fit)[idzero1:idzero2]))
+                    ydiffs.append(y2)
+                if idzero2 != idmax:
+                    y3 = np.max(np.abs((yin - fit)[idzero2:idmax]))
+                    ydiffs.append(y3)
+                if ydiffs:
+                    # combine the changes (ydiff2 has different sign)
+                    ydiff = np.sum(ydiffs)
+                    ydiff /= yin.max()
+                    value = np.log(1 + ydiff) * 2
+                else:
+                    value = np.nan
+            else:
+                value = np.nan
+        else:
+            value = np.nan
+        return value
+
+    def feat_con_idt_monotony(self):
+        """monotony of IDT
+
+        change of the gradient in the indentation part
+        """
+        if self.has_contact_point:
+            cp = self.contact_point
+            # indentation part
+            indidx = self.datax_apr < cp
+            # get approach curve
+            a_ind = self.datay_apr[indidx]
+            # perform gaussian blur
+            y = ndimage.gaussian_filter1d(a_ind, sigma=2)
+            if len(y) > 2:
+                grad = np.gradient(y)
+                gz = np.abs(np.sum(grad[grad > 0]))
+                lz = np.abs(np.sum(grad[grad < 0]))
+                value = np.sum(indidx) * lz / gz
+                value = np.log(1 + value) / 10
+            else:
+                value = np.nan
+        else:
+            value = np.nan
+        return value
+
+    def feat_con_idt_sum(self):
+        """overall IDT residuals
+
+        sum of the residuals in the indentation part
+        """
+        if self.has_contact_point:
+            cp = self.contact_point
+            x = self.datax_apr
+            y = self.datay_apr
+            f = self.datafit_apr
+            idind = x < cp
+            diff = (y - f)[idind]
+            if diff.size:
+                area = np.nansum(np.abs(diff))/diff.size
+                norm = np.abs(y.max() - y.min())/2
+                value = area/norm
+                value = np.log(1 + value) * 5
+            else:
+                value = np.nan
+        else:
+            value = np.nan
+        return value
+
+    def feat_con_idt_sum_75perc(self):
+        """residuals in 75% IDT
+
+        sum of the residuals in the indentation part in-between
+        25% and 100% relative to the maximum indentation
+        """
+        if self.has_contact_point:
+            yin = self.datay_apr
+            fit = self.datafit_apr
+            xin = self.datax_apr
+            cp = self.contact_point
+            id100 = np.argmin(xin)
+            id000 = np.argmin(np.abs(xin - cp))
+            id025 = int(id000 + .25 * (id100 - id000))
+            idmin, idmax = min(id025, id100), max(id025, id100)
+            ydiff = np.sum(np.abs(yin - fit)[idmin:idmax])
+            xnorm = np.abs(xin[idmin] - xin[idmax])
+            # area under the curve (normalization with absolute x interval)
+            area = ydiff * xnorm
+            # normalize by max force and multiply by 1e6 to get values around 1
+            value = area / np.max(yin) * 1e6
+            value = np.log(1+value) / 8
+        else:
+            value = np.nan
+        return value
+
+    def feat_con_idt_spike_area(self):
+        """area of IDT spikes
+
+        area of spikes appearing in the indentation part
+        """
+        if self.has_contact_point:
+            cp = self.contact_point
+            # indentation part
+            indidx = self.datax_apr < cp
+            diff = self.datares_apr[indidx]
+            diff = diff[~np.isnan(diff)]
+            if len(diff) > 20:
+                # find regions with peaks
+                diff_smooth = ndimage.gaussian_filter1d(diff, sigma=11)
+                delta1 = diff - diff_smooth
+                diff_smooth2 = ndimage.gaussian_filter1d(diff, sigma=1)
+                delta2 = np.abs(diff_smooth2 - diff_smooth)
+                std = np.std(delta1)
+                peaks = np.sum(delta2[delta1 > 3*std])
+                # add SD to avoid too many zero-valued samples
+                value = (std + peaks) / np.max(self.datay_apr)
+                value = np.log(1 + value) * 20
+            else:
+                value = np.nan
+        else:
+            value = np.nan
+        return value
```

### Comparing `nanite-3.5.4/nanite/rate/io.py` & `nanite-3.6.0/nanite/rate/io.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,390 +1,390 @@
-"""Save and load user-rated datasets"""
-from functools import lru_cache
-import hashlib
-import json
-import pathlib
-import shutil
-import tempfile
-import time
-
-import h5py
-import lmfit
-import numpy as np
-from sklearn import model_selection
-
-from .._version import version as nanite_version
-from ..group import IndentationGroup
-from . import rater
-
-
-class RateManager:
-    def __init__(self, path, verbose=0):
-        """Manage user-defined rates"""
-        #: Path to the manual ratings (directory or .h5 file)
-        self.path = pathlib.Path(path)
-        #: verbosity level
-        self.verbose = verbose
-        self._ratings = None
-
-    @staticmethod
-    def _get_samples(path, verbose=0):
-        rm = RateManager(path, verbose=verbose)
-        samples = []
-        idr = rater.IndentationRater
-        for ds in rm.datasets:
-            assert "success" in ds.fit_properties
-            features = idr.compute_features(ds)
-            samples.append(features)
-        return np.array(samples, dtype=float)
-
-    @property
-    def datasets(self):
-        return [r["data_set"] for r in self.ratings]
-
-    @property
-    def ratings(self):
-        if self._ratings is None:
-            self._ratings = load(self.path, verbose=self.verbose)
-        return self._ratings
-
-    @property
-    def samples(self):
-        """The individual sample ratings computed by afmlib"""
-        return RateManager._get_samples(self.path, verbose=self.verbose)
-
-    def export_training_set(self, path):
-        path = pathlib.Path(path)
-        path.mkdir(parents=True, exist_ok=True)
-        raters = rater.IndentationRater.get_feature_funcs()
-        samples = self.samples
-        for ii, rti in enumerate(raters):
-            rpath = path / "train_{}.txt".format(rti[0])
-            np.savetxt(rpath, samples[:, ii].flatten(), fmt="%.2e")
-        user = self.get_rates(which="user")
-        upath = str(path / "train_response.txt")
-        np.savetxt(upath, user.flatten(), fmt="%.2e")
-
-    def get_cross_validation_score(self, regressor, training_set=None,
-                                   n_splits=20, random_state=42):
-        """Regressor cross-validation scoring
-
-        Cross-validation is used to identify regressors that
-        over-fit the train set by splitting the train set into
-        multiple learn/test sets and quantifying the regressor
-        performance for each split.
-
-        Parameters
-        ----------
-        regressor: str or RegressorMixin
-            If a string, must be in `reg_names`.
-        training_set: X, y
-            If given, do not use self.samples
-
-        Notes
-        -----
-        A :class:`skimage.model_selection.KFold` cross validator is used
-        in combination with the mean squared error score.
-
-        Cross-validation score is computed from samples that are filtered
-        with the binary features and only from samples that do not contain
-        any nan values.
-        """
-        ir = rater.get_rater(regressor)
-
-        if training_set:
-            X, y = training_set
-        else:
-            # remove binary features and nans otherwise cross-validation
-            # will not work
-            X, y = self.get_training_set(prefilter_binary=True,
-                                         remove_nans=True)
-
-        # The score is maximized, therefore it is "neg_"
-        scoring = 'neg_mean_squared_error'
-        loo = model_selection.KFold(n_splits=n_splits, shuffle=True,
-                                    random_state=random_state)
-        scores = model_selection.cross_val_score(ir.pipeline, X, y,
-                                                 scoring=scoring, cv=loo)
-        return -scores
-
-    def get_rates(self, which="user", training_set="zef18"):
-        """
-        which: str
-            Which rating to return: "user" or a regressor name
-        """
-        if which == "user":
-            rtngs = np.array([ri["rating"]
-                              for ri in load(self.path, meta_only=True)])
-        else:
-            rt = rater.get_rater(regressor=which, training_set=training_set)
-            rtngs = rt.rate(self.samples)
-        return rtngs
-
-    def get_training_set(self, which_type="all", prefilter_binary=False,
-                         remove_nans=False, transform=False):
-        """Return (X, y) training set"""
-        X = self.samples
-        y = self.get_rates(which="user")
-
-        if prefilter_binary:
-            # remove samples with `False` in a binary feature
-            ir = rater.IndentationRater(regressor=None)
-            bnames, bind = ir.get_feature_names(which_type="binary",
-                                                ret_indices=True)
-            if bnames:
-                X_bool = X[:, bind]
-
-                X_f = []
-                y_f = []
-                for ii in range(len(y)):
-                    if ir._pre_rate(X_bool[ii]):
-                        X_f.append(X[ii])
-                        y_f.append(y[ii])
-                X, y = np.array(X_f), np.array(y_f)
-
-        # must come after prefilter_binary
-        if which_type != "all":
-            _unames, indices = rater.IndentationRater.get_feature_names(
-                which_type=which_type,
-                ret_indices=True)
-            # remove unwanted features
-            if X.size:
-                X = X[:, list(indices)]
-
-        if remove_nans:
-            X_n = []
-            y_n = []
-            for ii in range(len(y)):
-                if not np.sum(np.isnan(X[ii])):
-                    X_n.append(X[ii])
-                    y_n.append(y[ii])
-            X, y = np.array(X_n), np.array(y_n)
-
-        if transform:
-            # Transform data
-            ir = rater.IndentationRater(regressor=None,
-                                        training_set=(X, y)
-                                        )
-            X = ir.pipeline.transform(X)
-        return X, y
-
-
-@lru_cache(maxsize=100)
-def hash_file(path, blocksize=65536):
-    """Compute sha256 hex-hash of a file
-
-    Parameters
-    ----------
-    path: str or pathlib.Path
-        path to the file
-    blocksize: int
-        block size read from the file
-
-    Returns
-    -------
-    hex: str
-        The first six characters of the hash
-    """
-    fname = pathlib.Path(path)
-    hasher = hashlib.sha256()
-    with fname.open('rb') as fd:
-        buf = fd.read(blocksize)
-        while len(buf) > 0:
-            hasher.update(buf)
-            buf = fd.read(blocksize)
-    return hasher.hexdigest()[:6]
-
-
-def load(path, meta_only=False, verbose=0):
-    """
-
-    Notes
-    -----
-    The .fit_properties attribute of each Indentation instance
-    is overridden by a simple dictionary,
-    so its functionalities are not available anymore.
-    """
-    path = pathlib.Path(path)
-    ratings = []
-    if path.is_dir():
-        if verbose:
-            print("Performing iterative folder search.")
-        for fpath in sorted(path.rglob("*.h5")):
-            ratings += load(fpath, meta_only=meta_only)
-    elif path.suffix == ".h5":
-        if verbose:
-            print("Loading file '{}'... ".format(path), end="", flush=True)
-        ratings += load_hdf5(path, meta_only=meta_only)
-        if verbose:
-            print("Done.")
-    return ratings
-
-
-def load_hdf5(path, meta_only=False):
-    ratings = []
-    path = pathlib.Path(path)
-    # temporary directory for original data
-    tdir = tempfile.mkdtemp(prefix="nanite_rate_data_")
-    with h5py.File(path, mode="r") as h5:
-        if not meta_only:
-            # extract experimental data
-            dataset_dict = {}
-            for dkey in h5["data"]:
-                dset = h5["data"][dkey]
-                dbin = dset[...]
-                name = dkey + "_" + pathlib.Path(dset.attrs["path"]).name
-                dpath = pathlib.Path(tdir) / name
-                dbin.tofile(str(dpath))
-                dataset_dict[dkey] = IndentationGroup(dpath)
-        # load individual curves
-        for akey in h5["analysis"]:
-            h5gr = h5["analysis"][akey]
-            attrs = h5gr.attrs
-            if not meta_only:
-                indent = dataset_dict[attrs["data hash"]].get_enum(
-                    attrs["data enum"])
-                indent["fit"] = h5gr["fit"][...]
-                indent["fit range"] = h5gr["fit range"][...]
-                indent["force"] = h5gr["force"][...]
-                indent["fit residuals"] = h5gr["fit residuals"][...]
-                indent["tip position"] = h5gr["tip position"][...]
-                indent["segment"] = h5gr["segment"][...]
-            fit_properties = {}
-            fkeys = [key for key in attrs if key.startswith("fit ")]
-            for fkey in fkeys:
-                key = fkey[4:]
-                val = attrs[fkey]
-                if key.startswith("params"):
-                    parms = lmfit.Parameters()
-                    parms.loads(val)
-                    val = parms
-                elif key == "preprocessing":
-                    val = val.split(",")
-                elif key in ["preprocessing_options", "method_kws"]:
-                    val = json.loads(val)
-                elif key == "range_x":
-                    val = val.strip("[]() ").split(",")
-                    val = (float(val[0]), float(val[1]))
-                fit_properties[key] = val
-            rating = {
-                "name": attrs["user name"],
-                "rating": attrs["user rate"],
-                "comment": attrs["user comment"],
-                "enum": attrs["data enum"],
-                "fit properties": fit_properties,
-            }
-            if not meta_only:
-                # This overrides the FitProperties class!
-                indent.fit_properties = fit_properties
-                rating["data_set"] = indent
-            ratings.append(rating)
-
-    shutil.rmtree(tdir, ignore_errors=True)
-    return ratings
-
-
-def save_hdf5(h5path, indent, user_rate, user_name, user_comment, h5mode="a"):
-    """Store all relevant data of a user rating into an hdf5 file
-
-    Parameters
-    ----------
-    h5path: str or pathlib.Path
-        Path to HDF5 rating container where data will be stored
-    indent: nanite.Indentation
-        The experimental data processed and fitted with nanite
-    user_rate: float
-        Rating given by the user
-    user_name: str
-        Name of the rating user
-    """
-    dkw = {"fletcher32": True,
-           "compression": "gzip",
-           "compression_opts": 9}
-    with h5py.File(h5path, mode=h5mode) as h5:
-        # store raw experimental data as binary array
-        data = h5.require_group("data")
-        dhash = hash_file(indent.path)
-        if dhash not in data:
-            meas = data.create_dataset(
-                dhash,
-                data=np.fromfile(str(indent.path), dtype=bool),
-                **dkw
-            )
-            meas.attrs["path"] = str(indent.path)
-        # store indentation data along with the user rate
-        ana = h5.require_group("analysis")
-        idd = "{}_{}".format(dhash, indent.enum)
-        if idd in ana:
-            # Only allow overriding of user data if fit matches.
-            # Otherwise, the rating might be wrong.
-            if not np.allclose(indent["fit"], ana[idd]["fit"], equal_nan=True):
-                raise ValueError("Cannot store rating for different fit in "
-                                 "same rating container!")
-            out = ana[idd]
-        else:
-            out = ana.create_group(idd)
-            out.attrs["data enum"] = indent.enum
-            out.attrs["data hash"] = dhash
-            for key in indent.fit_properties:
-                val = indent.fit_properties[key]
-                if key.startswith("params_"):
-                    val = val.dumps()
-                elif key == "preprocessing":
-                    val = ",".join(val)
-                elif key in ["preprocessing_options", "method_kws"]:
-                    val = json.dumps(val)
-                elif key == "range_x":
-                    val = str(val)
-                out.attrs["fit {}".format(key)] = val
-
-            out.create_dataset("fit",
-                               data=indent["fit"][...],
-                               **dkw)
-            out.create_dataset("fit range",
-                               data=indent["fit range"][...],
-                               **dkw)
-            out.create_dataset("force",
-                               data=indent["force"][...],
-                               **dkw)
-            out.create_dataset("fit residuals",
-                               data=indent["fit residuals"][...],
-                               **dkw)
-            out.create_dataset("tip position",
-                               data=indent["tip position"][...],
-                               **dkw)
-            out.create_dataset("segment",
-                               data=indent["segment"][...],
-                               **dkw)
-        # update user data in any case
-        out.attrs["user comment"] = user_comment
-        out.attrs["user name"] = user_name
-        out.attrs["user rate"] = user_rate
-        out.attrs["user time"] = time.time()
-        out.attrs["user time str"] = time.ctime()
-        # add library versions for debugging
-        out.attrs["nanite version"] = nanite_version
-        out.attrs["h5py version"] = h5py.__version__
-
-
-def hdf5_rated(h5path, indent):
-    """Test whether an indentation has already been rated
-
-    Returns
-    -------
-    is_rated, rating, comment
-    """
-    is_rated = False
-    rating = -1
-    comment = ""
-    h5path = pathlib.Path(h5path)
-    if h5path.exists():
-        with h5py.File(h5path, mode="r") as h5:
-            if "analysis" in h5:
-                ana = h5["analysis"]
-                dhash = hash_file(indent.path)
-                idd = "{}_{}".format(dhash, indent.enum)
-                if idd in ana:
-                    is_rated = True
-                    rating = ana[idd].attrs["user rate"]
-                    comment = ana[idd].attrs["user comment"]
-    return is_rated, rating, comment
+"""Save and load user-rated datasets"""
+from functools import lru_cache
+import hashlib
+import json
+import pathlib
+import shutil
+import tempfile
+import time
+
+import h5py
+import lmfit
+import numpy as np
+from sklearn import model_selection
+
+from .._version import version as nanite_version
+from ..group import IndentationGroup
+from . import rater
+
+
+class RateManager:
+    def __init__(self, path, verbose=0):
+        """Manage user-defined rates"""
+        #: Path to the manual ratings (directory or .h5 file)
+        self.path = pathlib.Path(path)
+        #: verbosity level
+        self.verbose = verbose
+        self._ratings = None
+
+    @staticmethod
+    def _get_samples(path, verbose=0):
+        rm = RateManager(path, verbose=verbose)
+        samples = []
+        idr = rater.IndentationRater
+        for ds in rm.datasets:
+            assert "success" in ds.fit_properties
+            features = idr.compute_features(ds)
+            samples.append(features)
+        return np.array(samples, dtype=float)
+
+    @property
+    def datasets(self):
+        return [r["data_set"] for r in self.ratings]
+
+    @property
+    def ratings(self):
+        if self._ratings is None:
+            self._ratings = load(self.path, verbose=self.verbose)
+        return self._ratings
+
+    @property
+    def samples(self):
+        """The individual sample ratings computed by afmlib"""
+        return RateManager._get_samples(self.path, verbose=self.verbose)
+
+    def export_training_set(self, path):
+        path = pathlib.Path(path)
+        path.mkdir(parents=True, exist_ok=True)
+        raters = rater.IndentationRater.get_feature_funcs()
+        samples = self.samples
+        for ii, rti in enumerate(raters):
+            rpath = path / "train_{}.txt".format(rti[0])
+            np.savetxt(rpath, samples[:, ii].flatten(), fmt="%.2e")
+        user = self.get_rates(which="user")
+        upath = str(path / "train_response.txt")
+        np.savetxt(upath, user.flatten(), fmt="%.2e")
+
+    def get_cross_validation_score(self, regressor, training_set=None,
+                                   n_splits=20, random_state=42):
+        """Regressor cross-validation scoring
+
+        Cross-validation is used to identify regressors that
+        over-fit the train set by splitting the train set into
+        multiple learn/test sets and quantifying the regressor
+        performance for each split.
+
+        Parameters
+        ----------
+        regressor: str or RegressorMixin
+            If a string, must be in `reg_names`.
+        training_set: X, y
+            If given, do not use self.samples
+
+        Notes
+        -----
+        A :class:`skimage.model_selection.KFold` cross validator is used
+        in combination with the mean squared error score.
+
+        Cross-validation score is computed from samples that are filtered
+        with the binary features and only from samples that do not contain
+        any nan values.
+        """
+        ir = rater.get_rater(regressor)
+
+        if training_set:
+            X, y = training_set
+        else:
+            # remove binary features and nans otherwise cross-validation
+            # will not work
+            X, y = self.get_training_set(prefilter_binary=True,
+                                         remove_nans=True)
+
+        # The score is maximized, therefore it is "neg_"
+        scoring = 'neg_mean_squared_error'
+        loo = model_selection.KFold(n_splits=n_splits, shuffle=True,
+                                    random_state=random_state)
+        scores = model_selection.cross_val_score(ir.pipeline, X, y,
+                                                 scoring=scoring, cv=loo)
+        return -scores
+
+    def get_rates(self, which="user", training_set="zef18"):
+        """
+        which: str
+            Which rating to return: "user" or a regressor name
+        """
+        if which == "user":
+            rtngs = np.array([ri["rating"]
+                              for ri in load(self.path, meta_only=True)])
+        else:
+            rt = rater.get_rater(regressor=which, training_set=training_set)
+            rtngs = rt.rate(self.samples)
+        return rtngs
+
+    def get_training_set(self, which_type="all", prefilter_binary=False,
+                         remove_nans=False, transform=False):
+        """Return (X, y) training set"""
+        X = self.samples
+        y = self.get_rates(which="user")
+
+        if prefilter_binary:
+            # remove samples with `False` in a binary feature
+            ir = rater.IndentationRater(regressor=None)
+            bnames, bind = ir.get_feature_names(which_type="binary",
+                                                ret_indices=True)
+            if bnames:
+                X_bool = X[:, bind]
+
+                X_f = []
+                y_f = []
+                for ii in range(len(y)):
+                    if ir._pre_rate(X_bool[ii]):
+                        X_f.append(X[ii])
+                        y_f.append(y[ii])
+                X, y = np.array(X_f), np.array(y_f)
+
+        # must come after prefilter_binary
+        if which_type != "all":
+            _unames, indices = rater.IndentationRater.get_feature_names(
+                which_type=which_type,
+                ret_indices=True)
+            # remove unwanted features
+            if X.size:
+                X = X[:, list(indices)]
+
+        if remove_nans:
+            X_n = []
+            y_n = []
+            for ii in range(len(y)):
+                if not np.sum(np.isnan(X[ii])):
+                    X_n.append(X[ii])
+                    y_n.append(y[ii])
+            X, y = np.array(X_n), np.array(y_n)
+
+        if transform:
+            # Transform data
+            ir = rater.IndentationRater(regressor=None,
+                                        training_set=(X, y)
+                                        )
+            X = ir.pipeline.transform(X)
+        return X, y
+
+
+@lru_cache(maxsize=100)
+def hash_file(path, blocksize=65536):
+    """Compute sha256 hex-hash of a file
+
+    Parameters
+    ----------
+    path: str or pathlib.Path
+        path to the file
+    blocksize: int
+        block size read from the file
+
+    Returns
+    -------
+    hex: str
+        The first six characters of the hash
+    """
+    fname = pathlib.Path(path)
+    hasher = hashlib.sha256()
+    with fname.open('rb') as fd:
+        buf = fd.read(blocksize)
+        while len(buf) > 0:
+            hasher.update(buf)
+            buf = fd.read(blocksize)
+    return hasher.hexdigest()[:6]
+
+
+def load(path, meta_only=False, verbose=0):
+    """
+
+    Notes
+    -----
+    The .fit_properties attribute of each Indentation instance
+    is overridden by a simple dictionary,
+    so its functionalities are not available anymore.
+    """
+    path = pathlib.Path(path)
+    ratings = []
+    if path.is_dir():
+        if verbose:
+            print("Performing iterative folder search.")
+        for fpath in sorted(path.rglob("*.h5")):
+            ratings += load(fpath, meta_only=meta_only)
+    elif path.suffix == ".h5":
+        if verbose:
+            print("Loading file '{}'... ".format(path), end="", flush=True)
+        ratings += load_hdf5(path, meta_only=meta_only)
+        if verbose:
+            print("Done.")
+    return ratings
+
+
+def load_hdf5(path, meta_only=False):
+    ratings = []
+    path = pathlib.Path(path)
+    # temporary directory for original data
+    tdir = tempfile.mkdtemp(prefix="nanite_rate_data_")
+    with h5py.File(path, mode="r") as h5:
+        if not meta_only:
+            # extract experimental data
+            dataset_dict = {}
+            for dkey in h5["data"]:
+                dset = h5["data"][dkey]
+                dbin = dset[...]
+                name = dkey + "_" + pathlib.Path(dset.attrs["path"]).name
+                dpath = pathlib.Path(tdir) / name
+                dbin.tofile(str(dpath))
+                dataset_dict[dkey] = IndentationGroup(dpath)
+        # load individual curves
+        for akey in h5["analysis"]:
+            h5gr = h5["analysis"][akey]
+            attrs = h5gr.attrs
+            if not meta_only:
+                indent = dataset_dict[attrs["data hash"]].get_enum(
+                    attrs["data enum"])
+                indent["fit"] = h5gr["fit"][...]
+                indent["fit range"] = h5gr["fit range"][...]
+                indent["force"] = h5gr["force"][...]
+                indent["fit residuals"] = h5gr["fit residuals"][...]
+                indent["tip position"] = h5gr["tip position"][...]
+                indent["segment"] = h5gr["segment"][...]
+            fit_properties = {}
+            fkeys = [key for key in attrs if key.startswith("fit ")]
+            for fkey in fkeys:
+                key = fkey[4:]
+                val = attrs[fkey]
+                if key.startswith("params"):
+                    parms = lmfit.Parameters()
+                    parms.loads(val)
+                    val = parms
+                elif key == "preprocessing":
+                    val = val.split(",")
+                elif key in ["preprocessing_options", "method_kws"]:
+                    val = json.loads(val)
+                elif key == "range_x":
+                    val = val.strip("[]() ").split(",")
+                    val = (float(val[0]), float(val[1]))
+                fit_properties[key] = val
+            rating = {
+                "name": attrs["user name"],
+                "rating": attrs["user rate"],
+                "comment": attrs["user comment"],
+                "enum": attrs["data enum"],
+                "fit properties": fit_properties,
+            }
+            if not meta_only:
+                # This overrides the FitProperties class!
+                indent.fit_properties = fit_properties
+                rating["data_set"] = indent
+            ratings.append(rating)
+
+    shutil.rmtree(tdir, ignore_errors=True)
+    return ratings
+
+
+def save_hdf5(h5path, indent, user_rate, user_name, user_comment, h5mode="a"):
+    """Store all relevant data of a user rating into an hdf5 file
+
+    Parameters
+    ----------
+    h5path: str or pathlib.Path
+        Path to HDF5 rating container where data will be stored
+    indent: nanite.Indentation
+        The experimental data processed and fitted with nanite
+    user_rate: float
+        Rating given by the user
+    user_name: str
+        Name of the rating user
+    """
+    dkw = {"fletcher32": True,
+           "compression": "gzip",
+           "compression_opts": 9}
+    with h5py.File(h5path, mode=h5mode) as h5:
+        # store raw experimental data as binary array
+        data = h5.require_group("data")
+        dhash = hash_file(indent.path)
+        if dhash not in data:
+            meas = data.create_dataset(
+                dhash,
+                data=np.fromfile(str(indent.path), dtype=bool),
+                **dkw
+            )
+            meas.attrs["path"] = str(indent.path)
+        # store indentation data along with the user rate
+        ana = h5.require_group("analysis")
+        idd = "{}_{}".format(dhash, indent.enum)
+        if idd in ana:
+            # Only allow overriding of user data if fit matches.
+            # Otherwise, the rating might be wrong.
+            if not np.allclose(indent["fit"], ana[idd]["fit"], equal_nan=True):
+                raise ValueError("Cannot store rating for different fit in "
+                                 "same rating container!")
+            out = ana[idd]
+        else:
+            out = ana.create_group(idd)
+            out.attrs["data enum"] = indent.enum
+            out.attrs["data hash"] = dhash
+            for key in indent.fit_properties:
+                val = indent.fit_properties[key]
+                if key.startswith("params_"):
+                    val = val.dumps()
+                elif key == "preprocessing":
+                    val = ",".join(val)
+                elif key in ["preprocessing_options", "method_kws"]:
+                    val = json.dumps(val)
+                elif key == "range_x":
+                    val = str(val)
+                out.attrs["fit {}".format(key)] = val
+
+            out.create_dataset("fit",
+                               data=indent["fit"][...],
+                               **dkw)
+            out.create_dataset("fit range",
+                               data=indent["fit range"][...],
+                               **dkw)
+            out.create_dataset("force",
+                               data=indent["force"][...],
+                               **dkw)
+            out.create_dataset("fit residuals",
+                               data=indent["fit residuals"][...],
+                               **dkw)
+            out.create_dataset("tip position",
+                               data=indent["tip position"][...],
+                               **dkw)
+            out.create_dataset("segment",
+                               data=indent["segment"][...],
+                               **dkw)
+        # update user data in any case
+        out.attrs["user comment"] = user_comment
+        out.attrs["user name"] = user_name
+        out.attrs["user rate"] = user_rate
+        out.attrs["user time"] = time.time()
+        out.attrs["user time str"] = time.ctime()
+        # add library versions for debugging
+        out.attrs["nanite version"] = nanite_version
+        out.attrs["h5py version"] = h5py.__version__
+
+
+def hdf5_rated(h5path, indent):
+    """Test whether an indentation has already been rated
+
+    Returns
+    -------
+    is_rated, rating, comment
+    """
+    is_rated = False
+    rating = -1
+    comment = ""
+    h5path = pathlib.Path(h5path)
+    if h5path.exists():
+        with h5py.File(h5path, mode="r") as h5:
+            if "analysis" in h5:
+                ana = h5["analysis"]
+                dhash = hash_file(indent.path)
+                idd = "{}_{}".format(dhash, indent.enum)
+                if idd in ana:
+                    is_rated = True
+                    rating = ana[idd].attrs["user rate"]
+                    comment = ana[idd].attrs["user comment"]
+    return is_rated, rating, comment
```

### Comparing `nanite-3.5.4/nanite/rate/rater.py` & `nanite-3.6.0/nanite/rate/rater.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,326 +1,326 @@
-import pathlib
-from pkg_resources import resource_filename
-
-import numpy as np
-from sklearn.pipeline import make_pipeline
-from sklearn.preprocessing import StandardScaler
-from sklearn.discriminant_analysis import LinearDiscriminantAnalysis
-from sklearn.preprocessing import FunctionTransformer
-
-
-from .features import IndentationFeatures
-from .regressors import reg_dict, reg_names, reg_trees
-
-
-class IndentationRater(IndentationFeatures):
-    def __init__(self, regressor=None, scale=None, lda=None,
-                 training_set=None, names=None,
-                 weight=True, sample_weight=None,
-                 *args, **kwargs):
-        """Rate quality
-
-        Parameters
-        ----------
-        regressor: sciki-learn RegressorMixin
-            The regressor used for rating
-        scale: bool
-            If True, apply a Standard Scaler. If a regressor based on
-            decision trees is used, the Standard Scaler is not used
-            by default, otherwise it is.
-        lda: bool
-            If True, apply a Linear Discriminant Analysis (LDA). If a
-            regressor based on a decision tree is used, LDA is not
-            used by default, otherwise it is.
-        training_set: tuple of (X, y)
-            The training set (samples, response)
-        names: list of str
-            Feature names to use
-        weight: bool
-            Weight the input samples by the number of occurrences
-            or with `sample_weight`. For tree-based classifiers, set this
-            to True to avoid bias.
-        sample_weight: list-like
-            The sample weights. If set to `None` sample weights
-            are computed from the training set.
-        *args: list
-            Positional arguments for :class:`IndentationFeatures`
-        **kwargs:
-            Keyword arguments for :class:`IndentationFeatures`
-
-        See Also
-        --------
-        sklearn.preprocessing.StandardScaler:
-            Standard scaler
-        sklearn.discriminant_analysis.LinearDiscriminantAnalysis:
-            Linear discriminant analysis
-        nanite.rate.regressors.reg_trees:
-            List of regressors that are identified as tree-based
-        """
-        if regressor is not None:
-            _name = regressor.__class__.__name__
-            if lda is None:
-                lda = False if _name in reg_trees else True
-            if scale is None:
-                scale = False if _name in reg_trees else True
-
-        # training set
-        if training_set is None:
-            # default
-            training_set = self.load_training_set(names=names)
-        # sample weights
-        if sample_weight is None:
-            sample_weight = self.compute_sample_weight(*training_set)
-        steps = []
-
-        # scaling (does not affect decision trees / random forests)
-        if scale:
-            steps.append(StandardScaler())
-        # linear discriminant analysis
-        if lda:
-            steps.append(LinearDiscriminantAnalysis())
-
-        if regressor is not None:
-            steps.append(regressor)
-
-        if len(steps) == 0:
-            dummy = FunctionTransformer(lambda x: x)
-            steps.append(dummy)
-
-        #: sklearn pipeline with transforms (and regressor if given)
-        self.pipeline = make_pipeline(*steps)
-
-        fit_params = {}
-        if regressor is not None and weight:
-            # set weighting for regressor
-            key = "{}__sample_weight".format(self.pipeline.steps[-1][0])
-            fit_params[key] = sample_weight
-
-        if regressor is not None:
-            self.pipeline.fit(*training_set, **fit_params)
-
-        names = self.get_feature_names(names=names, which_type="all")
-
-        #: feature names used by the regressor pipeline
-        self.names = sorted(names)
-        super(IndentationRater, self).__init__(*args, **kwargs)
-
-    def _pre_rate(self, bsample):
-        """exclude based on boolean training set"""
-        if np.sum(bsample == 0):
-            # bad curve
-            return False
-        else:
-            # good curve
-            return True
-
-    def _rate(self, sample):
-        gd = self.pipeline.predict(np.atleast_2d(sample))
-        return gd[0]
-
-    @staticmethod
-    def compute_sample_weight(X, y):
-        """Weight samples according to occurrence in y"""
-        if not np.all(np.array(y, dtype=int) == y):
-            msg = "Only integer ratings allowed."
-            raise NotImplementedError(msg)
-        weight = np.zeros(y.shape[0], dtype=float)
-        for ii in range(11):
-            idxii = y == ii
-            occur = np.sum(idxii)
-            if occur:
-                # Sometimes the training set is not large enough.
-                # If no occurences were found, the weights remain
-                # zero.
-                weight[idxii] = 1 / occur
-        # normalize
-        weight /= np.sum(weight)
-        return weight
-
-    @staticmethod
-    def get_training_set_path(label="zef18"):
-        """Return the path to a training set shipped with nanite
-
-        Training sets are stored in the `nanite.rate`
-        module path with ``ts_`` prepended to `label`.
-        """
-        data_loc = "nanite.rate"
-        resp_path = resource_filename(data_loc, "ts_{}".format(label))
-        return resp_path
-
-    @classmethod
-    def load_training_set(cls, path=None, names=None,
-                          which_type=["continuous"],
-                          remove_nan=True, ret_names=False):
-        """Load a training set from a directory
-
-        By default, only the "continuous" features are imported. The
-        "binary" features are not needed for training; they are used
-        to sort out new force-distance data.
-        """
-        fnames = cls.get_feature_names(which_type=which_type, names=names)
-        sample_paths = []
-        if path is None:
-            path = cls.get_training_set_path()
-        path = pathlib.Path(path).resolve()
-
-        resp_path = str(path / "train_response.txt")
-        for fn in fnames:
-            resf = str(path / "train_{}.txt".format(fn))
-            sample_paths.append(resf)
-
-        samples = [np.loadtxt(sp, dtype=float, ndmin=2) for sp in sample_paths]
-        samples = np.concatenate(samples, axis=1)
-        response = np.loadtxt(resp_path, dtype=float)
-        if remove_nan:
-            # Remove nan-values from training set
-            valid = ~np.isnan(np.sum(samples, axis=1))
-            samples = samples[valid, :]
-            # remove corresponding responses
-            response = response[valid]
-
-        res = [samples, response]
-
-        if ret_names:
-            res.append(fnames)
-
-        return res
-
-    def rate(self, samples=None, datasets=None):
-        """Perform rating step
-
-        Parameters
-        ----------
-        samples: 1d or 2d ndarray (cast to 2d ndarray) or None
-            Measured samples, if set to None, `dataset` must be given.
-        dataset: list of nanite.Indentation
-            Full, fitted measurement
-
-        Returns
-        -------
-        ratings: list
-            Resulting ratings
-        """
-        if samples is None and datasets is None:
-            # use dataset from IndentationFeature
-            datasets = [self.dataset]
-        elif datasets is None:
-            # distinguish between binary and other samples
-            fsamples = []
-            bsamples = []
-            fnames = self.get_feature_names(
-                names=self.names,
-                which_type=["continuous"])
-            for samp in samples:
-                fsamp = []  # continuous samples
-                bsamp = []  # binary samples
-                for ii, name in enumerate(self.names):
-                    if name in fnames:
-                        fsamp.append(samp[ii])
-                    else:
-                        assert name.startswith("feat_bin_")
-                        bsamp.append(samp[ii])
-                fsamples.append(fsamp)
-                bsamples.append(bsamp)
-        else:
-            if not isinstance(datasets, (list, tuple)):
-                datasets = [datasets]
-            fsamples = []
-            bsamples = []
-            # continuous features
-            for idnt in datasets:
-                samp = self.compute_features(
-                    idnt=idnt,
-                    names=self.names,
-                    which_type=["continuous"])
-                fsamples.append(samp)
-            # binary features
-            for idnt in datasets:
-                bsamp = self.compute_features(idnt=idnt,
-                                              names=self.names,
-                                              which_type="binary")
-                bsamples.append(bsamp)
-
-        fsamples = np.atleast_2d(fsamples)
-        bsamples = np.atleast_2d(bsamples)
-
-        ratings = []
-        for bsamp, fsamp in zip(bsamples, fsamples):
-            if not self._pre_rate(bsamp):
-                # certainly a bad curve
-                gd = 0
-            elif np.isnan(np.sum(fsamp)):
-                # ignore nan-valued samples
-                gd = -1
-            else:
-                gd = self._rate(fsamp)
-            ratings.append(gd)
-
-        return np.array(ratings).flatten()
-
-
-def get_available_training_sets():
-    """List of internal training sets"""
-    data_loc = "nanite"
-    resp_path = resource_filename(data_loc, "rate")
-    avail = []
-    for pp in pathlib.Path(resp_path).glob("ts_*"):
-        avail.append(pp.name[3:])
-    return sorted(avail)
-
-
-def get_rater(regressor, training_set="zef18", names=None,
-              lda=None, **reg_kwargs):
-    """Convenience method to get a rater
-
-    Parameters
-    ----------
-    regressor: str or RegressorMixin
-        If a string, must be in `reg_names`.
-    training_set: str or pathlib.Path or tuple (X, y)
-        A string label representing a training set shipped with
-        nanite, the path to a training set, or a tuple
-        representing the training set (samples, response)
-        for use with sklearn.
-    names: list of str
-        Only use these features for rating
-    lda: bool
-        Perform linear discriminant analysis
-
-    Returns
-    -------
-    irater: nanite.IndentationRater
-        The rating instance.
-    """
-    avr = get_available_training_sets()
-    if isinstance(training_set, tuple):
-        pass
-    else:
-        if training_set in avr:
-            ts_path = IndentationRater.get_training_set_path(
-                label=training_set)
-        else:
-            ts_path = training_set
-        training_set = IndentationRater.load_training_set(
-            path=ts_path,
-            names=names)
-
-    if len(training_set) != 2:
-        raise ValueError("Expected training_set of the form (X, y)!")
-
-    if isinstance(regressor, str):
-        if regressor not in reg_names:
-            msg = "Unknown regressor name: '{}'!".format(regressor) \
-                  + " Please pass your own sklearn RegressorMixin."
-            raise ValueError(msg)
-        reg_cl, default_kw = reg_dict[regressor]
-        kw = default_kw.copy()
-        kw.update(reg_kwargs)
-        regr = reg_cl(**kw)
-    else:
-        regr = regressor
-
-    rater = IndentationRater(regressor=regr,
-                             training_set=training_set,
-                             names=names,
-                             lda=lda)
-    return rater
+import pathlib
+from pkg_resources import resource_filename
+
+import numpy as np
+from sklearn.pipeline import make_pipeline
+from sklearn.preprocessing import StandardScaler
+from sklearn.discriminant_analysis import LinearDiscriminantAnalysis
+from sklearn.preprocessing import FunctionTransformer
+
+
+from .features import IndentationFeatures
+from .regressors import reg_dict, reg_names, reg_trees
+
+
+class IndentationRater(IndentationFeatures):
+    def __init__(self, regressor=None, scale=None, lda=None,
+                 training_set=None, names=None,
+                 weight=True, sample_weight=None,
+                 *args, **kwargs):
+        """Rate quality
+
+        Parameters
+        ----------
+        regressor: sciki-learn RegressorMixin
+            The regressor used for rating
+        scale: bool
+            If True, apply a Standard Scaler. If a regressor based on
+            decision trees is used, the Standard Scaler is not used
+            by default, otherwise it is.
+        lda: bool
+            If True, apply a Linear Discriminant Analysis (LDA). If a
+            regressor based on a decision tree is used, LDA is not
+            used by default, otherwise it is.
+        training_set: tuple of (X, y)
+            The training set (samples, response)
+        names: list of str
+            Feature names to use
+        weight: bool
+            Weight the input samples by the number of occurrences
+            or with `sample_weight`. For tree-based classifiers, set this
+            to True to avoid bias.
+        sample_weight: list-like
+            The sample weights. If set to `None` sample weights
+            are computed from the training set.
+        *args: list
+            Positional arguments for :class:`IndentationFeatures`
+        **kwargs:
+            Keyword arguments for :class:`IndentationFeatures`
+
+        See Also
+        --------
+        sklearn.preprocessing.StandardScaler:
+            Standard scaler
+        sklearn.discriminant_analysis.LinearDiscriminantAnalysis:
+            Linear discriminant analysis
+        nanite.rate.regressors.reg_trees:
+            List of regressors that are identified as tree-based
+        """
+        if regressor is not None:
+            _name = regressor.__class__.__name__
+            if lda is None:
+                lda = False if _name in reg_trees else True
+            if scale is None:
+                scale = False if _name in reg_trees else True
+
+        # training set
+        if training_set is None:
+            # default
+            training_set = self.load_training_set(names=names)
+        # sample weights
+        if sample_weight is None:
+            sample_weight = self.compute_sample_weight(*training_set)
+        steps = []
+
+        # scaling (does not affect decision trees / random forests)
+        if scale:
+            steps.append(StandardScaler())
+        # linear discriminant analysis
+        if lda:
+            steps.append(LinearDiscriminantAnalysis())
+
+        if regressor is not None:
+            steps.append(regressor)
+
+        if len(steps) == 0:
+            dummy = FunctionTransformer(lambda x: x)
+            steps.append(dummy)
+
+        #: sklearn pipeline with transforms (and regressor if given)
+        self.pipeline = make_pipeline(*steps)
+
+        fit_params = {}
+        if regressor is not None and weight:
+            # set weighting for regressor
+            key = "{}__sample_weight".format(self.pipeline.steps[-1][0])
+            fit_params[key] = sample_weight
+
+        if regressor is not None:
+            self.pipeline.fit(*training_set, **fit_params)
+
+        names = self.get_feature_names(names=names, which_type="all")
+
+        #: feature names used by the regressor pipeline
+        self.names = sorted(names)
+        super(IndentationRater, self).__init__(*args, **kwargs)
+
+    def _pre_rate(self, bsample):
+        """exclude based on boolean training set"""
+        if np.sum(bsample == 0):
+            # bad curve
+            return False
+        else:
+            # good curve
+            return True
+
+    def _rate(self, sample):
+        gd = self.pipeline.predict(np.atleast_2d(sample))
+        return gd[0]
+
+    @staticmethod
+    def compute_sample_weight(X, y):
+        """Weight samples according to occurrence in y"""
+        if not np.all(np.array(y, dtype=int) == y):
+            msg = "Only integer ratings allowed."
+            raise NotImplementedError(msg)
+        weight = np.zeros(y.shape[0], dtype=float)
+        for ii in range(11):
+            idxii = y == ii
+            occur = np.sum(idxii)
+            if occur:
+                # Sometimes the training set is not large enough.
+                # If no occurences were found, the weights remain
+                # zero.
+                weight[idxii] = 1 / occur
+        # normalize
+        weight /= np.sum(weight)
+        return weight
+
+    @staticmethod
+    def get_training_set_path(label="zef18"):
+        """Return the path to a training set shipped with nanite
+
+        Training sets are stored in the `nanite.rate`
+        module path with ``ts_`` prepended to `label`.
+        """
+        data_loc = "nanite.rate"
+        resp_path = resource_filename(data_loc, "ts_{}".format(label))
+        return resp_path
+
+    @classmethod
+    def load_training_set(cls, path=None, names=None,
+                          which_type=["continuous"],
+                          remove_nan=True, ret_names=False):
+        """Load a training set from a directory
+
+        By default, only the "continuous" features are imported. The
+        "binary" features are not needed for training; they are used
+        to sort out new force-distance data.
+        """
+        fnames = cls.get_feature_names(which_type=which_type, names=names)
+        sample_paths = []
+        if path is None:
+            path = cls.get_training_set_path()
+        path = pathlib.Path(path).resolve()
+
+        resp_path = str(path / "train_response.txt")
+        for fn in fnames:
+            resf = str(path / "train_{}.txt".format(fn))
+            sample_paths.append(resf)
+
+        samples = [np.loadtxt(sp, dtype=float, ndmin=2) for sp in sample_paths]
+        samples = np.concatenate(samples, axis=1)
+        response = np.loadtxt(resp_path, dtype=float)
+        if remove_nan:
+            # Remove nan-values from training set
+            valid = ~np.isnan(np.sum(samples, axis=1))
+            samples = samples[valid, :]
+            # remove corresponding responses
+            response = response[valid]
+
+        res = [samples, response]
+
+        if ret_names:
+            res.append(fnames)
+
+        return res
+
+    def rate(self, samples=None, datasets=None):
+        """Perform rating step
+
+        Parameters
+        ----------
+        samples: 1d or 2d ndarray (cast to 2d ndarray) or None
+            Measured samples, if set to None, `dataset` must be given.
+        dataset: list of nanite.Indentation
+            Full, fitted measurement
+
+        Returns
+        -------
+        ratings: list
+            Resulting ratings
+        """
+        if samples is None and datasets is None:
+            # use dataset from IndentationFeature
+            datasets = [self.dataset]
+        elif datasets is None:
+            # distinguish between binary and other samples
+            fsamples = []
+            bsamples = []
+            fnames = self.get_feature_names(
+                names=self.names,
+                which_type=["continuous"])
+            for samp in samples:
+                fsamp = []  # continuous samples
+                bsamp = []  # binary samples
+                for ii, name in enumerate(self.names):
+                    if name in fnames:
+                        fsamp.append(samp[ii])
+                    else:
+                        assert name.startswith("feat_bin_")
+                        bsamp.append(samp[ii])
+                fsamples.append(fsamp)
+                bsamples.append(bsamp)
+        else:
+            if not isinstance(datasets, (list, tuple)):
+                datasets = [datasets]
+            fsamples = []
+            bsamples = []
+            # continuous features
+            for idnt in datasets:
+                samp = self.compute_features(
+                    idnt=idnt,
+                    names=self.names,
+                    which_type=["continuous"])
+                fsamples.append(samp)
+            # binary features
+            for idnt in datasets:
+                bsamp = self.compute_features(idnt=idnt,
+                                              names=self.names,
+                                              which_type="binary")
+                bsamples.append(bsamp)
+
+        fsamples = np.atleast_2d(fsamples)
+        bsamples = np.atleast_2d(bsamples)
+
+        ratings = []
+        for bsamp, fsamp in zip(bsamples, fsamples):
+            if not self._pre_rate(bsamp):
+                # certainly a bad curve
+                gd = 0
+            elif np.isnan(np.sum(fsamp)):
+                # ignore nan-valued samples
+                gd = -1
+            else:
+                gd = self._rate(fsamp)
+            ratings.append(gd)
+
+        return np.array(ratings).flatten()
+
+
+def get_available_training_sets():
+    """List of internal training sets"""
+    data_loc = "nanite"
+    resp_path = resource_filename(data_loc, "rate")
+    avail = []
+    for pp in pathlib.Path(resp_path).glob("ts_*"):
+        avail.append(pp.name[3:])
+    return sorted(avail)
+
+
+def get_rater(regressor, training_set="zef18", names=None,
+              lda=None, **reg_kwargs):
+    """Convenience method to get a rater
+
+    Parameters
+    ----------
+    regressor: str or RegressorMixin
+        If a string, must be in `reg_names`.
+    training_set: str or pathlib.Path or tuple (X, y)
+        A string label representing a training set shipped with
+        nanite, the path to a training set, or a tuple
+        representing the training set (samples, response)
+        for use with sklearn.
+    names: list of str
+        Only use these features for rating
+    lda: bool
+        Perform linear discriminant analysis
+
+    Returns
+    -------
+    irater: nanite.IndentationRater
+        The rating instance.
+    """
+    avr = get_available_training_sets()
+    if isinstance(training_set, tuple):
+        pass
+    else:
+        if training_set in avr:
+            ts_path = IndentationRater.get_training_set_path(
+                label=training_set)
+        else:
+            ts_path = training_set
+        training_set = IndentationRater.load_training_set(
+            path=ts_path,
+            names=names)
+
+    if len(training_set) != 2:
+        raise ValueError("Expected training_set of the form (X, y)!")
+
+    if isinstance(regressor, str):
+        if regressor not in reg_names:
+            msg = "Unknown regressor name: '{}'!".format(regressor) \
+                  + " Please pass your own sklearn RegressorMixin."
+            raise ValueError(msg)
+        reg_cl, default_kw = reg_dict[regressor]
+        kw = default_kw.copy()
+        kw.update(reg_kwargs)
+        regr = reg_cl(**kw)
+    else:
+        regr = regressor
+
+    rater = IndentationRater(regressor=regr,
+                             training_set=training_set,
+                             names=names,
+                             lda=lda)
+    return rater
```

### Comparing `nanite-3.5.4/nanite/rate/regressors.py` & `nanite-3.6.0/nanite/rate/regressors.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,74 +1,74 @@
-"""scikit-learn regressors and their keyword arguments"""
-from sklearn import ensemble, svm, tree
-
-
-reg_dict = {
-    "AdaBoost": [
-        ensemble.AdaBoostRegressor,
-        {"learning_rate": .18,
-         "n_estimators": 100,
-         "random_state": 42,
-         },
-    ],
-    "Decision Tree": [
-        tree.DecisionTreeRegressor,
-        {"max_depth": 6,
-         "min_samples_leaf": 14,
-         "min_samples_split": 3,
-         "random_state": 42,
-         }
-    ],
-    "Extra Trees": [
-        ensemble.ExtraTreesRegressor,
-        {"max_depth": 15,
-         "min_samples_leaf": 1,
-         "min_samples_split": 10,
-         "n_estimators": 100,
-         "random_state": 42,
-         }
-    ],
-    "Gradient Tree Boosting": [
-        ensemble.GradientBoostingRegressor,
-        {"max_depth": 4,
-         "min_samples_leaf": 4,
-         "min_samples_split": 7,
-         "n_estimators": 100,
-         "random_state": 42,
-         }
-    ],
-    "Random Forest": [
-        ensemble.RandomForestRegressor,
-        {"max_depth": 15,
-         "min_samples_leaf": 2,
-         "min_samples_split": 6,
-         "n_estimators": 100,
-         "random_state": 42,
-         }
-    ],
-    "SVR (linear kernel)": [
-        svm.LinearSVR,
-        {"C": 2,
-         "epsilon": .75,
-         "random_state": 42,
-         },
-    ],
-    "SVR (RBF kernel)": [
-        svm.SVR,
-        {"kernel": "rbf",
-         "C": 25,
-         "epsilon": 0.75,
-         },
-    ],
-}
-
-
-#: List of available default regressor names
-reg_names = sorted(reg_dict.keys())
-
-#: List of tree-based regressor class names (used for keyword defaults in
-#: :class:`IndentationRater`)
-reg_trees = ["AdaBoostRegressor",
-             "DecisionTreeRegressor",
-             "ExtraTreesRegressor",
-             "GradientBoostingRegressor",
-             "RandomForestRegressor"]
+"""scikit-learn regressors and their keyword arguments"""
+from sklearn import ensemble, svm, tree
+
+
+reg_dict = {
+    "AdaBoost": [
+        ensemble.AdaBoostRegressor,
+        {"learning_rate": .18,
+         "n_estimators": 100,
+         "random_state": 42,
+         },
+    ],
+    "Decision Tree": [
+        tree.DecisionTreeRegressor,
+        {"max_depth": 6,
+         "min_samples_leaf": 14,
+         "min_samples_split": 3,
+         "random_state": 42,
+         }
+    ],
+    "Extra Trees": [
+        ensemble.ExtraTreesRegressor,
+        {"max_depth": 15,
+         "min_samples_leaf": 1,
+         "min_samples_split": 10,
+         "n_estimators": 100,
+         "random_state": 42,
+         }
+    ],
+    "Gradient Tree Boosting": [
+        ensemble.GradientBoostingRegressor,
+        {"max_depth": 4,
+         "min_samples_leaf": 4,
+         "min_samples_split": 7,
+         "n_estimators": 100,
+         "random_state": 42,
+         }
+    ],
+    "Random Forest": [
+        ensemble.RandomForestRegressor,
+        {"max_depth": 15,
+         "min_samples_leaf": 2,
+         "min_samples_split": 6,
+         "n_estimators": 100,
+         "random_state": 42,
+         }
+    ],
+    "SVR (linear kernel)": [
+        svm.LinearSVR,
+        {"C": 2,
+         "epsilon": .75,
+         "random_state": 42,
+         },
+    ],
+    "SVR (RBF kernel)": [
+        svm.SVR,
+        {"kernel": "rbf",
+         "C": 25,
+         "epsilon": 0.75,
+         },
+    ],
+}
+
+
+#: List of available default regressor names
+reg_names = sorted(reg_dict.keys())
+
+#: List of tree-based regressor class names (used for keyword defaults in
+#: :class:`IndentationRater`)
+reg_trees = ["AdaBoostRegressor",
+             "DecisionTreeRegressor",
+             "ExtraTreesRegressor",
+             "GradientBoostingRegressor",
+             "RandomForestRegressor"]
```

### Comparing `nanite-3.5.4/nanite/rate/ts_zef18/train_feat_con_apr_flatness.txt` & `nanite-3.6.0/nanite/rate/ts_zef18/train_feat_con_apr_flatness.txt`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,1132 +1,1132 @@
-3.26e-01
-3.34e-01
-2.79e-01
-2.53e-01
-3.03e-01
-4.14e-01
-3.63e-01
-3.02e-01
-3.23e-01
-3.24e-01
-2.37e-01
-2.53e-01
-1.38e-01
-3.48e-01
-2.79e-01
-2.76e-01
-3.13e-01
-2.41e-01
-3.23e-01
-1.75e-01
-3.14e-01
-2.99e-01
-2.57e-01
-3.26e-01
-2.11e-01
-3.00e-01
-2.15e-01
-1.13e-01
-3.50e-01
-1.85e-01
-2.38e-01
-1.81e-01
-3.03e-01
-2.17e-01
-2.77e-01
-3.58e-01
-3.48e-01
-3.56e-01
-2.41e-01
-3.72e-01
-1.55e-01
-3.75e-01
-1.73e-01
-2.79e-01
-1.71e-01
-1.51e-01
-2.84e-01
-3.87e-01
-3.81e-01
-2.81e-01
-2.61e-01
-2.81e-01
-3.21e-01
-3.47e-01
-3.05e-01
-1.90e-01
-3.12e-01
-2.45e-01
-2.82e-01
-2.84e-01
-2.36e-01
-5.22e-01
-3.85e-01
-2.09e-01
-3.84e-01
-3.01e-01
-2.85e-01
-3.11e-01
-3.02e-01
-3.26e-01
-1.74e-01
-1.93e-01
-2.73e-01
-2.61e-01
-1.13e-01
-3.25e-01
-2.85e-01
-3.08e-01
-1.99e-01
-2.11e-01
-3.16e-01
-2.48e-01
-2.71e-01
-3.21e-01
-3.78e-01
-2.99e-01
-2.66e-01
-2.81e-01
-1.40e-01
-9.32e-02
-1.90e-01
-2.80e-01
-3.51e-01
-4.15e-01
-2.34e-01
-2.47e-01
-2.05e-01
-3.48e-01
-1.91e-01
-1.65e-01
-1.60e-01
-2.10e-01
-1.42e-01
-2.68e-01
-2.87e-01
-2.34e-01
-3.15e-01
-2.39e-01
-1.65e-01
-3.25e-01
-3.38e-01
-3.47e-01
-3.39e-01
-3.64e-01
-2.97e-01
-2.96e-01
-2.93e-01
-3.75e-01
-2.07e-01
-2.42e-01
-2.89e-01
-3.55e-01
-3.69e-01
-1.77e-01
-2.58e-01
-3.56e-01
-2.66e-01
-1.97e-01
-2.34e-01
-3.01e-01
-1.91e-01
-2.65e-01
-8.72e-02
-1.39e-01
-2.39e-01
-3.00e-01
-2.63e-01
-2.10e-02
-3.60e-01
-2.89e-01
-2.32e-01
-2.50e-01
-1.83e-01
-3.79e-01
-3.64e-01
-3.35e-01
-3.21e-01
-1.69e-01
-2.36e-01
-3.76e-01
-2.40e-01
-3.78e-01
-1.09e-01
-2.58e-01
-1.71e-01
-3.05e-01
-2.15e-01
-9.89e-02
-1.81e-01
-1.40e-01
-2.45e-01
-3.25e-01
-2.78e-01
-3.16e-01
-2.44e-01
-3.45e-01
-2.45e-01
-1.38e-01
-1.81e-01
-1.85e-01
-3.20e-01
-3.92e-01
-3.34e-01
-2.60e-01
-2.48e-01
-3.59e-01
-1.05e-01
-3.45e-01
-2.32e-01
-2.44e-01
-3.20e-01
-2.98e-01
-2.38e-01
-2.77e-01
-2.89e-01
-3.11e-01
-1.60e-01
-2.28e-01
-3.26e-01
-2.38e-01
-2.85e-01
-2.79e-01
-2.73e-01
-2.44e-01
-3.43e-01
-3.37e-01
-4.64e-01
-3.15e-01
-1.53e-01
-3.46e-01
-1.99e-01
-3.15e-01
-3.21e-01
-1.81e-01
-3.75e-02
-2.78e-01
-2.43e-01
-1.17e-01
-2.83e-01
-2.69e-01
-1.95e-01
-3.37e-01
-2.88e-01
-2.72e-01
-3.10e-01
-2.13e-01
-3.23e-01
-2.38e-01
-3.03e-01
-3.16e-01
-2.36e-01
-9.04e-02
-3.54e-01
-3.42e-01
-2.56e-01
-3.69e-01
-3.40e-01
-3.62e-01
-3.57e-01
-2.09e-01
-3.17e-01
-2.35e-01
-3.64e-01
-3.85e-01
-1.27e-01
-3.09e-01
-3.14e-01
-2.64e-01
-2.53e-01
-2.99e-01
-2.90e-01
-2.18e-01
-3.09e-01
-3.32e-01
-3.17e-01
-3.72e-01
-3.27e-01
-2.94e-01
-2.69e-01
-3.21e-01
-2.32e-01
-3.43e-01
-2.82e-01
-2.72e-01
-3.37e-01
-2.75e-01
-3.21e-01
-2.82e-01
-2.93e-01
-2.89e-01
-2.42e-01
-3.33e-01
-4.03e-01
-3.74e-01
-3.32e-01
-2.81e-01
-2.91e-01
-3.21e-01
-3.12e-01
-3.09e-01
-3.17e-01
-2.06e-01
-3.89e-01
-2.33e-01
-8.41e-02
-2.35e-01
-2.90e-01
-3.94e-01
-2.81e-01
-2.93e-01
-3.08e-01
-2.15e-01
-3.33e-01
-3.20e-01
-1.35e-01
-1.50e-01
-3.11e-01
-2.75e-01
-9.93e-02
-2.78e-01
-2.72e-01
-3.18e-01
-1.22e-01
-3.93e-01
-2.89e-01
-3.35e-01
-2.41e-01
-3.69e-01
-3.37e-01
-2.24e-01
-2.61e-01
-4.00e-01
-3.24e-01
-2.87e-01
-2.22e-01
-3.54e-01
-3.59e-01
-3.99e-01
-1.18e-01
-3.42e-01
-2.92e-01
-2.90e-01
-1.71e-01
-3.78e-01
-4.08e-01
-1.24e-01
-3.23e-01
-3.51e-01
-2.66e-01
-2.66e-01
-2.68e-01
-3.67e-01
-3.14e-01
-3.59e-01
-2.23e-01
-3.17e-01
-4.18e-01
-2.51e-01
-3.01e-01
-3.27e-01
-4.62e-01
-3.08e-01
-3.15e-01
-2.97e-01
-3.26e-01
-3.14e-01
-3.45e-01
-3.52e-01
-3.43e-01
-2.22e-01
-3.68e-01
-2.37e-02
-3.80e-01
-3.14e-01
-2.22e-01
-4.05e-01
-2.23e-01
-4.65e-01
-3.26e-01
-2.46e-01
-2.58e-01
-2.32e-01
-2.22e-01
-3.33e-01
-2.12e-01
-3.22e-01
-3.40e-01
-3.22e-01
-2.72e-01
-3.75e-01
-2.42e-01
-2.57e-01
-2.48e-01
-3.78e-01
-2.94e-01
-1.72e-01
-2.67e-01
-3.59e-01
-3.33e-01
-3.14e-01
-3.46e-01
-2.55e-01
-1.74e-01
-2.26e-01
-2.83e-01
-2.94e-01
-2.65e-01
-4.07e-01
-3.49e-01
-1.70e-01
-3.70e-01
-2.94e-01
-3.24e-01
-3.58e-01
-3.39e-01
-3.35e-01
-3.93e-01
-3.74e-01
-2.33e-01
-3.54e-01
-2.59e-01
-3.33e-01
-2.92e-01
-3.16e-01
-1.37e-01
-2.86e-01
-1.33e-01
-2.36e-01
-3.91e-01
-2.51e-01
-2.80e-01
-2.12e-01
-3.36e-01
-3.09e-01
-2.31e-01
-2.36e-01
-3.25e-01
-3.30e-01
-3.29e-01
-2.59e-01
-1.95e-01
-2.14e-01
-2.13e-01
-3.35e-01
-3.39e-01
-8.68e-02
-3.41e-01
-3.92e-01
-3.06e-01
-3.27e-01
-3.26e-01
-2.34e-01
-3.19e-01
-2.40e-01
-3.07e-01
-1.76e-01
-3.05e-01
-2.70e-01
-2.79e-01
-2.16e-01
-3.23e-01
-3.07e-01
-3.43e-01
-3.60e-01
-2.79e-01
-3.45e-01
-2.75e-01
-3.23e-01
-2.88e-01
-3.67e-01
-3.23e-01
-4.63e-01
-3.57e-01
-3.39e-01
-1.88e-01
-3.29e-01
-3.72e-01
-2.31e-01
-3.63e-01
-2.26e-01
-3.43e-01
-2.60e-01
-2.69e-01
-3.33e-01
-3.35e-01
-2.18e-01
-2.58e-01
-3.73e-01
-2.18e-01
-1.23e-01
-4.04e-01
-2.80e-01
-3.30e-01
-1.55e-01
-2.31e-01
-3.85e-01
-3.95e-01
-3.30e-01
-2.04e-01
-3.61e-01
-2.91e-01
-2.72e-01
-2.32e-01
-3.25e-01
-3.22e-01
-1.47e-01
-1.81e-01
-1.85e-01
-2.53e-01
-3.07e-01
-3.57e-01
-3.14e-01
-3.52e-01
-3.03e-01
-3.11e-01
-3.16e-01
-2.30e-01
-2.11e-01
-3.22e-01
-3.13e-01
-2.02e-01
-2.90e-01
-1.94e-01
-2.59e-01
-2.98e-01
-2.61e-01
-3.34e-01
-3.18e-01
-2.85e-01
-3.56e-01
-2.52e-01
-3.17e-01
-3.94e-01
-2.84e-01
-3.16e-01
-2.37e-01
-3.00e-01
-2.79e-01
-1.94e-01
-3.10e-01
-3.17e-01
-3.40e-01
-1.88e-01
-1.73e-01
-2.73e-01
-3.50e-01
-3.54e-01
-2.61e-01
-4.11e-01
-3.70e-01
-3.78e-01
-2.61e-01
-1.56e-01
-3.31e-01
-2.33e-01
-1.54e-01
-3.90e-01
-3.04e-01
-3.19e-01
-3.05e-01
-1.46e-01
-2.82e-01
-3.29e-01
-2.86e-01
-2.97e-01
-2.49e-01
-3.14e-01
-3.77e-01
-3.22e-01
-2.15e-01
-3.51e-01
-3.29e-01
-3.28e-01
-2.88e-01
-1.19e-01
-3.07e-01
-2.24e-01
-2.83e-01
-3.03e-01
-2.87e-01
-1.65e-01
-2.27e-01
-2.79e-01
-2.88e-01
-2.95e-01
-2.38e-01
-3.28e-01
-3.16e-01
-2.43e-01
-3.03e-01
-3.72e-01
-3.56e-01
-2.74e-01
-3.01e-01
-2.42e-01
-3.09e-01
-2.63e-01
-3.07e-01
-1.79e-01
-2.83e-01
-2.31e-01
-2.05e-01
-2.91e-01
-9.57e-02
-2.79e-01
-3.15e-01
-9.75e-03
-3.20e-01
-2.44e-01
-4.15e-01
-1.67e-01
-3.17e-01
-3.22e-01
-3.39e-01
-3.28e-01
-2.79e-01
-2.75e-01
-2.90e-01
-2.19e-01
-2.28e-01
-2.43e-01
-3.09e-01
-3.11e-01
-1.95e-01
-1.60e-01
-4.60e-01
-2.05e-01
-2.02e-01
-3.26e-01
-3.21e-01
-3.58e-01
-3.97e-01
-3.17e-01
-1.18e-01
-4.67e-01
-6.97e-02
-2.60e-01
-3.36e-01
-2.62e-01
-3.49e-01
-1.04e-01
-2.97e-01
-2.78e-01
-2.52e-01
-2.04e-01
-1.62e-01
-2.78e-01
-3.45e-01
-3.58e-01
-3.42e-01
-2.92e-01
-3.14e-01
-3.67e-01
-3.41e-01
-3.03e-01
-1.74e-01
-2.69e-01
-2.83e-01
-2.54e-01
-3.76e-01
-1.75e-01
-2.71e-01
-3.72e-01
-3.35e-01
-3.00e-01
-2.45e-01
-2.67e-01
-2.41e-01
-1.99e-01
-2.89e-01
-2.76e-01
-3.04e-01
-3.42e-01
-1.36e-01
-3.73e-01
-2.15e-01
-2.51e-01
-1.60e-01
-3.47e-01
-1.69e-01
-3.85e-01
-2.89e-01
-2.00e-01
-1.98e-01
-3.31e-01
-2.74e-01
-2.86e-01
-3.98e-01
-1.45e-01
-3.03e-01
-3.53e-01
-3.30e-01
-1.79e-01
-1.87e-01
-3.20e-01
-4.28e-02
-2.41e-01
-2.22e-01
-3.04e-01
-2.96e-01
-3.35e-01
-2.71e-01
-3.40e-01
-2.49e-01
-3.41e-01
-3.35e-01
-4.82e-01
-2.24e-01
-3.39e-01
-3.02e-01
-2.80e-01
-1.54e-01
-2.93e-01
-2.62e-01
-2.66e-01
-5.38e-02
-2.92e-01
-2.29e-01
-2.52e-01
-2.58e-01
-2.66e-01
-2.92e-01
-2.71e-01
-3.12e-01
-1.27e-01
-3.27e-01
-1.77e-01
-1.72e-01
-2.96e-01
-2.67e-01
-3.20e-01
-3.49e-01
-3.14e-01
-2.92e-01
-3.58e-01
-3.41e-01
-5.75e-02
-3.63e-01
-3.17e-01
-1.62e-01
-1.93e-01
-3.30e-01
-1.82e-01
-2.74e-01
-2.40e-01
-3.48e-01
-3.37e-01
-3.43e-01
-2.17e-01
-3.11e-01
-2.98e-01
-2.74e-01
-3.74e-01
-3.77e-01
-2.51e-01
-2.73e-01
-3.33e-01
-3.15e-01
-2.55e-01
-3.29e-01
-2.66e-01
-3.28e-01
-2.75e-01
-2.66e-01
-2.86e-01
-3.78e-01
-3.77e-01
-3.47e-01
-2.10e-01
-1.86e-01
-2.01e-01
-3.49e-01
-2.56e-01
-1.60e-01
-2.80e-01
-2.74e-01
-2.70e-01
-8.73e-02
-3.17e-01
-2.99e-01
-2.15e-01
-1.90e-01
-2.95e-01
-2.73e-01
-2.91e-01
-3.74e-01
-2.43e-01
-1.13e-01
-2.58e-01
-3.16e-01
-1.68e-01
-3.02e-01
-2.00e-01
-1.94e-01
-2.31e-01
-3.42e-01
-5.50e-01
-4.10e-01
-1.63e-01
-2.60e-01
-2.71e-01
-2.35e-01
-2.55e-01
-2.49e-01
-3.43e-01
-2.79e-01
-3.78e-01
-2.93e-01
-2.13e-01
-1.21e-01
-3.04e-01
-2.64e-01
-2.95e-01
-3.19e-01
-2.31e-01
-2.98e-01
-3.03e-01
-1.71e-02
-6.49e-02
-2.72e-01
-2.28e-01
-3.41e-01
-2.76e-01
-2.03e-01
-6.64e-02
-1.31e-01
-2.46e-01
-3.72e-01
-3.59e-01
-3.22e-01
-8.46e-02
-2.59e-01
-3.58e-01
-3.50e-01
-3.27e-01
-3.78e-01
-2.53e-01
-2.45e-01
-2.75e-01
-2.82e-01
-3.22e-01
-2.11e-01
-3.01e-01
-2.29e-01
-2.94e-01
-1.26e-01
-3.18e-01
-0.00e+00
-3.46e-01
-2.16e-01
-1.93e-01
-2.85e-01
-2.74e-01
-2.35e-01
-3.01e-01
-3.63e-01
-2.64e-01
-3.07e-01
-2.41e-01
-2.64e-01
-2.30e-01
-2.31e-01
-2.27e-01
-3.04e-01
-3.36e-01
-1.86e-01
-2.57e-01
-4.55e-01
-3.10e-01
-3.23e-01
-3.42e-01
-1.66e-01
-3.14e-01
-3.00e-01
-2.86e-01
-2.70e-01
-3.14e-01
-5.23e-02
-2.38e-01
-2.86e-01
-3.08e-01
-2.34e-01
-1.11e-01
-3.42e-01
-3.33e-01
-2.96e-01
-3.59e-01
-3.68e-01
-4.03e-01
-3.79e-01
-2.89e-01
-2.66e-01
-2.71e-01
-2.19e-01
-3.88e-01
-3.06e-01
-3.38e-01
-1.87e-01
-2.63e-01
-1.13e-01
-2.65e-01
-3.34e-01
-2.80e-01
-1.88e-01
-3.50e-01
-2.54e-01
-2.98e-01
-3.34e-01
-3.31e-01
-3.26e-01
-3.33e-01
-2.85e-01
-2.83e-01
-3.28e-01
-3.16e-01
-3.28e-01
-3.15e-01
-2.24e-01
-2.90e-01
-3.03e-01
-7.41e-02
-3.44e-01
-2.68e-01
-3.11e-01
-3.70e-01
-2.81e-01
-4.23e-01
-3.42e-01
-2.69e-01
-2.92e-01
-2.66e-01
-1.18e-01
-1.39e-01
-3.03e-01
-3.04e-01
-3.08e-01
-3.12e-01
-1.13e-01
-2.15e-01
-2.18e-01
-3.58e-01
-2.59e-01
-2.33e-01
-2.54e-01
-2.84e-01
-1.25e-01
-4.27e-01
-3.03e-02
-3.11e-01
-3.21e-01
-2.68e-01
-3.15e-01
-1.26e-01
-3.29e-01
-3.22e-01
-3.27e-01
-3.86e-01
-3.90e-01
-2.07e-01
-3.69e-01
-2.71e-01
-1.75e-01
-2.17e-01
-2.29e-01
-2.43e-01
-2.68e-01
-3.46e-01
-1.17e-01
-2.12e-01
-2.75e-01
-3.31e-01
-3.41e-01
-1.93e-01
-1.07e-01
-1.94e-01
-3.21e-01
-3.25e-01
-2.67e-01
-3.23e-01
-2.55e-01
-2.30e-01
-3.54e-01
-2.84e-01
-6.69e-01
-3.81e-01
-3.38e-01
-3.17e-01
-2.94e-01
-4.49e-01
-2.24e-01
-3.52e-01
-9.06e-02
-2.83e-01
-2.03e-01
-2.70e-01
-2.73e-01
-1.66e-01
-2.51e-01
-3.20e-01
-2.40e-01
-2.98e-01
-2.16e-01
-2.23e-01
-2.65e-01
-2.88e-01
-2.53e-01
-3.15e-01
-3.59e-01
-2.52e-01
-2.97e-01
-2.49e-01
-3.66e-01
-2.79e-01
-3.44e-01
-3.13e-01
-4.12e-01
-2.00e-01
-3.41e-01
-3.90e-01
-2.89e-01
-3.11e-01
-3.66e-01
-3.09e-01
-1.79e-01
-2.52e-01
-3.16e-01
-3.09e-01
-2.94e-01
-2.87e-01
-3.40e-01
-1.65e-01
-0.00e+00
-2.83e-01
-2.80e-01
-2.76e-01
-3.62e-01
-2.82e-01
-2.79e-01
-8.71e-02
-1.98e-01
-2.35e-01
-3.09e-01
-8.05e-02
-1.66e-01
-3.48e-01
-3.12e-01
-2.50e-01
-4.08e-01
-2.74e-01
-3.61e-01
-2.99e-01
-2.51e-01
-2.94e-01
-3.56e-01
-3.13e-01
-2.47e-01
-3.39e-01
-3.17e-01
-3.01e-01
-3.41e-01
-3.48e-01
-3.55e-01
-3.06e-01
-2.56e-01
-3.60e-01
-3.35e-01
-3.14e-01
-2.81e-01
-2.85e-01
-2.01e-01
-1.64e-01
-2.10e-01
-2.71e-01
-2.36e-01
-2.98e-01
-2.34e-01
-3.51e-01
-7.82e-02
-3.49e-01
-1.74e-01
-2.67e-01
-2.87e-01
-3.60e-01
-1.31e-01
-2.81e-01
-3.38e-01
-2.79e-01
-2.13e-01
-3.40e-01
-2.12e-01
-3.50e-01
-5.68e-02
-2.18e-01
-3.08e-01
-1.54e-01
-2.90e-01
-3.58e-01
-2.66e-01
-3.07e-01
-2.34e-01
-3.42e-01
-2.87e-01
-3.23e-01
-3.52e-01
-2.90e-01
-3.44e-01
-2.27e-01
-1.57e-01
-3.43e-01
-3.51e-01
-3.38e-01
-3.88e-01
-1.69e-01
-1.58e-01
-3.36e-01
-3.84e-01
-3.15e-01
-2.49e-01
-2.65e-01
-2.70e-01
-3.26e-01
-8.51e-02
-2.83e-01
-3.10e-01
-3.58e-01
-2.51e-01
-1.60e-01
-2.66e-01
-2.42e-01
-2.81e-01
-3.65e-01
-2.61e-01
-3.03e-01
-4.86e-01
-2.92e-01
-3.40e-01
-1.53e-01
-3.34e-01
-2.94e-01
-2.71e-01
-3.21e-01
-2.62e-01
-3.11e-01
-2.66e-01
-4.02e-01
-2.35e-01
-2.79e-01
-4.43e-01
-2.74e-01
-4.45e-01
-3.86e-01
-1.40e-01
-9.38e-02
-2.26e-01
-3.06e-01
-3.19e-01
-2.38e-01
-2.62e-01
-2.49e-01
-2.60e-01
-3.31e-01
-3.10e-01
+3.26e-01
+3.34e-01
+2.79e-01
+2.53e-01
+3.03e-01
+4.14e-01
+3.63e-01
+3.02e-01
+3.23e-01
+3.24e-01
+2.37e-01
+2.53e-01
+1.38e-01
+3.48e-01
+2.79e-01
+2.76e-01
+3.13e-01
+2.41e-01
+3.23e-01
+1.75e-01
+3.14e-01
+2.99e-01
+2.57e-01
+3.26e-01
+2.11e-01
+3.00e-01
+2.15e-01
+1.13e-01
+3.50e-01
+1.85e-01
+2.38e-01
+1.81e-01
+3.03e-01
+2.17e-01
+2.77e-01
+3.58e-01
+3.48e-01
+3.56e-01
+2.41e-01
+3.72e-01
+1.55e-01
+3.75e-01
+1.73e-01
+2.79e-01
+1.71e-01
+1.51e-01
+2.84e-01
+3.87e-01
+3.81e-01
+2.81e-01
+2.61e-01
+2.81e-01
+3.21e-01
+3.47e-01
+3.05e-01
+1.90e-01
+3.12e-01
+2.45e-01
+2.82e-01
+2.84e-01
+2.36e-01
+5.22e-01
+3.85e-01
+2.09e-01
+3.84e-01
+3.01e-01
+2.85e-01
+3.11e-01
+3.02e-01
+3.26e-01
+1.74e-01
+1.93e-01
+2.73e-01
+2.61e-01
+1.13e-01
+3.25e-01
+2.85e-01
+3.08e-01
+1.99e-01
+2.11e-01
+3.16e-01
+2.48e-01
+2.71e-01
+3.21e-01
+3.78e-01
+2.99e-01
+2.66e-01
+2.81e-01
+1.40e-01
+9.32e-02
+1.90e-01
+2.80e-01
+3.51e-01
+4.15e-01
+2.34e-01
+2.47e-01
+2.05e-01
+3.48e-01
+1.91e-01
+1.65e-01
+1.60e-01
+2.10e-01
+1.42e-01
+2.68e-01
+2.87e-01
+2.34e-01
+3.15e-01
+2.39e-01
+1.65e-01
+3.25e-01
+3.38e-01
+3.47e-01
+3.39e-01
+3.64e-01
+2.97e-01
+2.96e-01
+2.93e-01
+3.75e-01
+2.07e-01
+2.42e-01
+2.89e-01
+3.55e-01
+3.69e-01
+1.77e-01
+2.58e-01
+3.56e-01
+2.66e-01
+1.97e-01
+2.34e-01
+3.01e-01
+1.91e-01
+2.65e-01
+8.72e-02
+1.39e-01
+2.39e-01
+3.00e-01
+2.63e-01
+2.10e-02
+3.60e-01
+2.89e-01
+2.32e-01
+2.50e-01
+1.83e-01
+3.79e-01
+3.64e-01
+3.35e-01
+3.21e-01
+1.69e-01
+2.36e-01
+3.76e-01
+2.40e-01
+3.78e-01
+1.09e-01
+2.58e-01
+1.71e-01
+3.05e-01
+2.15e-01
+9.89e-02
+1.81e-01
+1.40e-01
+2.45e-01
+3.25e-01
+2.78e-01
+3.16e-01
+2.44e-01
+3.45e-01
+2.45e-01
+1.38e-01
+1.81e-01
+1.85e-01
+3.20e-01
+3.92e-01
+3.34e-01
+2.60e-01
+2.48e-01
+3.59e-01
+1.05e-01
+3.45e-01
+2.32e-01
+2.44e-01
+3.20e-01
+2.98e-01
+2.38e-01
+2.77e-01
+2.89e-01
+3.11e-01
+1.60e-01
+2.28e-01
+3.26e-01
+2.38e-01
+2.85e-01
+2.79e-01
+2.73e-01
+2.44e-01
+3.43e-01
+3.37e-01
+4.64e-01
+3.15e-01
+1.53e-01
+3.46e-01
+1.99e-01
+3.15e-01
+3.21e-01
+1.81e-01
+3.75e-02
+2.78e-01
+2.43e-01
+1.17e-01
+2.83e-01
+2.69e-01
+1.95e-01
+3.37e-01
+2.88e-01
+2.72e-01
+3.10e-01
+2.13e-01
+3.23e-01
+2.38e-01
+3.03e-01
+3.16e-01
+2.36e-01
+9.04e-02
+3.54e-01
+3.42e-01
+2.56e-01
+3.69e-01
+3.40e-01
+3.62e-01
+3.57e-01
+2.09e-01
+3.17e-01
+2.35e-01
+3.64e-01
+3.85e-01
+1.27e-01
+3.09e-01
+3.14e-01
+2.64e-01
+2.53e-01
+2.99e-01
+2.90e-01
+2.18e-01
+3.09e-01
+3.32e-01
+3.17e-01
+3.72e-01
+3.27e-01
+2.94e-01
+2.69e-01
+3.21e-01
+2.32e-01
+3.43e-01
+2.82e-01
+2.72e-01
+3.37e-01
+2.75e-01
+3.21e-01
+2.82e-01
+2.93e-01
+2.89e-01
+2.42e-01
+3.33e-01
+4.03e-01
+3.74e-01
+3.32e-01
+2.81e-01
+2.91e-01
+3.21e-01
+3.12e-01
+3.09e-01
+3.17e-01
+2.06e-01
+3.89e-01
+2.33e-01
+8.41e-02
+2.35e-01
+2.90e-01
+3.94e-01
+2.81e-01
+2.93e-01
+3.08e-01
+2.15e-01
+3.33e-01
+3.20e-01
+1.35e-01
+1.50e-01
+3.11e-01
+2.75e-01
+9.93e-02
+2.78e-01
+2.72e-01
+3.18e-01
+1.22e-01
+3.93e-01
+2.89e-01
+3.35e-01
+2.41e-01
+3.69e-01
+3.37e-01
+2.24e-01
+2.61e-01
+4.00e-01
+3.24e-01
+2.87e-01
+2.22e-01
+3.54e-01
+3.59e-01
+3.99e-01
+1.18e-01
+3.42e-01
+2.92e-01
+2.90e-01
+1.71e-01
+3.78e-01
+4.08e-01
+1.24e-01
+3.23e-01
+3.51e-01
+2.66e-01
+2.66e-01
+2.68e-01
+3.67e-01
+3.14e-01
+3.59e-01
+2.23e-01
+3.17e-01
+4.18e-01
+2.51e-01
+3.01e-01
+3.27e-01
+4.62e-01
+3.08e-01
+3.15e-01
+2.97e-01
+3.26e-01
+3.14e-01
+3.45e-01
+3.52e-01
+3.43e-01
+2.22e-01
+3.68e-01
+2.37e-02
+3.80e-01
+3.14e-01
+2.22e-01
+4.05e-01
+2.23e-01
+4.65e-01
+3.26e-01
+2.46e-01
+2.58e-01
+2.32e-01
+2.22e-01
+3.33e-01
+2.12e-01
+3.22e-01
+3.40e-01
+3.22e-01
+2.72e-01
+3.75e-01
+2.42e-01
+2.57e-01
+2.48e-01
+3.78e-01
+2.94e-01
+1.72e-01
+2.67e-01
+3.59e-01
+3.33e-01
+3.14e-01
+3.46e-01
+2.55e-01
+1.74e-01
+2.26e-01
+2.83e-01
+2.94e-01
+2.65e-01
+4.07e-01
+3.49e-01
+1.70e-01
+3.70e-01
+2.94e-01
+3.24e-01
+3.58e-01
+3.39e-01
+3.35e-01
+3.93e-01
+3.74e-01
+2.33e-01
+3.54e-01
+2.59e-01
+3.33e-01
+2.92e-01
+3.16e-01
+1.37e-01
+2.86e-01
+1.33e-01
+2.36e-01
+3.91e-01
+2.51e-01
+2.80e-01
+2.12e-01
+3.36e-01
+3.09e-01
+2.31e-01
+2.36e-01
+3.25e-01
+3.30e-01
+3.29e-01
+2.59e-01
+1.95e-01
+2.14e-01
+2.13e-01
+3.35e-01
+3.39e-01
+8.68e-02
+3.41e-01
+3.92e-01
+3.06e-01
+3.27e-01
+3.26e-01
+2.34e-01
+3.19e-01
+2.40e-01
+3.07e-01
+1.76e-01
+3.05e-01
+2.70e-01
+2.79e-01
+2.16e-01
+3.23e-01
+3.07e-01
+3.43e-01
+3.60e-01
+2.79e-01
+3.45e-01
+2.75e-01
+3.23e-01
+2.88e-01
+3.67e-01
+3.23e-01
+4.63e-01
+3.57e-01
+3.39e-01
+1.88e-01
+3.29e-01
+3.72e-01
+2.31e-01
+3.63e-01
+2.26e-01
+3.43e-01
+2.60e-01
+2.69e-01
+3.33e-01
+3.35e-01
+2.18e-01
+2.58e-01
+3.73e-01
+2.18e-01
+1.23e-01
+4.04e-01
+2.80e-01
+3.30e-01
+1.55e-01
+2.31e-01
+3.85e-01
+3.95e-01
+3.30e-01
+2.04e-01
+3.61e-01
+2.91e-01
+2.72e-01
+2.32e-01
+3.25e-01
+3.22e-01
+1.47e-01
+1.81e-01
+1.85e-01
+2.53e-01
+3.07e-01
+3.57e-01
+3.14e-01
+3.52e-01
+3.03e-01
+3.11e-01
+3.16e-01
+2.30e-01
+2.11e-01
+3.22e-01
+3.13e-01
+2.02e-01
+2.90e-01
+1.94e-01
+2.59e-01
+2.98e-01
+2.61e-01
+3.34e-01
+3.18e-01
+2.85e-01
+3.56e-01
+2.52e-01
+3.17e-01
+3.94e-01
+2.84e-01
+3.16e-01
+2.37e-01
+3.00e-01
+2.79e-01
+1.94e-01
+3.10e-01
+3.17e-01
+3.40e-01
+1.88e-01
+1.73e-01
+2.73e-01
+3.50e-01
+3.54e-01
+2.61e-01
+4.11e-01
+3.70e-01
+3.78e-01
+2.61e-01
+1.56e-01
+3.31e-01
+2.33e-01
+1.54e-01
+3.90e-01
+3.04e-01
+3.19e-01
+3.05e-01
+1.46e-01
+2.82e-01
+3.29e-01
+2.86e-01
+2.97e-01
+2.49e-01
+3.14e-01
+3.77e-01
+3.22e-01
+2.15e-01
+3.51e-01
+3.29e-01
+3.28e-01
+2.88e-01
+1.19e-01
+3.07e-01
+2.24e-01
+2.83e-01
+3.03e-01
+2.87e-01
+1.65e-01
+2.27e-01
+2.79e-01
+2.88e-01
+2.95e-01
+2.38e-01
+3.28e-01
+3.16e-01
+2.43e-01
+3.03e-01
+3.72e-01
+3.56e-01
+2.74e-01
+3.01e-01
+2.42e-01
+3.09e-01
+2.63e-01
+3.07e-01
+1.79e-01
+2.83e-01
+2.31e-01
+2.05e-01
+2.91e-01
+9.57e-02
+2.79e-01
+3.15e-01
+9.75e-03
+3.20e-01
+2.44e-01
+4.15e-01
+1.67e-01
+3.17e-01
+3.22e-01
+3.39e-01
+3.28e-01
+2.79e-01
+2.75e-01
+2.90e-01
+2.19e-01
+2.28e-01
+2.43e-01
+3.09e-01
+3.11e-01
+1.95e-01
+1.60e-01
+4.60e-01
+2.05e-01
+2.02e-01
+3.26e-01
+3.21e-01
+3.58e-01
+3.97e-01
+3.17e-01
+1.18e-01
+4.67e-01
+6.97e-02
+2.60e-01
+3.36e-01
+2.62e-01
+3.49e-01
+1.04e-01
+2.97e-01
+2.78e-01
+2.52e-01
+2.04e-01
+1.62e-01
+2.78e-01
+3.45e-01
+3.58e-01
+3.42e-01
+2.92e-01
+3.14e-01
+3.67e-01
+3.41e-01
+3.03e-01
+1.74e-01
+2.69e-01
+2.83e-01
+2.54e-01
+3.76e-01
+1.75e-01
+2.71e-01
+3.72e-01
+3.35e-01
+3.00e-01
+2.45e-01
+2.67e-01
+2.41e-01
+1.99e-01
+2.89e-01
+2.76e-01
+3.04e-01
+3.42e-01
+1.36e-01
+3.73e-01
+2.15e-01
+2.51e-01
+1.60e-01
+3.47e-01
+1.69e-01
+3.85e-01
+2.89e-01
+2.00e-01
+1.98e-01
+3.31e-01
+2.74e-01
+2.86e-01
+3.98e-01
+1.45e-01
+3.03e-01
+3.53e-01
+3.30e-01
+1.79e-01
+1.87e-01
+3.20e-01
+4.28e-02
+2.41e-01
+2.22e-01
+3.04e-01
+2.96e-01
+3.35e-01
+2.71e-01
+3.40e-01
+2.49e-01
+3.41e-01
+3.35e-01
+4.82e-01
+2.24e-01
+3.39e-01
+3.02e-01
+2.80e-01
+1.54e-01
+2.93e-01
+2.62e-01
+2.66e-01
+5.38e-02
+2.92e-01
+2.29e-01
+2.52e-01
+2.58e-01
+2.66e-01
+2.92e-01
+2.71e-01
+3.12e-01
+1.27e-01
+3.27e-01
+1.77e-01
+1.72e-01
+2.96e-01
+2.67e-01
+3.20e-01
+3.49e-01
+3.14e-01
+2.92e-01
+3.58e-01
+3.41e-01
+5.75e-02
+3.63e-01
+3.17e-01
+1.62e-01
+1.93e-01
+3.30e-01
+1.82e-01
+2.74e-01
+2.40e-01
+3.48e-01
+3.37e-01
+3.43e-01
+2.17e-01
+3.11e-01
+2.98e-01
+2.74e-01
+3.74e-01
+3.77e-01
+2.51e-01
+2.73e-01
+3.33e-01
+3.15e-01
+2.55e-01
+3.29e-01
+2.66e-01
+3.28e-01
+2.75e-01
+2.66e-01
+2.86e-01
+3.78e-01
+3.77e-01
+3.47e-01
+2.10e-01
+1.86e-01
+2.01e-01
+3.49e-01
+2.56e-01
+1.60e-01
+2.80e-01
+2.74e-01
+2.70e-01
+8.73e-02
+3.17e-01
+2.99e-01
+2.15e-01
+1.90e-01
+2.95e-01
+2.73e-01
+2.91e-01
+3.74e-01
+2.43e-01
+1.13e-01
+2.58e-01
+3.16e-01
+1.68e-01
+3.02e-01
+2.00e-01
+1.94e-01
+2.31e-01
+3.42e-01
+5.50e-01
+4.10e-01
+1.63e-01
+2.60e-01
+2.71e-01
+2.35e-01
+2.55e-01
+2.49e-01
+3.43e-01
+2.79e-01
+3.78e-01
+2.93e-01
+2.13e-01
+1.21e-01
+3.04e-01
+2.64e-01
+2.95e-01
+3.19e-01
+2.31e-01
+2.98e-01
+3.03e-01
+1.71e-02
+6.49e-02
+2.72e-01
+2.28e-01
+3.41e-01
+2.76e-01
+2.03e-01
+6.64e-02
+1.31e-01
+2.46e-01
+3.72e-01
+3.59e-01
+3.22e-01
+8.46e-02
+2.59e-01
+3.58e-01
+3.50e-01
+3.27e-01
+3.78e-01
+2.53e-01
+2.45e-01
+2.75e-01
+2.82e-01
+3.22e-01
+2.11e-01
+3.01e-01
+2.29e-01
+2.94e-01
+1.26e-01
+3.18e-01
+0.00e+00
+3.46e-01
+2.16e-01
+1.93e-01
+2.85e-01
+2.74e-01
+2.35e-01
+3.01e-01
+3.63e-01
+2.64e-01
+3.07e-01
+2.41e-01
+2.64e-01
+2.30e-01
+2.31e-01
+2.27e-01
+3.04e-01
+3.36e-01
+1.86e-01
+2.57e-01
+4.55e-01
+3.10e-01
+3.23e-01
+3.42e-01
+1.66e-01
+3.14e-01
+3.00e-01
+2.86e-01
+2.70e-01
+3.14e-01
+5.23e-02
+2.38e-01
+2.86e-01
+3.08e-01
+2.34e-01
+1.11e-01
+3.42e-01
+3.33e-01
+2.96e-01
+3.59e-01
+3.68e-01
+4.03e-01
+3.79e-01
+2.89e-01
+2.66e-01
+2.71e-01
+2.19e-01
+3.88e-01
+3.06e-01
+3.38e-01
+1.87e-01
+2.63e-01
+1.13e-01
+2.65e-01
+3.34e-01
+2.80e-01
+1.88e-01
+3.50e-01
+2.54e-01
+2.98e-01
+3.34e-01
+3.31e-01
+3.26e-01
+3.33e-01
+2.85e-01
+2.83e-01
+3.28e-01
+3.16e-01
+3.28e-01
+3.15e-01
+2.24e-01
+2.90e-01
+3.03e-01
+7.41e-02
+3.44e-01
+2.68e-01
+3.11e-01
+3.70e-01
+2.81e-01
+4.23e-01
+3.42e-01
+2.69e-01
+2.92e-01
+2.66e-01
+1.18e-01
+1.39e-01
+3.03e-01
+3.04e-01
+3.08e-01
+3.12e-01
+1.13e-01
+2.15e-01
+2.18e-01
+3.58e-01
+2.59e-01
+2.33e-01
+2.54e-01
+2.84e-01
+1.25e-01
+4.27e-01
+3.03e-02
+3.11e-01
+3.21e-01
+2.68e-01
+3.15e-01
+1.26e-01
+3.29e-01
+3.22e-01
+3.27e-01
+3.86e-01
+3.90e-01
+2.07e-01
+3.69e-01
+2.71e-01
+1.75e-01
+2.17e-01
+2.29e-01
+2.43e-01
+2.68e-01
+3.46e-01
+1.17e-01
+2.12e-01
+2.75e-01
+3.31e-01
+3.41e-01
+1.93e-01
+1.07e-01
+1.94e-01
+3.21e-01
+3.25e-01
+2.67e-01
+3.23e-01
+2.55e-01
+2.30e-01
+3.54e-01
+2.84e-01
+6.69e-01
+3.81e-01
+3.38e-01
+3.17e-01
+2.94e-01
+4.49e-01
+2.24e-01
+3.52e-01
+9.06e-02
+2.83e-01
+2.03e-01
+2.70e-01
+2.73e-01
+1.66e-01
+2.51e-01
+3.20e-01
+2.40e-01
+2.98e-01
+2.16e-01
+2.23e-01
+2.65e-01
+2.88e-01
+2.53e-01
+3.15e-01
+3.59e-01
+2.52e-01
+2.97e-01
+2.49e-01
+3.66e-01
+2.79e-01
+3.44e-01
+3.13e-01
+4.12e-01
+2.00e-01
+3.41e-01
+3.90e-01
+2.89e-01
+3.11e-01
+3.66e-01
+3.09e-01
+1.79e-01
+2.52e-01
+3.16e-01
+3.09e-01
+2.94e-01
+2.87e-01
+3.40e-01
+1.65e-01
+0.00e+00
+2.83e-01
+2.80e-01
+2.76e-01
+3.62e-01
+2.82e-01
+2.79e-01
+8.71e-02
+1.98e-01
+2.35e-01
+3.09e-01
+8.05e-02
+1.66e-01
+3.48e-01
+3.12e-01
+2.50e-01
+4.08e-01
+2.74e-01
+3.61e-01
+2.99e-01
+2.51e-01
+2.94e-01
+3.56e-01
+3.13e-01
+2.47e-01
+3.39e-01
+3.17e-01
+3.01e-01
+3.41e-01
+3.48e-01
+3.55e-01
+3.06e-01
+2.56e-01
+3.60e-01
+3.35e-01
+3.14e-01
+2.81e-01
+2.85e-01
+2.01e-01
+1.64e-01
+2.10e-01
+2.71e-01
+2.36e-01
+2.98e-01
+2.34e-01
+3.51e-01
+7.82e-02
+3.49e-01
+1.74e-01
+2.67e-01
+2.87e-01
+3.60e-01
+1.31e-01
+2.81e-01
+3.38e-01
+2.79e-01
+2.13e-01
+3.40e-01
+2.12e-01
+3.50e-01
+5.68e-02
+2.18e-01
+3.08e-01
+1.54e-01
+2.90e-01
+3.58e-01
+2.66e-01
+3.07e-01
+2.34e-01
+3.42e-01
+2.87e-01
+3.23e-01
+3.52e-01
+2.90e-01
+3.44e-01
+2.27e-01
+1.57e-01
+3.43e-01
+3.51e-01
+3.38e-01
+3.88e-01
+1.69e-01
+1.58e-01
+3.36e-01
+3.84e-01
+3.15e-01
+2.49e-01
+2.65e-01
+2.70e-01
+3.26e-01
+8.51e-02
+2.83e-01
+3.10e-01
+3.58e-01
+2.51e-01
+1.60e-01
+2.66e-01
+2.42e-01
+2.81e-01
+3.65e-01
+2.61e-01
+3.03e-01
+4.86e-01
+2.92e-01
+3.40e-01
+1.53e-01
+3.34e-01
+2.94e-01
+2.71e-01
+3.21e-01
+2.62e-01
+3.11e-01
+2.66e-01
+4.02e-01
+2.35e-01
+2.79e-01
+4.43e-01
+2.74e-01
+4.45e-01
+3.86e-01
+1.40e-01
+9.38e-02
+2.26e-01
+3.06e-01
+3.19e-01
+2.38e-01
+2.62e-01
+2.49e-01
+2.60e-01
+3.31e-01
+3.10e-01
```

### Comparing `nanite-3.5.4/nanite/rate/ts_zef18/train_feat_con_idt_sum.txt` & `nanite-3.6.0/nanite/rate/ts_zef18/train_feat_con_idt_sum_75perc.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,1132 +1,1132 @@
-2.29e-01
-1.66e-01
-1.88e-01
-3.67e-01
-5.73e-01
-1.79e-01
-1.21e-01
-1.97e-01
-3.24e-01
-2.28e-01
-2.34e-01
-2.95e-01
-2.82e-01
-1.49e-01
-3.09e-01
-2.32e-01
-3.15e-01
-1.36e-01
-1.99e-01
-4.31e-01
-5.37e-01
-1.73e-01
-4.07e-01
-1.97e-01
-6.63e-02
-1.42e-01
-2.21e-01
-3.84e-01
-3.39e-01
-2.45e-01
-1.48e-01
-2.73e-01
-3.51e-01
-4.74e-01
-3.39e-01
-3.49e-01
-3.69e-01
-3.82e-01
-2.96e-01
-1.68e-01
-4.51e-01
-1.56e-01
-2.62e-01
-2.87e-01
-1.97e-01
-1.20e-01
-4.86e-01
-1.53e-01
-2.43e-01
-2.08e-01
-1.75e-01
-5.19e-01
-2.64e-01
-2.14e-01
-1.52e-01
-3.23e-01
-2.01e-01
-3.15e-01
-2.84e-01
-1.99e-01
-2.45e-01
-8.53e-01
-1.29e-01
-1.79e-01
-2.04e-01
-2.31e-01
-2.62e-01
-2.53e-01
-2.59e-01
-2.46e-01
-3.68e-01
-4.93e-01
-3.71e-01
-1.38e-01
-2.55e-01
-1.89e-01
-2.46e-01
-4.57e-01
-2.13e-01
-3.12e-01
-2.68e-01
-1.80e-01
-3.09e-01
-2.26e-01
-2.39e-01
-2.76e-01
-1.57e-01
-2.50e-01
-3.84e-01
-2.73e-01
-4.05e-01
-1.97e-01
-3.72e-01
-5.59e-02
-3.80e-01
-2.25e-01
-2.77e-01
-2.70e-01
-3.04e-01
-4.43e-01
-1.45e-01
-4.29e-01
-2.28e-01
-2.79e-01
-4.35e-01
-2.43e-01
-3.34e-01
-3.32e-01
-2.84e-01
-1.39e-01
-2.02e-01
-3.06e-01
-1.64e-01
-1.27e-01
-3.87e-01
-2.24e-01
-2.11e-01
-2.63e-01
-2.87e-01
-3.06e-01
-2.77e-01
-2.41e-01
-2.13e-01
-2.41e-01
-2.92e-01
-3.07e-01
-1.73e-01
-2.53e-01
-2.65e-01
-6.31e-01
-3.50e-01
-4.63e-01
-7.29e-01
-5.36e-01
-3.02e-01
-7.21e-02
-3.60e-01
-3.22e-01
-1.45e-01
-2.69e-01
-4.41e-01
-3.38e-01
-2.65e-01
-1.77e-01
-2.39e-01
-3.12e-01
-1.14e-01
-3.16e-01
-1.79e-01
-1.63e-01
-4.64e-01
-5.36e-02
-4.66e-01
-4.22e-01
-3.91e-01
-2.68e-01
-2.61e-01
-3.59e-01
-4.29e-01
-2.58e-01
-2.88e-01
-1.50e-01
-2.16e-01
-3.01e-01
-3.57e-01
-3.12e-01
-2.84e-01
-4.08e-01
-4.38e-01
-2.24e-01
-1.60e-01
-7.17e-02
-1.88e-01
-1.51e-01
-2.75e-01
-2.23e-01
-1.33e-01
-1.05e-01
-2.53e-01
-1.97e-01
-1.47e-01
-1.81e-01
-3.19e-01
-5.15e-01
-8.34e-02
-2.04e-01
-3.10e-01
-2.92e-01
-3.19e-01
-2.80e-01
-2.68e-01
-9.80e-02
-1.77e-01
-8.14e-02
-5.32e-01
-1.21e-01
-4.41e-01
-1.48e-01
-6.62e-01
-1.76e-01
-2.48e-01
-2.40e-01
-1.69e-01
-1.63e-01
-1.69e-01
-1.97e-01
-1.82e-01
-3.55e-01
-2.26e-01
-3.26e-01
-1.48e-01
-1.08e-01
-9.92e-02
-4.32e-01
-3.38e-01
-3.05e-01
-2.41e-01
-3.08e-01
-2.71e-01
-4.90e-01
-1.38e-01
-2.55e-01
-2.56e-01
-2.37e-01
-1.85e-01
-4.39e-01
-1.38e-01
-4.53e-02
-4.30e-02
-3.86e-01
-1.65e-01
-1.03e-01
-2.67e-01
-1.71e-01
-2.66e-01
-2.50e-01
-2.71e-01
-1.15e-01
-4.77e-01
-4.49e-01
-2.38e-01
-2.41e-01
-2.19e-01
-4.46e-01
-2.55e-01
-1.60e-01
-1.43e-01
-3.74e-01
-3.03e-01
-2.29e-01
-2.24e-01
-1.68e-01
-2.23e-01
-1.37e-01
-3.99e-01
-2.52e-01
-3.51e-01
-3.83e-01
-1.62e-01
-1.81e-01
-3.14e-01
-4.41e-01
-3.66e-01
-2.20e-01
-4.15e-01
-1.67e-01
-1.74e-01
-2.05e-01
-1.86e-01
-2.51e-01
-3.90e-01
-1.71e-01
-5.03e-01
-2.70e-01
-3.73e-01
-3.26e-01
-1.48e-01
-1.56e-01
-4.31e-01
-2.21e-01
-2.83e-01
-3.80e-01
-3.73e-01
-7.73e-01
-2.98e-01
-2.59e-01
-2.23e-01
-2.41e-01
-4.06e-01
-1.47e-01
-5.56e-01
-2.03e-01
-2.43e-01
-3.08e-01
-1.67e-01
-1.46e-01
-1.84e-01
-2.23e-01
-1.87e-01
-1.90e-01
-2.75e-01
-3.19e-01
-6.64e-01
-2.68e-01
-4.03e-01
-1.38e-01
-2.57e-01
-3.21e-01
-5.70e-01
-3.24e-01
-4.27e-01
-1.86e-01
-1.52e-01
-9.80e-02
-2.24e-01
-4.34e-01
-2.95e-01
-9.76e-02
-2.16e-01
-1.62e-01
-3.25e-01
-1.66e-01
-2.33e-01
-1.34e-01
-2.86e-01
-2.30e-01
-3.24e-01
-3.18e-01
-4.11e-01
-5.16e-01
-3.29e-01
-4.35e-01
-1.95e-01
-1.66e-01
-1.20e-01
-2.02e-01
-1.24e-01
-1.65e-01
-2.11e-01
-4.50e-01
-2.36e-01
-4.32e-01
-2.32e-01
-3.01e-01
-3.96e-01
-1.75e-01
-1.52e-01
-2.59e-01
-2.74e-01
-2.43e-01
-1.77e-01
-1.76e-01
-2.16e-01
-2.63e-01
-3.23e-01
-2.09e-01
-1.65e-01
-5.43e-01
-2.09e-01
-2.24e-01
-5.71e-01
-1.58e-01
-2.01e-01
-1.63e-01
-2.95e-01
-5.32e-01
-1.68e-01
-1.62e-01
-2.19e-01
-5.85e-02
-2.73e-01
-2.48e-01
-2.84e-01
-3.04e-01
-1.54e-01
-1.77e-01
-1.46e-01
-1.82e-01
-4.76e-01
-7.70e-01
-1.35e-01
-1.90e-01
-2.98e-01
-4.01e-01
-5.86e-01
-2.69e-01
-1.87e-01
-2.97e-01
-1.93e-01
-1.98e-01
-2.58e-01
-2.66e-01
-1.88e-01
-2.39e-01
-4.31e-01
-2.05e-01
-2.87e-01
-2.81e-01
-1.40e-01
-8.27e-01
-3.46e-01
-2.26e-01
-3.76e-01
-2.25e-01
-2.02e-01
-4.39e-01
-3.53e-01
-1.33e-01
-3.31e-01
-3.75e-01
-2.18e-01
-3.48e-01
-1.06e-01
-1.96e-01
-1.47e-01
-2.38e-01
-3.93e-01
-2.31e-01
-7.69e-02
-1.40e-01
-3.59e-01
-4.51e-01
-2.06e-01
-1.55e-01
-2.41e-01
-1.26e-01
-1.22e-01
-1.83e-01
-2.18e-01
-3.83e-01
-1.75e-01
-3.17e-01
-2.74e-01
-2.55e-01
-3.26e-01
-2.80e-01
-8.78e-02
-1.84e-01
-3.60e-01
-1.17e-01
-3.02e-01
-4.77e-01
-2.12e-01
-3.60e-01
-3.16e-01
-4.86e-01
-2.93e-01
-4.31e-01
-2.62e-01
-3.40e-01
-1.15e-01
-4.63e-01
-1.44e-01
-3.27e-01
-1.82e-01
-2.55e-01
-2.89e-01
-1.74e-01
-1.13e-01
-2.03e-01
-2.90e-01
-1.46e-01
-3.65e-01
-2.90e-01
-3.52e-01
-5.16e-01
-5.97e-02
-3.11e-01
-3.18e-01
-2.93e-01
-2.18e-01
-3.18e-01
-8.87e-02
-1.93e-01
-1.42e-01
-3.78e-01
-2.22e-01
-1.73e-01
-3.21e-01
-1.80e-01
-2.16e-01
-1.25e-01
-6.96e-01
-2.88e-01
-6.41e-01
-4.46e-01
-2.84e-01
-3.44e-01
-1.34e-01
-3.34e-01
-2.42e-01
-3.21e-01
-3.11e-01
-3.41e-01
-2.77e-01
-3.16e-01
-1.12e-01
-3.27e-01
-2.32e-01
-2.16e-01
-5.44e-01
-3.64e-01
-2.89e-01
-2.21e-01
-1.24e-01
-1.20e-01
-3.91e-01
-8.07e-02
-4.46e-01
-1.70e-01
-4.65e-01
-1.92e-01
-1.97e-01
-1.88e-01
-2.24e-01
-2.74e-01
-7.96e-02
-3.19e-01
-4.13e-01
-5.12e-02
-2.31e-01
-3.28e-01
-3.69e-01
-2.00e-01
-1.13e-01
-1.44e-01
-1.67e-01
-3.66e-01
-2.25e-01
-2.03e-01
-2.01e-01
-3.32e-01
-2.15e-01
-2.82e-01
-3.85e-01
-3.10e-01
-3.15e-01
-1.52e-01
-2.03e-01
-2.80e-01
-2.80e-01
-2.75e-01
-9.87e-02
-3.01e-01
-1.53e-01
-1.92e-01
-2.82e-01
-3.07e-01
-2.84e-01
-2.11e-01
-3.65e-01
-1.31e-01
-2.89e-01
-2.43e-01
-3.68e-01
-1.43e-01
-1.94e-01
-1.76e-01
-4.08e-01
-8.83e-02
-3.51e-01
-1.84e-01
-3.36e-01
-4.93e-01
-2.64e-01
-3.80e-01
-2.40e-01
-1.15e-01
-3.27e-01
-2.69e-01
-4.23e-01
-1.54e-01
-2.85e-01
-4.30e-01
-1.08e-01
-5.98e-01
-2.27e-01
-2.20e-01
-1.84e-01
-3.37e-01
-2.63e-01
-1.26e-01
-2.41e-01
-2.49e-01
-2.39e-01
-2.21e-01
-3.09e-01
-2.66e-01
-1.77e-01
-2.71e-01
-2.41e-01
-1.30e-01
-2.05e-01
-1.95e-01
-1.35e-01
-2.18e-01
-2.74e-01
-3.36e-01
-3.76e-01
-2.46e-01
-1.89e-01
-3.69e-01
-3.65e-01
-2.27e-01
-2.98e-01
-4.17e-01
-2.13e-01
-2.39e-01
-2.74e-01
-3.03e-01
-2.72e-01
-8.06e-02
-3.21e-01
-3.61e-01
-2.50e-01
-2.86e-01
-3.73e-01
-1.65e-01
-2.74e-01
-1.78e-01
-2.32e-01
-1.66e-01
-1.45e-01
-3.19e-01
-2.11e-01
-5.09e-01
-3.24e-01
-2.64e-01
-3.81e-01
-2.27e-01
-1.92e-01
-3.87e-01
-2.81e-01
-1.43e-01
-2.45e-01
-3.58e-01
-2.83e-01
-2.37e-01
-2.20e-01
-1.47e-01
-9.53e-02
-2.68e-01
-2.99e-01
-2.04e-01
-3.04e-01
-4.30e-01
-1.97e-01
-1.33e-01
-3.09e-01
-3.81e-01
-3.92e-01
-2.73e-01
-2.08e-01
-2.19e-01
-2.55e-01
-2.71e-01
-1.96e-01
-1.70e-01
-7.35e-01
-4.40e-01
-1.67e-01
-2.01e-01
-4.83e-01
-2.47e-01
-2.00e-01
-1.91e-01
-2.00e-01
-8.27e-02
-3.16e-01
-5.10e-01
-2.55e-01
-1.83e-01
-2.67e-01
-6.67e-01
-3.42e-01
-2.59e-01
-1.91e-01
-3.57e-01
-2.63e-01
-2.63e-01
-1.88e-01
-1.71e-01
-1.77e-01
-3.82e-01
-4.05e-01
-1.70e-01
-3.00e-01
-1.13e-01
-1.67e-01
-3.01e-01
-1.94e-01
-2.86e-01
-2.39e-01
-1.89e-01
-2.59e-01
-5.58e-01
-2.88e-01
-2.30e-01
-1.53e-01
-2.44e-01
-2.45e-01
-2.21e-01
-3.65e-01
-1.96e-01
-1.85e-01
-1.55e-01
-2.26e-01
-3.55e-01
-2.52e-01
-4.21e-01
-2.08e-01
-2.06e-01
-2.40e-01
-3.06e-01
-4.28e-01
-2.57e-01
-2.35e-01
-4.13e-01
-2.55e-01
-3.53e-01
-2.57e-01
-7.61e-01
-2.06e-01
-1.52e-01
-6.35e-02
-3.19e-01
-2.75e-01
-2.15e-01
-3.81e-01
-1.34e-01
-2.70e-01
-1.22e-01
-8.48e-02
-1.34e-01
-1.16e-01
-3.14e-01
-2.11e-01
-3.71e-01
-2.31e-01
-2.69e-01
-1.64e-01
-2.33e-01
-4.66e-01
-2.95e-01
-3.36e-01
-8.09e-02
-2.11e-01
-3.00e-01
-6.92e-01
-2.10e-01
-3.15e-01
-1.56e-01
-1.98e-01
-1.15e-01
-2.10e-01
-2.89e-01
-2.75e-01
-2.65e-01
-2.60e-01
-2.31e-01
-2.41e-01
-1.76e-01
-2.20e-01
-2.80e-01
-2.83e-01
-2.07e-01
-2.17e-01
-1.80e-01
-2.54e-01
-2.68e-01
-2.87e-01
-4.54e-01
-2.59e-01
-3.70e-01
-6.46e-02
-1.75e-01
-1.02e-01
-3.15e-01
-2.09e-01
-2.36e-01
-2.49e-01
-3.38e-01
-4.01e-01
-3.47e-01
-1.35e-01
-2.96e-01
-4.44e-01
-2.93e-01
-1.77e-01
-5.13e-01
-2.89e-01
-9.19e-02
-1.24e-01
-1.28e-01
-2.34e-01
-3.01e-01
-3.72e-01
-3.51e-01
-4.21e-01
-3.97e-01
-6.59e-01
-1.89e-01
-1.86e-01
-3.56e-01
-2.37e-01
-5.10e-01
-2.71e-01
-6.18e-01
-6.72e-01
-1.46e-01
-2.64e-01
-3.32e-01
-4.76e-01
-2.07e-01
-3.03e-01
-2.52e-01
-1.11e-01
-3.00e-01
-2.33e-01
-2.30e-01
-1.87e-01
-2.26e-01
-2.49e-01
-1.08e-01
-1.90e-01
-3.17e-01
-2.83e-01
-2.16e-01
-4.12e-01
-9.85e-02
-1.77e-01
-2.49e-01
-2.11e-01
-2.46e-01
-2.71e-01
-4.20e-01
-2.02e-01
-3.84e-01
-1.75e-01
-1.07e-01
-2.56e-01
-2.00e-01
-3.57e-01
-1.71e-01
-2.31e-01
-2.13e-01
-2.75e-01
-3.96e-01
-2.53e-01
-2.68e-01
-1.41e-01
-1.30e-01
-3.74e-01
-3.20e-01
-2.43e-01
-2.64e-01
-4.56e-01
-3.22e-01
-2.70e-01
-1.89e-01
-3.29e-01
-2.67e-01
-1.75e-01
-2.68e-01
-1.66e-01
-4.33e-01
-1.16e-01
-4.49e-01
-2.20e-01
-1.11e-01
-2.69e-01
-2.00e-01
-4.64e-01
-1.70e-01
-1.44e-01
-3.22e-01
-8.22e-01
-1.48e-01
-2.39e-01
-2.80e-01
-2.59e-01
-2.79e-01
-2.48e-01
-2.14e-01
-1.23e-01
-4.23e-01
-1.78e-01
-2.27e-01
-3.00e-01
-3.73e-01
-3.32e-01
-3.27e-01
-1.80e-01
-3.05e-01
-1.91e-01
-3.42e-01
-2.63e-01
-1.46e-01
-2.82e-01
-3.04e-01
-1.90e-01
-1.21e-01
-3.40e-01
-1.51e-01
-3.59e-01
-2.00e-01
-2.57e-01
-3.38e-01
-4.48e-01
-2.75e-01
-1.63e-01
-7.42e-02
-2.85e-01
-1.88e-01
-2.48e-01
-1.49e-01
-1.42e-01
-3.67e-01
-1.55e-01
-1.94e-01
-1.11e-01
-2.53e-01
-4.73e-01
-1.68e-01
-4.63e-01
-4.60e-01
-4.00e-01
-3.18e-01
-1.51e-01
-3.94e-01
-3.52e-01
-1.56e-01
-1.64e-01
-3.04e-01
-2.52e-01
-3.03e-01
-1.62e-01
-1.71e-01
-3.40e-01
-4.16e-01
-4.73e-01
-7.23e-02
-3.54e-01
-2.81e-01
-1.89e-01
-4.88e-01
-7.51e-02
-4.03e-01
-5.86e-01
-2.94e-01
-2.31e-01
-4.16e-01
-1.46e-01
-2.36e-01
-2.86e-01
-4.28e-01
-2.03e-01
-2.41e-01
-2.19e-01
-1.59e-01
-1.45e-01
-3.10e-01
-5.08e-01
-1.60e-01
-2.92e-01
-3.40e-01
-1.36e-01
-4.04e-01
-1.35e-01
-2.42e-01
-2.03e-01
-1.45e-01
-1.73e-01
-4.72e-01
-3.59e-01
-1.71e-01
-2.17e-01
-2.16e-01
-1.33e-01
-2.01e-01
-3.32e-01
-1.18e-01
-2.91e-01
-4.40e-01
-1.89e-01
-2.77e-01
-3.76e-01
-4.05e-01
-3.52e-01
-3.74e-01
-7.37e-01
-1.80e-01
-1.17e-01
-1.69e-01
-2.42e-01
-2.16e-01
-2.76e-01
-2.19e-01
-1.45e-01
-3.60e-01
-4.62e-01
-1.94e-01
-2.87e-01
-2.63e-01
-2.61e-01
-8.26e-02
-3.50e-01
-5.11e-01
-3.32e-01
-4.39e-01
-1.29e-01
-2.83e-01
-2.30e-01
-3.80e-01
-3.51e-01
-1.77e-01
-4.75e-02
-2.28e-01
-3.13e-01
-1.69e-01
-2.57e-01
-2.16e-01
-1.39e-01
-2.31e-01
-1.24e-01
-3.20e-01
-3.03e-01
-5.09e-01
-3.01e-01
-3.17e-01
-1.30e-01
-1.15e-01
-3.78e-01
-3.75e-01
-2.27e-01
-1.50e-01
-4.02e-01
-4.23e-01
-2.95e-01
-5.05e-01
-3.23e-01
-3.84e-01
-2.82e-01
-1.14e-01
-1.24e-01
-3.12e-01
-1.60e-01
-3.87e-01
-3.55e-01
-3.79e-01
-4.12e-01
-4.21e-01
-3.25e-01
-3.26e-01
-1.94e-01
-1.05e-01
-3.01e-01
-3.88e-01
-1.87e-01
-3.17e-01
-1.60e-01
-5.73e-01
-3.01e-01
-1.79e-01
-1.72e-01
-4.37e-01
-4.15e-01
-3.85e-01
-2.23e-01
-1.78e-01
-1.12e-01
-2.34e-01
-3.88e-01
-2.28e-01
-2.02e-01
-1.10e-01
-2.14e-01
-4.06e-01
-2.22e-01
-2.97e-01
-2.52e-01
-4.38e-01
-1.40e-01
-3.74e-01
-2.95e-01
-3.39e-01
-2.25e-01
-7.14e-02
-3.50e-01
-3.38e-01
-1.93e-01
-1.12e-01
-9.06e-02
-3.30e-01
-2.61e-01
-1.87e-01
-3.25e-01
-8.43e-02
-3.10e-01
-2.55e-01
-1.67e-01
-3.00e-01
-4.11e-01
-1.77e-01
-2.13e-01
-1.88e-01
-2.64e-01
-2.04e-01
-5.15e-01
-2.39e-01
-9.17e-02
-3.71e-01
-1.35e-01
-1.93e-01
-1.31e-01
-1.56e-01
-1.41e-01
-2.24e-01
-1.16e-01
-1.40e-01
-1.61e-01
-2.41e-01
-3.92e-01
-2.14e-01
-4.66e-01
-2.92e-01
-2.50e-01
-1.30e-01
-1.88e-01
-2.55e-01
-4.89e-01
-1.41e-01
+3.77e-01
+4.60e-01
+3.48e-01
+3.87e-01
+1.03e+00
+4.35e-01
+2.60e-01
+5.25e-01
+4.34e-01
+5.42e-01
+4.59e-01
+3.45e-01
+5.36e-01
+5.39e-01
+2.46e-01
+3.57e-01
+6.21e-01
+4.27e-01
+5.34e-01
+6.16e-01
+4.15e-01
+3.49e-01
+4.44e-01
+3.68e-01
+3.84e-01
+2.52e-01
+3.61e-01
+4.67e-01
+3.54e-01
+8.28e-01
+5.21e-01
+4.03e-01
+4.31e-01
+6.51e-01
+4.46e-01
+3.81e-01
+7.62e-01
+7.96e-01
+5.81e-01
+4.64e-01
+8.61e-01
+2.43e-01
+3.44e-01
+3.78e-01
+2.63e-01
+2.36e-01
+4.36e-01
+3.57e-01
+4.74e-01
+5.51e-01
+4.83e-01
+7.21e-01
+6.24e-01
+3.92e-01
+4.37e-01
+6.91e-01
+3.37e-01
+3.50e-01
+4.81e-01
+5.85e-01
+3.14e-01
+1.36e+00
+3.95e-01
+2.08e-01
+1.50e-01
+6.03e-01
+4.51e-01
+4.43e-01
+6.17e-01
+6.37e-01
+4.21e-01
+3.67e-01
+3.95e-01
+3.67e-01
+2.63e-01
+3.07e-01
+6.13e-01
+5.49e-01
+5.54e-01
+4.74e-01
+4.00e-01
+3.01e-01
+3.76e-01
+3.11e-01
+7.04e-01
+5.44e-01
+5.92e-01
+3.59e-01
+7.64e-01
+5.10e-01
+5.00e-01
+5.13e-01
+8.48e-01
+1.86e-01
+3.65e-01
+3.72e-01
+2.31e-01
+6.01e-01
+4.60e-01
+6.39e-01
+4.57e-01
+3.04e-01
+2.83e-01
+4.01e-01
+5.96e-01
+6.22e-01
+3.55e-01
+3.91e-01
+6.53e-01
+4.87e-01
+3.77e-01
+4.57e-01
+4.10e-01
+3.81e-01
+5.94e-01
+4.10e-01
+2.48e-01
+3.58e-01
+2.08e-01
+3.39e-01
+4.93e-01
+5.20e-01
+3.08e-01
+6.68e-01
+5.98e-01
+6.19e-01
+4.10e-01
+4.27e-01
+5.75e-01
+4.37e-01
+4.57e-01
+4.19e-01
+4.85e-01
+4.75e-01
+4.99e-01
+3.76e-01
+2.49e-01
+4.35e-01
+5.84e-01
+4.85e-01
+4.65e-01
+5.71e-01
+5.36e-01
+2.87e-01
+3.71e-01
+5.02e-01
+2.29e-01
+2.79e-01
+5.25e-01
+2.37e-01
+6.76e-01
+3.50e-01
+4.56e-01
+3.80e-01
+2.55e-01
+3.79e-01
+3.62e-01
+6.85e-01
+4.41e-01
+4.16e-01
+5.62e-01
+6.04e-01
+4.48e-01
+2.90e-01
+6.37e-01
+4.32e-01
+6.11e-01
+4.48e-01
+8.05e-01
+3.37e-01
+3.34e-01
+3.02e-01
+3.42e-01
+5.75e-01
+4.73e-01
+2.56e-01
+2.43e-01
+3.25e-01
+5.62e-01
+5.08e-01
+2.74e-01
+3.76e-01
+7.48e-01
+7.07e-01
+1.86e-01
+3.75e-01
+3.75e-01
+3.89e-01
+6.90e-01
+3.14e-01
+5.13e-01
+1.99e-01
+3.79e-01
+3.12e-01
+6.17e-01
+2.91e-01
+7.93e-01
+3.88e-01
+5.26e-01
+5.62e-01
+7.40e-01
+3.06e-01
+4.20e-01
+3.26e-01
+3.98e-01
+5.84e-01
+2.99e-01
+4.66e-01
+3.61e-01
+3.04e-01
+3.78e-01
+3.17e-01
+3.31e-01
+3.11e-01
+5.84e-01
+4.15e-01
+4.10e-01
+3.51e-01
+5.58e-01
+6.80e-01
+3.52e-01
+5.67e-01
+3.13e-01
+2.83e-01
+3.75e-01
+5.08e-01
+2.23e-01
+1.93e-01
+1.42e-01
+4.46e-01
+2.65e-01
+2.89e-01
+3.50e-01
+3.38e-01
+5.08e-01
+4.45e-01
+4.08e-01
+2.37e-01
+5.65e-01
+6.45e-01
+6.18e-01
+4.98e-01
+5.81e-01
+5.03e-01
+5.43e-01
+3.10e-01
+3.76e-01
+3.91e-01
+4.97e-01
+5.54e-01
+3.91e-01
+3.10e-01
+3.23e-01
+3.58e-01
+7.42e-01
+3.52e-01
+4.50e-01
+4.09e-01
+4.90e-01
+5.49e-01
+3.70e-01
+4.93e-01
+7.10e-01
+3.64e-01
+8.16e-01
+4.08e-01
+2.89e-01
+6.03e-01
+2.49e-01
+4.07e-01
+5.30e-01
+5.88e-01
+7.63e-01
+4.09e-01
+5.46e-01
+6.05e-01
+5.38e-01
+4.21e-01
+4.11e-01
+3.64e-01
+2.77e-01
+7.46e-01
+5.88e-01
+6.27e-01
+4.08e-01
+5.11e-01
+8.04e-01
+6.44e-01
+4.87e-01
+4.66e-01
+7.71e-01
+5.25e-01
+3.00e-01
+3.52e-01
+3.86e-01
+6.02e-01
+3.18e-01
+4.55e-01
+4.27e-01
+4.54e-01
+3.57e-01
+4.65e-01
+8.30e-01
+4.53e-01
+8.73e-01
+5.41e-01
+7.10e-01
+5.47e-01
+4.24e-01
+4.18e-01
+3.94e-01
+2.56e-01
+2.75e-01
+3.55e-01
+5.77e-01
+4.68e-01
+5.41e-01
+5.46e-01
+2.67e-01
+5.12e-01
+4.47e-01
+3.02e-01
+4.02e-01
+2.94e-01
+4.33e-01
+7.12e-01
+3.89e-01
+6.10e-01
+3.88e-01
+5.20e-01
+5.74e-01
+4.10e-01
+3.74e-01
+4.45e-01
+2.74e-01
+2.77e-01
+2.40e-01
+2.73e-01
+2.93e-01
+4.67e-01
+5.18e-01
+3.49e-01
+5.92e-01
+6.16e-01
+3.17e-01
+2.43e-01
+3.07e-01
+5.26e-01
+4.45e-01
+2.58e-01
+3.96e-01
+6.16e-01
+2.33e-01
+7.22e-01
+4.02e-01
+3.38e-01
+3.22e-01
+6.27e-01
+5.06e-01
+3.01e-01
+4.47e-01
+2.13e-01
+5.74e-01
+5.10e-01
+4.85e-01
+5.33e-01
+4.66e-01
+2.10e-01
+5.84e-01
+1.63e-01
+3.85e-01
+3.22e-01
+4.08e-01
+5.75e-01
+3.05e-01
+3.33e-01
+3.65e-01
+4.70e-01
+7.98e-01
+4.90e-01
+2.21e-01
+3.34e-01
+4.81e-01
+5.17e-01
+5.08e-01
+4.91e-01
+4.03e-01
+4.43e-01
+4.42e-01
+3.53e-01
+4.24e-01
+4.61e-01
+5.18e-01
+5.57e-01
+3.17e-01
+3.53e-01
+3.86e-01
+5.26e-01
+2.85e-01
+5.23e-01
+2.91e-01
+5.07e-01
+5.23e-01
+3.02e-01
+2.33e-01
+7.20e-01
+6.64e-01
+6.45e-01
+2.90e-01
+5.40e-01
+2.74e-01
+4.15e-01
+2.65e-01
+2.60e-01
+2.66e-01
+2.09e-01
+4.50e-01
+5.21e-01
+2.14e-01
+5.95e-01
+4.38e-01
+5.64e-01
+6.40e-01
+3.08e-01
+2.95e-01
+5.38e-01
+3.98e-01
+5.21e-01
+2.88e-01
+5.15e-01
+2.34e-01
+4.47e-01
+4.09e-01
+6.61e-01
+3.33e-01
+5.21e-01
+3.18e-01
+2.96e-01
+4.24e-01
+4.66e-01
+4.07e-01
+8.38e-01
+3.65e-01
+4.20e-01
+5.25e-01
+3.32e-01
+5.52e-01
+4.40e-01
+2.49e-01
+6.61e-01
+4.62e-01
+3.98e-01
+2.08e-01
+3.76e-01
+4.32e-01
+5.44e-01
+2.68e-01
+4.05e-01
+2.23e-01
+4.15e-01
+4.53e-01
+4.59e-01
+5.07e-01
+4.56e-01
+3.81e-01
+7.22e-01
+2.24e-01
+4.68e-01
+4.97e-01
+5.86e-01
+2.77e-01
+4.65e-01
+2.11e-01
+3.35e-01
+5.77e-01
+3.10e-01
+7.48e-01
+7.16e-01
+5.07e-01
+3.43e-01
+2.32e-01
+2.21e-01
+6.66e-01
+3.45e-01
+5.34e-01
+5.50e-01
+4.77e-01
+6.78e-01
+2.52e-01
+4.94e-01
+4.78e-01
+4.77e-01
+6.34e-01
+4.94e-01
+3.58e-01
+4.73e-01
+3.40e-01
+4.29e-01
+4.38e-01
+5.29e-01
+4.77e-01
+4.33e-01
+3.90e-01
+6.03e-01
+6.03e-01
+3.86e-01
+4.87e-01
+3.43e-01
+3.77e-01
+3.15e-01
+8.09e-01
+3.30e-01
+5.05e-01
+3.44e-01
+4.96e-01
+6.19e-01
+3.22e-01
+4.54e-01
+8.08e-01
+3.67e-01
+6.40e-01
+4.66e-01
+4.80e-01
+4.83e-01
+5.57e-01
+3.48e-01
+6.04e-01
+4.43e-01
+5.33e-01
+5.21e-01
+2.84e-01
+5.25e-01
+3.09e-01
+3.48e-01
+5.80e-01
+5.49e-01
+6.14e-01
+4.72e-01
+5.41e-01
+4.34e-01
+4.22e-01
+5.50e-01
+1.87e-01
+3.31e-01
+3.95e-01
+6.47e-01
+4.65e-01
+3.84e-01
+4.40e-01
+3.41e-01
+3.58e-01
+2.85e-01
+3.85e-01
+5.97e-01
+6.75e-01
+3.37e-01
+4.01e-01
+4.88e-01
+4.54e-01
+2.58e-01
+4.96e-01
+3.15e-01
+3.05e-01
+5.10e-01
+3.06e-01
+4.55e-01
+5.18e-01
+3.61e-01
+7.79e-01
+3.09e-01
+6.90e-01
+3.09e-01
+6.63e-01
+8.10e-01
+3.10e-01
+6.95e-01
+4.08e-01
+4.81e-01
+4.08e-01
+4.23e-01
+5.45e-01
+3.02e-01
+4.62e-01
+3.46e-01
+3.25e-01
+2.02e-01
+4.63e-01
+5.67e-01
+2.98e-01
+4.28e-01
+3.17e-01
+2.67e-01
+3.43e-01
+5.51e-01
+6.38e-01
+6.25e-01
+5.03e-01
+5.41e-01
+3.12e-01
+4.96e-01
+3.23e-01
+2.94e-01
+3.95e-01
+2.65e-01
+8.88e-01
+4.63e-01
+3.45e-01
+4.05e-01
+6.46e-01
+5.13e-01
+4.97e-01
+1.93e-01
+7.18e-01
+4.91e-01
+5.03e-01
+2.77e-01
+4.36e-01
+2.30e-01
+4.13e-01
+2.34e-01
+3.29e-01
+5.68e-01
+2.37e-01
+3.22e-01
+5.34e-01
+7.98e-01
+3.86e-01
+5.22e-01
+6.77e-01
+4.46e-01
+3.09e-01
+2.97e-01
+4.27e-01
+3.70e-01
+4.34e-01
+6.86e-01
+5.35e-01
+4.49e-01
+5.35e-01
+4.96e-01
+5.68e-01
+3.53e-01
+6.96e-01
+2.84e-01
+3.96e-01
+4.81e-01
+3.36e-01
+1.54e-01
+3.77e-01
+5.48e-01
+1.08e+00
+2.76e-01
+4.30e-01
+2.25e-01
+6.69e-01
+4.07e-01
+5.68e-01
+3.49e-01
+5.67e-01
+5.59e-01
+2.83e-01
+3.89e-01
+5.78e-01
+3.38e-01
+1.93e-01
+2.56e-01
+4.33e-01
+3.92e-01
+3.05e-01
+4.21e-01
+4.85e-01
+2.58e-01
+4.52e-01
+9.98e-01
+6.47e-01
+4.28e-01
+5.98e-01
+3.30e-01
+6.32e-01
+6.07e-01
+3.71e-01
+2.71e-01
+2.70e-01
+3.77e-01
+4.95e-01
+6.42e-01
+7.23e-01
+4.75e-01
+2.27e-01
+3.50e-01
+4.07e-01
+5.38e-01
+3.41e-01
+3.06e-01
+5.44e-01
+4.74e-01
+2.47e-01
+4.44e-01
+2.07e-01
+4.82e-01
+2.97e-01
+5.16e-01
+4.59e-01
+4.95e-01
+3.87e-01
+3.80e-01
+3.72e-01
+2.86e-01
+5.60e-01
+4.66e-01
+2.72e-01
+3.20e-01
+5.51e-01
+3.93e-01
+4.71e-01
+6.73e-01
+4.45e-01
+5.79e-01
+6.42e-01
+5.56e-01
+3.04e-01
+5.90e-01
+5.99e-01
+3.18e-01
+2.48e-01
+6.56e-01
+5.79e-01
+2.07e-01
+8.08e-01
+2.57e-01
+6.68e-01
+2.14e-01
+2.01e-01
+2.36e-01
+1.90e-01
+6.49e-01
+7.88e-01
+8.98e-01
+2.48e-01
+5.10e-01
+6.07e-01
+3.39e-01
+5.02e-01
+5.25e-01
+4.66e-01
+1.47e-01
+4.45e-01
+4.62e-01
+8.11e-01
+3.92e-01
+5.85e-01
+5.09e-01
+5.81e-01
+5.17e-01
+5.42e-01
+3.23e-01
+4.52e-01
+2.02e-01
+3.93e-01
+3.79e-01
+3.81e-01
+3.41e-01
+4.97e-01
+6.28e-01
+4.19e-01
+3.14e-01
+5.58e-01
+6.43e-01
+4.70e-01
+5.19e-01
+6.95e-01
+3.51e-01
+6.11e-01
+5.85e-01
+3.45e-01
+3.48e-01
+2.32e-01
+4.93e-01
+5.72e-01
+2.70e-01
+3.63e-01
+6.98e-01
+3.94e-01
+4.07e-01
+3.08e-01
+5.11e-01
+4.92e-01
+2.74e-01
+3.16e-01
+7.29e-01
+5.95e-01
+3.98e-01
+2.67e-01
+4.69e-01
+3.27e-01
+5.63e-01
+4.80e-01
+5.28e-01
+4.37e-01
+5.50e-01
+4.03e-01
+6.10e-01
+3.30e-01
+4.12e-01
+3.21e-01
+5.57e-01
+6.18e-01
+8.65e-01
+6.06e-01
+3.21e-01
+5.09e-01
+2.62e-01
+3.51e-01
+5.86e-01
+7.40e-01
+6.39e-01
+2.43e-01
+2.89e-01
+3.18e-01
+3.34e-01
+2.83e-01
+3.95e-01
+4.29e-01
+2.42e-01
+3.33e-01
+5.23e-01
+3.26e-01
+3.77e-01
+7.48e-01
+1.95e-01
+4.57e-01
+3.01e-01
+2.79e-01
+4.57e-01
+3.10e-01
+4.09e-01
+3.88e-01
+5.04e-01
+2.70e-01
+2.61e-01
+2.97e-01
+4.71e-01
+4.29e-01
+5.32e-01
+3.06e-01
+6.13e-01
+3.33e-01
+4.78e-01
+6.56e-01
+4.01e-01
+2.34e-01
+4.26e-01
+3.71e-01
+6.70e-01
+3.07e-01
+4.25e-01
+6.57e-01
+3.65e-01
+2.09e-01
+5.42e-01
+7.34e-01
+6.08e-01
+4.48e-01
+5.68e-01
+3.35e-01
+5.10e-01
+1.97e-01
+5.48e-01
+7.00e-01
+2.50e-01
+3.52e-01
+5.48e-01
+6.52e-01
+4.60e-01
+3.59e-01
+3.54e-01
+6.32e-01
+3.13e-01
+4.49e-01
+5.11e-01
+3.39e-01
+3.94e-01
+4.92e-01
+4.83e-01
+5.01e-01
+5.55e-01
+2.40e-01
+2.86e-01
+4.77e-01
+3.80e-01
+4.33e-01
+5.00e-01
+2.91e-01
+6.49e-01
+3.34e-01
+4.06e-01
+7.72e-01
+2.34e-01
+3.12e-01
+5.16e-01
+1.63e-01
+5.17e-01
+4.28e-01
+2.55e-01
+7.63e-01
+2.81e-01
+4.25e-01
+2.83e-01
+5.38e-01
+5.37e-01
+2.99e-01
+3.92e-01
+4.91e-01
+4.78e-01
+3.88e-01
+3.15e-01
+2.90e-01
+3.41e-01
+2.91e-01
+3.05e-01
+4.20e-01
+4.31e-01
+4.59e-01
+3.24e-01
+5.35e-01
+5.39e-01
+3.72e-01
+3.60e-01
+3.42e-01
+7.77e-01
+5.46e-01
+2.89e-01
+5.20e-01
+4.34e-01
+4.32e-01
+4.69e-01
+2.80e-01
+3.02e-01
+6.57e-01
+5.18e-01
+5.36e-01
+1.51e-01
+3.36e-01
+2.72e-01
+3.72e-01
+4.44e-01
+4.59e-01
+4.49e-01
+4.99e-01
+6.30e-01
+4.22e-01
+6.44e-01
+2.24e-01
+3.76e-01
+5.61e-01
+2.91e-01
+2.40e-01
+4.11e-01
+6.62e-01
+4.24e-01
+6.38e-01
+3.60e-01
+7.14e-01
+4.48e-01
+5.95e-01
+5.87e-01
+4.53e-01
+7.12e-01
+5.61e-01
+6.00e-01
+3.97e-01
+2.33e-01
+3.23e-01
+4.48e-01
+3.40e-01
+4.70e-01
+3.22e-01
+5.73e-01
+3.31e-01
+3.06e-01
+4.31e-01
+4.54e-01
+3.96e-01
+6.00e-01
+3.57e-01
+4.38e-01
+3.72e-01
+4.94e-01
+6.66e-01
+5.23e-01
+5.45e-01
+5.73e-01
+2.70e-01
+5.67e-01
+4.34e-01
+2.80e-01
+3.65e-01
+5.99e-01
+3.50e-01
+3.87e-01
+3.69e-01
+5.29e-01
+5.20e-01
+3.45e-01
+6.49e-01
+3.33e-01
+4.71e-01
+5.51e-01
+4.61e-01
+4.09e-01
+4.27e-01
+3.60e-01
+2.81e-01
+5.06e-01
+6.69e-01
+7.38e-01
+2.10e-01
+3.43e-01
+7.21e-01
+3.81e-01
+3.75e-01
+3.00e-01
+3.41e-01
+4.56e-01
+4.34e-01
+6.61e-01
+3.88e-01
+6.10e-01
+3.61e-01
+4.57e-01
+1.64e-01
+5.50e-01
+4.92e-01
+6.55e-01
+3.10e-01
+2.20e-01
+4.01e-01
+4.32e-01
+4.95e-01
+4.75e-01
+6.28e-01
+5.77e-01
+3.95e-01
+2.97e-01
+3.89e-01
+3.77e-01
+5.17e-01
+3.75e-01
+4.45e-01
+3.34e-01
+4.53e-01
+7.58e-01
+3.99e-01
+6.25e-01
+3.41e-01
+2.55e-01
+5.21e-01
+5.47e-01
+4.21e-01
+2.98e-01
+2.50e-01
+5.85e-01
+5.20e-01
+3.85e-01
+5.24e-01
+3.91e-01
+7.08e-01
+6.07e-01
+3.32e-01
+6.34e-01
+2.92e-01
+2.76e-01
+6.20e-01
+2.35e-01
+3.05e-01
+2.05e-01
+1.64e-01
+4.01e-01
+6.12e-01
+4.37e-01
+5.04e-01
+1.08e+00
+6.74e-01
+5.28e-01
+5.42e-01
+4.65e-01
+4.17e-01
+3.66e-01
+5.01e-01
+2.42e-01
+1.74e-01
+4.25e-01
+4.63e-01
+4.58e-01
+4.04e-01
+3.20e-01
+4.67e-01
+3.35e-01
+2.90e-01
+7.34e-01
+3.98e-01
+3.56e-01
+3.45e-01
+4.35e-01
+3.03e-01
+2.04e-01
+5.98e-01
+2.13e-01
+6.47e-01
+5.37e-01
+2.84e-01
+4.98e-01
+3.04e-01
+5.13e-01
+2.58e-01
+3.03e-01
+2.21e-01
+5.67e-01
+1.51e-01
+3.14e-01
+4.54e-01
+4.40e-01
+3.92e-01
+4.95e-01
+6.66e-01
+3.38e-01
+3.46e-01
+3.63e-01
+3.07e-01
+5.91e-01
+5.12e-01
+5.87e-01
```

### Comparing `nanite-3.5.4/nanite/rate/ts_zef18/train_response.txt` & `nanite-3.6.0/nanite/rate/ts_zef18/train_response.txt`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,1132 +1,1132 @@
-5.00e+00
-6.00e+00
-8.00e+00
-5.00e+00
-0.00e+00
-5.00e+00
-6.00e+00
-2.00e+00
-5.00e+00
-4.00e+00
-5.00e+00
-5.00e+00
-4.00e+00
-4.00e+00
-3.00e+00
-5.00e+00
-4.00e+00
-6.00e+00
-4.00e+00
-3.00e+00
-3.00e+00
-6.00e+00
-4.00e+00
-4.00e+00
-6.00e+00
-3.00e+00
-5.00e+00
-3.00e+00
-5.00e+00
-2.00e+00
-5.00e+00
-5.00e+00
-4.00e+00
-3.00e+00
-4.00e+00
-4.00e+00
-2.00e+00
-3.00e+00
-4.00e+00
-5.00e+00
-3.00e+00
-9.00e+00
-4.00e+00
-5.00e+00
-4.00e+00
-6.00e+00
-3.00e+00
-7.00e+00
-4.00e+00
-5.00e+00
-4.00e+00
-3.00e+00
-5.00e+00
-6.00e+00
-4.00e+00
-4.00e+00
-7.00e+00
-4.00e+00
-4.00e+00
-5.00e+00
-4.00e+00
-0.00e+00
-3.00e+00
-8.00e+00
-5.00e+00
-4.00e+00
-4.00e+00
-4.00e+00
-4.00e+00
-4.00e+00
-4.00e+00
-4.00e+00
-3.00e+00
-5.00e+00
-5.00e+00
-5.00e+00
-4.00e+00
-3.00e+00
-4.00e+00
-3.00e+00
-5.00e+00
-6.00e+00
-6.00e+00
-6.00e+00
-2.00e+00
-4.00e+00
-5.00e+00
-5.00e+00
-3.00e+00
-4.00e+00
-3.00e+00
-3.00e+00
-1.00e+00
-1.00e+01
-4.00e+00
-5.00e+00
-3.00e+00
-4.00e+00
-4.00e+00
-3.00e+00
-4.00e+00
-4.00e+00
-6.00e+00
-3.00e+00
-3.00e+00
-3.00e+00
-4.00e+00
-3.00e+00
-3.00e+00
-5.00e+00
-6.00e+00
-4.00e+00
-5.00e+00
-4.00e+00
-3.00e+00
-5.00e+00
-6.00e+00
-5.00e+00
-5.00e+00
-4.00e+00
-4.00e+00
-1.00e+00
-6.00e+00
-3.00e+00
-4.00e+00
-4.00e+00
-4.00e+00
-3.00e+00
-4.00e+00
-2.00e+00
-3.00e+00
-4.00e+00
-2.00e+00
-3.00e+00
-4.00e+00
-1.00e+01
-5.00e+00
-3.00e+00
-5.00e+00
-4.00e+00
-4.00e+00
-0.00e+00
-4.00e+00
-6.00e+00
-9.00e+00
-4.00e+00
-1.00e+01
-5.00e+00
-6.00e+00
-1.00e+01
-3.00e+00
-7.00e+00
-1.00e+00
-4.00e+00
-4.00e+00
-5.00e+00
-5.00e+00
-3.00e+00
-3.00e+00
-5.00e+00
-3.00e+00
-5.00e+00
-4.00e+00
-4.00e+00
-3.00e+00
-4.00e+00
-3.00e+00
-4.00e+00
-2.00e+00
-5.00e+00
-4.00e+00
-1.00e+01
-8.00e+00
-4.00e+00
-4.00e+00
-4.00e+00
-1.00e+01
-8.00e+00
-4.00e+00
-5.00e+00
-7.00e+00
-6.00e+00
-4.00e+00
-3.00e+00
-7.00e+00
-4.00e+00
-4.00e+00
-5.00e+00
-3.00e+00
-4.00e+00
-5.00e+00
-8.00e+00
-6.00e+00
-1.00e+01
-3.00e+00
-8.00e+00
-3.00e+00
-8.00e+00
-3.00e+00
-2.00e+00
-3.00e+00
-5.00e+00
-3.00e+00
-9.00e+00
-5.00e+00
-5.00e+00
-9.00e+00
-4.00e+00
-5.00e+00
-5.00e+00
-5.00e+00
-1.00e+01
-6.00e+00
-4.00e+00
-4.00e+00
-5.00e+00
-5.00e+00
-4.00e+00
-4.00e+00
-3.00e+00
-7.00e+00
-4.00e+00
-5.00e+00
-8.00e+00
-5.00e+00
-3.00e+00
-7.00e+00
-1.00e+01
-1.00e+01
-3.00e+00
-7.00e+00
-7.00e+00
-6.00e+00
-5.00e+00
-3.00e+00
-5.00e+00
-5.00e+00
-1.00e+01
-2.00e+00
-3.00e+00
-5.00e+00
-4.00e+00
-4.00e+00
-3.00e+00
-4.00e+00
-5.00e+00
-9.00e+00
-3.00e+00
-4.00e+00
-3.00e+00
-5.00e+00
-9.00e+00
-5.00e+00
-1.00e+00
-4.00e+00
-6.00e+00
-4.00e+00
-5.00e+00
-5.00e+00
-5.00e+00
-4.00e+00
-4.00e+00
-3.00e+00
-6.00e+00
-3.00e+00
-5.00e+00
-6.00e+00
-4.00e+00
-9.00e+00
-6.00e+00
-3.00e+00
-4.00e+00
-3.00e+00
-2.00e+00
-4.00e+00
-4.00e+00
-4.00e+00
-4.00e+00
-3.00e+00
-5.00e+00
-4.00e+00
-0.00e+00
-3.00e+00
-0.00e+00
-2.00e+00
-4.00e+00
-3.00e+00
-3.00e+00
-3.00e+00
-9.00e+00
-0.00e+00
-3.00e+00
-5.00e+00
-6.00e+00
-6.00e+00
-4.00e+00
-3.00e+00
-4.00e+00
-5.00e+00
-5.00e+00
-4.00e+00
-4.00e+00
-3.00e+00
-5.00e+00
-0.00e+00
-4.00e+00
-4.00e+00
-2.00e+00
-2.00e+00
-4.00e+00
-3.00e+00
-5.00e+00
-6.00e+00
-1.00e+01
-4.00e+00
-3.00e+00
-4.00e+00
-3.00e+00
-6.00e+00
-4.00e+00
-5.00e+00
-5.00e+00
-5.00e+00
-2.00e+00
-3.00e+00
-4.00e+00
-5.00e+00
-3.00e+00
-2.00e+00
-3.00e+00
-3.00e+00
-4.00e+00
-4.00e+00
-5.00e+00
-6.00e+00
-7.00e+00
-1.00e+01
-6.00e+00
-9.00e+00
-3.00e+00
-3.00e+00
-4.00e+00
-3.00e+00
-4.00e+00
-4.00e+00
-5.00e+00
-6.00e+00
-3.00e+00
-4.00e+00
-6.00e+00
-9.00e+00
-5.00e+00
-7.00e+00
-4.00e+00
-5.00e+00
-2.00e+00
-8.00e+00
-3.00e+00
-6.00e+00
-7.00e+00
-1.00e+00
-5.00e+00
-4.00e+00
-5.00e+00
-4.00e+00
-3.00e+00
-6.00e+00
-8.00e+00
-4.00e+00
-1.00e+01
-4.00e+00
-5.00e+00
-4.00e+00
-4.00e+00
-6.00e+00
-6.00e+00
-6.00e+00
-4.00e+00
-2.00e+00
-0.00e+00
-6.00e+00
-6.00e+00
-5.00e+00
-3.00e+00
-3.00e+00
-4.00e+00
-5.00e+00
-4.00e+00
-5.00e+00
-6.00e+00
-4.00e+00
-3.00e+00
-4.00e+00
-4.00e+00
-3.00e+00
-8.00e+00
-4.00e+00
-1.00e+00
-6.00e+00
-2.00e+00
-4.00e+00
-3.00e+00
-0.00e+00
-8.00e+00
-6.00e+00
-3.00e+00
-3.00e+00
-3.00e+00
-4.00e+00
-3.00e+00
-5.00e+00
-5.00e+00
-1.00e+01
-3.00e+00
-7.00e+00
-4.00e+00
-4.00e+00
-4.00e+00
-1.00e+01
-5.00e+00
-4.00e+00
-3.00e+00
-1.00e+00
-8.00e+00
-6.00e+00
-6.00e+00
-5.00e+00
-5.00e+00
-7.00e+00
-4.00e+00
-9.00e+00
-5.00e+00
-3.00e+00
-4.00e+00
-4.00e+00
-4.00e+00
-1.00e+01
-6.00e+00
-3.00e+00
-7.00e+00
-4.00e+00
-0.00e+00
-5.00e+00
-4.00e+00
-2.00e+00
-2.00e+00
-3.00e+00
-4.00e+00
-5.00e+00
-3.00e+00
-4.00e+00
-3.00e+00
-1.00e+01
-3.00e+00
-3.00e+00
-4.00e+00
-3.00e+00
-9.00e+00
-8.00e+00
-5.00e+00
-3.00e+00
-5.00e+00
-4.00e+00
-4.00e+00
-4.00e+00
-3.00e+00
-6.00e+00
-4.00e+00
-4.00e+00
-3.00e+00
-3.00e+00
-3.00e+00
-1.00e+01
-7.00e+00
-3.00e+00
-3.00e+00
-4.00e+00
-3.00e+00
-3.00e+00
-5.00e+00
-7.00e+00
-6.00e+00
-2.00e+00
-5.00e+00
-1.00e+00
-3.00e+00
-4.00e+00
-4.00e+00
-8.00e+00
-4.00e+00
-4.00e+00
-4.00e+00
-4.00e+00
-4.00e+00
-5.00e+00
-4.00e+00
-8.00e+00
-3.00e+00
-4.00e+00
-4.00e+00
-2.00e+00
-4.00e+00
-4.00e+00
-4.00e+00
-4.00e+00
-9.00e+00
-4.00e+00
-5.00e+00
-2.00e+00
-6.00e+00
-0.00e+00
-5.00e+00
-5.00e+00
-6.00e+00
-4.00e+00
-4.00e+00
-7.00e+00
-4.00e+00
-1.00e+00
-7.00e+00
-4.00e+00
-3.00e+00
-4.00e+00
-4.00e+00
-3.00e+00
-5.00e+00
-3.00e+00
-4.00e+00
-4.00e+00
-4.00e+00
-3.00e+00
-4.00e+00
-5.00e+00
-4.00e+00
-3.00e+00
-4.00e+00
-4.00e+00
-4.00e+00
-4.00e+00
-5.00e+00
-4.00e+00
-3.00e+00
-1.00e+01
-4.00e+00
-5.00e+00
-5.00e+00
-1.00e+00
-4.00e+00
-4.00e+00
-5.00e+00
-4.00e+00
-9.00e+00
-5.00e+00
-4.00e+00
-2.00e+00
-5.00e+00
-6.00e+00
-4.00e+00
-4.00e+00
-1.00e+01
-4.00e+00
-9.00e+00
-4.00e+00
-3.00e+00
-5.00e+00
-4.00e+00
-1.00e+00
-9.00e+00
-1.00e+00
-5.00e+00
-3.00e+00
-8.00e+00
-4.00e+00
-0.00e+00
-6.00e+00
-2.00e+00
-5.00e+00
-2.00e+00
-6.00e+00
-4.00e+00
-4.00e+00
-9.00e+00
-5.00e+00
-4.00e+00
-5.00e+00
-5.00e+00
-4.00e+00
-4.00e+00
-5.00e+00
-4.00e+00
-8.00e+00
-4.00e+00
-6.00e+00
-4.00e+00
-3.00e+00
-4.00e+00
-4.00e+00
-4.00e+00
-5.00e+00
-4.00e+00
-5.00e+00
-4.00e+00
-4.00e+00
-5.00e+00
-1.00e+00
-3.00e+00
-5.00e+00
-5.00e+00
-2.00e+00
-4.00e+00
-4.00e+00
-1.00e+01
-3.00e+00
-4.00e+00
-4.00e+00
-5.00e+00
-4.00e+00
-4.00e+00
-4.00e+00
-9.00e+00
-5.00e+00
-5.00e+00
-5.00e+00
-5.00e+00
-3.00e+00
-3.00e+00
-3.00e+00
-5.00e+00
-4.00e+00
-1.00e+00
-6.00e+00
-4.00e+00
-4.00e+00
-7.00e+00
-3.00e+00
-2.00e+00
-3.00e+00
-5.00e+00
-3.00e+00
-5.00e+00
-5.00e+00
-6.00e+00
-3.00e+00
-4.00e+00
-4.00e+00
-3.00e+00
-6.00e+00
-6.00e+00
-4.00e+00
-3.00e+00
-0.00e+00
-4.00e+00
-3.00e+00
-7.00e+00
-4.00e+00
-5.00e+00
-4.00e+00
-5.00e+00
-1.00e+00
-4.00e+00
-8.00e+00
-5.00e+00
-3.00e+00
-5.00e+00
-6.00e+00
-5.00e+00
-5.00e+00
-5.00e+00
-4.00e+00
-3.00e+00
-5.00e+00
-8.00e+00
-4.00e+00
-2.00e+00
-4.00e+00
-4.00e+00
-4.00e+00
-4.00e+00
-4.00e+00
-4.00e+00
-6.00e+00
-7.00e+00
-5.00e+00
-4.00e+00
-4.00e+00
-4.00e+00
-2.00e+00
-6.00e+00
-9.00e+00
-5.00e+00
-5.00e+00
-4.00e+00
-4.00e+00
-6.00e+00
-4.00e+00
-3.00e+00
-5.00e+00
-5.00e+00
-6.00e+00
-4.00e+00
-6.00e+00
-4.00e+00
-4.00e+00
-4.00e+00
-8.00e+00
-7.00e+00
-3.00e+00
-4.00e+00
-4.00e+00
-3.00e+00
-5.00e+00
-4.00e+00
-4.00e+00
-3.00e+00
-3.00e+00
-4.00e+00
-4.00e+00
-3.00e+00
-3.00e+00
-1.00e+00
-9.00e+00
-3.00e+00
-4.00e+00
-7.00e+00
-1.00e+01
-3.00e+00
-4.00e+00
-5.00e+00
-2.00e+00
-5.00e+00
-3.00e+00
-5.00e+00
-1.00e+01
-8.00e+00
-7.00e+00
-4.00e+00
-3.00e+00
-3.00e+00
-4.00e+00
-2.00e+00
-4.00e+00
-5.00e+00
-3.00e+00
-3.00e+00
-4.00e+00
-9.00e+00
-5.00e+00
-4.00e+00
-0.00e+00
-4.00e+00
-4.00e+00
-5.00e+00
-4.00e+00
-5.00e+00
-5.00e+00
-5.00e+00
-4.00e+00
-4.00e+00
-4.00e+00
-4.00e+00
-5.00e+00
-1.00e+01
-5.00e+00
-3.00e+00
-4.00e+00
-5.00e+00
-4.00e+00
-4.00e+00
-4.00e+00
-5.00e+00
-4.00e+00
-3.00e+00
-4.00e+00
-3.00e+00
-7.00e+00
-6.00e+00
-8.00e+00
-3.00e+00
-5.00e+00
-6.00e+00
-4.00e+00
-3.00e+00
-4.00e+00
-4.00e+00
-7.00e+00
-4.00e+00
-3.00e+00
-4.00e+00
-4.00e+00
-3.00e+00
-4.00e+00
-8.00e+00
-9.00e+00
-6.00e+00
-7.00e+00
-4.00e+00
-3.00e+00
-3.00e+00
-4.00e+00
-2.00e+00
-2.00e+00
-4.00e+00
-8.00e+00
-4.00e+00
-5.00e+00
-0.00e+00
-3.00e+00
-0.00e+00
-3.00e+00
-5.00e+00
-4.00e+00
-3.00e+00
-4.00e+00
-3.00e+00
-3.00e+00
-3.00e+00
-1.00e+01
-3.00e+00
-6.00e+00
-6.00e+00
-7.00e+00
-5.00e+00
-5.00e+00
-7.00e+00
-7.00e+00
-2.00e+00
-4.00e+00
-5.00e+00
-3.00e+00
-6.00e+00
-5.00e+00
-5.00e+00
-6.00e+00
-4.00e+00
-6.00e+00
-4.00e+00
-4.00e+00
-3.00e+00
-6.00e+00
-1.00e+01
-5.00e+00
-4.00e+00
-4.00e+00
-5.00e+00
-6.00e+00
-4.00e+00
-6.00e+00
-3.00e+00
-4.00e+00
-5.00e+00
-7.00e+00
-4.00e+00
-4.00e+00
-4.00e+00
-6.00e+00
-5.00e+00
-3.00e+00
-4.00e+00
-6.00e+00
-2.00e+00
-3.00e+00
-4.00e+00
-4.00e+00
-4.00e+00
-6.00e+00
-0.00e+00
-9.00e+00
-3.00e+00
-3.00e+00
-4.00e+00
-5.00e+00
-4.00e+00
-3.00e+00
-5.00e+00
-9.00e+00
-4.00e+00
-2.00e+00
-7.00e+00
-2.00e+00
-4.00e+00
-6.00e+00
-4.00e+00
-4.00e+00
-4.00e+00
-5.00e+00
-3.00e+00
-8.00e+00
-5.00e+00
-4.00e+00
-4.00e+00
-4.00e+00
-3.00e+00
-5.00e+00
-1.00e+00
-7.00e+00
-4.00e+00
-3.00e+00
-8.00e+00
-5.00e+00
-3.00e+00
-4.00e+00
-6.00e+00
-3.00e+00
-6.00e+00
-4.00e+00
-7.00e+00
-5.00e+00
-4.00e+00
-1.00e+00
-4.00e+00
-7.00e+00
-9.00e+00
-4.00e+00
-5.00e+00
-5.00e+00
-6.00e+00
-6.00e+00
-4.00e+00
-5.00e+00
-5.00e+00
-6.00e+00
-4.00e+00
-3.00e+00
-3.00e+00
-4.00e+00
-2.00e+00
-4.00e+00
-3.00e+00
-5.00e+00
-2.00e+00
-3.00e+00
-6.00e+00
-5.00e+00
-3.00e+00
-5.00e+00
-4.00e+00
-8.00e+00
-5.00e+00
-4.00e+00
-3.00e+00
-3.00e+00
-7.00e+00
-4.00e+00
-5.00e+00
-5.00e+00
-4.00e+00
-5.00e+00
-4.00e+00
-3.00e+00
-3.00e+00
-1.00e+00
-3.00e+00
-9.00e+00
-4.00e+00
-4.00e+00
-3.00e+00
-7.00e+00
-3.00e+00
-3.00e+00
-6.00e+00
-3.00e+00
-4.00e+00
-2.00e+00
-5.00e+00
-4.00e+00
-3.00e+00
-4.00e+00
-4.00e+00
-5.00e+00
-4.00e+00
-5.00e+00
-6.00e+00
-7.00e+00
-0.00e+00
-4.00e+00
-0.00e+00
-7.00e+00
-3.00e+00
-4.00e+00
-5.00e+00
-4.00e+00
-3.00e+00
-4.00e+00
-3.00e+00
-4.00e+00
-3.00e+00
-4.00e+00
-4.00e+00
-3.00e+00
-4.00e+00
-3.00e+00
-4.00e+00
-1.00e+01
-5.00e+00
-5.00e+00
-3.00e+00
-4.00e+00
-4.00e+00
-9.00e+00
-4.00e+00
-3.00e+00
-4.00e+00
-2.00e+00
-5.00e+00
-4.00e+00
-1.00e+01
-4.00e+00
-3.00e+00
-3.00e+00
-4.00e+00
-6.00e+00
-5.00e+00
-7.00e+00
-4.00e+00
-3.00e+00
-3.00e+00
-9.00e+00
-6.00e+00
-4.00e+00
-4.00e+00
-5.00e+00
-5.00e+00
-6.00e+00
-5.00e+00
-4.00e+00
-3.00e+00
-6.00e+00
-3.00e+00
-4.00e+00
-4.00e+00
-6.00e+00
-5.00e+00
-2.00e+00
-3.00e+00
-5.00e+00
-9.00e+00
-4.00e+00
-4.00e+00
-4.00e+00
-3.00e+00
-4.00e+00
-3.00e+00
-5.00e+00
-5.00e+00
-7.00e+00
-5.00e+00
-5.00e+00
-3.00e+00
-0.00e+00
-4.00e+00
-4.00e+00
-2.00e+00
-5.00e+00
-4.00e+00
-7.00e+00
-1.00e+01
-4.00e+00
-2.00e+00
-5.00e+00
-4.00e+00
-5.00e+00
-3.00e+00
-3.00e+00
-7.00e+00
-5.00e+00
-4.00e+00
-3.00e+00
-3.00e+00
-5.00e+00
-1.00e+00
-1.00e+01
-5.00e+00
-2.00e+00
-4.00e+00
-8.00e+00
-8.00e+00
-5.00e+00
-4.00e+00
-4.00e+00
-4.00e+00
-5.00e+00
-1.00e+00
-3.00e+00
-4.00e+00
-4.00e+00
-4.00e+00
-4.00e+00
-8.00e+00
-4.00e+00
-3.00e+00
-6.00e+00
-6.00e+00
-4.00e+00
-4.00e+00
-4.00e+00
-6.00e+00
-3.00e+00
-7.00e+00
-4.00e+00
-4.00e+00
-5.00e+00
-4.00e+00
-3.00e+00
-5.00e+00
-6.00e+00
-6.00e+00
-4.00e+00
-6.00e+00
-3.00e+00
-4.00e+00
-7.00e+00
-3.00e+00
-9.00e+00
-4.00e+00
-9.00e+00
-6.00e+00
-8.00e+00
-4.00e+00
-9.00e+00
-1.00e+01
-4.00e+00
-4.00e+00
-2.00e+00
-4.00e+00
-2.00e+00
-5.00e+00
-5.00e+00
-5.00e+00
-9.00e+00
-4.00e+00
-3.00e+00
-4.00e+00
+5.00e+00
+6.00e+00
+8.00e+00
+5.00e+00
+0.00e+00
+5.00e+00
+6.00e+00
+2.00e+00
+5.00e+00
+4.00e+00
+5.00e+00
+5.00e+00
+4.00e+00
+4.00e+00
+3.00e+00
+5.00e+00
+4.00e+00
+6.00e+00
+4.00e+00
+3.00e+00
+3.00e+00
+6.00e+00
+4.00e+00
+4.00e+00
+6.00e+00
+3.00e+00
+5.00e+00
+3.00e+00
+5.00e+00
+2.00e+00
+5.00e+00
+5.00e+00
+4.00e+00
+3.00e+00
+4.00e+00
+4.00e+00
+2.00e+00
+3.00e+00
+4.00e+00
+5.00e+00
+3.00e+00
+9.00e+00
+4.00e+00
+5.00e+00
+4.00e+00
+6.00e+00
+3.00e+00
+7.00e+00
+4.00e+00
+5.00e+00
+4.00e+00
+3.00e+00
+5.00e+00
+6.00e+00
+4.00e+00
+4.00e+00
+7.00e+00
+4.00e+00
+4.00e+00
+5.00e+00
+4.00e+00
+0.00e+00
+3.00e+00
+8.00e+00
+5.00e+00
+4.00e+00
+4.00e+00
+4.00e+00
+4.00e+00
+4.00e+00
+4.00e+00
+4.00e+00
+3.00e+00
+5.00e+00
+5.00e+00
+5.00e+00
+4.00e+00
+3.00e+00
+4.00e+00
+3.00e+00
+5.00e+00
+6.00e+00
+6.00e+00
+6.00e+00
+2.00e+00
+4.00e+00
+5.00e+00
+5.00e+00
+3.00e+00
+4.00e+00
+3.00e+00
+3.00e+00
+1.00e+00
+1.00e+01
+4.00e+00
+5.00e+00
+3.00e+00
+4.00e+00
+4.00e+00
+3.00e+00
+4.00e+00
+4.00e+00
+6.00e+00
+3.00e+00
+3.00e+00
+3.00e+00
+4.00e+00
+3.00e+00
+3.00e+00
+5.00e+00
+6.00e+00
+4.00e+00
+5.00e+00
+4.00e+00
+3.00e+00
+5.00e+00
+6.00e+00
+5.00e+00
+5.00e+00
+4.00e+00
+4.00e+00
+1.00e+00
+6.00e+00
+3.00e+00
+4.00e+00
+4.00e+00
+4.00e+00
+3.00e+00
+4.00e+00
+2.00e+00
+3.00e+00
+4.00e+00
+2.00e+00
+3.00e+00
+4.00e+00
+1.00e+01
+5.00e+00
+3.00e+00
+5.00e+00
+4.00e+00
+4.00e+00
+0.00e+00
+4.00e+00
+6.00e+00
+9.00e+00
+4.00e+00
+1.00e+01
+5.00e+00
+6.00e+00
+1.00e+01
+3.00e+00
+7.00e+00
+1.00e+00
+4.00e+00
+4.00e+00
+5.00e+00
+5.00e+00
+3.00e+00
+3.00e+00
+5.00e+00
+3.00e+00
+5.00e+00
+4.00e+00
+4.00e+00
+3.00e+00
+4.00e+00
+3.00e+00
+4.00e+00
+2.00e+00
+5.00e+00
+4.00e+00
+1.00e+01
+8.00e+00
+4.00e+00
+4.00e+00
+4.00e+00
+1.00e+01
+8.00e+00
+4.00e+00
+5.00e+00
+7.00e+00
+6.00e+00
+4.00e+00
+3.00e+00
+7.00e+00
+4.00e+00
+4.00e+00
+5.00e+00
+3.00e+00
+4.00e+00
+5.00e+00
+8.00e+00
+6.00e+00
+1.00e+01
+3.00e+00
+8.00e+00
+3.00e+00
+8.00e+00
+3.00e+00
+2.00e+00
+3.00e+00
+5.00e+00
+3.00e+00
+9.00e+00
+5.00e+00
+5.00e+00
+9.00e+00
+4.00e+00
+5.00e+00
+5.00e+00
+5.00e+00
+1.00e+01
+6.00e+00
+4.00e+00
+4.00e+00
+5.00e+00
+5.00e+00
+4.00e+00
+4.00e+00
+3.00e+00
+7.00e+00
+4.00e+00
+5.00e+00
+8.00e+00
+5.00e+00
+3.00e+00
+7.00e+00
+1.00e+01
+1.00e+01
+3.00e+00
+7.00e+00
+7.00e+00
+6.00e+00
+5.00e+00
+3.00e+00
+5.00e+00
+5.00e+00
+1.00e+01
+2.00e+00
+3.00e+00
+5.00e+00
+4.00e+00
+4.00e+00
+3.00e+00
+4.00e+00
+5.00e+00
+9.00e+00
+3.00e+00
+4.00e+00
+3.00e+00
+5.00e+00
+9.00e+00
+5.00e+00
+1.00e+00
+4.00e+00
+6.00e+00
+4.00e+00
+5.00e+00
+5.00e+00
+5.00e+00
+4.00e+00
+4.00e+00
+3.00e+00
+6.00e+00
+3.00e+00
+5.00e+00
+6.00e+00
+4.00e+00
+9.00e+00
+6.00e+00
+3.00e+00
+4.00e+00
+3.00e+00
+2.00e+00
+4.00e+00
+4.00e+00
+4.00e+00
+4.00e+00
+3.00e+00
+5.00e+00
+4.00e+00
+0.00e+00
+3.00e+00
+0.00e+00
+2.00e+00
+4.00e+00
+3.00e+00
+3.00e+00
+3.00e+00
+9.00e+00
+0.00e+00
+3.00e+00
+5.00e+00
+6.00e+00
+6.00e+00
+4.00e+00
+3.00e+00
+4.00e+00
+5.00e+00
+5.00e+00
+4.00e+00
+4.00e+00
+3.00e+00
+5.00e+00
+0.00e+00
+4.00e+00
+4.00e+00
+2.00e+00
+2.00e+00
+4.00e+00
+3.00e+00
+5.00e+00
+6.00e+00
+1.00e+01
+4.00e+00
+3.00e+00
+4.00e+00
+3.00e+00
+6.00e+00
+4.00e+00
+5.00e+00
+5.00e+00
+5.00e+00
+2.00e+00
+3.00e+00
+4.00e+00
+5.00e+00
+3.00e+00
+2.00e+00
+3.00e+00
+3.00e+00
+4.00e+00
+4.00e+00
+5.00e+00
+6.00e+00
+7.00e+00
+1.00e+01
+6.00e+00
+9.00e+00
+3.00e+00
+3.00e+00
+4.00e+00
+3.00e+00
+4.00e+00
+4.00e+00
+5.00e+00
+6.00e+00
+3.00e+00
+4.00e+00
+6.00e+00
+9.00e+00
+5.00e+00
+7.00e+00
+4.00e+00
+5.00e+00
+2.00e+00
+8.00e+00
+3.00e+00
+6.00e+00
+7.00e+00
+1.00e+00
+5.00e+00
+4.00e+00
+5.00e+00
+4.00e+00
+3.00e+00
+6.00e+00
+8.00e+00
+4.00e+00
+1.00e+01
+4.00e+00
+5.00e+00
+4.00e+00
+4.00e+00
+6.00e+00
+6.00e+00
+6.00e+00
+4.00e+00
+2.00e+00
+0.00e+00
+6.00e+00
+6.00e+00
+5.00e+00
+3.00e+00
+3.00e+00
+4.00e+00
+5.00e+00
+4.00e+00
+5.00e+00
+6.00e+00
+4.00e+00
+3.00e+00
+4.00e+00
+4.00e+00
+3.00e+00
+8.00e+00
+4.00e+00
+1.00e+00
+6.00e+00
+2.00e+00
+4.00e+00
+3.00e+00
+0.00e+00
+8.00e+00
+6.00e+00
+3.00e+00
+3.00e+00
+3.00e+00
+4.00e+00
+3.00e+00
+5.00e+00
+5.00e+00
+1.00e+01
+3.00e+00
+7.00e+00
+4.00e+00
+4.00e+00
+4.00e+00
+1.00e+01
+5.00e+00
+4.00e+00
+3.00e+00
+1.00e+00
+8.00e+00
+6.00e+00
+6.00e+00
+5.00e+00
+5.00e+00
+7.00e+00
+4.00e+00
+9.00e+00
+5.00e+00
+3.00e+00
+4.00e+00
+4.00e+00
+4.00e+00
+1.00e+01
+6.00e+00
+3.00e+00
+7.00e+00
+4.00e+00
+0.00e+00
+5.00e+00
+4.00e+00
+2.00e+00
+2.00e+00
+3.00e+00
+4.00e+00
+5.00e+00
+3.00e+00
+4.00e+00
+3.00e+00
+1.00e+01
+3.00e+00
+3.00e+00
+4.00e+00
+3.00e+00
+9.00e+00
+8.00e+00
+5.00e+00
+3.00e+00
+5.00e+00
+4.00e+00
+4.00e+00
+4.00e+00
+3.00e+00
+6.00e+00
+4.00e+00
+4.00e+00
+3.00e+00
+3.00e+00
+3.00e+00
+1.00e+01
+7.00e+00
+3.00e+00
+3.00e+00
+4.00e+00
+3.00e+00
+3.00e+00
+5.00e+00
+7.00e+00
+6.00e+00
+2.00e+00
+5.00e+00
+1.00e+00
+3.00e+00
+4.00e+00
+4.00e+00
+8.00e+00
+4.00e+00
+4.00e+00
+4.00e+00
+4.00e+00
+4.00e+00
+5.00e+00
+4.00e+00
+8.00e+00
+3.00e+00
+4.00e+00
+4.00e+00
+2.00e+00
+4.00e+00
+4.00e+00
+4.00e+00
+4.00e+00
+9.00e+00
+4.00e+00
+5.00e+00
+2.00e+00
+6.00e+00
+0.00e+00
+5.00e+00
+5.00e+00
+6.00e+00
+4.00e+00
+4.00e+00
+7.00e+00
+4.00e+00
+1.00e+00
+7.00e+00
+4.00e+00
+3.00e+00
+4.00e+00
+4.00e+00
+3.00e+00
+5.00e+00
+3.00e+00
+4.00e+00
+4.00e+00
+4.00e+00
+3.00e+00
+4.00e+00
+5.00e+00
+4.00e+00
+3.00e+00
+4.00e+00
+4.00e+00
+4.00e+00
+4.00e+00
+5.00e+00
+4.00e+00
+3.00e+00
+1.00e+01
+4.00e+00
+5.00e+00
+5.00e+00
+1.00e+00
+4.00e+00
+4.00e+00
+5.00e+00
+4.00e+00
+9.00e+00
+5.00e+00
+4.00e+00
+2.00e+00
+5.00e+00
+6.00e+00
+4.00e+00
+4.00e+00
+1.00e+01
+4.00e+00
+9.00e+00
+4.00e+00
+3.00e+00
+5.00e+00
+4.00e+00
+1.00e+00
+9.00e+00
+1.00e+00
+5.00e+00
+3.00e+00
+8.00e+00
+4.00e+00
+0.00e+00
+6.00e+00
+2.00e+00
+5.00e+00
+2.00e+00
+6.00e+00
+4.00e+00
+4.00e+00
+9.00e+00
+5.00e+00
+4.00e+00
+5.00e+00
+5.00e+00
+4.00e+00
+4.00e+00
+5.00e+00
+4.00e+00
+8.00e+00
+4.00e+00
+6.00e+00
+4.00e+00
+3.00e+00
+4.00e+00
+4.00e+00
+4.00e+00
+5.00e+00
+4.00e+00
+5.00e+00
+4.00e+00
+4.00e+00
+5.00e+00
+1.00e+00
+3.00e+00
+5.00e+00
+5.00e+00
+2.00e+00
+4.00e+00
+4.00e+00
+1.00e+01
+3.00e+00
+4.00e+00
+4.00e+00
+5.00e+00
+4.00e+00
+4.00e+00
+4.00e+00
+9.00e+00
+5.00e+00
+5.00e+00
+5.00e+00
+5.00e+00
+3.00e+00
+3.00e+00
+3.00e+00
+5.00e+00
+4.00e+00
+1.00e+00
+6.00e+00
+4.00e+00
+4.00e+00
+7.00e+00
+3.00e+00
+2.00e+00
+3.00e+00
+5.00e+00
+3.00e+00
+5.00e+00
+5.00e+00
+6.00e+00
+3.00e+00
+4.00e+00
+4.00e+00
+3.00e+00
+6.00e+00
+6.00e+00
+4.00e+00
+3.00e+00
+0.00e+00
+4.00e+00
+3.00e+00
+7.00e+00
+4.00e+00
+5.00e+00
+4.00e+00
+5.00e+00
+1.00e+00
+4.00e+00
+8.00e+00
+5.00e+00
+3.00e+00
+5.00e+00
+6.00e+00
+5.00e+00
+5.00e+00
+5.00e+00
+4.00e+00
+3.00e+00
+5.00e+00
+8.00e+00
+4.00e+00
+2.00e+00
+4.00e+00
+4.00e+00
+4.00e+00
+4.00e+00
+4.00e+00
+4.00e+00
+6.00e+00
+7.00e+00
+5.00e+00
+4.00e+00
+4.00e+00
+4.00e+00
+2.00e+00
+6.00e+00
+9.00e+00
+5.00e+00
+5.00e+00
+4.00e+00
+4.00e+00
+6.00e+00
+4.00e+00
+3.00e+00
+5.00e+00
+5.00e+00
+6.00e+00
+4.00e+00
+6.00e+00
+4.00e+00
+4.00e+00
+4.00e+00
+8.00e+00
+7.00e+00
+3.00e+00
+4.00e+00
+4.00e+00
+3.00e+00
+5.00e+00
+4.00e+00
+4.00e+00
+3.00e+00
+3.00e+00
+4.00e+00
+4.00e+00
+3.00e+00
+3.00e+00
+1.00e+00
+9.00e+00
+3.00e+00
+4.00e+00
+7.00e+00
+1.00e+01
+3.00e+00
+4.00e+00
+5.00e+00
+2.00e+00
+5.00e+00
+3.00e+00
+5.00e+00
+1.00e+01
+8.00e+00
+7.00e+00
+4.00e+00
+3.00e+00
+3.00e+00
+4.00e+00
+2.00e+00
+4.00e+00
+5.00e+00
+3.00e+00
+3.00e+00
+4.00e+00
+9.00e+00
+5.00e+00
+4.00e+00
+0.00e+00
+4.00e+00
+4.00e+00
+5.00e+00
+4.00e+00
+5.00e+00
+5.00e+00
+5.00e+00
+4.00e+00
+4.00e+00
+4.00e+00
+4.00e+00
+5.00e+00
+1.00e+01
+5.00e+00
+3.00e+00
+4.00e+00
+5.00e+00
+4.00e+00
+4.00e+00
+4.00e+00
+5.00e+00
+4.00e+00
+3.00e+00
+4.00e+00
+3.00e+00
+7.00e+00
+6.00e+00
+8.00e+00
+3.00e+00
+5.00e+00
+6.00e+00
+4.00e+00
+3.00e+00
+4.00e+00
+4.00e+00
+7.00e+00
+4.00e+00
+3.00e+00
+4.00e+00
+4.00e+00
+3.00e+00
+4.00e+00
+8.00e+00
+9.00e+00
+6.00e+00
+7.00e+00
+4.00e+00
+3.00e+00
+3.00e+00
+4.00e+00
+2.00e+00
+2.00e+00
+4.00e+00
+8.00e+00
+4.00e+00
+5.00e+00
+0.00e+00
+3.00e+00
+0.00e+00
+3.00e+00
+5.00e+00
+4.00e+00
+3.00e+00
+4.00e+00
+3.00e+00
+3.00e+00
+3.00e+00
+1.00e+01
+3.00e+00
+6.00e+00
+6.00e+00
+7.00e+00
+5.00e+00
+5.00e+00
+7.00e+00
+7.00e+00
+2.00e+00
+4.00e+00
+5.00e+00
+3.00e+00
+6.00e+00
+5.00e+00
+5.00e+00
+6.00e+00
+4.00e+00
+6.00e+00
+4.00e+00
+4.00e+00
+3.00e+00
+6.00e+00
+1.00e+01
+5.00e+00
+4.00e+00
+4.00e+00
+5.00e+00
+6.00e+00
+4.00e+00
+6.00e+00
+3.00e+00
+4.00e+00
+5.00e+00
+7.00e+00
+4.00e+00
+4.00e+00
+4.00e+00
+6.00e+00
+5.00e+00
+3.00e+00
+4.00e+00
+6.00e+00
+2.00e+00
+3.00e+00
+4.00e+00
+4.00e+00
+4.00e+00
+6.00e+00
+0.00e+00
+9.00e+00
+3.00e+00
+3.00e+00
+4.00e+00
+5.00e+00
+4.00e+00
+3.00e+00
+5.00e+00
+9.00e+00
+4.00e+00
+2.00e+00
+7.00e+00
+2.00e+00
+4.00e+00
+6.00e+00
+4.00e+00
+4.00e+00
+4.00e+00
+5.00e+00
+3.00e+00
+8.00e+00
+5.00e+00
+4.00e+00
+4.00e+00
+4.00e+00
+3.00e+00
+5.00e+00
+1.00e+00
+7.00e+00
+4.00e+00
+3.00e+00
+8.00e+00
+5.00e+00
+3.00e+00
+4.00e+00
+6.00e+00
+3.00e+00
+6.00e+00
+4.00e+00
+7.00e+00
+5.00e+00
+4.00e+00
+1.00e+00
+4.00e+00
+7.00e+00
+9.00e+00
+4.00e+00
+5.00e+00
+5.00e+00
+6.00e+00
+6.00e+00
+4.00e+00
+5.00e+00
+5.00e+00
+6.00e+00
+4.00e+00
+3.00e+00
+3.00e+00
+4.00e+00
+2.00e+00
+4.00e+00
+3.00e+00
+5.00e+00
+2.00e+00
+3.00e+00
+6.00e+00
+5.00e+00
+3.00e+00
+5.00e+00
+4.00e+00
+8.00e+00
+5.00e+00
+4.00e+00
+3.00e+00
+3.00e+00
+7.00e+00
+4.00e+00
+5.00e+00
+5.00e+00
+4.00e+00
+5.00e+00
+4.00e+00
+3.00e+00
+3.00e+00
+1.00e+00
+3.00e+00
+9.00e+00
+4.00e+00
+4.00e+00
+3.00e+00
+7.00e+00
+3.00e+00
+3.00e+00
+6.00e+00
+3.00e+00
+4.00e+00
+2.00e+00
+5.00e+00
+4.00e+00
+3.00e+00
+4.00e+00
+4.00e+00
+5.00e+00
+4.00e+00
+5.00e+00
+6.00e+00
+7.00e+00
+0.00e+00
+4.00e+00
+0.00e+00
+7.00e+00
+3.00e+00
+4.00e+00
+5.00e+00
+4.00e+00
+3.00e+00
+4.00e+00
+3.00e+00
+4.00e+00
+3.00e+00
+4.00e+00
+4.00e+00
+3.00e+00
+4.00e+00
+3.00e+00
+4.00e+00
+1.00e+01
+5.00e+00
+5.00e+00
+3.00e+00
+4.00e+00
+4.00e+00
+9.00e+00
+4.00e+00
+3.00e+00
+4.00e+00
+2.00e+00
+5.00e+00
+4.00e+00
+1.00e+01
+4.00e+00
+3.00e+00
+3.00e+00
+4.00e+00
+6.00e+00
+5.00e+00
+7.00e+00
+4.00e+00
+3.00e+00
+3.00e+00
+9.00e+00
+6.00e+00
+4.00e+00
+4.00e+00
+5.00e+00
+5.00e+00
+6.00e+00
+5.00e+00
+4.00e+00
+3.00e+00
+6.00e+00
+3.00e+00
+4.00e+00
+4.00e+00
+6.00e+00
+5.00e+00
+2.00e+00
+3.00e+00
+5.00e+00
+9.00e+00
+4.00e+00
+4.00e+00
+4.00e+00
+3.00e+00
+4.00e+00
+3.00e+00
+5.00e+00
+5.00e+00
+7.00e+00
+5.00e+00
+5.00e+00
+3.00e+00
+0.00e+00
+4.00e+00
+4.00e+00
+2.00e+00
+5.00e+00
+4.00e+00
+7.00e+00
+1.00e+01
+4.00e+00
+2.00e+00
+5.00e+00
+4.00e+00
+5.00e+00
+3.00e+00
+3.00e+00
+7.00e+00
+5.00e+00
+4.00e+00
+3.00e+00
+3.00e+00
+5.00e+00
+1.00e+00
+1.00e+01
+5.00e+00
+2.00e+00
+4.00e+00
+8.00e+00
+8.00e+00
+5.00e+00
+4.00e+00
+4.00e+00
+4.00e+00
+5.00e+00
+1.00e+00
+3.00e+00
+4.00e+00
+4.00e+00
+4.00e+00
+4.00e+00
+8.00e+00
+4.00e+00
+3.00e+00
+6.00e+00
+6.00e+00
+4.00e+00
+4.00e+00
+4.00e+00
+6.00e+00
+3.00e+00
+7.00e+00
+4.00e+00
+4.00e+00
+5.00e+00
+4.00e+00
+3.00e+00
+5.00e+00
+6.00e+00
+6.00e+00
+4.00e+00
+6.00e+00
+3.00e+00
+4.00e+00
+7.00e+00
+3.00e+00
+9.00e+00
+4.00e+00
+9.00e+00
+6.00e+00
+8.00e+00
+4.00e+00
+9.00e+00
+1.00e+01
+4.00e+00
+4.00e+00
+2.00e+00
+4.00e+00
+2.00e+00
+5.00e+00
+5.00e+00
+5.00e+00
+9.00e+00
+4.00e+00
+3.00e+00
+4.00e+00
```

### Comparing `nanite-3.5.4/nanite/read.py` & `nanite-3.6.0/nanite/read.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,111 +1,111 @@
-import warnings
-
-import afmformats
-from .indent import Indentation
-
-#: The default imaging modality when loading AFM data. Set this to `None`
-#: to also be able to load e.g. creep-compliance data. See issue
-#: https://github.com/AFM-analysis/nanite/issues/11 for more
-#: information. Note that especially the export of rating containers
-#: may not work with any imaging modality other than force-distance.
-DEFAULT_MODALITY = "force-distance"
-
-
-def get_data_paths(path):
-    """Return list of data paths with force-distance data
-
-    DEPRECATED
-    """
-    warnings.warn("`get_data_paths` is deprecated! Please use "
-                  + "afmformats.find_data(path, modality='force-distance') "
-                  + "instead!",
-                  DeprecationWarning)
-    return afmformats.find_data(path, modality=DEFAULT_MODALITY)
-
-
-def get_data_paths_enum(path, skip_errors=False):
-    """Return a list with paths and their internal enumeration
-
-    Parameters
-    ----------
-    path: str or pathlib.Path or list of str or list of pathlib.Path
-        path to data files or directory containing data files;
-        if directories are given, they are searched recursively
-    skip_errors: bool
-        skip paths that raise errors
-
-    Returns
-    -------
-    path_enum: list of lists
-        each entry in the list is a list of [pathlib.Path, int],
-        enumerating all curves in each file
-    """
-    paths = afmformats.find_data(path, modality=DEFAULT_MODALITY)
-    enumpaths = []
-    for pp in paths:
-        try:
-            data = load_data(pp)
-        except BaseException:
-            if skip_errors:
-                continue
-            else:
-                raise
-        for dd in data:
-            enumpaths.append([pp, dd.enum])
-    return enumpaths
-
-
-def get_load_data_modality_kwargs():
-    """Return imaging modality kwargs for afmformats.load_data
-
-    Uses :const:`DEFAULT_MODALITY`.
-
-    Returns
-    -------
-    kwargs: dict
-        keyword arguments for :func:`afmformats.load_data`
-    """
-    kwargs = {
-        "modality": DEFAULT_MODALITY,
-        "data_classes_by_modality": {
-            "force-distance": Indentation,
-            "creep-compliance": Indentation,
-            "stress-relaxation": Indentation}
-    }
-    return kwargs
-
-
-def load_data(path, callback=None, meta_override=None):
-    """Load data and return list of :class:`afmformats.AFMForceDistance`
-
-    This is essentially a wrapper around
-    :func:`afmformats.formats.find_data` and
-    :func:`afmformats.formats.load_data` that returns
-    force-distance datasets.
-
-    Parameters
-    ----------
-    path: str or pathlib.Path or list of str or list of pathlib.Path
-        path to data files or directory containing data files;
-        if directories are given, they are searched recursively
-    callback: callable
-        function for progress tracking; must accept a float in
-        [0, 1] as an argument.
-    meta_override: dict
-        if specified, contains key-value pairs of metadata that
-        are used when loading the files
-        (see :data:`afmformats.meta.META_FIELDS`)
-    """
-    paths = afmformats.find_data(path, modality=DEFAULT_MODALITY)
-    data = []
-    for ii, pp in enumerate(paths):
-        measurements = afmformats.load_data(
-            pp,
-            # recurse callback function with None as default
-            callback=lambda x: callback((ii + x) / len(paths))
-            if callback else None,
-            meta_override=meta_override,
-            **get_load_data_modality_kwargs()
-        )
-        data += measurements
-    return data
+import warnings
+
+import afmformats
+from .indent import Indentation
+
+#: The default imaging modality when loading AFM data. Set this to `None`
+#: to also be able to load e.g. creep-compliance data. See issue
+#: https://github.com/AFM-analysis/nanite/issues/11 for more
+#: information. Note that especially the export of rating containers
+#: may not work with any imaging modality other than force-distance.
+DEFAULT_MODALITY = "force-distance"
+
+
+def get_data_paths(path):
+    """Return list of data paths with force-distance data
+
+    DEPRECATED
+    """
+    warnings.warn("`get_data_paths` is deprecated! Please use "
+                  + "afmformats.find_data(path, modality='force-distance') "
+                  + "instead!",
+                  DeprecationWarning)
+    return afmformats.find_data(path, modality=DEFAULT_MODALITY)
+
+
+def get_data_paths_enum(path, skip_errors=False):
+    """Return a list with paths and their internal enumeration
+
+    Parameters
+    ----------
+    path: str or pathlib.Path or list of str or list of pathlib.Path
+        path to data files or directory containing data files;
+        if directories are given, they are searched recursively
+    skip_errors: bool
+        skip paths that raise errors
+
+    Returns
+    -------
+    path_enum: list of lists
+        each entry in the list is a list of [pathlib.Path, int],
+        enumerating all curves in each file
+    """
+    paths = afmformats.find_data(path, modality=DEFAULT_MODALITY)
+    enumpaths = []
+    for pp in paths:
+        try:
+            data = load_data(pp)
+        except BaseException:
+            if skip_errors:
+                continue
+            else:
+                raise
+        for dd in data:
+            enumpaths.append([pp, dd.enum])
+    return enumpaths
+
+
+def get_load_data_modality_kwargs():
+    """Return imaging modality kwargs for afmformats.load_data
+
+    Uses :const:`DEFAULT_MODALITY`.
+
+    Returns
+    -------
+    kwargs: dict
+        keyword arguments for :func:`afmformats.load_data`
+    """
+    kwargs = {
+        "modality": DEFAULT_MODALITY,
+        "data_classes_by_modality": {
+            "force-distance": Indentation,
+            "creep-compliance": Indentation,
+            "stress-relaxation": Indentation}
+    }
+    return kwargs
+
+
+def load_data(path, callback=None, meta_override=None):
+    """Load data and return list of :class:`afmformats.AFMForceDistance`
+
+    This is essentially a wrapper around
+    :func:`afmformats.formats.find_data` and
+    :func:`afmformats.formats.load_data` that returns
+    force-distance datasets.
+
+    Parameters
+    ----------
+    path: str or pathlib.Path or list of str or list of pathlib.Path
+        path to data files or directory containing data files;
+        if directories are given, they are searched recursively
+    callback: callable
+        function for progress tracking; must accept a float in
+        [0, 1] as an argument.
+    meta_override: dict
+        if specified, contains key-value pairs of metadata that
+        are used when loading the files
+        (see :data:`afmformats.meta.META_FIELDS`)
+    """
+    paths = afmformats.find_data(path, modality=DEFAULT_MODALITY)
+    data = []
+    for ii, pp in enumerate(paths):
+        measurements = afmformats.load_data(
+            pp,
+            # recurse callback function with None as default
+            callback=lambda x: callback((ii + x) / len(paths))
+            if callback else None,
+            meta_override=meta_override,
+            **get_load_data_modality_kwargs()
+        )
+        data += measurements
+    return data
```

### Comparing `nanite-3.5.4/nanite/smooth.py` & `nanite-3.6.0/nanite/smooth.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,83 +1,83 @@
-"""smooth data"""
-import warnings
-
-import numpy as np
-import scipy.ndimage as im
-
-
-class DoubledSmoothingWindowWarning(UserWarning):
-    pass
-
-
-def smooth_axis(data, window=15):
-    """
-    Smooth a 1D  data array with a median filter of `width`.
-
-    See Also
-    --------
-    smooth_axis_monotone
-    """
-    smooth = im.median_filter(data, size=(window,), mode="nearest")
-    return smooth
-
-
-def smooth_axis_monotone(data, window=15, max_iter=1000):
-    """
-    Smooth a 1D  data array with a median filter of `width`.
-    This method makes sure that the data is monotonously
-    increasing or decreasing, by increasing the window
-    size automatically. If this happens, a
-    :class:`DoubledSmoothingWindowWarning` is raised.
-
-    Window should be an odd number.
-
-    See Also
-    --------
-    smooth_axis
-    """
-    smooth = smooth_axis(data, window=window)
-    gradient = np.gradient(smooth)
-
-    for _ in range(max_iter):
-        if np.abs(np.sum(gradient)) == np.sum(np.abs(gradient)):
-            break
-        window = window * 2 + 1
-        smooth = smooth_axis(data, window=window)
-        gradient = np.gradient(smooth)
-        warnings.warn("Automatically doubled smoothing `window` size to "
-                      + "{}. You might consider using a ".format(window)
-                      + "larger value by default.",
-                      DoubledSmoothingWindowWarning)
-    else:
-        raise ValueError("Reached `max_iter`={}".format(max_iter))
-
-    for _ in range(max_iter):
-        if np.unique(smooth).size == smooth.size:
-            break
-        # Keep axis monotonous.
-        # get the first element with equal values
-        equal = []
-        myset = False
-        for ii in range(smooth.size):
-            if smooth[ii+1] == smooth[ii]:
-                equal.append(ii+1)
-                myset = True
-            elif myset is True:
-                # continue with these values in the next for-loop
-                break
-            if smooth.size == ii+2:
-                # abort
-                break
-
-        for count, idx in enumerate(equal):
-            try:
-                smooth[idx] += (smooth[equal[-1]+1] -
-                                smooth[equal[0]])/(len(equal)+5)*(count+1)
-            except BaseException:
-                # we have last element
-                dx = (smooth[1]-smooth[0])/10
-                smooth[-1] += dx
-    else:
-        raise ValueError("Reached `max_iter`={}".format(max_iter))
-
-    return smooth
+"""smooth data"""
+import warnings
+
+import numpy as np
+import scipy.ndimage as im
+
+
+class DoubledSmoothingWindowWarning(UserWarning):
+    pass
+
+
+def smooth_axis(data, window=15):
+    """
+    Smooth a 1D  data array with a median filter of `width`.
+
+    See Also
+    --------
+    smooth_axis_monotone
+    """
+    smooth = im.median_filter(data, size=(window,), mode="nearest")
+    return smooth
+
+
+def smooth_axis_monotone(data, window=15, max_iter=1000):
+    """
+    Smooth a 1D  data array with a median filter of `width`.
+    This method makes sure that the data is monotonously
+    increasing or decreasing, by increasing the window
+    size automatically. If this happens, a
+    :class:`DoubledSmoothingWindowWarning` is raised.
+
+    Window should be an odd number.
+
+    See Also
+    --------
+    smooth_axis
+    """
+    smooth = smooth_axis(data, window=window)
+    gradient = np.gradient(smooth)
+
+    for _ in range(max_iter):
+        if np.abs(np.sum(gradient)) == np.sum(np.abs(gradient)):
+            break
+        window = window * 2 + 1
+        smooth = smooth_axis(data, window=window)
+        gradient = np.gradient(smooth)
+        warnings.warn("Automatically doubled smoothing `window` size to "
+                      + "{}. You might consider using a ".format(window)
+                      + "larger value by default.",
+                      DoubledSmoothingWindowWarning)
+    else:
+        raise ValueError("Reached `max_iter`={}".format(max_iter))
+
+    for _ in range(max_iter):
+        if np.unique(smooth).size == smooth.size:
+            break
+        # Keep axis monotonous.
+        # get the first element with equal values
+        equal = []
+        myset = False
+        for ii in range(smooth.size):
+            if smooth[ii+1] == smooth[ii]:
+                equal.append(ii+1)
+                myset = True
+            elif myset is True:
+                # continue with these values in the next for-loop
+                break
+            if smooth.size == ii+2:
+                # abort
+                break
+
+        for count, idx in enumerate(equal):
+            try:
+                smooth[idx] += (smooth[equal[-1]+1] -
+                                smooth[equal[0]])/(len(equal)+5)*(count+1)
+            except BaseException:
+                # we have last element
+                dx = (smooth[1]-smooth[0])/10
+                smooth[-1] += dx
+    else:
+        raise ValueError("Reached `max_iter`={}".format(max_iter))
+
+    return smooth
```

### Comparing `nanite-3.5.4/nanite.egg-info/PKG-INFO` & `nanite-3.6.0/nanite.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,52 @@
-Metadata-Version: 2.1
-Name: nanite
-Version: 3.5.4
-Summary: Loading, fitting, and rating AFM force-distance data
-Home-page: https://github.com/AFM-analysis/nanite
-Maintainer: Paul Müller
-Maintainer-email: dev@craban.de
-License: GPL v3
-Description: nanite
-        ======
-        
-        |PyPI Version| |Build Status| |Coverage Status| |Docs Status|
-        
-        Loading, fitting, and rating AFM force-distance data.
-        
-        Documentation
-        -------------
-        
-        The documentation, including the code reference and examples, is available at
-        `nanite.readthedocs.io <https://nanite.readthedocs.io/en/stable/>`__.
-        
-        
-        Installation
-        ------------
-        To install the latest release, simply run:
-        
-        ::
-        
-            pip install nanite[CLI]
-        
-        
-        .. |PyPI Version| image:: https://img.shields.io/pypi/v/nanite.svg
-           :target: https://pypi.python.org/pypi/nanite
-        .. |Build Status| image:: https://img.shields.io/github/actions/workflow/status/AFM-analysis/nanite/check.yml
-           :target: https://github.com/AFM-analysis/nanite/actions?query=workflow%3AChecks
-        .. |Coverage Status| image:: https://img.shields.io/codecov/c/github/AFM-analysis/nanite/master.svg
-           :target: https://codecov.io/gh/AFM-analysis/nanite
-        .. |Docs Status| image:: https://readthedocs.org/projects/nanite/badge/?version=latest
-           :target: https://readthedocs.org/projects/nanite/builds/
-        
-Keywords: atomic force microscopy,mechanical phenotyping,tissue analysis
-Platform: ALL
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Scientific/Engineering :: Visualization
-Classifier: Intended Audience :: Science/Research
-Requires-Python: >=3.8, <4
-Provides-Extra: CLI
+Metadata-Version: 2.1
+Name: nanite
+Version: 3.6.0
+Summary: Loading, fitting, and rating AFM force-distance data
+Author: Paul Müller, Shada Abuhattum
+Maintainer-email: Paul Müller <dev@craban.de>
+License: GPL version 3
+Project-URL: source, https://github.com/AFM-Analysis/nanite
+Project-URL: tracker, https://github.com/AFM-Analysis/nanite/issues
+Project-URL: documentation, https://nanite.readthedocs.io/en/stable/
+Project-URL: changelog, https://nanite.readthedocs.io/en/stable/sec_changelog.html
+Keywords: atomic force microscopy,mechanical phenotyping,tissue analysis
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering :: Visualization
+Classifier: Intended Audience :: Science/Research
+Requires-Python: <4,>=3.10
+Description-Content-Type: text/x-rst
+Provides-Extra: CLI
+License-File: LICENSE
+
+nanite
+======
+
+|PyPI Version| |Build Status| |Coverage Status| |Docs Status|
+
+Loading, fitting, and rating AFM force-distance data.
+
+Documentation
+-------------
+
+The documentation, including the code reference and examples, is available at
+`nanite.readthedocs.io <https://nanite.readthedocs.io/en/stable/>`__.
+
+
+Installation
+------------
+To install the latest release, simply run:
+
+::
+
+    pip install nanite[CLI]
+
+
+.. |PyPI Version| image:: https://img.shields.io/pypi/v/nanite.svg
+   :target: https://pypi.python.org/pypi/nanite
+.. |Build Status| image:: https://img.shields.io/github/actions/workflow/status/AFM-analysis/nanite/check.yml
+   :target: https://github.com/AFM-analysis/nanite/actions?query=workflow%3AChecks
+.. |Coverage Status| image:: https://img.shields.io/codecov/c/github/AFM-analysis/nanite/master.svg
+   :target: https://codecov.io/gh/AFM-analysis/nanite
+.. |Docs Status| image:: https://readthedocs.org/projects/nanite/badge/?version=latest
+   :target: https://readthedocs.org/projects/nanite/builds/
```

### Comparing `nanite-3.5.4/tests/common.py` & `nanite-3.6.0/tests/common.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,126 +1,126 @@
-import lmfit
-import nanite
-import nanite.model.logic
-from nanite.model import residuals
-import numpy as np
-
-
-class MockModelModule:
-    def __init__(self, model_key, **kwargs):
-        super(MockModelModule, self).__init__()
-        # rebase on hertz model
-        md = nanite.model.models_available["hertz_para"].module
-        for akey in dir(md):
-            setattr(self, akey, getattr(md, akey))
-        for kw in kwargs:
-            setattr(self, kw, kwargs[kw])
-        self.model_key = model_key
-
-    def __enter__(self):
-        return nanite.model.logic.register_model(self)
-
-    def __exit__(self, a, b, c):
-        nanite.model.models_available.pop(self.model_key)
-
-
-class MockModelModuleExpr:
-    def __init__(self, **kwargs):
-        """E and E1 add up to the actual emodulus. E1 is varied indirectly"""
-        self.model_doc = """Mock model with constraint"""
-        self.model_func = MockModelModuleExpr.hertz_constraint
-        self.model_key = "hertz_constraint"
-        self.model_name = "Hertz with constraint "
-        self.parameter_keys = ["E", "R", "nu", "virtual_parameter",
-                               "E1", "contact_point", "baseline"]
-        self.parameter_names = ["Young's Modulus", "Tip Radius",
-                                "Poisson's Ratio", "Virtual Parameter",
-                                "Another Modulus", "Contact Point",
-                                "Force Baseline"]
-        self.parameter_units = ["Pa", "m", "", "Pa", "Pa", "m", "N"]
-        self.valid_axes_x = ["tip position"]
-        self.valid_axes_y = ["force"]
-
-    def __enter__(self):
-        nanite.model.logic.register_model(self)
-        return self
-
-    def __exit__(self, a, b, c):
-        nanite.model.logic.deregister_model(self)
-
-    @staticmethod
-    def get_parameter_defaults():
-        # The order of the parameters must match the order
-        # of ´parameter_names´ and ´parameter_keys´.
-        params = lmfit.Parameters()
-        params.add("E", value=1e3, min=0, vary=False)
-        params.add("R", value=10e-6, vary=False)
-        params.add("nu", value=.5, vary=False)
-        params.add("virtual_parameter", value=10, min=0, vary=True)
-        params.add("E1", expr="virtual_parameter+E")
-        params.add("contact_point", value=0)
-        params.add("baseline", value=0)
-        return params
-
-    @staticmethod
-    def hertz_constraint(delta, E, R, nu, virtual_parameter, E1,
-                         contact_point=0, baseline=0):
-        aa1 = 4 / 3 * E1 / (1 - nu ** 2) * np.sqrt(R)
-
-        root = contact_point - delta
-        pos = root > 0
-        bb = np.zeros_like(delta)
-        bb[pos] = (root[pos]) ** (3 / 2)
-        cc = np.zeros_like(delta)
-        cc[pos] = 1 - 0.15 * root[pos] / R
-        return aa1 * bb * cc + baseline
-
-    @staticmethod
-    def model(params, x):
-        if x[0] < x[-1]:
-            revert = True
-        else:
-            revert = False
-        if revert:
-            x = x[::-1]
-        mf = MockModelModuleExpr.hertz_constraint(
-            E=params["E"].value,
-            delta=x,
-            R=params["R"].value,
-            nu=params["nu"].value,
-            virtual_parameter=params["virtual_parameter"].value,
-            E1=params["E1"].value,
-            contact_point=params["contact_point"].value,
-            baseline=params["baseline"].value)
-        if revert:
-            return mf[::-1]
-        return mf
-
-    @staticmethod
-    def residual(params, delta, force, weight_cp=5e-7):
-        """ Compute residuals for fitting
-
-        Parameters
-        ----------
-        params: lmfit.Parameters
-            The fitting parameters for `model`
-        delta: 1D ndarray of lenght M
-            The indentation distances
-        force: 1D ndarray of length M
-            The corresponding force data
-        weight_cp: positive float or zero/False
-            The distance from the contact point until which
-            linear weights will be applied. Set to zero to
-            disable weighting.
-        """
-        md = MockModelModuleExpr.model(params, delta)
-        resid = force - md
-
-        if weight_cp:
-            # weight the curve so that the data around the contact_point do
-            # not affect the fit so much.
-            weights = residuals.compute_contact_point_weights(
-                cp=params["contact_point"].value,
-                delta=delta,
-                weight_dist=weight_cp)
-            resid *= weights
-        return resid
+import lmfit
+import nanite
+import nanite.model.logic
+from nanite.model import residuals
+import numpy as np
+
+
+class MockModelModule:
+    def __init__(self, model_key, **kwargs):
+        super(MockModelModule, self).__init__()
+        # rebase on hertz model
+        md = nanite.model.models_available["hertz_para"].module
+        for akey in dir(md):
+            setattr(self, akey, getattr(md, akey))
+        for kw in kwargs:
+            setattr(self, kw, kwargs[kw])
+        self.model_key = model_key
+
+    def __enter__(self):
+        return nanite.model.logic.register_model(self)
+
+    def __exit__(self, a, b, c):
+        nanite.model.models_available.pop(self.model_key)
+
+
+class MockModelModuleExpr:
+    def __init__(self, **kwargs):
+        """E and E1 add up to the actual emodulus. E1 is varied indirectly"""
+        self.model_doc = """Mock model with constraint"""
+        self.model_func = MockModelModuleExpr.hertz_constraint
+        self.model_key = "hertz_constraint"
+        self.model_name = "Hertz with constraint "
+        self.parameter_keys = ["E", "R", "nu", "virtual_parameter",
+                               "E1", "contact_point", "baseline"]
+        self.parameter_names = ["Young's Modulus", "Tip Radius",
+                                "Poisson's Ratio", "Virtual Parameter",
+                                "Another Modulus", "Contact Point",
+                                "Force Baseline"]
+        self.parameter_units = ["Pa", "m", "", "Pa", "Pa", "m", "N"]
+        self.valid_axes_x = ["tip position"]
+        self.valid_axes_y = ["force"]
+
+    def __enter__(self):
+        nanite.model.logic.register_model(self)
+        return self
+
+    def __exit__(self, a, b, c):
+        nanite.model.logic.deregister_model(self)
+
+    @staticmethod
+    def get_parameter_defaults():
+        # The order of the parameters must match the order
+        # of ´parameter_names´ and ´parameter_keys´.
+        params = lmfit.Parameters()
+        params.add("E", value=1e3, min=0, vary=False)
+        params.add("R", value=10e-6, vary=False)
+        params.add("nu", value=.5, vary=False)
+        params.add("virtual_parameter", value=10, min=0, vary=True)
+        params.add("E1", expr="virtual_parameter+E")
+        params.add("contact_point", value=0)
+        params.add("baseline", value=0)
+        return params
+
+    @staticmethod
+    def hertz_constraint(delta, E, R, nu, virtual_parameter, E1,
+                         contact_point=0, baseline=0):
+        aa1 = 4 / 3 * E1 / (1 - nu ** 2) * np.sqrt(R)
+
+        root = contact_point - delta
+        pos = root > 0
+        bb = np.zeros_like(delta)
+        bb[pos] = (root[pos]) ** (3 / 2)
+        cc = np.zeros_like(delta)
+        cc[pos] = 1 - 0.15 * root[pos] / R
+        return aa1 * bb * cc + baseline
+
+    @staticmethod
+    def model(params, x):
+        if x[0] < x[-1]:
+            revert = True
+        else:
+            revert = False
+        if revert:
+            x = x[::-1]
+        mf = MockModelModuleExpr.hertz_constraint(
+            E=params["E"].value,
+            delta=x,
+            R=params["R"].value,
+            nu=params["nu"].value,
+            virtual_parameter=params["virtual_parameter"].value,
+            E1=params["E1"].value,
+            contact_point=params["contact_point"].value,
+            baseline=params["baseline"].value)
+        if revert:
+            return mf[::-1]
+        return mf
+
+    @staticmethod
+    def residual(params, delta, force, weight_cp=5e-7):
+        """ Compute residuals for fitting
+
+        Parameters
+        ----------
+        params: lmfit.Parameters
+            The fitting parameters for `model`
+        delta: 1D ndarray of lenght M
+            The indentation distances
+        force: 1D ndarray of length M
+            The corresponding force data
+        weight_cp: positive float or zero/False
+            The distance from the contact point until which
+            linear weights will be applied. Set to zero to
+            disable weighting.
+        """
+        md = MockModelModuleExpr.model(params, delta)
+        resid = force - md
+
+        if weight_cp:
+            # weight the curve so that the data around the contact_point do
+            # not affect the fit so much.
+            weights = residuals.compute_contact_point_weights(
+                cp=params["contact_point"].value,
+                delta=delta,
+                weight_dist=weight_cp)
+            resid *= weights
+        return resid
```

### Comparing `nanite-3.5.4/tests/data/fmt-jpk-cl_calibration_force-save-2015-02-04.jpk-force` & `nanite-3.6.0/tests/data/fmt-jpk-cl_calibration_force-save-2015-02-04.jpk-force`

 * *Files identical despite different names*

### Comparing `nanite-3.5.4/tests/data/fmt-jpk-fd_flipsign_2015.05.22-15.31.49.352.jpk-force` & `nanite-3.6.0/tests/data/fmt-jpk-fd_flipsign_2015.05.22-15.31.49.352.jpk-force`

 * *Files identical despite different names*

### Comparing `nanite-3.5.4/tests/data/fmt-jpk-fd_map-data-reference-points.jpk-force-map` & `nanite-3.6.0/tests/data/fmt-jpk-fd_map-data-reference-points.jpk-force-map`

 * *Files identical despite different names*

### Comparing `nanite-3.5.4/tests/data/fmt-jpk-fd_map0d_extracted.jpk-force-map` & `nanite-3.6.0/tests/data/fmt-jpk-fd_map0d_extracted.jpk-force-map`

 * *Files identical despite different names*

### Comparing `nanite-3.5.4/tests/data/fmt-jpk-fd_map1d_2016-11-07.jpk-force-map` & `nanite-3.6.0/tests/data/fmt-jpk-fd_map1d_2016-11-07.jpk-force-map`

 * *Files identical despite different names*

### Comparing `nanite-3.5.4/tests/data/fmt-jpk-fd_map2x2_extracted.jpk-force-map` & `nanite-3.6.0/tests/data/fmt-jpk-fd_map2x2_extracted.jpk-force-map`

 * *Files identical despite different names*

### Comparing `nanite-3.5.4/tests/data/fmt-jpk-fd_map_bad_2013-05-27_1.jpk-force-map` & `nanite-3.6.0/tests/data/fmt-jpk-fd_map_bad_2013-05-27_1.jpk-force-map`

 * *Files identical despite different names*

### Comparing `nanite-3.5.4/tests/data/fmt-jpk-fd_map_bad_2013-05-27_2.jpk-force-map` & `nanite-3.6.0/tests/data/fmt-jpk-fd_map_bad_2013-05-27_2.jpk-force-map`

 * *Files identical despite different names*

### Comparing `nanite-3.5.4/tests/data/fmt-jpk-fd_single_bad_2017-01-16_1.jpk-force` & `nanite-3.6.0/tests/data/fmt-jpk-fd_single_bad_2017-01-16_1.jpk-force`

 * *Files identical despite different names*

### Comparing `nanite-3.5.4/tests/data/fmt-jpk-fd_single_bad_2017-01-16_2.jpk-force` & `nanite-3.6.0/tests/data/fmt-jpk-fd_single_bad_2017-01-16_2.jpk-force`

 * *Files identical despite different names*

### Comparing `nanite-3.5.4/tests/data/fmt-jpk-fd_single_bad_2017-01-16_3.jpk-force` & `nanite-3.6.0/tests/data/fmt-jpk-fd_single_bad_2017-01-16_3.jpk-force`

 * *Files identical despite different names*

### Comparing `nanite-3.5.4/tests/data/fmt-jpk-fd_single_bad_2017-01-16_4.jpk-force` & `nanite-3.6.0/tests/data/fmt-jpk-fd_single_bad_2017-01-16_4.jpk-force`

 * *Files identical despite different names*

### Comparing `nanite-3.5.4/tests/data/fmt-jpk-fd_single_bad_2017-01-16_5.jpk-force` & `nanite-3.6.0/tests/data/fmt-jpk-fd_single_bad_2017-01-16_5.jpk-force`

 * *Files identical despite different names*

### Comparing `nanite-3.5.4/tests/data/fmt-jpk-fd_single_bad_GWAT_2017-10-17.jpk-force` & `nanite-3.6.0/tests/data/fmt-jpk-fd_single_bad_GWAT_2017-10-17.jpk-force`

 * *Files identical despite different names*

### Comparing `nanite-3.5.4/tests/data/fmt-jpk-fd_single_bad_bead10_2017-04-27.jpk-force` & `nanite-3.6.0/tests/data/fmt-jpk-fd_single_bad_bead10_2017-04-27.jpk-force`

 * *Files identical despite different names*

### Comparing `nanite-3.5.4/tests/data/fmt-jpk-fd_single_bad_bead46_2017-04-20.jpk-force` & `nanite-3.6.0/tests/data/fmt-jpk-fd_single_bad_bead46_2017-04-20.jpk-force`

 * *Files identical despite different names*

### Comparing `nanite-3.5.4/tests/data/fmt-jpk-fd_single_bad_bead7_2017-04-27.jpk-force` & `nanite-3.6.0/tests/data/fmt-jpk-fd_single_bad_bead7_2017-04-27.jpk-force`

 * *Files identical despite different names*

### Comparing `nanite-3.5.4/tests/data/fmt-jpk-fd_single_tilted-baseline-mitotic_2021-01-29.jpk-force` & `nanite-3.6.0/tests/data/fmt-jpk-fd_single_tilted-baseline-mitotic_2021-01-29.jpk-force`

 * *Files identical despite different names*

### Comparing `nanite-3.5.4/tests/data/fmt-jpk-fd_spot3-0192.jpk-force` & `nanite-3.6.0/tests/data/fmt-jpk-fd_spot3-0192.jpk-force`

 * *Files identical despite different names*

### Comparing `nanite-3.5.4/tests/data/model_external_basic.py` & `nanite-3.6.0/tests/data/model_external_basic.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-import lmfit
-import numpy as np
-
-
-def get_parameter_defaults():
-    """Return the default model parameters"""
-    # The order of the parameters must match the order
-    # of ´parameter_names´ and ´parameter_keys´.
-    params = lmfit.Parameters()
-    params.add("E", value=3e3, min=0)
-    params.add("R", value=10e-6, min=0, vary=False)
-    params.add("nu", value=.5, min=0, max=0.5, vary=False)
-    params.add("contact_point", value=0)
-    params.add("baseline", value=0)
-    return params
-
-
-def hertz_paraboloidal(delta, E, R, nu, contact_point=0, baseline=0):
-    """This is identical to the Hertz parabolic indenter model"""
-    aa = 4/3 * E/(1-nu**2)*np.sqrt(R)
-    root = contact_point-delta
-    pos = root > 0
-    bb = np.zeros_like(delta)
-    bb[pos] = (root[pos])**(3/2)
-    return aa*bb + baseline
-
-
-model_doc = hertz_paraboloidal.__doc__
-model_func = hertz_paraboloidal
-model_key = "hans_peter"
-model_name = "Hans Peter's model"
-parameter_keys = ["E", "R", "nu", "contact_point", "baseline"]
-parameter_names = ["Young's Modulus", "Tip Radius",
-                   "Poisson's Ratio", "Contact Point", "Force Baseline"]
-parameter_units = ["Pa", "m", "", "m", "N"]
-valid_axes_x = ["tip position"]
-valid_axes_y = ["force"]
+import lmfit
+import numpy as np
+
+
+def get_parameter_defaults():
+    """Return the default model parameters"""
+    # The order of the parameters must match the order
+    # of ´parameter_names´ and ´parameter_keys´.
+    params = lmfit.Parameters()
+    params.add("E", value=3e3, min=0)
+    params.add("R", value=10e-6, min=0, vary=False)
+    params.add("nu", value=.5, min=0, max=0.5, vary=False)
+    params.add("contact_point", value=0)
+    params.add("baseline", value=0)
+    return params
+
+
+def hertz_paraboloidal(delta, E, R, nu, contact_point=0, baseline=0):
+    """This is identical to the Hertz parabolic indenter model"""
+    aa = 4/3 * E/(1-nu**2)*np.sqrt(R)
+    root = contact_point-delta
+    pos = root > 0
+    bb = np.zeros_like(delta)
+    bb[pos] = (root[pos])**(3/2)
+    return aa*bb + baseline
+
+
+model_doc = hertz_paraboloidal.__doc__
+model_func = hertz_paraboloidal
+model_key = "hans_peter"
+model_name = "Hans Peter's model"
+parameter_keys = ["E", "R", "nu", "contact_point", "baseline"]
+parameter_names = ["Young's Modulus", "Tip Radius",
+                   "Poisson's Ratio", "Contact Point", "Force Baseline"]
+parameter_units = ["Pa", "m", "", "m", "N"]
+valid_axes_x = ["tip position"]
+valid_axes_y = ["force"]
```

### Comparing `nanite-3.5.4/tests/test_cli_plotting.py` & `nanite-3.6.0/tests/test_cli_plotting.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,27 @@
-import pathlib
-import tempfile
-
-from nanite.cli import plotting
-from nanite import load_group
-
-data_path = pathlib.Path(__file__).resolve().parent / "data"
-jpkfile = data_path / "fmt-jpk-fd_spot3-0192.jpk-force"
-
-
-def test_plotting():
-    # use temporary file
-    _, name = tempfile.mkstemp(suffix=".png", prefix="test_nanite_plotting_")
-    name = pathlib.Path(name)
-
-    grp = load_group(jpkfile)
-    idnt = grp[0]
-    idnt.apply_preprocessing(["compute_tip_position",
-                              "correct_force_offset"])
-    idnt.fit_model(model_key="hertz_para",
-                   params_initial=None,
-                   x_axis="tip position",
-                   y_axis="force",
-                   weight_cp=False,
-                   segment="retract")
-    plotting.plot_data(idnt=idnt, path=name)
-    assert name.stat().st_size > 90000
-
-
-if __name__ == "__main__":
-    # Run all tests
-    loc = locals()
-    for key in list(loc.keys()):
-        if key.startswith("test_") and hasattr(loc[key], "__call__"):
-            loc[key]()
+import pathlib
+import tempfile
+
+from nanite.cli import plotting
+from nanite import load_group
+
+data_path = pathlib.Path(__file__).resolve().parent / "data"
+jpkfile = data_path / "fmt-jpk-fd_spot3-0192.jpk-force"
+
+
+def test_plotting():
+    # use temporary file
+    _, name = tempfile.mkstemp(suffix=".png", prefix="test_nanite_plotting_")
+    name = pathlib.Path(name)
+
+    grp = load_group(jpkfile)
+    idnt = grp[0]
+    idnt.apply_preprocessing(["compute_tip_position",
+                              "correct_force_offset"])
+    idnt.fit_model(model_key="hertz_para",
+                   params_initial=None,
+                   x_axis="tip position",
+                   y_axis="force",
+                   weight_cp=False,
+                   segment="retract")
+    plotting.plot_data(idnt=idnt, path=name)
+    assert name.stat().st_size > 90000
```

### Comparing `nanite-3.5.4/tests/test_cli_profile.py` & `nanite-3.6.0/tests/test_cli_profile.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,85 +1,77 @@
-import pathlib
-import shutil
-import tempfile
-
-from nanite.cli import profile
-
-
-data_path = pathlib.Path(__file__).parent / "data"
-
-
-def test_profile_getter():
-    _, name = tempfile.mkstemp(suffix=".cfg", prefix="test_nanite_profile_")
-    name = pathlib.Path(name)
-    pf = profile.Profile(path=name)
-    # sanity checks (run twice to trigger loading and saving)
-    assert pf["segment"] == 0
-    assert pf["segment"] == 0
-    assert pf["preprocessing"] == ["compute_tip_position",
-                                   "correct_force_offset",
-                                   "correct_tip_offset"]
-    assert pf["preprocessing"] == ["compute_tip_position",
-                                   "correct_force_offset",
-                                   "correct_tip_offset"]
-    pf["preprocessing"] = ["compute_tip_position"]
-    assert pf["preprocessing"] == ["compute_tip_position"]
-    assert pf["range_x"] == [0, 0]
-    assert pf["range_x"] == [0, 0]
-    assert pf["weight_cp"] == 5e-7
-    assert pf["weight_cp"] == 5e-7
-
-
-def test_profile_getter_1_7_8():
-    """Load a profile from version 1.7.8"""
-    tdir = pathlib.Path(tempfile.mkdtemp(prefix="cli_profile_"))
-    name = "cli-profile-1.7.8.cfg"
-    cfgpath = tdir / name
-    shutil.copy2(data_path / name, cfgpath)
-    pf = profile.Profile(path=cfgpath)
-    assert pf["segment"] == 0
-    assert pf["segment"] == 0
-
-
-def test_profile_getter_2_1_0():
-    """Load a profile from version 2.1.0"""
-    tdir = pathlib.Path(tempfile.mkdtemp(prefix="cli_profile_"))
-    name = "cli-profile-2.1.0.cfg"
-    cfgpath = tdir / name
-    shutil.copy2(data_path / name, cfgpath)
-    pf = profile.Profile(path=cfgpath)
-    assert pf["segment"] == 0
-    assert pf["segment"] == 0
-    assert pf["rating training set"] == "zef18"
-
-
-def test_profile_fitparams():
-    _, name = tempfile.mkstemp(suffix=".cfg", prefix="test_nanite_profile_")
-    name = pathlib.Path(name)
-    pf = profile.Profile(path=name)
-    # sanity checks (run twice to trigger loading and saving)
-    pf["model_key"] = "hertz_cone"
-    params = pf.get_fit_params()
-    params2 = pf.get_fit_params()
-    assert params == params2
-    assert len(params) == 5
-    assert "E" in params.keys()
-
-
-def test_single_fitparam():
-    _, name = tempfile.mkstemp(suffix=".cfg", prefix="test_nanite_profile_")
-    name = pathlib.Path(name)
-    pf = profile.Profile(path=name)
-    # sanity checks (run twice to trigger loading and saving)
-    pf["fit param E value"] = 50
-    pf["fit param R value"] = 16e-6
-    params = pf.get_fit_params()
-    assert params["E"].value == 50
-    assert params["R"].value == 16e-6
-
-
-if __name__ == "__main__":
-    # Run all tests
-    loc = locals()
-    for key in list(loc.keys()):
-        if key.startswith("test_") and hasattr(loc[key], "__call__"):
-            loc[key]()
+import pathlib
+import shutil
+import tempfile
+
+from nanite.cli import profile
+
+
+data_path = pathlib.Path(__file__).parent / "data"
+
+
+def test_profile_getter():
+    _, name = tempfile.mkstemp(suffix=".cfg", prefix="test_nanite_profile_")
+    name = pathlib.Path(name)
+    pf = profile.Profile(path=name)
+    # sanity checks (run twice to trigger loading and saving)
+    assert pf["segment"] == 0
+    assert pf["segment"] == 0
+    assert pf["preprocessing"] == ["compute_tip_position",
+                                   "correct_force_offset",
+                                   "correct_tip_offset"]
+    assert pf["preprocessing"] == ["compute_tip_position",
+                                   "correct_force_offset",
+                                   "correct_tip_offset"]
+    pf["preprocessing"] = ["compute_tip_position"]
+    assert pf["preprocessing"] == ["compute_tip_position"]
+    assert pf["range_x"] == [0, 0]
+    assert pf["range_x"] == [0, 0]
+    assert pf["weight_cp"] == 5e-7
+    assert pf["weight_cp"] == 5e-7
+
+
+def test_profile_getter_1_7_8():
+    """Load a profile from version 1.7.8"""
+    tdir = pathlib.Path(tempfile.mkdtemp(prefix="cli_profile_"))
+    name = "cli-profile-1.7.8.cfg"
+    cfgpath = tdir / name
+    shutil.copy2(data_path / name, cfgpath)
+    pf = profile.Profile(path=cfgpath)
+    assert pf["segment"] == 0
+    assert pf["segment"] == 0
+
+
+def test_profile_getter_2_1_0():
+    """Load a profile from version 2.1.0"""
+    tdir = pathlib.Path(tempfile.mkdtemp(prefix="cli_profile_"))
+    name = "cli-profile-2.1.0.cfg"
+    cfgpath = tdir / name
+    shutil.copy2(data_path / name, cfgpath)
+    pf = profile.Profile(path=cfgpath)
+    assert pf["segment"] == 0
+    assert pf["segment"] == 0
+    assert pf["rating training set"] == "zef18"
+
+
+def test_profile_fitparams():
+    _, name = tempfile.mkstemp(suffix=".cfg", prefix="test_nanite_profile_")
+    name = pathlib.Path(name)
+    pf = profile.Profile(path=name)
+    # sanity checks (run twice to trigger loading and saving)
+    pf["model_key"] = "hertz_cone"
+    params = pf.get_fit_params()
+    params2 = pf.get_fit_params()
+    assert params == params2
+    assert len(params) == 5
+    assert "E" in params.keys()
+
+
+def test_single_fitparam():
+    _, name = tempfile.mkstemp(suffix=".cfg", prefix="test_nanite_profile_")
+    name = pathlib.Path(name)
+    pf = profile.Profile(path=name)
+    # sanity checks (run twice to trigger loading and saving)
+    pf["fit param E value"] = 50
+    pf["fit param R value"] = 16e-6
+    params = pf.get_fit_params()
+    assert params["E"].value == 50
+    assert params["R"].value == 16e-6
```

### Comparing `nanite-3.5.4/tests/test_cli_rating.py` & `nanite-3.6.0/tests/test_cli_rating.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,80 +1,71 @@
-import pathlib
-import tempfile
-
-import numpy as np
-
-from nanite.cli import profile, rating
-from nanite.rate import IndentationRater
-
-
-data_path = pathlib.Path(__file__).resolve().parent / "data"
-jpkfile = data_path / "fmt-jpk-fd_spot3-0192.jpk-force"
-jpkfile2 = data_path / "fmt-jpk-fd_map-data-reference-points.jpk-force-map"
-
-
-def setup_training_set(n=300):
-    tdir = tempfile.mkdtemp(prefix="test_nanite_rate_ts_")
-    tdir = pathlib.Path(tdir)
-    np.random.set_state(np.random.RandomState(47).get_state())
-    for bb in IndentationRater.get_feature_names(which_type="binary"):
-        bvals = np.random.choice([0, 1], size=n, p=[.05, .95])
-        np.savetxt(tdir / "train_{}.txt".format(bb), bvals)
-    for cc in IndentationRater.get_feature_names(which_type="continuous"):
-        cvals = np.random.random_sample(size=n)
-        np.savetxt(tdir / "train_{}.txt".format(cc), cvals)
-    thisrating = np.random.choice(range(11), size=n)
-    np.savetxt(tdir / "train_response.txt", thisrating)
-    return tdir
-
-
-def test_fit_data():
-    # use temporary file
-    _, name = tempfile.mkstemp(suffix=".cfg", prefix="test_nanite_cli_rate_")
-    name = pathlib.Path(name)
-    profile.Profile(path=name)
-
-    # this will fit with the profile default parameters
-    idnt = rating.fit_data(path=jpkfile, profile_path=name)
-    assert idnt.path == jpkfile
-    assert idnt.fit_properties["success"]
-
-
-def test_fit_data_with_user_training_set():
-    tdir = setup_training_set()
-    _, name = tempfile.mkstemp(suffix=".cfg", prefix="test_nanite_cli_rate_")
-    name = pathlib.Path(name)
-    pf = profile.Profile(path=name)
-    pf["rating training set"] = tdir
-    pf["fit param R value"] = 37.28e-6 / 2
-    pout = tempfile.mkdtemp(prefix="test_nanite_cli_rate_ts")
-    pout = pathlib.Path(pout)
-    rating.fit_perform(path=jpkfile2, path_results=pout, profile_path=name)
-    stats = np.loadtxt(pout / "statistics.tsv", skiprows=1, usecols=(1, 2, 3))
-    assert np.all(stats[:, 0] == [109, 129, 416])
-    assert np.all((3.5 < stats[:, 2]) * (stats[:, 2] < 5))
-
-
-def test_fit_data_with_zef18():
-    _, name = tempfile.mkstemp(suffix=".cfg", prefix="test_nanite_cli_rate_")
-    name = pathlib.Path(name)
-    pf = profile.Profile(path=name)
-    pf["rating training set"] = "zef18"
-    pf["weight_cp"] = 2e-6
-    pf["fit param R value"] = 137.28e-6 / 2
-    pout = tempfile.mkdtemp(prefix="test_nanite_cli_rate_ts")
-    pout = pathlib.Path(pout)
-    rating.fit_perform(path=jpkfile2, path_results=pout, profile_path=name)
-    stats = np.loadtxt(pout / "statistics.tsv", skiprows=1, usecols=(1, 2, 3))
-    assert np.all(stats[:, 0] == [109, 129, 416])
-    assert stats[0, 2] == 9.5
-    assert stats[1, 2] == 2.4
-    assert stats[2, 2] == 4.9
-
-
-if __name__ == "__main__":
-    # Run all tests
-    test_fit_data_with_zef18()
-    loc = locals()
-    for key in list(loc.keys()):
-        if key.startswith("test_") and hasattr(loc[key], "__call__"):
-            loc[key]()
+import pathlib
+import tempfile
+
+import numpy as np
+
+from nanite.cli import profile, rating
+from nanite.rate import IndentationRater
+
+
+data_path = pathlib.Path(__file__).resolve().parent / "data"
+jpkfile = data_path / "fmt-jpk-fd_spot3-0192.jpk-force"
+jpkfile2 = data_path / "fmt-jpk-fd_map-data-reference-points.jpk-force-map"
+
+
+def setup_training_set(n=300):
+    tdir = tempfile.mkdtemp(prefix="test_nanite_rate_ts_")
+    tdir = pathlib.Path(tdir)
+    np.random.set_state(np.random.RandomState(47).get_state())
+    for bb in IndentationRater.get_feature_names(which_type="binary"):
+        bvals = np.random.choice([0, 1], size=n, p=[.05, .95])
+        np.savetxt(tdir / "train_{}.txt".format(bb), bvals)
+    for cc in IndentationRater.get_feature_names(which_type="continuous"):
+        cvals = np.random.random_sample(size=n)
+        np.savetxt(tdir / "train_{}.txt".format(cc), cvals)
+    thisrating = np.random.choice(range(11), size=n)
+    np.savetxt(tdir / "train_response.txt", thisrating)
+    return tdir
+
+
+def test_fit_data():
+    # use temporary file
+    _, name = tempfile.mkstemp(suffix=".cfg", prefix="test_nanite_cli_rate_")
+    name = pathlib.Path(name)
+    profile.Profile(path=name)
+
+    # this will fit with the profile default parameters
+    idnt = rating.fit_data(path=jpkfile, profile_path=name)
+    assert idnt.path == jpkfile
+    assert idnt.fit_properties["success"]
+
+
+def test_fit_data_with_user_training_set():
+    tdir = setup_training_set()
+    _, name = tempfile.mkstemp(suffix=".cfg", prefix="test_nanite_cli_rate_")
+    name = pathlib.Path(name)
+    pf = profile.Profile(path=name)
+    pf["rating training set"] = tdir
+    pf["fit param R value"] = 37.28e-6 / 2
+    pout = tempfile.mkdtemp(prefix="test_nanite_cli_rate_ts")
+    pout = pathlib.Path(pout)
+    rating.fit_perform(path=jpkfile2, path_results=pout, profile_path=name)
+    stats = np.loadtxt(pout / "statistics.tsv", skiprows=1, usecols=(1, 2, 3))
+    assert np.all(stats[:, 0] == [109, 129, 416])
+    assert np.all((3.5 < stats[:, 2]) * (stats[:, 2] < 5))
+
+
+def test_fit_data_with_zef18():
+    _, name = tempfile.mkstemp(suffix=".cfg", prefix="test_nanite_cli_rate_")
+    name = pathlib.Path(name)
+    pf = profile.Profile(path=name)
+    pf["rating training set"] = "zef18"
+    pf["weight_cp"] = 2e-6
+    pf["fit param R value"] = 137.28e-6 / 2
+    pout = tempfile.mkdtemp(prefix="test_nanite_cli_rate_ts")
+    pout = pathlib.Path(pout)
+    rating.fit_perform(path=jpkfile2, path_results=pout, profile_path=name)
+    stats = np.loadtxt(pout / "statistics.tsv", skiprows=1, usecols=(1, 2, 3))
+    assert np.all(stats[:, 0] == [109, 129, 416])
+    assert stats[0, 2] == 9.5
+    assert stats[1, 2] == 2.4
+    assert stats[2, 2] == 4.9
```

### Comparing `nanite-3.5.4/tests/test_fit_ancillary.py` & `nanite-3.6.0/tests/test_fit_ancillary.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,73 +1,65 @@
-"""Test of ancillary parameters"""
-import pathlib
-
-import numpy as np
-
-import nanite
-import nanite.model
-
-from common import MockModelModule
-
-
-data_path = pathlib.Path(__file__).parent / "data"
-jpkfile = data_path / "fmt-jpk-fd_spot3-0192.jpk-force"
-
-
-def test_simple_ancillary_override():
-    """basic test for ancillary parameters"""
-    ds1 = nanite.IndentationGroup(jpkfile)
-    idnt = ds1[0]
-
-    with MockModelModule(
-        compute_ancillaries=lambda x: {"E": 1580},
-        parameter_anc_keys=["E"],
-        parameter_anc_names=["ancillary E guess"],
-        parameter_anc_units=["Pa"],
-            model_key="test1"):
-        # We need to perform preprocessing first, if we want to get the
-        # correct initial contact point.
-        idnt.apply_preprocessing(["compute_tip_position"])
-        # We set the baseline fixed, because this test was written so)
-        params_initial = idnt.get_initial_fit_parameters(model_key="test1")
-        params_initial["baseline"].set(vary=False)
-        idnt.fit_model(model_key="test1",
-                       params_initial=params_initial)
-        assert idnt.fit_properties["params_initial"]["E"].value == 1580
-        assert np.allclose(idnt.fit_properties["params_fitted"]["E"].value,
-                           1584.8941261696934,
-                           atol=1,
-                           rtol=0)
-
-
-def test_simple_ancillary_override_nan():
-    """nan values are not used and should be ignored"""
-    ds1 = nanite.IndentationGroup(jpkfile)
-    idnt = ds1[0]
-
-    with MockModelModule(
-        compute_ancillaries=lambda x: {"E": np.nan},
-        parameter_anc_keys=["E"],
-        parameter_anc_names=["ancillary E guess"],
-        parameter_anc_units=["Pa"],
-            model_key="test2"):
-        # We need to perform preprocessing first, if we want to get the
-        # correct initial contact point.
-        idnt.apply_preprocessing(["compute_tip_position"])
-        # We set the baseline fixed, because this test was written so)
-        params_initial = idnt.get_initial_fit_parameters(model_key="test2")
-        params_initial["baseline"].set(vary=False)
-        idnt.fit_model(model_key="test2",
-                       params_initial=params_initial)
-        assert idnt.fit_properties["params_initial"]["E"].value == 3000
-        assert np.allclose(idnt.fit_properties["params_fitted"]["E"].value,
-                           1584.8876592662375,
-                           atol=0,
-                           rtol=1e-5)
-
-
-if __name__ == "__main__":
-    # Run all tests
-    loc = locals()
-    for key in list(loc.keys()):
-        if key.startswith("test_") and hasattr(loc[key], "__call__"):
-            loc[key]()
+"""Test of ancillary parameters"""
+import pathlib
+
+import numpy as np
+
+import nanite
+import nanite.model
+
+from common import MockModelModule
+
+
+data_path = pathlib.Path(__file__).parent / "data"
+jpkfile = data_path / "fmt-jpk-fd_spot3-0192.jpk-force"
+
+
+def test_simple_ancillary_override():
+    """basic test for ancillary parameters"""
+    ds1 = nanite.IndentationGroup(jpkfile)
+    idnt = ds1[0]
+
+    with MockModelModule(
+        compute_ancillaries=lambda x: {"E": 1580},
+        parameter_anc_keys=["E"],
+        parameter_anc_names=["ancillary E guess"],
+        parameter_anc_units=["Pa"],
+            model_key="test1"):
+        # We need to perform preprocessing first, if we want to get the
+        # correct initial contact point.
+        idnt.apply_preprocessing(["compute_tip_position"])
+        # We set the baseline fixed, because this test was written so)
+        params_initial = idnt.get_initial_fit_parameters(model_key="test1")
+        params_initial["baseline"].set(vary=False)
+        idnt.fit_model(model_key="test1",
+                       params_initial=params_initial)
+        assert idnt.fit_properties["params_initial"]["E"].value == 1580
+        assert np.allclose(idnt.fit_properties["params_fitted"]["E"].value,
+                           1584.8941261696934,
+                           atol=1,
+                           rtol=0)
+
+
+def test_simple_ancillary_override_nan():
+    """nan values are not used and should be ignored"""
+    ds1 = nanite.IndentationGroup(jpkfile)
+    idnt = ds1[0]
+
+    with MockModelModule(
+        compute_ancillaries=lambda x: {"E": np.nan},
+        parameter_anc_keys=["E"],
+        parameter_anc_names=["ancillary E guess"],
+        parameter_anc_units=["Pa"],
+            model_key="test2"):
+        # We need to perform preprocessing first, if we want to get the
+        # correct initial contact point.
+        idnt.apply_preprocessing(["compute_tip_position"])
+        # We set the baseline fixed, because this test was written so)
+        params_initial = idnt.get_initial_fit_parameters(model_key="test2")
+        params_initial["baseline"].set(vary=False)
+        idnt.fit_model(model_key="test2",
+                       params_initial=params_initial)
+        assert idnt.fit_properties["params_initial"]["E"].value == 3000
+        assert np.allclose(idnt.fit_properties["params_fitted"]["E"].value,
+                           1584.8876592662375,
+                           atol=1,
+                           rtol=0)
```

### Comparing `nanite-3.5.4/tests/test_fit_base.py` & `nanite-3.6.0/tests/test_fit_base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,164 +1,164 @@
-"""Test basic fitting"""
-import pathlib
-
-import numpy as np
-
-import nanite
-from nanite import IndentationGroup
-import pytest
-
-
-data_path = pathlib.Path(__file__).parent / "data"
-jpkfile = data_path / "fmt-jpk-fd_spot3-0192.jpk-force"
-
-
-def test_lmfit_method():
-    ds1 = IndentationGroup(jpkfile)
-    apret = ds1[0]
-    apret.apply_preprocessing(["compute_tip_position"])
-
-    inparams = nanite.model.model_hertz_paraboloidal.get_parameter_defaults()
-    inparams["baseline"].vary = True
-    inparams["contact_point"].set(1.8321e-5)
-
-    # Fit with absolute full range
-    kwargs = dict(model_key="hertz_para",
-                  params_initial=inparams,
-                  range_x=(0, 0),
-                  range_type="absolute",
-                  x_axis="tip position",
-                  y_axis="force",
-                  segment="approach",
-                  weight_cp=False)
-
-    apret.fit_model(**kwargs)
-    params1 = apret.fit_properties["params_fitted"]
-    assert np.allclose(params1["contact_point"].value,
-                       1.802931023582261e-05,
-                       rtol=0,
-                       atol=0.000000000005,
-                       )
-
-    # make sure leastsq is the default
-    apret.fit_model(method="leastsq", **kwargs)
-    params2 = apret.fit_properties["params_fitted"]
-    assert params2["contact_point"].value == params1["contact_point"]
-
-    # use a different method
-    apret.fit_model(method="nelder", method_kws={"max_nfev": 5}, **kwargs)
-    params3 = apret.fit_properties["params_fitted"]
-    assert params3["contact_point"].value != params1["contact_point"]
-    assert np.allclose(params3["contact_point"].value,
-                       1.8779025e-05,
-                       rtol=0,
-                       atol=0.000000000005,
-                       )
-
-
-@pytest.mark.parametrize("gcf_k", [0.1, 0.23, 0.3, 1/np.pi, 0.5, 0.6, 1.0])
-def test_gcf_k_no_change_in_contact_point(gcf_k):
-    """Fit result for contact point does not change with gcf_k"""
-    ds1 = IndentationGroup(jpkfile)
-    apret = ds1[0]
-    apret.apply_preprocessing(["compute_tip_position"])
-
-    inparams = nanite.model.model_hertz_paraboloidal.get_parameter_defaults()
-    inparams["baseline"].vary = True
-    inparams["contact_point"].set(1.8321e-5)
-    # sane initial fit parameters with gcf_k in mind
-    inparams["E"].set(inparams["E"].value * (1/gcf_k)**(3/2))
-
-    # Fit with absolute full range
-    kwargs = dict(model_key="hertz_para",
-                  params_initial=inparams,
-                  range_x=(0, 0),
-                  range_type="absolute",
-                  x_axis="tip position",
-                  y_axis="force",
-                  segment="approach",
-                  weight_cp=False,
-                  gcf_k=gcf_k)
-
-    apret.fit_model(**kwargs)
-    params1 = apret.fit_properties["params_fitted"]
-    assert np.allclose(params1["contact_point"].value,
-                       1.802931023582261e-05,
-                       rtol=0,
-                       atol=0.000000000005,
-                       )
-
-
-@pytest.mark.parametrize("gcf_k", [0.1, 0.23, 0.3, 1/np.pi, 0.5, 0.6, 1.0])
-def test_gcf_k_no_change_in_fitted_curve(gcf_k):
-    """Fit result for contact point does not change with gcf_k"""
-    ds1 = IndentationGroup(jpkfile)
-    apret = ds1[0]
-    apret.apply_preprocessing(["compute_tip_position"])
-
-    inparams = nanite.model.model_hertz_paraboloidal.get_parameter_defaults()
-    inparams["baseline"].vary = True
-    inparams["contact_point"].set(1.8321e-5)
-    # sane initial fit parameters with gcf_k in mind
-    inparams["E"].set(inparams["E"].value * (1/gcf_k)**(3/2))
-
-    # Fit with absolute full range
-    kwargs = dict(model_key="hertz_para",
-                  params_initial=inparams,
-                  range_x=(0, 0),
-                  range_type="absolute",
-                  x_axis="tip position",
-                  y_axis="force",
-                  segment="approach",
-                  weight_cp=False,
-                  gcf_k=gcf_k)
-
-    apret.fit_model(**kwargs)
-    assert np.allclose(np.nanmax(apret["fit"]),
-                       3.496319691452543e-09,
-                       atol=0.000001e-9,
-                       rtol=0)
-    assert np.allclose(np.nanmax(apret["fit residuals"]),
-                       2.233069676202635e-10,
-                       atol=0.000001e-10,
-                       rtol=0)
-
-
-@pytest.mark.parametrize("gcf_k", [0.1, 0.23, 0.3, 1/np.pi, 0.5, 0.6, 1.0])
-def test_gcf_k_scaling_of_youngs_modulus(gcf_k):
-    """Fit result for Young's modulus should scale with gcf_k"""
-    ds1 = IndentationGroup(jpkfile)
-    apret = ds1[0]
-    apret.apply_preprocessing(["compute_tip_position", "correct_tip_offset"])
-
-    inparams = nanite.model.model_hertz_paraboloidal.get_parameter_defaults()
-    inparams["baseline"].vary = True
-    inparams["contact_point"].set(0)
-
-    # Fit with absolute full range
-    kwargs = dict(model_key="hertz_para",
-                  params_initial=inparams,
-                  range_x=(0, 0),
-                  range_type="absolute",
-                  x_axis="tip position",
-                  y_axis="force",
-                  segment="approach",
-                  weight_cp=False,
-                  gcf_k=gcf_k)
-
-    apret.fit_model(**kwargs)
-    params1 = apret.fit_properties["params_fitted"]
-    # proportionality between E and gcf_k
-    corrval = 14741.950622347102 * (1/gcf_k)**(3/2)
-    assert np.allclose(params1["E"].value,
-                       corrval,
-                       rtol=0.0001,
-                       atol=0,
-                       )
-
-
-if __name__ == "__main__":
-    # Run all tests
-    loc = locals()
-    for key in list(loc.keys()):
-        if key.startswith("test_") and hasattr(loc[key], "__call__"):
-            loc[key]()
+"""Test basic fitting"""
+import pathlib
+
+import numpy as np
+
+import nanite
+from nanite import IndentationGroup
+import pytest
+
+
+data_path = pathlib.Path(__file__).parent / "data"
+jpkfile = data_path / "fmt-jpk-fd_spot3-0192.jpk-force"
+
+
+def test_lmfit_method():
+    ds1 = IndentationGroup(jpkfile)
+    apret = ds1[0]
+    apret.apply_preprocessing(["compute_tip_position"])
+
+    inparams = nanite.model.model_hertz_paraboloidal.get_parameter_defaults()
+    inparams["baseline"].vary = True
+    inparams["contact_point"].set(1.8321e-5)
+
+    # Fit with absolute full range
+    kwargs = dict(model_key="hertz_para",
+                  params_initial=inparams,
+                  range_x=(0, 0),
+                  range_type="absolute",
+                  x_axis="tip position",
+                  y_axis="force",
+                  segment="approach",
+                  weight_cp=False)
+
+    apret.fit_model(**kwargs)
+    params1 = apret.fit_properties["params_fitted"]
+    assert np.allclose(params1["contact_point"].value,
+                       1.802931023582261e-05,
+                       atol=2e-10,
+                       rtol=0,
+                       )
+
+    # make sure leastsq is the default
+    apret.fit_model(method="leastsq", **kwargs)
+    params2 = apret.fit_properties["params_fitted"]
+    assert params2["contact_point"].value == params1["contact_point"]
+
+    # use a different method
+    apret.fit_model(method="nelder", method_kws={"max_nfev": 5}, **kwargs)
+    params3 = apret.fit_properties["params_fitted"]
+    assert params3["contact_point"].value != params1["contact_point"]
+    assert np.allclose(params3["contact_point"].value,
+                       1.8779025e-05,
+                       atol=2e-10,
+                       rtol=0,
+                       )
+
+
+@pytest.mark.parametrize("gcf_k", [0.1, 0.23, 0.3, 1/np.pi, 0.5, 0.6, 1.0])
+def test_gcf_k_no_change_in_contact_point(gcf_k):
+    """Fit result for contact point does not change with gcf_k"""
+    ds1 = IndentationGroup(jpkfile)
+    apret = ds1[0]
+    apret.apply_preprocessing(["compute_tip_position"])
+
+    inparams = nanite.model.model_hertz_paraboloidal.get_parameter_defaults()
+    inparams["baseline"].vary = True
+    inparams["contact_point"].set(1.8321e-5)
+    # sane initial fit parameters with gcf_k in mind
+    inparams["E"].set(inparams["E"].value * (1/gcf_k)**(3/2))
+
+    # Fit with absolute full range
+    kwargs = dict(model_key="hertz_para",
+                  params_initial=inparams,
+                  range_x=(0, 0),
+                  range_type="absolute",
+                  x_axis="tip position",
+                  y_axis="force",
+                  segment="approach",
+                  weight_cp=False,
+                  gcf_k=gcf_k)
+
+    apret.fit_model(**kwargs)
+    params1 = apret.fit_properties["params_fitted"]
+    assert np.allclose(params1["contact_point"].value,
+                       1.802931023582261e-05,
+                       atol=2e-11,
+                       rtol=0,
+                       )
+
+
+@pytest.mark.parametrize("gcf_k", [0.1, 0.23, 0.3, 1/np.pi, 0.5, 0.6, 1.0])
+def test_gcf_k_no_change_in_fitted_curve(gcf_k):
+    """Fit result for contact point does not change with gcf_k"""
+    ds1 = IndentationGroup(jpkfile)
+    apret = ds1[0]
+    apret.apply_preprocessing(["compute_tip_position"])
+
+    inparams = nanite.model.model_hertz_paraboloidal.get_parameter_defaults()
+    inparams["baseline"].vary = True
+    inparams["contact_point"].set(1.8321e-5)
+    # sane initial fit parameters with gcf_k in mind
+    inparams["E"].set(inparams["E"].value * (1/gcf_k)**(3/2))
+
+    # Fit with absolute full range
+    kwargs = dict(model_key="hertz_para",
+                  params_initial=inparams,
+                  range_x=(0, 0),
+                  range_type="absolute",
+                  x_axis="tip position",
+                  y_axis="force",
+                  segment="approach",
+                  weight_cp=False,
+                  gcf_k=gcf_k)
+
+    apret.fit_model(**kwargs)
+    assert np.allclose(np.nanmax(apret["fit"]),
+                       3.496152328502394e-09,
+                       atol=0,
+                       rtol=1e-4)
+    assert np.allclose(np.nanmax(apret["fit residuals"]),
+                       2.2340798430821952e-10,
+                       atol=0,
+                       rtol=1e-3)
+
+
+@pytest.mark.parametrize("gcf_k", [0.1, 0.23, 0.3, 1/np.pi, 0.5, 0.6, 1.0])
+def test_gcf_k_scaling_of_youngs_modulus(gcf_k):
+    """Fit result for Young's modulus should scale with gcf_k"""
+    ds1 = IndentationGroup(jpkfile)
+    apret = ds1[0]
+    apret.apply_preprocessing(["compute_tip_position", "correct_tip_offset"])
+
+    inparams = nanite.model.model_hertz_paraboloidal.get_parameter_defaults()
+    inparams["baseline"].vary = True
+    inparams["contact_point"].set(0)
+
+    # Fit with absolute full range
+    kwargs = dict(model_key="hertz_para",
+                  params_initial=inparams,
+                  range_x=(0, 0),
+                  range_type="absolute",
+                  x_axis="tip position",
+                  y_axis="force",
+                  segment="approach",
+                  weight_cp=False,
+                  gcf_k=gcf_k)
+
+    apret.fit_model(**kwargs)
+    params1 = apret.fit_properties["params_fitted"]
+    # proportionality between E and gcf_k
+    corrval = 14741.950622347102 * (1/gcf_k)**(3/2)
+    assert np.allclose(params1["E"].value,
+                       corrval,
+                       rtol=0.0001,
+                       atol=0,
+                       )
+
+
+if __name__ == "__main__":
+    # Run all tests
+    loc = locals()
+    for key in list(loc.keys()):
+        if key.startswith("test_") and hasattr(loc[key], "__call__"):
+            loc[key]()
```

### Comparing `nanite-3.5.4/tests/test_fit_emodulus_search.py` & `nanite-3.6.0/tests/test_fit_emodulus_search.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,120 +1,112 @@
-"""Test of data set functionalities"""
-import pathlib
-import time
-
-import numpy as np
-
-from nanite import IndentationGroup
-from nanite.fit import FitDataError
-
-
-data_path = pathlib.Path(__file__).parent / "data"
-jpkfile = data_path / "fmt-jpk-fd_spot3-0192.jpk-force"
-badjpk = data_path / "fmt-jpk-fd_single_bad_GWAT_2017-10-17.jpk-force"
-
-
-def test_emodulus_search():
-    ds = IndentationGroup(jpkfile)
-    ar = ds[0]
-    ar.apply_preprocessing(["compute_tip_position",
-                            "correct_force_offset",
-                            "correct_tip_offset"])
-    ar.fit_model(model_key="hertz_cone",
-                 params_initial=None,
-                 x_axis="tip position",
-                 y_axis="force",
-                 weight_cp=False,
-                 segment="approach",
-                 optimal_fit_edelta=True,
-                 )
-    assert "optimal_fit_delta_array" in ar.fit_properties
-    assert "optimal_fit_E_array" in ar.fit_properties
-    assert "optimal_fit_delta" in ar.fit_properties
-
-    # This assertion might fail when the preprocessing changes
-    # or when the search algorithm for the optimal fit changes.
-    dopt = -1.2047321672207138e-07
-    assert np.allclose(ar.fit_properties["optimal_fit_delta"], dopt)
-
-    if __name__ == "__main__":
-        import matplotlib.pylab as plt
-        _fig, axes = plt.subplots(2, 1)
-        axes[0].plot(ar["tip position"]*1e6, ar["force"]*1e9, label="data")
-        axes[0].plot(ar["tip position"]*1e6, ar["fit"]*1e9, label="fit")
-        axes[0].legend()
-        axes[0].grid()
-        axes[0].set_xlabel("indentation [µm]")
-        axes[0].set_ylabel("force [nN]")
-
-        deltas = ar.fit_properties["optimal_fit_delta_array"]*1e6
-        emod = ar.fit_properties["optimal_fit_E_array"]
-        axes[1].plot(deltas, emod, label="emodulus/minimal-indentation-curve")
-        axes[1].set_xlabel("minimal indentation [µm]")
-        axes[1].set_ylabel("emodulus [Pa]")
-        axes[1].vlines(ar.fit_properties["optimal_fit_delta"]*1e6,
-                       emod.min(), emod.max(),
-                       label="optimal minimal indentation at plateau",
-                       color="r")
-        axes[1].grid()
-        axes[1].legend()
-        plt.tight_layout()
-        plt.show()
-
-
-def test_cache_emodulus():
-    # Check that the fitting procedure does not perform unneccessary
-    # double fits and uses the cached variables for emoduli and
-    # minimal indentations.
-    ds = IndentationGroup(jpkfile)
-    ar = ds[0]
-    ar.apply_preprocessing(["compute_tip_position",
-                            "correct_force_offset",
-                            "correct_tip_offset"])
-    t01 = time.perf_counter()
-    ar.fit_model(model_key="hertz_cone",
-                 params_initial=None,
-                 x_axis="tip position",
-                 y_axis="force",
-                 weight_cp=False,
-                 segment="approach",
-                 optimal_fit_edelta=True,
-                 )
-    t02 = time.perf_counter()
-
-    t11 = time.perf_counter()
-    ar.fit_model()
-    t12 = time.perf_counter()
-    assert (t02-t01)*1e-4 > t12 - \
-        t11, "Second computation should yield cached value (faster)!"
-
-    # Make sure that changing the fit model is longer again
-    t21 = time.perf_counter()
-    ar.fit_model(model_key="hertz_para")
-    t22 = time.perf_counter()
-
-    assert ((t22-t21)*1e-4
-            > (t12 - t11)), "Changing model_key should slow down computation!"
-
-
-def test_fit_data_error():
-    # a FitDataError is raised when it is not possible to compute an
-    # E(delta) curve:
-    ds = IndentationGroup(badjpk)
-    ar = ds[0]
-    ar.apply_preprocessing(["compute_tip_position",
-                            "correct_force_offset",
-                            "correct_tip_offset"])
-    try:
-        ar.compute_emodulus_mindelta()
-    except FitDataError:
-        pass
-    else:
-        assert False, "Invalid input data should not allow E(delt) computation"
-
-
-if __name__ == "__main__":
-    # Run all tests
-    loc = locals()
-    for key in list(loc.keys()):
-        if key.startswith("test_") and hasattr(loc[key], "__call__"):
-            loc[key]()
+"""Test of data set functionalities"""
+import pathlib
+import time
+
+import numpy as np
+
+from nanite import IndentationGroup
+from nanite.fit import FitDataError
+
+
+data_path = pathlib.Path(__file__).parent / "data"
+jpkfile = data_path / "fmt-jpk-fd_spot3-0192.jpk-force"
+badjpk = data_path / "fmt-jpk-fd_single_bad_GWAT_2017-10-17.jpk-force"
+
+
+def test_emodulus_search():
+    ds = IndentationGroup(jpkfile)
+    ar = ds[0]
+    ar.apply_preprocessing(["compute_tip_position",
+                            "correct_force_offset",
+                            "correct_tip_offset"])
+    ar.fit_model(model_key="hertz_cone",
+                 params_initial=None,
+                 x_axis="tip position",
+                 y_axis="force",
+                 weight_cp=False,
+                 segment="approach",
+                 optimal_fit_edelta=True,
+                 )
+    assert "optimal_fit_delta_array" in ar.fit_properties
+    assert "optimal_fit_E_array" in ar.fit_properties
+    assert "optimal_fit_delta" in ar.fit_properties
+
+    # This assertion might fail when the preprocessing changes
+    # or when the search algorithm for the optimal fit changes.
+    dopt = -1.2047321672207138e-07
+    assert np.allclose(ar.fit_properties["optimal_fit_delta"], dopt)
+
+    if __name__ == "__main__":
+        import matplotlib.pylab as plt
+        _fig, axes = plt.subplots(2, 1)
+        axes[0].plot(ar["tip position"]*1e6, ar["force"]*1e9, label="data")
+        axes[0].plot(ar["tip position"]*1e6, ar["fit"]*1e9, label="fit")
+        axes[0].legend()
+        axes[0].grid()
+        axes[0].set_xlabel("indentation [µm]")
+        axes[0].set_ylabel("force [nN]")
+
+        deltas = ar.fit_properties["optimal_fit_delta_array"]*1e6
+        emod = ar.fit_properties["optimal_fit_E_array"]
+        axes[1].plot(deltas, emod, label="emodulus/minimal-indentation-curve")
+        axes[1].set_xlabel("minimal indentation [µm]")
+        axes[1].set_ylabel("emodulus [Pa]")
+        axes[1].vlines(ar.fit_properties["optimal_fit_delta"]*1e6,
+                       emod.min(), emod.max(),
+                       label="optimal minimal indentation at plateau",
+                       color="r")
+        axes[1].grid()
+        axes[1].legend()
+        plt.tight_layout()
+        plt.show()
+
+
+def test_cache_emodulus():
+    # Check that the fitting procedure does not perform unneccessary
+    # double fits and uses the cached variables for emoduli and
+    # minimal indentations.
+    ds = IndentationGroup(jpkfile)
+    ar = ds[0]
+    ar.apply_preprocessing(["compute_tip_position",
+                            "correct_force_offset",
+                            "correct_tip_offset"])
+    t01 = time.perf_counter()
+    ar.fit_model(model_key="hertz_cone",
+                 params_initial=None,
+                 x_axis="tip position",
+                 y_axis="force",
+                 weight_cp=False,
+                 segment="approach",
+                 optimal_fit_edelta=True,
+                 )
+    t02 = time.perf_counter()
+
+    t11 = time.perf_counter()
+    ar.fit_model()
+    t12 = time.perf_counter()
+    assert (t02-t01)*1e-4 > t12 - \
+        t11, "Second computation should yield cached value (faster)!"
+
+    # Make sure that changing the fit model is longer again
+    t21 = time.perf_counter()
+    ar.fit_model(model_key="hertz_para")
+    t22 = time.perf_counter()
+
+    assert ((t22-t21)*1e-4
+            > (t12 - t11)), "Changing model_key should slow down computation!"
+
+
+def test_fit_data_error():
+    # a FitDataError is raised when it is not possible to compute an
+    # E(delta) curve:
+    ds = IndentationGroup(badjpk)
+    ar = ds[0]
+    ar.apply_preprocessing(["compute_tip_position",
+                            "correct_force_offset",
+                            "correct_tip_offset"])
+    try:
+        ar.compute_emodulus_mindelta()
+    except FitDataError:
+        pass
+    else:
+        assert False, "Invalid input data should not allow E(delt) computation"
```

### Comparing `nanite-3.5.4/tests/test_fit_hash.py` & `nanite-3.6.0/tests/test_fit_hash.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,54 +1,46 @@
-"""Test hashing of fit results"""
-import pathlib
-import time
-
-import nanite
-from nanite import IndentationGroup
-
-
-data_path = pathlib.Path(__file__).parent / "data"
-jpkfile = data_path / "fmt-jpk-fd_spot3-0192.jpk-force"
-
-
-def test_hash_time():
-    ds1 = IndentationGroup(jpkfile)
-    apret = ds1[0]
-    apret.apply_preprocessing(["compute_tip_position"])
-
-    inparams = nanite.model.model_hertz_paraboloidal.get_parameter_defaults()
-    inparams["baseline"].vary = True
-    inparams["contact_point"].set(1.8321e-5)
-
-    # Fit with absolute full range
-    kwargs = dict(model_key="hertz_para",
-                  params_initial=inparams,
-                  range_x=(0, 0),
-                  range_type="absolute",
-                  x_axis="tip position",
-                  y_axis="force",
-                  segment="approach",
-                  weight_cp=False)
-    t0 = time.perf_counter()
-    apret.fit_model(**kwargs)
-    t1 = time.perf_counter()
-    apret.fit_model()
-    t2 = time.perf_counter()
-    kwargs["weight_cp"] = 1e-5
-    apret.fit_model(**kwargs)
-    t3 = time.perf_counter()
-    apret.fit_model()
-    t4 = time.perf_counter()
-
-    assert t1-t0 >= 100 * \
-        (t2-t1), "Consecutive fits with same parameters should be instant"
-    assert t3-t2 >= 100 * \
-        (t2-t1), "Changing parameters again should cause a new fit"
-    assert t3-t2 >= 100*(t4-t3), "And computing the same should be faster"
-
-
-if __name__ == "__main__":
-    # Run all tests
-    loc = locals()
-    for key in list(loc.keys()):
-        if key.startswith("test_") and hasattr(loc[key], "__call__"):
-            loc[key]()
+"""Test hashing of fit results"""
+import pathlib
+import time
+
+import nanite
+from nanite import IndentationGroup
+
+
+data_path = pathlib.Path(__file__).parent / "data"
+jpkfile = data_path / "fmt-jpk-fd_spot3-0192.jpk-force"
+
+
+def test_hash_time():
+    ds1 = IndentationGroup(jpkfile)
+    apret = ds1[0]
+    apret.apply_preprocessing(["compute_tip_position"])
+
+    inparams = nanite.model.model_hertz_paraboloidal.get_parameter_defaults()
+    inparams["baseline"].vary = True
+    inparams["contact_point"].set(1.8321e-5)
+
+    # Fit with absolute full range
+    kwargs = dict(model_key="hertz_para",
+                  params_initial=inparams,
+                  range_x=(0, 0),
+                  range_type="absolute",
+                  x_axis="tip position",
+                  y_axis="force",
+                  segment="approach",
+                  weight_cp=False)
+    t0 = time.perf_counter()
+    apret.fit_model(**kwargs)
+    t1 = time.perf_counter()
+    apret.fit_model()
+    t2 = time.perf_counter()
+    kwargs["weight_cp"] = 1e-5
+    apret.fit_model(**kwargs)
+    t3 = time.perf_counter()
+    apret.fit_model()
+    t4 = time.perf_counter()
+
+    assert t1-t0 >= 100 * \
+        (t2-t1), "Consecutive fits with same parameters should be instant"
+    assert t3-t2 >= 100 * \
+        (t2-t1), "Changing parameters again should cause a new fit"
+    assert t3-t2 >= 100*(t4-t3), "And computing the same should be faster"
```

### Comparing `nanite-3.5.4/tests/test_fit_properties.py` & `nanite-3.6.0/tests/test_fit_properties.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,136 +1,128 @@
-"""Test of data set functionalities"""
-import copy
-import pathlib
-
-from nanite.fit import FitProperties, FP_DEFAULT, FitKeyError
-from nanite import IndentationGroup
-from nanite import model
-
-
-data_path = pathlib.Path(__file__).parent / "data"
-jpkfile = data_path / "fmt-jpk-fd_spot3-0192.jpk-force"
-
-
-def test_changed_fit_properties():
-    ar = IndentationGroup(jpkfile)[0]
-    # Initially, fit properties are not set
-    assert not ar.fit_properties
-    assert isinstance(ar.fit_properties, dict)
-    # Prepprocessing
-    ar.apply_preprocessing(["compute_tip_position",
-                            "correct_tip_offset",
-                            "correct_force_offset"])
-    ar.fit_model()
-    hash1 = ar.fit_properties["hash"]
-    pinit = copy.deepcopy(ar.fit_properties["params_initial"])
-    pinit["E"].vary = False
-    assert "hash" in ar.fit_properties, "make sure we didn't change anything"
-    ar.fit_properties["params_initial"] = pinit
-    assert "hash" not in ar.fit_properties
-    ar.fit_model()
-    assert hash1 != ar.fit_properties["hash"]
-
-
-def test_fp_reset():
-    fp = FitProperties(**FP_DEFAULT)
-    fp["weight_cp"] = 1
-    assert "weight_cp" in fp
-    # Adding other than default keys is possible.
-    fp["hash"] = True
-    assert "hash" in fp
-    # Updating a default key with same value does not
-    # reset thedict.
-    fp["weight_cp"] = 1
-    assert "hash" in fp
-    # Changing the default value removes all other keys.
-    fp["hash"] = "laskdlai"
-    fp["weight_cp"] = 2
-    assert "test" not in fp
-    assert "rhababer" not in fp
-    # test manual resetting
-    fp["hash"] = "2"
-    fp.reset()
-    assert "hash" not in fp
-
-
-def test_with_dataset():
-    ar = IndentationGroup(jpkfile)[0]
-    # Initially, fit properties are not set
-    assert not ar.fit_properties
-    assert isinstance(ar.fit_properties, dict)
-    # Prepprocessing
-    ar.apply_preprocessing(["compute_tip_position",
-                            "correct_tip_offset",
-                            "correct_force_offset"])
-
-    # Fitting the data set will populate the dict
-    ar.fit_model()
-    assert isinstance(ar.fit_properties, dict)
-    assert isinstance(ar.fit_properties, FitProperties)
-    assert "hash" in ar.fit_properties
-    assert ar.fit_properties["success"]
-    hash1 = ar.fit_properties["hash"]
-    # Change something
-    ar.fit_properties["weight_cp"] = 0
-    assert "hash" not in ar.fit_properties
-    ar.fit_model()
-    hash2 = ar.fit_properties["hash"]
-    assert hash1 != hash2
-    # Change it back
-    ar.fit_properties["weight_cp"] = FP_DEFAULT["weight_cp"]
-    ar.fit_model()
-    hash3 = ar.fit_properties["hash"]
-    assert hash1 == hash3
-
-
-def test_change_model_key():
-    ar = IndentationGroup(jpkfile)[0]
-    # Prepprocessing
-    ar.apply_preprocessing(["compute_tip_position",
-                            "correct_tip_offset",
-                            "correct_force_offset"])
-
-    # Fitting the data set will populate the dict
-    ar.fit_model(model_key="hertz_para")
-    # Change the model
-    assert ar.fit_properties["params_initial"] is not None
-    ar.fit_properties["model_key"] = "hertz_cone"
-    # Changing the model key should reset the initial parameters
-    assert ar.fit_properties["params_initial"] is None
-
-
-def test_wrong_key():
-    fp = FitProperties(**FP_DEFAULT)
-    # unknown properties raise KeyError
-    try:
-        fp["dolce"] = False
-    except FitKeyError:
-        pass
-    else:
-        raise ValueError("Should not be able to set unknown key!")
-
-
-def test_wrong_params_initial():
-    ar = IndentationGroup(jpkfile)[0]
-    # Prepprocessing
-    ar.apply_preprocessing(["compute_tip_position",
-                            "correct_tip_offset",
-                            "correct_force_offset"])
-    md = model.models_available["hertz_para"]
-    params = md.get_parameter_defaults()
-    ar.fit_properties["model_key"] = "hertz_cone"
-    try:
-        ar.fit_model(params_initial=params)
-    except FitKeyError:
-        # We forced the wrong fitting parameters.
-        pass
-    else:
-        raise ValueError("Should not be able to use wrong fit parameters!")
-
-
-if __name__ == "__main__":
-    # Run all tests
-    loc = locals()
-    for key in list(loc.keys()):
-        if key.startswith("test_") and hasattr(loc[key], "__call__"):
-            loc[key]()
+"""Test of data set functionalities"""
+import copy
+import pathlib
+
+from nanite.fit import FitProperties, FP_DEFAULT, FitKeyError
+from nanite import IndentationGroup
+from nanite import model
+
+
+data_path = pathlib.Path(__file__).parent / "data"
+jpkfile = data_path / "fmt-jpk-fd_spot3-0192.jpk-force"
+
+
+def test_changed_fit_properties():
+    ar = IndentationGroup(jpkfile)[0]
+    # Initially, fit properties are not set
+    assert not ar.fit_properties
+    assert isinstance(ar.fit_properties, dict)
+    # Prepprocessing
+    ar.apply_preprocessing(["compute_tip_position",
+                            "correct_tip_offset",
+                            "correct_force_offset"])
+    ar.fit_model()
+    hash1 = ar.fit_properties["hash"]
+    pinit = copy.deepcopy(ar.fit_properties["params_initial"])
+    pinit["E"].vary = False
+    assert "hash" in ar.fit_properties, "make sure we didn't change anything"
+    ar.fit_properties["params_initial"] = pinit
+    assert "hash" not in ar.fit_properties
+    ar.fit_model()
+    assert hash1 != ar.fit_properties["hash"]
+
+
+def test_fp_reset():
+    fp = FitProperties(**FP_DEFAULT)
+    fp["weight_cp"] = 1
+    assert "weight_cp" in fp
+    # Adding other than default keys is possible.
+    fp["hash"] = True
+    assert "hash" in fp
+    # Updating a default key with same value does not
+    # reset thedict.
+    fp["weight_cp"] = 1
+    assert "hash" in fp
+    # Changing the default value removes all other keys.
+    fp["hash"] = "laskdlai"
+    fp["weight_cp"] = 2
+    assert "test" not in fp
+    assert "rhababer" not in fp
+    # test manual resetting
+    fp["hash"] = "2"
+    fp.reset()
+    assert "hash" not in fp
+
+
+def test_with_dataset():
+    ar = IndentationGroup(jpkfile)[0]
+    # Initially, fit properties are not set
+    assert not ar.fit_properties
+    assert isinstance(ar.fit_properties, dict)
+    # Prepprocessing
+    ar.apply_preprocessing(["compute_tip_position",
+                            "correct_tip_offset",
+                            "correct_force_offset"])
+
+    # Fitting the data set will populate the dict
+    ar.fit_model()
+    assert isinstance(ar.fit_properties, dict)
+    assert isinstance(ar.fit_properties, FitProperties)
+    assert "hash" in ar.fit_properties
+    assert ar.fit_properties["success"]
+    hash1 = ar.fit_properties["hash"]
+    # Change something
+    ar.fit_properties["weight_cp"] = 0
+    assert "hash" not in ar.fit_properties
+    ar.fit_model()
+    hash2 = ar.fit_properties["hash"]
+    assert hash1 != hash2
+    # Change it back
+    ar.fit_properties["weight_cp"] = FP_DEFAULT["weight_cp"]
+    ar.fit_model()
+    hash3 = ar.fit_properties["hash"]
+    assert hash1 == hash3
+
+
+def test_change_model_key():
+    ar = IndentationGroup(jpkfile)[0]
+    # Prepprocessing
+    ar.apply_preprocessing(["compute_tip_position",
+                            "correct_tip_offset",
+                            "correct_force_offset"])
+
+    # Fitting the data set will populate the dict
+    ar.fit_model(model_key="hertz_para")
+    # Change the model
+    assert ar.fit_properties["params_initial"] is not None
+    ar.fit_properties["model_key"] = "hertz_cone"
+    # Changing the model key should reset the initial parameters
+    assert ar.fit_properties["params_initial"] is None
+
+
+def test_wrong_key():
+    fp = FitProperties(**FP_DEFAULT)
+    # unknown properties raise KeyError
+    try:
+        fp["dolce"] = False
+    except FitKeyError:
+        pass
+    else:
+        raise ValueError("Should not be able to set unknown key!")
+
+
+def test_wrong_params_initial():
+    ar = IndentationGroup(jpkfile)[0]
+    # Prepprocessing
+    ar.apply_preprocessing(["compute_tip_position",
+                            "correct_tip_offset",
+                            "correct_force_offset"])
+    md = model.models_available["hertz_para"]
+    params = md.get_parameter_defaults()
+    ar.fit_properties["model_key"] = "hertz_cone"
+    try:
+        ar.fit_model(params_initial=params)
+    except FitKeyError:
+        # We forced the wrong fitting parameters.
+        pass
+    else:
+        raise ValueError("Should not be able to use wrong fit parameters!")
```

### Comparing `nanite-3.5.4/tests/test_group.py` & `nanite-3.6.0/tests/test_group.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,74 +1,66 @@
-"""Test group functionalities"""
-import pathlib
-import tempfile
-import shutil
-
-from afmformats.errors import MissingMetaDataError
-import pytest
-
-from nanite import Indentation, IndentationGroup, load_group
-
-
-data_path = pathlib.Path(__file__).resolve().parent / "data"
-jpkfile = data_path / "fmt-jpk-fd_spot3-0192.jpk-force"
-
-
-def test_base():
-    ds1 = IndentationGroup(jpkfile)
-    ds2 = IndentationGroup(jpkfile)
-
-    ds3 = ds1 + ds2
-    assert len(ds3) == 2
-    assert len(ds2) == 1
-    assert len(ds1) == 1
-
-    ds2 += ds3
-    assert len(ds3) == 2
-    assert len(ds2) == 3
-
-    for apret in ds3:
-        assert isinstance(apret, Indentation)
-    # test repr
-    print(ds3)
-
-
-def test_subgroup():
-    tmp = tempfile.mkdtemp(prefix="test_nanite_group")
-    shutil.copy(
-        data_path / "fmt-jpk-fd_map-data-reference-points.jpk-force-map", tmp)
-    shutil.copy(data_path / "fmt-jpk-fd_map2x2_extracted.jpk-force-map", tmp)
-    shutil.copy(
-        data_path / "fmt-jpk-fd_flipsign_2015.05.22-15.31.49.352.jpk-force",
-        tmp)
-
-    grp = load_group(tmp)
-    exp = pathlib.Path(tmp) / "fmt-jpk-fd_map2x2_extracted.jpk-force-map"
-    subgrp = grp.subgroup_with_path(path=exp)
-    assert len(grp) == 8
-    assert len(subgrp) == 4
-    assert subgrp[0].path == exp
-
-
-def test_open_dat_without_spring_constant():
-    # There are data files without spring constant but with force in nN.
-    # nanite requires the spring constant for computation of the tip
-    # position which we check for here.
-    tmp = tempfile.mkdtemp(prefix="test_nanite_group")
-    shutil.copy(data_path / "fmt-afm-workshop-fd_single_2021-10-22_14.16.csv",
-                tmp)
-
-    # try without explicit metadata
-    with pytest.raises(MissingMetaDataError, match="spring constant"):
-        load_group(tmp)
-
-    # try with metadata
-    grp = load_group(tmp, meta_override={"spring constant": 20})
-    assert grp[0].metadata["spring constant"] == 20
-
-
-if __name__ == "__main__":
-    # Run all tests
-    loc = locals()
-    for key in list(loc.keys()):
-        if key.startswith("test_") and hasattr(loc[key], "__call__"):
-            loc[key]()
+"""Test group functionalities"""
+import pathlib
+import tempfile
+import shutil
+
+from afmformats.errors import MissingMetaDataError
+import pytest
+
+from nanite import Indentation, IndentationGroup, load_group
+
+
+data_path = pathlib.Path(__file__).resolve().parent / "data"
+jpkfile = data_path / "fmt-jpk-fd_spot3-0192.jpk-force"
+
+
+def test_base():
+    ds1 = IndentationGroup(jpkfile)
+    ds2 = IndentationGroup(jpkfile)
+
+    ds3 = ds1 + ds2
+    assert len(ds3) == 2
+    assert len(ds2) == 1
+    assert len(ds1) == 1
+
+    ds2 += ds3
+    assert len(ds3) == 2
+    assert len(ds2) == 3
+
+    for apret in ds3:
+        assert isinstance(apret, Indentation)
+    # test repr
+    print(ds3)
+
+
+def test_subgroup():
+    tmp = tempfile.mkdtemp(prefix="test_nanite_group")
+    shutil.copy(
+        data_path / "fmt-jpk-fd_map-data-reference-points.jpk-force-map", tmp)
+    shutil.copy(data_path / "fmt-jpk-fd_map2x2_extracted.jpk-force-map", tmp)
+    shutil.copy(
+        data_path / "fmt-jpk-fd_flipsign_2015.05.22-15.31.49.352.jpk-force",
+        tmp)
+
+    grp = load_group(tmp)
+    exp = pathlib.Path(tmp) / "fmt-jpk-fd_map2x2_extracted.jpk-force-map"
+    subgrp = grp.subgroup_with_path(path=exp)
+    assert len(grp) == 8
+    assert len(subgrp) == 4
+    assert subgrp[0].path == exp
+
+
+def test_open_dat_without_spring_constant():
+    # There are data files without spring constant but with force in nN.
+    # nanite requires the spring constant for computation of the tip
+    # position which we check for here.
+    tmp = tempfile.mkdtemp(prefix="test_nanite_group")
+    shutil.copy(data_path / "fmt-afm-workshop-fd_single_2021-10-22_14.16.csv",
+                tmp)
+
+    # try without explicit metadata
+    with pytest.raises(MissingMetaDataError, match="spring constant"):
+        load_group(tmp)
+
+    # try with metadata
+    grp = load_group(tmp, meta_override={"spring constant": 20})
+    assert grp[0].metadata["spring constant"] == 20
```

### Comparing `nanite-3.5.4/tests/test_indent.py` & `nanite-3.6.0/tests/test_indent.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,305 +1,304 @@
-"""Test of data set functionalities"""
-import pathlib
-import tempfile
-
-import numpy as np
-import pytest
-
-import afmformats
-import nanite
-import nanite.model
-
-
-data_path = pathlib.Path(__file__).parent / "data"
-jpkfile = data_path / "fmt-jpk-fd_spot3-0192.jpk-force"
-
-
-def test_apply_preprocessing():
-    ds1 = nanite.IndentationGroup(jpkfile)
-    idnt = ds1[0]
-    # apply preprocessing by manually setting the list
-    idnt.preprocessing = ["compute_tip_position"]
-    idnt.apply_preprocessing()
-
-
-def test_apply_preprocessing_remember_fit_properties():
-    """
-    Normally, the fit properties would be overridden
-    if the preprocessing changes. For user convenience,
-    nanite remembers it. This is the test
-    """
-    ds1 = nanite.IndentationGroup(jpkfile)
-    idnt = ds1[0]
-    idnt.apply_preprocessing(["compute_tip_position"])
-
-    inparams = nanite.model.model_hertz_paraboloidal.get_parameter_defaults()
-    inparams["baseline"].vary = True
-    cp1 = 1.8029310065572342e-05
-    inparams["contact_point"].set(cp1)
-    inparams["contact_point"].vary = False
-
-    # Fit with absolute full range
-    idnt.fit_model(model_key="hertz_para",
-                   params_initial=inparams,
-                   range_x=(0, 0),
-                   range_type="absolute",
-                   x_axis="tip position",
-                   y_axis="force",
-                   segment="approach",
-                   weight_cp=False)
-    assert cp1 == idnt.fit_properties["params_initial"]["contact_point"].value
-    assert cp1 == idnt.fit_properties["params_fitted"]["contact_point"].value
-
-    # Change preprocessing
-    idnt.apply_preprocessing(["compute_tip_position",
-                              "correct_force_offset"])
-    assert cp1 == idnt.fit_properties["params_initial"]["contact_point"].value
-
-
-def test_basic():
-    ds1 = nanite.IndentationGroup(jpkfile)
-    idnt = ds1[0]
-    # tip-sample separation
-    idnt.apply_preprocessing(["compute_tip_position"])
-    assert idnt.preprocessing == ["compute_tip_position"]
-    assert idnt["tip position"][0] == 2.2803841798545836e-05
-    # correct for an offset in the tip
-    idnt.apply_preprocessing(["compute_tip_position",
-                              "correct_tip_offset"])
-    # This value is subject to change if a better way to estimate the
-    # contact point is found:
-    assert idnt["tip position"][0] == 4.765854684370548e-06
-
-
-def test_export():
-    ds1 = nanite.IndentationGroup(jpkfile)
-    idnt = ds1[0]
-    # tip-sample separation
-    idnt.apply_preprocessing(["compute_tip_position"])
-    # create temporary file
-    _, path = tempfile.mkstemp(suffix=".tab", prefix="nanite_idnt_export")
-    idnt.export_data(path)
-    data = afmformats.load_data(path)[0]
-    assert len(data) == 4000
-    assert np.allclose(data["force"][100], -4.853736717639109e-10)
-    assert np.allclose(data["height (measured)"][100], 2.256791903750211e-05,
-                       atol=1e-10, rtol=0)
-    assert data["segment"][100] == 0
-    assert np.allclose(data["time"][100], 0.04999999999999999)
-    assert np.allclose(data["tip position"][100], 2.255675939721752e-05,
-                       atol=1e-10, rtol=0)
-    assert data["segment"][3000] == 1
-
-
-def test_fitting():
-    ds1 = nanite.IndentationGroup(jpkfile)
-    idnt = ds1[0]
-    idnt.apply_preprocessing(["compute_tip_position"])
-
-    inparams = nanite.model.model_hertz_paraboloidal.get_parameter_defaults()
-    inparams["baseline"].vary = True
-    inparams["contact_point"].set(1.8e-5)
-
-    # Fit with absolute full range
-    idnt.fit_model(model_key="hertz_para",
-                   params_initial=inparams,
-                   range_x=(0, 0),
-                   range_type="absolute",
-                   x_axis="tip position",
-                   y_axis="force",
-                   segment="approach",
-                   weight_cp=False)
-    params = idnt.fit_properties["params_fitted"]
-    assert np.allclose(params["contact_point"].value, 1.8029310201193193e-05)
-    assert np.allclose(params["E"].value, 14741.958242422093)
-
-    # Fit with absolute short
-    idnt.fit_model(model_key="hertz_para",
-                   params_initial=inparams,
-                   range_x=(17e-06, 19e-6),
-                   range_type="absolute",
-                   x_axis="tip position",
-                   y_axis="force",
-                   segment="approach",
-                   weight_cp=False)
-    params2 = idnt.fit_properties["params_fitted"]
-    assert np.allclose(params2["contact_point"].value, 1.8028461828272924e-05)
-    assert np.allclose(params2["E"].value, 14840.840404880484)
-
-    # Fit with relative to initial fit
-    idnt.fit_model(model_key="hertz_para",
-                   params_initial=params2,
-                   range_x=(-2e-6, 1e-6),
-                   range_type="relative cp",
-                   x_axis="tip position",
-                   y_axis="force",
-                   segment="approach",
-                   weight_cp=False)
-    params3 = idnt.fit_properties["params_fitted"]
-    # These results are subject to change if the "relative cp" method is
-    # changed.
-    assert np.allclose(params3["contact_point"].value, 1.8028478083499856e-05)
-    assert np.allclose(params3["E"].value, 14839.821714634612)
-
-
-@pytest.mark.filterwarnings('ignore::nanite.fit.FitWarning')
-def test_get_initial_fit_parameters():
-    """This is a convenience function"""
-    ds1 = nanite.IndentationGroup(jpkfile)
-    idnt = ds1[0]
-    # A: sanity check
-    fp = idnt.get_initial_fit_parameters()
-    assert fp["contact_point"].value == 0, "need to get tip position first"
-    # B: get default fit parameters (hertz_para)
-    idnt.apply_preprocessing(["compute_tip_position"])
-    fp = idnt.get_initial_fit_parameters()
-    for kk in ['E', 'R', 'nu', 'contact_point', 'baseline']:
-        assert kk in fp.keys()
-    # C: set other model and get fit parameters
-    idnt.fit_properties["model_key"] = "hertz_pyr3s"
-    fp2 = idnt.get_initial_fit_parameters()
-    for kk in ['E', 'alpha', 'nu', 'contact_point', 'baseline']:
-        assert kk in fp2.keys()
-    # D: fit and get from fit_properties
-    idnt.fit_model(params_initial=fp2)
-    fp3 = idnt.get_initial_fit_parameters()
-    assert fp2 == fp3
-
-
-def test_get_model():
-    md = nanite.model.model_hertz_paraboloidal
-    model_name = "parabolic indenter (Hertz)"
-    md2 = nanite.model.get_model_by_name(model_name).module
-    assert md2 is md
-
-
-def test_preprocessing_reset():
-    fd = nanite.IndentationGroup(jpkfile)[0]
-    fd.apply_preprocessing(["compute_tip_position",
-                            "correct_force_offset",
-                            "correct_tip_offset"],
-                           options={"correct_tip_offset": {
-                               "method": "fit_constant_line"}})
-
-    inparams = nanite.model.model_hertz_paraboloidal.get_parameter_defaults()
-    inparams["baseline"].vary = True
-    inparams["contact_point"].set(1.8e-5)
-
-    # Perform fit and make sure that all properties are set
-    fd.fit_model(model_key="hertz_para",
-                 params_initial=inparams,
-                 range_x=(0, 0),
-                 range_type="absolute",
-                 x_axis="tip position",
-                 y_axis="force",
-                 segment="approach",
-                 weight_cp=False)
-    fd.rate_quality(training_set="zef18",
-                    regressor="Extra Trees")
-    assert fd._rating is not None
-    assert fd.preprocessing == ["compute_tip_position",
-                                "correct_force_offset",
-                                "correct_tip_offset"]
-    assert fd.preprocessing_options == {"correct_tip_offset": {
-                                        "method": "fit_constant_line"}}
-    assert not fd._preprocessing_details
-    assert np.allclose(
-        fd._fit_properties["params_fitted"]["contact_point"].value,
-        -3.5147555568064786e-06,
-        atol=0)
-    assert "tip position" in fd
-
-    # Change preprocessing and make sure properties are reset
-    fd.apply_preprocessing(["compute_tip_position",
-                            "correct_force_offset",
-                            "correct_tip_offset"],
-                           options={"correct_tip_offset": {
-                               "method": "fit_constant_polynomial"}})
-    assert fd._rating is None
-    assert fd.preprocessing == ["compute_tip_position",
-                                "correct_force_offset",
-                                "correct_tip_offset"]
-    assert fd.preprocessing_options == {"correct_tip_offset": {
-                                        "method": "fit_constant_polynomial"}}
-    assert not fd._preprocessing_details
-    assert "params_fitted" not in fd._fit_properties
-    assert "tip position" in fd
-
-    # Change preprocessing, removing tip position
-    fd.apply_preprocessing(["correct_force_offset"])
-    assert "tip position" not in fd
-
-
-def test_rate_quality_cache():
-    ds1 = nanite.IndentationGroup(jpkfile)
-    idnt = ds1[0]
-    idnt.apply_preprocessing(["compute_tip_position"])
-
-    inparams = nanite.model.model_hertz_paraboloidal.get_parameter_defaults()
-    inparams["baseline"].vary = True
-    inparams["contact_point"].set(1.8e-5)
-
-    # Fit with absolute full range
-    idnt.fit_model(model_key="hertz_para",
-                   params_initial=inparams,
-                   range_x=(0, 0),
-                   range_type="absolute",
-                   x_axis="tip position",
-                   y_axis="force",
-                   segment="approach",
-                   weight_cp=False)
-    r1 = idnt.rate_quality(training_set="zef18",
-                           regressor="Extra Trees")
-    assert idnt._rating[-1] == r1
-    r2 = idnt.rate_quality(training_set="zef18",
-                           regressor="Extra Trees")
-    assert r1 == r2
-
-
-def test_rate_quality_disabled():
-    ds1 = nanite.IndentationGroup(jpkfile)
-    idnt = ds1[0]
-    idnt.apply_preprocessing(["compute_tip_position"])
-
-    inparams = nanite.model.model_hertz_paraboloidal.get_parameter_defaults()
-    inparams["baseline"].vary = True
-    inparams["contact_point"].set(1.8e-5)
-
-    # Fit with absolute full range
-    idnt.fit_model(model_key="hertz_para",
-                   params_initial=inparams,
-                   range_x=(0, 0),
-                   range_type="absolute",
-                   x_axis="tip position",
-                   y_axis="force",
-                   segment="approach",
-                   weight_cp=False)
-
-    r1 = idnt.rate_quality(training_set="zef18",
-                           regressor="none")
-    assert r1 == -1
-
-
-def test_rate_quality_nofit():
-    ds1 = nanite.IndentationGroup(jpkfile)
-    idnt = ds1[0]
-    r1 = idnt.rate_quality()
-    assert r1 == -1
-
-
-def test_repr_str():
-    ds1 = nanite.IndentationGroup(jpkfile)
-    idnt = ds1[0]
-    assert "AFMForceDistance" not in str(idnt)
-    assert "Indentation" in str(idnt)
-    assert "fmt-jpk-fd_spot3-0192.jpk-force" in str(idnt)
-    assert "Indentation" in repr(idnt)
-    assert "fmt-jpk-fd_spot3-0192.jpk-force" in repr(idnt)
-
-
-if __name__ == "__main__":
-    # Run all tests
-    loc = locals()
-    for key in list(loc.keys()):
-        if key.startswith("test_") and hasattr(loc[key], "__call__"):
-            loc[key]()
+"""Test of data set functionalities"""
+import pathlib
+import tempfile
+
+import numpy as np
+import pytest
+
+import afmformats
+import nanite
+import nanite.model
+
+
+data_path = pathlib.Path(__file__).parent / "data"
+jpkfile = data_path / "fmt-jpk-fd_spot3-0192.jpk-force"
+
+
+def test_apply_preprocessing():
+    ds1 = nanite.IndentationGroup(jpkfile)
+    idnt = ds1[0]
+    # apply preprocessing by manually setting the list
+    idnt.preprocessing = ["compute_tip_position"]
+    idnt.apply_preprocessing()
+
+
+def test_apply_preprocessing_remember_fit_properties():
+    """
+    Normally, the fit properties would be overridden
+    if the preprocessing changes. For user convenience,
+    nanite remembers it. This is the test
+    """
+    ds1 = nanite.IndentationGroup(jpkfile)
+    idnt = ds1[0]
+    idnt.apply_preprocessing(["compute_tip_position"])
+
+    inparams = nanite.model.model_hertz_paraboloidal.get_parameter_defaults()
+    inparams["baseline"].vary = True
+    cp1 = 1.8029310065572342e-05
+    inparams["contact_point"].set(cp1)
+    inparams["contact_point"].vary = False
+
+    # Fit with absolute full range
+    idnt.fit_model(model_key="hertz_para",
+                   params_initial=inparams,
+                   range_x=(0, 0),
+                   range_type="absolute",
+                   x_axis="tip position",
+                   y_axis="force",
+                   segment="approach",
+                   weight_cp=False)
+    assert cp1 == idnt.fit_properties["params_initial"]["contact_point"].value
+    assert cp1 == idnt.fit_properties["params_fitted"]["contact_point"].value
+
+    # Change preprocessing
+    idnt.apply_preprocessing(["compute_tip_position",
+                              "correct_force_offset"])
+    assert cp1 == idnt.fit_properties["params_initial"]["contact_point"].value
+
+
+def test_basic():
+    ds1 = nanite.IndentationGroup(jpkfile)
+    idnt = ds1[0]
+    # tip-sample separation
+    idnt.apply_preprocessing(["compute_tip_position"])
+    assert idnt.preprocessing == ["compute_tip_position"]
+    assert idnt["tip position"][0] == 2.2803841798545836e-05
+    # correct for an offset in the tip
+    idnt.apply_preprocessing(["compute_tip_position",
+                              "correct_tip_offset"])
+    # This value is subject to change if a better way to estimate the
+    # contact point is found:
+    assert idnt["tip position"][0] == 4.765854684370548e-06
+
+
+def test_export():
+    ds1 = nanite.IndentationGroup(jpkfile)
+    idnt = ds1[0]
+    # tip-sample separation
+    idnt.apply_preprocessing(["compute_tip_position"])
+    # create temporary file
+    _, path = tempfile.mkstemp(suffix=".tab", prefix="nanite_idnt_export")
+    idnt.export_data(path)
+    data = afmformats.load_data(path)[0]
+    assert len(data) == 4000
+    assert np.allclose(data["force"][100], -4.853736717639109e-10)
+    assert np.allclose(data["height (measured)"][100], 2.256791903750211e-05,
+                       atol=1e-10, rtol=0)
+    assert data["segment"][100] == 0
+    assert np.allclose(data["time"][100], 0.04999999999999999)
+    assert np.allclose(data["tip position"][100], 2.255675939721752e-05,
+                       atol=1e-10, rtol=0)
+    assert data["segment"][3000] == 1
+
+
+def test_fitting():
+    ds1 = nanite.IndentationGroup(jpkfile)
+    idnt = ds1[0]
+    idnt.apply_preprocessing(["compute_tip_position"])
+
+    inparams = nanite.model.model_hertz_paraboloidal.get_parameter_defaults()
+    inparams["baseline"].vary = True
+    inparams["contact_point"].set(1.8e-5)
+
+    # Fit with absolute full range
+    idnt.fit_model(model_key="hertz_para",
+                   params_initial=inparams,
+                   range_x=(0, 0),
+                   range_type="absolute",
+                   x_axis="tip position",
+                   y_axis="force",
+                   segment="approach",
+                   weight_cp=False)
+    params = idnt.fit_properties["params_fitted"]
+    assert np.allclose(params["contact_point"].value, 1.8029310201193193e-05)
+    assert np.allclose(params["E"].value, 14741.958242422093,
+                       atol=1,
+                       rtol=0)
+
+    # Fit with absolute short
+    idnt.fit_model(model_key="hertz_para",
+                   params_initial=inparams,
+                   range_x=(17e-06, 19e-6),
+                   range_type="absolute",
+                   x_axis="tip position",
+                   y_axis="force",
+                   segment="approach",
+                   weight_cp=False)
+    params2 = idnt.fit_properties["params_fitted"]
+    assert np.allclose(params2["contact_point"].value, 1.8028461828272924e-05)
+    assert np.allclose(params2["E"].value, 14838.89245576058,
+                       atol=3,
+                       rtol=0)
+
+    # Fit with relative to initial fit
+    idnt.fit_model(model_key="hertz_para",
+                   params_initial=params2,
+                   range_x=(-2e-6, 1e-6),
+                   range_type="relative cp",
+                   x_axis="tip position",
+                   y_axis="force",
+                   segment="approach",
+                   weight_cp=False)
+    params3 = idnt.fit_properties["params_fitted"]
+    # These results are subject to change if the "relative cp" method is
+    # changed.
+    assert np.allclose(params3["contact_point"].value, 1.8028478083499856e-05)
+    assert np.allclose(params3["E"].value, 14838.010069354472,
+                       atol=2,
+                       rtol=0)
+
+
+@pytest.mark.filterwarnings('ignore::nanite.fit.FitWarning')
+def test_get_initial_fit_parameters():
+    """This is a convenience function"""
+    ds1 = nanite.IndentationGroup(jpkfile)
+    idnt = ds1[0]
+    # A: sanity check
+    fp = idnt.get_initial_fit_parameters()
+    assert fp["contact_point"].value == 0, "need to get tip position first"
+    # B: get default fit parameters (hertz_para)
+    idnt.apply_preprocessing(["compute_tip_position"])
+    fp = idnt.get_initial_fit_parameters()
+    for kk in ['E', 'R', 'nu', 'contact_point', 'baseline']:
+        assert kk in fp.keys()
+    # C: set other model and get fit parameters
+    idnt.fit_properties["model_key"] = "hertz_pyr3s"
+    fp2 = idnt.get_initial_fit_parameters()
+    for kk in ['E', 'alpha', 'nu', 'contact_point', 'baseline']:
+        assert kk in fp2.keys()
+    # D: fit and get from fit_properties
+    idnt.fit_model(params_initial=fp2)
+    fp3 = idnt.get_initial_fit_parameters()
+    assert fp2 == fp3
+
+
+def test_get_model():
+    md = nanite.model.model_hertz_paraboloidal
+    model_name = "parabolic indenter (Hertz)"
+    md2 = nanite.model.get_model_by_name(model_name).module
+    assert md2 is md
+
+
+def test_preprocessing_reset():
+    fd = nanite.IndentationGroup(jpkfile)[0]
+    fd.apply_preprocessing(["compute_tip_position",
+                            "correct_force_offset",
+                            "correct_tip_offset"],
+                           options={"correct_tip_offset": {
+                               "method": "fit_constant_line"}})
+
+    inparams = nanite.model.model_hertz_paraboloidal.get_parameter_defaults()
+    inparams["baseline"].vary = True
+    inparams["contact_point"].set(1.8e-5)
+
+    # Perform fit and make sure that all properties are set
+    fd.fit_model(model_key="hertz_para",
+                 params_initial=inparams,
+                 range_x=(0, 0),
+                 range_type="absolute",
+                 x_axis="tip position",
+                 y_axis="force",
+                 segment="approach",
+                 weight_cp=False)
+    fd.rate_quality(training_set="zef18",
+                    regressor="Extra Trees")
+    assert fd._rating is not None
+    assert fd.preprocessing == ["compute_tip_position",
+                                "correct_force_offset",
+                                "correct_tip_offset"]
+    assert fd.preprocessing_options == {"correct_tip_offset": {
+                                        "method": "fit_constant_line"}}
+    assert not fd._preprocessing_details
+    assert np.allclose(
+        fd._fit_properties["params_fitted"]["contact_point"].value,
+        -3.514699519428463e-06,
+        atol=0,
+        rtol=1e-4)
+    assert "tip position" in fd
+
+    # Change preprocessing and make sure properties are reset
+    fd.apply_preprocessing(["compute_tip_position",
+                            "correct_force_offset",
+                            "correct_tip_offset"],
+                           options={"correct_tip_offset": {
+                               "method": "fit_constant_polynomial"}})
+    assert fd._rating is None
+    assert fd.preprocessing == ["compute_tip_position",
+                                "correct_force_offset",
+                                "correct_tip_offset"]
+    assert fd.preprocessing_options == {"correct_tip_offset": {
+                                        "method": "fit_constant_polynomial"}}
+    assert not fd._preprocessing_details
+    assert "params_fitted" not in fd._fit_properties
+    assert "tip position" in fd
+
+    # Change preprocessing, removing tip position
+    fd.apply_preprocessing(["correct_force_offset"])
+    assert "tip position" not in fd
+
+
+def test_rate_quality_cache():
+    ds1 = nanite.IndentationGroup(jpkfile)
+    idnt = ds1[0]
+    idnt.apply_preprocessing(["compute_tip_position"])
+
+    inparams = nanite.model.model_hertz_paraboloidal.get_parameter_defaults()
+    inparams["baseline"].vary = True
+    inparams["contact_point"].set(1.8e-5)
+
+    # Fit with absolute full range
+    idnt.fit_model(model_key="hertz_para",
+                   params_initial=inparams,
+                   range_x=(0, 0),
+                   range_type="absolute",
+                   x_axis="tip position",
+                   y_axis="force",
+                   segment="approach",
+                   weight_cp=False)
+    r1 = idnt.rate_quality(training_set="zef18",
+                           regressor="Extra Trees")
+    assert idnt._rating[-1] == r1
+    r2 = idnt.rate_quality(training_set="zef18",
+                           regressor="Extra Trees")
+    assert r1 == r2
+
+
+def test_rate_quality_disabled():
+    ds1 = nanite.IndentationGroup(jpkfile)
+    idnt = ds1[0]
+    idnt.apply_preprocessing(["compute_tip_position"])
+
+    inparams = nanite.model.model_hertz_paraboloidal.get_parameter_defaults()
+    inparams["baseline"].vary = True
+    inparams["contact_point"].set(1.8e-5)
+
+    # Fit with absolute full range
+    idnt.fit_model(model_key="hertz_para",
+                   params_initial=inparams,
+                   range_x=(0, 0),
+                   range_type="absolute",
+                   x_axis="tip position",
+                   y_axis="force",
+                   segment="approach",
+                   weight_cp=False)
+
+    r1 = idnt.rate_quality(training_set="zef18",
+                           regressor="none")
+    assert r1 == -1
+
+
+def test_rate_quality_nofit():
+    ds1 = nanite.IndentationGroup(jpkfile)
+    idnt = ds1[0]
+    r1 = idnt.rate_quality()
+    assert r1 == -1
+
+
+def test_repr_str():
+    ds1 = nanite.IndentationGroup(jpkfile)
+    idnt = ds1[0]
+    assert "AFMForceDistance" not in str(idnt)
+    assert "Indentation" in str(idnt)
+    assert "fmt-jpk-fd_spot3-0192.jpk-force" in str(idnt)
+    assert "Indentation" in repr(idnt)
+    assert "fmt-jpk-fd_spot3-0192.jpk-force" in repr(idnt)
```

### Comparing `nanite-3.5.4/tests/test_indent2.py` & `nanite-3.6.0/tests/test_indent2.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-"""Test of data set functionalities"""
-import pathlib
-
-import numpy as np
-import pytest
-
-from nanite import IndentationGroup
-
-
-data_path = pathlib.Path(__file__).parent / "data"
-jpkfile = data_path / "fmt-jpk-fd_spot3-0192.jpk-force"
-
-
-@pytest.mark.filterwarnings('ignore::nanite.smooth.'
-                            + 'DoubledSmoothingWindowWarning')
-def test_app_ret():
-    grp = IndentationGroup(jpkfile)
-    idnt = grp[0]
-    idnt.apply_preprocessing(["compute_tip_position"])
-    height = np.array(idnt["height (measured)"], copy=True)
-    tip_position = np.array(idnt["tip position"], copy=True)
-    idnt.apply_preprocessing(["smooth_height"])
-    hms = np.array(idnt["height (measured)"])
-    assert not np.all(height == hms)
-    idnt.apply_preprocessing(["compute_tip_position",
-                              "smooth_height"])
-    hms2 = np.array(idnt["height (measured)"])
-    assert np.all(hms == hms2)
-    assert not np.all(idnt["tip position"] == tip_position)
-
-
-def test_tip_sample_separation():
-    grp = IndentationGroup(jpkfile)
-    idnt = grp[0]
-    # This computation correctly reproduces the column
-    # "Vertical Tip Position" as it is exported by the
-    # JPK analysis software with the checked option
-    # "Use Unsmoothed Height".
-    idnt.apply_preprocessing(["compute_tip_position"])
-    tip = np.array(idnt["tip position"])
-    assert tip[0] == 2.2803841798545836e-05
-
-
-def test_correct_app_ret():
-    grp = IndentationGroup(jpkfile)
-    idnt = grp[0]
-    idnt.apply_preprocessing(["compute_tip_position",
-                              "correct_split_approach_retract"])
-    a = idnt["segment"][idnt["segment"] == 0]
-    assert len(a) == 2006
-
-
-def test_correct_force_offset():
-    grp = IndentationGroup(jpkfile)
-    idnt = grp[0]
-    idnt.apply_preprocessing(["compute_tip_position",
-                              "correct_force_offset"])
-    idp = idnt.estimate_contact_point_index()
-    assert np.allclose(np.average(idnt["force"][:idp]), 0)
-
-
-@pytest.mark.parametrize(
-    "metadata,software",
-    [
-        (None, "JPK"),
-        ({"software": "custom1a"}, "custom1a"),
-    ])
-def test_metadata_override(metadata, software):
-    grp = IndentationGroup(jpkfile, meta_override=metadata)
-    idnt = grp[0]
-    assert idnt.metadata["software"] == software
+"""Test of data set functionalities"""
+import pathlib
+
+import numpy as np
+import pytest
+
+from nanite import IndentationGroup
+
+
+data_path = pathlib.Path(__file__).parent / "data"
+jpkfile = data_path / "fmt-jpk-fd_spot3-0192.jpk-force"
+
+
+@pytest.mark.filterwarnings('ignore::nanite.smooth.'
+                            + 'DoubledSmoothingWindowWarning')
+def test_app_ret():
+    grp = IndentationGroup(jpkfile)
+    idnt = grp[0]
+    idnt.apply_preprocessing(["compute_tip_position"])
+    height = np.array(idnt["height (measured)"], copy=True)
+    tip_position = np.array(idnt["tip position"], copy=True)
+    idnt.apply_preprocessing(["smooth_height"])
+    hms = np.array(idnt["height (measured)"])
+    assert not np.all(height == hms)
+    idnt.apply_preprocessing(["compute_tip_position",
+                              "smooth_height"])
+    hms2 = np.array(idnt["height (measured)"])
+    assert np.all(hms == hms2)
+    assert not np.all(idnt["tip position"] == tip_position)
+
+
+def test_tip_sample_separation():
+    grp = IndentationGroup(jpkfile)
+    idnt = grp[0]
+    # This computation correctly reproduces the column
+    # "Vertical Tip Position" as it is exported by the
+    # JPK analysis software with the checked option
+    # "Use Unsmoothed Height".
+    idnt.apply_preprocessing(["compute_tip_position"])
+    tip = np.array(idnt["tip position"])
+    assert tip[0] == 2.2803841798545836e-05
+
+
+def test_correct_app_ret():
+    grp = IndentationGroup(jpkfile)
+    idnt = grp[0]
+    idnt.apply_preprocessing(["compute_tip_position",
+                              "correct_split_approach_retract"])
+    a = idnt["segment"][idnt["segment"] == 0]
+    assert len(a) == 2006
+
+
+def test_correct_force_offset():
+    grp = IndentationGroup(jpkfile)
+    idnt = grp[0]
+    idnt.apply_preprocessing(["compute_tip_position",
+                              "correct_force_offset"])
+    idp = idnt.estimate_contact_point_index()
+    assert np.allclose(np.average(idnt["force"][:idp]), 0)
+
+
+@pytest.mark.parametrize(
+    "metadata,software",
+    [
+        (None, "JPK"),
+        ({"software": "custom1a"}, "custom1a"),
+    ])
+def test_metadata_override(metadata, software):
+    grp = IndentationGroup(jpkfile, meta_override=metadata)
+    idnt = grp[0]
+    assert idnt.metadata["software"] == software
```

### Comparing `nanite-3.5.4/tests/test_model_expr.py` & `nanite-3.6.0/tests/test_model_expr.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,135 +1,127 @@
-"""Test of models using expressions"""
-import pathlib
-
-import numpy as np
-
-from nanite import IndentationGroup
-
-from common import MockModelModuleExpr
-
-
-data_dir = pathlib.Path(__file__).resolve().parent / "data"
-jpkfile = data_dir / "fmt-jpk-fd_spot3-0192.jpk-force"
-
-
-def test_expr_model():
-    """Make sure that a model with an expression is fitted correctly"""
-    # Reference fit
-    rgrp = IndentationGroup(jpkfile)
-    ridnt = rgrp[0]
-    ridnt.apply_preprocessing(["compute_tip_position",
-                               "correct_force_offset"])
-    ridnt.fit_model(model_key="hertz_para",
-                    params_initial=None,
-                    x_axis="tip position",
-                    y_axis="force",
-                    weight_cp=False,
-                    segment="retract")
-    rparms = ridnt.fit_properties["params_fitted"]
-    remod = rparms["E"].value
-
-    with MockModelModuleExpr() as mod:
-        grp = IndentationGroup(jpkfile)
-        idnt = grp[0]
-        idnt.apply_preprocessing(["compute_tip_position",
-                                  "correct_force_offset"])
-        idnt.fit_model(model_key=mod.model_key,
-                       params_initial=None,
-                       x_axis="tip position",
-                       y_axis="force",
-                       weight_cp=False,
-                       segment="retract")
-        parms = idnt.fit_properties["params_fitted"]
-        # make sure the expression survives
-        assert parms["E1"].expr == "virtual_parameter+E"
-        emod = parms["E1"].value
-        # There are some difference due to heuristics
-        assert np.allclose(emod, remod, atol=0, rtol=3e-3)
-
-
-def test_expr_model_limit():
-    """Fit with a limit towards the correct solution"""
-    # Reference fit
-    rgrp = IndentationGroup(jpkfile)
-    ridnt = rgrp[0]
-    ridnt.apply_preprocessing(["compute_tip_position",
-                               "correct_force_offset"])
-    ridnt.fit_model(model_key="hertz_para",
-                    params_initial=None,
-                    x_axis="tip position",
-                    y_axis="force",
-                    weight_cp=False,
-                    segment="retract")
-    rparmsi = ridnt.fit_properties["params_initial"]
-
-    with MockModelModuleExpr() as mod:
-        grp = IndentationGroup(jpkfile)
-        idnt = grp[0]
-        idnt.apply_preprocessing(["compute_tip_position",
-                                  "correct_force_offset"])
-        params_initial = mod.get_parameter_defaults()
-        params_initial["E"].set(value=19000)
-        params_initial["virtual_parameter"].set(value=10, min=0, max=200)
-        params_initial["contact_point"].set(
-            value=rparmsi["contact_point"].value)
-        idnt.fit_model(model_key=mod.model_key,
-                       params_initial=params_initial,
-                       x_axis="tip position",
-                       y_axis="force",
-                       weight_cp=False,
-                       segment="retract")
-        parms = idnt.fit_properties["params_fitted"]
-        # make sure the expression survives
-        assert parms["E1"].expr == "virtual_parameter+E"
-        emod = parms["E1"].value
-        # It should have gone to the boundary
-        assert np.allclose(emod, 19200)
-
-
-def test_expr_model_sign():
-    """Fit with negative limit"""
-    # Reference fit
-    rgrp = IndentationGroup(jpkfile)
-    ridnt = rgrp[0]
-    ridnt.apply_preprocessing(["compute_tip_position",
-                               "correct_force_offset"])
-    ridnt.fit_model(model_key="hertz_para",
-                    params_initial=None,
-                    x_axis="tip position",
-                    y_axis="force",
-                    weight_cp=False,
-                    segment="retract")
-    rparms = ridnt.fit_properties["params_fitted"]
-    rparmsi = ridnt.fit_properties["params_initial"]
-    remod = rparms["E"].value
-
-    with MockModelModuleExpr() as mod:
-        grp = IndentationGroup(jpkfile)
-        idnt = grp[0]
-        idnt.apply_preprocessing(["compute_tip_position",
-                                  "correct_force_offset"])
-        params_initial = mod.get_parameter_defaults()
-        params_initial["E"].set(value=20000)
-        params_initial["virtual_parameter"].set(value=-1, min=-np.inf, max=0)
-        params_initial["contact_point"].set(
-            value=rparmsi["contact_point"].value)
-        idnt.fit_model(model_key=mod.model_key,
-                       params_initial=params_initial,
-                       x_axis="tip position",
-                       y_axis="force",
-                       weight_cp=False,
-                       segment="retract")
-        parms = idnt.fit_properties["params_fitted"]
-        # make sure the expression survives
-        assert parms["E1"].expr == "virtual_parameter+E"
-        emod = parms["E1"].value
-        # There are some difference due to heuristics
-        assert np.allclose(emod, remod, atol=0, rtol=3e-3)
-
-
-if __name__ == "__main__":
-    # Run all tests
-    loc = locals()
-    for key in list(loc.keys()):
-        if key.startswith("test_") and hasattr(loc[key], "__call__"):
-            loc[key]()
+"""Test of models using expressions"""
+import pathlib
+
+import numpy as np
+
+from nanite import IndentationGroup
+
+from common import MockModelModuleExpr
+
+
+data_dir = pathlib.Path(__file__).resolve().parent / "data"
+jpkfile = data_dir / "fmt-jpk-fd_spot3-0192.jpk-force"
+
+
+def test_expr_model():
+    """Make sure that a model with an expression is fitted correctly"""
+    # Reference fit
+    rgrp = IndentationGroup(jpkfile)
+    ridnt = rgrp[0]
+    ridnt.apply_preprocessing(["compute_tip_position",
+                               "correct_force_offset"])
+    ridnt.fit_model(model_key="hertz_para",
+                    params_initial=None,
+                    x_axis="tip position",
+                    y_axis="force",
+                    weight_cp=False,
+                    segment="retract")
+    rparms = ridnt.fit_properties["params_fitted"]
+    remod = rparms["E"].value
+
+    with MockModelModuleExpr() as mod:
+        grp = IndentationGroup(jpkfile)
+        idnt = grp[0]
+        idnt.apply_preprocessing(["compute_tip_position",
+                                  "correct_force_offset"])
+        idnt.fit_model(model_key=mod.model_key,
+                       params_initial=None,
+                       x_axis="tip position",
+                       y_axis="force",
+                       weight_cp=False,
+                       segment="retract")
+        parms = idnt.fit_properties["params_fitted"]
+        # make sure the expression survives
+        assert parms["E1"].expr == "virtual_parameter+E"
+        emod = parms["E1"].value
+        # There are some difference due to heuristics
+        assert np.allclose(emod, remod, atol=0, rtol=3e-3)
+
+
+def test_expr_model_limit():
+    """Fit with a limit towards the correct solution"""
+    # Reference fit
+    rgrp = IndentationGroup(jpkfile)
+    ridnt = rgrp[0]
+    ridnt.apply_preprocessing(["compute_tip_position",
+                               "correct_force_offset"])
+    ridnt.fit_model(model_key="hertz_para",
+                    params_initial=None,
+                    x_axis="tip position",
+                    y_axis="force",
+                    weight_cp=False,
+                    segment="retract")
+    rparmsi = ridnt.fit_properties["params_initial"]
+
+    with MockModelModuleExpr() as mod:
+        grp = IndentationGroup(jpkfile)
+        idnt = grp[0]
+        idnt.apply_preprocessing(["compute_tip_position",
+                                  "correct_force_offset"])
+        params_initial = mod.get_parameter_defaults()
+        params_initial["E"].set(value=19000)
+        params_initial["virtual_parameter"].set(value=10, min=0, max=200)
+        params_initial["contact_point"].set(
+            value=rparmsi["contact_point"].value)
+        idnt.fit_model(model_key=mod.model_key,
+                       params_initial=params_initial,
+                       x_axis="tip position",
+                       y_axis="force",
+                       weight_cp=False,
+                       segment="retract")
+        parms = idnt.fit_properties["params_fitted"]
+        # make sure the expression survives
+        assert parms["E1"].expr == "virtual_parameter+E"
+        emod = parms["E1"].value
+        # It should have gone to the boundary
+        assert np.allclose(emod, 19200)
+
+
+def test_expr_model_sign():
+    """Fit with negative limit"""
+    # Reference fit
+    rgrp = IndentationGroup(jpkfile)
+    ridnt = rgrp[0]
+    ridnt.apply_preprocessing(["compute_tip_position",
+                               "correct_force_offset"])
+    ridnt.fit_model(model_key="hertz_para",
+                    params_initial=None,
+                    x_axis="tip position",
+                    y_axis="force",
+                    weight_cp=False,
+                    segment="retract")
+    rparms = ridnt.fit_properties["params_fitted"]
+    rparmsi = ridnt.fit_properties["params_initial"]
+    remod = rparms["E"].value
+
+    with MockModelModuleExpr() as mod:
+        grp = IndentationGroup(jpkfile)
+        idnt = grp[0]
+        idnt.apply_preprocessing(["compute_tip_position",
+                                  "correct_force_offset"])
+        params_initial = mod.get_parameter_defaults()
+        params_initial["E"].set(value=20000)
+        params_initial["virtual_parameter"].set(value=-1, min=-np.inf, max=0)
+        params_initial["contact_point"].set(
+            value=rparmsi["contact_point"].value)
+        idnt.fit_model(model_key=mod.model_key,
+                       params_initial=params_initial,
+                       x_axis="tip position",
+                       y_axis="force",
+                       weight_cp=False,
+                       segment="retract")
+        parms = idnt.fit_properties["params_fitted"]
+        # make sure the expression survives
+        assert parms["E1"].expr == "virtual_parameter+E"
+        emod = parms["E1"].value
+        # There are some difference due to heuristics
+        assert np.allclose(emod, remod, atol=0, rtol=3e-3)
```

### Comparing `nanite-3.5.4/tests/test_model_hertz_cone.py` & `nanite-3.6.0/tests/test_model_hertz_cone.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,105 +1,105 @@
-"""Test of data set functionalities"""
-import pathlib
-
-import lmfit
-import numpy as np
-
-from nanite import IndentationGroup
-from nanite.model import model_conical_indenter as hertz_conical
-
-
-data_path = pathlib.Path(__file__).resolve().parent / "data"
-jpkfile = data_path / "fmt-jpk-fd_spot3-0192.jpk-force"
-
-
-def test_app_ret():
-    ds = IndentationGroup(jpkfile)
-    ar = ds[0]
-    ar.apply_preprocessing(["compute_tip_position",
-                            "correct_force_offset"])
-    idp = ar.estimate_contact_point_index()
-
-    aprid = ar["segment"] == 0
-    x = ar["tip position"][aprid]
-    y = ar["force"][aprid]
-    contact_point = x[idp]
-
-    # crop x and y around contact_point
-    distcp = x.shape[0]-idp
-    x = x[-3*distcp:]
-    y = y[-3*distcp:]
-
-    params = lmfit.Parameters()
-    params.add("contact_point", value=contact_point)
-    params.add("baseline", value=0, vary=False)
-    params.add("E", value=300e3, min=0)
-    params.add("nu", value=.5, vary=False)
-    params.add("alpha", value=30, vary=False)
-
-    fit_w = lmfit.minimize(hertz_conical.residual, params, args=(x, y, True))
-    fit_n = lmfit.minimize(hertz_conical.residual, params, args=(x, y, False))
-
-    # Correctly reproduces fit results in the JPK analysis software
-    # with "Vertical Tip Position", "Switchable Baseline Operation",
-    # and a conical indenter with the "Hertz/Sneddon" "Model type".
-    # The contact point was calculated through Hertz model and not adjusted
-    # before fitting by JPK Software.
-    # Set half cone angle to 30 Deg.
-    E_jpk = 348.6e3
-    cp_jpk = 18.06e-6
-    assert np.allclose(fit_n.params["E"].value, E_jpk, rtol=8e-2, atol=0)
-    assert np.allclose(
-        fit_n.params["contact_point"].value, cp_jpk, rtol=4e-3, atol=0)
-
-    if __name__ == "__main__" and False:
-        import matplotlib.pylab as plt
-        _fig, axes = plt.subplots(2, 1)
-        xf = np.linspace(x[0], x[-1], 100)
-        axes[0].plot(xf, hertz_conical.model(
-            fit_w.params, xf), label="fit with weights")
-        axes[0].plot(xf, hertz_conical.model(
-            fit_n.params, xf), label="fit no weights")
-        axes[0].plot(x, y, label="data")
-        axes[0].legend()
-        axes[0].grid()
-
-        axes[1].plot(x, hertz_conical.residual(fit_w.params, x, y,
-                                               weight_cp=True),
-                     label="residuals with weight")
-        axes[1].plot(x, hertz_conical.residual(fit_n.params, x, y,
-                                               weight_cp=False),
-                     label="residuals no weight")
-        axes[1].legend()
-        axes[1].grid()
-
-        plt.show()
-
-
-def test_fit_apret():
-    ds = IndentationGroup(jpkfile)
-    ar = ds[0]
-    ar.apply_preprocessing(["compute_tip_position",
-                            "correct_force_offset"])
-    ar.fit_model(model_key="hertz_cone",
-                 params_initial=None,
-                 x_axis="tip position",
-                 y_axis="force",
-                 weight_cp=False,
-                 segment="retract")
-
-    if __name__ == "__main__":
-        import matplotlib.pylab as plt
-        _fig, axes = plt.subplots(2, 1)
-        axes[0].plot(ar["tip position"], ar["force"], label="data")
-        axes[0].plot(ar["tip position"], ar["fit"], label="fit")
-        axes[0].legend()
-        axes[0].grid()
-        plt.show()
-
-
-if __name__ == "__main__":
-    # Run all tests
-    loc = locals()
-    for key in list(loc.keys()):
-        if key.startswith("test_") and hasattr(loc[key], "__call__"):
-            loc[key]()
+"""Test of data set functionalities"""
+import pathlib
+
+import lmfit
+import numpy as np
+
+from nanite import IndentationGroup
+from nanite.model import model_conical_indenter as hertz_conical
+
+
+data_path = pathlib.Path(__file__).resolve().parent / "data"
+jpkfile = data_path / "fmt-jpk-fd_spot3-0192.jpk-force"
+
+
+def test_app_ret():
+    ds = IndentationGroup(jpkfile)
+    ar = ds[0]
+    ar.apply_preprocessing(["compute_tip_position",
+                            "correct_force_offset"])
+    idp = ar.estimate_contact_point_index()
+
+    aprid = ar["segment"] == 0
+    x = ar["tip position"][aprid]
+    y = ar["force"][aprid]
+    contact_point = x[idp]
+
+    # crop x and y around contact_point
+    distcp = x.shape[0]-idp
+    x = x[-3*distcp:]
+    y = y[-3*distcp:]
+
+    params = lmfit.Parameters()
+    params.add("contact_point", value=contact_point)
+    params.add("baseline", value=0, vary=False)
+    params.add("E", value=300e3, min=0)
+    params.add("nu", value=.5, vary=False)
+    params.add("alpha", value=30, vary=False)
+
+    fit_w = lmfit.minimize(hertz_conical.residual, params, args=(x, y, True))
+    fit_n = lmfit.minimize(hertz_conical.residual, params, args=(x, y, False))
+
+    # Correctly reproduces fit results in the JPK analysis software
+    # with "Vertical Tip Position", "Switchable Baseline Operation",
+    # and a conical indenter with the "Hertz/Sneddon" "Model type".
+    # The contact point was calculated through Hertz model and not adjusted
+    # before fitting by JPK Software.
+    # Set half cone angle to 30 Deg.
+    E_jpk = 348.6e3
+    cp_jpk = 18.06e-6
+    assert np.allclose(fit_n.params["E"].value, E_jpk, rtol=8e-2, atol=0)
+    assert np.allclose(
+        fit_n.params["contact_point"].value, cp_jpk, rtol=4e-3, atol=0)
+
+    if __name__ == "__main__" and False:
+        import matplotlib.pylab as plt
+        _fig, axes = plt.subplots(2, 1)
+        xf = np.linspace(x[0], x[-1], 100)
+        axes[0].plot(xf, hertz_conical.model(
+            fit_w.params, xf), label="fit with weights")
+        axes[0].plot(xf, hertz_conical.model(
+            fit_n.params, xf), label="fit no weights")
+        axes[0].plot(x, y, label="data")
+        axes[0].legend()
+        axes[0].grid()
+
+        axes[1].plot(x, hertz_conical.residual(fit_w.params, x, y,
+                                               weight_cp=True),
+                     label="residuals with weight")
+        axes[1].plot(x, hertz_conical.residual(fit_n.params, x, y,
+                                               weight_cp=False),
+                     label="residuals no weight")
+        axes[1].legend()
+        axes[1].grid()
+
+        plt.show()
+
+
+def test_fit_apret():
+    ds = IndentationGroup(jpkfile)
+    ar = ds[0]
+    ar.apply_preprocessing(["compute_tip_position",
+                            "correct_force_offset"])
+    ar.fit_model(model_key="hertz_cone",
+                 params_initial=None,
+                 x_axis="tip position",
+                 y_axis="force",
+                 weight_cp=False,
+                 segment="retract")
+
+    if __name__ == "__main__":
+        import matplotlib.pylab as plt
+        _fig, axes = plt.subplots(2, 1)
+        axes[0].plot(ar["tip position"], ar["force"], label="data")
+        axes[0].plot(ar["tip position"], ar["fit"], label="fit")
+        axes[0].legend()
+        axes[0].grid()
+        plt.show()
+
+
+if __name__ == "__main__":
+    # Run all tests
+    loc = locals()
+    for key in list(loc.keys()):
+        if key.startswith("test_") and hasattr(loc[key], "__call__"):
+            loc[key]()
```

### Comparing `nanite-3.5.4/tests/test_model_hertz_parabol.py` & `nanite-3.6.0/tests/test_model_hertz_parabol.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,100 +1,100 @@
-"""Test of data set functionalities"""
-import pathlib
-
-import lmfit
-import numpy as np
-
-from nanite import IndentationGroup
-from nanite.model import model_hertz_paraboloidal as hertz
-
-
-data_path = pathlib.Path(__file__).resolve().parent / "data"
-jpkfile = data_path / "fmt-jpk-fd_spot3-0192.jpk-force"
-
-
-def test_app_ret():
-    grp = IndentationGroup(jpkfile)
-    idnt = grp[0]
-    idnt.apply_preprocessing(["compute_tip_position",
-                              "correct_force_offset"])
-    idp = idnt.estimate_contact_point_index()
-
-    aprid = idnt["segment"] == 0
-    x = idnt["tip position"][aprid]
-    y = idnt["force"][aprid]
-    contact_point = x[idp]
-
-    # crop x and y around contact_point
-    distcp = x.shape[0]-idp
-    x = x[-3*distcp:]
-    y = y[-3*distcp:]
-
-    params = lmfit.Parameters()
-    params.add("contact_point", value=contact_point)
-    params.add("baseline", value=0, vary=False)
-    params.add("E", value=300e3, min=0)
-    params.add("nu", value=.5, vary=False)
-    params.add("R", value=40e-9, vary=False)
-
-    fit_w = lmfit.minimize(hertz.residual, params, args=(x, y, True))
-    fit_n = lmfit.minimize(hertz.residual, params, args=(x, y, False))
-
-    # Correctly reproduces fit results in the JPK analysis software
-    # with "Vertical Tip Position", "Switchable Baseline Operation",
-    # and a parabolic indenter with the "Hertz/Sneddon" "Model type".
-    # Set tip radius to 40nm.
-    E_jpk = 233.1e3
-    cp_jpk = 18.03e-6
-    assert np.allclose(fit_n.params["E"].value, E_jpk, rtol=2e-3, atol=0)
-    assert np.allclose(
-        fit_n.params["contact_point"].value, cp_jpk, rtol=4e-5, atol=0)
-
-    if __name__ == "__main__" and False:
-        import matplotlib.pylab as plt
-        _fig, axes = plt.subplots(2, 1)
-        xf = np.linspace(x[0], x[-1], 100)
-        axes[0].plot(xf, hertz.model(fit_w.params, xf),
-                     label="fit with weights")
-        axes[0].plot(xf, hertz.model(fit_n.params, xf), label="fit no weights")
-        axes[0].plot(x, y, label="data")
-        axes[0].legend()
-        axes[0].grid()
-
-        axes[1].plot(x, hertz.residual(fit_w.params, x, y, weight_cp=True),
-                     label="residuals with weight")
-        axes[1].plot(x, hertz.residual(fit_n.params, x, y, weight_cp=False),
-                     label="residuals no weight")
-        axes[1].legend()
-        axes[1].grid()
-
-        plt.show()
-
-
-def test_fit_apret():
-    grp = IndentationGroup(jpkfile)
-    idnt = grp[0]
-    idnt.apply_preprocessing(["compute_tip_position",
-                              "correct_force_offset"])
-    idnt.fit_model(model_key="hertz_para",
-                   params_initial=None,
-                   x_axis="tip position",
-                   y_axis="force",
-                   weight_cp=False,
-                   segment="retract")
-
-    if __name__ == "__main__":
-        import matplotlib.pylab as plt
-        _fig, axes = plt.subplots(2, 1)
-        axes[0].plot(idnt["tip position"], idnt["force"], label="data")
-        axes[0].plot(idnt["tip position"], idnt["fit"], label="fit")
-        axes[0].legend()
-        axes[0].grid()
-        plt.show()
-
-
-if __name__ == "__main__":
-    # Run all tests
-    loc = locals()
-    for key in list(loc.keys()):
-        if key.startswith("test_") and hasattr(loc[key], "__call__"):
-            loc[key]()
+"""Test of data set functionalities"""
+import pathlib
+
+import lmfit
+import numpy as np
+
+from nanite import IndentationGroup
+from nanite.model import model_hertz_paraboloidal as hertz
+
+
+data_path = pathlib.Path(__file__).resolve().parent / "data"
+jpkfile = data_path / "fmt-jpk-fd_spot3-0192.jpk-force"
+
+
+def test_app_ret():
+    grp = IndentationGroup(jpkfile)
+    idnt = grp[0]
+    idnt.apply_preprocessing(["compute_tip_position",
+                              "correct_force_offset"])
+    idp = idnt.estimate_contact_point_index()
+
+    aprid = idnt["segment"] == 0
+    x = idnt["tip position"][aprid]
+    y = idnt["force"][aprid]
+    contact_point = x[idp]
+
+    # crop x and y around contact_point
+    distcp = x.shape[0]-idp
+    x = x[-3*distcp:]
+    y = y[-3*distcp:]
+
+    params = lmfit.Parameters()
+    params.add("contact_point", value=contact_point)
+    params.add("baseline", value=0, vary=False)
+    params.add("E", value=300e3, min=0)
+    params.add("nu", value=.5, vary=False)
+    params.add("R", value=40e-9, vary=False)
+
+    fit_w = lmfit.minimize(hertz.residual, params, args=(x, y, True))
+    fit_n = lmfit.minimize(hertz.residual, params, args=(x, y, False))
+
+    # Correctly reproduces fit results in the JPK analysis software
+    # with "Vertical Tip Position", "Switchable Baseline Operation",
+    # and a parabolic indenter with the "Hertz/Sneddon" "Model type".
+    # Set tip radius to 40nm.
+    E_jpk = 233.1e3
+    cp_jpk = 18.03e-6
+    assert np.allclose(fit_n.params["E"].value, E_jpk, rtol=2e-3, atol=0)
+    assert np.allclose(
+        fit_n.params["contact_point"].value, cp_jpk, rtol=4e-5, atol=0)
+
+    if __name__ == "__main__" and False:
+        import matplotlib.pylab as plt
+        _fig, axes = plt.subplots(2, 1)
+        xf = np.linspace(x[0], x[-1], 100)
+        axes[0].plot(xf, hertz.model(fit_w.params, xf),
+                     label="fit with weights")
+        axes[0].plot(xf, hertz.model(fit_n.params, xf), label="fit no weights")
+        axes[0].plot(x, y, label="data")
+        axes[0].legend()
+        axes[0].grid()
+
+        axes[1].plot(x, hertz.residual(fit_w.params, x, y, weight_cp=True),
+                     label="residuals with weight")
+        axes[1].plot(x, hertz.residual(fit_n.params, x, y, weight_cp=False),
+                     label="residuals no weight")
+        axes[1].legend()
+        axes[1].grid()
+
+        plt.show()
+
+
+def test_fit_apret():
+    grp = IndentationGroup(jpkfile)
+    idnt = grp[0]
+    idnt.apply_preprocessing(["compute_tip_position",
+                              "correct_force_offset"])
+    idnt.fit_model(model_key="hertz_para",
+                   params_initial=None,
+                   x_axis="tip position",
+                   y_axis="force",
+                   weight_cp=False,
+                   segment="retract")
+
+    if __name__ == "__main__":
+        import matplotlib.pylab as plt
+        _fig, axes = plt.subplots(2, 1)
+        axes[0].plot(idnt["tip position"], idnt["force"], label="data")
+        axes[0].plot(idnt["tip position"], idnt["fit"], label="fit")
+        axes[0].legend()
+        axes[0].grid()
+        plt.show()
+
+
+if __name__ == "__main__":
+    # Run all tests
+    loc = locals()
+    for key in list(loc.keys()):
+        if key.startswith("test_") and hasattr(loc[key], "__call__"):
+            loc[key]()
```

### Comparing `nanite-3.5.4/tests/test_model_hertz_pyramid_three.py` & `nanite-3.6.0/tests/test_model_hertz_pyramid_three.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,102 +1,102 @@
-"""Test of data set functionalities"""
-import pathlib
-
-import lmfit
-import numpy as np
-
-from nanite import IndentationGroup
-from nanite.model import model_hertz_three_sided_pyramid as mod_tsp
-
-
-data_path = pathlib.Path(__file__).resolve().parent / "data"
-jpkfile = data_path / "fmt-jpk-fd_spot3-0192.jpk-force"
-
-
-def test_app_ret():
-    ds = IndentationGroup(jpkfile)
-    ar = ds[0]
-    ar.apply_preprocessing(["compute_tip_position",
-                            "correct_force_offset"])
-    idp = ar.estimate_contact_point_index()
-
-    aprid = ar["segment"] == 0
-    x = ar["tip position"][aprid]
-    y = ar["force"][aprid]
-    contact_point = x[idp]
-
-    # crop x and y around contact_point
-    distcp = x.shape[0]-idp
-    x = x[-3*distcp:]
-    y = y[-3*distcp:]
-
-    params = lmfit.Parameters()
-    params.add("contact_point", value=contact_point)
-    params.add("baseline", value=0, vary=False)
-    params.add("E", value=350e3, min=0)
-    params.add("nu", value=.5, vary=False)
-    params.add("alpha", value=20, vary=False)
-
-    fit_w = lmfit.minimize(mod_tsp.residual, params, args=(x, y, True))
-    fit_n = lmfit.minimize(mod_tsp.residual, params, args=(x, y, False))
-    # Correctly reproduces fit results in the JPK analysis software
-    # with "Vertical Tip Position", "Switchable Baseline Operation",
-    # and a Triangular Pyramid indenter with the "Hertz/Sneddon" "Model type".
-    # The contact point was calculated through Hertz model and not adjusted
-    # before fitting by JPK Software.
-    # Set half angle to face to 20 Deg.
-    E_jpk = 396.1e3
-    cp_jpk = 18.06e-6
-    assert np.allclose(fit_n.params["E"].value, E_jpk, rtol=8e-2, atol=0)
-    assert np.allclose(
-        fit_n.params["contact_point"].value, cp_jpk, rtol=4e-3, atol=0)
-
-    if __name__ == "__main__" and False:
-        import matplotlib.pylab as plt
-        _fig, axes = plt.subplots(2, 1)
-        xf = np.linspace(x[0], x[-1], 100)
-        axes[0].plot(xf, mod_tsp.model(fit_w.params, xf),
-                     label="fit with weights")
-        axes[0].plot(xf, mod_tsp.model(fit_n.params, xf),
-                     label="fit no weights")
-        axes[0].plot(x, y, label="data")
-        axes[0].legend()
-        axes[0].grid()
-
-        axes[1].plot(x, mod_tsp.residual(fit_w.params, x, y, weight_cp=True),
-                     label="residuals with weight")
-        axes[1].plot(x, mod_tsp.residual(fit_n.params, x, y, weight_cp=False),
-                     label="residuals no weight")
-        axes[1].legend()
-        axes[1].grid()
-
-        plt.show()
-
-
-def test_fit_apret():
-    ds = IndentationGroup(jpkfile)
-    ar = ds[0]
-    ar.apply_preprocessing(["compute_tip_position",
-                            "correct_force_offset"])
-    ar.fit_model(model_key="hertz_pyr3s",
-                 params_initial=None,
-                 x_axis="tip position",
-                 y_axis="force",
-                 weight_cp=False,
-                 segment="retract")
-
-    if __name__ == "__main__":
-        import matplotlib.pylab as plt
-        _fig, axes = plt.subplots(2, 1)
-        axes[0].plot(ar["tip position"], ar["force"], label="data")
-        axes[0].plot(ar["tip position"], ar["fit"], label="fit")
-        axes[0].legend()
-        axes[0].grid()
-        plt.show()
-
-
-if __name__ == "__main__":
-    # Run all tests
-    loc = locals()
-    for key in list(loc.keys()):
-        if key.startswith("test_") and hasattr(loc[key], "__call__"):
-            loc[key]()
+"""Test of data set functionalities"""
+import pathlib
+
+import lmfit
+import numpy as np
+
+from nanite import IndentationGroup
+from nanite.model import model_hertz_three_sided_pyramid as mod_tsp
+
+
+data_path = pathlib.Path(__file__).resolve().parent / "data"
+jpkfile = data_path / "fmt-jpk-fd_spot3-0192.jpk-force"
+
+
+def test_app_ret():
+    ds = IndentationGroup(jpkfile)
+    ar = ds[0]
+    ar.apply_preprocessing(["compute_tip_position",
+                            "correct_force_offset"])
+    idp = ar.estimate_contact_point_index()
+
+    aprid = ar["segment"] == 0
+    x = ar["tip position"][aprid]
+    y = ar["force"][aprid]
+    contact_point = x[idp]
+
+    # crop x and y around contact_point
+    distcp = x.shape[0]-idp
+    x = x[-3*distcp:]
+    y = y[-3*distcp:]
+
+    params = lmfit.Parameters()
+    params.add("contact_point", value=contact_point)
+    params.add("baseline", value=0, vary=False)
+    params.add("E", value=350e3, min=0)
+    params.add("nu", value=.5, vary=False)
+    params.add("alpha", value=20, vary=False)
+
+    fit_w = lmfit.minimize(mod_tsp.residual, params, args=(x, y, True))
+    fit_n = lmfit.minimize(mod_tsp.residual, params, args=(x, y, False))
+    # Correctly reproduces fit results in the JPK analysis software
+    # with "Vertical Tip Position", "Switchable Baseline Operation",
+    # and a Triangular Pyramid indenter with the "Hertz/Sneddon" "Model type".
+    # The contact point was calculated through Hertz model and not adjusted
+    # before fitting by JPK Software.
+    # Set half angle to face to 20 Deg.
+    E_jpk = 396.1e3
+    cp_jpk = 18.06e-6
+    assert np.allclose(fit_n.params["E"].value, E_jpk, rtol=8e-2, atol=0)
+    assert np.allclose(
+        fit_n.params["contact_point"].value, cp_jpk, rtol=4e-3, atol=0)
+
+    if __name__ == "__main__" and False:
+        import matplotlib.pylab as plt
+        _fig, axes = plt.subplots(2, 1)
+        xf = np.linspace(x[0], x[-1], 100)
+        axes[0].plot(xf, mod_tsp.model(fit_w.params, xf),
+                     label="fit with weights")
+        axes[0].plot(xf, mod_tsp.model(fit_n.params, xf),
+                     label="fit no weights")
+        axes[0].plot(x, y, label="data")
+        axes[0].legend()
+        axes[0].grid()
+
+        axes[1].plot(x, mod_tsp.residual(fit_w.params, x, y, weight_cp=True),
+                     label="residuals with weight")
+        axes[1].plot(x, mod_tsp.residual(fit_n.params, x, y, weight_cp=False),
+                     label="residuals no weight")
+        axes[1].legend()
+        axes[1].grid()
+
+        plt.show()
+
+
+def test_fit_apret():
+    ds = IndentationGroup(jpkfile)
+    ar = ds[0]
+    ar.apply_preprocessing(["compute_tip_position",
+                            "correct_force_offset"])
+    ar.fit_model(model_key="hertz_pyr3s",
+                 params_initial=None,
+                 x_axis="tip position",
+                 y_axis="force",
+                 weight_cp=False,
+                 segment="retract")
+
+    if __name__ == "__main__":
+        import matplotlib.pylab as plt
+        _fig, axes = plt.subplots(2, 1)
+        axes[0].plot(ar["tip position"], ar["force"], label="data")
+        axes[0].plot(ar["tip position"], ar["fit"], label="fit")
+        axes[0].legend()
+        axes[0].grid()
+        plt.show()
+
+
+if __name__ == "__main__":
+    # Run all tests
+    loc = locals()
+    for key in list(loc.keys()):
+        if key.startswith("test_") and hasattr(loc[key], "__call__"):
+            loc[key]()
```

### Comparing `nanite-3.5.4/tests/test_model_logic.py` & `nanite-3.6.0/tests/test_model_logic.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-import pathlib
-
-import nanite
-
-
-data_dir = pathlib.Path(__file__).parent / "data"
-
-
-def test_load_model_from_file():
-    mpath = data_dir / "model_external_basic.py"
-    md = nanite.model.load_model_from_file(mpath, register=True)
-    assert md.model_key == "hans_peter"
-    assert md.model_key in nanite.model.models_available
-    nanite.model.deregister_model(md)
-    assert md.model_key not in nanite.model.models_available
-
-
-def test_load_model_from_model():
-    mpath = data_dir / "model_external_basic.py"
-    md = nanite.model.load_model_from_file(mpath, register=False)
-    assert md.model_key == "hans_peter"
-    assert md.model_key not in nanite.model.models_available
-    md2 = nanite.model.register_model(md)
-    assert md is md2
-    assert md.model_key in nanite.model.models_available
-    nanite.model.deregister_model(md)
-    assert md.model_key not in nanite.model.models_available
+import pathlib
+
+import nanite
+
+
+data_dir = pathlib.Path(__file__).parent / "data"
+
+
+def test_load_model_from_file():
+    mpath = data_dir / "model_external_basic.py"
+    md = nanite.model.load_model_from_file(mpath, register=True)
+    assert md.model_key == "hans_peter"
+    assert md.model_key in nanite.model.models_available
+    nanite.model.deregister_model(md)
+    assert md.model_key not in nanite.model.models_available
+
+
+def test_load_model_from_model():
+    mpath = data_dir / "model_external_basic.py"
+    md = nanite.model.load_model_from_file(mpath, register=False)
+    assert md.model_key == "hans_peter"
+    assert md.model_key not in nanite.model.models_available
+    md2 = nanite.model.register_model(md)
+    assert md is md2
+    assert md.model_key in nanite.model.models_available
+    nanite.model.deregister_model(md)
+    assert md.model_key not in nanite.model.models_available
```

### Comparing `nanite-3.5.4/tests/test_model_sneddon_spherical_approximation.py` & `nanite-3.6.0/tests/test_model_sneddon_spherical_approximation.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,91 +1,91 @@
-"""Test of data set functionalities"""
-import pathlib
-
-import lmfit
-import numpy as np
-
-from nanite import IndentationGroup
-from nanite.model import model_sneddon_spherical_approximation as mod_ssa
-
-
-data_path = pathlib.Path(__file__).resolve().parent / "data"
-jpkfile = data_path / "fmt-jpk-fd_spot3-0192.jpk-force"
-
-
-def test_app_ret():
-    ds = IndentationGroup(jpkfile)
-    ar = ds[0]
-    ar.apply_preprocessing(["compute_tip_position",
-                            "correct_force_offset"])
-    idp = ar.estimate_contact_point_index()
-
-    aprid = ar["segment"] == 0
-    x = ar["tip position"][aprid]
-    y = ar["force"][aprid]
-    contact_point = x[idp]
-
-    # crop x and y around contact_point
-    distcp = x.shape[0]-idp
-    x = x[-3*distcp:]
-    y = y[-3*distcp:]
-
-    params = lmfit.Parameters()
-    params.add("contact_point", value=contact_point)
-    params.add("baseline", value=0, vary=False)
-    params.add("E", value=300e3, min=0)
-    params.add("nu", value=.5, vary=False)
-    params.add("R", value=40e-9, vary=False)
-
-    fit_w = lmfit.minimize(mod_ssa.residual, params, args=(x, y, True))
-    fit_n = lmfit.minimize(mod_ssa.residual, params, args=(x, y, False))
-
-    if __name__ == "__main__" and False:
-        import matplotlib.pylab as plt
-        _fig, axes = plt.subplots(2, 1)
-        xf = np.linspace(x[0], x[-1], 100)
-        axes[0].plot(xf, mod_ssa.model(fit_w.params, xf),
-                     label="fit with weights")
-        axes[0].plot(xf, mod_ssa.model(fit_n.params, xf),
-                     label="fit no weights")
-        axes[0].plot(x, y, label="data")
-        axes[0].legend()
-        axes[0].grid()
-
-        axes[1].plot(x, mod_ssa.residual(fit_w.params, x, y, weight_cp=True),
-                     label="residuals with weight")
-        axes[1].plot(x, mod_ssa.residual(fit_n.params, x, y, weight_cp=False),
-                     label="residuals no weight")
-        axes[1].legend()
-        axes[1].grid()
-
-        plt.show()
-
-
-def test_fit_apret():
-    ds = IndentationGroup(jpkfile)
-    ar = ds[0]
-    ar.apply_preprocessing(["compute_tip_position",
-                            "correct_force_offset"])
-    ar.fit_model(model_key="sneddon_spher_approx",
-                 params_initial=None,
-                 x_axis="tip position",
-                 y_axis="force",
-                 weight_cp=False,
-                 segment="retract")
-
-    if __name__ == "__main__":
-        import matplotlib.pylab as plt
-        _fig, axes = plt.subplots(2, 1)
-        axes[0].plot(ar["tip position"], ar["force"], label="data")
-        axes[0].plot(ar["tip position"], ar["fit"], label="fit")
-        axes[0].legend()
-        axes[0].grid()
-        plt.show()
-
-
-if __name__ == "__main__":
-    # Run all tests
-    loc = locals()
-    for key in list(loc.keys()):
-        if key.startswith("test_") and hasattr(loc[key], "__call__"):
-            loc[key]()
+"""Test of data set functionalities"""
+import pathlib
+
+import lmfit
+import numpy as np
+
+from nanite import IndentationGroup
+from nanite.model import model_sneddon_spherical_approximation as mod_ssa
+
+
+data_path = pathlib.Path(__file__).resolve().parent / "data"
+jpkfile = data_path / "fmt-jpk-fd_spot3-0192.jpk-force"
+
+
+def test_app_ret():
+    ds = IndentationGroup(jpkfile)
+    ar = ds[0]
+    ar.apply_preprocessing(["compute_tip_position",
+                            "correct_force_offset"])
+    idp = ar.estimate_contact_point_index()
+
+    aprid = ar["segment"] == 0
+    x = ar["tip position"][aprid]
+    y = ar["force"][aprid]
+    contact_point = x[idp]
+
+    # crop x and y around contact_point
+    distcp = x.shape[0]-idp
+    x = x[-3*distcp:]
+    y = y[-3*distcp:]
+
+    params = lmfit.Parameters()
+    params.add("contact_point", value=contact_point)
+    params.add("baseline", value=0, vary=False)
+    params.add("E", value=300e3, min=0)
+    params.add("nu", value=.5, vary=False)
+    params.add("R", value=40e-9, vary=False)
+
+    fit_w = lmfit.minimize(mod_ssa.residual, params, args=(x, y, True))
+    fit_n = lmfit.minimize(mod_ssa.residual, params, args=(x, y, False))
+
+    if __name__ == "__main__" and False:
+        import matplotlib.pylab as plt
+        _fig, axes = plt.subplots(2, 1)
+        xf = np.linspace(x[0], x[-1], 100)
+        axes[0].plot(xf, mod_ssa.model(fit_w.params, xf),
+                     label="fit with weights")
+        axes[0].plot(xf, mod_ssa.model(fit_n.params, xf),
+                     label="fit no weights")
+        axes[0].plot(x, y, label="data")
+        axes[0].legend()
+        axes[0].grid()
+
+        axes[1].plot(x, mod_ssa.residual(fit_w.params, x, y, weight_cp=True),
+                     label="residuals with weight")
+        axes[1].plot(x, mod_ssa.residual(fit_n.params, x, y, weight_cp=False),
+                     label="residuals no weight")
+        axes[1].legend()
+        axes[1].grid()
+
+        plt.show()
+
+
+def test_fit_apret():
+    ds = IndentationGroup(jpkfile)
+    ar = ds[0]
+    ar.apply_preprocessing(["compute_tip_position",
+                            "correct_force_offset"])
+    ar.fit_model(model_key="sneddon_spher_approx",
+                 params_initial=None,
+                 x_axis="tip position",
+                 y_axis="force",
+                 weight_cp=False,
+                 segment="retract")
+
+    if __name__ == "__main__":
+        import matplotlib.pylab as plt
+        _fig, axes = plt.subplots(2, 1)
+        axes[0].plot(ar["tip position"], ar["force"], label="data")
+        axes[0].plot(ar["tip position"], ar["fit"], label="fit")
+        axes[0].legend()
+        axes[0].grid()
+        plt.show()
+
+
+if __name__ == "__main__":
+    # Run all tests
+    loc = locals()
+    for key in list(loc.keys()):
+        if key.startswith("test_") and hasattr(loc[key], "__call__"):
+            loc[key]()
```

### Comparing `nanite-3.5.4/tests/test_model_style.py` & `nanite-3.6.0/tests/test_model_style.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,61 +1,53 @@
-"""Test model integrity"""
-from nanite import model
-
-
-NAME_MAPPING = {
-    "alpha": ["Face Angle", "Half Cone Angle"],
-    "baseline": ["Force Baseline"],
-    "contact_point": ["Contact Point"],
-    "E": ["Young's Modulus"],
-    "nu": ["Poisson's Ratio"],
-    "R": "Tip Radius",
-}
-
-UNIT_MAPPING = {
-    "alpha": "°",
-    "baseline": "N",
-    "contact_point": "m",
-    "E": "Pa",
-    "nu": "",
-    "R": "m",
-}
-
-
-def test_model_parameter_name_order():
-    for key in model.models_available:
-        md = model.models_available[key]
-        std = md.get_parameter_defaults()
-        for n1, n2 in zip(list(std.keys()), md.parameter_keys):
-            assert n1 == n2, "Parameter defaults probably in wrong order!"
-
-
-def test_model_parameter_names():
-    for key in model.models_available:
-        md = model.models_available[key]
-        for key2, nn in zip(md.parameter_keys, md.parameter_names):
-            if key2 in NAME_MAPPING:
-                assert nn in NAME_MAPPING[key2], "bad {} in {}".format(
-                    key2, md)
-            else:
-                msg = "Parameter {} not registered for test!".format(key2)
-                assert False, msg
-
-
-def test_model_parameter_units():
-    for key in model.models_available:
-        md = model.models_available[key]
-        for key2, un in zip(md.parameter_keys, md.parameter_units):
-            if key2 in UNIT_MAPPING:
-                assert UNIT_MAPPING[key2] == un, "bad {} in {}".format(
-                    key2, md)
-            else:
-                msg = "Parameter {} not registered for test!".format(key2)
-                assert False, msg
-
-
-if __name__ == "__main__":
-    # Run all tests
-    loc = locals()
-    for _key in list(loc.keys()):
-        if _key.startswith("test_") and hasattr(loc[_key], "__call__"):
-            loc[_key]()
+"""Test model integrity"""
+from nanite import model
+
+
+NAME_MAPPING = {
+    "alpha": ["Face Angle", "Half Cone Angle"],
+    "baseline": ["Force Baseline"],
+    "contact_point": ["Contact Point"],
+    "E": ["Young's Modulus"],
+    "nu": ["Poisson's Ratio"],
+    "R": "Tip Radius",
+}
+
+UNIT_MAPPING = {
+    "alpha": "°",
+    "baseline": "N",
+    "contact_point": "m",
+    "E": "Pa",
+    "nu": "",
+    "R": "m",
+}
+
+
+def test_model_parameter_name_order():
+    for key in model.models_available:
+        md = model.models_available[key]
+        std = md.get_parameter_defaults()
+        for n1, n2 in zip(list(std.keys()), md.parameter_keys):
+            assert n1 == n2, "Parameter defaults probably in wrong order!"
+
+
+def test_model_parameter_names():
+    for key in model.models_available:
+        md = model.models_available[key]
+        for key2, nn in zip(md.parameter_keys, md.parameter_names):
+            if key2 in NAME_MAPPING:
+                assert nn in NAME_MAPPING[key2], "bad {} in {}".format(
+                    key2, md)
+            else:
+                msg = "Parameter {} not registered for test!".format(key2)
+                assert False, msg
+
+
+def test_model_parameter_units():
+    for key in model.models_available:
+        md = model.models_available[key]
+        for key2, un in zip(md.parameter_keys, md.parameter_units):
+            if key2 in UNIT_MAPPING:
+                assert UNIT_MAPPING[key2] == un, "bad {} in {}".format(
+                    key2, md)
+            else:
+                msg = "Parameter {} not registered for test!".format(key2)
+                assert False, msg
```

### Comparing `nanite-3.5.4/tests/test_open_jpk_variation.py` & `nanite-3.6.0/tests/test_open_jpk_variation.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,28 @@
-"""Test opening of file format variations"""
-import pathlib
-import numpy as np
-
-from nanite import IndentationGroup
-
-data_path = pathlib.Path(__file__).resolve().parent / "data"
-
-
-def test_process_flipsign():
-    # This is a curve extracted from a map file. When loading it
-    # with nanite, the sign of the force curve was flipped.
-    flipped = (data_path
-               / "fmt-jpk-fd_flipsign_2015.05.22-15.31.49.352.jpk-force")
-    idnt = IndentationGroup(flipped)[0]
-    idnt.apply_preprocessing(["compute_tip_position",
-                              "correct_force_offset",
-                              "correct_tip_offset",
-                              "correct_split_approach_retract"])
-    # We set the baseline fixed, because this test was written so)
-    params_initial = idnt.get_initial_fit_parameters(model_key="hertz_para")
-    params_initial["baseline"].set(vary=False)
-    idnt.fit_model(model_key="hertz_para", weight_cp=False,
-                   params_initial=params_initial)
-    assert np.allclose(idnt.fit_properties["params_fitted"]["E"].value,
-                       5230.008779761989,
-                       atol=1,
-                       rtol=0)
-
-
-if __name__ == "__main__":
-    # Run all tests
-    loc = locals()
-    for key in list(loc.keys()):
-        if key.startswith("test_") and hasattr(loc[key], "__call__"):
-            loc[key]()
+"""Test opening of file format variations"""
+import pathlib
+import numpy as np
+
+from nanite import IndentationGroup
+
+data_path = pathlib.Path(__file__).resolve().parent / "data"
+
+
+def test_process_flipsign():
+    # This is a curve extracted from a map file. When loading it
+    # with nanite, the sign of the force curve was flipped.
+    flipped = (data_path
+               / "fmt-jpk-fd_flipsign_2015.05.22-15.31.49.352.jpk-force")
+    idnt = IndentationGroup(flipped)[0]
+    idnt.apply_preprocessing(["compute_tip_position",
+                              "correct_force_offset",
+                              "correct_tip_offset",
+                              "correct_split_approach_retract"])
+    # We set the baseline fixed, because this test was written so)
+    params_initial = idnt.get_initial_fit_parameters(model_key="hertz_para")
+    params_initial["baseline"].set(vary=False)
+    idnt.fit_model(model_key="hertz_para", weight_cp=False,
+                   params_initial=params_initial)
+    assert np.allclose(idnt.fit_properties["params_fitted"]["E"].value,
+                       5230.008779761989,
+                       atol=1,
+                       rtol=0)
```

### Comparing `nanite-3.5.4/tests/test_poc.py` & `nanite-3.6.0/tests/test_poc.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,111 +1,111 @@
-"""Test point of contact (POC) estimation"""
-import pathlib
-
-import numpy as np
-import pytest
-
-from nanite import poc, IndentationGroup
-
-
-data_path = pathlib.Path(__file__).resolve().parent / "data"
-
-
-@pytest.mark.parametrize("method,contact_point", [
-    ["gradient_zero_crossing", 1895],
-    ["fit_constant_line", 1919],
-    ["fit_constant_polynomial", 1898],
-    ["fit_line_polynomial", 1899],
-    ["frechet_direct_path", 1903],
-    ["deviation_from_baseline", 1908],
-])
-def test_poc_estimation(method, contact_point):
-    fd = IndentationGroup(data_path / "fmt-jpk-fd_spot3-0192.jpk-force")[0]
-    fd.apply_preprocessing(["compute_tip_position",
-                            "correct_force_offset"])
-    assert poc.compute_poc(fd["force"], method) == contact_point
-
-
-@pytest.mark.parametrize("method,contact_point", [
-    ["gradient_zero_crossing", 1895],
-    ["fit_constant_line", 1919],
-    ["fit_constant_polynomial", 1898],
-    ["fit_line_polynomial", 1899],
-    ["frechet_direct_path", 1903],
-    ["deviation_from_baseline", 1908],
-])
-def test_poc_estimation_details(method, contact_point):
-    fd = IndentationGroup(data_path / "fmt-jpk-fd_spot3-0192.jpk-force")[0]
-    fd.apply_preprocessing(["compute_tip_position",
-                            "correct_force_offset"])
-    _, details = poc.compute_poc(fd["force"], method, ret_details=True)
-    assert np.all(np.array(details["plot poc"][0]) == contact_point)
-
-
-@pytest.mark.parametrize("method,contact_point", [
-    ["gradient_zero_crossing", 1895],
-    ["fit_constant_line", 1919],
-    ["fit_constant_polynomial", 1898],
-    ["fit_line_polynomial", 1899],
-    ["frechet_direct_path", 1903],
-    ["deviation_from_baseline", 1908],
-])
-def test_poc_estimation_via_indent(method, contact_point):
-    fd = IndentationGroup(data_path / "fmt-jpk-fd_spot3-0192.jpk-force")[0]
-    fd.apply_preprocessing(["compute_tip_position",
-                            "correct_force_offset",
-                            "correct_tip_offset"],
-                           options={"correct_tip_offset": {"method": method}})
-    assert np.argmin(np.abs(fd["tip position"])) == contact_point
-
-
-def test_poc_details_deviation_from_baseline():
-    fd = IndentationGroup(data_path / "fmt-jpk-fd_spot3-0192.jpk-force")[0]
-    details = fd.apply_preprocessing(
-        ["compute_tip_position", "correct_force_offset", "correct_tip_offset"],
-        options={"correct_tip_offset": {"method": "deviation_from_baseline"}},
-        ret_details=True)
-    pocd = details["correct_tip_offset"]
-    for key in ["plot force",
-                "plot baseline mean",
-                "plot baseline threshold",
-                "plot poc"]:
-        assert key in pocd
-    assert np.allclose(
-        np.mean(pocd["plot baseline threshold"][1]),
-        8.431890003513514e-11,
-        atol=0)
-    assert np.allclose(
-        np.mean(pocd["plot baseline mean"][1]),
-        -7.573822405258677e-12,
-        atol=0)
-
-
-def test_poc_details_fit_line_polynomial():
-    fd = IndentationGroup(
-        data_path
-        / "fmt-jpk-fd_single_tilted-baseline-mitotic_2021-01-29.jpk-force")[0]
-    details = fd.apply_preprocessing(
-        ["compute_tip_position", "correct_tip_offset"],
-        options={"correct_tip_offset": {"method": "fit_line_polynomial"}},
-        ret_details=True)
-    pocd = details["correct_tip_offset"]
-    for key in ["plot force",
-                "plot fit",
-                "plot poc"]:
-        assert key in pocd
-    assert np.allclose(
-        pocd["plot poc"][0][0],
-        15602,
-        atol=0)
-    assert np.allclose(
-        fd["force"][15602],
-        1.7313584441928315e-09,
-        atol=0,
-    )
-
-
-def test_poc_frechet_direct_path():
-    force = np.zeros(100)
-    force[50:] = np.arange(50)**2
-    cp = poc.poc_frechet_direct_path(force)
-    assert cp == 62  # makes sense
+"""Test point of contact (POC) estimation"""
+import pathlib
+
+import numpy as np
+import pytest
+
+from nanite import poc, IndentationGroup
+
+
+data_path = pathlib.Path(__file__).resolve().parent / "data"
+
+
+@pytest.mark.parametrize("method,contact_point", [
+    ["gradient_zero_crossing", 1895],
+    ["fit_constant_line", 1919],
+    ["fit_constant_polynomial", 1898],
+    ["fit_line_polynomial", 1899],
+    ["frechet_direct_path", 1903],
+    ["deviation_from_baseline", 1908],
+])
+def test_poc_estimation(method, contact_point):
+    fd = IndentationGroup(data_path / "fmt-jpk-fd_spot3-0192.jpk-force")[0]
+    fd.apply_preprocessing(["compute_tip_position",
+                            "correct_force_offset"])
+    assert poc.compute_poc(fd["force"], method) == contact_point
+
+
+@pytest.mark.parametrize("method,contact_point", [
+    ["gradient_zero_crossing", 1895],
+    ["fit_constant_line", 1919],
+    ["fit_constant_polynomial", 1898],
+    ["fit_line_polynomial", 1899],
+    ["frechet_direct_path", 1903],
+    ["deviation_from_baseline", 1908],
+])
+def test_poc_estimation_details(method, contact_point):
+    fd = IndentationGroup(data_path / "fmt-jpk-fd_spot3-0192.jpk-force")[0]
+    fd.apply_preprocessing(["compute_tip_position",
+                            "correct_force_offset"])
+    _, details = poc.compute_poc(fd["force"], method, ret_details=True)
+    assert np.all(np.array(details["plot poc"][0]) == contact_point)
+
+
+@pytest.mark.parametrize("method,contact_point", [
+    ["gradient_zero_crossing", 1895],
+    ["fit_constant_line", 1919],
+    ["fit_constant_polynomial", 1898],
+    ["fit_line_polynomial", 1899],
+    ["frechet_direct_path", 1903],
+    ["deviation_from_baseline", 1908],
+])
+def test_poc_estimation_via_indent(method, contact_point):
+    fd = IndentationGroup(data_path / "fmt-jpk-fd_spot3-0192.jpk-force")[0]
+    fd.apply_preprocessing(["compute_tip_position",
+                            "correct_force_offset",
+                            "correct_tip_offset"],
+                           options={"correct_tip_offset": {"method": method}})
+    assert np.argmin(np.abs(fd["tip position"])) == contact_point
+
+
+def test_poc_details_deviation_from_baseline():
+    fd = IndentationGroup(data_path / "fmt-jpk-fd_spot3-0192.jpk-force")[0]
+    details = fd.apply_preprocessing(
+        ["compute_tip_position", "correct_force_offset", "correct_tip_offset"],
+        options={"correct_tip_offset": {"method": "deviation_from_baseline"}},
+        ret_details=True)
+    pocd = details["correct_tip_offset"]
+    for key in ["plot force",
+                "plot baseline mean",
+                "plot baseline threshold",
+                "plot poc"]:
+        assert key in pocd
+    assert np.allclose(
+        np.mean(pocd["plot baseline threshold"][1]),
+        8.431890003513514e-11,
+        atol=0)
+    assert np.allclose(
+        np.mean(pocd["plot baseline mean"][1]),
+        -7.573822405258677e-12,
+        atol=0)
+
+
+def test_poc_details_fit_line_polynomial():
+    fd = IndentationGroup(
+        data_path
+        / "fmt-jpk-fd_single_tilted-baseline-mitotic_2021-01-29.jpk-force")[0]
+    details = fd.apply_preprocessing(
+        ["compute_tip_position", "correct_tip_offset"],
+        options={"correct_tip_offset": {"method": "fit_line_polynomial"}},
+        ret_details=True)
+    pocd = details["correct_tip_offset"]
+    for key in ["plot force",
+                "plot fit",
+                "plot poc"]:
+        assert key in pocd
+    assert np.allclose(
+        pocd["plot poc"][0][0],
+        15602,
+        atol=0)
+    assert np.allclose(
+        fd["force"][15602],
+        1.7313584441928315e-09,
+        atol=0,
+    )
+
+
+def test_poc_frechet_direct_path():
+    force = np.zeros(100)
+    force[50:] = np.arange(50)**2
+    cp = poc.poc_frechet_direct_path(force)
+    assert cp == 62  # makes sense
```

### Comparing `nanite-3.5.4/tests/test_preproc.py` & `nanite-3.6.0/tests/test_preproc.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,155 +1,147 @@
-"""Test preprocessing"""
-import pathlib
-
-import numpy as np
-import pytest
-
-from nanite import IndentationGroup
-from nanite import preproc
-
-
-data_path = pathlib.Path(__file__).resolve().parent / "data"
-bad_files = list(data_path.glob("bad*"))
-
-
-def test_autosort():
-    unsorted = ["correct_force_offset",
-                "correct_tip_offset",
-                "compute_tip_position"]
-    expected = ["correct_force_offset",
-                "compute_tip_position",
-                "correct_tip_offset"]
-    actual = preproc.autosort(unsorted)
-    assert expected == actual
-
-
-def test_autosort2():
-    unsorted = ["correct_split_approach_retract",
-                "correct_force_offset",
-                "correct_tip_offset",
-                "compute_tip_position",
-                ]
-    expected = ["compute_tip_position",
-                "correct_split_approach_retract",
-                "correct_force_offset",
-                "correct_tip_offset",
-                ]
-    actual = preproc.autosort(unsorted)
-    assert (actual.index("correct_split_approach_retract")
-            > actual.index("compute_tip_position"))
-    assert (actual.index("correct_tip_offset")
-            > actual.index("compute_tip_position"))
-    assert expected == actual
-
-
-def test_autosort3():
-    unsorted = ["smooth_height",
-                "correct_split_approach_retract",
-                "correct_force_offset",
-                "correct_tip_offset",
-                "compute_tip_position",
-                ]
-    expected = ["compute_tip_position",
-                "correct_split_approach_retract",
-                "smooth_height",
-                "correct_force_offset",
-                "correct_tip_offset",
-                ]
-    actual = preproc.autosort(unsorted)
-    assert expected == actual
-    assert (actual.index("correct_split_approach_retract")
-            > actual.index("compute_tip_position"))
-    assert (actual.index("correct_tip_offset")
-            > actual.index("compute_tip_position"))
-    assert (actual.index("smooth_height")
-            > actual.index("correct_split_approach_retract"))
-
-
-def test_check_order():
-    with pytest.raises(ValueError, match="Wrong optional step order"):
-        preproc.check_order([
-            "smooth_height",
-            "correct_split_approach_retract"])
-
-
-def test_correct_split_approach_retract():
-    fd = IndentationGroup(data_path / "fmt-jpk-fd_spot3-0192.jpk-force")[0]
-
-    fd.apply_preprocessing(["compute_tip_position",
-                            "correct_force_offset",
-                            "correct_tip_offset"])
-    assert fd.appr["segment"].size == 2000
-    fd.apply_preprocessing(["compute_tip_position",
-                            "correct_force_offset",
-                            "correct_tip_offset",
-                            "correct_split_approach_retract"])
-    assert fd.appr["segment"].size == 2006
-
-
-def test_get_steps_required():
-    req_act = preproc.get_steps_required("correct_tip_offset")
-    req_exp = ["compute_tip_position"]
-    assert req_act == req_exp
-
-
-@pytest.mark.filterwarnings('ignore::nanite.preproc.CannotSplitWarning',
-                            'ignore::UserWarning')
-def test_process_bad():
-    for bf in bad_files:
-        ds = IndentationGroup(bf)
-        for idnt in ds:
-            # Walk through the standard analysis pipeline without
-            # throwing any exceptions.
-            idnt.apply_preprocessing(["compute_tip_position",
-                                      "correct_force_offset",
-                                      "correct_tip_offset",
-                                      "correct_split_approach_retract"])
-            idnt.fit_model()
-
-
-@pytest.mark.filterwarnings(
-    'ignore::nanite.smooth.DoubledSmoothingWindowWarning:')
-def test_smooth():
-    idnt = IndentationGroup(data_path / "fmt-jpk-fd_spot3-0192.jpk-force")[0]
-    idnt.apply_preprocessing(["compute_tip_position",
-                              "correct_force_offset",
-                              "correct_tip_offset"])
-    orig = np.array(idnt["tip position"], copy=True)
-    # now apply smoothing filter
-    idnt.apply_preprocessing(["compute_tip_position",
-                              "correct_force_offset",
-                              "correct_tip_offset",
-                              "smooth_height"])
-    new = np.array(idnt["tip position"], copy=True)
-    assert not np.all(orig == new)
-
-
-def test_unknown_method():
-    idnt = IndentationGroup(data_path / "fmt-jpk-fd_spot3-0192.jpk-force")[0]
-    with pytest.raises(KeyError, match="unknown_method"):
-        idnt.apply_preprocessing(["compute_tip_position",
-                                  "unknown_method"])
-
-
-def test_wrong_order():
-    idnt = IndentationGroup(data_path / "fmt-jpk-fd_spot3-0192.jpk-force")[0]
-    with pytest.raises(ValueError, match="requires the steps"):
-        # order matters
-        idnt.apply_preprocessing(["correct_tip_offset",
-                                  "compute_tip_position"])
-
-
-def test_wrong_order_2():
-    idnt = IndentationGroup(data_path / "fmt-jpk-fd_spot3-0192.jpk-force")[0]
-    with pytest.raises(ValueError, match="requires the steps"):
-        # order matters
-        idnt.apply_preprocessing(["correct_split_approach_retract",
-                                  "compute_tip_position"])
-
-
-if __name__ == "__main__":
-    # Run all tests
-    loc = locals()
-    for key in list(loc.keys()):
-        if key.startswith("test_") and hasattr(loc[key], "__call__"):
-            loc[key]()
+"""Test preprocessing"""
+import pathlib
+
+import numpy as np
+import pytest
+
+from nanite import IndentationGroup
+from nanite import preproc
+
+
+data_path = pathlib.Path(__file__).resolve().parent / "data"
+bad_files = list(data_path.glob("bad*"))
+
+
+def test_autosort():
+    unsorted = ["correct_force_offset",
+                "correct_tip_offset",
+                "compute_tip_position"]
+    expected = ["correct_force_offset",
+                "compute_tip_position",
+                "correct_tip_offset"]
+    actual = preproc.autosort(unsorted)
+    assert expected == actual
+
+
+def test_autosort2():
+    unsorted = ["correct_split_approach_retract",
+                "correct_force_offset",
+                "correct_tip_offset",
+                "compute_tip_position",
+                ]
+    expected = ["compute_tip_position",
+                "correct_split_approach_retract",
+                "correct_force_offset",
+                "correct_tip_offset",
+                ]
+    actual = preproc.autosort(unsorted)
+    assert (actual.index("correct_split_approach_retract")
+            > actual.index("compute_tip_position"))
+    assert (actual.index("correct_tip_offset")
+            > actual.index("compute_tip_position"))
+    assert expected == actual
+
+
+def test_autosort3():
+    unsorted = ["smooth_height",
+                "correct_split_approach_retract",
+                "correct_force_offset",
+                "correct_tip_offset",
+                "compute_tip_position",
+                ]
+    expected = ["compute_tip_position",
+                "correct_split_approach_retract",
+                "smooth_height",
+                "correct_force_offset",
+                "correct_tip_offset",
+                ]
+    actual = preproc.autosort(unsorted)
+    assert expected == actual
+    assert (actual.index("correct_split_approach_retract")
+            > actual.index("compute_tip_position"))
+    assert (actual.index("correct_tip_offset")
+            > actual.index("compute_tip_position"))
+    assert (actual.index("smooth_height")
+            > actual.index("correct_split_approach_retract"))
+
+
+def test_check_order():
+    with pytest.raises(ValueError, match="Wrong optional step order"):
+        preproc.check_order([
+            "smooth_height",
+            "correct_split_approach_retract"])
+
+
+def test_correct_split_approach_retract():
+    fd = IndentationGroup(data_path / "fmt-jpk-fd_spot3-0192.jpk-force")[0]
+
+    fd.apply_preprocessing(["compute_tip_position",
+                            "correct_force_offset",
+                            "correct_tip_offset"])
+    assert fd.appr["segment"].size == 2000
+    fd.apply_preprocessing(["compute_tip_position",
+                            "correct_force_offset",
+                            "correct_tip_offset",
+                            "correct_split_approach_retract"])
+    assert fd.appr["segment"].size == 2006
+
+
+def test_get_steps_required():
+    req_act = preproc.get_steps_required("correct_tip_offset")
+    req_exp = ["compute_tip_position"]
+    assert req_act == req_exp
+
+
+@pytest.mark.filterwarnings('ignore::nanite.preproc.CannotSplitWarning',
+                            'ignore::UserWarning')
+def test_process_bad():
+    for bf in bad_files:
+        ds = IndentationGroup(bf)
+        for idnt in ds:
+            # Walk through the standard analysis pipeline without
+            # throwing any exceptions.
+            idnt.apply_preprocessing(["compute_tip_position",
+                                      "correct_force_offset",
+                                      "correct_tip_offset",
+                                      "correct_split_approach_retract"])
+            idnt.fit_model()
+
+
+@pytest.mark.filterwarnings(
+    'ignore::nanite.smooth.DoubledSmoothingWindowWarning:')
+def test_smooth():
+    idnt = IndentationGroup(data_path / "fmt-jpk-fd_spot3-0192.jpk-force")[0]
+    idnt.apply_preprocessing(["compute_tip_position",
+                              "correct_force_offset",
+                              "correct_tip_offset"])
+    orig = np.array(idnt["tip position"], copy=True)
+    # now apply smoothing filter
+    idnt.apply_preprocessing(["compute_tip_position",
+                              "correct_force_offset",
+                              "correct_tip_offset",
+                              "smooth_height"])
+    new = np.array(idnt["tip position"], copy=True)
+    assert not np.all(orig == new)
+
+
+def test_unknown_method():
+    idnt = IndentationGroup(data_path / "fmt-jpk-fd_spot3-0192.jpk-force")[0]
+    with pytest.raises(KeyError, match="unknown_method"):
+        idnt.apply_preprocessing(["compute_tip_position",
+                                  "unknown_method"])
+
+
+def test_wrong_order():
+    idnt = IndentationGroup(data_path / "fmt-jpk-fd_spot3-0192.jpk-force")[0]
+    with pytest.raises(ValueError, match="requires the steps"):
+        # order matters
+        idnt.apply_preprocessing(["correct_tip_offset",
+                                  "compute_tip_position"])
+
+
+def test_wrong_order_2():
+    idnt = IndentationGroup(data_path / "fmt-jpk-fd_spot3-0192.jpk-force")[0]
+    with pytest.raises(ValueError, match="requires the steps"):
+        # order matters
+        idnt.apply_preprocessing(["correct_split_approach_retract",
+                                  "compute_tip_position"])
```

### Comparing `nanite-3.5.4/tests/test_qmap.py` & `nanite-3.6.0/tests/test_qmap.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,205 +1,197 @@
-"""Test qmap feature"""
-import pathlib
-import warnings
-
-import numpy as np
-
-from nanite import model, qmap, IndentationGroup
-
-
-data_path = pathlib.Path(__file__).resolve().parent / "data"
-jpkfile = data_path / "fmt-jpk-fd_map2x2_extracted.jpk-force-map"
-jpkfile2 = data_path / "fmt-jpk-fd_map-data-reference-points.jpk-force-map"
-
-
-def test_feat_scan_order():
-    qm = qmap.QMap(jpkfile)
-    order = qm.get_qmap("data: scan order", qmap_only=True)
-    assert order[0, 0] == 0
-    assert order[0, -1] == 1
-    assert order[-1, -1] == 2
-    assert order[-1, 0] == 3
-    assert np.isnan(order[0, 1])
-
-
-def test_feat_min_height():
-    qm = qmap.QMap(jpkfile)
-    qd = qm.get_qmap("data: height base point", qmap_only=True)
-    assert np.allclose(qd[0, 0], 40.55030392499141)
-    assert np.allclose(qd[0, -1], 47.354988549298945)
-    assert np.allclose(qd[-1, -1], 96.1627883099352)
-    assert np.allclose(qd[-1, 0], 89.95170867840217)
-
-
-def test_feat_cp():
-    qm = qmap.QMap(jpkfile2)
-    # fit data
-    for idnt in qm.group:
-        idnt.apply_preprocessing(["compute_tip_position",
-                                  "correct_force_offset",
-                                  "correct_tip_offset",
-                                  ])
-        inparams = model.model_sneddon_spherical_approximation \
-            .get_parameter_defaults()
-        inparams["E"].value = 50
-        inparams["R"].value = 37.28e-6 / 2
-        inparams["baseline"].vary = False
-
-        # Fit with absolute full range
-        idnt.fit_model(model_key="sneddon_spher_approx",
-                       params_initial=inparams,
-                       range_x=(0, 0),
-                       range_type="absolute",
-                       x_axis="tip position",
-                       y_axis="force",
-                       segment="approach",
-                       weight_cp=2e-6)
-
-    qd = qm.get_qmap("fit: contact point", qmap_only=True)
-    vals = qd.flat[~np.isnan(qd.flat)]
-    # These are subject to change when contact point preprocessing
-    # changes.
-    assert np.allclose(vals[0], -1820.431327293334), "gray matter"
-    assert np.allclose(vals[2], -3581.010097829371), "white matter"
-    assert np.allclose(vals[1], -2106.9835957851064), "background"
-
-
-def test_feat_emod_nofit():
-    qm = qmap.QMap(jpkfile)
-    with warnings.catch_warnings(record=True) as w:
-        # No data available, because there is no fit
-        qd = qm.get_qmap("fit: Young's modulus", qmap_only=True)
-        assert len(w) == 4
-        assert w[0].category is qmap.DataMissingWarning
-    assert np.alltrue(np.isnan(qd))
-
-
-def test_feat_emod_withfit():
-    qm = qmap.QMap(jpkfile2)
-    # fit data
-    for idnt in qm.group:
-        idnt.apply_preprocessing(["compute_tip_position",
-                                  "correct_force_offset",
-                                  "correct_tip_offset",
-                                  ])
-        inparams = model.model_sneddon_spherical_approximation \
-            .get_parameter_defaults()
-        inparams["E"].value = 50
-        inparams["R"].value = 37.28e-6 / 2
-        inparams["baseline"].vary = False
-
-        # Fit with absolute full range
-        idnt.fit_model(model_key="sneddon_spher_approx",
-                       params_initial=inparams,
-                       range_x=(0, 0),
-                       range_type="absolute",
-                       x_axis="tip position",
-                       y_axis="force",
-                       segment="approach",
-                       weight_cp=2e-6)
-
-    qd = qm.get_qmap("fit: Young's modulus", qmap_only=True)
-    vals = qd.flat[~np.isnan(qd.flat)]
-    # gray matter
-    assert np.allclose(vals[0], 57.62946472325552, atol=0, rtol=.01)
-    # white matter
-    assert np.allclose(vals[2], 46.61406865570242, atol=0, rtol=.01)
-    # background
-    assert np.allclose(vals[1], 17605.034077063443, atol=0, rtol=0.0001)
-
-
-def test_feat_rating():
-    """Reproduces rating in figures 5K-M"""
-    qm = qmap.QMap(jpkfile2)
-    # fit data
-    for idnt in qm.group:
-        idnt.apply_preprocessing(["compute_tip_position",
-                                  "correct_force_offset",
-                                  "correct_tip_offset"])
-        inparams = model.model_sneddon_spherical_approximation \
-            .get_parameter_defaults()
-        inparams["E"].value = 50
-        inparams["R"].value = 37.28e-6 / 2
-        inparams["baseline"].vary = False
-
-        # Fit with absolute full range
-        idnt.fit_model(model_key="sneddon_spher_approx",
-                       params_initial=inparams,
-                       range_x=(0, 0),
-                       range_type="absolute",
-                       x_axis="tip position",
-                       y_axis="force",
-                       segment="approach",
-                       weight_cp=2e-6)
-        idnt.rate_quality(training_set="zef18",
-                          regressor="Extra Trees")
-
-    qd = qm.get_qmap("fit: rating", qmap_only=True)
-    vals = qd.flat[~np.isnan(qd.flat)]
-    assert np.allclose(vals[0], 9.370435813605962), "gray matter"
-    assert np.allclose(vals[2], 4.942804081687071), "white matter"
-    assert np.allclose(vals[1], 2.432396277782555), "background"
-
-
-def test_feat_rating_nofit():
-    qm = qmap.QMap(jpkfile)
-    with warnings.catch_warnings(record=True) as w:
-        # No data available, because there is no fit
-        qd = qm.get_qmap("fit: rating", qmap_only=True)
-        assert len(w) == 4
-        assert w[0].category is qmap.DataMissingWarning
-    assert np.alltrue(np.isnan(qd))
-
-
-def test_get_coords():
-    qm = qmap.QMap(jpkfile)
-
-    px = qm.get_coords(which="px")
-    refpx = np.array([[0, 0], [9, 0], [9, 9], [0, 9]])
-    assert np.all(px == refpx)
-
-    um = qm.get_coords(which="um")
-    refum = np.array([[31.972656250000004, -753.5351562500001],
-                      [571.8359375000001, -753.90625],
-                      [571.8359375000001, -213.73046875000003],
-                      [31.855468750000004, -213.73046875000003]])
-    assert np.all(um == refum)
-
-
-def test_get_coords_bad():
-    qm = qmap.QMap(jpkfile)
-    try:
-        qm.get_coords(which="mm")
-    except ValueError:
-        pass
-    else:
-        assert False, "Units [mm] should not be supported."
-
-
-def test_get_qmap():
-    qm = qmap.QMap(jpkfile)
-    x, y, _ = qm.get_qmap(feature="data: height base point", qmap_only=False)
-    assert x.size == 10
-    assert y.size == 10
-
-
-def test_init_with_dataset():
-    ds = IndentationGroup(jpkfile)
-    qm = qmap.QMap(ds)
-    assert qm.shape == (10, 10)
-
-
-def test_metadata():
-    qm = qmap.QMap(jpkfile)
-    assert np.allclose(qm.extent,
-                       [1.97265625, 601.97265625,
-                        -783.53515625, -183.53515625000006])
-    assert qm.shape == (10, 10)
-
-
-if __name__ == "__main__":
-    # Run all tests
-    loc = locals()
-    for key in list(loc.keys()):
-        if key.startswith("test_") and hasattr(loc[key], "__call__"):
-            loc[key]()
+"""Test qmap feature"""
+import pathlib
+import warnings
+
+import numpy as np
+
+from nanite import model, qmap, IndentationGroup
+
+
+data_path = pathlib.Path(__file__).resolve().parent / "data"
+jpkfile = data_path / "fmt-jpk-fd_map2x2_extracted.jpk-force-map"
+jpkfile2 = data_path / "fmt-jpk-fd_map-data-reference-points.jpk-force-map"
+
+
+def test_feat_scan_order():
+    qm = qmap.QMap(jpkfile)
+    order = qm.get_qmap("data: scan order", qmap_only=True)
+    assert order[0, 0] == 0
+    assert order[0, -1] == 1
+    assert order[-1, -1] == 2
+    assert order[-1, 0] == 3
+    assert np.isnan(order[0, 1])
+
+
+def test_feat_min_height():
+    qm = qmap.QMap(jpkfile)
+    qd = qm.get_qmap("data: height base point", qmap_only=True)
+    assert np.allclose(qd[0, 0], 40.55030392499141)
+    assert np.allclose(qd[0, -1], 47.354988549298945)
+    assert np.allclose(qd[-1, -1], 96.1627883099352)
+    assert np.allclose(qd[-1, 0], 89.95170867840217)
+
+
+def test_feat_cp():
+    qm = qmap.QMap(jpkfile2)
+    # fit data
+    for idnt in qm.group:
+        idnt.apply_preprocessing(["compute_tip_position",
+                                  "correct_force_offset",
+                                  "correct_tip_offset",
+                                  ])
+        inparams = model.model_sneddon_spherical_approximation \
+            .get_parameter_defaults()
+        inparams["E"].value = 50
+        inparams["R"].value = 37.28e-6 / 2
+        inparams["baseline"].vary = False
+
+        # Fit with absolute full range
+        idnt.fit_model(model_key="sneddon_spher_approx",
+                       params_initial=inparams,
+                       range_x=(0, 0),
+                       range_type="absolute",
+                       x_axis="tip position",
+                       y_axis="force",
+                       segment="approach",
+                       weight_cp=2e-6)
+
+    qd = qm.get_qmap("fit: contact point", qmap_only=True)
+    vals = qd.flat[~np.isnan(qd.flat)]
+    # These are subject to change when contact point preprocessing
+    # changes.
+    assert np.allclose(vals[0], -1820.431327293334), "gray matter"
+    assert np.allclose(vals[2], -3581.010097829371), "white matter"
+    assert np.allclose(vals[1], -2106.9835957851064), "background"
+
+
+def test_feat_emod_nofit():
+    qm = qmap.QMap(jpkfile)
+    with warnings.catch_warnings(record=True) as w:
+        # No data available, because there is no fit
+        qd = qm.get_qmap("fit: Young's modulus", qmap_only=True)
+        assert len(w) == 4
+        assert w[0].category is qmap.DataMissingWarning
+    assert np.all(np.isnan(qd))
+
+
+def test_feat_emod_withfit():
+    qm = qmap.QMap(jpkfile2)
+    # fit data
+    for idnt in qm.group:
+        idnt.apply_preprocessing(["compute_tip_position",
+                                  "correct_force_offset",
+                                  "correct_tip_offset",
+                                  ])
+        inparams = model.model_sneddon_spherical_approximation \
+            .get_parameter_defaults()
+        inparams["E"].value = 50
+        inparams["R"].value = 37.28e-6 / 2
+        inparams["baseline"].vary = False
+
+        # Fit with absolute full range
+        idnt.fit_model(model_key="sneddon_spher_approx",
+                       params_initial=inparams,
+                       range_x=(0, 0),
+                       range_type="absolute",
+                       x_axis="tip position",
+                       y_axis="force",
+                       segment="approach",
+                       weight_cp=2e-6)
+
+    qd = qm.get_qmap("fit: Young's modulus", qmap_only=True)
+    vals = qd.flat[~np.isnan(qd.flat)]
+    # gray matter
+    assert np.allclose(vals[0], 57.62946472325552, atol=0, rtol=.01)
+    # white matter
+    assert np.allclose(vals[2], 46.61406865570242, atol=0, rtol=.01)
+    # background
+    assert np.allclose(vals[1], 17608.123636775974, atol=4, rtol=0)
+
+
+def test_feat_rating():
+    """Reproduces rating in figures 5K-M"""
+    qm = qmap.QMap(jpkfile2)
+    # fit data
+    for idnt in qm.group:
+        idnt.apply_preprocessing(["compute_tip_position",
+                                  "correct_force_offset",
+                                  "correct_tip_offset"])
+        inparams = model.model_sneddon_spherical_approximation \
+            .get_parameter_defaults()
+        inparams["E"].value = 50
+        inparams["R"].value = 37.28e-6 / 2
+        inparams["baseline"].vary = False
+
+        # Fit with absolute full range
+        idnt.fit_model(model_key="sneddon_spher_approx",
+                       params_initial=inparams,
+                       range_x=(0, 0),
+                       range_type="absolute",
+                       x_axis="tip position",
+                       y_axis="force",
+                       segment="approach",
+                       weight_cp=2e-6)
+        idnt.rate_quality(training_set="zef18",
+                          regressor="Extra Trees")
+
+    qd = qm.get_qmap("fit: rating", qmap_only=True)
+    vals = qd.flat[~np.isnan(qd.flat)]
+    assert np.allclose(vals[0], 9.370435813605962), "gray matter"
+    assert np.allclose(vals[2], 4.942804081687071), "white matter"
+    assert np.allclose(vals[1], 2.432396277782555), "background"
+
+
+def test_feat_rating_nofit():
+    qm = qmap.QMap(jpkfile)
+    with warnings.catch_warnings(record=True) as w:
+        # No data available, because there is no fit
+        qd = qm.get_qmap("fit: rating", qmap_only=True)
+        assert len(w) == 4
+        assert w[0].category is qmap.DataMissingWarning
+    assert np.all(np.isnan(qd))
+
+
+def test_get_coords():
+    qm = qmap.QMap(jpkfile)
+
+    px = qm.get_coords(which="px")
+    refpx = np.array([[0, 0], [9, 0], [9, 9], [0, 9]])
+    assert np.all(px == refpx)
+
+    um = qm.get_coords(which="um")
+    refum = np.array([[31.972656250000004, -753.5351562500001],
+                      [571.8359375000001, -753.90625],
+                      [571.8359375000001, -213.73046875000003],
+                      [31.855468750000004, -213.73046875000003]])
+    assert np.all(um == refum)
+
+
+def test_get_coords_bad():
+    qm = qmap.QMap(jpkfile)
+    try:
+        qm.get_coords(which="mm")
+    except ValueError:
+        pass
+    else:
+        assert False, "Units [mm] should not be supported."
+
+
+def test_get_qmap():
+    qm = qmap.QMap(jpkfile)
+    x, y, _ = qm.get_qmap(feature="data: height base point", qmap_only=False)
+    assert x.size == 10
+    assert y.size == 10
+
+
+def test_init_with_dataset():
+    ds = IndentationGroup(jpkfile)
+    qm = qmap.QMap(ds)
+    assert qm.shape == (10, 10)
+
+
+def test_metadata():
+    qm = qmap.QMap(jpkfile)
+    assert np.allclose(qm.extent,
+                       [1.97265625, 601.97265625,
+                        -783.53515625, -183.53515625000006])
+    assert qm.shape == (10, 10)
```

### Comparing `nanite-3.5.4/tests/test_rate_io.py` & `nanite-3.6.0/tests/test_rate_io.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,192 +1,184 @@
-"""Test input/output of user rating data"""
-import pathlib
-import shutil
-import tempfile
-
-import h5py
-import numpy as np
-import pytest
-
-from nanite import model, IndentationGroup
-from nanite.rate.io import RateManager, hdf5_rated, load_hdf5, save_hdf5
-from nanite.rate.rater import IndentationRater
-
-data_path = pathlib.Path(__file__).resolve().parent / "data"
-jpkfile = data_path / "fmt-jpk-fd_spot3-0192.jpk-force"
-
-
-def setuph5(ret_idnt=False, path=jpkfile):
-    tdir = tempfile.mkdtemp(prefix="test_nanite_rate_io_")
-    tdir = pathlib.Path(tdir)
-    h5path = tdir / "simple.h5"
-    grp = IndentationGroup(path)
-    for idnt in grp:
-        idnt.apply_preprocessing(["compute_tip_position"])
-
-        inparams = model.model_hertz_paraboloidal.get_parameter_defaults()
-        inparams["baseline"].vary = True
-        inparams["contact_point"].set(1.8e-5)
-
-        # Fit with absolute full range
-        idnt.fit_model(model_key="hertz_para",
-                       params_initial=inparams,
-                       range_x=(0, 0),
-                       range_type="absolute",
-                       x_axis="tip position",
-                       y_axis="force",
-                       segment="approach",
-                       weight_cp=False)
-
-        save_hdf5(h5path=h5path,
-                  indent=idnt,
-                  user_rate=5,
-                  user_name="hans",
-                  user_comment="this is a comment",
-                  h5mode="a")
-    else:
-        idnt = grp[0]
-
-    if ret_idnt:
-        return tdir, h5path, idnt
-    else:
-        return tdir, h5path
-
-
-def test_hdf5rated():
-    tdir, h5path, idnt = setuph5(ret_idnt=True)
-    is_rated, rating, comment = hdf5_rated(h5path, idnt)
-    assert is_rated
-    assert rating == 5
-    assert comment == "this is a comment"
-
-
-def test_rate_manager_basic():
-    tdir, h5path, idnt = setuph5(ret_idnt=True)
-    rmg = RateManager(h5path)
-    # sanity checks
-    rr = rmg.ratings[0]
-    assert rr["name"] == "hans"
-    assert rr["rating"] == 5
-    # file name preserved
-    ds = rmg.datasets[0]
-    assert jpkfile.name in ds.path.name
-    # features are the same
-    idr = IndentationRater
-    ss = rmg.samples[0]
-    assert np.allclose(ss, idr.compute_features(idnt))
-    # rates
-    assert np.ndarray.item(rmg.get_rates(which="user")) == 5
-    # This will fail when the hyper-parameters for "Extra Trees" change
-    # or when new features are added.
-    assert np.allclose(
-        np.ndarray.item(rmg.get_rates(which="Extra Trees",
-                                      training_set="zef18")),
-        3.5492840783289035)
-
-
-def test_rate_manager_crossval():
-    path = data_path / "fmt-jpk-fd_map-data-reference-points.jpk-force-map"
-    tdir, h5path = setuph5(path=path)
-    rmg = RateManager(h5path)
-    cv = rmg.get_cross_validation_score(regressor="Extra Trees",
-                                        training_set=None,
-                                        n_splits=2,
-                                        random_state=42)
-    assert np.all(cv == 0)
-
-
-def test_rate_manager_export():
-    tdir, h5path = setuph5()
-    rmg = RateManager(h5path)
-    rmg.export_training_set(tdir)
-
-    ss = rmg.samples[0]
-    feats = IndentationRater.get_feature_names()
-
-    for ff, si in zip(feats, ss):
-        fi = np.loadtxt(tdir / "train_{}.txt".format(ff))
-        # :.2e, because features are not stored with high accuracy
-        assert np.ndarray.item(fi) == float("{:.2e}".format(si))
-
-
-def test_rate_manager_import():
-    pin = data_path / "rate-export_1.7.8.h5"
-    tdir = pathlib.Path(tempfile.mkdtemp(prefix="nanite_rate_load_"))
-    h5path = tdir / pin.name
-    shutil.copy2(pin, h5path)
-
-    datalist = load_hdf5(h5path)
-    rating = datalist[0]
-    dataset = rating["data_set"]
-    assert rating["rating"] == 5
-    assert dataset.fit_properties["segment"] == "approach"
-    # trigger recomputation of fit to force resetting of "segment"
-    dataset.fit_model(range_x=[1.75e-5, 2.3e-5])
-    assert dataset.fit_properties["segment"] == 0
-
-
-def test_rate_manager_get_ts():
-    path = data_path / "fmt-jpk-fd_map-data-reference-points.jpk-force-map"
-    tdir, h5path = setuph5(path=path)
-    rmg = RateManager(h5path)
-    x2, _ = rmg.get_training_set(which_type="binary")
-    assert np.all(x2 == 1)
-    x3, _ = rmg.get_training_set(which_type="continuous",
-                                 prefilter_binary=True)
-    x4, _ = rmg.get_training_set(remove_nans=True)
-    assert np.all(np.hstack((x2, x3)) == x4)
-
-
-@pytest.mark.filterwarnings('ignore::RuntimeWarning')
-def test_rate_manager_get_ts_bad():
-    path = data_path / "fmt-jpk-fd_map_bad_2013-05-27_2.jpk-force-map"
-    tdir, h5path = setuph5(path=path)
-    rmg = RateManager(h5path)
-    x2, _ = rmg.get_training_set(which_type="binary")
-    assert np.allclose(x2.flatten(), [1, 0, 1])
-    x3, _ = rmg.get_training_set(which_type="continuous",
-                                 prefilter_binary=True)
-    assert x3.size == 0
-    x4, _ = rmg.get_training_set(remove_nans=True)
-    assert x4.size == 0
-
-
-def test_rate_manager_get_ts_single():
-    tdir, h5path = setuph5()
-    rmg = RateManager(h5path)
-    x2, _ = rmg.get_training_set(which_type="binary")
-    assert np.all(x2 == 1)
-    x3, _ = rmg.get_training_set(which_type="continuous",
-                                 prefilter_binary=True)
-    x4, _ = rmg.get_training_set(remove_nans=True)
-    assert np.all(np.hstack((x2, x3)) == x4)
-
-
-def test_write():
-    tdir, h5path, idnt = setuph5(ret_idnt=True)
-
-    with h5py.File(str(h5path), mode="r") as hi:
-        # experimental data
-        assert "4443b7" in hi["data"]
-        # a few attributes
-        attrs = hi["analysis/4443b7_0"].attrs
-        assert attrs["fit model_key"] == "hertz_para"
-        assert not attrs["fit optimal_fit_edelta"]
-        assert attrs["fit preprocessing"] == "compute_tip_position"
-        assert np.allclose(hi["analysis/4443b7_0"]["fit"], idnt["fit"],
-                           equal_nan=True)
-
-
-def test_write_read():
-    tdir, h5path = setuph5()
-
-    datalist = load_hdf5(h5path)
-    assert datalist[0]["rating"] == 5
-
-
-if __name__ == "__main__":
-    # Run all tests
-    loc = locals()
-    for key in list(loc.keys()):
-        if key.startswith("test_") and hasattr(loc[key], "__call__"):
-            loc[key]()
+"""Test input/output of user rating data"""
+import pathlib
+import shutil
+import tempfile
+
+import h5py
+import numpy as np
+import pytest
+
+from nanite import model, IndentationGroup
+from nanite.rate.io import RateManager, hdf5_rated, load_hdf5, save_hdf5
+from nanite.rate.rater import IndentationRater
+
+data_path = pathlib.Path(__file__).resolve().parent / "data"
+jpkfile = data_path / "fmt-jpk-fd_spot3-0192.jpk-force"
+
+
+def setuph5(ret_idnt=False, path=jpkfile):
+    tdir = tempfile.mkdtemp(prefix="test_nanite_rate_io_")
+    tdir = pathlib.Path(tdir)
+    h5path = tdir / "simple.h5"
+    grp = IndentationGroup(path)
+    for idnt in grp:
+        idnt.apply_preprocessing(["compute_tip_position"])
+
+        inparams = model.model_hertz_paraboloidal.get_parameter_defaults()
+        inparams["baseline"].vary = True
+        inparams["contact_point"].set(1.8e-5)
+
+        # Fit with absolute full range
+        idnt.fit_model(model_key="hertz_para",
+                       params_initial=inparams,
+                       range_x=(0, 0),
+                       range_type="absolute",
+                       x_axis="tip position",
+                       y_axis="force",
+                       segment="approach",
+                       weight_cp=False)
+
+        save_hdf5(h5path=h5path,
+                  indent=idnt,
+                  user_rate=5,
+                  user_name="hans",
+                  user_comment="this is a comment",
+                  h5mode="a")
+    else:
+        idnt = grp[0]
+
+    if ret_idnt:
+        return tdir, h5path, idnt
+    else:
+        return tdir, h5path
+
+
+def test_hdf5rated():
+    tdir, h5path, idnt = setuph5(ret_idnt=True)
+    is_rated, rating, comment = hdf5_rated(h5path, idnt)
+    assert is_rated
+    assert rating == 5
+    assert comment == "this is a comment"
+
+
+def test_rate_manager_basic():
+    tdir, h5path, idnt = setuph5(ret_idnt=True)
+    rmg = RateManager(h5path)
+    # sanity checks
+    rr = rmg.ratings[0]
+    assert rr["name"] == "hans"
+    assert rr["rating"] == 5
+    # file name preserved
+    ds = rmg.datasets[0]
+    assert jpkfile.name in ds.path.name
+    # features are the same
+    idr = IndentationRater
+    ss = rmg.samples[0]
+    assert np.allclose(ss, idr.compute_features(idnt))
+    # rates
+    assert np.ndarray.item(rmg.get_rates(which="user")) == 5
+    # This will fail when the hyper-parameters for "Extra Trees" change
+    # or when new features are added.
+    assert np.allclose(
+        np.ndarray.item(rmg.get_rates(which="Extra Trees",
+                                      training_set="zef18")),
+        3.5492840783289035)
+
+
+def test_rate_manager_crossval():
+    path = data_path / "fmt-jpk-fd_map-data-reference-points.jpk-force-map"
+    tdir, h5path = setuph5(path=path)
+    rmg = RateManager(h5path)
+    cv = rmg.get_cross_validation_score(regressor="Extra Trees",
+                                        training_set=None,
+                                        n_splits=2,
+                                        random_state=42)
+    assert np.all(cv == 0)
+
+
+def test_rate_manager_export():
+    tdir, h5path = setuph5()
+    rmg = RateManager(h5path)
+    rmg.export_training_set(tdir)
+
+    ss = rmg.samples[0]
+    feats = IndentationRater.get_feature_names()
+
+    for ff, si in zip(feats, ss):
+        fi = np.loadtxt(tdir / "train_{}.txt".format(ff))
+        # :.2e, because features are not stored with high accuracy
+        assert np.ndarray.item(fi) == float("{:.2e}".format(si))
+
+
+def test_rate_manager_import():
+    pin = data_path / "rate-export_1.7.8.h5"
+    tdir = pathlib.Path(tempfile.mkdtemp(prefix="nanite_rate_load_"))
+    h5path = tdir / pin.name
+    shutil.copy2(pin, h5path)
+
+    datalist = load_hdf5(h5path)
+    rating = datalist[0]
+    dataset = rating["data_set"]
+    assert rating["rating"] == 5
+    assert dataset.fit_properties["segment"] == "approach"
+    # trigger recomputation of fit to force resetting of "segment"
+    dataset.fit_model(range_x=[1.75e-5, 2.3e-5])
+    assert dataset.fit_properties["segment"] == 0
+
+
+def test_rate_manager_get_ts():
+    path = data_path / "fmt-jpk-fd_map-data-reference-points.jpk-force-map"
+    tdir, h5path = setuph5(path=path)
+    rmg = RateManager(h5path)
+    x2, _ = rmg.get_training_set(which_type="binary")
+    assert np.all(x2 == 1)
+    x3, _ = rmg.get_training_set(which_type="continuous",
+                                 prefilter_binary=True)
+    x4, _ = rmg.get_training_set(remove_nans=True)
+    assert np.all(np.hstack((x2, x3)) == x4)
+
+
+@pytest.mark.filterwarnings('ignore::RuntimeWarning')
+def test_rate_manager_get_ts_bad():
+    path = data_path / "fmt-jpk-fd_map_bad_2013-05-27_2.jpk-force-map"
+    tdir, h5path = setuph5(path=path)
+    rmg = RateManager(h5path)
+    x2, _ = rmg.get_training_set(which_type="binary")
+    assert np.allclose(x2.flatten(), [1, 0, 1])
+    x3, _ = rmg.get_training_set(which_type="continuous",
+                                 prefilter_binary=True)
+    assert x3.size == 0
+    x4, _ = rmg.get_training_set(remove_nans=True)
+    assert x4.size == 0
+
+
+def test_rate_manager_get_ts_single():
+    tdir, h5path = setuph5()
+    rmg = RateManager(h5path)
+    x2, _ = rmg.get_training_set(which_type="binary")
+    assert np.all(x2 == 1)
+    x3, _ = rmg.get_training_set(which_type="continuous",
+                                 prefilter_binary=True)
+    x4, _ = rmg.get_training_set(remove_nans=True)
+    assert np.all(np.hstack((x2, x3)) == x4)
+
+
+def test_write():
+    tdir, h5path, idnt = setuph5(ret_idnt=True)
+
+    with h5py.File(str(h5path), mode="r") as hi:
+        # experimental data
+        assert "4443b7" in hi["data"]
+        # a few attributes
+        attrs = hi["analysis/4443b7_0"].attrs
+        assert attrs["fit model_key"] == "hertz_para"
+        assert not attrs["fit optimal_fit_edelta"]
+        assert attrs["fit preprocessing"] == "compute_tip_position"
+        assert np.allclose(hi["analysis/4443b7_0"]["fit"], idnt["fit"],
+                           equal_nan=True)
+
+
+def test_write_read():
+    tdir, h5path = setuph5()
+
+    datalist = load_hdf5(h5path)
+    assert datalist[0]["rating"] == 5
```

### Comparing `nanite-3.5.4/tests/test_rate_training_set.py` & `nanite-3.6.0/tests/test_rate_training_set.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,49 +1,41 @@
-"""Test usage of user-defined training set"""
-import pathlib
-import tempfile
-
-import numpy as np
-
-from nanite import IndentationGroup
-from nanite.rate import IndentationRater
-
-
-data_path = pathlib.Path(__file__).parent / "data"
-jpkfile = data_path / "fmt-jpk-fd_map-data-reference-points.jpk-force-map"
-
-
-def setup_training_set(n=300):
-    tdir = tempfile.mkdtemp(prefix="test_nanite_rate_ts_")
-    tdir = pathlib.Path(tdir)
-    np.random.set_state(np.random.RandomState(47).get_state())
-    for bb in IndentationRater.get_feature_names(which_type="binary"):
-        bvals = np.random.choice([0, 1], size=n, p=[.05, .95])
-        np.savetxt(tdir / "train_{}.txt".format(bb), bvals)
-    for cc in IndentationRater.get_feature_names(which_type="continuous"):
-        cvals = np.random.random_sample(size=n)
-        np.savetxt(tdir / "train_{}.txt".format(cc), cvals)
-    rating = np.random.choice(range(11), size=n)
-    np.savetxt(tdir / "train_response.txt", rating)
-    return tdir
-
-
-def test_user_training_set():
-    tdir = setup_training_set()
-    # load a curve
-    idnt = IndentationGroup(jpkfile)[0]
-    # fit it
-    idnt.fit_model(model_key="sneddon_spher_approx",
-                   preprocessing=["compute_tip_position",
-                                  "correct_force_offset"])
-    r1 = idnt.rate_quality(regressor="Extra Trees", training_set="zef18")
-    assert r1 > 9, "sanity check"
-    r2 = idnt.rate_quality(regressor="Extra Trees", training_set=tdir)
-    assert 4 < r2 < 5, "with the given random state we end up at 4.55"
-
-
-if __name__ == "__main__":
-    # Run all tests
-    loc = locals()
-    for key in list(loc.keys()):
-        if key.startswith("test_") and hasattr(loc[key], "__call__"):
-            loc[key]()
+"""Test usage of user-defined training set"""
+import pathlib
+import tempfile
+
+import numpy as np
+
+from nanite import IndentationGroup
+from nanite.rate import IndentationRater
+
+
+data_path = pathlib.Path(__file__).parent / "data"
+jpkfile = data_path / "fmt-jpk-fd_map-data-reference-points.jpk-force-map"
+
+
+def setup_training_set(n=300):
+    tdir = tempfile.mkdtemp(prefix="test_nanite_rate_ts_")
+    tdir = pathlib.Path(tdir)
+    np.random.set_state(np.random.RandomState(47).get_state())
+    for bb in IndentationRater.get_feature_names(which_type="binary"):
+        bvals = np.random.choice([0, 1], size=n, p=[.05, .95])
+        np.savetxt(tdir / "train_{}.txt".format(bb), bvals)
+    for cc in IndentationRater.get_feature_names(which_type="continuous"):
+        cvals = np.random.random_sample(size=n)
+        np.savetxt(tdir / "train_{}.txt".format(cc), cvals)
+    rating = np.random.choice(range(11), size=n)
+    np.savetxt(tdir / "train_response.txt", rating)
+    return tdir
+
+
+def test_user_training_set():
+    tdir = setup_training_set()
+    # load a curve
+    idnt = IndentationGroup(jpkfile)[0]
+    # fit it
+    idnt.fit_model(model_key="sneddon_spher_approx",
+                   preprocessing=["compute_tip_position",
+                                  "correct_force_offset"])
+    r1 = idnt.rate_quality(regressor="Extra Trees", training_set="zef18")
+    assert r1 > 9, "sanity check"
+    r2 = idnt.rate_quality(regressor="Extra Trees", training_set=tdir)
+    assert 4 < r2 < 5, "with the given random state we end up at 4.55"
```

### Comparing `nanite-3.5.4/tests/test_smooth.py` & `nanite-3.6.0/tests/test_smooth.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,68 +1,60 @@
-"""Test smoothing functionalities"""
-import numpy as np
-import pytest
-
-from nanite import smooth
-
-
-def test_smooth_monotone():
-    x = np.array([0]*30
-                 + [1]*30
-                 + [2]*30,
-                 dtype=float)
-    sm = smooth.smooth_axis_monotone(data=x, window=5)
-    assert np.unique(sm).size == sm.size
-
-
-@pytest.mark.filterwarnings('ignore::nanite.smooth.'
-                            + 'DoubledSmoothingWindowWarning')
-def test_smooth_monotone2():
-    x = np.array([0]*30
-                 + [1]*30
-                 + [0]*10  # the algorithm will smooth over this part
-                 + [1]*30,
-                 dtype=float)
-    sm = smooth.smooth_axis_monotone(data=x, window=5)
-    assert np.unique(sm).size == sm.size
-
-
-@pytest.mark.filterwarnings('ignore::nanite.smooth.'
-                            + 'DoubledSmoothingWindowWarning')
-def test_smooth_monotone_maxiter():
-    # this is not solvable
-    x = np.array([0]*30
-                 + [1]*30
-                 + [0]*30,
-                 dtype=float)
-    try:
-        smooth.smooth_axis_monotone(data=x, window=5, max_iter=100)
-    except ValueError:
-        pass
-    else:
-        assert False
-
-
-@pytest.mark.filterwarnings('ignore::nanite.smooth.'
-                            + 'DoubledSmoothingWindowWarning')
-def test_smooth_monotone_maxiter2():
-    # this is not solvable
-    x = np.array([0]*30
-                 + [1]*30
-                 + [0]*30,
-                 dtype=float)
-    try:
-        smooth.smooth_axis_monotone(data=x, window=5,
-                                    max_iter=0  # stop in first loop
-                                    )
-    except ValueError:
-        pass
-    else:
-        assert False
-
-
-if __name__ == "__main__":
-    # Run all tests
-    loc = locals()
-    for key in list(loc.keys()):
-        if key.startswith("test_") and hasattr(loc[key], "__call__"):
-            loc[key]()
+"""Test smoothing functionalities"""
+import numpy as np
+import pytest
+
+from nanite import smooth
+
+
+def test_smooth_monotone():
+    x = np.array([0]*30
+                 + [1]*30
+                 + [2]*30,
+                 dtype=float)
+    sm = smooth.smooth_axis_monotone(data=x, window=5)
+    assert np.unique(sm).size == sm.size
+
+
+@pytest.mark.filterwarnings('ignore::nanite.smooth.'
+                            + 'DoubledSmoothingWindowWarning')
+def test_smooth_monotone2():
+    x = np.array([0]*30
+                 + [1]*30
+                 + [0]*10  # the algorithm will smooth over this part
+                 + [1]*30,
+                 dtype=float)
+    sm = smooth.smooth_axis_monotone(data=x, window=5)
+    assert np.unique(sm).size == sm.size
+
+
+@pytest.mark.filterwarnings('ignore::nanite.smooth.'
+                            + 'DoubledSmoothingWindowWarning')
+def test_smooth_monotone_maxiter():
+    # this is not solvable
+    x = np.array([0]*30
+                 + [1]*30
+                 + [0]*30,
+                 dtype=float)
+    try:
+        smooth.smooth_axis_monotone(data=x, window=5, max_iter=100)
+    except ValueError:
+        pass
+    else:
+        assert False
+
+
+@pytest.mark.filterwarnings('ignore::nanite.smooth.'
+                            + 'DoubledSmoothingWindowWarning')
+def test_smooth_monotone_maxiter2():
+    # this is not solvable
+    x = np.array([0]*30
+                 + [1]*30
+                 + [0]*30,
+                 dtype=float)
+    try:
+        smooth.smooth_axis_monotone(data=x, window=5,
+                                    max_iter=0  # stop in first loop
+                                    )
+    except ValueError:
+        pass
+    else:
+        assert False
```

