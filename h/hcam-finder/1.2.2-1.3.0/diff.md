# Comparing `tmp/hcam_finder-1.2.2.tar.gz` & `tmp/hcam_finder-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcam_finder-1.2.2.tar", last modified: Thu Feb 23 13:49:18 2023, max compression
+gzip compressed data, was "hcam_finder-1.3.0.tar", last modified: Fri Jul 21 10:55:37 2023, max compression
```

## Comparing `hcam_finder-1.2.2.tar` & `hcam_finder-1.3.0.tar`

### file list

```diff
@@ -1,66 +1,68 @@
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-02-23 13:49:18.938707 hcam_finder-1.2.2/
--rw-r--r--   0 sl         (501) staff       (20)      166 2017-02-11 14:24:09.000000 hcam_finder-1.2.2/AUTHORS.rst
--rw-r--r--   0 sl         (501) staff       (20)     3291 2017-02-11 14:24:09.000000 hcam_finder-1.2.2/CONTRIBUTING.rst
--rw-r--r--   0 sl         (501) staff       (20)       89 2017-02-11 14:24:09.000000 hcam_finder-1.2.2/HISTORY.rst
--rw-r--r--   0 sl         (501) staff       (20)     1077 2017-02-11 14:24:09.000000 hcam_finder-1.2.2/LICENSE
--rw-r--r--   0 sl         (501) staff       (20)      302 2017-11-14 10:44:10.000000 hcam_finder-1.2.2/MANIFEST.in
--rw-r--r--   0 sl         (501) staff       (20)     3683 2023-02-23 13:49:18.938767 hcam_finder-1.2.2/PKG-INFO
--rw-r--r--   0 sl         (501) staff       (20)     2663 2021-08-05 13:35:16.000000 hcam_finder-1.2.2/README.rst
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-02-23 13:49:18.930628 hcam_finder-1.2.2/docs/
--rw-r--r--   0 sl         (501) staff       (20)     6782 2017-02-11 14:24:09.000000 hcam_finder-1.2.2/docs/Makefile
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-02-23 13:49:18.926715 hcam_finder-1.2.2/docs/_build/
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-02-23 13:49:18.926820 hcam_finder-1.2.2/docs/_build/html/
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-02-23 13:49:18.931265 hcam_finder-1.2.2/docs/_build/html/_images/
--rw-r--r--   0 sl         (501) staff       (20)    30314 2017-12-18 14:51:55.000000 hcam_finder-1.2.2/docs/_build/html/_images/inst.png
--rw-r--r--   0 sl         (501) staff       (20)    91154 2017-12-18 14:51:55.000000 hcam_finder-1.2.2/docs/_build/html/_images/main.png
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-02-23 13:49:18.932088 hcam_finder-1.2.2/docs/_build/html/_static/
--rw-r--r--   0 sl         (501) staff       (20)      286 2021-07-26 20:38:22.000000 hcam_finder-1.2.2/docs/_build/html/_static/file.png
--rw-r--r--   0 sl         (501) staff       (20)       90 2021-07-26 20:38:22.000000 hcam_finder-1.2.2/docs/_build/html/_static/minus.png
--rw-r--r--   0 sl         (501) staff       (20)       90 2021-07-26 20:38:22.000000 hcam_finder-1.2.2/docs/_build/html/_static/plus.png
--rwxr-xr-x   0 sl         (501) staff       (20)     8468 2021-01-18 16:26:27.000000 hcam_finder-1.2.2/docs/conf.py
--rw-r--r--   0 sl         (501) staff       (20)     1714 2021-08-06 11:55:33.000000 hcam_finder-1.2.2/docs/hcam_finder.rst
--rw-r--r--   0 sl         (501) staff       (20)    21523 2021-08-06 11:55:24.000000 hcam_finder-1.2.2/docs/hipercam.rst
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-02-23 13:49:18.932507 hcam_finder-1.2.2/docs/images/
--rw-r--r--   0 sl         (501) staff       (20)    30314 2017-12-18 14:51:55.000000 hcam_finder-1.2.2/docs/images/inst.png
--rw-r--r--   0 sl         (501) staff       (20)    91154 2017-12-18 14:51:55.000000 hcam_finder-1.2.2/docs/images/main.png
--rw-r--r--   0 sl         (501) staff       (20)      468 2021-01-18 16:44:46.000000 hcam_finder-1.2.2/docs/index.rst
--rw-r--r--   0 sl         (501) staff       (20)     6469 2017-02-11 14:24:09.000000 hcam_finder-1.2.2/docs/make.bat
--rw-r--r--   0 sl         (501) staff       (20)       70 2021-08-06 11:55:33.000000 hcam_finder-1.2.2/docs/modules.rst
--rw-r--r--   0 sl         (501) staff       (20)     5650 2021-01-18 16:44:46.000000 hcam_finder-1.2.2/docs/ultracam.rst
--rw-r--r--   0 sl         (501) staff       (20)       46 2021-01-18 16:44:46.000000 hcam_finder-1.2.2/docs/ultraspec.rst
--rw-r--r--   0 sl         (501) staff       (20)     4037 2021-08-06 11:47:27.000000 hcam_finder-1.2.2/docs/usage.rst
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-02-23 13:49:18.935091 hcam_finder-1.2.2/hcam_finder/
--rw-r--r--   0 sl         (501) staff       (20)      150 2023-02-23 13:46:28.000000 hcam_finder-1.2.2/hcam_finder/__init__.py
--rw-r--r--   0 sl         (501) staff       (20)     2462 2021-01-18 16:44:46.000000 hcam_finder-1.2.2/hcam_finder/config.py
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-02-23 13:49:18.937287 hcam_finder-1.2.2/hcam_finder/data/
--rwxr-xr-x   0 sl         (501) staff       (20)   114588 2017-05-05 16:12:30.000000 hcam_finder-1.2.2/hcam_finder/data/Lato-Black.ttf
--rwxr-xr-x   0 sl         (501) staff       (20)   120196 2017-05-05 16:12:30.000000 hcam_finder-1.2.2/hcam_finder/data/Lato-Regular.ttf
--rw-r--r--   0 sl         (501) staff       (20)      257 2017-02-12 22:30:12.000000 hcam_finder-1.2.2/hcam_finder/data/README.rst
--rw-r--r--   0 sl         (501) staff       (20)     3387 2021-01-18 19:11:06.000000 hcam_finder-1.2.2/hcam_finder/data/config
--rw-r--r--   0 sl         (501) staff       (20)     4062 2021-01-18 19:11:17.000000 hcam_finder-1.2.2/hcam_finder/data/configspec.ini
--rw-r--r--   0 sl         (501) staff       (20)     2966 2020-12-04 18:50:57.000000 hcam_finder-1.2.2/hcam_finder/data/guider_hole_arcseconds.txt
--rw-r--r--   0 sl         (501) staff       (20)    21032 2023-02-23 13:46:51.000000 hcam_finder-1.2.2/hcam_finder/finders.py
--rw-r--r--   0 sl         (501) staff       (20)     2632 2022-02-01 09:58:21.000000 hcam_finder-1.2.2/hcam_finder/finding_chart.py
--rw-r--r--   0 sl         (501) staff       (20)    10438 2023-02-23 13:46:51.000000 hcam_finder-1.2.2/hcam_finder/hcam_finder.py
--rw-r--r--   0 sl         (501) staff       (20)     5618 2021-02-22 09:06:04.000000 hcam_finder-1.2.2/hcam_finder/panstarrs.py
--rw-r--r--   0 sl         (501) staff       (20)     3391 2021-02-16 15:27:07.000000 hcam_finder-1.2.2/hcam_finder/shapes.py
--rw-r--r--   0 sl         (501) staff       (20)     4186 2020-12-04 18:50:57.000000 hcam_finder-1.2.2/hcam_finder/skyview.py
--rw-r--r--   0 sl         (501) staff       (20)     3050 2021-01-21 12:23:25.000000 hcam_finder-1.2.2/hcam_finder/ucam_finder.py
--rw-r--r--   0 sl         (501) staff       (20)     2394 2021-01-18 16:44:46.000000 hcam_finder-1.2.2/hcam_finder/uspec_finder.py
--rw-r--r--   0 sl         (501) staff       (20)     4764 2021-02-12 09:10:54.000000 hcam_finder-1.2.2/hcam_finder/ztf.py
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-02-23 13:49:18.935939 hcam_finder-1.2.2/hcam_finder.egg-info/
--rw-r--r--   0 sl         (501) staff       (20)     3683 2023-02-23 13:49:18.000000 hcam_finder-1.2.2/hcam_finder.egg-info/PKG-INFO
--rw-r--r--   0 sl         (501) staff       (20)     1231 2023-02-23 13:49:18.000000 hcam_finder-1.2.2/hcam_finder.egg-info/SOURCES.txt
--rw-r--r--   0 sl         (501) staff       (20)        1 2023-02-23 13:49:18.000000 hcam_finder-1.2.2/hcam_finder.egg-info/dependency_links.txt
--rw-r--r--   0 sl         (501) staff       (20)        1 2023-02-23 13:47:36.000000 hcam_finder-1.2.2/hcam_finder.egg-info/not-zip-safe
--rw-r--r--   0 sl         (501) staff       (20)       55 2023-02-23 13:49:18.000000 hcam_finder-1.2.2/hcam_finder.egg-info/requires.txt
--rw-r--r--   0 sl         (501) staff       (20)       12 2023-02-23 13:49:18.000000 hcam_finder-1.2.2/hcam_finder.egg-info/top_level.txt
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-02-23 13:49:18.938100 hcam_finder-1.2.2/scripts/
--rw-r--r--   0 sl         (501) staff       (20)    12564 2023-02-23 13:46:51.000000 hcam_finder-1.2.2/scripts/hfinder
--rw-r--r--   0 sl         (501) staff       (20)    10866 2023-02-23 13:46:51.000000 hcam_finder-1.2.2/scripts/ufinder
--rw-r--r--   0 sl         (501) staff       (20)    11371 2023-02-23 13:46:51.000000 hcam_finder-1.2.2/scripts/usfinder
--rw-r--r--   0 sl         (501) staff       (20)      312 2023-02-23 13:49:18.938999 hcam_finder-1.2.2/setup.cfg
--rw-r--r--   0 sl         (501) staff       (20)     1897 2023-02-23 13:46:28.000000 hcam_finder-1.2.2/setup.py
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-02-23 13:49:18.938480 hcam_finder-1.2.2/tests/
--rw-r--r--   0 sl         (501) staff       (20)       24 2017-02-11 14:24:09.000000 hcam_finder-1.2.2/tests/__init__.py
--rw-r--r--   0 sl         (501) staff       (20)      647 2017-02-11 14:24:09.000000 hcam_finder-1.2.2/tests/test_hcam_finder.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-21 10:55:37.992409 hcam_finder-1.3.0/
+-rw-r--r--   0 sl         (501) staff       (20)      166 2017-02-11 14:24:09.000000 hcam_finder-1.3.0/AUTHORS.rst
+-rw-r--r--   0 sl         (501) staff       (20)     3291 2017-02-11 14:24:09.000000 hcam_finder-1.3.0/CONTRIBUTING.rst
+-rw-r--r--   0 sl         (501) staff       (20)       89 2017-02-11 14:24:09.000000 hcam_finder-1.3.0/HISTORY.rst
+-rw-r--r--   0 sl         (501) staff       (20)     1077 2017-02-11 14:24:09.000000 hcam_finder-1.3.0/LICENSE
+-rw-r--r--   0 sl         (501) staff       (20)      302 2017-11-14 10:44:10.000000 hcam_finder-1.3.0/MANIFEST.in
+-rw-r--r--   0 sl         (501) staff       (20)     3683 2023-07-21 10:55:37.992471 hcam_finder-1.3.0/PKG-INFO
+-rw-r--r--   0 sl         (501) staff       (20)     2663 2021-08-05 13:35:16.000000 hcam_finder-1.3.0/README.rst
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-21 10:55:37.982507 hcam_finder-1.3.0/docs/
+-rw-r--r--   0 sl         (501) staff       (20)     6782 2017-02-11 14:24:09.000000 hcam_finder-1.3.0/docs/Makefile
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-21 10:55:37.977881 hcam_finder-1.3.0/docs/_build/
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-21 10:55:37.977979 hcam_finder-1.3.0/docs/_build/html/
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-21 10:55:37.984081 hcam_finder-1.3.0/docs/_build/html/_images/
+-rw-r--r--   0 sl         (501) staff       (20)   438400 2023-05-17 08:38:05.000000 hcam_finder-1.3.0/docs/_build/html/_images/compo.png
+-rw-r--r--   0 sl         (501) staff       (20)    30314 2017-12-18 14:51:55.000000 hcam_finder-1.3.0/docs/_build/html/_images/inst.png
+-rw-r--r--   0 sl         (501) staff       (20)    91154 2017-12-18 14:51:55.000000 hcam_finder-1.3.0/docs/_build/html/_images/main.png
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-21 10:55:37.984988 hcam_finder-1.3.0/docs/_build/html/_static/
+-rw-r--r--   0 sl         (501) staff       (20)      286 2022-07-14 07:38:21.000000 hcam_finder-1.3.0/docs/_build/html/_static/file.png
+-rw-r--r--   0 sl         (501) staff       (20)       90 2022-07-14 07:38:21.000000 hcam_finder-1.3.0/docs/_build/html/_static/minus.png
+-rw-r--r--   0 sl         (501) staff       (20)       90 2022-07-14 07:38:21.000000 hcam_finder-1.3.0/docs/_build/html/_static/plus.png
+-rwxr-xr-x   0 sl         (501) staff       (20)     8468 2021-01-18 16:26:27.000000 hcam_finder-1.3.0/docs/conf.py
+-rw-r--r--   0 sl         (501) staff       (20)     1714 2023-05-19 12:39:10.000000 hcam_finder-1.3.0/docs/hcam_finder.rst
+-rw-r--r--   0 sl         (501) staff       (20)    27352 2023-07-21 10:53:55.000000 hcam_finder-1.3.0/docs/hipercam.rst
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-21 10:55:37.986633 hcam_finder-1.3.0/docs/images/
+-rw-r--r--   0 sl         (501) staff       (20)   438400 2023-07-21 10:53:55.000000 hcam_finder-1.3.0/docs/images/compo.png
+-rw-r--r--   0 sl         (501) staff       (20)    30314 2017-12-18 14:51:55.000000 hcam_finder-1.3.0/docs/images/inst.png
+-rw-r--r--   0 sl         (501) staff       (20)    91154 2017-12-18 14:51:55.000000 hcam_finder-1.3.0/docs/images/main.png
+-rw-r--r--   0 sl         (501) staff       (20)      468 2021-01-18 16:44:46.000000 hcam_finder-1.3.0/docs/index.rst
+-rw-r--r--   0 sl         (501) staff       (20)     6469 2017-02-11 14:24:09.000000 hcam_finder-1.3.0/docs/make.bat
+-rw-r--r--   0 sl         (501) staff       (20)       70 2023-05-19 12:39:10.000000 hcam_finder-1.3.0/docs/modules.rst
+-rw-r--r--   0 sl         (501) staff       (20)     5650 2021-01-18 16:44:46.000000 hcam_finder-1.3.0/docs/ultracam.rst
+-rw-r--r--   0 sl         (501) staff       (20)       46 2021-01-18 16:44:46.000000 hcam_finder-1.3.0/docs/ultraspec.rst
+-rw-r--r--   0 sl         (501) staff       (20)     4055 2023-07-21 10:53:55.000000 hcam_finder-1.3.0/docs/usage.rst
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-21 10:55:37.989370 hcam_finder-1.3.0/hcam_finder/
+-rw-r--r--   0 sl         (501) staff       (20)      150 2023-07-21 10:55:19.000000 hcam_finder-1.3.0/hcam_finder/__init__.py
+-rw-r--r--   0 sl         (501) staff       (20)     2462 2021-01-18 16:44:46.000000 hcam_finder-1.3.0/hcam_finder/config.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-21 10:55:37.991276 hcam_finder-1.3.0/hcam_finder/data/
+-rwxr-xr-x   0 sl         (501) staff       (20)   114588 2017-05-05 16:12:30.000000 hcam_finder-1.3.0/hcam_finder/data/Lato-Black.ttf
+-rwxr-xr-x   0 sl         (501) staff       (20)   120196 2017-05-05 16:12:30.000000 hcam_finder-1.3.0/hcam_finder/data/Lato-Regular.ttf
+-rw-r--r--   0 sl         (501) staff       (20)      257 2017-02-12 22:30:12.000000 hcam_finder-1.3.0/hcam_finder/data/README.rst
+-rw-r--r--   0 sl         (501) staff       (20)     3387 2023-07-21 10:53:55.000000 hcam_finder-1.3.0/hcam_finder/data/config
+-rw-r--r--   0 sl         (501) staff       (20)     4062 2023-07-21 10:53:55.000000 hcam_finder-1.3.0/hcam_finder/data/configspec.ini
+-rw-r--r--   0 sl         (501) staff       (20)     2966 2020-12-04 18:50:57.000000 hcam_finder-1.3.0/hcam_finder/data/guider_hole_arcseconds.txt
+-rw-r--r--   0 sl         (501) staff       (20)    21032 2023-02-23 13:46:51.000000 hcam_finder-1.3.0/hcam_finder/finders.py
+-rw-r--r--   0 sl         (501) staff       (20)     2632 2022-02-01 09:58:21.000000 hcam_finder-1.3.0/hcam_finder/finding_chart.py
+-rw-r--r--   0 sl         (501) staff       (20)    10362 2023-07-21 10:53:55.000000 hcam_finder-1.3.0/hcam_finder/hcam_finder.py
+-rw-r--r--   0 sl         (501) staff       (20)     5618 2021-02-22 09:06:04.000000 hcam_finder-1.3.0/hcam_finder/panstarrs.py
+-rw-r--r--   0 sl         (501) staff       (20)     2414 2023-07-21 10:53:55.000000 hcam_finder-1.3.0/hcam_finder/shapes.py
+-rw-r--r--   0 sl         (501) staff       (20)     4186 2020-12-04 18:50:57.000000 hcam_finder-1.3.0/hcam_finder/skyview.py
+-rw-r--r--   0 sl         (501) staff       (20)     3050 2021-01-21 12:23:25.000000 hcam_finder-1.3.0/hcam_finder/ucam_finder.py
+-rw-r--r--   0 sl         (501) staff       (20)     2394 2021-01-18 16:44:46.000000 hcam_finder-1.3.0/hcam_finder/uspec_finder.py
+-rw-r--r--   0 sl         (501) staff       (20)     4764 2021-02-12 09:10:54.000000 hcam_finder-1.3.0/hcam_finder/ztf.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-21 10:55:37.990022 hcam_finder-1.3.0/hcam_finder.egg-info/
+-rw-r--r--   0 sl         (501) staff       (20)     3683 2023-07-21 10:55:37.000000 hcam_finder-1.3.0/hcam_finder.egg-info/PKG-INFO
+-rw-r--r--   0 sl         (501) staff       (20)     1288 2023-07-21 10:55:37.000000 hcam_finder-1.3.0/hcam_finder.egg-info/SOURCES.txt
+-rw-r--r--   0 sl         (501) staff       (20)        1 2023-07-21 10:55:37.000000 hcam_finder-1.3.0/hcam_finder.egg-info/dependency_links.txt
+-rw-r--r--   0 sl         (501) staff       (20)        1 2023-07-21 10:55:37.000000 hcam_finder-1.3.0/hcam_finder.egg-info/not-zip-safe
+-rw-r--r--   0 sl         (501) staff       (20)       55 2023-07-21 10:55:37.000000 hcam_finder-1.3.0/hcam_finder.egg-info/requires.txt
+-rw-r--r--   0 sl         (501) staff       (20)       12 2023-07-21 10:55:37.000000 hcam_finder-1.3.0/hcam_finder.egg-info/top_level.txt
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-21 10:55:37.991850 hcam_finder-1.3.0/scripts/
+-rw-r--r--   0 sl         (501) staff       (20)    12564 2023-02-23 13:46:51.000000 hcam_finder-1.3.0/scripts/hfinder
+-rw-r--r--   0 sl         (501) staff       (20)    10866 2023-02-23 13:46:51.000000 hcam_finder-1.3.0/scripts/ufinder
+-rw-r--r--   0 sl         (501) staff       (20)    11371 2023-02-23 13:46:51.000000 hcam_finder-1.3.0/scripts/usfinder
+-rw-r--r--   0 sl         (501) staff       (20)      312 2023-07-21 10:55:37.992703 hcam_finder-1.3.0/setup.cfg
+-rw-r--r--   0 sl         (501) staff       (20)     1858 2023-07-21 10:55:19.000000 hcam_finder-1.3.0/setup.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-21 10:55:37.992182 hcam_finder-1.3.0/tests/
+-rw-r--r--   0 sl         (501) staff       (20)       24 2017-02-11 14:24:09.000000 hcam_finder-1.3.0/tests/__init__.py
+-rw-r--r--   0 sl         (501) staff       (20)      647 2017-02-11 14:24:09.000000 hcam_finder-1.3.0/tests/test_hcam_finder.py
```

### Comparing `hcam_finder-1.2.2/CONTRIBUTING.rst` & `hcam_finder-1.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.2.2/LICENSE` & `hcam_finder-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.2.2/PKG-INFO` & `hcam_finder-1.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: hcam_finder
-Version: 1.2.2
+Version: 1.3.0
 Summary: Observation planning and finding charts for HiPerCAM
 Home-page: https://github.com/HiPERCAM/hcam_finder
-Download-URL: https://github.com/HiPERCAM/hcam_finder/archive/v1.2.2.tar.gz
+Download-URL: https://github.com/HiPERCAM/hcam_finder/archive/v1.3.0.tar.gz
 Author: Stuart Littlefair
 Author-email: s.littlefair@shef.ac.uk
 License: MIT license
 Keywords: hcam_finder
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hcam_finder-1.2.2/README.rst` & `hcam_finder-1.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.2.2/docs/Makefile` & `hcam_finder-1.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.2.2/docs/_build/html/_images/inst.png` & `hcam_finder-1.3.0/docs/_build/html/_images/inst.png`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.2.2/docs/_build/html/_images/main.png` & `hcam_finder-1.3.0/docs/_build/html/_images/main.png`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.2.2/docs/conf.py` & `hcam_finder-1.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.2.2/docs/hcam_finder.rst` & `hcam_finder-1.3.0/docs/hcam_finder.rst`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.2.2/docs/hipercam.rst` & `hcam_finder-1.3.0/docs/hipercam.rst`

 * *Files 11% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 =========
 HiPERCAM
 =========
 
 Because HiPERCAM is optimised for high time resolution, there are a number of peculiarities
 to it's use. You should read this document in full before creating a phase II submission.
 
-If you are already familiar with |hiper|, there is a handy :ref:`checklist` you can use
-to check your setups before submission.
+**HiPERCAM is a deceptively complex instrument to use.** Even if you are already familiar
+with |hiper|, we strongly recommend using the  :ref:`checklist` to check your setups before
+submission.
 
 The primary consideration when observing with HiPERCAM is to realise that its frame-transfer
 CCDs have no shutter. Instead, an image is rapidly moved into the storage area, which begins
 a new exposure in the image area. The image continues to expose whilst the storage area is
 reading out. As a result there is very little deadtime between exposures. However, one cannot 
 start a new exposure whilst the storage area is being read out; this sets a *minimum exposure 
 time* equal to the time needed to readout an image.
@@ -32,34 +33,45 @@
 less than 3 second cadence, you will need to use :ref:`windows_h`, or bin the
 readout. For extremely fast observations (more than 10Hz frame rate) there is a 
 special option (:ref:`drift_mode_h`) to reduce readout overheads further. 
 For observations where even shorter exposures are needed, there is a special mode 
 (:ref:`clear_mode_h`), which can be used at the expense of dead time overheads. 
 Therefore, the exposure time can define multiple other aspects of the setup.
 
-For any given setup (binning, window sizes, readout mode), there is an
+For any given setup (binning, window sizes and positions, readout mode), there is an
 absolute minimum exposure time which is set by the time taken to
 readout the storage area. One can expose for longer than
 this minimum by adding an arbitrary "exposure delay"; this is a key
 parameter of the ``hfinder`` setup. So perhaps your setup can be
 readout in 3 seconds, but for reasons of signal-to-noise perhaps you
 add 7 seconds exposure delay. Then your exposure time (and cadence, as
 dead time is negligible in this case) will be 10 seconds. If you set
 the exposure delay to 0 however, your exposure will be 3 seconds and
 you wouldn't be able to go faster without altering the setup.
 
 If your objects are not variable, then, as usual for CCD imaging, you
 should consider:
 
-#. the signal-to-noise you need, 
+#. the signal-to-noise you need (``hfinder`` will provide a summary and there
+   is an `online calculator <http://www.vikdhillon.staff.shef.ac.uk/hipercam/etc.html>`_ 
+   that gives full details), 
 #. the avoidance of saturation of your target and possibly comparison stars, 
 #. allowing enough time for the sky background to dominate over readout noise for faint sky-limited targets especially, and 
 #. whether you want to divide up exposures perhaps for dithering the position, or to enable 
    exploitation of brief periods of best sky conditions, e.g. seeing.
 
+.. note::
+
+   An exposure time of 30 seconds, binned 2x2, will be sky-noise sky-limited
+   (sky noise ~ 3x readout noise) in the u-band even in dark time. For 1x1
+   binning the same ratio is reached in 120 seconds. There is not much to be 
+   gained in using longer exposure times than this. We do not recommend using 
+   exposure times longer than 120 seconds when binned, or 240 seconds binned 
+   1x1.
+
 For time-series observations of variable targets, considerations
 1, 2 and 3 may still apply, but you also need to decide on the
 timescale you aim to sample. Because of the dependence of the minimum
 exposure time on the setup described earlier, this timescale may drive
 later decisions.  For instance, |hiper|'s full frame, unbinned readout
 time is about 3 seconds.  If you need to go faster than this, you will
 need to bin or window. This is a trivial but common example
@@ -75,21 +87,22 @@
 #. |hiper|'s native unbinned pixel size on the GTC is just 0.081 arcseconds,
    which significantly oversamples all but the very best seeing. Thus if you
    bin 2x2, 3x3 or even 4x4, you might not lose much resolution at all.
 
 #. Binning substantially reduces the amount of data. This can allow
    you to readout the CCD faster. This could mean for example that you
    can read the entire CCD binned, whereas you would have to
-   sub-window if unbinned. This can make observing easier, and ensure
+   sub-window if unbinned. Reading the whole CCD means there are more
+   comparison stars available, makes observing easier, and ensures
    that objects are not too close to the edge of the readout
    windows.
 
 #. Binning reduces the impact of readout noise. CCD binning occurs on
    chip before readout, so readout noise is incurred per binned pixel,
-   not per native CCD pixel. This is often very important gain,
+   not per native CCD pixel. This can have a very large impact on your data,
    depending upon target and sky brightness. You should, if possible,
    define a setup that ensures that the peak target counts per binned
    pixel are substantially in excess of :math:`R^2 G` where :math:`R`
    is the RMS readout noise in counts (ADU) and :math:`G` is the gain
    in electrons per ADU. **For HiPERCAM this means one wants if possible
    at least 100 counts/pixel at peak**, and preferably higher than this.
    There is a caveat to this in that if the sky counts are greater
@@ -100,17 +113,17 @@
    sometimes to use very large binning factors when going fast and sky
    noise is low. It is this sort of case when binning can quite dramatically
    improve your data, and if you are not worried about spatial resolution
    at all, 8x8 or even 16x16 binning might make sense.
 
 Binning has downsides of course; resolution is the obvious one. If you
 need to exploit good seeing, then you may not want to go beyond 2x2
-binning (0.162 arcseconds/pixel). The other one is that you make saturation. 
-However, points 2 and 3 above mean that more often than not
-you should bin, and you should think twice before simply selecting
+binning (0.162 arcseconds/pixel). The other effect is that you are more
+likely to saturate the CCD. However, points 2 and 3 above mean that more often
+than not you should bin, and you should think twice before simply selecting
 1x1. To understand more about how one guard against readout noise, see the
 section below on condition-tolerant setups.
 
 .. Note::
 
    The binning is the same for all CCDs. There is another option for
    accounting for differences between CCDs. See the discussion of ``nskips``
@@ -125,15 +138,15 @@
 Readout modes
 =============
 
 .. _outputs:
 
 Outputs
 -------
-HiPERCAM has four seperate outputs, or channels, per CCD. The division between these
+HiPERCAM has four separate outputs, or channels, per CCD. The division between these
 outputs is clearly shown in the FoV in ``hfinder``. 
 
 .. Warning::
 
     Each output has a different gain and bias level. You **must** avoid putting critical targets on the boundary 
     between outputs.
 
@@ -154,61 +167,65 @@
 
 If there are two window quads, they cannot overlap in y.
 
 Synchronising windows
 `````````````````````
 
 If on-chip binning is enabled, it is possible to define windows that do not align with the
-boundaries of the binned pixels. This means that one cannot use
-calibration frames taken with 1x1 binning (such as sky flats) to match the windowed data.
-If windows are not synchronised in this manner, the :guilabel:`Sync` button will be enabled.
-Clicking this will align the windows with the boundaries of binned pixels.
+boundaries of the binned pixels. This means that one cannot crop binned, full-frame calibrations (such as bias frames) to apply to the windowed data. If windows are not synchronised in this manner, the :guilabel:`Sync` button will be enabled. Clicking this will align the windows with the boundaries of binned pixels.
 
 .. Warning::
 
     Unless you have requested special calibrations for your data, e.g binned sky flats, you 
     should make sure your setup is synchronised.
 
 .. _clear_mode_h:
 
 Clear mode
 ----------
 
-Sometimes extremely short exposures are needed, even with full frame data. Sky flats would be
-one example. It is possible to *clear* the image area of the CCD, just after the storage area
-is read out. This allows exposure times as short as 10 microseconds. These short exposures come
+Sometimes extremely short exposures are needed, even with full frame data. Bright standard stars would be one example. It is possible to *clear* the image area of the CCD, just after the storage area is read out. This allows exposure times as short as 10 microseconds. These short exposures come
 at the expense of efficiency, since the charge accumulated whilst the storage area was reading
 out is lost.
 
 For example, if the storage area takes 2s to read out, clear mode is enabled and the exposure delay
 is set to 1s, then an image would be take every 3s with a duty cycle of 30%.
 
-As a result, if the user needs short exposure times to avoid saturation, it is often
-preferable to use a faster readout speed, :ref:`windows_h` or :ref:`drift_mode_h` to achieve
-this without sacrificing observing efficiency.
+As a result, if the user needs short exposure times to avoid saturation, or if short exposures
+are needed for science purposes, then it is often preferable to use a faster readout speed, :ref:`windows_h` or :ref:`drift_mode_h` to achieve this without sacrificing observing efficiency.
 
 Clear mode is enabled by selecting the :guilabel:`Clear` checkbox.
 
 .. _drift_mode_h:
 
 Drift mode
 ----------
 
 Drift mode is used to enable the highest frame rates. Instead of shifting the entire image area
-into the storage area at the end of each exposure, only a small window at the bottom of the CCD
-is shifted into the storage area. This minimises the dead time involved in shifting charge to the
-storage area and allows frame rates of ~1 kHz for relatively small windows.
+into the storage area at the end of each exposure (a process that takes 7.8 milliseconds), only a small window at the bottom of the CCD is shifted into the storage area. This minimises the dead time involved in shifting charge to the storage area and allows frame rates of ~1 kHz for relatively small windows.
 
 In drift mode, a number of windows are present in the storage area at any one time. At the same
 time, any charge in pixels above the windows is eventually clocked into the windows, and becomes
 part of that frame. To prevent bright stars from contaminating the drift mode data, a blade
 is inserted into the focal plane, blocking off most of the image area of the CCD. Because the
 windows in drift mode spend longer on the chip, they accumulate dark current; drift mode should
 only be used for frame rates faster than ~10 Hz as a result.
 
+In drift mode, only two windows are read out (at the bottom of the CCD). Clear mode is not possible in combination with drift mode. 
+
+Diff-Shift
+``````````
+
+After transfer to the storage area, both windows have to be clocked horizontally to reach the readout register. Therefore the fastest speeds are obtained when the windows are in the corners
+of the CCD. If the windows are moved in from corners, it  is best to move them inwards an equal 
+amount, since otherwise the window on the side closest to the readout register will have wait until the other window reaches the readout register, slowing down the frame rate.
+
+Details 
+```````
+
 For more information about drift mode, see the
 `ULTRACAM instrument paper <https://ui.adsabs.harvard.edu/#abs/2007MNRAS.378..825D/abstract>`_
 and it's appendix.
 
 Exposure multipliers (nskips)
 =============================
 
@@ -273,14 +290,62 @@
 .. Warning::
 
    Do not place your target or comparisons close to the half-way point
    in either X or Y in full frame mode because the |hiper| CCDs are
    read out at the 4 corners and you risk your target being divided across
    multiple :ref:`outputs`.
 
+.. _compo_h:
+
+Using COMPO for better comparison stars
+---------------------------------------
+
+Sometimes there are no good comparison stars in the field of view. To
+address this issue, HiPERCAM is equipped with a COMparison PickOff (COMPO).
+
+COMPO works by using a small pick-off mirror on a rotating arm to capture
+light from a star outside the field of view. The light is then fed into 
+an injection arm which can optically place the light from the star into one corner
+of the CCD, effectively changing the on-sky position of the star. The pickoff and injection arms have a field of view of 24 arcsec.
+
+The injection arm will vignette the corner of the CCD in which is is placed.
+
+Use of COMPO is enabled using the :guilabel:`COMPO` checkbox. This brings up a 
+small COMPO widget that allows one to set the position of the injection arm and 
+the rotation angle of the pickoff arm. The current COMPO setup is also displayed,
+as shown below.
+
+.. image:: images/compo.png
+    :alt: compo display
+    :align: center
+
+The pickoff and injection arms are shown in yellow. The rectangular region shows the vignetted
+area, and the circle shows the field of view of the arms. The black line shows the path the 
+pickoff arm will take as it rotates. 
+
+By :ref:`changing the telescope PA <manip_fov_h>` and pickoff arm angle, you can place your 
+desired comparison star within the field of view of the pickoff arm. The position of the 
+injection arm is selected using the radio buttons. The options available are:
+
+.. list-table:: Injection arm options
+   :widths: 10 90
+   :header-rows: 0
+
+   * - :guilabel:`L`
+     - Position arm in lower left corner of CCD
+   * - :guilabel:`R`
+     - Position arm in lower right corner of CCD
+   * - :guilabel:`G`
+     - Position injection arm over the guide camera.
+   * - :guilabel:`P`
+     - Park injection arm out of the FoV (also parks pickoff arm).
+
+By positioning the pickoff arm over a bright star and selecting :guilabel:`G` for the injection
+arm, compo can be used as an :ref:`off-axis autoguider <guiding_h>` for long exposures.
+
 Miscellaneous settings
 ======================
 
 The remaining settings you can change are described below:
 
 Num. exposures
     The number of exposures to take before stopping. Most HiPERCAM users will want to take a
@@ -291,23 +356,58 @@
 Readout speed
     Fast readout speed reduces the minimum exposure time in full-frame readout from 2.9s to 1.2s.
     This comes at the expense of increased readout noise. The impact of this on the S/N of your
     target is shown in ``hfinder``.
 
 Fast clocks
     Users wanting the ultimate in high speed performance can enable this option. This increases the
-    rate at which charge is clocked in the CCDs. It will have an impact on charge transfer efficiency.
-    As of today, this impact has not been well characterised, but we do not think it is serious.
+    rate at which charge is clocked in the CCDs. It will have an impact on charge transfer efficiency. As of today, this impact has not been well characterised, but we do not think it is serious.
 
 Overscan
     Enable the recording of the overscan regions at the left and right edges of the chip. Can be
-    useful if precise measurement of the bias in each frame is needed. This is important for the
-    highest levels of photometric precision, so consider this option for, e.g. exoplanet transit
-    observations.
+    useful if precise measurement of the bias in each frame is needed. This can be useful for the
+    highest levels of photometric precision. If the bias level is wrong, the sky background (and
+    thus the estimated errors on the photomtry) will be wrong, so consider this option for, e.g. exoplanet transit observations.
+
+.. _guiding_h:
+
+Autoguiding
+===========
+HiPERCAM is mounted on the FC-G rotator. This instrument port has no built-in autoguider. Autoguiding 
+is therefore provided by the science instrument itself. There are two options for autoguiding: guiding
+using the science images themselves, or using :ref:`COMPO <compo_h>` as an off-axis guider.
+
+Autoguiding using the science images
+------------------------------------
+For relative short exposure times (less than around 60 seconds), the tracking of the telescope is
+adequate to provide sharp images. The best option for guiding is therefore to use the position
+of bright targets in the science images to correct for any drift in the telescope pointing. 
+This requires no setup using ``hfinder``, and is performed by the support astronomer on the night.
+
+Autoguiding using COMPO
+-----------------------
+For longer exposure times, the tracking of the telescope is not adequate to provide sharp images.
+Active autoguiding during a single exposure is required. For this purpose, :ref:`COMPO <compo_h>`
+can be used as an off-axis guider. This is enabled by selecting :guilabel:`G` for the injection
+arm and positioning the pickoff arm over your chosen guide star.
+
+.. Note::
 
+   Guide stars in the magnitude range (XX-XX) are most suitable for guiding. 
+
+.. Warning::
+
+   Many extra-galactic observations use a combination of long exposures, and :ref:`dithering <nod>`
+   to allow accurate background removal. This is possible with COMPO autoguiding, but requires that
+   the offsets between dither positions is small. The FoV of the pickoff mirror is 24 arcseconds,
+   so no offset position should be further than 10 arcseconds from the central position. 
+
+   In principle it would be possible to supply a telescope PA and pickoff angle position for each
+   dither position, to ensure the guide star is always visible when larger offsets than 10 arcsecs are required. However, this mode is not currently
+   supported (as of Summer 2023).
 
 .. _nod:
 
 Dithering the Telescope
 =======================
 
 It is possible to dither the telescope between frames. This can be useful if, for example, you
@@ -333,15 +433,15 @@
 
 If you wish to visualise the dithering pattern on the sky, pressing the ``n`` key
 will cycle through the dithering pattern.
 
 Condition-tolerant setups
 =========================
 
-If you are sure that your target will only observed with seeing close
+If you are sure that your target will only be observed with seeing close
 to 1.2" and during clear conditions, you'll have a relatively easy job
 defining a setup. Much more difficult is if the seeing could be
 anything from 1.2 to 2.5", the reason being that the peak counts could
 vary by more than a factor of 4. The key point here is probably the
 binning.  It should definitely be at least 4x4, and arguably 6x6 to
 8x8, otherwise you could end up swamping the target with readout noise
 during poor seeing. One way to think about readout noise is as the
@@ -428,14 +528,18 @@
 
 #. For blue targets, have you included a bright comparison star (if available)
    for the u-band, even if it looks too bright for the griz bands?
 
 #. For variable targets, have you considered the impact of the full range
    of their variability in terms of possible saturation or readnoise?
 
+#. If your exposure times are long (more than approx 60 seconds), have you 
+   enabled the use of COMPO, and positioned the pick-off mirror over a suitable
+   guide star?
+
 #. Is the duty cycle of your setup what you expect? For most observations
    it should be above 95%.
 
 #. Is your setup tolerant of the full range of conditions you have
    specified for it? Variations in seeing especially, can cause
    dramatic variations in peak count levels and may veer you
    towards either saturation or readout noise limitations.
```

### Comparing `hcam_finder-1.2.2/docs/images/inst.png` & `hcam_finder-1.3.0/docs/images/inst.png`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.2.2/docs/images/main.png` & `hcam_finder-1.3.0/docs/images/main.png`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.2.2/docs/make.bat` & `hcam_finder-1.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.2.2/docs/ultracam.rst` & `hcam_finder-1.3.0/docs/ultracam.rst`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.2.2/docs/usage.rst` & `hcam_finder-1.3.0/docs/usage.rst`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,16 @@
 pressing the :guilabel:`Query Simbad` button. If SIMBAD lookup fails, you can enter
 your target coordinates by hand.
 
 Select a sky survey to grab images from and press the :guilabel:`Load Image` button. If an
 image is available in the selected sky survey it will be downloaded and displayed, along with
 the HiPERCAM field of view (FoV).
 
+.. _manip_fov_h:
+
 Manipulating the FoV
 ---------------------
 
 You can change the telescope pointing either by click-dragging the FoV, or by changing the values
 in the :guilabel:`Tel. RA` and :guilabel:`Tel. Dec` fields. Like all numerical entry boxes in ``hfinder``
 the right and left arrow keys will increment or decrement the values. Holding :kbd:`Shift` whilst
 pressing the arrow keys will make larger changes.
```

### Comparing `hcam_finder-1.2.2/hcam_finder/config.py` & `hcam_finder-1.3.0/hcam_finder/config.py`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.2.2/hcam_finder/data/Lato-Black.ttf` & `hcam_finder-1.3.0/hcam_finder/data/Lato-Black.ttf`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.2.2/hcam_finder/data/Lato-Regular.ttf` & `hcam_finder-1.3.0/hcam_finder/data/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.2.2/hcam_finder/data/config` & `hcam_finder-1.3.0/hcam_finder/data/config`

 * *Files 0% similar despite different names*

```diff
@@ -77,16 +77,16 @@
 # rotator position in degrees when chip runs N-S
 paOff = 1.7
 
 [GTC]
 px_scale = 0.081
 nxtot = 2048
 nytot = 1024
-rotcen_x = 1020.0
-rotcen_y = 524.0
+rotcen_x = 1027.0
+rotcen_y = 520.0
 # is image flipped E-W?
 flipEW = True
 # does increasing PA rotate towards east from north?
 EofN = True
 # rotator position in degrees when chip runs N-S
 paOff = 0
```

### Comparing `hcam_finder-1.2.2/hcam_finder/data/configspec.ini` & `hcam_finder-1.3.0/hcam_finder/data/configspec.ini`

 * *Files 1% similar despite different names*

```diff
@@ -69,16 +69,16 @@
 # rotator position in degrees when LHS of chip runs N-S
 paOff = float(default=0.0)
 
 [GTC]
 px_scale =  float(default=0.081)
 nxtot = integer(default=2048)
 nytot = integer(default=1024)
-rotcen_x = float(default=1020.0)
-rotcen_y = float(default=524.0)
+rotcen_x = float(default=1027.0)
+rotcen_y = float(default=520.0)
 # is image flipped E-W?
 flipEW = boolean(default=True)
 # does increasing PA rotate towards east from north?
 EofN = boolean(default=True)
 # rotator position in degrees when LHS of chip runs N-S
 paOff = float(default=0)
```

### Comparing `hcam_finder-1.2.2/hcam_finder/data/guider_hole_arcseconds.txt` & `hcam_finder-1.3.0/hcam_finder/data/guider_hole_arcseconds.txt`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.2.2/hcam_finder/finders.py` & `hcam_finder-1.3.0/hcam_finder/finders.py`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.2.2/hcam_finder/finding_chart.py` & `hcam_finder-1.3.0/hcam_finder/finding_chart.py`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.2.2/hcam_finder/hcam_finder.py` & `hcam_finder-1.3.0/hcam_finder/hcam_finder.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     PickoffArm,
     INJECTOR_THETA,
     PARK_POSITION,
 )
 from hcam_widgets.tkutils import get_root
 
 from .finders import FovSetter
-from .shapes import CompoPatrolArc, CompoFreeRegion
+from .shapes import CompoPatrolArc
 
 if not six.PY3:
     import tkFileDialog as filedialog
 else:
     from tkinter import filedialog
 
 
@@ -61,14 +61,17 @@
             print("Aborted save to disk")
             return False
 
         g = get_root(self).globals
         data = dict()
         data["appdata"] = g.ipars.dumpJSON()
 
+        # add compo setup info
+        data["compo"] = g.compo_hw.dumpJSON()
+
         # add user info that we should know of
         # includes target, user and proposal
         user = dict()
         user["target"] = self.targName.value()
         data["user"] = user
 
         # target info
@@ -128,14 +131,18 @@
         xc, yc = image.radectopix(self.ra_as_drawn, self.dec_as_drawn)
         xn, yn = image.radectopix(ra, dec)
         # update latest dither centre
         self.ra_as_drawn, self.dec_as_drawn = ra, dec
 
         obj = self.canvas.get_object_by_tag("ccd_overlay")
         obj.move_delta(xn - xc, yn - yc)
+
+        obj = self.canvas.get_object_by_tag("compo_overlay")
+        obj.move_delta(xn - xc, yn - yc)
+        
         self.canvas.update_canvas()
 
     def _make_ccd(self, image):
         """
         Converts the current instrument settings to a ginga canvas object
         """
         # get window pair object from top widget
@@ -215,39 +222,30 @@
         compo_angle = g.compo_hw.setup_frame.pickoff_angle.value()
         compo_side = g.compo_hw.setup_frame.injection_side.value()
 
         # get chip coordinates - COMPO is aligned to chip
         chip_ctr_ra, chip_ctr_dec = self._chip_cen()
 
         if compo_side == "R":
-            ia = -INJECTOR_THETA
-        elif compo_side == "L":
             ia = INJECTOR_THETA
+        elif compo_side == "L":
+            ia = -INJECTOR_THETA
         else:
             ia = PARK_POSITION
 
         # add COMPO components
         compo_arc = CompoPatrolArc(
             chip_ctr_ra,
             chip_ctr_dec,
             image,
             linewidth=10,
             color="black",
             linestyle="dash",
             name="COMPO_Arc",
         )
-        compo_free = CompoFreeRegion(
-            chip_ctr_ra,
-            chip_ctr_dec,
-            image,
-            fill=True,
-            fillcolor="green",
-            fillalpha=0.1,
-            name="compo_free_region",
-        )
 
         compo_pickoff = PickoffArm().to_ginga_object(
             compo_angle * u.deg,
             chip_ctr_ra * u.deg,
             chip_ctr_dec * u.deg,
             fill=True,
             fillcolor="yellow",
@@ -261,15 +259,15 @@
             chip_ctr_dec * u.deg,
             color="yellow",
             fillalpha=0.3,
             fill=True,
             name="COMPO_injector",
         )
 
-        obl = [compo_arc, compo_free, compo_pickoff, compo_injector]
+        obl = [compo_arc, compo_pickoff, compo_injector]
         obj = CompoundObject(*obl)
         obj.editable = True
         return obj
 
     def draw_ccd(self, *args):
         image = self.fitsimage.get_image()
         if image is None:
```

### Comparing `hcam_finder-1.2.2/hcam_finder/panstarrs.py` & `hcam_finder-1.3.0/hcam_finder/panstarrs.py`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.2.2/hcam_finder/shapes.py` & `hcam_finder-1.3.0/hcam_finder/shapes.py`

 * *Files 12% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         Parameters
         ----------
         ra_ctr_deg, dec_ctr_deg : float
               Tel pointing center (deg)
         image : `~ginga.AstroImage`
               image to plot Window on
         """
-        # assume patrol arc of 90 degrees
+        
         theta = np.linspace(-65, 65, 40)*u.deg
 
         # circular arc, swapping dec sign
         X, Y = field_stop_centre(theta)
         points = u.Quantity([X, -Y])
         # transform to shape (N, 2) and units of degrees
         with u.set_enabled_equivalencies(gtc_focalplane_equivalencies):
@@ -67,28 +67,7 @@
         ]
 
         self.points = [image.radectopix(ra, dec) for (ra, dec) in points_wcs]
         self.bezier = get_bezier(30, self.points)
         super(CompoPatrolArc, self).__init__(self.points, **params)
         self.name = params.pop('name', 'patrol_arc')
 
-
-class CompoFreeRegion(Polygon):
-    def __init__(self, ra_ctr_deg, dec_ctr_deg, image, **params):
-        """
-        Shape for drawing unvignetted area available to patrol arm
-
-        Parameters
-        ----------
-        ra_ctr_deg, dec_ctr_deg : float
-              Tel pointing center (deg)
-        image : `~ginga.AstroImage`
-              image to plot Window on
-        """
-        guider_file = pkg_resources.resource_filename('hcam_finder',
-                                                      'data/guider_hole_arcseconds.txt')
-        points = np.loadtxt(guider_file) / 36000
-        points_wcs = [wcs.add_offset_radec(ra_ctr_deg, dec_ctr_deg, p[0], p[1]) for p in points]
-        self.points = [image.radectopix(ra, dec) for (ra, dec) in points_wcs]
-        self.bezier = get_bezier(30, self.points)
-        super(CompoFreeRegion, self).__init__(self.bezier, **params)
-        self.name = params.pop('name', 'compo_free_region')
```

### Comparing `hcam_finder-1.2.2/hcam_finder/skyview.py` & `hcam_finder-1.3.0/hcam_finder/skyview.py`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.2.2/hcam_finder/ucam_finder.py` & `hcam_finder-1.3.0/hcam_finder/ucam_finder.py`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.2.2/hcam_finder/uspec_finder.py` & `hcam_finder-1.3.0/hcam_finder/uspec_finder.py`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.2.2/hcam_finder/ztf.py` & `hcam_finder-1.3.0/hcam_finder/ztf.py`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.2.2/hcam_finder.egg-info/PKG-INFO` & `hcam_finder-1.3.0/hcam_finder.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: hcam-finder
-Version: 1.2.2
+Version: 1.3.0
 Summary: Observation planning and finding charts for HiPerCAM
 Home-page: https://github.com/HiPERCAM/hcam_finder
-Download-URL: https://github.com/HiPERCAM/hcam_finder/archive/v1.2.2.tar.gz
+Download-URL: https://github.com/HiPERCAM/hcam_finder/archive/v1.3.0.tar.gz
 Author: Stuart Littlefair
 Author-email: s.littlefair@shef.ac.uk
 License: MIT license
 Keywords: hcam_finder
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hcam_finder-1.2.2/hcam_finder.egg-info/SOURCES.txt` & `hcam_finder-1.3.0/hcam_finder.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 docs/hipercam.rst
 docs/index.rst
 docs/make.bat
 docs/modules.rst
 docs/ultracam.rst
 docs/ultraspec.rst
 docs/usage.rst
+docs/_build/html/_images/compo.png
 docs/_build/html/_images/inst.png
 docs/_build/html/_images/main.png
 docs/_build/html/_static/file.png
 docs/_build/html/_static/minus.png
 docs/_build/html/_static/plus.png
+docs/images/compo.png
 docs/images/inst.png
 docs/images/main.png
 hcam_finder/__init__.py
 hcam_finder/config.py
 hcam_finder/finders.py
 hcam_finder/finding_chart.py
 hcam_finder/hcam_finder.py
```

### Comparing `hcam_finder-1.2.2/scripts/hfinder` & `hcam_finder-1.3.0/scripts/hfinder`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.2.2/scripts/ufinder` & `hcam_finder-1.3.0/scripts/ufinder`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.2.2/scripts/usfinder` & `hcam_finder-1.3.0/scripts/usfinder`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.2.2/setup.py` & `hcam_finder-1.3.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,66 +1,61 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 from setuptools import setup
 import glob
 import os
 
-with open('README.rst') as readme_file:
+with open("README.rst") as readme_file:
     readme = readme_file.read()
 
-with open('HISTORY.rst') as history_file:
+with open("HISTORY.rst") as history_file:
     history = history_file.read()
 
-requirements = [
-    'ginga',
-    'astropy',
-    'six',
-    'pillow',
-    'configobj',
-    'hcam_widgets>=1.0.0'
-]
+requirements = ["ginga", "astropy", "six", "pillow", "configobj", "hcam_widgets>=1.1.0"]
 
 test_requirements = [
     # TODO: put package test requirements here
 ]
 
 # Treat everything in scripts except README.rst as a script to be installed
-scripts = [fname for fname in glob.glob(os.path.join('scripts', '*'))
-           if os.path.basename(fname) != 'README.rst']
+scripts = [
+    fname
+    for fname in glob.glob(os.path.join("scripts", "*"))
+    if os.path.basename(fname) != "README.rst"
+]
 
 setup(
-    name='hcam_finder',
-    version='1.2.2',
+    name="hcam_finder",
+    version="1.3.0",
     description="Observation planning and finding charts for HiPerCAM",
-    long_description=readme + '\n\n' + history,
+    long_description=readme + "\n\n" + history,
     author="Stuart Littlefair",
-    author_email='s.littlefair@shef.ac.uk',
-    url='https://github.com/HiPERCAM/hcam_finder',
-    download_url='https://github.com/HiPERCAM/hcam_finder/archive/v1.2.2.tar.gz',
+    author_email="s.littlefair@shef.ac.uk",
+    url="https://github.com/HiPERCAM/hcam_finder",
+    download_url="https://github.com/HiPERCAM/hcam_finder/archive/v1.3.0.tar.gz",
     packages=[
-        'hcam_finder',
+        "hcam_finder",
     ],
-    package_dir={'hcam_finder':
-                 'hcam_finder'},
+    package_dir={"hcam_finder": "hcam_finder"},
     include_package_data=True,
     scripts=scripts,
     install_requires=requirements,
     license="MIT license",
     zip_safe=False,
-    keywords='hcam_finder',
+    keywords="hcam_finder",
     classifiers=[
-        'Development Status :: 2 - Pre-Alpha',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
-        'Natural Language :: English',
+        "Development Status :: 2 - Pre-Alpha",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: MIT License",
+        "Natural Language :: English",
         "Programming Language :: Python :: 2",
-        'Programming Language :: Python :: 2.6',
-        'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.3',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
+        "Programming Language :: Python :: 2.6",
+        "Programming Language :: Python :: 2.7",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.3",
+        "Programming Language :: Python :: 3.4",
+        "Programming Language :: Python :: 3.5",
     ],
-    test_suite='tests',
-    tests_require=test_requirements
+    test_suite="tests",
+    tests_require=test_requirements,
 )
```

### Comparing `hcam_finder-1.2.2/tests/test_hcam_finder.py` & `hcam_finder-1.3.0/tests/test_hcam_finder.py`

 * *Files identical despite different names*

