# Comparing `tmp/lib_path-1.0.3.tar.gz` & `tmp/lib_path-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib_path-1.0.3.tar", last modified: Fri Jul 21 15:36:24 2023, max compression
+gzip compressed data, was "lib_path-1.0.4.tar", last modified: Fri Jul 21 16:09:54 2023, max compression
```

## Comparing `lib_path-1.0.3.tar` & `lib_path-1.0.4.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:36:24.923353 lib_path-1.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:36:24.911353 lib_path-1.0.3/.3rd_party_stubs/
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-21 15:35:38.000000 lib_path-1.0.3/.3rd_party_stubs/readme.txt
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-21 15:35:38.000000 lib_path-1.0.3/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:36:24.915353 lib_path-1.0.3/.docs/
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-21 15:35:38.000000 lib_path-1.0.3/.docs/README_template.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-21 15:35:38.000000 lib_path-1.0.3/.docs/acknowledgment.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-21 15:35:38.000000 lib_path-1.0.3/.docs/badges.rst
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-21 15:35:38.000000 lib_path-1.0.3/.docs/commandline_help.rst
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-21 15:35:38.000000 lib_path-1.0.3/.docs/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-21 15:35:38.000000 lib_path-1.0.3/.docs/description.rst
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-21 15:35:38.000000 lib_path-1.0.3/.docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-21 15:35:38.000000 lib_path-1.0.3/.docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-21 15:35:38.000000 lib_path-1.0.3/.docs/installation_via_makefile.rst
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-21 15:35:38.000000 lib_path-1.0.3/.docs/installation_via_pypi.rst
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-21 15:35:38.000000 lib_path-1.0.3/.docs/licence_mit.rst
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-21 15:35:38.000000 lib_path-1.0.3/.docs/rst_include_help_include_output.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 15:35:38.000000 lib_path-1.0.3/.docs/rst_include_help_output.txt
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-21 15:35:38.000000 lib_path-1.0.3/.docs/rst_include_help_replace_output.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-07-21 15:35:38.000000 lib_path-1.0.3/.docs/rst_include_parameters.rst
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-21 15:35:38.000000 lib_path-1.0.3/.docs/tested_under.rst
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-21 15:35:38.000000 lib_path-1.0.3/.docs/try_in_jupyter.rst
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-21 15:35:38.000000 lib_path-1.0.3/.docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-21 15:35:38.000000 lib_path-1.0.3/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:36:24.903353 lib_path-1.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:36:24.915353 lib_path-1.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-21 15:35:38.000000 lib_path-1.0.3/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-07-21 15:35:38.000000 lib_path-1.0.3/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-21 15:35:38.000000 lib_path-1.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-21 15:35:38.000000 lib_path-1.0.3/.rotekignore
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-21 15:35:38.000000 lib_path-1.0.3/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-21 15:35:38.000000 lib_path-1.0.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-21 15:35:38.000000 lib_path-1.0.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-21 15:35:38.000000 lib_path-1.0.3/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-21 15:35:38.000000 lib_path-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-21 15:35:38.000000 lib_path-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-21 15:35:38.000000 lib_path-1.0.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-07-21 15:36:24.923353 lib_path-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-21 15:35:38.000000 lib_path-1.0.3/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-07-21 15:35:38.000000 lib_path-1.0.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-21 15:35:38.000000 lib_path-1.0.3/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:36:24.915353 lib_path-1.0.3/lib_path/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-21 15:35:38.000000 lib_path-1.0.3/lib_path/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-21 15:35:38.000000 lib_path-1.0.3/lib_path/__init__conf__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13555 2023-07-21 15:35:38.000000 lib_path-1.0.3/lib_path/lib_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-07-21 15:35:38.000000 lib_path-1.0.3/lib_path/lib_path_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 15:35:38.000000 lib_path-1.0.3/lib_path/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:36:24.919353 lib_path-1.0.3/lib_path.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-07-21 15:36:24.000000 lib_path-1.0.3/lib_path.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-21 15:36:24.000000 lib_path-1.0.3/lib_path.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 15:36:24.000000 lib_path-1.0.3/lib_path.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-21 15:36:24.000000 lib_path-1.0.3/lib_path.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-21 15:36:24.000000 lib_path-1.0.3/lib_path.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 15:36:24.000000 lib_path-1.0.3/lib_path.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-21 15:35:38.000000 lib_path-1.0.3/lib_path.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-21 15:35:38.000000 lib_path-1.0.3/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-07-21 15:35:38.000000 lib_path-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-21 15:35:38.000000 lib_path-1.0.3/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-21 15:35:38.000000 lib_path-1.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-21 15:35:38.000000 lib_path-1.0.3/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 15:36:24.927353 lib_path-1.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:36:24.919353 lib_path-1.0.3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:36:24.907353 lib_path-1.0.3/tests/dir_with_subdirs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:36:24.919353 lib_path-1.0.3/tests/dir_with_subdirs/subdir/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 15:35:38.000000 lib_path-1.0.3/tests/dir_with_subdirs/subdir/test.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:36:24.919353 lib_path-1.0.3/tests/dir_without_subdirs/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 15:35:38.000000 lib_path-1.0.3/tests/dir_without_subdirs/test.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:36:24.919353 lib_path-1.0.3/tests/local_testscripts/
--rwxrwxrwx   0 runner    (1001) docker     (123)     9552 2023-07-21 15:35:38.000000 lib_path-1.0.3/tests/local_testscripts/lib_bash_functions.sh
--rwxrwxrwx   0 runner    (1001) docker     (123)      254 2023-07-21 15:35:38.000000 lib_path-1.0.3/tests/local_testscripts/run_clean.sh
--rwxrwxrwx   0 runner    (1001) docker     (123)     1065 2023-07-21 15:35:38.000000 lib_path-1.0.3/tests/local_testscripts/run_pytest.sh
--rwxrwxrwx   0 runner    (1001) docker     (123)     1842 2023-07-21 15:35:38.000000 lib_path-1.0.3/tests/local_testscripts/run_testloop.sh
--rwxrwxrwx   0 runner    (1001) docker     (123)     1806 2023-07-21 15:35:38.000000 lib_path-1.0.3/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh
--rwxrwxrwx   0 runner    (1001) docker     (123)      878 2023-07-21 15:35:38.000000 lib_path-1.0.3/tests/local_testscripts/run_testloop_windows.cmd
--rwxrwxrwx   0 runner    (1001) docker     (123)     1515 2023-07-21 15:35:38.000000 lib_path-1.0.3/tests/local_testscripts/shellcheck.sh
--rwxrwxrwx   0 runner    (1001) docker     (123)     5620 2023-07-21 15:35:38.000000 lib_path-1.0.3/tests/local_testscripts/testing_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:36:24.919353 lib_path-1.0.3/tests/test_a/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 15:35:38.000000 lib_path-1.0.3/tests/test_a/.file_test_a_1.txt
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 15:35:38.000000 lib_path-1.0.3/tests/test_a/.file_test_a_2.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:36:24.923353 lib_path-1.0.3/tests/test_a/.test_a_a/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 15:35:38.000000 lib_path-1.0.3/tests/test_a/.test_a_a/.file_test_a_a_1.txt
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 15:35:38.000000 lib_path-1.0.3/tests/test_a/.test_a_a/.file_test_a_a_2.txt
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 15:35:38.000000 lib_path-1.0.3/tests/test_a/.test_a_a/file_test_a_a_1.txt
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 15:35:38.000000 lib_path-1.0.3/tests/test_a/.test_a_a/file_test_a_a_2.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:36:24.923353 lib_path-1.0.3/tests/test_a/.test_a_b/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 15:35:38.000000 lib_path-1.0.3/tests/test_a/.test_a_b/.file_test_a_b_1.txt
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 15:35:38.000000 lib_path-1.0.3/tests/test_a/.test_a_b/.file_test_a_b_2.txt
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 15:35:38.000000 lib_path-1.0.3/tests/test_a/.test_a_b/file_test_a_b_1.txt
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 15:35:38.000000 lib_path-1.0.3/tests/test_a/.test_a_b/file_test_a_b_2.txt
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 15:35:38.000000 lib_path-1.0.3/tests/test_a/file_test_a_1.txt
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 15:35:38.000000 lib_path-1.0.3/tests/test_a/file_test_a_2.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:36:24.923353 lib_path-1.0.3/tests/test_a/test_a_a/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 15:35:38.000000 lib_path-1.0.3/tests/test_a/test_a_a/.file_test_a_a_1.txt
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 15:35:38.000000 lib_path-1.0.3/tests/test_a/test_a_a/.file_test_a_a_2.txt
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 15:35:38.000000 lib_path-1.0.3/tests/test_a/test_a_a/file_test_a_a_1.txt
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 15:35:38.000000 lib_path-1.0.3/tests/test_a/test_a_a/file_test_a_a_2.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:36:24.923353 lib_path-1.0.3/tests/test_a/test_a_b/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 15:35:38.000000 lib_path-1.0.3/tests/test_a/test_a_b/.file_test_a_b_1.txt
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 15:35:38.000000 lib_path-1.0.3/tests/test_a/test_a_b/.file_test_a_b_2.txt
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 15:35:38.000000 lib_path-1.0.3/tests/test_a/test_a_b/file_test_a_b_1.txt
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 15:35:38.000000 lib_path-1.0.3/tests/test_a/test_a_b/file_test_a_b_2.txt
--rwxrwxrwx   0 runner    (1001) docker     (123)      784 2023-07-21 15:35:38.000000 lib_path-1.0.3/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:09:54.106176 lib_path-1.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:09:54.098175 lib_path-1.0.4/.3rd_party_stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-21 16:09:07.000000 lib_path-1.0.4/.3rd_party_stubs/readme.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-21 16:09:07.000000 lib_path-1.0.4/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:09:54.098175 lib_path-1.0.4/.docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-21 16:09:07.000000 lib_path-1.0.4/.docs/README_template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-21 16:09:07.000000 lib_path-1.0.4/.docs/acknowledgment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-21 16:09:07.000000 lib_path-1.0.4/.docs/badges.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-21 16:09:07.000000 lib_path-1.0.4/.docs/commandline_help.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-21 16:09:07.000000 lib_path-1.0.4/.docs/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-21 16:09:07.000000 lib_path-1.0.4/.docs/description.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-21 16:09:07.000000 lib_path-1.0.4/.docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-21 16:09:07.000000 lib_path-1.0.4/.docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-21 16:09:07.000000 lib_path-1.0.4/.docs/installation_via_makefile.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-21 16:09:07.000000 lib_path-1.0.4/.docs/installation_via_pypi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-21 16:09:07.000000 lib_path-1.0.4/.docs/licence_mit.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-21 16:09:07.000000 lib_path-1.0.4/.docs/rst_include_help_include_output.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:09:07.000000 lib_path-1.0.4/.docs/rst_include_help_output.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-21 16:09:07.000000 lib_path-1.0.4/.docs/rst_include_help_replace_output.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-07-21 16:09:07.000000 lib_path-1.0.4/.docs/rst_include_parameters.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-21 16:09:07.000000 lib_path-1.0.4/.docs/tested_under.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-21 16:09:07.000000 lib_path-1.0.4/.docs/try_in_jupyter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-21 16:09:07.000000 lib_path-1.0.4/.docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-21 16:09:07.000000 lib_path-1.0.4/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:09:54.094175 lib_path-1.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:09:54.098175 lib_path-1.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-21 16:09:07.000000 lib_path-1.0.4/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-07-21 16:09:07.000000 lib_path-1.0.4/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-21 16:09:07.000000 lib_path-1.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-21 16:09:07.000000 lib_path-1.0.4/.rotekignore
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-21 16:09:07.000000 lib_path-1.0.4/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-21 16:09:07.000000 lib_path-1.0.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-21 16:09:07.000000 lib_path-1.0.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-21 16:09:07.000000 lib_path-1.0.4/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-21 16:09:07.000000 lib_path-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-21 16:09:07.000000 lib_path-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-21 16:09:07.000000 lib_path-1.0.4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     9393 2023-07-21 16:09:54.106176 lib_path-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-21 16:09:07.000000 lib_path-1.0.4/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8475 2023-07-21 16:09:07.000000 lib_path-1.0.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-21 16:09:07.000000 lib_path-1.0.4/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:09:54.102175 lib_path-1.0.4/lib_path/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-21 16:09:07.000000 lib_path-1.0.4/lib_path/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-21 16:09:07.000000 lib_path-1.0.4/lib_path/__init__conf__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13555 2023-07-21 16:09:07.000000 lib_path-1.0.4/lib_path/lib_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-07-21 16:09:07.000000 lib_path-1.0.4/lib_path/lib_path_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:09:07.000000 lib_path-1.0.4/lib_path/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:09:54.102175 lib_path-1.0.4/lib_path.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9393 2023-07-21 16:09:54.000000 lib_path-1.0.4/lib_path.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-21 16:09:54.000000 lib_path-1.0.4/lib_path.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 16:09:54.000000 lib_path-1.0.4/lib_path.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-21 16:09:54.000000 lib_path-1.0.4/lib_path.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-21 16:09:54.000000 lib_path-1.0.4/lib_path.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 16:09:54.000000 lib_path-1.0.4/lib_path.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-21 16:09:07.000000 lib_path-1.0.4/lib_path.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-21 16:09:07.000000 lib_path-1.0.4/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-07-21 16:09:07.000000 lib_path-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-21 16:09:07.000000 lib_path-1.0.4/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-21 16:09:07.000000 lib_path-1.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-21 16:09:07.000000 lib_path-1.0.4/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 16:09:54.106176 lib_path-1.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:09:54.102175 lib_path-1.0.4/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:09:54.094175 lib_path-1.0.4/tests/dir_with_subdirs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:09:54.102175 lib_path-1.0.4/tests/dir_with_subdirs/subdir/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 16:09:07.000000 lib_path-1.0.4/tests/dir_with_subdirs/subdir/test.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:09:54.102175 lib_path-1.0.4/tests/dir_without_subdirs/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 16:09:07.000000 lib_path-1.0.4/tests/dir_without_subdirs/test.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:09:54.102175 lib_path-1.0.4/tests/local_testscripts/
+-rwxrwxrwx   0 runner    (1001) docker     (123)     9552 2023-07-21 16:09:07.000000 lib_path-1.0.4/tests/local_testscripts/lib_bash_functions.sh
+-rwxrwxrwx   0 runner    (1001) docker     (123)      254 2023-07-21 16:09:07.000000 lib_path-1.0.4/tests/local_testscripts/run_clean.sh
+-rwxrwxrwx   0 runner    (1001) docker     (123)     1065 2023-07-21 16:09:07.000000 lib_path-1.0.4/tests/local_testscripts/run_pytest.sh
+-rwxrwxrwx   0 runner    (1001) docker     (123)     1842 2023-07-21 16:09:07.000000 lib_path-1.0.4/tests/local_testscripts/run_testloop.sh
+-rwxrwxrwx   0 runner    (1001) docker     (123)     1806 2023-07-21 16:09:07.000000 lib_path-1.0.4/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh
+-rwxrwxrwx   0 runner    (1001) docker     (123)      878 2023-07-21 16:09:07.000000 lib_path-1.0.4/tests/local_testscripts/run_testloop_windows.cmd
+-rwxrwxrwx   0 runner    (1001) docker     (123)     1515 2023-07-21 16:09:07.000000 lib_path-1.0.4/tests/local_testscripts/shellcheck.sh
+-rwxrwxrwx   0 runner    (1001) docker     (123)     5620 2023-07-21 16:09:07.000000 lib_path-1.0.4/tests/local_testscripts/testing_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:09:54.102175 lib_path-1.0.4/tests/test_a/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 16:09:07.000000 lib_path-1.0.4/tests/test_a/.file_test_a_1.txt
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 16:09:07.000000 lib_path-1.0.4/tests/test_a/.file_test_a_2.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:09:54.102175 lib_path-1.0.4/tests/test_a/.test_a_a/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 16:09:07.000000 lib_path-1.0.4/tests/test_a/.test_a_a/.file_test_a_a_1.txt
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 16:09:07.000000 lib_path-1.0.4/tests/test_a/.test_a_a/.file_test_a_a_2.txt
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 16:09:07.000000 lib_path-1.0.4/tests/test_a/.test_a_a/file_test_a_a_1.txt
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 16:09:07.000000 lib_path-1.0.4/tests/test_a/.test_a_a/file_test_a_a_2.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:09:54.102175 lib_path-1.0.4/tests/test_a/.test_a_b/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 16:09:07.000000 lib_path-1.0.4/tests/test_a/.test_a_b/.file_test_a_b_1.txt
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 16:09:07.000000 lib_path-1.0.4/tests/test_a/.test_a_b/.file_test_a_b_2.txt
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 16:09:07.000000 lib_path-1.0.4/tests/test_a/.test_a_b/file_test_a_b_1.txt
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 16:09:07.000000 lib_path-1.0.4/tests/test_a/.test_a_b/file_test_a_b_2.txt
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 16:09:07.000000 lib_path-1.0.4/tests/test_a/file_test_a_1.txt
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 16:09:07.000000 lib_path-1.0.4/tests/test_a/file_test_a_2.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:09:54.106176 lib_path-1.0.4/tests/test_a/test_a_a/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 16:09:07.000000 lib_path-1.0.4/tests/test_a/test_a_a/.file_test_a_a_1.txt
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 16:09:07.000000 lib_path-1.0.4/tests/test_a/test_a_a/.file_test_a_a_2.txt
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 16:09:07.000000 lib_path-1.0.4/tests/test_a/test_a_a/file_test_a_a_1.txt
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 16:09:07.000000 lib_path-1.0.4/tests/test_a/test_a_a/file_test_a_a_2.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:09:54.106176 lib_path-1.0.4/tests/test_a/test_a_b/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 16:09:07.000000 lib_path-1.0.4/tests/test_a/test_a_b/.file_test_a_b_1.txt
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 16:09:07.000000 lib_path-1.0.4/tests/test_a/test_a_b/.file_test_a_b_2.txt
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 16:09:07.000000 lib_path-1.0.4/tests/test_a/test_a_b/file_test_a_b_1.txt
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-21 16:09:07.000000 lib_path-1.0.4/tests/test_a/test_a_b/file_test_a_b_2.txt
+-rwxrwxrwx   0 runner    (1001) docker     (123)      784 2023-07-21 16:09:07.000000 lib_path-1.0.4/tests/test_cli.py
```

### Comparing `lib_path-1.0.3/.3rd_party_stubs/readme.txt` & `lib_path-1.0.4/.3rd_party_stubs/readme.txt`

 * *Files identical despite different names*

### Comparing `lib_path-1.0.3/.coveragerc` & `lib_path-1.0.4/.coveragerc`

 * *Files identical despite different names*

### Comparing `lib_path-1.0.3/.docs/README_template.rst` & `lib_path-1.0.4/.docs/README_template.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 lib_path
 ========
 
 
-Version v1.0.3 as of 2023-07-21 see `Changelog`_
+Version v1.0.4 as of 2023-07-21 see `Changelog`_
 
 
 .. include:: ./badges.rst
 
 .. include:: ./description.rst
 
 ----
```

### Comparing `lib_path-1.0.3/.docs/badges.rst` & `lib_path-1.0.4/.docs/badges.rst`

 * *Files identical despite different names*

### Comparing `lib_path-1.0.3/.docs/installation.rst` & `lib_path-1.0.4/.docs/installation.rst`

 * *Files identical despite different names*

### Comparing `lib_path-1.0.3/.docs/rst_include_help_include_output.txt` & `lib_path-1.0.4/.docs/rst_include_help_include_output.txt`

 * *Files identical despite different names*

### Comparing `lib_path-1.0.3/.docs/rst_include_help_replace_output.txt` & `lib_path-1.0.4/.docs/rst_include_help_replace_output.txt`

 * *Files identical despite different names*

### Comparing `lib_path-1.0.3/.docs/rst_include_parameters.rst` & `lib_path-1.0.4/.docs/rst_include_parameters.rst`

 * *Files identical despite different names*

### Comparing `lib_path-1.0.3/.docs/usage.rst` & `lib_path-1.0.4/.docs/usage.rst`

 * *Files identical despite different names*

### Comparing `lib_path-1.0.3/.github/workflows/codeql-analysis.yml` & `lib_path-1.0.4/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `lib_path-1.0.3/.github/workflows/python-package.yml` & `lib_path-1.0.4/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `lib_path-1.0.3/.gitignore` & `lib_path-1.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `lib_path-1.0.3/.rotekignore` & `lib_path-1.0.4/.rotekignore`

 * *Files identical despite different names*

### Comparing `lib_path-1.0.3/CHANGES.rst` & `lib_path-1.0.4/CHANGES.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Changelog
 =========
 
+v1.0.4
+--------
+2023-07-21:
+    - update requirements
+
 v1.0.3
 --------
 2023-07-21:
     - require minimum python 3.8
     - remove python 3.7 tests
     - introduce PEP517 packaging standard
     - introduce pyproject.toml build-system
```

### Comparing `lib_path-1.0.3/CODE_OF_CONDUCT.md` & `lib_path-1.0.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `lib_path-1.0.3/CONTRIBUTING.md` & `lib_path-1.0.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `lib_path-1.0.3/ISSUE_TEMPLATE.md` & `lib_path-1.0.4/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `lib_path-1.0.3/LICENSE` & `lib_path-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lib_path-1.0.3/Makefile` & `lib_path-1.0.4/Makefile`

 * *Files identical despite different names*

### Comparing `lib_path-1.0.3/PKG-INFO` & `lib_path-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib_path
-Version: 1.0.3
+Version: 1.0.4
 Summary: path related function - deprecated
 Author-email: Robert Nowotny <bitranox@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/bitranox/lib_path
 Project-URL: Documentation, https://github.com/bitranox/lib_path/blob/master/README.rst
 Project-URL: Repository, https://github.com/bitranox/lib_path.git
 Project-URL: Changelog, https://github.com/bitranox/lib_path/blob/master/CHANGES.rst
@@ -20,15 +20,15 @@
 Provides-Extra: test
 License-File: LICENSE
 
 lib_path
 ========
 
 
-Version v1.0.3 as of 2023-07-21 see `Changelog`_
+Version v1.0.4 as of 2023-07-21 see `Changelog`_
 
 |build_badge| |codeql| |license| |jupyter| |pypi|
 |pypi-downloads| |black| |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/lib_path/actions/workflows/python-package.yml/badge.svg
@@ -242,14 +242,16 @@
 Requirements
 ------------
 following modules will be automatically installed :
 
 .. code-block:: bash
 
     ## Project Requirements
+    cli_exit_tools
+    lib_detect_testenv
     lib_platform
 
 Acknowledgements
 ----------------
 
 - special thanks to "uncle bob" Robert C. Martin, especially for his books on "clean code" and "clean architecture"
 
@@ -265,14 +267,19 @@
 This software is licensed under the `MIT license <http://en.wikipedia.org/wiki/MIT_License>`_
 
 ---
 
 Changelog
 =========
 
+v1.0.4
+--------
+2023-07-21:
+    - update requirements
+
 v1.0.3
 --------
 2023-07-21:
     - require minimum python 3.8
     - remove python 3.7 tests
     - introduce PEP517 packaging standard
     - introduce pyproject.toml build-system
```

### Comparing `lib_path-1.0.3/PULL_REQUEST_TEMPLATE.md` & `lib_path-1.0.4/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `lib_path-1.0.3/README.rst` & `lib_path-1.0.4/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 lib_path
 ========
 
 
-Version v1.0.3 as of 2023-07-21 see `Changelog`_
+Version v1.0.4 as of 2023-07-21 see `Changelog`_
 
 |build_badge| |codeql| |license| |jupyter| |pypi|
 |pypi-downloads| |black| |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/lib_path/actions/workflows/python-package.yml/badge.svg
@@ -220,14 +220,16 @@
 Requirements
 ------------
 following modules will be automatically installed :
 
 .. code-block:: bash
 
     ## Project Requirements
+    cli_exit_tools
+    lib_detect_testenv
     lib_platform
 
 Acknowledgements
 ----------------
 
 - special thanks to "uncle bob" Robert C. Martin, especially for his books on "clean code" and "clean architecture"
 
@@ -243,14 +245,19 @@
 This software is licensed under the `MIT license <http://en.wikipedia.org/wiki/MIT_License>`_
 
 ---
 
 Changelog
 =========
 
+v1.0.4
+--------
+2023-07-21:
+    - update requirements
+
 v1.0.3
 --------
 2023-07-21:
     - require minimum python 3.8
     - remove python 3.7 tests
     - introduce PEP517 packaging standard
     - introduce pyproject.toml build-system
```

### Comparing `lib_path-1.0.3/lib_path/lib_path.py` & `lib_path-1.0.4/lib_path/lib_path.py`

 * *Files identical despite different names*

### Comparing `lib_path-1.0.3/lib_path/lib_path_cli.py` & `lib_path-1.0.4/lib_path/lib_path_cli.py`

 * *Files identical despite different names*

### Comparing `lib_path-1.0.3/lib_path.egg-info/PKG-INFO` & `lib_path-1.0.4/lib_path.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-path
-Version: 1.0.3
+Version: 1.0.4
 Summary: path related function - deprecated
 Author-email: Robert Nowotny <bitranox@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/bitranox/lib_path
 Project-URL: Documentation, https://github.com/bitranox/lib_path/blob/master/README.rst
 Project-URL: Repository, https://github.com/bitranox/lib_path.git
 Project-URL: Changelog, https://github.com/bitranox/lib_path/blob/master/CHANGES.rst
@@ -20,15 +20,15 @@
 Provides-Extra: test
 License-File: LICENSE
 
 lib_path
 ========
 
 
-Version v1.0.3 as of 2023-07-21 see `Changelog`_
+Version v1.0.4 as of 2023-07-21 see `Changelog`_
 
 |build_badge| |codeql| |license| |jupyter| |pypi|
 |pypi-downloads| |black| |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/lib_path/actions/workflows/python-package.yml/badge.svg
@@ -242,14 +242,16 @@
 Requirements
 ------------
 following modules will be automatically installed :
 
 .. code-block:: bash
 
     ## Project Requirements
+    cli_exit_tools
+    lib_detect_testenv
     lib_platform
 
 Acknowledgements
 ----------------
 
 - special thanks to "uncle bob" Robert C. Martin, especially for his books on "clean code" and "clean architecture"
 
@@ -265,14 +267,19 @@
 This software is licensed under the `MIT license <http://en.wikipedia.org/wiki/MIT_License>`_
 
 ---
 
 Changelog
 =========
 
+v1.0.4
+--------
+2023-07-21:
+    - update requirements
+
 v1.0.3
 --------
 2023-07-21:
     - require minimum python 3.8
     - remove python 3.7 tests
     - introduce PEP517 packaging standard
     - introduce pyproject.toml build-system
```

### Comparing `lib_path-1.0.3/lib_path.egg-info/SOURCES.txt` & `lib_path-1.0.4/lib_path.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lib_path-1.0.3/lib_path.ipynb` & `lib_path-1.0.4/lib_path.ipynb`

 * *Files identical despite different names*

### Comparing `lib_path-1.0.3/pyproject.toml` & `lib_path-1.0.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -22,48 +22,50 @@
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 # dependencies - former setup.cfg "install_requires"
 # see: https://setuptools.pypa.io/en/latest/userguide/dependency_management.html
 dependencies = [
+    "cli_exit_tools",
+    "lib_detect_testenv",
     "lib_platform",
 ]
-version = "v1.0.3"
+version = "v1.0.4"
 # seems to be not allowed anymore
 # zip-save = false
 
 [project.urls]
 Homepage = "https://github.com/bitranox/lib_path"
 Documentation = "https://github.com/bitranox/lib_path/blob/master/README.rst"
 Repository = "https://github.com/bitranox/lib_path.git"
 Changelog = "https://github.com/bitranox/lib_path/blob/master/CHANGES.rst"
 
 [project.optional-dependencies]
 test = [
-    "readme_renderer",
-    "mypy",
-    "pytest-runner",
     "black",
-    "flake8",
+    "codecov",
     "coloredlogs",
     "coverage",
+    "flake8",
+    "mypy",
     "pytest",
     "pytest-cov",
-    "codecov",
+    "pytest-runner",
+    "readme_renderer",
 ]
 
 [project.scripts]
     lib_path = "lib_path.lib_path_cli:cli_main"
 
 [tool.setuptools.package-data]
 lib_path = [
-    "py.typed",
     "*.pyi",
     "__init__.pyi",
+    "py.typed",
 ]
 
 [tool.black]
 line-length = 160
 #You should include all Python versions that you want your code to run under
 target-version = ['py37', 'py38', 'py39', 'py310', 'py311']
 # Note that you have to use single-quoted strings in TOML for regular expressions
```

### Comparing `lib_path-1.0.3/pytest.ini` & `lib_path-1.0.4/pytest.ini`

 * *Files identical despite different names*

### Comparing `lib_path-1.0.3/tests/local_testscripts/lib_bash_functions.sh` & `lib_path-1.0.4/tests/local_testscripts/lib_bash_functions.sh`

 * *Files identical despite different names*

### Comparing `lib_path-1.0.3/tests/local_testscripts/run_pytest.sh` & `lib_path-1.0.4/tests/local_testscripts/run_pytest.sh`

 * *Files identical despite different names*

### Comparing `lib_path-1.0.3/tests/local_testscripts/run_testloop.sh` & `lib_path-1.0.4/tests/local_testscripts/run_testloop.sh`

 * *Files identical despite different names*

### Comparing `lib_path-1.0.3/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh` & `lib_path-1.0.4/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh`

 * *Files identical despite different names*

### Comparing `lib_path-1.0.3/tests/local_testscripts/run_testloop_windows.cmd` & `lib_path-1.0.4/tests/local_testscripts/run_testloop_windows.cmd`

 * *Files identical despite different names*

### Comparing `lib_path-1.0.3/tests/local_testscripts/shellcheck.sh` & `lib_path-1.0.4/tests/local_testscripts/shellcheck.sh`

 * *Files identical despite different names*

### Comparing `lib_path-1.0.3/tests/local_testscripts/testing_tools.py` & `lib_path-1.0.4/tests/local_testscripts/testing_tools.py`

 * *Files identical despite different names*

### Comparing `lib_path-1.0.3/tests/test_cli.py` & `lib_path-1.0.4/tests/test_cli.py`

 * *Files identical despite different names*

