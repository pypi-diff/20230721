# Comparing `tmp/napari_boxmanager-0.4.1.tar.gz` & `tmp/napari_boxmanager-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari_boxmanager-0.4.1.tar", last modified: Thu Jul 20 13:09:00 2023, max compression
+gzip compressed data, was "napari_boxmanager-0.4.2.tar", last modified: Fri Jul 21 10:29:37 2023, max compression
```

## Comparing `napari_boxmanager-0.4.1.tar` & `napari_boxmanager-0.4.2.tar`

### file list

```diff
@@ -1,142 +1,142 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:09:00.457433 napari_boxmanager-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:09:00.409431 napari_boxmanager-0.4.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:09:00.417431 napari_boxmanager-0.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:09:00.417431 napari_boxmanager-0.4.1/.napari/
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/.napari/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-07-20 13:09:00.457433 napari_boxmanager-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:09:00.421431 napari_boxmanager-0.4.1/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      232 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/bin/napari_boxmanager
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/conda_env.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:09:00.421431 napari_boxmanager-0.4.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:09:00.421431 napari_boxmanager-0.4.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/docs/_static/version-alert.js
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:09:00.421431 napari_boxmanager-0.4.1/docs/manual/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/docs/manual/general.rst
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/docs/manual/manual.rst
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/docs/manual/read.rst
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/docs/manual/write.rst
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-20 13:09:00.457433 napari_boxmanager-0.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:09:00.413431 napari_boxmanager-0.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:09:00.425431 napari_boxmanager-0.4.1/src/box_manager/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/src/box_manager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:09:00.425431 napari_boxmanager-0.4.1/src/box_manager/_qt/
--rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/src/box_manager/_qt/FilterImage.py
--rw-r--r--   0 runner    (1001) docker     (123)    14148 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/src/box_manager/_qt/OrganizeBox.py
--rw-r--r--   0 runner    (1001) docker     (123)    21663 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/src/box_manager/_qt/OrganizeLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    84364 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/src/box_manager/_qt/SelectMetric.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/src/box_manager/_qt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:09:00.425431 napari_boxmanager-0.4.1/src/box_manager/_qt/_icons/
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/src/box_manager/_qt/_icons/checkmark_black.png
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/src/box_manager/_qt/_icons/checkmark_white.png
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/src/box_manager/_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/src/box_manager/_sample_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:09:00.429432 napari_boxmanager-0.4.1/src/box_manager/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/src/box_manager/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/src/box_manager/_tests/test_box.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/src/box_manager/_tests/test_cbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/src/box_manager/_tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/src/box_manager/_tests/test_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/src/box_manager/_tests/test_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/src/box_manager/_tests/test_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:09:00.429432 napari_boxmanager-0.4.1/src/box_manager/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/src/box_manager/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/src/box_manager/_utils/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/src/box_manager/_utils/general.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-20 13:09:00.000000 napari_boxmanager-0.4.1/src/box_manager/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/src/box_manager/_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/src/box_manager/_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:09:00.433432 napari_boxmanager-0.4.1/src/box_manager/io/
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/src/box_manager/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9837 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/src/box_manager/io/box.py
--rw-r--r--   0 runner    (1001) docker     (123)    12263 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/src/box_manager/io/cbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/src/box_manager/io/coords.py
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/src/box_manager/io/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    20447 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/src/box_manager/io/io_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/src/box_manager/io/mrc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/src/box_manager/io/star.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/src/box_manager/io/tif.py
--rw-r--r--   0 runner    (1001) docker     (123)    10463 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/src/box_manager/io/tloc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/src/box_manager/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:09:00.437432 napari_boxmanager-0.4.1/src/napari_boxmanager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-07-20 13:09:00.000000 napari_boxmanager-0.4.1/src/napari_boxmanager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-07-20 13:09:00.000000 napari_boxmanager-0.4.1/src/napari_boxmanager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 13:09:00.000000 napari_boxmanager-0.4.1/src/napari_boxmanager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-20 13:09:00.000000 napari_boxmanager-0.4.1/src/napari_boxmanager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-20 13:09:00.000000 napari_boxmanager-0.4.1/src/napari_boxmanager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-20 13:09:00.000000 napari_boxmanager-0.4.1/src/napari_boxmanager.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:09:00.449432 napari_boxmanager-0.4.1/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    41024 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/test_data/2d.mrc
--rw-r--r--   0 runner    (1001) docker     (123)    41024 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/test_data/2d_0.mrc
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/test_data/2d_0_center.box
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/test_data/2d_center.box
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/test_data/2d_center_float.box
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/test_data/2d_corrupt_has_string.box
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/test_data/2d_corrupt_unqual_columns.box
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/test_data/2d_empty.box
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/test_data/2d_left.box
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/test_data/2d_particles.cbox
--rw-r--r--   0 runner    (1001) docker     (123)  4001024 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/test_data/3d.mrc
--rw-r--r--   0 runner    (1001) docker     (123)  4001024 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/test_data/3d.mrci
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/test_data/3d_particle.cbox
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:09:00.453433 napari_boxmanager-0.4.1/test_data/box_data/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/test_data/box_data/create_data.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/test_data/box_data/test_0.box
--rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/test_data/box_data/test_0.mrc
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/test_data/box_data/test_0_new.box
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/test_data/box_data/test_1.box
--rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/test_data/box_data/test_1.mrc
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/test_data/box_data/test_1_centered.box
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/test_data/box_data/test_1_new.box
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/test_data/box_data/test_2.box
--rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/test_data/box_data/test_2.mrc
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/test_data/box_data/test_2_centered.box
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/test_data/box_data/test_2_new.box
--rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/test_data/box_data/test_3.mrc
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/test_data/box_data/test_4.box
--rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/test_data/box_data/test_4.mrc
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/test_data/box_data/test_4_new.box
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/test_data/box_data/test_5.box
--rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/test_data/box_data/test_5.mrc
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/test_data/box_data/test_6.box
--rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/test_data/box_data/test_6.mrc
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/test_data/box_data/test_6_centered.box
--rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/test_data/box_data/test_7.mrc
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/test_data/box_data/test_7_centered.box
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/test_data/box_data/test_7_new.box
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/test_data/box_data/test_8.box
--rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/test_data/box_data/test_8.mrc
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/test_data/box_data/test_8_centered.box
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/test_data/box_data/test_9.box
--rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/test_data/box_data/test_9.mrc
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/test_data/box_data/test_9_new.box
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:09:00.457433 napari_boxmanager-0.4.1/test_data/filament_cbox_2d/
--rw-r--r--   0 runner    (1001) docker     (123)    19405 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/test_data/filament_cbox_2d/ActLifeact_02885.cbox
--rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/test_data/filament_cbox_2d/ActLifeact_03047.cbox
--rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/test_data/filament_cbox_2d/ActLifeact_03070.cbox
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/test_data/filament_cbox_2d/ActLifeact_03211.cbox
--rw-r--r--   0 runner    (1001) docker     (123)    63796 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/test_data/filament_cbox_2d/ActLifeact_04203.cbox
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/test_data/filament_cbox_2d/empty.cbox
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:09:00.457433 napari_boxmanager-0.4.1/test_data/particle_cbox_2d/
--rw-r--r--   0 runner    (1001) docker     (123)    11983 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/test_data/particle_cbox_2d/TcdA1-0018_frames_sum.cbox
--rw-r--r--   0 runner    (1001) docker     (123)    12858 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/test_data/particle_cbox_2d/TcdA1-0019_frames_sum.cbox
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/test_data/valid.tloc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:09:00.457433 napari_boxmanager-0.4.1/test_data/valid_box/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/test_data/valid_box/2d.box
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/test_data/valid_box/2d_0.box
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/test_data/valid_missing_dim_z.tloc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:09:00.457433 napari_boxmanager-0.4.1/test_data/valid_mrc/
--rw-r--r--   0 runner    (1001) docker     (123)    41024 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/test_data/valid_mrc/2d.mrc
--rw-r--r--   0 runner    (1001) docker     (123)    41024 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/test_data/valid_mrc/2d_0.mrc
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-20 13:08:42.000000 napari_boxmanager-0.4.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:37.025013 napari_boxmanager-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:37.005013 napari_boxmanager-0.4.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:37.005013 napari_boxmanager-0.4.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:37.005013 napari_boxmanager-0.4.2/.napari/
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/.napari/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-07-21 10:29:37.025013 napari_boxmanager-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:37.005013 napari_boxmanager-0.4.2/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      232 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/bin/napari_boxmanager
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/conda_env.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:37.005013 napari_boxmanager-0.4.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:37.005013 napari_boxmanager-0.4.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/docs/_static/version-alert.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:37.009013 napari_boxmanager-0.4.2/docs/manual/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/docs/manual/general.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/docs/manual/manual.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/docs/manual/read.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/docs/manual/write.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-21 10:29:37.025013 napari_boxmanager-0.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:37.005013 napari_boxmanager-0.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:37.009013 napari_boxmanager-0.4.2/src/box_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/src/box_manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:37.009013 napari_boxmanager-0.4.2/src/box_manager/_qt/
+-rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/src/box_manager/_qt/FilterImage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14148 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/src/box_manager/_qt/OrganizeBox.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21663 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/src/box_manager/_qt/OrganizeLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84364 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/src/box_manager/_qt/SelectMetric.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/src/box_manager/_qt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:37.009013 napari_boxmanager-0.4.2/src/box_manager/_qt/_icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/src/box_manager/_qt/_icons/checkmark_black.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/src/box_manager/_qt/_icons/checkmark_white.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/src/box_manager/_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/src/box_manager/_sample_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:37.009013 napari_boxmanager-0.4.2/src/box_manager/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/src/box_manager/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/src/box_manager/_tests/test_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/src/box_manager/_tests/test_cbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/src/box_manager/_tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/src/box_manager/_tests/test_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/src/box_manager/_tests/test_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/src/box_manager/_tests/test_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:37.009013 napari_boxmanager-0.4.2/src/box_manager/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/src/box_manager/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/src/box_manager/_utils/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/src/box_manager/_utils/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-21 10:29:36.000000 napari_boxmanager-0.4.2/src/box_manager/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/src/box_manager/_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/src/box_manager/_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:37.009013 napari_boxmanager-0.4.2/src/box_manager/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/src/box_manager/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9837 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/src/box_manager/io/box.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12263 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/src/box_manager/io/cbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/src/box_manager/io/coords.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/src/box_manager/io/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20447 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/src/box_manager/io/io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/src/box_manager/io/mrc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/src/box_manager/io/star.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/src/box_manager/io/tif.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10463 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/src/box_manager/io/tloc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/src/box_manager/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:37.013013 napari_boxmanager-0.4.2/src/napari_boxmanager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-07-21 10:29:36.000000 napari_boxmanager-0.4.2/src/napari_boxmanager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-07-21 10:29:37.000000 napari_boxmanager-0.4.2/src/napari_boxmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 10:29:36.000000 napari_boxmanager-0.4.2/src/napari_boxmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-21 10:29:36.000000 napari_boxmanager-0.4.2/src/napari_boxmanager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-21 10:29:36.000000 napari_boxmanager-0.4.2/src/napari_boxmanager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-21 10:29:36.000000 napari_boxmanager-0.4.2/src/napari_boxmanager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:37.021013 napari_boxmanager-0.4.2/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    41024 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/test_data/2d.mrc
+-rw-r--r--   0 runner    (1001) docker     (123)    41024 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/test_data/2d_0.mrc
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/test_data/2d_0_center.box
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/test_data/2d_center.box
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/test_data/2d_center_float.box
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/test_data/2d_corrupt_has_string.box
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/test_data/2d_corrupt_unqual_columns.box
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/test_data/2d_empty.box
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/test_data/2d_left.box
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/test_data/2d_particles.cbox
+-rw-r--r--   0 runner    (1001) docker     (123)  4001024 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/test_data/3d.mrc
+-rw-r--r--   0 runner    (1001) docker     (123)  4001024 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/test_data/3d.mrci
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/test_data/3d_particle.cbox
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:37.025013 napari_boxmanager-0.4.2/test_data/box_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/test_data/box_data/create_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/test_data/box_data/test_0.box
+-rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/test_data/box_data/test_0.mrc
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/test_data/box_data/test_0_new.box
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/test_data/box_data/test_1.box
+-rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/test_data/box_data/test_1.mrc
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/test_data/box_data/test_1_centered.box
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/test_data/box_data/test_1_new.box
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/test_data/box_data/test_2.box
+-rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/test_data/box_data/test_2.mrc
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/test_data/box_data/test_2_centered.box
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/test_data/box_data/test_2_new.box
+-rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/test_data/box_data/test_3.mrc
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/test_data/box_data/test_4.box
+-rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/test_data/box_data/test_4.mrc
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/test_data/box_data/test_4_new.box
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/test_data/box_data/test_5.box
+-rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/test_data/box_data/test_5.mrc
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/test_data/box_data/test_6.box
+-rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/test_data/box_data/test_6.mrc
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/test_data/box_data/test_6_centered.box
+-rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/test_data/box_data/test_7.mrc
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/test_data/box_data/test_7_centered.box
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/test_data/box_data/test_7_new.box
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/test_data/box_data/test_8.box
+-rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/test_data/box_data/test_8.mrc
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/test_data/box_data/test_8_centered.box
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/test_data/box_data/test_9.box
+-rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/test_data/box_data/test_9.mrc
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/test_data/box_data/test_9_new.box
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:37.025013 napari_boxmanager-0.4.2/test_data/filament_cbox_2d/
+-rw-r--r--   0 runner    (1001) docker     (123)    19405 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/test_data/filament_cbox_2d/ActLifeact_02885.cbox
+-rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/test_data/filament_cbox_2d/ActLifeact_03047.cbox
+-rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/test_data/filament_cbox_2d/ActLifeact_03070.cbox
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/test_data/filament_cbox_2d/ActLifeact_03211.cbox
+-rw-r--r--   0 runner    (1001) docker     (123)    63796 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/test_data/filament_cbox_2d/ActLifeact_04203.cbox
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/test_data/filament_cbox_2d/empty.cbox
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:37.025013 napari_boxmanager-0.4.2/test_data/particle_cbox_2d/
+-rw-r--r--   0 runner    (1001) docker     (123)    11983 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/test_data/particle_cbox_2d/TcdA1-0018_frames_sum.cbox
+-rw-r--r--   0 runner    (1001) docker     (123)    12858 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/test_data/particle_cbox_2d/TcdA1-0019_frames_sum.cbox
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/test_data/valid.tloc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:37.025013 napari_boxmanager-0.4.2/test_data/valid_box/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/test_data/valid_box/2d.box
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/test_data/valid_box/2d_0.box
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/test_data/valid_missing_dim_z.tloc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:37.025013 napari_boxmanager-0.4.2/test_data/valid_mrc/
+-rw-r--r--   0 runner    (1001) docker     (123)    41024 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/test_data/valid_mrc/2d.mrc
+-rw-r--r--   0 runner    (1001) docker     (123)    41024 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/test_data/valid_mrc/2d_0.mrc
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-21 10:29:18.000000 napari_boxmanager-0.4.2/tox.ini
```

### Comparing `napari_boxmanager-0.4.1/.github/workflows/test_and_deploy.yml` & `napari_boxmanager-0.4.2/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/.gitignore` & `napari_boxmanager-0.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/.napari/DESCRIPTION.md` & `napari_boxmanager-0.4.2/.napari/DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/.pre-commit-config.yaml` & `napari_boxmanager-0.4.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/LICENSE` & `napari_boxmanager-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/PKG-INFO` & `napari_boxmanager-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari_boxmanager
-Version: 0.4.1
+Version: 0.4.2
 Summary: Particle selection tool for cryo-em
 Home-page: https://github.com/MPI-Dortmund/napari-boxmanager
 Author: Markus Stabrin
 Author-email: markus.stabrin@mpi-dortmund.mpg.de
 License: MPL-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: napari
```

### Comparing `napari_boxmanager-0.4.1/README.md` & `napari_boxmanager-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/docs/_static/version-alert.js` & `napari_boxmanager-0.4.2/docs/_static/version-alert.js`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/docs/changes.rst` & `napari_boxmanager-0.4.2/docs/changes.rst`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/docs/conf.py` & `napari_boxmanager-0.4.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/docs/manual/general.rst` & `napari_boxmanager-0.4.2/docs/manual/general.rst`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/setup.cfg` & `napari_boxmanager-0.4.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 [options]
 packages = find:
 install_requires = 
 	matplotlib
 	mrcfile
 	numpy <=1.23.5
 	pystardb>=0.4.2
-	napari>=0.4.18
+	napari>=0.4.17
 	pandas
 	pyqt5
 	scipy
 	tifffile
 	tqdm
 python_requires = >=3.10
 include_package_data = True
```

### Comparing `napari_boxmanager-0.4.1/src/box_manager/_qt/FilterImage.py` & `napari_boxmanager-0.4.2/src/box_manager/_qt/FilterImage.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/src/box_manager/_qt/OrganizeBox.py` & `napari_boxmanager-0.4.2/src/box_manager/_qt/OrganizeBox.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/src/box_manager/_qt/OrganizeLayer.py` & `napari_boxmanager-0.4.2/src/box_manager/_qt/OrganizeLayer.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/src/box_manager/_qt/SelectMetric.py` & `napari_boxmanager-0.4.2/src/box_manager/_qt/SelectMetric.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/src/box_manager/_qt/_icons/checkmark_black.png` & `napari_boxmanager-0.4.2/src/box_manager/_qt/_icons/checkmark_black.png`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/src/box_manager/_qt/_icons/checkmark_white.png` & `napari_boxmanager-0.4.2/src/box_manager/_qt/_icons/checkmark_white.png`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/src/box_manager/_reader.py` & `napari_boxmanager-0.4.2/src/box_manager/_reader.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/src/box_manager/_tests/test_box.py` & `napari_boxmanager-0.4.2/src/box_manager/_tests/test_box.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/src/box_manager/_tests/test_cbox.py` & `napari_boxmanager-0.4.2/src/box_manager/_tests/test_cbox.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/src/box_manager/_tests/test_reader.py` & `napari_boxmanager-0.4.2/src/box_manager/_tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/src/box_manager/_tests/test_widget.py` & `napari_boxmanager-0.4.2/src/box_manager/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/src/box_manager/_utils/filters.py` & `napari_boxmanager-0.4.2/src/box_manager/_utils/filters.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/src/box_manager/_utils/general.py` & `napari_boxmanager-0.4.2/src/box_manager/_utils/general.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/src/box_manager/_widget.py` & `napari_boxmanager-0.4.2/src/box_manager/_widget.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/src/box_manager/_writer.py` & `napari_boxmanager-0.4.2/src/box_manager/_writer.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/src/box_manager/io/__init__.py` & `napari_boxmanager-0.4.2/src/box_manager/io/__init__.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/src/box_manager/io/box.py` & `napari_boxmanager-0.4.2/src/box_manager/io/box.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/src/box_manager/io/cbox.py` & `napari_boxmanager-0.4.2/src/box_manager/io/cbox.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/src/box_manager/io/coords.py` & `napari_boxmanager-0.4.2/src/box_manager/io/coords.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/src/box_manager/io/interface.py` & `napari_boxmanager-0.4.2/src/box_manager/io/interface.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/src/box_manager/io/io_utils.py` & `napari_boxmanager-0.4.2/src/box_manager/io/io_utils.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/src/box_manager/io/mrc.py` & `napari_boxmanager-0.4.2/src/box_manager/io/mrc.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/src/box_manager/io/star.py` & `napari_boxmanager-0.4.2/src/box_manager/io/star.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/src/box_manager/io/tif.py` & `napari_boxmanager-0.4.2/src/box_manager/io/tif.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/src/box_manager/io/tloc.py` & `napari_boxmanager-0.4.2/src/box_manager/io/tloc.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/src/box_manager/napari.yaml` & `napari_boxmanager-0.4.2/src/box_manager/napari.yaml`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/src/napari_boxmanager.egg-info/PKG-INFO` & `napari_boxmanager-0.4.2/src/napari_boxmanager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-boxmanager
-Version: 0.4.1
+Version: 0.4.2
 Summary: Particle selection tool for cryo-em
 Home-page: https://github.com/MPI-Dortmund/napari-boxmanager
 Author: Markus Stabrin
 Author-email: markus.stabrin@mpi-dortmund.mpg.de
 License: MPL-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: napari
```

### Comparing `napari_boxmanager-0.4.1/src/napari_boxmanager.egg-info/SOURCES.txt` & `napari_boxmanager-0.4.2/src/napari_boxmanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/test_data/2d.mrc` & `napari_boxmanager-0.4.2/test_data/2d.mrc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/test_data/2d_0.mrc` & `napari_boxmanager-0.4.2/test_data/2d_0.mrc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/test_data/2d_particles.cbox` & `napari_boxmanager-0.4.2/test_data/2d_particles.cbox`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/test_data/3d.mrc` & `napari_boxmanager-0.4.2/test_data/3d.mrc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/test_data/3d.mrci` & `napari_boxmanager-0.4.2/test_data/3d.mrci`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/test_data/3d_particle.cbox` & `napari_boxmanager-0.4.2/test_data/3d_particle.cbox`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/test_data/box_data/create_data.py` & `napari_boxmanager-0.4.2/test_data/box_data/create_data.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/test_data/box_data/test_0.mrc` & `napari_boxmanager-0.4.2/test_data/box_data/test_0.mrc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/test_data/box_data/test_1.mrc` & `napari_boxmanager-0.4.2/test_data/box_data/test_1.mrc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/test_data/box_data/test_2.mrc` & `napari_boxmanager-0.4.2/test_data/box_data/test_2.mrc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/test_data/box_data/test_3.mrc` & `napari_boxmanager-0.4.2/test_data/box_data/test_3.mrc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/test_data/box_data/test_4.mrc` & `napari_boxmanager-0.4.2/test_data/box_data/test_4.mrc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/test_data/box_data/test_5.mrc` & `napari_boxmanager-0.4.2/test_data/box_data/test_5.mrc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/test_data/box_data/test_6.mrc` & `napari_boxmanager-0.4.2/test_data/box_data/test_6.mrc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/test_data/box_data/test_7.mrc` & `napari_boxmanager-0.4.2/test_data/box_data/test_7.mrc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/test_data/box_data/test_8.mrc` & `napari_boxmanager-0.4.2/test_data/box_data/test_8.mrc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/test_data/box_data/test_9.mrc` & `napari_boxmanager-0.4.2/test_data/box_data/test_9.mrc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/test_data/filament_cbox_2d/ActLifeact_02885.cbox` & `napari_boxmanager-0.4.2/test_data/filament_cbox_2d/ActLifeact_02885.cbox`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/test_data/filament_cbox_2d/ActLifeact_03047.cbox` & `napari_boxmanager-0.4.2/test_data/filament_cbox_2d/ActLifeact_03047.cbox`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/test_data/filament_cbox_2d/ActLifeact_03070.cbox` & `napari_boxmanager-0.4.2/test_data/filament_cbox_2d/ActLifeact_03070.cbox`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/test_data/filament_cbox_2d/ActLifeact_03211.cbox` & `napari_boxmanager-0.4.2/test_data/filament_cbox_2d/ActLifeact_03211.cbox`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/test_data/filament_cbox_2d/ActLifeact_04203.cbox` & `napari_boxmanager-0.4.2/test_data/filament_cbox_2d/ActLifeact_04203.cbox`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/test_data/particle_cbox_2d/TcdA1-0018_frames_sum.cbox` & `napari_boxmanager-0.4.2/test_data/particle_cbox_2d/TcdA1-0018_frames_sum.cbox`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/test_data/particle_cbox_2d/TcdA1-0019_frames_sum.cbox` & `napari_boxmanager-0.4.2/test_data/particle_cbox_2d/TcdA1-0019_frames_sum.cbox`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/test_data/valid.tloc` & `napari_boxmanager-0.4.2/test_data/valid.tloc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/test_data/valid_missing_dim_z.tloc` & `napari_boxmanager-0.4.2/test_data/valid_missing_dim_z.tloc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/test_data/valid_mrc/2d.mrc` & `napari_boxmanager-0.4.2/test_data/valid_mrc/2d.mrc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/test_data/valid_mrc/2d_0.mrc` & `napari_boxmanager-0.4.2/test_data/valid_mrc/2d_0.mrc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.1/tox.ini` & `napari_boxmanager-0.4.2/tox.ini`

 * *Files identical despite different names*

