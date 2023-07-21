# Comparing `tmp/pyopal-0.3.0.tar.gz` & `tmp/pyopal-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyopal-0.3.0.tar", last modified: Tue May 30 12:36:00 2023, max compression
+gzip compressed data, was "pyopal-0.4.0.tar", last modified: Fri Jul 21 16:53:52 2023, max compression
```

## Comparing `pyopal-0.3.0.tar` & `pyopal-0.4.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:36:00.510659 pyopal-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-30 12:35:44.000000 pyopal-0.3.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-05-30 12:35:44.000000 pyopal-0.3.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-30 12:35:44.000000 pyopal-0.3.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-30 12:35:44.000000 pyopal-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10168 2023-05-30 12:36:00.510659 pyopal-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-05-30 12:35:44.000000 pyopal-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:36:00.506659 pyopal-0.3.0/include/
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-30 12:35:44.000000 pyopal-0.3.0/include/_unicode.pxd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:36:00.510659 pyopal-0.3.0/include/cpu_features/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 12:35:44.000000 pyopal-0.3.0/include/cpu_features/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-30 12:35:44.000000 pyopal-0.3.0/include/cpu_features/aarch64.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-30 12:35:44.000000 pyopal-0.3.0/include/cpu_features/arm.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-30 12:35:44.000000 pyopal-0.3.0/include/cpu_features/x86.pxd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:36:00.510659 pyopal-0.3.0/include/opal/
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-05-30 12:35:44.000000 pyopal-0.3.0/include/opal/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-30 12:35:44.000000 pyopal-0.3.0/include/opal/score_matrix.pxd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:36:00.510659 pyopal-0.3.0/pyopal/
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-30 12:35:44.000000 pyopal-0.3.0/pyopal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-05-30 12:35:44.000000 pyopal-0.3.0/pyopal/_opal.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    39490 2023-05-30 12:35:44.000000 pyopal-0.3.0/pyopal/_opal.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-30 12:35:44.000000 pyopal-0.3.0/pyopal/_opal_avx2.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-30 12:35:44.000000 pyopal-0.3.0/pyopal/_opal_avx2.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-30 12:35:44.000000 pyopal-0.3.0/pyopal/_opal_neon.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-30 12:35:44.000000 pyopal-0.3.0/pyopal/_opal_neon.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-30 12:35:44.000000 pyopal-0.3.0/pyopal/_opal_sse2.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-30 12:35:44.000000 pyopal-0.3.0/pyopal/_opal_sse2.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-30 12:35:44.000000 pyopal-0.3.0/pyopal/_opal_sse4.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-30 12:35:44.000000 pyopal-0.3.0/pyopal/_opal_sse4.pyx
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-30 12:35:44.000000 pyopal-0.3.0/pyopal/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 12:35:44.000000 pyopal-0.3.0/pyopal/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:36:00.510659 pyopal-0.3.0/pyopal/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-30 12:35:44.000000 pyopal-0.3.0/pyopal/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-05-30 12:35:44.000000 pyopal-0.3.0/pyopal/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-05-30 12:35:44.000000 pyopal-0.3.0/pyopal/tests/test_doctest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-05-30 12:35:44.000000 pyopal-0.3.0/pyopal/tests/test_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:36:00.510659 pyopal-0.3.0/pyopal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10168 2023-05-30 12:36:00.000000 pyopal-0.3.0/pyopal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-30 12:36:00.000000 pyopal-0.3.0/pyopal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 12:36:00.000000 pyopal-0.3.0/pyopal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 12:36:00.000000 pyopal-0.3.0/pyopal.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-30 12:36:00.000000 pyopal-0.3.0/pyopal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-30 12:36:00.000000 pyopal-0.3.0/pyopal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-30 12:36:00.000000 pyopal-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-05-30 12:36:00.510659 pyopal-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    18986 2023-05-30 12:35:44.000000 pyopal-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:36:00.506659 pyopal-0.3.0/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:36:00.510659 pyopal-0.3.0/vendor/opal/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-30 12:35:45.000000 pyopal-0.3.0/vendor/opal/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-05-30 12:35:45.000000 pyopal-0.3.0/vendor/opal/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:36:00.510659 pyopal-0.3.0/vendor/opal/src/
--rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-05-30 12:35:45.000000 pyopal-0.3.0/vendor/opal/src/ScoreMatrix.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-30 12:35:45.000000 pyopal-0.3.0/vendor/opal/src/ScoreMatrix.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    86020 2023-05-30 12:35:45.000000 pyopal-0.3.0/vendor/opal/src/opal.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8325 2023-05-30 12:35:45.000000 pyopal-0.3.0/vendor/opal/src/opal.h
--rw-r--r--   0 runner    (1001) docker     (123)    13260 2023-05-30 12:35:45.000000 pyopal-0.3.0/vendor/opal/src/opal_aligner.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    15339 2023-05-30 12:35:45.000000 pyopal-0.3.0/vendor/opal/src/test.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:53:52.612262 pyopal-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-21 16:53:41.000000 pyopal-0.4.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-21 16:53:41.000000 pyopal-0.4.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-21 16:53:41.000000 pyopal-0.4.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-21 16:53:41.000000 pyopal-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-07-21 16:53:52.612262 pyopal-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8149 2023-07-21 16:53:41.000000 pyopal-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:53:52.608262 pyopal-0.4.0/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:53:52.608262 pyopal-0.4.0/include/cpu_features/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:53:41.000000 pyopal-0.4.0/include/cpu_features/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-21 16:53:41.000000 pyopal-0.4.0/include/cpu_features/aarch64.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-21 16:53:41.000000 pyopal-0.4.0/include/cpu_features/arm.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-21 16:53:41.000000 pyopal-0.4.0/include/cpu_features/x86.pxd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:53:52.608262 pyopal-0.4.0/include/opal/
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-07-21 16:53:41.000000 pyopal-0.4.0/include/opal/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-21 16:53:41.000000 pyopal-0.4.0/include/opal/score_matrix.pxd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:53:52.608262 pyopal-0.4.0/pyopal/
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-21 16:53:41.000000 pyopal-0.4.0/pyopal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-07-21 16:53:41.000000 pyopal-0.4.0/pyopal/_opal.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    39193 2023-07-21 16:53:41.000000 pyopal-0.4.0/pyopal/_opal.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-21 16:53:41.000000 pyopal-0.4.0/pyopal/_opal_avx2.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-21 16:53:41.000000 pyopal-0.4.0/pyopal/_opal_avx2.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-21 16:53:41.000000 pyopal-0.4.0/pyopal/_opal_neon.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-21 16:53:41.000000 pyopal-0.4.0/pyopal/_opal_neon.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-21 16:53:41.000000 pyopal-0.4.0/pyopal/_opal_sse2.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-21 16:53:41.000000 pyopal-0.4.0/pyopal/_opal_sse2.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-21 16:53:41.000000 pyopal-0.4.0/pyopal/_opal_sse4.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-21 16:53:41.000000 pyopal-0.4.0/pyopal/_opal_sse4.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-21 16:53:41.000000 pyopal-0.4.0/pyopal/_patch.pxi
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-21 16:53:41.000000 pyopal-0.4.0/pyopal/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:53:41.000000 pyopal-0.4.0/pyopal/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:53:52.612262 pyopal-0.4.0/pyopal/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-21 16:53:41.000000 pyopal-0.4.0/pyopal/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-07-21 16:53:41.000000 pyopal-0.4.0/pyopal/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-21 16:53:41.000000 pyopal-0.4.0/pyopal/tests/test_doctest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-07-21 16:53:41.000000 pyopal-0.4.0/pyopal/tests/test_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:53:52.608262 pyopal-0.4.0/pyopal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-07-21 16:53:52.000000 pyopal-0.4.0/pyopal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-21 16:53:52.000000 pyopal-0.4.0/pyopal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 16:53:52.000000 pyopal-0.4.0/pyopal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 16:53:52.000000 pyopal-0.4.0/pyopal.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-21 16:53:52.000000 pyopal-0.4.0/pyopal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-21 16:53:52.000000 pyopal-0.4.0/pyopal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-21 16:53:52.000000 pyopal-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-07-21 16:53:52.612262 pyopal-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    20296 2023-07-21 16:53:41.000000 pyopal-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:53:52.608262 pyopal-0.4.0/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:53:52.612262 pyopal-0.4.0/vendor/opal/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-21 16:53:42.000000 pyopal-0.4.0/vendor/opal/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-07-21 16:53:42.000000 pyopal-0.4.0/vendor/opal/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:53:52.612262 pyopal-0.4.0/vendor/opal/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-07-21 16:53:42.000000 pyopal-0.4.0/vendor/opal/src/ScoreMatrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-21 16:53:42.000000 pyopal-0.4.0/vendor/opal/src/ScoreMatrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    86020 2023-07-21 16:53:42.000000 pyopal-0.4.0/vendor/opal/src/opal.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8325 2023-07-21 16:53:42.000000 pyopal-0.4.0/vendor/opal/src/opal.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13260 2023-07-21 16:53:42.000000 pyopal-0.4.0/vendor/opal/src/opal_aligner.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15339 2023-07-21 16:53:42.000000 pyopal-0.4.0/vendor/opal/src/test.cpp
```

### Comparing `pyopal-0.3.0/CHANGELOG.md` & `pyopal-0.4.0/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,25 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 
 ## [Unreleased]
-[Unreleased]: https://github.com/althonos/pyopal/compare/v0.3.0...HEAD
+[Unreleased]: https://github.com/althonos/pyopal/compare/v0.4.0...HEAD
+
+
+## [v0.4.0] - 2023-07-21
+[v0.4.0]: https://github.com/althonos/pyopal/compare/v0.3.0...v0.4.0
+
+### Changed
+- Bumped Cython dependency to `v3.0`.
+
+### Fixed
+- PyPy 3.9 builds failing on missing `PyInterpreterState_GetID`.
 
 
 ## [v0.3.0] - 2023-05-30
 [v0.3.0]: https://github.com/althonos/pyopal/compare/v0.2.0...v0.3.0
 
 ### Added
 - `Database.extract` method to subset a database given a sequence of indices.
```

### Comparing `pyopal-0.3.0/CONTRIBUTING.md` & `pyopal-0.4.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyopal-0.3.0/COPYING` & `pyopal-0.4.0/COPYING`

 * *Files identical despite different names*

### Comparing `pyopal-0.3.0/PKG-INFO` & `pyopal-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyopal
-Version: 0.3.0
+Version: 0.4.0
 Summary: Cython bindings and Python interface to Opal, a SIMD-accelerated pairwise aligner.
 Home-page: https://github.com/althonos/pyopal
 Author: Martin Larralde
 Author-email: martin.larralde@embl.de
 License: MIT
 Project-URL: Documentation, https://pyopal.readthedocs.io/en/stable/
 Project-URL: Bug Tracker, https://github.com/althonos/pyopal/issues
@@ -50,31 +50,31 @@
 [![Python Versions](https://img.shields.io/pypi/pyversions/pyopal.svg?style=flat-square&maxAge=600&logo=python)](https://pypi.org/project/pyopal/#files)
 [![Python Implementations](https://img.shields.io/pypi/implementation/pyopal.svg?style=flat-square&maxAge=600&label=impl)](https://pypi.org/project/pyopal/#files)
 [![Source](https://img.shields.io/badge/source-GitHub-303030.svg?maxAge=2678400&style=flat-square)](https://github.com/althonos/pyopal/)
 [![Mirror](https://img.shields.io/badge/mirror-EMBL-009f4d?style=flat-square&maxAge=2678400)](https://git.embl.de/larralde/pyopal/)
 [![Issues](https://img.shields.io/github/issues/althonos/pyopal.svg?style=flat-square&maxAge=600)](https://github.com/althonos/pyopal/issues)
 [![Docs](https://img.shields.io/readthedocs/pyopal/latest?style=flat-square&maxAge=600)](https://pyopal.readthedocs.io)
 [![Changelog](https://img.shields.io/badge/keep%20a-changelog-8A0707.svg?maxAge=2678400&style=flat-square)](https://github.com/althonos/pyopal/blob/main/CHANGELOG.md)
-[![Downloads](https://img.shields.io/badge/dynamic/json?style=flat-square&color=303f9f&maxAge=86400&label=downloads&query=%24.total_downloads&url=https%3A%2F%2Fapi.pepy.tech%2Fapi%2Fprojects%2Fpyopal)](https://pepy.tech/project/pyopal)
+[![Downloads](https://img.shields.io/pypi/dm/pyopal?style=flat-square&color=303f9f&maxAge=86400&label=downloads)](https://pepy.tech/project/pyopal)
 
 
 ## 🗺️ Overview
 
 [Opal](https://github.com/Martinsos/opal) is a sequence aligner enabling fast
 sequence similarity search using either of the Smith-Waterman, semi-global or
 Needleman-Wunsch algorithms.
 
 PyOpal is a Python module that provides bindings to [Opal](https://github.com/Martinsos/opal)
 using [Cython](https://cython.org/). It implements a user-friendly, Pythonic
 interface to query a database of sequences and access the search results. It
 interacts with the Opal interface rather than with the CLI, which has the
 following advantages:
 
-- **single dependency**: PyOpal is distributed as a Python package, so you
-  can add it as a dependency to your project, and stop worrying about the
+- **no binary dependency**: PyOpal is distributed as a Python package, so 
+  you can add it as a dependency to your project, and stop worrying about the
   Opal binary being present on the end-user machine.
 - **no intermediate files**: Everything happens in memory, in a Python object
   you control, so you don't have to invoke the Opal CLI using a sub-process
   and temporary files.
 - **better portability**: Opal uses SIMD to accelerate alignment scoring, but
   doesn't support dynamic dispatch, so it has to be compiled on the local
   machine to be able to use the full capabilities of the local CPU. PyOpal
@@ -83,20 +83,21 @@
 - **wider platform support**: The Opal code has been backported to work on SSE2
   rather than SSE4.1, allowing PyOpal to run on older x86 CPUs (all x86 CPUs
   support it since 2003). In addition, Armv7 and Aarch64 CPUs are also
   supported if they implement NEON extensions.
 
 ## 🔧 Installing
 
-PyOpal is available for all modern versions (3.6+), with no external dependencies.
+PyOpal is available for all modern versions (3.6+), depending only 
+on the lightweight Python package [`archspec`](https://pypi.org/project/archspec) 
+for runtime CPU feature detection.
 
 It can be installed directly from [PyPI](https://pypi.org/project/pyopal/),
-which hosts some pre-built wheels for the x86-64 architecture (Linux/OSX)
-and the Aarch64 architecture (Linux only), as well as the code required to compile
-from source with Cython:
+which hosts some pre-built x86-64 and Aarch64 wheels for Linux and MacOS,
+as well as the code required to compile from source with Cython:
 ```console
 $ pip install pyopal
 ```
 
 <!-- Otherwise, PyOpal is also available as a [Bioconda](https://bioconda.github.io/)
 package:
 ```console
@@ -191,16 +192,13 @@
 
 
 ## ⚖️ License
 
 This library is provided under the [MIT License](https://choosealicense.com/licenses/mit/).
 Opal is developed by [Martin Šošić](https://github.com/Martinsos) and is distributed under the
 terms of the MIT License as well. See `vendor/opal/LICENSE` for more information.
-The `cpu_features` library was written by [Guillaume Chatelet](https://github.com/gchatelet) and is
-licensed under the terms of the [Apache License 2.0](https://choosealicense.com/licenses/apache-2.0/).
-See `vendor/cpu_features/LICENSE` for more information.
 
 *This project is in no way not affiliated, sponsored, or otherwise endorsed
 by the [Opal authors](https://github.com/Martinsos). It was developed
 by [Martin Larralde](https://github.com/althonos/) during his PhD project
 at the [European Molecular Biology Laboratory](https://www.embl.de/) in
 the [Zeller team](https://github.com/zellerlab).*
```

### Comparing `pyopal-0.3.0/README.md` & `pyopal-0.4.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -12,31 +12,31 @@
 [![Python Versions](https://img.shields.io/pypi/pyversions/pyopal.svg?style=flat-square&maxAge=600&logo=python)](https://pypi.org/project/pyopal/#files)
 [![Python Implementations](https://img.shields.io/pypi/implementation/pyopal.svg?style=flat-square&maxAge=600&label=impl)](https://pypi.org/project/pyopal/#files)
 [![Source](https://img.shields.io/badge/source-GitHub-303030.svg?maxAge=2678400&style=flat-square)](https://github.com/althonos/pyopal/)
 [![Mirror](https://img.shields.io/badge/mirror-EMBL-009f4d?style=flat-square&maxAge=2678400)](https://git.embl.de/larralde/pyopal/)
 [![Issues](https://img.shields.io/github/issues/althonos/pyopal.svg?style=flat-square&maxAge=600)](https://github.com/althonos/pyopal/issues)
 [![Docs](https://img.shields.io/readthedocs/pyopal/latest?style=flat-square&maxAge=600)](https://pyopal.readthedocs.io)
 [![Changelog](https://img.shields.io/badge/keep%20a-changelog-8A0707.svg?maxAge=2678400&style=flat-square)](https://github.com/althonos/pyopal/blob/main/CHANGELOG.md)
-[![Downloads](https://img.shields.io/badge/dynamic/json?style=flat-square&color=303f9f&maxAge=86400&label=downloads&query=%24.total_downloads&url=https%3A%2F%2Fapi.pepy.tech%2Fapi%2Fprojects%2Fpyopal)](https://pepy.tech/project/pyopal)
+[![Downloads](https://img.shields.io/pypi/dm/pyopal?style=flat-square&color=303f9f&maxAge=86400&label=downloads)](https://pepy.tech/project/pyopal)
 
 
 ## 🗺️ Overview
 
 [Opal](https://github.com/Martinsos/opal) is a sequence aligner enabling fast
 sequence similarity search using either of the Smith-Waterman, semi-global or
 Needleman-Wunsch algorithms.
 
 PyOpal is a Python module that provides bindings to [Opal](https://github.com/Martinsos/opal)
 using [Cython](https://cython.org/). It implements a user-friendly, Pythonic
 interface to query a database of sequences and access the search results. It
 interacts with the Opal interface rather than with the CLI, which has the
 following advantages:
 
-- **single dependency**: PyOpal is distributed as a Python package, so you
-  can add it as a dependency to your project, and stop worrying about the
+- **no binary dependency**: PyOpal is distributed as a Python package, so 
+  you can add it as a dependency to your project, and stop worrying about the
   Opal binary being present on the end-user machine.
 - **no intermediate files**: Everything happens in memory, in a Python object
   you control, so you don't have to invoke the Opal CLI using a sub-process
   and temporary files.
 - **better portability**: Opal uses SIMD to accelerate alignment scoring, but
   doesn't support dynamic dispatch, so it has to be compiled on the local
   machine to be able to use the full capabilities of the local CPU. PyOpal
@@ -45,20 +45,21 @@
 - **wider platform support**: The Opal code has been backported to work on SSE2
   rather than SSE4.1, allowing PyOpal to run on older x86 CPUs (all x86 CPUs
   support it since 2003). In addition, Armv7 and Aarch64 CPUs are also
   supported if they implement NEON extensions.
 
 ## 🔧 Installing
 
-PyOpal is available for all modern versions (3.6+), with no external dependencies.
+PyOpal is available for all modern versions (3.6+), depending only 
+on the lightweight Python package [`archspec`](https://pypi.org/project/archspec) 
+for runtime CPU feature detection.
 
 It can be installed directly from [PyPI](https://pypi.org/project/pyopal/),
-which hosts some pre-built wheels for the x86-64 architecture (Linux/OSX)
-and the Aarch64 architecture (Linux only), as well as the code required to compile
-from source with Cython:
+which hosts some pre-built x86-64 and Aarch64 wheels for Linux and MacOS,
+as well as the code required to compile from source with Cython:
 ```console
 $ pip install pyopal
 ```
 
 <!-- Otherwise, PyOpal is also available as a [Bioconda](https://bioconda.github.io/)
 package:
 ```console
@@ -153,16 +154,13 @@
 
 
 ## ⚖️ License
 
 This library is provided under the [MIT License](https://choosealicense.com/licenses/mit/).
 Opal is developed by [Martin Šošić](https://github.com/Martinsos) and is distributed under the
 terms of the MIT License as well. See `vendor/opal/LICENSE` for more information.
-The `cpu_features` library was written by [Guillaume Chatelet](https://github.com/gchatelet) and is
-licensed under the terms of the [Apache License 2.0](https://choosealicense.com/licenses/apache-2.0/).
-See `vendor/cpu_features/LICENSE` for more information.
 
 *This project is in no way not affiliated, sponsored, or otherwise endorsed
 by the [Opal authors](https://github.com/Martinsos). It was developed
 by [Martin Larralde](https://github.com/althonos/) during his PhD project
 at the [European Molecular Biology Laboratory](https://www.embl.de/) in
 the [Zeller team](https://github.com/zellerlab).*
```

### Comparing `pyopal-0.3.0/include/cpu_features/aarch64.pxd` & `pyopal-0.4.0/include/cpu_features/aarch64.pxd`

 * *Files identical despite different names*

### Comparing `pyopal-0.3.0/include/cpu_features/arm.pxd` & `pyopal-0.4.0/include/cpu_features/arm.pxd`

 * *Files identical despite different names*

### Comparing `pyopal-0.3.0/include/opal/__init__.pxd` & `pyopal-0.4.0/include/opal/__init__.pxd`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 
 
 cdef extern from "opal.h" nogil:
 
-    const int OPAL_ERR_OVERFLOW        = 1
-    const int OPAL_ERR_NO_SIMD_SUPPORT = 2
-    const int OPAL_ERR_INVALID_MODE    = 3
-
-    const int OPAL_MODE_NW = 0
-    const int OPAL_MODE_HW = 1
-    const int OPAL_MODE_OV = 2
-    const int OPAL_MODE_SW = 3
-
-    const int OPAL_OVERFLOW_SIMPLE  = 0
-    const int OPAL_OVERFLOW_BUCKETS = 1
-
-    const int OPAL_SEARCH_SCORE     = 0
-    const int OPAL_SEARCH_SCORE_END = 1
-    const int OPAL_SEARCH_ALIGNMENT = 2
-
-    const int OPAL_ALIGN_MATCH    = 0
-    const int OPAL_ALIGN_DEL      = 1
-    const int OPAL_ALIGN_INS      = 2
-    const int OPAL_ALIGN_MISMATCH = 3
-    
+    const int OPAL_ERR_OVERFLOW
+    const int OPAL_ERR_NO_SIMD_SUPPORT
+    const int OPAL_ERR_INVALID_MODE
+
+    const int OPAL_MODE_NW
+    const int OPAL_MODE_HW
+    const int OPAL_MODE_OV
+    const int OPAL_MODE_SW
+
+    const int OPAL_OVERFLOW_SIMPLE
+    const int OPAL_OVERFLOW_BUCKETS
+
+    const int OPAL_SEARCH_SCORE
+    const int OPAL_SEARCH_SCORE_END
+    const int OPAL_SEARCH_ALIGNMENT
+
+    const int OPAL_ALIGN_MATCH
+    const int OPAL_ALIGN_DEL
+    const int OPAL_ALIGN_INS
+    const int OPAL_ALIGN_MISMATCH
+
     cdef struct OpalSearchResult:
         bint scoreSet
         int score
         int endLocationTarget
         int endLocationQuery
         int startLocationTarget
         int startLocationQuery
@@ -34,34 +34,34 @@
         int alignmentLength
 
     cdef void opalInitSearchResult(OpalSearchResult* result)
     cdef bint opalSearchResultIsEmpty(const OpalSearchResult result)
     cdef void opalSearchResultSetScore(OpalSearchResult* result, int score)
 
     cdef int opalSearchDatabase(
-        unsigned char query[], 
-        int queryLength, 
-        unsigned char* db[], 
+        unsigned char query[],
+        int queryLength,
+        unsigned char* db[],
         int dbLength,
-        int dbSeqLengths[], 
-        int gapOpen, 
-        int gapExt, 
+        int dbSeqLengths[],
+        int gapOpen,
+        int gapExt,
         int* scoreMatrix,
-        int alphabetLength, 
+        int alphabetLength,
         OpalSearchResult* results[],
-        const int searchType, 
-        int mode, 
+        const int searchType,
+        int mode,
         int overflowMethod
     )
 
     cdef int opalSearchDatabaseCharSW(
-        unsigned char query[], 
-        int queryLength, 
-        unsigned char** db, 
+        unsigned char query[],
+        int queryLength,
+        unsigned char** db,
         int dbLength,
-        int dbSeqLengths[], 
-        int gapOpen, 
-        int gapExt, 
+        int dbSeqLengths[],
+        int gapOpen,
+        int gapExt,
         int* scoreMatrix,
-        int alphabetLength, 
+        int alphabetLength,
         OpalSearchResult* results[]
     )
```

### Comparing `pyopal-0.3.0/pyopal/__init__.py` & `pyopal-0.4.0/pyopal/__init__.py`

 * *Files identical despite different names*

### Comparing `pyopal-0.3.0/pyopal/_opal.pyi` & `pyopal-0.4.0/pyopal/_opal.pyi`

 * *Files identical despite different names*

### Comparing `pyopal-0.3.0/pyopal/_opal.pyx` & `pyopal-0.4.0/pyopal/_opal.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -17,34 +17,33 @@
 from libcpp.string cimport string
 from libcpp.vector cimport vector
 
 from cpython cimport Py_INCREF
 from cpython.buffer cimport PyBUF_FORMAT
 from cpython.list cimport PyList_New, PyList_SET_ITEM
 from cpython.bytes cimport PyBytes_AsString, PyBytes_FromStringAndSize
-from cpython.mem cimport PyMem_Malloc, PyMem_Realloc, PyMem_Free
-from _unicode cimport (
-    PyUnicode_READY,
+from cpython.mem cimport PyMem_Calloc, PyMem_Realloc, PyMem_Free
+from cpython.unicode cimport (
     PyUnicode_KIND,
     PyUnicode_DATA,
     PyUnicode_READ,
     PyUnicode_GET_LENGTH,
 )
 
 cimport opal
 cimport opal.score_matrix
 from opal cimport OpalSearchResult
 
-IF NEON_BUILD_SUPPORT:
+if NEON_BUILD_SUPPORT:
     from pyopal._opal_neon cimport opalSearchDatabaseNEON
-IF SSE2_BUILD_SUPPORT:
+if SSE2_BUILD_SUPPORT:
     from pyopal._opal_sse2 cimport opalSearchDatabaseSSE2
-IF SSE4_BUILD_SUPPORT:
+if SSE4_BUILD_SUPPORT:
     from pyopal._opal_sse4 cimport opalSearchDatabaseSSE4
-IF AVX2_BUILD_SUPPORT:
+if AVX2_BUILD_SUPPORT:
     from pyopal._opal_avx2 cimport opalSearchDatabaseAVX2
 
 cdef extern from "<cctype>" namespace "std" nogil:
     cdef int toupper(int ch)
     cdef int tolower(int ch)
     cdef bint isalpha(int cht)
 
@@ -61,14 +60,16 @@
         void unlock_shared()
 
 
 # --- Python imports -----------------------------------------------------------
 
 import operator
 
+include "_version.py"
+include "_patch.pxi"
 
 # --- Constants ----------------------------------------------------------------
 
 cdef dict _OPAL_SEARCH_MODES = {
     "score": opal.OPAL_SEARCH_SCORE,
     "end": opal.OPAL_SEARCH_SCORE_END,
     "full": opal.OPAL_SEARCH_ALIGNMENT,
@@ -177,50 +178,44 @@
     def __exit__(self, exc_type, exc_value, traceback):
         self.owner.mutex.unlock()
 
 
 # --- Sequence encoding --------------------------------------------------------
 
 cdef inline void encode_str(str sequence, char* lut, seq_t* encoded, int* length) except *:
-    cdef size_t  i
+    cdef ssize_t i
     cdef char    code
     cdef Py_UCS4 letter
 
-    # make sure the unicode string is in canonical form,
-    # --> won't be needed anymore in Python 3.12
-    IF SYS_VERSION_INFO_MAJOR <= 3 and SYS_VERSION_INFO_MINOR < 12:
-        PyUnicode_READY(sequence)
-
     cdef int     kind = PyUnicode_KIND(sequence)
     cdef void*   data = PyUnicode_DATA(sequence)
     cdef ssize_t slen = PyUnicode_GET_LENGTH(sequence)
 
     length[0] = slen
-    encoded[0] = <seq_t> PyMem_Malloc(length[0] * sizeof(digit_t))
+    encoded[0] = <seq_t> PyMem_Calloc(length[0], sizeof(digit_t))
     if encoded[0] is NULL:
         raise MemoryError("Failed to allocate sequence data")
 
-    with nogil:
-        for i in range(length[0]):
-            letter = PyUnicode_READ(kind, data, i)
-            if not isalpha(letter):
-                raise ValueError(f"Character outside ASCII range: {letter}")
-            code = lut[<unsigned char> letter]
-            if code < 0:
-                raise ValueError(f"Non-alphabet character in sequence: {chr(letter)}")
-            encoded[0][i] = code
+    for i in range(length[0]):
+        letter = PyUnicode_READ(kind, data, i)
+        if not isalpha(letter):
+            raise ValueError(f"Character outside ASCII range: {letter}")
+        code = lut[<unsigned char> letter]
+        if code < 0:
+            raise ValueError(f"Non-alphabet character in sequence: {chr(letter)}")
+        encoded[0][i] = code
 
 
 cdef inline void encode_bytes(const unsigned char[:] sequence, char* lut, seq_t* encoded, int* length) except *:
-    cdef size_t        i
+    cdef ssize_t       i
     cdef char          code
     cdef unsigned char letter
 
     length[0]  = sequence.shape[0]
-    encoded[0] = <seq_t> PyMem_Malloc(length[0] * sizeof(digit_t))
+    encoded[0] = <seq_t> PyMem_Calloc(length[0], sizeof(digit_t))
     if encoded[0] is NULL:
         raise MemoryError("Failed to allocate sequence data")
 
     with nogil:
         for i in range(length[0]):
             letter = <unsigned char> sequence[i]
             code = lut[letter]
@@ -589,15 +584,15 @@
         Example:
             >>> db = Database(["AACCGCTG"])
             >>> hit = db.search("ACCTCG", mode="full", algorithm="nw")[0]
             >>> hit.cigar()
             '1D5M1D1M'
 
         """
-        cdef size_t        i
+        cdef ssize_t       i
         cdef unsigned char symbol
         cdef unsigned char current
         cdef size_t        count
         cdef Py_UCS4[3]    symbols = ['M', 'I', 'D']
         cdef list          chunks  = []
 
         if self._result.alignmentLength == 0 or self._result.alignment is None:
@@ -668,15 +663,15 @@
                 0.875
 
         .. versionadded:: 0.2.0
 
         """
         assert self._result.alignment is not NULL
 
-        cdef size_t  i
+        cdef ssize_t i
         cdef ssize_t length
         cdef ssize_t reflength
         cdef char    operation
 
         # compute alignment and total lengths on reference sequence
         if reference == "query":
             reflength = self._query_length
@@ -736,26 +731,22 @@
         self.clear()
         # record the score matrix
         self.score_matrix = score_matrix or ScoreMatrix.aa()
         # add the sequences to the database
         self.extend(sequences)
 
         # Select the best available SIMD backend
-        IF SSE2_BUILD_SUPPORT:
-            if _SSE2_RUNTIME_SUPPORT:
-                self._search = opalSearchDatabaseSSE2
-        IF SSE4_BUILD_SUPPORT:
-            if _SSE4_RUNTIME_SUPPORT:
-                self._search = opalSearchDatabaseSSE4
-        IF AVX2_BUILD_SUPPORT:
-            if _AVX2_RUNTIME_SUPPORT:
-                self._search = opalSearchDatabaseAVX2
-        IF NEON_BUILD_SUPPORT:
-            if _NEON_RUNTIME_SUPPORT:
-                self._search = opalSearchDatabaseNEON
+        if SSE2_BUILD_SUPPORT and _SSE2_RUNTIME_SUPPORT:
+            self._search = opalSearchDatabaseSSE2
+        if SSE4_BUILD_SUPPORT and _SSE4_RUNTIME_SUPPORT:
+            self._search = opalSearchDatabaseSSE4
+        if AVX2_BUILD_SUPPORT and _AVX2_RUNTIME_SUPPORT:
+            self._search = opalSearchDatabaseAVX2
+        if NEON_BUILD_SUPPORT and _NEON_RUNTIME_SUPPORT:
+            self._search = opalSearchDatabaseNEON
         if self._search is NULL:
             raise RuntimeError("No supported SIMD backend available")
 
     def __dealloc__(self):
         cdef size_t i
         for i in range(self._sequences.size()):
             PyMem_Free(self._sequences[i])
@@ -766,15 +757,15 @@
     # --- Sequence interface ---------------------------------------------------
 
     def __len__(self):
         with self.lock.read:
             return self._sequences.size()
 
     def __getitem__(self, ssize_t index):
-        cdef size_t         i
+        cdef ssize_t        i
         cdef bytearray      decoded
         cdef seq_t          encoded
         cdef size_t         size
         cdef ssize_t        index_   = index
         cdef unsigned char* alphabet = self.score_matrix._mx.getAlphabet()
 
         with self.lock.read:
@@ -991,15 +982,15 @@
         subdb = Database.__new__(Database)
         subdb.score_matrix = self.score_matrix
         subdb._search = self._search
 
         for i, b in enumerate(bitmask):
             if b:
                 length = self._lengths[i]
-                seq = <seq_t> PyMem_Malloc(length * sizeof(digit_t))
+                seq = <seq_t> PyMem_Calloc(length, sizeof(digit_t))
                 if seq is NULL:
                     raise MemoryError("Failed to allocate sequence data")
                 with nogil:
                     memcpy(seq, self._sequences[i], length * sizeof(digit_t))
                     subdb._sequences.push_back(seq)
                     subdb._lengths.push_back(length)
 
@@ -1036,15 +1027,15 @@
         subdb._sequences.reserve(len(indices))
         subdb._lengths.reserve(len(indices))
 
         for index in indices:
             if index < 0 or index >= len(self):
                 raise IndexError(index)
             length = self._lengths[index]
-            seq = <seq_t> PyMem_Malloc(length * sizeof(digit_t))
+            seq = <seq_t> PyMem_Calloc(length, sizeof(digit_t))
             if seq is NULL:
                 raise MemoryError("Failed to allocate sequence data")
             with nogil:
                 memcpy(seq, self._sequences[index], length * sizeof(digit_t))
                 subdb._sequences.push_back(seq)
                 subdb._lengths.push_back(length)
 
@@ -1145,15 +1136,15 @@
         # Prepare query
         encode(sequence, self.score_matrix._ahash, &query, &length)
 
         with self.lock.read:
             size = self._sequences.size()
 
             # Prepare list of results
-            res_array = PyMem_Malloc(sizeof(OpalSearchResult*) * size)
+            res_array = PyMem_Calloc(size, sizeof(OpalSearchResult*))
             results_raw.reserve(size)
             results = PyList_New(size)
             for i in range(size):
                 result = result_type.__new__(result_type)
                 result._target_index = i
                 Py_INCREF(result)
                 PyList_SET_ITEM(results, i, result)
```

### Comparing `pyopal-0.3.0/pyopal/_opal_avx2.pyx` & `pyopal-0.4.0/pyopal/_opal_neon.pyx`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # distutils: language = c++
 # cython: language_level=3, linetrace=True, embedsignature=True, binding=True
 
 cimport opal
 
-cdef int opalSearchDatabaseAVX2(
+include "_version.py"
+include "_patch.pxi"
+
+cdef int opalSearchDatabaseNEON(
     unsigned char query[], 
     int queryLength, 
     unsigned char* db[], 
     int dbLength,
     int dbSeqLengths[], 
     int gapOpen, 
     int gapExt,
```

### Comparing `pyopal-0.3.0/pyopal/_opal_neon.pyx` & `pyopal-0.4.0/pyopal/_opal_sse4.pyx`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # distutils: language = c++
 # cython: language_level=3, linetrace=True, embedsignature=True, binding=True
 
 cimport opal
 
-cdef int opalSearchDatabaseNEON(
+include "_version.py"
+include "_patch.pxi"
+
+cdef int opalSearchDatabaseSSE4(
     unsigned char query[], 
     int queryLength, 
     unsigned char* db[], 
     int dbLength,
     int dbSeqLengths[], 
     int gapOpen, 
     int gapExt,
```

### Comparing `pyopal-0.3.0/pyopal/_opal_sse2.pyx` & `pyopal-0.4.0/pyopal/_opal_avx2.pyx`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # distutils: language = c++
 # cython: language_level=3, linetrace=True, embedsignature=True, binding=True
 
 cimport opal
 
-cdef int opalSearchDatabaseSSE2(
+include "_version.py"
+include "_patch.pxi"
+
+cdef int opalSearchDatabaseAVX2(
     unsigned char query[], 
     int queryLength, 
     unsigned char* db[], 
     int dbLength,
     int dbSeqLengths[], 
     int gapOpen, 
     int gapExt,
```

### Comparing `pyopal-0.3.0/pyopal/_opal_sse4.pyx` & `pyopal-0.4.0/pyopal/_opal_sse2.pyx`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # distutils: language = c++
 # cython: language_level=3, linetrace=True, embedsignature=True, binding=True
 
 cimport opal
 
-cdef int opalSearchDatabaseSSE4(
+include "_version.py"
+include "_patch.pxi"
+
+cdef int opalSearchDatabaseSSE2(
     unsigned char query[], 
     int queryLength, 
     unsigned char* db[], 
     int dbLength,
     int dbSeqLengths[], 
     int gapOpen, 
     int gapExt,
```

### Comparing `pyopal-0.3.0/pyopal/tests/test_database.py` & `pyopal-0.4.0/pyopal/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `pyopal-0.3.0/pyopal/tests/test_doctest.py` & `pyopal-0.4.0/pyopal/tests/test_doctest.py`

 * *Files identical despite different names*

### Comparing `pyopal-0.3.0/pyopal/tests/test_search.py` & `pyopal-0.4.0/pyopal/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `pyopal-0.3.0/pyopal.egg-info/PKG-INFO` & `pyopal-0.4.0/pyopal.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyopal
-Version: 0.3.0
+Version: 0.4.0
 Summary: Cython bindings and Python interface to Opal, a SIMD-accelerated pairwise aligner.
 Home-page: https://github.com/althonos/pyopal
 Author: Martin Larralde
 Author-email: martin.larralde@embl.de
 License: MIT
 Project-URL: Documentation, https://pyopal.readthedocs.io/en/stable/
 Project-URL: Bug Tracker, https://github.com/althonos/pyopal/issues
@@ -50,31 +50,31 @@
 [![Python Versions](https://img.shields.io/pypi/pyversions/pyopal.svg?style=flat-square&maxAge=600&logo=python)](https://pypi.org/project/pyopal/#files)
 [![Python Implementations](https://img.shields.io/pypi/implementation/pyopal.svg?style=flat-square&maxAge=600&label=impl)](https://pypi.org/project/pyopal/#files)
 [![Source](https://img.shields.io/badge/source-GitHub-303030.svg?maxAge=2678400&style=flat-square)](https://github.com/althonos/pyopal/)
 [![Mirror](https://img.shields.io/badge/mirror-EMBL-009f4d?style=flat-square&maxAge=2678400)](https://git.embl.de/larralde/pyopal/)
 [![Issues](https://img.shields.io/github/issues/althonos/pyopal.svg?style=flat-square&maxAge=600)](https://github.com/althonos/pyopal/issues)
 [![Docs](https://img.shields.io/readthedocs/pyopal/latest?style=flat-square&maxAge=600)](https://pyopal.readthedocs.io)
 [![Changelog](https://img.shields.io/badge/keep%20a-changelog-8A0707.svg?maxAge=2678400&style=flat-square)](https://github.com/althonos/pyopal/blob/main/CHANGELOG.md)
-[![Downloads](https://img.shields.io/badge/dynamic/json?style=flat-square&color=303f9f&maxAge=86400&label=downloads&query=%24.total_downloads&url=https%3A%2F%2Fapi.pepy.tech%2Fapi%2Fprojects%2Fpyopal)](https://pepy.tech/project/pyopal)
+[![Downloads](https://img.shields.io/pypi/dm/pyopal?style=flat-square&color=303f9f&maxAge=86400&label=downloads)](https://pepy.tech/project/pyopal)
 
 
 ## 🗺️ Overview
 
 [Opal](https://github.com/Martinsos/opal) is a sequence aligner enabling fast
 sequence similarity search using either of the Smith-Waterman, semi-global or
 Needleman-Wunsch algorithms.
 
 PyOpal is a Python module that provides bindings to [Opal](https://github.com/Martinsos/opal)
 using [Cython](https://cython.org/). It implements a user-friendly, Pythonic
 interface to query a database of sequences and access the search results. It
 interacts with the Opal interface rather than with the CLI, which has the
 following advantages:
 
-- **single dependency**: PyOpal is distributed as a Python package, so you
-  can add it as a dependency to your project, and stop worrying about the
+- **no binary dependency**: PyOpal is distributed as a Python package, so 
+  you can add it as a dependency to your project, and stop worrying about the
   Opal binary being present on the end-user machine.
 - **no intermediate files**: Everything happens in memory, in a Python object
   you control, so you don't have to invoke the Opal CLI using a sub-process
   and temporary files.
 - **better portability**: Opal uses SIMD to accelerate alignment scoring, but
   doesn't support dynamic dispatch, so it has to be compiled on the local
   machine to be able to use the full capabilities of the local CPU. PyOpal
@@ -83,20 +83,21 @@
 - **wider platform support**: The Opal code has been backported to work on SSE2
   rather than SSE4.1, allowing PyOpal to run on older x86 CPUs (all x86 CPUs
   support it since 2003). In addition, Armv7 and Aarch64 CPUs are also
   supported if they implement NEON extensions.
 
 ## 🔧 Installing
 
-PyOpal is available for all modern versions (3.6+), with no external dependencies.
+PyOpal is available for all modern versions (3.6+), depending only 
+on the lightweight Python package [`archspec`](https://pypi.org/project/archspec) 
+for runtime CPU feature detection.
 
 It can be installed directly from [PyPI](https://pypi.org/project/pyopal/),
-which hosts some pre-built wheels for the x86-64 architecture (Linux/OSX)
-and the Aarch64 architecture (Linux only), as well as the code required to compile
-from source with Cython:
+which hosts some pre-built x86-64 and Aarch64 wheels for Linux and MacOS,
+as well as the code required to compile from source with Cython:
 ```console
 $ pip install pyopal
 ```
 
 <!-- Otherwise, PyOpal is also available as a [Bioconda](https://bioconda.github.io/)
 package:
 ```console
@@ -191,16 +192,13 @@
 
 
 ## ⚖️ License
 
 This library is provided under the [MIT License](https://choosealicense.com/licenses/mit/).
 Opal is developed by [Martin Šošić](https://github.com/Martinsos) and is distributed under the
 terms of the MIT License as well. See `vendor/opal/LICENSE` for more information.
-The `cpu_features` library was written by [Guillaume Chatelet](https://github.com/gchatelet) and is
-licensed under the terms of the [Apache License 2.0](https://choosealicense.com/licenses/apache-2.0/).
-See `vendor/cpu_features/LICENSE` for more information.
 
 *This project is in no way not affiliated, sponsored, or otherwise endorsed
 by the [Opal authors](https://github.com/Martinsos). It was developed
 by [Martin Larralde](https://github.com/althonos/) during his PhD project
 at the [European Molecular Biology Laboratory](https://www.embl.de/) in
 the [Zeller team](https://github.com/zellerlab).*
```

### Comparing `pyopal-0.3.0/pyopal.egg-info/SOURCES.txt` & `pyopal-0.4.0/pyopal.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 CONTRIBUTING.md
 COPYING
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
-include/_unicode.pxd
 include/cpu_features/__init__.pxd
 include/cpu_features/aarch64.pxd
 include/cpu_features/arm.pxd
 include/cpu_features/x86.pxd
 include/opal/__init__.pxd
 include/opal/score_matrix.pxd
 pyopal/__init__.py
@@ -20,14 +19,15 @@
 pyopal/_opal_avx2.pyx
 pyopal/_opal_neon.pxd
 pyopal/_opal_neon.pyx
 pyopal/_opal_sse2.pxd
 pyopal/_opal_sse2.pyx
 pyopal/_opal_sse4.pxd
 pyopal/_opal_sse4.pyx
+pyopal/_patch.pxi
 pyopal/_version.py
 pyopal/py.typed
 pyopal.egg-info/PKG-INFO
 pyopal.egg-info/SOURCES.txt
 pyopal.egg-info/dependency_links.txt
 pyopal.egg-info/not-zip-safe
 pyopal.egg-info/requires.txt
```

### Comparing `pyopal-0.3.0/setup.cfg` & `pyopal-0.4.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 [options]
 zip_safe = false
 packages = pyopal, pyopal.tests
 include_package_data = false
 python_requires = >=3.5
 setup_requires = 
 	setuptools >=46.4
-	cython ~=0.29.16
+	cython ~=3.0
 install_requires = 
 	archspec ~=0.2
 tests_require = 
 	importlib-resources ; python_version < '3.7'
 
 [options.package_data]
 pyopal = py.typed, *.pyi
```

### Comparing `pyopal-0.3.0/setup.py` & `pyopal-0.4.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -273,14 +273,53 @@
             header="arm_neon.h",
             vector="int16x8_t",
             set="vdupq_n_s16",
             op="vabsq_s16",
             extract="vgetq_lane_s16",
         )
 
+    def _check_getid(self):
+        _eprint('checking whether `PyInterpreterState_GetID` is available')
+
+        base = "have_getid"
+        testfile = os.path.join(self.build_temp, "{}.c".format(base))
+        objects = []
+
+        self.mkpath(self.build_temp)
+        with open(testfile, "w") as f:
+            f.write("""
+            #include <stdint.h>
+            #include <stdlib.h>
+            #include <Python.h>
+
+            int main(int argc, char *argv[]) {{
+                PyInterpreterState_GetID(NULL);
+                return 0;
+            }}
+            """)
+
+        if self.compiler.compiler_type == "msvc":
+            flags = ["/WX"]
+        else:
+            flags = ["-Werror=implicit-function-declaration"]
+
+        try:
+            self.mkpath(self.build_temp)
+            objects = self.compiler.compile([testfile], extra_postargs=flags)
+        except CompileError:
+            _eprint("no")
+            return False
+        else:
+            _eprint("yes")
+            return True
+        finally:
+            os.remove(testfile)
+            for obj in filter(os.path.isfile, objects):
+                os.remove(obj)
+
     # --- Build code ---
 
     def build_extension(self, ext):
         # show the compiler being used
         _eprint("building", ext.name, "with", self.compiler.compiler_type, "compiler")
 
         # add debug symbols if we are building in debug mode
@@ -315,14 +354,18 @@
             lib = self._clib_cmd.get_library(name)
             libfile = self.compiler.library_filename(
                 lib.name, output_dir=self._clib_cmd.build_clib
             )
             ext.depends.append(libfile)
             ext.extra_objects.append(libfile)
 
+        # check if `PyInterpreterState_GetID` is defined
+        if self._check_getid():
+            ext.define_macros.append(("HAS_PYINTERPRETERSTATE_GETID", 1))
+
         # build the rest of the extension as normal
         ext._needs_stub = False
 
         # compile extension in its own folder: since we need to compile
         # `opal.cpp` several times with different flags, we cannot use the
         # default build folder, otherwise the built object would be cached
         # and prevent recompilation
```

### Comparing `pyopal-0.3.0/vendor/opal/LICENSE` & `pyopal-0.4.0/vendor/opal/LICENSE`

 * *Files identical despite different names*

### Comparing `pyopal-0.3.0/vendor/opal/README.md` & `pyopal-0.4.0/vendor/opal/README.md`

 * *Files identical despite different names*

### Comparing `pyopal-0.3.0/vendor/opal/src/ScoreMatrix.cpp` & `pyopal-0.4.0/vendor/opal/src/ScoreMatrix.cpp`

 * *Files identical despite different names*

### Comparing `pyopal-0.3.0/vendor/opal/src/ScoreMatrix.hpp` & `pyopal-0.4.0/vendor/opal/src/ScoreMatrix.hpp`

 * *Files identical despite different names*

### Comparing `pyopal-0.3.0/vendor/opal/src/opal.cpp` & `pyopal-0.4.0/vendor/opal/src/opal.cpp`

 * *Files identical despite different names*

### Comparing `pyopal-0.3.0/vendor/opal/src/opal.h` & `pyopal-0.4.0/vendor/opal/src/opal.h`

 * *Files identical despite different names*

### Comparing `pyopal-0.3.0/vendor/opal/src/opal_aligner.cpp` & `pyopal-0.4.0/vendor/opal/src/opal_aligner.cpp`

 * *Files identical despite different names*

### Comparing `pyopal-0.3.0/vendor/opal/src/test.cpp` & `pyopal-0.4.0/vendor/opal/src/test.cpp`

 * *Files identical despite different names*

