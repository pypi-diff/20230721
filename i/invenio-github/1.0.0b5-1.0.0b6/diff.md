# Comparing `tmp/invenio-github-1.0.0b5.tar.gz` & `tmp/invenio-github-1.0.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-github-1.0.0b5.tar", last modified: Mon Jul 17 20:35:00 2023, max compression
+gzip compressed data, was "dist/invenio-github-1.0.0b6.tar", last modified: Fri Jul 21 16:11:38 2023, max compression
```

## Comparing `invenio-github-1.0.0b5.tar` & `invenio-github-1.0.0b6.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      973 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2509 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/.lgtm
--rw-r--r--   0 runner    (1001) docker     (122)     2747 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1382 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1549 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3464 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      105 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/MAINTAINERS
--rw-r--r--   0 runner    (1001) docker     (122)     1836 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     4857 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      762 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/RELEASE-NOTES.rst
--rw-r--r--   0 runner    (1001) docker     (122)      361 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/babel.ini
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/constraints-pypi.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/docs/
--rw-r--r--   0 runner    (1001) docker     (122)     7441 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)     1030 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10770 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     1013 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1571 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (122)      867 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6997 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1024 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github/
--rw-r--r--   0 runner    (1001) docker     (122)     1140 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github/alembic/
--rw-r--r--   0 runner    (1001) docker     (122)      552 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/alembic/5a5428312b2b_create_github_branch.py
--rw-r--r--   0 runner    (1001) docker     (122)     3766 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/alembic/b0eaee37b545_create_github_tables.py
--rw-r--r--   0 runner    (1001) docker     (122)    22856 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github/assets/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github/assets/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github/assets/semantic-ui/js/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github/assets/semantic-ui/js/invenio_github/
--rw-r--r--   0 runner    (1001) docker     (122)     3274 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/assets/semantic-ui/js/invenio_github/index.js
--rw-r--r--   0 runner    (1001) docker     (122)     2607 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     3876 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/errors.py
--rw-r--r--   0 runner    (1001) docker     (122)     2633 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/ext.py
--rw-r--r--   0 runner    (1001) docker     (122)     7738 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github/oauth/
--rw-r--r--   0 runner    (1001) docker     (122)     3167 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/oauth/handlers.py
--rw-r--r--   0 runner    (1001) docker     (122)      757 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/oauth/remote_app.py
--rw-r--r--   0 runner    (1001) docker     (122)     1155 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/proxies.py
--rw-r--r--   0 runner    (1001) docker     (122)     4091 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/receivers.py
--rw-r--r--   0 runner    (1001) docker     (122)     6382 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github/templates/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github/templates/semantic-ui/invenio_github/
--rw-r--r--   0 runner    (1001) docker     (122)      214 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/templates/semantic-ui/invenio_github/base.html
--rw-r--r--   0 runner    (1001) docker     (122)     1545 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/templates/semantic-ui/invenio_github/helpers.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github/templates/semantic-ui/invenio_github/settings/
--rw-r--r--   0 runner    (1001) docker     (122)      386 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/templates/semantic-ui/invenio_github/settings/base.html
--rw-r--r--   0 runner    (1001) docker     (122)     2656 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/templates/semantic-ui/invenio_github/settings/helpers.html
--rw-r--r--   0 runner    (1001) docker     (122)     6503 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/templates/semantic-ui/invenio_github/settings/index.html
--rw-r--r--   0 runner    (1001) docker     (122)      981 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/templates/semantic-ui/invenio_github/settings/index_item.html
--rw-r--r--   0 runner    (1001) docker     (122)    15043 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/templates/semantic-ui/invenio_github/settings/view.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github/translations/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github/translations/cs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github/translations/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1470 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github/translations/da/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github/translations/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1337 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/translations/da/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1337 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      475 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github/translations/en/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1776 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/translations/en/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github/translations/es/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github/translations/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1338 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1551 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/translations/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github/translations/it/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github/translations/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1556 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/translations/it/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)     1271 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/translations/messages.pot
--rw-r--r--   0 runner    (1001) docker     (122)     1698 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github/views/
--rw-r--r--   0 runner    (1001) docker     (122)      949 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2897 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/views/badge.py
--rw-r--r--   0 runner    (1001) docker     (122)     8193 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/views/github.py
--rw-r--r--   0 runner    (1001) docker     (122)      653 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/webpack.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4857 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2394 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      784 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      944 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      971 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (122)      347 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/run-i18n-tests.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)     1840 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (122)     3247 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1130 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      973 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2509 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/.lgtm
+-rw-r--r--   0 runner    (1001) docker     (122)     2747 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1382 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1610 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3464 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      105 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/MAINTAINERS
+-rw-r--r--   0 runner    (1001) docker     (122)     1836 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4950 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      762 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/RELEASE-NOTES.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      361 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/babel.ini
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/constraints-pypi.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     7441 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)     1030 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10770 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1013 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1571 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      867 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6997 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1024 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/invenio_github/
+-rw-r--r--   0 runner    (1001) docker     (122)     1140 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/invenio_github/alembic/
+-rw-r--r--   0 runner    (1001) docker     (122)      552 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/alembic/5a5428312b2b_create_github_branch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3766 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/alembic/b0eaee37b545_create_github_tables.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23408 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/invenio_github/assets/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/invenio_github/assets/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/invenio_github/assets/semantic-ui/js/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/invenio_github/assets/semantic-ui/js/invenio_github/
+-rw-r--r--   0 runner    (1001) docker     (122)     3388 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/assets/semantic-ui/js/invenio_github/index.js
+-rw-r--r--   0 runner    (1001) docker     (122)     2607 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3876 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2633 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/ext.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7738 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/invenio_github/oauth/
+-rw-r--r--   0 runner    (1001) docker     (122)     3167 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/oauth/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      757 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/oauth/remote_app.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1155 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4091 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/receivers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6382 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/invenio_github/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/invenio_github/templates/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/invenio_github/templates/semantic-ui/invenio_github/
+-rw-r--r--   0 runner    (1001) docker     (122)      214 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/templates/semantic-ui/invenio_github/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1330 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/templates/semantic-ui/invenio_github/helpers.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/invenio_github/templates/semantic-ui/invenio_github/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)      386 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/templates/semantic-ui/invenio_github/settings/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2656 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/templates/semantic-ui/invenio_github/settings/helpers.html
+-rw-r--r--   0 runner    (1001) docker     (122)     6538 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/templates/semantic-ui/invenio_github/settings/index.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1389 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/templates/semantic-ui/invenio_github/settings/index_item.html
+-rw-r--r--   0 runner    (1001) docker     (122)    15814 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/templates/semantic-ui/invenio_github/settings/view.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/invenio_github/translations/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/invenio_github/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/invenio_github/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1470 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/invenio_github/translations/da/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/invenio_github/translations/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1337 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/translations/da/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/invenio_github/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/invenio_github/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1337 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/invenio_github/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/invenio_github/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      475 2023-07-21 16:11:37.000000 invenio-github-1.0.0b6/invenio_github/translations/en/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1776 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/translations/en/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/invenio_github/translations/es/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/invenio_github/translations/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1338 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/invenio_github/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/invenio_github/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1551 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/invenio_github/translations/it/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/invenio_github/translations/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1556 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/translations/it/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)     1271 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/translations/messages.pot
+-rw-r--r--   0 runner    (1001) docker     (122)     1698 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/invenio_github/views/
+-rw-r--r--   0 runner    (1001) docker     (122)      949 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3596 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/views/badge.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8272 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/views/github.py
+-rw-r--r--   0 runner    (1001) docker     (122)      653 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/invenio_github/webpack.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/invenio_github.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4950 2023-07-21 16:11:37.000000 invenio-github-1.0.0b6/invenio_github.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2394 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/invenio_github.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-21 16:11:37.000000 invenio-github-1.0.0b6/invenio_github.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      784 2023-07-21 16:11:37.000000 invenio-github-1.0.0b6/invenio_github.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-21 16:11:37.000000 invenio-github-1.0.0b6/invenio_github.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      944 2023-07-21 16:11:37.000000 invenio-github-1.0.0b6/invenio_github.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-07-21 16:11:37.000000 invenio-github-1.0.0b6/invenio_github.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      971 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (122)      347 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/run-i18n-tests.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1840 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     3247 2023-07-21 16:11:38.000000 invenio-github-1.0.0b6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1130 2023-07-21 16:11:27.000000 invenio-github-1.0.0b6/setup.py
```

### Comparing `invenio-github-1.0.0b5/.github/workflows/pypi-publish.yml` & `invenio-github-1.0.0b6/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b5/.github/workflows/tests.yml` & `invenio-github-1.0.0b6/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b5/.travis.yml` & `invenio-github-1.0.0b6/.travis.yml`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b5/AUTHORS.rst` & `invenio-github-1.0.0b6/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b5/CHANGES.rst` & `invenio-github-1.0.0b6/CHANGES.rst`

 * *Files 8% similar despite different names*

```diff
@@ -21,14 +21,18 @@
     waive the privileges and immunities granted to it by virtue of its status
     as an Intergovernmental Organization or submit itself to any jurisdiction.
 
 
 Changes
 =======
 
+Version v1.0.0b6 (released 2023-07-21)
+
+- add github badges
+
 Version v1.0.0b5 (released 2023-07-17)
 
 - setup: enable tests
 - setup: update Manifest.in
 
 Version v1.0.0b4 (released 2023-07-17)
```

### Comparing `invenio-github-1.0.0b5/CONTRIBUTING.rst` & `invenio-github-1.0.0b6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b5/LICENSE` & `invenio-github-1.0.0b6/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b5/MANIFEST.in` & `invenio-github-1.0.0b6/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b5/PKG-INFO` & `invenio-github-1.0.0b6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-github
-Version: 1.0.0b5
+Version: 1.0.0b6
 Summary: "Invenio module that adds GitHub integration to the platform."
 Home-page: https://github.com/inveniosoftware/invenio-github
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -79,14 +79,18 @@
             waive the privileges and immunities granted to it by virtue of its status
             as an Intergovernmental Organization or submit itself to any jurisdiction.
         
         
         Changes
         =======
         
+        Version v1.0.0b6 (released 2023-07-21)
+        
+        - add github badges
+        
         Version v1.0.0b5 (released 2023-07-17)
         
         - setup: enable tests
         - setup: update Manifest.in
         
         Version v1.0.0b4 (released 2023-07-17)
```

### Comparing `invenio-github-1.0.0b5/README.rst` & `invenio-github-1.0.0b6/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b5/RELEASE-NOTES.rst` & `invenio-github-1.0.0b6/RELEASE-NOTES.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b5/docs/Makefile` & `invenio-github-1.0.0b6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b5/docs/api.rst` & `invenio-github-1.0.0b6/docs/api.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b5/docs/authors.rst` & `invenio-github-1.0.0b6/docs/authors.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b5/docs/changes.rst` & `invenio-github-1.0.0b6/docs/changes.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b5/docs/conf.py` & `invenio-github-1.0.0b6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b5/docs/contributing.rst` & `invenio-github-1.0.0b6/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b5/docs/index.rst` & `invenio-github-1.0.0b6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b5/docs/installation.rst` & `invenio-github-1.0.0b6/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b5/docs/license.rst` & `invenio-github-1.0.0b6/docs/license.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b5/docs/make.bat` & `invenio-github-1.0.0b6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b5/docs/usage.rst` & `invenio-github-1.0.0b6/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b5/invenio_github/__init__.py` & `invenio-github-1.0.0b6/invenio_github/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,10 +22,10 @@
 # waive the privileges and immunities granted to it by virtue of its status
 # as an Intergovernmental Organization or submit itself to any jurisdiction.
 
 """Invenio module that adds GitHub integration to the platform."""
 
 from .ext import InvenioGitHub
 
-__version__ = "1.0.0b5"
+__version__ = "1.0.0b6"
 
 __all__ = ("__version__", "InvenioGitHub")
```

### Comparing `invenio-github-1.0.0b5/invenio_github/alembic/5a5428312b2b_create_github_branch.py` & `invenio-github-1.0.0b6/invenio_github/alembic/5a5428312b2b_create_github_branch.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b5/invenio_github/alembic/b0eaee37b545_create_github_tables.py` & `invenio-github-1.0.0b6/invenio_github/alembic/b0eaee37b545_create_github_tables.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b5/invenio_github/api.py` & `invenio-github-1.0.0b6/invenio_github/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 # In applying this license, CERN does not
 # waive the privileges and immunities granted to it by virtue of its status
 # as an Intergovernmental Organization or submit itself to any jurisdiction.
 
 """Invenio module that adds GitHub integration to the platform."""
 
 import json
+from abc import abstractmethod
 from contextlib import contextmanager
 from copy import deepcopy
 
 import github3
 import humanize
 import requests
 from flask import current_app
@@ -52,18 +53,20 @@
     RemoteAccountDataNotSet,
     RemoteAccountNotFound,
     RepositoryAccessError,
     RepositoryNotFoundError,
 )
 
 
-def check_repo_access_permissions(repo, user_id, repo_id, repo_name):
+def check_repo_access_permissions(repo, user_id):
     """Checks permissions from user on repo."""
     if repo and repo.user_id and repo.user_id != int(user_id):
-        raise RepositoryAccessError(user=user_id, repo=repo_name, repo_id=repo_id)
+        raise RepositoryAccessError(
+            user=user_id, repo=repo.name, repo_id=repo.github_id
+        )
 
 
 class GitHubAPI(object):
     """Wrapper for GitHub API."""
 
     def __init__(self, user_id=None):
         """Create a GitHub API object."""
@@ -260,17 +263,15 @@
     def create_hook(self, repo_id, repo_name):
         """Create repository hook."""
         # Get or create the repo and check access permissions
         repo = Repository.get(github_id=repo_id, name=repo_name)
         if not repo:
             repo = Repository.create(self.user_id, repo_id, repo_name)
 
-        check_repo_access_permissions(
-            repo, self.user_id, repo_id=repo_id, repo_name=repo_name
-        )
+        check_repo_access_permissions(repo, self.user_id)
 
         # Create hook
         hook_config = dict(
             url=self.webhook_url,
             content_type="json",
             secret=current_app.config["GITHUB_SHARED_SECRET"],
             insecure_ssl="1" if current_app.config["GITHUB_INSECURE_SSL"] else "0",
@@ -303,49 +304,51 @@
     def remove_hook(self, repo_id, name):
         """Remove repository hook."""
         repo = Repository.get(github_id=repo_id, name=name)
 
         if not repo:
             raise RepositoryNotFoundError(repo_id)
 
-        check_repo_access_permissions(
-            repo, self.user_id, repo_id=repo_id, repo_name=name
-        )
+        check_repo_access_permissions(repo, self.user_id)
 
         ghrepo = self.api.repository_with_id(repo_id)
         if ghrepo:
             hooks = (
                 h for h in ghrepo.hooks() if h.config.get("url", "") == self.webhook_url
             )
             hook = next(hooks, None)
             if not hook or hook.delete():
                 self.disable_repo(repo)
                 return True
         return False
 
+    def repo_last_published_release(self, repo):
+        """Retrieves the repository last release."""
+        release_object = repo.latest_release(ReleaseStatus.PUBLISHED)
+        release_instance = current_github.release_api_class(release_object)
+        return release_instance
+
     def get_repository_releases(self, repo):
         """Retrieve repository releases. Returns API release objects."""
-        check_repo_access_permissions(repo, self.user_id, repo.github_id, repo.name)
+        check_repo_access_permissions(repo, self.user_id)
 
         # Retrieve releases and sort them by creation date
         release_instances = []
         for release_object in repo.releases.order_by(Release.created):
             release_instance = current_github.release_api_class(release_object)
             release_instances.append(release_instance)
 
         return release_instances
 
     def get_user_repositories(self):
         """Retrieves user repositories, containing db repositories plus remote repositories."""
         repos = deepcopy(self.user_available_repositories)
         if repos:
             # 'Enhance' our repos dict, from our database model
-            db_repos = self.user_enabled_repositories
-            for repo in db_repos:
-                # TODO here
+            for repo in self.user_enabled_repositories:
                 if str(repo.github_id) in repos:
                     release_instance = current_github.release_api_class(
                         repo.latest_release()
                     )
                     repos[str(repo.github_id)]["instance"] = repo
                     repos[str(repo.github_id)]["latest"] = release_instance
         return repos
@@ -358,22 +361,22 @@
     @property
     def user_available_repositories(self):
         """Retrieve user repositories from user's remote data."""
         return self.account.extra_data.get("repos", [])
 
     def disable_repo(self, repo):
         """Disables an user repository if the user has permission to do so."""
-        check_repo_access_permissions(repo, self.user_id, repo.github_id, repo.name)
+        check_repo_access_permissions(repo, self.user_id)
 
         repo.hook = None
         repo.user_id = None
 
     def enable_repo(self, repo, hook):
         """Enables an user repository if the user has permission to do so."""
-        check_repo_access_permissions(repo, self.user_id, repo.github_id, repo.name)
+        check_repo_access_permissions(repo, self.user_id)
 
         repo.hook = hook
         repo.user_id = self.user_id
 
     def get_last_sync_time(self):
         """Retrieves the last sync delta time from github's client extra data.
 
@@ -383,25 +386,25 @@
             raise RemoteAccountDataNotSet(
                 self.user_id, "Last sync data is not set for user (remote data)."
             )
 
         extra_data = self.account.extra_data
         return extra_data["last_sync"]
 
-    def get_repository(self, repo_name):
+    def get_repository(self, repo_name=None, repo_github_id=None):
         """Retrieves one repository.
 
         Checks for access permission.
         """
-        repo = Repository.get(name=repo_name)
+        repo = Repository.get(name=repo_name, github_id=repo_github_id)
         if not repo:
             raise RepositoryNotFoundError(repo_name)
 
         # Might raise a RepositoryAccessError
-        check_repo_access_permissions(repo, self.user_id, repo.github_id, repo_name)
+        check_repo_access_permissions(repo, self.user_id)
 
         return repo
 
     @classmethod
     def _dev_api(cls):
         """Get a developer instance for GitHub API access."""
         gh = github3.GitHub()
@@ -566,15 +569,14 @@
 
         assert (
             response.status_code == 200
         ), f"Could not retrieve archive from GitHub: {zipball_url}"
 
     # High level API
 
-    # TODO split maybe
     def release_failed(self):
         """Set release status to FAILED."""
         self.release_object.status = ReleaseStatus.FAILED
 
     def release_processing(self):
         """Set release status to PROCESSING."""
         self.release_object.status = ReleaseStatus.PROCESSING
@@ -619,7 +621,24 @@
     def resolve_record(self):
         """Resolves a record from the release. To be implemented by the API class implementation."""
         raise NotImplementedError
 
     def serialize_record(self):
         """Serializes the release record."""
         raise NotImplementedError
+
+    @property
+    @abstractmethod
+    def badge_title(self):
+        """Stores a string to render in the record badge title (e.g. 'DOI')."""
+        return None
+
+    @property
+    @abstractmethod
+    def badge_value(self):
+        """Stores a string to render in the record badge value (e.g. '10.1234/invenio.1234')."""
+        raise NotImplementedError
+
+    @property
+    def record_url(self):
+        """Release self url (e.g. github HTML url)."""
+        raise NotImplementedError
```

### Comparing `invenio-github-1.0.0b5/invenio_github/assets/semantic-ui/js/invenio_github/index.js` & `invenio-github-1.0.0b6/invenio_github/assets/semantic-ui/js/invenio_github/index.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,13 @@
 // This file is part of InvenioGithub
 // Copyright (C) 2023 CERN.
 //
 // Invenio Github is free software; you can redistribute it and/or modify it
 // under the terms of the MIT License; see LICENSE file for more details.
+import $ from "jquery";
 
 function addResultMessage(element, color, message) {
     element.classList.remove("hidden");
     element.classList.add("basic");
     element.classList.add(color);
     element.textContent = message;
 }
@@ -96,8 +97,12 @@
         } catch (error) {
             addResultMessage(switchMessage, "red", `There has been a problem: ${error}`);
             setTimeout(function() {
                 switchMessage.classList.add("hidden");
             }, 7000);
         }
     }
-}
+}
+
+$(".doi-badge-img").on("click", function() {
+    $(".doi-badge-modal").modal("show");
+});
```

### Comparing `invenio-github-1.0.0b5/invenio_github/config.py` & `invenio-github-1.0.0b6/invenio_github/config.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b5/invenio_github/errors.py` & `invenio-github-1.0.0b6/invenio_github/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b5/invenio_github/ext.py` & `invenio-github-1.0.0b6/invenio_github/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b5/invenio_github/models.py` & `invenio-github-1.0.0b6/invenio_github/models.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b5/invenio_github/oauth/handlers.py` & `invenio-github-1.0.0b6/invenio_github/oauth/handlers.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b5/invenio_github/oauth/remote_app.py` & `invenio-github-1.0.0b6/invenio_github/oauth/remote_app.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b5/invenio_github/proxies.py` & `invenio-github-1.0.0b6/invenio_github/proxies.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b5/invenio_github/receivers.py` & `invenio-github-1.0.0b6/invenio_github/receivers.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b5/invenio_github/tasks.py` & `invenio-github-1.0.0b6/invenio_github/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b5/invenio_github/templates/semantic-ui/invenio_github/settings/helpers.html` & `invenio-github-1.0.0b6/invenio_github/templates/semantic-ui/invenio_github/settings/helpers.html`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b5/invenio_github/templates/semantic-ui/invenio_github/settings/index.html` & `invenio-github-1.0.0b6/invenio_github/templates/semantic-ui/invenio_github/settings/index.html`

 * *Files 5% similar despite different names*

```diff
@@ -65,15 +65,16 @@
                 <input type="checkbox" checked>
                 <label></label>
               </div>
             </div>
             <div class="column"></div>
             <div class="column centered">
               <br>
-              <a class="ui label blue" href="https://doi.org/10.5281/zenodo.8475">
+              {#- TODO remove hardcoding Zenodo stuff #}
+              <a href="https://doi.org/10.5281/zenodo.8475">
                 <img src="{{ url_for('invenio_formatter_badges.badge', title='doi', value='10.5281/zenodo.8475', ext='svg') }}" alt="10.5281/zenodo.8475">
               </a>
               <br>
               <small>{{ _("(example)") }}</small>
             </div>
           </div>
         </div>
```

#### html2text {}

```diff
@@ -18,15 +18,15 @@
 default('System')) }}
 ***** 3 {{ _("Get the badge") }} *****
 {{ _('After your first release, a DOI badge that you can include in GitHub
 README will appear next to your repository below.') }}
 
 *
 
-[10.5281/zenodo.8475]
+{#- TODO remove hardcoding Zenodo stuff #} [10.5281/zenodo.8475]
 {{ _("(example)") }}
 {{ helpers.panel_end(with_body=False) }} {%- endblock %} {%- if repos %} {%-
 block enabled_repositories %} {%- for repo_id, repo in repos if repo.instance
 and repo.instance.hook %} {%- if loop.first %} {{ helpers.panel_start(_
 ('Enabled Repositories') , with_body=False) }}
 {%- endif %}
 {% include "invenio_github/settings/index_item.html" with context %}
```

### Comparing `invenio-github-1.0.0b5/invenio_github/templates/semantic-ui/invenio_github/settings/index_item.html` & `invenio-github-1.0.0b6/invenio_github/templates/semantic-ui/invenio_github/settings/index_item.html`

 * *Files 12% similar despite different names*

```diff
@@ -2,24 +2,34 @@
 
   This file is part of Invenio.
   Copyright (C) 2023 CERN.
 
   Invenio is free software; you can redistribute it and/or modify it
   under the terms of the MIT License; see LICENSE file for more details.
 #}
+{%- from "invenio_github/helpers.html" import doi_badge with context -%}
+{%- set release = repo.get('latest') %}
 {%- block repository_item %}
   <div class="ui grid">
     <div class="ten wide column">
       <div class="ui basic segment">
         <h4>
           <a href="https://github.com/{{ repo.full_name }}" data-tooltip="{{ _('Go to GitHub.') }}">
             <i class="github icon"></i>
           </a>
           <a href="{{ url_for('.get_repository', repo_name=repo.full_name) }}">{{ repo.full_name }}</a>
         </h4>
+        {%- if release.record %}
+          {%- set id_doi = release.record.pids.get('doi', {}).get('identifier') %}
+        {%- endif %}
+        {%- if id_doi %}
+          <p>
+            {{ doi_badge(id_doi, doi_url=release.record_url, github_id=repo_id) }}
+          </p>
+        {%- endif %}
       </div>
     </div>
     <div class="four wide column">
       <div id="repo-switch-message" class="ui label hidden"></div>
     </div>
     <div class="two wide column">
       {{ helpers.repo_switch(repo.instance, repo_id) }}
```

#### html2text {}

```diff
@@ -1,8 +1,13 @@
 {# -*- coding: utf-8 -*- This file is part of Invenio. Copyright (C) 2023 CERN.
 Invenio is free software; you can redistribute it and/or modify it under the
-terms of the MIT License; see LICENSE file for more details. #} {%- block
-repository_item %}
+terms of the MIT License; see LICENSE file for more details. #} {%- from
+"invenio_github/helpers.html" import doi_badge with context -%} {%- set release
+= repo.get('latest') %} {%- block repository_item %}
  {{_repo.full_name_}}
+{%- if release.record %} {%- set id_doi = release.record.pids.get('doi',
+{}).get('identifier') %} {%- endif %} {%- if id_doi %}
+{{ doi_badge(id_doi, doi_url=release.record_url, github_id=repo_id) }}
+{%- endif %}
 {{ helpers.repo_switch(repo.instance, repo_id) }}
 {%- if not loop.last %}
 {%- endif %} {%- endblock %}
```

### Comparing `invenio-github-1.0.0b5/invenio_github/templates/semantic-ui/invenio_github/settings/view.html` & `invenio-github-1.0.0b6/invenio_github/templates/semantic-ui/invenio_github/settings/view.html`

 * *Files 8% similar despite different names*

```diff
@@ -4,32 +4,35 @@
   Copyright (C) 2023 CERN.
 
   Invenio is free software; you can redistribute it and/or modify it
   under the terms of the MIT License; see LICENSE file for more details.
 #}
 
 {%- import "invenio_github/settings/helpers.html" as helpers with context %}
+{%- from "invenio_github/helpers.html" import doi_badge with context -%}
+
 {%- extends config.GITHUB_SETTINGS_TEMPLATE %}
 
 {%- block settings_content %}
   {%- set github_rel_url = 'https://github.com/{0}/releases/new'.format(repo.name) %}
-  {%- set latest_success_pid = None %}
-  {%- set latest_published = repo.latest_release(status='D') %}
   {% set active = true %}
-  {%- if latest_published %}
-    {%- set latest_success_pid = latest_published.release_id %}
-  {%- endif %}
-  {%- block repo_details_header %}
+  {%- block repo_details_header scoped %}
   <div class="repositories-list">
     <div class="ui grid">
       <div class="eleven wide column">
         <h1>
           <i class="github icon"></i>
           {{ repo.name }}
         </h1>
+          {%- if latest_release.record %}
+            {%- set id_doi = latest_release.record.pids.get('doi', {}).get('identifier') %}
+          {%- endif %}
+          {%- if id_doi %}
+            <p>{{ doi_badge(id_doi, doi_url=latest_release.record_url, github_id=repo.github_id) }}</p>
+          {%- endif %}
       </div>
       <div class="four wide right aligned column">
         <div id="repo-switch-message" class="ui label hidden"></div>
       </div>
       <div class="one wide column">
         {{ helpers.repo_switch(repo, repo.github_id) }}
       </div>
@@ -131,14 +134,26 @@
                              aria-expanded="false">
                             <h5>
                               <i class="tag icon tab-menu-accordion"></i>
                               {{ release.release_object.tag }} &nbsp; {%- if release.record %}{{ release.record.data["metadata"]["title"] }}{%- endif %}
                             </h5>
                           </a>
                           <br>
+                          {%- if release.record %}
+                            {%- set release_doi = release.record.pids.get('doi', {}).get('identifier') %}
+                          {%- endif %}
+                          {%- if release_doi %}
+                            <p>
+                              <a href={{release.record_url}}>
+                                <i class="barcode icon"></i>
+                                DOI: {{release_doi}}
+                              </a>
+                            </p>
+                          {%- endif %}
+                          <br>
                           <p>
                             <a href="{{ release.event.payload.release.html_url if release.event else 'https://github.com/{0}/releases/tag/{1}'.format(repo.name, release.model.tag) }}">
                               <i class="github icon tab-menu-accordion"></i>
                               {{ release.event.payload.release.name if release.event and release.event.payload.release.name else release.model.tag }}
                             </a>
                           </p>
                         </div>
```

### Comparing `invenio-github-1.0.0b5/invenio_github/translations/cs/LC_MESSAGES/messages.po` & `invenio-github-1.0.0b6/invenio_github/translations/cs/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b5/invenio_github/translations/da/LC_MESSAGES/messages.po` & `invenio-github-1.0.0b6/invenio_github/translations/da/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b5/invenio_github/translations/de/LC_MESSAGES/messages.po` & `invenio-github-1.0.0b6/invenio_github/translations/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b5/invenio_github/translations/en/LC_MESSAGES/messages.po` & `invenio-github-1.0.0b6/invenio_github/translations/en/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b5/invenio_github/translations/es/LC_MESSAGES/messages.po` & `invenio-github-1.0.0b6/invenio_github/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b5/invenio_github/translations/fr/LC_MESSAGES/messages.po` & `invenio-github-1.0.0b6/invenio_github/translations/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b5/invenio_github/translations/it/LC_MESSAGES/messages.po` & `invenio-github-1.0.0b6/invenio_github/translations/it/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b5/invenio_github/translations/messages.pot` & `invenio-github-1.0.0b6/invenio_github/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b5/invenio_github/utils.py` & `invenio-github-1.0.0b6/invenio_github/utils.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b5/invenio_github/views/__init__.py` & `invenio-github-1.0.0b6/invenio_github/views/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b5/invenio_github/views/badge.py` & `invenio-github-1.0.0b6/invenio_github/views/badge.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
-# Copyright (C) 2014, 2015, 2016 CERN.
+# Copyright (C) 2014-2023 CERN.
 #
 # Invenio is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # Invenio is distributed in the hope that it will be useful,
@@ -21,74 +21,93 @@
 # or submit itself to any jurisdiction.
 
 
 """DOI Badge Blueprint."""
 
 from __future__ import absolute_import
 
-from flask import Blueprint, abort, redirect, url_for
+from flask import Blueprint, abort, current_app, redirect, url_for
+from flask_login import current_user
 
-from ..api import GitHubRelease
-from ..models import ReleaseStatus, Repository
+from invenio_github.api import GitHubAPI, GitHubRelease
+from invenio_github.models import ReleaseStatus, Repository
 
 blueprint = Blueprint(
     "invenio_github_badge",
     __name__,
     url_prefix="/badge",
     static_folder="../static",
     template_folder="../templates",
 )
 
 
+# Kept for backward compatibility
 def get_pid_of_latest_release_or_404(**kwargs):
     """Return PID of the latest release."""
     repo = Repository.query.filter_by(**kwargs).first_or_404()
     release = repo.latest_release(ReleaseStatus.PUBLISHED)
     if release:
         return GitHubRelease(release).pid
     abort(404)
 
 
+# Kept for backward compatibility
 def get_badge_image_url(pid, ext="svg"):
     """Return the badge for a DOI."""
     return url_for(
         "invenio_formatter_badges.badge",
         title=pid.pid_type,
         value=pid.pid_value,
         ext=ext,
     )
 
 
+# Kept for backward compatibility
 def get_doi_url(pid):
     """Return the badge for a DOI."""
     return "https://doi.org/{pid.pid_value}".format(pid=pid)
 
 
 #
 # Views
 #
-@blueprint.route("/<int:github_id>.svg")
-def index(github_id):
+@blueprint.route("/<int:repo_github_id>.svg")
+def index(repo_github_id):
     """Generate a badge for a specific GitHub repository."""
-    pid = get_pid_of_latest_release_or_404(github_id=github_id)
-    return redirect(get_badge_image_url(pid))
+    try:
+        github_api = GitHubAPI(current_user.id)
+        repo = github_api.get_repository(repo_github_id=repo_github_id)
+        release = github_api.repo_last_published_release(repo)
+        badge_url = url_for(
+            "invenio_formatter_badges.badge",
+            title=release.badge_title,
+            value=release.badge_value,
+            ext="svg",
+        )
+        return redirect(badge_url)
+    except Exception as e:
+        current_app.logger.error(str(e), exc_info=True)
+        abort(404)
 
 
+# Kept for backward compatibility
 @blueprint.route("/<int:user_id>/<path:repo_name>.svg")
 def index_old(user_id, repo_name):
     """Generate a badge for a specific GitHub repository."""
     pid = get_pid_of_latest_release_or_404(name=repo_name)
     return redirect(get_badge_image_url(pid))
 
 
+# Kept for backward compatibility
 @blueprint.route("/latestdoi/<int:github_id>")
 def latest_doi(github_id):
     """Redirect to the newest record version."""
     pid = get_pid_of_latest_release_or_404(github_id=github_id)
     return redirect(get_doi_url(pid))
 
 
+# Kept for backward compatibility
 @blueprint.route("/latestdoi/<int:user_id>/<path:repo_name>")
 def latest_doi_old(user_id, repo_name):
     """Redirect to the newest record version."""
     pid = get_pid_of_latest_release_or_404(name=repo_name)
     return redirect(get_doi_url(pid))
```

### Comparing `invenio-github-1.0.0b5/invenio_github/views/github.py` & `invenio-github-1.0.0b6/invenio_github/views/github.py`

 * *Files 6% similar despite different names*

```diff
@@ -80,15 +80,14 @@
 
 
 def register_ui_routes(blueprint):
     """Register ui routes."""
 
     @blueprint.route("/")
     @login_required
-    @request_session_token()
     @register_menu(  # TODO modify?
         blueprint,
         "settings.github",
         # TODO substitute github for icon + 'Github'
         _("Github"),
         # _(
         #     "%(icon)s GitHub",
@@ -102,27 +101,26 @@
         # active_when=lambda: request.endpoint.startswith("invenio_github."),
     )
     @register_breadcrumb(blueprint, "breadcrumbs.settings.github", _("GitHub"))
     def get_repositories():
         """Display list of the user's repositories."""
         github = GitHubAPI(user_id=current_user.id)
         ctx = dict(connected=False)
-
-        # Generate the repositories view object
-        repos = github.get_user_repositories()
-        last_sync = github.get_last_sync_time()
-
-        ctx.update(
-            {
-                # TODO maybe can be refactored. e.g. have two templates and render the correct one.
-                "connected": True,
-                "repos": sorted(repos.items(), key=lambda x: x[1]["full_name"]),
-                "last_sync": last_sync,
-            }
-        )
+        if github.session_token:
+            # Generate the repositories view object
+            repos = github.get_user_repositories()
+            last_sync = github.get_last_sync_time()
+
+            ctx.update(
+                {
+                    "connected": True,
+                    "repos": sorted(repos.items(), key=lambda x: x[1]["full_name"]),
+                    "last_sync": last_sync,
+                }
+            )
 
         return render_template(current_app.config["GITHUB_TEMPLATE_INDEX"], **ctx)
 
     @blueprint.route("/repository/<path:repo_name>")
     @login_required
     @request_session_token()
     @register_breadcrumb(blueprint, "breadcrumbs.settings.github.repo", _("Repository"))
@@ -132,36 +130,39 @@
         Retrieves and builds context to display all repository releases, if any.
         """
         user_id = current_user.id
         github = GitHubAPI(user_id=user_id)
 
         try:
             repo = github.get_repository(repo_name)
+            latest_release = github.repo_last_published_release(repo)
             default_branch = (
                 github.account.extra_data.get("repos", [])
                 .get(str(repo.github_id), None)
                 .get("default_branch", None)
             )
             releases = github.get_repository_releases(repo=repo)
             return render_template(
                 current_app.config["GITHUB_TEMPLATE_VIEW"],
+                latest_release=latest_release,
                 repo=repo,
                 releases=releases,
                 default_branch=default_branch,
             )
-        except RepositoryAccessError as e:
+        except RepositoryAccessError:
             abort(403)
-        except NoResultFound as e:
+        except NoResultFound:
             abort(404)
 
 
 def register_api_routes(blueprint):
     """Register API routes."""
 
     @login_required
+    @request_session_token()
     @blueprint.route("/user/github/repositories/sync", methods=["POST"])
     def sync_user_repositories():
         """Synchronizes user repos.
 
         Currently:
             POST /api/user/github/repositories/sync
         Previously:
```

### Comparing `invenio-github-1.0.0b5/invenio_github/webpack.py` & `invenio-github-1.0.0b6/invenio_github/webpack.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b5/invenio_github.egg-info/PKG-INFO` & `invenio-github-1.0.0b6/invenio_github.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-github
-Version: 1.0.0b5
+Version: 1.0.0b6
 Summary: "Invenio module that adds GitHub integration to the platform."
 Home-page: https://github.com/inveniosoftware/invenio-github
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -79,14 +79,18 @@
             waive the privileges and immunities granted to it by virtue of its status
             as an Intergovernmental Organization or submit itself to any jurisdiction.
         
         
         Changes
         =======
         
+        Version v1.0.0b6 (released 2023-07-21)
+        
+        - add github badges
+        
         Version v1.0.0b5 (released 2023-07-17)
         
         - setup: enable tests
         - setup: update Manifest.in
         
         Version v1.0.0b4 (released 2023-07-17)
```

### Comparing `invenio-github-1.0.0b5/invenio_github.egg-info/SOURCES.txt` & `invenio-github-1.0.0b6/invenio_github.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b5/invenio_github.egg-info/entry_points.txt` & `invenio-github-1.0.0b6/invenio_github.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b5/invenio_github.egg-info/requires.txt` & `invenio-github-1.0.0b6/invenio_github.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b5/requirements-devel.txt` & `invenio-github-1.0.0b6/requirements-devel.txt`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b5/run-tests.sh` & `invenio-github-1.0.0b6/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b5/setup.cfg` & `invenio-github-1.0.0b6/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b5/setup.py` & `invenio-github-1.0.0b6/setup.py`

 * *Files identical despite different names*

