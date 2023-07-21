# Comparing `tmp/simframe-1.0.3rc1.tar.gz` & `tmp/simframe-1.0.4rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simframe-1.0.3rc1.tar", last modified: Wed May 24 13:40:49 2023, max compression
+gzip compressed data, was "simframe-1.0.4rc0.tar", last modified: Fri Jul 21 11:26:37 2023, max compression
```

## Comparing `simframe-1.0.3rc1.tar` & `simframe-1.0.4rc0.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-24 13:40:48.829551 simframe-1.0.3rc1/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1532 2022-03-10 11:03:13.000000 simframe-1.0.3rc1/LICENSE
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      198 2022-03-10 11:03:13.000000 simframe-1.0.3rc1/MANIFEST.in
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     4697 2023-05-24 13:40:48.826547 simframe-1.0.3rc1/PKG-INFO
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     3524 2023-05-12 14:36:17.000000 simframe-1.0.3rc1/README.md
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-24 13:40:46.132077 simframe-1.0.3rc1/docs/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      638 2021-12-24 09:33:56.000000 simframe-1.0.3rc1/docs/Makefile
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      799 2021-12-24 09:33:56.000000 simframe-1.0.3rc1/docs/make.bat
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      124 2023-05-24 13:30:47.000000 simframe-1.0.3rc1/docs/requirements.txt
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-24 13:40:46.236964 simframe-1.0.3rc1/docs/source/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      421 2021-12-24 09:33:56.000000 simframe-1.0.3rc1/docs/source/api.rst
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1828 2022-03-10 11:03:13.000000 simframe-1.0.3rc1/docs/source/conf.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1032 2022-03-10 11:03:13.000000 simframe-1.0.3rc1/docs/source/index.rst
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-24 13:40:46.814416 simframe-1.0.3rc1/examples/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)    63171 2023-05-24 13:30:47.000000 simframe-1.0.3rc1/examples/1_simple_integration.ipynb
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)    49497 2023-05-24 13:30:47.000000 simframe-1.0.3rc1/examples/2_advanced_integration.ipynb
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)   125218 2023-05-24 13:30:47.000000 simframe-1.0.3rc1/examples/3_updating.ipynb
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)    13834 2022-03-29 12:45:07.000000 simframe-1.0.3rc1/examples/4_custom_schemes.ipynb
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)   381957 2022-03-29 12:45:07.000000 simframe-1.0.3rc1/examples/5_adaptive_schemes.ipynb
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)    68256 2022-03-29 12:45:07.000000 simframe-1.0.3rc1/examples/6_implicit_integration.ipynb
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1380 2022-03-29 12:45:07.000000 simframe-1.0.3rc1/examples/A_citation.ipynb
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2648 2022-03-29 12:45:07.000000 simframe-1.0.3rc1/examples/B_contrib_bug_feature.ipynb
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)   391549 2022-03-29 12:45:07.000000 simframe-1.0.3rc1/examples/example_compartmental_models.ipynb
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)  4006805 2022-03-29 12:45:07.000000 simframe-1.0.3rc1/examples/example_coupled_oscillators.ipynb
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)  1280874 2022-03-29 12:45:07.000000 simframe-1.0.3rc1/examples/example_double_pendulum.ipynb
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)       38 2023-05-24 13:40:48.830551 simframe-1.0.3rc1/setup.cfg
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2056 2023-05-24 13:30:47.000000 simframe-1.0.3rc1/setup.py
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-24 13:40:46.863098 simframe-1.0.3rc1/simframe/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      359 2023-05-24 13:39:34.000000 simframe-1.0.3rc1/simframe/__init__.py
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-24 13:40:47.266282 simframe-1.0.3rc1/simframe/frame/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      529 2021-12-24 09:33:56.000000 simframe-1.0.3rc1/simframe/frame/__init__.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2074 2021-12-24 09:33:56.000000 simframe-1.0.3rc1/simframe/frame/abstractgroup.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)    10152 2023-05-12 14:36:17.000000 simframe-1.0.3rc1/simframe/frame/field.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     6707 2023-05-24 13:30:47.000000 simframe-1.0.3rc1/simframe/frame/frame.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)    13139 2023-05-12 14:54:08.000000 simframe-1.0.3rc1/simframe/frame/group.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     3897 2021-12-24 09:33:56.000000 simframe-1.0.3rc1/simframe/frame/heartbeat.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     5516 2021-12-24 09:33:56.000000 simframe-1.0.3rc1/simframe/frame/intvar.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      964 2021-12-24 09:33:56.000000 simframe-1.0.3rc1/simframe/frame/updater.py
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-24 13:40:47.426940 simframe-1.0.3rc1/simframe/integration/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      715 2021-12-24 09:33:56.000000 simframe-1.0.3rc1/simframe/integration/__init__.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2314 2021-12-24 09:33:56.000000 simframe-1.0.3rc1/simframe/integration/instruction.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     7722 2021-12-24 09:33:56.000000 simframe-1.0.3rc1/simframe/integration/integrator.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     3301 2021-12-24 09:33:56.000000 simframe-1.0.3rc1/simframe/integration/scheme.py
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-24 13:40:48.340939 simframe-1.0.3rc1/simframe/integration/schemes/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2659 2021-12-24 09:33:56.000000 simframe-1.0.3rc1/simframe/integration/schemes/__init__.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1087 2021-12-24 09:33:56.000000 simframe-1.0.3rc1/simframe/integration/schemes/expl_1_euler.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2631 2021-12-24 09:33:56.000000 simframe-1.0.3rc1/simframe/integration/schemes/expl_2_fehlberg_adptv.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1232 2021-12-24 09:33:56.000000 simframe-1.0.3rc1/simframe/integration/schemes/expl_2_heun.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2374 2021-12-24 09:33:56.000000 simframe-1.0.3rc1/simframe/integration/schemes/expl_2_heun_euler_adptv.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1218 2021-12-24 09:33:56.000000 simframe-1.0.3rc1/simframe/integration/schemes/expl_2_midpoint.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1250 2021-12-24 09:33:56.000000 simframe-1.0.3rc1/simframe/integration/schemes/expl_2_ralston.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2814 2021-12-24 09:33:56.000000 simframe-1.0.3rc1/simframe/integration/schemes/expl_3_bogacki_shampine_adptv.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2736 2021-12-24 09:33:56.000000 simframe-1.0.3rc1/simframe/integration/schemes/expl_3_gottlieb_shu_adptv.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1340 2021-12-24 09:33:56.000000 simframe-1.0.3rc1/simframe/integration/schemes/expl_3_heun.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1360 2021-12-24 09:33:56.000000 simframe-1.0.3rc1/simframe/integration/schemes/expl_3_kutta.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1375 2021-12-24 09:33:56.000000 simframe-1.0.3rc1/simframe/integration/schemes/expl_3_ralston.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1456 2021-12-24 09:33:56.000000 simframe-1.0.3rc1/simframe/integration/schemes/expl_3_ssprk.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1499 2021-12-24 09:33:56.000000 simframe-1.0.3rc1/simframe/integration/schemes/expl_4_38rule.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1818 2021-12-24 09:33:56.000000 simframe-1.0.3rc1/simframe/integration/schemes/expl_4_ralston.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1531 2021-12-24 09:33:56.000000 simframe-1.0.3rc1/simframe/integration/schemes/expl_4_runge_kutta.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     3718 2021-12-24 09:33:56.000000 simframe-1.0.3rc1/simframe/integration/schemes/expl_5_cash_karp_adptv.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     4164 2021-12-24 09:33:56.000000 simframe-1.0.3rc1/simframe/integration/schemes/expl_5_dormand_prince_adptv.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1362 2021-12-24 09:33:56.000000 simframe-1.0.3rc1/simframe/integration/schemes/impl_1_euler_direct.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1614 2021-12-24 09:33:56.000000 simframe-1.0.3rc1/simframe/integration/schemes/impl_1_euler_gmres.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1422 2021-12-24 09:33:56.000000 simframe-1.0.3rc1/simframe/integration/schemes/impl_2_midpoint_direct.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      764 2021-12-24 09:33:56.000000 simframe-1.0.3rc1/simframe/integration/schemes/update.py
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-24 13:40:48.541431 simframe-1.0.3rc1/simframe/io/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      710 2021-12-24 09:33:56.000000 simframe-1.0.3rc1/simframe/io/__init__.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      788 2023-05-24 13:30:47.000000 simframe-1.0.3rc1/simframe/io/dump.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     7507 2021-12-24 09:33:56.000000 simframe-1.0.3rc1/simframe/io/progress.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     4634 2021-12-24 09:33:56.000000 simframe-1.0.3rc1/simframe/io/reader.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     9406 2023-05-12 14:36:17.000000 simframe-1.0.3rc1/simframe/io/writer.py
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-24 13:40:48.673592 simframe-1.0.3rc1/simframe/io/writers/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      507 2021-12-24 09:33:56.000000 simframe-1.0.3rc1/simframe/io/writers/__init__.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     6983 2021-12-24 09:33:56.000000 simframe-1.0.3rc1/simframe/io/writers/hdf5writer.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     6050 2021-12-24 09:33:56.000000 simframe-1.0.3rc1/simframe/io/writers/namespacewriter.py
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-24 13:40:48.796692 simframe-1.0.3rc1/simframe/utils/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      451 2022-03-29 12:45:08.000000 simframe-1.0.3rc1/simframe/utils/__init__.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1770 2021-12-24 09:33:56.000000 simframe-1.0.3rc1/simframe/utils/color.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1249 2022-03-29 12:45:08.000000 simframe-1.0.3rc1/simframe/utils/format.py
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-24 13:40:46.960156 simframe-1.0.3rc1/simframe.egg-info/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     4697 2023-05-24 13:40:45.000000 simframe-1.0.3rc1/simframe.egg-info/PKG-INFO
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2484 2023-05-24 13:40:45.000000 simframe-1.0.3rc1/simframe.egg-info/SOURCES.txt
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)        1 2023-05-24 13:40:45.000000 simframe-1.0.3rc1/simframe.egg-info/dependency_links.txt
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)        1 2022-03-29 17:44:06.000000 simframe-1.0.3rc1/simframe.egg-info/not-zip-safe
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)       28 2023-05-24 13:40:45.000000 simframe-1.0.3rc1/simframe.egg-info/requires.txt
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)       15 2023-05-24 13:40:45.000000 simframe-1.0.3rc1/simframe.egg-info/top_level.txt
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-07-21 11:26:38.527776 simframe-1.0.4rc0/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1532 2022-03-10 11:03:13.000000 simframe-1.0.4rc0/LICENSE
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      198 2022-03-10 11:03:13.000000 simframe-1.0.4rc0/MANIFEST.in
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     4697 2023-07-21 11:26:38.524771 simframe-1.0.4rc0/PKG-INFO
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     3524 2023-05-12 14:36:17.000000 simframe-1.0.4rc0/README.md
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-07-21 11:26:36.282522 simframe-1.0.4rc0/docs/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      638 2021-12-24 09:33:56.000000 simframe-1.0.4rc0/docs/Makefile
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      799 2021-12-24 09:33:56.000000 simframe-1.0.4rc0/docs/make.bat
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      129 2023-07-21 11:25:41.000000 simframe-1.0.4rc0/docs/requirements.txt
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-07-21 11:26:36.368763 simframe-1.0.4rc0/docs/source/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      421 2021-12-24 09:33:56.000000 simframe-1.0.4rc0/docs/source/api.rst
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1828 2022-03-10 11:03:13.000000 simframe-1.0.4rc0/docs/source/conf.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1032 2022-03-10 11:03:13.000000 simframe-1.0.4rc0/docs/source/index.rst
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-07-21 11:26:36.941433 simframe-1.0.4rc0/examples/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)    63171 2023-05-24 13:30:47.000000 simframe-1.0.4rc0/examples/1_simple_integration.ipynb
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)    49497 2023-05-24 13:30:47.000000 simframe-1.0.4rc0/examples/2_advanced_integration.ipynb
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)   125218 2023-05-24 13:30:47.000000 simframe-1.0.4rc0/examples/3_updating.ipynb
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)    13834 2022-03-29 12:45:07.000000 simframe-1.0.4rc0/examples/4_custom_schemes.ipynb
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)   381957 2022-03-29 12:45:07.000000 simframe-1.0.4rc0/examples/5_adaptive_schemes.ipynb
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)    68256 2022-03-29 12:45:07.000000 simframe-1.0.4rc0/examples/6_implicit_integration.ipynb
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1380 2022-03-29 12:45:07.000000 simframe-1.0.4rc0/examples/A_citation.ipynb
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2648 2022-03-29 12:45:07.000000 simframe-1.0.4rc0/examples/B_contrib_bug_feature.ipynb
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)   391549 2022-03-29 12:45:07.000000 simframe-1.0.4rc0/examples/example_compartmental_models.ipynb
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)  4006805 2022-03-29 12:45:07.000000 simframe-1.0.4rc0/examples/example_coupled_oscillators.ipynb
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)  1280874 2022-03-29 12:45:07.000000 simframe-1.0.4rc0/examples/example_double_pendulum.ipynb
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)       38 2023-07-21 11:26:38.528772 simframe-1.0.4rc0/setup.cfg
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2064 2023-07-21 11:25:41.000000 simframe-1.0.4rc0/setup.py
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-07-21 11:26:36.985381 simframe-1.0.4rc0/simframe/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      359 2023-07-21 11:26:14.000000 simframe-1.0.4rc0/simframe/__init__.py
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-07-21 11:26:37.315410 simframe-1.0.4rc0/simframe/frame/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      529 2021-12-24 09:33:56.000000 simframe-1.0.4rc0/simframe/frame/__init__.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2074 2021-12-24 09:33:56.000000 simframe-1.0.4rc0/simframe/frame/abstractgroup.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)    10152 2023-05-12 14:36:17.000000 simframe-1.0.4rc0/simframe/frame/field.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     6707 2023-05-24 13:30:47.000000 simframe-1.0.4rc0/simframe/frame/frame.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)    13471 2023-07-21 11:25:41.000000 simframe-1.0.4rc0/simframe/frame/group.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     4855 2023-07-21 11:25:41.000000 simframe-1.0.4rc0/simframe/frame/heartbeat.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     5516 2021-12-24 09:33:56.000000 simframe-1.0.4rc0/simframe/frame/intvar.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2044 2023-07-21 11:25:41.000000 simframe-1.0.4rc0/simframe/frame/updater.py
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-07-21 11:26:37.420046 simframe-1.0.4rc0/simframe/integration/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      715 2021-12-24 09:33:56.000000 simframe-1.0.4rc0/simframe/integration/__init__.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2314 2021-12-24 09:33:56.000000 simframe-1.0.4rc0/simframe/integration/instruction.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     7733 2023-07-21 11:25:41.000000 simframe-1.0.4rc0/simframe/integration/integrator.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     3301 2021-12-24 09:33:56.000000 simframe-1.0.4rc0/simframe/integration/scheme.py
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-07-21 11:26:38.177804 simframe-1.0.4rc0/simframe/integration/schemes/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2659 2021-12-24 09:33:56.000000 simframe-1.0.4rc0/simframe/integration/schemes/__init__.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1087 2021-12-24 09:33:56.000000 simframe-1.0.4rc0/simframe/integration/schemes/expl_1_euler.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2631 2021-12-24 09:33:56.000000 simframe-1.0.4rc0/simframe/integration/schemes/expl_2_fehlberg_adptv.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1232 2021-12-24 09:33:56.000000 simframe-1.0.4rc0/simframe/integration/schemes/expl_2_heun.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2374 2021-12-24 09:33:56.000000 simframe-1.0.4rc0/simframe/integration/schemes/expl_2_heun_euler_adptv.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1218 2021-12-24 09:33:56.000000 simframe-1.0.4rc0/simframe/integration/schemes/expl_2_midpoint.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1250 2021-12-24 09:33:56.000000 simframe-1.0.4rc0/simframe/integration/schemes/expl_2_ralston.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2814 2021-12-24 09:33:56.000000 simframe-1.0.4rc0/simframe/integration/schemes/expl_3_bogacki_shampine_adptv.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2736 2021-12-24 09:33:56.000000 simframe-1.0.4rc0/simframe/integration/schemes/expl_3_gottlieb_shu_adptv.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1340 2021-12-24 09:33:56.000000 simframe-1.0.4rc0/simframe/integration/schemes/expl_3_heun.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1360 2021-12-24 09:33:56.000000 simframe-1.0.4rc0/simframe/integration/schemes/expl_3_kutta.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1375 2021-12-24 09:33:56.000000 simframe-1.0.4rc0/simframe/integration/schemes/expl_3_ralston.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1456 2021-12-24 09:33:56.000000 simframe-1.0.4rc0/simframe/integration/schemes/expl_3_ssprk.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1499 2021-12-24 09:33:56.000000 simframe-1.0.4rc0/simframe/integration/schemes/expl_4_38rule.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1818 2021-12-24 09:33:56.000000 simframe-1.0.4rc0/simframe/integration/schemes/expl_4_ralston.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1531 2021-12-24 09:33:56.000000 simframe-1.0.4rc0/simframe/integration/schemes/expl_4_runge_kutta.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     3718 2021-12-24 09:33:56.000000 simframe-1.0.4rc0/simframe/integration/schemes/expl_5_cash_karp_adptv.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     4164 2021-12-24 09:33:56.000000 simframe-1.0.4rc0/simframe/integration/schemes/expl_5_dormand_prince_adptv.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1362 2021-12-24 09:33:56.000000 simframe-1.0.4rc0/simframe/integration/schemes/impl_1_euler_direct.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1614 2021-12-24 09:33:56.000000 simframe-1.0.4rc0/simframe/integration/schemes/impl_1_euler_gmres.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1422 2021-12-24 09:33:56.000000 simframe-1.0.4rc0/simframe/integration/schemes/impl_2_midpoint_direct.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      764 2021-12-24 09:33:56.000000 simframe-1.0.4rc0/simframe/integration/schemes/update.py
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-07-21 11:26:38.308807 simframe-1.0.4rc0/simframe/io/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      710 2021-12-24 09:33:56.000000 simframe-1.0.4rc0/simframe/io/__init__.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      782 2023-07-21 11:25:41.000000 simframe-1.0.4rc0/simframe/io/dump.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     7507 2021-12-24 09:33:56.000000 simframe-1.0.4rc0/simframe/io/progress.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     4634 2021-12-24 09:33:56.000000 simframe-1.0.4rc0/simframe/io/reader.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     9406 2023-05-12 14:36:17.000000 simframe-1.0.4rc0/simframe/io/writer.py
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-07-21 11:26:38.417780 simframe-1.0.4rc0/simframe/io/writers/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      507 2021-12-24 09:33:56.000000 simframe-1.0.4rc0/simframe/io/writers/__init__.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     6996 2023-07-21 11:25:41.000000 simframe-1.0.4rc0/simframe/io/writers/hdf5writer.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     6050 2021-12-24 09:33:56.000000 simframe-1.0.4rc0/simframe/io/writers/namespacewriter.py
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-07-21 11:26:38.506812 simframe-1.0.4rc0/simframe/utils/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      451 2022-03-29 12:45:08.000000 simframe-1.0.4rc0/simframe/utils/__init__.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1770 2021-12-24 09:33:56.000000 simframe-1.0.4rc0/simframe/utils/color.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1249 2022-03-29 12:45:08.000000 simframe-1.0.4rc0/simframe/utils/format.py
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-07-21 11:26:37.084375 simframe-1.0.4rc0/simframe.egg-info/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     4697 2023-07-21 11:26:35.000000 simframe-1.0.4rc0/simframe.egg-info/PKG-INFO
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2484 2023-07-21 11:26:35.000000 simframe-1.0.4rc0/simframe.egg-info/SOURCES.txt
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)        1 2023-07-21 11:26:35.000000 simframe-1.0.4rc0/simframe.egg-info/dependency_links.txt
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)        1 2022-03-29 17:44:06.000000 simframe-1.0.4rc0/simframe.egg-info/not-zip-safe
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)       33 2023-07-21 11:26:35.000000 simframe-1.0.4rc0/simframe.egg-info/requires.txt
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)       15 2023-07-21 11:26:35.000000 simframe-1.0.4rc0/simframe.egg-info/top_level.txt
```

### Comparing `simframe-1.0.3rc1/LICENSE` & `simframe-1.0.4rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `simframe-1.0.3rc1/PKG-INFO` & `simframe-1.0.4rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simframe
-Version: 1.0.3rc1
+Version: 1.0.4rc0
 Summary: Framework for Scientific Simulations
 Home-page: https://github.com/stammler/simframe
 Author: Sebastian Stammler, Tilman Birnstiel
 Author-email: sebastian.stammler@gmail.com, til.birnstiel@lmu.de
 Maintainer: Sebastian Stammler
 License: BSD
 Project-URL: Source Code, https://github.com/stammler/simframe/
```

### Comparing `simframe-1.0.3rc1/README.md` & `simframe-1.0.4rc0/README.md`

 * *Files identical despite different names*

### Comparing `simframe-1.0.3rc1/docs/Makefile` & `simframe-1.0.4rc0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `simframe-1.0.3rc1/docs/make.bat` & `simframe-1.0.4rc0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `simframe-1.0.3rc1/docs/source/conf.py` & `simframe-1.0.4rc0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.3rc1/docs/source/index.rst` & `simframe-1.0.4rc0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `simframe-1.0.3rc1/examples/1_simple_integration.ipynb` & `simframe-1.0.4rc0/examples/1_simple_integration.ipynb`

 * *Files identical despite different names*

### Comparing `simframe-1.0.3rc1/examples/2_advanced_integration.ipynb` & `simframe-1.0.4rc0/examples/2_advanced_integration.ipynb`

 * *Files identical despite different names*

### Comparing `simframe-1.0.3rc1/examples/3_updating.ipynb` & `simframe-1.0.4rc0/examples/3_updating.ipynb`

 * *Files identical despite different names*

### Comparing `simframe-1.0.3rc1/examples/4_custom_schemes.ipynb` & `simframe-1.0.4rc0/examples/4_custom_schemes.ipynb`

 * *Files identical despite different names*

### Comparing `simframe-1.0.3rc1/examples/5_adaptive_schemes.ipynb` & `simframe-1.0.4rc0/examples/5_adaptive_schemes.ipynb`

 * *Files identical despite different names*

### Comparing `simframe-1.0.3rc1/examples/6_implicit_integration.ipynb` & `simframe-1.0.4rc0/examples/6_implicit_integration.ipynb`

 * *Files identical despite different names*

### Comparing `simframe-1.0.3rc1/examples/A_citation.ipynb` & `simframe-1.0.4rc0/examples/A_citation.ipynb`

 * *Files identical despite different names*

### Comparing `simframe-1.0.3rc1/examples/B_contrib_bug_feature.ipynb` & `simframe-1.0.4rc0/examples/B_contrib_bug_feature.ipynb`

 * *Files identical despite different names*

### Comparing `simframe-1.0.3rc1/examples/example_compartmental_models.ipynb` & `simframe-1.0.4rc0/examples/example_compartmental_models.ipynb`

 * *Files identical despite different names*

### Comparing `simframe-1.0.3rc1/examples/example_coupled_oscillators.ipynb` & `simframe-1.0.4rc0/examples/example_coupled_oscillators.ipynb`

 * *Files identical despite different names*

### Comparing `simframe-1.0.3rc1/examples/example_double_pendulum.ipynb` & `simframe-1.0.4rc0/examples/example_double_pendulum.ipynb`

 * *Files identical despite different names*

### Comparing `simframe-1.0.3rc1/setup.py` & `simframe-1.0.4rc0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,11 +48,11 @@
                  "Topic :: Education",
                  "Topic :: Scientific/Engineering",
                  "Topic :: Scientific/Engineering :: Mathematics",
                  "Topic :: Scientific/Engineering :: Physics",
                  ],
 
     packages=find_packages(),
-    install_requires=["h5py", "matplotlib", "numpy", "scipy"],
+    install_requires=["dill", "h5py", "matplotlib", "numpy", "scipy"],
     include_package_data=True,
     zip_safe=False,
 )
```

### Comparing `simframe-1.0.3rc1/simframe/frame/__init__.py` & `simframe-1.0.4rc0/simframe/frame/__init__.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.3rc1/simframe/frame/abstractgroup.py` & `simframe-1.0.4rc0/simframe/frame/abstractgroup.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.3rc1/simframe/frame/field.py` & `simframe-1.0.4rc0/simframe/frame/field.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.3rc1/simframe/frame/frame.py` & `simframe-1.0.4rc0/simframe/frame/frame.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.3rc1/simframe/frame/group.py` & `simframe-1.0.4rc0/simframe/frame/group.py`

 * *Files 2% similar despite different names*

```diff
@@ -252,15 +252,25 @@
         ls : list
             list of group attributes that should be updated in that order
 
         Returns
         -------
         func : callable
             Function that is reduced by <self> and <ls>."""
-        return partial(_dummyupdatewithlist, self, ls)
+
+        # To give meaningful information a new class of partial is created
+        # with a new __repr__ method
+        class list_updater(partial):
+
+            def __repr__(self):
+                return type(self).__name__
+
+        f = list_updater(_dummyupdatewithlist, self, ls)
+        f.__doc__ = f"The attributes in this group are updated in the order: \n{ls}."
+        return f
 
     def _toc(self):
         ret = _toc_tree(self)
         print(ret)
 
     def memory_usage(self, print_output=False, skip_hidden=False):
         """Determine memory usage of a Group
```

### Comparing `simframe-1.0.3rc1/simframe/frame/heartbeat.py` & `simframe-1.0.4rc0/simframe/frame/heartbeat.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from simframe.frame.updater import Updater
+from simframe.utils.color import colorize
 
 
 class Heartbeat(object):
     """This class controls an update including ``systole`` and ``diastole``.
 
     A full cardiac cycle constists of a systole operation, the actual update and a systole operation.
     All three are of type ``Updater``.
@@ -31,15 +32,36 @@
         self.systole = systole
         self.diastole = diastole
 
     def __str__(self):
         return "{}".format(str(self.__name__))
 
     def __repr__(self):
-        return self.__str__()
+        s = self.__str__() + "\n"
+        s += (len(s)-1)*"-" + "\n"
+        s += "\n"
+        s += "{} {}".format(colorize("Systole: ", color="red"),
+                            str(self.systole._func)) + "\n"
+        s += "{} {}".format(colorize("Updater: ", color="red"),
+                            str(self.updater._func)) + "\n"
+        s += "{} {}".format(colorize("Diastole:", color="red"),
+                            str(self.diastole._func)) + "\n"
+        s += "\n"
+        s += "Docstrings" + "\n"
+        s += 10*"-" + "\n"
+        s += "\n"
+        s += colorize("Systole:", color="red") + "\n"
+        s += str(self.systole._func.__doc__ or None) + "\n"
+        s += "\n"
+        s += colorize("Updater:", color="red") + "\n"
+        s += str(self.updater._func.__doc__ or None) + "\n"
+        s += "\n"
+        s += colorize("Diastole:", color="red") + "\n"
+        s += str(self.diastole._func.__doc__ or None)
+        return s
 
     @property
     def systole(self):
         '''``Updater`` that is called in the beginning of cardiac cycle.'''
         return self._systole
 
     @systole.setter
```

### Comparing `simframe-1.0.3rc1/simframe/frame/intvar.py` & `simframe-1.0.4rc0/simframe/frame/intvar.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.3rc1/simframe/integration/__init__.py` & `simframe-1.0.4rc0/simframe/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.3rc1/simframe/integration/instruction.py` & `simframe-1.0.4rc0/simframe/integration/instruction.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.3rc1/simframe/integration/integrator.py` & `simframe-1.0.4rc0/simframe/integration/integrator.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,15 @@
         """Method that executes one integration step."""
         # Preparation
         self._prepare()
         # Loop over all instructions. Exit the loop only if all instructions were executed successfully
         # And count the loops
         i = 0
         status = False
-        while(not status):
+        while (not status):
             # The suggested stepsize has to be reset in the beginning of every try.
             # We therefore have to copy the current stepsize in case the user is returning
             # the suggested stepsize in the stepsize function.
             stepsize = self.var.stepsize.copy()
             self.var._suggested = None
             if i >= self.maxit:
                 raise StopIteration(
@@ -165,15 +165,15 @@
         # Update the variables.
         upd = update()
         for i, inst in enumerate(self.instructions):
             if inst.Y._buffer is None:
                 continue
             upd(None, inst.Y, None)
         # Store the taken stepsize
-        self.var._prevstepsize = stepsize
+        self.var._prevstepsize = np.array(stepsize)
         # Finalization
         self._finalize()
 
     def _failoperation(self, *args, **kwargs):
         """This operation will be executed if any integration ``Instruction`` failed and before the
         ``Integrator`` tries it again. It will execute the ``Heartbeat`` of ``Integrator.failop``.
```

### Comparing `simframe-1.0.3rc1/simframe/integration/scheme.py` & `simframe-1.0.4rc0/simframe/integration/scheme.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.3rc1/simframe/integration/schemes/__init__.py` & `simframe-1.0.4rc0/simframe/integration/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.3rc1/simframe/integration/schemes/expl_1_euler.py` & `simframe-1.0.4rc0/simframe/integration/schemes/expl_1_euler.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.3rc1/simframe/integration/schemes/expl_2_fehlberg_adptv.py` & `simframe-1.0.4rc0/simframe/integration/schemes/expl_2_fehlberg_adptv.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.3rc1/simframe/integration/schemes/expl_2_heun.py` & `simframe-1.0.4rc0/simframe/integration/schemes/expl_2_heun.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.3rc1/simframe/integration/schemes/expl_2_heun_euler_adptv.py` & `simframe-1.0.4rc0/simframe/integration/schemes/expl_2_heun_euler_adptv.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.3rc1/simframe/integration/schemes/expl_2_midpoint.py` & `simframe-1.0.4rc0/simframe/integration/schemes/expl_2_midpoint.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.3rc1/simframe/integration/schemes/expl_2_ralston.py` & `simframe-1.0.4rc0/simframe/integration/schemes/expl_2_ralston.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.3rc1/simframe/integration/schemes/expl_3_bogacki_shampine_adptv.py` & `simframe-1.0.4rc0/simframe/integration/schemes/expl_3_bogacki_shampine_adptv.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.3rc1/simframe/integration/schemes/expl_3_gottlieb_shu_adptv.py` & `simframe-1.0.4rc0/simframe/integration/schemes/expl_3_gottlieb_shu_adptv.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.3rc1/simframe/integration/schemes/expl_3_heun.py` & `simframe-1.0.4rc0/simframe/integration/schemes/expl_3_heun.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.3rc1/simframe/integration/schemes/expl_3_kutta.py` & `simframe-1.0.4rc0/simframe/integration/schemes/expl_3_kutta.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.3rc1/simframe/integration/schemes/expl_3_ralston.py` & `simframe-1.0.4rc0/simframe/integration/schemes/expl_3_ralston.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.3rc1/simframe/integration/schemes/expl_3_ssprk.py` & `simframe-1.0.4rc0/simframe/integration/schemes/expl_3_ssprk.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.3rc1/simframe/integration/schemes/expl_4_38rule.py` & `simframe-1.0.4rc0/simframe/integration/schemes/expl_4_38rule.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.3rc1/simframe/integration/schemes/expl_4_ralston.py` & `simframe-1.0.4rc0/simframe/integration/schemes/expl_4_ralston.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.3rc1/simframe/integration/schemes/expl_4_runge_kutta.py` & `simframe-1.0.4rc0/simframe/integration/schemes/expl_4_runge_kutta.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.3rc1/simframe/integration/schemes/expl_5_cash_karp_adptv.py` & `simframe-1.0.4rc0/simframe/integration/schemes/expl_5_cash_karp_adptv.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.3rc1/simframe/integration/schemes/expl_5_dormand_prince_adptv.py` & `simframe-1.0.4rc0/simframe/integration/schemes/expl_5_dormand_prince_adptv.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.3rc1/simframe/integration/schemes/impl_1_euler_direct.py` & `simframe-1.0.4rc0/simframe/integration/schemes/impl_1_euler_direct.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.3rc1/simframe/integration/schemes/impl_1_euler_gmres.py` & `simframe-1.0.4rc0/simframe/integration/schemes/impl_1_euler_gmres.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.3rc1/simframe/integration/schemes/impl_2_midpoint_direct.py` & `simframe-1.0.4rc0/simframe/integration/schemes/impl_2_midpoint_direct.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.3rc1/simframe/integration/schemes/update.py` & `simframe-1.0.4rc0/simframe/integration/schemes/update.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.3rc1/simframe/io/__init__.py` & `simframe-1.0.4rc0/simframe/io/__init__.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.3rc1/simframe/io/dump.py` & `simframe-1.0.4rc0/simframe/io/dump.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-import pickle
+import dill
 
 
 def writedump(object, filename="object.dmp"):
     """Writes object to dump file
 
     Parameters
     ----------
     object : object
         object to be written to file
     filename : str, optional, default : "object.dmp"
         path to file to be written"""
     with open(filename, "wb") as dumpfile:
-        pickle.dump(object, dumpfile)
+        dill.dump(object, dumpfile)
 
 
 def readdump(filename):
     """Reads dumpfile and returns ``Frame`` object
 
     Parameters
     ----------
@@ -28,9 +28,9 @@
         object read from dump file
 
     Notes
     -----
     Only read dump files from sources you trust.
     Malware can be injected."""
     with open(filename, "rb") as dumpfile:
-        obj = pickle.load(dumpfile)
+        obj = dill.load(dumpfile)
     return obj
```

### Comparing `simframe-1.0.3rc1/simframe/io/progress.py` & `simframe-1.0.4rc0/simframe/io/progress.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.3rc1/simframe/io/reader.py` & `simframe-1.0.4rc0/simframe/io/reader.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.3rc1/simframe/io/writer.py` & `simframe-1.0.4rc0/simframe/io/writer.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.3rc1/simframe/io/writers/hdf5writer.py` & `simframe-1.0.4rc0/simframe/io/writers/hdf5writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,34 +152,34 @@
 
         Parameters
         ----------
         writer : Writer
             Writer object to which the reaer belongs."""
         super().__init__(writer)
 
-    def output(self, filename):
+    def output(self, output):
         """Reads a single output file.
 
         Parameters
         ----------
-        filename : str
-            Path to filename to be read
+        output : str or int
+            Path to filename to be read or number of output
 
         Returns
         -------
         data : SimpleNamespace
             Namespace of data in file."""
 
-        if not isinstance(filename, str):
-            filename = self._writer._getfilename(filename)
+        if not isinstance(output, str):
+            output = self._writer._getfilename(output)
 
-        if not os.path.isfile(filename):
+        if not os.path.isfile(output):
             raise RuntimeError("File does not exist.")
 
-        with h5py.File(filename, "r") as hdf5file:
+        with h5py.File(output, "r") as hdf5file:
             return self._readgroup(hdf5file)
 
     def sequence(self, field):
         """Reading the entire sequence of a specific field.
 
         Parameters
         ----------
```

### Comparing `simframe-1.0.3rc1/simframe/io/writers/namespacewriter.py` & `simframe-1.0.4rc0/simframe/io/writers/namespacewriter.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.3rc1/simframe/utils/color.py` & `simframe-1.0.4rc0/simframe/utils/color.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.3rc1/simframe/utils/format.py` & `simframe-1.0.4rc0/simframe/utils/format.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.3rc1/simframe.egg-info/PKG-INFO` & `simframe-1.0.4rc0/simframe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simframe
-Version: 1.0.3rc1
+Version: 1.0.4rc0
 Summary: Framework for Scientific Simulations
 Home-page: https://github.com/stammler/simframe
 Author: Sebastian Stammler, Tilman Birnstiel
 Author-email: sebastian.stammler@gmail.com, til.birnstiel@lmu.de
 Maintainer: Sebastian Stammler
 License: BSD
 Project-URL: Source Code, https://github.com/stammler/simframe/
```

### Comparing `simframe-1.0.3rc1/simframe.egg-info/SOURCES.txt` & `simframe-1.0.4rc0/simframe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

