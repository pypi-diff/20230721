# Comparing `tmp/qmcpy-1.4.tar.gz` & `tmp/qmcpy-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qmcpy-1.4.tar", last modified: Fri Apr  7 16:32:47 2023, max compression
+gzip compressed data, was "qmcpy-1.4.1.tar", last modified: Fri Jul 21 16:12:29 2023, max compression
```

## Comparing `qmcpy-1.4.tar` & `qmcpy-1.4.1.tar`

### file list

```diff
@@ -1,102 +1,104 @@
-drwxr-xr-x   0 alegresor   (501) staff       (20)        0 2023-04-07 16:32:47.467144 qmcpy-1.4/
--rw-r--r--   0 alegresor   (501) staff       (20)      579 2021-10-06 16:43:10.000000 qmcpy-1.4/LICENSE
--rw-r--r--   0 alegresor   (501) staff       (20)      262 2021-10-06 21:31:12.000000 qmcpy-1.4/MANIFEST.in
--rw-r--r--   0 alegresor   (501) staff       (20)    14716 2023-04-07 16:32:47.467516 qmcpy-1.4/PKG-INFO
--rw-r--r--   0 alegresor   (501) staff       (20)    13974 2023-04-07 16:32:34.000000 qmcpy-1.4/README.md
-drwxr-xr-x   0 alegresor   (501) staff       (20)        0 2023-04-07 16:32:47.178382 qmcpy-1.4/qmcpy/
--rw-r--r--   0 alegresor   (501) staff       (20)      160 2023-04-07 16:32:34.000000 qmcpy-1.4/qmcpy/__init__.py
-drwxr-xr-x   0 alegresor   (501) staff       (20)        0 2023-04-07 16:32:47.185814 qmcpy-1.4/qmcpy/accumulate_data/
--rw-r--r--   0 alegresor   (501) staff       (20)      301 2022-01-06 04:39:51.000000 qmcpy-1.4/qmcpy/accumulate_data/__init__.py
--rw-r--r--   0 alegresor   (501) staff       (20)      914 2022-01-12 21:42:58.000000 qmcpy-1.4/qmcpy/accumulate_data/_accumulate_data.py
--rw-r--r--   0 alegresor   (501) staff       (20)    15304 2023-02-15 20:59:49.000000 qmcpy-1.4/qmcpy/accumulate_data/ld_transform_bayes_data.py
--rw-r--r--   0 alegresor   (501) staff       (20)     5964 2022-02-28 15:17:39.000000 qmcpy-1.4/qmcpy/accumulate_data/ld_transform_data.py
--rw-r--r--   0 alegresor   (501) staff       (20)     4628 2022-03-31 23:55:11.000000 qmcpy-1.4/qmcpy/accumulate_data/mean_var_data.py
--rw-r--r--   0 alegresor   (501) staff       (20)      922 2022-02-28 15:17:39.000000 qmcpy-1.4/qmcpy/accumulate_data/mean_var_data_rep.py
--rw-r--r--   0 alegresor   (501) staff       (20)     5331 2021-10-06 16:43:11.000000 qmcpy-1.4/qmcpy/accumulate_data/mlmc_data.py
--rw-r--r--   0 alegresor   (501) staff       (20)     5463 2021-10-06 16:43:11.000000 qmcpy-1.4/qmcpy/accumulate_data/mlqmc_data.py
-drwxr-xr-x   0 alegresor   (501) staff       (20)        0 2023-04-07 16:32:47.188833 qmcpy-1.4/qmcpy/discrete_distribution/
--rw-r--r--   0 alegresor   (501) staff       (20)      216 2022-01-06 04:40:10.000000 qmcpy-1.4/qmcpy/discrete_distribution/__init__.py
--rw-r--r--   0 alegresor   (501) staff       (20)     5817 2023-04-07 16:32:34.000000 qmcpy-1.4/qmcpy/discrete_distribution/_discrete_distribution.py
-drwxr-xr-x   0 alegresor   (501) staff       (20)        0 2023-04-07 16:32:47.192854 qmcpy-1.4/qmcpy/discrete_distribution/c_lib/
--rw-r--r--   0 alegresor   (501) staff       (20)       29 2020-08-26 16:15:01.000000 qmcpy-1.4/qmcpy/discrete_distribution/c_lib/__init__.py
--rw-r--r--   0 alegresor   (501) staff       (20)     3889 2021-10-06 16:43:11.000000 qmcpy-1.4/qmcpy/discrete_distribution/c_lib/digital_net_b2.c
--rw-r--r--   0 alegresor   (501) staff       (20)      356 2021-10-06 16:43:11.000000 qmcpy-1.4/qmcpy/discrete_distribution/c_lib/export_ctypes.h
--rw-r--r--   0 alegresor   (501) staff       (20)     1567 2021-10-06 16:43:11.000000 qmcpy-1.4/qmcpy/discrete_distribution/c_lib/fwht.c
--rw-r--r--   0 alegresor   (501) staff       (20)     8005 2021-10-06 16:43:11.000000 qmcpy-1.4/qmcpy/discrete_distribution/c_lib/halton_qrng.c
--rw-r--r--   0 alegresor   (501) staff       (20)      222 2023-01-09 23:04:02.000000 qmcpy-1.4/qmcpy/discrete_distribution/c_lib/load_c_lib.py
-drwxr-xr-x   0 alegresor   (501) staff       (20)        0 2023-04-07 16:32:47.195758 qmcpy-1.4/qmcpy/discrete_distribution/digital_net_b2/
--rw-r--r--   0 alegresor   (501) staff       (20)       82 2021-10-06 16:43:11.000000 qmcpy-1.4/qmcpy/discrete_distribution/digital_net_b2/__init__.py
--rw-r--r--   0 alegresor   (501) staff       (20)    14785 2023-01-09 23:04:02.000000 qmcpy-1.4/qmcpy/discrete_distribution/digital_net_b2/digital_net_b2.py
-drwxr-xr-x   0 alegresor   (501) staff       (20)        0 2023-04-07 16:32:47.263294 qmcpy-1.4/qmcpy/discrete_distribution/digital_net_b2/generating_matrices/
--rw-r--r--   0 alegresor   (501) staff       (20)   572960 2021-10-06 16:43:11.000000 qmcpy-1.4/qmcpy/discrete_distribution/digital_net_b2/generating_matrices/niederreiter_mat.1377.52.52.lsb.npy
--rw-r--r--   0 alegresor   (501) staff       (20)  5120128 2021-10-06 16:43:11.000000 qmcpy-1.4/qmcpy/discrete_distribution/digital_net_b2/generating_matrices/niederreiter_mat.20000.32.32.msb.npy
--rw-r--r--   0 alegresor   (501) staff       (20)  2713856 2021-10-06 16:43:11.000000 qmcpy-1.4/qmcpy/discrete_distribution/digital_net_b2/generating_matrices/sobol_mat.21201.32.32.lsb.npy
--rw-r--r--   0 alegresor   (501) staff       (20)  2713856 2021-10-06 16:43:11.000000 qmcpy-1.4/qmcpy/discrete_distribution/digital_net_b2/generating_matrices/sobol_mat.21201.32.32.msb.npy
--rw-r--r--   0 alegresor   (501) staff       (20)    12320 2021-10-06 16:43:11.000000 qmcpy-1.4/qmcpy/discrete_distribution/digital_net_b2/generating_matrices/sobol_mat.51.30.30.msb.npy
--rw-r--r--   0 alegresor   (501) staff       (20)  2713728 2023-01-09 23:04:02.000000 qmcpy-1.4/qmcpy/discrete_distribution/digital_net_b2/generating_matrices/sobol_mat_alpha2.10600.64.32.lsb.npy
--rw-r--r--   0 alegresor   (501) staff       (20)     3957 2023-01-09 23:04:02.000000 qmcpy-1.4/qmcpy/discrete_distribution/digital_net_b2/sobol_scipy.py
--rw-r--r--   0 alegresor   (501) staff       (20)    12993 2022-11-17 19:37:53.000000 qmcpy-1.4/qmcpy/discrete_distribution/halton.py
--rw-r--r--   0 alegresor   (501) staff       (20)     1425 2022-11-17 19:37:53.000000 qmcpy-1.4/qmcpy/discrete_distribution/iid_std_uniform.py
-drwxr-xr-x   0 alegresor   (501) staff       (20)        0 2023-04-07 16:32:47.303023 qmcpy-1.4/qmcpy/discrete_distribution/lattice/
--rw-r--r--   0 alegresor   (501) staff       (20)       29 2021-10-06 21:31:12.000000 qmcpy-1.4/qmcpy/discrete_distribution/lattice/__init__.py
-drwxr-xr-x   0 alegresor   (501) staff       (20)        0 2023-04-07 16:32:47.308538 qmcpy-1.4/qmcpy/discrete_distribution/lattice/generating_vectors/
--rw-r--r--   0 alegresor   (501) staff       (20)    28928 2021-01-15 15:28:12.000000 qmcpy-1.4/qmcpy/discrete_distribution/lattice/generating_vectors/lattice_vec.3600.20.npy
--rw-r--r--   0 alegresor   (501) staff       (20)     6128 2021-10-06 16:43:11.000000 qmcpy-1.4/qmcpy/discrete_distribution/lattice/generating_vectors/lattice_vec_lnb.750.24.npy
--rw-r--r--   0 alegresor   (501) staff       (20)    12212 2023-04-07 16:32:34.000000 qmcpy-1.4/qmcpy/discrete_distribution/lattice/lattice.py
-drwxr-xr-x   0 alegresor   (501) staff       (20)        0 2023-04-07 16:32:47.353900 qmcpy-1.4/qmcpy/integrand/
--rw-r--r--   0 alegresor   (501) staff       (20)      503 2023-04-07 16:32:34.000000 qmcpy-1.4/qmcpy/integrand/__init__.py
--rw-r--r--   0 alegresor   (501) staff       (20)    12780 2023-01-09 23:04:02.000000 qmcpy-1.4/qmcpy/integrand/_integrand.py
--rw-r--r--   0 alegresor   (501) staff       (20)     6411 2023-01-09 23:04:02.000000 qmcpy-1.4/qmcpy/integrand/asian_option.py
--rw-r--r--   0 alegresor   (501) staff       (20)     4171 2023-01-09 23:04:02.000000 qmcpy-1.4/qmcpy/integrand/bayesian_lr_coeffs.py
--rw-r--r--   0 alegresor   (501) staff       (20)     2266 2023-01-09 23:04:02.000000 qmcpy-1.4/qmcpy/integrand/box_integral.py
--rw-r--r--   0 alegresor   (501) staff       (20)     2097 2023-01-09 23:04:02.000000 qmcpy-1.4/qmcpy/integrand/custom_fun.py
--rw-r--r--   0 alegresor   (501) staff       (20)     4440 2023-01-09 23:04:02.000000 qmcpy-1.4/qmcpy/integrand/european_option.py
--rw-r--r--   0 alegresor   (501) staff       (20)     2779 2023-01-09 23:04:02.000000 qmcpy-1.4/qmcpy/integrand/genz.py
--rw-r--r--   0 alegresor   (501) staff       (20)     3831 2023-01-09 23:04:02.000000 qmcpy-1.4/qmcpy/integrand/ishigami.py
--rw-r--r--   0 alegresor   (501) staff       (20)     2494 2023-01-09 23:04:02.000000 qmcpy-1.4/qmcpy/integrand/keister.py
--rw-r--r--   0 alegresor   (501) staff       (20)     1012 2023-01-09 23:04:02.000000 qmcpy-1.4/qmcpy/integrand/linear0.py
--rw-r--r--   0 alegresor   (501) staff       (20)     9461 2023-01-09 23:04:02.000000 qmcpy-1.4/qmcpy/integrand/ml_call_options.py
--rw-r--r--   0 alegresor   (501) staff       (20)     7014 2023-01-09 23:04:02.000000 qmcpy-1.4/qmcpy/integrand/sensitivity_indices.py
--rw-r--r--   0 alegresor   (501) staff       (20)     7728 2023-04-07 16:32:34.000000 qmcpy-1.4/qmcpy/integrand/um_bridge_wrapper.py
-drwxr-xr-x   0 alegresor   (501) staff       (20)        0 2023-04-07 16:32:47.452038 qmcpy-1.4/qmcpy/stopping_criterion/
--rw-r--r--   0 alegresor   (501) staff       (20)      576 2023-01-09 23:04:02.000000 qmcpy-1.4/qmcpy/stopping_criterion/__init__.py
--rw-r--r--   0 alegresor   (501) staff       (20)     9501 2023-02-15 20:59:49.000000 qmcpy-1.4/qmcpy/stopping_criterion/_cub_bayes_ld_g.py
--rw-r--r--   0 alegresor   (501) staff       (20)     8302 2023-01-09 23:04:02.000000 qmcpy-1.4/qmcpy/stopping_criterion/_cub_qmc_ld_g.py
--rw-r--r--   0 alegresor   (501) staff       (20)     4023 2023-01-09 23:04:02.000000 qmcpy-1.4/qmcpy/stopping_criterion/_stopping_criterion.py
--rw-r--r--   0 alegresor   (501) staff       (20)     7471 2023-01-09 23:04:02.000000 qmcpy-1.4/qmcpy/stopping_criterion/cub_mc_clt.py
--rw-r--r--   0 alegresor   (501) staff       (20)    11877 2022-11-17 19:37:53.000000 qmcpy-1.4/qmcpy/stopping_criterion/cub_mc_g.py
--rw-r--r--   0 alegresor   (501) staff       (20)     8166 2022-11-17 19:37:53.000000 qmcpy-1.4/qmcpy/stopping_criterion/cub_mc_ml.py
--rw-r--r--   0 alegresor   (501) staff       (20)     9679 2022-11-17 19:37:53.000000 qmcpy-1.4/qmcpy/stopping_criterion/cub_mc_ml_cont.py
--rw-r--r--   0 alegresor   (501) staff       (20)    11145 2023-04-07 16:32:34.000000 qmcpy-1.4/qmcpy/stopping_criterion/cub_qmc_bayes_lattice_g.py
--rw-r--r--   0 alegresor   (501) staff       (20)    10628 2023-02-15 20:59:49.000000 qmcpy-1.4/qmcpy/stopping_criterion/cub_qmc_bayes_net_g.py
--rw-r--r--   0 alegresor   (501) staff       (20)    11611 2023-04-07 16:32:34.000000 qmcpy-1.4/qmcpy/stopping_criterion/cub_qmc_clt.py
--rw-r--r--   0 alegresor   (501) staff       (20)     6866 2023-04-07 16:32:34.000000 qmcpy-1.4/qmcpy/stopping_criterion/cub_qmc_lattice_g.py
--rw-r--r--   0 alegresor   (501) staff       (20)     6478 2023-04-07 16:32:34.000000 qmcpy-1.4/qmcpy/stopping_criterion/cub_qmc_ml.py
--rw-r--r--   0 alegresor   (501) staff       (20)     8619 2023-04-07 16:32:34.000000 qmcpy-1.4/qmcpy/stopping_criterion/cub_qmc_ml_cont.py
--rw-r--r--   0 alegresor   (501) staff       (20)     8723 2023-01-09 23:04:02.000000 qmcpy-1.4/qmcpy/stopping_criterion/cub_qmc_net_g.py
-drwxr-xr-x   0 alegresor   (501) staff       (20)        0 2023-04-07 16:32:47.462898 qmcpy-1.4/qmcpy/true_measure/
--rw-r--r--   0 alegresor   (501) staff       (20)      336 2022-01-06 04:40:51.000000 qmcpy-1.4/qmcpy/true_measure/__init__.py
--rw-r--r--   0 alegresor   (501) staff       (20)     7274 2022-10-07 20:05:06.000000 qmcpy-1.4/qmcpy/true_measure/_true_measure.py
--rw-r--r--   0 alegresor   (501) staff       (20)     2500 2021-10-06 16:43:11.000000 qmcpy-1.4/qmcpy/true_measure/bernoulli_cont.py
--rw-r--r--   0 alegresor   (501) staff       (20)     2762 2023-04-07 16:32:34.000000 qmcpy-1.4/qmcpy/true_measure/brownian_motion.py
--rw-r--r--   0 alegresor   (501) staff       (20)     3908 2023-01-09 23:04:02.000000 qmcpy-1.4/qmcpy/true_measure/gaussian.py
--rw-r--r--   0 alegresor   (501) staff       (20)     3536 2021-10-06 16:43:11.000000 qmcpy-1.4/qmcpy/true_measure/johnsons_su.py
--rw-r--r--   0 alegresor   (501) staff       (20)     2477 2021-10-06 16:43:11.000000 qmcpy-1.4/qmcpy/true_measure/kumaraswamy.py
--rw-r--r--   0 alegresor   (501) staff       (20)     1496 2021-10-06 16:43:11.000000 qmcpy-1.4/qmcpy/true_measure/lebesgue.py
--rw-r--r--   0 alegresor   (501) staff       (20)     3359 2023-01-09 23:04:02.000000 qmcpy-1.4/qmcpy/true_measure/scipy_wrapper.py
--rw-r--r--   0 alegresor   (501) staff       (20)     2683 2021-10-06 16:43:11.000000 qmcpy-1.4/qmcpy/true_measure/uniform.py
-drwxr-xr-x   0 alegresor   (501) staff       (20)        0 2023-04-07 16:32:47.466745 qmcpy-1.4/qmcpy/util/
--rw-r--r--   0 alegresor   (501) staff       (20)      213 2023-04-07 16:32:34.000000 qmcpy-1.4/qmcpy/util/__init__.py
--rw-r--r--   0 alegresor   (501) staff       (20)     2280 2023-04-07 16:32:34.000000 qmcpy-1.4/qmcpy/util/abstraction_functions.py
--rw-r--r--   0 alegresor   (501) staff       (20)     1780 2021-01-15 15:28:12.000000 qmcpy-1.4/qmcpy/util/exceptions_warnings.py
--rw-r--r--   0 alegresor   (501) staff       (20)     2378 2023-01-09 23:04:02.000000 qmcpy-1.4/qmcpy/util/latnetbuilder_linker.py
--rw-r--r--   0 alegresor   (501) staff       (20)      850 2020-07-30 01:08:25.000000 qmcpy-1.4/qmcpy/util/math_functions.py
--rw-r--r--   0 alegresor   (501) staff       (20)      351 2023-04-07 16:32:34.000000 qmcpy-1.4/qmcpy/util/stop_notebook.py
-drwxr-xr-x   0 alegresor   (501) staff       (20)        0 2023-04-07 16:32:47.180622 qmcpy-1.4/qmcpy.egg-info/
--rw-r--r--   0 alegresor   (501) staff       (20)    14716 2023-04-07 16:32:47.000000 qmcpy-1.4/qmcpy.egg-info/PKG-INFO
--rw-r--r--   0 alegresor   (501) staff       (20)     3603 2023-04-07 16:32:47.000000 qmcpy-1.4/qmcpy.egg-info/SOURCES.txt
--rw-r--r--   0 alegresor   (501) staff       (20)        1 2023-04-07 16:32:47.000000 qmcpy-1.4/qmcpy.egg-info/dependency_links.txt
--rw-r--r--   0 alegresor   (501) staff       (20)       27 2023-04-07 16:32:47.000000 qmcpy-1.4/qmcpy.egg-info/requires.txt
--rw-r--r--   0 alegresor   (501) staff       (20)        6 2023-04-07 16:32:47.000000 qmcpy-1.4/qmcpy.egg-info/top_level.txt
--rw-r--r--   0 alegresor   (501) staff       (20)       79 2023-04-07 16:32:47.468210 qmcpy-1.4/setup.cfg
--rw-r--r--   0 alegresor   (501) staff       (20)     2802 2023-04-07 16:32:34.000000 qmcpy-1.4/setup.py
+drwxr-xr-x   0 alegresor   (501) staff       (20)        0 2023-07-21 16:12:29.258984 qmcpy-1.4.1/
+-rw-r--r--   0 alegresor   (501) staff       (20)      579 2023-06-06 16:56:01.000000 qmcpy-1.4.1/LICENSE
+-rw-r--r--   0 alegresor   (501) staff       (20)      291 2023-07-06 20:31:33.000000 qmcpy-1.4.1/MANIFEST.in
+-rw-r--r--   0 alegresor   (501) staff       (20)    15140 2023-07-21 16:12:29.259195 qmcpy-1.4.1/PKG-INFO
+-rw-r--r--   0 alegresor   (501) staff       (20)    14396 2023-07-06 20:31:33.000000 qmcpy-1.4.1/README.md
+drwxr-xr-x   0 alegresor   (501) staff       (20)        0 2023-07-21 16:12:29.171170 qmcpy-1.4.1/qmcpy/
+-rw-r--r--   0 alegresor   (501) staff       (20)      191 2023-07-21 16:11:26.000000 qmcpy-1.4.1/qmcpy/__init__.py
+drwxr-xr-x   0 alegresor   (501) staff       (20)        0 2023-07-21 16:12:29.179561 qmcpy-1.4.1/qmcpy/accumulate_data/
+-rw-r--r--   0 alegresor   (501) staff       (20)      301 2023-07-21 15:42:45.000000 qmcpy-1.4.1/qmcpy/accumulate_data/__init__.py
+-rw-r--r--   0 alegresor   (501) staff       (20)      914 2023-06-06 16:56:02.000000 qmcpy-1.4.1/qmcpy/accumulate_data/_accumulate_data.py
+-rw-r--r--   0 alegresor   (501) staff       (20)    15304 2023-06-06 16:56:02.000000 qmcpy-1.4.1/qmcpy/accumulate_data/ld_transform_bayes_data.py
+-rw-r--r--   0 alegresor   (501) staff       (20)     5964 2023-06-06 16:56:02.000000 qmcpy-1.4.1/qmcpy/accumulate_data/ld_transform_data.py
+-rw-r--r--   0 alegresor   (501) staff       (20)     4628 2023-06-06 16:56:02.000000 qmcpy-1.4.1/qmcpy/accumulate_data/mean_var_data.py
+-rw-r--r--   0 alegresor   (501) staff       (20)      922 2023-06-06 16:56:02.000000 qmcpy-1.4.1/qmcpy/accumulate_data/mean_var_data_rep.py
+-rw-r--r--   0 alegresor   (501) staff       (20)     5331 2023-06-06 16:56:02.000000 qmcpy-1.4.1/qmcpy/accumulate_data/mlmc_data.py
+-rw-r--r--   0 alegresor   (501) staff       (20)     5463 2023-06-06 16:56:02.000000 qmcpy-1.4.1/qmcpy/accumulate_data/mlqmc_data.py
+drwxr-xr-x   0 alegresor   (501) staff       (20)        0 2023-07-21 16:12:29.183210 qmcpy-1.4.1/qmcpy/discrete_distribution/
+-rw-r--r--   0 alegresor   (501) staff       (20)      216 2023-06-06 16:56:02.000000 qmcpy-1.4.1/qmcpy/discrete_distribution/__init__.py
+-rw-r--r--   0 alegresor   (501) staff       (20)     4674 2023-07-06 20:31:33.000000 qmcpy-1.4.1/qmcpy/discrete_distribution/_discrete_distribution.py
+drwxr-xr-x   0 alegresor   (501) staff       (20)        0 2023-07-21 16:12:29.187465 qmcpy-1.4.1/qmcpy/discrete_distribution/c_lib/
+-rw-r--r--   0 alegresor   (501) staff       (20)       29 2020-08-26 16:15:01.000000 qmcpy-1.4.1/qmcpy/discrete_distribution/c_lib/__init__.py
+-rw-r--r--   0 alegresor   (501) staff       (20)     3889 2023-06-06 16:56:02.000000 qmcpy-1.4.1/qmcpy/discrete_distribution/c_lib/digital_net_b2.c
+-rw-r--r--   0 alegresor   (501) staff       (20)      356 2023-06-06 16:56:02.000000 qmcpy-1.4.1/qmcpy/discrete_distribution/c_lib/export_ctypes.h
+-rw-r--r--   0 alegresor   (501) staff       (20)     1567 2023-06-06 16:56:02.000000 qmcpy-1.4.1/qmcpy/discrete_distribution/c_lib/fwht.c
+-rw-r--r--   0 alegresor   (501) staff       (20)     8005 2023-06-06 16:56:02.000000 qmcpy-1.4.1/qmcpy/discrete_distribution/c_lib/halton_qrng.c
+-rw-r--r--   0 alegresor   (501) staff       (20)      222 2023-06-06 16:56:02.000000 qmcpy-1.4.1/qmcpy/discrete_distribution/c_lib/load_c_lib.py
+drwxr-xr-x   0 alegresor   (501) staff       (20)        0 2023-07-21 16:12:29.189031 qmcpy-1.4.1/qmcpy/discrete_distribution/digital_net_b2/
+-rw-r--r--   0 alegresor   (501) staff       (20)       82 2023-06-06 16:56:02.000000 qmcpy-1.4.1/qmcpy/discrete_distribution/digital_net_b2/__init__.py
+-rw-r--r--   0 alegresor   (501) staff       (20)    14789 2023-07-21 16:10:14.000000 qmcpy-1.4.1/qmcpy/discrete_distribution/digital_net_b2/digital_net_b2.py
+drwxr-xr-x   0 alegresor   (501) staff       (20)        0 2023-07-21 16:12:29.216779 qmcpy-1.4.1/qmcpy/discrete_distribution/digital_net_b2/generating_matrices/
+-rw-r--r--   0 alegresor   (501) staff       (20)   572960 2023-06-06 16:56:02.000000 qmcpy-1.4.1/qmcpy/discrete_distribution/digital_net_b2/generating_matrices/niederreiter_mat.1377.52.52.lsb.npy
+-rw-r--r--   0 alegresor   (501) staff       (20)  5120128 2023-06-06 16:56:02.000000 qmcpy-1.4.1/qmcpy/discrete_distribution/digital_net_b2/generating_matrices/niederreiter_mat.20000.32.32.msb.npy
+-rw-r--r--   0 alegresor   (501) staff       (20)  2713856 2023-06-06 16:56:02.000000 qmcpy-1.4.1/qmcpy/discrete_distribution/digital_net_b2/generating_matrices/sobol_mat.21201.32.32.lsb.npy
+-rw-r--r--   0 alegresor   (501) staff       (20)  2713856 2023-06-06 16:56:02.000000 qmcpy-1.4.1/qmcpy/discrete_distribution/digital_net_b2/generating_matrices/sobol_mat.21201.32.32.msb.npy
+-rw-r--r--   0 alegresor   (501) staff       (20)    12320 2023-06-06 16:56:02.000000 qmcpy-1.4.1/qmcpy/discrete_distribution/digital_net_b2/generating_matrices/sobol_mat.51.30.30.msb.npy
+-rw-r--r--   0 alegresor   (501) staff       (20)  2713728 2023-06-06 16:56:02.000000 qmcpy-1.4.1/qmcpy/discrete_distribution/digital_net_b2/generating_matrices/sobol_mat_alpha2.10600.64.32.lsb.npy
+-rw-r--r--   0 alegresor   (501) staff       (20)     3957 2023-06-06 16:56:02.000000 qmcpy-1.4.1/qmcpy/discrete_distribution/digital_net_b2/sobol_scipy.py
+-rw-r--r--   0 alegresor   (501) staff       (20)    12993 2023-06-06 16:56:02.000000 qmcpy-1.4.1/qmcpy/discrete_distribution/halton.py
+-rw-r--r--   0 alegresor   (501) staff       (20)     1425 2023-06-06 16:56:02.000000 qmcpy-1.4.1/qmcpy/discrete_distribution/iid_std_uniform.py
+drwxr-xr-x   0 alegresor   (501) staff       (20)        0 2023-07-21 16:12:29.224342 qmcpy-1.4.1/qmcpy/discrete_distribution/lattice/
+-rw-r--r--   0 alegresor   (501) staff       (20)       29 2023-06-06 16:56:02.000000 qmcpy-1.4.1/qmcpy/discrete_distribution/lattice/__init__.py
+drwxr-xr-x   0 alegresor   (501) staff       (20)        0 2023-07-21 16:12:29.225880 qmcpy-1.4.1/qmcpy/discrete_distribution/lattice/generating_vectors/
+-rw-r--r--   0 alegresor   (501) staff       (20)    28928 2021-01-15 15:28:12.000000 qmcpy-1.4.1/qmcpy/discrete_distribution/lattice/generating_vectors/lattice_vec.3600.20.npy
+-rw-r--r--   0 alegresor   (501) staff       (20)     6128 2023-06-06 16:56:02.000000 qmcpy-1.4.1/qmcpy/discrete_distribution/lattice/generating_vectors/lattice_vec_lnb.750.24.npy
+-rw-r--r--   0 alegresor   (501) staff       (20)    12213 2023-07-06 20:31:33.000000 qmcpy-1.4.1/qmcpy/discrete_distribution/lattice/lattice.py
+drwxr-xr-x   0 alegresor   (501) staff       (20)        0 2023-07-21 16:12:29.235838 qmcpy-1.4.1/qmcpy/integrand/
+-rw-r--r--   0 alegresor   (501) staff       (20)      503 2023-07-06 17:46:37.000000 qmcpy-1.4.1/qmcpy/integrand/__init__.py
+-rw-r--r--   0 alegresor   (501) staff       (20)    12780 2023-06-06 16:56:02.000000 qmcpy-1.4.1/qmcpy/integrand/_integrand.py
+-rw-r--r--   0 alegresor   (501) staff       (20)     6493 2023-07-06 20:31:33.000000 qmcpy-1.4.1/qmcpy/integrand/asian_option.py
+-rw-r--r--   0 alegresor   (501) staff       (20)     4171 2023-06-06 16:56:02.000000 qmcpy-1.4.1/qmcpy/integrand/bayesian_lr_coeffs.py
+-rw-r--r--   0 alegresor   (501) staff       (20)     2266 2023-06-06 16:56:02.000000 qmcpy-1.4.1/qmcpy/integrand/box_integral.py
+-rw-r--r--   0 alegresor   (501) staff       (20)     2097 2023-06-06 16:56:02.000000 qmcpy-1.4.1/qmcpy/integrand/custom_fun.py
+-rw-r--r--   0 alegresor   (501) staff       (20)     4440 2023-06-06 16:56:02.000000 qmcpy-1.4.1/qmcpy/integrand/european_option.py
+-rw-r--r--   0 alegresor   (501) staff       (20)     2779 2023-06-06 16:56:02.000000 qmcpy-1.4.1/qmcpy/integrand/genz.py
+-rw-r--r--   0 alegresor   (501) staff       (20)     3831 2023-06-06 16:56:02.000000 qmcpy-1.4.1/qmcpy/integrand/ishigami.py
+-rw-r--r--   0 alegresor   (501) staff       (20)     2494 2023-06-06 16:56:02.000000 qmcpy-1.4.1/qmcpy/integrand/keister.py
+-rw-r--r--   0 alegresor   (501) staff       (20)     1012 2023-06-06 16:56:02.000000 qmcpy-1.4.1/qmcpy/integrand/linear0.py
+-rw-r--r--   0 alegresor   (501) staff       (20)     9461 2023-06-06 16:56:02.000000 qmcpy-1.4.1/qmcpy/integrand/ml_call_options.py
+-rw-r--r--   0 alegresor   (501) staff       (20)     7014 2023-06-06 16:56:02.000000 qmcpy-1.4.1/qmcpy/integrand/sensitivity_indices.py
+-rw-r--r--   0 alegresor   (501) staff       (20)     7728 2023-07-06 17:46:37.000000 qmcpy-1.4.1/qmcpy/integrand/um_bridge_wrapper.py
+-rw-r--r--   0 alegresor   (501) staff       (20)     1522 2023-07-06 20:31:33.000000 qmcpy-1.4.1/qmcpy/qmcpy.mplstyle
+drwxr-xr-x   0 alegresor   (501) staff       (20)        0 2023-07-21 16:12:29.246559 qmcpy-1.4.1/qmcpy/stopping_criterion/
+-rw-r--r--   0 alegresor   (501) staff       (20)      576 2023-07-21 15:42:45.000000 qmcpy-1.4.1/qmcpy/stopping_criterion/__init__.py
+-rw-r--r--   0 alegresor   (501) staff       (20)     9501 2023-06-06 16:56:02.000000 qmcpy-1.4.1/qmcpy/stopping_criterion/_cub_bayes_ld_g.py
+-rw-r--r--   0 alegresor   (501) staff       (20)     8302 2023-06-06 16:56:02.000000 qmcpy-1.4.1/qmcpy/stopping_criterion/_cub_qmc_ld_g.py
+-rw-r--r--   0 alegresor   (501) staff       (20)     4023 2023-06-06 16:56:02.000000 qmcpy-1.4.1/qmcpy/stopping_criterion/_stopping_criterion.py
+-rw-r--r--   0 alegresor   (501) staff       (20)     7471 2023-06-06 16:56:02.000000 qmcpy-1.4.1/qmcpy/stopping_criterion/cub_mc_clt.py
+-rw-r--r--   0 alegresor   (501) staff       (20)    11877 2023-06-06 16:56:02.000000 qmcpy-1.4.1/qmcpy/stopping_criterion/cub_mc_g.py
+-rw-r--r--   0 alegresor   (501) staff       (20)     8166 2023-06-06 16:56:02.000000 qmcpy-1.4.1/qmcpy/stopping_criterion/cub_mc_ml.py
+-rw-r--r--   0 alegresor   (501) staff       (20)     9679 2023-06-06 16:56:02.000000 qmcpy-1.4.1/qmcpy/stopping_criterion/cub_mc_ml_cont.py
+-rw-r--r--   0 alegresor   (501) staff       (20)    11145 2023-07-06 18:38:09.000000 qmcpy-1.4.1/qmcpy/stopping_criterion/cub_qmc_bayes_lattice_g.py
+-rw-r--r--   0 alegresor   (501) staff       (20)    10628 2023-06-06 16:56:02.000000 qmcpy-1.4.1/qmcpy/stopping_criterion/cub_qmc_bayes_net_g.py
+-rw-r--r--   0 alegresor   (501) staff       (20)    11611 2023-07-06 18:38:09.000000 qmcpy-1.4.1/qmcpy/stopping_criterion/cub_qmc_clt.py
+-rw-r--r--   0 alegresor   (501) staff       (20)     6866 2023-07-06 18:38:09.000000 qmcpy-1.4.1/qmcpy/stopping_criterion/cub_qmc_lattice_g.py
+-rw-r--r--   0 alegresor   (501) staff       (20)     6478 2023-07-06 18:38:09.000000 qmcpy-1.4.1/qmcpy/stopping_criterion/cub_qmc_ml.py
+-rw-r--r--   0 alegresor   (501) staff       (20)     8619 2023-07-06 18:38:09.000000 qmcpy-1.4.1/qmcpy/stopping_criterion/cub_qmc_ml_cont.py
+-rw-r--r--   0 alegresor   (501) staff       (20)     8723 2023-06-06 16:56:02.000000 qmcpy-1.4.1/qmcpy/stopping_criterion/cub_qmc_net_g.py
+drwxr-xr-x   0 alegresor   (501) staff       (20)        0 2023-07-21 16:12:29.253371 qmcpy-1.4.1/qmcpy/true_measure/
+-rw-r--r--   0 alegresor   (501) staff       (20)      336 2023-06-06 16:56:02.000000 qmcpy-1.4.1/qmcpy/true_measure/__init__.py
+-rw-r--r--   0 alegresor   (501) staff       (20)     7280 2023-07-06 20:31:33.000000 qmcpy-1.4.1/qmcpy/true_measure/_true_measure.py
+-rw-r--r--   0 alegresor   (501) staff       (20)     2500 2023-06-06 16:56:02.000000 qmcpy-1.4.1/qmcpy/true_measure/bernoulli_cont.py
+-rw-r--r--   0 alegresor   (501) staff       (20)     2762 2023-07-06 18:50:17.000000 qmcpy-1.4.1/qmcpy/true_measure/brownian_motion.py
+-rw-r--r--   0 alegresor   (501) staff       (20)     3925 2023-07-06 20:31:33.000000 qmcpy-1.4.1/qmcpy/true_measure/gaussian.py
+-rw-r--r--   0 alegresor   (501) staff       (20)     3536 2023-06-06 16:56:02.000000 qmcpy-1.4.1/qmcpy/true_measure/johnsons_su.py
+-rw-r--r--   0 alegresor   (501) staff       (20)     2477 2023-06-06 16:56:02.000000 qmcpy-1.4.1/qmcpy/true_measure/kumaraswamy.py
+-rw-r--r--   0 alegresor   (501) staff       (20)     1496 2023-06-06 16:56:02.000000 qmcpy-1.4.1/qmcpy/true_measure/lebesgue.py
+-rw-r--r--   0 alegresor   (501) staff       (20)     3359 2023-06-06 16:56:02.000000 qmcpy-1.4.1/qmcpy/true_measure/scipy_wrapper.py
+-rw-r--r--   0 alegresor   (501) staff       (20)     2683 2023-06-06 16:56:02.000000 qmcpy-1.4.1/qmcpy/true_measure/uniform.py
+drwxr-xr-x   0 alegresor   (501) staff       (20)        0 2023-07-21 16:12:29.258390 qmcpy-1.4.1/qmcpy/util/
+-rw-r--r--   0 alegresor   (501) staff       (20)      252 2023-07-06 20:31:33.000000 qmcpy-1.4.1/qmcpy/util/__init__.py
+-rw-r--r--   0 alegresor   (501) staff       (20)     2280 2023-07-06 17:46:37.000000 qmcpy-1.4.1/qmcpy/util/abstraction_functions.py
+-rw-r--r--   0 alegresor   (501) staff       (20)     1780 2021-01-15 15:28:12.000000 qmcpy-1.4.1/qmcpy/util/exceptions_warnings.py
+-rw-r--r--   0 alegresor   (501) staff       (20)     2378 2023-06-06 16:56:02.000000 qmcpy-1.4.1/qmcpy/util/latnetbuilder_linker.py
+-rw-r--r--   0 alegresor   (501) staff       (20)      850 2020-07-30 01:08:25.000000 qmcpy-1.4.1/qmcpy/util/math_functions.py
+-rw-r--r--   0 alegresor   (501) staff       (20)     3443 2023-07-06 20:31:33.000000 qmcpy-1.4.1/qmcpy/util/plot_functions.py
+-rw-r--r--   0 alegresor   (501) staff       (20)      351 2023-07-06 17:46:37.000000 qmcpy-1.4.1/qmcpy/util/stop_notebook.py
+drwxr-xr-x   0 alegresor   (501) staff       (20)        0 2023-07-21 16:12:29.173851 qmcpy-1.4.1/qmcpy.egg-info/
+-rw-r--r--   0 alegresor   (501) staff       (20)    15140 2023-07-21 16:12:29.000000 qmcpy-1.4.1/qmcpy.egg-info/PKG-INFO
+-rw-r--r--   0 alegresor   (501) staff       (20)     3653 2023-07-21 16:12:29.000000 qmcpy-1.4.1/qmcpy.egg-info/SOURCES.txt
+-rw-r--r--   0 alegresor   (501) staff       (20)        1 2023-07-21 16:12:29.000000 qmcpy-1.4.1/qmcpy.egg-info/dependency_links.txt
+-rw-r--r--   0 alegresor   (501) staff       (20)       27 2023-07-21 16:12:29.000000 qmcpy-1.4.1/qmcpy.egg-info/requires.txt
+-rw-r--r--   0 alegresor   (501) staff       (20)        6 2023-07-21 16:12:29.000000 qmcpy-1.4.1/qmcpy.egg-info/top_level.txt
+-rw-r--r--   0 alegresor   (501) staff       (20)       79 2023-07-21 16:12:29.259837 qmcpy-1.4.1/setup.cfg
+-rw-r--r--   0 alegresor   (501) staff       (20)     2804 2023-07-21 16:11:46.000000 qmcpy-1.4.1/setup.py
```

### Comparing `qmcpy-1.4/LICENSE` & `qmcpy-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qmcpy-1.4/PKG-INFO` & `qmcpy-1.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qmcpy
-Version: 1.4
+Version: 1.4.1
 Summary: (Quasi) Monte Carlo Framework in Python 3
 Home-page: https://qmcsoftware.github.io/QMCSoftware/
 Download-URL: https://github.com/QMCSoftware/QMCSoftware/releases/tag/v0.4.gz
 Author: Fred Hickernell, Sou-Cheng T. Choi, Mike McCourt, Jagadeeswaran Rathinavel, Aleksei Sorokin
 Author-email: asorokin@hawk.iit.edu
 License: Apache license 2.0
 Keywords: quasi,monte,carlo,community,software,cubature,numerical,integration,discrepancy,sobol,lattice
@@ -120,14 +120,21 @@
 QMCPy: A quasi-Monte Carlo Python Library. Working. 2020.
 https://qmcsoftware.github.io/QMCSoftware/
 ~~~
 
 BibTex citation available [here](https://github.com/QMCSoftware/QMCSoftware/blob/master/cite_qmcpy.bib)
 
 ----
+## Video Tutorial
+Please refer to [this video](https://www.youtube.com/watch?v=bRcKiLA2yBQ) for a quick introduction to QMCPy.
+[![Watch the video](https://img.youtube.com/vi/bRcKiLA2yBQ/0.jpg)](https://youtu.be/bRcKiLA2yBQ)
+
+For a more detail introduction refer to [this video](https://www.youtube.com/watch?v=gL8M_7c-YUE).
+[![Watch the video](https://img.youtube.com/vi/gL8M_7c-YUE/0.jpg)](https://youtu.be/gL8M_7c-YUE)
+
 
 ## References
 
 <b>[1]</b> F. Y. Kuo and D. Nuyens. "Application of quasi-Monte Carlo methods to elliptic PDEs with random diffusion coefficients - a survey of analysis and implementation," Foundations of Computational Mathematics, 16(6):1631-1696, 2016. ([springer link](https://link.springer.com/article/10.1007/s10208-016-9329-5), [arxiv link](https://arxiv.org/abs/1606.06613))
 
 <b>[2]</b> Fred J. Hickernell, Lan Jiang, Yuewei Liu, and Art B. Owen, "Guaranteed conservative fixed width confidence intervals via Monte Carlo sampling," Monte Carlo and Quasi-Monte Carlo Methods 2012 (J. Dick, F.Y. Kuo, G. W. Peters, and I. H. Sloan, eds.), pp. 105-128, Springer-Verlag, Berlin, 2014. DOI: 10.1007/978-3-642-41095-6_5
```

### Comparing `qmcpy-1.4/README.md` & `qmcpy-1.4.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -103,14 +103,21 @@
 QMCPy: A quasi-Monte Carlo Python Library. Working. 2020.
 https://qmcsoftware.github.io/QMCSoftware/
 ~~~
 
 BibTex citation available [here](https://github.com/QMCSoftware/QMCSoftware/blob/master/cite_qmcpy.bib)
 
 ----
+## Video Tutorial
+Please refer to [this video](https://www.youtube.com/watch?v=bRcKiLA2yBQ) for a quick introduction to QMCPy.
+[![Watch the video](https://img.youtube.com/vi/bRcKiLA2yBQ/0.jpg)](https://youtu.be/bRcKiLA2yBQ)
+
+For a more detail introduction refer to [this video](https://www.youtube.com/watch?v=gL8M_7c-YUE).
+[![Watch the video](https://img.youtube.com/vi/gL8M_7c-YUE/0.jpg)](https://youtu.be/gL8M_7c-YUE)
+
 
 ## References
 
 <b>[1]</b> F. Y. Kuo and D. Nuyens. "Application of quasi-Monte Carlo methods to elliptic PDEs with random diffusion coefficients - a survey of analysis and implementation," Foundations of Computational Mathematics, 16(6):1631-1696, 2016. ([springer link](https://link.springer.com/article/10.1007/s10208-016-9329-5), [arxiv link](https://arxiv.org/abs/1606.06613))
 
 <b>[2]</b> Fred J. Hickernell, Lan Jiang, Yuewei Liu, and Art B. Owen, "Guaranteed conservative fixed width confidence intervals via Monte Carlo sampling," Monte Carlo and Quasi-Monte Carlo Methods 2012 (J. Dick, F.Y. Kuo, G. W. Peters, and I. H. Sloan, eds.), pp. 105-128, Springer-Verlag, Berlin, 2014. DOI: 10.1007/978-3-642-41095-6_5
```

### Comparing `qmcpy-1.4/qmcpy/accumulate_data/_accumulate_data.py` & `qmcpy-1.4.1/qmcpy/accumulate_data/_accumulate_data.py`

 * *Files identical despite different names*

### Comparing `qmcpy-1.4/qmcpy/accumulate_data/ld_transform_bayes_data.py` & `qmcpy-1.4.1/qmcpy/accumulate_data/ld_transform_bayes_data.py`

 * *Files identical despite different names*

### Comparing `qmcpy-1.4/qmcpy/accumulate_data/ld_transform_data.py` & `qmcpy-1.4.1/qmcpy/accumulate_data/ld_transform_data.py`

 * *Files identical despite different names*

### Comparing `qmcpy-1.4/qmcpy/accumulate_data/mean_var_data.py` & `qmcpy-1.4.1/qmcpy/accumulate_data/mean_var_data.py`

 * *Files identical despite different names*

### Comparing `qmcpy-1.4/qmcpy/accumulate_data/mean_var_data_rep.py` & `qmcpy-1.4.1/qmcpy/accumulate_data/mean_var_data_rep.py`

 * *Files identical despite different names*

### Comparing `qmcpy-1.4/qmcpy/accumulate_data/mlmc_data.py` & `qmcpy-1.4.1/qmcpy/accumulate_data/mlmc_data.py`

 * *Files identical despite different names*

### Comparing `qmcpy-1.4/qmcpy/accumulate_data/mlqmc_data.py` & `qmcpy-1.4.1/qmcpy/accumulate_data/mlqmc_data.py`

 * *Files identical despite different names*

### Comparing `qmcpy-1.4/qmcpy/discrete_distribution/_discrete_distribution.py` & `qmcpy-1.4.1/qmcpy/discrete_distribution/_discrete_distribution.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from ..util import ParameterError, MethodImplementationError, _univ_repr, DimensionError
 from numpy import *
 
-
-
 class DiscreteDistribution(object):
     """ Discrete Distribution abstract class. DO NOT INSTANTIATE. """
 
     def __init__(self, dimension, seed):
         """
         Args:
             dimension (int or ndarray): dimension of the generator.
@@ -49,41 +47,15 @@
         """
         raise MethodImplementationError(self, 'gen_samples')
 
     def pdf(self, x):
         """ ABSTRACT METHOD to evaluate pdf of distribution the samples mimic at locations of x. """
         raise MethodImplementationError(self, 'pdf')
 
-    def plot(self, n, d_horizontal=0, d_vertical = 1, axis=None, **kwargs):
-        """
-        Args:
-            n (int): n is the number of samples that will be plotted 
-            d_vertical (int): d_vertical is the index of points that will be plotted on the vertical axis. 
-            d_horizontal (int): d_horizontal is the index of points that will be plotted as the horizontial axis.
-        """
-        try:
-            import matplotlib.pyplot as plt
-        except:
-            raise ImportError("Missing matplotlib.pyplot as plt, Matplotlib must be intalled to run DiscreteDistribution.plot")
-        samples = self.gen_samples(n)
-        if axis is None:
-            fig, ax = plt.subplots(nrows=1, ncols=1, figsize=(5, 5))
-        else: 
-            ax = axis 
-            fig = plt.figure()
-        ax.scatter(samples[:, d_horizontal], samples[:, d_vertical], **kwargs)
-        ax.set_xlabel(r'$x_{%d}$'%d_horizontal)
-        ax.set_ylabel(r'$x_{%d}$'%d_vertical)
-        ax.set_xlim([0, 1])
-        ax.set_ylim([0, 1])
-        ax.set_xticks([0, 1])
-        ax.set_yticks([0, 1])
-        ax.set_aspect(1)
-        return fig, ax
-
+    
     def spawn(self, s=1, dimensions=None):
         """
         Spawn new instances of the current discrete distribution but with new seeds and dimensions.
         Developed for multi-level and multi-replication (Q)MC algorithms.
 
         Args:
             s (int): number of spawn
```

### Comparing `qmcpy-1.4/qmcpy/discrete_distribution/c_lib/digital_net_b2.c` & `qmcpy-1.4.1/qmcpy/discrete_distribution/c_lib/digital_net_b2.c`

 * *Files identical despite different names*

### Comparing `qmcpy-1.4/qmcpy/discrete_distribution/c_lib/fwht.c` & `qmcpy-1.4.1/qmcpy/discrete_distribution/c_lib/fwht.c`

 * *Files identical despite different names*

### Comparing `qmcpy-1.4/qmcpy/discrete_distribution/c_lib/halton_qrng.c` & `qmcpy-1.4.1/qmcpy/discrete_distribution/c_lib/halton_qrng.c`

 * *Files identical despite different names*

### Comparing `qmcpy-1.4/qmcpy/discrete_distribution/digital_net_b2/digital_net_b2.py` & `qmcpy-1.4.1/qmcpy/discrete_distribution/digital_net_b2/digital_net_b2.py`

 * *Files 0% similar despite different names*

```diff
@@ -210,15 +210,15 @@
         # set the linear matrix scrambling and random shift
         if self.set_lms and self._verbose: print('s (scrambling_matrix)')
         for j in range(self.d):
             dvecj = self.dvec[j]
             if self.set_lms:
                 if self._verbose: print('\n\ts[dvec[%d]]\n\t\t'%j,end='',flush=True)
                 for t in range(self.t_lms):
-                    t1 = min(t,self.t_max)
+                    t1 = minimum(t,self.t_max)
                     u = self.rng.integers(low=0, high=1<<t1, size=1, dtype=uint64)
                     u <<= (self.t_max-t1)
                     if t1<self.t_max: u += 1<<(self.t_max-t1-1)
                     for m in range(self.m_max):
                         v = u&self.z_og[dvecj,m]
                         s = self._count_set_bits(v)%2
                         if s: self.z[j,m] += uint64(1<<(self.t_lms-t-1))
```

### Comparing `qmcpy-1.4/qmcpy/discrete_distribution/digital_net_b2/generating_matrices/niederreiter_mat.1377.52.52.lsb.npy` & `qmcpy-1.4.1/qmcpy/discrete_distribution/digital_net_b2/generating_matrices/niederreiter_mat.1377.52.52.lsb.npy`

 * *Files identical despite different names*

### Comparing `qmcpy-1.4/qmcpy/discrete_distribution/digital_net_b2/generating_matrices/niederreiter_mat.20000.32.32.msb.npy` & `qmcpy-1.4.1/qmcpy/discrete_distribution/digital_net_b2/generating_matrices/niederreiter_mat.20000.32.32.msb.npy`

 * *Files identical despite different names*

### Comparing `qmcpy-1.4/qmcpy/discrete_distribution/digital_net_b2/generating_matrices/sobol_mat.21201.32.32.lsb.npy` & `qmcpy-1.4.1/qmcpy/discrete_distribution/digital_net_b2/generating_matrices/sobol_mat.21201.32.32.lsb.npy`

 * *Files identical despite different names*

### Comparing `qmcpy-1.4/qmcpy/discrete_distribution/digital_net_b2/generating_matrices/sobol_mat.21201.32.32.msb.npy` & `qmcpy-1.4.1/qmcpy/discrete_distribution/digital_net_b2/generating_matrices/sobol_mat.21201.32.32.msb.npy`

 * *Files identical despite different names*

### Comparing `qmcpy-1.4/qmcpy/discrete_distribution/digital_net_b2/generating_matrices/sobol_mat.51.30.30.msb.npy` & `qmcpy-1.4.1/qmcpy/discrete_distribution/digital_net_b2/generating_matrices/sobol_mat.51.30.30.msb.npy`

 * *Files identical despite different names*

### Comparing `qmcpy-1.4/qmcpy/discrete_distribution/digital_net_b2/generating_matrices/sobol_mat_alpha2.10600.64.32.lsb.npy` & `qmcpy-1.4.1/qmcpy/discrete_distribution/digital_net_b2/generating_matrices/sobol_mat_alpha2.10600.64.32.lsb.npy`

 * *Files identical despite different names*

### Comparing `qmcpy-1.4/qmcpy/discrete_distribution/digital_net_b2/sobol_scipy.py` & `qmcpy-1.4.1/qmcpy/discrete_distribution/digital_net_b2/sobol_scipy.py`

 * *Files identical despite different names*

### Comparing `qmcpy-1.4/qmcpy/discrete_distribution/halton.py` & `qmcpy-1.4.1/qmcpy/discrete_distribution/halton.py`

 * *Files identical despite different names*

### Comparing `qmcpy-1.4/qmcpy/discrete_distribution/iid_std_uniform.py` & `qmcpy-1.4.1/qmcpy/discrete_distribution/iid_std_uniform.py`

 * *Files identical despite different names*

### Comparing `qmcpy-1.4/qmcpy/discrete_distribution/lattice/generating_vectors/lattice_vec.3600.20.npy` & `qmcpy-1.4.1/qmcpy/discrete_distribution/lattice/generating_vectors/lattice_vec.3600.20.npy`

 * *Files identical despite different names*

### Comparing `qmcpy-1.4/qmcpy/discrete_distribution/lattice/generating_vectors/lattice_vec_lnb.750.24.npy` & `qmcpy-1.4.1/qmcpy/discrete_distribution/lattice/generating_vectors/lattice_vec_lnb.750.24.npy`

 * *Files identical despite different names*

### Comparing `qmcpy-1.4/qmcpy/discrete_distribution/lattice/lattice.py` & `qmcpy-1.4.1/qmcpy/discrete_distribution/lattice/lattice.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 
         [5] L'Ecuyer, Pierre & Munger, David. (2015).
         LatticeBuilder: A General Software Tool for Constructing Rank-1 Lattice Rules.
         ACM Transactions on Mathematical Software. 42. 10.1145/2754929.
     """
 
     def __init__(self, dimension=1, randomize=True, order='natural', seed=None,
-        generating_vector='lattice_vec.3600.20.npy', d_max=None, m_max=None):
+        generating_vector= 'lattice_vec.3600.20.npy', d_max=None, m_max=None):
         """
         Args:
             dimension (int or ndarray): dimension of the generator.
                 If an int is passed in, use sequence dimensions [0,...,dimensions-1].
                 If a ndarray is passed in, use these dimension indices in the sequence.
             randomize (bool): If True, apply shift to generated samples.
                 Note: Non-randomized lattice sequence includes the origin.
```

### Comparing `qmcpy-1.4/qmcpy/integrand/_integrand.py` & `qmcpy-1.4.1/qmcpy/integrand/_integrand.py`

 * *Files identical despite different names*

### Comparing `qmcpy-1.4/qmcpy/integrand/asian_option.py` & `qmcpy-1.4.1/qmcpy/integrand/asian_option.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     ...     level_est = ac2_single_level.f(x).mean()
     ...     yml += level_est
     >>> yml
     1.779...
     """
                           
     def __init__(self, sampler, volatility=0.5, start_price=30., strike_price=35.,\
-        interest_rate=0., t_final=1, call_put='call', mean_type='arithmetic', multilevel_dims=None, _dim_frac=0):
+        interest_rate=0., t_final=1, call_put='call', mean_type='arithmetic', multilevel_dims=None, decomp_type='PCA', _dim_frac=0):
         """
         Args:
             sampler (DiscreteDistribution/TrueMeasure): A 
                 discrete distribution from which to transform samples or a
                 true measure by which to compose a transform
             volatility (float): sigma, the volatility of the asset
             start_price (float): S(0), the asset value at t=0
@@ -51,20 +51,21 @@
             mean_type (string): 'arithmetic' or 'geometric' mean
             multilevel_dims (list of ints): list of dimensions at each level. 
                 Leave as None for single-level problems
             _dim_frac (float): for internal use only, users should not set this parameter. 
         """
         self.parameters = ['volatility', 'call_put', 'start_price', 'strike_price', 'interest_rate','mean_type']
         self.sampler = sampler
-        self.true_measure = BrownianMotion(self.sampler,t_final)
+        self.true_measure = BrownianMotion(self.sampler,t_final,decomp_type=decomp_type)
         self.volatility = float(volatility)
         self.start_price = float(start_price)
         self.strike_price = float(strike_price)
         self.interest_rate = float(interest_rate)
         self.t_final = t_final
+        self.decomp_type = decomp_type
         self.call_put = call_put.lower()
         if self.call_put not in ['call','put']:
             raise ParameterError("call_put must be either 'call' or 'put'")
         self.mean_type = mean_type.lower()
         if self.mean_type not in ['arithmetic','geometric']:
             raise ParameterError("mean_type must either 'arithmetic' or 'geometric'")
         # handle single vs multilevel
```

### Comparing `qmcpy-1.4/qmcpy/integrand/bayesian_lr_coeffs.py` & `qmcpy-1.4.1/qmcpy/integrand/bayesian_lr_coeffs.py`

 * *Files identical despite different names*

### Comparing `qmcpy-1.4/qmcpy/integrand/box_integral.py` & `qmcpy-1.4.1/qmcpy/integrand/box_integral.py`

 * *Files identical despite different names*

### Comparing `qmcpy-1.4/qmcpy/integrand/custom_fun.py` & `qmcpy-1.4.1/qmcpy/integrand/custom_fun.py`

 * *Files identical despite different names*

### Comparing `qmcpy-1.4/qmcpy/integrand/european_option.py` & `qmcpy-1.4.1/qmcpy/integrand/european_option.py`

 * *Files identical despite different names*

### Comparing `qmcpy-1.4/qmcpy/integrand/genz.py` & `qmcpy-1.4.1/qmcpy/integrand/genz.py`

 * *Files identical despite different names*

### Comparing `qmcpy-1.4/qmcpy/integrand/ishigami.py` & `qmcpy-1.4.1/qmcpy/integrand/ishigami.py`

 * *Files identical despite different names*

### Comparing `qmcpy-1.4/qmcpy/integrand/keister.py` & `qmcpy-1.4.1/qmcpy/integrand/keister.py`

 * *Files identical despite different names*

### Comparing `qmcpy-1.4/qmcpy/integrand/linear0.py` & `qmcpy-1.4.1/qmcpy/integrand/linear0.py`

 * *Files identical despite different names*

### Comparing `qmcpy-1.4/qmcpy/integrand/ml_call_options.py` & `qmcpy-1.4.1/qmcpy/integrand/ml_call_options.py`

 * *Files identical despite different names*

### Comparing `qmcpy-1.4/qmcpy/integrand/sensitivity_indices.py` & `qmcpy-1.4.1/qmcpy/integrand/sensitivity_indices.py`

 * *Files identical despite different names*

### Comparing `qmcpy-1.4/qmcpy/integrand/um_bridge_wrapper.py` & `qmcpy-1.4.1/qmcpy/integrand/um_bridge_wrapper.py`

 * *Files identical despite different names*

### Comparing `qmcpy-1.4/qmcpy/stopping_criterion/__init__.py` & `qmcpy-1.4.1/qmcpy/stopping_criterion/__init__.py`

 * *Files identical despite different names*

### Comparing `qmcpy-1.4/qmcpy/stopping_criterion/_cub_bayes_ld_g.py` & `qmcpy-1.4.1/qmcpy/stopping_criterion/_cub_bayes_ld_g.py`

 * *Files identical despite different names*

### Comparing `qmcpy-1.4/qmcpy/stopping_criterion/_cub_qmc_ld_g.py` & `qmcpy-1.4.1/qmcpy/stopping_criterion/_cub_qmc_ld_g.py`

 * *Files identical despite different names*

### Comparing `qmcpy-1.4/qmcpy/stopping_criterion/_stopping_criterion.py` & `qmcpy-1.4.1/qmcpy/stopping_criterion/_stopping_criterion.py`

 * *Files identical despite different names*

### Comparing `qmcpy-1.4/qmcpy/stopping_criterion/cub_mc_clt.py` & `qmcpy-1.4.1/qmcpy/stopping_criterion/cub_mc_clt.py`

 * *Files identical despite different names*

### Comparing `qmcpy-1.4/qmcpy/stopping_criterion/cub_mc_g.py` & `qmcpy-1.4.1/qmcpy/stopping_criterion/cub_mc_g.py`

 * *Files identical despite different names*

### Comparing `qmcpy-1.4/qmcpy/stopping_criterion/cub_mc_ml.py` & `qmcpy-1.4.1/qmcpy/stopping_criterion/cub_mc_ml.py`

 * *Files identical despite different names*

### Comparing `qmcpy-1.4/qmcpy/stopping_criterion/cub_mc_ml_cont.py` & `qmcpy-1.4.1/qmcpy/stopping_criterion/cub_mc_ml_cont.py`

 * *Files identical despite different names*

### Comparing `qmcpy-1.4/qmcpy/stopping_criterion/cub_qmc_bayes_lattice_g.py` & `qmcpy-1.4.1/qmcpy/stopping_criterion/cub_qmc_bayes_lattice_g.py`

 * *Files identical despite different names*

### Comparing `qmcpy-1.4/qmcpy/stopping_criterion/cub_qmc_bayes_net_g.py` & `qmcpy-1.4.1/qmcpy/stopping_criterion/cub_qmc_bayes_net_g.py`

 * *Files identical despite different names*

### Comparing `qmcpy-1.4/qmcpy/stopping_criterion/cub_qmc_clt.py` & `qmcpy-1.4.1/qmcpy/stopping_criterion/cub_qmc_clt.py`

 * *Files identical despite different names*

### Comparing `qmcpy-1.4/qmcpy/stopping_criterion/cub_qmc_lattice_g.py` & `qmcpy-1.4.1/qmcpy/stopping_criterion/cub_qmc_lattice_g.py`

 * *Files identical despite different names*

### Comparing `qmcpy-1.4/qmcpy/stopping_criterion/cub_qmc_ml.py` & `qmcpy-1.4.1/qmcpy/stopping_criterion/cub_qmc_ml.py`

 * *Files identical despite different names*

### Comparing `qmcpy-1.4/qmcpy/stopping_criterion/cub_qmc_ml_cont.py` & `qmcpy-1.4.1/qmcpy/stopping_criterion/cub_qmc_ml_cont.py`

 * *Files identical despite different names*

### Comparing `qmcpy-1.4/qmcpy/stopping_criterion/cub_qmc_net_g.py` & `qmcpy-1.4.1/qmcpy/stopping_criterion/cub_qmc_net_g.py`

 * *Files identical despite different names*

### Comparing `qmcpy-1.4/qmcpy/true_measure/_true_measure.py` & `qmcpy-1.4.1/qmcpy/true_measure/_true_measure.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,7 +164,9 @@
         Return: 
             TrueMeasure: spawn with dimension and sampler
         """
         raise MethodImplementationError(self, '_spawn')  
         
     def __repr__(self):
         return _univ_repr(self, "TrueMeasure", self.parameters)
+    
+
```

### Comparing `qmcpy-1.4/qmcpy/true_measure/bernoulli_cont.py` & `qmcpy-1.4.1/qmcpy/true_measure/bernoulli_cont.py`

 * *Files identical despite different names*

### Comparing `qmcpy-1.4/qmcpy/true_measure/brownian_motion.py` & `qmcpy-1.4.1/qmcpy/true_measure/brownian_motion.py`

 * *Files identical despite different names*

### Comparing `qmcpy-1.4/qmcpy/true_measure/gaussian.py` & `qmcpy-1.4.1/qmcpy/true_measure/gaussian.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
                     mean must have length d and
                     covariance must be of shape d x d''')
         if self.decomp_type == 'PCA':
             evals,evecs = eigh(self.sigma) # get eigenvectors and eigenvalues for
             order = argsort(-evals)
             self.a = dot(evecs[:,order],diag(sqrt(evals[order])))
         elif self.decomp_type == 'CHOLESKY':
-            self.a = cholesky(self.sigma).T
+            self.a = cholesky(self.sigma) #Fred changed this
         else:
             raise ParameterError("decomp_type should be 'PCA' or 'Cholesky'") 
         self.mvn_scipy = multivariate_normal(mean=self.mu,cov=self.sigma)
 
     def _transform(self, x):
         return self.mu + norm.ppf(x)@self.a.T
```

### Comparing `qmcpy-1.4/qmcpy/true_measure/johnsons_su.py` & `qmcpy-1.4.1/qmcpy/true_measure/johnsons_su.py`

 * *Files identical despite different names*

### Comparing `qmcpy-1.4/qmcpy/true_measure/kumaraswamy.py` & `qmcpy-1.4.1/qmcpy/true_measure/kumaraswamy.py`

 * *Files identical despite different names*

### Comparing `qmcpy-1.4/qmcpy/true_measure/lebesgue.py` & `qmcpy-1.4.1/qmcpy/true_measure/lebesgue.py`

 * *Files identical despite different names*

### Comparing `qmcpy-1.4/qmcpy/true_measure/scipy_wrapper.py` & `qmcpy-1.4.1/qmcpy/true_measure/scipy_wrapper.py`

 * *Files identical despite different names*

### Comparing `qmcpy-1.4/qmcpy/true_measure/uniform.py` & `qmcpy-1.4.1/qmcpy/true_measure/uniform.py`

 * *Files identical despite different names*

### Comparing `qmcpy-1.4/qmcpy/util/abstraction_functions.py` & `qmcpy-1.4.1/qmcpy/util/abstraction_functions.py`

 * *Files identical despite different names*

### Comparing `qmcpy-1.4/qmcpy/util/exceptions_warnings.py` & `qmcpy-1.4.1/qmcpy/util/exceptions_warnings.py`

 * *Files identical despite different names*

### Comparing `qmcpy-1.4/qmcpy/util/latnetbuilder_linker.py` & `qmcpy-1.4.1/qmcpy/util/latnetbuilder_linker.py`

 * *Files identical despite different names*

### Comparing `qmcpy-1.4/qmcpy/util/math_functions.py` & `qmcpy-1.4.1/qmcpy/util/math_functions.py`

 * *Files identical despite different names*

### Comparing `qmcpy-1.4/qmcpy.egg-info/PKG-INFO` & `qmcpy-1.4.1/qmcpy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qmcpy
-Version: 1.4
+Version: 1.4.1
 Summary: (Quasi) Monte Carlo Framework in Python 3
 Home-page: https://qmcsoftware.github.io/QMCSoftware/
 Download-URL: https://github.com/QMCSoftware/QMCSoftware/releases/tag/v0.4.gz
 Author: Fred Hickernell, Sou-Cheng T. Choi, Mike McCourt, Jagadeeswaran Rathinavel, Aleksei Sorokin
 Author-email: asorokin@hawk.iit.edu
 License: Apache license 2.0
 Keywords: quasi,monte,carlo,community,software,cubature,numerical,integration,discrepancy,sobol,lattice
@@ -120,14 +120,21 @@
 QMCPy: A quasi-Monte Carlo Python Library. Working. 2020.
 https://qmcsoftware.github.io/QMCSoftware/
 ~~~
 
 BibTex citation available [here](https://github.com/QMCSoftware/QMCSoftware/blob/master/cite_qmcpy.bib)
 
 ----
+## Video Tutorial
+Please refer to [this video](https://www.youtube.com/watch?v=bRcKiLA2yBQ) for a quick introduction to QMCPy.
+[![Watch the video](https://img.youtube.com/vi/bRcKiLA2yBQ/0.jpg)](https://youtu.be/bRcKiLA2yBQ)
+
+For a more detail introduction refer to [this video](https://www.youtube.com/watch?v=gL8M_7c-YUE).
+[![Watch the video](https://img.youtube.com/vi/gL8M_7c-YUE/0.jpg)](https://youtu.be/gL8M_7c-YUE)
+
 
 ## References
 
 <b>[1]</b> F. Y. Kuo and D. Nuyens. "Application of quasi-Monte Carlo methods to elliptic PDEs with random diffusion coefficients - a survey of analysis and implementation," Foundations of Computational Mathematics, 16(6):1631-1696, 2016. ([springer link](https://link.springer.com/article/10.1007/s10208-016-9329-5), [arxiv link](https://arxiv.org/abs/1606.06613))
 
 <b>[2]</b> Fred J. Hickernell, Lan Jiang, Yuewei Liu, and Art B. Owen, "Guaranteed conservative fixed width confidence intervals via Monte Carlo sampling," Monte Carlo and Quasi-Monte Carlo Methods 2012 (J. Dick, F.Y. Kuo, G. W. Peters, and I. H. Sloan, eds.), pp. 105-128, Springer-Verlag, Berlin, 2014. DOI: 10.1007/978-3-642-41095-6_5
```

### Comparing `qmcpy-1.4/qmcpy.egg-info/SOURCES.txt` & `qmcpy-1.4.1/qmcpy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 qmcpy/__init__.py
+qmcpy/qmcpy.mplstyle
 qmcpy.egg-info/PKG-INFO
 qmcpy.egg-info/SOURCES.txt
 qmcpy.egg-info/dependency_links.txt
 qmcpy.egg-info/requires.txt
 qmcpy.egg-info/top_level.txt
 qmcpy/accumulate_data/__init__.py
 qmcpy/accumulate_data/_accumulate_data.py
@@ -80,8 +81,9 @@
 qmcpy/true_measure/scipy_wrapper.py
 qmcpy/true_measure/uniform.py
 qmcpy/util/__init__.py
 qmcpy/util/abstraction_functions.py
 qmcpy/util/exceptions_warnings.py
 qmcpy/util/latnetbuilder_linker.py
 qmcpy/util/math_functions.py
+qmcpy/util/plot_functions.py
 qmcpy/util/stop_notebook.py
```

### Comparing `qmcpy-1.4/setup.py` & `qmcpy-1.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     'qmcpy.util',
     'qmcpy.discrete_distribution.lattice',
     'qmcpy.discrete_distribution.c_lib',
     'qmcpy.discrete_distribution.digital_net_b2']
 
 setuptools.setup(
     name="qmcpy",
-    version="1.4",
+    version="1.4.1",
     author="Fred Hickernell, Sou-Cheng T. Choi, Mike McCourt, Jagadeeswaran Rathinavel, Aleksei Sorokin",
     author_email="asorokin@hawk.iit.edu",
     license='Apache license 2.0',
     description="(Quasi) Monte Carlo Framework in Python 3",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://qmcsoftware.github.io/QMCSoftware/",
```

