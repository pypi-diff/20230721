# Comparing `tmp/lib_path-1.0.2.tar.gz` & `tmp/lib_path-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lib_path-1.0.2.tar", last modified: Fri Oct  9 14:04:23 2020, max compression
+gzip compressed data, was "lib_path-1.0.3.tar", last modified: Fri Jul 21 15:36:24 2023, max compression
```

## Comparing `lib_path-1.0.2.tar` & `lib_path-1.0.3.tar`

### file list

```diff
@@ -1,22 +1,102 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-09 14:04:22.000000 lib_path-1.0.2/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4135 2020-10-09 14:03:40.000000 lib_path-1.0.2/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-09 14:04:22.000000 lib_path-1.0.2/lib_path.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-10-09 14:04:22.000000 lib_path-1.0.2/lib_path.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)      405 2020-10-09 14:04:22.000000 lib_path-1.0.2/lib_path.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       61 2020-10-09 14:04:22.000000 lib_path-1.0.2/lib_path.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        9 2020-10-09 14:04:22.000000 lib_path-1.0.2/lib_path.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-10-09 14:04:22.000000 lib_path-1.0.2/lib_path.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       13 2020-10-09 14:04:22.000000 lib_path-1.0.2/lib_path.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    10105 2020-10-09 14:04:22.000000 lib_path-1.0.2/lib_path.egg-info/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-09 14:04:22.000000 lib_path-1.0.2/lib_path/
--rw-rw-r--   0 travis    (2000) travis    (2000)    13681 2020-10-09 14:03:40.000000 lib_path-1.0.2/lib_path/lib_path.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-09 14:03:40.000000 lib_path-1.0.2/lib_path/py.typed
--rw-rw-r--   0 travis    (2000) travis    (2000)     1603 2020-10-09 14:03:40.000000 lib_path-1.0.2/lib_path/lib_path_cli.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      458 2020-10-09 14:03:40.000000 lib_path-1.0.2/lib_path/__init__conf__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      329 2020-10-09 14:03:40.000000 lib_path-1.0.2/lib_path/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7416 2020-10-09 14:03:40.000000 lib_path-1.0.2/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)    10105 2020-10-09 14:04:23.000000 lib_path-1.0.2/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      124 2020-10-09 14:03:40.000000 lib_path-1.0.2/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)      592 2020-10-09 14:04:23.000000 lib_path-1.0.2/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      252 2020-10-09 14:03:40.000000 lib_path-1.0.2/pyproject.toml
--rw-rw-r--   0 travis    (2000) travis    (2000)      337 2020-10-09 14:03:40.000000 lib_path-1.0.2/CHANGES.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:36:24.923353 lib_path-1.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:36:24.911353 lib_path-1.0.3/.3rd_party_stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-21 15:35:38.000000 lib_path-1.0.3/.3rd_party_stubs/readme.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-21 15:35:38.000000 lib_path-1.0.3/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:36:24.915353 lib_path-1.0.3/.docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-21 15:35:38.000000 lib_path-1.0.3/.docs/README_template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-21 15:35:38.000000 lib_path-1.0.3/.docs/acknowledgment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-21 15:35:38.000000 lib_path-1.0.3/.docs/badges.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-21 15:35:38.000000 lib_path-1.0.3/.docs/commandline_help.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-21 15:35:38.000000 lib_path-1.0.3/.docs/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-21 15:35:38.000000 lib_path-1.0.3/.docs/description.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-21 15:35:38.000000 lib_path-1.0.3/.docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-21 15:35:38.000000 lib_path-1.0.3/.docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-21 15:35:38.000000 lib_path-1.0.3/.docs/installation_via_makefile.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-21 15:35:38.000000 lib_path-1.0.3/.docs/installation_via_pypi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-21 15:35:38.000000 lib_path-1.0.3/.docs/licence_mit.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-21 15:35:38.000000 lib_path-1.0.3/.docs/rst_include_help_include_output.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 15:35:38.000000 lib_path-1.0.3/.docs/rst_include_help_output.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-21 15:35:38.000000 lib_path-1.0.3/.docs/rst_include_help_replace_output.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-07-21 15:35:38.000000 lib_path-1.0.3/.docs/rst_include_parameters.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-21 15:35:38.000000 lib_path-1.0.3/.docs/tested_under.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-21 15:35:38.000000 lib_path-1.0.3/.docs/try_in_jupyter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-21 15:35:38.000000 lib_path-1.0.3/.docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-21 15:35:38.000000 lib_path-1.0.3/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:36:24.903353 lib_path-1.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:36:24.915353 lib_path-1.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-21 15:35:38.000000 lib_path-1.0.3/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-07-21 15:35:38.000000 lib_path-1.0.3/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-21 15:35:38.000000 lib_path-1.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-21 15:35:38.000000 lib_path-1.0.3/.rotekignore
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-21 15:35:38.000000 lib_path-1.0.3/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-21 15:35:38.000000 lib_path-1.0.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-21 15:35:38.000000 lib_path-1.0.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-21 15:35:38.000000 lib_path-1.0.3/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-21 15:35:38.000000 lib_path-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-21 15:35:38.000000 lib_path-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-21 15:35:38.000000 lib_path-1.0.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-07-21 15:36:24.923353 lib_path-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-21 15:35:38.000000 lib_path-1.0.3/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-07-21 15:35:38.000000 lib_path-1.0.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-21 15:35:38.000000 lib_path-1.0.3/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:36:24.915353 lib_path-1.0.3/lib_path/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-21 15:35:38.000000 lib_path-1.0.3/lib_path/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-21 15:35:38.000000 lib_path-1.0.3/lib_path/__init__conf__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13555 2023-07-21 15:35:38.000000 lib_path-1.0.3/lib_path/lib_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-07-21 15:35:38.000000 lib_path-1.0.3/lib_path/lib_path_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 15:35:38.000000 lib_path-1.0.3/lib_path/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:36:24.919353 lib_path-1.0.3/lib_path.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-07-21 15:36:24.000000 lib_path-1.0.3/lib_path.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-21 15:36:24.000000 lib_path-1.0.3/lib_path.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 15:36:24.000000 lib_path-1.0.3/lib_path.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-21 15:36:24.000000 lib_path-1.0.3/lib_path.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-21 15:36:24.000000 lib_path-1.0.3/lib_path.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 15:36:24.000000 lib_path-1.0.3/lib_path.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-21 15:35:38.000000 lib_path-1.0.3/lib_path.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-21 15:35:38.000000 lib_path-1.0.3/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-07-21 15:35:38.000000 lib_path-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-21 15:35:38.000000 lib_path-1.0.3/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-21 15:35:38.000000 lib_path-1.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-21 15:35:38.000000 lib_path-1.0.3/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 15:36:24.927353 lib_path-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:36:24.919353 lib_path-1.0.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:36:24.907353 lib_path-1.0.3/tests/dir_with_subdirs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:36:24.919353 lib_path-1.0.3/tests/dir_with_subdirs/subdir/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 15:35:38.000000 lib_path-1.0.3/tests/dir_with_subdirs/subdir/test.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:36:24.919353 lib_path-1.0.3/tests/dir_without_subdirs/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 15:35:38.000000 lib_path-1.0.3/tests/dir_without_subdirs/test.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:36:24.919353 lib_path-1.0.3/tests/local_testscripts/
+-rwxrwxrwx   0 runner    (1001) docker     (123)     9552 2023-07-21 15:35:38.000000 lib_path-1.0.3/tests/local_testscripts/lib_bash_functions.sh
+-rwxrwxrwx   0 runner    (1001) docker     (123)      254 2023-07-21 15:35:38.000000 lib_path-1.0.3/tests/local_testscripts/run_clean.sh
+-rwxrwxrwx   0 runner    (1001) docker     (123)     1065 2023-07-21 15:35:38.000000 lib_path-1.0.3/tests/local_testscripts/run_pytest.sh
+-rwxrwxrwx   0 runner    (1001) docker     (123)     1842 2023-07-21 15:35:38.000000 lib_path-1.0.3/tests/local_testscripts/run_testloop.sh
+-rwxrwxrwx   0 runner    (1001) docker     (123)     1806 2023-07-21 15:35:38.000000 lib_path-1.0.3/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh
+-rwxrwxrwx   0 runner    (1001) docker     (123)      878 2023-07-21 15:35:38.000000 lib_path-1.0.3/tests/local_testscripts/run_testloop_windows.cmd
+-rwxrwxrwx   0 runner    (1001) docker     (123)     1515 2023-07-21 15:35:38.000000 lib_path-1.0.3/tests/local_testscripts/shellcheck.sh
+-rwxrwxrwx   0 runner    (1001) docker     (123)     5620 2023-07-21 15:35:38.000000 lib_path-1.0.3/tests/local_testscripts/testing_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:36:24.919353 lib_path-1.0.3/tests/test_a/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 15:35:38.000000 lib_path-1.0.3/tests/test_a/.file_test_a_1.txt
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 15:35:38.000000 lib_path-1.0.3/tests/test_a/.file_test_a_2.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:36:24.923353 lib_path-1.0.3/tests/test_a/.test_a_a/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 15:35:38.000000 lib_path-1.0.3/tests/test_a/.test_a_a/.file_test_a_a_1.txt
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 15:35:38.000000 lib_path-1.0.3/tests/test_a/.test_a_a/.file_test_a_a_2.txt
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 15:35:38.000000 lib_path-1.0.3/tests/test_a/.test_a_a/file_test_a_a_1.txt
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 15:35:38.000000 lib_path-1.0.3/tests/test_a/.test_a_a/file_test_a_a_2.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:36:24.923353 lib_path-1.0.3/tests/test_a/.test_a_b/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 15:35:38.000000 lib_path-1.0.3/tests/test_a/.test_a_b/.file_test_a_b_1.txt
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 15:35:38.000000 lib_path-1.0.3/tests/test_a/.test_a_b/.file_test_a_b_2.txt
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 15:35:38.000000 lib_path-1.0.3/tests/test_a/.test_a_b/file_test_a_b_1.txt
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 15:35:38.000000 lib_path-1.0.3/tests/test_a/.test_a_b/file_test_a_b_2.txt
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 15:35:38.000000 lib_path-1.0.3/tests/test_a/file_test_a_1.txt
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 15:35:38.000000 lib_path-1.0.3/tests/test_a/file_test_a_2.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:36:24.923353 lib_path-1.0.3/tests/test_a/test_a_a/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 15:35:38.000000 lib_path-1.0.3/tests/test_a/test_a_a/.file_test_a_a_1.txt
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 15:35:38.000000 lib_path-1.0.3/tests/test_a/test_a_a/.file_test_a_a_2.txt
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 15:35:38.000000 lib_path-1.0.3/tests/test_a/test_a_a/file_test_a_a_1.txt
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 15:35:38.000000 lib_path-1.0.3/tests/test_a/test_a_a/file_test_a_a_2.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:36:24.923353 lib_path-1.0.3/tests/test_a/test_a_b/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 15:35:38.000000 lib_path-1.0.3/tests/test_a/test_a_b/.file_test_a_b_1.txt
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 15:35:38.000000 lib_path-1.0.3/tests/test_a/test_a_b/.file_test_a_b_2.txt
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 15:35:38.000000 lib_path-1.0.3/tests/test_a/test_a_b/file_test_a_b_1.txt
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 15:35:38.000000 lib_path-1.0.3/tests/test_a/test_a_b/file_test_a_b_2.txt
+-rwxrwxrwx   0 runner    (1001) docker     (123)      784 2023-07-21 15:35:38.000000 lib_path-1.0.3/tests/test_cli.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `lib_path-1.0.2/lib_path/lib_path.py` & `lib_path-1.0.3/lib_path/lib_path.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     >>> # Test Raise
     >>> log_and_raise_if_path_does_not_exist(test_non_existing)
     Traceback (most recent call last):
     ...
     FileNotFoundError: path does not exist: does_not_exist
     """
     if not path.exists():
-        s_error = 'path does not exist: {path}'.format(path=path)
+        s_error = f'path does not exist: {path}'
         logger.error(s_error)
         raise FileNotFoundError(s_error)
 
 
 def log_and_raise_if_not_isdir(path_dir: pathlib.Path) -> None:
     """
     >>> # SETUP
@@ -60,15 +60,15 @@
     Traceback (most recent call last):
     ...
     NotADirectoryError: not a directory : does_not_exist
 
     """
 
     if not path_dir.is_dir():
-        s_error = 'not a directory : {path_dir}'.format(path_dir=path_dir)
+        s_error = f'not a directory : {path_dir}'
         logger.error(s_error)
         raise NotADirectoryError(s_error)
 
 
 def log_and_raise_if_target_directory_within_source_directory(path_source_dir: pathlib.Path, path_target_dir: pathlib.Path) -> None:
     """
     >>> # Setup
@@ -83,15 +83,15 @@
     >>> log_and_raise_if_target_directory_within_source_directory(path_source_dir, path_target_dir_err)
     Traceback (most recent call last):
     ...
     FileExistsError: target directory: "..." is within the source directory "..."
 
     """
     if is_target_directory_within_source_directory(path_source_dir, path_target_dir):
-        s_error = 'target directory: "{}" is within the source directory "{}"'.format(path_target_dir, path_source_dir)
+        s_error = f'target directory: "{path_target_dir}" is within the source directory "{path_source_dir}"'
         logger.error(s_error)
         raise FileExistsError(s_error)
 
 
 def is_target_directory_within_source_directory(path_source_dir: pathlib.Path, path_target_dir: pathlib.Path) -> bool:
     s_source_dir = str(path_source_dir.resolve()).replace('\\', '/') + '/'
     s_target_dir = str(path_target_dir.resolve()).replace('\\', '/') + '/'
@@ -113,15 +113,15 @@
     >>> # TEST ERR
     >>> log_and_raise_if_not_isfile(path_file_err)
     Traceback (most recent call last):
     ...
     FileNotFoundError: file does not exist or no permission: does_not_exist
     """
     if not path_file.is_file():
-        s_error = 'file does not exist or no permission: {path_file}'.format(path_file=path_file)
+        s_error = f'file does not exist or no permission: {path_file}'
         logger.error(s_error)
         raise FileNotFoundError(s_error)
 
 
 def path_join_posix(path: str, *paths: str) -> str:
     """
     liefert beim joinen einen Pfad jedenfalls als posix pfad retour.
@@ -397,15 +397,15 @@
     path_origin_resolved_directory = path_origin_directory.resolve()
     # for doctest under pycharm, we need to go probably some levels up:
     root_directory = pathlib.Path('/')
     while True:
         if (path_origin_resolved_directory / test_directory_name).is_dir():
             break
         if path_origin_resolved_directory == root_directory:
-            raise FileNotFoundError('test directory "{test_directory_name}" not found'.format(test_directory_name=test_directory_name))
+            raise FileNotFoundError(f'test directory "{test_directory_name}" not found')
         path_origin_resolved_directory = path_origin_resolved_directory.parent
     path_to_test_directory = path_origin_resolved_directory / test_directory_name
     return path_to_test_directory
 
 
 def make_test_directory_and_subdirs_fully_accessible_by_current_user(path_directory_name: Union[str, pathlib.Path]) -> None:
     """ Linux only, Change Mask to 777 for all Files and change Owner and Group to the current user
```

### Comparing `lib_path-1.0.2/lib_path/lib_path_cli.py` & `lib_path-1.0.3/lib_path/lib_path_cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,18 +26,18 @@
     >>> info()
     Info for ...
 
     """
     __init__conf__.print_info()
 
 
-@click.group(help=__init__conf__.title, context_settings=CLICK_CONTEXT_SETTINGS)
+@click.group(help=__init__conf__.title, context_settings=CLICK_CONTEXT_SETTINGS)    # type: ignore
 @click.version_option(version=__init__conf__.version,
                       prog_name=__init__conf__.shell_command,
-                      message='{} version %(version)s'.format(__init__conf__.shell_command))
+                      message=f'{__init__conf__.shell_command} version {__init__conf__.version}')
 @click.option('--traceback/--no-traceback', is_flag=True, type=bool, default=None, help='return traceback information on cli')
 def cli_main(traceback: Optional[bool] = None) -> None:
     if traceback is not None:
         cli_exit_tools.config.traceback = traceback
         # lib_path.main() # there is no main in lib_path
 
 
@@ -46,13 +46,13 @@
     """ get program informations """
     info()
 
 
 # entry point if main
 if __name__ == '__main__':
     try:
-        cli_main()
+        cli_main()  # type: ignore
     except Exception as exc:
         cli_exit_tools.print_exception_message()
         sys.exit(cli_exit_tools.get_system_exit_code(exc))
     finally:
         cli_exit_tools.flush_streams()
```

### Comparing `lib_path-1.0.2/README.rst` & `lib_path-1.0.3/lib_path.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,69 +1,96 @@
+Metadata-Version: 2.1
+Name: lib-path
+Version: 1.0.3
+Summary: path related function - deprecated
+Author-email: Robert Nowotny <bitranox@gmail.com>
+License: MIT
+Project-URL: Homepage, https://github.com/bitranox/lib_path
+Project-URL: Documentation, https://github.com/bitranox/lib_path/blob/master/README.rst
+Project-URL: Repository, https://github.com/bitranox/lib_path.git
+Project-URL: Changelog, https://github.com/bitranox/lib_path/blob/master/CHANGES.rst
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
 lib_path
 ========
 
 
-Version v1.0.2 as of 2020-10-09 see `Changelog`_
+Version v1.0.3 as of 2023-07-21 see `Changelog`_
+
+|build_badge| |codeql| |license| |jupyter| |pypi|
+|pypi-downloads| |black| |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+
 
-|travis_build| |license| |jupyter| |pypi|
 
-|codecov| |better_code| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+.. |build_badge| image:: https://github.com/bitranox/lib_path/actions/workflows/python-package.yml/badge.svg
+   :target: https://github.com/bitranox/lib_path/actions/workflows/python-package.yml
 
 
-.. |travis_build| image:: https://img.shields.io/travis/bitranox/lib_path/master.svg
-   :target: https://travis-ci.org/bitranox/lib_path
+.. |codeql| image:: https://github.com/bitranox/lib_path/actions/workflows/codeql-analysis.yml/badge.svg?event=push
+   :target: https://github.com//bitranox/lib_path/actions/workflows/codeql-analysis.yml
 
 .. |license| image:: https://img.shields.io/github/license/webcomics/pywine.svg
    :target: http://en.wikipedia.org/wiki/MIT_License
 
 .. |jupyter| image:: https://mybinder.org/badge_logo.svg
- :target: https://mybinder.org/v2/gh/bitranox/lib_path/master?filepath=lib_path.ipynb
+   :target: https://mybinder.org/v2/gh/bitranox/lib_path/master?filepath=lib_path.ipynb
 
 .. for the pypi status link note the dashes, not the underscore !
 .. |pypi| image:: https://img.shields.io/pypi/status/lib-path?label=PyPI%20Package
    :target: https://badge.fury.io/py/lib_path
 
 .. |codecov| image:: https://img.shields.io/codecov/c/github/bitranox/lib_path
    :target: https://codecov.io/gh/bitranox/lib_path
 
-.. |better_code| image:: https://bettercodehub.com/edge/badge/bitranox/lib_path?branch=master
-   :target: https://bettercodehub.com/results/bitranox/lib_path
-
 .. |cc_maintain| image:: https://img.shields.io/codeclimate/maintainability-percentage/bitranox/lib_path?label=CC%20maintainability
    :target: https://codeclimate.com/github/bitranox/lib_path/maintainability
    :alt: Maintainability
 
 .. |cc_issues| image:: https://img.shields.io/codeclimate/issues/bitranox/lib_path?label=CC%20issues
    :target: https://codeclimate.com/github/bitranox/lib_path/maintainability
    :alt: Maintainability
 
 .. |cc_coverage| image:: https://img.shields.io/codeclimate/coverage/bitranox/lib_path?label=CC%20coverage
    :target: https://codeclimate.com/github/bitranox/lib_path/test_coverage
    :alt: Code Coverage
 
-.. |snyk| image:: https://img.shields.io/snyk/vulnerabilities/github/bitranox/lib_path
+.. |snyk| image:: https://snyk.io/test/github/bitranox/lib_path/badge.svg
    :target: https://snyk.io/test/github/bitranox/lib_path
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
 
+.. |pypi-downloads| image:: https://img.shields.io/pypi/dm/lib-path
+   :target: https://pypi.org/project/lib-path/
+   :alt: PyPI - Downloads
+
 functions to handle string paths, were pathlib is not applicable.
 also works correctly with windows UNC Paths like //server/share/directory/../../directory2
 deprecated
 
 ----
 
-automated tests, Travis Matrix, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
+automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
-Python version required: 3.6.0 or newer
+Python version required: 3.8.0 or newer
 
-tested on linux "bionic" with python 3.6, 3.7, 3.8, 3.9-dev, pypy3 - architectures: amd64, ppc64le, s390x, arm64
+tested on recent linux with python 3.8, 3.9, 3.10, 3.11, 3.12-dev, pypy-3.9, pypy-3.10 - architectures: amd64
 
-`100% code coverage <https://codecov.io/gh/bitranox/lib_path>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://travis-ci.org/bitranox/lib_path>`_, automatic daily builds and monitoring
+`100% code coverage <https://codeclimate.com/github/bitranox/lib_path/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/lib_path/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
 - `Usage from Commandline`_
 - `Installation and Upgrade`_
@@ -116,15 +143,15 @@
     strip_and_replace_backslashes(path: str) -> str
 
     substract_windows_drive_letter(path: str) -> str
 
 Usage from Commandline
 ------------------------
 
-.. code-block:: bash
+.. code-block::
 
    Usage: lib_path [OPTIONS] COMMAND [ARGS]...
 
      path related function - deprecated
 
    Options:
      --version                     Show the version and exit.
@@ -136,56 +163,63 @@
 
 Installation and Upgrade
 ------------------------
 
 - Before You start, its highly recommended to update pip and setup tools:
 
 
-.. code-block:: bash
+.. code-block::
 
     python -m pip --upgrade pip
     python -m pip --upgrade setuptools
 
 - to install the latest release from PyPi via pip (recommended):
 
-.. code-block:: bash
+.. code-block::
 
     python -m pip install --upgrade lib_path
 
+
+- to install the latest release from PyPi via pip, including test dependencies:
+
+.. code-block::
+
+    python -m pip install --upgrade lib_path[test]
+
 - to install the latest version from github via pip:
 
 
-.. code-block:: bash
+.. code-block::
 
     python -m pip install --upgrade git+https://github.com/bitranox/lib_path.git
 
 
 - include it into Your requirements.txt:
 
-.. code-block:: bash
+.. code-block::
 
     # Insert following line in Your requirements.txt:
     # for the latest Release on pypi:
     lib_path
 
     # for the latest development version :
     lib_path @ git+https://github.com/bitranox/lib_path.git
 
     # to install and upgrade all modules mentioned in requirements.txt:
     python -m pip install --upgrade -r /<path>/requirements.txt
 
 
-- to install the latest development version from source code:
+- to install the latest development version, including test dependencies from source code:
 
-.. code-block:: bash
+.. code-block::
 
     # cd ~
     $ git clone https://github.com/bitranox/lib_path.git
     $ cd lib_path
-    python setup.py install
+    python -m pip install -e .[test]
 
 - via makefile:
   makefiles are a very convenient way to install. Here we can do much more,
   like installing virtual environments, clean caches and so on.
 
 .. code-block:: shell
 
@@ -208,15 +242,15 @@
 Requirements
 ------------
 following modules will be automatically installed :
 
 .. code-block:: bash
 
     ## Project Requirements
-    lib_platform @ git+https://github.com/bitranox/lib_platform.git
+    lib_platform
 
 Acknowledgements
 ----------------
 
 - special thanks to "uncle bob" Robert C. Martin, especially for his books on "clean code" and "clean architecture"
 
 Contribute
@@ -231,14 +265,34 @@
 This software is licensed under the `MIT license <http://en.wikipedia.org/wiki/MIT_License>`_
 
 ---
 
 Changelog
 =========
 
+v1.0.3
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
 v1.0.2
 --------
 2020-10-09: service release
     - update travis build matrix for linux 3.9-dev
     - update travis build matrix (paths) for windows 3.9 / 3.10
 
 1.0.1
```

