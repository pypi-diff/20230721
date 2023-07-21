# Comparing `tmp/thermoblock-23.7.0.dev1.tar.gz` & `tmp/thermoblock-23.7.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thermoblock-23.7.0.dev1.tar", last modified: Thu Jul 20 13:50:23 2023, max compression
+gzip compressed data, was "thermoblock-23.7.0.dev2.tar", last modified: Fri Jul 21 13:10:37 2023, max compression
```

## Comparing `thermoblock-23.7.0.dev1.tar` & `thermoblock-23.7.0.dev2.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:50:23.220284 thermoblock-23.7.0.dev1/
--rw-r--r--   0 runner    (1001) docker     (122)      298 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:50:23.212284 thermoblock-23.7.0.dev1/.github/
--rw-r--r--   0 runner    (1001) docker     (122)      454 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:50:23.212284 thermoblock-23.7.0.dev1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     1131 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1999 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (122)     3704 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1394 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (122)      184 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1745 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1020 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (122)     1565 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     5901 2023-07-20 13:50:23.220284 thermoblock-23.7.0.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3340 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:50:23.212284 thermoblock-23.7.0.dev1/conda/
--rw-r--r--   0 runner    (1001) docker     (122)      671 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/conda/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:50:23.212284 thermoblock-23.7.0.dev1/docs/
--rw-r--r--   0 runner    (1001) docker     (122)     5672 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:50:23.216284 thermoblock-23.7.0.dev1/docs/developer/
--rw-r--r--   0 runner    (1001) docker     (122)     3541 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/docs/developer/coding-conventions.md
--rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/docs/developer/dependency-management.md
--rw-r--r--   0 runner    (1001) docker     (122)     1776 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/docs/developer/getting-started.md
--rw-r--r--   0 runner    (1001) docker     (122)      207 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/docs/developer/index.md
--rw-r--r--   0 runner    (1001) docker     (122)      190 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (122)     1490 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:50:23.216284 thermoblock-23.7.0.dev1/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      180 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/requirements/ci.in
--rw-r--r--   0 runner    (1001) docker     (122)      933 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/requirements/ci.txt
--rw-r--r--   0 runner    (1001) docker     (122)      108 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/requirements/dev.in
--rw-r--r--   0 runner    (1001) docker     (122)     2070 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)      306 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (122)     4649 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/requirements/static.in
--rw-r--r--   0 runner    (1001) docker     (122)      575 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/requirements/static.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (122)      359 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/requirements/wheels.in
--rw-r--r--   0 runner    (1001) docker     (122)      282 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/requirements/wheels.txt
--rw-r--r--   0 runner    (1001) docker     (122)      252 2023-07-20 13:50:23.220284 thermoblock-23.7.0.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      135 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/setup.sh
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:50:23.208284 thermoblock-23.7.0.dev1/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:50:23.216284 thermoblock-23.7.0.dev1/src/thermoblock/
--rw-r--r--   0 runner    (1001) docker     (122)      311 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/src/thermoblock/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:50:23.220284 thermoblock-23.7.0.dev1/src/thermoblock/resources/
--rw-r--r--   0 runner    (1001) docker     (122)    39823 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/src/thermoblock/resources/colorspectrum.jpg
--rw-r--r--   0 runner    (1001) docker     (122)    28100 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/src/thermoblock/resources/colorspectrum.pck
--rw-r--r--   0 runner    (1001) docker     (122)      136 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/src/thermoblock/resources/materiallist.pck
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:50:23.220284 thermoblock-23.7.0.dev1/src/thermoblock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     5901 2023-07-20 13:50:23.000000 thermoblock-23.7.0.dev1/src/thermoblock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-07-20 13:50:23.000000 thermoblock-23.7.0.dev1/src/thermoblock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 13:50:23.000000 thermoblock-23.7.0.dev1/src/thermoblock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-07-20 13:50:23.000000 thermoblock-23.7.0.dev1/src/thermoblock.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:50:23.220284 thermoblock-23.7.0.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      210 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/tests/package_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1528 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 13:10:37.693289 thermoblock-23.7.0.dev2/
+-rw-r--r--   0 runner    (1001) docker     (122)      298 2023-07-21 13:10:23.000000 thermoblock-23.7.0.dev2/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 13:10:37.681289 thermoblock-23.7.0.dev2/.github/
+-rw-r--r--   0 runner    (1001) docker     (122)      454 2023-07-21 13:10:23.000000 thermoblock-23.7.0.dev2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 13:10:37.685289 thermoblock-23.7.0.dev2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     1131 2023-07-21 13:10:23.000000 thermoblock-23.7.0.dev2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1999 2023-07-21 13:10:23.000000 thermoblock-23.7.0.dev2/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     3704 2023-07-21 13:10:23.000000 thermoblock-23.7.0.dev2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1406 2023-07-21 13:10:23.000000 thermoblock-23.7.0.dev2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      184 2023-07-21 13:10:23.000000 thermoblock-23.7.0.dev2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1745 2023-07-21 13:10:23.000000 thermoblock-23.7.0.dev2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1020 2023-07-21 13:10:23.000000 thermoblock-23.7.0.dev2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1565 2023-07-21 13:10:23.000000 thermoblock-23.7.0.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-07-21 13:10:23.000000 thermoblock-23.7.0.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     5898 2023-07-21 13:10:37.693289 thermoblock-23.7.0.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3331 2023-07-21 13:10:23.000000 thermoblock-23.7.0.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 13:10:37.685289 thermoblock-23.7.0.dev2/conda/
+-rw-r--r--   0 runner    (1001) docker     (122)      671 2023-07-21 13:10:23.000000 thermoblock-23.7.0.dev2/conda/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 13:10:37.685289 thermoblock-23.7.0.dev2/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     5684 2023-07-21 13:10:23.000000 thermoblock-23.7.0.dev2/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 13:10:37.685289 thermoblock-23.7.0.dev2/docs/developer/
+-rw-r--r--   0 runner    (1001) docker     (122)     3541 2023-07-21 13:10:23.000000 thermoblock-23.7.0.dev2/docs/developer/coding-conventions.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-07-21 13:10:23.000000 thermoblock-23.7.0.dev2/docs/developer/dependency-management.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1776 2023-07-21 13:10:23.000000 thermoblock-23.7.0.dev2/docs/developer/getting-started.md
+-rw-r--r--   0 runner    (1001) docker     (122)      207 2023-07-21 13:10:23.000000 thermoblock-23.7.0.dev2/docs/developer/index.md
+-rw-r--r--   0 runner    (1001) docker     (122)      190 2023-07-21 13:10:23.000000 thermoblock-23.7.0.dev2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1496 2023-07-21 13:10:23.000000 thermoblock-23.7.0.dev2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 13:10:37.689289 thermoblock-23.7.0.dev2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-07-21 13:10:23.000000 thermoblock-23.7.0.dev2/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      180 2023-07-21 13:10:23.000000 thermoblock-23.7.0.dev2/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-07-21 13:10:23.000000 thermoblock-23.7.0.dev2/requirements/ci.in
+-rw-r--r--   0 runner    (1001) docker     (122)      933 2023-07-21 13:10:23.000000 thermoblock-23.7.0.dev2/requirements/ci.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      108 2023-07-21 13:10:23.000000 thermoblock-23.7.0.dev2/requirements/dev.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2070 2023-07-21 13:10:23.000000 thermoblock-23.7.0.dev2/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      306 2023-07-21 13:10:23.000000 thermoblock-23.7.0.dev2/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4649 2023-07-21 13:10:23.000000 thermoblock-23.7.0.dev2/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-07-21 13:10:23.000000 thermoblock-23.7.0.dev2/requirements/static.in
+-rw-r--r--   0 runner    (1001) docker     (122)      575 2023-07-21 13:10:23.000000 thermoblock-23.7.0.dev2/requirements/static.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-07-21 13:10:23.000000 thermoblock-23.7.0.dev2/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (122)      359 2023-07-21 13:10:23.000000 thermoblock-23.7.0.dev2/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-07-21 13:10:23.000000 thermoblock-23.7.0.dev2/requirements/wheels.in
+-rw-r--r--   0 runner    (1001) docker     (122)      282 2023-07-21 13:10:23.000000 thermoblock-23.7.0.dev2/requirements/wheels.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-07-21 13:10:37.693289 thermoblock-23.7.0.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2023-07-21 13:10:23.000000 thermoblock-23.7.0.dev2/setup.sh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 13:10:37.681289 thermoblock-23.7.0.dev2/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 13:10:37.689289 thermoblock-23.7.0.dev2/src/thermoblock/
+-rw-r--r--   0 runner    (1001) docker     (122)      311 2023-07-21 13:10:23.000000 thermoblock-23.7.0.dev2/src/thermoblock/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 13:10:37.689289 thermoblock-23.7.0.dev2/src/thermoblock/resources/
+-rw-r--r--   0 runner    (1001) docker     (122)    39823 2023-07-21 13:10:23.000000 thermoblock-23.7.0.dev2/src/thermoblock/resources/colorspectrum.jpg
+-rw-r--r--   0 runner    (1001) docker     (122)    28100 2023-07-21 13:10:23.000000 thermoblock-23.7.0.dev2/src/thermoblock/resources/colorspectrum.pck
+-rw-r--r--   0 runner    (1001) docker     (122)      136 2023-07-21 13:10:23.000000 thermoblock-23.7.0.dev2/src/thermoblock/resources/materiallist.pck
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 13:10:37.689289 thermoblock-23.7.0.dev2/src/thermoblock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     5898 2023-07-21 13:10:37.000000 thermoblock-23.7.0.dev2/src/thermoblock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-07-21 13:10:37.000000 thermoblock-23.7.0.dev2/src/thermoblock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-21 13:10:37.000000 thermoblock-23.7.0.dev2/src/thermoblock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-07-21 13:10:37.000000 thermoblock-23.7.0.dev2/src/thermoblock.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 13:10:37.693289 thermoblock-23.7.0.dev2/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      210 2023-07-21 13:10:23.000000 thermoblock-23.7.0.dev2/tests/package_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1528 2023-07-21 13:10:23.000000 thermoblock-23.7.0.dev2/tox.ini
```

### Comparing `thermoblock-23.7.0.dev1/.github/workflows/ci.yml` & `thermoblock-23.7.0.dev2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `thermoblock-23.7.0.dev1/.github/workflows/docs.yml` & `thermoblock-23.7.0.dev2/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `thermoblock-23.7.0.dev1/.github/workflows/release.yml` & `thermoblock-23.7.0.dev2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `thermoblock-23.7.0.dev1/.github/workflows/test.yml` & `thermoblock-23.7.0.dev2/.github/workflows/test.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
+# Copyright (c) 2023 PhysicsCore contributors (https://github.com/physicscore)
 
 name: Test
 
 on:
   workflow_dispatch:
     inputs:
       os-variant:
```

### Comparing `thermoblock-23.7.0.dev1/.pre-commit-config.yaml` & `thermoblock-23.7.0.dev2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `thermoblock-23.7.0.dev1/CONTRIBUTING.md` & `thermoblock-23.7.0.dev2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `thermoblock-23.7.0.dev1/LICENSE` & `thermoblock-23.7.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `thermoblock-23.7.0.dev1/PKG-INFO` & `thermoblock-23.7.0.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: thermoblock
-Version: 23.7.0.dev1
+Version: 23.7.0.dev2
 Summary: Flux simulation toy building library.
-Author: Scipp contributors
+Author: PhysicsCore contributors
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Physicscore contributors (https://github.com/physicscore)
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
@@ -45,16 +45,16 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<!-- [![PyPI badge](http://img.shields.io/pypi/v/thermoblock.svg)](https://pypi.python.org/pypi/thermoblock)
-[![Anaconda-Server Badge](https://anaconda.org/physicscore/thermoblock/badges/version.svg)](https://anaconda.org/physicscore/thermoblock) -->
+[![PyPI badge](http://img.shields.io/pypi/v/thermoblock.svg)](https://pypi.python.org/pypi/thermoblock)
+[![Anaconda-Server Badge](https://anaconda.org/physicscore/thermoblock/badges/version.svg)](https://anaconda.org/physicscore/thermoblock)
 [![License: BSD 3-Clause](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](LICENSE)
 
 # thermoblock
 
 ## About
 
 Flux simulation toy building library.
```

### Comparing `thermoblock-23.7.0.dev1/README.md` & `thermoblock-23.7.0.dev2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-<!-- [![PyPI badge](http://img.shields.io/pypi/v/thermoblock.svg)](https://pypi.python.org/pypi/thermoblock)
-[![Anaconda-Server Badge](https://anaconda.org/physicscore/thermoblock/badges/version.svg)](https://anaconda.org/physicscore/thermoblock) -->
+[![PyPI badge](http://img.shields.io/pypi/v/thermoblock.svg)](https://pypi.python.org/pypi/thermoblock)
+[![Anaconda-Server Badge](https://anaconda.org/physicscore/thermoblock/badges/version.svg)](https://anaconda.org/physicscore/thermoblock)
 [![License: BSD 3-Clause](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](LICENSE)
 
 # thermoblock
 
 ## About
 
 Flux simulation toy building library.
```

### Comparing `thermoblock-23.7.0.dev1/conda/meta.yaml` & `thermoblock-23.7.0.dev2/conda/meta.yaml`

 * *Files identical despite different names*

### Comparing `thermoblock-23.7.0.dev1/docs/conf.py` & `thermoblock-23.7.0.dev2/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
 import thermoblock
 
 sys.path.insert(0, os.path.abspath('.'))
 
 # General information about the project.
 project = u'thermoblock'
-copyright = u'2023 Scipp contributors'
-author = u'Scipp contributors'
+copyright = u'2023 PhysicsCore contributors'
+author = u'PhysicsCore contributors'
 
 html_show_sourcelink = True
 
 extensions = [
     'sphinx.ext.autodoc',
     'sphinx.ext.autosummary',
     'sphinx.ext.doctest',
@@ -140,15 +140,15 @@
             "name": "PyPI",
             "url": "https://pypi.org/project/thermoblock/",
             "icon": "fa-brands fa-python",
             "type": "fontawesome",
         },
         {
             "name": "Conda",
-            "url": "https://anaconda.org/conda-forge/thermoblock",
+            "url": "https://anaconda.org/physicscore/thermoblock",
             "icon": "_static/anaconda-logo.svg",
             "type": "local",
         },
     ],
 }
 html_context = {
     "doc_path": "docs",
```

### Comparing `thermoblock-23.7.0.dev1/docs/developer/coding-conventions.md` & `thermoblock-23.7.0.dev2/docs/developer/coding-conventions.md`

 * *Files identical despite different names*

### Comparing `thermoblock-23.7.0.dev1/docs/developer/dependency-management.md` & `thermoblock-23.7.0.dev2/docs/developer/dependency-management.md`

 * *Files identical despite different names*

### Comparing `thermoblock-23.7.0.dev1/docs/developer/getting-started.md` & `thermoblock-23.7.0.dev2/docs/developer/getting-started.md`

 * *Files identical despite different names*

### Comparing `thermoblock-23.7.0.dev1/pyproject.toml` & `thermoblock-23.7.0.dev2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   "setuptools_scm[toml]>=7.0",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "thermoblock"
 description = "Flux simulation toy building library."
-authors= [{name="Scipp contributors"}]
+authors= [{name="PhysicsCore contributors"}]
 license = { file = "LICENSE" }
 readme = "README.md"
 classifiers = [
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: BSD License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
```

### Comparing `thermoblock-23.7.0.dev1/requirements/ci.txt` & `thermoblock-23.7.0.dev2/requirements/ci.txt`

 * *Files identical despite different names*

### Comparing `thermoblock-23.7.0.dev1/requirements/dev.txt` & `thermoblock-23.7.0.dev2/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `thermoblock-23.7.0.dev1/requirements/docs.txt` & `thermoblock-23.7.0.dev2/requirements/docs.txt`

 * *Files identical despite different names*

### Comparing `thermoblock-23.7.0.dev1/requirements/static.txt` & `thermoblock-23.7.0.dev2/requirements/static.txt`

 * *Files identical despite different names*

### Comparing `thermoblock-23.7.0.dev1/src/thermoblock/resources/colorspectrum.jpg` & `thermoblock-23.7.0.dev2/src/thermoblock/resources/colorspectrum.jpg`

 * *Files identical despite different names*

### Comparing `thermoblock-23.7.0.dev1/src/thermoblock/resources/colorspectrum.pck` & `thermoblock-23.7.0.dev2/src/thermoblock/resources/colorspectrum.pck`

 * *Files identical despite different names*

### Comparing `thermoblock-23.7.0.dev1/src/thermoblock.egg-info/PKG-INFO` & `thermoblock-23.7.0.dev2/src/thermoblock.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: thermoblock
-Version: 23.7.0.dev1
+Version: 23.7.0.dev2
 Summary: Flux simulation toy building library.
-Author: Scipp contributors
+Author: PhysicsCore contributors
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Physicscore contributors (https://github.com/physicscore)
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
@@ -45,16 +45,16 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<!-- [![PyPI badge](http://img.shields.io/pypi/v/thermoblock.svg)](https://pypi.python.org/pypi/thermoblock)
-[![Anaconda-Server Badge](https://anaconda.org/physicscore/thermoblock/badges/version.svg)](https://anaconda.org/physicscore/thermoblock) -->
+[![PyPI badge](http://img.shields.io/pypi/v/thermoblock.svg)](https://pypi.python.org/pypi/thermoblock)
+[![Anaconda-Server Badge](https://anaconda.org/physicscore/thermoblock/badges/version.svg)](https://anaconda.org/physicscore/thermoblock)
 [![License: BSD 3-Clause](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](LICENSE)
 
 # thermoblock
 
 ## About
 
 Flux simulation toy building library.
```

### Comparing `thermoblock-23.7.0.dev1/src/thermoblock.egg-info/SOURCES.txt` & `thermoblock-23.7.0.dev2/src/thermoblock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `thermoblock-23.7.0.dev1/tox.ini` & `thermoblock-23.7.0.dev2/tox.ini`

 * *Files identical despite different names*

