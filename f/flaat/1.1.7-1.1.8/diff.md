# Comparing `tmp/flaat-1.1.7.tar.gz` & `tmp/flaat-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flaat-1.1.7.tar", last modified: Fri Jan 20 13:08:20 2023, max compression
+gzip compressed data, was "flaat-1.1.8.tar", last modified: Fri Jan 20 13:11:19 2023, max compression
```

## Comparing `flaat-1.1.7.tar` & `flaat-1.1.8.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 marcus    (1000) marcus    (1000)        0 2023-01-20 13:08:20.528771 flaat-1.1.7/
--rw-r--r--   0 marcus    (1000) marcus    (1000)      936 2022-03-22 11:31:25.000000 flaat-1.1.7/.env-template
-drwxr-xr-x   0 marcus    (1000) marcus    (1000)        0 2023-01-20 13:08:20.516771 flaat-1.1.7/.github/
-drwxr-xr-x   0 marcus    (1000) marcus    (1000)        0 2023-01-20 13:08:20.520771 flaat-1.1.7/.github/workflows/
--rw-r--r--   0 marcus    (1000) marcus    (1000)      610 2022-02-25 13:23:38.000000 flaat-1.1.7/.github/workflows/ci.yml
--rw-r--r--   0 marcus    (1000) marcus    (1000)       55 2022-10-10 14:37:09.000000 flaat-1.1.7/.mdlrc
--rw-r--r--   0 marcus    (1000) marcus    (1000)    14596 2022-02-25 13:23:38.000000 flaat-1.1.7/.pylintrc
--rw-r--r--   0 marcus    (1000) marcus    (1000)      726 2022-04-14 15:23:41.000000 flaat-1.1.7/.readthedocs.yaml
--rw-r--r--   0 marcus    (1000) marcus    (1000)      308 2023-01-20 13:08:19.000000 flaat-1.1.7/AUTHORS
--rw-r--r--   0 marcus    (1000) marcus    (1000)       69 2022-10-10 14:42:12.000000 flaat-1.1.7/CODE_OF_CONDUCT
--rw-r--r--   0 marcus    (1000) marcus    (1000)       71 2022-10-10 14:41:46.000000 flaat-1.1.7/CONTRIBUTING
--rw-r--r--   0 marcus    (1000) marcus    (1000)    14624 2023-01-20 13:08:19.000000 flaat-1.1.7/ChangeLog
--rw-r--r--   0 marcus    (1000) marcus    (1000)     1130 2022-02-25 13:23:38.000000 flaat-1.1.7/LICENSE
--rw-r--r--   0 marcus    (1000) marcus    (1000)      543 2022-02-25 13:23:38.000000 flaat-1.1.7/Makefile
--rw-r--r--   0 marcus    (1000) marcus    (1000)     2547 2023-01-20 13:08:20.528771 flaat-1.1.7/PKG-INFO
--rw-r--r--   0 marcus    (1000) marcus    (1000)     1338 2022-10-10 14:39:30.000000 flaat-1.1.7/README.md
--rw-r--r--   0 marcus    (1000) marcus    (1000)     2888 2022-07-26 10:24:50.000000 flaat-1.1.7/conftest.py
-drwxr-xr-x   0 marcus    (1000) marcus    (1000)        0 2023-01-20 13:08:20.516771 flaat-1.1.7/doc/
-drwxr-xr-x   0 marcus    (1000) marcus    (1000)        0 2023-01-20 13:08:20.520771 flaat-1.1.7/doc/source/
-drwxr-xr-x   0 marcus    (1000) marcus    (1000)        0 2023-01-20 13:08:20.520771 flaat-1.1.7/doc/source/_static/
--rw-r--r--   0 marcus    (1000) marcus    (1000)     9342 2020-04-29 10:22:45.000000 flaat-1.1.7/doc/source/_static/logo.png
-drwxr-xr-x   0 marcus    (1000) marcus    (1000)        0 2023-01-20 13:08:20.520771 flaat-1.1.7/doc/source/_templates/
--rw-r--r--   0 marcus    (1000) marcus    (1000)      282 2020-04-29 10:22:45.000000 flaat-1.1.7/doc/source/_templates/sidebarfooter.html
--rw-r--r--   0 marcus    (1000) marcus    (1000)     7948 2022-02-25 13:23:38.000000 flaat-1.1.7/doc/source/conf.py
-drwxr-xr-x   0 marcus    (1000) marcus    (1000)        0 2023-01-20 13:08:20.520771 flaat-1.1.7/doc/source/flaat/
-drwxr-xr-x   0 marcus    (1000) marcus    (1000)        0 2023-01-20 13:08:20.520771 flaat-1.1.7/doc/source/flaat/api/
--rw-r--r--   0 marcus    (1000) marcus    (1000)      218 2022-02-25 13:23:38.000000 flaat-1.1.7/doc/source/flaat/api/config.rst
--rw-r--r--   0 marcus    (1000) marcus    (1000)      760 2022-04-22 08:42:40.000000 flaat-1.1.7/doc/source/flaat/api/index.rst
--rw-r--r--   0 marcus    (1000) marcus    (1000)     2387 2022-02-25 13:23:38.000000 flaat-1.1.7/doc/source/flaat/development.rst
-drwxr-xr-x   0 marcus    (1000) marcus    (1000)        0 2023-01-20 13:08:20.524771 flaat-1.1.7/doc/source/flaat/examples/
--rw-r--r--   0 marcus    (1000) marcus    (1000)      592 2022-02-25 13:23:38.000000 flaat-1.1.7/doc/source/flaat/examples/aio.rst
--rw-r--r--   0 marcus    (1000) marcus    (1000)      157 2022-02-25 13:23:38.000000 flaat-1.1.7/doc/source/flaat/examples/fastapi.rst
--rw-r--r--   0 marcus    (1000) marcus    (1000)      149 2022-02-25 13:23:38.000000 flaat-1.1.7/doc/source/flaat/examples/flask.rst
--rw-r--r--   0 marcus    (1000) marcus    (1000)     3073 2022-03-22 11:31:25.000000 flaat-1.1.7/doc/source/flaat/flaat-userinfo.rst
--rw-r--r--   0 marcus    (1000) marcus    (1000)      677 2022-02-25 13:23:38.000000 flaat-1.1.7/doc/source/flaat/installation.rst
--rw-r--r--   0 marcus    (1000) marcus    (1000)     1132 2022-07-26 10:24:50.000000 flaat-1.1.7/doc/source/index.rst
--rw-r--r--   0 marcus    (1000) marcus    (1000)       73 2022-04-14 10:02:26.000000 flaat-1.1.7/doc/source/requirements.txt
-drwxr-xr-x   0 marcus    (1000) marcus    (1000)        0 2023-01-20 13:08:20.524771 flaat-1.1.7/examples/
--rw-r--r--   0 marcus    (1000) marcus    (1000)        0 2022-02-25 13:23:38.000000 flaat-1.1.7/examples/__init__.py
--rw-r--r--   0 marcus    (1000) marcus    (1000)     5889 2023-01-20 13:06:19.000000 flaat-1.1.7/examples/example_aio.py
--rw-r--r--   0 marcus    (1000) marcus    (1000)     7216 2023-01-20 13:06:24.000000 flaat-1.1.7/examples/example_fastapi.py
--rw-r--r--   0 marcus    (1000) marcus    (1000)     9332 2023-01-20 13:06:29.000000 flaat-1.1.7/examples/example_flask.py
--rwxr-xr-x   0 marcus    (1000) marcus    (1000)     2631 2022-02-25 13:23:38.000000 flaat-1.1.7/examples/life-test.sh
--rw-r--r--   0 marcus    (1000) marcus    (1000)       30 2022-02-25 13:23:38.000000 flaat-1.1.7/examples/requirements.txt
--rwxr-xr-x   0 marcus    (1000) marcus    (1000)      896 2022-02-25 13:23:38.000000 flaat-1.1.7/examples/testing.sh
-drwxr-xr-x   0 marcus    (1000) marcus    (1000)        0 2023-01-20 13:08:20.524771 flaat-1.1.7/flaat/
--rw-r--r--   0 marcus    (1000) marcus    (1000)    21454 2023-01-20 13:04:55.000000 flaat-1.1.7/flaat/__init__.py
--rw-r--r--   0 marcus    (1000) marcus    (1000)     5757 2023-01-20 13:03:45.000000 flaat-1.1.7/flaat/access_tokens.py
-drwxr-xr-x   0 marcus    (1000) marcus    (1000)        0 2023-01-20 13:08:20.524771 flaat-1.1.7/flaat/aio/
--rw-r--r--   0 marcus    (1000) marcus    (1000)      834 2022-02-25 13:23:38.000000 flaat-1.1.7/flaat/aio/__init__.py
--rw-r--r--   0 marcus    (1000) marcus    (1000)     1434 2022-02-25 13:23:38.000000 flaat-1.1.7/flaat/aio/aio_test.py
--rw-r--r--   0 marcus    (1000) marcus    (1000)     2781 2022-02-25 13:23:38.000000 flaat-1.1.7/flaat/aio/overrides_test.py
--rw-r--r--   0 marcus    (1000) marcus    (1000)     1003 2022-10-06 14:58:10.000000 flaat-1.1.7/flaat/caches.py
--rw-r--r--   0 marcus    (1000) marcus    (1000)     5694 2022-07-26 10:24:50.000000 flaat-1.1.7/flaat/config.py
--rw-r--r--   0 marcus    (1000) marcus    (1000)     1118 2022-02-25 13:23:38.000000 flaat-1.1.7/flaat/exceptions.py
-drwxr-xr-x   0 marcus    (1000) marcus    (1000)        0 2023-01-20 13:08:20.524771 flaat-1.1.7/flaat/fastapi/
--rw-r--r--   0 marcus    (1000) marcus    (1000)      702 2022-02-25 13:23:38.000000 flaat-1.1.7/flaat/fastapi/__init__.py
--rw-r--r--   0 marcus    (1000) marcus    (1000)     1139 2022-02-25 13:23:38.000000 flaat-1.1.7/flaat/fastapi/fastapi_test.py
--rwxr-xr-x   0 marcus    (1000) marcus    (1000)    11416 2023-01-20 13:05:14.000000 flaat-1.1.7/flaat/flaat_userinfo.py
-drwxr-xr-x   0 marcus    (1000) marcus    (1000)        0 2023-01-20 13:08:20.528771 flaat-1.1.7/flaat/flask/
--rw-r--r--   0 marcus    (1000) marcus    (1000)     5367 2022-10-04 08:41:21.000000 flaat-1.1.7/flaat/flask/__init__.py
--rw-r--r--   0 marcus    (1000) marcus    (1000)     1822 2022-10-04 08:41:21.000000 flaat-1.1.7/flaat/flask/conftest.py
--rw-r--r--   0 marcus    (1000) marcus    (1000)      495 2022-07-26 10:24:50.000000 flaat-1.1.7/flaat/flask/flask_test.py
--rw-r--r--   0 marcus    (1000) marcus    (1000)     1013 2022-07-26 10:24:50.000000 flaat-1.1.7/flaat/flask/flask_test_cases.py
--rw-r--r--   0 marcus    (1000) marcus    (1000)     6320 2022-04-13 15:10:38.000000 flaat-1.1.7/flaat/issuers.py
--rw-r--r--   0 marcus    (1000) marcus    (1000)    12220 2022-10-04 08:41:21.000000 flaat-1.1.7/flaat/requirements.py
--rw-r--r--   0 marcus    (1000) marcus    (1000)     6349 2022-03-22 11:31:25.000000 flaat-1.1.7/flaat/test_env.py
-drwxr-xr-x   0 marcus    (1000) marcus    (1000)        0 2023-01-20 13:08:20.528771 flaat-1.1.7/flaat/tests/
--rw-r--r--   0 marcus    (1000) marcus    (1000)     7358 2022-03-23 16:42:38.000000 flaat-1.1.7/flaat/tests/access_tokens_test.py
--rw-r--r--   0 marcus    (1000) marcus    (1000)     2160 2022-02-25 13:23:38.000000 flaat-1.1.7/flaat/tests/flaat_test.py
--rw-r--r--   0 marcus    (1000) marcus    (1000)     2850 2022-03-22 11:31:25.000000 flaat-1.1.7/flaat/tests/flaat_userinfo_test.py
--rw-r--r--   0 marcus    (1000) marcus    (1000)     1214 2022-02-25 13:23:38.000000 flaat-1.1.7/flaat/tests/issuers_test.py
--rw-r--r--   0 marcus    (1000) marcus    (1000)     5188 2022-03-22 11:31:25.000000 flaat-1.1.7/flaat/tests/requirements_test.py
--rw-r--r--   0 marcus    (1000) marcus    (1000)     4895 2022-03-14 11:39:22.000000 flaat-1.1.7/flaat/user_infos.py
-drwxr-xr-x   0 marcus    (1000) marcus    (1000)        0 2023-01-20 13:08:20.524771 flaat-1.1.7/flaat.egg-info/
--rw-r--r--   0 marcus    (1000) marcus    (1000)     2547 2023-01-20 13:08:19.000000 flaat-1.1.7/flaat.egg-info/PKG-INFO
--rw-r--r--   0 marcus    (1000) marcus    (1000)     1615 2023-01-20 13:08:20.000000 flaat-1.1.7/flaat.egg-info/SOURCES.txt
--rw-r--r--   0 marcus    (1000) marcus    (1000)        1 2023-01-20 13:08:19.000000 flaat-1.1.7/flaat.egg-info/dependency_links.txt
--rw-r--r--   0 marcus    (1000) marcus    (1000)       61 2023-01-20 13:08:19.000000 flaat-1.1.7/flaat.egg-info/entry_points.txt
--rw-r--r--   0 marcus    (1000) marcus    (1000)        1 2022-07-26 10:28:58.000000 flaat-1.1.7/flaat.egg-info/not-zip-safe
--rw-r--r--   0 marcus    (1000) marcus    (1000)       47 2023-01-20 13:08:19.000000 flaat-1.1.7/flaat.egg-info/pbr.json
--rw-r--r--   0 marcus    (1000) marcus    (1000)      314 2023-01-20 13:08:19.000000 flaat-1.1.7/flaat.egg-info/requires.txt
--rw-r--r--   0 marcus    (1000) marcus    (1000)        6 2023-01-20 13:08:20.000000 flaat-1.1.7/flaat.egg-info/top_level.txt
--rw-r--r--   0 marcus    (1000) marcus    (1000)      129 2022-03-14 11:48:53.000000 flaat-1.1.7/requirements.txt
--rw-r--r--   0 marcus    (1000) marcus    (1000)     1236 2023-01-20 13:08:20.528771 flaat-1.1.7/setup.cfg
--rw-r--r--   0 marcus    (1000) marcus    (1000)       86 2022-02-25 13:23:38.000000 flaat-1.1.7/setup.py
--rw-r--r--   0 marcus    (1000) marcus    (1000)      117 2022-07-26 10:24:50.000000 flaat-1.1.7/test-requirements.txt
--rw-r--r--   0 marcus    (1000) marcus    (1000)     1163 2022-04-22 10:09:55.000000 flaat-1.1.7/tox.ini
+drwxr-xr-x   0 marcus    (1000) marcus    (1000)        0 2023-01-20 13:11:19.648959 flaat-1.1.8/
+-rw-r--r--   0 marcus    (1000) marcus    (1000)      936 2022-03-22 11:31:25.000000 flaat-1.1.8/.env-template
+drwxr-xr-x   0 marcus    (1000) marcus    (1000)        0 2023-01-20 13:11:19.632959 flaat-1.1.8/.github/
+drwxr-xr-x   0 marcus    (1000) marcus    (1000)        0 2023-01-20 13:11:19.636959 flaat-1.1.8/.github/workflows/
+-rw-r--r--   0 marcus    (1000) marcus    (1000)      610 2022-02-25 13:23:38.000000 flaat-1.1.8/.github/workflows/ci.yml
+-rw-r--r--   0 marcus    (1000) marcus    (1000)       55 2022-10-10 14:37:09.000000 flaat-1.1.8/.mdlrc
+-rw-r--r--   0 marcus    (1000) marcus    (1000)    14596 2022-02-25 13:23:38.000000 flaat-1.1.8/.pylintrc
+-rw-r--r--   0 marcus    (1000) marcus    (1000)      726 2022-04-14 15:23:41.000000 flaat-1.1.8/.readthedocs.yaml
+-rw-r--r--   0 marcus    (1000) marcus    (1000)      308 2023-01-20 13:11:18.000000 flaat-1.1.8/AUTHORS
+-rw-r--r--   0 marcus    (1000) marcus    (1000)       69 2022-10-10 14:42:12.000000 flaat-1.1.8/CODE_OF_CONDUCT
+-rw-r--r--   0 marcus    (1000) marcus    (1000)       71 2022-10-10 14:41:46.000000 flaat-1.1.8/CONTRIBUTING
+-rw-r--r--   0 marcus    (1000) marcus    (1000)    14677 2023-01-20 13:11:18.000000 flaat-1.1.8/ChangeLog
+-rw-r--r--   0 marcus    (1000) marcus    (1000)     1130 2022-02-25 13:23:38.000000 flaat-1.1.8/LICENSE
+-rw-r--r--   0 marcus    (1000) marcus    (1000)      543 2022-02-25 13:23:38.000000 flaat-1.1.8/Makefile
+-rw-r--r--   0 marcus    (1000) marcus    (1000)     2547 2023-01-20 13:11:19.648959 flaat-1.1.8/PKG-INFO
+-rw-r--r--   0 marcus    (1000) marcus    (1000)     1338 2022-10-10 14:39:30.000000 flaat-1.1.8/README.md
+-rw-r--r--   0 marcus    (1000) marcus    (1000)     2888 2022-07-26 10:24:50.000000 flaat-1.1.8/conftest.py
+drwxr-xr-x   0 marcus    (1000) marcus    (1000)        0 2023-01-20 13:11:19.632959 flaat-1.1.8/doc/
+drwxr-xr-x   0 marcus    (1000) marcus    (1000)        0 2023-01-20 13:11:19.636959 flaat-1.1.8/doc/source/
+drwxr-xr-x   0 marcus    (1000) marcus    (1000)        0 2023-01-20 13:11:19.636959 flaat-1.1.8/doc/source/_static/
+-rw-r--r--   0 marcus    (1000) marcus    (1000)     9342 2020-04-29 10:22:45.000000 flaat-1.1.8/doc/source/_static/logo.png
+drwxr-xr-x   0 marcus    (1000) marcus    (1000)        0 2023-01-20 13:11:19.636959 flaat-1.1.8/doc/source/_templates/
+-rw-r--r--   0 marcus    (1000) marcus    (1000)      282 2020-04-29 10:22:45.000000 flaat-1.1.8/doc/source/_templates/sidebarfooter.html
+-rw-r--r--   0 marcus    (1000) marcus    (1000)     7948 2022-02-25 13:23:38.000000 flaat-1.1.8/doc/source/conf.py
+drwxr-xr-x   0 marcus    (1000) marcus    (1000)        0 2023-01-20 13:11:19.636959 flaat-1.1.8/doc/source/flaat/
+drwxr-xr-x   0 marcus    (1000) marcus    (1000)        0 2023-01-20 13:11:19.640959 flaat-1.1.8/doc/source/flaat/api/
+-rw-r--r--   0 marcus    (1000) marcus    (1000)      218 2022-02-25 13:23:38.000000 flaat-1.1.8/doc/source/flaat/api/config.rst
+-rw-r--r--   0 marcus    (1000) marcus    (1000)      760 2022-04-22 08:42:40.000000 flaat-1.1.8/doc/source/flaat/api/index.rst
+-rw-r--r--   0 marcus    (1000) marcus    (1000)     2387 2022-02-25 13:23:38.000000 flaat-1.1.8/doc/source/flaat/development.rst
+drwxr-xr-x   0 marcus    (1000) marcus    (1000)        0 2023-01-20 13:11:19.640959 flaat-1.1.8/doc/source/flaat/examples/
+-rw-r--r--   0 marcus    (1000) marcus    (1000)      592 2022-02-25 13:23:38.000000 flaat-1.1.8/doc/source/flaat/examples/aio.rst
+-rw-r--r--   0 marcus    (1000) marcus    (1000)      157 2022-02-25 13:23:38.000000 flaat-1.1.8/doc/source/flaat/examples/fastapi.rst
+-rw-r--r--   0 marcus    (1000) marcus    (1000)      149 2022-02-25 13:23:38.000000 flaat-1.1.8/doc/source/flaat/examples/flask.rst
+-rw-r--r--   0 marcus    (1000) marcus    (1000)     3073 2022-03-22 11:31:25.000000 flaat-1.1.8/doc/source/flaat/flaat-userinfo.rst
+-rw-r--r--   0 marcus    (1000) marcus    (1000)      677 2022-02-25 13:23:38.000000 flaat-1.1.8/doc/source/flaat/installation.rst
+-rw-r--r--   0 marcus    (1000) marcus    (1000)     1132 2022-07-26 10:24:50.000000 flaat-1.1.8/doc/source/index.rst
+-rw-r--r--   0 marcus    (1000) marcus    (1000)       73 2022-04-14 10:02:26.000000 flaat-1.1.8/doc/source/requirements.txt
+drwxr-xr-x   0 marcus    (1000) marcus    (1000)        0 2023-01-20 13:11:19.640959 flaat-1.1.8/examples/
+-rw-r--r--   0 marcus    (1000) marcus    (1000)        0 2022-02-25 13:23:38.000000 flaat-1.1.8/examples/__init__.py
+-rw-r--r--   0 marcus    (1000) marcus    (1000)     5889 2023-01-20 13:06:19.000000 flaat-1.1.8/examples/example_aio.py
+-rw-r--r--   0 marcus    (1000) marcus    (1000)     7216 2023-01-20 13:06:24.000000 flaat-1.1.8/examples/example_fastapi.py
+-rw-r--r--   0 marcus    (1000) marcus    (1000)     9332 2023-01-20 13:06:29.000000 flaat-1.1.8/examples/example_flask.py
+-rwxr-xr-x   0 marcus    (1000) marcus    (1000)     2631 2022-02-25 13:23:38.000000 flaat-1.1.8/examples/life-test.sh
+-rw-r--r--   0 marcus    (1000) marcus    (1000)       30 2022-02-25 13:23:38.000000 flaat-1.1.8/examples/requirements.txt
+-rwxr-xr-x   0 marcus    (1000) marcus    (1000)      896 2022-02-25 13:23:38.000000 flaat-1.1.8/examples/testing.sh
+drwxr-xr-x   0 marcus    (1000) marcus    (1000)        0 2023-01-20 13:11:19.644959 flaat-1.1.8/flaat/
+-rw-r--r--   0 marcus    (1000) marcus    (1000)    21454 2023-01-20 13:04:55.000000 flaat-1.1.8/flaat/__init__.py
+-rw-r--r--   0 marcus    (1000) marcus    (1000)     5757 2023-01-20 13:03:45.000000 flaat-1.1.8/flaat/access_tokens.py
+drwxr-xr-x   0 marcus    (1000) marcus    (1000)        0 2023-01-20 13:11:19.644959 flaat-1.1.8/flaat/aio/
+-rw-r--r--   0 marcus    (1000) marcus    (1000)      834 2022-02-25 13:23:38.000000 flaat-1.1.8/flaat/aio/__init__.py
+-rw-r--r--   0 marcus    (1000) marcus    (1000)     1434 2022-02-25 13:23:38.000000 flaat-1.1.8/flaat/aio/aio_test.py
+-rw-r--r--   0 marcus    (1000) marcus    (1000)     2781 2022-02-25 13:23:38.000000 flaat-1.1.8/flaat/aio/overrides_test.py
+-rw-r--r--   0 marcus    (1000) marcus    (1000)     1003 2022-10-06 14:58:10.000000 flaat-1.1.8/flaat/caches.py
+-rw-r--r--   0 marcus    (1000) marcus    (1000)     5694 2022-07-26 10:24:50.000000 flaat-1.1.8/flaat/config.py
+-rw-r--r--   0 marcus    (1000) marcus    (1000)     1118 2022-02-25 13:23:38.000000 flaat-1.1.8/flaat/exceptions.py
+drwxr-xr-x   0 marcus    (1000) marcus    (1000)        0 2023-01-20 13:11:19.644959 flaat-1.1.8/flaat/fastapi/
+-rw-r--r--   0 marcus    (1000) marcus    (1000)      702 2022-02-25 13:23:38.000000 flaat-1.1.8/flaat/fastapi/__init__.py
+-rw-r--r--   0 marcus    (1000) marcus    (1000)     1139 2022-02-25 13:23:38.000000 flaat-1.1.8/flaat/fastapi/fastapi_test.py
+-rwxr-xr-x   0 marcus    (1000) marcus    (1000)    11416 2023-01-20 13:05:14.000000 flaat-1.1.8/flaat/flaat_userinfo.py
+drwxr-xr-x   0 marcus    (1000) marcus    (1000)        0 2023-01-20 13:11:19.644959 flaat-1.1.8/flaat/flask/
+-rw-r--r--   0 marcus    (1000) marcus    (1000)     5367 2022-10-04 08:41:21.000000 flaat-1.1.8/flaat/flask/__init__.py
+-rw-r--r--   0 marcus    (1000) marcus    (1000)     1822 2022-10-04 08:41:21.000000 flaat-1.1.8/flaat/flask/conftest.py
+-rw-r--r--   0 marcus    (1000) marcus    (1000)      495 2022-07-26 10:24:50.000000 flaat-1.1.8/flaat/flask/flask_test.py
+-rw-r--r--   0 marcus    (1000) marcus    (1000)     1013 2022-07-26 10:24:50.000000 flaat-1.1.8/flaat/flask/flask_test_cases.py
+-rw-r--r--   0 marcus    (1000) marcus    (1000)     6320 2022-04-13 15:10:38.000000 flaat-1.1.8/flaat/issuers.py
+-rw-r--r--   0 marcus    (1000) marcus    (1000)    12220 2022-10-04 08:41:21.000000 flaat-1.1.8/flaat/requirements.py
+-rw-r--r--   0 marcus    (1000) marcus    (1000)     6349 2022-03-22 11:31:25.000000 flaat-1.1.8/flaat/test_env.py
+drwxr-xr-x   0 marcus    (1000) marcus    (1000)        0 2023-01-20 13:11:19.648959 flaat-1.1.8/flaat/tests/
+-rw-r--r--   0 marcus    (1000) marcus    (1000)     7358 2022-03-23 16:42:38.000000 flaat-1.1.8/flaat/tests/access_tokens_test.py
+-rw-r--r--   0 marcus    (1000) marcus    (1000)     2160 2022-02-25 13:23:38.000000 flaat-1.1.8/flaat/tests/flaat_test.py
+-rw-r--r--   0 marcus    (1000) marcus    (1000)     2850 2022-03-22 11:31:25.000000 flaat-1.1.8/flaat/tests/flaat_userinfo_test.py
+-rw-r--r--   0 marcus    (1000) marcus    (1000)     1214 2022-02-25 13:23:38.000000 flaat-1.1.8/flaat/tests/issuers_test.py
+-rw-r--r--   0 marcus    (1000) marcus    (1000)     5188 2022-03-22 11:31:25.000000 flaat-1.1.8/flaat/tests/requirements_test.py
+-rw-r--r--   0 marcus    (1000) marcus    (1000)     4895 2022-03-14 11:39:22.000000 flaat-1.1.8/flaat/user_infos.py
+drwxr-xr-x   0 marcus    (1000) marcus    (1000)        0 2023-01-20 13:11:19.644959 flaat-1.1.8/flaat.egg-info/
+-rw-r--r--   0 marcus    (1000) marcus    (1000)     2547 2023-01-20 13:11:18.000000 flaat-1.1.8/flaat.egg-info/PKG-INFO
+-rw-r--r--   0 marcus    (1000) marcus    (1000)     1615 2023-01-20 13:11:19.000000 flaat-1.1.8/flaat.egg-info/SOURCES.txt
+-rw-r--r--   0 marcus    (1000) marcus    (1000)        1 2023-01-20 13:11:18.000000 flaat-1.1.8/flaat.egg-info/dependency_links.txt
+-rw-r--r--   0 marcus    (1000) marcus    (1000)       61 2023-01-20 13:11:18.000000 flaat-1.1.8/flaat.egg-info/entry_points.txt
+-rw-r--r--   0 marcus    (1000) marcus    (1000)        1 2022-07-26 10:28:58.000000 flaat-1.1.8/flaat.egg-info/not-zip-safe
+-rw-r--r--   0 marcus    (1000) marcus    (1000)       47 2023-01-20 13:11:18.000000 flaat-1.1.8/flaat.egg-info/pbr.json
+-rw-r--r--   0 marcus    (1000) marcus    (1000)      333 2023-01-20 13:11:19.000000 flaat-1.1.8/flaat.egg-info/requires.txt
+-rw-r--r--   0 marcus    (1000) marcus    (1000)        6 2023-01-20 13:11:19.000000 flaat-1.1.8/flaat.egg-info/top_level.txt
+-rw-r--r--   0 marcus    (1000) marcus    (1000)      148 2023-01-20 13:10:38.000000 flaat-1.1.8/requirements.txt
+-rw-r--r--   0 marcus    (1000) marcus    (1000)     1236 2023-01-20 13:11:19.648959 flaat-1.1.8/setup.cfg
+-rw-r--r--   0 marcus    (1000) marcus    (1000)       86 2022-02-25 13:23:38.000000 flaat-1.1.8/setup.py
+-rw-r--r--   0 marcus    (1000) marcus    (1000)      117 2022-07-26 10:24:50.000000 flaat-1.1.8/test-requirements.txt
+-rw-r--r--   0 marcus    (1000) marcus    (1000)     1163 2022-04-22 10:09:55.000000 flaat-1.1.8/tox.ini
```

### Comparing `flaat-1.1.7/.env-template` & `flaat-1.1.8/.env-template`

 * *Files identical despite different names*

### Comparing `flaat-1.1.7/.github/workflows/ci.yml` & `flaat-1.1.8/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `flaat-1.1.7/.pylintrc` & `flaat-1.1.8/.pylintrc`

 * *Files identical despite different names*

### Comparing `flaat-1.1.7/.readthedocs.yaml` & `flaat-1.1.8/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `flaat-1.1.7/ChangeLog` & `flaat-1.1.8/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 CHANGES
 =======
 
+v1.1.8
+------
+
+* add "cryptography" to dependencies
+
 v1.1.7
 ------
 
 * add proxy.eduteams.org as a trustedOP
 
 v1.1.6
 ------
```

### Comparing `flaat-1.1.7/LICENSE` & `flaat-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `flaat-1.1.7/Makefile` & `flaat-1.1.8/Makefile`

 * *Files identical despite different names*

### Comparing `flaat-1.1.7/PKG-INFO` & `flaat-1.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flaat
-Version: 1.1.7
+Version: 1.1.8
 Summary: User authorization for OIDC authenticated python web APIs.
 Home-page: https://github.com/indigo-dc/flaat
 Author: Marcus Hardt
 Author-email: hardt@kit.edu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/indigo-dc/flaat/issues
 Project-URL: Documentation, https://flaat.readthedocs.io/en/latest/
```

### Comparing `flaat-1.1.7/README.md` & `flaat-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `flaat-1.1.7/conftest.py` & `flaat-1.1.8/conftest.py`

 * *Files identical despite different names*

### Comparing `flaat-1.1.7/doc/source/_static/logo.png` & `flaat-1.1.8/doc/source/_static/logo.png`

 * *Files identical despite different names*

### Comparing `flaat-1.1.7/doc/source/conf.py` & `flaat-1.1.8/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `flaat-1.1.7/doc/source/flaat/api/index.rst` & `flaat-1.1.8/doc/source/flaat/api/index.rst`

 * *Files identical despite different names*

### Comparing `flaat-1.1.7/doc/source/flaat/development.rst` & `flaat-1.1.8/doc/source/flaat/development.rst`

 * *Files identical despite different names*

### Comparing `flaat-1.1.7/doc/source/flaat/examples/aio.rst` & `flaat-1.1.8/doc/source/flaat/examples/aio.rst`

 * *Files identical despite different names*

### Comparing `flaat-1.1.7/doc/source/flaat/flaat-userinfo.rst` & `flaat-1.1.8/doc/source/flaat/flaat-userinfo.rst`

 * *Files identical despite different names*

### Comparing `flaat-1.1.7/doc/source/flaat/installation.rst` & `flaat-1.1.8/doc/source/flaat/installation.rst`

 * *Files identical despite different names*

### Comparing `flaat-1.1.7/doc/source/index.rst` & `flaat-1.1.8/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `flaat-1.1.7/examples/example_aio.py` & `flaat-1.1.8/examples/example_aio.py`

 * *Files identical despite different names*

### Comparing `flaat-1.1.7/examples/example_fastapi.py` & `flaat-1.1.8/examples/example_fastapi.py`

 * *Files identical despite different names*

### Comparing `flaat-1.1.7/examples/example_flask.py` & `flaat-1.1.8/examples/example_flask.py`

 * *Files identical despite different names*

### Comparing `flaat-1.1.7/examples/life-test.sh` & `flaat-1.1.8/examples/life-test.sh`

 * *Files identical despite different names*

### Comparing `flaat-1.1.7/examples/testing.sh` & `flaat-1.1.8/examples/testing.sh`

 * *Files identical despite different names*

### Comparing `flaat-1.1.7/flaat/__init__.py` & `flaat-1.1.8/flaat/__init__.py`

 * *Files identical despite different names*

### Comparing `flaat-1.1.7/flaat/access_tokens.py` & `flaat-1.1.8/flaat/access_tokens.py`

 * *Files identical despite different names*

### Comparing `flaat-1.1.7/flaat/aio/__init__.py` & `flaat-1.1.8/flaat/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `flaat-1.1.7/flaat/aio/aio_test.py` & `flaat-1.1.8/flaat/aio/aio_test.py`

 * *Files identical despite different names*

### Comparing `flaat-1.1.7/flaat/aio/overrides_test.py` & `flaat-1.1.8/flaat/aio/overrides_test.py`

 * *Files identical despite different names*

### Comparing `flaat-1.1.7/flaat/caches.py` & `flaat-1.1.8/flaat/caches.py`

 * *Files identical despite different names*

### Comparing `flaat-1.1.7/flaat/config.py` & `flaat-1.1.8/flaat/config.py`

 * *Files identical despite different names*

### Comparing `flaat-1.1.7/flaat/exceptions.py` & `flaat-1.1.8/flaat/exceptions.py`

 * *Files identical despite different names*

### Comparing `flaat-1.1.7/flaat/fastapi/__init__.py` & `flaat-1.1.8/flaat/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `flaat-1.1.7/flaat/fastapi/fastapi_test.py` & `flaat-1.1.8/flaat/fastapi/fastapi_test.py`

 * *Files identical despite different names*

### Comparing `flaat-1.1.7/flaat/flaat_userinfo.py` & `flaat-1.1.8/flaat/flaat_userinfo.py`

 * *Files identical despite different names*

### Comparing `flaat-1.1.7/flaat/flask/__init__.py` & `flaat-1.1.8/flaat/flask/__init__.py`

 * *Files identical despite different names*

### Comparing `flaat-1.1.7/flaat/flask/conftest.py` & `flaat-1.1.8/flaat/flask/conftest.py`

 * *Files identical despite different names*

### Comparing `flaat-1.1.7/flaat/flask/flask_test_cases.py` & `flaat-1.1.8/flaat/flask/flask_test_cases.py`

 * *Files identical despite different names*

### Comparing `flaat-1.1.7/flaat/issuers.py` & `flaat-1.1.8/flaat/issuers.py`

 * *Files identical despite different names*

### Comparing `flaat-1.1.7/flaat/requirements.py` & `flaat-1.1.8/flaat/requirements.py`

 * *Files identical despite different names*

### Comparing `flaat-1.1.7/flaat/test_env.py` & `flaat-1.1.8/flaat/test_env.py`

 * *Files identical despite different names*

### Comparing `flaat-1.1.7/flaat/tests/access_tokens_test.py` & `flaat-1.1.8/flaat/tests/access_tokens_test.py`

 * *Files identical despite different names*

### Comparing `flaat-1.1.7/flaat/tests/flaat_test.py` & `flaat-1.1.8/flaat/tests/flaat_test.py`

 * *Files identical despite different names*

### Comparing `flaat-1.1.7/flaat/tests/flaat_userinfo_test.py` & `flaat-1.1.8/flaat/tests/flaat_userinfo_test.py`

 * *Files identical despite different names*

### Comparing `flaat-1.1.7/flaat/tests/issuers_test.py` & `flaat-1.1.8/flaat/tests/issuers_test.py`

 * *Files identical despite different names*

### Comparing `flaat-1.1.7/flaat/tests/requirements_test.py` & `flaat-1.1.8/flaat/tests/requirements_test.py`

 * *Files identical despite different names*

### Comparing `flaat-1.1.7/flaat/user_infos.py` & `flaat-1.1.8/flaat/user_infos.py`

 * *Files identical despite different names*

### Comparing `flaat-1.1.7/flaat.egg-info/PKG-INFO` & `flaat-1.1.8/flaat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flaat
-Version: 1.1.7
+Version: 1.1.8
 Summary: User authorization for OIDC authenticated python web APIs.
 Home-page: https://github.com/indigo-dc/flaat
 Author: Marcus Hardt
 Author-email: hardt@kit.edu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/indigo-dc/flaat/issues
 Project-URL: Documentation, https://flaat.readthedocs.io/en/latest/
```

### Comparing `flaat-1.1.7/flaat.egg-info/SOURCES.txt` & `flaat-1.1.8/flaat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flaat-1.1.7/setup.cfg` & `flaat-1.1.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `flaat-1.1.7/tox.ini` & `flaat-1.1.8/tox.ini`

 * *Files identical despite different names*

