# Comparing `tmp/dwave-samplers-1.0.0.dev2.tar.gz` & `tmp/dwave-samplers-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dwave-samplers-1.0.0.dev2.tar", last modified: Mon Nov 14 21:57:29 2022, max compression
+gzip compressed data, was "dwave-samplers-1.1.0.tar", last modified: Fri Jul 21 20:07:21 2023, max compression
```

## Comparing `dwave-samplers-1.0.0.dev2.tar` & `dwave-samplers-1.1.0.tar`

### file list

```diff
@@ -1,93 +1,94 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-11-14 21:57:29.945268 dwave-samplers-1.0.0.dev2/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11386 2022-11-14 21:57:01.000000 dwave-samplers-1.0.0.dev2/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)       91 2022-11-14 21:57:01.000000 dwave-samplers-1.0.0.dev2/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9705 2022-11-14 21:57:29.945268 dwave-samplers-1.0.0.dev2/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8579 2022-11-14 21:57:01.000000 dwave-samplers-1.0.0.dev2/README.rst
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-11-14 21:57:29.929268 dwave-samplers-1.0.0.dev2/dwave/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-11-14 21:57:29.929268 dwave-samplers-1.0.0.dev2/dwave/samplers/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      823 2022-11-14 21:57:01.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-11-14 21:57:29.933267 dwave-samplers-1.0.0.dev2/dwave/samplers/greedy/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      749 2022-11-14 21:57:01.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/greedy/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2584 2022-11-14 21:57:01.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/greedy/composite.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1043 2022-11-14 21:57:01.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/greedy/decl.pxd
--rw-r--r--   0 circleci  (3434) circleci  (3434)   886191 2022-11-14 21:57:22.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/greedy/descent.cpp
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4365 2022-11-14 21:57:01.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/greedy/descent.pyx
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10848 2022-11-14 21:57:01.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/greedy/sampler.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-11-14 21:57:29.933267 dwave-samplers-1.0.0.dev2/dwave/samplers/greedy/src/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15644 2022-11-14 21:57:01.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/greedy/src/descent.cpp
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1808 2022-11-14 21:57:01.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/greedy/src/descent.h
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-11-14 21:57:29.933267 dwave-samplers-1.0.0.dev2/dwave/samplers/planar/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      624 2022-11-14 21:57:01.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/planar/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7276 2022-11-14 21:57:01.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/planar/planar.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4750 2022-11-14 21:57:01.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/planar/sampler.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1369 2022-11-14 21:57:01.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/planar/util.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-11-14 21:57:29.933267 dwave-samplers-1.0.0.dev2/dwave/samplers/random/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      655 2022-11-14 21:57:01.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/random/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)   945516 2022-11-14 21:57:23.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/random/cyrandom.cpp
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5545 2022-11-14 21:57:01.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/random/cyrandom.pyx
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5072 2022-11-14 21:57:01.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/random/sampler.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-11-14 21:57:29.933267 dwave-samplers-1.0.0.dev2/dwave/samplers/sa/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      684 2022-11-14 21:57:01.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/sa/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    24600 2022-11-14 21:57:01.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/sa/sampler.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)   909372 2022-11-14 21:57:24.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/sa/simulated_annealing.cpp
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6041 2022-11-14 21:57:01.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/sa/simulated_annealing.pyx
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-11-14 21:57:29.937267 dwave-samplers-1.0.0.dev2/dwave/samplers/sa/src/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13963 2022-11-14 21:57:01.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/sa/src/cpu_sa.cpp
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2153 2022-11-14 21:57:01.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/sa/src/cpu_sa.h
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-11-14 21:57:29.937267 dwave-samplers-1.0.0.dev2/dwave/samplers/tabu/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      716 2022-11-14 21:57:01.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/tabu/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9429 2022-11-14 21:57:01.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/tabu/sampler.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-11-14 21:57:29.937267 dwave-samplers-1.0.0.dev2/dwave/samplers/tabu/src/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3270 2022-11-14 21:57:01.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/tabu/src/bqp.cpp
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2852 2022-11-14 21:57:01.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/tabu/src/bqp.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1013 2022-11-14 21:57:01.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/tabu/src/common.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16205 2022-11-14 21:57:01.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/tabu/src/tabu_search.cpp
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6359 2022-11-14 21:57:01.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/tabu/src/tabu_search.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1110 2022-11-14 21:57:01.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/tabu/src/tabu_utils.cpp
--rw-r--r--   0 circleci  (3434) circleci  (3434)      726 2022-11-14 21:57:01.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/tabu/src/tabu_utils.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1130 2022-11-14 21:57:01.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/tabu/tabu.pxd
--rw-r--r--   0 circleci  (3434) circleci  (3434)   838481 2022-11-14 21:57:25.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/tabu/tabu_search.cpp
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2823 2022-11-14 21:57:01.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/tabu/tabu_search.pyx
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1271 2022-11-14 21:57:01.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/tabu/utils.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-11-14 21:57:29.941268 dwave-samplers-1.0.0.dev2/dwave/samplers/tree/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      654 2022-11-14 21:57:01.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/tree/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      814 2022-11-14 21:57:01.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/tree/orang.pxd
--rw-r--r--   0 circleci  (3434) circleci  (3434)   977136 2022-11-14 21:57:26.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/tree/sample.cpp
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6139 2022-11-14 21:57:01.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/tree/sample.pyx
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14870 2022-11-14 21:57:01.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/tree/samplers.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)   946492 2022-11-14 21:57:28.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/tree/solve.cpp
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4063 2022-11-14 21:57:01.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/tree/solve.pyx
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-11-14 21:57:29.929268 dwave-samplers-1.0.0.dev2/dwave/samplers/tree/src/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-11-14 21:57:29.941268 dwave-samplers-1.0.0.dev2/dwave/samplers/tree/src/include/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1111 2022-11-14 21:57:01.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/tree/src/include/base.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8204 2022-11-14 21:57:01.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/tree/src/include/buckettree.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1401 2022-11-14 21:57:01.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/tree/src/include/combine.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1475 2022-11-14 21:57:01.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/tree/src/include/exception.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2554 2022-11-14 21:57:01.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/tree/src/include/graph.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2867 2022-11-14 21:57:01.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/tree/src/include/marginalizer.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10589 2022-11-14 21:57:01.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/tree/src/include/merger.h
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-11-14 21:57:29.941268 dwave-samplers-1.0.0.dev2/dwave/samplers/tree/src/include/operations/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3809 2022-11-14 21:57:01.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/tree/src/include/operations/count.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1924 2022-11-14 21:57:01.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/tree/src/include/operations/dummy.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4853 2022-11-14 21:57:01.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/tree/src/include/operations/logsumprod.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8211 2022-11-14 21:57:01.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/tree/src/include/operations/min.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1132 2022-11-14 21:57:01.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/tree/src/include/orang.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8434 2022-11-14 21:57:01.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/tree/src/include/sample.hpp
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4378 2022-11-14 21:57:01.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/tree/src/include/solve.hpp
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5554 2022-11-14 21:57:01.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/tree/src/include/table.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8549 2022-11-14 21:57:01.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/tree/src/include/task.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6578 2022-11-14 21:57:01.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/tree/src/include/treedecomp.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3334 2022-11-14 21:57:01.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/tree/src/include/utils.hpp
--rw-r--r--   0 circleci  (3434) circleci  (3434)    18737 2022-11-14 21:57:01.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/tree/src/include/varorder.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)   892627 2022-11-14 21:57:29.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/tree/utilities.cpp
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4498 2022-11-14 21:57:01.000000 dwave-samplers-1.0.0.dev2/dwave/samplers/tree/utilities.pyx
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-11-14 21:57:29.945268 dwave-samplers-1.0.0.dev2/dwave_samplers.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9705 2022-11-14 21:57:29.000000 dwave-samplers-1.0.0.dev2/dwave_samplers.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2630 2022-11-14 21:57:29.000000 dwave-samplers-1.0.0.dev2/dwave_samplers.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-11-14 21:57:29.000000 dwave-samplers-1.0.0.dev2/dwave_samplers.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-11-14 21:57:29.000000 dwave-samplers-1.0.0.dev2/dwave_samplers.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)       59 2022-11-14 21:57:29.000000 dwave-samplers-1.0.0.dev2/dwave_samplers.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        6 2022-11-14 21:57:29.000000 dwave-samplers-1.0.0.dev2/dwave_samplers.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      580 2022-11-14 21:57:01.000000 dwave-samplers-1.0.0.dev2/pyproject.toml
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1408 2022-11-14 21:57:29.945268 dwave-samplers-1.0.0.dev2/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1804 2022-11-14 21:57:01.000000 dwave-samplers-1.0.0.dev2/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-21 20:07:21.845608 dwave-samplers-1.1.0/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11386 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       91 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/MANIFEST.in
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9781 2023-07-21 20:07:21.845608 dwave-samplers-1.1.0/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8589 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/README.rst
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-21 20:07:21.833608 dwave-samplers-1.1.0/dwave/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      677 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/dwave/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-21 20:07:21.833608 dwave-samplers-1.1.0/dwave/samplers/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      818 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/dwave/samplers/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-21 20:07:21.833608 dwave-samplers-1.1.0/dwave/samplers/greedy/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      749 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/dwave/samplers/greedy/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2576 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/dwave/samplers/greedy/composite.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1069 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/dwave/samplers/greedy/decl.pxd
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   878496 2023-07-21 20:07:14.000000 dwave-samplers-1.1.0/dwave/samplers/greedy/descent.cpp
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4380 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/dwave/samplers/greedy/descent.pyx
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12187 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/dwave/samplers/greedy/sampler.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-21 20:07:21.837608 dwave-samplers-1.1.0/dwave/samplers/greedy/src/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15691 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/dwave/samplers/greedy/src/descent.cpp
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1862 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/dwave/samplers/greedy/src/descent.h
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-21 20:07:21.837608 dwave-samplers-1.1.0/dwave/samplers/planar/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      624 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/dwave/samplers/planar/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7276 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/dwave/samplers/planar/planar.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4865 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/dwave/samplers/planar/sampler.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1369 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/dwave/samplers/planar/util.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-21 20:07:21.837608 dwave-samplers-1.1.0/dwave/samplers/random/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      655 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/dwave/samplers/random/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   937641 2023-07-21 20:07:15.000000 dwave-samplers-1.1.0/dwave/samplers/random/cyrandom.cpp
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5545 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/dwave/samplers/random/cyrandom.pyx
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5072 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/dwave/samplers/random/sampler.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-21 20:07:21.837608 dwave-samplers-1.1.0/dwave/samplers/sa/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      684 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/dwave/samplers/sa/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    27362 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/dwave/samplers/sa/sampler.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   914532 2023-07-21 20:07:16.000000 dwave-samplers-1.1.0/dwave/samplers/sa/simulated_annealing.cpp
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8105 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/dwave/samplers/sa/simulated_annealing.pyx
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-21 20:07:21.837608 dwave-samplers-1.1.0/dwave/samplers/sa/src/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16087 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/dwave/samplers/sa/src/cpu_sa.cpp
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2610 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/dwave/samplers/sa/src/cpu_sa.h
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-21 20:07:21.841608 dwave-samplers-1.1.0/dwave/samplers/tabu/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      716 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/dwave/samplers/tabu/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9429 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/dwave/samplers/tabu/sampler.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-21 20:07:21.841608 dwave-samplers-1.1.0/dwave/samplers/tabu/src/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3270 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/dwave/samplers/tabu/src/bqp.cpp
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2852 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/dwave/samplers/tabu/src/bqp.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1013 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/dwave/samplers/tabu/src/common.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16205 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/dwave/samplers/tabu/src/tabu_search.cpp
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6359 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/dwave/samplers/tabu/src/tabu_search.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1110 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/dwave/samplers/tabu/src/tabu_utils.cpp
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      726 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/dwave/samplers/tabu/src/tabu_utils.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1130 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/dwave/samplers/tabu/tabu.pxd
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   838481 2023-07-21 20:07:17.000000 dwave-samplers-1.1.0/dwave/samplers/tabu/tabu_search.cpp
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2823 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/dwave/samplers/tabu/tabu_search.pyx
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1271 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/dwave/samplers/tabu/utils.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-21 20:07:21.845608 dwave-samplers-1.1.0/dwave/samplers/tree/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      654 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/dwave/samplers/tree/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      814 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/dwave/samplers/tree/orang.pxd
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   969263 2023-07-21 20:07:18.000000 dwave-samplers-1.1.0/dwave/samplers/tree/sample.cpp
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6139 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/dwave/samplers/tree/sample.pyx
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13926 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/dwave/samplers/tree/samplers.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   938619 2023-07-21 20:07:20.000000 dwave-samplers-1.1.0/dwave/samplers/tree/solve.cpp
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4063 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/dwave/samplers/tree/solve.pyx
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-21 20:07:21.833608 dwave-samplers-1.1.0/dwave/samplers/tree/src/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-21 20:07:21.845608 dwave-samplers-1.1.0/dwave/samplers/tree/src/include/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1111 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/dwave/samplers/tree/src/include/base.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8204 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/dwave/samplers/tree/src/include/buckettree.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1401 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/dwave/samplers/tree/src/include/combine.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1475 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/dwave/samplers/tree/src/include/exception.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2554 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/dwave/samplers/tree/src/include/graph.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2867 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/dwave/samplers/tree/src/include/marginalizer.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10589 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/dwave/samplers/tree/src/include/merger.h
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-21 20:07:21.845608 dwave-samplers-1.1.0/dwave/samplers/tree/src/include/operations/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3809 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/dwave/samplers/tree/src/include/operations/count.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1924 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/dwave/samplers/tree/src/include/operations/dummy.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4793 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/dwave/samplers/tree/src/include/operations/logsumprod.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8211 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/dwave/samplers/tree/src/include/operations/min.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1132 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/dwave/samplers/tree/src/include/orang.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8434 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/dwave/samplers/tree/src/include/sample.hpp
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4378 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/dwave/samplers/tree/src/include/solve.hpp
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5554 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/dwave/samplers/tree/src/include/table.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8549 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/dwave/samplers/tree/src/include/task.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6578 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/dwave/samplers/tree/src/include/treedecomp.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3334 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/dwave/samplers/tree/src/include/utils.hpp
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    18737 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/dwave/samplers/tree/src/include/varorder.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   884754 2023-07-21 20:07:21.000000 dwave-samplers-1.1.0/dwave/samplers/tree/utilities.cpp
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4498 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/dwave/samplers/tree/utilities.pyx
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-21 20:07:21.845608 dwave-samplers-1.1.0/dwave_samplers.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9781 2023-07-21 20:07:21.000000 dwave-samplers-1.1.0/dwave_samplers.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2648 2023-07-21 20:07:21.000000 dwave-samplers-1.1.0/dwave_samplers.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-07-21 20:07:21.000000 dwave-samplers-1.1.0/dwave_samplers.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-07-21 20:07:21.000000 dwave-samplers-1.1.0/dwave_samplers.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       59 2023-07-21 20:07:21.000000 dwave-samplers-1.1.0/dwave_samplers.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        6 2023-07-21 20:07:21.000000 dwave-samplers-1.1.0/dwave_samplers.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1236 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/pyproject.toml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1455 2023-07-21 20:07:21.845608 dwave-samplers-1.1.0/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1804 2023-07-21 20:07:00.000000 dwave-samplers-1.1.0/setup.py
```

### Comparing `dwave-samplers-1.0.0.dev2/LICENSE` & `dwave-samplers-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dwave-samplers-1.0.0.dev2/PKG-INFO` & `dwave-samplers-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: dwave-samplers
-Version: 1.0.0.dev2
+Version: 1.1.0
 Summary: Ocean-compatible collection of solvers/samplers
 Home-page: https://github.com/dwavesystems/dwave-samplers
 Author: D-Wave Systems Inc.
 Author-email: tools@dwavesys.com
 License: Apache 2.0
 Project-URL: Documentation, https://docs.ocean.dwavesys.com/en/stable/docs_greedy/sdk_index.html
 Project-URL: Issue Tracker, https://github.com/dwavesystems/dwave-samplers/issues/
 Project-URL: Source Code, https://github.com/dwavesystems/dwave-samplers/
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 .. image:: https://img.shields.io/pypi/v/dwave-samplers.svg
     :target: https://pypi.python.org/pypi/dwave-samplers
@@ -47,16 +49,16 @@
 that run either remotely (for example, in D-Wave's
 `Leap <https://cloud.dwavesys.com/leap/>`_ environment) or locally on your CPU.
 
 *dwave-samplers* implements the following classical algorithms for solving
 `binary quadratic models <https://docs.ocean.dwavesys.com/en/stable/concepts/bqm.html>`_
 (BQM):
 
-* Planar: an exact solver for planar Ising problems with no linear biases.
-* Random: a sampler that draws uniform random samples.
+* `Planar`_: an exact solver for planar Ising problems with no linear biases.
+* `Random`_: a sampler that draws uniform random samples.
 * `Simulated Annealing`_: a probabilistic heuristic for optimization and approximate
   Boltzmann sampling well suited to finding good solutions of large problems.
 * `Steepest Descent`_: a discrete analogue of gradient descent, often used in
   machine learning, that quickly finds a local minimum.
 * `Tabu`_: a heuristic that employs local search with methods to escape local minima.
 * `Tree Decomposition`_: an exact solver for problems with low treewidth.
 
@@ -97,15 +99,15 @@
 
 >>> sampleset = sampler.sample(bqm, time_limit=.1, max_num_samples=5)
 >>> num_reads = sampleset.info['num_reads']  # the total number of samples generated
 
 Simulated Annealing
 ===================
 
-`Simulated annealing <https://en.wikipedia.org/wiki/Simulated_annealing>`_ can be
+`Simulated annealing <https://en.wikipedia.org/wiki/Simulated_annealing>`__ can be
 used for heuristic optimization or approximate Boltzmann sampling. The
 *dwave-samplers* implementation approaches the equilibrium distribution by
 performing updates at a sequence of decreasing temperatures, terminating at the
 target `β`.\ [#]_ Each spin is updated once in a fixed order per point
 per temperature according to a Metropolis-Hastings update. When the temperature
 is low the target distribution concentrates, at equilibrium, over ground states
 of the model. Samples are guaranteed to match the equilibrium for long, smooth
@@ -129,15 +131,15 @@
 
 >>> sampleset = sampler.sample(bqm)
 >>> sampleset = sampler.sample(bqm, beta_range=[.1, 4.2], beta_schedule_type='linear')
 
 Steepest Descent
 ================
 
-`Steepest descent <https://en.wikipedia.org/wiki/Gradient_descent>`_ is the
+`Steepest descent <https://en.wikipedia.org/wiki/Gradient_descent>`__ is the
 discrete analogue of gradient descent, but the best move is computed using a local
 minimization rather rather than computing a gradient. The dimension along which
 to descend is determined, at each step, by the variable flip that causes the
 greatest reduction in energy.
 
 Steepest descent is fast and effective for unfrustrated problems, but it can get
 stuck in local minima.
@@ -171,15 +173,15 @@
    x  y energy num_oc. num_st.
 0  0  0    0.0       1       0
 ['BINARY', 1 rows, 1 samples, 2 variables]
 
 Tabu
 ====
 
-`Tabu search <https://en.wikipedia.org/wiki/Tabu_search>`_ is a heuristic that
+`Tabu search <https://en.wikipedia.org/wiki/Tabu_search>`__ is a heuristic that
 employs local search and can escape local minima by maintaining a "tabu list" of
 recently explored states that it does not revisit. The length of this tabu list
 is called the "tenure". *dwave-samplers* implementats the
 `MST2 multistart tabu search algorithm <https://link.springer.com/article/10.1023/B:ANOR.0000039522.58036.68>`_
 for quadratic unconstrained binary optimization (QUBO) problems.
 
 Each read of the tabu algorithm consists of many starts. The solver takes the best
@@ -198,15 +200,15 @@
 
 >>> sampleset0 = sampler.sample(qubo)
 >>> sampleset1 = sampler.sample(qubo, tenure=1, num_restarts=1)
 
 Tree Decomposition
 ==================
 
-`Tree decomposition <https://en.wikipedia.org/wiki/Tree_decomposition>`_-based
+`Tree decomposition <https://en.wikipedia.org/wiki/Tree_decomposition>`__-based
 solvers have a runtime that is exponential in the
 `treewidth <https://en.wikipedia.org/wiki/Treewidth>`_ of the problem graph. For
 problems with low treewidth, the solver can find ground states very quickly.
 However, for even moderately dense problems, performance is very poor.
 
 >>> from dwave.samplers import TreeDecompositionSolver
 >>> solver = TreeDecompositionSolver()
@@ -263,7 +265,9 @@
 .. code-block:: bash
 
     reno new your-short-descriptor-here
 
 You can then edit the file created under ``releasenotes/notes/``.
 Remove any sections not relevant to your changes.
 Commit the file along with your changes.
+
+
```

### Comparing `dwave-samplers-1.0.0.dev2/README.rst` & `dwave-samplers-1.1.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 that run either remotely (for example, in D-Wave's
 `Leap <https://cloud.dwavesys.com/leap/>`_ environment) or locally on your CPU.
 
 *dwave-samplers* implements the following classical algorithms for solving
 `binary quadratic models <https://docs.ocean.dwavesys.com/en/stable/concepts/bqm.html>`_
 (BQM):
 
-* Planar: an exact solver for planar Ising problems with no linear biases.
-* Random: a sampler that draws uniform random samples.
+* `Planar`_: an exact solver for planar Ising problems with no linear biases.
+* `Random`_: a sampler that draws uniform random samples.
 * `Simulated Annealing`_: a probabilistic heuristic for optimization and approximate
   Boltzmann sampling well suited to finding good solutions of large problems.
 * `Steepest Descent`_: a discrete analogue of gradient descent, often used in
   machine learning, that quickly finds a local minimum.
 * `Tabu`_: a heuristic that employs local search with methods to escape local minima.
 * `Tree Decomposition`_: an exact solver for problems with low treewidth.
 
@@ -72,15 +72,15 @@
 
 >>> sampleset = sampler.sample(bqm, time_limit=.1, max_num_samples=5)
 >>> num_reads = sampleset.info['num_reads']  # the total number of samples generated
 
 Simulated Annealing
 ===================
 
-`Simulated annealing <https://en.wikipedia.org/wiki/Simulated_annealing>`_ can be
+`Simulated annealing <https://en.wikipedia.org/wiki/Simulated_annealing>`__ can be
 used for heuristic optimization or approximate Boltzmann sampling. The
 *dwave-samplers* implementation approaches the equilibrium distribution by
 performing updates at a sequence of decreasing temperatures, terminating at the
 target `β`.\ [#]_ Each spin is updated once in a fixed order per point
 per temperature according to a Metropolis-Hastings update. When the temperature
 is low the target distribution concentrates, at equilibrium, over ground states
 of the model. Samples are guaranteed to match the equilibrium for long, smooth
@@ -104,15 +104,15 @@
 
 >>> sampleset = sampler.sample(bqm)
 >>> sampleset = sampler.sample(bqm, beta_range=[.1, 4.2], beta_schedule_type='linear')
 
 Steepest Descent
 ================
 
-`Steepest descent <https://en.wikipedia.org/wiki/Gradient_descent>`_ is the
+`Steepest descent <https://en.wikipedia.org/wiki/Gradient_descent>`__ is the
 discrete analogue of gradient descent, but the best move is computed using a local
 minimization rather rather than computing a gradient. The dimension along which
 to descend is determined, at each step, by the variable flip that causes the
 greatest reduction in energy.
 
 Steepest descent is fast and effective for unfrustrated problems, but it can get
 stuck in local minima.
@@ -146,15 +146,15 @@
    x  y energy num_oc. num_st.
 0  0  0    0.0       1       0
 ['BINARY', 1 rows, 1 samples, 2 variables]
 
 Tabu
 ====
 
-`Tabu search <https://en.wikipedia.org/wiki/Tabu_search>`_ is a heuristic that
+`Tabu search <https://en.wikipedia.org/wiki/Tabu_search>`__ is a heuristic that
 employs local search and can escape local minima by maintaining a "tabu list" of
 recently explored states that it does not revisit. The length of this tabu list
 is called the "tenure". *dwave-samplers* implementats the
 `MST2 multistart tabu search algorithm <https://link.springer.com/article/10.1023/B:ANOR.0000039522.58036.68>`_
 for quadratic unconstrained binary optimization (QUBO) problems.
 
 Each read of the tabu algorithm consists of many starts. The solver takes the best
@@ -173,15 +173,15 @@
 
 >>> sampleset0 = sampler.sample(qubo)
 >>> sampleset1 = sampler.sample(qubo, tenure=1, num_restarts=1)
 
 Tree Decomposition
 ==================
 
-`Tree decomposition <https://en.wikipedia.org/wiki/Tree_decomposition>`_-based
+`Tree decomposition <https://en.wikipedia.org/wiki/Tree_decomposition>`__-based
 solvers have a runtime that is exponential in the
 `treewidth <https://en.wikipedia.org/wiki/Treewidth>`_ of the problem graph. For
 problems with low treewidth, the solver can find ground states very quickly.
 However, for even moderately dense problems, performance is very poor.
 
 >>> from dwave.samplers import TreeDecompositionSolver
 >>> solver = TreeDecompositionSolver()
```

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/__init__.py` & `dwave-samplers-1.1.0/dwave/samplers/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = '1.0.0.dev2'
+__version__ = '1.1.0'
 
 from dwave.samplers.greedy import *
 
 from dwave.samplers.random import *
 
 from dwave.samplers.sa import *
```

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/greedy/__init__.py` & `dwave-samplers-1.1.0/dwave/samplers/greedy/__init__.py`

 * *Files identical despite different names*

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/greedy/composite.py` & `dwave-samplers-1.1.0/dwave/samplers/greedy/composite.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     properties = None  # overwritten by init
     """Properties in the form of a dict.
 
     Contains the properties of the child sampler.
     """
 
     def sample(self, bqm: dimod.BinaryQuadraticModel, **parameters) -> dimod.SampleSet:
-        """Sample from the provided binary quadratic model.
+        """Find minima of a binary quadratic model.
 
         Args:
             bqm:
                 Binary quadratic model to be sampled from.
 
             **parameters:
                 Parameters for the sampling method, specified by the child
```

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/greedy/decl.pxd` & `dwave-samplers-1.1.0/dwave/samplers/greedy/decl.pxd`

 * *Files 12% similar despite different names*

```diff
@@ -11,18 +11,20 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from libcpp cimport bool
 from libcpp.vector cimport vector
 
+cimport numpy as np
+
 cdef extern from "descent.h":
 
     unsigned int steepest_gradient_descent(
-        char* states,
+        np.int8_t* states,
         double* energies,
         unsigned* num_steps,
         const int num_samples,
         const vector[double]& linear_biases,
         const vector[int]& coupler_starts,
         const vector[int]& coupler_ends,
         const vector[double]& coupler_weights,
```

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/greedy/descent.cpp` & `dwave-samplers-1.1.0/dwave/samplers/greedy/descent.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -720,17 +720,14 @@
 #include "new"
 #include "stdexcept"
 #include "typeinfo"
 #include <vector>
 #include <string.h>
 #include <stdio.h>
 #include "numpy/arrayobject.h"
-#include "numpy/ndarrayobject.h"
-#include "numpy/ndarraytypes.h"
-#include "numpy/arrayscalars.h"
 #include "numpy/ufuncobject.h"
 
     /* NumPy API declarations from "numpy/__init__.pxd" */
     
 #include "descent.h"
 #include "pythread.h"
 #include <stdlib.h>
@@ -1076,195 +1073,195 @@
 
 /* ForceInitThreads.proto */
 #ifndef __PYX_FORCE_INIT_THREADS
   #define __PYX_FORCE_INIT_THREADS 0
 #endif
 
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":690
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":691
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":692
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":693
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":697
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":698
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":699
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":700
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":704
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":705
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":714
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":715
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":716
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":718
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":719
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":720
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":722
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":723
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":725
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":726
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":727
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1295,42 +1292,42 @@
 
 /*--- Type declarations ---*/
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":729
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":730
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":731
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":733
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -2240,24 +2237,14 @@
 /* Module declarations from 'numpy' */
 
 /* Module declarations from 'numpy' */
 static PyTypeObject *__pyx_ptype_5numpy_dtype = 0;
 static PyTypeObject *__pyx_ptype_5numpy_flatiter = 0;
 static PyTypeObject *__pyx_ptype_5numpy_broadcast = 0;
 static PyTypeObject *__pyx_ptype_5numpy_ndarray = 0;
-static PyTypeObject *__pyx_ptype_5numpy_generic = 0;
-static PyTypeObject *__pyx_ptype_5numpy_number = 0;
-static PyTypeObject *__pyx_ptype_5numpy_integer = 0;
-static PyTypeObject *__pyx_ptype_5numpy_signedinteger = 0;
-static PyTypeObject *__pyx_ptype_5numpy_unsignedinteger = 0;
-static PyTypeObject *__pyx_ptype_5numpy_inexact = 0;
-static PyTypeObject *__pyx_ptype_5numpy_floating = 0;
-static PyTypeObject *__pyx_ptype_5numpy_complexfloating = 0;
-static PyTypeObject *__pyx_ptype_5numpy_flexible = 0;
-static PyTypeObject *__pyx_ptype_5numpy_character = 0;
 static PyTypeObject *__pyx_ptype_5numpy_ufunc = 0;
 
 /* Module declarations from 'dwave.samplers.greedy.decl' */
 
 /* Module declarations from 'dwave.samplers.greedy.descent' */
 static PyTypeObject *__pyx_array_type = 0;
 static PyTypeObject *__pyx_MemviewEnum_type = 0;
@@ -2301,15 +2288,15 @@
 static void __pyx_memoryview_broadcast_leading(__Pyx_memviewslice *, int, int); /*proto*/
 static void __pyx_memoryview_refcount_copying(__Pyx_memviewslice *, int, int, int); /*proto*/
 static void __pyx_memoryview_refcount_objects_in_slice_with_gil(char *, Py_ssize_t *, Py_ssize_t *, int, int); /*proto*/
 static void __pyx_memoryview_refcount_objects_in_slice(char *, Py_ssize_t *, Py_ssize_t *, int, int); /*proto*/
 static void __pyx_memoryview_slice_assign_scalar(__Pyx_memviewslice *, int, size_t, void *, int); /*proto*/
 static void __pyx_memoryview__slice_assign_scalar(char *, Py_ssize_t *, Py_ssize_t *, int, size_t, void *); /*proto*/
 static PyObject *__pyx_unpickle_Enum__set_state(struct __pyx_MemviewEnum_obj *, PyObject *); /*proto*/
-static __Pyx_TypeInfo __Pyx_TypeInfo_char = { "char", NULL, sizeof(char), { 0 }, 0, 'H', IS_UNSIGNED(char), 0 };
+static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_5numpy_int8_t = { "int8_t", NULL, sizeof(__pyx_t_5numpy_int8_t), { 0 }, 0, IS_UNSIGNED(__pyx_t_5numpy_int8_t) ? 'U' : 'I', IS_UNSIGNED(__pyx_t_5numpy_int8_t), 0 };
 static __Pyx_TypeInfo __Pyx_TypeInfo_double = { "double", NULL, sizeof(double), { 0 }, 0, 'R', 0, 0 };
 static __Pyx_TypeInfo __Pyx_TypeInfo_unsigned_int = { "unsigned int", NULL, sizeof(unsigned int), { 0 }, 0, IS_UNSIGNED(unsigned int) ? 'U' : 'I', IS_UNSIGNED(unsigned int), 0 };
 #define __Pyx_MODULE_NAME "dwave.samplers.greedy.descent"
 extern int __pyx_module_is_main_dwave__samplers__greedy__descent;
 int __pyx_module_is_main_dwave__samplers__greedy__descent = 0;
 
 /* Implementation of 'dwave.samplers.greedy.descent' */
@@ -2654,15 +2641,15 @@
  * def steepest_gradient_descent(num_samples,             # <<<<<<<<<<<<<<
  *                               linear_biases,
  *                               coupler_starts, coupler_ends, coupler_weights,
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_5dwave_8samplers_6greedy_7descent_1steepest_gradient_descent(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_5dwave_8samplers_6greedy_7descent_steepest_gradient_descent[] = "Wraps `steepest_gradient_descent` from `descent.cpp`. Accepts\n    an Ising problem defined on a general graph and returns samples\n    using steepest gradient descent seeded with initial states from\n    `states_numpy`.\n\n    Parameters\n    ----------\n    num_samples : int\n        Number of samples to get from the sampler.\n\n    linear_biases : list(float)\n        The linear biases or field values for the problem.\n\n    coupler_starts : list(int)\n        A list of the start variable of each coupler. For a problem\n        with the couplers (0, 1), (1, 2), and (3, 1), `coupler_starts`\n        should be [0, 1, 3].\n\n    coupler_ends : list(int)\n        A list of the end variable of each coupler. For a problem\n        with the couplers (0, 1), (1, 2), and (3, 1), `coupler_ends`\n        should be [1, 2, 1].\n\n    coupler_weights : list(float)\n        A list of the J values or weight on each coupler, in the same\n        order as `coupler_starts` and `coupler_ends`.\n\n    states_numpy : np.ndarray[char, ndim=2, mode=\"c\"], values in (-1, 1)\n        The initial seeded states of the gradient descent runs. Should be of\n        a contiguous numpy.ndarray of shape (num_samples, num_variables).\n\n    large_sparse_opt : bool\n        When set to True, large-and-sparse problem graph optimizations are used.\n\n    Returns\n    -------\n    samples : numpy.ndarray\n        A 2D numpy array where each row is a sample.\n\n    energies: numpy.ndarray\n        Sample energies.\n\n    num_steps: numpy.ndarray\n        Number of downhill steps per sample.\n    ";
+static char __pyx_doc_5dwave_8samplers_6greedy_7descent_steepest_gradient_descent[] = "Wraps `steepest_gradient_descent` from `descent.cpp`. Accepts\n    an Ising problem defined on a general graph and returns samples\n    using steepest gradient descent seeded with initial states from\n    `states_numpy`.\n\n    Parameters\n    ----------\n    num_samples : int\n        Number of samples to get from the sampler.\n\n    linear_biases : list(float)\n        The linear biases or field values for the problem.\n\n    coupler_starts : list(int)\n        A list of the start variable of each coupler. For a problem\n        with the couplers (0, 1), (1, 2), and (3, 1), `coupler_starts`\n        should be [0, 1, 3].\n\n    coupler_ends : list(int)\n        A list of the end variable of each coupler. For a problem\n        with the couplers (0, 1), (1, 2), and (3, 1), `coupler_ends`\n        should be [1, 2, 1].\n\n    coupler_weights : list(float)\n        A list of the J values or weight on each coupler, in the same\n        order as `coupler_starts` and `coupler_ends`.\n\n    states_numpy : np.ndarray[np.int8_t, ndim=2, mode=\"c\"], values in (-1, 1)\n        The initial seeded states of the gradient descent runs. Should be of\n        a contiguous numpy.ndarray of shape (num_samples, num_variables).\n\n    large_sparse_opt : bool\n        When set to True, large-and-sparse problem graph optimizations are used.\n\n    Returns\n    -------\n    samples : numpy.ndarray\n        A 2D numpy array where each row is a sample.\n\n    energies: numpy.ndarray\n        Sample energies.\n\n    num_steps: numpy.ndarray\n        Number of downhill steps per sample.\n    ";
 static PyMethodDef __pyx_mdef_5dwave_8samplers_6greedy_7descent_1steepest_gradient_descent = {"steepest_gradient_descent", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_5dwave_8samplers_6greedy_7descent_1steepest_gradient_descent, METH_VARARGS|METH_KEYWORDS, __pyx_doc_5dwave_8samplers_6greedy_7descent_steepest_gradient_descent};
 static PyObject *__pyx_pw_5dwave_8samplers_6greedy_7descent_1steepest_gradient_descent(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_num_samples = 0;
   PyObject *__pyx_v_linear_biases = 0;
   PyObject *__pyx_v_coupler_starts = 0;
   PyObject *__pyx_v_coupler_ends = 0;
   PyObject *__pyx_v_coupler_weights = 0;
@@ -2676,15 +2663,15 @@
   __Pyx_RefNannySetupContext("steepest_gradient_descent (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_num_samples,&__pyx_n_s_linear_biases,&__pyx_n_s_coupler_starts,&__pyx_n_s_coupler_ends,&__pyx_n_s_coupler_weights,&__pyx_n_s_states_numpy,&__pyx_n_s_large_sparse_opt,0};
     PyObject* values[7] = {0,0,0,0,0,0,0};
 
     /* "dwave/samplers/greedy/descent.pyx":33
  *                               coupler_starts, coupler_ends, coupler_weights,
- *                               np.ndarray[char, ndim=2, mode="c"] states_numpy,
+ *                               np.ndarray[np.int8_t, ndim=2, mode="c"] states_numpy,
  *                               large_sparse_opt=False):             # <<<<<<<<<<<<<<
  * 
  *     """Wraps `steepest_gradient_descent` from `descent.cpp`. Accepts
  */
     values[6] = ((PyObject *)Py_False);
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
@@ -2805,15 +2792,15 @@
 static PyObject *__pyx_pf_5dwave_8samplers_6greedy_7descent_steepest_gradient_descent(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_num_samples, PyObject *__pyx_v_linear_biases, PyObject *__pyx_v_coupler_starts, PyObject *__pyx_v_coupler_ends, PyObject *__pyx_v_coupler_weights, PyArrayObject *__pyx_v_states_numpy, PyObject *__pyx_v_large_sparse_opt) {
   Py_ssize_t __pyx_v_num_vars;
   PyObject *__pyx_v_states = NULL;
   PyObject *__pyx_v_energies_numpy = NULL;
   __Pyx_memviewslice __pyx_v_energies = { 0, 0, { 0 }, { 0 }, { 0 } };
   PyObject *__pyx_v_num_steps_numpy = NULL;
   __Pyx_memviewslice __pyx_v_num_steps = { 0, 0, { 0 }, { 0 }, { 0 } };
-  char *__pyx_v__states;
+  __pyx_t_5numpy_int8_t *__pyx_v__states;
   double *__pyx_v__energies;
   unsigned int *__pyx_v__num_steps;
   int __pyx_v__num_samples;
   bool __pyx_v__large_sparse_opt;
   std::vector<double>  __pyx_v__linear_biases;
   std::vector<int>  __pyx_v__coupler_starts;
   std::vector<int>  __pyx_v__coupler_ends;
@@ -2845,15 +2832,15 @@
   __Pyx_RefNannySetupContext("steepest_gradient_descent", 0);
   __pyx_pybuffer_states_numpy.pybuffer.buf = NULL;
   __pyx_pybuffer_states_numpy.refcount = 0;
   __pyx_pybuffernd_states_numpy.data = NULL;
   __pyx_pybuffernd_states_numpy.rcbuffer = &__pyx_pybuffer_states_numpy;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_states_numpy.rcbuffer->pybuffer, (PyObject*)__pyx_v_states_numpy, &__Pyx_TypeInfo_char, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 2, 0, __pyx_stack) == -1)) __PYX_ERR(0, 29, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_states_numpy.rcbuffer->pybuffer, (PyObject*)__pyx_v_states_numpy, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int8_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 2, 0, __pyx_stack) == -1)) __PYX_ERR(0, 29, __pyx_L1_error)
   }
   __pyx_pybuffernd_states_numpy.diminfo[0].strides = __pyx_pybuffernd_states_numpy.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_states_numpy.diminfo[0].shape = __pyx_pybuffernd_states_numpy.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_states_numpy.diminfo[1].strides = __pyx_pybuffernd_states_numpy.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_states_numpy.diminfo[1].shape = __pyx_pybuffernd_states_numpy.rcbuffer->pybuffer.shape[1];
 
   /* "dwave/samplers/greedy/descent.pyx":80
  *         Number of downhill steps per sample.
  *     """
  *     num_vars = len(linear_biases)             # <<<<<<<<<<<<<<
@@ -3123,15 +3110,15 @@
   __pyx_v_num_steps = __pyx_t_11;
   __pyx_t_11.memview = NULL;
   __pyx_t_11.data = NULL;
 
   /* "dwave/samplers/greedy/descent.pyx":98
  * 
  *     # explicitly convert all Python types to C while we have the GIL
- *     cdef char* _states = &states_numpy[0, 0]             # <<<<<<<<<<<<<<
+ *     cdef np.int8_t* _states = &states_numpy[0, 0]             # <<<<<<<<<<<<<<
  *     cdef double* _energies = &energies[0]
  *     cdef unsigned* _num_steps = &num_steps[0]
  */
   __pyx_t_12 = 0;
   __pyx_t_13 = 0;
   __pyx_t_14 = -1;
   if (__pyx_t_12 < 0) {
@@ -3142,19 +3129,19 @@
     __pyx_t_13 += __pyx_pybuffernd_states_numpy.diminfo[1].shape;
     if (unlikely(__pyx_t_13 < 0)) __pyx_t_14 = 1;
   } else if (unlikely(__pyx_t_13 >= __pyx_pybuffernd_states_numpy.diminfo[1].shape)) __pyx_t_14 = 1;
   if (unlikely(__pyx_t_14 != -1)) {
     __Pyx_RaiseBufferIndexError(__pyx_t_14);
     __PYX_ERR(0, 98, __pyx_L1_error)
   }
-  __pyx_v__states = (&(*__Pyx_BufPtrCContig2d(char *, __pyx_pybuffernd_states_numpy.rcbuffer->pybuffer.buf, __pyx_t_12, __pyx_pybuffernd_states_numpy.diminfo[0].strides, __pyx_t_13, __pyx_pybuffernd_states_numpy.diminfo[1].strides)));
+  __pyx_v__states = (&(*__Pyx_BufPtrCContig2d(__pyx_t_5numpy_int8_t *, __pyx_pybuffernd_states_numpy.rcbuffer->pybuffer.buf, __pyx_t_12, __pyx_pybuffernd_states_numpy.diminfo[0].strides, __pyx_t_13, __pyx_pybuffernd_states_numpy.diminfo[1].strides)));
 
   /* "dwave/samplers/greedy/descent.pyx":99
  *     # explicitly convert all Python types to C while we have the GIL
- *     cdef char* _states = &states_numpy[0, 0]
+ *     cdef np.int8_t* _states = &states_numpy[0, 0]
  *     cdef double* _energies = &energies[0]             # <<<<<<<<<<<<<<
  *     cdef unsigned* _num_steps = &num_steps[0]
  *     cdef int _num_samples = num_samples
  */
   __pyx_t_13 = 0;
   __pyx_t_14 = -1;
   if (__pyx_t_13 < 0) {
@@ -3164,15 +3151,15 @@
   if (unlikely(__pyx_t_14 != -1)) {
     __Pyx_RaiseBufferIndexError(__pyx_t_14);
     __PYX_ERR(0, 99, __pyx_L1_error)
   }
   __pyx_v__energies = (&(*((double *) ( /* dim=0 */ (__pyx_v_energies.data + __pyx_t_13 * __pyx_v_energies.strides[0]) ))));
 
   /* "dwave/samplers/greedy/descent.pyx":100
- *     cdef char* _states = &states_numpy[0, 0]
+ *     cdef np.int8_t* _states = &states_numpy[0, 0]
  *     cdef double* _energies = &energies[0]
  *     cdef unsigned* _num_steps = &num_steps[0]             # <<<<<<<<<<<<<<
  *     cdef int _num_samples = num_samples
  *     cdef bool _large_sparse_opt = large_sparse_opt
  */
   __pyx_t_13 = 0;
   __pyx_t_14 = -1;
@@ -3347,15 +3334,15 @@
   __Pyx_XDECREF(__pyx_v_num_steps_numpy);
   __PYX_XDEC_MEMVIEW(&__pyx_v_num_steps, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":735
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3364,29 +3351,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":736
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 736, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":735
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3397,15 +3384,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":738
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3414,29 +3401,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":739
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 739, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":738
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3447,15 +3434,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":741
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3464,29 +3451,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":742
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 742, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":741
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3497,15 +3484,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":744
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3514,29 +3501,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":745
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 745, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":744
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3547,15 +3534,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":747
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3564,29 +3551,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":748
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 748, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":747
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3597,212 +3584,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":750
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":751
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":752
+    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":751
+    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":754
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":750
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":929
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":868
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":930
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":869
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":931
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":870
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":929
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":868
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":933
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":872
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":934
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":873
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":935
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":874
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":936
+    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":875
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":935
+    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":874
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":937
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":876
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":933
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":872
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":941
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":880
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -3818,15 +3805,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":942
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":881
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -3834,84 +3821,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":943
+      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":882
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 943, __pyx_L3_error)
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 882, __pyx_L3_error)
 
-      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":942
+      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":881
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":944
+    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":883
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 944, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 883, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":945
+      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":884
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 945, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 884, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 945, __pyx_L5_except_error)
+      __PYX_ERR(1, 884, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":942
+    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":881
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":941
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":880
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -3926,15 +3913,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":947
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":886
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -3950,15 +3937,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":948
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":887
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -3966,84 +3953,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":949
+      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":888
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 949, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 888, __pyx_L3_error)
 
-      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":948
+      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":887
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":950
+    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":889
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 950, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 889, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":951
+      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":890
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 951, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 890, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 951, __pyx_L5_except_error)
+      __PYX_ERR(1, 890, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":948
+    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":887
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":947
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":886
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4058,15 +4045,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":953
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":892
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4082,15 +4069,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":954
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":893
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4098,84 +4085,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":955
+      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":894
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 955, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 894, __pyx_L3_error)
 
-      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":954
+      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":893
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":956
+    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":895
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 956, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 895, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":957
+      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":896
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 957, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 896, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 957, __pyx_L5_except_error)
+      __PYX_ERR(1, 896, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":954
+    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":893
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":953
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":892
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4190,188 +4177,14 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":967
- * 
- * 
- * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
- *     """
- *     Cython equivalent of `isinstance(obj, np.timedelta64)`
- */
-
-static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
-
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":979
- *     bool
- *     """
- *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
-  goto __pyx_L0;
-
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":967
- * 
- * 
- * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
- *     """
- *     Cython equivalent of `isinstance(obj, np.timedelta64)`
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":982
- * 
- * 
- * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
- *     """
- *     Cython equivalent of `isinstance(obj, np.datetime64)`
- */
-
-static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("is_datetime64_object", 0);
-
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":994
- *     bool
- *     """
- *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
-  goto __pyx_L0;
-
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":982
- * 
- * 
- * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
- *     """
- *     Cython equivalent of `isinstance(obj, np.datetime64)`
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":997
- * 
- * 
- * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the int64 value underlying scalar numpy datetime64 object
- */
-
-static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
-  npy_datetime __pyx_r;
-
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":1004
- *     also needed.  That can be found using `get_datetime64_unit`.
- *     """
- *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
-  goto __pyx_L0;
-
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":997
- * 
- * 
- * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the int64 value underlying scalar numpy datetime64 object
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  return __pyx_r;
-}
-
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":1007
- * 
- * 
- * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the int64 value underlying scalar numpy timedelta64 object
- */
-
-static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
-  npy_timedelta __pyx_r;
-
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":1011
- *     returns the int64 value underlying scalar numpy timedelta64 object
- *     """
- *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
-  goto __pyx_L0;
-
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":1007
- * 
- * 
- * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the int64 value underlying scalar numpy timedelta64 object
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  return __pyx_r;
-}
-
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":1014
- * 
- * 
- * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the unit part of the dtype for a numpy datetime64 object.
- */
-
-static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
-  NPY_DATETIMEUNIT __pyx_r;
-
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":1018
- *     returns the unit part of the dtype for a numpy datetime64 object.
- *     """
- *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
- */
-  __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
-  goto __pyx_L0;
-
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":1014
- * 
- * 
- * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the unit part of the dtype for a numpy datetime64 object.
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  return __pyx_r;
-}
-
 /* "vector.from_py":45
  * 
  * @cname("__pyx_convert_vector_from_py_double")
  * cdef vector[X] __pyx_convert_vector_from_py_double(object o) except *:             # <<<<<<<<<<<<<<
  *     cdef vector[X] v
  *     for item in o:
  */
@@ -18517,15 +18330,15 @@
   {&__pyx_kp_s_unable_to_allocate_shape_and_str, __pyx_k_unable_to_allocate_shape_and_str, sizeof(__pyx_k_unable_to_allocate_shape_and_str), 0, 0, 1, 0},
   {&__pyx_n_s_unpack, __pyx_k_unpack, sizeof(__pyx_k_unpack), 0, 0, 1, 1},
   {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
   {&__pyx_n_s_zeros, __pyx_k_zeros, sizeof(__pyx_k_zeros), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 945, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 884, __pyx_L1_error)
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(2, 133, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(2, 148, __pyx_L1_error)
   __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(2, 151, __pyx_L1_error)
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(2, 180, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(2, 2, __pyx_L1_error)
   __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(2, 404, __pyx_L1_error)
   __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(2, 613, __pyx_L1_error)
@@ -18535,33 +18348,33 @@
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":945
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":884
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 945, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 884, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":951
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":890
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 951, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 890, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
   /* "View.MemoryView":133
  * 
  *         if not self.ndim:
  *             raise ValueError("Empty shape tuple for cython.array")             # <<<<<<<<<<<<<<
@@ -18964,46 +18777,26 @@
   sizeof(PyTypeObject),
   #else
   sizeof(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 200, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 200, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 199, __pyx_L1_error)
   __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 223, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 222, __pyx_L1_error)
   __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 227, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 226, __pyx_L1_error)
   __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 239, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 771, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 773, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 775, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 777, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 779, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 781, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 783, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 785, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 787, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 789, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
   __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 827, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 764, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
```

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/greedy/descent.pyx` & `dwave-samplers-1.1.0/dwave/samplers/greedy/descent.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 cimport decl
 
 
 def steepest_gradient_descent(num_samples,
                               linear_biases,
                               coupler_starts, coupler_ends, coupler_weights,
-                              np.ndarray[char, ndim=2, mode="c"] states_numpy,
+                              np.ndarray[np.int8_t, ndim=2, mode="c"] states_numpy,
                               large_sparse_opt=False):
 
     """Wraps `steepest_gradient_descent` from `descent.cpp`. Accepts
     an Ising problem defined on a general graph and returns samples
     using steepest gradient descent seeded with initial states from
     `states_numpy`.
 
@@ -55,15 +55,15 @@
         with the couplers (0, 1), (1, 2), and (3, 1), `coupler_ends`
         should be [1, 2, 1].
 
     coupler_weights : list(float)
         A list of the J values or weight on each coupler, in the same
         order as `coupler_starts` and `coupler_ends`.
 
-    states_numpy : np.ndarray[char, ndim=2, mode="c"], values in (-1, 1)
+    states_numpy : np.ndarray[np.int8_t, ndim=2, mode="c"], values in (-1, 1)
         The initial seeded states of the gradient descent runs. Should be of
         a contiguous numpy.ndarray of shape (num_samples, num_variables).
 
     large_sparse_opt : bool
         When set to True, large-and-sparse problem graph optimizations are used.
 
     Returns
@@ -91,15 +91,15 @@
     cdef double[:] energies = energies_numpy
 
     # allocate ndarray for steps
     num_steps_numpy = np.empty(num_samples, dtype=np.uint32)
     cdef unsigned[:] num_steps = num_steps_numpy
 
     # explicitly convert all Python types to C while we have the GIL
-    cdef char* _states = &states_numpy[0, 0]
+    cdef np.int8_t* _states = &states_numpy[0, 0]
     cdef double* _energies = &energies[0]
     cdef unsigned* _num_steps = &num_steps[0]
     cdef int _num_samples = num_samples
     cdef bool _large_sparse_opt = large_sparse_opt
     cdef vector[double] _linear_biases = linear_biases
 
     # TODO: in dimod 0.10+, coupler indices default to int64, but we downcast
```

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/greedy/sampler.py` & `dwave-samplers-1.1.0/dwave/samplers/greedy/sampler.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """A dimod sampler that uses the steepest gradient descent."""
 
 from numbers import Integral
+from time import perf_counter_ns
 from typing import Optional
 
 from dimod.core.initialized import InitialStateGenerator
 
 import dimod
 import numpy as np
 
@@ -119,15 +120,15 @@
 
     def sample(self, bqm: dimod.BinaryQuadraticModel,
                num_reads: Optional[int] = None,
                initial_states: Optional[dimod.typing.SamplesLike] = None,
                initial_states_generator: InitialStateGenerator = "random",
                seed: Optional[int] = None,
                large_sparse_opt: bool = False, **kwargs) -> dimod.SampleSet:
-        """Sample from a binary quadratic model.
+        """Find minima of a binary quadratic model.
 
         Starts from ``initial_states``, and converges to local minima using
         discrete steepest-descent method.
 
         Args:
             bqm: Binary quadratic model to be sampled.
 
@@ -165,16 +166,26 @@
                 particular seed with a constant set of parameters produces
                 identical results. If not provided, a random seed is chosen.
 
             large_sparse_opt:
                 Use optimizations for large and sparse problems (search tree for
                 next descent variable instead of linear array).
 
+        Returns:
+            A `dimod.SampleSet` for the binary quadratic model.
+
+            The `info` field of the sample set contains three categories of timing information:
+            preprocessing, sampling, and postprocessing time. All timings are reported in units of
+            nanoseconds. Preprocessing time is the total time spent converting the BQM variable type
+            (if required) and parsing input arguments. Sampling time is the total time the algorithm
+            spent in sampling states of the binary quadratic model. Postprocessing time is the total
+            time spent reverting variable type and creating a `dimod.SampleSet`.
+
         Note:
-            Number of descends (single variable flips) taken to reach the local
+            Number of descents (single variable flips) taken to reach the local
             minimum for each sample is stored in a data vector called ``num_steps``.
 
         Examples:
             This example samples a simple two-variable Ising model.
 
             >>> import dimod
             >>> bqm = dimod.BQM.from_ising({}, {'ab': 1})
@@ -215,15 +226,15 @@
             2 -1 -1   -5.0       1       2
             ['SPIN', 3 rows, 3 samples, 2 variables]
 
             Notice it required 2 variable flips (``num_steps`` field in the last
             column) to reach the minimum state, ``(-1, -1)``, from the initial
             state, ``(1, 1)``.
         """
-
+        timestamp_preprocess = perf_counter_ns()
         # get the original vartype so we can return consistently
         original_vartype = bqm.vartype
 
         # convert to spin
         if bqm.vartype is not dimod.SPIN:
             bqm = bqm.change_vartype(dimod.SPIN, inplace=False)
 
@@ -248,27 +259,40 @@
         linear, (coupler_starts, coupler_ends, coupler_weights), offset = \
             bqm.to_numpy_vectors(variable_order=initial_states.variables)
 
         # we need initial states as contiguous numpy array
         initial_states_array = \
             np.ascontiguousarray(initial_states.record.sample, dtype=np.int8)
 
+        timestamp_sample = perf_counter_ns()
+
         # run the steepest descent
         samples, energies, num_steps = steepest_gradient_descent(
             num_reads,
             linear, coupler_starts, coupler_ends, coupler_weights,
             initial_states_array, large_sparse_opt)
 
+        timestamp_postprocess = perf_counter_ns()
+
         # resulting sampleset
         result = dimod.SampleSet.from_samples(
             (samples, initial_states.variables),
             energy=energies + offset,
             vartype=dimod.SPIN,
             num_steps=num_steps,
         )
 
         result.change_vartype(original_vartype, inplace=True)
 
+        # Developer note: the specific keys of the timing dict are chosen to be consistent with
+        #                 other samplers' timing dict.
+        result.info.update(dict(timing=dict(
+            preprocessing_ns=timestamp_sample - timestamp_preprocess,
+            sampling_ns=timestamp_postprocess - timestamp_sample,
+            # Update timing info last to capture the full postprocessing time
+            postprocessing_ns=perf_counter_ns() - timestamp_postprocess,
+        )))
+
         return result
 
 
 SteepestDescentSampler = SteepestDescentSolver
```

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/greedy/src/descent.cpp` & `dwave-samplers-1.1.0/dwave/samplers/greedy/src/descent.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 //
 // Unless required by applicable law or agreed to in writing, software
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
+#include <cstdint>
 #include <vector>
 #include <set>
 #include <cassert>
 #include <stdexcept>
 #include "descent.h"
 
 using std::vector;
@@ -33,15 +34,15 @@
 // @param neighbour_couplings same as neighbors, but instead has the J value.
 //     neighbour_couplings[i][j] is the J value or weight on the coupling
 //     between variables i and neighbors[i][j]. 
 //
 // @return delta energy
 double get_flip_energy(
     int var,
-    char *state,
+    std::int8_t *state,
     const vector<double>& linear_biases,
     const vector<vector<int>>& neighbors,
     const vector<vector<double>>& neighbour_couplings
 ) {
     // var -1 flips to +1 => delta is +2
     // var +1 flips to -1 => delta is -2
     double delta = -2 * state[var];
@@ -55,27 +56,27 @@
 
     return delta * contrib;
 }
 
 
 // Returns the energy of a given state for the input problem.
 //
-// @param state a char array containing the spin state to compute the energy of
+// @param state a int8 array containing the spin state to compute the energy of
 // @param linear_biases vector of h or field value on each variable
 // @param coupler_starts an int vector containing the variables of one side of
 //        each coupler in the problem
 // @param coupler_ends an int vector containing the variables of the other side 
 //        of each coupler in the problem
 // @param coupler_weights a double vector containing the weights of the 
 //        couplers in the same order as coupler_starts and coupler_ends
 //
 // @return A double corresponding to the energy for `state` on the problem
 //        defined by linear_biases and the couplers passed in
 double get_state_energy(
-    char* state,
+    std::int8_t* state,
     const vector<double>& linear_biases,
     const vector<int>& coupler_starts,
     const vector<int>& coupler_ends,
     const vector<double>& coupler_weights
 ) {
     double energy = 0.0;
 
@@ -94,29 +95,29 @@
 
 
 // One run of the steepest gradient descent on the input Ising model.
 //
 // Linear search for the steepest descent variable. Fastest approach for
 // complete and/or dense problem graphs.
 //
-// @param state a signed char array where each char holds the state of a
+// @param state a int8 array where each int8 holds the state of a
 //        variable. Note that this will be used as the initial state of the
 //        run.
 // @param linear_biases vector of h or field value on each variable
 // @param neighbors lists of the neighbors of each variable, such that
 //        neighbors[i][j] is the jth neighbor of variable i. Note
 // @param neighbour_couplings same as neighbors, but instead has the J value.
 //        neighbour_couplings[i][j] is the J value or weight on the coupling
 //        between variables i and neighbors[i][j].
 // @param flip_energies vector used for caching of variable flip delta
 //        energies
 //
 // @return number of downhill steps; `state` contains the result of the run.
 unsigned int steepest_gradient_descent_solver(
-    char* state,
+    std::int8_t* state,
     const vector<double>& linear_biases,
     const vector<vector<int>>& neighbors,
     const vector<vector<double>>& neighbour_couplings,
     vector<double>& flip_energies
 ) {
     const int num_vars = linear_biases.size();
 
@@ -199,29 +200,29 @@
 // One run of the steepest gradient descent on the input Ising model.
 //
 // Flip energies are kept in an ordered set (balanced binary tree) resulting in
 // faster steepest descent variable lookup, but higher constant overhead of
 // maintaining the order. Scaling advantage only for very *large* (and *sparse*)
 // problem graphs.
 //
-// @param state a signed char array where each char holds the state of a
+// @param state a int8 array where each int8 holds the state of a
 //        variable. Note that this will be used as the initial state of the
 //        run.
 // @param linear_biases vector of h or field value on each variable
 // @param neighbors lists of the neighbors of each variable, such that
 //        neighbors[i][j] is the jth neighbor of variable i. Note
 // @param neighbour_couplings same as neighbors, but instead has the J value.
 //        neighbour_couplings[i][j] is the J value or weight on the coupling
 //        between variables i and neighbors[i][j].
 // @param flip_energies_vector vector used for caching of variable flip delta
 //        energies
 //
 // @return number of downhill steps; `state` contains the result of the run.
 unsigned int steepest_gradient_descent_ls_solver(
-    char* state,
+    std::int8_t* state,
     const vector<double>& linear_biases,
     const vector<vector<int>>& neighbors,
     const vector<vector<double>>& neighbour_couplings,
     vector<double>& flip_energies_vector
 ) {
     const int num_vars = linear_biases.size();
 
@@ -307,15 +308,15 @@
 
     return steps;
 }
 
 
 // Perform `num_samples` runs of steepest gradient descent on a general problem.
 //
-// @param states char array of size num_samples * number of variables in the
+// @param states int8 array of size num_samples * number of variables in the
 //        problem. Will be overwritten by this function as samples are filled
 //        in. The initial state of the samples are used to seed the gradient
 //        descent runs.
 // @param energies a double array of size num_samples. Will be overwritten by
 //        this function as energies are filled in.
 // @param steps an unsigned int array of size num_samples. Will be overwritten
 //        by this function as number of downhill steps per sample are received.
@@ -328,15 +329,15 @@
 // @param coupler_weights a double vector containing the weights of the couplers
 //        in the same order as coupler_starts and coupler_ends
 // @param large_sparse_opt boolean that determines
 //        if linear search or balanced tree search should be used for descent.
 //
 // @return Nothing. Results are in `states` buffer.
 void steepest_gradient_descent(
-    char* states,
+    std::int8_t* states,
     double* energies,
     unsigned* num_steps,
     const int num_samples,
     const vector<double>& linear_biases,
     const vector<int>& coupler_starts,
     const vector<int>& coupler_ends,
     const vector<double>& coupler_weights,
@@ -379,15 +380,15 @@
     // variable flip energies cache
     vector<double> flip_energies_vector(num_vars);
 
     // run the steepest descent for `num_samples` times,
     // each time seeded with the initial state from `states`
     for (int sample = 0; sample < num_samples; sample++) {
         // get initial state from states buffer; the solution overwrites the same buffer
-        char *state = states + sample * num_vars;
+        std::int8_t *state = states + sample * num_vars;
 
         if (large_sparse_opt) {
             num_steps[sample] = steepest_gradient_descent_ls_solver(
                 state, linear_biases, neighbors, neighbour_couplings, flip_energies_vector
             );
         } else {
             num_steps[sample] = steepest_gradient_descent_solver(
```

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/greedy/src/descent.h` & `dwave-samplers-1.1.0/dwave/samplers/greedy/src/descent.h`

 * *Files 14% similar despite different names*

```diff
@@ -11,51 +11,52 @@
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
 #ifndef _DESCENT_H
 #define _DESCENT_H
 
+#include <cstdint>
 #include <vector>
 
 using std::vector;
 
 
 double get_flip_energy(
     int var,
-    char *state,
+    std::int8_t *state,
     const vector<double>& linear_biases,
     const vector<vector<int>>& neighbors,
     const vector<vector<double>>& neighbour_couplings
 );
 
 double get_state_energy(
-    char* state,
+    std::int8_t* state,
     const vector<double>& linear_biases,
     const vector<int>& coupler_starts,
     const vector<int>& coupler_ends,
     const vector<double>& coupler_weights
 );
 
 unsigned steepest_gradient_descent_solver(
-    char* state,
+    std::int8_t* state,
     const vector<double>& linear_biases,
     const vector<vector<int>>& neighbors,
     const vector<vector<double>>& neighbour_couplings
 );
 
 unsigned steepest_gradient_descent_ls_solver(
-    char* state,
+    std::int8_t* state,
     const vector<double>& linear_biases,
     const vector<vector<int>>& neighbors,
     const vector<vector<double>>& neighbour_couplings
 );
 
 void steepest_gradient_descent(
-    char* states,
+    std::int8_t* states,
     double* energies,
     unsigned* num_steps,
     const int num_samples,
     const vector<double>& linear_biases,
     const vector<int>& coupler_starts,
     const vector<int>& coupler_ends,
     const vector<double>& coupler_weights,
```

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/planar/__init__.py` & `dwave-samplers-1.1.0/dwave/samplers/planar/__init__.py`

 * *Files identical despite different names*

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/planar/planar.py` & `dwave-samplers-1.1.0/dwave/samplers/planar/planar.py`

 * *Files identical despite different names*

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/planar/sampler.py` & `dwave-samplers-1.1.0/dwave/samplers/planar/sampler.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,31 +35,31 @@
         self.parameters = copy.deepcopy(self.parameters)
         self.properties = copy.deepcopy(self.properties)
 
     def sample(self,
                bqm: dimod.BinaryQuadraticModel,
                pos: typing.Optional[typing.Mapping[dimod.typing.Variable, typing.Tuple[float, float]]] = None,
                **kwargs) -> dimod.SampleSet:
-        """Sample from a binary quadratic model.
+        """Find a ground state of a planar Ising problem without linear biases.
 
         Args:
-            bqm: Binary quadratic model to be sampled.
-            pos: Position for each node
+            bqm: Binary quadratic model representing a planar Ising model with no linear biases.
+            pos: Position for each node as a dict of form ``{node: (x-coordinate, y-coordinate),...}``.
 
         Examples:
             >>> import dimod
             >>> from dwave.samplers.planar import PlanarGraphSolver
             >>> bqm = dimod.BinaryQuadraticModel.empty(dimod.SPIN)
             >>> bqm.add_interaction('a', 'b', +1.0)
             >>> bqm.add_interaction('b', 'c', +1.0)
             >>> bqm.add_interaction('c', 'a', +1.0)
             >>> pos = {'a': (0, 0), 'b': (1, 0), 'c': (0, 1)}
             >>> sample = PlanarGraphSolver().sample(bqm, pos)
             >>> sample.first
-            Sample(sample={'a': 1, 'b': -1, 'c': -1}, energy=0, num_occurrences=1)
+            Sample(sample={'a': 1, 'b': -1, 'c': -1}, energy=-1.0, num_occurrences=1)
 
         """
 
         if len(bqm) < 3:
             raise ValueError("The provided BQM must have at least three variables")
 
         G, off = bqm_to_multigraph(bqm)
@@ -85,16 +85,15 @@
 
         cut = _dual_matching_to_cut(G, matching)
         state = _cut_to_state(G, cut)
 
         if bqm.vartype is not dimod.BINARY:
             state = {v: 2 * b - 1 for v, b in state.items()}
 
-        ret = dimod.SampleSet.from_samples(state, bqm.vartype, 0)
-        return ret
+        return dimod.SampleSet.from_samples_bqm(state, bqm)
 
 
 def _determine_pos(G: nx.MultiGraph) -> dict:
     is_planar, P = nx.check_planarity(G)
     if not is_planar:
         raise ValueError("The provided BQM does not yield a planar embedding")
```

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/planar/util.py` & `dwave-samplers-1.1.0/dwave/samplers/planar/util.py`

 * *Files identical despite different names*

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/random/__init__.py` & `dwave-samplers-1.1.0/dwave/samplers/random/__init__.py`

 * *Files identical despite different names*

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/random/cyrandom.cpp` & `dwave-samplers-1.1.0/dwave/samplers/random/cyrandom.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -731,17 +731,14 @@
 
     #endif
     
 #include <vector>
 #include <string.h>
 #include <stdio.h>
 #include "numpy/arrayobject.h"
-#include "numpy/ndarrayobject.h"
-#include "numpy/ndarraytypes.h"
-#include "numpy/arrayscalars.h"
 #include "numpy/ufuncobject.h"
 
     /* NumPy API declarations from "numpy/__init__.pxd" */
     
 #include "dimod/vartypes.h"
 #include "dimod/abc.h"
 #include "dimod/binary_quadratic_model.h"
@@ -1111,195 +1108,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":690
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":691
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":692
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":693
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":697
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":698
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":699
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":700
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":704
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":705
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":714
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":715
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":716
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":718
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":719
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":720
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":722
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":723
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":725
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":726
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":727
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1382,42 +1379,42 @@
 struct __pyx_obj_5dimod_9quadratic_4cyqm_12cyqm_float64_cyQM_template;
 struct __pyx_obj_5dimod_9quadratic_4cyqm_12cyqm_float64_cyQM_float64;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":729
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":730
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":731
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":733
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -1527,15 +1524,15 @@
  *     cdef readonly tuple spawn_key
  */
 struct __pyx_obj_5numpy_6random_13bit_generator_SeedSequence {
   PyObject_HEAD
   struct __pyx_vtabstruct_5numpy_6random_13bit_generator_SeedSequence *__pyx_vtab;
   PyObject *entropy;
   PyObject *spawn_key;
-  Py_ssize_t pool_size;
+  uint32_t pool_size;
   PyObject *pool;
   uint32_t n_children_spawned;
 };
 
 
 /* "numpy/random/bit_generator.pxd":34
  *     cdef get_assembled_entropy(self)
@@ -2939,24 +2936,14 @@
 /* Module declarations from 'numpy.random' */
 
 /* Module declarations from 'numpy' */
 static PyTypeObject *__pyx_ptype_5numpy_dtype = 0;
 static PyTypeObject *__pyx_ptype_5numpy_flatiter = 0;
 static PyTypeObject *__pyx_ptype_5numpy_broadcast = 0;
 static PyTypeObject *__pyx_ptype_5numpy_ndarray = 0;
-static PyTypeObject *__pyx_ptype_5numpy_generic = 0;
-static PyTypeObject *__pyx_ptype_5numpy_number = 0;
-static PyTypeObject *__pyx_ptype_5numpy_integer = 0;
-static PyTypeObject *__pyx_ptype_5numpy_signedinteger = 0;
-static PyTypeObject *__pyx_ptype_5numpy_unsignedinteger = 0;
-static PyTypeObject *__pyx_ptype_5numpy_inexact = 0;
-static PyTypeObject *__pyx_ptype_5numpy_floating = 0;
-static PyTypeObject *__pyx_ptype_5numpy_complexfloating = 0;
-static PyTypeObject *__pyx_ptype_5numpy_flexible = 0;
-static PyTypeObject *__pyx_ptype_5numpy_character = 0;
 static PyTypeObject *__pyx_ptype_5numpy_ufunc = 0;
 
 /* Module declarations from 'dimod.cyvariables' */
 static PyTypeObject *__pyx_ptype_5dimod_11cyvariables_cyVariables = 0;
 
 /* Module declarations from 'dimod.libcpp.vartypes' */
 
@@ -4570,15 +4557,15 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_sample_view, 1);
   __Pyx_XDECREF(__pyx_v_sampleset);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":735
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -4587,29 +4574,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":736
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 736, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":735
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -4620,15 +4607,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":738
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -4637,29 +4624,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":739
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 739, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":738
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -4670,15 +4657,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":741
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -4687,29 +4674,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":742
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 742, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":741
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -4720,15 +4707,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":744
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -4737,29 +4724,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":745
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 745, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":744
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -4770,15 +4757,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":747
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -4787,29 +4774,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":748
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 748, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":747
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -4820,212 +4807,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":750
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":751
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":752
+    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":751
+    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":754
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":750
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":929
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":868
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":930
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":869
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":931
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":870
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":929
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":868
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":933
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":872
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":934
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":873
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":935
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":874
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":936
+    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":875
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":935
+    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":874
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":937
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":876
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":933
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":872
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":941
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":880
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -5041,15 +5028,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":942
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":881
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -5057,84 +5044,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":943
+      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":882
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 943, __pyx_L3_error)
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 882, __pyx_L3_error)
 
-      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":942
+      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":881
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":944
+    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":883
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 944, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 883, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":945
+      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":884
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 945, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 884, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 945, __pyx_L5_except_error)
+      __PYX_ERR(1, 884, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":942
+    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":881
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":941
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":880
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -5149,15 +5136,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":947
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":886
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5173,15 +5160,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":948
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":887
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -5189,84 +5176,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":949
+      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":888
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 949, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 888, __pyx_L3_error)
 
-      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":948
+      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":887
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":950
+    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":889
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 950, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 889, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":951
+      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":890
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 951, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 890, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 951, __pyx_L5_except_error)
+      __PYX_ERR(1, 890, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":948
+    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":887
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":947
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":886
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5281,15 +5268,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":953
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":892
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5305,15 +5292,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":954
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":893
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -5321,84 +5308,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":955
+      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":894
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 955, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 894, __pyx_L3_error)
 
-      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":954
+      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":893
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":956
+    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":895
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 956, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 895, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":957
+      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":896
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 957, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 896, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 957, __pyx_L5_except_error)
+      __PYX_ERR(1, 896, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":954
+    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":893
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":953
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":892
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5413,188 +5400,14 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":967
- * 
- * 
- * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
- *     """
- *     Cython equivalent of `isinstance(obj, np.timedelta64)`
- */
-
-static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
-
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":979
- *     bool
- *     """
- *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
-  goto __pyx_L0;
-
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":967
- * 
- * 
- * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
- *     """
- *     Cython equivalent of `isinstance(obj, np.timedelta64)`
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":982
- * 
- * 
- * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
- *     """
- *     Cython equivalent of `isinstance(obj, np.datetime64)`
- */
-
-static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("is_datetime64_object", 0);
-
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":994
- *     bool
- *     """
- *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
-  goto __pyx_L0;
-
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":982
- * 
- * 
- * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
- *     """
- *     Cython equivalent of `isinstance(obj, np.datetime64)`
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":997
- * 
- * 
- * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the int64 value underlying scalar numpy datetime64 object
- */
-
-static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
-  npy_datetime __pyx_r;
-
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":1004
- *     also needed.  That can be found using `get_datetime64_unit`.
- *     """
- *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
-  goto __pyx_L0;
-
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":997
- * 
- * 
- * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the int64 value underlying scalar numpy datetime64 object
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  return __pyx_r;
-}
-
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":1007
- * 
- * 
- * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the int64 value underlying scalar numpy timedelta64 object
- */
-
-static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
-  npy_timedelta __pyx_r;
-
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":1011
- *     returns the int64 value underlying scalar numpy timedelta64 object
- *     """
- *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
-  goto __pyx_L0;
-
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":1007
- * 
- * 
- * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the int64 value underlying scalar numpy timedelta64 object
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  return __pyx_r;
-}
-
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":1014
- * 
- * 
- * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the unit part of the dtype for a numpy datetime64 object.
- */
-
-static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
-  NPY_DATETIMEUNIT __pyx_r;
-
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":1018
- *     returns the unit part of the dtype for a numpy datetime64 object.
- *     """
- *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
- */
-  __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
-  goto __pyx_L0;
-
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":1014
- * 
- * 
- * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the unit part of the dtype for a numpy datetime64 object.
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  return __pyx_r;
-}
-
 /* "View.MemoryView":122
  *         cdef bint dtype_is_object
  * 
  *     def __cinit__(array self, tuple shape, Py_ssize_t itemsize, format not None,             # <<<<<<<<<<<<<<
  *                   mode="c", bint allocate_buffer=True):
  * 
  */
@@ -19522,15 +19335,15 @@
   {&__pyx_n_s_variables, __pyx_k_variables, sizeof(__pyx_k_variables), 0, 0, 1, 1},
   {&__pyx_n_s_vartype, __pyx_k_vartype, sizeof(__pyx_k_vartype), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 59, __pyx_L1_error)
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 88, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 945, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 884, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(2, 148, __pyx_L1_error)
   __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(2, 151, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(2, 2, __pyx_L1_error)
   __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(2, 404, __pyx_L1_error)
   __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(2, 613, __pyx_L1_error)
   __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(2, 832, __pyx_L1_error)
   return 0;
@@ -19593,33 +19406,33 @@
  * 
  *     cdef np.float64_t[:] energies_view = record['energy']
  */
   __pyx_slice__5 = PySlice_New(Py_None, Py_None, Py_None); if (unlikely(!__pyx_slice__5)) __PYX_ERR(0, 145, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_slice__5);
   __Pyx_GIVEREF(__pyx_slice__5);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":945
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":884
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(1, 945, __pyx_L1_error)
+  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(1, 884, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":951
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":890
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(1, 951, __pyx_L1_error)
+  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(1, 890, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__7);
   __Pyx_GIVEREF(__pyx_tuple__7);
 
   /* "View.MemoryView":133
  * 
  *         if not self.ndim:
  *             raise ValueError("Empty shape tuple for cython.array")             # <<<<<<<<<<<<<<
@@ -20021,46 +19834,26 @@
    if (!__pyx_ptype_5numpy_6random_13bit_generator_BitGenerator) __PYX_ERR(4, 14, __pyx_L1_error)
   __pyx_ptype_5numpy_6random_13bit_generator_SeedSequence = __Pyx_ImportType(__pyx_t_1, "numpy.random.bit_generator", "SeedSequence", sizeof(struct __pyx_obj_5numpy_6random_13bit_generator_SeedSequence), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_6random_13bit_generator_SeedSequence) __PYX_ERR(4, 23, __pyx_L1_error)
   __pyx_vtabptr_5numpy_6random_13bit_generator_SeedSequence = (struct __pyx_vtabstruct_5numpy_6random_13bit_generator_SeedSequence*)__Pyx_GetVtable(__pyx_ptype_5numpy_6random_13bit_generator_SeedSequence->tp_dict); if (unlikely(!__pyx_vtabptr_5numpy_6random_13bit_generator_SeedSequence)) __PYX_ERR(4, 23, __pyx_L1_error)
   __pyx_ptype_5numpy_6random_13bit_generator_SeedlessSequence = __Pyx_ImportType(__pyx_t_1, "numpy.random.bit_generator", "SeedlessSequence", sizeof(struct __pyx_obj_5numpy_6random_13bit_generator_SeedlessSequence), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_6random_13bit_generator_SeedlessSequence) __PYX_ERR(4, 34, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 200, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 200, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 199, __pyx_L1_error)
   __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 223, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 222, __pyx_L1_error)
   __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 227, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 226, __pyx_L1_error)
   __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 239, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 771, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 773, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 775, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 777, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 779, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 781, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 783, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 785, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 787, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 789, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
   __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 827, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 764, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("dimod.cyvariables"); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_5dimod_11cyvariables_cyVariables = __Pyx_ImportType(__pyx_t_1, "dimod.cyvariables", "cyVariables", sizeof(struct __pyx_obj_5dimod_11cyvariables_cyVariables), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5dimod_11cyvariables_cyVariables) __PYX_ERR(5, 20, __pyx_L1_error)
   __pyx_vtabptr_5dimod_11cyvariables_cyVariables = (struct __pyx_vtabstruct_5dimod_11cyvariables_cyVariables*)__Pyx_GetVtable(__pyx_ptype_5dimod_11cyvariables_cyVariables->tp_dict); if (unlikely(!__pyx_vtabptr_5dimod_11cyvariables_cyVariables)) __PYX_ERR(5, 20, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
```

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/random/cyrandom.pyx` & `dwave-samplers-1.1.0/dwave/samplers/random/cyrandom.pyx`

 * *Files identical despite different names*

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/random/sampler.py` & `dwave-samplers-1.1.0/dwave/samplers/random/sampler.py`

 * *Files identical despite different names*

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/sa/__init__.py` & `dwave-samplers-1.1.0/dwave/samplers/sa/__init__.py`

 * *Files identical despite different names*

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/sa/sampler.py` & `dwave-samplers-1.1.0/dwave/samplers/sa/sampler.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,20 +14,22 @@
 
 import math
 
 from numbers import Integral
 from numpy.random import randint
 from collections import defaultdict
 from typing import List, Sequence, Tuple, Optional, Union
+from time import perf_counter_ns
 try:
     from typing import Literal
     BetaScheduleType = Literal['linear', 'geometric', 'custom']
 except ImportError:
     BetaScheduleType = str
 
+    
 from dimod.core.initialized import InitialStateGenerator
 
 import dimod
 import numpy as np
 
 from dwave.samplers.sa.simulated_annealing import simulated_annealing
 
@@ -39,15 +41,15 @@
 class SimulatedAnnealingSampler(dimod.Sampler, dimod.Initialized):
     """Simulated annealing sampler for binary quadratic models.
 
     `Simulated annealing <https://en.wikipedia.org/wiki/Simulated_annealing>`_
     can be used for heuristic optimization or approximate Boltzmann sampling. This
     implementation approaches the equilibrium distribution by performing updates
     at a sequence of decreasing temperatures, terminating at the target
-    :math:`\\beta`.\ [#]_ Each spin is updated once in a fixed order per point
+    :math:`\\beta`.\ [#]_ By default each spin is updated once in a fixed order per point
     per :math:`\\beta` according to a Metropolis-Hastings update. When :math:`\\beta`
     is large the target distribution concentrates, at equilibrium, over ground
     states of the model. Samples are guaranteed to match the equilibrium for
     long, smooth :math:`\\beta` schedules.
 
     .. [#] :math:`\\beta` represents the inverse temperature, :math:`1/(k_B T)`,
        of a `Boltzmann distribution <https://en.wikipedia.org/wiki/Boltzmann_distribution>`_
@@ -132,18 +134,20 @@
     def sample(self, bqm: dimod.BinaryQuadraticModel,
                beta_range: Optional[Union[List[float], Tuple[float, float]]] = None,
                num_reads: Optional[int] = None,
                num_sweeps: Optional[int] = None,
                num_sweeps_per_beta: int = 1,
                beta_schedule_type: BetaScheduleType = "geometric",
                seed: Optional[int] = None,
-               interrupt_function=None,
+               interrupt_function = None,
                beta_schedule: Optional[Union[Sequence[float], np.ndarray]] = None,
                initial_states: Optional[dimod.typing.SamplesLike] = None,
                initial_states_generator: InitialStateGenerator = "random",
+               randomize_order: bool = False,
+               proposal_acceptance_criteria: str = 'Metropolis',
                **kwargs) -> dimod.SampleSet:
         """Sample from a binary quadratic model.
 
         Args:
             bqm: Binary quadratic model to be sampled.
 
             beta_range:
@@ -215,20 +219,57 @@
                     Reuses the specified initial states if fewer than
                     ``num_reads`` or truncates if greater.
 
                 * "random":
                     Expands the specified initial states with randomly generated
                     states if fewer than ``num_reads`` or truncates if greater.
 
+            randomize_order:
+                When `True`, each spin update selects a variable uniformly at random.
+                This method is ergodic, obeys detailed balance and preserves symmetries 
+                of the model.
+
+                When `False`, updates proceed sequentially through the labeled variables 
+                on each sweep so that all variables are updated once per sweep. This method:
+
+                * can be non-ergodic in special cases when used with ``proposal_acceptance_critera=="Metropolis"``.
+
+                * can introduce a dynamical bias as a function of variable order.
+
+                * has faster per spin update than the True method.
+
+            proposal_acceptance_criteria:
+                When "Gibbs", each spin flip proposal is accepted according
+                to the Gibbs criteria.
+                When "Metropolis", each spin flip proposal is accepted according
+                to the Metropolis-Hastings criteria.
+
             interrupt_function (function, optional):
                 A function called with no parameters between each sample of
                 simulated annealing. If the function returns True, simulated
                 annealing terminates and returns with all of the samples and
                 energies found so far.
 
+        Returns:
+            A `dimod.SampleSet` for the binary quadratic model.
+
+            The `info` field of the sample set contains information about the sampling procedure:
+            1. the beta range used,
+            2. the beta schedule type used, and
+            3. timing information (details below).
+
+            Timing information is categorized into three: preprocessing, sampling, and
+            postprocessing time. All timings are reported in units of nanoseconds.
+
+            Preprocessing time is the total time spent converting the BQM variable type (if
+            required), parsing input arguments, and determining an annealing schedule. Sampling time
+            is the total time the algorithm spent in sampling states of the binary quadratic model.
+            Postprocessing time is the total time spent reverting variable type and creating a
+            `dimod.SampleSet`.
+
         Examples:
             This example runs simulated annealing on a binary quadratic model
             with various input parameters.
 
             >>> import dimod
             >>> from dwave.samplers import SimulatedAnnealingSampler
             ...
@@ -251,14 +292,15 @@
 
             .. [#] :math:`\\beta` represents the inverse temperature, :math:`1/(k_B T)`, of a
                `Boltzmann distribution <https://en.wikipedia.org/wiki/Boltzmann_distribution>`_
                where :math:`T` is the thermodynamic temperature in kelvin and :math:`k_B` is
                Boltzmann's constant.
 
         """
+        timestamp_preprocess = perf_counter_ns()
         # get the original vartype so we can return consistently
         original_vartype = bqm.vartype
 
         # convert to spin (if needed)
         if bqm.vartype is not dimod.SPIN:
             bqm = bqm.change_vartype(dimod.SPIN, inplace=False)
 
@@ -356,33 +398,48 @@
                     if min(beta_range) <= 0:
                         error_msg = "'beta_range' must contain non-zero values for 'beta_schedule_type' = 'geometric'"
                         raise ValueError(error_msg)
                     # interpolate a geometric beta schedule
                     beta_schedule = np.geomspace(*beta_range, num=num_betas)
                 else:
                     raise ValueError("Beta schedule type {} not implemented".format(beta_schedule_type))
+
+        timestamp_sample = perf_counter_ns()
+
         # run the simulated annealing algorithm
         samples, energies = simulated_annealing(
             num_reads, ldata, irow, icol, qdata,
             num_sweeps_per_beta, beta_schedule,
-            seed, initial_states_array, interrupt_function)
+            seed, initial_states_array,
+            randomize_order, proposal_acceptance_criteria,
+            interrupt_function)
+        timestamp_postprocess = perf_counter_ns()
 
         info = {
             "beta_range": beta_range,
             "beta_schedule_type": beta_schedule_type
         }
         response = dimod.SampleSet.from_samples(
             (samples, variable_order),
             energy=energies+bqm.offset,  # add back in the offset
             info=info,
             vartype=dimod.SPIN
         )
 
         response.change_vartype(original_vartype, inplace=True)
 
+        # Developer note: the specific keys of the timing dict are chosen to be consistent with
+        #                 other samplers' timing dict.
+        response.info.update(dict(timing=dict(
+            preprocessing_ns=timestamp_sample - timestamp_preprocess,
+            sampling_ns=timestamp_postprocess - timestamp_sample,
+            # Update timing info last to capture the full postprocessing time
+            postprocessing_ns=perf_counter_ns() - timestamp_postprocess,
+        )))
+
         return response
 
 
 Neal = SimulatedAnnealingSampler
 
 
 def _default_ising_beta_range(h, J,
@@ -433,15 +490,14 @@
     We use an approximation to the minimum bias per spin to give a lower bound on the minimum
     energy gap, such that for the final sweeps states are highly unlikely to excite away from
     a global (or local) minimum.
     """
     if not 0 < max_single_qubit_excitation_rate < 1:
         raise ValueError('Targeted single qubit excitations rates must be in range (0,1)')
 
-
     # Approximate worst and best cases of the [non-zero] energy signal (effective field)
     # experienced per spin as function of neighbors: bias = h_i + sum_j Jij s_j:
     sum_abs_bias_dict = defaultdict(int, {k: abs(v) for k, v in h.items()})
     if sum_abs_bias_dict:
         min_abs_bias_dict = {k: v for k, v in sum_abs_bias_dict.items() if v != 0}
     else:
         min_abs_bias_dict = {}
```

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/sa/simulated_annealing.cpp` & `dwave-samplers-1.1.0/dwave/samplers/sa/simulated_annealing.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -720,17 +720,14 @@
 #include "new"
 #include "stdexcept"
 #include "typeinfo"
 #include <vector>
 #include <string.h>
 #include <stdio.h>
 #include "numpy/arrayobject.h"
-#include "numpy/ndarrayobject.h"
-#include "numpy/ndarraytypes.h"
-#include "numpy/arrayscalars.h"
 #include "numpy/ufuncobject.h"
 
     /* NumPy API declarations from "numpy/__init__.pxd" */
     
 #include "cpu_sa.h"
 #include "pythread.h"
 #include <stdlib.h>
@@ -1076,195 +1073,195 @@
 
 /* ForceInitThreads.proto */
 #ifndef __PYX_FORCE_INIT_THREADS
   #define __PYX_FORCE_INIT_THREADS 0
 #endif
 
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":690
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":691
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":692
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":693
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":697
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":698
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":699
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":700
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":704
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":705
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":714
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":715
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":716
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":718
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":719
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":720
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":722
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":723
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":725
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":726
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":727
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1295,42 +1292,42 @@
 
 /*--- Type declarations ---*/
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":729
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":730
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":731
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":733
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -1520,14 +1517,24 @@
 #define __Pyx_DECREF_SET(r, v) do {\
         PyObject *tmp = (PyObject *) r;\
         r = v; __Pyx_DECREF(tmp);\
     } while (0)
 #define __Pyx_CLEAR(r)    do { PyObject* tmp = ((PyObject*)(r)); r = NULL; __Pyx_DECREF(tmp);} while(0)
 #define __Pyx_XCLEAR(r)   do { if((r) != NULL) {PyObject* tmp = ((PyObject*)(r)); r = NULL; __Pyx_DECREF(tmp);}} while(0)
 
+/* PyObjectGetAttrStr.proto */
+#if CYTHON_USE_TYPE_SLOTS
+static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStr(PyObject* obj, PyObject* attr_name);
+#else
+#define __Pyx_PyObject_GetAttrStr(o,n) PyObject_GetAttr(o,n)
+#endif
+
+/* GetBuiltinName.proto */
+static PyObject *__Pyx_GetBuiltinName(PyObject *name);
+
 /* RaiseArgTupleInvalid.proto */
 static void __Pyx_RaiseArgtupleInvalid(const char* func_name, int exact,
     Py_ssize_t num_min, Py_ssize_t num_max, Py_ssize_t num_found);
 
 /* RaiseDoubleKeywords.proto */
 static void __Pyx_RaiseDoubleKeywordsError(const char* func_name, PyObject* kw_name);
 
@@ -1562,24 +1569,14 @@
 static CYTHON_INLINE void __Pyx_SafeReleaseBuffer(Py_buffer* info);
 static Py_ssize_t __Pyx_minusones[] = { -1, -1, -1, -1, -1, -1, -1, -1 };
 static Py_ssize_t __Pyx_zeros[] = { 0, 0, 0, 0, 0, 0, 0, 0 };
 
 /* PyIntCompare.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_EqObjC(PyObject *op1, PyObject *op2, long intval, long inplace);
 
-/* PyObjectGetAttrStr.proto */
-#if CYTHON_USE_TYPE_SLOTS
-static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStr(PyObject* obj, PyObject* attr_name);
-#else
-#define __Pyx_PyObject_GetAttrStr(o,n) PyObject_GetAttr(o,n)
-#endif
-
-/* GetBuiltinName.proto */
-static PyObject *__Pyx_GetBuiltinName(PyObject *name);
-
 /* PyDictVersioning.proto */
 #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
 #define __PYX_DICT_VERSION_INIT  ((PY_UINT64_T) -1)
 #define __PYX_GET_DICT_VERSION(dict)  (((PyDictObject*)(dict))->ma_version_tag)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)\
     (version_var) = __PYX_GET_DICT_VERSION(dict);\
     (cache_var) = (value);
@@ -1630,14 +1627,131 @@
 #define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
 #endif
 
 /* BufferIndexError.proto */
 static void __Pyx_RaiseBufferIndexError(int axis);
 
 #define __Pyx_BufPtrCContig2d(type, buf, i0, s0, i1, s1) ((type)((char*)buf + i0 * s0) + i1)
+/* PyFunctionFastCall.proto */
+#if CYTHON_FAST_PYCALL
+#define __Pyx_PyFunction_FastCall(func, args, nargs)\
+    __Pyx_PyFunction_FastCallDict((func), (args), (nargs), NULL)
+#if 1 || PY_VERSION_HEX < 0x030600B1
+static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs);
+#else
+#define __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs) _PyFunction_FastCallDict(func, args, nargs, kwargs)
+#endif
+#define __Pyx_BUILD_ASSERT_EXPR(cond)\
+    (sizeof(char [1 - 2*!(cond)]) - 1)
+#ifndef Py_MEMBER_SIZE
+#define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
+#endif
+#if CYTHON_FAST_PYCALL
+  static size_t __pyx_pyframe_localsplus_offset = 0;
+  #include "frameobject.h"
+  #define __Pxy_PyFrame_Initialize_Offsets()\
+    ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
+     (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
+  #define __Pyx_PyFrame_GetLocalsplus(frame)\
+    (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
+#endif // CYTHON_FAST_PYCALL
+#endif
+
+/* PyObjectCallMethO.proto */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg);
+#endif
+
+/* PyObjectCallNoArg.proto */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func);
+#else
+#define __Pyx_PyObject_CallNoArg(func) __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL)
+#endif
+
+/* PyCFunctionFastCall.proto */
+#if CYTHON_FAST_PYCCALL
+static CYTHON_INLINE PyObject *__Pyx_PyCFunction_FastCall(PyObject *func, PyObject **args, Py_ssize_t nargs);
+#else
+#define __Pyx_PyCFunction_FastCall(func, args, nargs)  (assert(0), NULL)
+#endif
+
+/* PyObjectCallOneArg.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg);
+
+/* IncludeStringH.proto */
+#include <string.h>
+
+/* BytesEquals.proto */
+static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals);
+
+/* UnicodeEquals.proto */
+static CYTHON_INLINE int __Pyx_PyUnicode_Equals(PyObject* s1, PyObject* s2, int equals);
+
+/* PyObjectFormatSimple.proto */
+#if CYTHON_COMPILING_IN_PYPY
+    #define __Pyx_PyObject_FormatSimple(s, f) (\
+        likely(PyUnicode_CheckExact(s)) ? (Py_INCREF(s), s) :\
+        PyObject_Format(s, f))
+#elif PY_MAJOR_VERSION < 3
+    #define __Pyx_PyObject_FormatSimple(s, f) (\
+        likely(PyUnicode_CheckExact(s)) ? (Py_INCREF(s), s) :\
+        likely(PyString_CheckExact(s)) ? PyUnicode_FromEncodedObject(s, NULL, "strict") :\
+        PyObject_Format(s, f))
+#elif CYTHON_USE_TYPE_SLOTS
+    #define __Pyx_PyObject_FormatSimple(s, f) (\
+        likely(PyUnicode_CheckExact(s)) ? (Py_INCREF(s), s) :\
+        likely(PyLong_CheckExact(s)) ? PyLong_Type.tp_str(s) :\
+        likely(PyFloat_CheckExact(s)) ? PyFloat_Type.tp_str(s) :\
+        PyObject_Format(s, f))
+#else
+    #define __Pyx_PyObject_FormatSimple(s, f) (\
+        likely(PyUnicode_CheckExact(s)) ? (Py_INCREF(s), s) :\
+        PyObject_Format(s, f))
+#endif
+
+/* PyThreadStateGet.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_PyThreadState_declare  PyThreadState *__pyx_tstate;
+#define __Pyx_PyThreadState_assign  __pyx_tstate = __Pyx_PyThreadState_Current;
+#define __Pyx_PyErr_Occurred()  __pyx_tstate->curexc_type
+#else
+#define __Pyx_PyThreadState_declare
+#define __Pyx_PyThreadState_assign
+#define __Pyx_PyErr_Occurred()  PyErr_Occurred()
+#endif
+
+/* PyErrFetchRestore.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_PyErr_Clear() __Pyx_ErrRestore(NULL, NULL, NULL)
+#define __Pyx_ErrRestoreWithState(type, value, tb)  __Pyx_ErrRestoreInState(PyThreadState_GET(), type, value, tb)
+#define __Pyx_ErrFetchWithState(type, value, tb)    __Pyx_ErrFetchInState(PyThreadState_GET(), type, value, tb)
+#define __Pyx_ErrRestore(type, value, tb)  __Pyx_ErrRestoreInState(__pyx_tstate, type, value, tb)
+#define __Pyx_ErrFetch(type, value, tb)    __Pyx_ErrFetchInState(__pyx_tstate, type, value, tb)
+static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
+static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
+#if CYTHON_COMPILING_IN_CPYTHON
+#define __Pyx_PyErr_SetNone(exc) (Py_INCREF(exc), __Pyx_ErrRestore((exc), NULL, NULL))
+#else
+#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
+#endif
+#else
+#define __Pyx_PyErr_Clear() PyErr_Clear()
+#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
+#define __Pyx_ErrRestoreWithState(type, value, tb)  PyErr_Restore(type, value, tb)
+#define __Pyx_ErrFetchWithState(type, value, tb)  PyErr_Fetch(type, value, tb)
+#define __Pyx_ErrRestoreInState(tstate, type, value, tb)  PyErr_Restore(type, value, tb)
+#define __Pyx_ErrFetchInState(tstate, type, value, tb)  PyErr_Fetch(type, value, tb)
+#define __Pyx_ErrRestore(type, value, tb)  PyErr_Restore(type, value, tb)
+#define __Pyx_ErrFetch(type, value, tb)  PyErr_Fetch(type, value, tb)
+#endif
+
+/* RaiseException.proto */
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
+
 /* GetItemInt.proto */
 #define __Pyx_GetItemInt(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
     (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
     __Pyx_GetItemInt_Fast(o, (Py_ssize_t)i, is_list, wraparound, boundscheck) :\
     (is_list ? (PyErr_SetString(PyExc_IndexError, "list index out of range"), (PyObject*)NULL) :\
                __Pyx_GetItemInt_Generic(o, to_py_func(i))))
 #define __Pyx_GetItemInt_List(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
@@ -1691,97 +1805,14 @@
 #define __pyx_get_slice_count_pointer(memview) (memview->acquisition_count_aligned_p)
 #define __pyx_get_slice_count(memview) (*__pyx_get_slice_count_pointer(memview))
 #define __PYX_INC_MEMVIEW(slice, have_gil) __Pyx_INC_MEMVIEW(slice, have_gil, __LINE__)
 #define __PYX_XDEC_MEMVIEW(slice, have_gil) __Pyx_XDEC_MEMVIEW(slice, have_gil, __LINE__)
 static CYTHON_INLINE void __Pyx_INC_MEMVIEW(__Pyx_memviewslice *, int, int);
 static CYTHON_INLINE void __Pyx_XDEC_MEMVIEW(__Pyx_memviewslice *, int, int);
 
-/* PyThreadStateGet.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_PyThreadState_declare  PyThreadState *__pyx_tstate;
-#define __Pyx_PyThreadState_assign  __pyx_tstate = __Pyx_PyThreadState_Current;
-#define __Pyx_PyErr_Occurred()  __pyx_tstate->curexc_type
-#else
-#define __Pyx_PyThreadState_declare
-#define __Pyx_PyThreadState_assign
-#define __Pyx_PyErr_Occurred()  PyErr_Occurred()
-#endif
-
-/* PyErrFetchRestore.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_PyErr_Clear() __Pyx_ErrRestore(NULL, NULL, NULL)
-#define __Pyx_ErrRestoreWithState(type, value, tb)  __Pyx_ErrRestoreInState(PyThreadState_GET(), type, value, tb)
-#define __Pyx_ErrFetchWithState(type, value, tb)    __Pyx_ErrFetchInState(PyThreadState_GET(), type, value, tb)
-#define __Pyx_ErrRestore(type, value, tb)  __Pyx_ErrRestoreInState(__pyx_tstate, type, value, tb)
-#define __Pyx_ErrFetch(type, value, tb)    __Pyx_ErrFetchInState(__pyx_tstate, type, value, tb)
-static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
-static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
-#if CYTHON_COMPILING_IN_CPYTHON
-#define __Pyx_PyErr_SetNone(exc) (Py_INCREF(exc), __Pyx_ErrRestore((exc), NULL, NULL))
-#else
-#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
-#endif
-#else
-#define __Pyx_PyErr_Clear() PyErr_Clear()
-#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
-#define __Pyx_ErrRestoreWithState(type, value, tb)  PyErr_Restore(type, value, tb)
-#define __Pyx_ErrFetchWithState(type, value, tb)  PyErr_Fetch(type, value, tb)
-#define __Pyx_ErrRestoreInState(tstate, type, value, tb)  PyErr_Restore(type, value, tb)
-#define __Pyx_ErrFetchInState(tstate, type, value, tb)  PyErr_Fetch(type, value, tb)
-#define __Pyx_ErrRestore(type, value, tb)  PyErr_Restore(type, value, tb)
-#define __Pyx_ErrFetch(type, value, tb)  PyErr_Fetch(type, value, tb)
-#endif
-
-/* PyFunctionFastCall.proto */
-#if CYTHON_FAST_PYCALL
-#define __Pyx_PyFunction_FastCall(func, args, nargs)\
-    __Pyx_PyFunction_FastCallDict((func), (args), (nargs), NULL)
-#if 1 || PY_VERSION_HEX < 0x030600B1
-static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs);
-#else
-#define __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs) _PyFunction_FastCallDict(func, args, nargs, kwargs)
-#endif
-#define __Pyx_BUILD_ASSERT_EXPR(cond)\
-    (sizeof(char [1 - 2*!(cond)]) - 1)
-#ifndef Py_MEMBER_SIZE
-#define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
-#endif
-#if CYTHON_FAST_PYCALL
-  static size_t __pyx_pyframe_localsplus_offset = 0;
-  #include "frameobject.h"
-  #define __Pxy_PyFrame_Initialize_Offsets()\
-    ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
-     (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
-  #define __Pyx_PyFrame_GetLocalsplus(frame)\
-    (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
-#endif // CYTHON_FAST_PYCALL
-#endif
-
-/* PyObjectCallMethO.proto */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg);
-#endif
-
-/* PyObjectCallNoArg.proto */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func);
-#else
-#define __Pyx_PyObject_CallNoArg(func) __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL)
-#endif
-
-/* PyCFunctionFastCall.proto */
-#if CYTHON_FAST_PYCCALL
-static CYTHON_INLINE PyObject *__Pyx_PyCFunction_FastCall(PyObject *func, PyObject **args, Py_ssize_t nargs);
-#else
-#define __Pyx_PyCFunction_FastCall(func, args, nargs)  (assert(0), NULL)
-#endif
-
-/* PyObjectCallOneArg.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg);
-
 /* GetTopmostException.proto */
 #if CYTHON_USE_EXC_INFO_STACK
 static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
 #endif
 
 /* SaveResetException.proto */
 #if CYTHON_FAST_THREAD_STATE
@@ -1811,29 +1842,17 @@
 #endif
 
 /* WriteUnraisableException.proto */
 static void __Pyx_WriteUnraisable(const char *name, int clineno,
                                   int lineno, const char *filename,
                                   int full_traceback, int nogil);
 
-/* RaiseException.proto */
-static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
-
 /* PyObjectCall2Args.proto */
 static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2);
 
-/* IncludeStringH.proto */
-#include <string.h>
-
-/* BytesEquals.proto */
-static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals);
-
-/* UnicodeEquals.proto */
-static CYTHON_INLINE int __Pyx_PyUnicode_Equals(PyObject* s1, PyObject* s2, int equals);
-
 /* StrEquals.proto */
 #if PY_MAJOR_VERSION >= 3
 #define __Pyx_PyString_Equals __Pyx_PyUnicode_Equals
 #else
 #define __Pyx_PyString_Equals __Pyx_PyBytes_Equals
 #endif
 
@@ -2258,24 +2277,14 @@
 /* Module declarations from 'numpy' */
 
 /* Module declarations from 'numpy' */
 static PyTypeObject *__pyx_ptype_5numpy_dtype = 0;
 static PyTypeObject *__pyx_ptype_5numpy_flatiter = 0;
 static PyTypeObject *__pyx_ptype_5numpy_broadcast = 0;
 static PyTypeObject *__pyx_ptype_5numpy_ndarray = 0;
-static PyTypeObject *__pyx_ptype_5numpy_generic = 0;
-static PyTypeObject *__pyx_ptype_5numpy_number = 0;
-static PyTypeObject *__pyx_ptype_5numpy_integer = 0;
-static PyTypeObject *__pyx_ptype_5numpy_signedinteger = 0;
-static PyTypeObject *__pyx_ptype_5numpy_unsignedinteger = 0;
-static PyTypeObject *__pyx_ptype_5numpy_inexact = 0;
-static PyTypeObject *__pyx_ptype_5numpy_floating = 0;
-static PyTypeObject *__pyx_ptype_5numpy_complexfloating = 0;
-static PyTypeObject *__pyx_ptype_5numpy_flexible = 0;
-static PyTypeObject *__pyx_ptype_5numpy_character = 0;
 static PyTypeObject *__pyx_ptype_5numpy_ufunc = 0;
 
 /* Module declarations from 'dwave.samplers.sa.simulated_annealing' */
 static PyTypeObject *__pyx_array_type = 0;
 static PyTypeObject *__pyx_MemviewEnum_type = 0;
 static PyTypeObject *__pyx_memoryview_type = 0;
 static PyTypeObject *__pyx_memoryviewslice_type = 0;
@@ -2318,23 +2327,23 @@
 static void __pyx_memoryview_broadcast_leading(__Pyx_memviewslice *, int, int); /*proto*/
 static void __pyx_memoryview_refcount_copying(__Pyx_memviewslice *, int, int, int); /*proto*/
 static void __pyx_memoryview_refcount_objects_in_slice_with_gil(char *, Py_ssize_t *, Py_ssize_t *, int, int); /*proto*/
 static void __pyx_memoryview_refcount_objects_in_slice(char *, Py_ssize_t *, Py_ssize_t *, int, int); /*proto*/
 static void __pyx_memoryview_slice_assign_scalar(__Pyx_memviewslice *, int, size_t, void *, int); /*proto*/
 static void __pyx_memoryview__slice_assign_scalar(char *, Py_ssize_t *, Py_ssize_t *, int, size_t, void *); /*proto*/
 static PyObject *__pyx_unpickle_Enum__set_state(struct __pyx_MemviewEnum_obj *, PyObject *); /*proto*/
-static __Pyx_TypeInfo __Pyx_TypeInfo_char = { "char", NULL, sizeof(char), { 0 }, 0, 'H', IS_UNSIGNED(char), 0 };
+static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_5numpy_int8_t = { "int8_t", NULL, sizeof(__pyx_t_5numpy_int8_t), { 0 }, 0, IS_UNSIGNED(__pyx_t_5numpy_int8_t) ? 'U' : 'I', IS_UNSIGNED(__pyx_t_5numpy_int8_t), 0 };
 static __Pyx_TypeInfo __Pyx_TypeInfo_double = { "double", NULL, sizeof(double), { 0 }, 0, 'R', 0, 0 };
 #define __Pyx_MODULE_NAME "dwave.samplers.sa.simulated_annealing"
 extern int __pyx_module_is_main_dwave__samplers__sa__simulated_annealing;
 int __pyx_module_is_main_dwave__samplers__sa__simulated_annealing = 0;
 
 /* Implementation of 'dwave.samplers.sa.simulated_annealing' */
-static PyObject *__pyx_builtin_ImportError;
 static PyObject *__pyx_builtin_ValueError;
+static PyObject *__pyx_builtin_ImportError;
 static PyObject *__pyx_builtin_MemoryError;
 static PyObject *__pyx_builtin_enumerate;
 static PyObject *__pyx_builtin_range;
 static PyObject *__pyx_builtin_TypeError;
 static PyObject *__pyx_builtin_Ellipsis;
 static PyObject *__pyx_builtin_id;
 static PyObject *__pyx_builtin_IndexError;
@@ -2362,14 +2371,16 @@
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_ASCII[] = "ASCII";
 static const char __pyx_k_class[] = "__class__";
 static const char __pyx_k_dtype[] = "dtype";
 static const char __pyx_k_empty[] = "empty";
 static const char __pyx_k_error[] = "error";
 static const char __pyx_k_flags[] = "flags";
+static const char __pyx_k_gibbs[] = "gibbs";
+static const char __pyx_k_lower[] = "lower";
 static const char __pyx_k_numpy[] = "numpy";
 static const char __pyx_k_range[] = "range";
 static const char __pyx_k_shape[] = "shape";
 static const char __pyx_k_start[] = "start";
 static const char __pyx_k_zeros[] = "zeros";
 static const char __pyx_k_double[] = "double";
 static const char __pyx_k_encode[] = "encode";
@@ -2389,21 +2400,24 @@
 static const char __pyx_k_Ellipsis[] = "Ellipsis";
 static const char __pyx_k_energies[] = "energies";
 static const char __pyx_k_getstate[] = "__getstate__";
 static const char __pyx_k_itemsize[] = "itemsize";
 static const char __pyx_k_num_vars[] = "num_vars";
 static const char __pyx_k_pyx_type[] = "__pyx_type";
 static const char __pyx_k_setstate[] = "__setstate__";
+static const char __pyx_k_varorder[] = "_varorder";
 static const char __pyx_k_TypeError[] = "TypeError";
 static const char __pyx_k_enumerate[] = "enumerate";
 static const char __pyx_k_pyx_state[] = "__pyx_state";
 static const char __pyx_k_reduce_ex[] = "__reduce_ex__";
 static const char __pyx_k_IndexError[] = "IndexError";
+static const char __pyx_k_Metropolis[] = "Metropolis";
 static const char __pyx_k_ValueError[] = "ValueError";
 static const char __pyx_k_energies_2[] = "_energies";
+static const char __pyx_k_metropolis[] = "metropolis";
 static const char __pyx_k_pyx_result[] = "__pyx_result";
 static const char __pyx_k_pyx_vtable[] = "__pyx_vtable__";
 static const char __pyx_k_ImportError[] = "ImportError";
 static const char __pyx_k_MemoryError[] = "MemoryError";
 static const char __pyx_k_PickleError[] = "PickleError";
 static const char __pyx_k_num_samples[] = "num_samples";
 static const char __pyx_k_coupler_ends[] = "coupler_ends";
@@ -2420,14 +2434,15 @@
 static const char __pyx_k_View_MemoryView[] = "View.MemoryView";
 static const char __pyx_k_allocate_buffer[] = "allocate_buffer";
 static const char __pyx_k_annealed_states[] = "annealed_states";
 static const char __pyx_k_beta_schedule_2[] = "_beta_schedule";
 static const char __pyx_k_coupler_weights[] = "coupler_weights";
 static const char __pyx_k_dtype_is_object[] = "dtype_is_object";
 static const char __pyx_k_pyx_PickleError[] = "__pyx_PickleError";
+static const char __pyx_k_randomize_order[] = "randomize_order";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
 static const char __pyx_k_sweeps_per_beta[] = "sweeps_per_beta";
 static const char __pyx_k_coupler_starts_2[] = "_coupler_starts";
 static const char __pyx_k_coupler_weights_2[] = "_coupler_weights";
 static const char __pyx_k_pyx_unpickle_Enum[] = "__pyx_unpickle_Enum";
 static const char __pyx_k_sweeps_per_beta_2[] = "_sweeps_per_beta";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
@@ -2439,27 +2454,30 @@
 static const char __pyx_k_contiguous_and_direct[] = "<contiguous and direct>";
 static const char __pyx_k_MemoryView_of_r_object[] = "<MemoryView of %r object>";
 static const char __pyx_k_MemoryView_of_r_at_0x_x[] = "<MemoryView of %r at 0x%x>";
 static const char __pyx_k_contiguous_and_indirect[] = "<contiguous and indirect>";
 static const char __pyx_k_Cannot_index_with_type_s[] = "Cannot index with type '%s'";
 static const char __pyx_k_Invalid_shape_in_axis_d_d[] = "Invalid shape in axis %d: %d.";
 static const char __pyx_k_itemsize_0_for_cython_array[] = "itemsize <= 0 for cython.array";
+static const char __pyx_k_proposal_acceptance_criteria[] = "proposal_acceptance_criteria";
 static const char __pyx_k_unable_to_allocate_array_data[] = "unable to allocate array data.";
+static const char __pyx_k_proposal_acceptance_criteria_2[] = "_proposal_acceptance_criteria";
 static const char __pyx_k_strided_and_direct_or_indirect[] = "<strided and direct or indirect>";
 static const char __pyx_k_numpy_core_multiarray_failed_to[] = "numpy.core.multiarray failed to import";
 static const char __pyx_k_Buffer_view_does_not_expose_stri[] = "Buffer view does not expose strides";
 static const char __pyx_k_Can_only_create_a_buffer_that_is[] = "Can only create a buffer that is contiguous in memory.";
 static const char __pyx_k_Cannot_assign_to_read_only_memor[] = "Cannot assign to read-only memoryview";
 static const char __pyx_k_Cannot_create_writable_memory_vi[] = "Cannot create writable memory view from read-only memoryview";
 static const char __pyx_k_Empty_shape_tuple_for_cython_arr[] = "Empty shape tuple for cython.array";
 static const char __pyx_k_Incompatible_checksums_s_vs_0xb0[] = "Incompatible checksums (%s vs 0xb068931 = (name))";
 static const char __pyx_k_Indirect_dimensions_not_supporte[] = "Indirect dimensions not supported";
 static const char __pyx_k_Invalid_mode_expected_c_or_fortr[] = "Invalid mode, expected 'c' or 'fortran', got %s";
 static const char __pyx_k_Out_of_bounds_on_buffer_access_a[] = "Out of bounds on buffer access (axis %d)";
 static const char __pyx_k_Unable_to_convert_item_to_object[] = "Unable to convert item to object";
+static const char __pyx_k_Unknown_proposal_acceptance_crit[] = "Unknown proposal_acceptance_criteria: ";
 static const char __pyx_k_dwave_samplers_sa_simulated_anne[] = "dwave/samplers/sa/simulated_annealing.pyx";
 static const char __pyx_k_got_differing_extents_in_dimensi[] = "got differing extents in dimension %d (got %d and %d)";
 static const char __pyx_k_no_default___reduce___due_to_non[] = "no default __reduce__ due to non-trivial __cinit__";
 static const char __pyx_k_numpy_core_umath_failed_to_impor[] = "numpy.core.umath failed to import";
 static const char __pyx_k_unable_to_allocate_shape_and_str[] = "unable to allocate shape and strides.";
 static const char __pyx_k_dwave_samplers_sa_simulated_anne_2[] = "dwave.samplers.sa.simulated_annealing";
 static PyObject *__pyx_n_s_ASCII;
@@ -2475,19 +2493,21 @@
 static PyObject *__pyx_n_s_IndexError;
 static PyObject *__pyx_kp_s_Indirect_dimensions_not_supporte;
 static PyObject *__pyx_kp_s_Invalid_mode_expected_c_or_fortr;
 static PyObject *__pyx_kp_s_Invalid_shape_in_axis_d_d;
 static PyObject *__pyx_n_s_MemoryError;
 static PyObject *__pyx_kp_s_MemoryView_of_r_at_0x_x;
 static PyObject *__pyx_kp_s_MemoryView_of_r_object;
+static PyObject *__pyx_n_u_Metropolis;
 static PyObject *__pyx_n_b_O;
 static PyObject *__pyx_kp_s_Out_of_bounds_on_buffer_access_a;
 static PyObject *__pyx_n_s_PickleError;
 static PyObject *__pyx_n_s_TypeError;
 static PyObject *__pyx_kp_s_Unable_to_convert_item_to_object;
+static PyObject *__pyx_kp_u_Unknown_proposal_acceptance_crit;
 static PyObject *__pyx_n_s_ValueError;
 static PyObject *__pyx_n_s_View_MemoryView;
 static PyObject *__pyx_n_s_allocate_buffer;
 static PyObject *__pyx_n_s_annealed_states;
 static PyObject *__pyx_n_s_base;
 static PyObject *__pyx_n_s_beta_schedule;
 static PyObject *__pyx_n_s_beta_schedule_2;
@@ -2518,26 +2538,29 @@
 static PyObject *__pyx_n_s_error;
 static PyObject *__pyx_n_s_flags;
 static PyObject *__pyx_n_s_float64;
 static PyObject *__pyx_n_s_format;
 static PyObject *__pyx_n_s_fortran;
 static PyObject *__pyx_n_u_fortran;
 static PyObject *__pyx_n_s_getstate;
+static PyObject *__pyx_n_u_gibbs;
 static PyObject *__pyx_kp_s_got_differing_extents_in_dimensi;
 static PyObject *__pyx_n_s_h;
 static PyObject *__pyx_n_s_h_2;
 static PyObject *__pyx_n_s_id;
 static PyObject *__pyx_n_s_import;
 static PyObject *__pyx_n_s_int8;
 static PyObject *__pyx_n_s_interrupt_function;
 static PyObject *__pyx_n_s_interrupt_function_2;
 static PyObject *__pyx_n_s_itemsize;
 static PyObject *__pyx_kp_s_itemsize_0_for_cython_array;
+static PyObject *__pyx_n_s_lower;
 static PyObject *__pyx_n_s_main;
 static PyObject *__pyx_n_s_memview;
+static PyObject *__pyx_n_u_metropolis;
 static PyObject *__pyx_n_s_mode;
 static PyObject *__pyx_n_s_name;
 static PyObject *__pyx_n_s_name_2;
 static PyObject *__pyx_n_s_ndim;
 static PyObject *__pyx_n_s_new;
 static PyObject *__pyx_kp_s_no_default___reduce___due_to_non;
 static PyObject *__pyx_n_s_np;
@@ -2547,22 +2570,25 @@
 static PyObject *__pyx_n_s_num_vars;
 static PyObject *__pyx_n_s_numpy;
 static PyObject *__pyx_kp_u_numpy_core_multiarray_failed_to;
 static PyObject *__pyx_kp_u_numpy_core_umath_failed_to_impor;
 static PyObject *__pyx_n_s_obj;
 static PyObject *__pyx_n_s_pack;
 static PyObject *__pyx_n_s_pickle;
+static PyObject *__pyx_n_s_proposal_acceptance_criteria;
+static PyObject *__pyx_n_s_proposal_acceptance_criteria_2;
 static PyObject *__pyx_n_s_pyx_PickleError;
 static PyObject *__pyx_n_s_pyx_checksum;
 static PyObject *__pyx_n_s_pyx_getbuffer;
 static PyObject *__pyx_n_s_pyx_result;
 static PyObject *__pyx_n_s_pyx_state;
 static PyObject *__pyx_n_s_pyx_type;
 static PyObject *__pyx_n_s_pyx_unpickle_Enum;
 static PyObject *__pyx_n_s_pyx_vtable;
+static PyObject *__pyx_n_s_randomize_order;
 static PyObject *__pyx_n_s_range;
 static PyObject *__pyx_n_s_reduce;
 static PyObject *__pyx_n_s_reduce_cython;
 static PyObject *__pyx_n_s_reduce_ex;
 static PyObject *__pyx_n_s_seed;
 static PyObject *__pyx_n_s_seed_2;
 static PyObject *__pyx_n_s_setstate;
@@ -2583,16 +2609,17 @@
 static PyObject *__pyx_n_s_sweeps_per_beta;
 static PyObject *__pyx_n_s_sweeps_per_beta_2;
 static PyObject *__pyx_n_s_test;
 static PyObject *__pyx_kp_s_unable_to_allocate_array_data;
 static PyObject *__pyx_kp_s_unable_to_allocate_shape_and_str;
 static PyObject *__pyx_n_s_unpack;
 static PyObject *__pyx_n_s_update;
+static PyObject *__pyx_n_s_varorder;
 static PyObject *__pyx_n_s_zeros;
-static PyObject *__pyx_pf_5dwave_8samplers_2sa_19simulated_annealing_simulated_annealing(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_num_samples, PyObject *__pyx_v_h, PyObject *__pyx_v_coupler_starts, PyObject *__pyx_v_coupler_ends, PyObject *__pyx_v_coupler_weights, PyObject *__pyx_v_sweeps_per_beta, PyObject *__pyx_v_beta_schedule, PyObject *__pyx_v_seed, PyArrayObject *__pyx_v_states_numpy, PyObject *__pyx_v_interrupt_function); /* proto */
+static PyObject *__pyx_pf_5dwave_8samplers_2sa_19simulated_annealing_simulated_annealing(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_num_samples, PyObject *__pyx_v_h, PyObject *__pyx_v_coupler_starts, PyObject *__pyx_v_coupler_ends, PyObject *__pyx_v_coupler_weights, PyObject *__pyx_v_sweeps_per_beta, PyObject *__pyx_v_beta_schedule, PyObject *__pyx_v_seed, PyArrayObject *__pyx_v_states_numpy, PyObject *__pyx_v_randomize_order, PyObject *__pyx_v_proposal_acceptance_criteria, PyObject *__pyx_v_interrupt_function); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array___cinit__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_shape, Py_ssize_t __pyx_v_itemsize, PyObject *__pyx_v_format, PyObject *__pyx_v_mode, int __pyx_v_allocate_buffer); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array_2__getbuffer__(struct __pyx_array_obj *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags); /* proto */
 static void __pyx_array___pyx_pf_15View_dot_MemoryView_5array_4__dealloc__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_15View_dot_MemoryView_5array_7memview___get__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static Py_ssize_t __pyx_array___pyx_pf_15View_dot_MemoryView_5array_6__len__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_array___pyx_pf_15View_dot_MemoryView_5array_8__getattr__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_attr); /* proto */
 static PyObject *__pyx_array___pyx_pf_15View_dot_MemoryView_5array_10__getitem__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_item); /* proto */
@@ -2666,59 +2693,75 @@
 static PyObject *__pyx_tuple__26;
 static PyObject *__pyx_tuple__27;
 static PyObject *__pyx_tuple__28;
 static PyObject *__pyx_codeobj__22;
 static PyObject *__pyx_codeobj__29;
 /* Late includes */
 
-/* "dwave/samplers/sa/simulated_annealing.pyx":45
+/* "dwave/samplers/sa/simulated_annealing.pyx":50
  * 
  * 
  * def simulated_annealing(num_samples, h, coupler_starts, coupler_ends,             # <<<<<<<<<<<<<<
  *                         coupler_weights, sweeps_per_beta, beta_schedule, seed,
- *                         np.ndarray[char, ndim=2, mode="c"] states_numpy,
+ *                         np.ndarray[np.int8_t, ndim=2, mode="c"] states_numpy,
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_5dwave_8samplers_2sa_19simulated_annealing_1simulated_annealing(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_5dwave_8samplers_2sa_19simulated_annealing_simulated_annealing[] = "Wraps `general_simulated_annealing` from `cpu_sa.cpp`. Accepts\n    an Ising problem defined on a general graph and returns samples\n    using simulated annealing.\n\n    Parameters\n    ----------\n    num_samples : int\n        Number of samples to get from the sampler.\n\n    h : list(float)\n        The h or field values for the problem.\n\n    coupler_starts : list(int)\n        A list of the start variable of each coupler. For a problem\n        with the couplers (0, 1), (1, 2), and (3, 1), `coupler_starts`\n        should be [0, 1, 3].\n\n    coupler_ends : list(int)\n        A list of the end variable of each coupler. For a problem\n        with the couplers (0, 1), (1, 2), and (3, 1), `coupler_ends`\n        should be [1, 2, 1].\n\n    coupler_weights : list(float)\n        A list of the J values or weight on each coupler, in the same\n        order as `coupler_starts` and `coupler_ends`.\n\n    sweeps_per_beta : int\n        The number of sweeps to perform at each beta value provided in\n        `beta_schedule`. The total number of sweeps per sample is\n        sweeps_per_beta * len(beta_schedule).\n\n    beta_schedule : list(float)\n        A list of the different beta values to run sweeps at.\n\n    seed : 64 bit int > 0\n        The seed to use for the PRNG. Must be a positive integer\n        greater than 0. If the same seed is used and the rest of the\n        parameters are the same, the returned samples will be\n        identical.\n\n    states_numpy : np.ndarray[char, ndim=2, mode=\"c\"], values in (-1, 1)\n        The initial seeded states of the simulated annealing runs. Should be of\n        a contiguous numpy.ndarray of shape (num_samples, num_variables).\n\n    interrupt_function: function\n        Should accept no arguments and return a bool. The function is\n        called between samples and if it returns True, simulated annealing\n        will return early with the samples it already has.\n\n    Returns\n    -------\n    samples : numpy.nd""array\n        A 2D numpy array where each row is a sample.\n\n    energies: np.ndarray\n        The energies.\n\n    ";
+static char __pyx_doc_5dwave_8samplers_2sa_19simulated_annealing_simulated_annealing[] = "Wraps `general_simulated_annealing` from `cpu_sa.cpp`. Accepts\n    an Ising problem defined on a general graph and returns samples\n    using simulated annealing.\n\n    Parameters\n    ----------\n    num_samples : int\n        Number of samples to get from the sampler.\n\n    h : list(float)\n        The h or field values for the problem.\n\n    coupler_starts : list(int)\n        A list of the start variable of each coupler. For a problem\n        with the couplers (0, 1), (1, 2), and (3, 1), `coupler_starts`\n        should be [0, 1, 3].\n\n    coupler_ends : list(int)\n        A list of the end variable of each coupler. For a problem\n        with the couplers (0, 1), (1, 2), and (3, 1), `coupler_ends`\n        should be [1, 2, 1].\n\n    coupler_weights : list(float)\n        A list of the J values or weight on each coupler, in the same\n        order as `coupler_starts` and `coupler_ends`.\n\n    sweeps_per_beta : int\n        The number of sweeps to perform at each beta value provided in\n        `beta_schedule`. The total number of sweeps per sample is\n        sweeps_per_beta * len(beta_schedule).\n\n    beta_schedule : list(float)\n        A list of the different beta values to run sweeps at.\n\n    seed : 64 bit int > 0\n        The seed to use for the PRNG. Must be a positive integer\n        greater than 0. If the same seed is used and the rest of the\n        parameters are the same, the returned samples will be\n        identical.\n\n    states_numpy : np.ndarray[int8_t, ndim=2, mode=\"c\"], values in (-1, 1)\n        The initial seeded states of the simulated annealing runs. Should be of\n        a contiguous numpy.ndarray of shape (num_samples, num_variables).\n\n    interrupt_function: function\n        Should accept no arguments and return a bool. The function is\n        called between samples and if it returns True, simulated annealing\n        will return early with the samples it already has.\n\n    randomize_order: bool\n        When True, ""each spin update selects a variable uniformly at random.\n        When False, updates proceed sequentially through the labeled variables \n        on each sweep so that all variables are updated once per sweep.\n        The random method is ergodic and obeys detailed balance at all temperatures.\n        Symmetries of the Boltzmann distribution(s) are not broken by the\n        update order.\n        The sequential method:\n            - when combined with ``proposal_acceptance_criteria=Metropolis`` can be\n            non-ergodic in the limits of zero or infinite temperature,\n            and converge slowly near these limits.\n            - can introduce a dynamical bias as a function of variable\n            labeling convention.\n            - has faster per spin update than the random method.\n\n    proposal_acceptance_criteria: str\n        When `Gibbs`, each spin flip proposal is accepted according to the\n        Gibbs criteria.\n        When `Metropolis`, each spin flip proposal is accepted according to the\n        Metropolis-Hastings criteria.\n\n    Returns\n    -------\n    samples : numpy.ndarray\n        A 2D numpy array where each row is a sample.\n\n    energies: np.ndarray\n        The energies.\n\n    ";
 static PyMethodDef __pyx_mdef_5dwave_8samplers_2sa_19simulated_annealing_1simulated_annealing = {"simulated_annealing", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_5dwave_8samplers_2sa_19simulated_annealing_1simulated_annealing, METH_VARARGS|METH_KEYWORDS, __pyx_doc_5dwave_8samplers_2sa_19simulated_annealing_simulated_annealing};
 static PyObject *__pyx_pw_5dwave_8samplers_2sa_19simulated_annealing_1simulated_annealing(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_num_samples = 0;
   PyObject *__pyx_v_h = 0;
   PyObject *__pyx_v_coupler_starts = 0;
   PyObject *__pyx_v_coupler_ends = 0;
   PyObject *__pyx_v_coupler_weights = 0;
   PyObject *__pyx_v_sweeps_per_beta = 0;
   PyObject *__pyx_v_beta_schedule = 0;
   PyObject *__pyx_v_seed = 0;
   PyArrayObject *__pyx_v_states_numpy = 0;
+  PyObject *__pyx_v_randomize_order = 0;
+  PyObject *__pyx_v_proposal_acceptance_criteria = 0;
   PyObject *__pyx_v_interrupt_function = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("simulated_annealing (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_num_samples,&__pyx_n_s_h,&__pyx_n_s_coupler_starts,&__pyx_n_s_coupler_ends,&__pyx_n_s_coupler_weights,&__pyx_n_s_sweeps_per_beta,&__pyx_n_s_beta_schedule,&__pyx_n_s_seed,&__pyx_n_s_states_numpy,&__pyx_n_s_interrupt_function,0};
-    PyObject* values[10] = {0,0,0,0,0,0,0,0,0,0};
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_num_samples,&__pyx_n_s_h,&__pyx_n_s_coupler_starts,&__pyx_n_s_coupler_ends,&__pyx_n_s_coupler_weights,&__pyx_n_s_sweeps_per_beta,&__pyx_n_s_beta_schedule,&__pyx_n_s_seed,&__pyx_n_s_states_numpy,&__pyx_n_s_randomize_order,&__pyx_n_s_proposal_acceptance_criteria,&__pyx_n_s_interrupt_function,0};
+    PyObject* values[12] = {0,0,0,0,0,0,0,0,0,0,0,0};
 
-    /* "dwave/samplers/sa/simulated_annealing.pyx":48
+    /* "dwave/samplers/sa/simulated_annealing.pyx":53
  *                         coupler_weights, sweeps_per_beta, beta_schedule, seed,
- *                         np.ndarray[char, ndim=2, mode="c"] states_numpy,
+ *                         np.ndarray[np.int8_t, ndim=2, mode="c"] states_numpy,
+ *                         randomize_order=False,             # <<<<<<<<<<<<<<
+ *                         proposal_acceptance_criteria='Metropolis',
+ *                         interrupt_function=None):
+ */
+    values[9] = ((PyObject *)Py_False);
+    values[10] = ((PyObject *)__pyx_n_u_Metropolis);
+
+    /* "dwave/samplers/sa/simulated_annealing.pyx":55
+ *                         randomize_order=False,
+ *                         proposal_acceptance_criteria='Metropolis',
  *                         interrupt_function=None):             # <<<<<<<<<<<<<<
  *     """Wraps `general_simulated_annealing` from `cpu_sa.cpp`. Accepts
  *     an Ising problem defined on a general graph and returns samples
  */
-    values[9] = ((PyObject *)Py_None);
+    values[11] = ((PyObject *)Py_None);
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
+        case 12: values[11] = PyTuple_GET_ITEM(__pyx_args, 11);
+        CYTHON_FALLTHROUGH;
+        case 11: values[10] = PyTuple_GET_ITEM(__pyx_args, 10);
+        CYTHON_FALLTHROUGH;
         case 10: values[9] = PyTuple_GET_ITEM(__pyx_args, 9);
         CYTHON_FALLTHROUGH;
         case  9: values[8] = PyTuple_GET_ITEM(__pyx_args, 8);
         CYTHON_FALLTHROUGH;
         case  8: values[7] = PyTuple_GET_ITEM(__pyx_args, 7);
         CYTHON_FALLTHROUGH;
         case  7: values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
@@ -2743,70 +2786,86 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_num_samples)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_h)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("simulated_annealing", 0, 9, 10, 1); __PYX_ERR(0, 45, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("simulated_annealing", 0, 9, 12, 1); __PYX_ERR(0, 50, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_coupler_starts)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("simulated_annealing", 0, 9, 10, 2); __PYX_ERR(0, 45, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("simulated_annealing", 0, 9, 12, 2); __PYX_ERR(0, 50, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_coupler_ends)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("simulated_annealing", 0, 9, 10, 3); __PYX_ERR(0, 45, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("simulated_annealing", 0, 9, 12, 3); __PYX_ERR(0, 50, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_coupler_weights)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("simulated_annealing", 0, 9, 10, 4); __PYX_ERR(0, 45, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("simulated_annealing", 0, 9, 12, 4); __PYX_ERR(0, 50, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (likely((values[5] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_sweeps_per_beta)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("simulated_annealing", 0, 9, 10, 5); __PYX_ERR(0, 45, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("simulated_annealing", 0, 9, 12, 5); __PYX_ERR(0, 50, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  6:
         if (likely((values[6] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_beta_schedule)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("simulated_annealing", 0, 9, 10, 6); __PYX_ERR(0, 45, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("simulated_annealing", 0, 9, 12, 6); __PYX_ERR(0, 50, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  7:
         if (likely((values[7] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_seed)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("simulated_annealing", 0, 9, 10, 7); __PYX_ERR(0, 45, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("simulated_annealing", 0, 9, 12, 7); __PYX_ERR(0, 50, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  8:
         if (likely((values[8] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_states_numpy)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("simulated_annealing", 0, 9, 10, 8); __PYX_ERR(0, 45, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("simulated_annealing", 0, 9, 12, 8); __PYX_ERR(0, 50, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  9:
         if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_interrupt_function);
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_randomize_order);
           if (value) { values[9] = value; kw_args--; }
         }
+        CYTHON_FALLTHROUGH;
+        case 10:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_proposal_acceptance_criteria);
+          if (value) { values[10] = value; kw_args--; }
+        }
+        CYTHON_FALLTHROUGH;
+        case 11:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_interrupt_function);
+          if (value) { values[11] = value; kw_args--; }
+        }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "simulated_annealing") < 0)) __PYX_ERR(0, 45, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "simulated_annealing") < 0)) __PYX_ERR(0, 50, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
+        case 12: values[11] = PyTuple_GET_ITEM(__pyx_args, 11);
+        CYTHON_FALLTHROUGH;
+        case 11: values[10] = PyTuple_GET_ITEM(__pyx_args, 10);
+        CYTHON_FALLTHROUGH;
         case 10: values[9] = PyTuple_GET_ITEM(__pyx_args, 9);
         CYTHON_FALLTHROUGH;
         case  9: values[8] = PyTuple_GET_ITEM(__pyx_args, 8);
         values[7] = PyTuple_GET_ITEM(__pyx_args, 7);
         values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
         values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
         values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
@@ -2823,59 +2882,63 @@
     __pyx_v_coupler_starts = values[2];
     __pyx_v_coupler_ends = values[3];
     __pyx_v_coupler_weights = values[4];
     __pyx_v_sweeps_per_beta = values[5];
     __pyx_v_beta_schedule = values[6];
     __pyx_v_seed = values[7];
     __pyx_v_states_numpy = ((PyArrayObject *)values[8]);
-    __pyx_v_interrupt_function = values[9];
+    __pyx_v_randomize_order = values[9];
+    __pyx_v_proposal_acceptance_criteria = values[10];
+    __pyx_v_interrupt_function = values[11];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("simulated_annealing", 0, 9, 10, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 45, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("simulated_annealing", 0, 9, 12, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 50, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("dwave.samplers.sa.simulated_annealing.simulated_annealing", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_states_numpy), __pyx_ptype_5numpy_ndarray, 1, "states_numpy", 0))) __PYX_ERR(0, 47, __pyx_L1_error)
-  __pyx_r = __pyx_pf_5dwave_8samplers_2sa_19simulated_annealing_simulated_annealing(__pyx_self, __pyx_v_num_samples, __pyx_v_h, __pyx_v_coupler_starts, __pyx_v_coupler_ends, __pyx_v_coupler_weights, __pyx_v_sweeps_per_beta, __pyx_v_beta_schedule, __pyx_v_seed, __pyx_v_states_numpy, __pyx_v_interrupt_function);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_states_numpy), __pyx_ptype_5numpy_ndarray, 1, "states_numpy", 0))) __PYX_ERR(0, 52, __pyx_L1_error)
+  __pyx_r = __pyx_pf_5dwave_8samplers_2sa_19simulated_annealing_simulated_annealing(__pyx_self, __pyx_v_num_samples, __pyx_v_h, __pyx_v_coupler_starts, __pyx_v_coupler_ends, __pyx_v_coupler_weights, __pyx_v_sweeps_per_beta, __pyx_v_beta_schedule, __pyx_v_seed, __pyx_v_states_numpy, __pyx_v_randomize_order, __pyx_v_proposal_acceptance_criteria, __pyx_v_interrupt_function);
 
-  /* "dwave/samplers/sa/simulated_annealing.pyx":45
+  /* "dwave/samplers/sa/simulated_annealing.pyx":50
  * 
  * 
  * def simulated_annealing(num_samples, h, coupler_starts, coupler_ends,             # <<<<<<<<<<<<<<
  *                         coupler_weights, sweeps_per_beta, beta_schedule, seed,
- *                         np.ndarray[char, ndim=2, mode="c"] states_numpy,
+ *                         np.ndarray[np.int8_t, ndim=2, mode="c"] states_numpy,
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_5dwave_8samplers_2sa_19simulated_annealing_simulated_annealing(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_num_samples, PyObject *__pyx_v_h, PyObject *__pyx_v_coupler_starts, PyObject *__pyx_v_coupler_ends, PyObject *__pyx_v_coupler_weights, PyObject *__pyx_v_sweeps_per_beta, PyObject *__pyx_v_beta_schedule, PyObject *__pyx_v_seed, PyArrayObject *__pyx_v_states_numpy, PyObject *__pyx_v_interrupt_function) {
+static PyObject *__pyx_pf_5dwave_8samplers_2sa_19simulated_annealing_simulated_annealing(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_num_samples, PyObject *__pyx_v_h, PyObject *__pyx_v_coupler_starts, PyObject *__pyx_v_coupler_ends, PyObject *__pyx_v_coupler_weights, PyObject *__pyx_v_sweeps_per_beta, PyObject *__pyx_v_beta_schedule, PyObject *__pyx_v_seed, PyArrayObject *__pyx_v_states_numpy, PyObject *__pyx_v_randomize_order, PyObject *__pyx_v_proposal_acceptance_criteria, PyObject *__pyx_v_interrupt_function) {
   PyObject *__pyx_v_num_vars = NULL;
   PyObject *__pyx_v_annealed_states = NULL;
   PyObject *__pyx_v_energies_numpy = NULL;
   __Pyx_memviewslice __pyx_v_energies = { 0, 0, { 0 }, { 0 }, { 0 } };
-  char *__pyx_v__states;
+  __pyx_t_5numpy_int8_t *__pyx_v__states;
   double *__pyx_v__energies;
   int __pyx_v__num_samples;
   std::vector<double>  __pyx_v__h;
   std::vector<int>  __pyx_v__coupler_starts;
   std::vector<int>  __pyx_v__coupler_ends;
   std::vector<double>  __pyx_v__coupler_weights;
   int __pyx_v__sweeps_per_beta;
   std::vector<double>  __pyx_v__beta_schedule;
   unsigned PY_LONG_LONG __pyx_v__seed;
+  VariableOrder __pyx_v__varorder;
+  Proposal __pyx_v__proposal_acceptance_criteria;
   void *__pyx_v__interrupt_function;
   int __pyx_v_num;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_states_numpy;
   __Pyx_Buffer __pyx_pybuffer_states_numpy;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
@@ -2899,192 +2962,192 @@
   __Pyx_RefNannySetupContext("simulated_annealing", 0);
   __pyx_pybuffer_states_numpy.pybuffer.buf = NULL;
   __pyx_pybuffer_states_numpy.refcount = 0;
   __pyx_pybuffernd_states_numpy.data = NULL;
   __pyx_pybuffernd_states_numpy.rcbuffer = &__pyx_pybuffer_states_numpy;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_states_numpy.rcbuffer->pybuffer, (PyObject*)__pyx_v_states_numpy, &__Pyx_TypeInfo_char, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 2, 0, __pyx_stack) == -1)) __PYX_ERR(0, 45, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_states_numpy.rcbuffer->pybuffer, (PyObject*)__pyx_v_states_numpy, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int8_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 2, 0, __pyx_stack) == -1)) __PYX_ERR(0, 50, __pyx_L1_error)
   }
   __pyx_pybuffernd_states_numpy.diminfo[0].strides = __pyx_pybuffernd_states_numpy.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_states_numpy.diminfo[0].shape = __pyx_pybuffernd_states_numpy.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_states_numpy.diminfo[1].strides = __pyx_pybuffernd_states_numpy.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_states_numpy.diminfo[1].shape = __pyx_pybuffernd_states_numpy.rcbuffer->pybuffer.shape[1];
 
-  /* "dwave/samplers/sa/simulated_annealing.pyx":107
+  /* "dwave/samplers/sa/simulated_annealing.pyx":135
  * 
  *     """
  *     num_vars = len(h)             # <<<<<<<<<<<<<<
  * 
  *     # in the case that we either need no samples or there are no variables,
  */
-  __pyx_t_1 = PyObject_Length(__pyx_v_h); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 107, __pyx_L1_error)
-  __pyx_t_2 = PyInt_FromSsize_t(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 107, __pyx_L1_error)
+  __pyx_t_1 = PyObject_Length(__pyx_v_h); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 135, __pyx_L1_error)
+  __pyx_t_2 = PyInt_FromSsize_t(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 135, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_v_num_vars = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "dwave/samplers/sa/simulated_annealing.pyx":111
+  /* "dwave/samplers/sa/simulated_annealing.pyx":139
  *     # in the case that we either need no samples or there are no variables,
  *     # we can safely return an empty array (and set energies to 0)
  *     if num_samples*num_vars == 0:             # <<<<<<<<<<<<<<
  *         annealed_states = np.empty((num_samples, num_vars), dtype=np.int8)
  *         return annealed_states, np.zeros(num_samples, dtype=np.double)
  */
-  __pyx_t_2 = PyNumber_Multiply(__pyx_v_num_samples, __pyx_v_num_vars); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 111, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Multiply(__pyx_v_num_samples, __pyx_v_num_vars); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 139, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyInt_EqObjC(__pyx_t_2, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 111, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_EqObjC(__pyx_t_2, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 139, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 111, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 139, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (__pyx_t_4) {
 
-    /* "dwave/samplers/sa/simulated_annealing.pyx":112
+    /* "dwave/samplers/sa/simulated_annealing.pyx":140
  *     # we can safely return an empty array (and set energies to 0)
  *     if num_samples*num_vars == 0:
  *         annealed_states = np.empty((num_samples, num_vars), dtype=np.int8)             # <<<<<<<<<<<<<<
  *         return annealed_states, np.zeros(num_samples, dtype=np.double)
  * 
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 112, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 140, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 112, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 140, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 112, __pyx_L1_error)
+    __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 140, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_v_num_samples);
     __Pyx_GIVEREF(__pyx_v_num_samples);
     PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_num_samples);
     __Pyx_INCREF(__pyx_v_num_vars);
     __Pyx_GIVEREF(__pyx_v_num_vars);
     PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_v_num_vars);
-    __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 112, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 140, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_3);
     __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 112, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 140, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 112, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 140, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_int8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 112, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_int8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 140, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_7) < 0) __PYX_ERR(0, 112, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_7) < 0) __PYX_ERR(0, 140, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, __pyx_t_3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 112, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, __pyx_t_3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 140, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_annealed_states = __pyx_t_7;
     __pyx_t_7 = 0;
 
-    /* "dwave/samplers/sa/simulated_annealing.pyx":113
+    /* "dwave/samplers/sa/simulated_annealing.pyx":141
  *     if num_samples*num_vars == 0:
  *         annealed_states = np.empty((num_samples, num_vars), dtype=np.int8)
  *         return annealed_states, np.zeros(num_samples, dtype=np.double)             # <<<<<<<<<<<<<<
  * 
  *     # allocate ndarray for energies
  */
     __Pyx_XDECREF(__pyx_r);
-    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 113, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 141, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 113, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 141, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 113, __pyx_L1_error)
+    __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 141, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_INCREF(__pyx_v_num_samples);
     __Pyx_GIVEREF(__pyx_v_num_samples);
     PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_v_num_samples);
-    __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 113, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 141, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 113, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 141, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_double); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 113, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_double); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 141, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 113, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 141, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_7, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 113, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_7, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 141, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 113, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 141, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_INCREF(__pyx_v_annealed_states);
     __Pyx_GIVEREF(__pyx_v_annealed_states);
     PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_v_annealed_states);
     __Pyx_GIVEREF(__pyx_t_6);
     PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_6);
     __pyx_t_6 = 0;
     __pyx_r = __pyx_t_5;
     __pyx_t_5 = 0;
     goto __pyx_L0;
 
-    /* "dwave/samplers/sa/simulated_annealing.pyx":111
+    /* "dwave/samplers/sa/simulated_annealing.pyx":139
  *     # in the case that we either need no samples or there are no variables,
  *     # we can safely return an empty array (and set energies to 0)
  *     if num_samples*num_vars == 0:             # <<<<<<<<<<<<<<
  *         annealed_states = np.empty((num_samples, num_vars), dtype=np.int8)
  *         return annealed_states, np.zeros(num_samples, dtype=np.double)
  */
   }
 
-  /* "dwave/samplers/sa/simulated_annealing.pyx":116
+  /* "dwave/samplers/sa/simulated_annealing.pyx":144
  * 
  *     # allocate ndarray for energies
  *     energies_numpy = np.empty(num_samples, dtype=np.float64)             # <<<<<<<<<<<<<<
  *     cdef double[:] energies = energies_numpy
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 116, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 144, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_empty); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 116, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_empty); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 144, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 116, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 144, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_INCREF(__pyx_v_num_samples);
   __Pyx_GIVEREF(__pyx_v_num_samples);
   PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_v_num_samples);
-  __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 116, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 144, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 116, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 144, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_float64); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 116, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_float64); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 144, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_dtype, __pyx_t_2) < 0) __PYX_ERR(0, 116, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_dtype, __pyx_t_2) < 0) __PYX_ERR(0, 144, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_5, __pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 116, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_5, __pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 144, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_v_energies_numpy = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "dwave/samplers/sa/simulated_annealing.pyx":117
+  /* "dwave/samplers/sa/simulated_annealing.pyx":145
  *     # allocate ndarray for energies
  *     energies_numpy = np.empty(num_samples, dtype=np.float64)
  *     cdef double[:] energies = energies_numpy             # <<<<<<<<<<<<<<
  * 
  *     # explicitly convert all Python types to C while we have the GIL
  */
-  __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_ds_double(__pyx_v_energies_numpy, PyBUF_WRITABLE); if (unlikely(!__pyx_t_8.memview)) __PYX_ERR(0, 117, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_ds_double(__pyx_v_energies_numpy, PyBUF_WRITABLE); if (unlikely(!__pyx_t_8.memview)) __PYX_ERR(0, 145, __pyx_L1_error)
   __pyx_v_energies = __pyx_t_8;
   __pyx_t_8.memview = NULL;
   __pyx_t_8.data = NULL;
 
-  /* "dwave/samplers/sa/simulated_annealing.pyx":120
+  /* "dwave/samplers/sa/simulated_annealing.pyx":148
  * 
  *     # explicitly convert all Python types to C while we have the GIL
- *     cdef char* _states = &states_numpy[0, 0]             # <<<<<<<<<<<<<<
+ *     cdef np.int8_t* _states = &states_numpy[0, 0]             # <<<<<<<<<<<<<<
  *     cdef double* _energies = &energies[0]
  *     cdef int _num_samples = num_samples
  */
   __pyx_t_9 = 0;
   __pyx_t_10 = 0;
   __pyx_t_11 = -1;
   if (__pyx_t_9 < 0) {
@@ -3093,239 +3156,396 @@
   } else if (unlikely(__pyx_t_9 >= __pyx_pybuffernd_states_numpy.diminfo[0].shape)) __pyx_t_11 = 0;
   if (__pyx_t_10 < 0) {
     __pyx_t_10 += __pyx_pybuffernd_states_numpy.diminfo[1].shape;
     if (unlikely(__pyx_t_10 < 0)) __pyx_t_11 = 1;
   } else if (unlikely(__pyx_t_10 >= __pyx_pybuffernd_states_numpy.diminfo[1].shape)) __pyx_t_11 = 1;
   if (unlikely(__pyx_t_11 != -1)) {
     __Pyx_RaiseBufferIndexError(__pyx_t_11);
-    __PYX_ERR(0, 120, __pyx_L1_error)
+    __PYX_ERR(0, 148, __pyx_L1_error)
   }
-  __pyx_v__states = (&(*__Pyx_BufPtrCContig2d(char *, __pyx_pybuffernd_states_numpy.rcbuffer->pybuffer.buf, __pyx_t_9, __pyx_pybuffernd_states_numpy.diminfo[0].strides, __pyx_t_10, __pyx_pybuffernd_states_numpy.diminfo[1].strides)));
+  __pyx_v__states = (&(*__Pyx_BufPtrCContig2d(__pyx_t_5numpy_int8_t *, __pyx_pybuffernd_states_numpy.rcbuffer->pybuffer.buf, __pyx_t_9, __pyx_pybuffernd_states_numpy.diminfo[0].strides, __pyx_t_10, __pyx_pybuffernd_states_numpy.diminfo[1].strides)));
 
-  /* "dwave/samplers/sa/simulated_annealing.pyx":121
+  /* "dwave/samplers/sa/simulated_annealing.pyx":149
  *     # explicitly convert all Python types to C while we have the GIL
- *     cdef char* _states = &states_numpy[0, 0]
+ *     cdef np.int8_t* _states = &states_numpy[0, 0]
  *     cdef double* _energies = &energies[0]             # <<<<<<<<<<<<<<
  *     cdef int _num_samples = num_samples
  *     cdef vector[double] _h = h
  */
   __pyx_t_10 = 0;
   __pyx_t_11 = -1;
   if (__pyx_t_10 < 0) {
     __pyx_t_10 += __pyx_v_energies.shape[0];
     if (unlikely(__pyx_t_10 < 0)) __pyx_t_11 = 0;
   } else if (unlikely(__pyx_t_10 >= __pyx_v_energies.shape[0])) __pyx_t_11 = 0;
   if (unlikely(__pyx_t_11 != -1)) {
     __Pyx_RaiseBufferIndexError(__pyx_t_11);
-    __PYX_ERR(0, 121, __pyx_L1_error)
+    __PYX_ERR(0, 149, __pyx_L1_error)
   }
   __pyx_v__energies = (&(*((double *) ( /* dim=0 */ (__pyx_v_energies.data + __pyx_t_10 * __pyx_v_energies.strides[0]) ))));
 
-  /* "dwave/samplers/sa/simulated_annealing.pyx":122
- *     cdef char* _states = &states_numpy[0, 0]
+  /* "dwave/samplers/sa/simulated_annealing.pyx":150
+ *     cdef np.int8_t* _states = &states_numpy[0, 0]
  *     cdef double* _energies = &energies[0]
  *     cdef int _num_samples = num_samples             # <<<<<<<<<<<<<<
  *     cdef vector[double] _h = h
  *     cdef vector[int] _coupler_starts = coupler_starts
  */
-  __pyx_t_11 = __Pyx_PyInt_As_int(__pyx_v_num_samples); if (unlikely((__pyx_t_11 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 122, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyInt_As_int(__pyx_v_num_samples); if (unlikely((__pyx_t_11 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 150, __pyx_L1_error)
   __pyx_v__num_samples = __pyx_t_11;
 
-  /* "dwave/samplers/sa/simulated_annealing.pyx":123
+  /* "dwave/samplers/sa/simulated_annealing.pyx":151
  *     cdef double* _energies = &energies[0]
  *     cdef int _num_samples = num_samples
  *     cdef vector[double] _h = h             # <<<<<<<<<<<<<<
  *     cdef vector[int] _coupler_starts = coupler_starts
  *     cdef vector[int] _coupler_ends = coupler_ends
  */
-  __pyx_t_12 = __pyx_convert_vector_from_py_double(__pyx_v_h); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 123, __pyx_L1_error)
+  __pyx_t_12 = __pyx_convert_vector_from_py_double(__pyx_v_h); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 151, __pyx_L1_error)
   __pyx_v__h = __pyx_t_12;
 
-  /* "dwave/samplers/sa/simulated_annealing.pyx":124
+  /* "dwave/samplers/sa/simulated_annealing.pyx":152
  *     cdef int _num_samples = num_samples
  *     cdef vector[double] _h = h
  *     cdef vector[int] _coupler_starts = coupler_starts             # <<<<<<<<<<<<<<
  *     cdef vector[int] _coupler_ends = coupler_ends
  *     cdef vector[double] _coupler_weights = coupler_weights
  */
-  __pyx_t_13 = __pyx_convert_vector_from_py_int(__pyx_v_coupler_starts); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 124, __pyx_L1_error)
+  __pyx_t_13 = __pyx_convert_vector_from_py_int(__pyx_v_coupler_starts); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 152, __pyx_L1_error)
   __pyx_v__coupler_starts = __pyx_t_13;
 
-  /* "dwave/samplers/sa/simulated_annealing.pyx":125
+  /* "dwave/samplers/sa/simulated_annealing.pyx":153
  *     cdef vector[double] _h = h
  *     cdef vector[int] _coupler_starts = coupler_starts
  *     cdef vector[int] _coupler_ends = coupler_ends             # <<<<<<<<<<<<<<
  *     cdef vector[double] _coupler_weights = coupler_weights
  *     cdef int _sweeps_per_beta = sweeps_per_beta
  */
-  __pyx_t_13 = __pyx_convert_vector_from_py_int(__pyx_v_coupler_ends); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 125, __pyx_L1_error)
+  __pyx_t_13 = __pyx_convert_vector_from_py_int(__pyx_v_coupler_ends); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 153, __pyx_L1_error)
   __pyx_v__coupler_ends = __pyx_t_13;
 
-  /* "dwave/samplers/sa/simulated_annealing.pyx":126
+  /* "dwave/samplers/sa/simulated_annealing.pyx":154
  *     cdef vector[int] _coupler_starts = coupler_starts
  *     cdef vector[int] _coupler_ends = coupler_ends
  *     cdef vector[double] _coupler_weights = coupler_weights             # <<<<<<<<<<<<<<
  *     cdef int _sweeps_per_beta = sweeps_per_beta
  *     cdef vector[double] _beta_schedule = beta_schedule
  */
-  __pyx_t_12 = __pyx_convert_vector_from_py_double(__pyx_v_coupler_weights); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 126, __pyx_L1_error)
+  __pyx_t_12 = __pyx_convert_vector_from_py_double(__pyx_v_coupler_weights); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 154, __pyx_L1_error)
   __pyx_v__coupler_weights = __pyx_t_12;
 
-  /* "dwave/samplers/sa/simulated_annealing.pyx":127
+  /* "dwave/samplers/sa/simulated_annealing.pyx":155
  *     cdef vector[int] _coupler_ends = coupler_ends
  *     cdef vector[double] _coupler_weights = coupler_weights
  *     cdef int _sweeps_per_beta = sweeps_per_beta             # <<<<<<<<<<<<<<
  *     cdef vector[double] _beta_schedule = beta_schedule
  *     cdef unsigned long long _seed = seed
  */
-  __pyx_t_11 = __Pyx_PyInt_As_int(__pyx_v_sweeps_per_beta); if (unlikely((__pyx_t_11 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 127, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyInt_As_int(__pyx_v_sweeps_per_beta); if (unlikely((__pyx_t_11 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 155, __pyx_L1_error)
   __pyx_v__sweeps_per_beta = __pyx_t_11;
 
-  /* "dwave/samplers/sa/simulated_annealing.pyx":128
+  /* "dwave/samplers/sa/simulated_annealing.pyx":156
  *     cdef vector[double] _coupler_weights = coupler_weights
  *     cdef int _sweeps_per_beta = sweeps_per_beta
  *     cdef vector[double] _beta_schedule = beta_schedule             # <<<<<<<<<<<<<<
  *     cdef unsigned long long _seed = seed
- * 
+ *     cdef VariableOrder _varorder
  */
-  __pyx_t_12 = __pyx_convert_vector_from_py_double(__pyx_v_beta_schedule); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 128, __pyx_L1_error)
+  __pyx_t_12 = __pyx_convert_vector_from_py_double(__pyx_v_beta_schedule); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 156, __pyx_L1_error)
   __pyx_v__beta_schedule = __pyx_t_12;
 
-  /* "dwave/samplers/sa/simulated_annealing.pyx":129
+  /* "dwave/samplers/sa/simulated_annealing.pyx":157
  *     cdef int _sweeps_per_beta = sweeps_per_beta
  *     cdef vector[double] _beta_schedule = beta_schedule
  *     cdef unsigned long long _seed = seed             # <<<<<<<<<<<<<<
- * 
- *     cdef void* _interrupt_function
+ *     cdef VariableOrder _varorder
+ *     if randomize_order:
  */
-  __pyx_t_14 = __Pyx_PyInt_As_unsigned_PY_LONG_LONG(__pyx_v_seed); if (unlikely((__pyx_t_14 == (unsigned PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 129, __pyx_L1_error)
+  __pyx_t_14 = __Pyx_PyInt_As_unsigned_PY_LONG_LONG(__pyx_v_seed); if (unlikely((__pyx_t_14 == (unsigned PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 157, __pyx_L1_error)
   __pyx_v__seed = __pyx_t_14;
 
-  /* "dwave/samplers/sa/simulated_annealing.pyx":132
- * 
+  /* "dwave/samplers/sa/simulated_annealing.pyx":159
+ *     cdef unsigned long long _seed = seed
+ *     cdef VariableOrder _varorder
+ *     if randomize_order:             # <<<<<<<<<<<<<<
+ *         _varorder = Random
+ *     else:
+ */
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_v_randomize_order); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 159, __pyx_L1_error)
+  if (__pyx_t_4) {
+
+    /* "dwave/samplers/sa/simulated_annealing.pyx":160
+ *     cdef VariableOrder _varorder
+ *     if randomize_order:
+ *         _varorder = Random             # <<<<<<<<<<<<<<
+ *     else:
+ *         _varorder = Sequential
+ */
+    __pyx_v__varorder = Random;
+
+    /* "dwave/samplers/sa/simulated_annealing.pyx":159
+ *     cdef unsigned long long _seed = seed
+ *     cdef VariableOrder _varorder
+ *     if randomize_order:             # <<<<<<<<<<<<<<
+ *         _varorder = Random
+ *     else:
+ */
+    goto __pyx_L4;
+  }
+
+  /* "dwave/samplers/sa/simulated_annealing.pyx":162
+ *         _varorder = Random
+ *     else:
+ *         _varorder = Sequential             # <<<<<<<<<<<<<<
+ *     cdef Proposal _proposal_acceptance_criteria
+ *     if proposal_acceptance_criteria.lower() == 'gibbs':
+ */
+  /*else*/ {
+    __pyx_v__varorder = Sequential;
+  }
+  __pyx_L4:;
+
+  /* "dwave/samplers/sa/simulated_annealing.pyx":164
+ *         _varorder = Sequential
+ *     cdef Proposal _proposal_acceptance_criteria
+ *     if proposal_acceptance_criteria.lower() == 'gibbs':             # <<<<<<<<<<<<<<
+ *         _proposal_acceptance_criteria = Gibbs
+ *     elif proposal_acceptance_criteria.lower() == 'metropolis':
+ */
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_proposal_acceptance_criteria, __pyx_n_s_lower); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 164, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_7))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_7);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
+      __Pyx_INCREF(__pyx_t_5);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_7, function);
+    }
+  }
+  __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 164, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_t_2, __pyx_n_u_gibbs, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 164, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (__pyx_t_4) {
+
+    /* "dwave/samplers/sa/simulated_annealing.pyx":165
+ *     cdef Proposal _proposal_acceptance_criteria
+ *     if proposal_acceptance_criteria.lower() == 'gibbs':
+ *         _proposal_acceptance_criteria = Gibbs             # <<<<<<<<<<<<<<
+ *     elif proposal_acceptance_criteria.lower() == 'metropolis':
+ *         _proposal_acceptance_criteria = Metropolis
+ */
+    __pyx_v__proposal_acceptance_criteria = Gibbs;
+
+    /* "dwave/samplers/sa/simulated_annealing.pyx":164
+ *         _varorder = Sequential
+ *     cdef Proposal _proposal_acceptance_criteria
+ *     if proposal_acceptance_criteria.lower() == 'gibbs':             # <<<<<<<<<<<<<<
+ *         _proposal_acceptance_criteria = Gibbs
+ *     elif proposal_acceptance_criteria.lower() == 'metropolis':
+ */
+    goto __pyx_L5;
+  }
+
+  /* "dwave/samplers/sa/simulated_annealing.pyx":166
+ *     if proposal_acceptance_criteria.lower() == 'gibbs':
+ *         _proposal_acceptance_criteria = Gibbs
+ *     elif proposal_acceptance_criteria.lower() == 'metropolis':             # <<<<<<<<<<<<<<
+ *         _proposal_acceptance_criteria = Metropolis
+ *     else:
+ */
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_proposal_acceptance_criteria, __pyx_n_s_lower); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 166, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_7))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_7);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
+      __Pyx_INCREF(__pyx_t_5);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_7, function);
+    }
+  }
+  __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 166, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_t_2, __pyx_n_u_metropolis, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 166, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (likely(__pyx_t_4)) {
+
+    /* "dwave/samplers/sa/simulated_annealing.pyx":167
+ *         _proposal_acceptance_criteria = Gibbs
+ *     elif proposal_acceptance_criteria.lower() == 'metropolis':
+ *         _proposal_acceptance_criteria = Metropolis             # <<<<<<<<<<<<<<
+ *     else:
+ *         raise ValueError(f'Unknown proposal_acceptance_criteria: {proposal_acceptance_criteria}')
+ */
+    __pyx_v__proposal_acceptance_criteria = Metropolis;
+
+    /* "dwave/samplers/sa/simulated_annealing.pyx":166
+ *     if proposal_acceptance_criteria.lower() == 'gibbs':
+ *         _proposal_acceptance_criteria = Gibbs
+ *     elif proposal_acceptance_criteria.lower() == 'metropolis':             # <<<<<<<<<<<<<<
+ *         _proposal_acceptance_criteria = Metropolis
+ *     else:
+ */
+    goto __pyx_L5;
+  }
+
+  /* "dwave/samplers/sa/simulated_annealing.pyx":169
+ *         _proposal_acceptance_criteria = Metropolis
+ *     else:
+ *         raise ValueError(f'Unknown proposal_acceptance_criteria: {proposal_acceptance_criteria}')             # <<<<<<<<<<<<<<
+ *     cdef void* _interrupt_function
+ *     if interrupt_function is None:
+ */
+  /*else*/ {
+    __pyx_t_2 = __Pyx_PyObject_FormatSimple(__pyx_v_proposal_acceptance_criteria, __pyx_empty_unicode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 169, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_7 = __Pyx_PyUnicode_Concat(__pyx_kp_u_Unknown_proposal_acceptance_crit, __pyx_t_2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 169, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 169, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __Pyx_Raise(__pyx_t_2, 0, 0, 0);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __PYX_ERR(0, 169, __pyx_L1_error)
+  }
+  __pyx_L5:;
+
+  /* "dwave/samplers/sa/simulated_annealing.pyx":171
+ *         raise ValueError(f'Unknown proposal_acceptance_criteria: {proposal_acceptance_criteria}')
  *     cdef void* _interrupt_function
  *     if interrupt_function is None:             # <<<<<<<<<<<<<<
  *         _interrupt_function = NULL
  *     else:
  */
   __pyx_t_4 = (__pyx_v_interrupt_function == Py_None);
   __pyx_t_15 = (__pyx_t_4 != 0);
   if (__pyx_t_15) {
 
-    /* "dwave/samplers/sa/simulated_annealing.pyx":133
+    /* "dwave/samplers/sa/simulated_annealing.pyx":172
  *     cdef void* _interrupt_function
  *     if interrupt_function is None:
  *         _interrupt_function = NULL             # <<<<<<<<<<<<<<
  *     else:
  *         _interrupt_function = <void *>interrupt_function
  */
     __pyx_v__interrupt_function = NULL;
 
-    /* "dwave/samplers/sa/simulated_annealing.pyx":132
- * 
+    /* "dwave/samplers/sa/simulated_annealing.pyx":171
+ *         raise ValueError(f'Unknown proposal_acceptance_criteria: {proposal_acceptance_criteria}')
  *     cdef void* _interrupt_function
  *     if interrupt_function is None:             # <<<<<<<<<<<<<<
  *         _interrupt_function = NULL
  *     else:
  */
-    goto __pyx_L4;
+    goto __pyx_L6;
   }
 
-  /* "dwave/samplers/sa/simulated_annealing.pyx":135
+  /* "dwave/samplers/sa/simulated_annealing.pyx":174
  *         _interrupt_function = NULL
  *     else:
  *         _interrupt_function = <void *>interrupt_function             # <<<<<<<<<<<<<<
  * 
- *     with nogil:
+ * 
  */
   /*else*/ {
     __pyx_v__interrupt_function = ((void *)__pyx_v_interrupt_function);
   }
-  __pyx_L4:;
+  __pyx_L6:;
 
-  /* "dwave/samplers/sa/simulated_annealing.pyx":137
- *         _interrupt_function = <void *>interrupt_function
+  /* "dwave/samplers/sa/simulated_annealing.pyx":177
+ * 
  * 
  *     with nogil:             # <<<<<<<<<<<<<<
  *         num = general_simulated_annealing(_states,
  *                                           _energies,
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "dwave/samplers/sa/simulated_annealing.pyx":138
+        /* "dwave/samplers/sa/simulated_annealing.pyx":178
  * 
  *     with nogil:
  *         num = general_simulated_annealing(_states,             # <<<<<<<<<<<<<<
  *                                           _energies,
  *                                           _num_samples,
  */
-        __pyx_v_num = general_simulated_annealing(__pyx_v__states, __pyx_v__energies, __pyx_v__num_samples, __pyx_v__h, __pyx_v__coupler_starts, __pyx_v__coupler_ends, __pyx_v__coupler_weights, __pyx_v__sweeps_per_beta, __pyx_v__beta_schedule, __pyx_v__seed, __pyx_f_5dwave_8samplers_2sa_19simulated_annealing_interrupt_callback, __pyx_v__interrupt_function);
+        __pyx_v_num = general_simulated_annealing(__pyx_v__states, __pyx_v__energies, __pyx_v__num_samples, __pyx_v__h, __pyx_v__coupler_starts, __pyx_v__coupler_ends, __pyx_v__coupler_weights, __pyx_v__sweeps_per_beta, __pyx_v__beta_schedule, __pyx_v__seed, __pyx_v__varorder, __pyx_v__proposal_acceptance_criteria, __pyx_f_5dwave_8samplers_2sa_19simulated_annealing_interrupt_callback, __pyx_v__interrupt_function);
       }
 
-      /* "dwave/samplers/sa/simulated_annealing.pyx":137
- *         _interrupt_function = <void *>interrupt_function
+      /* "dwave/samplers/sa/simulated_annealing.pyx":177
+ * 
  * 
  *     with nogil:             # <<<<<<<<<<<<<<
  *         num = general_simulated_annealing(_states,
  *                                           _energies,
  */
       /*finally:*/ {
         /*normal exit:*/{
           #ifdef WITH_THREAD
           __Pyx_FastGIL_Forget();
           Py_BLOCK_THREADS
           #endif
-          goto __pyx_L7;
+          goto __pyx_L9;
         }
-        __pyx_L7:;
+        __pyx_L9:;
       }
   }
 
-  /* "dwave/samplers/sa/simulated_annealing.pyx":152
+  /* "dwave/samplers/sa/simulated_annealing.pyx":194
  * 
  *     # discard the noise if we were interrupted
  *     return states_numpy[:num], energies_numpy[:num]             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_num); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 152, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_num); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 194, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_7 = PySlice_New(Py_None, __pyx_t_2, Py_None); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 152, __pyx_L1_error)
+  __pyx_t_7 = PySlice_New(Py_None, __pyx_t_2, Py_None); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 194, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_states_numpy), __pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 152, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_states_numpy), __pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 194, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_t_7 = __Pyx_PyObject_GetSlice(__pyx_v_energies_numpy, 0, __pyx_v_num, NULL, NULL, NULL, 0, 1, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 152, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetSlice(__pyx_v_energies_numpy, 0, __pyx_v_num, NULL, NULL, NULL, 0, 1, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 194, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 152, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 194, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_7);
   PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_7);
   __pyx_t_2 = 0;
   __pyx_t_7 = 0;
   __pyx_r = __pyx_t_5;
   __pyx_t_5 = 0;
   goto __pyx_L0;
 
-  /* "dwave/samplers/sa/simulated_annealing.pyx":45
+  /* "dwave/samplers/sa/simulated_annealing.pyx":50
  * 
  * 
  * def simulated_annealing(num_samples, h, coupler_starts, coupler_ends,             # <<<<<<<<<<<<<<
  *                         coupler_weights, sweeps_per_beta, beta_schedule, seed,
- *                         np.ndarray[char, ndim=2, mode="c"] states_numpy,
+ *                         np.ndarray[np.int8_t, ndim=2, mode="c"] states_numpy,
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_5);
@@ -3349,15 +3569,15 @@
   __Pyx_XDECREF(__pyx_v_energies_numpy);
   __PYX_XDEC_MEMVIEW(&__pyx_v_energies, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "dwave/samplers/sa/simulated_annealing.pyx":155
+/* "dwave/samplers/sa/simulated_annealing.pyx":197
  * 
  * 
  * cdef bool interrupt_callback(void * const interrupt_function) with gil:             # <<<<<<<<<<<<<<
  *     try:
  *         return (<object>interrupt_function)()
  */
 
@@ -3376,15 +3596,15 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
   __Pyx_RefNannySetupContext("interrupt_callback", 0);
 
-  /* "dwave/samplers/sa/simulated_annealing.pyx":156
+  /* "dwave/samplers/sa/simulated_annealing.pyx":198
  * 
  * cdef bool interrupt_callback(void * const interrupt_function) with gil:
  *     try:             # <<<<<<<<<<<<<<
  *         return (<object>interrupt_function)()
  *     except Exception:
  */
   {
@@ -3392,15 +3612,15 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "dwave/samplers/sa/simulated_annealing.pyx":157
+      /* "dwave/samplers/sa/simulated_annealing.pyx":199
  * cdef bool interrupt_callback(void * const interrupt_function) with gil:
  *     try:
  *         return (<object>interrupt_function)()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         # if an exception occurs, treat as an interrupt
  */
       __Pyx_INCREF(((PyObject *)__pyx_v_interrupt_function));
@@ -3412,65 +3632,65 @@
           __Pyx_INCREF(__pyx_t_6);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_5, function);
         }
       }
       __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_6) : __Pyx_PyObject_CallNoArg(__pyx_t_5);
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 157, __pyx_L3_error)
+      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 199, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely((__pyx_t_7 == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(0, 157, __pyx_L3_error)
+      __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely((__pyx_t_7 == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(0, 199, __pyx_L3_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_r = __pyx_t_7;
       goto __pyx_L7_try_return;
 
-      /* "dwave/samplers/sa/simulated_annealing.pyx":156
+      /* "dwave/samplers/sa/simulated_annealing.pyx":198
  * 
  * cdef bool interrupt_callback(void * const interrupt_function) with gil:
  *     try:             # <<<<<<<<<<<<<<
  *         return (<object>interrupt_function)()
  *     except Exception:
  */
     }
     __pyx_L3_error:;
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-    /* "dwave/samplers/sa/simulated_annealing.pyx":158
+    /* "dwave/samplers/sa/simulated_annealing.pyx":200
  *     try:
  *         return (<object>interrupt_function)()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         # if an exception occurs, treat as an interrupt
  *         return True
  */
     __pyx_t_8 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_8) {
       __Pyx_AddTraceback("dwave.samplers.sa.simulated_annealing.interrupt_callback", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_4, &__pyx_t_5, &__pyx_t_6) < 0) __PYX_ERR(0, 158, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_4, &__pyx_t_5, &__pyx_t_6) < 0) __PYX_ERR(0, 200, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
 
-      /* "dwave/samplers/sa/simulated_annealing.pyx":160
+      /* "dwave/samplers/sa/simulated_annealing.pyx":202
  *     except Exception:
  *         # if an exception occurs, treat as an interrupt
  *         return True             # <<<<<<<<<<<<<<
  */
       __pyx_r = 1;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       goto __pyx_L6_except_return;
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "dwave/samplers/sa/simulated_annealing.pyx":156
+    /* "dwave/samplers/sa/simulated_annealing.pyx":198
  * 
  * cdef bool interrupt_callback(void * const interrupt_function) with gil:
  *     try:             # <<<<<<<<<<<<<<
  *         return (<object>interrupt_function)()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
@@ -3488,15 +3708,15 @@
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L0;
   }
 
-  /* "dwave/samplers/sa/simulated_annealing.pyx":155
+  /* "dwave/samplers/sa/simulated_annealing.pyx":197
  * 
  * 
  * cdef bool interrupt_callback(void * const interrupt_function) with gil:             # <<<<<<<<<<<<<<
  *     try:
  *         return (<object>interrupt_function)()
  */
 
@@ -3511,15 +3731,15 @@
   __Pyx_RefNannyFinishContext();
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":735
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3528,29 +3748,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":736
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 736, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":735
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3561,15 +3781,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":738
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3578,29 +3798,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":739
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 739, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":738
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3611,15 +3831,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":741
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3628,29 +3848,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":742
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 742, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":741
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3661,15 +3881,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":744
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3678,29 +3898,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":745
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 745, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":744
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3711,15 +3931,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":747
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3728,29 +3948,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":748
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 748, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":747
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3761,212 +3981,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":750
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":751
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":752
+    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":751
+    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":754
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":750
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":929
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":868
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":930
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":869
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":931
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":870
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":929
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":868
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":933
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":872
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":934
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":873
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":935
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":874
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":936
+    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":875
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":935
+    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":874
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":937
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":876
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":933
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":872
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":941
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":880
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -3982,15 +4202,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":942
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":881
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -3998,84 +4218,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":943
+      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":882
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 943, __pyx_L3_error)
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 882, __pyx_L3_error)
 
-      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":942
+      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":881
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":944
+    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":883
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 944, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 883, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":945
+      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":884
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 945, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 884, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 945, __pyx_L5_except_error)
+      __PYX_ERR(1, 884, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":942
+    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":881
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":941
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":880
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4090,15 +4310,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":947
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":886
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4114,15 +4334,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":948
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":887
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4130,84 +4350,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":949
+      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":888
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 949, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 888, __pyx_L3_error)
 
-      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":948
+      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":887
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":950
+    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":889
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 950, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 889, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":951
+      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":890
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 951, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 890, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 951, __pyx_L5_except_error)
+      __PYX_ERR(1, 890, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":948
+    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":887
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":947
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":886
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4222,15 +4442,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":953
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":892
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4246,15 +4466,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":954
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":893
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4262,84 +4482,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":955
+      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":894
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 955, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 894, __pyx_L3_error)
 
-      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":954
+      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":893
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":956
+    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":895
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 956, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 895, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":957
+      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":896
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 957, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 896, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 957, __pyx_L5_except_error)
+      __PYX_ERR(1, 896, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":954
+    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":893
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":953
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":892
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4354,188 +4574,14 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":967
- * 
- * 
- * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
- *     """
- *     Cython equivalent of `isinstance(obj, np.timedelta64)`
- */
-
-static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
-
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":979
- *     bool
- *     """
- *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
-  goto __pyx_L0;
-
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":967
- * 
- * 
- * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
- *     """
- *     Cython equivalent of `isinstance(obj, np.timedelta64)`
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":982
- * 
- * 
- * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
- *     """
- *     Cython equivalent of `isinstance(obj, np.datetime64)`
- */
-
-static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("is_datetime64_object", 0);
-
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":994
- *     bool
- *     """
- *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
-  goto __pyx_L0;
-
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":982
- * 
- * 
- * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
- *     """
- *     Cython equivalent of `isinstance(obj, np.datetime64)`
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":997
- * 
- * 
- * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the int64 value underlying scalar numpy datetime64 object
- */
-
-static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
-  npy_datetime __pyx_r;
-
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":1004
- *     also needed.  That can be found using `get_datetime64_unit`.
- *     """
- *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
-  goto __pyx_L0;
-
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":997
- * 
- * 
- * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the int64 value underlying scalar numpy datetime64 object
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  return __pyx_r;
-}
-
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":1007
- * 
- * 
- * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the int64 value underlying scalar numpy timedelta64 object
- */
-
-static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
-  npy_timedelta __pyx_r;
-
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":1011
- *     returns the int64 value underlying scalar numpy timedelta64 object
- *     """
- *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
-  goto __pyx_L0;
-
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":1007
- * 
- * 
- * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the int64 value underlying scalar numpy timedelta64 object
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  return __pyx_r;
-}
-
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":1014
- * 
- * 
- * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the unit part of the dtype for a numpy datetime64 object.
- */
-
-static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
-  NPY_DATETIMEUNIT __pyx_r;
-
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":1018
- *     returns the unit part of the dtype for a numpy datetime64 object.
- *     """
- *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
- */
-  __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
-  goto __pyx_L0;
-
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":1014
- * 
- * 
- * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the unit part of the dtype for a numpy datetime64 object.
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  return __pyx_r;
-}
-
 /* "vector.from_py":45
  * 
  * @cname("__pyx_convert_vector_from_py_double")
  * cdef vector[X] __pyx_convert_vector_from_py_double(object o) except *:             # <<<<<<<<<<<<<<
  *     cdef vector[X] v
  *     for item in o:
  */
@@ -18572,19 +18618,21 @@
   {&__pyx_n_s_IndexError, __pyx_k_IndexError, sizeof(__pyx_k_IndexError), 0, 0, 1, 1},
   {&__pyx_kp_s_Indirect_dimensions_not_supporte, __pyx_k_Indirect_dimensions_not_supporte, sizeof(__pyx_k_Indirect_dimensions_not_supporte), 0, 0, 1, 0},
   {&__pyx_kp_s_Invalid_mode_expected_c_or_fortr, __pyx_k_Invalid_mode_expected_c_or_fortr, sizeof(__pyx_k_Invalid_mode_expected_c_or_fortr), 0, 0, 1, 0},
   {&__pyx_kp_s_Invalid_shape_in_axis_d_d, __pyx_k_Invalid_shape_in_axis_d_d, sizeof(__pyx_k_Invalid_shape_in_axis_d_d), 0, 0, 1, 0},
   {&__pyx_n_s_MemoryError, __pyx_k_MemoryError, sizeof(__pyx_k_MemoryError), 0, 0, 1, 1},
   {&__pyx_kp_s_MemoryView_of_r_at_0x_x, __pyx_k_MemoryView_of_r_at_0x_x, sizeof(__pyx_k_MemoryView_of_r_at_0x_x), 0, 0, 1, 0},
   {&__pyx_kp_s_MemoryView_of_r_object, __pyx_k_MemoryView_of_r_object, sizeof(__pyx_k_MemoryView_of_r_object), 0, 0, 1, 0},
+  {&__pyx_n_u_Metropolis, __pyx_k_Metropolis, sizeof(__pyx_k_Metropolis), 0, 1, 0, 1},
   {&__pyx_n_b_O, __pyx_k_O, sizeof(__pyx_k_O), 0, 0, 0, 1},
   {&__pyx_kp_s_Out_of_bounds_on_buffer_access_a, __pyx_k_Out_of_bounds_on_buffer_access_a, sizeof(__pyx_k_Out_of_bounds_on_buffer_access_a), 0, 0, 1, 0},
   {&__pyx_n_s_PickleError, __pyx_k_PickleError, sizeof(__pyx_k_PickleError), 0, 0, 1, 1},
   {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
   {&__pyx_kp_s_Unable_to_convert_item_to_object, __pyx_k_Unable_to_convert_item_to_object, sizeof(__pyx_k_Unable_to_convert_item_to_object), 0, 0, 1, 0},
+  {&__pyx_kp_u_Unknown_proposal_acceptance_crit, __pyx_k_Unknown_proposal_acceptance_crit, sizeof(__pyx_k_Unknown_proposal_acceptance_crit), 0, 1, 0, 0},
   {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
   {&__pyx_n_s_View_MemoryView, __pyx_k_View_MemoryView, sizeof(__pyx_k_View_MemoryView), 0, 0, 1, 1},
   {&__pyx_n_s_allocate_buffer, __pyx_k_allocate_buffer, sizeof(__pyx_k_allocate_buffer), 0, 0, 1, 1},
   {&__pyx_n_s_annealed_states, __pyx_k_annealed_states, sizeof(__pyx_k_annealed_states), 0, 0, 1, 1},
   {&__pyx_n_s_base, __pyx_k_base, sizeof(__pyx_k_base), 0, 0, 1, 1},
   {&__pyx_n_s_beta_schedule, __pyx_k_beta_schedule, sizeof(__pyx_k_beta_schedule), 0, 0, 1, 1},
   {&__pyx_n_s_beta_schedule_2, __pyx_k_beta_schedule_2, sizeof(__pyx_k_beta_schedule_2), 0, 0, 1, 1},
@@ -18615,26 +18663,29 @@
   {&__pyx_n_s_error, __pyx_k_error, sizeof(__pyx_k_error), 0, 0, 1, 1},
   {&__pyx_n_s_flags, __pyx_k_flags, sizeof(__pyx_k_flags), 0, 0, 1, 1},
   {&__pyx_n_s_float64, __pyx_k_float64, sizeof(__pyx_k_float64), 0, 0, 1, 1},
   {&__pyx_n_s_format, __pyx_k_format, sizeof(__pyx_k_format), 0, 0, 1, 1},
   {&__pyx_n_s_fortran, __pyx_k_fortran, sizeof(__pyx_k_fortran), 0, 0, 1, 1},
   {&__pyx_n_u_fortran, __pyx_k_fortran, sizeof(__pyx_k_fortran), 0, 1, 0, 1},
   {&__pyx_n_s_getstate, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
+  {&__pyx_n_u_gibbs, __pyx_k_gibbs, sizeof(__pyx_k_gibbs), 0, 1, 0, 1},
   {&__pyx_kp_s_got_differing_extents_in_dimensi, __pyx_k_got_differing_extents_in_dimensi, sizeof(__pyx_k_got_differing_extents_in_dimensi), 0, 0, 1, 0},
   {&__pyx_n_s_h, __pyx_k_h, sizeof(__pyx_k_h), 0, 0, 1, 1},
   {&__pyx_n_s_h_2, __pyx_k_h_2, sizeof(__pyx_k_h_2), 0, 0, 1, 1},
   {&__pyx_n_s_id, __pyx_k_id, sizeof(__pyx_k_id), 0, 0, 1, 1},
   {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
   {&__pyx_n_s_int8, __pyx_k_int8, sizeof(__pyx_k_int8), 0, 0, 1, 1},
   {&__pyx_n_s_interrupt_function, __pyx_k_interrupt_function, sizeof(__pyx_k_interrupt_function), 0, 0, 1, 1},
   {&__pyx_n_s_interrupt_function_2, __pyx_k_interrupt_function_2, sizeof(__pyx_k_interrupt_function_2), 0, 0, 1, 1},
   {&__pyx_n_s_itemsize, __pyx_k_itemsize, sizeof(__pyx_k_itemsize), 0, 0, 1, 1},
   {&__pyx_kp_s_itemsize_0_for_cython_array, __pyx_k_itemsize_0_for_cython_array, sizeof(__pyx_k_itemsize_0_for_cython_array), 0, 0, 1, 0},
+  {&__pyx_n_s_lower, __pyx_k_lower, sizeof(__pyx_k_lower), 0, 0, 1, 1},
   {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
   {&__pyx_n_s_memview, __pyx_k_memview, sizeof(__pyx_k_memview), 0, 0, 1, 1},
+  {&__pyx_n_u_metropolis, __pyx_k_metropolis, sizeof(__pyx_k_metropolis), 0, 1, 0, 1},
   {&__pyx_n_s_mode, __pyx_k_mode, sizeof(__pyx_k_mode), 0, 0, 1, 1},
   {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
   {&__pyx_n_s_name_2, __pyx_k_name_2, sizeof(__pyx_k_name_2), 0, 0, 1, 1},
   {&__pyx_n_s_ndim, __pyx_k_ndim, sizeof(__pyx_k_ndim), 0, 0, 1, 1},
   {&__pyx_n_s_new, __pyx_k_new, sizeof(__pyx_k_new), 0, 0, 1, 1},
   {&__pyx_kp_s_no_default___reduce___due_to_non, __pyx_k_no_default___reduce___due_to_non, sizeof(__pyx_k_no_default___reduce___due_to_non), 0, 0, 1, 0},
   {&__pyx_n_s_np, __pyx_k_np, sizeof(__pyx_k_np), 0, 0, 1, 1},
@@ -18644,22 +18695,25 @@
   {&__pyx_n_s_num_vars, __pyx_k_num_vars, sizeof(__pyx_k_num_vars), 0, 0, 1, 1},
   {&__pyx_n_s_numpy, __pyx_k_numpy, sizeof(__pyx_k_numpy), 0, 0, 1, 1},
   {&__pyx_kp_u_numpy_core_multiarray_failed_to, __pyx_k_numpy_core_multiarray_failed_to, sizeof(__pyx_k_numpy_core_multiarray_failed_to), 0, 1, 0, 0},
   {&__pyx_kp_u_numpy_core_umath_failed_to_impor, __pyx_k_numpy_core_umath_failed_to_impor, sizeof(__pyx_k_numpy_core_umath_failed_to_impor), 0, 1, 0, 0},
   {&__pyx_n_s_obj, __pyx_k_obj, sizeof(__pyx_k_obj), 0, 0, 1, 1},
   {&__pyx_n_s_pack, __pyx_k_pack, sizeof(__pyx_k_pack), 0, 0, 1, 1},
   {&__pyx_n_s_pickle, __pyx_k_pickle, sizeof(__pyx_k_pickle), 0, 0, 1, 1},
+  {&__pyx_n_s_proposal_acceptance_criteria, __pyx_k_proposal_acceptance_criteria, sizeof(__pyx_k_proposal_acceptance_criteria), 0, 0, 1, 1},
+  {&__pyx_n_s_proposal_acceptance_criteria_2, __pyx_k_proposal_acceptance_criteria_2, sizeof(__pyx_k_proposal_acceptance_criteria_2), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_PickleError, __pyx_k_pyx_PickleError, sizeof(__pyx_k_pyx_PickleError), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_checksum, __pyx_k_pyx_checksum, sizeof(__pyx_k_pyx_checksum), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_getbuffer, __pyx_k_pyx_getbuffer, sizeof(__pyx_k_pyx_getbuffer), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_result, __pyx_k_pyx_result, sizeof(__pyx_k_pyx_result), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_state, __pyx_k_pyx_state, sizeof(__pyx_k_pyx_state), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_type, __pyx_k_pyx_type, sizeof(__pyx_k_pyx_type), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_unpickle_Enum, __pyx_k_pyx_unpickle_Enum, sizeof(__pyx_k_pyx_unpickle_Enum), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_vtable, __pyx_k_pyx_vtable, sizeof(__pyx_k_pyx_vtable), 0, 0, 1, 1},
+  {&__pyx_n_s_randomize_order, __pyx_k_randomize_order, sizeof(__pyx_k_randomize_order), 0, 0, 1, 1},
   {&__pyx_n_s_range, __pyx_k_range, sizeof(__pyx_k_range), 0, 0, 1, 1},
   {&__pyx_n_s_reduce, __pyx_k_reduce, sizeof(__pyx_k_reduce), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_cython, __pyx_k_reduce_cython, sizeof(__pyx_k_reduce_cython), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_ex, __pyx_k_reduce_ex, sizeof(__pyx_k_reduce_ex), 0, 0, 1, 1},
   {&__pyx_n_s_seed, __pyx_k_seed, sizeof(__pyx_k_seed), 0, 0, 1, 1},
   {&__pyx_n_s_seed_2, __pyx_k_seed_2, sizeof(__pyx_k_seed_2), 0, 0, 1, 1},
   {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
@@ -18680,20 +18734,21 @@
   {&__pyx_n_s_sweeps_per_beta, __pyx_k_sweeps_per_beta, sizeof(__pyx_k_sweeps_per_beta), 0, 0, 1, 1},
   {&__pyx_n_s_sweeps_per_beta_2, __pyx_k_sweeps_per_beta_2, sizeof(__pyx_k_sweeps_per_beta_2), 0, 0, 1, 1},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_kp_s_unable_to_allocate_array_data, __pyx_k_unable_to_allocate_array_data, sizeof(__pyx_k_unable_to_allocate_array_data), 0, 0, 1, 0},
   {&__pyx_kp_s_unable_to_allocate_shape_and_str, __pyx_k_unable_to_allocate_shape_and_str, sizeof(__pyx_k_unable_to_allocate_shape_and_str), 0, 0, 1, 0},
   {&__pyx_n_s_unpack, __pyx_k_unpack, sizeof(__pyx_k_unpack), 0, 0, 1, 1},
   {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
+  {&__pyx_n_s_varorder, __pyx_k_varorder, sizeof(__pyx_k_varorder), 0, 0, 1, 1},
   {&__pyx_n_s_zeros, __pyx_k_zeros, sizeof(__pyx_k_zeros), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 945, __pyx_L1_error)
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(2, 133, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 169, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 884, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(2, 148, __pyx_L1_error)
   __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(2, 151, __pyx_L1_error)
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(2, 180, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(2, 2, __pyx_L1_error)
   __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(2, 404, __pyx_L1_error)
   __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(2, 613, __pyx_L1_error)
   __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(2, 832, __pyx_L1_error)
@@ -18702,33 +18757,33 @@
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":945
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":884
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 945, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 884, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":951
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":890
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 951, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 890, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
   /* "View.MemoryView":133
  * 
  *         if not self.ndim:
  *             raise ValueError("Empty shape tuple for cython.array")             # <<<<<<<<<<<<<<
@@ -18916,25 +18971,25 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__20 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(2, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__20);
   __Pyx_GIVEREF(__pyx_tuple__20);
 
-  /* "dwave/samplers/sa/simulated_annealing.pyx":45
+  /* "dwave/samplers/sa/simulated_annealing.pyx":50
  * 
  * 
  * def simulated_annealing(num_samples, h, coupler_starts, coupler_ends,             # <<<<<<<<<<<<<<
  *                         coupler_weights, sweeps_per_beta, beta_schedule, seed,
- *                         np.ndarray[char, ndim=2, mode="c"] states_numpy,
+ *                         np.ndarray[np.int8_t, ndim=2, mode="c"] states_numpy,
  */
-  __pyx_tuple__21 = PyTuple_Pack(26, __pyx_n_s_num_samples, __pyx_n_s_h, __pyx_n_s_coupler_starts, __pyx_n_s_coupler_ends, __pyx_n_s_coupler_weights, __pyx_n_s_sweeps_per_beta, __pyx_n_s_beta_schedule, __pyx_n_s_seed, __pyx_n_s_states_numpy, __pyx_n_s_interrupt_function, __pyx_n_s_num_vars, __pyx_n_s_annealed_states, __pyx_n_s_energies_numpy, __pyx_n_s_energies, __pyx_n_s_states, __pyx_n_s_energies_2, __pyx_n_s_num_samples_2, __pyx_n_s_h_2, __pyx_n_s_coupler_starts_2, __pyx_n_s_coupler_ends_2, __pyx_n_s_coupler_weights_2, __pyx_n_s_sweeps_per_beta_2, __pyx_n_s_beta_schedule_2, __pyx_n_s_seed_2, __pyx_n_s_interrupt_function_2, __pyx_n_s_num); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(0, 45, __pyx_L1_error)
+  __pyx_tuple__21 = PyTuple_Pack(30, __pyx_n_s_num_samples, __pyx_n_s_h, __pyx_n_s_coupler_starts, __pyx_n_s_coupler_ends, __pyx_n_s_coupler_weights, __pyx_n_s_sweeps_per_beta, __pyx_n_s_beta_schedule, __pyx_n_s_seed, __pyx_n_s_states_numpy, __pyx_n_s_randomize_order, __pyx_n_s_proposal_acceptance_criteria, __pyx_n_s_interrupt_function, __pyx_n_s_num_vars, __pyx_n_s_annealed_states, __pyx_n_s_energies_numpy, __pyx_n_s_energies, __pyx_n_s_states, __pyx_n_s_energies_2, __pyx_n_s_num_samples_2, __pyx_n_s_h_2, __pyx_n_s_coupler_starts_2, __pyx_n_s_coupler_ends_2, __pyx_n_s_coupler_weights_2, __pyx_n_s_sweeps_per_beta_2, __pyx_n_s_beta_schedule_2, __pyx_n_s_seed_2, __pyx_n_s_varorder, __pyx_n_s_proposal_acceptance_criteria_2, __pyx_n_s_interrupt_function_2, __pyx_n_s_num); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(0, 50, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__21);
   __Pyx_GIVEREF(__pyx_tuple__21);
-  __pyx_codeobj__22 = (PyObject*)__Pyx_PyCode_New(10, 0, 26, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__21, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_dwave_samplers_sa_simulated_anne, __pyx_n_s_simulated_annealing, 45, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__22)) __PYX_ERR(0, 45, __pyx_L1_error)
+  __pyx_codeobj__22 = (PyObject*)__Pyx_PyCode_New(12, 0, 30, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__21, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_dwave_samplers_sa_simulated_anne, __pyx_n_s_simulated_annealing, 50, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__22)) __PYX_ERR(0, 50, __pyx_L1_error)
 
   /* "View.MemoryView":286
  *         return self.name
  * 
  * cdef generic = Enum("<strided and direct or indirect>")             # <<<<<<<<<<<<<<
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")
@@ -19131,46 +19186,26 @@
   sizeof(PyTypeObject),
   #else
   sizeof(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 200, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 200, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 199, __pyx_L1_error)
   __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 223, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 222, __pyx_L1_error)
   __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 227, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 226, __pyx_L1_error)
   __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 239, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 771, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 773, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 775, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 777, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 779, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 781, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 783, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 785, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 787, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 789, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
   __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 827, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 764, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -19401,24 +19436,24 @@
  * 
  */
   __pyx_t_1 = __Pyx_Import(__pyx_n_s_numpy, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 23, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_np, __pyx_t_1) < 0) __PYX_ERR(0, 23, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "dwave/samplers/sa/simulated_annealing.pyx":45
+  /* "dwave/samplers/sa/simulated_annealing.pyx":50
  * 
  * 
  * def simulated_annealing(num_samples, h, coupler_starts, coupler_ends,             # <<<<<<<<<<<<<<
  *                         coupler_weights, sweeps_per_beta, beta_schedule, seed,
- *                         np.ndarray[char, ndim=2, mode="c"] states_numpy,
+ *                         np.ndarray[np.int8_t, ndim=2, mode="c"] states_numpy,
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_5dwave_8samplers_2sa_19simulated_annealing_1simulated_annealing, NULL, __pyx_n_s_dwave_samplers_sa_simulated_anne_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 45, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_5dwave_8samplers_2sa_19simulated_annealing_1simulated_annealing, NULL, __pyx_n_s_dwave_samplers_sa_simulated_anne_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 50, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_simulated_annealing, __pyx_t_1) < 0) __PYX_ERR(0, 45, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_simulated_annealing, __pyx_t_1) < 0) __PYX_ERR(0, 50, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "dwave/samplers/sa/simulated_annealing.pyx":1
  * # distutils: language = c++             # <<<<<<<<<<<<<<
  * # distutils: include_dirs = dwave/samplers/sa/src/
  * # distutils: sources = dwave/samplers/sa/src/cpu_sa.cpp
  */
@@ -19618,14 +19653,42 @@
 end:
     Py_XDECREF(p);
     Py_XDECREF(m);
     return (__Pyx_RefNannyAPIStruct *)r;
 }
 #endif
 
+/* PyObjectGetAttrStr */
+#if CYTHON_USE_TYPE_SLOTS
+static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStr(PyObject* obj, PyObject* attr_name) {
+    PyTypeObject* tp = Py_TYPE(obj);
+    if (likely(tp->tp_getattro))
+        return tp->tp_getattro(obj, attr_name);
+#if PY_MAJOR_VERSION < 3
+    if (likely(tp->tp_getattr))
+        return tp->tp_getattr(obj, PyString_AS_STRING(attr_name));
+#endif
+    return PyObject_GetAttr(obj, attr_name);
+}
+#endif
+
+/* GetBuiltinName */
+static PyObject *__Pyx_GetBuiltinName(PyObject *name) {
+    PyObject* result = __Pyx_PyObject_GetAttrStr(__pyx_b, name);
+    if (unlikely(!result)) {
+        PyErr_Format(PyExc_NameError,
+#if PY_MAJOR_VERSION >= 3
+            "name '%U' is not defined", name);
+#else
+            "name '%.200s' is not defined", PyString_AS_STRING(name));
+#endif
+    }
+    return result;
+}
+
 /* RaiseArgTupleInvalid */
 static void __Pyx_RaiseArgtupleInvalid(
     const char* func_name,
     int exact,
     Py_ssize_t num_min,
     Py_ssize_t num_max,
     Py_ssize_t num_found)
@@ -20408,42 +20471,14 @@
         double a = PyFloat_AS_DOUBLE(op1);
         if ((double)a == (double)b) Py_RETURN_TRUE; else Py_RETURN_FALSE;
     }
     return (
         PyObject_RichCompare(op1, op2, Py_EQ));
 }
 
-/* PyObjectGetAttrStr */
-  #if CYTHON_USE_TYPE_SLOTS
-static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStr(PyObject* obj, PyObject* attr_name) {
-    PyTypeObject* tp = Py_TYPE(obj);
-    if (likely(tp->tp_getattro))
-        return tp->tp_getattro(obj, attr_name);
-#if PY_MAJOR_VERSION < 3
-    if (likely(tp->tp_getattr))
-        return tp->tp_getattr(obj, PyString_AS_STRING(attr_name));
-#endif
-    return PyObject_GetAttr(obj, attr_name);
-}
-#endif
-
-/* GetBuiltinName */
-  static PyObject *__Pyx_GetBuiltinName(PyObject *name) {
-    PyObject* result = __Pyx_PyObject_GetAttrStr(__pyx_b, name);
-    if (unlikely(!result)) {
-        PyErr_Format(PyExc_NameError,
-#if PY_MAJOR_VERSION >= 3
-            "name '%U' is not defined", name);
-#else
-            "name '%.200s' is not defined", PyString_AS_STRING(name));
-#endif
-    }
-    return result;
-}
-
 /* PyDictVersioning */
   #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
 static CYTHON_INLINE PY_UINT64_T __Pyx_get_tp_dict_version(PyObject *obj) {
     PyObject *dict = Py_TYPE(obj)->tp_dict;
     return likely(dict) ? __PYX_GET_DICT_VERSION(dict) : 0;
 }
 static CYTHON_INLINE PY_UINT64_T __Pyx_get_object_dict_version(PyObject *obj) {
@@ -20523,14 +20558,570 @@
 
 /* BufferIndexError */
   static void __Pyx_RaiseBufferIndexError(int axis) {
   PyErr_Format(PyExc_IndexError,
      "Out of bounds on buffer access (axis %d)", axis);
 }
 
+/* PyFunctionFastCall */
+  #if CYTHON_FAST_PYCALL
+static PyObject* __Pyx_PyFunction_FastCallNoKw(PyCodeObject *co, PyObject **args, Py_ssize_t na,
+                                               PyObject *globals) {
+    PyFrameObject *f;
+    PyThreadState *tstate = __Pyx_PyThreadState_Current;
+    PyObject **fastlocals;
+    Py_ssize_t i;
+    PyObject *result;
+    assert(globals != NULL);
+    /* XXX Perhaps we should create a specialized
+       PyFrame_New() that doesn't take locals, but does
+       take builtins without sanity checking them.
+       */
+    assert(tstate != NULL);
+    f = PyFrame_New(tstate, co, globals, NULL);
+    if (f == NULL) {
+        return NULL;
+    }
+    fastlocals = __Pyx_PyFrame_GetLocalsplus(f);
+    for (i = 0; i < na; i++) {
+        Py_INCREF(*args);
+        fastlocals[i] = *args++;
+    }
+    result = PyEval_EvalFrameEx(f,0);
+    ++tstate->recursion_depth;
+    Py_DECREF(f);
+    --tstate->recursion_depth;
+    return result;
+}
+#if 1 || PY_VERSION_HEX < 0x030600B1
+static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs) {
+    PyCodeObject *co = (PyCodeObject *)PyFunction_GET_CODE(func);
+    PyObject *globals = PyFunction_GET_GLOBALS(func);
+    PyObject *argdefs = PyFunction_GET_DEFAULTS(func);
+    PyObject *closure;
+#if PY_MAJOR_VERSION >= 3
+    PyObject *kwdefs;
+#endif
+    PyObject *kwtuple, **k;
+    PyObject **d;
+    Py_ssize_t nd;
+    Py_ssize_t nk;
+    PyObject *result;
+    assert(kwargs == NULL || PyDict_Check(kwargs));
+    nk = kwargs ? PyDict_Size(kwargs) : 0;
+    if (Py_EnterRecursiveCall((char*)" while calling a Python object")) {
+        return NULL;
+    }
+    if (
+#if PY_MAJOR_VERSION >= 3
+            co->co_kwonlyargcount == 0 &&
+#endif
+            likely(kwargs == NULL || nk == 0) &&
+            co->co_flags == (CO_OPTIMIZED | CO_NEWLOCALS | CO_NOFREE)) {
+        if (argdefs == NULL && co->co_argcount == nargs) {
+            result = __Pyx_PyFunction_FastCallNoKw(co, args, nargs, globals);
+            goto done;
+        }
+        else if (nargs == 0 && argdefs != NULL
+                 && co->co_argcount == Py_SIZE(argdefs)) {
+            /* function called with no arguments, but all parameters have
+               a default value: use default values as arguments .*/
+            args = &PyTuple_GET_ITEM(argdefs, 0);
+            result =__Pyx_PyFunction_FastCallNoKw(co, args, Py_SIZE(argdefs), globals);
+            goto done;
+        }
+    }
+    if (kwargs != NULL) {
+        Py_ssize_t pos, i;
+        kwtuple = PyTuple_New(2 * nk);
+        if (kwtuple == NULL) {
+            result = NULL;
+            goto done;
+        }
+        k = &PyTuple_GET_ITEM(kwtuple, 0);
+        pos = i = 0;
+        while (PyDict_Next(kwargs, &pos, &k[i], &k[i+1])) {
+            Py_INCREF(k[i]);
+            Py_INCREF(k[i+1]);
+            i += 2;
+        }
+        nk = i / 2;
+    }
+    else {
+        kwtuple = NULL;
+        k = NULL;
+    }
+    closure = PyFunction_GET_CLOSURE(func);
+#if PY_MAJOR_VERSION >= 3
+    kwdefs = PyFunction_GET_KW_DEFAULTS(func);
+#endif
+    if (argdefs != NULL) {
+        d = &PyTuple_GET_ITEM(argdefs, 0);
+        nd = Py_SIZE(argdefs);
+    }
+    else {
+        d = NULL;
+        nd = 0;
+    }
+#if PY_MAJOR_VERSION >= 3
+    result = PyEval_EvalCodeEx((PyObject*)co, globals, (PyObject *)NULL,
+                               args, (int)nargs,
+                               k, (int)nk,
+                               d, (int)nd, kwdefs, closure);
+#else
+    result = PyEval_EvalCodeEx(co, globals, (PyObject *)NULL,
+                               args, (int)nargs,
+                               k, (int)nk,
+                               d, (int)nd, closure);
+#endif
+    Py_XDECREF(kwtuple);
+done:
+    Py_LeaveRecursiveCall();
+    return result;
+}
+#endif
+#endif
+
+/* PyObjectCallMethO */
+  #if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg) {
+    PyObject *self, *result;
+    PyCFunction cfunc;
+    cfunc = PyCFunction_GET_FUNCTION(func);
+    self = PyCFunction_GET_SELF(func);
+    if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
+        return NULL;
+    result = cfunc(self, arg);
+    Py_LeaveRecursiveCall();
+    if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
+        PyErr_SetString(
+            PyExc_SystemError,
+            "NULL result without error in PyObject_Call");
+    }
+    return result;
+}
+#endif
+
+/* PyObjectCallNoArg */
+  #if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
+#if CYTHON_FAST_PYCALL
+    if (PyFunction_Check(func)) {
+        return __Pyx_PyFunction_FastCall(func, NULL, 0);
+    }
+#endif
+#ifdef __Pyx_CyFunction_USED
+    if (likely(PyCFunction_Check(func) || __Pyx_CyFunction_Check(func)))
+#else
+    if (likely(PyCFunction_Check(func)))
+#endif
+    {
+        if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
+            return __Pyx_PyObject_CallMethO(func, NULL);
+        }
+    }
+    return __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL);
+}
+#endif
+
+/* PyCFunctionFastCall */
+  #if CYTHON_FAST_PYCCALL
+static CYTHON_INLINE PyObject * __Pyx_PyCFunction_FastCall(PyObject *func_obj, PyObject **args, Py_ssize_t nargs) {
+    PyCFunctionObject *func = (PyCFunctionObject*)func_obj;
+    PyCFunction meth = PyCFunction_GET_FUNCTION(func);
+    PyObject *self = PyCFunction_GET_SELF(func);
+    int flags = PyCFunction_GET_FLAGS(func);
+    assert(PyCFunction_Check(func));
+    assert(METH_FASTCALL == (flags & ~(METH_CLASS | METH_STATIC | METH_COEXIST | METH_KEYWORDS | METH_STACKLESS)));
+    assert(nargs >= 0);
+    assert(nargs == 0 || args != NULL);
+    /* _PyCFunction_FastCallDict() must not be called with an exception set,
+       because it may clear it (directly or indirectly) and so the
+       caller loses its exception */
+    assert(!PyErr_Occurred());
+    if ((PY_VERSION_HEX < 0x030700A0) || unlikely(flags & METH_KEYWORDS)) {
+        return (*((__Pyx_PyCFunctionFastWithKeywords)(void*)meth)) (self, args, nargs, NULL);
+    } else {
+        return (*((__Pyx_PyCFunctionFast)(void*)meth)) (self, args, nargs);
+    }
+}
+#endif
+
+/* PyObjectCallOneArg */
+  #if CYTHON_COMPILING_IN_CPYTHON
+static PyObject* __Pyx__PyObject_CallOneArg(PyObject *func, PyObject *arg) {
+    PyObject *result;
+    PyObject *args = PyTuple_New(1);
+    if (unlikely(!args)) return NULL;
+    Py_INCREF(arg);
+    PyTuple_SET_ITEM(args, 0, arg);
+    result = __Pyx_PyObject_Call(func, args, NULL);
+    Py_DECREF(args);
+    return result;
+}
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg) {
+#if CYTHON_FAST_PYCALL
+    if (PyFunction_Check(func)) {
+        return __Pyx_PyFunction_FastCall(func, &arg, 1);
+    }
+#endif
+    if (likely(PyCFunction_Check(func))) {
+        if (likely(PyCFunction_GET_FLAGS(func) & METH_O)) {
+            return __Pyx_PyObject_CallMethO(func, arg);
+#if CYTHON_FAST_PYCCALL
+        } else if (__Pyx_PyFastCFunction_Check(func)) {
+            return __Pyx_PyCFunction_FastCall(func, &arg, 1);
+#endif
+        }
+    }
+    return __Pyx__PyObject_CallOneArg(func, arg);
+}
+#else
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg) {
+    PyObject *result;
+    PyObject *args = PyTuple_Pack(1, arg);
+    if (unlikely(!args)) return NULL;
+    result = __Pyx_PyObject_Call(func, args, NULL);
+    Py_DECREF(args);
+    return result;
+}
+#endif
+
+/* BytesEquals */
+  static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals) {
+#if CYTHON_COMPILING_IN_PYPY
+    return PyObject_RichCompareBool(s1, s2, equals);
+#else
+    if (s1 == s2) {
+        return (equals == Py_EQ);
+    } else if (PyBytes_CheckExact(s1) & PyBytes_CheckExact(s2)) {
+        const char *ps1, *ps2;
+        Py_ssize_t length = PyBytes_GET_SIZE(s1);
+        if (length != PyBytes_GET_SIZE(s2))
+            return (equals == Py_NE);
+        ps1 = PyBytes_AS_STRING(s1);
+        ps2 = PyBytes_AS_STRING(s2);
+        if (ps1[0] != ps2[0]) {
+            return (equals == Py_NE);
+        } else if (length == 1) {
+            return (equals == Py_EQ);
+        } else {
+            int result;
+#if CYTHON_USE_UNICODE_INTERNALS
+            Py_hash_t hash1, hash2;
+            hash1 = ((PyBytesObject*)s1)->ob_shash;
+            hash2 = ((PyBytesObject*)s2)->ob_shash;
+            if (hash1 != hash2 && hash1 != -1 && hash2 != -1) {
+                return (equals == Py_NE);
+            }
+#endif
+            result = memcmp(ps1, ps2, (size_t)length);
+            return (equals == Py_EQ) ? (result == 0) : (result != 0);
+        }
+    } else if ((s1 == Py_None) & PyBytes_CheckExact(s2)) {
+        return (equals == Py_NE);
+    } else if ((s2 == Py_None) & PyBytes_CheckExact(s1)) {
+        return (equals == Py_NE);
+    } else {
+        int result;
+        PyObject* py_result = PyObject_RichCompare(s1, s2, equals);
+        if (!py_result)
+            return -1;
+        result = __Pyx_PyObject_IsTrue(py_result);
+        Py_DECREF(py_result);
+        return result;
+    }
+#endif
+}
+
+/* UnicodeEquals */
+  static CYTHON_INLINE int __Pyx_PyUnicode_Equals(PyObject* s1, PyObject* s2, int equals) {
+#if CYTHON_COMPILING_IN_PYPY
+    return PyObject_RichCompareBool(s1, s2, equals);
+#else
+#if PY_MAJOR_VERSION < 3
+    PyObject* owned_ref = NULL;
+#endif
+    int s1_is_unicode, s2_is_unicode;
+    if (s1 == s2) {
+        goto return_eq;
+    }
+    s1_is_unicode = PyUnicode_CheckExact(s1);
+    s2_is_unicode = PyUnicode_CheckExact(s2);
+#if PY_MAJOR_VERSION < 3
+    if ((s1_is_unicode & (!s2_is_unicode)) && PyString_CheckExact(s2)) {
+        owned_ref = PyUnicode_FromObject(s2);
+        if (unlikely(!owned_ref))
+            return -1;
+        s2 = owned_ref;
+        s2_is_unicode = 1;
+    } else if ((s2_is_unicode & (!s1_is_unicode)) && PyString_CheckExact(s1)) {
+        owned_ref = PyUnicode_FromObject(s1);
+        if (unlikely(!owned_ref))
+            return -1;
+        s1 = owned_ref;
+        s1_is_unicode = 1;
+    } else if (((!s2_is_unicode) & (!s1_is_unicode))) {
+        return __Pyx_PyBytes_Equals(s1, s2, equals);
+    }
+#endif
+    if (s1_is_unicode & s2_is_unicode) {
+        Py_ssize_t length;
+        int kind;
+        void *data1, *data2;
+        if (unlikely(__Pyx_PyUnicode_READY(s1) < 0) || unlikely(__Pyx_PyUnicode_READY(s2) < 0))
+            return -1;
+        length = __Pyx_PyUnicode_GET_LENGTH(s1);
+        if (length != __Pyx_PyUnicode_GET_LENGTH(s2)) {
+            goto return_ne;
+        }
+#if CYTHON_USE_UNICODE_INTERNALS
+        {
+            Py_hash_t hash1, hash2;
+        #if CYTHON_PEP393_ENABLED
+            hash1 = ((PyASCIIObject*)s1)->hash;
+            hash2 = ((PyASCIIObject*)s2)->hash;
+        #else
+            hash1 = ((PyUnicodeObject*)s1)->hash;
+            hash2 = ((PyUnicodeObject*)s2)->hash;
+        #endif
+            if (hash1 != hash2 && hash1 != -1 && hash2 != -1) {
+                goto return_ne;
+            }
+        }
+#endif
+        kind = __Pyx_PyUnicode_KIND(s1);
+        if (kind != __Pyx_PyUnicode_KIND(s2)) {
+            goto return_ne;
+        }
+        data1 = __Pyx_PyUnicode_DATA(s1);
+        data2 = __Pyx_PyUnicode_DATA(s2);
+        if (__Pyx_PyUnicode_READ(kind, data1, 0) != __Pyx_PyUnicode_READ(kind, data2, 0)) {
+            goto return_ne;
+        } else if (length == 1) {
+            goto return_eq;
+        } else {
+            int result = memcmp(data1, data2, (size_t)(length * kind));
+            #if PY_MAJOR_VERSION < 3
+            Py_XDECREF(owned_ref);
+            #endif
+            return (equals == Py_EQ) ? (result == 0) : (result != 0);
+        }
+    } else if ((s1 == Py_None) & s2_is_unicode) {
+        goto return_ne;
+    } else if ((s2 == Py_None) & s1_is_unicode) {
+        goto return_ne;
+    } else {
+        int result;
+        PyObject* py_result = PyObject_RichCompare(s1, s2, equals);
+        #if PY_MAJOR_VERSION < 3
+        Py_XDECREF(owned_ref);
+        #endif
+        if (!py_result)
+            return -1;
+        result = __Pyx_PyObject_IsTrue(py_result);
+        Py_DECREF(py_result);
+        return result;
+    }
+return_eq:
+    #if PY_MAJOR_VERSION < 3
+    Py_XDECREF(owned_ref);
+    #endif
+    return (equals == Py_EQ);
+return_ne:
+    #if PY_MAJOR_VERSION < 3
+    Py_XDECREF(owned_ref);
+    #endif
+    return (equals == Py_NE);
+#endif
+}
+
+/* PyErrFetchRestore */
+  #if CYTHON_FAST_THREAD_STATE
+static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
+    PyObject *tmp_type, *tmp_value, *tmp_tb;
+    tmp_type = tstate->curexc_type;
+    tmp_value = tstate->curexc_value;
+    tmp_tb = tstate->curexc_traceback;
+    tstate->curexc_type = type;
+    tstate->curexc_value = value;
+    tstate->curexc_traceback = tb;
+    Py_XDECREF(tmp_type);
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(tmp_tb);
+}
+static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
+    *type = tstate->curexc_type;
+    *value = tstate->curexc_value;
+    *tb = tstate->curexc_traceback;
+    tstate->curexc_type = 0;
+    tstate->curexc_value = 0;
+    tstate->curexc_traceback = 0;
+}
+#endif
+
+/* RaiseException */
+  #if PY_MAJOR_VERSION < 3
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb,
+                        CYTHON_UNUSED PyObject *cause) {
+    __Pyx_PyThreadState_declare
+    Py_XINCREF(type);
+    if (!value || value == Py_None)
+        value = NULL;
+    else
+        Py_INCREF(value);
+    if (!tb || tb == Py_None)
+        tb = NULL;
+    else {
+        Py_INCREF(tb);
+        if (!PyTraceBack_Check(tb)) {
+            PyErr_SetString(PyExc_TypeError,
+                "raise: arg 3 must be a traceback or None");
+            goto raise_error;
+        }
+    }
+    if (PyType_Check(type)) {
+#if CYTHON_COMPILING_IN_PYPY
+        if (!value) {
+            Py_INCREF(Py_None);
+            value = Py_None;
+        }
+#endif
+        PyErr_NormalizeException(&type, &value, &tb);
+    } else {
+        if (value) {
+            PyErr_SetString(PyExc_TypeError,
+                "instance exception may not have a separate value");
+            goto raise_error;
+        }
+        value = type;
+        type = (PyObject*) Py_TYPE(type);
+        Py_INCREF(type);
+        if (!PyType_IsSubtype((PyTypeObject *)type, (PyTypeObject *)PyExc_BaseException)) {
+            PyErr_SetString(PyExc_TypeError,
+                "raise: exception class must be a subclass of BaseException");
+            goto raise_error;
+        }
+    }
+    __Pyx_PyThreadState_assign
+    __Pyx_ErrRestore(type, value, tb);
+    return;
+raise_error:
+    Py_XDECREF(value);
+    Py_XDECREF(type);
+    Py_XDECREF(tb);
+    return;
+}
+#else
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause) {
+    PyObject* owned_instance = NULL;
+    if (tb == Py_None) {
+        tb = 0;
+    } else if (tb && !PyTraceBack_Check(tb)) {
+        PyErr_SetString(PyExc_TypeError,
+            "raise: arg 3 must be a traceback or None");
+        goto bad;
+    }
+    if (value == Py_None)
+        value = 0;
+    if (PyExceptionInstance_Check(type)) {
+        if (value) {
+            PyErr_SetString(PyExc_TypeError,
+                "instance exception may not have a separate value");
+            goto bad;
+        }
+        value = type;
+        type = (PyObject*) Py_TYPE(value);
+    } else if (PyExceptionClass_Check(type)) {
+        PyObject *instance_class = NULL;
+        if (value && PyExceptionInstance_Check(value)) {
+            instance_class = (PyObject*) Py_TYPE(value);
+            if (instance_class != type) {
+                int is_subclass = PyObject_IsSubclass(instance_class, type);
+                if (!is_subclass) {
+                    instance_class = NULL;
+                } else if (unlikely(is_subclass == -1)) {
+                    goto bad;
+                } else {
+                    type = instance_class;
+                }
+            }
+        }
+        if (!instance_class) {
+            PyObject *args;
+            if (!value)
+                args = PyTuple_New(0);
+            else if (PyTuple_Check(value)) {
+                Py_INCREF(value);
+                args = value;
+            } else
+                args = PyTuple_Pack(1, value);
+            if (!args)
+                goto bad;
+            owned_instance = PyObject_Call(type, args, NULL);
+            Py_DECREF(args);
+            if (!owned_instance)
+                goto bad;
+            value = owned_instance;
+            if (!PyExceptionInstance_Check(value)) {
+                PyErr_Format(PyExc_TypeError,
+                             "calling %R should have returned an instance of "
+                             "BaseException, not %R",
+                             type, Py_TYPE(value));
+                goto bad;
+            }
+        }
+    } else {
+        PyErr_SetString(PyExc_TypeError,
+            "raise: exception class must be a subclass of BaseException");
+        goto bad;
+    }
+    if (cause) {
+        PyObject *fixed_cause;
+        if (cause == Py_None) {
+            fixed_cause = NULL;
+        } else if (PyExceptionClass_Check(cause)) {
+            fixed_cause = PyObject_CallObject(cause, NULL);
+            if (fixed_cause == NULL)
+                goto bad;
+        } else if (PyExceptionInstance_Check(cause)) {
+            fixed_cause = cause;
+            Py_INCREF(fixed_cause);
+        } else {
+            PyErr_SetString(PyExc_TypeError,
+                            "exception causes must derive from "
+                            "BaseException");
+            goto bad;
+        }
+        PyException_SetCause(value, fixed_cause);
+    }
+    PyErr_SetObject(type, value);
+    if (tb) {
+#if CYTHON_COMPILING_IN_PYPY
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
+#else
+        PyThreadState *tstate = __Pyx_PyThreadState_Current;
+        PyObject* tmp_tb = tstate->curexc_traceback;
+        if (tb != tmp_tb) {
+            Py_INCREF(tb);
+            tstate->curexc_traceback = tb;
+            Py_XDECREF(tmp_tb);
+        }
+#endif
+    }
+bad:
+    Py_XDECREF(owned_instance);
+    return;
+}
+#endif
+
 /* GetItemInt */
   static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j) {
     PyObject *r;
     if (!j) return NULL;
     r = PyObject_GetItem(o, j);
     Py_DECREF(j);
     return r;
@@ -20868,262 +21459,14 @@
             PyGILState_Release(_gilstate);
         }
     } else {
         memslice->memview = NULL;
     }
 }
 
-/* PyErrFetchRestore */
-  #if CYTHON_FAST_THREAD_STATE
-static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
-    PyObject *tmp_type, *tmp_value, *tmp_tb;
-    tmp_type = tstate->curexc_type;
-    tmp_value = tstate->curexc_value;
-    tmp_tb = tstate->curexc_traceback;
-    tstate->curexc_type = type;
-    tstate->curexc_value = value;
-    tstate->curexc_traceback = tb;
-    Py_XDECREF(tmp_type);
-    Py_XDECREF(tmp_value);
-    Py_XDECREF(tmp_tb);
-}
-static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
-    *type = tstate->curexc_type;
-    *value = tstate->curexc_value;
-    *tb = tstate->curexc_traceback;
-    tstate->curexc_type = 0;
-    tstate->curexc_value = 0;
-    tstate->curexc_traceback = 0;
-}
-#endif
-
-/* PyFunctionFastCall */
-  #if CYTHON_FAST_PYCALL
-static PyObject* __Pyx_PyFunction_FastCallNoKw(PyCodeObject *co, PyObject **args, Py_ssize_t na,
-                                               PyObject *globals) {
-    PyFrameObject *f;
-    PyThreadState *tstate = __Pyx_PyThreadState_Current;
-    PyObject **fastlocals;
-    Py_ssize_t i;
-    PyObject *result;
-    assert(globals != NULL);
-    /* XXX Perhaps we should create a specialized
-       PyFrame_New() that doesn't take locals, but does
-       take builtins without sanity checking them.
-       */
-    assert(tstate != NULL);
-    f = PyFrame_New(tstate, co, globals, NULL);
-    if (f == NULL) {
-        return NULL;
-    }
-    fastlocals = __Pyx_PyFrame_GetLocalsplus(f);
-    for (i = 0; i < na; i++) {
-        Py_INCREF(*args);
-        fastlocals[i] = *args++;
-    }
-    result = PyEval_EvalFrameEx(f,0);
-    ++tstate->recursion_depth;
-    Py_DECREF(f);
-    --tstate->recursion_depth;
-    return result;
-}
-#if 1 || PY_VERSION_HEX < 0x030600B1
-static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs) {
-    PyCodeObject *co = (PyCodeObject *)PyFunction_GET_CODE(func);
-    PyObject *globals = PyFunction_GET_GLOBALS(func);
-    PyObject *argdefs = PyFunction_GET_DEFAULTS(func);
-    PyObject *closure;
-#if PY_MAJOR_VERSION >= 3
-    PyObject *kwdefs;
-#endif
-    PyObject *kwtuple, **k;
-    PyObject **d;
-    Py_ssize_t nd;
-    Py_ssize_t nk;
-    PyObject *result;
-    assert(kwargs == NULL || PyDict_Check(kwargs));
-    nk = kwargs ? PyDict_Size(kwargs) : 0;
-    if (Py_EnterRecursiveCall((char*)" while calling a Python object")) {
-        return NULL;
-    }
-    if (
-#if PY_MAJOR_VERSION >= 3
-            co->co_kwonlyargcount == 0 &&
-#endif
-            likely(kwargs == NULL || nk == 0) &&
-            co->co_flags == (CO_OPTIMIZED | CO_NEWLOCALS | CO_NOFREE)) {
-        if (argdefs == NULL && co->co_argcount == nargs) {
-            result = __Pyx_PyFunction_FastCallNoKw(co, args, nargs, globals);
-            goto done;
-        }
-        else if (nargs == 0 && argdefs != NULL
-                 && co->co_argcount == Py_SIZE(argdefs)) {
-            /* function called with no arguments, but all parameters have
-               a default value: use default values as arguments .*/
-            args = &PyTuple_GET_ITEM(argdefs, 0);
-            result =__Pyx_PyFunction_FastCallNoKw(co, args, Py_SIZE(argdefs), globals);
-            goto done;
-        }
-    }
-    if (kwargs != NULL) {
-        Py_ssize_t pos, i;
-        kwtuple = PyTuple_New(2 * nk);
-        if (kwtuple == NULL) {
-            result = NULL;
-            goto done;
-        }
-        k = &PyTuple_GET_ITEM(kwtuple, 0);
-        pos = i = 0;
-        while (PyDict_Next(kwargs, &pos, &k[i], &k[i+1])) {
-            Py_INCREF(k[i]);
-            Py_INCREF(k[i+1]);
-            i += 2;
-        }
-        nk = i / 2;
-    }
-    else {
-        kwtuple = NULL;
-        k = NULL;
-    }
-    closure = PyFunction_GET_CLOSURE(func);
-#if PY_MAJOR_VERSION >= 3
-    kwdefs = PyFunction_GET_KW_DEFAULTS(func);
-#endif
-    if (argdefs != NULL) {
-        d = &PyTuple_GET_ITEM(argdefs, 0);
-        nd = Py_SIZE(argdefs);
-    }
-    else {
-        d = NULL;
-        nd = 0;
-    }
-#if PY_MAJOR_VERSION >= 3
-    result = PyEval_EvalCodeEx((PyObject*)co, globals, (PyObject *)NULL,
-                               args, (int)nargs,
-                               k, (int)nk,
-                               d, (int)nd, kwdefs, closure);
-#else
-    result = PyEval_EvalCodeEx(co, globals, (PyObject *)NULL,
-                               args, (int)nargs,
-                               k, (int)nk,
-                               d, (int)nd, closure);
-#endif
-    Py_XDECREF(kwtuple);
-done:
-    Py_LeaveRecursiveCall();
-    return result;
-}
-#endif
-#endif
-
-/* PyObjectCallMethO */
-  #if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg) {
-    PyObject *self, *result;
-    PyCFunction cfunc;
-    cfunc = PyCFunction_GET_FUNCTION(func);
-    self = PyCFunction_GET_SELF(func);
-    if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
-        return NULL;
-    result = cfunc(self, arg);
-    Py_LeaveRecursiveCall();
-    if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
-        PyErr_SetString(
-            PyExc_SystemError,
-            "NULL result without error in PyObject_Call");
-    }
-    return result;
-}
-#endif
-
-/* PyObjectCallNoArg */
-  #if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
-#if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(func)) {
-        return __Pyx_PyFunction_FastCall(func, NULL, 0);
-    }
-#endif
-#ifdef __Pyx_CyFunction_USED
-    if (likely(PyCFunction_Check(func) || __Pyx_CyFunction_Check(func)))
-#else
-    if (likely(PyCFunction_Check(func)))
-#endif
-    {
-        if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
-            return __Pyx_PyObject_CallMethO(func, NULL);
-        }
-    }
-    return __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL);
-}
-#endif
-
-/* PyCFunctionFastCall */
-  #if CYTHON_FAST_PYCCALL
-static CYTHON_INLINE PyObject * __Pyx_PyCFunction_FastCall(PyObject *func_obj, PyObject **args, Py_ssize_t nargs) {
-    PyCFunctionObject *func = (PyCFunctionObject*)func_obj;
-    PyCFunction meth = PyCFunction_GET_FUNCTION(func);
-    PyObject *self = PyCFunction_GET_SELF(func);
-    int flags = PyCFunction_GET_FLAGS(func);
-    assert(PyCFunction_Check(func));
-    assert(METH_FASTCALL == (flags & ~(METH_CLASS | METH_STATIC | METH_COEXIST | METH_KEYWORDS | METH_STACKLESS)));
-    assert(nargs >= 0);
-    assert(nargs == 0 || args != NULL);
-    /* _PyCFunction_FastCallDict() must not be called with an exception set,
-       because it may clear it (directly or indirectly) and so the
-       caller loses its exception */
-    assert(!PyErr_Occurred());
-    if ((PY_VERSION_HEX < 0x030700A0) || unlikely(flags & METH_KEYWORDS)) {
-        return (*((__Pyx_PyCFunctionFastWithKeywords)(void*)meth)) (self, args, nargs, NULL);
-    } else {
-        return (*((__Pyx_PyCFunctionFast)(void*)meth)) (self, args, nargs);
-    }
-}
-#endif
-
-/* PyObjectCallOneArg */
-  #if CYTHON_COMPILING_IN_CPYTHON
-static PyObject* __Pyx__PyObject_CallOneArg(PyObject *func, PyObject *arg) {
-    PyObject *result;
-    PyObject *args = PyTuple_New(1);
-    if (unlikely(!args)) return NULL;
-    Py_INCREF(arg);
-    PyTuple_SET_ITEM(args, 0, arg);
-    result = __Pyx_PyObject_Call(func, args, NULL);
-    Py_DECREF(args);
-    return result;
-}
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg) {
-#if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(func)) {
-        return __Pyx_PyFunction_FastCall(func, &arg, 1);
-    }
-#endif
-    if (likely(PyCFunction_Check(func))) {
-        if (likely(PyCFunction_GET_FLAGS(func) & METH_O)) {
-            return __Pyx_PyObject_CallMethO(func, arg);
-#if CYTHON_FAST_PYCCALL
-        } else if (__Pyx_PyFastCFunction_Check(func)) {
-            return __Pyx_PyCFunction_FastCall(func, &arg, 1);
-#endif
-        }
-    }
-    return __Pyx__PyObject_CallOneArg(func, arg);
-}
-#else
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg) {
-    PyObject *result;
-    PyObject *args = PyTuple_Pack(1, arg);
-    if (unlikely(!args)) return NULL;
-    result = __Pyx_PyObject_Call(func, args, NULL);
-    Py_DECREF(args);
-    return result;
-}
-#endif
-
 /* GetTopmostException */
   #if CYTHON_USE_EXC_INFO_STACK
 static _PyErr_StackItem *
 __Pyx_PyErr_GetTopmostException(PyThreadState *tstate)
 {
     _PyErr_StackItem *exc_info = tstate->exc_info;
     while ((exc_info->exc_type == NULL || exc_info->exc_type == Py_None) &&
@@ -21313,173 +21656,14 @@
     }
 #ifdef WITH_THREAD
     if (nogil)
         PyGILState_Release(state);
 #endif
 }
 
-/* RaiseException */
-  #if PY_MAJOR_VERSION < 3
-static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb,
-                        CYTHON_UNUSED PyObject *cause) {
-    __Pyx_PyThreadState_declare
-    Py_XINCREF(type);
-    if (!value || value == Py_None)
-        value = NULL;
-    else
-        Py_INCREF(value);
-    if (!tb || tb == Py_None)
-        tb = NULL;
-    else {
-        Py_INCREF(tb);
-        if (!PyTraceBack_Check(tb)) {
-            PyErr_SetString(PyExc_TypeError,
-                "raise: arg 3 must be a traceback or None");
-            goto raise_error;
-        }
-    }
-    if (PyType_Check(type)) {
-#if CYTHON_COMPILING_IN_PYPY
-        if (!value) {
-            Py_INCREF(Py_None);
-            value = Py_None;
-        }
-#endif
-        PyErr_NormalizeException(&type, &value, &tb);
-    } else {
-        if (value) {
-            PyErr_SetString(PyExc_TypeError,
-                "instance exception may not have a separate value");
-            goto raise_error;
-        }
-        value = type;
-        type = (PyObject*) Py_TYPE(type);
-        Py_INCREF(type);
-        if (!PyType_IsSubtype((PyTypeObject *)type, (PyTypeObject *)PyExc_BaseException)) {
-            PyErr_SetString(PyExc_TypeError,
-                "raise: exception class must be a subclass of BaseException");
-            goto raise_error;
-        }
-    }
-    __Pyx_PyThreadState_assign
-    __Pyx_ErrRestore(type, value, tb);
-    return;
-raise_error:
-    Py_XDECREF(value);
-    Py_XDECREF(type);
-    Py_XDECREF(tb);
-    return;
-}
-#else
-static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause) {
-    PyObject* owned_instance = NULL;
-    if (tb == Py_None) {
-        tb = 0;
-    } else if (tb && !PyTraceBack_Check(tb)) {
-        PyErr_SetString(PyExc_TypeError,
-            "raise: arg 3 must be a traceback or None");
-        goto bad;
-    }
-    if (value == Py_None)
-        value = 0;
-    if (PyExceptionInstance_Check(type)) {
-        if (value) {
-            PyErr_SetString(PyExc_TypeError,
-                "instance exception may not have a separate value");
-            goto bad;
-        }
-        value = type;
-        type = (PyObject*) Py_TYPE(value);
-    } else if (PyExceptionClass_Check(type)) {
-        PyObject *instance_class = NULL;
-        if (value && PyExceptionInstance_Check(value)) {
-            instance_class = (PyObject*) Py_TYPE(value);
-            if (instance_class != type) {
-                int is_subclass = PyObject_IsSubclass(instance_class, type);
-                if (!is_subclass) {
-                    instance_class = NULL;
-                } else if (unlikely(is_subclass == -1)) {
-                    goto bad;
-                } else {
-                    type = instance_class;
-                }
-            }
-        }
-        if (!instance_class) {
-            PyObject *args;
-            if (!value)
-                args = PyTuple_New(0);
-            else if (PyTuple_Check(value)) {
-                Py_INCREF(value);
-                args = value;
-            } else
-                args = PyTuple_Pack(1, value);
-            if (!args)
-                goto bad;
-            owned_instance = PyObject_Call(type, args, NULL);
-            Py_DECREF(args);
-            if (!owned_instance)
-                goto bad;
-            value = owned_instance;
-            if (!PyExceptionInstance_Check(value)) {
-                PyErr_Format(PyExc_TypeError,
-                             "calling %R should have returned an instance of "
-                             "BaseException, not %R",
-                             type, Py_TYPE(value));
-                goto bad;
-            }
-        }
-    } else {
-        PyErr_SetString(PyExc_TypeError,
-            "raise: exception class must be a subclass of BaseException");
-        goto bad;
-    }
-    if (cause) {
-        PyObject *fixed_cause;
-        if (cause == Py_None) {
-            fixed_cause = NULL;
-        } else if (PyExceptionClass_Check(cause)) {
-            fixed_cause = PyObject_CallObject(cause, NULL);
-            if (fixed_cause == NULL)
-                goto bad;
-        } else if (PyExceptionInstance_Check(cause)) {
-            fixed_cause = cause;
-            Py_INCREF(fixed_cause);
-        } else {
-            PyErr_SetString(PyExc_TypeError,
-                            "exception causes must derive from "
-                            "BaseException");
-            goto bad;
-        }
-        PyException_SetCause(value, fixed_cause);
-    }
-    PyErr_SetObject(type, value);
-    if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
-        PyThreadState *tstate = __Pyx_PyThreadState_Current;
-        PyObject* tmp_tb = tstate->curexc_traceback;
-        if (tb != tmp_tb) {
-            Py_INCREF(tb);
-            tstate->curexc_traceback = tb;
-            Py_XDECREF(tmp_tb);
-        }
-#endif
-    }
-bad:
-    Py_XDECREF(owned_instance);
-    return;
-}
-#endif
-
 /* PyObjectCall2Args */
   static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2) {
     PyObject *args, *result = NULL;
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(function)) {
         PyObject *args[2] = {arg1, arg2};
         return __Pyx_PyFunction_FastCall(function, args, 2);
@@ -21501,163 +21685,14 @@
     result = __Pyx_PyObject_Call(function, args, NULL);
     Py_DECREF(args);
     Py_DECREF(function);
 done:
     return result;
 }
 
-/* BytesEquals */
-  static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals) {
-#if CYTHON_COMPILING_IN_PYPY
-    return PyObject_RichCompareBool(s1, s2, equals);
-#else
-    if (s1 == s2) {
-        return (equals == Py_EQ);
-    } else if (PyBytes_CheckExact(s1) & PyBytes_CheckExact(s2)) {
-        const char *ps1, *ps2;
-        Py_ssize_t length = PyBytes_GET_SIZE(s1);
-        if (length != PyBytes_GET_SIZE(s2))
-            return (equals == Py_NE);
-        ps1 = PyBytes_AS_STRING(s1);
-        ps2 = PyBytes_AS_STRING(s2);
-        if (ps1[0] != ps2[0]) {
-            return (equals == Py_NE);
-        } else if (length == 1) {
-            return (equals == Py_EQ);
-        } else {
-            int result;
-#if CYTHON_USE_UNICODE_INTERNALS
-            Py_hash_t hash1, hash2;
-            hash1 = ((PyBytesObject*)s1)->ob_shash;
-            hash2 = ((PyBytesObject*)s2)->ob_shash;
-            if (hash1 != hash2 && hash1 != -1 && hash2 != -1) {
-                return (equals == Py_NE);
-            }
-#endif
-            result = memcmp(ps1, ps2, (size_t)length);
-            return (equals == Py_EQ) ? (result == 0) : (result != 0);
-        }
-    } else if ((s1 == Py_None) & PyBytes_CheckExact(s2)) {
-        return (equals == Py_NE);
-    } else if ((s2 == Py_None) & PyBytes_CheckExact(s1)) {
-        return (equals == Py_NE);
-    } else {
-        int result;
-        PyObject* py_result = PyObject_RichCompare(s1, s2, equals);
-        if (!py_result)
-            return -1;
-        result = __Pyx_PyObject_IsTrue(py_result);
-        Py_DECREF(py_result);
-        return result;
-    }
-#endif
-}
-
-/* UnicodeEquals */
-  static CYTHON_INLINE int __Pyx_PyUnicode_Equals(PyObject* s1, PyObject* s2, int equals) {
-#if CYTHON_COMPILING_IN_PYPY
-    return PyObject_RichCompareBool(s1, s2, equals);
-#else
-#if PY_MAJOR_VERSION < 3
-    PyObject* owned_ref = NULL;
-#endif
-    int s1_is_unicode, s2_is_unicode;
-    if (s1 == s2) {
-        goto return_eq;
-    }
-    s1_is_unicode = PyUnicode_CheckExact(s1);
-    s2_is_unicode = PyUnicode_CheckExact(s2);
-#if PY_MAJOR_VERSION < 3
-    if ((s1_is_unicode & (!s2_is_unicode)) && PyString_CheckExact(s2)) {
-        owned_ref = PyUnicode_FromObject(s2);
-        if (unlikely(!owned_ref))
-            return -1;
-        s2 = owned_ref;
-        s2_is_unicode = 1;
-    } else if ((s2_is_unicode & (!s1_is_unicode)) && PyString_CheckExact(s1)) {
-        owned_ref = PyUnicode_FromObject(s1);
-        if (unlikely(!owned_ref))
-            return -1;
-        s1 = owned_ref;
-        s1_is_unicode = 1;
-    } else if (((!s2_is_unicode) & (!s1_is_unicode))) {
-        return __Pyx_PyBytes_Equals(s1, s2, equals);
-    }
-#endif
-    if (s1_is_unicode & s2_is_unicode) {
-        Py_ssize_t length;
-        int kind;
-        void *data1, *data2;
-        if (unlikely(__Pyx_PyUnicode_READY(s1) < 0) || unlikely(__Pyx_PyUnicode_READY(s2) < 0))
-            return -1;
-        length = __Pyx_PyUnicode_GET_LENGTH(s1);
-        if (length != __Pyx_PyUnicode_GET_LENGTH(s2)) {
-            goto return_ne;
-        }
-#if CYTHON_USE_UNICODE_INTERNALS
-        {
-            Py_hash_t hash1, hash2;
-        #if CYTHON_PEP393_ENABLED
-            hash1 = ((PyASCIIObject*)s1)->hash;
-            hash2 = ((PyASCIIObject*)s2)->hash;
-        #else
-            hash1 = ((PyUnicodeObject*)s1)->hash;
-            hash2 = ((PyUnicodeObject*)s2)->hash;
-        #endif
-            if (hash1 != hash2 && hash1 != -1 && hash2 != -1) {
-                goto return_ne;
-            }
-        }
-#endif
-        kind = __Pyx_PyUnicode_KIND(s1);
-        if (kind != __Pyx_PyUnicode_KIND(s2)) {
-            goto return_ne;
-        }
-        data1 = __Pyx_PyUnicode_DATA(s1);
-        data2 = __Pyx_PyUnicode_DATA(s2);
-        if (__Pyx_PyUnicode_READ(kind, data1, 0) != __Pyx_PyUnicode_READ(kind, data2, 0)) {
-            goto return_ne;
-        } else if (length == 1) {
-            goto return_eq;
-        } else {
-            int result = memcmp(data1, data2, (size_t)(length * kind));
-            #if PY_MAJOR_VERSION < 3
-            Py_XDECREF(owned_ref);
-            #endif
-            return (equals == Py_EQ) ? (result == 0) : (result != 0);
-        }
-    } else if ((s1 == Py_None) & s2_is_unicode) {
-        goto return_ne;
-    } else if ((s2 == Py_None) & s1_is_unicode) {
-        goto return_ne;
-    } else {
-        int result;
-        PyObject* py_result = PyObject_RichCompare(s1, s2, equals);
-        #if PY_MAJOR_VERSION < 3
-        Py_XDECREF(owned_ref);
-        #endif
-        if (!py_result)
-            return -1;
-        result = __Pyx_PyObject_IsTrue(py_result);
-        Py_DECREF(py_result);
-        return result;
-    }
-return_eq:
-    #if PY_MAJOR_VERSION < 3
-    Py_XDECREF(owned_ref);
-    #endif
-    return (equals == Py_EQ);
-return_ne:
-    #if PY_MAJOR_VERSION < 3
-    Py_XDECREF(owned_ref);
-    #endif
-    return (equals == Py_NE);
-#endif
-}
-
 /* DivInt[Py_ssize_t] */
   static CYTHON_INLINE Py_ssize_t __Pyx_div_Py_ssize_t(Py_ssize_t a, Py_ssize_t b) {
     Py_ssize_t q = a / b;
     Py_ssize_t r = a - q*b;
     q -= ((r != 0) & ((r ^ b) < 0));
     return q;
 }
```

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/sa/simulated_annealing.pyx` & `dwave-samplers-1.1.0/dwave/samplers/sa/simulated_annealing.pyx`

 * *Files 26% similar despite different names*

```diff
@@ -22,33 +22,40 @@
 
 import numpy as np
 cimport numpy as np
 
 
 cdef extern from "cpu_sa.h":
     ctypedef bool (*callback)(void *function)
-
+    ctypedef enum Proposal:
+        Gibbs, Metropolis
+    ctypedef enum VariableOrder:
+        Sequential, Random
     int general_simulated_annealing(
-            char* samples,
+            np.int8_t* samples,
             double* energies,
             const int num_samples,
             const vector[double] & h,
             const vector[int] & coupler_starts,
             const vector[int] & coupler_ends,
             const vector[double] & coupler_weights,
             const int sweeps_per_beta,
             const vector[double] & beta_schedule,
             const unsigned long long seed,
+            const VariableOrder varorder,
+            const Proposal proposal_acceptance_criteria,
             callback interrupt_callback,
             void *interrupt_function) nogil
 
 
 def simulated_annealing(num_samples, h, coupler_starts, coupler_ends,
                         coupler_weights, sweeps_per_beta, beta_schedule, seed,
-                        np.ndarray[char, ndim=2, mode="c"] states_numpy,
+                        np.ndarray[np.int8_t, ndim=2, mode="c"] states_numpy,
+                        randomize_order=False,
+                        proposal_acceptance_criteria='Metropolis',
                         interrupt_function=None):
     """Wraps `general_simulated_annealing` from `cpu_sa.cpp`. Accepts
     an Ising problem defined on a general graph and returns samples
     using simulated annealing.
 
     Parameters
     ----------
@@ -82,23 +89,44 @@
 
     seed : 64 bit int > 0
         The seed to use for the PRNG. Must be a positive integer
         greater than 0. If the same seed is used and the rest of the
         parameters are the same, the returned samples will be
         identical.
 
-    states_numpy : np.ndarray[char, ndim=2, mode="c"], values in (-1, 1)
+    states_numpy : np.ndarray[int8_t, ndim=2, mode="c"], values in (-1, 1)
         The initial seeded states of the simulated annealing runs. Should be of
         a contiguous numpy.ndarray of shape (num_samples, num_variables).
 
     interrupt_function: function
         Should accept no arguments and return a bool. The function is
         called between samples and if it returns True, simulated annealing
         will return early with the samples it already has.
 
+    randomize_order: bool
+        When True, each spin update selects a variable uniformly at random.
+        When False, updates proceed sequentially through the labeled variables 
+        on each sweep so that all variables are updated once per sweep.
+        The random method is ergodic and obeys detailed balance at all temperatures.
+        Symmetries of the Boltzmann distribution(s) are not broken by the
+        update order.
+        The sequential method:
+            - when combined with ``proposal_acceptance_criteria=Metropolis`` can be
+            non-ergodic in the limits of zero or infinite temperature,
+            and converge slowly near these limits.
+            - can introduce a dynamical bias as a function of variable
+            labeling convention.
+            - has faster per spin update than the random method.
+
+    proposal_acceptance_criteria: str
+        When `Gibbs`, each spin flip proposal is accepted according to the
+        Gibbs criteria.
+        When `Metropolis`, each spin flip proposal is accepted according to the
+        Metropolis-Hastings criteria.
+
     Returns
     -------
     samples : numpy.ndarray
         A 2D numpy array where each row is a sample.
 
     energies: np.ndarray
         The energies.
@@ -113,42 +141,56 @@
         return annealed_states, np.zeros(num_samples, dtype=np.double)
 
     # allocate ndarray for energies
     energies_numpy = np.empty(num_samples, dtype=np.float64)
     cdef double[:] energies = energies_numpy
 
     # explicitly convert all Python types to C while we have the GIL
-    cdef char* _states = &states_numpy[0, 0]
+    cdef np.int8_t* _states = &states_numpy[0, 0]
     cdef double* _energies = &energies[0]
     cdef int _num_samples = num_samples
     cdef vector[double] _h = h
     cdef vector[int] _coupler_starts = coupler_starts
     cdef vector[int] _coupler_ends = coupler_ends
     cdef vector[double] _coupler_weights = coupler_weights
     cdef int _sweeps_per_beta = sweeps_per_beta
     cdef vector[double] _beta_schedule = beta_schedule
     cdef unsigned long long _seed = seed
-
+    cdef VariableOrder _varorder
+    if randomize_order:
+        _varorder = Random
+    else:
+        _varorder = Sequential
+    cdef Proposal _proposal_acceptance_criteria
+    if proposal_acceptance_criteria.lower() == 'gibbs':
+        _proposal_acceptance_criteria = Gibbs
+    elif proposal_acceptance_criteria.lower() == 'metropolis':
+        _proposal_acceptance_criteria = Metropolis
+    else:
+        raise ValueError(f'Unknown proposal_acceptance_criteria: {proposal_acceptance_criteria}')
     cdef void* _interrupt_function
     if interrupt_function is None:
         _interrupt_function = NULL
     else:
         _interrupt_function = <void *>interrupt_function
 
+
     with nogil:
         num = general_simulated_annealing(_states,
                                           _energies,
                                           _num_samples,
                                           _h,
                                           _coupler_starts,
                                           _coupler_ends,
                                           _coupler_weights,
                                           _sweeps_per_beta,
                                           _beta_schedule,
                                           _seed,
+                                          _varorder,
+                                          _proposal_acceptance_criteria,
                                           interrupt_callback,
                                           _interrupt_function)
 
     # discard the noise if we were interrupted
     return states_numpy[:num], energies_numpy[:num]
```

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/sa/src/cpu_sa.cpp` & `dwave-samplers-1.1.0/dwave/samplers/sa/src/cpu_sa.cpp`

 * *Files 12% similar despite different names*

```diff
@@ -10,19 +10,21 @@
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 //
 // ===========================================================================
 
+#include <cstdint>
 #include <math.h>
 #include <vector>
 #include <stdexcept>
 #include "cpu_sa.h"
 
+
 // xorshift128+ as defined https://en.wikipedia.org/wiki/Xorshift#xorshift.2B
 #define FASTRAND(rand) do {                       \
     uint64_t x = rng_state[0];                    \
     uint64_t const y = rng_state[1];              \
     rng_state[0] = y;                             \
     x ^= x << 23;                                 \
     rng_state[1] = x ^ y ^ (x >> 17) ^ (y >> 26); \
@@ -45,15 +47,15 @@
 //     neighbors[i][j] is the jth neighbor of variable i.
 // @param neighbour_couplings same as neighbors, but instead has the J value.
 //     neighbour_couplings[i][j] is the J value or weight on the coupling
 //     between variables i and neighbors[i][j]. 
 // @return delta energy
 double get_flip_energy(
     int var,
-    char *state,
+    std::int8_t *state,
     const vector<double>& h,
     const vector<int>& degrees,
     const vector<vector<int>>& neighbors,
     const vector<vector<double>>& neighbour_couplings
 ) {
     double energy = h[var];
     // iterate over the neighbors of variable `var`
@@ -66,15 +68,15 @@
     // coefficients of `var`.  we then multiply this by -2 * the state of `var`
     // because the energy delta is given by: (x_i_new - x_i_old) * sum(coefs),
     // and (x_i_new - x_i_old) = -2 * x_i_old
     return -2 * state[var] * energy;
 }
 
 // Performs a single run of simulated annealing with the given inputs.
-// @param state a signed char array where each char holds the state of a
+// @param state a int8 array where each int8 holds the state of a
 //        variable. Note that this will be used as the initial state of the
 //        run.
 // @param h vector of h or field value on each variable
 // @param degrees the degree of each variable
 // @param neighbors lists of the neighbors of each variable, such that 
 //        neighbors[i][j] is the jth neighbor of variable i. Note
 // @param neighbour_couplings same as neighbors, but instead has the J value.
@@ -82,16 +84,17 @@
 //        between variables i and neighbors[i][j]. 
 // @param sweeps_per_beta The number of sweeps to perform at each beta value.
 //        Total number of sweeps is `sweeps_per_beta` * length of
 //        `beta_schedule`.
 // @param beta_schedule A list of the beta values to run `sweeps_per_beta`
 //        sweeps at.
 // @return Nothing, but `state` now contains the result of the run.
+template <VariableOrder varorder, Proposal proposal_acceptance_criteria>
 void simulated_annealing_run(
-    char* state,
+    std::int8_t* state,
     const vector<double>& h,
     const vector<int>& degrees,
     const vector<vector<int>>& neighbors,
     const vector<vector<double>>& neighbour_couplings,
     const int sweeps_per_beta,
     const vector<double>& beta_schedule
 ) {
@@ -120,39 +123,55 @@
             // this threshold will allow us to skip the metropolis update for
             // variables that have zero chance of getting flipped.
             // our RNG generates 64 bit integers, so we have a resolution of
             // 1 / 2^64. since log(1 / 2^64) = -44.361, if the delta energy is
             // greater than 44.361 / beta, then we can safely skip computing
             // the probability.
             const double threshold = 44.36142 / beta;
-
-            for (int var = 0; var < num_vars; var++) {
+            for (int varI = 0; varI < num_vars; varI++) {
+                int var;
+                if constexpr (varorder == Random) {
+                    FASTRAND(rand);
+                    var = rand%num_vars;
+                } else {
+                    var = varI;
+                }
                 if (delta_energy[var] >= threshold) continue;
 
                 flip_spin = false;
 
-                if (delta_energy[var] <= 0.0) {
-                    // automatically accept any flip that results in a lower 
-                    // energy
-                    flip_spin = true;
+                if constexpr (proposal_acceptance_criteria == Metropolis) {
+                    // Metropolis-Hastings acceptance rule
+                    if (delta_energy[var] <= 0.0) {
+                        // automatically accept any flip that results in a lower
+                        // energy
+                        flip_spin = true;
+                    } else {
+                        // get a random number, storing it in rand
+                        FASTRAND(rand);
+                        // accept the flip if exp(-delta_energy*beta) > random(0, 1)
+                        if (exp(-delta_energy[var]*beta) * RANDMAX > rand) {
+                            flip_spin = true;
+                        }
+                    }
                 }
                 else {
-                    // get a random number, storing it in rand
-                    FASTRAND(rand); 
-                    // accept the flip if exp(-delta_energy*beta) > random(0, 1)
-                    if (exp(-delta_energy[var]*beta) * RANDMAX > rand) {
+                    // Gibbs update: Sample fairly from the two available states,
+                    // independent of the current value
+                    FASTRAND(rand);
+                    if (RANDMAX > rand * (1+exp(delta_energy[var]*beta))) {
                         flip_spin = true;
                     }
                 }
 
                 if (flip_spin) {
                     // since we have accepted the spin flip of variable `var`, 
                     // we need to adjust the delta energies of all the 
                     // neighboring variables
-                    const char multiplier = 4 * state[var];
+                    const std::int8_t multiplier = 4 * state[var];
                     // iterate over the neighbors of `var`
                     for (int n_i = 0; n_i < degrees[var]; n_i++) {
                         int neighbor = neighbors[var][n_i];
                         // adjust the delta energy by 
                         // 4 * `var` state * coupler weight * neighbor state
                         // the 4 is because the original contribution from 
                         // `var` to the neighbor's delta energy was
@@ -172,26 +191,26 @@
         }
     }
 
     free(delta_energy);
 }
 
 // Returns the energy of a given state and problem
-// @param state a char array containing the spin state to compute the energy of
+// @param state a int8 array containing the spin state to compute the energy of
 // @param h vector of h or field value on each variable
 // @param coupler_starts an int vector containing the variables of one side of
 //        each coupler in the problem
 // @param coupler_ends an int vector containing the variables of the other side 
 //        of each coupler in the problem
 // @param coupler_weights a double vector containing the weights of the 
 //        couplers in the same order as coupler_starts and coupler_ends
 // @return A double corresponding to the energy for `state` on the problem
 //        defined by h and the couplers passed in
 double get_state_energy(
-    char* state,
+    std::int8_t* state,
     const vector<double>& h,
     const vector<int>& coupler_starts,
     const vector<int>& coupler_ends,
     const vector<double>& coupler_weights
 ) {
     double energy = 0.0;
     // sum the energy due to local fields on variables
@@ -202,15 +221,15 @@
     for (unsigned int c = 0; c < coupler_starts.size(); c++) {
         energy += state[coupler_starts[c]] * coupler_weights[c] * state[coupler_ends[c]];
     }
     return energy;
 }
 
 // Perform simulated annealing on a general problem
-// @param states a char array of size num_samples * number of variables in the
+// @param states a int8 array of size num_samples * number of variables in the
 //        problem. Will be overwritten by this function as samples are filled
 //        in. The initial state of the samples are used to seed the simulated
 //        annealing runs.
 // @param energies a double array of size num_samples. Will be overwritten by
 //        this function as energies are filled in.
 // @param num_samples the number of samples to get.
 // @param h vector of h or field value on each variable
@@ -226,29 +245,31 @@
 // @param beta_schedule A list of the beta values to run `sweeps_per_beta`
 //        sweeps at.
 // @param interrupt_callback A function that is invoked between each run of simulated annealing
 //        if the function returns True then it will stop running.
 // @param interrupt_function A pointer to contents that are passed to interrupt_callback.
 // @return the number of samples taken. If no interrupt occured, will equal num_samples.
 int general_simulated_annealing(
-    char* states,
+    std::int8_t* states,
     double* energies,
     const int num_samples,
     const vector<double> h,
     const vector<int> coupler_starts,
     const vector<int> coupler_ends,
     const vector<double> coupler_weights,
     const int sweeps_per_beta,
     const vector<double> beta_schedule,
     const uint64_t seed,
+    const VariableOrder varorder,
+    const Proposal proposal_acceptance_criteria,
     callback interrupt_callback,
     void * const interrupt_function
 ) {
     // TODO 
-    // assert len(states) == num_samples*num_vars*sizeof(char)
+    // assert len(states) == num_samples*num_vars*sizeof(int8_t)
     // assert len(coupler_starts) == len(coupler_ends) == len(coupler_weights)
     // assert max(coupler_starts + coupler_ends) < num_vars
     
     // the number of variables in the problem
     const int num_vars = h.size();
     if (!((coupler_starts.size() == coupler_ends.size()) &&
                 (coupler_starts.size() == coupler_weights.size()))) {
@@ -295,21 +316,39 @@
 
     // get the simulated annealing samples
     int sample = 0;
     while (sample < num_samples) {
         // states is a giant spin array that will hold the resulting states for
         // all the samples, so we need to get the location inside that vector
         // where we will store the sample for this sample
-        char *state = states + sample*num_vars;
+        std::int8_t *state = states + sample*num_vars;
         // then do the actual sample. this function will modify state, storing
         // the sample there
-        simulated_annealing_run(state, h, degrees, 
-                                neighbors, neighbour_couplings, 
-                                sweeps_per_beta, beta_schedule);
-
+	// Branching here is designed to make expicit compile time optimizations
+        if (varorder == Random) {
+            if (proposal_acceptance_criteria == Metropolis) {
+                simulated_annealing_run<Random, Metropolis>(state, h, degrees,
+                                                    neighbors, neighbour_couplings,
+                                                    sweeps_per_beta, beta_schedule);
+            } else {
+                simulated_annealing_run<Random, Gibbs>(state, h, degrees,
+                                                     neighbors, neighbour_couplings,
+                                                     sweeps_per_beta, beta_schedule);
+          }
+        } else {
+            if (proposal_acceptance_criteria == Metropolis) {
+                simulated_annealing_run<Sequential, Metropolis>(state, h, degrees,
+                                                     neighbors, neighbour_couplings,
+                                                     sweeps_per_beta, beta_schedule);
+            } else {
+                simulated_annealing_run<Sequential, Gibbs>(state, h, degrees,
+                                                      neighbors, neighbour_couplings,
+                                                      sweeps_per_beta, beta_schedule);
+            }
+        }
         // compute the energy of the sample and store it in `energies`
         energies[sample] = get_state_energy(state, h, coupler_starts, 
                                             coupler_ends, coupler_weights);
 
         sample++;
 
         // if interrupt_function returns true, stop sampling
```

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/sa/src/cpu_sa.h` & `dwave-samplers-1.1.0/dwave/samplers/sa/src/cpu_sa.h`

 * *Files 26% similar despite different names*

```diff
@@ -13,53 +13,66 @@
 // limitations under the License.
 //
 // ===========================================================================
 
 #ifndef _cpu_sa_h
 #define _cpu_sa_h
 
+#include <cstdint>
+
 #ifdef _MSC_VER
     // add uint64_t definition for windows
     typedef __int64 int64_t;
     typedef unsigned __int64 uint64_t;
 
     // add thread_local (C++11) support for MSVC 9 and 10 (py2.7 and py3.4 on win)
     // note: thread_local support was added in MSVC 14 (Visual Studio 2015, MSC_VER 1900)
     #if _MSC_VER < 1900
     #define thread_local __declspec(thread)
     #endif
 #endif
 
+enum Proposal {
+    Gibbs,       /// Gibbs acceptance critera on each variable update
+    Metropolis,  /// Metropolis acceptance criteria one each variable update
+};
+enum VariableOrder {
+    Sequential,   /// Variables updated sequentially on each sweep
+    Random,       /// Variable updated uniformly at random per spin-update
+};
+
 double get_flip_energy(
-    int var, char *state, const std::vector<double> & h,
+    int var, std::int8_t *state, const std::vector<double> & h,
     const std::vector<int>& degrees,
     const std::vector<std::vector<int>>& neighbors,
     const std::vector<std::vector<double>>& neighbour_couplings
 );
 
 void simulated_annealing_run(
-    char *state, const std::vector<double>& h,
+    std::int8_t *state, const std::vector<double>& h,
     const std::vector<int>& degrees,
     const std::vector<std::vector<int>>& neighbors,
     const std::vector<std::vector<double>>& neighbour_couplings,
     const int sweeps_per_beta,
     const std::vector<double>& beta_schedule
 );
 
 typedef bool (*const callback)(void * const function);
 
 int general_simulated_annealing(
-    char *states,
+    std::int8_t *states,
     double *energies,
     const int num_samples,
     const std::vector<double> h,
     const std::vector<int> coupler_starts,
     const std::vector<int> coupler_ends,
     const std::vector<double> coupler_values,
     const int sweeps_per_beta,
     const std::vector<double> beta_schedule,
     const uint64_t seed,
+    const VariableOrder varorder,
+    const Proposal proposal_acceptance_criteria,
     callback interrupt_callback,
     void * const interrupt_function
 );
 
 #endif
```

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/tabu/__init__.py` & `dwave-samplers-1.1.0/dwave/samplers/tabu/__init__.py`

 * *Files identical despite different names*

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/tabu/sampler.py` & `dwave-samplers-1.1.0/dwave/samplers/tabu/sampler.py`

 * *Files identical despite different names*

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/tabu/src/bqp.cpp` & `dwave-samplers-1.1.0/dwave/samplers/tabu/src/bqp.cpp`

 * *Files identical despite different names*

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/tabu/src/bqp.h` & `dwave-samplers-1.1.0/dwave/samplers/tabu/src/bqp.h`

 * *Files identical despite different names*

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/tabu/src/common.h` & `dwave-samplers-1.1.0/dwave/samplers/tabu/src/common.h`

 * *Files identical despite different names*

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/tabu/src/tabu_search.cpp` & `dwave-samplers-1.1.0/dwave/samplers/tabu/src/tabu_search.cpp`

 * *Files identical despite different names*

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/tabu/src/tabu_search.h` & `dwave-samplers-1.1.0/dwave/samplers/tabu/src/tabu_search.h`

 * *Files identical despite different names*

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/tabu/src/tabu_utils.cpp` & `dwave-samplers-1.1.0/dwave/samplers/tabu/src/tabu_utils.cpp`

 * *Files identical despite different names*

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/tabu/src/tabu_utils.h` & `dwave-samplers-1.1.0/dwave/samplers/tabu/src/tabu_utils.h`

 * *Files identical despite different names*

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/tabu/tabu.pxd` & `dwave-samplers-1.1.0/dwave/samplers/tabu/tabu.pxd`

 * *Files identical despite different names*

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/tabu/tabu_search.cpp` & `dwave-samplers-1.1.0/dwave/samplers/tabu/tabu_search.cpp`

 * *Files identical despite different names*

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/tabu/tabu_search.pyx` & `dwave-samplers-1.1.0/dwave/samplers/tabu/tabu_search.pyx`

 * *Files identical despite different names*

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/tabu/utils.py` & `dwave-samplers-1.1.0/dwave/samplers/tabu/utils.py`

 * *Files identical despite different names*

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/tree/__init__.py` & `dwave-samplers-1.1.0/dwave/samplers/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/tree/orang.pxd` & `dwave-samplers-1.1.0/dwave/samplers/tree/orang.pxd`

 * *Files identical despite different names*

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/tree/sample.cpp` & `dwave-samplers-1.1.0/dwave/samplers/tree/sample.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -717,17 +717,14 @@
 #define __PYX_HAVE__dwave__samplers__tree__sample
 #define __PYX_HAVE_API__dwave__samplers__tree__sample
 /* Early includes */
 #include <string.h>
 #include <stdlib.h>
 #include <stdio.h>
 #include "numpy/arrayobject.h"
-#include "numpy/ndarrayobject.h"
-#include "numpy/ndarraytypes.h"
-#include "numpy/arrayscalars.h"
 #include "numpy/ufuncobject.h"
 
     /* NumPy API declarations from "numpy/__init__.pxd" */
     
 #include "ios"
 #include "new"
 #include "stdexcept"
@@ -1108,195 +1105,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":690
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":691
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":692
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":693
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":697
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":698
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":699
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":700
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":704
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":705
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":714
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":715
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":716
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":718
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":719
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":720
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":722
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":723
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":725
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":726
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":727
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1394,42 +1391,42 @@
 struct __pyx_obj_5dimod_9quadratic_4cyqm_12cyqm_float64_cyQM_template;
 struct __pyx_obj_5dimod_9quadratic_4cyqm_12cyqm_float64_cyQM_float64;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":729
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":730
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":731
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":733
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -2883,24 +2880,14 @@
 /* Module declarations from 'numpy' */
 
 /* Module declarations from 'numpy' */
 static PyTypeObject *__pyx_ptype_5numpy_dtype = 0;
 static PyTypeObject *__pyx_ptype_5numpy_flatiter = 0;
 static PyTypeObject *__pyx_ptype_5numpy_broadcast = 0;
 static PyTypeObject *__pyx_ptype_5numpy_ndarray = 0;
-static PyTypeObject *__pyx_ptype_5numpy_generic = 0;
-static PyTypeObject *__pyx_ptype_5numpy_number = 0;
-static PyTypeObject *__pyx_ptype_5numpy_integer = 0;
-static PyTypeObject *__pyx_ptype_5numpy_signedinteger = 0;
-static PyTypeObject *__pyx_ptype_5numpy_unsignedinteger = 0;
-static PyTypeObject *__pyx_ptype_5numpy_inexact = 0;
-static PyTypeObject *__pyx_ptype_5numpy_floating = 0;
-static PyTypeObject *__pyx_ptype_5numpy_complexfloating = 0;
-static PyTypeObject *__pyx_ptype_5numpy_flexible = 0;
-static PyTypeObject *__pyx_ptype_5numpy_character = 0;
 static PyTypeObject *__pyx_ptype_5numpy_ufunc = 0;
 
 /* Module declarations from 'dimod.cyvariables' */
 static PyTypeObject *__pyx_ptype_5dimod_11cyvariables_cyVariables = 0;
 
 /* Module declarations from 'libcpp.utility' */
 
@@ -4589,15 +4576,15 @@
   __Pyx_XDECREF(__pyx_v_interactions);
   __Pyx_XDECREF(__pyx_v_marginal_data);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":735
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -4606,29 +4593,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":736
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 736, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":735
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -4639,15 +4626,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":738
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -4656,29 +4643,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":739
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 739, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":738
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -4689,15 +4676,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":741
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -4706,29 +4693,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":742
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 742, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":741
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -4739,15 +4726,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":744
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -4756,29 +4743,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":745
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 745, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":744
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -4789,15 +4776,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":747
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -4806,29 +4793,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":748
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 748, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":747
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -4839,212 +4826,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":750
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":751
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":752
+    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":751
+    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":754
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":750
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":929
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":868
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":930
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":869
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":931
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":870
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":929
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":868
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":933
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":872
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":934
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":873
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":935
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":874
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":936
+    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":875
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":935
+    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":874
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":937
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":876
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":933
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":872
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":941
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":880
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -5060,15 +5047,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":942
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":881
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -5076,84 +5063,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":943
+      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":882
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 943, __pyx_L3_error)
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 882, __pyx_L3_error)
 
-      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":942
+      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":881
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":944
+    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":883
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 944, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 883, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":945
+      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":884
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 945, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 884, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 945, __pyx_L5_except_error)
+      __PYX_ERR(1, 884, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":942
+    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":881
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":941
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":880
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -5168,15 +5155,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":947
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":886
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5192,15 +5179,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":948
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":887
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -5208,84 +5195,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":949
+      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":888
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 949, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 888, __pyx_L3_error)
 
-      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":948
+      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":887
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":950
+    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":889
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 950, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 889, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":951
+      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":890
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 951, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 890, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 951, __pyx_L5_except_error)
+      __PYX_ERR(1, 890, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":948
+    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":887
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":947
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":886
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5300,15 +5287,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":953
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":892
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5324,15 +5311,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":954
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":893
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -5340,84 +5327,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":955
+      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":894
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 955, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 894, __pyx_L3_error)
 
-      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":954
+      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":893
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":956
+    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":895
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 956, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 895, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":957
+      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":896
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 957, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 896, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 957, __pyx_L5_except_error)
+      __PYX_ERR(1, 896, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":954
+    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":893
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":953
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":892
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5432,188 +5419,14 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":967
- * 
- * 
- * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
- *     """
- *     Cython equivalent of `isinstance(obj, np.timedelta64)`
- */
-
-static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
-
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":979
- *     bool
- *     """
- *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
-  goto __pyx_L0;
-
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":967
- * 
- * 
- * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
- *     """
- *     Cython equivalent of `isinstance(obj, np.timedelta64)`
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":982
- * 
- * 
- * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
- *     """
- *     Cython equivalent of `isinstance(obj, np.datetime64)`
- */
-
-static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("is_datetime64_object", 0);
-
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":994
- *     bool
- *     """
- *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
-  goto __pyx_L0;
-
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":982
- * 
- * 
- * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
- *     """
- *     Cython equivalent of `isinstance(obj, np.datetime64)`
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":997
- * 
- * 
- * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the int64 value underlying scalar numpy datetime64 object
- */
-
-static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
-  npy_datetime __pyx_r;
-
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":1004
- *     also needed.  That can be found using `get_datetime64_unit`.
- *     """
- *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
-  goto __pyx_L0;
-
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":997
- * 
- * 
- * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the int64 value underlying scalar numpy datetime64 object
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  return __pyx_r;
-}
-
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":1007
- * 
- * 
- * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the int64 value underlying scalar numpy timedelta64 object
- */
-
-static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
-  npy_timedelta __pyx_r;
-
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":1011
- *     returns the int64 value underlying scalar numpy timedelta64 object
- *     """
- *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
-  goto __pyx_L0;
-
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":1007
- * 
- * 
- * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the int64 value underlying scalar numpy timedelta64 object
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  return __pyx_r;
-}
-
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":1014
- * 
- * 
- * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the unit part of the dtype for a numpy datetime64 object.
- */
-
-static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
-  NPY_DATETIMEUNIT __pyx_r;
-
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":1018
- *     returns the unit part of the dtype for a numpy datetime64 object.
- *     """
- *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
- */
-  __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
-  goto __pyx_L0;
-
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":1014
- * 
- * 
- * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the unit part of the dtype for a numpy datetime64 object.
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  return __pyx_r;
-}
-
 /* "View.MemoryView":122
  *         cdef bint dtype_is_object
  * 
  *     def __cinit__(array self, tuple shape, Py_ssize_t itemsize, format not None,             # <<<<<<<<<<<<<<
  *                   mode="c", bint allocate_buffer=True):
  * 
  */
@@ -19916,15 +19729,15 @@
   {&__pyx_n_s_variables, __pyx_k_variables, sizeof(__pyx_k_variables), 0, 0, 1, 1},
   {&__pyx_n_s_vartype, __pyx_k_vartype, sizeof(__pyx_k_vartype), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 87, __pyx_L1_error)
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 146, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 945, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 884, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(2, 148, __pyx_L1_error)
   __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(2, 151, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(2, 2, __pyx_L1_error)
   __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(2, 404, __pyx_L1_error)
   __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(2, 613, __pyx_L1_error)
   __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(2, 832, __pyx_L1_error)
   return 0;
@@ -19954,33 +19767,33 @@
  * 
  *     cdef cyBQM_float64 cybqm = bqm.data
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_order_must_contain_the_variables); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 90, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":945
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":884
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 945, __pyx_L1_error)
+  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 884, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":951
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":890
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 951, __pyx_L1_error)
+  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 890, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
 
   /* "View.MemoryView":133
  * 
  *         if not self.ndim:
  *             raise ValueError("Empty shape tuple for cython.array")             # <<<<<<<<<<<<<<
@@ -20383,46 +20196,26 @@
   sizeof(PyTypeObject),
   #else
   sizeof(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 200, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 200, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 199, __pyx_L1_error)
   __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 223, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 222, __pyx_L1_error)
   __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 227, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 226, __pyx_L1_error)
   __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 239, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 771, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 773, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 775, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 777, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 779, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 781, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 783, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 785, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 787, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 789, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
   __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 827, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 764, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("dimod.cyvariables"); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_5dimod_11cyvariables_cyVariables = __Pyx_ImportType(__pyx_t_1, "dimod.cyvariables", "cyVariables", sizeof(struct __pyx_obj_5dimod_11cyvariables_cyVariables), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5dimod_11cyvariables_cyVariables) __PYX_ERR(4, 20, __pyx_L1_error)
   __pyx_vtabptr_5dimod_11cyvariables_cyVariables = (struct __pyx_vtabstruct_5dimod_11cyvariables_cyVariables*)__Pyx_GetVtable(__pyx_ptype_5dimod_11cyvariables_cyVariables->tp_dict); if (unlikely(!__pyx_vtabptr_5dimod_11cyvariables_cyVariables)) __PYX_ERR(4, 20, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
```

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/tree/sample.pyx` & `dwave-samplers-1.1.0/dwave/samplers/tree/sample.pyx`

 * *Files identical despite different names*

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/tree/samplers.py` & `dwave-samplers-1.1.0/dwave/samplers/tree/samplers.py`

 * *Files 4% similar despite different names*

```diff
@@ -186,44 +186,14 @@
 
     The tree decomposition sampler uses `tree decomposition`_ to sample from a
     `Boltzmann distribution`_ defined by the given binary quadratic model.
 
     .. Important:: The performance of this sampler is highly dependant on the
         treewidth of the problem.
 
-    Examples:
-        Create a sampler:
-
-        >>> from dwave.samplers import TreeDecompositionSampler
-        >>> sampler = TreeDecompositionSampler()
-
-        Create a simple Ising problem:
-
-        >>> h = {'a': .1, 'b': 0}
-        >>> J = {('a', 'b') : -1}
-
-        Sample from the given problem.
-
-        >>> sampleset = sampler.sample_ising(h, J, num_reads=100,
-        ...                                  elimination_order=['a', 'b'])
-        >>> sampleset.first.sample
-        {'a': -1, 'b': -1}
-
-        View information about the distribution.
-
-        >>> variable_marginals = sampleset.info['variable_marginals']
-        >>> round(variable_marginals['a'], 3)  # prob(a == 1)
-        0.354
-        >>> round(1 - variable_marginals['b'], 3)  # prob(b == -1)
-        0.645
-
-        >>> pair_marg = sampleset.info['interaction_marginals']
-        >>> round(pair_marg[('a', 'b')][(1, -1)], 3)  # prob(a == 1 & b == -1)
-        0.001
-
     .. _tree decomposition: https://en.wikipedia.org/wiki/Tree_decomposition
 
     .. _Boltzmann distribution: https://en.wikipedia.org/wiki/Boltzmann_distribution
 
     """
     parameters = {'num_reads': [],
                   'elimination_order': ['max_treewidth'],
@@ -257,15 +227,15 @@
 
     def __init__(self):
         # make these object properties rather than class properties
         self.parameters = dict(self.parameters)
         self.properties = dict(self.properties)
 
     def sample(self, bqm: dimod.BinaryQuadraticModel, num_reads: Optional[int] = 1,
-               elimination_order: Optional[List[Variable]] = None, beta: Optional[float] = 3.0,
+               elimination_order: Optional[List[Variable]] = None, beta: Optional[float] = 1.0,
                marginals: Optional[bool] = True, seed: Optional[int] = None) -> dimod.SampleSet:
         """Draw samples and compute marginals of a binary quadratic model.
 
         Args:
             bqm:
                 Binary quadratic model.
```

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/tree/solve.cpp` & `dwave-samplers-1.1.0/dwave/samplers/tree/solve.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -716,17 +716,14 @@
 
 #define __PYX_HAVE__dwave__samplers__tree__solve
 #define __PYX_HAVE_API__dwave__samplers__tree__solve
 /* Early includes */
 #include <string.h>
 #include <stdio.h>
 #include "numpy/arrayobject.h"
-#include "numpy/ndarrayobject.h"
-#include "numpy/ndarraytypes.h"
-#include "numpy/arrayscalars.h"
 #include "numpy/ufuncobject.h"
 
     /* NumPy API declarations from "numpy/__init__.pxd" */
     
 #include "ios"
 #include "new"
 #include "stdexcept"
@@ -1108,195 +1105,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":690
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":691
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":692
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":693
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":697
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":698
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":699
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":700
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":704
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":705
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":714
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":715
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":716
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":718
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":719
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":720
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":722
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":723
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":725
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":726
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":727
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1394,42 +1391,42 @@
 struct __pyx_obj_5dimod_9quadratic_4cyqm_12cyqm_float64_cyQM_template;
 struct __pyx_obj_5dimod_9quadratic_4cyqm_12cyqm_float64_cyQM_float64;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":729
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":730
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":731
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":733
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -2864,24 +2861,14 @@
 /* Module declarations from 'numpy' */
 
 /* Module declarations from 'numpy' */
 static PyTypeObject *__pyx_ptype_5numpy_dtype = 0;
 static PyTypeObject *__pyx_ptype_5numpy_flatiter = 0;
 static PyTypeObject *__pyx_ptype_5numpy_broadcast = 0;
 static PyTypeObject *__pyx_ptype_5numpy_ndarray = 0;
-static PyTypeObject *__pyx_ptype_5numpy_generic = 0;
-static PyTypeObject *__pyx_ptype_5numpy_number = 0;
-static PyTypeObject *__pyx_ptype_5numpy_integer = 0;
-static PyTypeObject *__pyx_ptype_5numpy_signedinteger = 0;
-static PyTypeObject *__pyx_ptype_5numpy_unsignedinteger = 0;
-static PyTypeObject *__pyx_ptype_5numpy_inexact = 0;
-static PyTypeObject *__pyx_ptype_5numpy_floating = 0;
-static PyTypeObject *__pyx_ptype_5numpy_complexfloating = 0;
-static PyTypeObject *__pyx_ptype_5numpy_flexible = 0;
-static PyTypeObject *__pyx_ptype_5numpy_character = 0;
 static PyTypeObject *__pyx_ptype_5numpy_ufunc = 0;
 
 /* Module declarations from 'dimod.cyvariables' */
 static PyTypeObject *__pyx_ptype_5dimod_11cyvariables_cyVariables = 0;
 
 /* Module declarations from 'libcpp.utility' */
 
@@ -4020,15 +4007,15 @@
   __Pyx_XDECREF(__pyx_v_samples);
   __Pyx_XDECREF(__pyx_v_energies);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":735
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -4037,29 +4024,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":736
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 736, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":735
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -4070,15 +4057,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":738
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -4087,29 +4074,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":739
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 739, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":738
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -4120,15 +4107,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":741
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -4137,29 +4124,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":742
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 742, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":741
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -4170,15 +4157,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":744
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -4187,29 +4174,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":745
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 745, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":744
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -4220,15 +4207,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":747
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -4237,29 +4224,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":748
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 748, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":747
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -4270,212 +4257,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":750
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":751
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":752
+    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":751
+    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":754
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":750
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":929
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":868
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":930
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":869
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":931
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":870
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":929
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":868
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":933
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":872
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":934
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":873
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":935
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":874
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":936
+    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":875
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":935
+    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":874
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":937
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":876
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":933
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":872
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":941
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":880
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4491,15 +4478,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":942
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":881
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -4507,84 +4494,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":943
+      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":882
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 943, __pyx_L3_error)
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 882, __pyx_L3_error)
 
-      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":942
+      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":881
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":944
+    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":883
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 944, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 883, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":945
+      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":884
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 945, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 884, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 945, __pyx_L5_except_error)
+      __PYX_ERR(1, 884, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":942
+    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":881
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":941
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":880
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4599,15 +4586,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":947
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":886
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4623,15 +4610,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":948
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":887
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4639,84 +4626,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":949
+      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":888
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 949, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 888, __pyx_L3_error)
 
-      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":948
+      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":887
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":950
+    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":889
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 950, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 889, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":951
+      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":890
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 951, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 890, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 951, __pyx_L5_except_error)
+      __PYX_ERR(1, 890, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":948
+    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":887
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":947
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":886
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4731,15 +4718,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":953
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":892
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4755,15 +4742,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":954
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":893
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4771,84 +4758,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":955
+      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":894
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 955, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 894, __pyx_L3_error)
 
-      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":954
+      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":893
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":956
+    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":895
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 956, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 895, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":957
+      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":896
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 957, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 896, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 957, __pyx_L5_except_error)
+      __PYX_ERR(1, 896, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":954
+    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":893
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":953
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":892
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4863,188 +4850,14 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":967
- * 
- * 
- * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
- *     """
- *     Cython equivalent of `isinstance(obj, np.timedelta64)`
- */
-
-static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
-
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":979
- *     bool
- *     """
- *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
-  goto __pyx_L0;
-
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":967
- * 
- * 
- * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
- *     """
- *     Cython equivalent of `isinstance(obj, np.timedelta64)`
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":982
- * 
- * 
- * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
- *     """
- *     Cython equivalent of `isinstance(obj, np.datetime64)`
- */
-
-static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("is_datetime64_object", 0);
-
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":994
- *     bool
- *     """
- *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
-  goto __pyx_L0;
-
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":982
- * 
- * 
- * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
- *     """
- *     Cython equivalent of `isinstance(obj, np.datetime64)`
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":997
- * 
- * 
- * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the int64 value underlying scalar numpy datetime64 object
- */
-
-static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
-  npy_datetime __pyx_r;
-
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":1004
- *     also needed.  That can be found using `get_datetime64_unit`.
- *     """
- *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
-  goto __pyx_L0;
-
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":997
- * 
- * 
- * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the int64 value underlying scalar numpy datetime64 object
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  return __pyx_r;
-}
-
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":1007
- * 
- * 
- * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the int64 value underlying scalar numpy timedelta64 object
- */
-
-static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
-  npy_timedelta __pyx_r;
-
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":1011
- *     returns the int64 value underlying scalar numpy timedelta64 object
- *     """
- *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
-  goto __pyx_L0;
-
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":1007
- * 
- * 
- * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the int64 value underlying scalar numpy timedelta64 object
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  return __pyx_r;
-}
-
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":1014
- * 
- * 
- * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the unit part of the dtype for a numpy datetime64 object.
- */
-
-static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
-  NPY_DATETIMEUNIT __pyx_r;
-
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":1018
- *     returns the unit part of the dtype for a numpy datetime64 object.
- *     """
- *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
- */
-  __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
-  goto __pyx_L0;
-
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":1014
- * 
- * 
- * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the unit part of the dtype for a numpy datetime64 object.
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  return __pyx_r;
-}
-
 /* "View.MemoryView":122
  *         cdef bint dtype_is_object
  * 
  *     def __cinit__(array self, tuple shape, Py_ssize_t itemsize, format not None,             # <<<<<<<<<<<<<<
  *                   mode="c", bint allocate_buffer=True):
  * 
  */
@@ -19326,15 +19139,15 @@
   {&__pyx_n_s_variables, __pyx_k_variables, sizeof(__pyx_k_variables), 0, 0, 1, 1},
   {&__pyx_n_s_vartype, __pyx_k_vartype, sizeof(__pyx_k_vartype), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 67, __pyx_L1_error)
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 105, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 945, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 884, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(2, 148, __pyx_L1_error)
   __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(2, 151, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(2, 2, __pyx_L1_error)
   __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(2, 404, __pyx_L1_error)
   __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(2, 613, __pyx_L1_error)
   __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(2, 832, __pyx_L1_error)
   return 0;
@@ -19364,33 +19177,33 @@
  * 
  *     cdef cyBQM_float64 cybqm = bqm.data
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_order_must_contain_the_variables); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":945
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":884
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 945, __pyx_L1_error)
+  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 884, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":951
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":890
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 951, __pyx_L1_error)
+  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 890, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
 
   /* "View.MemoryView":133
  * 
  *         if not self.ndim:
  *             raise ValueError("Empty shape tuple for cython.array")             # <<<<<<<<<<<<<<
@@ -19793,46 +19606,26 @@
   sizeof(PyTypeObject),
   #else
   sizeof(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 200, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 200, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 199, __pyx_L1_error)
   __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 223, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 222, __pyx_L1_error)
   __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 227, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 226, __pyx_L1_error)
   __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 239, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 771, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 773, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 775, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 777, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 779, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 781, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 783, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 785, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 787, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 789, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
   __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 827, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 764, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("dimod.cyvariables"); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_5dimod_11cyvariables_cyVariables = __Pyx_ImportType(__pyx_t_1, "dimod.cyvariables", "cyVariables", sizeof(struct __pyx_obj_5dimod_11cyvariables_cyVariables), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5dimod_11cyvariables_cyVariables) __PYX_ERR(4, 20, __pyx_L1_error)
   __pyx_vtabptr_5dimod_11cyvariables_cyVariables = (struct __pyx_vtabstruct_5dimod_11cyvariables_cyVariables*)__Pyx_GetVtable(__pyx_ptype_5dimod_11cyvariables_cyVariables->tp_dict); if (unlikely(!__pyx_vtabptr_5dimod_11cyvariables_cyVariables)) __PYX_ERR(4, 20, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
```

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/tree/solve.pyx` & `dwave-samplers-1.1.0/dwave/samplers/tree/solve.pyx`

 * *Files identical despite different names*

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/tree/src/include/base.h` & `dwave-samplers-1.1.0/dwave/samplers/tree/src/include/base.h`

 * *Files identical despite different names*

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/tree/src/include/buckettree.h` & `dwave-samplers-1.1.0/dwave/samplers/tree/src/include/buckettree.h`

 * *Files identical despite different names*

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/tree/src/include/combine.h` & `dwave-samplers-1.1.0/dwave/samplers/tree/src/include/combine.h`

 * *Files identical despite different names*

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/tree/src/include/exception.h` & `dwave-samplers-1.1.0/dwave/samplers/tree/src/include/exception.h`

 * *Files identical despite different names*

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/tree/src/include/graph.h` & `dwave-samplers-1.1.0/dwave/samplers/tree/src/include/graph.h`

 * *Files identical despite different names*

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/tree/src/include/marginalizer.h` & `dwave-samplers-1.1.0/dwave/samplers/tree/src/include/marginalizer.h`

 * *Files identical despite different names*

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/tree/src/include/merger.h` & `dwave-samplers-1.1.0/dwave/samplers/tree/src/include/merger.h`

 * *Files identical despite different names*

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/tree/src/include/operations/count.h` & `dwave-samplers-1.1.0/dwave/samplers/tree/src/include/operations/count.h`

 * *Files identical despite different names*

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/tree/src/include/operations/dummy.h` & `dwave-samplers-1.1.0/dwave/samplers/tree/src/include/operations/dummy.h`

 * *Files identical despite different names*

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/tree/src/include/operations/logsumprod.h` & `dwave-samplers-1.1.0/dwave/samplers/tree/src/include/operations/logsumprod.h`

 * *Files 7% similar despite different names*

```diff
@@ -60,16 +60,14 @@
   varstep_vector inVarsSteps_;
   Var outVar_;
   DomIndex outStepSize_;
   std::vector<double> cumProbs_;
 
   virtual double marginalizeImpl(std::size_t n, const table_type& mrgTable) {
     using std::transform;
-    using std::divides;
-    using std::bind2nd;
     using std::make_pair;
     typedef std::vector<double>::iterator value_iterator;
 
     double yMax = *std::max_element(mrgTable.begin(), mrgTable.end());
     double fsum(0.0);
 
     value_iterator cpBegin = cumProbs_.begin() + n * outStepSize_;
@@ -79,35 +77,34 @@
     while (cpIter != cpEnd) {
       fsum += exp(*tblIter - yMax);
       *cpIter = fsum;
       ++cpIter;
       ++tblIter;
     }
     fsum += exp(*tblIter - yMax);
-    transform(cpBegin, cpEnd, cpBegin, bind2nd(divides<double>(), fsum));
+    transform(cpBegin, cpEnd, cpBegin, [&](double a){ return a / fsum; });
 
     return yMax + log(fsum);
   }
 
   virtual void solveImpl(DomIndexVector& s) const {
     using std::find_if;
-    using std::less;
-    using std::bind1st;
     using std::make_pair;
     typedef std::vector<double>::const_iterator value_const_iterator;
 
     size_t n = 0;
     for (const auto &vs: inVarsSteps_) {
       n += s[vs.first] * vs.second;
     }
     n *= outStepSize_;
 
     value_const_iterator cpBegin = cumProbs_.begin() + n;
     value_const_iterator cpEnd = cpBegin + outStepSize_;
-    value_const_iterator cpFound = find_if(cpBegin, cpEnd, bind1st(less<double>(), rng_()));
+    const double rng = rng_();
+    value_const_iterator cpFound = find_if(cpBegin, cpEnd, [&](double a){ return rng < a; });
     DomIndex outI = static_cast<DomIndex>(cpFound - cpBegin);
 
     s[outVar_] = outI;
   }
 
 public:
```

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/tree/src/include/operations/min.h` & `dwave-samplers-1.1.0/dwave/samplers/tree/src/include/operations/min.h`

 * *Files identical despite different names*

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/tree/src/include/orang.h` & `dwave-samplers-1.1.0/dwave/samplers/tree/src/include/orang.h`

 * *Files identical despite different names*

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/tree/src/include/sample.hpp` & `dwave-samplers-1.1.0/dwave/samplers/tree/src/include/sample.hpp`

 * *Files identical despite different names*

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/tree/src/include/solve.hpp` & `dwave-samplers-1.1.0/dwave/samplers/tree/src/include/solve.hpp`

 * *Files identical despite different names*

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/tree/src/include/table.h` & `dwave-samplers-1.1.0/dwave/samplers/tree/src/include/table.h`

 * *Files identical despite different names*

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/tree/src/include/task.h` & `dwave-samplers-1.1.0/dwave/samplers/tree/src/include/task.h`

 * *Files identical despite different names*

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/tree/src/include/treedecomp.h` & `dwave-samplers-1.1.0/dwave/samplers/tree/src/include/treedecomp.h`

 * *Files identical despite different names*

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/tree/src/include/utils.hpp` & `dwave-samplers-1.1.0/dwave/samplers/tree/src/include/utils.hpp`

 * *Files identical despite different names*

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/tree/src/include/varorder.h` & `dwave-samplers-1.1.0/dwave/samplers/tree/src/include/varorder.h`

 * *Files identical despite different names*

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/tree/utilities.cpp` & `dwave-samplers-1.1.0/dwave/samplers/tree/utilities.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -732,17 +732,14 @@
     #endif
     
 #include <unordered_map>
 #include <unordered_set>
 #include <string.h>
 #include <stdio.h>
 #include "numpy/arrayobject.h"
-#include "numpy/ndarrayobject.h"
-#include "numpy/ndarraytypes.h"
-#include "numpy/arrayscalars.h"
 #include "numpy/ufuncobject.h"
 
     /* NumPy API declarations from "numpy/__init__.pxd" */
     
 #include "dimod/vartypes.h"
 #include "dimod/abc.h"
 #include "dimod/binary_quadratic_model.h"
@@ -1101,195 +1098,195 @@
   Py_ssize_t shape[8];
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":690
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":691
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":692
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":693
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":697
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":698
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":699
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":700
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":704
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":705
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":714
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":715
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":716
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":718
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":719
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":720
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":722
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":723
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":725
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":726
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":727
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1369,42 +1366,42 @@
 struct __pyx_obj_5dimod_9quadratic_4cyqm_12cyqm_float64_cyQM_template;
 struct __pyx_obj_5dimod_9quadratic_4cyqm_12cyqm_float64_cyQM_float64;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":729
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":730
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":731
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":733
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -2785,24 +2782,14 @@
 /* Module declarations from 'numpy' */
 
 /* Module declarations from 'numpy' */
 static PyTypeObject *__pyx_ptype_5numpy_dtype = 0;
 static PyTypeObject *__pyx_ptype_5numpy_flatiter = 0;
 static PyTypeObject *__pyx_ptype_5numpy_broadcast = 0;
 static PyTypeObject *__pyx_ptype_5numpy_ndarray = 0;
-static PyTypeObject *__pyx_ptype_5numpy_generic = 0;
-static PyTypeObject *__pyx_ptype_5numpy_number = 0;
-static PyTypeObject *__pyx_ptype_5numpy_integer = 0;
-static PyTypeObject *__pyx_ptype_5numpy_signedinteger = 0;
-static PyTypeObject *__pyx_ptype_5numpy_unsignedinteger = 0;
-static PyTypeObject *__pyx_ptype_5numpy_inexact = 0;
-static PyTypeObject *__pyx_ptype_5numpy_floating = 0;
-static PyTypeObject *__pyx_ptype_5numpy_complexfloating = 0;
-static PyTypeObject *__pyx_ptype_5numpy_flexible = 0;
-static PyTypeObject *__pyx_ptype_5numpy_character = 0;
 static PyTypeObject *__pyx_ptype_5numpy_ufunc = 0;
 
 /* Module declarations from 'dimod.cyvariables' */
 static PyTypeObject *__pyx_ptype_5dimod_11cyvariables_cyVariables = 0;
 
 /* Module declarations from 'dimod.libcpp.vartypes' */
 
@@ -4292,15 +4279,15 @@
   __Pyx_XDECREF((PyObject *)__pyx_v_cybqm);
   __Pyx_XDECREF(__pyx_v_variables);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":735
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -4309,29 +4296,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":736
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 736, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":735
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -4342,15 +4329,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":738
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -4359,29 +4346,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":739
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 739, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":738
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -4392,15 +4379,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":741
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -4409,29 +4396,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":742
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 742, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":741
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -4442,15 +4429,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":744
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -4459,29 +4446,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":745
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 745, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":744
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -4492,15 +4479,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":747
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -4509,29 +4496,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":748
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 748, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":747
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -4542,212 +4529,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":750
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":751
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":752
+    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":751
+    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":754
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":750
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":929
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":868
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":930
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":869
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":931
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":870
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":929
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":868
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":933
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":872
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":934
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":873
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":935
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":874
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":936
+    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":875
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":935
+    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":874
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":937
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":876
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":933
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":872
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":941
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":880
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4763,15 +4750,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":942
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":881
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -4779,84 +4766,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":943
+      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":882
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 943, __pyx_L3_error)
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 882, __pyx_L3_error)
 
-      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":942
+      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":881
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":944
+    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":883
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 944, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 883, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":945
+      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":884
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 945, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 884, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 945, __pyx_L5_except_error)
+      __PYX_ERR(1, 884, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":942
+    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":881
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":941
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":880
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4871,15 +4858,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":947
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":886
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4895,15 +4882,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":948
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":887
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4911,84 +4898,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":949
+      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":888
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 949, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 888, __pyx_L3_error)
 
-      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":948
+      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":887
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":950
+    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":889
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 950, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 889, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":951
+      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":890
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 951, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 890, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 951, __pyx_L5_except_error)
+      __PYX_ERR(1, 890, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":948
+    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":887
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":947
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":886
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5003,15 +4990,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":953
+/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":892
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5027,15 +5014,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":954
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":893
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -5043,84 +5030,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":955
+      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":894
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 955, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 894, __pyx_L3_error)
 
-      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":954
+      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":893
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":956
+    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":895
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 956, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 895, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":957
+      /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":896
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 957, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 896, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 957, __pyx_L5_except_error)
+      __PYX_ERR(1, 896, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":954
+    /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":893
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":953
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":892
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5135,188 +5122,14 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":967
- * 
- * 
- * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
- *     """
- *     Cython equivalent of `isinstance(obj, np.timedelta64)`
- */
-
-static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
-
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":979
- *     bool
- *     """
- *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
-  goto __pyx_L0;
-
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":967
- * 
- * 
- * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
- *     """
- *     Cython equivalent of `isinstance(obj, np.timedelta64)`
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":982
- * 
- * 
- * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
- *     """
- *     Cython equivalent of `isinstance(obj, np.datetime64)`
- */
-
-static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("is_datetime64_object", 0);
-
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":994
- *     bool
- *     """
- *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
-  goto __pyx_L0;
-
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":982
- * 
- * 
- * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
- *     """
- *     Cython equivalent of `isinstance(obj, np.datetime64)`
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":997
- * 
- * 
- * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the int64 value underlying scalar numpy datetime64 object
- */
-
-static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
-  npy_datetime __pyx_r;
-
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":1004
- *     also needed.  That can be found using `get_datetime64_unit`.
- *     """
- *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
-  goto __pyx_L0;
-
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":997
- * 
- * 
- * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the int64 value underlying scalar numpy datetime64 object
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  return __pyx_r;
-}
-
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":1007
- * 
- * 
- * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the int64 value underlying scalar numpy timedelta64 object
- */
-
-static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
-  npy_timedelta __pyx_r;
-
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":1011
- *     returns the int64 value underlying scalar numpy timedelta64 object
- *     """
- *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
-  goto __pyx_L0;
-
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":1007
- * 
- * 
- * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the int64 value underlying scalar numpy timedelta64 object
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  return __pyx_r;
-}
-
-/* "env/lib/python3.9/site-packages/numpy/__init__.pxd":1014
- * 
- * 
- * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the unit part of the dtype for a numpy datetime64 object.
- */
-
-static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
-  NPY_DATETIMEUNIT __pyx_r;
-
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":1018
- *     returns the unit part of the dtype for a numpy datetime64 object.
- *     """
- *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
- */
-  __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
-  goto __pyx_L0;
-
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":1014
- * 
- * 
- * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the unit part of the dtype for a numpy datetime64 object.
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  return __pyx_r;
-}
-
 /* "View.MemoryView":122
  *         cdef bint dtype_is_object
  * 
  *     def __cinit__(array self, tuple shape, Py_ssize_t itemsize, format not None,             # <<<<<<<<<<<<<<
  *                   mode="c", bint allocate_buffer=True):
  * 
  */
@@ -19216,15 +19029,15 @@
   {&__pyx_n_s_variables, __pyx_k_variables, sizeof(__pyx_k_variables), 0, 0, 1, 1},
   {&__pyx_n_s_vi, __pyx_k_vi, sizeof(__pyx_k_vi), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 24, __pyx_L1_error)
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 66, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 945, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 884, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(2, 148, __pyx_L1_error)
   __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(2, 151, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(2, 2, __pyx_L1_error)
   __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(2, 404, __pyx_L1_error)
   __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(2, 613, __pyx_L1_error)
   __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(2, 832, __pyx_L1_error)
   return 0;
@@ -19243,33 +19056,33 @@
  * 
  *     cdef dimod.cyBQM_float64 cybqm = dimod.as_bqm(bqm, dtype=float).data
  */
   __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_bqm_and_order_must_have_the_name); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":945
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":884
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 945, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 884, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":951
+  /* "env/lib/python3.9/site-packages/numpy/__init__.pxd":890
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 951, __pyx_L1_error)
+  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 890, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
   /* "View.MemoryView":133
  * 
  *         if not self.ndim:
  *             raise ValueError("Empty shape tuple for cython.array")             # <<<<<<<<<<<<<<
@@ -19684,46 +19497,26 @@
   sizeof(PyTypeObject),
   #else
   sizeof(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 200, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 200, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 199, __pyx_L1_error)
   __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 223, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 222, __pyx_L1_error)
   __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 227, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 226, __pyx_L1_error)
   __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 239, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 771, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 773, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 775, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 777, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 779, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 781, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 783, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 785, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 787, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 789, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
   __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 827, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 764, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("dimod.cyvariables"); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_5dimod_11cyvariables_cyVariables = __Pyx_ImportType(__pyx_t_1, "dimod.cyvariables", "cyVariables", sizeof(struct __pyx_obj_5dimod_11cyvariables_cyVariables), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5dimod_11cyvariables_cyVariables) __PYX_ERR(4, 20, __pyx_L1_error)
   __pyx_vtabptr_5dimod_11cyvariables_cyVariables = (struct __pyx_vtabstruct_5dimod_11cyvariables_cyVariables*)__Pyx_GetVtable(__pyx_ptype_5dimod_11cyvariables_cyVariables->tp_dict); if (unlikely(!__pyx_vtabptr_5dimod_11cyvariables_cyVariables)) __PYX_ERR(4, 20, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
```

### Comparing `dwave-samplers-1.0.0.dev2/dwave/samplers/tree/utilities.pyx` & `dwave-samplers-1.1.0/dwave/samplers/tree/utilities.pyx`

 * *Files identical despite different names*

### Comparing `dwave-samplers-1.0.0.dev2/dwave_samplers.egg-info/PKG-INFO` & `dwave-samplers-1.1.0/dwave_samplers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: dwave-samplers
-Version: 1.0.0.dev2
+Version: 1.1.0
 Summary: Ocean-compatible collection of solvers/samplers
 Home-page: https://github.com/dwavesystems/dwave-samplers
 Author: D-Wave Systems Inc.
 Author-email: tools@dwavesys.com
 License: Apache 2.0
 Project-URL: Documentation, https://docs.ocean.dwavesys.com/en/stable/docs_greedy/sdk_index.html
 Project-URL: Issue Tracker, https://github.com/dwavesystems/dwave-samplers/issues/
 Project-URL: Source Code, https://github.com/dwavesystems/dwave-samplers/
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 .. image:: https://img.shields.io/pypi/v/dwave-samplers.svg
     :target: https://pypi.python.org/pypi/dwave-samplers
@@ -47,16 +49,16 @@
 that run either remotely (for example, in D-Wave's
 `Leap <https://cloud.dwavesys.com/leap/>`_ environment) or locally on your CPU.
 
 *dwave-samplers* implements the following classical algorithms for solving
 `binary quadratic models <https://docs.ocean.dwavesys.com/en/stable/concepts/bqm.html>`_
 (BQM):
 
-* Planar: an exact solver for planar Ising problems with no linear biases.
-* Random: a sampler that draws uniform random samples.
+* `Planar`_: an exact solver for planar Ising problems with no linear biases.
+* `Random`_: a sampler that draws uniform random samples.
 * `Simulated Annealing`_: a probabilistic heuristic for optimization and approximate
   Boltzmann sampling well suited to finding good solutions of large problems.
 * `Steepest Descent`_: a discrete analogue of gradient descent, often used in
   machine learning, that quickly finds a local minimum.
 * `Tabu`_: a heuristic that employs local search with methods to escape local minima.
 * `Tree Decomposition`_: an exact solver for problems with low treewidth.
 
@@ -97,15 +99,15 @@
 
 >>> sampleset = sampler.sample(bqm, time_limit=.1, max_num_samples=5)
 >>> num_reads = sampleset.info['num_reads']  # the total number of samples generated
 
 Simulated Annealing
 ===================
 
-`Simulated annealing <https://en.wikipedia.org/wiki/Simulated_annealing>`_ can be
+`Simulated annealing <https://en.wikipedia.org/wiki/Simulated_annealing>`__ can be
 used for heuristic optimization or approximate Boltzmann sampling. The
 *dwave-samplers* implementation approaches the equilibrium distribution by
 performing updates at a sequence of decreasing temperatures, terminating at the
 target `β`.\ [#]_ Each spin is updated once in a fixed order per point
 per temperature according to a Metropolis-Hastings update. When the temperature
 is low the target distribution concentrates, at equilibrium, over ground states
 of the model. Samples are guaranteed to match the equilibrium for long, smooth
@@ -129,15 +131,15 @@
 
 >>> sampleset = sampler.sample(bqm)
 >>> sampleset = sampler.sample(bqm, beta_range=[.1, 4.2], beta_schedule_type='linear')
 
 Steepest Descent
 ================
 
-`Steepest descent <https://en.wikipedia.org/wiki/Gradient_descent>`_ is the
+`Steepest descent <https://en.wikipedia.org/wiki/Gradient_descent>`__ is the
 discrete analogue of gradient descent, but the best move is computed using a local
 minimization rather rather than computing a gradient. The dimension along which
 to descend is determined, at each step, by the variable flip that causes the
 greatest reduction in energy.
 
 Steepest descent is fast and effective for unfrustrated problems, but it can get
 stuck in local minima.
@@ -171,15 +173,15 @@
    x  y energy num_oc. num_st.
 0  0  0    0.0       1       0
 ['BINARY', 1 rows, 1 samples, 2 variables]
 
 Tabu
 ====
 
-`Tabu search <https://en.wikipedia.org/wiki/Tabu_search>`_ is a heuristic that
+`Tabu search <https://en.wikipedia.org/wiki/Tabu_search>`__ is a heuristic that
 employs local search and can escape local minima by maintaining a "tabu list" of
 recently explored states that it does not revisit. The length of this tabu list
 is called the "tenure". *dwave-samplers* implementats the
 `MST2 multistart tabu search algorithm <https://link.springer.com/article/10.1023/B:ANOR.0000039522.58036.68>`_
 for quadratic unconstrained binary optimization (QUBO) problems.
 
 Each read of the tabu algorithm consists of many starts. The solver takes the best
@@ -198,15 +200,15 @@
 
 >>> sampleset0 = sampler.sample(qubo)
 >>> sampleset1 = sampler.sample(qubo, tenure=1, num_restarts=1)
 
 Tree Decomposition
 ==================
 
-`Tree decomposition <https://en.wikipedia.org/wiki/Tree_decomposition>`_-based
+`Tree decomposition <https://en.wikipedia.org/wiki/Tree_decomposition>`__-based
 solvers have a runtime that is exponential in the
 `treewidth <https://en.wikipedia.org/wiki/Treewidth>`_ of the problem graph. For
 problems with low treewidth, the solver can find ground states very quickly.
 However, for even moderately dense problems, performance is very poor.
 
 >>> from dwave.samplers import TreeDecompositionSolver
 >>> solver = TreeDecompositionSolver()
@@ -263,7 +265,9 @@
 .. code-block:: bash
 
     reno new your-short-descriptor-here
 
 You can then edit the file created under ``releasenotes/notes/``.
 Remove any sections not relevant to your changes.
 Commit the file along with your changes.
+
+
```

### Comparing `dwave-samplers-1.0.0.dev2/dwave_samplers.egg-info/SOURCES.txt` & `dwave-samplers-1.1.0/dwave_samplers.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 MANIFEST.in
 README.rst
 pyproject.toml
 setup.cfg
 setup.py
+dwave/__init__.py
 dwave/samplers/__init__.py
 dwave/samplers/greedy/__init__.py
 dwave/samplers/greedy/composite.py
 dwave/samplers/greedy/decl.pxd
 dwave/samplers/greedy/descent.cpp
 dwave/samplers/greedy/descent.pyx
 dwave/samplers/greedy/sampler.py
```

### Comparing `dwave-samplers-1.0.0.dev2/setup.cfg` & `dwave-samplers-1.1.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -19,30 +19,32 @@
 	Development Status :: 4 - Beta
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: Implementation :: CPython
 
 [options]
 packages = 
+	dwave
 	dwave.samplers
 	dwave.samplers.greedy
 	dwave.samplers.planar
 	dwave.samplers.random
 	dwave.samplers.sa
 	dwave.samplers.tabu
 	dwave.samplers.tree
 zip_safe = false
 include_package_data = true
 python_requires = >=3.7
 install_requires = 
-	numpy>=1.20.0,<2.0.0
+	numpy>=1.19.0,<2.0.0
 	dimod>=0.12.0,<0.13.0
 	networkx>=2.4.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `dwave-samplers-1.0.0.dev2/setup.py` & `dwave-samplers-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,21 +20,21 @@
 import numpy
 
 
 class build_ext_with_args(build_ext):
     """Add compiler-specific compile/link flags."""
 
     extra_compile_args = {
-        'msvc': ['/std:c++14'],
-        'unix': ['-std=c++11'],
+        'msvc': ['/std:c++17'],
+        'unix': ['-std=c++17'],
     }
 
     extra_link_args = {
         'msvc': [],
-        'unix': ['-std=c++11'],
+        'unix': ['-std=c++17'],
     }
 
     def build_extensions(self):
         compiler = self.compiler.compiler_type
 
         compile_args = self.extra_compile_args[compiler]
         for ext in self.extensions:
```

