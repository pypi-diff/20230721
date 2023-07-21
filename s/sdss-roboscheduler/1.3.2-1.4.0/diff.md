# Comparing `tmp/sdss-roboscheduler-1.3.2.tar.gz` & `tmp/sdss-roboscheduler-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sdss-roboscheduler-1.3.2.tar", last modified: Mon Jan 30 17:36:02 2023, max compression
+gzip compressed data, was "sdss-roboscheduler-1.4.0.tar", last modified: Fri Jul 21 14:43:06 2023, max compression
```

## Comparing `sdss-roboscheduler-1.3.2.tar` & `sdss-roboscheduler-1.4.0.tar`

### file list

```diff
@@ -1,76 +1,81 @@
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-01-30 17:36:02.000000 sdss-roboscheduler-1.3.2/
--rw-r--r--   0 john      (1000) john      (1000)     1504 2020-01-24 18:08:13.000000 sdss-roboscheduler-1.3.2/LICENSE.md
--rw-rw-r--   0 john      (1000) john      (1000)       73 2021-08-23 20:53:04.000000 sdss-roboscheduler-1.3.2/MANIFEST.in
--rw-rw-r--   0 john      (1000) john      (1000)     1625 2023-01-30 17:36:02.000000 sdss-roboscheduler-1.3.2/PKG-INFO
--rw-r--r--   0 john      (1000) john      (1000)      758 2020-01-24 18:08:13.000000 sdss-roboscheduler-1.3.2/README.rst
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-01-30 17:36:02.000000 sdss-roboscheduler-1.3.2/bin/
--rwxrwxr-x   0 john      (1000) john      (1000)     6027 2021-11-29 21:13:50.000000 sdss-roboscheduler-1.3.2/bin/make_ms
--rw-rw-r--   0 john      (1000) john      (1000)     1645 2022-04-11 18:34:46.000000 sdss-roboscheduler-1.3.2/bin/night_length
--rwxrwxr-x   0 john      (1000) john      (1000)       99 2021-11-29 21:15:50.000000 sdss-roboscheduler-1.3.2/bin/roboschedulerversion.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-01-30 17:36:02.000000 sdss-roboscheduler-1.3.2/cextern/
--rw-r--r--   0 john      (1000) john      (1000)        0 2021-01-14 18:45:08.000000 sdss-roboscheduler-1.3.2/cextern/Makefile
--rw-r--r--   0 john      (1000) john      (1000)       42 2020-01-24 18:08:13.000000 sdss-roboscheduler-1.3.2/cextern/README.txt
--rw-rw-r--   0 john      (1000) john      (1000)     1805 2021-11-12 20:04:29.000000 sdss-roboscheduler-1.3.2/cextern/cCadenceCore.cpp
--rw-rw-r--   0 john      (1000) john      (1000)     9432 2021-11-12 20:04:29.000000 sdss-roboscheduler-1.3.2/cextern/cadenceCore.cpp
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-01-30 17:36:02.000000 sdss-roboscheduler-1.3.2/include/
--rw-rw-r--   0 john      (1000) john      (1000)     1441 2021-11-12 20:04:29.000000 sdss-roboscheduler-1.3.2/include/cadenceCore.h
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-01-30 17:36:02.000000 sdss-roboscheduler-1.3.2/python/
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-01-30 17:36:02.000000 sdss-roboscheduler-1.3.2/python/roboscheduler/
--rw-rw-r--   0 john      (1000) john      (1000)     1322 2023-01-30 17:33:19.000000 sdss-roboscheduler-1.3.2/python/roboscheduler/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)    37015 2023-01-25 22:16:43.000000 sdss-roboscheduler-1.3.2/python/roboscheduler/cadence.py
--rw-r--r--   0 john      (1000) john      (1000)    34796 2020-01-24 18:08:13.000000 sdss-roboscheduler-1.3.2/python/roboscheduler/coords.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-01-30 17:36:02.000000 sdss-roboscheduler-1.3.2/python/roboscheduler/core/
--rw-r--r--   0 john      (1000) john      (1000)        0 2020-01-24 18:08:13.000000 sdss-roboscheduler-1.3.2/python/roboscheduler/core/__init__.py
--rw-r--r--   0 john      (1000) john      (1000)     1979 2020-01-24 18:08:13.000000 sdss-roboscheduler-1.3.2/python/roboscheduler/core/exceptions.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-01-30 17:36:02.000000 sdss-roboscheduler-1.3.2/python/roboscheduler/etc/
--rw-rw-r--   0 john      (1000) john      (1000)     6275 2021-08-23 20:53:04.000000 sdss-roboscheduler-1.3.2/python/roboscheduler/etc/master_schedule_apo_gamma.par
--rw-rw-r--   0 john      (1000) john      (1000)      941 2021-08-23 20:53:04.000000 sdss-roboscheduler-1.3.2/python/roboscheduler/etc/master_schedule_apo_maximal.par
--rw-rw-r--   0 john      (1000) john      (1000)     6786 2021-08-23 20:53:04.000000 sdss-roboscheduler-1.3.2/python/roboscheduler/etc/master_schedule_apo_maximal_v2.par
--rw-rw-r--   0 john      (1000) john      (1000)     8144 2021-10-25 17:35:42.000000 sdss-roboscheduler-1.3.2/python/roboscheduler/etc/master_schedule_apo_maximal_v3.par
--rw-rw-r--   0 john      (1000) john      (1000)     5509 2021-08-23 20:53:04.000000 sdss-roboscheduler-1.3.2/python/roboscheduler/etc/master_schedule_apo_may21.par
--rw-rw-r--   0 john      (1000) john      (1000)     4803 2021-08-23 20:53:04.000000 sdss-roboscheduler-1.3.2/python/roboscheduler/etc/master_schedule_apo_minimal.par
--rw-rw-r--   0 john      (1000) john      (1000)     6275 2021-08-23 20:53:04.000000 sdss-roboscheduler-1.3.2/python/roboscheduler/etc/master_schedule_apo_normal.par
--rw-rw-r--   0 john      (1000) john      (1000)     5533 2021-08-23 20:53:04.000000 sdss-roboscheduler-1.3.2/python/roboscheduler/etc/master_schedule_apo_normal_v2.par
--rw-rw-r--   0 john      (1000) john      (1000)     6576 2021-10-25 17:35:42.000000 sdss-roboscheduler-1.3.2/python/roboscheduler/etc/master_schedule_apo_normal_v3.par
--rw-rw-r--   0 john      (1000) john      (1000)     6639 2022-02-10 16:10:21.000000 sdss-roboscheduler-1.3.2/python/roboscheduler/etc/master_schedule_apo_normal_v4.par
--rw-rw-r--   0 john      (1000) john      (1000)     6639 2022-10-12 16:42:56.000000 sdss-roboscheduler-1.3.2/python/roboscheduler/etc/master_schedule_apo_normal_v5.par
--rw-rw-r--   0 john      (1000) john      (1000)     1659 2021-08-23 20:53:04.000000 sdss-roboscheduler-1.3.2/python/roboscheduler/etc/master_schedule_apo_plates.par
--rw-rw-r--   0 john      (1000) john      (1000)     1669 2021-10-12 19:39:21.000000 sdss-roboscheduler-1.3.2/python/roboscheduler/etc/master_schedule_apo_test.par
--rw-rw-r--   0 john      (1000) john      (1000)     6805 2021-08-23 20:53:04.000000 sdss-roboscheduler-1.3.2/python/roboscheduler/etc/master_schedule_lco_gamma.par
--rw-rw-r--   0 john      (1000) john      (1000)      540 2021-08-23 20:53:04.000000 sdss-roboscheduler-1.3.2/python/roboscheduler/etc/master_schedule_lco_maximal.par
--rw-rw-r--   0 john      (1000) john      (1000)    10890 2021-08-23 20:53:04.000000 sdss-roboscheduler-1.3.2/python/roboscheduler/etc/master_schedule_lco_maximal_v2.par
--rw-rw-r--   0 john      (1000) john      (1000)    13430 2021-10-25 17:35:42.000000 sdss-roboscheduler-1.3.2/python/roboscheduler/etc/master_schedule_lco_maximal_v3.par
--rw-rw-r--   0 john      (1000) john      (1000)     5881 2021-08-23 20:53:04.000000 sdss-roboscheduler-1.3.2/python/roboscheduler/etc/master_schedule_lco_may21.par
--rw-rw-r--   0 john      (1000) john      (1000)     4955 2021-08-23 20:53:04.000000 sdss-roboscheduler-1.3.2/python/roboscheduler/etc/master_schedule_lco_minimal.par
--rw-rw-r--   0 john      (1000) john      (1000)     6819 2021-08-23 20:53:04.000000 sdss-roboscheduler-1.3.2/python/roboscheduler/etc/master_schedule_lco_normal.par
--rw-rw-r--   0 john      (1000) john      (1000)     8665 2021-08-23 20:53:04.000000 sdss-roboscheduler-1.3.2/python/roboscheduler/etc/master_schedule_lco_normal_v2.par
--rw-rw-r--   0 john      (1000) john      (1000)    10680 2021-10-25 17:35:42.000000 sdss-roboscheduler-1.3.2/python/roboscheduler/etc/master_schedule_lco_normal_v3.par
--rw-rw-r--   0 john      (1000) john      (1000)    10680 2022-02-08 19:26:39.000000 sdss-roboscheduler-1.3.2/python/roboscheduler/etc/master_schedule_lco_normal_v4.par
--rw-rw-r--   0 john      (1000) john      (1000)     2095 2021-10-12 19:39:21.000000 sdss-roboscheduler-1.3.2/python/roboscheduler/etc/master_schedule_lco_test.par
--rw-rw-r--   0 john      (1000) john      (1000)      172 2021-08-23 20:53:04.000000 sdss-roboscheduler-1.3.2/python/roboscheduler/etc/observatories.par
--rw-r--r--   0 john      (1000) john      (1000)      123 2020-01-24 18:08:13.000000 sdss-roboscheduler-1.3.2/python/roboscheduler/etc/roboscheduler.yml
--rw-rw-r--   0 john      (1000) john      (1000)      434 2021-11-29 19:55:34.000000 sdss-roboscheduler-1.3.2/python/roboscheduler/etc/sch_head.txt
--rw-rw-r--   0 john      (1000) john      (1000)    15159 2022-10-12 16:42:56.000000 sdss-roboscheduler-1.3.2/python/roboscheduler/fields.py
--rw-rw-r--   0 john      (1000) john      (1000)     2242 2021-06-30 18:24:57.000000 sdss-roboscheduler-1.3.2/python/roboscheduler/ks91.py
--rw-r--r--   0 john      (1000) john      (1000)     1929 2020-01-24 18:08:13.000000 sdss-roboscheduler-1.3.2/python/roboscheduler/moonphase.py
--rw-rw-r--   0 john      (1000) john      (1000)     6289 2022-01-07 04:04:12.000000 sdss-roboscheduler-1.3.2/python/roboscheduler/observations.py
--rw-rw-r--   0 john      (1000) john      (1000)    49317 2023-01-25 22:16:43.000000 sdss-roboscheduler-1.3.2/python/roboscheduler/scheduler.py
--rw-r--r--   0 john      (1000) john      (1000)     9266 2020-01-24 18:08:13.000000 sdss-roboscheduler-1.3.2/python/roboscheduler/sunpos2.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-01-30 17:36:02.000000 sdss-roboscheduler-1.3.2/python/roboscheduler/tests/
--rw-r--r--   0 john      (1000) john      (1000)        0 2020-01-24 18:08:13.000000 sdss-roboscheduler-1.3.2/python/roboscheduler/tests/__init__.py
--rw-r--r--   0 john      (1000) john      (1000)      639 2021-01-20 21:14:52.000000 sdss-roboscheduler-1.3.2/python/roboscheduler/tests/conftest.py
--rw-r--r--   0 john      (1000) john      (1000)     6060 2020-01-24 18:08:13.000000 sdss-roboscheduler-1.3.2/python/roboscheduler/tests/test_cadence.py
--rw-r--r--   0 john      (1000) john      (1000)     4290 2021-01-20 21:14:52.000000 sdss-roboscheduler-1.3.2/python/roboscheduler/tests/test_packing.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-01-30 17:36:02.000000 sdss-roboscheduler-1.3.2/python/roboscheduler/utils/
--rw-r--r--   0 john      (1000) john      (1000)       23 2020-01-24 18:08:13.000000 sdss-roboscheduler-1.3.2/python/roboscheduler/utils/__init__.py
--rw-r--r--   0 john      (1000) john      (1000)     6472 2020-01-24 18:08:13.000000 sdss-roboscheduler-1.3.2/python/roboscheduler/utils/color_print.py
--rw-r--r--   0 john      (1000) john      (1000)     6165 2020-01-24 18:08:13.000000 sdss-roboscheduler-1.3.2/python/roboscheduler/utils/logger.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-01-30 17:36:02.000000 sdss-roboscheduler-1.3.2/python/sdss_roboscheduler.egg-info/
--rw-rw-r--   0 john      (1000) john      (1000)     1625 2023-01-30 17:36:02.000000 sdss-roboscheduler-1.3.2/python/sdss_roboscheduler.egg-info/PKG-INFO
--rw-rw-r--   0 john      (1000) john      (1000)     2662 2023-01-30 17:36:02.000000 sdss-roboscheduler-1.3.2/python/sdss_roboscheduler.egg-info/SOURCES.txt
--rw-rw-r--   0 john      (1000) john      (1000)        1 2023-01-30 17:36:02.000000 sdss-roboscheduler-1.3.2/python/sdss_roboscheduler.egg-info/dependency_links.txt
--rw-rw-r--   0 john      (1000) john      (1000)        1 2021-08-23 20:48:43.000000 sdss-roboscheduler-1.3.2/python/sdss_roboscheduler.egg-info/not-zip-safe
--rw-rw-r--   0 john      (1000) john      (1000)      209 2023-01-30 17:36:02.000000 sdss-roboscheduler-1.3.2/python/sdss_roboscheduler.egg-info/requires.txt
--rw-rw-r--   0 john      (1000) john      (1000)       14 2023-01-30 17:36:02.000000 sdss-roboscheduler-1.3.2/python/sdss_roboscheduler.egg-info/top_level.txt
--rw-rw-r--   0 john      (1000) john      (1000)     1424 2023-01-30 17:36:02.000000 sdss-roboscheduler-1.3.2/setup.cfg
--rw-rw-r--   0 john      (1000) john      (1000)     1236 2021-08-23 20:53:04.000000 sdss-roboscheduler-1.3.2/setup.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-07-21 14:43:06.186611 sdss-roboscheduler-1.4.0/
+-rw-r--r--   0 john      (1000) john      (1000)     1504 2023-05-09 16:48:00.000000 sdss-roboscheduler-1.4.0/LICENSE.md
+-rw-rw-r--   0 john      (1000) john      (1000)       73 2023-05-09 16:48:00.000000 sdss-roboscheduler-1.4.0/MANIFEST.in
+-rw-rw-r--   0 john      (1000) john      (1000)     1676 2023-07-21 14:43:06.186611 sdss-roboscheduler-1.4.0/PKG-INFO
+-rw-r--r--   0 john      (1000) john      (1000)      758 2023-05-09 16:48:00.000000 sdss-roboscheduler-1.4.0/README.rst
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-07-21 14:43:06.182611 sdss-roboscheduler-1.4.0/bin/
+-rwxrwxr-x   0 john      (1000) john      (1000)     6027 2023-05-09 16:48:00.000000 sdss-roboscheduler-1.4.0/bin/make_ms
+-rw-rw-r--   0 john      (1000) john      (1000)     1645 2023-05-09 16:48:00.000000 sdss-roboscheduler-1.4.0/bin/night_length
+-rwxrwxr-x   0 john      (1000) john      (1000)       99 2023-05-09 16:48:00.000000 sdss-roboscheduler-1.4.0/bin/roboschedulerversion.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-07-21 14:43:06.182611 sdss-roboscheduler-1.4.0/cextern/
+-rw-r--r--   0 john      (1000) john      (1000)        0 2023-05-09 16:48:00.000000 sdss-roboscheduler-1.4.0/cextern/Makefile
+-rw-r--r--   0 john      (1000) john      (1000)       42 2023-05-09 16:48:00.000000 sdss-roboscheduler-1.4.0/cextern/README.txt
+-rw-rw-r--   0 john      (1000) john      (1000)     1805 2023-05-09 16:48:00.000000 sdss-roboscheduler-1.4.0/cextern/cCadenceCore.cpp
+-rw-rw-r--   0 john      (1000) john      (1000)     9432 2023-05-09 16:48:00.000000 sdss-roboscheduler-1.4.0/cextern/cadenceCore.cpp
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-07-21 14:43:06.182611 sdss-roboscheduler-1.4.0/include/
+-rw-rw-r--   0 john      (1000) john      (1000)     1441 2023-05-09 16:48:01.000000 sdss-roboscheduler-1.4.0/include/cadenceCore.h
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-07-21 14:43:06.182611 sdss-roboscheduler-1.4.0/python/
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-07-21 14:43:06.182611 sdss-roboscheduler-1.4.0/python/roboscheduler/
+-rw-rw-r--   0 john      (1000) john      (1000)     1322 2023-07-21 14:39:05.000000 sdss-roboscheduler-1.4.0/python/roboscheduler/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)    37189 2023-07-19 15:17:18.000000 sdss-roboscheduler-1.4.0/python/roboscheduler/cadence.py
+-rw-r--r--   0 john      (1000) john      (1000)    34796 2023-05-09 16:48:00.000000 sdss-roboscheduler-1.4.0/python/roboscheduler/coords.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-07-21 14:43:06.182611 sdss-roboscheduler-1.4.0/python/roboscheduler/core/
+-rw-r--r--   0 john      (1000) john      (1000)        0 2023-05-09 16:48:00.000000 sdss-roboscheduler-1.4.0/python/roboscheduler/core/__init__.py
+-rw-r--r--   0 john      (1000) john      (1000)     1979 2023-05-09 16:48:00.000000 sdss-roboscheduler-1.4.0/python/roboscheduler/core/exceptions.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-07-21 14:43:06.186611 sdss-roboscheduler-1.4.0/python/roboscheduler/etc/
+-rw-rw-r--   0 john      (1000) john      (1000)     6275 2023-05-09 16:48:00.000000 sdss-roboscheduler-1.4.0/python/roboscheduler/etc/master_schedule_apo_gamma.par
+-rw-rw-r--   0 john      (1000) john      (1000)      941 2023-05-09 16:48:00.000000 sdss-roboscheduler-1.4.0/python/roboscheduler/etc/master_schedule_apo_maximal.par
+-rw-rw-r--   0 john      (1000) john      (1000)     6786 2023-05-09 16:48:00.000000 sdss-roboscheduler-1.4.0/python/roboscheduler/etc/master_schedule_apo_maximal_v2.par
+-rw-rw-r--   0 john      (1000) john      (1000)     8144 2023-05-09 16:48:00.000000 sdss-roboscheduler-1.4.0/python/roboscheduler/etc/master_schedule_apo_maximal_v3.par
+-rw-rw-r--   0 john      (1000) john      (1000)     5509 2023-05-09 16:48:00.000000 sdss-roboscheduler-1.4.0/python/roboscheduler/etc/master_schedule_apo_may21.par
+-rw-rw-r--   0 john      (1000) john      (1000)     4803 2023-05-09 16:48:00.000000 sdss-roboscheduler-1.4.0/python/roboscheduler/etc/master_schedule_apo_minimal.par
+-rw-rw-r--   0 john      (1000) john      (1000)     6275 2023-05-09 16:48:00.000000 sdss-roboscheduler-1.4.0/python/roboscheduler/etc/master_schedule_apo_normal.par
+-rw-rw-r--   0 john      (1000) john      (1000)     5533 2023-05-09 16:48:00.000000 sdss-roboscheduler-1.4.0/python/roboscheduler/etc/master_schedule_apo_normal_v2.par
+-rw-rw-r--   0 john      (1000) john      (1000)     6576 2023-05-09 16:48:00.000000 sdss-roboscheduler-1.4.0/python/roboscheduler/etc/master_schedule_apo_normal_v3.par
+-rw-rw-r--   0 john      (1000) john      (1000)     6639 2023-05-09 16:48:00.000000 sdss-roboscheduler-1.4.0/python/roboscheduler/etc/master_schedule_apo_normal_v4.par
+-rw-rw-r--   0 john      (1000) john      (1000)     6639 2023-05-09 16:48:00.000000 sdss-roboscheduler-1.4.0/python/roboscheduler/etc/master_schedule_apo_normal_v5.par
+-rw-rw-r--   0 john      (1000) john      (1000)     1659 2023-05-09 16:48:00.000000 sdss-roboscheduler-1.4.0/python/roboscheduler/etc/master_schedule_apo_plates.par
+-rw-rw-r--   0 john      (1000) john      (1000)     1669 2023-05-09 16:48:00.000000 sdss-roboscheduler-1.4.0/python/roboscheduler/etc/master_schedule_apo_test.par
+-rw-rw-r--   0 john      (1000) john      (1000)     6681 2023-07-19 16:23:34.000000 sdss-roboscheduler-1.4.0/python/roboscheduler/etc/master_schedule_apo_v6.par
+-rw-rw-r--   0 john      (1000) john      (1000)     6805 2023-05-09 16:48:00.000000 sdss-roboscheduler-1.4.0/python/roboscheduler/etc/master_schedule_lco_gamma.par
+-rw-rw-r--   0 john      (1000) john      (1000)      540 2023-05-09 16:48:00.000000 sdss-roboscheduler-1.4.0/python/roboscheduler/etc/master_schedule_lco_maximal.par
+-rw-rw-r--   0 john      (1000) john      (1000)    10890 2023-05-09 16:48:00.000000 sdss-roboscheduler-1.4.0/python/roboscheduler/etc/master_schedule_lco_maximal_v2.par
+-rw-rw-r--   0 john      (1000) john      (1000)    13430 2023-05-09 16:48:00.000000 sdss-roboscheduler-1.4.0/python/roboscheduler/etc/master_schedule_lco_maximal_v3.par
+-rw-rw-r--   0 john      (1000) john      (1000)     5881 2023-05-09 16:48:00.000000 sdss-roboscheduler-1.4.0/python/roboscheduler/etc/master_schedule_lco_may21.par
+-rw-rw-r--   0 john      (1000) john      (1000)     4955 2023-05-09 16:48:00.000000 sdss-roboscheduler-1.4.0/python/roboscheduler/etc/master_schedule_lco_minimal.par
+-rw-rw-r--   0 john      (1000) john      (1000)     6819 2023-05-09 16:48:00.000000 sdss-roboscheduler-1.4.0/python/roboscheduler/etc/master_schedule_lco_normal.par
+-rw-rw-r--   0 john      (1000) john      (1000)     8665 2023-05-09 16:48:00.000000 sdss-roboscheduler-1.4.0/python/roboscheduler/etc/master_schedule_lco_normal_v2.par
+-rw-rw-r--   0 john      (1000) john      (1000)    10680 2023-05-09 16:48:00.000000 sdss-roboscheduler-1.4.0/python/roboscheduler/etc/master_schedule_lco_normal_v3.par
+-rw-rw-r--   0 john      (1000) john      (1000)    10680 2023-05-09 16:48:00.000000 sdss-roboscheduler-1.4.0/python/roboscheduler/etc/master_schedule_lco_normal_v4.par
+-rw-rw-r--   0 john      (1000) john      (1000)     2095 2023-05-09 16:48:00.000000 sdss-roboscheduler-1.4.0/python/roboscheduler/etc/master_schedule_lco_test.par
+-rw-rw-r--   0 john      (1000) john      (1000)    10660 2023-07-20 22:20:04.000000 sdss-roboscheduler-1.4.0/python/roboscheduler/etc/master_schedule_lco_v6.par
+-rw-rw-r--   0 john      (1000) john      (1000)      172 2023-05-09 16:48:00.000000 sdss-roboscheduler-1.4.0/python/roboscheduler/etc/observatories.par
+-rw-r--r--   0 john      (1000) john      (1000)      123 2023-05-09 16:48:00.000000 sdss-roboscheduler-1.4.0/python/roboscheduler/etc/roboscheduler.yml
+-rw-rw-r--   0 john      (1000) john      (1000)      434 2023-05-09 16:48:00.000000 sdss-roboscheduler-1.4.0/python/roboscheduler/etc/sch_head.txt
+-rw-rw-r--   0 john      (1000) john      (1000)    16410 2023-07-19 15:17:18.000000 sdss-roboscheduler-1.4.0/python/roboscheduler/fields.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2242 2023-05-09 16:48:00.000000 sdss-roboscheduler-1.4.0/python/roboscheduler/ks91.py
+-rw-r--r--   0 john      (1000) john      (1000)     1929 2023-05-09 16:48:00.000000 sdss-roboscheduler-1.4.0/python/roboscheduler/moonphase.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6570 2023-05-09 16:48:00.000000 sdss-roboscheduler-1.4.0/python/roboscheduler/observations.py
+-rw-rw-r--   0 john      (1000) john      (1000)    49797 2023-07-19 15:17:18.000000 sdss-roboscheduler-1.4.0/python/roboscheduler/scheduler.py
+-rw-r--r--   0 john      (1000) john      (1000)     9266 2023-05-09 16:48:00.000000 sdss-roboscheduler-1.4.0/python/roboscheduler/sunpos2.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-07-21 14:43:06.186611 sdss-roboscheduler-1.4.0/python/roboscheduler/tests/
+-rw-r--r--   0 john      (1000) john      (1000)        0 2023-05-09 16:48:00.000000 sdss-roboscheduler-1.4.0/python/roboscheduler/tests/__init__.py
+-rw-r--r--   0 john      (1000) john      (1000)      639 2023-05-09 16:48:00.000000 sdss-roboscheduler-1.4.0/python/roboscheduler/tests/conftest.py
+-rw-r--r--   0 john      (1000) john      (1000)     6060 2023-05-09 16:48:00.000000 sdss-roboscheduler-1.4.0/python/roboscheduler/tests/test_cadence.py
+-rw-r--r--   0 john      (1000) john      (1000)     4290 2023-05-09 16:48:00.000000 sdss-roboscheduler-1.4.0/python/roboscheduler/tests/test_packing.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-07-21 14:43:06.186611 sdss-roboscheduler-1.4.0/python/roboscheduler/utils/
+-rw-r--r--   0 john      (1000) john      (1000)       23 2023-05-09 16:48:00.000000 sdss-roboscheduler-1.4.0/python/roboscheduler/utils/__init__.py
+-rw-r--r--   0 john      (1000) john      (1000)     6472 2023-05-09 16:48:00.000000 sdss-roboscheduler-1.4.0/python/roboscheduler/utils/color_print.py
+-rw-r--r--   0 john      (1000) john      (1000)     6165 2023-05-09 16:48:00.000000 sdss-roboscheduler-1.4.0/python/roboscheduler/utils/logger.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-07-21 14:43:06.186611 sdss-roboscheduler-1.4.0/python/sdss_roboscheduler.egg-info/
+-rw-rw-r--   0 john      (1000) john      (1000)     1676 2023-07-21 14:43:06.000000 sdss-roboscheduler-1.4.0/python/sdss_roboscheduler.egg-info/PKG-INFO
+-rw-rw-r--   0 john      (1000) john      (1000)     2812 2023-07-21 14:43:06.000000 sdss-roboscheduler-1.4.0/python/sdss_roboscheduler.egg-info/SOURCES.txt
+-rw-rw-r--   0 john      (1000) john      (1000)        1 2023-07-21 14:43:06.000000 sdss-roboscheduler-1.4.0/python/sdss_roboscheduler.egg-info/dependency_links.txt
+-rw-rw-r--   0 john      (1000) john      (1000)        1 2023-05-09 16:48:01.000000 sdss-roboscheduler-1.4.0/python/sdss_roboscheduler.egg-info/not-zip-safe
+-rw-rw-r--   0 john      (1000) john      (1000)      201 2023-07-21 14:43:06.000000 sdss-roboscheduler-1.4.0/python/sdss_roboscheduler.egg-info/requires.txt
+-rw-rw-r--   0 john      (1000) john      (1000)       14 2023-07-21 14:43:06.000000 sdss-roboscheduler-1.4.0/python/sdss_roboscheduler.egg-info/top_level.txt
+-rw-rw-r--   0 john      (1000) john      (1000)     1456 2023-07-21 14:43:06.190611 sdss-roboscheduler-1.4.0/setup.cfg
+-rw-rw-r--   0 john      (1000) john      (1000)     1236 2023-05-09 16:48:00.000000 sdss-roboscheduler-1.4.0/setup.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-07-21 14:43:06.186611 sdss-roboscheduler-1.4.0/tests/
+-rw-rw-r--   0 john      (1000) john      (1000)    34225 2023-05-09 16:48:01.000000 sdss-roboscheduler-1.4.0/tests/test_cadence.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2888 2023-05-09 16:48:01.000000 sdss-roboscheduler-1.4.0/tests/test_scheduler.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `sdss-roboscheduler-1.3.2/LICENSE.md` & `sdss-roboscheduler-1.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdss-roboscheduler-1.3.2/PKG-INFO` & `sdss-roboscheduler-1.4.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-roboscheduler
-Version: 1.3.2
+Version: 1.4.0
 Summary: fps scheduling software for SDSS V
 Home-page: https://github.com/sdss/roboscheduler
 Author: Michael Blanton
 Maintainer: John Donor
 Maintainer-email: j.donor@tcu.edu
 License: BSD 3-Clause License
 Project-URL: Repository, https://github.com/sdss/roboscheduler
@@ -12,14 +12,15 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 License-File: LICENSE.md
 
 roboscheduler
```

### Comparing `sdss-roboscheduler-1.3.2/README.rst` & `sdss-roboscheduler-1.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `sdss-roboscheduler-1.3.2/bin/make_ms` & `sdss-roboscheduler-1.4.0/bin/make_ms`

 * *Files identical despite different names*

### Comparing `sdss-roboscheduler-1.3.2/bin/night_length` & `sdss-roboscheduler-1.4.0/bin/night_length`

 * *Files identical despite different names*

### Comparing `sdss-roboscheduler-1.3.2/cextern/cCadenceCore.cpp` & `sdss-roboscheduler-1.4.0/cextern/cCadenceCore.cpp`

 * *Files identical despite different names*

### Comparing `sdss-roboscheduler-1.3.2/cextern/cadenceCore.cpp` & `sdss-roboscheduler-1.4.0/cextern/cadenceCore.cpp`

 * *Files identical despite different names*

### Comparing `sdss-roboscheduler-1.3.2/include/cadenceCore.h` & `sdss-roboscheduler-1.4.0/include/cadenceCore.h`

 * *Files identical despite different names*

### Comparing `sdss-roboscheduler-1.3.2/python/roboscheduler/__init__.py` & `sdss-roboscheduler-1.4.0/python/roboscheduler/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,8 +39,8 @@
 if os.path.exists(custom_config_fn):
     try:
         config = merge(yaml.load(open(custom_config_fn),
                                  Loader=yaml.FullLoader), config)
     except AttributeError:
         config = merge(yaml.load(open(custom_config_fn)), config)
 
-__version__ = '1.3.2'
+__version__ = '1.4.0'
```

### Comparing `sdss-roboscheduler-1.3.2/python/roboscheduler/cadence.py` & `sdss-roboscheduler-1.4.0/python/roboscheduler/cadence.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,28 +125,28 @@
         max_length = self._arrayify(max_length, dtype=np.float32)
         min_moon_sep = self._arrayify(min_moon_sep, dtype=np.float32)
         min_deltav_ks91 = self._arrayify(min_deltav_ks91,
                                          dtype=np.float32)
         min_twilight_ang = self._arrayify(min_twilight_ang,
                                           dtype=np.float32)
         max_airmass = self._arrayify(max_airmass, dtype=np.float32)
-        self.obsmode_pk = np.array(obsmode_pk, dtype=np.str)
-        self.label_root = np.str(label_root)
-        self.label_version = np.str(label_version)
+        self.obsmode_pk = np.array(obsmode_pk, dtype=np.str_)
+        self.label_root = np.str_(label_root)
+        self.label_version = np.str_(label_version)
         epoch_indx = np.zeros(nepochs + 1, dtype=np.int32)
         epochs = np.zeros(nexp.sum(), dtype=np.int32)
         super().__init__(name, nepochs,
                          skybrightness, delta, delta_min,
                          delta_max, nexp, max_length,
                          min_moon_sep, min_deltav_ks91,
                          min_twilight_ang, max_airmass,
                          epoch_indx, epochs)
 
         self.partialEpochPri = priorities.get("partialEpochPri", 500)
-        self.brightDurDarkPenalty = priorities.get("brightDurDarkPenalty", -200)
+        self.brightDurDarkPenalty = priorities.get("brightDurDarkPenalty", -1000)
         self.deltaMaxPriBump = priorities.get("deltaMaxPriBump", 20)
         self.deltaNomBump = priorities.get("deltaNomBump", 20)
         self.overDeltaMaxBump = priorities.get("overDeltaMaxBump", 100)
         self.base_priority = priorities.get("base_priority", 100)
 
         return
 
@@ -161,25 +161,25 @@
         delta_max = np.array(cfg.get(name, 'delta_max').split(),
                              dtype=np.float32)
         nexp = np.array(cfg.get(name, 'nexp').split(),
                         dtype=np.int32)
         max_length = np.array(cfg.get(name, 'max_length').split(),
                               dtype=np.float32)
         obsmode_pk = np.array(cfg.get(name, 'obsmode_pk').split(),
-                              dtype=np.str)
+                              dtype=np.str_)
         min_moon_sep = np.array(cfg.get(name, 'min_moon_sep').split(),
                                 dtype=np.float32)
         min_deltav_ks91 = np.array(cfg.get(name, 'min_deltav_ks91').split(),
                                    dtype=np.float32)
         min_twilight_ang = np.array(cfg.get(name, 'min_twilight_ang').split(),
                                     dtype=np.float32)
         max_airmass = np.array(cfg.get(name, 'max_airmass').split(),
                                dtype=np.float32)
-        label_root = np.str(cfg.get(name, 'label_root'))
-        label_version = np.str(cfg.get(name, 'label_version'))
+        label_root = np.str_(cfg.get(name, 'label_root'))
+        label_version = np.str_(cfg.get(name, 'label_version'))
 
         self.__init__(name=name, nepochs=nepochs, skybrightness=skybrightness,
                       delta=delta, delta_min=delta_min, delta_max=delta_max,
                       nexp=nexp, max_length=max_length, obsmode_pk=obsmode_pk,
                       min_moon_sep=min_moon_sep, min_deltav_ks91=min_deltav_ks91,
                       min_twilight_ang=min_twilight_ang, max_airmass=max_airmass,
                       label_root=label_root, label_version=label_version)
@@ -332,18 +332,19 @@
 
     Notes:
     -----
 
     This is a singleton, so there can only be one CadenceList defined
     within any session.
     """
-    def __init__(self, skybrightness_only=False):
+    def __init__(self, skybrightness_only=False, observatory="apo"):
         self.reset()
         self.max_nsolns = 100
         self.skybrightness_only = skybrightness_only
+        self.observatory = observatory.lower()
         return
 
     def reset(self):
         """Reset cadence list to be empty"""
         self.ncadences = 0
         self.cadences = dict()
         self._cadence_consistency = dict()
@@ -831,15 +832,15 @@
         obsmode_dicts = targetdb.ObsMode.select().dicts()
         obsmodes = dict()
         for obsmode_dict in obsmode_dicts:
             curr = dict()
             curr['min_deltav_ks91'] = obsmode_dict['min_deltav_ks91']
             curr['min_moon_sep'] = obsmode_dict['min_moon_sep']
             curr['min_twilight_ang'] = obsmode_dict['min_twilight_ang']
-            curr['max_airmass'] = obsmode_dict['max_airmass']
+            curr[f'max_airmass'] = obsmode_dict[f'max_airmass_{self.observatory}']
             obsmodes[obsmode_dict['label']] = curr
 
         for cadence in cadence_dicts:
             if(cadence['delta'] is None or len(cadence['delta']) == 0):
                 continue
 
             if(version is not None):
@@ -856,14 +857,16 @@
                     continue
 
             if(use_label_root):
                 label = label_root
             else:
                 label = str(cadence['label'])
 
+            cadence["obsmode_pk"] = [o.strip() for o in cadence["obsmode_pk"]]
+
             if(cadence['obsmode_pk'] is not None):
                 min_moon_sep = np.array([obsmodes[x]['min_moon_sep']
                                          for x in cadence['obsmode_pk']],
                                         dtype=np.float32)
                 min_deltav_ks91 = np.array([obsmodes[x]['min_deltav_ks91']
                                             for x in cadence['obsmode_pk']],
                                            dtype=np.float32)
```

### Comparing `sdss-roboscheduler-1.3.2/python/roboscheduler/coords.py` & `sdss-roboscheduler-1.4.0/python/roboscheduler/coords.py`

 * *Files identical despite different names*

### Comparing `sdss-roboscheduler-1.3.2/python/roboscheduler/core/exceptions.py` & `sdss-roboscheduler-1.4.0/python/roboscheduler/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `sdss-roboscheduler-1.3.2/python/roboscheduler/etc/master_schedule_apo_gamma.par` & `sdss-roboscheduler-1.4.0/python/roboscheduler/etc/master_schedule_apo_gamma.par`

 * *Files identical despite different names*

### Comparing `sdss-roboscheduler-1.3.2/python/roboscheduler/etc/master_schedule_apo_maximal.par` & `sdss-roboscheduler-1.4.0/python/roboscheduler/etc/master_schedule_apo_maximal.par`

 * *Files identical despite different names*

### Comparing `sdss-roboscheduler-1.3.2/python/roboscheduler/etc/master_schedule_apo_maximal_v2.par` & `sdss-roboscheduler-1.4.0/python/roboscheduler/etc/master_schedule_apo_maximal_v2.par`

 * *Files identical despite different names*

### Comparing `sdss-roboscheduler-1.3.2/python/roboscheduler/etc/master_schedule_apo_maximal_v3.par` & `sdss-roboscheduler-1.4.0/python/roboscheduler/etc/master_schedule_apo_maximal_v3.par`

 * *Files identical despite different names*

### Comparing `sdss-roboscheduler-1.3.2/python/roboscheduler/etc/master_schedule_apo_may21.par` & `sdss-roboscheduler-1.4.0/python/roboscheduler/etc/master_schedule_apo_may21.par`

 * *Files identical despite different names*

### Comparing `sdss-roboscheduler-1.3.2/python/roboscheduler/etc/master_schedule_apo_minimal.par` & `sdss-roboscheduler-1.4.0/python/roboscheduler/etc/master_schedule_apo_minimal.par`

 * *Files identical despite different names*

### Comparing `sdss-roboscheduler-1.3.2/python/roboscheduler/etc/master_schedule_apo_normal.par` & `sdss-roboscheduler-1.4.0/python/roboscheduler/etc/master_schedule_apo_normal.par`

 * *Files identical despite different names*

### Comparing `sdss-roboscheduler-1.3.2/python/roboscheduler/etc/master_schedule_apo_normal_v2.par` & `sdss-roboscheduler-1.4.0/python/roboscheduler/etc/master_schedule_apo_normal_v2.par`

 * *Files identical despite different names*

### Comparing `sdss-roboscheduler-1.3.2/python/roboscheduler/etc/master_schedule_apo_normal_v3.par` & `sdss-roboscheduler-1.4.0/python/roboscheduler/etc/master_schedule_apo_normal_v3.par`

 * *Files identical despite different names*

### Comparing `sdss-roboscheduler-1.3.2/python/roboscheduler/etc/master_schedule_apo_normal_v4.par` & `sdss-roboscheduler-1.4.0/python/roboscheduler/etc/master_schedule_apo_normal_v4.par`

 * *Files identical despite different names*

### Comparing `sdss-roboscheduler-1.3.2/python/roboscheduler/etc/master_schedule_apo_normal_v5.par` & `sdss-roboscheduler-1.4.0/python/roboscheduler/etc/master_schedule_apo_normal_v5.par`

 * *Files identical despite different names*

### Comparing `sdss-roboscheduler-1.3.2/python/roboscheduler/etc/master_schedule_apo_plates.par` & `sdss-roboscheduler-1.4.0/python/roboscheduler/etc/master_schedule_apo_plates.par`

 * *Files identical despite different names*

### Comparing `sdss-roboscheduler-1.3.2/python/roboscheduler/etc/master_schedule_apo_test.par` & `sdss-roboscheduler-1.4.0/python/roboscheduler/etc/master_schedule_apo_test.par`

 * *Files identical despite different names*

### Comparing `sdss-roboscheduler-1.3.2/python/roboscheduler/etc/master_schedule_lco_gamma.par` & `sdss-roboscheduler-1.4.0/python/roboscheduler/etc/master_schedule_lco_gamma.par`

 * *Files identical despite different names*

### Comparing `sdss-roboscheduler-1.3.2/python/roboscheduler/etc/master_schedule_lco_maximal.par` & `sdss-roboscheduler-1.4.0/python/roboscheduler/etc/master_schedule_lco_maximal.par`

 * *Files identical despite different names*

### Comparing `sdss-roboscheduler-1.3.2/python/roboscheduler/etc/master_schedule_lco_maximal_v2.par` & `sdss-roboscheduler-1.4.0/python/roboscheduler/etc/master_schedule_lco_maximal_v2.par`

 * *Files identical despite different names*

### Comparing `sdss-roboscheduler-1.3.2/python/roboscheduler/etc/master_schedule_lco_maximal_v3.par` & `sdss-roboscheduler-1.4.0/python/roboscheduler/etc/master_schedule_lco_maximal_v3.par`

 * *Files identical despite different names*

### Comparing `sdss-roboscheduler-1.3.2/python/roboscheduler/etc/master_schedule_lco_may21.par` & `sdss-roboscheduler-1.4.0/python/roboscheduler/etc/master_schedule_lco_may21.par`

 * *Files identical despite different names*

### Comparing `sdss-roboscheduler-1.3.2/python/roboscheduler/etc/master_schedule_lco_minimal.par` & `sdss-roboscheduler-1.4.0/python/roboscheduler/etc/master_schedule_lco_minimal.par`

 * *Files identical despite different names*

### Comparing `sdss-roboscheduler-1.3.2/python/roboscheduler/etc/master_schedule_lco_normal.par` & `sdss-roboscheduler-1.4.0/python/roboscheduler/etc/master_schedule_lco_normal.par`

 * *Files identical despite different names*

### Comparing `sdss-roboscheduler-1.3.2/python/roboscheduler/etc/master_schedule_lco_normal_v2.par` & `sdss-roboscheduler-1.4.0/python/roboscheduler/etc/master_schedule_lco_normal_v2.par`

 * *Files identical despite different names*

### Comparing `sdss-roboscheduler-1.3.2/python/roboscheduler/etc/master_schedule_lco_normal_v3.par` & `sdss-roboscheduler-1.4.0/python/roboscheduler/etc/master_schedule_lco_normal_v3.par`

 * *Files identical despite different names*

### Comparing `sdss-roboscheduler-1.3.2/python/roboscheduler/etc/master_schedule_lco_normal_v4.par` & `sdss-roboscheduler-1.4.0/python/roboscheduler/etc/master_schedule_lco_normal_v4.par`

 * *Files identical despite different names*

### Comparing `sdss-roboscheduler-1.3.2/python/roboscheduler/etc/master_schedule_lco_test.par` & `sdss-roboscheduler-1.4.0/python/roboscheduler/etc/master_schedule_lco_test.par`

 * *Files identical despite different names*

### Comparing `sdss-roboscheduler-1.3.2/python/roboscheduler/fields.py` & `sdss-roboscheduler-1.4.0/python/roboscheduler/fields.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,27 +75,28 @@
         self.nfields = 0
         self.racen = np.zeros(0, dtype=np.float64)
         self.deccen = np.zeros(0, dtype=np.float64)
         self.nfilled = np.zeros(0, dtype=np.float64)
         self.pk = np.zeros(0, dtype=np.int32)
         # self.nextmjd = np.zeros(0, dtype=np.float64)
         self.epoch_idx = np.zeros(0, dtype=np.int32)
-        self.notDone = np.ones(0, dtype=np.bool)  # true is not done to skip the invert elsewhere
+        self.notDone = np.ones(0, dtype=np.bool_)  # true is not done to skip the invert elsewhere
         self.cadence = []
         self.observations = []
         self.slots = []
         self.flag = []
         self.lstObserved = np.zeros(0, dtype=np.int32)
-        self.cadencelist = roboscheduler.cadence.CadenceList()
+        self.cadencelist = roboscheduler.cadence.CadenceList(observatory=observatory)
         self._validCadance = None
         self._obsPlan = None
         self._lstPlan = None
         self._lunationPlan = None
         self._hist = None
         self._database = _database
+        self._designs = None
         return
 
     def setPriorities(self):
         scale = [10 if "bhm_rm" in c else 1 for c in self.cadence]
         self.basePriority = self.basePriority * np.array(scale)
         return
 
@@ -109,23 +110,42 @@
         self.cadence = [c.strip().decode() for c in fields_array['cadence']]
         self.slots = fields_array['slots_exposures']
         self.lstObserved = np.zeros((len(self.slots), 24), dtype=np.int32)
         self.observations = [np.zeros(0, dtype=np.int32)] * self.nfields
         self.icadence = np.zeros(self.nfields, dtype=np.int32)
         # self.nextmjd = np.zeros(self.nfields, dtype=np.float64)
         self.epoch_idx = np.zeros(self.nfields, dtype=np.float64)
-        self.basePriority = np.ones(self.nfields) * 200
-        self.notDone = np.ones(self.nfields, dtype=np.bool)
+        if "base_priority" in fields_array.dtype.names:
+            self.basePriority = fields_array["base_priority"]
+        else:
+            self.basePriority = np.ones(self.nfields)
+        self.notDone = np.ones(self.nfields, dtype=np.bool_)
         if "flag" in fields_array.dtype.names:
             self.flag = fields_array["flag"]
         else:
             self.flag = np.zeros(self.nfields)
         self.setPriorities()
         return
 
+    def createDummyDesigns(self):
+        """Create a list of arrays of dummy design ids
+        """
+        runningNumber = 1e6
+        self._designs = list()
+        for n in self.nfilled:
+            self._designs.append(np.arange(n) + runningNumber)
+            runningNumber += n
+            assert runningNumber not in self._designs[-1], "bad math"
+
+    @property
+    def designs(self):
+        if self._designs is None:
+            self.createDummyDesigns()
+        return self._designs
+
     def fromfits(self, filename=None):
         """Load a fits file into this Fields object,
            likely an RS-Allocation file.
 
         Parameters:
         ----------
 
@@ -151,14 +171,15 @@
         self.fields_fits["racen"] = fits_dat["racen"]
         self.fields_fits["deccen"] = fits_dat["deccen"]
         self.fields_fits["nfilled"] = fits_dat["nfilled"]
         self.fields_fits["slots_exposures"] = fits_dat["slots_exposures"]
         self.fields_fits["cadence"] = [c[:c.index("_v")] for c in fits_dat["cadence"]]
 
         self.fromarray(self.fields_fits)
+        self.createDummyDesigns()
         return
 
     @property
     def validCadence(self):
         if self._validCadance is None:
             assert len(self.cadence) > 0, "no field cadences!"
             assert len(self.cadencelist.cadences) > 0, "no cadences in cadencelist!"
@@ -271,34 +292,42 @@
 
         fields_model = [('pk', np.int32),
                         ('field_id', np.int32),
                         ('racen', np.float64),
                         ('deccen', np.float64),
                         ('nfilled', np.int32),
                         ('flag', np.int32),
+                        ('base_priority', np.int32),
                         ('slots_exposures', np.int32, (24, 2)),
                         ('cadence', np.dtype('a25'))]
 
         versionDB = targetdb.Version()
         ver = versionDB.get(plan=version)
 
         obsDB = targetdb.Observatory()
         obs = obsDB.get(label=self.observatory.upper())
 
         Field = targetdb.Field
         dbfields = Field.select().where(Field.version == ver,
                                         Field.observatory == obs)
 
+        pri_ver = opsdb.PriorityVersion.get(label="bulge")
+
+        bp = opsdb.BasePriority
+        prioritizedFields = bp.select().where(bp.version==pri_ver).dicts()
+        priorityDict = {p["field"]: p["priority"] for p in prioritizedFields}
+
         pk = list()
         field_id = list()
         racen = list()
         deccen = list()
         slots_exposures = list()
         cadence = list()
         flags = list()
+        base_priority = list()
 
         for field in dbfields:
             pk.append(field.pk)
             field_id.append(field.field_id)
             racen.append(field.racen)
             deccen.append(field.deccen)
             slots_exposures.append(field.slots_exposures)
@@ -306,22 +335,27 @@
             if len(field.priority) > 0:
                 if field.priority[0].label == "top":
                     flags.append(1)
                 elif field.priority[0].label == "disabled":
                     flags.append(-1)
             else:
                 flags.append(0)
+            if field.pk in priorityDict:
+                base_priority.append(priorityDict[field.pk])
+            else:
+                base_priority.append(1)
 
         fields = np.zeros(len(dbfields), dtype=fields_model)
 
         fields["pk"] = pk
         fields["field_id"] = field_id
         fields["racen"] = racen
         fields["deccen"] = deccen
         fields["flag"] = flags
+        fields["base_priority"] = base_priority
         fields["slots_exposures"] = slots_exposures
         fields["cadence"] = cadence
 
         # we're resetting field hist, so need to re-cache
         self._hist = None
 
         self.fromarray(fields_array=fields)
```

### Comparing `sdss-roboscheduler-1.3.2/python/roboscheduler/ks91.py` & `sdss-roboscheduler-1.4.0/python/roboscheduler/ks91.py`

 * *Files identical despite different names*

### Comparing `sdss-roboscheduler-1.3.2/python/roboscheduler/moonphase.py` & `sdss-roboscheduler-1.4.0/python/roboscheduler/moonphase.py`

 * *Files identical despite different names*

### Comparing `sdss-roboscheduler-1.3.2/python/roboscheduler/observations.py` & `sdss-roboscheduler-1.4.0/python/roboscheduler/observations.py`

 * *Files 5% similar despite different names*

```diff
@@ -81,20 +81,21 @@
         self.rSN2 = np.zeros(0, dtype=np.float32)
         self.bSN2 = np.zeros(0, dtype=np.float32)
         self.airmass = np.zeros(0, dtype=np.float32)
         self.skybrightness = np.zeros(0, dtype=np.float32)
         self.lst = np.zeros(0, dtype=np.float32)
         self.ha = np.zeros(0, dtype=np.float64)
         self.nexp_cumul = np.zeros(0, dtype=np.int32)
+        self.design_id = np.zeros(0, dtype=np.int32)
         return
 
     def add(self, field_pk=None, mjd=None, duration=None, apgSN2=None,
             rSN2=None, bSN2=None, skybrightness=None, airmass=None,
             lst=None, racen=None, deccen=None, cadence=None, nfilled=None,
-            nexp_cumul=None):
+            nexp_cumul=None, design_id=None):
         self.field_pk = np.append(self.field_pk,
                                  np.array([np.float64(field_pk)]))
         self.mjd = np.append(self.mjd,
                              np.array([np.float64(mjd)]))
         self.duration = np.append(self.duration,
                                   np.array([np.float64(duration)]))
         self.apgSN2 = np.append(self.apgSN2,
@@ -121,14 +122,16 @@
                                  np.array([np.int32(nfilled)]))
 
         ha = wrapHA(lst - racen)
         self.ha = np.append(self.ha,
                             np.array([np.float64(ha)]))
         self.nexp_cumul = np.append(self.nexp_cumul,
                                     np.array([np.int32(nexp_cumul)]))
+        self.design_id = np.append(self.design_id,
+                                   np.array([np.int32(design_id)]))
 
         return(self.nobservations - 1)
 
     def forfield(self, mjd=None, field_pk=None):
         indx = np.where((self.mjd <= mjd) &
                         (self.field_pk == field_pk))[0]
         return(self.toarray(indx=indx))
@@ -158,15 +161,16 @@
                 ('skybrightness', np.float32),
                 ('lst', np.float32),
                 ('racen', np.float64),
                 ('deccen', np.float64),
                 ('cadence', np.dtype('a20')),
                 ('nfilled', np.int32),
                 ('ha', np.float32),
-                ('nexp_cumul', np.int32)]
+                ('nexp_cumul', np.int32),
+                ('design_id', np.int32)]
         if(indx is None):
             indx = np.arange(self.nobservations)
         nobs = len(indx)
         obs = np.zeros(nobs, dtype=obs0)
         if(nobs > 0):
             obs['field_pk'] = self.field_pk[indx]
             obs['mjd'] = self.mjd[indx]
@@ -179,8 +183,9 @@
             obs['lst'] = self.lst[indx]
             obs['racen'] = self.racen[indx]
             obs['deccen'] = self.deccen[indx]
             obs['cadence'] = self.cadence[indx]
             obs['nfilled'] = self.nfilled[indx]
             obs['ha'] = self.ha[indx]
             obs['nexp_cumul'] = self.nexp_cumul[indx]
+            obs['design_id'] = self.design_id[indx]
         return(obs)
```

### Comparing `sdss-roboscheduler-1.3.2/python/roboscheduler/scheduler.py` & `sdss-roboscheduler-1.4.0/python/roboscheduler/scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import os, sys
+import os
 import numpy as np
 import fitsio
 import scipy.optimize as optimize
 import PyAstronomy.pyasl as pyasl
 import astropy.units as units
 import astropy.time as atime
 import pydl.pydlutils.yanny as yanny
@@ -938,14 +938,15 @@
         self.nExpPriAward = priorities.get("nExpPriAward", 1e5)
         self.nExpPriPenalty = priorities.get("nExpPriPenalty", -5)
         self.basePri = priorities.get("basePri", 100)
         self.lstPri = priorities.get("lstPri", 400)
         self.overheadPri = priorities.get("overheadPri", 40)
         self.remainAward = priorities.get("remainAward", 100)
         self.airmassPri = priorities.get("airmassPri", 20)
+        self.randomPri = priorities.get("randomPri", 0)
 
         return
 
     def initdb(self, designbase='plan-0', fromFits=True):
         """Initialize Scheduler fields and observation lists.
         Required before fields can be scheduled.
 
@@ -1024,24 +1025,26 @@
         # valid cadence checks against "none" cadence issue
         observable = (alt > 30.) & self.fields.validCadence & self.fields.notDone
         nexp = np.ones(len(observable), dtype=int)
         exp_epochs = np.zeros(len(observable), dtype=np.int32)
         epoch_idxs = np.zeros(len(observable), dtype=np.int32)
         delta_priority = np.zeros(len(observable), dtype=np.float64)
 
+        delta_priority += np.random.randn(len(observable)) * self.randomPri
+
         deltav = self.deltaV_sky_pos(mjd, self.fields.racen, self.fields.deccen)
         airmass = self.alt2airmass(alt)
         moon_dist = self.moon_dist(mjd=mjd, ra=self.fields.racen,
                                    dec=self.fields.deccen)
 
         # skybrightness in 2 days. Checked at each slot. Gives two chances to
         # finish partial field if scheduled
-        skybrightness_2days = self.skybrightness(mjd+2)
+        skybrightness_2days = self.skybrightness(mjd + 2)
 
-        whereRM = np.where(["174x" in c for c in self.fields.cadence])[0]
+        # whereRM = np.where(["174x" in c for c in self.fields.cadence])[0]
         # where_uhoh = np.where(["dark_2x" in c for c in self.fields.cadence])[0]
 
         # print("\n")
 
         next_change, next_brightness = self.next_change(mjd)
 
         nexp_change = int((next_change - mjd) / self.exp_time)
@@ -1208,17 +1211,17 @@
         Returns:
         -------
 
         priority : ndarray of np.float64
             calculated priority for each field
         """
 
-        priority = np.ones(len(iobservable)) * self.basePri
-        # priority = self.fields.basePriority[fieldid]
-        priority += delta_priority
+        # priority = np.ones(len(iobservable)) * self.basePri
+        priority = self.fields.basePriority[iobservable] * self.basePri + delta_priority
+        # priority += delta_priority
 
         lst = self.lst(mjd)
 
         lstHrs = lst/15
 
         # lstDiffs = lstDiff(self.fields.lstPlan[fieldid], np.ones(len(fieldid))*lstHrs)
 
@@ -1424,14 +1427,20 @@
 
         racen = self.fields.racen[fieldidx]
         deccen = self.fields.deccen[fieldidx]
         cadence = self.fields.cadence[fieldidx]
         nfilled = self.fields.nfilled[fieldidx]
         nexp_cumul = len(self.fields.observations[fieldidx]) + 1
 
+        design_indx = len(self.fields.hist[field_pk])
+        if design_indx == nfilled\
+            and self.fields.hist[field_pk][-1] - result["mjd"] < 0.1:
+            design_indx -= 1
+        design_id = self.fields.designs[fieldidx][design_indx]
+
         (alt, az) = self.radec2altaz(mjd=result['mjd'],
                                      ra=racen,
                                      dec=deccen)
         airmass = self.alt2airmass(alt)
         skybrightness = self.skybrightness(result['mjd'])
         lst = self.lst(result['mjd'])
         iobs = self.observations.add(field_pk=field_pk,
@@ -1443,15 +1452,16 @@
                                      skybrightness=skybrightness,
                                      airmass=airmass,
                                      lst=lst,
                                      racen=racen,
                                      deccen=deccen,
                                      cadence=cadence,
                                      nfilled=nfilled,
-                                     nexp_cumul=nexp_cumul)
+                                     nexp_cumul=nexp_cumul,
+                                     design_id=design_id)
 
         # iobservations = self.fields.observations[fieldidx]
         # mjd_past = self.observations.mjd[iobservations]
         # epoch_idx is the *index* of the *next* epoch
         # for 0 indexed arrays, this equivalent to
         # "how many epochs have I done previously"
         # epoch_idx, mjd_prev = epochs_completed(mjd_past, tolerance=45)
```

### Comparing `sdss-roboscheduler-1.3.2/python/roboscheduler/sunpos2.py` & `sdss-roboscheduler-1.4.0/python/roboscheduler/sunpos2.py`

 * *Files identical despite different names*

### Comparing `sdss-roboscheduler-1.3.2/python/roboscheduler/tests/conftest.py` & `sdss-roboscheduler-1.4.0/python/roboscheduler/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sdss-roboscheduler-1.3.2/python/roboscheduler/tests/test_cadence.py` & `sdss-roboscheduler-1.4.0/python/roboscheduler/tests/test_cadence.py`

 * *Files identical despite different names*

### Comparing `sdss-roboscheduler-1.3.2/python/roboscheduler/tests/test_packing.py` & `sdss-roboscheduler-1.4.0/python/roboscheduler/tests/test_packing.py`

 * *Files identical despite different names*

### Comparing `sdss-roboscheduler-1.3.2/python/roboscheduler/utils/color_print.py` & `sdss-roboscheduler-1.4.0/python/roboscheduler/utils/color_print.py`

 * *Files identical despite different names*

### Comparing `sdss-roboscheduler-1.3.2/python/roboscheduler/utils/logger.py` & `sdss-roboscheduler-1.4.0/python/roboscheduler/utils/logger.py`

 * *Files identical despite different names*

### Comparing `sdss-roboscheduler-1.3.2/python/sdss_roboscheduler.egg-info/PKG-INFO` & `sdss-roboscheduler-1.4.0/python/sdss_roboscheduler.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-roboscheduler
-Version: 1.3.2
+Version: 1.4.0
 Summary: fps scheduling software for SDSS V
 Home-page: https://github.com/sdss/roboscheduler
 Author: Michael Blanton
 Maintainer: John Donor
 Maintainer-email: j.donor@tcu.edu
 License: BSD 3-Clause License
 Project-URL: Repository, https://github.com/sdss/roboscheduler
@@ -12,14 +12,15 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 License-File: LICENSE.md
 
 roboscheduler
```

### Comparing `sdss-roboscheduler-1.3.2/python/sdss_roboscheduler.egg-info/SOURCES.txt` & `sdss-roboscheduler-1.4.0/python/sdss_roboscheduler.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -31,25 +31,27 @@
 python/roboscheduler/etc/master_schedule_apo_normal.par
 python/roboscheduler/etc/master_schedule_apo_normal_v2.par
 python/roboscheduler/etc/master_schedule_apo_normal_v3.par
 python/roboscheduler/etc/master_schedule_apo_normal_v4.par
 python/roboscheduler/etc/master_schedule_apo_normal_v5.par
 python/roboscheduler/etc/master_schedule_apo_plates.par
 python/roboscheduler/etc/master_schedule_apo_test.par
+python/roboscheduler/etc/master_schedule_apo_v6.par
 python/roboscheduler/etc/master_schedule_lco_gamma.par
 python/roboscheduler/etc/master_schedule_lco_maximal.par
 python/roboscheduler/etc/master_schedule_lco_maximal_v2.par
 python/roboscheduler/etc/master_schedule_lco_maximal_v3.par
 python/roboscheduler/etc/master_schedule_lco_may21.par
 python/roboscheduler/etc/master_schedule_lco_minimal.par
 python/roboscheduler/etc/master_schedule_lco_normal.par
 python/roboscheduler/etc/master_schedule_lco_normal_v2.par
 python/roboscheduler/etc/master_schedule_lco_normal_v3.par
 python/roboscheduler/etc/master_schedule_lco_normal_v4.par
 python/roboscheduler/etc/master_schedule_lco_test.par
+python/roboscheduler/etc/master_schedule_lco_v6.par
 python/roboscheduler/etc/observatories.par
 python/roboscheduler/etc/roboscheduler.yml
 python/roboscheduler/etc/sch_head.txt
 python/roboscheduler/tests/__init__.py
 python/roboscheduler/tests/conftest.py
 python/roboscheduler/tests/test_cadence.py
 python/roboscheduler/tests/test_packing.py
@@ -57,8 +59,10 @@
 python/roboscheduler/utils/color_print.py
 python/roboscheduler/utils/logger.py
 python/sdss_roboscheduler.egg-info/PKG-INFO
 python/sdss_roboscheduler.egg-info/SOURCES.txt
 python/sdss_roboscheduler.egg-info/dependency_links.txt
 python/sdss_roboscheduler.egg-info/not-zip-safe
 python/sdss_roboscheduler.egg-info/requires.txt
-python/sdss_roboscheduler.egg-info/top_level.txt
+python/sdss_roboscheduler.egg-info/top_level.txt
+tests/test_cadence.py
+tests/test_scheduler.py
```

### Comparing `sdss-roboscheduler-1.3.2/setup.cfg` & `sdss-roboscheduler-1.4.0/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sdss-roboscheduler
-version = 1.3.2
+version = 1.4.0
 author = Michael Blanton
 maintainer = John Donor
 maintainer_email = j.donor@tcu.edu
 description = fps scheduling software for SDSS V
 url = https://github.com/sdss/roboscheduler
 project_urls = 
 	Repository = https://github.com/sdss/roboscheduler
@@ -17,27 +17,28 @@
 	Intended Audience :: Science/Research
 	Natural Language :: English
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
 	Topic :: Software Development :: Libraries :: Python Modules
 
 [options]
 zip_safe = False
 include_package_data = True
 python_requires = >=3.7
 packages = find:
 package_dir = 
 	= python
 setup_requires = 
 	pybind11>=2.6.2
 install_requires = 
-	numpy==1.21.4
+	numpy
 	PyAstronomy
 	ortools
 	astropy
 	scipy
 	fitsio
 	peewee
 	pydl
```

### Comparing `sdss-roboscheduler-1.3.2/setup.py` & `sdss-roboscheduler-1.4.0/setup.py`

 * *Files identical despite different names*

