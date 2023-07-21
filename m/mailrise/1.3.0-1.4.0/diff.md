# Comparing `tmp/mailrise-1.3.0.tar.gz` & `tmp/mailrise-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mailrise-1.3.0.tar", last modified: Tue Dec 27 07:28:26 2022, max compression
+gzip compressed data, was "mailrise-1.4.0.tar", last modified: Fri Jul 21 18:00:00 2023, max compression
```

## Comparing `mailrise-1.3.0.tar` & `mailrise-1.4.0.tar`

### file list

```diff
@@ -1,84 +1,91 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2022-12-27 07:28:26.454944 mailrise-1.3.0/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      591 2022-08-09 14:20:17.000000 mailrise-1.3.0/.coveragerc
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2022-12-27 07:28:26.434944 mailrise-1.3.0/.devcontainer/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1371 2022-08-09 14:20:17.000000 mailrise-1.3.0/.devcontainer/Dockerfile
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2026 2022-12-26 04:23:56.000000 mailrise-1.3.0/.devcontainer/devcontainer.json
--rw-r--r--   0 vscode    (1000) vscode    (1000)       88 2022-08-09 14:20:17.000000 mailrise-1.3.0/.gitattributes
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2022-12-27 07:28:26.434944 mailrise-1.3.0/.github/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      600 2022-12-26 04:23:56.000000 mailrise-1.3.0/.github/dependabot.yml
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2022-12-27 07:28:26.434944 mailrise-1.3.0/.github/workflows/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2443 2022-12-26 04:23:56.000000 mailrise-1.3.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2544 2022-12-26 04:23:56.000000 mailrise-1.3.0/.github/workflows/docker-hub.yml
--rw-r--r--   0 vscode    (1000) vscode    (1000)      550 2022-09-03 16:07:21.000000 mailrise-1.3.0/.gitignore
--rw-r--r--   0 vscode    (1000) vscode    (1000)      461 2022-08-09 14:20:17.000000 mailrise-1.3.0/.readthedocs.yml
--rw-r--r--   0 vscode    (1000) vscode    (1000)      117 2022-08-09 14:20:17.000000 mailrise-1.3.0/AUTHORS.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1108 2022-12-27 07:23:15.000000 mailrise-1.3.0/CHANGELOG.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)    13828 2022-12-26 04:23:56.000000 mailrise-1.3.0/CONTRIBUTING.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)      439 2022-12-26 09:40:33.000000 mailrise-1.3.0/Dockerfile
--rw-r--r--   0 vscode    (1000) vscode    (1000)      457 2022-12-26 04:23:56.000000 mailrise-1.3.0/Dockerfile.buster
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1077 2022-08-09 14:20:17.000000 mailrise-1.3.0/LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)    17140 2022-12-27 07:28:26.454944 mailrise-1.3.0/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)    16270 2022-12-27 07:12:33.000000 mailrise-1.3.0/README.rst
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2022-12-27 07:28:26.434944 mailrise-1.3.0/docs/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1154 2022-12-26 04:23:56.000000 mailrise-1.3.0/docs/Makefile
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2022-12-27 07:28:26.434944 mailrise-1.3.0/docs/_static/
--rw-r--r--   0 vscode    (1000) vscode    (1000)       18 2022-08-09 14:20:17.000000 mailrise-1.3.0/docs/_static/.gitignore
--rw-r--r--   0 vscode    (1000) vscode    (1000)       41 2022-08-09 14:20:17.000000 mailrise-1.3.0/docs/authors.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)       43 2022-08-09 14:20:17.000000 mailrise-1.3.0/docs/changelog.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9735 2022-12-26 04:23:56.000000 mailrise-1.3.0/docs/conf.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)       33 2022-12-26 04:23:56.000000 mailrise-1.3.0/docs/contributing.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2246 2022-08-09 14:20:17.000000 mailrise-1.3.0/docs/index.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)       67 2022-08-09 14:20:17.000000 mailrise-1.3.0/docs/license.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)       39 2022-08-09 14:20:17.000000 mailrise-1.3.0/docs/readme.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)      233 2022-08-09 14:20:17.000000 mailrise-1.3.0/docs/requirements.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)      311 2022-08-09 14:20:17.000000 mailrise-1.3.0/pyproject.toml
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1543 2022-12-27 07:28:26.454944 mailrise-1.3.0/setup.cfg
--rw-r--r--   0 vscode    (1000) vscode    (1000)      705 2022-12-26 04:23:56.000000 mailrise-1.3.0/setup.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2022-12-27 07:28:26.424944 mailrise-1.3.0/src/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2022-12-27 07:28:26.444944 mailrise-1.3.0/src/mailrise/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      577 2022-12-26 04:23:56.000000 mailrise-1.3.0/src/mailrise/__init__.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2022-12-27 07:28:26.454944 mailrise-1.3.0/src/mailrise/asset/
--rw-r--r--   0 vscode    (1000) vscode    (1000)    92446 2022-12-27 07:06:57.000000 mailrise-1.3.0/src/mailrise/asset/homelab-diagram.png
--rw-r--r--   0 vscode    (1000) vscode    (1000)    20737 2022-12-27 06:58:54.000000 mailrise-1.3.0/src/mailrise/asset/homelab-diagram.svg
--rw-r--r--   0 vscode    (1000) vscode    (1000)    67646 2022-08-09 14:20:17.000000 mailrise-1.3.0/src/mailrise/asset/mailrise-failure-128x128.ico
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5142 2022-08-09 14:20:17.000000 mailrise-1.3.0/src/mailrise/asset/mailrise-failure-128x128.png
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10512 2022-08-09 14:20:17.000000 mailrise-1.3.0/src/mailrise/asset/mailrise-failure-256x256.png
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1293 2022-08-09 14:20:17.000000 mailrise-1.3.0/src/mailrise/asset/mailrise-failure-32x32.png
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2886 2022-08-09 14:20:17.000000 mailrise-1.3.0/src/mailrise/asset/mailrise-failure-72x72.png
--rw-r--r--   0 vscode    (1000) vscode    (1000)    67646 2022-08-09 14:20:17.000000 mailrise-1.3.0/src/mailrise/asset/mailrise-info-128x128.ico
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5042 2022-08-09 14:20:17.000000 mailrise-1.3.0/src/mailrise/asset/mailrise-info-128x128.png
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10120 2022-08-09 14:20:17.000000 mailrise-1.3.0/src/mailrise/asset/mailrise-info-256x256.png
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1293 2022-08-09 14:20:17.000000 mailrise-1.3.0/src/mailrise/asset/mailrise-info-32x32.png
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2873 2022-08-09 14:20:17.000000 mailrise-1.3.0/src/mailrise/asset/mailrise-info-72x72.png
--rw-r--r--   0 vscode    (1000) vscode    (1000)    18731 2022-08-09 14:20:17.000000 mailrise-1.3.0/src/mailrise/asset/mailrise-logo.png
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9722 2022-08-09 14:20:17.000000 mailrise-1.3.0/src/mailrise/asset/mailrise-logo.svg
--rw-r--r--   0 vscode    (1000) vscode    (1000)    67646 2022-08-09 14:20:17.000000 mailrise-1.3.0/src/mailrise/asset/mailrise-success-128x128.ico
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5186 2022-08-09 14:20:17.000000 mailrise-1.3.0/src/mailrise/asset/mailrise-success-128x128.png
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10355 2022-08-09 14:20:17.000000 mailrise-1.3.0/src/mailrise/asset/mailrise-success-256x256.png
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1311 2022-08-09 14:20:17.000000 mailrise-1.3.0/src/mailrise/asset/mailrise-success-32x32.png
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2901 2022-08-09 14:20:17.000000 mailrise-1.3.0/src/mailrise/asset/mailrise-success-72x72.png
--rw-r--r--   0 vscode    (1000) vscode    (1000)    67646 2022-08-09 14:20:17.000000 mailrise-1.3.0/src/mailrise/asset/mailrise-warning-128x128.ico
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5030 2022-08-09 14:20:17.000000 mailrise-1.3.0/src/mailrise/asset/mailrise-warning-128x128.png
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10292 2022-08-09 14:20:17.000000 mailrise-1.3.0/src/mailrise/asset/mailrise-warning-256x256.png
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1279 2022-08-09 14:20:17.000000 mailrise-1.3.0/src/mailrise/asset/mailrise-warning-32x32.png
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2851 2022-08-09 14:20:17.000000 mailrise-1.3.0/src/mailrise/asset/mailrise-warning-72x72.png
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1065 2022-12-26 04:23:56.000000 mailrise-1.3.0/src/mailrise/authenticator.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9207 2022-12-27 06:03:51.000000 mailrise-1.3.0/src/mailrise/config.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2022-08-09 14:20:17.000000 mailrise-1.3.0/src/mailrise/py.typed
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5662 2022-12-26 09:23:13.000000 mailrise-1.3.0/src/mailrise/skeleton.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    11321 2022-12-26 04:23:56.000000 mailrise-1.3.0/src/mailrise/smtp.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      484 2022-08-09 14:20:17.000000 mailrise-1.3.0/src/mailrise/util.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2022-12-27 07:28:26.444944 mailrise-1.3.0/src/mailrise.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)    17140 2022-12-27 07:28:26.000000 mailrise-1.3.0/src/mailrise.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2097 2022-12-27 07:28:26.000000 mailrise-1.3.0/src/mailrise.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2022-12-27 07:28:26.000000 mailrise-1.3.0/src/mailrise.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       51 2022-12-27 07:28:26.000000 mailrise-1.3.0/src/mailrise.egg-info/entry_points.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2022-08-09 14:20:52.000000 mailrise-1.3.0/src/mailrise.egg-info/not-zip-safe
--rw-r--r--   0 vscode    (1000) vscode    (1000)       96 2022-12-27 07:28:26.000000 mailrise-1.3.0/src/mailrise.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        9 2022-12-27 07:28:26.000000 mailrise-1.3.0/src/mailrise.egg-info/top_level.txt
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2022-12-27 07:28:26.454944 mailrise-1.3.0/tests/
--rw-r--r--   0 vscode    (1000) vscode    (1000)    12082 2022-08-09 14:20:17.000000 mailrise-1.3.0/tests/bridge.jpg
--rw-r--r--   0 vscode    (1000) vscode    (1000)      276 2022-08-09 14:20:17.000000 mailrise-1.3.0/tests/conftest.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6779 2022-12-27 06:21:21.000000 mailrise-1.3.0/tests/test_config.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4982 2022-12-26 04:23:56.000000 mailrise-1.3.0/tests/test_smtp.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2184 2022-08-09 14:20:17.000000 mailrise-1.3.0/tox.ini
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-21 18:00:00.691309 mailrise-1.4.0/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      591 2022-08-09 14:20:17.000000 mailrise-1.4.0/.coveragerc
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-21 18:00:00.471309 mailrise-1.4.0/.devcontainer/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1371 2022-08-09 14:20:17.000000 mailrise-1.4.0/.devcontainer/Dockerfile
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2026 2022-12-26 04:23:56.000000 mailrise-1.4.0/.devcontainer/devcontainer.json
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       88 2022-08-09 14:20:17.000000 mailrise-1.4.0/.gitattributes
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-21 18:00:00.471309 mailrise-1.4.0/.github/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-21 18:00:00.451309 mailrise-1.4.0/.github/actions/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-21 18:00:00.471309 mailrise-1.4.0/.github/actions/docker-build/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1162 2022-12-29 02:17:10.000000 mailrise-1.4.0/.github/actions/docker-build/action.yml
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      600 2022-12-26 04:23:56.000000 mailrise-1.4.0/.github/dependabot.yml
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-21 18:00:00.491309 mailrise-1.4.0/.github/workflows/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2443 2022-12-26 04:23:56.000000 mailrise-1.4.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      559 2023-04-15 04:15:08.000000 mailrise-1.4.0/.github/workflows/docker-hub.yml
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      658 2023-05-30 23:10:17.000000 mailrise-1.4.0/.github/workflows/github-packages.yml
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      550 2022-09-03 16:07:21.000000 mailrise-1.4.0/.gitignore
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      461 2022-08-09 14:20:17.000000 mailrise-1.4.0/.readthedocs.yml
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      117 2022-08-09 14:20:17.000000 mailrise-1.4.0/AUTHORS.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1358 2023-07-21 17:54:17.000000 mailrise-1.4.0/CHANGELOG.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    13828 2022-12-26 04:23:56.000000 mailrise-1.4.0/CONTRIBUTING.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      439 2022-12-26 09:40:33.000000 mailrise-1.4.0/Dockerfile
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1077 2022-08-09 14:20:17.000000 mailrise-1.4.0/LICENSE.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    19715 2023-07-21 18:00:00.691309 mailrise-1.4.0/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    18845 2023-04-15 20:48:36.000000 mailrise-1.4.0/README.rst
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-21 18:00:00.501309 mailrise-1.4.0/docs/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1154 2022-12-26 04:23:56.000000 mailrise-1.4.0/docs/Makefile
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-21 18:00:00.501309 mailrise-1.4.0/docs/_static/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       18 2022-08-09 14:20:17.000000 mailrise-1.4.0/docs/_static/.gitignore
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       41 2022-08-09 14:20:17.000000 mailrise-1.4.0/docs/authors.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       43 2022-08-09 14:20:17.000000 mailrise-1.4.0/docs/changelog.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9735 2022-12-26 04:23:56.000000 mailrise-1.4.0/docs/conf.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       33 2022-12-26 04:23:56.000000 mailrise-1.4.0/docs/contributing.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2246 2022-08-09 14:20:17.000000 mailrise-1.4.0/docs/index.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       67 2022-08-09 14:20:17.000000 mailrise-1.4.0/docs/license.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       39 2022-08-09 14:20:17.000000 mailrise-1.4.0/docs/readme.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      233 2022-08-09 14:20:17.000000 mailrise-1.4.0/docs/requirements.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      311 2022-08-09 14:20:17.000000 mailrise-1.4.0/pyproject.toml
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1565 2023-07-21 18:00:00.691309 mailrise-1.4.0/setup.cfg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      705 2022-12-26 04:23:56.000000 mailrise-1.4.0/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-21 18:00:00.451309 mailrise-1.4.0/src/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-21 18:00:00.501309 mailrise-1.4.0/src/mailrise/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      577 2022-12-26 04:23:56.000000 mailrise-1.4.0/src/mailrise/__init__.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-21 18:00:00.681309 mailrise-1.4.0/src/mailrise/asset/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    92446 2022-12-27 07:06:57.000000 mailrise-1.4.0/src/mailrise/asset/homelab-diagram.png
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    20737 2022-12-27 06:58:54.000000 mailrise-1.4.0/src/mailrise/asset/homelab-diagram.svg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    67646 2022-08-09 14:20:17.000000 mailrise-1.4.0/src/mailrise/asset/mailrise-failure-128x128.ico
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5142 2022-08-09 14:20:17.000000 mailrise-1.4.0/src/mailrise/asset/mailrise-failure-128x128.png
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    10512 2022-08-09 14:20:17.000000 mailrise-1.4.0/src/mailrise/asset/mailrise-failure-256x256.png
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1293 2022-08-09 14:20:17.000000 mailrise-1.4.0/src/mailrise/asset/mailrise-failure-32x32.png
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2886 2022-08-09 14:20:17.000000 mailrise-1.4.0/src/mailrise/asset/mailrise-failure-72x72.png
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    67646 2022-08-09 14:20:17.000000 mailrise-1.4.0/src/mailrise/asset/mailrise-info-128x128.ico
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5042 2022-08-09 14:20:17.000000 mailrise-1.4.0/src/mailrise/asset/mailrise-info-128x128.png
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    10120 2022-08-09 14:20:17.000000 mailrise-1.4.0/src/mailrise/asset/mailrise-info-256x256.png
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1293 2022-08-09 14:20:17.000000 mailrise-1.4.0/src/mailrise/asset/mailrise-info-32x32.png
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2873 2022-08-09 14:20:17.000000 mailrise-1.4.0/src/mailrise/asset/mailrise-info-72x72.png
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    18731 2022-08-09 14:20:17.000000 mailrise-1.4.0/src/mailrise/asset/mailrise-logo.png
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9722 2022-08-09 14:20:17.000000 mailrise-1.4.0/src/mailrise/asset/mailrise-logo.svg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    67646 2022-08-09 14:20:17.000000 mailrise-1.4.0/src/mailrise/asset/mailrise-success-128x128.ico
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5186 2022-08-09 14:20:17.000000 mailrise-1.4.0/src/mailrise/asset/mailrise-success-128x128.png
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    10355 2022-08-09 14:20:17.000000 mailrise-1.4.0/src/mailrise/asset/mailrise-success-256x256.png
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1311 2022-08-09 14:20:17.000000 mailrise-1.4.0/src/mailrise/asset/mailrise-success-32x32.png
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2901 2022-08-09 14:20:17.000000 mailrise-1.4.0/src/mailrise/asset/mailrise-success-72x72.png
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    67646 2022-08-09 14:20:17.000000 mailrise-1.4.0/src/mailrise/asset/mailrise-warning-128x128.ico
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5030 2022-08-09 14:20:17.000000 mailrise-1.4.0/src/mailrise/asset/mailrise-warning-128x128.png
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    10292 2022-08-09 14:20:17.000000 mailrise-1.4.0/src/mailrise/asset/mailrise-warning-256x256.png
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1279 2022-08-09 14:20:17.000000 mailrise-1.4.0/src/mailrise/asset/mailrise-warning-32x32.png
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2851 2022-08-09 14:20:17.000000 mailrise-1.4.0/src/mailrise/asset/mailrise-warning-72x72.png
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      996 2023-04-15 20:11:39.000000 mailrise-1.4.0/src/mailrise/basic_authenticator.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6639 2023-04-15 19:50:20.000000 mailrise-1.4.0/src/mailrise/config.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2022-08-09 14:20:17.000000 mailrise-1.4.0/src/mailrise/py.typed
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3798 2023-04-15 19:31:22.000000 mailrise-1.4.0/src/mailrise/router.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7454 2023-04-15 19:31:56.000000 mailrise-1.4.0/src/mailrise/simple_router.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5506 2023-07-21 17:41:23.000000 mailrise-1.4.0/src/mailrise/skeleton.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8532 2023-04-15 20:13:07.000000 mailrise-1.4.0/src/mailrise/smtp.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-21 18:00:00.511309 mailrise-1.4.0/src/mailrise.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    19715 2023-07-21 18:00:00.000000 mailrise-1.4.0/src/mailrise.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2270 2023-07-21 18:00:00.000000 mailrise-1.4.0/src/mailrise.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-07-21 18:00:00.000000 mailrise-1.4.0/src/mailrise.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       51 2023-07-21 18:00:00.000000 mailrise-1.4.0/src/mailrise.egg-info/entry_points.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2022-08-09 14:20:52.000000 mailrise-1.4.0/src/mailrise.egg-info/not-zip-safe
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      117 2023-07-21 18:00:00.000000 mailrise-1.4.0/src/mailrise.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        9 2023-07-21 18:00:00.000000 mailrise-1.4.0/src/mailrise.egg-info/top_level.txt
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-21 18:00:00.691309 mailrise-1.4.0/tests/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    12082 2022-08-09 14:20:17.000000 mailrise-1.4.0/tests/bridge.jpg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      276 2022-08-09 14:20:17.000000 mailrise-1.4.0/tests/conftest.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1774 2023-04-15 20:13:37.000000 mailrise-1.4.0/tests/noop_pluggable.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7679 2023-04-15 19:51:33.000000 mailrise-1.4.0/tests/test_config.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1112 2023-04-15 20:01:57.000000 mailrise-1.4.0/tests/test_importer.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1212 2023-03-03 07:09:25.000000 mailrise-1.4.0/tests/test_simple_router.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3944 2023-03-03 08:22:14.000000 mailrise-1.4.0/tests/test_smtp.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2184 2022-08-09 14:20:17.000000 mailrise-1.4.0/tox.ini
```

### Comparing `mailrise-1.3.0/.coveragerc` & `mailrise-1.4.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `mailrise-1.3.0/.devcontainer/Dockerfile` & `mailrise-1.4.0/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `mailrise-1.3.0/.devcontainer/devcontainer.json` & `mailrise-1.4.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `mailrise-1.3.0/.github/dependabot.yml` & `mailrise-1.4.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `mailrise-1.3.0/.github/workflows/codeql-analysis.yml` & `mailrise-1.4.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `mailrise-1.3.0/.gitignore` & `mailrise-1.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mailrise-1.3.0/CHANGELOG.rst` & `mailrise-1.4.0/CHANGELOG.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 =========
 Changelog
 =========
 
+Version 1.4.0
+=============
+
+:Date: July 21, 2023
+
+- FIX: Make it possible to run Mailrise on Windows
+- Upgrade to Apprise v1.4.5
+- Add custom routers for programmable notification routing
+- Add custom authenticators for programmable authentication
+
 Version 1.3.0
 =============
 
 :Date: December 26, 2022
 
 - FIX: Docker image not responding to stop signal
 - Upgrade to Apprise v1.2.0
```

### Comparing `mailrise-1.3.0/CONTRIBUTING.rst` & `mailrise-1.4.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `mailrise-1.3.0/LICENSE.txt` & `mailrise-1.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mailrise-1.3.0/PKG-INFO` & `mailrise-1.4.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,7 @@
-Metadata-Version: 2.1
-Name: mailrise
-Version: 1.3.0
-Summary: An SMTP gateway for Apprise notifications.
-Home-page: https://mailrise.xyz
-Author: Ryan Young
-Author-email: ryan@youngryan.com
-License: MIT
-Project-URL: Documentation, https://pyscaffold.org/
-Platform: any
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: Communications :: Email
-Classifier: Environment :: No Input/Output (Daemon)
-Classifier: Intended Audience :: System Administrators
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >=3.8
-Description-Content-Type: text/x-rst; charset=UTF-8
-Provides-Extra: testing
-License-File: LICENSE.txt
-License-File: AUTHORS.rst
-
 .. image:: https://raw.githubusercontent.com/YoRyan/mailrise/main/src/mailrise/asset/mailrise-logo.png
   :alt: Mailrise logo
 
 
 ========
 mailrise
 ========
@@ -62,15 +37,15 @@
 
 Just as email brought written messages into the 21st century, Mailrise
 brings email notifications into the year 2021 and beyond. Compared to a
 conventional SMTP server, it's more secure, too—no more replicating your Gmail
 password to each of your Linux boxes!
 
     "After a few very negative experiences with mail providers and their
-    detection of spam accounts in the last year... Fuck email. I will never set
+    detection of spam accounts in the last year... F––k email. I will never set
     up a mail account for notifications. And with Mailrise I don't have to
     anymore!"
 
     -- `u/Sarcism <https://www.reddit.com/r/selfhosted/comments/wwx0ue/comment/ilnqhkf/>`_
 
 A Mailrise daemon is configured with a list of Apprise
 `configuration files <https://github.com/caronc/apprise/wiki/config_yaml>`_.
@@ -112,15 +87,36 @@
 ============
 
 As a Docker container
 ---------------------
 
 An official Docker image is available
 `from Docker Hub <https://hub.docker.com/r/yoryan/mailrise>`_. To use it, you
-must bind mount a configuration file to ``/etc/mailrise.conf``.
+must bind mount a configuration file to ``/etc/mailrise.conf``. This mount must
+be a *file*, not a directory, and it cannot override anything else in /etc.
+
+Notes for NAS users
+^^^^^^^^^^^^^^^^^^^
+
+Consumer NAS operating systems often conceal Docker's controls behind a GUI that
+is opaque and difficult to troubleshoot. There are some known gotchas when using
+Mailrise with one:
+
+* Unraid can only passthrough directories, not files, making it impossible to
+  bind mount the mailrise.conf file. (While attempting to do so, some users have
+  accidentally passed through their entire /etc directory, thereby completely
+  breaking Python.) To fix this, `override
+  <https://docs.docker.com/compose/compose-file/compose-file-v3/#command>`_ the
+  image's default command with something like ``-v /etc/myconfig/mailrise.conf``
+  so you can passthrough the ``myconfig`` directory without interfering with the
+  rest of the filesystem.
+* TrueNAS SCALE runs containers as root by default. This breaks Mailrise, which
+  is designed to run as a non-root container for enhanced security. Ensure the
+  container is running as user ``999`` and group ``999``.
+
 
 From PyPI
 ---------
 
 You can find Mailrise `on PyPI <https://pypi.org/project/mailrise/>`_. The
 minimum Python version is 3.8+.
 
@@ -199,14 +195,19 @@
                                                   `uses <https://github.com/caronc/apprise/wiki/Development_API#notify--send-notifications>`_
                                                   this information to determine whether or not the upstream notification
                                                   service can handle the provided content.
 
                                                   If not specified here, the data type is inferred from the body part of the
                                                   email message. So if you have your body template set to anything but the
                                                   default value of ``$body``, you might want to set a data type here.
+import_code                            string     Allows advanced users to supply their own Python code to replace key
+                                                  components of Mailrise. Place the path to the Python source file here.
+                                                  See "Custom routers and authenticators" below. Custom routers ignore any
+                                                  data in the ``configs`` section, and custom authenticators ignore any
+                                                  data in the ``smtp.auth`` section.
 listen.host                            string     Specifies the network address to listen on.
 
                                                   Defaults to all interfaces.
 listen.port                            number     Specifies the network port to listen on.
 
                                                   Defaults to 8025.
 tls.mode                               string     Selects the operating mode for TLS encryption. Must be ``off``,
@@ -280,15 +281,15 @@
         urls:
           - hasio://HOST/ACCESS_TOKEN
 
       # You can send to this config with "telegram_and_discord@mailrise.xyz".
       #
       telegram_and_discord:
         urls:
-          - tgam://MY_BOT_TOKEN
+          - tgram://MY_BOT_TOKEN
           - discord://WEBHOOK_ID/WEBHOOK_TOKEN
         # You can also control the layout of the message with custom template
         # strings.
         mailrise:
           title_template: "Urgent: ${body}"
           body_template: ""
           body_format: text
@@ -383,7 +384,27 @@
 
     certificatesResolvers:
       letsencrypt:
         # ...
 
 SMTP clients can then connect to my.public.mailrise.domain.com, on port 465,
 using the TLS-on-connect mode.
+
+Custom routers and authenticators
+---------------------------------
+
+If you are handy with Python and want to overcome the limitations of the
+configuration format, you can replace Mailrise's notification
+routing and SMTP authentication logic with your own. Use the ``import_code``
+directive in your configuration file with the path to a Python source file.
+
+The router class, if provided, should be stored in a module-level variable named
+``router``. The authenticator callback, if provided, should be stored in a
+module-level variable named ``authenticator``.
+
+For further details, refer to the
+`sample file used for testing
+<https://github.com/YoRyan/mailrise/blob/main/tests/noop_pluggable.py>`_, the
+`Mailrise router API
+<https://github.com/YoRyan/mailrise/blob/main/src/mailrise/router.py>`_, and
+the `aiosmtpd authenticator callback
+<https://aiosmtpd.readthedocs.io/en/latest/auth.html#authenticator-callback>`_.
```

### Comparing `mailrise-1.3.0/README.rst` & `mailrise-1.4.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,32 @@
+Metadata-Version: 2.1
+Name: mailrise
+Version: 1.4.0
+Summary: An SMTP gateway for Apprise notifications.
+Home-page: https://mailrise.xyz
+Author: Ryan Young
+Author-email: ryan@youngryan.com
+License: MIT
+Project-URL: Documentation, https://pyscaffold.org/
+Platform: any
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Topic :: Communications :: Email
+Classifier: Environment :: No Input/Output (Daemon)
+Classifier: Intended Audience :: System Administrators
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Microsoft :: Windows
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst; charset=UTF-8
+Provides-Extra: testing
+License-File: LICENSE.txt
+License-File: AUTHORS.rst
+
 .. image:: https://raw.githubusercontent.com/YoRyan/mailrise/main/src/mailrise/asset/mailrise-logo.png
   :alt: Mailrise logo
 
 
 ========
 mailrise
 ========
@@ -37,15 +62,15 @@
 
 Just as email brought written messages into the 21st century, Mailrise
 brings email notifications into the year 2021 and beyond. Compared to a
 conventional SMTP server, it's more secure, too—no more replicating your Gmail
 password to each of your Linux boxes!
 
     "After a few very negative experiences with mail providers and their
-    detection of spam accounts in the last year... Fuck email. I will never set
+    detection of spam accounts in the last year... F––k email. I will never set
     up a mail account for notifications. And with Mailrise I don't have to
     anymore!"
 
     -- `u/Sarcism <https://www.reddit.com/r/selfhosted/comments/wwx0ue/comment/ilnqhkf/>`_
 
 A Mailrise daemon is configured with a list of Apprise
 `configuration files <https://github.com/caronc/apprise/wiki/config_yaml>`_.
@@ -87,15 +112,36 @@
 ============
 
 As a Docker container
 ---------------------
 
 An official Docker image is available
 `from Docker Hub <https://hub.docker.com/r/yoryan/mailrise>`_. To use it, you
-must bind mount a configuration file to ``/etc/mailrise.conf``.
+must bind mount a configuration file to ``/etc/mailrise.conf``. This mount must
+be a *file*, not a directory, and it cannot override anything else in /etc.
+
+Notes for NAS users
+^^^^^^^^^^^^^^^^^^^
+
+Consumer NAS operating systems often conceal Docker's controls behind a GUI that
+is opaque and difficult to troubleshoot. There are some known gotchas when using
+Mailrise with one:
+
+* Unraid can only passthrough directories, not files, making it impossible to
+  bind mount the mailrise.conf file. (While attempting to do so, some users have
+  accidentally passed through their entire /etc directory, thereby completely
+  breaking Python.) To fix this, `override
+  <https://docs.docker.com/compose/compose-file/compose-file-v3/#command>`_ the
+  image's default command with something like ``-v /etc/myconfig/mailrise.conf``
+  so you can passthrough the ``myconfig`` directory without interfering with the
+  rest of the filesystem.
+* TrueNAS SCALE runs containers as root by default. This breaks Mailrise, which
+  is designed to run as a non-root container for enhanced security. Ensure the
+  container is running as user ``999`` and group ``999``.
+
 
 From PyPI
 ---------
 
 You can find Mailrise `on PyPI <https://pypi.org/project/mailrise/>`_. The
 minimum Python version is 3.8+.
 
@@ -174,14 +220,19 @@
                                                   `uses <https://github.com/caronc/apprise/wiki/Development_API#notify--send-notifications>`_
                                                   this information to determine whether or not the upstream notification
                                                   service can handle the provided content.
 
                                                   If not specified here, the data type is inferred from the body part of the
                                                   email message. So if you have your body template set to anything but the
                                                   default value of ``$body``, you might want to set a data type here.
+import_code                            string     Allows advanced users to supply their own Python code to replace key
+                                                  components of Mailrise. Place the path to the Python source file here.
+                                                  See "Custom routers and authenticators" below. Custom routers ignore any
+                                                  data in the ``configs`` section, and custom authenticators ignore any
+                                                  data in the ``smtp.auth`` section.
 listen.host                            string     Specifies the network address to listen on.
 
                                                   Defaults to all interfaces.
 listen.port                            number     Specifies the network port to listen on.
 
                                                   Defaults to 8025.
 tls.mode                               string     Selects the operating mode for TLS encryption. Must be ``off``,
@@ -255,15 +306,15 @@
         urls:
           - hasio://HOST/ACCESS_TOKEN
 
       # You can send to this config with "telegram_and_discord@mailrise.xyz".
       #
       telegram_and_discord:
         urls:
-          - tgam://MY_BOT_TOKEN
+          - tgram://MY_BOT_TOKEN
           - discord://WEBHOOK_ID/WEBHOOK_TOKEN
         # You can also control the layout of the message with custom template
         # strings.
         mailrise:
           title_template: "Urgent: ${body}"
           body_template: ""
           body_format: text
@@ -357,8 +408,28 @@
         address: ":465"
 
     certificatesResolvers:
       letsencrypt:
         # ...
 
 SMTP clients can then connect to my.public.mailrise.domain.com, on port 465,
-using the TLS-on-connect mode.
+using the TLS-on-connect mode.
+
+Custom routers and authenticators
+---------------------------------
+
+If you are handy with Python and want to overcome the limitations of the
+configuration format, you can replace Mailrise's notification
+routing and SMTP authentication logic with your own. Use the ``import_code``
+directive in your configuration file with the path to a Python source file.
+
+The router class, if provided, should be stored in a module-level variable named
+``router``. The authenticator callback, if provided, should be stored in a
+module-level variable named ``authenticator``.
+
+For further details, refer to the
+`sample file used for testing
+<https://github.com/YoRyan/mailrise/blob/main/tests/noop_pluggable.py>`_, the
+`Mailrise router API
+<https://github.com/YoRyan/mailrise/blob/main/src/mailrise/router.py>`_, and
+the `aiosmtpd authenticator callback
+<https://aiosmtpd.readthedocs.io/en/latest/auth.html#authenticator-callback>`_.
```

### Comparing `mailrise-1.3.0/docs/Makefile` & `mailrise-1.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mailrise-1.3.0/docs/conf.py` & `mailrise-1.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mailrise-1.3.0/docs/index.rst` & `mailrise-1.4.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `mailrise-1.3.0/setup.cfg` & `mailrise-1.4.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -25,28 +25,29 @@
 zip_safe = False
 packages = find_namespace:
 include_package_data = True
 package_dir = 
 	=src
 python_requires = >=3.8
 install_requires = 
-	apprise==1.2.0
-	aiosmtpd==1.4.3
+	apprise==1.4.5
+	aiosmtpd==1.4.4.post2
 	PyYAML==6.0
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
 [options.extras_require]
 testing = 
 	setuptools
 	types-PyYAML
 	pytest
+	pytest-asyncio
 	pytest-cov
 
 [options.entry_points]
 console_scripts = 
 	mailrise = mailrise.skeleton:run
 
 [tool:pytest]
```

### Comparing `mailrise-1.3.0/setup.py` & `mailrise-1.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `mailrise-1.3.0/src/mailrise/__init__.py` & `mailrise-1.4.0/src/mailrise/__init__.py`

 * *Files identical despite different names*

### Comparing `mailrise-1.3.0/src/mailrise/asset/homelab-diagram.png` & `mailrise-1.4.0/src/mailrise/asset/homelab-diagram.png`

 * *Files identical despite different names*

### Comparing `mailrise-1.3.0/src/mailrise/asset/homelab-diagram.svg` & `mailrise-1.4.0/src/mailrise/asset/homelab-diagram.svg`

 * *Files identical despite different names*

### Comparing `mailrise-1.3.0/src/mailrise/asset/mailrise-failure-128x128.ico` & `mailrise-1.4.0/src/mailrise/asset/mailrise-failure-128x128.ico`

 * *Files identical despite different names*

### Comparing `mailrise-1.3.0/src/mailrise/asset/mailrise-failure-128x128.png` & `mailrise-1.4.0/src/mailrise/asset/mailrise-failure-128x128.png`

 * *Files identical despite different names*

### Comparing `mailrise-1.3.0/src/mailrise/asset/mailrise-failure-256x256.png` & `mailrise-1.4.0/src/mailrise/asset/mailrise-failure-256x256.png`

 * *Files identical despite different names*

### Comparing `mailrise-1.3.0/src/mailrise/asset/mailrise-failure-32x32.png` & `mailrise-1.4.0/src/mailrise/asset/mailrise-failure-32x32.png`

 * *Files identical despite different names*

### Comparing `mailrise-1.3.0/src/mailrise/asset/mailrise-failure-72x72.png` & `mailrise-1.4.0/src/mailrise/asset/mailrise-failure-72x72.png`

 * *Files identical despite different names*

### Comparing `mailrise-1.3.0/src/mailrise/asset/mailrise-info-128x128.ico` & `mailrise-1.4.0/src/mailrise/asset/mailrise-info-128x128.ico`

 * *Files identical despite different names*

### Comparing `mailrise-1.3.0/src/mailrise/asset/mailrise-info-128x128.png` & `mailrise-1.4.0/src/mailrise/asset/mailrise-info-128x128.png`

 * *Files identical despite different names*

### Comparing `mailrise-1.3.0/src/mailrise/asset/mailrise-info-256x256.png` & `mailrise-1.4.0/src/mailrise/asset/mailrise-info-256x256.png`

 * *Files identical despite different names*

### Comparing `mailrise-1.3.0/src/mailrise/asset/mailrise-info-32x32.png` & `mailrise-1.4.0/src/mailrise/asset/mailrise-info-32x32.png`

 * *Files identical despite different names*

### Comparing `mailrise-1.3.0/src/mailrise/asset/mailrise-info-72x72.png` & `mailrise-1.4.0/src/mailrise/asset/mailrise-info-72x72.png`

 * *Files identical despite different names*

### Comparing `mailrise-1.3.0/src/mailrise/asset/mailrise-logo.png` & `mailrise-1.4.0/src/mailrise/asset/mailrise-logo.png`

 * *Files identical despite different names*

### Comparing `mailrise-1.3.0/src/mailrise/asset/mailrise-logo.svg` & `mailrise-1.4.0/src/mailrise/asset/mailrise-logo.svg`

 * *Files identical despite different names*

### Comparing `mailrise-1.3.0/src/mailrise/asset/mailrise-success-128x128.ico` & `mailrise-1.4.0/src/mailrise/asset/mailrise-success-128x128.ico`

 * *Files identical despite different names*

### Comparing `mailrise-1.3.0/src/mailrise/asset/mailrise-success-128x128.png` & `mailrise-1.4.0/src/mailrise/asset/mailrise-success-128x128.png`

 * *Files identical despite different names*

### Comparing `mailrise-1.3.0/src/mailrise/asset/mailrise-success-256x256.png` & `mailrise-1.4.0/src/mailrise/asset/mailrise-success-256x256.png`

 * *Files identical despite different names*

### Comparing `mailrise-1.3.0/src/mailrise/asset/mailrise-success-32x32.png` & `mailrise-1.4.0/src/mailrise/asset/mailrise-success-32x32.png`

 * *Files identical despite different names*

### Comparing `mailrise-1.3.0/src/mailrise/asset/mailrise-success-72x72.png` & `mailrise-1.4.0/src/mailrise/asset/mailrise-success-72x72.png`

 * *Files identical despite different names*

### Comparing `mailrise-1.3.0/src/mailrise/asset/mailrise-warning-128x128.ico` & `mailrise-1.4.0/src/mailrise/asset/mailrise-warning-128x128.ico`

 * *Files identical despite different names*

### Comparing `mailrise-1.3.0/src/mailrise/asset/mailrise-warning-128x128.png` & `mailrise-1.4.0/src/mailrise/asset/mailrise-warning-128x128.png`

 * *Files identical despite different names*

### Comparing `mailrise-1.3.0/src/mailrise/asset/mailrise-warning-256x256.png` & `mailrise-1.4.0/src/mailrise/asset/mailrise-warning-256x256.png`

 * *Files identical despite different names*

### Comparing `mailrise-1.3.0/src/mailrise/asset/mailrise-warning-32x32.png` & `mailrise-1.4.0/src/mailrise/asset/mailrise-warning-32x32.png`

 * *Files identical despite different names*

### Comparing `mailrise-1.3.0/src/mailrise/asset/mailrise-warning-72x72.png` & `mailrise-1.4.0/src/mailrise/asset/mailrise-warning-72x72.png`

 * *Files identical despite different names*

### Comparing `mailrise-1.3.0/src/mailrise/authenticator.py` & `mailrise-1.4.0/src/mailrise/basic_authenticator.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,29 @@
 """
 This is the authentication functionality for the SMTP server.
 """
 
 import typing as typ
 
-from aiosmtpd.smtp import AuthResult, Envelope, LoginPassword, Session, SMTP
+from aiosmtpd import smtp
 
 
 class BasicAuthenticator(typ.NamedTuple):
-    """A simple authenticator that uses a static username and password list.
-    """
+    """A simple authenticator that uses a static username and password list."""
     logins: typ.Mapping[str, str]
 
     # pylint: disable=too-many-arguments
-    def __call__(self, server: SMTP, session: Session, envelope: Envelope,
-                 mechanism: str, auth_data: LoginPassword):
-        fail_nothandled = AuthResult(success=False, handled=False)
+    def __call__(self, server: smtp.SMTP, session: smtp.Session,
+                 envelope: smtp.Envelope, mechanism: str, auth_data: typ.Any):
+        fail_nothandled = smtp.AuthResult(success=False, handled=False)
         if mechanism not in ("LOGIN", "PLAIN"):
             return fail_nothandled
-        if not isinstance(auth_data, LoginPassword):
+        if not isinstance(auth_data, smtp.LoginPassword):
             return fail_nothandled
 
         username = auth_data.login.decode("utf-8")
         password = auth_data.password.decode("utf-8")
         success = self.logins.get(username) == password
-        return AuthResult(success=success)
+        return smtp.AuthResult(success=success)
 
     def __str__(self) -> str:
         return f'Basic({len(self.logins)})'
-
-
-Authenticator = BasicAuthenticator
```

### Comparing `mailrise-1.3.0/src/mailrise/config.py` & `mailrise-1.4.0/src/mailrise/smtp.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,270 +1,236 @@
 """
-This is the YAML configuration parser for Mailrise.
+This is the SMTP server functionality for Mailrise.
 """
 
 from __future__ import annotations
 
-import io
+import asyncio
+import email.policy
 import os
 import typing as typ
-from enum import Enum
-from fnmatch import fnmatchcase
-from functools import partial
-from logging import Logger
-from string import Template
-from typing import NamedTuple
+from email import contentmanager
+from email.message import EmailMessage as StdlibEmailMessage
+from email.parser import BytesParser
+from tempfile import NamedTemporaryFile
 
 import apprise
-import yaml
-from apprise.common import NotifyType
+from aiosmtpd.smtp import Envelope, Session, SMTP
+from apprise.common import ContentLocation
 
-from mailrise.authenticator import Authenticator, BasicAuthenticator
-from mailrise.util import parseaddrparts
+from mailrise.config import MailriseConfig
+import mailrise.router as r
 
+# Mypy, for some reason, considers AttachBase a module, not a class.
+MYPY = False
+# pylint: disable=ungrouped-imports
+if MYPY:
+    from apprise.attachment.AttachBase import AttachBase
+else:
+    from apprise.attachment import AttachBase
 
-DEFAULT_ASSET = apprise.AppriseAsset(
-    app_id='Mailrise',
-    app_desc='Mailrise SMTP Notification Relay',
-    app_url='https://mailrise.xyz',
-    html_notify_map={
-        NotifyType.INFO: '#2e6e99',
-        NotifyType.SUCCESS: '#2e992e',
-        NotifyType.WARNING: '#99972e',
-        NotifyType.FAILURE: '#993a2e'
-    },
-    theme=None,
-    default_extension='.png',
-    image_url_mask='https://raw.githubusercontent.com/YoRyan/mailrise/main/'
-                   'src/mailrise/asset/mailrise-{TYPE}-{XY}{EXTENSION}',
-    image_url_logo='https://raw.githubusercontent.com/YoRyan/mailrise/main/'
-                   'src/mailrise/asset/mailrise-logo.png',
-    image_path_mask=os.path.abspath(
-        os.path.join(
-            os.path.dirname(__file__),
-            'asset',
-            'mailrise-{TYPE}-{XY}{EXTENSION}'
-        )
-    )
-)
-
-
-class ConfigFileLoader(yaml.FullLoader):  # pylint: disable=too-many-ancestors
-    """Our YAML loader class, which comes with an attached logger."""
-    logger: Logger
 
-    def __init__(self, stream, logger: Logger) -> None:
-        super().__init__(stream)
-        self.logger = logger
-        self.add_constructor('!env_var', ConfigFileLoader._env_var_constructor)
+class AppriseNotifyFailure(Exception):
+    """Exception raised when Apprise fails to deliver a notification.
 
-    @staticmethod
-    def _env_var_constructor(loader: ConfigFileLoader, node: yaml.nodes.Node) -> str:
-        """Load environment variables and embed them into the configuration YAML."""
-        value = str(node.value)
-        try:
-            env, default = value.split(maxsplit=1)
-        except ValueError:
-            env, default = value, None
-
-        if env in os.environ:
-            return os.environ[env]
-        if default:
-            loader.logger.warning(
-                'Environment variable %s not defined, using default value: %s',
-                env, default)
-            return default
-        raise ConfigFileError(
-            f'Environment variable {env} not defined and no default value provided')
+    Note: Apprise does not provide any information about the reason for the
+    failure.
+    """
 
 
-class ConfigFileError(Exception):
-    """Exception raised for invalid configuration files.
+class UnreadableMultipart(Exception):
+    """Exception raised for multipart messages that can't be parsed.
 
     Attributes:
-        message: The reason the configuration file is invalid.
+        message: The multipart email part.
     """
-    message: str
+    message: StdlibEmailMessage
 
-    def __init__(self, message: str) -> None:
+    def __init__(self, message: StdlibEmailMessage) -> None:
         super().__init__(self)
         self.message = message
 
 
-class TLSMode(Enum):
-    """Specifies a TLS encryption operating mode."""
-    OFF = 'no TLS'
-    ONCONNECT = 'TLS on connect'
-    STARTTLS = 'STARTTLS, optional'
-    STARTTLSREQUIRE = 'STARTTLS, required'
-
-
-class Key(NamedTuple):
-    """A unique identifier for a sender target.
+class AppriseHandler(typ.NamedTuple):
+    """The aiosmtpd handler for Mailrise. Dispatches Apprise notifications.
 
     Attributes:
-        user: The user portion of the recipient address.
-        domain: The domain portion of the recipient address, which defaults
-            to "mailrise.xyz".
+        config: This server's Mailrise configuration.
     """
-    user: str
-    domain: str = 'mailrise.xyz'
-
-    def __str__(self) -> str:
-        return f'{self.user}@{self.domain}'
+    config: MailriseConfig
 
-    def as_configured(self) -> str:
-        """Drop the domain part of this identifier if it is 'mailrise.xyz'."""
-        return self.user if self.domain == 'mailrise.xyz' else str(self)
+    # pylint: disable=invalid-name,unused-argument,too-many-arguments
+    async def handle_RCPT(self, server: SMTP, session: Session, envelope: Envelope,
+                          address: str, rcpt_options: list[str]) -> str:
+        """Called during RCPT TO."""
+        self.config.logger.info('Added recipient: %s', address)
+        envelope.rcpt_tos.append(address)
+        return '250 OK'
+
+    # pylint: disable=invalid-name,unused-argument
+    async def handle_DATA(self, server: SMTP, session: Session, envelope: Envelope) \
+            -> str:
+        """Called during DATA after the entire message ('SMTP content' as described
+        in RFC 5321) has been received."""
+        assert isinstance(envelope.content, bytes)
+        parser = BytesParser(policy=email.policy.default)
+        message = parser.parsebytes(envelope.content)
+        assert isinstance(message, StdlibEmailMessage)
+        try:
+            notification = _parsemessage(message, envelope)
+        except UnreadableMultipart as mpe:
+            subparts = \
+                ' '.join(part.get_content_type() for part in mpe.message.iter_parts())
+            self.config.logger.error('Failed to parse %s message: [ %s ]',
+                                     mpe.message.get_content_type(), subparts)
+        self.config.logger.info('Accepted email, subject: %s', notification.subject)
 
+        try:
+            to_send = [data async for data in self.config.router.email_to_apprise(
+                           logger=self.config.logger,
+                           email=notification,
+                           auth_data=session.auth_data
+                       )]
+        except Exception as exc:  # pylint: disable=broad-except
+            return f'450 router had internal exception: {exc}'
+
+        results = await asyncio.gather(
+            *(_apprise_notify(self.config, data) for data in to_send),
+            return_exceptions=True
+        )
+        if any(isinstance(result, AppriseNotifyFailure) for result in results):
+            addresses = ' '.join(envelope.rcpt_tos)
+            self.config.logger.warning('Notification failed: %s ➤ %s',
+                                       notification.subject, addresses)
+            return '450 failed to send notification'
 
-class Sender(NamedTuple):
-    """A configured target for Apprise notifications.
+        return '250 OK'
 
-    Attributes:
-        notifier: The Apprise instance.
-        title_template: The template string for notification title texts.
-        body_template: The template string for notification body texts.
-        body_format: The content type for notifications. If None, this will be
-            auto-detected from the body parts of emails.
-    """
-    notifier: apprise.Apprise
-    title_template: Template
-    body_template: Template
-    body_format: typ.Optional[apprise.NotifyFormat]
 
+def _parsemessage(msg: StdlibEmailMessage, envelope: Envelope) -> r.EmailMessage:
+    """Parses an email message into an `EmailNotification`.
 
-class MailriseConfig(NamedTuple):
-    """Configuration data for a Mailrise instance.
+    Args:
+        msg: The email message.
 
-    Attributes:
-        logger: The logger, which is used to record interesting events.
-        listen_host: The network address to listen on.
-        listen_port: The network port to listen on.
-        tls_mode: The TLS encryption mode.
-        tls_certfile: The path to the TLS certificate chain file.
-        tls_keyfile: The path to the TLS key file.
-        smtp_hostname: The advertised SMTP server hostname.
-        senders: A list of notification targets, each with a [key, sender]
-            tuple, where key contains username and domain patterns that can be
-            matched by fnmatch and sender is the Sender instance itself.
+    Returns:
+        The `EmailNotification` instance.
     """
-    logger: Logger
-    listen_host: str
-    listen_port: int
-    tls_mode: TLSMode
-    tls_certfile: typ.Optional[str]
-    tls_keyfile: typ.Optional[str]
-    smtp_hostname: typ.Optional[str]
-    senders: list[typ.Tuple[Key, Sender]]
-    authenticator: typ.Optional[Authenticator]
-
-    def get_sender(self, key: Key) -> Sender | None:
-        """Find a sender by recipient key."""
-        return next(
-            (sender for (pattern_key, sender) in self.senders
-             if fnmatchcase(key.user, pattern_key.user)
-             and fnmatchcase(key.domain, pattern_key.domain)), None)
+    py_body_part = msg.get_body()
+    body: typ.Optional[tuple[str, apprise.NotifyFormat]]
+    if isinstance(py_body_part, StdlibEmailMessage):
+        body_part: StdlibEmailMessage
+        try:
+            py_body_part.get_content()
+        except KeyError:  # stdlib failed to read the content, which means multipart
+            body_part = _getmultiparttext(py_body_part)
+        else:
+            body_part = py_body_part
+        body_content = contentmanager.raw_data_manager.get_content(body_part)
+        is_html = body_part.get_content_subtype() == 'html'
+        body = (body_content.strip(),
+                apprise.NotifyFormat.HTML if is_html else apprise.NotifyFormat.TEXT)
+    else:
+        body = None
+    attachments = [_parseattachment(part) for part in msg.iter_attachments()
+                   if isinstance(part, StdlibEmailMessage)]
+    return r.EmailMessage(
+        email_message=msg,
+        subject=msg.get('Subject', '[no subject]'),
+        from_=msg.get('From', '[no sender]'),
+        to=envelope.rcpt_tos,
+        # Apprise will fail if no body is supplied.
+        body=body[0] if body else '[no body]',
+        body_format=body[1] if body else apprise.NotifyFormat.TEXT,
+        attachments=attachments
+    )
 
 
-def load_config(logger: Logger, file: io.TextIOWrapper) -> MailriseConfig:
-    """Loads configuration data from a YAML file.
+def _getmultiparttext(msg: StdlibEmailMessage) -> StdlibEmailMessage:
+    """Search for the textual body part of a multipart email."""
+    content_type = msg.get_content_type()
+    if content_type in ('multipart/related', 'multipart/alternative'):
+        parts = list(msg.iter_parts())
+        # Look for these types of parts in descending order.
+        for parttype in ('multipart/alternative', 'multipart/related',
+                         'text/html', 'text/plain'):
+            found = \
+                next((p for p in parts if isinstance(p, StdlibEmailMessage)
+                     and p.get_content_type() == parttype), None)
+            if found is not None:
+                return _getmultiparttext(found)
+        raise UnreadableMultipart(msg)
+    return msg
+
+
+def _parseattachment(part: StdlibEmailMessage) -> r.EmailAttachment:
+    return r.EmailAttachment(data=part.get_content(), filename=part.get_filename(''))
+
+
+async def _apprise_notify(config: MailriseConfig, data: r.AppriseNotification):
+    ap_config = apprise.AppriseConfig(asset=data.asset or r.DEFAULT_ASSET)
+    ap_config.add_config(data.config, format=data.config_format)
+    ap_instance = apprise.Apprise(ap_config)
+
+    attach_base = [_AttachMailrise(config, attach) for attach in data.attachments]
+    success = await ap_instance.async_notify(
+        title=data.title,
+        body=data.body,
+        body_format=data.body_format,
+        notify_type=data.notify_type,
+        attach=attach_base
+    )
+    # NOTE: This should probably be called by Apprise itself, but it isn't?
+    for base in attach_base:
+        base.invalidate()
+    if not success:
+        raise AppriseNotifyFailure
 
-    Args:
-        logger: The logger, which will be passed to the `MailriseConfig` instance.
-        file: The file handle to load YAML from.
 
-    Returns:
-        The `MailriseConfig` instance.
+class _AttachMailrise(AttachBase):
+    """An Apprise attachment type that wraps `Attachment`.
 
-    Raises:
-        ConfigFileError: The configuration file is invalid.
-    """
-    yml = yaml.load(file, Loader=partial(ConfigFileLoader, logger=logger))
-    if not isinstance(yml, dict):
-        raise ConfigFileError("root node not a mapping")
-
-    yml_listen = yml.get('listen', {})
-
-    yml_tls = yml.get('tls', {})
-    try:
-        tls_mode = TLSMode[yml_tls.get('mode', 'off').upper()]
-    except KeyError as key_err:
-        raise ConfigFileError('invalid TLS operating mode') from key_err
-    tls_certfile = yml_tls.get('certfile', None)
-    tls_keyfile = yml_tls.get('keyfile', None)
-    if tls_mode != TLSMode.OFF and not (tls_certfile and tls_keyfile):
-        raise ConfigFileError(
-            'TLS enabled, but certificate and key files not specified')
-
-    yml_smtp = yml.get('smtp', {})
-
-    yml_configs = yml.get('configs', [])
-    if not isinstance(yml_configs, dict):
-        raise ConfigFileError("'configs' node not a mapping")
-    senders = [(_parsekey(key), _load_sender(config))
-               for key, config in yml_configs.items()]
-
-    logger.info('Loaded configuration with %d recipient(s)', len(senders))
-    return MailriseConfig(
-        logger=logger,
-        listen_host=yml_listen.get('host', ''),
-        listen_port=yml_listen.get('port', 8025),
-        tls_mode=tls_mode,
-        tls_certfile=tls_certfile,
-        tls_keyfile=tls_keyfile,
-        smtp_hostname=yml_smtp.get('hostname', None),
-        senders=senders,
-        authenticator=_load_authenticator(yml_smtp.get('auth', {}))
-    )
+    Data is stored in temporary files for upload.
 
+    Args:
+        config: The Mailrise configuration to use.
+        attach: The `Attachment` instance.
+    """
+    location = ContentLocation.LOCAL
 
-def _parsekey(key: str) -> Key:
-    def err():
-        return ConfigFileError(f"invalid config key '{key}'; should be a string or "
-                               "an email address without periods in the username")
-    if '@' in key:
-        user, domain = parseaddrparts(key)
-        if not user or not domain or '.' in user:
-            raise err()
-        return Key(user=user, domain=domain.lower())
-    if '.' in key:
-        raise err()
-
-    return Key(user=key)
-
-
-def _load_sender(config: dict[str, typ.Any]) -> Sender:
-    if not isinstance(config, dict):
-        raise ConfigFileError("apprise config node not a mapping")
-
-    # Extract Mailrise-specific values.
-    mr_config = config.get('mailrise', {})
-    config.pop('mailrise', None)
-    title_template = mr_config.get('title_template', '$subject ($from)')
-    body_template = mr_config.get('body_template', '$body')
-    body_format = mr_config.get('body_format', None)
-    if not any(body_format == c for c in (None,
-                                          apprise.NotifyFormat.TEXT,
-                                          apprise.NotifyFormat.HTML,
-                                          apprise.NotifyFormat.MARKDOWN)):
-        raise ConfigFileError(f"invalid apprise notification format: {body_format}")
-
-    aconfig = apprise.AppriseConfig(asset=DEFAULT_ASSET)
-    aconfig.add_config(yaml.safe_dump(config), format='yaml')
-    apobj = apprise.Apprise(aconfig)
-
-    return Sender(
-        notifier=apobj,
-        title_template=Template(title_template),
-        body_template=Template(body_template),
-        body_format=body_format
-    )
+    _mrfile = None  # Satisfy mypy by initializing as an Optional.
 
+    def __init__(self, config: MailriseConfig,
+                 attach: r.EmailAttachment, **kwargs: typ.Any) -> None:
+        super().__init__(**kwargs)
+        self._mrconfig = config
+        self._mrattach = attach
+
+    def download(self) -> bool:
+        self.invalidate()
+
+        with NamedTemporaryFile(delete=False) as tfile:
+            tfile.write(self._mrattach.data)
+        self._mrfile = tfile
+        self.download_path = tfile.name
+        self.detected_name = self._mrattach.filename
+
+        return True  # Indicates the "download" was successful.
+
+    def invalidate(self) -> None:
+        tfile = self._mrfile
+        if tfile:
+            try:
+                os.remove(tfile.name)
+            except (FileNotFoundError, OSError):
+                self._mrconfig.logger.info(
+                    'Failed to delete attachment file: %s', tfile.name)
+            self._mrfile = None
+        super().invalidate()
 
-def _load_authenticator(config: dict[str, typ.Any]) -> typ.Optional[Authenticator]:
-    if 'basic' in config and isinstance(config['basic'], dict):
-        logins = {str(username): str(password)
-                  for username, password in config['basic'].items()}
-        return BasicAuthenticator(logins=logins)
+    def url(self, *args: typ.Any, **kwargs: typ.Any) -> str:
+        return f'mailrise://{hex(id(self))}'
 
-    return None
+    @staticmethod
+    def parse_url(url: str, verify_host: bool = True,
+                  mimetype_db: typ.Any = None) -> typ.Dict[str, typ.Any]:
+        return {}
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mailrise-1.3.0/src/mailrise/skeleton.py` & `mailrise-1.4.0/src/mailrise/skeleton.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import typing as typ
 from asyncio.events import new_event_loop
 from functools import partial
 
 from aiosmtpd.controller import UnthreadedController
 
 from mailrise import __version__
-from mailrise.config import ConfigFileError, TLSMode, load_config
+from mailrise.config import TLSMode, load_config
 from mailrise.smtp import AppriseHandler
 
 __author__ = "Ryan Young"
 __copyright__ = "Ryan Young"
 __license__ = "MIT"
 
 _logger = logging.getLogger(__name__)
@@ -100,23 +100,15 @@
     Args:
       args (List[str]): command line parameters as list of strings
           (for example  ``["--verbose", "42"]``).
     """
     pargs = parse_args(args)
     setup_logging(pargs.loglevel)
 
-    try:
-        config = load_config(_logger, pargs.config)
-    except ConfigFileError as err:
-        _logger.critical('Error loading configuration file: %s', err.message)
-        return
-    if len(config.senders) < 1:
-        _logger.critical('Error loading configuration file: '
-                         'there are no Apprise configs')
-        return
+    config = load_config(_logger, pargs.config)
 
     tls: typ.Optional[ssl.SSLContext] = None
     tls_mode = config.tls_mode
     if tls_mode != TLSMode.OFF:
         assert isinstance(config.tls_certfile, str)
         assert isinstance(config.tls_keyfile, str)
         tls = ssl.create_default_context(ssl.Purpose.CLIENT_AUTH)
@@ -151,16 +143,22 @@
     eloop = new_event_loop()
     controller = makecon(loop=eloop)
 
     def clean_exit():
         _logger.info('Caught exit signal...')
         eloop.stop()
         controller.end()
-    for sig in (signal.SIGINT, signal.SIGTERM):
-        eloop.add_signal_handler(sig, clean_exit)
+
+    try:
+        for sig in (signal.SIGINT, signal.SIGTERM):
+            eloop.add_signal_handler(sig, clean_exit)
+    except NotImplementedError:
+        # add_signal_handler() is exclusive to Unix. No big deal if we can't set
+        # up a handler.
+        pass
 
     controller.begin()
     eloop.run_forever()
 
 
 def run() -> None:
     """Calls :func:`main` passing the CLI arguments extracted from :obj:`sys.argv`.
```

### Comparing `mailrise-1.3.0/src/mailrise.egg-info/PKG-INFO` & `mailrise-1.4.0/src/mailrise.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mailrise
-Version: 1.3.0
+Version: 1.4.0
 Summary: An SMTP gateway for Apprise notifications.
 Home-page: https://mailrise.xyz
 Author: Ryan Young
 Author-email: ryan@youngryan.com
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
@@ -62,15 +62,15 @@
 
 Just as email brought written messages into the 21st century, Mailrise
 brings email notifications into the year 2021 and beyond. Compared to a
 conventional SMTP server, it's more secure, too—no more replicating your Gmail
 password to each of your Linux boxes!
 
     "After a few very negative experiences with mail providers and their
-    detection of spam accounts in the last year... Fuck email. I will never set
+    detection of spam accounts in the last year... F––k email. I will never set
     up a mail account for notifications. And with Mailrise I don't have to
     anymore!"
 
     -- `u/Sarcism <https://www.reddit.com/r/selfhosted/comments/wwx0ue/comment/ilnqhkf/>`_
 
 A Mailrise daemon is configured with a list of Apprise
 `configuration files <https://github.com/caronc/apprise/wiki/config_yaml>`_.
@@ -112,15 +112,36 @@
 ============
 
 As a Docker container
 ---------------------
 
 An official Docker image is available
 `from Docker Hub <https://hub.docker.com/r/yoryan/mailrise>`_. To use it, you
-must bind mount a configuration file to ``/etc/mailrise.conf``.
+must bind mount a configuration file to ``/etc/mailrise.conf``. This mount must
+be a *file*, not a directory, and it cannot override anything else in /etc.
+
+Notes for NAS users
+^^^^^^^^^^^^^^^^^^^
+
+Consumer NAS operating systems often conceal Docker's controls behind a GUI that
+is opaque and difficult to troubleshoot. There are some known gotchas when using
+Mailrise with one:
+
+* Unraid can only passthrough directories, not files, making it impossible to
+  bind mount the mailrise.conf file. (While attempting to do so, some users have
+  accidentally passed through their entire /etc directory, thereby completely
+  breaking Python.) To fix this, `override
+  <https://docs.docker.com/compose/compose-file/compose-file-v3/#command>`_ the
+  image's default command with something like ``-v /etc/myconfig/mailrise.conf``
+  so you can passthrough the ``myconfig`` directory without interfering with the
+  rest of the filesystem.
+* TrueNAS SCALE runs containers as root by default. This breaks Mailrise, which
+  is designed to run as a non-root container for enhanced security. Ensure the
+  container is running as user ``999`` and group ``999``.
+
 
 From PyPI
 ---------
 
 You can find Mailrise `on PyPI <https://pypi.org/project/mailrise/>`_. The
 minimum Python version is 3.8+.
 
@@ -199,14 +220,19 @@
                                                   `uses <https://github.com/caronc/apprise/wiki/Development_API#notify--send-notifications>`_
                                                   this information to determine whether or not the upstream notification
                                                   service can handle the provided content.
 
                                                   If not specified here, the data type is inferred from the body part of the
                                                   email message. So if you have your body template set to anything but the
                                                   default value of ``$body``, you might want to set a data type here.
+import_code                            string     Allows advanced users to supply their own Python code to replace key
+                                                  components of Mailrise. Place the path to the Python source file here.
+                                                  See "Custom routers and authenticators" below. Custom routers ignore any
+                                                  data in the ``configs`` section, and custom authenticators ignore any
+                                                  data in the ``smtp.auth`` section.
 listen.host                            string     Specifies the network address to listen on.
 
                                                   Defaults to all interfaces.
 listen.port                            number     Specifies the network port to listen on.
 
                                                   Defaults to 8025.
 tls.mode                               string     Selects the operating mode for TLS encryption. Must be ``off``,
@@ -280,15 +306,15 @@
         urls:
           - hasio://HOST/ACCESS_TOKEN
 
       # You can send to this config with "telegram_and_discord@mailrise.xyz".
       #
       telegram_and_discord:
         urls:
-          - tgam://MY_BOT_TOKEN
+          - tgram://MY_BOT_TOKEN
           - discord://WEBHOOK_ID/WEBHOOK_TOKEN
         # You can also control the layout of the message with custom template
         # strings.
         mailrise:
           title_template: "Urgent: ${body}"
           body_template: ""
           body_format: text
@@ -383,7 +409,27 @@
 
     certificatesResolvers:
       letsencrypt:
         # ...
 
 SMTP clients can then connect to my.public.mailrise.domain.com, on port 465,
 using the TLS-on-connect mode.
+
+Custom routers and authenticators
+---------------------------------
+
+If you are handy with Python and want to overcome the limitations of the
+configuration format, you can replace Mailrise's notification
+routing and SMTP authentication logic with your own. Use the ``import_code``
+directive in your configuration file with the path to a Python source file.
+
+The router class, if provided, should be stored in a module-level variable named
+``router``. The authenticator callback, if provided, should be stored in a
+module-level variable named ``authenticator``.
+
+For further details, refer to the
+`sample file used for testing
+<https://github.com/YoRyan/mailrise/blob/main/tests/noop_pluggable.py>`_, the
+`Mailrise router API
+<https://github.com/YoRyan/mailrise/blob/main/src/mailrise/router.py>`_, and
+the `aiosmtpd authenticator callback
+<https://aiosmtpd.readthedocs.io/en/latest/auth.html#authenticator-callback>`_.
```

### Comparing `mailrise-1.3.0/src/mailrise.egg-info/SOURCES.txt` & `mailrise-1.4.0/src/mailrise.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -2,43 +2,45 @@
 .gitattributes
 .gitignore
 .readthedocs.yml
 AUTHORS.rst
 CHANGELOG.rst
 CONTRIBUTING.rst
 Dockerfile
-Dockerfile.buster
 LICENSE.txt
 README.rst
 pyproject.toml
 setup.cfg
 setup.py
 tox.ini
 .devcontainer/Dockerfile
 .devcontainer/devcontainer.json
 .github/dependabot.yml
+.github/actions/docker-build/action.yml
 .github/workflows/codeql-analysis.yml
 .github/workflows/docker-hub.yml
+.github/workflows/github-packages.yml
 docs/Makefile
 docs/authors.rst
 docs/changelog.rst
 docs/conf.py
 docs/contributing.rst
 docs/index.rst
 docs/license.rst
 docs/readme.rst
 docs/requirements.txt
 docs/_static/.gitignore
 src/mailrise/__init__.py
-src/mailrise/authenticator.py
+src/mailrise/basic_authenticator.py
 src/mailrise/config.py
 src/mailrise/py.typed
+src/mailrise/router.py
+src/mailrise/simple_router.py
 src/mailrise/skeleton.py
 src/mailrise/smtp.py
-src/mailrise/util.py
 src/mailrise.egg-info/PKG-INFO
 src/mailrise.egg-info/SOURCES.txt
 src/mailrise.egg-info/dependency_links.txt
 src/mailrise.egg-info/entry_points.txt
 src/mailrise.egg-info/not-zip-safe
 src/mailrise.egg-info/requires.txt
 src/mailrise.egg-info/top_level.txt
@@ -64,9 +66,12 @@
 src/mailrise/asset/mailrise-warning-128x128.ico
 src/mailrise/asset/mailrise-warning-128x128.png
 src/mailrise/asset/mailrise-warning-256x256.png
 src/mailrise/asset/mailrise-warning-32x32.png
 src/mailrise/asset/mailrise-warning-72x72.png
 tests/bridge.jpg
 tests/conftest.py
+tests/noop_pluggable.py
 tests/test_config.py
+tests/test_importer.py
+tests/test_simple_router.py
 tests/test_smtp.py
```

### Comparing `mailrise-1.3.0/tests/bridge.jpg` & `mailrise-1.4.0/tests/bridge.jpg`

 * *Files identical despite different names*

### Comparing `mailrise-1.3.0/tests/test_config.py` & `mailrise-1.4.0/tests/test_config.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,37 +2,38 @@
 Tests for configuration loading.
 """
 
 import logging
 from io import StringIO
 
 import pytest
-from apprise import NotifyFormat
+from apprise import Apprise, AppriseConfig, NotifyFormat
 from pytest import MonkeyPatch
 
-from mailrise.authenticator import BasicAuthenticator
-from mailrise.config import ConfigFileError, Key, load_config
+from mailrise.basic_authenticator import BasicAuthenticator
+from mailrise.config import load_config
+from mailrise.simple_router import _Key, SimpleRouter
 
 
 _logger = logging.getLogger(__name__)
 
 
 def test_errors() -> None:
     """Tests for :fun:`load_config`'s failure conditions."""
-    with pytest.raises(ConfigFileError):
+    with pytest.raises(SystemExit):
         file = StringIO("""
             24
         """)
         load_config(_logger, file)
-    with pytest.raises(ConfigFileError):
+    with pytest.raises(SystemExit):
         file = StringIO("""
             configs: 24
         """)
         load_config(_logger, file)
-    with pytest.raises(ConfigFileError):
+    with pytest.raises(SystemExit):
         file = StringIO("""
             configs:
               test: 24
         """)
         load_config(_logger, file)
 
 
@@ -41,45 +42,51 @@
     file = StringIO("""
         configs:
           test:
             urls:
               - json://localhost
     """)
     mrise = load_config(_logger, file)
-    assert len(mrise.senders) == 1
-    key = Key(user='test')
+    router = mrise.router
+    assert isinstance(router, SimpleRouter)
+    assert len(router.senders) == 1
+    key = _Key(user='test')
     assert mrise.authenticator is None
 
-    sender = mrise.get_sender(key)
+    sender = router.get_sender(key)
     assert sender is not None
-    assert len(sender.notifier) == 1
-    assert sender.notifier[0].url().startswith('json://localhost/')
+    notifier = _make_notifier(sender.config_yaml)
+    assert len(notifier) == 1
+    assert notifier[0].url().startswith('json://localhost/')
 
 
 def test_multi_load() -> None:
     """Tests a sucessful load with :fun:`load_config` with multiple configs."""
     file = StringIO("""
         configs:
           test1:
             urls:
               - json://localhost
           test2:
             urls:
               - json://localhost
     """)
     mrise = load_config(_logger, file)
-    assert len(mrise.senders) == 2
+    router = mrise.router
+    assert isinstance(router, SimpleRouter)
+    assert len(router.senders) == 2
 
     for user in ('test1', 'test2'):
-        key = Key(user=user)
+        key = _Key(user=user)
 
-        sender = mrise.get_sender(key)
+        sender = router.get_sender(key)
         assert sender is not None
-        assert len(sender.notifier) == 1
-        assert sender.notifier[0].url().startswith('json://localhost/')
+        notifier = _make_notifier(sender.config_yaml)
+        assert len(notifier) == 1
+        assert notifier[0].url().startswith('json://localhost/')
 
 
 def test_mailrise_options() -> None:
     """Tests a successful load with :fun:`load_config` with Mailrise-specific
     options."""
     file = StringIO("""
         configs:
@@ -87,101 +94,111 @@
             urls:
               - json://localhost
             mailrise:
               title_template: ""
               body_format: "text"
     """)
     mrise = load_config(_logger, file)
-    assert len(mrise.senders) == 1
-    key = Key(user='test')
+    router = mrise.router
+    assert isinstance(router, SimpleRouter)
+    assert len(router.senders) == 1
+    key = _Key(user='test')
 
-    sender = mrise.get_sender(key)
+    sender = router.get_sender(key)
     assert sender is not None
     assert sender.title_template.template == ''
     assert sender.body_format == NotifyFormat.TEXT
 
-    with pytest.raises(ConfigFileError):
+    with pytest.raises(SystemExit):
         file = StringIO("""
             configs:
               test:
                 urls:
                   - json://localhost
                 mailrise:
                   body_format: "BAD"
         """)
         load_config(_logger, file)
 
 
 def test_config_keys() -> None:
     """Tests the config key parser with both string and full email formats."""
-    with pytest.raises(ConfigFileError):
+    with pytest.raises(SystemExit):
         file = StringIO("""
             configs:
               has.periods:
                 urls:
                   - json://localhost
         """)
         load_config(_logger, file)
-    with pytest.raises(ConfigFileError):
+    with pytest.raises(SystemExit):
         file = StringIO("""
             configs:
               bademail@:
                 urls:
                   - json://localhost
         """)
         load_config(_logger, file)
     file = StringIO("""
         configs:
           user@example.com:
             urls:
               - json://localhost
     """)
     mrise = load_config(_logger, file)
-    assert len(mrise.senders) == 1
-    key = Key(user='user', domain='example.com')
-    assert mrise.get_sender(key) is not None
+    router = mrise.router
+    assert isinstance(router, SimpleRouter)
+    assert len(router.senders) == 1
+    key = _Key(user='user', domain='example.com')
+    assert router.get_sender(key) is not None
 
 
 def test_fnmatch_config_keys() -> None:
     """Tests the config key parser with fnmatch pattern tokens."""
     # This defaults to "*@mailrise.xyz", which may not be obvious at first
     # glance.
     file = StringIO("""
         configs:
           "*":
             urls:
               - json://localhost
     """)
     mrise = load_config(_logger, file)
-    key = Key(user='user', domain='example.com')
-    assert mrise.get_sender(key) is None
-    key = Key(user='user', domain='mailrise.xyz')
-    assert mrise.get_sender(key) is not None
+    router = mrise.router
+    assert isinstance(router, SimpleRouter)
+    key = _Key(user='user', domain='example.com')
+    assert router.get_sender(key) is None
+    key = _Key(user='user', domain='mailrise.xyz')
+    assert router.get_sender(key) is not None
 
     file = StringIO("""
         configs:
           "*@*":
             urls:
               - json://localhost
     """)
     mrise = load_config(_logger, file)
-    key = Key(user='user', domain='example.com')
-    assert mrise.get_sender(key) is not None
+    router = mrise.router
+    assert isinstance(router, SimpleRouter)
+    key = _Key(user='user', domain='example.com')
+    assert router.get_sender(key) is not None
 
     file = StringIO("""
         configs:
           "the*@*":
             urls:
               - json://localhost
     """)
     mrise = load_config(_logger, file)
-    key = Key(user='user', domain='example.com')
-    assert mrise.get_sender(key) is None
-    key = Key(user='thequickbrownfox', domain='example.com')
-    assert mrise.get_sender(key) is not None
+    router = mrise.router
+    assert isinstance(router, SimpleRouter)
+    key = _Key(user='user', domain='example.com')
+    assert router.get_sender(key) is None
+    key = _Key(user='thequickbrownfox', domain='example.com')
+    assert router.get_sender(key) is not None
 
 
 def test_authenticator() -> None:
     """Tests a successful load with an authenticator."""
     file = StringIO("""
         configs:
           test:
@@ -218,27 +235,36 @@
                 test:
                   urls:
                     - !env_var fallback json://localhost
             """)
         ]
         for file in files:
             mrise = load_config(_logger, file)
-            assert len(mrise.senders) == 1
-            key = Key(user='test')
-            sender = mrise.get_sender(key)
+            router = mrise.router
+            assert isinstance(router, SimpleRouter)
+            assert len(router.senders) == 1
+            key = _Key(user='test')
+            sender = router.get_sender(key)
             assert sender is not None
+            notifier = _make_notifier(sender.config_yaml)
             # Missing type annotation for this property as of Dec 2022.
-            ap_servers = sender.notifier.servers  # type: ignore
+            ap_servers = notifier.servers  # type: ignore
             assert len(ap_servers) == 1
             config = ap_servers[0]
             servers = config.servers()
             assert len(servers) == 1
             assert servers[0].url().startswith('json://localhost')
 
-    with pytest.raises(ConfigFileError):
+    with pytest.raises(SystemExit):
         file = StringIO("""
           configs:
             test:
               urls:
                 - !env_var error
         """)
         load_config(_logger, file)
+
+
+def _make_notifier(config: str):
+    ap_config = AppriseConfig()
+    ap_config.add_config(config, format='yaml')
+    return Apprise(ap_config)
```

### Comparing `mailrise-1.3.0/tests/test_smtp.py` & `mailrise-1.4.0/tests/test_smtp.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,65 +2,34 @@
 Tests for the SMTP server functionality.
 """
 
 from email.message import EmailMessage
 from pathlib import Path
 
 import apprise
-import pytest
+from aiosmtpd.smtp import Envelope
 
-from mailrise.config import Key
-from mailrise.smtp import RecipientError, parsemessage, parsercpt
-
-
-def test_parsercpt() -> None:
-    """Tests for recipient parsing."""
-    rcpt = parsercpt('test@mailrise.xyz')
-    assert rcpt.key == Key(user='test')
-    assert rcpt.notify_type == apprise.NotifyType.INFO
-
-    rcpt = parsercpt('test.warning@mailrise.xyz')
-    assert rcpt.key == Key(user='test')
-    assert rcpt.notify_type == apprise.NotifyType.WARNING
-
-    rcpt = parsercpt('"with_quotes"@mailrise.xyz')
-    assert rcpt.key == Key(user='with_quotes')
-    assert rcpt.notify_type == apprise.NotifyType.INFO
-
-    rcpt = parsercpt('"with_quotes.success"@mailrise.xyz')
-    assert rcpt.key == Key('with_quotes')
-    assert rcpt.notify_type == apprise.NotifyType.SUCCESS
-
-    rcpt = parsercpt('"weird_quotes".success@mailrise.xyz')
-    assert rcpt.key == Key('"weird_quotes"')
-    assert rcpt.notify_type == apprise.NotifyType.SUCCESS
-
-    rcpt = parsercpt('John Doe <johndoe.warning@mailrise.xyz>')
-    assert rcpt.key == Key('johndoe')
-    assert rcpt.notify_type == apprise.NotifyType.WARNING
-
-    with pytest.raises(RecipientError):
-        parsercpt("Invalid Email <bad@>")
+from mailrise.smtp import _parsemessage
 
 
 def test_parsemessage() -> None:
     """Tests for email message parsing."""
     msg = EmailMessage()
     msg.set_content('Hello, World!')
     msg['From'] = ''
     msg['Subject'] = 'Test Message'
-    notification = parsemessage(msg)
+    notification = _parsemessage(msg, Envelope())
     assert notification.subject == 'Test Message'
     assert notification.body == 'Hello, World!'
     assert notification.body_format == apprise.NotifyFormat.TEXT
 
     msg = EmailMessage()
     msg.set_content('Hello, World!')
     msg.add_alternative('Hello, <strong>World!</strong>', subtype='html')
-    notification = parsemessage(msg)
+    notification = _parsemessage(msg, Envelope())
     assert notification.subject == '[no subject]'
     assert notification.from_ == '[no sender]'
     assert notification.body == 'Hello, <strong>World!</strong>'
     assert notification.body_format == apprise.NotifyFormat.HTML
 
 
 def test_multipart() -> None:
@@ -69,25 +38,25 @@
     with open(Path(__file__).parent/img_name, 'rb') as file:
         img_data = file.read()
     msg = EmailMessage()
     msg.add_related('Hello, World!')
     msg.add_related(img_data, maintype='image', subtype='jpeg')
     msg['From'] = ''
     msg['Subject'] = 'Test Message'
-    notification = parsemessage(msg)
+    notification = _parsemessage(msg, Envelope())
     assert notification.subject == 'Test Message'
     assert notification.body == 'Hello, World!'
     assert notification.body_format == apprise.NotifyFormat.TEXT
 
     msg = EmailMessage()
     msg.add_alternative('Hello, World!', subtype='plain')
     msg.add_alternative('<strong>Hello, World!</strong>', subtype='html')
     msg['From'] = ''
     msg['Subject'] = 'Test Message'
-    notification = parsemessage(msg)
+    notification = _parsemessage(msg, Envelope())
     assert notification.subject == 'Test Message'
     assert notification.body == '<strong>Hello, World!</strong>'
     assert notification.body_format == apprise.NotifyFormat.HTML
 
 
 def test_parseattachments() -> None:
     """Tests for email message parsing with attachments."""
@@ -101,15 +70,15 @@
     msg['Subject'] = 'Now With Images'
     msg.add_attachment(
         img_data,
         maintype='image',
         subtype='jpeg',
         filename=img_name
     )
-    notification = parsemessage(msg)
+    notification = _parsemessage(msg, Envelope())
     assert notification.subject == 'Now With Images'
     assert notification.from_ == 'sender@example.com'
     assert notification.body == 'Hello, World!'
     assert notification.body_format == apprise.NotifyFormat.TEXT
     assert len(notification.attachments) == 1
     assert notification.attachments[0].data == img_data
     assert notification.attachments[0].filename == img_name
@@ -126,15 +95,15 @@
     )
     msg.add_attachment(
         img_data,
         maintype='image',
         subtype='jpeg',
         filename=f'2_{img_name}'
     )
-    notification = parsemessage(msg)
+    notification = _parsemessage(msg, Envelope())
     assert notification.subject == 'Now With Images'
     assert notification.from_ == 'sender@example.com'
     assert notification.body == 'Hello, World!'
     assert notification.body_format == apprise.NotifyFormat.TEXT
     assert len(notification.attachments) == 2
     for attach in notification.attachments:
         assert attach.data == img_data
```

### Comparing `mailrise-1.3.0/tox.ini` & `mailrise-1.4.0/tox.ini`

 * *Files identical despite different names*

