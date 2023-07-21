# Comparing `tmp/mapel-core-2.0.8.tar.gz` & `tmp/mapel-core-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapel-core-2.0.8.tar", last modified: Tue Jul 18 07:11:26 2023, max compression
+gzip compressed data, was "mapel-core-2.0.9.tar", last modified: Fri Jul 21 15:01:53 2023, max compression
```

## Comparing `mapel-core-2.0.8.tar` & `mapel-core-2.0.9.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:26.101167 mapel-core-2.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-18 07:11:08.000000 mapel-core-2.0.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-18 07:11:26.101167 mapel-core-2.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-18 07:11:08.000000 mapel-core-2.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-18 07:11:08.000000 mapel-core-2.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-18 07:11:08.000000 mapel-core-2.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 07:11:26.101167 mapel-core-2.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:26.097167 mapel-core-2.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:26.097167 mapel-core-2.0.8/src/mapel/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:26.097167 mapel-core-2.0.8/src/mapel/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:08.000000 mapel-core-2.0.8/src/mapel/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:26.097167 mapel-core-2.0.8/src/mapel/core/embedding/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:08.000000 mapel-core-2.0.8/src/mapel/core/embedding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-07-18 07:11:08.000000 mapel-core-2.0.8/src/mapel/core/embedding/embed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-07-18 07:11:08.000000 mapel-core-2.0.8/src/mapel/core/embedding/initial_positions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:26.097167 mapel-core-2.0.8/src/mapel/core/embedding/kamada_kawai/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:08.000000 mapel-core-2.0.8/src/mapel/core/embedding/kamada_kawai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-07-18 07:11:08.000000 mapel-core-2.0.8/src/mapel/core/embedding/kamada_kawai/energy_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-07-18 07:11:08.000000 mapel-core-2.0.8/src/mapel/core/embedding/kamada_kawai/kamada_kawai.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-07-18 07:11:08.000000 mapel-core-2.0.8/src/mapel/core/embedding/kamada_kawai/optimization_algorithms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:26.097167 mapel-core-2.0.8/src/mapel/core/embedding/simulated_annealing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:08.000000 mapel-core-2.0.8/src/mapel/core/embedding/simulated_annealing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-07-18 07:11:08.000000 mapel-core-2.0.8/src/mapel/core/embedding/simulated_annealing/simulated_annealing.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-18 07:11:08.000000 mapel-core-2.0.8/src/mapel/core/embedding/simulated_annealing/simulated_annealing_energy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:26.097167 mapel-core-2.0.8/src/mapel/core/features/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:08.000000 mapel-core-2.0.8/src/mapel/core/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-18 07:11:08.000000 mapel-core-2.0.8/src/mapel/core/features/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-07-18 07:11:08.000000 mapel-core-2.0.8/src/mapel/core/features/distortion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-07-18 07:11:08.000000 mapel-core-2.0.8/src/mapel/core/features/mallows.py
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-07-18 07:11:08.000000 mapel-core-2.0.8/src/mapel/core/features/monotonicity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-07-18 07:11:08.000000 mapel-core-2.0.8/src/mapel/core/features/stability.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-18 07:11:08.000000 mapel-core-2.0.8/src/mapel/core/features_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-07-18 07:11:08.000000 mapel-core-2.0.8/src/mapel/core/glossary.py
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-07-18 07:11:08.000000 mapel-core-2.0.8/src/mapel/core/inner_distances.py
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-07-18 07:11:08.000000 mapel-core-2.0.8/src/mapel/core/matchings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:26.097167 mapel-core-2.0.8/src/mapel/core/objects/
--rw-r--r--   0 runner    (1001) docker     (123)    16992 2023-07-18 07:11:08.000000 mapel-core-2.0.8/src/mapel/core/objects/Experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-18 07:11:08.000000 mapel-core-2.0.8/src/mapel/core/objects/Family.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-18 07:11:08.000000 mapel-core-2.0.8/src/mapel/core/objects/Instance.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:08.000000 mapel-core-2.0.8/src/mapel/core/objects/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:26.101167 mapel-core-2.0.8/src/mapel/core/persistence/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:08.000000 mapel-core-2.0.8/src/mapel/core/persistence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-07-18 07:11:08.000000 mapel-core-2.0.8/src/mapel/core/persistence/experiment_exports.py
--rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-07-18 07:11:08.000000 mapel-core-2.0.8/src/mapel/core/persistence/experiment_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)    62429 2023-07-18 07:11:08.000000 mapel-core-2.0.8/src/mapel/core/printing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-18 07:11:08.000000 mapel-core-2.0.8/src/mapel/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:26.101167 mapel-core-2.0.8/src/mapel_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-18 07:11:26.000000 mapel-core-2.0.8/src/mapel_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-18 07:11:26.000000 mapel-core-2.0.8/src/mapel_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 07:11:26.000000 mapel-core-2.0.8/src/mapel_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-18 07:11:26.000000 mapel-core-2.0.8/src/mapel_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-18 07:11:26.000000 mapel-core-2.0.8/src/mapel_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:01:53.321685 mapel-core-2.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-21 15:01:36.000000 mapel-core-2.0.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-21 15:01:53.321685 mapel-core-2.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-21 15:01:36.000000 mapel-core-2.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-21 15:01:36.000000 mapel-core-2.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-21 15:01:36.000000 mapel-core-2.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 15:01:53.321685 mapel-core-2.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:01:53.317685 mapel-core-2.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:01:53.317685 mapel-core-2.0.9/src/mapel/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:01:53.321685 mapel-core-2.0.9/src/mapel/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 15:01:36.000000 mapel-core-2.0.9/src/mapel/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:01:53.321685 mapel-core-2.0.9/src/mapel/core/embedding/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 15:01:36.000000 mapel-core-2.0.9/src/mapel/core/embedding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-07-21 15:01:36.000000 mapel-core-2.0.9/src/mapel/core/embedding/embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-07-21 15:01:36.000000 mapel-core-2.0.9/src/mapel/core/embedding/initial_positions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:01:53.321685 mapel-core-2.0.9/src/mapel/core/embedding/kamada_kawai/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 15:01:36.000000 mapel-core-2.0.9/src/mapel/core/embedding/kamada_kawai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-07-21 15:01:36.000000 mapel-core-2.0.9/src/mapel/core/embedding/kamada_kawai/energy_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-07-21 15:01:36.000000 mapel-core-2.0.9/src/mapel/core/embedding/kamada_kawai/kamada_kawai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-07-21 15:01:36.000000 mapel-core-2.0.9/src/mapel/core/embedding/kamada_kawai/optimization_algorithms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:01:53.321685 mapel-core-2.0.9/src/mapel/core/embedding/simulated_annealing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 15:01:36.000000 mapel-core-2.0.9/src/mapel/core/embedding/simulated_annealing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-07-21 15:01:36.000000 mapel-core-2.0.9/src/mapel/core/embedding/simulated_annealing/simulated_annealing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-21 15:01:36.000000 mapel-core-2.0.9/src/mapel/core/embedding/simulated_annealing/simulated_annealing_energy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:01:53.321685 mapel-core-2.0.9/src/mapel/core/features/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 15:01:36.000000 mapel-core-2.0.9/src/mapel/core/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-21 15:01:36.000000 mapel-core-2.0.9/src/mapel/core/features/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-07-21 15:01:36.000000 mapel-core-2.0.9/src/mapel/core/features/distortion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-07-21 15:01:36.000000 mapel-core-2.0.9/src/mapel/core/features/mallows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-07-21 15:01:36.000000 mapel-core-2.0.9/src/mapel/core/features/monotonicity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-07-21 15:01:36.000000 mapel-core-2.0.9/src/mapel/core/features/stability.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-21 15:01:36.000000 mapel-core-2.0.9/src/mapel/core/features_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-07-21 15:01:36.000000 mapel-core-2.0.9/src/mapel/core/glossary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-07-21 15:01:36.000000 mapel-core-2.0.9/src/mapel/core/inner_distances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-07-21 15:01:36.000000 mapel-core-2.0.9/src/mapel/core/matchings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:01:53.321685 mapel-core-2.0.9/src/mapel/core/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)    16992 2023-07-21 15:01:36.000000 mapel-core-2.0.9/src/mapel/core/objects/Experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-21 15:01:36.000000 mapel-core-2.0.9/src/mapel/core/objects/Family.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-21 15:01:36.000000 mapel-core-2.0.9/src/mapel/core/objects/Instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 15:01:36.000000 mapel-core-2.0.9/src/mapel/core/objects/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:01:53.321685 mapel-core-2.0.9/src/mapel/core/persistence/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 15:01:36.000000 mapel-core-2.0.9/src/mapel/core/persistence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-07-21 15:01:36.000000 mapel-core-2.0.9/src/mapel/core/persistence/experiment_exports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-07-21 15:01:36.000000 mapel-core-2.0.9/src/mapel/core/persistence/experiment_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62429 2023-07-21 15:01:36.000000 mapel-core-2.0.9/src/mapel/core/printing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-21 15:01:36.000000 mapel-core-2.0.9/src/mapel/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:01:53.321685 mapel-core-2.0.9/src/mapel_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-21 15:01:53.000000 mapel-core-2.0.9/src/mapel_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-21 15:01:53.000000 mapel-core-2.0.9/src/mapel_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 15:01:53.000000 mapel-core-2.0.9/src/mapel_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-21 15:01:53.000000 mapel-core-2.0.9/src/mapel_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-21 15:01:53.000000 mapel-core-2.0.9/src/mapel_core.egg-info/top_level.txt
```

### Comparing `mapel-core-2.0.8/LICENSE.txt` & `mapel-core-2.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.8/PKG-INFO` & `mapel-core-2.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapel-core
-Version: 2.0.8
+Version: 2.0.9
 Summary: Map of Elections---essential parts
 Author-email: Stanislaw Szufa <s.szufa@gmail.com>, Niclas Boehmer <niclas.boehmer@tu-berlin.de>, Andrzej Kaczmarczyk <andrzej.kaczmarczyk@agh.edu.pl>, Kasper Sapala <kasper.sapala@gmail.com>, Tomasz Was <tomasz.t.was@gmail.com>
 License: Copyright (c) 2018-2022 Stanisław Szufa and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `mapel-core-2.0.8/README.md` & `mapel-core-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.8/pyproject.toml` & `mapel-core-2.0.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65", "wheel", "pybind11>=2.6.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mapel-core"
-version = "2.0.8"
+version = "2.0.9"
 authors = [
  {name = "Stanislaw Szufa", email = "s.szufa@gmail.com"},
  {name = "Niclas Boehmer", email = "niclas.boehmer@tu-berlin.de"},
  {name = "Andrzej Kaczmarczyk", email = "andrzej.kaczmarczyk@agh.edu.pl"},
  {name = "Kasper Sapala", email = "kasper.sapala@gmail.com"},
  {name = "Tomasz Was", email = "tomasz.t.was@gmail.com"},
 ]
```

### Comparing `mapel-core-2.0.8/src/mapel/core/embedding/embed.py` & `mapel-core-2.0.9/src/mapel/core/embedding/embed.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.8/src/mapel/core/embedding/initial_positions.py` & `mapel-core-2.0.9/src/mapel/core/embedding/initial_positions.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.8/src/mapel/core/embedding/kamada_kawai/energy_functions.py` & `mapel-core-2.0.9/src/mapel/core/embedding/kamada_kawai/energy_functions.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.8/src/mapel/core/embedding/kamada_kawai/kamada_kawai.py` & `mapel-core-2.0.9/src/mapel/core/embedding/kamada_kawai/kamada_kawai.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.8/src/mapel/core/embedding/kamada_kawai/optimization_algorithms.py` & `mapel-core-2.0.9/src/mapel/core/embedding/kamada_kawai/optimization_algorithms.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.8/src/mapel/core/embedding/simulated_annealing/simulated_annealing.py` & `mapel-core-2.0.9/src/mapel/core/embedding/simulated_annealing/simulated_annealing.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.8/src/mapel/core/embedding/simulated_annealing/simulated_annealing_energy.py` & `mapel-core-2.0.9/src/mapel/core/embedding/simulated_annealing/simulated_annealing_energy.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.8/src/mapel/core/features/common.py` & `mapel-core-2.0.9/src/mapel/core/features/common.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.8/src/mapel/core/features/distortion.py` & `mapel-core-2.0.9/src/mapel/core/features/distortion.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.8/src/mapel/core/features/mallows.py` & `mapel-core-2.0.9/src/mapel/core/features/mallows.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.8/src/mapel/core/features/monotonicity.py` & `mapel-core-2.0.9/src/mapel/core/features/monotonicity.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.8/src/mapel/core/features/stability.py` & `mapel-core-2.0.9/src/mapel/core/features/stability.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.8/src/mapel/core/features_main.py` & `mapel-core-2.0.9/src/mapel/core/features_main.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.8/src/mapel/core/glossary.py` & `mapel-core-2.0.9/src/mapel/core/glossary.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.8/src/mapel/core/inner_distances.py` & `mapel-core-2.0.9/src/mapel/core/inner_distances.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.8/src/mapel/core/matchings.py` & `mapel-core-2.0.9/src/mapel/core/matchings.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.8/src/mapel/core/objects/Experiment.py` & `mapel-core-2.0.9/src/mapel/core/objects/Experiment.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.8/src/mapel/core/objects/Family.py` & `mapel-core-2.0.9/src/mapel/core/objects/Family.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.8/src/mapel/core/persistence/experiment_exports.py` & `mapel-core-2.0.9/src/mapel/core/persistence/experiment_exports.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.8/src/mapel/core/persistence/experiment_imports.py` & `mapel-core-2.0.9/src/mapel/core/persistence/experiment_imports.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.8/src/mapel/core/printing.py` & `mapel-core-2.0.9/src/mapel/core/printing.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.8/src/mapel/core/utils.py` & `mapel-core-2.0.9/src/mapel/core/utils.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.8/src/mapel_core.egg-info/PKG-INFO` & `mapel-core-2.0.9/src/mapel_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapel-core
-Version: 2.0.8
+Version: 2.0.9
 Summary: Map of Elections---essential parts
 Author-email: Stanislaw Szufa <s.szufa@gmail.com>, Niclas Boehmer <niclas.boehmer@tu-berlin.de>, Andrzej Kaczmarczyk <andrzej.kaczmarczyk@agh.edu.pl>, Kasper Sapala <kasper.sapala@gmail.com>, Tomasz Was <tomasz.t.was@gmail.com>
 License: Copyright (c) 2018-2022 Stanisław Szufa and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `mapel-core-2.0.8/src/mapel_core.egg-info/SOURCES.txt` & `mapel-core-2.0.9/src/mapel_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

