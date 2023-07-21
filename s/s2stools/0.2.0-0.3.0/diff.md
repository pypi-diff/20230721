# Comparing `tmp/s2stools-0.2.0.tar.gz` & `tmp/s2stools-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s2stools-0.2.0.tar", last modified: Mon Jun 19 14:47:27 2023, max compression
+gzip compressed data, was "s2stools-0.3.0.tar", last modified: Fri Jul 21 10:12:53 2023, max compression
```

## Comparing `s2stools-0.2.0.tar` & `s2stools-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,49 @@
-drwxr-xr-x   0 Jonas.Spaeth   (503) staff       (20)        0 2023-06-19 14:47:27.405931 s2stools-0.2.0/
--rw-r--r--   0 Jonas.Spaeth   (503) staff       (20)     1053 2023-04-20 15:07:18.000000 s2stools-0.2.0/LICENSE
--rw-r--r--   0 Jonas.Spaeth   (503) staff       (20)      265 2023-06-19 14:47:27.405319 s2stools-0.2.0/PKG-INFO
--rw-r--r--   0 Jonas.Spaeth   (503) staff       (20)     2372 2023-04-20 15:07:18.000000 s2stools-0.2.0/README.md
-drwxr-xr-x   0 Jonas.Spaeth   (503) staff       (20)        0 2023-06-19 14:47:27.401924 s2stools-0.2.0/s2stools/
--rw-r--r--   0 Jonas.Spaeth   (503) staff       (20)      107 2023-05-04 12:00:27.000000 s2stools-0.2.0/s2stools/__init__.py
--rw-r--r--   0 Jonas.Spaeth   (503) staff       (20)     5911 2023-05-04 12:12:47.000000 s2stools-0.2.0/s2stools/clim.py
--rw-r--r--   0 Jonas.Spaeth   (503) staff       (20)     1974 2023-05-04 12:07:19.000000 s2stools-0.2.0/s2stools/events.py
--rw-r--r--   0 Jonas.Spaeth   (503) staff       (20)     3145 2023-05-04 12:12:47.000000 s2stools-0.2.0/s2stools/plot.py
--rw-r--r--   0 Jonas.Spaeth   (503) staff       (20)     4182 2023-05-04 12:12:47.000000 s2stools-0.2.0/s2stools/process.py
-drwxr-xr-x   0 Jonas.Spaeth   (503) staff       (20)        0 2023-06-19 14:47:27.404723 s2stools-0.2.0/s2stools.egg-info/
--rw-r--r--   0 Jonas.Spaeth   (503) staff       (20)      265 2023-06-19 14:47:27.000000 s2stools-0.2.0/s2stools.egg-info/PKG-INFO
--rw-r--r--   0 Jonas.Spaeth   (503) staff       (20)      279 2023-06-19 14:47:27.000000 s2stools-0.2.0/s2stools.egg-info/SOURCES.txt
--rw-r--r--   0 Jonas.Spaeth   (503) staff       (20)        1 2023-06-19 14:47:27.000000 s2stools-0.2.0/s2stools.egg-info/dependency_links.txt
--rw-r--r--   0 Jonas.Spaeth   (503) staff       (20)       36 2023-06-19 14:47:27.000000 s2stools-0.2.0/s2stools.egg-info/requires.txt
--rw-r--r--   0 Jonas.Spaeth   (503) staff       (20)        9 2023-06-19 14:47:27.000000 s2stools-0.2.0/s2stools.egg-info/top_level.txt
--rw-r--r--   0 Jonas.Spaeth   (503) staff       (20)       38 2023-06-19 14:47:27.406157 s2stools-0.2.0/setup.cfg
--rw-r--r--   0 Jonas.Spaeth   (503) staff       (20)      926 2023-06-19 10:34:06.000000 s2stools-0.2.0/setup.py
+drwxr-xr-x   0 jonas.spaeth (14484) ag-birner (11658)        0 2023-07-21 10:12:53.000000 s2stools-0.3.0/
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)       99 2023-07-20 08:28:10.000000 s2stools-0.3.0/AUTHORS.rst
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)       52 2023-07-20 08:28:10.000000 s2stools-0.3.0/CONTRIBUTING.rst
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)       15 2023-07-20 08:28:10.000000 s2stools-0.3.0/LICENSE
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      359 2023-07-20 08:28:10.000000 s2stools-0.3.0/MANIFEST.in
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     1642 2023-07-21 10:12:53.000000 s2stools-0.3.0/PKG-INFO
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      913 2023-07-20 08:28:10.000000 s2stools-0.3.0/README.rst
+drwxr-xr-x   0 jonas.spaeth (14484) ag-birner (11658)        0 2023-07-21 10:12:52.000000 s2stools-0.3.0/docs/
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      638 2023-07-20 08:28:10.000000 s2stools-0.3.0/docs/Makefile
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      769 2023-07-20 08:28:10.000000 s2stools-0.3.0/docs/make.bat
+drwxr-xr-x   0 jonas.spaeth (14484) ag-birner (11658)        0 2023-07-21 10:12:52.000000 s2stools-0.3.0/docs/source/
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      260 2023-07-20 08:28:10.000000 s2stools-0.3.0/docs/source/clim.rst
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      190 2023-07-21 09:20:50.000000 s2stools-0.3.0/docs/source/compute.rst
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     1247 2023-07-20 08:28:10.000000 s2stools-0.3.0/docs/source/conf.py
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      598 2023-07-21 09:20:50.000000 s2stools-0.3.0/docs/source/events.rst
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      576 2023-07-21 09:20:50.000000 s2stools-0.3.0/docs/source/index.rst
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      539 2023-07-21 09:20:50.000000 s2stools-0.3.0/docs/source/indices.rst
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      274 2023-07-21 10:10:48.000000 s2stools-0.3.0/docs/source/install.rst
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     3432 2023-07-20 08:28:10.000000 s2stools-0.3.0/docs/source/intro.rst
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      301 2023-07-20 08:28:10.000000 s2stools-0.3.0/docs/source/plot.rst
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      189 2023-07-20 08:28:10.000000 s2stools-0.3.0/docs/source/process.rst
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      939 2023-07-21 10:10:48.000000 s2stools-0.3.0/pyproject.toml
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)       87 2023-07-20 08:28:10.000000 s2stools-0.3.0/requirements.txt
+drwxr-xr-x   0 jonas.spaeth (14484) ag-birner (11658)        0 2023-07-21 10:12:52.000000 s2stools-0.3.0/s2stools/
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      100 2023-07-21 10:12:08.000000 s2stools-0.3.0/s2stools/__init__.py
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      211 2023-07-20 08:28:10.000000 s2stools-0.3.0/s2stools/_version.py
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)    13035 2023-07-21 09:20:50.000000 s2stools-0.3.0/s2stools/clim.py
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     9421 2023-07-21 09:20:50.000000 s2stools-0.3.0/s2stools/compute.py
+drwxr-xr-x   0 jonas.spaeth (14484) ag-birner (11658)        0 2023-07-21 10:12:53.000000 s2stools-0.3.0/s2stools/download/
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      825 2023-07-21 09:20:50.000000 s2stools-0.3.0/s2stools/download/S2SDownloader.py
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)       61 2023-07-21 09:20:50.000000 s2stools-0.3.0/s2stools/download/__init__.py
+drwxr-xr-x   0 jonas.spaeth (14484) ag-birner (11658)        0 2023-07-21 10:12:53.000000 s2stools-0.3.0/s2stools/download/ecmwf/
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     6725 2023-07-21 09:20:50.000000 s2stools-0.3.0/s2stools/download/ecmwf/S2SDownloaderECMWF.py
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)       33 2023-07-21 09:20:50.000000 s2stools-0.3.0/s2stools/download/ecmwf/__init__.py
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     2430 2023-07-21 09:20:50.000000 s2stools-0.3.0/s2stools/download/ecmwf/model_setup.py
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      530 2023-07-21 10:10:48.000000 s2stools-0.3.0/s2stools/download/utils.py
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)    21424 2023-07-21 09:20:50.000000 s2stools-0.3.0/s2stools/events.py
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     4685 2023-07-21 09:20:50.000000 s2stools-0.3.0/s2stools/indices.py
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     7252 2023-07-21 09:20:50.000000 s2stools-0.3.0/s2stools/plot.py
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)    16985 2023-07-21 09:20:50.000000 s2stools-0.3.0/s2stools/process.py
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     2459 2023-07-21 09:20:50.000000 s2stools-0.3.0/s2stools/utils.py
+drwxr-xr-x   0 jonas.spaeth (14484) ag-birner (11658)        0 2023-07-21 10:12:52.000000 s2stools-0.3.0/s2stools.egg-info/
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     1642 2023-07-21 10:12:52.000000 s2stools-0.3.0/s2stools.egg-info/PKG-INFO
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      898 2023-07-21 10:12:52.000000 s2stools-0.3.0/s2stools.egg-info/SOURCES.txt
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)        1 2023-07-21 10:12:52.000000 s2stools-0.3.0/s2stools.egg-info/dependency_links.txt
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)       42 2023-07-21 10:12:52.000000 s2stools-0.3.0/s2stools.egg-info/requires.txt
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)        9 2023-07-21 10:12:52.000000 s2stools-0.3.0/s2stools.egg-info/top_level.txt
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)       38 2023-07-21 10:12:53.000000 s2stools-0.3.0/setup.cfg
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)       69 2023-07-20 08:28:10.000000 s2stools-0.3.0/setup.py
```

