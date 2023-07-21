# Comparing `tmp/gustaf-0.0.8.tar.gz` & `tmp/gustaf-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gustaf-0.0.8.tar", last modified: Sun Feb 12 04:39:29 2023, max compression
+gzip compressed data, was "gustaf-0.0.9.tar", last modified: Fri Apr 14 12:44:25 2023, max compression
```

## Comparing `gustaf-0.0.8.tar` & `gustaf-0.0.9.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 04:39:29.543978 gustaf-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-02-12 04:39:21.000000 gustaf-0.0.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-02-12 04:39:29.543978 gustaf-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-02-12 04:39:21.000000 gustaf-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 04:39:29.539978 gustaf-0.0.8/gustaf/
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-02-12 04:39:21.000000 gustaf-0.0.8/gustaf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-02-12 04:39:21.000000 gustaf-0.0.8/gustaf/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-02-12 04:39:21.000000 gustaf-0.0.8/gustaf/_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-02-12 04:39:21.000000 gustaf-0.0.8/gustaf/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 04:39:29.539978 gustaf-0.0.8/gustaf/create/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-02-12 04:39:21.000000 gustaf-0.0.8/gustaf/create/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-02-12 04:39:21.000000 gustaf-0.0.8/gustaf/create/edges.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-02-12 04:39:21.000000 gustaf-0.0.8/gustaf/create/faces.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-02-12 04:39:21.000000 gustaf-0.0.8/gustaf/create/vertices.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-02-12 04:39:21.000000 gustaf-0.0.8/gustaf/create/volumes.py
--rw-r--r--   0 runner    (1001) docker     (123)    12402 2023-02-12 04:39:21.000000 gustaf-0.0.8/gustaf/edges.py
--rw-r--r--   0 runner    (1001) docker     (123)     7555 2023-02-12 04:39:21.000000 gustaf-0.0.8/gustaf/faces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 04:39:29.543978 gustaf-0.0.8/gustaf/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-02-12 04:39:21.000000 gustaf-0.0.8/gustaf/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27090 2023-02-12 04:39:21.000000 gustaf-0.0.8/gustaf/helpers/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    11033 2023-02-12 04:39:21.000000 gustaf-0.0.8/gustaf/helpers/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-02-12 04:39:21.000000 gustaf-0.0.8/gustaf/helpers/raise_if.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 04:39:29.543978 gustaf-0.0.8/gustaf/io/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-02-12 04:39:21.000000 gustaf-0.0.8/gustaf/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-02-12 04:39:21.000000 gustaf-0.0.8/gustaf/io/default.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-02-12 04:39:21.000000 gustaf-0.0.8/gustaf/io/ioutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-02-12 04:39:21.000000 gustaf-0.0.8/gustaf/io/meshio.py
--rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-02-12 04:39:21.000000 gustaf-0.0.8/gustaf/io/mfem.py
--rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-02-12 04:39:21.000000 gustaf-0.0.8/gustaf/io/mixd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-02-12 04:39:21.000000 gustaf-0.0.8/gustaf/io/nutils.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-02-12 04:39:21.000000 gustaf-0.0.8/gustaf/meshmaker.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-02-12 04:39:21.000000 gustaf-0.0.8/gustaf/segment.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-02-12 04:39:21.000000 gustaf-0.0.8/gustaf/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    16945 2023-02-12 04:39:21.000000 gustaf-0.0.8/gustaf/show.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 04:39:29.543978 gustaf-0.0.8/gustaf/spline/
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-02-12 04:39:21.000000 gustaf-0.0.8/gustaf/spline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14702 2023-02-12 04:39:21.000000 gustaf-0.0.8/gustaf/spline/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    22121 2023-02-12 04:39:21.000000 gustaf-0.0.8/gustaf/spline/create.py
--rw-r--r--   0 runner    (1001) docker     (123)    15912 2023-02-12 04:39:21.000000 gustaf-0.0.8/gustaf/spline/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)    16337 2023-02-12 04:39:21.000000 gustaf-0.0.8/gustaf/spline/ffd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 04:39:29.543978 gustaf-0.0.8/gustaf/spline/microstructure/
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-02-12 04:39:21.000000 gustaf-0.0.8/gustaf/spline/microstructure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20539 2023-02-12 04:39:21.000000 gustaf-0.0.8/gustaf/spline/microstructure/microstructure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 04:39:29.543978 gustaf-0.0.8/gustaf/spline/microstructure/tiles/
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-02-12 04:39:21.000000 gustaf-0.0.8/gustaf/spline/microstructure/tiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14359 2023-02-12 04:39:21.000000 gustaf-0.0.8/gustaf/spline/microstructure/tiles/crosstile2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    19824 2023-02-12 04:39:21.000000 gustaf-0.0.8/gustaf/spline/microstructure/tiles/crosstile3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    67243 2023-02-12 04:39:21.000000 gustaf-0.0.8/gustaf/spline/microstructure/tiles/inversecrosstile3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-02-12 04:39:21.000000 gustaf-0.0.8/gustaf/spline/microstructure/tiles/tilebase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-02-12 04:39:21.000000 gustaf-0.0.8/gustaf/spline/proximity.py
--rw-r--r--   0 runner    (1001) docker     (123)    10921 2023-02-12 04:39:21.000000 gustaf-0.0.8/gustaf/spline/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 04:39:29.543978 gustaf-0.0.8/gustaf/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-02-12 04:39:21.000000 gustaf-0.0.8/gustaf/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11495 2023-02-12 04:39:21.000000 gustaf-0.0.8/gustaf/utils/arr.py
--rw-r--r--   0 runner    (1001) docker     (123)    14669 2023-02-12 04:39:21.000000 gustaf-0.0.8/gustaf/utils/connec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-02-12 04:39:21.000000 gustaf-0.0.8/gustaf/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-02-12 04:39:21.000000 gustaf-0.0.8/gustaf/utils/tictoc.py
--rw-r--r--   0 runner    (1001) docker     (123)    16378 2023-02-12 04:39:21.000000 gustaf-0.0.8/gustaf/vertices.py
--rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-02-12 04:39:21.000000 gustaf-0.0.8/gustaf/volumes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 04:39:29.539978 gustaf-0.0.8/gustaf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-02-12 04:39:29.000000 gustaf-0.0.8/gustaf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-02-12 04:39:29.000000 gustaf-0.0.8/gustaf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-12 04:39:29.000000 gustaf-0.0.8/gustaf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-02-12 04:39:29.000000 gustaf-0.0.8/gustaf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-12 04:39:29.000000 gustaf-0.0.8/gustaf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-02-12 04:39:29.543978 gustaf-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-02-12 04:39:21.000000 gustaf-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 04:39:29.543978 gustaf-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-02-12 04:39:21.000000 gustaf-0.0.8/tests/test_basic_calls.py
--rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-02-12 04:39:21.000000 gustaf-0.0.8/tests/test_vertices_and_element_updates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:44:25.233850 gustaf-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-04-14 12:44:17.000000 gustaf-0.0.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-04-14 12:44:25.233850 gustaf-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-04-14 12:44:17.000000 gustaf-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:44:25.221850 gustaf-0.0.9/gustaf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-04-14 12:44:17.000000 gustaf-0.0.9/gustaf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-14 12:44:17.000000 gustaf-0.0.9/gustaf/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-14 12:44:17.000000 gustaf-0.0.9/gustaf/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-14 12:44:17.000000 gustaf-0.0.9/gustaf/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:44:25.225850 gustaf-0.0.9/gustaf/create/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-14 12:44:17.000000 gustaf-0.0.9/gustaf/create/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-04-14 12:44:17.000000 gustaf-0.0.9/gustaf/create/edges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-04-14 12:44:17.000000 gustaf-0.0.9/gustaf/create/faces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-14 12:44:17.000000 gustaf-0.0.9/gustaf/create/vertices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-14 12:44:17.000000 gustaf-0.0.9/gustaf/create/volumes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12423 2023-04-14 12:44:17.000000 gustaf-0.0.9/gustaf/edges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7556 2023-04-14 12:44:17.000000 gustaf-0.0.9/gustaf/faces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:44:25.225850 gustaf-0.0.9/gustaf/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-14 12:44:17.000000 gustaf-0.0.9/gustaf/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26641 2023-04-14 12:44:17.000000 gustaf-0.0.9/gustaf/helpers/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11045 2023-04-14 12:44:17.000000 gustaf-0.0.9/gustaf/helpers/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-04-14 12:44:17.000000 gustaf-0.0.9/gustaf/helpers/raise_if.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:44:25.225850 gustaf-0.0.9/gustaf/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-14 12:44:17.000000 gustaf-0.0.9/gustaf/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-14 12:44:17.000000 gustaf-0.0.9/gustaf/io/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-14 12:44:17.000000 gustaf-0.0.9/gustaf/io/ioutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-04-14 12:44:17.000000 gustaf-0.0.9/gustaf/io/meshio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-04-14 12:44:17.000000 gustaf-0.0.9/gustaf/io/mfem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-04-14 12:44:17.000000 gustaf-0.0.9/gustaf/io/mixd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-04-14 12:44:17.000000 gustaf-0.0.9/gustaf/io/nutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-14 12:44:17.000000 gustaf-0.0.9/gustaf/meshmaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-14 12:44:17.000000 gustaf-0.0.9/gustaf/segment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-14 12:44:17.000000 gustaf-0.0.9/gustaf/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17108 2023-04-14 12:44:17.000000 gustaf-0.0.9/gustaf/show.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:44:25.229850 gustaf-0.0.9/gustaf/spline/
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-14 12:44:17.000000 gustaf-0.0.9/gustaf/spline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14709 2023-04-14 12:44:17.000000 gustaf-0.0.9/gustaf/spline/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22139 2023-04-14 12:44:17.000000 gustaf-0.0.9/gustaf/spline/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15988 2023-04-14 12:44:17.000000 gustaf-0.0.9/gustaf/spline/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16340 2023-04-14 12:44:17.000000 gustaf-0.0.9/gustaf/spline/ffd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:44:25.229850 gustaf-0.0.9/gustaf/spline/microstructure/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-14 12:44:17.000000 gustaf-0.0.9/gustaf/spline/microstructure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20539 2023-04-14 12:44:17.000000 gustaf-0.0.9/gustaf/spline/microstructure/microstructure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:44:25.229850 gustaf-0.0.9/gustaf/spline/microstructure/tiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 12:44:17.000000 gustaf-0.0.9/gustaf/spline/microstructure/tiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14359 2023-04-14 12:44:17.000000 gustaf-0.0.9/gustaf/spline/microstructure/tiles/crosstile2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19824 2023-04-14 12:44:17.000000 gustaf-0.0.9/gustaf/spline/microstructure/tiles/crosstile3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67243 2023-04-14 12:44:17.000000 gustaf-0.0.9/gustaf/spline/microstructure/tiles/inversecrosstile3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-04-14 12:44:17.000000 gustaf-0.0.9/gustaf/spline/microstructure/tiles/tilebase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-14 12:44:17.000000 gustaf-0.0.9/gustaf/spline/proximity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10963 2023-04-14 12:44:17.000000 gustaf-0.0.9/gustaf/spline/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:44:25.233850 gustaf-0.0.9/gustaf/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-14 12:44:17.000000 gustaf-0.0.9/gustaf/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11563 2023-04-14 12:44:17.000000 gustaf-0.0.9/gustaf/utils/arr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14796 2023-04-14 12:44:17.000000 gustaf-0.0.9/gustaf/utils/connec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-04-14 12:44:17.000000 gustaf-0.0.9/gustaf/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-04-14 12:44:17.000000 gustaf-0.0.9/gustaf/utils/tictoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16409 2023-04-14 12:44:17.000000 gustaf-0.0.9/gustaf/vertices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-04-14 12:44:17.000000 gustaf-0.0.9/gustaf/volumes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:44:25.221850 gustaf-0.0.9/gustaf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-04-14 12:44:25.000000 gustaf-0.0.9/gustaf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-14 12:44:25.000000 gustaf-0.0.9/gustaf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 12:44:25.000000 gustaf-0.0.9/gustaf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-14 12:44:25.000000 gustaf-0.0.9/gustaf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-14 12:44:25.000000 gustaf-0.0.9/gustaf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-14 12:44:25.233850 gustaf-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-04-14 12:44:17.000000 gustaf-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:44:25.233850 gustaf-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-04-14 12:44:17.000000 gustaf-0.0.9/tests/test_basic_calls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-04-14 12:44:17.000000 gustaf-0.0.9/tests/test_vertices_and_element_updates.py
```

### Comparing `gustaf-0.0.8/LICENSE.txt` & `gustaf-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gustaf-0.0.8/PKG-INFO` & `gustaf-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gustaf
-Version: 0.0.8
+Version: 0.0.9
 Summary: Process and visualize numerical-analysis-geometries.
 Home-page: https://github.com/tataratat/gustaf
 Author: Jaewook Lee
 Author-email: jaewooklee042@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 Provides-Extra: all
 License-File: LICENSE.txt
 
-![gustaf](https://github.com/tataratat/gustaf/raw/gustaf/docs/source/gustaf-logo.png)
+![gustaf](https://github.com/tataratat/gustaf/raw/main/docs/source/gustaf-logo.png)
 
 __gustaf__ is a python library to process and visualize numerical-analysis-geometries; especially for Finite Element Methods (FEM) and Isogemetric Analysis (IGA).
 gustaf currently supports linear elements:
 - triangle,
 - quadrilateral,
 - tetrahedron, and
 - hexahedron,
@@ -81,16 +81,16 @@
         [7, 0, 3, 1],
     ],
 )
 tet.show()
 
 # elements can transform to their subelement types
 # set unique=True, if you don't want duplicating internal subelements
-as_faces = tet.tofaces(unique=False)
-as_edges = tet.toedges(unique=False)
+as_faces = tet.to_faces(unique=False)
+as_edges = tet.to_edges(unique=False)
 
 # as geometry classes inherit from its subelement class, we can
 # extract subelement connectivity directly.
 # Volumes' subelements are faces and subsubelements are edges
 face_connectivity = tet.faces()
 edge_connectivity = tet.edges()
 
@@ -110,18 +110,18 @@
 # there's a shortcut - single_volumes(), single_faces(), single_edges()
 assert np.allclose(
     tet.single_faces(),
     unique_face_infos.ids[unique_face_infos.counts == 1]
 )
 
 # let's visualize some scalar data and vector data defined on vertices
-tet.vertexdata["arange"] = np.arange(len(tet.vertices))  # scalar
-tet.show_options["dataname"] = "arange"
-tet.vertexdata["random"] = np.random.random((len(tet.vertices), 3))  # vector
-tet.show_options["arrowdata"] = "random"
+tet.vertex_data["arange"] = np.arange(len(tet.vertices))  # scalar
+tet.show_options["data_name"] = "arange"
+tet.vertex_data["random"] = np.random.random((len(tet.vertices), 3))  # vector
+tet.show_options["arrow_data"] = "random"
 tet.show()
 
 
 # create a 2D NURBS disc and visualize
 # all the spline types inherits from splinepy's splines and equipped with
 # additional functionalities
 nurbs = gus.NURBS(
@@ -167,19 +167,19 @@
 )
 
 # create derived spline using Creator helper class
 extruded = nurbs.create.extruded(extrusion_vector=[0, 0, 1])
 revolved = nurbs.create.revolved(axis=[1, 0, 0], angle=70)
 parametric_view = nurbs.create.parametric_view()
 
-# just like vertexdata, you can define splinedata
+# just like vertex_data, you can define spline_data
 # for more options, checkout `gus.spline.SplineDataAdaptor`
 # following will plot the norm of nurbs' physical coordinates
-nurbs.splinedata["coords"] = nurbs
-nurbs.show_options["dataname"] = "coords"
+nurbs.spline_data["coords"] = nurbs
+nurbs.show_options["data_name"] = "coords"
 
 # show them all together. each arg is plotted on a separate subplot
 # translate tet a bit to avoid overlapping
 tet.vertices += [2, 0, 0]
 gus.show(
     ["NURBS and translated tet together", nurbs, tet],
     ["Extruded NURBS", extruded],
```

### Comparing `gustaf-0.0.8/README.md` & `gustaf-0.0.9/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-![gustaf](https://github.com/tataratat/gustaf/raw/gustaf/docs/source/gustaf-logo.png)
+![gustaf](https://github.com/tataratat/gustaf/raw/main/docs/source/gustaf-logo.png)
 
 __gustaf__ is a python library to process and visualize numerical-analysis-geometries; especially for Finite Element Methods (FEM) and Isogemetric Analysis (IGA).
 gustaf currently supports linear elements:
 - triangle,
 - quadrilateral,
 - tetrahedron, and
 - hexahedron,
@@ -58,16 +58,16 @@
         [7, 0, 3, 1],
     ],
 )
 tet.show()
 
 # elements can transform to their subelement types
 # set unique=True, if you don't want duplicating internal subelements
-as_faces = tet.tofaces(unique=False)
-as_edges = tet.toedges(unique=False)
+as_faces = tet.to_faces(unique=False)
+as_edges = tet.to_edges(unique=False)
 
 # as geometry classes inherit from its subelement class, we can
 # extract subelement connectivity directly.
 # Volumes' subelements are faces and subsubelements are edges
 face_connectivity = tet.faces()
 edge_connectivity = tet.edges()
 
@@ -87,18 +87,18 @@
 # there's a shortcut - single_volumes(), single_faces(), single_edges()
 assert np.allclose(
     tet.single_faces(),
     unique_face_infos.ids[unique_face_infos.counts == 1]
 )
 
 # let's visualize some scalar data and vector data defined on vertices
-tet.vertexdata["arange"] = np.arange(len(tet.vertices))  # scalar
-tet.show_options["dataname"] = "arange"
-tet.vertexdata["random"] = np.random.random((len(tet.vertices), 3))  # vector
-tet.show_options["arrowdata"] = "random"
+tet.vertex_data["arange"] = np.arange(len(tet.vertices))  # scalar
+tet.show_options["data_name"] = "arange"
+tet.vertex_data["random"] = np.random.random((len(tet.vertices), 3))  # vector
+tet.show_options["arrow_data"] = "random"
 tet.show()
 
 
 # create a 2D NURBS disc and visualize
 # all the spline types inherits from splinepy's splines and equipped with
 # additional functionalities
 nurbs = gus.NURBS(
@@ -144,19 +144,19 @@
 )
 
 # create derived spline using Creator helper class
 extruded = nurbs.create.extruded(extrusion_vector=[0, 0, 1])
 revolved = nurbs.create.revolved(axis=[1, 0, 0], angle=70)
 parametric_view = nurbs.create.parametric_view()
 
-# just like vertexdata, you can define splinedata
+# just like vertex_data, you can define spline_data
 # for more options, checkout `gus.spline.SplineDataAdaptor`
 # following will plot the norm of nurbs' physical coordinates
-nurbs.splinedata["coords"] = nurbs
-nurbs.show_options["dataname"] = "coords"
+nurbs.spline_data["coords"] = nurbs
+nurbs.show_options["data_name"] = "coords"
 
 # show them all together. each arg is plotted on a separate subplot
 # translate tet a bit to avoid overlapping
 tet.vertices += [2, 0, 0]
 gus.show(
     ["NURBS and translated tet together", nurbs, tet],
     ["Extruded NURBS", extruded],
```

### Comparing `gustaf-0.0.8/gustaf/__init__.py` & `gustaf-0.0.9/gustaf/__init__.py`

 * *Files identical despite different names*

### Comparing `gustaf-0.0.8/gustaf/_base.py` & `gustaf-0.0.9/gustaf/_base.py`

 * *Files identical despite different names*

### Comparing `gustaf-0.0.8/gustaf/_typing.py` & `gustaf-0.0.9/gustaf/_typing.py`

 * *Files identical despite different names*

### Comparing `gustaf-0.0.8/gustaf/create/edges.py` & `gustaf-0.0.9/gustaf/create/edges.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,29 +8,29 @@
 from gustaf.edges import Edges
 
 
 def from_data(gus_obj, data, scale=None, data_norm=None):
     """
     Creates edges from gustaf object with vertices.
     Data can be either multi-dim array-like data or a str describing a name
-    of vertexdata that belongs to given gustaf object.
+    of vertex_data that belongs to given gustaf object.
     len(gus_obj.vertices) number of edges will be created, where origin and
     end of each edge is created using the following scheme:
     [[vertices[0], vertices[0] + (array_data[0] * scale)], ...].
     By default, scaling value will be
     max([1, (aabb_diagonal_norm * 0.1 / max_data_norm)]).
     If there's dimension mismatch between vertices and the data, will append
     zero paddings!
 
     Parameters
     ----------
     gus_obj: Vertices
       gus.Vertices or its derived classes
     data: str or (n_vertices, d) array-like
-     If str, will be considered as dataname and search for saved vertexdata.
+     If str, will be considered as data_name and search for saved vertex_data.
     scale: float
       Absolute value.
     data_norm: float or array-like
       If float, will be considered as max_norm of the data. Else, searches for
       max value. Doesn't enforce len to match.
 
     Returns
@@ -42,15 +42,15 @@
             "Invalid input. Expecting gus.Vertices or its subclasses"
         )
 
     # get origin and increment (= array_data * scale)
     origin = gus_obj.const_vertices
     if isinstance(data, str):
         # will raise if data doesn't exist
-        increment = gus_obj.vertexdata[data]
+        increment = gus_obj.vertex_data[data]
     elif isinstance(data, (tuple, list, np.ndarray)):
         increment = np.asanyarray(data)
         if len(increment) != len(origin):
             raise ValueError(
                 f"Data length mismatch: expected ({len(origin)}) / "
                 "given ({len(increment)})"
             )
@@ -79,15 +79,15 @@
             origin = np.hstack((origin, zero_pad))
         else:
             increment = np.hstack((increment, zero_pad))
 
     # apply default scale
     if scale is None:
         if isinstance(data, str):
-            norm = gus_obj.vertexdata.as_scalar(data, None, True)
+            norm = gus_obj.vertex_data.as_scalar(data, None, True)
         else:
             # compute
             if data_norm is None:
                 norm = np.linalg.norm(increment, axis=1)
             else:
                 norm = np.asanyarray(data_norm)
```

### Comparing `gustaf-0.0.8/gustaf/create/faces.py` & `gustaf-0.0.9/gustaf/create/faces.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,28 +35,28 @@
         raise ValueError("All resolution values must be at least 2.")
 
     if simplex:
         # create quad mesh as basis
         quad_mesh = box(bounds=bounds, resolutions=resolutions)
 
         # turn into triangles
-        face_mesh = tosimplex(quad_mesh, backslash)
+        face_mesh = to_simplex(quad_mesh, backslash)
 
     else:
         vertex_mesh = create.vertices.raster(bounds, resolutions)
         connectivity = utils.connec.make_quad_faces(resolutions)
         face_mesh = Faces(vertex_mesh.vertices, connectivity)
 
     return face_mesh
 
 
-def tosimplex(quad, backslash=False):
+def to_simplex(quad, backslash=False):
     """Given quad faces, diagonalize them to turn them into triangles.
 
-    If quad is counterclockwiese (CCW), triangle will also be CCW and
+    If quad is counterclockwise (CCW), triangle will also be CCW and
     vice versa. Will return a tri-mesh, if input is triangular.
     Default diagonalization looks like this:
 
     .. code-block::
 
         (3) *---* (2)
             |  /|
@@ -89,15 +89,15 @@
     --------
     tri: Faces
         Simplexifyed mesh.
     """
 
     if not isinstance(quad, Faces):
         raise ValueError(
-            "Input to tosimplex needs to be of type Faces, but it's "
+            "Input to to_simplex needs to be of type Faces, but it's "
             + type(quad)
         )
 
     if quad.whatami.startswith("quad"):
         # split variants
         split_slash = [[0, 1, 2], [2, 3, 0]]
         split_backslash = [[0, 1, 3], [3, 1, 2]]
```

### Comparing `gustaf-0.0.8/gustaf/create/vertices.py` & `gustaf-0.0.9/gustaf/create/volumes.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,37 @@
-"""gustaf/create/vertices.py.
-
-Routines to create vertices.
+"""gustaf/create/volumes.py
+Routines to create volumes.
 """
 
 import numpy as np
 
-from gustaf.vertices import Vertices
+from gustaf import create, utils
+from gustaf.volumes import Volumes
 
 
-def raster(
-    bounds,
-    resolutions,
-):
-    """Simple wraper of np.mgrid to extract raster points of desired bounds and
-    resolutions.
+def box(bounds=[[0.0, 0.0, 0.0], [1.0, 1.0, 1.0]], resolutions=[2, 2, 2]):
+    """Create structured hexahedron block mesh.
 
     Parameters
     -----------
-    bounds: (2, d) array-like
-      float
-    resolutions: (d,) array-like
-      int. It will be casted to int.
+    bounds: (2, 3) array
+        Minimum and maximum coordinates.
+    resolutions: (3) array
+        Vertex count in each dimension.
 
     Returns
     --------
-    raster_vertices: Vertices
+    volume_mesh: Volumes
     """
-    if len(resolutions) != len(bounds[0]) == len(bounds[1]):
-        raise ValueError("Length of resolutions and bounds should match.")
-
-    slices = list()
-    for b0, b1, r in zip(bounds[0], bounds[1], resolutions):
-        slices.append(slice(b0, b1, r * 1j))
 
-    # Organize it nicely: 2D np.ndarray with shape (prod(resolutions), dim)
-    points = np.mgrid[slices].T.reshape(-1, len(resolutions))
+    if np.array(bounds).shape != (2, 3):
+        raise ValueError("Bounds must have a dimension of (2, 3).")
+    if len(resolutions) != 3:
+        raise ValueError("Resolutions must have three entries.")
+    if not np.greater(resolutions, 1).all():
+        raise ValueError("All resolution values must be at least 2.")
+
+    vertex_mesh = create.vertices.raster(bounds, resolutions)
+    connectivity = utils.connec.make_hexa_volumes(resolutions)
+    volume_mesh = Volumes(vertex_mesh.vertices, connectivity)
 
-    return Vertices(points)
+    return volume_mesh
```

### Comparing `gustaf-0.0.8/gustaf/edges.py` & `gustaf-0.0.9/gustaf/edges.py`

 * *Files 2% similar despite different names*

```diff
@@ -246,31 +246,31 @@
         """
         elem_name = type(self).__qualname__.lower()
         self._logd(f"returning {elem_name}")
 
         return getattr(self, elem_name)
 
     @elements.setter
-    def elements(self, elems):
+    def elements(self, elements):
         """Calls corresponding connectivity setter. A short cut in FEM friendly
         term. Vertices -> vertices Edges -> edges Faces -> faces Volumes ->
         volumes.
 
         Parameters
         -----------
-        elems: (n, d) np.ndarray
+        elements: (n, d) np.ndarray
 
         Returns
         --------
         None
         """
         # naming rule in gustaf
         elem_name = type(self).__qualname__.lower()
-        self._logd(f"seting {elem_name}'s connectivity.")
-        return setattr(self, elem_name, elems)
+        self._logd(f"Setting {elem_name}'s connectivity.")
+        return setattr(self, elem_name, elements)
 
     @property
     def const_elements(self):
         """Returns non-mutable version of elements.
 
         Parameters
         -----------
@@ -394,38 +394,38 @@
         linspaces = (((distances // (spacing * 1.5)) + 1) * 3).astype(np.int32)
 
         # chop vertices!
         new_vs = []
         for v0, v1, lins in zip(v0s, v1s, linspaces):
             new_vs.append(np.linspace(v0, v1, lins))
 
-        # we need all choped vertices.
+        # we need all chopped vertices.
         # there might be duplicating vertices. you can use merge_vertices
         new_vs = np.vstack(new_vs)
         # all mid points are explicitly defined, but they aren't required
         # so, rm.
         mask = np.ones(len(new_vs), dtype=bool)
         mask[1::3] = False
         new_vs = new_vs[mask]
 
         # prepare edges
         tmp_es = utils.connec.range_to_edges((0, len(new_vs)), closed=False)
         new_es = tmp_es[::2]
 
         return Edges(vertices=new_vs, edges=new_es)
 
-    def shrink(self, ratio=0.8, map_vertexdata=True):
+    def shrink(self, ratio=0.8, map_vertex_data=True):
         """Returns shrunk elements.
 
         Parameters
         -----------
         ratio: float
           Default is 0.8
-        map_vertexdata: bool
-          Default is True. Maps all vertexdata.
+        map_vertex_data: bool
+          Default is True. Maps all vertex_data.
 
         Returns
         --------
         s_elements: Elements
           shrunk elements
         """
         elements = self.const_elements
@@ -439,27 +439,27 @@
 
         vs -= mids
         vs *= ratio
         vs += mids
 
         s_elements = type(self)(vertices=vs, elements=es)
 
-        if map_vertexdata:
+        if map_vertex_data:
             elements_flat = elements.ravel()
-            for key, value in self.vertexdata.items():
-                s_elements.vertexdata[key] = value[elements_flat]
+            for key, value in self.vertex_data.items():
+                s_elements.vertex_data[key] = value[elements_flat]
 
-            # probably wanna take visulation options too
+            # probably wanna take visualization options too
             s_elements._show_options._options = deepcopy(
                 self.show_options._options
             )
 
         return s_elements
 
-    def tovertices(self):
+    def to_vertices(self):
         """Returns Vertices obj.
 
         Parameters
         -----------
         None
 
         Returns
```

### Comparing `gustaf-0.0.8/gustaf/faces.py` & `gustaf-0.0.9/gustaf/faces.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,15 +191,15 @@
         faces
         """
         self._logd("returning faces")
         return self._faces
 
     @faces.setter
     def faces(self, fs):
-        """Faces setter. Similar to veritces, this will be a tracked array.
+        """Faces setter. Similar to vertices, this will be a tracked array.
 
         Parameters
         -----------
         fs: (n, 2) np.ndarray
 
         Returns
         --------
@@ -216,15 +216,15 @@
         if fs is not None:
             utils.arr.is_one_of_shapes(
                 fs,
                 ((-1, 3), (-1, 4)),
                 strict=True,
             )
 
-        # same, but non-writeable view of tracekd array
+        # same, but non-writeable view of tracked array
         self._const_faces = self._faces.view()
         self._const_faces.flags.writeable = False
 
     @property
     def const_faces(self):
         """Returns non-writeable view of faces.
 
@@ -294,15 +294,15 @@
 
         return unique_info.ids[unique_info.counts == 1]
 
     def update_faces(self, *args, **kwargs):
         """Alias to update_elements."""
         self.update_elements(*args, **kwargs)
 
-    def toedges(self, unique=True):
+    def to_edges(self, unique=True):
         """Returns Edges obj.
 
         Parameters
         -----------
         unique: bool
           Default is True. If True, only takes unique edges.
```

### Comparing `gustaf-0.0.8/gustaf/helpers/data.py` & `gustaf-0.0.9/gustaf/helpers/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,18 +186,14 @@
         "_helpee",
         "_saved",
     )
 
     def __init__(self, helpee):
         """Base class for any data holder. Behaves similar to dict.
 
-        Attributes
-        -----------
-        None
-
         Parameters
         -----------
         helpee: object
           GustafBase objects would probably make the most sense here.
         """
         self._helpee = helpee
         self._saved = dict()
@@ -205,18 +201,14 @@
     def __setitem__(self, key, value):
         """Raise Error to disable direct value setting.
 
         Parameters
         -----------
         key: str
         value: object
-
-        Returns
-        --------
-        None
         """
         raise NotImplementedError(
             "Sorry, you can't set items directly for "
             f"{type(self).__qualname__}"
         )
 
     def __getitem__(self, key):
@@ -250,22 +242,14 @@
         value: object
         """
         return self._saved.pop(key, default)
 
     def clear(self):
         """
         Clears saved data by reassigning new dict
-
-        Parameters
-        ----------
-        None
-
-        Returns
-        -------
-        None
         """
         self._saved = dict()
 
     def get(self, key, default_values=None):
         """Returns stored item if the key exists. Else, given default value. If
         the key exist, default value always exists, since it is initialized
         that way.
@@ -283,64 +267,50 @@
             return self._saved[key]
         else:
             return default_values
 
     def keys(self):
         """Returns keys of data holding dict.
 
-        Parameters
-        -----------
-        None
-
         Returns
         --------
         keys: dict_keys
         """
         return self._saved.keys()
 
     def values(self):
         """Returns values of data holding dict.
 
-        Parameters
-        -----------
-        None
-
         Returns
         --------
         values: dict_values
         """
         return self._saved.values()
 
     def items(self):
         """Returns items of data holding dict.
 
-        Parameters
-        -----------
-        None
-
         Returns
         --------
         values: dict_values
         """
         return self._saved.items()
 
 
 class ComputedData(DataHolder):
     _depends = None
     _inv_depends = None
 
     __slots__ = ()
 
     def __init__(self, helpee, **kwargs):
-        """Stores last computed values. Keys are expected to be the same as
-        helpee's function that computes the value.
+        """Stores last computed values.
 
-        Attributes
-        -----------
-        None
+        Keys are expected to be the same as helpee's function that computes the
+         value.
 
         Parameters
         -----------
         helpee: GustafBase
         """
         super().__init__(helpee)
 
@@ -447,34 +417,29 @@
     gustaf supports two kinds of data representation: scalar-data with cmap
     and vector-data with arrows.
     """
 
     __slots__ = ()
 
     def __init__(self, helpee):
-        """
-        Checks if helpee has vertices as attr beforehand.
+        """Checks if helpee has vertices as attr beforehand.
 
         Parameters
         ----------
         helpee: Vertices
           Vertices and its derived classes.
-
-        Returns
-        -------
-        None
         """
         if not hasattr(helpee, "vertices"):
             raise AttributeError("Helpee does not have `vertices`.")
 
         super().__init__(helpee)
 
     def _validate_len(self, value=None, raise_=True):
-        """
-        Checks if given value is a valid vertexdata based of its length.
+        """Checks if given value is a valid vertex_data based of its length.
+
         If raise_, throws error, else, deletes all incompatible values.
         Only checks len(). If array has (1, len) shape, this will still return
         False.
 
         Parameters
         ----------
         value: array-like
@@ -521,15 +486,15 @@
                 self._saved.pop(key)
                 self._saved.pop(key + "__norm", None)
 
         return valid
 
     def __setitem__(self, key, value):
         """
-        Performs len() based check before stroing vertexdata.
+        Performs len() based check before storing vertex_data.
 
         Parameters
         ----------
         key: str
         value: object
 
         Returns
@@ -581,36 +546,36 @@
         """
         if key not in self.keys():
             return default
 
         # interpret scalar as norm
         # save the norm once it is called.
         if "__norm" not in key:
-            normkey = key + "__norm"
+            norm_key = key + "__norm"
         else:
-            normkey = key
+            norm_key = key
             key = key.replace("__norm", "")
 
-        if normkey in self.keys():
-            saved = self[normkey]  # performs len check
+        if norm_key in self.keys():
+            saved = self[norm_key]  # performs len check
             # return if original is not modified
             if not self[key]._modified:  # check if original data is modified
                 return saved
             else:
-                self._saved.pop(normkey)
+                self._saved.pop(norm_key)
 
         # we are here because we have to compute norm. let's save norm
         value = self[key]
         if value.shape[1] == 1:
             value_norm = value
         else:
             value_norm = np.linalg.norm(value, axis=1).reshape(-1, 1)
 
         # save norm
-        self[normkey] = value_norm
+        self[norm_key] = value_norm
         # considered not modified
         self[key]._modified = False
 
         return value_norm
 
     def as_arrow(self, key, default=None, raise_=True):
         """
@@ -651,28 +616,28 @@
         "data",
         "function",
         "locations",
         "is_spline",
         "has_function",
         "has_locations",
         "has_evaluate",
-        "arrowdata_only",
+        "arrow_data_only",
         "_user_created",
     )
 
     def __init__(self, data, locations=None, function=None):
         """ """
         # default
         self._user_created = True
         self.data = data
         self.is_spline = False
         self.has_function = False
         self.has_locations = False
         self.has_evaluate = False
-        self.arrowdata_only = False
+        self.arrow_data_only = False
 
         # is spline we know?
         if "CoreSpline" in str(type(data).__mro__):
             self.is_spline = True
 
         # data has evaluate?
         if hasattr(data, "evaluate"):
@@ -686,15 +651,15 @@
             self.function = function
 
         # locations? - keep this compatible with functions. maybe
         # we want to have some state dependent value at certain locations
         if locations is not None:
             # set what holds true
             self.has_locations = True
-            self.arrowdata_only = True
+            self.arrow_data_only = True
             self.locations = np.asanyarray(locations)
 
             # if this is not a spline we know, it doesn't have a function,
             # it should:
             # -> `data.evaluate` is callable, or
             # -> len(data) == len(locations)
             if not self.is_spline and not self.has_function:
@@ -702,37 +667,37 @@
                 if hasattr(data, "__len__"):
                     len_matches = len(locations) == len(data)
                 if not (self.has_evaluate or len_matches):
                     raise ValueError(
                         "Data cannot be represented at specified locations."
                         "Requires one of the following requirements: "
                         "1) is a spline derived from splinepy's spline; "
-                        "2) data has `data.evalauate()`; "
+                        "2) data has `data.evaluate()`; "
                         "3) length of the data and location should match."
                     )
-            # location is sepcified, meaning we don't need sample()
+            # location is specified, meaning we don't need sample()
             return None
 
         # can call sample or has a function?
         if not self.has_function and not self.is_spline:
             raise ValueError(
                 "None spline data should at least have an accompanying "
                 "function."
             )
 
-    def as_vertexdata(self, resolutions=None, on=None):
+    def as_vertex_data(self, resolutions=None, on=None):
         """
         Parameters
         ----------
         resolutions: list or tuple
         at: (n, d) array-like
 
         Returns
         -------
-        vertexdata: (m, r) array-like
+        vertex_data: (m, r) array-like
         """
         if resolutions is not None and on is not None:
             raise ValueError(
                 "Please only specify either `resolutions` or `on`"
             )
 
         if self.has_locations and (resolutions is not None or on is not None):
@@ -846,15 +811,15 @@
         value: np.ndarray
         """
         if key not in self._saved:
             return default
 
         saved = super().__getitem__(key)
         # will raise
-        return saved.as_vertexdata(resolutions=resolutions)
+        return saved.as_vertex_data(resolutions=resolutions)
 
     def as_arrow(self, key, resolutions=None, on=None, default=None):
         """
         Returns as-arrow-representable data on certain places, with given
         resolution, or on predefined places.
 
         Parameters
@@ -864,15 +829,15 @@
         on: array-like
         """
         if key not in self._saved:
             return default
 
         saved = super().__getitem__(key)
         # will raise
-        return saved.as_vertexdata(resolutions=resolutions, on=on)
+        return saved.as_vertex_data(resolutions=resolutions, on=on)
 
 
 Unique2DFloats = namedtuple(
     "Unique2DFloats", ["values", "ids", "inverse", "intersection"]
 )
 Unique2DFloats.__doc__ = """
 namedtuple to hold unique information of float type arrays.
```

### Comparing `gustaf-0.0.8/gustaf/helpers/options.py` & `gustaf-0.0.9/gustaf/helpers/options.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,34 +50,34 @@
         "c",
         "Color in {rgb, RGB, str of (hex, name), int}",
         (str, tuple, list, int),
     ),
     Option("vedo", "alpha", "Transparency in range [0, 1].", (float, int)),
     Option(
         "vedo",
-        "dataname",
-        "Name of vertexdata to show. "
-        "Object must have vertexdata with the same name.",
+        "data_name",
+        "Name of vertex_data to show. "
+        "Object must have vertex_data with the same name.",
         (str,),
     ),
     Option("vedo", "vertex_ids", "Show ids of vertices", (bool,)),
     Option("vedo", "element_ids", "Show ids of elements", (bool,)),
     Option(
         "vedo",
         "lighting",
         "Lighting options {'default', 'metallic', 'plastic', 'shiny', "
         "'glossy', 'ambient', 'off'}",
         (str,),
     ),
-    Option("vedo", "cmap", "Colormap for vertexdata plots.", (str,)),
+    Option("vedo", "cmap", "Colormap for vertex_data plots.", (str,)),
     Option("vedo", "vmin", "Minimum value for cmap", (float, int)),
     Option("vedo", "vmax", "Maximum value for cmap", (float, int)),
     Option(
         "vedo",
-        "cmapalpha",
+        "cmap_alpha",
         "Colormap Transparency in range [0, 1].",
         (float, int),
     ),
     Option(
         "vedo",
         "scalarbar",
         "Scalarbar describing cmap. At least an empty dict or "
@@ -85,29 +85,29 @@
         "{title: str, pos: tuple, title_yoffset: int, font_size: int, "
         "nlabels: int, c: str, horizontal: bool, use_alpha: bool, "
         "label_format: str}. Setting bool will add a default scalarbar",
         (bool, dict),
     ),
     Option(
         "vedo",
-        "arrowdata",
-        "Name of vertexdata to plot as arrow. Corresponding data should be "
+        "arrow_data",
+        "Name of vertex_data to plot as arrow. Corresponding data should be "
         "at least 2D. If you want more control over arrows, consider creating "
         "edges using gus.create.edges.from_data().",
         (str,),
     ),
     Option(
         "vedo",
-        "arrowdata_scale",
+        "arrow_data_scale",
         "Scaling factor for arrow data.",
         (float, int),
     ),
     Option(
         "vedo",
-        "arrowdata_color",
+        "arrow_data_color",
         "Color for arrow data. Can be either cmap name or color. For "
         "cmap, colors are based on the size of the arrows.",
         (str, tuple, list, int),
     ),
     Option(
         "vedo",
         "axes",
@@ -144,15 +144,15 @@
 
     return valid_options
 
 
 class ShowOption:
     """
     Behaves similar to dict, but will only accept a set of options that's
-    applicable to the helpee class. Intented use is to create a
+    applicable to the helpee class. Intended use is to create a
     subclass that would define valid options for helpee.
     Options should be described by Option object.
     Helps all the way up to initializing backend showables up to their backend
     specific common routines. ShowOption and ShowManager in a sense.
     """
 
     __slots__ = ("_helpee", "_options", "_backend")
@@ -384,15 +384,15 @@
         -------
         value: object
         """
         self._options[self._backend].pop(*args, **kwargs)
 
     def copy_valid_options(self, copy_to, keys=None):
         """
-        Copies valid option to other showopts. Simply iterates and treis.
+        Copies valid option to other show_option. Simply iterates and tries.
 
         Parameters
         ----------
         copy_to: ShowOption
         keys: tuple or list
           Can specify keys
```

### Comparing `gustaf-0.0.8/gustaf/helpers/raise_if.py` & `gustaf-0.0.9/gustaf/helpers/raise_if.py`

 * *Files identical despite different names*

### Comparing `gustaf-0.0.8/gustaf/io/default.py` & `gustaf-0.0.9/gustaf/io/default.py`

 * *Files identical despite different names*

### Comparing `gustaf-0.0.8/gustaf/io/ioutils.py` & `gustaf-0.0.9/gustaf/io/ioutils.py`

 * *Files identical despite different names*

### Comparing `gustaf-0.0.8/gustaf/io/meshio.py` & `gustaf-0.0.9/gustaf/io/meshio.py`

 * *Files identical despite different names*

### Comparing `gustaf-0.0.8/gustaf/io/mfem.py` & `gustaf-0.0.9/gustaf/io/mfem.py`

 * *Files identical despite different names*

### Comparing `gustaf-0.0.8/gustaf/io/mixd.py` & `gustaf-0.0.9/gustaf/io/mixd.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,18 +77,18 @@
 
     # boundary conditions
     bcs = dict()
     try:
         bcs_in = np.fromfile(mrng, dtype=">i").astype(np.int32)  # flattened
         uniq_bcs_in = np.unique(bcs_in)
         uniq_bcs_in = uniq_bcs_in[uniq_bcs_in > 0]  # keep only natural nums
-        subelemids = np.arange(bcs_in.size)
+        sub_elem_ids = np.arange(bcs_in.size)
 
         for ubci in uniq_bcs_in:
-            bcs.update({str(ubci): subelemids[bcs_in == ubci]})
+            bcs.update({str(ubci): sub_elem_ids[bcs_in == ubci]})
 
     except BaseException:
         log.debug(f"mrng file, `{mrng}`, does not exist. Skipping.")
 
     # reshape vertices
     vertices = vertices.reshape(-1, 3) if volume else vertices.reshape(-1, 2)
 
@@ -117,15 +117,15 @@
     and hexahedron semi-discrete and (flat) space-time mesh output.
 
     Parameters
     -----------
     mesh: Faces or Volumes
     fname: str
     space_time : bool
-      Export Mesh as Space-Time Slab for discontinous space-time
+      Export Mesh as Space-Time Slab for discontinuous space-time
 
     Returns
     --------
     None
     """
     # did you give us an acceptable mesh?
     acceptable_shapes = ["tri", "quad", "tet", "hexa"]
@@ -225,15 +225,15 @@
 
     Returns
     --------
     boundaries : ndarray
       The mrng-array.
     """
 
-    # determine number of subelements
+    # determine number of sub elements
     whatami = mesh.whatami
     nbelem = 3
 
     if whatami.startswith("quad") or whatami.startswith("tet"):
         nbelem += 1
     elif whatami.startswith("hexa"):
         nbelem += 3
```

### Comparing `gustaf-0.0.8/gustaf/io/nutils.py` & `gustaf-0.0.9/gustaf/io/nutils.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,21 +20,21 @@
       The npz file needs the following keys:
       nodes, cnodes, coords, tags, btags, ptags.
 
     Returns
     --------
     mesh: Faces or Volumes
     """
-    npzfile = np.load(fname, allow_pickle=True)
-    nodes = npzfile["nodes"]
-    _ = npzfile["cnodes"]
-    coords = npzfile["coords"]
-    _ = npzfile["tags"].item()
-    btags = npzfile["btags"].item()
-    _ = npzfile["ptags"].item()
+    npz_file = np.load(fname, allow_pickle=True)
+    nodes = npz_file["nodes"]
+    _ = npz_file["cnodes"]
+    coords = npz_file["coords"]
+    _ = npz_file["tags"].item()
+    btags = npz_file["btags"].item()
+    _ = npz_file["ptags"].item()
 
     if nodes.shape[0] == 0:
         raise TypeError("Can not find nodes. Check nutils mesh description.")
     if coords.shape[0] == 0:
         raise TypeError("Can not find coords. Check nutils mesh description.")
 
     vertices = coords
@@ -129,15 +129,15 @@
     bcs_in = np.ndarray.reshape(
         bcs_in, (int(len(bcs_in) / (dimension + 1)), (dimension + 1))
     )
 
     bound_id = np.unique(bcs_in)
     bound_id = bound_id[bound_id > 0]
 
-    # Reorder the mrng according to nutils permutation: swap collumns
+    # Reorder the mrng according to nutils permutation: swap columns
     bcs_in[:, :] = bcs_in[:, permutation]
 
     # Let's reorder the bcs file with the sort_array
     bcs_sorted = np.take_along_axis(bcs_in, sort_array, axis=1)
 
     for bi in bound_id:
         bcs[str(bi)] = np.argwhere(bcs_sorted == bi)
```

### Comparing `gustaf-0.0.8/gustaf/show.py` & `gustaf-0.0.9/gustaf/show.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,29 +31,29 @@
         """call show()"""
         return show(*args, **kwargs)
 
 
 sys.modules[__name__].__class__ = _CallableShowDotPy
 
 
-def show(*gusobj, **kwargs):
+def show(*gus_obj, **kwargs):
     """Shows using appropriate backend.
 
     Parameters
     -----------
-    *gusobj: gustaf objects
+    *gus_obj: gustaf objects
 
     Returns
     --------
     None
     """
     vis_b = settings.VISUALIZATION_BACKEND
 
     if vis_b.startswith("vedo"):
-        return show_vedo(*gusobj, **kwargs)
+        return show_vedo(*gus_obj, **kwargs)
     elif vis_b.startswith("trimesh"):
         pass
     elif vis_b.startswith("matplotlib"):
         pass
     else:
         raise NotImplementedError
 
@@ -68,130 +68,129 @@
     Parameters
     -----------
     *args: Union[List[Union[gustaf_obj, vedo_obj]], Dict[str, Any]]]
     """
     # vedo plotter parameter
     N = len(args)
     offs = kwargs.get("offscreen", False)
-    interac = kwargs.get("interactive", True)
+    interact = kwargs.get("interactive", True)
     plt = kwargs.get("vedoplot", None)
     skip_clear = kwargs.get("skip_clear", False)
     close = kwargs.get("close", None)
     size = kwargs.get("size", "auto")
     cam = kwargs.get("cam", None)
     title = kwargs.get("title", "gustaf")
     return_show_list = kwargs.get("return_showable_list", False)
 
-    def clear_vedoplotter(plotter, numrenderers, skipcl=skip_clear):
+    def clear_vedo_plotter(plotter, num_renderers, skip_cl=skip_clear):
         """enough said."""
         # for whatever reason it is desired
-        if skipcl:
+        if skip_cl:
             return None
 
-        for i in range(numrenderers):
+        for i in range(num_renderers):
             plotter.clear(at=i)
 
         return None
 
-    def cam_tuple_to_list(dictcam):
+    def cam_tuple_to_list(dict_cam):
         """if entity is tuple, turns it into list."""
-        if dictcam is None:
+        if dict_cam is None:
             return None
 
-        for key, value in dictcam.items():
+        for key, value in dict_cam.items():
             if isinstance(value, tuple):
-                dictcam[key] = list(value)
+                dict_cam[key] = list(value)
 
-        return dictcam
+        return dict_cam
 
     # get plotter
     if plt is None:
         plt = vedo.Plotter(
             N=N, sharecam=False, offscreen=offs, size=size, title=title
         )
 
     else:
         # check if plt has enough Ns
         trueN = np.prod(plt.shape)
-        clear_vedoplotter(plt, trueN)  # always clear.
+        clear_vedo_plotter(plt, trueN)  # always clear.
         if trueN != N:
             utils.log.warning(
                 "Number of args exceed given vedo.Plotter's capacity.",
                 "Assigning a new one",
             )
             title = plt.title
             if close:  # only if it is explicitly stated
-                plt.close()  # Hope that this truely releases..
+                plt.close()  # Hope that this truly releases..
             # assign a new one
             plt = vedo.Plotter(
                 N=N, sharecam=False, offscreen=offs, size=size, title=title
             )
 
     # loop and plot
     for i, arg in enumerate(args):
         # form valid input type.
         if isinstance(arg, dict):
-            showlist = list(arg.values())
+            show_list = list(arg.values())
         elif isinstance(arg, list):
-            showlist = arg.copy()
+            show_list = arg.copy()
         else:
             # raise TypeError(
             #     "For vedo_show, only list or dict is valid input")
             utils.log.debug(
                 "one of args for show_vedo is neither `dict` nor",
                 "`list`. Putting it naively into a list.",
             )
-            showlist = [arg]
+            show_list = [arg]
 
-        # quickcheck if the list is gustaf or non-gustaf
+        # quick check if the list is gustaf or non-gustaf
         # if gustaf, make it vedo-showable.
         # if there's spline, we need to pop the element and
         # extend showables to the list.
-        # A showlist is a list to be plotted into a single subframe of the
+        # A show_list is a list to be plotted into a single sub frame of the
         # plot
         list_of_showables = []
-        for sl in showlist:
+        for sl in show_list:
             if not isinstance(sl, list):
                 sl = [sl]
             for k, item in enumerate(sl):
                 if isinstance(item, GustafBase):
                     tmp_showable = item.showable(backend="vedo", **kwargs)
                     # splines return dict
                     # - maybe it is time to do some typing..
                     if isinstance(tmp_showable, dict):
                         # add to extend later
                         list_of_showables.extend(list(tmp_showable.values()))
-
                     else:
-                        # replace gustafobj with vedo_obj.
+                        # replace gustaf_obj with vedo_obj.
                         list_of_showables.append(tmp_showable)
                 else:
                     list_of_showables.extend(sl)
         # set interactive to true at last element
         if int(i + 1) == len(args):
             plt.show(
                 list_of_showables,
                 at=i,
-                interactive=interac,
+                interactive=interact,
                 camera=cam_tuple_to_list(cam),
                 # offscreen=offs,
             )
 
         else:
             plt.show(
                 list_of_showables,
                 at=i,
                 interactive=False,
                 camera=cam_tuple_to_list(cam),
                 # offscreen=offs,
             )
 
-    if interac and not offs:
+    if interact and not offs:
         # only way to ensure memory is released
-        clear_vedoplotter(plt, np.prod(plt.shape))
+        clear_vedo_plotter(plt, np.prod(plt.shape))
 
         if close or close is None:  # explicitly given or None.
             # It seems to leak some memory, but here it goes.
             plt.close()  # if i close it, this cannot be reused...
             plt = None
 
     if return_show_list:
@@ -204,15 +203,15 @@
     """Generates a vedo obj based on `kind` attribute from given obj, as well
     as show_options.
 
     Parameters
     -----------
     obj: gustaf obj
     as_dict: bool
-      If True, returns vedo objects in a dict. Corresponding main objecst will
+      If True, returns vedo objects in a dict. Corresponding main objects will
       be available with ["main"] key. Else, returns vedo.Assembly object,
       where all the objects are grouped together.
     **kwargs: kwargs
       Will try to overwrite applicable items.
 
     Returns
     --------
@@ -231,15 +230,15 @@
             except BaseException:
                 utils.log.debug(
                     f"Skipping invalid option {key} for "
                     f"{obj.show_options._helps}"
                 )
                 continue
 
-    # minimal-initalization of vedo objects
+    # minimal-initialization of vedo objects
     vedo_obj = obj.show_options._initialize_showable()
     # as dict?
     if as_dict:
         return_as_dict = dict()
 
     # set common values. Could be a perfect place to try :=, but we want to
     # support p3.6.
@@ -263,93 +262,93 @@
         if element_ids:
             utils.log.debug(
                 "`element_ids` option is True for Vertices. Overwriting it as"
                 "vertex_ids."
             )
             element_ids = False
     if vertex_ids:
-        # use vtk font. supposedly faster. And differs from cellid.
+        # use vtk font. supposedly faster. And differs from cell id.
         vertex_ids = vedo_obj.labels("id", on="points", font="VTK")
         if not as_dict:
             vedo_obj += vertex_ids
         else:
             return_as_dict["vertex_ids"] = vertex_ids
     if element_ids:
         # should only reach here if this obj is not vertex
         element_ids = vedo.Points(obj.centers()).labels("id", on="points")
         if not as_dict:
             vedo_obj += element_ids
         else:
             return_as_dict["element_ids"] = element_ids
 
     # data plotting
-    dataname = obj.show_options.get("dataname", None)
-    vertexdata = obj.vertexdata.as_scalar(dataname, None)
-    if dataname is not None and vertexdata is not None:
+    data_name = obj.show_options.get("data_name", None)
+    vertex_data = obj.vertex_data.as_scalar(data_name, None)
+    if data_name is not None and vertex_data is not None:
         # transfer data
         if obj.kind.startswith("edge"):
-            vedo_obj.pointdata[dataname] = vertexdata[obj.edges].reshape(
-                -1, vertexdata.shape[1]
+            vedo_obj.pointdata[data_name] = vertex_data[obj.edges].reshape(
+                -1, vertex_data.shape[1]
             )
         else:
-            vedo_obj.pointdata[dataname] = vertexdata
+            vedo_obj.pointdata[data_name] = vertex_data
 
         # form cmap kwargs for init
         cmap_keys = ("vmin", "vmax")
         cmap_kwargs = obj.show_options[cmap_keys]
-        # set adefault cmap if needed
-        cmap_kwargs["cname"] = obj.show_options.get("cmap", "plasma")
-        cmap_kwargs["alpha"] = obj.show_options.get("cmapalpha", 1)
-        # add dataname
-        cmap_kwargs["input_array"] = dataname
+        # set a default cmap if needed
+        cmap_kwargs["input_cmap"] = obj.show_options.get("cmap", "plasma")
+        cmap_kwargs["alpha"] = obj.show_options.get("cmap_alpha", 1)
+        # add data_name
+        cmap_kwargs["input_array"] = data_name
 
         # set cmap
         vedo_obj.cmap(**cmap_kwargs)
 
         # at last, scalarbar
-        # deprecated function name, keeep it for now for backward compat
+        # deprecated function name, keep it for now for backward compat
         sb_kwargs = obj.show_options.get("scalarbar", None)
         if sb_kwargs is not None and sb_kwargs is not False:
             sb_kwargs = dict() if isinstance(sb_kwargs, bool) else sb_kwargs
             vedo_obj.addScalarBar(**sb_kwargs)
 
-    elif dataname is not None and vertexdata is None:
+    elif data_name is not None and vertex_data is None:
         utils.log.debug(
-            f"No vertexdata named '{dataname}' for {obj}. Skipping"
+            f"No vertex_data named '{data_name}' for {obj}. Skipping"
         )
 
     # arrow plots - this is independent from data plotting.
-    arrowdata_name = obj.show_options.get("arrowdata", None)
+    arrow_data_name = obj.show_options.get("arrow_data", None)
     # will raise if data is scalar
-    arrowdata_value = obj.vertexdata.as_arrow(arrowdata_name, None, True)
-    if arrowdata_name is not None and arrowdata_value is not None:
+    arrow_data_value = obj.vertex_data.as_arrow(arrow_data_name, None, True)
+    if arrow_data_name is not None and arrow_data_value is not None:
         from gustaf.create.edges import from_data
 
         # we are here because this data is not a scalar
         # is showable?
-        if arrowdata_value.shape[1] not in (2, 3):
+        if arrow_data_value.shape[1] not in (2, 3):
             raise ValueError(
                 "Only 2D or 3D data can be shown.",
-                f"Requested data is {arrowdata_value.shape[1]}",
+                f"Requested data is {arrow_data_value.shape[1]}",
             )
 
         as_edges = from_data(
             obj,
-            arrowdata_value,
-            obj.show_options.get("arrowdata_scale", None),
-            data_norm=obj.vertexdata.as_scalar(arrowdata_name),
+            arrow_data_value,
+            obj.show_options.get("arrow_data_scale", None),
+            data_norm=obj.vertex_data.as_scalar(arrow_data_name),
         )
         arrows = vedo.Arrows(
             as_edges.vertices[as_edges.edges],
-            c=obj.show_options.get("arrowdata_color", "plasma"),
+            c=obj.show_options.get("arrow_data_color", "plasma"),
         )
         if not as_dict:
             vedo_obj += arrows
         else:
-            return_as_dict["arrowdata"] = arrows
+            return_as_dict["arrow_data"] = arrows
 
     axes_kw = obj.show_options.get("axes", None)
     # need to explicitly check if it is false
     if axes_kw is not None and axes_kw is not False:
         axes_kw = dict() if isinstance(axes_kw, bool) else axes_kw
         axes = vedo.Axes(vedo_obj, **axes_kw)
         if not as_dict:
@@ -378,41 +377,42 @@
     pass
 
 
 def make_showable(obj, backend=settings.VISUALIZATION_BACKEND, **kwargs):
     """Since gustaf does not natively support visualization, one of the
     following library is used to visualize gustaf (visualizable) objects: (1)
     vedo -> Fast, offers a lot of features (2) trimesh -> Fast, compatible with
-    old opengl (3) matplotlib -> Slow, offers vector graphics.
+    old OpenGL (3) matplotlib -> Slow, offers vector graphics.
 
     This determines showing types using `whatami`.
 
     Parameters
     -----------
     obj: gustaf-objects
     backend: str
       (Optional) Default is `gustaf.settings.VISUALIZATION_BACKEND`.
       Options are: "vedo" | "trimesh" | "matplotlib"
 
     Returns
     --------
-    showalbe_objs: list
+    showable_objs: list
       List of showable objects.
     """
     if backend.startswith("vedo"):
         return _vedo_showable(obj, **kwargs)
     elif backend.startswith("trimesh"):
         return _trimesh_showable(obj, **kwargs)
     elif backend.startswith("matplotlib"):
         return _matplotlib_showable(obj, **kwargs)
     else:
         raise NotImplementedError
 
 
-# possibly relocate
+# possibly relocate, is this actually used?
+# could not find any usage in this repo
 def interpolate_vedo_dictcam(cameras, resolutions, spline_degree=1):
     """Interpolate between vedo dict cameras.
 
     Parameters
     ------------
     cameras: list or tuple
     resolutions: int
@@ -429,20 +429,20 @@
 
         spp = True
 
     except ImportError:
         spp = False
 
     # quick type check loop
-    camkeys = ["pos", "focalPoint", "viewup", "distance", "clippingRange"]
+    cam_keys = ["pos", "focalPoint", "viewup", "distance", "clippingRange"]
     for cam in cameras:
         if not isinstance(cam, dict):
             raise TypeError("Only `dict` description of vedo cam is allowed.")
         else:
-            for key in camkeys:
+            for key in cam_keys:
                 if cam[key] is None:
                     raise ValueError(
                         f"One of the camera does not contain `{key}` info"
                     )
 
     interpolated_cams = []
     total_cams = int(resolutions) * (len(cameras) - 1)
@@ -456,71 +456,71 @@
 
         ps = []
         fs = []
         vs = []
         ds = []
         cs = []
         for cam in cameras:
-            ps.append(list(cam[camkeys[0]]))
-            fs.append(list(cam[camkeys[1]]))
-            vs.append(list(cam[camkeys[2]]))
-            ds.append([float(cam[camkeys[3]])])
-            cs.append(list(cam[camkeys[4]]))
+            ps.append(list(cam[cam_keys[0]]))
+            fs.append(list(cam[cam_keys[1]]))
+            vs.append(list(cam[cam_keys[2]]))
+            ds.append([float(cam[cam_keys[3]])])
+            cs.append(list(cam[cam_keys[4]]))
 
         interpolated = dict()
         for i, prop in enumerate([ps, fs, vs, ds, cs]):
-            ispline = splinepy.BSpline()
-            ispline.interpolate_curve(
+            i_spline = splinepy.BSpline()
+            i_spline.interpolate_curve(
                 query_points=prop,
                 degree=spline_degree,
                 save_query=False,
             )
-            interpolated[camkeys[i]] = ispline.sample([total_cams])
+            interpolated[cam_keys[i]] = i_spline.sample([total_cams])
 
         for i in range(total_cams):
             interpolated_cams.append(
                 {
-                    camkeys[0]: interpolated[camkeys[0]][i].tolist(),
-                    camkeys[1]: interpolated[camkeys[1]][i].tolist(),
-                    camkeys[2]: interpolated[camkeys[2]][i].tolist(),
-                    camkeys[3]: interpolated[camkeys[3]][i][0],  # float?
-                    camkeys[4]: interpolated[camkeys[4]][i].tolist(),
+                    cam_keys[0]: interpolated[cam_keys[0]][i].tolist(),
+                    cam_keys[1]: interpolated[cam_keys[1]][i].tolist(),
+                    cam_keys[2]: interpolated[cam_keys[2]][i].tolist(),
+                    cam_keys[3]: interpolated[cam_keys[3]][i][0],  # float?
+                    cam_keys[4]: interpolated[cam_keys[4]][i].tolist(),
                 }
             )
 
     else:
         i = 0
-        for startcam, endcam in zip(cameras[:-1], cameras[1:]):
+        for start_cam, end_cam in zip(cameras[:-1], cameras[1:]):
             if i == 0:
                 interpolated = [
                     np.linspace(
-                        startcam[ckeys],
-                        endcam[ckeys],
+                        start_cam[ckeys],
+                        end_cam[ckeys],
                         resolutions,
                     ).tolist()
-                    for ckeys in camkeys
+                    for ckeys in cam_keys
                 ]
 
             else:
                 interpolated = [
                     np.linspace(
-                        startcam[ckeys],
-                        endcam[ckeys],
+                        start_cam[ckeys],
+                        end_cam[ckeys],
                         int(resolutions + 1),
                     )[1:].tolist()
-                    for ckeys in camkeys
+                    for ckeys in cam_keys
                 ]
 
             i += 1
 
             for j in range(resolutions):
                 interpolated_cams.append(
                     {
-                        camkeys[0]: interpolated[0][j],
-                        camkeys[1]: interpolated[1][j],
-                        camkeys[2]: interpolated[2][j],
-                        camkeys[3]: interpolated[3][j],  # float?
-                        camkeys[4]: interpolated[4][j],
+                        cam_keys[0]: interpolated[0][j],
+                        cam_keys[1]: interpolated[1][j],
+                        cam_keys[2]: interpolated[2][j],
+                        cam_keys[3]: interpolated[3][j],  # float?
+                        cam_keys[4]: interpolated[4][j],
                     }
                 )
 
     return interpolated_cams
```

### Comparing `gustaf-0.0.8/gustaf/spline/__init__.py` & `gustaf-0.0.9/gustaf/spline/__init__.py`

 * *Files identical despite different names*

### Comparing `gustaf-0.0.8/gustaf/spline/base.py` & `gustaf-0.0.9/gustaf/spline/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,16 +14,17 @@
 from gustaf.spline import visualize
 from gustaf.spline.create import Creator
 from gustaf.spline.extract import Extractor
 from gustaf.spline.proximity import Proximity
 
 
 def show(spline, **kwargs):
-    """Shows splines with various options. They are excessively listed, so that
-    it can be adjustable.
+    """Shows splines with various options.
+
+    They are excessively listed, so that it can be adjustable.
 
     Parameters
     -----------
     spline: BSpline or NURBS
     resolutions: int or (spline.para_dim,) array-like
     control_points: bool
     knots: bool
@@ -100,24 +101,24 @@
     return showmodule.show_vedo(things_to_show, **kwargs)
 
 
 class GustafSpline(GustafBase):
     __show_option__ = visualize.SplineShowOption
 
     def __init__(self):
-        """Contructor as abstractmethod.
+        """Constructor as abstractmethod.
 
         This needs to be inherited first to make sure duplicating
         functions properly override splinepy.Spline
         """
         self._extractor = Extractor(self)
         self._proximity = Proximity(self)
         self._creator = Creator(self)
         self._show_options = self.__show_option__(self)
-        self._splinedata = SplineData(self)
+        self._spline_data = SplineData(self)
 
     @property
     def show_options(self):
         """
         Show option manager for splines.
 
         Parameters
@@ -127,45 +128,45 @@
         Returns
         -------
         show_options: SplineShowOption
         """
         return self._show_options
 
     @property
-    def splinedata(self):
+    def spline_data(self):
         """
         Spline data helper for splines.
 
         Parameters
         ----------
         None
 
         Returns
         -------
-        splinedata: SplineData
+        spline_data: SplineData
         """
-        return self._splinedata
+        return self._spline_data
 
     @property
     def extract(self):
-        """Returns spline extracter. Can directly perform extractions available
+        """Returns spline extractor. Can directly perform extractions available
         at `gustaf/spline/extract.py`. For more info, take a look at
-        `gustaf/spline/extract.py`: Extracter.
+        `gustaf/spline/extract.py`: Extractor.
 
         Examples
         ---------
-        >>> splinefaces = spline.extract.faces()
+        >>> spline_faces = spline.extract.faces()
 
         Parameters
         -----------
         None
 
         Returns
         --------
-        spline_extracter: Extracter
+        spline_extractor: Extractor
         """
         return self._extractor
 
     @property
     def create(self):
         """Returns spline creator Can be used to create new splines using
         geometric relations.
```

### Comparing `gustaf-0.0.8/gustaf/spline/create.py` & `gustaf-0.0.9/gustaf/spline/create.py`

 * *Files 2% similar despite different names*

```diff
@@ -257,36 +257,36 @@
     Returns
     --------
     spline: BSpline
     """
     physical_bounds = np.asanyarray(physical_bounds).reshape(2, -1)
     parametric_bounds = np.asanyarray(parametric_bounds).reshape(2, -1)
 
-    # get correctly sized bezbox
+    # get correctly sized bez box
     phys_size = physical_bounds[1] - physical_bounds[0]
 
     # minimal bspline
     bspline_box = box(*phys_size).bspline  # kvs are in [0, 1]
     bspline_box.cps += physical_bounds[0]  # apply offset
 
     # update parametric bounds
     for i, kv in enumerate(bspline_box.kvs):
         # apply scale and offset
-        newkv = (kv * parametric_bounds[1][i]) + parametric_bounds[0][i]
-        bspline_box.kvs[i] = newkv
+        new_kv = (kv * parametric_bounds[1][i]) + parametric_bounds[0][i]
+        bspline_box.kvs[i] = new_kv
 
     return bspline_box
 
 
 def parametric_view(spline, axes=True):
     """Create parametric view of given spline. Previously called
     `naive_spline()`. Degrees are always 1 and knot multiplicity is not
     preserved. Returns BSpline, as BSpline and NURBS should look the same as
     parametric view.
-    Will take shallow copy of underlying data of splinedata and show_options
+    Will take shallow copy of underlying data of spline_data and show_options
     from original spline.
 
     Parameters
     -----------
     spline: BSpline or NURBS
     axes: bool
      If True, will configure axes settings, it is supported.
@@ -302,39 +302,39 @@
 
     # loop through knot vectors and insert missing knots
     for i, kv in enumerate(spline.unique_knots):
         if len(kv) > 2:
             para_spline.insert_knots(i, kv[1:-1])
 
     # take shallow copy
-    para_spline._splinedata._saved = spline.splinedata._saved.copy()
+    para_spline._spline_data._saved = spline.spline_data._saved.copy()
     para_spline._show_options._options[
         para_spline._show_options._backend
     ] = spline.show_options._options[spline._show_options._backend].copy()
 
     if axes and "axes" in spline.show_options.valid_keys():
         # configure axes
         bs = p_bounds
         bs_diff_001 = (bs[1] - bs[0]) * 0.001
-        lowerb = bs[0] - bs_diff_001
-        upperb = bs[1] + bs_diff_001
+        lower_b = bs[0] - bs_diff_001
+        upper_b = bs[1] + bs_diff_001
         axes_config = dict(
             xtitle="u",
             ytitle="v",
-            xrange=[lowerb[0], upperb[0]],
-            yrange=[lowerb[1], upperb[1]],
+            xrange=[lower_b[0], upper_b[0]],
+            yrange=[lower_b[1], upper_b[1]],
             tip_size=0,
             xminor_ticks=3,
             yminor_ticks=3,
             xygrid=False,
             yzgrid=False,
         )
         if spline.para_dim == 3:
             axes_config.update(ztitle="w")
-            axes_config.update(zrange=[lowerb[2], upperb[2]])
+            axes_config.update(zrange=[lower_b[2], upper_b[2]])
             axes_config.update(zminor_ticks=3)
             axes_config.update(zxgrid=False)
 
         para_spline.show_options["axes"] = axes_config
         # it is a view, so cps won't be realistic
         para_spline.show_options["control_points"] = False
         para_spline.show_options["lighting"] = "off"
@@ -416,24 +416,24 @@
         degrees=[0], control_points=[start_point], weights=[1.0]
     )
     # Bezier splines only support angles lower than 180 degrees
     if abs(angle) >= np.pi or n_knot_spans > 1:
         point_spline = point_spline.nurbs
 
     # Revolve - set degree to False, since all the angles are converted to rad
-    arc_attribs = point_spline.create.revolved(
+    arc_attrib = point_spline.create.revolved(
         angle=angle, n_knot_spans=n_knot_spans, degree=False
     ).todict()
-    # Remove the first parametric dimenions, which is only a point and
+    # Remove the first parametric dimensions, which is only a point and
     # only used for the revolution
-    arc_attribs["degrees"] = list(arc_attribs["degrees"])[1:]
+    arc_attrib["degrees"] = list(arc_attrib["degrees"])[1:]
     if point_spline.has_knot_vectors:
-        arc_attribs["knot_vectors"] = list(arc_attribs["knot_vectors"])[1:]
+        arc_attrib["knot_vectors"] = list(arc_attrib["knot_vectors"])[1:]
 
-    return type(point_spline)(**arc_attribs)
+    return type(point_spline)(**arc_attrib)
 
 
 def circle(radius=1.0, n_knot_spans=3):
     """Circle (parametric dim = 1) with radius r in the x-y plane around the
     origin. The spline has an open knot vector and degree 2.
 
     Parameters
@@ -447,34 +447,34 @@
     -------
     circle: NURBS
     """
     return arc(radius=radius, angle=360, n_knot_spans=n_knot_spans)
 
 
 def box(*lengths):
-    """ND box (hyperrectangle).
+    """ND box (hyper rectangle).
 
     Parameters
     ----------
     *lengths: list(float)
 
     Returns
     -------
-    ndbox: Bezier
+    nd_box: Bezier
     """
     from gustaf import Bezier
 
     # may dim check here?
     # starting point
-    ndbox = Bezier(degrees=[1], control_points=[[0], [lengths[0]]])
+    nd_box = Bezier(degrees=[1], control_points=[[0], [lengths[0]]])
     # use extrude
     for i, l in enumerate(lengths[1:]):
-        ndbox = ndbox.create.extruded([0] * int(i + 1) + [l])
+        nd_box = nd_box.create.extruded([0] * int(i + 1) + [l])
 
-    return ndbox
+    return nd_box
 
 
 def plate(radius=1.0):
     """Creates a biquadratic 2-D spline in the shape of a plate with given
     radius.
 
     Parameters
@@ -573,15 +573,15 @@
     torus_radius : float
       Radius of the torus
     section_outer_radius : float
       Radius of the section of the torus
     section_inner_radius : float, optional
       Inner radius in case of hollow torus, by default 0.
     torus_angle : float, optional
-      Rotational anlge of the torus, by default None, giving a complete
+      Rotational angle of the torus, by default None, giving a complete
       revolution
     section_angle : float, optional
       Rotational angle, by default None, yielding a complete revolution
     section_n_knot_spans : float, optional
       Number of knot spans along the cross-section, by default 4
     torus_n_knot_spans : float, optional
       Number of knot spans along the torus, by default 4
@@ -699,15 +699,15 @@
       Parameter whether surface or volume spline, by default True
     angle : float
       Rotation angle in degrees, only used for solid model
 
     Returns
     -------
     cone: NURBS
-      Volumetric or surface NURBS descibing a cone
+      Volumetric or surface NURBS describing a cone
     """
 
     if volumetric:
         ground = disk(
             outer_radius, inner_radius=inner_radius, angle=angle, degree=degree
         )
     else:
@@ -729,15 +729,15 @@
     """Creates a volumetric spline in the shape of a pyramid with linear degree
     in every direction.
 
     Parameters
     ----------
     width : float
       Dimension of base in x-axis
-    lenght : float
+    length : float
       Dimension of base in y-axis
     height : float
       Height in z-direction
 
     Returns
     -------
     pyramid: BSpline
@@ -754,16 +754,16 @@
 
 
 class Creator:
     """Helper class to build new splines from existing geometries.
 
     Examples
     ---------
-    >>> myspline = <your-spline>
-    >>> spline_faces = myspline.create.extrude(vector=[3,1,3])
+    >>> my_spline = <your-spline>
+    >>> spline_faces = my_spline.create.extrude(vector=[3,1,3])
     """
 
     def __init__(self, spl):
         self.spline = spl
 
     def extruded(self, *args, **kwargs):
         return extruded(self.spline, *args, **kwargs)
```

### Comparing `gustaf-0.0.8/gustaf/spline/extract.py` & `gustaf-0.0.9/gustaf/spline/extract.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,28 +58,30 @@
             if len(extract_knot) != spline.para_dim - 1:
                 raise ValueError(
                     "Must satisfy len(extract_knot) == spline.para_dim -1."
                 )
 
         # This may take awhile.
         if all_knots:
-            edgess = []  # edges' is not a valid syntax
+            temp_edges = []  # edges' is not a valid syntax
             unique_knots = np.array(spline.unique_knots, dtype=object)
             for i in range(spline.para_dim):
                 mask = np.ones(spline.para_dim, dtype=bool)
                 mask[i] = False
                 # gather knots along current knot
                 extract_knot_queries = list(
                     itertools.product(*unique_knots[mask])
                 )
 
                 for ekq in extract_knot_queries:
-                    edgess.append(edges(spline, resolution[i], i, ekq, False))
+                    temp_edges.append(
+                        edges(spline, resolution[i], i, ekq, False)
+                    )
 
-            return Edges.concat(edgess)
+            return Edges.concat(temp_edges)
 
         # Get parametric points to extract
         queries = np.empty(
             (resolution, spline.para_dim),
             dtype="float64",  # hardcoded for splinelibpy
             order="C",  # hardcoded for splinelibpy
         )
@@ -138,38 +140,38 @@
         # TODO: use spline extraction routine to first extract
         # spline, extract faces, merge vertices.
 
         # Spline to surfaces
         vertices = []
         faces = []
         offset = 0
-        # accomodate bezier Splines
-        ukvs = spline.unique_knots
+        # accommodate bezier Splines
+        u_kvs = spline.unique_knots
 
         for i in range(spline.para_dim):
             extract = i
             # Get extracting dimension
             extract_along = [0, 1, 2]
             extract_along.pop(extract)
 
             # Extract range
             extract_range = [
                 [
-                    min(ukvs[extract_along[0]]),
-                    max(ukvs[extract_along[0]]),
+                    min(u_kvs[extract_along[0]]),
+                    max(u_kvs[extract_along[0]]),
                 ],
                 [
-                    min(ukvs[extract_along[1]]),
-                    max(ukvs[extract_along[1]]),
+                    min(u_kvs[extract_along[1]]),
+                    max(u_kvs[extract_along[1]]),
                 ],
             ]
 
             extract_list = [
-                min(ukvs[extract]),
-                max(ukvs[extract]),
+                min(u_kvs[extract]),
+                max(u_kvs[extract]),
             ]
 
             # surface point queries (spq)
             spq = np.linspace(
                 extract_range[0][0],
                 extract_range[0][1],
                 resolutions[extract_along[0]],
@@ -370,33 +372,33 @@
     else:
         raise ValueError(
             "Invalid para_dim to extract control_mesh. " "Supports 1 to 3."
         )
 
 
 def spline(spline, para_dim, split_plane):
-    """Extract a subspline from a given representation.
+    """Extract a sub spline from a given representation.
 
     Parameters
     ----------
     para_dim : int
-      parametric dimension to be extrac ted
+      parametric dimension to be extract ted
     split_plane : float / tuple<float, float>
-      intervall or value in parametric space to be extracted from the spline
+      interval or value in parametric space to be extracted from the spline
       representation
 
     Returns
     -------
     spline
     """
     from gustaf.spline.base import GustafSpline
 
     # Check type
     if not issubclass(type(spline), GustafSpline):
-        raise TypeError("Unknown spline representation passed to subspline")
+        raise TypeError("Unknown spline representation passed to sub spline")
 
     # Check arguments for sanity
     if para_dim > spline.para_dim:
         raise ValueError(
             "Requested parametric dimension exceeds spline's parametric"
             " dimensionality."
         )
@@ -431,15 +433,15 @@
     for _ in range(spline_copy.degrees[para_dim]):
         # Will do nothing if spline already has sufficient number of knots
         # at given position
         spline_copy.insert_knots(para_dim, split_plane)
 
     # Start extraction
     cps_res = spline_copy.control_mesh_resolutions
-    # start and end id. indicies correspond to [first dim][first appearance]
+    # start and end id. indices correspond to [first dim][first appearance]
     start_id = np.where(
         abs(spline_copy.knot_vectors[para_dim] - split_plane[0])
         < settings.TOLERANCE
     )[0][0]
     end_id = np.where(
         abs(spline_copy.knot_vectors[para_dim] - split_plane[-1])
         < settings.TOLERANCE
@@ -461,23 +463,23 @@
         spline_info["degrees"].pop(para_dim)
     if not is_bezier:
         spline_info["knot_vectors"] = spline_copy.knot_vectors.copy()
         if start_id == end_id:
             spline_info["knot_vectors"].pop(para_dim)
         else:
             start_knot = spline_copy.knot_vectors[para_dim][start_id]
-            knots_inbetween = spline_copy.knot_vectors[para_dim][
+            knots_in_between = spline_copy.knot_vectors[para_dim][
                 start_id : (end_id + spline_copy.degrees[para_dim])
             ]
             end_knot = spline_copy.knot_vectors[para_dim][
                 (end_id + spline_copy.degrees[para_dim] - 1)
             ]
 
             spline_info["knot_vectors"][para_dim] = np.concatenate(
-                ([start_knot], knots_inbetween, [end_knot])
+                ([start_knot], knots_in_between, [end_knot])
             )
 
     if is_rational:
         spline_info["weights"] = spline_copy.weights[
             (para_dim_ids >= start_id) & (para_dim_ids <= end_id)
         ]
 
@@ -486,16 +488,16 @@
 
 class Extractor:
     """Helper class to allow direct extraction from spline obj (BSpline or
     NURBS). Internal use only.
 
     Examples
     ---------
-    >>> myspline = <your-spline>
-    >>> spline_faces = myspline.extract.faces()
+    >>> my_spline = <your-spline>
+    >>> spline_faces = my_spline.extract.faces()
     """
 
     def __init__(self, spl):
         self._spline = spl
 
     def edges(self, *args, **kwargs):
         return edges(self._spline, *args, **kwargs)
@@ -523,37 +525,37 @@
 
     def beziers(self):
         return self._spline.extract_bezier_patches()
 
     def boundaries(self, *args, **kwargs):
         return self._spline.extract_boundaries(*args, **kwargs)
 
-    def spline(self, splittin_plane=None, interval=None):
+    def spline(self, splitting_plane=None, interval=None):
         """Extract a spline from a spline.
 
         Use a (number of) splitting planes to extract a subsection from the
         parametric domain of it.
 
         Parameters
         ----------
         splitting_plane : int / dictionary (int : (float))
           if integer : parametric dimension to be extracted
           if dictionary : list of splitting planes and ranges to be passed
         interval : float / tuple<float,float>
-          intervall or value in parametric space to be extracted from the
+          interval or value in parametric space to be extracted from the
           spline representation
         Returns
         -------
         spline
         """
-        if isinstance(splittin_plane, dict):
+        if isinstance(splitting_plane, dict):
             if interval is not None:
                 raise ValueError("Arguments incompatible expect dictionary")
-            splittin_plane = dict(
-                sorted(splittin_plane.items(), key=lambda x: x[0])[::-1]
+            splitting_plane = dict(
+                sorted(splitting_plane.items(), key=lambda x: x[0])[::-1]
             )
             spline_copy = self._spline.copy()
-            for key, item in splittin_plane.items():
+            for key, item in splitting_plane.items():
                 spline_copy = spline(spline_copy, key, item)
             return spline_copy
         else:
-            return spline(self._spline, splittin_plane, interval)
+            return spline(self._spline, splitting_plane, interval)
```

### Comparing `gustaf-0.0.8/gustaf/spline/ffd.py` & `gustaf-0.0.9/gustaf/spline/ffd.py`

 * *Files 1% similar despite different names*

```diff
@@ -438,17 +438,17 @@
         # prepare deformed
         d_mesh = self.mesh  # copies
 
         things_to_show = dict()
         # let's show faces at most, since volumes can take awhile
         if o_mesh.kind == "volume":
             # only outer faces. overwrite
-            o_mesh = o_mesh.tofaces(unique=False)
+            o_mesh = o_mesh.to_faces(unique=False)
             o_mesh.update_faces(o_mesh.single_faces())
-            d_mesh = d_mesh.tofaces(unique=False)
+            d_mesh = d_mesh.to_faces(unique=False)
             d_mesh.update_faces(d_mesh.single_faces())
 
         # update meshes
         things_to_show.update(original_mesh=o_mesh)
         things_to_show.update(original_description="Original Mesh")
         things_to_show.update(deformed_mesh=d_mesh)
         things_to_show.update(deformed_description="Deformed Mesh with Spline")
@@ -457,15 +457,15 @@
         things_to_show.update(deformed_spline=self.spline)
 
         if return_discrete or not backend.startswith("vedo"):
             # spline is strictly not discrete.
             return things_to_show
 
         if return_showable:
-            # let's turn everthing into showable and return
+            # let's turn everything into showable and return
             for k, v in things_to_show.items():
                 if isinstance(v, GustafBase):
                     things_to_show[k] = v.showable()
 
             return things_to_show
 
         # current workaround to set spline's surface alpha correctly
```

### Comparing `gustaf-0.0.8/gustaf/spline/microstructure/microstructure.py` & `gustaf-0.0.9/gustaf/spline/microstructure/microstructure.py`

 * *Files identical despite different names*

### Comparing `gustaf-0.0.8/gustaf/spline/microstructure/tiles/__init__.py` & `gustaf-0.0.9/gustaf/spline/microstructure/tiles/__init__.py`

 * *Files identical despite different names*

### Comparing `gustaf-0.0.8/gustaf/spline/microstructure/tiles/crosstile2d.py` & `gustaf-0.0.9/gustaf/spline/microstructure/tiles/crosstile2d.py`

 * *Files identical despite different names*

### Comparing `gustaf-0.0.8/gustaf/spline/microstructure/tiles/crosstile3d.py` & `gustaf-0.0.9/gustaf/spline/microstructure/tiles/crosstile3d.py`

 * *Files identical despite different names*

### Comparing `gustaf-0.0.8/gustaf/spline/microstructure/tiles/inversecrosstile3d.py` & `gustaf-0.0.9/gustaf/spline/microstructure/tiles/inversecrosstile3d.py`

 * *Files identical despite different names*

### Comparing `gustaf-0.0.8/gustaf/spline/microstructure/tiles/tilebase.py` & `gustaf-0.0.9/gustaf/spline/microstructure/tiles/tilebase.py`

 * *Files identical despite different names*

### Comparing `gustaf-0.0.8/gustaf/spline/proximity.py` & `gustaf-0.0.9/gustaf/spline/proximity.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,16 +50,16 @@
 
 class Proximity:
     """Helper class to allow direct proximity queries for spline obj (BSpline
     or NURBS). Internal use only.
 
     Examples
     ---------
-    >>> myspline = <your-spline>
-    >>> closest_cp_ids = myspline.proximity.closest_control_points(queries)
+    >>> my_spline = <your-spline>
+    >>> closest_cp_ids = my_spline.proximity.closest_control_points(queries)
     """
 
     def __init__(self, spl):
         self.spline = spl
 
     def closest_control_points(self, *args, **kwargs):
         return closest_control_points(self.spline, *args, **kwargs)
```

### Comparing `gustaf-0.0.8/gustaf/spline/visualize.py` & `gustaf-0.0.9/gustaf/spline/visualize.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,16 +58,16 @@
             "vedo",
             "resolutions",
             "Sampling resolution for spline.",
             (int, list, tuple, np.ndarray),
         ),
         options.Option(
             "vedo",
-            "arrowdata_on",
-            "Specify parametric coordinates to place arrowdata.",
+            "arrow_data_on",
+            "Specify parametric coordinates to place arrow_data.",
             (list, tuple, np.ndarray),
         ),
     )
 
     _helps = "GustafSpline"
 
     def __init__(self, helpee):
@@ -90,15 +90,15 @@
 
 def make_showable(spline):
     return eval(f"_{spline.show_options._backend}_showable(spline)")
 
 
 def _vedo_showable(spline):
     """
-    Goes through common precedures for preparing showable splines.
+    Goes through common procedures for preparing showable splines.
 
     Parameters
     ----------
     None
 
     Returns
     -------
@@ -124,99 +124,99 @@
         "axes", False
     )
 
     # with color representable, scalar field data
     res = enforce_len(
         spline.show_options.get("resolutions", 100), spline.para_dim
     )
-    dataname = spline.show_options.get("dataname", None)
-    sampled_splinedata = spline.splinedata.as_scalar(
-        dataname, res, default=None
+    data_name = spline.show_options.get("data_name", None)
+    sampled_spline_data = spline.spline_data.as_scalar(
+        data_name, res, default=None
     )
-    if dataname is not None and sampled_splinedata is not None:
+    if data_name is not None and sampled_spline_data is not None:
         # transfer data
-        sampled_spline.vertexdata[dataname] = sampled_splinedata
+        sampled_spline.vertex_data[data_name] = sampled_spline_data
 
         # transfer options - maybe vectorized query?
-        keys = ("vmin", "vmax", "scalarbar", "cmap", "cmapalpha")
+        keys = ("vmin", "vmax", "scalarbar", "cmap", "cmap_alpha")
         spline.show_options.copy_valid_options(
             sampled_spline.show_options, keys
         )
 
         # mark that we want to see this data
-        sampled_spline.show_options["dataname"] = dataname
+        sampled_spline.show_options["data_name"] = data_name
 
-    elif dataname is not None and sampled_splinedata is None:
-        log.debug(f"No splinedata named ({dataname}) for {spline}. Skipping")
+    elif data_name is not None and sampled_spline_data is None:
+        log.debug(f"No spline_data named ({data_name}) for {spline}. Skipping")
 
     # with arrow representable, vector data
-    adata_name = spline.show_options.get("arrowdata", None)
-    adapted_adata = spline.splinedata.get(adata_name, None)
+    adata_name = spline.show_options.get("arrow_data", None)
+    adapted_adata = spline.spline_data.get(adata_name, None)
     if adata_name is not None and adapted_adata is not None:
         # if location is specified, this will be a separate Vertices obj with
-        # configured arrowdata
+        # configured arrow_data
         has_locations = adapted_adata.has_locations
-        adata_on = "arrowdata_on" in spline.show_options.keys()
+        adata_on = "arrow_data_on" in spline.show_options.keys()
         create_vertices = has_locations or adata_on
 
         # this case causes conflict of interest. raise
         if has_locations and adata_on:
             raise ValueError(
-                f"arrowdata-({adata_name}) has fixed location, "
-                "but and `arrowdata_on` is set.",
+                f"arrow_data-({adata_name}) has fixed location, "
+                "but and `arrow_data_on` is set.",
             )
 
         if create_vertices:
             # prepare corresponding queries
             if adapted_adata.has_locations:
                 queries = adapted_adata.locations
                 on = None
             else:
-                queries = spline.show_options["arrowdata_on"]
+                queries = spline.show_options["arrow_data_on"]
                 on = queries
 
             # bound /  dim check
             bounds = spline.parametric_bounds
             if queries.shape[1] != len(bounds[0]):
                 raise ValueError(
-                    "Dimension mismatch: arrowdata locations-"
+                    "Dimension mismatch: arrow_data locations-"
                     f"{queries.shape[1]} / para_dim-{spline.para_dim}."
                 )
             # tolerance padding. may still cause issues in splinepy.
             # in that case, we will have to scale queries.
             lb_diff = queries.min(axis=0) - bounds[0] + settings.TOLERANCE
             ub_diff = queries.max(axis=0) - bounds[1] - settings.TOLERANCE
             if any(lb_diff < 0) or any(ub_diff > 0):
                 raise ValueError(
                     f"Specified locations of ({adata_name}) are out side the "
                     f"parametric bounds ({bounds}) by [{lb_diff}, {ub_diff}]."
                 )
 
             # get arrow
-            adata = spline.splinedata.as_arrow(adata_name, on=on)
+            adata = spline.spline_data.as_arrow(adata_name, on=on)
 
             # create vertices that can be shown as arrows
             loc_vertices = Vertices(spline.evaluate(queries), copy=False)
-            loc_vertices.vertexdata[adata_name] = adata
+            loc_vertices.vertex_data[adata_name] = adata
 
             # transfer options
-            keys = ("arrowdata_scale", "arrowdata_color", "arrowdata")
+            keys = ("arrow_data_scale", "arrow_data_color", "arrow_data")
             spline.show_options.copy_valid_options(
                 loc_vertices.show_options, keys
             )
 
             # add to primitives
-            gus_primitives["arrowdata"] = loc_vertices
+            gus_primitives["arrow_data"] = loc_vertices
 
         else:  # sample arrows and append to sampled spline.
-            sampled_spline.vertexdata[adata_name] = spline.splinedata.as_arrow(
-                adata_name, resolutions=res
-            )
+            sampled_spline.vertex_data[
+                adata_name
+            ] = spline.spline_data.as_arrow(adata_name, resolutions=res)
             # transfer options
-            keys = ("arrowdata_scale", "arrowdata_color", "arrowdata")
+            keys = ("arrow_data_scale", "arrow_data_color", "arrow_data")
             spline.show_options.copy_valid_options(
                 sampled_spline.show_options, keys
             )
 
     # double check on same obj ref
     gus_primitives["spline"] = sampled_spline
 
@@ -238,41 +238,40 @@
             cp_ids = spline.extract.control_points()
             cp_ids.show_options["labels"] = np.arange(len(cp_ids.vertices))
             cp_ids.show_options["label_options"] = {"font": "VTK"}
             gus_primitives["control_point_ids"] = cp_ids
 
     if spline.show_options.get("control_mesh", show_cps):
         # pure control mesh
-        cmesh = spline.extract.control_mesh()  # either edges or faces
+        c_mesh = spline.extract.control_mesh()  # either edges or faces
         if spline.para_dim != 1:
-            cmesh = cmesh.toedges(unique=True)
+            c_mesh = c_mesh.to_edges(unique=True)
 
-        cmesh.show_options["c"] = "red"
-        cmesh.show_options["lw"] = 4
-        cmesh.show_options["alpha"] = spline.show_options.get(
+        c_mesh.show_options["c"] = "red"
+        c_mesh.show_options["lw"] = 4
+        c_mesh.show_options["alpha"] = spline.show_options.get(
             "control_points_alpha", 0.8
         )
         # add
-        gus_primitives["control_mesh"] = cmesh
+        gus_primitives["control_mesh"] = c_mesh
 
     # fitting queries
     if hasattr(spline, "_fitting_queries") and spline.show_options.get(
         "fitting_queries", True
     ):
         fqs = Vertices(spline._fitting_queries)
         fqs.show_options["c"] = "blue"
         fqs.show_options["r"] = 10
         gus_primitives["fitting_queries"] = fqs
 
     return gus_primitives
 
 
 def _vedo_showable_para_dim_1(spline):
-    """
-    Assumes showability check has been already performed
+    """Assumes showability check has been already performed.
 
     Parameters
     ----------
     spline: GustafSpline
 
     Returns
     -------
```

### Comparing `gustaf-0.0.8/gustaf/utils/arr.py` & `gustaf-0.0.9/gustaf/utils/arr.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,15 @@
         id of neighbors within the tolerance.
     """
     from scipy.spatial import cKDTree as KDTree
 
     if tolerance is None:
         tolerance = settings.TOLERANCE
 
-    # Build kdtree
+    # Build kd tree
     kdt = KDTree(arr)
 
     # Ball point query, taking tolerance as radius
     neighbors = kdt.query_ball_point(
         arr,
         tolerance,
         # workers=workers,
@@ -336,19 +336,21 @@
             rotation_axis, settings.FLOAT_DTYPE
         ).ravel()
 
     if rotation_axis is None:
         return np.matmul(arr, rotation_matrix(rotation, degree))
 
     else:
-        rarr = arr - rotation_axis
-        rarr = np.matmul(rarr, rotation_matrix(rotation, degree))
-        rarr += rotation_axis
+        rotated_array = arr - rotation_axis
+        rotated_array = np.matmul(
+            rotated_array, rotation_matrix(rotation, degree)
+        )
+        rotated_array += rotation_axis
 
-        return rarr
+        return rotated_array
 
 
 def rotation_matrix_around_axis(axis=None, rotation=None, degree=True):
     """Compute rotation matrix given the axis of rotation. Works for both 2D
     and 3D Uses Rodrigues' formula.
 
     If axis is not specified, 2D rotation matrix is assumed.
```

### Comparing `gustaf-0.0.8/gustaf/utils/connec.py` & `gustaf-0.0.9/gustaf/utils/connec.py`

 * *Files 3% similar despite different names*

```diff
@@ -232,15 +232,15 @@
 
     # closed is ignored
     if not continuous:
         if indices.size % 2 == 1:
             raise ValueError("Ranges should result in even number of indices.")
         return indices.reshape(-1, 2)
 
-    # continous edges
+    # continuous edges
     indices = np.repeat(indices, 2)
     if closed:
         indices = np.append(indices, indices[0])[1:]
     else:
         indices = indices[1:-1]
 
     return indices.reshape(-1, 2)
@@ -395,15 +395,15 @@
 
     Parameters
     -----------
     edges: (n, 2) np.ndarray
 
     Returns
     --------
-    subd_edges: (n * 2, 2) np.ndarray
+    subdivided_edges: (n * 2, 2) np.ndarray
     """
     if edges.ndim != 2 or edges.shape[1] != 2:
         raise ValueError("Invalid edges shape!")
 
     raise NotImplementedError
 
 
@@ -441,57 +441,57 @@
     -----------
     mesh: Mesh
     return_dict: bool
 
     Returns
     --------
     new_vertices: (n, d) np.ndarray
-    subd_faces: (m, 3) np.ndarray
+    subdivided_faces: (m, 3) np.ndarray
     mesh_dict: dict
       iff `return_dict=True`,
-      returns dict(vertices=new_vertices, faces=subd_faces).
+      returns dict(vertices=new_vertices, faces=subdivided_faces).
     """
     # This will only pass if the mesh is triangle mesh.
     if mesh.faces.shape[1] != 3:
         raise ValueError("Invalid faces shape!")
 
     # Form new vertices
     edge_mid_v = mesh.vertices[mesh.unique_edges().values].mean(axis=1)
     new_vertices = np.vstack((mesh.vertices, edge_mid_v))
 
-    subd_faces = np.empty(
+    subdivided_faces = np.empty(
         (mesh.faces.shape[0] * 4, mesh.faces.shape[1]),
         dtype=np.int32,
     )
 
-    mask = np.ones(subd_faces.shape[0], dtype=bool)
+    mask = np.ones(subdivided_faces.shape[0], dtype=bool)
     mask[3::4] = False
 
     # 0th column minus (every 4th row, starting from 3rd row)
-    subd_faces[mask, 0] = mesh.faces.flatten()  # copies
+    subdivided_faces[mask, 0] = mesh.faces.flatten()  # copies
 
     # Form ids for new vertices
     new_vertices_ids = mesh.unique_edges().inverse + int(mesh.faces.max() + 1)
     # 1st & 2nd columns
-    subd_faces[mask, 1] = new_vertices_ids
-    subd_faces[mask, 2] = new_vertices_ids.reshape(-1, 3)[
+    subdivided_faces[mask, 1] = new_vertices_ids
+    subdivided_faces[mask, 2] = new_vertices_ids.reshape(-1, 3)[
         :, [2, 0, 1]
     ].flatten()
 
     # Every 4th row, starting from 3rd row
-    subd_faces[~mask, :] = new_vertices_ids.reshape(-1, 3)
+    subdivided_faces[~mask, :] = new_vertices_ids.reshape(-1, 3)
 
     if return_dict:
         return dict(
             vertices=new_vertices,
-            faces=subd_faces,
+            faces=subdivided_faces,
         )
 
     else:
-        return new_vertices, subd_faces
+        return new_vertices, subdivided_faces
 
 
 def subdivide_quad(
     mesh,
     return_dict=False,
 ):
     """Subdivide quads.
@@ -500,18 +500,18 @@
     -----------
     mesh: Mesh
     return_dict: bool
 
     Returns
     --------
     new_vertices: (n, d) np.ndarray
-    subd_faces: (m, 4) np.ndarray
+    subdivided_faces: (m, 4) np.ndarray
     mesh_dict: dict
       iff `return_dict=True`,
-      returns dict(vertices=new_vertices, faces=subd_faces).
+      returns dict(vertices=new_vertices, faces=subdivided_faces).
     """
     # This will only pass if the mesh is quad mesh.
     if mesh.faces.shape[1] != 4:
         raise ValueError("Invalid faces shape!")
 
     # Form new vertices
     edge_mid_v = mesh.vertices[mesh.unique_edges().values].mean(axis=1)
@@ -520,38 +520,38 @@
         (
             mesh.vertices,
             edge_mid_v,
             face_centers,
         )
     )
 
-    subd_faces = np.empty(
+    subdivided_faces = np.empty(
         (mesh.faces.shape[0] * 4, mesh.faces.shape[1]),
         dtype=np.int32,
     )
 
-    subd_faces[:, 0] = mesh.faces.flatten()
-    subd_faces[:, 1] = mesh.unique_edges().inverse + len(mesh.vertices)
-    subd_faces[:, 2] = np.repeat(
+    subdivided_faces[:, 0] = mesh.faces.flatten()
+    subdivided_faces[:, 1] = mesh.unique_edges().inverse + len(mesh.vertices)
+    subdivided_faces[:, 2] = np.repeat(
         np.arange(len(face_centers)) + (len(mesh.vertices) + len(edge_mid_v)),
         4,
         # dtype=np.int32,
     )
-    subd_faces[:, 3] = (
-        subd_faces[:, 1].reshape(-1, 4)[:, [3, 0, 1, 2]].flatten()
+    subdivided_faces[:, 3] = (
+        subdivided_faces[:, 1].reshape(-1, 4)[:, [3, 0, 1, 2]].flatten()
     )
 
     if return_dict:
         return dict(
             vertices=new_vertices,
-            faces=subd_faces,
+            faces=subdivided_faces,
         )
 
     else:
-        return new_vertices, subd_faces
+        return new_vertices, subdivided_faces
 
 
 def sorted_unique(connectivity, sorted_=False):
     """Given connectivity array, finds unique entries, based on its axis=1
     sorted values. Returned value will be sorted.
 
     Parameters
```

### Comparing `gustaf-0.0.8/gustaf/utils/log.py` & `gustaf-0.0.9/gustaf/utils/log.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 
 def prepended_log(message, log_func):
     """
     Prepend message before a logging function.
 
     Parameters
     ----------
-    messgae: str
+    message: str
     log_func: function
       one of the followings - {info, debug, warning}
 
     Returns
     -------
     prepended: function
     """
```

### Comparing `gustaf-0.0.8/gustaf/vertices.py` & `gustaf-0.0.9/gustaf/vertices.py`

 * *Files 6% similar despite different names*

```diff
@@ -87,18 +87,18 @@
 
     __slots__ = (
         "_vertices",
         "_const_vertices",
         "_computed",
         "_show_options",
         "_setter_copies",
-        "_vertexdata",
+        "_vertex_data",
     )
 
-    # define freuqently used types as dunder variable
+    # define frequently used types as dunder variable
     __show_option__ = VerticesShowOption
 
     def __init__(
         self,
         vertices=None,
         copy=True,
     ):
@@ -115,15 +115,15 @@
         None
         """
         # call setters
         self.setter_copies = copy
         self.vertices = vertices
 
         # init helpers
-        self._vertexdata = helpers.data.VertexData(self)
+        self._vertex_data = helpers.data.VertexData(self)
         self._computed = helpers.data.ComputedMeshData(self)
         self._show_options = self.__show_option__(self)
 
     @property
     def vertices(self):
         """Returns vertices.
 
@@ -164,18 +164,18 @@
         if self._vertices.size > 0:
             utils.arr.is_shape(self._vertices, (-1, -1), strict=True)
 
         # exact same, but not tracked.
         self._const_vertices = self._vertices.view()
         self._const_vertices.flags.writeable = False
 
-        # at each setting, validate vertexdata
+        # at each setting, validate vertex_data
         # --> by len mismatch, will clear data
-        if hasattr(self, "vertexdata"):
-            self.vertexdata._validate_len(raise_=False)
+        if hasattr(self, "vertex_data"):
+            self.vertex_data._validate_len(raise_=False)
 
     @property
     def const_vertices(self):
         """Returns non-mutable view of `vertices`. Naming inspired by c/cpp
         sessions.
 
         Parameters
@@ -186,29 +186,29 @@
         --------
         None
         """
         self._logd("returning const_vertices")
         return self._const_vertices
 
     @property
-    def vertexdata(self):
+    def vertex_data(self):
         """
-        Returns vertexdata manager. Behaves similar to dict() and can be used
+        Returns vertex_data manager. Behaves similar to dict() and can be used
         to store values/data associated with each vertex.
 
         Parameters
         ----------
         None
 
         Returns
         -------
-        vertexdata: VertexData
+        vertex_data: VertexData
         """
-        self._logd("returning vertexdata")
-        return self._vertexdata
+        self._logd("returning vertex_data")
+        return self._vertex_data
 
     @property
     def setter_copies(self):
         """
         Switch to set if setter should copy or try to avoid copying.
         If data is np.ndarray, c_contiguous, and has same dtype as
         corresponding settings.<FLOAT/INT>_dtype, it can probably avoid being
@@ -341,15 +341,15 @@
 
         Parameters
         -----------
         None
 
         Returns
         --------
-        bounds_digonal: (d,) np.ndarray
+        bounds_diagonal: (d,) np.ndarray
           same as `bounds[1] - bounds[0]`
         """
         self._logd("computing bounds_diagonal")
         bounds = self.bounds()
         return bounds[1] - bounds[0]
 
     @helpers.data.ComputedMeshData.depends_on(["vertices"])
@@ -407,40 +407,40 @@
         if inverse is not None and self.kind != "vertex":
             elements = self.const_elements.copy()
             elements = inverse[elements.reshape(-1)].reshape(
                 (-1, elements.shape[1])
             )
             # remove all the elements that's not part of inverse
             if check_neg:
-                emask = (elements > -1).all(axis=1)
-                elements = elements[emask]
+                elem_mask = (elements > -1).all(axis=1)
+                elements = elements[elem_mask]
 
         # apply mask
         vertices = vertices[mask]
 
-        def update_vertexdata(obj, m, vertex_data=None):
+        def update_vertex_data(obj, m, vertex_data=None):
             """apply mask to vertex data if there's any."""
-            newdata = helpers.data.VertexData(obj)
+            new_data = helpers.data.VertexData(obj)
             if vertex_data is None:
-                vertex_data = obj.vertexdata
+                vertex_data = obj.vertex_data
 
             for key, values in vertex_data.items():
                 # should work, since this is called after updating vertices
-                newdata[key] = values[m]
+                new_data[key] = values[m]
 
-            obj._vertexdata = newdata
+            obj._vertex_data = new_data
 
             return obj
 
         # update
         self.vertices = vertices
         if elements is not None:
             self.elements = elements
 
-        update_vertexdata(self, mask)
+        update_vertex_data(self, mask)
 
         return self
 
     def select_vertices(self, ranges):
         """Returns vertices inside the given range.
 
         Parameters
@@ -526,15 +526,15 @@
 
         Parameters
         -----------
         None
 
         Returns
         --------
-        selfcopy: type(self)
+        self_copy: type(self)
         """
         # all attributes are deepcopy-able
         return copy.deepcopy(self)
 
     @classmethod
     def concat(cls, *instances):
         """Sequentially put them together to make one object.
@@ -562,16 +562,16 @@
             len(instances) == 1
             and not isinstance(instances[0], str)
             and hasattr(instances[0], "__iter__")
         ):
             instances = instances[0]
 
         vertices = []
-        haselem = cls.kind != "vertex"
-        if haselem:
+        has_elem = cls.kind != "vertex"
+        if has_elem:
             elements = []
 
         # check if everything is "concatable".
         for ins in instances:
             if not is_concatable(ins):
                 raise TypeError(
                     "Can't concat. One of the instances is not "
@@ -579,28 +579,28 @@
                 )
 
             # make sure each element index starts from 0 & end at len(vertices)
             tmp_ins = ins.copy().remove_unreferenced_vertices()
 
             vertices.append(tmp_ins.vertices.copy())
 
-            if haselem:
+            if has_elem:
                 if len(elements) == 0:
                     elements.append(tmp_ins.elements.copy())
                     e_offset = elements[-1].max() + 1
 
                 else:
                     elements.append(
                         # copy is not necessary here,
                         tmp_ins.elements
                         + e_offset
                     )
                     e_offset = elements[-1].max() + 1
 
-        if haselem:
+        if has_elem:
             return cls(
                 vertices=np.vstack(vertices),
                 elements=np.vstack(elements),
             )
 
         else:
             return Vertices(vertices=np.vstack(vertices))
```

### Comparing `gustaf-0.0.8/gustaf/volumes.py` & `gustaf-0.0.9/gustaf/volumes.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,37 +33,37 @@
         Returns
         -------
         volumes: vedo.UGrid or vedo.Mesh
         """
         # without a data to plot on the surface, return vedo.UGrid
         # if vertex_ids is on, we will go with mesh
         if (
-            self.get("dataname", None) is None
+            self.get("data_name", None) is None
             and not self.get("vertex_ids", False)
-            and not self.get("arrowdata", False)
+            and not self.get("arrow_data", False)
         ):
             from vtk import VTK_HEXAHEDRON as herr_hexa
             from vtk import VTK_TETRA as frau_tetra
 
             to_vtktype = {"tet": frau_tetra, "hexa": herr_hexa}
             grid_type = to_vtktype[self._helpee.whatami]
-            ugrid = show.vedo.UGrid(
+            u_grid = show.vedo.UGrid(
                 [
                     self._helpee.const_vertices,
                     self._helpee.const_volumes,
                     [grid_type] * len(self._helpee.const_volumes),
                 ]
             )
-            return ugrid.c("hotpink")
+            return u_grid.c("hotpink")
 
         # to show data, let's use Faces. This will plot all the elements
         # as well as invisible ones. This will at least try to avoid
         # duplicating faces.  If you wanna see inside faces, try
-        # as_shrinked_faces = volumes.tofaces(unique=False).shrink(.8)
-        faces = self._helpee.tofaces(unique=True)
+        # as_shrunk_faces = volumes.to_faces(unique=False).shrink(.8)
+        faces = self._helpee.to_faces(unique=True)
         self.copy_valid_options(faces.show_options)
 
         return faces.show_options._initialize_vedo_showable()
 
 
 class Volumes(Faces):
     kind = "volume"
@@ -236,15 +236,15 @@
         Parameters
         -----------
         None
 
         Returns
         --------
         unique_info: Unique2DIntegers
-          valid attribut4es are {values, ids, inverse, counts}
+          valid attributes are {values, ids, inverse, counts}
         """
         unique_info = utils.connec.sorted_unique(
             self.sorted_volumes(),
             sorted_=True,
         )
 
         volumes = self._get_attr("volumes")
@@ -253,15 +253,15 @@
 
         return unique_info
 
     def update_volumes(self, *args, **kwargs):
         """Alias to update_elements."""
         self.update_elements(*args, **kwargs)
 
-    def tofaces(self, unique=True):
+    def to_faces(self, unique=True):
         """Returns Faces obj.
 
         Parameters
         -----------
         unique: bool
           Default is True. If True, only takes unique faces.
```

### Comparing `gustaf-0.0.8/gustaf.egg-info/PKG-INFO` & `gustaf-0.0.9/gustaf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gustaf
-Version: 0.0.8
+Version: 0.0.9
 Summary: Process and visualize numerical-analysis-geometries.
 Home-page: https://github.com/tataratat/gustaf
 Author: Jaewook Lee
 Author-email: jaewooklee042@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 Provides-Extra: all
 License-File: LICENSE.txt
 
-![gustaf](https://github.com/tataratat/gustaf/raw/gustaf/docs/source/gustaf-logo.png)
+![gustaf](https://github.com/tataratat/gustaf/raw/main/docs/source/gustaf-logo.png)
 
 __gustaf__ is a python library to process and visualize numerical-analysis-geometries; especially for Finite Element Methods (FEM) and Isogemetric Analysis (IGA).
 gustaf currently supports linear elements:
 - triangle,
 - quadrilateral,
 - tetrahedron, and
 - hexahedron,
@@ -81,16 +81,16 @@
         [7, 0, 3, 1],
     ],
 )
 tet.show()
 
 # elements can transform to their subelement types
 # set unique=True, if you don't want duplicating internal subelements
-as_faces = tet.tofaces(unique=False)
-as_edges = tet.toedges(unique=False)
+as_faces = tet.to_faces(unique=False)
+as_edges = tet.to_edges(unique=False)
 
 # as geometry classes inherit from its subelement class, we can
 # extract subelement connectivity directly.
 # Volumes' subelements are faces and subsubelements are edges
 face_connectivity = tet.faces()
 edge_connectivity = tet.edges()
 
@@ -110,18 +110,18 @@
 # there's a shortcut - single_volumes(), single_faces(), single_edges()
 assert np.allclose(
     tet.single_faces(),
     unique_face_infos.ids[unique_face_infos.counts == 1]
 )
 
 # let's visualize some scalar data and vector data defined on vertices
-tet.vertexdata["arange"] = np.arange(len(tet.vertices))  # scalar
-tet.show_options["dataname"] = "arange"
-tet.vertexdata["random"] = np.random.random((len(tet.vertices), 3))  # vector
-tet.show_options["arrowdata"] = "random"
+tet.vertex_data["arange"] = np.arange(len(tet.vertices))  # scalar
+tet.show_options["data_name"] = "arange"
+tet.vertex_data["random"] = np.random.random((len(tet.vertices), 3))  # vector
+tet.show_options["arrow_data"] = "random"
 tet.show()
 
 
 # create a 2D NURBS disc and visualize
 # all the spline types inherits from splinepy's splines and equipped with
 # additional functionalities
 nurbs = gus.NURBS(
@@ -167,19 +167,19 @@
 )
 
 # create derived spline using Creator helper class
 extruded = nurbs.create.extruded(extrusion_vector=[0, 0, 1])
 revolved = nurbs.create.revolved(axis=[1, 0, 0], angle=70)
 parametric_view = nurbs.create.parametric_view()
 
-# just like vertexdata, you can define splinedata
+# just like vertex_data, you can define spline_data
 # for more options, checkout `gus.spline.SplineDataAdaptor`
 # following will plot the norm of nurbs' physical coordinates
-nurbs.splinedata["coords"] = nurbs
-nurbs.show_options["dataname"] = "coords"
+nurbs.spline_data["coords"] = nurbs
+nurbs.show_options["data_name"] = "coords"
 
 # show them all together. each arg is plotted on a separate subplot
 # translate tet a bit to avoid overlapping
 tet.vertices += [2, 0, 0]
 gus.show(
     ["NURBS and translated tet together", nurbs, tet],
     ["Extruded NURBS", extruded],
```

### Comparing `gustaf-0.0.8/gustaf.egg-info/SOURCES.txt` & `gustaf-0.0.9/gustaf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gustaf-0.0.8/setup.py` & `gustaf-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `gustaf-0.0.8/tests/test_basic_calls.py` & `gustaf-0.0.9/tests/test_basic_calls.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         es.single_edges()
         es.elements = es.elements
         es.const_elements
         es.centers()
         es.referenced_vertices()
         es.dashed()
         es.shrink()
-        es.tovertices()
+        es.to_vertices()
         es.single_edges()
         es.remove_unreferenced_vertices()
 
         # es.update_elements()
         # es.update_edges()
 
     def test_faces_basics(self):
@@ -69,36 +69,36 @@
 
             fs.sorted_edges()
             fs.unique_edges()
             fs.single_edges()
             fs.centers()
             fs.referenced_vertices()
             fs.shrink()
-            fs.tovertices()
+            fs.to_vertices()
             fs.remove_unreferenced_vertices()
 
             # fs.update_faces()
             # gus.Faces.whatareyou()
 
     def test_volumes_bascis(self):
         for vs in (gus.Volumes(self.V, self.TV), gus.Volumes(self.V, self.HV)):
             vs.faces()
             vs.whatami
             vs.volumes = vs.volumes
             vs.const_volumes
             vs.sorted_volumes()
             vs.unique_volumes()
-            vs.tofaces()
+            vs.to_faces()
 
             vs.sorted_edges()
             vs.unique_edges()
             vs.single_edges()
             vs.centers()
             vs.referenced_vertices()
             vs.shrink()
-            vs.tovertices()
+            vs.to_vertices()
             vs.remove_unreferenced_vertices()
 
             vs.sorted_faces()
             vs.unique_faces()
             vs.single_faces()
             # gus.Faces.whatareyou()
```

### Comparing `gustaf-0.0.8/tests/test_vertices_and_element_updates.py` & `gustaf-0.0.9/tests/test_vertices_and_element_updates.py`

 * *Files identical despite different names*

