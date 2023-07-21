# Comparing `tmp/spluscalib-0.3.2.tar.gz` & `tmp/spluscalib-0.3.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spluscalib-0.3.2.tar", last modified: Fri Jul 21 00:24:07 2023, max compression
+gzip compressed data, was "spluscalib-0.3.21.tar", last modified: Fri Jul 21 00:30:47 2023, max compression
```

## Comparing `spluscalib-0.3.2.tar` & `spluscalib-0.3.21.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2023-07-21 00:24:07.324988 spluscalib-0.3.2/
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    35149 2021-05-14 02:47:40.000000 spluscalib-0.3.2/LICENSE
--rw-rw-r--   0 felipe    (1000) felipe    (1000)      320 2021-06-24 00:10:00.000000 spluscalib-0.3.2/MANIFEST.in
--rw-rw-r--   0 felipe    (1000) felipe    (1000)      304 2023-07-21 00:24:07.324988 spluscalib-0.3.2/PKG-INFO
--rw-rw-r--   0 felipe    (1000) felipe    (1000)      153 2021-11-03 23:00:24.000000 spluscalib-0.3.2/README.md
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    22214 2021-06-24 00:09:46.000000 spluscalib-0.3.2/documentation.txt
--rw-rw-r--   0 felipe    (1000) felipe    (1000)       38 2023-07-21 00:24:07.324988 spluscalib-0.3.2/setup.cfg
--rw-rw-r--   0 felipe    (1000) felipe    (1000)      843 2023-07-21 00:23:39.000000 spluscalib-0.3.2/setup.py
-drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2023-07-21 00:24:07.316988 spluscalib-0.3.2/spluscalib/
--rw-rw-r--   0 felipe    (1000) felipe    (1000)        0 2021-05-14 02:47:40.000000 spluscalib-0.3.2/spluscalib/__init__.py
-drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2023-07-21 00:24:07.320989 spluscalib-0.3.2/spluscalib/additionalsteps/
--rw-rw-r--   0 felipe    (1000) felipe    (1000)        0 2021-05-14 02:47:40.000000 spluscalib-0.3.2/spluscalib/additionalsteps/__init__.py
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    10844 2022-05-10 20:35:46.000000 spluscalib-0.3.2/spluscalib/additionalsteps/combine_calibration_catalogs.py
--rw-rw-r--   0 felipe    (1000) felipe    (1000)     8615 2021-10-24 08:28:10.000000 spluscalib-0.3.2/spluscalib/additionalsteps/compute_XY_maps.py
--rw-rw-r--   0 felipe    (1000) felipe    (1000)     6498 2022-04-26 04:41:42.000000 spluscalib-0.3.2/spluscalib/additionalsteps/fit_inst_offsets.py
--rw-rw-r--   0 felipe    (1000) felipe    (1000)     7383 2022-04-26 04:41:42.000000 spluscalib-0.3.2/spluscalib/additionalsteps/fit_zp_offsets.py
--rw-rw-r--   0 felipe    (1000) felipe    (1000)     5765 2021-06-05 10:32:36.000000 spluscalib-0.3.2/spluscalib/dust_laws.py
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    18909 2023-07-06 23:27:20.000000 spluscalib-0.3.2/spluscalib/pipeline.py
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    24012 2023-05-24 18:21:08.000000 spluscalib-0.3.2/spluscalib/pipeline_backup.py
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    22256 2023-06-29 19:03:28.000000 spluscalib-0.3.2/spluscalib/quality_check.py
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    12013 2022-04-28 12:37:51.000000 spluscalib-0.3.2/spluscalib/quality_check_PSF.py
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    12039 2022-03-07 07:29:08.000000 spluscalib-0.3.2/spluscalib/quality_check_PSFbackup.py
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    12938 2021-10-21 22:08:52.000000 spluscalib-0.3.2/spluscalib/sed_fitting.py
-drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2023-07-21 00:24:07.320989 spluscalib-0.3.2/spluscalib/steps/
--rw-rw-r--   0 felipe    (1000) felipe    (1000)        0 2021-05-14 02:47:40.000000 spluscalib-0.3.2/spluscalib/steps/__init__.py
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    19310 2022-05-11 17:52:21.000000 spluscalib-0.3.2/spluscalib/steps/calibration_catalog.py
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    12795 2022-05-10 20:35:46.000000 spluscalib-0.3.2/spluscalib/steps/calibration_diagnostic.py
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    12846 2023-07-15 07:02:23.000000 spluscalib-0.3.2/spluscalib/steps/calibration_external.py
--rw-rw-r--   0 felipe    (1000) felipe    (1000)     5589 2022-04-21 05:03:07.000000 spluscalib-0.3.2/spluscalib/steps/calibration_finalzp.py
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    18290 2023-07-18 11:34:33.000000 spluscalib-0.3.2/spluscalib/steps/calibration_gaiascale.py
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    13197 2023-07-15 20:15:36.000000 spluscalib-0.3.2/spluscalib/steps/calibration_internal.py
--rw-rw-r--   0 felipe    (1000) felipe    (1000)     8732 2022-04-21 16:01:27.000000 spluscalib-0.3.2/spluscalib/steps/calibration_stloc.py
--rw-rw-r--   0 felipe    (1000) felipe    (1000)     9990 2023-07-06 23:49:42.000000 spluscalib-0.3.2/spluscalib/steps/copy_images.py
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    19129 2021-09-15 19:22:31.000000 spluscalib-0.3.2/spluscalib/steps/correction_aper.py
--rw-rw-r--   0 felipe    (1000) felipe    (1000)     9586 2021-10-28 04:09:28.000000 spluscalib-0.3.2/spluscalib/steps/correction_xy.py
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    15158 2023-07-15 22:37:56.000000 spluscalib-0.3.2/spluscalib/steps/crossmatch.py
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    29037 2023-05-27 18:28:45.000000 spluscalib-0.3.2/spluscalib/steps/photometry_ID.py
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    10485 2023-07-06 23:28:14.000000 spluscalib-0.3.2/spluscalib/steps/photometry_aperimages.py
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    22584 2023-07-06 21:50:25.000000 spluscalib-0.3.2/spluscalib/steps/photometry_dual.py
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    17542 2022-04-21 05:03:07.000000 spluscalib-0.3.2/spluscalib/steps/photometry_master.py
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    12159 2022-09-20 18:44:12.000000 spluscalib-0.3.2/spluscalib/steps/photometry_psf.py
--rw-rw-r--   0 felipe    (1000) felipe    (1000)     9710 2023-07-06 20:58:53.000000 spluscalib-0.3.2/spluscalib/steps/photometry_single.py
-drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2023-07-21 00:24:07.324988 spluscalib-0.3.2/spluscalib/steps/resources/
--rwxrwxr-x   0 felipe    (1000) felipe    (1000)      572 2020-09-04 18:32:49.000000 spluscalib-0.3.2/spluscalib/steps/resources/SExsplus.param
--rwxrwxr-x   0 felipe    (1000) felipe    (1000)     3008 2021-06-04 20:30:56.000000 spluscalib-0.3.2/spluscalib/steps/resources/SExsplus.sex
--rw-rw-r--   0 felipe    (1000) felipe    (1000)     2153 2023-07-15 19:48:08.000000 spluscalib-0.3.2/spluscalib/steps/resources/default_config.conf
--rw-------   0 felipe    (1000) felipe    (1000)    12302 2021-05-19 06:03:20.000000 spluscalib-0.3.2/spluscalib/steps/resources/dophot_paramdefault
--rw-rw-r--   0 felipe    (1000) felipe    (1000)      973 2021-05-18 02:36:19.000000 spluscalib-0.3.2/spluscalib/steps/resources/swarpsplus.swarp
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   210720 2023-07-21 00:10:32.000000 spluscalib-0.3.2/spluscalib/utils.py
-drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2023-07-21 00:24:07.324988 spluscalib-0.3.2/spluscalib/vacs/
--rw-rw-r--   0 felipe    (1000) felipe    (1000)        0 2021-05-14 02:47:40.000000 spluscalib-0.3.2/spluscalib/vacs/__init__.py
-drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2023-07-21 00:24:07.320989 spluscalib-0.3.2/spluscalib.egg-info/
--rw-rw-r--   0 felipe    (1000) felipe    (1000)      304 2023-07-21 00:24:07.000000 spluscalib-0.3.2/spluscalib.egg-info/PKG-INFO
--rw-rw-r--   0 felipe    (1000) felipe    (1000)     1822 2023-07-21 00:24:07.000000 spluscalib-0.3.2/spluscalib.egg-info/SOURCES.txt
--rw-rw-r--   0 felipe    (1000) felipe    (1000)        1 2023-07-21 00:24:07.000000 spluscalib-0.3.2/spluscalib.egg-info/dependency_links.txt
--rw-rw-r--   0 felipe    (1000) felipe    (1000)       79 2023-07-21 00:24:07.000000 spluscalib-0.3.2/spluscalib.egg-info/requires.txt
--rw-rw-r--   0 felipe    (1000) felipe    (1000)       26 2023-07-21 00:24:07.000000 spluscalib-0.3.2/spluscalib.egg-info/top_level.txt
-drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2023-07-21 00:24:07.324988 spluscalib-0.3.2/stellarlibrary/
--rw-rw-r--   0 felipe    (1000) felipe    (1000)        1 2021-05-14 02:47:40.000000 spluscalib-0.3.2/stellarlibrary/__init__.py
--rw-rw-r--   0 felipe    (1000) felipe    (1000)     5766 2021-08-18 02:59:55.000000 spluscalib-0.3.2/stellarlibrary/dust_laws.py
--rw-rw-r--   0 felipe    (1000) felipe    (1000)     2789 2022-06-14 05:33:30.000000 spluscalib-0.3.2/stellarlibrary/generate_models_photometry.py
--rw-rw-r--   0 felipe    (1000) felipe    (1000)     2840 2023-07-06 23:12:28.000000 spluscalib-0.3.2/stellarlibrary/generate_models_photometry_iDR5.py
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    23858 2023-07-06 23:26:33.000000 spluscalib-0.3.2/stellarlibrary/models.py
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    11821 2021-09-14 16:27:59.000000 spluscalib-0.3.2/stellarlibrary/prior.py
+drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2023-07-21 00:30:47.665761 spluscalib-0.3.21/
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    35149 2021-05-14 02:47:40.000000 spluscalib-0.3.21/LICENSE
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)      320 2021-06-24 00:10:00.000000 spluscalib-0.3.21/MANIFEST.in
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)      305 2023-07-21 00:30:47.665761 spluscalib-0.3.21/PKG-INFO
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)      153 2021-11-03 23:00:24.000000 spluscalib-0.3.21/README.md
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    22214 2021-06-24 00:09:46.000000 spluscalib-0.3.21/documentation.txt
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)       38 2023-07-21 00:30:47.665761 spluscalib-0.3.21/setup.cfg
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)      857 2023-07-21 00:30:22.000000 spluscalib-0.3.21/setup.py
+drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2023-07-21 00:30:47.657761 spluscalib-0.3.21/spluscalib/
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)        0 2021-05-14 02:47:40.000000 spluscalib-0.3.21/spluscalib/__init__.py
+drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2023-07-21 00:30:47.661761 spluscalib-0.3.21/spluscalib/additionalsteps/
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)        0 2021-05-14 02:47:40.000000 spluscalib-0.3.21/spluscalib/additionalsteps/__init__.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    10844 2022-05-10 20:35:46.000000 spluscalib-0.3.21/spluscalib/additionalsteps/combine_calibration_catalogs.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)     8615 2021-10-24 08:28:10.000000 spluscalib-0.3.21/spluscalib/additionalsteps/compute_XY_maps.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)     6498 2022-04-26 04:41:42.000000 spluscalib-0.3.21/spluscalib/additionalsteps/fit_inst_offsets.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)     7383 2022-04-26 04:41:42.000000 spluscalib-0.3.21/spluscalib/additionalsteps/fit_zp_offsets.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)     5765 2021-06-05 10:32:36.000000 spluscalib-0.3.21/spluscalib/dust_laws.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    18909 2023-07-06 23:27:20.000000 spluscalib-0.3.21/spluscalib/pipeline.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    24012 2023-05-24 18:21:08.000000 spluscalib-0.3.21/spluscalib/pipeline_backup.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    22256 2023-06-29 19:03:28.000000 spluscalib-0.3.21/spluscalib/quality_check.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    12013 2022-04-28 12:37:51.000000 spluscalib-0.3.21/spluscalib/quality_check_PSF.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    12039 2022-03-07 07:29:08.000000 spluscalib-0.3.21/spluscalib/quality_check_PSFbackup.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    12938 2021-10-21 22:08:52.000000 spluscalib-0.3.21/spluscalib/sed_fitting.py
+drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2023-07-21 00:30:47.665761 spluscalib-0.3.21/spluscalib/steps/
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)        0 2021-05-14 02:47:40.000000 spluscalib-0.3.21/spluscalib/steps/__init__.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    19310 2022-05-11 17:52:21.000000 spluscalib-0.3.21/spluscalib/steps/calibration_catalog.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    12795 2022-05-10 20:35:46.000000 spluscalib-0.3.21/spluscalib/steps/calibration_diagnostic.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    12846 2023-07-15 07:02:23.000000 spluscalib-0.3.21/spluscalib/steps/calibration_external.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)     5589 2022-04-21 05:03:07.000000 spluscalib-0.3.21/spluscalib/steps/calibration_finalzp.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    18290 2023-07-18 11:34:33.000000 spluscalib-0.3.21/spluscalib/steps/calibration_gaiascale.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    13197 2023-07-15 20:15:36.000000 spluscalib-0.3.21/spluscalib/steps/calibration_internal.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)     8732 2022-04-21 16:01:27.000000 spluscalib-0.3.21/spluscalib/steps/calibration_stloc.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)     9990 2023-07-06 23:49:42.000000 spluscalib-0.3.21/spluscalib/steps/copy_images.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    19129 2021-09-15 19:22:31.000000 spluscalib-0.3.21/spluscalib/steps/correction_aper.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)     9586 2021-10-28 04:09:28.000000 spluscalib-0.3.21/spluscalib/steps/correction_xy.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    15158 2023-07-15 22:37:56.000000 spluscalib-0.3.21/spluscalib/steps/crossmatch.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    29037 2023-05-27 18:28:45.000000 spluscalib-0.3.21/spluscalib/steps/photometry_ID.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    10485 2023-07-06 23:28:14.000000 spluscalib-0.3.21/spluscalib/steps/photometry_aperimages.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    22584 2023-07-06 21:50:25.000000 spluscalib-0.3.21/spluscalib/steps/photometry_dual.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    17542 2022-04-21 05:03:07.000000 spluscalib-0.3.21/spluscalib/steps/photometry_master.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    12159 2022-09-20 18:44:12.000000 spluscalib-0.3.21/spluscalib/steps/photometry_psf.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)     9710 2023-07-06 20:58:53.000000 spluscalib-0.3.21/spluscalib/steps/photometry_single.py
+drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2023-07-21 00:30:47.665761 spluscalib-0.3.21/spluscalib/steps/resources/
+-rwxrwxr-x   0 felipe    (1000) felipe    (1000)      572 2020-09-04 18:32:49.000000 spluscalib-0.3.21/spluscalib/steps/resources/SExsplus.param
+-rwxrwxr-x   0 felipe    (1000) felipe    (1000)     3008 2021-06-04 20:30:56.000000 spluscalib-0.3.21/spluscalib/steps/resources/SExsplus.sex
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)     2153 2023-07-15 19:48:08.000000 spluscalib-0.3.21/spluscalib/steps/resources/default_config.conf
+-rw-------   0 felipe    (1000) felipe    (1000)    12302 2021-05-19 06:03:20.000000 spluscalib-0.3.21/spluscalib/steps/resources/dophot_paramdefault
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)      973 2021-05-18 02:36:19.000000 spluscalib-0.3.21/spluscalib/steps/resources/swarpsplus.swarp
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   210720 2023-07-21 00:10:32.000000 spluscalib-0.3.21/spluscalib/utils.py
+drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2023-07-21 00:30:47.665761 spluscalib-0.3.21/spluscalib/vacs/
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)        0 2021-05-14 02:47:40.000000 spluscalib-0.3.21/spluscalib/vacs/__init__.py
+drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2023-07-21 00:30:47.661761 spluscalib-0.3.21/spluscalib.egg-info/
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)      305 2023-07-21 00:30:47.000000 spluscalib-0.3.21/spluscalib.egg-info/PKG-INFO
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)     1822 2023-07-21 00:30:47.000000 spluscalib-0.3.21/spluscalib.egg-info/SOURCES.txt
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)        1 2023-07-21 00:30:47.000000 spluscalib-0.3.21/spluscalib.egg-info/dependency_links.txt
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)       89 2023-07-21 00:30:47.000000 spluscalib-0.3.21/spluscalib.egg-info/requires.txt
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)       26 2023-07-21 00:30:47.000000 spluscalib-0.3.21/spluscalib.egg-info/top_level.txt
+drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2023-07-21 00:30:47.665761 spluscalib-0.3.21/stellarlibrary/
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)        1 2021-05-14 02:47:40.000000 spluscalib-0.3.21/stellarlibrary/__init__.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)     5766 2021-08-18 02:59:55.000000 spluscalib-0.3.21/stellarlibrary/dust_laws.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)     2789 2022-06-14 05:33:30.000000 spluscalib-0.3.21/stellarlibrary/generate_models_photometry.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)     2840 2023-07-06 23:12:28.000000 spluscalib-0.3.21/stellarlibrary/generate_models_photometry_iDR5.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    23858 2023-07-06 23:26:33.000000 spluscalib-0.3.21/stellarlibrary/models.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    11821 2021-09-14 16:27:59.000000 spluscalib-0.3.21/stellarlibrary/prior.py
```

### Comparing `spluscalib-0.3.2/LICENSE` & `spluscalib-0.3.21/LICENSE`

 * *Files identical despite different names*

### Comparing `spluscalib-0.3.2/documentation.txt` & `spluscalib-0.3.21/documentation.txt`

 * *Files identical despite different names*

### Comparing `spluscalib-0.3.2/setup.py` & `spluscalib-0.3.21/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import setuptools
 
 setuptools.setup(
    name='spluscalib',
-   version='0.3.2',
+   version='0.3.21',
    description='S-PLUS calibration pipeline',
    author='Felipe Almeida Fernandes',
    author_email='felipefer42@gmail.com',
    packages=setuptools.find_packages(),
    install_requires=['astropy', 'astroquery', 'sfdmap', 'numpy',
                      'pandas', 'scipy', 'sklearn', 'matplotlib',
-                     'shapely', 'Pillow'],
+                     'shapely', 'Pillow', 'termcolor'],
    url='https://github.com/felipefer42/spluscalib',
    python_requires='>3.6.0',
    include_package_data=True
 )
 
 # python setup.py sdist
 # python setup.py bdist_wheel
```

### Comparing `spluscalib-0.3.2/spluscalib/additionalsteps/combine_calibration_catalogs.py` & `spluscalib-0.3.21/spluscalib/additionalsteps/combine_calibration_catalogs.py`

 * *Files identical despite different names*

### Comparing `spluscalib-0.3.2/spluscalib/additionalsteps/compute_XY_maps.py` & `spluscalib-0.3.21/spluscalib/additionalsteps/compute_XY_maps.py`

 * *Files identical despite different names*

### Comparing `spluscalib-0.3.2/spluscalib/additionalsteps/fit_inst_offsets.py` & `spluscalib-0.3.21/spluscalib/additionalsteps/fit_inst_offsets.py`

 * *Files identical despite different names*

### Comparing `spluscalib-0.3.2/spluscalib/additionalsteps/fit_zp_offsets.py` & `spluscalib-0.3.21/spluscalib/additionalsteps/fit_zp_offsets.py`

 * *Files identical despite different names*

### Comparing `spluscalib-0.3.2/spluscalib/dust_laws.py` & `spluscalib-0.3.21/spluscalib/dust_laws.py`

 * *Files identical despite different names*

### Comparing `spluscalib-0.3.2/spluscalib/pipeline.py` & `spluscalib-0.3.21/spluscalib/pipeline.py`

 * *Files identical despite different names*

### Comparing `spluscalib-0.3.2/spluscalib/pipeline_backup.py` & `spluscalib-0.3.21/spluscalib/pipeline_backup.py`

 * *Files identical despite different names*

### Comparing `spluscalib-0.3.2/spluscalib/quality_check.py` & `spluscalib-0.3.21/spluscalib/quality_check.py`

 * *Files identical despite different names*

### Comparing `spluscalib-0.3.2/spluscalib/quality_check_PSF.py` & `spluscalib-0.3.21/spluscalib/quality_check_PSF.py`

 * *Files identical despite different names*

### Comparing `spluscalib-0.3.2/spluscalib/quality_check_PSFbackup.py` & `spluscalib-0.3.21/spluscalib/quality_check_PSFbackup.py`

 * *Files identical despite different names*

### Comparing `spluscalib-0.3.2/spluscalib/sed_fitting.py` & `spluscalib-0.3.21/spluscalib/sed_fitting.py`

 * *Files identical despite different names*

### Comparing `spluscalib-0.3.2/spluscalib/steps/calibration_catalog.py` & `spluscalib-0.3.21/spluscalib/steps/calibration_catalog.py`

 * *Files identical despite different names*

### Comparing `spluscalib-0.3.2/spluscalib/steps/calibration_diagnostic.py` & `spluscalib-0.3.21/spluscalib/steps/calibration_diagnostic.py`

 * *Files identical despite different names*

### Comparing `spluscalib-0.3.2/spluscalib/steps/calibration_external.py` & `spluscalib-0.3.21/spluscalib/steps/calibration_external.py`

 * *Files identical despite different names*

### Comparing `spluscalib-0.3.2/spluscalib/steps/calibration_finalzp.py` & `spluscalib-0.3.21/spluscalib/steps/calibration_finalzp.py`

 * *Files identical despite different names*

### Comparing `spluscalib-0.3.2/spluscalib/steps/calibration_gaiascale.py` & `spluscalib-0.3.21/spluscalib/steps/calibration_gaiascale.py`

 * *Files identical despite different names*

### Comparing `spluscalib-0.3.2/spluscalib/steps/calibration_internal.py` & `spluscalib-0.3.21/spluscalib/steps/calibration_internal.py`

 * *Files identical despite different names*

### Comparing `spluscalib-0.3.2/spluscalib/steps/calibration_stloc.py` & `spluscalib-0.3.21/spluscalib/steps/calibration_stloc.py`

 * *Files identical despite different names*

### Comparing `spluscalib-0.3.2/spluscalib/steps/copy_images.py` & `spluscalib-0.3.21/spluscalib/steps/copy_images.py`

 * *Files identical despite different names*

### Comparing `spluscalib-0.3.2/spluscalib/steps/correction_aper.py` & `spluscalib-0.3.21/spluscalib/steps/correction_aper.py`

 * *Files identical despite different names*

### Comparing `spluscalib-0.3.2/spluscalib/steps/correction_xy.py` & `spluscalib-0.3.21/spluscalib/steps/correction_xy.py`

 * *Files identical despite different names*

### Comparing `spluscalib-0.3.2/spluscalib/steps/crossmatch.py` & `spluscalib-0.3.21/spluscalib/steps/crossmatch.py`

 * *Files identical despite different names*

### Comparing `spluscalib-0.3.2/spluscalib/steps/photometry_ID.py` & `spluscalib-0.3.21/spluscalib/steps/photometry_ID.py`

 * *Files identical despite different names*

### Comparing `spluscalib-0.3.2/spluscalib/steps/photometry_aperimages.py` & `spluscalib-0.3.21/spluscalib/steps/photometry_aperimages.py`

 * *Files identical despite different names*

### Comparing `spluscalib-0.3.2/spluscalib/steps/photometry_dual.py` & `spluscalib-0.3.21/spluscalib/steps/photometry_dual.py`

 * *Files identical despite different names*

### Comparing `spluscalib-0.3.2/spluscalib/steps/photometry_master.py` & `spluscalib-0.3.21/spluscalib/steps/photometry_master.py`

 * *Files identical despite different names*

### Comparing `spluscalib-0.3.2/spluscalib/steps/photometry_psf.py` & `spluscalib-0.3.21/spluscalib/steps/photometry_psf.py`

 * *Files identical despite different names*

### Comparing `spluscalib-0.3.2/spluscalib/steps/photometry_single.py` & `spluscalib-0.3.21/spluscalib/steps/photometry_single.py`

 * *Files identical despite different names*

### Comparing `spluscalib-0.3.2/spluscalib/steps/resources/SExsplus.param` & `spluscalib-0.3.21/spluscalib/steps/resources/SExsplus.param`

 * *Files identical despite different names*

### Comparing `spluscalib-0.3.2/spluscalib/steps/resources/SExsplus.sex` & `spluscalib-0.3.21/spluscalib/steps/resources/SExsplus.sex`

 * *Files identical despite different names*

### Comparing `spluscalib-0.3.2/spluscalib/steps/resources/default_config.conf` & `spluscalib-0.3.21/spluscalib/steps/resources/default_config.conf`

 * *Files identical despite different names*

### Comparing `spluscalib-0.3.2/spluscalib/steps/resources/dophot_paramdefault` & `spluscalib-0.3.21/spluscalib/steps/resources/dophot_paramdefault`

 * *Files identical despite different names*

### Comparing `spluscalib-0.3.2/spluscalib/steps/resources/swarpsplus.swarp` & `spluscalib-0.3.21/spluscalib/steps/resources/swarpsplus.swarp`

 * *Files identical despite different names*

### Comparing `spluscalib-0.3.2/spluscalib/utils.py` & `spluscalib-0.3.21/spluscalib/utils.py`

 * *Files identical despite different names*

### Comparing `spluscalib-0.3.2/spluscalib.egg-info/SOURCES.txt` & `spluscalib-0.3.21/spluscalib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spluscalib-0.3.2/stellarlibrary/dust_laws.py` & `spluscalib-0.3.21/stellarlibrary/dust_laws.py`

 * *Files identical despite different names*

### Comparing `spluscalib-0.3.2/stellarlibrary/generate_models_photometry.py` & `spluscalib-0.3.21/stellarlibrary/generate_models_photometry.py`

 * *Files identical despite different names*

### Comparing `spluscalib-0.3.2/stellarlibrary/generate_models_photometry_iDR5.py` & `spluscalib-0.3.21/stellarlibrary/generate_models_photometry_iDR5.py`

 * *Files identical despite different names*

### Comparing `spluscalib-0.3.2/stellarlibrary/models.py` & `spluscalib-0.3.21/stellarlibrary/models.py`

 * *Files identical despite different names*

### Comparing `spluscalib-0.3.2/stellarlibrary/prior.py` & `spluscalib-0.3.21/stellarlibrary/prior.py`

 * *Files identical despite different names*

