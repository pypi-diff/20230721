# Comparing `tmp/lib_cicd_github-1.0.1.2.tar.gz` & `tmp/lib_cicd_github-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lib_cicd_github-1.0.1.2.tar", last modified: Thu Jun  2 12:23:12 2022, max compression
+gzip compressed data, was "lib_cicd_github-1.0.2.tar", last modified: Fri Jul 21 17:54:34 2023, max compression
```

## Comparing `lib_cicd_github-1.0.1.2.tar` & `lib_cicd_github-1.0.2.tar`

### file list

```diff
@@ -1,23 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 12:23:12.000000 lib_cicd_github-1.0.1.2/
--rw-r--r--   0 runner    (1001) docker     (121)      253 2022-06-02 12:22:23.000000 lib_cicd_github-1.0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     4241 2022-06-02 12:22:23.000000 lib_cicd_github-1.0.1.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    26696 2022-06-02 12:22:23.000000 lib_cicd_github-1.0.1.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1076 2022-06-02 12:22:23.000000 lib_cicd_github-1.0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      617 2022-06-02 12:23:12.000000 lib_cicd_github-1.0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 12:23:12.000000 lib_cicd_github-1.0.1.2/lib_cicd_github/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-02 12:22:23.000000 lib_cicd_github-1.0.1.2/lib_cicd_github/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)      530 2022-06-02 12:22:23.000000 lib_cicd_github-1.0.1.2/lib_cicd_github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3676 2022-06-02 12:22:23.000000 lib_cicd_github-1.0.1.2/lib_cicd_github/lib_cicd_github_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)      609 2022-06-02 12:22:23.000000 lib_cicd_github-1.0.1.2/lib_cicd_github/__init__conf__.py
--rw-r--r--   0 runner    (1001) docker     (121)    32873 2022-06-02 12:22:23.000000 lib_cicd_github-1.0.1.2/lib_cicd_github/lib_cicd_github.py
--rw-r--r--   0 runner    (1001) docker     (121)      523 2022-06-02 12:22:23.000000 lib_cicd_github-1.0.1.2/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)    27433 2022-06-02 12:23:12.000000 lib_cicd_github-1.0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-06-02 12:22:23.000000 lib_cicd_github-1.0.1.2/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 12:23:12.000000 lib_cicd_github-1.0.1.2/lib_cicd_github.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-06-02 12:23:12.000000 lib_cicd_github-1.0.1.2/lib_cicd_github.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-02 12:23:12.000000 lib_cicd_github-1.0.1.2/lib_cicd_github.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-02 12:23:11.000000 lib_cicd_github-1.0.1.2/lib_cicd_github.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-06-02 12:23:12.000000 lib_cicd_github-1.0.1.2/lib_cicd_github.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      511 2022-06-02 12:23:12.000000 lib_cicd_github-1.0.1.2/lib_cicd_github.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)    27433 2022-06-02 12:23:12.000000 lib_cicd_github-1.0.1.2/lib_cicd_github.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-06-02 12:23:12.000000 lib_cicd_github-1.0.1.2/lib_cicd_github.egg-info/requires.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:54:34.668894 lib_cicd_github-1.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:54:34.664894 lib_cicd_github-1.0.2/.3rd_party_stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-21 17:53:51.000000 lib_cicd_github-1.0.2/.3rd_party_stubs/readme.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-21 17:53:51.000000 lib_cicd_github-1.0.2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:54:34.664894 lib_cicd_github-1.0.2/.docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-21 17:53:51.000000 lib_cicd_github-1.0.2/.docs/README_template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-21 17:53:51.000000 lib_cicd_github-1.0.2/.docs/acknowledgment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-07-21 17:53:51.000000 lib_cicd_github-1.0.2/.docs/badges.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-21 17:53:51.000000 lib_cicd_github-1.0.2/.docs/commandline_help.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-21 17:53:51.000000 lib_cicd_github-1.0.2/.docs/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-21 17:53:51.000000 lib_cicd_github-1.0.2/.docs/description.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-21 17:53:51.000000 lib_cicd_github-1.0.2/.docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-21 17:53:51.000000 lib_cicd_github-1.0.2/.docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-21 17:53:51.000000 lib_cicd_github-1.0.2/.docs/installation_via_makefile.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-21 17:53:51.000000 lib_cicd_github-1.0.2/.docs/installation_via_pypi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-21 17:53:51.000000 lib_cicd_github-1.0.2/.docs/licence_mit.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-21 17:53:51.000000 lib_cicd_github-1.0.2/.docs/tested_under.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-21 17:53:51.000000 lib_cicd_github-1.0.2/.docs/try_in_jupyter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-21 17:53:51.000000 lib_cicd_github-1.0.2/.docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-21 17:53:51.000000 lib_cicd_github-1.0.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:54:34.660894 lib_cicd_github-1.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:54:34.664894 lib_cicd_github-1.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-21 17:53:51.000000 lib_cicd_github-1.0.2/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-07-21 17:53:51.000000 lib_cicd_github-1.0.2/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-21 17:53:51.000000 lib_cicd_github-1.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-07-21 17:53:51.000000 lib_cicd_github-1.0.2/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-21 17:53:51.000000 lib_cicd_github-1.0.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-21 17:53:51.000000 lib_cicd_github-1.0.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-21 17:53:51.000000 lib_cicd_github-1.0.2/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-21 17:53:51.000000 lib_cicd_github-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-21 17:53:51.000000 lib_cicd_github-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-21 17:53:51.000000 lib_cicd_github-1.0.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    28628 2023-07-21 17:54:34.668894 lib_cicd_github-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-21 17:53:51.000000 lib_cicd_github-1.0.2/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    27630 2023-07-21 17:53:51.000000 lib_cicd_github-1.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-21 17:53:51.000000 lib_cicd_github-1.0.2/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:54:34.664894 lib_cicd_github-1.0.2/lib_cicd_github/
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-21 17:53:51.000000 lib_cicd_github-1.0.2/lib_cicd_github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-21 17:53:51.000000 lib_cicd_github-1.0.2/lib_cicd_github/__init__conf__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31416 2023-07-21 17:53:51.000000 lib_cicd_github-1.0.2/lib_cicd_github/lib_cicd_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-07-21 17:53:51.000000 lib_cicd_github-1.0.2/lib_cicd_github/lib_cicd_github_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 17:53:51.000000 lib_cicd_github-1.0.2/lib_cicd_github/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:54:34.668894 lib_cicd_github-1.0.2/lib_cicd_github.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    28628 2023-07-21 17:54:34.000000 lib_cicd_github-1.0.2/lib_cicd_github.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-21 17:54:34.000000 lib_cicd_github-1.0.2/lib_cicd_github.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 17:54:34.000000 lib_cicd_github-1.0.2/lib_cicd_github.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-21 17:54:34.000000 lib_cicd_github-1.0.2/lib_cicd_github.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-21 17:54:34.000000 lib_cicd_github-1.0.2/lib_cicd_github.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-21 17:54:34.000000 lib_cicd_github-1.0.2/lib_cicd_github.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-21 17:53:51.000000 lib_cicd_github-1.0.2/lib_cicd_github.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-07-21 17:53:51.000000 lib_cicd_github-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-21 17:53:51.000000 lib_cicd_github-1.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-21 17:53:51.000000 lib_cicd_github-1.0.2/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 17:54:34.668894 lib_cicd_github-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:54:34.668894 lib_cicd_github-1.0.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:54:34.668894 lib_cicd_github-1.0.2/tests/local_testscripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     9587 2023-07-21 17:53:51.000000 lib_cicd_github-1.0.2/tests/local_testscripts/lib_bash_functions.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-21 17:53:51.000000 lib_cicd_github-1.0.2/tests/local_testscripts/run_clean.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-21 17:53:51.000000 lib_cicd_github-1.0.2/tests/local_testscripts/run_pytest.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-21 17:53:51.000000 lib_cicd_github-1.0.2/tests/local_testscripts/run_testloop.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-21 17:53:51.000000 lib_cicd_github-1.0.2/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-21 17:53:51.000000 lib_cicd_github-1.0.2/tests/local_testscripts/run_testloop_windows.cmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-21 17:53:51.000000 lib_cicd_github-1.0.2/tests/local_testscripts/shellcheck.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-07-21 17:53:51.000000 lib_cicd_github-1.0.2/tests/local_testscripts/testing_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-21 17:53:51.000000 lib_cicd_github-1.0.2/tests/test_cli.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `lib_cicd_github-1.0.1.2/README.rst` & `lib_cicd_github-1.0.2/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,52 +1,51 @@
 lib_cicd_github
 ===============
 
 
-Version v1.0.1.2 as of 2022-06-02 see `Changelog`_
+Version v1.0.2 as of 2023-07-21 see `Changelog`_
 
-|build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
-
-|codecov| |better_code| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+|build_badge| |codeql| |license| |jupyter| |pypi|
+|pypi-downloads| |black| |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/lib_cicd_github/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/lib_cicd_github/actions/workflows/python-package.yml
 
 
+.. |codeql| image:: https://github.com/bitranox/lib_cicd_github/actions/workflows/codeql-analysis.yml/badge.svg?event=push
+   :target: https://github.com//bitranox/lib_cicd_github/actions/workflows/codeql-analysis.yml
+
 .. |license| image:: https://img.shields.io/github/license/webcomics/pywine.svg
    :target: http://en.wikipedia.org/wiki/MIT_License
 
 .. |jupyter| image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/bitranox/lib_cicd_github/master?filepath=lib_cicd_github.ipynb
 
 .. for the pypi status link note the dashes, not the underscore !
 .. |pypi| image:: https://img.shields.io/pypi/status/lib-cicd-github?label=PyPI%20Package
    :target: https://badge.fury.io/py/lib_cicd_github
 
 .. |codecov| image:: https://img.shields.io/codecov/c/github/bitranox/lib_cicd_github
    :target: https://codecov.io/gh/bitranox/lib_cicd_github
 
-.. |better_code| image:: https://bettercodehub.com/edge/badge/bitranox/lib_cicd_github?branch=master
-   :target: https://bettercodehub.com/results/bitranox/lib_cicd_github
-
 .. |cc_maintain| image:: https://img.shields.io/codeclimate/maintainability-percentage/bitranox/lib_cicd_github?label=CC%20maintainability
    :target: https://codeclimate.com/github/bitranox/lib_cicd_github/maintainability
    :alt: Maintainability
 
 .. |cc_issues| image:: https://img.shields.io/codeclimate/issues/bitranox/lib_cicd_github?label=CC%20issues
    :target: https://codeclimate.com/github/bitranox/lib_cicd_github/maintainability
    :alt: Maintainability
 
 .. |cc_coverage| image:: https://img.shields.io/codeclimate/coverage/bitranox/lib_cicd_github?label=CC%20coverage
    :target: https://codeclimate.com/github/bitranox/lib_cicd_github/test_coverage
    :alt: Code Coverage
 
-.. |snyk| image:: https://img.shields.io/snyk/vulnerabilities/github/bitranox/lib_cicd_github
+.. |snyk| image:: https://snyk.io/test/github/bitranox/lib_cicd_github/badge.svg
    :target: https://snyk.io/test/github/bitranox/lib_cicd_github
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/lib-cicd-github
    :target: https://pypi.org/project/lib-cicd-github/
@@ -55,22 +54,22 @@
 small utils for github actions:
  - print colored banners
  - wrap commands into run/success/error banners, with automatic retry
  - resolve the branch to test, based on the environment variables
 
 ----
 
-automated tests, Travis Matrix, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
+automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
-Python version required: 3.6.0 or newer
+Python version required: 3.8.0 or newer
 
-tested on recent linux with python 3.6, 3.7, 3.8, 3.9, 3.10, pypy-3.8 - architectures: amd64
+tested on recent linux with python 3.8, 3.9, 3.10, 3.11, 3.12-dev, pypy-3.9, pypy-3.10 - architectures: amd64
 
-`100% code coverage <https://codecov.io/gh/bitranox/lib_cicd_github>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/lib_cicd_github/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
+`100% code coverage <https://codeclimate.com/github/bitranox/lib_cicd_github/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/lib_cicd_github/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
 - `Usage from Commandline`_
 - `Installation and Upgrade`_
@@ -125,26 +124,27 @@
         cPIP
             from environment, the command to launch pip, like "python -m pip"
 
 
         Examples
         --------
 
+        >>> # Test
         >>> if is_github_actions_active():
         ...     install(dry_run=True)
 
         """
 
 - script, run all tests
 
 .. code-block:: python
 
     def script(dry_run: bool = True) -> None:
         """
-        travis jobs to run in travis.yml section "script":
+        jobs to run in CICD section "script":
         - run setup.py test
         - run pip with install option test
         - run pip standard install
         - test the CLI Registration
         - install the test requirements
         - install codecov
         - install pytest-codecov
@@ -160,15 +160,15 @@
         cPREFIX
             from environment, the command prefix like 'wine' or ''
         cPIP
             from environment, the command to launch pip, like "python -m pip"
         cPYTHON
             from environment, the command to launch python, like 'python' or 'python3' on MacOS
         CLI_COMMAND
-            from environment, must be set in travis - the CLI command to test with option --version
+            from environment, must be set in CICD configuration file - the CLI command to test with option --version
         MYPY_STRICT
             from environment, if pytest with mypy --strict should run
         PACKAGE_NAME
             from environment, the package name to pass to mypy
         BUILD_DOCS
             from environment, if rst file should be rebuilt
         RST_INCLUDE_SOURCE
@@ -180,46 +180,46 @@
             only if setup.py exists and on non-tagged builds (there we deploy for real)
         dry_run
             if set, this returns immediately - for CLI tests
 
 
         Examples
         --------
+        >>> # test
         >>> script()
 
         """
 
 - after_success, upload code coverage and codeclimate reports
 
 .. code-block:: python
 
     def after_success(dry_run: bool = True) -> None:
         """
-        travis jobs to run in travis.yml section "after_success":
+        jobs to run in CICD "after_success":
             - coverage report
             - codecov
             - codeclimate report upload
 
 
         Parameter
         ---------
         cPREFIX
             from environment, the command prefix like 'wine' or ''
         cPIP
             from environment, the command to launch pip, like "python -m pip"
         CC_TEST_REPORTER_ID
-            from environment, must be set in travis
-        TRAVIS_TEST_RESULT
-            from environment, this is set by TRAVIS automatically
+            from environment, must be set in CICD configuration file
         dry_run
             if set, this returns immediately - for CLI tests
 
 
         Examples
         --------
+        >>> # test
         >>> after_success()
 
         """
 
 - deploy, deploy to pypi
 
 .. code-block:: python
@@ -231,24 +231,23 @@
 
         Parameter
         ---------
         cPREFIX
             from environment, the command prefix like 'wine' or ''
         PYPI_PASSWORD
             from environment, passed as secure, encrypted variable to environment
-        TRAVIS_TAG
-            from environment, needs to be set
         DEPLOY_SDIST, DEPLOY_WHEEL
             from environment, one of it needs to be true
         dry_run
             if set, this returns immediately - for CLI tests
 
 
         Examples
         --------
+        >>> # test
         >>> deploy()
 
         """
 
 - get_branch, determine the branch to work on
 
 .. code-block:: python
@@ -436,15 +435,15 @@
 
             # FLAKE8 tests
             DO_FLAKE8_TESTS: "True"
 
             # MYPY tests
             MYPY_DO_TESTS: "True"
             MYPY_OPTIONS: "--follow-imports=normal --ignore-missing-imports --implicit-reexport --install-types --no-warn-unused-ignores --non-interactive --strict"
-            MYPYPATH: "./lib_cicd_github/3rd_party_stubs"
+            MYPYPATH: "./.3rd_party_stubs"
 
             # coverage
             DO_COVERAGE: "True"
             DO_COVERAGE_UPLOAD_CODECOV: "True"
             DO_COVERAGE_UPLOAD_CODE_CLIMATE: "True"
 
             # package name
@@ -461,113 +460,117 @@
             PYPI_PASSWORD: ${{ secrets.PYPI_PASSWORD }}
 
 
         strategy:
           matrix:
             include:
               # https://docs.github.com/en/actions/using-github-hosted-runners/about-github-hosted-runners#supported-software
+              # https://github.com/actions/setup-python/blob/main/docs/advanced-usage.md#available-versions-of-python-and-pypy
 
               - os: windows-latest
-                python-version: "3.10"
+                python-version: "3.11"
                 env:
                   cEXPORT: "SET"
                   BUILD_DOCS: "False"
-                  DEPLOY_SDIST: "False"
-                  DEPLOY_WHEEL: "False"
-                  DEPLOY_TEST: "False"
+                  BUILD: "False"
+                  BUILD_TEST: "False"
                   MYPY_DO_TESTS: "True"
                   # Setup tests
                   DO_SETUP_INSTALL: "False"
                   DO_SETUP_INSTALL_TEST: "True"
                   # Test registered CLI Command
                   DO_CLI_TEST: "True"
 
 
               - os: ubuntu-latest
-                python-version: "3.6"
+                python-version: "3.8"
                 env:
                   BUILD_DOCS: "False"
-                  DEPLOY_SDIST: "True"
-                  DEPLOY_WHEEL: "True"
-                  DEPLOY_TEST: "True"
+                  BUILD: "True"
+                  BUILD_TEST: "True"
                   MYPY_DO_TESTS: "True"
                   DO_SETUP_INSTALL: "True"
-                  DO_SETUP_INSTALL_TEST: "False"
+                  DO_SETUP_INSTALL_TEST: "True"
                   DO_CLI_TEST: "True"
 
               - os: ubuntu-latest
-                python-version: "3.7"
+                python-version: "3.9"
                 env:
                   BUILD_DOCS: "False"
-                  DEPLOY_SDIST: "True"
-                  DEPLOY_WHEEL: "True"
-                  DEPLOY_TEST: "True"
+                  BUILD: "True"
+                  BUILD_TEST: "True"
                   MYPY_DO_TESTS: "True"
                   DO_SETUP_INSTALL: "True"
-                  DO_SETUP_INSTALL_TEST: "False"
+                  DO_SETUP_INSTALL_TEST: "True"
                   DO_CLI_TEST: "True"
 
               - os: ubuntu-latest
-                python-version: "3.8"
+                python-version: "3.10"
                 env:
                   BUILD_DOCS: "False"
-                  DEPLOY_SDIST: "True"
-                  DEPLOY_WHEEL: "True"
-                  DEPLOY_TEST: "True"
+                  BUILD: "True"
+                  BUILD_TEST: "True"
                   MYPY_DO_TESTS: "True"
                   DO_SETUP_INSTALL: "True"
-                  DO_SETUP_INSTALL_TEST: "False"
+                  DO_SETUP_INSTALL_TEST: "True"
                   DO_CLI_TEST: "True"
 
               - os: ubuntu-latest
-                python-version: "3.9"
+                python-version: "3.11"
                 env:
-                  BUILD_DOCS: "False"
-                  DEPLOY_SDIST: "True"
-                  DEPLOY_WHEEL: "True"
-                  DEPLOY_TEST: "True"
+                  BUILD_DOCS: "True"
+                  BUILD: "True"
+                  BUILD_TEST: "True"
                   MYPY_DO_TESTS: "True"
                   DO_SETUP_INSTALL: "True"
-                  DO_SETUP_INSTALL_TEST: "False"
+                  DO_SETUP_INSTALL_TEST: "True"
                   DO_CLI_TEST: "True"
 
               - os: ubuntu-latest
-                python-version: "3.10"
+                python-version: "3.12-dev"
                 env:
                   BUILD_DOCS: "True"
-                  DEPLOY_SDIST: "True"
-                  DEPLOY_WHEEL: "True"
-                  DEPLOY_TEST: "True"
+                  BUILD: "True"
+                  BUILD_TEST: "True"
                   MYPY_DO_TESTS: "True"
                   DO_SETUP_INSTALL: "True"
                   DO_SETUP_INSTALL_TEST: "True"
                   DO_CLI_TEST: "True"
 
               - os: ubuntu-latest
-                python-version: "pypy-3.8"
+                python-version: "pypy-3.9"
                 env:
                   BUILD_DOCS: "False"
-                  DEPLOY_SDIST: "True"
-                  DEPLOY_WHEEL: "True"
-                  DEPLOY_TEST: "True"
-                  MYPY_DO_TESTS: "False"
+                  BUILD: "True"
+                  BUILD_TEST: "True"
+                  MYPY_DO_TESTS: "True"
                   DO_SETUP_INSTALL: "True"
-                  DO_SETUP_INSTALL_TEST: "False"
+                  DO_SETUP_INSTALL_TEST: "True"
+                  DO_CLI_TEST: "True"
+
+              - os: ubuntu-latest
+                python-version: "pypy-3.10"
+                env:
+                  BUILD_DOCS: "False"
+                  BUILD: "True"
+                  BUILD_TEST: "True"
+                  MYPY_DO_TESTS: "True"
+                  DO_SETUP_INSTALL: "True"
+                  DO_SETUP_INSTALL_TEST: "True"
                   DO_CLI_TEST: "True"
 
               - os: macos-latest
-                python-version: "3.10"
+                python-version: "3.11"
                 env:
                   cPREFIX: ""               # prefix before commands - used for wine, there the prefix is "wine"
                   cPYTHON: "python3"        # command to launch python interpreter (it's different on macOS, there we need python3)
                   cPIP: "python3 -m pip"    # command to launch pip (it's different on macOS, there we need pip3)
                   BUILD_DOCS: "False"
-                  DEPLOY_SDIST: "True"
-                  DEPLOY_WHEEL: "True"
-                  DEPLOY_TEST: "True"
+                  BUILD: "True"
+                  BUILD_TEST: "True"
                   MYPY_DO_TESTS: "True"
                   # Setup tests
                   DO_SETUP_INSTALL: "True"
                   DO_SETUP_INSTALL_TEST: "True"
                   # Test registered CLI Command
                   DO_CLI_TEST: "True"
 
@@ -575,15 +578,16 @@
         name: "${{ matrix.os }} Python ${{ matrix.python-version }}"
 
         steps:
         # see : https://github.com/actions/checkout
         - uses: actions/checkout@v3
 
         - name: Setting up Python ${{ matrix.python-version }}
-          uses: actions/setup-python@v3
+          # see: https://github.com/actions/setup-python
+          uses: actions/setup-python@v4
           with:
             python-version: ${{ matrix.python-version }}
 
         - name: Install dependencies
           # see: https://github.community/t/github-actions-new-bug-unable-to-create-environment-variables-based-matrix/16104/3
           env: ${{ matrix.env }}             # make matrix env variables accessible
           # lib_cicd_github install: upgrades pip, setuptools, wheel and pytest-pycodestyle
@@ -684,14 +688,21 @@
 
 - to install the latest release from PyPi via pip (recommended):
 
 .. code-block::
 
     python -m pip install --upgrade lib_cicd_github
 
+
+- to install the latest release from PyPi via pip, including test dependencies:
+
+.. code-block::
+
+    python -m pip install --upgrade lib_cicd_github[test]
+
 - to install the latest version from github via pip:
 
 
 .. code-block::
 
     python -m pip install --upgrade git+https://github.com/bitranox/lib_cicd_github.git
 
@@ -707,22 +718,22 @@
     # for the latest development version :
     lib_cicd_github @ git+https://github.com/bitranox/lib_cicd_github.git
 
     # to install and upgrade all modules mentioned in requirements.txt:
     python -m pip install --upgrade -r /<path>/requirements.txt
 
 
-- to install the latest development version from source code:
+- to install the latest development version, including test dependencies from source code:
 
 .. code-block::
 
     # cd ~
     $ git clone https://github.com/bitranox/lib_cicd_github.git
     $ cd lib_cicd_github
-    python setup.py install
+    python -m pip install -e .[test]
 
 - via makefile:
   makefiles are a very convenient way to install. Here we can do much more,
   like installing virtual environments, clean caches and so on.
 
 .. code-block:: shell
 
@@ -776,14 +787,36 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v1.0.2
+--------
+2023-07-21:
+    - create mypy cache dir '.mypy_cache'
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
+
 v1.0.1.2
 ---------
 2022-06-02: update to github actions checkout@v3 and setup-python@v3
 
 v1.0.1
 --------
 2022-03-29: remedy mypy Untyped decorator in cli
```

### Comparing `lib_cicd_github-1.0.1.2/LICENSE` & `lib_cicd_github-1.0.2/LICENSE`

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

### Comparing `lib_cicd_github-1.0.1.2/lib_cicd_github/__init__.py` & `lib_cicd_github-1.0.2/lib_cicd_github/__init__.py`

 * *Files identical despite different names*

### Comparing `lib_cicd_github-1.0.1.2/lib_cicd_github/lib_cicd_github_cli.py` & `lib_cicd_github-1.0.2/lib_cicd_github/lib_cicd_github_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     >>> info()
     Info for ...
 
     """
     __init__conf__.print_info()
 
 
-@click.group(help=__init__conf__.title, context_settings=CLICK_CONTEXT_SETTINGS)
+@click.group(help=__init__conf__.title, context_settings=CLICK_CONTEXT_SETTINGS)        # type: ignore
 @click.version_option(
     version=__init__conf__.version,
     prog_name=__init__conf__.shell_command,
     message=f"{__init__conf__.shell_command} version {__init__conf__.version}",
 )
 @click.option(
     "--traceback/--no-traceback",
@@ -100,13 +100,13 @@
     """deploy on pypi"""
     lib_cicd_github.deploy(dry_run)
 
 
 # entry point if main
 if __name__ == "__main__":
     try:
-        cli_main()
+        cli_main()      # type: ignore
     except Exception as exc:
         cli_exit_tools.print_exception_message()
         sys.exit(cli_exit_tools.get_system_exit_code(exc))
     finally:
         cli_exit_tools.flush_streams()
```

### Comparing `lib_cicd_github-1.0.1.2/lib_cicd_github/__init__conf__.py` & `lib_cicd_github-1.0.2/lib_cicd_github/__init__conf__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 # CONF
 
-name = "lib_cicd_github"
-title = "CI/CD (Continuous Integration / Continuous Delivery) - utils for github actions"
-version = "v1.0.1.2"
-url = "https://github.com/bitranox/lib_cicd_github"
-author = "Robert Nowotny"
-author_email = "bitranox@gmail.com"
-shell_command = "lib_cicd_github"
+name = 'lib_cicd_github'
+title = 'CI/CD (Continuous Integration / Continuous Delivery) - utils for github actions'
+version = 'v1.0.2'
+url = 'https://github.com/bitranox/lib_cicd_github'
+author = 'Robert Nowotny'
+author_email = 'bitranox@gmail.com'
+shell_command = 'lib_cicd_github'
 
 
 def print_info() -> None:
-    print(
-        """\
+    print("""\
 
 Info for lib_cicd_github:
 
     CI/CD (Continuous Integration / Continuous Delivery) - utils for github actions
 
-    Version : v1.0.1.2
+    Version : v1.0.2
     Url     : https://github.com/bitranox/lib_cicd_github
     Author  : Robert Nowotny
-    Email   : bitranox@gmail.com"""
-    )
+    Email   : bitranox@gmail.com""")
```

### Comparing `lib_cicd_github-1.0.1.2/lib_cicd_github/lib_cicd_github.py` & `lib_cicd_github-1.0.2/lib_cicd_github/lib_cicd_github.py`

 * *Files 5% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     while True:
         try:
             subprocess.run(command, shell=True, check=True)
             lib_log_utils.banner_success(f"Success: {description}", banner=False)
             break
         except Exception as exc:
             tries = tries - 1
-            # try 3 times, because sometimes connection or other errors on travis
+            # try 3 times, because sometimes connection or other errors on the CICD Cloud Instance
             if tries:
                 lib_log_utils.banner_spam(
                     f"Retry in {sleep} seconds: {description}\nCommand: {command_description}",
                     banner=False,
                 )
                 time.sleep(sleep)
             else:
@@ -223,14 +223,15 @@
     cPIP
         from environment, the command to launch pip, like "python -m pip"
 
 
     Examples
     --------
 
+    >>> # Test
     >>> if is_github_actions_active():
     ...     install(dry_run=True)
 
     """
     # install}}}
     if dry_run:
         return
@@ -239,41 +240,33 @@
         description="install pip",
         command=" ".join([pip_prefix, "install --upgrade pip"]),
     )
     run(
         description="install setuptools",
         command=" ".join([pip_prefix, "install --upgrade setuptools"]),
     )
-    run(
-        description="install readme renderer",
-        command=" ".join([pip_prefix, "install --upgrade readme_renderer"]),
-    )
 
-    run(
-        description="install twine",
-        command=" ".join([pip_prefix, "install --upgrade twine"]),
-    )
-    run(
-        description="install wheel",
-        command=" ".join([pip_prefix, "install --upgrade wheel"]),
-    )
-    run(
-        description="install requirements",
-        command=" ".join([pip_prefix, "install --upgrade -r ./requirements.txt"]),
-    )
-    run(
-        description="install test requirements",
-        command=" ".join([pip_prefix, "install --upgrade -r ./requirements_test.txt"]),
-    )
+    if is_do_pip_install_test():
+        run(
+            description="pip install package in editable(develop) mode",
+            command=" ".join([pip_prefix, "install --editable .[test]"]),
+        )
+    elif is_do_pip_install():
+        run(
+            description="pip install package",
+            command=" ".join([pip_prefix, "install ."]),
+        )
+    else:
+        lib_log_utils.banner_spam("package will be not installed")
 
 
 # script{{{
 def script(dry_run: bool = True) -> None:
     """
-    travis jobs to run in travis.yml section "script":
+    jobs to run in CICD section "script":
     - run setup.py test
     - run pip with install option test
     - run pip standard install
     - test the CLI Registration
     - install the test requirements
     - install codecov
     - install pytest-codecov
@@ -289,15 +282,15 @@
     cPREFIX
         from environment, the command prefix like 'wine' or ''
     cPIP
         from environment, the command to launch pip, like "python -m pip"
     cPYTHON
         from environment, the command to launch python, like 'python' or 'python3' on MacOS
     CLI_COMMAND
-        from environment, must be set in travis - the CLI command to test with option --version
+        from environment, must be set in CICD configuration file - the CLI command to test with option --version
     MYPY_STRICT
         from environment, if pytest with mypy --strict should run
     PACKAGE_NAME
         from environment, the package name to pass to mypy
     BUILD_DOCS
         from environment, if rst file should be rebuilt
     RST_INCLUDE_SOURCE
@@ -309,132 +302,111 @@
         only if setup.py exists and on non-tagged builds (there we deploy for real)
     dry_run
         if set, this returns immediately - for CLI tests
 
 
     Examples
     --------
+    >>> # test
     >>> script()
 
     """
     # script}}}
     if dry_run:
         return
     lib_log_utils.setup_handler()
     command_prefix = get_env_data("cPREFIX")
     package_name = get_env_data("PACKAGE_NAME")
     python_prefix = get_python_prefix()
-    # pip_prefix = get_pip_prefix()
+    pip_prefix = get_pip_prefix()
 
     if do_flake8_tests():
         run(description="flake8 tests", command=f"{python_prefix} -m flake8 --statistics --benchmark")
     else:
         lib_log_utils.banner_spam("flake8 tests disabled on this build")
 
-    if do_mypy_tests():
-        mypy_options = get_env_data("MYPY_OPTIONS")
-        run(description="mypy tests", command=f"{python_prefix} -m mypy -p {package_name} {mypy_options}")
+    if is_run_mypy_tests():
+        run_mypy_tests(package_name=package_name, python_prefix=python_prefix)
     else:
         lib_log_utils.banner_spam("mypy tests disabled on this build")
 
     if do_pytest():
         if do_coverage():
             option_codecov = f"--cov={package_name}"
         else:
             lib_log_utils.banner_spam("coverage disabled on this build")
             option_codecov = ""
         run(description="run pytest", command=f"{python_prefix} -m pytest {option_codecov}")
     else:
         lib_log_utils.banner_spam("pytest disabled on this build")
 
-    """
-    # this takes a long time - we did not implement atm
-    if do_pip_install_option_test():
-        # pip install git+https://github.com/bitranox/cli_exit_tools.git@development
-        run(description='pip install --install-option test', command=f'{pip_prefix} install {repository} --install-option test')
-    """
-
-    """
-    # we dont need to test it
-    if do_pip_install():
-        # pip install git+https://github.com/bitranox/cli_exit_tools.git@development
-        run(description='pip standard install', command=' '.join([pip_prefix, 'install', repository]))
-    """
-
-    if do_setup_py_test():
-        run(description="setup.py test", command=f"{python_prefix} ./setup.py test")
-
-    if do_setup_py():
-        run(description="setup.py install", command=f"{python_prefix} ./setup.py install")
-
     if do_check_cli():
-        cli_command = get_env_data("CLI_COMMAND")
+        cli_command = get_env_data("CLI_COMMAND").strip()
         run(description="check CLI command", command=f"{command_prefix} {cli_command} --version")
 
     if do_build_docs():
         rst_include_source = os.getenv("RST_INCLUDE_SOURCE", "")
         rst_include_target = os.getenv("RST_INCLUDE_TARGET", "")
         rst_include_source_name = pathlib.Path(rst_include_source).name
         rst_include_target_name = pathlib.Path(rst_include_target).name
         run(
             description=f"rst rebuild {rst_include_target_name} from {rst_include_source_name}",
             command=f"{command_prefix} rst_include include {rst_include_source} {rst_include_target}",
         )
     else:
         lib_log_utils.banner_spam("rebuild doc file is disabled on this build")
 
-    if do_deploy_sdist() or do_build_test():
+    if do_build() or do_build_test():
         run(
-            description="create source distribution",
-            command=" ".join([python_prefix, "setup.py sdist"]),
+            description="upgrade building system",
+            command=" ".join([pip_prefix, "install --upgrade build"]),
         )
-    else:
-        lib_log_utils.banner_spam("create source distribution is disabled on this build")
 
-    if do_deploy_wheel() or do_build_test():
         run(
-            description="create binary distribution (wheel)",
-            command=" ".join([python_prefix, "setup.py bdist_wheel"]),
+            description="upgrade twine",
+            command=" ".join([pip_prefix, "install --upgrade twine"]),
+        )
+
+        run(
+            description="build wheel and sdist",
+            command=" ".join([python_prefix, "-m build"]),
         )
-    else:
-        lib_log_utils.banner_spam("create wheel distribution is disabled on this build")
 
-    if do_deploy_sdist() or do_deploy_wheel() or do_build_test():
         run(
             description="check distributions",
-            command=" ".join([command_prefix, "twine check dist/*"]),
+            command=" ".join([python_prefix, "-m twine check dist/*"]),
         )
+
         list_dist_directory()
 
 
 # after_success{{{
 def after_success(dry_run: bool = True) -> None:
     """
-    travis jobs to run in travis.yml section "after_success":
+    jobs to run in CICD "after_success":
         - coverage report
         - codecov
         - codeclimate report upload
 
 
     Parameter
     ---------
     cPREFIX
         from environment, the command prefix like 'wine' or ''
     cPIP
         from environment, the command to launch pip, like "python -m pip"
     CC_TEST_REPORTER_ID
-        from environment, must be set in travis
-    TRAVIS_TEST_RESULT
-        from environment, this is set by TRAVIS automatically
+        from environment, must be set in CICD configuration file
     dry_run
         if set, this returns immediately - for CLI tests
 
 
     Examples
     --------
+    >>> # test
     >>> after_success()
 
     """
     # after_success}}}
 
     if dry_run:
         return
@@ -500,45 +472,42 @@
 
     Parameter
     ---------
     cPREFIX
         from environment, the command prefix like 'wine' or ''
     PYPI_PASSWORD
         from environment, passed as secure, encrypted variable to environment
-    TRAVIS_TAG
-        from environment, needs to be set
     DEPLOY_SDIST, DEPLOY_WHEEL
         from environment, one of it needs to be true
     dry_run
         if set, this returns immediately - for CLI tests
 
 
     Examples
     --------
+    >>> # test
     >>> deploy()
 
     """
     # deploy}}}
 
     if dry_run:
         return
-    command_prefix = get_env_data("cPREFIX")
-    github_username = get_github_username()
     pypi_password = get_env_data("PYPI_PASSWORD").strip()
     if not pypi_password:
         lib_log_utils.banner_warning("can not deploy, because secret PYPI_PASSWORD is missing")
     elif do_deploy():
         if not dry_run:  # pragma: no cover
             run(
                 description="upload to pypi",
                 command=" ".join(
                     [
-                        command_prefix,
-                        "twine upload --repository-url https://upload.pypi.org/legacy/ -u",
-                        github_username,
+                        get_python_prefix(),
+                        "-m twine upload --repository-url https://upload.pypi.org/legacy/ -u",
+                        get_github_username(),
                         "-p",
                         pypi_password,
                         "--skip-existing",
                         "dist/*",
                     ]
                 ),
                 show_command=False,
@@ -556,51 +525,51 @@
         lib_log_utils.banner_warning('no "./dist" directory found')
 
 
 def get_pip_prefix() -> str:
     """
     get the pip_prefix including the command prefix like : 'wine python -m pip'
 
-    >>> if 'TRAVIS' in os.environ:
+    >>> # test
+    >>> if 'cPREFIX' in os.environ:
     ...    discard = get_pip_prefix()
-
     """
     c_parts: List[str] = list()
     c_parts.append(os.getenv("cPREFIX", ""))
     c_parts.append(os.getenv("cPIP", ""))
     command_prefix = " ".join(c_parts).strip()
     return command_prefix
 
 
 def get_python_prefix() -> str:
     """
     get the python_prefix including the command prefix like : 'wine python'
 
-    >>> if 'TRAVIS' in os.environ:
+    >>> # test
+    >>> if 'cPREFIX' in os.environ:
     ...    discard = get_python_prefix()
-
     """
     c_parts: List[str] = list()
     c_parts.append(os.getenv("cPREFIX", ""))
     c_parts.append(os.getenv("cPYTHON", ""))
     python_prefix = " ".join(c_parts).strip()
     return python_prefix
 
 
 def get_github_username() -> str:
     """
     get the github username like 'bitranox' (the OWNER of the Repository !)
 
+    >>> # test
     >>> discard = get_github_username()
-
     """
     return get_env_data("GITHUB_REPOSITORY_OWNER")
 
 
-def do_mypy_tests() -> bool:
+def is_run_mypy_tests() -> bool:
     """
     if mypy should be run
 
     Parameter
     ---------
     MYPY_DO_TESTS
         from environment
@@ -608,26 +577,25 @@
     Examples:
 
     >>> # Setup
     >>> save_do_mypy = os.getenv('MYPY_DO_TESTS')
 
     >>> # BUILD_TEST != 'True'
     >>> os.environ['MYPY_DO_TESTS'] = 'false'
-    >>> assert not do_mypy_tests()
+    >>> assert not is_run_mypy_tests()
 
     >>> # BUILD_TEST == 'true'
     >>> os.environ['MYPY_DO_TESTS'] = 'True'
-    >>> assert do_mypy_tests()
+    >>> assert is_run_mypy_tests()
 
     >>> # Teardown
     >>> if save_do_mypy is None:
     ...     os.unsetenv('MYPY_DO_TESTS')
     ... else:
     ...     os.environ['MYPY_DO_TESTS'] = save_do_mypy
-
     """
 
     if os.getenv("MYPY_DO_TESTS", "").lower() == "true":
         return True
     else:
         return False
 
@@ -655,15 +623,14 @@
     >>> assert do_pytest()
 
     >>> # Teardown
     >>> if save_do_pytest is None:
     ...     os.unsetenv('PYTEST_DO_TESTS')
     ... else:
     ...     os.environ['PYTEST_DO_TESTS'] = save_do_pytest
-
     """
     if os.getenv("PYTEST_DO_TESTS", "").lower() == "true":
         return True
     else:
         return False
 
 
@@ -690,15 +657,14 @@
     >>> assert do_coverage()
 
     >>> # Teardown
     >>> if save_do_coverage is None:
     ...     os.unsetenv('DO_COVERAGE')
     ... else:
     ...     os.environ['DO_COVERAGE'] = save_do_coverage
-
     """
     return get_env_data("DO_COVERAGE").lower() == "true"
 
 
 def do_upload_codecov() -> bool:
     """
     if code coverage should be uploaded to codecov
@@ -754,25 +720,28 @@
     >>> assert do_upload_code_climate()
 
     >>> # Teardown
     >>> if save_upload_code_climate is None:
     ...     os.unsetenv('DO_COVERAGE_UPLOAD_CODE_CLIMATE')
     ... else:
     ...     os.environ['DO_COVERAGE_UPLOAD_CODE_CLIMATE'] = save_upload_code_climate
-
     """
     return get_env_data("DO_COVERAGE_UPLOAD_CODE_CLIMATE").lower() == "true"
 
 
-def do_setup_py() -> bool:
-    return get_env_data("DO_SETUP_INSTALL").lower() == "true"
+def is_do_pip_install() -> bool:
+    # "DO_SETUP_INSTALL" is deprecated and will be replaced with "DO_PIP_INSTALL"
+    do_pip_install = get_env_data("DO_SETUP_INSTALL").lower() == "true" or get_env_data("DO_PIP_INSTALL").lower() == "true"
+    return do_pip_install
 
 
-def do_setup_py_test() -> bool:
-    return get_env_data("DO_SETUP_INSTALL_TEST").lower() == "true"
+def is_do_pip_install_test() -> bool:
+    # "DO_SETUP_INSTALL_TEST" is deprecated and will be replaced with "DO_PIP_INSTALL_TEST"
+    do_pip_install_test = get_env_data("DO_SETUP_INSTALL_TEST").lower() == "true" or get_env_data("DO_PIP_INSTALL_TEST").lower() == "true"
+    return do_pip_install_test
 
 
 def do_check_cli() -> bool:
     return get_env_data("DO_CLI_TEST").lower() == "true"
 
 
 def do_build_docs() -> bool:
@@ -820,87 +789,27 @@
     >>> set_env_data('RST_INCLUDE_TARGET', 'some_target')
     >>> assert do_build_docs() == True
 
     >>> # Teardown
     >>> set_env_data('BUILD_DOCS', save_build_docs)
     >>> set_env_data('RST_INCLUDE_SOURCE', save_rst_include_source)
     >>> set_env_data('RST_INCLUDE_TARGET', save_rst_include_target)
-
     """
     if get_env_data("BUILD_DOCS").lower() != "true":
         return False
 
     if not get_env_data("RST_INCLUDE_SOURCE"):
         return False
 
     if not get_env_data("RST_INCLUDE_TARGET"):
         return False
     else:
         return True
 
 
-def do_deploy_sdist() -> bool:
-    """
-    if we should deploy sdist
-
-
-    Parameter
-    ---------
-    DEPLOY_SDIST
-        from environment
-
-    Examples:
-
-    >>> # Setup
-    >>> save_deploy_sdist = get_env_data('DEPLOY_SDIST')
-
-    >>> # DEPLOY_SDIST != 'true'
-    >>> os.environ['DEPLOY_SDIST'] = 'false'
-    >>> assert False == do_deploy_sdist()
-
-    >>> # DEPLOY_SDIST == 'true'
-    >>> os.environ['DEPLOY_SDIST'] = 'True'
-    >>> assert True == do_deploy_sdist()
-
-    >>> # Teardown
-    >>> set_env_data('DEPLOY_SDIST', save_deploy_sdist)
-
-    """
-    return get_env_data("DEPLOY_SDIST").lower() == "true"
-
-
-def do_deploy_wheel() -> bool:
-    """
-    if we should deploy wheels
-
-    Parameter
-    ---------
-    DEPLOY_WHEEL
-        from environment
-
-    Examples:
-
-    >>> # Setup
-    >>> save_deploy_wheel = get_env_data('DEPLOY_WHEEL')
-
-    >>> # DEPLOY_WHEEL != 'true'
-    >>> os.environ['DEPLOY_WHEEL'] = 'false'
-    >>> assert not do_deploy_wheel()
-
-    >>> # DEPLOY_WHEEL == 'true'
-    >>> os.environ['DEPLOY_WHEEL'] = 'True'
-    >>> assert do_deploy_wheel()
-
-    >>> # Teardown
-    >>> set_env_data('DEPLOY_WHEEL', save_deploy_wheel)
-
-    """
-    return get_env_data("DEPLOY_WHEEL").lower() == "true"
-
-
 def do_flake8_tests() -> bool:
     """
     if we should do flake8 tests
 
     Parameter
     ---------
     DO_FLAKE8_TESTS
@@ -920,19 +829,50 @@
     >>> assert do_flake8_tests()
 
     >>> # Teardown
     >>> if save_flake8_test is None:
     ...     os.unsetenv('DO_FLAKE8_TESTS')
     ... else:
     ...     os.environ['DO_FLAKE8_TESTS'] = save_flake8_test
+    """
+    if os.getenv("DO_FLAKE8_TESTS", "").lower() == "true":
+        return True
+    else:
+        return False
+
+
+def do_build() -> bool:
+    """
+    if a build (sdist and wheel) should be done
+
+    Parameter
+    ---------
+    BUILD
+        from environment
+
+    Examples:
 
+    >>> # Setup
+    >>> save_build = os.getenv('BUILD')
+
+    >>> # BUILD_TEST != 'True'
+    >>> os.environ['BUILD'] = 'false'
+    >>> assert not do_build()
 
+    >>> # BUILD_TEST == 'true'
+    >>> os.environ['BUILD'] = 'True'
+    >>> assert do_build()
 
+    >>> # Teardown
+    >>> if save_build is None:
+    ...     os.unsetenv('BUILD')
+    ... else:
+    ...     os.environ['BUILD'] = save_build
     """
-    if os.getenv("DO_FLAKE8_TESTS", "").lower() == "true":
+    if os.getenv("BUILD", "").lower() == "true":
         return True
     else:
         return False
 
 
 def do_build_test() -> bool:
     """
@@ -957,15 +897,14 @@
     >>> assert do_build_test()
 
     >>> # Teardown
     >>> if save_build_test is None:
     ...     os.unsetenv('BUILD_TEST')
     ... else:
     ...     os.environ['BUILD_TEST'] = save_build_test
-
     """
     if os.getenv("BUILD_TEST", "").lower() == "true":
         return True
     else:
         return False
 
 
@@ -988,15 +927,14 @@
     >>> assert is_pypy3() == True
 
     >>> set_env_data('matrix.python-version', '3.9')
     >>> assert is_pypy3() == False
 
     >>> # Teardown
     >>> set_env_data('matrix.python-version', save_python_version)
-
     """
     return get_env_data("matrix.python-version").lower().startswith("pypy-3")
 
 
 def is_ci_runner_os_windows() -> bool:
     """
     if the ci runner os is windows
@@ -1011,22 +949,20 @@
     >>> # Setup
     >>> save_gha_os_name = get_env_data('RUNNER_OS')
 
     >>> # runner.os == 'linux'
     >>> set_env_data('RUNNER_OS', 'Linux')
     >>> assert is_ci_runner_os_windows() == False
 
-    >>> # TRAVIS_OS_NAME == 'windows'
+    >>> # RUNNER_OS == 'windows'
     >>> set_env_data('RUNNER_OS', 'Windows')
     >>> assert is_ci_runner_os_windows() == True
 
     >>> # Teardown
     >>> set_env_data('RUNNER_OS', save_gha_os_name)
-
-
     """
     return get_env_data("RUNNER_OS").lower() == "windows"
 
 
 def is_ci_runner_os_linux() -> bool:
     """
     if the ci runner os is linux
@@ -1041,21 +977,20 @@
     >>> # Setup
     >>> save_gha_os_name = get_env_data('RUNNER_OS')
 
     >>> # runner.os == 'linux'
     >>> set_env_data('RUNNER_OS', 'Linux')
     >>> assert is_ci_runner_os_linux() == True
 
-    >>> # TRAVIS_OS_NAME == 'windows'
+    >>> # RUNNER_OS == 'windows'
     >>> set_env_data('RUNNER_OS', 'Windows')
     >>> assert is_ci_runner_os_linux() == False
 
     >>> # Teardown
     >>> set_env_data('RUNNER_OS', save_gha_os_name)
-
     """
     return get_env_data("RUNNER_OS").lower() == "linux"
 
 
 def is_ci_runner_os_macos() -> bool:
     """
     if the ci runner os is macos
@@ -1070,22 +1005,20 @@
     >>> # Setup
     >>> save_gha_os_name = get_env_data('RUNNER_OS')
 
     >>> # runner.os == 'linux'
     >>> set_env_data('RUNNER_OS', 'Linux')
     >>> assert is_ci_runner_os_macos() == False
 
-    >>> # TRAVIS_OS_NAME == 'windows'
+    >>> # RUNNER_OS == 'macOS'
     >>> set_env_data('RUNNER_OS', 'macOS')
     >>> assert is_ci_runner_os_macos() == True
 
     >>> # Teardown
     >>> set_env_data('RUNNER_OS', save_gha_os_name)
-
-
     """
     return get_env_data("RUNNER_OS").lower() == "macos"
 
 
 def do_deploy() -> bool:
     """
     if we should deploy
@@ -1100,39 +1033,35 @@
     GITHUB_EVENT_NAME
         from environment
 
     Examples:
 
     >>> # Setup
     >>> save_github_event_name = get_env_data('GITHUB_EVENT_NAME')
-    >>> save_deploy_sdist = get_env_data('DEPLOY_SDIST')
-    >>> save_deploy_wheel = get_env_data('DEPLOY_WHEEL')
+    >>> save_build = get_env_data('BUILD')
 
     >>> # no Tagged Commit
     >>> set_env_data('GITHUB_EVENT_NAME', 'push')
     >>> assert False == do_deploy()
 
     >>> # Tagged Commit, DEPLOY_SDIST, DEPLOY_WHEEL != True
     >>> set_env_data('GITHUB_EVENT_NAME', 'release')
-    >>> set_env_data('DEPLOY_SDIST', '')
-    >>> set_env_data('DEPLOY_WHEEL', '')
+    >>> set_env_data('BUILD', '')
     >>> assert False == do_deploy()
 
     >>> # Tagged Commit, DEPLOY_SDIST == True
     >>> set_env_data('GITHUB_EVENT_NAME', 'release')
-    >>> set_env_data('DEPLOY_SDIST', 'True')
-    >>> set_env_data('DEPLOY_WHEEL', '')
+    >>> set_env_data('BUILD', 'True')
     >>> assert True == do_deploy()
 
     >>> # Teardown
     >>> set_env_data('GITHUB_EVENT_NAME', save_github_event_name)
-    >>> set_env_data('DEPLOY_SDIST', save_deploy_sdist)
-    >>> set_env_data('DEPLOY_WHEEL', save_deploy_wheel)
+    >>> set_env_data('BUILD', save_build)
     """
-    return (do_deploy_sdist() or do_deploy_wheel()) and is_release()
+    return do_build() and is_release()
 
 
 def is_release() -> bool:
     """
     Returns True, if this is a release (and then we deploy to pypi probably)
     """
     return get_env_data("GITHUB_EVENT_NAME") == "release"
@@ -1145,15 +1074,14 @@
 
     >>> # Test
     >>> set_env_data('MYPYPATH', 'some_test')
     >>> assert get_env_data('MYPYPATH') == 'some_test'
 
     >>> # Teardown
     >>> set_env_data('MYPYPATH', save_mypy_path)
-
     """
     if env_variable in os.environ:
         env_data = os.environ[env_variable]
     else:
         env_data = ""
     return env_data
 
@@ -1162,17 +1090,29 @@
     os.environ[env_variable] = env_str
 
 
 def is_github_actions_active() -> bool:
     """
     if we are on github actions environment
 
+    >>> # Test
     >>> assert is_github_actions_active() == is_github_actions_active()
     """
     return bool(get_env_data("CI") and get_env_data("GITHUB_WORKFLOW") and get_env_data("GITHUB_RUN_ID"))
 
 
+def run_mypy_tests(package_name: str, python_prefix: str) -> None:
+    crate_mypy_cache_directory()
+    mypy_options = get_env_data("MYPY_OPTIONS")
+    run(description="mypy tests", command=f"{python_prefix} -m mypy -p {package_name} {mypy_options}")
+
+
+def crate_mypy_cache_directory() -> None:
+    path_mypy_cache_dir = pathlib.Path.cwd() / '.mypy_cache'
+    path_mypy_cache_dir.mkdir(exist_ok=True)
+
+
 if __name__ == "__main__":
     print(
         b'this is a library only, the executable is named "lib_cicd_github_cli.py"',
         file=sys.stderr,
     )
```

### Comparing `lib_cicd_github-1.0.1.2/PKG-INFO` & `lib_cicd_github-1.0.2/lib_cicd_github.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,72 +1,73 @@
 Metadata-Version: 2.1
-Name: lib_cicd_github
-Version: 1.0.1.2
+Name: lib-cicd-github
+Version: 1.0.2
 Summary: CI/CD (Continuous Integration / Continuous Delivery) - utils for github actions
-Home-page: https://github.com/bitranox/lib_cicd_github
-Author: Robert Nowotny
-Author-email: bitranox@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
+Author-email: Robert Nowotny <bitranox@gmail.com>
+License: MIT
+Project-URL: Homepage, https://github.com/bitranox/lib_cicd_github
+Project-URL: Documentation, https://github.com/bitranox/lib_cicd_github/blob/master/README.rst
+Project-URL: Repository, https://github.com/bitranox/lib_cicd_github.git
+Project-URL: Changelog, https://github.com/bitranox/lib_cicd_github/blob/master/CHANGES.rst
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
 
 lib_cicd_github
 ===============
 
 
-Version v1.0.1.2 as of 2022-06-02 see `Changelog`_
+Version v1.0.2 as of 2023-07-21 see `Changelog`_
 
-|build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
-
-|codecov| |better_code| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+|build_badge| |codeql| |license| |jupyter| |pypi|
+|pypi-downloads| |black| |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/lib_cicd_github/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/lib_cicd_github/actions/workflows/python-package.yml
 
 
+.. |codeql| image:: https://github.com/bitranox/lib_cicd_github/actions/workflows/codeql-analysis.yml/badge.svg?event=push
+   :target: https://github.com//bitranox/lib_cicd_github/actions/workflows/codeql-analysis.yml
+
 .. |license| image:: https://img.shields.io/github/license/webcomics/pywine.svg
    :target: http://en.wikipedia.org/wiki/MIT_License
 
 .. |jupyter| image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/bitranox/lib_cicd_github/master?filepath=lib_cicd_github.ipynb
 
 .. for the pypi status link note the dashes, not the underscore !
 .. |pypi| image:: https://img.shields.io/pypi/status/lib-cicd-github?label=PyPI%20Package
    :target: https://badge.fury.io/py/lib_cicd_github
 
 .. |codecov| image:: https://img.shields.io/codecov/c/github/bitranox/lib_cicd_github
    :target: https://codecov.io/gh/bitranox/lib_cicd_github
 
-.. |better_code| image:: https://bettercodehub.com/edge/badge/bitranox/lib_cicd_github?branch=master
-   :target: https://bettercodehub.com/results/bitranox/lib_cicd_github
-
 .. |cc_maintain| image:: https://img.shields.io/codeclimate/maintainability-percentage/bitranox/lib_cicd_github?label=CC%20maintainability
    :target: https://codeclimate.com/github/bitranox/lib_cicd_github/maintainability
    :alt: Maintainability
 
 .. |cc_issues| image:: https://img.shields.io/codeclimate/issues/bitranox/lib_cicd_github?label=CC%20issues
    :target: https://codeclimate.com/github/bitranox/lib_cicd_github/maintainability
    :alt: Maintainability
 
 .. |cc_coverage| image:: https://img.shields.io/codeclimate/coverage/bitranox/lib_cicd_github?label=CC%20coverage
    :target: https://codeclimate.com/github/bitranox/lib_cicd_github/test_coverage
    :alt: Code Coverage
 
-.. |snyk| image:: https://img.shields.io/snyk/vulnerabilities/github/bitranox/lib_cicd_github
+.. |snyk| image:: https://snyk.io/test/github/bitranox/lib_cicd_github/badge.svg
    :target: https://snyk.io/test/github/bitranox/lib_cicd_github
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/lib-cicd-github
    :target: https://pypi.org/project/lib-cicd-github/
@@ -75,22 +76,22 @@
 small utils for github actions:
  - print colored banners
  - wrap commands into run/success/error banners, with automatic retry
  - resolve the branch to test, based on the environment variables
 
 ----
 
-automated tests, Travis Matrix, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
+automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
-Python version required: 3.6.0 or newer
+Python version required: 3.8.0 or newer
 
-tested on recent linux with python 3.6, 3.7, 3.8, 3.9, 3.10, pypy-3.8 - architectures: amd64
+tested on recent linux with python 3.8, 3.9, 3.10, 3.11, 3.12-dev, pypy-3.9, pypy-3.10 - architectures: amd64
 
-`100% code coverage <https://codecov.io/gh/bitranox/lib_cicd_github>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/lib_cicd_github/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
+`100% code coverage <https://codeclimate.com/github/bitranox/lib_cicd_github/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/lib_cicd_github/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
 - `Usage from Commandline`_
 - `Installation and Upgrade`_
@@ -145,26 +146,27 @@
         cPIP
             from environment, the command to launch pip, like "python -m pip"
 
 
         Examples
         --------
 
+        >>> # Test
         >>> if is_github_actions_active():
         ...     install(dry_run=True)
 
         """
 
 - script, run all tests
 
 .. code-block:: python
 
     def script(dry_run: bool = True) -> None:
         """
-        travis jobs to run in travis.yml section "script":
+        jobs to run in CICD section "script":
         - run setup.py test
         - run pip with install option test
         - run pip standard install
         - test the CLI Registration
         - install the test requirements
         - install codecov
         - install pytest-codecov
@@ -180,15 +182,15 @@
         cPREFIX
             from environment, the command prefix like 'wine' or ''
         cPIP
             from environment, the command to launch pip, like "python -m pip"
         cPYTHON
             from environment, the command to launch python, like 'python' or 'python3' on MacOS
         CLI_COMMAND
-            from environment, must be set in travis - the CLI command to test with option --version
+            from environment, must be set in CICD configuration file - the CLI command to test with option --version
         MYPY_STRICT
             from environment, if pytest with mypy --strict should run
         PACKAGE_NAME
             from environment, the package name to pass to mypy
         BUILD_DOCS
             from environment, if rst file should be rebuilt
         RST_INCLUDE_SOURCE
@@ -200,46 +202,46 @@
             only if setup.py exists and on non-tagged builds (there we deploy for real)
         dry_run
             if set, this returns immediately - for CLI tests
 
 
         Examples
         --------
+        >>> # test
         >>> script()
 
         """
 
 - after_success, upload code coverage and codeclimate reports
 
 .. code-block:: python
 
     def after_success(dry_run: bool = True) -> None:
         """
-        travis jobs to run in travis.yml section "after_success":
+        jobs to run in CICD "after_success":
             - coverage report
             - codecov
             - codeclimate report upload
 
 
         Parameter
         ---------
         cPREFIX
             from environment, the command prefix like 'wine' or ''
         cPIP
             from environment, the command to launch pip, like "python -m pip"
         CC_TEST_REPORTER_ID
-            from environment, must be set in travis
-        TRAVIS_TEST_RESULT
-            from environment, this is set by TRAVIS automatically
+            from environment, must be set in CICD configuration file
         dry_run
             if set, this returns immediately - for CLI tests
 
 
         Examples
         --------
+        >>> # test
         >>> after_success()
 
         """
 
 - deploy, deploy to pypi
 
 .. code-block:: python
@@ -251,24 +253,23 @@
 
         Parameter
         ---------
         cPREFIX
             from environment, the command prefix like 'wine' or ''
         PYPI_PASSWORD
             from environment, passed as secure, encrypted variable to environment
-        TRAVIS_TAG
-            from environment, needs to be set
         DEPLOY_SDIST, DEPLOY_WHEEL
             from environment, one of it needs to be true
         dry_run
             if set, this returns immediately - for CLI tests
 
 
         Examples
         --------
+        >>> # test
         >>> deploy()
 
         """
 
 - get_branch, determine the branch to work on
 
 .. code-block:: python
@@ -456,15 +457,15 @@
 
             # FLAKE8 tests
             DO_FLAKE8_TESTS: "True"
 
             # MYPY tests
             MYPY_DO_TESTS: "True"
             MYPY_OPTIONS: "--follow-imports=normal --ignore-missing-imports --implicit-reexport --install-types --no-warn-unused-ignores --non-interactive --strict"
-            MYPYPATH: "./lib_cicd_github/3rd_party_stubs"
+            MYPYPATH: "./.3rd_party_stubs"
 
             # coverage
             DO_COVERAGE: "True"
             DO_COVERAGE_UPLOAD_CODECOV: "True"
             DO_COVERAGE_UPLOAD_CODE_CLIMATE: "True"
 
             # package name
@@ -481,113 +482,117 @@
             PYPI_PASSWORD: ${{ secrets.PYPI_PASSWORD }}
 
 
         strategy:
           matrix:
             include:
               # https://docs.github.com/en/actions/using-github-hosted-runners/about-github-hosted-runners#supported-software
+              # https://github.com/actions/setup-python/blob/main/docs/advanced-usage.md#available-versions-of-python-and-pypy
 
               - os: windows-latest
-                python-version: "3.10"
+                python-version: "3.11"
                 env:
                   cEXPORT: "SET"
                   BUILD_DOCS: "False"
-                  DEPLOY_SDIST: "False"
-                  DEPLOY_WHEEL: "False"
-                  DEPLOY_TEST: "False"
+                  BUILD: "False"
+                  BUILD_TEST: "False"
                   MYPY_DO_TESTS: "True"
                   # Setup tests
                   DO_SETUP_INSTALL: "False"
                   DO_SETUP_INSTALL_TEST: "True"
                   # Test registered CLI Command
                   DO_CLI_TEST: "True"
 
 
               - os: ubuntu-latest
-                python-version: "3.6"
+                python-version: "3.8"
                 env:
                   BUILD_DOCS: "False"
-                  DEPLOY_SDIST: "True"
-                  DEPLOY_WHEEL: "True"
-                  DEPLOY_TEST: "True"
+                  BUILD: "True"
+                  BUILD_TEST: "True"
                   MYPY_DO_TESTS: "True"
                   DO_SETUP_INSTALL: "True"
-                  DO_SETUP_INSTALL_TEST: "False"
+                  DO_SETUP_INSTALL_TEST: "True"
                   DO_CLI_TEST: "True"
 
               - os: ubuntu-latest
-                python-version: "3.7"
+                python-version: "3.9"
                 env:
                   BUILD_DOCS: "False"
-                  DEPLOY_SDIST: "True"
-                  DEPLOY_WHEEL: "True"
-                  DEPLOY_TEST: "True"
+                  BUILD: "True"
+                  BUILD_TEST: "True"
                   MYPY_DO_TESTS: "True"
                   DO_SETUP_INSTALL: "True"
-                  DO_SETUP_INSTALL_TEST: "False"
+                  DO_SETUP_INSTALL_TEST: "True"
                   DO_CLI_TEST: "True"
 
               - os: ubuntu-latest
-                python-version: "3.8"
+                python-version: "3.10"
                 env:
                   BUILD_DOCS: "False"
-                  DEPLOY_SDIST: "True"
-                  DEPLOY_WHEEL: "True"
-                  DEPLOY_TEST: "True"
+                  BUILD: "True"
+                  BUILD_TEST: "True"
                   MYPY_DO_TESTS: "True"
                   DO_SETUP_INSTALL: "True"
-                  DO_SETUP_INSTALL_TEST: "False"
+                  DO_SETUP_INSTALL_TEST: "True"
                   DO_CLI_TEST: "True"
 
               - os: ubuntu-latest
-                python-version: "3.9"
+                python-version: "3.11"
                 env:
-                  BUILD_DOCS: "False"
-                  DEPLOY_SDIST: "True"
-                  DEPLOY_WHEEL: "True"
-                  DEPLOY_TEST: "True"
+                  BUILD_DOCS: "True"
+                  BUILD: "True"
+                  BUILD_TEST: "True"
                   MYPY_DO_TESTS: "True"
                   DO_SETUP_INSTALL: "True"
-                  DO_SETUP_INSTALL_TEST: "False"
+                  DO_SETUP_INSTALL_TEST: "True"
                   DO_CLI_TEST: "True"
 
               - os: ubuntu-latest
-                python-version: "3.10"
+                python-version: "3.12-dev"
                 env:
                   BUILD_DOCS: "True"
-                  DEPLOY_SDIST: "True"
-                  DEPLOY_WHEEL: "True"
-                  DEPLOY_TEST: "True"
+                  BUILD: "True"
+                  BUILD_TEST: "True"
                   MYPY_DO_TESTS: "True"
                   DO_SETUP_INSTALL: "True"
                   DO_SETUP_INSTALL_TEST: "True"
                   DO_CLI_TEST: "True"
 
               - os: ubuntu-latest
-                python-version: "pypy-3.8"
+                python-version: "pypy-3.9"
                 env:
                   BUILD_DOCS: "False"
-                  DEPLOY_SDIST: "True"
-                  DEPLOY_WHEEL: "True"
-                  DEPLOY_TEST: "True"
-                  MYPY_DO_TESTS: "False"
+                  BUILD: "True"
+                  BUILD_TEST: "True"
+                  MYPY_DO_TESTS: "True"
                   DO_SETUP_INSTALL: "True"
-                  DO_SETUP_INSTALL_TEST: "False"
+                  DO_SETUP_INSTALL_TEST: "True"
+                  DO_CLI_TEST: "True"
+
+              - os: ubuntu-latest
+                python-version: "pypy-3.10"
+                env:
+                  BUILD_DOCS: "False"
+                  BUILD: "True"
+                  BUILD_TEST: "True"
+                  MYPY_DO_TESTS: "True"
+                  DO_SETUP_INSTALL: "True"
+                  DO_SETUP_INSTALL_TEST: "True"
                   DO_CLI_TEST: "True"
 
               - os: macos-latest
-                python-version: "3.10"
+                python-version: "3.11"
                 env:
                   cPREFIX: ""               # prefix before commands - used for wine, there the prefix is "wine"
                   cPYTHON: "python3"        # command to launch python interpreter (it's different on macOS, there we need python3)
                   cPIP: "python3 -m pip"    # command to launch pip (it's different on macOS, there we need pip3)
                   BUILD_DOCS: "False"
-                  DEPLOY_SDIST: "True"
-                  DEPLOY_WHEEL: "True"
-                  DEPLOY_TEST: "True"
+                  BUILD: "True"
+                  BUILD_TEST: "True"
                   MYPY_DO_TESTS: "True"
                   # Setup tests
                   DO_SETUP_INSTALL: "True"
                   DO_SETUP_INSTALL_TEST: "True"
                   # Test registered CLI Command
                   DO_CLI_TEST: "True"
 
@@ -595,15 +600,16 @@
         name: "${{ matrix.os }} Python ${{ matrix.python-version }}"
 
         steps:
         # see : https://github.com/actions/checkout
         - uses: actions/checkout@v3
 
         - name: Setting up Python ${{ matrix.python-version }}
-          uses: actions/setup-python@v3
+          # see: https://github.com/actions/setup-python
+          uses: actions/setup-python@v4
           with:
             python-version: ${{ matrix.python-version }}
 
         - name: Install dependencies
           # see: https://github.community/t/github-actions-new-bug-unable-to-create-environment-variables-based-matrix/16104/3
           env: ${{ matrix.env }}             # make matrix env variables accessible
           # lib_cicd_github install: upgrades pip, setuptools, wheel and pytest-pycodestyle
@@ -704,14 +710,21 @@
 
 - to install the latest release from PyPi via pip (recommended):
 
 .. code-block::
 
     python -m pip install --upgrade lib_cicd_github
 
+
+- to install the latest release from PyPi via pip, including test dependencies:
+
+.. code-block::
+
+    python -m pip install --upgrade lib_cicd_github[test]
+
 - to install the latest version from github via pip:
 
 
 .. code-block::
 
     python -m pip install --upgrade git+https://github.com/bitranox/lib_cicd_github.git
 
@@ -727,22 +740,22 @@
     # for the latest development version :
     lib_cicd_github @ git+https://github.com/bitranox/lib_cicd_github.git
 
     # to install and upgrade all modules mentioned in requirements.txt:
     python -m pip install --upgrade -r /<path>/requirements.txt
 
 
-- to install the latest development version from source code:
+- to install the latest development version, including test dependencies from source code:
 
 .. code-block::
 
     # cd ~
     $ git clone https://github.com/bitranox/lib_cicd_github.git
     $ cd lib_cicd_github
-    python setup.py install
+    python -m pip install -e .[test]
 
 - via makefile:
   makefiles are a very convenient way to install. Here we can do much more,
   like installing virtual environments, clean caches and so on.
 
 .. code-block:: shell
 
@@ -796,14 +809,36 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v1.0.2
+--------
+2023-07-21:
+    - create mypy cache dir '.mypy_cache'
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
+
 v1.0.1.2
 ---------
 2022-06-02: update to github actions checkout@v3 and setup-python@v3
 
 v1.0.1
 --------
 2022-03-29: remedy mypy Untyped decorator in cli
@@ -815,9 +850,7 @@
  - update documentation and tests
  - list ./dist dir if existing
 
 v0.0.1
 ---------
 2021-08-23: initial release
 
-
-
```

### Comparing `lib_cicd_github-1.0.1.2/lib_cicd_github.egg-info/PKG-INFO` & `lib_cicd_github-1.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,72 +1,73 @@
 Metadata-Version: 2.1
-Name: lib-cicd-github
-Version: 1.0.1.2
+Name: lib_cicd_github
+Version: 1.0.2
 Summary: CI/CD (Continuous Integration / Continuous Delivery) - utils for github actions
-Home-page: https://github.com/bitranox/lib_cicd_github
-Author: Robert Nowotny
-Author-email: bitranox@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
+Author-email: Robert Nowotny <bitranox@gmail.com>
+License: MIT
+Project-URL: Homepage, https://github.com/bitranox/lib_cicd_github
+Project-URL: Documentation, https://github.com/bitranox/lib_cicd_github/blob/master/README.rst
+Project-URL: Repository, https://github.com/bitranox/lib_cicd_github.git
+Project-URL: Changelog, https://github.com/bitranox/lib_cicd_github/blob/master/CHANGES.rst
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
 
 lib_cicd_github
 ===============
 
 
-Version v1.0.1.2 as of 2022-06-02 see `Changelog`_
+Version v1.0.2 as of 2023-07-21 see `Changelog`_
 
-|build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
-
-|codecov| |better_code| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+|build_badge| |codeql| |license| |jupyter| |pypi|
+|pypi-downloads| |black| |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/lib_cicd_github/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/lib_cicd_github/actions/workflows/python-package.yml
 
 
+.. |codeql| image:: https://github.com/bitranox/lib_cicd_github/actions/workflows/codeql-analysis.yml/badge.svg?event=push
+   :target: https://github.com//bitranox/lib_cicd_github/actions/workflows/codeql-analysis.yml
+
 .. |license| image:: https://img.shields.io/github/license/webcomics/pywine.svg
    :target: http://en.wikipedia.org/wiki/MIT_License
 
 .. |jupyter| image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/bitranox/lib_cicd_github/master?filepath=lib_cicd_github.ipynb
 
 .. for the pypi status link note the dashes, not the underscore !
 .. |pypi| image:: https://img.shields.io/pypi/status/lib-cicd-github?label=PyPI%20Package
    :target: https://badge.fury.io/py/lib_cicd_github
 
 .. |codecov| image:: https://img.shields.io/codecov/c/github/bitranox/lib_cicd_github
    :target: https://codecov.io/gh/bitranox/lib_cicd_github
 
-.. |better_code| image:: https://bettercodehub.com/edge/badge/bitranox/lib_cicd_github?branch=master
-   :target: https://bettercodehub.com/results/bitranox/lib_cicd_github
-
 .. |cc_maintain| image:: https://img.shields.io/codeclimate/maintainability-percentage/bitranox/lib_cicd_github?label=CC%20maintainability
    :target: https://codeclimate.com/github/bitranox/lib_cicd_github/maintainability
    :alt: Maintainability
 
 .. |cc_issues| image:: https://img.shields.io/codeclimate/issues/bitranox/lib_cicd_github?label=CC%20issues
    :target: https://codeclimate.com/github/bitranox/lib_cicd_github/maintainability
    :alt: Maintainability
 
 .. |cc_coverage| image:: https://img.shields.io/codeclimate/coverage/bitranox/lib_cicd_github?label=CC%20coverage
    :target: https://codeclimate.com/github/bitranox/lib_cicd_github/test_coverage
    :alt: Code Coverage
 
-.. |snyk| image:: https://img.shields.io/snyk/vulnerabilities/github/bitranox/lib_cicd_github
+.. |snyk| image:: https://snyk.io/test/github/bitranox/lib_cicd_github/badge.svg
    :target: https://snyk.io/test/github/bitranox/lib_cicd_github
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/lib-cicd-github
    :target: https://pypi.org/project/lib-cicd-github/
@@ -75,22 +76,22 @@
 small utils for github actions:
  - print colored banners
  - wrap commands into run/success/error banners, with automatic retry
  - resolve the branch to test, based on the environment variables
 
 ----
 
-automated tests, Travis Matrix, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
+automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
-Python version required: 3.6.0 or newer
+Python version required: 3.8.0 or newer
 
-tested on recent linux with python 3.6, 3.7, 3.8, 3.9, 3.10, pypy-3.8 - architectures: amd64
+tested on recent linux with python 3.8, 3.9, 3.10, 3.11, 3.12-dev, pypy-3.9, pypy-3.10 - architectures: amd64
 
-`100% code coverage <https://codecov.io/gh/bitranox/lib_cicd_github>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/lib_cicd_github/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
+`100% code coverage <https://codeclimate.com/github/bitranox/lib_cicd_github/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/lib_cicd_github/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
 - `Usage from Commandline`_
 - `Installation and Upgrade`_
@@ -145,26 +146,27 @@
         cPIP
             from environment, the command to launch pip, like "python -m pip"
 
 
         Examples
         --------
 
+        >>> # Test
         >>> if is_github_actions_active():
         ...     install(dry_run=True)
 
         """
 
 - script, run all tests
 
 .. code-block:: python
 
     def script(dry_run: bool = True) -> None:
         """
-        travis jobs to run in travis.yml section "script":
+        jobs to run in CICD section "script":
         - run setup.py test
         - run pip with install option test
         - run pip standard install
         - test the CLI Registration
         - install the test requirements
         - install codecov
         - install pytest-codecov
@@ -180,15 +182,15 @@
         cPREFIX
             from environment, the command prefix like 'wine' or ''
         cPIP
             from environment, the command to launch pip, like "python -m pip"
         cPYTHON
             from environment, the command to launch python, like 'python' or 'python3' on MacOS
         CLI_COMMAND
-            from environment, must be set in travis - the CLI command to test with option --version
+            from environment, must be set in CICD configuration file - the CLI command to test with option --version
         MYPY_STRICT
             from environment, if pytest with mypy --strict should run
         PACKAGE_NAME
             from environment, the package name to pass to mypy
         BUILD_DOCS
             from environment, if rst file should be rebuilt
         RST_INCLUDE_SOURCE
@@ -200,46 +202,46 @@
             only if setup.py exists and on non-tagged builds (there we deploy for real)
         dry_run
             if set, this returns immediately - for CLI tests
 
 
         Examples
         --------
+        >>> # test
         >>> script()
 
         """
 
 - after_success, upload code coverage and codeclimate reports
 
 .. code-block:: python
 
     def after_success(dry_run: bool = True) -> None:
         """
-        travis jobs to run in travis.yml section "after_success":
+        jobs to run in CICD "after_success":
             - coverage report
             - codecov
             - codeclimate report upload
 
 
         Parameter
         ---------
         cPREFIX
             from environment, the command prefix like 'wine' or ''
         cPIP
             from environment, the command to launch pip, like "python -m pip"
         CC_TEST_REPORTER_ID
-            from environment, must be set in travis
-        TRAVIS_TEST_RESULT
-            from environment, this is set by TRAVIS automatically
+            from environment, must be set in CICD configuration file
         dry_run
             if set, this returns immediately - for CLI tests
 
 
         Examples
         --------
+        >>> # test
         >>> after_success()
 
         """
 
 - deploy, deploy to pypi
 
 .. code-block:: python
@@ -251,24 +253,23 @@
 
         Parameter
         ---------
         cPREFIX
             from environment, the command prefix like 'wine' or ''
         PYPI_PASSWORD
             from environment, passed as secure, encrypted variable to environment
-        TRAVIS_TAG
-            from environment, needs to be set
         DEPLOY_SDIST, DEPLOY_WHEEL
             from environment, one of it needs to be true
         dry_run
             if set, this returns immediately - for CLI tests
 
 
         Examples
         --------
+        >>> # test
         >>> deploy()
 
         """
 
 - get_branch, determine the branch to work on
 
 .. code-block:: python
@@ -456,15 +457,15 @@
 
             # FLAKE8 tests
             DO_FLAKE8_TESTS: "True"
 
             # MYPY tests
             MYPY_DO_TESTS: "True"
             MYPY_OPTIONS: "--follow-imports=normal --ignore-missing-imports --implicit-reexport --install-types --no-warn-unused-ignores --non-interactive --strict"
-            MYPYPATH: "./lib_cicd_github/3rd_party_stubs"
+            MYPYPATH: "./.3rd_party_stubs"
 
             # coverage
             DO_COVERAGE: "True"
             DO_COVERAGE_UPLOAD_CODECOV: "True"
             DO_COVERAGE_UPLOAD_CODE_CLIMATE: "True"
 
             # package name
@@ -481,113 +482,117 @@
             PYPI_PASSWORD: ${{ secrets.PYPI_PASSWORD }}
 
 
         strategy:
           matrix:
             include:
               # https://docs.github.com/en/actions/using-github-hosted-runners/about-github-hosted-runners#supported-software
+              # https://github.com/actions/setup-python/blob/main/docs/advanced-usage.md#available-versions-of-python-and-pypy
 
               - os: windows-latest
-                python-version: "3.10"
+                python-version: "3.11"
                 env:
                   cEXPORT: "SET"
                   BUILD_DOCS: "False"
-                  DEPLOY_SDIST: "False"
-                  DEPLOY_WHEEL: "False"
-                  DEPLOY_TEST: "False"
+                  BUILD: "False"
+                  BUILD_TEST: "False"
                   MYPY_DO_TESTS: "True"
                   # Setup tests
                   DO_SETUP_INSTALL: "False"
                   DO_SETUP_INSTALL_TEST: "True"
                   # Test registered CLI Command
                   DO_CLI_TEST: "True"
 
 
               - os: ubuntu-latest
-                python-version: "3.6"
+                python-version: "3.8"
                 env:
                   BUILD_DOCS: "False"
-                  DEPLOY_SDIST: "True"
-                  DEPLOY_WHEEL: "True"
-                  DEPLOY_TEST: "True"
+                  BUILD: "True"
+                  BUILD_TEST: "True"
                   MYPY_DO_TESTS: "True"
                   DO_SETUP_INSTALL: "True"
-                  DO_SETUP_INSTALL_TEST: "False"
+                  DO_SETUP_INSTALL_TEST: "True"
                   DO_CLI_TEST: "True"
 
               - os: ubuntu-latest
-                python-version: "3.7"
+                python-version: "3.9"
                 env:
                   BUILD_DOCS: "False"
-                  DEPLOY_SDIST: "True"
-                  DEPLOY_WHEEL: "True"
-                  DEPLOY_TEST: "True"
+                  BUILD: "True"
+                  BUILD_TEST: "True"
                   MYPY_DO_TESTS: "True"
                   DO_SETUP_INSTALL: "True"
-                  DO_SETUP_INSTALL_TEST: "False"
+                  DO_SETUP_INSTALL_TEST: "True"
                   DO_CLI_TEST: "True"
 
               - os: ubuntu-latest
-                python-version: "3.8"
+                python-version: "3.10"
                 env:
                   BUILD_DOCS: "False"
-                  DEPLOY_SDIST: "True"
-                  DEPLOY_WHEEL: "True"
-                  DEPLOY_TEST: "True"
+                  BUILD: "True"
+                  BUILD_TEST: "True"
                   MYPY_DO_TESTS: "True"
                   DO_SETUP_INSTALL: "True"
-                  DO_SETUP_INSTALL_TEST: "False"
+                  DO_SETUP_INSTALL_TEST: "True"
                   DO_CLI_TEST: "True"
 
               - os: ubuntu-latest
-                python-version: "3.9"
+                python-version: "3.11"
                 env:
-                  BUILD_DOCS: "False"
-                  DEPLOY_SDIST: "True"
-                  DEPLOY_WHEEL: "True"
-                  DEPLOY_TEST: "True"
+                  BUILD_DOCS: "True"
+                  BUILD: "True"
+                  BUILD_TEST: "True"
                   MYPY_DO_TESTS: "True"
                   DO_SETUP_INSTALL: "True"
-                  DO_SETUP_INSTALL_TEST: "False"
+                  DO_SETUP_INSTALL_TEST: "True"
                   DO_CLI_TEST: "True"
 
               - os: ubuntu-latest
-                python-version: "3.10"
+                python-version: "3.12-dev"
                 env:
                   BUILD_DOCS: "True"
-                  DEPLOY_SDIST: "True"
-                  DEPLOY_WHEEL: "True"
-                  DEPLOY_TEST: "True"
+                  BUILD: "True"
+                  BUILD_TEST: "True"
                   MYPY_DO_TESTS: "True"
                   DO_SETUP_INSTALL: "True"
                   DO_SETUP_INSTALL_TEST: "True"
                   DO_CLI_TEST: "True"
 
               - os: ubuntu-latest
-                python-version: "pypy-3.8"
+                python-version: "pypy-3.9"
                 env:
                   BUILD_DOCS: "False"
-                  DEPLOY_SDIST: "True"
-                  DEPLOY_WHEEL: "True"
-                  DEPLOY_TEST: "True"
-                  MYPY_DO_TESTS: "False"
+                  BUILD: "True"
+                  BUILD_TEST: "True"
+                  MYPY_DO_TESTS: "True"
                   DO_SETUP_INSTALL: "True"
-                  DO_SETUP_INSTALL_TEST: "False"
+                  DO_SETUP_INSTALL_TEST: "True"
+                  DO_CLI_TEST: "True"
+
+              - os: ubuntu-latest
+                python-version: "pypy-3.10"
+                env:
+                  BUILD_DOCS: "False"
+                  BUILD: "True"
+                  BUILD_TEST: "True"
+                  MYPY_DO_TESTS: "True"
+                  DO_SETUP_INSTALL: "True"
+                  DO_SETUP_INSTALL_TEST: "True"
                   DO_CLI_TEST: "True"
 
               - os: macos-latest
-                python-version: "3.10"
+                python-version: "3.11"
                 env:
                   cPREFIX: ""               # prefix before commands - used for wine, there the prefix is "wine"
                   cPYTHON: "python3"        # command to launch python interpreter (it's different on macOS, there we need python3)
                   cPIP: "python3 -m pip"    # command to launch pip (it's different on macOS, there we need pip3)
                   BUILD_DOCS: "False"
-                  DEPLOY_SDIST: "True"
-                  DEPLOY_WHEEL: "True"
-                  DEPLOY_TEST: "True"
+                  BUILD: "True"
+                  BUILD_TEST: "True"
                   MYPY_DO_TESTS: "True"
                   # Setup tests
                   DO_SETUP_INSTALL: "True"
                   DO_SETUP_INSTALL_TEST: "True"
                   # Test registered CLI Command
                   DO_CLI_TEST: "True"
 
@@ -595,15 +600,16 @@
         name: "${{ matrix.os }} Python ${{ matrix.python-version }}"
 
         steps:
         # see : https://github.com/actions/checkout
         - uses: actions/checkout@v3
 
         - name: Setting up Python ${{ matrix.python-version }}
-          uses: actions/setup-python@v3
+          # see: https://github.com/actions/setup-python
+          uses: actions/setup-python@v4
           with:
             python-version: ${{ matrix.python-version }}
 
         - name: Install dependencies
           # see: https://github.community/t/github-actions-new-bug-unable-to-create-environment-variables-based-matrix/16104/3
           env: ${{ matrix.env }}             # make matrix env variables accessible
           # lib_cicd_github install: upgrades pip, setuptools, wheel and pytest-pycodestyle
@@ -704,14 +710,21 @@
 
 - to install the latest release from PyPi via pip (recommended):
 
 .. code-block::
 
     python -m pip install --upgrade lib_cicd_github
 
+
+- to install the latest release from PyPi via pip, including test dependencies:
+
+.. code-block::
+
+    python -m pip install --upgrade lib_cicd_github[test]
+
 - to install the latest version from github via pip:
 
 
 .. code-block::
 
     python -m pip install --upgrade git+https://github.com/bitranox/lib_cicd_github.git
 
@@ -727,22 +740,22 @@
     # for the latest development version :
     lib_cicd_github @ git+https://github.com/bitranox/lib_cicd_github.git
 
     # to install and upgrade all modules mentioned in requirements.txt:
     python -m pip install --upgrade -r /<path>/requirements.txt
 
 
-- to install the latest development version from source code:
+- to install the latest development version, including test dependencies from source code:
 
 .. code-block::
 
     # cd ~
     $ git clone https://github.com/bitranox/lib_cicd_github.git
     $ cd lib_cicd_github
-    python setup.py install
+    python -m pip install -e .[test]
 
 - via makefile:
   makefiles are a very convenient way to install. Here we can do much more,
   like installing virtual environments, clean caches and so on.
 
 .. code-block:: shell
 
@@ -796,14 +809,36 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v1.0.2
+--------
+2023-07-21:
+    - create mypy cache dir '.mypy_cache'
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
+
 v1.0.1.2
 ---------
 2022-06-02: update to github actions checkout@v3 and setup-python@v3
 
 v1.0.1
 --------
 2022-03-29: remedy mypy Untyped decorator in cli
@@ -815,9 +850,7 @@
  - update documentation and tests
  - list ./dist dir if existing
 
 v0.0.1
 ---------
 2021-08-23: initial release
 
-
-
```

