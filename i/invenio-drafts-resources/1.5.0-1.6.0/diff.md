# Comparing `tmp/invenio-drafts-resources-1.5.0.tar.gz` & `tmp/invenio-drafts-resources-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-drafts-resources-1.5.0.tar", last modified: Tue Jul 11 15:40:26 2023, max compression
+gzip compressed data, was "dist/invenio-drafts-resources-1.6.0.tar", last modified: Fri Jul 21 13:19:39 2023, max compression
```

## Comparing `invenio-drafts-resources-1.5.0.tar` & `invenio-drafts-resources-1.6.0.tar`

### file list

```diff
@@ -1,327 +1,327 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/.github/workflows/i18n-pull.yml
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/.github/workflows/i18n-push.yml
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/.github/workflows/tests.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/.tx/
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/.tx/config
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/babel.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10309 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7017 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/records/
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/records/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/records/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/records/systemfields/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/records/systemfields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/records/systemfields/parent.py
--rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/records/systemfields/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/resources/records/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/resources/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/resources/records/args.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/resources/records/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/resources/records/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7603 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/resources/records/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/services/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/services/records/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/services/records/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/services/records/components/
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/services/records/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10339 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/services/records/components/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/services/records/components/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/services/records/components/media_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/services/records/components/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/services/records/components/pid.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/services/records/components/relations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/services/records/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/services/records/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/services/records/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/services/records/search_params.py
--rw-r--r--   0 runner    (1001) docker     (123)    22122 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/services/records/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/services/records/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/af/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/af/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-11 15:40:25.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/af/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/af/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ar/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-11 15:40:25.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ar/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ar/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/bg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/bg/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/bg/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ca/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-11 15:40:25.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ca/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ca/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/cs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-11 15:40:25.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/cs/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/da/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-11 15:40:25.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/da/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/da/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-11 15:40:25.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/de_AT/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/de_AT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/de_AT/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/de_AT/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/de_DE/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/de_DE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-11 15:40:25.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/de_DE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/de_DE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/el/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-11 15:40:25.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/el/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/el/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/en_AT/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/en_AT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-11 15:40:25.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/en_AT/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/en_AT/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/en_HU/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/en_HU/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-11 15:40:25.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/en_HU/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/en_HU/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-11 15:40:25.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/es_CU/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/es_CU/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/es_CU/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/es_CU/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/es_MX/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/es_MX/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/es_MX/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/es_MX/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/et/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-11 15:40:25.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/et/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/et/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/et_EE/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/et_EE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/et_EE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/et_EE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/fa/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-11 15:40:25.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/fa/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/fa/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/fa_IR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/fa_IR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/fa_IR/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/fa_IR/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-11 15:40:25.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/fr_CI/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/fr_CI/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-11 15:40:25.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/fr_CI/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/fr_CI/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/fr_FR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/fr_FR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-11 15:40:25.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/fr_FR/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/fr_FR/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/gl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/gl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/gl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/gl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/hi_IN/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/hi_IN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/hi_IN/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/hi_IN/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/hr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/hr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/hr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/hu/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/hu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-11 15:40:25.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/hu/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/hu/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/hu_HU/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/hu_HU/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/hu_HU/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/hu_HU/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/it/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/it/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/it/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ja/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-11 15:40:25.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ja/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ja/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ka/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ka/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ka/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ka/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/lt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-11 15:40:25.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/lt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/lt/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/messages.pot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ne/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ne/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ne/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ne/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/no/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/no/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-11 15:40:25.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/no/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/no/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/pl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/pl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/pl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/pt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/pt/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ro/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ro/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ro/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-11 15:40:25.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ru/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ru/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/rw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/rw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-11 15:40:25.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/rw/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/rw/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/sk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-11 15:40:25.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/sk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/sk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/sv/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-11 15:40:25.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/sv/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/sv/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/sv_SE/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/sv_SE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-11 15:40:25.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/sv_SE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/sv_SE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/tr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/tr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/tr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/uk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/uk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/uk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/uk_UA/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/uk_UA/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-11 15:40:25.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/uk_UA/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/uk_UA/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/zh_CN/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/zh_CN/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-11 15:40:25.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/zh_TW/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/zh_TW/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10200 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1905 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/tests/mock_module/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/mock_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/mock_module/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/tests/mock_module/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/mock_module/jsonschemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/tests/mock_module/jsonschemas/records/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/mock_module/jsonschemas/records/parent-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/mock_module/jsonschemas/records/record-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/tests/mock_module/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/mock_module/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/tests/mock_module/mappings/os-v1/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/mock_module/mappings/os-v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/tests/mock_module/mappings/os-v1/draftsresources/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/mock_module/mappings/os-v1/draftsresources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/tests/mock_module/mappings/os-v1/draftsresources/drafts/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/mock_module/mappings/os-v1/draftsresources/drafts/draft-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/tests/mock_module/mappings/os-v1/draftsresources/records/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/mock_module/mappings/os-v1/draftsresources/records/record-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/tests/mock_module/mappings/os-v2/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/mock_module/mappings/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/tests/mock_module/mappings/os-v2/draftsresources/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/mock_module/mappings/os-v2/draftsresources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/tests/mock_module/mappings/os-v2/draftsresources/drafts/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/mock_module/mappings/os-v2/draftsresources/drafts/draft-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/tests/mock_module/mappings/os-v2/draftsresources/records/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/mock_module/mappings/os-v2/draftsresources/records/record-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/tests/mock_module/mappings/v7/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/mock_module/mappings/v7/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/tests/mock_module/mappings/v7/draftsresources/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/mock_module/mappings/v7/draftsresources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/tests/mock_module/mappings/v7/draftsresources/drafts/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/mock_module/mappings/v7/draftsresources/drafts/draft-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/tests/mock_module/mappings/v7/draftsresources/records/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/mock_module/mappings/v7/draftsresources/records/record-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/mock_module/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/mock_module/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/mock_module/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/mock_module/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/mock_module/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/tests/records/
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/records/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11614 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/records/test_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/resources/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6782 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/resources/test_files_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/resources/test_record_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/resources/test_resource_links.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/tests/services/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/services/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13306 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/services/test_record_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    21966 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/services/test_record_service_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/services/test_record_service_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/services/test_record_service_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/services/test_services.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/services/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/.github/workflows/i18n-pull.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/.github/workflows/i18n-push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/.github/workflows/tests.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/.tx/
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/.tx/config
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/babel.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10309 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7017 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/records/
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/records/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/records/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/records/systemfields/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/records/systemfields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/records/systemfields/parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7935 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/records/systemfields/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/resources/records/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/resources/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/resources/records/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/resources/records/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/resources/records/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7603 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/resources/records/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/services/records/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/services/records/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/services/records/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/services/records/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10339 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/services/records/components/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/services/records/components/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/services/records/components/media_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/services/records/components/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/services/records/components/pid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/services/records/components/relations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/services/records/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/services/records/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/services/records/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/services/records/search_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22161 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/services/records/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/services/records/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/af/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/af/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/af/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/af/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/ar/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/ar/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/bg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/bg/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/bg/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/ca/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/ca/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/ca/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/cs/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/da/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/da/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/da/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/de_AT/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/de_AT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/de_AT/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/de_AT/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/de_DE/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/de_DE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/de_DE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/de_DE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/el/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/el/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/el/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/en_AT/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/en_AT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/en_AT/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/en_AT/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/en_HU/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/en_HU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/en_HU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/en_HU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/es_CU/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/es_CU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/es_CU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/es_CU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/es_MX/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/es_MX/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/es_MX/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/es_MX/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/et/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/et/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/et/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/et_EE/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/et_EE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/et_EE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/et_EE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/fa/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/fa/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/fa/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/fa_IR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/fa_IR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/fa_IR/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/fa_IR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/fr_CI/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/fr_CI/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/fr_CI/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/fr_CI/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/fr_FR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/fr_FR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/fr_FR/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/fr_FR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/gl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/gl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/gl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/gl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/hi_IN/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/hi_IN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/hi_IN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/hi_IN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/hr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/hr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/hr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/hu/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/hu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/hu/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/hu/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/hu_HU/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/hu_HU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/hu_HU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/hu_HU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/it/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/it/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/ja/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/ja/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/ja/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/ka/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/ka/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/ka/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/ka/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/lt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/lt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/lt/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/messages.pot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/ne/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/ne/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/ne/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/ne/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/no/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/no/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/no/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/no/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/pl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/pl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/pl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/pt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/pt/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/ro/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/ro/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/ro/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/ru/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/ru/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/rw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/rw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/rw/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/rw/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/sk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/sk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/sk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/sv/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/sv/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/sv/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/sv_SE/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/sv_SE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/sv_SE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/sv_SE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/tr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/tr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/tr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/uk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/uk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/uk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/uk_UA/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/uk_UA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/uk_UA/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/uk_UA/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/zh_CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/zh_CN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/zh_TW/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/zh_TW/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10200 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/invenio_drafts_resources.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1905 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/tests/mock_module/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/tests/mock_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/tests/mock_module/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/tests/mock_module/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/tests/mock_module/jsonschemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/tests/mock_module/jsonschemas/records/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/tests/mock_module/jsonschemas/records/parent-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/tests/mock_module/jsonschemas/records/record-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/tests/mock_module/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/tests/mock_module/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/tests/mock_module/mappings/os-v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/tests/mock_module/mappings/os-v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/tests/mock_module/mappings/os-v1/draftsresources/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/tests/mock_module/mappings/os-v1/draftsresources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/tests/mock_module/mappings/os-v1/draftsresources/drafts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/tests/mock_module/mappings/os-v1/draftsresources/drafts/draft-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/tests/mock_module/mappings/os-v1/draftsresources/records/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/tests/mock_module/mappings/os-v1/draftsresources/records/record-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/tests/mock_module/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/tests/mock_module/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/tests/mock_module/mappings/os-v2/draftsresources/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/tests/mock_module/mappings/os-v2/draftsresources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/tests/mock_module/mappings/os-v2/draftsresources/drafts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/tests/mock_module/mappings/os-v2/draftsresources/drafts/draft-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/tests/mock_module/mappings/os-v2/draftsresources/records/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/tests/mock_module/mappings/os-v2/draftsresources/records/record-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/tests/mock_module/mappings/v7/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/tests/mock_module/mappings/v7/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/tests/mock_module/mappings/v7/draftsresources/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/tests/mock_module/mappings/v7/draftsresources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/tests/mock_module/mappings/v7/draftsresources/drafts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/tests/mock_module/mappings/v7/draftsresources/drafts/draft-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/tests/mock_module/mappings/v7/draftsresources/records/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/tests/mock_module/mappings/v7/draftsresources/records/record-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/tests/mock_module/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/tests/mock_module/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/tests/mock_module/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/tests/mock_module/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/tests/mock_module/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/tests/records/
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/tests/records/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12639 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/tests/records/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/tests/resources/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6782 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/tests/resources/test_files_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/tests/resources/test_record_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/tests/resources/test_resource_links.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:19:39.000000 invenio-drafts-resources-1.6.0/tests/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/tests/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/tests/services/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13306 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/tests/services/test_record_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21966 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/tests/services/test_record_service_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/tests/services/test_record_service_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/tests/services/test_record_service_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/tests/services/test_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-21 13:19:32.000000 invenio-drafts-resources-1.6.0/tests/services/utils.py
```

### Comparing `invenio-drafts-resources-1.5.0/.editorconfig` & `invenio-drafts-resources-1.6.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/.github/workflows/pypi-publish.yml` & `invenio-drafts-resources-1.6.0/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/.github/workflows/tests.yml` & `invenio-drafts-resources-1.6.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/.tx/config` & `invenio-drafts-resources-1.6.0/.tx/config`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/CHANGES.rst` & `invenio-drafts-resources-1.6.0/CHANGES.rst`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,18 @@
     Invenio-Drafts-Resources is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
+Version 1.6.0 (2023-07-21)
+
+- Add parent id resolver
+
 Version 1.5.0 (2023-07-11)
 
 - add media files components
 
 Version 1.4.2 (2023-07-05)
 
 - transifex: update config
```

### Comparing `invenio-drafts-resources-1.5.0/CONTRIBUTING.rst` & `invenio-drafts-resources-1.6.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/LICENSE` & `invenio-drafts-resources-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/MANIFEST.in` & `invenio-drafts-resources-1.6.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/PKG-INFO` & `invenio-drafts-resources-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-drafts-resources
-Version: 1.5.0
+Version: 1.6.0
 Summary: Invenio Drafts Resources module to create REST APIs
 Home-page: https://github.com/inveniosoftware/Invenio-Drafts-Resources
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2020 CERN.
@@ -47,14 +47,18 @@
             Invenio-Drafts-Resources is free software; you can redistribute it and/or
             modify it under the terms of the MIT License; see LICENSE file for more
             details.
         
         Changes
         =======
         
+        Version 1.6.0 (2023-07-21)
+        
+        - Add parent id resolver
+        
         Version 1.5.0 (2023-07-11)
         
         - add media files components
         
         Version 1.4.2 (2023-07-05)
         
         - transifex: update config
```

### Comparing `invenio-drafts-resources-1.5.0/README.rst` & `invenio-drafts-resources-1.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/babel.ini` & `invenio-drafts-resources-1.6.0/babel.ini`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/docs/Makefile` & `invenio-drafts-resources-1.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/docs/conf.py` & `invenio-drafts-resources-1.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/docs/index.rst` & `invenio-drafts-resources-1.6.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/docs/make.bat` & `invenio-drafts-resources-1.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/records/__init__.py` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/records/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/records/api.py` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/records/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2020-2021 CERN.
+# Copyright (C) 2020-2023 CERN.
 # Copyright (C) 2021 Northwestern University.
 #
 # Invenio-Drafts-Resources is free software; you can redistribute it and/or
 # modify it under the terms of the MIT License; see LICENSE file for more
 # details.
 
 """Record, Draft and Parent Record API classes.
@@ -88,23 +88,22 @@
 
     #: Version relationship
     versions = VersionsField(create=True, set_latest=True)
 
     @classmethod
     def get_records_by_parent(cls, parent, include_deleted=True):
         """Get all sibling records for the specified parent record."""
-        query = cls.model_cls.query.filter_by(parent_id=parent.id)
+        versions = cls.model_cls.query.filter_by(parent_id=parent.id)
         if not include_deleted:
-            query = query.filter_by(is_deleted=False)
-        versions = query.all()
+            versions = versions.filter_by(is_deleted=False)
 
-        return [
+        return (
             cls(rec_model.data, model=rec_model, parent=parent)
             for rec_model in versions
-        ]
+        )
 
     @classmethod
     def publish(cls, draft):
         """Publish a draft as a new record.
 
         If a record already exists, we simply get the record. If a draft has
         not yet been published, we create the record.
```

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/records/models.py` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/records/models.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/records/systemfields/parent.py` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/records/systemfields/parent.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/records/systemfields/versions.py` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/records/systemfields/versions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2021 CERN.
+# Copyright (C) 2021-2023 CERN.
 #
 # Invenio-Drafts-Resources is free software; you can redistribute it and/or
 # modify it under the terms of the MIT License; see LICENSE file for more
 # details.
 
 """Versions field."""
 
 import uuid
-from copy import copy
 
 from invenio_db import db
-from invenio_records.systemfields import RelatedModelField
+from invenio_records.systemfields import SystemFieldContext
 from invenio_records.systemfields.base import SystemField
-from sqlalchemy import inspect
-from sqlalchemy.exc import IntegrityError
 
 
 def uuid_or_none(val):
     """Convert string to UUID object."""
     if val is not None and not isinstance(val, uuid.UUID):
         return uuid.UUID(val)
     return val
@@ -162,14 +159,27 @@
             f"<{type(self).__name__} (parent_id: {self.parent_id}, "
             f"index: {self.index}, latest_id: {self.latest_id}, "
             f"latest_index: {self.latest_index}, "
             f"next_draft_id: {self.next_draft_id})>"
         )
 
 
+class VersionsFieldContext(SystemFieldContext):
+    """Version field context."""
+
+    @property
+    def model_cls(self):
+        """Versions model class."""
+        return self.record_cls.versions_model_cls
+
+    def resolve(self, *, parent_id):
+        """Resolve a versions state from a parent ID."""
+        return self.model_cls.query.filter_by(parent_id=parent_id).one()
+
+
 class VersionsField(SystemField):
     """Versions field."""
 
     def __init__(self, create=True, set_next=False, set_latest=False):
         """Initialise the versions field."""
         self._create = create
         self._set_next = set_next
@@ -236,15 +246,15 @@
             # Access by object
             record.versions
             # Access by object
             Record.versions
         """
         if record is None:
             # access by class
-            return self
+            return VersionsFieldContext(self, owner)
         # access by object
         return self.obj(record)
 
     def __set__(self, record, obj):
         """Assign a value to the field.
 
         Called when a value is assigned to the field, e.g.:
```

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/resources/records/args.py` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/resources/records/args.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/resources/records/config.py` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/resources/records/config.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/resources/records/errors.py` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/resources/records/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/resources/records/resource.py` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/resources/records/resource.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/services/records/components/__init__.py` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/services/records/components/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/services/records/components/base.py` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/services/records/components/base.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/services/records/components/files.py` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/services/records/components/files.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/services/records/components/media_files.py` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/services/records/components/media_files.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/services/records/components/metadata.py` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/services/records/components/metadata.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/services/records/components/pid.py` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/services/records/components/pid.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/services/records/components/relations.py` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/services/records/components/relations.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/services/records/config.py` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/services/records/config.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/services/records/permissions.py` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/services/records/permissions.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/services/records/schema.py` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/services/records/schema.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/services/records/search_params.py` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/services/records/search_params.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/services/records/service.py` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/services/records/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 #
 # Invenio-Drafts-Resources is free software; you can redistribute it and/or
 # modify it under the terms of the MIT License; see LICENSE file for more
 # details.
 
 """Primary service for working with records and drafts."""
 
+import itertools
+
 from flask import current_app
 from invenio_db import db
 from invenio_records_resources.services import LinksTemplate
 from invenio_records_resources.services import RecordService as RecordServiceBase
 from invenio_records_resources.services import ServiceSchemaWrapper
 from invenio_records_resources.services.uow import (
     RecordCommitOp,
@@ -602,15 +604,15 @@
         siblings = self.record_cls.get_records_by_parent(_parent, include_deleted=False)
 
         if self.draft_cls is not None:
             # if drafts are available, reindex them as well
             drafts = self.draft_cls.get_records_by_parent(
                 _parent, include_deleted=False
             )
-            siblings.extend(drafts)
+            siblings = itertools.chain(siblings, drafts)
 
         # TODO only index the current record immediately;
         #      all siblings should be sent to a high-priority celery task
         #      instead (requires bulk indexing to work)
         for sibling in siblings:
             uow.register(RecordIndexOp(sibling, indexer=self.indexer))
```

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/services/records/tasks.py` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/services/records/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/af/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/af/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/af/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/af/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ar/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/ar/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ar/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/ar/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/bg/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/bg/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/bg/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/bg/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ca/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/ca/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ca/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/ca/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/cs/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/cs/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/cs/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/cs/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/da/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/da/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/da/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/da/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/de/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/de/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/de/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/de_AT/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/de_AT/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/de_AT/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/de_AT/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/de_DE/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/de_DE/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/de_DE/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/de_DE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/el/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/el/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/el/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/el/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/en_AT/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/en_AT/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/en_AT/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/en_AT/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/en_HU/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/en_HU/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/es/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/es/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/es_CU/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/es_CU/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/es_CU/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/es_CU/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/es_MX/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/es_MX/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/es_MX/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/es_MX/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/et/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/et/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/et/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/et/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/et_EE/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/et_EE/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/et_EE/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/et_EE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/fa/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/fa/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/fa/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/fa/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/fa_IR/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/fa_IR/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/fa_IR/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/fa_IR/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/fr/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/fr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/fr/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/fr_CI/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/fr_CI/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/fr_CI/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/fr_CI/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/fr_FR/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/fr_FR/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/fr_FR/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/fr_FR/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/gl/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/gl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/gl/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/gl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/hi_IN/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/hi_IN/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/hi_IN/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/hi_IN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/hr/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/hr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/hr/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/hr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/hu/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/hu/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/hu/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/hu/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/hu_HU/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/hu_HU/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/hu_HU/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/hu_HU/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/it/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/it/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/it/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/it/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ja/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/ja/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ja/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/ja/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ka/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/ka/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ka/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/ka/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/lt/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/lt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/lt/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/lt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/messages.pot` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ne/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/ne/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ne/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/ne/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/no/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/no/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/no/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/no/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/pl/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/pl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/pl/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/pl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/pt/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/pt/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ro/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/ro/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ro/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/ro/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ru/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/ru/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ru/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/ru/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/rw/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/rw/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/rw/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/rw/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/sk/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/sk/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/sk/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/sk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/sv/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/sv/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/sv/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/sv/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/sv_SE/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/sv_SE/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/sv_SE/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/sv_SE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/tr/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/tr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/tr/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/tr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/uk/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/uk/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/uk/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/uk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/uk_UA/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/uk_UA/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/uk_UA/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/uk_UA/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/zh_CN/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/zh_CN/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/zh_CN/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/zh_CN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/zh_TW/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/zh_TW/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/zh_TW/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources/translations/zh_TW/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources.egg-info/PKG-INFO` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-drafts-resources
-Version: 1.5.0
+Version: 1.6.0
 Summary: Invenio Drafts Resources module to create REST APIs
 Home-page: https://github.com/inveniosoftware/Invenio-Drafts-Resources
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2020 CERN.
@@ -47,14 +47,18 @@
             Invenio-Drafts-Resources is free software; you can redistribute it and/or
             modify it under the terms of the MIT License; see LICENSE file for more
             details.
         
         Changes
         =======
         
+        Version 1.6.0 (2023-07-21)
+        
+        - Add parent id resolver
+        
         Version 1.5.0 (2023-07-11)
         
         - add media files components
         
         Version 1.4.2 (2023-07-05)
         
         - transifex: update config
```

### Comparing `invenio-drafts-resources-1.5.0/invenio_drafts_resources.egg-info/SOURCES.txt` & `invenio-drafts-resources-1.6.0/invenio_drafts_resources.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/run-tests.sh` & `invenio-drafts-resources-1.6.0/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/setup.cfg` & `invenio-drafts-resources-1.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/tests/conftest.py` & `invenio-drafts-resources-1.6.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/tests/mock_module/api.py` & `invenio-drafts-resources-1.6.0/tests/mock_module/api.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/tests/mock_module/mappings/os-v1/draftsresources/drafts/draft-v1.0.0.json` & `invenio-drafts-resources-1.6.0/tests/mock_module/mappings/os-v1/draftsresources/drafts/draft-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/tests/mock_module/mappings/os-v1/draftsresources/records/record-v1.0.0.json` & `invenio-drafts-resources-1.6.0/tests/mock_module/mappings/os-v1/draftsresources/records/record-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/tests/mock_module/mappings/os-v2/draftsresources/drafts/draft-v1.0.0.json` & `invenio-drafts-resources-1.6.0/tests/mock_module/mappings/os-v2/draftsresources/drafts/draft-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/tests/mock_module/mappings/os-v2/draftsresources/records/record-v1.0.0.json` & `invenio-drafts-resources-1.6.0/tests/mock_module/mappings/os-v2/draftsresources/records/record-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/tests/mock_module/mappings/v7/draftsresources/drafts/draft-v1.0.0.json` & `invenio-drafts-resources-1.6.0/tests/mock_module/mappings/v7/draftsresources/drafts/draft-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/tests/mock_module/mappings/v7/draftsresources/records/record-v1.0.0.json` & `invenio-drafts-resources-1.6.0/tests/mock_module/mappings/v7/draftsresources/records/record-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/tests/mock_module/models.py` & `invenio-drafts-resources-1.6.0/tests/mock_module/models.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/tests/mock_module/permissions.py` & `invenio-drafts-resources-1.6.0/tests/mock_module/permissions.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/tests/mock_module/resource.py` & `invenio-drafts-resources-1.6.0/tests/mock_module/resource.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/tests/mock_module/schemas.py` & `invenio-drafts-resources-1.6.0/tests/mock_module/schemas.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/tests/mock_module/service.py` & `invenio-drafts-resources-1.6.0/tests/mock_module/service.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/tests/records/conftest.py` & `invenio-drafts-resources-1.6.0/tests/records/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/tests/records/test_api.py` & `invenio-drafts-resources-1.6.0/tests/records/test_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -307,48 +307,72 @@
 #
 def test_get_records_by_parent(app, db, location):
     """Test get by parent."""
     # Create two published records
     draft_v1 = Draft.create({})
     db.session.commit()
     parent = draft_v1.parent
-    drafts = Draft.get_records_by_parent(parent)
+    drafts = list(Draft.get_records_by_parent(parent))
     assert len(drafts) == 1
     assert id(parent) == id(drafts[0].parent)
-    records = Record.get_records_by_parent(parent)
+    records = list(Record.get_records_by_parent(parent))
     assert len(records) == 0
 
+    state = Draft.versions.resolve(parent_id=parent.id)
+    assert state == Record.versions.resolve(parent_id=parent.id)
+    assert state.latest_id is None
+    assert state.latest_index is None
+    assert state.next_draft_id == draft_v1.id
+
     record_v1 = Record.publish(draft_v1)
     draft_v1.delete()  # simulate service `publish`, will soft delete drafts
     db.session.commit()
     parent = record_v1.parent
-    drafts = Draft.get_records_by_parent(parent)
+    drafts = list(Draft.get_records_by_parent(parent))
     assert len(drafts) == 1
     assert id(parent) == id(drafts[0].parent)
-    drafts = Draft.get_records_by_parent(parent, include_deleted=False)
+    drafts = list(Draft.get_records_by_parent(parent, include_deleted=False))
     assert len(drafts) == 0
-    records = Record.get_records_by_parent(parent)
+    records = list(Record.get_records_by_parent(parent))
     assert len(records) == 1
     assert id(parent) == id(records[0].parent)
 
+    state = Record.versions.resolve(parent_id=parent.id)
+    assert state == Draft.versions.resolve(parent_id=parent.id)
+    assert state.latest_id == record_v1.id
+    assert state.latest_index == 1
+    assert state.next_draft_id is None
+
     draft_v2 = Draft.new_version(record_v1)
     draft_v2.commit()
     parent = draft_v2.parent
     db.session.commit()
-    drafts = Draft.get_records_by_parent(parent)
+    drafts = list(Draft.get_records_by_parent(parent))
     assert len(drafts) == 2
     assert id(parent) == id(drafts[0].parent)
-    records = Record.get_records_by_parent(record_v1.parent)
+    records = list(Record.get_records_by_parent(record_v1.parent))
     assert len(records) == 1
     assert id(record_v1.parent) == id(records[0].parent)
 
+    state = Draft.versions.resolve(parent_id=parent.id)
+    assert state == Record.versions.resolve(parent_id=parent.id)
+    assert state.latest_id == record_v1.id
+    assert state.latest_index == 1
+    assert state.next_draft_id == draft_v2.id
+
     record_v2 = Record.publish(draft_v2)
     draft_v2.delete()  # simulate service `publish`, will soft delete drafts
     db.session.commit()
     parent = record_v2.parent
-    drafts = Draft.get_records_by_parent(parent)
+    drafts = list(Draft.get_records_by_parent(parent))
     assert len(drafts) == 2
-    drafts = Draft.get_records_by_parent(parent, include_deleted=False)
+    drafts = list(Draft.get_records_by_parent(parent, include_deleted=False))
     assert len(drafts) == 0
-    records = Record.get_records_by_parent(parent)
+    records = list(Record.get_records_by_parent(parent))
     assert len(records) == 2
     assert id(parent) == id(records[0].parent) == id(records[1].parent)
+
+    state = Record.versions.resolve(parent_id=parent.id)
+    assert state == Draft.versions.resolve(parent_id=parent.id)
+    assert state.latest_id == record_v2.id
+    assert state.latest_index == 2
+    assert state.next_draft_id is None
```

### Comparing `invenio-drafts-resources-1.5.0/tests/resources/conftest.py` & `invenio-drafts-resources-1.6.0/tests/resources/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/tests/resources/test_files_resource.py` & `invenio-drafts-resources-1.6.0/tests/resources/test_files_resource.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/tests/resources/test_record_resource.py` & `invenio-drafts-resources-1.6.0/tests/resources/test_record_resource.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/tests/resources/test_resource_links.py` & `invenio-drafts-resources-1.6.0/tests/resources/test_resource_links.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/tests/services/conftest.py` & `invenio-drafts-resources-1.6.0/tests/services/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/tests/services/test_record_service.py` & `invenio-drafts-resources-1.6.0/tests/services/test_record_service.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/tests/services/test_record_service_files.py` & `invenio-drafts-resources-1.6.0/tests/services/test_record_service_files.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/tests/services/test_record_service_search.py` & `invenio-drafts-resources-1.6.0/tests/services/test_record_service_search.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/tests/services/test_record_service_tasks.py` & `invenio-drafts-resources-1.6.0/tests/services/test_record_service_tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/tests/services/test_services.py` & `invenio-drafts-resources-1.6.0/tests/services/test_services.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.5.0/tests/services/utils.py` & `invenio-drafts-resources-1.6.0/tests/services/utils.py`

 * *Files identical despite different names*

