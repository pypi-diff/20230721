# Comparing `tmp/fdasrsf-2.4.1.tar.gz` & `tmp/fdasrsf-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fdasrsf-2.4.1.tar", last modified: Wed May 24 12:57:39 2023, max compression
+gzip compressed data, was "fdasrsf-2.4.2.tar", last modified: Fri Jul 21 17:51:22 2023, max compression
```

## Comparing `fdasrsf-2.4.1.tar` & `fdasrsf-2.4.2.tar`

### file list

```diff
@@ -1,681 +1,681 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-24 12:57:39.950606 fdasrsf-2.4.1/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1522 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/LICENSE.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      111 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     7522 2023-05-24 12:57:39.950606 fdasrsf-2.4.1/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     6597 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-24 12:57:39.870598 fdasrsf-2.4.1/bin/
--rw-rw-r--   0 travis    (2000) travis    (2000)  2156461 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/bin/MPEG7.npz
--rw-rw-r--   0 travis    (2000) travis    (2000)      174 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/bin/ex_srsf_align.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18146 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/bin/simu_data.npz
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-24 12:57:39.866598 fdasrsf-2.4.1/doc/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-24 12:57:39.866598 fdasrsf-2.4.1/doc/build/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-24 12:57:39.870598 fdasrsf-2.4.1/doc/build/man/
--rw-rw-r--   0 travis    (2000) travis    (2000)    98266 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/doc/build/man/fdasrsf.1
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-24 12:57:39.870598 fdasrsf-2.4.1/fdasrsf/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2559 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/fdasrsf/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8417 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/fdasrsf/bayesian_functions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18148 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/fdasrsf/boxplots.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    28679 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/fdasrsf/curve_functions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5532 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/fdasrsf/curve_pcr_regression.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    34875 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/fdasrsf/curve_regression.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14960 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/fdasrsf/curve_stats.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7146 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/fdasrsf/elastic_glm_regression.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17557 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/fdasrsf/fPCA.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1592 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/fdasrsf/fPLS.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16748 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/fdasrsf/geodesic.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2097 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/fdasrsf/geometry.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2907 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/fdasrsf/image.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6763 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/fdasrsf/image_functions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7320 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/fdasrsf/kmeans.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    26063 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/fdasrsf/pcr_regression.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6921 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/fdasrsf/plot_style.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19590 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/fdasrsf/rbfgs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    30908 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/fdasrsf/regression.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    66648 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/fdasrsf/time_warping.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5229 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/fdasrsf/tolerance.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8929 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/fdasrsf/umap_metric.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    29552 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/fdasrsf/utility_functions.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-24 12:57:39.870598 fdasrsf-2.4.1/fdasrsf.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     7522 2023-05-24 12:57:39.000000 fdasrsf-2.4.1/fdasrsf.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    23358 2023-05-24 12:57:39.000000 fdasrsf-2.4.1/fdasrsf.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-05-24 12:57:39.000000 fdasrsf-2.4.1/fdasrsf.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       84 2023-05-24 12:57:39.000000 fdasrsf-2.4.1/fdasrsf.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      114 2023-05-24 12:57:39.000000 fdasrsf-2.4.1/fdasrsf.egg-info/top_level.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-24 12:57:39.874598 fdasrsf-2.4.1/notebooks/
--rw-rw-r--   0 travis    (2000) travis    (2000)   515522 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/notebooks/example_curve.ipynb
--rw-rw-r--   0 travis    (2000) travis    (2000)  2208768 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/notebooks/example_warping.ipynb
--rw-rw-r--   0 travis    (2000) travis    (2000)     1249 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/pyproject.toml
--rw-rw-r--   0 travis    (2000) travis    (2000)      209 2023-05-24 12:57:39.950606 fdasrsf-2.4.1/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     3848 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-24 12:57:39.882599 fdasrsf-2.4.1/src/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6436 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/DP.c
--rw-rw-r--   0 travis    (2000) travis    (2000)       81 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/DP.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     1322 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/DynamicProgrammingQ2.c
--rw-rw-r--   0 travis    (2000) travis    (2000)      209 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/DynamicProgrammingQ2.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    17484 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/ImageRegister.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    20502 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/UnitSquareImage.cpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1607 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/UnitSquareImage.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-24 12:57:39.882599 fdasrsf-2.4.1/src/__pycache__/
--rw-rw-r--   0 travis    (2000) travis    (2000)      519 2023-05-24 12:57:39.000000 fdasrsf-2.4.1/src/__pycache__/dp_build.cpython-39.pyc
--rw-rw-r--   0 travis    (2000) travis    (2000)    29600 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-24 12:57:39.950606 fdasrsf-2.4.1/src/armadillo_bits/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2586 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/BaseCube_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     6151 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/BaseCube_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     5960 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/Base_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    17954 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/Base_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    10452 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/Col_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    35001 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/Col_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1633 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/CubeToMatOp_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1294 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/CubeToMatOp_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    26562 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/Cube_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)   122156 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/Cube_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2320 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/GenCube_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     5327 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/GenCube_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1723 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/GenSpecialiser.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2428 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/Gen_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     7185 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/Gen_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1437 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/GlueCube_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1225 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/GlueCube_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2186 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/Glue_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1359 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/Glue_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     7793 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/MapMat_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    34555 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/MapMat_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    43618 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/Mat_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)   195024 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/Mat_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2517 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/OpCube_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2841 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/OpCube_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2617 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/Op_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2133 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/Op_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    89635 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/Proxy.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    22986 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/ProxyCube.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    10441 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/Row_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    34942 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/Row_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1541 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/SizeCube_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3299 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/SizeCube_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1479 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/SizeMat_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2704 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/SizeMat_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     4328 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/SpBase_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    13609 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/SpBase_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2739 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/SpCol_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     8241 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/SpCol_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1697 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/SpGlue_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1594 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/SpGlue_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    34828 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/SpMat_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    25327 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/SpMat_iterators_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)   144757 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/SpMat_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1914 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/SpOp_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1674 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/SpOp_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    24709 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/SpProxy.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2736 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/SpRow_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     8959 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/SpRow_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    16131 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/SpSubview_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    32307 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/SpSubview_iterators_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    33981 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/SpSubview_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2278 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/SpToDOp_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1266 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/SpToDOp_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2651 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/SpValProxy_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     6557 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/SpValProxy_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2125 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/access.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    13212 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/arma_cmath.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     4176 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/arma_config.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    12926 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/arma_forward.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2998 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/arma_ostream_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    18819 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/arma_ostream_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2768 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/arma_rel_comparators.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    11543 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/arma_rng.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     4867 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/arma_rng_cxx11.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3856 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/arma_rng_cxx98.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1600 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/arma_static_check.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    11121 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/arma_str.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1476 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/arma_version.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     5601 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/arrayops_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    18194 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/arrayops_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    18669 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/auxlib_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)   178527 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/auxlib_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     9571 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/band_helper.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1194 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/compiler_extra.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    18078 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/compiler_setup.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)      815 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/compiler_setup_post.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1295 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/cond_rel_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2002 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/cond_rel_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    10927 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/config.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    11020 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/config.hpp.cmake
--rw-rw-r--   0 travis    (2000) travis    (2000)    10845 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/constants.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     6993 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/constants_old.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    31865 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/debug.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    10732 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/def_arpack.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     9041 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/def_atlas.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    10257 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/def_blas.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     6638 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/def_hdf5.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)   106546 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/def_lapack.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     4068 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/def_superlu.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    15762 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/diagmat_proxy.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3707 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/diagview_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    21581 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/diagview_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    12922 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/diskio_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)   109914 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/diskio_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1292 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/distr_param.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2071 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/eGlueCube_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     4160 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/eGlueCube_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2287 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/eGlue_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3786 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/eGlue_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2902 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/eOpCube_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3858 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/eOpCube_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2524 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/eOp_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3034 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/eOp_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3020 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/eglue_core_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    47137 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/eglue_core_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    20246 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/eop_aux.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     7192 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/eop_core_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    31181 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/eop_core_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    11016 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fft_engine.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    15975 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/field_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    61755 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/field_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    20671 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_accu.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1869 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_all.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1869 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_any.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    14171 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_approx_equal.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    11396 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_as_scalar.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3717 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_chi2rnd.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2005 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_chol.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2761 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_clamp.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1363 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_cond.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2162 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_conv.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    17558 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_conv_to.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1527 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_cor.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1525 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_cov.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1141 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_cross.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1747 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_cumprod.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1736 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_cumsum.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3837 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_det.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2197 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_diagmat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1450 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_diagvec.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1687 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_diff.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     7012 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_dot.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     4054 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_eig_gen.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3041 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_eig_pair.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     4538 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_eig_sym.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3520 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_eigs_gen.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3320 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_eigs_sym.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    21305 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_elem.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2231 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_eps.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2304 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_expmat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2782 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_eye.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2961 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_fft.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3156 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_fft2.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     7304 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_find.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1581 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_find_unique.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1691 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_flip.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3643 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_hess.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1994 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_hist.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1684 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_histc.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3156 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_index_max.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3156 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_index_min.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2595 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_inplace_strans.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2442 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_inplace_trans.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     8822 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_interp1.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     8197 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_interp2.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1605 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_intersect.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     7737 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_inv.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    11090 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_join.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1554 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_kmeans.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2409 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_kron.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3165 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_log_det.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3486 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_logmat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2269 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_lu.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     5279 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_max.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2752 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_mean.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1698 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_median.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     5279 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_min.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    12474 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_misc.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2729 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_mvnrnd.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3291 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_n_unique.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1244 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_nonzeros.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     7189 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_norm.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2523 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_normalise.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     5824 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_normcdf.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     5342 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_normpdf.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1780 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_numel.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3830 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_ones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2410 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_orth_null.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2221 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_pinv.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1742 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_polyfit.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1248 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_polyval.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     4450 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_princomp.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2103 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_prod.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2040 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_qr.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1868 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_qz.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     6611 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_randg.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     5410 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_randi.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     4355 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_randn.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3161 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_randperm.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     4329 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_randu.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1562 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_range.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1783 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_rank.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     5705 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_regspace.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1330 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_repelem.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1323 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_repmat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     4322 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_reshape.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2444 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_resize.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1882 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_reverse.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1616 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_roots.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2500 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_schur.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2062 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_shift.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1650 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_shuffle.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     4694 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_size.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     9829 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_solve.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     4487 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_sort.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3710 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_sort_index.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2110 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_speye.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1346 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_spones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2850 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_sprandn.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2816 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_sprandu.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     5492 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_spsolve.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3365 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_sqrtmat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1923 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_stddev.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2622 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_strans.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2763 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_sum.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     4704 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_svd.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     9154 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_svds.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2604 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_syl_lyap.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3516 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_symmat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1533 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_toeplitz.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    16312 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_trace.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1989 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_trans.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1426 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_trapz.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     8752 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_trig.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3407 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_trimat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1904 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_trunc_exp.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2027 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_trunc_log.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1323 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_unique.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2896 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_var.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2358 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_vectorise.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     4214 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_wishrnd.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     4705 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/fn_zeros.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1743 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/glue_affmul_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    12978 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/glue_affmul_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1493 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/glue_atan2_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     5681 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/glue_atan2_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1606 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/glue_conv_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     8897 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/glue_conv_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1216 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/glue_cor_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2152 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/glue_cor_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1216 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/glue_cov_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2054 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/glue_cov_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1169 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/glue_cross_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2412 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/glue_cross_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1509 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/glue_hist_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     6262 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/glue_hist_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1506 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/glue_histc_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     4559 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/glue_histc_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1493 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/glue_hypot_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     4113 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/glue_hypot_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1453 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/glue_intersect_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3395 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/glue_intersect_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2836 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/glue_join_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    11657 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/glue_join_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1656 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/glue_kron_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3504 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/glue_kron_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1788 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/glue_max_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     6523 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/glue_max_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1788 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/glue_min_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     6523 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/glue_min_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3019 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/glue_mixed_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    15254 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/glue_mixed_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1718 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/glue_mvnrnd_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     4850 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/glue_mvnrnd_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1511 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/glue_polyfit_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3372 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/glue_polyfit_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1296 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/glue_polyval_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1951 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/glue_polyval_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3493 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/glue_relational_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     8023 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/glue_relational_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     5402 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/glue_solve_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    17305 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/glue_solve_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     5293 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/glue_times_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    34538 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/glue_times_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1016 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/glue_toeplitz_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1906 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/glue_toeplitz_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1574 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/glue_trapz_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3733 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/glue_trapz_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     7179 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/gmm_diag_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    65539 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/gmm_diag_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     6978 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/gmm_full_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    67945 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/gmm_full_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3638 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/gmm_misc_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3129 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/gmm_misc_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    20647 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/hdf5_misc.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1377 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/include_atlas.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1365 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/include_hdf5.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     9903 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/include_superlu.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2566 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/injector_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    11015 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/injector_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     5866 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/memory.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1899 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/mp_misc.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1537 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/mtGlueCube_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1473 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/mtGlueCube_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1724 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/mtGlue_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1445 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/mtGlue_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2365 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/mtOpCube_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2704 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/mtOpCube_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2390 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/mtOp_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2521 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/mtOp_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1620 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/mtSpGlue_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1433 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/mtSpGlue_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2113 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/mtSpOp_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1870 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/mtSpOp_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    12770 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/mul_gemm.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    10728 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/mul_gemm_mixed.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    13014 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/mul_gemv.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    13647 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/mul_herk.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    12651 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/mul_syrk.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1211 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/newarp_DenseGenMatProd_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1345 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/newarp_DenseGenMatProd_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2508 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/newarp_DoubleShiftQR_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     9455 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/newarp_DoubleShiftQR_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2229 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/newarp_EigsSelect.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     4025 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/newarp_GenEigsSolver_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    11776 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/newarp_GenEigsSolver_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     5212 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/newarp_SortEigenvalue.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1219 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/newarp_SparseGenMatProd_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1349 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/newarp_SparseGenMatProd_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3860 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/newarp_SymEigsSolver_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    11768 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/newarp_SymEigsSolver_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1799 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/newarp_TridiagEigen_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3112 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/newarp_TridiagEigen_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2037 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/newarp_UpperHessenbergEigen_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     4191 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/newarp_UpperHessenbergEigen_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2547 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/newarp_UpperHessenbergQR_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     7405 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/newarp_UpperHessenbergQR_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1345 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/newarp_cx_attrib.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2127 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_all_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    11428 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_all_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2127 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_any_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    10489 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_any_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1458 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_chi2rnd_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3971 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_chi2rnd_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1139 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_chol_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2406 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_chol_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1839 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_clamp_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     6009 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_clamp_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1083 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_cond_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2696 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_cond_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1114 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_cor_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3035 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_cor_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1114 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_cov_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2637 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_cov_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1293 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_cumprod_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3706 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_cumprod_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1288 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_cumsum_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3695 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_cumsum_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     4051 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_cx_scalar_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    12332 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_cx_scalar_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1415 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_diagmat_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     5997 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_diagmat_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1359 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_diagvec_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3374 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_diagvec_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1293 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_diff_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     4995 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_diff_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3575 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_dot_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    13170 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_dot_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1528 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_dotext_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3783 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_dotext_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1458 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_expmat_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     4584 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_expmat_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2002 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_fft_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     8593 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_fft_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3025 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_find_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    15563 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_find_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1860 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_find_unique_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3030 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_find_unique_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1602 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_flip_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     6062 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_flip_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1106 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_hist_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2790 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_hist_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     4103 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_htrans_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    14274 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_htrans_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1752 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_index_max_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     9985 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_index_max_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1752 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_index_min_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     9985 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_index_min_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1723 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_inv_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3672 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_inv_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2555 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_logmat_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     9789 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_logmat_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3957 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_max_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    27214 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_max_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3247 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_mean_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    14153 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_mean_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1978 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_median_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    11241 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_median_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3959 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_min_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    27217 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_min_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2195 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_misc_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     8945 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_misc_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1331 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_nonzeros_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2925 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_nonzeros_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3349 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_norm_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    20201 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_norm_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1313 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_normalise_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3420 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_normalise_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1505 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_orth_null_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     4150 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_orth_null_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1175 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_pinv_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     4137 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_pinv_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2047 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_princomp_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     8194 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_princomp_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1273 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_prod_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     4316 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_prod_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1184 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_range_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2234 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_range_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3854 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_relational_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    10234 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_relational_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1152 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_repelem_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2706 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_repelem_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1149 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_repmat_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3334 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_repmat_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1651 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_reshape_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     9015 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_reshape_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1104 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_resize_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3546 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_resize_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1181 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_reverse_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2354 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_reverse_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1329 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_roots_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3297 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_roots_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1579 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_shift_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     5550 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_shift_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1287 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_shuffle_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     5430 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_shuffle_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1704 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_sort_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3257 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_sort_index_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     4420 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_sort_index_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     4787 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_sort_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2570 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_sp_minus_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     6739 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_sp_minus_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1647 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_sp_plus_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3747 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_sp_plus_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2352 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_sqrtmat_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     8036 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_sqrtmat_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1046 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_stddev_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2648 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_stddev_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3869 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_strans_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    20110 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_strans_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2356 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_sum_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    12428 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_sum_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1173 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_symmat_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     5233 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_symmat_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1181 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_toeplitz_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2725 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_toeplitz_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2174 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_trimat_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     9932 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_trimat_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1825 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_unique_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3586 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_unique_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2013 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_var_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     7196 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_var_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2356 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_vectorise_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     8852 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_vectorise_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1998 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_wishrnd_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     7225 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/op_wishrnd_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     4533 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/operator_cube_div.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     4772 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/operator_cube_minus.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     4834 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/operator_cube_plus.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     7523 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/operator_cube_relational.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3176 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/operator_cube_schur.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2815 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/operator_cube_times.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     8483 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/operator_div.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    12570 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/operator_minus.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3111 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/operator_ostream.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    12134 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/operator_plus.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     8602 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/operator_relational.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     9043 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/operator_schur.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    10985 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/operator_times.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2399 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/podarray_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     7031 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/podarray_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    14914 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/promote_type.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     9996 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/restrictors.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3005 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/running_stat_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     8559 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/running_stat_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     5655 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/running_stat_vec_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    14416 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/running_stat_vec_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     4444 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/sp_auxlib_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    49055 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/sp_auxlib_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1650 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/span.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3543 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/spdiagview_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    21592 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/spdiagview_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1162 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/spglue_elem_helper_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3143 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/spglue_elem_helper_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2635 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/spglue_join_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    10296 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/spglue_join_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1328 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/spglue_kron_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     4094 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/spglue_kron_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1691 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/spglue_max_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     5465 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/spglue_max_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1321 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/spglue_merge_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    14147 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/spglue_merge_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1691 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/spglue_min_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     5459 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/spglue_min_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1976 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/spglue_minus_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     8408 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/spglue_minus_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1768 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/spglue_plus_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     7250 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/spglue_plus_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1497 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/spglue_relational_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     7051 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/spglue_relational_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1991 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/spglue_schur_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     9148 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/spglue_schur_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2828 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/spglue_times_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    18473 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/spglue_times_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2097 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/spop_diagmat_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    10585 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/spop_diagmat_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1496 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/spop_htrans_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1565 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/spop_htrans_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2344 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/spop_max_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    15656 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/spop_max_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2257 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/spop_mean_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     8610 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/spop_mean_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2344 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/spop_min_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    16374 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/spop_min_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     5203 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/spop_misc_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    11453 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/spop_misc_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1134 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/spop_normalise_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     5360 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/spop_normalise_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1138 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/spop_repmat_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     4648 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/spop_repmat_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1237 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/spop_reverse_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3990 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/spop_reverse_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1474 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/spop_strans_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3110 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/spop_strans_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)      989 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/spop_sum_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2455 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/spop_sum_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1191 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/spop_symmat_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2382 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/spop_symmat_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1132 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/spop_trimat_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3452 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/spop_trimat_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2539 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/spop_var_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     9582 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/spop_var_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1632 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/spop_vectorise_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2554 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/spop_vectorise_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2923 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/strip.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    21282 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/subview_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     8797 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/subview_cube_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     4833 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/subview_cube_each_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    22436 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/subview_cube_each_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    64070 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/subview_cube_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3377 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/subview_cube_slices_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    11803 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/subview_cube_slices_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     5925 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/subview_each_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    30357 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/subview_each_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3915 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/subview_elem1_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    22905 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/subview_elem1_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3543 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/subview_elem2_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    19223 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/subview_elem2_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3272 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/subview_field_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    12376 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/subview_field_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    96617 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/subview_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     6152 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/sympd_helper.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    26376 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/traits.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     9700 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/translate_arpack.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    13125 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/translate_atlas.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    10351 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/translate_blas.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    81970 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/translate_lapack.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     4273 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/translate_superlu.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2473 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/trimat_helper.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     5112 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/typedef_elem.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2134 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/typedef_elem_check.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3966 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/typedef_mat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     9947 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/typedef_mat_fixed.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    72198 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/unwrap.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2250 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/unwrap_cube.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3963 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/unwrap_spmat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     5103 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/upgrade_val.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1330 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/wall_clock_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2371 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/wall_clock_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1673 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/xtrans_mat_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1989 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/xtrans_mat_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1566 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/xvec_htrans_bones.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2114 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/armadillo_bits/xvec_htrans_meat.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2393 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/bayesian.cpp
--rw-rw-r--   0 travis    (2000) travis    (2000)      365 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/bayesian.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    86846 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/c8lib.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     5670 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/c8lib.h
--rw-rw-r--   0 travis    (2000) travis    (2000)      112 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/cDP.pxd
--rw-rw-r--   0 travis    (2000) travis    (2000)      314 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/cDPQ.pxd
--rw-rw-r--   0 travis    (2000) travis    (2000)      228 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/cUnitSquareImage.pxd
--rw-rw-r--   0 travis    (2000) travis    (2000)      268 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/cbayesian.pxd
--rw-rw-r--   0 travis    (2000) travis    (2000)     1345 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/cbayesian.pyx
--rw-rw-r--   0 travis    (2000) travis    (2000)      253 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/cfPLS.pxd
--rw-rw-r--   0 travis    (2000) travis    (2000)      233 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/cmlogit.pxd
--rw-rw-r--   0 travis    (2000) travis    (2000)      239 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/coclogit.pxd
--rw-rw-r--   0 travis    (2000) travis    (2000)      250 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/cocmlogit.pxd
--rwxrwxr-x   0 travis    (2000) travis    (2000)     5186 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/cyarma.pxd
--rwxrwxr-x   0 travis    (2000) travis    (2000)     9637 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/cyarma.pyx
--rw-rw-r--   0 travis    (2000) travis    (2000)      319 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/dp_build.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4129 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/dp_grid.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     4289 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/dp_grid.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     3501 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/dp_nbhd.c
--rw-rw-r--   0 travis    (2000) travis    (2000)      171 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/dp_nbhd.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2354 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/fpls_warp.pyx
--rw-rw-r--   0 travis    (2000) travis    (2000)     6609 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/fpls_warp_grad.c
--rw-rw-r--   0 travis    (2000) travis    (2000)      190 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/fpls_warp_grad.h
--rw-rw-r--   0 travis    (2000) travis    (2000)   334639 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/imagecpp.cpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2056 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/imagecpp.pyx
--rw-rw-r--   0 travis    (2000) travis    (2000)     4781 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/matrix_exponential.c
--rw-rw-r--   0 travis    (2000) travis    (2000)      129 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/matrix_exponential.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    16436 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/misc_funcs.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     2098 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/misc_funcs.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2034 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/mlogit_warp.pyx
--rw-rw-r--   0 travis    (2000) travis    (2000)     5301 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/mlogit_warp_grad.c
--rw-rw-r--   0 travis    (2000) travis    (2000)      191 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/mlogit_warp_grad.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2543 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/myVector.cpp
--rw-rw-r--   0 travis    (2000) travis    (2000)      481 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/myVector.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2049 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/oclogit_warp.pyx
--rw-rw-r--   0 travis    (2000) travis    (2000)     5725 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/oclogit_warp_grad.c
--rw-rw-r--   0 travis    (2000) travis    (2000)      196 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/oclogit_warp_grad.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2114 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/ocmlogit_warp.pyx
--rw-rw-r--   0 travis    (2000) travis    (2000)     7383 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/ocmlogit_warp_grad.c
--rw-rw-r--   0 travis    (2000) travis    (2000)      206 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/ocmlogit_warp_grad.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    10666 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/optimum_reparamN2.pyx
--rw-rw-r--   0 travis    (2000) travis    (2000)     7480 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/optimum_reparam_N.pyx
--rw-rw-r--   0 travis    (2000) travis    (2000)   832370 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/r8lib.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    32641 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/src/r8lib.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-24 12:57:39.950606 fdasrsf-2.4.1/test/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4425 2023-05-24 12:54:23.000000 fdasrsf-2.4.1/test/test_all.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-21 17:51:22.488302 fdasrsf-2.4.2/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1522 2023-07-21 17:48:04.000000 fdasrsf-2.4.2/LICENSE.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      111 2023-07-21 17:48:04.000000 fdasrsf-2.4.2/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7522 2023-07-21 17:51:22.488302 fdasrsf-2.4.2/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6597 2023-07-21 17:48:04.000000 fdasrsf-2.4.2/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-21 17:51:22.428295 fdasrsf-2.4.2/bin/
+-rw-rw-r--   0 travis    (2000) travis    (2000)  2156461 2023-07-21 17:48:04.000000 fdasrsf-2.4.2/bin/MPEG7.npz
+-rw-rw-r--   0 travis    (2000) travis    (2000)      174 2023-07-21 17:48:04.000000 fdasrsf-2.4.2/bin/ex_srsf_align.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18146 2023-07-21 17:48:04.000000 fdasrsf-2.4.2/bin/simu_data.npz
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-21 17:51:22.424295 fdasrsf-2.4.2/doc/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-21 17:51:22.424295 fdasrsf-2.4.2/doc/build/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-21 17:51:22.428295 fdasrsf-2.4.2/doc/build/man/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    98266 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/doc/build/man/fdasrsf.1
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-21 17:51:22.432296 fdasrsf-2.4.2/fdasrsf/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2565 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/fdasrsf/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8417 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/fdasrsf/bayesian_functions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18148 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/fdasrsf/boxplots.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    28679 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/fdasrsf/curve_functions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5532 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/fdasrsf/curve_pcr_regression.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34875 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/fdasrsf/curve_regression.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14960 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/fdasrsf/curve_stats.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7146 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/fdasrsf/elastic_glm_regression.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17557 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/fdasrsf/fPCA.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1592 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/fdasrsf/fPLS.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16748 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/fdasrsf/geodesic.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2097 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/fdasrsf/geometry.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      644 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/fdasrsf/gp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2907 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/fdasrsf/image.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6763 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/fdasrsf/image_functions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7320 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/fdasrsf/kmeans.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    26063 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/fdasrsf/pcr_regression.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6921 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/fdasrsf/plot_style.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19590 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/fdasrsf/rbfgs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    30908 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/fdasrsf/regression.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    66925 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/fdasrsf/time_warping.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5229 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/fdasrsf/tolerance.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8929 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/fdasrsf/umap_metric.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29552 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/fdasrsf/utility_functions.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-21 17:51:22.432296 fdasrsf-2.4.2/fdasrsf.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7522 2023-07-21 17:51:22.000000 fdasrsf-2.4.2/fdasrsf.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23355 2023-07-21 17:51:22.000000 fdasrsf-2.4.2/fdasrsf.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-07-21 17:51:22.000000 fdasrsf-2.4.2/fdasrsf.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       80 2023-07-21 17:51:22.000000 fdasrsf-2.4.2/fdasrsf.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      114 2023-07-21 17:51:22.000000 fdasrsf-2.4.2/fdasrsf.egg-info/top_level.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-21 17:51:22.432296 fdasrsf-2.4.2/notebooks/
+-rw-rw-r--   0 travis    (2000) travis    (2000)   515522 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/notebooks/example_curve.ipynb
+-rw-rw-r--   0 travis    (2000) travis    (2000)  2208768 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/notebooks/example_warping.ipynb
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1234 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/pyproject.toml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      209 2023-07-21 17:51:22.488302 fdasrsf-2.4.2/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3848 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-21 17:51:22.440297 fdasrsf-2.4.2/src/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6436 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/DP.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)       81 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/DP.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1322 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/DynamicProgrammingQ2.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)      209 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/DynamicProgrammingQ2.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17484 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/ImageRegister.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20502 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/UnitSquareImage.cpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1607 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/UnitSquareImage.h
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-21 17:51:22.440297 fdasrsf-2.4.2/src/__pycache__/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      499 2023-07-21 17:51:22.000000 fdasrsf-2.4.2/src/__pycache__/dp_build.cpython-38.pyc
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29600 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-21 17:51:22.488302 fdasrsf-2.4.2/src/armadillo_bits/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2586 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/BaseCube_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6151 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/BaseCube_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5960 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/Base_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17954 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/Base_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10452 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/Col_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35001 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/Col_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1633 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/CubeToMatOp_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1294 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/CubeToMatOp_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    26562 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/Cube_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)   122156 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/Cube_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2320 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/GenCube_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5327 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/GenCube_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1723 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/GenSpecialiser.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2428 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/Gen_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7185 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/Gen_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1437 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/GlueCube_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1225 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/GlueCube_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2186 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/Glue_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1359 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/Glue_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7793 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/MapMat_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34555 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/MapMat_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    43618 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/Mat_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)   195024 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/Mat_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2517 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/OpCube_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2841 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/OpCube_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2617 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/Op_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2133 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/Op_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    89635 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/Proxy.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22986 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/ProxyCube.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10441 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/Row_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34942 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/Row_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1541 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/SizeCube_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3299 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/SizeCube_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1479 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/SizeMat_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2704 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/SizeMat_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4328 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/SpBase_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13609 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/SpBase_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2739 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/SpCol_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8241 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/SpCol_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1697 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/SpGlue_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1594 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/SpGlue_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34828 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/SpMat_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25327 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/SpMat_iterators_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)   144757 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/SpMat_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1914 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/SpOp_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1674 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/SpOp_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24709 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/SpProxy.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2736 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/SpRow_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8959 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/SpRow_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16131 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/SpSubview_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    32307 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/SpSubview_iterators_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    33981 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/SpSubview_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2278 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/SpToDOp_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1266 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/SpToDOp_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2651 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/SpValProxy_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6557 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/SpValProxy_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2125 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/access.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13212 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/arma_cmath.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4176 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/arma_config.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12926 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/arma_forward.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2998 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/arma_ostream_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18819 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/arma_ostream_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2768 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/arma_rel_comparators.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11543 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/arma_rng.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4867 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/arma_rng_cxx11.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3856 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/arma_rng_cxx98.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1600 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/arma_static_check.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11121 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/arma_str.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1476 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/arma_version.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5601 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/arrayops_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18194 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/arrayops_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18669 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/auxlib_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)   178527 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/auxlib_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9571 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/band_helper.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1194 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/compiler_extra.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18078 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/compiler_setup.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)      815 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/compiler_setup_post.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1295 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/cond_rel_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2002 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/cond_rel_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10927 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/config.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11020 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/config.hpp.cmake
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10845 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/constants.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6993 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/constants_old.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    31865 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/debug.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10732 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/def_arpack.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9041 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/def_atlas.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10257 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/def_blas.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6638 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/def_hdf5.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)   106546 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/def_lapack.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4068 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/def_superlu.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15762 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/diagmat_proxy.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3707 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/diagview_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21581 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/diagview_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12922 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/diskio_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)   109914 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/diskio_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1292 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/distr_param.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2071 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/eGlueCube_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4160 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/eGlueCube_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2287 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/eGlue_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3786 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/eGlue_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2902 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/eOpCube_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3858 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/eOpCube_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2524 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/eOp_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3034 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/eOp_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3020 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/eglue_core_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    47137 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/eglue_core_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20246 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/eop_aux.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7192 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/eop_core_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    31181 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/eop_core_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11016 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fft_engine.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15975 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/field_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    61755 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/field_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20671 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_accu.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1869 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_all.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1869 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_any.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14171 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_approx_equal.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11396 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_as_scalar.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3717 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_chi2rnd.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2005 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_chol.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2761 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_clamp.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1363 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_cond.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2162 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_conv.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17558 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_conv_to.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1527 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_cor.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1525 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_cov.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1141 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_cross.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1747 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_cumprod.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1736 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_cumsum.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3837 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_det.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2197 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_diagmat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1450 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_diagvec.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1687 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_diff.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7012 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_dot.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4054 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_eig_gen.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3041 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_eig_pair.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4538 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_eig_sym.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3520 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_eigs_gen.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3320 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_eigs_sym.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21305 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_elem.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2231 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_eps.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2304 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_expmat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2782 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_eye.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2961 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_fft.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3156 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_fft2.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7304 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_find.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1581 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_find_unique.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1691 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_flip.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3643 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_hess.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1994 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_hist.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1684 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_histc.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3156 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_index_max.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3156 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_index_min.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2595 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_inplace_strans.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2442 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_inplace_trans.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8822 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_interp1.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8197 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_interp2.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1605 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_intersect.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7737 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_inv.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11090 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_join.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1554 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_kmeans.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2409 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_kron.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3165 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_log_det.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3486 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_logmat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2269 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_lu.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5279 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_max.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2752 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_mean.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1698 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_median.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5279 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_min.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12474 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_misc.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2729 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_mvnrnd.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3291 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_n_unique.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1244 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_nonzeros.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7189 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_norm.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2523 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_normalise.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5824 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_normcdf.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5342 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_normpdf.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1780 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_numel.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3830 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_ones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2410 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_orth_null.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2221 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_pinv.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1742 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_polyfit.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1248 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_polyval.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4450 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_princomp.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2103 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_prod.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2040 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_qr.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1868 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_qz.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6611 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_randg.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5410 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_randi.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4355 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_randn.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3161 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_randperm.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4329 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_randu.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1562 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_range.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1783 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_rank.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5705 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_regspace.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1330 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_repelem.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1323 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_repmat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4322 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_reshape.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2444 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_resize.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1882 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_reverse.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1616 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_roots.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2500 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_schur.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2062 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_shift.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1650 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_shuffle.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4694 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_size.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9829 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_solve.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4487 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_sort.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3710 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_sort_index.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2110 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_speye.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1346 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_spones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2850 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_sprandn.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2816 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_sprandu.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5492 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_spsolve.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3365 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_sqrtmat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1923 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_stddev.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2622 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_strans.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2763 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_sum.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4704 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_svd.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9154 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_svds.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2604 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_syl_lyap.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3516 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_symmat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1533 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_toeplitz.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16312 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_trace.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1989 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_trans.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1426 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_trapz.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8752 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_trig.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3407 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_trimat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1904 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_trunc_exp.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2027 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_trunc_log.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1323 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_unique.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2896 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_var.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2358 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_vectorise.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4214 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_wishrnd.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4705 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/fn_zeros.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1743 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/glue_affmul_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12978 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/glue_affmul_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1493 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/glue_atan2_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5681 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/glue_atan2_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1606 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/glue_conv_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8897 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/glue_conv_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1216 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/glue_cor_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2152 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/glue_cor_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1216 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/glue_cov_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2054 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/glue_cov_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1169 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/glue_cross_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2412 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/glue_cross_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1509 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/glue_hist_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6262 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/glue_hist_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1506 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/glue_histc_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4559 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/glue_histc_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1493 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/glue_hypot_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4113 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/glue_hypot_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1453 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/glue_intersect_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3395 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/glue_intersect_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2836 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/glue_join_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11657 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/glue_join_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1656 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/glue_kron_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3504 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/glue_kron_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1788 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/glue_max_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6523 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/glue_max_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1788 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/glue_min_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6523 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/glue_min_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3019 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/glue_mixed_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15254 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/glue_mixed_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1718 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/glue_mvnrnd_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4850 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/glue_mvnrnd_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1511 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/glue_polyfit_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3372 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/glue_polyfit_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1296 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/glue_polyval_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1951 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/glue_polyval_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3493 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/glue_relational_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8023 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/glue_relational_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5402 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/glue_solve_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17305 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/glue_solve_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5293 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/glue_times_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34538 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/glue_times_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1016 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/glue_toeplitz_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1906 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/glue_toeplitz_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1574 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/glue_trapz_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3733 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/glue_trapz_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7179 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/gmm_diag_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    65539 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/gmm_diag_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6978 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/gmm_full_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    67945 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/gmm_full_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3638 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/gmm_misc_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3129 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/gmm_misc_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20647 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/hdf5_misc.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1377 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/include_atlas.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1365 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/include_hdf5.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9903 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/include_superlu.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2566 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/injector_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11015 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/injector_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5866 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/memory.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1899 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/mp_misc.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1537 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/mtGlueCube_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1473 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/mtGlueCube_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1724 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/mtGlue_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1445 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/mtGlue_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2365 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/mtOpCube_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2704 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/mtOpCube_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2390 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/mtOp_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2521 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/mtOp_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1620 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/mtSpGlue_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1433 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/mtSpGlue_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2113 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/mtSpOp_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1870 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/mtSpOp_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12770 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/mul_gemm.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10728 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/mul_gemm_mixed.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13014 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/mul_gemv.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13647 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/mul_herk.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12651 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/mul_syrk.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1211 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/newarp_DenseGenMatProd_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1345 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/newarp_DenseGenMatProd_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2508 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/newarp_DoubleShiftQR_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9455 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/newarp_DoubleShiftQR_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2229 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/newarp_EigsSelect.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4025 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/newarp_GenEigsSolver_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11776 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/newarp_GenEigsSolver_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5212 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/newarp_SortEigenvalue.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1219 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/newarp_SparseGenMatProd_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1349 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/newarp_SparseGenMatProd_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3860 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/newarp_SymEigsSolver_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11768 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/newarp_SymEigsSolver_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1799 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/newarp_TridiagEigen_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3112 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/newarp_TridiagEigen_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2037 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/newarp_UpperHessenbergEigen_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4191 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/newarp_UpperHessenbergEigen_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2547 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/newarp_UpperHessenbergQR_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7405 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/newarp_UpperHessenbergQR_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1345 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/newarp_cx_attrib.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2127 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_all_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11428 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_all_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2127 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_any_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10489 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_any_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1458 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_chi2rnd_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3971 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_chi2rnd_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1139 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_chol_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2406 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_chol_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1839 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_clamp_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6009 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_clamp_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1083 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_cond_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2696 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_cond_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1114 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_cor_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3035 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_cor_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1114 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_cov_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2637 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_cov_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1293 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_cumprod_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3706 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_cumprod_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1288 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_cumsum_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3695 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_cumsum_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4051 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_cx_scalar_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12332 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_cx_scalar_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1415 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_diagmat_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5997 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_diagmat_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1359 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_diagvec_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3374 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_diagvec_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1293 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_diff_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4995 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_diff_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3575 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_dot_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13170 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_dot_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1528 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_dotext_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3783 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_dotext_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1458 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_expmat_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4584 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_expmat_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2002 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_fft_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8593 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_fft_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3025 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_find_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15563 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_find_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1860 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_find_unique_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3030 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_find_unique_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1602 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_flip_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6062 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_flip_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1106 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_hist_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2790 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_hist_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4103 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_htrans_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14274 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_htrans_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1752 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_index_max_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9985 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_index_max_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1752 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_index_min_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9985 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_index_min_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1723 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_inv_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3672 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_inv_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2555 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_logmat_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9789 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_logmat_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3957 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_max_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    27214 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_max_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3247 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_mean_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14153 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_mean_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1978 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_median_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11241 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_median_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3959 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_min_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    27217 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_min_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2195 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_misc_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8945 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_misc_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1331 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_nonzeros_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2925 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_nonzeros_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3349 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_norm_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20201 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_norm_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1313 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_normalise_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3420 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_normalise_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1505 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_orth_null_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4150 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_orth_null_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1175 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_pinv_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4137 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_pinv_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2047 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_princomp_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8194 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_princomp_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1273 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_prod_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4316 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_prod_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1184 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_range_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2234 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_range_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3854 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_relational_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10234 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_relational_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1152 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_repelem_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2706 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_repelem_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1149 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_repmat_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3334 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_repmat_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1651 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_reshape_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9015 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_reshape_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1104 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_resize_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3546 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_resize_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1181 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_reverse_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2354 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_reverse_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1329 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_roots_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3297 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_roots_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1579 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_shift_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5550 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_shift_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1287 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_shuffle_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5430 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_shuffle_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1704 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_sort_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3257 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_sort_index_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4420 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_sort_index_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4787 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_sort_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2570 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_sp_minus_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6739 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_sp_minus_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1647 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_sp_plus_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3747 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_sp_plus_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2352 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_sqrtmat_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8036 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_sqrtmat_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1046 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_stddev_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2648 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_stddev_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3869 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_strans_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20110 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_strans_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2356 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_sum_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12428 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_sum_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1173 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_symmat_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5233 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_symmat_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1181 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_toeplitz_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2725 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_toeplitz_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2174 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_trimat_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9932 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_trimat_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1825 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_unique_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3586 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_unique_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2013 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_var_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7196 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_var_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2356 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_vectorise_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8852 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_vectorise_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1998 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_wishrnd_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7225 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/op_wishrnd_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4533 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/operator_cube_div.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4772 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/operator_cube_minus.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4834 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/operator_cube_plus.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7523 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/operator_cube_relational.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3176 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/operator_cube_schur.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2815 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/operator_cube_times.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8483 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/operator_div.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12570 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/operator_minus.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3111 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/operator_ostream.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12134 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/operator_plus.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8602 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/operator_relational.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9043 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/operator_schur.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10985 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/operator_times.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2399 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/podarray_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7031 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/podarray_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14914 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/promote_type.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9996 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/restrictors.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3005 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/running_stat_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8559 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/running_stat_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5655 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/running_stat_vec_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14416 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/running_stat_vec_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4444 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/sp_auxlib_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    49055 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/sp_auxlib_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1650 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/span.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3543 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/spdiagview_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21592 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/spdiagview_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1162 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/spglue_elem_helper_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3143 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/spglue_elem_helper_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2635 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/spglue_join_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10296 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/spglue_join_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1328 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/spglue_kron_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4094 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/spglue_kron_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1691 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/spglue_max_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5465 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/spglue_max_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1321 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/spglue_merge_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14147 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/spglue_merge_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1691 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/spglue_min_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5459 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/spglue_min_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1976 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/spglue_minus_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8408 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/spglue_minus_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1768 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/spglue_plus_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7250 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/spglue_plus_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1497 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/spglue_relational_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7051 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/spglue_relational_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1991 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/spglue_schur_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9148 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/spglue_schur_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2828 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/spglue_times_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18473 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/spglue_times_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2097 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/spop_diagmat_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10585 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/spop_diagmat_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1496 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/spop_htrans_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1565 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/spop_htrans_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2344 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/spop_max_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15656 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/spop_max_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2257 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/spop_mean_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8610 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/spop_mean_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2344 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/spop_min_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16374 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/spop_min_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5203 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/spop_misc_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11453 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/spop_misc_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1134 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/spop_normalise_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5360 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/spop_normalise_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1138 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/spop_repmat_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4648 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/spop_repmat_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1237 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/spop_reverse_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3990 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/spop_reverse_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1474 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/spop_strans_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3110 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/spop_strans_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)      989 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/spop_sum_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2455 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/spop_sum_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1191 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/spop_symmat_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2382 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/spop_symmat_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1132 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/spop_trimat_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3452 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/spop_trimat_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2539 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/spop_var_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9582 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/spop_var_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1632 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/spop_vectorise_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2554 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/spop_vectorise_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2923 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/strip.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21282 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/subview_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8797 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/subview_cube_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4833 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/subview_cube_each_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22436 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/subview_cube_each_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    64070 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/subview_cube_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3377 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/subview_cube_slices_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11803 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/subview_cube_slices_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5925 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/subview_each_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    30357 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/subview_each_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3915 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/subview_elem1_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22905 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/subview_elem1_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3543 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/subview_elem2_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19223 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/subview_elem2_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3272 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/subview_field_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12376 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/subview_field_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    96617 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/subview_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6152 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/sympd_helper.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    26376 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/traits.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9700 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/translate_arpack.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13125 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/translate_atlas.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10351 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/translate_blas.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    81970 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/translate_lapack.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4273 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/translate_superlu.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2473 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/trimat_helper.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5112 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/typedef_elem.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2134 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/typedef_elem_check.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3966 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/typedef_mat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9947 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/typedef_mat_fixed.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    72198 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/unwrap.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2250 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/unwrap_cube.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3963 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/unwrap_spmat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5103 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/upgrade_val.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1330 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/wall_clock_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2371 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/wall_clock_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1673 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/xtrans_mat_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1989 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/xtrans_mat_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1566 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/xvec_htrans_bones.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2114 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/armadillo_bits/xvec_htrans_meat.hpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2393 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/bayesian.cpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)      365 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/bayesian.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    86846 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/c8lib.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5670 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/c8lib.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)      112 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/cDP.pxd
+-rw-rw-r--   0 travis    (2000) travis    (2000)      314 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/cDPQ.pxd
+-rw-rw-r--   0 travis    (2000) travis    (2000)      228 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/cUnitSquareImage.pxd
+-rw-rw-r--   0 travis    (2000) travis    (2000)      268 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/cbayesian.pxd
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1345 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/cbayesian.pyx
+-rw-rw-r--   0 travis    (2000) travis    (2000)      253 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/cfPLS.pxd
+-rw-rw-r--   0 travis    (2000) travis    (2000)      233 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/cmlogit.pxd
+-rw-rw-r--   0 travis    (2000) travis    (2000)      239 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/coclogit.pxd
+-rw-rw-r--   0 travis    (2000) travis    (2000)      250 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/cocmlogit.pxd
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     5186 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/cyarma.pxd
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     9637 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/cyarma.pyx
+-rw-rw-r--   0 travis    (2000) travis    (2000)      319 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/dp_build.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4129 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/dp_grid.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4289 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/dp_grid.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3501 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/dp_nbhd.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)      171 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/dp_nbhd.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2354 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/fpls_warp.pyx
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6609 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/fpls_warp_grad.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)      190 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/fpls_warp_grad.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2056 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/imagecpp.pyx
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4781 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/matrix_exponential.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)      129 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/matrix_exponential.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16436 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/misc_funcs.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2098 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/misc_funcs.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2034 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/mlogit_warp.pyx
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5301 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/mlogit_warp_grad.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)      191 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/mlogit_warp_grad.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2543 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/myVector.cpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)      481 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/myVector.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2049 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/oclogit_warp.pyx
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5725 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/oclogit_warp_grad.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)      196 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/oclogit_warp_grad.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2114 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/ocmlogit_warp.pyx
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7383 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/ocmlogit_warp_grad.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)      206 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/ocmlogit_warp_grad.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10666 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/optimum_reparamN2.pyx
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7480 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/optimum_reparam_N.pyx
+-rw-rw-r--   0 travis    (2000) travis    (2000)   832370 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/r8lib.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    32641 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/src/r8lib.h
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-21 17:51:22.488302 fdasrsf-2.4.2/test/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4425 2023-07-21 17:48:05.000000 fdasrsf-2.4.2/test/test_all.py
```

### Comparing `fdasrsf-2.4.1/LICENSE.txt` & `fdasrsf-2.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/PKG-INFO` & `fdasrsf-2.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fdasrsf
-Version: 2.4.1
+Version: 2.4.2
 Summary: functional data analysis using the square root slope framework
 Home-page: http://research.tetonedge.net
 Author: J. Derek Tucker
 Author-email: "J. Derek Tucker" <jdtuck@sandia.gov>
 License: BSD 3-Clause
 Project-URL: homepage, http://research.tetonedge.net
 Project-URL: repository, https://github.com/jdtuck/fdasrsf_python
@@ -36,15 +36,15 @@
 A python package for functional data analysis using the square root
 slope framework and curves using the square root velocity framework
 which performs pair-wise and group-wise alignment as well as modeling
 using functional component analysis and regression. 
 
 ### Installation
 ------------------------------------------------------------------------------
-v2.4.1 is on pip and can be installed using
+v2.4.2 is on pip and can be installed using
 > `pip install fdasrsf`
 
 or conda
 
 > `conda install -c conda-forge fdasrsf`
 
 To install the most up to date version on github
```

### Comparing `fdasrsf-2.4.1/README.md` & `fdasrsf-2.4.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 A python package for functional data analysis using the square root
 slope framework and curves using the square root velocity framework
 which performs pair-wise and group-wise alignment as well as modeling
 using functional component analysis and regression. 
 
 ### Installation
 ------------------------------------------------------------------------------
-v2.4.1 is on pip and can be installed using
+v2.4.2 is on pip and can be installed using
 > `pip install fdasrsf`
 
 or conda
 
 > `conda install -c conda-forge fdasrsf`
 
 To install the most up to date version on github
```

### Comparing `fdasrsf-2.4.1/bin/MPEG7.npz` & `fdasrsf-2.4.2/bin/MPEG7.npz`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/bin/simu_data.npz` & `fdasrsf-2.4.2/bin/simu_data.npz`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/doc/build/man/fdasrsf.1` & `fdasrsf-2.4.2/doc/build/man/fdasrsf.1`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/fdasrsf/__init__.py` & `fdasrsf-2.4.2/fdasrsf/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 slope framework which performs pair-wise and group-wise
 alignment as well as modeling using functional component
 analysis
 
 """
 __all__ = ["time_warping", "utility_functions", "bayesian_functions", "curve_stats", "geodesic", "curve_functions", 
            "geometry", "pcr_regression", "tolerance", "boxplots", "curve_regression", "regression", "fPCA", 
-           "elastic_glm_regression", "curve_pcr_regression", "kmeans", "image", "image_functions"]
+           "elastic_glm_regression", "curve_pcr_regression", "kmeans", "image", "image_functions", "gp"]
 
-__version__ = "2.4.1"
+__version__ = "2.4.2"
 
 import sys
 
 if sys.version_info[0] == 3 and sys.version_info[1] < 6:
     raise ImportError("Python Version 3.6 or above is required for fdasrsf.")
 else:  # Python 3
     pass
```

### Comparing `fdasrsf-2.4.1/fdasrsf/bayesian_functions.py` & `fdasrsf-2.4.2/fdasrsf/bayesian_functions.py`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/fdasrsf/boxplots.py` & `fdasrsf-2.4.2/fdasrsf/boxplots.py`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/fdasrsf/curve_functions.py` & `fdasrsf-2.4.2/fdasrsf/curve_functions.py`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/fdasrsf/curve_pcr_regression.py` & `fdasrsf-2.4.2/fdasrsf/curve_pcr_regression.py`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/fdasrsf/curve_regression.py` & `fdasrsf-2.4.2/fdasrsf/curve_regression.py`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/fdasrsf/curve_stats.py` & `fdasrsf-2.4.2/fdasrsf/curve_stats.py`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/fdasrsf/elastic_glm_regression.py` & `fdasrsf-2.4.2/fdasrsf/elastic_glm_regression.py`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/fdasrsf/fPCA.py` & `fdasrsf-2.4.2/fdasrsf/fPCA.py`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/fdasrsf/fPLS.py` & `fdasrsf-2.4.2/fdasrsf/fPLS.py`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/fdasrsf/geodesic.py` & `fdasrsf-2.4.2/fdasrsf/geodesic.py`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/fdasrsf/geometry.py` & `fdasrsf-2.4.2/fdasrsf/geometry.py`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/fdasrsf/image.py` & `fdasrsf-2.4.2/fdasrsf/image.py`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/fdasrsf/image_functions.py` & `fdasrsf-2.4.2/fdasrsf/image_functions.py`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/fdasrsf/kmeans.py` & `fdasrsf-2.4.2/fdasrsf/kmeans.py`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/fdasrsf/pcr_regression.py` & `fdasrsf-2.4.2/fdasrsf/pcr_regression.py`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/fdasrsf/plot_style.py` & `fdasrsf-2.4.2/fdasrsf/plot_style.py`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/fdasrsf/rbfgs.py` & `fdasrsf-2.4.2/fdasrsf/rbfgs.py`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/fdasrsf/regression.py` & `fdasrsf-2.4.2/fdasrsf/regression.py`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/fdasrsf/time_warping.py` & `fdasrsf-2.4.2/fdasrsf/time_warping.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 """
 import numpy as np
 import matplotlib.pyplot as plt
 import fdasrsf.utility_functions as uf
 import fdasrsf.bayesian_functions as bf
 import fdasrsf.fPCA as fpca
 import fdasrsf.geometry as geo
+from fdasrsf.gp import gp_posterior
 from scipy.integrate import trapz, cumtrapz
 from scipy.interpolate import interp1d
 from scipy.linalg import svd, cholesky
 from scipy.cluster.hierarchy import linkage, fcluster
 from scipy.spatial.distance import squareform, pdist
-import GPy
 from numpy.linalg import norm, inv
 from numpy.random import rand, normal
 from joblib import Parallel, delayed
 from fdasrsf.fPLS import pls_svd
 from tqdm import tqdm
 import fdasrsf.plot_style as plot
 import fpls_warp as fpls
@@ -1104,29 +1104,28 @@
     # f1,f2 prior, propoposal params
     sigma1_ini = 0.01
     sigma2_ini = 0.01
     f1_propvar = mcmcopts["f1propvar"]
     f2_propvar = mcmcopts["f2propvar"]
     y1itmp = y1i[0::mcmcopts["sampfreq"]]
     timetmp = time[0::mcmcopts["sampfreq"]]
-    kernel1 = GPy.kern.RBF(input_dim=1, variance=y1itmp.std()/np.sqrt(2), lengthscale=np.mean(timetmp.std()))
     y2itmp = y2i[0::mcmcopts["sampfreq"]]
-    kernel2 = GPy.kern.RBF(input_dim=1, variance=y2itmp.std()/np.sqrt(2), lengthscale=np.mean(timetmp.std()))
     M1 = timetmp.shape[0]
-    model1 = GPy.models.GPRegression(timetmp.reshape((M1,1)),y1itmp.reshape((M1,1)),kernel1)
-    model1.optimize()
-    model2 = GPy.models.GPRegression(timetmp.reshape((M1,1)),y2itmp.reshape((M1,1)),kernel2)
-    model2.optimize()
 
-    s1_ini = model1.kern.param_array[0]
-    s2_ini = model2.kern.param_array[0]
+    f1_curr, predvar = gp_posterior(timetmp.reshape((M1,1)), y1itmp.reshape((M1,1)), timetmp.reshape((M1,1)), 
+                                    l2=np.mean(timetmp.std()), noise_var=y1itmp.std()/np.sqrt(2))
+    f2_curr, predvar = gp_posterior(timetmp.reshape((M1,1)), y2itmp.reshape((M1,1)), timetmp.reshape((M1,1)), 
+                                    l2=np.mean(timetmp.std()), noise_var=y2itmp.std()/np.sqrt(2))
+
+    s1_ini = y1itmp.std()/np.sqrt(2)
+    s2_ini = y2itmp.std()/np.sqrt(2)
     L1_propvar = mcmcopts["L1propvar"]
     L2_propvar = mcmcopts["L2propvar"]
-    L1_ini = model2.kern.param_array[1]
-    L2_ini = model2.kern.param_array[1]
+    L1_ini = np.mean(timetmp.std())
+    L2_ini = np.mean(timetmp.std())
 
     K_f1_corr = uf.exp2corr2(L1_ini,Dmat)+0.1 * np.eye(y1i.shape[0])
     K_f1 = s1_ini * K_f1_corr
     K_f1 = inv(K_f1)
     K_f2_corr = uf.exp2corr2(L2_ini,Dmat)+0.1 * np.eye(y2i.shape[0])
     K_f2 = s2_ini * K_f2_corr
     K_f2 = inv(K_f2)
@@ -1159,17 +1158,20 @@
     v_curr = uf.f_basistofunction(v_basis["x"],0,v_coef_ini,v_basis)
     sigma_curr = sigma_ini
     sigma1_curr = sigma1_ini
     sigma2_curr = sigma2_ini
     L1_curr = L1_ini
     L2_curr = L2_ini
 
-    f1_curr, predvar = model1.predict(time.reshape((T,1)))
+    f1_curr, predvar = gp_posterior(timetmp.reshape((M1,1)), y1itmp.reshape((M1,1)), time.reshape((T,1)), 
+                                    l2=np.mean(timetmp.std()), noise_var=y1itmp.std()/np.sqrt(2))
+    f2_curr, predvar = gp_posterior(timetmp.reshape((M1,1)), y2itmp.reshape((M1,1)), time.reshape((T,1)), 
+                                    l2=np.mean(timetmp.std()), noise_var=y2itmp.std()/np.sqrt(2))
+    
     f1_curr = f1_curr.reshape(T)
-    f2_curr, predvar = model2.predict(time.reshape((T,1)))
     f2_curr = f2_curr.reshape(T)
 
     # srsf transformation
     q1_curr = uf.f_to_srsf(f1_curr, time)
     q2_curr = uf.f_to_srsf(f2_curr, time)
 
     SSE_curr = bf.f_SSEv_pw(v_curr, q1_curr, q2_curr)
```

### Comparing `fdasrsf-2.4.1/fdasrsf/tolerance.py` & `fdasrsf-2.4.2/fdasrsf/tolerance.py`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/fdasrsf/umap_metric.py` & `fdasrsf-2.4.2/fdasrsf/umap_metric.py`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/fdasrsf/utility_functions.py` & `fdasrsf-2.4.2/fdasrsf/utility_functions.py`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/fdasrsf.egg-info/PKG-INFO` & `fdasrsf-2.4.2/fdasrsf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fdasrsf
-Version: 2.4.1
+Version: 2.4.2
 Summary: functional data analysis using the square root slope framework
 Home-page: http://research.tetonedge.net
 Author: J. Derek Tucker
 Author-email: "J. Derek Tucker" <jdtuck@sandia.gov>
 License: BSD 3-Clause
 Project-URL: homepage, http://research.tetonedge.net
 Project-URL: repository, https://github.com/jdtuck/fdasrsf_python
@@ -36,15 +36,15 @@
 A python package for functional data analysis using the square root
 slope framework and curves using the square root velocity framework
 which performs pair-wise and group-wise alignment as well as modeling
 using functional component analysis and regression. 
 
 ### Installation
 ------------------------------------------------------------------------------
-v2.4.1 is on pip and can be installed using
+v2.4.2 is on pip and can be installed using
 > `pip install fdasrsf`
 
 or conda
 
 > `conda install -c conda-forge fdasrsf`
 
 To install the most up to date version on github
```

### Comparing `fdasrsf-2.4.1/fdasrsf.egg-info/SOURCES.txt` & `fdasrsf-2.4.2/fdasrsf.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 fdasrsf/curve_regression.py
 fdasrsf/curve_stats.py
 fdasrsf/elastic_glm_regression.py
 fdasrsf/fPCA.py
 fdasrsf/fPLS.py
 fdasrsf/geodesic.py
 fdasrsf/geometry.py
+fdasrsf/gp.py
 fdasrsf/image.py
 fdasrsf/image_functions.py
 fdasrsf/kmeans.py
 fdasrsf/pcr_regression.py
 fdasrsf/plot_style.py
 fdasrsf/rbfgs.py
 fdasrsf/regression.py
@@ -65,15 +66,14 @@
 src/dp_grid.c
 src/dp_grid.h
 src/dp_nbhd.c
 src/dp_nbhd.h
 src/fpls_warp.pyx
 src/fpls_warp_grad.c
 src/fpls_warp_grad.h
-src/imagecpp.cpp
 src/imagecpp.pyx
 src/matrix_exponential.c
 src/matrix_exponential.h
 src/misc_funcs.c
 src/misc_funcs.h
 src/mlogit_warp.pyx
 src/mlogit_warp_grad.c
@@ -86,15 +86,15 @@
 src/ocmlogit_warp.pyx
 src/ocmlogit_warp_grad.c
 src/ocmlogit_warp_grad.h
 src/optimum_reparamN2.pyx
 src/optimum_reparam_N.pyx
 src/r8lib.c
 src/r8lib.h
-src/__pycache__/dp_build.cpython-39.pyc
+src/__pycache__/dp_build.cpython-38.pyc
 src/armadillo_bits/BaseCube_bones.hpp
 src/armadillo_bits/BaseCube_meat.hpp
 src/armadillo_bits/Base_bones.hpp
 src/armadillo_bits/Base_meat.hpp
 src/armadillo_bits/Col_bones.hpp
 src/armadillo_bits/Col_meat.hpp
 src/armadillo_bits/CubeToMatOp_bones.hpp
```

### Comparing `fdasrsf-2.4.1/notebooks/example_curve.ipynb` & `fdasrsf-2.4.2/notebooks/example_curve.ipynb`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/notebooks/example_warping.ipynb` & `fdasrsf-2.4.2/notebooks/example_warping.ipynb`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/pyproject.toml` & `fdasrsf-2.4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "fdasrsf"
-version = "2.4.1"
+version = "2.4.2"
 description = "functional data analysis using the square root slope framework"
 authors = [
 	{name = "J. Derek Tucker", email = "jdtuck@sandia.gov"}
 ]
 license = {text = "BSD 3-Clause"}
 readme = "README.md"
 requires-python = ">=3.6"
@@ -17,15 +17,14 @@
         "numpy",
         "scipy",
         "joblib",
         "patsy",
         "tqdm",
         "six",
         "numba",
-        "GPy",
         "cffi>=1.0.0",
         "pyparsing",
     ]
 
 classifiers = [
     'License :: OSI Approved :: BSD License',
     'Operating System :: OS Independent',
```

### Comparing `fdasrsf-2.4.1/setup.py` & `fdasrsf-2.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 ]
 
 
 setup(
     cmdclass={'build_ext': build_ext, 'build_docs': build_docs},
 	ext_modules=extensions,
     name='fdasrsf',
-    version='2.4.1',
+    version='2.4.2',
     packages=['fdasrsf'],
     url='http://research.tetonedge.net',
     license='LICENSE.txt',
     author='J. Derek Tucker',
     author_email='jdtuck@sandia.gov',
     scripts=['bin/ex_srsf_align.py'],
     keywords=['functional data analysis'],
```

### Comparing `fdasrsf-2.4.1/src/DP.c` & `fdasrsf-2.4.2/src/DP.c`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/DynamicProgrammingQ2.c` & `fdasrsf-2.4.2/src/DynamicProgrammingQ2.c`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/ImageRegister.h` & `fdasrsf-2.4.2/src/ImageRegister.h`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/UnitSquareImage.cpp` & `fdasrsf-2.4.2/src/UnitSquareImage.cpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/UnitSquareImage.h` & `fdasrsf-2.4.2/src/UnitSquareImage.h`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo` & `fdasrsf-2.4.2/src/armadillo`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/BaseCube_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/BaseCube_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/BaseCube_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/BaseCube_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/Base_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/Base_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/Base_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/Base_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/Col_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/Col_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/Col_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/Col_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/CubeToMatOp_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/CubeToMatOp_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/CubeToMatOp_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/CubeToMatOp_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/Cube_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/Cube_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/Cube_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/Cube_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/GenCube_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/GenCube_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/GenCube_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/GenCube_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/GenSpecialiser.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/GenSpecialiser.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/Gen_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/Gen_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/Gen_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/Gen_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/GlueCube_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/GlueCube_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/GlueCube_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/GlueCube_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/Glue_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/Glue_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/Glue_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/Glue_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/MapMat_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/MapMat_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/MapMat_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/MapMat_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/Mat_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/Mat_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/Mat_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/Mat_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/OpCube_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/OpCube_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/OpCube_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/OpCube_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/Op_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/Op_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/Op_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/Op_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/Proxy.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/Proxy.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/ProxyCube.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/ProxyCube.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/Row_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/Row_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/Row_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/Row_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/SizeCube_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/SizeCube_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/SizeCube_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/SizeCube_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/SizeMat_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/SizeMat_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/SizeMat_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/SizeMat_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/SpBase_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/SpBase_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/SpBase_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/SpBase_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/SpCol_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/SpCol_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/SpCol_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/SpCol_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/SpGlue_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/SpGlue_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/SpGlue_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/SpGlue_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/SpMat_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/SpMat_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/SpMat_iterators_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/SpMat_iterators_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/SpMat_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/SpMat_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/SpOp_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/SpOp_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/SpOp_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/SpOp_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/SpProxy.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/SpProxy.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/SpRow_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/SpRow_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/SpRow_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/SpRow_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/SpSubview_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/SpSubview_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/SpSubview_iterators_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/SpSubview_iterators_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/SpSubview_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/SpSubview_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/SpToDOp_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/SpToDOp_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/SpToDOp_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/SpToDOp_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/SpValProxy_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/SpValProxy_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/SpValProxy_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/SpValProxy_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/access.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/access.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/arma_cmath.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/arma_cmath.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/arma_config.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/arma_config.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/arma_forward.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/arma_forward.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/arma_ostream_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/arma_ostream_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/arma_ostream_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/arma_ostream_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/arma_rel_comparators.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/arma_rel_comparators.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/arma_rng.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/arma_rng.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/arma_rng_cxx11.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/arma_rng_cxx11.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/arma_rng_cxx98.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/arma_rng_cxx98.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/arma_static_check.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/arma_static_check.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/arma_str.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/arma_str.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/arma_version.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/arma_version.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/arrayops_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/arrayops_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/arrayops_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/arrayops_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/auxlib_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/auxlib_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/auxlib_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/auxlib_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/band_helper.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/band_helper.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/compiler_extra.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/compiler_extra.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/compiler_setup.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/compiler_setup.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/compiler_setup_post.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/compiler_setup_post.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/cond_rel_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/cond_rel_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/cond_rel_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/cond_rel_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/config.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/config.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/config.hpp.cmake` & `fdasrsf-2.4.2/src/armadillo_bits/config.hpp.cmake`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/constants.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/constants.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/constants_old.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/constants_old.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/debug.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/debug.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/def_arpack.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/def_arpack.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/def_atlas.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/def_atlas.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/def_blas.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/def_blas.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/def_hdf5.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/def_hdf5.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/def_lapack.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/def_lapack.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/def_superlu.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/def_superlu.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/diagmat_proxy.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/diagmat_proxy.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/diagview_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/diagview_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/diagview_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/diagview_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/diskio_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/diskio_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/diskio_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/diskio_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/distr_param.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/distr_param.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/eGlueCube_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/eGlueCube_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/eGlueCube_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/eGlueCube_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/eGlue_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/eGlue_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/eGlue_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/eGlue_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/eOpCube_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/eOpCube_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/eOpCube_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/eOpCube_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/eOp_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/eOp_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/eOp_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/eOp_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/eglue_core_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/eglue_core_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/eglue_core_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/eglue_core_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/eop_aux.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/eop_aux.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/eop_core_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/eop_core_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/eop_core_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/eop_core_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fft_engine.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fft_engine.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/field_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/field_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/field_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/field_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_accu.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_accu.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_all.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_all.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_any.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_any.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_approx_equal.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_approx_equal.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_as_scalar.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_as_scalar.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_chi2rnd.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_chi2rnd.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_chol.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_chol.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_clamp.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_clamp.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_cond.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_cond.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_conv.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_conv.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_conv_to.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_conv_to.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_cor.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_cor.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_cov.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_cov.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_cross.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_cross.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_cumprod.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_cumprod.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_cumsum.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_cumsum.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_det.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_det.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_diagmat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_diagmat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_diagvec.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_diagvec.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_diff.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_diff.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_dot.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_dot.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_eig_gen.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_eig_gen.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_eig_pair.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_eig_pair.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_eig_sym.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_eig_sym.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_eigs_gen.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_eigs_gen.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_eigs_sym.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_eigs_sym.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_elem.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_elem.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_eps.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_eps.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_expmat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_expmat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_eye.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_eye.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_fft.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_fft.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_fft2.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_fft2.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_find.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_find.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_find_unique.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_find_unique.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_flip.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_flip.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_hess.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_hess.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_hist.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_hist.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_histc.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_histc.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_index_max.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_index_max.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_index_min.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_index_min.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_inplace_strans.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_inplace_strans.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_inplace_trans.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_inplace_trans.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_interp1.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_interp1.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_interp2.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_interp2.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_intersect.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_intersect.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_inv.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_inv.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_join.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_join.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_kmeans.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_kmeans.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_kron.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_kron.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_log_det.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_log_det.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_logmat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_logmat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_lu.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_lu.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_max.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_max.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_mean.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_mean.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_median.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_median.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_min.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_min.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_misc.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_misc.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_mvnrnd.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_mvnrnd.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_n_unique.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_n_unique.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_nonzeros.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_nonzeros.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_norm.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_norm.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_normalise.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_normalise.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_normcdf.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_normcdf.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_normpdf.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_normpdf.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_numel.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_numel.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_ones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_ones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_orth_null.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_orth_null.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_pinv.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_pinv.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_polyfit.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_polyfit.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_polyval.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_polyval.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_princomp.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_princomp.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_prod.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_prod.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_qr.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_qr.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_qz.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_qz.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_randg.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_randg.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_randi.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_randi.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_randn.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_randn.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_randperm.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_randperm.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_randu.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_randu.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_range.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_range.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_rank.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_rank.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_regspace.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_regspace.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_repelem.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_repelem.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_repmat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_repmat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_reshape.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_reshape.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_resize.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_resize.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_reverse.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_reverse.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_roots.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_roots.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_schur.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_schur.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_shift.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_shift.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_shuffle.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_shuffle.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_size.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_size.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_solve.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_solve.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_sort.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_sort.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_sort_index.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_sort_index.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_speye.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_speye.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_spones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_spones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_sprandn.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_sprandn.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_sprandu.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_sprandu.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_spsolve.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_spsolve.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_sqrtmat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_sqrtmat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_stddev.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_stddev.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_strans.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_strans.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_sum.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_sum.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_svd.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_svd.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_svds.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_svds.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_syl_lyap.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_syl_lyap.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_symmat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_symmat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_toeplitz.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_toeplitz.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_trace.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_trace.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_trans.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_trans.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_trapz.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_trapz.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_trig.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_trig.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_trimat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_trimat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_trunc_exp.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_trunc_exp.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_trunc_log.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_trunc_log.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_unique.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_unique.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_var.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_var.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_vectorise.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_vectorise.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_wishrnd.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_wishrnd.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/fn_zeros.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/fn_zeros.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/glue_affmul_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/glue_affmul_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/glue_affmul_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/glue_affmul_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/glue_atan2_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/glue_atan2_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/glue_atan2_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/glue_atan2_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/glue_conv_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/glue_conv_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/glue_conv_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/glue_conv_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/glue_cor_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/glue_cor_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/glue_cor_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/glue_cor_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/glue_cov_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/glue_cov_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/glue_cov_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/glue_cov_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/glue_cross_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/glue_cross_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/glue_cross_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/glue_cross_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/glue_hist_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/glue_hist_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/glue_hist_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/glue_hist_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/glue_histc_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/glue_histc_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/glue_histc_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/glue_histc_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/glue_hypot_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/glue_hypot_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/glue_hypot_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/glue_hypot_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/glue_intersect_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/glue_intersect_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/glue_intersect_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/glue_intersect_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/glue_join_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/glue_join_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/glue_join_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/glue_join_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/glue_kron_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/glue_kron_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/glue_kron_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/glue_kron_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/glue_max_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/glue_max_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/glue_max_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/glue_max_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/glue_min_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/glue_min_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/glue_min_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/glue_min_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/glue_mixed_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/glue_mixed_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/glue_mixed_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/glue_mixed_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/glue_mvnrnd_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/glue_mvnrnd_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/glue_mvnrnd_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/glue_mvnrnd_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/glue_polyfit_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/glue_polyfit_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/glue_polyfit_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/glue_polyfit_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/glue_polyval_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/glue_polyval_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/glue_polyval_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/glue_polyval_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/glue_relational_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/glue_relational_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/glue_relational_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/glue_relational_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/glue_solve_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/glue_solve_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/glue_solve_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/glue_solve_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/glue_times_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/glue_times_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/glue_times_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/glue_times_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/glue_toeplitz_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/glue_toeplitz_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/glue_toeplitz_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/glue_toeplitz_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/glue_trapz_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/glue_trapz_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/glue_trapz_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/glue_trapz_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/gmm_diag_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/gmm_diag_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/gmm_diag_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/gmm_diag_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/gmm_full_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/gmm_full_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/gmm_full_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/gmm_full_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/gmm_misc_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/gmm_misc_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/gmm_misc_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/gmm_misc_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/hdf5_misc.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/hdf5_misc.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/include_atlas.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/include_atlas.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/include_hdf5.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/include_hdf5.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/include_superlu.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/include_superlu.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/injector_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/injector_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/injector_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/injector_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/memory.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/memory.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/mp_misc.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/mp_misc.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/mtGlueCube_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/mtGlueCube_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/mtGlueCube_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/mtGlueCube_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/mtGlue_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/mtGlue_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/mtGlue_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/mtGlue_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/mtOpCube_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/mtOpCube_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/mtOpCube_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/mtOpCube_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/mtOp_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/mtOp_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/mtOp_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/mtOp_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/mtSpGlue_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/mtSpGlue_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/mtSpGlue_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/mtSpGlue_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/mtSpOp_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/mtSpOp_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/mtSpOp_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/mtSpOp_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/mul_gemm.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/mul_gemm.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/mul_gemm_mixed.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/mul_gemm_mixed.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/mul_gemv.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/mul_gemv.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/mul_herk.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/mul_herk.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/mul_syrk.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/mul_syrk.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/newarp_DenseGenMatProd_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/newarp_DenseGenMatProd_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/newarp_DenseGenMatProd_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/newarp_DenseGenMatProd_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/newarp_DoubleShiftQR_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/newarp_DoubleShiftQR_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/newarp_DoubleShiftQR_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/newarp_DoubleShiftQR_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/newarp_EigsSelect.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/newarp_EigsSelect.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/newarp_GenEigsSolver_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/newarp_GenEigsSolver_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/newarp_GenEigsSolver_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/newarp_GenEigsSolver_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/newarp_SortEigenvalue.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/newarp_SortEigenvalue.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/newarp_SparseGenMatProd_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/newarp_SparseGenMatProd_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/newarp_SparseGenMatProd_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/newarp_SparseGenMatProd_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/newarp_SymEigsSolver_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/newarp_SymEigsSolver_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/newarp_SymEigsSolver_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/newarp_SymEigsSolver_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/newarp_TridiagEigen_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/newarp_TridiagEigen_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/newarp_TridiagEigen_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/newarp_TridiagEigen_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/newarp_UpperHessenbergEigen_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/newarp_UpperHessenbergEigen_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/newarp_UpperHessenbergEigen_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/newarp_UpperHessenbergEigen_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/newarp_UpperHessenbergQR_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/newarp_UpperHessenbergQR_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/newarp_UpperHessenbergQR_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/newarp_UpperHessenbergQR_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/newarp_cx_attrib.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/newarp_cx_attrib.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_all_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_all_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_all_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_all_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_any_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_any_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_any_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_any_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_chi2rnd_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_chi2rnd_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_chi2rnd_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_chi2rnd_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_chol_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_chol_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_chol_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_chol_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_clamp_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_clamp_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_clamp_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_clamp_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_cond_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_cond_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_cond_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_cond_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_cor_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_cor_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_cor_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_cor_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_cov_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_cov_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_cov_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_cov_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_cumprod_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_cumprod_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_cumprod_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_cumprod_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_cumsum_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_cumsum_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_cumsum_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_cumsum_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_cx_scalar_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_cx_scalar_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_cx_scalar_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_cx_scalar_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_diagmat_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_diagmat_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_diagmat_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_diagmat_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_diagvec_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_diagvec_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_diagvec_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_diagvec_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_diff_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_diff_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_diff_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_diff_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_dot_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_dot_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_dot_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_dot_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_dotext_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_dotext_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_dotext_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_dotext_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_expmat_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_expmat_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_expmat_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_expmat_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_fft_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_fft_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_fft_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_fft_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_find_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_find_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_find_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_find_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_find_unique_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_find_unique_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_find_unique_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_find_unique_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_flip_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_flip_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_flip_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_flip_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_hist_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_hist_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_hist_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_hist_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_htrans_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_htrans_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_htrans_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_htrans_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_index_max_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_index_max_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_index_max_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_index_max_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_index_min_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_index_min_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_index_min_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_index_min_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_inv_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_inv_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_inv_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_inv_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_logmat_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_logmat_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_logmat_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_logmat_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_max_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_max_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_max_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_max_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_mean_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_mean_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_mean_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_mean_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_median_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_median_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_median_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_median_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_min_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_min_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_min_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_min_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_misc_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_misc_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_misc_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_misc_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_nonzeros_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_nonzeros_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_nonzeros_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_nonzeros_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_norm_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_norm_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_norm_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_norm_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_normalise_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_normalise_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_normalise_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_normalise_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_orth_null_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_orth_null_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_orth_null_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_orth_null_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_pinv_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_pinv_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_pinv_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_pinv_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_princomp_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_princomp_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_princomp_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_princomp_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_prod_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_prod_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_prod_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_prod_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_range_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_range_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_range_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_range_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_relational_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_relational_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_relational_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_relational_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_repelem_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_repelem_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_repelem_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_repelem_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_repmat_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_repmat_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_repmat_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_repmat_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_reshape_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_reshape_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_reshape_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_reshape_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_resize_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_resize_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_resize_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_resize_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_reverse_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_reverse_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_reverse_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_reverse_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_roots_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_roots_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_roots_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_roots_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_shift_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_shift_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_shift_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_shift_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_shuffle_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_shuffle_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_shuffle_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_shuffle_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_sort_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_sort_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_sort_index_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_sort_index_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_sort_index_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_sort_index_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_sort_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_sort_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_sp_minus_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_sp_minus_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_sp_minus_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_sp_minus_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_sp_plus_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_sp_plus_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_sp_plus_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_sp_plus_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_sqrtmat_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_sqrtmat_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_sqrtmat_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_sqrtmat_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_stddev_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_stddev_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_stddev_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_stddev_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_strans_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_strans_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_strans_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_strans_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_sum_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_sum_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_sum_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_sum_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_symmat_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_symmat_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_symmat_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_symmat_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_toeplitz_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_toeplitz_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_toeplitz_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_toeplitz_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_trimat_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_trimat_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_trimat_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_trimat_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_unique_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_unique_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_unique_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_unique_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_var_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_var_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_var_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_var_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_vectorise_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_vectorise_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_vectorise_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_vectorise_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_wishrnd_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_wishrnd_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/op_wishrnd_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/op_wishrnd_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/operator_cube_div.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/operator_cube_div.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/operator_cube_minus.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/operator_cube_minus.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/operator_cube_plus.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/operator_cube_plus.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/operator_cube_relational.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/operator_cube_relational.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/operator_cube_schur.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/operator_cube_schur.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/operator_cube_times.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/operator_cube_times.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/operator_div.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/operator_div.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/operator_minus.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/operator_minus.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/operator_ostream.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/operator_ostream.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/operator_plus.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/operator_plus.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/operator_relational.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/operator_relational.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/operator_schur.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/operator_schur.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/operator_times.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/operator_times.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/podarray_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/podarray_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/podarray_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/podarray_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/promote_type.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/promote_type.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/restrictors.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/restrictors.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/running_stat_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/running_stat_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/running_stat_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/running_stat_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/running_stat_vec_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/running_stat_vec_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/running_stat_vec_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/running_stat_vec_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/sp_auxlib_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/sp_auxlib_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/sp_auxlib_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/sp_auxlib_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/span.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/span.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/spdiagview_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/spdiagview_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/spdiagview_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/spdiagview_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/spglue_elem_helper_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/spglue_elem_helper_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/spglue_elem_helper_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/spglue_elem_helper_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/spglue_join_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/spglue_join_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/spglue_join_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/spglue_join_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/spglue_kron_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/spglue_kron_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/spglue_kron_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/spglue_kron_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/spglue_max_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/spglue_max_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/spglue_max_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/spglue_max_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/spglue_merge_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/spglue_merge_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/spglue_merge_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/spglue_merge_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/spglue_min_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/spglue_min_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/spglue_min_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/spglue_min_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/spglue_minus_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/spglue_minus_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/spglue_minus_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/spglue_minus_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/spglue_plus_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/spglue_plus_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/spglue_plus_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/spglue_plus_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/spglue_relational_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/spglue_relational_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/spglue_relational_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/spglue_relational_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/spglue_schur_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/spglue_schur_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/spglue_schur_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/spglue_schur_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/spglue_times_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/spglue_times_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/spglue_times_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/spglue_times_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/spop_diagmat_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/spop_diagmat_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/spop_diagmat_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/spop_diagmat_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/spop_htrans_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/spop_htrans_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/spop_htrans_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/spop_htrans_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/spop_max_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/spop_max_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/spop_max_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/spop_max_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/spop_mean_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/spop_mean_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/spop_mean_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/spop_mean_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/spop_min_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/spop_min_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/spop_min_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/spop_min_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/spop_misc_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/spop_misc_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/spop_misc_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/spop_misc_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/spop_normalise_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/spop_normalise_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/spop_normalise_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/spop_normalise_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/spop_repmat_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/spop_repmat_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/spop_repmat_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/spop_repmat_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/spop_reverse_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/spop_reverse_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/spop_reverse_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/spop_reverse_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/spop_strans_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/spop_strans_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/spop_strans_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/spop_strans_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/spop_sum_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/spop_sum_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/spop_sum_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/spop_sum_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/spop_symmat_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/spop_symmat_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/spop_symmat_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/spop_symmat_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/spop_trimat_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/spop_trimat_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/spop_trimat_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/spop_trimat_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/spop_var_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/spop_var_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/spop_var_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/spop_var_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/spop_vectorise_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/spop_vectorise_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/spop_vectorise_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/spop_vectorise_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/strip.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/strip.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/subview_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/subview_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/subview_cube_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/subview_cube_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/subview_cube_each_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/subview_cube_each_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/subview_cube_each_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/subview_cube_each_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/subview_cube_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/subview_cube_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/subview_cube_slices_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/subview_cube_slices_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/subview_cube_slices_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/subview_cube_slices_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/subview_each_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/subview_each_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/subview_each_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/subview_each_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/subview_elem1_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/subview_elem1_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/subview_elem1_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/subview_elem1_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/subview_elem2_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/subview_elem2_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/subview_elem2_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/subview_elem2_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/subview_field_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/subview_field_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/subview_field_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/subview_field_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/subview_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/subview_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/sympd_helper.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/sympd_helper.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/traits.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/traits.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/translate_arpack.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/translate_arpack.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/translate_atlas.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/translate_atlas.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/translate_blas.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/translate_blas.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/translate_lapack.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/translate_lapack.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/translate_superlu.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/translate_superlu.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/trimat_helper.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/trimat_helper.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/typedef_elem.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/typedef_elem.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/typedef_elem_check.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/typedef_elem_check.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/typedef_mat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/typedef_mat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/typedef_mat_fixed.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/typedef_mat_fixed.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/unwrap.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/unwrap.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/unwrap_cube.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/unwrap_cube.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/unwrap_spmat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/unwrap_spmat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/upgrade_val.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/upgrade_val.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/wall_clock_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/wall_clock_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/wall_clock_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/wall_clock_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/xtrans_mat_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/xtrans_mat_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/xtrans_mat_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/xtrans_mat_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/xvec_htrans_bones.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/xvec_htrans_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/armadillo_bits/xvec_htrans_meat.hpp` & `fdasrsf-2.4.2/src/armadillo_bits/xvec_htrans_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/bayesian.cpp` & `fdasrsf-2.4.2/src/bayesian.cpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/c8lib.c` & `fdasrsf-2.4.2/src/c8lib.c`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/c8lib.h` & `fdasrsf-2.4.2/src/c8lib.h`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/cbayesian.pyx` & `fdasrsf-2.4.2/src/cbayesian.pyx`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/cyarma.pxd` & `fdasrsf-2.4.2/src/cyarma.pxd`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/cyarma.pyx` & `fdasrsf-2.4.2/src/cyarma.pyx`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/dp_grid.c` & `fdasrsf-2.4.2/src/dp_grid.c`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/dp_grid.h` & `fdasrsf-2.4.2/src/dp_grid.h`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/dp_nbhd.c` & `fdasrsf-2.4.2/src/dp_nbhd.c`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/fpls_warp.pyx` & `fdasrsf-2.4.2/src/fpls_warp.pyx`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/fpls_warp_grad.c` & `fdasrsf-2.4.2/src/fpls_warp_grad.c`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/imagecpp.pyx` & `fdasrsf-2.4.2/src/imagecpp.pyx`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/matrix_exponential.c` & `fdasrsf-2.4.2/src/matrix_exponential.c`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/misc_funcs.c` & `fdasrsf-2.4.2/src/misc_funcs.c`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/misc_funcs.h` & `fdasrsf-2.4.2/src/misc_funcs.h`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/mlogit_warp.pyx` & `fdasrsf-2.4.2/src/mlogit_warp.pyx`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/mlogit_warp_grad.c` & `fdasrsf-2.4.2/src/mlogit_warp_grad.c`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/myVector.cpp` & `fdasrsf-2.4.2/src/myVector.cpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/oclogit_warp.pyx` & `fdasrsf-2.4.2/src/oclogit_warp.pyx`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/oclogit_warp_grad.c` & `fdasrsf-2.4.2/src/oclogit_warp_grad.c`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/ocmlogit_warp.pyx` & `fdasrsf-2.4.2/src/ocmlogit_warp.pyx`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/ocmlogit_warp_grad.c` & `fdasrsf-2.4.2/src/ocmlogit_warp_grad.c`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/optimum_reparamN2.pyx` & `fdasrsf-2.4.2/src/optimum_reparamN2.pyx`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/optimum_reparam_N.pyx` & `fdasrsf-2.4.2/src/optimum_reparam_N.pyx`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/r8lib.c` & `fdasrsf-2.4.2/src/r8lib.c`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/src/r8lib.h` & `fdasrsf-2.4.2/src/r8lib.h`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.4.1/test/test_all.py` & `fdasrsf-2.4.2/test/test_all.py`

 * *Files identical despite different names*

