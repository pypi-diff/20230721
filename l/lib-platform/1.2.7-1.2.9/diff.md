# Comparing `tmp/lib_platform-1.2.7.tar.gz` & `tmp/lib_platform-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lib_platform-1.2.7.tar", last modified: Fri Oct  9 15:18:00 2020, max compression
+gzip compressed data, was "lib_platform-1.2.9.tar", last modified: Fri Jul 21 09:46:15 2023, max compression
```

## Comparing `lib_platform-1.2.7.tar` & `lib_platform-1.2.9.tar`

### file list

```diff
@@ -1,22 +1,67 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-09 15:18:00.000000 lib_platform-1.2.7/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4229 2020-10-09 15:17:11.000000 lib_platform-1.2.7/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8934 2020-10-09 15:17:11.000000 lib_platform-1.2.7/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)    12167 2020-10-09 15:18:00.000000 lib_platform-1.2.7/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-09 15:18:00.000000 lib_platform-1.2.7/lib_platform.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-10-09 15:17:59.000000 lib_platform-1.2.7/lib_platform.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)      461 2020-10-09 15:18:00.000000 lib_platform-1.2.7/lib_platform.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       73 2020-10-09 15:18:00.000000 lib_platform-1.2.7/lib_platform.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       13 2020-10-09 15:18:00.000000 lib_platform-1.2.7/lib_platform.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-10-09 15:18:00.000000 lib_platform-1.2.7/lib_platform.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       34 2020-10-09 15:18:00.000000 lib_platform-1.2.7/lib_platform.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    12167 2020-10-09 15:18:00.000000 lib_platform-1.2.7/lib_platform.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      124 2020-10-09 15:17:11.000000 lib_platform-1.2.7/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)      592 2020-10-09 15:18:00.000000 lib_platform-1.2.7/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      252 2020-10-09 15:17:11.000000 lib_platform-1.2.7/pyproject.toml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-09 15:18:00.000000 lib_platform-1.2.7/lib_platform/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1554 2020-10-09 15:17:11.000000 lib_platform-1.2.7/lib_platform/lib_platform_cli.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-09 15:17:11.000000 lib_platform-1.2.7/lib_platform/py.typed
--rw-rw-r--   0 travis    (2000) travis    (2000)     5440 2020-10-09 15:17:11.000000 lib_platform-1.2.7/lib_platform/lib_platform.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      542 2020-10-09 15:17:11.000000 lib_platform-1.2.7/lib_platform/__init__conf__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      333 2020-10-09 15:17:11.000000 lib_platform-1.2.7/lib_platform/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1296 2020-10-09 15:17:11.000000 lib_platform-1.2.7/CHANGES.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:46:15.131340 lib_platform-1.2.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:46:15.123340 lib_platform-1.2.9/.3rd_party_stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-21 09:45:20.000000 lib_platform-1.2.9/.3rd_party_stubs/readme.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-21 09:45:20.000000 lib_platform-1.2.9/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:46:15.127340 lib_platform-1.2.9/.docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-21 09:45:20.000000 lib_platform-1.2.9/.docs/README_template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-21 09:45:20.000000 lib_platform-1.2.9/.docs/acknowledgment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-07-21 09:45:20.000000 lib_platform-1.2.9/.docs/badges.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-21 09:45:20.000000 lib_platform-1.2.9/.docs/commandline_help.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-21 09:45:20.000000 lib_platform-1.2.9/.docs/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-21 09:45:20.000000 lib_platform-1.2.9/.docs/description.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-21 09:45:20.000000 lib_platform-1.2.9/.docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-21 09:45:20.000000 lib_platform-1.2.9/.docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-21 09:45:20.000000 lib_platform-1.2.9/.docs/installation_via_makefile.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-21 09:45:20.000000 lib_platform-1.2.9/.docs/installation_via_pypi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-21 09:45:20.000000 lib_platform-1.2.9/.docs/licence_mit.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-21 09:45:20.000000 lib_platform-1.2.9/.docs/tested_under.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-21 09:45:20.000000 lib_platform-1.2.9/.docs/try_in_jupyter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-21 09:45:20.000000 lib_platform-1.2.9/.docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-21 09:45:20.000000 lib_platform-1.2.9/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:46:15.119340 lib_platform-1.2.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:46:15.127340 lib_platform-1.2.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-21 09:45:20.000000 lib_platform-1.2.9/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9432 2023-07-21 09:45:20.000000 lib_platform-1.2.9/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-21 09:45:20.000000 lib_platform-1.2.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-21 09:45:20.000000 lib_platform-1.2.9/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-21 09:45:20.000000 lib_platform-1.2.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-21 09:45:20.000000 lib_platform-1.2.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-21 09:45:20.000000 lib_platform-1.2.9/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-21 09:45:20.000000 lib_platform-1.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-21 09:45:20.000000 lib_platform-1.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-21 09:45:20.000000 lib_platform-1.2.9/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    10985 2023-07-21 09:46:15.131340 lib_platform-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-21 09:45:20.000000 lib_platform-1.2.9/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10015 2023-07-21 09:45:20.000000 lib_platform-1.2.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-21 09:45:20.000000 lib_platform-1.2.9/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-07-21 09:45:20.000000 lib_platform-1.2.9/jupyter_test_lib_platform.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:46:15.127340 lib_platform-1.2.9/lib_platform/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-21 09:45:20.000000 lib_platform-1.2.9/lib_platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-21 09:45:20.000000 lib_platform-1.2.9/lib_platform/__init__conf__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-07-21 09:45:20.000000 lib_platform-1.2.9/lib_platform/lib_platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-21 09:45:20.000000 lib_platform-1.2.9/lib_platform/lib_platform_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 09:45:20.000000 lib_platform-1.2.9/lib_platform/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:46:15.131340 lib_platform-1.2.9/lib_platform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10985 2023-07-21 09:46:15.000000 lib_platform-1.2.9/lib_platform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-21 09:46:15.000000 lib_platform-1.2.9/lib_platform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 09:46:15.000000 lib_platform-1.2.9/lib_platform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-21 09:46:15.000000 lib_platform-1.2.9/lib_platform.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-21 09:46:15.000000 lib_platform-1.2.9/lib_platform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-21 09:46:15.000000 lib_platform-1.2.9/lib_platform.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-07-21 09:45:20.000000 lib_platform-1.2.9/lib_platform.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-07-21 09:45:20.000000 lib_platform-1.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-21 09:45:20.000000 lib_platform-1.2.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-21 09:45:20.000000 lib_platform-1.2.9/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 09:46:15.131340 lib_platform-1.2.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:46:15.131340 lib_platform-1.2.9/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:46:15.131340 lib_platform-1.2.9/tests/local_testscripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     9572 2023-07-21 09:45:20.000000 lib_platform-1.2.9/tests/local_testscripts/lib_bash_functions.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-21 09:45:20.000000 lib_platform-1.2.9/tests/local_testscripts/run_clean.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-21 09:45:20.000000 lib_platform-1.2.9/tests/local_testscripts/run_pytest.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-21 09:45:20.000000 lib_platform-1.2.9/tests/local_testscripts/run_testloop.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-21 09:45:20.000000 lib_platform-1.2.9/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-21 09:45:20.000000 lib_platform-1.2.9/tests/local_testscripts/run_testloop_windows.cmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-21 09:45:20.000000 lib_platform-1.2.9/tests/local_testscripts/shellcheck.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-07-21 09:45:20.000000 lib_platform-1.2.9/tests/local_testscripts/testing_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-21 09:45:20.000000 lib_platform-1.2.9/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-07-21 09:45:20.000000 lib_platform-1.2.9/tests/test_lib_platform.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `lib_platform-1.2.7/README.rst` & `lib_platform-1.2.9/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,67 +1,94 @@
+Metadata-Version: 2.1
+Name: lib_platform
+Version: 1.2.9
+Summary: some platform related functions, which also work correctly on wine
+Author-email: Robert Nowotny <bitranox@gmail.com>
+License: MIT
+Project-URL: Homepage, https://github.com/bitranox/lib_platform
+Project-URL: Documentation, https://github.com/bitranox/lib_platform/blob/master/README.rst
+Project-URL: Repository, https://github.com/bitranox/lib_platform.git
+Project-URL: Changelog, https://github.com/bitranox/lib_platform/blob/master/CHANGES.rst
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
 lib_platform
 ============
 
 
-Version v1.2.7 as of 2020-10-09 see `Changelog`_
+Version v1.2.9 as of 2023-07-21 see `Changelog`_
+
+|build_badge| |codeql| |license| |jupyter| |pypi|
+|pypi-downloads| |black| |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+
 
-|travis_build| |license| |jupyter| |pypi|
 
-|codecov| |better_code| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+.. |build_badge| image:: https://github.com/bitranox/lib_platform/actions/workflows/python-package.yml/badge.svg
+   :target: https://github.com/bitranox/lib_platform/actions/workflows/python-package.yml
 
 
-.. |travis_build| image:: https://img.shields.io/travis/bitranox/lib_platform/master.svg
-   :target: https://travis-ci.org/bitranox/lib_platform
+.. |codeql| image:: https://github.com/bitranox/lib_platform/actions/workflows/codeql-analysis.yml/badge.svg?event=push
+   :target: https://github.com//bitranox/lib_platform/actions/workflows/codeql-analysis.yml
 
 .. |license| image:: https://img.shields.io/github/license/webcomics/pywine.svg
    :target: http://en.wikipedia.org/wiki/MIT_License
 
 .. |jupyter| image:: https://mybinder.org/badge_logo.svg
- :target: https://mybinder.org/v2/gh/bitranox/lib_platform/master?filepath=lib_platform.ipynb
+   :target: https://mybinder.org/v2/gh/bitranox/lib_platform/master?filepath=lib_platform.ipynb
 
 .. for the pypi status link note the dashes, not the underscore !
 .. |pypi| image:: https://img.shields.io/pypi/status/lib-platform?label=PyPI%20Package
    :target: https://badge.fury.io/py/lib_platform
 
 .. |codecov| image:: https://img.shields.io/codecov/c/github/bitranox/lib_platform
    :target: https://codecov.io/gh/bitranox/lib_platform
 
-.. |better_code| image:: https://bettercodehub.com/edge/badge/bitranox/lib_platform?branch=master
-   :target: https://bettercodehub.com/results/bitranox/lib_platform
-
 .. |cc_maintain| image:: https://img.shields.io/codeclimate/maintainability-percentage/bitranox/lib_platform?label=CC%20maintainability
    :target: https://codeclimate.com/github/bitranox/lib_platform/maintainability
    :alt: Maintainability
 
 .. |cc_issues| image:: https://img.shields.io/codeclimate/issues/bitranox/lib_platform?label=CC%20issues
    :target: https://codeclimate.com/github/bitranox/lib_platform/maintainability
    :alt: Maintainability
 
 .. |cc_coverage| image:: https://img.shields.io/codeclimate/coverage/bitranox/lib_platform?label=CC%20coverage
    :target: https://codeclimate.com/github/bitranox/lib_platform/test_coverage
    :alt: Code Coverage
 
-.. |snyk| image:: https://img.shields.io/snyk/vulnerabilities/github/bitranox/lib_platform
+.. |snyk| image:: https://snyk.io/test/github/bitranox/lib_platform/badge.svg
    :target: https://snyk.io/test/github/bitranox/lib_platform
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
 
+.. |pypi-downloads| image:: https://img.shields.io/pypi/dm/lib-platform
+   :target: https://pypi.org/project/lib-platform/
+   :alt: PyPI - Downloads
+
 some platform related functions, which also work correctly on wine
 
 ----
 
-automated tests, Travis Matrix, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
+automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
-Python version required: 3.6.0 or newer
+Python version required: 3.8.0 or newer
 
-tested on linux "bionic" with python 3.6, 3.7, 3.8, 3.9-dev, pypy3 - architectures: amd64, ppc64le, s390x, arm64
+tested on recent linux with python 3.8, 3.9, 3.10, 3.11, 3.12-dev, pypy-3.9, pypy-3.10 - architectures: amd64
 
-`100% code coverage <https://codecov.io/gh/bitranox/lib_platform>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://travis-ci.org/bitranox/lib_platform>`_, automatic daily builds and monitoring
+`100% code coverage <https://codeclimate.com/github/bitranox/lib_platform/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/lib_platform/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
 - `Usage from Commandline`_
 - `Installation and Upgrade`_
@@ -129,15 +156,15 @@
 
     >>> # is user administrator (has user admin rights)
     >>> is_user_admin = lib_platform.is_user_admin
 
 Usage from Commandline
 ------------------------
 
-.. code-block:: bash
+.. code-block::
 
    Usage: lib_platform [OPTIONS] COMMAND [ARGS]...
 
      some platform related functions, which also work correctly on wine
 
    Options:
      --version                     Show the version and exit.
@@ -149,56 +176,63 @@
 
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
 
     python -m pip install --upgrade lib_platform
 
+
+- to install the latest release from PyPi via pip, including test dependencies:
+
+.. code-block::
+
+    python -m pip install --upgrade lib_platform[test]
+
 - to install the latest version from github via pip:
 
 
-.. code-block:: bash
+.. code-block::
 
     python -m pip install --upgrade git+https://github.com/bitranox/lib_platform.git
 
 
 - include it into Your requirements.txt:
 
-.. code-block:: bash
+.. code-block::
 
     # Insert following line in Your requirements.txt:
     # for the latest Release on pypi:
     lib_platform
 
     # for the latest development version :
     lib_platform @ git+https://github.com/bitranox/lib_platform.git
 
     # to install and upgrade all modules mentioned in requirements.txt:
     python -m pip install --upgrade -r /<path>/requirements.txt
 
 
-- to install the latest development version from source code:
+- to install the latest development version, including test dependencies from source code:
 
-.. code-block:: bash
+.. code-block::
 
     # cd ~
     $ git clone https://github.com/bitranox/lib_platform.git
     $ cd lib_platform
-    python setup.py install
+    python -m pip install -e .[test]
 
 - via makefile:
   makefiles are a very convenient way to install. Here we can do much more,
   like installing virtual environments, clean caches and so on.
 
 .. code-block:: shell
 
@@ -222,16 +256,16 @@
 ------------
 following modules will be automatically installed :
 
 .. code-block:: bash
 
     ## Project Requirements
     click
-    cli_exit_tools @ git+https://github.com/bitranox/cli_exit_tools.git
-    lib_registry @ git+https://github.com/bitranox/lib_registry.git
+    cli_exit_tools
+    lib_registry
 
 Acknowledgements
 ----------------
 
 - special thanks to "uncle bob" Robert C. Martin, especially for his books on "clean code" and "clean architecture"
 
 Contribute
@@ -250,14 +284,39 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v1.2.9
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
+v1.2.8
+--------
+2022-11-09:
+    - fix get hostname, if something is tinkering with the loopback interface on Windows - for instance 'Solid Works 3DExperience'
+
 v1.2.7
 --------
 2020-10-09: service release
     - update travis build matrix for linux 3.9-dev
     - update travis build matrix (paths) for windows 3.9 / 3.10
 
 v1.2.6
```

### Comparing `lib_platform-1.2.7/PKG-INFO` & `lib_platform-1.2.9/lib_platform.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,335 +1,375 @@
 Metadata-Version: 2.1
-Name: lib_platform
-Version: 1.2.7
+Name: lib-platform
+Version: 1.2.9
 Summary: some platform related functions, which also work correctly on wine
-Home-page: https://github.com/bitranox/lib_platform
-Author: Robert Nowotny
-Author-email: bitranox@gmail.com
-License: UNKNOWN
-Description: lib_platform
-        ============
-        
-        
-        Version v1.2.7 as of 2020-10-09 see `Changelog`_
-        
-        |travis_build| |license| |jupyter| |pypi|
-        
-        |codecov| |better_code| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
-        
-        
-        .. |travis_build| image:: https://img.shields.io/travis/bitranox/lib_platform/master.svg
-           :target: https://travis-ci.org/bitranox/lib_platform
-        
-        .. |license| image:: https://img.shields.io/github/license/webcomics/pywine.svg
-           :target: http://en.wikipedia.org/wiki/MIT_License
-        
-        .. |jupyter| image:: https://mybinder.org/badge_logo.svg
-         :target: https://mybinder.org/v2/gh/bitranox/lib_platform/master?filepath=lib_platform.ipynb
-        
-        .. for the pypi status link note the dashes, not the underscore !
-        .. |pypi| image:: https://img.shields.io/pypi/status/lib-platform?label=PyPI%20Package
-           :target: https://badge.fury.io/py/lib_platform
-        
-        .. |codecov| image:: https://img.shields.io/codecov/c/github/bitranox/lib_platform
-           :target: https://codecov.io/gh/bitranox/lib_platform
-        
-        .. |better_code| image:: https://bettercodehub.com/edge/badge/bitranox/lib_platform?branch=master
-           :target: https://bettercodehub.com/results/bitranox/lib_platform
-        
-        .. |cc_maintain| image:: https://img.shields.io/codeclimate/maintainability-percentage/bitranox/lib_platform?label=CC%20maintainability
-           :target: https://codeclimate.com/github/bitranox/lib_platform/maintainability
-           :alt: Maintainability
-        
-        .. |cc_issues| image:: https://img.shields.io/codeclimate/issues/bitranox/lib_platform?label=CC%20issues
-           :target: https://codeclimate.com/github/bitranox/lib_platform/maintainability
-           :alt: Maintainability
-        
-        .. |cc_coverage| image:: https://img.shields.io/codeclimate/coverage/bitranox/lib_platform?label=CC%20coverage
-           :target: https://codeclimate.com/github/bitranox/lib_platform/test_coverage
-           :alt: Code Coverage
-        
-        .. |snyk| image:: https://img.shields.io/snyk/vulnerabilities/github/bitranox/lib_platform
-           :target: https://snyk.io/test/github/bitranox/lib_platform
-        
-        .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
-           :target: https://github.com/psf/black
-        
-        some platform related functions, which also work correctly on wine
-        
-        ----
-        
-        automated tests, Travis Matrix, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
-        .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
-        
-        Python version required: 3.6.0 or newer
-        
-        tested on linux "bionic" with python 3.6, 3.7, 3.8, 3.9-dev, pypy3 - architectures: amd64, ppc64le, s390x, arm64
-        
-        `100% code coverage <https://codecov.io/gh/bitranox/lib_platform>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://travis-ci.org/bitranox/lib_platform>`_, automatic daily builds and monitoring
-        
-        ----
-        
-        - `Try it Online`_
-        - `Usage`_
-        - `Usage from Commandline`_
-        - `Installation and Upgrade`_
-        - `Requirements`_
-        - `Acknowledgements`_
-        - `Contribute`_
-        - `Report Issues <https://github.com/bitranox/lib_platform/blob/master/ISSUE_TEMPLATE.md>`_
-        - `Pull Request <https://github.com/bitranox/lib_platform/blob/master/PULL_REQUEST_TEMPLATE.md>`_
-        - `Code of Conduct <https://github.com/bitranox/lib_platform/blob/master/CODE_OF_CONDUCT.md>`_
-        - `License`_
-        - `Changelog`_
-        
-        ----
-        
-        Try it Online
-        -------------
-        
-        You might try it right away in Jupyter Notebook by using the "launch binder" badge, or click `here <https://mybinder.org/v2/gh/{{rst_include.
-        repository_slug}}/master?filepath=lib_platform.ipynb>`_
-        
-        Usage
-        -----------
-        
-        .. code-block:: python
-        
-            >>> import lib_platform
-        
-            >>> # get system as string
-            >>> system = lib_platform.system
-        
-            >>> # bool is_platform_linux
-            >>> is_platform_linux = lib_platform.is_platform_linux
-        
-            >>> # bool is_platform_darwin
-            >>> is_platform_darwin = lib_platform.is_platform_darwin
-        
-            >>> # bool is_platform_posix
-            >>> # either darwin or linux
-            >>> is_platform_posix = lib_platform.is_platform_posix
-        
-            >>> # bool is_platform_windows
-            >>> # also True for windows_xp or windows_wine
-            >>> is_platform_windows = lib_platform.is_platform_windows
-        
-            >>> # bool is_platform_windows_xp
-            >>> is_platform_windows_xp = lib_platform.is_platform_windows_xp
-        
-            >>> # bool is_platform_windows_wine
-            >>> is_platform_windows_wine = lib_platform.is_platform_windows_wine
-        
-            >>> # bool is_platform_windows_wine_xp
-            >>> is_platform_windows_wine_xp = lib_platform.is_platform_windows_wine_xp
-        
-            >>> # string username lib_platform.username
-            >>> username = lib_platform.username
-        
-            >>> # string fqdn hostname
-            >>> hostname = lib_platform.hostname
-        
-            >>> # string hostname short
-            >>> hostname_short = lib_platform.hostname_short
-        
-            >>> # path to userhome
-            >>> path_userhome = lib_platform.path_userhome
-        
-            >>> # is user administrator (has user admin rights)
-            >>> is_user_admin = lib_platform.is_user_admin
-        
-        Usage from Commandline
-        ------------------------
-        
-        .. code-block:: bash
-        
-           Usage: lib_platform [OPTIONS] COMMAND [ARGS]...
-        
-             some platform related functions, which also work correctly on wine
-        
-           Options:
-             --version                     Show the version and exit.
-             --traceback / --no-traceback  return traceback information on cli
-             -h, --help                    Show this message and exit.
-        
-           Commands:
-             info  get program informations
-        
-        Installation and Upgrade
-        ------------------------
-        
-        - Before You start, its highly recommended to update pip and setup tools:
-        
-        
-        .. code-block:: bash
-        
-            python -m pip --upgrade pip
-            python -m pip --upgrade setuptools
-        
-        - to install the latest release from PyPi via pip (recommended):
-        
-        .. code-block:: bash
-        
-            python -m pip install --upgrade lib_platform
-        
-        - to install the latest version from github via pip:
-        
-        
-        .. code-block:: bash
-        
-            python -m pip install --upgrade git+https://github.com/bitranox/lib_platform.git
-        
-        
-        - include it into Your requirements.txt:
-        
-        .. code-block:: bash
-        
-            # Insert following line in Your requirements.txt:
-            # for the latest Release on pypi:
-            lib_platform
-        
-            # for the latest development version :
-            lib_platform @ git+https://github.com/bitranox/lib_platform.git
-        
-            # to install and upgrade all modules mentioned in requirements.txt:
-            python -m pip install --upgrade -r /<path>/requirements.txt
-        
-        
-        - to install the latest development version from source code:
-        
-        .. code-block:: bash
-        
-            # cd ~
-            $ git clone https://github.com/bitranox/lib_platform.git
-            $ cd lib_platform
-            python setup.py install
-        
-        - via makefile:
-          makefiles are a very convenient way to install. Here we can do much more,
-          like installing virtual environments, clean caches and so on.
-        
-        .. code-block:: shell
-        
-            # from Your shell's homedirectory:
-            $ git clone https://github.com/bitranox/lib_platform.git
-            $ cd lib_platform
-        
-            # to run the tests:
-            $ make test
-        
-            # to install the package
-            $ make install
-        
-            # to clean the package
-            $ make clean
-        
-            # uninstall the package
-            $ make uninstall
-        
-        Requirements
-        ------------
-        following modules will be automatically installed :
-        
-        .. code-block:: bash
-        
-            ## Project Requirements
-            click
-            cli_exit_tools @ git+https://github.com/bitranox/cli_exit_tools.git
-            lib_registry @ git+https://github.com/bitranox/lib_registry.git
-        
-        Acknowledgements
-        ----------------
-        
-        - special thanks to "uncle bob" Robert C. Martin, especially for his books on "clean code" and "clean architecture"
-        
-        Contribute
-        ----------
-        
-        I would love for you to fork and send me pull request for this project.
-        - `please Contribute <https://github.com/bitranox/lib_platform/blob/master/CONTRIBUTING.md>`_
-        
-        License
-        -------
-        
-        This software is licensed under the `MIT license <http://en.wikipedia.org/wiki/MIT_License>`_
-        
-        ---
-        
-        Changelog
-        =========
-        
-        - new MAJOR version for incompatible API changes,
-        - new MINOR version for added functionality in a backwards compatible manner
-        - new PATCH version for backwards compatible bug fixes
-        
-        v1.2.7
-        --------
-        2020-10-09: service release
-            - update travis build matrix for linux 3.9-dev
-            - update travis build matrix (paths) for windows 3.9 / 3.10
-        
-        v1.2.6
-        --------
-        2020-08-08: service release
-            - fix documentation
-            - fix travis
-            - deprecate pycodestyle
-            - implement flake8
-        
-        v1.2.5
-        ---------
-        2020-08-01: fix pypi deploy
-        
-        v1.2.4
-        --------
-        2020-07-31: fix travis build
-        
-        v1.2.3
-        --------
-        2020-07-29: feature release
-            - use the new pizzacutter template
-            - use cli_exit_tools
-        
-        v1.2.2
-        --------
-        2020-07-16: feature release
-            - fix cli test
-            - enable traceback option on cli errors
-        
-        v1.2.1
-        --------
-        2020-07-14 : patch release
-            - make it compatible with latest lib_registry
-        
-        
-        v1.2.0
-        --------
-        2020-07-07 : service release
-            - new click cli
-            - use PizzaCutter Template
-            - added jupyter notebook
-            - dropped python2.7 - python3.5 support
-        
-        v1.0.3
-        --------
-        2019-06-14: add is_user_admin (check for administration rights)
-        
-        v1.0.2
-        --------
-        2019-04-28: Documentation Update, minor Fixes in setup.py
-        
-        v1.0.0
-        --------
-        2019-03-28: Initial public release, PyPi Release
-        
-        
-Platform: UNKNOWN
+Author-email: Robert Nowotny <bitranox@gmail.com>
+License: MIT
+Project-URL: Homepage, https://github.com/bitranox/lib_platform
+Project-URL: Documentation, https://github.com/bitranox/lib_platform/blob/master/README.rst
+Project-URL: Repository, https://github.com/bitranox/lib_platform.git
+Project-URL: Changelog, https://github.com/bitranox/lib_platform/blob/master/CHANGES.rst
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
+License-File: LICENSE
+
+lib_platform
+============
+
+
+Version v1.2.9 as of 2023-07-21 see `Changelog`_
+
+|build_badge| |codeql| |license| |jupyter| |pypi|
+|pypi-downloads| |black| |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+
+
+
+.. |build_badge| image:: https://github.com/bitranox/lib_platform/actions/workflows/python-package.yml/badge.svg
+   :target: https://github.com/bitranox/lib_platform/actions/workflows/python-package.yml
+
+
+.. |codeql| image:: https://github.com/bitranox/lib_platform/actions/workflows/codeql-analysis.yml/badge.svg?event=push
+   :target: https://github.com//bitranox/lib_platform/actions/workflows/codeql-analysis.yml
+
+.. |license| image:: https://img.shields.io/github/license/webcomics/pywine.svg
+   :target: http://en.wikipedia.org/wiki/MIT_License
+
+.. |jupyter| image:: https://mybinder.org/badge_logo.svg
+   :target: https://mybinder.org/v2/gh/bitranox/lib_platform/master?filepath=lib_platform.ipynb
+
+.. for the pypi status link note the dashes, not the underscore !
+.. |pypi| image:: https://img.shields.io/pypi/status/lib-platform?label=PyPI%20Package
+   :target: https://badge.fury.io/py/lib_platform
+
+.. |codecov| image:: https://img.shields.io/codecov/c/github/bitranox/lib_platform
+   :target: https://codecov.io/gh/bitranox/lib_platform
+
+.. |cc_maintain| image:: https://img.shields.io/codeclimate/maintainability-percentage/bitranox/lib_platform?label=CC%20maintainability
+   :target: https://codeclimate.com/github/bitranox/lib_platform/maintainability
+   :alt: Maintainability
+
+.. |cc_issues| image:: https://img.shields.io/codeclimate/issues/bitranox/lib_platform?label=CC%20issues
+   :target: https://codeclimate.com/github/bitranox/lib_platform/maintainability
+   :alt: Maintainability
+
+.. |cc_coverage| image:: https://img.shields.io/codeclimate/coverage/bitranox/lib_platform?label=CC%20coverage
+   :target: https://codeclimate.com/github/bitranox/lib_platform/test_coverage
+   :alt: Code Coverage
+
+.. |snyk| image:: https://snyk.io/test/github/bitranox/lib_platform/badge.svg
+   :target: https://snyk.io/test/github/bitranox/lib_platform
+
+.. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
+   :target: https://github.com/psf/black
+
+.. |pypi-downloads| image:: https://img.shields.io/pypi/dm/lib-platform
+   :target: https://pypi.org/project/lib-platform/
+   :alt: PyPI - Downloads
+
+some platform related functions, which also work correctly on wine
+
+----
+
+automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
+.com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
+
+Python version required: 3.8.0 or newer
+
+tested on recent linux with python 3.8, 3.9, 3.10, 3.11, 3.12-dev, pypy-3.9, pypy-3.10 - architectures: amd64
+
+`100% code coverage <https://codeclimate.com/github/bitranox/lib_platform/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/lib_platform/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
+
+----
+
+- `Try it Online`_
+- `Usage`_
+- `Usage from Commandline`_
+- `Installation and Upgrade`_
+- `Requirements`_
+- `Acknowledgements`_
+- `Contribute`_
+- `Report Issues <https://github.com/bitranox/lib_platform/blob/master/ISSUE_TEMPLATE.md>`_
+- `Pull Request <https://github.com/bitranox/lib_platform/blob/master/PULL_REQUEST_TEMPLATE.md>`_
+- `Code of Conduct <https://github.com/bitranox/lib_platform/blob/master/CODE_OF_CONDUCT.md>`_
+- `License`_
+- `Changelog`_
+
+----
+
+Try it Online
+-------------
+
+You might try it right away in Jupyter Notebook by using the "launch binder" badge, or click `here <https://mybinder.org/v2/gh/{{rst_include.
+repository_slug}}/master?filepath=lib_platform.ipynb>`_
+
+Usage
+-----------
+
+.. code-block:: python
+
+    >>> import lib_platform
+
+    >>> # get system as string
+    >>> system = lib_platform.system
+
+    >>> # bool is_platform_linux
+    >>> is_platform_linux = lib_platform.is_platform_linux
+
+    >>> # bool is_platform_darwin
+    >>> is_platform_darwin = lib_platform.is_platform_darwin
+
+    >>> # bool is_platform_posix
+    >>> # either darwin or linux
+    >>> is_platform_posix = lib_platform.is_platform_posix
+
+    >>> # bool is_platform_windows
+    >>> # also True for windows_xp or windows_wine
+    >>> is_platform_windows = lib_platform.is_platform_windows
+
+    >>> # bool is_platform_windows_xp
+    >>> is_platform_windows_xp = lib_platform.is_platform_windows_xp
+
+    >>> # bool is_platform_windows_wine
+    >>> is_platform_windows_wine = lib_platform.is_platform_windows_wine
+
+    >>> # bool is_platform_windows_wine_xp
+    >>> is_platform_windows_wine_xp = lib_platform.is_platform_windows_wine_xp
+
+    >>> # string username lib_platform.username
+    >>> username = lib_platform.username
+
+    >>> # string fqdn hostname
+    >>> hostname = lib_platform.hostname
+
+    >>> # string hostname short
+    >>> hostname_short = lib_platform.hostname_short
+
+    >>> # path to userhome
+    >>> path_userhome = lib_platform.path_userhome
+
+    >>> # is user administrator (has user admin rights)
+    >>> is_user_admin = lib_platform.is_user_admin
+
+Usage from Commandline
+------------------------
+
+.. code-block::
+
+   Usage: lib_platform [OPTIONS] COMMAND [ARGS]...
+
+     some platform related functions, which also work correctly on wine
+
+   Options:
+     --version                     Show the version and exit.
+     --traceback / --no-traceback  return traceback information on cli
+     -h, --help                    Show this message and exit.
+
+   Commands:
+     info  get program informations
+
+Installation and Upgrade
+------------------------
+
+- Before You start, its highly recommended to update pip and setup tools:
+
+
+.. code-block::
+
+    python -m pip --upgrade pip
+    python -m pip --upgrade setuptools
+
+- to install the latest release from PyPi via pip (recommended):
+
+.. code-block::
+
+    python -m pip install --upgrade lib_platform
+
+
+- to install the latest release from PyPi via pip, including test dependencies:
+
+.. code-block::
+
+    python -m pip install --upgrade lib_platform[test]
+
+- to install the latest version from github via pip:
+
+
+.. code-block::
+
+    python -m pip install --upgrade git+https://github.com/bitranox/lib_platform.git
+
+
+- include it into Your requirements.txt:
+
+.. code-block::
+
+    # Insert following line in Your requirements.txt:
+    # for the latest Release on pypi:
+    lib_platform
+
+    # for the latest development version :
+    lib_platform @ git+https://github.com/bitranox/lib_platform.git
+
+    # to install and upgrade all modules mentioned in requirements.txt:
+    python -m pip install --upgrade -r /<path>/requirements.txt
+
+
+- to install the latest development version, including test dependencies from source code:
+
+.. code-block::
+
+    # cd ~
+    $ git clone https://github.com/bitranox/lib_platform.git
+    $ cd lib_platform
+    python -m pip install -e .[test]
+
+- via makefile:
+  makefiles are a very convenient way to install. Here we can do much more,
+  like installing virtual environments, clean caches and so on.
+
+.. code-block:: shell
+
+    # from Your shell's homedirectory:
+    $ git clone https://github.com/bitranox/lib_platform.git
+    $ cd lib_platform
+
+    # to run the tests:
+    $ make test
+
+    # to install the package
+    $ make install
+
+    # to clean the package
+    $ make clean
+
+    # uninstall the package
+    $ make uninstall
+
+Requirements
+------------
+following modules will be automatically installed :
+
+.. code-block:: bash
+
+    ## Project Requirements
+    click
+    cli_exit_tools
+    lib_registry
+
+Acknowledgements
+----------------
+
+- special thanks to "uncle bob" Robert C. Martin, especially for his books on "clean code" and "clean architecture"
+
+Contribute
+----------
+
+I would love for you to fork and send me pull request for this project.
+- `please Contribute <https://github.com/bitranox/lib_platform/blob/master/CONTRIBUTING.md>`_
+
+License
+-------
+
+This software is licensed under the `MIT license <http://en.wikipedia.org/wiki/MIT_License>`_
+
+---
+
+Changelog
+=========
+
+- new MAJOR version for incompatible API changes,
+- new MINOR version for added functionality in a backwards compatible manner
+- new PATCH version for backwards compatible bug fixes
+
+v1.2.9
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
+v1.2.8
+--------
+2022-11-09:
+    - fix get hostname, if something is tinkering with the loopback interface on Windows - for instance 'Solid Works 3DExperience'
+
+v1.2.7
+--------
+2020-10-09: service release
+    - update travis build matrix for linux 3.9-dev
+    - update travis build matrix (paths) for windows 3.9 / 3.10
+
+v1.2.6
+--------
+2020-08-08: service release
+    - fix documentation
+    - fix travis
+    - deprecate pycodestyle
+    - implement flake8
+
+v1.2.5
+---------
+2020-08-01: fix pypi deploy
+
+v1.2.4
+--------
+2020-07-31: fix travis build
+
+v1.2.3
+--------
+2020-07-29: feature release
+    - use the new pizzacutter template
+    - use cli_exit_tools
+
+v1.2.2
+--------
+2020-07-16: feature release
+    - fix cli test
+    - enable traceback option on cli errors
+
+v1.2.1
+--------
+2020-07-14 : patch release
+    - make it compatible with latest lib_registry
+
+
+v1.2.0
+--------
+2020-07-07 : service release
+    - new click cli
+    - use PizzaCutter Template
+    - added jupyter notebook
+    - dropped python2.7 - python3.5 support
+
+v1.0.3
+--------
+2019-06-14: add is_user_admin (check for administration rights)
+
+v1.0.2
+--------
+2019-04-28: Documentation Update, minor Fixes in setup.py
+
+v1.0.0
+--------
+2019-03-28: Initial public release, PyPi Release
+
```

### Comparing `lib_platform-1.2.7/lib_platform/lib_platform_cli.py` & `lib_platform-1.2.9/lib_platform/lib_platform_cli.py`

 * *Files 10% similar despite different names*

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
 
 
 @cli_main.command('info', context_settings=CLICK_CONTEXT_SETTINGS)
@@ -45,13 +45,13 @@
     """ get program informations """
     info()
 
 
 # entry point if main
 if __name__ == '__main__':
     try:
-        cli_main()
+        cli_main()                  # type: ignore
     except Exception as exc:
         cli_exit_tools.print_exception_message()
         sys.exit(cli_exit_tools.get_system_exit_code(exc))
     finally:
         cli_exit_tools.flush_streams()
```

### Comparing `lib_platform-1.2.7/lib_platform/lib_platform.py` & `lib_platform-1.2.9/lib_platform/lib_platform.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,46 +13,61 @@
 
 def get_hostname() -> str:
     """
     Returns fqdn hostname lowercase, also for WINE
 
     >>> result = get_hostname()
     >>> assert len(result) > 1
-
     """
 
-    if get_is_platform_windows_wine():  # for wine get hostname not via IP Adress - would give name of the host
+    if get_is_platform_windows_wine():  # for wine get hostname not via IP Adress - that would give name of the linux host
         # noinspection PyBroadException
         try:
             result_wine_reg = lib_registry.Registry().get_value(key=r'HKLM\System\CurrentControlSet\Control\ComputerName', value_name='ComputerName')
             assert isinstance(result_wine_reg, str)
             _hostname = result_wine_reg
         except Exception:
             result_wine_env = os.getenv('COMPUTERNAME')  # max 15 Zeichen
             if result_wine_env is None:
                 raise RuntimeError('can not determine Username on Wine')
             else:
                 _hostname = result_wine_env
 
     elif get_is_platform_windows():
-        _hostname = socket.getfqdn()
+        _hostname = _get_fqdn_by_hostname()
     else:
         # this one failed on the first call sometimes - use now getfqdn() supports both IPv4 and IPv6. - and sometimes give WRONG HOSTNAME
         # _hostname = socket.gethostbyaddr(socket.gethostname())[0]
 
         # sometimes gives WRONG HOSTNAME on a bridge after reboot - WEIRD !
         # _hostname = socket.getfqdn()
 
         # this always works
         _hostname = subprocess.getoutput('uname -n')
 
     _hostname = str(_hostname.lower())
     return str(_hostname)
 
 
+def _get_fqdn_by_hostname() -> str:
+    """
+    Returns fqdn by hostname
+    if You use just socket.getfqdn(), it will return 'dslauncher.3ds.com' if Solid Works 3DExperience is installed.
+    this is because they tinker with the loopback address
+    therefore we get hostname --> ip adress --> fqdn
+
+    >>> assert _get_fqdn_by_hostname()
+
+    """
+    _hostname_short = socket.gethostname()
+    _ip_address = socket.gethostbyname(_hostname_short)
+    _fqdn = socket.getfqdn(name=_ip_address)
+    return _fqdn
+
+
 def get_hostname_short() -> str:
     """
     Returns hostname lowercase without domain part
 
     >>> result = get_hostname_short()
     >>> assert len(result) > 1
```

### Comparing `lib_platform-1.2.7/lib_platform/__init__conf__.py` & `lib_platform-1.2.9/lib_platform/__init__conf__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,22 @@
+# CONF
+
 name = 'lib_platform'
 title = 'some platform related functions, which also work correctly on wine'
-version = 'v1.2.7'
+version = 'v1.2.9'
 url = 'https://github.com/bitranox/lib_platform'
 author = 'Robert Nowotny'
 author_email = 'bitranox@gmail.com'
 shell_command = 'lib_platform'
 
 
 def print_info() -> None:
     print("""\
 
 Info for lib_platform:
 
     some platform related functions, which also work correctly on wine
 
-    Version : v1.2.7
+    Version : v1.2.9
     Url     : https://github.com/bitranox/lib_platform
     Author  : Robert Nowotny
     Email   : bitranox@gmail.com""")
```

