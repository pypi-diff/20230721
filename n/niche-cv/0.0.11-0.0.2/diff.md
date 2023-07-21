# Comparing `tmp/niche_cv-0.0.11.tar.gz` & `tmp/niche_cv-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "niche_cv-0.0.11.tar", last modified: Fri Jul 21 01:48:32 2023, max compression
+gzip compressed data, was "niche_cv-0.0.2.tar", last modified: Thu Jul 13 03:18:16 2023, max compression
```

## Comparing `niche_cv-0.0.11.tar` & `niche_cv-0.0.2.tar`

### file list

```diff
@@ -1,35 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:48:32.682678 niche_cv-0.0.11/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 01:48:22.000000 niche_cv-0.0.11/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 01:48:22.000000 niche_cv-0.0.11/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-21 01:48:32.682678 niche_cv-0.0.11/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-21 01:48:22.000000 niche_cv-0.0.11/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:48:32.682678 niche_cv-0.0.11/niche_cv/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 01:48:22.000000 niche_cv-0.0.11/niche_cv/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:48:32.682678 niche_cv-0.0.11/niche_cv/detection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 01:48:22.000000 niche_cv-0.0.11/niche_cv/detection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:48:32.682678 niche_cv-0.0.11/niche_cv/detection/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 01:48:22.000000 niche_cv-0.0.11/niche_cv/detection/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:48:32.682678 niche_cv-0.0.11/niche_cv/detection/data/balloon/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 01:48:22.000000 niche_cv-0.0.11/niche_cv/detection/data/balloon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-21 01:48:22.000000 niche_cv-0.0.11/niche_cv/detection/data/shuffle_balloon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:48:32.682678 niche_cv-0.0.11/niche_cv/detection/data/splitter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 01:48:22.000000 niche_cv-0.0.11/niche_cv/detection/data/splitter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-07-21 01:48:22.000000 niche_cv-0.0.11/niche_cv/detection/data/splitter/coco.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-21 01:48:22.000000 niche_cv-0.0.11/niche_cv/detection/data/splitter/splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-07-21 01:48:22.000000 niche_cv-0.0.11/niche_cv/detection/data/splitter/yolo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:48:32.682678 niche_cv-0.0.11/niche_cv/detection/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 01:48:22.000000 niche_cv-0.0.11/niche_cv/detection/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-07-21 01:48:22.000000 niche_cv-0.0.11/niche_cv/detection/models/detr.py
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-21 01:48:22.000000 niche_cv-0.0.11/niche_cv/detection/models/mrcnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-07-21 01:48:22.000000 niche_cv-0.0.11/niche_cv/detection/models/yolo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-07-21 01:48:22.000000 niche_cv-0.0.11/niche_cv/detr.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-21 01:48:22.000000 niche_cv-0.0.11/niche_cv/device.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-21 01:48:22.000000 niche_cv-0.0.11/niche_cv/show.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:48:32.682678 niche_cv-0.0.11/niche_cv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-21 01:48:32.000000 niche_cv-0.0.11/niche_cv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-21 01:48:32.000000 niche_cv-0.0.11/niche_cv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 01:48:32.000000 niche_cv-0.0.11/niche_cv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-21 01:48:32.000000 niche_cv-0.0.11/niche_cv.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 01:48:32.000000 niche_cv-0.0.11/niche_cv.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 01:48:32.682678 niche_cv-0.0.11/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-21 01:48:22.000000 niche_cv-0.0.11/setup.py
+drwxr-xr-x   0 niche      (502) staff       (20)        0 2023-07-13 03:18:16.050017 niche_cv-0.0.2/
+-rw-r--r--   0 niche      (502) staff       (20)        0 2023-07-13 03:01:41.000000 niche_cv-0.0.2/LICENSE
+-rw-r--r--   0 niche      (502) staff       (20)        0 2023-07-13 03:01:46.000000 niche_cv-0.0.2/MANIFEST.in
+-rw-r--r--   0 niche      (502) staff       (20)      224 2023-07-13 03:18:16.048525 niche_cv-0.0.2/PKG-INFO
+drwxr-xr-x   0 niche      (502) staff       (20)        0 2023-07-13 03:18:16.045517 niche_cv-0.0.2/niche_cv/
+-rw-r--r--   0 niche      (502) staff       (20)        0 2023-07-13 03:03:11.000000 niche_cv-0.0.2/niche_cv/__init__.py
+drwxr-xr-x   0 niche      (502) staff       (20)        0 2023-07-13 03:18:16.047659 niche_cv-0.0.2/niche_cv/data/
+-rw-r--r--   0 niche      (502) staff       (20)        0 2023-07-13 03:03:24.000000 niche_cv-0.0.2/niche_cv/data/__init__.py
+drwxr-xr-x   0 niche      (502) staff       (20)        0 2023-07-13 03:18:16.047911 niche_cv-0.0.2/niche_cv/models/
+-rw-r--r--   0 niche      (502) staff       (20)        0 2023-07-13 03:03:16.000000 niche_cv-0.0.2/niche_cv/models/__init__.py
+-rw-r--r--   0 niche      (502) staff       (20)      289 2023-07-13 03:11:53.000000 niche_cv-0.0.2/niche_cv/show.py
+drwxr-xr-x   0 niche      (502) staff       (20)        0 2023-07-13 03:18:16.047358 niche_cv-0.0.2/niche_cv.egg-info/
+-rw-r--r--   0 niche      (502) staff       (20)      224 2023-07-13 03:18:15.000000 niche_cv-0.0.2/niche_cv.egg-info/PKG-INFO
+-rw-r--r--   0 niche      (502) staff       (20)      283 2023-07-13 03:18:15.000000 niche_cv-0.0.2/niche_cv.egg-info/SOURCES.txt
+-rw-r--r--   0 niche      (502) staff       (20)        1 2023-07-13 03:18:15.000000 niche_cv-0.0.2/niche_cv.egg-info/dependency_links.txt
+-rw-r--r--   0 niche      (502) staff       (20)       45 2023-07-13 03:18:15.000000 niche_cv-0.0.2/niche_cv.egg-info/entry_points.txt
+-rw-r--r--   0 niche      (502) staff       (20)        9 2023-07-13 03:18:15.000000 niche_cv-0.0.2/niche_cv.egg-info/top_level.txt
+-rw-r--r--   0 niche      (502) staff       (20)       38 2023-07-13 03:18:16.050124 niche_cv-0.0.2/setup.cfg
+-rw-r--r--   0 niche      (502) staff       (20)      391 2023-07-13 03:17:57.000000 niche_cv-0.0.2/setup.py
```

