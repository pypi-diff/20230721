# Comparing `tmp/rst_include-2.1.2.2.tar.gz` & `tmp/rst_include-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rst_include-2.1.2.2.tar", last modified: Fri Jun  3 18:57:09 2022, max compression
+gzip compressed data, was "rst_include-2.1.3.tar", last modified: Fri Jul 21 16:46:12 2023, max compression
```

## Comparing `rst_include-2.1.2.2.tar` & `rst_include-2.1.3.tar`

### file list

```diff
@@ -1,48 +1,124 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 18:57:09.000000 rst_include-2.1.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 18:57:09.000000 rst_include-2.1.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      230 2022-06-03 18:56:22.000000 rst_include-2.1.2.2/tests/include2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 18:57:09.000000 rst_include-2.1.2.2/tests/subdir/
--rw-r--r--   0 runner    (1001) docker     (121)      228 2022-06-03 18:56:22.000000 rst_include-2.1.2.2/tests/subdir/include_subdir.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-03 18:56:22.000000 rst_include-2.1.2.2/tests/subdir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-03 18:56:22.000000 rst_include-2.1.2.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1266 2022-06-03 18:56:22.000000 rst_include-2.1.2.2/tests/test_include_files.py
--rw-r--r--   0 runner    (1001) docker     (121)      986 2022-06-03 18:56:22.000000 rst_include-2.1.2.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-06-03 18:56:22.000000 rst_include-2.1.2.2/tests/include1.py
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-06-03 18:56:22.000000 rst_include-2.1.2.2/tests/include3.py
--rw-r--r--   0 runner    (1001) docker     (121)      253 2022-06-03 18:56:22.000000 rst_include-2.1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     4149 2022-06-03 18:56:22.000000 rst_include-2.1.2.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    17911 2022-06-03 18:56:22.000000 rst_include-2.1.2.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)   106885 2022-06-03 18:56:22.000000 rst_include-2.1.2.2/test.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 18:57:09.000000 rst_include-2.1.2.2/rst_include/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-03 18:56:22.000000 rst_include-2.1.2.2/rst_include/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     4940 2022-06-03 18:56:22.000000 rst_include-2.1.2.2/rst_include/rst_include.py
--rw-r--r--   0 runner    (1001) docker     (121)      438 2022-06-03 18:56:22.000000 rst_include-2.1.2.2/rst_include/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      521 2022-06-03 18:56:22.000000 rst_include-2.1.2.2/rst_include/__init__conf__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 18:57:09.000000 rst_include-2.1.2.2/rst_include/libs/
--rw-r--r--   0 runner    (1001) docker     (121)    14005 2022-06-03 18:56:22.000000 rst_include-2.1.2.2/rst_include/libs/lib_get_include_options.py
--rw-r--r--   0 runner    (1001) docker     (121)     3563 2022-06-03 18:56:22.000000 rst_include-2.1.2.2/rst_include/libs/lib_test_compare_results.py
--rw-r--r--   0 runner    (1001) docker     (121)     2427 2022-06-03 18:56:22.000000 rst_include-2.1.2.2/rst_include/libs/lib_block.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-03 18:56:22.000000 rst_include-2.1.2.2/rst_include/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7595 2022-06-03 18:56:22.000000 rst_include-2.1.2.2/rst_include/libs/lib_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    11352 2022-06-03 18:56:22.000000 rst_include-2.1.2.2/rst_include/libs/lib_include_file.py
--rw-r--r--   0 runner    (1001) docker     (121)     6662 2022-06-03 18:56:22.000000 rst_include-2.1.2.2/rst_include/libs/lib_block_options.py
--rw-r--r--   0 runner    (1001) docker     (121)     2249 2022-06-03 18:56:22.000000 rst_include-2.1.2.2/rst_include/libs/lib_main.py
--rw-r--r--   0 runner    (1001) docker     (121)    11309 2022-06-03 18:56:22.000000 rst_include-2.1.2.2/rst_include/libs/lib_check_files.py
--rw-r--r--   0 runner    (1001) docker     (121)     1511 2022-06-03 18:56:22.000000 rst_include-2.1.2.2/rst_include/libs/lib_str.py
--rw-r--r--   0 runner    (1001) docker     (121)     9361 2022-06-03 18:56:22.000000 rst_include-2.1.2.2/rst_include/libs/lib_assemble_block.py
--rw-r--r--   0 runner    (1001) docker     (121)     2060 2022-06-03 18:56:22.000000 rst_include-2.1.2.2/rst_include/libs/lib_classes.py
--rw-r--r--   0 runner    (1001) docker     (121)     5033 2022-06-03 18:56:22.000000 rst_include-2.1.2.2/rst_include/libs/lib_source_line.py
--rw-r--r--   0 runner    (1001) docker     (121)     3943 2022-06-03 18:56:22.000000 rst_include-2.1.2.2/rst_include/rst_include_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     1076 2022-06-03 18:56:22.000000 rst_include-2.1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      617 2022-06-03 18:57:09.000000 rst_include-2.1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2089 2022-06-03 18:56:22.000000 rst_include-2.1.2.2/CHANGES.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 18:57:09.000000 rst_include-2.1.2.2/rst_include.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-06-03 18:57:09.000000 rst_include-2.1.2.2/rst_include.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-03 18:57:09.000000 rst_include-2.1.2.2/rst_include.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-03 18:57:08.000000 rst_include-2.1.2.2/rst_include.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-06-03 18:57:09.000000 rst_include-2.1.2.2/rst_include.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1090 2022-06-03 18:57:09.000000 rst_include-2.1.2.2/rst_include.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)    18606 2022-06-03 18:57:09.000000 rst_include-2.1.2.2/rst_include.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-06-03 18:57:09.000000 rst_include-2.1.2.2/rst_include.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)    18606 2022-06-03 18:57:09.000000 rst_include-2.1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-06-03 18:56:22.000000 rst_include-2.1.2.2/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:46:12.613271 rst_include-2.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:46:12.601271 rst_include-2.1.3/.3rd_party_stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-21 16:45:23.000000 rst_include-2.1.3/.3rd_party_stubs/readme.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-21 16:45:23.000000 rst_include-2.1.3/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:46:12.605271 rst_include-2.1.3/.docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-21 16:45:23.000000 rst_include-2.1.3/.docs/README_template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-21 16:45:23.000000 rst_include-2.1.3/.docs/acknowledgment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-07-21 16:45:23.000000 rst_include-2.1.3/.docs/badges.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-21 16:45:23.000000 rst_include-2.1.3/.docs/commandline_help.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-21 16:45:23.000000 rst_include-2.1.3/.docs/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-21 16:45:23.000000 rst_include-2.1.3/.docs/description.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-21 16:45:23.000000 rst_include-2.1.3/.docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-21 16:45:23.000000 rst_include-2.1.3/.docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-21 16:45:23.000000 rst_include-2.1.3/.docs/installation_via_makefile.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-21 16:45:23.000000 rst_include-2.1.3/.docs/installation_via_pypi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-21 16:45:23.000000 rst_include-2.1.3/.docs/licence_mit.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-21 16:45:23.000000 rst_include-2.1.3/.docs/tested_under.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-21 16:45:23.000000 rst_include-2.1.3/.docs/try_in_jupyter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-21 16:45:23.000000 rst_include-2.1.3/.docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-21 16:45:23.000000 rst_include-2.1.3/.docs/usage_commandline_parameter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-21 16:45:23.000000 rst_include-2.1.3/.docs/usage_examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-21 16:45:23.000000 rst_include-2.1.3/.docs/usage_examples_batch.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-21 16:45:23.000000 rst_include-2.1.3/.docs/usage_examples_python.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-21 16:45:23.000000 rst_include-2.1.3/.docs/usage_examples_shellscript.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-21 16:45:23.000000 rst_include-2.1.3/.docs/usage_include_from_commandline.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-21 16:45:23.000000 rst_include-2.1.3/.docs/usage_multiline_text_replacement.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-21 16:45:23.000000 rst_include-2.1.3/.docs/usage_rst_file_examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-21 16:45:23.000000 rst_include-2.1.3/.docs/usage_rst_file_examples_jupyter_include.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-21 16:45:23.000000 rst_include-2.1.3/.docs/usage_rst_file_examples_simple_code_include.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-21 16:45:23.000000 rst_include-2.1.3/.docs/usage_rst_file_examples_txt_or_rst_include.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-07-21 16:45:23.000000 rst_include-2.1.3/.docs/usage_rst_file_include_parameters.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-21 16:45:23.000000 rst_include-2.1.3/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:46:12.597271 rst_include-2.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:46:12.605271 rst_include-2.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-21 16:45:23.000000 rst_include-2.1.3/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9430 2023-07-21 16:45:23.000000 rst_include-2.1.3/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-21 16:45:23.000000 rst_include-2.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-21 16:45:23.000000 rst_include-2.1.3/.rotekignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-07-21 16:45:23.000000 rst_include-2.1.3/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-21 16:45:23.000000 rst_include-2.1.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-21 16:45:23.000000 rst_include-2.1.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-21 16:45:23.000000 rst_include-2.1.3/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-21 16:45:23.000000 rst_include-2.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-21 16:45:23.000000 rst_include-2.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-21 16:45:23.000000 rst_include-2.1.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    19657 2023-07-21 16:46:12.613271 rst_include-2.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-21 16:45:23.000000 rst_include-2.1.3/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    18713 2023-07-21 16:45:23.000000 rst_include-2.1.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-21 16:45:23.000000 rst_include-2.1.3/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-07-21 16:45:23.000000 rst_include-2.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-21 16:45:23.000000 rst_include-2.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-21 16:45:23.000000 rst_include-2.1.3/requirements_test.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:46:12.605271 rst_include-2.1.3/rst_include/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-21 16:45:23.000000 rst_include-2.1.3/rst_include/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-21 16:45:23.000000 rst_include-2.1.3/rst_include/__init__conf__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:46:12.609271 rst_include-2.1.3/rst_include/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:45:23.000000 rst_include-2.1.3/rst_include/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9400 2023-07-21 16:45:23.000000 rst_include-2.1.3/rst_include/libs/lib_assemble_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-07-21 16:45:23.000000 rst_include-2.1.3/rst_include/libs/lib_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6798 2023-07-21 16:45:23.000000 rst_include-2.1.3/rst_include/libs/lib_block_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11309 2023-07-21 16:45:23.000000 rst_include-2.1.3/rst_include/libs/lib_check_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-21 16:45:23.000000 rst_include-2.1.3/rst_include/libs/lib_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14005 2023-07-21 16:45:23.000000 rst_include-2.1.3/rst_include/libs/lib_get_include_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11470 2023-07-21 16:45:23.000000 rst_include-2.1.3/rst_include/libs/lib_include_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-07-21 16:45:23.000000 rst_include-2.1.3/rst_include/libs/lib_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-07-21 16:45:23.000000 rst_include-2.1.3/rst_include/libs/lib_source_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-21 16:45:23.000000 rst_include-2.1.3/rst_include/libs/lib_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7595 2023-07-21 16:45:23.000000 rst_include-2.1.3/rst_include/libs/lib_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-07-21 16:45:23.000000 rst_include-2.1.3/rst_include/libs/lib_test_compare_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:45:23.000000 rst_include-2.1.3/rst_include/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-07-21 16:45:23.000000 rst_include-2.1.3/rst_include/rst_include.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-07-21 16:45:23.000000 rst_include-2.1.3/rst_include/rst_include_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:46:12.605271 rst_include-2.1.3/rst_include.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19657 2023-07-21 16:46:12.000000 rst_include-2.1.3/rst_include.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-07-21 16:46:12.000000 rst_include-2.1.3/rst_include.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 16:46:12.000000 rst_include-2.1.3/rst_include.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-21 16:46:12.000000 rst_include-2.1.3/rst_include.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-21 16:46:12.000000 rst_include-2.1.3/rst_include.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-21 16:46:12.000000 rst_include-2.1.3/rst_include.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-21 16:45:23.000000 rst_include-2.1.3/rst_include.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 16:46:12.613271 rst_include-2.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)   182086 2023-07-21 16:45:23.000000 rst_include-2.1.3/test.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   106885 2023-07-21 16:45:23.000000 rst_include-2.1.3/test.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:46:12.613271 rst_include-2.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:45:23.000000 rst_include-2.1.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-21 16:45:23.000000 rst_include-2.1.3/tests/include0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-21 16:45:23.000000 rst_include-2.1.3/tests/include1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-21 16:45:23.000000 rst_include-2.1.3/tests/include2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-21 16:45:23.000000 rst_include-2.1.3/tests/include3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:46:12.613271 rst_include-2.1.3/tests/local_testscripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     9567 2023-07-21 16:45:23.000000 rst_include-2.1.3/tests/local_testscripts/lib_bash_functions.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-21 16:45:23.000000 rst_include-2.1.3/tests/local_testscripts/run_clean.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-21 16:45:23.000000 rst_include-2.1.3/tests/local_testscripts/run_pytest.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-21 16:45:23.000000 rst_include-2.1.3/tests/local_testscripts/run_testloop.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-21 16:45:23.000000 rst_include-2.1.3/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-21 16:45:23.000000 rst_include-2.1.3/tests/local_testscripts/run_testloop_windows.cmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-21 16:45:23.000000 rst_include-2.1.3/tests/local_testscripts/shellcheck.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-07-21 16:45:23.000000 rst_include-2.1.3/tests/local_testscripts/testing_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:46:12.613271 rst_include-2.1.3/tests/subdir/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:45:23.000000 rst_include-2.1.3/tests/subdir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-21 16:45:23.000000 rst_include-2.1.3/tests/subdir/include_subdir.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-21 16:45:23.000000 rst_include-2.1.3/tests/temp_test.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8346 2023-07-21 16:45:23.000000 rst_include-2.1.3/tests/test1_no_includes_expected.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8345 2023-07-21 16:45:23.000000 rst_include-2.1.3/tests/test1_no_includes_expected_replace.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8345 2023-07-21 16:45:23.000000 rst_include-2.1.3/tests/test1_no_includes_template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-21 16:45:23.000000 rst_include-2.1.3/tests/test2_include_samedir_expected.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-21 16:45:23.000000 rst_include-2.1.3/tests/test2_include_samedir_template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-21 16:45:23.000000 rst_include-2.1.3/tests/test3_include_subdir_expected.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-21 16:45:23.000000 rst_include-2.1.3/tests/test3_include_subdir_template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-21 16:45:23.000000 rst_include-2.1.3/tests/test4_include_nocode_expected.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-21 16:45:23.000000 rst_include-2.1.3/tests/test4_include_nocode_template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-21 16:45:23.000000 rst_include-2.1.3/tests/test5_not_supported_expected.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-21 16:45:23.000000 rst_include-2.1.3/tests/test5_not_supported_template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-21 16:45:23.000000 rst_include-2.1.3/tests/test6_include_recursion1_template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-21 16:45:23.000000 rst_include-2.1.3/tests/test6_include_recursion2_template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-21 16:45:23.000000 rst_include-2.1.3/tests/test6_include_recursion3_template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-21 16:45:23.000000 rst_include-2.1.3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-21 16:45:23.000000 rst_include-2.1.3/tests/test_compare_file_original.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-21 16:45:23.000000 rst_include-2.1.3/tests/test_compare_file_result_different.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-21 16:45:23.000000 rst_include-2.1.3/tests/test_compare_file_result_equal.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-21 16:45:23.000000 rst_include-2.1.3/tests/test_compare_file_result_longer.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-21 16:45:23.000000 rst_include-2.1.3/tests/test_compare_file_result_shorter.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-21 16:45:23.000000 rst_include-2.1.3/tests/test_include_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 16:45:23.000000 rst_include-2.1.3/tests/test_read.rst
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `rst_include-2.1.2.2/tests/test_include_files.py` & `rst_include-2.1.3/tests/test_include_files.py`

 * *Files identical despite different names*

### Comparing `rst_include-2.1.2.2/tests/test_cli.py` & `rst_include-2.1.3/tests/test_cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,14 +17,12 @@
         subprocess.run(command, shell=True, check=True)
     except subprocess.CalledProcessError:
         return False
     return True
 
 
 def test_cli_commands() -> None:
-    # due to a bug in python 3.8.1 with setup.py test on travis we need to cancel the click tests there !
-    if sys.version_info < (3, 8, 1) or sys.version_info >= (3, 8, 2):
-        assert not call_cli_command("--unknown_option")
-        assert call_cli_command("--version")
-        assert call_cli_command("-h")
-        assert call_cli_command("info")
-        assert call_cli_command("--traceback info")
+    assert not call_cli_command("--unknown_option")
+    assert call_cli_command("--version")
+    assert call_cli_command("-h")
+    assert call_cli_command("info")
+    assert call_cli_command("--traceback info")
```

### Comparing `rst_include-2.1.2.2/README.rst` & `rst_include-2.1.3/rst_include.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,73 @@
+Metadata-Version: 2.1
+Name: rst-include
+Version: 2.1.3
+Summary: commandline tool to resolve RST File includes
+Author-email: Robert Nowotny <bitranox@gmail.com>
+License: MIT
+Project-URL: Homepage, https://github.com/bitranox/rst_include
+Project-URL: Documentation, https://github.com/bitranox/rst_include/blob/master/README.rst
+Project-URL: Repository, https://github.com/bitranox/rst_include.git
+Project-URL: Changelog, https://github.com/bitranox/rst_include/blob/master/CHANGES.rst
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.8.0
+Description-Content-Type: text/x-rst
+Provides-Extra: test
+License-File: LICENSE
+
 rst_include
 ===========
 
 
-Version v2.1.2.2 as of 2022-06-03 see `Changelog`_
-
-|build_badge| |license| |pypi| |pypi-downloads| |black|
+Version v2.1.3 as of 2023-07-21 see `Changelog`_
 
-|codecov| |better_code| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+|build_badge| |codeql| |license| |pypi|
+|pypi-downloads| |black| |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/rst_include/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/rst_include/actions/workflows/python-package.yml
 
 
+.. |codeql| image:: https://github.com/bitranox/rst_include/actions/workflows/codeql-analysis.yml/badge.svg?event=push
+   :target: https://github.com//bitranox/rst_include/actions/workflows/codeql-analysis.yml
+
 .. |license| image:: https://img.shields.io/github/license/webcomics/pywine.svg
    :target: http://en.wikipedia.org/wiki/MIT_License
 
 .. |jupyter| image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/bitranox/rst_include/master?filepath=rst_include.ipynb
 
 .. for the pypi status link note the dashes, not the underscore !
 .. |pypi| image:: https://img.shields.io/pypi/status/rst-include?label=PyPI%20Package
    :target: https://badge.fury.io/py/rst_include
 
 .. |codecov| image:: https://img.shields.io/codecov/c/github/bitranox/rst_include
    :target: https://codecov.io/gh/bitranox/rst_include
 
-.. |better_code| image:: https://bettercodehub.com/edge/badge/bitranox/rst_include?branch=master
-   :target: https://bettercodehub.com/results/bitranox/rst_include
-
 .. |cc_maintain| image:: https://img.shields.io/codeclimate/maintainability-percentage/bitranox/rst_include?label=CC%20maintainability
    :target: https://codeclimate.com/github/bitranox/rst_include/maintainability
    :alt: Maintainability
 
 .. |cc_issues| image:: https://img.shields.io/codeclimate/issues/bitranox/rst_include?label=CC%20issues
    :target: https://codeclimate.com/github/bitranox/rst_include/maintainability
    :alt: Maintainability
 
 .. |cc_coverage| image:: https://img.shields.io/codeclimate/coverage/bitranox/rst_include?label=CC%20coverage
    :target: https://codeclimate.com/github/bitranox/rst_include/test_coverage
    :alt: Code Coverage
 
-.. |snyk| image:: https://img.shields.io/snyk/vulnerabilities/github/bitranox/rst_include
+.. |snyk| image:: https://snyk.io/test/github/bitranox/rst_include/badge.svg
    :target: https://snyk.io/test/github/bitranox/rst_include
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/rst-include
    :target: https://pypi.org/project/rst-include/
@@ -67,22 +88,22 @@
 - include other RST Files
 - very simple usage, throwing exit codes to detect errors on documentation at travis build-time
 - commandline or programmatic interface, You can even use it in the travis.yml
 - commandline interface supporting shellscript, cmd, pipes, config-files
 
 ----
 
-automated tests, Travis Matrix, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
+automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
-Python version required: 3.6.0 or newer
+Python version required: 3.8.0 or newer
 
-tested on recent linux with python 3.6, 3.7, 3.8, 3.9, 3.10, pypy-3.8 - architectures: amd64
+tested on recent linux with python 3.8, 3.9, 3.10, 3.11, 3.12-dev, pypy-3.9, pypy-3.10 - architectures: amd64
 
-`100% code coverage <https://codecov.io/gh/bitranox/rst_include>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/rst_include/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
+`100% code coverage <https://codeclimate.com/github/bitranox/rst_include/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/rst_include/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Usage`_
 - `Usage from Commandline`_
 - `Installation and Upgrade`_
 - `Requirements`_
@@ -387,14 +408,21 @@
 
 - to install the latest release from PyPi via pip (recommended):
 
 .. code-block::
 
     python -m pip install --upgrade rst_include
 
+
+- to install the latest release from PyPi via pip, including test dependencies:
+
+.. code-block::
+
+    python -m pip install --upgrade rst_include[test]
+
 - to install the latest version from github via pip:
 
 
 .. code-block::
 
     python -m pip install --upgrade git+https://github.com/bitranox/rst_include.git
 
@@ -410,22 +438,22 @@
     # for the latest development version :
     rst_include @ git+https://github.com/bitranox/rst_include.git
 
     # to install and upgrade all modules mentioned in requirements.txt:
     python -m pip install --upgrade -r /<path>/requirements.txt
 
 
-- to install the latest development version from source code:
+- to install the latest development version, including test dependencies from source code:
 
 .. code-block::
 
     # cd ~
     $ git clone https://github.com/bitranox/rst_include.git
     $ cd rst_include
-    python setup.py install
+    python -m pip install -e .[test]
 
 - via makefile:
   makefiles are a very convenient way to install. Here we can do much more,
   like installing virtual environments, clean caches and so on.
 
 .. code-block:: shell
 
@@ -479,14 +507,34 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.1.3
+--------
+2023-07-21:
+    - require minimum python 3.8
+    - remove python 3.7 tests
+    - introduce PEP517 packaging standard
+    - introduce pyproject.toml build-system
+    - remove mypy.ini
+    - remove pytest.ini
+    - remove setup.cfg
+    - remove setup.py
+    - remove .bettercodehub.yml
+    - remove .travis.yml
+    - update black config
+    - clean ./tests/test_cli.py
+    - add codeql badge
+    - move 3rd_party_stubs outside the src directory to ``./.3rd_party_stubs``
+    - add pypy 3.10 tests
+    - add python 3.12-dev tests
+
 v2.1.2.2
 --------
 2022-06-02: setup github actions v3, python3.10 test matrix
 
 v2.1.1
 --------
 2020-10-09: service release
```

### Comparing `rst_include-2.1.2.2/test.rst` & `rst_include-2.1.3/test.rst`

 * *Files identical despite different names*

### Comparing `rst_include-2.1.2.2/rst_include/rst_include.py` & `rst_include-2.1.3/rst_include/rst_include.py`

 * *Files identical despite different names*

### Comparing `rst_include-2.1.2.2/rst_include/libs/lib_get_include_options.py` & `rst_include-2.1.3/rst_include/libs/lib_get_include_options.py`

 * *Files identical despite different names*

### Comparing `rst_include-2.1.2.2/rst_include/libs/lib_test_compare_results.py` & `rst_include-2.1.3/rst_include/libs/lib_test_compare_results.py`

 * *Files identical despite different names*

### Comparing `rst_include-2.1.2.2/rst_include/libs/lib_block.py` & `rst_include-2.1.3/rst_include/libs/lib_block.py`

 * *Files identical despite different names*

### Comparing `rst_include-2.1.2.2/rst_include/libs/lib_test.py` & `rst_include-2.1.3/rst_include/libs/lib_test.py`

 * *Files identical despite different names*

### Comparing `rst_include-2.1.2.2/rst_include/libs/lib_include_file.py` & `rst_include-2.1.3/rst_include/libs/lib_include_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         include_file_lines = delete_empty_lines_from_list(include_file_lines)
         block.include_file_lines = include_file_lines
         includes_stack.popitem()
         return include_file_lines
 
     except FileNotFoundError:
         s_error = f'Error in File "{block.source}", Line {block.l_source_lines[0].line_number}: File not found : '\
-                  '"{block.include_filename_absolut}"'
+                  '"{block.include_filename_absolut}"'  # noqa: E126    # for python 3.12beta
         lib_log_utils.log_traceback.log_exception_traceback(s_error)
         raise IOError(s_error)
 
 
 def delete_empty_lines_from_list(source_lines: List[str]) -> List[str]:
     source_lines_without_empty_lines = [str(element) for element in lib_list.ls_strip_list(source_lines)]
     return source_lines_without_empty_lines
@@ -221,24 +221,24 @@
     content = lib_str.strip_multiline_string(content)
     block.include_file_sliced_content = content
 
 
 def log_and_raise_if_start_after_not_found_in_string(content: str, block: Block) -> None:
     if block.include_file_start_after not in content:
         s_error = f'Error in File "{block.source}", Line {block.l_source_lines[0].line_number}: '\
-                  f'include File "{block.include_filename}" : start-after "{block.include_file_start_after}" not found'
+                  f'include File "{block.include_filename}" : start-after "{block.include_file_start_after}" not found'   # noqa: E126    # for python 3.12beta
         s_error = s_error + get_additional_error_string(block)
         lib_log_utils.log_error(s_error)
         raise ValueError(s_error)
 
 
 def log_and_raise_if_end_before_not_found_in_string(content: str, block: Block) -> None:
     if block.include_file_end_before not in content:
         s_error = f'Error in File "{block.source}", Line {block.l_source_lines[0].line_number}: ' \
-                  f'include File "{block.include_filename}" : end-before "{block.include_file_end_before}" not found'
+                  f'include File "{block.include_filename}" : end-before "{block.include_file_end_before}" not found'  # noqa: E126    # for python 3.12beta
         s_error = s_error + get_additional_error_string(block)
         s_error = s_error + get_additional_error_string_start_after(block)
         lib_log_utils.log_error(s_error)
         raise ValueError(s_error)
 
 
 def get_additional_error_string(block: Block) -> str:
```

### Comparing `rst_include-2.1.2.2/rst_include/libs/lib_block_options.py` & `rst_include-2.1.3/rst_include/libs/lib_block_options.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,57 +15,57 @@
     import lib_source_line                          # type: ignore # pragma: no cover
     import lib_test                                 # type: ignore # pragma: no cover
 
 
 def get_option_value_from_block_or_raise_if_empty_or_invalid(option: str, block: Block, value_must_be_int: bool = False) -> str:
 
     """
-    >>> block = lib_test.get_test_block_ok()
+    >>> my_block = lib_test.get_test_block_ok()
     >>> # test ok
-    >>> get_option_value_from_block_or_raise_if_empty_or_invalid('code', block)
+    >>> get_option_value_from_block_or_raise_if_empty_or_invalid('code', my_block)
     'python'
 
     >>> # empty value
-    >>> get_option_value_from_block_or_raise_if_empty_or_invalid('pass-through1', block)
+    >>> get_option_value_from_block_or_raise_if_empty_or_invalid('pass-through1', my_block)
     Traceback (most recent call last):
     ...
     ValueError: Error in File ".../README.template.rst", Line 47107: option "pass-through1" has no value
 
     >>> # option not found
-    >>> get_option_value_from_block_or_raise_if_empty_or_invalid('no-option', block)
+    >>> get_option_value_from_block_or_raise_if_empty_or_invalid('no-option', my_block)
     Traceback (most recent call last):
     ...
     ValueError: Error in File: ".../README.template.rst", option "no-option" not found in block starting with Line: 47100
 
     >>> # option check type integer ok
-    >>> get_option_value_from_block_or_raise_if_empty_or_invalid('start-line', block, value_must_be_int=True)
+    >>> get_option_value_from_block_or_raise_if_empty_or_invalid('start-line', my_block, value_must_be_int=True)
     '10'
 
     >>> # option check type not integer
-    >>> get_option_value_from_block_or_raise_if_empty_or_invalid('start-after', block, value_must_be_int=True)
+    >>> get_option_value_from_block_or_raise_if_empty_or_invalid('start-after', my_block, value_must_be_int=True)
     Traceback (most recent call last):
     ...
     TypeError: Error in File ".../README.template.rst", Line 47105: option "start-after" has to be integer
 
     """
     log_and_raise_value_error_if_option_not_in_block(option, block)
     value = get_option_value_from_block(option, block)
     log_and_raise_if_value_of_option_in_block_is_empty(value, option, block)
     log_and_raise_if_value_of_option_in_block_must_be_int_castable_but_is_not(value, option, block, value_must_be_int)
     return value
 
 
 def get_option_value_from_block(option: str, block: Block) -> str:
     """
-    >>> block = lib_test.get_test_block_ok()
-    >>> get_option_value_from_block('code', block)
+    >>> my_block = lib_test.get_test_block_ok()
+    >>> get_option_value_from_block('code', my_block)
     'python'
-    >>> get_option_value_from_block('encoding', block)
+    >>> get_option_value_from_block('encoding', my_block)
     'utf-8'
-    >>> get_option_value_from_block('no-option', block)
+    >>> get_option_value_from_block('no-option', my_block)
     Traceback (most recent call last):
     ...
     ValueError: Error in File: ".../README.template.rst", option "no-option" not found in block starting with Line: 47100
 
     """
     log_and_raise_value_error_if_option_not_in_block(option, block)
     option_value = ''
@@ -79,37 +79,37 @@
 def get_option_value_from_source_line(source_line: SourceLine) -> str:
     option_value = source_line.content.split(':', 2)[2].strip()
     return option_value
 
 
 def is_option_in_block(option: str, block: Block) -> bool:
     """
-    >>> block = lib_test.get_test_block_ok()
-    >>> is_option_in_block('code', block)
+    >>> my_block = lib_test.get_test_block_ok()
+    >>> is_option_in_block('code', my_block)
     True
-    >>> is_option_in_block('no-option', block)
+    >>> is_option_in_block('no-option', my_block)
     False
 
     """
     for source_line in block.l_source_lines:
         if is_option_in_source_line(source_line, option):
             return True
         if not lib_source_line.source_line_contains_option(source_line):
             break
     return False
 
 
 def get_source_line_number_for_option(option: str, block: Block) -> int:
     """
-    >>> block = lib_test.get_test_block_ok()
-    >>> get_source_line_number_for_option('code', block)
+    >>> my_block = lib_test.get_test_block_ok()
+    >>> get_source_line_number_for_option('code', my_block)
     47101
-    >>> get_source_line_number_for_option('encoding', block)
+    >>> get_source_line_number_for_option('encoding', my_block)
     47102
-    >>> get_source_line_number_for_option('no-option', block)
+    >>> get_source_line_number_for_option('no-option', my_block)
     Traceback (most recent call last):
       ...
     ValueError: Error in File: ".../README.template.rst", option "no-option" not found in block starting with Line: 47100
     """
     log_and_raise_value_error_if_option_not_in_block(option, block)
     line_number = 0
     for source_line in block.l_source_lines:                    # pragma: no cover    # there are always lines, otherwise Value Error is raised
@@ -117,41 +117,42 @@
             line_number = source_line.line_number
             break
     return line_number
 
 
 def is_option_in_source_line(source_line: SourceLine, option: str) -> bool:
     """
-    >>> source_line = lib_classes.SourceLine(line_number=4711, content='   :code:')
-    >>> is_option_in_source_line(source_line, 'code')
+    >>> my_source_line = lib_classes.SourceLine(line_number=4711, content='   :code:')
+    >>> is_option_in_source_line(my_source_line, 'code')
     True
-    >>> is_option_in_source_line(source_line, 'encoding')
+    >>> is_option_in_source_line(my_source_line, 'encoding')
     False
 
     """
     option_marked = ':' + option + ':'
     if source_line.content.strip().startswith(option_marked):
         return True
     else:
         return False
 
 
 def get_option_key_from_source_line(source_line: SourceLine) -> str:
     """
-    >>> source_line = lib_classes.SourceLine(line_number=4711, content='   :code:')
-    >>> get_option_key_from_source_line(source_line)
+    >>> my_source_line = lib_classes.SourceLine(line_number=4711, content='   :code:')
+    >>> get_option_key_from_source_line(my_source_line)
     'code'
     """
     key = source_line.content.split(':')[1]
     return key
 
 
 def log_and_raise_value_error_if_option_not_in_block(option: str, block: Block) -> None:
     if not is_option_in_block(option, block):
-        s_error = f'Error in File: "{block.source}", option "{option}" not found in block starting with Line: {block.l_source_lines[0].line_number}'
+        s_error = f'Error in File: "{block.source}", option "{option}' \
+                  f'" not found in block starting with Line: {block.l_source_lines[0].line_number}'    # noqa: E126 E713    # for python 3.12beta
         lib_log_utils.log_error(s_error)
         raise ValueError(s_error)
 
 
 def log_and_raise_if_value_of_option_in_block_is_empty(value: str, option: str, block: Block) -> None:
     if not value:
         line_number = get_source_line_number_for_option(option, block)
```

### Comparing `rst_include-2.1.2.2/rst_include/libs/lib_main.py` & `rst_include-2.1.3/rst_include/libs/lib_main.py`

 * *Files identical despite different names*

### Comparing `rst_include-2.1.2.2/rst_include/libs/lib_check_files.py` & `rst_include-2.1.3/rst_include/libs/lib_check_files.py`

 * *Files identical despite different names*

### Comparing `rst_include-2.1.2.2/rst_include/libs/lib_str.py` & `rst_include-2.1.3/rst_include/libs/lib_str.py`

 * *Files identical despite different names*

### Comparing `rst_include-2.1.2.2/rst_include/libs/lib_assemble_block.py` & `rst_include-2.1.3/rst_include/libs/lib_assemble_block.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,15 @@
     >>> block.include_file_code = ''
     >>> get_block_header(block)
     ''
     """
     content = ''
     if block.include_file_code:
         content_lines = list()
-        content_lines.append(f'.. code-block:: {block.include_file_code}')
+        content_lines.append(f'.. code-block:: {block.include_file_code}')  # noqa: E231    # for python 3.12beta
         content_lines = content_lines + [pass_through_option.content for pass_through_option in block.pass_through_options]
         content = '\n'.join(content_lines)
     return content
 
 
 def set_number_of_blanks_to_add(block: Block) -> int:
     """
```

### Comparing `rst_include-2.1.2.2/rst_include/libs/lib_classes.py` & `rst_include-2.1.3/rst_include/libs/lib_classes.py`

 * *Files identical despite different names*

### Comparing `rst_include-2.1.2.2/rst_include/libs/lib_source_line.py` & `rst_include-2.1.3/rst_include/libs/lib_source_line.py`

 * *Files identical despite different names*

### Comparing `rst_include-2.1.2.2/rst_include/rst_include_cli.py` & `rst_include-2.1.3/rst_include/rst_include_cli.py`

 * *Files identical despite different names*

### Comparing `rst_include-2.1.2.2/LICENSE` & `rst_include-2.1.3/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 1990-2022 Robert Nowotny
+Copyright (c) 1990-2023 Robert Nowotny
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `rst_include-2.1.2.2/CHANGES.rst` & `rst_include-2.1.3/CHANGES.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,34 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.1.3
+--------
+2023-07-21:
+    - require minimum python 3.8
+    - remove python 3.7 tests
+    - introduce PEP517 packaging standard
+    - introduce pyproject.toml build-system
+    - remove mypy.ini
+    - remove pytest.ini
+    - remove setup.cfg
+    - remove setup.py
+    - remove .bettercodehub.yml
+    - remove .travis.yml
+    - update black config
+    - clean ./tests/test_cli.py
+    - add codeql badge
+    - move 3rd_party_stubs outside the src directory to ``./.3rd_party_stubs``
+    - add pypy 3.10 tests
+    - add python 3.12-dev tests
+
 v2.1.2.2
 --------
 2022-06-02: setup github actions v3, python3.10 test matrix
 
 v2.1.1
 --------
 2020-10-09: service release
```

### Comparing `rst_include-2.1.2.2/rst_include.egg-info/PKG-INFO` & `rst_include-2.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,72 +1,73 @@
 Metadata-Version: 2.1
-Name: rst-include
-Version: 2.1.2.2
+Name: rst_include
+Version: 2.1.3
 Summary: commandline tool to resolve RST File includes
-Home-page: https://github.com/bitranox/rst_include
-Author: Robert Nowotny
-Author-email: bitranox@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
+Author-email: Robert Nowotny <bitranox@gmail.com>
+License: MIT
+Project-URL: Homepage, https://github.com/bitranox/rst_include
+Project-URL: Documentation, https://github.com/bitranox/rst_include/blob/master/README.rst
+Project-URL: Repository, https://github.com/bitranox/rst_include.git
+Project-URL: Changelog, https://github.com/bitranox/rst_include/blob/master/CHANGES.rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6.0
+Requires-Python: >=3.8.0
 Description-Content-Type: text/x-rst
+Provides-Extra: test
 License-File: LICENSE
 
 rst_include
 ===========
 
 
-Version v2.1.2.2 as of 2022-06-03 see `Changelog`_
+Version v2.1.3 as of 2023-07-21 see `Changelog`_
 
-|build_badge| |license| |pypi| |pypi-downloads| |black|
-
-|codecov| |better_code| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+|build_badge| |codeql| |license| |pypi|
+|pypi-downloads| |black| |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/rst_include/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/rst_include/actions/workflows/python-package.yml
 
 
+.. |codeql| image:: https://github.com/bitranox/rst_include/actions/workflows/codeql-analysis.yml/badge.svg?event=push
+   :target: https://github.com//bitranox/rst_include/actions/workflows/codeql-analysis.yml
+
 .. |license| image:: https://img.shields.io/github/license/webcomics/pywine.svg
    :target: http://en.wikipedia.org/wiki/MIT_License
 
 .. |jupyter| image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/bitranox/rst_include/master?filepath=rst_include.ipynb
 
 .. for the pypi status link note the dashes, not the underscore !
 .. |pypi| image:: https://img.shields.io/pypi/status/rst-include?label=PyPI%20Package
    :target: https://badge.fury.io/py/rst_include
 
 .. |codecov| image:: https://img.shields.io/codecov/c/github/bitranox/rst_include
    :target: https://codecov.io/gh/bitranox/rst_include
 
-.. |better_code| image:: https://bettercodehub.com/edge/badge/bitranox/rst_include?branch=master
-   :target: https://bettercodehub.com/results/bitranox/rst_include
-
 .. |cc_maintain| image:: https://img.shields.io/codeclimate/maintainability-percentage/bitranox/rst_include?label=CC%20maintainability
    :target: https://codeclimate.com/github/bitranox/rst_include/maintainability
    :alt: Maintainability
 
 .. |cc_issues| image:: https://img.shields.io/codeclimate/issues/bitranox/rst_include?label=CC%20issues
    :target: https://codeclimate.com/github/bitranox/rst_include/maintainability
    :alt: Maintainability
 
 .. |cc_coverage| image:: https://img.shields.io/codeclimate/coverage/bitranox/rst_include?label=CC%20coverage
    :target: https://codeclimate.com/github/bitranox/rst_include/test_coverage
    :alt: Code Coverage
 
-.. |snyk| image:: https://img.shields.io/snyk/vulnerabilities/github/bitranox/rst_include
+.. |snyk| image:: https://snyk.io/test/github/bitranox/rst_include/badge.svg
    :target: https://snyk.io/test/github/bitranox/rst_include
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/rst-include
    :target: https://pypi.org/project/rst-include/
@@ -87,22 +88,22 @@
 - include other RST Files
 - very simple usage, throwing exit codes to detect errors on documentation at travis build-time
 - commandline or programmatic interface, You can even use it in the travis.yml
 - commandline interface supporting shellscript, cmd, pipes, config-files
 
 ----
 
-automated tests, Travis Matrix, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
+automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
-Python version required: 3.6.0 or newer
+Python version required: 3.8.0 or newer
 
-tested on recent linux with python 3.6, 3.7, 3.8, 3.9, 3.10, pypy-3.8 - architectures: amd64
+tested on recent linux with python 3.8, 3.9, 3.10, 3.11, 3.12-dev, pypy-3.9, pypy-3.10 - architectures: amd64
 
-`100% code coverage <https://codecov.io/gh/bitranox/rst_include>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/rst_include/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
+`100% code coverage <https://codeclimate.com/github/bitranox/rst_include/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/rst_include/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Usage`_
 - `Usage from Commandline`_
 - `Installation and Upgrade`_
 - `Requirements`_
@@ -407,14 +408,21 @@
 
 - to install the latest release from PyPi via pip (recommended):
 
 .. code-block::
 
     python -m pip install --upgrade rst_include
 
+
+- to install the latest release from PyPi via pip, including test dependencies:
+
+.. code-block::
+
+    python -m pip install --upgrade rst_include[test]
+
 - to install the latest version from github via pip:
 
 
 .. code-block::
 
     python -m pip install --upgrade git+https://github.com/bitranox/rst_include.git
 
@@ -430,22 +438,22 @@
     # for the latest development version :
     rst_include @ git+https://github.com/bitranox/rst_include.git
 
     # to install and upgrade all modules mentioned in requirements.txt:
     python -m pip install --upgrade -r /<path>/requirements.txt
 
 
-- to install the latest development version from source code:
+- to install the latest development version, including test dependencies from source code:
 
 .. code-block::
 
     # cd ~
     $ git clone https://github.com/bitranox/rst_include.git
     $ cd rst_include
-    python setup.py install
+    python -m pip install -e .[test]
 
 - via makefile:
   makefiles are a very convenient way to install. Here we can do much more,
   like installing virtual environments, clean caches and so on.
 
 .. code-block:: shell
 
@@ -499,14 +507,34 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.1.3
+--------
+2023-07-21:
+    - require minimum python 3.8
+    - remove python 3.7 tests
+    - introduce PEP517 packaging standard
+    - introduce pyproject.toml build-system
+    - remove mypy.ini
+    - remove pytest.ini
+    - remove setup.cfg
+    - remove setup.py
+    - remove .bettercodehub.yml
+    - remove .travis.yml
+    - update black config
+    - clean ./tests/test_cli.py
+    - add codeql badge
+    - move 3rd_party_stubs outside the src directory to ``./.3rd_party_stubs``
+    - add pypy 3.10 tests
+    - add python 3.12-dev tests
+
 v2.1.2.2
 --------
 2022-06-02: setup github actions v3, python3.10 test matrix
 
 v2.1.1
 --------
 2020-10-09: service release
@@ -599,9 +627,7 @@
 ---------
 2019-04-28: add empty line at the end of the assembled documentation, to be able to add CHANGES.rst with setup.py
 
 1.0.0
 ---------
 2019-04-19: Initial public release, PyPi Release
 
-
-
```

### Comparing `rst_include-2.1.2.2/PKG-INFO` & `rst_include-2.1.3/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,72 +1,51 @@
-Metadata-Version: 2.1
-Name: rst_include
-Version: 2.1.2.2
-Summary: commandline tool to resolve RST File includes
-Home-page: https://github.com/bitranox/rst_include
-Author: Robert Nowotny
-Author-email: bitranox@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6.0
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
 rst_include
 ===========
 
 
-Version v2.1.2.2 as of 2022-06-03 see `Changelog`_
-
-|build_badge| |license| |pypi| |pypi-downloads| |black|
+Version v2.1.3 as of 2023-07-21 see `Changelog`_
 
-|codecov| |better_code| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+|build_badge| |codeql| |license| |pypi|
+|pypi-downloads| |black| |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/rst_include/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/rst_include/actions/workflows/python-package.yml
 
 
+.. |codeql| image:: https://github.com/bitranox/rst_include/actions/workflows/codeql-analysis.yml/badge.svg?event=push
+   :target: https://github.com//bitranox/rst_include/actions/workflows/codeql-analysis.yml
+
 .. |license| image:: https://img.shields.io/github/license/webcomics/pywine.svg
    :target: http://en.wikipedia.org/wiki/MIT_License
 
 .. |jupyter| image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/bitranox/rst_include/master?filepath=rst_include.ipynb
 
 .. for the pypi status link note the dashes, not the underscore !
 .. |pypi| image:: https://img.shields.io/pypi/status/rst-include?label=PyPI%20Package
    :target: https://badge.fury.io/py/rst_include
 
 .. |codecov| image:: https://img.shields.io/codecov/c/github/bitranox/rst_include
    :target: https://codecov.io/gh/bitranox/rst_include
 
-.. |better_code| image:: https://bettercodehub.com/edge/badge/bitranox/rst_include?branch=master
-   :target: https://bettercodehub.com/results/bitranox/rst_include
-
 .. |cc_maintain| image:: https://img.shields.io/codeclimate/maintainability-percentage/bitranox/rst_include?label=CC%20maintainability
    :target: https://codeclimate.com/github/bitranox/rst_include/maintainability
    :alt: Maintainability
 
 .. |cc_issues| image:: https://img.shields.io/codeclimate/issues/bitranox/rst_include?label=CC%20issues
    :target: https://codeclimate.com/github/bitranox/rst_include/maintainability
    :alt: Maintainability
 
 .. |cc_coverage| image:: https://img.shields.io/codeclimate/coverage/bitranox/rst_include?label=CC%20coverage
    :target: https://codeclimate.com/github/bitranox/rst_include/test_coverage
    :alt: Code Coverage
 
-.. |snyk| image:: https://img.shields.io/snyk/vulnerabilities/github/bitranox/rst_include
+.. |snyk| image:: https://snyk.io/test/github/bitranox/rst_include/badge.svg
    :target: https://snyk.io/test/github/bitranox/rst_include
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/rst-include
    :target: https://pypi.org/project/rst-include/
@@ -87,22 +66,22 @@
 - include other RST Files
 - very simple usage, throwing exit codes to detect errors on documentation at travis build-time
 - commandline or programmatic interface, You can even use it in the travis.yml
 - commandline interface supporting shellscript, cmd, pipes, config-files
 
 ----
 
-automated tests, Travis Matrix, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
+automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
-Python version required: 3.6.0 or newer
+Python version required: 3.8.0 or newer
 
-tested on recent linux with python 3.6, 3.7, 3.8, 3.9, 3.10, pypy-3.8 - architectures: amd64
+tested on recent linux with python 3.8, 3.9, 3.10, 3.11, 3.12-dev, pypy-3.9, pypy-3.10 - architectures: amd64
 
-`100% code coverage <https://codecov.io/gh/bitranox/rst_include>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/rst_include/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
+`100% code coverage <https://codeclimate.com/github/bitranox/rst_include/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/rst_include/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Usage`_
 - `Usage from Commandline`_
 - `Installation and Upgrade`_
 - `Requirements`_
@@ -407,14 +386,21 @@
 
 - to install the latest release from PyPi via pip (recommended):
 
 .. code-block::
 
     python -m pip install --upgrade rst_include
 
+
+- to install the latest release from PyPi via pip, including test dependencies:
+
+.. code-block::
+
+    python -m pip install --upgrade rst_include[test]
+
 - to install the latest version from github via pip:
 
 
 .. code-block::
 
     python -m pip install --upgrade git+https://github.com/bitranox/rst_include.git
 
@@ -430,22 +416,22 @@
     # for the latest development version :
     rst_include @ git+https://github.com/bitranox/rst_include.git
 
     # to install and upgrade all modules mentioned in requirements.txt:
     python -m pip install --upgrade -r /<path>/requirements.txt
 
 
-- to install the latest development version from source code:
+- to install the latest development version, including test dependencies from source code:
 
 .. code-block::
 
     # cd ~
     $ git clone https://github.com/bitranox/rst_include.git
     $ cd rst_include
-    python setup.py install
+    python -m pip install -e .[test]
 
 - via makefile:
   makefiles are a very convenient way to install. Here we can do much more,
   like installing virtual environments, clean caches and so on.
 
 .. code-block:: shell
 
@@ -499,14 +485,34 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.1.3
+--------
+2023-07-21:
+    - require minimum python 3.8
+    - remove python 3.7 tests
+    - introduce PEP517 packaging standard
+    - introduce pyproject.toml build-system
+    - remove mypy.ini
+    - remove pytest.ini
+    - remove setup.cfg
+    - remove setup.py
+    - remove .bettercodehub.yml
+    - remove .travis.yml
+    - update black config
+    - clean ./tests/test_cli.py
+    - add codeql badge
+    - move 3rd_party_stubs outside the src directory to ``./.3rd_party_stubs``
+    - add pypy 3.10 tests
+    - add python 3.12-dev tests
+
 v2.1.2.2
 --------
 2022-06-02: setup github actions v3, python3.10 test matrix
 
 v2.1.1
 --------
 2020-10-09: service release
@@ -599,9 +605,7 @@
 ---------
 2019-04-28: add empty line at the end of the assembled documentation, to be able to add CHANGES.rst with setup.py
 
 1.0.0
 ---------
 2019-04-19: Initial public release, PyPi Release
 
-
-
```

