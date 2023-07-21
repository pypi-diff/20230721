# Comparing `tmp/hcam_devices-0.3.0.tar.gz` & `tmp/hcam_devices-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcam_devices-0.3.0.tar", last modified: Mon Sep 13 09:37:53 2021, max compression
+gzip compressed data, was "hcam_devices-1.0.0.tar", last modified: Fri Jul 21 10:47:52 2023, max compression
```

## Comparing `hcam_devices-0.3.0.tar` & `hcam_devices-1.0.0.tar`

### file list

```diff
@@ -1,76 +1,75 @@
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2021-09-13 09:37:53.691919 hcam_devices-0.3.0/
--rw-r--r--   0 sl         (501) staff       (20)      166 2020-06-05 15:17:54.000000 hcam_devices-0.3.0/AUTHORS.rst
--rw-r--r--   0 sl         (501) staff       (20)     3303 2020-06-05 15:22:14.000000 hcam_devices-0.3.0/CONTRIBUTING.rst
--rw-r--r--   0 sl         (501) staff       (20)       89 2020-06-05 15:22:33.000000 hcam_devices-0.3.0/HISTORY.rst
--rw-r--r--   0 sl         (501) staff       (20)     1077 2020-06-05 15:22:38.000000 hcam_devices-0.3.0/LICENSE
--rw-r--r--   0 sl         (501) staff       (20)      344 2020-06-05 16:07:50.000000 hcam_devices-0.3.0/MANIFEST.in
--rw-r--r--   0 sl         (501) staff       (20)     5621 2021-09-13 09:37:53.691984 hcam_devices-0.3.0/PKG-INFO
--rw-r--r--   0 sl         (501) staff       (20)     4587 2021-05-26 10:03:02.000000 hcam_devices-0.3.0/README.rst
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2021-09-13 09:37:53.679967 hcam_devices-0.3.0/hcam_devices/
--rw-r--r--   0 sl         (501) staff       (20)       96 2021-09-13 09:37:36.000000 hcam_devices-0.3.0/hcam_devices/__init__.py
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2021-09-13 09:37:53.680667 hcam_devices-0.3.0/hcam_devices/components/
--rw-r--r--   0 sl         (501) staff       (20)     4505 2021-06-07 22:45:32.000000 hcam_devices-0.3.0/hcam_devices/components/__init__.py
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2021-09-13 09:37:53.682601 hcam_devices-0.3.0/hcam_devices/devices/
--rw-r--r--   0 sl         (501) staff       (20)        0 2020-02-12 17:25:36.000000 hcam_devices-0.3.0/hcam_devices/devices/__init__.py
--rw-r--r--   0 sl         (501) staff       (20)     3307 2020-05-08 10:58:12.000000 hcam_devices-0.3.0/hcam_devices/devices/honeywell.py
--rw-r--r--   0 sl         (501) staff       (20)     9075 2021-06-17 04:27:50.000000 hcam_devices-0.3.0/hcam_devices/devices/meerstetter.py
--rw-r--r--   0 sl         (501) staff       (20)    21347 2020-07-30 09:16:47.000000 hcam_devices-0.3.0/hcam_devices/devices/newport.py
--rw-r--r--   0 sl         (501) staff       (20)    11601 2021-09-13 09:19:48.000000 hcam_devices-0.3.0/hcam_devices/devices/ngc.py
--rw-r--r--   0 sl         (501) staff       (20)     5308 2021-06-16 22:45:47.000000 hcam_devices-0.3.0/hcam_devices/devices/pdr900.py
--rw-r--r--   0 sl         (501) staff       (20)     4332 2020-02-11 15:35:28.000000 hcam_devices-0.3.0/hcam_devices/devices/properties.py
--rw-r--r--   0 sl         (501) staff       (20)     4075 2020-02-19 21:22:52.000000 hcam_devices-0.3.0/hcam_devices/devices/unichiller.py
--rw-r--r--   0 sl         (501) staff       (20)     8076 2021-05-21 10:38:02.000000 hcam_devices-0.3.0/hcam_devices/devices/zaber.py
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2021-09-13 09:37:53.682969 hcam_devices-0.3.0/hcam_devices/gtc/
--rw-r--r--   0 sl         (501) staff       (20)     4603 2020-06-04 13:32:09.000000 hcam_devices-0.3.0/hcam_devices/gtc/corba.py
--rw-r--r--   0 sl         (501) staff       (20)     3063 2021-05-18 10:00:55.000000 hcam_devices-0.3.0/hcam_devices/gtc/headers.py
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2021-09-13 09:37:53.686583 hcam_devices-0.3.0/hcam_devices/machines/
--rw-r--r--   0 sl         (501) staff       (20)      704 2021-06-14 09:56:58.000000 hcam_devices-0.3.0/hcam_devices/machines/__init__.py
--rw-r--r--   0 sl         (501) staff       (20)    35721 2021-06-16 15:02:37.000000 hcam_devices-0.3.0/hcam_devices/machines/connections.png
--rw-r--r--   0 sl         (501) staff       (20)     1353 2021-06-16 15:03:37.000000 hcam_devices-0.3.0/hcam_devices/machines/connections.yaml
--rw-r--r--   0 sl         (501) staff       (20)     1740 2021-06-16 14:39:38.000000 hcam_devices-0.3.0/hcam_devices/machines/controller.yaml
--rw-r--r--   0 sl         (501) staff       (20)    97935 2021-06-02 10:59:02.000000 hcam_devices-0.3.0/hcam_devices/machines/gtc.png
--rw-r--r--   0 sl         (501) staff       (20)     3696 2021-06-14 09:55:07.000000 hcam_devices-0.3.0/hcam_devices/machines/gtc.yaml
--rw-r--r--   0 sl         (501) staff       (20)    89357 2021-06-15 11:22:14.000000 hcam_devices-0.3.0/hcam_devices/machines/motors.png
--rw-r--r--   0 sl         (501) staff       (20)     3227 2021-06-15 11:13:19.000000 hcam_devices-0.3.0/hcam_devices/machines/motors.yaml
--rw-r--r--   0 sl         (501) staff       (20)    23023 2021-06-15 11:11:30.000000 hcam_devices-0.3.0/hcam_devices/machines/sensor.png
--rw-r--r--   0 sl         (501) staff       (20)     1226 2021-06-15 14:29:59.000000 hcam_devices-0.3.0/hcam_devices/machines/sensor.yaml
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2021-09-13 09:37:53.688624 hcam_devices-0.3.0/hcam_devices/models/
--rw-r--r--   0 sl         (501) staff       (20)        0 2020-02-12 17:25:47.000000 hcam_devices-0.3.0/hcam_devices/models/__init__.py
--rw-r--r--   0 sl         (501) staff       (20)     5001 2021-07-29 10:15:12.000000 hcam_devices-0.3.0/hcam_devices/models/ccd.py
--rw-r--r--   0 sl         (501) staff       (20)     4972 2021-06-15 01:16:55.000000 hcam_devices-0.3.0/hcam_devices/models/compo.py
--rw-r--r--   0 sl         (501) staff       (20)     2979 2021-06-15 01:16:59.000000 hcam_devices-0.3.0/hcam_devices/models/flow_sensor.py
--rw-r--r--   0 sl         (501) staff       (20)     6197 2021-06-17 03:52:46.000000 hcam_devices-0.3.0/hcam_devices/models/meerstetter.py
--rw-r--r--   0 sl         (501) staff       (20)     8967 2021-09-13 09:19:48.000000 hcam_devices-0.3.0/hcam_devices/models/ngc.py
--rw-r--r--   0 sl         (501) staff       (20)     5514 2021-06-15 01:17:10.000000 hcam_devices-0.3.0/hcam_devices/models/slide.py
--rw-r--r--   0 sl         (501) staff       (20)     5017 2021-06-14 09:58:19.000000 hcam_devices-0.3.0/hcam_devices/models/telescope.py
--rw-r--r--   0 sl         (501) staff       (20)     1952 2021-07-27 12:21:19.000000 hcam_devices-0.3.0/hcam_devices/models/vac_gauge.py
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2021-09-13 09:37:53.689560 hcam_devices-0.3.0/hcam_devices/testing/
--rw-r--r--   0 sl         (501) staff       (20)        0 2020-05-08 10:58:12.000000 hcam_devices-0.3.0/hcam_devices/testing/__init__.py
--rw-r--r--   0 sl         (501) staff       (20)     1227 2020-05-08 10:58:12.000000 hcam_devices-0.3.0/hcam_devices/testing/axis.py
--rw-r--r--   0 sl         (501) staff       (20)     2961 2020-05-08 10:58:12.000000 hcam_devices-0.3.0/hcam_devices/testing/fakeserial.py
--rw-r--r--   0 sl         (501) staff       (20)     2634 2020-05-08 10:58:12.000000 hcam_devices-0.3.0/hcam_devices/testing/properties.py
--rw-r--r--   0 sl         (501) staff       (20)     1051 2020-05-08 10:58:12.000000 hcam_devices-0.3.0/hcam_devices/testing/sensors.py
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2021-09-13 09:37:53.690063 hcam_devices-0.3.0/hcam_devices/utils/
--rw-r--r--   0 sl         (501) staff       (20)        0 2020-07-27 08:52:26.000000 hcam_devices-0.3.0/hcam_devices/utils/__init__.py
--rw-r--r--   0 sl         (501) staff       (20)     3334 2021-06-10 08:14:00.000000 hcam_devices-0.3.0/hcam_devices/utils/filesystem.py
--rw-r--r--   0 sl         (501) staff       (20)    13201 2021-06-11 14:55:21.000000 hcam_devices-0.3.0/hcam_devices/utils/obsmodes.py
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2021-09-13 09:37:53.690289 hcam_devices-0.3.0/hcam_devices/wamp/
--rw-r--r--   0 sl         (501) staff       (20)    10895 2021-09-13 09:19:48.000000 hcam_devices-0.3.0/hcam_devices/wamp/__init__.py
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2021-09-13 09:37:53.690525 hcam_devices-0.3.0/hcam_devices/wamp/utils/
--rw-r--r--   0 sl         (501) staff       (20)     2708 2021-05-26 12:52:51.000000 hcam_devices-0.3.0/hcam_devices/wamp/utils/__init__.py
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2021-09-13 09:37:53.680571 hcam_devices-0.3.0/hcam_devices.egg-info/
--rw-r--r--   0 sl         (501) staff       (20)     5621 2021-09-13 09:37:53.000000 hcam_devices-0.3.0/hcam_devices.egg-info/PKG-INFO
--rw-r--r--   0 sl         (501) staff       (20)     1776 2021-09-13 09:37:53.000000 hcam_devices-0.3.0/hcam_devices.egg-info/SOURCES.txt
--rw-r--r--   0 sl         (501) staff       (20)        1 2021-09-13 09:37:53.000000 hcam_devices-0.3.0/hcam_devices.egg-info/dependency_links.txt
--rw-r--r--   0 sl         (501) staff       (20)        1 2021-09-13 09:37:53.000000 hcam_devices-0.3.0/hcam_devices.egg-info/not-zip-safe
--rw-r--r--   0 sl         (501) staff       (20)       88 2021-09-13 09:37:53.000000 hcam_devices-0.3.0/hcam_devices.egg-info/requires.txt
--rw-r--r--   0 sl         (501) staff       (20)       13 2021-09-13 09:37:53.000000 hcam_devices-0.3.0/hcam_devices.egg-info/top_level.txt
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2021-09-13 09:37:53.691792 hcam_devices-0.3.0/scripts/
--rw-r--r--   0 sl         (501) staff       (20)     1784 2021-06-07 21:48:54.000000 hcam_devices-0.3.0/scripts/do_wamp_call
--rw-r--r--   0 sl         (501) staff       (20)      683 2021-03-26 10:24:58.000000 hcam_devices-0.3.0/scripts/gtcserver
--rwxr-xr-x   0 sl         (501) staff       (20)      628 2021-03-26 10:48:52.000000 hcam_devices-0.3.0/scripts/hserver
--rwxr-xr-x   0 sl         (501) staff       (20)     4840 2021-07-28 09:28:32.000000 hcam_devices-0.3.0/scripts/hwlogger
--rwxr-xr-x   0 sl         (501) staff       (20)     4876 2021-06-15 11:18:43.000000 hcam_devices-0.3.0/scripts/hwserver
--rw-r--r--   0 sl         (501) staff       (20)      479 2020-06-05 16:05:29.000000 hcam_devices-0.3.0/scripts/make_diagrams.py
--rw-r--r--   0 sl         (501) staff       (20)      313 2021-09-13 09:37:53.692280 hcam_devices-0.3.0/setup.cfg
--rw-r--r--   0 sl         (501) staff       (20)     2352 2021-09-13 09:37:36.000000 hcam_devices-0.3.0/setup.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-21 10:47:52.202196 hcam_devices-1.0.0/
+-rw-r--r--   0 sl         (501) staff       (20)      166 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/AUTHORS.rst
+-rw-r--r--   0 sl         (501) staff       (20)     3303 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 sl         (501) staff       (20)       89 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/HISTORY.rst
+-rw-r--r--   0 sl         (501) staff       (20)     1077 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/LICENSE
+-rw-r--r--   0 sl         (501) staff       (20)      344 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/MANIFEST.in
+-rw-r--r--   0 sl         (501) staff       (20)     5601 2023-07-21 10:47:52.202280 hcam_devices-1.0.0/PKG-INFO
+-rw-r--r--   0 sl         (501) staff       (20)     4587 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/README.rst
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-21 10:47:52.192788 hcam_devices-1.0.0/hcam_devices/
+-rw-r--r--   0 sl         (501) staff       (20)       96 2023-07-21 10:45:39.000000 hcam_devices-1.0.0/hcam_devices/__init__.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-21 10:47:52.193640 hcam_devices-1.0.0/hcam_devices/components/
+-rw-r--r--   0 sl         (501) staff       (20)     5584 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/hcam_devices/components/__init__.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-21 10:47:52.195293 hcam_devices-1.0.0/hcam_devices/devices/
+-rw-r--r--   0 sl         (501) staff       (20)        0 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/hcam_devices/devices/__init__.py
+-rw-r--r--   0 sl         (501) staff       (20)     3228 2023-07-21 10:44:48.000000 hcam_devices-1.0.0/hcam_devices/devices/honeywell.py
+-rw-r--r--   0 sl         (501) staff       (20)     9262 2023-07-21 10:44:48.000000 hcam_devices-1.0.0/hcam_devices/devices/meerstetter.py
+-rw-r--r--   0 sl         (501) staff       (20)    22137 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/hcam_devices/devices/newport.py
+-rw-r--r--   0 sl         (501) staff       (20)    11601 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/hcam_devices/devices/ngc.py
+-rw-r--r--   0 sl         (501) staff       (20)     5308 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/hcam_devices/devices/pdr900.py
+-rw-r--r--   0 sl         (501) staff       (20)     4293 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/hcam_devices/devices/properties.py
+-rw-r--r--   0 sl         (501) staff       (20)     4075 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/hcam_devices/devices/unichiller.py
+-rw-r--r--   0 sl         (501) staff       (20)     9819 2023-07-21 10:44:48.000000 hcam_devices-1.0.0/hcam_devices/devices/zaber.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-21 10:47:52.196100 hcam_devices-1.0.0/hcam_devices/gtc/
+-rw-r--r--   0 sl         (501) staff       (20)     5058 2023-07-21 10:44:48.000000 hcam_devices-1.0.0/hcam_devices/gtc/corba.py
+-rw-r--r--   0 sl         (501) staff       (20)     3063 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/hcam_devices/gtc/headers.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-21 10:47:52.198159 hcam_devices-1.0.0/hcam_devices/machines/
+-rw-r--r--   0 sl         (501) staff       (20)      704 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/hcam_devices/machines/__init__.py
+-rw-r--r--   0 sl         (501) staff       (20)     1366 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/hcam_devices/machines/connections.yaml
+-rw-r--r--   0 sl         (501) staff       (20)     1736 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/hcam_devices/machines/controller.yaml
+-rw-r--r--   0 sl         (501) staff       (20)     3982 2023-07-21 10:44:48.000000 hcam_devices-1.0.0/hcam_devices/machines/gtc.yaml
+-rw-r--r--   0 sl         (501) staff       (20)     4081 2023-07-21 10:44:48.000000 hcam_devices-1.0.0/hcam_devices/machines/motors.yaml
+-rw-r--r--   0 sl         (501) staff       (20)     1252 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/hcam_devices/machines/sensor.yaml
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-21 10:47:52.199517 hcam_devices-1.0.0/hcam_devices/models/
+-rw-r--r--   0 sl         (501) staff       (20)        0 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/hcam_devices/models/__init__.py
+-rw-r--r--   0 sl         (501) staff       (20)     5001 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/hcam_devices/models/ccd.py
+-rw-r--r--   0 sl         (501) staff       (20)     7703 2023-07-21 10:44:48.000000 hcam_devices-1.0.0/hcam_devices/models/compo.py
+-rw-r--r--   0 sl         (501) staff       (20)     2979 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/hcam_devices/models/flow_sensor.py
+-rw-r--r--   0 sl         (501) staff       (20)     6197 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/hcam_devices/models/meerstetter.py
+-rw-r--r--   0 sl         (501) staff       (20)     8967 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/hcam_devices/models/ngc.py
+-rw-r--r--   0 sl         (501) staff       (20)     7821 2023-07-21 10:44:48.000000 hcam_devices-1.0.0/hcam_devices/models/slide.py
+-rw-r--r--   0 sl         (501) staff       (20)     8325 2023-07-21 10:44:48.000000 hcam_devices-1.0.0/hcam_devices/models/telescope.py
+-rw-r--r--   0 sl         (501) staff       (20)     1952 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/hcam_devices/models/vac_gauge.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-21 10:47:52.200147 hcam_devices-1.0.0/hcam_devices/testing/
+-rw-r--r--   0 sl         (501) staff       (20)        0 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/hcam_devices/testing/__init__.py
+-rw-r--r--   0 sl         (501) staff       (20)     1227 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/hcam_devices/testing/axis.py
+-rw-r--r--   0 sl         (501) staff       (20)     2989 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/hcam_devices/testing/fakeserial.py
+-rw-r--r--   0 sl         (501) staff       (20)     2634 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/hcam_devices/testing/properties.py
+-rw-r--r--   0 sl         (501) staff       (20)     1051 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/hcam_devices/testing/sensors.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-21 10:47:52.200493 hcam_devices-1.0.0/hcam_devices/utils/
+-rw-r--r--   0 sl         (501) staff       (20)        0 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/hcam_devices/utils/__init__.py
+-rw-r--r--   0 sl         (501) staff       (20)     3334 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/hcam_devices/utils/filesystem.py
+-rw-r--r--   0 sl         (501) staff       (20)    13201 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/hcam_devices/utils/obsmodes.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-21 10:47:52.200631 hcam_devices-1.0.0/hcam_devices/wamp/
+-rw-r--r--   0 sl         (501) staff       (20)    10895 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/hcam_devices/wamp/__init__.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-21 10:47:52.200771 hcam_devices-1.0.0/hcam_devices/wamp/utils/
+-rw-r--r--   0 sl         (501) staff       (20)     2708 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/hcam_devices/wamp/utils/__init__.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-21 10:47:52.193523 hcam_devices-1.0.0/hcam_devices.egg-info/
+-rw-r--r--   0 sl         (501) staff       (20)     5601 2023-07-21 10:47:51.000000 hcam_devices-1.0.0/hcam_devices.egg-info/PKG-INFO
+-rw-r--r--   0 sl         (501) staff       (20)     1711 2023-07-21 10:47:51.000000 hcam_devices-1.0.0/hcam_devices.egg-info/SOURCES.txt
+-rw-r--r--   0 sl         (501) staff       (20)        1 2023-07-21 10:47:51.000000 hcam_devices-1.0.0/hcam_devices.egg-info/dependency_links.txt
+-rw-r--r--   0 sl         (501) staff       (20)        1 2023-07-21 10:47:51.000000 hcam_devices-1.0.0/hcam_devices.egg-info/not-zip-safe
+-rw-r--r--   0 sl         (501) staff       (20)      153 2023-07-21 10:47:51.000000 hcam_devices-1.0.0/hcam_devices.egg-info/requires.txt
+-rw-r--r--   0 sl         (501) staff       (20)       13 2023-07-21 10:47:51.000000 hcam_devices-1.0.0/hcam_devices.egg-info/top_level.txt
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-21 10:47:52.202059 hcam_devices-1.0.0/scripts/
+-rw-r--r--   0 sl         (501) staff       (20)     1784 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/scripts/do_wamp_call
+-rw-r--r--   0 sl         (501) staff       (20)      760 2023-07-21 10:44:48.000000 hcam_devices-1.0.0/scripts/gtcserver
+-rwxr-xr-x   0 sl         (501) staff       (20)      701 2023-07-21 10:44:48.000000 hcam_devices-1.0.0/scripts/hserver
+-rwxr-xr-x   0 sl         (501) staff       (20)     7021 2023-07-21 10:44:48.000000 hcam_devices-1.0.0/scripts/hwlogger
+-rwxr-xr-x   0 sl         (501) staff       (20)     6026 2023-07-21 10:44:48.000000 hcam_devices-1.0.0/scripts/hwserver
+-rw-r--r--   0 sl         (501) staff       (20)      479 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/scripts/make_diagrams.py
+-rw-r--r--   0 sl         (501) staff       (20)     1065 2023-07-21 10:44:48.000000 hcam_devices-1.0.0/scripts/show_telemetry
+-rw-r--r--   0 sl         (501) staff       (20)     7513 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/scripts/tcp_serial_bridge
+-rw-r--r--   0 sl         (501) staff       (20)      535 2023-07-21 10:44:48.000000 hcam_devices-1.0.0/scripts/zaber_ascii
+-rw-r--r--   0 sl         (501) staff       (20)      313 2023-07-21 10:47:52.202577 hcam_devices-1.0.0/setup.cfg
+-rw-r--r--   0 sl         (501) staff       (20)     2512 2023-07-21 10:45:39.000000 hcam_devices-1.0.0/setup.py
```

### Comparing `hcam_devices-0.3.0/CONTRIBUTING.rst` & `hcam_devices-1.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `hcam_devices-0.3.0/LICENSE` & `hcam_devices-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hcam_devices-0.3.0/PKG-INFO` & `hcam_devices-1.0.0/hcam_devices.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
-Name: hcam_devices
-Version: 0.3.0
+Name: hcam-devices
+Version: 1.0.0
 Summary: Device Communication via WAMP for HiPerCAM
 Home-page: https://github.com/HiPERCAM/hcam_devices
+Download-URL: https://github.com/HiPERCAM/hcam_devices/archive/v1.0.0.tar.gz
 Author: Stuart Littlefair
 Author-email: s.littlefair@shef.ac.uk
 License: MIT license
-Download-URL: https://github.com/HiPERCAM/hcam_devices/archive/v0.3.0.tar.gz
 Keywords: hcam_devices
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
@@ -143,9 +142,7 @@
 History
 =======
 
 0.1.0 (2020-06-05)
 ------------------
 
 * First release on PyPI.
-
-
```

### Comparing `hcam_devices-0.3.0/README.rst` & `hcam_devices-1.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `hcam_devices-0.3.0/hcam_devices/components/__init__.py` & `hcam_devices-1.0.0/hcam_devices/components/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from ..wamp import ModelComponentMixin, WrapperComponentMixin
 from ..models.slide import FocalPlaneSlide
 from ..models.flow_sensor import FlowSensor
-from ..models.compo import Compo
+from ..models.compo import Compo, CompoArms, CompoLens
 from ..models.meerstetter import Meerstetter
 from ..models.vac_gauge import VacGauge
 from ..models.ccd import CCDHead
 from ..models.ngc import NGC
 from ..models.telescope import GTC
 
 
@@ -89,25 +89,53 @@
         ).lower()
         host = config.extra.get('host', None)
         port = config.extra.get('port', None)
         emulation_mode = config.extra.get('emulate')
         self.model = FlowSensor(host, port, emulate=emulation_mode)
 
 
-class CompoComponent(ModelComponentMixin):
+class CompoArmComponent(ModelComponentMixin):
     def __init__(self, config):
-        super(CompoComponent, self).__init__(config)
+        super(CompoArmComponent, self).__init__(config)
         self.traceback_app = True
         self._component_name = config.extra.get(
             'name',
             str(self.__class__).replace('Component', '')
         ).lower()
         port = config.extra.get('port', None)
         emulation_mode = config.extra.get('emulate')
-        self.model = Compo(port, emulate=emulation_mode)
+        self.model = CompoArms(port, emulate=emulation_mode)
+
+class CompoLensComponent(ModelComponentMixin):
+    def __init__(self, config):
+        super(CompoLensComponent, self).__init__(config)
+        self.traceback_app = True
+        self._component_name = config.extra.get(
+            'name',
+            str(self.__class__).replace('Component', '')
+        ).lower()
+        host = config.extra.get('host', None)
+        port = config.extra.get('port', None)
+        emulation_mode = config.extra.get('emulate')
+        self.model = CompoLens(host, port, emulate=emulation_mode)
+
+
+class CompoComponent(WrapperComponentMixin):
+    def __init__(self, config):
+        # get name from config, or class name if missing
+        self._component_name = config.extra.get(
+            'name',
+            str(self.__class__).replace('Component', '')
+        ).lower()
+        arm_topic = config.extra.get('arm_topic')
+        lens_topic = config.extra.get('lens_topic')
+
+        super(CompoComponent, self).__init__(config)
+        self.traceback_app = True
+        self.model = Compo(arm_topic, lens_topic)
 
 
 class MeerstetterComponent(ModelComponentMixin):
     def __init__(self, config):
         super(MeerstetterComponent, self).__init__(config)
         self.traceback_app = True
         self._component_name = config.extra.get(
```

### Comparing `hcam_devices-0.3.0/hcam_devices/devices/honeywell.py` & `hcam_devices-1.0.0/hcam_devices/devices/honeywell.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # talk to honeywell temperature monitor
 from __future__ import absolute_import, unicode_literals, print_function, division
 import threading
 import six
 from random import normalvariate
-if not six.PY3:
+
+try:
     from pymodbus.constants import Endian
     from pymodbus.payload import BinaryPayloadDecoder
-    from pymodbus.client.sync import ModbusTcpClient as ModbusClient
-else:
+    from pymodbus.client import ModbusTcpClient as ModbusClient
+except:
     from pymodbus3.constants import Endian
     from pymodbus3.payload import BinaryPayloadDecoder
-    from pymodbus3.client.sync import ModbusTcpClient as ModbusClient
-
+    from pymodbus3.client.sync import ModbusTcpClient as ModbusClient    
 
 class MinitrendError(Exception):
     pass
 
 
 class Minitrend:
     def __init__(self, address, port):
         self.address = address
         self.client = ModbusClient(address, port=port)
         # list mapping pen ID number to address
-        self.pen_addresses = {i: 0x18C0 + i*0x2 for i in range(16)}
-        self.alarm_addresses = {i: 0x1980 + i*0x1 for i in range(16)}
+        self.pen_addresses = {i: 0x18C0 + i * 0x2 for i in range(16)}
+        self.alarm_addresses = {i: 0x1980 + i * 0x1 for i in range(16)}
         self.unit_id = 0x01  # allows us to address different units on the same network
         # thread safe access
         self._lock = threading.Lock()
 
     def __del__(self):
         self.disconnect()
 
@@ -45,47 +45,52 @@
         Raises
         ------
         MinitrendError
             When reading fails
         """
         with self._lock:
             try:
-                payload = self.client.read_input_registers(address, size, unit=self.unit_id)
+                payload = self.client.read_input_registers(
+                    address, size, unit=self.unit_id
+                )
             except Exception as err:
                 raise MinitrendError(str(err))
         return payload
 
     def get_pen(self, pen_number):
         address = self.pen_addresses[pen_number]
         result = self.read_register(address, 2)
         if not six.PY3:
-            decoder = BinaryPayloadDecoder.fromRegisters(result.registers,
-                                                         endian=Endian.Big)
+            decoder = BinaryPayloadDecoder.fromRegisters(
+                result.registers, endian=Endian.Big
+            )
         else:
-            decoder = BinaryPayloadDecoder.from_registers(result.registers,
-                                                          endian=Endian.Big)
+            decoder = BinaryPayloadDecoder.from_registers(
+                result.registers, endian=Endian.Big
+            )
         return decoder.decode_32bit_float()
 
     def get_alarm(self, alarm_number):
         address = self.alarm_addresses[alarm_number]
         result = self.read_register(address, 1)
         if not six.PY3:
-            decoder = BinaryPayloadDecoder.fromRegisters(result.registers,
-                                                         endian=Endian.Big)
+            decoder = BinaryPayloadDecoder.fromRegisters(
+                result.registers, endian=Endian.Big
+            )
         else:
-            decoder = BinaryPayloadDecoder.from_registers(result.registers,
-                                                          endian=Endian.Big)
+            decoder = BinaryPayloadDecoder.from_registers(
+                result.registers, endian=Endian.Big
+            )
         value = decoder.decode_16bit_uint()
         # six alarms, each corresponding to a bit of the return value
         flags = [(value >> i) & 1 for i in range(6)]
         return flags
 
 
 class MinitrendEmulator:
-
     def __init__(self, pen_values, noise_level=0):
         self.pen_values = pen_values
         self.noise_level = noise_level
 
     def connect(self):
         return True
```

### Comparing `hcam_devices-0.3.0/hcam_devices/devices/meerstetter.py` & `hcam_devices-1.0.0/hcam_devices/devices/meerstetter.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,47 +10,51 @@
 from ..testing.sensors import SensorEmulator
 
 DEFAULT_TIMEOUT = 5
 TEC_CURRENT_LIMIT = 10.7
 
 
 error_codes = {
-    '+01': 'Command not available',
-    '+02': 'Device is busy',
-    '+03': 'Communication error',
-    '+04': 'Format error',
-    '+05': 'Parameter not available',
-    '+06': 'Parameter is read only',
-    '+07': 'Value is out of range',
-    '+08': 'Instance not available'
+    "+01": "Command not available",
+    "+02": "Device is busy",
+    "+03": "Communication error",
+    "+04": "Format error",
+    "+05": "Parameter not available",
+    "+06": "Parameter is read only",
+    "+07": "Value is out of range",
+    "+08": "Instance not available",
 }
 
 STATUS_CODES = {
-    0: 'init', 1: 'ready', 2: 'run', 3: 'error',
-    4: 'bootloader', 5: 'resetting'
+    0: "init",
+    1: "ready",
+    2: "run",
+    3: "error",
+    4: "bootloader",
+    5: "resetting",
 }
 
 
 def hex_to_int(hexstring):
     return int(hexstring, 16)
 
 
 def hex_to_float32(hexstring):
     try:
         if six.PY2:
-            byteval = hexstring.strip().decode('hex')
+            byteval = hexstring.strip().decode("hex")
         else:
             byteval = bytes.fromhex(hexstring.strip())
     except Exception as err:
-        raise RuntimeError('cannot decode string {}!\n{}'.format(hexstring, err))
-    return struct.unpack(str('!f'), byteval)[0]
+        raise RuntimeError("cannot decode string {}!\n{}".format(hexstring, err))
+    return struct.unpack(str("!f"), byteval)[0]
 
 
 def float32_to_hex(f):
-    return format(struct.unpack(str('<I'), struct.pack(str('<f'), f))[0], 'X')
+    return format(struct.unpack(str("<I"), struct.pack(str("<f"), f))[0], "X")
 
 
 class CRCCalculator(object):
     def __init__(self):
         self.polynomial = 0x1021
         self.preset = 0
         self._lut = [self._calc_initial(i) for i in range(256)]
@@ -63,39 +67,39 @@
                 crc = (crc << 1) ^ self.polynomial
             else:
                 crc = crc << 1
             c = c << 1
         return crc
 
     def _update_crc(self, crc, c):
-        cc = 0xff & c
+        cc = 0xFF & c
 
         tmp = (crc >> 8) ^ cc
-        crc = (crc << 8) ^ self._lut[tmp & 0xff]
-        crc = crc & 0xffff
+        crc = (crc << 8) ^ self._lut[tmp & 0xFF]
+        crc = crc & 0xFFFF
         return crc
 
     def __call__(self, msg):
         crc = self.preset
         for c in msg:
             crc = self._update_crc(crc, ord(c))
-        return format(crc, '0>4X')
+        return format(crc, "0>4X")
 
 
 class MeerstetterTEC1090Emulator(object):
     def __init__(self, address, port):
         self._heatsinks = {i: SensorEmulator(38, 0.1, 0.001) for i in range(1, 4)}
         self._currents = {i: SensorEmulator(8, 0.1, 0.001) for i in range(1, 4)}
         self._temperatures = {i: SensorEmulator(-90, 0.1, 0.01) for i in range(1, 4)}
 
     def disconnect(self):
-        pass
+        return True
 
     def connect(self):
-        pass
+        return True
 
     def get_status(self, addr):
         return 2
 
     def get_heatsink_temp(self, addr):
         return self._heatsinks[addr].current_value
 
@@ -116,23 +120,26 @@
     """
     Class to use TCP/IP to communicate with TEC-1090 controllers
     mounted in LTR-1200. Communication protocol is MeCom.
 
     See MeCom protocol spec document 5117B and TEC protocol document
     5136 for details.
     """
-    def __init__(self, address, port):
 
-        self.logger = logging.getLogger('meerstetter.{}'.format(address))
+    def __init__(self, address, port, file_logging=False):
+        self.logger = logging.getLogger("meerstetter.{}".format(address))
         self.logger.setLevel(logging.DEBUG)
-        fh = logging.FileHandler('meerstetter.log')
-        fh.setLevel(logging.DEBUG)
-        formatter = logging.Formatter('%(asctime)s - %(name)s - %(threadName)s - %(message)s')
-        fh.setFormatter(formatter)
-        self.logger.addHandler(fh)
+        if file_logging:
+            fh = logging.FileHandler("meerstetter.log")
+            fh.setLevel(logging.DEBUG)
+            formatter = logging.Formatter(
+                "%(asctime)s - %(name)s - %(threadName)s - %(message)s"
+            )
+            fh.setFormatter(formatter)
+            self.logger.addHandler(fh)
 
         self.address = address
         self.port = port
         self.seq_no = random.randint(1, 1000)
         self.crc_calc = CRCCalculator()
         self.tec_current_limit = TEC_CURRENT_LIMIT
         self._lock = threading.Lock()
@@ -147,17 +154,17 @@
 
     def connect(self):
         try:
             s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
             s.settimeout(DEFAULT_TIMEOUT)
             s.connect((self.address, self.port))
             welcome = s.recv(1024)
-            if 'Welcome' not in welcome.decode():
-                self.logger.error('did not receive welcome message from meerstetter')
-                raise IOError('did not receive welcome message from meerstetter')
+            if "Welcome" not in welcome.decode():
+                self.logger.error("did not receive welcome message from meerstetter")
+                raise IOError("did not receive welcome message from meerstetter")
         except Exception:
             # connection failed
             return False
         self.sock = s
         return True
 
     def _assemble_frame(self, address, payload):
@@ -170,111 +177,116 @@
         1: Control (source); ASCII Char; 1 bytes
         2: Address; UINT8; 2 bytes
         3: Sequence No; UINT16; 4 bytes
         4: Payload; N bytes
         5: Checksum, 4 bytes
         6: End of Frame, 1 byte <CR>
         """
-        cs = '#'
-        addr = format(address, '0>2X')
-        seq = format(self.seq_no, '0>4X')
+        cs = "#"
+        addr = format(address, "0>2X")
+        seq = format(self.seq_no, "0>4X")
         # increment sequence number, but ensure it's not > 65535
         # that would overflow buffer! We roll over at 65534
         self.seq_no = (self.seq_no + 1) % 65535
         msg = cs + addr + seq + payload
-        eof = '\r'
+        eof = "\r"
         return msg + self.crc_calc(msg) + eof
 
     def _send_frame(self, frame_msg):
         # threadsafe and error-safe opening of socket
         with self._lock:
             self.sock.send(frame_msg.encode())
             ret_msg = self.sock.recv(1024)
         ret_msg = ret_msg.decode().strip()
-        self.logger.info('got ret_msg = {}'.format(ret_msg))
+        self.logger.info("got ret_msg = {}".format(ret_msg))
         self._check_response(frame_msg, ret_msg)
         return self._strip_response(ret_msg)
 
     def _check_response(self, frame_msg, ret_msg):
-        if ret_msg[0] == '!' and frame_msg[1:7] == ret_msg[1:7]:
+        if ret_msg[0] == "!" and frame_msg[1:7] == ret_msg[1:7]:
             # a valid response, and same seq no. so far so good
             crc_back = ret_msg[-4:]
             crc_out = frame_msg[-5:-1]
             package_in = ret_msg[:-4]
             if self.crc_calc(package_in) != crc_back and crc_out != crc_back:
-                raise IOError('checksum of return message not OK:\nOut: {}\nBack: {}'.format(
-                                frame_msg, ret_msg
-                              ))
+                raise IOError(
+                    "checksum of return message not OK:\nOut: {}\nBack: {}".format(
+                        frame_msg, ret_msg
+                    )
+                )
         else:
-            raise IOError('response not from device, or sequence number mismatch:\nOut: {}\nBack: {}'.format(
-                            frame_msg, ret_msg
-                          ))
+            raise IOError(
+                "response not from device, or sequence number mismatch:\nOut: {}\nBack: {}".format(
+                    frame_msg, ret_msg
+                )
+            )
 
     def _strip_response(self, ret_msg):
         return ret_msg[7:-4]
 
-    def get_param(self, address, param_no, instance, param_type='float'):
-        payload = '?VR{param_no:0>4X}{instance:0>2X}'.format(
+    def get_param(self, address, param_no, instance, param_type="float"):
+        payload = "?VR{param_no:0>4X}{instance:0>2X}".format(
             param_no=param_no, instance=instance
         )
-        self.logger.info('payload = {}'.format(payload))
+        self.logger.info("payload = {}".format(payload))
         frame_msg = self._assemble_frame(address, payload)
         encoded_param_val = self._send_frame(frame_msg)
-        if encoded_param_val == '+05':
-            raise IOError('param {} not available'.format(param_no))
+        if encoded_param_val == "+05":
+            raise IOError("param {} not available".format(param_no))
 
         if encoded_param_val in error_codes:
             raise IOError(
-                'failed to get param {}\n{}'.format(param_no, error_codes[encoded_param_val])
+                "failed to get param {}\n{}".format(
+                    param_no, error_codes[encoded_param_val]
+                )
             )
 
-        if param_type == 'float':
+        if param_type == "float":
             return hex_to_float32(encoded_param_val)
         else:
             return hex_to_int(encoded_param_val)
 
     def reset_tec(self, address):
-        payload = 'RS'
+        payload = "RS"
         frame_msg = self._assemble_frame(address, payload)
         ret_msg = self._send_frame(frame_msg)
-        if ret_msg != '':
-            raise IOError('unexpected response to reset command {}'.format(ret_msg))
+        if ret_msg != "":
+            raise IOError("unexpected response to reset command {}".format(ret_msg))
 
     def set_ccd_temp(self, address, target_temp):
         param_no = 3000
-        payload = 'VS{param_no:0>4X}{instance:0>2X}{encoded_val}'.format(
-            param_no=param_no, instance=1,
-            encoded_val=float32_to_hex(target_temp)
+        payload = "VS{param_no:0>4X}{instance:0>2X}{encoded_val}".format(
+            param_no=param_no, instance=1, encoded_val=float32_to_hex(target_temp)
         )
         frame_msg = self._assemble_frame(address, payload)
         ret_msg = self._send_frame(frame_msg)
-        if ret_msg.startswith('+'):
+        if ret_msg.startswith("+"):
             if ret_msg in error_codes:
                 raise IOError(error_codes[ret_msg])
             else:
-                raise IOError('unknown error code {}'.format(ret_msg))
+                raise IOError("unknown error code {}".format(ret_msg))
 
     def get_ccd_temp(self, address):
-        self.logger.info('getting CCD{} temp'.format(address))
+        self.logger.info("getting CCD{} temp".format(address))
         param_no = 1000
         return self.get_param(address, param_no, 1)
 
     def get_setpoint(self, address):
         param_no = 1010
         return self.get_param(address, param_no, 1)
 
     def get_heatsink_temp(self, address):
         param_no = 1001
         return self.get_param(address, param_no, 1)
 
     def get_power(self, address):
         current = self.get_param(address, 1020, 1)
         voltage = self.get_param(address, 1021, 1)
-        return current*voltage
+        return current * voltage
 
     def get_current(self, address):
         return self.get_param(address, 1020, 1)
 
     def get_status(self, address):
         param_no = 104
-        status = self.get_param(address, param_no, 1, param_type='int')
+        status = self.get_param(address, param_no, 1, param_type="int")
         return status
```

### Comparing `hcam_devices-0.3.0/hcam_devices/devices/newport.py` & `hcam_devices-1.0.0/hcam_devices/devices/newport.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,15 +110,16 @@
                 self.axis[i] = NewportESP301Axis(
                     self, i+1, unit_equivalencies=self._unit_equivalencies)
             except (NewportError, serial.SerialException):
                 # this will fail if axis is not enabled in controller
                 self.axis[i] = None
 
     def disconnect(self):
-        self.ser.close()
+        if self.ser is not None:
+            self.ser.close()
         self.ser = None
 
     def __del__(self):
         self.disconnect()
 
     def _execute(self, cmd, errcheck):
         """
@@ -126,25 +127,25 @@
         """
         response = None
 
         with self.lock:
             with NoKeyboardInterrupt():
                 if not cmd.endswith('\r'):
                     cmd += '\r'
-                self.ser.write(cmd)
+                self.ser.write(cmd.encode())
                 if '?' in cmd:
                     response = self.ser.readline().strip()
 
                 if errcheck:
-                    self.ser.write('TB?\r')
-                    error_string = self.ser.readline().strip()
+                    self.ser.write(b'TB?\r')
+                    error_string = self.ser.readline().decode().strip()
                     if not error_string.startswith('0'):
                         raise NewportError(error_string)
 
-        return response
+        return response.decode() if response is not None else ''
 
     def _cmd(self, cmd, params=tuple(), target=None, errcheck=True):
         """
         Here we wrap low-level read/write commands to allow specifying different axis and error checking
 
         Write to device.
 
@@ -404,16 +405,25 @@
             0 : search by zero position count
             1 : search for home and index signals (default)
             2 : search only for home signal
             3 : search for positive limit signal
             4 : search for negative limit signal
             5 : seach for positive limit and index signals
             6 : search for negative limit and index signals
+
+       Returns
+        -------
+        success: bool
+            True or False depending on whether home command was successful        
         """
-        self._cmd('OR', params=[search_mode], errcheck=errcheck)
+        try:
+            self._cmd('OR', params=[search_mode], errcheck=errcheck)
+        except Exception:
+            return False
+        return True
 
     def move(self, position, absolute=True, wait=False, block=False):
         """
         Move to or by a specified position.
 
         Parameters
         ----------
@@ -424,30 +434,39 @@
         absolute : bool
             If `False`, position is a relative offset from current position
         wait : bool
             If `True`, function returns immediately, but axis is instructed
             not to execute other commands until move is finished.
         block : bool
             IF `True`, function will not return until move is complete.
+
+        Returns
+        -------
+        success: bool
+            True or False depending on whether move command was successful
         """
         if not isinstance(position, u.Quantity):
             position = position * self.units
         position = position.to(self.units,
                                equivalencies=self._unit_equivalencies).value
 
         cmd = 'PA' if absolute else 'PR'
-        self._cmd(cmd, params=[position])
-        if wait:
-            self.wait_for_position(position)
-        if block:
-            time.sleep(0.01)
-            done = self.motion_complete
-            while not done:
-                done = self.motion_complete
+        try:
+            self._cmd(cmd, params=[position])
+            if wait:
+                self.wait_for_position(position)
+            if block:
                 time.sleep(0.01)
+                done = self.motion_complete
+                while not done:
+                    done = self.motion_complete
+                    time.sleep(0.01)
+        except Exception:
+            return False
+        return True
 
     def wait_for_position(self, position):
         """
         Wait for axis to reach given position before executing other commands.
 
         Following this call, other commands can be sent to the controller, but they
         will not be executed until the specified position is reached. Most useful
@@ -479,16 +498,25 @@
         Stops motion immediately
         """
         self._cmd('AB')
 
     def stop(self):
         """
         Stops motion with programmed decceleration.
+
+        Returns
+        -------
+        success: bool
+            True or False depending on whether stop command was successful
         """
-        self._cmd('ST')
+        try:
+            self._cmd('ST')
+        except Exception:
+            return False
+        return True
 
     def move_to_hardware_limit(self):
         """
         Move to hardware travel limit
         """
         self._cmd('MT')
```

### Comparing `hcam_devices-0.3.0/hcam_devices/devices/ngc.py` & `hcam_devices-1.0.0/hcam_devices/devices/ngc.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-0.3.0/hcam_devices/devices/pdr900.py` & `hcam_devices-1.0.0/hcam_devices/devices/pdr900.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-0.3.0/hcam_devices/devices/properties.py` & `hcam_devices-1.0.0/hcam_devices/devices/properties.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,20 +62,21 @@
             raise AttributeError("can't set attribute")
 
         # if we are passed a float or int, assume correct units and create quantity
         if not isinstance(value, u.Quantity):
             value = value * self.units * instance.units if self.relative_units else value * self.units
 
         # get value in correct units
-        value = value.to(self.units * instance.units if self.relative_units else self.units,
-                         equivalencies=self.unit_equivalencies).value
+        value = value.to_value(
+            self.units * instance.units if self.relative_units else self.units
+        )
 
         # set value
         code = instance._format_set_command(self.code)
-        instance._cmd(code, params=value, errcheck=self.errcheck)
+        instance._cmd(code, params=(value,), errcheck=self.errcheck)
 
 
 class IntegerDeviceProperty(DeviceProperty):
     """
     An Device property that must be integer.
     """
     def __init__(self, code, errcheck=True, readonly=False):
```

### Comparing `hcam_devices-0.3.0/hcam_devices/devices/unichiller.py` & `hcam_devices-1.0.0/hcam_devices/devices/unichiller.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-0.3.0/hcam_devices/devices/zaber.py` & `hcam_devices-1.0.0/hcam_devices/devices/zaber.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 """
 Zaber Linear Stages, including T-LLS devices
 """
-from __future__ import (print_function, division, absolute_import)
+from __future__ import print_function, division, absolute_import
 import struct
 import six
 import socket
 import threading
 import time
 
 from .properties import DeviceProperty, BooleanDeviceProperty, microstep
@@ -16,28 +16,33 @@
     ConnectionRefusedError = socket.error
 
 
 class ZaberError(Exception):
     pass
 
 
+class ZaberTimeoutError(ZaberError):
+    pass
+
+
 # how long to wait before giving up on a response
 DEFAULT_TIMEOUT = 5
 
 # number of bytes to transmit & recieve
 PACKET_SIZE = 6
 
 # command numbers
 RESET = 0
 HOME = 1
 MOVE_ABSOLUTE = 20
 MOVE_RELATIVE = 21
 STOP = 23
 RESTORE = 36
 SET_MODE = 40
+MAX_POSITION = 44
 RETURN_SETTING = 53
 RETURN_STATUS = 54
 POSITION = 60
 NULL = 0
 
 # error return from slide
 ERROR = 255
@@ -53,29 +58,30 @@
 FALSE = 0
 
 
 class ZaberLS(object):
     position = DeviceProperty(POSITION, readonly=True)
     moving = BooleanDeviceProperty(RETURN_STATUS, readonly=True)
 
-    def __init__(self, host='192.168.1.3', port=10001, unit_equivalencies=None):
+    def __init__(self, host="192.168.1.3", port=10001, unit_equivalencies=None):
         """
         Creates a Zaber device. Arguments::
 
          host: IP address of terminal server
          port: port device representing the slide
 
         """
         self.port = port
         self.host = host
         # thread lock for threadsafe operations
         self._lock = threading.Lock()
         self.unit = UNIT
         self.unit_equivalencies = unit_equivalencies
         self.units = microstep
+        self.sock = None
 
     def __del__(self):
         # must close connection on object deletion
         self.close()
 
     def connect(self):
         # connect to socket on terminal server
@@ -92,83 +98,125 @@
     def _format_get_command(self, code):
         return code
 
     def _format_set_command(self, code):
         return code
 
     def _cmd(self, cmd, params=NULL, errcheck=True):
-
         # set command data
         to_send = self._encodeCommandData(params)
         # add bytes to define instruction at start of array
         to_send.insert(0, cmd)
         # add unit byte
         to_send.insert(0, self.unit)
 
         received = self._sendRecv(to_send)
         value = self._decodeCommandData(received)
 
         if received[1] == ERROR and errcheck:
             # spontaneous error reply
-            raise ZaberError('Error occured with code: {}'.format(value))
-        """
-        if errcheck:
-            error_code = self._cmd(ERROR, errcheck=False)
-            if error_code != 0:
-                raise ZaberError('Device error code {}'.format(error_code))
-        """
+            raise ZaberError("Error occured with code: {}".format(value))
         return value
 
     def _sendRecv(self, byteArr):
         # only one thread at a time talks to the slide
         with self._lock:
             try:
                 self.sock.send(byteArr)
             except socket.timeout:
-                raise ZaberError('timed out waiting for slide response. this is normal on long moves')
+                raise ZaberTimeoutError(
+                    "timed out sending data to slide. this is normal on long moves"
+                )
             except Exception as e:
-                raise ZaberError('failed to send bytes to slide' + str(e))
-            msg = self.sock.recv(6)
+                raise ZaberError("failed to send bytes to slide" + str(e))
+
+            # now try and receive
+            start_time = time.time()
+            msg = b""
+            while len(msg) < 6 and time.time() - start_time < DEFAULT_TIMEOUT:
+                try:
+                    chunk = self.sock.recv(6 - len(msg))
+                    msg += chunk
+                except socket.timeout:
+                    raise ZaberTimeoutError(
+                        "timed out getting response from slide. normal on long moves."
+                    )
+                except Exception as e:
+                    raise ZaberError("failed to receive bytes to slide" + str(e))
+            if time.time() - start_time >= DEFAULT_TIMEOUT:
+                raise ZaberTimeoutError("timed out gettin response from slide")
         return bytearray(msg)
 
     def _decodeCommandData(self, byteArr):
-        return struct.unpack('<L', byteArr[2:])[0]
+        return struct.unpack("<L", byteArr[2:])[0]
 
     def _encodeCommandData(self, int):
-        return bytearray(struct.pack('<L', int))
+        return bytearray(struct.pack("<L", int))
 
     def _encodeByteArr(self, intArr):
         if len(intArr) != 6:
-            raise ZaberError('must send 6 bytes to slide: cannot send ' +
-                             repr(intArr))
+            raise ZaberError("must send 6 bytes to slide: cannot send " + repr(intArr))
         return bytearray(intArr)
 
     @property
+    def max_position(self):
+        """
+        returns the maximum position of the slide in microsteps
+
+        this is a lazy property, and is only read once from the device
+        """
+        if not hasattr(self, "_max_position"):
+            byteArr = self._encodeByteArr(
+                [UNIT, RETURN_SETTING, MAX_POSITION, NULL, NULL, NULL]
+            )
+            byteArr = self._sendRecv(byteArr)
+            if byteArr[1] == ERROR:
+                raise ZaberError("Error trying to get the max position")
+            self._max_position = self._decodeCommandData(byteArr)
+        return self._max_position
+
+    @property
     def homed(self):
         """
         returns true if the slide has been homed and has a calibrated
         position
         """
-        byteArr = self._encodeByteArr([UNIT, RETURN_SETTING,
-                                       SET_MODE, NULL, NULL, NULL])
+        byteArr = self._encodeByteArr(
+            [UNIT, RETURN_SETTING, SET_MODE, NULL, NULL, NULL]
+        )
         byteArr = self._sendRecv(byteArr)
         if byteArr[1] == ERROR:
-            raise ZaberError('Error trying to get the setting byte')
+            raise ZaberError("Error trying to get the setting byte")
 
         # if 7th bit is set, we have been homed
         if byteArr[2] & 128:
             return True
         else:
             return False
 
     def move(self, position):
         """
         move to a defined position
         """
-        nstep = int(position.to(microstep, equivalencies=self.unit_equivalencies).value)
+        if hasattr(position, "unit"):
+            nstep = int(
+                position.to(microstep, equivalencies=self.unit_equivalencies).value
+            )
+        else:
+            # not a unit, assume microsteps
+            nstep = int(position)
+
+        # valid position?
+        if nstep < 0 or nstep > self.max_position:
+            raise ZaberError(
+                "Cannot move to position {} as it is outside the range of the slide".format(
+                    nstep
+                )
+            )
+
         self._cmd(MOVE_ABSOLUTE, nstep, errcheck=True)
 
     def home(self):
         """
         move the slide to the home position. This is needed after a power on
         to calibrate the slide
         """
@@ -205,16 +253,15 @@
 
     def stop(self):
         """stop the slide"""
         self._cmd(STOP)
 
 
 class ZaberLSEmulator(ZaberLS):
-
-    def __init__(self, host='192.168.1.3', port=10001, unit_equivalencies=None):
+    def __init__(self, host="192.168.1.3", port=10001, unit_equivalencies=None):
         super(ZaberLSEmulator, self).__init__(host, port, unit_equivalencies)
         self.target_position = None
         self.current_position = None
         self._homed = False
         self._moving = False
         self._running_thread = None
         self.abort_thread = False
@@ -242,15 +289,14 @@
         pass
 
     def stop(self):
         self.abort_thread = True
         self._moving = False
 
     def _cmd(self, cmd, params=NULL, errcheck=True):
-
         response_data = params
 
         if cmd == HOME:
             self.target_position = 0 * microstep
             if self.current_position is None:
                 self.current_position = 19000 * microstep
             self.homed = True
@@ -278,15 +324,22 @@
         to_send.insert(0, self.unit)
         return self._decodeCommandData(to_send)
 
     def _move_thread(self):
         self.abort_thread = False
         speed = 9000  # steps/s
         step_time = 0.1  # s
-        nsteps = int(abs((self.target_position - self.current_position).value)/speed/step_time)
-        step = (self.target_position - self.current_position)/nsteps
-        for l in range(nsteps):
+        nsteps = int(
+            abs((self.target_position - self.current_position).value)
+            / speed
+            / step_time
+        )
+        if nsteps == 0:
+            step = 0
+        else:
+            step = (self.target_position - self.current_position) / nsteps
+        for _ in range(nsteps):
             self.current_position += step
             time.sleep(step_time)
             if self.abort_thread:
                 break
         self.moving = False
```

### Comparing `hcam_devices-0.3.0/hcam_devices/gtc/corba.py` & `hcam_devices-1.0.0/hcam_devices/gtc/corba.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 import CosNaming
 from omniORB import CORBA
+
 # not part of this module, copy modules from GCS and place in PYTHONPATH
 import HIPERTELESCOPESERVER
 import os
 
+from ..wamp.utils import call
 
-class TelescopeServer(object):
 
+class TelescopeServer(object):
     def __init__(self):
         self.establish_connection()
 
     def establish_connection(self):
         conn = CORBAConnection()
 
         conn.init_orb()
         conn.resolve_nameservice()
 
         # name of CORBA object to access telescope server
-        name = [CosNaming.NameComponent(id='HIPERTelescopeServer', kind='')]
+        name = [CosNaming.NameComponent(id="HIPERTelescopeServer", kind="")]
 
-        self._server = conn.get_object(name, HIPERTELESCOPESERVER.HIPERTelescopeServer_ifce)
+        self._server = conn.get_object(
+            name, HIPERTELESCOPESERVER.HIPERTelescopeServer_ifce
+        )
 
     @property
     def ready(self):
         try:
             self._server.getTelescopeParams()
         except:
             return False
@@ -39,25 +43,37 @@
             ready = ready and self._server.isM1NoiseBelowThreshold()
         except:
             # failed to read status, don't assume OK.
             ready = False
 
         return ready
 
+    def requestTelescopeOffset(self, dra, ddec):
+        """
+        Request a telescope offset
+        """
+        self._server.requestTelescopeOffset(dra, ddec)
+        # notify autoguider of offset
+        try:
+            call("hipercam.autoguider.rpc.add_relative_dither", dra, ddec)
+        except Exception as err:
+            print("Failed to notify autoguider of offset: {}".format(err))
+
     # pass all unknown method lookups to server
     def __getattr__(self, name):
         return getattr(self._server, name)
 
 
 class CORBAConnection(object):
     """
     A class to handle communication with the GTC CORBA system.
 
     Simply delegates the relevant operations to the current state object.
     """
+
     def __init__(self):
         self.new_state(RawCORBAState)
 
     def new_state(self, state):
         # change the class to a concrete type
         self._state = state
 
@@ -74,86 +90,89 @@
         return self._state.get_object(self, binding_name, cls)
 
 
 class RawCORBAState(object):
     """
     A CORBA state just after creation, with no ORB or nameservice
     """
+
     @staticmethod
     def init_orb(conn):
         # setup CORBA, TODO put correct GTC host here
-        os.environ['ORBDefaultInitRef'] = 'corbaname::161.72.88.75:12008'
-        os.environ['ORBclientCallTimeOutPeriod'] = '2000'  # in milliseconds
+        os.environ["ORBDefaultInitRef"] = "corbaname::161.72.88.75:12008"
+        os.environ["ORBclientCallTimeOutPeriod"] = "2000"  # in milliseconds
         orb = CORBA.ORB_init([], CORBA.ORB_ID)
         conn.orb = orb
         conn.new_state(InitialisedCORBAState)
 
     @staticmethod
     def resolve_nameservice(conn):
-        raise RuntimeError('ORB not initialised')
+        raise RuntimeError("ORB not initialised")
 
     @staticmethod
     def get_object(conn, binding_name, cls):
         """
         Get a reference to a remote object using CORBA
         """
-        raise RuntimeError('ORB not initialised')
+        raise RuntimeError("ORB not initialised")
 
 
 class InitialisedCORBAState(object):
     """
     A CORBA state just after creation, with no ORB or nameservice
     """
+
     @staticmethod
     def init_orb(conn):
-        raise RuntimeError('ORB already initialised')
+        raise RuntimeError("ORB already initialised")
 
     @staticmethod
     def resolve_nameservice(conn):
         # get instance of nameserver from GTC CORBA sever
         try:
-            obj = conn.orb.resolve_initial_references('NameService')
+            obj = conn.orb.resolve_initial_references("NameService")
             rootContext = obj._narrow(CosNaming.NamingContext)
         except CORBA.TRANSIENT:
-            raise IOError('could not connect to GTC CORBA NameServer')
+            raise IOError("could not connect to GTC CORBA NameServer")
 
         if rootContext is None:
-            raise IOError('attempt to get NameServer from GTC failed')
+            raise IOError("attempt to get NameServer from GTC failed")
         conn.rootContext = rootContext
         conn.new_state(ReadyCORBAState)
 
     @staticmethod
     def get_object(conn, binding_name, cls):
         """
         Get a reference to a remote object using CORBA
         """
-        raise RuntimeError('NameService needs to be resolved first')
+        raise RuntimeError("NameService needs to be resolved first")
 
 
 class ReadyCORBAState(object):
     """
     A CORBA state which is ready to retrieve objects
     """
+
     @staticmethod
     def init_orb(conn):
-        raise RuntimeError('ORB already initialised')
+        raise RuntimeError("ORB already initialised")
 
     @staticmethod
     def resolve_nameservice(conn):
         # get instance of nameserver from GTC CORBA sever
-        raise RuntimeError('NameService already resolved')
+        raise RuntimeError("NameService already resolved")
 
     @staticmethod
     def get_object(conn, binding_name, object_cls):
         """
         Get a reference to a remote object using CORBA
         """
         try:
             obj = conn.rootContext.resolve(binding_name)
             narrowed = obj._narrow(object_cls)
         except CORBA.TRANSIENT:
-            raise IOError('Attempt to retrieve object failed')
+            raise IOError("Attempt to retrieve object failed")
 
         if narrowed is None:
-            raise IOError('Attempt to retrieve object got a different class of object')
+            raise IOError("Attempt to retrieve object got a different class of object")
 
         return narrowed
```

### Comparing `hcam_devices-0.3.0/hcam_devices/gtc/headers.py` & `hcam_devices-1.0.0/hcam_devices/gtc/headers.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-0.3.0/hcam_devices/machines/__init__.py` & `hcam_devices-1.0.0/hcam_devices/machines/__init__.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-0.3.0/hcam_devices/machines/connections.yaml` & `hcam_devices-1.0.0/hcam_devices/machines/connections.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     This machine expects a device object in it's initial context.
     The device object should implement try_connect and disconnect methods.
 
     The machine is designed to send connect and disconnect events to a
     second, bound, state machine.
   preamble: |
     setdefault('name', 'anon')  
-    twait = 2  
+    setdefault('twait', 2)  
   root state:
     name: active
     initial: offline
     states:
       - name: offline
         transitions:
           - target: connecting
```

### Comparing `hcam_devices-0.3.0/hcam_devices/machines/controller.yaml` & `hcam_devices-1.0.0/hcam_devices/machines/controller.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -4,17 +4,17 @@
     Connection is handled by a separate connection handler that is bound to this machine.
 
     This machine expects a method in it's initial context called "read". This returns
     a value. We also need a method called "write", which
     accepts a single value and updates the setpoint. Finally, to ensure the setpoint
     is correct on connection, we need a method called "read_setpoint".
   preamble: |
-    poll_time = 2
-    value = setdefault('value', 0)
-    target = setdefault('target', 0)
+    setdefault('poll_time', 2)
+    setdefault('value', 0)
+    setdefault('target', 0)
     last_read = time
     setdefault('name', 'anon')
   root state:
     name: active
     initial: disabled
     states:
       - name: disabled
```

### Comparing `hcam_devices-0.3.0/hcam_devices/machines/gtc.yaml` & `hcam_devices-1.0.0/hcam_devices/machines/gtc.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -14,16 +14,24 @@
     last_read = time
   root state:
     name: active
     initial: offline
     states:
       - name: offline
         transitions:
-        - target: online
-          guard: after(10) and server.ready
+          - target: online
+            guard: after(10) and server.ready
+          - target: offline
+            priority: 1
+            guard: after(240)
+            action: |
+              try:
+                server.establish_connection()
+              except:
+                pass
 
       - name: online
         initial: in position
         transitions:
           - target: offline
             priority: 1
             guard: after(60) and not server.ready
@@ -63,49 +71,48 @@
               - name: in position history
                 type: deep history
 
               - name: nodding disabled
                 transitions:
                   - target: nodding enabled
                     event: start_nodding
-                    action : |
+                    action: |
+                      send('clear_offsets')
                       print('dithering enabled')
                   - target: nodding disabled
-                    event: stop_nodding                
+                    event: stop_nodding
 
               - name: nodding enabled
                 initial: idle
                 transitions:
                   - target: nodding disabled
                     event: stop_nodding
-                    action : |
-                      print('dithering disabled')                      
-
-                states:
-                - name: idle
-                  transitions:
-                    - target: waiting_for_frame
-                      guard: after(0.05)
-                      action: |
-                        send('trigger_exposure')
-                        print('starting exposure')
-
-                - name: waiting_for_frame
-                  transitions:
-                  - target: nodding
-                    event: frame_written
                     action: |
-                      raoff = event.raoff
-                      decoff = event.decoff
-                      print('sending offsets to telescope: ', raoff, decoff)
-                      try:
-                        server.requestTelescopeOffset(raoff, decoff)
-                      except Exception as err:
-                        print('offsets failed: ' + str(err))
-
-                - name: nodding
-                  on exit: print('telescope ready')
-                  transitions:
-                    - target: idle
-                      guard: after(0.2) and server.in_position()
-
+                      print('dithering disabled')
 
+                states:
+                  - name: idle
+                    transitions:
+                      - target: waiting_for_frame
+                        guard: after(0.05)
+                        action: |
+                          send('trigger_exposure')
+                          print('starting exposure')
+
+                  - name: waiting_for_frame
+                    transitions:
+                      - target: nodding
+                        event: frame_written
+                        action: |
+                          raoff = event.raoff
+                          decoff = event.decoff
+                          print('sending offsets to telescope: ', raoff, decoff)
+                          try:
+                            server.requestTelescopeOffset(raoff, decoff)
+                          except Exception as err:
+                            print('offsets failed: ' + str(err))
+
+                  - name: nodding
+                    on exit: print('telescope ready')
+                    transitions:
+                      - target: idle
+                        guard: after(0.2) and server.in_position()
```

### Comparing `hcam_devices-0.3.0/hcam_devices/machines/sensor.yaml` & `hcam_devices-1.0.0/hcam_devices/machines/sensor.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -2,16 +2,16 @@
   name: A basic device sensor for reading values only
   description: |
     Connection is handled by a separate connection handler that is bound to this machine.
 
     This machine expects a method in it's initial context called "read_value". This returns
     a value. There is also a method expected called "read_alarm". The latter is optional.
   preamble: |
-    poll_time = 2
-    value = 0
+    setdefault('poll_time', 2)
+    setdefault('value', 0)
     alarm = False
     setdefault('read_alarm', lambda *args: False)
     last_read = time 
     setdefault('name', 'anon')
   root state:
     name: active
     initial: disabled
```

### Comparing `hcam_devices-0.3.0/hcam_devices/models/ccd.py` & `hcam_devices-1.0.0/hcam_devices/models/ccd.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-0.3.0/hcam_devices/models/flow_sensor.py` & `hcam_devices-1.0.0/hcam_devices/models/flow_sensor.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-0.3.0/hcam_devices/models/meerstetter.py` & `hcam_devices-1.0.0/hcam_devices/models/meerstetter.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-0.3.0/hcam_devices/models/ngc.py` & `hcam_devices-1.0.0/hcam_devices/models/ngc.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-0.3.0/hcam_devices/models/slide.py` & `hcam_devices-1.0.0/hcam_devices/models/slide.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,169 +1,198 @@
 # focal plane slide
 import astropy.units as u
 from astropy.time import Time
 from twisted.logger import Logger
 
 from ..devices.properties import microstep
-from ..devices.zaber import ZaberLS, ZaberLSEmulator
+from ..devices.zaber import ZaberLS, ZaberLSEmulator, ZaberTimeoutError
 from ..machines import create_machine
 
 # the next define ranges for the movement in terms of
 # microsteps, millimetres and pixels
 MIN_MS = 0
-MAX_MS = 1664000
-MIN_PX = 2760.2
-MAX_PX = -1155.3
-MM_PER_MS = 0.000078
-MIN_MM = MM_PER_MS*MIN_MS
-MAX_MM = MM_PER_MS*MAX_MS
+MAX_MS = 672000
+MIN_PX = 1453.1212
+MAX_PX = -125.0606
+MM_PER_MS = 0.00015625
+# END VIK CHANGE ME!
+MIN_MM = MM_PER_MS * MIN_MS
+MAX_MM = MM_PER_MS * MAX_MS
 
 # Standard pixel positions for unblocking and blocking the CCD
-UNBLOCK_POS = 1100.
-BLOCK_POS = -100.
+UNBLOCK_POS = 1100.0
+BLOCK_POS = -100.0
 
 
 def mm_to_ms(value):
-    return MIN_MS + int((MAX_MS - MIN_MS) * (value - MIN_MM) / (MAX_MM-MIN_MM) + 0.5)
+    return MIN_MS + int((MAX_MS - MIN_MS) * (value - MIN_MM) / (MAX_MM - MIN_MM) + 0.5)
 
 
 def ms_to_mm(value):
-    return MIN_MM + (MAX_MM - MIN_MM)*(value - MIN_MS)/(MAX_MS - MIN_MS)
+    return MIN_MM + (MAX_MM - MIN_MM) * (value - MIN_MS) / (MAX_MS - MIN_MS)
 
 
 def px_to_ms(value):
-    return MIN_MS + int((MAX_MS-MIN_MS) * (value - MIN_PX) / (MAX_PX - MIN_PX) + 0.5)
+    return MIN_MS + int((MAX_MS - MIN_MS) * (value - MIN_PX) / (MAX_PX - MIN_PX) + 0.5)
 
 
 def ms_to_px(value):
-    return MIN_PX + (MAX_PX - MIN_PX)*(value - MIN_MS)/(MAX_MS - MIN_MS)
+    return MIN_PX + (MAX_PX - MIN_PX) * (value - MIN_MS) / (MAX_MS - MIN_MS)
 
 
-unit_scale = [
+fps_scale = [
     # from, to, forward, backward
     (u.pix, microstep, px_to_ms, ms_to_px),
-    (u.mm, microstep, mm_to_ms, ms_to_mm)
+    (u.mm, microstep, mm_to_ms, ms_to_mm),
 ]
 
 
-class FocalPlaneSlide(object):
+class LinearStage(object):
     """
-    Focal plane slide.
+    Zaber linear stage.
 
     Uses a Motor state machine to track state, and a Zaber linear stage device to send
     messages.
 
     Periodically updates WAMP server with updates of position and state.
-
-    All positions in pixels
     """
 
     log = Logger()
 
     # can be set by publishing to device level topic of same name
-    settable_attributes = ('target_position',)
-    # all state change triggers are automatically addded as RPC calls
-    # add any extra methods you want exposed here
-    extra_rpc_calls = ('block', 'unblock', 'enable', 'disable', 'reset')
+    settable_attributes = ("target_position",)
+    extra_rpc_calls = ()
+
+    def __init__(self, ip_address, port, equivalencies, emulate=True):
+        # unit handling
+        self.equivalencies = equivalencies
+        # units used for public facing reports
+        self.natural_units = microstep
 
-    def __init__(self, ip_address, port, emulate=True):
         if emulate:
-            self.dev = ZaberLSEmulator(ip_address, port, unit_equivalencies=unit_scale)
+            self.dev = ZaberLSEmulator(
+                ip_address, port, unit_equivalencies=equivalencies
+            )
         else:
-            self.dev = ZaberLS(ip_address, port, unit_equivalencies=unit_scale)
+            self.dev = ZaberLS(ip_address, port, unit_equivalencies=equivalencies)
 
         # state machines to keep track of state
-        self._controller = create_machine('connections',
-                                          initial_context={'device': self, 'name': 'slide'})
-        self._axis = create_machine('motors',
-                                    initial_context={'device': self, 'current': 0*u.pix,
-                                                     'target': 0*u.pix, 'poll_time': 1})
+        self._controller = create_machine(
+            "connections", initial_context={"device": self, "name": "slide"}
+        )
+        self._axis = create_machine(
+            "motors",
+            initial_context={
+                "device": self,
+                "current": 0 * self.natural_units,
+                "target": 0 * self.natural_units,
+                "poll_time": 1,
+            },
+        )
 
-        self.machines = {'connection': self._controller, 'stage': self._axis}
+        self.machines = {"connection": self._controller, "stage": self._axis}
         # axis will recieve events from controller
         self._controller.bind(self._axis)
 
     @property
     def current_position(self):
-        return self._axis.context['current']
+        with u.set_enabled_equivalencies(self.equivalencies):
+            return self._axis.context["current"].to(self.natural_units)
 
     @property
     def target_position(self):
-        return self._axis.context['target']
+        with u.set_enabled_equivalencies(self.equivalencies):
+            return self._axis.context["target"].to(self.natural_units)
 
     @target_position.setter
     def target_position(self, value):
         if not isinstance(value, u.Quantity):
-            value = value * u.pix
-        self._axis.queue('positionSet', position=value)
-
-    def block(self):
-        self.target_position = BLOCK_POS
-        self._axis.queue('move')
-
-    def unblock(self):
-        self.target_position = UNBLOCK_POS
-        self._axis.queue('move')
-
-    def enable(self):
-        self.dev.enable()
-
-    def disable(self):
-        self.dev.disable()
-
-    def reset(self):
-        self.dev.reset()
-        self._controller.queue('disconnect')
+            value = value * self.natural_units
+        self._axis.queue("positionSet", position=value)
 
     def telemetry(self):
         """
         Called periodically to provide a telemetry package for the device
         """
         ts = Time.now()
         return dict(
             timestamp=ts,
-            position=dict(current=self.current_position,
-                          target=self.target_position),
-            state={key: self.machines[key].configuration for key in self.machines}
+            position=dict(current=self.current_position, target=self.target_position),
+            state={key: self.machines[key].configuration for key in self.machines},
         )
 
     # methods and properties required for motor state machine
     # Keep these on slide object rather than moving to Zaber since
     # querying target position of Zaber stage is not implemented
     def home(self):
         try:
             self.dev.home()
+        except ZaberTimeoutError as err:
+            # assume if reply times out it's fine
+            self.log.error("timeout " + str(err))
+            return True
         except Exception as err:
             self.log.error(str(err))
+            return False
+        return True
 
     def homed(self):
         is_homed = False
         try:
             is_homed = self.dev.homed
         except Exception as err:
             self.log.error(str(err))
         return is_homed
 
     def on_target(self):
-        current = self.current_position.to(microstep, equivalencies=unit_scale)
-        target = self.target_position.to(microstep, equivalencies=unit_scale)
-        delta = abs((current-target).value)
-        return int(delta) < 5
+        try:
+            current = self.current_position
+            target = self.target_position
+            if not isinstance(current, u.Quantity):
+                current = current * self.natural_units
+            if not isinstance(target, u.Quantity):
+                target = target * self.natural_units
+            current = self.current_position.to(
+                microstep, equivalencies=self.equivalencies
+            )
+            target = self.target_position.to(
+                microstep, equivalencies=self.equivalencies
+            )
+            delta = abs((current - target).value)
+            return int(delta) < 5
+        except Exception as err:
+            self.log.error(str(err))
+            return False
 
     def move(self, value):
         if not isinstance(value, u.Quantity):
-            # assume pixels
-            value = value * u.pix
+            # no units, assume natural units
+            value = value * self.natural_units
         try:
             self.dev.move(value)
+        except ZaberTimeoutError as err:
+            # assume if reply times out it's fine
+            self.log.error("timeout " + str(err))
+            return True
         except Exception as err:
             self.log.error(str(err))
+            return False
+        return True
 
     def stop(self):
-        self.dev.stop()
+        try:
+            self.dev.stop()
+        except ZaberTimeoutError as err:
+            # assume if reply times out it's fine
+            self.log.error("timeout " + str(err))
+            return True
+        except Exception as err:
+            self.log.error(str(err))
+            return False
+        return True
 
     def try_connect(self):
         """
         Always needs to be defined.  Returns True on successful connection attempt.
         """
         # attempt connection, return true to allow device state to change
         try:
@@ -177,9 +206,53 @@
 
     def poll(self):
         """
         State machines mean that this is automatically polled.
 
         Update current position and return True/False for moving state
         """
-        current_position = self.dev.position.to(u.pix, equivalencies=unit_scale)
+        try:
+            current_position = self.dev.position.to(
+                self.natural_units, equivalencies=self.equivalencies
+            )
+            moving = self.dev.moving
+        except Exception as err:
+            self.log.error(str(err))
+            current_position = 0 * self.natural_units
+            moving = True
         return current_position, self.dev.moving
+
+
+class FocalPlaneSlide(LinearStage):
+    """
+    Focal plane slide.
+
+    Uses the unit equivalencies defined above and adds "block" etc as RPC calls
+
+    All positions in pixels
+    """
+
+    # all state change triggers are automatically addded as RPC calls
+    # add any extra methods you want exposed here
+    extra_rpc_calls = ("block", "unblock", "enable", "disable", "reset")
+
+    def __init__(self, ip_address, port, emulate=True):
+        super().__init__(ip_address, port, fps_scale, emulate)
+        self.natural_units = u.pix
+
+    def block(self):
+        self.target_position = BLOCK_POS
+        self._axis.queue("move")
+
+    def unblock(self):
+        self.target_position = UNBLOCK_POS
+        self._axis.queue("move")
+
+    def enable(self):
+        self.dev.enable()
+
+    def disable(self):
+        self.dev.disable()
+
+    def reset(self):
+        self.dev.reset()
+        self._controller.queue("disconnect")
```

### Comparing `hcam_devices-0.3.0/hcam_devices/models/vac_gauge.py` & `hcam_devices-1.0.0/hcam_devices/models/vac_gauge.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-0.3.0/hcam_devices/testing/axis.py` & `hcam_devices-1.0.0/hcam_devices/testing/axis.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-0.3.0/hcam_devices/testing/fakeserial.py` & `hcam_devices-1.0.0/hcam_devices/testing/fakeserial.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         self.baudrate = baudrate
         self.bytesize = bytesize
         self.stopbits = stopbits
         self.xonxoff = xonxoff
         self.rtscts = rtscts
         self._isOpen = True
         self._receivedData = ""
-        self._data = ""
+        self._data = b""
 
     @classmethod
     def register_command(cls, name, type_conv):
         def inner(func):
             cls.registered_commands[name] = (func, type_conv)
             return func
         return inner
@@ -32,34 +32,34 @@
     def open(self):
         self._isOpen = True
 
     def close(self):
         self._isOpen = False
 
     def write(self, string):
-        self._receivedData += string
+        self._receivedData += string.decode()
         self._process_received()
 
     def read(self, n=1):
         """
         reads n characters from data buffer
         """
         s = self._data[0:n]
         self._data = self._data[n:]
-        return s
+        return s.encode()
 
     def readline(self):
         try:
             returnIndex = self._data.index("\n")
         except ValueError:
             return ""
         else:
             s = self._data[0:returnIndex+1]
             self._data = self._data[returnIndex+1:]
-            return s
+            return s.encode()
 
     def __str__(self):
         template = "Serial<id=0xa81c10, open={}>(port='{}', baudrate={},"
         template += " bytesize={:d}, parity='{}', stopbits={:d}, xonxoff={:d}, rtscts={:d})"
         return template.format(
             str(self.isOpen()), self.port, self.baudrate,
             self.bytesize, self.parity, self.stopbits, self.xonxoff,
```

### Comparing `hcam_devices-0.3.0/hcam_devices/testing/properties.py` & `hcam_devices-1.0.0/hcam_devices/testing/properties.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-0.3.0/hcam_devices/testing/sensors.py` & `hcam_devices-1.0.0/hcam_devices/testing/sensors.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-0.3.0/hcam_devices/utils/filesystem.py` & `hcam_devices-1.0.0/hcam_devices/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-0.3.0/hcam_devices/utils/obsmodes.py` & `hcam_devices-1.0.0/hcam_devices/utils/obsmodes.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-0.3.0/hcam_devices/wamp/__init__.py` & `hcam_devices-1.0.0/hcam_devices/wamp/__init__.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-0.3.0/hcam_devices/wamp/utils/__init__.py` & `hcam_devices-1.0.0/hcam_devices/wamp/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-0.3.0/hcam_devices.egg-info/PKG-INFO` & `hcam_devices-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
-Name: hcam-devices
-Version: 0.3.0
+Name: hcam_devices
+Version: 1.0.0
 Summary: Device Communication via WAMP for HiPerCAM
 Home-page: https://github.com/HiPERCAM/hcam_devices
+Download-URL: https://github.com/HiPERCAM/hcam_devices/archive/v1.0.0.tar.gz
 Author: Stuart Littlefair
 Author-email: s.littlefair@shef.ac.uk
 License: MIT license
-Download-URL: https://github.com/HiPERCAM/hcam_devices/archive/v0.3.0.tar.gz
 Keywords: hcam_devices
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
@@ -143,9 +142,7 @@
 History
 =======
 
 0.1.0 (2020-06-05)
 ------------------
 
 * First release on PyPI.
-
-
```

### Comparing `hcam_devices-0.3.0/hcam_devices.egg-info/SOURCES.txt` & `hcam_devices-1.0.0/hcam_devices.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -22,22 +22,18 @@
 hcam_devices/devices/pdr900.py
 hcam_devices/devices/properties.py
 hcam_devices/devices/unichiller.py
 hcam_devices/devices/zaber.py
 hcam_devices/gtc/corba.py
 hcam_devices/gtc/headers.py
 hcam_devices/machines/__init__.py
-hcam_devices/machines/connections.png
 hcam_devices/machines/connections.yaml
 hcam_devices/machines/controller.yaml
-hcam_devices/machines/gtc.png
 hcam_devices/machines/gtc.yaml
-hcam_devices/machines/motors.png
 hcam_devices/machines/motors.yaml
-hcam_devices/machines/sensor.png
 hcam_devices/machines/sensor.yaml
 hcam_devices/models/__init__.py
 hcam_devices/models/ccd.py
 hcam_devices/models/compo.py
 hcam_devices/models/flow_sensor.py
 hcam_devices/models/meerstetter.py
 hcam_devices/models/ngc.py
@@ -55,8 +51,11 @@
 hcam_devices/wamp/__init__.py
 hcam_devices/wamp/utils/__init__.py
 scripts/do_wamp_call
 scripts/gtcserver
 scripts/hserver
 scripts/hwlogger
 scripts/hwserver
-scripts/make_diagrams.py
+scripts/make_diagrams.py
+scripts/show_telemetry
+scripts/tcp_serial_bridge
+scripts/zaber_ascii
```

### Comparing `hcam_devices-0.3.0/scripts/do_wamp_call` & `hcam_devices-1.0.0/scripts/do_wamp_call`

 * *Files identical despite different names*

### Comparing `hcam_devices-0.3.0/scripts/gtcserver` & `hcam_devices-1.0.0/scripts/hserver`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 #! /usr/bin/env python
 import argparse
+import os
 
 from autobahn.twisted.component import Component, run
 
-from hcam_devices.components import GTCComponent
+from hcam_devices.components import NGCComponent
+
+URL = os.getenv("WAMP_SERVER", "192.168.1.2")
 
 transport_cfg = dict(
-    type='websocket',
-    url='ws://localhost:8080/ws',
+    type="websocket",
+    url="ws://{}:8080/ws".format(URL),
     max_retries=-1,
     max_retry_delay=30,
 )
 
-
 parser = argparse.ArgumentParser()
-parser.add_argument('path', help='full path where FITS files of raw data are written')
-parser.add_argument('-e', '--emulate', help='use emulated hardware', action='store_true')
+parser.add_argument(
+    "-e", "--emulate", help="use emulated hardware", action="store_true"
+)
 args = parser.parse_args()
+if args.emulate:
+    print("EMULATION MODE")
 
-gtc = Component(
-    transports=transport_cfg, realm='realm1', session_factory=GTCComponent,
-    extra=dict(name='GTC', emulate=args.emulate, path=args.path)
+ngc = Component(
+    transports=transport_cfg,
+    realm="realm1",
+    session_factory=NGCComponent,
+    extra=dict(name="NGC", emulate=args.emulate),
 )
 
-run([gtc])
+run([ngc])
```

### Comparing `hcam_devices-0.3.0/scripts/hserver` & `hcam_devices-1.0.0/scripts/gtcserver`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 #! /usr/bin/env python
 import argparse
+import os
 
 from autobahn.twisted.component import Component, run
 
-from hcam_devices.components import NGCComponent
+from hcam_devices.components import GTCComponent
+
+URL = os.getenv("WAMP_SERVER", "192.168.1.2")
 
 transport_cfg = dict(
-    type='websocket',
-    url='ws://localhost:8080/ws',
+    type="websocket",
+    url="ws://{}:8080/ws".format(URL),
     max_retries=-1,
     max_retry_delay=30,
 )
 
+
 parser = argparse.ArgumentParser()
-parser.add_argument('-e', '--emulate', help='use emulated hardware', action='store_true')
+parser.add_argument("path", help="full path where FITS files of raw data are written")
+parser.add_argument(
+    "-e", "--emulate", help="use emulated hardware", action="store_true"
+)
 args = parser.parse_args()
-if args.emulate:
-    print('EMULATION MODE')
-    
-ngc = Component(
-    transports=transport_cfg, realm='realm1', session_factory=NGCComponent,
-    extra=dict(name='NGC', emulate=args.emulate)
+
+gtc = Component(
+    transports=transport_cfg,
+    realm="realm1",
+    session_factory=GTCComponent,
+    extra=dict(name="GTC", emulate=args.emulate, path=args.path),
 )
 
-run([ngc])
+run([gtc])
```

