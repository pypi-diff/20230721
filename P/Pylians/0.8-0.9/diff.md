# Comparing `tmp/Pylians-0.8.tar.gz` & `tmp/Pylians-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pylians-0.8.tar", last modified: Fri Jul 21 15:14:11 2023, max compression
+gzip compressed data, was "Pylians-0.9.tar", last modified: Fri Jul 21 15:24:15 2023, max compression
```

## Comparing `Pylians-0.8.tar` & `Pylians-0.9.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 fvillaescusa   (503) staff       (20)        0 2023-07-21 15:14:11.354364 Pylians-0.8/
--rw-r--r--   0 fvillaescusa   (503) staff       (20)     1086 2020-11-14 18:25:56.000000 Pylians-0.8/LICENSE
--rw-r--r--   0 fvillaescusa   (503) staff       (20)     1393 2023-07-21 15:14:11.353741 Pylians-0.8/PKG-INFO
--rw-r--r--   0 fvillaescusa   (503) staff       (20)     1036 2022-08-31 14:07:54.000000 Pylians-0.8/README.md
-drwxr-xr-x   0 fvillaescusa   (503) staff       (20)        0 2023-07-21 15:14:11.302024 Pylians-0.8/library/
--rw-r--r--   0 fvillaescusa   (503) staff       (20)     5512 2022-02-15 13:27:25.000000 Pylians-0.8/library/CAMB_library.py
-drwxr-xr-x   0 fvillaescusa   (503) staff       (20)        0 2023-07-21 15:14:11.304260 Pylians-0.8/library/HI_clusters_library/
--rw-r--r--   0 fvillaescusa   (503) staff       (20)   903511 2023-07-21 15:13:59.000000 Pylians-0.8/library/HI_clusters_library/HI_clusters_library.c
--rw-r--r--   0 fvillaescusa   (503) staff       (20)       67 2020-11-14 18:25:56.000000 Pylians-0.8/library/HI_clusters_library/__init__.py
-drwxr-xr-x   0 fvillaescusa   (503) staff       (20)        0 2023-07-21 15:14:11.305454 Pylians-0.8/library/HI_image_library/
--rw-r--r--   0 fvillaescusa   (503) staff       (20)    17718 2023-07-21 15:07:33.000000 Pylians-0.8/library/HI_image_library/HI_image_library.py
--rw-r--r--   0 fvillaescusa   (503) staff       (20)       61 2020-11-14 18:25:56.000000 Pylians-0.8/library/HI_image_library/__init__.py
-drwxr-xr-x   0 fvillaescusa   (503) staff       (20)        0 2023-07-21 15:14:11.308106 Pylians-0.8/library/HI_library/
--rw-r--r--   0 fvillaescusa   (503) staff       (20)  1557988 2023-07-21 15:14:01.000000 Pylians-0.8/library/HI_library/HI_library.c
--rw-r--r--   0 fvillaescusa   (503) staff       (20)       49 2020-11-14 18:25:56.000000 Pylians-0.8/library/HI_library/__init__.py
--rw-r--r--   0 fvillaescusa   (503) staff       (20)    18270 2020-11-14 18:25:56.000000 Pylians-0.8/library/HOD_library.py
--rw-r--r--   0 fvillaescusa   (503) staff       (20)    53303 2020-11-14 18:25:56.000000 Pylians-0.8/library/IM_library.py
-drwxr-xr-x   0 fvillaescusa   (503) staff       (20)        0 2023-07-21 15:14:11.312565 Pylians-0.8/library/MAS_library/
--rw-r--r--   0 fvillaescusa   (503) staff       (20)     5864 2020-11-14 18:25:56.000000 Pylians-0.8/library/MAS_library/MAS_c.c
--rw-r--r--   0 fvillaescusa   (503) staff       (20)     3107 2020-11-14 18:25:56.000000 Pylians-0.8/library/MAS_library/MAS_gadget.py
--rw-r--r--   0 fvillaescusa   (503) staff       (20)  1712039 2023-07-21 15:14:02.000000 Pylians-0.8/library/MAS_library/MAS_library.c
--rw-r--r--   0 fvillaescusa   (503) staff       (20)      143 2020-11-14 18:25:56.000000 Pylians-0.8/library/MAS_library/__init__.py
--rw-r--r--   0 fvillaescusa   (503) staff       (20)   985372 2023-07-21 15:14:03.000000 Pylians-0.8/library/MAS_library/field_properties.c
-drwxr-xr-x   0 fvillaescusa   (503) staff       (20)        0 2023-07-21 15:14:11.320937 Pylians-0.8/library/Pk_library/
--rw-r--r--   0 fvillaescusa   (503) staff       (20)  2955640 2023-07-21 15:14:04.000000 Pylians-0.8/library/Pk_library/Pk_library.c
--rw-r--r--   0 fvillaescusa   (503) staff       (20)    12012 2020-11-14 18:25:56.000000 Pylians-0.8/library/Pk_library/Pk_snapshot.py
--rw-r--r--   0 fvillaescusa   (503) staff       (20)      126 2020-11-14 18:25:56.000000 Pylians-0.8/library/Pk_library/__init__.py
--rw-r--r--   0 fvillaescusa   (503) staff       (20)  1153420 2023-07-21 15:14:05.000000 Pylians-0.8/library/Pk_library/bispectrum_library.c
-drwxr-xr-x   0 fvillaescusa   (503) staff       (20)        0 2023-07-21 15:14:11.326237 Pylians-0.8/library/Pylians.egg-info/
--rw-r--r--   0 fvillaescusa   (503) staff       (20)     1393 2023-07-21 15:14:11.000000 Pylians-0.8/library/Pylians.egg-info/PKG-INFO
--rw-r--r--   0 fvillaescusa   (503) staff       (20)     1912 2023-07-21 15:14:11.000000 Pylians-0.8/library/Pylians.egg-info/SOURCES.txt
--rw-r--r--   0 fvillaescusa   (503) staff       (20)        1 2023-07-21 15:14:11.000000 Pylians-0.8/library/Pylians.egg-info/dependency_links.txt
--rw-r--r--   0 fvillaescusa   (503) staff       (20)       93 2023-07-21 15:14:11.000000 Pylians-0.8/library/Pylians.egg-info/requires.txt
--rw-r--r--   0 fvillaescusa   (503) staff       (20)      448 2023-07-21 15:14:11.000000 Pylians-0.8/library/Pylians.egg-info/top_level.txt
--rw-r--r--   0 fvillaescusa   (503) staff       (20)     3115 2020-11-14 18:25:56.000000 Pylians-0.8/library/bias_library.py
--rw-r--r--   0 fvillaescusa   (503) staff       (20)    40062 2020-11-14 18:25:56.000000 Pylians-0.8/library/correlation_function_library.py
--rw-r--r--   0 fvillaescusa   (503) staff       (20)     8188 2020-11-14 18:25:56.000000 Pylians-0.8/library/cosmology_library.py
-drwxr-xr-x   0 fvillaescusa   (503) staff       (20)        0 2023-07-21 15:14:11.327590 Pylians-0.8/library/density_field_library/
--rw-r--r--   0 fvillaescusa   (503) staff       (20)       71 2020-11-14 18:25:56.000000 Pylians-0.8/library/density_field_library/__init__.py
--rw-r--r--   0 fvillaescusa   (503) staff       (20)  1253424 2023-07-21 15:14:06.000000 Pylians-0.8/library/density_field_library/density_field_library.c
-drwxr-xr-x   0 fvillaescusa   (503) staff       (20)        0 2023-07-21 15:14:11.338322 Pylians-0.8/library/integration_library/
--rw-r--r--   0 fvillaescusa   (503) staff       (20)       67 2020-11-14 18:25:56.000000 Pylians-0.8/library/integration_library/__init__.py
--rw-r--r--   0 fvillaescusa   (503) staff       (20)      398 2020-11-14 18:25:56.000000 Pylians-0.8/library/integration_library/integral.py
--rw-r--r--   0 fvillaescusa   (503) staff       (20)     1580 2020-11-14 18:25:56.000000 Pylians-0.8/library/integration_library/integration.c
--rw-r--r--   0 fvillaescusa   (503) staff       (20)   971802 2023-07-21 15:14:07.000000 Pylians-0.8/library/integration_library/integration_library.c
--rw-r--r--   0 fvillaescusa   (503) staff       (20)    10626 2020-11-14 18:25:56.000000 Pylians-0.8/library/integration_library/runge_kutta.c
--rw-r--r--   0 fvillaescusa   (503) staff       (20)      411 2020-11-14 18:25:56.000000 Pylians-0.8/library/integration_library/setup.py
--rw-r--r--   0 fvillaescusa   (503) staff       (20)    22246 2021-03-22 14:02:07.000000 Pylians-0.8/library/mass_function_library.py
--rw-r--r--   0 fvillaescusa   (503) staff       (20)     5764 2020-11-14 18:25:56.000000 Pylians-0.8/library/plotting_library.py
--rw-r--r--   0 fvillaescusa   (503) staff       (20)     8238 2020-11-14 18:25:56.000000 Pylians-0.8/library/readfof.py
--rw-r--r--   0 fvillaescusa   (503) staff       (20)     6637 2023-07-21 15:07:33.000000 Pylians-0.8/library/readgadget.py
--rw-r--r--   0 fvillaescusa   (503) staff       (20)    14264 2020-11-14 18:25:56.000000 Pylians-0.8/library/readsnap.py
--rw-r--r--   0 fvillaescusa   (503) staff       (20)    11617 2020-11-14 18:25:56.000000 Pylians-0.8/library/readsnap2.py
--rw-r--r--   0 fvillaescusa   (503) staff       (20)    15640 2021-03-22 13:39:43.000000 Pylians-0.8/library/readsnapHDF5.py
--rw-r--r--   0 fvillaescusa   (503) staff       (20)     4448 2020-11-14 18:25:56.000000 Pylians-0.8/library/readsnap_mpi.py
--rw-r--r--   0 fvillaescusa   (503) staff       (20)    11854 2020-11-14 18:25:56.000000 Pylians-0.8/library/readsubf.py
-drwxr-xr-x   0 fvillaescusa   (503) staff       (20)        0 2023-07-21 15:14:11.339939 Pylians-0.8/library/redshift_space_library/
--rw-r--r--   0 fvillaescusa   (503) staff       (20)       73 2020-11-14 18:25:56.000000 Pylians-0.8/library/redshift_space_library/__init__.py
--rw-r--r--   0 fvillaescusa   (503) staff       (20)   840030 2023-07-21 15:14:08.000000 Pylians-0.8/library/redshift_space_library/redshift_space_library.c
--rw-r--r--   0 fvillaescusa   (503) staff       (20)    21969 2020-11-14 18:25:56.000000 Pylians-0.8/library/routines.py
-drwxr-xr-x   0 fvillaescusa   (503) staff       (20)        0 2023-07-21 15:14:11.343160 Pylians-0.8/library/smoothing_library/
--rw-r--r--   0 fvillaescusa   (503) staff       (20)       65 2020-11-14 18:25:56.000000 Pylians-0.8/library/smoothing_library/__init__.py
--rw-r--r--   0 fvillaescusa   (503) staff       (20)  1033120 2023-07-21 15:14:09.000000 Pylians-0.8/library/smoothing_library/smoothing_library.c
-drwxr-xr-x   0 fvillaescusa   (503) staff       (20)        0 2023-07-21 15:14:11.347142 Pylians-0.8/library/sorting_library/
--rw-r--r--   0 fvillaescusa   (503) staff       (20)       59 2020-11-14 18:25:56.000000 Pylians-0.8/library/sorting_library/__init__.py
--rw-r--r--   0 fvillaescusa   (503) staff       (20)  1019293 2023-07-21 15:14:10.000000 Pylians-0.8/library/sorting_library/sorting_library.c
--rw-r--r--   0 fvillaescusa   (503) staff       (20)      767 2020-11-14 18:25:56.000000 Pylians-0.8/library/units_library.py
-drwxr-xr-x   0 fvillaescusa   (503) staff       (20)        0 2023-07-21 15:14:11.352877 Pylians-0.8/library/void_library/
--rw-r--r--   0 fvillaescusa   (503) staff       (20)       56 2020-11-14 18:25:56.000000 Pylians-0.8/library/void_library/__init__.py
--rw-r--r--   0 fvillaescusa   (503) staff       (20)  1192954 2023-07-21 15:14:11.000000 Pylians-0.8/library/void_library/void_library.c
--rw-r--r--   0 fvillaescusa   (503) staff       (20)     3266 2020-11-14 18:25:56.000000 Pylians-0.8/library/void_library/void_openmp_library.c
--rw-r--r--   0 fvillaescusa   (503) staff       (20)      128 2023-07-21 15:09:36.000000 Pylians-0.8/pyproject.toml
--rw-r--r--   0 fvillaescusa   (503) staff       (20)       38 2023-07-21 15:14:11.354503 Pylians-0.8/setup.cfg
--rw-r--r--   0 fvillaescusa   (503) staff       (20)     4207 2023-07-21 15:12:24.000000 Pylians-0.8/setup.py
+drwxr-xr-x   0 fvillaescusa   (503) staff       (20)        0 2023-07-21 15:24:15.486664 Pylians-0.9/
+-rw-r--r--   0 fvillaescusa   (503) staff       (20)     1086 2020-11-14 18:25:56.000000 Pylians-0.9/LICENSE
+-rw-r--r--   0 fvillaescusa   (503) staff       (20)     1393 2023-07-21 15:24:15.486240 Pylians-0.9/PKG-INFO
+-rw-r--r--   0 fvillaescusa   (503) staff       (20)     1036 2022-08-31 14:07:54.000000 Pylians-0.9/README.md
+drwxr-xr-x   0 fvillaescusa   (503) staff       (20)        0 2023-07-21 15:24:15.429586 Pylians-0.9/library/
+-rw-r--r--   0 fvillaescusa   (503) staff       (20)     5512 2022-02-15 13:27:25.000000 Pylians-0.9/library/CAMB_library.py
+drwxr-xr-x   0 fvillaescusa   (503) staff       (20)        0 2023-07-21 15:24:15.432157 Pylians-0.9/library/HI_clusters_library/
+-rw-r--r--   0 fvillaescusa   (503) staff       (20)   903511 2023-07-21 15:13:59.000000 Pylians-0.9/library/HI_clusters_library/HI_clusters_library.c
+-rw-r--r--   0 fvillaescusa   (503) staff       (20)       67 2020-11-14 18:25:56.000000 Pylians-0.9/library/HI_clusters_library/__init__.py
+drwxr-xr-x   0 fvillaescusa   (503) staff       (20)        0 2023-07-21 15:24:15.433555 Pylians-0.9/library/HI_image_library/
+-rw-r--r--   0 fvillaescusa   (503) staff       (20)    17718 2023-07-21 15:07:33.000000 Pylians-0.9/library/HI_image_library/HI_image_library.py
+-rw-r--r--   0 fvillaescusa   (503) staff       (20)       61 2020-11-14 18:25:56.000000 Pylians-0.9/library/HI_image_library/__init__.py
+drwxr-xr-x   0 fvillaescusa   (503) staff       (20)        0 2023-07-21 15:24:15.437447 Pylians-0.9/library/HI_library/
+-rw-r--r--   0 fvillaescusa   (503) staff       (20)  1557988 2023-07-21 15:14:01.000000 Pylians-0.9/library/HI_library/HI_library.c
+-rw-r--r--   0 fvillaescusa   (503) staff       (20)       49 2020-11-14 18:25:56.000000 Pylians-0.9/library/HI_library/__init__.py
+-rw-r--r--   0 fvillaescusa   (503) staff       (20)    18270 2020-11-14 18:25:56.000000 Pylians-0.9/library/HOD_library.py
+-rw-r--r--   0 fvillaescusa   (503) staff       (20)    53303 2020-11-14 18:25:56.000000 Pylians-0.9/library/IM_library.py
+drwxr-xr-x   0 fvillaescusa   (503) staff       (20)        0 2023-07-21 15:24:15.444486 Pylians-0.9/library/MAS_library/
+-rw-r--r--   0 fvillaescusa   (503) staff       (20)     5864 2020-11-14 18:25:56.000000 Pylians-0.9/library/MAS_library/MAS_c.c
+-rw-r--r--   0 fvillaescusa   (503) staff       (20)     3107 2020-11-14 18:25:56.000000 Pylians-0.9/library/MAS_library/MAS_gadget.py
+-rw-r--r--   0 fvillaescusa   (503) staff       (20)  1712039 2023-07-21 15:14:02.000000 Pylians-0.9/library/MAS_library/MAS_library.c
+-rw-r--r--   0 fvillaescusa   (503) staff       (20)      143 2020-11-14 18:25:56.000000 Pylians-0.9/library/MAS_library/__init__.py
+-rw-r--r--   0 fvillaescusa   (503) staff       (20)   985372 2023-07-21 15:14:03.000000 Pylians-0.9/library/MAS_library/field_properties.c
+drwxr-xr-x   0 fvillaescusa   (503) staff       (20)        0 2023-07-21 15:24:15.455893 Pylians-0.9/library/Pk_library/
+-rw-r--r--   0 fvillaescusa   (503) staff       (20)  2955640 2023-07-21 15:14:04.000000 Pylians-0.9/library/Pk_library/Pk_library.c
+-rw-r--r--   0 fvillaescusa   (503) staff       (20)    12012 2020-11-14 18:25:56.000000 Pylians-0.9/library/Pk_library/Pk_snapshot.py
+-rw-r--r--   0 fvillaescusa   (503) staff       (20)      126 2020-11-14 18:25:56.000000 Pylians-0.9/library/Pk_library/__init__.py
+-rw-r--r--   0 fvillaescusa   (503) staff       (20)  1153420 2023-07-21 15:14:05.000000 Pylians-0.9/library/Pk_library/bispectrum_library.c
+drwxr-xr-x   0 fvillaescusa   (503) staff       (20)        0 2023-07-21 15:24:15.461379 Pylians-0.9/library/Pylians.egg-info/
+-rw-r--r--   0 fvillaescusa   (503) staff       (20)     1393 2023-07-21 15:24:15.000000 Pylians-0.9/library/Pylians.egg-info/PKG-INFO
+-rw-r--r--   0 fvillaescusa   (503) staff       (20)     1912 2023-07-21 15:24:15.000000 Pylians-0.9/library/Pylians.egg-info/SOURCES.txt
+-rw-r--r--   0 fvillaescusa   (503) staff       (20)        1 2023-07-21 15:24:15.000000 Pylians-0.9/library/Pylians.egg-info/dependency_links.txt
+-rw-r--r--   0 fvillaescusa   (503) staff       (20)      106 2023-07-21 15:24:15.000000 Pylians-0.9/library/Pylians.egg-info/requires.txt
+-rw-r--r--   0 fvillaescusa   (503) staff       (20)      448 2023-07-21 15:24:15.000000 Pylians-0.9/library/Pylians.egg-info/top_level.txt
+-rw-r--r--   0 fvillaescusa   (503) staff       (20)     3115 2020-11-14 18:25:56.000000 Pylians-0.9/library/bias_library.py
+-rw-r--r--   0 fvillaescusa   (503) staff       (20)    40062 2020-11-14 18:25:56.000000 Pylians-0.9/library/correlation_function_library.py
+-rw-r--r--   0 fvillaescusa   (503) staff       (20)     8188 2020-11-14 18:25:56.000000 Pylians-0.9/library/cosmology_library.py
+drwxr-xr-x   0 fvillaescusa   (503) staff       (20)        0 2023-07-21 15:24:15.462646 Pylians-0.9/library/density_field_library/
+-rw-r--r--   0 fvillaescusa   (503) staff       (20)       71 2020-11-14 18:25:56.000000 Pylians-0.9/library/density_field_library/__init__.py
+-rw-r--r--   0 fvillaescusa   (503) staff       (20)  1253424 2023-07-21 15:14:06.000000 Pylians-0.9/library/density_field_library/density_field_library.c
+drwxr-xr-x   0 fvillaescusa   (503) staff       (20)        0 2023-07-21 15:24:15.471326 Pylians-0.9/library/integration_library/
+-rw-r--r--   0 fvillaescusa   (503) staff       (20)       67 2020-11-14 18:25:56.000000 Pylians-0.9/library/integration_library/__init__.py
+-rw-r--r--   0 fvillaescusa   (503) staff       (20)      398 2020-11-14 18:25:56.000000 Pylians-0.9/library/integration_library/integral.py
+-rw-r--r--   0 fvillaescusa   (503) staff       (20)     1580 2020-11-14 18:25:56.000000 Pylians-0.9/library/integration_library/integration.c
+-rw-r--r--   0 fvillaescusa   (503) staff       (20)   971802 2023-07-21 15:14:07.000000 Pylians-0.9/library/integration_library/integration_library.c
+-rw-r--r--   0 fvillaescusa   (503) staff       (20)    10626 2020-11-14 18:25:56.000000 Pylians-0.9/library/integration_library/runge_kutta.c
+-rw-r--r--   0 fvillaescusa   (503) staff       (20)      411 2020-11-14 18:25:56.000000 Pylians-0.9/library/integration_library/setup.py
+-rw-r--r--   0 fvillaescusa   (503) staff       (20)    22246 2021-03-22 14:02:07.000000 Pylians-0.9/library/mass_function_library.py
+-rw-r--r--   0 fvillaescusa   (503) staff       (20)     5764 2020-11-14 18:25:56.000000 Pylians-0.9/library/plotting_library.py
+-rw-r--r--   0 fvillaescusa   (503) staff       (20)     8238 2020-11-14 18:25:56.000000 Pylians-0.9/library/readfof.py
+-rw-r--r--   0 fvillaescusa   (503) staff       (20)     6637 2023-07-21 15:07:33.000000 Pylians-0.9/library/readgadget.py
+-rw-r--r--   0 fvillaescusa   (503) staff       (20)    14264 2020-11-14 18:25:56.000000 Pylians-0.9/library/readsnap.py
+-rw-r--r--   0 fvillaescusa   (503) staff       (20)    11617 2020-11-14 18:25:56.000000 Pylians-0.9/library/readsnap2.py
+-rw-r--r--   0 fvillaescusa   (503) staff       (20)    15640 2021-03-22 13:39:43.000000 Pylians-0.9/library/readsnapHDF5.py
+-rw-r--r--   0 fvillaescusa   (503) staff       (20)     4448 2020-11-14 18:25:56.000000 Pylians-0.9/library/readsnap_mpi.py
+-rw-r--r--   0 fvillaescusa   (503) staff       (20)    11854 2020-11-14 18:25:56.000000 Pylians-0.9/library/readsubf.py
+drwxr-xr-x   0 fvillaescusa   (503) staff       (20)        0 2023-07-21 15:24:15.472668 Pylians-0.9/library/redshift_space_library/
+-rw-r--r--   0 fvillaescusa   (503) staff       (20)       73 2020-11-14 18:25:56.000000 Pylians-0.9/library/redshift_space_library/__init__.py
+-rw-r--r--   0 fvillaescusa   (503) staff       (20)   840030 2023-07-21 15:14:08.000000 Pylians-0.9/library/redshift_space_library/redshift_space_library.c
+-rw-r--r--   0 fvillaescusa   (503) staff       (20)    21969 2020-11-14 18:25:56.000000 Pylians-0.9/library/routines.py
+drwxr-xr-x   0 fvillaescusa   (503) staff       (20)        0 2023-07-21 15:24:15.475529 Pylians-0.9/library/smoothing_library/
+-rw-r--r--   0 fvillaescusa   (503) staff       (20)       65 2020-11-14 18:25:56.000000 Pylians-0.9/library/smoothing_library/__init__.py
+-rw-r--r--   0 fvillaescusa   (503) staff       (20)  1033120 2023-07-21 15:14:09.000000 Pylians-0.9/library/smoothing_library/smoothing_library.c
+drwxr-xr-x   0 fvillaescusa   (503) staff       (20)        0 2023-07-21 15:24:15.479079 Pylians-0.9/library/sorting_library/
+-rw-r--r--   0 fvillaescusa   (503) staff       (20)       59 2020-11-14 18:25:56.000000 Pylians-0.9/library/sorting_library/__init__.py
+-rw-r--r--   0 fvillaescusa   (503) staff       (20)  1019293 2023-07-21 15:14:10.000000 Pylians-0.9/library/sorting_library/sorting_library.c
+-rw-r--r--   0 fvillaescusa   (503) staff       (20)      767 2020-11-14 18:25:56.000000 Pylians-0.9/library/units_library.py
+drwxr-xr-x   0 fvillaescusa   (503) staff       (20)        0 2023-07-21 15:24:15.485503 Pylians-0.9/library/void_library/
+-rw-r--r--   0 fvillaescusa   (503) staff       (20)       56 2020-11-14 18:25:56.000000 Pylians-0.9/library/void_library/__init__.py
+-rw-r--r--   0 fvillaescusa   (503) staff       (20)  1192954 2023-07-21 15:14:11.000000 Pylians-0.9/library/void_library/void_library.c
+-rw-r--r--   0 fvillaescusa   (503) staff       (20)     3266 2020-11-14 18:25:56.000000 Pylians-0.9/library/void_library/void_openmp_library.c
+-rw-r--r--   0 fvillaescusa   (503) staff       (20)      128 2023-07-21 15:09:36.000000 Pylians-0.9/pyproject.toml
+-rw-r--r--   0 fvillaescusa   (503) staff       (20)       38 2023-07-21 15:24:15.486827 Pylians-0.9/setup.cfg
+-rw-r--r--   0 fvillaescusa   (503) staff       (20)     4231 2023-07-21 15:23:36.000000 Pylians-0.9/setup.py
```

### Comparing `Pylians-0.8/LICENSE` & `Pylians-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `Pylians-0.8/PKG-INFO` & `Pylians-0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pylians
-Version: 0.8
+Version: 0.9
 Summary: Python libraries for the analysis of numerical simulations
 Home-page: https://github.com/franciscovillaescusa/Pylians3
 Author: Francisco Villaescusa-Navarro
 Author-email: villaescusa.francisco@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `Pylians-0.8/README.md` & `Pylians-0.9/README.md`

 * *Files identical despite different names*

### Comparing `Pylians-0.8/library/CAMB_library.py` & `Pylians-0.9/library/CAMB_library.py`

 * *Files identical despite different names*

### Comparing `Pylians-0.8/library/HI_clusters_library/HI_clusters_library.c` & `Pylians-0.9/library/HI_clusters_library/HI_clusters_library.c`

 * *Files identical despite different names*

### Comparing `Pylians-0.8/library/HI_image_library/HI_image_library.py` & `Pylians-0.9/library/HI_image_library/HI_image_library.py`

 * *Files identical despite different names*

### Comparing `Pylians-0.8/library/HI_library/HI_library.c` & `Pylians-0.9/library/HI_library/HI_library.c`

 * *Files identical despite different names*

### Comparing `Pylians-0.8/library/HOD_library.py` & `Pylians-0.9/library/HOD_library.py`

 * *Files identical despite different names*

### Comparing `Pylians-0.8/library/IM_library.py` & `Pylians-0.9/library/IM_library.py`

 * *Files identical despite different names*

### Comparing `Pylians-0.8/library/MAS_library/MAS_c.c` & `Pylians-0.9/library/MAS_library/MAS_c.c`

 * *Files identical despite different names*

### Comparing `Pylians-0.8/library/MAS_library/MAS_gadget.py` & `Pylians-0.9/library/MAS_library/MAS_gadget.py`

 * *Files identical despite different names*

### Comparing `Pylians-0.8/library/MAS_library/MAS_library.c` & `Pylians-0.9/library/MAS_library/MAS_library.c`

 * *Files identical despite different names*

### Comparing `Pylians-0.8/library/MAS_library/field_properties.c` & `Pylians-0.9/library/MAS_library/field_properties.c`

 * *Files identical despite different names*

### Comparing `Pylians-0.8/library/Pk_library/Pk_library.c` & `Pylians-0.9/library/Pk_library/Pk_library.c`

 * *Files identical despite different names*

### Comparing `Pylians-0.8/library/Pk_library/Pk_snapshot.py` & `Pylians-0.9/library/Pk_library/Pk_snapshot.py`

 * *Files identical despite different names*

### Comparing `Pylians-0.8/library/Pk_library/bispectrum_library.c` & `Pylians-0.9/library/Pk_library/bispectrum_library.c`

 * *Files identical despite different names*

### Comparing `Pylians-0.8/library/Pylians.egg-info/PKG-INFO` & `Pylians-0.9/library/Pylians.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pylians
-Version: 0.8
+Version: 0.9
 Summary: Python libraries for the analysis of numerical simulations
 Home-page: https://github.com/franciscovillaescusa/Pylians3
 Author: Francisco Villaescusa-Navarro
 Author-email: villaescusa.francisco@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `Pylians-0.8/library/Pylians.egg-info/SOURCES.txt` & `Pylians-0.9/library/Pylians.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Pylians-0.8/library/bias_library.py` & `Pylians-0.9/library/bias_library.py`

 * *Files identical despite different names*

### Comparing `Pylians-0.8/library/correlation_function_library.py` & `Pylians-0.9/library/correlation_function_library.py`

 * *Files identical despite different names*

### Comparing `Pylians-0.8/library/cosmology_library.py` & `Pylians-0.9/library/cosmology_library.py`

 * *Files identical despite different names*

### Comparing `Pylians-0.8/library/density_field_library/density_field_library.c` & `Pylians-0.9/library/density_field_library/density_field_library.c`

 * *Files identical despite different names*

### Comparing `Pylians-0.8/library/integration_library/integration.c` & `Pylians-0.9/library/integration_library/integration.c`

 * *Files identical despite different names*

### Comparing `Pylians-0.8/library/integration_library/integration_library.c` & `Pylians-0.9/library/integration_library/integration_library.c`

 * *Files identical despite different names*

### Comparing `Pylians-0.8/library/integration_library/runge_kutta.c` & `Pylians-0.9/library/integration_library/runge_kutta.c`

 * *Files identical despite different names*

### Comparing `Pylians-0.8/library/mass_function_library.py` & `Pylians-0.9/library/mass_function_library.py`

 * *Files identical despite different names*

### Comparing `Pylians-0.8/library/plotting_library.py` & `Pylians-0.9/library/plotting_library.py`

 * *Files identical despite different names*

### Comparing `Pylians-0.8/library/readfof.py` & `Pylians-0.9/library/readfof.py`

 * *Files identical despite different names*

### Comparing `Pylians-0.8/library/readgadget.py` & `Pylians-0.9/library/readgadget.py`

 * *Files identical despite different names*

### Comparing `Pylians-0.8/library/readsnap.py` & `Pylians-0.9/library/readsnap.py`

 * *Files identical despite different names*

### Comparing `Pylians-0.8/library/readsnap2.py` & `Pylians-0.9/library/readsnap2.py`

 * *Files identical despite different names*

### Comparing `Pylians-0.8/library/readsnapHDF5.py` & `Pylians-0.9/library/readsnapHDF5.py`

 * *Files identical despite different names*

### Comparing `Pylians-0.8/library/readsnap_mpi.py` & `Pylians-0.9/library/readsnap_mpi.py`

 * *Files identical despite different names*

### Comparing `Pylians-0.8/library/readsubf.py` & `Pylians-0.9/library/readsubf.py`

 * *Files identical despite different names*

### Comparing `Pylians-0.8/library/redshift_space_library/redshift_space_library.c` & `Pylians-0.9/library/redshift_space_library/redshift_space_library.c`

 * *Files identical despite different names*

### Comparing `Pylians-0.8/library/routines.py` & `Pylians-0.9/library/routines.py`

 * *Files identical despite different names*

### Comparing `Pylians-0.8/library/smoothing_library/smoothing_library.c` & `Pylians-0.9/library/smoothing_library/smoothing_library.c`

 * *Files identical despite different names*

### Comparing `Pylians-0.8/library/sorting_library/sorting_library.c` & `Pylians-0.9/library/sorting_library/sorting_library.c`

 * *Files identical despite different names*

### Comparing `Pylians-0.8/library/units_library.py` & `Pylians-0.9/library/units_library.py`

 * *Files identical despite different names*

### Comparing `Pylians-0.8/library/void_library/void_library.c` & `Pylians-0.9/library/void_library/void_library.c`

 * *Files identical despite different names*

### Comparing `Pylians-0.8/library/void_library/void_openmp_library.c` & `Pylians-0.9/library/void_library/void_openmp_library.c`

 * *Files identical despite different names*

### Comparing `Pylians-0.8/setup.py` & `Pylians-0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 
 
 with open("README.md", "r") as f:
     documentation = f.read()
 
 setup(
     name="Pylians",
-    version="0.8",
+    version="0.9",
     author="Francisco Villaescusa-Navarro",
     author_email="villaescusa.francisco@gmail.com",
     description="Python libraries for the analysis of numerical simulations",
     url="https://github.com/franciscovillaescusa/Pylians3",
     license="MIT",
     long_description_content_type="text/markdown",
     long_description=documentation,
@@ -107,14 +107,15 @@
     ),
     include_dirs=[numpy.get_include()],
     install_requires=[
         "h5py",
         "pyfftw; platform_system!='Darwin' and platform_machine!='arm64'",
         "scipy",
         "hdf5plugin",
+        "Cython<3.0.0",
     ],
     package_dir={"": "library/"},
     py_modules=[
         "bias_library",
         "CAMB_library",
         "correlation_function_library",
         "cosmology_library",
```

