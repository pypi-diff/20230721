# Comparing `tmp/stardist-0.8.4.tar.gz` & `tmp/stardist-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stardist-0.8.4.tar", last modified: Tue Jul 18 23:39:21 2023, max compression
+gzip compressed data, was "stardist-0.8.5.tar", last modified: Fri Jul 21 14:51:55 2023, max compression
```

## Comparing `stardist-0.8.4.tar` & `stardist-0.8.5.tar`

### file list

```diff
@@ -1,158 +1,147 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:39:21.224069 stardist-0.8.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-18 23:39:10.000000 stardist-0.8.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-18 23:39:10.000000 stardist-0.8.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    20462 2023-07-18 23:39:21.224069 stardist-0.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19486 2023-07-18 23:39:10.000000 stardist-0.8.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-18 23:39:11.000000 stardist-0.8.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-18 23:39:21.224069 stardist-0.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5657 2023-07-18 23:39:11.000000 stardist-0.8.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:39:21.208069 stardist-0.8.4/stardist/
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24004 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/big.py
--rw-r--r--   0 runner    (1001) docker     (123)    19488 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/bioimageio_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:39:21.208069 stardist-0.8.4/stardist/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:39:21.208069 stardist-0.8.4/stardist/data/images/
--rw-r--r--   0 runner    (1001) docker     (123)    35505 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/data/images/histo.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   524544 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/data/images/img2d.tif
--rw-r--r--   0 runner    (1001) docker     (123)   138925 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/data/images/img3d.tif
--rw-r--r--   0 runner    (1001) docker     (123)   524544 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/data/images/mask2d.tif
--rw-r--r--   0 runner    (1001) docker     (123)    15419 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/data/images/mask3d.tif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:39:21.212069 stardist-0.8.4/stardist/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/geometry/geom2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    12542 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/geometry/geom3d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:39:21.212069 stardist-0.8.4/stardist/kernels/
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/kernels/stardist2d.cl
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/kernels/stardist3d.cl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:39:21.212069 stardist-0.8.4/stardist/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:39:21.204069 stardist-0.8.4/stardist/lib/external/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:39:21.212069 stardist-0.8.4/stardist/lib/external/clipper/
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/clipper/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)   142184 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/clipper/clipper.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    15423 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/clipper/clipper.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:39:21.212069 stardist-0.8.4/stardist/lib/external/nanoflann/
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/nanoflann/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    73558 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/nanoflann/nanoflann.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:39:21.212069 stardist-0.8.4/stardist/lib/external/qhull_src/
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/Announce.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/COPYING.txt
--rw-r--r--   0 runner    (1001) docker     (123)    21849 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:39:21.204069 stardist-0.8.4/stardist/lib/external/qhull_src/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:39:21.216069 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhull_r/
--rw-r--r--   0 runner    (1001) docker     (123)    73854 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhull_r/geom2_r.c
--rw-r--r--   0 runner    (1001) docker     (123)    45785 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhull_r/geom_r.c
--rw-r--r--   0 runner    (1001) docker     (123)     8149 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhull_r/geom_r.h
--rw-r--r--   0 runner    (1001) docker     (123)    75784 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhull_r/global_r.c
--rw-r--r--   0 runner    (1001) docker     (123)   140430 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhull_r/io_r.c
--rw-r--r--   0 runner    (1001) docker     (123)     8707 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhull_r/io_r.h
--rw-r--r--   0 runner    (1001) docker     (123)    66346 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhull_r/libqhull_r.c
--rw-r--r--   0 runner    (1001) docker     (123)    56702 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhull_r/libqhull_r.h
--rw-r--r--   0 runner    (1001) docker     (123)    21438 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhull_r/mem_r.c
--rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhull_r/mem_r.h
--rw-r--r--   0 runner    (1001) docker     (123)   208318 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhull_r/merge_r.c
--rw-r--r--   0 runner    (1001) docker     (123)    12247 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhull_r/merge_r.h
--rw-r--r--   0 runner    (1001) docker     (123)   145471 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhull_r/poly2_r.c
--rw-r--r--   0 runner    (1001) docker     (123)    47472 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhull_r/poly_r.c
--rw-r--r--   0 runner    (1001) docker     (123)    12127 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhull_r/poly_r.h
--rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhull_r/qhull_ra.h
--rw-r--r--   0 runner    (1001) docker     (123)    34690 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhull_r/qset_r.c
--rw-r--r--   0 runner    (1001) docker     (123)    15528 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhull_r/qset_r.h
--rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhull_r/random_r.c
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhull_r/random_r.h
--rw-r--r--   0 runner    (1001) docker     (123)    25609 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhull_r/rboxlib_r.c
--rw-r--r--   0 runner    (1001) docker     (123)    30324 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhull_r/stat_r.c
--rw-r--r--   0 runner    (1001) docker     (123)    12533 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhull_r/stat_r.h
--rw-r--r--   0 runner    (1001) docker     (123)    20848 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhull_r/user_r.c
--rw-r--r--   0 runner    (1001) docker     (123)    33496 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhull_r/user_r.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:39:21.220069 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/Coordinates.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    15929 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/Coordinates.h
--rw-r--r--   0 runner    (1001) docker     (123)     9577 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/PointCoordinates.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8049 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/PointCoordinates.h
--rw-r--r--   0 runner    (1001) docker     (123)    12043 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/Qhull.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6540 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/Qhull.h
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/QhullError.h
--rw-r--r--   0 runner    (1001) docker     (123)    15508 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacet.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacet.h
--rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetList.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetList.h
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetSet.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetSet.h
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/QhullHyperplane.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/QhullHyperplane.h
--rw-r--r--   0 runner    (1001) docker     (123)     8054 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/QhullIterator.h
--rw-r--r--   0 runner    (1001) docker     (123)    12637 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/QhullLinkedList.h
--rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoint.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7707 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoint.h
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPointSet.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPointSet.h
--rw-r--r--   0 runner    (1001) docker     (123)     7186 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoints.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    18839 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoints.h
--rw-r--r--   0 runner    (1001) docker     (123)     6626 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/QhullQh.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/QhullQh.h
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/QhullRidge.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/QhullRidge.h
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/QhullSet.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    19140 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/QhullSet.h
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/QhullSets.h
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/QhullStat.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/QhullStat.h
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertex.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertex.h
--rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertexSet.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertexSet.h
--rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/RboxPoints.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/RboxPoints.h
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/RoadError.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/RoadError.h
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/RoadLogEvent.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/RoadLogEvent.h
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/functionObjects.h
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/usermem_r-cpp.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    19957 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/stardist2d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    12832 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/stardist3d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    47157 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/stardist3d_impl.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/stardist3d_impl.h
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/stardist3d_lib.c
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/stardist3d_lib.h
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/test_lib3d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/utils.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/lib/utils.h
--rw-r--r--   0 runner    (1001) docker     (123)    19434 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/matching.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:39:21.220069 stardist-0.8.4/stardist/models/
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55742 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    27280 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/models/model2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    32215 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/models/model3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    12632 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/nms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:39:21.220069 stardist-0.8.4/stardist/plot/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/plot/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/plot/render.py
--rw-r--r--   0 runner    (1001) docker     (123)    11608 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/rays3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/sample_patches.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:39:21.220069 stardist-0.8.4/stardist/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/scripts/predict2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/scripts/predict3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    15240 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-18 23:39:11.000000 stardist-0.8.4/stardist/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:39:21.208069 stardist-0.8.4/stardist.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20462 2023-07-18 23:39:21.000000 stardist-0.8.4/stardist.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9436 2023-07-18 23:39:21.000000 stardist-0.8.4/stardist.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 23:39:21.000000 stardist-0.8.4/stardist.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-18 23:39:21.000000 stardist-0.8.4/stardist.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-18 23:39:21.000000 stardist-0.8.4/stardist.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-18 23:39:21.000000 stardist-0.8.4/stardist.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:39:21.224069 stardist-0.8.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8101 2023-07-18 23:39:11.000000 stardist-0.8.4/tests/test_big.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-07-18 23:39:11.000000 stardist-0.8.4/tests/test_bioimageio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-07-18 23:39:11.000000 stardist-0.8.4/tests/test_matching.py
--rw-r--r--   0 runner    (1001) docker     (123)    18846 2023-07-18 23:39:11.000000 stardist-0.8.4/tests/test_model2D.py
--rw-r--r--   0 runner    (1001) docker     (123)    13679 2023-07-18 23:39:11.000000 stardist-0.8.4/tests/test_model3D.py
--rw-r--r--   0 runner    (1001) docker     (123)     7863 2023-07-18 23:39:11.000000 stardist-0.8.4/tests/test_nms2D.py
--rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-07-18 23:39:11.000000 stardist-0.8.4/tests/test_nms3D.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-07-18 23:39:11.000000 stardist-0.8.4/tests/test_stardist2D.py
--rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-07-18 23:39:11.000000 stardist-0.8.4/tests/test_stardist3D.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-18 23:39:11.000000 stardist-0.8.4/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:51:55.934452 stardist-0.8.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-21 14:51:44.000000 stardist-0.8.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-21 14:51:44.000000 stardist-0.8.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    20462 2023-07-21 14:51:55.934452 stardist-0.8.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19486 2023-07-21 14:51:44.000000 stardist-0.8.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-21 14:51:44.000000 stardist-0.8.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-21 14:51:55.934452 stardist-0.8.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5978 2023-07-21 14:51:44.000000 stardist-0.8.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:51:55.918451 stardist-0.8.5/stardist/
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24004 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/big.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19488 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/bioimageio_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:51:55.918451 stardist-0.8.5/stardist/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:51:55.922452 stardist-0.8.5/stardist/data/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    35505 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/data/images/histo.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   524544 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/data/images/img2d.tif
+-rw-r--r--   0 runner    (1001) docker     (123)   138925 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/data/images/img3d.tif
+-rw-r--r--   0 runner    (1001) docker     (123)   524544 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/data/images/mask2d.tif
+-rw-r--r--   0 runner    (1001) docker     (123)    15419 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/data/images/mask3d.tif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:51:55.922452 stardist-0.8.5/stardist/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/geometry/geom2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12542 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/geometry/geom3d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:51:55.922452 stardist-0.8.5/stardist/kernels/
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/kernels/stardist2d.cl
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/kernels/stardist3d.cl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:51:55.922452 stardist-0.8.5/stardist/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:51:55.914451 stardist-0.8.5/stardist/lib/external/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:51:55.922452 stardist-0.8.5/stardist/lib/external/clipper/
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/clipper/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   142184 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/clipper/clipper.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15423 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/clipper/clipper.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:51:55.922452 stardist-0.8.5/stardist/lib/external/nanoflann/
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/nanoflann/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    73558 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/nanoflann/nanoflann.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:51:55.922452 stardist-0.8.5/stardist/lib/external/qhull_src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/Announce.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/COPYING.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    21849 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:51:55.918451 stardist-0.8.5/stardist/lib/external/qhull_src/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:51:55.926452 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/
+-rw-r--r--   0 runner    (1001) docker     (123)    73854 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/geom2_r.c
+-rw-r--r--   0 runner    (1001) docker     (123)    45785 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/geom_r.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8149 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/geom_r.h
+-rw-r--r--   0 runner    (1001) docker     (123)    75784 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/global_r.c
+-rw-r--r--   0 runner    (1001) docker     (123)   140430 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/io_r.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8707 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/io_r.h
+-rw-r--r--   0 runner    (1001) docker     (123)    66346 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/libqhull_r.c
+-rw-r--r--   0 runner    (1001) docker     (123)    56702 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/libqhull_r.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21438 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/mem_r.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/mem_r.h
+-rw-r--r--   0 runner    (1001) docker     (123)   208318 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/merge_r.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12247 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/merge_r.h
+-rw-r--r--   0 runner    (1001) docker     (123)   145471 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/poly2_r.c
+-rw-r--r--   0 runner    (1001) docker     (123)    47472 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/poly_r.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12127 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/poly_r.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/qhull_ra.h
+-rw-r--r--   0 runner    (1001) docker     (123)    34690 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/qset_r.c
+-rw-r--r--   0 runner    (1001) docker     (123)    15528 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/qset_r.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/random_r.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/random_r.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25609 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/rboxlib_r.c
+-rw-r--r--   0 runner    (1001) docker     (123)    30324 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/stat_r.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12533 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/stat_r.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20848 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/user_r.c
+-rw-r--r--   0 runner    (1001) docker     (123)    33496 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/user_r.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:51:55.934452 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/Coordinates.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15929 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/Coordinates.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9577 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/PointCoordinates.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8049 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/PointCoordinates.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12043 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/Qhull.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6540 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/Qhull.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullError.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15508 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacet.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacet.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetList.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetList.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetSet.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetSet.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullHyperplane.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullHyperplane.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8054 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullIterator.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12637 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullLinkedList.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoint.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7707 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoint.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPointSet.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPointSet.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7186 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoints.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    18839 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoints.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6626 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullQh.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullQh.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullRidge.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullRidge.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullSet.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    19140 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullSet.h
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullSets.h
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullStat.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullStat.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertex.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertexSet.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertexSet.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/RboxPoints.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/RboxPoints.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/RoadError.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/RoadError.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/RoadLogEvent.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/RoadLogEvent.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/functionObjects.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/usermem_r-cpp.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    19957 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/stardist2d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12832 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/stardist3d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    47157 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/stardist3d_impl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/stardist3d_impl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/stardist3d_lib.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/stardist3d_lib.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/test_lib3d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19434 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/matching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:51:55.934452 stardist-0.8.5/stardist/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55742 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27280 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/models/model2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32215 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/models/model3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12632 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/nms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:51:55.934452 stardist-0.8.5/stardist/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/plot/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/plot/render.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11608 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/rays3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/sample_patches.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:51:55.934452 stardist-0.8.5/stardist/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/scripts/predict2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/scripts/predict3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15240 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:51:55.918451 stardist-0.8.5/stardist.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20462 2023-07-21 14:51:55.000000 stardist-0.8.5/stardist.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5838 2023-07-21 14:51:55.000000 stardist-0.8.5/stardist.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 14:51:55.000000 stardist-0.8.5/stardist.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-21 14:51:55.000000 stardist-0.8.5/stardist.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-21 14:51:55.000000 stardist-0.8.5/stardist.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 14:51:55.000000 stardist-0.8.5/stardist.egg-info/top_level.txt
```

### Comparing `stardist-0.8.4/LICENSE.txt` & `stardist-0.8.5/LICENSE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2018-2022, Uwe Schmidt, Martin Weigert
+Copyright (c) 2018-2023, Uwe Schmidt, Martin Weigert
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

### Comparing `stardist-0.8.4/PKG-INFO` & `stardist-0.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stardist
-Version: 0.8.4
+Version: 0.8.5
 Summary: StarDist - Object Detection with Star-convex Shapes
 Home-page: https://github.com/stardist/stardist
 Author: Uwe Schmidt, Martin Weigert
 Author-email: research@uweschmidt.org, martin.weigert@epfl.ch
 License: BSD-3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `stardist-0.8.4/README.md` & `stardist-0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/setup.py` & `stardist-0.8.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,17 +51,22 @@
         ext.extra_compile_args = _extra_compile_args
         ext.extra_link_args    = _extra_link_args
         return super(build_ext_openmp, self).build_extension(ext)
 
 
 #------------------------------------------------------------------------------------
 
+# https://stackoverflow.com/a/22866630
+# python setup.py sdist                    ->  __file__ is relative path
+# python /absolute/path/to/setup.py sdist  ->  __file__ is absolute path
+# python -m build --sdist                  ->  __file__ is absolute path
 
 # cf. https://github.com/mkleehammer/pyodbc/issues/82#issuecomment-231561240
-_dir = path.dirname(__file__)
+# _dir = path.dirname(__file__)
+_dir = '' #  assumption: Path(__file__).parent == Path.cwd()
 
 with open(path.join(_dir,'stardist','version.py'), encoding="utf-8") as f:
     exec(f.read())
 
 with open(path.join(_dir,'README.md'), encoding="utf-8") as f:
     long_description = f.read()
```

### Comparing `stardist-0.8.4/stardist/__init__.py` & `stardist-0.8.5/stardist/__init__.py`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/big.py` & `stardist-0.8.5/stardist/big.py`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/bioimageio_utils.py` & `stardist-0.8.5/stardist/bioimageio_utils.py`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/data/__init__.py` & `stardist-0.8.5/stardist/data/__init__.py`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/data/images/histo.jpg` & `stardist-0.8.5/stardist/data/images/histo.jpg`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/data/images/img2d.tif` & `stardist-0.8.5/stardist/data/images/img2d.tif`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/data/images/img3d.tif` & `stardist-0.8.5/stardist/data/images/img3d.tif`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/data/images/mask2d.tif` & `stardist-0.8.5/stardist/data/images/mask2d.tif`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/data/images/mask3d.tif` & `stardist-0.8.5/stardist/data/images/mask3d.tif`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/geometry/geom2d.py` & `stardist-0.8.5/stardist/geometry/geom2d.py`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/geometry/geom3d.py` & `stardist-0.8.5/stardist/geometry/geom3d.py`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/kernels/stardist2d.cl` & `stardist-0.8.5/stardist/kernels/stardist2d.cl`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/kernels/stardist3d.cl` & `stardist-0.8.5/stardist/kernels/stardist3d.cl`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/clipper/LICENSE.txt` & `stardist-0.8.5/stardist/lib/external/clipper/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/clipper/clipper.cpp` & `stardist-0.8.5/stardist/lib/external/clipper/clipper.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/clipper/clipper.hpp` & `stardist-0.8.5/stardist/lib/external/clipper/clipper.hpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/nanoflann/LICENSE.txt` & `stardist-0.8.5/stardist/lib/external/nanoflann/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/nanoflann/nanoflann.hpp` & `stardist-0.8.5/stardist/lib/external/nanoflann/nanoflann.hpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/Announce.txt` & `stardist-0.8.5/stardist/lib/external/qhull_src/Announce.txt`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/COPYING.txt` & `stardist-0.8.5/stardist/lib/external/qhull_src/COPYING.txt`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/README.txt` & `stardist-0.8.5/stardist/lib/external/qhull_src/README.txt`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhull_r/geom2_r.c` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/geom2_r.c`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhull_r/geom_r.c` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/geom_r.c`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhull_r/geom_r.h` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/geom_r.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhull_r/global_r.c` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/global_r.c`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhull_r/io_r.c` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/io_r.c`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhull_r/io_r.h` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/io_r.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhull_r/libqhull_r.c` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/libqhull_r.c`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhull_r/libqhull_r.h` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/libqhull_r.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhull_r/mem_r.c` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/mem_r.c`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhull_r/mem_r.h` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/mem_r.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhull_r/merge_r.c` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/merge_r.c`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhull_r/merge_r.h` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/merge_r.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhull_r/poly2_r.c` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/poly2_r.c`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhull_r/poly_r.c` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/poly_r.c`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhull_r/poly_r.h` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/poly_r.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhull_r/qhull_ra.h` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/qhull_ra.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhull_r/qset_r.c` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/qset_r.c`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhull_r/qset_r.h` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/qset_r.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhull_r/random_r.c` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/random_r.c`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhull_r/random_r.h` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/random_r.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhull_r/rboxlib_r.c` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/rboxlib_r.c`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhull_r/stat_r.c` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/stat_r.c`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhull_r/stat_r.h` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/stat_r.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhull_r/user_r.c` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/user_r.c`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhull_r/user_r.h` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/user_r.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/Coordinates.cpp` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/Coordinates.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/Coordinates.h` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/Coordinates.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/PointCoordinates.cpp` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/PointCoordinates.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/PointCoordinates.h` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/PointCoordinates.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/Qhull.cpp` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/Qhull.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/Qhull.h` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/Qhull.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/QhullError.h` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullError.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacet.cpp` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacet.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacet.h` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacet.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetList.cpp` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetList.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetList.h` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetList.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetSet.cpp` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetSet.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetSet.h` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetSet.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/QhullHyperplane.cpp` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullHyperplane.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/QhullHyperplane.h` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullHyperplane.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/QhullIterator.h` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullIterator.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/QhullLinkedList.h` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullLinkedList.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoint.cpp` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoint.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoint.h` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoint.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPointSet.cpp` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPointSet.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPointSet.h` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPointSet.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoints.cpp` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoints.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoints.h` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoints.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/QhullQh.cpp` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullQh.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/QhullQh.h` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullQh.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/QhullRidge.cpp` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullRidge.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/QhullRidge.h` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullRidge.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/QhullSet.cpp` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullSet.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/QhullSet.h` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullSet.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/QhullSets.h` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullSets.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/QhullStat.cpp` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullStat.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/QhullStat.h` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullStat.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertex.cpp` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertex.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertex.h` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertex.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertexSet.cpp` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertexSet.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertexSet.h` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertexSet.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/RboxPoints.cpp` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/RboxPoints.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/RboxPoints.h` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/RboxPoints.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/RoadError.cpp` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/RoadError.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/RoadError.h` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/RoadError.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/RoadLogEvent.cpp` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/RoadLogEvent.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/RoadLogEvent.h` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/RoadLogEvent.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/functionObjects.h` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/functionObjects.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/external/qhull_src/src/libqhullcpp/usermem_r-cpp.cpp` & `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/usermem_r-cpp.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/stardist2d.cpp` & `stardist-0.8.5/stardist/lib/stardist2d.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/stardist3d.cpp` & `stardist-0.8.5/stardist/lib/stardist3d.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/stardist3d_impl.cpp` & `stardist-0.8.5/stardist/lib/stardist3d_impl.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/stardist3d_impl.h` & `stardist-0.8.5/stardist/lib/stardist3d_impl.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/stardist3d_lib.c` & `stardist-0.8.5/stardist/lib/stardist3d_lib.c`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/stardist3d_lib.h` & `stardist-0.8.5/stardist/lib/stardist3d_lib.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/test_lib3d.cpp` & `stardist-0.8.5/stardist/lib/test_lib3d.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/lib/utils.cpp` & `stardist-0.8.5/stardist/lib/utils.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/matching.py` & `stardist-0.8.5/stardist/matching.py`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/models/__init__.py` & `stardist-0.8.5/stardist/models/__init__.py`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/models/base.py` & `stardist-0.8.5/stardist/models/base.py`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/models/model2d.py` & `stardist-0.8.5/stardist/models/model2d.py`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/models/model3d.py` & `stardist-0.8.5/stardist/models/model3d.py`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/nms.py` & `stardist-0.8.5/stardist/nms.py`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/plot/plot.py` & `stardist-0.8.5/stardist/plot/plot.py`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/plot/render.py` & `stardist-0.8.5/stardist/plot/render.py`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/rays3d.py` & `stardist-0.8.5/stardist/rays3d.py`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/sample_patches.py` & `stardist-0.8.5/stardist/sample_patches.py`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/scripts/predict2d.py` & `stardist-0.8.5/stardist/scripts/predict2d.py`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/scripts/predict3d.py` & `stardist-0.8.5/stardist/scripts/predict3d.py`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist/utils.py` & `stardist-0.8.5/stardist/utils.py`

 * *Files identical despite different names*

### Comparing `stardist-0.8.4/stardist.egg-info/PKG-INFO` & `stardist-0.8.5/stardist.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stardist
-Version: 0.8.4
+Version: 0.8.5
 Summary: StarDist - Object Detection with Star-convex Shapes
 Home-page: https://github.com/stardist/stardist
 Author: Uwe Schmidt, Martin Weigert
 Author-email: research@uweschmidt.org, martin.weigert@epfl.ch
 License: BSD-3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

