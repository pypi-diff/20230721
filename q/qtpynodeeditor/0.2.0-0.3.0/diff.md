# Comparing `tmp/qtpynodeeditor-0.2.0.tar.gz` & `tmp/qtpynodeeditor-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/qtpynodeeditor-0.2.0.tar", last modified: Wed Sep  2 18:03:52 2020, max compression
+gzip compressed data, was "qtpynodeeditor-0.3.0.tar", last modified: Fri Jul 21 17:29:49 2023, max compression
```

## Comparing `qtpynodeeditor-0.2.0.tar` & `qtpynodeeditor-0.3.0.tar`

### file list

```diff
@@ -1,65 +1,78 @@
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2020-09-02 18:03:52.000000 qtpynodeeditor-0.2.0/
--rw-r--r--   0 klauer   (1318172782) 1704612529      130 2019-03-26 20:01:33.000000 qtpynodeeditor-0.2.0/AUTHORS.rst
--rw-r--r--   0 klauer   (1318172782) 1704612529     3076 2019-03-26 20:01:33.000000 qtpynodeeditor-0.2.0/CONTRIBUTING.rst
--rw-r--r--   0 klauer   (1318172782) 1704612529     1641 2019-03-23 18:16:34.000000 qtpynodeeditor-0.2.0/LICENSE
--rw-r--r--   0 klauer   (1318172782) 1704612529      351 2020-09-02 16:54:28.000000 qtpynodeeditor-0.2.0/MANIFEST.in
--rw-r--r--   0 klauer   (1318172782) 1704612529     2518 2020-09-02 18:03:52.000000 qtpynodeeditor-0.2.0/PKG-INFO
--rw-r--r--   0 klauer   (1318172782) 1704612529     1620 2020-09-02 17:58:41.000000 qtpynodeeditor-0.2.0/README.rst
--rw-r--r--   0 klauer   (1318172782) 1704612529      333 2019-03-26 20:01:33.000000 qtpynodeeditor-0.2.0/dev-requirements.txt
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2020-09-02 18:03:52.000000 qtpynodeeditor-0.2.0/docs/
--rw-r--r--   0 klauer   (1318172782) 1704612529      616 2019-03-26 20:01:33.000000 qtpynodeeditor-0.2.0/docs/Makefile
--rw-r--r--   0 klauer   (1318172782) 1704612529      786 2019-03-26 20:01:33.000000 qtpynodeeditor-0.2.0/docs/make.bat
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2020-09-02 18:03:52.000000 qtpynodeeditor-0.2.0/docs/source/
--rw-r--r--   0 klauer   (1318172782) 1704612529     2546 2020-09-02 17:58:41.000000 qtpynodeeditor-0.2.0/docs/source/api.rst
--rw-r--r--   0 klauer   (1318172782) 1704612529     5326 2020-09-02 16:54:28.000000 qtpynodeeditor-0.2.0/docs/source/conf.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     1506 2020-09-02 17:58:41.000000 qtpynodeeditor-0.2.0/docs/source/getting_started.rst
--rw-r--r--   0 klauer   (1318172782) 1704612529      494 2020-09-02 17:58:41.000000 qtpynodeeditor-0.2.0/docs/source/index.rst
--rw-r--r--   0 klauer   (1318172782) 1704612529     1846 2020-09-02 17:58:41.000000 qtpynodeeditor-0.2.0/docs/source/release_notes.rst
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2020-09-02 18:03:52.000000 qtpynodeeditor-0.2.0/qtpynodeeditor/
--rw-r--r--   0 klauer   (1318172782) 1704612529     1047 2019-03-26 20:01:33.000000 qtpynodeeditor-0.2.0/qtpynodeeditor/DefaultStyle.json
--rw-r--r--   0 klauer   (1318172782) 1704612529     2161 2020-09-02 17:58:41.000000 qtpynodeeditor-0.2.0/qtpynodeeditor/__init__.py
--rw-r--r--   0 klauer   (1318172782) 1704612529      497 2020-09-02 18:03:52.000000 qtpynodeeditor-0.2.0/qtpynodeeditor/_version.py
--rw-r--r--   0 klauer   (1318172782) 1704612529      431 2019-03-29 18:35:11.000000 qtpynodeeditor-0.2.0/qtpynodeeditor/base.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    11406 2020-09-02 16:54:28.000000 qtpynodeeditor-0.2.0/qtpynodeeditor/connection.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     3849 2020-09-02 16:54:28.000000 qtpynodeeditor-0.2.0/qtpynodeeditor/connection_geometry.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     6846 2020-09-02 16:54:28.000000 qtpynodeeditor-0.2.0/qtpynodeeditor/connection_graphics_object.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     5707 2020-09-02 16:54:28.000000 qtpynodeeditor-0.2.0/qtpynodeeditor/connection_painter.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     3508 2020-09-02 16:54:28.000000 qtpynodeeditor-0.2.0/qtpynodeeditor/data_model_registry.py
--rw-r--r--   0 klauer   (1318172782) 1704612529      389 2019-03-26 20:01:33.000000 qtpynodeeditor-0.2.0/qtpynodeeditor/enums.py
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2020-09-02 18:03:52.000000 qtpynodeeditor-0.2.0/qtpynodeeditor/examples/
--rw-r--r--   0 klauer   (1318172782) 1704612529      123 2020-09-02 16:54:28.000000 qtpynodeeditor-0.2.0/qtpynodeeditor/examples/__init__.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    12553 2020-09-02 16:54:28.000000 qtpynodeeditor-0.2.0/qtpynodeeditor/examples/calculator.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     2168 2020-09-02 16:54:28.000000 qtpynodeeditor-0.2.0/qtpynodeeditor/examples/connection_colors.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     2537 2020-06-16 16:29:34.000000 qtpynodeeditor-0.2.0/qtpynodeeditor/examples/dynamic_ports.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     4687 2020-09-02 16:54:28.000000 qtpynodeeditor-0.2.0/qtpynodeeditor/examples/image.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     2314 2020-06-16 16:52:29.000000 qtpynodeeditor-0.2.0/qtpynodeeditor/examples/semi_dynamic_ports.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     2422 2020-09-02 16:54:28.000000 qtpynodeeditor-0.2.0/qtpynodeeditor/examples/style.py
--rw-r--r--   0 klauer   (1318172782) 1704612529      883 2020-09-02 16:54:28.000000 qtpynodeeditor-0.2.0/qtpynodeeditor/exceptions.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    20110 2020-09-02 16:54:28.000000 qtpynodeeditor-0.2.0/qtpynodeeditor/flow_scene.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    11015 2020-09-02 16:54:28.000000 qtpynodeeditor-0.2.0/qtpynodeeditor/flow_view.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     9660 2020-09-02 16:54:28.000000 qtpynodeeditor-0.2.0/qtpynodeeditor/node.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     9351 2020-09-02 16:54:28.000000 qtpynodeeditor-0.2.0/qtpynodeeditor/node_connection_interaction.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    10267 2020-09-02 16:54:28.000000 qtpynodeeditor-0.2.0/qtpynodeeditor/node_data.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    13038 2020-09-02 16:54:28.000000 qtpynodeeditor-0.2.0/qtpynodeeditor/node_geometry.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    10686 2020-09-02 16:54:28.000000 qtpynodeeditor-0.2.0/qtpynodeeditor/node_graphics_object.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    11535 2020-09-02 16:54:28.000000 qtpynodeeditor-0.2.0/qtpynodeeditor/node_painter.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     4369 2020-09-02 16:54:28.000000 qtpynodeeditor-0.2.0/qtpynodeeditor/node_state.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     4031 2020-09-02 16:54:28.000000 qtpynodeeditor-0.2.0/qtpynodeeditor/port.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     8114 2020-09-02 16:54:28.000000 qtpynodeeditor-0.2.0/qtpynodeeditor/style.py
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2020-09-02 18:03:52.000000 qtpynodeeditor-0.2.0/qtpynodeeditor/tests/
--rw-r--r--   0 klauer   (1318172782) 1704612529        0 2019-03-26 20:01:33.000000 qtpynodeeditor-0.2.0/qtpynodeeditor/tests/__init__.py
--rw-r--r--   0 klauer   (1318172782) 1704612529       68 2020-09-02 16:54:28.000000 qtpynodeeditor-0.2.0/qtpynodeeditor/tests/conftest.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    12248 2020-09-02 16:54:28.000000 qtpynodeeditor-0.2.0/qtpynodeeditor/tests/test_basic.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     2783 2020-09-02 16:54:28.000000 qtpynodeeditor-0.2.0/qtpynodeeditor/tests/test_examples.py
--rw-r--r--   0 klauer   (1318172782) 1704612529      522 2019-03-26 20:01:33.000000 qtpynodeeditor-0.2.0/qtpynodeeditor/type_converter.py
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2020-09-02 18:03:52.000000 qtpynodeeditor-0.2.0/qtpynodeeditor.egg-info/
--rw-r--r--   0 klauer   (1318172782) 1704612529     2518 2020-09-02 18:03:52.000000 qtpynodeeditor-0.2.0/qtpynodeeditor.egg-info/PKG-INFO
--rw-r--r--   0 klauer   (1318172782) 1704612529     1638 2020-09-02 18:03:52.000000 qtpynodeeditor-0.2.0/qtpynodeeditor.egg-info/SOURCES.txt
--rw-r--r--   0 klauer   (1318172782) 1704612529        1 2020-09-02 18:03:52.000000 qtpynodeeditor-0.2.0/qtpynodeeditor.egg-info/dependency_links.txt
--rw-r--r--   0 klauer   (1318172782) 1704612529       20 2020-09-02 18:03:52.000000 qtpynodeeditor-0.2.0/qtpynodeeditor.egg-info/entry_points.txt
--rw-r--r--   0 klauer   (1318172782) 1704612529       25 2020-09-02 18:03:52.000000 qtpynodeeditor-0.2.0/qtpynodeeditor.egg-info/requires.txt
--rw-r--r--   0 klauer   (1318172782) 1704612529       15 2020-09-02 18:03:52.000000 qtpynodeeditor-0.2.0/qtpynodeeditor.egg-info/top_level.txt
--rw-r--r--   0 klauer   (1318172782) 1704612529       25 2019-03-26 20:01:33.000000 qtpynodeeditor-0.2.0/requirements.txt
--rw-r--r--   0 klauer   (1318172782) 1704612529      187 2020-09-02 18:03:52.000000 qtpynodeeditor-0.2.0/setup.cfg
--rw-r--r--   0 klauer   (1318172782) 1704612529     1851 2020-09-02 16:54:28.000000 qtpynodeeditor-0.2.0/setup.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    68611 2019-08-06 11:53:59.000000 qtpynodeeditor-0.2.0/versioneer.py
+drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2023-07-21 17:29:49.464068 qtpynodeeditor-0.3.0/
+-rw-r--r--   0 klauer   (1318172782) 1704612529      177 2023-07-21 17:29:17.000000 qtpynodeeditor-0.3.0/.codecov.yml
+-rw-r--r--   0 klauer   (1318172782) 1704612529      148 2022-06-03 18:45:57.000000 qtpynodeeditor-0.3.0/.coveragerc
+-rw-r--r--   0 klauer   (1318172782) 1704612529      982 2023-07-21 17:29:17.000000 qtpynodeeditor-0.3.0/.flake8
+-rw-r--r--   0 klauer   (1318172782) 1704612529      125 2023-07-21 17:29:17.000000 qtpynodeeditor-0.3.0/.git_archival.txt
+-rw-r--r--   0 klauer   (1318172782) 1704612529       32 2023-07-21 17:29:17.000000 qtpynodeeditor-0.3.0/.gitattributes
+drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2023-07-21 17:29:49.410627 qtpynodeeditor-0.3.0/.github/
+-rw-r--r--   0 klauer   (1318172782) 1704612529     1068 2022-06-03 18:45:57.000000 qtpynodeeditor-0.3.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 klauer   (1318172782) 1704612529      751 2022-06-03 18:45:57.000000 qtpynodeeditor-0.3.0/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2023-07-21 17:29:49.412264 qtpynodeeditor-0.3.0/.github/workflows/
+-rw-r--r--   0 klauer   (1318172782) 1704612529     1921 2023-07-21 17:29:17.000000 qtpynodeeditor-0.3.0/.github/workflows/pcds.yml
+-rw-r--r--   0 klauer   (1318172782) 1704612529      892 2022-06-03 18:45:57.000000 qtpynodeeditor-0.3.0/.gitignore
+-rw-r--r--   0 klauer   (1318172782) 1704612529      793 2023-07-21 17:29:17.000000 qtpynodeeditor-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 klauer   (1318172782) 1704612529    17502 2023-07-21 17:29:17.000000 qtpynodeeditor-0.3.0/.pylintrc
+-rw-r--r--   0 klauer   (1318172782) 1704612529      130 2022-06-03 18:45:57.000000 qtpynodeeditor-0.3.0/AUTHORS.rst
+-rw-r--r--   0 klauer   (1318172782) 1704612529     3075 2023-07-21 17:29:17.000000 qtpynodeeditor-0.3.0/CONTRIBUTING.rst
+-rw-r--r--   0 klauer   (1318172782) 1704612529     1641 2022-06-03 18:45:57.000000 qtpynodeeditor-0.3.0/LICENSE
+-rw-r--r--   0 klauer   (1318172782) 1704612529      351 2022-06-03 18:45:57.000000 qtpynodeeditor-0.3.0/MANIFEST.in
+-rw-r--r--   0 klauer   (1318172782) 1704612529     3912 2023-07-21 17:29:49.463323 qtpynodeeditor-0.3.0/PKG-INFO
+-rw-r--r--   0 klauer   (1318172782) 1704612529     1620 2022-06-03 18:45:57.000000 qtpynodeeditor-0.3.0/README.rst
+drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2023-07-21 17:29:49.412941 qtpynodeeditor-0.3.0/conda-recipe/
+-rw-r--r--   0 klauer   (1318172782) 1704612529      697 2023-07-21 17:29:17.000000 qtpynodeeditor-0.3.0/conda-recipe/meta.yaml
+-rw-r--r--   0 klauer   (1318172782) 1704612529      192 2023-07-21 17:29:17.000000 qtpynodeeditor-0.3.0/dev-requirements.txt
+drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2023-07-21 17:29:49.414830 qtpynodeeditor-0.3.0/docs/
+-rw-r--r--   0 klauer   (1318172782) 1704612529      616 2022-06-03 18:45:57.000000 qtpynodeeditor-0.3.0/docs/Makefile
+-rw-r--r--   0 klauer   (1318172782) 1704612529      786 2022-06-03 18:45:57.000000 qtpynodeeditor-0.3.0/docs/make.bat
+drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2023-07-21 17:29:49.418547 qtpynodeeditor-0.3.0/docs/source/
+-rw-r--r--   0 klauer   (1318172782) 1704612529     2546 2022-06-03 18:45:57.000000 qtpynodeeditor-0.3.0/docs/source/api.rst
+-rw-r--r--   0 klauer   (1318172782) 1704612529     5394 2023-07-21 17:29:17.000000 qtpynodeeditor-0.3.0/docs/source/conf.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529     1506 2022-06-03 18:45:57.000000 qtpynodeeditor-0.3.0/docs/source/getting_started.rst
+-rw-r--r--   0 klauer   (1318172782) 1704612529      494 2022-06-03 18:45:57.000000 qtpynodeeditor-0.3.0/docs/source/index.rst
+-rw-r--r--   0 klauer   (1318172782) 1704612529     1846 2022-06-03 18:45:57.000000 qtpynodeeditor-0.3.0/docs/source/release_notes.rst
+-rw-r--r--   0 klauer   (1318172782) 1704612529       70 2023-07-21 17:29:17.000000 qtpynodeeditor-0.3.0/docs-requirements.txt
+-rw-r--r--   0 klauer   (1318172782) 1704612529     1041 2023-07-21 17:29:17.000000 qtpynodeeditor-0.3.0/pyproject.toml
+drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2023-07-21 17:29:49.447776 qtpynodeeditor-0.3.0/qtpynodeeditor/
+-rw-r--r--   0 klauer   (1318172782) 1704612529     1047 2022-06-03 18:45:57.000000 qtpynodeeditor-0.3.0/qtpynodeeditor/DefaultStyle.json
+-rw-r--r--   0 klauer   (1318172782) 1704612529     2208 2023-07-21 17:29:17.000000 qtpynodeeditor-0.3.0/qtpynodeeditor/__init__.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529      160 2023-07-21 17:29:49.000000 qtpynodeeditor-0.3.0/qtpynodeeditor/_version.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529      342 2023-07-21 17:29:17.000000 qtpynodeeditor-0.3.0/qtpynodeeditor/base.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529    11452 2023-07-21 17:29:17.000000 qtpynodeeditor-0.3.0/qtpynodeeditor/connection.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529     3849 2022-06-03 18:45:57.000000 qtpynodeeditor-0.3.0/qtpynodeeditor/connection_geometry.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529     6900 2023-07-21 17:29:17.000000 qtpynodeeditor-0.3.0/qtpynodeeditor/connection_graphics_object.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529     5726 2023-07-21 17:29:17.000000 qtpynodeeditor-0.3.0/qtpynodeeditor/connection_painter.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529     3830 2023-07-21 17:29:17.000000 qtpynodeeditor-0.3.0/qtpynodeeditor/data_model_registry.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529      389 2022-06-03 18:45:57.000000 qtpynodeeditor-0.3.0/qtpynodeeditor/enums.py
+drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2023-07-21 17:29:49.457621 qtpynodeeditor-0.3.0/qtpynodeeditor/examples/
+-rw-r--r--   0 klauer   (1318172782) 1704612529      123 2022-06-03 18:45:57.000000 qtpynodeeditor-0.3.0/qtpynodeeditor/examples/__init__.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529    12553 2023-07-21 17:29:17.000000 qtpynodeeditor-0.3.0/qtpynodeeditor/examples/calculator.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529     2168 2022-06-03 18:45:57.000000 qtpynodeeditor-0.3.0/qtpynodeeditor/examples/connection_colors.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529     4727 2023-07-21 17:29:17.000000 qtpynodeeditor-0.3.0/qtpynodeeditor/examples/image.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529     2422 2022-06-03 18:45:57.000000 qtpynodeeditor-0.3.0/qtpynodeeditor/examples/style.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529      883 2022-06-03 18:45:57.000000 qtpynodeeditor-0.3.0/qtpynodeeditor/exceptions.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529    20354 2023-07-21 17:29:17.000000 qtpynodeeditor-0.3.0/qtpynodeeditor/flow_scene.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529    11015 2023-07-21 17:29:17.000000 qtpynodeeditor-0.3.0/qtpynodeeditor/flow_view.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529    10118 2023-07-21 17:29:17.000000 qtpynodeeditor-0.3.0/qtpynodeeditor/node.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529     9659 2023-07-21 17:29:17.000000 qtpynodeeditor-0.3.0/qtpynodeeditor/node_connection_interaction.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529    10309 2023-07-21 17:29:17.000000 qtpynodeeditor-0.3.0/qtpynodeeditor/node_data.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529    13148 2023-07-21 17:29:17.000000 qtpynodeeditor-0.3.0/qtpynodeeditor/node_geometry.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529    10721 2023-07-21 17:29:17.000000 qtpynodeeditor-0.3.0/qtpynodeeditor/node_graphics_object.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529    11769 2023-07-21 17:29:17.000000 qtpynodeeditor-0.3.0/qtpynodeeditor/node_painter.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529     4421 2023-07-21 17:29:17.000000 qtpynodeeditor-0.3.0/qtpynodeeditor/node_state.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529     4423 2023-07-21 17:29:17.000000 qtpynodeeditor-0.3.0/qtpynodeeditor/port.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529     8114 2022-06-03 18:45:57.000000 qtpynodeeditor-0.3.0/qtpynodeeditor/style.py
+drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2023-07-21 17:29:49.462066 qtpynodeeditor-0.3.0/qtpynodeeditor/tests/
+-rw-r--r--   0 klauer   (1318172782) 1704612529        0 2022-06-03 18:45:57.000000 qtpynodeeditor-0.3.0/qtpynodeeditor/tests/__init__.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529       68 2022-06-03 18:45:57.000000 qtpynodeeditor-0.3.0/qtpynodeeditor/tests/conftest.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529    12248 2022-06-03 18:45:57.000000 qtpynodeeditor-0.3.0/qtpynodeeditor/tests/test_basic.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529     2803 2023-07-21 17:29:17.000000 qtpynodeeditor-0.3.0/qtpynodeeditor/tests/test_examples.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529      522 2022-06-03 18:45:57.000000 qtpynodeeditor-0.3.0/qtpynodeeditor/type_converter.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529     1898 2023-07-21 17:29:17.000000 qtpynodeeditor-0.3.0/qtpynodeeditor/version.py
+drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2023-07-21 17:29:49.452876 qtpynodeeditor-0.3.0/qtpynodeeditor.egg-info/
+-rw-r--r--   0 klauer   (1318172782) 1704612529     3912 2023-07-21 17:29:49.000000 qtpynodeeditor-0.3.0/qtpynodeeditor.egg-info/PKG-INFO
+-rw-r--r--   0 klauer   (1318172782) 1704612529     1760 2023-07-21 17:29:49.000000 qtpynodeeditor-0.3.0/qtpynodeeditor.egg-info/SOURCES.txt
+-rw-r--r--   0 klauer   (1318172782) 1704612529        1 2023-07-21 17:29:49.000000 qtpynodeeditor-0.3.0/qtpynodeeditor.egg-info/dependency_links.txt
+-rw-r--r--   0 klauer   (1318172782) 1704612529      156 2023-07-21 17:29:49.000000 qtpynodeeditor-0.3.0/qtpynodeeditor.egg-info/requires.txt
+-rw-r--r--   0 klauer   (1318172782) 1704612529       15 2023-07-21 17:29:49.000000 qtpynodeeditor-0.3.0/qtpynodeeditor.egg-info/top_level.txt
+-rw-r--r--   0 klauer   (1318172782) 1704612529       22 2023-07-21 17:29:17.000000 qtpynodeeditor-0.3.0/requirements.txt
+-rw-r--r--   0 klauer   (1318172782) 1704612529       38 2023-07-21 17:29:49.464299 qtpynodeeditor-0.3.0/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `qtpynodeeditor-0.2.0/CONTRIBUTING.rst` & `qtpynodeeditor-0.3.0/CONTRIBUTING.rst`

 * *Files 0% similar despite different names*

```diff
@@ -97,8 +97,7 @@
 1. The pull request should include tests.
 2. If the pull request adds functionality, the docs should be updated. Put your
    new functionality into a function with a docstring, and add the feature to
    the list in README.rst.
 3. The pull request should work for Python 3.6 and up. Check
    https://travis-ci.org/klauer/qtpynodeeditor/pull_requests
    and make sure that the tests pass for all supported Python versions.
-
```

### Comparing `qtpynodeeditor-0.2.0/LICENSE` & `qtpynodeeditor-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qtpynodeeditor-0.2.0/PKG-INFO` & `qtpynodeeditor-0.3.0/README.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,80 +1,67 @@
-Metadata-Version: 1.1
-Name: qtpynodeeditor
-Version: 0.2.0
-Summary: Python Qt node editor
-Home-page: https://github.com/klauer/qtpynodeeditor
-Author: Ken Lauer
-Author-email: UNKNOWN
-License: BSD
-Description: .. image:: https://img.shields.io/travis/klauer/qtpynodeeditor.svg
-                :target: https://travis-ci.org/klauer/qtpynodeeditor
-        
-        .. image:: https://img.shields.io/pypi/v/qtpynodeeditor.svg
-                :target: https://pypi.python.org/pypi/qtpynodeeditor
-        
-        ===============================
-        qtpynodeeditor
-        ===============================
-        
-        Python Qt node editor
-        
-        Pure Python port of `NodeEditor <https://github.com/paceholder/nodeeditor>`_,
-        supporting PyQt5 and PySide through `qtpy <https://github.com/spyder-ide/qtpy>`_.
-        
-        Requirements
-        ------------
-        
-        * Python 3.6+
-        * qtpy
-        * PyQt5 / PySide
-        
-        
-        Documentation
-        -------------
-        
-        `Sphinx-generated documentation <https://klauer.github.io/qtpynodeeditor/>`_
-        
-        
-        Screenshots
-        -----------
-        
-        `Style example <https://github.com/klauer/qtpynodeeditor/blob/master/qtpynodeeditor/examples/style.py>`_
-        
-        .. image:: https://raw.githubusercontent.com/klauer/qtpynodeeditor/assets/screenshots/style.png
-        
-        `Calculator example <https://github.com/klauer/qtpynodeeditor/blob/master/qtpynodeeditor/examples/calculator.py>`_
-        
-        .. image:: https://raw.githubusercontent.com/klauer/qtpynodeeditor/assets/screenshots/calculator.png
-        
-        
-        Installation
-        ------------
-        
-        We recommend using conda to install qtpynodeeditor.
-        
-        ::
-        
-           $ conda create -n my_new_environment -c conda-forge python=3.7 qtpynodeeditor
-           $ conda activate my_new_environment
-        
-        qtpynodeeditor may also be installed using pip from PyPI.
-        
-        ::
-        
-            $ python -m pip install qtpynodeeditor pyqt5
-        
-        
-        Running the Tests
-        -----------------
-        
-        Tests must be run with pytest and pytest-qt.
-        
-        ::
-        
-           $ pip install -r dev-requirements.txt
-           $ pytest -v qtpynodeeditor/tests
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
+.. image:: https://img.shields.io/travis/klauer/qtpynodeeditor.svg
+        :target: https://travis-ci.org/klauer/qtpynodeeditor
+
+.. image:: https://img.shields.io/pypi/v/qtpynodeeditor.svg
+        :target: https://pypi.python.org/pypi/qtpynodeeditor
+
+===============================
+qtpynodeeditor
+===============================
+
+Python Qt node editor
+
+Pure Python port of `NodeEditor <https://github.com/paceholder/nodeeditor>`_,
+supporting PyQt5 and PySide through `qtpy <https://github.com/spyder-ide/qtpy>`_.
+
+Requirements
+------------
+
+* Python 3.6+
+* qtpy
+* PyQt5 / PySide
+
+
+Documentation
+-------------
+
+`Sphinx-generated documentation <https://klauer.github.io/qtpynodeeditor/>`_
+
+
+Screenshots
+-----------
+
+`Style example <https://github.com/klauer/qtpynodeeditor/blob/master/qtpynodeeditor/examples/style.py>`_
+
+.. image:: https://raw.githubusercontent.com/klauer/qtpynodeeditor/assets/screenshots/style.png
+
+`Calculator example <https://github.com/klauer/qtpynodeeditor/blob/master/qtpynodeeditor/examples/calculator.py>`_
+
+.. image:: https://raw.githubusercontent.com/klauer/qtpynodeeditor/assets/screenshots/calculator.png
+
+
+Installation
+------------
+
+We recommend using conda to install qtpynodeeditor.
+
+::
+
+   $ conda create -n my_new_environment -c conda-forge python=3.7 qtpynodeeditor
+   $ conda activate my_new_environment
+
+qtpynodeeditor may also be installed using pip from PyPI.
+
+::
+
+    $ python -m pip install qtpynodeeditor pyqt5
+
+
+Running the Tests
+-----------------
+
+Tests must be run with pytest and pytest-qt.
+
+::
+
+   $ pip install -r dev-requirements.txt
+   $ pytest -v qtpynodeeditor/tests
```

### Comparing `qtpynodeeditor-0.2.0/README.rst` & `qtpynodeeditor-0.3.0/docs/source/getting_started.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-.. image:: https://img.shields.io/travis/klauer/qtpynodeeditor.svg
-        :target: https://travis-ci.org/klauer/qtpynodeeditor
-
-.. image:: https://img.shields.io/pypi/v/qtpynodeeditor.svg
-        :target: https://pypi.python.org/pypi/qtpynodeeditor
-
-===============================
-qtpynodeeditor
-===============================
-
-Python Qt node editor
-
-Pure Python port of `NodeEditor <https://github.com/paceholder/nodeeditor>`_,
-supporting PyQt5 and PySide through `qtpy <https://github.com/spyder-ide/qtpy>`_.
+Getting Started
+===============
 
 Requirements
 ------------
 
 * Python 3.6+
 * qtpy
 * PyQt5 / PySide
 
 
-Documentation
--------------
+Installation
+------------
 
-`Sphinx-generated documentation <https://klauer.github.io/qtpynodeeditor/>`_
+We recommend using conda to install qtpynodeeditor.
 
+::
 
-Screenshots
------------
+   $ conda create -n my_new_environment -c conda-forge python=3.7 qtpynodeeditor
+   $ conda activate my_new_environment
 
-`Style example <https://github.com/klauer/qtpynodeeditor/blob/master/qtpynodeeditor/examples/style.py>`_
+qtpynodeeditor may also be installed using pip from PyPI.
 
-.. image:: https://raw.githubusercontent.com/klauer/qtpynodeeditor/assets/screenshots/style.png
+::
 
-`Calculator example <https://github.com/klauer/qtpynodeeditor/blob/master/qtpynodeeditor/examples/calculator.py>`_
+    $ python -m pip install qtpynodeeditor pyqt5
 
-.. image:: https://raw.githubusercontent.com/klauer/qtpynodeeditor/assets/screenshots/calculator.png
 
+Examples
+--------
 
-Installation
-------------
+1. `Connection colors <https://github.com/klauer/qtpynodeeditor/blob/master/qtpynodeeditor/examples/connection_colors.py>`_
 
-We recommend using conda to install qtpynodeeditor.
+::
+
+    $ python -m qtpynodeeditor.examples.connection_colors
+
+
+.. image:: https://raw.githubusercontent.com/klauer/qtpynodeeditor/assets/screenshots/connection_colors.png
+
+2. `Image <https://github.com/klauer/qtpynodeeditor/blob/master/qtpynodeeditor/examples/image.py>`_
 
 ::
 
-   $ conda create -n my_new_environment -c conda-forge python=3.7 qtpynodeeditor
-   $ conda activate my_new_environment
+    $ python -m qtpynodeeditor.examples.image
 
-qtpynodeeditor may also be installed using pip from PyPI.
+.. image:: https://raw.githubusercontent.com/klauer/qtpynodeeditor/assets/screenshots/image.png
+
+
+3. `Style <https://github.com/klauer/qtpynodeeditor/blob/master/qtpynodeeditor/examples/style.py>`_
 
 ::
 
-    $ python -m pip install qtpynodeeditor pyqt5
+    $ python -m qtpynodeeditor.examples.style
+
+
+.. image:: https://raw.githubusercontent.com/klauer/qtpynodeeditor/assets/screenshots/style.png
 
 
-Running the Tests
------------------
 
-Tests must be run with pytest and pytest-qt.
+4. `Calculator <https://github.com/klauer/qtpynodeeditor/blob/master/qtpynodeeditor/examples/calculator.py>`_
 
 ::
 
-   $ pip install -r dev-requirements.txt
-   $ pytest -v qtpynodeeditor/tests
+    $ python -m qtpynodeeditor.examples.calculator
+
+.. image:: https://raw.githubusercontent.com/klauer/qtpynodeeditor/assets/screenshots/calculator.png
```

### Comparing `qtpynodeeditor-0.2.0/docs/Makefile` & `qtpynodeeditor-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `qtpynodeeditor-0.2.0/docs/make.bat` & `qtpynodeeditor-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `qtpynodeeditor-0.2.0/docs/source/api.rst` & `qtpynodeeditor-0.3.0/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `qtpynodeeditor-0.2.0/docs/source/conf.py` & `qtpynodeeditor-0.3.0/docs/source/conf.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Configuration file for the Sphinx documentation builder.
 #
 # This file does only contain a selection of the most common options. For a
 # full list see the documentation:
 # http://www.sphinx-doc.org/en/master/config
 
@@ -11,98 +10,97 @@
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 import os
 import sys
 
-import sphinx_rtd_theme
-
-module_path = os.path.join(os.path.dirname(os.path.abspath(__file__)),'../../')
-sys.path.insert(0,module_path)
+module_path = os.path.join(os.path.dirname(os.path.abspath(__file__)), "../../")
+sys.path.insert(0, module_path)
 
 # -- Project information -----------------------------------------------------
 
-project = 'qtpynodeeditor'
-copyright = '2019, Ken Lauer'
-author = 'Ken Lauer'
+project = "qtpynodeeditor"
+copyright = "2019, Ken Lauer"
+author = "Ken Lauer"
 
 # The short X.Y version
-version = ''
+version = ""
 # The full version, including alpha/beta/rc tags
-release = ''
+release = ""
 
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
-    'sphinx.ext.autodoc',
-    'sphinx.ext.todo',
-    'sphinx.ext.coverage',
-    'sphinx.ext.mathjax',
-    'sphinx.ext.viewcode',
-    'sphinx.ext.githubpages',
-    'numpydoc',
+    "sphinxcontrib.jquery",
+    "sphinx.ext.autodoc",
+    "sphinx.ext.todo",
+    "sphinx.ext.coverage",
+    "sphinx.ext.mathjax",
+    "sphinx.ext.viewcode",
+    "sphinx.ext.githubpages",
+    "numpydoc",
 ]
 
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
+templates_path = ["_templates"]
 
 autosummary_generate = True
 numpydoc_show_class_members = False
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 #
 # source_suffix = ['.rst', '.md']
-source_suffix = '.rst'
+source_suffix = ".rst"
 
 # The master toctree document.
-master_doc = 'index'
+master_doc = "index"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = "en"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path .
 exclude_patterns = []
 
 # The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
+pygments_style = "sphinx"
 
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = 'sphinx_rtd_theme'
+html_theme = "sphinx_rtd_theme"
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 #
 # html_theme_options = {}
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ['_static']
+html_static_path = ["_static"]
 
 # Custom sidebar templates, must be a dictionary that maps document names
 # to template names.
 #
 # The default sidebars (for documents that don't match any pattern) are
 # defined by theme itself.  Builtin themes are using these templates by
 # default: ``['localtoc.html', 'relations.html', 'sourcelink.html',
@@ -110,65 +108,72 @@
 #
 # html_sidebars = {}
 
 
 # -- Options for HTMLHelp output ---------------------------------------------
 
 # Output file base name for HTML help builder.
-htmlhelp_basename = 'qtpynodeeditor'
+htmlhelp_basename = "qtpynodeeditor"
 
 
 # -- Options for LaTeX output ------------------------------------------------
 
 latex_elements = {
     # The paper size ('letterpaper' or 'a4paper').
     #
     # 'papersize': 'letterpaper',
-
     # The font size ('10pt', '11pt' or '12pt').
     #
     # 'pointsize': '10pt',
-
     # Additional stuff for the LaTeX preamble.
     #
     # 'preamble': '',
-
     # Latex figure (float) alignment
     #
     # 'figure_align': 'htbp',
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title,
 #  author, documentclass [howto, manual, or own class]).
 latex_documents = [
-    (master_doc, 'qtpynodeeditor.tex', 'qtpynodeeditor Documentation',
-     'Ken Lauer', 'manual'),
+    (
+        master_doc,
+        "qtpynodeeditor.tex",
+        "qtpynodeeditor Documentation",
+        "Ken Lauer",
+        "manual",
+    ),
 ]
 
 
 # -- Options for manual page output ------------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
 man_pages = [
-    (master_doc, 'qtpynodeeditor', 'qtpynodeeditor Documentation',
-     [author], 1)
+    (master_doc, "qtpynodeeditor", "qtpynodeeditor Documentation", [author], 1)
 ]
 
 
 # -- Options for Texinfo output ----------------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
-    (master_doc, 'qtpynodeeditor', 'qtpynodeeditor Documentation',
-     author, 'qtpynodeeditor', 'Python Qt Node Editor',
-     'Miscellaneous'),
+    (
+        master_doc,
+        "qtpynodeeditor",
+        "qtpynodeeditor Documentation",
+        author,
+        "qtpynodeeditor",
+        "Python Qt Node Editor",
+        "Miscellaneous",
+    ),
 ]
 
 
 # -- Extension configuration -------------------------------------------------
 
 # -- Options for todo extension ----------------------------------------------
```

### Comparing `qtpynodeeditor-0.2.0/docs/source/release_notes.rst` & `qtpynodeeditor-0.3.0/docs/source/release_notes.rst`

 * *Files identical despite different names*

### Comparing `qtpynodeeditor-0.2.0/qtpynodeeditor/DefaultStyle.json` & `qtpynodeeditor-0.3.0/qtpynodeeditor/DefaultStyle.json`

 * *Files identical despite different names*

### Comparing `qtpynodeeditor-0.2.0/qtpynodeeditor/__init__.py` & `qtpynodeeditor-0.3.0/qtpynodeeditor/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from .node_geometry import NodeGeometry
 from .node_graphics_object import NodeGraphicsObject
 from .node_painter import NodePainter, NodePainterDelegate
 from .node_state import NodeState
 from .port import Port, opposite_port
 from .style import (ConnectionStyle, FlowViewStyle, NodeStyle, Style,
                     StyleCollection)
+from .version import __version__  # noqa: F401
 
 __all__ = [
     'Connection',
     'ConnectionCycleFailure',
     'ConnectionDataTypeFailure',
     'ConnectionGeometry',
     'ConnectionGraphicsObject',
```

### Comparing `qtpynodeeditor-0.2.0/qtpynodeeditor/connection.py` & `qtpynodeeditor-0.3.0/qtpynodeeditor/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
+import typing
 import uuid
 
 from qtpy.QtCore import QObject, Signal
 
 from . import exceptions
-from .base import ConnectionBase, Serializable
+from .base import Serializable
 from .connection_geometry import ConnectionGeometry
 from .connection_graphics_object import ConnectionGraphicsObject
 from .node import Node, NodeDataType
 from .node_data import NodeData
 from .port import Port, PortType, opposite_port
 from .style import StyleCollection
 from .type_converter import TypeConverter
 
 
-class Connection(QObject, Serializable, ConnectionBase):
+class Connection(QObject, Serializable):
     connection_completed = Signal(QObject)
     connection_made_incomplete = Signal(QObject)
     updated = Signal(QObject)
 
     def __init__(self, port_a: Port, port_b: Port = None, *,
                  style: StyleCollection, converter: TypeConverter = None):
         super().__init__()
@@ -225,29 +226,28 @@
 
         Returns
         -------
         value : ConnectionGeometry
         """
         return self._connection_geometry
 
-    def get_node(self, port_type: PortType) -> Node:
+    def get_node(self, port_type: PortType) -> typing.Optional[Node]:
         """
         Get node
 
         Parameters
         ----------
         port_type : PortType
 
         Returns
         -------
         value : Node
         """
         port = self._ports[port_type]
-        if port is not None:
-            return port.node
+        return port.node if port is not None else None
 
     @property
     def nodes(self):
         # TODO namedtuple; TODO order
         return (self.get_node(PortType.input), self.get_node(PortType.output))
 
     @property
@@ -310,21 +310,21 @@
         try:
             return ports[port_type].data_type
         except KeyError:
             valid_type, = ports
             return ports[valid_type].data_type
 
     @property
-    def type_converter(self) -> TypeConverter:
+    def type_converter(self) -> typing.Optional[TypeConverter]:
         """
-        Set type converter
+        The type converter used for the connection.
 
         Returns
         -------
-        converter : TypeConverter
+        converter : TypeConverter or None
         """
         return self._converter
 
     @type_converter.setter
     def type_converter(self, converter: TypeConverter):
         self._converter = converter
```

### Comparing `qtpynodeeditor-0.2.0/qtpynodeeditor/connection_geometry.py` & `qtpynodeeditor-0.3.0/qtpynodeeditor/connection_geometry.py`

 * *Files identical despite different names*

### Comparing `qtpynodeeditor-0.2.0/qtpynodeeditor/connection_graphics_object.py` & `qtpynodeeditor-0.3.0/qtpynodeeditor/connection_graphics_object.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,24 @@
+import typing
+
 from qtpy.QtCore import QRectF
 from qtpy.QtGui import QPainter, QPainterPath
 from qtpy.QtWidgets import (QGraphicsBlurEffect, QGraphicsItem,
                             QGraphicsObject, QGraphicsSceneHoverEvent,
                             QGraphicsSceneMouseEvent, QStyleOptionGraphicsItem,
                             QWidget)
 
-from .base import ConnectionBase
 from .connection_painter import ConnectionPainter
 from .node_connection_interaction import NodeConnectionInteraction
 from .port import PortType, opposite_port
 
+if typing.TYPE_CHECKING:
+    from .connection import Connection  # noqa
+
+
 debug_drawing = False
 
 
 class ConnectionGraphicsObject(QGraphicsObject):
     def __init__(self, scene, connection):
         '''
         connection_graphics_object
@@ -40,15 +45,15 @@
 
     def _cleanup(self):
         if self._scene is not None:
             self._scene.removeItem(self)
             self._scene = None
 
     @property
-    def connection(self) -> ConnectionBase:
+    def connection(self) -> 'Connection':
         """
         Connection
 
         Returns
         -------
         value : Connection
         """
```

### Comparing `qtpynodeeditor-0.2.0/qtpynodeeditor/connection_painter.py` & `qtpynodeeditor-0.3.0/qtpynodeeditor/connection_painter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,20 @@
-from qtpy.QtCore import QLineF, QPoint, QSize, Qt
+import typing
+
+from qtpy.QtCore import QLineF, QPointF, QSize, Qt
 from qtpy.QtGui import QIcon, QPainter, QPainterPath, QPainterPathStroker, QPen
 
-from .base import ConnectionBase
 from .connection_geometry import ConnectionGeometry
 from .enums import PortType
 from .style import ConnectionStyle
 
+if typing.TYPE_CHECKING:
+    from .connection import Connection  # noqa
+
+
 use_debug_drawing = False
 
 
 def cubic_path(geom):
     source, sink = geom.source, geom.sink
     c1, c2 = geom.points_c1_c2()
 
@@ -43,15 +48,15 @@
 
 
 def draw_sketch_line(painter, connection, style):
     if not connection.requires_port:
         return
 
     p = QPen()
-    p.setWidth(style.construction_line_width)
+    p.setWidthF(style.construction_line_width)
     p.setColor(style.construction_color)
     p.setStyle(Qt.DashLine)
 
     painter.setPen(p)
     painter.setBrush(Qt.NoBrush)
 
     geom = connection.geometry
@@ -70,18 +75,16 @@
 
     # drawn as a fat background
     if hovered or selected:
         p = QPen()
 
         line_width = style.line_width
 
-        p.setWidth(2 * line_width)
-        p.setColor((style.selected_halo_color
-                    if selected
-                    else style.hovered_color))
+        p.setWidthF(2.0 * line_width)
+        p.setColor(style.selected_halo_color if selected else style.hovered_color)
 
         painter.setPen(p)
         painter.setBrush(Qt.NoBrush)
 
         # cubic spline
         cubic = cubic_path(geom)
         painter.drawPath(cubic)
@@ -110,15 +113,15 @@
 
     # geometry
     geom = connection.geometry
     line_width = style.line_width
 
     # draw normal line
     p = QPen()
-    p.setWidth(line_width)
+    p.setWidthF(line_width)
 
     graphics_object = connection.graphics_object
     selected = graphics_object.isSelected()
 
     cubic = cubic_path(geom)
     if gradient_color:
         painter.setBrush(Qt.NoBrush)
@@ -145,30 +148,30 @@
                 painter.setPen(p)
 
             painter.drawLine(cubic.pointAtPercent(ratio_prev), cubic.pointAtPercent(ratio))
 
         icon = QIcon(":convert.png")
 
         pixmap = icon.pixmap(QSize(22, 22))
-        painter.drawPixmap(cubic.pointAtPercent(0.50) - QPoint(pixmap.width() / 2, pixmap.height() / 2), pixmap)
+        painter.drawPixmap(cubic.pointAtPercent(0.50) - QPointF(pixmap.width() / 2, pixmap.height() / 2), pixmap)
     else:
         p.setColor(normal_color_out)
 
         if selected:
             p.setColor(selected_color)
 
         painter.setPen(p)
         painter.setBrush(Qt.NoBrush)
 
         painter.drawPath(cubic)
 
 
 class ConnectionPainter:
     @staticmethod
-    def paint(painter: QPainter, connection: ConnectionBase,
+    def paint(painter: QPainter, connection: 'Connection',
               style: ConnectionStyle):
         """
         Paint
 
         Parameters
         ----------
         painter : QPainter
```

### Comparing `qtpynodeeditor-0.2.0/qtpynodeeditor/data_model_registry.py` & `qtpynodeeditor-0.3.0/qtpynodeeditor/data_model_registry.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 import typing
 
-from .node_data import NodeDataModel, NodeDataType
+from .node_data import NodeData, NodeDataModel, NodeDataType
 from .type_converter import TypeConverter
 
 logger = logging.getLogger(__name__)
 
 
 class DataModelRegistry:
     def __init__(self):
@@ -16,29 +16,37 @@
 
     def register_model(self, creator, category='', *, style=None, **init_kwargs):
         name = creator.name
         self._item_creators[name] = (creator, {'style': style, **init_kwargs})
         self._categories.add(category)
         self._models_category[name] = category
 
-    def register_type_converter(self, type_in: NodeDataType, type_out:
-                                NodeDataType, type_converter: TypeConverter):
+    def register_type_converter(self,
+                                type_in: NodeDataType,
+                                type_out: NodeDataType,
+                                type_converter: TypeConverter):
         """
-        Register type converter
+        Register a type converter for a given data type.
 
         Parameters
         ----------
-        id_ : NodeData subclass or TypeConverterId
+        type_in : NodeDataType or NodeData subclass
+            The input type.
+
+        type_out : NodeDataType or NodeData subclass
+            The output type.
+
         type_converter : TypeConverter
+            The type converter to use for the conversion.
         """
         # TODO typing annotation
-        if hasattr(type_in, 'type'):
-            type_in = type_in.type
-        if hasattr(type_out, 'type'):
-            type_out = type_out.type
+        if hasattr(type_in, 'data_type'):
+            type_in = typing.cast(NodeData, type_in).data_type
+        if hasattr(type_out, 'data_type'):
+            type_out = typing.cast(NodeData, type_out).data_type
 
         self.type_converters[(type_in, type_out)] = type_converter
 
     def create(self, model_name: str) -> NodeDataModel:
         """
         Create a :class:`NodeDataModel` given its user-friendly name.
 
@@ -56,15 +64,15 @@
         ValueError
             If the model name is not registered.
         """
         cls, kwargs = self.get_model_by_name(model_name)
         return cls(**kwargs)
 
     def get_model_by_name(self, model_name: str
-                          ) -> typing.Tuple[typing.Type[NodeDataModel], dict]:
+                          ) -> tuple[type[NodeDataModel], dict]:
         """
         Get information on how to create a specific :class:`NodeDataModel`
         node given its user-friendly name.
 
         Parameters
         ----------
         model_name : str
```

### Comparing `qtpynodeeditor-0.2.0/qtpynodeeditor/examples/calculator.py` & `qtpynodeeditor-0.3.0/qtpynodeeditor/examples/calculator.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import logging
 import threading
 
 from qtpy.QtGui import QDoubleValidator
 from qtpy.QtWidgets import QApplication, QLabel, QLineEdit, QWidget
 
 import qtpynodeeditor as nodeeditor
-from qtpynodeeditor.type_converter import TypeConverter
 from qtpynodeeditor import (NodeData, NodeDataModel, NodeDataType,
                             NodeValidationState, Port, PortType)
+from qtpynodeeditor.type_converter import TypeConverter
 
 
 class DecimalData(NodeData):
     'Node data holding a decimal (floating point) number'
     data_type = NodeDataType("decimal", "Decimal")
 
     def __init__(self, number: float = 0.0):
```

### Comparing `qtpynodeeditor-0.2.0/qtpynodeeditor/examples/connection_colors.py` & `qtpynodeeditor-0.3.0/qtpynodeeditor/examples/connection_colors.py`

 * *Files identical despite different names*

### Comparing `qtpynodeeditor-0.2.0/qtpynodeeditor/examples/image.py` & `qtpynodeeditor-0.3.0/qtpynodeeditor/examples/image.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,21 +32,23 @@
         font.setItalic(True)
         self._label.setFont(font)
 
         self._label.setFixedSize(200, 200)
         self._label.installEventFilter(self)
 
     def eventFilter(self, obj, event):
-        def set_pixmap():
-            w, h = self._label.width(), self._label.height()
-            self._label.setPixmap(self._pixmap.scaled(w, h, Qt.KeepAspectRatio))
+        label = getattr(self, "_label", None)
 
-        if obj is not self._label:
+        if label is None or obj is not label:
             return False
 
+        def set_pixmap():
+            w, h = label.width(), label.height()
+            label.setPixmap(self._pixmap.scaled(w, h, Qt.KeepAspectRatio))
+
         if event.type() == QtCore.QEvent.MouseButtonPress:
             file_name, _ = QtWidgets.QFileDialog.getOpenFileName(
                 None, "Open Image", QtCore.QDir.homePath(),
                 "Image files (*.png *.jpg *.bmp)")
             try:
                 self._pixmap = QtGui.QPixmap(file_name)
             except Exception as ex:
```

### Comparing `qtpynodeeditor-0.2.0/qtpynodeeditor/examples/style.py` & `qtpynodeeditor-0.3.0/qtpynodeeditor/examples/style.py`

 * *Files identical despite different names*

### Comparing `qtpynodeeditor-0.2.0/qtpynodeeditor/exceptions.py` & `qtpynodeeditor-0.3.0/qtpynodeeditor/exceptions.py`

 * *Files identical despite different names*

### Comparing `qtpynodeeditor-0.2.0/qtpynodeeditor/flow_scene.py` & `qtpynodeeditor-0.3.0/qtpynodeeditor/flow_scene.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,27 +115,27 @@
                 "Flow Scene Files (*.flow)")
 
         if file_name:
             file_name = str(file_name)
             if not file_name.endswith(".flow"):
                 file_name += ".flow"
 
-            with open(file_name, 'wt') as f:
+            with open(file_name, 'w') as f:
                 json.dump(self.__getstate__(), f)
 
     def load(self, file_name=None):
         if file_name is None:
             file_name, _ = QFileDialog.getOpenFileName(
                 None, "Open Flow Scene", QDir.homePath(),
                 "Flow Scene Files (*.flow)")
 
         if not os.path.exists(file_name):
             return
 
-        with open(file_name, 'rt') as f:
+        with open(file_name) as f:
             doc = json.load(f)
 
         self.__setstate__(doc)
 
     def __getstate__(self) -> dict:
         """
         Save scene state to a dictionary
@@ -155,14 +155,27 @@
             connection_json = connection.__getstate__()
             if connection_json:
                 connection_json_array.append(connection_json)
 
         scene_json["connections"] = connection_json_array
         return scene_json
 
+    def restore_connection(self, connection_json: dict) -> Connection:
+        """
+        Restore a connection.  To be overridden in a subclass.
+
+        Parameters
+        ----------
+        connection_json : dict
+
+        Returns
+        -------
+        value : Connection
+        """
+
     def __setstate__(self, doc: dict):
         """
         Load scene state from a dictionary
 
         Parameters
         ----------
         doc : dict
@@ -215,16 +228,15 @@
         output_node.model.output_connection_deleted(conn)
         input_node.model.input_connection_deleted(conn)
 
     def iterate_over_nodes(self):
         """
         Generator: Iterate over nodes
         """
-        for node in self._nodes.values():
-            yield node
+        yield from self._nodes.values()
 
     def iterate_over_node_data(self):
         """
         Generator: Iterate over node data
         """
         for node in self._nodes.values():
             yield node.model
@@ -534,15 +546,15 @@
         """
         port_in = node_in[PortType.input][port_index_in]
         port_out = node_out[PortType.output][port_index_out]
         return self.create_connection(port_out, port_in, converter=converter)
 
     def restore_connection(self, connection_json: dict) -> Connection:
         """
-        Restore connection
+        Restore a connection.
 
         Parameters
         ----------
         connection_json : dict
 
         Returns
         -------
@@ -628,23 +640,23 @@
         ImportError
             If networkx is unavailable
         '''
         import networkx
         dig = self.to_digraph()
 
         layouts = {
-            name: getattr(networkx.layout, '{}_layout'.format(name))
+            name: getattr(networkx.layout, f'{name}_layout')
             for name in ('bipartite', 'circular', 'kamada_kawai', 'random',
                          'shell', 'spring', 'spectral')
         }
 
         try:
             layout_func = layouts[layout]
         except KeyError:
-            raise ValueError('Unknown layout type {}'.format(layout)) from None
+            raise ValueError(f'Unknown layout type {layout}') from None
 
         layout = layout_func(dig, **kwargs)
         for node, pos in layout.items():
             pos_x, pos_y = pos
             node.position = (pos_x * scale, pos_y * scale)
 
     def selected_nodes(self) -> list:
```

### Comparing `qtpynodeeditor-0.2.0/qtpynodeeditor/flow_view.py` & `qtpynodeeditor-0.3.0/qtpynodeeditor/flow_view.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 import math
 
 from qtpy.QtCore import QLineF, QPoint, QRectF, Qt
-from qtpy.QtGui import (QContextMenuEvent, QKeyEvent, QMouseEvent, QPainter,
-                        QPen, QShowEvent, QWheelEvent, QKeySequence)
+from qtpy.QtGui import (QContextMenuEvent, QKeyEvent, QKeySequence,
+                        QMouseEvent, QPainter, QPen, QShowEvent, QWheelEvent)
 from qtpy.QtWidgets import (QAction, QGraphicsView, QLineEdit, QMenu,
                             QTreeWidget, QTreeWidgetItem, QWidgetAction)
 
 from .connection_graphics_object import ConnectionGraphicsObject
 from .flow_scene import FlowScene
 from .node_graphics_object import NodeGraphicsObject
```

### Comparing `qtpynodeeditor-0.2.0/qtpynodeeditor/node.py` & `qtpynodeeditor-0.3.0/qtpynodeeditor/node.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 import collections
 import typing
 import uuid
+from typing import Optional
 
 from qtpy.QtCore import QObject, QPointF, QSizeF
 
-from .base import NodeBase, Serializable
+from .base import Serializable
 from .enums import ReactToConnectionState
 from .node_data import NodeData, NodeDataModel, NodeDataType
 from .node_geometry import NodeGeometry
 from .node_graphics_object import NodeGraphicsObject
 from .node_state import NodeState
 from .port import Port, PortType
 from .style import NodeStyle
 
 
-class Node(QObject, Serializable, NodeBase):
+class Node(QObject, Serializable):
+    _model: NodeDataModel
+    _uid: str
+    _style: NodeStyle
+    _state: NodeState
+    _geometry: NodeGeometry
+    _graphics_obj: Optional[NodeGraphicsObject]
+
     def __init__(self, data_model: NodeDataModel):
         '''
         A single Node in the scene
 
         Parameters
         ----------
         data_model : NodeDataModel
@@ -79,24 +87,30 @@
         """
         return any(
             path[-1] == target
             for path in self.walk_paths_by_port_type(port_type)
         )
 
     def walk_paths_by_port_type(
-            self, port_type: PortType) -> typing.Iterable['Node']:
+        self, port_type: PortType
+    ) -> typing.Generator[tuple["Node", ...], None, None]:
         """
         Yields paths to connected nodes by port type
 
         Yields
         ------
         node_path : tuple
             The path to the node
         """
-        seen = set([None])
+        seen: set[typing.Union[Node, None]]
+        pending: typing.Deque[
+            tuple[list[Node], Node]
+        ]
+
+        seen = {None}
         pending = collections.deque([([], self)])
 
         if port_type == PortType.output:
             def get_connection_nodes(state):
                 for con in state.output_connections:
                     yield con.input_node
         elif port_type == PortType.input:
@@ -130,14 +144,15 @@
         """
         Save
 
         Returns
         -------
         value : dict
         """
+        assert self._graphics_obj is not None
         return {
             "id": self._uid,
             "model": self._model.__getstate__(),
             "position": {"x": self._graphics_obj.pos().x(),
                          "y": self._graphics_obj.pos().y()}
         }
 
@@ -175,65 +190,61 @@
 
         Parameters
         ----------
         port_type : PortType
         node_data_type : NodeDataType
         scene_point : QPointF
         """
+        if self._graphics_obj is None:
+            return
+
         transform = self._graphics_obj.sceneTransform()
         inverted, invertible = transform.inverted()
         if invertible:
             pos = inverted.map(scene_point)
             self._geometry.dragging_position = pos
         self._graphics_obj.update()
         self._state.set_reaction(ReactToConnectionState.reacting,
                                  reacting_port_type, reacting_data_type)
 
     def reset_reaction_to_connection(self):
         self._state.set_reaction(ReactToConnectionState.not_reacting)
         self._graphics_obj.update()
 
     @property
-    def graphics_object(self) -> NodeGraphicsObject:
+    def graphics_object(self) -> Optional[NodeGraphicsObject]:
         """
-        Node graphics object
+        Get/set the associated node graphics object.
 
         Returns
         -------
         value : NodeGraphicsObject
         """
         return self._graphics_obj
 
     @graphics_object.setter
     def graphics_object(self, graphics: NodeGraphicsObject):
-        """
-        Set graphics object
-
-        Parameters
-        ----------
-        graphics : NodeGraphicsObject
-        """
         self._graphics_obj = graphics
         self._geometry.recalculate_size()
 
     @property
     def geometry(self) -> NodeGeometry:
         """
-        Node geometry
+        Get the node geometry.
 
         Returns
         -------
         value : NodeGeometry
         """
         return self._geometry
 
     @property
     def model(self) -> NodeDataModel:
         """
-        Node data model
+        Get the node data model.
 
         Returns
         -------
         value : NodeDataModel
         """
         return self._model
 
@@ -249,21 +260,22 @@
         if input_port.node is not self:
             raise ValueError('Port does not belong to this Node')
         elif input_port.port_type != PortType.input:
             raise ValueError('Port is not an input port')
 
         self._model.set_in_data(node_data, input_port)
 
-        # Recalculate the nodes visuals. A data change can result in the node
-        # taking more space than before, so self forces a recalculate+repaint
-        # on the affected node
-        self._graphics_obj.set_geometry_changed()
-        self._geometry.recalculate_size()
-        self._graphics_obj.update()
-        self._graphics_obj.move_connections()
+        if self._graphics_obj is not None:
+            # Recalculate the nodes visuals. A data change can result in the
+            # node taking more space than before, so self forces a
+            # recalculate+repaint on the affected node
+            self._graphics_obj.set_geometry_changed()
+            self._geometry.recalculate_size()
+            self._graphics_obj.update()
+            self._graphics_obj.move_connections()
 
     def _on_port_index_data_updated(self, port_index: int):
         """
         Data has been updated on this Node's output port port_index;
         propagate it to any connections.
 
         Parameters
@@ -322,15 +334,16 @@
         ----------
         node : Node
 
         Returns
         -------
         value : QPointF
         """
-        return self._graphics_obj.pos()
+        if self._graphics_obj is not None:
+            return self._graphics_obj.pos()
 
     @position.setter
     def position(self, pos):
         if not isinstance(pos, QPointF):
             px, py = pos
             pos = QPointF(px, py)
```

### Comparing `qtpynodeeditor-0.2.0/qtpynodeeditor/node_connection_interaction.py` & `qtpynodeeditor-0.3.0/qtpynodeeditor/node_connection_interaction.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,34 @@
 import logging
+import typing
+from typing import Optional
 
 from qtpy.QtCore import QPointF
 
-from .base import ConnectionBase, FlowSceneBase, NodeBase
-from .exceptions import (ConnectionCycleFailure, ConnectionPointFailure,
-                         ConnectionPortNotEmptyFailure,
+from .exceptions import (ConnectionCycleFailure, ConnectionDataTypeFailure,
+                         ConnectionPointFailure, ConnectionPortNotEmptyFailure,
                          ConnectionRequiresPortFailure, ConnectionSelfFailure,
-                         ConnectionDataTypeFailure, NodeConnectionFailure)
+                         NodeConnectionFailure)
 from .port import PortType, opposite_port
+from .type_converter import TypeConverter
+
+if typing.TYPE_CHECKING:
+    from .connection import Connection  # noqa
+    from .flow_scene import FlowScene  # noqa
+    from .node import Node  # noqa
+    from .port import Port  # noqa
+
 
 logger = logging.getLogger(__name__)
 
 
 class NodeConnectionInteraction:
-    def __init__(self, node: NodeBase, connection: ConnectionBase, scene: FlowSceneBase):
+    def __init__(self, node: 'Node',
+                 connection: 'Connection',
+                 scene: 'FlowScene'):
         '''
         An interactive connection interaction to complete `connection` with the
         given node
 
         Parameters
         ----------
         node : Node
@@ -31,15 +42,15 @@
     @property
     def creates_cycle(self):
         """Would completing the connection introduce a cycle?"""
         required_port = self.connection_required_port
         return self.connection_node.has_connection_by_port_type(
             self._node, required_port)
 
-    def can_connect(self) -> bool:
+    def can_connect(self) -> tuple['Port', Optional[TypeConverter]]:
         """
         Can connect when following conditions are met:
             1) Connection 'requires' a port - i.e., is missing either a start
                node or an end node
             2) Connection's vacant end is above the node port in the user
                interface
             3) Node port is vacant
@@ -48,16 +59,19 @@
                type conversion that can translate between the two
 
         Parameters
         ----------
 
         Returns
         -------
-        (port_index, converter) : (int, TypeConverter)
-            where port_index is the index of the port to be connected
+        port : Port
+            The port to be connected.
+
+        converter : TypeConverter
+            The data type converter to use.
 
         Raises
         ------
         NodeConnectionFailure
         ConnectionDataTypeFailure
             If port data types are not compatible
         """
@@ -158,28 +172,24 @@
         # 5) Poke model to intiate data transfer
         _, out_port = self._connection.ports
         if out_port:
             out_port.node.on_data_updated(out_port)
 
         return True
 
-    def disconnect(self, port_to_disconnect: PortType) -> bool:
+    def disconnect(self, port_to_disconnect: PortType):
         """
         1) Node and Connection should be already connected
         2) If so, clear Connection entry in the NodeState
         3) Propagate invalid data to IN node
         4) Set Connection end to 'requiring a port'
 
         Parameters
         ----------
         port_to_disconnect : PortType
-
-        Returns
-        -------
-        value : bool
         """
         port_index = self._connection.get_port_index(port_to_disconnect)
         state = self._node.state
 
         # clear pointer to Connection in the NodeState
         state.erase_connection(port_to_disconnect, port_index,
                                self._connection)
@@ -239,26 +249,28 @@
         -------
         value : QPointF
         """
         port = self._node.state[port_type][port_index]
         return port.get_mapped_scene_position(
             self._node.graphics_object.sceneTransform())
 
-    def node_port_under_scene_point(self, port_type: PortType, scene_point: QPointF) -> NodeBase:
+    def node_port_under_scene_point(self,
+                                    port_type: PortType,
+                                    scene_point: QPointF) -> Optional['Port']:
         """
         Node port under scene point
 
         Parameters
         ----------
         port_type : PortType
         p : QPointF
 
         Returns
         -------
-        value : int
+        port : Port
         """
         node_geom = self._node.geometry
         scene_transform = self._node.graphics_object.sceneTransform()
         return node_geom.check_hit_scene_point(port_type, scene_point, scene_transform)
 
     def node_port_is_empty(self, port_type: PortType, port_index: int) -> bool:
         """
```

### Comparing `qtpynodeeditor-0.2.0/qtpynodeeditor/node_data.py` & `qtpynodeeditor-0.3.0/qtpynodeeditor/node_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import inspect
 from collections import namedtuple
+from typing import Optional
 
 from qtpy.QtCore import QObject, Signal
 from qtpy.QtWidgets import QWidget
 
 from . import style as style_module
 from .base import Serializable
 from .enums import ConnectionPolicy, NodeValidationState, PortType
@@ -38,16 +39,16 @@
         -------
         value : bool
         """
         return self.data_type.id == other.data_type.id
 
 
 class NodeDataModel(QObject, Serializable):
-    name = None
-    caption = None
+    name: Optional[str] = None
+    caption: Optional[str] = None
     caption_visible = True
     num_ports = {PortType.input: 1,
                  PortType.output: 1,
                  }
 
     # data_updated and data_invalidated refer to the port index that has
     # changed:
@@ -140,15 +141,15 @@
 
         def fill_defaults(attr, default, valid_type=None):
             if isinstance(getattr(cls, attr, None), dict):
                 return
 
             default = get_default(attr, default, valid_type)
             if default is None:
-                raise ValueError('Cannot leave {} unspecified'.format(attr))
+                raise ValueError(f'Cannot leave {attr} unspecified')
 
             setattr(cls, attr, new_dict(default))
 
         fill_defaults('port_caption', '')
         fill_defaults('port_caption_visible', False)
         fill_defaults('data_type', None, valid_type=NodeDataType)
 
@@ -175,15 +176,15 @@
 
                 for i in range(num_ports[port_type]):
                     if i not in dct[port_type]:
                         reasons.append('Port key {}[{!r}][{}] missing'
                                        ''.format(attr, port_type, i))
 
         if reasons:
-            reason_text = '\n'.join('* {}'.format(reason)
+            reason_text = '\n'.join(f'* {reason}'
                                     for reason in reasons)
             raise ValueError(
                 'Verification of NodeDataModel class failed:\n{}'
                 ''.format(reason_text)
             )
 
     @property
```

### Comparing `qtpynodeeditor-0.2.0/qtpynodeeditor/node_geometry.py` & `qtpynodeeditor-0.3.0/qtpynodeeditor/node_geometry.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 import math
+import typing
 
 from qtpy.QtCore import QPointF, QRect, QRectF, QSizeF
 from qtpy.QtGui import QFont, QFontMetrics, QTransform
 from qtpy.QtWidgets import QSizePolicy
 
-from .base import NodeBase
 from .enums import NodeValidationState, PortType
 from .port import Port
 
+if typing.TYPE_CHECKING:
+    from .node import Node  # noqa
+
 
 class NodeGeometry:
-    def __init__(self, node: NodeBase):
+    def __init__(self, node: 'Node'):
         super().__init__()
         self._node = node
         self._model = node.model
         self._dragging_pos = QPointF(-1000, -1000)
         self._entry_width = 0
         self._entry_height = 20
         self._font_metrics = QFontMetrics(QFont())
@@ -29,46 +32,39 @@
         f = QFont()
         f.setBold(True)
         self._bold_font_metrics = QFontMetrics(f)
 
     @property
     def height(self) -> int:
         """
-        Height
+        Node height.
 
         Returns
         -------
         value : int
         """
         return self._height
 
     @height.setter
     def height(self, h: int):
         self._height = int(h)
 
     @property
     def width(self) -> int:
         """
-        Width
+        Node width.
 
         Returns
         -------
         value : int
         """
         return self._width
 
     @width.setter
     def width(self, width: int):
-        """
-        Set width
-
-        Parameters
-        ----------
-        width : int
-        """
         self._width = int(width)
 
     @property
     def entry_height(self) -> int:
         """
         Entry height
 
@@ -76,21 +72,14 @@
         -------
         value : int
         """
         return self._entry_height
 
     @entry_height.setter
     def entry_height(self, h: int):
-        """
-        Set entry height
-
-        Parameters
-        ----------
-        h : int
-        """
         self._entry_height = int(h)
 
     @property
     def entry_width(self) -> int:
         """
         Entry width
 
@@ -98,21 +87,14 @@
         -------
         value : int
         """
         return self._entry_width
 
     @entry_width.setter
     def entry_width(self, width: int):
-        """
-        Set entry width
-
-        Parameters
-        ----------
-        width : int
-        """
         self._entry_width = int(width)
 
     @property
     def spacing(self) -> int:
         """
         Spacing
 
@@ -120,21 +102,14 @@
         -------
         value : int
         """
         return self._spacing
 
     @spacing.setter
     def spacing(self, s: int):
-        """
-        Set spacing
-
-        Parameters
-        ----------
-        s : int
-        """
         self._spacing = int(s)
 
     @property
     def hovered(self) -> bool:
         """
         Hovered
 
@@ -142,60 +117,56 @@
         -------
         value : bool
         """
         return self._hovered
 
     @hovered.setter
     def hovered(self, h: int):
-        """
-        Set hovered
-
-        Parameters
-        ----------
-        h : int
-        """
         self._hovered = bool(h)
 
     @property
     def num_sources(self) -> int:
         """
-        N sources
+        Number of sources.
 
         Returns
         -------
         value : int
         """
         return self._model.num_ports[PortType.output]
 
     @property
     def num_sinks(self) -> int:
         """
-        N sinks
+        Number of sinks.
 
         Returns
         -------
         value : int
         """
         return self._model.num_ports[PortType.input]
 
     @property
-    def dragging_pos(self) -> QPointF:
+    def dragging_position(self) -> QPointF:
         """
         Dragging pos
 
         Returns
         -------
         value : QPointF
         """
         return self._dragging_pos
 
-    @dragging_pos.setter
+    @dragging_position.setter
     def dragging_position(self, pos: QPointF):
         self._dragging_pos = QPointF(pos)
 
+    # Back-compatibility
+    dragging_pos = dragging_position
+
     def entry_bounding_rect(self, *, addon=0.0) -> QRectF:
         """
         Entry bounding rect
 
         Returns
         -------
         value : QRectF
@@ -293,37 +264,48 @@
             result = QPointF(x, total_height)
         else:
             raise ValueError(port_type)
 
         return t.map(result)
 
     def check_hit_scene_point(self, port_type: PortType, scene_point: QPointF,
-                              scene_transform: QTransform) -> Port:
+                              scene_transform: QTransform) -> typing.Optional[Port]:
         """
-        Check hit scene point
+        Check a scene point for a specific port type.
 
         Parameters
         ----------
         port_type : PortType
+            The port type to check for.
+
         scene_point : QPointF
+            The point in the scene.
+
         scene_transform : QTransform
+            The scene transform.
 
         Returns
         -------
-        value : Port
+        port : Port or None
+            The nearby port, if found.
         """
         if port_type == PortType.none:
             return None
 
+        nearby_port = None
+
         tolerance = 2.0 * self._style.connection_point_diameter
         for idx, port in self._node.state[port_type].items():
             pos = port.get_mapped_scene_position(scene_transform) - scene_point
             distance = math.sqrt(QPointF.dotProduct(pos, pos))
             if distance < tolerance:
-                return port
+                nearby_port = port
+                break
+
+        return nearby_port
 
     @property
     def resize_rect(self) -> QRect:
         """
         Resize rect
 
         Returns
@@ -349,15 +331,15 @@
         if not widget:
             return QPointF()
 
         if widget.sizePolicy().verticalPolicy() & QSizePolicy.ExpandFlag:
             # If the widget wants to use as much vertical space as possible,
             # place it immediately after the caption.
             return QPointF(self._spacing + self.port_width(PortType.input),
-                           self.caption_height())
+                           self.caption_height)
 
         if self._model.validation_state() != NodeValidationState.valid:
             return QPointF(
                 self._spacing + self.port_width(PortType.input),
                 (self.caption_height + self._height - self.validation_height -
                  self._spacing - widget.height()) / 2.0,
             )
@@ -371,18 +353,18 @@
         '''
         The maximum height a widget can be without causing the node to grow.
 
         Returns
         -------
         value : int
         '''
-        base_height = self.height() - self.caption_height()
+        base_height = self.height - self.caption_height
 
         if self._model.validation_state() != NodeValidationState.valid:
-            return (base_height + self.validation_height())
+            return base_height + self.validation_height
 
         return base_height
 
     @property
     def validation_height(self) -> int:
         """
         Validation height
@@ -404,17 +386,21 @@
         value : int
         """
         msg = self._model.validation_message()
         return self._bold_font_metrics.boundingRect(msg).width()
 
     @staticmethod
     def calculate_node_position_between_node_ports(
-            target_port_index: int, target_port: PortType, target_node:
-            NodeBase, source_port_index: int, source_port: PortType,
-            source_node: NodeBase, new_node: NodeBase) -> QPointF:
+            target_port_index: int,
+            target_port: PortType,
+            target_node: 'Node',
+            source_port_index: int,
+            source_port: PortType,
+            source_node: 'Node',
+            new_node: 'Node') -> QPointF:
         """
         calculate node position between node ports
 
         Calculating the nodes position in the scene. It'll be positioned half
         way between the two ports that it "connects".  The first line
         calculates the halfway point between the ports (node position + port
         position on the node for both nodes averaged).  The second line offsets
@@ -432,14 +418,17 @@
         source_node : Node
         new_node : Node
 
         Returns
         -------
         value : QPointF
         """
+        if (source_node.graphics_object is None
+                or target_node.graphics_object is None):
+            raise ValueError('Uninitialized node')
         converter_node_pos = (
             source_node.graphics_object.pos()
             + source_node.geometry.port_scene_position(source_port, source_port_index)
             + target_node.graphics_object.pos()
             + target_node.geometry.port_scene_position(target_port, target_port_index)
         ) / 2.0
         converter_node_pos.setX(converter_node_pos.x() - new_node.geometry.width / 2.0)
```

### Comparing `qtpynodeeditor-0.2.0/qtpynodeeditor/node_graphics_object.py` & `qtpynodeeditor-0.3.0/qtpynodeeditor/node_graphics_object.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,14 +113,15 @@
         Parameters
         ----------
         painter : QPainter
         option : QStyleOptionGraphicsItem
         widget : QWidget
         """
         from .node_painter import NodePainter
+
         # TODO
         painter.setClipRect(option.exposedRect)
         NodePainter.paint(painter, self._node, self._scene,
                           node_style=self._style.node,
                           connection_style=self._style.connection,
                           )
 
@@ -181,15 +182,15 @@
                     conn, = connections
                     self._scene.delete_connection(conn)
 
                 # TODO_UPSTREAM: add to FlowScene
                 connection = self._scene.create_connection(port)
                 connection.graphics_object.grabMouse()
 
-        pos = QPoint(event.pos().x(), event.pos().y())
+        pos = QPoint(int(event.pos().x()), int(event.pos().y()))
         geom = self._node.geometry
         state = self._node.state
         if self._node.model.resizable() and geom.resize_rect.contains(pos):
             state.resizing = True
 
     def mouseMoveEvent(self, event: QGraphicsSceneMouseEvent):
         """
@@ -202,15 +203,15 @@
         geom = self._node.geometry
         state = self._node.state
         if state.resizing:
             diff = event.pos() - event.lastPos()
             w = self._node.model.embedded_widget()
             if w:
                 self.prepareGeometryChange()
-                old_size = w.size() + QSize(diff.x(), diff.y())
+                old_size = w.size() + QSize(int(diff.x()), int(diff.y()))
                 w.setFixedSize(old_size)
 
                 old_size_f = QSizeF(old_size)
                 self._proxy_widget.setMinimumSize(old_size_f)
                 self._proxy_widget.setMaximumSize(old_size_f)
                 self._proxy_widget.setPos(geom.widget_position)
                 geom.recalculate_size()
@@ -283,16 +284,17 @@
 
         Parameters
         ----------
         q_graphics_scene_hover_event : QGraphicsSceneHoverEvent
         """
         pos = event.pos()
         geom = self._node.geometry
-        if (self._node.model.resizable() and
-                geom.resize_rect.contains(QPoint(pos.x(), pos.y()))):
+        if self._node.model.resizable() and geom.resize_rect.contains(
+            QPoint(int(pos.x()), int(pos.y()))
+        ):
             self.setCursor(QCursor(Qt.SizeFDiagCursor))
         else:
             self.setCursor(QCursor())
 
         event.accept()
 
     def mouseDoubleClickEvent(self, event: QGraphicsSceneMouseEvent):
```

### Comparing `qtpynodeeditor-0.2.0/qtpynodeeditor/node_painter.py` & `qtpynodeeditor-0.3.0/qtpynodeeditor/node_painter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 import math
+import typing
 
 from qtpy.QtCore import QPointF, QRectF, Qt
 from qtpy.QtGui import QFontMetrics, QLinearGradient, QPainter, QPen
 
-from .base import FlowSceneBase, NodeBase
 from .enums import NodeValidationState, PortType
 from .node_data import NodeDataModel
 from .node_geometry import NodeGeometry
 from .node_graphics_object import NodeGraphicsObject
 from .node_state import NodeState
 from .style import ConnectionStyle, NodeStyle
 
+if typing.TYPE_CHECKING:
+    from .connection import Connection  # noqa
+    from .flow_scene import FlowScene  # noqa
+    from .node import Node  # noqa
+
 
 class NodePainterDelegate:
     def paint(self, painter: QPainter, geom: NodeGeometry, model: NodeDataModel):
         """
         Paint
 
         Parameters
@@ -24,15 +29,15 @@
         model : NodeDataModel
         """
         ...
 
 
 class NodePainter:
     @staticmethod
-    def paint(painter: QPainter, node: NodeBase, scene: FlowSceneBase,
+    def paint(painter: QPainter, node: 'Node', scene: 'FlowScene',
               node_style: NodeStyle, connection_style: ConnectionStyle):
         """
         Paint
 
         Parameters
         ----------
         painter : QPainter
@@ -40,14 +45,19 @@
         scene : FlowScene
         node_style : NodeStyle
         connection_style : ConnectionStyle
         """
         geom = node.geometry
         state = node.state
         graphics_object = node.graphics_object
+
+        if graphics_object is None:
+            # On CI, we might not have a graphics object
+            return
+
         geom.recalculate_size(painter.font())
 
         model = node.model
         NodePainter.draw_node_rect(painter, geom, model, graphics_object,
                                    node_style)
         NodePainter.draw_connection_points(painter, geom, state, model, scene,
                                            node_style, connection_style)
@@ -167,15 +177,15 @@
                 scene_pos.setX(geom.width - 5.0 - rect.width())
 
             painter.drawText(scene_pos, display_text)
 
     @staticmethod
     def draw_connection_points(painter: QPainter, geom: NodeGeometry,
                                state: NodeState, model: NodeDataModel,
-                               scene: FlowSceneBase, node_style: NodeStyle,
+                               scene: 'FlowScene', node_style: NodeStyle,
                                connection_style: ConnectionStyle
                                ):
         """
         Draw connection points
 
         Parameters
         ----------
```

### Comparing `qtpynodeeditor-0.2.0/qtpynodeeditor/node_state.py` & `qtpynodeeditor-0.3.0/qtpynodeeditor/node_state.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+import typing
 from collections import OrderedDict
 
-from .base import ConnectionBase
 from .enums import ReactToConnectionState
 from .node_data import NodeDataType
 from .port import Port, PortType
 
+if typing.TYPE_CHECKING:
+    from .connection import Connection  # noqa
+
 
 class NodeState:
     def __init__(self, node):
         '''
         node_state
 
         Parameters
@@ -82,15 +85,15 @@
 
         Returns
         -------
         value : list
         """
         return list(self._ports[port_type][port_index].connections)
 
-    def erase_connection(self, port_type: PortType, port_index: int, connection: ConnectionBase):
+    def erase_connection(self, port_type: PortType, port_index: int, connection: 'Connection'):
         """
         Erase connection
 
         Parameters
         ----------
         port_type : PortType
         port_index : int
```

### Comparing `qtpynodeeditor-0.2.0/qtpynodeeditor/port.py` & `qtpynodeeditor-0.3.0/qtpynodeeditor/port.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,45 @@
+import typing
+
 from qtpy.QtCore import QObject, Signal
 
-from .base import ConnectionBase
 from .enums import ConnectionPolicy, PortType
 
+if typing.TYPE_CHECKING:
+    from .connection import Connection  # noqa
+
 
-def opposite_port(port: PortType):
+def opposite_port(port: PortType) -> PortType:
+    """
+    Get the opposite port of `port`.
+
+    Parameters
+    ----------
+    port : PortType
+    """
     return {PortType.input: PortType.output,
             PortType.output: PortType.input}.get(port, PortType.none)
 
 
 class Port(QObject):
-    connection_created = Signal(ConnectionBase)
-    connection_deleted = Signal(ConnectionBase)
+    """
+
+    Signals
+    -------
+    connection_created : Signal(Connection)
+    connection_deleted : Signal(Connection)
+    data_updated : Signal(QObject)
+    data_invalidated : Signal(QObject)
+    """
+
+    connection_created = Signal(object)
+    connection_deleted = Signal(object)
     data_updated = Signal(QObject)
     data_invalidated = Signal(QObject)
+    _connections: list['Connection']
 
     def __init__(self, node, *, port_type: PortType, index: int):
         super().__init__(parent=node)
         self.node = node
         self.port_type = port_type
         self.index = index
         self._connections = []
@@ -75,23 +97,23 @@
     def connection_policy(self):
         'The connection policy (one/many) for the port'
         if self.port_type == PortType.input:
             return ConnectionPolicy.one
         else:
             return self.model.port_out_connection_policy(self.index)
 
-    def add_connection(self, connection: ConnectionBase):
+    def add_connection(self, connection: 'Connection'):
         'Add a Connection to the Port'
         if connection in self._connections:
             raise ValueError('Connection already in list')
 
         self._connections.append(connection)
         self.connection_created.emit(connection)
 
-    def remove_connection(self, connection: ConnectionBase):
+    def remove_connection(self, connection: 'Connection'):
         'Remove a Connection from the Port'
         try:
             self._connections.remove(connection)
         except ValueError:
             # TODO: should not be reaching this
             ...
         else:
```

### Comparing `qtpynodeeditor-0.2.0/qtpynodeeditor/style.py` & `qtpynodeeditor-0.3.0/qtpynodeeditor/style.py`

 * *Files identical despite different names*

### Comparing `qtpynodeeditor-0.2.0/qtpynodeeditor/tests/test_basic.py` & `qtpynodeeditor-0.3.0/qtpynodeeditor/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `qtpynodeeditor-0.2.0/qtpynodeeditor/tests/test_examples.py` & `qtpynodeeditor-0.3.0/qtpynodeeditor/tests/test_examples.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,16 +81,16 @@
                           QtCore.Qt.NoModifier)
 
         if node.model.num_ports['input']:
             pos = node.geometry.port_scene_position('input', 0)
         else:
             pos = node.geometry.port_scene_position('output', 0)
 
-        ev.scene_pos = QtCore.QPoint(pos.x(), pos.y())
-        ev.last_pos = QtCore.QPoint(pos.x(), pos.y())
+        ev.scene_pos = QtCore.QPoint(int(pos.x()), int(pos.y()))
+        ev.last_pos = QtCore.QPoint(int(pos.x()), int(pos.y()))
 
         if node.model.resizable():
             # Other case will try to propagate to mouseMoveEvent
             node.state.resizing = True
             ngo.mouseMoveEvent(ev)
 
         ngo.mousePressEvent(ev)
```

### Comparing `qtpynodeeditor-0.2.0/qtpynodeeditor/type_converter.py` & `qtpynodeeditor-0.3.0/qtpynodeeditor/type_converter.py`

 * *Files identical despite different names*

