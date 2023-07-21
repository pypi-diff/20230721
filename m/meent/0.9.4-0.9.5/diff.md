# Comparing `tmp/meent-0.9.4.tar.gz` & `tmp/meent-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meent-0.9.4.tar", last modified: Wed Jul 19 12:56:19 2023, max compression
+gzip compressed data, was "meent-0.9.5.tar", last modified: Fri Jul 21 11:27:25 2023, max compression
```

## Comparing `meent-0.9.4.tar` & `meent-0.9.5.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:56:19.286350 meent-0.9.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-19 12:56:01.000000 meent-0.9.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-19 12:56:19.286350 meent-0.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-07-19 12:56:01.000000 meent-0.9.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:56:19.270350 meent-0.9.4/meent/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-19 12:56:01.000000 meent-0.9.4/meent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-07-19 12:56:01.000000 meent-0.9.4/meent/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:56:19.270350 meent-0.9.4/meent/nk_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:56:19.274350 meent-0.9.4/meent/nk_data/filmetrics/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-19 12:56:01.000000 meent-0.9.4/meent/nk_data/filmetrics/Al2O3.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-07-19 12:56:01.000000 meent-0.9.4/meent/nk_data/filmetrics/Si.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-07-19 12:56:01.000000 meent-0.9.4/meent/nk_data/filmetrics/Si3N4.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-07-19 12:56:01.000000 meent-0.9.4/meent/nk_data/filmetrics/SiO2.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:56:19.274350 meent-0.9.4/meent/nk_data/matlab/
--rw-r--r--   0 runner    (1001) docker     (123)    11222 2023-07-19 12:56:01.000000 meent-0.9.4/meent/nk_data/matlab/p_Si.mat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:56:19.274350 meent-0.9.4/meent/on_jax/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_jax/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:56:19.278350 meent-0.9.4/meent/on_jax/emsolver/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_jax/emsolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16856 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_jax/emsolver/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12769 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_jax/emsolver/convolution_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    38784 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_jax/emsolver/field_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_jax/emsolver/primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)    14059 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_jax/emsolver/rcwa.py
--rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_jax/emsolver/scattering_method.py
--rw-r--r--   0 runner    (1001) docker     (123)    10546 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_jax/emsolver/smm_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    14577 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_jax/emsolver/transfer_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_jax/mee.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:56:19.278350 meent-0.9.4/meent/on_jax/modeler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_jax/modeler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_jax/modeler/modeling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:56:19.278350 meent-0.9.4/meent/on_jax/optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_jax/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_jax/optimizer/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_jax/optimizer/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:56:19.278350 meent-0.9.4/meent/on_numpy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_numpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:56:19.278350 meent-0.9.4/meent/on_numpy/emsolver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_numpy/emsolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14816 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_numpy/emsolver/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_numpy/emsolver/convolution_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    27387 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_numpy/emsolver/field_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     9893 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_numpy/emsolver/rcwa.py
--rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_numpy/emsolver/scattering_method.py
--rw-r--r--   0 runner    (1001) docker     (123)    10530 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_numpy/emsolver/smm_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    12377 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_numpy/emsolver/transfer_method.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_numpy/mee.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:56:19.282350 meent-0.9.4/meent/on_numpy/modeler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_numpy/modeler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_numpy/modeler/modeling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:56:19.282350 meent-0.9.4/meent/on_torch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:56:19.286350 meent-0.9.4/meent/on_torch/emsolver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_torch/emsolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18452 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_torch/emsolver/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    20183 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_torch/emsolver/convolution_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    29243 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_torch/emsolver/field_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_torch/emsolver/primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)    11864 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_torch/emsolver/rcwa.py
--rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_torch/emsolver/scattering_method.py
--rw-r--r--   0 runner    (1001) docker     (123)    10516 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_torch/emsolver/smm_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    14085 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_torch/emsolver/transfer_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_torch/mee.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:56:19.286350 meent-0.9.4/meent/on_torch/modeler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_torch/modeler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15628 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_torch/modeler/modeling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:56:19.286350 meent-0.9.4/meent/on_torch/optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_torch/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_torch/optimizer/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_torch/optimizer/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:56:19.274350 meent-0.9.4/meent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-19 12:56:19.000000 meent-0.9.4/meent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-07-19 12:56:19.000000 meent-0.9.4/meent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 12:56:19.000000 meent-0.9.4/meent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-19 12:56:19.000000 meent-0.9.4/meent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-19 12:56:19.000000 meent-0.9.4/meent.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 12:56:19.286350 meent-0.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-19 12:56:01.000000 meent-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:27:25.861595 meent-0.9.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-21 11:27:16.000000 meent-0.9.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-21 11:27:25.861595 meent-0.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-07-21 11:27:16.000000 meent-0.9.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:27:25.853595 meent-0.9.5/meent/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-21 11:27:16.000000 meent-0.9.5/meent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-07-21 11:27:16.000000 meent-0.9.5/meent/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:27:25.853595 meent-0.9.5/meent/nk_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:27:25.857595 meent-0.9.5/meent/nk_data/filmetrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-21 11:27:16.000000 meent-0.9.5/meent/nk_data/filmetrics/Al2O3.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-07-21 11:27:16.000000 meent-0.9.5/meent/nk_data/filmetrics/Si.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-07-21 11:27:16.000000 meent-0.9.5/meent/nk_data/filmetrics/Si3N4.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-07-21 11:27:16.000000 meent-0.9.5/meent/nk_data/filmetrics/SiO2.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:27:25.857595 meent-0.9.5/meent/nk_data/matlab/
+-rw-r--r--   0 runner    (1001) docker     (123)    11222 2023-07-21 11:27:16.000000 meent-0.9.5/meent/nk_data/matlab/p_Si.mat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:27:25.857595 meent-0.9.5/meent/on_jax/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-21 11:27:16.000000 meent-0.9.5/meent/on_jax/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:27:25.857595 meent-0.9.5/meent/on_jax/emsolver/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-21 11:27:16.000000 meent-0.9.5/meent/on_jax/emsolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16856 2023-07-21 11:27:16.000000 meent-0.9.5/meent/on_jax/emsolver/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12769 2023-07-21 11:27:16.000000 meent-0.9.5/meent/on_jax/emsolver/convolution_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38784 2023-07-21 11:27:16.000000 meent-0.9.5/meent/on_jax/emsolver/field_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-07-21 11:27:16.000000 meent-0.9.5/meent/on_jax/emsolver/primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14059 2023-07-21 11:27:16.000000 meent-0.9.5/meent/on_jax/emsolver/rcwa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-07-21 11:27:16.000000 meent-0.9.5/meent/on_jax/emsolver/scattering_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10546 2023-07-21 11:27:16.000000 meent-0.9.5/meent/on_jax/emsolver/smm_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14577 2023-07-21 11:27:16.000000 meent-0.9.5/meent/on_jax/emsolver/transfer_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-21 11:27:16.000000 meent-0.9.5/meent/on_jax/mee.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:27:25.857595 meent-0.9.5/meent/on_jax/modeler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 11:27:16.000000 meent-0.9.5/meent/on_jax/modeler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-07-21 11:27:16.000000 meent-0.9.5/meent/on_jax/modeler/modeling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:27:25.857595 meent-0.9.5/meent/on_jax/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-21 11:27:16.000000 meent-0.9.5/meent/on_jax/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-21 11:27:16.000000 meent-0.9.5/meent/on_jax/optimizer/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-07-21 11:27:16.000000 meent-0.9.5/meent/on_jax/optimizer/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:27:25.857595 meent-0.9.5/meent/on_numpy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 11:27:16.000000 meent-0.9.5/meent/on_numpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:27:25.857595 meent-0.9.5/meent/on_numpy/emsolver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 11:27:16.000000 meent-0.9.5/meent/on_numpy/emsolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14816 2023-07-21 11:27:16.000000 meent-0.9.5/meent/on_numpy/emsolver/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-07-21 11:27:16.000000 meent-0.9.5/meent/on_numpy/emsolver/convolution_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27387 2023-07-21 11:27:16.000000 meent-0.9.5/meent/on_numpy/emsolver/field_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9893 2023-07-21 11:27:16.000000 meent-0.9.5/meent/on_numpy/emsolver/rcwa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-07-21 11:27:16.000000 meent-0.9.5/meent/on_numpy/emsolver/scattering_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10530 2023-07-21 11:27:16.000000 meent-0.9.5/meent/on_numpy/emsolver/smm_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12377 2023-07-21 11:27:16.000000 meent-0.9.5/meent/on_numpy/emsolver/transfer_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-21 11:27:16.000000 meent-0.9.5/meent/on_numpy/mee.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:27:25.857595 meent-0.9.5/meent/on_numpy/modeler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 11:27:16.000000 meent-0.9.5/meent/on_numpy/modeler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-07-21 11:27:16.000000 meent-0.9.5/meent/on_numpy/modeler/modeling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:27:25.861595 meent-0.9.5/meent/on_torch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 11:27:16.000000 meent-0.9.5/meent/on_torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:27:25.861595 meent-0.9.5/meent/on_torch/emsolver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 11:27:16.000000 meent-0.9.5/meent/on_torch/emsolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18452 2023-07-21 11:27:16.000000 meent-0.9.5/meent/on_torch/emsolver/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20183 2023-07-21 11:27:16.000000 meent-0.9.5/meent/on_torch/emsolver/convolution_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29243 2023-07-21 11:27:16.000000 meent-0.9.5/meent/on_torch/emsolver/field_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-21 11:27:16.000000 meent-0.9.5/meent/on_torch/emsolver/primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11864 2023-07-21 11:27:16.000000 meent-0.9.5/meent/on_torch/emsolver/rcwa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-07-21 11:27:16.000000 meent-0.9.5/meent/on_torch/emsolver/scattering_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10516 2023-07-21 11:27:16.000000 meent-0.9.5/meent/on_torch/emsolver/smm_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14085 2023-07-21 11:27:16.000000 meent-0.9.5/meent/on_torch/emsolver/transfer_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-21 11:27:16.000000 meent-0.9.5/meent/on_torch/mee.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:27:25.861595 meent-0.9.5/meent/on_torch/modeler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 11:27:16.000000 meent-0.9.5/meent/on_torch/modeler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16965 2023-07-21 11:27:16.000000 meent-0.9.5/meent/on_torch/modeler/modeling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:27:25.861595 meent-0.9.5/meent/on_torch/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 11:27:16.000000 meent-0.9.5/meent/on_torch/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-21 11:27:16.000000 meent-0.9.5/meent/on_torch/optimizer/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-21 11:27:16.000000 meent-0.9.5/meent/on_torch/optimizer/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:27:25.853595 meent-0.9.5/meent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-21 11:27:25.000000 meent-0.9.5/meent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-07-21 11:27:25.000000 meent-0.9.5/meent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 11:27:25.000000 meent-0.9.5/meent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-21 11:27:25.000000 meent-0.9.5/meent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-21 11:27:25.000000 meent-0.9.5/meent.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 11:27:25.861595 meent-0.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-21 11:27:16.000000 meent-0.9.5/setup.py
```

### Comparing `meent-0.9.4/LICENSE` & `meent-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `meent-0.9.4/README.md` & `meent-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `meent-0.9.4/meent/main.py` & `meent-0.9.5/meent/main.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.4/meent/nk_data/filmetrics/Al2O3.txt` & `meent-0.9.5/meent/nk_data/filmetrics/Al2O3.txt`

 * *Files identical despite different names*

### Comparing `meent-0.9.4/meent/nk_data/filmetrics/Si.txt` & `meent-0.9.5/meent/nk_data/filmetrics/Si.txt`

 * *Files identical despite different names*

### Comparing `meent-0.9.4/meent/nk_data/filmetrics/Si3N4.txt` & `meent-0.9.5/meent/nk_data/filmetrics/Si3N4.txt`

 * *Files identical despite different names*

### Comparing `meent-0.9.4/meent/nk_data/filmetrics/SiO2.txt` & `meent-0.9.5/meent/nk_data/filmetrics/SiO2.txt`

 * *Files identical despite different names*

### Comparing `meent-0.9.4/meent/nk_data/matlab/p_Si.mat` & `meent-0.9.5/meent/nk_data/matlab/p_Si.mat`

 * *Files identical despite different names*

### Comparing `meent-0.9.4/meent/on_jax/emsolver/_base.py` & `meent-0.9.5/meent/on_jax/emsolver/_base.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.4/meent/on_jax/emsolver/convolution_matrix.py` & `meent-0.9.5/meent/on_jax/emsolver/convolution_matrix.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.4/meent/on_jax/emsolver/field_distribution.py` & `meent-0.9.5/meent/on_jax/emsolver/field_distribution.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.4/meent/on_jax/emsolver/primitives.py` & `meent-0.9.5/meent/on_jax/emsolver/primitives.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.4/meent/on_jax/emsolver/rcwa.py` & `meent-0.9.5/meent/on_jax/emsolver/rcwa.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.4/meent/on_jax/emsolver/scattering_method.py` & `meent-0.9.5/meent/on_jax/emsolver/scattering_method.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.4/meent/on_jax/emsolver/smm_util.py` & `meent-0.9.5/meent/on_jax/emsolver/smm_util.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.4/meent/on_jax/emsolver/transfer_method.py` & `meent-0.9.5/meent/on_jax/emsolver/transfer_method.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.4/meent/on_jax/mee.py` & `meent-0.9.5/meent/on_jax/mee.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.4/meent/on_jax/modeler/modeling.py` & `meent-0.9.5/meent/on_jax/modeler/modeling.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.4/meent/on_jax/optimizer/loss.py` & `meent-0.9.5/meent/on_jax/optimizer/loss.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.4/meent/on_jax/optimizer/optimizer.py` & `meent-0.9.5/meent/on_jax/optimizer/optimizer.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.4/meent/on_numpy/emsolver/_base.py` & `meent-0.9.5/meent/on_numpy/emsolver/_base.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.4/meent/on_numpy/emsolver/convolution_matrix.py` & `meent-0.9.5/meent/on_numpy/emsolver/convolution_matrix.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.4/meent/on_numpy/emsolver/field_distribution.py` & `meent-0.9.5/meent/on_numpy/emsolver/field_distribution.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.4/meent/on_numpy/emsolver/rcwa.py` & `meent-0.9.5/meent/on_numpy/emsolver/rcwa.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.4/meent/on_numpy/emsolver/scattering_method.py` & `meent-0.9.5/meent/on_numpy/emsolver/scattering_method.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.4/meent/on_numpy/emsolver/smm_util.py` & `meent-0.9.5/meent/on_numpy/emsolver/smm_util.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.4/meent/on_numpy/emsolver/transfer_method.py` & `meent-0.9.5/meent/on_numpy/emsolver/transfer_method.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.4/meent/on_numpy/mee.py` & `meent-0.9.5/meent/on_numpy/mee.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.4/meent/on_numpy/modeler/modeling.py` & `meent-0.9.5/meent/on_numpy/modeler/modeling.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.4/meent/on_torch/emsolver/_base.py` & `meent-0.9.5/meent/on_torch/emsolver/_base.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.4/meent/on_torch/emsolver/convolution_matrix.py` & `meent-0.9.5/meent/on_torch/emsolver/convolution_matrix.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.4/meent/on_torch/emsolver/field_distribution.py` & `meent-0.9.5/meent/on_torch/emsolver/field_distribution.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.4/meent/on_torch/emsolver/primitives.py` & `meent-0.9.5/meent/on_torch/emsolver/primitives.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.4/meent/on_torch/emsolver/rcwa.py` & `meent-0.9.5/meent/on_torch/emsolver/rcwa.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.4/meent/on_torch/emsolver/scattering_method.py` & `meent-0.9.5/meent/on_torch/emsolver/scattering_method.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.4/meent/on_torch/emsolver/smm_util.py` & `meent-0.9.5/meent/on_torch/emsolver/smm_util.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.4/meent/on_torch/emsolver/transfer_method.py` & `meent-0.9.5/meent/on_torch/emsolver/transfer_method.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.4/meent/on_torch/mee.py` & `meent-0.9.5/meent/on_torch/mee.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.4/meent/on_torch/modeler/modeling.py` & `meent-0.9.5/meent/on_torch/modeler/modeling.py`

 * *Files 16% similar despite different names*

```diff
@@ -258,14 +258,15 @@
 
         points = rotate @ torch.vstack((points_x, points_y))
         res = [points[0], points[1], base]
         return res
 
     def vector(self, layer_info, x64=True):
 
+        # TODO: activate and apply 'x64' option thru this function and connect to meent class.
         if x64:
             datatype = torch.complex128
             perturbation = 1E-14
         else:
             datatype = torch.complex64
             perturbation = 1E-6
 
@@ -278,59 +279,81 @@
         for obj in obj_list:
             top_left, bottom_right, _ = obj
 
             # top_left[0]
             for _ in range(100):
                 index = bisect_left(row_list, top_left[0].real, key=lambda x: x.real)
                 if len(row_list) > index and top_left[0] == row_list[index]:
-                    top_left[0] = top_left[0] - (top_left[0] * perturbation)
+                    if top_left[0] == 0:
+                        top_left[0] = top_left[0] + perturbation
+                    else:
+                        # top_left[0] = top_left[0] - (top_left[0] * perturbation)  # TODO: plus or minus?
+                        top_left[0] = top_left[0] + (top_left[0] * perturbation)
                 else:
                     row_list.insert(index, top_left[0])
                     break
             else:
-                print('WARNING: Overlapping of the objects in modeling is too complicated. Backprop may not work as expected.')
+                print('WARNING: Vector modeling has unexpected case. Backprop may not work as expected.')
                 index = bisect_left(row_list, top_left[0].real, key=lambda x: x.real)
                 row_list.insert(index, top_left[0])
 
             # bottom_right[0]
             for _ in range(100):
                 index = bisect_left(row_list, bottom_right[0].real, key=lambda x: x.real)
                 if len(row_list) > index and bottom_right[0] == row_list[index]:
-                    bottom_right[0] = bottom_right[0] + (bottom_right[0] * perturbation)
+                    # if bottom_right[0] == 0:
+                    #     bottom_right[0] = bottom_right[0] + perturbation
+                    # else:
+                    #     # bottom_right[0] = bottom_right[0] + (bottom_right[0] * perturbation)
+                    #     bottom_right[0] = bottom_right[0] - (bottom_right[0] * perturbation)
+
+                    # bottom_right[0] = bottom_right[0] + (bottom_right[0] * perturbation)
+                    bottom_right[0] = bottom_right[0] - (bottom_right[0] * perturbation)
                 else:
                     row_list.insert(index, bottom_right[0])
                     break
             else:
-                print('WARNING: Overlapping of the objects in modeling is too complicated. Backprop may not work as expected.')
+                print('WARNING: Vector modeling has unexpected case. Backprop may not work as expected.')
                 index = bisect_left(row_list, bottom_right[0].real, key=lambda x: x.real)
                 row_list.insert(index, bottom_right[0])
 
             # top_left[1]
             for _ in range(100):
                 index = bisect_left(col_list, top_left[1].real, key=lambda x: x.real)
                 if len(col_list) > index and top_left[1] == col_list[index]:
-                    top_left[1] = top_left[1] - (top_left[1] * perturbation)
+                    if top_left[1] == 0:
+                        top_left[1] = top_left[1] + perturbation
+                    else:
+                        # top_left[1] = top_left[1] - (top_left[1] * perturbation)
+                        top_left[1] = top_left[1] + (top_left[1] * perturbation)
                 else:
                     col_list.insert(index, top_left[1])
                     break
             else:
-                print('WARNING: Overlapping of the objects in modeling is too complicated. Backprop may not work as expected.')
+                print('WARNING: Vector modeling has unexpected case. Backprop may not work as expected.')
                 index = bisect_left(col_list, top_left[1].real, key=lambda x: x.real)
                 col_list.insert(index, top_left[1])
 
             # bottom_right[1]
             for _ in range(100):
                 index = bisect_left(col_list, bottom_right[1].real, key=lambda x: x.real)
                 if len(col_list) > index and bottom_right[1] == col_list[index]:
-                    bottom_right[1] = bottom_right[1] + (bottom_right[1] * perturbation)
+                    # if bottom_right[1] == 0:
+                    #     bottom_right[1] = bottom_right[1] + perturbation
+                    # else:
+                    #     # bottom_right[1] = bottom_right[1] + (bottom_right[1] * perturbation)
+                    #     bottom_right[1] = bottom_right[1] - (bottom_right[1] * perturbation)
+
+                    # bottom_right[1] = bottom_right[1] + (bottom_right[1] * perturbation)
+                    bottom_right[1] = bottom_right[1] - (bottom_right[1] * perturbation)
                 else:
                     col_list.insert(index, bottom_right[1])
                     break
             else:
-                print('WARNING: Overlapping of the objects in modeling is too complicated. Backprop may not work as expected.')
+                print('WARNING: Vector modeling has unexpected case. Backprop may not work as expected.')
                 index = bisect_left(col_list, bottom_right[1].real, key=lambda x: x.real)
                 col_list.insert(index, bottom_right[1])
 
         if not row_list or row_list[-1] != self.period[1]:
             row_list.append(self.period[1])
         if not col_list or col_list[-1] != self.period[0]:
             col_list.append(self.period[0])
```

### Comparing `meent-0.9.4/meent/on_torch/optimizer/loss.py` & `meent-0.9.5/meent/on_torch/optimizer/loss.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.4/meent/on_torch/optimizer/optimizer.py` & `meent-0.9.5/meent/on_torch/optimizer/optimizer.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.4/meent.egg-info/SOURCES.txt` & `meent-0.9.5/meent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meent-0.9.4/setup.py` & `meent-0.9.5/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,15 +8,15 @@
             ],
     'pytorch': ['torch>=2.0.0',
                 'tqdm>=4.64.1',
                 ],
 }
 setup(
     name='meent',
-    version='0.9.4',
+    version='0.9.5',
     url='https://github.com/kc-ml2/meent',
     author='KC ML2',
     author_email='yongha@kc-ml2.com',
     packages=['meent'] + find_packages(include=['meent.*']),
     install_requires=[
         'numpy>=1.23.3',
         'scipy>=1.9.1',
```

