# Comparing `tmp/arcticpy-2.2.tar.gz` & `tmp/arcticpy-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcticpy-2.2.tar", last modified: Tue Mar 21 12:50:14 2023, max compression
+gzip compressed data, was "arcticpy-2.3.tar", last modified: Fri Jul 21 17:48:24 2023, max compression
```

## Comparing `arcticpy-2.2.tar` & `arcticpy-2.3.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-21 12:50:14.247203 arcticpy-2.2/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      148 2022-09-21 12:28:55.000000 arcticpy-2.2/.clang-format
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      213 2022-12-13 13:44:27.000000 arcticpy-2.2/.gitignore
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      136 2022-10-05 11:34:58.000000 arcticpy-2.2/MANIFEST.in
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      206 2023-03-21 12:50:14.246204 arcticpy-2.2/PKG-INFO
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    29665 2022-09-27 13:16:11.000000 arcticpy-2.2/README.md
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      124 2022-09-21 12:28:55.000000 arcticpy-2.2/format.sh
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      383 2022-09-27 13:16:11.000000 arcticpy-2.2/generate_image.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      942 2022-12-13 13:44:27.000000 arcticpy-2.2/get_gsl.sh
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-21 12:50:14.174203 arcticpy-2.2/include/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      858 2023-02-27 14:41:26.000000 arcticpy-2.2/include/ccd.hpp
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3744 2023-02-27 14:41:26.000000 arcticpy-2.2/include/cti.hpp
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3097 2022-09-27 13:16:11.000000 arcticpy-2.2/include/roe.hpp
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6228 2023-02-27 14:41:26.000000 arcticpy-2.2/include/trap_managers.hpp
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3636 2023-01-13 13:05:53.000000 arcticpy-2.2/include/traps.hpp
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2871 2022-09-30 16:35:11.000000 arcticpy-2.2/include/util.hpp
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2534 2022-11-08 17:01:26.000000 arcticpy-2.2/jn_speed.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1403 2022-11-08 17:30:40.000000 arcticpy-2.2/jn_speed_2.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1285 2022-11-08 17:27:04.000000 arcticpy-2.2/jn_speed_3.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1057 2022-09-27 13:16:11.000000 arcticpy-2.2/license.txt
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2270 2023-01-13 13:05:53.000000 arcticpy-2.2/make_setup.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4920 2023-02-27 14:50:45.000000 arcticpy-2.2/makefile
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      618 2023-03-21 12:49:50.000000 arcticpy-2.2/pyproject.toml
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-21 12:50:14.129203 arcticpy-2.2/python/
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-21 12:50:14.193203 arcticpy-2.2/python/arcticpy/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13043 2023-02-27 14:41:26.000000 arcticpy-2.2/python/arcticpy/OLDread_noise.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      731 2022-10-05 13:29:36.000000 arcticpy-2.2/python/arcticpy/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2292 2023-02-27 14:44:04.000000 arcticpy-2.2/python/arcticpy/ccd.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    19355 2023-02-27 14:41:26.000000 arcticpy-2.2/python/arcticpy/cti.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-21 12:50:14.207203 arcticpy-2.2/python/arcticpy/include/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2810 2023-02-27 14:41:26.000000 arcticpy-2.2/python/arcticpy/include/interface.hpp
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10851 2022-09-27 13:16:11.000000 arcticpy-2.2/python/arcticpy/pixel_bounce.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    36323 2023-02-27 14:41:26.000000 arcticpy-2.2/python/arcticpy/read_noise.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4509 2022-11-08 14:25:28.000000 arcticpy-2.2/python/arcticpy/roe.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-21 12:50:14.210203 arcticpy-2.2/python/arcticpy/src/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    16371 2023-02-27 14:41:26.000000 arcticpy-2.2/python/arcticpy/src/interface.cpp
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2723 2022-09-27 13:16:33.000000 arcticpy-2.2/python/arcticpy/traps.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)   417796 2023-03-21 12:50:09.000000 arcticpy-2.2/python/arcticpy/wrapper.cpp
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10295 2023-02-27 14:41:26.000000 arcticpy-2.2/python/arcticpy/wrapper.pyx
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-21 12:50:14.205204 arcticpy-2.2/python/arcticpy.egg-info/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      206 2023-03-21 12:50:13.000000 arcticpy-2.2/python/arcticpy.egg-info/PKG-INFO
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1285 2023-03-21 12:50:14.000000 arcticpy-2.2/python/arcticpy.egg-info/SOURCES.txt
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        1 2023-03-21 12:50:13.000000 arcticpy-2.2/python/arcticpy.egg-info/dependency_links.txt
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        1 2022-10-05 13:18:06.000000 arcticpy-2.2/python/arcticpy.egg-info/not-zip-safe
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       47 2023-03-21 12:50:13.000000 arcticpy-2.2/python/arcticpy.egg-info/requires.txt
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        9 2023-03-21 12:50:13.000000 arcticpy-2.2/python/arcticpy.egg-info/top_level.txt
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       38 2023-03-21 12:50:14.247203 arcticpy-2.2/setup.cfg
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1883 2023-01-13 13:05:53.000000 arcticpy-2.2/setup.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-21 12:50:14.223203 arcticpy-2.2/src/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4225 2023-02-27 14:41:26.000000 arcticpy-2.2/src/ccd.cpp
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    32374 2023-02-27 14:41:26.000000 arcticpy-2.2/src/cti.cpp
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9241 2023-02-27 14:41:26.000000 arcticpy-2.2/src/main.cpp
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    43327 2022-11-08 14:25:28.000000 arcticpy-2.2/src/roe.cpp
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    92340 2023-02-27 14:41:26.000000 arcticpy-2.2/src/trap_managers.cpp
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    33182 2023-01-13 13:05:53.000000 arcticpy-2.2/src/traps.cpp
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7872 2022-09-27 13:53:34.000000 arcticpy-2.2/src/util.cpp
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-21 12:50:14.239203 arcticpy-2.2/test/
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-21 12:50:14.241203 arcticpy-2.2/test/catch2/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)   671275 2022-09-27 13:16:11.000000 arcticpy-2.2/test/catch2/catch.hpp
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-21 12:50:14.244203 arcticpy-2.2/test/files/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       14 2022-09-21 12:28:55.000000 arcticpy-2.2/test/files/.gitignore
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    36565 2022-09-21 12:28:55.000000 arcticpy-2.2/test/test_arcticpy.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4339 2023-02-27 14:41:26.000000 arcticpy-2.2/test/test_ccd.cpp
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    41135 2023-02-27 14:41:26.000000 arcticpy-2.2/test/test_cti.cpp
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1787 2022-09-27 13:16:11.000000 arcticpy-2.2/test/test_lib.cpp
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       83 2022-09-21 12:28:55.000000 arcticpy-2.2/test/test_main.cpp
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    96688 2022-09-21 12:28:55.000000 arcticpy-2.2/test/test_roe.cpp
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)   163280 2022-09-21 12:28:55.000000 arcticpy-2.2/test/test_trap_managers.cpp
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    26159 2022-09-21 12:28:55.000000 arcticpy-2.2/test/test_traps.cpp
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4578 2022-09-27 13:16:11.000000 arcticpy-2.2/test/test_util.cpp
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1884 2022-09-30 16:35:11.000000 arcticpy-2.2/tst_cil.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1472 2023-02-27 14:41:26.000000 arcticpy-2.2/tst_correct.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2333 2023-02-27 14:41:26.000000 arcticpy-2.2/tst_covar.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4819 2023-02-27 14:41:26.000000 arcticpy-2.2/tst_dark.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4977 2023-02-27 14:41:26.000000 arcticpy-2.2/tst_negative_image.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2106 2022-09-30 16:35:11.000000 arcticpy-2.2/tst_pixel_bounce.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-07-21 17:48:24.769588 arcticpy-2.3/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      148 2022-09-21 12:28:55.000000 arcticpy-2.3/.clang-format
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      213 2022-12-13 13:44:27.000000 arcticpy-2.3/.gitignore
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      136 2022-10-05 11:34:58.000000 arcticpy-2.3/MANIFEST.in
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      206 2023-07-21 17:48:24.768588 arcticpy-2.3/PKG-INFO
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    29658 2023-05-11 09:40:23.000000 arcticpy-2.3/README.md
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      124 2022-09-21 12:28:55.000000 arcticpy-2.3/format.sh
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      390 2023-06-05 20:22:34.000000 arcticpy-2.3/generate_image.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      942 2022-12-13 13:44:27.000000 arcticpy-2.3/get_gsl.sh
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-07-21 17:48:24.699598 arcticpy-2.3/include/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      858 2023-02-27 14:41:26.000000 arcticpy-2.3/include/ccd.hpp
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3744 2023-02-27 14:41:26.000000 arcticpy-2.3/include/cti.hpp
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3097 2022-09-27 13:16:11.000000 arcticpy-2.3/include/roe.hpp
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6228 2023-02-27 14:41:26.000000 arcticpy-2.3/include/trap_managers.hpp
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3636 2023-01-13 13:05:53.000000 arcticpy-2.3/include/traps.hpp
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2871 2022-09-30 16:35:11.000000 arcticpy-2.3/include/util.hpp
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2574 2023-06-05 20:22:35.000000 arcticpy-2.3/jn_speed.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1403 2022-11-08 17:30:40.000000 arcticpy-2.3/jn_speed_2.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1285 2022-11-08 17:27:04.000000 arcticpy-2.3/jn_speed_3.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1057 2022-09-27 13:16:11.000000 arcticpy-2.3/license.txt
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2454 2023-06-05 20:22:35.000000 arcticpy-2.3/make_setup.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4920 2023-05-10 17:58:13.000000 arcticpy-2.3/makefile
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      619 2023-07-21 17:48:19.000000 arcticpy-2.3/pyproject.toml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-07-21 17:48:24.653592 arcticpy-2.3/python/
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-07-21 17:48:24.720599 arcticpy-2.3/python/arcticpy/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    14125 2023-06-05 20:22:35.000000 arcticpy-2.3/python/arcticpy/OLDread_noise.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      735 2023-06-05 20:22:35.000000 arcticpy-2.3/python/arcticpy/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2297 2023-06-05 20:22:35.000000 arcticpy-2.3/python/arcticpy/ccd.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    19426 2023-06-05 20:22:35.000000 arcticpy-2.3/python/arcticpy/cti.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-07-21 17:48:24.733600 arcticpy-2.3/python/arcticpy/include/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2810 2023-02-27 14:41:26.000000 arcticpy-2.3/python/arcticpy/include/interface.hpp
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10595 2023-06-05 20:22:35.000000 arcticpy-2.3/python/arcticpy/pixel_bounce.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    39440 2023-06-05 20:22:36.000000 arcticpy-2.3/python/arcticpy/read_noise.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4501 2023-06-05 20:22:35.000000 arcticpy-2.3/python/arcticpy/roe.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-07-21 17:48:24.735605 arcticpy-2.3/python/arcticpy/src/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    16371 2023-02-27 14:41:26.000000 arcticpy-2.3/python/arcticpy/src/interface.cpp
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2831 2023-06-05 20:22:35.000000 arcticpy-2.3/python/arcticpy/traps.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   570423 2023-07-21 17:48:23.000000 arcticpy-2.3/python/arcticpy/wrapper.cpp
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10295 2023-02-27 14:41:26.000000 arcticpy-2.3/python/arcticpy/wrapper.pyx
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-07-21 17:48:24.731599 arcticpy-2.3/python/arcticpy.egg-info/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      206 2023-07-21 17:48:24.000000 arcticpy-2.3/python/arcticpy.egg-info/PKG-INFO
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1285 2023-07-21 17:48:24.000000 arcticpy-2.3/python/arcticpy.egg-info/SOURCES.txt
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        1 2023-07-21 17:48:24.000000 arcticpy-2.3/python/arcticpy.egg-info/dependency_links.txt
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        1 2022-10-05 13:18:06.000000 arcticpy-2.3/python/arcticpy.egg-info/not-zip-safe
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       47 2023-07-21 17:48:24.000000 arcticpy-2.3/python/arcticpy.egg-info/requires.txt
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        9 2023-07-21 17:48:24.000000 arcticpy-2.3/python/arcticpy.egg-info/top_level.txt
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       38 2023-07-21 17:48:24.769588 arcticpy-2.3/setup.cfg
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1973 2023-06-05 20:22:35.000000 arcticpy-2.3/setup.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-07-21 17:48:24.747602 arcticpy-2.3/src/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4225 2023-02-27 14:41:26.000000 arcticpy-2.3/src/ccd.cpp
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    32374 2023-02-27 14:41:26.000000 arcticpy-2.3/src/cti.cpp
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9241 2023-02-27 14:41:26.000000 arcticpy-2.3/src/main.cpp
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    43327 2022-11-08 14:25:28.000000 arcticpy-2.3/src/roe.cpp
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    92340 2023-02-27 14:41:26.000000 arcticpy-2.3/src/trap_managers.cpp
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    33182 2023-01-13 13:05:53.000000 arcticpy-2.3/src/traps.cpp
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7872 2022-09-27 13:53:34.000000 arcticpy-2.3/src/util.cpp
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-07-21 17:48:24.762614 arcticpy-2.3/test/
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-07-21 17:48:24.764615 arcticpy-2.3/test/catch2/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   671275 2022-09-27 13:16:11.000000 arcticpy-2.3/test/catch2/catch.hpp
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-07-21 17:48:24.767587 arcticpy-2.3/test/files/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       14 2022-09-21 12:28:55.000000 arcticpy-2.3/test/files/.gitignore
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    36565 2022-09-21 12:28:55.000000 arcticpy-2.3/test/test_arcticpy.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4339 2023-02-27 14:41:26.000000 arcticpy-2.3/test/test_ccd.cpp
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    41135 2023-02-27 14:41:26.000000 arcticpy-2.3/test/test_cti.cpp
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1787 2022-09-27 13:16:11.000000 arcticpy-2.3/test/test_lib.cpp
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       83 2022-09-21 12:28:55.000000 arcticpy-2.3/test/test_main.cpp
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    96688 2022-09-21 12:28:55.000000 arcticpy-2.3/test/test_roe.cpp
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   163280 2022-09-21 12:28:55.000000 arcticpy-2.3/test/test_trap_managers.cpp
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    26159 2022-09-21 12:28:55.000000 arcticpy-2.3/test/test_traps.cpp
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4578 2022-09-27 13:16:11.000000 arcticpy-2.3/test/test_util.cpp
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1905 2023-06-05 20:22:35.000000 arcticpy-2.3/tst_cil.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1448 2023-06-05 20:22:35.000000 arcticpy-2.3/tst_correct.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2323 2023-06-05 20:22:35.000000 arcticpy-2.3/tst_covar.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4937 2023-06-05 20:22:35.000000 arcticpy-2.3/tst_dark.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4887 2023-06-05 20:22:35.000000 arcticpy-2.3/tst_negative_image.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2160 2023-06-05 20:22:35.000000 arcticpy-2.3/tst_pixel_bounce.py
```

### Comparing `arcticpy-2.2/README.md` & `arcticpy-2.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -129,15 +129,15 @@
 git clone https://github.com/jkeger/arctic.git
 ```
 2. Install arCTIc C++ core <!-- and unit tests -->
     + Run `make core` to compile the C++ code into an `arctic` executable and `libarctic.so` dynamic library. <!-- + Add `/***current*directory***/arctic` to your `$PATH`. -->
     + You should now get output from `./arctic --demo`.
 3. arCTIc python wrapper
     + Run `sudo make wrapper` (sudo only required on MacOS) to create `arcticpy/wrapper.cypython*.so`
-    + Add `/***current*directory***/arctic/python` to your system variable `$PYTHONPATH` and `/***current*directory***/arctic` to to another system variable `$DYLD_LIBRARY_PATH`
+    + Add `/***current*directory***/arctic/python` to your system variable `$PYTHONPATH` and `/***current*directory***/arctic` to another system variable `$DYLD_LIBRARY_PATH`
     + You should now get output (in python) from `import numpy, arcticpy ; test=arcticpy.add_cti(numpy.zeros((5,5)))`
 
 
     **MacOS:** requires `sudo make wrapper`, or equivalently `cd arcticpy; python3 setup.py build_ext --inplace`.
 
 \
 Usage
@@ -150,20 +150,20 @@
 For example, to correct CTI in a Hubble Space Telescope ACS image
 (using the [autoarray](https://pypi.org/project/autoarray/) package
 to load and save the fits image with correct units and quadrant rotations, etc):
 ```python
 import arcticpy as arctic
 import autoarray as aa
 
-image_path = "image_path/image_name"
+data_path = "data_path/image_name"
 
 # Load each quadrant of the image  (see pypi.org/project/autoarray)
 image_A, image_B, image_C, image_D = [
     aa.acs.ImageACS.from_fits(
-        file_path=image_path + ".fits",
+        file_path=data_path + ".fits",
         quadrant_letter=quadrant,
         bias_subtract_via_bias_file=True,
         bias_subtract_via_prescan=True,
     ).native
     for quadrant in ["A", "B", "C", "D"]
 ]
 
@@ -192,15 +192,15 @@
            verbosity=1,
     )
     for image in [image_A, image_B, image_C, image_D]
 ]
 
 # Save the corrected image
 aa.acs.output_quadrants_to_fits(
-    file_path=image_path + "_out.fits",
+    file_path=data_path + "_out.fits",
     quadrant_a=image_out_A,
     quadrant_b=image_out_B,
     quadrant_c=image_out_C,
     quadrant_d=image_out_D,
     header_a=image_A.header,
     header_b=image_B.header,
     header_c=image_C.header,
```

### Comparing `arcticpy-2.2/get_gsl.sh` & `arcticpy-2.3/get_gsl.sh`

 * *Files identical despite different names*

### Comparing `arcticpy-2.2/include/ccd.hpp` & `arcticpy-2.3/include/ccd.hpp`

 * *Files identical despite different names*

### Comparing `arcticpy-2.2/include/cti.hpp` & `arcticpy-2.3/include/cti.hpp`

 * *Files identical despite different names*

### Comparing `arcticpy-2.2/include/roe.hpp` & `arcticpy-2.3/include/roe.hpp`

 * *Files identical despite different names*

### Comparing `arcticpy-2.2/include/trap_managers.hpp` & `arcticpy-2.3/include/trap_managers.hpp`

 * *Files identical despite different names*

### Comparing `arcticpy-2.2/include/traps.hpp` & `arcticpy-2.3/include/traps.hpp`

 * *Files identical despite different names*

### Comparing `arcticpy-2.2/include/util.hpp` & `arcticpy-2.3/include/util.hpp`

 * *Files identical despite different names*

### Comparing `arcticpy-2.2/jn_speed.py` & `arcticpy-2.3/jn_speed.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,90 +1,90 @@
 import numpy as np
 import arcticpy
 import time
-np.set_printoptions(linewidth=205,edgeitems=56,suppress=True)
 
+np.set_printoptions(linewidth=205, edgeitems=56, suppress=True)
 
-parallel_prune_n_electrons=1e-18
-parallel_prune_frequency=5
-parallel_express=5
+
+parallel_prune_n_electrons = 1e-18
+parallel_prune_frequency = 5
+parallel_express = 5
 
 #
 # Test different values of pruning (edit here)
 #
-parallel_prune_n_electrons=-1e-12
-parallel_prune_frequency=1000
-parallel_express=1
+parallel_prune_n_electrons = -1e-12
+parallel_prune_frequency = 1000
+parallel_express = 1
 
 #
 # Set up test image
 #
-image_model = np.zeros((2000,10))+200
-image_model[0:5,:]+=700
-#image_model[500:505,:]+=700
-#image_model[1000:1005,:]+=700
-#image_model[1500:1505,:]+=700
+image_model = np.zeros((2000, 10)) + 200
+image_model[0:5, :] += 700
+# image_model[500:505,:]+=700
+# image_model[1000:1005,:]+=700
+# image_model[1500:1505,:]+=700
 
 parallel_traps = [
-    arcticpy.TrapInstantCapture(density=10.0, release_timescale=(-1/np.log(0.5))),
-    #arcticpy.TrapInstantCapture(density=10.0, release_timescale=100),
-    #arcticpy.TrapSlowCapture(density=10.0, release_timescale=(-1/np.log(0.5)), capture_timescale=0.001),
-    #arcticpy.TrapSlowCapture(density=10.0, release_timescale=(4), capture_timescale=0.001),
-    #arcticpy.TrapInstantCaptureContinuum(density=10.0, release_timescale=(1.), release_timescale_sigma=0.1),
-    #arcticpy.TrapSlowCaptureContinuum(density=10.0, release_timescale=(1.), capture_timescale=1, release_timescale_sigma=0.1),
+    arcticpy.TrapInstantCapture(density=10.0, release_timescale=(-1 / np.log(0.5))),
+    # arcticpy.TrapInstantCapture(density=10.0, release_timescale=100),
+    # arcticpy.TrapSlowCapture(density=10.0, release_timescale=(-1/np.log(0.5)), capture_timescale=0.001),
+    # arcticpy.TrapSlowCapture(density=10.0, release_timescale=(4), capture_timescale=0.001),
+    # arcticpy.TrapInstantCaptureContinuum(density=10.0, release_timescale=(1.), release_timescale_sigma=0.1),
+    # arcticpy.TrapSlowCaptureContinuum(density=10.0, release_timescale=(1.), capture_timescale=1, release_timescale_sigma=0.1),
 ]
 
 parallel_ccd = arcticpy.CCD(full_well_depth=1000, well_fill_power=1.0)
 parallel_roe = arcticpy.ROE(
     empty_traps_between_columns=True,
     empty_traps_for_first_transfers=False,
     overscan_start=1990,
-    prescan_offset=10
+    prescan_offset=10,
 )
 
 
-
 #
 # Noisy image
 #
-image_pre_cti = image_model + np.random.normal(0,0.01,image_model.shape)
-#image_pre_cti = np.maximum(image_pre_cti,np.zeros(image_pre_cti.shape));
-#print(image_pre_cti[0:10,0])
+image_pre_cti = image_model + np.random.normal(0, 0.01, image_model.shape)
+# image_pre_cti = np.maximum(image_pre_cti,np.zeros(image_pre_cti.shape));
+# print(image_pre_cti[0:10,0])
 
 start = time.time_ns()
 
 image_post_cti = arcticpy.add_cti(
     image=image_pre_cti,
     parallel_traps=parallel_traps,
     parallel_ccd=parallel_ccd,
     parallel_roe=parallel_roe,
     parallel_express=parallel_express,
     parallel_prune_n_electrons=parallel_prune_n_electrons,
     parallel_prune_frequency=parallel_prune_frequency,
-    verbosity=0
+    verbosity=0,
 )
 
 print(f"Clocking Time Noisy = {((time.time_ns() - start)/1e9)} s")
-#print(image_post_cti[0:10,0])
+# print(image_post_cti[0:10,0])
 
 #
 # Noise-free image
 #
 
 image_pre_cti = image_model
-#print(image_pre_cti[0:10,0])
+# print(image_pre_cti[0:10,0])
 
 start = time.time_ns()
 
 image_post_cti = arcticpy.add_cti(
     image=image_pre_cti,
     parallel_traps=parallel_traps,
     parallel_ccd=parallel_ccd,
     parallel_roe=parallel_roe,
     parallel_express=parallel_express,
     parallel_prune_n_electrons=parallel_prune_n_electrons,
     parallel_prune_frequency=parallel_prune_frequency,
-    verbosity=0
+    verbosity=0,
 )
 
 print(f"Clocking Time No Noise = {((time.time_ns() - start)/1e9)} s")
-print(image_post_cti[0:10,0])
+print(image_post_cti[0:10, 0])
```

### Comparing `arcticpy-2.2/jn_speed_2.py` & `arcticpy-2.3/jn_speed_2.py`

 * *Files identical despite different names*

### Comparing `arcticpy-2.2/jn_speed_3.py` & `arcticpy-2.3/jn_speed_3.py`

 * *Files identical despite different names*

### Comparing `arcticpy-2.2/license.txt` & `arcticpy-2.3/license.txt`

 * *Files identical despite different names*

### Comparing `arcticpy-2.2/make_setup.py` & `arcticpy-2.3/make_setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -20,17 +20,20 @@
 
 dir_wrapper = dir_arctic + "python/arcticpy/"
 dir_wrapper_src = dir_wrapper + "src/"
 dir_wrapper_include = dir_wrapper + "include/"
 
 # Find GSL
 dir_gsl_fallback = dir_arctic + "gsl/"
-if os.path.exists("/usr/local/include/gsl"): dir_gsl_fallback = "/usr/local/" # brew install llvm libomp gsl
-if os.path.exists("/opt/local/include/gsl"): dir_gsl_fallback = "/opt/local/" # sudo port install libomp gsl
-if os.path.exists("/cosma/local/gsl/2.5/lib"): dir_gsl_fallback = "/cosma/local/gsl/2.5/lib/" # use on cosma
+if os.path.exists("/usr/local/include/gsl"):
+    dir_gsl_fallback = "/usr/local/"  # brew install llvm libomp gsl
+if os.path.exists("/opt/local/include/gsl"):
+    dir_gsl_fallback = "/opt/local/"  # sudo port install libomp gsl
+if os.path.exists("/cosma/local/gsl/2.5/lib"):
+    dir_gsl_fallback = "/cosma/local/gsl/2.5/lib/"  # use on cosma
 dir_gsl = os.environ.get("DIR_GSL", dir_gsl_fallback)
 dir_include_gsl = dir_gsl + "include/"
 dir_lib_gsl = dir_gsl + "lib/"
 
 # Clean
 for root, dirs, files in os.walk(dir_wrapper, topdown=False):
     for name in files:
@@ -46,20 +49,28 @@
 if "CC" not in os.environ:
     os.environ["CC"] = "g++"
 setup(
     ext_modules=cythonize(
         [
             Extension(
                 "wrapper",
-                sources=[dir_wrapper + "wrapper.pyx", dir_wrapper_src + "interface.cpp"],
+                sources=[
+                    dir_wrapper + "wrapper.pyx",
+                    dir_wrapper_src + "interface.cpp",
+                ],
                 language="c++",
                 libraries=["arctic"],
                 library_dirs=[dir_lib, dir_lib_gsl],
                 runtime_library_dirs=[dir_lib, dir_lib_gsl],
-                include_dirs=[dir_include, np.get_include(), dir_wrapper_include, dir_include_gsl],
+                include_dirs=[
+                    dir_include,
+                    np.get_include(),
+                    dir_wrapper_include,
+                    dir_include_gsl,
+                ],
                 extra_compile_args=["-std=c++17", "-O3"],
-                define_macros=[('NPY_NO_DEPRECATED_API', 0)],
+                define_macros=[("NPY_NO_DEPRECATED_API", 0)],
             )
         ],
         compiler_directives={"language_level": "3"},
     )
 )
```

### Comparing `arcticpy-2.2/makefile` & `arcticpy-2.3/makefile`

 * *Files 0% similar despite different names*

```diff
@@ -95,17 +95,17 @@
 INCLUDE := -I $(DIR_INC) -I $(DIR_GSL)/include
 LIBS := -L $(DIR_GSL)/lib -Wl,-rpath,$(DIR_GSL)/lib -lgsl -lgslcblas -lm
 LIBARCTIC := -L $(DIR_ROOT) -Wl,-rpath,$(DIR_ROOT) -l$(TARGET)
 
 # Add multithreading to reduce runtime (requires OpenMP to have been installed)
 CXXFLAGS += -Xpreprocessor -fopenmp
 # Use this on a mac
-LIBS += -L $(DIR_OMP)/lib -lomp
+#LIBS += -L $(DIR_OMP)/lib -lomp
 # Use the following on cosma (can also use with macports)
-#LIBS += -L $(DIR_OMP)/lib -lgomp
+LIBS += -L $(DIR_OMP)/lib -lgomp
 
 
 # ========
 # Rules
 # ========
 # Default to main program and library
 .DEFAULT_GOAL := default
```

### Comparing `arcticpy-2.2/pyproject.toml` & `arcticpy-2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = [
     "setuptools_scm==7.0.5",
     "setuptools >=62",
     "numpy ~=1.21",
-    "cython ~=0.29",
+    "cython ~=3.0.0",
     "pytest-runner",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "arcticpy"
-version= "2.2"
+version= "2.3"
 description = "This is the python module for the arCTIc code"
 authors = [
     { name = "Richard Massey", email = "r.j.massey@durham.ac.uk" }
 ]
 dependencies = [
     "autoconf",
     "numpy ~=1.21",
```

### Comparing `arcticpy-2.2/python/arcticpy/OLDread_noise.py` & `arcticpy-2.3/python/arcticpy/OLDread_noise.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 moves read noise - which was not trailed in the first place. The net effect is to
 amplify read noise, and hide the difference in the (anti)correlation between
 adjacent pixels. 
 
 This class provides a set of routines to predict this effect, and counteract it.
 """
 
+
 class ReadNoise:
     def __init__(
-            self, 
-            sigma_readnoise=0.0, 
-            adjacency=0.3, 
-            noise_model_scaling=1.0, # originally 0.75 
-            amplitude_scale=0.2,     # originally 0.33
-            n_iter=200,
-            serial=True
-            
+        self,
+        sigma_readnoise=0.0,
+        adjacency=0.3,
+        noise_model_scaling=1.0,  # originally 0.75
+        amplitude_scale=0.2,  # originally 0.33
+        n_iter=200,
+        serial=True,
     ):
         self.sigmaRN = sigma_readnoise
         self.adjacency = adjacency
         self.ampScale = amplitude_scale
         self.outScale = noise_model_scaling
         self.n_iter = n_iter
         self.smoothCol = serial
@@ -33,284 +33,354 @@
         RMS value of read noise, in units of electrons
         """
         return self._sigma
 
     @sigma.setter
     def sigma(self, value):
         if value < 0:
-            value = 0.
+            value = 0.0
         self._sigma = value
+
     ###############
     ###############
     def determine_noise_model(self, imageIn, imageOut):
         readNoiseAmp = self.sigmaRN
-        
+
         dval0 = imageIn - imageOut
         dval0u = dval0.copy()
-        
-        dval0u[dval0u>1] = 1
-        dval0u[dval0u<-1] = -1
-        
-        dval9 = imageIn*0
-        dcount = imageIn*0
-        
-        dval9[:-1,:-1]+=(imageIn[1: ,1: ]-imageOut[1: ,1: ]); dcount[:-1,:-1]+=1
-        dval9[:-1,:  ]+=(imageIn[1: ,:  ]-imageOut[1: ,:  ]); dcount[:-1,:  ]+=1
-        dval9[:-1,1: ]+=(imageIn[1: ,:-1]-imageOut[1: ,:-1]); dcount[:-1,1: ]+=1
-        dval9[:  ,:-1]+=(imageIn[:  ,1: ]-imageOut[:  ,1: ]); dcount[:  ,:-1]+=1
-        dval9[:  ,:  ]+=(imageIn[:  ,:  ]-imageOut[:  ,:  ]); dcount[:  ,:  ]+=1
-        dval9[:  ,1: ]+=(imageIn[:  ,:-1]-imageOut[:  ,:-1]); dcount[:  ,1: ]+=1
-        dval9[1: ,:-1]+=(imageIn[:-1,1: ]-imageOut[:-1,1: ]); dcount[1: ,:-1]+=1
-        dval9[1: ,:  ]+=(imageIn[:-1,:  ]-imageOut[:-1,:  ]); dcount[1: ,:  ]+=1
-        dval9[1: ,1: ]+=(imageIn[:-1,:-1]-imageOut[:-1,:-1]); dcount[1: ,1: ]+=1
-        
-        dval9/=dcount
-        
+
+        dval0u[dval0u > 1] = 1
+        dval0u[dval0u < -1] = -1
+
+        dval9 = imageIn * 0
+        dcount = imageIn * 0
+
+        dval9[:-1, :-1] += imageIn[1:, 1:] - imageOut[1:, 1:]
+        dcount[:-1, :-1] += 1
+        dval9[:-1, :] += imageIn[1:, :] - imageOut[1:, :]
+        dcount[:-1, :] += 1
+        dval9[:-1, 1:] += imageIn[1:, :-1] - imageOut[1:, :-1]
+        dcount[:-1, 1:] += 1
+        dval9[:, :-1] += imageIn[:, 1:] - imageOut[:, 1:]
+        dcount[:, :-1] += 1
+        dval9[:, :] += imageIn[:, :] - imageOut[:, :]
+        dcount[:, :] += 1
+        dval9[:, 1:] += imageIn[:, :-1] - imageOut[:, :-1]
+        dcount[:, 1:] += 1
+        dval9[1:, :-1] += imageIn[:-1, 1:] - imageOut[:-1, 1:]
+        dcount[1:, :-1] += 1
+        dval9[1:, :] += imageIn[:-1, :] - imageOut[:-1, :]
+        dcount[1:, :] += 1
+        dval9[1:, 1:] += imageIn[:-1, :-1] - imageOut[:-1, :-1]
+        dcount[1:, 1:] += 1
+
+        dval9 /= dcount
+
         readNoiseAmpFraction = self.ampScale
         dval9u = dval9.copy()
-        if type(readNoiseAmp)==np.ndarray:
+        if type(readNoiseAmp) == np.ndarray:
             dval9u = dval9u.flatten()
             readNoiseAmp = readNoiseAmp.flatten()
-            dval9u[dval9u > readNoiseAmp*readNoiseAmpFraction] = (readNoiseAmp*readNoiseAmpFraction)[dval9u > readNoiseAmp*readNoiseAmpFraction]
-            dval9u[dval9u < readNoiseAmp*-readNoiseAmpFraction] = (readNoiseAmp*-readNoiseAmpFraction)[dval9u < readNoiseAmp*-readNoiseAmpFraction]
+            dval9u[dval9u > readNoiseAmp * readNoiseAmpFraction] = (
+                readNoiseAmp * readNoiseAmpFraction
+            )[dval9u > readNoiseAmp * readNoiseAmpFraction]
+            dval9u[dval9u < readNoiseAmp * -readNoiseAmpFraction] = (
+                readNoiseAmp * -readNoiseAmpFraction
+            )[dval9u < readNoiseAmp * -readNoiseAmpFraction]
             dval9u = dval9u.reshape(imageIn.shape)
-            readNoiseAmp = readNoiseAmp.reshape(imageIn.shape)        
+            readNoiseAmp = readNoiseAmp.reshape(imageIn.shape)
         else:
-            dval9u[dval9u > readNoiseAmp*readNoiseAmpFraction] = readNoiseAmp*readNoiseAmpFraction
-            dval9u[dval9u < readNoiseAmp*-readNoiseAmpFraction] = readNoiseAmp*-readNoiseAmpFraction
-            
-        dmod1 = imageIn*0
-        dmod1[1:,:] = imageOut[:-1,:] - imageOut[1:,:]
-        dmod2 = imageIn*0
-        dmod2[:-1,:] = imageOut[1:,:] - imageOut[:-1,:]
-        
+            dval9u[dval9u > readNoiseAmp * readNoiseAmpFraction] = (
+                readNoiseAmp * readNoiseAmpFraction
+            )
+            dval9u[dval9u < readNoiseAmp * -readNoiseAmpFraction] = (
+                readNoiseAmp * -readNoiseAmpFraction
+            )
+
+        dmod1 = imageIn * 0
+        dmod1[1:, :] = imageOut[:-1, :] - imageOut[1:, :]
+        dmod2 = imageIn * 0
+        dmod2[:-1, :] = imageOut[1:, :] - imageOut[:-1, :]
+
         if self.smoothCol:
-            cmod1 = imageIn*0
-            cmod1[:,1:] = imageOut[:,:-1] - imageOut[:,1:]
-            cmod2 = imageIn*0
-            cmod2[:,:-1] = imageOut[:,1:] - imageOut[:,:-1]
-            
+            cmod1 = imageIn * 0
+            cmod1[:, 1:] = imageOut[:, :-1] - imageOut[:, 1:]
+            cmod2 = imageIn * 0
+            cmod2[:, :-1] = imageOut[:, 1:] - imageOut[:, :-1]
+
         dmod1u = dmod1.copy()
-        if type(readNoiseAmp)==np.ndarray:
+        if type(readNoiseAmp) == np.ndarray:
             dmod1u = dmod1u.flatten()
             readNoiseAmp = readNoiseAmp.flatten()
-            dmod1u[dmod1u>readNoiseAmp*readNoiseAmpFraction] = (readNoiseAmp*readNoiseAmpFraction)[dmod1u>readNoiseAmp*readNoiseAmpFraction]
-            dmod1u[dmod1u<readNoiseAmp*-readNoiseAmpFraction] = (readNoiseAmp*-readNoiseAmpFraction)[dmod1u<readNoiseAmp*-readNoiseAmpFraction]
-            dmod1u = dmod1u.reshape(imageIn.shape)       
+            dmod1u[dmod1u > readNoiseAmp * readNoiseAmpFraction] = (
+                readNoiseAmp * readNoiseAmpFraction
+            )[dmod1u > readNoiseAmp * readNoiseAmpFraction]
+            dmod1u[dmod1u < readNoiseAmp * -readNoiseAmpFraction] = (
+                readNoiseAmp * -readNoiseAmpFraction
+            )[dmod1u < readNoiseAmp * -readNoiseAmpFraction]
+            dmod1u = dmod1u.reshape(imageIn.shape)
         else:
-            dmod1u[dmod1u>readNoiseAmp*readNoiseAmpFraction] = readNoiseAmp*readNoiseAmpFraction
-            dmod1u[dmod1u<readNoiseAmp*-readNoiseAmpFraction] = readNoiseAmp*-readNoiseAmpFraction
-            
+            dmod1u[dmod1u > readNoiseAmp * readNoiseAmpFraction] = (
+                readNoiseAmp * readNoiseAmpFraction
+            )
+            dmod1u[dmod1u < readNoiseAmp * -readNoiseAmpFraction] = (
+                readNoiseAmp * -readNoiseAmpFraction
+            )
+
         dmod2u = dmod2.copy()
-        if type(readNoiseAmp)==np.ndarray:
+        if type(readNoiseAmp) == np.ndarray:
             dmod2u = dmod2u.flatten()
             readNoiseAmp = readNoiseAmp.flatten()
-            dmod2u[dmod2u>readNoiseAmp*readNoiseAmpFraction] = (readNoiseAmp*readNoiseAmpFraction)[dmod2u>readNoiseAmp*readNoiseAmpFraction]
-            dmod2u[dmod2u<readNoiseAmp*-readNoiseAmpFraction] = (readNoiseAmp*-readNoiseAmpFraction)[dmod2u<readNoiseAmp*-readNoiseAmpFraction]
+            dmod2u[dmod2u > readNoiseAmp * readNoiseAmpFraction] = (
+                readNoiseAmp * readNoiseAmpFraction
+            )[dmod2u > readNoiseAmp * readNoiseAmpFraction]
+            dmod2u[dmod2u < readNoiseAmp * -readNoiseAmpFraction] = (
+                readNoiseAmp * -readNoiseAmpFraction
+            )[dmod2u < readNoiseAmp * -readNoiseAmpFraction]
             dmod2u = dmod2u.reshape(imageIn.shape)
-            readNoiseAmp = readNoiseAmp.reshape(imageIn.shape) 
+            readNoiseAmp = readNoiseAmp.reshape(imageIn.shape)
         else:
-            dmod2u[dmod2u>readNoiseAmp*readNoiseAmpFraction] = readNoiseAmp*readNoiseAmpFraction
-            dmod2u[dmod2u<readNoiseAmp*-readNoiseAmpFraction] = readNoiseAmp*-readNoiseAmpFraction
-            
+            dmod2u[dmod2u > readNoiseAmp * readNoiseAmpFraction] = (
+                readNoiseAmp * readNoiseAmpFraction
+            )
+            dmod2u[dmod2u < readNoiseAmp * -readNoiseAmpFraction] = (
+                readNoiseAmp * -readNoiseAmpFraction
+            )
+
         if self.smoothCol:
             cmod1u = cmod1.copy()
-            if type(readNoiseAmp)==np.ndarray:
+            if type(readNoiseAmp) == np.ndarray:
                 cmod1u = cmod1u.flatten()
                 readNoiseAmp = readNoiseAmp.flatten()
-                cmod1u[cmod1u>readNoiseAmp*readNoiseAmpFraction] = (readNoiseAmp*readNoiseAmpFraction)[cmod1u>readNoiseAmp*readNoiseAmpFraction]
-                cmod1u[cmod1u<readNoiseAmp*-readNoiseAmpFraction] = (readNoiseAmp*-readNoiseAmpFraction)[cmod1u<readNoiseAmp*-readNoiseAmpFraction]
+                cmod1u[cmod1u > readNoiseAmp * readNoiseAmpFraction] = (
+                    readNoiseAmp * readNoiseAmpFraction
+                )[cmod1u > readNoiseAmp * readNoiseAmpFraction]
+                cmod1u[cmod1u < readNoiseAmp * -readNoiseAmpFraction] = (
+                    readNoiseAmp * -readNoiseAmpFraction
+                )[cmod1u < readNoiseAmp * -readNoiseAmpFraction]
                 cmod1u = cmod1u.reshape(imageIn.shape)
                 readNoiseAmp = readNoiseAmp.reshape(imageIn.shape)
             else:
-                cmod1u[cmod1u>readNoiseAmp*readNoiseAmpFraction] = readNoiseAmp*readNoiseAmpFraction
-                cmod1u[cmod1u<readNoiseAmp*-readNoiseAmpFraction] = readNoiseAmp*-readNoiseAmpFraction
-                
+                cmod1u[cmod1u > readNoiseAmp * readNoiseAmpFraction] = (
+                    readNoiseAmp * readNoiseAmpFraction
+                )
+                cmod1u[cmod1u < readNoiseAmp * -readNoiseAmpFraction] = (
+                    readNoiseAmp * -readNoiseAmpFraction
+                )
+
             cmod2u = cmod2.copy()
-            if type(readNoiseAmp)==np.ndarray:
+            if type(readNoiseAmp) == np.ndarray:
                 cmod2u = cmod2u.flatten()
                 readNoiseAmp = readNoiseAmp.flatten()
-                cmod2u[cmod2u>readNoiseAmp*readNoiseAmpFraction] = (readNoiseAmp*readNoiseAmpFraction)[cmod2u>readNoiseAmp*readNoiseAmpFraction]
-                cmod2u[cmod2u<readNoiseAmp*-readNoiseAmpFraction] = (readNoiseAmp*-readNoiseAmpFraction)[cmod2u<readNoiseAmp*-readNoiseAmpFraction]
+                cmod2u[cmod2u > readNoiseAmp * readNoiseAmpFraction] = (
+                    readNoiseAmp * readNoiseAmpFraction
+                )[cmod2u > readNoiseAmp * readNoiseAmpFraction]
+                cmod2u[cmod2u < readNoiseAmp * -readNoiseAmpFraction] = (
+                    readNoiseAmp * -readNoiseAmpFraction
+                )[cmod2u < readNoiseAmp * -readNoiseAmpFraction]
                 cmod2u = cmod2u.reshape(imageIn.shape)
-                readNoiseAmp = readNoiseAmp.reshape(imageIn.shape)          
+                readNoiseAmp = readNoiseAmp.reshape(imageIn.shape)
             else:
-                cmod2u[cmod2u>readNoiseAmp*readNoiseAmpFraction] = readNoiseAmp*readNoiseAmpFraction
-                cmod2u[cmod2u<readNoiseAmp*-readNoiseAmpFraction] = readNoiseAmp*-readNoiseAmpFraction
-                
+                cmod2u[cmod2u > readNoiseAmp * readNoiseAmpFraction] = (
+                    readNoiseAmp * readNoiseAmpFraction
+                )
+                cmod2u[cmod2u < readNoiseAmp * -readNoiseAmpFraction] = (
+                    readNoiseAmp * -readNoiseAmpFraction
+                )
+
         readNoiseAmp2 = readNoiseAmp**2
-        w0 =     dval0 * dval0 / (dval0 * dval0 + 4.0 * readNoiseAmp2)
-        w9 =     dval9 * dval9 / (dval9 * dval9 + 18.0 * readNoiseAmp2)
+        w0 = dval0 * dval0 / (dval0 * dval0 + 4.0 * readNoiseAmp2)
+        w9 = dval9 * dval9 / (dval9 * dval9 + 18.0 * readNoiseAmp2)
         w1 = 4 * readNoiseAmp2 / (dmod1 * dmod1 + 4.0 * readNoiseAmp2)
         w2 = 4 * readNoiseAmp2 / (dmod2 * dmod2 + 4.0 * readNoiseAmp2)
         if self.smoothCol:
             wc1 = 4 * readNoiseAmp2 / (cmod1 * cmod1 + 4.0 * readNoiseAmp2)
-            wc2 = 4 * readNoiseAmp2 / (cmod2 * cmod2 + 4.0 * readNoiseAmp2)    
-            
+            wc2 = 4 * readNoiseAmp2 / (cmod2 * cmod2 + 4.0 * readNoiseAmp2)
+
         if self.smoothCol:
-            return  (dval0u * w0 / 6) + (dval9u * w9 / 6) +(dmod1u * w1 / 6) + (dmod2u * w2 / 6) +(cmod1u * wc1 / 6) + (cmod2u * wc2 / 6)
+            return (
+                (dval0u * w0 / 6)
+                + (dval9u * w9 / 6)
+                + (dmod1u * w1 / 6)
+                + (dmod2u * w2 / 6)
+                + (cmod1u * wc1 / 6)
+                + (cmod2u * wc2 / 6)
+            )
         else:
-            return  (dval0u * w0 * 0.25) + (dval9u * w9 * 0.25) +(dmod1u * w1 * 0.25) + (dmod2u * w2 * 0.25)
+            return (
+                (dval0u * w0 * 0.25)
+                + (dval9u * w9 * 0.25)
+                + (dmod1u * w1 * 0.25)
+                + (dmod2u * w2 * 0.25)
+            )
+
     ###############
     ###############
     def estimate_read_noise_model_from_image(self, image):
         ampReadNoise = self.sigmaRN
 
         imageIn = image
-        imageAdj = np.zeros_like(imageIn) #adjustment image (for read noise modeling)
-        imageOut = imageIn.copy()         #output ("smoothed") image
-        
+        imageAdj = np.zeros_like(imageIn)  # adjustment image (for read noise modeling)
+        imageOut = imageIn.copy()  # output ("smoothed") image
+
         nrows = imageIn.shape[0]
         ncols = imageIn.shape[1]
-        
-        rmsGlobal = 0.
-        nrmsGlobal = 0.
-        
+
+        rmsGlobal = 0.0
+        nrmsGlobal = 0.0
+
         smoother = 1
         for s in range(self.n_iter):
-            oldchk = ampReadNoise-rmsGlobal
-            imageAdj= self.determine_noise_model(imageIn,imageOut)
+            oldchk = ampReadNoise - rmsGlobal
+            imageAdj = self.determine_noise_model(imageIn, imageOut)
 
-            if (ampReadNoise-rmsGlobal) > 0:
+            if (ampReadNoise - rmsGlobal) > 0:
                 imageOut += imageAdj * self.outScale / smoother
                 noiseImage = imageIn - imageOut
             else:
                 imageOut -= imageAdj * self.outScale / smoother
                 noiseImage = imageIn - imageOut
-        
-            cond = abs(imageIn > 0.1)|abs(imageOut > 0.1)
-            rmsGlobal = np.sum(noiseImage[cond]**2)
+
+            cond = abs(imageIn > 0.1) | abs(imageOut > 0.1)
+            rmsGlobal = np.sum(noiseImage[cond] ** 2)
             nrmsGlobal = noiseImage[cond].size
 
-            rmsGlobal = np.sqrt(rmsGlobal/nrmsGlobal)
-            print(s,rmsGlobal, (ampReadNoise-rmsGlobal))
-            
-            chk = ampReadNoise-rmsGlobal
-            if chk*oldchk < 0:
-                smoother+=1
-                
-            if type(ampReadNoise)==np.ndarray:
+            rmsGlobal = np.sqrt(rmsGlobal / nrmsGlobal)
+            print(s, rmsGlobal, (ampReadNoise - rmsGlobal))
+
+            chk = ampReadNoise - rmsGlobal
+            if chk * oldchk < 0:
+                smoother += 1
+
+            if type(ampReadNoise) == np.ndarray:
                 if np.max(ampReadNoise - rmsGlobal) < 0.0001:
                     break
             else:
                 if abs(ampReadNoise - rmsGlobal) < 0.0001:
                     break
-        return imageOut,noiseImage
-        #raise NotImplementedError
-        #return image
+        return imageOut, noiseImage
+        # raise NotImplementedError
+        # return image
+
     ###############
     ###############
     def estimate_residual_covariance(
-        self, 
+        self,
         background_level,
         # Parallel
-        parallel_ccd=None, #can we do this with **kwargs ? I'm not sure in python
+        parallel_ccd=None,  # can we do this with **kwargs ? I'm not sure in python
         parallel_roe=None,
         parallel_traps=None,
         parallel_express=0,
         parallel_window_offset=0,
         parallel_window_start=0,
         parallel_window_stop=-1,
         parallel_time_start=0,
         parallel_time_stop=-1,
-        parallel_prune_n_electrons=1e-10, 
-        parallel_prune_frequency=20
+        parallel_prune_n_electrons=1e-10,
+        parallel_prune_frequency=20,
     ):
         # Serial
-        if ( self.smoothCol ): 
-            #should be more agnostic about direction or rows/cols (for variable names...)  
-            serial_ccd=None,
-            serial_roe=None,
-            serial_traps=None,
-            serial_express=0,
-            serial_window_offset=0,
-            serial_window_start=0,
-            serial_window_stop=-1,
-            serial_time_start=0,
-            serial_time_stop=-1,
-            serial_prune_n_electrons=1e-10, 
-            serial_prune_frequency=20,
+        if self.smoothCol:
+            # should be more agnostic about direction or rows/cols (for variable names...)
+            serial_ccd = (None,)
+            serial_roe = (None,)
+            serial_traps = (None,)
+            serial_express = (0,)
+            serial_window_offset = (0,)
+            serial_window_start = (0,)
+            serial_window_stop = (-1,)
+            serial_time_start = (0,)
+            serial_time_stop = (-1,)
+            serial_prune_n_electrons = (1e-10,)
+            serial_prune_frequency = (20,)
             # Pixel bounce
-            pixel_bounce=None,
+            pixel_bounce = (None,)
             # Output
-            verbosity=1
-    
-   
+            verbosity = 1
+
         raise NotImplementedError
 
     ###############
-    ############### 
+    ###############
     def optimise_parameters(
         self,
-        image,    
+        image,
         background_level,
-        #figure_of_merit=figure_of_merit(), # should probably pass a function here
-        **kwargs 
+        # figure_of_merit=figure_of_merit(), # should probably pass a function here
+        **kwargs
         ## Parallel
-        #parallel_ccd=None, #again, should do this with **kwargs 
-        #parallel_roe=None,
-        #parallel_traps=None,
-        #parallel_express=0,
-        #parallel_window_offset=0,
-        #parallel_window_start=0,
-        #parallel_window_stop=-1,
-        #parallel_time_start=0,
-        #parallel_time_stop=-1,
-        #parallel_prune_n_electrons=1e-10, 
-        #parallel_prune_frequency=20,
+        # parallel_ccd=None, #again, should do this with **kwargs
+        # parallel_roe=None,
+        # parallel_traps=None,
+        # parallel_express=0,
+        # parallel_window_offset=0,
+        # parallel_window_start=0,
+        # parallel_window_stop=-1,
+        # parallel_time_start=0,
+        # parallel_time_stop=-1,
+        # parallel_prune_n_electrons=1e-10,
+        # parallel_prune_frequency=20,
         ## Serial
-        #serial_ccd=None,
-        #serial_roe=None,
-        #serial_traps=None,
-        #serial_express=0,
-        #serial_window_offset=0,
-        #serial_window_start=0,
-        #serial_window_stop=-1,
-        #serial_time_start=0,
-        #serial_time_stop=-1,
-        #serial_prune_n_electrons=1e-10, 
-        #serial_prune_frequency=20,
+        # serial_ccd=None,
+        # serial_roe=None,
+        # serial_traps=None,
+        # serial_express=0,
+        # serial_window_offset=0,
+        # serial_window_start=0,
+        # serial_window_stop=-1,
+        # serial_time_start=0,
+        # serial_time_stop=-1,
+        # serial_prune_n_electrons=1e-10,
+        # serial_prune_frequency=20,
         ## Pixel bounce
-        #pixel_bounce=None,
+        # pixel_bounce=None,
         ## Output
-        #verbosity=1,
+        # verbosity=1,
     ):
-        #things to compare over iterations
-        outputFrame,noiseFrame = self.estimate_read_noise_model_from_image(image)
+        # things to compare over iterations
+        outputFrame, noiseFrame = self.estimate_read_noise_model_from_image(image)
         covar = self.covariance_matrix_from_image(image)
         raise NotImplementedError
 
     ###############
     ###############
-    def figure_of_merit(self,covariance_matrix):
-        xlen = covariance_matrix.shape[1]//2
-        ylen = covariance_matrix.shape[0]//2
-        fullsum = np.sum(covariance_matrix)         #sum over all cells
-        rowsum = np.sum(covariance_matrix[ylen,:])  #sum over central row (for serial CTI)
-        colsum = np.sum(covariance_matrix[:,xlen])  #sum over central column (for parallel CTI)
-        #raise NotImplementedError
-        return fullsum,rowsum,colsum
+    def figure_of_merit(self, covariance_matrix):
+        xlen = covariance_matrix.shape[1] // 2
+        ylen = covariance_matrix.shape[0] // 2
+        fullsum = np.sum(covariance_matrix)  # sum over all cells
+        rowsum = np.sum(
+            covariance_matrix[ylen, :]
+        )  # sum over central row (for serial CTI)
+        colsum = np.sum(
+            covariance_matrix[:, xlen]
+        )  # sum over central column (for parallel CTI)
+        # raise NotImplementedError
+        return fullsum, rowsum, colsum
 
     ###############
     ###############
     def covariance_matrix_from_image(self, image, n_pixels=5):
-        #raise NotImplementedError
-        covariance_matrix = np.zeros(n_pixels,n_pixels)
-        #calcluate mean stats on image
+        # raise NotImplementedError
+        covariance_matrix = np.zeros(n_pixels, n_pixels)
+        # calcluate mean stats on image
         x = image.flatten()
         xbar = np.mean(x)
 
-        #roll image to get cross correlation
-        matRange= n_pixels//2
-        for i in range(-matRange,matRange+1,1):
-            for j in range(-matRange,matRange+1,1):
-                y = np.roll(img,(-j,-i),axis=(0,1)).flatten()
+        # roll image to get cross correlation
+        matRange = n_pixels // 2
+        for i in range(-matRange, matRange + 1, 1):
+            for j in range(-matRange, matRange + 1, 1):
+                y = np.roll(img, (-j, -i), axis=(0, 1)).flatten()
                 ybar = np.mean(y)
 
-                #calculate covariance
-                covar = np.sum((x-xbar)*(y-ybar))/(pl.std(x-xbar)*pl.std(y-ybar))/(x.size)
+                # calculate covariance
+                covar = (
+                    np.sum((x - xbar) * (y - ybar))
+                    / (pl.std(x - xbar) * pl.std(y - ybar))
+                    / (x.size)
+                )
 
-                #populate matrix cells
-                covariance_matrix[i+2,j+2] = covar
-        
-        return covariance_matrix
+                # populate matrix cells
+                covariance_matrix[i + 2, j + 2] = covar
 
+        return covariance_matrix
```

### Comparing `arcticpy-2.2/python/arcticpy/__init__.py` & `arcticpy-2.3/python/arcticpy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 from arcticpy.traps import (
     TrapInstantCapture,
     TrapSlowCapture,
     TrapInstantCaptureContinuum,
     TrapSlowCaptureContinuum,
 )
 from arcticpy.read_noise import ReadNoise
+
 try:
     from arcticpy.wrapper import (
         cy_print_array as print_array,
         cy_print_array_2D as print_array_2D,
     )
 except ModuleNotFoundError:
     from wrapper import (
         cy_print_array as print_array,
         cy_print_array_2D as print_array_2D,
-    )
+    )
```

### Comparing `arcticpy-2.2/python/arcticpy/ccd.py` & `arcticpy-2.3/python/arcticpy/ccd.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import numpy as np
 
 from autoconf.dictable import Dictable
 
-class CCDPhase(Dictable):
 
-    def __init__(self, 
-        full_well_depth=1e4, 
-        well_notch_depth=0.0, 
-        well_fill_power=1.0, 
-        first_electron_fill=0.0
+class CCDPhase(Dictable):
+    def __init__(
+        self,
+        full_well_depth=1e4,
+        well_notch_depth=0.0,
+        well_fill_power=1.0,
+        first_electron_fill=0.0,
     ):
-
         self.full_well_depth = full_well_depth
         self.well_notch_depth = well_notch_depth
         self.well_fill_power = well_fill_power
         self.first_electron_fill = first_electron_fill
 
 
 class CCD(object):
```

### Comparing `arcticpy-2.2/python/arcticpy/cti.py` & `arcticpy-2.3/python/arcticpy/cti.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 from arcticpy.roe import ROE
 from arcticpy.traps import (
     TrapInstantCapture,
     TrapSlowCapture,
     TrapInstantCaptureContinuum,
     TrapSlowCaptureContinuum,
 )
-#from arcticpy.src.pixel_bounce import add_pixel_bounce
+
+# from arcticpy.src.pixel_bounce import add_pixel_bounce
 from arcticpy.pixel_bounce import PixelBounce, add_pixel_bounce
 
 
 def _extract_trap_parameters(traps):
     """Extract trap parameters for add/remove_cti() to pass to the wrapper.
 
     Returns the converted arguments in the formats and types required by the
@@ -122,27 +123,27 @@
     parallel_traps=None,
     parallel_express=0,
     parallel_window_offset=0,
     parallel_window_start=0,
     parallel_window_stop=-1,
     parallel_time_start=0,
     parallel_time_stop=-1,
-    parallel_prune_n_electrons=1e-10, 
+    parallel_prune_n_electrons=1e-10,
     parallel_prune_frequency=20,
     # Serial
     serial_ccd=None,
     serial_roe=None,
     serial_traps=None,
     serial_express=0,
     serial_window_offset=0,
     serial_window_start=0,
     serial_window_stop=-1,
     serial_time_start=0,
     serial_time_stop=-1,
-    serial_prune_n_electrons=1e-10, 
+    serial_prune_n_electrons=1e-10,
     serial_prune_frequency=20,
     # Combined
     allow_negative_pixels=1,
     # Pixel bounce
     pixel_bounce=None,
     # Output
     verbosity=1,
@@ -229,15 +230,14 @@
             serial_trap_fourth_params,
             serial_n_traps_ic,
             serial_n_traps_sc,
             serial_n_traps_ic_co,
             serial_n_traps_sc_co,
         ) = _set_dummy_parameters()
     serial_prune_n_es = np.array([serial_prune_n_electrons], dtype=np.double)
-        
 
     # ========
     # Add CTI
     # ========
     # Pass the extracted inputs to C++ via the cython wrapper
     image_trailed = w.cy_add_cti(
         image,
@@ -309,50 +309,56 @@
         # Misc
         serial_express,
         serial_window_offset,
         serial_window_start,
         serial_window_stop,
         serial_time_start,
         serial_time_stop,
-        serial_prune_n_es, 
+        serial_prune_n_es,
         serial_prune_frequency,
         # ========
         # Combined
         # ========
         allow_negative_pixels,
         # ========
         # Output
         # ========
         verbosity,
-        iteration
+        iteration,
     )
-    
 
     # ================
     # Add pixel bounce
     # ================
     if pixel_bounce is not None:
         image_trailed = pixel_bounce.add_pixel_bounce(
             image,
             parallel_window_start=parallel_window_start,
             parallel_window_stop=parallel_window_stop,
             serial_window_start=serial_window_start,
             serial_window_stop=serial_window_stop,
-            verbosity=verbosity
+            verbosity=verbosity,
         )
-    
-    
+
     # ===================
     # Update image header
     # ===================
     if header is not None:
-        #TBD       
-        #print(w.cy_version_arctic())
-        header.set("cticor", "ArCTIc", "CTI correction performed using ArCTIc v"+w.cy_version_arctic())
-        header.set("ctipar", "ArCTIc", "CTI correction performed using ArCTIc v"+w.cy_version_arctic())
+        # TBD
+        # print(w.cy_version_arctic())
+        header.set(
+            "cticor",
+            "ArCTIc",
+            "CTI correction performed using ArCTIc v" + w.cy_version_arctic(),
+        )
+        header.set(
+            "ctipar",
+            "ArCTIc",
+            "CTI correction performed using ArCTIc v" + w.cy_version_arctic(),
+        )
 
     return image_trailed
 
 
 def remove_cti(
     image,
     n_iterations,
@@ -375,15 +381,15 @@
     serial_traps=None,
     serial_express=0,
     serial_window_offset=0,
     serial_window_start=0,
     serial_window_stop=-1,
     serial_time_start=0,
     serial_time_stop=-1,
-    serial_prune_n_electrons=1e-10, 
+    serial_prune_n_electrons=1e-10,
     serial_prune_frequency=20,
     # Combined
     allow_negative_pixels=1,
     # Pixel bounce
     pixel_bounce=None,
     # Read noise de-amplification
     read_noise=None,
@@ -412,20 +418,22 @@
             2   Extra details.
     """
     image = np.copy(image).astype(np.double)
     image_remove_cti = np.copy(image).astype(np.double)
 
     if verbosity >= 1:
         w.cy_print_version()
-    
+
     # Attempt to estimate and remove read noise, so it it not amplified
     if read_noise is not None:
-        image_remove_cti,image_read_noise = read_noise.generate_SR_frames_from_image(image_remove_cti)
-        #image_remove_cti -= image_read_noise
-        print("\nMean of read noise:",np.mean(image_read_noise))        
+        image_remove_cti, image_read_noise = read_noise.generate_SR_frames_from_image(
+            image_remove_cti
+        )
+        # image_remove_cti -= image_read_noise
+        print("\nMean of read noise:", np.mean(image_read_noise))
 
     # Estimate the image with removed CTI more accurately each iteration
     for iteration in range(1, n_iterations + 1):
         if verbosity >= 1:
             print("Iter %d: " % iteration, end="", flush=True)
 
         # Model the effect of adding CTI trails
@@ -450,47 +458,47 @@
             serial_traps=serial_traps,
             serial_express=serial_express,
             serial_window_offset=serial_window_offset,
             serial_window_start=serial_window_start,
             serial_window_stop=serial_window_stop,
             serial_time_start=serial_time_start,
             serial_time_stop=serial_time_stop,
-            serial_prune_n_electrons=serial_prune_n_electrons, 
+            serial_prune_n_electrons=serial_prune_n_electrons,
             serial_prune_frequency=serial_prune_frequency,
             # Combined
             allow_negative_pixels=allow_negative_pixels,
             # Pixel bounce
             pixel_bounce=pixel_bounce,
             # Output
             verbosity=verbosity,
-            iteration=iteration
+            iteration=iteration,
         )
 
         # Improve the estimate of the image with CTI trails removed
         delta = image - image_add_cti
         if read_noise is not None:
             delta -= image_read_noise
-            delta_squared = delta ** 2
+            delta_squared = delta**2
             # Doing the following should be right, but biases the
             # mean of the output image
-            #delta *= delta_squared / ( delta_squared + read_noise.sigmaRN ** 2 )
+            # delta *= delta_squared / ( delta_squared + read_noise.sigmaRN ** 2 )
         image_remove_cti += delta
-        
+
         # Prevent negative image values
         if not allow_negative_pixels:
             image_remove_cti[image_remove_cti < 0.0] = 0.0
-        
+
         print(iteration)
         if iteration == 1 and n_iterations >= 2:
             image_remove_cti[image_remove_cti < 0.0] = 0.0
 
     # Add back the read noise, if it had been removed
     if read_noise is not None:
         image_remove_cti += image_read_noise
-   
+
     return image_remove_cti
 
 
 def CTI_model_for_HST_ACS(date):
     """
     Return arcticpy objects that provide a preset CTI model for the Hubble Space
     Telescope (HST) Advanced Camera for Surveys (ACS).
```

### Comparing `arcticpy-2.2/python/arcticpy/include/interface.hpp` & `arcticpy-2.3/python/arcticpy/include/interface.hpp`

 * *Files identical despite different names*

### Comparing `arcticpy-2.2/python/arcticpy/pixel_bounce.py` & `arcticpy-2.3/python/arcticpy/pixel_bounce.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,155 +1,156 @@
 import numpy as np
 
+
 class PixelBounce:
 
     """
-    In flat fields acquired during ground testing of Euclid CCDs, the serial 
-    overscan shows spurious features that may be a combination of CTI and pixel 
+    In flat fields acquired during ground testing of Euclid CCDs, the serial
+    overscan shows spurious features that may be a combination of CTI and pixel
     bounce. In particular, the spurious signal dies away over several pixels but
-    is not monotonic. An increase between pixels 2 and 3 of the overscan region 
-    cannot be due to CTI. 
-    
-    To model pixel bounce, we regard the reference voltage as receiving an 
+    is not monotonic. An increase between pixels 2 and 3 of the overscan region
+    cannot be due to CTI.
+
+    To model pixel bounce, we regard the reference voltage as receiving an
     impulse when the signal voltage changes suddenly, then returning to ground
     as a heavily damped harmonic oscillator. Correlated double sampling then
-    produces a spurious, oscillating bias offset in the first few pixels after 
-    the change in signal. 
-    
-    Parameters of a damped harmonic oscillator are 
-    * the natural frequency and damping - both of which presumably depend on 
-      capacitance between the sampling phase and ground. 
-    * an initial amplitude and velocity of oscillation - which could depend on 
-      the coupling between the signal and reference voltage, and the clocking time, 
+    produces a spurious, oscillating bias offset in the first few pixels after
+    the change in signal.
+
+    Parameters of a damped harmonic oscillator are
+    * the natural frequency and damping - both of which presumably depend on
+      capacitance between the sampling phase and ground.
+    * an initial amplitude and velocity of oscillation - which could depend on
+      the coupling between the signal and reference voltage, and the clocking time,
       during which the spurious bias might start to oscillate unnoticed.
-    
+
 
     Parameters
     ----------
-    kA : float 
-        Initial condition of reference volatage in the pixel after a change in 
+    kA : float
+        Initial condition of reference volatage in the pixel after a change in
         signal voltage.
     kv : float
-        Initial condition of rate of change of reference volatage in the pixel 
+        Initial condition of rate of change of reference volatage in the pixel
         after a change in signal voltage.
     gamma : float
         Damping coefficicent of oscillations in the reference voltage, expressed
         as a ~half life in units of the time between clocks.
     omega : float
-        Frequency of oscillations in the reference voltage, in units (per pixel) 
+        Frequency of oscillations in the reference voltage, in units (per pixel)
         i.e. freq in Hz * clock speed.
     """
-    
-    def __init__(
-        self,
-        kA=0, 
-        kv=0, 
-        gamma=1.,
-        omega=1.
-    ):
-        if(gamma<0): raise Exception("Damping factor gamma cannot be negative")
-        if(omega<0): raise Exception("Oscillation frequency omega should not be negative")
+
+    def __init__(self, kA=0, kv=0, gamma=1.0, omega=1.0):
+        if gamma < 0:
+            raise Exception("Damping factor gamma cannot be negative")
+        if omega < 0:
+            raise Exception("Oscillation frequency omega should not be negative")
         self.kA = kA
         self.kv = kv
         self.gamma = gamma
         self.omega = omega
 
     @property
     def omega0(self):
-        return np.sqrt(omega**2 + gamma**2) # natural frequency of oscillator
+        return np.sqrt(omega**2 + gamma**2)  # natural frequency of oscillator
 
     def add_pixel_bounce(
         self,
         image,
         parallel_window_start=0,
         parallel_window_stop=-1,
         serial_window_start=0,
         serial_window_stop=-1,
-        verbosity=1
+        verbosity=1,
     ):
         """
         Add pixel bounce to an image, modelled as Damped Harmonic Oscillations (DHO)
         in a CCD's reference voltage, driven by sudden changes in the signal. This
-        creates spurious features in the serial (same row) direction away from any 
-        gradient in the image. 
-        
+        creates spurious features in the serial (same row) direction away from any
+        gradient in the image.
+
         Parameters
         ----------
         image : [[float]]
             The input array of pixel values, assumed to be in units of electrons.
-            
-            The first dimension is the "row" (y) index, the second is the "column" 
+
+            The first dimension is the "row" (y) index, the second is the "column"
             (x) index. Pixel bounce is only ever added in the x direction (ie during
             serial readout for images oriented as usual in ArCTIc).
-        
+
         parallel_window_start/stop : int
             First and last row of pixels (in the y direction) to process, for speed.
-            Default is to process the entire image. 
-        
+            Default is to process the entire image.
+
         serial_window_start/stop : int
             First and last column of pixels (in the x direction) to process, for speed.
-            Default is to process the entire image. 
-    
+            Default is to process the entire image.
+
         Returns
         -------
         image : [[float]]
             The output array of pixel values.
         """
-                
+
         # Parse inputs needed to process only a subset of the image
         image = np.copy(image).astype(np.double)
-        if (self.kA == 0) and (self.kv == 0): return image
+        if (self.kA == 0) and (self.kv == 0):
+            return image
         n_y, n_x = image.shape
-        if parallel_window_stop == -1: parallel_window_stop = n_y
-        if serial_window_stop == -1: serial_window_stop = n_x
-        image_subarray = image[parallel_window_start:parallel_window_stop, 
-                               serial_window_start:serial_window_stop]
-        n_y, n_x = image_subarray.shape            
-        
+        if parallel_window_stop == -1:
+            parallel_window_stop = n_y
+        if serial_window_stop == -1:
+            serial_window_stop = n_x
+        image_subarray = image[
+            parallel_window_start:parallel_window_stop,
+            serial_window_start:serial_window_stop,
+        ]
+        n_y, n_x = image_subarray.shape
+
         # Pre-calcualte useful quantities from eqn (43) of
         # Cieslinski & Ratkiewicz (2005) https://arxiv.org/abs/physics/0507182
         epsilon = 1
         coeffA = 2 * np.exp(-1 * self.gamma * epsilon) * np.cos(self.omega * epsilon)
         coeffB = np.exp(-2 * self.gamma * epsilon)
-        
+
         # Initialise bias offset voltage, which should settle during prescan
         # of each row
         bias = np.zeros(image_subarray.shape)
         biasm1 = np.zeros(n_y)
-        
+
         # Read out (a column of) pixels along a row, starting at second pixel (this
         # assumes the first pixel in each row cannot be affected by pixel bounce, as
         # the electronics have been reset and stabilised during prescan).
         for i in range(1, n_x):
-        
-            # Store previous values of bias, so difference equation can 
-            # compute rates of change 
+            # Store previous values of bias, so difference equation can
+            # compute rates of change
             biasm2 = biasm1.copy()
             biasm1 = bias[:, i - 1].copy()
-    
+
             # What electronic impulse is being experienced?
-            delta = image_subarray[:, i] - image_subarray[:, i - 1] 
-            
+            delta = image_subarray[:, i] - image_subarray[:, i - 1]
+
             # Impose this (linearly) on the difference equation,
             # as one term that creates a bias offset (propto pixel_bounce_kA)
             # and one that creates a rate of change of bias (propto pixel_bounce_kV)
             biasm1 += (self.kA - self.kv) * delta
             biasm2 += (self.kA - 2 * self.kv) * delta
-            
+
             # DHO difference equation, Cieslinski & Ratkiewicz (2005) eqn (43)
             bias[:, i] = coeffA * biasm1 - coeffB * biasm2
 
         # Spurious bias caused by correlated double sampling
-        image[parallel_window_start:parallel_window_stop, 
-              serial_window_start:serial_window_stop] -= bias[:,:]
-        
-        return image
+        image[
+            parallel_window_start:parallel_window_stop,
+            serial_window_start:serial_window_stop,
+        ] -= bias[:, :]
 
+        return image
 
-   
     def remove_pixel_bounce(
         self,
         image,
         n_iterations,
         parallel_window_start=0,
         parallel_window_stop=-1,
         serial_window_start=0,
@@ -161,90 +162,85 @@
         pixel bounce is added to it, recovers the input.
         """
         image = np.copy(image).astype(np.double)
         image_remove_pixel_bounce = np.copy(image).astype(np.double)
         for iteration in range(1, n_iterations + 1):
             if verbosity >= 1:
                 print("Iter %d: " % iteration, end="", flush=True)
-        
+
             # Iteratively add pixel bounce to a model of the corrected image
             image_add_pixel_bounce = self.add_pixel_bounce(
                 image_remove_pixel_bounce,
                 parallel_window_start=parallel_window_start,
                 parallel_window_stop=parallel_window_stop,
                 serial_window_start=serial_window_start,
                 serial_window_stop=serial_window_stop,
-                verbosity=verbosity
+                verbosity=verbosity,
             )
 
             # Improve the estimate of the image with pixel bounce removed
             image_remove_pixel_bounce += image - image_add_pixel_bounce
-        
+
         return image_remove_pixel_bounce
 
-  
-  
-    def add_pixel_bounce_slow(
-        self,
-        image,
-        do_Plot = False
-    ):
+    def add_pixel_bounce_slow(self, image, do_Plot=False):
         """
         C++ style version, looping over each row one at a time
         """
         # Pre-calcualte (once) useful quantities from eqn (43) of
         # Cieslinski & Ratkiewicz (2005) https://arxiv.org/abs/physics/0507182
         epsilon = 1
-        #omega = np.sqrt(self.omegaO**2 - self.gamma**2)
+        # omega = np.sqrt(self.omegaO**2 - self.gamma**2)
         coeffA = 2 * np.exp(-1 * self.gamma * epsilon) * np.cos(self.omega * epsilon)
         coeffB = np.exp(-2 * self.gamma * epsilon)
-        biasm1 = 0.
-        
+        biasm1 = 0.0
+
         # Read out one column of pixels through the (column of) traps
         n_rows_in_image, n_columns_in_image = image.shape
         import copy
+
         for row_index in range(n_rows_in_image):
-            
             print("Bouncing, one row at a time")
-            
+
             # Initialise bias offset voltage, which should settle during prescan
             # of each row
-            bias = np.zeros((1,n_columns_in_image))
-            
+            bias = np.zeros((1, n_columns_in_image))
+
             # Each pixel
-            #for row_index in window_row_range:
+            # for row_index in window_row_range:
             for column_index in range(1, n_columns_in_image):
-                
-                # Store previous values of bias, so difference equation can 
-                # compute rates of change 
+                # Store previous values of bias, so difference equation can
+                # compute rates of change
                 biasm2 = copy.copy(biasm1)
-                biasm1 = bias[row_index,column_index - 1]
-    
+                biasm1 = bias[row_index, column_index - 1]
+
                 # What electronic impulse is being experienced?
-                delta = image[row_index, column_index] - image[row_index, column_index - 1] 
-                
+                delta = (
+                    image[row_index, column_index] - image[row_index, column_index - 1]
+                )
+
                 # Impose this (linearly) on the difference equation,
                 # as one term that creates a bias offset (propto pixel_bounce_kA)
                 # and one that creates a rate of change of bias (propto pixel_bounce_kV)
                 biasm1 += (self.kA - self.kv) * delta
                 biasm2 += (self.kA - 2 * self.kv) * delta
-                
+
                 # DHO difference equation, Cieslinski & Ratkiewicz (2005) eqn (43)
-                bias[0,column_index] = coeffA * biasm1 - coeffB * biasm2
-                
-            image[row_index:row_index+1, :] -= bias
-   
-        return image
-    
+                bias[0, column_index] = coeffA * biasm1 - coeffB * biasm2
 
+            image[row_index : row_index + 1, :] -= bias
+
+        return image
 
 
 """
 Standalone functions to call the above, but mirroring syntax of add_cti() and remove_cti()
 """
+
+
 def add_pixel_bounce(
     image,
     pixel_bounce=None,
     parallel_window_start=0,
     parallel_window_stop=-1,
     serial_window_start=0,
     serial_window_stop=-1,
@@ -253,18 +249,19 @@
     if pixel_bounce is not None:
         image = pixel_bounce.add_pixel_bounce(
             image,
             parallel_window_start=parallel_window_start,
             parallel_window_stop=parallel_window_stop,
             serial_window_start=serial_window_start,
             serial_window_stop=serial_window_stop,
-            verbosity=verbosity
+            verbosity=verbosity,
         )
     return image
-   
+
+
 def remove_pixel_bounce(
     image,
     n_iterations,
     pixel_bounce=None,
     parallel_window_start=0,
     parallel_window_stop=-1,
     serial_window_start=0,
@@ -275,9 +272,10 @@
         image = pixel_bounce.remove_pixel_bounce(
             image,
             n_iterations,
             parallel_window_start=parallel_window_start,
             parallel_window_stop=parallel_window_stop,
             serial_window_start=serial_window_start,
             serial_window_stop=serial_window_stop,
-            verbosity=verbosity)
+            verbosity=verbosity,
+        )
     return image
```

### Comparing `arcticpy-2.2/python/arcticpy/read_noise.py` & `arcticpy-2.3/python/arcticpy/read_noise.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 import arcticpy as ac
 import matplotlib as mpl
-from scipy.optimize import curve_fit 
+from scipy.optimize import curve_fit
 
 """
 CTI correction moves trailed electrons back to their proper location, but also
 moves read noise - which was not trailed in the first place. The net effect is to
 amplify read noise, and hide the difference in the (anti)correlation between
 adjacent pixels. 
 
@@ -72,716 +72,938 @@
                   matrix_size=5, fprSize=5, 
                   parallel_roe, parallel_ccd, parallel_traps)
 
 
 
 """
 
+
 class ReadNoise:
     def __init__(
-            self, 
-            sigma_readnoise=0.0, 
-            adjacency=0.3, 
-            noise_model_scaling=1.0, # originally 0.75 
-            amplitude_scale=0.2,     # originally 0.33
-            n_iter=200,
-            sr_fraction=None,
-            serial=True,
-            covariance_matrices=None,
-            **kwargs
-            
+        self,
+        sigma_readnoise=0.0,
+        adjacency=0.3,
+        noise_model_scaling=1.0,  # originally 0.75
+        amplitude_scale=0.2,  # originally 0.33
+        n_iter=200,
+        sr_fraction=None,
+        serial=True,
+        covariance_matrices=None,
+        **kwargs
     ):
         self.sigmaRN = sigma_readnoise
         self.adjacency = adjacency
         self.ampScale = amplitude_scale
         self.outScale = noise_model_scaling
         self.n_iter = n_iter
         self.smoothCol = serial
-        self.sigmaSky = None        
+        self.sigmaSky = None
         self.skyFrameSim = None
         self.readnoiseFrameSim = None
         self.SRfrac_optimised = None
         self.arcKwargs = {}
         self.covarianceMatrices = {}
         self.dataFrames = {}
 
-#        self._sr_fraction = sr_fraction
-#        self._sr_fraction_optimised = None
+    #        self._sr_fraction = sr_fraction
+    #        self._sr_fraction_optimised = None
 
-#    @property
-#    def sr_fraction(self):
-#        """
-#        RMS value of read noise, in units of electrons
-#        """
-#        if self._sr_fraction is not None: return self._sr_fraction
-#        #if self._sr_fraction_optimised is None: self.optimise_sr_fraction()
-#        return self._sr_fraction_optimised
-#
-#    @sr_fraction.setter
-#    def sr_fraction(self, value):
-#        self._sr_fraction = value
-#
-#    @property
-#    def sr_fraction_optimised(self, **kwargs):
-#        """
-#        Value of S+R splitting fraction that will minimise pixel-to-pixel covariance
-#        after CTI correction
-#        """
-#        if self._sr_fraction_optimised is None: self.optimise_sr_fraction(**kwargs)
-#        return self._sr_fraction_optimised
-#
-#    @sr_fraction_optimised.setter
-#    def sr_fraction_optimised(self, value):
-#        self._sr_fraction_optimised = value
+    #    @property
+    #    def sr_fraction(self):
+    #        """
+    #        RMS value of read noise, in units of electrons
+    #        """
+    #        if self._sr_fraction is not None: return self._sr_fraction
+    #        #if self._sr_fraction_optimised is None: self.optimise_sr_fraction()
+    #        return self._sr_fraction_optimised
+    #
+    #    @sr_fraction.setter
+    #    def sr_fraction(self, value):
+    #        self._sr_fraction = value
+    #
+    #    @property
+    #    def sr_fraction_optimised(self, **kwargs):
+    #        """
+    #        Value of S+R splitting fraction that will minimise pixel-to-pixel covariance
+    #        after CTI correction
+    #        """
+    #        if self._sr_fraction_optimised is None: self.optimise_sr_fraction(**kwargs)
+    #        return self._sr_fraction_optimised
+    #
+    #    @sr_fraction_optimised.setter
+    #    def sr_fraction_optimised(self, value):
+    #        self._sr_fraction_optimised = value
 
     @property
     def sigma(self):
         """
         RMS value of read noise, in units of electrons
         """
         return self._sigma
 
     @sigma.setter
     def sigma(self, value):
         if value < 0:
-            value = 0.
+            value = 0.0
         self._sigma = value
 
     ###############
-    # 
-    #USER-FACING FUNCTIONS
+    #
+    # USER-FACING FUNCTIONS
     #
     ###############
-    def set_arctic_parameters(
-            self,
-            **kwargs
-    ):
-        '''
+    def set_arctic_parameters(self, **kwargs):
+        """
         Function for pre-setting arCTIc parameters (such as CCD, trap density, and ROE)
         This is a convenience function to eliminate multiple, bulky keyword argument calls in other functions
-        If desired, the user can still specify or overwrite these values (on the fly) in the other functions 
-        by explicitly calling the keyword arguments there. 
+        If desired, the user can still specify or overwrite these values (on the fly) in the other functions
+        by explicitly calling the keyword arguments there.
 
         Parameters
         ----------
         **kwargs : variables
             Keyword arguments specifying arCTIc parameters
-        '''
+        """
         self.arcKwargs = kwargs
+
     ###############
     ###############
-    def generate_SR_frames_from_image(
-            self,
-            image,
-            sr_fraction = None
-    ):
-        '''
+    def generate_SR_frames_from_image(self, image, sr_fraction=None):
+        """
         Function for generating a model of read noise in an image, using the level specified in the
-        initial ReadNoise call. Once modeled, the read noise component is separated from the data, 
-        leaving a smooth "S" component and a read-noise-only "R" component. The S somponent can then 
+        initial ReadNoise call. Once modeled, the read noise component is separated from the data,
+        leaving a smooth "S" component and a read-noise-only "R" component. The S somponent can then
         be CTI-corrected and recombined with the R model to minimise residual covariance in the image.
 
         Parameters
         ----------
 
         image: 2D numpy aray
             This can be a real science image or a simulation generated by <optimise_SR_fraction>
 
         sr_fraction: float
             scale fraction specifying what percentage of read noise should be separated into the R
             frame. Default is set to the optimised value measured in <optimise_SR_frac>, or 100%
             if <optimise_SR_frac> has not been previously run.
 
-        
-        '''
+
+        """
         ampReadNoise = self.sigmaRN
 
-        #if sr_fraction is unset, use system value
+        # if sr_fraction is unset, use system value
         if sr_fraction == None:
             sr_fraction = self.SRfrac_optimised
             # if optimisation is not set, default to 100%
             if sr_fraction == None:
                 sr_fraction = 1.0
 
         imageIn = image
-        imageAdj = np.zeros_like(imageIn) #adjustment image (for read noise modeling)
-        imageOut = imageIn.copy()         #output ("smoothed") image
-        
+        imageAdj = np.zeros_like(imageIn)  # adjustment image (for read noise modeling)
+        imageOut = imageIn.copy()  # output ("smoothed") image
+
         nrows = imageIn.shape[0]
         ncols = imageIn.shape[1]
-        
-        rmsGlobal = 0.
-        nrmsGlobal = 0.
-        
+
+        rmsGlobal = 0.0
+        nrmsGlobal = 0.0
+
         smoother = 1
-        print('iter','model_rms','target_rms','residual')
+        print("iter", "model_rms", "target_rms", "residual")
         for s in range(self.n_iter):
-            oldchk = ampReadNoise-rmsGlobal
-            imageAdj= self._determine_noise_model(imageIn,imageOut)
+            oldchk = ampReadNoise - rmsGlobal
+            imageAdj = self._determine_noise_model(imageIn, imageOut)
 
-            if (ampReadNoise-rmsGlobal) > 0:
+            if (ampReadNoise - rmsGlobal) > 0:
                 imageOut += imageAdj * self.outScale / smoother
                 noiseImage = imageIn - imageOut
             else:
                 imageOut -= imageAdj * self.outScale / smoother
                 noiseImage = imageIn - imageOut
-        
-            cond = abs(imageIn > 0.1)|abs(imageOut > 0.1)
-            rmsGlobal = np.sum(noiseImage[cond]**2)
+
+            cond = abs(imageIn > 0.1) | abs(imageOut > 0.1)
+            rmsGlobal = np.sum(noiseImage[cond] ** 2)
             nrmsGlobal = noiseImage[cond].size
 
-            rmsGlobal = np.sqrt(rmsGlobal/nrmsGlobal)
-            print("\033[K",end='\r')
-            print('%4d  %f    %5.2f    %f'%(s,rmsGlobal, self.sigmaRN, (ampReadNoise-rmsGlobal)),end='')
-            
-            chk = ampReadNoise-rmsGlobal
-            if chk*oldchk < 0:
-                smoother+=1
-                
-            if type(ampReadNoise)==np.ndarray:
+            rmsGlobal = np.sqrt(rmsGlobal / nrmsGlobal)
+            print("\033[K", end="\r")
+            print(
+                "%4d  %f    %5.2f    %f"
+                % (s, rmsGlobal, self.sigmaRN, (ampReadNoise - rmsGlobal)),
+                end="",
+            )
+
+            chk = ampReadNoise - rmsGlobal
+            if chk * oldchk < 0:
+                smoother += 1
+
+            if type(ampReadNoise) == np.ndarray:
                 if np.max(ampReadNoise - rmsGlobal) < 0.0001:
                     break
             else:
                 if abs(ampReadNoise - rmsGlobal) < 0.0001:
                     break
 
-        #scale the smooth and noise frames if <sr_fraction> != 1
-        if sr_fraction !=1:
-            imageOut+=noiseImage
-            noiseImage*=sr_fraction
-            imageOut-=noiseImage
-                
-        return imageOut,noiseImage #These are the "S" and "R" frames, respectively
-    ###############    
+        # scale the smooth and noise frames if <sr_fraction> != 1
+        if sr_fraction != 1:
+            imageOut += noiseImage
+            noiseImage *= sr_fraction
+            imageOut -= noiseImage
+
+        return imageOut, noiseImage  # These are the "S" and "R" frames, respectively
+
+    ###############
     ###############
     def optimise_SR_fraction(
-            self,
-            background_level,
-            background_sigma=None,
-            n_pixels=2048,    
-            subchip_size=500,  
-            matrix_size=5,    
-            fom_method='box',
-            **kwargs
+        self,
+        background_level,
+        background_sigma=None,
+        n_pixels=2048,
+        subchip_size=500,
+        matrix_size=5,
+        fom_method="box",
+        **kwargs
     ):
-        '''
+        """
         Adjust parameters of the S+R algorithm that estimates the read noise in an image.
         The image itself is not required; merely its dimensions and sky level parameters.
-        
+
         It works by simulating a subchip_size x subchip_size regions of the image, one
         at each corner of the CCD, then tries to minimise the pixel-to-pixel covariance
         after CTI correction in the most distant corner.
-        
+
         This merely adjusts the self parameters contained within the ReadNoise instance.
-        The final optimised S+R value is stored as the <optimised_SR_fraction> class variable 
-        
-        Parameters 
+        The final optimised S+R value is stored as the <optimised_SR_fraction> class variable
+
+        Parameters
         ----------
         background_level : Float
             The mean (sky) background level across the image.
 
         background_sigma : Float
             The rms variation per pixel around the background level.
             If not specified, it will assume sqrt(background_level) for shot noise.
-        
+
         n_pixels : Float or (Float, Float)
             The number of pixels in the CCD. If a single number is supplied, it assumes
             the CCD is square. If two numbers are supplied, the assumed order is (n_y,n_x).
-    
+
         subchip_size : Float
-            size of the cutout region, to test CTI behaviour in different regimes (e.g. far from readout, close to readout, etc.) 
-    
+            size of the cutout region, to test CTI behaviour in different regimes (e.g. far from readout, close to readout, etc.)
+
         matrix_size : Int
             Size of covariance matrix used to estimate covariance. By default the program creates a 5x5 matrix
 
         fom_method : String
             Method used to estimate the mean value of a covariance matrix, for figure-of-merit purposes. Can be:
                 box : take a square (3x3) region around the central pixel [DEFAULT]
                 row : take all cells along the central row
                 column : take all cells along the central column
 
-        **kwargs : parameters that characterise CTI features in arCTIc (trap density, CCD, read out electronics (ROE) descriptions) 
-        '''
+        **kwargs : parameters that characterise CTI features in arCTIc (trap density, CCD, read out electronics (ROE) descriptions)
+        """
 
         # Parse inputs
         if type(n_pixels) == int:
-            n_pixels=(n_pixels,n_pixels)
+            n_pixels = (n_pixels, n_pixels)
         chip_size = n_pixels
-        if background_sigma==None:
+        if background_sigma == None:
             background_sigma = np.sqrt(background_level)
         self.sigmaSky = background_sigma
-        
-        #set prescan regions (this simulates the maximum possible CTI trailing, averaged at the far edge of the real CCD)
-        if 'parallel_roe' in kwargs:
-            kwargs['parallel_roe'].prescan_offset = n_pixels[0]+(subchip_size//2)
-        if 'serial_roe' in kwargs:
-            kwargs['serial_roe'].prescan_offset = n_pixels[1]+(subchip_size//2)
 
-        #container for optimised values
+        # set prescan regions (this simulates the maximum possible CTI trailing, averaged at the far edge of the real CCD)
+        if "parallel_roe" in kwargs:
+            kwargs["parallel_roe"].prescan_offset = n_pixels[0] + (subchip_size // 2)
+        if "serial_roe" in kwargs:
+            kwargs["serial_roe"].prescan_offset = n_pixels[1] + (subchip_size // 2)
+
+        # container for optimised values
         self.optVals = {}
 
-        #if they don't exist, make the sky background and readnoise images for the simulations
+        # if they don't exist, make the sky background and readnoise images for the simulations
         if (self.skyFrameSim is None) & (self.readnoiseFrameSim is None):
-            self._create_initial_sim_images(background_level,background_sigma,image_size=subchip_size)
+            self._create_initial_sim_images(
+                background_level, background_sigma, image_size=subchip_size
+            )
+
+        # create "simulation noise" covariance matrix (estimated from the sky+readnoise image)
+        # in this case, the fpr decrement is set to zero, because there is no CTI trailing
+        sim_matrix = self.covariance_matrix_from_image(
+            self.skyFrameSim + self.readnoiseFrameSim,
+            matrix_size=matrix_size,
+            fprSize=5,
+        )
+
+        # ideally, the matrix should be all zeros except for the centre square (== sigmaSky**2 + sigmaReadnoise**2)
+        # therefore, subtracting this from sim_matrix will provide the simulation noise covariance
+        sim_matrix[matrix_size // 2, matrix_size // 2] -= (
+            self.sigmaRN**2 + self.sigmaSky**2
+        )
 
-        #create "simulation noise" covariance matrix (estimated from the sky+readnoise image)
-        #in this case, the fpr decrement is set to zero, because there is no CTI trailing
-        sim_matrix = self.covariance_matrix_from_image(self.skyFrameSim+self.readnoiseFrameSim,matrix_size=matrix_size,fprSize=5)
+        self.optVals["pre-benchmark"] = sim_matrix
 
-        #ideally, the matrix should be all zeros except for the centre square (== sigmaSky**2 + sigmaReadnoise**2)
-        #therefore, subtracting this from sim_matrix will provide the simulation noise covariance
-        sim_matrix[matrix_size//2,matrix_size//2] -= (self.sigmaRN**2+self.sigmaSky**2)
-
-        self.optVals['pre-benchmark'] = sim_matrix
-
-        #run S+R routine at 0% and 100% S+R fraction
+        # run S+R routine at 0% and 100% S+R fraction
         result_array = np.array([])
-        matrix_array = np.zeros((2,matrix_size,matrix_size))
-        sr_frac = np.array([0.0,1.0])
+        matrix_array = np.zeros((2, matrix_size, matrix_size))
+        sr_frac = np.array([0.0, 1.0])
         for frac in sr_frac:
-            print('\nestimating S+R covariance at %d percent level'%(100*frac))
-            raw_matrix,correction_matrix = self._estimate_residual_covariance(self.skyFrameSim,self.readnoiseFrameSim,frac,matrix_size=matrix_size,**self.arcKwargs,**kwargs)
+            print("\nestimating S+R covariance at %d percent level" % (100 * frac))
+            raw_matrix, correction_matrix = self._estimate_residual_covariance(
+                self.skyFrameSim,
+                self.readnoiseFrameSim,
+                frac,
+                matrix_size=matrix_size,
+                **self.arcKwargs,
+                **kwargs
+            )
             matrix_array[int(frac)] = correction_matrix
-            result = self.figure_of_merit(correction_matrix,fom_method=fom_method) #TODO: check to see if changing subgrid_size actually matters
-            result_array = np.append(result_array,result)
-        #interpolate between the results to determine the point of minimum residual covariance
-        a_fit,cov=curve_fit(self._fitter_function,sr_frac,result_array,absolute_sigma=True)
+            result = self.figure_of_merit(
+                correction_matrix, fom_method=fom_method
+            )  # TODO: check to see if changing subgrid_size actually matters
+            result_array = np.append(result_array, result)
+        # interpolate between the results to determine the point of minimum residual covariance
+        a_fit, cov = curve_fit(
+            self._fitter_function, sr_frac, result_array, absolute_sigma=True
+        )
         m = a_fit[1]
         b = a_fit[0]
-        xint = -b/m #this intercept will be the optimised S+R fraction (where mean covariance=0)
+        xint = (
+            -b / m
+        )  # this intercept will be the optimised S+R fraction (where mean covariance=0)
 
-        #store final optimised fraction as a class variable
+        # store final optimised fraction as a class variable
         self.SRfrac_optimised = xint
-        #self.optVals['optSRfrac'] = xint
+        # self.optVals['optSRfrac'] = xint
+
     ###############
     ###############
     def optimise_SR_fraction_from_image(
-            self,
-            image,
-            subchip_size=500, #size of the cutout region, to test CTI behaviour (a subset of pixels far form the readout)  
-            matrix_size=5,    #covariance matrix size (NxN array)
-            fom_method='box',
-            **kwargs
+        self,
+        image,
+        subchip_size=500,  # size of the cutout region, to test CTI behaviour (a subset of pixels far form the readout)
+        matrix_size=5,  # covariance matrix size (NxN array)
+        fom_method="box",
+        **kwargs
     ):
-        '''
+        """
         A wrapper function for running the S+R optimisation routine using a real astronomical image rather than theoretical values.
         This routine still calls <optimise_SR_fraction> but the sky paramerters and image size are determined from the data itself.
 
         Parameters
         ----------
         image : numpy array
             2D numpy array containing the pixel values of the image
 
         subchip_size : Float
-            size of the cutout region, to test CTI behaviour in different regimes (e.g. far from readout, close to readout, etc.) 
-    
+            size of the cutout region, to test CTI behaviour in different regimes (e.g. far from readout, close to readout, etc.)
+
         matrix_size : Int
             Size of covariance matrix used to estimate covariance. By default the program creates a 5x5 matrix
 
         fom_method : String
             Method used to estimate the mean value of a covariance matrix, for figure-of-merit purposes. Can be:
                 box : take a square (3x3) region around the central pixel [DEFAULT]
                 row : take all cells along the central row
                 column : take all cells along the central column
 
-        **kwargs : parameters that characterise CTI features in arCTIc (trap density, CCD, read out electronics (ROE) descriptions) 
-        
-        '''
+        **kwargs : parameters that characterise CTI features in arCTIc (trap density, CCD, read out electronics (ROE) descriptions)
+
+        """
 
         image_shape = image.shape
         sky_level = np.median(image)
-        sky_back = np.sqrt(sky_level) #assume pure shot noise for now
+        sky_back = np.sqrt(sky_level)  # assume pure shot noise for now
+
+        self.optimise_SR_fraction(
+            sky_level,
+            sky_back,
+            image_shape,
+            subchip_size,
+            matrix_size,
+            fom_method,
+            **kwargs
+        )
 
-        self.optimise_SR_fraction(sky_level,sky_back,image_shape,subchip_size,matrix_size,fom_method,**kwargs)     
     ###############
     ###############
     def calculate_covariance_corners_from_image(
-            self,
-            image,
+        self,
+        image,
     ):
-        raise NotImplementedError           
+        raise NotImplementedError
+
+    ###############
     ###############
-    ###############    
     def plot_matrix(
-            self,
-            covariance_matrix,
-            supressCentralPix=True,
-            title='MyPlotMatrix',
-            clearFrame=True,
-            **kwargs
+        self,
+        covariance_matrix,
+        supressCentralPix=True,
+        title="MyPlotMatrix",
+        clearFrame=True,
+        **kwargs
     ):
         if supressCentralPix == True:
             matrix = covariance_matrix.copy()
             matrix_size = matrix.shape[0]
-            matrix[matrix_size//2,matrix_size//2] = 0 # set central pixel to zero, to better see correlation dynamic range
+            matrix[
+                matrix_size // 2, matrix_size // 2
+            ] = 0  # set central pixel to zero, to better see correlation dynamic range
         else:
             matrix = covariance_matrix.copy()
 
         if clearFrame:
             mpl.pyplot.clf()
-        mpl.pyplot.imshow(matrix,cmap='bwr',**kwargs)
+        mpl.pyplot.imshow(matrix, cmap="bwr", **kwargs)
         mpl.pyplot.colorbar()
         mpl.pyplot.title(title)
         mpl.pyplot.show()
+
     ###############
     ###############
-    def plot_optimised_covariance_matrices(
-            self
-    ):
+    def plot_optimised_covariance_matrices(self):
         mpl.pyplot.figure()
         mpl.pyplot.subplot(221)
-        self.plot_matrix(self.optVals['noCTIQuadMatrix_diff'],title='Readout Corner',clearFrame=False,vmin=-0.01,vmax=0.01)
+        self.plot_matrix(
+            self.optVals["noCTIQuadMatrix_diff"],
+            title="Readout Corner",
+            clearFrame=False,
+            vmin=-0.01,
+            vmax=0.01,
+        )
         mpl.pyplot.subplot(222)
-        self.plot_matrix(self.optVals['serialQuadMatrix_diff'],title='Serial Corner',clearFrame=False,vmin=-0.01,vmax=0.01)
+        self.plot_matrix(
+            self.optVals["serialQuadMatrix_diff"],
+            title="Serial Corner",
+            clearFrame=False,
+            vmin=-0.01,
+            vmax=0.01,
+        )
         mpl.pyplot.subplot(223)
-        self.plot_matrix(self.optVals['parallelQuadMatrix_diff'],title='Parallel Corner',clearFrame=False,vmin=-0.01,vmax=0.01)
+        self.plot_matrix(
+            self.optVals["parallelQuadMatrix_diff"],
+            title="Parallel Corner",
+            clearFrame=False,
+            vmin=-0.01,
+            vmax=0.01,
+        )
         mpl.pyplot.subplot(224)
-        self.plot_matrix(self.optVals['combinedQuadMatrix_diff'],title='Combined Corner',clearFrame=False,vmin=-0.01,vmax=0.01)            
+        self.plot_matrix(
+            self.optVals["combinedQuadMatrix_diff"],
+            title="Combined Corner",
+            clearFrame=False,
+            vmin=-0.01,
+            vmax=0.01,
+        )
+
     ###############
 
-    
     ###############
     #
-    #BACKGROUND FUNCTIONS
+    # BACKGROUND FUNCTIONS
     #
     ###############
     def _determine_noise_model(self, imageIn, imageOut):
-        '''
+        """
         Method for estimating readnoise on image (in S+R fashion)
         assumes parallel+serial CTI trailing by default
-        '''
+        """
         readNoiseAmp = self.sigmaRN
-        
+
         dval0 = imageIn - imageOut
         dval0u = dval0.copy()
-        
-        dval0u[dval0u>1] = 1
-        dval0u[dval0u<-1] = -1
-        
-        dval9 = imageIn*0
-        dcount = imageIn*0
-        
-        dval9[:-1,:-1]+=(imageIn[1: ,1: ]-imageOut[1: ,1: ]); dcount[:-1,:-1]+=1
-        dval9[:-1,:  ]+=(imageIn[1: ,:  ]-imageOut[1: ,:  ]); dcount[:-1,:  ]+=1
-        dval9[:-1,1: ]+=(imageIn[1: ,:-1]-imageOut[1: ,:-1]); dcount[:-1,1: ]+=1
-        dval9[:  ,:-1]+=(imageIn[:  ,1: ]-imageOut[:  ,1: ]); dcount[:  ,:-1]+=1
-        dval9[:  ,:  ]+=(imageIn[:  ,:  ]-imageOut[:  ,:  ]); dcount[:  ,:  ]+=1
-        dval9[:  ,1: ]+=(imageIn[:  ,:-1]-imageOut[:  ,:-1]); dcount[:  ,1: ]+=1
-        dval9[1: ,:-1]+=(imageIn[:-1,1: ]-imageOut[:-1,1: ]); dcount[1: ,:-1]+=1
-        dval9[1: ,:  ]+=(imageIn[:-1,:  ]-imageOut[:-1,:  ]); dcount[1: ,:  ]+=1
-        dval9[1: ,1: ]+=(imageIn[:-1,:-1]-imageOut[:-1,:-1]); dcount[1: ,1: ]+=1
-        
-        dval9/=dcount
-        
+
+        dval0u[dval0u > 1] = 1
+        dval0u[dval0u < -1] = -1
+
+        dval9 = imageIn * 0
+        dcount = imageIn * 0
+
+        dval9[:-1, :-1] += imageIn[1:, 1:] - imageOut[1:, 1:]
+        dcount[:-1, :-1] += 1
+        dval9[:-1, :] += imageIn[1:, :] - imageOut[1:, :]
+        dcount[:-1, :] += 1
+        dval9[:-1, 1:] += imageIn[1:, :-1] - imageOut[1:, :-1]
+        dcount[:-1, 1:] += 1
+        dval9[:, :-1] += imageIn[:, 1:] - imageOut[:, 1:]
+        dcount[:, :-1] += 1
+        dval9[:, :] += imageIn[:, :] - imageOut[:, :]
+        dcount[:, :] += 1
+        dval9[:, 1:] += imageIn[:, :-1] - imageOut[:, :-1]
+        dcount[:, 1:] += 1
+        dval9[1:, :-1] += imageIn[:-1, 1:] - imageOut[:-1, 1:]
+        dcount[1:, :-1] += 1
+        dval9[1:, :] += imageIn[:-1, :] - imageOut[:-1, :]
+        dcount[1:, :] += 1
+        dval9[1:, 1:] += imageIn[:-1, :-1] - imageOut[:-1, :-1]
+        dcount[1:, 1:] += 1
+
+        dval9 /= dcount
+
         readNoiseAmpFraction = self.ampScale
         dval9u = dval9.copy()
-        if type(readNoiseAmp)==np.ndarray:
+        if type(readNoiseAmp) == np.ndarray:
             dval9u = dval9u.flatten()
             readNoiseAmp = readNoiseAmp.flatten()
-            dval9u[dval9u > readNoiseAmp*readNoiseAmpFraction] = (readNoiseAmp*readNoiseAmpFraction)[dval9u > readNoiseAmp*readNoiseAmpFraction]
-            dval9u[dval9u < readNoiseAmp*-readNoiseAmpFraction] = (readNoiseAmp*-readNoiseAmpFraction)[dval9u < readNoiseAmp*-readNoiseAmpFraction]
+            dval9u[dval9u > readNoiseAmp * readNoiseAmpFraction] = (
+                readNoiseAmp * readNoiseAmpFraction
+            )[dval9u > readNoiseAmp * readNoiseAmpFraction]
+            dval9u[dval9u < readNoiseAmp * -readNoiseAmpFraction] = (
+                readNoiseAmp * -readNoiseAmpFraction
+            )[dval9u < readNoiseAmp * -readNoiseAmpFraction]
             dval9u = dval9u.reshape(imageIn.shape)
-            readNoiseAmp = readNoiseAmp.reshape(imageIn.shape)        
+            readNoiseAmp = readNoiseAmp.reshape(imageIn.shape)
         else:
-            dval9u[dval9u > readNoiseAmp*readNoiseAmpFraction] = readNoiseAmp*readNoiseAmpFraction
-            dval9u[dval9u < readNoiseAmp*-readNoiseAmpFraction] = readNoiseAmp*-readNoiseAmpFraction
-            
-        dmod1 = imageIn*0
-        dmod1[1:,:] = imageOut[:-1,:] - imageOut[1:,:]
-        dmod2 = imageIn*0
-        dmod2[:-1,:] = imageOut[1:,:] - imageOut[:-1,:]
-        
+            dval9u[dval9u > readNoiseAmp * readNoiseAmpFraction] = (
+                readNoiseAmp * readNoiseAmpFraction
+            )
+            dval9u[dval9u < readNoiseAmp * -readNoiseAmpFraction] = (
+                readNoiseAmp * -readNoiseAmpFraction
+            )
+
+        dmod1 = imageIn * 0
+        dmod1[1:, :] = imageOut[:-1, :] - imageOut[1:, :]
+        dmod2 = imageIn * 0
+        dmod2[:-1, :] = imageOut[1:, :] - imageOut[:-1, :]
+
         if self.smoothCol:
-            cmod1 = imageIn*0
-            cmod1[:,1:] = imageOut[:,:-1] - imageOut[:,1:]
-            cmod2 = imageIn*0
-            cmod2[:,:-1] = imageOut[:,1:] - imageOut[:,:-1]
-            
+            cmod1 = imageIn * 0
+            cmod1[:, 1:] = imageOut[:, :-1] - imageOut[:, 1:]
+            cmod2 = imageIn * 0
+            cmod2[:, :-1] = imageOut[:, 1:] - imageOut[:, :-1]
+
         dmod1u = dmod1.copy()
-        if type(readNoiseAmp)==np.ndarray:
+        if type(readNoiseAmp) == np.ndarray:
             dmod1u = dmod1u.flatten()
             readNoiseAmp = readNoiseAmp.flatten()
-            dmod1u[dmod1u>readNoiseAmp*readNoiseAmpFraction] = (readNoiseAmp*readNoiseAmpFraction)[dmod1u>readNoiseAmp*readNoiseAmpFraction]
-            dmod1u[dmod1u<readNoiseAmp*-readNoiseAmpFraction] = (readNoiseAmp*-readNoiseAmpFraction)[dmod1u<readNoiseAmp*-readNoiseAmpFraction]
-            dmod1u = dmod1u.reshape(imageIn.shape)       
+            dmod1u[dmod1u > readNoiseAmp * readNoiseAmpFraction] = (
+                readNoiseAmp * readNoiseAmpFraction
+            )[dmod1u > readNoiseAmp * readNoiseAmpFraction]
+            dmod1u[dmod1u < readNoiseAmp * -readNoiseAmpFraction] = (
+                readNoiseAmp * -readNoiseAmpFraction
+            )[dmod1u < readNoiseAmp * -readNoiseAmpFraction]
+            dmod1u = dmod1u.reshape(imageIn.shape)
         else:
-            dmod1u[dmod1u>readNoiseAmp*readNoiseAmpFraction] = readNoiseAmp*readNoiseAmpFraction
-            dmod1u[dmod1u<readNoiseAmp*-readNoiseAmpFraction] = readNoiseAmp*-readNoiseAmpFraction
-            
+            dmod1u[dmod1u > readNoiseAmp * readNoiseAmpFraction] = (
+                readNoiseAmp * readNoiseAmpFraction
+            )
+            dmod1u[dmod1u < readNoiseAmp * -readNoiseAmpFraction] = (
+                readNoiseAmp * -readNoiseAmpFraction
+            )
+
         dmod2u = dmod2.copy()
-        if type(readNoiseAmp)==np.ndarray:
+        if type(readNoiseAmp) == np.ndarray:
             dmod2u = dmod2u.flatten()
             readNoiseAmp = readNoiseAmp.flatten()
-            dmod2u[dmod2u>readNoiseAmp*readNoiseAmpFraction] = (readNoiseAmp*readNoiseAmpFraction)[dmod2u>readNoiseAmp*readNoiseAmpFraction]
-            dmod2u[dmod2u<readNoiseAmp*-readNoiseAmpFraction] = (readNoiseAmp*-readNoiseAmpFraction)[dmod2u<readNoiseAmp*-readNoiseAmpFraction]
+            dmod2u[dmod2u > readNoiseAmp * readNoiseAmpFraction] = (
+                readNoiseAmp * readNoiseAmpFraction
+            )[dmod2u > readNoiseAmp * readNoiseAmpFraction]
+            dmod2u[dmod2u < readNoiseAmp * -readNoiseAmpFraction] = (
+                readNoiseAmp * -readNoiseAmpFraction
+            )[dmod2u < readNoiseAmp * -readNoiseAmpFraction]
             dmod2u = dmod2u.reshape(imageIn.shape)
-            readNoiseAmp = readNoiseAmp.reshape(imageIn.shape) 
+            readNoiseAmp = readNoiseAmp.reshape(imageIn.shape)
         else:
-            dmod2u[dmod2u>readNoiseAmp*readNoiseAmpFraction] = readNoiseAmp*readNoiseAmpFraction
-            dmod2u[dmod2u<readNoiseAmp*-readNoiseAmpFraction] = readNoiseAmp*-readNoiseAmpFraction
-            
+            dmod2u[dmod2u > readNoiseAmp * readNoiseAmpFraction] = (
+                readNoiseAmp * readNoiseAmpFraction
+            )
+            dmod2u[dmod2u < readNoiseAmp * -readNoiseAmpFraction] = (
+                readNoiseAmp * -readNoiseAmpFraction
+            )
+
         if self.smoothCol:
             cmod1u = cmod1.copy()
-            if type(readNoiseAmp)==np.ndarray:
+            if type(readNoiseAmp) == np.ndarray:
                 cmod1u = cmod1u.flatten()
                 readNoiseAmp = readNoiseAmp.flatten()
-                cmod1u[cmod1u>readNoiseAmp*readNoiseAmpFraction] = (readNoiseAmp*readNoiseAmpFraction)[cmod1u>readNoiseAmp*readNoiseAmpFraction]
-                cmod1u[cmod1u<readNoiseAmp*-readNoiseAmpFraction] = (readNoiseAmp*-readNoiseAmpFraction)[cmod1u<readNoiseAmp*-readNoiseAmpFraction]
+                cmod1u[cmod1u > readNoiseAmp * readNoiseAmpFraction] = (
+                    readNoiseAmp * readNoiseAmpFraction
+                )[cmod1u > readNoiseAmp * readNoiseAmpFraction]
+                cmod1u[cmod1u < readNoiseAmp * -readNoiseAmpFraction] = (
+                    readNoiseAmp * -readNoiseAmpFraction
+                )[cmod1u < readNoiseAmp * -readNoiseAmpFraction]
                 cmod1u = cmod1u.reshape(imageIn.shape)
                 readNoiseAmp = readNoiseAmp.reshape(imageIn.shape)
             else:
-                cmod1u[cmod1u>readNoiseAmp*readNoiseAmpFraction] = readNoiseAmp*readNoiseAmpFraction
-                cmod1u[cmod1u<readNoiseAmp*-readNoiseAmpFraction] = readNoiseAmp*-readNoiseAmpFraction
-                
+                cmod1u[cmod1u > readNoiseAmp * readNoiseAmpFraction] = (
+                    readNoiseAmp * readNoiseAmpFraction
+                )
+                cmod1u[cmod1u < readNoiseAmp * -readNoiseAmpFraction] = (
+                    readNoiseAmp * -readNoiseAmpFraction
+                )
+
             cmod2u = cmod2.copy()
-            if type(readNoiseAmp)==np.ndarray:
+            if type(readNoiseAmp) == np.ndarray:
                 cmod2u = cmod2u.flatten()
                 readNoiseAmp = readNoiseAmp.flatten()
-                cmod2u[cmod2u>readNoiseAmp*readNoiseAmpFraction] = (readNoiseAmp*readNoiseAmpFraction)[cmod2u>readNoiseAmp*readNoiseAmpFraction]
-                cmod2u[cmod2u<readNoiseAmp*-readNoiseAmpFraction] = (readNoiseAmp*-readNoiseAmpFraction)[cmod2u<readNoiseAmp*-readNoiseAmpFraction]
+                cmod2u[cmod2u > readNoiseAmp * readNoiseAmpFraction] = (
+                    readNoiseAmp * readNoiseAmpFraction
+                )[cmod2u > readNoiseAmp * readNoiseAmpFraction]
+                cmod2u[cmod2u < readNoiseAmp * -readNoiseAmpFraction] = (
+                    readNoiseAmp * -readNoiseAmpFraction
+                )[cmod2u < readNoiseAmp * -readNoiseAmpFraction]
                 cmod2u = cmod2u.reshape(imageIn.shape)
-                readNoiseAmp = readNoiseAmp.reshape(imageIn.shape)          
+                readNoiseAmp = readNoiseAmp.reshape(imageIn.shape)
             else:
-                cmod2u[cmod2u>readNoiseAmp*readNoiseAmpFraction] = readNoiseAmp*readNoiseAmpFraction
-                cmod2u[cmod2u<readNoiseAmp*-readNoiseAmpFraction] = readNoiseAmp*-readNoiseAmpFraction
-                
+                cmod2u[cmod2u > readNoiseAmp * readNoiseAmpFraction] = (
+                    readNoiseAmp * readNoiseAmpFraction
+                )
+                cmod2u[cmod2u < readNoiseAmp * -readNoiseAmpFraction] = (
+                    readNoiseAmp * -readNoiseAmpFraction
+                )
+
         readNoiseAmp2 = readNoiseAmp**2
-        w0 =     dval0 * dval0 / (dval0 * dval0 + 4.0 * readNoiseAmp2)
-        w9 =     dval9 * dval9 / (dval9 * dval9 + 18.0 * readNoiseAmp2)
+        w0 = dval0 * dval0 / (dval0 * dval0 + 4.0 * readNoiseAmp2)
+        w9 = dval9 * dval9 / (dval9 * dval9 + 18.0 * readNoiseAmp2)
         w1 = 4 * readNoiseAmp2 / (dmod1 * dmod1 + 4.0 * readNoiseAmp2)
         w2 = 4 * readNoiseAmp2 / (dmod2 * dmod2 + 4.0 * readNoiseAmp2)
         if self.smoothCol:
             wc1 = 4 * readNoiseAmp2 / (cmod1 * cmod1 + 4.0 * readNoiseAmp2)
-            wc2 = 4 * readNoiseAmp2 / (cmod2 * cmod2 + 4.0 * readNoiseAmp2)    
-            
+            wc2 = 4 * readNoiseAmp2 / (cmod2 * cmod2 + 4.0 * readNoiseAmp2)
+
         if self.smoothCol:
-            return  (dval0u * w0 / 6) + (dval9u * w9 / 6) +(dmod1u * w1 / 6) + (dmod2u * w2 / 6) +(cmod1u * wc1 / 6) + (cmod2u * wc2 / 6)
+            return (
+                (dval0u * w0 / 6)
+                + (dval9u * w9 / 6)
+                + (dmod1u * w1 / 6)
+                + (dmod2u * w2 / 6)
+                + (cmod1u * wc1 / 6)
+                + (cmod2u * wc2 / 6)
+            )
         else:
-            return  (dval0u * w0 * 0.25) + (dval9u * w9 * 0.25) +(dmod1u * w1 * 0.25) + (dmod2u * w2 * 0.25)
+            return (
+                (dval0u * w0 * 0.25)
+                + (dval9u * w9 * 0.25)
+                + (dmod1u * w1 * 0.25)
+                + (dmod2u * w2 * 0.25)
+            )
 
     ###############
     ###############
     def _create_initial_sim_images(
-            self,
-            background_level,
-            background_sigma,
-            image_size=500,
-            overwrite=False #figure out how to implement this (it fails currently)
+        self,
+        background_level,
+        background_sigma,
+        image_size=500,
+        overwrite=False,  # figure out how to implement this (it fails currently)
     ):
-        '''
+        """
         A subroutine to generate sky_background and readnoise frames for S+R simulations
 
         These components will create a baseline "clean" image (sky + readnoise) that we
         would expect to observe in the absence of CTI smearing effects
         in each simulated corner. Keeping this fixed will control random noise fluctuations
         ("simulation noise") when estimating covariances throughout the simulation.
 
         Note: This routine will be normally be called in <optimise_sr_fraction>
               rather than through direct user input
-        '''
+        """
 
-        #create sky frame    
-        skyFrame = np.random.normal(background_level, background_sigma, (image_size,image_size))
+        # create sky frame
+        skyFrame = np.random.normal(
+            background_level, background_sigma, (image_size, image_size)
+        )
         self.skyFrameSim = skyFrame
-            
-        #create readnoise_frame
-        noiseFrame = np.random.normal(0, self.sigmaRN, (image_size,image_size))
+
+        # create readnoise_frame
+        noiseFrame = np.random.normal(0, self.sigmaRN, (image_size, image_size))
         self.readnoiseFrameSim = noiseFrame
 
-        #generate covariance matrix from clean image
-        
+        # generate covariance matrix from clean image
+
+        return
 
-        return                                    
     ###############
-    ###############    
+    ###############
     def _estimate_residual_covariance(
-            self,
-            skyFrame,
-            noiseFrame,
-            sr_fraction,
-            matrix_size=5, #size of covariance grid, in pixels (also assumes square)
-            **kwargs
+        self,
+        skyFrame,
+        noiseFrame,
+        sr_fraction,
+        matrix_size=5,  # size of covariance grid, in pixels (also assumes square)
+        **kwargs
     ):
-        '''
+        """
         Estimate a covariance matrix for an optimising simulation, assuming the sky/noise frames have already been created
-        '''
-        #add CTI effects to skyFrame
-        ctiTrailedFrame = ac.add_cti(skyFrame,**kwargs)
-        #add read noise to CTI-trailed image
+        """
+        # add CTI effects to skyFrame
+        ctiTrailedFrame = ac.add_cti(skyFrame, **kwargs)
+        # add read noise to CTI-trailed image
         readNoiseAddedFrame = ctiTrailedFrame + noiseFrame
-        #do S+R routine
-        sFrame, rFrame = self.generate_SR_frames_from_image(readNoiseAddedFrame,sr_fraction)
+        # do S+R routine
+        sFrame, rFrame = self.generate_SR_frames_from_image(
+            readNoiseAddedFrame, sr_fraction
+        )
         ###rescale S+R correction to a fractional value (for optimization)
         ##sFrame+=rFrame
         ##rFrame*=sr_fraction
-        ##sFrame-=rFrame 
-        #clean CTI from S frame
-        ctiCorrectedFrame = ac.remove_cti(sFrame,1,**kwargs)
-        #re-add R frame to correction
+        ##sFrame-=rFrame
+        # clean CTI from S frame
+        ctiCorrectedFrame = ac.remove_cti(sFrame, 1, **kwargs)
+        # re-add R frame to correction
         outputFrame = ctiCorrectedFrame + rFrame
 
-        #determine covariance FOMs
-        fomSR = self.covariance_matrix_from_image(outputFrame,matrix_size=matrix_size)
-        fomBenchmark = self.covariance_matrix_from_image(skyFrame+noiseFrame,matrix_size=matrix_size)
+        # determine covariance FOMs
+        fomSR = self.covariance_matrix_from_image(outputFrame, matrix_size=matrix_size)
+        fomBenchmark = self.covariance_matrix_from_image(
+            skyFrame + noiseFrame, matrix_size=matrix_size
+        )
         fomDiff = fomSR - fomBenchmark
 
-        return fomSR,fomDiff
+        return fomSR, fomDiff
+
     ###############
     ###############
-    def _fitter_function(self,x,intercept,slope):
-        '''
+    def _fitter_function(self, x, intercept, slope):
+        """
         simple functional form to optimize a (linear) S+R fit using covariance matrix data
         passed to python optiser in optimise_SR_fraction, not needed by the user
-        '''
+        """
         y = intercept + slope * x
         return y
-    ###############        
+
+    ###############
     ###############
-    def figure_of_merit(self, covariance_matrix, fom_method='box',subgrid_size=None):
-        '''
+    def figure_of_merit(self, covariance_matrix, fom_method="box", subgrid_size=None):
+        """
         function for estimating the covariance figure of merit: the average value over some section of a covariance matrix
         if method == 'box' take a square region around the central pixel; 'row' is along the central row; column is along the central column
         if subgrid size is selected, use only an NxN subset of pixels in the matrix, starting from the center outward
-        '''
+        """
         xlen = covariance_matrix.shape[1]
         ylen = covariance_matrix.shape[0]
-        xcenter = xlen//2
-        ycenter = ylen//2
-        xstart,xend = 0,xlen
-        ystart,yend = 0,ylen
+        xcenter = xlen // 2
+        ycenter = ylen // 2
+        xstart, xend = 0, xlen
+        ystart, yend = 0, ylen
         if subgrid_size is not None:
-            xdiff = (xlen-subgrid_size)//2
-            ydiff = (ylen-subgrid_size)//2
-            xstart+=xdiff
-            xend-=xdiff
-            ystart+=ydiff
-            yend-=ydiff
-
-        covariance_matrix[ycenter,xcenter] = 0 #supress autocorrelation pixel    
-            
-        if fom_method == 'box':
-            result_mean = (np.sum(covariance_matrix[ystart:yend,xstart:xend]) - covariance_matrix[ycenter,xcenter])/8   #average over central box
-        if fom_method == 'row':
-            result_mean = (np.sum(covariance_matrix[ycenter,xstart:xend]) - covariance_matrix[ycenter,xcenter])/4  #average over central row (for serial CTI)
-        if fom_method == 'column':
-            result_mean = (np.sum(covariance_matrix[ystart:yend,xcenter]) - covariance_matrix[ycenter,xcenter])/4  #sum over central column (for parallel CTI)
-        #raise NotImplementedError
+            xdiff = (xlen - subgrid_size) // 2
+            ydiff = (ylen - subgrid_size) // 2
+            xstart += xdiff
+            xend -= xdiff
+            ystart += ydiff
+            yend -= ydiff
+
+        covariance_matrix[ycenter, xcenter] = 0  # supress autocorrelation pixel
+
+        if fom_method == "box":
+            result_mean = (
+                np.sum(covariance_matrix[ystart:yend, xstart:xend])
+                - covariance_matrix[ycenter, xcenter]
+            ) / 8  # average over central box
+        if fom_method == "row":
+            result_mean = (
+                np.sum(covariance_matrix[ycenter, xstart:xend])
+                - covariance_matrix[ycenter, xcenter]
+            ) / 4  # average over central row (for serial CTI)
+        if fom_method == "column":
+            result_mean = (
+                np.sum(covariance_matrix[ystart:yend, xcenter])
+                - covariance_matrix[ycenter, xcenter]
+            ) / 4  # sum over central column (for parallel CTI)
+        # raise NotImplementedError
         return result_mean
+
     ###############
     ###############
-    def covariance_matrix_from_image(self, image, matrix_size=5,fprSize=5):
-
-        matRange= matrix_size//2 #set positions of correlation pixels and set limits to remove "roll-over" region
-        
-        covariance_matrix = np.zeros((matrix_size,matrix_size))
-        #calcluate mean stats on image
-        image2 = image[fprSize:,fprSize:] #remove FPR decrement
-        x = image2[matRange:-matRange,matRange:-matRange].flatten() #remove possible roll-over region
+    def covariance_matrix_from_image(self, image, matrix_size=5, fprSize=5):
+        matRange = (
+            matrix_size // 2
+        )  # set positions of correlation pixels and set limits to remove "roll-over" region
+
+        covariance_matrix = np.zeros((matrix_size, matrix_size))
+        # calcluate mean stats on image
+        image2 = image[fprSize:, fprSize:]  # remove FPR decrement
+        x = image2[
+            matRange:-matRange, matRange:-matRange
+        ].flatten()  # remove possible roll-over region
         xbar = np.mean(x)
 
-        #roll image to get cross correlation
-        for i in range(-matRange,matRange+1,1):
-            for j in range(-matRange,matRange+1,1):
-                y = np.roll(image2,(-j,-i),axis=(0,1))[2:-2,2:-2].flatten()
+        # roll image to get cross correlation
+        for i in range(-matRange, matRange + 1, 1):
+            for j in range(-matRange, matRange + 1, 1):
+                y = np.roll(image2, (-j, -i), axis=(0, 1))[2:-2, 2:-2].flatten()
                 ybar = np.mean(y)
 
-                #calculate covariance
-                covar = np.sum((x-xbar)*(y-ybar))/x.size #/(np.std(x-xbar)*np.std(y-ybar))/(x.size) #removing noise-level normalization
-                #covar = np.sum((x-xbar)*(y-ybar))/(np.std(x-xbar)*np.std(y-ybar))/(x.size)
-                #populate matrix cells
-                covariance_matrix[i+matRange,j+matRange] = covar
-        #covariance_matrix[matRange,matRange] = 0 #switch this normalization to plotting
-                
-        return covariance_matrix
-    ###############
+                # calculate covariance
+                covar = (
+                    np.sum((x - xbar) * (y - ybar)) / x.size
+                )  # /(np.std(x-xbar)*np.std(y-ybar))/(x.size) #removing noise-level normalization
+                # covar = np.sum((x-xbar)*(y-ybar))/(np.std(x-xbar)*np.std(y-ybar))/(x.size)
+                # populate matrix cells
+                covariance_matrix[i + matRange, j + matRange] = covar
+        # covariance_matrix[matRange,matRange] = 0 #switch this normalization to plotting
 
+        return covariance_matrix
 
+    ###############
 
-    
     ###############
     #
     # FUNCTIONS TO BE REFORMATTED / RETHOUGHT? (WORK IN PROGRESS)
     #
     ###############
     def measure_simulated_covariance_corners(
-            self,
-            n_pixels=None,    #the size of the entire CCD over which the procedure will be run
-            subchip_size=500, #size of the cutout region, to test CTI behaviour (a subset of pixels far form the readout)  
-            matrix_size=5,    #covariance matrix size (NxN array)
-            fom_method='box',
-            **kwargs
+        self,
+        n_pixels=None,  # the size of the entire CCD over which the procedure will be run
+        subchip_size=500,  # size of the cutout region, to test CTI behaviour (a subset of pixels far form the readout)
+        matrix_size=5,  # covariance matrix size (NxN array)
+        fom_method="box",
+        **kwargs
     ):
-        '''
+        """
         Apply optimised S+R correction to the four corners of the CCD (close to readout, far from parallel register, far from serial register, far from both)
         and estimate a covariance matrix for each corner. These matrices can be used to correct any residual covariance in weak lensing shapes.
-        '''
+        """
+
+        # update any keyword arguments
+        allKwargs = kwargs | self.arcKwargs
 
-        #update any keyword arguments
-        allKwargs = kwargs|self.arcKwargs
-        
-        frac_opt = self.SRfrac_optimised #self.optVals['optSRfrac'] #set the optimized S+R fraction
+        frac_opt = (
+            self.SRfrac_optimised
+        )  # self.optVals['optSRfrac'] #set the optimized S+R fraction
         if frac_opt == None:
             frac_opt = 1.0
 
         if type(n_pixels) == int:
-            n_pixels=(n_pixels,n_pixels)
+            n_pixels = (n_pixels, n_pixels)
         chip_size = n_pixels
-        
+
         ##set prescan regions (this simulates the maximum possible CTI trailing, averaged at the far edge of the real CCD)
-        #if 'parallel_roe' in allKwargs:
+        # if 'parallel_roe' in allKwargs:
         #    kwargs['parallel_roe'].prescan_offset = n_pixels[0]+(subchip_size//2)
-        #if 'serial_roe' in allKwargs:
+        # if 'serial_roe' in allKwargs:
         #    kwargs['serial_roe'].prescan_offset = n_pixels[1]+(subchip_size//2)
-        
-        #re-run the S+R routine with the optimised level
-        raw_matrix_opt,correction_matrix_opt = self._estimate_residual_covariance(self.skyFrameSim,self.readnoiseFrameSim,frac_opt,matrix_size=matrix_size,**self.arcKwargs,**kwargs)
-        raw_matrix_opt_noSR,correction_matrix_opt_noSR = self._estimate_residual_covariance(self.skyFrameSim,self.readnoiseFrameSim,0,matrix_size=matrix_size,**self.arcKwargs,**kwargs) #this is dumb...do it better
-
-        #run a second S+R routine in the region close to the readout registers, to identify/remove stochastic simulation noise
-        kwargs_noCTI = kwargs|self.arcKwargs
-        kwargs_noCTI['parallel_traps']=None 
-        kwargs_noCTI['serial_traps']=None
-        #effectively, we are removing the effects of CTI, but still calculating a covariance matrix
-        raw_matrix_opt_noCTI,correction_matrix_opt_noCTI = self._estimate_residual_covariance(self.skyFrameSim,self.readnoiseFrameSim,frac_opt,matrix_size=matrix_size,**kwargs_noCTI)
-        raw_matrix_opt_noCTI_noSR,correction_matrix_opt_noCTI_noSR = self._estimate_residual_covariance(self.skyFrameSim,self.readnoiseFrameSim,0,matrix_size=matrix_size,**kwargs_noCTI)
-
-        #create the "benchmark" covariance matrix: a purely non-correlated array with the central pixel equal to (readnoise_sigma**2 + background_sigma**2)
-        #Any difference between this and "raw_matrix_opt_noCTI" is the simulation noise, and can be eliminated
-        benchmark_matrix = raw_matrix_opt_noCTI*0
-        centrePix = matrix_size//2
-        benchmark_matrix[centrePix,centrePix] = self.sigmaRN**2 + self.sigmaSky**2
-        #calculate the simulation-noise residual
+
+        # re-run the S+R routine with the optimised level
+        raw_matrix_opt, correction_matrix_opt = self._estimate_residual_covariance(
+            self.skyFrameSim,
+            self.readnoiseFrameSim,
+            frac_opt,
+            matrix_size=matrix_size,
+            **self.arcKwargs,
+            **kwargs
+        )
+        (
+            raw_matrix_opt_noSR,
+            correction_matrix_opt_noSR,
+        ) = self._estimate_residual_covariance(
+            self.skyFrameSim,
+            self.readnoiseFrameSim,
+            0,
+            matrix_size=matrix_size,
+            **self.arcKwargs,
+            **kwargs
+        )  # this is dumb...do it better
+
+        # run a second S+R routine in the region close to the readout registers, to identify/remove stochastic simulation noise
+        kwargs_noCTI = kwargs | self.arcKwargs
+        kwargs_noCTI["parallel_traps"] = None
+        kwargs_noCTI["serial_traps"] = None
+        # effectively, we are removing the effects of CTI, but still calculating a covariance matrix
+        (
+            raw_matrix_opt_noCTI,
+            correction_matrix_opt_noCTI,
+        ) = self._estimate_residual_covariance(
+            self.skyFrameSim,
+            self.readnoiseFrameSim,
+            frac_opt,
+            matrix_size=matrix_size,
+            **kwargs_noCTI
+        )
+        (
+            raw_matrix_opt_noCTI_noSR,
+            correction_matrix_opt_noCTI_noSR,
+        ) = self._estimate_residual_covariance(
+            self.skyFrameSim,
+            self.readnoiseFrameSim,
+            0,
+            matrix_size=matrix_size,
+            **kwargs_noCTI
+        )
+
+        # create the "benchmark" covariance matrix: a purely non-correlated array with the central pixel equal to (readnoise_sigma**2 + background_sigma**2)
+        # Any difference between this and "raw_matrix_opt_noCTI" is the simulation noise, and can be eliminated
+        benchmark_matrix = raw_matrix_opt_noCTI * 0
+        centrePix = matrix_size // 2
+        benchmark_matrix[centrePix, centrePix] = self.sigmaRN**2 + self.sigmaSky**2
+        # calculate the simulation-noise residual
         residual_benchmark_matrix = raw_matrix_opt_noCTI - benchmark_matrix
 
-        #Finally, if both parallel and serial CTI are present, calculate covariances of the "cross-region" chip corners (far from serial readout but close to parallel readout, and vice-versa)
-        if ('parallel_traps' in allKwargs)&('serial_traps' in allKwargs):
-            if (allKwargs['parallel_traps'] is not None)&(allKwargs['serial_traps'] is not None):
-                kwargs_parallelOnly = kwargs|self.arcKwargs
-                kwargs_parallelOnly['serial_traps']=None #make a parallel-only corner
-                kwargs_serialOnly = kwargs|self.arcKwargs
-                kwargs_serialOnly['parallel_traps']=None #make a serial-only corner
-
-                raw_matrix_opt_parallel,correction_matrix_opt_parallel = self._estimate_residual_covariance(self.skyFrameSim,self.readnoiseFrameSim,frac_opt,matrix_size=matrix_size,**kwargs_parallelOnly)
-                raw_matrix_opt_serial,correction_matrix_opt_serial = self._estimate_residual_covariance(self.skyFrameSim,self.readnoiseFrameSim,frac_opt,matrix_size=matrix_size,**kwargs_serialOnly)
-                raw_matrix_opt_parallel_noSR,correction_matrix_opt_parallel_noSR = self._estimate_residual_covariance(self.skyFrameSim,self.readnoiseFrameSim,0,matrix_size=matrix_size,**kwargs_parallelOnly)
-                raw_matrix_opt_serial_noSR,correction_matrix_opt_serial_noSR = self._estimate_residual_covariance(self.skyFrameSim,self.readnoiseFrameSim,0,matrix_size=matrix_size,**kwargs_serialOnly)
-
-                #package all relevant quantities into optVals and return
-                self.optVals['combinedQuadMatrix'] = raw_matrix_opt
-                self.optVals['combinedQuadMatrix_diff'] = correction_matrix_opt
-                self.optVals['combinedQuadMatrix_noSR'] = raw_matrix_opt_noSR
-                self.optVals['combinedQuadMatrix_noSR_diff'] = correction_matrix_opt_noSR
-                self.optVals['parallelQuadMatrix'] = raw_matrix_opt_parallel
-                self.optVals['parallelQuadMatrix_diff'] = correction_matrix_opt_parallel
-                self.optVals['parallelQuadMatrix_noSR'] = raw_matrix_opt_parallel_noSR
-                self.optVals['parallelQuadMatrix_noSR_diff'] = correction_matrix_opt_parallel_noSR
-                self.optVals['serialQuadMatrix'] = raw_matrix_opt_serial
-                self.optVals['serialQuadMatrix_diff'] = correction_matrix_opt_serial
-                self.optVals['serialQuadMatrix_noSR'] = raw_matrix_opt_serial_noSR
-                self.optVals['serialQuadMatrix_noSR_diff'] = correction_matrix_opt_serial_noSR
-                self.optVals['noCTIQuadMatrix'] = raw_matrix_opt_noCTI
-                self.optVals['noCTIQuadMatrix_diff'] = correction_matrix_opt_noCTI
-                self.optVals['noCTIQuadMatrix_noSR'] = raw_matrix_opt_noCTI
-                self.optVals['noCTIQuadMatrix_diff_noSR'] = correction_matrix_opt_noCTI
-                self.optVals['benchmark'] = benchmark_matrix
-                self.optVals['benchmark_resid'] = residual_benchmark_matrix
-    ###############    
+        # Finally, if both parallel and serial CTI are present, calculate covariances of the "cross-region" chip corners (far from serial readout but close to parallel readout, and vice-versa)
+        if ("parallel_traps" in allKwargs) & ("serial_traps" in allKwargs):
+            if (allKwargs["parallel_traps"] is not None) & (
+                allKwargs["serial_traps"] is not None
+            ):
+                kwargs_parallelOnly = kwargs | self.arcKwargs
+                kwargs_parallelOnly[
+                    "serial_traps"
+                ] = None  # make a parallel-only corner
+                kwargs_serialOnly = kwargs | self.arcKwargs
+                kwargs_serialOnly["parallel_traps"] = None  # make a serial-only corner
+
+                (
+                    raw_matrix_opt_parallel,
+                    correction_matrix_opt_parallel,
+                ) = self._estimate_residual_covariance(
+                    self.skyFrameSim,
+                    self.readnoiseFrameSim,
+                    frac_opt,
+                    matrix_size=matrix_size,
+                    **kwargs_parallelOnly
+                )
+                (
+                    raw_matrix_opt_serial,
+                    correction_matrix_opt_serial,
+                ) = self._estimate_residual_covariance(
+                    self.skyFrameSim,
+                    self.readnoiseFrameSim,
+                    frac_opt,
+                    matrix_size=matrix_size,
+                    **kwargs_serialOnly
+                )
+                (
+                    raw_matrix_opt_parallel_noSR,
+                    correction_matrix_opt_parallel_noSR,
+                ) = self._estimate_residual_covariance(
+                    self.skyFrameSim,
+                    self.readnoiseFrameSim,
+                    0,
+                    matrix_size=matrix_size,
+                    **kwargs_parallelOnly
+                )
+                (
+                    raw_matrix_opt_serial_noSR,
+                    correction_matrix_opt_serial_noSR,
+                ) = self._estimate_residual_covariance(
+                    self.skyFrameSim,
+                    self.readnoiseFrameSim,
+                    0,
+                    matrix_size=matrix_size,
+                    **kwargs_serialOnly
+                )
+
+                # package all relevant quantities into optVals and return
+                self.optVals["combinedQuadMatrix"] = raw_matrix_opt
+                self.optVals["combinedQuadMatrix_diff"] = correction_matrix_opt
+                self.optVals["combinedQuadMatrix_noSR"] = raw_matrix_opt_noSR
+                self.optVals[
+                    "combinedQuadMatrix_noSR_diff"
+                ] = correction_matrix_opt_noSR
+                self.optVals["parallelQuadMatrix"] = raw_matrix_opt_parallel
+                self.optVals["parallelQuadMatrix_diff"] = correction_matrix_opt_parallel
+                self.optVals["parallelQuadMatrix_noSR"] = raw_matrix_opt_parallel_noSR
+                self.optVals[
+                    "parallelQuadMatrix_noSR_diff"
+                ] = correction_matrix_opt_parallel_noSR
+                self.optVals["serialQuadMatrix"] = raw_matrix_opt_serial
+                self.optVals["serialQuadMatrix_diff"] = correction_matrix_opt_serial
+                self.optVals["serialQuadMatrix_noSR"] = raw_matrix_opt_serial_noSR
+                self.optVals[
+                    "serialQuadMatrix_noSR_diff"
+                ] = correction_matrix_opt_serial_noSR
+                self.optVals["noCTIQuadMatrix"] = raw_matrix_opt_noCTI
+                self.optVals["noCTIQuadMatrix_diff"] = correction_matrix_opt_noCTI
+                self.optVals["noCTIQuadMatrix_noSR"] = raw_matrix_opt_noCTI
+                self.optVals["noCTIQuadMatrix_diff_noSR"] = correction_matrix_opt_noCTI
+                self.optVals["benchmark"] = benchmark_matrix
+                self.optVals["benchmark_resid"] = residual_benchmark_matrix
+
+    ###############
```

### Comparing `arcticpy-2.2/python/arcticpy/roe.py` & `arcticpy-2.3/python/arcticpy/roe.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 
-#from .dictable import Dictable
+# from .dictable import Dictable
 
 roe_type_standard = 0
 roe_type_charge_injection = 1
 roe_type_trap_pumping = 2
 
 
 class ROE:
@@ -13,68 +13,66 @@
         dwell_times=[1.0],
         prescan_offset=0,
         overscan_start=-1,
         empty_traps_between_columns=True,
         empty_traps_for_first_transfers=False,
         force_release_away_from_readout=True,
         use_integer_express_matrix=False,
-        pixel_bounce_kA=0.,
-        pixel_bounce_kv=0.,
-        pixel_bounce_omega=1.,
-        pixel_bounce_gamma=1.
+        pixel_bounce_kA=0.0,
+        pixel_bounce_kv=0.0,
+        pixel_bounce_omega=1.0,
+        pixel_bounce_gamma=1.0,
     ):
         self.dwell_times = np.array(dwell_times, dtype=np.double)
         self.prescan_offset = prescan_offset
         self.overscan_start = overscan_start
         self.empty_traps_between_columns = empty_traps_between_columns
         self.empty_traps_for_first_transfers = empty_traps_for_first_transfers
         self.force_release_away_from_readout = force_release_away_from_readout
         self.use_integer_express_matrix = use_integer_express_matrix
-        self.pixel_bounce_kA    = pixel_bounce_kA
-        self.pixel_bounce_kv    = pixel_bounce_kv
+        self.pixel_bounce_kA = pixel_bounce_kA
+        self.pixel_bounce_kv = pixel_bounce_kv
         self.pixel_bounce_omega = pixel_bounce_omega
         self.pixel_bounce_gamma = pixel_bounce_gamma
         self.n_pumps = -1  # Dummy value
 
         self.type = roe_type_standard
-    
 
 
 class ROEChargeInjection(ROE):
     def __init__(
         self,
         dwell_times=[1.0],
         prescan_offset=0,
         overscan_start=-1,
         empty_traps_between_columns=True,
         force_release_away_from_readout=True,
         use_integer_express_matrix=False,
-        pixel_bounce_kA=0.,
-        pixel_bounce_kv=0.,
-        pixel_bounce_omega=1.,
-        pixel_bounce_gamma=1.
-        
+        pixel_bounce_kA=0.0,
+        pixel_bounce_kv=0.0,
+        pixel_bounce_omega=1.0,
+        pixel_bounce_gamma=1.0,
     ):
         ROE.__init__(
             self,
             dwell_times=dwell_times,
             prescan_offset=prescan_offset,
             overscan_start=overscan_start,
             empty_traps_between_columns=empty_traps_between_columns,
             empty_traps_for_first_transfers=False,
             force_release_away_from_readout=force_release_away_from_readout,
             use_integer_express_matrix=use_integer_express_matrix,
             pixel_bounce_kA=pixel_bounce_kA,
             pixel_bounce_kv=pixel_bounce_kv,
             pixel_bounce_omega=pixel_bounce_omega,
-            pixel_bounce_gamma=pixel_bounce_gamma
+            pixel_bounce_gamma=pixel_bounce_gamma,
         )
 
         self.type = roe_type_charge_injection
-    
+
     def from_normal_roe(roe, n_pixels_in_image):
         """
         Convert a normal ROE sequence, with all its options, to one modelling
         charge injection readout.
         Must specify the number of physical pixels between the charge injection
         register and the readout node.
         """
@@ -84,42 +82,42 @@
             overscan_start=roe.overscan_start,
             empty_traps_between_columns=roe.empty_traps_between_columns,
             force_release_away_from_readout=roe.force_release_away_from_readout,
             use_integer_express_matrix=roe.use_integer_express_matrix,
             pixel_bounce_kA=roe.pixel_bounce_kA,
             pixel_bounce_kv=roe.pixel_bounce_kv,
             pixel_bounce_omega=roe.pixel_bounce_omega,
-            pixel_bounce_gamma=roe.pixel_bounce_gamma
+            pixel_bounce_gamma=roe.pixel_bounce_gamma,
         )
 
 
 class ROETrapPumping(ROE):
     def __init__(
         self,
         dwell_times=[0.5, 0.5],
         prescan_offset=0,
         overscan_start=-1,
         n_pumps=1,
         empty_traps_for_first_transfers=False,
         use_integer_express_matrix=False,
-        pixel_bounce_kA=0.,
-        pixel_bounce_kv=0.,
-        pixel_bounce_omega=1.,
-        pixel_bounce_gamma=1.
-     ):
+        pixel_bounce_kA=0.0,
+        pixel_bounce_kv=0.0,
+        pixel_bounce_omega=1.0,
+        pixel_bounce_gamma=1.0,
+    ):
         ROE.__init__(
             self,
             dwell_times=dwell_times,
             prescan_offset=prescan_offset,
             overscan_start=overscan_start,
             empty_traps_between_columns=True,
             empty_traps_for_first_transfers=empty_traps_for_first_transfers,
             force_release_away_from_readout=False,
             use_integer_express_matrix=use_integer_express_matrix,
             pixel_bounce_kA=pixel_bounce_kA,
             pixel_bounce_kv=pixel_bounce_kv,
             pixel_bounce_omega=pixel_bounce_omega,
-            pixel_bounce_gamma=pixel_bounce_gamma
+            pixel_bounce_gamma=pixel_bounce_gamma,
         )
         self.n_pumps = n_pumps
 
         self.type = roe_type_trap_pumping
```

### Comparing `arcticpy-2.2/python/arcticpy/src/interface.cpp` & `arcticpy-2.3/python/arcticpy/src/interface.cpp`

 * *Files identical despite different names*

### Comparing `arcticpy-2.2/python/arcticpy/traps.py` & `arcticpy-2.3/python/arcticpy/traps.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,69 +1,75 @@
 import numpy as np
 
 from autoconf.dictable import Dictable
 
+
 class AbstractTrap(Dictable):
     def __init__(self, density=1.0, release_timescale=1.0):
         self.density = density
         self.release_timescale = release_timescale
 
     @property
     def delta_ellipticity(self):
         raise NotImplementedError
 
+
 class TrapInstantCapture(AbstractTrap):
     def __init__(
         self,
-        density:float=1.0,
+        density: float = 1.0,
         release_timescale=1.0,
         fractional_volume_none_exposed=0.0,
         fractional_volume_full_exposed=0.0,
     ):
         super().__init__(density, release_timescale)
 
         self.fractional_volume_none_exposed = fractional_volume_none_exposed
         self.fractional_volume_full_exposed = fractional_volume_full_exposed
 
     @property
     def delta_ellipticity(self):
-
         a = 0.05333
         d_a = -0.03357
         d_p = 1.628
         d_w = 0.2951
         g_a = 0.09901
         g_p = 0.4553
         g_w = 0.4132
 
-        return 4.0 * self.density * (
-            a
-            + d_a * (np.arctan((np.log10(self.release_timescale) - d_p) / d_w))
-            + (
-                g_a
-                * np.exp(
-                    -((np.log10(self.release_timescale) - g_p) ** 2.0) / (2 * g_w ** 2.0)
+        return (
+            4.0
+            * self.density
+            * (
+                a
+                + d_a * (np.arctan((np.log10(self.release_timescale) - d_p) / d_w))
+                + (
+                    g_a
+                    * np.exp(
+                        -((np.log10(self.release_timescale) - g_p) ** 2.0)
+                        / (2 * g_w**2.0)
+                    )
                 )
             )
         )
 
     def poisson_density_from(self, total_pixels, seed=-1):
-
         if seed == -1:
-            seed = np.random.randint(
-                0, int(1e9)
-            )
+            seed = np.random.randint(0, int(1e9))
 
         np.random.seed(seed)
 
         density_pixels = self.density * total_pixels
         poisson_density_pixels = np.random.poisson(density_pixels)
         poisson_density_per_pixel = poisson_density_pixels / total_pixels
 
-        return TrapInstantCapture(density=poisson_density_per_pixel, release_timescale=self.release_timescale)
+        return TrapInstantCapture(
+            density=poisson_density_per_pixel, release_timescale=self.release_timescale
+        )
+
 
 class TrapSlowCapture(AbstractTrap):
     def __init__(self, density=1.0, release_timescale=1.0, capture_timescale=0.0):
         super().__init__(density, release_timescale)
 
         self.capture_timescale = capture_timescale
```

### Comparing `arcticpy-2.2/python/arcticpy/wrapper.cpp` & `arcticpy-2.3/python/arcticpy/wrapper.cpp`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.32 */
+/* Generated by Cython 3.0.0 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "define_macros": [
             [
                 "NPY_NO_DEPRECATED_API",
@@ -51,28 +51,40 @@
     "module_name": "arcticpy.wrapper"
 }
 END: Cython Metadata */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
+#if defined(CYTHON_LIMITED_API) && 0
+  #ifndef Py_LIMITED_API
+    #if CYTHON_LIMITED_API+0 > 0x03030000
+      #define Py_LIMITED_API CYTHON_LIMITED_API
+    #else
+      #define Py_LIMITED_API 0x03030000
+    #endif
+  #endif
+#endif
+
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
-#elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
-    #error Cython requires Python 2.6+ or Python 3.3+.
+#elif PY_VERSION_HEX < 0x02070000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
+    #error Cython requires Python 2.7+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_32"
-#define CYTHON_HEX_VERSION 0x001D20F0
+#define CYTHON_ABI "3_0_0"
+#define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
+#define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
+#define CYTHON_HEX_VERSION 0x030000F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
-#if !defined(WIN32) && !defined(MS_WINDOWS)
+#if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
     #define __stdcall
   #endif
   #ifndef __cdecl
     #define __cdecl
   #endif
   #ifndef __fastcall
@@ -83,31 +95,34 @@
   #define DL_IMPORT(t) t
 #endif
 #ifndef DL_EXPORT
   #define DL_EXPORT(t) t
 #endif
 #define __PYX_COMMA ,
 #ifndef HAVE_LONG_LONG
-  #if PY_VERSION_HEX >= 0x02070000
-    #define HAVE_LONG_LONG
-  #endif
+  #define HAVE_LONG_LONG
 #endif
 #ifndef PY_LONG_LONG
   #define PY_LONG_LONG LONG_LONG
 #endif
 #ifndef Py_HUGE_VAL
   #define Py_HUGE_VAL HUGE_VAL
 #endif
-#ifdef PYPY_VERSION
-  #define CYTHON_COMPILING_IN_PYPY 1
-  #define CYTHON_COMPILING_IN_PYSTON 0
+#if defined(GRAALVM_PYTHON)
+  /* For very preliminary testing purposes. Most variables are set the same as PyPy.
+     The existence of this section does not imply that anything works or is even tested */
+  #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_LIMITED_API 0
+  #define CYTHON_COMPILING_IN_GRAAL 1
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
   #define CYTHON_USE_TYPE_SLOTS 0
+  #undef CYTHON_USE_TYPE_SPECS
+  #define CYTHON_USE_TYPE_SPECS 0
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #if PY_VERSION_HEX < 0x03050000
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
@@ -124,76 +139,158 @@
   #define CYTHON_AVOID_BORROWED_REFS 1
   #undef CYTHON_ASSUME_SAFE_MACROS
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #undef CYTHON_METH_FASTCALL
+  #define CYTHON_METH_FASTCALL 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS (PY_MAJOR_VERSION >= 3)
+  #endif
   #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #undef CYTHON_USE_MODULE_STATE
+  #define CYTHON_USE_MODULE_STATE 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
-#elif defined(PYSTON_VERSION)
-  #define CYTHON_COMPILING_IN_PYPY 0
-  #define CYTHON_COMPILING_IN_PYSTON 1
+#elif defined(PYPY_VERSION)
+  #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_LIMITED_API 0
+  #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
-  #ifndef CYTHON_USE_TYPE_SLOTS
-    #define CYTHON_USE_TYPE_SLOTS 1
+  #undef CYTHON_USE_TYPE_SLOTS
+  #define CYTHON_USE_TYPE_SLOTS 0
+  #undef CYTHON_USE_TYPE_SPECS
+  #define CYTHON_USE_TYPE_SPECS 0
+  #undef CYTHON_USE_PYTYPE_LOOKUP
+  #define CYTHON_USE_PYTYPE_LOOKUP 0
+  #if PY_VERSION_HEX < 0x03050000
+    #undef CYTHON_USE_ASYNC_SLOTS
+    #define CYTHON_USE_ASYNC_SLOTS 0
+  #elif !defined(CYTHON_USE_ASYNC_SLOTS)
+    #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #undef CYTHON_USE_PYLIST_INTERNALS
+  #define CYTHON_USE_PYLIST_INTERNALS 0
+  #undef CYTHON_USE_UNICODE_INTERNALS
+  #define CYTHON_USE_UNICODE_INTERNALS 0
+  #undef CYTHON_USE_UNICODE_WRITER
+  #define CYTHON_USE_UNICODE_WRITER 0
+  #undef CYTHON_USE_PYLONG_INTERNALS
+  #define CYTHON_USE_PYLONG_INTERNALS 0
+  #undef CYTHON_AVOID_BORROWED_REFS
+  #define CYTHON_AVOID_BORROWED_REFS 1
+  #undef CYTHON_ASSUME_SAFE_MACROS
+  #define CYTHON_ASSUME_SAFE_MACROS 0
+  #undef CYTHON_UNPACK_METHODS
+  #define CYTHON_UNPACK_METHODS 0
+  #undef CYTHON_FAST_THREAD_STATE
+  #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #undef CYTHON_METH_FASTCALL
+  #define CYTHON_METH_FASTCALL 0
+  #undef CYTHON_FAST_PYCALL
+  #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS (PY_MAJOR_VERSION >= 3)
+  #endif
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
+  #undef CYTHON_USE_MODULE_STATE
+  #define CYTHON_USE_MODULE_STATE 0
+  #undef CYTHON_USE_TP_FINALIZE
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
+  #undef CYTHON_USE_DICT_VERSIONS
+  #define CYTHON_USE_DICT_VERSIONS 0
+  #undef CYTHON_USE_EXC_INFO_STACK
+  #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
+#elif defined(CYTHON_LIMITED_API)
+  #define CYTHON_COMPILING_IN_PYPY 0
+  #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_LIMITED_API 1
+  #define CYTHON_COMPILING_IN_GRAAL 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
+  #undef CYTHON_CLINE_IN_TRACEBACK
+  #define CYTHON_CLINE_IN_TRACEBACK 0
+  #undef CYTHON_USE_TYPE_SLOTS
+  #define CYTHON_USE_TYPE_SLOTS 0
+  #undef CYTHON_USE_TYPE_SPECS
+  #define CYTHON_USE_TYPE_SPECS 1
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #undef CYTHON_USE_ASYNC_SLOTS
   #define CYTHON_USE_ASYNC_SLOTS 0
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
-  #ifndef CYTHON_USE_UNICODE_INTERNALS
-    #define CYTHON_USE_UNICODE_INTERNALS 1
+  #undef CYTHON_USE_UNICODE_INTERNALS
+  #define CYTHON_USE_UNICODE_INTERNALS 0
+  #ifndef CYTHON_USE_UNICODE_WRITER
+    #define CYTHON_USE_UNICODE_WRITER 0
   #endif
-  #undef CYTHON_USE_UNICODE_WRITER
-  #define CYTHON_USE_UNICODE_WRITER 0
   #undef CYTHON_USE_PYLONG_INTERNALS
   #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
-  #ifndef CYTHON_ASSUME_SAFE_MACROS
-    #define CYTHON_ASSUME_SAFE_MACROS 1
-  #endif
-  #ifndef CYTHON_UNPACK_METHODS
-    #define CYTHON_UNPACK_METHODS 1
-  #endif
+  #undef CYTHON_ASSUME_SAFE_MACROS
+  #define CYTHON_ASSUME_SAFE_MACROS 0
+  #undef CYTHON_UNPACK_METHODS
+  #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #undef CYTHON_METH_FASTCALL
+  #define CYTHON_METH_FASTCALL 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #undef CYTHON_PEP489_MULTI_PHASE_INIT
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
-  #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #undef CYTHON_USE_MODULE_STATE
+  #define CYTHON_USE_MODULE_STATE 1
+  #ifndef CYTHON_USE_TP_FINALIZE
+    #define CYTHON_USE_TP_FINALIZE 1
+  #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
 #elif defined(PY_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
-  #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_LIMITED_API 0
+  #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
@@ -229,36 +326,34 @@
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
-  #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
+  #define CYTHON_COMPILING_IN_LIMITED_API 0
+  #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
-  #if PY_VERSION_HEX < 0x02070000
-    #undef CYTHON_USE_PYTYPE_LOOKUP
-    #define CYTHON_USE_PYTYPE_LOOKUP 0
-  #elif !defined(CYTHON_USE_PYTYPE_LOOKUP)
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
+  #ifndef CYTHON_USE_PYTYPE_LOOKUP
     #define CYTHON_USE_PYTYPE_LOOKUP 1
   #endif
   #if PY_MAJOR_VERSION < 3
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
-  #if PY_VERSION_HEX < 0x02070000
-    #undef CYTHON_USE_PYLONG_INTERNALS
-    #define CYTHON_USE_PYLONG_INTERNALS 0
-  #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
@@ -274,45 +369,67 @@
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
-  #if PY_VERSION_HEX >= 0x030B00A4
-    #undef CYTHON_FAST_THREAD_STATE
-    #define CYTHON_FAST_THREAD_STATE 0
-  #elif !defined(CYTHON_FAST_THREAD_STATE)
+  #ifndef CYTHON_FAST_THREAD_STATE
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
+  #ifndef CYTHON_FAST_GIL
+    #define CYTHON_FAST_GIL (PY_MAJOR_VERSION < 3 || PY_VERSION_HEX >= 0x03060000 && PY_VERSION_HEX < 0x030C00A6)
+  #endif
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL (PY_VERSION_HEX >= 0x030700A1)
+  #endif
   #ifndef CYTHON_FAST_PYCALL
-    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030A0000)
+    #define CYTHON_FAST_PYCALL 1
   #endif
-  #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
-    #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
   #endif
-  #ifndef CYTHON_USE_TP_FINALIZE
-    #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
+  #if PY_VERSION_HEX < 0x03050000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
   #endif
-  #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+  #if PY_VERSION_HEX < 0x030400a1
+    #undef CYTHON_USE_TP_FINALIZE
+    #define CYTHON_USE_TP_FINALIZE 0
+  #elif !defined(CYTHON_USE_TP_FINALIZE)
+    #define CYTHON_USE_TP_FINALIZE 1
+  #endif
+  #if PY_VERSION_HEX < 0x030600B1
+    #undef CYTHON_USE_DICT_VERSIONS
+    #define CYTHON_USE_DICT_VERSIONS 0
+  #elif !defined(CYTHON_USE_DICT_VERSIONS)
+    #define CYTHON_USE_DICT_VERSIONS  (PY_VERSION_HEX < 0x030C00A5)
   #endif
-  #if PY_VERSION_HEX >= 0x030B00A4
+  #if PY_VERSION_HEX < 0x030700A3
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
-    #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
+    #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
+#if !defined(CYTHON_VECTORCALL)
+#define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
+#endif
+#define CYTHON_BACKPORT_VECTORCALL (CYTHON_METH_FASTCALL && PY_VERSION_HEX < 0x030800B1)
 #if CYTHON_USE_PYLONG_INTERNALS
   #if PY_MAJOR_VERSION < 3
     #include "longintrepr.h"
   #endif
   #undef SHIFT
   #undef BASE
   #undef MASK
@@ -334,78 +451,128 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_RESTRICT restrict
   #else
     #define CYTHON_RESTRICT
   #endif
 #endif
 #ifndef CYTHON_UNUSED
+  #if defined(__cplusplus)
+    /* for clang __has_cpp_attribute(maybe_unused) is true even before C++17
+     * but leads to warnings with -pedantic, since it is a C++17 feature */
+    #if ((defined(_MSVC_LANG) && _MSVC_LANG >= 201703L) || __cplusplus >= 201703L)
+      #if __has_cpp_attribute(maybe_unused)
+        #define CYTHON_UNUSED [[maybe_unused]]
+      #endif
+    #endif
+  #endif
+#endif
+#ifndef CYTHON_UNUSED
 # if defined(__GNUC__)
 #   if !(defined(__cplusplus)) || (__GNUC__ > 3 || (__GNUC__ == 3 && __GNUC_MINOR__ >= 4))
 #     define CYTHON_UNUSED __attribute__ ((__unused__))
 #   else
 #     define CYTHON_UNUSED
 #   endif
 # elif defined(__ICC) || (defined(__INTEL_COMPILER) && !defined(_MSC_VER))
 #   define CYTHON_UNUSED __attribute__ ((__unused__))
 # else
 #   define CYTHON_UNUSED
 # endif
 #endif
-#ifndef CYTHON_MAYBE_UNUSED_VAR
+#ifndef CYTHON_UNUSED_VAR
 #  if defined(__cplusplus)
-     template<class T> void CYTHON_MAYBE_UNUSED_VAR( const T& ) { }
+     template<class T> void CYTHON_UNUSED_VAR( const T& ) { }
 #  else
-#    define CYTHON_MAYBE_UNUSED_VAR(x) (void)(x)
+#    define CYTHON_UNUSED_VAR(x) (void)(x)
 #  endif
 #endif
+#ifndef CYTHON_MAYBE_UNUSED_VAR
+  #define CYTHON_MAYBE_UNUSED_VAR(x) CYTHON_UNUSED_VAR(x)
+#endif
 #ifndef CYTHON_NCP_UNUSED
 # if CYTHON_COMPILING_IN_CPYTHON
 #  define CYTHON_NCP_UNUSED
 # else
 #  define CYTHON_NCP_UNUSED CYTHON_UNUSED
 # endif
 #endif
 #define __Pyx_void_to_None(void_result) ((void)(void_result), Py_INCREF(Py_None), Py_None)
 #ifdef _MSC_VER
     #ifndef _MSC_STDINT_H_
         #if _MSC_VER < 1300
-           typedef unsigned char     uint8_t;
-           typedef unsigned int      uint32_t;
+            typedef unsigned char     uint8_t;
+            typedef unsigned short    uint16_t;
+            typedef unsigned int      uint32_t;
+        #else
+            typedef unsigned __int8   uint8_t;
+            typedef unsigned __int16  uint16_t;
+            typedef unsigned __int32  uint32_t;
+        #endif
+    #endif
+    #if _MSC_VER < 1300
+        #ifdef _WIN64
+            typedef unsigned long long  __pyx_uintptr_t;
+        #else
+            typedef unsigned int        __pyx_uintptr_t;
+        #endif
+    #else
+        #ifdef _WIN64
+            typedef unsigned __int64    __pyx_uintptr_t;
         #else
-           typedef unsigned __int8   uint8_t;
-           typedef unsigned __int32  uint32_t;
+            typedef unsigned __int32    __pyx_uintptr_t;
         #endif
     #endif
 #else
-   #include <stdint.h>
+    #include <stdint.h>
+    typedef uintptr_t  __pyx_uintptr_t;
 #endif
 #ifndef CYTHON_FALLTHROUGH
-  #if defined(__cplusplus) && __cplusplus >= 201103L
-    #if __has_cpp_attribute(fallthrough)
-      #define CYTHON_FALLTHROUGH [[fallthrough]]
-    #elif __has_cpp_attribute(clang::fallthrough)
-      #define CYTHON_FALLTHROUGH [[clang::fallthrough]]
-    #elif __has_cpp_attribute(gnu::fallthrough)
-      #define CYTHON_FALLTHROUGH [[gnu::fallthrough]]
+  #if defined(__cplusplus)
+    /* for clang __has_cpp_attribute(fallthrough) is true even before C++17
+     * but leads to warnings with -pedantic, since it is a C++17 feature */
+    #if ((defined(_MSVC_LANG) && _MSVC_LANG >= 201703L) || __cplusplus >= 201703L)
+      #if __has_cpp_attribute(fallthrough)
+        #define CYTHON_FALLTHROUGH [[fallthrough]]
+      #endif
+    #endif
+    #ifndef CYTHON_FALLTHROUGH
+      #if __has_cpp_attribute(clang::fallthrough)
+        #define CYTHON_FALLTHROUGH [[clang::fallthrough]]
+      #elif __has_cpp_attribute(gnu::fallthrough)
+        #define CYTHON_FALLTHROUGH [[gnu::fallthrough]]
+      #endif
     #endif
   #endif
   #ifndef CYTHON_FALLTHROUGH
     #if __has_attribute(fallthrough)
       #define CYTHON_FALLTHROUGH __attribute__((fallthrough))
     #else
       #define CYTHON_FALLTHROUGH
     #endif
   #endif
-  #if defined(__clang__ ) && defined(__apple_build_version__)
+  #if defined(__clang__) && defined(__apple_build_version__)
     #if __apple_build_version__ < 7000000
       #undef  CYTHON_FALLTHROUGH
       #define CYTHON_FALLTHROUGH
     #endif
   #endif
 #endif
+#ifdef __cplusplus
+  template <typename T>
+  struct __PYX_IS_UNSIGNED_IMPL {static const bool value = T(0) < T(-1);};
+  #define __PYX_IS_UNSIGNED(type) (__PYX_IS_UNSIGNED_IMPL<type>::value)
+#else
+  #define __PYX_IS_UNSIGNED(type) (((type)-1) > 0)
+#endif
+#if CYTHON_COMPILING_IN_PYPY == 1
+  #define __PYX_NEED_TP_PRINT_SLOT  (PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x030A0000)
+#else
+  #define __PYX_NEED_TP_PRINT_SLOT  (PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000)
+#endif
+#define __PYX_REINTERPRET_FUNCION(func_pointer, other_pointer) ((func_pointer)(void(*)(void))(other_pointer))
 
 #ifndef __cplusplus
   #error "Cython files generated with the C++ option must be compiled with a C++ compiler."
 #endif
 #ifndef CYTHON_INLINE
   #if defined(__clang__)
     #define CYTHON_INLINE __inline__ __attribute__ ((__unused__))
@@ -421,49 +588,48 @@
 class __Pyx_FakeReference {
   public:
     __Pyx_FakeReference() : ptr(NULL) { }
     __Pyx_FakeReference(const T& ref) : ptr(const_cast<T*>(&ref)) { }
     T *operator->() { return ptr; }
     T *operator&() { return ptr; }
     operator T&() { return *ptr; }
-    template<typename U> bool operator ==(U other) { return *ptr == other; }
-    template<typename U> bool operator !=(U other) { return *ptr != other; }
+    template<typename U> bool operator ==(const U& other) const { return *ptr == other; }
+    template<typename U> bool operator !=(const U& other) const { return *ptr != other; }
+    template<typename U> bool operator==(const __Pyx_FakeReference<U>& other) const { return *ptr == *other.ptr; }
+    template<typename U> bool operator!=(const __Pyx_FakeReference<U>& other) const { return *ptr != *other.ptr; }
   private:
     T *ptr;
 };
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
-  #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
-          PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
+  #define __Pyx_PyCode_New(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
+          PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #else
   #define __Pyx_BUILTIN_MODULE_NAME "builtins"
   #define __Pyx_DefaultClassType PyType_Type
 #if PY_VERSION_HEX >= 0x030B00A1
-    static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int k, int l, int s, int f,
+    static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
                                                     PyObject *code, PyObject *c, PyObject* n, PyObject *v,
                                                     PyObject *fv, PyObject *cell, PyObject* fn,
                                                     PyObject *name, int fline, PyObject *lnos) {
         PyObject *kwds=NULL, *argcount=NULL, *posonlyargcount=NULL, *kwonlyargcount=NULL;
-        PyObject *nlocals=NULL, *stacksize=NULL, *flags=NULL, *replace=NULL, *call_result=NULL, *empty=NULL;
+        PyObject *nlocals=NULL, *stacksize=NULL, *flags=NULL, *replace=NULL, *empty=NULL;
         const char *fn_cstr=NULL;
         const char *name_cstr=NULL;
-        PyCodeObject* co=NULL;
+        PyCodeObject *co=NULL, *result=NULL;
         PyObject *type, *value, *traceback;
         PyErr_Fetch(&type, &value, &traceback);
         if (!(kwds=PyDict_New())) goto end;
         if (!(argcount=PyLong_FromLong(a))) goto end;
         if (PyDict_SetItemString(kwds, "co_argcount", argcount) != 0) goto end;
-        if (!(posonlyargcount=PyLong_FromLong(0))) goto end;
+        if (!(posonlyargcount=PyLong_FromLong(p))) goto end;
         if (PyDict_SetItemString(kwds, "co_posonlyargcount", posonlyargcount) != 0) goto end;
         if (!(kwonlyargcount=PyLong_FromLong(k))) goto end;
         if (PyDict_SetItemString(kwds, "co_kwonlyargcount", kwonlyargcount) != 0) goto end;
         if (!(nlocals=PyLong_FromLong(l))) goto end;
         if (PyDict_SetItemString(kwds, "co_nlocals", nlocals) != 0) goto end;
         if (!(stacksize=PyLong_FromLong(s))) goto end;
         if (PyDict_SetItemString(kwds, "co_stacksize", stacksize) != 0) goto end;
@@ -475,104 +641,180 @@
         if (PyDict_SetItemString(kwds, "co_varnames", v) != 0) goto end;
         if (PyDict_SetItemString(kwds, "co_freevars", fv) != 0) goto end;
         if (PyDict_SetItemString(kwds, "co_cellvars", cell) != 0) goto end;
         if (PyDict_SetItemString(kwds, "co_linetable", lnos) != 0) goto end;
         if (!(fn_cstr=PyUnicode_AsUTF8AndSize(fn, NULL))) goto end;
         if (!(name_cstr=PyUnicode_AsUTF8AndSize(name, NULL))) goto end;
         if (!(co = PyCode_NewEmpty(fn_cstr, name_cstr, fline))) goto end;
-        if (!(replace = PyObject_GetAttrString((PyObject*)co, "replace"))) goto cleanup_code_too;
-        if (!(empty = PyTuple_New(0))) goto cleanup_code_too; // unfortunately __pyx_empty_tuple isn't available here
-        if (!(call_result = PyObject_Call(replace, empty, kwds))) goto cleanup_code_too;
-        Py_XDECREF((PyObject*)co);
-        co = (PyCodeObject*)call_result;
-        call_result = NULL;
-        if (0) {
-            cleanup_code_too:
-            Py_XDECREF((PyObject*)co);
-            co = NULL;
-        }
-        end:
+        if (!(replace = PyObject_GetAttrString((PyObject*)co, "replace"))) goto end;
+        if (!(empty = PyTuple_New(0))) goto end;
+        result = (PyCodeObject*) PyObject_Call(replace, empty, kwds);
+    end:
+        Py_XDECREF((PyObject*) co);
         Py_XDECREF(kwds);
         Py_XDECREF(argcount);
         Py_XDECREF(posonlyargcount);
         Py_XDECREF(kwonlyargcount);
         Py_XDECREF(nlocals);
         Py_XDECREF(stacksize);
         Py_XDECREF(replace);
-        Py_XDECREF(call_result);
         Py_XDECREF(empty);
         if (type) {
             PyErr_Restore(type, value, traceback);
         }
-        return co;
+        return result;
     }
+#elif PY_VERSION_HEX >= 0x030800B2 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyCode_New(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
+          PyCode_NewWithPosOnlyArgs(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #else
-  #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
+  #define __Pyx_PyCode_New(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
-  #define __Pyx_DefaultClassType PyType_Type
+#endif
+#if PY_VERSION_HEX >= 0x030900A4 || defined(Py_IS_TYPE)
+  #define __Pyx_IS_TYPE(ob, type) Py_IS_TYPE(ob, type)
+#else
+  #define __Pyx_IS_TYPE(ob, type) (((const PyObject*)ob)->ob_type == (type))
+#endif
+#if PY_VERSION_HEX >= 0x030A00B1 || defined(Py_Is)
+  #define __Pyx_Py_Is(x, y)  Py_Is(x, y)
+#else
+  #define __Pyx_Py_Is(x, y) ((x) == (y))
+#endif
+#if PY_VERSION_HEX >= 0x030A00B1 || defined(Py_IsNone)
+  #define __Pyx_Py_IsNone(ob) Py_IsNone(ob)
+#else
+  #define __Pyx_Py_IsNone(ob) __Pyx_Py_Is((ob), Py_None)
+#endif
+#if PY_VERSION_HEX >= 0x030A00B1 || defined(Py_IsTrue)
+  #define __Pyx_Py_IsTrue(ob) Py_IsTrue(ob)
+#else
+  #define __Pyx_Py_IsTrue(ob) __Pyx_Py_Is((ob), Py_True)
+#endif
+#if PY_VERSION_HEX >= 0x030A00B1 || defined(Py_IsFalse)
+  #define __Pyx_Py_IsFalse(ob) Py_IsFalse(ob)
+#else
+  #define __Pyx_Py_IsFalse(ob) __Pyx_Py_Is((ob), Py_False)
+#endif
+#define __Pyx_NoneAsNull(obj)  (__Pyx_Py_IsNone(obj) ? NULL : (obj))
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
+#ifndef CO_COROUTINE
+  #define CO_COROUTINE 0x80
+#endif
+#ifndef CO_ASYNC_GENERATOR
+  #define CO_ASYNC_GENERATOR 0x200
 #endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
   #define Py_TPFLAGS_HAVE_NEWBUFFER 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_FINALIZE
   #define Py_TPFLAGS_HAVE_FINALIZE 0
 #endif
+#ifndef Py_TPFLAGS_SEQUENCE
+  #define Py_TPFLAGS_SEQUENCE 0
+#endif
+#ifndef Py_TPFLAGS_MAPPING
+  #define Py_TPFLAGS_MAPPING 0
+#endif
 #ifndef METH_STACKLESS
   #define METH_STACKLESS 0
 #endif
 #if PY_VERSION_HEX <= 0x030700A3 || !defined(METH_FASTCALL)
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
   #define __Pyx_PyCFunctionFast _PyCFunctionFast
   #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
 #endif
-#if CYTHON_FAST_PYCCALL
-#define __Pyx_PyFastCFunction_Check(func)\
-    ((PyCFunction_Check(func) && (METH_FASTCALL == (PyCFunction_GET_FLAGS(func) & ~(METH_CLASS | METH_STATIC | METH_COEXIST | METH_KEYWORDS | METH_STACKLESS)))))
+#if CYTHON_METH_FASTCALL
+  #define __Pyx_METH_FASTCALL METH_FASTCALL
+  #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
+  #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
+#else
+  #define __Pyx_METH_FASTCALL METH_VARARGS
+  #define __Pyx_PyCFunction_FastCall PyCFunction
+  #define __Pyx_PyCFunction_FastCallWithKeywords PyCFunctionWithKeywords
+#endif
+#if CYTHON_VECTORCALL
+  #define __pyx_vectorcallfunc vectorcallfunc
+  #define __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET  PY_VECTORCALL_ARGUMENTS_OFFSET
+  #define __Pyx_PyVectorcall_NARGS(n)  PyVectorcall_NARGS((size_t)(n))
+#elif CYTHON_BACKPORT_VECTORCALL
+  typedef PyObject *(*__pyx_vectorcallfunc)(PyObject *callable, PyObject *const *args,
+                                            size_t nargsf, PyObject *kwnames);
+  #define __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET  ((size_t)1 << (8 * sizeof(size_t) - 1))
+  #define __Pyx_PyVectorcall_NARGS(n)  ((Py_ssize_t)(((size_t)(n)) & ~__Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET))
+#else
+  #define __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET  0
+  #define __Pyx_PyVectorcall_NARGS(n)  ((Py_ssize_t)(n))
+#endif
+#if PY_VERSION_HEX < 0x030900B1
+  #define __Pyx_PyType_FromModuleAndSpec(m, s, b)  ((void)m, PyType_FromSpecWithBases(s, b))
+  typedef PyObject *(*__Pyx_PyCMethod)(PyObject *, PyTypeObject *, PyObject *const *, size_t, PyObject *);
 #else
-#define __Pyx_PyFastCFunction_Check(func) 0
+  #define __Pyx_PyType_FromModuleAndSpec(m, s, b)  PyType_FromModuleAndSpec(m, s, b)
+  #define __Pyx_PyCMethod  PyCMethod
+#endif
+#ifndef METH_METHOD
+  #define METH_METHOD 0x200
 #endif
 #if CYTHON_COMPILING_IN_PYPY && !defined(PyObject_Malloc)
   #define PyObject_Malloc(s)   PyMem_Malloc(s)
   #define PyObject_Free(p)     PyMem_Free(p)
   #define PyObject_Realloc(p)  PyMem_Realloc(p)
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030400A1
-  #define PyMem_RawMalloc(n)           PyMem_Malloc(n)
-  #define PyMem_RawRealloc(p, n)       PyMem_Realloc(p, n)
-  #define PyMem_RawFree(p)             PyMem_Free(p)
-#endif
-#if CYTHON_COMPILING_IN_PYSTON
-  #define __Pyx_PyCode_HasFreeVars(co)  PyCode_HasFreeVars(co)
-  #define __Pyx_PyFrame_SetLineNumber(frame, lineno) PyFrame_SetLineNumber(frame, lineno)
+#if CYTHON_COMPILING_IN_LIMITED_API
+  #define __Pyx_PyCode_HasFreeVars(co)  (PyCode_GetNumFree(co) > 0)
+  #define __Pyx_PyFrame_SetLineNumber(frame, lineno)
 #else
   #define __Pyx_PyCode_HasFreeVars(co)  (PyCode_GetNumFree(co) > 0)
   #define __Pyx_PyFrame_SetLineNumber(frame, lineno)  (frame)->f_lineno = (lineno)
 #endif
-#if !CYTHON_FAST_THREAD_STATE || PY_VERSION_HEX < 0x02070000
+#if CYTHON_COMPILING_IN_LIMITED_API
+  #define __Pyx_PyThreadState_Current PyThreadState_Get()
+#elif !CYTHON_FAST_THREAD_STATE
   #define __Pyx_PyThreadState_Current PyThreadState_GET()
 #elif PY_VERSION_HEX >= 0x03060000
   #define __Pyx_PyThreadState_Current _PyThreadState_UncheckedGet()
 #elif PY_VERSION_HEX >= 0x03000000
   #define __Pyx_PyThreadState_Current PyThreadState_GET()
 #else
   #define __Pyx_PyThreadState_Current _PyThreadState_Current
 #endif
+#if CYTHON_COMPILING_IN_LIMITED_API
+static CYTHON_INLINE void *__Pyx_PyModule_GetState(PyObject *op)
+{
+    void *result;
+    result = PyModule_GetState(op);
+    if (!result)
+        Py_FatalError("Couldn't find the module state");
+    return result;
+}
+#endif
+#define __Pyx_PyObject_GetSlot(obj, name, func_ctype)  __Pyx_PyType_GetSlot(Py_TYPE(obj), name, func_ctype)
+#if CYTHON_COMPILING_IN_LIMITED_API
+  #define __Pyx_PyType_GetSlot(type, name, func_ctype)  ((func_ctype) PyType_GetSlot((type), Py_##name))
+#else
+  #define __Pyx_PyType_GetSlot(type, name, func_ctype)  ((type)->name)
+#endif
 #if PY_VERSION_HEX < 0x030700A2 && !defined(PyThread_tss_create) && !defined(Py_tss_NEEDS_INIT)
 #include "pythread.h"
 #define Py_tss_NEEDS_INIT 0
 typedef int Py_tss_t;
 static CYTHON_INLINE int PyThread_tss_create(Py_tss_t *key) {
   *key = PyThread_create_key();
   return 0;
@@ -595,86 +837,166 @@
 static CYTHON_INLINE int PyThread_tss_set(Py_tss_t *key, void *value) {
   return PyThread_set_key_value(*key, value);
 }
 static CYTHON_INLINE void * PyThread_tss_get(Py_tss_t *key) {
   return PyThread_get_key_value(*key);
 }
 #endif
+#if PY_MAJOR_VERSION < 3
+    #if CYTHON_COMPILING_IN_PYPY
+        #if PYPY_VERSION_NUM < 0x07030600
+            #if defined(__cplusplus) && __cplusplus >= 201402L
+                [[deprecated("`with nogil:` inside a nogil function will not release the GIL in PyPy2 < 7.3.6")]]
+            #elif defined(__GNUC__) || defined(__clang__)
+                __attribute__ ((__deprecated__("`with nogil:` inside a nogil function will not release the GIL in PyPy2 < 7.3.6")))
+            #elif defined(_MSC_VER)
+                __declspec(deprecated("`with nogil:` inside a nogil function will not release the GIL in PyPy2 < 7.3.6"))
+            #endif
+            static CYTHON_INLINE int PyGILState_Check(void) {
+                return 0;
+            }
+        #else  // PYPY_VERSION_NUM < 0x07030600
+        #endif  // PYPY_VERSION_NUM < 0x07030600
+    #else
+        static CYTHON_INLINE int PyGILState_Check(void) {
+            PyThreadState * tstate = _PyThreadState_Current;
+            return tstate && (tstate == PyGILState_GetThisThreadState());
+        }
+    #endif
+#endif
 #if CYTHON_COMPILING_IN_CPYTHON || defined(_PyDict_NewPresized)
 #define __Pyx_PyDict_NewPresized(n)  ((n <= 8) ? PyDict_New() : _PyDict_NewPresized(n))
 #else
 #define __Pyx_PyDict_NewPresized(n)  PyDict_New()
 #endif
 #if PY_MAJOR_VERSION >= 3 || CYTHON_FUTURE_DIVISION
   #define __Pyx_PyNumber_Divide(x,y)         PyNumber_TrueDivide(x,y)
   #define __Pyx_PyNumber_InPlaceDivide(x,y)  PyNumber_InPlaceTrueDivide(x,y)
 #else
   #define __Pyx_PyNumber_Divide(x,y)         PyNumber_Divide(x,y)
   #define __Pyx_PyNumber_InPlaceDivide(x,y)  PyNumber_InPlaceDivide(x,y)
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
-#define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX > 0x030600B4 && CYTHON_USE_UNICODE_INTERNALS
+#define __Pyx_PyDict_GetItemStrWithError(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
+static CYTHON_INLINE PyObject * __Pyx_PyDict_GetItemStr(PyObject *dict, PyObject *name) {
+    PyObject *res = __Pyx_PyDict_GetItemStrWithError(dict, name);
+    if (res == NULL) PyErr_Clear();
+    return res;
+}
+#elif PY_MAJOR_VERSION >= 3 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07020000)
+#define __Pyx_PyDict_GetItemStrWithError  PyDict_GetItemWithError
+#define __Pyx_PyDict_GetItemStr           PyDict_GetItem
 #else
-#define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
+static CYTHON_INLINE PyObject * __Pyx_PyDict_GetItemStrWithError(PyObject *dict, PyObject *name) {
+#if CYTHON_COMPILING_IN_PYPY
+    return PyDict_GetItem(dict, name);
+#else
+    PyDictEntry *ep;
+    PyDictObject *mp = (PyDictObject*) dict;
+    long hash = ((PyStringObject *) name)->ob_shash;
+    assert(hash != -1);
+    ep = (mp->ma_lookup)(mp, name, hash);
+    if (ep == NULL) {
+        return NULL;
+    }
+    return ep->me_value;
 #endif
-#if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
+}
+#define __Pyx_PyDict_GetItemStr           PyDict_GetItem
+#endif
+#if CYTHON_USE_TYPE_SLOTS
+  #define __Pyx_PyType_GetFlags(tp)   (((PyTypeObject *)tp)->tp_flags)
+  #define __Pyx_PyType_HasFeature(type, feature)  ((__Pyx_PyType_GetFlags(type) & (feature)) != 0)
+  #define __Pyx_PyObject_GetIterNextFunc(obj)  (Py_TYPE(obj)->tp_iternext)
+#else
+  #define __Pyx_PyType_GetFlags(tp)   (PyType_GetFlags((PyTypeObject *)tp))
+  #define __Pyx_PyType_HasFeature(type, feature)  PyType_HasFeature(type, feature)
+  #define __Pyx_PyObject_GetIterNextFunc(obj)  PyIter_Next
+#endif
+#if CYTHON_USE_TYPE_SPECS && PY_VERSION_HEX >= 0x03080000
+#define __Pyx_PyHeapTypeObject_GC_Del(obj)  {\
+    PyTypeObject *type = Py_TYPE(obj);\
+    assert(__Pyx_PyType_HasFeature(type, Py_TPFLAGS_HEAPTYPE));\
+    PyObject_GC_Del(obj);\
+    Py_DECREF(type);\
+}
+#else
+#define __Pyx_PyHeapTypeObject_GC_Del(obj)  PyObject_GC_Del(obj)
+#endif
+#if CYTHON_COMPILING_IN_LIMITED_API
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
-  #else
   #define __Pyx_PyUnicode_READY(op)       (0)
+  #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GetLength(u)
+  #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_ReadChar(u, i)
+  #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   ((void)u, 1114111U)
+  #define __Pyx_PyUnicode_KIND(u)         ((void)u, (0))
+  #define __Pyx_PyUnicode_DATA(u)         ((void*)u)
+  #define __Pyx_PyUnicode_READ(k, d, i)   ((void)k, PyUnicode_ReadChar((PyObject*)(d), i))
+  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GetLength(u))
+#elif PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
+  #define CYTHON_PEP393_ENABLED 1
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
+  #else
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
-  #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
+  #define __Pyx_PyUnicode_KIND(u)         ((int)PyUnicode_KIND(u))
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
-  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
-  #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
+  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, (Py_UCS4) ch)
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_SIZE(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) ((Py_UCS4)(PyUnicode_AS_UNICODE(u)[i]))
-  #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   ((sizeof(Py_UNICODE) == 2) ? 65535 : 1114111)
-  #define __Pyx_PyUnicode_KIND(u)         (sizeof(Py_UNICODE))
+  #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   ((sizeof(Py_UNICODE) == 2) ? 65535U : 1114111U)
+  #define __Pyx_PyUnicode_KIND(u)         ((int)sizeof(Py_UNICODE))
   #define __Pyx_PyUnicode_DATA(u)         ((void*)PyUnicode_AS_UNICODE(u))
   #define __Pyx_PyUnicode_READ(k, d, i)   ((void)(k), (Py_UCS4)(((Py_UNICODE*)d)[i]))
-  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  (((void)(k)), ((Py_UNICODE*)d)[i] = ch)
+  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  (((void)(k)), ((Py_UNICODE*)d)[i] = (Py_UNICODE) ch)
   #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_SIZE(u))
 #endif
 #if CYTHON_COMPILING_IN_PYPY
   #define __Pyx_PyUnicode_Concat(a, b)      PyNumber_Add(a, b)
   #define __Pyx_PyUnicode_ConcatSafe(a, b)  PyNumber_Add(a, b)
 #else
   #define __Pyx_PyUnicode_Concat(a, b)      PyUnicode_Concat(a, b)
   #define __Pyx_PyUnicode_ConcatSafe(a, b)  ((unlikely((a) == Py_None) || unlikely((b) == Py_None)) ?\
       PyNumber_Add(a, b) : __Pyx_PyUnicode_Concat(a, b))
 #endif
-#if CYTHON_COMPILING_IN_PYPY && !defined(PyUnicode_Contains)
-  #define PyUnicode_Contains(u, s)  PySequence_Contains(u, s)
-#endif
-#if CYTHON_COMPILING_IN_PYPY && !defined(PyByteArray_Check)
-  #define PyByteArray_Check(obj)  PyObject_TypeCheck(obj, &PyByteArray_Type)
-#endif
-#if CYTHON_COMPILING_IN_PYPY && !defined(PyObject_Format)
-  #define PyObject_Format(obj, fmt)  PyObject_CallMethod(obj, "__format__", "O", fmt)
+#if CYTHON_COMPILING_IN_PYPY
+  #if !defined(PyUnicode_DecodeUnicodeEscape)
+    #define PyUnicode_DecodeUnicodeEscape(s, size, errors)  PyUnicode_Decode(s, size, "unicode_escape", errors)
+  #endif
+  #if !defined(PyUnicode_Contains) || (PY_MAJOR_VERSION == 2 && PYPY_VERSION_NUM < 0x07030500)
+    #undef PyUnicode_Contains
+    #define PyUnicode_Contains(u, s)  PySequence_Contains(u, s)
+  #endif
+  #if !defined(PyByteArray_Check)
+    #define PyByteArray_Check(obj)  PyObject_TypeCheck(obj, &PyByteArray_Type)
+  #endif
+  #if !defined(PyObject_Format)
+    #define PyObject_Format(obj, fmt)  PyObject_CallMethod(obj, "__format__", "O", fmt)
+  #endif
 #endif
 #define __Pyx_PyString_FormatSafe(a, b)   ((unlikely((a) == Py_None || (PyString_Check(b) && !PyString_CheckExact(b)))) ? PyNumber_Remainder(a, b) : __Pyx_PyString_Format(a, b))
 #define __Pyx_PyUnicode_FormatSafe(a, b)  ((unlikely((a) == Py_None || (PyUnicode_Check(b) && !PyUnicode_CheckExact(b)))) ? PyNumber_Remainder(a, b) : PyUnicode_Format(a, b))
 #if PY_MAJOR_VERSION >= 3
   #define __Pyx_PyString_Format(a, b)  PyUnicode_Format(a, b)
 #else
   #define __Pyx_PyString_Format(a, b)  PyString_Format(a, b)
@@ -695,16 +1017,22 @@
 #if PY_MAJOR_VERSION >= 3
   #define __Pyx_PyBaseString_Check(obj) PyUnicode_Check(obj)
   #define __Pyx_PyBaseString_CheckExact(obj) PyUnicode_CheckExact(obj)
 #else
   #define __Pyx_PyBaseString_Check(obj) (PyString_Check(obj) || PyUnicode_Check(obj))
   #define __Pyx_PyBaseString_CheckExact(obj) (PyString_CheckExact(obj) || PyUnicode_CheckExact(obj))
 #endif
+#if CYTHON_COMPILING_IN_CPYTHON
+  #define __Pyx_PySequence_ListKeepNew(obj)\
+    (likely(PyList_CheckExact(obj) && Py_REFCNT(obj) == 1) ? __Pyx_NewRef(obj) : PySequence_List(obj))
+#else
+  #define __Pyx_PySequence_ListKeepNew(obj)  PySequence_List(obj)
+#endif
 #ifndef PySet_CheckExact
-  #define PySet_CheckExact(obj)        (Py_TYPE(obj) == &PySet_Type)
+  #define PySet_CheckExact(obj)        __Pyx_IS_TYPE(obj, &PySet_Type)
 #endif
 #if PY_VERSION_HEX >= 0x030900A4
   #define __Pyx_SET_REFCNT(obj, refcnt) Py_SET_REFCNT(obj, refcnt)
   #define __Pyx_SET_SIZE(obj, size) Py_SET_SIZE(obj, size)
 #else
   #define __Pyx_SET_REFCNT(obj, refcnt) Py_REFCNT(obj) = (refcnt)
   #define __Pyx_SET_SIZE(obj, size) Py_SIZE(obj) = (size)
@@ -715,25 +1043,30 @@
   #define __Pyx_PySequence_SIZE(seq)  PySequence_Size(seq)
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define PyIntObject                  PyLongObject
   #define PyInt_Type                   PyLong_Type
   #define PyInt_Check(op)              PyLong_Check(op)
   #define PyInt_CheckExact(op)         PyLong_CheckExact(op)
+  #define __Pyx_Py3Int_Check(op)       PyLong_Check(op)
+  #define __Pyx_Py3Int_CheckExact(op)  PyLong_CheckExact(op)
   #define PyInt_FromString             PyLong_FromString
   #define PyInt_FromUnicode            PyLong_FromUnicode
   #define PyInt_FromLong               PyLong_FromLong
   #define PyInt_FromSize_t             PyLong_FromSize_t
   #define PyInt_FromSsize_t            PyLong_FromSsize_t
   #define PyInt_AsLong                 PyLong_AsLong
   #define PyInt_AS_LONG                PyLong_AS_LONG
   #define PyInt_AsSsize_t              PyLong_AsSsize_t
   #define PyInt_AsUnsignedLongMask     PyLong_AsUnsignedLongMask
   #define PyInt_AsUnsignedLongLongMask PyLong_AsUnsignedLongLongMask
   #define PyNumber_Int                 PyNumber_Long
+#else
+  #define __Pyx_Py3Int_Check(op)       (PyLong_Check(op) || PyInt_Check(op))
+  #define __Pyx_Py3Int_CheckExact(op)  (PyLong_CheckExact(op) || PyInt_CheckExact(op))
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define PyBoolObject                 PyLongObject
 #endif
 #if PY_MAJOR_VERSION >= 3 && CYTHON_COMPILING_IN_PYPY
   #ifndef PyUnicode_InternFromString
     #define PyUnicode_InternFromString(s) PyUnicode_FromString(s)
@@ -743,19 +1076,14 @@
   typedef long Py_hash_t;
   #define __Pyx_PyInt_FromHash_t PyInt_FromLong
   #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsHash_t
 #else
   #define __Pyx_PyInt_FromHash_t PyInt_FromSsize_t
   #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsSsize_t
 #endif
-#if PY_MAJOR_VERSION >= 3
-  #define __Pyx_PyMethod_New(func, self, klass) ((self) ? ((void)(klass), PyMethod_New(func, self)) : __Pyx_NewRef(func))
-#else
-  #define __Pyx_PyMethod_New(func, self, klass) PyMethod_New(func, self, klass)
-#endif
 #if CYTHON_USE_ASYNC_SLOTS
   #if PY_VERSION_HEX >= 0x030500B1
     #define __Pyx_PyAsyncMethodsStruct PyAsyncMethods
     #define __Pyx_PyType_AsAsync(obj) (Py_TYPE(obj)->tp_as_async)
   #else
     #define __Pyx_PyType_AsAsync(obj) ((__Pyx_PyAsyncMethodsStruct*) (Py_TYPE(obj)->tp_reserved))
   #endif
@@ -792,35 +1120,40 @@
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
     { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
-#ifndef __PYX_EXTERN_C
-  #ifdef __cplusplus
-    #define __PYX_EXTERN_C extern "C"
-  #else
-    #define __PYX_EXTERN_C extern
-  #endif
+#ifdef CYTHON_EXTERN_C
+    #undef __PYX_EXTERN_C
+    #define __PYX_EXTERN_C CYTHON_EXTERN_C
+#elif defined(__PYX_EXTERN_C)
+    #ifdef _MSC_VER
+    #pragma message ("Please do not define the '__PYX_EXTERN_C' macro externally. Use 'CYTHON_EXTERN_C' instead.")
+    #else
+    #warning Please do not define the '__PYX_EXTERN_C' macro externally. Use 'CYTHON_EXTERN_C' instead.
+    #endif
+#else
+    #define __PYX_EXTERN_C extern "C++"
 #endif
 
 #define __PYX_HAVE__arcticpy__wrapper
 #define __PYX_HAVE_API__arcticpy__wrapper
 /* Early includes */
 #include <string.h>
 #include <stdio.h>
+
+    /* Using NumPy API declarations from "numpy/__init__.cython-30.pxd" */
+    
 #include "numpy/arrayobject.h"
 #include "numpy/ndarrayobject.h"
 #include "numpy/ndarraytypes.h"
 #include "numpy/arrayscalars.h"
 #include "numpy/ufuncobject.h"
-
-    /* NumPy API declarations from "numpy/__init__.pxd" */
-    
 #include <string>
 #include "ios"
 #include "new"
 #include "stdexcept"
 #include "typeinfo"
 #include "util.hpp"
 #include "interface.hpp"
@@ -888,29 +1221,40 @@
 #endif
 #define __Pyx_PyBytes_AsWritableString(s)     ((char*) PyBytes_AS_STRING(s))
 #define __Pyx_PyBytes_AsWritableSString(s)    ((signed char*) PyBytes_AS_STRING(s))
 #define __Pyx_PyBytes_AsWritableUString(s)    ((unsigned char*) PyBytes_AS_STRING(s))
 #define __Pyx_PyBytes_AsString(s)     ((const char*) PyBytes_AS_STRING(s))
 #define __Pyx_PyBytes_AsSString(s)    ((const signed char*) PyBytes_AS_STRING(s))
 #define __Pyx_PyBytes_AsUString(s)    ((const unsigned char*) PyBytes_AS_STRING(s))
-#define __Pyx_PyObject_AsWritableString(s)    ((char*) __Pyx_PyObject_AsString(s))
-#define __Pyx_PyObject_AsWritableSString(s)    ((signed char*) __Pyx_PyObject_AsString(s))
-#define __Pyx_PyObject_AsWritableUString(s)    ((unsigned char*) __Pyx_PyObject_AsString(s))
+#define __Pyx_PyObject_AsWritableString(s)    ((char*)(__pyx_uintptr_t) __Pyx_PyObject_AsString(s))
+#define __Pyx_PyObject_AsWritableSString(s)    ((signed char*)(__pyx_uintptr_t) __Pyx_PyObject_AsString(s))
+#define __Pyx_PyObject_AsWritableUString(s)    ((unsigned char*)(__pyx_uintptr_t) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u) {
+#if CYTHON_COMPILING_IN_LIMITED_API
+static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const wchar_t *u)
+{
+    const wchar_t *u_end = u;
+    while (*u_end++) ;
+    return (size_t)(u_end - u - 1);
+}
+#else
+static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
+{
     const Py_UNICODE *u_end = u;
     while (*u_end++) ;
     return (size_t)(u_end - u - 1);
 }
+#endif
+#define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
 #define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
 #define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
@@ -928,15 +1272,60 @@
 #endif
 #define __pyx_PyFloat_AsFloat(x) ((float) __pyx_PyFloat_AsDouble(x))
 #if PY_MAJOR_VERSION >= 3
 #define __Pyx_PyNumber_Int(x) (PyLong_CheckExact(x) ? __Pyx_NewRef(x) : PyNumber_Long(x))
 #else
 #define __Pyx_PyNumber_Int(x) (PyInt_CheckExact(x) ? __Pyx_NewRef(x) : PyNumber_Int(x))
 #endif
-#define __Pyx_PyNumber_Float(x) (PyFloat_CheckExact(x) ? __Pyx_NewRef(x) : PyNumber_Float(x))
+#if CYTHON_USE_PYLONG_INTERNALS
+  #if PY_VERSION_HEX >= 0x030C00A7
+  #ifndef _PyLong_SIGN_MASK
+    #define _PyLong_SIGN_MASK 3
+  #endif
+  #ifndef _PyLong_NON_SIZE_BITS
+    #define _PyLong_NON_SIZE_BITS 3
+  #endif
+  #define __Pyx_PyLong_Sign(x)  (((PyLongObject*)x)->long_value.lv_tag & _PyLong_SIGN_MASK)
+  #define __Pyx_PyLong_IsNeg(x)  ((__Pyx_PyLong_Sign(x) & 2) != 0)
+  #define __Pyx_PyLong_IsNonNeg(x)  (!__Pyx_PyLong_IsNeg(x))
+  #define __Pyx_PyLong_IsZero(x)  (__Pyx_PyLong_Sign(x) & 1)
+  #define __Pyx_PyLong_IsPos(x)  (__Pyx_PyLong_Sign(x) == 0)
+  #define __Pyx_PyLong_CompactValueUnsigned(x)  (__Pyx_PyLong_Digits(x)[0])
+  #define __Pyx_PyLong_DigitCount(x)  ((Py_ssize_t) (((PyLongObject*)x)->long_value.lv_tag >> _PyLong_NON_SIZE_BITS))
+  #define __Pyx_PyLong_SignedDigitCount(x)\
+        ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * __Pyx_PyLong_DigitCount(x))
+  #if defined(PyUnstable_Long_IsCompact) && defined(PyUnstable_Long_CompactValue)
+    #define __Pyx_PyLong_IsCompact(x)     PyUnstable_Long_IsCompact((PyLongObject*) x)
+    #define __Pyx_PyLong_CompactValue(x)  PyUnstable_Long_CompactValue((PyLongObject*) x)
+  #else
+    #define __Pyx_PyLong_IsCompact(x)     (((PyLongObject*)x)->long_value.lv_tag < (2 << _PyLong_NON_SIZE_BITS))
+    #define __Pyx_PyLong_CompactValue(x)  ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * (Py_ssize_t) __Pyx_PyLong_Digits(x)[0])
+  #endif
+  typedef Py_ssize_t  __Pyx_compact_pylong;
+  typedef size_t  __Pyx_compact_upylong;
+  #else  // Py < 3.12
+  #define __Pyx_PyLong_IsNeg(x)  (Py_SIZE(x) < 0)
+  #define __Pyx_PyLong_IsNonNeg(x)  (Py_SIZE(x) >= 0)
+  #define __Pyx_PyLong_IsZero(x)  (Py_SIZE(x) == 0)
+  #define __Pyx_PyLong_IsPos(x)  (Py_SIZE(x) > 0)
+  #define __Pyx_PyLong_CompactValueUnsigned(x)  ((Py_SIZE(x) == 0) ? 0 : __Pyx_PyLong_Digits(x)[0])
+  #define __Pyx_PyLong_DigitCount(x)  __Pyx_sst_abs(Py_SIZE(x))
+  #define __Pyx_PyLong_SignedDigitCount(x)  Py_SIZE(x)
+  #define __Pyx_PyLong_IsCompact(x)  (Py_SIZE(x) == 0 || Py_SIZE(x) == 1 || Py_SIZE(x) == -1)
+  #define __Pyx_PyLong_CompactValue(x)\
+        ((Py_SIZE(x) == 0) ? (sdigit) 0 : ((Py_SIZE(x) < 0) ? -(sdigit)__Pyx_PyLong_Digits(x)[0] : (sdigit)__Pyx_PyLong_Digits(x)[0]))
+  typedef sdigit  __Pyx_compact_pylong;
+  typedef digit  __Pyx_compact_upylong;
+  #endif
+  #if PY_VERSION_HEX >= 0x030C00A5
+  #define __Pyx_PyLong_Digits(x)  (((PyLongObject*)x)->long_value.ob_digit)
+  #else
+  #define __Pyx_PyLong_Digits(x)  (((PyLongObject*)x)->ob_digit)
+  #endif
+#endif
 #if PY_MAJOR_VERSION < 3 && __PYX_DEFAULT_STRING_ENCODING_IS_ASCII
 static int __Pyx_sys_getdefaultencoding_not_ascii;
 static int __Pyx_init_sys_getdefaultencoding_params(void) {
     PyObject* sys;
     PyObject* default_encoding = NULL;
     PyObject* ascii_chars_u = NULL;
     PyObject* ascii_chars_b = NULL;
@@ -950,15 +1339,15 @@
     if (!default_encoding_c) goto bad;
     if (strcmp(default_encoding_c, "ascii") == 0) {
         __Pyx_sys_getdefaultencoding_not_ascii = 0;
     } else {
         char ascii_chars[128];
         int c;
         for (c = 0; c < 128; c++) {
-            ascii_chars[c] = c;
+            ascii_chars[c] = (char) c;
         }
         __Pyx_sys_getdefaultencoding_not_ascii = 1;
         ascii_chars_u = PyUnicode_DecodeASCII(ascii_chars, 128, NULL);
         if (!ascii_chars_u) goto bad;
         ascii_chars_b = PyUnicode_AsEncodedString(ascii_chars_u, default_encoding_c, NULL);
         if (!ascii_chars_b || !PyBytes_Check(ascii_chars_b) || memcmp(ascii_chars, PyBytes_AS_STRING(ascii_chars_b), 128) != 0) {
             PyErr_Format(
@@ -1015,31 +1404,27 @@
   #define unlikely(x) __builtin_expect(!!(x), 0)
 #else /* !__GNUC__ or GCC < 2.95 */
   #define likely(x)   (x)
   #define unlikely(x) (x)
 #endif /* __GNUC__ */
 static CYTHON_INLINE void __Pyx_pretend_to_initialize(void* ptr) { (void)ptr; }
 
+#if !CYTHON_USE_MODULE_STATE
 static PyObject *__pyx_m = NULL;
-static PyObject *__pyx_d;
-static PyObject *__pyx_b;
-static PyObject *__pyx_cython_runtime = NULL;
-static PyObject *__pyx_empty_tuple;
-static PyObject *__pyx_empty_bytes;
-static PyObject *__pyx_empty_unicode;
+#endif
 static int __pyx_lineno;
 static int __pyx_clineno = 0;
-static const char * __pyx_cfilenm= __FILE__;
+static const char * __pyx_cfilenm = __FILE__;
 static const char *__pyx_filename;
 
 /* Header.proto */
 #if !defined(CYTHON_CCOMPLEX)
   #if defined(__cplusplus)
     #define CYTHON_CCOMPLEX 1
-  #elif defined(_Complex_I)
+  #elif (defined(_Complex_I) && !defined(_MSC_VER)) || ((defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) && !defined(__STDC_NO_COMPLEX__))
     #define CYTHON_CCOMPLEX 1
   #else
     #define CYTHON_CCOMPLEX 0
   #endif
 #endif
 #if CYTHON_CCOMPLEX
   #ifdef __cplusplus
@@ -1049,23 +1434,24 @@
   #endif
 #endif
 #if CYTHON_CCOMPLEX && !defined(__cplusplus) && defined(__sun__) && defined(__GNUC__)
   #undef _Complex_I
   #define _Complex_I 1.0fj
 #endif
 
+/* #### Code section: filename_table ### */
 
 static const char *__pyx_f[] = {
+  "<stringsource>",
+  "__init__.cython-30.pxd",
   "python/arcticpy/wrapper.pyx",
-  "__init__.pxd",
-  "stringsource",
   "type.pxd",
 };
+/* #### Code section: utility_code_proto_before_types ### */
 /* BufferFormatStructs.proto */
-#define IS_UNSIGNED(type) (((type) -1) > 0)
 struct __Pyx_StructField_;
 #define __PYX_BUF_FLAGS_PACKED_STRUCT (1 << 0)
 typedef struct {
   const char* name;
   struct __Pyx_StructField_* fields;
   size_t size;
   size_t arraysize[8];
@@ -1092,330 +1478,490 @@
   int is_complex;
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
+/* #### Code section: numeric_typedefs ### */
 
-/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":689
+/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":732
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":690
+/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":733
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":691
+/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":734
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":692
+/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":735
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":696
+/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":739
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":697
+/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":740
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":698
+/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":741
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":699
+/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":742
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":703
+/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":746
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":704
+/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":747
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":713
+/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":756
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":714
+/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":757
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":715
+/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":758
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":717
+/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":718
+/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":719
+/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":762
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":721
+/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":764
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":722
+/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":765
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":724
+/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":725
+/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":726
+/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
+/* #### Code section: complex_type_declarations ### */
 /* Declarations.proto */
-#if CYTHON_CCOMPLEX
+#if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
   #ifdef __cplusplus
     typedef ::std::complex< float > __pyx_t_float_complex;
   #else
     typedef float _Complex __pyx_t_float_complex;
   #endif
 #else
     typedef struct { float real, imag; } __pyx_t_float_complex;
 #endif
 static CYTHON_INLINE __pyx_t_float_complex __pyx_t_float_complex_from_parts(float, float);
 
 /* Declarations.proto */
-#if CYTHON_CCOMPLEX
+#if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
   #ifdef __cplusplus
     typedef ::std::complex< double > __pyx_t_double_complex;
   #else
     typedef double _Complex __pyx_t_double_complex;
   #endif
 #else
     typedef struct { double real, imag; } __pyx_t_double_complex;
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
+/* #### Code section: type_declarations ### */
 
 /*--- Type declarations ---*/
 
-/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":728
+/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":729
+/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":772
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":730
+/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":732
+/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":775
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
+/* #### Code section: utility_code_proto ### */
 
 /* --- Runtime support code (head) --- */
 /* Refnanny.proto */
 #ifndef CYTHON_REFNANNY
   #define CYTHON_REFNANNY 0
 #endif
 #if CYTHON_REFNANNY
   typedef struct {
-    void (*INCREF)(void*, PyObject*, int);
-    void (*DECREF)(void*, PyObject*, int);
-    void (*GOTREF)(void*, PyObject*, int);
-    void (*GIVEREF)(void*, PyObject*, int);
-    void* (*SetupContext)(const char*, int, const char*);
+    void (*INCREF)(void*, PyObject*, Py_ssize_t);
+    void (*DECREF)(void*, PyObject*, Py_ssize_t);
+    void (*GOTREF)(void*, PyObject*, Py_ssize_t);
+    void (*GIVEREF)(void*, PyObject*, Py_ssize_t);
+    void* (*SetupContext)(const char*, Py_ssize_t, const char*);
     void (*FinishContext)(void**);
   } __Pyx_RefNannyAPIStruct;
   static __Pyx_RefNannyAPIStruct *__Pyx_RefNanny = NULL;
   static __Pyx_RefNannyAPIStruct *__Pyx_RefNannyImportAPI(const char *modname);
   #define __Pyx_RefNannyDeclarations void *__pyx_refnanny = NULL;
 #ifdef WITH_THREAD
   #define __Pyx_RefNannySetupContext(name, acquire_gil)\
           if (acquire_gil) {\
               PyGILState_STATE __pyx_gilstate_save = PyGILState_Ensure();\
-              __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), __LINE__, __FILE__);\
+              __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), (__LINE__), (__FILE__));\
               PyGILState_Release(__pyx_gilstate_save);\
           } else {\
-              __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), __LINE__, __FILE__);\
+              __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), (__LINE__), (__FILE__));\
+          }
+  #define __Pyx_RefNannyFinishContextNogil() {\
+              PyGILState_STATE __pyx_gilstate_save = PyGILState_Ensure();\
+              __Pyx_RefNannyFinishContext();\
+              PyGILState_Release(__pyx_gilstate_save);\
           }
 #else
   #define __Pyx_RefNannySetupContext(name, acquire_gil)\
-          __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), __LINE__, __FILE__)
+          __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), (__LINE__), (__FILE__))
+  #define __Pyx_RefNannyFinishContextNogil() __Pyx_RefNannyFinishContext()
 #endif
+  #define __Pyx_RefNannyFinishContextNogil() {\
+              PyGILState_STATE __pyx_gilstate_save = PyGILState_Ensure();\
+              __Pyx_RefNannyFinishContext();\
+              PyGILState_Release(__pyx_gilstate_save);\
+          }
   #define __Pyx_RefNannyFinishContext()\
           __Pyx_RefNanny->FinishContext(&__pyx_refnanny)
-  #define __Pyx_INCREF(r)  __Pyx_RefNanny->INCREF(__pyx_refnanny, (PyObject *)(r), __LINE__)
-  #define __Pyx_DECREF(r)  __Pyx_RefNanny->DECREF(__pyx_refnanny, (PyObject *)(r), __LINE__)
-  #define __Pyx_GOTREF(r)  __Pyx_RefNanny->GOTREF(__pyx_refnanny, (PyObject *)(r), __LINE__)
-  #define __Pyx_GIVEREF(r) __Pyx_RefNanny->GIVEREF(__pyx_refnanny, (PyObject *)(r), __LINE__)
-  #define __Pyx_XINCREF(r)  do { if((r) != NULL) {__Pyx_INCREF(r); }} while(0)
-  #define __Pyx_XDECREF(r)  do { if((r) != NULL) {__Pyx_DECREF(r); }} while(0)
-  #define __Pyx_XGOTREF(r)  do { if((r) != NULL) {__Pyx_GOTREF(r); }} while(0)
-  #define __Pyx_XGIVEREF(r) do { if((r) != NULL) {__Pyx_GIVEREF(r);}} while(0)
+  #define __Pyx_INCREF(r)  __Pyx_RefNanny->INCREF(__pyx_refnanny, (PyObject *)(r), (__LINE__))
+  #define __Pyx_DECREF(r)  __Pyx_RefNanny->DECREF(__pyx_refnanny, (PyObject *)(r), (__LINE__))
+  #define __Pyx_GOTREF(r)  __Pyx_RefNanny->GOTREF(__pyx_refnanny, (PyObject *)(r), (__LINE__))
+  #define __Pyx_GIVEREF(r) __Pyx_RefNanny->GIVEREF(__pyx_refnanny, (PyObject *)(r), (__LINE__))
+  #define __Pyx_XINCREF(r)  do { if((r) == NULL); else {__Pyx_INCREF(r); }} while(0)
+  #define __Pyx_XDECREF(r)  do { if((r) == NULL); else {__Pyx_DECREF(r); }} while(0)
+  #define __Pyx_XGOTREF(r)  do { if((r) == NULL); else {__Pyx_GOTREF(r); }} while(0)
+  #define __Pyx_XGIVEREF(r) do { if((r) == NULL); else {__Pyx_GIVEREF(r);}} while(0)
 #else
   #define __Pyx_RefNannyDeclarations
   #define __Pyx_RefNannySetupContext(name, acquire_gil)
+  #define __Pyx_RefNannyFinishContextNogil()
   #define __Pyx_RefNannyFinishContext()
   #define __Pyx_INCREF(r) Py_INCREF(r)
   #define __Pyx_DECREF(r) Py_DECREF(r)
   #define __Pyx_GOTREF(r)
   #define __Pyx_GIVEREF(r)
   #define __Pyx_XINCREF(r) Py_XINCREF(r)
   #define __Pyx_XDECREF(r) Py_XDECREF(r)
   #define __Pyx_XGOTREF(r)
   #define __Pyx_XGIVEREF(r)
 #endif
+#define __Pyx_Py_XDECREF_SET(r, v) do {\
+        PyObject *tmp = (PyObject *) r;\
+        r = v; Py_XDECREF(tmp);\
+    } while (0)
 #define __Pyx_XDECREF_SET(r, v) do {\
         PyObject *tmp = (PyObject *) r;\
         r = v; __Pyx_XDECREF(tmp);\
     } while (0)
 #define __Pyx_DECREF_SET(r, v) do {\
         PyObject *tmp = (PyObject *) r;\
         r = v; __Pyx_DECREF(tmp);\
     } while (0)
 #define __Pyx_CLEAR(r)    do { PyObject* tmp = ((PyObject*)(r)); r = NULL; __Pyx_DECREF(tmp);} while(0)
 #define __Pyx_XCLEAR(r)   do { if((r) != NULL) {PyObject* tmp = ((PyObject*)(r)); r = NULL; __Pyx_DECREF(tmp);}} while(0)
 
+/* PyErrExceptionMatches.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_PyErr_ExceptionMatches(err) __Pyx_PyErr_ExceptionMatchesInState(__pyx_tstate, err)
+static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err);
+#else
+#define __Pyx_PyErr_ExceptionMatches(err)  PyErr_ExceptionMatches(err)
+#endif
+
+/* PyThreadStateGet.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_PyThreadState_declare  PyThreadState *__pyx_tstate;
+#define __Pyx_PyThreadState_assign  __pyx_tstate = __Pyx_PyThreadState_Current;
+#if PY_VERSION_HEX >= 0x030C00A6
+#define __Pyx_PyErr_Occurred()  (__pyx_tstate->current_exception != NULL)
+#define __Pyx_PyErr_CurrentExceptionType()  (__pyx_tstate->current_exception ? (PyObject*) Py_TYPE(__pyx_tstate->current_exception) : (PyObject*) NULL)
+#else
+#define __Pyx_PyErr_Occurred()  (__pyx_tstate->curexc_type != NULL)
+#define __Pyx_PyErr_CurrentExceptionType()  (__pyx_tstate->curexc_type)
+#endif
+#else
+#define __Pyx_PyThreadState_declare
+#define __Pyx_PyThreadState_assign
+#define __Pyx_PyErr_Occurred()  (PyErr_Occurred() != NULL)
+#define __Pyx_PyErr_CurrentExceptionType()  PyErr_Occurred()
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
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A6
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
+/* PyObjectGetAttrStr.proto */
+#if CYTHON_USE_TYPE_SLOTS
+static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStr(PyObject* obj, PyObject* attr_name);
+#else
+#define __Pyx_PyObject_GetAttrStr(o,n) PyObject_GetAttr(o,n)
+#endif
+
+/* PyObjectGetAttrStrNoError.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
+
+/* GetBuiltinName.proto */
+static PyObject *__Pyx_GetBuiltinName(PyObject *name);
+
+/* GetTopmostException.proto */
+#if CYTHON_USE_EXC_INFO_STACK && CYTHON_FAST_THREAD_STATE
+static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
+#endif
+
+/* SaveResetException.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_ExceptionSave(type, value, tb)  __Pyx__ExceptionSave(__pyx_tstate, type, value, tb)
+static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
+#define __Pyx_ExceptionReset(type, value, tb)  __Pyx__ExceptionReset(__pyx_tstate, type, value, tb)
+static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
+#else
+#define __Pyx_ExceptionSave(type, value, tb)   PyErr_GetExcInfo(type, value, tb)
+#define __Pyx_ExceptionReset(type, value, tb)  PyErr_SetExcInfo(type, value, tb)
+#endif
+
+/* GetException.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_GetException(type, value, tb)  __Pyx__GetException(__pyx_tstate, type, value, tb)
+static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
+#else
+static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb);
+#endif
+
+/* PyObjectCall.proto */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw);
+#else
+#define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
+#endif
+
+/* RaiseException.proto */
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
+
+/* TupleAndListFromArray.proto */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyList_FromArray(PyObject *const *src, Py_ssize_t n);
+static CYTHON_INLINE PyObject* __Pyx_PyTuple_FromArray(PyObject *const *src, Py_ssize_t n);
+#endif
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
+/* fastcall.proto */
+#define __Pyx_Arg_VARARGS(args, i) PyTuple_GET_ITEM(args, i)
+#define __Pyx_NumKwargs_VARARGS(kwds) PyDict_Size(kwds)
+#define __Pyx_KwValues_VARARGS(args, nargs) NULL
+#define __Pyx_GetKwValue_VARARGS(kw, kwvalues, s) __Pyx_PyDict_GetItemStrWithError(kw, s)
+#define __Pyx_KwargsAsDict_VARARGS(kw, kwvalues) PyDict_Copy(kw)
+#if CYTHON_METH_FASTCALL
+    #define __Pyx_Arg_FASTCALL(args, i) args[i]
+    #define __Pyx_NumKwargs_FASTCALL(kwds) PyTuple_GET_SIZE(kwds)
+    #define __Pyx_KwValues_FASTCALL(args, nargs) ((args) + (nargs))
+    static CYTHON_INLINE PyObject * __Pyx_GetKwValue_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues, PyObject *s);
+    #define __Pyx_KwargsAsDict_FASTCALL(kw, kwvalues) _PyStack_AsDict(kwvalues, kw)
+#else
+    #define __Pyx_Arg_FASTCALL __Pyx_Arg_VARARGS
+    #define __Pyx_NumKwargs_FASTCALL __Pyx_NumKwargs_VARARGS
+    #define __Pyx_KwValues_FASTCALL __Pyx_KwValues_VARARGS
+    #define __Pyx_GetKwValue_FASTCALL __Pyx_GetKwValue_VARARGS
+    #define __Pyx_KwargsAsDict_FASTCALL __Pyx_KwargsAsDict_VARARGS
+#endif
+#if CYTHON_COMPILING_IN_CPYTHON
+#define __Pyx_ArgsSlice_VARARGS(args, start, stop) __Pyx_PyTuple_FromArray(&__Pyx_Arg_VARARGS(args, start), stop - start)
+#define __Pyx_ArgsSlice_FASTCALL(args, start, stop) __Pyx_PyTuple_FromArray(&__Pyx_Arg_FASTCALL(args, start), stop - start)
+#else
+#define __Pyx_ArgsSlice_VARARGS(args, start, stop) PyTuple_GetSlice(args, start, stop)
+#define __Pyx_ArgsSlice_FASTCALL(args, start, stop) PyTuple_GetSlice(args, start, stop)
+#endif
+
 /* IncludeCppStringH.proto */
 #include <string>
 
 /* decode_c_string_utf16.proto */
 static CYTHON_INLINE PyObject *__Pyx_PyUnicode_DecodeUTF16(const char *s, Py_ssize_t size, const char *errors) {
     int byteorder = 0;
     return PyUnicode_DecodeUTF16(s, size, errors, &byteorder);
@@ -1440,35 +1986,38 @@
          std::string cppstring, Py_ssize_t start, Py_ssize_t stop,
          const char* encoding, const char* errors,
          PyObject* (*decode_func)(const char *s, Py_ssize_t size, const char *errors)) {
     return __Pyx_decode_c_bytes(
         cppstring.data(), cppstring.size(), start, stop, encoding, errors, decode_func);
 }
 
-/* PyObjectGetAttrStr.proto */
-#if CYTHON_USE_TYPE_SLOTS
-static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStr(PyObject* obj, PyObject* attr_name);
-#else
-#define __Pyx_PyObject_GetAttrStr(o,n) PyObject_GetAttr(o,n)
-#endif
+/* RaiseDoubleKeywords.proto */
+static void __Pyx_RaiseDoubleKeywordsError(const char* func_name, PyObject* kw_name);
+
+/* ParseKeywords.proto */
+static int __Pyx_ParseOptionalKeywords(PyObject *kwds, PyObject *const *kwvalues,
+    PyObject **argnames[],
+    PyObject *kwds2, PyObject *values[], Py_ssize_t num_pos_args,
+    const char* function_name);
+
+/* RaiseArgTupleInvalid.proto */
+static void __Pyx_RaiseArgtupleInvalid(const char* func_name, int exact,
+    Py_ssize_t num_min, Py_ssize_t num_max, Py_ssize_t num_found);
 
 /* DictGetItem.proto */
 #if PY_MAJOR_VERSION >= 3 && !CYTHON_COMPILING_IN_PYPY
 static PyObject *__Pyx_PyDict_GetItem(PyObject *d, PyObject* key);
 #define __Pyx_PyObject_Dict_GetItem(obj, name)\
     (likely(PyDict_CheckExact(obj)) ?\
      __Pyx_PyDict_GetItem(obj, name) : PyObject_GetItem(obj, name))
 #else
 #define __Pyx_PyDict_GetItem(d, key) PyObject_GetItem(d, key)
 #define __Pyx_PyObject_Dict_GetItem(obj, name)  PyObject_GetItem(obj, name)
 #endif
 
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
@@ -1489,92 +2038,80 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
-/* PyCFunctionFastCall.proto */
-#if CYTHON_FAST_PYCCALL
-static CYTHON_INLINE PyObject *__Pyx_PyCFunction_FastCall(PyObject *func, PyObject **args, Py_ssize_t nargs);
-#else
-#define __Pyx_PyCFunction_FastCall(func, args, nargs)  (assert(0), NULL)
-#endif
-
 /* PyFunctionFastCall.proto */
 #if CYTHON_FAST_PYCALL
+#if !CYTHON_VECTORCALL
 #define __Pyx_PyFunction_FastCall(func, args, nargs)\
     __Pyx_PyFunction_FastCallDict((func), (args), (nargs), NULL)
-#if 1 || PY_VERSION_HEX < 0x030600B1
 static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs);
-#else
-#define __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs) _PyFunction_FastCallDict(func, args, nargs, kwargs)
 #endif
 #define __Pyx_BUILD_ASSERT_EXPR(cond)\
     (sizeof(char [1 - 2*!(cond)]) - 1)
 #ifndef Py_MEMBER_SIZE
 #define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
 #endif
-#if CYTHON_FAST_PYCALL
-  static size_t __pyx_pyframe_localsplus_offset = 0;
+#if !CYTHON_VECTORCALL
+#if PY_VERSION_HEX >= 0x03080000
   #include "frameobject.h"
 #if PY_VERSION_HEX >= 0x030b00a6
   #ifndef Py_BUILD_CORE
     #define Py_BUILD_CORE 1
   #endif
   #include "internal/pycore_frame.h"
 #endif
+  #define __Pxy_PyFrame_Initialize_Offsets()
+  #define __Pyx_PyFrame_GetLocalsplus(frame)  ((frame)->f_localsplus)
+#else
+  static size_t __pyx_pyframe_localsplus_offset = 0;
+  #include "frameobject.h"
   #define __Pxy_PyFrame_Initialize_Offsets()\
     ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
      (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
   #define __Pyx_PyFrame_GetLocalsplus(frame)\
     (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
-#endif // CYTHON_FAST_PYCALL
 #endif
-
-/* PyObjectCall.proto */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw);
-#else
-#define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
 #endif
-
-/* PyObjectCall2Args.proto */
-static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2);
+#endif
 
 /* PyObjectCallMethO.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg);
 #endif
 
-/* PyObjectCallOneArg.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg);
+/* PyObjectFastCall.proto */
+#define __Pyx_PyObject_FastCall(func, args, nargs)  __Pyx_PyObject_FastCallDict(func, args, (size_t)(nargs), NULL)
+static CYTHON_INLINE PyObject* __Pyx_PyObject_FastCallDict(PyObject *func, PyObject **args, size_t nargs, PyObject *kwargs);
 
 /* ArgTypeTest.proto */
 #define __Pyx_ArgTypeTest(obj, type, none_allowed, name, exact)\
-    ((likely((Py_TYPE(obj) == type) | (none_allowed && (obj == Py_None)))) ? 1 :\
+    ((likely(__Pyx_IS_TYPE(obj, type) | (none_allowed && (obj == Py_None)))) ? 1 :\
         __Pyx__ArgTypeTest(obj, type, name, exact))
 static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact);
 
 /* IsLittleEndian.proto */
 static CYTHON_INLINE int __Pyx_Is_Little_Endian(void);
 
 /* BufferFormatCheck.proto */
@@ -1601,133 +2138,192 @@
 /* BufferFallbackError.proto */
 static void __Pyx_RaiseBufferFallbackError(void);
 
 /* BufferIndexError.proto */
 static void __Pyx_RaiseBufferIndexError(int axis);
 
 #define __Pyx_BufPtrStrided1d(type, buf, i0, s0) (type)((char*)buf + i0 * s0)
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
+#define __Pyx_BufPtrStrided2d(type, buf, i0, s0, i1, s1) (type)((char*)buf + i0 * s0 + i1 * s1)
+/* TypeImport.proto */
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_0
+#define __PYX_HAVE_RT_ImportType_proto_3_0_0
+#if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_0(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_0(s) sizeof(void*)
+#endif
+enum __Pyx_ImportType_CheckSize_3_0_0 {
+   __Pyx_ImportType_CheckSize_Error_3_0_0 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_0 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_0 = 2
+};
+static PyTypeObject *__Pyx_ImportType_3_0_0(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_0 check_size);
 #endif
 
-#define __Pyx_BufPtrStrided2d(type, buf, i0, s0, i1, s1) (type)((char*)buf + i0 * s0 + i1 * s1)
-/* RaiseArgTupleInvalid.proto */
-static void __Pyx_RaiseArgtupleInvalid(const char* func_name, int exact,
-    Py_ssize_t num_min, Py_ssize_t num_max, Py_ssize_t num_found);
+/* Import.proto */
+static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
-/* RaiseDoubleKeywords.proto */
-static void __Pyx_RaiseDoubleKeywordsError(const char* func_name, PyObject* kw_name);
+/* ImportDottedModule.proto */
+static PyObject *__Pyx_ImportDottedModule(PyObject *name, PyObject *parts_tuple);
+#if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx_ImportDottedModule_WalkParts(PyObject *module, PyObject *name, PyObject *parts_tuple);
+#endif
 
-/* ParseKeywords.proto */
-static int __Pyx_ParseOptionalKeywords(PyObject *kwds, PyObject **argnames[],\
-    PyObject *kwds2, PyObject *values[], Py_ssize_t num_pos_args,\
-    const char* function_name);
+/* IncludeStructmemberH.proto */
+#include <structmember.h>
 
-/* GetTopmostException.proto */
-#if CYTHON_USE_EXC_INFO_STACK
-static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
+/* FixUpExtensionType.proto */
+#if CYTHON_USE_TYPE_SPECS
+static int __Pyx_fix_up_extension_type_from_spec(PyType_Spec *spec, PyTypeObject *type);
 #endif
 
-/* SaveResetException.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_ExceptionSave(type, value, tb)  __Pyx__ExceptionSave(__pyx_tstate, type, value, tb)
-static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
-#define __Pyx_ExceptionReset(type, value, tb)  __Pyx__ExceptionReset(__pyx_tstate, type, value, tb)
-static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
-#else
-#define __Pyx_ExceptionSave(type, value, tb)   PyErr_GetExcInfo(type, value, tb)
-#define __Pyx_ExceptionReset(type, value, tb)  PyErr_SetExcInfo(type, value, tb)
-#endif
+/* FetchSharedCythonModule.proto */
+static PyObject *__Pyx_FetchSharedCythonABIModule(void);
 
-/* PyErrExceptionMatches.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_PyErr_ExceptionMatches(err) __Pyx_PyErr_ExceptionMatchesInState(__pyx_tstate, err)
-static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err);
+/* FetchCommonType.proto */
+#if !CYTHON_USE_TYPE_SPECS
+static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type);
 #else
-#define __Pyx_PyErr_ExceptionMatches(err)  PyErr_ExceptionMatches(err)
+static PyTypeObject* __Pyx_FetchCommonTypeFromSpec(PyObject *module, PyType_Spec *spec, PyObject *bases);
 #endif
 
-/* GetException.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_GetException(type, value, tb)  __Pyx__GetException(__pyx_tstate, type, value, tb)
-static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
+/* PyMethodNew.proto */
+#if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx_PyMethod_New(PyObject *func, PyObject *self, PyObject *typ) {
+    CYTHON_UNUSED_VAR(typ);
+    if (!self)
+        return __Pyx_NewRef(func);
+    return PyMethod_New(func, self);
+}
+#else
+    #define __Pyx_PyMethod_New PyMethod_New
+#endif
+
+/* PyVectorcallFastCallDict.proto */
+#if CYTHON_METH_FASTCALL
+static CYTHON_INLINE PyObject *__Pyx_PyVectorcall_FastCallDict(PyObject *func, __pyx_vectorcallfunc vc, PyObject *const *args, size_t nargs, PyObject *kw);
+#endif
+
+/* CythonFunctionShared.proto */
+#define __Pyx_CyFunction_USED
+#define __Pyx_CYFUNCTION_STATICMETHOD  0x01
+#define __Pyx_CYFUNCTION_CLASSMETHOD   0x02
+#define __Pyx_CYFUNCTION_CCLASS        0x04
+#define __Pyx_CYFUNCTION_COROUTINE     0x08
+#define __Pyx_CyFunction_GetClosure(f)\
+    (((__pyx_CyFunctionObject *) (f))->func_closure)
+#if PY_VERSION_HEX < 0x030900B1
+  #define __Pyx_CyFunction_GetClassObj(f)\
+      (((__pyx_CyFunctionObject *) (f))->func_classobj)
+#else
+  #define __Pyx_CyFunction_GetClassObj(f)\
+      ((PyObject*) ((PyCMethodObject *) (f))->mm_class)
+#endif
+#define __Pyx_CyFunction_SetClassObj(f, classobj)\
+    __Pyx__CyFunction_SetClassObj((__pyx_CyFunctionObject *) (f), (classobj))
+#define __Pyx_CyFunction_Defaults(type, f)\
+    ((type *)(((__pyx_CyFunctionObject *) (f))->defaults))
+#define __Pyx_CyFunction_SetDefaultsGetter(f, g)\
+    ((__pyx_CyFunctionObject *) (f))->defaults_getter = (g)
+typedef struct {
+#if PY_VERSION_HEX < 0x030900B1
+    PyCFunctionObject func;
 #else
-static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb);
+    PyCMethodObject func;
 #endif
-
-/* RaiseException.proto */
-static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
-
-/* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
-};
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+#if CYTHON_BACKPORT_VECTORCALL
+    __pyx_vectorcallfunc func_vectorcall;
 #endif
-
-/* Import.proto */
-static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
+#if PY_VERSION_HEX < 0x030500A0
+    PyObject *func_weakreflist;
+#endif
+    PyObject *func_dict;
+    PyObject *func_name;
+    PyObject *func_qualname;
+    PyObject *func_doc;
+    PyObject *func_globals;
+    PyObject *func_code;
+    PyObject *func_closure;
+#if PY_VERSION_HEX < 0x030900B1
+    PyObject *func_classobj;
+#endif
+    void *defaults;
+    int defaults_pyobjects;
+    size_t defaults_size;  // used by FusedFunction for copying defaults
+    int flags;
+    PyObject *defaults_tuple;
+    PyObject *defaults_kwdict;
+    PyObject *(*defaults_getter)(PyObject *);
+    PyObject *func_annotations;
+    PyObject *func_is_coroutine;
+} __pyx_CyFunctionObject;
+#define __Pyx_CyFunction_Check(obj)  __Pyx_TypeCheck(obj, __pyx_CyFunctionType)
+#define __Pyx_IsCyOrPyCFunction(obj)  __Pyx_TypeCheck2(obj, __pyx_CyFunctionType, &PyCFunction_Type)
+#define __Pyx_CyFunction_CheckExact(obj)  __Pyx_IS_TYPE(obj, __pyx_CyFunctionType)
+static PyObject *__Pyx_CyFunction_Init(__pyx_CyFunctionObject* op, PyMethodDef *ml,
+                                      int flags, PyObject* qualname,
+                                      PyObject *closure,
+                                      PyObject *module, PyObject *globals,
+                                      PyObject* code);
+static CYTHON_INLINE void __Pyx__CyFunction_SetClassObj(__pyx_CyFunctionObject* f, PyObject* classobj);
+static CYTHON_INLINE void *__Pyx_CyFunction_InitDefaults(PyObject *m,
+                                                         size_t size,
+                                                         int pyobjects);
+static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsTuple(PyObject *m,
+                                                            PyObject *tuple);
+static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsKwDict(PyObject *m,
+                                                             PyObject *dict);
+static CYTHON_INLINE void __Pyx_CyFunction_SetAnnotationsDict(PyObject *m,
+                                                              PyObject *dict);
+static int __pyx_CyFunction_init(PyObject *module);
+#if CYTHON_METH_FASTCALL
+static PyObject * __Pyx_CyFunction_Vectorcall_NOARGS(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames);
+static PyObject * __Pyx_CyFunction_Vectorcall_O(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames);
+static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames);
+static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames);
+#if CYTHON_BACKPORT_VECTORCALL
+#define __Pyx_CyFunction_func_vectorcall(f) (((__pyx_CyFunctionObject*)f)->func_vectorcall)
+#else
+#define __Pyx_CyFunction_func_vectorcall(f) (((PyCFunctionObject*)f)->vectorcall)
+#endif
+#endif
+
+/* CythonFunction.proto */
+static PyObject *__Pyx_CyFunction_New(PyMethodDef *ml,
+                                      int flags, PyObject* qualname,
+                                      PyObject *closure,
+                                      PyObject *module, PyObject *globals,
+                                      PyObject* code);
 
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
 #define __Pyx_CLineForTraceback(tstate, c_line)  (((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0)
 #else
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line);
 #endif
 
 /* CodeObjectCache.proto */
+#if !CYTHON_COMPILING_IN_LIMITED_API
 typedef struct {
     PyCodeObject* code_object;
     int code_line;
 } __Pyx_CodeObjectCacheEntry;
 struct __Pyx_CodeObjectCache {
     int count;
     int max_count;
     __Pyx_CodeObjectCacheEntry* entries;
 };
 static struct __Pyx_CodeObjectCache __pyx_code_cache = {0,0,NULL};
 static int __pyx_bisect_code_objects(__Pyx_CodeObjectCacheEntry* entries, int count, int code_line);
 static PyCodeObject *__pyx_find_code_object(int code_line);
 static void __pyx_insert_code_object(int code_line, PyCodeObject* code_object);
+#endif
 
 /* AddTraceback.proto */
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename);
 
 /* BufferStructDeclare.proto */
 typedef struct {
@@ -1749,15 +2345,15 @@
 #else
     #define __Pyx_GetBuffer PyObject_GetBuffer
     #define __Pyx_ReleaseBuffer PyBuffer_Release
 #endif
 
 
 /* GCCDiagnostics.proto */
-#if defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
+#if !defined(__INTEL_COMPILER) && defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
 #define __Pyx_HAS_GCC_DIAGNOSTIC
 #endif
 
 /* RealImag.proto */
 #if CYTHON_CCOMPLEX
   #ifdef __cplusplus
     #define __Pyx_CREAL(z) ((z).real())
@@ -1776,15 +2372,15 @@
     #define __Pyx_SET_CIMAG(z,y) ((z).imag(y))
 #else
     #define __Pyx_SET_CREAL(z,x) __Pyx_CREAL(z) = (x)
     #define __Pyx_SET_CIMAG(z,y) __Pyx_CIMAG(z) = (y)
 #endif
 
 /* Arithmetic.proto */
-#if CYTHON_CCOMPLEX
+#if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
     #define __Pyx_c_eq_float(a, b)   ((a)==(b))
     #define __Pyx_c_sum_float(a, b)  ((a)+(b))
     #define __Pyx_c_diff_float(a, b) ((a)-(b))
     #define __Pyx_c_prod_float(a, b) ((a)*(b))
     #define __Pyx_c_quot_float(a, b) ((a)/(b))
     #define __Pyx_c_neg_float(a)     (-(a))
   #ifdef __cplusplus
@@ -1814,15 +2410,15 @@
     #if 1
         static CYTHON_INLINE float __Pyx_c_abs_float(__pyx_t_float_complex);
         static CYTHON_INLINE __pyx_t_float_complex __Pyx_c_pow_float(__pyx_t_float_complex, __pyx_t_float_complex);
     #endif
 #endif
 
 /* Arithmetic.proto */
-#if CYTHON_CCOMPLEX
+#if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
     #define __Pyx_c_eq_double(a, b)   ((a)==(b))
     #define __Pyx_c_sum_double(a, b)  ((a)+(b))
     #define __Pyx_c_diff_double(a, b) ((a)-(b))
     #define __Pyx_c_prod_double(a, b) ((a)*(b))
     #define __Pyx_c_quot_double(a, b) ((a)/(b))
     #define __Pyx_c_neg_double(a)     (-(a))
   #ifdef __cplusplus
@@ -1854,107 +2450,121 @@
         static CYTHON_INLINE __pyx_t_double_complex __Pyx_c_pow_double(__pyx_t_double_complex, __pyx_t_double_complex);
     #endif
 #endif
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
 
+/* FormatTypeName.proto */
+#if CYTHON_COMPILING_IN_LIMITED_API
+typedef PyObject *__Pyx_TypeName;
+#define __Pyx_FMT_TYPENAME "%U"
+static __Pyx_TypeName __Pyx_PyType_GetName(PyTypeObject* tp);
+#define __Pyx_DECREF_TypeName(obj) Py_XDECREF(obj)
+#else
+typedef const char *__Pyx_TypeName;
+#define __Pyx_FMT_TYPENAME "%.200s"
+#define __Pyx_PyType_GetName(tp) ((tp)->tp_name)
+#define __Pyx_DECREF_TypeName(obj)
+#endif
+
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *);
 
 /* FastTypeChecks.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 #define __Pyx_TypeCheck(obj, type) __Pyx_IsSubtype(Py_TYPE(obj), (PyTypeObject *)type)
+#define __Pyx_TypeCheck2(obj, type1, type2) __Pyx_IsAnySubtype2(Py_TYPE(obj), (PyTypeObject *)type1, (PyTypeObject *)type2)
 static CYTHON_INLINE int __Pyx_IsSubtype(PyTypeObject *a, PyTypeObject *b);
+static CYTHON_INLINE int __Pyx_IsAnySubtype2(PyTypeObject *cls, PyTypeObject *a, PyTypeObject *b);
 static CYTHON_INLINE int __Pyx_PyErr_GivenExceptionMatches(PyObject *err, PyObject *type);
 static CYTHON_INLINE int __Pyx_PyErr_GivenExceptionMatches2(PyObject *err, PyObject *type1, PyObject *type2);
 #else
 #define __Pyx_TypeCheck(obj, type) PyObject_TypeCheck(obj, (PyTypeObject *)type)
+#define __Pyx_TypeCheck2(obj, type1, type2) (PyObject_TypeCheck(obj, (PyTypeObject *)type1) || PyObject_TypeCheck(obj, (PyTypeObject *)type2))
 #define __Pyx_PyErr_GivenExceptionMatches(err, type) PyErr_GivenExceptionMatches(err, type)
 #define __Pyx_PyErr_GivenExceptionMatches2(err, type1, type2) (PyErr_GivenExceptionMatches(err, type1) || PyErr_GivenExceptionMatches(err, type2))
 #endif
+#define __Pyx_PyErr_ExceptionMatches2(err1, err2)  __Pyx_PyErr_GivenExceptionMatches2(__Pyx_PyErr_CurrentExceptionType(), err1, err2)
 #define __Pyx_PyException_Check(obj) __Pyx_TypeCheck(obj, PyExc_Exception)
 
 /* CheckBinaryVersion.proto */
 static int __Pyx_check_binary_version(void);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
+/* #### Code section: module_declarations ### */
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self); /* proto*/
+static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self); /* proto*/
+static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self); /* proto*/
+static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self); /* proto*/
+static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self); /* proto*/
+static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self); /* proto*/
+static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self); /* proto*/
 
-/* Module declarations from 'cpython.buffer' */
-
-/* Module declarations from 'libc.string' */
+/* Module declarations from "libc.string" */
 
-/* Module declarations from 'libc.stdio' */
+/* Module declarations from "libc.stdio" */
 
-/* Module declarations from '__builtin__' */
+/* Module declarations from "__builtin__" */
 
-/* Module declarations from 'cpython.type' */
-static PyTypeObject *__pyx_ptype_7cpython_4type_type = 0;
+/* Module declarations from "cpython.type" */
 
-/* Module declarations from 'cpython' */
+/* Module declarations from "cpython" */
 
-/* Module declarations from 'cpython.object' */
+/* Module declarations from "cpython.object" */
 
-/* Module declarations from 'cpython.ref' */
+/* Module declarations from "cpython.ref" */
 
-/* Module declarations from 'cpython.mem' */
+/* Module declarations from "numpy" */
 
-/* Module declarations from 'numpy' */
+/* Module declarations from "numpy" */
 
-/* Module declarations from 'numpy' */
-static PyTypeObject *__pyx_ptype_5numpy_dtype = 0;
-static PyTypeObject *__pyx_ptype_5numpy_flatiter = 0;
-static PyTypeObject *__pyx_ptype_5numpy_broadcast = 0;
-static PyTypeObject *__pyx_ptype_5numpy_ndarray = 0;
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
-static PyTypeObject *__pyx_ptype_5numpy_ufunc = 0;
+/* Module declarations from "libcpp.string" */
 
-/* Module declarations from 'libcpp.string' */
-
-/* Module declarations from 'arcticpy.wrapper' */
+/* Module declarations from "arcticpy.wrapper" */
 static CYTHON_INLINE PyObject *__pyx_convert_PyObject_string_to_py_std__in_string(std::string const &); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_convert_PyUnicode_string_to_py_std__in_string(std::string const &); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_convert_PyStr_string_to_py_std__in_string(std::string const &); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_convert_PyBytes_string_to_py_std__in_string(std::string const &); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_convert_PyByteArray_string_to_py_std__in_string(std::string const &); /*proto*/
+/* #### Code section: typeinfo ### */
 static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_5numpy_double_t = { "double_t", NULL, sizeof(__pyx_t_5numpy_double_t), { 0 }, 0, 'R', 0, 0 };
+/* #### Code section: before_global_var ### */
 #define __Pyx_MODULE_NAME "arcticpy.wrapper"
 extern int __pyx_module_is_main_arcticpy__wrapper;
 int __pyx_module_is_main_arcticpy__wrapper = 0;
 
-/* Implementation of 'arcticpy.wrapper' */
+/* Implementation of "arcticpy.wrapper" */
+/* #### Code section: global_var ### */
 static PyObject *__pyx_builtin_ImportError;
+/* #### Code section: string_decls ### */
+static const char __pyx_k__3[] = "*";
 static const char __pyx_k_np[] = "np";
+static const char __pyx_k__12[] = "?";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
+static const char __pyx_k_spec[] = "__spec__";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_array[] = "array";
 static const char __pyx_k_flags[] = "flags";
 static const char __pyx_k_image[] = "image";
 static const char __pyx_k_numpy[] = "numpy";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_iteration[] = "iteration";
 static const char __pyx_k_verbosity[] = "verbosity";
 static const char __pyx_k_cy_add_cti[] = "cy_add_cti";
 static const char __pyx_k_ImportError[] = "ImportError";
 static const char __pyx_k_C_CONTIGUOUS[] = "C_CONTIGUOUS";
+static const char __pyx_k_initializing[] = "_initializing";
+static const char __pyx_k_is_coroutine[] = "_is_coroutine";
 static const char __pyx_k_cy_print_array[] = "cy_print_array";
 static const char __pyx_k_serial_express[] = "serial_express";
 static const char __pyx_k_serial_n_pumps[] = "serial_n_pumps";
 static const char __pyx_k_serial_roe_type[] = "serial_roe_type";
 static const char __pyx_k_arcticpy_wrapper[] = "arcticpy.wrapper";
 static const char __pyx_k_check_contiguous[] = "check_contiguous";
 static const char __pyx_k_cy_print_version[] = "cy_print_version";
@@ -1964,14 +2574,15 @@
 static const char __pyx_k_ascontiguousarray[] = "ascontiguousarray";
 static const char __pyx_k_cy_print_array_2D[] = "cy_print_array_2D";
 static const char __pyx_k_cy_version_arctic[] = "cy_version_arctic";
 static const char __pyx_k_parallel_roe_type[] = "parallel_roe_type";
 static const char __pyx_k_serial_n_traps_ic[] = "serial_n_traps_ic";
 static const char __pyx_k_serial_n_traps_sc[] = "serial_n_traps_sc";
 static const char __pyx_k_serial_time_start[] = "serial_time_start";
+static const char __pyx_k_asyncio_coroutines[] = "asyncio.coroutines";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_parallel_time_stop[] = "parallel_time_stop";
 static const char __pyx_k_serial_dwell_times[] = "serial_dwell_times";
 static const char __pyx_k_serial_window_stop[] = "serial_window_stop";
 static const char __pyx_k_parallel_n_traps_ic[] = "parallel_n_traps_ic";
 static const char __pyx_k_parallel_n_traps_sc[] = "parallel_n_traps_sc";
 static const char __pyx_k_parallel_time_start[] = "parallel_time_start";
@@ -2019,132 +2630,2181 @@
 static const char __pyx_k_parallel_trap_release_timescales[] = "parallel_trap_release_timescales";
 static const char __pyx_k_parallel_use_integer_express_mat[] = "parallel_use_integer_express_matrix";
 static const char __pyx_k_serial_empty_traps_between_colum[] = "serial_empty_traps_between_columns";
 static const char __pyx_k_serial_empty_traps_for_first_tra[] = "serial_empty_traps_for_first_transfers";
 static const char __pyx_k_serial_force_release_away_from_r[] = "serial_force_release_away_from_readout";
 static const char __pyx_k_serial_fraction_of_traps_per_pha[] = "serial_fraction_of_traps_per_phase";
 static const char __pyx_k_serial_use_integer_express_matri[] = "serial_use_integer_express_matrix";
-static PyObject *__pyx_n_u_C_CONTIGUOUS;
-static PyObject *__pyx_n_s_ImportError;
-static PyObject *__pyx_n_s_allow_negative_pixels;
-static PyObject *__pyx_n_s_arcticpy_wrapper;
-static PyObject *__pyx_n_s_array;
-static PyObject *__pyx_n_s_ascontiguousarray;
-static PyObject *__pyx_n_s_check_contiguous;
-static PyObject *__pyx_n_s_cline_in_traceback;
-static PyObject *__pyx_n_s_cy_add_cti;
-static PyObject *__pyx_n_s_cy_print_array;
-static PyObject *__pyx_n_s_cy_print_array_2D;
-static PyObject *__pyx_n_s_cy_print_version;
-static PyObject *__pyx_n_s_cy_version_arctic;
-static PyObject *__pyx_n_s_flags;
-static PyObject *__pyx_n_s_image;
-static PyObject *__pyx_n_s_import;
-static PyObject *__pyx_n_s_iteration;
-static PyObject *__pyx_n_s_main;
-static PyObject *__pyx_n_s_name;
-static PyObject *__pyx_n_s_np;
-static PyObject *__pyx_n_s_numpy;
-static PyObject *__pyx_kp_u_numpy_core_multiarray_failed_to;
-static PyObject *__pyx_kp_u_numpy_core_umath_failed_to_impor;
-static PyObject *__pyx_n_s_parallel_dwell_times;
-static PyObject *__pyx_n_s_parallel_empty_traps_between_col;
-static PyObject *__pyx_n_s_parallel_empty_traps_for_first_t;
-static PyObject *__pyx_n_s_parallel_express;
-static PyObject *__pyx_n_s_parallel_first_electron_fills;
-static PyObject *__pyx_n_s_parallel_force_release_away_from;
-static PyObject *__pyx_n_s_parallel_fraction_of_traps_per_p;
-static PyObject *__pyx_n_s_parallel_full_well_depths;
-static PyObject *__pyx_n_s_parallel_n_pumps;
-static PyObject *__pyx_n_s_parallel_n_traps_ic;
-static PyObject *__pyx_n_s_parallel_n_traps_ic_co;
-static PyObject *__pyx_n_s_parallel_n_traps_sc;
-static PyObject *__pyx_n_s_parallel_n_traps_sc_co;
-static PyObject *__pyx_n_s_parallel_overscan_start;
-static PyObject *__pyx_n_s_parallel_prescan_offset;
-static PyObject *__pyx_n_s_parallel_prune_frequency;
-static PyObject *__pyx_n_s_parallel_prune_n_electrons;
-static PyObject *__pyx_n_s_parallel_roe_type;
-static PyObject *__pyx_n_s_parallel_time_start;
-static PyObject *__pyx_n_s_parallel_time_stop;
-static PyObject *__pyx_n_s_parallel_trap_densities;
-static PyObject *__pyx_n_s_parallel_trap_fourth_params;
-static PyObject *__pyx_n_s_parallel_trap_release_timescales;
-static PyObject *__pyx_n_s_parallel_trap_third_params;
-static PyObject *__pyx_n_s_parallel_use_integer_express_mat;
-static PyObject *__pyx_n_s_parallel_well_fill_powers;
-static PyObject *__pyx_n_s_parallel_well_notch_depths;
-static PyObject *__pyx_n_s_parallel_window_offset;
-static PyObject *__pyx_n_s_parallel_window_start;
-static PyObject *__pyx_n_s_parallel_window_stop;
-static PyObject *__pyx_kp_s_python_arcticpy_wrapper_pyx;
-static PyObject *__pyx_n_s_serial_dwell_times;
-static PyObject *__pyx_n_s_serial_empty_traps_between_colum;
-static PyObject *__pyx_n_s_serial_empty_traps_for_first_tra;
-static PyObject *__pyx_n_s_serial_express;
-static PyObject *__pyx_n_s_serial_first_electron_fills;
-static PyObject *__pyx_n_s_serial_force_release_away_from_r;
-static PyObject *__pyx_n_s_serial_fraction_of_traps_per_pha;
-static PyObject *__pyx_n_s_serial_full_well_depths;
-static PyObject *__pyx_n_s_serial_n_pumps;
-static PyObject *__pyx_n_s_serial_n_traps_ic;
-static PyObject *__pyx_n_s_serial_n_traps_ic_co;
-static PyObject *__pyx_n_s_serial_n_traps_sc;
-static PyObject *__pyx_n_s_serial_n_traps_sc_co;
-static PyObject *__pyx_n_s_serial_overscan_start;
-static PyObject *__pyx_n_s_serial_prescan_offset;
-static PyObject *__pyx_n_s_serial_prune_frequency;
-static PyObject *__pyx_n_s_serial_prune_n_electrons;
-static PyObject *__pyx_n_s_serial_roe_type;
-static PyObject *__pyx_n_s_serial_time_start;
-static PyObject *__pyx_n_s_serial_time_stop;
-static PyObject *__pyx_n_s_serial_trap_densities;
-static PyObject *__pyx_n_s_serial_trap_fourth_params;
-static PyObject *__pyx_n_s_serial_trap_release_timescales;
-static PyObject *__pyx_n_s_serial_trap_third_params;
-static PyObject *__pyx_n_s_serial_use_integer_express_matri;
-static PyObject *__pyx_n_s_serial_well_fill_powers;
-static PyObject *__pyx_n_s_serial_well_notch_depths;
-static PyObject *__pyx_n_s_serial_window_offset;
-static PyObject *__pyx_n_s_serial_window_start;
-static PyObject *__pyx_n_s_serial_window_stop;
-static PyObject *__pyx_n_s_test;
-static PyObject *__pyx_n_s_verbosity;
+/* #### Code section: decls ### */
 static PyObject *__pyx_pf_8arcticpy_7wrapper_cy_print_version(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_8arcticpy_7wrapper_2cy_version_arctic(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_8arcticpy_7wrapper_4check_contiguous(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_array); /* proto */
 static PyObject *__pyx_pf_8arcticpy_7wrapper_6cy_print_array(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_array); /* proto */
 static PyObject *__pyx_pf_8arcticpy_7wrapper_8cy_print_array_2D(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_array); /* proto */
 static PyObject *__pyx_pf_8arcticpy_7wrapper_10cy_add_cti(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_image, PyArrayObject *__pyx_v_parallel_dwell_times, int __pyx_v_parallel_prescan_offset, int __pyx_v_parallel_overscan_start, int __pyx_v_parallel_empty_traps_between_columns, int __pyx_v_parallel_empty_traps_for_first_transfers, int __pyx_v_parallel_force_release_away_from_readout, int __pyx_v_parallel_use_integer_express_matrix, int __pyx_v_parallel_n_pumps, int __pyx_v_parallel_roe_type, PyArrayObject *__pyx_v_parallel_fraction_of_traps_per_phase, PyArrayObject *__pyx_v_parallel_full_well_depths, PyArrayObject *__pyx_v_parallel_well_notch_depths, PyArrayObject *__pyx_v_parallel_well_fill_powers, PyArrayObject *__pyx_v_parallel_first_electron_fills, PyArrayObject *__pyx_v_parallel_trap_densities, PyArrayObject *__pyx_v_parallel_trap_release_timescales, PyArrayObject *__pyx_v_parallel_trap_third_params, PyArrayObject *__pyx_v_parallel_trap_fourth_params, int __pyx_v_parallel_n_traps_ic, int __pyx_v_parallel_n_traps_sc, int __pyx_v_parallel_n_traps_ic_co, int __pyx_v_parallel_n_traps_sc_co, int __pyx_v_parallel_express, int __pyx_v_parallel_window_offset, int __pyx_v_parallel_window_start, int __pyx_v_parallel_window_stop, int __pyx_v_parallel_time_start, int __pyx_v_parallel_time_stop, PyArrayObject *__pyx_v_parallel_prune_n_electrons, int __pyx_v_parallel_prune_frequency, PyArrayObject *__pyx_v_serial_dwell_times, int __pyx_v_serial_prescan_offset, int __pyx_v_serial_overscan_start, int __pyx_v_serial_empty_traps_between_columns, int __pyx_v_serial_empty_traps_for_first_transfers, int __pyx_v_serial_force_release_away_from_readout, int __pyx_v_serial_use_integer_express_matrix, int __pyx_v_serial_n_pumps, int __pyx_v_serial_roe_type, PyArrayObject *__pyx_v_serial_fraction_of_traps_per_phase, PyArrayObject *__pyx_v_serial_full_well_depths, PyArrayObject *__pyx_v_serial_well_notch_depths, PyArrayObject *__pyx_v_serial_well_fill_powers, PyArrayObject *__pyx_v_serial_first_electron_fills, PyArrayObject *__pyx_v_serial_trap_densities, PyArrayObject *__pyx_v_serial_trap_release_timescales, PyArrayObject *__pyx_v_serial_trap_third_params, PyArrayObject *__pyx_v_serial_trap_fourth_params, int __pyx_v_serial_n_traps_ic, int __pyx_v_serial_n_traps_sc, int __pyx_v_serial_n_traps_ic_co, int __pyx_v_serial_n_traps_sc_co, int __pyx_v_serial_express, int __pyx_v_serial_window_offset, int __pyx_v_serial_window_start, int __pyx_v_serial_window_stop, int __pyx_v_serial_time_start, int __pyx_v_serial_time_stop, PyArrayObject *__pyx_v_serial_prune_n_electrons, int __pyx_v_serial_prune_frequency, int __pyx_v_allow_negative_pixels, int __pyx_v_verbosity, int __pyx_v_iteration); /* proto */
-static PyObject *__pyx_tuple_;
-static PyObject *__pyx_tuple__2;
-static PyObject *__pyx_tuple__5;
-static PyObject *__pyx_tuple__7;
-static PyObject *__pyx_tuple__9;
-static PyObject *__pyx_tuple__11;
-static PyObject *__pyx_codeobj__3;
-static PyObject *__pyx_codeobj__4;
-static PyObject *__pyx_codeobj__6;
-static PyObject *__pyx_codeobj__8;
-static PyObject *__pyx_codeobj__10;
-static PyObject *__pyx_codeobj__12;
-/* Late includes */
+/* #### Code section: late_includes ### */
+/* #### Code section: module_state ### */
+typedef struct {
+  PyObject *__pyx_d;
+  PyObject *__pyx_b;
+  PyObject *__pyx_cython_runtime;
+  PyObject *__pyx_empty_tuple;
+  PyObject *__pyx_empty_bytes;
+  PyObject *__pyx_empty_unicode;
+  #ifdef __Pyx_CyFunction_USED
+  PyTypeObject *__pyx_CyFunctionType;
+  #endif
+  #ifdef __Pyx_FusedFunction_USED
+  PyTypeObject *__pyx_FusedFunctionType;
+  #endif
+  #ifdef __Pyx_Generator_USED
+  PyTypeObject *__pyx_GeneratorType;
+  #endif
+  #ifdef __Pyx_IterableCoroutine_USED
+  PyTypeObject *__pyx_IterableCoroutineType;
+  #endif
+  #ifdef __Pyx_Coroutine_USED
+  PyTypeObject *__pyx_CoroutineAwaitType;
+  #endif
+  #ifdef __Pyx_Coroutine_USED
+  PyTypeObject *__pyx_CoroutineType;
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  PyTypeObject *__pyx_ptype_7cpython_4type_type;
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  PyTypeObject *__pyx_ptype_5numpy_dtype;
+  PyTypeObject *__pyx_ptype_5numpy_flatiter;
+  PyTypeObject *__pyx_ptype_5numpy_broadcast;
+  PyTypeObject *__pyx_ptype_5numpy_ndarray;
+  PyTypeObject *__pyx_ptype_5numpy_generic;
+  PyTypeObject *__pyx_ptype_5numpy_number;
+  PyTypeObject *__pyx_ptype_5numpy_integer;
+  PyTypeObject *__pyx_ptype_5numpy_signedinteger;
+  PyTypeObject *__pyx_ptype_5numpy_unsignedinteger;
+  PyTypeObject *__pyx_ptype_5numpy_inexact;
+  PyTypeObject *__pyx_ptype_5numpy_floating;
+  PyTypeObject *__pyx_ptype_5numpy_complexfloating;
+  PyTypeObject *__pyx_ptype_5numpy_flexible;
+  PyTypeObject *__pyx_ptype_5numpy_character;
+  PyTypeObject *__pyx_ptype_5numpy_ufunc;
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  PyObject *__pyx_n_u_C_CONTIGUOUS;
+  PyObject *__pyx_n_s_ImportError;
+  PyObject *__pyx_n_s__12;
+  PyObject *__pyx_n_s__3;
+  PyObject *__pyx_n_s_allow_negative_pixels;
+  PyObject *__pyx_n_s_arcticpy_wrapper;
+  PyObject *__pyx_n_s_array;
+  PyObject *__pyx_n_s_ascontiguousarray;
+  PyObject *__pyx_n_s_asyncio_coroutines;
+  PyObject *__pyx_n_s_check_contiguous;
+  PyObject *__pyx_n_s_cline_in_traceback;
+  PyObject *__pyx_n_s_cy_add_cti;
+  PyObject *__pyx_n_s_cy_print_array;
+  PyObject *__pyx_n_s_cy_print_array_2D;
+  PyObject *__pyx_n_s_cy_print_version;
+  PyObject *__pyx_n_s_cy_version_arctic;
+  PyObject *__pyx_n_s_flags;
+  PyObject *__pyx_n_s_image;
+  PyObject *__pyx_n_s_import;
+  PyObject *__pyx_n_s_initializing;
+  PyObject *__pyx_n_s_is_coroutine;
+  PyObject *__pyx_n_s_iteration;
+  PyObject *__pyx_n_s_main;
+  PyObject *__pyx_n_s_name;
+  PyObject *__pyx_n_s_np;
+  PyObject *__pyx_n_s_numpy;
+  PyObject *__pyx_kp_u_numpy_core_multiarray_failed_to;
+  PyObject *__pyx_kp_u_numpy_core_umath_failed_to_impor;
+  PyObject *__pyx_n_s_parallel_dwell_times;
+  PyObject *__pyx_n_s_parallel_empty_traps_between_col;
+  PyObject *__pyx_n_s_parallel_empty_traps_for_first_t;
+  PyObject *__pyx_n_s_parallel_express;
+  PyObject *__pyx_n_s_parallel_first_electron_fills;
+  PyObject *__pyx_n_s_parallel_force_release_away_from;
+  PyObject *__pyx_n_s_parallel_fraction_of_traps_per_p;
+  PyObject *__pyx_n_s_parallel_full_well_depths;
+  PyObject *__pyx_n_s_parallel_n_pumps;
+  PyObject *__pyx_n_s_parallel_n_traps_ic;
+  PyObject *__pyx_n_s_parallel_n_traps_ic_co;
+  PyObject *__pyx_n_s_parallel_n_traps_sc;
+  PyObject *__pyx_n_s_parallel_n_traps_sc_co;
+  PyObject *__pyx_n_s_parallel_overscan_start;
+  PyObject *__pyx_n_s_parallel_prescan_offset;
+  PyObject *__pyx_n_s_parallel_prune_frequency;
+  PyObject *__pyx_n_s_parallel_prune_n_electrons;
+  PyObject *__pyx_n_s_parallel_roe_type;
+  PyObject *__pyx_n_s_parallel_time_start;
+  PyObject *__pyx_n_s_parallel_time_stop;
+  PyObject *__pyx_n_s_parallel_trap_densities;
+  PyObject *__pyx_n_s_parallel_trap_fourth_params;
+  PyObject *__pyx_n_s_parallel_trap_release_timescales;
+  PyObject *__pyx_n_s_parallel_trap_third_params;
+  PyObject *__pyx_n_s_parallel_use_integer_express_mat;
+  PyObject *__pyx_n_s_parallel_well_fill_powers;
+  PyObject *__pyx_n_s_parallel_well_notch_depths;
+  PyObject *__pyx_n_s_parallel_window_offset;
+  PyObject *__pyx_n_s_parallel_window_start;
+  PyObject *__pyx_n_s_parallel_window_stop;
+  PyObject *__pyx_kp_s_python_arcticpy_wrapper_pyx;
+  PyObject *__pyx_n_s_serial_dwell_times;
+  PyObject *__pyx_n_s_serial_empty_traps_between_colum;
+  PyObject *__pyx_n_s_serial_empty_traps_for_first_tra;
+  PyObject *__pyx_n_s_serial_express;
+  PyObject *__pyx_n_s_serial_first_electron_fills;
+  PyObject *__pyx_n_s_serial_force_release_away_from_r;
+  PyObject *__pyx_n_s_serial_fraction_of_traps_per_pha;
+  PyObject *__pyx_n_s_serial_full_well_depths;
+  PyObject *__pyx_n_s_serial_n_pumps;
+  PyObject *__pyx_n_s_serial_n_traps_ic;
+  PyObject *__pyx_n_s_serial_n_traps_ic_co;
+  PyObject *__pyx_n_s_serial_n_traps_sc;
+  PyObject *__pyx_n_s_serial_n_traps_sc_co;
+  PyObject *__pyx_n_s_serial_overscan_start;
+  PyObject *__pyx_n_s_serial_prescan_offset;
+  PyObject *__pyx_n_s_serial_prune_frequency;
+  PyObject *__pyx_n_s_serial_prune_n_electrons;
+  PyObject *__pyx_n_s_serial_roe_type;
+  PyObject *__pyx_n_s_serial_time_start;
+  PyObject *__pyx_n_s_serial_time_stop;
+  PyObject *__pyx_n_s_serial_trap_densities;
+  PyObject *__pyx_n_s_serial_trap_fourth_params;
+  PyObject *__pyx_n_s_serial_trap_release_timescales;
+  PyObject *__pyx_n_s_serial_trap_third_params;
+  PyObject *__pyx_n_s_serial_use_integer_express_matri;
+  PyObject *__pyx_n_s_serial_well_fill_powers;
+  PyObject *__pyx_n_s_serial_well_notch_depths;
+  PyObject *__pyx_n_s_serial_window_offset;
+  PyObject *__pyx_n_s_serial_window_start;
+  PyObject *__pyx_n_s_serial_window_stop;
+  PyObject *__pyx_n_s_spec;
+  PyObject *__pyx_n_s_test;
+  PyObject *__pyx_n_s_verbosity;
+  PyObject *__pyx_tuple_;
+  PyObject *__pyx_tuple__2;
+  PyObject *__pyx_tuple__6;
+  PyObject *__pyx_tuple__10;
+  PyObject *__pyx_codeobj__4;
+  PyObject *__pyx_codeobj__5;
+  PyObject *__pyx_codeobj__7;
+  PyObject *__pyx_codeobj__8;
+  PyObject *__pyx_codeobj__9;
+  PyObject *__pyx_codeobj__11;
+} __pyx_mstate;
+
+#if CYTHON_USE_MODULE_STATE
+#ifdef __cplusplus
+namespace {
+  extern struct PyModuleDef __pyx_moduledef;
+} /* anonymous namespace */
+#else
+static struct PyModuleDef __pyx_moduledef;
+#endif
+
+#define __pyx_mstate(o) ((__pyx_mstate *)__Pyx_PyModule_GetState(o))
+
+#define __pyx_mstate_global (__pyx_mstate(PyState_FindModule(&__pyx_moduledef)))
+
+#define __pyx_m (PyState_FindModule(&__pyx_moduledef))
+#else
+static __pyx_mstate __pyx_mstate_global_static =
+#ifdef __cplusplus
+    {};
+#else
+    {0};
+#endif
+static __pyx_mstate *__pyx_mstate_global = &__pyx_mstate_global_static;
+#endif
+/* #### Code section: module_state_clear ### */
+#if CYTHON_USE_MODULE_STATE
+static int __pyx_m_clear(PyObject *m) {
+  __pyx_mstate *clear_module_state = __pyx_mstate(m);
+  if (!clear_module_state) return 0;
+  Py_CLEAR(clear_module_state->__pyx_d);
+  Py_CLEAR(clear_module_state->__pyx_b);
+  Py_CLEAR(clear_module_state->__pyx_cython_runtime);
+  Py_CLEAR(clear_module_state->__pyx_empty_tuple);
+  Py_CLEAR(clear_module_state->__pyx_empty_bytes);
+  Py_CLEAR(clear_module_state->__pyx_empty_unicode);
+  #ifdef __Pyx_CyFunction_USED
+  Py_CLEAR(clear_module_state->__pyx_CyFunctionType);
+  #endif
+  #ifdef __Pyx_FusedFunction_USED
+  Py_CLEAR(clear_module_state->__pyx_FusedFunctionType);
+  #endif
+  Py_CLEAR(clear_module_state->__pyx_ptype_7cpython_4type_type);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_dtype);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_flatiter);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_broadcast);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_ndarray);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_generic);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_number);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_integer);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_signedinteger);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_unsignedinteger);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_inexact);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_floating);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_complexfloating);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_flexible);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_character);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_ufunc);
+  Py_CLEAR(clear_module_state->__pyx_n_u_C_CONTIGUOUS);
+  Py_CLEAR(clear_module_state->__pyx_n_s_ImportError);
+  Py_CLEAR(clear_module_state->__pyx_n_s__12);
+  Py_CLEAR(clear_module_state->__pyx_n_s__3);
+  Py_CLEAR(clear_module_state->__pyx_n_s_allow_negative_pixels);
+  Py_CLEAR(clear_module_state->__pyx_n_s_arcticpy_wrapper);
+  Py_CLEAR(clear_module_state->__pyx_n_s_array);
+  Py_CLEAR(clear_module_state->__pyx_n_s_ascontiguousarray);
+  Py_CLEAR(clear_module_state->__pyx_n_s_asyncio_coroutines);
+  Py_CLEAR(clear_module_state->__pyx_n_s_check_contiguous);
+  Py_CLEAR(clear_module_state->__pyx_n_s_cline_in_traceback);
+  Py_CLEAR(clear_module_state->__pyx_n_s_cy_add_cti);
+  Py_CLEAR(clear_module_state->__pyx_n_s_cy_print_array);
+  Py_CLEAR(clear_module_state->__pyx_n_s_cy_print_array_2D);
+  Py_CLEAR(clear_module_state->__pyx_n_s_cy_print_version);
+  Py_CLEAR(clear_module_state->__pyx_n_s_cy_version_arctic);
+  Py_CLEAR(clear_module_state->__pyx_n_s_flags);
+  Py_CLEAR(clear_module_state->__pyx_n_s_image);
+  Py_CLEAR(clear_module_state->__pyx_n_s_import);
+  Py_CLEAR(clear_module_state->__pyx_n_s_initializing);
+  Py_CLEAR(clear_module_state->__pyx_n_s_is_coroutine);
+  Py_CLEAR(clear_module_state->__pyx_n_s_iteration);
+  Py_CLEAR(clear_module_state->__pyx_n_s_main);
+  Py_CLEAR(clear_module_state->__pyx_n_s_name);
+  Py_CLEAR(clear_module_state->__pyx_n_s_np);
+  Py_CLEAR(clear_module_state->__pyx_n_s_numpy);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_numpy_core_multiarray_failed_to);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_numpy_core_umath_failed_to_impor);
+  Py_CLEAR(clear_module_state->__pyx_n_s_parallel_dwell_times);
+  Py_CLEAR(clear_module_state->__pyx_n_s_parallel_empty_traps_between_col);
+  Py_CLEAR(clear_module_state->__pyx_n_s_parallel_empty_traps_for_first_t);
+  Py_CLEAR(clear_module_state->__pyx_n_s_parallel_express);
+  Py_CLEAR(clear_module_state->__pyx_n_s_parallel_first_electron_fills);
+  Py_CLEAR(clear_module_state->__pyx_n_s_parallel_force_release_away_from);
+  Py_CLEAR(clear_module_state->__pyx_n_s_parallel_fraction_of_traps_per_p);
+  Py_CLEAR(clear_module_state->__pyx_n_s_parallel_full_well_depths);
+  Py_CLEAR(clear_module_state->__pyx_n_s_parallel_n_pumps);
+  Py_CLEAR(clear_module_state->__pyx_n_s_parallel_n_traps_ic);
+  Py_CLEAR(clear_module_state->__pyx_n_s_parallel_n_traps_ic_co);
+  Py_CLEAR(clear_module_state->__pyx_n_s_parallel_n_traps_sc);
+  Py_CLEAR(clear_module_state->__pyx_n_s_parallel_n_traps_sc_co);
+  Py_CLEAR(clear_module_state->__pyx_n_s_parallel_overscan_start);
+  Py_CLEAR(clear_module_state->__pyx_n_s_parallel_prescan_offset);
+  Py_CLEAR(clear_module_state->__pyx_n_s_parallel_prune_frequency);
+  Py_CLEAR(clear_module_state->__pyx_n_s_parallel_prune_n_electrons);
+  Py_CLEAR(clear_module_state->__pyx_n_s_parallel_roe_type);
+  Py_CLEAR(clear_module_state->__pyx_n_s_parallel_time_start);
+  Py_CLEAR(clear_module_state->__pyx_n_s_parallel_time_stop);
+  Py_CLEAR(clear_module_state->__pyx_n_s_parallel_trap_densities);
+  Py_CLEAR(clear_module_state->__pyx_n_s_parallel_trap_fourth_params);
+  Py_CLEAR(clear_module_state->__pyx_n_s_parallel_trap_release_timescales);
+  Py_CLEAR(clear_module_state->__pyx_n_s_parallel_trap_third_params);
+  Py_CLEAR(clear_module_state->__pyx_n_s_parallel_use_integer_express_mat);
+  Py_CLEAR(clear_module_state->__pyx_n_s_parallel_well_fill_powers);
+  Py_CLEAR(clear_module_state->__pyx_n_s_parallel_well_notch_depths);
+  Py_CLEAR(clear_module_state->__pyx_n_s_parallel_window_offset);
+  Py_CLEAR(clear_module_state->__pyx_n_s_parallel_window_start);
+  Py_CLEAR(clear_module_state->__pyx_n_s_parallel_window_stop);
+  Py_CLEAR(clear_module_state->__pyx_kp_s_python_arcticpy_wrapper_pyx);
+  Py_CLEAR(clear_module_state->__pyx_n_s_serial_dwell_times);
+  Py_CLEAR(clear_module_state->__pyx_n_s_serial_empty_traps_between_colum);
+  Py_CLEAR(clear_module_state->__pyx_n_s_serial_empty_traps_for_first_tra);
+  Py_CLEAR(clear_module_state->__pyx_n_s_serial_express);
+  Py_CLEAR(clear_module_state->__pyx_n_s_serial_first_electron_fills);
+  Py_CLEAR(clear_module_state->__pyx_n_s_serial_force_release_away_from_r);
+  Py_CLEAR(clear_module_state->__pyx_n_s_serial_fraction_of_traps_per_pha);
+  Py_CLEAR(clear_module_state->__pyx_n_s_serial_full_well_depths);
+  Py_CLEAR(clear_module_state->__pyx_n_s_serial_n_pumps);
+  Py_CLEAR(clear_module_state->__pyx_n_s_serial_n_traps_ic);
+  Py_CLEAR(clear_module_state->__pyx_n_s_serial_n_traps_ic_co);
+  Py_CLEAR(clear_module_state->__pyx_n_s_serial_n_traps_sc);
+  Py_CLEAR(clear_module_state->__pyx_n_s_serial_n_traps_sc_co);
+  Py_CLEAR(clear_module_state->__pyx_n_s_serial_overscan_start);
+  Py_CLEAR(clear_module_state->__pyx_n_s_serial_prescan_offset);
+  Py_CLEAR(clear_module_state->__pyx_n_s_serial_prune_frequency);
+  Py_CLEAR(clear_module_state->__pyx_n_s_serial_prune_n_electrons);
+  Py_CLEAR(clear_module_state->__pyx_n_s_serial_roe_type);
+  Py_CLEAR(clear_module_state->__pyx_n_s_serial_time_start);
+  Py_CLEAR(clear_module_state->__pyx_n_s_serial_time_stop);
+  Py_CLEAR(clear_module_state->__pyx_n_s_serial_trap_densities);
+  Py_CLEAR(clear_module_state->__pyx_n_s_serial_trap_fourth_params);
+  Py_CLEAR(clear_module_state->__pyx_n_s_serial_trap_release_timescales);
+  Py_CLEAR(clear_module_state->__pyx_n_s_serial_trap_third_params);
+  Py_CLEAR(clear_module_state->__pyx_n_s_serial_use_integer_express_matri);
+  Py_CLEAR(clear_module_state->__pyx_n_s_serial_well_fill_powers);
+  Py_CLEAR(clear_module_state->__pyx_n_s_serial_well_notch_depths);
+  Py_CLEAR(clear_module_state->__pyx_n_s_serial_window_offset);
+  Py_CLEAR(clear_module_state->__pyx_n_s_serial_window_start);
+  Py_CLEAR(clear_module_state->__pyx_n_s_serial_window_stop);
+  Py_CLEAR(clear_module_state->__pyx_n_s_spec);
+  Py_CLEAR(clear_module_state->__pyx_n_s_test);
+  Py_CLEAR(clear_module_state->__pyx_n_s_verbosity);
+  Py_CLEAR(clear_module_state->__pyx_tuple_);
+  Py_CLEAR(clear_module_state->__pyx_tuple__2);
+  Py_CLEAR(clear_module_state->__pyx_tuple__6);
+  Py_CLEAR(clear_module_state->__pyx_tuple__10);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__4);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__5);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__7);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__8);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__9);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__11);
+  return 0;
+}
+#endif
+/* #### Code section: module_state_traverse ### */
+#if CYTHON_USE_MODULE_STATE
+static int __pyx_m_traverse(PyObject *m, visitproc visit, void *arg) {
+  __pyx_mstate *traverse_module_state = __pyx_mstate(m);
+  if (!traverse_module_state) return 0;
+  Py_VISIT(traverse_module_state->__pyx_d);
+  Py_VISIT(traverse_module_state->__pyx_b);
+  Py_VISIT(traverse_module_state->__pyx_cython_runtime);
+  Py_VISIT(traverse_module_state->__pyx_empty_tuple);
+  Py_VISIT(traverse_module_state->__pyx_empty_bytes);
+  Py_VISIT(traverse_module_state->__pyx_empty_unicode);
+  #ifdef __Pyx_CyFunction_USED
+  Py_VISIT(traverse_module_state->__pyx_CyFunctionType);
+  #endif
+  #ifdef __Pyx_FusedFunction_USED
+  Py_VISIT(traverse_module_state->__pyx_FusedFunctionType);
+  #endif
+  Py_VISIT(traverse_module_state->__pyx_ptype_7cpython_4type_type);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_dtype);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_flatiter);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_broadcast);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_ndarray);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_generic);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_number);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_integer);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_signedinteger);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_unsignedinteger);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_inexact);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_floating);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_complexfloating);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_flexible);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_character);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_ufunc);
+  Py_VISIT(traverse_module_state->__pyx_n_u_C_CONTIGUOUS);
+  Py_VISIT(traverse_module_state->__pyx_n_s_ImportError);
+  Py_VISIT(traverse_module_state->__pyx_n_s__12);
+  Py_VISIT(traverse_module_state->__pyx_n_s__3);
+  Py_VISIT(traverse_module_state->__pyx_n_s_allow_negative_pixels);
+  Py_VISIT(traverse_module_state->__pyx_n_s_arcticpy_wrapper);
+  Py_VISIT(traverse_module_state->__pyx_n_s_array);
+  Py_VISIT(traverse_module_state->__pyx_n_s_ascontiguousarray);
+  Py_VISIT(traverse_module_state->__pyx_n_s_asyncio_coroutines);
+  Py_VISIT(traverse_module_state->__pyx_n_s_check_contiguous);
+  Py_VISIT(traverse_module_state->__pyx_n_s_cline_in_traceback);
+  Py_VISIT(traverse_module_state->__pyx_n_s_cy_add_cti);
+  Py_VISIT(traverse_module_state->__pyx_n_s_cy_print_array);
+  Py_VISIT(traverse_module_state->__pyx_n_s_cy_print_array_2D);
+  Py_VISIT(traverse_module_state->__pyx_n_s_cy_print_version);
+  Py_VISIT(traverse_module_state->__pyx_n_s_cy_version_arctic);
+  Py_VISIT(traverse_module_state->__pyx_n_s_flags);
+  Py_VISIT(traverse_module_state->__pyx_n_s_image);
+  Py_VISIT(traverse_module_state->__pyx_n_s_import);
+  Py_VISIT(traverse_module_state->__pyx_n_s_initializing);
+  Py_VISIT(traverse_module_state->__pyx_n_s_is_coroutine);
+  Py_VISIT(traverse_module_state->__pyx_n_s_iteration);
+  Py_VISIT(traverse_module_state->__pyx_n_s_main);
+  Py_VISIT(traverse_module_state->__pyx_n_s_name);
+  Py_VISIT(traverse_module_state->__pyx_n_s_np);
+  Py_VISIT(traverse_module_state->__pyx_n_s_numpy);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_numpy_core_multiarray_failed_to);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_numpy_core_umath_failed_to_impor);
+  Py_VISIT(traverse_module_state->__pyx_n_s_parallel_dwell_times);
+  Py_VISIT(traverse_module_state->__pyx_n_s_parallel_empty_traps_between_col);
+  Py_VISIT(traverse_module_state->__pyx_n_s_parallel_empty_traps_for_first_t);
+  Py_VISIT(traverse_module_state->__pyx_n_s_parallel_express);
+  Py_VISIT(traverse_module_state->__pyx_n_s_parallel_first_electron_fills);
+  Py_VISIT(traverse_module_state->__pyx_n_s_parallel_force_release_away_from);
+  Py_VISIT(traverse_module_state->__pyx_n_s_parallel_fraction_of_traps_per_p);
+  Py_VISIT(traverse_module_state->__pyx_n_s_parallel_full_well_depths);
+  Py_VISIT(traverse_module_state->__pyx_n_s_parallel_n_pumps);
+  Py_VISIT(traverse_module_state->__pyx_n_s_parallel_n_traps_ic);
+  Py_VISIT(traverse_module_state->__pyx_n_s_parallel_n_traps_ic_co);
+  Py_VISIT(traverse_module_state->__pyx_n_s_parallel_n_traps_sc);
+  Py_VISIT(traverse_module_state->__pyx_n_s_parallel_n_traps_sc_co);
+  Py_VISIT(traverse_module_state->__pyx_n_s_parallel_overscan_start);
+  Py_VISIT(traverse_module_state->__pyx_n_s_parallel_prescan_offset);
+  Py_VISIT(traverse_module_state->__pyx_n_s_parallel_prune_frequency);
+  Py_VISIT(traverse_module_state->__pyx_n_s_parallel_prune_n_electrons);
+  Py_VISIT(traverse_module_state->__pyx_n_s_parallel_roe_type);
+  Py_VISIT(traverse_module_state->__pyx_n_s_parallel_time_start);
+  Py_VISIT(traverse_module_state->__pyx_n_s_parallel_time_stop);
+  Py_VISIT(traverse_module_state->__pyx_n_s_parallel_trap_densities);
+  Py_VISIT(traverse_module_state->__pyx_n_s_parallel_trap_fourth_params);
+  Py_VISIT(traverse_module_state->__pyx_n_s_parallel_trap_release_timescales);
+  Py_VISIT(traverse_module_state->__pyx_n_s_parallel_trap_third_params);
+  Py_VISIT(traverse_module_state->__pyx_n_s_parallel_use_integer_express_mat);
+  Py_VISIT(traverse_module_state->__pyx_n_s_parallel_well_fill_powers);
+  Py_VISIT(traverse_module_state->__pyx_n_s_parallel_well_notch_depths);
+  Py_VISIT(traverse_module_state->__pyx_n_s_parallel_window_offset);
+  Py_VISIT(traverse_module_state->__pyx_n_s_parallel_window_start);
+  Py_VISIT(traverse_module_state->__pyx_n_s_parallel_window_stop);
+  Py_VISIT(traverse_module_state->__pyx_kp_s_python_arcticpy_wrapper_pyx);
+  Py_VISIT(traverse_module_state->__pyx_n_s_serial_dwell_times);
+  Py_VISIT(traverse_module_state->__pyx_n_s_serial_empty_traps_between_colum);
+  Py_VISIT(traverse_module_state->__pyx_n_s_serial_empty_traps_for_first_tra);
+  Py_VISIT(traverse_module_state->__pyx_n_s_serial_express);
+  Py_VISIT(traverse_module_state->__pyx_n_s_serial_first_electron_fills);
+  Py_VISIT(traverse_module_state->__pyx_n_s_serial_force_release_away_from_r);
+  Py_VISIT(traverse_module_state->__pyx_n_s_serial_fraction_of_traps_per_pha);
+  Py_VISIT(traverse_module_state->__pyx_n_s_serial_full_well_depths);
+  Py_VISIT(traverse_module_state->__pyx_n_s_serial_n_pumps);
+  Py_VISIT(traverse_module_state->__pyx_n_s_serial_n_traps_ic);
+  Py_VISIT(traverse_module_state->__pyx_n_s_serial_n_traps_ic_co);
+  Py_VISIT(traverse_module_state->__pyx_n_s_serial_n_traps_sc);
+  Py_VISIT(traverse_module_state->__pyx_n_s_serial_n_traps_sc_co);
+  Py_VISIT(traverse_module_state->__pyx_n_s_serial_overscan_start);
+  Py_VISIT(traverse_module_state->__pyx_n_s_serial_prescan_offset);
+  Py_VISIT(traverse_module_state->__pyx_n_s_serial_prune_frequency);
+  Py_VISIT(traverse_module_state->__pyx_n_s_serial_prune_n_electrons);
+  Py_VISIT(traverse_module_state->__pyx_n_s_serial_roe_type);
+  Py_VISIT(traverse_module_state->__pyx_n_s_serial_time_start);
+  Py_VISIT(traverse_module_state->__pyx_n_s_serial_time_stop);
+  Py_VISIT(traverse_module_state->__pyx_n_s_serial_trap_densities);
+  Py_VISIT(traverse_module_state->__pyx_n_s_serial_trap_fourth_params);
+  Py_VISIT(traverse_module_state->__pyx_n_s_serial_trap_release_timescales);
+  Py_VISIT(traverse_module_state->__pyx_n_s_serial_trap_third_params);
+  Py_VISIT(traverse_module_state->__pyx_n_s_serial_use_integer_express_matri);
+  Py_VISIT(traverse_module_state->__pyx_n_s_serial_well_fill_powers);
+  Py_VISIT(traverse_module_state->__pyx_n_s_serial_well_notch_depths);
+  Py_VISIT(traverse_module_state->__pyx_n_s_serial_window_offset);
+  Py_VISIT(traverse_module_state->__pyx_n_s_serial_window_start);
+  Py_VISIT(traverse_module_state->__pyx_n_s_serial_window_stop);
+  Py_VISIT(traverse_module_state->__pyx_n_s_spec);
+  Py_VISIT(traverse_module_state->__pyx_n_s_test);
+  Py_VISIT(traverse_module_state->__pyx_n_s_verbosity);
+  Py_VISIT(traverse_module_state->__pyx_tuple_);
+  Py_VISIT(traverse_module_state->__pyx_tuple__2);
+  Py_VISIT(traverse_module_state->__pyx_tuple__6);
+  Py_VISIT(traverse_module_state->__pyx_tuple__10);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__4);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__5);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__7);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__8);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__9);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__11);
+  return 0;
+}
+#endif
+/* #### Code section: module_state_defines ### */
+#define __pyx_d __pyx_mstate_global->__pyx_d
+#define __pyx_b __pyx_mstate_global->__pyx_b
+#define __pyx_cython_runtime __pyx_mstate_global->__pyx_cython_runtime
+#define __pyx_empty_tuple __pyx_mstate_global->__pyx_empty_tuple
+#define __pyx_empty_bytes __pyx_mstate_global->__pyx_empty_bytes
+#define __pyx_empty_unicode __pyx_mstate_global->__pyx_empty_unicode
+#ifdef __Pyx_CyFunction_USED
+#define __pyx_CyFunctionType __pyx_mstate_global->__pyx_CyFunctionType
+#endif
+#ifdef __Pyx_FusedFunction_USED
+#define __pyx_FusedFunctionType __pyx_mstate_global->__pyx_FusedFunctionType
+#endif
+#ifdef __Pyx_Generator_USED
+#define __pyx_GeneratorType __pyx_mstate_global->__pyx_GeneratorType
+#endif
+#ifdef __Pyx_IterableCoroutine_USED
+#define __pyx_IterableCoroutineType __pyx_mstate_global->__pyx_IterableCoroutineType
+#endif
+#ifdef __Pyx_Coroutine_USED
+#define __pyx_CoroutineAwaitType __pyx_mstate_global->__pyx_CoroutineAwaitType
+#endif
+#ifdef __Pyx_Coroutine_USED
+#define __pyx_CoroutineType __pyx_mstate_global->__pyx_CoroutineType
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#define __pyx_ptype_7cpython_4type_type __pyx_mstate_global->__pyx_ptype_7cpython_4type_type
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#define __pyx_ptype_5numpy_dtype __pyx_mstate_global->__pyx_ptype_5numpy_dtype
+#define __pyx_ptype_5numpy_flatiter __pyx_mstate_global->__pyx_ptype_5numpy_flatiter
+#define __pyx_ptype_5numpy_broadcast __pyx_mstate_global->__pyx_ptype_5numpy_broadcast
+#define __pyx_ptype_5numpy_ndarray __pyx_mstate_global->__pyx_ptype_5numpy_ndarray
+#define __pyx_ptype_5numpy_generic __pyx_mstate_global->__pyx_ptype_5numpy_generic
+#define __pyx_ptype_5numpy_number __pyx_mstate_global->__pyx_ptype_5numpy_number
+#define __pyx_ptype_5numpy_integer __pyx_mstate_global->__pyx_ptype_5numpy_integer
+#define __pyx_ptype_5numpy_signedinteger __pyx_mstate_global->__pyx_ptype_5numpy_signedinteger
+#define __pyx_ptype_5numpy_unsignedinteger __pyx_mstate_global->__pyx_ptype_5numpy_unsignedinteger
+#define __pyx_ptype_5numpy_inexact __pyx_mstate_global->__pyx_ptype_5numpy_inexact
+#define __pyx_ptype_5numpy_floating __pyx_mstate_global->__pyx_ptype_5numpy_floating
+#define __pyx_ptype_5numpy_complexfloating __pyx_mstate_global->__pyx_ptype_5numpy_complexfloating
+#define __pyx_ptype_5numpy_flexible __pyx_mstate_global->__pyx_ptype_5numpy_flexible
+#define __pyx_ptype_5numpy_character __pyx_mstate_global->__pyx_ptype_5numpy_character
+#define __pyx_ptype_5numpy_ufunc __pyx_mstate_global->__pyx_ptype_5numpy_ufunc
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#define __pyx_n_u_C_CONTIGUOUS __pyx_mstate_global->__pyx_n_u_C_CONTIGUOUS
+#define __pyx_n_s_ImportError __pyx_mstate_global->__pyx_n_s_ImportError
+#define __pyx_n_s__12 __pyx_mstate_global->__pyx_n_s__12
+#define __pyx_n_s__3 __pyx_mstate_global->__pyx_n_s__3
+#define __pyx_n_s_allow_negative_pixels __pyx_mstate_global->__pyx_n_s_allow_negative_pixels
+#define __pyx_n_s_arcticpy_wrapper __pyx_mstate_global->__pyx_n_s_arcticpy_wrapper
+#define __pyx_n_s_array __pyx_mstate_global->__pyx_n_s_array
+#define __pyx_n_s_ascontiguousarray __pyx_mstate_global->__pyx_n_s_ascontiguousarray
+#define __pyx_n_s_asyncio_coroutines __pyx_mstate_global->__pyx_n_s_asyncio_coroutines
+#define __pyx_n_s_check_contiguous __pyx_mstate_global->__pyx_n_s_check_contiguous
+#define __pyx_n_s_cline_in_traceback __pyx_mstate_global->__pyx_n_s_cline_in_traceback
+#define __pyx_n_s_cy_add_cti __pyx_mstate_global->__pyx_n_s_cy_add_cti
+#define __pyx_n_s_cy_print_array __pyx_mstate_global->__pyx_n_s_cy_print_array
+#define __pyx_n_s_cy_print_array_2D __pyx_mstate_global->__pyx_n_s_cy_print_array_2D
+#define __pyx_n_s_cy_print_version __pyx_mstate_global->__pyx_n_s_cy_print_version
+#define __pyx_n_s_cy_version_arctic __pyx_mstate_global->__pyx_n_s_cy_version_arctic
+#define __pyx_n_s_flags __pyx_mstate_global->__pyx_n_s_flags
+#define __pyx_n_s_image __pyx_mstate_global->__pyx_n_s_image
+#define __pyx_n_s_import __pyx_mstate_global->__pyx_n_s_import
+#define __pyx_n_s_initializing __pyx_mstate_global->__pyx_n_s_initializing
+#define __pyx_n_s_is_coroutine __pyx_mstate_global->__pyx_n_s_is_coroutine
+#define __pyx_n_s_iteration __pyx_mstate_global->__pyx_n_s_iteration
+#define __pyx_n_s_main __pyx_mstate_global->__pyx_n_s_main
+#define __pyx_n_s_name __pyx_mstate_global->__pyx_n_s_name
+#define __pyx_n_s_np __pyx_mstate_global->__pyx_n_s_np
+#define __pyx_n_s_numpy __pyx_mstate_global->__pyx_n_s_numpy
+#define __pyx_kp_u_numpy_core_multiarray_failed_to __pyx_mstate_global->__pyx_kp_u_numpy_core_multiarray_failed_to
+#define __pyx_kp_u_numpy_core_umath_failed_to_impor __pyx_mstate_global->__pyx_kp_u_numpy_core_umath_failed_to_impor
+#define __pyx_n_s_parallel_dwell_times __pyx_mstate_global->__pyx_n_s_parallel_dwell_times
+#define __pyx_n_s_parallel_empty_traps_between_col __pyx_mstate_global->__pyx_n_s_parallel_empty_traps_between_col
+#define __pyx_n_s_parallel_empty_traps_for_first_t __pyx_mstate_global->__pyx_n_s_parallel_empty_traps_for_first_t
+#define __pyx_n_s_parallel_express __pyx_mstate_global->__pyx_n_s_parallel_express
+#define __pyx_n_s_parallel_first_electron_fills __pyx_mstate_global->__pyx_n_s_parallel_first_electron_fills
+#define __pyx_n_s_parallel_force_release_away_from __pyx_mstate_global->__pyx_n_s_parallel_force_release_away_from
+#define __pyx_n_s_parallel_fraction_of_traps_per_p __pyx_mstate_global->__pyx_n_s_parallel_fraction_of_traps_per_p
+#define __pyx_n_s_parallel_full_well_depths __pyx_mstate_global->__pyx_n_s_parallel_full_well_depths
+#define __pyx_n_s_parallel_n_pumps __pyx_mstate_global->__pyx_n_s_parallel_n_pumps
+#define __pyx_n_s_parallel_n_traps_ic __pyx_mstate_global->__pyx_n_s_parallel_n_traps_ic
+#define __pyx_n_s_parallel_n_traps_ic_co __pyx_mstate_global->__pyx_n_s_parallel_n_traps_ic_co
+#define __pyx_n_s_parallel_n_traps_sc __pyx_mstate_global->__pyx_n_s_parallel_n_traps_sc
+#define __pyx_n_s_parallel_n_traps_sc_co __pyx_mstate_global->__pyx_n_s_parallel_n_traps_sc_co
+#define __pyx_n_s_parallel_overscan_start __pyx_mstate_global->__pyx_n_s_parallel_overscan_start
+#define __pyx_n_s_parallel_prescan_offset __pyx_mstate_global->__pyx_n_s_parallel_prescan_offset
+#define __pyx_n_s_parallel_prune_frequency __pyx_mstate_global->__pyx_n_s_parallel_prune_frequency
+#define __pyx_n_s_parallel_prune_n_electrons __pyx_mstate_global->__pyx_n_s_parallel_prune_n_electrons
+#define __pyx_n_s_parallel_roe_type __pyx_mstate_global->__pyx_n_s_parallel_roe_type
+#define __pyx_n_s_parallel_time_start __pyx_mstate_global->__pyx_n_s_parallel_time_start
+#define __pyx_n_s_parallel_time_stop __pyx_mstate_global->__pyx_n_s_parallel_time_stop
+#define __pyx_n_s_parallel_trap_densities __pyx_mstate_global->__pyx_n_s_parallel_trap_densities
+#define __pyx_n_s_parallel_trap_fourth_params __pyx_mstate_global->__pyx_n_s_parallel_trap_fourth_params
+#define __pyx_n_s_parallel_trap_release_timescales __pyx_mstate_global->__pyx_n_s_parallel_trap_release_timescales
+#define __pyx_n_s_parallel_trap_third_params __pyx_mstate_global->__pyx_n_s_parallel_trap_third_params
+#define __pyx_n_s_parallel_use_integer_express_mat __pyx_mstate_global->__pyx_n_s_parallel_use_integer_express_mat
+#define __pyx_n_s_parallel_well_fill_powers __pyx_mstate_global->__pyx_n_s_parallel_well_fill_powers
+#define __pyx_n_s_parallel_well_notch_depths __pyx_mstate_global->__pyx_n_s_parallel_well_notch_depths
+#define __pyx_n_s_parallel_window_offset __pyx_mstate_global->__pyx_n_s_parallel_window_offset
+#define __pyx_n_s_parallel_window_start __pyx_mstate_global->__pyx_n_s_parallel_window_start
+#define __pyx_n_s_parallel_window_stop __pyx_mstate_global->__pyx_n_s_parallel_window_stop
+#define __pyx_kp_s_python_arcticpy_wrapper_pyx __pyx_mstate_global->__pyx_kp_s_python_arcticpy_wrapper_pyx
+#define __pyx_n_s_serial_dwell_times __pyx_mstate_global->__pyx_n_s_serial_dwell_times
+#define __pyx_n_s_serial_empty_traps_between_colum __pyx_mstate_global->__pyx_n_s_serial_empty_traps_between_colum
+#define __pyx_n_s_serial_empty_traps_for_first_tra __pyx_mstate_global->__pyx_n_s_serial_empty_traps_for_first_tra
+#define __pyx_n_s_serial_express __pyx_mstate_global->__pyx_n_s_serial_express
+#define __pyx_n_s_serial_first_electron_fills __pyx_mstate_global->__pyx_n_s_serial_first_electron_fills
+#define __pyx_n_s_serial_force_release_away_from_r __pyx_mstate_global->__pyx_n_s_serial_force_release_away_from_r
+#define __pyx_n_s_serial_fraction_of_traps_per_pha __pyx_mstate_global->__pyx_n_s_serial_fraction_of_traps_per_pha
+#define __pyx_n_s_serial_full_well_depths __pyx_mstate_global->__pyx_n_s_serial_full_well_depths
+#define __pyx_n_s_serial_n_pumps __pyx_mstate_global->__pyx_n_s_serial_n_pumps
+#define __pyx_n_s_serial_n_traps_ic __pyx_mstate_global->__pyx_n_s_serial_n_traps_ic
+#define __pyx_n_s_serial_n_traps_ic_co __pyx_mstate_global->__pyx_n_s_serial_n_traps_ic_co
+#define __pyx_n_s_serial_n_traps_sc __pyx_mstate_global->__pyx_n_s_serial_n_traps_sc
+#define __pyx_n_s_serial_n_traps_sc_co __pyx_mstate_global->__pyx_n_s_serial_n_traps_sc_co
+#define __pyx_n_s_serial_overscan_start __pyx_mstate_global->__pyx_n_s_serial_overscan_start
+#define __pyx_n_s_serial_prescan_offset __pyx_mstate_global->__pyx_n_s_serial_prescan_offset
+#define __pyx_n_s_serial_prune_frequency __pyx_mstate_global->__pyx_n_s_serial_prune_frequency
+#define __pyx_n_s_serial_prune_n_electrons __pyx_mstate_global->__pyx_n_s_serial_prune_n_electrons
+#define __pyx_n_s_serial_roe_type __pyx_mstate_global->__pyx_n_s_serial_roe_type
+#define __pyx_n_s_serial_time_start __pyx_mstate_global->__pyx_n_s_serial_time_start
+#define __pyx_n_s_serial_time_stop __pyx_mstate_global->__pyx_n_s_serial_time_stop
+#define __pyx_n_s_serial_trap_densities __pyx_mstate_global->__pyx_n_s_serial_trap_densities
+#define __pyx_n_s_serial_trap_fourth_params __pyx_mstate_global->__pyx_n_s_serial_trap_fourth_params
+#define __pyx_n_s_serial_trap_release_timescales __pyx_mstate_global->__pyx_n_s_serial_trap_release_timescales
+#define __pyx_n_s_serial_trap_third_params __pyx_mstate_global->__pyx_n_s_serial_trap_third_params
+#define __pyx_n_s_serial_use_integer_express_matri __pyx_mstate_global->__pyx_n_s_serial_use_integer_express_matri
+#define __pyx_n_s_serial_well_fill_powers __pyx_mstate_global->__pyx_n_s_serial_well_fill_powers
+#define __pyx_n_s_serial_well_notch_depths __pyx_mstate_global->__pyx_n_s_serial_well_notch_depths
+#define __pyx_n_s_serial_window_offset __pyx_mstate_global->__pyx_n_s_serial_window_offset
+#define __pyx_n_s_serial_window_start __pyx_mstate_global->__pyx_n_s_serial_window_start
+#define __pyx_n_s_serial_window_stop __pyx_mstate_global->__pyx_n_s_serial_window_stop
+#define __pyx_n_s_spec __pyx_mstate_global->__pyx_n_s_spec
+#define __pyx_n_s_test __pyx_mstate_global->__pyx_n_s_test
+#define __pyx_n_s_verbosity __pyx_mstate_global->__pyx_n_s_verbosity
+#define __pyx_tuple_ __pyx_mstate_global->__pyx_tuple_
+#define __pyx_tuple__2 __pyx_mstate_global->__pyx_tuple__2
+#define __pyx_tuple__6 __pyx_mstate_global->__pyx_tuple__6
+#define __pyx_tuple__10 __pyx_mstate_global->__pyx_tuple__10
+#define __pyx_codeobj__4 __pyx_mstate_global->__pyx_codeobj__4
+#define __pyx_codeobj__5 __pyx_mstate_global->__pyx_codeobj__5
+#define __pyx_codeobj__7 __pyx_mstate_global->__pyx_codeobj__7
+#define __pyx_codeobj__8 __pyx_mstate_global->__pyx_codeobj__8
+#define __pyx_codeobj__9 __pyx_mstate_global->__pyx_codeobj__9
+#define __pyx_codeobj__11 __pyx_mstate_global->__pyx_codeobj__11
+/* #### Code section: module_code ### */
+
+/* "string.to_py":31
+ * 
+ * @cname("__pyx_convert_PyObject_string_to_py_std__in_string")
+ * cdef inline object __pyx_convert_PyObject_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
+ *     return __Pyx_PyObject_FromStringAndSize(s.data(), s.size())
+ * cdef extern from *:
+ */
+
+static CYTHON_INLINE PyObject *__pyx_convert_PyObject_string_to_py_std__in_string(std::string const &__pyx_v_s) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_convert_PyObject_string_to_py_std__in_string", 0);
+
+  /* "string.to_py":32
+ * @cname("__pyx_convert_PyObject_string_to_py_std__in_string")
+ * cdef inline object __pyx_convert_PyObject_string_to_py_std__in_string(const string& s):
+ *     return __Pyx_PyObject_FromStringAndSize(s.data(), s.size())             # <<<<<<<<<<<<<<
+ * cdef extern from *:
+ *     cdef object __Pyx_PyUnicode_FromStringAndSize(const char*, size_t)
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = __Pyx_PyObject_FromStringAndSize(__pyx_v_s.data(), __pyx_v_s.size()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 32, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* "string.to_py":31
+ * 
+ * @cname("__pyx_convert_PyObject_string_to_py_std__in_string")
+ * cdef inline object __pyx_convert_PyObject_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
+ *     return __Pyx_PyObject_FromStringAndSize(s.data(), s.size())
+ * cdef extern from *:
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("string.to_py.__pyx_convert_PyObject_string_to_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "string.to_py":37
+ * 
+ * @cname("__pyx_convert_PyUnicode_string_to_py_std__in_string")
+ * cdef inline object __pyx_convert_PyUnicode_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
+ *     return __Pyx_PyUnicode_FromStringAndSize(s.data(), s.size())
+ * cdef extern from *:
+ */
+
+static CYTHON_INLINE PyObject *__pyx_convert_PyUnicode_string_to_py_std__in_string(std::string const &__pyx_v_s) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_convert_PyUnicode_string_to_py_std__in_string", 0);
+
+  /* "string.to_py":38
+ * @cname("__pyx_convert_PyUnicode_string_to_py_std__in_string")
+ * cdef inline object __pyx_convert_PyUnicode_string_to_py_std__in_string(const string& s):
+ *     return __Pyx_PyUnicode_FromStringAndSize(s.data(), s.size())             # <<<<<<<<<<<<<<
+ * cdef extern from *:
+ *     cdef object __Pyx_PyStr_FromStringAndSize(const char*, size_t)
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = __Pyx_PyUnicode_FromStringAndSize(__pyx_v_s.data(), __pyx_v_s.size()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 38, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* "string.to_py":37
+ * 
+ * @cname("__pyx_convert_PyUnicode_string_to_py_std__in_string")
+ * cdef inline object __pyx_convert_PyUnicode_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
+ *     return __Pyx_PyUnicode_FromStringAndSize(s.data(), s.size())
+ * cdef extern from *:
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("string.to_py.__pyx_convert_PyUnicode_string_to_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "string.to_py":43
+ * 
+ * @cname("__pyx_convert_PyStr_string_to_py_std__in_string")
+ * cdef inline object __pyx_convert_PyStr_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
+ *     return __Pyx_PyStr_FromStringAndSize(s.data(), s.size())
+ * cdef extern from *:
+ */
+
+static CYTHON_INLINE PyObject *__pyx_convert_PyStr_string_to_py_std__in_string(std::string const &__pyx_v_s) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_convert_PyStr_string_to_py_std__in_string", 0);
+
+  /* "string.to_py":44
+ * @cname("__pyx_convert_PyStr_string_to_py_std__in_string")
+ * cdef inline object __pyx_convert_PyStr_string_to_py_std__in_string(const string& s):
+ *     return __Pyx_PyStr_FromStringAndSize(s.data(), s.size())             # <<<<<<<<<<<<<<
+ * cdef extern from *:
+ *     cdef object __Pyx_PyBytes_FromStringAndSize(const char*, size_t)
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = __Pyx_PyStr_FromStringAndSize(__pyx_v_s.data(), __pyx_v_s.size()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 44, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* "string.to_py":43
+ * 
+ * @cname("__pyx_convert_PyStr_string_to_py_std__in_string")
+ * cdef inline object __pyx_convert_PyStr_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
+ *     return __Pyx_PyStr_FromStringAndSize(s.data(), s.size())
+ * cdef extern from *:
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("string.to_py.__pyx_convert_PyStr_string_to_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "string.to_py":49
+ * 
+ * @cname("__pyx_convert_PyBytes_string_to_py_std__in_string")
+ * cdef inline object __pyx_convert_PyBytes_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
+ *     return __Pyx_PyBytes_FromStringAndSize(s.data(), s.size())
+ * cdef extern from *:
+ */
+
+static CYTHON_INLINE PyObject *__pyx_convert_PyBytes_string_to_py_std__in_string(std::string const &__pyx_v_s) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_convert_PyBytes_string_to_py_std__in_string", 0);
+
+  /* "string.to_py":50
+ * @cname("__pyx_convert_PyBytes_string_to_py_std__in_string")
+ * cdef inline object __pyx_convert_PyBytes_string_to_py_std__in_string(const string& s):
+ *     return __Pyx_PyBytes_FromStringAndSize(s.data(), s.size())             # <<<<<<<<<<<<<<
+ * cdef extern from *:
+ *     cdef object __Pyx_PyByteArray_FromStringAndSize(const char*, size_t)
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_s.data(), __pyx_v_s.size()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* "string.to_py":49
+ * 
+ * @cname("__pyx_convert_PyBytes_string_to_py_std__in_string")
+ * cdef inline object __pyx_convert_PyBytes_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
+ *     return __Pyx_PyBytes_FromStringAndSize(s.data(), s.size())
+ * cdef extern from *:
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("string.to_py.__pyx_convert_PyBytes_string_to_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "string.to_py":55
+ * 
+ * @cname("__pyx_convert_PyByteArray_string_to_py_std__in_string")
+ * cdef inline object __pyx_convert_PyByteArray_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
+ *     return __Pyx_PyByteArray_FromStringAndSize(s.data(), s.size())
+ * 
+ */
+
+static CYTHON_INLINE PyObject *__pyx_convert_PyByteArray_string_to_py_std__in_string(std::string const &__pyx_v_s) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_convert_PyByteArray_string_to_py_std__in_string", 0);
+
+  /* "string.to_py":56
+ * @cname("__pyx_convert_PyByteArray_string_to_py_std__in_string")
+ * cdef inline object __pyx_convert_PyByteArray_string_to_py_std__in_string(const string& s):
+ *     return __Pyx_PyByteArray_FromStringAndSize(s.data(), s.size())             # <<<<<<<<<<<<<<
+ * 
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = __Pyx_PyByteArray_FromStringAndSize(__pyx_v_s.data(), __pyx_v_s.size()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 56, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* "string.to_py":55
+ * 
+ * @cname("__pyx_convert_PyByteArray_string_to_py_std__in_string")
+ * cdef inline object __pyx_convert_PyByteArray_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
+ *     return __Pyx_PyByteArray_FromStringAndSize(s.data(), s.size())
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("string.to_py.__pyx_convert_PyByteArray_string_to_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":246
+ * 
+ *         @property
+ *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
+ *             """Returns a borrowed reference to the object owning the data/memory.
+ *             """
+ */
+
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
+  PyObject *__pyx_r;
+
+  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":249
+ *             """Returns a borrowed reference to the object owning the data/memory.
+ *             """
+ *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __pyx_r = PyArray_BASE(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":246
+ * 
+ *         @property
+ *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
+ *             """Returns a borrowed reference to the object owning the data/memory.
+ *             """
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":252
+ * 
+ *         @property
+ *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
+ *             """Returns an owned reference to the dtype of the array.
+ *             """
+ */
+
+static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
+  PyArray_Descr *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyArray_Descr *__pyx_t_1;
+  __Pyx_RefNannySetupContext("descr", 0);
+
+  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":255
+ *             """Returns an owned reference to the dtype of the array.
+ *             """
+ *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __Pyx_XDECREF((PyObject *)__pyx_r);
+  __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
+  __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
+  __pyx_r = ((PyArray_Descr *)__pyx_t_1);
+  goto __pyx_L0;
+
+  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":252
+ * 
+ *         @property
+ *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
+ *             """Returns an owned reference to the dtype of the array.
+ *             """
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_XGIVEREF((PyObject *)__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":258
+ * 
+ *         @property
+ *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
+ *             """Returns the number of dimensions in the array.
+ *             """
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
+  int __pyx_r;
+
+  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":261
+ *             """Returns the number of dimensions in the array.
+ *             """
+ *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __pyx_r = PyArray_NDIM(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":258
+ * 
+ *         @property
+ *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
+ *             """Returns the number of dimensions in the array.
+ *             """
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":264
+ * 
+ *         @property
+ *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
+ *             """Returns a pointer to the dimensions/shape of the array.
+ *             The number of elements matches the number of dimensions of the array (ndim).
+ */
+
+static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
+  npy_intp *__pyx_r;
+
+  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":269
+ *             Can return NULL for 0-dimensional arrays.
+ *             """
+ *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __pyx_r = PyArray_DIMS(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":264
+ * 
+ *         @property
+ *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
+ *             """Returns a pointer to the dimensions/shape of the array.
+ *             The number of elements matches the number of dimensions of the array (ndim).
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":272
+ * 
+ *         @property
+ *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
+ *             """Returns a pointer to the strides of the array.
+ *             The number of elements matches the number of dimensions of the array (ndim).
+ */
+
+static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
+  npy_intp *__pyx_r;
+
+  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":276
+ *             The number of elements matches the number of dimensions of the array (ndim).
+ *             """
+ *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __pyx_r = PyArray_STRIDES(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":272
+ * 
+ *         @property
+ *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
+ *             """Returns a pointer to the strides of the array.
+ *             The number of elements matches the number of dimensions of the array (ndim).
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":279
+ * 
+ *         @property
+ *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
+ *             """Returns the total size (in number of elements) of the array.
+ *             """
+ */
+
+static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
+  npy_intp __pyx_r;
+
+  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":282
+ *             """Returns the total size (in number of elements) of the array.
+ *             """
+ *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __pyx_r = PyArray_SIZE(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":279
+ * 
+ *         @property
+ *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
+ *             """Returns the total size (in number of elements) of the array.
+ *             """
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":285
+ * 
+ *         @property
+ *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
+ *             """The pointer to the data buffer as a char*.
+ *             This is provided for legacy reasons to avoid direct struct field access.
+ */
+
+static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
+  char *__pyx_r;
+
+  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":291
+ *             of `PyArray_DATA()` instead, which returns a 'void*'.
+ *             """
+ *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
+ * 
+ *     ctypedef unsigned char      npy_bool
+ */
+  __pyx_r = PyArray_BYTES(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":285
+ * 
+ *         @property
+ *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
+ *             """The pointer to the data buffer as a char*.
+ *             This is provided for legacy reasons to avoid direct struct field access.
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":777
+ * ctypedef npy_cdouble     complex_t
+ * 
+ * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
+ *     return PyArray_MultiIterNew(1, <void*>a)
+ * 
+ */
+
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew1(PyObject *__pyx_v_a) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
+
+  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":778
+ * 
+ * cdef inline object PyArray_MultiIterNew1(a):
+ *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
+ * 
+ * cdef inline object PyArray_MultiIterNew2(a, b):
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 778, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":777
+ * ctypedef npy_cdouble     complex_t
+ * 
+ * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
+ *     return PyArray_MultiIterNew(1, <void*>a)
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("numpy.PyArray_MultiIterNew1", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":780
+ *     return PyArray_MultiIterNew(1, <void*>a)
+ * 
+ * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
+ *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
+ * 
+ */
+
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew2(PyObject *__pyx_v_a, PyObject *__pyx_v_b) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
+
+  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":781
+ * 
+ * cdef inline object PyArray_MultiIterNew2(a, b):
+ *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
+ * 
+ * cdef inline object PyArray_MultiIterNew3(a, b, c):
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 781, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":780
+ *     return PyArray_MultiIterNew(1, <void*>a)
+ * 
+ * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
+ *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("numpy.PyArray_MultiIterNew2", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":783
+ *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
+ * 
+ * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
+ *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
+ * 
+ */
+
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew3(PyObject *__pyx_v_a, PyObject *__pyx_v_b, PyObject *__pyx_v_c) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
+
+  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":784
+ * 
+ * cdef inline object PyArray_MultiIterNew3(a, b, c):
+ *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
+ * 
+ * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 784, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":783
+ *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
+ * 
+ * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
+ *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("numpy.PyArray_MultiIterNew3", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":786
+ *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
+ * 
+ * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
+ *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
+ * 
+ */
+
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew4(PyObject *__pyx_v_a, PyObject *__pyx_v_b, PyObject *__pyx_v_c, PyObject *__pyx_v_d) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
+
+  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":787
+ * 
+ * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
+ *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
+ * 
+ * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 787, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":786
+ *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
+ * 
+ * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
+ *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("numpy.PyArray_MultiIterNew4", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
+ *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
+ * 
+ * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
+ *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
+ * 
+ */
+
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew5(PyObject *__pyx_v_a, PyObject *__pyx_v_b, PyObject *__pyx_v_c, PyObject *__pyx_v_d, PyObject *__pyx_v_e) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
+
+  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":790
+ * 
+ * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
+ *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
+ * 
+ * cdef inline tuple PyDataType_SHAPE(dtype d):
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 790, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
+ *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
+ * 
+ * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
+ *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("numpy.PyArray_MultiIterNew5", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":792
+ *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
+ * 
+ * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
+ *     if PyDataType_HASSUBARRAY(d):
+ *         return <tuple>d.subarray.shape
+ */
+
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  int __pyx_t_1;
+  __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
+
+  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":793
+ * 
+ * cdef inline tuple PyDataType_SHAPE(dtype d):
+ *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
+ *         return <tuple>d.subarray.shape
+ *     else:
+ */
+  __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
+  if (__pyx_t_1) {
+
+    /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":794
+ * cdef inline tuple PyDataType_SHAPE(dtype d):
+ *     if PyDataType_HASSUBARRAY(d):
+ *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
+ *     else:
+ *         return ()
+ */
+    __Pyx_XDECREF(__pyx_r);
+    __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
+    __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
+    goto __pyx_L0;
+
+    /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":793
+ * 
+ * cdef inline tuple PyDataType_SHAPE(dtype d):
+ *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
+ *         return <tuple>d.subarray.shape
+ *     else:
+ */
+  }
+
+  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":796
+ *         return <tuple>d.subarray.shape
+ *     else:
+ *         return ()             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  /*else*/ {
+    __Pyx_XDECREF(__pyx_r);
+    __Pyx_INCREF(__pyx_empty_tuple);
+    __pyx_r = __pyx_empty_tuple;
+    goto __pyx_L0;
+  }
+
+  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":792
+ *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
+ * 
+ * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
+ *     if PyDataType_HASSUBARRAY(d):
+ *         return <tuple>d.subarray.shape
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":971
+ *     int _import_umath() except -1
+ * 
+ * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
+ *     Py_INCREF(base) # important to do this before stealing the reference below!
+ *     PyArray_SetBaseObject(arr, base)
+ */
+
+static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("set_array_base", 0);
+
+  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":972
+ * 
+ * cdef inline void set_array_base(ndarray arr, object base):
+ *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
+ *     PyArray_SetBaseObject(arr, base)
+ * 
+ */
+  Py_INCREF(__pyx_v_base);
+
+  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":973
+ * cdef inline void set_array_base(ndarray arr, object base):
+ *     Py_INCREF(base) # important to do this before stealing the reference below!
+ *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
+ * 
+ * cdef inline object get_array_base(ndarray arr):
+ */
+  (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
+
+  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":971
+ *     int _import_umath() except -1
+ * 
+ * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
+ *     Py_INCREF(base) # important to do this before stealing the reference below!
+ *     PyArray_SetBaseObject(arr, base)
+ */
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+}
+
+/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":975
+ *     PyArray_SetBaseObject(arr, base)
+ * 
+ * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
+ *     base = PyArray_BASE(arr)
+ *     if base is NULL:
+ */
+
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
+  PyObject *__pyx_v_base;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  int __pyx_t_1;
+  __Pyx_RefNannySetupContext("get_array_base", 0);
+
+  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":976
+ * 
+ * cdef inline object get_array_base(ndarray arr):
+ *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
+ *     if base is NULL:
+ *         return None
+ */
+  __pyx_v_base = PyArray_BASE(__pyx_v_arr);
+
+  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":977
+ * cdef inline object get_array_base(ndarray arr):
+ *     base = PyArray_BASE(arr)
+ *     if base is NULL:             # <<<<<<<<<<<<<<
+ *         return None
+ *     return <object>base
+ */
+  __pyx_t_1 = (__pyx_v_base == NULL);
+  if (__pyx_t_1) {
+
+    /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":978
+ *     base = PyArray_BASE(arr)
+ *     if base is NULL:
+ *         return None             # <<<<<<<<<<<<<<
+ *     return <object>base
+ * 
+ */
+    __Pyx_XDECREF(__pyx_r);
+    __pyx_r = Py_None; __Pyx_INCREF(Py_None);
+    goto __pyx_L0;
+
+    /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":977
+ * cdef inline object get_array_base(ndarray arr):
+ *     base = PyArray_BASE(arr)
+ *     if base is NULL:             # <<<<<<<<<<<<<<
+ *         return None
+ *     return <object>base
+ */
+  }
+
+  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":979
+ *     if base is NULL:
+ *         return None
+ *     return <object>base             # <<<<<<<<<<<<<<
+ * 
+ * # Versions of the import_* functions which are more suitable for
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_INCREF(((PyObject *)__pyx_v_base));
+  __pyx_r = ((PyObject *)__pyx_v_base);
+  goto __pyx_L0;
+
+  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":975
+ *     PyArray_SetBaseObject(arr, base)
+ * 
+ * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
+ *     base = PyArray_BASE(arr)
+ *     if base is NULL:
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":983
+ * # Versions of the import_* functions which are more suitable for
+ * # Cython code.
+ * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
+ *     try:
+ *         __pyx_import_array()
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_import_array(void) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  int __pyx_t_4;
+  PyObject *__pyx_t_5 = NULL;
+  PyObject *__pyx_t_6 = NULL;
+  PyObject *__pyx_t_7 = NULL;
+  PyObject *__pyx_t_8 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("import_array", 0);
+
+  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":984
+ * # Cython code.
+ * cdef inline int import_array() except -1:
+ *     try:             # <<<<<<<<<<<<<<
+ *         __pyx_import_array()
+ *     except Exception:
+ */
+  {
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
+    __Pyx_XGOTREF(__pyx_t_1);
+    __Pyx_XGOTREF(__pyx_t_2);
+    __Pyx_XGOTREF(__pyx_t_3);
+    /*try:*/ {
+
+      /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":985
+ * cdef inline int import_array() except -1:
+ *     try:
+ *         __pyx_import_array()             # <<<<<<<<<<<<<<
+ *     except Exception:
+ *         raise ImportError("numpy.core.multiarray failed to import")
+ */
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 985, __pyx_L3_error)
+
+      /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":984
+ * # Cython code.
+ * cdef inline int import_array() except -1:
+ *     try:             # <<<<<<<<<<<<<<
+ *         __pyx_import_array()
+ *     except Exception:
+ */
+    }
+    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    goto __pyx_L8_try_end;
+    __pyx_L3_error:;
+
+    /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
+ *     try:
+ *         __pyx_import_array()
+ *     except Exception:             # <<<<<<<<<<<<<<
+ *         raise ImportError("numpy.core.multiarray failed to import")
+ * 
+ */
+    __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
+    if (__pyx_t_4) {
+      __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 986, __pyx_L5_except_error)
+      __Pyx_XGOTREF(__pyx_t_5);
+      __Pyx_XGOTREF(__pyx_t_6);
+      __Pyx_XGOTREF(__pyx_t_7);
+
+      /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
+ *         __pyx_import_array()
+ *     except Exception:
+ *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
+ * 
+ * cdef inline int import_umath() except -1:
+ */
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 987, __pyx_L5_except_error)
+      __Pyx_GOTREF(__pyx_t_8);
+      __Pyx_Raise(__pyx_t_8, 0, 0, 0);
+      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      __PYX_ERR(1, 987, __pyx_L5_except_error)
+    }
+    goto __pyx_L5_except_error;
+
+    /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":984
+ * # Cython code.
+ * cdef inline int import_array() except -1:
+ *     try:             # <<<<<<<<<<<<<<
+ *         __pyx_import_array()
+ *     except Exception:
+ */
+    __pyx_L5_except_error:;
+    __Pyx_XGIVEREF(__pyx_t_1);
+    __Pyx_XGIVEREF(__pyx_t_2);
+    __Pyx_XGIVEREF(__pyx_t_3);
+    __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
+    goto __pyx_L1_error;
+    __pyx_L8_try_end:;
+  }
+
+  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":983
+ * # Versions of the import_* functions which are more suitable for
+ * # Cython code.
+ * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
+ *     try:
+ *         __pyx_import_array()
+ */
+
+  /* function exit code */
+  __pyx_r = 0;
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_8);
+  __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = -1;
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":989
+ *         raise ImportError("numpy.core.multiarray failed to import")
+ * 
+ * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
+ *     try:
+ *         _import_umath()
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_import_umath(void) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  int __pyx_t_4;
+  PyObject *__pyx_t_5 = NULL;
+  PyObject *__pyx_t_6 = NULL;
+  PyObject *__pyx_t_7 = NULL;
+  PyObject *__pyx_t_8 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("import_umath", 0);
+
+  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":990
+ * 
+ * cdef inline int import_umath() except -1:
+ *     try:             # <<<<<<<<<<<<<<
+ *         _import_umath()
+ *     except Exception:
+ */
+  {
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
+    __Pyx_XGOTREF(__pyx_t_1);
+    __Pyx_XGOTREF(__pyx_t_2);
+    __Pyx_XGOTREF(__pyx_t_3);
+    /*try:*/ {
+
+      /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":991
+ * cdef inline int import_umath() except -1:
+ *     try:
+ *         _import_umath()             # <<<<<<<<<<<<<<
+ *     except Exception:
+ *         raise ImportError("numpy.core.umath failed to import")
+ */
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 991, __pyx_L3_error)
+
+      /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":990
+ * 
+ * cdef inline int import_umath() except -1:
+ *     try:             # <<<<<<<<<<<<<<
+ *         _import_umath()
+ *     except Exception:
+ */
+    }
+    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    goto __pyx_L8_try_end;
+    __pyx_L3_error:;
+
+    /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
+ *     try:
+ *         _import_umath()
+ *     except Exception:             # <<<<<<<<<<<<<<
+ *         raise ImportError("numpy.core.umath failed to import")
+ * 
+ */
+    __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
+    if (__pyx_t_4) {
+      __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 992, __pyx_L5_except_error)
+      __Pyx_XGOTREF(__pyx_t_5);
+      __Pyx_XGOTREF(__pyx_t_6);
+      __Pyx_XGOTREF(__pyx_t_7);
+
+      /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
+ *         _import_umath()
+ *     except Exception:
+ *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
+ * 
+ * cdef inline int import_ufunc() except -1:
+ */
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 993, __pyx_L5_except_error)
+      __Pyx_GOTREF(__pyx_t_8);
+      __Pyx_Raise(__pyx_t_8, 0, 0, 0);
+      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      __PYX_ERR(1, 993, __pyx_L5_except_error)
+    }
+    goto __pyx_L5_except_error;
+
+    /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":990
+ * 
+ * cdef inline int import_umath() except -1:
+ *     try:             # <<<<<<<<<<<<<<
+ *         _import_umath()
+ *     except Exception:
+ */
+    __pyx_L5_except_error:;
+    __Pyx_XGIVEREF(__pyx_t_1);
+    __Pyx_XGIVEREF(__pyx_t_2);
+    __Pyx_XGIVEREF(__pyx_t_3);
+    __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
+    goto __pyx_L1_error;
+    __pyx_L8_try_end:;
+  }
+
+  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":989
+ *         raise ImportError("numpy.core.multiarray failed to import")
+ * 
+ * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
+ *     try:
+ *         _import_umath()
+ */
+
+  /* function exit code */
+  __pyx_r = 0;
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_8);
+  __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = -1;
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":995
+ *         raise ImportError("numpy.core.umath failed to import")
+ * 
+ * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
+ *     try:
+ *         _import_umath()
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_import_ufunc(void) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  int __pyx_t_4;
+  PyObject *__pyx_t_5 = NULL;
+  PyObject *__pyx_t_6 = NULL;
+  PyObject *__pyx_t_7 = NULL;
+  PyObject *__pyx_t_8 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("import_ufunc", 0);
+
+  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":996
+ * 
+ * cdef inline int import_ufunc() except -1:
+ *     try:             # <<<<<<<<<<<<<<
+ *         _import_umath()
+ *     except Exception:
+ */
+  {
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
+    __Pyx_XGOTREF(__pyx_t_1);
+    __Pyx_XGOTREF(__pyx_t_2);
+    __Pyx_XGOTREF(__pyx_t_3);
+    /*try:*/ {
+
+      /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":997
+ * cdef inline int import_ufunc() except -1:
+ *     try:
+ *         _import_umath()             # <<<<<<<<<<<<<<
+ *     except Exception:
+ *         raise ImportError("numpy.core.umath failed to import")
+ */
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 997, __pyx_L3_error)
+
+      /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":996
+ * 
+ * cdef inline int import_ufunc() except -1:
+ *     try:             # <<<<<<<<<<<<<<
+ *         _import_umath()
+ *     except Exception:
+ */
+    }
+    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    goto __pyx_L8_try_end;
+    __pyx_L3_error:;
+
+    /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":998
+ *     try:
+ *         _import_umath()
+ *     except Exception:             # <<<<<<<<<<<<<<
+ *         raise ImportError("numpy.core.umath failed to import")
+ * 
+ */
+    __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
+    if (__pyx_t_4) {
+      __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 998, __pyx_L5_except_error)
+      __Pyx_XGOTREF(__pyx_t_5);
+      __Pyx_XGOTREF(__pyx_t_6);
+      __Pyx_XGOTREF(__pyx_t_7);
+
+      /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":999
+ *         _import_umath()
+ *     except Exception:
+ *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 999, __pyx_L5_except_error)
+      __Pyx_GOTREF(__pyx_t_8);
+      __Pyx_Raise(__pyx_t_8, 0, 0, 0);
+      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      __PYX_ERR(1, 999, __pyx_L5_except_error)
+    }
+    goto __pyx_L5_except_error;
+
+    /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":996
+ * 
+ * cdef inline int import_ufunc() except -1:
+ *     try:             # <<<<<<<<<<<<<<
+ *         _import_umath()
+ *     except Exception:
+ */
+    __pyx_L5_except_error:;
+    __Pyx_XGIVEREF(__pyx_t_1);
+    __Pyx_XGIVEREF(__pyx_t_2);
+    __Pyx_XGIVEREF(__pyx_t_3);
+    __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
+    goto __pyx_L1_error;
+    __pyx_L8_try_end:;
+  }
+
+  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":995
+ *         raise ImportError("numpy.core.umath failed to import")
+ * 
+ * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
+ *     try:
+ *         _import_umath()
+ */
+
+  /* function exit code */
+  __pyx_r = 0;
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_8);
+  __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = -1;
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1002
+ * 
+ * 
+ * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.timedelta64)`
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
+
+  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1014
+ *     bool
+ *     """
+ *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
+  goto __pyx_L0;
+
+  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1002
+ * 
+ * 
+ * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.timedelta64)`
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1017
+ * 
+ * 
+ * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.datetime64)`
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("is_datetime64_object", 0);
+
+  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1029
+ *     bool
+ *     """
+ *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
+  goto __pyx_L0;
+
+  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1017
+ * 
+ * 
+ * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.datetime64)`
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1032
+ * 
+ * 
+ * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy datetime64 object
+ */
+
+static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
+  npy_datetime __pyx_r;
+
+  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1039
+ *     also needed.  That can be found using `get_datetime64_unit`.
+ *     """
+ *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
+  goto __pyx_L0;
+
+  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1032
+ * 
+ * 
+ * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy datetime64 object
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1042
+ * 
+ * 
+ * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy timedelta64 object
+ */
+
+static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
+  npy_timedelta __pyx_r;
+
+  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1046
+ *     returns the int64 value underlying scalar numpy timedelta64 object
+ *     """
+ *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
+  goto __pyx_L0;
+
+  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1042
+ * 
+ * 
+ * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy timedelta64 object
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1049
+ * 
+ * 
+ * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the unit part of the dtype for a numpy datetime64 object.
+ */
+
+static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
+  NPY_DATETIMEUNIT __pyx_r;
+
+  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1053
+ *     returns the unit part of the dtype for a numpy datetime64 object.
+ *     """
+ *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
+ */
+  __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
+  goto __pyx_L0;
+
+  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1049
+ * 
+ * 
+ * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the unit part of the dtype for a numpy datetime64 object.
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
 
 /* "arcticpy/wrapper.pyx":105
  * 
  * 
  * def cy_print_version():             # <<<<<<<<<<<<<<
  *     print_version()
  * 
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_8arcticpy_7wrapper_1cy_print_version(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused); /*proto*/
 static PyMethodDef __pyx_mdef_8arcticpy_7wrapper_1cy_print_version = {"cy_print_version", (PyCFunction)__pyx_pw_8arcticpy_7wrapper_1cy_print_version, METH_NOARGS, 0};
 static PyObject *__pyx_pw_8arcticpy_7wrapper_1cy_print_version(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused) {
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("cy_print_version (wrapper)", 0);
   __pyx_r = __pyx_pf_8arcticpy_7wrapper_cy_print_version(__pyx_self);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
@@ -2188,14 +4848,15 @@
  * 
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_8arcticpy_7wrapper_3cy_version_arctic(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused); /*proto*/
 static PyMethodDef __pyx_mdef_8arcticpy_7wrapper_3cy_version_arctic = {"cy_version_arctic", (PyCFunction)__pyx_pw_8arcticpy_7wrapper_3cy_version_arctic, METH_NOARGS, 0};
 static PyObject *__pyx_pw_8arcticpy_7wrapper_3cy_version_arctic(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused) {
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("cy_version_arctic (wrapper)", 0);
   __pyx_r = __pyx_pf_8arcticpy_7wrapper_2cy_version_arctic(__pyx_self);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
@@ -2215,15 +4876,15 @@
  * 
  * def cy_version_arctic():
  *     return version_arctic().decode("utf-8")             # <<<<<<<<<<<<<<
  * 
  * def check_contiguous(array):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_decode_cpp_string(version_arctic(), 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 109, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_decode_cpp_string(version_arctic(), 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 109, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* "arcticpy/wrapper.pyx":108
  *     print_version()
@@ -2249,86 +4910,149 @@
  * 
  * def check_contiguous(array):             # <<<<<<<<<<<<<<
  *     """ Make sure an array is contiguous and C-style. """
  *     if not array.flags['C_CONTIGUOUS']:
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8arcticpy_7wrapper_5check_contiguous(PyObject *__pyx_self, PyObject *__pyx_v_array); /*proto*/
-static char __pyx_doc_8arcticpy_7wrapper_4check_contiguous[] = " Make sure an array is contiguous and C-style. ";
-static PyMethodDef __pyx_mdef_8arcticpy_7wrapper_5check_contiguous = {"check_contiguous", (PyCFunction)__pyx_pw_8arcticpy_7wrapper_5check_contiguous, METH_O, __pyx_doc_8arcticpy_7wrapper_4check_contiguous};
-static PyObject *__pyx_pw_8arcticpy_7wrapper_5check_contiguous(PyObject *__pyx_self, PyObject *__pyx_v_array) {
+static PyObject *__pyx_pw_8arcticpy_7wrapper_5check_contiguous(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+PyDoc_STRVAR(__pyx_doc_8arcticpy_7wrapper_4check_contiguous, " Make sure an array is contiguous and C-style. ");
+static PyMethodDef __pyx_mdef_8arcticpy_7wrapper_5check_contiguous = {"check_contiguous", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8arcticpy_7wrapper_5check_contiguous, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_8arcticpy_7wrapper_4check_contiguous};
+static PyObject *__pyx_pw_8arcticpy_7wrapper_5check_contiguous(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
+  PyObject *__pyx_v_array = 0;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("check_contiguous (wrapper)", 0);
-  __pyx_r = __pyx_pf_8arcticpy_7wrapper_4check_contiguous(__pyx_self, ((PyObject *)__pyx_v_array));
+  {
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_array,0};
+    PyObject* values[1] = {0};
+    if (__pyx_kwds) {
+      Py_ssize_t kw_args;
+      switch (__pyx_nargs) {
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
+        case  0:
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_array)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 111, __pyx_L3_error)
+        else goto __pyx_L5_argtuple_error;
+      }
+      if (unlikely(kw_args > 0)) {
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "check_contiguous") < 0)) __PYX_ERR(2, 111, __pyx_L3_error)
+      }
+    } else if (unlikely(__pyx_nargs != 1)) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+    }
+    __pyx_v_array = values[0];
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("check_contiguous", 1, 1, 1, __pyx_nargs); __PYX_ERR(2, 111, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("arcticpy.wrapper.check_contiguous", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_8arcticpy_7wrapper_4check_contiguous(__pyx_self, __pyx_v_array);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_8arcticpy_7wrapper_4check_contiguous(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_array) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_t_3;
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
+  int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("check_contiguous", 0);
 
   /* "arcticpy/wrapper.pyx":113
  * def check_contiguous(array):
  *     """ Make sure an array is contiguous and C-style. """
  *     if not array.flags['C_CONTIGUOUS']:             # <<<<<<<<<<<<<<
  *         return np.ascontiguousarray(array)
  *     else:
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_array, __pyx_n_s_flags); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 113, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_array, __pyx_n_s_flags); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 113, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_t_1, __pyx_n_u_C_CONTIGUOUS); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 113, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_t_1, __pyx_n_u_C_CONTIGUOUS); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 113, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 113, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely((__pyx_t_3 < 0))) __PYX_ERR(2, 113, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_4 = ((!__pyx_t_3) != 0);
+  __pyx_t_4 = (!__pyx_t_3);
   if (__pyx_t_4) {
 
     /* "arcticpy/wrapper.pyx":114
  *     """ Make sure an array is contiguous and C-style. """
  *     if not array.flags['C_CONTIGUOUS']:
  *         return np.ascontiguousarray(array)             # <<<<<<<<<<<<<<
  *     else:
  *         return array
  */
     __Pyx_XDECREF(__pyx_r);
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 114, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 114, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_ascontiguousarray); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 114, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_ascontiguousarray); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 114, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_1 = NULL;
+    __pyx_t_6 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_1)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
         __Pyx_INCREF(__pyx_t_1);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_5, function);
+        __pyx_t_6 = 1;
       }
     }
-    __pyx_t_2 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_1, __pyx_v_array) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_v_array);
-    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 114, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    {
+      PyObject *__pyx_callargs[2] = {__pyx_t_1, __pyx_v_array};
+      __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
+      __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 114, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_2);
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    }
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L0;
 
     /* "arcticpy/wrapper.pyx":113
  * def check_contiguous(array):
  *     """ Make sure an array is contiguous and C-style. """
@@ -2378,25 +5102,79 @@
  * 
  * def cy_print_array(np.ndarray[np.double_t, ndim=1] array):             # <<<<<<<<<<<<<<
  *     array = check_contiguous(array)
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8arcticpy_7wrapper_7cy_print_array(PyObject *__pyx_self, PyObject *__pyx_v_array); /*proto*/
-static PyMethodDef __pyx_mdef_8arcticpy_7wrapper_7cy_print_array = {"cy_print_array", (PyCFunction)__pyx_pw_8arcticpy_7wrapper_7cy_print_array, METH_O, 0};
-static PyObject *__pyx_pw_8arcticpy_7wrapper_7cy_print_array(PyObject *__pyx_self, PyObject *__pyx_v_array) {
+static PyObject *__pyx_pw_8arcticpy_7wrapper_7cy_print_array(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+static PyMethodDef __pyx_mdef_8arcticpy_7wrapper_7cy_print_array = {"cy_print_array", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8arcticpy_7wrapper_7cy_print_array, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_8arcticpy_7wrapper_7cy_print_array(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
+  PyArrayObject *__pyx_v_array = 0;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("cy_print_array (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_array), __pyx_ptype_5numpy_ndarray, 1, "array", 0))) __PYX_ERR(0, 119, __pyx_L1_error)
-  __pyx_r = __pyx_pf_8arcticpy_7wrapper_6cy_print_array(__pyx_self, ((PyArrayObject *)__pyx_v_array));
+  {
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_array,0};
+    PyObject* values[1] = {0};
+    if (__pyx_kwds) {
+      Py_ssize_t kw_args;
+      switch (__pyx_nargs) {
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
+        case  0:
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_array)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 119, __pyx_L3_error)
+        else goto __pyx_L5_argtuple_error;
+      }
+      if (unlikely(kw_args > 0)) {
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "cy_print_array") < 0)) __PYX_ERR(2, 119, __pyx_L3_error)
+      }
+    } else if (unlikely(__pyx_nargs != 1)) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+    }
+    __pyx_v_array = ((PyArrayObject *)values[0]);
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("cy_print_array", 1, 1, 1, __pyx_nargs); __PYX_ERR(2, 119, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("arcticpy.wrapper.cy_print_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_array), __pyx_ptype_5numpy_ndarray, 1, "array", 0))) __PYX_ERR(2, 119, __pyx_L1_error)
+  __pyx_r = __pyx_pf_8arcticpy_7wrapper_6cy_print_array(__pyx_self, __pyx_v_array);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
@@ -2407,100 +5185,107 @@
   __Pyx_LocalBuf_ND __pyx_pybuffernd_array;
   __Pyx_Buffer __pyx_pybuffer_array;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
-  PyArrayObject *__pyx_t_4 = NULL;
-  int __pyx_t_5;
+  int __pyx_t_4;
+  PyArrayObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   Py_ssize_t __pyx_t_9;
+  npy_intp *__pyx_t_10;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("cy_print_array", 0);
   __Pyx_INCREF((PyObject *)__pyx_v_array);
   __pyx_pybuffer_array.pybuffer.buf = NULL;
   __pyx_pybuffer_array.refcount = 0;
   __pyx_pybuffernd_array.data = NULL;
   __pyx_pybuffernd_array.rcbuffer = &__pyx_pybuffer_array;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_array.rcbuffer->pybuffer, (PyObject*)__pyx_v_array, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 119, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_array.rcbuffer->pybuffer, (PyObject*)__pyx_v_array, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(2, 119, __pyx_L1_error)
   }
   __pyx_pybuffernd_array.diminfo[0].strides = __pyx_pybuffernd_array.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_array.diminfo[0].shape = __pyx_pybuffernd_array.rcbuffer->pybuffer.shape[0];
 
   /* "arcticpy/wrapper.pyx":120
  * 
  * def cy_print_array(np.ndarray[np.double_t, ndim=1] array):
  *     array = check_contiguous(array)             # <<<<<<<<<<<<<<
  * 
  *     print_array(&array[0], array.shape[0])
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_check_contiguous); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 120, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_check_contiguous); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 120, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
+  __pyx_t_4 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
+      __pyx_t_4 = 1;
     }
   }
-  __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, ((PyObject *)__pyx_v_array)) : __Pyx_PyObject_CallOneArg(__pyx_t_2, ((PyObject *)__pyx_v_array));
-  __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 120, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 120, __pyx_L1_error)
-  __pyx_t_4 = ((PyArrayObject *)__pyx_t_1);
+  {
+    PyObject *__pyx_callargs[2] = {__pyx_t_3, ((PyObject *)__pyx_v_array)};
+    __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 120, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  }
+  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(2, 120, __pyx_L1_error)
+  __pyx_t_5 = ((PyArrayObject *)__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_array.rcbuffer->pybuffer);
-    __pyx_t_5 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_array.rcbuffer->pybuffer, (PyObject*)__pyx_t_4, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack);
-    if (unlikely(__pyx_t_5 < 0)) {
+    __pyx_t_4 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_array.rcbuffer->pybuffer, (PyObject*)__pyx_t_5, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack);
+    if (unlikely(__pyx_t_4 < 0)) {
       PyErr_Fetch(&__pyx_t_6, &__pyx_t_7, &__pyx_t_8);
       if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_array.rcbuffer->pybuffer, (PyObject*)__pyx_v_array, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
         Py_XDECREF(__pyx_t_6); Py_XDECREF(__pyx_t_7); Py_XDECREF(__pyx_t_8);
         __Pyx_RaiseBufferFallbackError();
       } else {
         PyErr_Restore(__pyx_t_6, __pyx_t_7, __pyx_t_8);
       }
       __pyx_t_6 = __pyx_t_7 = __pyx_t_8 = 0;
     }
     __pyx_pybuffernd_array.diminfo[0].strides = __pyx_pybuffernd_array.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_array.diminfo[0].shape = __pyx_pybuffernd_array.rcbuffer->pybuffer.shape[0];
-    if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 120, __pyx_L1_error)
+    if (unlikely((__pyx_t_4 < 0))) __PYX_ERR(2, 120, __pyx_L1_error)
   }
-  __pyx_t_4 = 0;
+  __pyx_t_5 = 0;
   __Pyx_DECREF_SET(__pyx_v_array, ((PyArrayObject *)__pyx_t_1));
   __pyx_t_1 = 0;
 
   /* "arcticpy/wrapper.pyx":122
  *     array = check_contiguous(array)
  * 
  *     print_array(&array[0], array.shape[0])             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_t_9 = 0;
-  __pyx_t_5 = -1;
+  __pyx_t_4 = -1;
   if (__pyx_t_9 < 0) {
     __pyx_t_9 += __pyx_pybuffernd_array.diminfo[0].shape;
-    if (unlikely(__pyx_t_9 < 0)) __pyx_t_5 = 0;
-  } else if (unlikely(__pyx_t_9 >= __pyx_pybuffernd_array.diminfo[0].shape)) __pyx_t_5 = 0;
-  if (unlikely(__pyx_t_5 != -1)) {
-    __Pyx_RaiseBufferIndexError(__pyx_t_5);
-    __PYX_ERR(0, 122, __pyx_L1_error)
+    if (unlikely(__pyx_t_9 < 0)) __pyx_t_4 = 0;
+  } else if (unlikely(__pyx_t_9 >= __pyx_pybuffernd_array.diminfo[0].shape)) __pyx_t_4 = 0;
+  if (unlikely(__pyx_t_4 != -1)) {
+    __Pyx_RaiseBufferIndexError(__pyx_t_4);
+    __PYX_ERR(2, 122, __pyx_L1_error)
   }
-  print_array((&(*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_array.rcbuffer->pybuffer.buf, __pyx_t_9, __pyx_pybuffernd_array.diminfo[0].strides))), (__pyx_v_array->dimensions[0]));
+  __pyx_t_10 = __pyx_f_5numpy_7ndarray_5shape_shape(((PyArrayObject *)__pyx_v_array)); if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 122, __pyx_L1_error)
+  print_array((&(*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_array.rcbuffer->pybuffer.buf, __pyx_t_9, __pyx_pybuffernd_array.diminfo[0].strides))), (__pyx_t_10[0]));
 
   /* "arcticpy/wrapper.pyx":119
  * 
  * 
  * def cy_print_array(np.ndarray[np.double_t, ndim=1] array):             # <<<<<<<<<<<<<<
  *     array = check_contiguous(array)
  * 
@@ -2536,25 +5321,79 @@
  * 
  * def cy_print_array_2D(np.ndarray[np.double_t, ndim=2] array):             # <<<<<<<<<<<<<<
  *     array = check_contiguous(array)
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8arcticpy_7wrapper_9cy_print_array_2D(PyObject *__pyx_self, PyObject *__pyx_v_array); /*proto*/
-static PyMethodDef __pyx_mdef_8arcticpy_7wrapper_9cy_print_array_2D = {"cy_print_array_2D", (PyCFunction)__pyx_pw_8arcticpy_7wrapper_9cy_print_array_2D, METH_O, 0};
-static PyObject *__pyx_pw_8arcticpy_7wrapper_9cy_print_array_2D(PyObject *__pyx_self, PyObject *__pyx_v_array) {
+static PyObject *__pyx_pw_8arcticpy_7wrapper_9cy_print_array_2D(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+static PyMethodDef __pyx_mdef_8arcticpy_7wrapper_9cy_print_array_2D = {"cy_print_array_2D", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8arcticpy_7wrapper_9cy_print_array_2D, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_8arcticpy_7wrapper_9cy_print_array_2D(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
+  PyArrayObject *__pyx_v_array = 0;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("cy_print_array_2D (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_array), __pyx_ptype_5numpy_ndarray, 1, "array", 0))) __PYX_ERR(0, 125, __pyx_L1_error)
-  __pyx_r = __pyx_pf_8arcticpy_7wrapper_8cy_print_array_2D(__pyx_self, ((PyArrayObject *)__pyx_v_array));
+  {
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_array,0};
+    PyObject* values[1] = {0};
+    if (__pyx_kwds) {
+      Py_ssize_t kw_args;
+      switch (__pyx_nargs) {
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
+        case  0:
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_array)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 125, __pyx_L3_error)
+        else goto __pyx_L5_argtuple_error;
+      }
+      if (unlikely(kw_args > 0)) {
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "cy_print_array_2D") < 0)) __PYX_ERR(2, 125, __pyx_L3_error)
+      }
+    } else if (unlikely(__pyx_nargs != 1)) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+    }
+    __pyx_v_array = ((PyArrayObject *)values[0]);
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("cy_print_array_2D", 1, 1, 1, __pyx_nargs); __PYX_ERR(2, 125, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("arcticpy.wrapper.cy_print_array_2D", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_array), __pyx_ptype_5numpy_ndarray, 1, "array", 0))) __PYX_ERR(2, 125, __pyx_L1_error)
+  __pyx_r = __pyx_pf_8arcticpy_7wrapper_8cy_print_array_2D(__pyx_self, __pyx_v_array);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
@@ -2565,106 +5404,115 @@
   __Pyx_LocalBuf_ND __pyx_pybuffernd_array;
   __Pyx_Buffer __pyx_pybuffer_array;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
-  PyArrayObject *__pyx_t_4 = NULL;
-  int __pyx_t_5;
+  int __pyx_t_4;
+  PyArrayObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   Py_ssize_t __pyx_t_9;
   Py_ssize_t __pyx_t_10;
+  npy_intp *__pyx_t_11;
+  npy_intp *__pyx_t_12;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("cy_print_array_2D", 0);
   __Pyx_INCREF((PyObject *)__pyx_v_array);
   __pyx_pybuffer_array.pybuffer.buf = NULL;
   __pyx_pybuffer_array.refcount = 0;
   __pyx_pybuffernd_array.data = NULL;
   __pyx_pybuffernd_array.rcbuffer = &__pyx_pybuffer_array;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_array.rcbuffer->pybuffer, (PyObject*)__pyx_v_array, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) __PYX_ERR(0, 125, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_array.rcbuffer->pybuffer, (PyObject*)__pyx_v_array, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) __PYX_ERR(2, 125, __pyx_L1_error)
   }
   __pyx_pybuffernd_array.diminfo[0].strides = __pyx_pybuffernd_array.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_array.diminfo[0].shape = __pyx_pybuffernd_array.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_array.diminfo[1].strides = __pyx_pybuffernd_array.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_array.diminfo[1].shape = __pyx_pybuffernd_array.rcbuffer->pybuffer.shape[1];
 
   /* "arcticpy/wrapper.pyx":126
  * 
  * def cy_print_array_2D(np.ndarray[np.double_t, ndim=2] array):
  *     array = check_contiguous(array)             # <<<<<<<<<<<<<<
  * 
  *     print_array_2D(&array[0, 0], array.shape[0], array.shape[1])
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_check_contiguous); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 126, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_check_contiguous); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 126, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
+  __pyx_t_4 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
+      __pyx_t_4 = 1;
     }
   }
-  __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, ((PyObject *)__pyx_v_array)) : __Pyx_PyObject_CallOneArg(__pyx_t_2, ((PyObject *)__pyx_v_array));
-  __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 126, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 126, __pyx_L1_error)
-  __pyx_t_4 = ((PyArrayObject *)__pyx_t_1);
+  {
+    PyObject *__pyx_callargs[2] = {__pyx_t_3, ((PyObject *)__pyx_v_array)};
+    __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 126, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  }
+  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(2, 126, __pyx_L1_error)
+  __pyx_t_5 = ((PyArrayObject *)__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_array.rcbuffer->pybuffer);
-    __pyx_t_5 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_array.rcbuffer->pybuffer, (PyObject*)__pyx_t_4, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack);
-    if (unlikely(__pyx_t_5 < 0)) {
+    __pyx_t_4 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_array.rcbuffer->pybuffer, (PyObject*)__pyx_t_5, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack);
+    if (unlikely(__pyx_t_4 < 0)) {
       PyErr_Fetch(&__pyx_t_6, &__pyx_t_7, &__pyx_t_8);
       if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_array.rcbuffer->pybuffer, (PyObject*)__pyx_v_array, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) {
         Py_XDECREF(__pyx_t_6); Py_XDECREF(__pyx_t_7); Py_XDECREF(__pyx_t_8);
         __Pyx_RaiseBufferFallbackError();
       } else {
         PyErr_Restore(__pyx_t_6, __pyx_t_7, __pyx_t_8);
       }
       __pyx_t_6 = __pyx_t_7 = __pyx_t_8 = 0;
     }
     __pyx_pybuffernd_array.diminfo[0].strides = __pyx_pybuffernd_array.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_array.diminfo[0].shape = __pyx_pybuffernd_array.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_array.diminfo[1].strides = __pyx_pybuffernd_array.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_array.diminfo[1].shape = __pyx_pybuffernd_array.rcbuffer->pybuffer.shape[1];
-    if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 126, __pyx_L1_error)
+    if (unlikely((__pyx_t_4 < 0))) __PYX_ERR(2, 126, __pyx_L1_error)
   }
-  __pyx_t_4 = 0;
+  __pyx_t_5 = 0;
   __Pyx_DECREF_SET(__pyx_v_array, ((PyArrayObject *)__pyx_t_1));
   __pyx_t_1 = 0;
 
   /* "arcticpy/wrapper.pyx":128
  *     array = check_contiguous(array)
  * 
  *     print_array_2D(&array[0, 0], array.shape[0], array.shape[1])             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_t_9 = 0;
   __pyx_t_10 = 0;
-  __pyx_t_5 = -1;
+  __pyx_t_4 = -1;
   if (__pyx_t_9 < 0) {
     __pyx_t_9 += __pyx_pybuffernd_array.diminfo[0].shape;
-    if (unlikely(__pyx_t_9 < 0)) __pyx_t_5 = 0;
-  } else if (unlikely(__pyx_t_9 >= __pyx_pybuffernd_array.diminfo[0].shape)) __pyx_t_5 = 0;
+    if (unlikely(__pyx_t_9 < 0)) __pyx_t_4 = 0;
+  } else if (unlikely(__pyx_t_9 >= __pyx_pybuffernd_array.diminfo[0].shape)) __pyx_t_4 = 0;
   if (__pyx_t_10 < 0) {
     __pyx_t_10 += __pyx_pybuffernd_array.diminfo[1].shape;
-    if (unlikely(__pyx_t_10 < 0)) __pyx_t_5 = 1;
-  } else if (unlikely(__pyx_t_10 >= __pyx_pybuffernd_array.diminfo[1].shape)) __pyx_t_5 = 1;
-  if (unlikely(__pyx_t_5 != -1)) {
-    __Pyx_RaiseBufferIndexError(__pyx_t_5);
-    __PYX_ERR(0, 128, __pyx_L1_error)
-  }
-  print_array_2D((&(*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_array.rcbuffer->pybuffer.buf, __pyx_t_9, __pyx_pybuffernd_array.diminfo[0].strides, __pyx_t_10, __pyx_pybuffernd_array.diminfo[1].strides))), (__pyx_v_array->dimensions[0]), (__pyx_v_array->dimensions[1]));
+    if (unlikely(__pyx_t_10 < 0)) __pyx_t_4 = 1;
+  } else if (unlikely(__pyx_t_10 >= __pyx_pybuffernd_array.diminfo[1].shape)) __pyx_t_4 = 1;
+  if (unlikely(__pyx_t_4 != -1)) {
+    __Pyx_RaiseBufferIndexError(__pyx_t_4);
+    __PYX_ERR(2, 128, __pyx_L1_error)
+  }
+  __pyx_t_11 = __pyx_f_5numpy_7ndarray_5shape_shape(((PyArrayObject *)__pyx_v_array)); if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 128, __pyx_L1_error)
+  __pyx_t_12 = __pyx_f_5numpy_7ndarray_5shape_shape(((PyArrayObject *)__pyx_v_array)); if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 128, __pyx_L1_error)
+  print_array_2D((&(*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_array.rcbuffer->pybuffer.buf, __pyx_t_9, __pyx_pybuffernd_array.diminfo[0].strides, __pyx_t_10, __pyx_pybuffernd_array.diminfo[1].strides))), (__pyx_t_11[0]), (__pyx_t_12[1]));
 
   /* "arcticpy/wrapper.pyx":125
  * 
  * 
  * def cy_print_array_2D(np.ndarray[np.double_t, ndim=2] array):             # <<<<<<<<<<<<<<
  *     array = check_contiguous(array)
  * 
@@ -2700,18 +5548,30 @@
  * 
  * def cy_add_cti(             # <<<<<<<<<<<<<<
  *     np.ndarray[np.double_t, ndim=2] image,
  *     # ========
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8arcticpy_7wrapper_11cy_add_cti(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_8arcticpy_7wrapper_10cy_add_cti[] = "\n    Cython wrapper for arctic's add_cti() in src/cti.cpp.\n\n    This wrapper passes the individual numbers and arrays extracted by the\n    python wrapper to the C++ interface. See add_cti() in cti.py and add_cti()\n    in interface.cpp.\n    ";
-static PyMethodDef __pyx_mdef_8arcticpy_7wrapper_11cy_add_cti = {"cy_add_cti", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8arcticpy_7wrapper_11cy_add_cti, METH_VARARGS|METH_KEYWORDS, __pyx_doc_8arcticpy_7wrapper_10cy_add_cti};
-static PyObject *__pyx_pw_8arcticpy_7wrapper_11cy_add_cti(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_8arcticpy_7wrapper_11cy_add_cti(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+PyDoc_STRVAR(__pyx_doc_8arcticpy_7wrapper_10cy_add_cti, "\n    Cython wrapper for arctic's add_cti() in src/cti.cpp.\n\n    This wrapper passes the individual numbers and arrays extracted by the\n    python wrapper to the C++ interface. See add_cti() in cti.py and add_cti()\n    in interface.cpp.\n    ");
+static PyMethodDef __pyx_mdef_8arcticpy_7wrapper_11cy_add_cti = {"cy_add_cti", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8arcticpy_7wrapper_11cy_add_cti, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_8arcticpy_7wrapper_10cy_add_cti};
+static PyObject *__pyx_pw_8arcticpy_7wrapper_11cy_add_cti(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
   PyArrayObject *__pyx_v_image = 0;
   PyArrayObject *__pyx_v_parallel_dwell_times = 0;
   int __pyx_v_parallel_prescan_offset;
   int __pyx_v_parallel_overscan_start;
   int __pyx_v_parallel_empty_traps_between_columns;
   int __pyx_v_parallel_empty_traps_for_first_transfers;
   int __pyx_v_parallel_force_release_away_from_readout;
@@ -2768,709 +5628,777 @@
   int __pyx_v_serial_time_start;
   int __pyx_v_serial_time_stop;
   PyArrayObject *__pyx_v_serial_prune_n_electrons = 0;
   int __pyx_v_serial_prune_frequency;
   int __pyx_v_allow_negative_pixels;
   int __pyx_v_verbosity;
   int __pyx_v_iteration;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("cy_add_cti (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_image,&__pyx_n_s_parallel_dwell_times,&__pyx_n_s_parallel_prescan_offset,&__pyx_n_s_parallel_overscan_start,&__pyx_n_s_parallel_empty_traps_between_col,&__pyx_n_s_parallel_empty_traps_for_first_t,&__pyx_n_s_parallel_force_release_away_from,&__pyx_n_s_parallel_use_integer_express_mat,&__pyx_n_s_parallel_n_pumps,&__pyx_n_s_parallel_roe_type,&__pyx_n_s_parallel_fraction_of_traps_per_p,&__pyx_n_s_parallel_full_well_depths,&__pyx_n_s_parallel_well_notch_depths,&__pyx_n_s_parallel_well_fill_powers,&__pyx_n_s_parallel_first_electron_fills,&__pyx_n_s_parallel_trap_densities,&__pyx_n_s_parallel_trap_release_timescales,&__pyx_n_s_parallel_trap_third_params,&__pyx_n_s_parallel_trap_fourth_params,&__pyx_n_s_parallel_n_traps_ic,&__pyx_n_s_parallel_n_traps_sc,&__pyx_n_s_parallel_n_traps_ic_co,&__pyx_n_s_parallel_n_traps_sc_co,&__pyx_n_s_parallel_express,&__pyx_n_s_parallel_window_offset,&__pyx_n_s_parallel_window_start,&__pyx_n_s_parallel_window_stop,&__pyx_n_s_parallel_time_start,&__pyx_n_s_parallel_time_stop,&__pyx_n_s_parallel_prune_n_electrons,&__pyx_n_s_parallel_prune_frequency,&__pyx_n_s_serial_dwell_times,&__pyx_n_s_serial_prescan_offset,&__pyx_n_s_serial_overscan_start,&__pyx_n_s_serial_empty_traps_between_colum,&__pyx_n_s_serial_empty_traps_for_first_tra,&__pyx_n_s_serial_force_release_away_from_r,&__pyx_n_s_serial_use_integer_express_matri,&__pyx_n_s_serial_n_pumps,&__pyx_n_s_serial_roe_type,&__pyx_n_s_serial_fraction_of_traps_per_pha,&__pyx_n_s_serial_full_well_depths,&__pyx_n_s_serial_well_notch_depths,&__pyx_n_s_serial_well_fill_powers,&__pyx_n_s_serial_first_electron_fills,&__pyx_n_s_serial_trap_densities,&__pyx_n_s_serial_trap_release_timescales,&__pyx_n_s_serial_trap_third_params,&__pyx_n_s_serial_trap_fourth_params,&__pyx_n_s_serial_n_traps_ic,&__pyx_n_s_serial_n_traps_sc,&__pyx_n_s_serial_n_traps_ic_co,&__pyx_n_s_serial_n_traps_sc_co,&__pyx_n_s_serial_express,&__pyx_n_s_serial_window_offset,&__pyx_n_s_serial_window_start,&__pyx_n_s_serial_window_stop,&__pyx_n_s_serial_time_start,&__pyx_n_s_serial_time_stop,&__pyx_n_s_serial_prune_n_electrons,&__pyx_n_s_serial_prune_frequency,&__pyx_n_s_allow_negative_pixels,&__pyx_n_s_verbosity,&__pyx_n_s_iteration,0};
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_image,&__pyx_n_s_parallel_dwell_times,&__pyx_n_s_parallel_prescan_offset,&__pyx_n_s_parallel_overscan_start,&__pyx_n_s_parallel_empty_traps_between_col,&__pyx_n_s_parallel_empty_traps_for_first_t,&__pyx_n_s_parallel_force_release_away_from,&__pyx_n_s_parallel_use_integer_express_mat,&__pyx_n_s_parallel_n_pumps,&__pyx_n_s_parallel_roe_type,&__pyx_n_s_parallel_fraction_of_traps_per_p,&__pyx_n_s_parallel_full_well_depths,&__pyx_n_s_parallel_well_notch_depths,&__pyx_n_s_parallel_well_fill_powers,&__pyx_n_s_parallel_first_electron_fills,&__pyx_n_s_parallel_trap_densities,&__pyx_n_s_parallel_trap_release_timescales,&__pyx_n_s_parallel_trap_third_params,&__pyx_n_s_parallel_trap_fourth_params,&__pyx_n_s_parallel_n_traps_ic,&__pyx_n_s_parallel_n_traps_sc,&__pyx_n_s_parallel_n_traps_ic_co,&__pyx_n_s_parallel_n_traps_sc_co,&__pyx_n_s_parallel_express,&__pyx_n_s_parallel_window_offset,&__pyx_n_s_parallel_window_start,&__pyx_n_s_parallel_window_stop,&__pyx_n_s_parallel_time_start,&__pyx_n_s_parallel_time_stop,&__pyx_n_s_parallel_prune_n_electrons,&__pyx_n_s_parallel_prune_frequency,&__pyx_n_s_serial_dwell_times,&__pyx_n_s_serial_prescan_offset,&__pyx_n_s_serial_overscan_start,&__pyx_n_s_serial_empty_traps_between_colum,&__pyx_n_s_serial_empty_traps_for_first_tra,&__pyx_n_s_serial_force_release_away_from_r,&__pyx_n_s_serial_use_integer_express_matri,&__pyx_n_s_serial_n_pumps,&__pyx_n_s_serial_roe_type,&__pyx_n_s_serial_fraction_of_traps_per_pha,&__pyx_n_s_serial_full_well_depths,&__pyx_n_s_serial_well_notch_depths,&__pyx_n_s_serial_well_fill_powers,&__pyx_n_s_serial_first_electron_fills,&__pyx_n_s_serial_trap_densities,&__pyx_n_s_serial_trap_release_timescales,&__pyx_n_s_serial_trap_third_params,&__pyx_n_s_serial_trap_fourth_params,&__pyx_n_s_serial_n_traps_ic,&__pyx_n_s_serial_n_traps_sc,&__pyx_n_s_serial_n_traps_ic_co,&__pyx_n_s_serial_n_traps_sc_co,&__pyx_n_s_serial_express,&__pyx_n_s_serial_window_offset,&__pyx_n_s_serial_window_start,&__pyx_n_s_serial_window_stop,&__pyx_n_s_serial_time_start,&__pyx_n_s_serial_time_stop,&__pyx_n_s_serial_prune_n_electrons,&__pyx_n_s_serial_prune_frequency,&__pyx_n_s_allow_negative_pixels,&__pyx_n_s_verbosity,&__pyx_n_s_iteration,0};
     PyObject* values[64] = {0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0};
-    if (unlikely(__pyx_kwds)) {
+    if (__pyx_kwds) {
       Py_ssize_t kw_args;
-      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
-      switch (pos_args) {
-        case 64: values[63] = PyTuple_GET_ITEM(__pyx_args, 63);
+      switch (__pyx_nargs) {
+        case 64: values[63] = __Pyx_Arg_FASTCALL(__pyx_args, 63);
         CYTHON_FALLTHROUGH;
-        case 63: values[62] = PyTuple_GET_ITEM(__pyx_args, 62);
+        case 63: values[62] = __Pyx_Arg_FASTCALL(__pyx_args, 62);
         CYTHON_FALLTHROUGH;
-        case 62: values[61] = PyTuple_GET_ITEM(__pyx_args, 61);
+        case 62: values[61] = __Pyx_Arg_FASTCALL(__pyx_args, 61);
         CYTHON_FALLTHROUGH;
-        case 61: values[60] = PyTuple_GET_ITEM(__pyx_args, 60);
+        case 61: values[60] = __Pyx_Arg_FASTCALL(__pyx_args, 60);
         CYTHON_FALLTHROUGH;
-        case 60: values[59] = PyTuple_GET_ITEM(__pyx_args, 59);
+        case 60: values[59] = __Pyx_Arg_FASTCALL(__pyx_args, 59);
         CYTHON_FALLTHROUGH;
-        case 59: values[58] = PyTuple_GET_ITEM(__pyx_args, 58);
+        case 59: values[58] = __Pyx_Arg_FASTCALL(__pyx_args, 58);
         CYTHON_FALLTHROUGH;
-        case 58: values[57] = PyTuple_GET_ITEM(__pyx_args, 57);
+        case 58: values[57] = __Pyx_Arg_FASTCALL(__pyx_args, 57);
         CYTHON_FALLTHROUGH;
-        case 57: values[56] = PyTuple_GET_ITEM(__pyx_args, 56);
+        case 57: values[56] = __Pyx_Arg_FASTCALL(__pyx_args, 56);
         CYTHON_FALLTHROUGH;
-        case 56: values[55] = PyTuple_GET_ITEM(__pyx_args, 55);
+        case 56: values[55] = __Pyx_Arg_FASTCALL(__pyx_args, 55);
         CYTHON_FALLTHROUGH;
-        case 55: values[54] = PyTuple_GET_ITEM(__pyx_args, 54);
+        case 55: values[54] = __Pyx_Arg_FASTCALL(__pyx_args, 54);
         CYTHON_FALLTHROUGH;
-        case 54: values[53] = PyTuple_GET_ITEM(__pyx_args, 53);
+        case 54: values[53] = __Pyx_Arg_FASTCALL(__pyx_args, 53);
         CYTHON_FALLTHROUGH;
-        case 53: values[52] = PyTuple_GET_ITEM(__pyx_args, 52);
+        case 53: values[52] = __Pyx_Arg_FASTCALL(__pyx_args, 52);
         CYTHON_FALLTHROUGH;
-        case 52: values[51] = PyTuple_GET_ITEM(__pyx_args, 51);
+        case 52: values[51] = __Pyx_Arg_FASTCALL(__pyx_args, 51);
         CYTHON_FALLTHROUGH;
-        case 51: values[50] = PyTuple_GET_ITEM(__pyx_args, 50);
+        case 51: values[50] = __Pyx_Arg_FASTCALL(__pyx_args, 50);
         CYTHON_FALLTHROUGH;
-        case 50: values[49] = PyTuple_GET_ITEM(__pyx_args, 49);
+        case 50: values[49] = __Pyx_Arg_FASTCALL(__pyx_args, 49);
         CYTHON_FALLTHROUGH;
-        case 49: values[48] = PyTuple_GET_ITEM(__pyx_args, 48);
+        case 49: values[48] = __Pyx_Arg_FASTCALL(__pyx_args, 48);
         CYTHON_FALLTHROUGH;
-        case 48: values[47] = PyTuple_GET_ITEM(__pyx_args, 47);
+        case 48: values[47] = __Pyx_Arg_FASTCALL(__pyx_args, 47);
         CYTHON_FALLTHROUGH;
-        case 47: values[46] = PyTuple_GET_ITEM(__pyx_args, 46);
+        case 47: values[46] = __Pyx_Arg_FASTCALL(__pyx_args, 46);
         CYTHON_FALLTHROUGH;
-        case 46: values[45] = PyTuple_GET_ITEM(__pyx_args, 45);
+        case 46: values[45] = __Pyx_Arg_FASTCALL(__pyx_args, 45);
         CYTHON_FALLTHROUGH;
-        case 45: values[44] = PyTuple_GET_ITEM(__pyx_args, 44);
+        case 45: values[44] = __Pyx_Arg_FASTCALL(__pyx_args, 44);
         CYTHON_FALLTHROUGH;
-        case 44: values[43] = PyTuple_GET_ITEM(__pyx_args, 43);
+        case 44: values[43] = __Pyx_Arg_FASTCALL(__pyx_args, 43);
         CYTHON_FALLTHROUGH;
-        case 43: values[42] = PyTuple_GET_ITEM(__pyx_args, 42);
+        case 43: values[42] = __Pyx_Arg_FASTCALL(__pyx_args, 42);
         CYTHON_FALLTHROUGH;
-        case 42: values[41] = PyTuple_GET_ITEM(__pyx_args, 41);
+        case 42: values[41] = __Pyx_Arg_FASTCALL(__pyx_args, 41);
         CYTHON_FALLTHROUGH;
-        case 41: values[40] = PyTuple_GET_ITEM(__pyx_args, 40);
+        case 41: values[40] = __Pyx_Arg_FASTCALL(__pyx_args, 40);
         CYTHON_FALLTHROUGH;
-        case 40: values[39] = PyTuple_GET_ITEM(__pyx_args, 39);
+        case 40: values[39] = __Pyx_Arg_FASTCALL(__pyx_args, 39);
         CYTHON_FALLTHROUGH;
-        case 39: values[38] = PyTuple_GET_ITEM(__pyx_args, 38);
+        case 39: values[38] = __Pyx_Arg_FASTCALL(__pyx_args, 38);
         CYTHON_FALLTHROUGH;
-        case 38: values[37] = PyTuple_GET_ITEM(__pyx_args, 37);
+        case 38: values[37] = __Pyx_Arg_FASTCALL(__pyx_args, 37);
         CYTHON_FALLTHROUGH;
-        case 37: values[36] = PyTuple_GET_ITEM(__pyx_args, 36);
+        case 37: values[36] = __Pyx_Arg_FASTCALL(__pyx_args, 36);
         CYTHON_FALLTHROUGH;
-        case 36: values[35] = PyTuple_GET_ITEM(__pyx_args, 35);
+        case 36: values[35] = __Pyx_Arg_FASTCALL(__pyx_args, 35);
         CYTHON_FALLTHROUGH;
-        case 35: values[34] = PyTuple_GET_ITEM(__pyx_args, 34);
+        case 35: values[34] = __Pyx_Arg_FASTCALL(__pyx_args, 34);
         CYTHON_FALLTHROUGH;
-        case 34: values[33] = PyTuple_GET_ITEM(__pyx_args, 33);
+        case 34: values[33] = __Pyx_Arg_FASTCALL(__pyx_args, 33);
         CYTHON_FALLTHROUGH;
-        case 33: values[32] = PyTuple_GET_ITEM(__pyx_args, 32);
+        case 33: values[32] = __Pyx_Arg_FASTCALL(__pyx_args, 32);
         CYTHON_FALLTHROUGH;
-        case 32: values[31] = PyTuple_GET_ITEM(__pyx_args, 31);
+        case 32: values[31] = __Pyx_Arg_FASTCALL(__pyx_args, 31);
         CYTHON_FALLTHROUGH;
-        case 31: values[30] = PyTuple_GET_ITEM(__pyx_args, 30);
+        case 31: values[30] = __Pyx_Arg_FASTCALL(__pyx_args, 30);
         CYTHON_FALLTHROUGH;
-        case 30: values[29] = PyTuple_GET_ITEM(__pyx_args, 29);
+        case 30: values[29] = __Pyx_Arg_FASTCALL(__pyx_args, 29);
         CYTHON_FALLTHROUGH;
-        case 29: values[28] = PyTuple_GET_ITEM(__pyx_args, 28);
+        case 29: values[28] = __Pyx_Arg_FASTCALL(__pyx_args, 28);
         CYTHON_FALLTHROUGH;
-        case 28: values[27] = PyTuple_GET_ITEM(__pyx_args, 27);
+        case 28: values[27] = __Pyx_Arg_FASTCALL(__pyx_args, 27);
         CYTHON_FALLTHROUGH;
-        case 27: values[26] = PyTuple_GET_ITEM(__pyx_args, 26);
+        case 27: values[26] = __Pyx_Arg_FASTCALL(__pyx_args, 26);
         CYTHON_FALLTHROUGH;
-        case 26: values[25] = PyTuple_GET_ITEM(__pyx_args, 25);
+        case 26: values[25] = __Pyx_Arg_FASTCALL(__pyx_args, 25);
         CYTHON_FALLTHROUGH;
-        case 25: values[24] = PyTuple_GET_ITEM(__pyx_args, 24);
+        case 25: values[24] = __Pyx_Arg_FASTCALL(__pyx_args, 24);
         CYTHON_FALLTHROUGH;
-        case 24: values[23] = PyTuple_GET_ITEM(__pyx_args, 23);
+        case 24: values[23] = __Pyx_Arg_FASTCALL(__pyx_args, 23);
         CYTHON_FALLTHROUGH;
-        case 23: values[22] = PyTuple_GET_ITEM(__pyx_args, 22);
+        case 23: values[22] = __Pyx_Arg_FASTCALL(__pyx_args, 22);
         CYTHON_FALLTHROUGH;
-        case 22: values[21] = PyTuple_GET_ITEM(__pyx_args, 21);
+        case 22: values[21] = __Pyx_Arg_FASTCALL(__pyx_args, 21);
         CYTHON_FALLTHROUGH;
-        case 21: values[20] = PyTuple_GET_ITEM(__pyx_args, 20);
+        case 21: values[20] = __Pyx_Arg_FASTCALL(__pyx_args, 20);
         CYTHON_FALLTHROUGH;
-        case 20: values[19] = PyTuple_GET_ITEM(__pyx_args, 19);
+        case 20: values[19] = __Pyx_Arg_FASTCALL(__pyx_args, 19);
         CYTHON_FALLTHROUGH;
-        case 19: values[18] = PyTuple_GET_ITEM(__pyx_args, 18);
+        case 19: values[18] = __Pyx_Arg_FASTCALL(__pyx_args, 18);
         CYTHON_FALLTHROUGH;
-        case 18: values[17] = PyTuple_GET_ITEM(__pyx_args, 17);
+        case 18: values[17] = __Pyx_Arg_FASTCALL(__pyx_args, 17);
         CYTHON_FALLTHROUGH;
-        case 17: values[16] = PyTuple_GET_ITEM(__pyx_args, 16);
+        case 17: values[16] = __Pyx_Arg_FASTCALL(__pyx_args, 16);
         CYTHON_FALLTHROUGH;
-        case 16: values[15] = PyTuple_GET_ITEM(__pyx_args, 15);
+        case 16: values[15] = __Pyx_Arg_FASTCALL(__pyx_args, 15);
         CYTHON_FALLTHROUGH;
-        case 15: values[14] = PyTuple_GET_ITEM(__pyx_args, 14);
+        case 15: values[14] = __Pyx_Arg_FASTCALL(__pyx_args, 14);
         CYTHON_FALLTHROUGH;
-        case 14: values[13] = PyTuple_GET_ITEM(__pyx_args, 13);
+        case 14: values[13] = __Pyx_Arg_FASTCALL(__pyx_args, 13);
         CYTHON_FALLTHROUGH;
-        case 13: values[12] = PyTuple_GET_ITEM(__pyx_args, 12);
+        case 13: values[12] = __Pyx_Arg_FASTCALL(__pyx_args, 12);
         CYTHON_FALLTHROUGH;
-        case 12: values[11] = PyTuple_GET_ITEM(__pyx_args, 11);
+        case 12: values[11] = __Pyx_Arg_FASTCALL(__pyx_args, 11);
         CYTHON_FALLTHROUGH;
-        case 11: values[10] = PyTuple_GET_ITEM(__pyx_args, 10);
+        case 11: values[10] = __Pyx_Arg_FASTCALL(__pyx_args, 10);
         CYTHON_FALLTHROUGH;
-        case 10: values[9] = PyTuple_GET_ITEM(__pyx_args, 9);
+        case 10: values[9] = __Pyx_Arg_FASTCALL(__pyx_args, 9);
         CYTHON_FALLTHROUGH;
-        case  9: values[8] = PyTuple_GET_ITEM(__pyx_args, 8);
+        case  9: values[8] = __Pyx_Arg_FASTCALL(__pyx_args, 8);
         CYTHON_FALLTHROUGH;
-        case  8: values[7] = PyTuple_GET_ITEM(__pyx_args, 7);
+        case  8: values[7] = __Pyx_Arg_FASTCALL(__pyx_args, 7);
         CYTHON_FALLTHROUGH;
-        case  7: values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
+        case  7: values[6] = __Pyx_Arg_FASTCALL(__pyx_args, 6);
         CYTHON_FALLTHROUGH;
-        case  6: values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
+        case  6: values[5] = __Pyx_Arg_FASTCALL(__pyx_args, 5);
         CYTHON_FALLTHROUGH;
-        case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
+        case  5: values[4] = __Pyx_Arg_FASTCALL(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
-        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
+        case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
-        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
-      kw_args = PyDict_Size(__pyx_kwds);
-      switch (pos_args) {
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_image)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_image)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
-        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_parallel_dwell_times)) != 0)) kw_args--;
+        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_parallel_dwell_times)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 1); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 1); __PYX_ERR(2, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
-        if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_parallel_prescan_offset)) != 0)) kw_args--;
+        if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_parallel_prescan_offset)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 2); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 2); __PYX_ERR(2, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
-        if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_parallel_overscan_start)) != 0)) kw_args--;
+        if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_parallel_overscan_start)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 3); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 3); __PYX_ERR(2, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
-        if (likely((values[4] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_parallel_empty_traps_between_col)) != 0)) kw_args--;
+        if (likely((values[4] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_parallel_empty_traps_between_col)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 4); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 4); __PYX_ERR(2, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
-        if (likely((values[5] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_parallel_empty_traps_for_first_t)) != 0)) kw_args--;
+        if (likely((values[5] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_parallel_empty_traps_for_first_t)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 5); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 5); __PYX_ERR(2, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  6:
-        if (likely((values[6] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_parallel_force_release_away_from)) != 0)) kw_args--;
+        if (likely((values[6] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_parallel_force_release_away_from)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 6); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 6); __PYX_ERR(2, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  7:
-        if (likely((values[7] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_parallel_use_integer_express_mat)) != 0)) kw_args--;
+        if (likely((values[7] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_parallel_use_integer_express_mat)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 7); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 7); __PYX_ERR(2, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  8:
-        if (likely((values[8] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_parallel_n_pumps)) != 0)) kw_args--;
+        if (likely((values[8] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_parallel_n_pumps)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 8); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 8); __PYX_ERR(2, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  9:
-        if (likely((values[9] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_parallel_roe_type)) != 0)) kw_args--;
+        if (likely((values[9] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_parallel_roe_type)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 9); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 9); __PYX_ERR(2, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 10:
-        if (likely((values[10] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_parallel_fraction_of_traps_per_p)) != 0)) kw_args--;
+        if (likely((values[10] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_parallel_fraction_of_traps_per_p)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 10); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 10); __PYX_ERR(2, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 11:
-        if (likely((values[11] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_parallel_full_well_depths)) != 0)) kw_args--;
+        if (likely((values[11] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_parallel_full_well_depths)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 11); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 11); __PYX_ERR(2, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 12:
-        if (likely((values[12] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_parallel_well_notch_depths)) != 0)) kw_args--;
+        if (likely((values[12] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_parallel_well_notch_depths)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 12); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 12); __PYX_ERR(2, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 13:
-        if (likely((values[13] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_parallel_well_fill_powers)) != 0)) kw_args--;
+        if (likely((values[13] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_parallel_well_fill_powers)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 13); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 13); __PYX_ERR(2, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 14:
-        if (likely((values[14] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_parallel_first_electron_fills)) != 0)) kw_args--;
+        if (likely((values[14] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_parallel_first_electron_fills)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 14); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 14); __PYX_ERR(2, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 15:
-        if (likely((values[15] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_parallel_trap_densities)) != 0)) kw_args--;
+        if (likely((values[15] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_parallel_trap_densities)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 15); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 15); __PYX_ERR(2, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 16:
-        if (likely((values[16] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_parallel_trap_release_timescales)) != 0)) kw_args--;
+        if (likely((values[16] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_parallel_trap_release_timescales)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 16); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 16); __PYX_ERR(2, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 17:
-        if (likely((values[17] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_parallel_trap_third_params)) != 0)) kw_args--;
+        if (likely((values[17] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_parallel_trap_third_params)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 17); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 17); __PYX_ERR(2, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 18:
-        if (likely((values[18] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_parallel_trap_fourth_params)) != 0)) kw_args--;
+        if (likely((values[18] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_parallel_trap_fourth_params)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 18); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 18); __PYX_ERR(2, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 19:
-        if (likely((values[19] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_parallel_n_traps_ic)) != 0)) kw_args--;
+        if (likely((values[19] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_parallel_n_traps_ic)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 19); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 19); __PYX_ERR(2, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 20:
-        if (likely((values[20] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_parallel_n_traps_sc)) != 0)) kw_args--;
+        if (likely((values[20] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_parallel_n_traps_sc)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 20); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 20); __PYX_ERR(2, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 21:
-        if (likely((values[21] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_parallel_n_traps_ic_co)) != 0)) kw_args--;
+        if (likely((values[21] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_parallel_n_traps_ic_co)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 21); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 21); __PYX_ERR(2, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 22:
-        if (likely((values[22] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_parallel_n_traps_sc_co)) != 0)) kw_args--;
+        if (likely((values[22] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_parallel_n_traps_sc_co)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 22); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 22); __PYX_ERR(2, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 23:
-        if (likely((values[23] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_parallel_express)) != 0)) kw_args--;
+        if (likely((values[23] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_parallel_express)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 23); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 23); __PYX_ERR(2, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 24:
-        if (likely((values[24] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_parallel_window_offset)) != 0)) kw_args--;
+        if (likely((values[24] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_parallel_window_offset)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 24); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 24); __PYX_ERR(2, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 25:
-        if (likely((values[25] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_parallel_window_start)) != 0)) kw_args--;
+        if (likely((values[25] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_parallel_window_start)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 25); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 25); __PYX_ERR(2, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 26:
-        if (likely((values[26] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_parallel_window_stop)) != 0)) kw_args--;
+        if (likely((values[26] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_parallel_window_stop)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 26); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 26); __PYX_ERR(2, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 27:
-        if (likely((values[27] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_parallel_time_start)) != 0)) kw_args--;
+        if (likely((values[27] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_parallel_time_start)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 27); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 27); __PYX_ERR(2, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 28:
-        if (likely((values[28] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_parallel_time_stop)) != 0)) kw_args--;
+        if (likely((values[28] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_parallel_time_stop)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 28); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 28); __PYX_ERR(2, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 29:
-        if (likely((values[29] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_parallel_prune_n_electrons)) != 0)) kw_args--;
+        if (likely((values[29] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_parallel_prune_n_electrons)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 29); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 29); __PYX_ERR(2, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 30:
-        if (likely((values[30] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_parallel_prune_frequency)) != 0)) kw_args--;
+        if (likely((values[30] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_parallel_prune_frequency)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 30); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 30); __PYX_ERR(2, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 31:
-        if (likely((values[31] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_serial_dwell_times)) != 0)) kw_args--;
+        if (likely((values[31] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_serial_dwell_times)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 31); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 31); __PYX_ERR(2, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 32:
-        if (likely((values[32] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_serial_prescan_offset)) != 0)) kw_args--;
+        if (likely((values[32] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_serial_prescan_offset)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 32); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 32); __PYX_ERR(2, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 33:
-        if (likely((values[33] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_serial_overscan_start)) != 0)) kw_args--;
+        if (likely((values[33] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_serial_overscan_start)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 33); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 33); __PYX_ERR(2, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 34:
-        if (likely((values[34] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_serial_empty_traps_between_colum)) != 0)) kw_args--;
+        if (likely((values[34] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_serial_empty_traps_between_colum)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 34); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 34); __PYX_ERR(2, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 35:
-        if (likely((values[35] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_serial_empty_traps_for_first_tra)) != 0)) kw_args--;
+        if (likely((values[35] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_serial_empty_traps_for_first_tra)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 35); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 35); __PYX_ERR(2, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 36:
-        if (likely((values[36] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_serial_force_release_away_from_r)) != 0)) kw_args--;
+        if (likely((values[36] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_serial_force_release_away_from_r)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 36); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 36); __PYX_ERR(2, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 37:
-        if (likely((values[37] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_serial_use_integer_express_matri)) != 0)) kw_args--;
+        if (likely((values[37] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_serial_use_integer_express_matri)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 37); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 37); __PYX_ERR(2, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 38:
-        if (likely((values[38] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_serial_n_pumps)) != 0)) kw_args--;
+        if (likely((values[38] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_serial_n_pumps)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 38); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 38); __PYX_ERR(2, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 39:
-        if (likely((values[39] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_serial_roe_type)) != 0)) kw_args--;
+        if (likely((values[39] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_serial_roe_type)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 39); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 39); __PYX_ERR(2, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 40:
-        if (likely((values[40] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_serial_fraction_of_traps_per_pha)) != 0)) kw_args--;
+        if (likely((values[40] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_serial_fraction_of_traps_per_pha)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 40); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 40); __PYX_ERR(2, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 41:
-        if (likely((values[41] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_serial_full_well_depths)) != 0)) kw_args--;
+        if (likely((values[41] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_serial_full_well_depths)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 41); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 41); __PYX_ERR(2, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 42:
-        if (likely((values[42] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_serial_well_notch_depths)) != 0)) kw_args--;
+        if (likely((values[42] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_serial_well_notch_depths)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 42); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 42); __PYX_ERR(2, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 43:
-        if (likely((values[43] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_serial_well_fill_powers)) != 0)) kw_args--;
+        if (likely((values[43] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_serial_well_fill_powers)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 43); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 43); __PYX_ERR(2, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 44:
-        if (likely((values[44] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_serial_first_electron_fills)) != 0)) kw_args--;
+        if (likely((values[44] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_serial_first_electron_fills)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 44); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 44); __PYX_ERR(2, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 45:
-        if (likely((values[45] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_serial_trap_densities)) != 0)) kw_args--;
+        if (likely((values[45] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_serial_trap_densities)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 45); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 45); __PYX_ERR(2, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 46:
-        if (likely((values[46] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_serial_trap_release_timescales)) != 0)) kw_args--;
+        if (likely((values[46] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_serial_trap_release_timescales)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 46); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 46); __PYX_ERR(2, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 47:
-        if (likely((values[47] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_serial_trap_third_params)) != 0)) kw_args--;
+        if (likely((values[47] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_serial_trap_third_params)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 47); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 47); __PYX_ERR(2, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 48:
-        if (likely((values[48] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_serial_trap_fourth_params)) != 0)) kw_args--;
+        if (likely((values[48] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_serial_trap_fourth_params)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 48); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 48); __PYX_ERR(2, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 49:
-        if (likely((values[49] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_serial_n_traps_ic)) != 0)) kw_args--;
+        if (likely((values[49] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_serial_n_traps_ic)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 49); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 49); __PYX_ERR(2, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 50:
-        if (likely((values[50] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_serial_n_traps_sc)) != 0)) kw_args--;
+        if (likely((values[50] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_serial_n_traps_sc)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 50); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 50); __PYX_ERR(2, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 51:
-        if (likely((values[51] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_serial_n_traps_ic_co)) != 0)) kw_args--;
+        if (likely((values[51] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_serial_n_traps_ic_co)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 51); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 51); __PYX_ERR(2, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 52:
-        if (likely((values[52] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_serial_n_traps_sc_co)) != 0)) kw_args--;
+        if (likely((values[52] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_serial_n_traps_sc_co)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 52); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 52); __PYX_ERR(2, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 53:
-        if (likely((values[53] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_serial_express)) != 0)) kw_args--;
+        if (likely((values[53] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_serial_express)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 53); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 53); __PYX_ERR(2, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 54:
-        if (likely((values[54] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_serial_window_offset)) != 0)) kw_args--;
+        if (likely((values[54] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_serial_window_offset)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 54); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 54); __PYX_ERR(2, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 55:
-        if (likely((values[55] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_serial_window_start)) != 0)) kw_args--;
+        if (likely((values[55] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_serial_window_start)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 55); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 55); __PYX_ERR(2, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 56:
-        if (likely((values[56] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_serial_window_stop)) != 0)) kw_args--;
+        if (likely((values[56] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_serial_window_stop)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 56); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 56); __PYX_ERR(2, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 57:
-        if (likely((values[57] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_serial_time_start)) != 0)) kw_args--;
+        if (likely((values[57] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_serial_time_start)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 57); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 57); __PYX_ERR(2, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 58:
-        if (likely((values[58] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_serial_time_stop)) != 0)) kw_args--;
+        if (likely((values[58] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_serial_time_stop)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 58); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 58); __PYX_ERR(2, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 59:
-        if (likely((values[59] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_serial_prune_n_electrons)) != 0)) kw_args--;
+        if (likely((values[59] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_serial_prune_n_electrons)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 59); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 59); __PYX_ERR(2, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 60:
-        if (likely((values[60] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_serial_prune_frequency)) != 0)) kw_args--;
+        if (likely((values[60] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_serial_prune_frequency)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 60); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 60); __PYX_ERR(2, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 61:
-        if (likely((values[61] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_allow_negative_pixels)) != 0)) kw_args--;
+        if (likely((values[61] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_allow_negative_pixels)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 61); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 61); __PYX_ERR(2, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 62:
-        if (likely((values[62] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_verbosity)) != 0)) kw_args--;
+        if (likely((values[62] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_verbosity)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 62); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 62); __PYX_ERR(2, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 63:
-        if (likely((values[63] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_iteration)) != 0)) kw_args--;
+        if (likely((values[63] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_iteration)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 131, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 63); __PYX_ERR(0, 131, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, 63); __PYX_ERR(2, 131, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "cy_add_cti") < 0)) __PYX_ERR(0, 131, __pyx_L3_error)
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "cy_add_cti") < 0)) __PYX_ERR(2, 131, __pyx_L3_error)
       }
-    } else if (PyTuple_GET_SIZE(__pyx_args) != 64) {
+    } else if (unlikely(__pyx_nargs != 64)) {
       goto __pyx_L5_argtuple_error;
     } else {
-      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-      values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
-      values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
-      values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
-      values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
-      values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
-      values[7] = PyTuple_GET_ITEM(__pyx_args, 7);
-      values[8] = PyTuple_GET_ITEM(__pyx_args, 8);
-      values[9] = PyTuple_GET_ITEM(__pyx_args, 9);
-      values[10] = PyTuple_GET_ITEM(__pyx_args, 10);
-      values[11] = PyTuple_GET_ITEM(__pyx_args, 11);
-      values[12] = PyTuple_GET_ITEM(__pyx_args, 12);
-      values[13] = PyTuple_GET_ITEM(__pyx_args, 13);
-      values[14] = PyTuple_GET_ITEM(__pyx_args, 14);
-      values[15] = PyTuple_GET_ITEM(__pyx_args, 15);
-      values[16] = PyTuple_GET_ITEM(__pyx_args, 16);
-      values[17] = PyTuple_GET_ITEM(__pyx_args, 17);
-      values[18] = PyTuple_GET_ITEM(__pyx_args, 18);
-      values[19] = PyTuple_GET_ITEM(__pyx_args, 19);
-      values[20] = PyTuple_GET_ITEM(__pyx_args, 20);
-      values[21] = PyTuple_GET_ITEM(__pyx_args, 21);
-      values[22] = PyTuple_GET_ITEM(__pyx_args, 22);
-      values[23] = PyTuple_GET_ITEM(__pyx_args, 23);
-      values[24] = PyTuple_GET_ITEM(__pyx_args, 24);
-      values[25] = PyTuple_GET_ITEM(__pyx_args, 25);
-      values[26] = PyTuple_GET_ITEM(__pyx_args, 26);
-      values[27] = PyTuple_GET_ITEM(__pyx_args, 27);
-      values[28] = PyTuple_GET_ITEM(__pyx_args, 28);
-      values[29] = PyTuple_GET_ITEM(__pyx_args, 29);
-      values[30] = PyTuple_GET_ITEM(__pyx_args, 30);
-      values[31] = PyTuple_GET_ITEM(__pyx_args, 31);
-      values[32] = PyTuple_GET_ITEM(__pyx_args, 32);
-      values[33] = PyTuple_GET_ITEM(__pyx_args, 33);
-      values[34] = PyTuple_GET_ITEM(__pyx_args, 34);
-      values[35] = PyTuple_GET_ITEM(__pyx_args, 35);
-      values[36] = PyTuple_GET_ITEM(__pyx_args, 36);
-      values[37] = PyTuple_GET_ITEM(__pyx_args, 37);
-      values[38] = PyTuple_GET_ITEM(__pyx_args, 38);
-      values[39] = PyTuple_GET_ITEM(__pyx_args, 39);
-      values[40] = PyTuple_GET_ITEM(__pyx_args, 40);
-      values[41] = PyTuple_GET_ITEM(__pyx_args, 41);
-      values[42] = PyTuple_GET_ITEM(__pyx_args, 42);
-      values[43] = PyTuple_GET_ITEM(__pyx_args, 43);
-      values[44] = PyTuple_GET_ITEM(__pyx_args, 44);
-      values[45] = PyTuple_GET_ITEM(__pyx_args, 45);
-      values[46] = PyTuple_GET_ITEM(__pyx_args, 46);
-      values[47] = PyTuple_GET_ITEM(__pyx_args, 47);
-      values[48] = PyTuple_GET_ITEM(__pyx_args, 48);
-      values[49] = PyTuple_GET_ITEM(__pyx_args, 49);
-      values[50] = PyTuple_GET_ITEM(__pyx_args, 50);
-      values[51] = PyTuple_GET_ITEM(__pyx_args, 51);
-      values[52] = PyTuple_GET_ITEM(__pyx_args, 52);
-      values[53] = PyTuple_GET_ITEM(__pyx_args, 53);
-      values[54] = PyTuple_GET_ITEM(__pyx_args, 54);
-      values[55] = PyTuple_GET_ITEM(__pyx_args, 55);
-      values[56] = PyTuple_GET_ITEM(__pyx_args, 56);
-      values[57] = PyTuple_GET_ITEM(__pyx_args, 57);
-      values[58] = PyTuple_GET_ITEM(__pyx_args, 58);
-      values[59] = PyTuple_GET_ITEM(__pyx_args, 59);
-      values[60] = PyTuple_GET_ITEM(__pyx_args, 60);
-      values[61] = PyTuple_GET_ITEM(__pyx_args, 61);
-      values[62] = PyTuple_GET_ITEM(__pyx_args, 62);
-      values[63] = PyTuple_GET_ITEM(__pyx_args, 63);
+      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+      values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
+      values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
+      values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
+      values[4] = __Pyx_Arg_FASTCALL(__pyx_args, 4);
+      values[5] = __Pyx_Arg_FASTCALL(__pyx_args, 5);
+      values[6] = __Pyx_Arg_FASTCALL(__pyx_args, 6);
+      values[7] = __Pyx_Arg_FASTCALL(__pyx_args, 7);
+      values[8] = __Pyx_Arg_FASTCALL(__pyx_args, 8);
+      values[9] = __Pyx_Arg_FASTCALL(__pyx_args, 9);
+      values[10] = __Pyx_Arg_FASTCALL(__pyx_args, 10);
+      values[11] = __Pyx_Arg_FASTCALL(__pyx_args, 11);
+      values[12] = __Pyx_Arg_FASTCALL(__pyx_args, 12);
+      values[13] = __Pyx_Arg_FASTCALL(__pyx_args, 13);
+      values[14] = __Pyx_Arg_FASTCALL(__pyx_args, 14);
+      values[15] = __Pyx_Arg_FASTCALL(__pyx_args, 15);
+      values[16] = __Pyx_Arg_FASTCALL(__pyx_args, 16);
+      values[17] = __Pyx_Arg_FASTCALL(__pyx_args, 17);
+      values[18] = __Pyx_Arg_FASTCALL(__pyx_args, 18);
+      values[19] = __Pyx_Arg_FASTCALL(__pyx_args, 19);
+      values[20] = __Pyx_Arg_FASTCALL(__pyx_args, 20);
+      values[21] = __Pyx_Arg_FASTCALL(__pyx_args, 21);
+      values[22] = __Pyx_Arg_FASTCALL(__pyx_args, 22);
+      values[23] = __Pyx_Arg_FASTCALL(__pyx_args, 23);
+      values[24] = __Pyx_Arg_FASTCALL(__pyx_args, 24);
+      values[25] = __Pyx_Arg_FASTCALL(__pyx_args, 25);
+      values[26] = __Pyx_Arg_FASTCALL(__pyx_args, 26);
+      values[27] = __Pyx_Arg_FASTCALL(__pyx_args, 27);
+      values[28] = __Pyx_Arg_FASTCALL(__pyx_args, 28);
+      values[29] = __Pyx_Arg_FASTCALL(__pyx_args, 29);
+      values[30] = __Pyx_Arg_FASTCALL(__pyx_args, 30);
+      values[31] = __Pyx_Arg_FASTCALL(__pyx_args, 31);
+      values[32] = __Pyx_Arg_FASTCALL(__pyx_args, 32);
+      values[33] = __Pyx_Arg_FASTCALL(__pyx_args, 33);
+      values[34] = __Pyx_Arg_FASTCALL(__pyx_args, 34);
+      values[35] = __Pyx_Arg_FASTCALL(__pyx_args, 35);
+      values[36] = __Pyx_Arg_FASTCALL(__pyx_args, 36);
+      values[37] = __Pyx_Arg_FASTCALL(__pyx_args, 37);
+      values[38] = __Pyx_Arg_FASTCALL(__pyx_args, 38);
+      values[39] = __Pyx_Arg_FASTCALL(__pyx_args, 39);
+      values[40] = __Pyx_Arg_FASTCALL(__pyx_args, 40);
+      values[41] = __Pyx_Arg_FASTCALL(__pyx_args, 41);
+      values[42] = __Pyx_Arg_FASTCALL(__pyx_args, 42);
+      values[43] = __Pyx_Arg_FASTCALL(__pyx_args, 43);
+      values[44] = __Pyx_Arg_FASTCALL(__pyx_args, 44);
+      values[45] = __Pyx_Arg_FASTCALL(__pyx_args, 45);
+      values[46] = __Pyx_Arg_FASTCALL(__pyx_args, 46);
+      values[47] = __Pyx_Arg_FASTCALL(__pyx_args, 47);
+      values[48] = __Pyx_Arg_FASTCALL(__pyx_args, 48);
+      values[49] = __Pyx_Arg_FASTCALL(__pyx_args, 49);
+      values[50] = __Pyx_Arg_FASTCALL(__pyx_args, 50);
+      values[51] = __Pyx_Arg_FASTCALL(__pyx_args, 51);
+      values[52] = __Pyx_Arg_FASTCALL(__pyx_args, 52);
+      values[53] = __Pyx_Arg_FASTCALL(__pyx_args, 53);
+      values[54] = __Pyx_Arg_FASTCALL(__pyx_args, 54);
+      values[55] = __Pyx_Arg_FASTCALL(__pyx_args, 55);
+      values[56] = __Pyx_Arg_FASTCALL(__pyx_args, 56);
+      values[57] = __Pyx_Arg_FASTCALL(__pyx_args, 57);
+      values[58] = __Pyx_Arg_FASTCALL(__pyx_args, 58);
+      values[59] = __Pyx_Arg_FASTCALL(__pyx_args, 59);
+      values[60] = __Pyx_Arg_FASTCALL(__pyx_args, 60);
+      values[61] = __Pyx_Arg_FASTCALL(__pyx_args, 61);
+      values[62] = __Pyx_Arg_FASTCALL(__pyx_args, 62);
+      values[63] = __Pyx_Arg_FASTCALL(__pyx_args, 63);
     }
     __pyx_v_image = ((PyArrayObject *)values[0]);
     __pyx_v_parallel_dwell_times = ((PyArrayObject *)values[1]);
-    __pyx_v_parallel_prescan_offset = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_parallel_prescan_offset == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 138, __pyx_L3_error)
-    __pyx_v_parallel_overscan_start = __Pyx_PyInt_As_int(values[3]); if (unlikely((__pyx_v_parallel_overscan_start == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 139, __pyx_L3_error)
-    __pyx_v_parallel_empty_traps_between_columns = __Pyx_PyInt_As_int(values[4]); if (unlikely((__pyx_v_parallel_empty_traps_between_columns == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 140, __pyx_L3_error)
-    __pyx_v_parallel_empty_traps_for_first_transfers = __Pyx_PyInt_As_int(values[5]); if (unlikely((__pyx_v_parallel_empty_traps_for_first_transfers == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 141, __pyx_L3_error)
-    __pyx_v_parallel_force_release_away_from_readout = __Pyx_PyInt_As_int(values[6]); if (unlikely((__pyx_v_parallel_force_release_away_from_readout == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 142, __pyx_L3_error)
-    __pyx_v_parallel_use_integer_express_matrix = __Pyx_PyInt_As_int(values[7]); if (unlikely((__pyx_v_parallel_use_integer_express_matrix == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 143, __pyx_L3_error)
-    __pyx_v_parallel_n_pumps = __Pyx_PyInt_As_int(values[8]); if (unlikely((__pyx_v_parallel_n_pumps == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 144, __pyx_L3_error)
-    __pyx_v_parallel_roe_type = __Pyx_PyInt_As_int(values[9]); if (unlikely((__pyx_v_parallel_roe_type == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 145, __pyx_L3_error)
+    __pyx_v_parallel_prescan_offset = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_parallel_prescan_offset == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 138, __pyx_L3_error)
+    __pyx_v_parallel_overscan_start = __Pyx_PyInt_As_int(values[3]); if (unlikely((__pyx_v_parallel_overscan_start == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 139, __pyx_L3_error)
+    __pyx_v_parallel_empty_traps_between_columns = __Pyx_PyInt_As_int(values[4]); if (unlikely((__pyx_v_parallel_empty_traps_between_columns == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 140, __pyx_L3_error)
+    __pyx_v_parallel_empty_traps_for_first_transfers = __Pyx_PyInt_As_int(values[5]); if (unlikely((__pyx_v_parallel_empty_traps_for_first_transfers == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 141, __pyx_L3_error)
+    __pyx_v_parallel_force_release_away_from_readout = __Pyx_PyInt_As_int(values[6]); if (unlikely((__pyx_v_parallel_force_release_away_from_readout == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 142, __pyx_L3_error)
+    __pyx_v_parallel_use_integer_express_matrix = __Pyx_PyInt_As_int(values[7]); if (unlikely((__pyx_v_parallel_use_integer_express_matrix == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 143, __pyx_L3_error)
+    __pyx_v_parallel_n_pumps = __Pyx_PyInt_As_int(values[8]); if (unlikely((__pyx_v_parallel_n_pumps == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 144, __pyx_L3_error)
+    __pyx_v_parallel_roe_type = __Pyx_PyInt_As_int(values[9]); if (unlikely((__pyx_v_parallel_roe_type == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 145, __pyx_L3_error)
     __pyx_v_parallel_fraction_of_traps_per_phase = ((PyArrayObject *)values[10]);
     __pyx_v_parallel_full_well_depths = ((PyArrayObject *)values[11]);
     __pyx_v_parallel_well_notch_depths = ((PyArrayObject *)values[12]);
     __pyx_v_parallel_well_fill_powers = ((PyArrayObject *)values[13]);
     __pyx_v_parallel_first_electron_fills = ((PyArrayObject *)values[14]);
     __pyx_v_parallel_trap_densities = ((PyArrayObject *)values[15]);
     __pyx_v_parallel_trap_release_timescales = ((PyArrayObject *)values[16]);
     __pyx_v_parallel_trap_third_params = ((PyArrayObject *)values[17]);
     __pyx_v_parallel_trap_fourth_params = ((PyArrayObject *)values[18]);
-    __pyx_v_parallel_n_traps_ic = __Pyx_PyInt_As_int(values[19]); if (unlikely((__pyx_v_parallel_n_traps_ic == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 157, __pyx_L3_error)
-    __pyx_v_parallel_n_traps_sc = __Pyx_PyInt_As_int(values[20]); if (unlikely((__pyx_v_parallel_n_traps_sc == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 158, __pyx_L3_error)
-    __pyx_v_parallel_n_traps_ic_co = __Pyx_PyInt_As_int(values[21]); if (unlikely((__pyx_v_parallel_n_traps_ic_co == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 159, __pyx_L3_error)
-    __pyx_v_parallel_n_traps_sc_co = __Pyx_PyInt_As_int(values[22]); if (unlikely((__pyx_v_parallel_n_traps_sc_co == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 160, __pyx_L3_error)
-    __pyx_v_parallel_express = __Pyx_PyInt_As_int(values[23]); if (unlikely((__pyx_v_parallel_express == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 162, __pyx_L3_error)
-    __pyx_v_parallel_window_offset = __Pyx_PyInt_As_int(values[24]); if (unlikely((__pyx_v_parallel_window_offset == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 163, __pyx_L3_error)
-    __pyx_v_parallel_window_start = __Pyx_PyInt_As_int(values[25]); if (unlikely((__pyx_v_parallel_window_start == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 164, __pyx_L3_error)
-    __pyx_v_parallel_window_stop = __Pyx_PyInt_As_int(values[26]); if (unlikely((__pyx_v_parallel_window_stop == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 165, __pyx_L3_error)
-    __pyx_v_parallel_time_start = __Pyx_PyInt_As_int(values[27]); if (unlikely((__pyx_v_parallel_time_start == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 166, __pyx_L3_error)
-    __pyx_v_parallel_time_stop = __Pyx_PyInt_As_int(values[28]); if (unlikely((__pyx_v_parallel_time_stop == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 167, __pyx_L3_error)
+    __pyx_v_parallel_n_traps_ic = __Pyx_PyInt_As_int(values[19]); if (unlikely((__pyx_v_parallel_n_traps_ic == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 157, __pyx_L3_error)
+    __pyx_v_parallel_n_traps_sc = __Pyx_PyInt_As_int(values[20]); if (unlikely((__pyx_v_parallel_n_traps_sc == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 158, __pyx_L3_error)
+    __pyx_v_parallel_n_traps_ic_co = __Pyx_PyInt_As_int(values[21]); if (unlikely((__pyx_v_parallel_n_traps_ic_co == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 159, __pyx_L3_error)
+    __pyx_v_parallel_n_traps_sc_co = __Pyx_PyInt_As_int(values[22]); if (unlikely((__pyx_v_parallel_n_traps_sc_co == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 160, __pyx_L3_error)
+    __pyx_v_parallel_express = __Pyx_PyInt_As_int(values[23]); if (unlikely((__pyx_v_parallel_express == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 162, __pyx_L3_error)
+    __pyx_v_parallel_window_offset = __Pyx_PyInt_As_int(values[24]); if (unlikely((__pyx_v_parallel_window_offset == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 163, __pyx_L3_error)
+    __pyx_v_parallel_window_start = __Pyx_PyInt_As_int(values[25]); if (unlikely((__pyx_v_parallel_window_start == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 164, __pyx_L3_error)
+    __pyx_v_parallel_window_stop = __Pyx_PyInt_As_int(values[26]); if (unlikely((__pyx_v_parallel_window_stop == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 165, __pyx_L3_error)
+    __pyx_v_parallel_time_start = __Pyx_PyInt_As_int(values[27]); if (unlikely((__pyx_v_parallel_time_start == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 166, __pyx_L3_error)
+    __pyx_v_parallel_time_stop = __Pyx_PyInt_As_int(values[28]); if (unlikely((__pyx_v_parallel_time_stop == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 167, __pyx_L3_error)
     __pyx_v_parallel_prune_n_electrons = ((PyArrayObject *)values[29]);
-    __pyx_v_parallel_prune_frequency = __Pyx_PyInt_As_int(values[30]); if (unlikely((__pyx_v_parallel_prune_frequency == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 169, __pyx_L3_error)
+    __pyx_v_parallel_prune_frequency = __Pyx_PyInt_As_int(values[30]); if (unlikely((__pyx_v_parallel_prune_frequency == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 169, __pyx_L3_error)
     __pyx_v_serial_dwell_times = ((PyArrayObject *)values[31]);
-    __pyx_v_serial_prescan_offset = __Pyx_PyInt_As_int(values[32]); if (unlikely((__pyx_v_serial_prescan_offset == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 175, __pyx_L3_error)
-    __pyx_v_serial_overscan_start = __Pyx_PyInt_As_int(values[33]); if (unlikely((__pyx_v_serial_overscan_start == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 176, __pyx_L3_error)
-    __pyx_v_serial_empty_traps_between_columns = __Pyx_PyInt_As_int(values[34]); if (unlikely((__pyx_v_serial_empty_traps_between_columns == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 177, __pyx_L3_error)
-    __pyx_v_serial_empty_traps_for_first_transfers = __Pyx_PyInt_As_int(values[35]); if (unlikely((__pyx_v_serial_empty_traps_for_first_transfers == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 178, __pyx_L3_error)
-    __pyx_v_serial_force_release_away_from_readout = __Pyx_PyInt_As_int(values[36]); if (unlikely((__pyx_v_serial_force_release_away_from_readout == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 179, __pyx_L3_error)
-    __pyx_v_serial_use_integer_express_matrix = __Pyx_PyInt_As_int(values[37]); if (unlikely((__pyx_v_serial_use_integer_express_matrix == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 180, __pyx_L3_error)
-    __pyx_v_serial_n_pumps = __Pyx_PyInt_As_int(values[38]); if (unlikely((__pyx_v_serial_n_pumps == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 181, __pyx_L3_error)
-    __pyx_v_serial_roe_type = __Pyx_PyInt_As_int(values[39]); if (unlikely((__pyx_v_serial_roe_type == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 182, __pyx_L3_error)
+    __pyx_v_serial_prescan_offset = __Pyx_PyInt_As_int(values[32]); if (unlikely((__pyx_v_serial_prescan_offset == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 175, __pyx_L3_error)
+    __pyx_v_serial_overscan_start = __Pyx_PyInt_As_int(values[33]); if (unlikely((__pyx_v_serial_overscan_start == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 176, __pyx_L3_error)
+    __pyx_v_serial_empty_traps_between_columns = __Pyx_PyInt_As_int(values[34]); if (unlikely((__pyx_v_serial_empty_traps_between_columns == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 177, __pyx_L3_error)
+    __pyx_v_serial_empty_traps_for_first_transfers = __Pyx_PyInt_As_int(values[35]); if (unlikely((__pyx_v_serial_empty_traps_for_first_transfers == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 178, __pyx_L3_error)
+    __pyx_v_serial_force_release_away_from_readout = __Pyx_PyInt_As_int(values[36]); if (unlikely((__pyx_v_serial_force_release_away_from_readout == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 179, __pyx_L3_error)
+    __pyx_v_serial_use_integer_express_matrix = __Pyx_PyInt_As_int(values[37]); if (unlikely((__pyx_v_serial_use_integer_express_matrix == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 180, __pyx_L3_error)
+    __pyx_v_serial_n_pumps = __Pyx_PyInt_As_int(values[38]); if (unlikely((__pyx_v_serial_n_pumps == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 181, __pyx_L3_error)
+    __pyx_v_serial_roe_type = __Pyx_PyInt_As_int(values[39]); if (unlikely((__pyx_v_serial_roe_type == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 182, __pyx_L3_error)
     __pyx_v_serial_fraction_of_traps_per_phase = ((PyArrayObject *)values[40]);
     __pyx_v_serial_full_well_depths = ((PyArrayObject *)values[41]);
     __pyx_v_serial_well_notch_depths = ((PyArrayObject *)values[42]);
     __pyx_v_serial_well_fill_powers = ((PyArrayObject *)values[43]);
     __pyx_v_serial_first_electron_fills = ((PyArrayObject *)values[44]);
     __pyx_v_serial_trap_densities = ((PyArrayObject *)values[45]);
     __pyx_v_serial_trap_release_timescales = ((PyArrayObject *)values[46]);
     __pyx_v_serial_trap_third_params = ((PyArrayObject *)values[47]);
     __pyx_v_serial_trap_fourth_params = ((PyArrayObject *)values[48]);
-    __pyx_v_serial_n_traps_ic = __Pyx_PyInt_As_int(values[49]); if (unlikely((__pyx_v_serial_n_traps_ic == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 194, __pyx_L3_error)
-    __pyx_v_serial_n_traps_sc = __Pyx_PyInt_As_int(values[50]); if (unlikely((__pyx_v_serial_n_traps_sc == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 195, __pyx_L3_error)
-    __pyx_v_serial_n_traps_ic_co = __Pyx_PyInt_As_int(values[51]); if (unlikely((__pyx_v_serial_n_traps_ic_co == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 196, __pyx_L3_error)
-    __pyx_v_serial_n_traps_sc_co = __Pyx_PyInt_As_int(values[52]); if (unlikely((__pyx_v_serial_n_traps_sc_co == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_serial_express = __Pyx_PyInt_As_int(values[53]); if (unlikely((__pyx_v_serial_express == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 199, __pyx_L3_error)
-    __pyx_v_serial_window_offset = __Pyx_PyInt_As_int(values[54]); if (unlikely((__pyx_v_serial_window_offset == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 200, __pyx_L3_error)
-    __pyx_v_serial_window_start = __Pyx_PyInt_As_int(values[55]); if (unlikely((__pyx_v_serial_window_start == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
-    __pyx_v_serial_window_stop = __Pyx_PyInt_As_int(values[56]); if (unlikely((__pyx_v_serial_window_stop == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 202, __pyx_L3_error)
-    __pyx_v_serial_time_start = __Pyx_PyInt_As_int(values[57]); if (unlikely((__pyx_v_serial_time_start == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 203, __pyx_L3_error)
-    __pyx_v_serial_time_stop = __Pyx_PyInt_As_int(values[58]); if (unlikely((__pyx_v_serial_time_stop == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 204, __pyx_L3_error)
+    __pyx_v_serial_n_traps_ic = __Pyx_PyInt_As_int(values[49]); if (unlikely((__pyx_v_serial_n_traps_ic == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 194, __pyx_L3_error)
+    __pyx_v_serial_n_traps_sc = __Pyx_PyInt_As_int(values[50]); if (unlikely((__pyx_v_serial_n_traps_sc == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 195, __pyx_L3_error)
+    __pyx_v_serial_n_traps_ic_co = __Pyx_PyInt_As_int(values[51]); if (unlikely((__pyx_v_serial_n_traps_ic_co == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 196, __pyx_L3_error)
+    __pyx_v_serial_n_traps_sc_co = __Pyx_PyInt_As_int(values[52]); if (unlikely((__pyx_v_serial_n_traps_sc_co == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 197, __pyx_L3_error)
+    __pyx_v_serial_express = __Pyx_PyInt_As_int(values[53]); if (unlikely((__pyx_v_serial_express == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 199, __pyx_L3_error)
+    __pyx_v_serial_window_offset = __Pyx_PyInt_As_int(values[54]); if (unlikely((__pyx_v_serial_window_offset == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 200, __pyx_L3_error)
+    __pyx_v_serial_window_start = __Pyx_PyInt_As_int(values[55]); if (unlikely((__pyx_v_serial_window_start == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 201, __pyx_L3_error)
+    __pyx_v_serial_window_stop = __Pyx_PyInt_As_int(values[56]); if (unlikely((__pyx_v_serial_window_stop == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 202, __pyx_L3_error)
+    __pyx_v_serial_time_start = __Pyx_PyInt_As_int(values[57]); if (unlikely((__pyx_v_serial_time_start == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 203, __pyx_L3_error)
+    __pyx_v_serial_time_stop = __Pyx_PyInt_As_int(values[58]); if (unlikely((__pyx_v_serial_time_stop == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 204, __pyx_L3_error)
     __pyx_v_serial_prune_n_electrons = ((PyArrayObject *)values[59]);
-    __pyx_v_serial_prune_frequency = __Pyx_PyInt_As_int(values[60]); if (unlikely((__pyx_v_serial_prune_frequency == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 206, __pyx_L3_error)
-    __pyx_v_allow_negative_pixels = __Pyx_PyInt_As_int(values[61]); if (unlikely((__pyx_v_allow_negative_pixels == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 210, __pyx_L3_error)
-    __pyx_v_verbosity = __Pyx_PyInt_As_int(values[62]); if (unlikely((__pyx_v_verbosity == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 212, __pyx_L3_error)
-    __pyx_v_iteration = __Pyx_PyInt_As_int(values[63]); if (unlikely((__pyx_v_iteration == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 213, __pyx_L3_error)
+    __pyx_v_serial_prune_frequency = __Pyx_PyInt_As_int(values[60]); if (unlikely((__pyx_v_serial_prune_frequency == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 206, __pyx_L3_error)
+    __pyx_v_allow_negative_pixels = __Pyx_PyInt_As_int(values[61]); if (unlikely((__pyx_v_allow_negative_pixels == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 210, __pyx_L3_error)
+    __pyx_v_verbosity = __Pyx_PyInt_As_int(values[62]); if (unlikely((__pyx_v_verbosity == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 212, __pyx_L3_error)
+    __pyx_v_iteration = __Pyx_PyInt_As_int(values[63]); if (unlikely((__pyx_v_iteration == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 213, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 131, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("cy_add_cti", 1, 64, 64, __pyx_nargs); __PYX_ERR(2, 131, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("arcticpy.wrapper.cy_add_cti", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_image), __pyx_ptype_5numpy_ndarray, 1, "image", 0))) __PYX_ERR(0, 132, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_parallel_dwell_times), __pyx_ptype_5numpy_ndarray, 1, "parallel_dwell_times", 0))) __PYX_ERR(0, 137, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_parallel_fraction_of_traps_per_phase), __pyx_ptype_5numpy_ndarray, 1, "parallel_fraction_of_traps_per_phase", 0))) __PYX_ERR(0, 147, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_parallel_full_well_depths), __pyx_ptype_5numpy_ndarray, 1, "parallel_full_well_depths", 0))) __PYX_ERR(0, 148, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_parallel_well_notch_depths), __pyx_ptype_5numpy_ndarray, 1, "parallel_well_notch_depths", 0))) __PYX_ERR(0, 149, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_parallel_well_fill_powers), __pyx_ptype_5numpy_ndarray, 1, "parallel_well_fill_powers", 0))) __PYX_ERR(0, 150, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_parallel_first_electron_fills), __pyx_ptype_5numpy_ndarray, 1, "parallel_first_electron_fills", 0))) __PYX_ERR(0, 151, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_parallel_trap_densities), __pyx_ptype_5numpy_ndarray, 1, "parallel_trap_densities", 0))) __PYX_ERR(0, 153, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_parallel_trap_release_timescales), __pyx_ptype_5numpy_ndarray, 1, "parallel_trap_release_timescales", 0))) __PYX_ERR(0, 154, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_parallel_trap_third_params), __pyx_ptype_5numpy_ndarray, 1, "parallel_trap_third_params", 0))) __PYX_ERR(0, 155, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_parallel_trap_fourth_params), __pyx_ptype_5numpy_ndarray, 1, "parallel_trap_fourth_params", 0))) __PYX_ERR(0, 156, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_parallel_prune_n_electrons), __pyx_ptype_5numpy_ndarray, 1, "parallel_prune_n_electrons", 0))) __PYX_ERR(0, 168, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_serial_dwell_times), __pyx_ptype_5numpy_ndarray, 1, "serial_dwell_times", 0))) __PYX_ERR(0, 174, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_serial_fraction_of_traps_per_phase), __pyx_ptype_5numpy_ndarray, 1, "serial_fraction_of_traps_per_phase", 0))) __PYX_ERR(0, 184, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_serial_full_well_depths), __pyx_ptype_5numpy_ndarray, 1, "serial_full_well_depths", 0))) __PYX_ERR(0, 185, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_serial_well_notch_depths), __pyx_ptype_5numpy_ndarray, 1, "serial_well_notch_depths", 0))) __PYX_ERR(0, 186, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_serial_well_fill_powers), __pyx_ptype_5numpy_ndarray, 1, "serial_well_fill_powers", 0))) __PYX_ERR(0, 187, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_serial_first_electron_fills), __pyx_ptype_5numpy_ndarray, 1, "serial_first_electron_fills", 0))) __PYX_ERR(0, 188, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_serial_trap_densities), __pyx_ptype_5numpy_ndarray, 1, "serial_trap_densities", 0))) __PYX_ERR(0, 190, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_serial_trap_release_timescales), __pyx_ptype_5numpy_ndarray, 1, "serial_trap_release_timescales", 0))) __PYX_ERR(0, 191, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_serial_trap_third_params), __pyx_ptype_5numpy_ndarray, 1, "serial_trap_third_params", 0))) __PYX_ERR(0, 192, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_serial_trap_fourth_params), __pyx_ptype_5numpy_ndarray, 1, "serial_trap_fourth_params", 0))) __PYX_ERR(0, 193, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_serial_prune_n_electrons), __pyx_ptype_5numpy_ndarray, 1, "serial_prune_n_electrons", 0))) __PYX_ERR(0, 205, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_image), __pyx_ptype_5numpy_ndarray, 1, "image", 0))) __PYX_ERR(2, 132, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_parallel_dwell_times), __pyx_ptype_5numpy_ndarray, 1, "parallel_dwell_times", 0))) __PYX_ERR(2, 137, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_parallel_fraction_of_traps_per_phase), __pyx_ptype_5numpy_ndarray, 1, "parallel_fraction_of_traps_per_phase", 0))) __PYX_ERR(2, 147, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_parallel_full_well_depths), __pyx_ptype_5numpy_ndarray, 1, "parallel_full_well_depths", 0))) __PYX_ERR(2, 148, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_parallel_well_notch_depths), __pyx_ptype_5numpy_ndarray, 1, "parallel_well_notch_depths", 0))) __PYX_ERR(2, 149, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_parallel_well_fill_powers), __pyx_ptype_5numpy_ndarray, 1, "parallel_well_fill_powers", 0))) __PYX_ERR(2, 150, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_parallel_first_electron_fills), __pyx_ptype_5numpy_ndarray, 1, "parallel_first_electron_fills", 0))) __PYX_ERR(2, 151, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_parallel_trap_densities), __pyx_ptype_5numpy_ndarray, 1, "parallel_trap_densities", 0))) __PYX_ERR(2, 153, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_parallel_trap_release_timescales), __pyx_ptype_5numpy_ndarray, 1, "parallel_trap_release_timescales", 0))) __PYX_ERR(2, 154, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_parallel_trap_third_params), __pyx_ptype_5numpy_ndarray, 1, "parallel_trap_third_params", 0))) __PYX_ERR(2, 155, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_parallel_trap_fourth_params), __pyx_ptype_5numpy_ndarray, 1, "parallel_trap_fourth_params", 0))) __PYX_ERR(2, 156, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_parallel_prune_n_electrons), __pyx_ptype_5numpy_ndarray, 1, "parallel_prune_n_electrons", 0))) __PYX_ERR(2, 168, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_serial_dwell_times), __pyx_ptype_5numpy_ndarray, 1, "serial_dwell_times", 0))) __PYX_ERR(2, 174, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_serial_fraction_of_traps_per_phase), __pyx_ptype_5numpy_ndarray, 1, "serial_fraction_of_traps_per_phase", 0))) __PYX_ERR(2, 184, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_serial_full_well_depths), __pyx_ptype_5numpy_ndarray, 1, "serial_full_well_depths", 0))) __PYX_ERR(2, 185, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_serial_well_notch_depths), __pyx_ptype_5numpy_ndarray, 1, "serial_well_notch_depths", 0))) __PYX_ERR(2, 186, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_serial_well_fill_powers), __pyx_ptype_5numpy_ndarray, 1, "serial_well_fill_powers", 0))) __PYX_ERR(2, 187, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_serial_first_electron_fills), __pyx_ptype_5numpy_ndarray, 1, "serial_first_electron_fills", 0))) __PYX_ERR(2, 188, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_serial_trap_densities), __pyx_ptype_5numpy_ndarray, 1, "serial_trap_densities", 0))) __PYX_ERR(2, 190, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_serial_trap_release_timescales), __pyx_ptype_5numpy_ndarray, 1, "serial_trap_release_timescales", 0))) __PYX_ERR(2, 191, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_serial_trap_third_params), __pyx_ptype_5numpy_ndarray, 1, "serial_trap_third_params", 0))) __PYX_ERR(2, 192, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_serial_trap_fourth_params), __pyx_ptype_5numpy_ndarray, 1, "serial_trap_fourth_params", 0))) __PYX_ERR(2, 193, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_serial_prune_n_electrons), __pyx_ptype_5numpy_ndarray, 1, "serial_prune_n_electrons", 0))) __PYX_ERR(2, 205, __pyx_L1_error)
   __pyx_r = __pyx_pf_8arcticpy_7wrapper_10cy_add_cti(__pyx_self, __pyx_v_image, __pyx_v_parallel_dwell_times, __pyx_v_parallel_prescan_offset, __pyx_v_parallel_overscan_start, __pyx_v_parallel_empty_traps_between_columns, __pyx_v_parallel_empty_traps_for_first_transfers, __pyx_v_parallel_force_release_away_from_readout, __pyx_v_parallel_use_integer_express_matrix, __pyx_v_parallel_n_pumps, __pyx_v_parallel_roe_type, __pyx_v_parallel_fraction_of_traps_per_phase, __pyx_v_parallel_full_well_depths, __pyx_v_parallel_well_notch_depths, __pyx_v_parallel_well_fill_powers, __pyx_v_parallel_first_electron_fills, __pyx_v_parallel_trap_densities, __pyx_v_parallel_trap_release_timescales, __pyx_v_parallel_trap_third_params, __pyx_v_parallel_trap_fourth_params, __pyx_v_parallel_n_traps_ic, __pyx_v_parallel_n_traps_sc, __pyx_v_parallel_n_traps_ic_co, __pyx_v_parallel_n_traps_sc_co, __pyx_v_parallel_express, __pyx_v_parallel_window_offset, __pyx_v_parallel_window_start, __pyx_v_parallel_window_stop, __pyx_v_parallel_time_start, __pyx_v_parallel_time_stop, __pyx_v_parallel_prune_n_electrons, __pyx_v_parallel_prune_frequency, __pyx_v_serial_dwell_times, __pyx_v_serial_prescan_offset, __pyx_v_serial_overscan_start, __pyx_v_serial_empty_traps_between_columns, __pyx_v_serial_empty_traps_for_first_transfers, __pyx_v_serial_force_release_away_from_readout, __pyx_v_serial_use_integer_express_matrix, __pyx_v_serial_n_pumps, __pyx_v_serial_roe_type, __pyx_v_serial_fraction_of_traps_per_phase, __pyx_v_serial_full_well_depths, __pyx_v_serial_well_notch_depths, __pyx_v_serial_well_fill_powers, __pyx_v_serial_first_electron_fills, __pyx_v_serial_trap_densities, __pyx_v_serial_trap_release_timescales, __pyx_v_serial_trap_third_params, __pyx_v_serial_trap_fourth_params, __pyx_v_serial_n_traps_ic, __pyx_v_serial_n_traps_sc, __pyx_v_serial_n_traps_ic_co, __pyx_v_serial_n_traps_sc_co, __pyx_v_serial_express, __pyx_v_serial_window_offset, __pyx_v_serial_window_start, __pyx_v_serial_window_stop, __pyx_v_serial_time_start, __pyx_v_serial_time_stop, __pyx_v_serial_prune_n_electrons, __pyx_v_serial_prune_frequency, __pyx_v_allow_negative_pixels, __pyx_v_verbosity, __pyx_v_iteration);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -3526,23 +6454,23 @@
   __Pyx_LocalBuf_ND __pyx_pybuffernd_serial_well_notch_depths;
   __Pyx_Buffer __pyx_pybuffer_serial_well_notch_depths;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
-  PyArrayObject *__pyx_t_4 = NULL;
-  int __pyx_t_5;
+  int __pyx_t_4;
+  PyArrayObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   Py_ssize_t __pyx_t_9;
   Py_ssize_t __pyx_t_10;
-  Py_ssize_t __pyx_t_11;
-  Py_ssize_t __pyx_t_12;
+  npy_intp *__pyx_t_11;
+  npy_intp *__pyx_t_12;
   Py_ssize_t __pyx_t_13;
   Py_ssize_t __pyx_t_14;
   Py_ssize_t __pyx_t_15;
   Py_ssize_t __pyx_t_16;
   Py_ssize_t __pyx_t_17;
   Py_ssize_t __pyx_t_18;
   Py_ssize_t __pyx_t_19;
@@ -3559,14 +6487,16 @@
   Py_ssize_t __pyx_t_30;
   Py_ssize_t __pyx_t_31;
   Py_ssize_t __pyx_t_32;
   Py_ssize_t __pyx_t_33;
   Py_ssize_t __pyx_t_34;
   Py_ssize_t __pyx_t_35;
   Py_ssize_t __pyx_t_36;
+  Py_ssize_t __pyx_t_37;
+  Py_ssize_t __pyx_t_38;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("cy_add_cti", 0);
   __Pyx_INCREF((PyObject *)__pyx_v_image);
   __pyx_pybuffer_image.pybuffer.buf = NULL;
   __pyx_pybuffer_image.refcount = 0;
@@ -3658,646 +6588,669 @@
   __pyx_pybuffernd_serial_trap_fourth_params.rcbuffer = &__pyx_pybuffer_serial_trap_fourth_params;
   __pyx_pybuffer_serial_prune_n_electrons.pybuffer.buf = NULL;
   __pyx_pybuffer_serial_prune_n_electrons.refcount = 0;
   __pyx_pybuffernd_serial_prune_n_electrons.data = NULL;
   __pyx_pybuffernd_serial_prune_n_electrons.rcbuffer = &__pyx_pybuffer_serial_prune_n_electrons;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_image.rcbuffer->pybuffer, (PyObject*)__pyx_v_image, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) __PYX_ERR(0, 131, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_image.rcbuffer->pybuffer, (PyObject*)__pyx_v_image, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) __PYX_ERR(2, 131, __pyx_L1_error)
   }
   __pyx_pybuffernd_image.diminfo[0].strides = __pyx_pybuffernd_image.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_image.diminfo[0].shape = __pyx_pybuffernd_image.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_image.diminfo[1].strides = __pyx_pybuffernd_image.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_image.diminfo[1].shape = __pyx_pybuffernd_image.rcbuffer->pybuffer.shape[1];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_parallel_dwell_times.rcbuffer->pybuffer, (PyObject*)__pyx_v_parallel_dwell_times, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 131, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_parallel_dwell_times.rcbuffer->pybuffer, (PyObject*)__pyx_v_parallel_dwell_times, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(2, 131, __pyx_L1_error)
   }
   __pyx_pybuffernd_parallel_dwell_times.diminfo[0].strides = __pyx_pybuffernd_parallel_dwell_times.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_parallel_dwell_times.diminfo[0].shape = __pyx_pybuffernd_parallel_dwell_times.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_parallel_fraction_of_traps_per_phase.rcbuffer->pybuffer, (PyObject*)__pyx_v_parallel_fraction_of_traps_per_phase, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 131, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_parallel_fraction_of_traps_per_phase.rcbuffer->pybuffer, (PyObject*)__pyx_v_parallel_fraction_of_traps_per_phase, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(2, 131, __pyx_L1_error)
   }
   __pyx_pybuffernd_parallel_fraction_of_traps_per_phase.diminfo[0].strides = __pyx_pybuffernd_parallel_fraction_of_traps_per_phase.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_parallel_fraction_of_traps_per_phase.diminfo[0].shape = __pyx_pybuffernd_parallel_fraction_of_traps_per_phase.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_parallel_full_well_depths.rcbuffer->pybuffer, (PyObject*)__pyx_v_parallel_full_well_depths, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 131, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_parallel_full_well_depths.rcbuffer->pybuffer, (PyObject*)__pyx_v_parallel_full_well_depths, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(2, 131, __pyx_L1_error)
   }
   __pyx_pybuffernd_parallel_full_well_depths.diminfo[0].strides = __pyx_pybuffernd_parallel_full_well_depths.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_parallel_full_well_depths.diminfo[0].shape = __pyx_pybuffernd_parallel_full_well_depths.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_parallel_well_notch_depths.rcbuffer->pybuffer, (PyObject*)__pyx_v_parallel_well_notch_depths, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 131, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_parallel_well_notch_depths.rcbuffer->pybuffer, (PyObject*)__pyx_v_parallel_well_notch_depths, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(2, 131, __pyx_L1_error)
   }
   __pyx_pybuffernd_parallel_well_notch_depths.diminfo[0].strides = __pyx_pybuffernd_parallel_well_notch_depths.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_parallel_well_notch_depths.diminfo[0].shape = __pyx_pybuffernd_parallel_well_notch_depths.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_parallel_well_fill_powers.rcbuffer->pybuffer, (PyObject*)__pyx_v_parallel_well_fill_powers, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 131, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_parallel_well_fill_powers.rcbuffer->pybuffer, (PyObject*)__pyx_v_parallel_well_fill_powers, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(2, 131, __pyx_L1_error)
   }
   __pyx_pybuffernd_parallel_well_fill_powers.diminfo[0].strides = __pyx_pybuffernd_parallel_well_fill_powers.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_parallel_well_fill_powers.diminfo[0].shape = __pyx_pybuffernd_parallel_well_fill_powers.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_parallel_first_electron_fills.rcbuffer->pybuffer, (PyObject*)__pyx_v_parallel_first_electron_fills, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 131, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_parallel_first_electron_fills.rcbuffer->pybuffer, (PyObject*)__pyx_v_parallel_first_electron_fills, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(2, 131, __pyx_L1_error)
   }
   __pyx_pybuffernd_parallel_first_electron_fills.diminfo[0].strides = __pyx_pybuffernd_parallel_first_electron_fills.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_parallel_first_electron_fills.diminfo[0].shape = __pyx_pybuffernd_parallel_first_electron_fills.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_parallel_trap_densities.rcbuffer->pybuffer, (PyObject*)__pyx_v_parallel_trap_densities, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 131, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_parallel_trap_densities.rcbuffer->pybuffer, (PyObject*)__pyx_v_parallel_trap_densities, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(2, 131, __pyx_L1_error)
   }
   __pyx_pybuffernd_parallel_trap_densities.diminfo[0].strides = __pyx_pybuffernd_parallel_trap_densities.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_parallel_trap_densities.diminfo[0].shape = __pyx_pybuffernd_parallel_trap_densities.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_parallel_trap_release_timescales.rcbuffer->pybuffer, (PyObject*)__pyx_v_parallel_trap_release_timescales, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 131, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_parallel_trap_release_timescales.rcbuffer->pybuffer, (PyObject*)__pyx_v_parallel_trap_release_timescales, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(2, 131, __pyx_L1_error)
   }
   __pyx_pybuffernd_parallel_trap_release_timescales.diminfo[0].strides = __pyx_pybuffernd_parallel_trap_release_timescales.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_parallel_trap_release_timescales.diminfo[0].shape = __pyx_pybuffernd_parallel_trap_release_timescales.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_parallel_trap_third_params.rcbuffer->pybuffer, (PyObject*)__pyx_v_parallel_trap_third_params, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 131, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_parallel_trap_third_params.rcbuffer->pybuffer, (PyObject*)__pyx_v_parallel_trap_third_params, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(2, 131, __pyx_L1_error)
   }
   __pyx_pybuffernd_parallel_trap_third_params.diminfo[0].strides = __pyx_pybuffernd_parallel_trap_third_params.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_parallel_trap_third_params.diminfo[0].shape = __pyx_pybuffernd_parallel_trap_third_params.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_parallel_trap_fourth_params.rcbuffer->pybuffer, (PyObject*)__pyx_v_parallel_trap_fourth_params, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 131, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_parallel_trap_fourth_params.rcbuffer->pybuffer, (PyObject*)__pyx_v_parallel_trap_fourth_params, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(2, 131, __pyx_L1_error)
   }
   __pyx_pybuffernd_parallel_trap_fourth_params.diminfo[0].strides = __pyx_pybuffernd_parallel_trap_fourth_params.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_parallel_trap_fourth_params.diminfo[0].shape = __pyx_pybuffernd_parallel_trap_fourth_params.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_parallel_prune_n_electrons.rcbuffer->pybuffer, (PyObject*)__pyx_v_parallel_prune_n_electrons, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 131, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_parallel_prune_n_electrons.rcbuffer->pybuffer, (PyObject*)__pyx_v_parallel_prune_n_electrons, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(2, 131, __pyx_L1_error)
   }
   __pyx_pybuffernd_parallel_prune_n_electrons.diminfo[0].strides = __pyx_pybuffernd_parallel_prune_n_electrons.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_parallel_prune_n_electrons.diminfo[0].shape = __pyx_pybuffernd_parallel_prune_n_electrons.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_serial_dwell_times.rcbuffer->pybuffer, (PyObject*)__pyx_v_serial_dwell_times, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 131, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_serial_dwell_times.rcbuffer->pybuffer, (PyObject*)__pyx_v_serial_dwell_times, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(2, 131, __pyx_L1_error)
   }
   __pyx_pybuffernd_serial_dwell_times.diminfo[0].strides = __pyx_pybuffernd_serial_dwell_times.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_serial_dwell_times.diminfo[0].shape = __pyx_pybuffernd_serial_dwell_times.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_serial_fraction_of_traps_per_phase.rcbuffer->pybuffer, (PyObject*)__pyx_v_serial_fraction_of_traps_per_phase, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 131, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_serial_fraction_of_traps_per_phase.rcbuffer->pybuffer, (PyObject*)__pyx_v_serial_fraction_of_traps_per_phase, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(2, 131, __pyx_L1_error)
   }
   __pyx_pybuffernd_serial_fraction_of_traps_per_phase.diminfo[0].strides = __pyx_pybuffernd_serial_fraction_of_traps_per_phase.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_serial_fraction_of_traps_per_phase.diminfo[0].shape = __pyx_pybuffernd_serial_fraction_of_traps_per_phase.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_serial_full_well_depths.rcbuffer->pybuffer, (PyObject*)__pyx_v_serial_full_well_depths, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 131, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_serial_full_well_depths.rcbuffer->pybuffer, (PyObject*)__pyx_v_serial_full_well_depths, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(2, 131, __pyx_L1_error)
   }
   __pyx_pybuffernd_serial_full_well_depths.diminfo[0].strides = __pyx_pybuffernd_serial_full_well_depths.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_serial_full_well_depths.diminfo[0].shape = __pyx_pybuffernd_serial_full_well_depths.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_serial_well_notch_depths.rcbuffer->pybuffer, (PyObject*)__pyx_v_serial_well_notch_depths, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 131, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_serial_well_notch_depths.rcbuffer->pybuffer, (PyObject*)__pyx_v_serial_well_notch_depths, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(2, 131, __pyx_L1_error)
   }
   __pyx_pybuffernd_serial_well_notch_depths.diminfo[0].strides = __pyx_pybuffernd_serial_well_notch_depths.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_serial_well_notch_depths.diminfo[0].shape = __pyx_pybuffernd_serial_well_notch_depths.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_serial_well_fill_powers.rcbuffer->pybuffer, (PyObject*)__pyx_v_serial_well_fill_powers, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 131, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_serial_well_fill_powers.rcbuffer->pybuffer, (PyObject*)__pyx_v_serial_well_fill_powers, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(2, 131, __pyx_L1_error)
   }
   __pyx_pybuffernd_serial_well_fill_powers.diminfo[0].strides = __pyx_pybuffernd_serial_well_fill_powers.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_serial_well_fill_powers.diminfo[0].shape = __pyx_pybuffernd_serial_well_fill_powers.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_serial_first_electron_fills.rcbuffer->pybuffer, (PyObject*)__pyx_v_serial_first_electron_fills, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 131, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_serial_first_electron_fills.rcbuffer->pybuffer, (PyObject*)__pyx_v_serial_first_electron_fills, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(2, 131, __pyx_L1_error)
   }
   __pyx_pybuffernd_serial_first_electron_fills.diminfo[0].strides = __pyx_pybuffernd_serial_first_electron_fills.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_serial_first_electron_fills.diminfo[0].shape = __pyx_pybuffernd_serial_first_electron_fills.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_serial_trap_densities.rcbuffer->pybuffer, (PyObject*)__pyx_v_serial_trap_densities, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 131, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_serial_trap_densities.rcbuffer->pybuffer, (PyObject*)__pyx_v_serial_trap_densities, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(2, 131, __pyx_L1_error)
   }
   __pyx_pybuffernd_serial_trap_densities.diminfo[0].strides = __pyx_pybuffernd_serial_trap_densities.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_serial_trap_densities.diminfo[0].shape = __pyx_pybuffernd_serial_trap_densities.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_serial_trap_release_timescales.rcbuffer->pybuffer, (PyObject*)__pyx_v_serial_trap_release_timescales, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 131, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_serial_trap_release_timescales.rcbuffer->pybuffer, (PyObject*)__pyx_v_serial_trap_release_timescales, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(2, 131, __pyx_L1_error)
   }
   __pyx_pybuffernd_serial_trap_release_timescales.diminfo[0].strides = __pyx_pybuffernd_serial_trap_release_timescales.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_serial_trap_release_timescales.diminfo[0].shape = __pyx_pybuffernd_serial_trap_release_timescales.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_serial_trap_third_params.rcbuffer->pybuffer, (PyObject*)__pyx_v_serial_trap_third_params, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 131, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_serial_trap_third_params.rcbuffer->pybuffer, (PyObject*)__pyx_v_serial_trap_third_params, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(2, 131, __pyx_L1_error)
   }
   __pyx_pybuffernd_serial_trap_third_params.diminfo[0].strides = __pyx_pybuffernd_serial_trap_third_params.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_serial_trap_third_params.diminfo[0].shape = __pyx_pybuffernd_serial_trap_third_params.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_serial_trap_fourth_params.rcbuffer->pybuffer, (PyObject*)__pyx_v_serial_trap_fourth_params, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 131, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_serial_trap_fourth_params.rcbuffer->pybuffer, (PyObject*)__pyx_v_serial_trap_fourth_params, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(2, 131, __pyx_L1_error)
   }
   __pyx_pybuffernd_serial_trap_fourth_params.diminfo[0].strides = __pyx_pybuffernd_serial_trap_fourth_params.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_serial_trap_fourth_params.diminfo[0].shape = __pyx_pybuffernd_serial_trap_fourth_params.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_serial_prune_n_electrons.rcbuffer->pybuffer, (PyObject*)__pyx_v_serial_prune_n_electrons, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 131, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_serial_prune_n_electrons.rcbuffer->pybuffer, (PyObject*)__pyx_v_serial_prune_n_electrons, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(2, 131, __pyx_L1_error)
   }
   __pyx_pybuffernd_serial_prune_n_electrons.diminfo[0].strides = __pyx_pybuffernd_serial_prune_n_electrons.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_serial_prune_n_electrons.diminfo[0].shape = __pyx_pybuffernd_serial_prune_n_electrons.rcbuffer->pybuffer.shape[0];
 
   /* "arcticpy/wrapper.pyx":222
  *     in interface.cpp.
  *     """
  *     image = check_contiguous(image)             # <<<<<<<<<<<<<<
  * 
  *     add_cti(
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_check_contiguous); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 222, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_check_contiguous); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 222, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
+  __pyx_t_4 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
+      __pyx_t_4 = 1;
     }
   }
-  __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, ((PyObject *)__pyx_v_image)) : __Pyx_PyObject_CallOneArg(__pyx_t_2, ((PyObject *)__pyx_v_image));
-  __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 222, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 222, __pyx_L1_error)
-  __pyx_t_4 = ((PyArrayObject *)__pyx_t_1);
+  {
+    PyObject *__pyx_callargs[2] = {__pyx_t_3, ((PyObject *)__pyx_v_image)};
+    __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 222, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  }
+  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(2, 222, __pyx_L1_error)
+  __pyx_t_5 = ((PyArrayObject *)__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_image.rcbuffer->pybuffer);
-    __pyx_t_5 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_image.rcbuffer->pybuffer, (PyObject*)__pyx_t_4, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack);
-    if (unlikely(__pyx_t_5 < 0)) {
+    __pyx_t_4 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_image.rcbuffer->pybuffer, (PyObject*)__pyx_t_5, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack);
+    if (unlikely(__pyx_t_4 < 0)) {
       PyErr_Fetch(&__pyx_t_6, &__pyx_t_7, &__pyx_t_8);
       if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_image.rcbuffer->pybuffer, (PyObject*)__pyx_v_image, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) {
         Py_XDECREF(__pyx_t_6); Py_XDECREF(__pyx_t_7); Py_XDECREF(__pyx_t_8);
         __Pyx_RaiseBufferFallbackError();
       } else {
         PyErr_Restore(__pyx_t_6, __pyx_t_7, __pyx_t_8);
       }
       __pyx_t_6 = __pyx_t_7 = __pyx_t_8 = 0;
     }
     __pyx_pybuffernd_image.diminfo[0].strides = __pyx_pybuffernd_image.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_image.diminfo[0].shape = __pyx_pybuffernd_image.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_image.diminfo[1].strides = __pyx_pybuffernd_image.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_image.diminfo[1].shape = __pyx_pybuffernd_image.rcbuffer->pybuffer.shape[1];
-    if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 222, __pyx_L1_error)
+    if (unlikely((__pyx_t_4 < 0))) __PYX_ERR(2, 222, __pyx_L1_error)
   }
-  __pyx_t_4 = 0;
+  __pyx_t_5 = 0;
   __Pyx_DECREF_SET(__pyx_v_image, ((PyArrayObject *)__pyx_t_1));
   __pyx_t_1 = 0;
 
   /* "arcticpy/wrapper.pyx":225
  * 
  *     add_cti(
  *         &image[0, 0],             # <<<<<<<<<<<<<<
  *         image.shape[0],
  *         image.shape[1],
  */
   __pyx_t_9 = 0;
   __pyx_t_10 = 0;
-  __pyx_t_5 = -1;
+  __pyx_t_4 = -1;
   if (__pyx_t_9 < 0) {
     __pyx_t_9 += __pyx_pybuffernd_image.diminfo[0].shape;
-    if (unlikely(__pyx_t_9 < 0)) __pyx_t_5 = 0;
-  } else if (unlikely(__pyx_t_9 >= __pyx_pybuffernd_image.diminfo[0].shape)) __pyx_t_5 = 0;
+    if (unlikely(__pyx_t_9 < 0)) __pyx_t_4 = 0;
+  } else if (unlikely(__pyx_t_9 >= __pyx_pybuffernd_image.diminfo[0].shape)) __pyx_t_4 = 0;
   if (__pyx_t_10 < 0) {
     __pyx_t_10 += __pyx_pybuffernd_image.diminfo[1].shape;
-    if (unlikely(__pyx_t_10 < 0)) __pyx_t_5 = 1;
-  } else if (unlikely(__pyx_t_10 >= __pyx_pybuffernd_image.diminfo[1].shape)) __pyx_t_5 = 1;
-  if (unlikely(__pyx_t_5 != -1)) {
-    __Pyx_RaiseBufferIndexError(__pyx_t_5);
-    __PYX_ERR(0, 225, __pyx_L1_error)
+    if (unlikely(__pyx_t_10 < 0)) __pyx_t_4 = 1;
+  } else if (unlikely(__pyx_t_10 >= __pyx_pybuffernd_image.diminfo[1].shape)) __pyx_t_4 = 1;
+  if (unlikely(__pyx_t_4 != -1)) {
+    __Pyx_RaiseBufferIndexError(__pyx_t_4);
+    __PYX_ERR(2, 225, __pyx_L1_error)
   }
 
+  /* "arcticpy/wrapper.pyx":226
+ *     add_cti(
+ *         &image[0, 0],
+ *         image.shape[0],             # <<<<<<<<<<<<<<
+ *         image.shape[1],
+ *         # ========
+ */
+  __pyx_t_11 = __pyx_f_5numpy_7ndarray_5shape_shape(((PyArrayObject *)__pyx_v_image)); if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 226, __pyx_L1_error)
+
+  /* "arcticpy/wrapper.pyx":227
+ *         &image[0, 0],
+ *         image.shape[0],
+ *         image.shape[1],             # <<<<<<<<<<<<<<
+ *         # ========
+ *         # Parallel
+ */
+  __pyx_t_12 = __pyx_f_5numpy_7ndarray_5shape_shape(((PyArrayObject *)__pyx_v_image)); if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 227, __pyx_L1_error)
+
   /* "arcticpy/wrapper.pyx":232
  *         # ========
  *         # ROE
  *         &parallel_dwell_times[0],             # <<<<<<<<<<<<<<
  *         len(parallel_dwell_times),
  *         parallel_prescan_offset,
  */
-  __pyx_t_11 = 0;
-  __pyx_t_5 = -1;
-  if (__pyx_t_11 < 0) {
-    __pyx_t_11 += __pyx_pybuffernd_parallel_dwell_times.diminfo[0].shape;
-    if (unlikely(__pyx_t_11 < 0)) __pyx_t_5 = 0;
-  } else if (unlikely(__pyx_t_11 >= __pyx_pybuffernd_parallel_dwell_times.diminfo[0].shape)) __pyx_t_5 = 0;
-  if (unlikely(__pyx_t_5 != -1)) {
-    __Pyx_RaiseBufferIndexError(__pyx_t_5);
-    __PYX_ERR(0, 232, __pyx_L1_error)
+  __pyx_t_13 = 0;
+  __pyx_t_4 = -1;
+  if (__pyx_t_13 < 0) {
+    __pyx_t_13 += __pyx_pybuffernd_parallel_dwell_times.diminfo[0].shape;
+    if (unlikely(__pyx_t_13 < 0)) __pyx_t_4 = 0;
+  } else if (unlikely(__pyx_t_13 >= __pyx_pybuffernd_parallel_dwell_times.diminfo[0].shape)) __pyx_t_4 = 0;
+  if (unlikely(__pyx_t_4 != -1)) {
+    __Pyx_RaiseBufferIndexError(__pyx_t_4);
+    __PYX_ERR(2, 232, __pyx_L1_error)
   }
 
   /* "arcticpy/wrapper.pyx":233
  *         # ROE
  *         &parallel_dwell_times[0],
  *         len(parallel_dwell_times),             # <<<<<<<<<<<<<<
  *         parallel_prescan_offset,
  *         parallel_overscan_start,
  */
-  __pyx_t_12 = PyObject_Length(((PyObject *)__pyx_v_parallel_dwell_times)); if (unlikely(__pyx_t_12 == ((Py_ssize_t)-1))) __PYX_ERR(0, 233, __pyx_L1_error)
+  __pyx_t_14 = PyObject_Length(((PyObject *)__pyx_v_parallel_dwell_times)); if (unlikely(__pyx_t_14 == ((Py_ssize_t)-1))) __PYX_ERR(2, 233, __pyx_L1_error)
 
   /* "arcticpy/wrapper.pyx":243
  *         parallel_roe_type,
  *         # CCD
  *         &parallel_fraction_of_traps_per_phase[0],             # <<<<<<<<<<<<<<
  *         len(parallel_fraction_of_traps_per_phase),
  *         &parallel_full_well_depths[0],
  */
-  __pyx_t_13 = 0;
-  __pyx_t_5 = -1;
-  if (__pyx_t_13 < 0) {
-    __pyx_t_13 += __pyx_pybuffernd_parallel_fraction_of_traps_per_phase.diminfo[0].shape;
-    if (unlikely(__pyx_t_13 < 0)) __pyx_t_5 = 0;
-  } else if (unlikely(__pyx_t_13 >= __pyx_pybuffernd_parallel_fraction_of_traps_per_phase.diminfo[0].shape)) __pyx_t_5 = 0;
-  if (unlikely(__pyx_t_5 != -1)) {
-    __Pyx_RaiseBufferIndexError(__pyx_t_5);
-    __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_15 = 0;
+  __pyx_t_4 = -1;
+  if (__pyx_t_15 < 0) {
+    __pyx_t_15 += __pyx_pybuffernd_parallel_fraction_of_traps_per_phase.diminfo[0].shape;
+    if (unlikely(__pyx_t_15 < 0)) __pyx_t_4 = 0;
+  } else if (unlikely(__pyx_t_15 >= __pyx_pybuffernd_parallel_fraction_of_traps_per_phase.diminfo[0].shape)) __pyx_t_4 = 0;
+  if (unlikely(__pyx_t_4 != -1)) {
+    __Pyx_RaiseBufferIndexError(__pyx_t_4);
+    __PYX_ERR(2, 243, __pyx_L1_error)
   }
 
   /* "arcticpy/wrapper.pyx":244
  *         # CCD
  *         &parallel_fraction_of_traps_per_phase[0],
  *         len(parallel_fraction_of_traps_per_phase),             # <<<<<<<<<<<<<<
  *         &parallel_full_well_depths[0],
  *         &parallel_well_notch_depths[0],
  */
-  __pyx_t_14 = PyObject_Length(((PyObject *)__pyx_v_parallel_fraction_of_traps_per_phase)); if (unlikely(__pyx_t_14 == ((Py_ssize_t)-1))) __PYX_ERR(0, 244, __pyx_L1_error)
+  __pyx_t_16 = PyObject_Length(((PyObject *)__pyx_v_parallel_fraction_of_traps_per_phase)); if (unlikely(__pyx_t_16 == ((Py_ssize_t)-1))) __PYX_ERR(2, 244, __pyx_L1_error)
 
   /* "arcticpy/wrapper.pyx":245
  *         &parallel_fraction_of_traps_per_phase[0],
  *         len(parallel_fraction_of_traps_per_phase),
  *         &parallel_full_well_depths[0],             # <<<<<<<<<<<<<<
  *         &parallel_well_notch_depths[0],
  *         &parallel_well_fill_powers[0],
  */
-  __pyx_t_15 = 0;
-  __pyx_t_5 = -1;
-  if (__pyx_t_15 < 0) {
-    __pyx_t_15 += __pyx_pybuffernd_parallel_full_well_depths.diminfo[0].shape;
-    if (unlikely(__pyx_t_15 < 0)) __pyx_t_5 = 0;
-  } else if (unlikely(__pyx_t_15 >= __pyx_pybuffernd_parallel_full_well_depths.diminfo[0].shape)) __pyx_t_5 = 0;
-  if (unlikely(__pyx_t_5 != -1)) {
-    __Pyx_RaiseBufferIndexError(__pyx_t_5);
-    __PYX_ERR(0, 245, __pyx_L1_error)
+  __pyx_t_17 = 0;
+  __pyx_t_4 = -1;
+  if (__pyx_t_17 < 0) {
+    __pyx_t_17 += __pyx_pybuffernd_parallel_full_well_depths.diminfo[0].shape;
+    if (unlikely(__pyx_t_17 < 0)) __pyx_t_4 = 0;
+  } else if (unlikely(__pyx_t_17 >= __pyx_pybuffernd_parallel_full_well_depths.diminfo[0].shape)) __pyx_t_4 = 0;
+  if (unlikely(__pyx_t_4 != -1)) {
+    __Pyx_RaiseBufferIndexError(__pyx_t_4);
+    __PYX_ERR(2, 245, __pyx_L1_error)
   }
 
   /* "arcticpy/wrapper.pyx":246
  *         len(parallel_fraction_of_traps_per_phase),
  *         &parallel_full_well_depths[0],
  *         &parallel_well_notch_depths[0],             # <<<<<<<<<<<<<<
  *         &parallel_well_fill_powers[0],
  *         &parallel_first_electron_fills[0],
  */
-  __pyx_t_16 = 0;
-  __pyx_t_5 = -1;
-  if (__pyx_t_16 < 0) {
-    __pyx_t_16 += __pyx_pybuffernd_parallel_well_notch_depths.diminfo[0].shape;
-    if (unlikely(__pyx_t_16 < 0)) __pyx_t_5 = 0;
-  } else if (unlikely(__pyx_t_16 >= __pyx_pybuffernd_parallel_well_notch_depths.diminfo[0].shape)) __pyx_t_5 = 0;
-  if (unlikely(__pyx_t_5 != -1)) {
-    __Pyx_RaiseBufferIndexError(__pyx_t_5);
-    __PYX_ERR(0, 246, __pyx_L1_error)
+  __pyx_t_18 = 0;
+  __pyx_t_4 = -1;
+  if (__pyx_t_18 < 0) {
+    __pyx_t_18 += __pyx_pybuffernd_parallel_well_notch_depths.diminfo[0].shape;
+    if (unlikely(__pyx_t_18 < 0)) __pyx_t_4 = 0;
+  } else if (unlikely(__pyx_t_18 >= __pyx_pybuffernd_parallel_well_notch_depths.diminfo[0].shape)) __pyx_t_4 = 0;
+  if (unlikely(__pyx_t_4 != -1)) {
+    __Pyx_RaiseBufferIndexError(__pyx_t_4);
+    __PYX_ERR(2, 246, __pyx_L1_error)
   }
 
   /* "arcticpy/wrapper.pyx":247
  *         &parallel_full_well_depths[0],
  *         &parallel_well_notch_depths[0],
  *         &parallel_well_fill_powers[0],             # <<<<<<<<<<<<<<
  *         &parallel_first_electron_fills[0],
  *         # Traps
  */
-  __pyx_t_17 = 0;
-  __pyx_t_5 = -1;
-  if (__pyx_t_17 < 0) {
-    __pyx_t_17 += __pyx_pybuffernd_parallel_well_fill_powers.diminfo[0].shape;
-    if (unlikely(__pyx_t_17 < 0)) __pyx_t_5 = 0;
-  } else if (unlikely(__pyx_t_17 >= __pyx_pybuffernd_parallel_well_fill_powers.diminfo[0].shape)) __pyx_t_5 = 0;
-  if (unlikely(__pyx_t_5 != -1)) {
-    __Pyx_RaiseBufferIndexError(__pyx_t_5);
-    __PYX_ERR(0, 247, __pyx_L1_error)
+  __pyx_t_19 = 0;
+  __pyx_t_4 = -1;
+  if (__pyx_t_19 < 0) {
+    __pyx_t_19 += __pyx_pybuffernd_parallel_well_fill_powers.diminfo[0].shape;
+    if (unlikely(__pyx_t_19 < 0)) __pyx_t_4 = 0;
+  } else if (unlikely(__pyx_t_19 >= __pyx_pybuffernd_parallel_well_fill_powers.diminfo[0].shape)) __pyx_t_4 = 0;
+  if (unlikely(__pyx_t_4 != -1)) {
+    __Pyx_RaiseBufferIndexError(__pyx_t_4);
+    __PYX_ERR(2, 247, __pyx_L1_error)
   }
 
   /* "arcticpy/wrapper.pyx":248
  *         &parallel_well_notch_depths[0],
  *         &parallel_well_fill_powers[0],
  *         &parallel_first_electron_fills[0],             # <<<<<<<<<<<<<<
  *         # Traps
  *         &parallel_trap_densities[0],
  */
-  __pyx_t_18 = 0;
-  __pyx_t_5 = -1;
-  if (__pyx_t_18 < 0) {
-    __pyx_t_18 += __pyx_pybuffernd_parallel_first_electron_fills.diminfo[0].shape;
-    if (unlikely(__pyx_t_18 < 0)) __pyx_t_5 = 0;
-  } else if (unlikely(__pyx_t_18 >= __pyx_pybuffernd_parallel_first_electron_fills.diminfo[0].shape)) __pyx_t_5 = 0;
-  if (unlikely(__pyx_t_5 != -1)) {
-    __Pyx_RaiseBufferIndexError(__pyx_t_5);
-    __PYX_ERR(0, 248, __pyx_L1_error)
+  __pyx_t_20 = 0;
+  __pyx_t_4 = -1;
+  if (__pyx_t_20 < 0) {
+    __pyx_t_20 += __pyx_pybuffernd_parallel_first_electron_fills.diminfo[0].shape;
+    if (unlikely(__pyx_t_20 < 0)) __pyx_t_4 = 0;
+  } else if (unlikely(__pyx_t_20 >= __pyx_pybuffernd_parallel_first_electron_fills.diminfo[0].shape)) __pyx_t_4 = 0;
+  if (unlikely(__pyx_t_4 != -1)) {
+    __Pyx_RaiseBufferIndexError(__pyx_t_4);
+    __PYX_ERR(2, 248, __pyx_L1_error)
   }
 
   /* "arcticpy/wrapper.pyx":250
  *         &parallel_first_electron_fills[0],
  *         # Traps
  *         &parallel_trap_densities[0],             # <<<<<<<<<<<<<<
  *         &parallel_trap_release_timescales[0],
  *         &parallel_trap_third_params[0],
  */
-  __pyx_t_19 = 0;
-  __pyx_t_5 = -1;
-  if (__pyx_t_19 < 0) {
-    __pyx_t_19 += __pyx_pybuffernd_parallel_trap_densities.diminfo[0].shape;
-    if (unlikely(__pyx_t_19 < 0)) __pyx_t_5 = 0;
-  } else if (unlikely(__pyx_t_19 >= __pyx_pybuffernd_parallel_trap_densities.diminfo[0].shape)) __pyx_t_5 = 0;
-  if (unlikely(__pyx_t_5 != -1)) {
-    __Pyx_RaiseBufferIndexError(__pyx_t_5);
-    __PYX_ERR(0, 250, __pyx_L1_error)
+  __pyx_t_21 = 0;
+  __pyx_t_4 = -1;
+  if (__pyx_t_21 < 0) {
+    __pyx_t_21 += __pyx_pybuffernd_parallel_trap_densities.diminfo[0].shape;
+    if (unlikely(__pyx_t_21 < 0)) __pyx_t_4 = 0;
+  } else if (unlikely(__pyx_t_21 >= __pyx_pybuffernd_parallel_trap_densities.diminfo[0].shape)) __pyx_t_4 = 0;
+  if (unlikely(__pyx_t_4 != -1)) {
+    __Pyx_RaiseBufferIndexError(__pyx_t_4);
+    __PYX_ERR(2, 250, __pyx_L1_error)
   }
 
   /* "arcticpy/wrapper.pyx":251
  *         # Traps
  *         &parallel_trap_densities[0],
  *         &parallel_trap_release_timescales[0],             # <<<<<<<<<<<<<<
  *         &parallel_trap_third_params[0],
  *         &parallel_trap_fourth_params[0],
  */
-  __pyx_t_20 = 0;
-  __pyx_t_5 = -1;
-  if (__pyx_t_20 < 0) {
-    __pyx_t_20 += __pyx_pybuffernd_parallel_trap_release_timescales.diminfo[0].shape;
-    if (unlikely(__pyx_t_20 < 0)) __pyx_t_5 = 0;
-  } else if (unlikely(__pyx_t_20 >= __pyx_pybuffernd_parallel_trap_release_timescales.diminfo[0].shape)) __pyx_t_5 = 0;
-  if (unlikely(__pyx_t_5 != -1)) {
-    __Pyx_RaiseBufferIndexError(__pyx_t_5);
-    __PYX_ERR(0, 251, __pyx_L1_error)
+  __pyx_t_22 = 0;
+  __pyx_t_4 = -1;
+  if (__pyx_t_22 < 0) {
+    __pyx_t_22 += __pyx_pybuffernd_parallel_trap_release_timescales.diminfo[0].shape;
+    if (unlikely(__pyx_t_22 < 0)) __pyx_t_4 = 0;
+  } else if (unlikely(__pyx_t_22 >= __pyx_pybuffernd_parallel_trap_release_timescales.diminfo[0].shape)) __pyx_t_4 = 0;
+  if (unlikely(__pyx_t_4 != -1)) {
+    __Pyx_RaiseBufferIndexError(__pyx_t_4);
+    __PYX_ERR(2, 251, __pyx_L1_error)
   }
 
   /* "arcticpy/wrapper.pyx":252
  *         &parallel_trap_densities[0],
  *         &parallel_trap_release_timescales[0],
  *         &parallel_trap_third_params[0],             # <<<<<<<<<<<<<<
  *         &parallel_trap_fourth_params[0],
  *         parallel_n_traps_ic,
  */
-  __pyx_t_21 = 0;
-  __pyx_t_5 = -1;
-  if (__pyx_t_21 < 0) {
-    __pyx_t_21 += __pyx_pybuffernd_parallel_trap_third_params.diminfo[0].shape;
-    if (unlikely(__pyx_t_21 < 0)) __pyx_t_5 = 0;
-  } else if (unlikely(__pyx_t_21 >= __pyx_pybuffernd_parallel_trap_third_params.diminfo[0].shape)) __pyx_t_5 = 0;
-  if (unlikely(__pyx_t_5 != -1)) {
-    __Pyx_RaiseBufferIndexError(__pyx_t_5);
-    __PYX_ERR(0, 252, __pyx_L1_error)
+  __pyx_t_23 = 0;
+  __pyx_t_4 = -1;
+  if (__pyx_t_23 < 0) {
+    __pyx_t_23 += __pyx_pybuffernd_parallel_trap_third_params.diminfo[0].shape;
+    if (unlikely(__pyx_t_23 < 0)) __pyx_t_4 = 0;
+  } else if (unlikely(__pyx_t_23 >= __pyx_pybuffernd_parallel_trap_third_params.diminfo[0].shape)) __pyx_t_4 = 0;
+  if (unlikely(__pyx_t_4 != -1)) {
+    __Pyx_RaiseBufferIndexError(__pyx_t_4);
+    __PYX_ERR(2, 252, __pyx_L1_error)
   }
 
   /* "arcticpy/wrapper.pyx":253
  *         &parallel_trap_release_timescales[0],
  *         &parallel_trap_third_params[0],
  *         &parallel_trap_fourth_params[0],             # <<<<<<<<<<<<<<
  *         parallel_n_traps_ic,
  *         parallel_n_traps_sc,
  */
-  __pyx_t_22 = 0;
-  __pyx_t_5 = -1;
-  if (__pyx_t_22 < 0) {
-    __pyx_t_22 += __pyx_pybuffernd_parallel_trap_fourth_params.diminfo[0].shape;
-    if (unlikely(__pyx_t_22 < 0)) __pyx_t_5 = 0;
-  } else if (unlikely(__pyx_t_22 >= __pyx_pybuffernd_parallel_trap_fourth_params.diminfo[0].shape)) __pyx_t_5 = 0;
-  if (unlikely(__pyx_t_5 != -1)) {
-    __Pyx_RaiseBufferIndexError(__pyx_t_5);
-    __PYX_ERR(0, 253, __pyx_L1_error)
+  __pyx_t_24 = 0;
+  __pyx_t_4 = -1;
+  if (__pyx_t_24 < 0) {
+    __pyx_t_24 += __pyx_pybuffernd_parallel_trap_fourth_params.diminfo[0].shape;
+    if (unlikely(__pyx_t_24 < 0)) __pyx_t_4 = 0;
+  } else if (unlikely(__pyx_t_24 >= __pyx_pybuffernd_parallel_trap_fourth_params.diminfo[0].shape)) __pyx_t_4 = 0;
+  if (unlikely(__pyx_t_4 != -1)) {
+    __Pyx_RaiseBufferIndexError(__pyx_t_4);
+    __PYX_ERR(2, 253, __pyx_L1_error)
   }
 
   /* "arcticpy/wrapper.pyx":265
  *         parallel_time_start,
  *         parallel_time_stop,
  *         &parallel_prune_n_electrons[0],             # <<<<<<<<<<<<<<
  *         parallel_prune_frequency,
  *         # ========
  */
-  __pyx_t_23 = 0;
-  __pyx_t_5 = -1;
-  if (__pyx_t_23 < 0) {
-    __pyx_t_23 += __pyx_pybuffernd_parallel_prune_n_electrons.diminfo[0].shape;
-    if (unlikely(__pyx_t_23 < 0)) __pyx_t_5 = 0;
-  } else if (unlikely(__pyx_t_23 >= __pyx_pybuffernd_parallel_prune_n_electrons.diminfo[0].shape)) __pyx_t_5 = 0;
-  if (unlikely(__pyx_t_5 != -1)) {
-    __Pyx_RaiseBufferIndexError(__pyx_t_5);
-    __PYX_ERR(0, 265, __pyx_L1_error)
+  __pyx_t_25 = 0;
+  __pyx_t_4 = -1;
+  if (__pyx_t_25 < 0) {
+    __pyx_t_25 += __pyx_pybuffernd_parallel_prune_n_electrons.diminfo[0].shape;
+    if (unlikely(__pyx_t_25 < 0)) __pyx_t_4 = 0;
+  } else if (unlikely(__pyx_t_25 >= __pyx_pybuffernd_parallel_prune_n_electrons.diminfo[0].shape)) __pyx_t_4 = 0;
+  if (unlikely(__pyx_t_4 != -1)) {
+    __Pyx_RaiseBufferIndexError(__pyx_t_4);
+    __PYX_ERR(2, 265, __pyx_L1_error)
   }
 
   /* "arcticpy/wrapper.pyx":271
  *         # ========
  *         # ROE
  *         &serial_dwell_times[0],             # <<<<<<<<<<<<<<
  *         len(serial_dwell_times),
  *         serial_prescan_offset,
  */
-  __pyx_t_24 = 0;
-  __pyx_t_5 = -1;
-  if (__pyx_t_24 < 0) {
-    __pyx_t_24 += __pyx_pybuffernd_serial_dwell_times.diminfo[0].shape;
-    if (unlikely(__pyx_t_24 < 0)) __pyx_t_5 = 0;
-  } else if (unlikely(__pyx_t_24 >= __pyx_pybuffernd_serial_dwell_times.diminfo[0].shape)) __pyx_t_5 = 0;
-  if (unlikely(__pyx_t_5 != -1)) {
-    __Pyx_RaiseBufferIndexError(__pyx_t_5);
-    __PYX_ERR(0, 271, __pyx_L1_error)
+  __pyx_t_26 = 0;
+  __pyx_t_4 = -1;
+  if (__pyx_t_26 < 0) {
+    __pyx_t_26 += __pyx_pybuffernd_serial_dwell_times.diminfo[0].shape;
+    if (unlikely(__pyx_t_26 < 0)) __pyx_t_4 = 0;
+  } else if (unlikely(__pyx_t_26 >= __pyx_pybuffernd_serial_dwell_times.diminfo[0].shape)) __pyx_t_4 = 0;
+  if (unlikely(__pyx_t_4 != -1)) {
+    __Pyx_RaiseBufferIndexError(__pyx_t_4);
+    __PYX_ERR(2, 271, __pyx_L1_error)
   }
 
   /* "arcticpy/wrapper.pyx":272
  *         # ROE
  *         &serial_dwell_times[0],
  *         len(serial_dwell_times),             # <<<<<<<<<<<<<<
  *         serial_prescan_offset,
  *         serial_overscan_start,
  */
-  __pyx_t_25 = PyObject_Length(((PyObject *)__pyx_v_serial_dwell_times)); if (unlikely(__pyx_t_25 == ((Py_ssize_t)-1))) __PYX_ERR(0, 272, __pyx_L1_error)
+  __pyx_t_27 = PyObject_Length(((PyObject *)__pyx_v_serial_dwell_times)); if (unlikely(__pyx_t_27 == ((Py_ssize_t)-1))) __PYX_ERR(2, 272, __pyx_L1_error)
 
   /* "arcticpy/wrapper.pyx":282
  *         serial_roe_type,
  *         # CCD
  *         &serial_fraction_of_traps_per_phase[0],             # <<<<<<<<<<<<<<
  *         len(serial_fraction_of_traps_per_phase),
  *         &serial_full_well_depths[0],
  */
-  __pyx_t_26 = 0;
-  __pyx_t_5 = -1;
-  if (__pyx_t_26 < 0) {
-    __pyx_t_26 += __pyx_pybuffernd_serial_fraction_of_traps_per_phase.diminfo[0].shape;
-    if (unlikely(__pyx_t_26 < 0)) __pyx_t_5 = 0;
-  } else if (unlikely(__pyx_t_26 >= __pyx_pybuffernd_serial_fraction_of_traps_per_phase.diminfo[0].shape)) __pyx_t_5 = 0;
-  if (unlikely(__pyx_t_5 != -1)) {
-    __Pyx_RaiseBufferIndexError(__pyx_t_5);
-    __PYX_ERR(0, 282, __pyx_L1_error)
+  __pyx_t_28 = 0;
+  __pyx_t_4 = -1;
+  if (__pyx_t_28 < 0) {
+    __pyx_t_28 += __pyx_pybuffernd_serial_fraction_of_traps_per_phase.diminfo[0].shape;
+    if (unlikely(__pyx_t_28 < 0)) __pyx_t_4 = 0;
+  } else if (unlikely(__pyx_t_28 >= __pyx_pybuffernd_serial_fraction_of_traps_per_phase.diminfo[0].shape)) __pyx_t_4 = 0;
+  if (unlikely(__pyx_t_4 != -1)) {
+    __Pyx_RaiseBufferIndexError(__pyx_t_4);
+    __PYX_ERR(2, 282, __pyx_L1_error)
   }
 
   /* "arcticpy/wrapper.pyx":283
  *         # CCD
  *         &serial_fraction_of_traps_per_phase[0],
  *         len(serial_fraction_of_traps_per_phase),             # <<<<<<<<<<<<<<
  *         &serial_full_well_depths[0],
  *         &serial_well_notch_depths[0],
  */
-  __pyx_t_27 = PyObject_Length(((PyObject *)__pyx_v_serial_fraction_of_traps_per_phase)); if (unlikely(__pyx_t_27 == ((Py_ssize_t)-1))) __PYX_ERR(0, 283, __pyx_L1_error)
+  __pyx_t_29 = PyObject_Length(((PyObject *)__pyx_v_serial_fraction_of_traps_per_phase)); if (unlikely(__pyx_t_29 == ((Py_ssize_t)-1))) __PYX_ERR(2, 283, __pyx_L1_error)
 
   /* "arcticpy/wrapper.pyx":284
  *         &serial_fraction_of_traps_per_phase[0],
  *         len(serial_fraction_of_traps_per_phase),
  *         &serial_full_well_depths[0],             # <<<<<<<<<<<<<<
  *         &serial_well_notch_depths[0],
  *         &serial_well_fill_powers[0],
  */
-  __pyx_t_28 = 0;
-  __pyx_t_5 = -1;
-  if (__pyx_t_28 < 0) {
-    __pyx_t_28 += __pyx_pybuffernd_serial_full_well_depths.diminfo[0].shape;
-    if (unlikely(__pyx_t_28 < 0)) __pyx_t_5 = 0;
-  } else if (unlikely(__pyx_t_28 >= __pyx_pybuffernd_serial_full_well_depths.diminfo[0].shape)) __pyx_t_5 = 0;
-  if (unlikely(__pyx_t_5 != -1)) {
-    __Pyx_RaiseBufferIndexError(__pyx_t_5);
-    __PYX_ERR(0, 284, __pyx_L1_error)
+  __pyx_t_30 = 0;
+  __pyx_t_4 = -1;
+  if (__pyx_t_30 < 0) {
+    __pyx_t_30 += __pyx_pybuffernd_serial_full_well_depths.diminfo[0].shape;
+    if (unlikely(__pyx_t_30 < 0)) __pyx_t_4 = 0;
+  } else if (unlikely(__pyx_t_30 >= __pyx_pybuffernd_serial_full_well_depths.diminfo[0].shape)) __pyx_t_4 = 0;
+  if (unlikely(__pyx_t_4 != -1)) {
+    __Pyx_RaiseBufferIndexError(__pyx_t_4);
+    __PYX_ERR(2, 284, __pyx_L1_error)
   }
 
   /* "arcticpy/wrapper.pyx":285
  *         len(serial_fraction_of_traps_per_phase),
  *         &serial_full_well_depths[0],
  *         &serial_well_notch_depths[0],             # <<<<<<<<<<<<<<
  *         &serial_well_fill_powers[0],
  *         &serial_first_electron_fills[0],
  */
-  __pyx_t_29 = 0;
-  __pyx_t_5 = -1;
-  if (__pyx_t_29 < 0) {
-    __pyx_t_29 += __pyx_pybuffernd_serial_well_notch_depths.diminfo[0].shape;
-    if (unlikely(__pyx_t_29 < 0)) __pyx_t_5 = 0;
-  } else if (unlikely(__pyx_t_29 >= __pyx_pybuffernd_serial_well_notch_depths.diminfo[0].shape)) __pyx_t_5 = 0;
-  if (unlikely(__pyx_t_5 != -1)) {
-    __Pyx_RaiseBufferIndexError(__pyx_t_5);
-    __PYX_ERR(0, 285, __pyx_L1_error)
+  __pyx_t_31 = 0;
+  __pyx_t_4 = -1;
+  if (__pyx_t_31 < 0) {
+    __pyx_t_31 += __pyx_pybuffernd_serial_well_notch_depths.diminfo[0].shape;
+    if (unlikely(__pyx_t_31 < 0)) __pyx_t_4 = 0;
+  } else if (unlikely(__pyx_t_31 >= __pyx_pybuffernd_serial_well_notch_depths.diminfo[0].shape)) __pyx_t_4 = 0;
+  if (unlikely(__pyx_t_4 != -1)) {
+    __Pyx_RaiseBufferIndexError(__pyx_t_4);
+    __PYX_ERR(2, 285, __pyx_L1_error)
   }
 
   /* "arcticpy/wrapper.pyx":286
  *         &serial_full_well_depths[0],
  *         &serial_well_notch_depths[0],
  *         &serial_well_fill_powers[0],             # <<<<<<<<<<<<<<
  *         &serial_first_electron_fills[0],
  *         # Traps
  */
-  __pyx_t_30 = 0;
-  __pyx_t_5 = -1;
-  if (__pyx_t_30 < 0) {
-    __pyx_t_30 += __pyx_pybuffernd_serial_well_fill_powers.diminfo[0].shape;
-    if (unlikely(__pyx_t_30 < 0)) __pyx_t_5 = 0;
-  } else if (unlikely(__pyx_t_30 >= __pyx_pybuffernd_serial_well_fill_powers.diminfo[0].shape)) __pyx_t_5 = 0;
-  if (unlikely(__pyx_t_5 != -1)) {
-    __Pyx_RaiseBufferIndexError(__pyx_t_5);
-    __PYX_ERR(0, 286, __pyx_L1_error)
+  __pyx_t_32 = 0;
+  __pyx_t_4 = -1;
+  if (__pyx_t_32 < 0) {
+    __pyx_t_32 += __pyx_pybuffernd_serial_well_fill_powers.diminfo[0].shape;
+    if (unlikely(__pyx_t_32 < 0)) __pyx_t_4 = 0;
+  } else if (unlikely(__pyx_t_32 >= __pyx_pybuffernd_serial_well_fill_powers.diminfo[0].shape)) __pyx_t_4 = 0;
+  if (unlikely(__pyx_t_4 != -1)) {
+    __Pyx_RaiseBufferIndexError(__pyx_t_4);
+    __PYX_ERR(2, 286, __pyx_L1_error)
   }
 
   /* "arcticpy/wrapper.pyx":287
  *         &serial_well_notch_depths[0],
  *         &serial_well_fill_powers[0],
  *         &serial_first_electron_fills[0],             # <<<<<<<<<<<<<<
  *         # Traps
  *         &serial_trap_densities[0],
  */
-  __pyx_t_31 = 0;
-  __pyx_t_5 = -1;
-  if (__pyx_t_31 < 0) {
-    __pyx_t_31 += __pyx_pybuffernd_serial_first_electron_fills.diminfo[0].shape;
-    if (unlikely(__pyx_t_31 < 0)) __pyx_t_5 = 0;
-  } else if (unlikely(__pyx_t_31 >= __pyx_pybuffernd_serial_first_electron_fills.diminfo[0].shape)) __pyx_t_5 = 0;
-  if (unlikely(__pyx_t_5 != -1)) {
-    __Pyx_RaiseBufferIndexError(__pyx_t_5);
-    __PYX_ERR(0, 287, __pyx_L1_error)
+  __pyx_t_33 = 0;
+  __pyx_t_4 = -1;
+  if (__pyx_t_33 < 0) {
+    __pyx_t_33 += __pyx_pybuffernd_serial_first_electron_fills.diminfo[0].shape;
+    if (unlikely(__pyx_t_33 < 0)) __pyx_t_4 = 0;
+  } else if (unlikely(__pyx_t_33 >= __pyx_pybuffernd_serial_first_electron_fills.diminfo[0].shape)) __pyx_t_4 = 0;
+  if (unlikely(__pyx_t_4 != -1)) {
+    __Pyx_RaiseBufferIndexError(__pyx_t_4);
+    __PYX_ERR(2, 287, __pyx_L1_error)
   }
 
   /* "arcticpy/wrapper.pyx":289
  *         &serial_first_electron_fills[0],
  *         # Traps
  *         &serial_trap_densities[0],             # <<<<<<<<<<<<<<
  *         &serial_trap_release_timescales[0],
  *         &serial_trap_third_params[0],
  */
-  __pyx_t_32 = 0;
-  __pyx_t_5 = -1;
-  if (__pyx_t_32 < 0) {
-    __pyx_t_32 += __pyx_pybuffernd_serial_trap_densities.diminfo[0].shape;
-    if (unlikely(__pyx_t_32 < 0)) __pyx_t_5 = 0;
-  } else if (unlikely(__pyx_t_32 >= __pyx_pybuffernd_serial_trap_densities.diminfo[0].shape)) __pyx_t_5 = 0;
-  if (unlikely(__pyx_t_5 != -1)) {
-    __Pyx_RaiseBufferIndexError(__pyx_t_5);
-    __PYX_ERR(0, 289, __pyx_L1_error)
+  __pyx_t_34 = 0;
+  __pyx_t_4 = -1;
+  if (__pyx_t_34 < 0) {
+    __pyx_t_34 += __pyx_pybuffernd_serial_trap_densities.diminfo[0].shape;
+    if (unlikely(__pyx_t_34 < 0)) __pyx_t_4 = 0;
+  } else if (unlikely(__pyx_t_34 >= __pyx_pybuffernd_serial_trap_densities.diminfo[0].shape)) __pyx_t_4 = 0;
+  if (unlikely(__pyx_t_4 != -1)) {
+    __Pyx_RaiseBufferIndexError(__pyx_t_4);
+    __PYX_ERR(2, 289, __pyx_L1_error)
   }
 
   /* "arcticpy/wrapper.pyx":290
  *         # Traps
  *         &serial_trap_densities[0],
  *         &serial_trap_release_timescales[0],             # <<<<<<<<<<<<<<
  *         &serial_trap_third_params[0],
  *         &serial_trap_fourth_params[0],
  */
-  __pyx_t_33 = 0;
-  __pyx_t_5 = -1;
-  if (__pyx_t_33 < 0) {
-    __pyx_t_33 += __pyx_pybuffernd_serial_trap_release_timescales.diminfo[0].shape;
-    if (unlikely(__pyx_t_33 < 0)) __pyx_t_5 = 0;
-  } else if (unlikely(__pyx_t_33 >= __pyx_pybuffernd_serial_trap_release_timescales.diminfo[0].shape)) __pyx_t_5 = 0;
-  if (unlikely(__pyx_t_5 != -1)) {
-    __Pyx_RaiseBufferIndexError(__pyx_t_5);
-    __PYX_ERR(0, 290, __pyx_L1_error)
+  __pyx_t_35 = 0;
+  __pyx_t_4 = -1;
+  if (__pyx_t_35 < 0) {
+    __pyx_t_35 += __pyx_pybuffernd_serial_trap_release_timescales.diminfo[0].shape;
+    if (unlikely(__pyx_t_35 < 0)) __pyx_t_4 = 0;
+  } else if (unlikely(__pyx_t_35 >= __pyx_pybuffernd_serial_trap_release_timescales.diminfo[0].shape)) __pyx_t_4 = 0;
+  if (unlikely(__pyx_t_4 != -1)) {
+    __Pyx_RaiseBufferIndexError(__pyx_t_4);
+    __PYX_ERR(2, 290, __pyx_L1_error)
   }
 
   /* "arcticpy/wrapper.pyx":291
  *         &serial_trap_densities[0],
  *         &serial_trap_release_timescales[0],
  *         &serial_trap_third_params[0],             # <<<<<<<<<<<<<<
  *         &serial_trap_fourth_params[0],
  *         serial_n_traps_ic,
  */
-  __pyx_t_34 = 0;
-  __pyx_t_5 = -1;
-  if (__pyx_t_34 < 0) {
-    __pyx_t_34 += __pyx_pybuffernd_serial_trap_third_params.diminfo[0].shape;
-    if (unlikely(__pyx_t_34 < 0)) __pyx_t_5 = 0;
-  } else if (unlikely(__pyx_t_34 >= __pyx_pybuffernd_serial_trap_third_params.diminfo[0].shape)) __pyx_t_5 = 0;
-  if (unlikely(__pyx_t_5 != -1)) {
-    __Pyx_RaiseBufferIndexError(__pyx_t_5);
-    __PYX_ERR(0, 291, __pyx_L1_error)
+  __pyx_t_36 = 0;
+  __pyx_t_4 = -1;
+  if (__pyx_t_36 < 0) {
+    __pyx_t_36 += __pyx_pybuffernd_serial_trap_third_params.diminfo[0].shape;
+    if (unlikely(__pyx_t_36 < 0)) __pyx_t_4 = 0;
+  } else if (unlikely(__pyx_t_36 >= __pyx_pybuffernd_serial_trap_third_params.diminfo[0].shape)) __pyx_t_4 = 0;
+  if (unlikely(__pyx_t_4 != -1)) {
+    __Pyx_RaiseBufferIndexError(__pyx_t_4);
+    __PYX_ERR(2, 291, __pyx_L1_error)
   }
 
   /* "arcticpy/wrapper.pyx":292
  *         &serial_trap_release_timescales[0],
  *         &serial_trap_third_params[0],
  *         &serial_trap_fourth_params[0],             # <<<<<<<<<<<<<<
  *         serial_n_traps_ic,
  *         serial_n_traps_sc,
  */
-  __pyx_t_35 = 0;
-  __pyx_t_5 = -1;
-  if (__pyx_t_35 < 0) {
-    __pyx_t_35 += __pyx_pybuffernd_serial_trap_fourth_params.diminfo[0].shape;
-    if (unlikely(__pyx_t_35 < 0)) __pyx_t_5 = 0;
-  } else if (unlikely(__pyx_t_35 >= __pyx_pybuffernd_serial_trap_fourth_params.diminfo[0].shape)) __pyx_t_5 = 0;
-  if (unlikely(__pyx_t_5 != -1)) {
-    __Pyx_RaiseBufferIndexError(__pyx_t_5);
-    __PYX_ERR(0, 292, __pyx_L1_error)
+  __pyx_t_37 = 0;
+  __pyx_t_4 = -1;
+  if (__pyx_t_37 < 0) {
+    __pyx_t_37 += __pyx_pybuffernd_serial_trap_fourth_params.diminfo[0].shape;
+    if (unlikely(__pyx_t_37 < 0)) __pyx_t_4 = 0;
+  } else if (unlikely(__pyx_t_37 >= __pyx_pybuffernd_serial_trap_fourth_params.diminfo[0].shape)) __pyx_t_4 = 0;
+  if (unlikely(__pyx_t_4 != -1)) {
+    __Pyx_RaiseBufferIndexError(__pyx_t_4);
+    __PYX_ERR(2, 292, __pyx_L1_error)
   }
 
   /* "arcticpy/wrapper.pyx":304
  *         serial_time_start,
  *         serial_time_stop,
  *         &serial_prune_n_electrons[0],             # <<<<<<<<<<<<<<
  *         serial_prune_frequency,
  *         # ========
  */
-  __pyx_t_36 = 0;
-  __pyx_t_5 = -1;
-  if (__pyx_t_36 < 0) {
-    __pyx_t_36 += __pyx_pybuffernd_serial_prune_n_electrons.diminfo[0].shape;
-    if (unlikely(__pyx_t_36 < 0)) __pyx_t_5 = 0;
-  } else if (unlikely(__pyx_t_36 >= __pyx_pybuffernd_serial_prune_n_electrons.diminfo[0].shape)) __pyx_t_5 = 0;
-  if (unlikely(__pyx_t_5 != -1)) {
-    __Pyx_RaiseBufferIndexError(__pyx_t_5);
-    __PYX_ERR(0, 304, __pyx_L1_error)
+  __pyx_t_38 = 0;
+  __pyx_t_4 = -1;
+  if (__pyx_t_38 < 0) {
+    __pyx_t_38 += __pyx_pybuffernd_serial_prune_n_electrons.diminfo[0].shape;
+    if (unlikely(__pyx_t_38 < 0)) __pyx_t_4 = 0;
+  } else if (unlikely(__pyx_t_38 >= __pyx_pybuffernd_serial_prune_n_electrons.diminfo[0].shape)) __pyx_t_4 = 0;
+  if (unlikely(__pyx_t_4 != -1)) {
+    __Pyx_RaiseBufferIndexError(__pyx_t_4);
+    __PYX_ERR(2, 304, __pyx_L1_error)
   }
 
   /* "arcticpy/wrapper.pyx":224
  *     image = check_contiguous(image)
  * 
  *     add_cti(             # <<<<<<<<<<<<<<
  *         &image[0, 0],
  *         image.shape[0],
  */
-  add_cti((&(*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_image.rcbuffer->pybuffer.buf, __pyx_t_9, __pyx_pybuffernd_image.diminfo[0].strides, __pyx_t_10, __pyx_pybuffernd_image.diminfo[1].strides))), (__pyx_v_image->dimensions[0]), (__pyx_v_image->dimensions[1]), (&(*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_parallel_dwell_times.rcbuffer->pybuffer.buf, __pyx_t_11, __pyx_pybuffernd_parallel_dwell_times.diminfo[0].strides))), __pyx_t_12, __pyx_v_parallel_prescan_offset, __pyx_v_parallel_overscan_start, __pyx_v_parallel_empty_traps_between_columns, __pyx_v_parallel_empty_traps_for_first_transfers, __pyx_v_parallel_force_release_away_from_readout, __pyx_v_parallel_use_integer_express_matrix, __pyx_v_parallel_n_pumps, __pyx_v_parallel_roe_type, (&(*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_parallel_fraction_of_traps_per_phase.rcbuffer->pybuffer.buf, __pyx_t_13, __pyx_pybuffernd_parallel_fraction_of_traps_per_phase.diminfo[0].strides))), __pyx_t_14, (&(*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_parallel_full_well_depths.rcbuffer->pybuffer.buf, __pyx_t_15, __pyx_pybuffernd_parallel_full_well_depths.diminfo[0].strides))), (&(*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_parallel_well_notch_depths.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_parallel_well_notch_depths.diminfo[0].strides))), (&(*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_parallel_well_fill_powers.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_parallel_well_fill_powers.diminfo[0].strides))), (&(*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_parallel_first_electron_fills.rcbuffer->pybuffer.buf, __pyx_t_18, __pyx_pybuffernd_parallel_first_electron_fills.diminfo[0].strides))), (&(*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_parallel_trap_densities.rcbuffer->pybuffer.buf, __pyx_t_19, __pyx_pybuffernd_parallel_trap_densities.diminfo[0].strides))), (&(*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_parallel_trap_release_timescales.rcbuffer->pybuffer.buf, __pyx_t_20, __pyx_pybuffernd_parallel_trap_release_timescales.diminfo[0].strides))), (&(*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_parallel_trap_third_params.rcbuffer->pybuffer.buf, __pyx_t_21, __pyx_pybuffernd_parallel_trap_third_params.diminfo[0].strides))), (&(*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_parallel_trap_fourth_params.rcbuffer->pybuffer.buf, __pyx_t_22, __pyx_pybuffernd_parallel_trap_fourth_params.diminfo[0].strides))), __pyx_v_parallel_n_traps_ic, __pyx_v_parallel_n_traps_sc, __pyx_v_parallel_n_traps_ic_co, __pyx_v_parallel_n_traps_sc_co, __pyx_v_parallel_express, __pyx_v_parallel_window_offset, __pyx_v_parallel_window_start, __pyx_v_parallel_window_stop, __pyx_v_parallel_time_start, __pyx_v_parallel_time_stop, (&(*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_parallel_prune_n_electrons.rcbuffer->pybuffer.buf, __pyx_t_23, __pyx_pybuffernd_parallel_prune_n_electrons.diminfo[0].strides))), __pyx_v_parallel_prune_frequency, (&(*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_serial_dwell_times.rcbuffer->pybuffer.buf, __pyx_t_24, __pyx_pybuffernd_serial_dwell_times.diminfo[0].strides))), __pyx_t_25, __pyx_v_serial_prescan_offset, __pyx_v_serial_overscan_start, __pyx_v_serial_empty_traps_between_columns, __pyx_v_serial_empty_traps_for_first_transfers, __pyx_v_serial_force_release_away_from_readout, __pyx_v_serial_use_integer_express_matrix, __pyx_v_serial_n_pumps, __pyx_v_serial_roe_type, (&(*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_serial_fraction_of_traps_per_phase.rcbuffer->pybuffer.buf, __pyx_t_26, __pyx_pybuffernd_serial_fraction_of_traps_per_phase.diminfo[0].strides))), __pyx_t_27, (&(*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_serial_full_well_depths.rcbuffer->pybuffer.buf, __pyx_t_28, __pyx_pybuffernd_serial_full_well_depths.diminfo[0].strides))), (&(*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_serial_well_notch_depths.rcbuffer->pybuffer.buf, __pyx_t_29, __pyx_pybuffernd_serial_well_notch_depths.diminfo[0].strides))), (&(*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_serial_well_fill_powers.rcbuffer->pybuffer.buf, __pyx_t_30, __pyx_pybuffernd_serial_well_fill_powers.diminfo[0].strides))), (&(*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_serial_first_electron_fills.rcbuffer->pybuffer.buf, __pyx_t_31, __pyx_pybuffernd_serial_first_electron_fills.diminfo[0].strides))), (&(*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_serial_trap_densities.rcbuffer->pybuffer.buf, __pyx_t_32, __pyx_pybuffernd_serial_trap_densities.diminfo[0].strides))), (&(*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_serial_trap_release_timescales.rcbuffer->pybuffer.buf, __pyx_t_33, __pyx_pybuffernd_serial_trap_release_timescales.diminfo[0].strides))), (&(*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_serial_trap_third_params.rcbuffer->pybuffer.buf, __pyx_t_34, __pyx_pybuffernd_serial_trap_third_params.diminfo[0].strides))), (&(*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_serial_trap_fourth_params.rcbuffer->pybuffer.buf, __pyx_t_35, __pyx_pybuffernd_serial_trap_fourth_params.diminfo[0].strides))), __pyx_v_serial_n_traps_ic, __pyx_v_serial_n_traps_sc, __pyx_v_serial_n_traps_ic_co, __pyx_v_serial_n_traps_sc_co, __pyx_v_serial_express, __pyx_v_serial_window_offset, __pyx_v_serial_window_start, __pyx_v_serial_window_stop, __pyx_v_serial_time_start, __pyx_v_serial_time_stop, (&(*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_serial_prune_n_electrons.rcbuffer->pybuffer.buf, __pyx_t_36, __pyx_pybuffernd_serial_prune_n_electrons.diminfo[0].strides))), __pyx_v_serial_prune_frequency, __pyx_v_allow_negative_pixels, __pyx_v_verbosity, __pyx_v_iteration);
+  add_cti((&(*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_image.rcbuffer->pybuffer.buf, __pyx_t_9, __pyx_pybuffernd_image.diminfo[0].strides, __pyx_t_10, __pyx_pybuffernd_image.diminfo[1].strides))), (__pyx_t_11[0]), (__pyx_t_12[1]), (&(*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_parallel_dwell_times.rcbuffer->pybuffer.buf, __pyx_t_13, __pyx_pybuffernd_parallel_dwell_times.diminfo[0].strides))), __pyx_t_14, __pyx_v_parallel_prescan_offset, __pyx_v_parallel_overscan_start, __pyx_v_parallel_empty_traps_between_columns, __pyx_v_parallel_empty_traps_for_first_transfers, __pyx_v_parallel_force_release_away_from_readout, __pyx_v_parallel_use_integer_express_matrix, __pyx_v_parallel_n_pumps, __pyx_v_parallel_roe_type, (&(*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_parallel_fraction_of_traps_per_phase.rcbuffer->pybuffer.buf, __pyx_t_15, __pyx_pybuffernd_parallel_fraction_of_traps_per_phase.diminfo[0].strides))), __pyx_t_16, (&(*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_parallel_full_well_depths.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_parallel_full_well_depths.diminfo[0].strides))), (&(*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_parallel_well_notch_depths.rcbuffer->pybuffer.buf, __pyx_t_18, __pyx_pybuffernd_parallel_well_notch_depths.diminfo[0].strides))), (&(*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_parallel_well_fill_powers.rcbuffer->pybuffer.buf, __pyx_t_19, __pyx_pybuffernd_parallel_well_fill_powers.diminfo[0].strides))), (&(*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_parallel_first_electron_fills.rcbuffer->pybuffer.buf, __pyx_t_20, __pyx_pybuffernd_parallel_first_electron_fills.diminfo[0].strides))), (&(*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_parallel_trap_densities.rcbuffer->pybuffer.buf, __pyx_t_21, __pyx_pybuffernd_parallel_trap_densities.diminfo[0].strides))), (&(*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_parallel_trap_release_timescales.rcbuffer->pybuffer.buf, __pyx_t_22, __pyx_pybuffernd_parallel_trap_release_timescales.diminfo[0].strides))), (&(*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_parallel_trap_third_params.rcbuffer->pybuffer.buf, __pyx_t_23, __pyx_pybuffernd_parallel_trap_third_params.diminfo[0].strides))), (&(*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_parallel_trap_fourth_params.rcbuffer->pybuffer.buf, __pyx_t_24, __pyx_pybuffernd_parallel_trap_fourth_params.diminfo[0].strides))), __pyx_v_parallel_n_traps_ic, __pyx_v_parallel_n_traps_sc, __pyx_v_parallel_n_traps_ic_co, __pyx_v_parallel_n_traps_sc_co, __pyx_v_parallel_express, __pyx_v_parallel_window_offset, __pyx_v_parallel_window_start, __pyx_v_parallel_window_stop, __pyx_v_parallel_time_start, __pyx_v_parallel_time_stop, (&(*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_parallel_prune_n_electrons.rcbuffer->pybuffer.buf, __pyx_t_25, __pyx_pybuffernd_parallel_prune_n_electrons.diminfo[0].strides))), __pyx_v_parallel_prune_frequency, (&(*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_serial_dwell_times.rcbuffer->pybuffer.buf, __pyx_t_26, __pyx_pybuffernd_serial_dwell_times.diminfo[0].strides))), __pyx_t_27, __pyx_v_serial_prescan_offset, __pyx_v_serial_overscan_start, __pyx_v_serial_empty_traps_between_columns, __pyx_v_serial_empty_traps_for_first_transfers, __pyx_v_serial_force_release_away_from_readout, __pyx_v_serial_use_integer_express_matrix, __pyx_v_serial_n_pumps, __pyx_v_serial_roe_type, (&(*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_serial_fraction_of_traps_per_phase.rcbuffer->pybuffer.buf, __pyx_t_28, __pyx_pybuffernd_serial_fraction_of_traps_per_phase.diminfo[0].strides))), __pyx_t_29, (&(*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_serial_full_well_depths.rcbuffer->pybuffer.buf, __pyx_t_30, __pyx_pybuffernd_serial_full_well_depths.diminfo[0].strides))), (&(*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_serial_well_notch_depths.rcbuffer->pybuffer.buf, __pyx_t_31, __pyx_pybuffernd_serial_well_notch_depths.diminfo[0].strides))), (&(*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_serial_well_fill_powers.rcbuffer->pybuffer.buf, __pyx_t_32, __pyx_pybuffernd_serial_well_fill_powers.diminfo[0].strides))), (&(*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_serial_first_electron_fills.rcbuffer->pybuffer.buf, __pyx_t_33, __pyx_pybuffernd_serial_first_electron_fills.diminfo[0].strides))), (&(*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_serial_trap_densities.rcbuffer->pybuffer.buf, __pyx_t_34, __pyx_pybuffernd_serial_trap_densities.diminfo[0].strides))), (&(*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_serial_trap_release_timescales.rcbuffer->pybuffer.buf, __pyx_t_35, __pyx_pybuffernd_serial_trap_release_timescales.diminfo[0].strides))), (&(*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_serial_trap_third_params.rcbuffer->pybuffer.buf, __pyx_t_36, __pyx_pybuffernd_serial_trap_third_params.diminfo[0].strides))), (&(*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_serial_trap_fourth_params.rcbuffer->pybuffer.buf, __pyx_t_37, __pyx_pybuffernd_serial_trap_fourth_params.diminfo[0].strides))), __pyx_v_serial_n_traps_ic, __pyx_v_serial_n_traps_sc, __pyx_v_serial_n_traps_ic_co, __pyx_v_serial_n_traps_sc_co, __pyx_v_serial_express, __pyx_v_serial_window_offset, __pyx_v_serial_window_start, __pyx_v_serial_window_stop, __pyx_v_serial_time_start, __pyx_v_serial_time_stop, (&(*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_serial_prune_n_electrons.rcbuffer->pybuffer.buf, __pyx_t_38, __pyx_pybuffernd_serial_prune_n_electrons.diminfo[0].strides))), __pyx_v_serial_prune_frequency, __pyx_v_allow_negative_pixels, __pyx_v_verbosity, __pyx_v_iteration);
 
   /* "arcticpy/wrapper.pyx":315
  *     )
  * 
  *     return image             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_INCREF(((PyObject *)__pyx_v_image));
+  __Pyx_INCREF((PyObject *)__pyx_v_image);
   __pyx_r = ((PyObject *)__pyx_v_image);
   goto __pyx_L0;
 
   /* "arcticpy/wrapper.pyx":131
  * 
  * 
  * def cy_add_cti(             # <<<<<<<<<<<<<<
@@ -4368,1525 +7321,261 @@
   __pyx_L2:;
   __Pyx_XDECREF((PyObject *)__pyx_v_image);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":734
- * ctypedef npy_cdouble     complex_t
- * 
- * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
- *     return PyArray_MultiIterNew(1, <void*>a)
- * 
- */
-
-static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew1(PyObject *__pyx_v_a) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
-
-  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":735
- * 
- * cdef inline object PyArray_MultiIterNew1(a):
- *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
- * 
- * cdef inline object PyArray_MultiIterNew2(a, b):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":734
- * ctypedef npy_cdouble     complex_t
- * 
- * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
- *     return PyArray_MultiIterNew(1, <void*>a)
- * 
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("numpy.PyArray_MultiIterNew1", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":737
- *     return PyArray_MultiIterNew(1, <void*>a)
- * 
- * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
- *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
- * 
- */
-
-static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew2(PyObject *__pyx_v_a, PyObject *__pyx_v_b) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
-
-  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":738
- * 
- * cdef inline object PyArray_MultiIterNew2(a, b):
- *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
- * 
- * cdef inline object PyArray_MultiIterNew3(a, b, c):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":737
- *     return PyArray_MultiIterNew(1, <void*>a)
- * 
- * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
- *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
- * 
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("numpy.PyArray_MultiIterNew2", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":740
- *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
- * 
- * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
- *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
- * 
- */
-
-static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew3(PyObject *__pyx_v_a, PyObject *__pyx_v_b, PyObject *__pyx_v_c) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
-
-  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":741
- * 
- * cdef inline object PyArray_MultiIterNew3(a, b, c):
- *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
- * 
- * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":740
- *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
- * 
- * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
- *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
- * 
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("numpy.PyArray_MultiIterNew3", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":743
- *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
- * 
- * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
- *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
- * 
- */
-
-static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew4(PyObject *__pyx_v_a, PyObject *__pyx_v_b, PyObject *__pyx_v_c, PyObject *__pyx_v_d) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
-
-  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":744
- * 
- * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
- *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
- * 
- * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":743
- *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
- * 
- * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
- *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
- * 
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("numpy.PyArray_MultiIterNew4", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":746
- *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
- * 
- * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
- *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
- * 
- */
-
-static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew5(PyObject *__pyx_v_a, PyObject *__pyx_v_b, PyObject *__pyx_v_c, PyObject *__pyx_v_d, PyObject *__pyx_v_e) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
-
-  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":747
- * 
- * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
- *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
- * 
- * cdef inline tuple PyDataType_SHAPE(dtype d):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 747, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":746
- *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
- * 
- * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
- *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
- * 
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("numpy.PyArray_MultiIterNew5", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":749
- *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
- * 
- * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
- *     if PyDataType_HASSUBARRAY(d):
- *         return <tuple>d.subarray.shape
- */
-
-static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
-
-  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":750
- * 
- * cdef inline tuple PyDataType_SHAPE(dtype d):
- *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
- *         return <tuple>d.subarray.shape
- *     else:
- */
-  __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
-  if (__pyx_t_1) {
-
-    /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":751
- * cdef inline tuple PyDataType_SHAPE(dtype d):
- *     if PyDataType_HASSUBARRAY(d):
- *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
- *     else:
- *         return ()
- */
-    __Pyx_XDECREF(__pyx_r);
-    __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
-    __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
-    goto __pyx_L0;
-
-    /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":750
- * 
- * cdef inline tuple PyDataType_SHAPE(dtype d):
- *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
- *         return <tuple>d.subarray.shape
- *     else:
- */
-  }
-
-  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":753
- *         return <tuple>d.subarray.shape
- *     else:
- *         return ()             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  /*else*/ {
-    __Pyx_XDECREF(__pyx_r);
-    __Pyx_INCREF(__pyx_empty_tuple);
-    __pyx_r = __pyx_empty_tuple;
-    goto __pyx_L0;
-  }
-
-  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":749
- *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
- * 
- * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
- *     if PyDataType_HASSUBARRAY(d):
- *         return <tuple>d.subarray.shape
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":928
- *     int _import_umath() except -1
- * 
- * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
- *     Py_INCREF(base) # important to do this before stealing the reference below!
- *     PyArray_SetBaseObject(arr, base)
- */
-
-static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("set_array_base", 0);
-
-  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":929
- * 
- * cdef inline void set_array_base(ndarray arr, object base):
- *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
- *     PyArray_SetBaseObject(arr, base)
- * 
- */
-  Py_INCREF(__pyx_v_base);
-
-  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":930
- * cdef inline void set_array_base(ndarray arr, object base):
- *     Py_INCREF(base) # important to do this before stealing the reference below!
- *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
- * 
- * cdef inline object get_array_base(ndarray arr):
- */
-  (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
-
-  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":928
- *     int _import_umath() except -1
- * 
- * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
- *     Py_INCREF(base) # important to do this before stealing the reference below!
- *     PyArray_SetBaseObject(arr, base)
- */
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-}
-
-/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":932
- *     PyArray_SetBaseObject(arr, base)
- * 
- * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
- *     base = PyArray_BASE(arr)
- *     if base is NULL:
- */
-
-static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
-  PyObject *__pyx_v_base;
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  __Pyx_RefNannySetupContext("get_array_base", 0);
-
-  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":933
- * 
- * cdef inline object get_array_base(ndarray arr):
- *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
- *     if base is NULL:
- *         return None
- */
-  __pyx_v_base = PyArray_BASE(__pyx_v_arr);
-
-  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":934
- * cdef inline object get_array_base(ndarray arr):
- *     base = PyArray_BASE(arr)
- *     if base is NULL:             # <<<<<<<<<<<<<<
- *         return None
- *     return <object>base
- */
-  __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
-  if (__pyx_t_1) {
-
-    /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":935
- *     base = PyArray_BASE(arr)
- *     if base is NULL:
- *         return None             # <<<<<<<<<<<<<<
- *     return <object>base
- * 
- */
-    __Pyx_XDECREF(__pyx_r);
-    __pyx_r = Py_None; __Pyx_INCREF(Py_None);
-    goto __pyx_L0;
-
-    /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":934
- * cdef inline object get_array_base(ndarray arr):
- *     base = PyArray_BASE(arr)
- *     if base is NULL:             # <<<<<<<<<<<<<<
- *         return None
- *     return <object>base
- */
-  }
-
-  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":936
- *     if base is NULL:
- *         return None
- *     return <object>base             # <<<<<<<<<<<<<<
- * 
- * # Versions of the import_* functions which are more suitable for
- */
-  __Pyx_XDECREF(__pyx_r);
-  __Pyx_INCREF(((PyObject *)__pyx_v_base));
-  __pyx_r = ((PyObject *)__pyx_v_base);
-  goto __pyx_L0;
-
-  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":932
- *     PyArray_SetBaseObject(arr, base)
- * 
- * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
- *     base = PyArray_BASE(arr)
- *     if base is NULL:
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":940
- * # Versions of the import_* functions which are more suitable for
- * # Cython code.
- * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
- *     try:
- *         __pyx_import_array()
- */
-
-static CYTHON_INLINE int __pyx_f_5numpy_import_array(void) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
-  int __pyx_t_4;
-  PyObject *__pyx_t_5 = NULL;
-  PyObject *__pyx_t_6 = NULL;
-  PyObject *__pyx_t_7 = NULL;
-  PyObject *__pyx_t_8 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("import_array", 0);
-
-  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":941
- * # Cython code.
- * cdef inline int import_array() except -1:
- *     try:             # <<<<<<<<<<<<<<
- *         __pyx_import_array()
- *     except Exception:
- */
-  {
-    __Pyx_PyThreadState_declare
-    __Pyx_PyThreadState_assign
-    __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
-    __Pyx_XGOTREF(__pyx_t_1);
-    __Pyx_XGOTREF(__pyx_t_2);
-    __Pyx_XGOTREF(__pyx_t_3);
-    /*try:*/ {
-
-      /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":942
- * cdef inline int import_array() except -1:
- *     try:
- *         __pyx_import_array()             # <<<<<<<<<<<<<<
- *     except Exception:
- *         raise ImportError("numpy.core.multiarray failed to import")
- */
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 942, __pyx_L3_error)
-
-      /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":941
- * # Cython code.
- * cdef inline int import_array() except -1:
- *     try:             # <<<<<<<<<<<<<<
- *         __pyx_import_array()
- *     except Exception:
- */
-    }
-    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    goto __pyx_L8_try_end;
-    __pyx_L3_error:;
-
-    /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":943
- *     try:
- *         __pyx_import_array()
- *     except Exception:             # <<<<<<<<<<<<<<
- *         raise ImportError("numpy.core.multiarray failed to import")
- * 
- */
-    __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
-    if (__pyx_t_4) {
-      __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 943, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_5);
-      __Pyx_GOTREF(__pyx_t_6);
-      __Pyx_GOTREF(__pyx_t_7);
-
-      /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":944
- *         __pyx_import_array()
- *     except Exception:
- *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
- * 
- * cdef inline int import_umath() except -1:
- */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 944, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_Raise(__pyx_t_8, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 944, __pyx_L5_except_error)
-    }
-    goto __pyx_L5_except_error;
-    __pyx_L5_except_error:;
-
-    /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":941
- * # Cython code.
- * cdef inline int import_array() except -1:
- *     try:             # <<<<<<<<<<<<<<
- *         __pyx_import_array()
- *     except Exception:
- */
-    __Pyx_XGIVEREF(__pyx_t_1);
-    __Pyx_XGIVEREF(__pyx_t_2);
-    __Pyx_XGIVEREF(__pyx_t_3);
-    __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
-    goto __pyx_L1_error;
-    __pyx_L8_try_end:;
-  }
-
-  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":940
- * # Versions of the import_* functions which are more suitable for
- * # Cython code.
- * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
- *     try:
- *         __pyx_import_array()
- */
-
-  /* function exit code */
-  __pyx_r = 0;
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_XDECREF(__pyx_t_8);
-  __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = -1;
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":946
- *         raise ImportError("numpy.core.multiarray failed to import")
- * 
- * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
- *     try:
- *         _import_umath()
- */
-
-static CYTHON_INLINE int __pyx_f_5numpy_import_umath(void) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
-  int __pyx_t_4;
-  PyObject *__pyx_t_5 = NULL;
-  PyObject *__pyx_t_6 = NULL;
-  PyObject *__pyx_t_7 = NULL;
-  PyObject *__pyx_t_8 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("import_umath", 0);
-
-  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":947
- * 
- * cdef inline int import_umath() except -1:
- *     try:             # <<<<<<<<<<<<<<
- *         _import_umath()
- *     except Exception:
- */
-  {
-    __Pyx_PyThreadState_declare
-    __Pyx_PyThreadState_assign
-    __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
-    __Pyx_XGOTREF(__pyx_t_1);
-    __Pyx_XGOTREF(__pyx_t_2);
-    __Pyx_XGOTREF(__pyx_t_3);
-    /*try:*/ {
-
-      /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":948
- * cdef inline int import_umath() except -1:
- *     try:
- *         _import_umath()             # <<<<<<<<<<<<<<
- *     except Exception:
- *         raise ImportError("numpy.core.umath failed to import")
- */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 948, __pyx_L3_error)
-
-      /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":947
- * 
- * cdef inline int import_umath() except -1:
- *     try:             # <<<<<<<<<<<<<<
- *         _import_umath()
- *     except Exception:
- */
-    }
-    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    goto __pyx_L8_try_end;
-    __pyx_L3_error:;
-
-    /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":949
- *     try:
- *         _import_umath()
- *     except Exception:             # <<<<<<<<<<<<<<
- *         raise ImportError("numpy.core.umath failed to import")
- * 
- */
-    __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
-    if (__pyx_t_4) {
-      __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 949, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_5);
-      __Pyx_GOTREF(__pyx_t_6);
-      __Pyx_GOTREF(__pyx_t_7);
-
-      /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":950
- *         _import_umath()
- *     except Exception:
- *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
- * 
- * cdef inline int import_ufunc() except -1:
- */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 950, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_Raise(__pyx_t_8, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 950, __pyx_L5_except_error)
-    }
-    goto __pyx_L5_except_error;
-    __pyx_L5_except_error:;
-
-    /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":947
- * 
- * cdef inline int import_umath() except -1:
- *     try:             # <<<<<<<<<<<<<<
- *         _import_umath()
- *     except Exception:
- */
-    __Pyx_XGIVEREF(__pyx_t_1);
-    __Pyx_XGIVEREF(__pyx_t_2);
-    __Pyx_XGIVEREF(__pyx_t_3);
-    __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
-    goto __pyx_L1_error;
-    __pyx_L8_try_end:;
-  }
-
-  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":946
- *         raise ImportError("numpy.core.multiarray failed to import")
- * 
- * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
- *     try:
- *         _import_umath()
- */
-
-  /* function exit code */
-  __pyx_r = 0;
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_XDECREF(__pyx_t_8);
-  __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = -1;
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":952
- *         raise ImportError("numpy.core.umath failed to import")
- * 
- * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
- *     try:
- *         _import_umath()
- */
-
-static CYTHON_INLINE int __pyx_f_5numpy_import_ufunc(void) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
-  int __pyx_t_4;
-  PyObject *__pyx_t_5 = NULL;
-  PyObject *__pyx_t_6 = NULL;
-  PyObject *__pyx_t_7 = NULL;
-  PyObject *__pyx_t_8 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("import_ufunc", 0);
-
-  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":953
- * 
- * cdef inline int import_ufunc() except -1:
- *     try:             # <<<<<<<<<<<<<<
- *         _import_umath()
- *     except Exception:
- */
-  {
-    __Pyx_PyThreadState_declare
-    __Pyx_PyThreadState_assign
-    __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
-    __Pyx_XGOTREF(__pyx_t_1);
-    __Pyx_XGOTREF(__pyx_t_2);
-    __Pyx_XGOTREF(__pyx_t_3);
-    /*try:*/ {
-
-      /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":954
- * cdef inline int import_ufunc() except -1:
- *     try:
- *         _import_umath()             # <<<<<<<<<<<<<<
- *     except Exception:
- *         raise ImportError("numpy.core.umath failed to import")
- */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 954, __pyx_L3_error)
-
-      /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":953
- * 
- * cdef inline int import_ufunc() except -1:
- *     try:             # <<<<<<<<<<<<<<
- *         _import_umath()
- *     except Exception:
- */
-    }
-    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    goto __pyx_L8_try_end;
-    __pyx_L3_error:;
-
-    /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":955
- *     try:
- *         _import_umath()
- *     except Exception:             # <<<<<<<<<<<<<<
- *         raise ImportError("numpy.core.umath failed to import")
- * 
- */
-    __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
-    if (__pyx_t_4) {
-      __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 955, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_5);
-      __Pyx_GOTREF(__pyx_t_6);
-      __Pyx_GOTREF(__pyx_t_7);
-
-      /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":956
- *         _import_umath()
- *     except Exception:
- *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
- * 
- * cdef extern from *:
- */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 956, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_Raise(__pyx_t_8, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 956, __pyx_L5_except_error)
-    }
-    goto __pyx_L5_except_error;
-    __pyx_L5_except_error:;
-
-    /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":953
- * 
- * cdef inline int import_ufunc() except -1:
- *     try:             # <<<<<<<<<<<<<<
- *         _import_umath()
- *     except Exception:
- */
-    __Pyx_XGIVEREF(__pyx_t_1);
-    __Pyx_XGIVEREF(__pyx_t_2);
-    __Pyx_XGIVEREF(__pyx_t_3);
-    __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
-    goto __pyx_L1_error;
-    __pyx_L8_try_end:;
-  }
-
-  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":952
- *         raise ImportError("numpy.core.umath failed to import")
- * 
- * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
- *     try:
- *         _import_umath()
- */
-
-  /* function exit code */
-  __pyx_r = 0;
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_XDECREF(__pyx_t_8);
-  __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = -1;
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":966
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
-  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":978
- *     bool
- *     """
- *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
-  goto __pyx_L0;
-
-  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":966
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
-/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":981
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
-  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":993
- *     bool
- *     """
- *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
-  goto __pyx_L0;
-
-  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":981
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
-/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":996
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
-  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":1003
- *     also needed.  That can be found using `get_datetime64_unit`.
- *     """
- *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
-  goto __pyx_L0;
-
-  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":996
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
-/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":1006
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
-  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":1010
- *     returns the int64 value underlying scalar numpy timedelta64 object
- *     """
- *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
-  goto __pyx_L0;
-
-  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":1006
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
-/* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":1013
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
-  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":1017
- *     returns the unit part of the dtype for a numpy datetime64 object.
- *     """
- *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
- */
-  __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
-  goto __pyx_L0;
-
-  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":1013
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
-/* "string.to_py":31
- * 
- * @cname("__pyx_convert_PyObject_string_to_py_std__in_string")
- * cdef inline object __pyx_convert_PyObject_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
- *     return __Pyx_PyObject_FromStringAndSize(s.data(), s.size())
- * cdef extern from *:
- */
-
-static CYTHON_INLINE PyObject *__pyx_convert_PyObject_string_to_py_std__in_string(std::string const &__pyx_v_s) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_convert_PyObject_string_to_py_std__in_string", 0);
-
-  /* "string.to_py":32
- * @cname("__pyx_convert_PyObject_string_to_py_std__in_string")
- * cdef inline object __pyx_convert_PyObject_string_to_py_std__in_string(const string& s):
- *     return __Pyx_PyObject_FromStringAndSize(s.data(), s.size())             # <<<<<<<<<<<<<<
- * cdef extern from *:
- *     cdef object __Pyx_PyUnicode_FromStringAndSize(const char*, size_t)
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_FromStringAndSize(__pyx_v_s.data(), __pyx_v_s.size()); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 32, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "string.to_py":31
- * 
- * @cname("__pyx_convert_PyObject_string_to_py_std__in_string")
- * cdef inline object __pyx_convert_PyObject_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
- *     return __Pyx_PyObject_FromStringAndSize(s.data(), s.size())
- * cdef extern from *:
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("string.to_py.__pyx_convert_PyObject_string_to_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "string.to_py":37
- * 
- * @cname("__pyx_convert_PyUnicode_string_to_py_std__in_string")
- * cdef inline object __pyx_convert_PyUnicode_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
- *     return __Pyx_PyUnicode_FromStringAndSize(s.data(), s.size())
- * cdef extern from *:
- */
-
-static CYTHON_INLINE PyObject *__pyx_convert_PyUnicode_string_to_py_std__in_string(std::string const &__pyx_v_s) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_convert_PyUnicode_string_to_py_std__in_string", 0);
-
-  /* "string.to_py":38
- * @cname("__pyx_convert_PyUnicode_string_to_py_std__in_string")
- * cdef inline object __pyx_convert_PyUnicode_string_to_py_std__in_string(const string& s):
- *     return __Pyx_PyUnicode_FromStringAndSize(s.data(), s.size())             # <<<<<<<<<<<<<<
- * cdef extern from *:
- *     cdef object __Pyx_PyStr_FromStringAndSize(const char*, size_t)
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyUnicode_FromStringAndSize(__pyx_v_s.data(), __pyx_v_s.size()); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 38, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "string.to_py":37
- * 
- * @cname("__pyx_convert_PyUnicode_string_to_py_std__in_string")
- * cdef inline object __pyx_convert_PyUnicode_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
- *     return __Pyx_PyUnicode_FromStringAndSize(s.data(), s.size())
- * cdef extern from *:
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("string.to_py.__pyx_convert_PyUnicode_string_to_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "string.to_py":43
- * 
- * @cname("__pyx_convert_PyStr_string_to_py_std__in_string")
- * cdef inline object __pyx_convert_PyStr_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
- *     return __Pyx_PyStr_FromStringAndSize(s.data(), s.size())
- * cdef extern from *:
- */
-
-static CYTHON_INLINE PyObject *__pyx_convert_PyStr_string_to_py_std__in_string(std::string const &__pyx_v_s) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_convert_PyStr_string_to_py_std__in_string", 0);
-
-  /* "string.to_py":44
- * @cname("__pyx_convert_PyStr_string_to_py_std__in_string")
- * cdef inline object __pyx_convert_PyStr_string_to_py_std__in_string(const string& s):
- *     return __Pyx_PyStr_FromStringAndSize(s.data(), s.size())             # <<<<<<<<<<<<<<
- * cdef extern from *:
- *     cdef object __Pyx_PyBytes_FromStringAndSize(const char*, size_t)
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyStr_FromStringAndSize(__pyx_v_s.data(), __pyx_v_s.size()); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 44, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "string.to_py":43
- * 
- * @cname("__pyx_convert_PyStr_string_to_py_std__in_string")
- * cdef inline object __pyx_convert_PyStr_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
- *     return __Pyx_PyStr_FromStringAndSize(s.data(), s.size())
- * cdef extern from *:
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("string.to_py.__pyx_convert_PyStr_string_to_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "string.to_py":49
- * 
- * @cname("__pyx_convert_PyBytes_string_to_py_std__in_string")
- * cdef inline object __pyx_convert_PyBytes_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
- *     return __Pyx_PyBytes_FromStringAndSize(s.data(), s.size())
- * cdef extern from *:
- */
-
-static CYTHON_INLINE PyObject *__pyx_convert_PyBytes_string_to_py_std__in_string(std::string const &__pyx_v_s) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_convert_PyBytes_string_to_py_std__in_string", 0);
-
-  /* "string.to_py":50
- * @cname("__pyx_convert_PyBytes_string_to_py_std__in_string")
- * cdef inline object __pyx_convert_PyBytes_string_to_py_std__in_string(const string& s):
- *     return __Pyx_PyBytes_FromStringAndSize(s.data(), s.size())             # <<<<<<<<<<<<<<
- * cdef extern from *:
- *     cdef object __Pyx_PyByteArray_FromStringAndSize(const char*, size_t)
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_s.data(), __pyx_v_s.size()); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 50, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "string.to_py":49
- * 
- * @cname("__pyx_convert_PyBytes_string_to_py_std__in_string")
- * cdef inline object __pyx_convert_PyBytes_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
- *     return __Pyx_PyBytes_FromStringAndSize(s.data(), s.size())
- * cdef extern from *:
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("string.to_py.__pyx_convert_PyBytes_string_to_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "string.to_py":55
- * 
- * @cname("__pyx_convert_PyByteArray_string_to_py_std__in_string")
- * cdef inline object __pyx_convert_PyByteArray_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
- *     return __Pyx_PyByteArray_FromStringAndSize(s.data(), s.size())
- * 
- */
-
-static CYTHON_INLINE PyObject *__pyx_convert_PyByteArray_string_to_py_std__in_string(std::string const &__pyx_v_s) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_convert_PyByteArray_string_to_py_std__in_string", 0);
-
-  /* "string.to_py":56
- * @cname("__pyx_convert_PyByteArray_string_to_py_std__in_string")
- * cdef inline object __pyx_convert_PyByteArray_string_to_py_std__in_string(const string& s):
- *     return __Pyx_PyByteArray_FromStringAndSize(s.data(), s.size())             # <<<<<<<<<<<<<<
- * 
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyByteArray_FromStringAndSize(__pyx_v_s.data(), __pyx_v_s.size()); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 56, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "string.to_py":55
- * 
- * @cname("__pyx_convert_PyByteArray_string_to_py_std__in_string")
- * cdef inline object __pyx_convert_PyByteArray_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
- *     return __Pyx_PyByteArray_FromStringAndSize(s.data(), s.size())
- * 
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("string.to_py.__pyx_convert_PyByteArray_string_to_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
-
-#if PY_MAJOR_VERSION >= 3
-#if CYTHON_PEP489_MULTI_PHASE_INIT
-static PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def); /*proto*/
-static int __pyx_pymod_exec_wrapper(PyObject* module); /*proto*/
-static PyModuleDef_Slot __pyx_moduledef_slots[] = {
-  {Py_mod_create, (void*)__pyx_pymod_create},
-  {Py_mod_exec, (void*)__pyx_pymod_exec_wrapper},
-  {0, NULL}
-};
-#endif
-
-static struct PyModuleDef __pyx_moduledef = {
-    PyModuleDef_HEAD_INIT,
-    "wrapper",
-    0, /* m_doc */
-  #if CYTHON_PEP489_MULTI_PHASE_INIT
-    0, /* m_size */
-  #else
-    -1, /* m_size */
-  #endif
-    __pyx_methods /* m_methods */,
-  #if CYTHON_PEP489_MULTI_PHASE_INIT
-    __pyx_moduledef_slots, /* m_slots */
-  #else
-    NULL, /* m_reload */
-  #endif
-    NULL, /* m_traverse */
-    NULL, /* m_clear */
-    NULL /* m_free */
-};
-#endif
 #ifndef CYTHON_SMALL_CODE
 #if defined(__clang__)
     #define CYTHON_SMALL_CODE
 #elif defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 3))
     #define CYTHON_SMALL_CODE __attribute__((cold))
 #else
     #define CYTHON_SMALL_CODE
 #endif
 #endif
+/* #### Code section: pystring_table ### */
 
-static __Pyx_StringTabEntry __pyx_string_tab[] = {
-  {&__pyx_n_u_C_CONTIGUOUS, __pyx_k_C_CONTIGUOUS, sizeof(__pyx_k_C_CONTIGUOUS), 0, 1, 0, 1},
-  {&__pyx_n_s_ImportError, __pyx_k_ImportError, sizeof(__pyx_k_ImportError), 0, 0, 1, 1},
-  {&__pyx_n_s_allow_negative_pixels, __pyx_k_allow_negative_pixels, sizeof(__pyx_k_allow_negative_pixels), 0, 0, 1, 1},
-  {&__pyx_n_s_arcticpy_wrapper, __pyx_k_arcticpy_wrapper, sizeof(__pyx_k_arcticpy_wrapper), 0, 0, 1, 1},
-  {&__pyx_n_s_array, __pyx_k_array, sizeof(__pyx_k_array), 0, 0, 1, 1},
-  {&__pyx_n_s_ascontiguousarray, __pyx_k_ascontiguousarray, sizeof(__pyx_k_ascontiguousarray), 0, 0, 1, 1},
-  {&__pyx_n_s_check_contiguous, __pyx_k_check_contiguous, sizeof(__pyx_k_check_contiguous), 0, 0, 1, 1},
-  {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
-  {&__pyx_n_s_cy_add_cti, __pyx_k_cy_add_cti, sizeof(__pyx_k_cy_add_cti), 0, 0, 1, 1},
-  {&__pyx_n_s_cy_print_array, __pyx_k_cy_print_array, sizeof(__pyx_k_cy_print_array), 0, 0, 1, 1},
-  {&__pyx_n_s_cy_print_array_2D, __pyx_k_cy_print_array_2D, sizeof(__pyx_k_cy_print_array_2D), 0, 0, 1, 1},
-  {&__pyx_n_s_cy_print_version, __pyx_k_cy_print_version, sizeof(__pyx_k_cy_print_version), 0, 0, 1, 1},
-  {&__pyx_n_s_cy_version_arctic, __pyx_k_cy_version_arctic, sizeof(__pyx_k_cy_version_arctic), 0, 0, 1, 1},
-  {&__pyx_n_s_flags, __pyx_k_flags, sizeof(__pyx_k_flags), 0, 0, 1, 1},
-  {&__pyx_n_s_image, __pyx_k_image, sizeof(__pyx_k_image), 0, 0, 1, 1},
-  {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
-  {&__pyx_n_s_iteration, __pyx_k_iteration, sizeof(__pyx_k_iteration), 0, 0, 1, 1},
-  {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
-  {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
-  {&__pyx_n_s_np, __pyx_k_np, sizeof(__pyx_k_np), 0, 0, 1, 1},
-  {&__pyx_n_s_numpy, __pyx_k_numpy, sizeof(__pyx_k_numpy), 0, 0, 1, 1},
-  {&__pyx_kp_u_numpy_core_multiarray_failed_to, __pyx_k_numpy_core_multiarray_failed_to, sizeof(__pyx_k_numpy_core_multiarray_failed_to), 0, 1, 0, 0},
-  {&__pyx_kp_u_numpy_core_umath_failed_to_impor, __pyx_k_numpy_core_umath_failed_to_impor, sizeof(__pyx_k_numpy_core_umath_failed_to_impor), 0, 1, 0, 0},
-  {&__pyx_n_s_parallel_dwell_times, __pyx_k_parallel_dwell_times, sizeof(__pyx_k_parallel_dwell_times), 0, 0, 1, 1},
-  {&__pyx_n_s_parallel_empty_traps_between_col, __pyx_k_parallel_empty_traps_between_col, sizeof(__pyx_k_parallel_empty_traps_between_col), 0, 0, 1, 1},
-  {&__pyx_n_s_parallel_empty_traps_for_first_t, __pyx_k_parallel_empty_traps_for_first_t, sizeof(__pyx_k_parallel_empty_traps_for_first_t), 0, 0, 1, 1},
-  {&__pyx_n_s_parallel_express, __pyx_k_parallel_express, sizeof(__pyx_k_parallel_express), 0, 0, 1, 1},
-  {&__pyx_n_s_parallel_first_electron_fills, __pyx_k_parallel_first_electron_fills, sizeof(__pyx_k_parallel_first_electron_fills), 0, 0, 1, 1},
-  {&__pyx_n_s_parallel_force_release_away_from, __pyx_k_parallel_force_release_away_from, sizeof(__pyx_k_parallel_force_release_away_from), 0, 0, 1, 1},
-  {&__pyx_n_s_parallel_fraction_of_traps_per_p, __pyx_k_parallel_fraction_of_traps_per_p, sizeof(__pyx_k_parallel_fraction_of_traps_per_p), 0, 0, 1, 1},
-  {&__pyx_n_s_parallel_full_well_depths, __pyx_k_parallel_full_well_depths, sizeof(__pyx_k_parallel_full_well_depths), 0, 0, 1, 1},
-  {&__pyx_n_s_parallel_n_pumps, __pyx_k_parallel_n_pumps, sizeof(__pyx_k_parallel_n_pumps), 0, 0, 1, 1},
-  {&__pyx_n_s_parallel_n_traps_ic, __pyx_k_parallel_n_traps_ic, sizeof(__pyx_k_parallel_n_traps_ic), 0, 0, 1, 1},
-  {&__pyx_n_s_parallel_n_traps_ic_co, __pyx_k_parallel_n_traps_ic_co, sizeof(__pyx_k_parallel_n_traps_ic_co), 0, 0, 1, 1},
-  {&__pyx_n_s_parallel_n_traps_sc, __pyx_k_parallel_n_traps_sc, sizeof(__pyx_k_parallel_n_traps_sc), 0, 0, 1, 1},
-  {&__pyx_n_s_parallel_n_traps_sc_co, __pyx_k_parallel_n_traps_sc_co, sizeof(__pyx_k_parallel_n_traps_sc_co), 0, 0, 1, 1},
-  {&__pyx_n_s_parallel_overscan_start, __pyx_k_parallel_overscan_start, sizeof(__pyx_k_parallel_overscan_start), 0, 0, 1, 1},
-  {&__pyx_n_s_parallel_prescan_offset, __pyx_k_parallel_prescan_offset, sizeof(__pyx_k_parallel_prescan_offset), 0, 0, 1, 1},
-  {&__pyx_n_s_parallel_prune_frequency, __pyx_k_parallel_prune_frequency, sizeof(__pyx_k_parallel_prune_frequency), 0, 0, 1, 1},
-  {&__pyx_n_s_parallel_prune_n_electrons, __pyx_k_parallel_prune_n_electrons, sizeof(__pyx_k_parallel_prune_n_electrons), 0, 0, 1, 1},
-  {&__pyx_n_s_parallel_roe_type, __pyx_k_parallel_roe_type, sizeof(__pyx_k_parallel_roe_type), 0, 0, 1, 1},
-  {&__pyx_n_s_parallel_time_start, __pyx_k_parallel_time_start, sizeof(__pyx_k_parallel_time_start), 0, 0, 1, 1},
-  {&__pyx_n_s_parallel_time_stop, __pyx_k_parallel_time_stop, sizeof(__pyx_k_parallel_time_stop), 0, 0, 1, 1},
-  {&__pyx_n_s_parallel_trap_densities, __pyx_k_parallel_trap_densities, sizeof(__pyx_k_parallel_trap_densities), 0, 0, 1, 1},
-  {&__pyx_n_s_parallel_trap_fourth_params, __pyx_k_parallel_trap_fourth_params, sizeof(__pyx_k_parallel_trap_fourth_params), 0, 0, 1, 1},
-  {&__pyx_n_s_parallel_trap_release_timescales, __pyx_k_parallel_trap_release_timescales, sizeof(__pyx_k_parallel_trap_release_timescales), 0, 0, 1, 1},
-  {&__pyx_n_s_parallel_trap_third_params, __pyx_k_parallel_trap_third_params, sizeof(__pyx_k_parallel_trap_third_params), 0, 0, 1, 1},
-  {&__pyx_n_s_parallel_use_integer_express_mat, __pyx_k_parallel_use_integer_express_mat, sizeof(__pyx_k_parallel_use_integer_express_mat), 0, 0, 1, 1},
-  {&__pyx_n_s_parallel_well_fill_powers, __pyx_k_parallel_well_fill_powers, sizeof(__pyx_k_parallel_well_fill_powers), 0, 0, 1, 1},
-  {&__pyx_n_s_parallel_well_notch_depths, __pyx_k_parallel_well_notch_depths, sizeof(__pyx_k_parallel_well_notch_depths), 0, 0, 1, 1},
-  {&__pyx_n_s_parallel_window_offset, __pyx_k_parallel_window_offset, sizeof(__pyx_k_parallel_window_offset), 0, 0, 1, 1},
-  {&__pyx_n_s_parallel_window_start, __pyx_k_parallel_window_start, sizeof(__pyx_k_parallel_window_start), 0, 0, 1, 1},
-  {&__pyx_n_s_parallel_window_stop, __pyx_k_parallel_window_stop, sizeof(__pyx_k_parallel_window_stop), 0, 0, 1, 1},
-  {&__pyx_kp_s_python_arcticpy_wrapper_pyx, __pyx_k_python_arcticpy_wrapper_pyx, sizeof(__pyx_k_python_arcticpy_wrapper_pyx), 0, 0, 1, 0},
-  {&__pyx_n_s_serial_dwell_times, __pyx_k_serial_dwell_times, sizeof(__pyx_k_serial_dwell_times), 0, 0, 1, 1},
-  {&__pyx_n_s_serial_empty_traps_between_colum, __pyx_k_serial_empty_traps_between_colum, sizeof(__pyx_k_serial_empty_traps_between_colum), 0, 0, 1, 1},
-  {&__pyx_n_s_serial_empty_traps_for_first_tra, __pyx_k_serial_empty_traps_for_first_tra, sizeof(__pyx_k_serial_empty_traps_for_first_tra), 0, 0, 1, 1},
-  {&__pyx_n_s_serial_express, __pyx_k_serial_express, sizeof(__pyx_k_serial_express), 0, 0, 1, 1},
-  {&__pyx_n_s_serial_first_electron_fills, __pyx_k_serial_first_electron_fills, sizeof(__pyx_k_serial_first_electron_fills), 0, 0, 1, 1},
-  {&__pyx_n_s_serial_force_release_away_from_r, __pyx_k_serial_force_release_away_from_r, sizeof(__pyx_k_serial_force_release_away_from_r), 0, 0, 1, 1},
-  {&__pyx_n_s_serial_fraction_of_traps_per_pha, __pyx_k_serial_fraction_of_traps_per_pha, sizeof(__pyx_k_serial_fraction_of_traps_per_pha), 0, 0, 1, 1},
-  {&__pyx_n_s_serial_full_well_depths, __pyx_k_serial_full_well_depths, sizeof(__pyx_k_serial_full_well_depths), 0, 0, 1, 1},
-  {&__pyx_n_s_serial_n_pumps, __pyx_k_serial_n_pumps, sizeof(__pyx_k_serial_n_pumps), 0, 0, 1, 1},
-  {&__pyx_n_s_serial_n_traps_ic, __pyx_k_serial_n_traps_ic, sizeof(__pyx_k_serial_n_traps_ic), 0, 0, 1, 1},
-  {&__pyx_n_s_serial_n_traps_ic_co, __pyx_k_serial_n_traps_ic_co, sizeof(__pyx_k_serial_n_traps_ic_co), 0, 0, 1, 1},
-  {&__pyx_n_s_serial_n_traps_sc, __pyx_k_serial_n_traps_sc, sizeof(__pyx_k_serial_n_traps_sc), 0, 0, 1, 1},
-  {&__pyx_n_s_serial_n_traps_sc_co, __pyx_k_serial_n_traps_sc_co, sizeof(__pyx_k_serial_n_traps_sc_co), 0, 0, 1, 1},
-  {&__pyx_n_s_serial_overscan_start, __pyx_k_serial_overscan_start, sizeof(__pyx_k_serial_overscan_start), 0, 0, 1, 1},
-  {&__pyx_n_s_serial_prescan_offset, __pyx_k_serial_prescan_offset, sizeof(__pyx_k_serial_prescan_offset), 0, 0, 1, 1},
-  {&__pyx_n_s_serial_prune_frequency, __pyx_k_serial_prune_frequency, sizeof(__pyx_k_serial_prune_frequency), 0, 0, 1, 1},
-  {&__pyx_n_s_serial_prune_n_electrons, __pyx_k_serial_prune_n_electrons, sizeof(__pyx_k_serial_prune_n_electrons), 0, 0, 1, 1},
-  {&__pyx_n_s_serial_roe_type, __pyx_k_serial_roe_type, sizeof(__pyx_k_serial_roe_type), 0, 0, 1, 1},
-  {&__pyx_n_s_serial_time_start, __pyx_k_serial_time_start, sizeof(__pyx_k_serial_time_start), 0, 0, 1, 1},
-  {&__pyx_n_s_serial_time_stop, __pyx_k_serial_time_stop, sizeof(__pyx_k_serial_time_stop), 0, 0, 1, 1},
-  {&__pyx_n_s_serial_trap_densities, __pyx_k_serial_trap_densities, sizeof(__pyx_k_serial_trap_densities), 0, 0, 1, 1},
-  {&__pyx_n_s_serial_trap_fourth_params, __pyx_k_serial_trap_fourth_params, sizeof(__pyx_k_serial_trap_fourth_params), 0, 0, 1, 1},
-  {&__pyx_n_s_serial_trap_release_timescales, __pyx_k_serial_trap_release_timescales, sizeof(__pyx_k_serial_trap_release_timescales), 0, 0, 1, 1},
-  {&__pyx_n_s_serial_trap_third_params, __pyx_k_serial_trap_third_params, sizeof(__pyx_k_serial_trap_third_params), 0, 0, 1, 1},
-  {&__pyx_n_s_serial_use_integer_express_matri, __pyx_k_serial_use_integer_express_matri, sizeof(__pyx_k_serial_use_integer_express_matri), 0, 0, 1, 1},
-  {&__pyx_n_s_serial_well_fill_powers, __pyx_k_serial_well_fill_powers, sizeof(__pyx_k_serial_well_fill_powers), 0, 0, 1, 1},
-  {&__pyx_n_s_serial_well_notch_depths, __pyx_k_serial_well_notch_depths, sizeof(__pyx_k_serial_well_notch_depths), 0, 0, 1, 1},
-  {&__pyx_n_s_serial_window_offset, __pyx_k_serial_window_offset, sizeof(__pyx_k_serial_window_offset), 0, 0, 1, 1},
-  {&__pyx_n_s_serial_window_start, __pyx_k_serial_window_start, sizeof(__pyx_k_serial_window_start), 0, 0, 1, 1},
-  {&__pyx_n_s_serial_window_stop, __pyx_k_serial_window_stop, sizeof(__pyx_k_serial_window_stop), 0, 0, 1, 1},
-  {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
-  {&__pyx_n_s_verbosity, __pyx_k_verbosity, sizeof(__pyx_k_verbosity), 0, 0, 1, 1},
-  {0, 0, 0, 0, 0, 0, 0}
-};
+static int __Pyx_CreateStringTabAndInitStrings(void) {
+  __Pyx_StringTabEntry __pyx_string_tab[] = {
+    {&__pyx_n_u_C_CONTIGUOUS, __pyx_k_C_CONTIGUOUS, sizeof(__pyx_k_C_CONTIGUOUS), 0, 1, 0, 1},
+    {&__pyx_n_s_ImportError, __pyx_k_ImportError, sizeof(__pyx_k_ImportError), 0, 0, 1, 1},
+    {&__pyx_n_s__12, __pyx_k__12, sizeof(__pyx_k__12), 0, 0, 1, 1},
+    {&__pyx_n_s__3, __pyx_k__3, sizeof(__pyx_k__3), 0, 0, 1, 1},
+    {&__pyx_n_s_allow_negative_pixels, __pyx_k_allow_negative_pixels, sizeof(__pyx_k_allow_negative_pixels), 0, 0, 1, 1},
+    {&__pyx_n_s_arcticpy_wrapper, __pyx_k_arcticpy_wrapper, sizeof(__pyx_k_arcticpy_wrapper), 0, 0, 1, 1},
+    {&__pyx_n_s_array, __pyx_k_array, sizeof(__pyx_k_array), 0, 0, 1, 1},
+    {&__pyx_n_s_ascontiguousarray, __pyx_k_ascontiguousarray, sizeof(__pyx_k_ascontiguousarray), 0, 0, 1, 1},
+    {&__pyx_n_s_asyncio_coroutines, __pyx_k_asyncio_coroutines, sizeof(__pyx_k_asyncio_coroutines), 0, 0, 1, 1},
+    {&__pyx_n_s_check_contiguous, __pyx_k_check_contiguous, sizeof(__pyx_k_check_contiguous), 0, 0, 1, 1},
+    {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
+    {&__pyx_n_s_cy_add_cti, __pyx_k_cy_add_cti, sizeof(__pyx_k_cy_add_cti), 0, 0, 1, 1},
+    {&__pyx_n_s_cy_print_array, __pyx_k_cy_print_array, sizeof(__pyx_k_cy_print_array), 0, 0, 1, 1},
+    {&__pyx_n_s_cy_print_array_2D, __pyx_k_cy_print_array_2D, sizeof(__pyx_k_cy_print_array_2D), 0, 0, 1, 1},
+    {&__pyx_n_s_cy_print_version, __pyx_k_cy_print_version, sizeof(__pyx_k_cy_print_version), 0, 0, 1, 1},
+    {&__pyx_n_s_cy_version_arctic, __pyx_k_cy_version_arctic, sizeof(__pyx_k_cy_version_arctic), 0, 0, 1, 1},
+    {&__pyx_n_s_flags, __pyx_k_flags, sizeof(__pyx_k_flags), 0, 0, 1, 1},
+    {&__pyx_n_s_image, __pyx_k_image, sizeof(__pyx_k_image), 0, 0, 1, 1},
+    {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
+    {&__pyx_n_s_initializing, __pyx_k_initializing, sizeof(__pyx_k_initializing), 0, 0, 1, 1},
+    {&__pyx_n_s_is_coroutine, __pyx_k_is_coroutine, sizeof(__pyx_k_is_coroutine), 0, 0, 1, 1},
+    {&__pyx_n_s_iteration, __pyx_k_iteration, sizeof(__pyx_k_iteration), 0, 0, 1, 1},
+    {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
+    {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
+    {&__pyx_n_s_np, __pyx_k_np, sizeof(__pyx_k_np), 0, 0, 1, 1},
+    {&__pyx_n_s_numpy, __pyx_k_numpy, sizeof(__pyx_k_numpy), 0, 0, 1, 1},
+    {&__pyx_kp_u_numpy_core_multiarray_failed_to, __pyx_k_numpy_core_multiarray_failed_to, sizeof(__pyx_k_numpy_core_multiarray_failed_to), 0, 1, 0, 0},
+    {&__pyx_kp_u_numpy_core_umath_failed_to_impor, __pyx_k_numpy_core_umath_failed_to_impor, sizeof(__pyx_k_numpy_core_umath_failed_to_impor), 0, 1, 0, 0},
+    {&__pyx_n_s_parallel_dwell_times, __pyx_k_parallel_dwell_times, sizeof(__pyx_k_parallel_dwell_times), 0, 0, 1, 1},
+    {&__pyx_n_s_parallel_empty_traps_between_col, __pyx_k_parallel_empty_traps_between_col, sizeof(__pyx_k_parallel_empty_traps_between_col), 0, 0, 1, 1},
+    {&__pyx_n_s_parallel_empty_traps_for_first_t, __pyx_k_parallel_empty_traps_for_first_t, sizeof(__pyx_k_parallel_empty_traps_for_first_t), 0, 0, 1, 1},
+    {&__pyx_n_s_parallel_express, __pyx_k_parallel_express, sizeof(__pyx_k_parallel_express), 0, 0, 1, 1},
+    {&__pyx_n_s_parallel_first_electron_fills, __pyx_k_parallel_first_electron_fills, sizeof(__pyx_k_parallel_first_electron_fills), 0, 0, 1, 1},
+    {&__pyx_n_s_parallel_force_release_away_from, __pyx_k_parallel_force_release_away_from, sizeof(__pyx_k_parallel_force_release_away_from), 0, 0, 1, 1},
+    {&__pyx_n_s_parallel_fraction_of_traps_per_p, __pyx_k_parallel_fraction_of_traps_per_p, sizeof(__pyx_k_parallel_fraction_of_traps_per_p), 0, 0, 1, 1},
+    {&__pyx_n_s_parallel_full_well_depths, __pyx_k_parallel_full_well_depths, sizeof(__pyx_k_parallel_full_well_depths), 0, 0, 1, 1},
+    {&__pyx_n_s_parallel_n_pumps, __pyx_k_parallel_n_pumps, sizeof(__pyx_k_parallel_n_pumps), 0, 0, 1, 1},
+    {&__pyx_n_s_parallel_n_traps_ic, __pyx_k_parallel_n_traps_ic, sizeof(__pyx_k_parallel_n_traps_ic), 0, 0, 1, 1},
+    {&__pyx_n_s_parallel_n_traps_ic_co, __pyx_k_parallel_n_traps_ic_co, sizeof(__pyx_k_parallel_n_traps_ic_co), 0, 0, 1, 1},
+    {&__pyx_n_s_parallel_n_traps_sc, __pyx_k_parallel_n_traps_sc, sizeof(__pyx_k_parallel_n_traps_sc), 0, 0, 1, 1},
+    {&__pyx_n_s_parallel_n_traps_sc_co, __pyx_k_parallel_n_traps_sc_co, sizeof(__pyx_k_parallel_n_traps_sc_co), 0, 0, 1, 1},
+    {&__pyx_n_s_parallel_overscan_start, __pyx_k_parallel_overscan_start, sizeof(__pyx_k_parallel_overscan_start), 0, 0, 1, 1},
+    {&__pyx_n_s_parallel_prescan_offset, __pyx_k_parallel_prescan_offset, sizeof(__pyx_k_parallel_prescan_offset), 0, 0, 1, 1},
+    {&__pyx_n_s_parallel_prune_frequency, __pyx_k_parallel_prune_frequency, sizeof(__pyx_k_parallel_prune_frequency), 0, 0, 1, 1},
+    {&__pyx_n_s_parallel_prune_n_electrons, __pyx_k_parallel_prune_n_electrons, sizeof(__pyx_k_parallel_prune_n_electrons), 0, 0, 1, 1},
+    {&__pyx_n_s_parallel_roe_type, __pyx_k_parallel_roe_type, sizeof(__pyx_k_parallel_roe_type), 0, 0, 1, 1},
+    {&__pyx_n_s_parallel_time_start, __pyx_k_parallel_time_start, sizeof(__pyx_k_parallel_time_start), 0, 0, 1, 1},
+    {&__pyx_n_s_parallel_time_stop, __pyx_k_parallel_time_stop, sizeof(__pyx_k_parallel_time_stop), 0, 0, 1, 1},
+    {&__pyx_n_s_parallel_trap_densities, __pyx_k_parallel_trap_densities, sizeof(__pyx_k_parallel_trap_densities), 0, 0, 1, 1},
+    {&__pyx_n_s_parallel_trap_fourth_params, __pyx_k_parallel_trap_fourth_params, sizeof(__pyx_k_parallel_trap_fourth_params), 0, 0, 1, 1},
+    {&__pyx_n_s_parallel_trap_release_timescales, __pyx_k_parallel_trap_release_timescales, sizeof(__pyx_k_parallel_trap_release_timescales), 0, 0, 1, 1},
+    {&__pyx_n_s_parallel_trap_third_params, __pyx_k_parallel_trap_third_params, sizeof(__pyx_k_parallel_trap_third_params), 0, 0, 1, 1},
+    {&__pyx_n_s_parallel_use_integer_express_mat, __pyx_k_parallel_use_integer_express_mat, sizeof(__pyx_k_parallel_use_integer_express_mat), 0, 0, 1, 1},
+    {&__pyx_n_s_parallel_well_fill_powers, __pyx_k_parallel_well_fill_powers, sizeof(__pyx_k_parallel_well_fill_powers), 0, 0, 1, 1},
+    {&__pyx_n_s_parallel_well_notch_depths, __pyx_k_parallel_well_notch_depths, sizeof(__pyx_k_parallel_well_notch_depths), 0, 0, 1, 1},
+    {&__pyx_n_s_parallel_window_offset, __pyx_k_parallel_window_offset, sizeof(__pyx_k_parallel_window_offset), 0, 0, 1, 1},
+    {&__pyx_n_s_parallel_window_start, __pyx_k_parallel_window_start, sizeof(__pyx_k_parallel_window_start), 0, 0, 1, 1},
+    {&__pyx_n_s_parallel_window_stop, __pyx_k_parallel_window_stop, sizeof(__pyx_k_parallel_window_stop), 0, 0, 1, 1},
+    {&__pyx_kp_s_python_arcticpy_wrapper_pyx, __pyx_k_python_arcticpy_wrapper_pyx, sizeof(__pyx_k_python_arcticpy_wrapper_pyx), 0, 0, 1, 0},
+    {&__pyx_n_s_serial_dwell_times, __pyx_k_serial_dwell_times, sizeof(__pyx_k_serial_dwell_times), 0, 0, 1, 1},
+    {&__pyx_n_s_serial_empty_traps_between_colum, __pyx_k_serial_empty_traps_between_colum, sizeof(__pyx_k_serial_empty_traps_between_colum), 0, 0, 1, 1},
+    {&__pyx_n_s_serial_empty_traps_for_first_tra, __pyx_k_serial_empty_traps_for_first_tra, sizeof(__pyx_k_serial_empty_traps_for_first_tra), 0, 0, 1, 1},
+    {&__pyx_n_s_serial_express, __pyx_k_serial_express, sizeof(__pyx_k_serial_express), 0, 0, 1, 1},
+    {&__pyx_n_s_serial_first_electron_fills, __pyx_k_serial_first_electron_fills, sizeof(__pyx_k_serial_first_electron_fills), 0, 0, 1, 1},
+    {&__pyx_n_s_serial_force_release_away_from_r, __pyx_k_serial_force_release_away_from_r, sizeof(__pyx_k_serial_force_release_away_from_r), 0, 0, 1, 1},
+    {&__pyx_n_s_serial_fraction_of_traps_per_pha, __pyx_k_serial_fraction_of_traps_per_pha, sizeof(__pyx_k_serial_fraction_of_traps_per_pha), 0, 0, 1, 1},
+    {&__pyx_n_s_serial_full_well_depths, __pyx_k_serial_full_well_depths, sizeof(__pyx_k_serial_full_well_depths), 0, 0, 1, 1},
+    {&__pyx_n_s_serial_n_pumps, __pyx_k_serial_n_pumps, sizeof(__pyx_k_serial_n_pumps), 0, 0, 1, 1},
+    {&__pyx_n_s_serial_n_traps_ic, __pyx_k_serial_n_traps_ic, sizeof(__pyx_k_serial_n_traps_ic), 0, 0, 1, 1},
+    {&__pyx_n_s_serial_n_traps_ic_co, __pyx_k_serial_n_traps_ic_co, sizeof(__pyx_k_serial_n_traps_ic_co), 0, 0, 1, 1},
+    {&__pyx_n_s_serial_n_traps_sc, __pyx_k_serial_n_traps_sc, sizeof(__pyx_k_serial_n_traps_sc), 0, 0, 1, 1},
+    {&__pyx_n_s_serial_n_traps_sc_co, __pyx_k_serial_n_traps_sc_co, sizeof(__pyx_k_serial_n_traps_sc_co), 0, 0, 1, 1},
+    {&__pyx_n_s_serial_overscan_start, __pyx_k_serial_overscan_start, sizeof(__pyx_k_serial_overscan_start), 0, 0, 1, 1},
+    {&__pyx_n_s_serial_prescan_offset, __pyx_k_serial_prescan_offset, sizeof(__pyx_k_serial_prescan_offset), 0, 0, 1, 1},
+    {&__pyx_n_s_serial_prune_frequency, __pyx_k_serial_prune_frequency, sizeof(__pyx_k_serial_prune_frequency), 0, 0, 1, 1},
+    {&__pyx_n_s_serial_prune_n_electrons, __pyx_k_serial_prune_n_electrons, sizeof(__pyx_k_serial_prune_n_electrons), 0, 0, 1, 1},
+    {&__pyx_n_s_serial_roe_type, __pyx_k_serial_roe_type, sizeof(__pyx_k_serial_roe_type), 0, 0, 1, 1},
+    {&__pyx_n_s_serial_time_start, __pyx_k_serial_time_start, sizeof(__pyx_k_serial_time_start), 0, 0, 1, 1},
+    {&__pyx_n_s_serial_time_stop, __pyx_k_serial_time_stop, sizeof(__pyx_k_serial_time_stop), 0, 0, 1, 1},
+    {&__pyx_n_s_serial_trap_densities, __pyx_k_serial_trap_densities, sizeof(__pyx_k_serial_trap_densities), 0, 0, 1, 1},
+    {&__pyx_n_s_serial_trap_fourth_params, __pyx_k_serial_trap_fourth_params, sizeof(__pyx_k_serial_trap_fourth_params), 0, 0, 1, 1},
+    {&__pyx_n_s_serial_trap_release_timescales, __pyx_k_serial_trap_release_timescales, sizeof(__pyx_k_serial_trap_release_timescales), 0, 0, 1, 1},
+    {&__pyx_n_s_serial_trap_third_params, __pyx_k_serial_trap_third_params, sizeof(__pyx_k_serial_trap_third_params), 0, 0, 1, 1},
+    {&__pyx_n_s_serial_use_integer_express_matri, __pyx_k_serial_use_integer_express_matri, sizeof(__pyx_k_serial_use_integer_express_matri), 0, 0, 1, 1},
+    {&__pyx_n_s_serial_well_fill_powers, __pyx_k_serial_well_fill_powers, sizeof(__pyx_k_serial_well_fill_powers), 0, 0, 1, 1},
+    {&__pyx_n_s_serial_well_notch_depths, __pyx_k_serial_well_notch_depths, sizeof(__pyx_k_serial_well_notch_depths), 0, 0, 1, 1},
+    {&__pyx_n_s_serial_window_offset, __pyx_k_serial_window_offset, sizeof(__pyx_k_serial_window_offset), 0, 0, 1, 1},
+    {&__pyx_n_s_serial_window_start, __pyx_k_serial_window_start, sizeof(__pyx_k_serial_window_start), 0, 0, 1, 1},
+    {&__pyx_n_s_serial_window_stop, __pyx_k_serial_window_stop, sizeof(__pyx_k_serial_window_stop), 0, 0, 1, 1},
+    {&__pyx_n_s_spec, __pyx_k_spec, sizeof(__pyx_k_spec), 0, 0, 1, 1},
+    {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
+    {&__pyx_n_s_verbosity, __pyx_k_verbosity, sizeof(__pyx_k_verbosity), 0, 0, 1, 1},
+    {0, 0, 0, 0, 0, 0, 0}
+  };
+  return __Pyx_InitStrings(__pyx_string_tab);
+}
+/* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 944, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 987, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
+/* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":944
+  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 944, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 987, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.pxd":950
+  /* "../../../../../../../home/jammy/venvs/PyAuto/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 950, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 993, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
   /* "arcticpy/wrapper.pyx":105
  * 
  * 
  * def cy_print_version():             # <<<<<<<<<<<<<<
  *     print_version()
  * 
  */
-  __pyx_codeobj__3 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_python_arcticpy_wrapper_pyx, __pyx_n_s_cy_print_version, 105, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__3)) __PYX_ERR(0, 105, __pyx_L1_error)
+  __pyx_codeobj__4 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_python_arcticpy_wrapper_pyx, __pyx_n_s_cy_print_version, 105, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__4)) __PYX_ERR(2, 105, __pyx_L1_error)
 
   /* "arcticpy/wrapper.pyx":108
  *     print_version()
  * 
  * def cy_version_arctic():             # <<<<<<<<<<<<<<
  *     return version_arctic().decode("utf-8")
  * 
  */
-  __pyx_codeobj__4 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_python_arcticpy_wrapper_pyx, __pyx_n_s_cy_version_arctic, 108, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__4)) __PYX_ERR(0, 108, __pyx_L1_error)
+  __pyx_codeobj__5 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_python_arcticpy_wrapper_pyx, __pyx_n_s_cy_version_arctic, 108, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__5)) __PYX_ERR(2, 108, __pyx_L1_error)
 
   /* "arcticpy/wrapper.pyx":111
  *     return version_arctic().decode("utf-8")
  * 
  * def check_contiguous(array):             # <<<<<<<<<<<<<<
  *     """ Make sure an array is contiguous and C-style. """
  *     if not array.flags['C_CONTIGUOUS']:
  */
-  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_n_s_array); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 111, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__5);
-  __Pyx_GIVEREF(__pyx_tuple__5);
-  __pyx_codeobj__6 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__5, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_python_arcticpy_wrapper_pyx, __pyx_n_s_check_contiguous, 111, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__6)) __PYX_ERR(0, 111, __pyx_L1_error)
+  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_n_s_array); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(2, 111, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__6);
+  __Pyx_GIVEREF(__pyx_tuple__6);
+  __pyx_codeobj__7 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_python_arcticpy_wrapper_pyx, __pyx_n_s_check_contiguous, 111, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__7)) __PYX_ERR(2, 111, __pyx_L1_error)
 
   /* "arcticpy/wrapper.pyx":119
  * 
  * 
  * def cy_print_array(np.ndarray[np.double_t, ndim=1] array):             # <<<<<<<<<<<<<<
  *     array = check_contiguous(array)
  * 
  */
-  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_n_s_array); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 119, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__7);
-  __Pyx_GIVEREF(__pyx_tuple__7);
-  __pyx_codeobj__8 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_python_arcticpy_wrapper_pyx, __pyx_n_s_cy_print_array, 119, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__8)) __PYX_ERR(0, 119, __pyx_L1_error)
+  __pyx_codeobj__8 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_python_arcticpy_wrapper_pyx, __pyx_n_s_cy_print_array, 119, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__8)) __PYX_ERR(2, 119, __pyx_L1_error)
 
   /* "arcticpy/wrapper.pyx":125
  * 
  * 
  * def cy_print_array_2D(np.ndarray[np.double_t, ndim=2] array):             # <<<<<<<<<<<<<<
  *     array = check_contiguous(array)
  * 
  */
-  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_n_s_array); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 125, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__9);
-  __Pyx_GIVEREF(__pyx_tuple__9);
-  __pyx_codeobj__10 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__9, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_python_arcticpy_wrapper_pyx, __pyx_n_s_cy_print_array_2D, 125, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__10)) __PYX_ERR(0, 125, __pyx_L1_error)
+  __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_python_arcticpy_wrapper_pyx, __pyx_n_s_cy_print_array_2D, 125, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(2, 125, __pyx_L1_error)
 
   /* "arcticpy/wrapper.pyx":131
  * 
  * 
  * def cy_add_cti(             # <<<<<<<<<<<<<<
  *     np.ndarray[np.double_t, ndim=2] image,
  *     # ========
  */
-  __pyx_tuple__11 = PyTuple_Pack(64, __pyx_n_s_image, __pyx_n_s_parallel_dwell_times, __pyx_n_s_parallel_prescan_offset, __pyx_n_s_parallel_overscan_start, __pyx_n_s_parallel_empty_traps_between_col, __pyx_n_s_parallel_empty_traps_for_first_t, __pyx_n_s_parallel_force_release_away_from, __pyx_n_s_parallel_use_integer_express_mat, __pyx_n_s_parallel_n_pumps, __pyx_n_s_parallel_roe_type, __pyx_n_s_parallel_fraction_of_traps_per_p, __pyx_n_s_parallel_full_well_depths, __pyx_n_s_parallel_well_notch_depths, __pyx_n_s_parallel_well_fill_powers, __pyx_n_s_parallel_first_electron_fills, __pyx_n_s_parallel_trap_densities, __pyx_n_s_parallel_trap_release_timescales, __pyx_n_s_parallel_trap_third_params, __pyx_n_s_parallel_trap_fourth_params, __pyx_n_s_parallel_n_traps_ic, __pyx_n_s_parallel_n_traps_sc, __pyx_n_s_parallel_n_traps_ic_co, __pyx_n_s_parallel_n_traps_sc_co, __pyx_n_s_parallel_express, __pyx_n_s_parallel_window_offset, __pyx_n_s_parallel_window_start, __pyx_n_s_parallel_window_stop, __pyx_n_s_parallel_time_start, __pyx_n_s_parallel_time_stop, __pyx_n_s_parallel_prune_n_electrons, __pyx_n_s_parallel_prune_frequency, __pyx_n_s_serial_dwell_times, __pyx_n_s_serial_prescan_offset, __pyx_n_s_serial_overscan_start, __pyx_n_s_serial_empty_traps_between_colum, __pyx_n_s_serial_empty_traps_for_first_tra, __pyx_n_s_serial_force_release_away_from_r, __pyx_n_s_serial_use_integer_express_matri, __pyx_n_s_serial_n_pumps, __pyx_n_s_serial_roe_type, __pyx_n_s_serial_fraction_of_traps_per_pha, __pyx_n_s_serial_full_well_depths, __pyx_n_s_serial_well_notch_depths, __pyx_n_s_serial_well_fill_powers, __pyx_n_s_serial_first_electron_fills, __pyx_n_s_serial_trap_densities, __pyx_n_s_serial_trap_release_timescales, __pyx_n_s_serial_trap_third_params, __pyx_n_s_serial_trap_fourth_params, __pyx_n_s_serial_n_traps_ic, __pyx_n_s_serial_n_traps_sc, __pyx_n_s_serial_n_traps_ic_co, __pyx_n_s_serial_n_traps_sc_co, __pyx_n_s_serial_express, __pyx_n_s_serial_window_offset, __pyx_n_s_serial_window_start, __pyx_n_s_serial_window_stop, __pyx_n_s_serial_time_start, __pyx_n_s_serial_time_stop, __pyx_n_s_serial_prune_n_electrons, __pyx_n_s_serial_prune_frequency, __pyx_n_s_allow_negative_pixels, __pyx_n_s_verbosity, __pyx_n_s_iteration); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 131, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__11);
-  __Pyx_GIVEREF(__pyx_tuple__11);
-  __pyx_codeobj__12 = (PyObject*)__Pyx_PyCode_New(64, 0, 64, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_python_arcticpy_wrapper_pyx, __pyx_n_s_cy_add_cti, 131, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__12)) __PYX_ERR(0, 131, __pyx_L1_error)
+  __pyx_tuple__10 = PyTuple_Pack(64, __pyx_n_s_image, __pyx_n_s_parallel_dwell_times, __pyx_n_s_parallel_prescan_offset, __pyx_n_s_parallel_overscan_start, __pyx_n_s_parallel_empty_traps_between_col, __pyx_n_s_parallel_empty_traps_for_first_t, __pyx_n_s_parallel_force_release_away_from, __pyx_n_s_parallel_use_integer_express_mat, __pyx_n_s_parallel_n_pumps, __pyx_n_s_parallel_roe_type, __pyx_n_s_parallel_fraction_of_traps_per_p, __pyx_n_s_parallel_full_well_depths, __pyx_n_s_parallel_well_notch_depths, __pyx_n_s_parallel_well_fill_powers, __pyx_n_s_parallel_first_electron_fills, __pyx_n_s_parallel_trap_densities, __pyx_n_s_parallel_trap_release_timescales, __pyx_n_s_parallel_trap_third_params, __pyx_n_s_parallel_trap_fourth_params, __pyx_n_s_parallel_n_traps_ic, __pyx_n_s_parallel_n_traps_sc, __pyx_n_s_parallel_n_traps_ic_co, __pyx_n_s_parallel_n_traps_sc_co, __pyx_n_s_parallel_express, __pyx_n_s_parallel_window_offset, __pyx_n_s_parallel_window_start, __pyx_n_s_parallel_window_stop, __pyx_n_s_parallel_time_start, __pyx_n_s_parallel_time_stop, __pyx_n_s_parallel_prune_n_electrons, __pyx_n_s_parallel_prune_frequency, __pyx_n_s_serial_dwell_times, __pyx_n_s_serial_prescan_offset, __pyx_n_s_serial_overscan_start, __pyx_n_s_serial_empty_traps_between_colum, __pyx_n_s_serial_empty_traps_for_first_tra, __pyx_n_s_serial_force_release_away_from_r, __pyx_n_s_serial_use_integer_express_matri, __pyx_n_s_serial_n_pumps, __pyx_n_s_serial_roe_type, __pyx_n_s_serial_fraction_of_traps_per_pha, __pyx_n_s_serial_full_well_depths, __pyx_n_s_serial_well_notch_depths, __pyx_n_s_serial_well_fill_powers, __pyx_n_s_serial_first_electron_fills, __pyx_n_s_serial_trap_densities, __pyx_n_s_serial_trap_release_timescales, __pyx_n_s_serial_trap_third_params, __pyx_n_s_serial_trap_fourth_params, __pyx_n_s_serial_n_traps_ic, __pyx_n_s_serial_n_traps_sc, __pyx_n_s_serial_n_traps_ic_co, __pyx_n_s_serial_n_traps_sc_co, __pyx_n_s_serial_express, __pyx_n_s_serial_window_offset, __pyx_n_s_serial_window_start, __pyx_n_s_serial_window_stop, __pyx_n_s_serial_time_start, __pyx_n_s_serial_time_stop, __pyx_n_s_serial_prune_n_electrons, __pyx_n_s_serial_prune_frequency, __pyx_n_s_allow_negative_pixels, __pyx_n_s_verbosity, __pyx_n_s_iteration); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 131, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__10);
+  __Pyx_GIVEREF(__pyx_tuple__10);
+  __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(64, 0, 0, 64, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__10, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_python_arcticpy_wrapper_pyx, __pyx_n_s_cy_add_cti, 131, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(2, 131, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
+/* #### Code section: init_constants ### */
+
+static CYTHON_SMALL_CODE int __Pyx_InitConstants(void) {
+  if (__Pyx_CreateStringTabAndInitStrings() < 0) __PYX_ERR(2, 2, __pyx_L1_error);
+  return 0;
+  __pyx_L1_error:;
+  return -1;
+}
+/* #### Code section: init_globals ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 2, __pyx_L1_error);
+  /* NumpyImportArray.init */
+  /*
+ * Cython has automatically inserted a call to _import_array since
+ * you didn't include one when you cimported numpy. To disable this
+ * add the line
+ *   <void>numpy._import_array
+ */
+#ifdef NPY_FEATURE_VERSION
+#if !NO_IMPORT_ARRAY
+if (unlikely(_import_array() == -1)) {
+    PyErr_SetString(PyExc_ImportError, "numpy.core.multiarray failed to import "
+    "(auto-generated because you didn't call 'numpy.import_array()' after cimporting numpy; "
+    "use '<void>numpy._import_array' to disable if you are certain you don't need it).");
+}
+#endif
+#endif
+
+if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 2, __pyx_L1_error)
+
   return 0;
   __pyx_L1_error:;
   return -1;
 }
+/* #### Code section: init_module ### */
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_variable_export_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_function_export_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_type_init_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_type_import_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_variable_import_code(void); /*proto*/
@@ -5930,55 +7619,41 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_0(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyTypeObject),
+  #elif CYTHON_COMPILING_IN_LIMITED_API
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 199, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 203, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 199, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 222, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 770, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 772, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 774, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 776, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 778, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 780, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 782, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 784, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 786, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 788, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 826, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_0); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 203, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_0); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 226, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_0); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 230, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_0); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 239, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 813, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 815, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 817, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 819, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 821, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 823, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 825, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 827, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 829, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 831, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_0); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 869, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -5997,14 +7672,63 @@
   __Pyx_RefNannySetupContext("__Pyx_modinit_function_import_code", 0);
   /*--- Function import code ---*/
   __Pyx_RefNannyFinishContext();
   return 0;
 }
 
 
+#if PY_MAJOR_VERSION >= 3
+#if CYTHON_PEP489_MULTI_PHASE_INIT
+static PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def); /*proto*/
+static int __pyx_pymod_exec_wrapper(PyObject* module); /*proto*/
+static PyModuleDef_Slot __pyx_moduledef_slots[] = {
+  {Py_mod_create, (void*)__pyx_pymod_create},
+  {Py_mod_exec, (void*)__pyx_pymod_exec_wrapper},
+  {0, NULL}
+};
+#endif
+
+#ifdef __cplusplus
+namespace {
+  struct PyModuleDef __pyx_moduledef =
+  #else
+  static struct PyModuleDef __pyx_moduledef =
+  #endif
+  {
+      PyModuleDef_HEAD_INIT,
+      "wrapper",
+      0, /* m_doc */
+    #if CYTHON_PEP489_MULTI_PHASE_INIT
+      0, /* m_size */
+    #elif CYTHON_USE_MODULE_STATE
+      sizeof(__pyx_mstate), /* m_size */
+    #else
+      -1, /* m_size */
+    #endif
+      __pyx_methods /* m_methods */,
+    #if CYTHON_PEP489_MULTI_PHASE_INIT
+      __pyx_moduledef_slots, /* m_slots */
+    #else
+      NULL, /* m_reload */
+    #endif
+    #if CYTHON_USE_MODULE_STATE
+      __pyx_m_traverse, /* m_traverse */
+      __pyx_m_clear, /* m_clear */
+      NULL /* m_free */
+    #else
+      NULL, /* m_traverse */
+      NULL, /* m_clear */
+      NULL /* m_free */
+    #endif
+  };
+  #ifdef __cplusplus
+} /* anonymous namespace */
+#endif
+#endif
+
 #ifndef CYTHON_NO_PYINIT_EXPORT
 #define __Pyx_PyMODINIT_FUNC PyMODINIT_FUNC
 #elif PY_MAJOR_VERSION < 3
 #ifdef __cplusplus
 #define __Pyx_PyMODINIT_FUNC extern "C" void
 #else
 #define __Pyx_PyMODINIT_FUNC void
@@ -6047,42 +7771,56 @@
         PyErr_SetString(
             PyExc_ImportError,
             "Interpreter change detected - this module can only be loaded into one interpreter per process.");
         return -1;
     }
     return 0;
 }
-static CYTHON_SMALL_CODE int __Pyx_copy_spec_to_module(PyObject *spec, PyObject *moddict, const char* from_name, const char* to_name, int allow_none) {
+#if CYTHON_COMPILING_IN_LIMITED_API
+static CYTHON_SMALL_CODE int __Pyx_copy_spec_to_module(PyObject *spec, PyObject *module, const char* from_name, const char* to_name, int allow_none)
+#else
+static CYTHON_SMALL_CODE int __Pyx_copy_spec_to_module(PyObject *spec, PyObject *moddict, const char* from_name, const char* to_name, int allow_none)
+#endif
+{
     PyObject *value = PyObject_GetAttrString(spec, from_name);
     int result = 0;
     if (likely(value)) {
         if (allow_none || value != Py_None) {
+#if CYTHON_COMPILING_IN_LIMITED_API
+            result = PyModule_AddObject(module, to_name, value);
+#else
             result = PyDict_SetItemString(moddict, to_name, value);
+#endif
         }
         Py_DECREF(value);
     } else if (PyErr_ExceptionMatches(PyExc_AttributeError)) {
         PyErr_Clear();
     } else {
         result = -1;
     }
     return result;
 }
-static CYTHON_SMALL_CODE PyObject* __pyx_pymod_create(PyObject *spec, CYTHON_UNUSED PyModuleDef *def) {
+static CYTHON_SMALL_CODE PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def) {
     PyObject *module = NULL, *moddict, *modname;
+    CYTHON_UNUSED_VAR(def);
     if (__Pyx_check_single_interpreter())
         return NULL;
     if (__pyx_m)
         return __Pyx_NewRef(__pyx_m);
     modname = PyObject_GetAttrString(spec, "name");
     if (unlikely(!modname)) goto bad;
     module = PyModule_NewObject(modname);
     Py_DECREF(modname);
     if (unlikely(!module)) goto bad;
+#if CYTHON_COMPILING_IN_LIMITED_API
+    moddict = module;
+#else
     moddict = PyModule_GetDict(module);
     if (unlikely(!moddict)) goto bad;
+#endif
     if (unlikely(__Pyx_copy_spec_to_module(spec, moddict, "loader", "__loader__", 1) < 0)) goto bad;
     if (unlikely(__Pyx_copy_spec_to_module(spec, moddict, "origin", "__file__", 1) < 0)) goto bad;
     if (unlikely(__Pyx_copy_spec_to_module(spec, moddict, "parent", "__package__", 1) < 0)) goto bad;
     if (unlikely(__Pyx_copy_spec_to_module(spec, moddict, "submodule_search_locations", "__path__", 0) < 0)) goto bad;
     return module;
 bad:
     Py_XDECREF(module);
@@ -6090,246 +7828,281 @@
 }
 
 
 static CYTHON_SMALL_CODE int __pyx_pymod_exec_wrapper(PyObject *__pyx_pyinit_module)
 #endif
 #endif
 {
+  int stringtab_initialized = 0;
+  #if CYTHON_USE_MODULE_STATE
+  int pystate_addmodule_run = 0;
+  #endif
   PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   if (__pyx_m) {
     if (__pyx_m == __pyx_pyinit_module) return 0;
     PyErr_SetString(PyExc_RuntimeError, "Module 'wrapper' has already been imported. Re-initialisation is not supported.");
     return -1;
   }
   #elif PY_MAJOR_VERSION >= 3
   if (__pyx_m) return __Pyx_NewRef(__pyx_m);
   #endif
+  /*--- Module creation code ---*/
+  #if CYTHON_PEP489_MULTI_PHASE_INIT
+  __pyx_m = __pyx_pyinit_module;
+  Py_INCREF(__pyx_m);
+  #else
+  #if PY_MAJOR_VERSION < 3
+  __pyx_m = Py_InitModule4("wrapper", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
+  if (unlikely(!__pyx_m)) __PYX_ERR(2, 2, __pyx_L1_error)
+  #elif CYTHON_USE_MODULE_STATE
+  __pyx_t_1 = PyModule_Create(&__pyx_moduledef); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 2, __pyx_L1_error)
+  {
+    int add_module_result = PyState_AddModule(__pyx_t_1, &__pyx_moduledef);
+    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to wrapper pseudovariable */
+    if (unlikely((add_module_result < 0))) __PYX_ERR(2, 2, __pyx_L1_error)
+    pystate_addmodule_run = 1;
+  }
+  #else
+  __pyx_m = PyModule_Create(&__pyx_moduledef);
+  if (unlikely(!__pyx_m)) __PYX_ERR(2, 2, __pyx_L1_error)
+  #endif
+  #endif
+  CYTHON_UNUSED_VAR(__pyx_t_1);
+  __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(2, 2, __pyx_L1_error)
+  Py_INCREF(__pyx_d);
+  __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(2, 2, __pyx_L1_error)
+  Py_INCREF(__pyx_b);
+  __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(2, 2, __pyx_L1_error)
+  Py_INCREF(__pyx_cython_runtime);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(2, 2, __pyx_L1_error)
   #if CYTHON_REFNANNY
 __Pyx_RefNanny = __Pyx_RefNannyImportAPI("refnanny");
 if (!__Pyx_RefNanny) {
   PyErr_Clear();
   __Pyx_RefNanny = __Pyx_RefNannyImportAPI("Cython.Runtime.refnanny");
   if (!__Pyx_RefNanny)
       Py_FatalError("failed to import 'refnanny' module");
 }
 #endif
   __Pyx_RefNannySetupContext("__Pyx_PyMODINIT_FUNC PyInit_wrapper(void)", 0);
-  if (__Pyx_check_binary_version() < 0) __PYX_ERR(0, 2, __pyx_L1_error)
+  if (__Pyx_check_binary_version() < 0) __PYX_ERR(2, 2, __pyx_L1_error)
   #ifdef __Pxy_PyFrame_Initialize_Offsets
   __Pxy_PyFrame_Initialize_Offsets();
   #endif
-  __pyx_empty_tuple = PyTuple_New(0); if (unlikely(!__pyx_empty_tuple)) __PYX_ERR(0, 2, __pyx_L1_error)
-  __pyx_empty_bytes = PyBytes_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_bytes)) __PYX_ERR(0, 2, __pyx_L1_error)
-  __pyx_empty_unicode = PyUnicode_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_unicode)) __PYX_ERR(0, 2, __pyx_L1_error)
+  __pyx_empty_tuple = PyTuple_New(0); if (unlikely(!__pyx_empty_tuple)) __PYX_ERR(2, 2, __pyx_L1_error)
+  __pyx_empty_bytes = PyBytes_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_bytes)) __PYX_ERR(2, 2, __pyx_L1_error)
+  __pyx_empty_unicode = PyUnicode_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_unicode)) __PYX_ERR(2, 2, __pyx_L1_error)
   #ifdef __Pyx_CyFunction_USED
-  if (__pyx_CyFunction_init() < 0) __PYX_ERR(0, 2, __pyx_L1_error)
+  if (__pyx_CyFunction_init(__pyx_m) < 0) __PYX_ERR(2, 2, __pyx_L1_error)
   #endif
   #ifdef __Pyx_FusedFunction_USED
-  if (__pyx_FusedFunction_init() < 0) __PYX_ERR(0, 2, __pyx_L1_error)
+  if (__pyx_FusedFunction_init(__pyx_m) < 0) __PYX_ERR(2, 2, __pyx_L1_error)
   #endif
   #ifdef __Pyx_Coroutine_USED
-  if (__pyx_Coroutine_init() < 0) __PYX_ERR(0, 2, __pyx_L1_error)
+  if (__pyx_Coroutine_init(__pyx_m) < 0) __PYX_ERR(2, 2, __pyx_L1_error)
   #endif
   #ifdef __Pyx_Generator_USED
-  if (__pyx_Generator_init() < 0) __PYX_ERR(0, 2, __pyx_L1_error)
+  if (__pyx_Generator_init(__pyx_m) < 0) __PYX_ERR(2, 2, __pyx_L1_error)
   #endif
   #ifdef __Pyx_AsyncGen_USED
-  if (__pyx_AsyncGen_init() < 0) __PYX_ERR(0, 2, __pyx_L1_error)
+  if (__pyx_AsyncGen_init(__pyx_m) < 0) __PYX_ERR(2, 2, __pyx_L1_error)
   #endif
   #ifdef __Pyx_StopAsyncIteration_USED
-  if (__pyx_StopAsyncIteration_init() < 0) __PYX_ERR(0, 2, __pyx_L1_error)
+  if (__pyx_StopAsyncIteration_init(__pyx_m) < 0) __PYX_ERR(2, 2, __pyx_L1_error)
   #endif
   /*--- Library function declarations ---*/
   /*--- Threads initialization code ---*/
   #if defined(WITH_THREAD) && PY_VERSION_HEX < 0x030700F0 && defined(__PYX_FORCE_INIT_THREADS) && __PYX_FORCE_INIT_THREADS
   PyEval_InitThreads();
   #endif
-  /*--- Module creation code ---*/
-  #if CYTHON_PEP489_MULTI_PHASE_INIT
-  __pyx_m = __pyx_pyinit_module;
-  Py_INCREF(__pyx_m);
-  #else
-  #if PY_MAJOR_VERSION < 3
-  __pyx_m = Py_InitModule4("wrapper", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
-  #else
-  __pyx_m = PyModule_Create(&__pyx_moduledef);
-  #endif
-  if (unlikely(!__pyx_m)) __PYX_ERR(0, 2, __pyx_L1_error)
-  #endif
-  __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 2, __pyx_L1_error)
-  Py_INCREF(__pyx_d);
-  __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 2, __pyx_L1_error)
-  Py_INCREF(__pyx_b);
-  __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 2, __pyx_L1_error)
-  Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 2, __pyx_L1_error);
   /*--- Initialize various global constants etc. ---*/
-  if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 2, __pyx_L1_error)
+  if (__Pyx_InitConstants() < 0) __PYX_ERR(2, 2, __pyx_L1_error)
+  stringtab_initialized = 1;
+  if (__Pyx_InitGlobals() < 0) __PYX_ERR(2, 2, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
-  if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 2, __pyx_L1_error)
+  if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(2, 2, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_arcticpy__wrapper) {
-    if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 2, __pyx_L1_error)
+    if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(2, 2, __pyx_L1_error)
   }
   #if PY_MAJOR_VERSION >= 3
   {
-    PyObject *modules = PyImport_GetModuleDict(); if (unlikely(!modules)) __PYX_ERR(0, 2, __pyx_L1_error)
+    PyObject *modules = PyImport_GetModuleDict(); if (unlikely(!modules)) __PYX_ERR(2, 2, __pyx_L1_error)
     if (!PyDict_GetItemString(modules, "arcticpy.wrapper")) {
-      if (unlikely(PyDict_SetItemString(modules, "arcticpy.wrapper", __pyx_m) < 0)) __PYX_ERR(0, 2, __pyx_L1_error)
+      if (unlikely((PyDict_SetItemString(modules, "arcticpy.wrapper", __pyx_m) < 0))) __PYX_ERR(2, 2, __pyx_L1_error)
     }
   }
   #endif
   /*--- Builtin init code ---*/
-  if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(0, 2, __pyx_L1_error)
+  if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(2, 2, __pyx_L1_error)
   /*--- Constants init code ---*/
-  if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(0, 2, __pyx_L1_error)
+  if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(2, 2, __pyx_L1_error)
   /*--- Global type/function init code ---*/
   (void)__Pyx_modinit_global_init_code();
   (void)__Pyx_modinit_variable_export_code();
   (void)__Pyx_modinit_function_export_code();
   (void)__Pyx_modinit_type_init_code();
-  if (unlikely(__Pyx_modinit_type_import_code() < 0)) __PYX_ERR(0, 2, __pyx_L1_error)
+  if (unlikely((__Pyx_modinit_type_import_code() < 0))) __PYX_ERR(2, 2, __pyx_L1_error)
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
-  if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 2, __pyx_L1_error)
+  if (__Pyx_patch_abc() < 0) __PYX_ERR(2, 2, __pyx_L1_error)
   #endif
 
   /* "arcticpy/wrapper.pyx":3
  * 
  * cimport numpy as np
  * import numpy as np             # <<<<<<<<<<<<<<
  * from libcpp.string cimport string
  * 
  */
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_numpy, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_np, __pyx_t_1) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_2 = __Pyx_ImportDottedModule(__pyx_n_s_numpy, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 3, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_np, __pyx_t_2) < 0) __PYX_ERR(2, 3, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "arcticpy/wrapper.pyx":105
  * 
  * 
  * def cy_print_version():             # <<<<<<<<<<<<<<
  *     print_version()
  * 
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8arcticpy_7wrapper_1cy_print_version, NULL, __pyx_n_s_arcticpy_wrapper); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 105, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_cy_print_version, __pyx_t_1) < 0) __PYX_ERR(0, 105, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8arcticpy_7wrapper_1cy_print_version, 0, __pyx_n_s_cy_print_version, NULL, __pyx_n_s_arcticpy_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__4)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 105, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_cy_print_version, __pyx_t_2) < 0) __PYX_ERR(2, 105, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "arcticpy/wrapper.pyx":108
  *     print_version()
  * 
  * def cy_version_arctic():             # <<<<<<<<<<<<<<
  *     return version_arctic().decode("utf-8")
  * 
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8arcticpy_7wrapper_3cy_version_arctic, NULL, __pyx_n_s_arcticpy_wrapper); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 108, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_cy_version_arctic, __pyx_t_1) < 0) __PYX_ERR(0, 108, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8arcticpy_7wrapper_3cy_version_arctic, 0, __pyx_n_s_cy_version_arctic, NULL, __pyx_n_s_arcticpy_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__5)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 108, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_cy_version_arctic, __pyx_t_2) < 0) __PYX_ERR(2, 108, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "arcticpy/wrapper.pyx":111
  *     return version_arctic().decode("utf-8")
  * 
  * def check_contiguous(array):             # <<<<<<<<<<<<<<
  *     """ Make sure an array is contiguous and C-style. """
  *     if not array.flags['C_CONTIGUOUS']:
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8arcticpy_7wrapper_5check_contiguous, NULL, __pyx_n_s_arcticpy_wrapper); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 111, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_check_contiguous, __pyx_t_1) < 0) __PYX_ERR(0, 111, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8arcticpy_7wrapper_5check_contiguous, 0, __pyx_n_s_check_contiguous, NULL, __pyx_n_s_arcticpy_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__7)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 111, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_check_contiguous, __pyx_t_2) < 0) __PYX_ERR(2, 111, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "arcticpy/wrapper.pyx":119
  * 
  * 
  * def cy_print_array(np.ndarray[np.double_t, ndim=1] array):             # <<<<<<<<<<<<<<
  *     array = check_contiguous(array)
  * 
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8arcticpy_7wrapper_7cy_print_array, NULL, __pyx_n_s_arcticpy_wrapper); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 119, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_cy_print_array, __pyx_t_1) < 0) __PYX_ERR(0, 119, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8arcticpy_7wrapper_7cy_print_array, 0, __pyx_n_s_cy_print_array, NULL, __pyx_n_s_arcticpy_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__8)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 119, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_cy_print_array, __pyx_t_2) < 0) __PYX_ERR(2, 119, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "arcticpy/wrapper.pyx":125
  * 
  * 
  * def cy_print_array_2D(np.ndarray[np.double_t, ndim=2] array):             # <<<<<<<<<<<<<<
  *     array = check_contiguous(array)
  * 
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8arcticpy_7wrapper_9cy_print_array_2D, NULL, __pyx_n_s_arcticpy_wrapper); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 125, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_cy_print_array_2D, __pyx_t_1) < 0) __PYX_ERR(0, 125, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8arcticpy_7wrapper_9cy_print_array_2D, 0, __pyx_n_s_cy_print_array_2D, NULL, __pyx_n_s_arcticpy_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__9)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 125, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_cy_print_array_2D, __pyx_t_2) < 0) __PYX_ERR(2, 125, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "arcticpy/wrapper.pyx":131
  * 
  * 
  * def cy_add_cti(             # <<<<<<<<<<<<<<
  *     np.ndarray[np.double_t, ndim=2] image,
  *     # ========
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8arcticpy_7wrapper_11cy_add_cti, NULL, __pyx_n_s_arcticpy_wrapper); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 131, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_cy_add_cti, __pyx_t_1) < 0) __PYX_ERR(0, 131, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8arcticpy_7wrapper_11cy_add_cti, 0, __pyx_n_s_cy_add_cti, NULL, __pyx_n_s_arcticpy_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__11)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 131, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_cy_add_cti, __pyx_t_2) < 0) __PYX_ERR(2, 131, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "arcticpy/wrapper.pyx":2
  * 
  * cimport numpy as np             # <<<<<<<<<<<<<<
  * import numpy as np
  * from libcpp.string cimport string
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 2, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-
-  /* "string.to_py":55
- * 
- * @cname("__pyx_convert_PyByteArray_string_to_py_std__in_string")
- * cdef inline object __pyx_convert_PyByteArray_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
- *     return __Pyx_PyByteArray_FromStringAndSize(s.data(), s.size())
- * 
- */
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 2, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(2, 2, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
   if (__pyx_m) {
-    if (__pyx_d) {
+    if (__pyx_d && stringtab_initialized) {
       __Pyx_AddTraceback("init arcticpy.wrapper", __pyx_clineno, __pyx_lineno, __pyx_filename);
     }
+    #if !CYTHON_USE_MODULE_STATE
     Py_CLEAR(__pyx_m);
+    #else
+    Py_DECREF(__pyx_m);
+    if (pystate_addmodule_run) {
+      PyObject *tp, *value, *tb;
+      PyErr_Fetch(&tp, &value, &tb);
+      PyState_RemoveModule(&__pyx_moduledef);
+      PyErr_Restore(tp, value, tb);
+    }
+    #endif
   } else if (!PyErr_Occurred()) {
     PyErr_SetString(PyExc_ImportError, "init arcticpy.wrapper");
   }
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   return (__pyx_m != NULL) ? 0 : -1;
   #elif PY_MAJOR_VERSION >= 3
   return __pyx_m;
   #else
   return;
   #endif
 }
+/* #### Code section: cleanup_globals ### */
+/* #### Code section: cleanup_module ### */
+/* #### Code section: main_method ### */
+/* #### Code section: utility_code_pragmas ### */
+#ifdef _MSC_VER
+#pragma warning( push )
+/* Warning 4127: conditional expression is constant
+ * Cython uses constant conditional expressions to allow in inline functions to be optimized at
+ * compile-time, so this warning is not useful
+ */
+#pragma warning( disable : 4127 )
+#endif
+
+
+
+/* #### Code section: utility_code_def ### */
 
 /* --- Runtime support code --- */
 /* Refnanny */
 #if CYTHON_REFNANNY
 static __Pyx_RefNannyAPIStruct *__Pyx_RefNannyImportAPI(const char *modname) {
     PyObject *m = NULL, *p = NULL;
     void *r = NULL;
@@ -6341,14 +8114,729 @@
 end:
     Py_XDECREF(p);
     Py_XDECREF(m);
     return (__Pyx_RefNannyAPIStruct *)r;
 }
 #endif
 
+/* PyErrExceptionMatches */
+#if CYTHON_FAST_THREAD_STATE
+static int __Pyx_PyErr_ExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
+    Py_ssize_t i, n;
+    n = PyTuple_GET_SIZE(tuple);
+#if PY_MAJOR_VERSION >= 3
+    for (i=0; i<n; i++) {
+        if (exc_type == PyTuple_GET_ITEM(tuple, i)) return 1;
+    }
+#endif
+    for (i=0; i<n; i++) {
+        if (__Pyx_PyErr_GivenExceptionMatches(exc_type, PyTuple_GET_ITEM(tuple, i))) return 1;
+    }
+    return 0;
+}
+static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err) {
+    int result;
+    PyObject *exc_type;
+#if PY_VERSION_HEX >= 0x030C00A6
+    PyObject *current_exception = tstate->current_exception;
+    if (unlikely(!current_exception)) return 0;
+    exc_type = (PyObject*) Py_TYPE(current_exception);
+    if (exc_type == err) return 1;
+#else
+    exc_type = tstate->curexc_type;
+    if (exc_type == err) return 1;
+    if (unlikely(!exc_type)) return 0;
+#endif
+    #if CYTHON_AVOID_BORROWED_REFS
+    Py_INCREF(exc_type);
+    #endif
+    if (unlikely(PyTuple_Check(err))) {
+        result = __Pyx_PyErr_ExceptionMatchesTuple(exc_type, err);
+    } else {
+        result = __Pyx_PyErr_GivenExceptionMatches(exc_type, err);
+    }
+    #if CYTHON_AVOID_BORROWED_REFS
+    Py_DECREF(exc_type);
+    #endif
+    return result;
+}
+#endif
+
+/* PyErrFetchRestore */
+#if CYTHON_FAST_THREAD_STATE
+static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
+#if PY_VERSION_HEX >= 0x030C00A6
+    PyObject *tmp_value;
+    assert(type == NULL || (value != NULL && type == (PyObject*) Py_TYPE(value)));
+    if (value) {
+        #if CYTHON_COMPILING_IN_CPYTHON
+        if (unlikely(((PyBaseExceptionObject*) value)->traceback != tb))
+        #endif
+            PyException_SetTraceback(value, tb);
+    }
+    tmp_value = tstate->current_exception;
+    tstate->current_exception = value;
+    Py_XDECREF(tmp_value);
+#else
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
+#endif
+}
+static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
+#if PY_VERSION_HEX >= 0x030C00A6
+    PyObject* exc_value;
+    exc_value = tstate->current_exception;
+    tstate->current_exception = 0;
+    *value = exc_value;
+    *type = NULL;
+    *tb = NULL;
+    if (exc_value) {
+        *type = (PyObject*) Py_TYPE(exc_value);
+        Py_INCREF(*type);
+        #if CYTHON_COMPILING_IN_CPYTHON
+        *tb = ((PyBaseExceptionObject*) exc_value)->traceback;
+        Py_XINCREF(*tb);
+        #else
+        *tb = PyException_GetTraceback(exc_value);
+        #endif
+    }
+#else
+    *type = tstate->curexc_type;
+    *value = tstate->curexc_value;
+    *tb = tstate->curexc_traceback;
+    tstate->curexc_type = 0;
+    tstate->curexc_value = 0;
+    tstate->curexc_traceback = 0;
+#endif
+}
+#endif
+
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
+/* PyObjectGetAttrStrNoError */
+static void __Pyx_PyObject_GetAttrStr_ClearAttributeError(void) {
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    if (likely(__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
+        __Pyx_PyErr_Clear();
+}
+static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name) {
+    PyObject *result;
+#if CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_TYPE_SLOTS && PY_VERSION_HEX >= 0x030700B1
+    PyTypeObject* tp = Py_TYPE(obj);
+    if (likely(tp->tp_getattro == PyObject_GenericGetAttr)) {
+        return _PyObject_GenericGetAttrWithDict(obj, attr_name, NULL, 1);
+    }
+#endif
+    result = __Pyx_PyObject_GetAttrStr(obj, attr_name);
+    if (unlikely(!result)) {
+        __Pyx_PyObject_GetAttrStr_ClearAttributeError();
+    }
+    return result;
+}
+
+/* GetBuiltinName */
+static PyObject *__Pyx_GetBuiltinName(PyObject *name) {
+    PyObject* result = __Pyx_PyObject_GetAttrStrNoError(__pyx_b, name);
+    if (unlikely(!result) && !PyErr_Occurred()) {
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
+/* GetTopmostException */
+#if CYTHON_USE_EXC_INFO_STACK && CYTHON_FAST_THREAD_STATE
+static _PyErr_StackItem *
+__Pyx_PyErr_GetTopmostException(PyThreadState *tstate)
+{
+    _PyErr_StackItem *exc_info = tstate->exc_info;
+    while ((exc_info->exc_value == NULL || exc_info->exc_value == Py_None) &&
+           exc_info->previous_item != NULL)
+    {
+        exc_info = exc_info->previous_item;
+    }
+    return exc_info;
+}
+#endif
+
+/* SaveResetException */
+#if CYTHON_FAST_THREAD_STATE
+static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
+  #if CYTHON_USE_EXC_INFO_STACK && PY_VERSION_HEX >= 0x030B00a4
+    _PyErr_StackItem *exc_info = __Pyx_PyErr_GetTopmostException(tstate);
+    PyObject *exc_value = exc_info->exc_value;
+    if (exc_value == NULL || exc_value == Py_None) {
+        *value = NULL;
+        *type = NULL;
+        *tb = NULL;
+    } else {
+        *value = exc_value;
+        Py_INCREF(*value);
+        *type = (PyObject*) Py_TYPE(exc_value);
+        Py_INCREF(*type);
+        *tb = PyException_GetTraceback(exc_value);
+    }
+  #elif CYTHON_USE_EXC_INFO_STACK
+    _PyErr_StackItem *exc_info = __Pyx_PyErr_GetTopmostException(tstate);
+    *type = exc_info->exc_type;
+    *value = exc_info->exc_value;
+    *tb = exc_info->exc_traceback;
+    Py_XINCREF(*type);
+    Py_XINCREF(*value);
+    Py_XINCREF(*tb);
+  #else
+    *type = tstate->exc_type;
+    *value = tstate->exc_value;
+    *tb = tstate->exc_traceback;
+    Py_XINCREF(*type);
+    Py_XINCREF(*value);
+    Py_XINCREF(*tb);
+  #endif
+}
+static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
+  #if CYTHON_USE_EXC_INFO_STACK && PY_VERSION_HEX >= 0x030B00a4
+    _PyErr_StackItem *exc_info = tstate->exc_info;
+    PyObject *tmp_value = exc_info->exc_value;
+    exc_info->exc_value = value;
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(type);
+    Py_XDECREF(tb);
+  #else
+    PyObject *tmp_type, *tmp_value, *tmp_tb;
+    #if CYTHON_USE_EXC_INFO_STACK
+    _PyErr_StackItem *exc_info = tstate->exc_info;
+    tmp_type = exc_info->exc_type;
+    tmp_value = exc_info->exc_value;
+    tmp_tb = exc_info->exc_traceback;
+    exc_info->exc_type = type;
+    exc_info->exc_value = value;
+    exc_info->exc_traceback = tb;
+    #else
+    tmp_type = tstate->exc_type;
+    tmp_value = tstate->exc_value;
+    tmp_tb = tstate->exc_traceback;
+    tstate->exc_type = type;
+    tstate->exc_value = value;
+    tstate->exc_traceback = tb;
+    #endif
+    Py_XDECREF(tmp_type);
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(tmp_tb);
+  #endif
+}
+#endif
+
+/* GetException */
+#if CYTHON_FAST_THREAD_STATE
+static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb)
+#else
+static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb)
+#endif
+{
+    PyObject *local_type = NULL, *local_value, *local_tb = NULL;
+#if CYTHON_FAST_THREAD_STATE
+    PyObject *tmp_type, *tmp_value, *tmp_tb;
+  #if PY_VERSION_HEX >= 0x030C00A6
+    local_value = tstate->current_exception;
+    tstate->current_exception = 0;
+    if (likely(local_value)) {
+        local_type = (PyObject*) Py_TYPE(local_value);
+        Py_INCREF(local_type);
+        local_tb = PyException_GetTraceback(local_value);
+    }
+  #else
+    local_type = tstate->curexc_type;
+    local_value = tstate->curexc_value;
+    local_tb = tstate->curexc_traceback;
+    tstate->curexc_type = 0;
+    tstate->curexc_value = 0;
+    tstate->curexc_traceback = 0;
+  #endif
+#else
+    PyErr_Fetch(&local_type, &local_value, &local_tb);
+#endif
+    PyErr_NormalizeException(&local_type, &local_value, &local_tb);
+#if CYTHON_FAST_THREAD_STATE && PY_VERSION_HEX >= 0x030C00A6
+    if (unlikely(tstate->current_exception))
+#elif CYTHON_FAST_THREAD_STATE
+    if (unlikely(tstate->curexc_type))
+#else
+    if (unlikely(PyErr_Occurred()))
+#endif
+        goto bad;
+    #if PY_MAJOR_VERSION >= 3
+    if (local_tb) {
+        if (unlikely(PyException_SetTraceback(local_value, local_tb) < 0))
+            goto bad;
+    }
+    #endif
+    Py_XINCREF(local_tb);
+    Py_XINCREF(local_type);
+    Py_XINCREF(local_value);
+    *type = local_type;
+    *value = local_value;
+    *tb = local_tb;
+#if CYTHON_FAST_THREAD_STATE
+    #if CYTHON_USE_EXC_INFO_STACK
+    {
+        _PyErr_StackItem *exc_info = tstate->exc_info;
+      #if PY_VERSION_HEX >= 0x030B00a4
+        tmp_value = exc_info->exc_value;
+        exc_info->exc_value = local_value;
+        tmp_type = NULL;
+        tmp_tb = NULL;
+        Py_XDECREF(local_type);
+        Py_XDECREF(local_tb);
+      #else
+        tmp_type = exc_info->exc_type;
+        tmp_value = exc_info->exc_value;
+        tmp_tb = exc_info->exc_traceback;
+        exc_info->exc_type = local_type;
+        exc_info->exc_value = local_value;
+        exc_info->exc_traceback = local_tb;
+      #endif
+    }
+    #else
+    tmp_type = tstate->exc_type;
+    tmp_value = tstate->exc_value;
+    tmp_tb = tstate->exc_traceback;
+    tstate->exc_type = local_type;
+    tstate->exc_value = local_value;
+    tstate->exc_traceback = local_tb;
+    #endif
+    Py_XDECREF(tmp_type);
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(tmp_tb);
+#else
+    PyErr_SetExcInfo(local_type, local_value, local_tb);
+#endif
+    return 0;
+bad:
+    *type = 0;
+    *value = 0;
+    *tb = 0;
+    Py_XDECREF(local_type);
+    Py_XDECREF(local_value);
+    Py_XDECREF(local_tb);
+    return -1;
+}
+
+/* PyObjectCall */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
+    PyObject *result;
+    ternaryfunc call = Py_TYPE(func)->tp_call;
+    if (unlikely(!call))
+        return PyObject_Call(func, arg, kw);
+    if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
+        return NULL;
+    result = (*call)(func, arg, kw);
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
+/* RaiseException */
+#if PY_MAJOR_VERSION < 3
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause) {
+    __Pyx_PyThreadState_declare
+    CYTHON_UNUSED_VAR(cause);
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
+      #if PY_VERSION_HEX >= 0x030C00A6
+        PyException_SetTraceback(value, tb);
+      #elif CYTHON_FAST_THREAD_STATE
+        PyThreadState *tstate = __Pyx_PyThreadState_Current;
+        PyObject* tmp_tb = tstate->curexc_traceback;
+        if (tb != tmp_tb) {
+            Py_INCREF(tb);
+            tstate->curexc_traceback = tb;
+            Py_XDECREF(tmp_tb);
+        }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
+#endif
+    }
+bad:
+    Py_XDECREF(owned_instance);
+    return;
+}
+#endif
+
+/* TupleAndListFromArray */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE void __Pyx_copy_object_array(PyObject *const *CYTHON_RESTRICT src, PyObject** CYTHON_RESTRICT dest, Py_ssize_t length) {
+    PyObject *v;
+    Py_ssize_t i;
+    for (i = 0; i < length; i++) {
+        v = dest[i] = src[i];
+        Py_INCREF(v);
+    }
+}
+static CYTHON_INLINE PyObject *
+__Pyx_PyTuple_FromArray(PyObject *const *src, Py_ssize_t n)
+{
+    PyObject *res;
+    if (n <= 0) {
+        Py_INCREF(__pyx_empty_tuple);
+        return __pyx_empty_tuple;
+    }
+    res = PyTuple_New(n);
+    if (unlikely(res == NULL)) return NULL;
+    __Pyx_copy_object_array(src, ((PyTupleObject*)res)->ob_item, n);
+    return res;
+}
+static CYTHON_INLINE PyObject *
+__Pyx_PyList_FromArray(PyObject *const *src, Py_ssize_t n)
+{
+    PyObject *res;
+    if (n <= 0) {
+        return PyList_New(0);
+    }
+    res = PyList_New(n);
+    if (unlikely(res == NULL)) return NULL;
+    __Pyx_copy_object_array(src, ((PyListObject*)res)->ob_item, n);
+    return res;
+}
+#endif
+
+/* BytesEquals */
+static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals) {
+#if CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API
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
+#if CYTHON_USE_UNICODE_INTERNALS && (PY_VERSION_HEX < 0x030B0000)
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
+static CYTHON_INLINE int __Pyx_PyUnicode_Equals(PyObject* s1, PyObject* s2, int equals) {
+#if CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API
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
+/* fastcall */
+#if CYTHON_METH_FASTCALL
+static CYTHON_INLINE PyObject * __Pyx_GetKwValue_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues, PyObject *s)
+{
+    Py_ssize_t i, n = PyTuple_GET_SIZE(kwnames);
+    for (i = 0; i < n; i++)
+    {
+        if (s == PyTuple_GET_ITEM(kwnames, i)) return kwvalues[i];
+    }
+    for (i = 0; i < n; i++)
+    {
+        int eq = __Pyx_PyUnicode_Equals(s, PyTuple_GET_ITEM(kwnames, i), Py_EQ);
+        if (unlikely(eq != 0)) {
+            if (unlikely(eq < 0)) return NULL;  // error
+            return kwvalues[i];
+        }
+    }
+    return NULL;  // not found (no exception set)
+}
+#endif
+
 /* decode_c_bytes */
 static CYTHON_INLINE PyObject* __Pyx_decode_c_bytes(
          const char* cstring, Py_ssize_t length, Py_ssize_t start, Py_ssize_t stop,
          const char* encoding, const char* errors,
          PyObject* (*decode_func)(const char *s, Py_ssize_t size, const char *errors)) {
     if (unlikely((start < 0) | (stop < 0))) {
         if (start < 0) {
@@ -6368,27 +8856,169 @@
     if (decode_func) {
         return decode_func(cstring, length, errors);
     } else {
         return PyUnicode_Decode(cstring, length, encoding, errors);
     }
 }
 
-/* PyObjectGetAttrStr */
-#if CYTHON_USE_TYPE_SLOTS
-static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStr(PyObject* obj, PyObject* attr_name) {
-    PyTypeObject* tp = Py_TYPE(obj);
-    if (likely(tp->tp_getattro))
-        return tp->tp_getattro(obj, attr_name);
-#if PY_MAJOR_VERSION < 3
-    if (likely(tp->tp_getattr))
-        return tp->tp_getattr(obj, PyString_AS_STRING(attr_name));
-#endif
-    return PyObject_GetAttr(obj, attr_name);
+/* RaiseDoubleKeywords */
+static void __Pyx_RaiseDoubleKeywordsError(
+    const char* func_name,
+    PyObject* kw_name)
+{
+    PyErr_Format(PyExc_TypeError,
+        #if PY_MAJOR_VERSION >= 3
+        "%s() got multiple values for keyword argument '%U'", func_name, kw_name);
+        #else
+        "%s() got multiple values for keyword argument '%s'", func_name,
+        PyString_AsString(kw_name));
+        #endif
+}
+
+/* ParseKeywords */
+static int __Pyx_ParseOptionalKeywords(
+    PyObject *kwds,
+    PyObject *const *kwvalues,
+    PyObject **argnames[],
+    PyObject *kwds2,
+    PyObject *values[],
+    Py_ssize_t num_pos_args,
+    const char* function_name)
+{
+    PyObject *key = 0, *value = 0;
+    Py_ssize_t pos = 0;
+    PyObject*** name;
+    PyObject*** first_kw_arg = argnames + num_pos_args;
+    int kwds_is_tuple = CYTHON_METH_FASTCALL && likely(PyTuple_Check(kwds));
+    while (1) {
+        if (kwds_is_tuple) {
+            if (pos >= PyTuple_GET_SIZE(kwds)) break;
+            key = PyTuple_GET_ITEM(kwds, pos);
+            value = kwvalues[pos];
+            pos++;
+        }
+        else
+        {
+            if (!PyDict_Next(kwds, &pos, &key, &value)) break;
+        }
+        name = first_kw_arg;
+        while (*name && (**name != key)) name++;
+        if (*name) {
+            values[name-argnames] = value;
+            continue;
+        }
+        name = first_kw_arg;
+        #if PY_MAJOR_VERSION < 3
+        if (likely(PyString_Check(key))) {
+            while (*name) {
+                if ((CYTHON_COMPILING_IN_PYPY || PyString_GET_SIZE(**name) == PyString_GET_SIZE(key))
+                        && _PyString_Eq(**name, key)) {
+                    values[name-argnames] = value;
+                    break;
+                }
+                name++;
+            }
+            if (*name) continue;
+            else {
+                PyObject*** argname = argnames;
+                while (argname != first_kw_arg) {
+                    if ((**argname == key) || (
+                            (CYTHON_COMPILING_IN_PYPY || PyString_GET_SIZE(**argname) == PyString_GET_SIZE(key))
+                             && _PyString_Eq(**argname, key))) {
+                        goto arg_passed_twice;
+                    }
+                    argname++;
+                }
+            }
+        } else
+        #endif
+        if (likely(PyUnicode_Check(key))) {
+            while (*name) {
+                int cmp = (
+                #if !CYTHON_COMPILING_IN_PYPY && PY_MAJOR_VERSION >= 3
+                    (__Pyx_PyUnicode_GET_LENGTH(**name) != __Pyx_PyUnicode_GET_LENGTH(key)) ? 1 :
+                #endif
+                    PyUnicode_Compare(**name, key)
+                );
+                if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
+                if (cmp == 0) {
+                    values[name-argnames] = value;
+                    break;
+                }
+                name++;
+            }
+            if (*name) continue;
+            else {
+                PyObject*** argname = argnames;
+                while (argname != first_kw_arg) {
+                    int cmp = (**argname == key) ? 0 :
+                    #if !CYTHON_COMPILING_IN_PYPY && PY_MAJOR_VERSION >= 3
+                        (__Pyx_PyUnicode_GET_LENGTH(**argname) != __Pyx_PyUnicode_GET_LENGTH(key)) ? 1 :
+                    #endif
+                        PyUnicode_Compare(**argname, key);
+                    if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
+                    if (cmp == 0) goto arg_passed_twice;
+                    argname++;
+                }
+            }
+        } else
+            goto invalid_keyword_type;
+        if (kwds2) {
+            if (unlikely(PyDict_SetItem(kwds2, key, value))) goto bad;
+        } else {
+            goto invalid_keyword;
+        }
+    }
+    return 0;
+arg_passed_twice:
+    __Pyx_RaiseDoubleKeywordsError(function_name, key);
+    goto bad;
+invalid_keyword_type:
+    PyErr_Format(PyExc_TypeError,
+        "%.200s() keywords must be strings", function_name);
+    goto bad;
+invalid_keyword:
+    #if PY_MAJOR_VERSION < 3
+    PyErr_Format(PyExc_TypeError,
+        "%.200s() got an unexpected keyword argument '%.200s'",
+        function_name, PyString_AsString(key));
+    #else
+    PyErr_Format(PyExc_TypeError,
+        "%s() got an unexpected keyword argument '%U'",
+        function_name, key);
+    #endif
+bad:
+    return -1;
+}
+
+/* RaiseArgTupleInvalid */
+static void __Pyx_RaiseArgtupleInvalid(
+    const char* func_name,
+    int exact,
+    Py_ssize_t num_min,
+    Py_ssize_t num_max,
+    Py_ssize_t num_found)
+{
+    Py_ssize_t num_expected;
+    const char *more_or_less;
+    if (num_found < num_min) {
+        num_expected = num_min;
+        more_or_less = "at least";
+    } else {
+        num_expected = num_max;
+        more_or_less = "at most";
+    }
+    if (exact) {
+        more_or_less = "exactly";
+    }
+    PyErr_Format(PyExc_TypeError,
+                 "%.200s() takes %.8s %" CYTHON_FORMAT_SSIZE_T "d positional argument%.1s (%" CYTHON_FORMAT_SSIZE_T "d given)",
+                 func_name, more_or_less, num_expected,
+                 (num_expected == 1) ? "" : "s", num_found);
 }
-#endif
 
 /* DictGetItem */
 #if PY_MAJOR_VERSION >= 3 && !CYTHON_COMPILING_IN_PYPY
 static PyObject *__Pyx_PyDict_GetItem(PyObject *d, PyObject* key) {
     PyObject *value;
     value = PyDict_GetItemWithError(d, key);
     if (unlikely(!value)) {
@@ -6406,28 +9036,14 @@
         return NULL;
     }
     Py_INCREF(value);
     return value;
 }
 #endif
 
-/* GetBuiltinName */
-static PyObject *__Pyx_GetBuiltinName(PyObject *name) {
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
@@ -6463,14 +9079,22 @@
     result = _PyDict_GetItem_KnownHash(__pyx_d, name, ((PyASCIIObject *) name)->hash);
     __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
     if (likely(result)) {
         return __Pyx_NewRef(result);
     } else if (unlikely(PyErr_Occurred())) {
         return NULL;
     }
+#elif CYTHON_COMPILING_IN_LIMITED_API
+    if (unlikely(!__pyx_m)) {
+        return NULL;
+    }
+    result = PyObject_GetAttr(__pyx_m, name);
+    if (likely(result)) {
+        return result;
+    }
 #else
     result = PyDict_GetItem(__pyx_d, name);
     __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
     if (likely(result)) {
         return __Pyx_NewRef(result);
     }
 #endif
@@ -6481,39 +9105,16 @@
         return __Pyx_NewRef(result);
     }
     PyErr_Clear();
 #endif
     return __Pyx_GetBuiltinName(name);
 }
 
-/* PyCFunctionFastCall */
-#if CYTHON_FAST_PYCCALL
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
 /* PyFunctionFastCall */
-#if CYTHON_FAST_PYCALL
+#if CYTHON_FAST_PYCALL && !CYTHON_VECTORCALL
 static PyObject* __Pyx_PyFunction_FastCallNoKw(PyCodeObject *co, PyObject **args, Py_ssize_t na,
                                                PyObject *globals) {
     PyFrameObject *f;
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
     PyObject **fastlocals;
     Py_ssize_t i;
     PyObject *result;
@@ -6534,15 +9135,14 @@
     }
     result = PyEval_EvalFrameEx(f,0);
     ++tstate->recursion_depth;
     Py_DECREF(f);
     --tstate->recursion_depth;
     return result;
 }
-#if 1 || PY_VERSION_HEX < 0x030600B1
 static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs) {
     PyCodeObject *co = (PyCodeObject *)PyFunction_GET_CODE(func);
     PyObject *globals = PyFunction_GET_GLOBALS(func);
     PyObject *argdefs = PyFunction_GET_DEFAULTS(func);
     PyObject *closure;
 #if PY_MAJOR_VERSION >= 3
     PyObject *kwdefs;
@@ -6550,15 +9150,15 @@
     PyObject *kwtuple, **k;
     PyObject **d;
     Py_ssize_t nd;
     Py_ssize_t nk;
     PyObject *result;
     assert(kwargs == NULL || PyDict_Check(kwargs));
     nk = kwargs ? PyDict_Size(kwargs) : 0;
-    if (Py_EnterRecursiveCall((char*)" while calling a Python object")) {
+    if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object"))) {
         return NULL;
     }
     if (
 #if PY_MAJOR_VERSION >= 3
             co->co_kwonlyargcount == 0 &&
 #endif
             likely(kwargs == NULL || nk == 0) &&
@@ -6621,64 +9221,14 @@
 #endif
     Py_XDECREF(kwtuple);
 done:
     Py_LeaveRecursiveCall();
     return result;
 }
 #endif
-#endif
-
-/* PyObjectCall */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
-    PyObject *result;
-    ternaryfunc call = Py_TYPE(func)->tp_call;
-    if (unlikely(!call))
-        return PyObject_Call(func, arg, kw);
-    if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
-        return NULL;
-    result = (*call)(func, arg, kw);
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
-/* PyObjectCall2Args */
-static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2) {
-    PyObject *args, *result = NULL;
-    #if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(function)) {
-        PyObject *args[2] = {arg1, arg2};
-        return __Pyx_PyFunction_FastCall(function, args, 2);
-    }
-    #endif
-    #if CYTHON_FAST_PYCCALL
-    if (__Pyx_PyFastCFunction_Check(function)) {
-        PyObject *args[2] = {arg1, arg2};
-        return __Pyx_PyCFunction_FastCall(function, args, 2);
-    }
-    #endif
-    args = PyTuple_New(2);
-    if (unlikely(!args)) goto done;
-    Py_INCREF(arg1);
-    PyTuple_SET_ITEM(args, 0, arg1);
-    Py_INCREF(arg2);
-    PyTuple_SET_ITEM(args, 1, arg2);
-    Py_INCREF(function);
-    result = __Pyx_PyObject_Call(function, args, NULL);
-    Py_DECREF(args);
-    Py_DECREF(function);
-done:
-    return result;
-}
 
 /* PyObjectCallMethO */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg) {
     PyObject *self, *result;
     PyCFunction cfunc;
     cfunc = PyCFunction_GET_FUNCTION(func);
@@ -6692,72 +9242,115 @@
             PyExc_SystemError,
             "NULL result without error in PyObject_Call");
     }
     return result;
 }
 #endif
 
-/* PyObjectCallOneArg */
-#if CYTHON_COMPILING_IN_CPYTHON
-static PyObject* __Pyx__PyObject_CallOneArg(PyObject *func, PyObject *arg) {
+/* PyObjectFastCall */
+static PyObject* __Pyx_PyObject_FastCall_fallback(PyObject *func, PyObject **args, size_t nargs, PyObject *kwargs) {
+    PyObject *argstuple;
     PyObject *result;
-    PyObject *args = PyTuple_New(1);
-    if (unlikely(!args)) return NULL;
-    Py_INCREF(arg);
-    PyTuple_SET_ITEM(args, 0, arg);
-    result = __Pyx_PyObject_Call(func, args, NULL);
-    Py_DECREF(args);
+    size_t i;
+    argstuple = PyTuple_New((Py_ssize_t)nargs);
+    if (unlikely(!argstuple)) return NULL;
+    for (i = 0; i < nargs; i++) {
+        Py_INCREF(args[i]);
+        PyTuple_SET_ITEM(argstuple, (Py_ssize_t)i, args[i]);
+    }
+    result = __Pyx_PyObject_Call(func, argstuple, kwargs);
+    Py_DECREF(argstuple);
     return result;
 }
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg) {
-#if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(func)) {
-        return __Pyx_PyFunction_FastCall(func, &arg, 1);
-    }
+static CYTHON_INLINE PyObject* __Pyx_PyObject_FastCallDict(PyObject *func, PyObject **args, size_t _nargs, PyObject *kwargs) {
+    Py_ssize_t nargs = __Pyx_PyVectorcall_NARGS(_nargs);
+#if CYTHON_COMPILING_IN_CPYTHON
+    if (nargs == 0 && kwargs == NULL) {
+#if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
+        if (__Pyx_IsCyOrPyCFunction(func))
+#else
+        if (PyCFunction_Check(func))
 #endif
-    if (likely(PyCFunction_Check(func))) {
-        if (likely(PyCFunction_GET_FLAGS(func) & METH_O)) {
-            return __Pyx_PyObject_CallMethO(func, arg);
-#if CYTHON_FAST_PYCCALL
-        } else if (__Pyx_PyFastCFunction_Check(func)) {
-            return __Pyx_PyCFunction_FastCall(func, &arg, 1);
+        {
+            if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
+                return __Pyx_PyObject_CallMethO(func, NULL);
+            }
+        }
+    }
+    else if (nargs == 1 && kwargs == NULL) {
+        if (PyCFunction_Check(func))
+        {
+            if (likely(PyCFunction_GET_FLAGS(func) & METH_O)) {
+                return __Pyx_PyObject_CallMethO(func, args[0]);
+            }
+        }
+    }
 #endif
+    #if PY_VERSION_HEX < 0x030800B1
+    #if CYTHON_FAST_PYCCALL
+    if (PyCFunction_Check(func)) {
+        if (kwargs) {
+            return _PyCFunction_FastCallDict(func, args, nargs, kwargs);
+        } else {
+            return _PyCFunction_FastCallKeywords(func, args, nargs, NULL);
         }
     }
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
+    #if PY_VERSION_HEX >= 0x030700A1
+    if (!kwargs && __Pyx_IS_TYPE(func, &PyMethodDescr_Type)) {
+        return _PyMethodDescr_FastCallKeywords(func, args, nargs, NULL);
+    }
+    #endif
+    #endif
+    #if CYTHON_FAST_PYCALL
+    if (PyFunction_Check(func)) {
+        return __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs);
+    }
+    #endif
+    #endif
+    #if CYTHON_VECTORCALL
+    vectorcallfunc f = _PyVectorcall_Function(func);
+    if (f) {
+        return f(func, args, (size_t)nargs, kwargs);
+    }
+    #elif defined(__Pyx_CyFunction_USED) && CYTHON_BACKPORT_VECTORCALL
+    if (__Pyx_CyFunction_CheckExact(func)) {
+        __pyx_vectorcallfunc f = __Pyx_CyFunction_func_vectorcall(func);
+        if (f) return f(func, args, (size_t)nargs, kwargs);
+    }
+    #endif
+    if (nargs == 0) {
+        return __Pyx_PyObject_Call(func, __pyx_empty_tuple, kwargs);
+    }
+    return __Pyx_PyObject_FastCall_fallback(func, args, (size_t)nargs, kwargs);
 }
-#endif
 
 /* ArgTypeTest */
 static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact)
 {
+    __Pyx_TypeName type_name;
+    __Pyx_TypeName obj_type_name;
     if (unlikely(!type)) {
         PyErr_SetString(PyExc_SystemError, "Missing type object");
         return 0;
     }
     else if (exact) {
         #if PY_MAJOR_VERSION == 2
         if ((type == &PyBaseString_Type) && likely(__Pyx_PyBaseString_CheckExact(obj))) return 1;
         #endif
     }
     else {
         if (likely(__Pyx_TypeCheck(obj, type))) return 1;
     }
+    type_name = __Pyx_PyType_GetName(type);
+    obj_type_name = __Pyx_PyType_GetName(Py_TYPE(obj));
     PyErr_Format(PyExc_TypeError,
-        "Argument '%.200s' has incorrect type (expected %.200s, got %.200s)",
-        name, type->tp_name, Py_TYPE(obj)->tp_name);
+        "Argument '%.200s' has incorrect type (expected " __Pyx_FMT_TYPENAME
+        ", got " __Pyx_FMT_TYPENAME ")", name, type_name, obj_type_name);
+    __Pyx_DECREF_TypeName(type_name);
+    __Pyx_DECREF_TypeName(obj_type_name);
     return 0;
 }
 
 /* IsLittleEndian */
 static CYTHON_INLINE int __Pyx_Is_Little_Endian(void)
 {
   union {
@@ -6840,15 +9433,15 @@
     case 'd': return (is_complex ? "'complex double'" : "'double'");
     case 'g': return (is_complex ? "'complex long double'" : "'long double'");
     case 'T': return "a struct";
     case 'O': return "Python object";
     case 'P': return "a pointer";
     case 's': case 'p': return "a string";
     case 0: return "end";
-    default: return "unparseable format string";
+    default: return "unparsable format string";
   }
 }
 static size_t __Pyx_BufFmt_TypeCharToStandardSize(char ch, int is_complex) {
   switch (ch) {
     case '?': case 'c': case 'b': case 'B': case 's': case 'p': return 1;
     case 'h': case 'H': return 2;
     case 'i': case 'I': case 'l': case 'L': return 4;
@@ -6890,15 +9483,16 @@
 typedef struct { char c; float x; } __Pyx_st_float;
 typedef struct { char c; double x; } __Pyx_st_double;
 typedef struct { char c; long double x; } __Pyx_st_longdouble;
 typedef struct { char c; void *x; } __Pyx_st_void_p;
 #ifdef HAVE_LONG_LONG
 typedef struct { char c; PY_LONG_LONG x; } __Pyx_st_longlong;
 #endif
-static size_t __Pyx_BufFmt_TypeCharToAlignment(char ch, CYTHON_UNUSED int is_complex) {
+static size_t __Pyx_BufFmt_TypeCharToAlignment(char ch, int is_complex) {
+  CYTHON_UNUSED_VAR(is_complex);
   switch (ch) {
     case '?': case 'c': case 'b': case 'B': case 's': case 'p': return 1;
     case 'h': case 'H': return sizeof(__Pyx_st_short) - sizeof(short);
     case 'i': case 'I': return sizeof(__Pyx_st_int) - sizeof(int);
     case 'l': case 'L': return sizeof(__Pyx_st_long) - sizeof(long);
 #ifdef HAVE_LONG_LONG
     case 'q': case 'Q': return sizeof(__Pyx_st_longlong) - sizeof(PY_LONG_LONG);
@@ -6922,15 +9516,16 @@
 typedef struct { float x; char c; } __Pyx_pad_float;
 typedef struct { double x; char c; } __Pyx_pad_double;
 typedef struct { long double x; char c; } __Pyx_pad_longdouble;
 typedef struct { void *x; char c; } __Pyx_pad_void_p;
 #ifdef HAVE_LONG_LONG
 typedef struct { PY_LONG_LONG x; char c; } __Pyx_pad_longlong;
 #endif
-static size_t __Pyx_BufFmt_TypeCharToPadding(char ch, CYTHON_UNUSED int is_complex) {
+static size_t __Pyx_BufFmt_TypeCharToPadding(char ch, int is_complex) {
+  CYTHON_UNUSED_VAR(is_complex);
   switch (ch) {
     case '?': case 'c': case 'b': case 'B': case 's': case 'p': return 1;
     case 'h': case 'H': return sizeof(__Pyx_pad_short) - sizeof(short);
     case 'i': case 'I': return sizeof(__Pyx_pad_int) - sizeof(int);
     case 'l': case 'L': return sizeof(__Pyx_pad_long) - sizeof(long);
 #ifdef HAVE_LONG_LONG
     case 'q': case 'Q': return sizeof(__Pyx_pad_longlong) - sizeof(PY_LONG_LONG);
@@ -7315,22 +9910,29 @@
 fail:;
   __Pyx_SafeReleaseBuffer(buf);
   return -1;
 }
 
 /* ExtTypeTest */
   static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type) {
+    __Pyx_TypeName obj_type_name;
+    __Pyx_TypeName type_name;
     if (unlikely(!type)) {
         PyErr_SetString(PyExc_SystemError, "Missing type object");
         return 0;
     }
     if (likely(__Pyx_TypeCheck(obj, type)))
         return 1;
-    PyErr_Format(PyExc_TypeError, "Cannot convert %.200s to %.200s",
-                 Py_TYPE(obj)->tp_name, type->tp_name);
+    obj_type_name = __Pyx_PyType_GetName(Py_TYPE(obj));
+    type_name = __Pyx_PyType_GetName(type);
+    PyErr_Format(PyExc_TypeError,
+                 "Cannot convert " __Pyx_FMT_TYPENAME " to " __Pyx_FMT_TYPENAME,
+                 obj_type_name, type_name);
+    __Pyx_DECREF_TypeName(obj_type_name);
+    __Pyx_DECREF_TypeName(type_name);
     return 0;
 }
 
 /* BufferFallbackError */
   static void __Pyx_RaiseBufferFallbackError(void) {
   PyErr_SetString(PyExc_ValueError,
      "Buffer acquisition failed on assignment; and then reacquiring the old buffer failed too!");
@@ -7338,542 +9940,81 @@
 
 /* BufferIndexError */
   static void __Pyx_RaiseBufferIndexError(int axis) {
   PyErr_Format(PyExc_IndexError,
      "Out of bounds on buffer access (axis %d)", axis);
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
-/* RaiseArgTupleInvalid */
-  static void __Pyx_RaiseArgtupleInvalid(
-    const char* func_name,
-    int exact,
-    Py_ssize_t num_min,
-    Py_ssize_t num_max,
-    Py_ssize_t num_found)
-{
-    Py_ssize_t num_expected;
-    const char *more_or_less;
-    if (num_found < num_min) {
-        num_expected = num_min;
-        more_or_less = "at least";
-    } else {
-        num_expected = num_max;
-        more_or_less = "at most";
-    }
-    if (exact) {
-        more_or_less = "exactly";
-    }
-    PyErr_Format(PyExc_TypeError,
-                 "%.200s() takes %.8s %" CYTHON_FORMAT_SSIZE_T "d positional argument%.1s (%" CYTHON_FORMAT_SSIZE_T "d given)",
-                 func_name, more_or_less, num_expected,
-                 (num_expected == 1) ? "" : "s", num_found);
-}
-
-/* RaiseDoubleKeywords */
-  static void __Pyx_RaiseDoubleKeywordsError(
-    const char* func_name,
-    PyObject* kw_name)
-{
-    PyErr_Format(PyExc_TypeError,
-        #if PY_MAJOR_VERSION >= 3
-        "%s() got multiple values for keyword argument '%U'", func_name, kw_name);
-        #else
-        "%s() got multiple values for keyword argument '%s'", func_name,
-        PyString_AsString(kw_name));
-        #endif
-}
-
-/* ParseKeywords */
-  static int __Pyx_ParseOptionalKeywords(
-    PyObject *kwds,
-    PyObject **argnames[],
-    PyObject *kwds2,
-    PyObject *values[],
-    Py_ssize_t num_pos_args,
-    const char* function_name)
-{
-    PyObject *key = 0, *value = 0;
-    Py_ssize_t pos = 0;
-    PyObject*** name;
-    PyObject*** first_kw_arg = argnames + num_pos_args;
-    while (PyDict_Next(kwds, &pos, &key, &value)) {
-        name = first_kw_arg;
-        while (*name && (**name != key)) name++;
-        if (*name) {
-            values[name-argnames] = value;
-            continue;
-        }
-        name = first_kw_arg;
-        #if PY_MAJOR_VERSION < 3
-        if (likely(PyString_Check(key))) {
-            while (*name) {
-                if ((CYTHON_COMPILING_IN_PYPY || PyString_GET_SIZE(**name) == PyString_GET_SIZE(key))
-                        && _PyString_Eq(**name, key)) {
-                    values[name-argnames] = value;
-                    break;
-                }
-                name++;
-            }
-            if (*name) continue;
-            else {
-                PyObject*** argname = argnames;
-                while (argname != first_kw_arg) {
-                    if ((**argname == key) || (
-                            (CYTHON_COMPILING_IN_PYPY || PyString_GET_SIZE(**argname) == PyString_GET_SIZE(key))
-                             && _PyString_Eq(**argname, key))) {
-                        goto arg_passed_twice;
-                    }
-                    argname++;
-                }
-            }
-        } else
-        #endif
-        if (likely(PyUnicode_Check(key))) {
-            while (*name) {
-                int cmp = (**name == key) ? 0 :
-                #if !CYTHON_COMPILING_IN_PYPY && PY_MAJOR_VERSION >= 3
-                    (__Pyx_PyUnicode_GET_LENGTH(**name) != __Pyx_PyUnicode_GET_LENGTH(key)) ? 1 :
-                #endif
-                    PyUnicode_Compare(**name, key);
-                if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
-                if (cmp == 0) {
-                    values[name-argnames] = value;
-                    break;
-                }
-                name++;
-            }
-            if (*name) continue;
-            else {
-                PyObject*** argname = argnames;
-                while (argname != first_kw_arg) {
-                    int cmp = (**argname == key) ? 0 :
-                    #if !CYTHON_COMPILING_IN_PYPY && PY_MAJOR_VERSION >= 3
-                        (__Pyx_PyUnicode_GET_LENGTH(**argname) != __Pyx_PyUnicode_GET_LENGTH(key)) ? 1 :
-                    #endif
-                        PyUnicode_Compare(**argname, key);
-                    if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
-                    if (cmp == 0) goto arg_passed_twice;
-                    argname++;
-                }
-            }
-        } else
-            goto invalid_keyword_type;
-        if (kwds2) {
-            if (unlikely(PyDict_SetItem(kwds2, key, value))) goto bad;
-        } else {
-            goto invalid_keyword;
-        }
-    }
-    return 0;
-arg_passed_twice:
-    __Pyx_RaiseDoubleKeywordsError(function_name, key);
-    goto bad;
-invalid_keyword_type:
-    PyErr_Format(PyExc_TypeError,
-        "%.200s() keywords must be strings", function_name);
-    goto bad;
-invalid_keyword:
-    PyErr_Format(PyExc_TypeError,
-    #if PY_MAJOR_VERSION < 3
-        "%.200s() got an unexpected keyword argument '%.200s'",
-        function_name, PyString_AsString(key));
-    #else
-        "%s() got an unexpected keyword argument '%U'",
-        function_name, key);
-    #endif
-bad:
-    return -1;
-}
-
-/* GetTopmostException */
-  #if CYTHON_USE_EXC_INFO_STACK
-static _PyErr_StackItem *
-__Pyx_PyErr_GetTopmostException(PyThreadState *tstate)
-{
-    _PyErr_StackItem *exc_info = tstate->exc_info;
-    while ((exc_info->exc_type == NULL || exc_info->exc_type == Py_None) &&
-           exc_info->previous_item != NULL)
-    {
-        exc_info = exc_info->previous_item;
-    }
-    return exc_info;
-}
-#endif
-
-/* SaveResetException */
-  #if CYTHON_FAST_THREAD_STATE
-static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
-    #if CYTHON_USE_EXC_INFO_STACK
-    _PyErr_StackItem *exc_info = __Pyx_PyErr_GetTopmostException(tstate);
-    *type = exc_info->exc_type;
-    *value = exc_info->exc_value;
-    *tb = exc_info->exc_traceback;
-    #else
-    *type = tstate->exc_type;
-    *value = tstate->exc_value;
-    *tb = tstate->exc_traceback;
-    #endif
-    Py_XINCREF(*type);
-    Py_XINCREF(*value);
-    Py_XINCREF(*tb);
-}
-static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
-    PyObject *tmp_type, *tmp_value, *tmp_tb;
-    #if CYTHON_USE_EXC_INFO_STACK
-    _PyErr_StackItem *exc_info = tstate->exc_info;
-    tmp_type = exc_info->exc_type;
-    tmp_value = exc_info->exc_value;
-    tmp_tb = exc_info->exc_traceback;
-    exc_info->exc_type = type;
-    exc_info->exc_value = value;
-    exc_info->exc_traceback = tb;
-    #else
-    tmp_type = tstate->exc_type;
-    tmp_value = tstate->exc_value;
-    tmp_tb = tstate->exc_traceback;
-    tstate->exc_type = type;
-    tstate->exc_value = value;
-    tstate->exc_traceback = tb;
-    #endif
-    Py_XDECREF(tmp_type);
-    Py_XDECREF(tmp_value);
-    Py_XDECREF(tmp_tb);
-}
-#endif
-
-/* PyErrExceptionMatches */
-  #if CYTHON_FAST_THREAD_STATE
-static int __Pyx_PyErr_ExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
-    Py_ssize_t i, n;
-    n = PyTuple_GET_SIZE(tuple);
-#if PY_MAJOR_VERSION >= 3
-    for (i=0; i<n; i++) {
-        if (exc_type == PyTuple_GET_ITEM(tuple, i)) return 1;
-    }
-#endif
-    for (i=0; i<n; i++) {
-        if (__Pyx_PyErr_GivenExceptionMatches(exc_type, PyTuple_GET_ITEM(tuple, i))) return 1;
-    }
-    return 0;
-}
-static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err) {
-    PyObject *exc_type = tstate->curexc_type;
-    if (exc_type == err) return 1;
-    if (unlikely(!exc_type)) return 0;
-    if (unlikely(PyTuple_Check(err)))
-        return __Pyx_PyErr_ExceptionMatchesTuple(exc_type, err);
-    return __Pyx_PyErr_GivenExceptionMatches(exc_type, err);
-}
-#endif
-
-/* GetException */
-  #if CYTHON_FAST_THREAD_STATE
-static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb)
-#else
-static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb)
-#endif
-{
-    PyObject *local_type, *local_value, *local_tb;
-#if CYTHON_FAST_THREAD_STATE
-    PyObject *tmp_type, *tmp_value, *tmp_tb;
-    local_type = tstate->curexc_type;
-    local_value = tstate->curexc_value;
-    local_tb = tstate->curexc_traceback;
-    tstate->curexc_type = 0;
-    tstate->curexc_value = 0;
-    tstate->curexc_traceback = 0;
-#else
-    PyErr_Fetch(&local_type, &local_value, &local_tb);
-#endif
-    PyErr_NormalizeException(&local_type, &local_value, &local_tb);
-#if CYTHON_FAST_THREAD_STATE
-    if (unlikely(tstate->curexc_type))
-#else
-    if (unlikely(PyErr_Occurred()))
-#endif
-        goto bad;
-    #if PY_MAJOR_VERSION >= 3
-    if (local_tb) {
-        if (unlikely(PyException_SetTraceback(local_value, local_tb) < 0))
-            goto bad;
-    }
-    #endif
-    Py_XINCREF(local_tb);
-    Py_XINCREF(local_type);
-    Py_XINCREF(local_value);
-    *type = local_type;
-    *value = local_value;
-    *tb = local_tb;
-#if CYTHON_FAST_THREAD_STATE
-    #if CYTHON_USE_EXC_INFO_STACK
-    {
-        _PyErr_StackItem *exc_info = tstate->exc_info;
-        tmp_type = exc_info->exc_type;
-        tmp_value = exc_info->exc_value;
-        tmp_tb = exc_info->exc_traceback;
-        exc_info->exc_type = local_type;
-        exc_info->exc_value = local_value;
-        exc_info->exc_traceback = local_tb;
-    }
-    #else
-    tmp_type = tstate->exc_type;
-    tmp_value = tstate->exc_value;
-    tmp_tb = tstate->exc_traceback;
-    tstate->exc_type = local_type;
-    tstate->exc_value = local_value;
-    tstate->exc_traceback = local_tb;
-    #endif
-    Py_XDECREF(tmp_type);
-    Py_XDECREF(tmp_value);
-    Py_XDECREF(tmp_tb);
-#else
-    PyErr_SetExcInfo(local_type, local_value, local_tb);
-#endif
-    return 0;
-bad:
-    *type = 0;
-    *value = 0;
-    *tb = 0;
-    Py_XDECREF(local_type);
-    Py_XDECREF(local_value);
-    Py_XDECREF(local_tb);
-    return -1;
-}
-
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
 /* TypeImport */
-  #ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+  #ifndef __PYX_HAVE_RT_ImportType_3_0_0
+#define __PYX_HAVE_RT_ImportType_3_0_0
+static PyTypeObject *__Pyx_ImportType_3_0_0(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_0 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
-#ifdef Py_LIMITED_API
+    Py_ssize_t itemsize;
+#if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
-#ifndef Py_LIMITED_API
+#if !CYTHON_COMPILING_IN_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
-            module_name, class_name, size, basicsize);
+            module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_0 &&
+            ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
-            "Expected %zd from C header, got %zd from PyObject",
-            module_name, class_name, size, basicsize);
+            "Expected %zd from C header, got %zd-%zd from PyObject",
+            module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_0 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -7881,99 +10022,1353 @@
     Py_XDECREF(result);
     return NULL;
 }
 #endif
 
 /* Import */
   static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level) {
-    PyObject *empty_list = 0;
     PyObject *module = 0;
-    PyObject *global_dict = 0;
     PyObject *empty_dict = 0;
-    PyObject *list;
+    PyObject *empty_list = 0;
     #if PY_MAJOR_VERSION < 3
     PyObject *py_import;
     py_import = __Pyx_PyObject_GetAttrStr(__pyx_b, __pyx_n_s_import);
-    if (!py_import)
+    if (unlikely(!py_import))
         goto bad;
-    #endif
-    if (from_list)
-        list = from_list;
-    else {
+    if (!from_list) {
         empty_list = PyList_New(0);
-        if (!empty_list)
+        if (unlikely(!empty_list))
             goto bad;
-        list = empty_list;
+        from_list = empty_list;
     }
-    global_dict = PyModule_GetDict(__pyx_m);
-    if (!global_dict)
-        goto bad;
+    #endif
     empty_dict = PyDict_New();
-    if (!empty_dict)
+    if (unlikely(!empty_dict))
         goto bad;
     {
         #if PY_MAJOR_VERSION >= 3
         if (level == -1) {
             if ((1) && (strchr(__Pyx_MODULE_NAME, '.'))) {
+                #if CYTHON_COMPILING_IN_LIMITED_API
+                module = PyImport_ImportModuleLevelObject(
+                    name, empty_dict, empty_dict, from_list, 1);
+                #else
                 module = PyImport_ImportModuleLevelObject(
-                    name, global_dict, empty_dict, list, 1);
-                if (!module) {
-                    if (!PyErr_ExceptionMatches(PyExc_ImportError))
+                    name, __pyx_d, empty_dict, from_list, 1);
+                #endif
+                if (unlikely(!module)) {
+                    if (unlikely(!PyErr_ExceptionMatches(PyExc_ImportError)))
                         goto bad;
                     PyErr_Clear();
                 }
             }
             level = 0;
         }
         #endif
         if (!module) {
             #if PY_MAJOR_VERSION < 3
             PyObject *py_level = PyInt_FromLong(level);
-            if (!py_level)
+            if (unlikely(!py_level))
                 goto bad;
             module = PyObject_CallFunctionObjArgs(py_import,
-                name, global_dict, empty_dict, list, py_level, (PyObject *)NULL);
+                name, __pyx_d, empty_dict, from_list, py_level, (PyObject *)NULL);
             Py_DECREF(py_level);
             #else
+            #if CYTHON_COMPILING_IN_LIMITED_API
+            module = PyImport_ImportModuleLevelObject(
+                name, empty_dict, empty_dict, from_list, level);
+            #else
             module = PyImport_ImportModuleLevelObject(
-                name, global_dict, empty_dict, list, level);
+                name, __pyx_d, empty_dict, from_list, level);
+            #endif
             #endif
         }
     }
 bad:
+    Py_XDECREF(empty_dict);
+    Py_XDECREF(empty_list);
     #if PY_MAJOR_VERSION < 3
     Py_XDECREF(py_import);
     #endif
-    Py_XDECREF(empty_list);
-    Py_XDECREF(empty_dict);
     return module;
 }
 
+/* ImportDottedModule */
+  #if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx__ImportDottedModule_Error(PyObject *name, PyObject *parts_tuple, Py_ssize_t count) {
+    PyObject *partial_name = NULL, *slice = NULL, *sep = NULL;
+    if (unlikely(PyErr_Occurred())) {
+        PyErr_Clear();
+    }
+    if (likely(PyTuple_GET_SIZE(parts_tuple) == count)) {
+        partial_name = name;
+    } else {
+        slice = PySequence_GetSlice(parts_tuple, 0, count);
+        if (unlikely(!slice))
+            goto bad;
+        sep = PyUnicode_FromStringAndSize(".", 1);
+        if (unlikely(!sep))
+            goto bad;
+        partial_name = PyUnicode_Join(sep, slice);
+    }
+    PyErr_Format(
+#if PY_MAJOR_VERSION < 3
+        PyExc_ImportError,
+        "No module named '%s'", PyString_AS_STRING(partial_name));
+#else
+#if PY_VERSION_HEX >= 0x030600B1
+        PyExc_ModuleNotFoundError,
+#else
+        PyExc_ImportError,
+#endif
+        "No module named '%U'", partial_name);
+#endif
+bad:
+    Py_XDECREF(sep);
+    Py_XDECREF(slice);
+    Py_XDECREF(partial_name);
+    return NULL;
+}
+#endif
+#if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx__ImportDottedModule_Lookup(PyObject *name) {
+    PyObject *imported_module;
+#if PY_VERSION_HEX < 0x030700A1 || (CYTHON_COMPILING_IN_PYPY && PYPY_VERSION_NUM  < 0x07030400)
+    PyObject *modules = PyImport_GetModuleDict();
+    if (unlikely(!modules))
+        return NULL;
+    imported_module = __Pyx_PyDict_GetItemStr(modules, name);
+    Py_XINCREF(imported_module);
+#else
+    imported_module = PyImport_GetModule(name);
+#endif
+    return imported_module;
+}
+#endif
+#if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx_ImportDottedModule_WalkParts(PyObject *module, PyObject *name, PyObject *parts_tuple) {
+    Py_ssize_t i, nparts;
+    nparts = PyTuple_GET_SIZE(parts_tuple);
+    for (i=1; i < nparts && module; i++) {
+        PyObject *part, *submodule;
+#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        part = PyTuple_GET_ITEM(parts_tuple, i);
+#else
+        part = PySequence_ITEM(parts_tuple, i);
+#endif
+        submodule = __Pyx_PyObject_GetAttrStrNoError(module, part);
+#if !(CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS)
+        Py_DECREF(part);
+#endif
+        Py_DECREF(module);
+        module = submodule;
+    }
+    if (unlikely(!module)) {
+        return __Pyx__ImportDottedModule_Error(name, parts_tuple, i);
+    }
+    return module;
+}
+#endif
+static PyObject *__Pyx__ImportDottedModule(PyObject *name, PyObject *parts_tuple) {
+#if PY_MAJOR_VERSION < 3
+    PyObject *module, *from_list, *star = __pyx_n_s__3;
+    CYTHON_UNUSED_VAR(parts_tuple);
+    from_list = PyList_New(1);
+    if (unlikely(!from_list))
+        return NULL;
+    Py_INCREF(star);
+    PyList_SET_ITEM(from_list, 0, star);
+    module = __Pyx_Import(name, from_list, 0);
+    Py_DECREF(from_list);
+    return module;
+#else
+    PyObject *imported_module;
+    PyObject *module = __Pyx_Import(name, NULL, 0);
+    if (!parts_tuple || unlikely(!module))
+        return module;
+    imported_module = __Pyx__ImportDottedModule_Lookup(name);
+    if (likely(imported_module)) {
+        Py_DECREF(module);
+        return imported_module;
+    }
+    PyErr_Clear();
+    return __Pyx_ImportDottedModule_WalkParts(module, name, parts_tuple);
+#endif
+}
+static PyObject *__Pyx_ImportDottedModule(PyObject *name, PyObject *parts_tuple) {
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030400B1
+    PyObject *module = __Pyx__ImportDottedModule_Lookup(name);
+    if (likely(module)) {
+        PyObject *spec = __Pyx_PyObject_GetAttrStrNoError(module, __pyx_n_s_spec);
+        if (likely(spec)) {
+            PyObject *unsafe = __Pyx_PyObject_GetAttrStrNoError(spec, __pyx_n_s_initializing);
+            if (likely(!unsafe || !__Pyx_PyObject_IsTrue(unsafe))) {
+                Py_DECREF(spec);
+                spec = NULL;
+            }
+            Py_XDECREF(unsafe);
+        }
+        if (likely(!spec)) {
+            PyErr_Clear();
+            return module;
+        }
+        Py_DECREF(spec);
+        Py_DECREF(module);
+    } else if (PyErr_Occurred()) {
+        PyErr_Clear();
+    }
+#endif
+    return __Pyx__ImportDottedModule(name, parts_tuple);
+}
+
+/* FixUpExtensionType */
+  #if CYTHON_USE_TYPE_SPECS
+static int __Pyx_fix_up_extension_type_from_spec(PyType_Spec *spec, PyTypeObject *type) {
+#if PY_VERSION_HEX > 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
+    CYTHON_UNUSED_VAR(spec);
+    CYTHON_UNUSED_VAR(type);
+#else
+    const PyType_Slot *slot = spec->slots;
+    while (slot && slot->slot && slot->slot != Py_tp_members)
+        slot++;
+    if (slot && slot->slot == Py_tp_members) {
+        int changed = 0;
+#if !(PY_VERSION_HEX <= 0x030900b1 && CYTHON_COMPILING_IN_CPYTHON)
+        const
+#endif
+            PyMemberDef *memb = (PyMemberDef*) slot->pfunc;
+        while (memb && memb->name) {
+            if (memb->name[0] == '_' && memb->name[1] == '_') {
+#if PY_VERSION_HEX < 0x030900b1
+                if (strcmp(memb->name, "__weaklistoffset__") == 0) {
+                    assert(memb->type == T_PYSSIZET);
+                    assert(memb->flags == READONLY);
+                    type->tp_weaklistoffset = memb->offset;
+                    changed = 1;
+                }
+                else if (strcmp(memb->name, "__dictoffset__") == 0) {
+                    assert(memb->type == T_PYSSIZET);
+                    assert(memb->flags == READONLY);
+                    type->tp_dictoffset = memb->offset;
+                    changed = 1;
+                }
+#if CYTHON_METH_FASTCALL
+                else if (strcmp(memb->name, "__vectorcalloffset__") == 0) {
+                    assert(memb->type == T_PYSSIZET);
+                    assert(memb->flags == READONLY);
+#if PY_VERSION_HEX >= 0x030800b4
+                    type->tp_vectorcall_offset = memb->offset;
+#else
+                    type->tp_print = (printfunc) memb->offset;
+#endif
+                    changed = 1;
+                }
+#endif
+#else
+                if ((0));
+#endif
+#if PY_VERSION_HEX <= 0x030900b1 && CYTHON_COMPILING_IN_CPYTHON
+                else if (strcmp(memb->name, "__module__") == 0) {
+                    PyObject *descr;
+                    assert(memb->type == T_OBJECT);
+                    assert(memb->flags == 0 || memb->flags == READONLY);
+                    descr = PyDescr_NewMember(type, memb);
+                    if (unlikely(!descr))
+                        return -1;
+                    if (unlikely(PyDict_SetItem(type->tp_dict, PyDescr_NAME(descr), descr) < 0)) {
+                        Py_DECREF(descr);
+                        return -1;
+                    }
+                    Py_DECREF(descr);
+                    changed = 1;
+                }
+#endif
+            }
+            memb++;
+        }
+        if (changed)
+            PyType_Modified(type);
+    }
+#endif
+    return 0;
+}
+#endif
+
+/* FetchSharedCythonModule */
+  static PyObject *__Pyx_FetchSharedCythonABIModule(void) {
+    PyObject *abi_module = PyImport_AddModule((char*) __PYX_ABI_MODULE_NAME);
+    if (unlikely(!abi_module)) return NULL;
+    Py_INCREF(abi_module);
+    return abi_module;
+}
+
+/* FetchCommonType */
+  static int __Pyx_VerifyCachedType(PyObject *cached_type,
+                               const char *name,
+                               Py_ssize_t basicsize,
+                               Py_ssize_t expected_basicsize) {
+    if (!PyType_Check(cached_type)) {
+        PyErr_Format(PyExc_TypeError,
+            "Shared Cython type %.200s is not a type object", name);
+        return -1;
+    }
+    if (basicsize != expected_basicsize) {
+        PyErr_Format(PyExc_TypeError,
+            "Shared Cython type %.200s has the wrong size, try recompiling",
+            name);
+        return -1;
+    }
+    return 0;
+}
+#if !CYTHON_USE_TYPE_SPECS
+static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type) {
+    PyObject* abi_module;
+    const char* object_name;
+    PyTypeObject *cached_type = NULL;
+    abi_module = __Pyx_FetchSharedCythonABIModule();
+    if (!abi_module) return NULL;
+    object_name = strrchr(type->tp_name, '.');
+    object_name = object_name ? object_name+1 : type->tp_name;
+    cached_type = (PyTypeObject*) PyObject_GetAttrString(abi_module, object_name);
+    if (cached_type) {
+        if (__Pyx_VerifyCachedType(
+              (PyObject *)cached_type,
+              object_name,
+              cached_type->tp_basicsize,
+              type->tp_basicsize) < 0) {
+            goto bad;
+        }
+        goto done;
+    }
+    if (!PyErr_ExceptionMatches(PyExc_AttributeError)) goto bad;
+    PyErr_Clear();
+    if (PyType_Ready(type) < 0) goto bad;
+    if (PyObject_SetAttrString(abi_module, object_name, (PyObject *)type) < 0)
+        goto bad;
+    Py_INCREF(type);
+    cached_type = type;
+done:
+    Py_DECREF(abi_module);
+    return cached_type;
+bad:
+    Py_XDECREF(cached_type);
+    cached_type = NULL;
+    goto done;
+}
+#else
+static PyTypeObject *__Pyx_FetchCommonTypeFromSpec(PyObject *module, PyType_Spec *spec, PyObject *bases) {
+    PyObject *abi_module, *cached_type = NULL;
+    const char* object_name = strrchr(spec->name, '.');
+    object_name = object_name ? object_name+1 : spec->name;
+    abi_module = __Pyx_FetchSharedCythonABIModule();
+    if (!abi_module) return NULL;
+    cached_type = PyObject_GetAttrString(abi_module, object_name);
+    if (cached_type) {
+        Py_ssize_t basicsize;
+#if CYTHON_COMPILING_IN_LIMITED_API
+        PyObject *py_basicsize;
+        py_basicsize = PyObject_GetAttrString(cached_type, "__basicsize__");
+        if (unlikely(!py_basicsize)) goto bad;
+        basicsize = PyLong_AsSsize_t(py_basicsize);
+        Py_DECREF(py_basicsize);
+        py_basicsize = 0;
+        if (unlikely(basicsize == (Py_ssize_t)-1) && PyErr_Occurred()) goto bad;
+#else
+        basicsize = likely(PyType_Check(cached_type)) ? ((PyTypeObject*) cached_type)->tp_basicsize : -1;
+#endif
+        if (__Pyx_VerifyCachedType(
+              cached_type,
+              object_name,
+              basicsize,
+              spec->basicsize) < 0) {
+            goto bad;
+        }
+        goto done;
+    }
+    if (!PyErr_ExceptionMatches(PyExc_AttributeError)) goto bad;
+    PyErr_Clear();
+    CYTHON_UNUSED_VAR(module);
+    cached_type = __Pyx_PyType_FromModuleAndSpec(abi_module, spec, bases);
+    if (unlikely(!cached_type)) goto bad;
+    if (unlikely(__Pyx_fix_up_extension_type_from_spec(spec, (PyTypeObject *) cached_type) < 0)) goto bad;
+    if (PyObject_SetAttrString(abi_module, object_name, cached_type) < 0) goto bad;
+done:
+    Py_DECREF(abi_module);
+    assert(cached_type == NULL || PyType_Check(cached_type));
+    return (PyTypeObject *) cached_type;
+bad:
+    Py_XDECREF(cached_type);
+    cached_type = NULL;
+    goto done;
+}
+#endif
+
+/* PyVectorcallFastCallDict */
+  #if CYTHON_METH_FASTCALL
+static PyObject *__Pyx_PyVectorcall_FastCallDict_kw(PyObject *func, __pyx_vectorcallfunc vc, PyObject *const *args, size_t nargs, PyObject *kw)
+{
+    PyObject *res = NULL;
+    PyObject *kwnames;
+    PyObject **newargs;
+    PyObject **kwvalues;
+    Py_ssize_t i, pos;
+    size_t j;
+    PyObject *key, *value;
+    unsigned long keys_are_strings;
+    Py_ssize_t nkw = PyDict_GET_SIZE(kw);
+    newargs = (PyObject **)PyMem_Malloc((nargs + (size_t)nkw) * sizeof(args[0]));
+    if (unlikely(newargs == NULL)) {
+        PyErr_NoMemory();
+        return NULL;
+    }
+    for (j = 0; j < nargs; j++) newargs[j] = args[j];
+    kwnames = PyTuple_New(nkw);
+    if (unlikely(kwnames == NULL)) {
+        PyMem_Free(newargs);
+        return NULL;
+    }
+    kwvalues = newargs + nargs;
+    pos = i = 0;
+    keys_are_strings = Py_TPFLAGS_UNICODE_SUBCLASS;
+    while (PyDict_Next(kw, &pos, &key, &value)) {
+        keys_are_strings &= Py_TYPE(key)->tp_flags;
+        Py_INCREF(key);
+        Py_INCREF(value);
+        PyTuple_SET_ITEM(kwnames, i, key);
+        kwvalues[i] = value;
+        i++;
+    }
+    if (unlikely(!keys_are_strings)) {
+        PyErr_SetString(PyExc_TypeError, "keywords must be strings");
+        goto cleanup;
+    }
+    res = vc(func, newargs, nargs, kwnames);
+cleanup:
+    Py_DECREF(kwnames);
+    for (i = 0; i < nkw; i++)
+        Py_DECREF(kwvalues[i]);
+    PyMem_Free(newargs);
+    return res;
+}
+static CYTHON_INLINE PyObject *__Pyx_PyVectorcall_FastCallDict(PyObject *func, __pyx_vectorcallfunc vc, PyObject *const *args, size_t nargs, PyObject *kw)
+{
+    if (likely(kw == NULL) || PyDict_GET_SIZE(kw) == 0) {
+        return vc(func, args, nargs, NULL);
+    }
+    return __Pyx_PyVectorcall_FastCallDict_kw(func, vc, args, nargs, kw);
+}
+#endif
+
+/* CythonFunctionShared */
+  static CYTHON_INLINE void __Pyx__CyFunction_SetClassObj(__pyx_CyFunctionObject* f, PyObject* classobj) {
+#if PY_VERSION_HEX < 0x030900B1
+    __Pyx_Py_XDECREF_SET(
+        __Pyx_CyFunction_GetClassObj(f),
+            ((classobj) ? __Pyx_NewRef(classobj) : NULL));
+#else
+    __Pyx_Py_XDECREF_SET(
+        ((PyCMethodObject *) (f))->mm_class,
+        (PyTypeObject*)((classobj) ? __Pyx_NewRef(classobj) : NULL));
+#endif
+}
+static PyObject *
+__Pyx_CyFunction_get_doc(__pyx_CyFunctionObject *op, void *closure)
+{
+    CYTHON_UNUSED_VAR(closure);
+    if (unlikely(op->func_doc == NULL)) {
+        if (((PyCFunctionObject*)op)->m_ml->ml_doc) {
+#if PY_MAJOR_VERSION >= 3
+            op->func_doc = PyUnicode_FromString(((PyCFunctionObject*)op)->m_ml->ml_doc);
+#else
+            op->func_doc = PyString_FromString(((PyCFunctionObject*)op)->m_ml->ml_doc);
+#endif
+            if (unlikely(op->func_doc == NULL))
+                return NULL;
+        } else {
+            Py_INCREF(Py_None);
+            return Py_None;
+        }
+    }
+    Py_INCREF(op->func_doc);
+    return op->func_doc;
+}
+static int
+__Pyx_CyFunction_set_doc(__pyx_CyFunctionObject *op, PyObject *value, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    if (value == NULL) {
+        value = Py_None;
+    }
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->func_doc, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_name(__pyx_CyFunctionObject *op, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(op->func_name == NULL)) {
+#if PY_MAJOR_VERSION >= 3
+        op->func_name = PyUnicode_InternFromString(((PyCFunctionObject*)op)->m_ml->ml_name);
+#else
+        op->func_name = PyString_InternFromString(((PyCFunctionObject*)op)->m_ml->ml_name);
+#endif
+        if (unlikely(op->func_name == NULL))
+            return NULL;
+    }
+    Py_INCREF(op->func_name);
+    return op->func_name;
+}
+static int
+__Pyx_CyFunction_set_name(__pyx_CyFunctionObject *op, PyObject *value, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+#if PY_MAJOR_VERSION >= 3
+    if (unlikely(value == NULL || !PyUnicode_Check(value)))
+#else
+    if (unlikely(value == NULL || !PyString_Check(value)))
+#endif
+    {
+        PyErr_SetString(PyExc_TypeError,
+                        "__name__ must be set to a string object");
+        return -1;
+    }
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->func_name, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_qualname(__pyx_CyFunctionObject *op, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    Py_INCREF(op->func_qualname);
+    return op->func_qualname;
+}
+static int
+__Pyx_CyFunction_set_qualname(__pyx_CyFunctionObject *op, PyObject *value, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+#if PY_MAJOR_VERSION >= 3
+    if (unlikely(value == NULL || !PyUnicode_Check(value)))
+#else
+    if (unlikely(value == NULL || !PyString_Check(value)))
+#endif
+    {
+        PyErr_SetString(PyExc_TypeError,
+                        "__qualname__ must be set to a string object");
+        return -1;
+    }
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->func_qualname, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_dict(__pyx_CyFunctionObject *op, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(op->func_dict == NULL)) {
+        op->func_dict = PyDict_New();
+        if (unlikely(op->func_dict == NULL))
+            return NULL;
+    }
+    Py_INCREF(op->func_dict);
+    return op->func_dict;
+}
+static int
+__Pyx_CyFunction_set_dict(__pyx_CyFunctionObject *op, PyObject *value, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(value == NULL)) {
+        PyErr_SetString(PyExc_TypeError,
+               "function's dictionary may not be deleted");
+        return -1;
+    }
+    if (unlikely(!PyDict_Check(value))) {
+        PyErr_SetString(PyExc_TypeError,
+               "setting function's dictionary to a non-dict");
+        return -1;
+    }
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->func_dict, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_globals(__pyx_CyFunctionObject *op, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    Py_INCREF(op->func_globals);
+    return op->func_globals;
+}
+static PyObject *
+__Pyx_CyFunction_get_closure(__pyx_CyFunctionObject *op, void *context)
+{
+    CYTHON_UNUSED_VAR(op);
+    CYTHON_UNUSED_VAR(context);
+    Py_INCREF(Py_None);
+    return Py_None;
+}
+static PyObject *
+__Pyx_CyFunction_get_code(__pyx_CyFunctionObject *op, void *context)
+{
+    PyObject* result = (op->func_code) ? op->func_code : Py_None;
+    CYTHON_UNUSED_VAR(context);
+    Py_INCREF(result);
+    return result;
+}
+static int
+__Pyx_CyFunction_init_defaults(__pyx_CyFunctionObject *op) {
+    int result = 0;
+    PyObject *res = op->defaults_getter((PyObject *) op);
+    if (unlikely(!res))
+        return -1;
+    #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+    op->defaults_tuple = PyTuple_GET_ITEM(res, 0);
+    Py_INCREF(op->defaults_tuple);
+    op->defaults_kwdict = PyTuple_GET_ITEM(res, 1);
+    Py_INCREF(op->defaults_kwdict);
+    #else
+    op->defaults_tuple = PySequence_ITEM(res, 0);
+    if (unlikely(!op->defaults_tuple)) result = -1;
+    else {
+        op->defaults_kwdict = PySequence_ITEM(res, 1);
+        if (unlikely(!op->defaults_kwdict)) result = -1;
+    }
+    #endif
+    Py_DECREF(res);
+    return result;
+}
+static int
+__Pyx_CyFunction_set_defaults(__pyx_CyFunctionObject *op, PyObject* value, void *context) {
+    CYTHON_UNUSED_VAR(context);
+    if (!value) {
+        value = Py_None;
+    } else if (unlikely(value != Py_None && !PyTuple_Check(value))) {
+        PyErr_SetString(PyExc_TypeError,
+                        "__defaults__ must be set to a tuple object");
+        return -1;
+    }
+    PyErr_WarnEx(PyExc_RuntimeWarning, "changes to cyfunction.__defaults__ will not "
+                 "currently affect the values used in function calls", 1);
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->defaults_tuple, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_defaults(__pyx_CyFunctionObject *op, void *context) {
+    PyObject* result = op->defaults_tuple;
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(!result)) {
+        if (op->defaults_getter) {
+            if (unlikely(__Pyx_CyFunction_init_defaults(op) < 0)) return NULL;
+            result = op->defaults_tuple;
+        } else {
+            result = Py_None;
+        }
+    }
+    Py_INCREF(result);
+    return result;
+}
+static int
+__Pyx_CyFunction_set_kwdefaults(__pyx_CyFunctionObject *op, PyObject* value, void *context) {
+    CYTHON_UNUSED_VAR(context);
+    if (!value) {
+        value = Py_None;
+    } else if (unlikely(value != Py_None && !PyDict_Check(value))) {
+        PyErr_SetString(PyExc_TypeError,
+                        "__kwdefaults__ must be set to a dict object");
+        return -1;
+    }
+    PyErr_WarnEx(PyExc_RuntimeWarning, "changes to cyfunction.__kwdefaults__ will not "
+                 "currently affect the values used in function calls", 1);
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->defaults_kwdict, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_kwdefaults(__pyx_CyFunctionObject *op, void *context) {
+    PyObject* result = op->defaults_kwdict;
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(!result)) {
+        if (op->defaults_getter) {
+            if (unlikely(__Pyx_CyFunction_init_defaults(op) < 0)) return NULL;
+            result = op->defaults_kwdict;
+        } else {
+            result = Py_None;
+        }
+    }
+    Py_INCREF(result);
+    return result;
+}
+static int
+__Pyx_CyFunction_set_annotations(__pyx_CyFunctionObject *op, PyObject* value, void *context) {
+    CYTHON_UNUSED_VAR(context);
+    if (!value || value == Py_None) {
+        value = NULL;
+    } else if (unlikely(!PyDict_Check(value))) {
+        PyErr_SetString(PyExc_TypeError,
+                        "__annotations__ must be set to a dict object");
+        return -1;
+    }
+    Py_XINCREF(value);
+    __Pyx_Py_XDECREF_SET(op->func_annotations, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_annotations(__pyx_CyFunctionObject *op, void *context) {
+    PyObject* result = op->func_annotations;
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(!result)) {
+        result = PyDict_New();
+        if (unlikely(!result)) return NULL;
+        op->func_annotations = result;
+    }
+    Py_INCREF(result);
+    return result;
+}
+static PyObject *
+__Pyx_CyFunction_get_is_coroutine(__pyx_CyFunctionObject *op, void *context) {
+    int is_coroutine;
+    CYTHON_UNUSED_VAR(context);
+    if (op->func_is_coroutine) {
+        return __Pyx_NewRef(op->func_is_coroutine);
+    }
+    is_coroutine = op->flags & __Pyx_CYFUNCTION_COROUTINE;
+#if PY_VERSION_HEX >= 0x03050000
+    if (is_coroutine) {
+        PyObject *module, *fromlist, *marker = __pyx_n_s_is_coroutine;
+        fromlist = PyList_New(1);
+        if (unlikely(!fromlist)) return NULL;
+        Py_INCREF(marker);
+        PyList_SET_ITEM(fromlist, 0, marker);
+        module = PyImport_ImportModuleLevelObject(__pyx_n_s_asyncio_coroutines, NULL, NULL, fromlist, 0);
+        Py_DECREF(fromlist);
+        if (unlikely(!module)) goto ignore;
+        op->func_is_coroutine = __Pyx_PyObject_GetAttrStr(module, marker);
+        Py_DECREF(module);
+        if (likely(op->func_is_coroutine)) {
+            return __Pyx_NewRef(op->func_is_coroutine);
+        }
+ignore:
+        PyErr_Clear();
+    }
+#endif
+    op->func_is_coroutine = __Pyx_PyBool_FromLong(is_coroutine);
+    return __Pyx_NewRef(op->func_is_coroutine);
+}
+static PyGetSetDef __pyx_CyFunction_getsets[] = {
+    {(char *) "func_doc", (getter)__Pyx_CyFunction_get_doc, (setter)__Pyx_CyFunction_set_doc, 0, 0},
+    {(char *) "__doc__",  (getter)__Pyx_CyFunction_get_doc, (setter)__Pyx_CyFunction_set_doc, 0, 0},
+    {(char *) "func_name", (getter)__Pyx_CyFunction_get_name, (setter)__Pyx_CyFunction_set_name, 0, 0},
+    {(char *) "__name__", (getter)__Pyx_CyFunction_get_name, (setter)__Pyx_CyFunction_set_name, 0, 0},
+    {(char *) "__qualname__", (getter)__Pyx_CyFunction_get_qualname, (setter)__Pyx_CyFunction_set_qualname, 0, 0},
+    {(char *) "func_dict", (getter)__Pyx_CyFunction_get_dict, (setter)__Pyx_CyFunction_set_dict, 0, 0},
+    {(char *) "__dict__", (getter)__Pyx_CyFunction_get_dict, (setter)__Pyx_CyFunction_set_dict, 0, 0},
+    {(char *) "func_globals", (getter)__Pyx_CyFunction_get_globals, 0, 0, 0},
+    {(char *) "__globals__", (getter)__Pyx_CyFunction_get_globals, 0, 0, 0},
+    {(char *) "func_closure", (getter)__Pyx_CyFunction_get_closure, 0, 0, 0},
+    {(char *) "__closure__", (getter)__Pyx_CyFunction_get_closure, 0, 0, 0},
+    {(char *) "func_code", (getter)__Pyx_CyFunction_get_code, 0, 0, 0},
+    {(char *) "__code__", (getter)__Pyx_CyFunction_get_code, 0, 0, 0},
+    {(char *) "func_defaults", (getter)__Pyx_CyFunction_get_defaults, (setter)__Pyx_CyFunction_set_defaults, 0, 0},
+    {(char *) "__defaults__", (getter)__Pyx_CyFunction_get_defaults, (setter)__Pyx_CyFunction_set_defaults, 0, 0},
+    {(char *) "__kwdefaults__", (getter)__Pyx_CyFunction_get_kwdefaults, (setter)__Pyx_CyFunction_set_kwdefaults, 0, 0},
+    {(char *) "__annotations__", (getter)__Pyx_CyFunction_get_annotations, (setter)__Pyx_CyFunction_set_annotations, 0, 0},
+    {(char *) "_is_coroutine", (getter)__Pyx_CyFunction_get_is_coroutine, 0, 0, 0},
+    {0, 0, 0, 0, 0}
+};
+static PyMemberDef __pyx_CyFunction_members[] = {
+    {(char *) "__module__", T_OBJECT, offsetof(PyCFunctionObject, m_module), 0, 0},
+#if CYTHON_USE_TYPE_SPECS
+    {(char *) "__dictoffset__", T_PYSSIZET, offsetof(__pyx_CyFunctionObject, func_dict), READONLY, 0},
+#if CYTHON_METH_FASTCALL
+#if CYTHON_BACKPORT_VECTORCALL
+    {(char *) "__vectorcalloffset__", T_PYSSIZET, offsetof(__pyx_CyFunctionObject, func_vectorcall), READONLY, 0},
+#else
+    {(char *) "__vectorcalloffset__", T_PYSSIZET, offsetof(PyCFunctionObject, vectorcall), READONLY, 0},
+#endif
+#endif
+#if PY_VERSION_HEX < 0x030500A0
+    {(char *) "__weaklistoffset__", T_PYSSIZET, offsetof(__pyx_CyFunctionObject, func_weakreflist), READONLY, 0},
+#else
+    {(char *) "__weaklistoffset__", T_PYSSIZET, offsetof(PyCFunctionObject, m_weakreflist), READONLY, 0},
+#endif
+#endif
+    {0, 0, 0,  0, 0}
+};
+static PyObject *
+__Pyx_CyFunction_reduce(__pyx_CyFunctionObject *m, PyObject *args)
+{
+    CYTHON_UNUSED_VAR(args);
+#if PY_MAJOR_VERSION >= 3
+    Py_INCREF(m->func_qualname);
+    return m->func_qualname;
+#else
+    return PyString_FromString(((PyCFunctionObject*)m)->m_ml->ml_name);
+#endif
+}
+static PyMethodDef __pyx_CyFunction_methods[] = {
+    {"__reduce__", (PyCFunction)__Pyx_CyFunction_reduce, METH_VARARGS, 0},
+    {0, 0, 0, 0}
+};
+#if PY_VERSION_HEX < 0x030500A0
+#define __Pyx_CyFunction_weakreflist(cyfunc) ((cyfunc)->func_weakreflist)
+#else
+#define __Pyx_CyFunction_weakreflist(cyfunc) (((PyCFunctionObject*)cyfunc)->m_weakreflist)
+#endif
+static PyObject *__Pyx_CyFunction_Init(__pyx_CyFunctionObject *op, PyMethodDef *ml, int flags, PyObject* qualname,
+                                       PyObject *closure, PyObject *module, PyObject* globals, PyObject* code) {
+    PyCFunctionObject *cf = (PyCFunctionObject*) op;
+    if (unlikely(op == NULL))
+        return NULL;
+    op->flags = flags;
+    __Pyx_CyFunction_weakreflist(op) = NULL;
+    cf->m_ml = ml;
+    cf->m_self = (PyObject *) op;
+    Py_XINCREF(closure);
+    op->func_closure = closure;
+    Py_XINCREF(module);
+    cf->m_module = module;
+    op->func_dict = NULL;
+    op->func_name = NULL;
+    Py_INCREF(qualname);
+    op->func_qualname = qualname;
+    op->func_doc = NULL;
+#if PY_VERSION_HEX < 0x030900B1
+    op->func_classobj = NULL;
+#else
+    ((PyCMethodObject*)op)->mm_class = NULL;
+#endif
+    op->func_globals = globals;
+    Py_INCREF(op->func_globals);
+    Py_XINCREF(code);
+    op->func_code = code;
+    op->defaults_pyobjects = 0;
+    op->defaults_size = 0;
+    op->defaults = NULL;
+    op->defaults_tuple = NULL;
+    op->defaults_kwdict = NULL;
+    op->defaults_getter = NULL;
+    op->func_annotations = NULL;
+    op->func_is_coroutine = NULL;
+#if CYTHON_METH_FASTCALL
+    switch (ml->ml_flags & (METH_VARARGS | METH_FASTCALL | METH_NOARGS | METH_O | METH_KEYWORDS | METH_METHOD)) {
+    case METH_NOARGS:
+        __Pyx_CyFunction_func_vectorcall(op) = __Pyx_CyFunction_Vectorcall_NOARGS;
+        break;
+    case METH_O:
+        __Pyx_CyFunction_func_vectorcall(op) = __Pyx_CyFunction_Vectorcall_O;
+        break;
+    case METH_METHOD | METH_FASTCALL | METH_KEYWORDS:
+        __Pyx_CyFunction_func_vectorcall(op) = __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD;
+        break;
+    case METH_FASTCALL | METH_KEYWORDS:
+        __Pyx_CyFunction_func_vectorcall(op) = __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS;
+        break;
+    case METH_VARARGS | METH_KEYWORDS:
+        __Pyx_CyFunction_func_vectorcall(op) = NULL;
+        break;
+    default:
+        PyErr_SetString(PyExc_SystemError, "Bad call flags for CyFunction");
+        Py_DECREF(op);
+        return NULL;
+    }
+#endif
+    return (PyObject *) op;
+}
+static int
+__Pyx_CyFunction_clear(__pyx_CyFunctionObject *m)
+{
+    Py_CLEAR(m->func_closure);
+    Py_CLEAR(((PyCFunctionObject*)m)->m_module);
+    Py_CLEAR(m->func_dict);
+    Py_CLEAR(m->func_name);
+    Py_CLEAR(m->func_qualname);
+    Py_CLEAR(m->func_doc);
+    Py_CLEAR(m->func_globals);
+    Py_CLEAR(m->func_code);
+#if PY_VERSION_HEX < 0x030900B1
+    Py_CLEAR(__Pyx_CyFunction_GetClassObj(m));
+#else
+    {
+        PyObject *cls = (PyObject*) ((PyCMethodObject *) (m))->mm_class;
+        ((PyCMethodObject *) (m))->mm_class = NULL;
+        Py_XDECREF(cls);
+    }
+#endif
+    Py_CLEAR(m->defaults_tuple);
+    Py_CLEAR(m->defaults_kwdict);
+    Py_CLEAR(m->func_annotations);
+    Py_CLEAR(m->func_is_coroutine);
+    if (m->defaults) {
+        PyObject **pydefaults = __Pyx_CyFunction_Defaults(PyObject *, m);
+        int i;
+        for (i = 0; i < m->defaults_pyobjects; i++)
+            Py_XDECREF(pydefaults[i]);
+        PyObject_Free(m->defaults);
+        m->defaults = NULL;
+    }
+    return 0;
+}
+static void __Pyx__CyFunction_dealloc(__pyx_CyFunctionObject *m)
+{
+    if (__Pyx_CyFunction_weakreflist(m) != NULL)
+        PyObject_ClearWeakRefs((PyObject *) m);
+    __Pyx_CyFunction_clear(m);
+    __Pyx_PyHeapTypeObject_GC_Del(m);
+}
+static void __Pyx_CyFunction_dealloc(__pyx_CyFunctionObject *m)
+{
+    PyObject_GC_UnTrack(m);
+    __Pyx__CyFunction_dealloc(m);
+}
+static int __Pyx_CyFunction_traverse(__pyx_CyFunctionObject *m, visitproc visit, void *arg)
+{
+    Py_VISIT(m->func_closure);
+    Py_VISIT(((PyCFunctionObject*)m)->m_module);
+    Py_VISIT(m->func_dict);
+    Py_VISIT(m->func_name);
+    Py_VISIT(m->func_qualname);
+    Py_VISIT(m->func_doc);
+    Py_VISIT(m->func_globals);
+    Py_VISIT(m->func_code);
+    Py_VISIT(__Pyx_CyFunction_GetClassObj(m));
+    Py_VISIT(m->defaults_tuple);
+    Py_VISIT(m->defaults_kwdict);
+    Py_VISIT(m->func_is_coroutine);
+    if (m->defaults) {
+        PyObject **pydefaults = __Pyx_CyFunction_Defaults(PyObject *, m);
+        int i;
+        for (i = 0; i < m->defaults_pyobjects; i++)
+            Py_VISIT(pydefaults[i]);
+    }
+    return 0;
+}
+static PyObject*
+__Pyx_CyFunction_repr(__pyx_CyFunctionObject *op)
+{
+#if PY_MAJOR_VERSION >= 3
+    return PyUnicode_FromFormat("<cyfunction %U at %p>",
+                                op->func_qualname, (void *)op);
+#else
+    return PyString_FromFormat("<cyfunction %s at %p>",
+                               PyString_AsString(op->func_qualname), (void *)op);
+#endif
+}
+static PyObject * __Pyx_CyFunction_CallMethod(PyObject *func, PyObject *self, PyObject *arg, PyObject *kw) {
+    PyCFunctionObject* f = (PyCFunctionObject*)func;
+    PyCFunction meth = f->m_ml->ml_meth;
+    Py_ssize_t size;
+    switch (f->m_ml->ml_flags & (METH_VARARGS | METH_KEYWORDS | METH_NOARGS | METH_O)) {
+    case METH_VARARGS:
+        if (likely(kw == NULL || PyDict_Size(kw) == 0))
+            return (*meth)(self, arg);
+        break;
+    case METH_VARARGS | METH_KEYWORDS:
+        return (*(PyCFunctionWithKeywords)(void*)meth)(self, arg, kw);
+    case METH_NOARGS:
+        if (likely(kw == NULL || PyDict_Size(kw) == 0)) {
+            size = PyTuple_GET_SIZE(arg);
+            if (likely(size == 0))
+                return (*meth)(self, NULL);
+            PyErr_Format(PyExc_TypeError,
+                "%.200s() takes no arguments (%" CYTHON_FORMAT_SSIZE_T "d given)",
+                f->m_ml->ml_name, size);
+            return NULL;
+        }
+        break;
+    case METH_O:
+        if (likely(kw == NULL || PyDict_Size(kw) == 0)) {
+            size = PyTuple_GET_SIZE(arg);
+            if (likely(size == 1)) {
+                PyObject *result, *arg0;
+                #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+                arg0 = PyTuple_GET_ITEM(arg, 0);
+                #else
+                arg0 = PySequence_ITEM(arg, 0); if (unlikely(!arg0)) return NULL;
+                #endif
+                result = (*meth)(self, arg0);
+                #if !(CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS)
+                Py_DECREF(arg0);
+                #endif
+                return result;
+            }
+            PyErr_Format(PyExc_TypeError,
+                "%.200s() takes exactly one argument (%" CYTHON_FORMAT_SSIZE_T "d given)",
+                f->m_ml->ml_name, size);
+            return NULL;
+        }
+        break;
+    default:
+        PyErr_SetString(PyExc_SystemError, "Bad call flags for CyFunction");
+        return NULL;
+    }
+    PyErr_Format(PyExc_TypeError, "%.200s() takes no keyword arguments",
+                 f->m_ml->ml_name);
+    return NULL;
+}
+static CYTHON_INLINE PyObject *__Pyx_CyFunction_Call(PyObject *func, PyObject *arg, PyObject *kw) {
+    return __Pyx_CyFunction_CallMethod(func, ((PyCFunctionObject*)func)->m_self, arg, kw);
+}
+static PyObject *__Pyx_CyFunction_CallAsMethod(PyObject *func, PyObject *args, PyObject *kw) {
+    PyObject *result;
+    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *) func;
+#if CYTHON_METH_FASTCALL
+     __pyx_vectorcallfunc vc = __Pyx_CyFunction_func_vectorcall(cyfunc);
+    if (vc) {
+#if CYTHON_ASSUME_SAFE_MACROS
+        return __Pyx_PyVectorcall_FastCallDict(func, vc, &PyTuple_GET_ITEM(args, 0), (size_t)PyTuple_GET_SIZE(args), kw);
+#else
+        (void) &__Pyx_PyVectorcall_FastCallDict;
+        return PyVectorcall_Call(func, args, kw);
+#endif
+    }
+#endif
+    if ((cyfunc->flags & __Pyx_CYFUNCTION_CCLASS) && !(cyfunc->flags & __Pyx_CYFUNCTION_STATICMETHOD)) {
+        Py_ssize_t argc;
+        PyObject *new_args;
+        PyObject *self;
+        argc = PyTuple_GET_SIZE(args);
+        new_args = PyTuple_GetSlice(args, 1, argc);
+        if (unlikely(!new_args))
+            return NULL;
+        self = PyTuple_GetItem(args, 0);
+        if (unlikely(!self)) {
+            Py_DECREF(new_args);
+#if PY_MAJOR_VERSION > 2
+            PyErr_Format(PyExc_TypeError,
+                         "unbound method %.200S() needs an argument",
+                         cyfunc->func_qualname);
+#else
+            PyErr_SetString(PyExc_TypeError,
+                            "unbound method needs an argument");
+#endif
+            return NULL;
+        }
+        result = __Pyx_CyFunction_CallMethod(func, self, new_args, kw);
+        Py_DECREF(new_args);
+    } else {
+        result = __Pyx_CyFunction_Call(func, args, kw);
+    }
+    return result;
+}
+#if CYTHON_METH_FASTCALL
+static CYTHON_INLINE int __Pyx_CyFunction_Vectorcall_CheckArgs(__pyx_CyFunctionObject *cyfunc, Py_ssize_t nargs, PyObject *kwnames)
+{
+    int ret = 0;
+    if ((cyfunc->flags & __Pyx_CYFUNCTION_CCLASS) && !(cyfunc->flags & __Pyx_CYFUNCTION_STATICMETHOD)) {
+        if (unlikely(nargs < 1)) {
+            PyErr_Format(PyExc_TypeError, "%.200s() needs an argument",
+                         ((PyCFunctionObject*)cyfunc)->m_ml->ml_name);
+            return -1;
+        }
+        ret = 1;
+    }
+    if (unlikely(kwnames) && unlikely(PyTuple_GET_SIZE(kwnames))) {
+        PyErr_Format(PyExc_TypeError,
+                     "%.200s() takes no keyword arguments", ((PyCFunctionObject*)cyfunc)->m_ml->ml_name);
+        return -1;
+    }
+    return ret;
+}
+static PyObject * __Pyx_CyFunction_Vectorcall_NOARGS(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
+{
+    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
+    PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
+#if CYTHON_BACKPORT_VECTORCALL
+    Py_ssize_t nargs = (Py_ssize_t)nargsf;
+#else
+    Py_ssize_t nargs = PyVectorcall_NARGS(nargsf);
+#endif
+    PyObject *self;
+    switch (__Pyx_CyFunction_Vectorcall_CheckArgs(cyfunc, nargs, kwnames)) {
+    case 1:
+        self = args[0];
+        args += 1;
+        nargs -= 1;
+        break;
+    case 0:
+        self = ((PyCFunctionObject*)cyfunc)->m_self;
+        break;
+    default:
+        return NULL;
+    }
+    if (unlikely(nargs != 0)) {
+        PyErr_Format(PyExc_TypeError,
+            "%.200s() takes no arguments (%" CYTHON_FORMAT_SSIZE_T "d given)",
+            def->ml_name, nargs);
+        return NULL;
+    }
+    return def->ml_meth(self, NULL);
+}
+static PyObject * __Pyx_CyFunction_Vectorcall_O(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
+{
+    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
+    PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
+#if CYTHON_BACKPORT_VECTORCALL
+    Py_ssize_t nargs = (Py_ssize_t)nargsf;
+#else
+    Py_ssize_t nargs = PyVectorcall_NARGS(nargsf);
+#endif
+    PyObject *self;
+    switch (__Pyx_CyFunction_Vectorcall_CheckArgs(cyfunc, nargs, kwnames)) {
+    case 1:
+        self = args[0];
+        args += 1;
+        nargs -= 1;
+        break;
+    case 0:
+        self = ((PyCFunctionObject*)cyfunc)->m_self;
+        break;
+    default:
+        return NULL;
+    }
+    if (unlikely(nargs != 1)) {
+        PyErr_Format(PyExc_TypeError,
+            "%.200s() takes exactly one argument (%" CYTHON_FORMAT_SSIZE_T "d given)",
+            def->ml_name, nargs);
+        return NULL;
+    }
+    return def->ml_meth(self, args[0]);
+}
+static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
+{
+    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
+    PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
+#if CYTHON_BACKPORT_VECTORCALL
+    Py_ssize_t nargs = (Py_ssize_t)nargsf;
+#else
+    Py_ssize_t nargs = PyVectorcall_NARGS(nargsf);
+#endif
+    PyObject *self;
+    switch (__Pyx_CyFunction_Vectorcall_CheckArgs(cyfunc, nargs, NULL)) {
+    case 1:
+        self = args[0];
+        args += 1;
+        nargs -= 1;
+        break;
+    case 0:
+        self = ((PyCFunctionObject*)cyfunc)->m_self;
+        break;
+    default:
+        return NULL;
+    }
+    return ((_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
+}
+static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
+{
+    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
+    PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
+    PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
+#if CYTHON_BACKPORT_VECTORCALL
+    Py_ssize_t nargs = (Py_ssize_t)nargsf;
+#else
+    Py_ssize_t nargs = PyVectorcall_NARGS(nargsf);
+#endif
+    PyObject *self;
+    switch (__Pyx_CyFunction_Vectorcall_CheckArgs(cyfunc, nargs, NULL)) {
+    case 1:
+        self = args[0];
+        args += 1;
+        nargs -= 1;
+        break;
+    case 0:
+        self = ((PyCFunctionObject*)cyfunc)->m_self;
+        break;
+    default:
+        return NULL;
+    }
+    return ((__Pyx_PyCMethod)(void(*)(void))def->ml_meth)(self, cls, args, (size_t)nargs, kwnames);
+}
+#endif
+#if CYTHON_USE_TYPE_SPECS
+static PyType_Slot __pyx_CyFunctionType_slots[] = {
+    {Py_tp_dealloc, (void *)__Pyx_CyFunction_dealloc},
+    {Py_tp_repr, (void *)__Pyx_CyFunction_repr},
+    {Py_tp_call, (void *)__Pyx_CyFunction_CallAsMethod},
+    {Py_tp_traverse, (void *)__Pyx_CyFunction_traverse},
+    {Py_tp_clear, (void *)__Pyx_CyFunction_clear},
+    {Py_tp_methods, (void *)__pyx_CyFunction_methods},
+    {Py_tp_members, (void *)__pyx_CyFunction_members},
+    {Py_tp_getset, (void *)__pyx_CyFunction_getsets},
+    {Py_tp_descr_get, (void *)__Pyx_PyMethod_New},
+    {0, 0},
+};
+static PyType_Spec __pyx_CyFunctionType_spec = {
+    __PYX_TYPE_MODULE_PREFIX "cython_function_or_method",
+    sizeof(__pyx_CyFunctionObject),
+    0,
+#ifdef Py_TPFLAGS_METHOD_DESCRIPTOR
+    Py_TPFLAGS_METHOD_DESCRIPTOR |
+#endif
+#if (defined(_Py_TPFLAGS_HAVE_VECTORCALL) && CYTHON_METH_FASTCALL)
+    _Py_TPFLAGS_HAVE_VECTORCALL |
+#endif
+    Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HAVE_GC | Py_TPFLAGS_BASETYPE,
+    __pyx_CyFunctionType_slots
+};
+#else
+static PyTypeObject __pyx_CyFunctionType_type = {
+    PyVarObject_HEAD_INIT(0, 0)
+    __PYX_TYPE_MODULE_PREFIX "cython_function_or_method",
+    sizeof(__pyx_CyFunctionObject),
+    0,
+    (destructor) __Pyx_CyFunction_dealloc,
+#if !CYTHON_METH_FASTCALL
+    0,
+#elif CYTHON_BACKPORT_VECTORCALL
+    (printfunc)offsetof(__pyx_CyFunctionObject, func_vectorcall),
+#else
+    offsetof(PyCFunctionObject, vectorcall),
+#endif
+    0,
+    0,
+#if PY_MAJOR_VERSION < 3
+    0,
+#else
+    0,
+#endif
+    (reprfunc) __Pyx_CyFunction_repr,
+    0,
+    0,
+    0,
+    0,
+    __Pyx_CyFunction_CallAsMethod,
+    0,
+    0,
+    0,
+    0,
+#ifdef Py_TPFLAGS_METHOD_DESCRIPTOR
+    Py_TPFLAGS_METHOD_DESCRIPTOR |
+#endif
+#ifdef _Py_TPFLAGS_HAVE_VECTORCALL
+    _Py_TPFLAGS_HAVE_VECTORCALL |
+#endif
+    Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HAVE_GC | Py_TPFLAGS_BASETYPE,
+    0,
+    (traverseproc) __Pyx_CyFunction_traverse,
+    (inquiry) __Pyx_CyFunction_clear,
+    0,
+#if PY_VERSION_HEX < 0x030500A0
+    offsetof(__pyx_CyFunctionObject, func_weakreflist),
+#else
+    offsetof(PyCFunctionObject, m_weakreflist),
+#endif
+    0,
+    0,
+    __pyx_CyFunction_methods,
+    __pyx_CyFunction_members,
+    __pyx_CyFunction_getsets,
+    0,
+    0,
+    __Pyx_PyMethod_New,
+    0,
+    offsetof(__pyx_CyFunctionObject, func_dict),
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+#if PY_VERSION_HEX >= 0x030400a1
+    0,
+#endif
+#if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
+    0,
+#endif
+#if __PYX_NEED_TP_PRINT_SLOT
+    0,
+#endif
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+    0,
+#endif
+};
+#endif
+static int __pyx_CyFunction_init(PyObject *module) {
+#if CYTHON_USE_TYPE_SPECS
+    __pyx_CyFunctionType = __Pyx_FetchCommonTypeFromSpec(module, &__pyx_CyFunctionType_spec, NULL);
+#else
+    CYTHON_UNUSED_VAR(module);
+    __pyx_CyFunctionType = __Pyx_FetchCommonType(&__pyx_CyFunctionType_type);
+#endif
+    if (unlikely(__pyx_CyFunctionType == NULL)) {
+        return -1;
+    }
+    return 0;
+}
+static CYTHON_INLINE void *__Pyx_CyFunction_InitDefaults(PyObject *func, size_t size, int pyobjects) {
+    __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
+    m->defaults = PyObject_Malloc(size);
+    if (unlikely(!m->defaults))
+        return PyErr_NoMemory();
+    memset(m->defaults, 0, size);
+    m->defaults_pyobjects = pyobjects;
+    m->defaults_size = size;
+    return m->defaults;
+}
+static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsTuple(PyObject *func, PyObject *tuple) {
+    __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
+    m->defaults_tuple = tuple;
+    Py_INCREF(tuple);
+}
+static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsKwDict(PyObject *func, PyObject *dict) {
+    __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
+    m->defaults_kwdict = dict;
+    Py_INCREF(dict);
+}
+static CYTHON_INLINE void __Pyx_CyFunction_SetAnnotationsDict(PyObject *func, PyObject *dict) {
+    __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
+    m->func_annotations = dict;
+    Py_INCREF(dict);
+}
+
+/* CythonFunction */
+  static PyObject *__Pyx_CyFunction_New(PyMethodDef *ml, int flags, PyObject* qualname,
+                                      PyObject *closure, PyObject *module, PyObject* globals, PyObject* code) {
+    PyObject *op = __Pyx_CyFunction_Init(
+        PyObject_GC_New(__pyx_CyFunctionObject, __pyx_CyFunctionType),
+        ml, flags, qualname, closure, module, globals, code
+    );
+    if (likely(op)) {
+        PyObject_GC_Track(op);
+    }
+    return op;
+}
+
 /* CLineInTraceback */
   #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
+    CYTHON_MAYBE_UNUSED_VAR(tstate);
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
     }
     __Pyx_ErrFetchInState(tstate, &ptype, &pvalue, &ptraceback);
 #if CYTHON_COMPILING_IN_CPYTHON
     cython_runtime_dict = _PyObject_GetDictPtr(__pyx_cython_runtime);
     if (likely(cython_runtime_dict)) {
         __PYX_PY_DICT_LOOKUP_IF_MODIFIED(
             use_cline, *cython_runtime_dict,
             __Pyx_PyDict_GetItemStr(*cython_runtime_dict, __pyx_n_s_cline_in_traceback))
     } else
 #endif
     {
-      PyObject *use_cline_obj = __Pyx_PyObject_GetAttrStr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback);
+      PyObject *use_cline_obj = __Pyx_PyObject_GetAttrStrNoError(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback);
       if (use_cline_obj) {
         use_cline = PyObject_Not(use_cline_obj) ? Py_False : Py_True;
         Py_DECREF(use_cline_obj);
       } else {
         PyErr_Clear();
         use_cline = NULL;
       }
@@ -7987,15 +11382,16 @@
     }
     __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
     return c_line;
 }
 #endif
 
 /* CodeObjectCache */
-  static int __pyx_bisect_code_objects(__Pyx_CodeObjectCacheEntry* entries, int count, int code_line) {
+  #if !CYTHON_COMPILING_IN_LIMITED_API
+static int __pyx_bisect_code_objects(__Pyx_CodeObjectCacheEntry* entries, int count, int code_line) {
     int start = 0, mid = 0, end = count - 1;
     if (end >= 0 && code_line > entries[end].code_line) {
         return count;
     }
     while (start < end) {
         mid = start + (end - start) / 2;
         if (code_line < entries[mid].code_line) {
@@ -8065,25 +11461,36 @@
         entries[i] = entries[i-1];
     }
     entries[pos].code_line = code_line;
     entries[pos].code_object = code_object;
     __pyx_code_cache.count++;
     Py_INCREF(code_object);
 }
+#endif
 
 /* AddTraceback */
   #include "compile.h"
 #include "frameobject.h"
 #include "traceback.h"
 #if PY_VERSION_HEX >= 0x030b00a6
   #ifndef Py_BUILD_CORE
     #define Py_BUILD_CORE 1
   #endif
   #include "internal/pycore_frame.h"
 #endif
+#if CYTHON_COMPILING_IN_LIMITED_API
+static void __Pyx_AddTraceback(const char *funcname, int c_line,
+                               int py_line, const char *filename) {
+    if (c_line) {
+        (void) __pyx_cfilenm;
+        (void) __Pyx_CLineForTraceback(__Pyx_PyThreadState_Current, c_line);
+    }
+    _PyTraceback_Add(funcname, filename, py_line);
+}
+#else
 static PyCodeObject* __Pyx_CreateCodeObjectForTraceback(
             const char *funcname, int c_line,
             int py_line, const char *filename) {
     PyCodeObject *py_code = NULL;
     PyObject *py_funcname = NULL;
     #if PY_MAJOR_VERSION < 3
     PyObject *py_srcfile = NULL;
@@ -8110,14 +11517,15 @@
     #if PY_MAJOR_VERSION < 3
     py_code = __Pyx_PyCode_New(
         0,
         0,
         0,
         0,
         0,
+        0,
         __pyx_empty_bytes, /*PyObject *code,*/
         __pyx_empty_tuple, /*PyObject *consts,*/
         __pyx_empty_tuple, /*PyObject *names,*/
         __pyx_empty_tuple, /*PyObject *varnames,*/
         __pyx_empty_tuple, /*PyObject *freevars,*/
         __pyx_empty_tuple, /*PyObject *cellvars,*/
         py_srcfile,   /*PyObject *filename,*/
@@ -8172,19 +11580,25 @@
     if (!py_frame) goto bad;
     __Pyx_PyFrame_SetLineNumber(py_frame, py_line);
     PyTraceBack_Here(py_frame);
 bad:
     Py_XDECREF(py_code);
     Py_XDECREF(py_frame);
 }
+#endif
 
 #if PY_MAJOR_VERSION < 3
 static int __Pyx_GetBuffer(PyObject *obj, Py_buffer *view, int flags) {
+    __Pyx_TypeName obj_type_name;
     if (PyObject_CheckBuffer(obj)) return PyObject_GetBuffer(obj, view, flags);
-    PyErr_Format(PyExc_TypeError, "'%.200s' does not have the buffer interface", Py_TYPE(obj)->tp_name);
+    obj_type_name = __Pyx_PyType_GetName(Py_TYPE(obj));
+    PyErr_Format(PyExc_TypeError,
+                 "'" __Pyx_FMT_TYPENAME "' does not have the buffer interface",
+                 obj_type_name);
+    __Pyx_DECREF_TypeName(obj_type_name);
     return -1;
 }
 static void __Pyx_ReleaseBuffer(Py_buffer *view) {
     PyObject *obj = view->obj;
     if (!obj) return;
     if (PyObject_CheckBuffer(obj)) {
         PyBuffer_Release(view);
@@ -8216,15 +11630,15 @@
                     goto raise_overflow;\
             }\
         }\
         return (target_type) value;\
     }
 
 /* Declarations */
-  #if CYTHON_CCOMPLEX
+  #if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
   #ifdef __cplusplus
     static CYTHON_INLINE __pyx_t_float_complex __pyx_t_float_complex_from_parts(float x, float y) {
       return ::std::complex< float >(x, y);
     }
   #else
     static CYTHON_INLINE __pyx_t_float_complex __pyx_t_float_complex_from_parts(float x, float y) {
       return x + y*(__pyx_t_float_complex)_Complex_I;
@@ -8236,15 +11650,15 @@
       z.real = x;
       z.imag = y;
       return z;
     }
 #endif
 
 /* Arithmetic */
-  #if CYTHON_CCOMPLEX
+  #if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
 #else
     static CYTHON_INLINE int __Pyx_c_eq_float(__pyx_t_float_complex a, __pyx_t_float_complex b) {
        return (a.real == b.real) && (a.imag == b.imag);
     }
     static CYTHON_INLINE __pyx_t_float_complex __Pyx_c_sum_float(__pyx_t_float_complex a, __pyx_t_float_complex b) {
         __pyx_t_float_complex z;
         z.real = a.real + b.real;
@@ -8344,15 +11758,15 @@
                         z = __Pyx_c_prod_float(a, a);
                         return __Pyx_c_prod_float(z, z);
                 }
             }
             if (a.imag == 0) {
                 if (a.real == 0) {
                     return a;
-                } else if (b.imag == 0) {
+                } else if ((b.imag == 0) && (a.real >= 0)) {
                     z.real = powf(a.real, b.real);
                     z.imag = 0;
                     return z;
                 } else if (a.real > 0) {
                     r = a.real;
                     theta = 0;
                 } else {
@@ -8370,15 +11784,15 @@
             z.imag = z_r * sinf(z_theta);
             return z;
         }
     #endif
 #endif
 
 /* Declarations */
-  #if CYTHON_CCOMPLEX
+  #if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
   #ifdef __cplusplus
     static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double x, double y) {
       return ::std::complex< double >(x, y);
     }
   #else
     static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double x, double y) {
       return x + y*(__pyx_t_double_complex)_Complex_I;
@@ -8390,15 +11804,15 @@
       z.real = x;
       z.imag = y;
       return z;
     }
 #endif
 
 /* Arithmetic */
-  #if CYTHON_CCOMPLEX
+  #if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
 #else
     static CYTHON_INLINE int __Pyx_c_eq_double(__pyx_t_double_complex a, __pyx_t_double_complex b) {
        return (a.real == b.real) && (a.imag == b.imag);
     }
     static CYTHON_INLINE __pyx_t_double_complex __Pyx_c_sum_double(__pyx_t_double_complex a, __pyx_t_double_complex b) {
         __pyx_t_double_complex z;
         z.real = a.real + b.real;
@@ -8498,15 +11912,15 @@
                         z = __Pyx_c_prod_double(a, a);
                         return __Pyx_c_prod_double(z, z);
                 }
             }
             if (a.imag == 0) {
                 if (a.real == 0) {
                     return a;
-                } else if (b.imag == 0) {
+                } else if ((b.imag == 0) && (a.real >= 0)) {
                     z.real = pow(a.real, b.real);
                     z.imag = 0;
                     return z;
                 } else if (a.real > 0) {
                     r = a.real;
                     theta = 0;
                 } else {
@@ -8536,177 +11950,254 @@
     const int neg_one = (int) -1, const_zero = (int) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
 #endif
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
-        if (sizeof(int) < sizeof(long)) {
+        if ((sizeof(int) < sizeof(long))) {
             __PYX_VERIFY_RETURN_INT(int, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
             if (is_unsigned && unlikely(val < 0)) {
                 goto raise_neg_overflow;
             }
             return (int) val;
         }
     } else
 #endif
     if (likely(PyLong_Check(x))) {
         if (is_unsigned) {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (int) 0;
-                case  1: __PYX_VERIFY_RETURN_INT(int, digit, digits[0])
-                case 2:
-                    if (8 * sizeof(int) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) >= 2 * PyLong_SHIFT) {
-                            return (int) (((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+            if (unlikely(__Pyx_PyLong_IsNeg(x))) {
+                goto raise_neg_overflow;
+            } else if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(int, __Pyx_compact_upylong, __Pyx_PyLong_CompactValueUnsigned(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_DigitCount(x)) {
+                    case 2:
+                        if ((8 * sizeof(int) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) >= 2 * PyLong_SHIFT)) {
+                                return (int) (((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(int) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) >= 3 * PyLong_SHIFT) {
-                            return (int) (((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(int) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) >= 3 * PyLong_SHIFT)) {
+                                return (int) (((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(int) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
-                            return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(int) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) >= 4 * PyLong_SHIFT)) {
+                                return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
                     return (int) -1;
                 if (unlikely(result == 1))
                     goto raise_neg_overflow;
             }
 #endif
-            if (sizeof(int) <= sizeof(unsigned long)) {
+            if ((sizeof(int) <= sizeof(unsigned long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(int, unsigned long, PyLong_AsUnsignedLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
+            } else if ((sizeof(int) <= sizeof(unsigned PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(int, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
 #endif
             }
         } else {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (int) 0;
-                case -1: __PYX_VERIFY_RETURN_INT(int, sdigit, (sdigit) (-(sdigit)digits[0]))
-                case  1: __PYX_VERIFY_RETURN_INT(int,  digit, +digits[0])
-                case -2:
-                    if (8 * sizeof(int) - 1 > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 2 * PyLong_SHIFT) {
-                            return (int) (((int)-1)*(((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+            if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(int, __Pyx_compact_pylong, __Pyx_PyLong_CompactValue(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_SignedDigitCount(x)) {
+                    case -2:
+                        if ((8 * sizeof(int) - 1 > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
+                                return (int) (((int)-1)*(((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 2:
-                    if (8 * sizeof(int) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 2 * PyLong_SHIFT) {
-                            return (int) ((((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        break;
+                    case 2:
+                        if ((8 * sizeof(int) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
+                                return (int) ((((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -3:
-                    if (8 * sizeof(int) - 1 > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 3 * PyLong_SHIFT) {
-                            return (int) (((int)-1)*(((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        break;
+                    case -3:
+                        if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
+                                return (int) (((int)-1)*(((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(int) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 3 * PyLong_SHIFT) {
-                            return (int) ((((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(int) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
+                                return (int) ((((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -4:
-                    if (8 * sizeof(int) - 1 > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 4 * PyLong_SHIFT) {
-                            return (int) (((int)-1)*(((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        break;
+                    case -4:
+                        if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 4 * PyLong_SHIFT)) {
+                                return (int) (((int)-1)*(((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(int) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 4 * PyLong_SHIFT) {
-                            return (int) ((((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(int) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 4 * PyLong_SHIFT)) {
+                                return (int) ((((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
-            if (sizeof(int) <= sizeof(long)) {
+            if ((sizeof(int) <= sizeof(long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(int, long, PyLong_AsLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
+            } else if ((sizeof(int) <= sizeof(PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(int, PY_LONG_LONG, PyLong_AsLongLong(x))
 #endif
             }
         }
         {
-#if CYTHON_COMPILING_IN_PYPY && !defined(_PyLong_AsByteArray)
-            PyErr_SetString(PyExc_RuntimeError,
-                            "_PyLong_AsByteArray() not available in PyPy, cannot convert large numbers");
-#else
             int val;
             PyObject *v = __Pyx_PyNumber_IntOrLong(x);
- #if PY_MAJOR_VERSION < 3
+#if PY_MAJOR_VERSION < 3
             if (likely(v) && !PyLong_Check(v)) {
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
- #endif
+#endif
             if (likely(v)) {
+                int ret = -1;
+#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
-                int ret = _PyLong_AsByteArray((PyLongObject *)v,
-                                              bytes, sizeof(val),
-                                              is_little, !is_unsigned);
+                ret = _PyLong_AsByteArray((PyLongObject *)v,
+                                           bytes, sizeof(val),
+                                           is_little, !is_unsigned);
+#else
+                PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
+                int bits, remaining_bits, is_negative = 0;
+                long idigit;
+                int chunk_size = (sizeof(long) < 8) ? 30 : 62;
+                if (unlikely(!PyLong_CheckExact(v))) {
+                    PyObject *tmp = v;
+                    v = PyNumber_Long(v);
+                    assert(PyLong_CheckExact(v));
+                    Py_DECREF(tmp);
+                    if (unlikely(!v)) return (int) -1;
+                }
+#if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                if (Py_SIZE(x) == 0)
+                    return (int) 0;
+                is_negative = Py_SIZE(x) < 0;
+#else
+                {
+                    int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
+                    if (unlikely(result < 0))
+                        return (int) -1;
+                    is_negative = result == 1;
+                }
+#endif
+                if (is_unsigned && unlikely(is_negative)) {
+                    goto raise_neg_overflow;
+                } else if (is_negative) {
+                    stepval = PyNumber_Invert(v);
+                    if (unlikely(!stepval))
+                        return (int) -1;
+                } else {
+                    stepval = __Pyx_NewRef(v);
+                }
+                val = (int) 0;
+                mask = PyLong_FromLong((1L << chunk_size) - 1); if (unlikely(!mask)) goto done;
+                shift = PyLong_FromLong(chunk_size); if (unlikely(!shift)) goto done;
+                for (bits = 0; bits < (int) sizeof(int) * 8 - chunk_size; bits += chunk_size) {
+                    PyObject *tmp, *digit;
+                    digit = PyNumber_And(stepval, mask);
+                    if (unlikely(!digit)) goto done;
+                    idigit = PyLong_AsLong(digit);
+                    Py_DECREF(digit);
+                    if (unlikely(idigit < 0)) goto done;
+                    tmp = PyNumber_Rshift(stepval, shift);
+                    if (unlikely(!tmp)) goto done;
+                    Py_DECREF(stepval); stepval = tmp;
+                    val |= ((int) idigit) << bits;
+                    #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                    if (Py_SIZE(stepval) == 0)
+                        goto unpacking_done;
+                    #endif
+                }
+                idigit = PyLong_AsLong(stepval);
+                if (unlikely(idigit < 0)) goto done;
+                remaining_bits = ((int) sizeof(int) * 8) - bits - (is_unsigned ? 0 : 1);
+                if (unlikely(idigit >= (1L << remaining_bits)))
+                    goto raise_overflow;
+                val |= ((int) idigit) << bits;
+            #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+            unpacking_done:
+            #endif
+                if (!is_unsigned) {
+                    if (unlikely(val & (((int) 1) << (sizeof(int) * 8 - 1))))
+                        goto raise_overflow;
+                    if (is_negative)
+                        val = ~val;
+                }
+                ret = 0;
+            done:
+                Py_XDECREF(shift);
+                Py_XDECREF(mask);
+                Py_XDECREF(stepval);
+#endif
                 Py_DECREF(v);
                 if (likely(!ret))
                     return val;
             }
-#endif
             return (int) -1;
         }
     } else {
         int val;
         PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
         if (!tmp) return (int) -1;
         val = __Pyx_PyInt_As_int(tmp);
@@ -8719,14 +12210,29 @@
     return (int) -1;
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to int");
     return (int) -1;
 }
 
+/* FormatTypeName */
+  #if CYTHON_COMPILING_IN_LIMITED_API
+static __Pyx_TypeName
+__Pyx_PyType_GetName(PyTypeObject* tp)
+{
+    PyObject *name = __Pyx_PyObject_GetAttrStr((PyObject *)tp,
+                                               __pyx_n_s_name);
+    if (unlikely(name == NULL) || unlikely(!PyUnicode_Check(name))) {
+        PyErr_Clear();
+        Py_XSETREF(name, __Pyx_NewRef(__pyx_n_s__12));
+    }
+    return name;
+}
+#endif
+
 /* CIntToPy */
   static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const long neg_one = (long) -1, const_zero = (long) 0;
@@ -8770,177 +12276,254 @@
     const long neg_one = (long) -1, const_zero = (long) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
 #endif
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
-        if (sizeof(long) < sizeof(long)) {
+        if ((sizeof(long) < sizeof(long))) {
             __PYX_VERIFY_RETURN_INT(long, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
             if (is_unsigned && unlikely(val < 0)) {
                 goto raise_neg_overflow;
             }
             return (long) val;
         }
     } else
 #endif
     if (likely(PyLong_Check(x))) {
         if (is_unsigned) {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (long) 0;
-                case  1: __PYX_VERIFY_RETURN_INT(long, digit, digits[0])
-                case 2:
-                    if (8 * sizeof(long) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) >= 2 * PyLong_SHIFT) {
-                            return (long) (((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+            if (unlikely(__Pyx_PyLong_IsNeg(x))) {
+                goto raise_neg_overflow;
+            } else if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(long, __Pyx_compact_upylong, __Pyx_PyLong_CompactValueUnsigned(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_DigitCount(x)) {
+                    case 2:
+                        if ((8 * sizeof(long) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) >= 2 * PyLong_SHIFT)) {
+                                return (long) (((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(long) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) >= 3 * PyLong_SHIFT) {
-                            return (long) (((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(long) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) >= 3 * PyLong_SHIFT)) {
+                                return (long) (((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(long) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
-                            return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(long) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) >= 4 * PyLong_SHIFT)) {
+                                return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
                     return (long) -1;
                 if (unlikely(result == 1))
                     goto raise_neg_overflow;
             }
 #endif
-            if (sizeof(long) <= sizeof(unsigned long)) {
+            if ((sizeof(long) <= sizeof(unsigned long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(long, unsigned long, PyLong_AsUnsignedLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(long) <= sizeof(unsigned PY_LONG_LONG)) {
+            } else if ((sizeof(long) <= sizeof(unsigned PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(long, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
 #endif
             }
         } else {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (long) 0;
-                case -1: __PYX_VERIFY_RETURN_INT(long, sdigit, (sdigit) (-(sdigit)digits[0]))
-                case  1: __PYX_VERIFY_RETURN_INT(long,  digit, +digits[0])
-                case -2:
-                    if (8 * sizeof(long) - 1 > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
-                            return (long) (((long)-1)*(((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+            if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(long, __Pyx_compact_pylong, __Pyx_PyLong_CompactValue(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_SignedDigitCount(x)) {
+                    case -2:
+                        if ((8 * sizeof(long) - 1 > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
+                                return (long) (((long)-1)*(((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 2:
-                    if (8 * sizeof(long) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
-                            return (long) ((((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                        break;
+                    case 2:
+                        if ((8 * sizeof(long) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
+                                return (long) ((((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -3:
-                    if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
-                            return (long) (((long)-1)*(((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                        break;
+                    case -3:
+                        if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
+                                return (long) (((long)-1)*(((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(long) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
-                            return (long) ((((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(long) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
+                                return (long) ((((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -4:
-                    if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 4 * PyLong_SHIFT) {
-                            return (long) (((long)-1)*(((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                        break;
+                    case -4:
+                        if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 4 * PyLong_SHIFT)) {
+                                return (long) (((long)-1)*(((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(long) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 4 * PyLong_SHIFT) {
-                            return (long) ((((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(long) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 4 * PyLong_SHIFT)) {
+                                return (long) ((((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
-            if (sizeof(long) <= sizeof(long)) {
+            if ((sizeof(long) <= sizeof(long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(long, long, PyLong_AsLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(long) <= sizeof(PY_LONG_LONG)) {
+            } else if ((sizeof(long) <= sizeof(PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(long, PY_LONG_LONG, PyLong_AsLongLong(x))
 #endif
             }
         }
         {
-#if CYTHON_COMPILING_IN_PYPY && !defined(_PyLong_AsByteArray)
-            PyErr_SetString(PyExc_RuntimeError,
-                            "_PyLong_AsByteArray() not available in PyPy, cannot convert large numbers");
-#else
             long val;
             PyObject *v = __Pyx_PyNumber_IntOrLong(x);
- #if PY_MAJOR_VERSION < 3
+#if PY_MAJOR_VERSION < 3
             if (likely(v) && !PyLong_Check(v)) {
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
- #endif
+#endif
             if (likely(v)) {
+                int ret = -1;
+#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
-                int ret = _PyLong_AsByteArray((PyLongObject *)v,
-                                              bytes, sizeof(val),
-                                              is_little, !is_unsigned);
+                ret = _PyLong_AsByteArray((PyLongObject *)v,
+                                           bytes, sizeof(val),
+                                           is_little, !is_unsigned);
+#else
+                PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
+                int bits, remaining_bits, is_negative = 0;
+                long idigit;
+                int chunk_size = (sizeof(long) < 8) ? 30 : 62;
+                if (unlikely(!PyLong_CheckExact(v))) {
+                    PyObject *tmp = v;
+                    v = PyNumber_Long(v);
+                    assert(PyLong_CheckExact(v));
+                    Py_DECREF(tmp);
+                    if (unlikely(!v)) return (long) -1;
+                }
+#if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                if (Py_SIZE(x) == 0)
+                    return (long) 0;
+                is_negative = Py_SIZE(x) < 0;
+#else
+                {
+                    int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
+                    if (unlikely(result < 0))
+                        return (long) -1;
+                    is_negative = result == 1;
+                }
+#endif
+                if (is_unsigned && unlikely(is_negative)) {
+                    goto raise_neg_overflow;
+                } else if (is_negative) {
+                    stepval = PyNumber_Invert(v);
+                    if (unlikely(!stepval))
+                        return (long) -1;
+                } else {
+                    stepval = __Pyx_NewRef(v);
+                }
+                val = (long) 0;
+                mask = PyLong_FromLong((1L << chunk_size) - 1); if (unlikely(!mask)) goto done;
+                shift = PyLong_FromLong(chunk_size); if (unlikely(!shift)) goto done;
+                for (bits = 0; bits < (int) sizeof(long) * 8 - chunk_size; bits += chunk_size) {
+                    PyObject *tmp, *digit;
+                    digit = PyNumber_And(stepval, mask);
+                    if (unlikely(!digit)) goto done;
+                    idigit = PyLong_AsLong(digit);
+                    Py_DECREF(digit);
+                    if (unlikely(idigit < 0)) goto done;
+                    tmp = PyNumber_Rshift(stepval, shift);
+                    if (unlikely(!tmp)) goto done;
+                    Py_DECREF(stepval); stepval = tmp;
+                    val |= ((long) idigit) << bits;
+                    #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                    if (Py_SIZE(stepval) == 0)
+                        goto unpacking_done;
+                    #endif
+                }
+                idigit = PyLong_AsLong(stepval);
+                if (unlikely(idigit < 0)) goto done;
+                remaining_bits = ((int) sizeof(long) * 8) - bits - (is_unsigned ? 0 : 1);
+                if (unlikely(idigit >= (1L << remaining_bits)))
+                    goto raise_overflow;
+                val |= ((long) idigit) << bits;
+            #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+            unpacking_done:
+            #endif
+                if (!is_unsigned) {
+                    if (unlikely(val & (((long) 1) << (sizeof(long) * 8 - 1))))
+                        goto raise_overflow;
+                    if (is_negative)
+                        val = ~val;
+                }
+                ret = 0;
+            done:
+                Py_XDECREF(shift);
+                Py_XDECREF(mask);
+                Py_XDECREF(stepval);
+#endif
                 Py_DECREF(v);
                 if (likely(!ret))
                     return val;
             }
-#endif
             return (long) -1;
         }
     } else {
         long val;
         PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
         if (!tmp) return (long) -1;
         val = __Pyx_PyInt_As_long(tmp);
@@ -8957,15 +12540,15 @@
     return (long) -1;
 }
 
 /* FastTypeChecks */
   #if CYTHON_COMPILING_IN_CPYTHON
 static int __Pyx_InBases(PyTypeObject *a, PyTypeObject *b) {
     while (a) {
-        a = a->tp_base;
+        a = __Pyx_PyType_GetSlot(a, tp_base, PyTypeObject*);
         if (a == b)
             return 1;
     }
     return b == &PyBaseObject_Type;
 }
 static CYTHON_INLINE int __Pyx_IsSubtype(PyTypeObject *a, PyTypeObject *b) {
     PyObject *mro;
@@ -8978,14 +12561,30 @@
             if (PyTuple_GET_ITEM(mro, i) == (PyObject *)b)
                 return 1;
         }
         return 0;
     }
     return __Pyx_InBases(a, b);
 }
+static CYTHON_INLINE int __Pyx_IsAnySubtype2(PyTypeObject *cls, PyTypeObject *a, PyTypeObject *b) {
+    PyObject *mro;
+    if (cls == a || cls == b) return 1;
+    mro = cls->tp_mro;
+    if (likely(mro)) {
+        Py_ssize_t i, n;
+        n = PyTuple_GET_SIZE(mro);
+        for (i = 0; i < n; i++) {
+            PyObject *base = PyTuple_GET_ITEM(mro, i);
+            if (base == (PyObject *)a || base == (PyObject *)b)
+                return 1;
+        }
+        return 0;
+    }
+    return __Pyx_InBases(cls, a) || __Pyx_InBases(cls, b);
+}
 #if PY_MAJOR_VERSION == 2
 static int __Pyx_inner_PyErr_GivenExceptionMatches2(PyObject *err, PyObject* exc_type1, PyObject* exc_type2) {
     PyObject *exception, *value, *tb;
     int res;
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ErrFetch(&exception, &value, &tb);
@@ -9002,19 +12601,19 @@
         }
     }
     __Pyx_ErrRestore(exception, value, tb);
     return res;
 }
 #else
 static CYTHON_INLINE int __Pyx_inner_PyErr_GivenExceptionMatches2(PyObject *err, PyObject* exc_type1, PyObject *exc_type2) {
-    int res = exc_type1 ? __Pyx_IsSubtype((PyTypeObject*)err, (PyTypeObject*)exc_type1) : 0;
-    if (!res) {
-        res = __Pyx_IsSubtype((PyTypeObject*)err, (PyTypeObject*)exc_type2);
+    if (exc_type1) {
+        return __Pyx_IsAnySubtype2((PyTypeObject*)err, (PyTypeObject*)exc_type1, (PyTypeObject*)exc_type2);
+    } else {
+        return __Pyx_IsSubtype((PyTypeObject*)err, (PyTypeObject*)exc_type2);
     }
-    return res;
 }
 #endif
 static int __Pyx_PyErr_GivenExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
     Py_ssize_t i, n;
     assert(PyExceptionClass_Check(exc_type));
     n = PyTuple_GET_SIZE(tuple);
 #if PY_MAJOR_VERSION >= 3
@@ -9083,50 +12682,60 @@
                 found_dot = 1;
             } else if (rt_from_call[i] < '0' || rt_from_call[i] > '9') {
                 break;
             }
             rtversion[i] = rt_from_call[i];
         }
         PyOS_snprintf(message, sizeof(message),
-                      "compiletime version %s of module '%.100s' "
+                      "compile time version %s of module '%.100s' "
                       "does not match runtime version %s",
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
 }
 
 /* InitStrings */
-  static int __Pyx_InitStrings(__Pyx_StringTabEntry *t) {
+  #if PY_MAJOR_VERSION >= 3
+static int __Pyx_InitString(__Pyx_StringTabEntry t, PyObject **str) {
+    if (t.is_unicode | t.is_str) {
+        if (t.intern) {
+            *str = PyUnicode_InternFromString(t.s);
+        } else if (t.encoding) {
+            *str = PyUnicode_Decode(t.s, t.n - 1, t.encoding, NULL);
+        } else {
+            *str = PyUnicode_FromStringAndSize(t.s, t.n - 1);
+        }
+    } else {
+        *str = PyBytes_FromStringAndSize(t.s, t.n - 1);
+    }
+    if (!*str)
+        return -1;
+    if (PyObject_Hash(*str) == -1)
+        return -1;
+    return 0;
+}
+#endif
+static int __Pyx_InitStrings(__Pyx_StringTabEntry *t) {
     while (t->p) {
-        #if PY_MAJOR_VERSION < 3
+        #if PY_MAJOR_VERSION >= 3
+        __Pyx_InitString(*t, t->p);
+        #else
         if (t->is_unicode) {
             *t->p = PyUnicode_DecodeUTF8(t->s, t->n - 1, NULL);
         } else if (t->intern) {
             *t->p = PyString_InternFromString(t->s);
         } else {
             *t->p = PyString_FromStringAndSize(t->s, t->n - 1);
         }
-        #else
-        if (t->is_unicode | t->is_str) {
-            if (t->intern) {
-                *t->p = PyUnicode_InternFromString(t->s);
-            } else if (t->encoding) {
-                *t->p = PyUnicode_Decode(t->s, t->n - 1, t->encoding, NULL);
-            } else {
-                *t->p = PyUnicode_FromStringAndSize(t->s, t->n - 1);
-            }
-        } else {
-            *t->p = PyBytes_FromStringAndSize(t->s, t->n - 1);
-        }
-        #endif
         if (!*t->p)
             return -1;
         if (PyObject_Hash(*t->p) == -1)
             return -1;
+        #endif
         ++t;
     }
     return 0;
 }
 
 static CYTHON_INLINE PyObject* __Pyx_PyUnicode_FromString(const char* c_str) {
     return __Pyx_PyUnicode_FromStringAndSize(c_str, (Py_ssize_t)strlen(c_str));
@@ -9180,15 +12789,15 @@
 #if PY_MAJOR_VERSION < 3 && __PYX_DEFAULT_STRING_ENCODING_IS_ASCII
             __Pyx_sys_getdefaultencoding_not_ascii &&
 #endif
             PyUnicode_Check(o)) {
         return __Pyx_PyUnicode_AsStringAndSize(o, length);
     } else
 #endif
-#if (!CYTHON_COMPILING_IN_PYPY) || (defined(PyByteArray_AS_STRING) && defined(PyByteArray_GET_SIZE))
+#if (!CYTHON_COMPILING_IN_PYPY && !CYTHON_COMPILING_IN_LIMITED_API) || (defined(PyByteArray_AS_STRING) && defined(PyByteArray_GET_SIZE))
     if (PyByteArray_Check(o)) {
         *length = PyByteArray_GET_SIZE(o);
         return PyByteArray_AS_STRING(o);
     } else
 #endif
     {
         char* result;
@@ -9209,30 +12818,34 @@
     int retval;
     if (unlikely(!x)) return -1;
     retval = __Pyx_PyObject_IsTrue(x);
     Py_DECREF(x);
     return retval;
 }
 static PyObject* __Pyx_PyNumber_IntOrLongWrongResultType(PyObject* result, const char* type_name) {
+    __Pyx_TypeName result_type_name = __Pyx_PyType_GetName(Py_TYPE(result));
 #if PY_MAJOR_VERSION >= 3
     if (PyLong_Check(result)) {
         if (PyErr_WarnFormat(PyExc_DeprecationWarning, 1,
-                "__int__ returned non-int (type %.200s).  "
-                "The ability to return an instance of a strict subclass of int "
-                "is deprecated, and may be removed in a future version of Python.",
-                Py_TYPE(result)->tp_name)) {
+                "__int__ returned non-int (type " __Pyx_FMT_TYPENAME ").  "
+                "The ability to return an instance of a strict subclass of int is deprecated, "
+                "and may be removed in a future version of Python.",
+                result_type_name)) {
+            __Pyx_DECREF_TypeName(result_type_name);
             Py_DECREF(result);
             return NULL;
         }
+        __Pyx_DECREF_TypeName(result_type_name);
         return result;
     }
 #endif
     PyErr_Format(PyExc_TypeError,
-                 "__%.4s__ returned non-%.4s (type %.200s)",
-                 type_name, type_name, Py_TYPE(result)->tp_name);
+                 "__%.4s__ returned non-%.4s (type " __Pyx_FMT_TYPENAME ")",
+                 type_name, type_name, result_type_name);
+    __Pyx_DECREF_TypeName(result_type_name);
     Py_DECREF(result);
     return NULL;
 }
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x) {
 #if CYTHON_USE_TYPE_SLOTS
   PyNumberMethods *m;
 #endif
@@ -9290,21 +12903,19 @@
         return PyInt_AS_LONG(b);
     else
         return PyInt_AsSsize_t(b);
   }
 #endif
   if (likely(PyLong_CheckExact(b))) {
     #if CYTHON_USE_PYLONG_INTERNALS
-    const digit* digits = ((PyLongObject*)b)->ob_digit;
-    const Py_ssize_t size = Py_SIZE(b);
-    if (likely(__Pyx_sst_abs(size) <= 1)) {
-        ival = likely(size) ? digits[0] : 0;
-        if (size == -1) ival = -ival;
-        return ival;
+    if (likely(__Pyx_PyLong_IsCompact(b))) {
+        return __Pyx_PyLong_CompactValue(b);
     } else {
+      const digit* digits = __Pyx_PyLong_Digits(b);
+      const Py_ssize_t size = __Pyx_PyLong_SignedDigitCount(b);
       switch (size) {
          case 2:
            if (8 * sizeof(Py_ssize_t) > 2 * PyLong_SHIFT) {
              return (Py_ssize_t) (((((size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
            }
            break;
          case -2:
@@ -9364,8 +12975,16 @@
   return b ? __Pyx_NewRef(Py_True) : __Pyx_NewRef(Py_False);
 }
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t ival) {
     return PyInt_FromSize_t(ival);
 }
 
 
+/* #### Code section: utility_code_pragmas_end ### */
+#ifdef _MSC_VER
+#pragma warning( pop )
+#endif
+
+
+
+/* #### Code section: end ### */
 #endif /* Py_PYTHON_H */
```

### Comparing `arcticpy-2.2/python/arcticpy/wrapper.pyx` & `arcticpy-2.3/python/arcticpy/wrapper.pyx`

 * *Files identical despite different names*

### Comparing `arcticpy-2.2/python/arcticpy.egg-info/SOURCES.txt` & `arcticpy-2.3/python/arcticpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arcticpy-2.2/setup.py` & `arcticpy-2.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 # Directories
 dir_wrapper = "python/arcticpy"
 dir_wrapper_src = os.path.join(dir_wrapper, "src")
 dir_wrapper_include = os.path.join(dir_wrapper, "include")
 dir_include = "include/"
 dir_src = "src/"
-dir_gsl = os.environ.get("DIR_GSL", '/usr/local/')
+dir_gsl = os.environ.get("DIR_GSL", "/usr/local/")
 dir_gsl_include = os.path.join(dir_gsl, "include")
 dir_gsl_lib = os.path.join(dir_gsl, "lib")
 
 # Clean (really needed anymore?)
 for root, dirs, files in os.walk(dir_wrapper, topdown=False):
     for name in files:
         file = os.path.join(root, name)
@@ -37,24 +37,30 @@
 
 ext_headers = [os.path.join(dir_include, header) for header in os.listdir(dir_include)]
 ext_sources = [os.path.join(dir_src, src) for src in os.listdir(dir_src)]
 
 extensions = [
     Extension(
         name="arcticpy.wrapper",
-        sources=[os.path.join(dir_wrapper, "wrapper.pyx"), os.path.join(dir_wrapper_src, "interface.cpp"), *ext_sources],
+        sources=[
+            os.path.join(dir_wrapper, "wrapper.pyx"),
+            os.path.join(dir_wrapper_src, "interface.cpp"),
+            *ext_sources,
+        ],
         language="c++",
         libraries=["gsl"],
         runtime_library_dirs=[dir_gsl_lib],
-        include_dirs=[dir_wrapper_include, dir_include, np.get_include(), dir_gsl_include],
+        include_dirs=[
+            dir_wrapper_include,
+            dir_include,
+            np.get_include(),
+            dir_gsl_include,
+        ],
         extra_compile_args=["-std=c++17", "-O3"],
-        define_macros=[('NPY_NO_DEPRECATED_API', 0)],
+        define_macros=[("NPY_NO_DEPRECATED_API", 0)],
     ),
 ]
 
 setup(
-    ext_modules=cythonize(
-        extensions,
-        compiler_directives={"language_level": "3"}
-    ),
+    ext_modules=cythonize(extensions, compiler_directives={"language_level": "3"}),
     headers=ext_headers,  # currently ignored (?)
 )
```

### Comparing `arcticpy-2.2/src/ccd.cpp` & `arcticpy-2.3/src/ccd.cpp`

 * *Files identical despite different names*

### Comparing `arcticpy-2.2/src/cti.cpp` & `arcticpy-2.3/src/cti.cpp`

 * *Files identical despite different names*

### Comparing `arcticpy-2.2/src/main.cpp` & `arcticpy-2.3/src/main.cpp`

 * *Files identical despite different names*

### Comparing `arcticpy-2.2/src/roe.cpp` & `arcticpy-2.3/src/roe.cpp`

 * *Files identical despite different names*

### Comparing `arcticpy-2.2/src/trap_managers.cpp` & `arcticpy-2.3/src/trap_managers.cpp`

 * *Files identical despite different names*

### Comparing `arcticpy-2.2/src/traps.cpp` & `arcticpy-2.3/src/traps.cpp`

 * *Files identical despite different names*

### Comparing `arcticpy-2.2/src/util.cpp` & `arcticpy-2.3/src/util.cpp`

 * *Files identical despite different names*

### Comparing `arcticpy-2.2/test/catch2/catch.hpp` & `arcticpy-2.3/test/catch2/catch.hpp`

 * *Files identical despite different names*

### Comparing `arcticpy-2.2/test/test_arcticpy.py` & `arcticpy-2.3/test/test_arcticpy.py`

 * *Files identical despite different names*

### Comparing `arcticpy-2.2/test/test_ccd.cpp` & `arcticpy-2.3/test/test_ccd.cpp`

 * *Files identical despite different names*

### Comparing `arcticpy-2.2/test/test_cti.cpp` & `arcticpy-2.3/test/test_cti.cpp`

 * *Files identical despite different names*

### Comparing `arcticpy-2.2/test/test_lib.cpp` & `arcticpy-2.3/test/test_lib.cpp`

 * *Files identical despite different names*

### Comparing `arcticpy-2.2/test/test_roe.cpp` & `arcticpy-2.3/test/test_roe.cpp`

 * *Files identical despite different names*

### Comparing `arcticpy-2.2/test/test_trap_managers.cpp` & `arcticpy-2.3/test/test_trap_managers.cpp`

 * *Files identical despite different names*

### Comparing `arcticpy-2.2/test/test_traps.cpp` & `arcticpy-2.3/test/test_traps.cpp`

 * *Files identical despite different names*

### Comparing `arcticpy-2.2/test/test_util.cpp` & `arcticpy-2.3/test/test_util.cpp`

 * *Files identical despite different names*

### Comparing `arcticpy-2.2/tst_cil.py` & `arcticpy-2.3/tst_cil.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,80 +1,80 @@
 import numpy as np
 import arcticpy as ac
 import numpy as np
 import arcticpy
 import time
 import matplotlib.pyplot as plt
-np.set_printoptions(linewidth=205,edgeitems=56,suppress=True)
+
+np.set_printoptions(linewidth=205, edgeitems=56, suppress=True)
 
 
 #
 # Test different values of pruning (edit here)
 #
-parallel_prune_n_electrons=1e-9
-parallel_prune_frequency=20
-parallel_express=0
+parallel_prune_n_electrons = 1e-9
+parallel_prune_frequency = 20
+parallel_express = 0
 
 #
 # Set up test image
 #
-image_pre_cti = np.zeros((2000,1))+200
-image_pre_cti[0:5,:]+=700
-image_pre_cti[500:505,:]+=700
-image_pre_cti[1000:1005,:]+=7000
-image_pre_cti[1500:1505,:]+=70000
+image_pre_cti = np.zeros((2000, 1)) + 200
+image_pre_cti[0:5, :] += 700
+image_pre_cti[500:505, :] += 700
+image_pre_cti[1000:1005, :] += 7000
+image_pre_cti[1500:1505, :] += 70000
 
-parallel_trap_list = [
-    ac.TrapInstantCapture(density=3, release_timescale=2)
-]
+parallel_trap_list = [ac.TrapInstantCapture(density=3, release_timescale=2)]
 
 parallel_slowtrap_list = [
     ac.TrapSlowCapture(density=3, release_timescale=2, capture_timescale=5.0)
 ]
 
 parallel_ccd = ac.CCD(
     well_fill_power=0.58, well_notch_depth=0.0, full_well_depth=200000.0
 )
 
 image_post_cti_0 = ac.add_cti(
     image=image_pre_cti,
     parallel_express=1,
     parallel_traps=parallel_trap_list,
     parallel_ccd=parallel_ccd,
-    parallel_roe=ac.ROEChargeInjection()
+    parallel_roe=ac.ROEChargeInjection(),
 )
 
 
 image_post_cti_1 = ac.add_cti(
     image=image_pre_cti,
     parallel_express=1,
     parallel_traps=parallel_slowtrap_list,
     parallel_ccd=parallel_ccd,
-    parallel_roe=ac.ROEChargeInjection()
+    parallel_roe=ac.ROEChargeInjection(),
 )
 
 
 print(np.max(abs(image_post_cti_0 - image_post_cti_1)))
 
-rn=ac.ReadNoise(sigma=-4.5)
+rn = ac.ReadNoise(sigma=-4.5)
 print(rn.sigma)
 
 
 #
-# Plot 
+# Plot
 #
 n_rows_in_image, n_columns_in_image = image_pre_cti.shape
 pixels = np.arange(n_rows_in_image)
 colours = ["#1199ff", "#ee4400", "#7711dd", "#44dd44", "#775533"]
 fig, ax = plt.subplots()
-ax.plot(pixels, image_pre_cti[:,0], alpha=0.8, label="%d")
-ax.plot(pixels, image_post_cti_0[:,0], alpha=0.8, label="%d")
-ax.plot(pixels, image_post_cti_1[:,0], alpha=0.8, label="%d")
+ax.plot(pixels, image_pre_cti[:, 0], alpha=0.8, label="%d")
+ax.plot(pixels, image_post_cti_0[:, 0], alpha=0.8, label="%d")
+ax.plot(pixels, image_post_cti_1[:, 0], alpha=0.8, label="%d")
 
-ax.set(xlabel='pixel', ylabel='offset bias [n_e]', #yscale='log',
-       title='Effect of CTI')
+ax.set(
+    xlabel="pixel", ylabel="offset bias [n_e]", title="Effect of CTI"  # yscale='log',
+)
 ax.grid()
 plt.tight_layout()
-plt.show(block=False)   
-plt.show()   
+plt.show(block=False)
+plt.show()
 
-print(pixels.shape,image_post_cti_1[:,0].shape)
+print(pixels.shape, image_post_cti_1[:, 0].shape)
```

### Comparing `arcticpy-2.2/tst_correct.py` & `arcticpy-2.3/tst_correct.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import arcticpy as arctic
 import autoarray as aa
 import time
 
-image_path = "/Users/rjm/GitHub/testdata/je0o30lzq"
+data_path = "/Users/rjm/GitHub/testdata/je0o30lzq"
 
 # Load each quadrant of the image  (see pypi.org/project/autoarray)
 image_A, image_B, image_C, image_D = [
     aa.acs.ImageACS.from_fits(
-        file_path=image_path + "_raw.fits",
+        file_path=data_path + "_raw.fits",
         quadrant_letter=quadrant,
         bias_subtract_via_bias_file=True,
         bias_subtract_via_prescan=True,
     ).native
     for quadrant in ["A", "B", "C", "D"]
 ]
 
@@ -19,29 +19,29 @@
 date = 2400000.5 + image_A.header.modified_julian_date
 roe, ccd, traps = arctic.CTI_model_for_HST_ACS(date)
 
 # Remove CTI  (see remove_cti() in src/cti.cpp)
 start = time.time_ns()
 image_out_A, image_out_B, image_out_C, image_out_D = [
     arctic.remove_cti(
-           image=image,
-           n_iterations=5,
-           parallel_roe=roe,
-           parallel_ccd=ccd,
-           parallel_traps=traps,
-           parallel_express=5,
-           verbosity=1,
+        image=image,
+        n_iterations=5,
+        parallel_roe=roe,
+        parallel_ccd=ccd,
+        parallel_traps=traps,
+        parallel_express=5,
+        verbosity=1,
     )
     for image in [image_A, image_B, image_C, image_D]
 ]
 print(f"Time taken = {((time.time_ns() - start)/1e9)} s")
 
 # Save the corrected image
 aa.acs.output_quadrants_to_fits(
-    file_path=image_path + "_out.fits",
+    file_path=data_path + "_out.fits",
     quadrant_a=image_out_A,
     quadrant_b=image_out_B,
     quadrant_c=image_out_C,
     quadrant_d=image_out_D,
     header_a=image_A.header,
     header_b=image_B.header,
     header_c=image_C.header,
```

### Comparing `arcticpy-2.2/tst_covar.py` & `arcticpy-2.3/tst_covar.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import arcticpy as arctic
 import autoarray as aa
 import time
 import numpy as np
 
-image_path = "/Users/rjm/GitHub/testdata/je0o30lzq"
+data_path = "/Users/rjm/GitHub/testdata/je0o30lzq"
 
 # Load each quadrant of the image  (see pypi.org/project/autoarray)
 image_A, image_B, image_C, image_D = [
     aa.acs.ImageACS.from_fits(
-        file_path=image_path + "_raw.fits",
+        file_path=data_path + "_raw.fits",
         quadrant_letter=quadrant,
         bias_subtract_via_bias_file=True,
         bias_subtract_via_prescan=True,
     ).native
     for quadrant in ["A", "B", "C", "D"]
 ]
 
@@ -20,77 +20,63 @@
 date = 2400000.5 + image_A.header.modified_julian_date
 roe, ccd, traps = arctic.CTI_model_for_HST_ACS(date)
 
 
 noise = arctic.ReadNoise(sigma_readnoise=4.5)
 
 
-background_level= 2.5*np.median(image_A) - 1.5*np.mean(image_A)
-background_level= np.max(np.median(image_A),0)
+background_level = 2.5 * np.median(image_A) - 1.5 * np.mean(image_A)
+background_level = np.max(np.median(image_A), 0)
 
 print(background_level)
 
-noise.optimise_parameters(background_level,
-        n_pixels=2066, 
-        parallel_traps=traps,
-        parallel_ccd=ccd,
-        parallel_roe=roe) #,
+noise.optimise_parameters(
+    background_level,
+    n_pixels=2066,
+    parallel_traps=traps,
+    parallel_ccd=ccd,
+    parallel_roe=roe,
+)  # ,
 #        serial_traps=traps,
 #        serial_ccd=ccd,
 #        serial_roe=roe)
 
 
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
 # Or manual CTI model  (see class docstrings in src/<traps,roe,ccd>.cpp)
-#traps = [
+# traps = [
 #    arctic.TrapInstantCapture(density=0.6, release_timescale=0.74),
 #    arctic.TrapInstantCapture(density=1.6, release_timescale=7.70),
 #    arctic.TrapInstantCapture(density=1.4, release_timescale=37.0),
-#]
-#roe = arctic.ROE()
-#ccd = arctic.CCD(full_well_depth=84700, well_fill_power=0.478)
+# ]
+# roe = arctic.ROE()
+# ccd = arctic.CCD(full_well_depth=84700, well_fill_power=0.478)
 
 
 # Remove CTI  (see remove_cti() in src/cti.cpp)
-#start = time.time_ns()
-#image_out_A, image_out_B, image_out_C, image_out_D = [
+# start = time.time_ns()
+# image_out_A, image_out_B, image_out_C, image_out_D = [
 #    arctic.remove_cti(
 #           image=image,
 #           n_iterations=5,
 #           parallel_roe=roe,
 #           parallel_ccd=ccd,
 #           parallel_traps=traps,
 #           parallel_express=5,
 #           verbosity=1,
 #    )
 #    for image in [image_A, image_B, image_C, image_D]
-#]
-#print(f"Time taken = {((time.time_ns() - start)/1e9)} s")
+# ]
+# print(f"Time taken = {((time.time_ns() - start)/1e9)} s")
 
 # Save the corrected image
-#aa.acs.output_quadrants_to_fits(
-#    file_path=image_path + "_out.fits",
+# aa.acs.output_quadrants_to_fits(
+#    file_path=data_path + "_out.fits",
 #    quadrant_a=image_out_A,
 #    quadrant_b=image_out_B,
 #    quadrant_c=image_out_C,
 #    quadrant_d=image_out_D,
 #    header_a=image_A.header,
 #    header_b=image_B.header,
 #    header_c=image_C.header,
 #    header_d=image_D.header,
 #    overwrite=True,
-#)
+# )
```

### Comparing `arcticpy-2.2/tst_dark.py` & `arcticpy-2.3/tst_dark.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,57 +1,56 @@
 import numpy as np
 import arcticpy
 import time
 import matplotlib.pyplot as plt
-np.set_printoptions(linewidth=205,edgeitems=56,suppress=True)
+
+np.set_printoptions(linewidth=205, edgeitems=56, suppress=True)
 
 
 #
 # Test different values of pruning (edit here)
 #
-parallel_prune_n_electrons=1e-6
-parallel_prune_frequency=10
-parallel_express=2
-stats_range=np.arange(500,1900)
-plot_range=np.arange(1200,1400)
+parallel_prune_n_electrons = 1e-6
+parallel_prune_frequency = 10
+parallel_express = 2
+stats_range = np.arange(500, 1900)
+plot_range = np.arange(1200, 1400)
 
 
 #
 # Set up test image
 #
-dark_level=300
-read_noise=4.5
-
-image_model = np.zeros((2000,100))
-#image_model += dark_level
-image_model += np.random.poisson(dark_level,image_model.shape)
-#image_model[20:1900,:]+=dark_level
-#image_model += np.random.normal(dark_level,np.sqrt(dark_level)/1000,image_model.shape)
+dark_level = 300
+read_noise = 4.5
 
+image_model = np.zeros((2000, 100))
+# image_model += dark_level
+image_model += np.random.poisson(dark_level, image_model.shape)
+# image_model[20:1900,:]+=dark_level
+# image_model += np.random.normal(dark_level,np.sqrt(dark_level)/1000,image_model.shape)
 
 
 parallel_traps = [
-    arcticpy.TrapInstantCapture(density=1.0, release_timescale=(-1/np.log(0.5))),
-    #arcticpy.TrapInstantCapture(density=10.0, release_timescale=100),
-    #arcticpy.TrapSlowCapture(density=10.0, release_timescale=(-1/np.log(0.5)), capture_timescale=0.001),
-    #arcticpy.TrapSlowCapture(density=10.0, release_timescale=(4), capture_timescale=0.001),
-    #arcticpy.TrapInstantCaptureContinuum(density=10.0, release_timescale=(1.), release_timescale_sigma=0.1),
-    #arcticpy.TrapSlowCaptureContinuum(density=10.0, release_timescale=(1.), capture_timescale=1, release_timescale_sigma=0.1),
+    arcticpy.TrapInstantCapture(density=1.0, release_timescale=(-1 / np.log(0.5))),
+    # arcticpy.TrapInstantCapture(density=10.0, release_timescale=100),
+    # arcticpy.TrapSlowCapture(density=10.0, release_timescale=(-1/np.log(0.5)), capture_timescale=0.001),
+    # arcticpy.TrapSlowCapture(density=10.0, release_timescale=(4), capture_timescale=0.001),
+    # arcticpy.TrapInstantCaptureContinuum(density=10.0, release_timescale=(1.), release_timescale_sigma=0.1),
+    # arcticpy.TrapSlowCaptureContinuum(density=10.0, release_timescale=(1.), capture_timescale=1, release_timescale_sigma=0.1),
 ]
 
 parallel_ccd = arcticpy.CCD(full_well_depth=10000, well_fill_power=1.0)
 parallel_roe = arcticpy.ROE(
     empty_traps_between_columns=True,
     empty_traps_for_first_transfers=False,
     overscan_start=1900,
-    prescan_offset=50
+    prescan_offset=50,
 )
 
 
-
 #
 # Add CTI
 #
 
 start = time.time_ns()
 
 image_post_cti = arcticpy.add_cti(
@@ -59,95 +58,114 @@
     parallel_traps=parallel_traps,
     parallel_ccd=parallel_ccd,
     parallel_roe=parallel_roe,
     parallel_express=parallel_express,
     parallel_prune_n_electrons=parallel_prune_n_electrons,
     parallel_prune_frequency=parallel_prune_frequency,
     allow_negative_pixels=1,
-    verbosity=0
+    verbosity=0,
 )
 
 print(f"Clocking Time Noisy = {((time.time_ns() - start)/1e9)} s")
-print("mean level (true)    ",np.mean(image_model[stats_range,:]))
-print("mean level (trailed) ",np.mean(image_post_cti[stats_range,:]))
+print("mean level (true)    ", np.mean(image_model[stats_range, :]))
+print("mean level (trailed) ", np.mean(image_post_cti[stats_range, :]))
 
 
 #
 # Add read noise
 #
-read_noise_image = np.random.normal(0,read_noise,image_model.shape)
+read_noise_image = np.random.normal(0, read_noise, image_model.shape)
 image_pre_cti_noisy = image_model + read_noise_image
 image_post_cti_noisy = image_post_cti + read_noise_image
 
 read_noise_obj = arcticpy.ReadNoise(read_noise)
 read_noise_obj.set_arctic_parameters(
     parallel_traps=parallel_traps,
     parallel_ccd=parallel_ccd,
     parallel_roe=parallel_roe,
     parallel_express=parallel_express,
     parallel_prune_n_electrons=parallel_prune_n_electrons,
     parallel_prune_frequency=parallel_prune_frequency,
 )
 read_noise_obj.optimise_SR_fraction_from_image(image_post_cti_noisy)
-print("Optimum S+R fraction: ",read_noise_obj.SRfrac_optimised)
+print("Optimum S+R fraction: ", read_noise_obj.SRfrac_optimised)
 read_noise_obj.SRfrac_optimised = 0.3
 
 #
 # Correct CTI
 #
 start = time.time_ns()
 image_corrected_noisy = arcticpy.remove_cti(
-    image=image_post_cti_noisy, n_iterations=19,
+    image=image_post_cti_noisy,
+    n_iterations=19,
     parallel_traps=parallel_traps,
     parallel_ccd=parallel_ccd,
     parallel_roe=parallel_roe,
     parallel_express=parallel_express,
     parallel_prune_n_electrons=parallel_prune_n_electrons,
     parallel_prune_frequency=parallel_prune_frequency,
     allow_negative_pixels=1,
     read_noise=read_noise_obj,
-    verbosity=0
+    verbosity=0,
 )
 print(f"Correction Time Noisy = {((time.time_ns() - start)/1e9)} s")
-print("mean level (correct) ",np.mean(image_corrected_noisy[stats_range,:]),
-      " +/-",np.std(image_corrected_noisy[stats_range,:]) 
-           / np.sqrt(np.size(image_corrected_noisy[stats_range,:])))
-
-
+print(
+    "mean level (correct) ",
+    np.mean(image_corrected_noisy[stats_range, :]),
+    " +/-",
+    np.std(image_corrected_noisy[stats_range, :])
+    / np.sqrt(np.size(image_corrected_noisy[stats_range, :])),
+)
 
 
 #
-# Plot 
+# Plot
 #
 n_rows_in_image, n_columns_in_image = image_model.shape
 pixels = np.arange(n_rows_in_image)
 colours = ["#1199ff", "#ee4400", "#7711dd", "#44dd44", "#775533"]
 fig, ax = plt.subplots()
-ax.plot(pixels[plot_range], image_model[plot_range,0], alpha=0.8, label="No read noise")
-#ax.plot(pixels[0:50], image_post_cti_nonoise[0:50,0]-image_model[0,0:50], alpha=0.8, label="%d")
-ax.plot(pixels[plot_range], image_pre_cti_noisy[plot_range,0], alpha=0.8, label="Ideal correction")
-ax.plot(pixels[plot_range], image_corrected_noisy[plot_range,0], alpha=0.8, label="Achieved correction")
-ax.plot(pixels[plot_range], image_post_cti_noisy[plot_range,0], alpha=0.8, label="Downloaded")
+ax.plot(
+    pixels[plot_range], image_model[plot_range, 0], alpha=0.8, label="No read noise"
+)
+# ax.plot(pixels[0:50], image_post_cti_nonoise[0:50,0]-image_model[0,0:50], alpha=0.8, label="%d")
+ax.plot(
+    pixels[plot_range],
+    image_pre_cti_noisy[plot_range, 0],
+    alpha=0.8,
+    label="Ideal correction",
+)
+ax.plot(
+    pixels[plot_range],
+    image_corrected_noisy[plot_range, 0],
+    alpha=0.8,
+    label="Achieved correction",
+)
+ax.plot(
+    pixels[plot_range],
+    image_post_cti_noisy[plot_range, 0],
+    alpha=0.8,
+    label="Downloaded",
+)
 
-ax.set(xlabel='pixel', ylabel='offset bias [n_e]',
-       title='Effect of CTI')
+ax.set(xlabel="pixel", ylabel="offset bias [n_e]", title="Effect of CTI")
 ax.grid()
 ax.legend()
 plt.tight_layout()
-#plt.ioff()
-#plt.pause(0.01)
-plt.show(block=False)   
-#plt.gcf().canvas.draw_idle()
-#plt.gcf().canvas.start_event_loop(0.3)
+# plt.ioff()
+# plt.pause(0.01)
+plt.show(block=False)
+# plt.gcf().canvas.draw_idle()
+# plt.gcf().canvas.start_event_loop(0.3)
 
-#import time
-#time.sleep(2)
+# import time
+# time.sleep(2)
 # Press enter to continue
 input("Press Enter to continue...")
 # Press any key to continue
-#print("Press any key to continue...")
-#orig_settings = termios.tcgetattr(sys.stdin)
-#tty.setcbreak(sys.stdin)
-#x = 0
-#while x == 0:
+# print("Press any key to continue...")
+# orig_settings = termios.tcgetattr(sys.stdin)
+# tty.setcbreak(sys.stdin)
+# x = 0
+# while x == 0:
 #    x=sys.stdin.read(1)[0]
-#termios.tcsetattr(sys.stdin, termios.TCSADRAIN, orig_settings)  
+# termios.tcsetattr(sys.stdin, termios.TCSADRAIN, orig_settings)
```

### Comparing `arcticpy-2.2/tst_negative_image.py` & `arcticpy-2.3/tst_negative_image.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,165 +1,164 @@
 import numpy as np
 import arcticpy
 import time
 import matplotlib.pyplot as plt
-np.set_printoptions(linewidth=205,edgeitems=56,suppress=True)
 
+np.set_printoptions(linewidth=205, edgeitems=56, suppress=True)
 
-parallel_prune_n_electrons=1e-18
-parallel_prune_frequency=0
-parallel_express=1
+
+parallel_prune_n_electrons = 1e-18
+parallel_prune_frequency = 0
+parallel_express = 1
 
 #
 # Test different values of pruning (edit here)
 #
-parallel_prune_n_electrons=1e-6
-parallel_prune_frequency=10
-parallel_express=0
+parallel_prune_n_electrons = 1e-6
+parallel_prune_frequency = 10
+parallel_express = 0
 
 #
 # Set up test image
 #
-image_model = np.zeros((50,1))+0
-image_model[3:8,:]+=70
-#image_model[12:17,:]-=20
-#image_model[13:17,:]-=50
-image_model[12:17,:]-=70
-#image_model[500:505,:]+=700
-#image_model[1000:1005,:]+=700
-#image_model[1500:1505,:]+=700
+image_model = np.zeros((50, 1)) + 0
+image_model[3:8, :] += 70
+# image_model[12:17,:]-=20
+# image_model[13:17,:]-=50
+image_model[12:17, :] -= 70
+# image_model[500:505,:]+=700
+# image_model[1000:1005,:]+=700
+# image_model[1500:1505,:]+=700
 
 parallel_traps = [
-    arcticpy.TrapInstantCapture(density=10.0, release_timescale=(-1/np.log(0.5))),
-    #arcticpy.TrapInstantCapture(density=10.0, release_timescale=100),
-    #arcticpy.TrapSlowCapture(density=10.0, release_timescale=(-1/np.log(0.5)), capture_timescale=0.001),
-    #arcticpy.TrapSlowCapture(density=10.0, release_timescale=(4), capture_timescale=0.001),
-    #arcticpy.TrapInstantCaptureContinuum(density=10.0, release_timescale=(1.), release_timescale_sigma=0.1),
-    #arcticpy.TrapSlowCaptureContinuum(density=10.0, release_timescale=(1.), capture_timescale=1, release_timescale_sigma=0.1),
+    arcticpy.TrapInstantCapture(density=10.0, release_timescale=(-1 / np.log(0.5))),
+    # arcticpy.TrapInstantCapture(density=10.0, release_timescale=100),
+    # arcticpy.TrapSlowCapture(density=10.0, release_timescale=(-1/np.log(0.5)), capture_timescale=0.001),
+    # arcticpy.TrapSlowCapture(density=10.0, release_timescale=(4), capture_timescale=0.001),
+    # arcticpy.TrapInstantCaptureContinuum(density=10.0, release_timescale=(1.), release_timescale_sigma=0.1),
+    # arcticpy.TrapSlowCaptureContinuum(density=10.0, release_timescale=(1.), capture_timescale=1, release_timescale_sigma=0.1),
 ]
 
-parallel_ccd = arcticpy.CCD(full_well_depth=1000, 
-                            well_fill_power=1.0, 
-                            well_notch_depth=0.0,
-                            first_electron_fill=0.0)
+parallel_ccd = arcticpy.CCD(
+    full_well_depth=1000,
+    well_fill_power=1.0,
+    well_notch_depth=0.0,
+    first_electron_fill=0.0,
+)
 parallel_roe = arcticpy.ROE(
     empty_traps_between_columns=True,
     empty_traps_for_first_transfers=True,
     overscan_start=1990,
-    prescan_offset=10
+    prescan_offset=10,
 )
-#parallel_roe = arcticpy.ROEChargeInjection()
-
+# parallel_roe = arcticpy.ROEChargeInjection()
 
 
 #
 # Noisy image
 #
-image_pre_cti_noisy = image_model #+ np.random.normal(0,4.5,image_model.shape)
-#image_pre_cti = np.maximum(image_pre_cti,np.zeros(image_pre_cti.shape));
-#print(image_pre_cti[0:10,0])
-parallel_ccd_alt = arcticpy.CCD(full_well_depth=1000, 
-                                well_fill_power=1.0, 
-                                well_notch_depth=-200,
-                                first_electron_fill=0.)
+image_pre_cti_noisy = image_model  # + np.random.normal(0,4.5,image_model.shape)
+# image_pre_cti = np.maximum(image_pre_cti,np.zeros(image_pre_cti.shape));
+# print(image_pre_cti[0:10,0])
+parallel_ccd_alt = arcticpy.CCD(
+    full_well_depth=1000,
+    well_fill_power=1.0,
+    well_notch_depth=-200,
+    first_electron_fill=0.0,
+)
 
 start = time.time_ns()
 
 image_post_cti_noisy = arcticpy.add_cti(
     image=image_pre_cti_noisy,
     parallel_traps=parallel_traps,
     parallel_ccd=parallel_ccd_alt,
     parallel_roe=parallel_roe,
     parallel_express=parallel_express,
     parallel_prune_n_electrons=parallel_prune_n_electrons,
     parallel_prune_frequency=parallel_prune_frequency,
-    verbosity=0
+    verbosity=0,
 )
 
 print(f"Clocking Time Noisy = {((time.time_ns() - start)/1e9)} s")
 
 #
 # Noise-free image
 #
 
 image_pre_cti = image_model
-#print(image_pre_cti[0:10,0])
+# print(image_pre_cti[0:10,0])
 
 start = time.time_ns()
 
 image_post_cti_nonoise = arcticpy.add_cti(
     image=image_pre_cti,
     parallel_traps=parallel_traps,
     parallel_ccd=parallel_ccd,
     parallel_roe=parallel_roe,
     parallel_express=1,
     parallel_prune_n_electrons=parallel_prune_n_electrons,
     parallel_prune_frequency=0,
     allow_negative_pixels=1,
-    verbosity=0
+    verbosity=0,
 )
 
 print(f"Clocking Time No Noise = {((time.time_ns() - start)/1e9)} s")
-print(np.sum(image_model),image_model[0:49,0])
-print(np.sum(image_post_cti_noisy),image_post_cti_noisy[0:49,0])
-print(np.sum(image_post_cti_nonoise),image_post_cti_nonoise[0:49,0])
-
+print(np.sum(image_model), image_model[0:49, 0])
+print(np.sum(image_post_cti_noisy), image_post_cti_noisy[0:49, 0])
+print(np.sum(image_post_cti_nonoise), image_post_cti_nonoise[0:49, 0])
 
 
 #
 # Correct CTI
 #
-#start = time.time_ns()
-#image_corrected_nonoise = arcticpy.remove_cti(
+# start = time.time_ns()
+# image_corrected_nonoise = arcticpy.remove_cti(
 #    image=image_post_cti_nonoise, n_iterations=5,
 #    parallel_traps=parallel_traps,
 #    parallel_ccd=parallel_ccd,
 #    parallel_roe=parallel_roe,
 #    parallel_express=parallel_express,
 #    parallel_prune_n_electrons=parallel_prune_n_electrons,
 #    parallel_prune_frequency=parallel_prune_frequency,
 #    allow_negative_pixels=1,
 #    verbosity=0
-#)
-#print(f"Correction Time No Noise = {((time.time_ns() - start)/1e9)} s")
-
-
-
+# )
+# print(f"Correction Time No Noise = {((time.time_ns() - start)/1e9)} s")
 
 
 #
-# Plot 
+# Plot
 #
 n_rows_in_image, n_columns_in_image = image_post_cti_nonoise.shape
 pixels = np.arange(n_rows_in_image)
 colours = ["#1199ff", "#ee4400", "#7711dd", "#44dd44", "#775533"]
 fig, ax = plt.subplots()
-ax.plot(pixels[0:50], image_model[0:50,0], alpha=0.8, label="Input")
-#ax.plot(pixels[0:50], image_post_cti_nonoise[0:50,0]-image_model[0,0:50], alpha=0.8, label="%d")
-#ax.plot(pixels[0:50], image_post_cti[0:50,0], alpha=0.8, label="%d")
-ax.plot(pixels[0:50], image_post_cti_nonoise[0:50,0], alpha=0.8, label="Trailed")
-ax.plot(pixels[0:50], image_post_cti_noisy[0:50,0], alpha=0.8, label="Alt CCD")
-#ax.plot(pixels[0:50], image_corrected_nonoise[0:50,0], alpha=0.8, label="%d")
+ax.plot(pixels[0:50], image_model[0:50, 0], alpha=0.8, label="Input")
+# ax.plot(pixels[0:50], image_post_cti_nonoise[0:50,0]-image_model[0,0:50], alpha=0.8, label="%d")
+# ax.plot(pixels[0:50], image_post_cti[0:50,0], alpha=0.8, label="%d")
+ax.plot(pixels[0:50], image_post_cti_nonoise[0:50, 0], alpha=0.8, label="Trailed")
+ax.plot(pixels[0:50], image_post_cti_noisy[0:50, 0], alpha=0.8, label="Alt CCD")
+# ax.plot(pixels[0:50], image_corrected_nonoise[0:50,0], alpha=0.8, label="%d")
 
-ax.set(xlabel='pixel', ylabel='offset bias [n_e]',
-       title='Effect of CTI')
+ax.set(xlabel="pixel", ylabel="offset bias [n_e]", title="Effect of CTI")
 ax.grid()
 ax.legend()
 plt.tight_layout()
-#plt.ioff()
-#plt.pause(0.01)
-plt.show(block=False)   
-#plt.gcf().canvas.draw_idle()
-#plt.gcf().canvas.start_event_loop(0.3)
+# plt.ioff()
+# plt.pause(0.01)
+plt.show(block=False)
+# plt.gcf().canvas.draw_idle()
+# plt.gcf().canvas.start_event_loop(0.3)
 
-#import time
-#time.sleep(2)
+# import time
+# time.sleep(2)
 # Press enter to continue
 input("Press Enter to continue...")
 # Press any key to continue
-#print("Press any key to continue...")
-#orig_settings = termios.tcgetattr(sys.stdin)
-#tty.setcbreak(sys.stdin)
-#x = 0
-#while x == 0:
+# print("Press any key to continue...")
+# orig_settings = termios.tcgetattr(sys.stdin)
+# tty.setcbreak(sys.stdin)
+# x = 0
+# while x == 0:
 #    x=sys.stdin.read(1)[0]
-#termios.tcsetattr(sys.stdin, termios.TCSADRAIN, orig_settings)  
+# termios.tcsetattr(sys.stdin, termios.TCSADRAIN, orig_settings)
```

