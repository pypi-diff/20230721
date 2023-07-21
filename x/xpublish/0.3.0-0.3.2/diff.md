# Comparing `tmp/xpublish-0.3.0.tar.gz` & `tmp/xpublish-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xpublish-0.3.0.tar", last modified: Thu May 11 14:29:36 2023, max compression
+gzip compressed data, was "xpublish-0.3.2.tar", last modified: Fri Jul 21 16:05:15 2023, max compression
```

## Comparing `xpublish-0.3.0.tar` & `xpublish-0.3.2.tar`

### file list

```diff
@@ -1,98 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:29:36.397112 xpublish-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:29:36.389112 xpublish-0.3.0/.binder/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-11 14:29:19.000000 xpublish-0.3.0/.binder/dask_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-11 14:29:19.000000 xpublish-0.3.0/.binder/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-11 14:29:19.000000 xpublish-0.3.0/.binder/postBuild
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-11 14:29:19.000000 xpublish-0.3.0/.binder/start
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-11 14:29:19.000000 xpublish-0.3.0/.binder/test.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-11 14:29:19.000000 xpublish-0.3.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:29:36.389112 xpublish-0.3.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-11 14:29:19.000000 xpublish-0.3.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:29:36.389112 xpublish-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-05-11 14:29:19.000000 xpublish-0.3.0/.github/workflows/main.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-11 14:29:19.000000 xpublish-0.3.0/.github/workflows/pypipublish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-05-11 14:29:19.000000 xpublish-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-11 14:29:19.000000 xpublish-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-11 14:29:19.000000 xpublish-0.3.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11378 2023-05-11 14:29:19.000000 xpublish-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-05-11 14:29:36.397112 xpublish-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-05-11 14:29:19.000000 xpublish-0.3.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-11 14:29:19.000000 xpublish-0.3.0/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-11 14:29:19.000000 xpublish-0.3.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:29:36.389112 xpublish-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-05-11 14:29:19.000000 xpublish-0.3.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-05-11 14:29:19.000000 xpublish-0.3.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-11 14:29:19.000000 xpublish-0.3.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:29:36.389112 xpublish-0.3.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-05-11 14:29:19.000000 xpublish-0.3.0/docs/source/api.md
--rw-r--r--   0 runner    (1001) docker     (123)     9640 2023-05-11 14:29:19.000000 xpublish-0.3.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-05-11 14:29:19.000000 xpublish-0.3.0/docs/source/contributing.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:29:36.389112 xpublish-0.3.0/docs/source/ecosystem/
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-11 14:29:19.000000 xpublish-0.3.0/docs/source/ecosystem/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:29:36.389112 xpublish-0.3.0/docs/source/getting-started/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-11 14:29:19.000000 xpublish-0.3.0/docs/source/getting-started/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-11 14:29:19.000000 xpublish-0.3.0/docs/source/getting-started/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:29:36.393112 xpublish-0.3.0/docs/source/getting-started/tutorial/
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-11 14:29:19.000000 xpublish-0.3.0/docs/source/getting-started/tutorial/dataset-provider-plugin.md
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-11 14:29:19.000000 xpublish-0.3.0/docs/source/getting-started/tutorial/dataset-provider-plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-05-11 14:29:19.000000 xpublish-0.3.0/docs/source/getting-started/tutorial/dataset-router-plugin.md
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-11 14:29:19.000000 xpublish-0.3.0/docs/source/getting-started/tutorial/dataset-router-plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-05-11 14:29:19.000000 xpublish-0.3.0/docs/source/getting-started/tutorial/dataset-router.md
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-11 14:29:19.000000 xpublish-0.3.0/docs/source/getting-started/tutorial/dataset-router.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-11 14:29:19.000000 xpublish-0.3.0/docs/source/getting-started/tutorial/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-05-11 14:29:19.000000 xpublish-0.3.0/docs/source/getting-started/tutorial/introduction.md
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-11 14:29:19.000000 xpublish-0.3.0/docs/source/getting-started/tutorial/serving-multiple-datasets.md
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-11 14:29:19.000000 xpublish-0.3.0/docs/source/getting-started/tutorial/using-plugins.md
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-05-11 14:29:19.000000 xpublish-0.3.0/docs/source/getting-started/why-xpublish.md
--rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-05-11 14:29:19.000000 xpublish-0.3.0/docs/source/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:29:36.393112 xpublish-0.3.0/docs/source/user-guide/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:29:36.393112 xpublish-0.3.0/docs/source/user-guide/deployment/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-11 14:29:19.000000 xpublish-0.3.0/docs/source/user-guide/deployment/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-11 14:29:19.000000 xpublish-0.3.0/docs/source/user-guide/index.md
--rw-r--r--   0 runner    (1001) docker     (123)    10733 2023-05-11 14:29:19.000000 xpublish-0.3.0/docs/source/user-guide/plugins.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:29:36.393112 xpublish-0.3.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-05-11 14:29:19.000000 xpublish-0.3.0/examples/open_dataset.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-11 14:29:19.000000 xpublish-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-11 14:29:19.000000 xpublish-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 14:29:36.397112 xpublish-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-11 14:29:19.000000 xpublish-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:29:36.393112 xpublish-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 14:29:19.000000 xpublish-0.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-11 14:29:19.000000 xpublish-0.3.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-05-11 14:29:19.000000 xpublish-0.3.0/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-11 14:29:19.000000 xpublish-0.3.0/tests/test_fsspec_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-05-11 14:29:19.000000 xpublish-0.3.0/tests/test_plugin_management.py
--rw-r--r--   0 runner    (1001) docker     (123)    12257 2023-05-11 14:29:19.000000 xpublish-0.3.0/tests/test_rest_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-05-11 14:29:19.000000 xpublish-0.3.0/tests/test_zarr_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-05-11 14:29:19.000000 xpublish-0.3.0/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:29:36.393112 xpublish-0.3.0/xpublish/
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-11 14:29:19.000000 xpublish-0.3.0/xpublish/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-05-11 14:29:19.000000 xpublish-0.3.0/xpublish/accessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-05-11 14:29:19.000000 xpublish-0.3.0/xpublish/dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:29:36.393112 xpublish-0.3.0/xpublish/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-11 14:29:19.000000 xpublish-0.3.0/xpublish/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-05-11 14:29:19.000000 xpublish-0.3.0/xpublish/plugins/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:29:36.393112 xpublish-0.3.0/xpublish/plugins/included/
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-11 14:29:19.000000 xpublish-0.3.0/xpublish/plugins/included/dataset_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-11 14:29:19.000000 xpublish-0.3.0/xpublish/plugins/included/module_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-11 14:29:19.000000 xpublish-0.3.0/xpublish/plugins/included/plugin_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-05-11 14:29:19.000000 xpublish-0.3.0/xpublish/plugins/included/zarr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-11 14:29:19.000000 xpublish-0.3.0/xpublish/plugins/manage.py
--rw-r--r--   0 runner    (1001) docker     (123)    13303 2023-05-11 14:29:19.000000 xpublish-0.3.0/xpublish/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:29:36.393112 xpublish-0.3.0/xpublish/routers/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-11 14:29:19.000000 xpublish-0.3.0/xpublish/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-11 14:29:19.000000 xpublish-0.3.0/xpublish/routers/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:29:36.397112 xpublish-0.3.0/xpublish/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 14:29:19.000000 xpublish-0.3.0/xpublish/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-05-11 14:29:19.000000 xpublish-0.3.0/xpublish/utils/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-11 14:29:19.000000 xpublish-0.3.0/xpublish/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-11 14:29:19.000000 xpublish-0.3.0/xpublish/utils/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-05-11 14:29:19.000000 xpublish-0.3.0/xpublish/utils/zarr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:29:36.393112 xpublish-0.3.0/xpublish.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-05-11 14:29:36.000000 xpublish-0.3.0/xpublish.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-05-11 14:29:36.000000 xpublish-0.3.0/xpublish.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 14:29:36.000000 xpublish-0.3.0/xpublish.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-11 14:29:36.000000 xpublish-0.3.0/xpublish.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 14:29:36.000000 xpublish-0.3.0/xpublish.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-11 14:29:36.000000 xpublish-0.3.0/xpublish.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-11 14:29:36.000000 xpublish-0.3.0/xpublish.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:05:15.119820 xpublish-0.3.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:05:15.111820 xpublish-0.3.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-21 16:05:03.000000 xpublish-0.3.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:05:15.111820 xpublish-0.3.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-07-21 16:05:03.000000 xpublish-0.3.2/.github/workflows/main.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-21 16:05:03.000000 xpublish-0.3.2/.github/workflows/pypipublish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11378 2023-07-21 16:05:03.000000 xpublish-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-21 16:05:03.000000 xpublish-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17019 2023-07-21 16:05:15.119820 xpublish-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-07-21 16:05:03.000000 xpublish-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-21 16:05:03.000000 xpublish-0.3.2/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-07-21 16:05:03.000000 xpublish-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-21 16:05:03.000000 xpublish-0.3.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 16:05:15.119820 xpublish-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:05:15.115821 xpublish-0.3.2/xpublish/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-21 16:05:03.000000 xpublish-0.3.2/xpublish/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-07-21 16:05:03.000000 xpublish-0.3.2/xpublish/accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-07-21 16:05:03.000000 xpublish-0.3.2/xpublish/dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:05:15.115821 xpublish-0.3.2/xpublish/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-21 16:05:03.000000 xpublish-0.3.2/xpublish/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-07-21 16:05:03.000000 xpublish-0.3.2/xpublish/plugins/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:05:15.115821 xpublish-0.3.2/xpublish/plugins/included/
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-07-21 16:05:03.000000 xpublish-0.3.2/xpublish/plugins/included/dataset_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-07-21 16:05:03.000000 xpublish-0.3.2/xpublish/plugins/included/module_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-21 16:05:03.000000 xpublish-0.3.2/xpublish/plugins/included/plugin_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-07-21 16:05:03.000000 xpublish-0.3.2/xpublish/plugins/included/zarr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-21 16:05:03.000000 xpublish-0.3.2/xpublish/plugins/manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13673 2023-07-21 16:05:03.000000 xpublish-0.3.2/xpublish/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:05:15.115821 xpublish-0.3.2/xpublish/routers/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-21 16:05:03.000000 xpublish-0.3.2/xpublish/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-21 16:05:03.000000 xpublish-0.3.2/xpublish/routers/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:05:15.119820 xpublish-0.3.2/xpublish/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:05:03.000000 xpublish-0.3.2/xpublish/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-07-21 16:05:03.000000 xpublish-0.3.2/xpublish/utils/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-21 16:05:03.000000 xpublish-0.3.2/xpublish/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-07-21 16:05:03.000000 xpublish-0.3.2/xpublish/utils/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-07-21 16:05:03.000000 xpublish-0.3.2/xpublish/utils/zarr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:05:15.119820 xpublish-0.3.2/xpublish.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-21 16:05:15.000000 xpublish-0.3.2/xpublish.egg-info/SOURCES.txt
```

### Comparing `xpublish-0.3.0/.github/workflows/main.yaml` & `xpublish-0.3.2/.github/workflows/main.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -4,72 +4,91 @@
   push:
     branches: "*"
   pull_request:
     branches: main
 
 jobs:
   test:
-    name: ${{ matrix.python-version }}-build
+    name: ${{ matrix.python-version }}-pydantic${{ matrix.pydantic-version }}-build
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.9", "3.10"]
+        python-version: ["3.9", "3.10", "3.11"]
+        pydantic-version: ["<2", ">=2"]
     steps:
       - uses: actions/checkout@v3
+
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
           architecture: x64
-      - uses: actions/cache@v3.3.1
+
+      - name: Setup pip cache
+        uses: actions/cache@v3.3.1
         with:
           path: ~/.cache/pip
-          key: ${{ runner.os }}-pip-${{ hashFiles('**/dev-requirements.txt') }}
+          key: ${{ runner.os }}-pip-${{ matrix.python-version }}-pydantic${{ matrix.pydantic-version }}-${{ hashFiles('**/dev-requirements.txt') }}
           restore-keys: |
-            ${{ runner.os }}-pip-
-      - run: |
+            ${{ runner.os }}-pip-${{ matrix.python-version }}-pydantic${{ matrix.pydantic-version }}
+            ${{ runner.os }}-pip-${{ matrix.python-version }}
+            ${{ runner.os }}-pip
+            ${{ runner.os }}-pip-dev
+
+      - name: Install dependencies
+        run: |
           python -m pip install -r dev-requirements.txt
           python -m pip install --no-deps -e .
+          python -m pip install "pydantic${{ matrix.pydantic-version }}"
           python -m pip list
+
       - name: Running Tests
         run: |
           python -m pytest --cov=./ --cov-report=xml --verbose
+
       - name: Upload coverage to Codecov
-        uses: codecov/codecov-action@v3.1.3
-        if: ${{ matrix.python-version }} == 3.9
+        uses: codecov/codecov-action@v3.1.4
         with:
           file: ./coverage.xml
           fail_ci_if_error: false
 
   test-upstream:
     name: ${{ matrix.python-version }}-dev-build
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.9", "3.10"]
+        python-version: ["3.9", "3.10", "3.11"]
     steps:
       - uses: actions/checkout@v3
+
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
           architecture: x64
-      - uses: actions/cache@v3.3.1
+
+      - name: Setup pip cache
+        uses: actions/cache@v3.3.1
         with:
           path: ~/.cache/pip
-          key: ${{ runner.os }}-pip-${{ hashFiles('**/dev-requirements.txt') }}
+          key: ${{ runner.os }}-pip-dev-${{ matrix.python-version }}-${{ hashFiles('**/dev-requirements.txt') }}
           restore-keys: |
-            ${{ runner.os }}-pip-
-      - run: |
+            ${{ runner.os }}-pip-dev-${{ matrix.python-version }}
+            ${{ runner.os }}-pip-dev
+            ${{ runner.os }}-pip
+
+      - name: Install dev dependencies
+        run: |
           python -m pip install -r dev-requirements.txt
           python -m pip install --no-deps --upgrade \
                 git+https://github.com/dask/dask \
                 git+https://github.com/dask/cachey \
                 git+https://github.com/zarr-developers/zarr \
                 git+https://github.com/pydata/xarray \
                 git+https://github.com/tiangolo/fastapi \
                 git+https://github.com/encode/uvicorn
           python -m pip install --no-deps -e .
           python -m pip list
+
       - name: Running Tests
         run: |
           python -m pytest --verbose
```

### Comparing `xpublish-0.3.0/LICENSE` & `xpublish-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xpublish-0.3.0/README.rst` & `xpublish-0.3.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,77 +1,78 @@
-Xpublish
-========
+# Xpublish
 
-Publish Xarray Datasets via a REST API.
+Publish Xarray Datasets to the web
 
-.. image:: https://github.com/xpublish-community/xpublish/actions/workflows/main.yaml/badge.svg
-   :target: https://github.com/xpublish-community/xpublish/actions/workflows/main.yaml
-   :alt: GitHub Workflow Status
+<!-- badges-start -->
 
-.. image:: https://readthedocs.org/projects/xpublish/badge/?version=latest
-   :target: https://xpublish.readthedocs.io/en/latest/?badge=latest
-   :alt: Documentation Status
+[![PyPI](https://img.shields.io/pypi/v/xpublish)](https://pypi.org/project/xpublish/)
+[![Conda](https://img.shields.io/conda/v/conda-forge/xpublish)](https://anaconda.org/conda-forge/xpublish)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/xpublish)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/xpublish-community/xpublish/main)
 
-.. image:: https://mybinder.org/badge_logo.svg
-   :target: https://mybinder.org/v2/gh/xarray-contrib/xpublish/main
-   :alt: Binder
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/xpublish-community/xpublish/main.yaml?logo=github)](https://github.com/xpublish-community/xpublish/actions/workflows/main.yaml)
+[![Documentation Status](https://readthedocs.org/projects/xpublish/badge/?version=latest)](https://xpublish.readthedocs.io/en/latest/?badge=latest)
+[![](https://codecov.io/gh/xpublish-community/xpublish/branch/main/graph/badge.svg)](https://codecov.io/gh/xpublish-community/xpublish)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/xpublish-community/xpublish/main.svg)](https://results.pre-commit.ci/latest/github/xpublish-community/xpublish/main)
 
-.. image:: https://codecov.io/gh/xarray-contrib/xpublish/branch/main/graph/badge.svg
-   :target: https://codecov.io/gh/xarray-contrib/xpublish
+<!-- badges-end -->
 
-.. image:: https://results.pre-commit.ci/badge/github/xpublish-community/xpublish/main.svg
-   :target: https://results.pre-commit.ci/latest/github/xpublish-community/xpublish/main
-   :alt: pre-commit.ci status
+## A quick example
 
 **Serverside: Publish a Xarray Dataset through a rest API**
 
-.. code-block:: python
+<!-- server-example-start -->
 
-   ds.rest.serve(host="0.0.0.0", port=9000)
+```python
+ds.rest.serve(host="0.0.0.0", port=9000)
+```
 
+<!-- server-example-end -->
 
 **Client-side: Connect to a published dataset**
 
-The published dataset can be accessed from various kinds of client applications.
-Here is an example of directly accessing the data from within Python:
+<!-- client-example-start -->
 
-.. code-block:: python
+The published datasets can be accessed from various kinds of client applications, e.g., from within Python using Zarr and fsspec.
 
-   import xarray as xr
-   import zarr
-   from fsspec.implementations.http import HTTPFileSystem
+```python
+import xarray as xr
+import zarr
+from fsspec.implementations.http import HTTPFileSystem
 
-   fs = HTTPFileSystem()
-   http_map = fs.get_mapper("http://0.0.0.0:9000")
+fs = HTTPFileSystem()
+http_map = fs.get_mapper("http://0.0.0.0:9000/zarr/")
 
-   # open as a zarr group
-   zg = zarr.open_consolidated(http_map, mode="r")
+# open as a zarr group
+zg = zarr.open_consolidated(http_map, mode="r")
 
-   # or open as another Xarray Dataset
-   ds = xr.open_zarr(http_map, consolidated=True)
+# or open as another Xarray Dataset
+ds = xr.open_zarr(http_map, consolidated=True)
+```
 
+Or to explore other access methods, open [http://0.0.0.0:9000/docs](http://0.0.0.0:9000/docs) in a browser.
 
-Why?
-^^^^
+<!-- client-example-end -->
+
+## Why?
 
 Xpublish lets you serve/share/publish Xarray Datasets via a web application.
 
-The data and/or metadata in the Xarray Datasets can be exposed in various forms
-through pluggable REST API endpoints. Efficient, on-demand delivery of large
-datasets may be enabled with Dask on the server-side.
+The data and/or metadata in the Xarray Datasets can be exposed in various forms through [pluggable REST API endpoints](https://xpublish.readthedocs.io/en/latest/user-guide/plugins.html).
+Efficient, on-demand delivery of large datasets may be enabled with Dask on the server-side.
 
-We are exploring applications of Xpublish that include:
+Xpublish's [plugin ecosystem](https://xpublish.readthedocs.io/en/latest/ecosystem/index.html#plugins) has capabilities including:
 
-* publish on-demand or derived data products
-* turning xarray objects into streaming services (e.g. OPeNDAP)
+- publish on-demand or derived data products
+- turning xarray objects into streaming services (e.g. OPeNDAP)
 
-How?
-^^^^
+## How?
 
 Under the hood, Xpublish is using a web app (FastAPI) that is exposing a
 REST-like API with builtin and/or user-defined endpoints.
 
-For example, Xpublish provides by default a minimal Zarr compatible REST-like
-API with the following endpoints:
+For example, Xpublish provides by default a minimal Zarr compatible REST-like API with the following endpoints:
+
+- `zarr/.zmetadata`: returns Zarr-formatted metadata keys as json strings.
+- `zarr/var/0.0.0`: returns a variable data chunk as a binary string.
 
-* ``.zmetadata``: returns Zarr-formatted metadata keys as json strings.
-* ``var/0.0.0``: returns a variable data chunk as a binary string.
+Futher endpoints can be added by installing or writing plugins.
```

### Comparing `xpublish-0.3.0/xpublish/accessor.py` & `xpublish-0.3.2/xpublish/accessor.py`

 * *Files identical despite different names*

### Comparing `xpublish-0.3.0/xpublish/dependencies.py` & `xpublish-0.3.2/xpublish/dependencies.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import cachey
 import pluggy
 import xarray as xr
 from fastapi import Depends
 
 from .utils.api import DATASET_ID_ATTR_KEY
-from .utils.zarr import create_zmetadata, create_zvariables, zarr_metadata_key
+from .utils.zarr import ZARR_METADATA_KEY, create_zmetadata, create_zvariables
 
 if TYPE_CHECKING:
     from .plugins import Plugin  # pragma: no cover
 
 
 def get_dataset_ids() -> List[str]:
     """FastAPI dependency for getting the list of ids (string keys)
@@ -86,15 +86,15 @@
 def get_zmetadata(
     dataset: xr.Dataset = Depends(get_dataset),
     cache: cachey.Cache = Depends(get_cache),
     zvariables: dict = Depends(get_zvariables),
 ):
     """FastAPI dependency that returns a consolidated zmetadata dictionary."""
 
-    cache_key = dataset.attrs.get(DATASET_ID_ATTR_KEY, '') + '/' + zarr_metadata_key
+    cache_key = dataset.attrs.get(DATASET_ID_ATTR_KEY, '') + '/' + ZARR_METADATA_KEY
     zmeta = cache.get(cache_key)
 
     if zmeta is None:
         zmeta = create_zmetadata(dataset)
 
         # we want to permanently cache this: set high cost value
         cache.put(cache_key, zmeta, 99999)
```

### Comparing `xpublish-0.3.0/xpublish/plugins/hooks.py` & `xpublish-0.3.2/xpublish/plugins/hooks.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,27 +22,32 @@
     Some routers may be 'borrowed' by other routers to expose different
     geometries of data, thus the default dependencies may need to be overridden.
     By depending on the passed in version of this class, the dependencies
     can be overridden predictably.
     """
 
     dataset_ids: Callable[..., List[str]] = Field(
-        get_dataset_ids, description='Returns a list of all valid dataset ids'
+        get_dataset_ids,
+        description='Returns a list of all valid dataset ids',
     )
     dataset: Callable[[str], xr.Dataset] = Field(
-        get_dataset, description='Returns a dataset using ``/<dataset_id>/`` in the path.'
+        get_dataset,
+        description='Returns a dataset using ``/<dataset_id>/`` in the path.',
     )
     cache: Callable[..., cachey.Cache] = Field(
-        get_cache, description='Provide access to :py:class:`cachey.Cache`'
+        get_cache,
+        description='Provide access to :py:class:`cachey.Cache`',
     )
     plugins: Callable[..., Dict[str, 'Plugin']] = Field(
-        get_plugins, description='A dictionary of plugins allowing direct access'
+        get_plugins,
+        description='A dictionary of plugins allowing direct access',
     )
     plugin_manager: Callable[..., pluggy.PluginManager] = Field(
-        get_plugin_manager, description='The plugin manager itself, allowing for maximum creativity'
+        get_plugin_manager,
+        description='The plugin manager itself, allowing for maximum creativity',
     )
 
     def __hash__(self):
         """Dependency functions aren't easy to hash"""
         return 0  # pragma: no cover
 
 
@@ -60,15 +65,21 @@
 
     name: str = Field(..., description='Fallback name of plugin')
 
     def __hash__(self):
         """Make sure that the plugin is hashable to load with pluggy"""
         things_to_hash = []
 
-        for e in self.dict():
+        # try/except is for pydantic backwards compatibility
+        try:
+            model_dict = self.model_dump()
+        except AttributeError:
+            model_dict = self.dict()
+
+        for e in model_dict:
             if isinstance(e, list):
                 things_to_hash.append(tuple(e))  # pragma: no cover
             else:
                 things_to_hash.append(e)
 
         return hash(tuple(things_to_hash))
 
@@ -111,15 +122,16 @@
         """
 
     @hookspec
     def get_datasets(self) -> Iterable[str]:  # type: ignore
         """Return an iterable of dataset ids that the plugin can provide"""
 
     @hookspec(firstresult=True)
-    def get_dataset(self, dataset_id: str) -> Optional[xr.Dataset]:  # type: ignore
+    # type: ignore
+    def get_dataset(self, dataset_id: str) -> Optional[xr.Dataset]:
         """Return a dataset by requested dataset_id.
 
         If the plugin does not have the dataset, return None
         """
 
     @hookspec
     def register_hookspec(self):  # type: ignore
```

### Comparing `xpublish-0.3.0/xpublish/plugins/included/dataset_info.py` & `xpublish-0.3.2/xpublish/plugins/included/dataset_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,63 +8,72 @@
 from xpublish.utils.api import JSONResponse
 
 from ...dependencies import get_zmetadata, get_zvariables
 from .. import Dependencies, Plugin, hookimpl
 
 
 class DatasetInfoPlugin(Plugin):
-    name = 'dataset_info'
+    """Dataset metadata"""
+
+    name: str = 'dataset_info'
 
     dataset_router_prefix: str = ''
-    dataset_router_tags: Sequence[str] = []
+    dataset_router_tags: Sequence[str] = ['dataset_info']
 
     @hookimpl
-    def dataset_router(self, deps: Dependencies):
-        router = APIRouter(prefix=self.dataset_router_prefix, tags=list(self.dataset_router_tags))
+    def dataset_router(self, deps: Dependencies) -> APIRouter:
+        router = APIRouter(
+            prefix=self.dataset_router_prefix,
+            tags=list(self.dataset_router_tags),
+        )
 
         @router.get('/')
         def html_representation(
             dataset=Depends(deps.dataset),
-        ):
-            """Returns a HTML representation of the dataset."""
+        ) -> HTMLResponse:
+            """Returns the xarray HTML representation of the dataset."""
 
             with xr.set_options(display_style='html'):
                 return HTMLResponse(dataset._repr_html_())
 
         @router.get('/keys')
         def list_keys(
             dataset=Depends(deps.dataset),
-        ):
+        ) -> list[str]:
+            """List of the keys in a dataset"""
+
             return JSONResponse(list(dataset.variables))
 
         @router.get('/dict')
         def to_dict(
             dataset=Depends(deps.dataset),
-        ):
+        ) -> dict:
+            """The full dataset as a dictionary"""
             return JSONResponse(dataset.to_dict(data=False))
 
         @router.get('/info')
         def info(
             dataset=Depends(deps.dataset),
             cache=Depends(deps.cache),
-        ):
+        ) -> dict:
             """Dataset schema (close to the NCO-JSON schema)."""
 
             zvariables = get_zvariables(dataset, cache)
             zmetadata = get_zmetadata(dataset, cache, zvariables)
 
             info = {}
             info['dimensions'] = dict(dataset.dims.items())
             info['variables'] = {}
 
             meta = zmetadata['metadata']
 
             for name, var in zvariables.items():
                 attrs = meta[f'{name}/{attrs_key}'].copy()
                 attrs.pop('_ARRAY_DIMENSIONS')
+
                 info['variables'][name] = {
                     'type': var.data.dtype.name,
                     'dimensions': list(var.dims),
                     'attributes': attrs,
                 }
 
             info['global_attributes'] = meta[attrs_key]
```

### Comparing `xpublish-0.3.0/xpublish/plugins/included/module_version.py` & `xpublish-0.3.2/xpublish/plugins/included/module_version.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 """
 Version information router
 """
 import importlib
 import sys
-from typing import List
+from typing import Sequence
 
 from fastapi import APIRouter
 
 from ...utils.info import get_sys_info, netcdf_and_hdf5_versions
 from .. import Plugin, hookimpl
 
 
 class ModuleVersionPlugin(Plugin):
-    name = 'module_version'
+    """Share the currently loaded versions of key libraries"""
+
+    name: str = 'module_version'
 
     app_router_prefix: str = ''
-    app_router_tags: List[str] = []
+    app_router_tags: Sequence[str] = ['module_version']
 
     @hookimpl
-    def app_router(self):
-        router = APIRouter(prefix=self.app_router_prefix, tags=self.app_router_tags)
+    def app_router(self) -> APIRouter:
+        router = APIRouter(
+            prefix=self.app_router_prefix,
+            tags=self.app_router_tags,
+        )
 
         @router.get('/versions')
-        def get_versions():
+        def get_versions() -> dict:
+            """Currently loaded versions of key libraries"""
             versions = dict(get_sys_info() + netcdf_and_hdf5_versions())
             modules = [
                 'xarray',
                 'zarr',
                 'numcodecs',
                 'fastapi',
                 'starlette',
```

### Comparing `xpublish-0.3.0/xpublish/plugins/included/plugin_info.py` & `xpublish-0.3.2/xpublish/plugins/included/plugin_info.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,42 +8,49 @@
 from pydantic import BaseModel
 
 from .. import Dependencies, Plugin, hookimpl
 
 
 class PluginInfo(BaseModel):
     path: str
-    version: Optional[str]
+    version: Optional[str] = None
 
 
 class PluginInfoPlugin(Plugin):
-    name = 'plugin_info'
+    """Expose plugin source and version"""
+
+    name: str = 'plugin_info'
 
     app_router_prefix: str = ''
-    app_router_tags: Sequence[str] = []
+    app_router_tags: Sequence[str] = ['plugin_info']
 
     @hookimpl
-    def app_router(self, deps: Dependencies):
-        router = APIRouter(prefix=self.app_router_prefix, tags=list(self.app_router_tags))
+    def app_router(self, deps: Dependencies) -> APIRouter:
+        router = APIRouter(
+            prefix=self.app_router_prefix,
+            tags=list(self.app_router_tags),
+        )
 
         @router.get('/plugins')
         def get_plugins(
             plugins: Dict[str, Plugin] = Depends(deps.plugins)
         ) -> Dict[str, PluginInfo]:
+            """Return the source and version of the currently loaded plugins"""
             plugin_info = {}
 
             for name, plugin in plugins.items():
                 plugin_type = type(plugin)
                 module_name = plugin_type.__module__.split('.')[0]
                 try:
                     mod = importlib.import_module(module_name)
                     version = getattr(mod, '__version__', None)
                 except ImportError:  # pragma: no cover
                     version = None  # pragma: no cover
 
                 plugin_info[name] = PluginInfo(
-                    path=f'{plugin_type.__module__}.{plugin.__repr_name__()}', version=version
+                    path=f'{plugin_type.__module__}.{plugin.__repr_name__()}',
+                    version=version,
                 )
 
             return plugin_info
 
         return router
```

### Comparing `xpublish-0.3.0/xpublish/plugins/included/zarr.py` & `xpublish-0.3.2/xpublish/plugins/included/zarr.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,75 +1,86 @@
 import logging
 from typing import Sequence
 
 import cachey  # type: ignore
 import xarray as xr
-from fastapi import APIRouter, Depends, HTTPException
+from fastapi import APIRouter, Depends, HTTPException, Path
 from starlette.responses import Response  # type: ignore
 from zarr.storage import array_meta_key, attrs_key, group_meta_key  # type: ignore
 
 from xpublish.utils.api import JSONResponse
 
 from ...dependencies import get_zmetadata, get_zvariables
 from ...utils.api import DATASET_ID_ATTR_KEY
 from ...utils.cache import CostTimer
-from ...utils.zarr import encode_chunk, get_data_chunk, jsonify_zmetadata, zarr_metadata_key
+from ...utils.zarr import (
+    ZARR_METADATA_KEY,
+    encode_chunk,
+    get_data_chunk,
+    jsonify_zmetadata,
+)
 from .. import Dependencies, Plugin, hookimpl
 
 logger = logging.getLogger('zarr_api')
 
 
 class ZarrPlugin(Plugin):
     """Adds Zarr-like accessing endpoints for datasets"""
 
-    name = 'zarr'
+    name: str = 'zarr'
 
     dataset_router_prefix: str = '/zarr'
     dataset_router_tags: Sequence[str] = ['zarr']
 
     @hookimpl
-    def dataset_router(self, deps: Dependencies):
-        router = APIRouter(prefix=self.dataset_router_prefix, tags=list(self.dataset_router_tags))
+    def dataset_router(self, deps: Dependencies) -> APIRouter:
+        router = APIRouter(
+            prefix=self.dataset_router_prefix,
+            tags=list(self.dataset_router_tags),
+        )
 
-        @router.get(f'/{zarr_metadata_key}')
+        @router.get(f'/{ZARR_METADATA_KEY}')
         def get_zarr_metadata(
             dataset=Depends(deps.dataset),
             cache=Depends(deps.cache),
-        ):
+        ) -> dict:
+            """Consolidated Zarr metadata"""
             zvariables = get_zvariables(dataset, cache)
             zmetadata = get_zmetadata(dataset, cache, zvariables)
 
             zjson = jsonify_zmetadata(dataset, zmetadata)
 
             return JSONResponse(zjson)
 
         @router.get(f'/{group_meta_key}')
         def get_zarr_group(
             dataset=Depends(deps.dataset),
             cache=Depends(deps.cache),
-        ):
+        ) -> dict:
+            """Zarr group data"""
             zvariables = get_zvariables(dataset, cache)
             zmetadata = get_zmetadata(dataset, cache, zvariables)
 
             return JSONResponse(zmetadata['metadata'][group_meta_key])
 
         @router.get(f'/{attrs_key}')
         def get_zarr_attrs(
             dataset=Depends(deps.dataset),
             cache=Depends(deps.cache),
-        ):
+        ) -> dict:
+            """Zarr attributes"""
             zvariables = get_zvariables(dataset, cache)
             zmetadata = get_zmetadata(dataset, cache, zvariables)
 
             return JSONResponse(zmetadata['metadata'][attrs_key])
 
         @router.get('/{var}/{chunk}')
         def get_variable_chunk(
-            var: str,
-            chunk: str,
+            var: str = Path(description='Variable in dataset'),
+            chunk: str = Path(description='Zarr chunk'),
             dataset: xr.Dataset = Depends(deps.dataset),
             cache: cachey.Cache = Depends(deps.cache),
         ):
             """Get a zarr array chunk.
 
             This will return cached responses when available.
 
@@ -92,22 +103,29 @@
                 response = cache.get(cache_key)
 
                 if response is None:
                     with CostTimer() as ct:
                         arr_meta = zmetadata['metadata'][f'{var}/{array_meta_key}']
                         da = zvariables[var].data
 
-                        data_chunk = get_data_chunk(da, chunk, out_shape=arr_meta['chunks'])
+                        data_chunk = get_data_chunk(
+                            da,
+                            chunk,
+                            out_shape=arr_meta['chunks'],
+                        )
 
                         echunk = encode_chunk(
                             data_chunk.tobytes(),
                             filters=arr_meta['filters'],
                             compressor=arr_meta['compressor'],
                         )
 
-                        response = Response(echunk, media_type='application/octet-stream')
+                        response = Response(
+                            echunk,
+                            media_type='application/octet-stream',
+                        )
 
                     cache.put(cache_key, response, ct.time, len(echunk))
 
                 return response
 
         return router
```

### Comparing `xpublish-0.3.0/xpublish/plugins/manage.py` & `xpublish-0.3.2/xpublish/plugins/manage.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,26 +21,29 @@
     for entry_point in entry_points()['xpublish.plugin']:
         if entry_point.name not in exclude_plugins:
             plugins[entry_point.name] = entry_point.load()
 
     return plugins
 
 
-def load_default_plugins(exclude_plugins: Optional[Iterable[str]] = None) -> Dict[str, Plugin]:
+def load_default_plugins(
+    exclude_plugins: Optional[Iterable[str]] = None,
+) -> Dict[str, Plugin]:
     """Find and initialize plugins from entry point group `xpublish.plugin`"""
     initialized_plugins: Dict[str, Plugin] = {}
 
     for name, plugin in find_default_plugins(exclude_plugins=exclude_plugins).items():
         initialized_plugins[name] = plugin()
 
     return initialized_plugins
 
 
 def configure_plugins(
-    plugins: Dict[str, Type[Plugin]], plugin_configs: Optional[Dict] = None
+    plugins: Dict[str, Type[Plugin]],
+    plugin_configs: Optional[Dict] = None,
 ) -> Dict[str, Plugin]:
     """Initialize and configure plugins with given dictionary of configurations"""
     initialized_plugins: Dict[str, Plugin] = {}
     plugin_configs = plugin_configs or {}
 
     for name, plugin in plugins.items():
         kwargs = plugin_configs.get(name, {})
```

### Comparing `xpublish-0.3.0/xpublish/rest.py` & `xpublish-0.3.2/xpublish/rest.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Dict, List, Optional, Tuple
 
 import cachey
 import pluggy
 import uvicorn
 import xarray as xr
-from fastapi import APIRouter, FastAPI, HTTPException
+from fastapi import APIRouter, FastAPI, HTTPException, Path
 
 from .dependencies import get_cache, get_dataset, get_dataset_ids, get_plugin_manager
 from .plugins import Dependencies, Plugin, PluginSpec, get_plugins, load_default_plugins
 from .routers import dataset_collection_router
 from .utils.api import (
     SingleDatasetOpenAPIOverrider,
     check_route_conflicts,
@@ -78,15 +78,18 @@
             raise TypeError(
                 'xpublish.Rest no longer directly handles single datasets. Please use xpublish.SingleDatasetRest instead'
             )
 
         self.setup_datasets(datasets or {})
         self.setup_plugins(plugins)
 
-        routers = normalize_app_routers(routers or [], self._dataset_route_prefix)
+        routers = normalize_app_routers(
+            routers or [],
+            self._dataset_route_prefix,
+        )
         check_route_conflicts(routers)
         self._routers = routers
 
         self.init_app_kwargs(app_kws)
         self.init_cache_kwargs(cache_kws)
 
     def setup_datasets(self, datasets: Dict[str, xr.Dataset]) -> str:
@@ -114,15 +117,18 @@
         dataset_ids = list(self._datasets)
 
         for plugin_dataset_ids in self.pm.hook.get_datasets():
             dataset_ids.extend(plugin_dataset_ids)
 
         return dataset_ids
 
-    def get_dataset_from_plugins(self, dataset_id: str) -> xr.Dataset:
+    def get_dataset_from_plugins(
+        self,
+        dataset_id: str = Path(description='Unique ID of dataset'),
+    ) -> xr.Dataset:
         """Attempt to load dataset from plugins, otherwise return dataset from passed in dictionary of datasets
 
         Parameters:
             dataset_id:
                 Unique key of dataset to attempt to load from plugins or
                 those provided to :class:`xpublish.Rest` at initialization.
 
@@ -138,15 +144,18 @@
             return dataset
 
         if dataset_id not in self._datasets:
             raise HTTPException(status_code=404, detail=f"Dataset '{dataset_id}' not found")
 
         return self._datasets[dataset_id]
 
-    def setup_plugins(self, plugins: Optional[Dict[str, Plugin]] = None):
+    def setup_plugins(
+        self,
+        plugins: Optional[Dict[str, Plugin]] = None,
+    ) -> None:
         """Initialize and load plugins from entry_points unless explicitly provided
 
         Parameters:
             plugins:
                 If a dictionary of initialized plugins is provided,
                 then the automatic loading of plugins is disabled.
 
@@ -162,16 +171,19 @@
         for name, plugin in plugins.items():
             self.pm.register(plugin, name=name)
 
         for hookspec in self.pm.hook.register_hookspec():
             self.pm.add_hookspecs(hookspec)
 
     def register_plugin(
-        self, plugin: Plugin, plugin_name: Optional[str] = None, overwrite: bool = False
-    ):
+        self,
+        plugin: Plugin,
+        plugin_name: Optional[str] = None,
+        overwrite: bool = False,
+    ) -> None:
         """
         Register a plugin with the xpublish system
 
         Args:
             plugin: Instantiated Plugin object
             plugin_name: Plugin name
             overwrite: If a plugin of the same name exist,
@@ -200,22 +212,22 @@
             ) from e
 
         for hookspec in self.pm.subset_hook_caller(
             'register_hookspec', remove_plugins=existing_plugins
         )():
             self.pm.add_hookspecs(hookspec)
 
-    def init_cache_kwargs(self, cache_kws):
+    def init_cache_kwargs(self, cache_kws: dict) -> None:
         """Set up cache kwargs"""
         self._cache = None
         self._cache_kws = {'available_bytes': 1e6}
         if cache_kws is not None:
             self._cache_kws.update(cache_kws)
 
-    def init_app_kwargs(self, app_kws):
+    def init_app_kwargs(self, app_kws: dict) -> None:
         """Set up FastAPI application kwargs"""
         self._app = None
         self._app_kws = {}
         if app_kws is not None:
             self._app_kws.update(app_kws)
 
     @property
@@ -227,15 +239,15 @@
         return self._cache
 
     @property
     def plugins(self) -> Dict[str, Plugin]:
         """Returns the loaded plugins"""
         return dict(self.pm.list_name_plugin())
 
-    def _init_routers(self, dataset_routers: Optional[APIRouter]):
+    def _init_routers(self, dataset_routers: Optional[APIRouter]) -> None:
         """Setup plugin and dataset routers. Needs to run after dataset and plugin setup"""
         app_routers, plugin_dataset_routers = self.plugin_routers()
 
         if self._dataset_route_prefix:
             app_routers.append((dataset_collection_router, {'tags': ['info']}))
 
         app_routers.extend(
@@ -276,25 +288,25 @@
             cache=lambda: self.cache,
             plugins=lambda: self.plugins,
             plugin_manager=lambda: self.pm,
         )
 
         return deps
 
-    def _init_dependencies(self):
+    def _init_dependencies(self) -> None:
         """Initialize dependencies"""
         deps = self.dependencies()
 
         self._app.dependency_overrides[get_dataset_ids] = deps.dataset_ids
         self._app.dependency_overrides[get_dataset] = deps.dataset
         self._app.dependency_overrides[get_cache] = deps.cache
         self._app.dependency_overrides[get_plugins] = deps.plugins
         self._app.dependency_overrides[get_plugin_manager] = deps.plugin_manager
 
-    def _init_app(self):
+    def _init_app(self) -> FastAPI:
         """Initiate the FastAPI application."""
 
         self._app = FastAPI(**self._app_kws)
 
         self._init_routers(self._routers)
         for rt, kwargs in self._app_routers:
             self._app.include_router(rt, **kwargs)
@@ -312,15 +324,21 @@
         Plugins registered with :meth:`xpublish.Rest.register_plugin` after :meth:`xpublish.Rest.app`
         is accessed or :meth:`xpublish.Rest.serve` is called once may not take effect.
         """
         if self._app is None:
             self._app = self._init_app()
         return self._app
 
-    def serve(self, host: str = '0.0.0.0', port: int = 9000, log_level: str = 'debug', **kwargs):
+    def serve(
+        self,
+        host: str = '0.0.0.0',
+        port: int = 9000,
+        log_level: str = 'debug',
+        **kwargs,
+    ) -> None:
         """Serve this FastAPI application via :func:`uvicorn.run`.
 
         Parameters
         ----------
         host :
             Bind socket to this host.
         port :
@@ -332,15 +350,21 @@
             Additional arguments to be passed to :func:`uvicorn.run`.
 
         Notes
         -----
         This method is blocking and does not return.
 
         """
-        uvicorn.run(self.app, host=host, port=port, log_level=log_level, **kwargs)
+        uvicorn.run(
+            self.app,
+            host=host,
+            port=port,
+            log_level=log_level,
+            **kwargs,
+        )
 
 
 class SingleDatasetRest(Rest):
     """Used to publish a single Xarray dataset via a REST API (FastAPI application).
     Use :class:`xpublish.Rest` to publish multiple datasets.
 
     Parameters:
@@ -357,23 +381,23 @@
         app_kws: Optional[Dict] = None,
         plugins: Optional[Dict[str, Plugin]] = None,
     ):
         self._dataset = dataset
 
         super().__init__({}, routers, cache_kws, app_kws, plugins)
 
-    def setup_datasets(self, datasets):
+    def setup_datasets(self, datasets) -> str:
         """Modifies the dataset loading to instead connect to the
         single dataset"""
         self._dataset_route_prefix = ''
         self._datasets = {}
 
         self._get_dataset_func = lambda: self._dataset
 
         return self._dataset_route_prefix
 
-    def _init_app(self):
+    def _init_app(self) -> FastAPI:
         self._app = super()._init_app()
 
         self._app.openapi = SingleDatasetOpenAPIOverrider(self._app).openapi
 
         return self._app
```

### Comparing `xpublish-0.3.0/xpublish/utils/api.py` & `xpublish-0.3.2/xpublish/utils/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,18 @@
         if not all(isinstance(obj, xr.Dataset) for obj in datasets.values()):
             raise TypeError(error_msg)
         return {str(k): ds.assign_attrs({DATASET_ID_ATTR_KEY: k}) for k, ds in datasets.items()}
     else:
         raise TypeError(error_msg)
 
 
-def normalize_app_routers(routers: list, prefix: str) -> List[Tuple[APIRouter, Dict]]:
+def normalize_app_routers(
+    routers: list,
+    prefix: str,
+) -> List[Tuple[APIRouter, Dict]]:
     """Normalise the given list of (dataset-specific) API routers.
 
     Add or prepend ``prefix`` to all routers.
 
     """
     new_routers = []
 
@@ -52,15 +55,15 @@
                 'Invalid type/format for routers argument, please provide either an APIRouter '
                 'instance or a (APIRouter, {...}) tuple.'
             )
 
     return new_routers
 
 
-def check_route_conflicts(routers):
+def check_route_conflicts(routers) -> None:
     paths = []
 
     for router, kws in routers:
         prefix = kws.get('prefix', '')
         paths += [prefix + r.path for r in router.routes]
 
     seen = set()
@@ -86,18 +89,18 @@
     See:
 
     - https://fastapi.tiangolo.com/advanced/extending-openapi/
     - https://github.com/tiangolo/fastapi/issues/1594
 
     """
 
-    def __init__(self, app):
+    def __init__(self, app) -> None:
         self._app = app
 
-    def openapi(self):
+    def openapi(self) -> dict:
         if self._app.openapi_schema:
             return self._app.openapi_schema
 
         kwargs = {
             'title': self._app.title,
             'version': self._app.version,
             'description': self._app.description,
@@ -119,15 +122,15 @@
 
         self._app.openapi_schema = openapi_schema
 
         return self._app.openapi_schema
 
 
 class JSONResponse(StarletteJSONResponse):
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, **kwargs) -> None:
         self._render_kwargs = {
             'ensure_ascii': True,
             'allow_nan': True,
             'indent': None,
             'separators': (',', ':'),
         }
         self._render_kwargs.update(kwargs.pop('render_kwargs', {}))
```

### Comparing `xpublish-0.3.0/xpublish/utils/info.py` & `xpublish-0.3.2/xpublish/utils/info.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 """
 import locale
 import os
 import platform
 import struct
 import subprocess
 import sys
+from typing import Union
 
 
-def get_sys_info():
+def get_sys_info() -> list:
     'Returns system information as a dict'
 
     blob = []
 
     # get full commit hash
     if os.path.isdir('.git') and os.path.isdir('xpublish'):
         try:
@@ -53,15 +54,15 @@
             ('LOCALE', '%s.%s' % locale.getlocale()),
         ]
     )
 
     return blob
 
 
-def netcdf_and_hdf5_versions():
+def netcdf_and_hdf5_versions() -> list[tuple[str, Union[str, None]]]:
     libhdf5_version = None
     libnetcdf_version = None
     try:
         import netCDF4
 
         libhdf5_version = netCDF4.__hdf5libversion__
         libnetcdf_version = netCDF4.__netcdf4libversion__
```

### Comparing `xpublish-0.3.0/xpublish/utils/zarr.py` & `xpublish-0.3.2/xpublish/utils/zarr.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,140 +1,168 @@
 import copy
 import logging
+from typing import (
+    Any,
+    Optional,
+)
 
 import dask.array
 import numpy as np
 import xarray as xr
+from numcodecs.abc import Codec
 from numcodecs.compat import ensure_ndarray
 from xarray.backends.zarr import (
     DIMENSION_KEY,
     encode_zarr_attr_value,
     encode_zarr_variable,
     extract_zarr_variable_encoding,
 )
 from zarr.meta import encode_fill_value
-from zarr.storage import array_meta_key, attrs_key, default_compressor, group_meta_key
+from zarr.storage import (
+    array_meta_key,
+    attrs_key,
+    default_compressor,
+    group_meta_key,
+)
 from zarr.util import normalize_shape
 
 from .api import DATASET_ID_ATTR_KEY
 
-dask_array_type = (dask.array.Array,)
-zarr_format = 2
-zarr_consolidated_format = 1
-zarr_metadata_key = '.zmetadata'
+DaskArrayType = (dask.array.Array,)
+ZARR_FORMAT = 2
+ZARR_CONSOLIDATED_FORMAT = 1
+ZARR_METADATA_KEY = '.zmetadata'
 
 logger = logging.getLogger('api')
 
 
-def _extract_dataset_zattrs(dataset: xr.Dataset):
+def _extract_dataset_zattrs(dataset: xr.Dataset) -> dict:
     """helper function to create zattrs dictionary from Dataset global attrs"""
     zattrs = {}
     for k, v in dataset.attrs.items():
         zattrs[k] = encode_zarr_attr_value(v)
 
     # remove xpublish internal attribute
     zattrs.pop(DATASET_ID_ATTR_KEY, None)
 
     return zattrs
 
 
-def _extract_dataarray_zattrs(da):
+def _extract_dataarray_zattrs(da: xr.DataArray) -> dict:
     """helper function to extract zattrs dictionary from DataArray"""
     zattrs = {}
     for k, v in da.attrs.items():
         zattrs[k] = encode_zarr_attr_value(v)
     zattrs[DIMENSION_KEY] = list(da.dims)
 
     # We don't want `_FillValue` in `.zattrs`
     # It should go in `fill_value` section of `.zarray`
     _ = zattrs.pop('_FillValue', None)
 
     return zattrs
 
 
-def _extract_dataarray_coords(da, zattrs):
+def _extract_dataarray_coords(
+    da: xr.DataArray,
+    zattrs: dict,
+) -> dict:
     '''helper function to extract coords from DataArray into a directionary'''
     if da.coords:
         # Coordinates are only encoded if there are non-dimension coordinates
         nondim_coords = set(da.coords) - set(da.dims)
 
         if len(nondim_coords) > 0 and da.name not in nondim_coords:
             coords = ' '.join(sorted(nondim_coords))
             zattrs['coordinates'] = encode_zarr_attr_value(coords)
     return zattrs
 
 
-def _extract_fill_value(da, dtype):
+def _extract_fill_value(
+    da: xr.DataArray,
+    dtype: np.dtype,
+) -> Any:
     """helper function to extract fill value from DataArray."""
     fill_value = da.attrs.pop('_FillValue', None)
     return encode_fill_value(fill_value, dtype)
 
 
-def _extract_zarray(da, encoding, dtype):
+def _extract_zarray(
+    da: xr.DataArray,
+    encoding: dict,
+    dtype: np.dtype,
+) -> dict:
     """helper function to extract zarr array metadata."""
     meta = {
         'compressor': encoding.get('compressor', da.encoding.get('compressor', default_compressor)),
         'filters': encoding.get('filters', da.encoding.get('filters', None)),
         'chunks': encoding.get('chunks', None),
         'dtype': dtype.str,
         'fill_value': _extract_fill_value(da, dtype),
         'order': 'C',
         'shape': list(normalize_shape(da.shape)),
-        'zarr_format': zarr_format,
+        'zarr_format': ZARR_FORMAT,
     }
 
     if meta['chunks'] is None:
         meta['chunks'] = da.shape
 
     # validate chunks
-    if isinstance(da.data, dask_array_type):
+    if isinstance(da.data, DaskArrayType):
         var_chunks = tuple([c[0] for c in da.data.chunks])
     else:
         var_chunks = da.shape
     if not var_chunks == tuple(meta['chunks']):
         raise ValueError('Encoding chunks do not match inferred chunks')
 
     meta['chunks'] = list(meta['chunks'])  # return chunks as a list
 
     return meta
 
 
-def create_zvariables(dataset):
+def create_zvariables(dataset: xr.Dataset) -> dict:
     """Helper function to create a dictionary of zarr encoded variables."""
     zvariables = {}
 
     for key, da in dataset.variables.items():
         encoded_da = encode_zarr_variable(da, name=key)
         zvariables[key] = encoded_da
 
     return zvariables
 
 
-def create_zmetadata(dataset):
+def create_zmetadata(dataset: xr.Dataset) -> dict:
     """Helper function to create a consolidated zmetadata dictionary."""
 
-    zmeta = {'zarr_consolidated_format': zarr_consolidated_format, 'metadata': {}}
-    zmeta['metadata'][group_meta_key] = {'zarr_format': zarr_format}
+    zmeta = {
+        'zarr_consolidated_format': ZARR_CONSOLIDATED_FORMAT,
+        'metadata': {},
+    }
+    zmeta['metadata'][group_meta_key] = {'zarr_format': ZARR_FORMAT}
     zmeta['metadata'][attrs_key] = _extract_dataset_zattrs(dataset)
 
     for key, dvar in dataset.variables.items():
         da = dataset[key]
         encoded_da = encode_zarr_variable(dvar, name=key)
         encoding = extract_zarr_variable_encoding(dvar)
         zattrs = _extract_dataarray_zattrs(encoded_da)
         zattrs = _extract_dataarray_coords(da, zattrs)
         zmeta['metadata'][f'{key}/{attrs_key}'] = zattrs
         zmeta['metadata'][f'{key}/{array_meta_key}'] = _extract_zarray(
-            encoded_da, encoding, encoded_da.dtype
+            encoded_da,
+            encoding,
+            encoded_da.dtype,
         )
 
     return zmeta
 
 
-def jsonify_zmetadata(dataset: xr.Dataset, zmetadata: dict) -> dict:
+def jsonify_zmetadata(
+    dataset: xr.Dataset,
+    zmetadata: dict,
+) -> dict:
     """Helper function to convert zmetadata dictionary to a json
     compatible dictionary.
 
     """
     zjson = copy.deepcopy(zmetadata)
 
     for key in list(dataset.variables):
@@ -145,15 +173,19 @@
                 'compressor'
             ].get_config()
             zjson['metadata'][f'{key}/{array_meta_key}']['compressor'] = compressor_config
 
     return zjson
 
 
-def encode_chunk(chunk, filters=None, compressor=None):
+def encode_chunk(
+    chunk: np.typing.ArrayLike,
+    filters: Optional[list[Codec]] = None,
+    compressor: Optional[Codec] = None,
+) -> np.typing.ArrayLike:
     """helper function largely copied from zarr.Array"""
     # apply filters
     if filters:
         for f in filters:
             chunk = f.encode(chunk)
 
     # check object encoding
@@ -165,33 +197,37 @@
         cdata = compressor.encode(chunk)
     else:
         cdata = chunk
 
     return cdata
 
 
-def get_data_chunk(da, chunk_id, out_shape):
+def get_data_chunk(
+    da: xr.DataArray,
+    chunk_id: str,
+    out_shape: tuple,
+) -> np.typing.ArrayLike:
     """Get one chunk of data from this DataArray (da).
 
     If this is an incomplete edge chunk, pad the returned array to match out_shape.
     """
     ikeys = tuple(map(int, chunk_id.split('.')))
-    if isinstance(da, dask_array_type):
+    if isinstance(da, DaskArrayType):
         chunk_data = da.blocks[ikeys]
     else:
         if da.ndim > 0 and ikeys != ((0,) * da.ndim):
             raise ValueError(
                 'Invalid chunk_id for numpy array: %s. Should have been: %s'
                 % (chunk_id, ((0,) * da.ndim))
             )
         chunk_data = np.asarray(da)
 
     logger.debug('checking chunk output size, %s == %s' % (chunk_data.shape, out_shape))
 
-    if isinstance(chunk_data, dask_array_type):
+    if isinstance(chunk_data, DaskArrayType):
         chunk_data = chunk_data.compute()
 
     # zarr expects full edge chunks, contents out of bounds for the array are undefined
     if chunk_data.shape != tuple(out_shape):
         new_chunk = np.empty_like(chunk_data, shape=out_shape)
         write_slice = tuple([slice(0, s) for s in chunk_data.shape])
         new_chunk[write_slice] = chunk_data
```

