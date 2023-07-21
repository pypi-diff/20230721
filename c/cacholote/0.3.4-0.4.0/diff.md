# Comparing `tmp/cacholote-0.3.4.tar.gz` & `tmp/cacholote-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cacholote-0.3.4.tar", last modified: Wed Jul 19 22:19:36 2023, max compression
+gzip compressed data, was "cacholote-0.4.0.tar", last modified: Fri Jul 21 08:03:57 2023, max compression
```

## Comparing `cacholote-0.3.4.tar` & `cacholote-0.4.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:19:36.746936 cacholote-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-19 22:19:20.000000 cacholote-0.3.4/.cruft.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:19:36.738936 cacholote-0.3.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:19:36.742936 cacholote-0.3.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-07-19 22:19:20.000000 cacholote-0.3.4/.github/workflows/on-push.yml
--rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-07-19 22:19:20.000000 cacholote-0.3.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-19 22:19:20.000000 cacholote-0.3.4/.pre-commit-config-cruft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-19 22:19:20.000000 cacholote-0.3.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-19 22:19:20.000000 cacholote-0.3.4/DESIGN.rst
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-19 22:19:20.000000 cacholote-0.3.4/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-07-19 22:19:20.000000 cacholote-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-19 22:19:20.000000 cacholote-0.3.4/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-19 22:19:20.000000 cacholote-0.3.4/OBJECT-STORAGE-DESIGN.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15708 2023-07-19 22:19:36.746936 cacholote-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-19 22:19:20.000000 cacholote-0.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:19:36.742936 cacholote-0.3.4/cacholote/
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-07-19 22:19:20.000000 cacholote-0.3.4/cacholote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-07-19 22:19:20.000000 cacholote-0.3.4/cacholote/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    10248 2023-07-19 22:19:20.000000 cacholote-0.3.4/cacholote/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-07-19 22:19:20.000000 cacholote-0.3.4/cacholote/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-19 22:19:20.000000 cacholote-0.3.4/cacholote/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-07-19 22:19:20.000000 cacholote-0.3.4/cacholote/decode.py
--rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-07-19 22:19:20.000000 cacholote-0.3.4/cacholote/encode.py
--rw-r--r--   0 runner    (1001) docker     (123)    12807 2023-07-19 22:19:20.000000 cacholote-0.3.4/cacholote/extra_encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 22:19:20.000000 cacholote-0.3.4/cacholote/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-07-19 22:19:20.000000 cacholote-0.3.4/cacholote/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-19 22:19:36.000000 cacholote-0.3.4/cacholote/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:19:36.742936 cacholote-0.3.4/cacholote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15708 2023-07-19 22:19:36.000000 cacholote-0.3.4/cacholote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-19 22:19:36.000000 cacholote-0.3.4/cacholote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 22:19:36.000000 cacholote-0.3.4/cacholote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-19 22:19:36.000000 cacholote-0.3.4/cacholote.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-19 22:19:36.000000 cacholote-0.3.4/cacholote.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:19:36.742936 cacholote-0.3.4/ci/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-19 22:19:20.000000 cacholote-0.3.4/ci/environment-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-19 22:19:20.000000 cacholote-0.3.4/ci/environment-integration.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:19:36.742936 cacholote-0.3.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-19 22:19:20.000000 cacholote-0.3.4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:19:36.742936 cacholote-0.3.4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 22:19:20.000000 cacholote-0.3.4/docs/_static/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:19:36.742936 cacholote-0.3.4/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 22:19:20.000000 cacholote-0.3.4/docs/_templates/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-19 22:19:20.000000 cacholote-0.3.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-19 22:19:20.000000 cacholote-0.3.4/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-19 22:19:20.000000 cacholote-0.3.4/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-19 22:19:20.000000 cacholote-0.3.4/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-19 22:19:20.000000 cacholote-0.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 22:19:36.746936 cacholote-0.3.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:19:36.746936 cacholote-0.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-07-19 22:19:20.000000 cacholote-0.3.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-19 22:19:20.000000 cacholote-0.3.4/tests/test_00_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-07-19 22:19:20.000000 cacholote-0.3.4/tests/test_01_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-19 22:19:20.000000 cacholote-0.3.4/tests/test_02_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-19 22:19:20.000000 cacholote-0.3.4/tests/test_10_decode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-07-19 22:19:20.000000 cacholote-0.3.4/tests/test_20_encode.py
--rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-07-19 22:19:20.000000 cacholote-0.3.4/tests/test_30_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-07-19 22:19:20.000000 cacholote-0.3.4/tests/test_40_xarray_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-07-19 22:19:20.000000 cacholote-0.3.4/tests/test_50_io_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7251 2023-07-19 22:19:20.000000 cacholote-0.3.4/tests/test_60_clean.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:03:57.540683 cacholote-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-21 08:03:37.000000 cacholote-0.4.0/.cruft.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:03:57.532683 cacholote-0.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:03:57.536683 cacholote-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-07-21 08:03:37.000000 cacholote-0.4.0/.github/workflows/on-push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     8802 2023-07-21 08:03:37.000000 cacholote-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-21 08:03:37.000000 cacholote-0.4.0/.pre-commit-config-cruft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-21 08:03:37.000000 cacholote-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-21 08:03:37.000000 cacholote-0.4.0/DESIGN.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-21 08:03:37.000000 cacholote-0.4.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-07-21 08:03:37.000000 cacholote-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-21 08:03:37.000000 cacholote-0.4.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-21 08:03:37.000000 cacholote-0.4.0/OBJECT-STORAGE-DESIGN.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15708 2023-07-21 08:03:57.540683 cacholote-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-21 08:03:37.000000 cacholote-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:03:57.536683 cacholote-0.4.0/cacholote/
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-07-21 08:03:37.000000 cacholote-0.4.0/cacholote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-07-21 08:03:37.000000 cacholote-0.4.0/cacholote/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10248 2023-07-21 08:03:37.000000 cacholote-0.4.0/cacholote/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-07-21 08:03:37.000000 cacholote-0.4.0/cacholote/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-21 08:03:37.000000 cacholote-0.4.0/cacholote/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-07-21 08:03:37.000000 cacholote-0.4.0/cacholote/decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-07-21 08:03:37.000000 cacholote-0.4.0/cacholote/encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12807 2023-07-21 08:03:37.000000 cacholote-0.4.0/cacholote/extra_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 08:03:37.000000 cacholote-0.4.0/cacholote/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-07-21 08:03:37.000000 cacholote-0.4.0/cacholote/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-21 08:03:57.000000 cacholote-0.4.0/cacholote/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:03:57.536683 cacholote-0.4.0/cacholote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15708 2023-07-21 08:03:57.000000 cacholote-0.4.0/cacholote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-21 08:03:57.000000 cacholote-0.4.0/cacholote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 08:03:57.000000 cacholote-0.4.0/cacholote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-21 08:03:57.000000 cacholote-0.4.0/cacholote.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-21 08:03:57.000000 cacholote-0.4.0/cacholote.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:03:57.536683 cacholote-0.4.0/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-21 08:03:37.000000 cacholote-0.4.0/ci/environment-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-21 08:03:37.000000 cacholote-0.4.0/ci/environment-integration.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:03:57.540683 cacholote-0.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-21 08:03:37.000000 cacholote-0.4.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:03:57.540683 cacholote-0.4.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 08:03:37.000000 cacholote-0.4.0/docs/_static/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:03:57.540683 cacholote-0.4.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 08:03:37.000000 cacholote-0.4.0/docs/_templates/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-21 08:03:37.000000 cacholote-0.4.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-21 08:03:37.000000 cacholote-0.4.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-21 08:03:37.000000 cacholote-0.4.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-21 08:03:37.000000 cacholote-0.4.0/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-21 08:03:37.000000 cacholote-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 08:03:57.540683 cacholote-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:03:57.540683 cacholote-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-07-21 08:03:37.000000 cacholote-0.4.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-21 08:03:37.000000 cacholote-0.4.0/tests/test_00_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-07-21 08:03:37.000000 cacholote-0.4.0/tests/test_01_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-21 08:03:37.000000 cacholote-0.4.0/tests/test_02_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-21 08:03:37.000000 cacholote-0.4.0/tests/test_10_decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-07-21 08:03:37.000000 cacholote-0.4.0/tests/test_20_encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-07-21 08:03:37.000000 cacholote-0.4.0/tests/test_30_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-07-21 08:03:37.000000 cacholote-0.4.0/tests/test_40_xarray_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-07-21 08:03:37.000000 cacholote-0.4.0/tests/test_50_io_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7251 2023-07-21 08:03:37.000000 cacholote-0.4.0/tests/test_60_clean.py
```

### Comparing `cacholote-0.3.4/.cruft.json` & `cacholote-0.4.0/.cruft.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'commit'": "'8a346c4ecd7ada4447ab9c224fe3a8b17a79f540'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "checkout": null,
-    "commit": "9627920059b31038e1bb8a978921806cb835fde7",
+    "commit": "8a346c4ecd7ada4447ab9c224fe3a8b17a79f540",
     "context": {
         "cookiecutter": {
             "_template": "https://github.com/ecmwf-projects/cookiecutter-conda-package",
             "copyright_holder": "B-Open Solutions srl",
             "copyright_year": "2019",
             "integration_tests": "True",
             "mypy_strict": "True",
```

### Comparing `cacholote-0.3.4/.github/workflows/on-push.yml` & `cacholote-0.4.0/.github/workflows/on-push.yml`

 * *Files identical despite different names*

### Comparing `cacholote-0.3.4/.gitignore` & `cacholote-0.4.0/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # setuptools-scm
 version.py
 
 # Sphinx automatic generation of API
 docs/_api/
 
+# Combined environments
+ci/combined-environment-*.yml
+
 # Created by https://www.toptal.com/developers/gitignore/api/python,jupyternotebooks,vim,visualstudiocode,pycharm,emacs,linux,macos,windows
 # Edit at https://www.toptal.com/developers/gitignore?templates=python,jupyternotebooks,vim,visualstudiocode,pycharm,emacs,linux,macos,windows
 
 ### Emacs ###
 # -*- mode: gitignore; -*-
 *~
 \#*\#
```

### Comparing `cacholote-0.3.4/.pre-commit-config.yaml` & `cacholote-0.4.0/.pre-commit-config.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -7,31 +7,35 @@
   - id: check-json
   - id: check-yaml
   - id: check-toml
   - id: check-added-large-files
   - id: debug-statements
   - id: mixed-line-ending
 - repo: https://github.com/psf/black
-  rev: 23.3.0
+  rev: 23.7.0
   hooks:
   - id: black
 - repo: https://github.com/keewis/blackdoc
   rev: v0.3.8
   hooks:
   - id: blackdoc
     additional_dependencies: [black==22.3.0]
 - repo: https://github.com/astral-sh/ruff-pre-commit
-  rev: v0.0.277
+  rev: v0.0.278
   hooks:
   - id: ruff
     args: [--fix, --show-fixes]
 - repo: https://github.com/executablebooks/mdformat
   rev: 0.7.16
   hooks:
   - id: mdformat
 - repo: https://github.com/macisamuele/language-formatters-pre-commit-hooks
-  rev: v2.9.0
+  rev: v2.10.0
   hooks:
   - id: pretty-format-yaml
     args: [--autofix, --preserve-quotes]
   - id: pretty-format-toml
     args: [--autofix]
+- repo: https://github.com/gitleaks/gitleaks
+  rev: v8.17.0
+  hooks:
+  - id: gitleaks
```

### Comparing `cacholote-0.3.4/DESIGN.rst` & `cacholote-0.4.0/DESIGN.rst`

 * *Files identical despite different names*

### Comparing `cacholote-0.3.4/LICENSE` & `cacholote-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cacholote-0.3.4/Makefile` & `cacholote-0.4.0/Makefile`

 * *Files 17% similar despite different names*

```diff
@@ -11,16 +11,17 @@
 unit-tests:
 	python -m pytest -vv --cov=. --cov-report=$(COV_REPORT) --doctest-glob="*.md" --doctest-glob="*.rst"
 
 type-check:
 	python -m mypy .
 
 conda-env-update:
-	$(CONDA) env update $(CONDAFLAGS) -f ci/environment-ci.yml
-	$(CONDA) env update $(CONDAFLAGS) -f environment.yml
+	$(CONDA) install -y -c conda-forge conda-merge
+	$(CONDA) run conda-merge environment.yml ci/environment-ci.yml > ci/combined-environment-ci.yml
+	$(CONDA) env update $(CONDAFLAGS) -f ci/combined-environment-ci.yml
 
 docker-build:
 	docker build -t $(PROJECT) .
 
 docker-run:
 	docker run --rm -ti -v $(PWD):/srv $(PROJECT)
```

### Comparing `cacholote-0.3.4/OBJECT-STORAGE-DESIGN.rst` & `cacholote-0.4.0/OBJECT-STORAGE-DESIGN.rst`

 * *Files identical despite different names*

### Comparing `cacholote-0.3.4/PKG-INFO` & `cacholote-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cacholote
-Version: 0.3.4
+Version: 0.4.0
 Summary: Efficiently cache calls to functions
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `cacholote-0.3.4/README.md` & `cacholote-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `cacholote-0.3.4/cacholote/__init__.py` & `cacholote-0.4.0/cacholote/__init__.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.3.4/cacholote/cache.py` & `cacholote-0.4.0/cacholote/cache.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.3.4/cacholote/clean.py` & `cacholote-0.4.0/cacholote/clean.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.3.4/cacholote/config.py` & `cacholote-0.4.0/cacholote/config.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.3.4/cacholote/database.py` & `cacholote-0.4.0/cacholote/database.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.3.4/cacholote/decode.py` & `cacholote-0.4.0/cacholote/decode.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.3.4/cacholote/encode.py` & `cacholote-0.4.0/cacholote/encode.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.3.4/cacholote/extra_encoders.py` & `cacholote-0.4.0/cacholote/extra_encoders.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.3.4/cacholote/utils.py` & `cacholote-0.4.0/cacholote/utils.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.3.4/cacholote.egg-info/PKG-INFO` & `cacholote-0.4.0/cacholote.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cacholote
-Version: 0.3.4
+Version: 0.4.0
 Summary: Efficiently cache calls to functions
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `cacholote-0.3.4/cacholote.egg-info/SOURCES.txt` & `cacholote-0.4.0/cacholote.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cacholote-0.3.4/docs/Makefile` & `cacholote-0.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cacholote-0.3.4/docs/conf.py` & `cacholote-0.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.3.4/docs/make.bat` & `cacholote-0.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cacholote-0.3.4/pyproject.toml` & `cacholote-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cacholote-0.3.4/tests/conftest.py` & `cacholote-0.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.3.4/tests/test_01_settings.py` & `cacholote-0.4.0/tests/test_01_settings.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.3.4/tests/test_02_utils.py` & `cacholote-0.4.0/tests/test_02_utils.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.3.4/tests/test_10_decode.py` & `cacholote-0.4.0/tests/test_10_decode.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.3.4/tests/test_20_encode.py` & `cacholote-0.4.0/tests/test_20_encode.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.3.4/tests/test_30_cache.py` & `cacholote-0.4.0/tests/test_30_cache.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.3.4/tests/test_40_xarray_encoder.py` & `cacholote-0.4.0/tests/test_40_xarray_encoder.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.3.4/tests/test_50_io_encoder.py` & `cacholote-0.4.0/tests/test_50_io_encoder.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.3.4/tests/test_60_clean.py` & `cacholote-0.4.0/tests/test_60_clean.py`

 * *Files identical despite different names*

