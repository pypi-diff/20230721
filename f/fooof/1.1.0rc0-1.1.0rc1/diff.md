# Comparing `tmp/fooof-1.1.0rc0.tar.gz` & `tmp/fooof-1.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fooof-1.1.0rc0.tar", last modified: Fri Jun 30 19:07:34 2023, max compression
+gzip compressed data, was "/Users/tom/Code/ModCode/fooof/dist/.tmp-cwsuvxtn/fooof-1.1.0rc1.tar", last modified: Fri Jul 21 19:21:34 2023, max compression
```

## Comparing `fooof-1.1.0rc0.tar` & `fooof-1.1.0rc1.tar`

### file list

```diff
@@ -1,126 +1,127 @@
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-30 19:07:34.426153 fooof-1.1.0rc0/
--rw-r--r--   0 tom        (501) staff       (20)    11340 2019-01-23 01:14:03.000000 fooof-1.1.0rc0/LICENSE
--rw-r--r--   0 tom        (501) staff       (20)       16 2019-01-23 01:14:03.000000 fooof-1.1.0rc0/MANIFEST.in
--rw-r--r--   0 tom        (501) staff       (20)    13337 2023-06-30 19:07:34.425744 fooof-1.1.0rc0/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)    11796 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/README.rst
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-30 19:07:34.390298 fooof-1.1.0rc0/fooof/
--rw-r--r--   0 tom        (501) staff       (20)      825 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/__init__.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-30 19:07:34.394756 fooof-1.1.0rc0/fooof/analysis/
--rw-r--r--   0 tom        (501) staff       (20)      169 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/analysis/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     3837 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/analysis/error.py
--rw-r--r--   0 tom        (501) staff       (20)     9350 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/analysis/periodic.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-30 19:07:34.395706 fooof-1.1.0rc0/fooof/bands/
--rw-r--r--   0 tom        (501) staff       (20)       60 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/bands/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     4091 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/bands/bands.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-30 19:07:34.399831 fooof-1.1.0rc0/fooof/core/
--rw-r--r--   0 tom        (501) staff       (20)       47 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/core/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      616 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/core/errors.py
--rw-r--r--   0 tom        (501) staff       (20)     5271 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/core/funcs.py
--rw-r--r--   0 tom        (501) staff       (20)     3860 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/core/info.py
--rw-r--r--   0 tom        (501) staff       (20)     8186 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/core/io.py
--rw-r--r--   0 tom        (501) staff       (20)      411 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/core/items.py
--rw-r--r--   0 tom        (501) staff       (20)     4703 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/core/modutils.py
--rw-r--r--   0 tom        (501) staff       (20)     4766 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/core/reports.py
--rw-r--r--   0 tom        (501) staff       (20)    14913 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/core/strings.py
--rw-r--r--   0 tom        (501) staff       (20)     6880 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/core/utils.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-30 19:07:34.401025 fooof-1.1.0rc0/fooof/data/
--rw-r--r--   0 tom        (501) staff       (20)      106 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/data/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     3216 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/data/conversions.py
--rw-r--r--   0 tom        (501) staff       (20)     3784 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/data/data.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-30 19:07:34.402455 fooof-1.1.0rc0/fooof/objs/
--rw-r--r--   0 tom        (501) staff       (20)      217 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/objs/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)    53885 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/objs/fit.py
--rw-r--r--   0 tom        (501) staff       (20)    25446 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/objs/group.py
--rw-r--r--   0 tom        (501) staff       (20)     8153 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/objs/utils.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-30 19:07:34.406123 fooof-1.1.0rc0/fooof/plts/
--rw-r--r--   0 tom        (501) staff       (20)      120 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/plts/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)    10159 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/plts/annotate.py
--rw-r--r--   0 tom        (501) staff       (20)     4754 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/plts/aperiodic.py
--rw-r--r--   0 tom        (501) staff       (20)     1912 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/plts/error.py
--rw-r--r--   0 tom        (501) staff       (20)     4046 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/plts/fg.py
--rw-r--r--   0 tom        (501) staff       (20)    11410 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/plts/fm.py
--rw-r--r--   0 tom        (501) staff       (20)     5105 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/plts/periodic.py
--rw-r--r--   0 tom        (501) staff       (20)     2027 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/plts/settings.py
--rw-r--r--   0 tom        (501) staff       (20)     7604 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/plts/spectra.py
--rw-r--r--   0 tom        (501) staff       (20)     8892 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/plts/style.py
--rw-r--r--   0 tom        (501) staff       (20)     3747 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/plts/templates.py
--rw-r--r--   0 tom        (501) staff       (20)     6682 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/plts/utils.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-30 19:07:34.408186 fooof-1.1.0rc0/fooof/sim/
--rw-r--r--   0 tom        (501) staff       (20)      220 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/sim/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)    17522 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/sim/gen.py
--rw-r--r--   0 tom        (501) staff       (20)     9749 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/sim/params.py
--rw-r--r--   0 tom        (501) staff       (20)     9002 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/sim/transform.py
--rw-r--r--   0 tom        (501) staff       (20)      468 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/sim/utils.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-30 19:07:34.409456 fooof-1.1.0rc0/fooof/tests/
--rw-r--r--   0 tom        (501) staff       (20)       23 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/__init__.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-30 19:07:34.410611 fooof-1.1.0rc0/fooof/tests/analysis/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/analysis/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     1065 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/analysis/test_error.py
--rw-r--r--   0 tom        (501) staff       (20)     2771 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/analysis/test_periodic.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-30 19:07:34.411303 fooof-1.1.0rc0/fooof/tests/bands/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/bands/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     1176 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/bands/test_bands.py
--rw-r--r--   0 tom        (501) staff       (20)     1748 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/conftest.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-30 19:07:34.413500 fooof-1.1.0rc0/fooof/tests/core/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/core/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     2960 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/core/test_funcs.py
--rw-r--r--   0 tom        (501) staff       (20)     1485 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/core/test_info.py
--rw-r--r--   0 tom        (501) staff       (20)     5874 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/core/test_io.py
--rw-r--r--   0 tom        (501) staff       (20)     1605 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/core/test_modutils.py
--rw-r--r--   0 tom        (501) staff       (20)      766 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/core/test_reports.py
--rw-r--r--   0 tom        (501) staff       (20)     1355 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/core/test_strings.py
--rw-r--r--   0 tom        (501) staff       (20)     4127 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/core/test_utils.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-30 19:07:34.414286 fooof-1.1.0rc0/fooof/tests/data/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/data/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     1657 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/data/test_conversions.py
--rw-r--r--   0 tom        (501) staff       (20)     1284 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/data/test_data.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-30 19:07:34.415642 fooof-1.1.0rc0/fooof/tests/objs/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/objs/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)    14153 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/objs/test_fit.py
--rw-r--r--   0 tom        (501) staff       (20)    11469 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/objs/test_group.py
--rw-r--r--   0 tom        (501) staff       (20)     4261 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/objs/test_utils.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-30 19:07:34.419169 fooof-1.1.0rc0/fooof/tests/plts/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/plts/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      895 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/plts/test_annotate.py
--rw-r--r--   0 tom        (501) staff       (20)     1461 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/plts/test_aperiodic.py
--rw-r--r--   0 tom        (501) staff       (20)      637 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/plts/test_error.py
--rw-r--r--   0 tom        (501) staff       (20)     1248 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/plts/test_fg.py
--rw-r--r--   0 tom        (501) staff       (20)      987 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/plts/test_fm.py
--rw-r--r--   0 tom        (501) staff       (20)     1104 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/plts/test_periodic.py
--rw-r--r--   0 tom        (501) staff       (20)     4095 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/plts/test_spectra.py
--rw-r--r--   0 tom        (501) staff       (20)     2625 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/plts/test_styles.py
--rw-r--r--   0 tom        (501) staff       (20)      809 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/plts/test_templates.py
--rw-r--r--   0 tom        (501) staff       (20)     3396 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/plts/test_utils.py
--rw-r--r--   0 tom        (501) staff       (20)      544 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/settings.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-30 19:07:34.420603 fooof-1.1.0rc0/fooof/tests/sim/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/sim/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     4266 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/sim/test_gen.py
--rw-r--r--   0 tom        (501) staff       (20)     4050 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/sim/test_params.py
--rw-r--r--   0 tom        (501) staff       (20)     2503 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/sim/test_transform.py
--rw-r--r--   0 tom        (501) staff       (20)      328 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/sim/test_utils.py
--rw-r--r--   0 tom        (501) staff       (20)     2513 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/tutils.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-30 19:07:34.423155 fooof-1.1.0rc0/fooof/tests/utils/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/utils/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     2831 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/utils/test_data.py
--rw-r--r--   0 tom        (501) staff       (20)      315 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/utils/test_debug.py
--rw-r--r--   0 tom        (501) staff       (20)     1268 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/utils/test_download.py
--rw-r--r--   0 tom        (501) staff       (20)     1430 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/utils/test_io.py
--rw-r--r--   0 tom        (501) staff       (20)      575 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/utils/test_params.py
--rw-r--r--   0 tom        (501) staff       (20)      573 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/tests/utils/test_reports.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-30 19:07:34.425260 fooof-1.1.0rc0/fooof/utils/
--rw-r--r--   0 tom        (501) staff       (20)      112 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/utils/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     6887 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/utils/data.py
--rw-r--r--   0 tom        (501) staff       (20)      924 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/utils/debug.py
--rw-r--r--   0 tom        (501) staff       (20)     2419 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/utils/download.py
--rw-r--r--   0 tom        (501) staff       (20)     1626 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/utils/io.py
--rw-r--r--   0 tom        (501) staff       (20)     1637 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/utils/params.py
--rw-r--r--   0 tom        (501) staff       (20)     1675 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/utils/reports.py
--rw-r--r--   0 tom        (501) staff       (20)       24 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/fooof/version.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-30 19:07:34.393169 fooof-1.1.0rc0/fooof.egg-info/
--rw-r--r--   0 tom        (501) staff       (20)    13337 2023-06-30 19:07:34.000000 fooof-1.1.0rc0/fooof.egg-info/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)     2658 2023-06-30 19:07:34.000000 fooof-1.1.0rc0/fooof.egg-info/SOURCES.txt
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-06-30 19:07:34.000000 fooof-1.1.0rc0/fooof.egg-info/dependency_links.txt
--rw-r--r--   0 tom        (501) staff       (20)      105 2023-06-30 19:07:34.000000 fooof-1.1.0rc0/fooof.egg-info/requires.txt
--rw-r--r--   0 tom        (501) staff       (20)        6 2023-06-30 19:07:34.000000 fooof-1.1.0rc0/fooof.egg-info/top_level.txt
--rw-r--r--   0 tom        (501) staff       (20)       38 2023-06-30 19:07:34.426266 fooof-1.1.0rc0/setup.cfg
--rw-r--r--   0 tom        (501) staff       (20)     2466 2023-06-30 18:58:38.000000 fooof-1.1.0rc0/setup.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-21 19:21:34.771598 fooof-1.1.0rc1/
+-rw-r--r--   0 tom        (501) staff       (20)    11340 2019-01-23 01:14:03.000000 fooof-1.1.0rc1/LICENSE
+-rw-r--r--   0 tom        (501) staff       (20)       33 2023-07-21 19:12:54.000000 fooof-1.1.0rc1/MANIFEST.in
+-rw-r--r--   0 tom        (501) staff       (20)    13337 2023-07-21 19:21:34.771198 fooof-1.1.0rc1/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)    11796 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/README.rst
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-21 19:21:34.723908 fooof-1.1.0rc1/fooof/
+-rw-r--r--   0 tom        (501) staff       (20)      825 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/__init__.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-21 19:21:34.727379 fooof-1.1.0rc1/fooof/analysis/
+-rw-r--r--   0 tom        (501) staff       (20)      169 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/analysis/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     3837 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/analysis/error.py
+-rw-r--r--   0 tom        (501) staff       (20)     9350 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/analysis/periodic.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-21 19:21:34.729415 fooof-1.1.0rc1/fooof/bands/
+-rw-r--r--   0 tom        (501) staff       (20)       60 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/bands/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     4091 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/bands/bands.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-21 19:21:34.733976 fooof-1.1.0rc1/fooof/core/
+-rw-r--r--   0 tom        (501) staff       (20)       47 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/core/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      616 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/core/errors.py
+-rw-r--r--   0 tom        (501) staff       (20)     5271 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/core/funcs.py
+-rw-r--r--   0 tom        (501) staff       (20)     3860 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/core/info.py
+-rw-r--r--   0 tom        (501) staff       (20)     8226 2023-07-21 19:12:54.000000 fooof-1.1.0rc1/fooof/core/io.py
+-rw-r--r--   0 tom        (501) staff       (20)      411 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/core/items.py
+-rw-r--r--   0 tom        (501) staff       (20)     9298 2023-07-21 19:20:06.000000 fooof-1.1.0rc1/fooof/core/modutils.py
+-rw-r--r--   0 tom        (501) staff       (20)     4843 2023-07-21 19:12:54.000000 fooof-1.1.0rc1/fooof/core/reports.py
+-rw-r--r--   0 tom        (501) staff       (20)    14814 2023-07-21 19:12:54.000000 fooof-1.1.0rc1/fooof/core/strings.py
+-rw-r--r--   0 tom        (501) staff       (20)     6880 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/core/utils.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-21 19:21:34.735170 fooof-1.1.0rc1/fooof/data/
+-rw-r--r--   0 tom        (501) staff       (20)      106 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/data/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     3894 2023-07-21 19:12:54.000000 fooof-1.1.0rc1/fooof/data/conversions.py
+-rw-r--r--   0 tom        (501) staff       (20)     3784 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/data/data.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-21 19:21:34.737380 fooof-1.1.0rc1/fooof/objs/
+-rw-r--r--   0 tom        (501) staff       (20)      217 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/objs/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)    54716 2023-07-21 19:12:54.000000 fooof-1.1.0rc1/fooof/objs/fit.py
+-rw-r--r--   0 tom        (501) staff       (20)    24050 2023-07-21 19:17:17.000000 fooof-1.1.0rc1/fooof/objs/group.py
+-rw-r--r--   0 tom        (501) staff       (20)     9236 2023-07-21 19:12:54.000000 fooof-1.1.0rc1/fooof/objs/utils.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-21 19:21:34.742296 fooof-1.1.0rc1/fooof/plts/
+-rw-r--r--   0 tom        (501) staff       (20)       84 2023-07-21 19:12:54.000000 fooof-1.1.0rc1/fooof/plts/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)    10159 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/plts/annotate.py
+-rw-r--r--   0 tom        (501) staff       (20)     4754 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/plts/aperiodic.py
+-rw-r--r--   0 tom        (501) staff       (20)     1912 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/plts/error.py
+-rw-r--r--   0 tom        (501) staff       (20)     4115 2023-07-21 19:12:54.000000 fooof-1.1.0rc1/fooof/plts/fg.py
+-rw-r--r--   0 tom        (501) staff       (20)    12213 2023-07-21 19:12:54.000000 fooof-1.1.0rc1/fooof/plts/fm.py
+-rw-r--r--   0 tom        (501) staff       (20)     5105 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/plts/periodic.py
+-rw-r--r--   0 tom        (501) staff       (20)     2028 2023-07-21 19:12:54.000000 fooof-1.1.0rc1/fooof/plts/settings.py
+-rw-r--r--   0 tom        (501) staff       (20)     8110 2023-07-21 19:12:54.000000 fooof-1.1.0rc1/fooof/plts/spectra.py
+-rw-r--r--   0 tom        (501) staff       (20)     9326 2023-07-21 19:18:09.000000 fooof-1.1.0rc1/fooof/plts/style.py
+-rw-r--r--   0 tom        (501) staff       (20)     3930 2023-07-21 19:12:54.000000 fooof-1.1.0rc1/fooof/plts/templates.py
+-rw-r--r--   0 tom        (501) staff       (20)     6682 2023-07-21 19:12:54.000000 fooof-1.1.0rc1/fooof/plts/utils.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-21 19:21:34.745448 fooof-1.1.0rc1/fooof/sim/
+-rw-r--r--   0 tom        (501) staff       (20)      220 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/sim/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)    17522 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/sim/gen.py
+-rw-r--r--   0 tom        (501) staff       (20)     9749 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/sim/params.py
+-rw-r--r--   0 tom        (501) staff       (20)     9002 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/sim/transform.py
+-rw-r--r--   0 tom        (501) staff       (20)      468 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/sim/utils.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-21 19:21:34.747771 fooof-1.1.0rc1/fooof/tests/
+-rw-r--r--   0 tom        (501) staff       (20)       23 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/__init__.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-21 19:21:34.749202 fooof-1.1.0rc1/fooof/tests/analysis/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/analysis/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     1065 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/analysis/test_error.py
+-rw-r--r--   0 tom        (501) staff       (20)     2771 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/analysis/test_periodic.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-21 19:21:34.749792 fooof-1.1.0rc1/fooof/tests/bands/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/bands/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     1176 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/bands/test_bands.py
+-rw-r--r--   0 tom        (501) staff       (20)     1844 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/conftest.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-21 19:21:34.753671 fooof-1.1.0rc1/fooof/tests/core/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/core/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     2960 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/core/test_funcs.py
+-rw-r--r--   0 tom        (501) staff       (20)     1485 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/core/test_info.py
+-rw-r--r--   0 tom        (501) staff       (20)     5966 2023-07-21 19:12:54.000000 fooof-1.1.0rc1/fooof/tests/core/test_io.py
+-rw-r--r--   0 tom        (501) staff       (20)     3389 2023-07-21 19:12:54.000000 fooof-1.1.0rc1/fooof/tests/core/test_modutils.py
+-rw-r--r--   0 tom        (501) staff       (20)      766 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/core/test_reports.py
+-rw-r--r--   0 tom        (501) staff       (20)     1355 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/core/test_strings.py
+-rw-r--r--   0 tom        (501) staff       (20)     4127 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/core/test_utils.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-21 19:21:34.754665 fooof-1.1.0rc1/fooof/tests/data/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/data/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     1997 2023-07-21 19:12:54.000000 fooof-1.1.0rc1/fooof/tests/data/test_conversions.py
+-rw-r--r--   0 tom        (501) staff       (20)     1284 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/data/test_data.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-21 19:21:34.756084 fooof-1.1.0rc1/fooof/tests/objs/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/objs/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)    14153 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/objs/test_fit.py
+-rw-r--r--   0 tom        (501) staff       (20)    11469 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/objs/test_group.py
+-rw-r--r--   0 tom        (501) staff       (20)     4482 2023-07-21 19:12:54.000000 fooof-1.1.0rc1/fooof/tests/objs/test_utils.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-21 19:21:34.760636 fooof-1.1.0rc1/fooof/tests/plts/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/plts/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      895 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/plts/test_annotate.py
+-rw-r--r--   0 tom        (501) staff       (20)     1461 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/plts/test_aperiodic.py
+-rw-r--r--   0 tom        (501) staff       (20)      637 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/plts/test_error.py
+-rw-r--r--   0 tom        (501) staff       (20)     1248 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/plts/test_fg.py
+-rw-r--r--   0 tom        (501) staff       (20)     1549 2023-07-21 19:12:54.000000 fooof-1.1.0rc1/fooof/tests/plts/test_fm.py
+-rw-r--r--   0 tom        (501) staff       (20)     1104 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/plts/test_periodic.py
+-rw-r--r--   0 tom        (501) staff       (20)     4095 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/plts/test_spectra.py
+-rw-r--r--   0 tom        (501) staff       (20)     2625 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/plts/test_styles.py
+-rw-r--r--   0 tom        (501) staff       (20)      809 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/plts/test_templates.py
+-rw-r--r--   0 tom        (501) staff       (20)     3396 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/plts/test_utils.py
+-rw-r--r--   0 tom        (501) staff       (20)      544 2023-07-21 19:12:54.000000 fooof-1.1.0rc1/fooof/tests/settings.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-21 19:21:34.763173 fooof-1.1.0rc1/fooof/tests/sim/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/sim/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     4266 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/sim/test_gen.py
+-rw-r--r--   0 tom        (501) staff       (20)     4050 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/sim/test_params.py
+-rw-r--r--   0 tom        (501) staff       (20)     2503 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/sim/test_transform.py
+-rw-r--r--   0 tom        (501) staff       (20)      328 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/sim/test_utils.py
+-rw-r--r--   0 tom        (501) staff       (20)     2860 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/tutils.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-21 19:21:34.766448 fooof-1.1.0rc1/fooof/tests/utils/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/utils/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     3384 2023-07-21 19:12:54.000000 fooof-1.1.0rc1/fooof/tests/utils/test_data.py
+-rw-r--r--   0 tom        (501) staff       (20)      315 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/utils/test_debug.py
+-rw-r--r--   0 tom        (501) staff       (20)     1268 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/utils/test_download.py
+-rw-r--r--   0 tom        (501) staff       (20)     1430 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/utils/test_io.py
+-rw-r--r--   0 tom        (501) staff       (20)      575 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/utils/test_params.py
+-rw-r--r--   0 tom        (501) staff       (20)      573 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/utils/test_reports.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-21 19:21:34.770344 fooof-1.1.0rc1/fooof/utils/
+-rw-r--r--   0 tom        (501) staff       (20)      112 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/utils/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     8781 2023-07-21 19:12:54.000000 fooof-1.1.0rc1/fooof/utils/data.py
+-rw-r--r--   0 tom        (501) staff       (20)      924 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/utils/debug.py
+-rw-r--r--   0 tom        (501) staff       (20)     2549 2023-07-21 19:15:35.000000 fooof-1.1.0rc1/fooof/utils/download.py
+-rw-r--r--   0 tom        (501) staff       (20)     1634 2023-07-21 19:12:54.000000 fooof-1.1.0rc1/fooof/utils/io.py
+-rw-r--r--   0 tom        (501) staff       (20)     1637 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/utils/params.py
+-rw-r--r--   0 tom        (501) staff       (20)     1675 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/utils/reports.py
+-rw-r--r--   0 tom        (501) staff       (20)       24 2023-07-21 19:13:09.000000 fooof-1.1.0rc1/fooof/version.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-21 19:21:34.725460 fooof-1.1.0rc1/fooof.egg-info/
+-rw-r--r--   0 tom        (501) staff       (20)    13337 2023-07-21 19:21:34.000000 fooof-1.1.0rc1/fooof.egg-info/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)     2675 2023-07-21 19:21:34.000000 fooof-1.1.0rc1/fooof.egg-info/SOURCES.txt
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-07-21 19:21:34.000000 fooof-1.1.0rc1/fooof.egg-info/dependency_links.txt
+-rw-r--r--   0 tom        (501) staff       (20)      105 2023-07-21 19:21:34.000000 fooof-1.1.0rc1/fooof.egg-info/requires.txt
+-rw-r--r--   0 tom        (501) staff       (20)        6 2023-07-21 19:21:34.000000 fooof-1.1.0rc1/fooof.egg-info/top_level.txt
+-rw-r--r--   0 tom        (501) staff       (20)       17 2020-05-18 17:32:04.000000 fooof-1.1.0rc1/requirements.txt
+-rw-r--r--   0 tom        (501) staff       (20)       38 2023-07-21 19:21:34.771690 fooof-1.1.0rc1/setup.cfg
+-rw-r--r--   0 tom        (501) staff       (20)     2466 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/setup.py
```

### Comparing `fooof-1.1.0rc0/LICENSE` & `fooof-1.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc0/PKG-INFO` & `fooof-1.1.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fooof
-Version: 1.1.0rc0
+Version: 1.1.0rc1
 Summary: fitting oscillations & one-over f
 Home-page: https://github.com/fooof-tools/fooof
 Download-URL: https://github.com/fooof-tools/fooof/releases
 Author: The Voytek Lab
 Author-email: voyteklab@gmail.com
 Maintainer: Thomas Donoghue
 Maintainer-email: tdonoghue.research@gmail.com
```

### Comparing `fooof-1.1.0rc0/README.rst` & `fooof-1.1.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc0/fooof/__init__.py` & `fooof-1.1.0rc1/fooof/__init__.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc0/fooof/analysis/error.py` & `fooof-1.1.0rc1/fooof/analysis/error.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc0/fooof/analysis/periodic.py` & `fooof-1.1.0rc1/fooof/analysis/periodic.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc0/fooof/bands/bands.py` & `fooof-1.1.0rc1/fooof/bands/bands.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc0/fooof/core/errors.py` & `fooof-1.1.0rc1/fooof/core/errors.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc0/fooof/core/funcs.py` & `fooof-1.1.0rc1/fooof/core/funcs.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc0/fooof/core/info.py` & `fooof-1.1.0rc1/fooof/core/info.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc0/fooof/core/io.py` & `fooof-1.1.0rc1/fooof/core/io.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 
 def fpath(file_path, file_name):
     """Build the full file path from file name and directory.
 
     Parameters
     ----------
-    file_path : str or None
+    file_path : Path or str or None
         Path to the directory where the file is located.
     file_name : str
         Name of the file.
 
     Returns
     -------
     full_path : str
@@ -67,15 +67,15 @@
 
     Parameters
     ----------
     fm : FOOOF
         Object to save data from.
     file_name : str or FileObject
         File to save data to.
-    file_path : str, optional
+    file_path : Path or str, optional
         Path to directory to save to. If None, saves to current directory.
     append : bool, optional, default: False
         Whether to append to an existing file, if available.
         This option is only valid (and only used) if 'file_name' is a str.
     save_results : bool, optional
         Whether to save out FOOOF model fit results.
     save_settings : bool, optional
@@ -125,15 +125,15 @@
 
     Parameters
     ----------
     fg : FOOOFGroup
         Object to save data from.
     file_name : str or FileObject
         File to save data to.
-    file_path : str, optional
+    file_path : Path or str, optional
         Path to directory to load from. If None, loads from current directory.
     append : bool, optional, default: False
         Whether to append to an existing file, if available.
         This option is only valid (and only used) if 'file_name' is a str.
     save_results : bool, optional
         Whether to save out FOOOF model fit results.
     save_settings : bool, optional
@@ -171,15 +171,15 @@
 def load_json(file_name, file_path):
     """Load json file.
 
     Parameters
     ----------
     file_name : str or FileObject
         File to load data from.
-    file_path : str
+    file_path : Path or str
         Path to directory to load from.
 
     Returns
     -------
     data : dict
         Dictionary of data loaded from file.
     """
@@ -200,15 +200,15 @@
 def load_jsonlines(file_name, file_path):
     """Load a json-lines file, yielding data line by line.
 
     Parameters
     ----------
     file_name : str
         File to load data from.
-    file_path : str
+    file_path : Path or str
         Path to directory from load from.
 
     Yields
     ------
     dict
         Dictionary of data loaded from file.
     """
```

### Comparing `fooof-1.1.0rc0/fooof/core/reports.py` & `fooof-1.1.0rc1/fooof/core/reports.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
     Parameters
     ----------
     fm : FOOOF
         Object with results from fitting a power spectrum.
     file_name : str
         Name to give the saved out file.
-    file_path : str, optional
+    file_path : Path or str, optional
         Path to directory to save to. If None, saves to current directory.
     plt_log : bool, optional, default: False
         Whether or not to plot the frequency axis in log space.
     add_settings : bool, optional, default: True
         Whether to add a print out of the model settings to the end of the report.
     plot_kwargs : keyword arguments
         Keyword arguments to pass into the plot method.
@@ -79,48 +79,48 @@
 
     Parameters
     ----------
     fg : FOOOFGroup
         Object with results from fitting a group of power spectra.
     file_name : str
         Name to give the saved out file.
-    file_path : str, optional
+    file_path : Path or str, optional
         Path to directory to save to. If None, saves to current directory.
     add_settings : bool, optional, default: True
         Whether to add a print out of the model settings to the end of the report.
     """
 
     # Define grid settings based on what is to be plotted
     n_rows = 4 if add_settings else 3
     height_ratios = [1.0, 1.0, 1.0, 0.5] if add_settings else [0.8, 1.0, 1.0]
 
     # Initialize figure
     _ = plt.figure(figsize=REPORT_FIGSIZE)
-    grid = gridspec.GridSpec(n_rows, 2, wspace=0.4, hspace=0.25, height_ratios=height_ratios)
+    grid = gridspec.GridSpec(n_rows, 2, wspace=0.35, hspace=0.25, height_ratios=height_ratios)
 
     # First / top: text results
     ax0 = plt.subplot(grid[0, :])
     results_str = gen_results_fg_str(fg)
     ax0.text(0.5, 0.7, results_str, REPORT_FONT, ha='center', va='center')
     ax0.set_frame_on(False)
     ax0.set(xticks=[], yticks=[])
 
     # Second - data plots
 
     # Aperiodic parameters plot
     ax1 = plt.subplot(grid[1, 0])
-    plot_fg_ap(fg, ax1)
+    plot_fg_ap(fg, ax1, custom_styler=None)
 
     # Goodness of fit plot
     ax2 = plt.subplot(grid[1, 1])
-    plot_fg_gf(fg, ax2)
+    plot_fg_gf(fg, ax2, custom_styler=None)
 
     # Peak center frequencies plot
     ax3 = plt.subplot(grid[2, :])
-    plot_fg_peak_cens(fg, ax3)
+    plot_fg_peak_cens(fg, ax3, custom_styler=None)
 
     # Third - Model settings
     if add_settings:
         ax4 = plt.subplot(grid[3, :])
         settings_str = gen_settings_str(fg, False)
         ax4.text(0.5, 0.1, settings_str, REPORT_FONT, ha='center', va='center')
         ax4.set_frame_on(False)
```

### Comparing `fooof-1.1.0rc0/fooof/core/strings.py` & `fooof-1.1.0rc1/fooof/core/strings.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,15 +205,15 @@
         '',
         'FOOOF - REPORTING',
         '',
 
         # Methods report information
         'To report on using FOOOF, you should report (at minimum):',
         '',
-        '- the code version that was used used',
+        '- the code version that was used',
         '- the algorithm settings that were used',
         '- the frequency range that was fit',
 
         # Footer
         '',
         '='
     ]
@@ -352,28 +352,25 @@
     n_peaks = len(fg.get_params('peak_params'))
     r2s = fg.get_params('r_squared')
     errors = fg.get_params('error')
     exps = fg.get_params('aperiodic_params', 'exponent')
     kns = fg.get_params('aperiodic_params', 'knee') \
         if fg.aperiodic_mode == 'knee' else np.array([0])
 
-    # Check if there are any power spectra that failed to fit
-    n_failed = sum(np.isnan(exps))
-
     str_lst = [
 
         # Header
         '=',
         '',
         ' FOOOF - GROUP RESULTS',
         '',
 
         # Group information
         'Number of power spectra in the Group: {}'.format(len(fg.group_results)),
-        *[el for el in ['{} power spectra failed to fit'.format(n_failed)] if n_failed],
+        *[el for el in ['{} power spectra failed to fit'.format(fg.n_null_)] if fg.n_null_],
         '',
 
         # Frequency range and resolution
         'The model was run on the frequency range {} - {} Hz'.format(
             int(np.floor(fg.freq_range[0])), int(np.ceil(fg.freq_range[1]))),
         'Frequency Resolution is {:1.2f} Hz'.format(fg.freq_res),
         '',
```

### Comparing `fooof-1.1.0rc0/fooof/core/utils.py` & `fooof-1.1.0rc1/fooof/core/utils.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc0/fooof/data/conversions.py` & `fooof-1.1.0rc1/fooof/data/conversions.py`

 * *Files 17% similar despite different names*

```diff
@@ -80,14 +80,40 @@
     pd.Series
         Model results organized into a dataframe.
     """
 
     return pd.Series(model_to_dict(fit_results, peak_org))
 
 
+def group_to_dict(fit_results, peak_org):
+    """Convert a group of model fit results into a dictionary.
+
+    Parameters
+    ----------
+    fit_results : list of FOOOFResults
+        List of FOOOFResults objects.
+    peak_org : int or Bands
+        How to organize peaks.
+        If int, extracts the first n peaks.
+        If Bands, extracts peaks based on band definitions.
+
+    Returns
+    -------
+    dict
+        Model results organized into a dictionary.
+    """
+
+    fr_dict = {ke : [] for ke in model_to_dict(fit_results[0], peak_org).keys()}
+    for f_res in fit_results:
+        for key, val in model_to_dict(f_res, peak_org).items():
+            fr_dict[key].append(val)
+
+    return fr_dict
+
+
 @check_dependency(pd, 'pandas')
 def group_to_dataframe(fit_results, peak_org):
     """Convert a group of model fit results into a dataframe.
 
     Parameters
     ----------
     fit_results : list of FOOOFResults
@@ -99,8 +125,8 @@
 
     Returns
     -------
     pd.DataFrame
         Model results organized into a dataframe.
     """
 
-    return pd.DataFrame([model_to_dataframe(f_res, peak_org) for f_res in fit_results])
+    return pd.DataFrame(group_to_dict(fit_results, peak_org))
```

### Comparing `fooof-1.1.0rc0/fooof/data/data.py` & `fooof-1.1.0rc1/fooof/data/data.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc0/fooof/objs/fit.py` & `fooof-1.1.0rc1/fooof/objs/fit.py`

 * *Files 1% similar despite different names*

```diff
@@ -375,38 +375,48 @@
         self.r_squared_ = fooof_result.r_squared
         self.error_ = fooof_result.error
 
         self._check_loaded_results(fooof_result._asdict())
 
 
     def report(self, freqs=None, power_spectrum=None, freq_range=None,
-               plt_log=False, **plot_kwargs):
+               plt_log=False, plot_full_range=False, **plot_kwargs):
         """Run model fit, and display a report, which includes a plot, and printed results.
 
         Parameters
         ----------
         freqs : 1d array, optional
             Frequency values for the power spectrum.
         power_spectrum : 1d array, optional
             Power values, which must be input in linear space.
         freq_range : list of [float, float], optional
             Desired frequency range to fit the model to.
             If not provided, fits across the entire given range.
         plt_log : bool, optional, default: False
             Whether or not to plot the frequency axis in log space.
+        plot_full_range : bool, default: False
+            If True, plots the full range of the given power spectrum.
+            Only relevant / effective if `freqs` and `power_spectrum` passed in in this call.
         **plot_kwargs
             Keyword arguments to pass into the plot method.
+            Plot options with a name conflict be passed by pre-pending 'plot_'.
+            e.g. `freqs`, `power_spectrum` and `freq_range`.
 
         Notes
         -----
         Data is optional, if data has already been added to the object.
         """
 
         self.fit(freqs, power_spectrum, freq_range)
-        self.plot(plt_log=plt_log, **plot_kwargs)
+        self.plot(plt_log=plt_log,
+                  freqs=freqs if plot_full_range else plot_kwargs.pop('plot_freqs', None),
+                  power_spectrum=power_spectrum if \
+                      plot_full_range else plot_kwargs.pop('plot_power_spectrum', None),
+                  freq_range=plot_kwargs.pop('plot_freq_range', None),
+                  **plot_kwargs)
         self.print_results(concise=False)
 
 
     def fit(self, freqs=None, power_spectrum=None, freq_range=None):
         """Fit the full power spectrum as a combination of periodic and aperiodic components.
 
         Parameters
@@ -635,20 +645,21 @@
         """
 
         return FOOOFResults(**{key.strip('_') : getattr(self, key) \
             for key in OBJ_DESC['results']})
 
 
     @copy_doc_func_to_method(plot_fm)
-    def plot(self, plot_peaks=None, plot_aperiodic=True, plt_log=False,
-             add_legend=True, save_fig=False, file_name=None, file_path=None,
-             ax=None, data_kwargs=None, model_kwargs=None,
+    def plot(self, plot_peaks=None, plot_aperiodic=True, freqs=None, power_spectrum=None,
+             freq_range=None, plt_log=False, add_legend=True, save_fig=False, file_name=None,
+             file_path=None, ax=None, data_kwargs=None, model_kwargs=None,
              aperiodic_kwargs=None, peak_kwargs=None, **plot_kwargs):
 
-        plot_fm(self, plot_peaks=plot_peaks, plot_aperiodic=plot_aperiodic, plt_log=plt_log,
+        plot_fm(self, plot_peaks=plot_peaks, plot_aperiodic=plot_aperiodic, freqs=freqs,
+                power_spectrum=power_spectrum, freq_range=freq_range, plt_log=plt_log,
                 add_legend=add_legend, save_fig=save_fig, file_name=file_name,
                 file_path=file_path, ax=ax, data_kwargs=data_kwargs, model_kwargs=model_kwargs,
                 aperiodic_kwargs=aperiodic_kwargs, peak_kwargs=peak_kwargs, **plot_kwargs)
 
 
     @copy_doc_func_to_method(save_report_fm)
     def save_report(self, file_name, file_path=None, plt_log=False,
@@ -667,15 +678,15 @@
     def load(self, file_name, file_path=None, regenerate=True):
         """Load in a FOOOF formatted JSON file to the current object.
 
         Parameters
         ----------
         file_name : str or FileObject
             File to load data from.
-        file_path : str or None, optional
+        file_path : Path or str, optional
             Path to directory to load from. If None, loads from current directory.
         regenerate : bool, optional, default: True
             Whether to regenerate the model fit from the loaded data, if data is available.
         """
 
         # Reset data in object, so old data can't interfere
         self._reset_data_results(True, True, True)
```

### Comparing `fooof-1.1.0rc0/fooof/objs/group.py` & `fooof-1.1.0rc1/fooof/objs/group.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,42 +16,34 @@
 from fooof.core.items import OBJ_DESC
 from fooof.core.info import get_indices
 from fooof.core.utils import check_inds
 from fooof.core.errors import NoModelError
 from fooof.core.reports import save_report_fg
 from fooof.core.strings import gen_results_fg_str
 from fooof.core.io import save_fg, load_jsonlines
-from fooof.core.modutils import copy_doc_func_to_method, safe_import
+from fooof.core.modutils import (copy_doc_func_to_method, safe_import,
+                                 docs_get_section, replace_docstring_sections)
 from fooof.data.conversions import group_to_dataframe
 
 ###################################################################################################
 ###################################################################################################
 
+@replace_docstring_sections([docs_get_section(FOOOF.__doc__, 'Parameters'),
+                             docs_get_section(FOOOF.__doc__, 'Notes')])
 class FOOOFGroup(FOOOF):
     """Model a group of power spectra as a combination of aperiodic and periodic components.
 
     WARNING: FOOOF expects frequency and power values in linear space.
 
     Passing in logged frequencies and/or power spectra is not detected,
     and will silently produce incorrect results.
 
     Parameters
     ----------
-    peak_width_limits : tuple of (float, float), optional, default: (0.5, 12.0)
-        Limits on possible peak width, as (lower_bound, upper_bound).
-    max_n_peaks : int, optional, default: inf
-        Maximum number of gaussians to be fit in a single spectrum.
-    min_peak_height : float, optional, default: 0
-        Absolute threshold for detecting peaks, in units of the input data.
-    peak_threshold : float, optional, default: 2.0
-        Relative threshold for detecting peaks, in units of standard deviation of the input data.
-    aperiodic_mode : {'fixed', 'knee'}
-        Which approach to take for fitting the aperiodic component.
-    verbose : bool, optional, default: True
-        Verbosity mode. If True, prints out warnings and general status updates.
+    %copied in from FOOOF object
 
     Attributes
     ----------
     freqs : 1d array
         Frequency values for the power spectra.
     power_spectra : 2d array
         Power values for the group of power spectra, as [n_power_spectra, n_freqs].
@@ -64,33 +56,22 @@
         Results of FOOOF model fit for each power spectrum.
     has_data : bool
         Whether data is loaded to the object.
     has_model : bool
         Whether model results are available in the object.
     n_peaks_ : int
         The number of peaks fit in the model.
-    n_failed_fits_ : int
-        The number of models that failed to fit.
-    failed_fit_inds_ : list of int
-        The indices of any models that failed to fit.
+    n_null_ : int
+        The number of models that failed to fit and/or that are marked as null.
+    null_inds_ : list of int
+        The indices of any models that are null.
 
     Notes
     -----
-    - Commonly used abbreviations used in this module include:
-      CF: center frequency, PW: power, BW: Bandwidth, AP: aperiodic
-    - Input power spectra must be provided in linear scale.
-      Internally they are stored in log10 scale, as this is what the model operates upon.
-    - Input power spectra should be smooth, as overly noisy power spectra may lead to bad fits.
-      For example, raw FFT inputs are not appropriate. Where possible and appropriate, use
-      longer time segments for power spectrum calculation to get smoother power spectra,
-      as this will give better model fits.
-    - The gaussian params are those that define the gaussian of the fit, where as the peak
-      params are a modified version, in which the CF of the peak is the mean of the gaussian,
-      the PW of the peak is the height of the gaussian over and above the aperiodic component,
-      and the BW of the peak, is 2*std of the gaussian (as 'two sided' bandwidth).
+    %copied in from FOOOF object
     - The FOOOFGroup object inherits from the FOOOF object. As such it also has data
       attributes (`power_spectrum` & `fooofed_spectrum_`), and parameter attributes
       (`aperiodic_params_`, `peak_params_`, `gaussian_params_`, `r_squared_`, `error_`)
       which are defined in the context of individual model fits. These attributes are
       used during the fitting process, but in the group context do not store results
       post-fitting. Rather, all model fit results are collected and stored into the
       `group_results` attribute. To access individual parameters of the fit, use
@@ -418,15 +399,15 @@
     def load(self, file_name, file_path=None):
         """Load FOOOFGroup data from file.
 
         Parameters
         ----------
         file_name : str
             File to load data from.
-        file_path : str, optional
+        file_path : Path or str, optional
             Path to directory to load from. If None, loads from current directory.
         """
 
         # Clear results so as not to have possible prior results interfere
         self._reset_group_results()
 
         power_spectra = []
@@ -548,26 +529,26 @@
 
         Parameters
         ----------
         index : int
             Index of the model fit to save out.
         file_name : str
             Name to give the saved out file.
-        file_path : str, optional
+        file_path : Path or str, optional
             Path to directory to save to. If None, saves to current directory.
         plt_log : bool, optional, default: False
             Whether or not to plot the frequency axis in log space.
         add_settings : bool, optional, default: True
             Whether to add a print out of the model settings to the end of the report.
         plot_kwargs : keyword arguments
             Keyword arguments to pass into the plot method.
         """
 
         self.get_fooof(ind=index, regenerate=True).save_report(\
-            file_name, file_path, plt_log, **plot_kwargs)
+            file_name, file_path, plt_log, add_settings, **plot_kwargs)
 
 
     def to_df(self, peak_org):
         """Convert and extract the model results as a pandas object.
 
         Parameters
         ----------
```

### Comparing `fooof-1.1.0rc0/fooof/plts/annotate.py` & `fooof-1.1.0rc1/fooof/plts/annotate.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc0/fooof/plts/aperiodic.py` & `fooof-1.1.0rc1/fooof/plts/aperiodic.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc0/fooof/plts/error.py` & `fooof-1.1.0rc1/fooof/plts/error.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc0/fooof/plts/fg.py` & `fooof-1.1.0rc1/fooof/plts/fg.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,44 +27,44 @@
     ----------
     fg : FOOOFGroup
         Object containing results from fitting a group of power spectra.
     save_fig : bool, optional, default: False
         Whether to save out a copy of the plot.
     file_name : str, optional
         Name to give the saved out file.
-    file_path : str, optional
+    file_path : Path or str, optional
         Path to directory to save to. If None, saves to current directory.
 
     Raises
     ------
     NoModelError
         If the FOOOF object does not have model fit data available to plot.
     """
 
     if not fg.has_model:
         raise NoModelError("No model fit results are available, can not proceed.")
 
     fig = plt.figure(figsize=plot_kwargs.pop('figsize', PLT_FIGSIZES['group']))
-    gs = gridspec.GridSpec(2, 2, wspace=0.4, hspace=0.25, height_ratios=[1, 1.2])
+    gs = gridspec.GridSpec(2, 2, wspace=0.35, hspace=0.35, height_ratios=[1, 1.2])
 
     # Apply scatter kwargs to all subplots
     scatter_kwargs = plot_kwargs
     scatter_kwargs['all_axes'] = True
 
     # Aperiodic parameters plot
     ax0 = plt.subplot(gs[0, 0])
-    plot_fg_ap(fg, ax0, **scatter_kwargs)
+    plot_fg_ap(fg, ax0, **scatter_kwargs, custom_styler=None)
 
     # Goodness of fit plot
     ax1 = plt.subplot(gs[0, 1])
-    plot_fg_gf(fg, ax1, **scatter_kwargs)
+    plot_fg_gf(fg, ax1, **scatter_kwargs, custom_styler=None)
 
     # Center frequencies plot
     ax2 = plt.subplot(gs[1, :])
-    plot_fg_peak_cens(fg, ax2, **plot_kwargs)
+    plot_fg_peak_cens(fg, ax2, **plot_kwargs, custom_styler=None)
 
 
 @savefig
 @style_plot
 @check_dependency(plt, 'matplotlib')
 def plot_fg_ap(fg, ax=None, **plot_kwargs):
     """Plot aperiodic fit parameters, in a scatter plot.
```

### Comparing `fooof-1.1.0rc0/fooof/plts/fm.py` & `fooof-1.1.0rc1/fooof/plts/fm.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,37 +21,46 @@
 
 ###################################################################################################
 ###################################################################################################
 
 @savefig
 @style_plot
 @check_dependency(plt, 'matplotlib')
-def plot_fm(fm, plot_peaks=None, plot_aperiodic=True, plt_log=False, add_legend=True,
-            save_fig=False, file_name=None, file_path=None, ax=None, data_kwargs=None,
-            model_kwargs=None, aperiodic_kwargs=None, peak_kwargs=None, **plot_kwargs):
+def plot_fm(fm, plot_peaks=None, plot_aperiodic=True, freqs=None, power_spectrum=None,
+            freq_range=None, plt_log=False, add_legend=True, save_fig=False, file_name=None,
+            file_path=None, ax=None, data_kwargs=None, model_kwargs=None, aperiodic_kwargs=None,
+            peak_kwargs=None, **plot_kwargs):
     """Plot the power spectrum and model fit results from a FOOOF object.
 
     Parameters
     ----------
     fm : FOOOF
         Object containing a power spectrum and (optionally) results from fitting.
     plot_peaks : None or {'shade', 'dot', 'outline', 'line'}, optional
         What kind of approach to take to plot peaks. If None, peaks are not specifically plotted.
         Can also be a combination of approaches, separated by '-', for example: 'shade-line'.
     plot_aperiodic : boolean, optional, default: True
         Whether to plot the aperiodic component of the model fit.
+    freqs : 1d array, optional
+        Frequency values of the power spectrum to plot, in linear space.
+        If provided, this overrides the values in the model object.
+    power_spectrum : 1d array, optional
+        Power values to plot, in linear space.
+        If provided, this overrides the values in the model object.
+    freq_range : list of [float, float], optional
+        Frequency range to plot, defined in linear space.
     plt_log : boolean, optional, default: False
         Whether to plot the frequency values in log10 spacing.
     add_legend : boolean, optional, default: False
         Whether to add a legend describing the plot components.
     save_fig : bool, optional, default: False
         Whether to save out a copy of the plot.
     file_name : str, optional
         Name to give the saved out file.
-    file_path : str, optional
+    file_path : Path or str, optional
         Path to directory to save to. If None, saves to current directory.
     ax : matplotlib.Axes, optional
         Figure axes upon which to plot.
     data_kwargs, model_kwargs, aperiodic_kwargs, peak_kwargs : None or dict, optional
         Keyword arguments to pass into the plot call for each plot element.
     **plot_kwargs
         Keyword arguments to pass into the ``style_plot``.
@@ -60,24 +69,30 @@
     -----
     Since FOOOF objects store power values in log spacing,
     the y-axis (power) is plotted in log spacing by default.
     """
 
     ax = check_ax(ax, plot_kwargs.pop('figsize', PLT_FIGSIZES['spectral']))
 
+    # Check inputs for what to plot
+    custom_spectrum = (np.any(freqs) and np.any(power_spectrum))
+
     # Log settings - note that power values in FOOOF objects are already logged
     log_freqs = plt_log
     log_powers = False
 
     # Plot the data, if available
-    if fm.has_data:
+    if fm.has_data or custom_spectrum:
         data_defaults = {'color' : PLT_COLORS['data'], 'linewidth' : 2.0,
                          'label' : 'Original Spectrum' if add_legend else None}
         data_kwargs = check_plot_kwargs(data_kwargs, data_defaults)
-        plot_spectra(fm.freqs, fm.power_spectrum, log_freqs, log_powers, ax=ax, **data_kwargs)
+        plot_spectra(freqs if custom_spectrum else fm.freqs,
+                     power_spectrum if custom_spectrum else fm.power_spectrum,
+                     log_freqs, log_powers if not custom_spectrum else True,
+                     freq_range, ax=ax, **data_kwargs)
 
     # Add the full model fit, and components (if requested)
     if fm.has_model:
         model_defaults = {'color' : PLT_COLORS['model'], 'linewidth' : 3.0, 'alpha' : 0.5,
                           'label' : 'Full Model Fit' if add_legend else None}
         model_kwargs = check_plot_kwargs(model_kwargs, model_defaults)
         plot_spectra(fm.freqs, fm.fooofed_spectrum_, log_freqs, log_powers, ax=ax, **model_kwargs)
```

### Comparing `fooof-1.1.0rc0/fooof/plts/periodic.py` & `fooof-1.1.0rc1/fooof/plts/periodic.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc0/fooof/plts/settings.py` & `fooof-1.1.0rc1/fooof/plts/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 from collections import OrderedDict
 
 ###################################################################################################
 ###################################################################################################
 
 # Define default figure sizes
-PLT_FIGSIZES = {'spectral' : (10, 8),
+PLT_FIGSIZES = {'spectral' : (8.5, 6.5),
                 'params' : (7, 6),
-                'group' : (12, 10)}
+                'group' : (9, 7)}
 
 # Define defaults for colors for plots, based on what is plotted
 PLT_COLORS = {'data' : 'black',
               'periodic' : 'green',
               'aperiodic' : 'blue',
               'model' : 'red'}
 
@@ -41,12 +41,12 @@
 CUSTOM_STYLE_ARGS = ['title_fontsize', 'label_size', 'tick_labelsize',
                      'legend_size', 'legend_loc']
 STYLERS = ['axis_styler', 'line_styler', 'custom_styler']
 STYLE_ARGS = AXIS_STYLE_ARGS + LINE_STYLE_ARGS + CUSTOM_STYLE_ARGS + STYLERS
 
 ## Define default values for plot aesthetics
 # These are all custom style arguments
-TITLE_FONTSIZE = 20
-LABEL_SIZE = 16
-TICK_LABELSIZE = 16
+TITLE_FONTSIZE = 18
+LABEL_SIZE = 14
+TICK_LABELSIZE = 12
 LEGEND_SIZE = 12
 LEGEND_LOC = 'best'
```

### Comparing `fooof-1.1.0rc0/fooof/plts/spectra.py` & `fooof-1.1.0rc1/fooof/plts/spectra.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,67 +20,79 @@
 
 ###################################################################################################
 ###################################################################################################
 
 @savefig
 @style_plot
 @check_dependency(plt, 'matplotlib')
-def plot_spectra(freqs, power_spectra, log_freqs=False, log_powers=False,
+def plot_spectra(freqs, power_spectra, log_freqs=False, log_powers=False, freq_range=None,
                  colors=None, labels=None, ax=None, **plot_kwargs):
     """Plot one or multiple power spectra.
 
     Parameters
     ----------
     freqs : 1d or 2d array or list of 1d array
         Frequency values, to be plotted on the x-axis.
     power_spectra : 1d or 2d array or list of 1d array
         Power values, to be plotted on the y-axis.
     log_freqs : bool, optional, default: False
         Whether to plot the frequency axis in log spacing.
     log_powers : bool, optional, default: False
         Whether to plot the power axis in log spacing.
+    freq_range : list of [float, float], optional
+        Frequency range to plot, defined in linear space.
     colors : list of str, optional, default: None
         Line colors of the spectra.
     labels : list of str, optional, default: None
         Legend labels for the spectra.
     ax : matplotlib.Axes, optional
         Figure axes upon which to plot.
     **plot_kwargs
-        Keyword arguments to pass into the ``style_plot``.
+        Additional plot related keyword arguments.
     """
 
     ax = check_ax(ax, plot_kwargs.pop('figsize', PLT_FIGSIZES['spectral']))
 
     # Create the plot
     plot_kwargs = check_plot_kwargs(plot_kwargs, {'linewidth' : 2.0})
 
+    # Check for frequency range input, and log if x-axis is in log space
+    if freq_range is not None:
+        freq_range = np.log10(freq_range) if log_freqs else freq_range
+
     # Make inputs iterable if need to be passed multiple times to plot each spectrum
     plt_powers = np.reshape(power_spectra, (1, -1)) if np.ndim(power_spectra) == 1 else \
         power_spectra
     plt_freqs = repeat(freqs) if isinstance(freqs, np.ndarray) and freqs.ndim == 1 else freqs
 
     # Set labels
     labels = plot_kwargs.pop('label') if 'label' in plot_kwargs.keys() and labels is None else labels
     labels = repeat(labels) if not isinstance(labels, list) else cycle(labels)
     colors = repeat(colors) if not isinstance(colors, list) else cycle(colors)
 
-    # Plot
+    # Plot power spectra, looping across all spectra to plot
     for freqs, powers, color, label in zip(plt_freqs, plt_powers, colors, labels):
 
         # Set plot data, logging if requested, and collect color, if absent
         freqs = np.log10(freqs) if log_freqs else freqs
         powers = np.log10(powers) if log_powers else powers
         if color:
             plot_kwargs['color'] = color
 
         ax.plot(freqs, powers, label=label, **plot_kwargs)
 
+    ax.set_xlim(freq_range)
+
     style_spectrum_plot(ax, log_freqs, log_powers)
 
 
+# Alias `plot_spectrum` to `plot_spectra` for backwards compatibility
+plot_spectrum = plot_spectra
+
+
 @savefig
 @check_dependency(plt, 'matplotlib')
 def plot_spectra_shading(freqs, power_spectra, shades, shade_colors='r',
                          add_center=False, ax=None, **plot_kwargs):
     """Plot one or multiple power spectra with a shaded frequency region (or regions).
 
     Parameters
@@ -94,15 +106,16 @@
     shade_colors : str or list of string
         Color(s) to plot shades.
     add_center : bool, optional, default: False
         Whether to add a line at the center point of the shaded regions.
     ax : matplotlib.Axes, optional
         Figure axes upon which to plot.
     **plot_kwargs
-        Keyword arguments to pass into :func:`~.plot_spectra`.
+        Additional plot related keyword arguments.
+        This can include additional inputs into :func:`~.plot_spectra`.
 
     Notes
     -----
     Parameters for `plot_spectra` can also be passed into this function as keyword arguments.
 
     This includes `log_freqs`, `log_powers` & `labels`. See `plot_spectra` for usage details.
     """
@@ -144,15 +157,15 @@
     color : str, optional, default: None
         Line color of the spectrum.
     label : str, optional, default: None
         Legend label for the spectrum.
     ax : matplotlib.Axes, optional
         Figure axes upon which to plot.
     **plot_kwargs
-        Keyword arguments to be passed to `plot_spectra` or to the plot call.
+        Additional plot related keyword arguments.
     """
 
     if (isinstance(shade, str) or isfunction(shade)) and power_spectra.ndim != 2:
         raise ValueError('Power spectra must be 2d if shade is not given.')
 
     ax = check_ax(ax, plot_kwargs.pop('figsize', PLT_FIGSIZES['spectral']))
```

### Comparing `fooof-1.1.0rc0/fooof/plts/style.py` & `fooof-1.1.0rc1/fooof/plts/style.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 from itertools import cycle
 from functools import wraps
 
 import matplotlib.pyplot as plt
 
 from fooof.plts.settings import (AXIS_STYLE_ARGS, LINE_STYLE_ARGS, COLLECTION_STYLE_ARGS,
-                                 CUSTOM_STYLE_ARGS, STYLE_ARGS, LABEL_SIZE, LEGEND_SIZE,
-                                 LEGEND_LOC, TICK_LABELSIZE, TITLE_FONTSIZE)
+                                 STYLE_ARGS, LABEL_SIZE, LEGEND_SIZE, LEGEND_LOC,
+                                 TICK_LABELSIZE, TITLE_FONTSIZE)
 
 ###################################################################################################
 ###################################################################################################
 
 def style_spectrum_plot(ax, log_freqs, log_powers):
     """Apply style and aesthetics to a power spectrum plot.
 
@@ -165,15 +165,22 @@
                    labelsize=kwargs.pop('tick_labelsize', TICK_LABELSIZE))
 
     # If labels were provided, add a legend
     if ax.get_legend_handles_labels()[0]:
         ax.legend(prop={'size': kwargs.pop('legend_size', LEGEND_SIZE)},
                   loc=kwargs.pop('legend_loc', LEGEND_LOC))
 
-    plt.tight_layout()
+    # Apply tight layout to the figure object, if matplotlib is new enough
+    #   If available, `.set_layout_engine` should be equivalent to
+    #   `plt.tight_layout()`, but seems to raise fewer warnings...
+    try:
+        fig = plt.gcf()
+        fig.set_layout_engine('tight')
+    except:
+        plt.tight_layout()
 
 
 def apply_style(ax, axis_styler=apply_axis_style, line_styler=apply_line_style,
                 collection_styler=apply_collection_style, custom_styler=apply_custom_style,
                 **kwargs):
     """Apply plot style to a figure axis.
 
@@ -188,18 +195,18 @@
 
     Notes
     -----
     This function wraps sub-functions which apply style to different plot elements.
     Each of these sub-functions can be replaced by passing in replacement callables.
     """
 
-    axis_styler(ax, **kwargs)
-    line_styler(ax, **kwargs)
-    collection_styler(ax, **kwargs)
-    custom_styler(ax, **kwargs)
+    axis_styler(ax, **kwargs) if axis_styler is not None else None
+    line_styler(ax, **kwargs) if line_styler is not None else None
+    collection_styler(ax, **kwargs) if collection_styler is not None else None
+    custom_styler(ax, **kwargs) if custom_styler is not None else None
 
 
 def style_plot(func, *args, **kwargs):
     """Decorator function to apply a plot style function, after plot generation.
 
     Parameters
     ----------
```

### Comparing `fooof-1.1.0rc0/fooof/plts/templates.py` & `fooof-1.1.0rc1/fooof/plts/templates.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 They are not expected to be used directly by the user.
 """
 
 import numpy as np
 
 from fooof.core.modutils import safe_import, check_dependency
 from fooof.plts.utils import check_ax, set_alpha
+from fooof.plts.settings import TITLE_FONTSIZE, LABEL_SIZE, TICK_LABELSIZE
 
 plt = safe_import('.pyplot', 'matplotlib')
 
 ###################################################################################################
 ###################################################################################################
 
 @check_dependency(plt, 'matplotlib')
@@ -42,22 +43,22 @@
 
     # Create x-axis data, with small jitter for visualization purposes
     x_data = np.ones_like(data) * x_val + np.random.normal(0, 0.025, data.shape)
 
     ax.scatter(x_data, data, s=36, alpha=set_alpha(len(data)))
 
     if label:
-        ax.set_ylabel(label, fontsize=16)
+        ax.set_ylabel(label, fontsize=LABEL_SIZE)
         ax.set(xticks=[x_val], xticklabels=[label])
 
     if title:
-        ax.set_title(title, fontsize=20)
+        ax.set_title(title, fontsize=TITLE_FONTSIZE)
 
-    ax.tick_params(axis='x', labelsize=16)
-    ax.tick_params(axis='y', labelsize=12)
+    ax.tick_params(axis='x', labelsize=TICK_LABELSIZE)
+    ax.tick_params(axis='y', labelsize=TICK_LABELSIZE)
 
     ax.set_xlim([-0.5, 0.5])
 
 
 @check_dependency(plt, 'matplotlib')
 def plot_scatter_2(data_0, label_0, data_1, label_1, title=None, ax=None):
     """Plot a scatter plot, with two y-axes.
@@ -85,20 +86,20 @@
     ax = check_ax(ax)
     ax1 = ax.twinx()
 
     plot_scatter_1(data_0, label_0, ax=ax)
     plot_scatter_1(data_1, label_1, x_val=1, ax=ax1)
 
     if title:
-        ax.set_title(title, fontsize=20)
+        ax.set_title(title, fontsize=TITLE_FONTSIZE)
 
     ax.set(xlim=[-0.5, 1.5],
            xticks=[0, 1],
            xticklabels=[label_0, label_1])
-    ax.tick_params(axis='x', labelsize=16)
+    ax.tick_params(axis='x', labelsize=TICK_LABELSIZE)
 
 
 @check_dependency(plt, 'matplotlib')
 def plot_hist(data, label, title=None, n_bins=25, x_lims=None, ax=None):
     """Plot a histogram.
 
     Parameters
@@ -117,17 +118,17 @@
         Figure axes upon which to plot.
     """
 
     ax = check_ax(ax)
 
     ax.hist(data[~np.isnan(data)], n_bins, range=x_lims, alpha=0.8)
 
-    ax.set_xlabel(label, fontsize=16)
-    ax.set_ylabel('Count', fontsize=16)
+    ax.set_xlabel(label, fontsize=LABEL_SIZE)
+    ax.set_ylabel('Count', fontsize=LABEL_SIZE)
 
     if x_lims:
         ax.set_xlim(x_lims)
 
     if title:
-        ax.set_title(title, fontsize=20)
+        ax.set_title(title, fontsize=TITLE_FONTSIZE)
 
-    ax.tick_params(axis='both', labelsize=12)
+    ax.tick_params(axis='both', labelsize=TICK_LABELSIZE)
```

### Comparing `fooof-1.1.0rc0/fooof/plts/utils.py` & `fooof-1.1.0rc1/fooof/plts/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -207,15 +207,15 @@
 def save_figure(file_name, file_path=None, close=False, **save_kwargs):
     """Save out a figure.
 
     Parameters
     ----------
     file_name : str
         File name for the figure file to save out.
-    file_path : str or Path
+    file_path : Path or str
         Path for where to save out the figure to.
     close : bool, optional, default: False
         Whether to close the plot after saving.
     save_kwargs
         Additional arguments to pass into the save function.
     """
```

### Comparing `fooof-1.1.0rc0/fooof/sim/gen.py` & `fooof-1.1.0rc1/fooof/sim/gen.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc0/fooof/sim/params.py` & `fooof-1.1.0rc1/fooof/sim/params.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc0/fooof/sim/transform.py` & `fooof-1.1.0rc1/fooof/sim/transform.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc0/fooof/tests/analysis/test_error.py` & `fooof-1.1.0rc1/fooof/tests/analysis/test_error.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc0/fooof/tests/analysis/test_periodic.py` & `fooof-1.1.0rc1/fooof/tests/analysis/test_periodic.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc0/fooof/tests/bands/test_bands.py` & `fooof-1.1.0rc1/fooof/tests/bands/test_bands.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc0/fooof/tests/conftest.py` & `fooof-1.1.0rc1/fooof/tests/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import shutil
 import pytest
 
 import numpy as np
 
 from fooof.core.modutils import safe_import
 
-from fooof.tests.tutils import get_tfm, get_tfg, get_tbands, get_tresults
+from fooof.tests.tutils import get_tfm, get_tfg, get_tbands, get_tresults, get_tdocstring
 from fooof.tests.settings import (BASE_TEST_FILE_PATH, TEST_DATA_PATH,
                                   TEST_REPORTS_PATH, TEST_PLOTS_PATH)
 
 plt = safe_import('.pyplot', 'matplotlib')
 
 ###################################################################################################
 ###################################################################################################
@@ -48,14 +48,18 @@
 def tbands():
     yield get_tbands()
 
 @pytest.fixture(scope='session')
 def tresults():
     yield get_tresults()
 
+@pytest.fixture(scope='function')
+def tdocstring():
+    yield get_tdocstring()
+
 @pytest.fixture(scope='session')
 def skip_if_no_mpl():
     if not safe_import('matplotlib'):
         pytest.skip('Matplotlib not available: skipping test.')
 
 @pytest.fixture(scope='session')
 def skip_if_no_pandas():
```

### Comparing `fooof-1.1.0rc0/fooof/tests/core/test_funcs.py` & `fooof-1.1.0rc1/fooof/tests/core/test_funcs.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc0/fooof/tests/core/test_info.py` & `fooof-1.1.0rc1/fooof/tests/core/test_info.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc0/fooof/tests/core/test_io.py` & `fooof-1.1.0rc1/fooof/tests/core/test_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Tests for fooof.core.io."""
 
 import os
+from pathlib import Path
 
 from fooof.core.items import OBJ_DESC
 
 from fooof.tests.settings import TEST_DATA_PATH
 
 from fooof.core.io import *
 
@@ -22,14 +23,15 @@
     assert fname('report.png', 'pdf') == 'report.png'
 
 def test_fpath():
     """Check that the file path checker helper function properly checks / combines file paths."""
 
     assert fpath(None, 'data.json') == 'data.json'
     assert fpath('/path/', 'data.json') == '/path/data.json'
+    assert fpath(Path('/path/'), 'data.json') == '/path/data.json'
 
 def test_save_fm_str(tfm):
     """Check saving fm data, with file specifiers as strings."""
 
     # Test saving out each set of save elements
     file_name_res = 'test_fooof_res'
     file_name_set = 'test_fooof_set'
```

### Comparing `fooof-1.1.0rc0/fooof/tests/core/test_reports.py` & `fooof-1.1.0rc1/fooof/tests/core/test_reports.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc0/fooof/tests/core/test_strings.py` & `fooof-1.1.0rc1/fooof/tests/core/test_strings.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc0/fooof/tests/core/test_utils.py` & `fooof-1.1.0rc1/fooof/tests/core/test_utils.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc0/fooof/tests/data/test_conversions.py` & `fooof-1.1.0rc1/fooof/tests/data/test_conversions.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,14 +37,25 @@
     for peak_org in [1, 2, 3]:
         out = model_to_dataframe(tresults, peak_org=peak_org)
         assert isinstance(out, pd.Series)
 
     out = model_to_dataframe(tresults, peak_org=tbands)
     assert isinstance(out, pd.Series)
 
+def test_group_to_dict(tresults, tbands):
+
+    fit_results = [deepcopy(tresults), deepcopy(tresults), deepcopy(tresults)]
+
+    for peak_org in [1, 2, 3]:
+        out = group_to_dict(fit_results, peak_org=peak_org)
+        assert isinstance(out, dict)
+
+    out = group_to_dict(fit_results, peak_org=tbands)
+    assert isinstance(out, dict)
+
 def test_group_to_dataframe(tresults,  tbands, skip_if_no_pandas):
 
     fit_results = [deepcopy(tresults), deepcopy(tresults), deepcopy(tresults)]
 
     for peak_org in [1, 2, 3]:
         out = group_to_dataframe(fit_results, peak_org=peak_org)
         assert isinstance(out, pd.DataFrame)
```

### Comparing `fooof-1.1.0rc0/fooof/tests/data/test_data.py` & `fooof-1.1.0rc1/fooof/tests/data/test_data.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc0/fooof/tests/objs/test_fit.py` & `fooof-1.1.0rc1/fooof/tests/objs/test_fit.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc0/fooof/tests/objs/test_group.py` & `fooof-1.1.0rc1/fooof/tests/objs/test_group.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc0/fooof/tests/objs/test_utils.py` & `fooof-1.1.0rc1/fooof/tests/objs/test_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -41,14 +41,21 @@
         average_fg(tfg, tbands, avg_method='BAD')
 
     # Test no data available error
     ntfg = FOOOFGroup()
     with raises(NoModelError):
         average_fg(ntfg, tbands)
 
+def test_average_reconstructions(tfg):
+
+    freqs, avg_model = average_reconstructions(tfg)
+    assert isinstance(freqs, np.ndarray)
+    assert isinstance(avg_model, np.ndarray)
+    assert freqs.shape == avg_model.shape
+
 def test_combine_fooofs(tfm, tfg):
 
     tfm2 = tfm.copy()
     tfm3 = tfm.copy()
     tfg2 = tfg.copy()
     tfg3 = tfg.copy()
```

### Comparing `fooof-1.1.0rc0/fooof/tests/plts/test_annotate.py` & `fooof-1.1.0rc1/fooof/tests/plts/test_annotate.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc0/fooof/tests/plts/test_aperiodic.py` & `fooof-1.1.0rc1/fooof/tests/plts/test_aperiodic.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc0/fooof/tests/plts/test_error.py` & `fooof-1.1.0rc1/fooof/tests/plts/test_error.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc0/fooof/tests/plts/test_fg.py` & `fooof-1.1.0rc1/fooof/tests/plts/test_fg.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc0/fooof/tests/plts/test_periodic.py` & `fooof-1.1.0rc1/fooof/tests/plts/test_periodic.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc0/fooof/tests/plts/test_spectra.py` & `fooof-1.1.0rc1/fooof/tests/plts/test_spectra.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc0/fooof/tests/plts/test_styles.py` & `fooof-1.1.0rc1/fooof/tests/plts/test_styles.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc0/fooof/tests/plts/test_templates.py` & `fooof-1.1.0rc1/fooof/tests/plts/test_templates.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc0/fooof/tests/plts/test_utils.py` & `fooof-1.1.0rc1/fooof/tests/plts/test_utils.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc0/fooof/tests/settings.py` & `fooof-1.1.0rc1/fooof/tests/settings.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Settings for testing fooof."""
 
 import os
-import pkg_resources as pkg
+from pathlib import Path
 
 ###################################################################################################
 ###################################################################################################
 
 # Path Settings
-BASE_TEST_FILE_PATH = pkg.resource_filename(__name__, 'test_files')
-TEST_DATA_PATH = os.path.join(BASE_TEST_FILE_PATH, 'data')
-TEST_REPORTS_PATH = os.path.join(BASE_TEST_FILE_PATH, 'reports')
-TEST_PLOTS_PATH = os.path.join(BASE_TEST_FILE_PATH, 'plots')
+TESTS_PATH = Path(os.path.abspath(os.path.dirname(__file__)))
+BASE_TEST_FILE_PATH = TESTS_PATH / 'test_files'
+TEST_DATA_PATH = BASE_TEST_FILE_PATH / 'data'
+TEST_REPORTS_PATH = BASE_TEST_FILE_PATH / 'reports'
+TEST_PLOTS_PATH = BASE_TEST_FILE_PATH / 'plots'
```

### Comparing `fooof-1.1.0rc0/fooof/tests/sim/test_gen.py` & `fooof-1.1.0rc1/fooof/tests/sim/test_gen.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc0/fooof/tests/sim/test_params.py` & `fooof-1.1.0rc1/fooof/tests/sim/test_params.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc0/fooof/tests/sim/test_transform.py` & `fooof-1.1.0rc1/fooof/tests/sim/test_transform.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc0/fooof/tests/tutils.py` & `fooof-1.1.0rc1/fooof/tests/tutils.py`

 * *Files 12% similar despite different names*

```diff
@@ -50,14 +50,35 @@
     """Get a FOOOFResults objet, for testing."""
 
     return FOOOFResults(aperiodic_params=np.array([1.0, 1.00]),
                         peak_params=np.array([[10.0, 1.25, 2.0], [20.0, 1.0, 3.0]]),
                         r_squared=0.97, error=0.01,
                         gaussian_params=np.array([[10.0, 1.25, 1.0], [20.0, 1.0, 1.5]]))
 
+def get_tdocstring():
+    """Get an example docstring, for testing."""
+
+    docstring = \
+    """This is a test doctring.
+
+    Parameters
+    ----------
+    first : thing
+        Words, words, words.
+    second : stuff
+        Words, words, words.
+
+    Returns
+    -------
+    out : yay
+        Words, words, words.
+    """
+
+    return docstring
+
 def default_group_params():
     """Create default parameters for generating a test group of power spectra."""
 
     freq_range = [3, 50]
     ap_opts = param_sampler([[20, 2], [50, 2.5], [35, 1.5]])
     gauss_opts = param_sampler([[10, 0.5, 2], [10, 0.5, 2, 20, 0.3, 4]])
```

### Comparing `fooof-1.1.0rc0/fooof/tests/utils/test_data.py` & `fooof-1.1.0rc1/fooof/tests/utils/test_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,14 +46,29 @@
     assert np.all(powers)
     assert powers.shape == powers_out.shape
 
     for f_range in exclude:
         mask = np.logical_and(freqs >= f_range[0], freqs <= f_range[1])
         assert powers[mask].sum() > powers_out[mask].sum()
 
+def test_interpolate_spectra():
+
+    freqs, powers = gen_group_power_spectra(\
+        5, [1, 150], [1, 100, 1], [[10, 0.5, 1.0], [60, 1, 0.1], [120, 0.5, 0.1]])
+
+    exclude = [[58, 62], [118, 122]]
+    freqs_out, powers_out = interpolate_spectra(freqs, powers, exclude)
+    assert np.array_equal(freqs, freqs_out)
+    assert np.all(powers)
+    assert powers.shape == powers_out.shape
+
+    for f_range in exclude:
+        mask = np.logical_and(freqs >= f_range[0], freqs <= f_range[1])
+        assert powers[:, mask].sum() > powers_out[:, mask].sum()
+
 def test_subsample_spectra():
 
     # Simulate spectra, each with unique osc peak (for checking)
     n_sim = 10
     oscs = [[10 + ind, 0.25, 0.5] for ind in range(n_sim)]
     freqs, powers = gen_group_power_spectra(\
         n_sim, [1, 50], [1, 1], oscs)
```

### Comparing `fooof-1.1.0rc0/fooof/tests/utils/test_download.py` & `fooof-1.1.0rc1/fooof/tests/utils/test_download.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc0/fooof/tests/utils/test_io.py` & `fooof-1.1.0rc1/fooof/tests/utils/test_io.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc0/fooof/tests/utils/test_params.py` & `fooof-1.1.0rc1/fooof/tests/utils/test_params.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc0/fooof/tests/utils/test_reports.py` & `fooof-1.1.0rc1/fooof/tests/utils/test_reports.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc0/fooof/utils/data.py` & `fooof-1.1.0rc1/fooof/utils/data.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 """Utilities for working with data and models."""
 
 from itertools import repeat
+from functools import partial
 
 import numpy as np
 
+from fooof.core.modutils import docs_get_section, replace_docstring_sections
+
 ###################################################################################################
 ###################################################################################################
 
 def trim_spectrum(freqs, power_spectra, f_range):
     """Extract a frequency range from power spectra.
 
     Parameters
@@ -134,14 +137,63 @@
                          [np.median(xs1), np.median(xs2)],
                          [np.median(ys1), np.median(ys2)])
         powers[interp_mask] = np.power(10, vals)
 
     return freqs, powers
 
 
+def wrap_interpolate_spectrum(powers, freqs, interp_range, buffer):
+    """Wraps interpolate function, organizing inputs & outputs to use `partial`."""
+    return interpolate_spectrum(freqs, powers, interp_range, buffer)[1]
+
+
+@replace_docstring_sections(docs_get_section(interpolate_spectrum.__doc__, 'Notes', end='Examples'))
+def interpolate_spectra(freqs, powers, interp_range, buffer=3):
+    """Interpolate a frequency region across a group of power spectra.
+
+    Parameters
+    ----------
+    freqs : 1d array
+        Frequency values for the power spectrum.
+    powers : 2d array
+        Power values for the power spectra.
+    interp_range : list of float or list of list of float
+        Frequency range to interpolate, as [lowest_freq, highest_freq].
+        If a list of lists, applies each as it's own interpolation range.
+    buffer : int or list of int
+        The number of samples to use on either side of the interpolation
+        range, that are then averaged and used to calculate the interpolation.
+
+    Returns
+    -------
+    freqs : 1d array
+        Frequency values for the power spectrum.
+    powers : 2d array
+        Power values, with interpolation, for the power spectra.
+
+    Notes
+    -----
+    % copied in from interpolate_spectrum
+
+    Examples
+    --------
+    Using simulated spectra, interpolate away line noise peaks:
+
+    >>> from fooof.sim import gen_group_power_spectra
+    >>> freqs, powers = gen_group_power_spectra(5, [1, 75], [1, 1], [[10, 0.5, 1.0], [60, 2, 0.1]])
+    >>> freqs, powers = interpolate_spectra(freqs, powers, [58, 62])
+    """
+
+    tfunc = partial(wrap_interpolate_spectrum, freqs=freqs,
+                    interp_range=interp_range, buffer=buffer)
+    powers = np.apply_along_axis(tfunc, 1, powers)
+
+    return freqs,powers
+
+
 def subsample_spectra(spectra, selection, return_inds=False):
     """Subsample a group of power spectra.
 
     Parameters
     ----------
     spectra : 2d array
         A group of power spectra to subsample from.
```

### Comparing `fooof-1.1.0rc0/fooof/utils/debug.py` & `fooof-1.1.0rc1/fooof/utils/debug.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc0/fooof/utils/download.py` & `fooof-1.1.0rc1/fooof/utils/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,57 +1,61 @@
 """Functions and utilities for downloading example data for fooof."""
 
 import os
 from urllib.request import urlretrieve
 
 import numpy as np
 
+from fooof.core.io import fpath
+
 ###################################################################################################
 ###################################################################################################
 
 DATA_URL = 'https://raw.githubusercontent.com/fooof-tools/fooof/main/data/'
 
 def check_data_folder(folder):
     """Check if a data folder exists, and create if not.
 
     Parameters
     ----------
-    folder : str
+    folder : Path or str
         Name of the folder to check and create if missing.
     """
 
     if folder and not os.path.isdir(folder):
         os.mkdir(folder)
 
 
 def check_data_file(filename, folder, url=DATA_URL):
     """Check if a data folder exists, and download it if not.
 
     Parameters
     ----------
     filename : str
         Name of the data file to check and download if missing.
-    folder : str
+    folder : Path or str
         Name of the folder to save the datafile to.
+    url : str, optional
+        The URL to download the data file from.
     """
 
-    filepath = os.path.join(folder, filename)
+    filepath = fpath(folder, filename)
 
     if not os.path.isfile(filepath):
         urlretrieve(url + filename, filename=filepath)
 
 
 def fetch_fooof_data(filename, folder='data', url=DATA_URL):
     """Download a data file for FOOOF.
 
     Parameters
     ----------
     filename : str
         Name of the data file to download.
-    folder : str, optional
+    folder : Path or str, optional
         Name of the folder to save the datafile to.
     url : str, optional
         The URL to download the data file from.
 
     Notes
     -----
     This function checks if the file already exists, and downloads it if not.
@@ -65,15 +69,15 @@
 def load_fooof_data(filename, folder='data', url=DATA_URL):
     """Download, if not already available, and load an example data file for fooof.
 
     Parameters
     ----------
     filename : str
         Name of the data file to download.
-    folder : str, optional
+    folder : Path or str, optional
         Name of the folder to save the datafile to.
     url : str, optional
         The URL to download the data file from.
 
     Returns
     -------
     data : ndarray
```

### Comparing `fooof-1.1.0rc0/fooof/utils/io.py` & `fooof-1.1.0rc1/fooof/utils/io.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def load_fooof(file_name, file_path=None, regenerate=True):
     """Load a FOOOF file into a FOOOF object.
 
     Parameters
     ----------
     file_name : str or FileObject
         File to load the data from.
-    file_path : str or None, optional
+    file_path : Path or str, optional
         Path to directory to load from. If None, loads from current directory.
     regenerate : bool, optional, default: True
         Whether to regenerate the model fit from the loaded data, if data is available.
 
     Returns
     -------
     fm : FOOOF
@@ -34,15 +34,15 @@
 def load_fooofgroup(file_name, file_path=None):
     """Load data from file into a FOOOFGroup object.
 
     Parameters
     ----------
     file_name : str
         File to load data data.
-    file_path : str, optional
+    file_path : Path or str, optional
         Path to directory to load from. If None, loads from current directory.
 
     Returns
     -------
     fg : FOOOFGroup
         Object with the loaded data.
     """
```

### Comparing `fooof-1.1.0rc0/fooof/utils/params.py` & `fooof-1.1.0rc1/fooof/utils/params.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc0/fooof/utils/reports.py` & `fooof-1.1.0rc1/fooof/utils/reports.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc0/fooof.egg-info/PKG-INFO` & `fooof-1.1.0rc1/fooof.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fooof
-Version: 1.1.0rc0
+Version: 1.1.0rc1
 Summary: fitting oscillations & one-over f
 Home-page: https://github.com/fooof-tools/fooof
 Download-URL: https://github.com/fooof-tools/fooof/releases
 Author: The Voytek Lab
 Author-email: voyteklab@gmail.com
 Maintainer: Thomas Donoghue
 Maintainer-email: tdonoghue.research@gmail.com
```

### Comparing `fooof-1.1.0rc0/fooof.egg-info/SOURCES.txt` & `fooof-1.1.0rc1/fooof.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.rst
+requirements.txt
 setup.py
 fooof/__init__.py
 fooof/version.py
 fooof.egg-info/PKG-INFO
 fooof.egg-info/SOURCES.txt
 fooof.egg-info/dependency_links.txt
 fooof.egg-info/requires.txt
```

### Comparing `fooof-1.1.0rc0/setup.py` & `fooof-1.1.0rc1/setup.py`

 * *Files identical despite different names*

