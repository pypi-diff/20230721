# Comparing `tmp/molgenis-py-bbmri-eric-1.8.0.tar.gz` & `tmp/molgenis-py-bbmri-eric-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/jenkins/agent/workspace/enis_molgenis-py-bbmri-eric_main/dist/tmpoi69wz_0/molgenis-py-bbmri-eric-1.8.0.tar", last modified: Thu Sep 22 06:21:18 2022, max compression
+gzip compressed data, was "molgenis-py-bbmri-eric-1.9.0.tar", last modified: Thu Nov 24 08:07:53 2022, max compression
```

## Comparing `molgenis-py-bbmri-eric-1.8.0.tar` & `molgenis-py-bbmri-eric-1.9.0.tar`

### file list

```diff
@@ -1,72 +1,79 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-22 06:21:18.000000 molgenis-py-bbmri-eric-1.8.0/
--rw-r--r--   0 root         (0) root         (0)      623 2022-09-22 06:14:11.000000 molgenis-py-bbmri-eric-1.8.0/.coveragerc
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-22 06:21:18.000000 molgenis-py-bbmri-eric-1.8.0/.github/
--rw-r--r--   0 root         (0) root         (0)      194 2022-09-22 06:14:11.000000 molgenis-py-bbmri-eric-1.8.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 root         (0) root         (0)      585 2022-09-22 06:14:11.000000 molgenis-py-bbmri-eric-1.8.0/.gitignore
--rw-r--r--   0 root         (0) root         (0)       56 2022-09-22 06:14:11.000000 molgenis-py-bbmri-eric-1.8.0/.isort.cfg
--rw-r--r--   0 root         (0) root         (0)      751 2022-09-22 06:14:11.000000 molgenis-py-bbmri-eric-1.8.0/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)      115 2022-09-22 06:14:11.000000 molgenis-py-bbmri-eric-1.8.0/AUTHORS.md
--rw-r--r--   0 root         (0) root         (0)     2277 2022-09-22 06:14:11.000000 molgenis-py-bbmri-eric-1.8.0/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     5821 2022-09-22 06:14:11.000000 molgenis-py-bbmri-eric-1.8.0/Jenkinsfile
--rw-r--r--   0 root         (0) root         (0)     7651 2022-09-22 06:14:11.000000 molgenis-py-bbmri-eric-1.8.0/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     3034 2022-09-22 06:21:18.000000 molgenis-py-bbmri-eric-1.8.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      283 2022-09-22 06:14:11.000000 molgenis-py-bbmri-eric-1.8.0/Pipfile
--rw-r--r--   0 root         (0) root         (0)    24601 2022-09-22 06:14:11.000000 molgenis-py-bbmri-eric-1.8.0/Pipfile.lock
--rw-r--r--   0 root         (0) root         (0)     2342 2022-09-22 06:14:11.000000 molgenis-py-bbmri-eric-1.8.0/README.md
--rw-r--r--   0 root         (0) root         (0)      435 2022-09-22 06:14:11.000000 molgenis-py-bbmri-eric-1.8.0/bump-version.sh
--rw-r--r--   0 root         (0) root         (0)      311 2022-09-22 06:14:11.000000 molgenis-py-bbmri-eric-1.8.0/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-22 06:21:18.000000 molgenis-py-bbmri-eric-1.8.0/scripts/
--rw-r--r--   0 root         (0) root         (0)       25 2022-09-22 06:14:11.000000 molgenis-py-bbmri-eric-1.8.0/scripts/.gitignore
--rw-r--r--   0 root         (0) root         (0)     1913 2022-09-22 06:14:11.000000 molgenis-py-bbmri-eric-1.8.0/scripts/biobank_pid_assignment.py
--rw-r--r--   0 root         (0) root         (0)     1331 2022-09-22 06:14:11.000000 molgenis-py-bbmri-eric-1.8.0/scripts/example.py
--rw-r--r--   0 root         (0) root         (0)     4852 2022-09-22 06:14:11.000000 molgenis-py-bbmri-eric-1.8.0/scripts/hook.py
--rw-r--r--   0 root         (0) root         (0)     1047 2022-09-22 06:14:11.000000 molgenis-py-bbmri-eric-1.8.0/scripts/sync_DE_qualities.py
--rw-r--r--   0 root         (0) root         (0)     1567 2022-09-22 06:21:18.000000 molgenis-py-bbmri-eric-1.8.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      719 2022-09-22 06:14:11.000000 molgenis-py-bbmri-eric-1.8.0/setup.py
--rw-r--r--   0 root         (0) root         (0)      412 2022-09-22 06:14:11.000000 molgenis-py-bbmri-eric-1.8.0/sonar-project.properties
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-22 06:21:18.000000 molgenis-py-bbmri-eric-1.8.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-22 06:21:18.000000 molgenis-py-bbmri-eric-1.8.0/src/molgenis/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-22 06:21:18.000000 molgenis-py-bbmri-eric-1.8.0/src/molgenis/bbmri_eric/
--rw-r--r--   0 root         (0) root         (0)      508 2022-09-22 06:14:11.000000 molgenis-py-bbmri-eric-1.8.0/src/molgenis/bbmri_eric/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14828 2022-09-22 06:14:11.000000 molgenis-py-bbmri-eric-1.8.0/src/molgenis/bbmri_eric/bbmri_client.py
--rw-r--r--   0 root         (0) root         (0)     3338 2022-09-22 06:14:11.000000 molgenis-py-bbmri-eric-1.8.0/src/molgenis/bbmri_eric/categories.py
--rw-r--r--   0 root         (0) root         (0)     5343 2022-09-22 06:14:11.000000 molgenis-py-bbmri-eric-1.8.0/src/molgenis/bbmri_eric/eric.py
--rw-r--r--   0 root         (0) root         (0)     1915 2022-09-22 06:14:11.000000 molgenis-py-bbmri-eric-1.8.0/src/molgenis/bbmri_eric/errors.py
--rw-r--r--   0 root         (0) root         (0)    10437 2022-09-22 06:14:11.000000 molgenis-py-bbmri-eric-1.8.0/src/molgenis/bbmri_eric/model.py
--rw-r--r--   0 root         (0) root         (0)     4302 2022-09-22 06:14:11.000000 molgenis-py-bbmri-eric-1.8.0/src/molgenis/bbmri_eric/pid_manager.py
--rw-r--r--   0 root         (0) root         (0)     6610 2022-09-22 06:14:11.000000 molgenis-py-bbmri-eric-1.8.0/src/molgenis/bbmri_eric/pid_service.py
--rw-r--r--   0 root         (0) root         (0)     2386 2022-09-22 06:14:11.000000 molgenis-py-bbmri-eric-1.8.0/src/molgenis/bbmri_eric/printer.py
--rw-r--r--   0 root         (0) root         (0)     2713 2022-09-22 06:14:11.000000 molgenis-py-bbmri-eric-1.8.0/src/molgenis/bbmri_eric/publication_preparer.py
--rw-r--r--   0 root         (0) root         (0)     4579 2022-09-22 06:14:11.000000 molgenis-py-bbmri-eric-1.8.0/src/molgenis/bbmri_eric/publisher.py
--rw-r--r--   0 root         (0) root         (0)     1881 2022-09-22 06:14:11.000000 molgenis-py-bbmri-eric-1.8.0/src/molgenis/bbmri_eric/stager.py
--rw-r--r--   0 root         (0) root         (0)     8522 2022-09-22 06:14:11.000000 molgenis-py-bbmri-eric-1.8.0/src/molgenis/bbmri_eric/transformer.py
--rw-r--r--   0 root         (0) root         (0)     1200 2022-09-22 06:14:11.000000 molgenis-py-bbmri-eric-1.8.0/src/molgenis/bbmri_eric/utils.py
--rw-r--r--   0 root         (0) root         (0)     4757 2022-09-22 06:14:11.000000 molgenis-py-bbmri-eric-1.8.0/src/molgenis/bbmri_eric/validation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-22 06:21:18.000000 molgenis-py-bbmri-eric-1.8.0/src/molgenis_py_bbmri_eric.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3034 2022-09-22 06:21:18.000000 molgenis-py-bbmri-eric-1.8.0/src/molgenis_py_bbmri_eric.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1662 2022-09-22 06:21:18.000000 molgenis-py-bbmri-eric-1.8.0/src/molgenis_py_bbmri_eric.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-22 06:21:18.000000 molgenis-py-bbmri-eric-1.8.0/src/molgenis_py_bbmri_eric.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-22 06:14:51.000000 molgenis-py-bbmri-eric-1.8.0/src/molgenis_py_bbmri_eric.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      157 2022-09-22 06:21:18.000000 molgenis-py-bbmri-eric-1.8.0/src/molgenis_py_bbmri_eric.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2022-09-22 06:21:18.000000 molgenis-py-bbmri-eric-1.8.0/src/molgenis_py_bbmri_eric.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-22 06:21:18.000000 molgenis-py-bbmri-eric-1.8.0/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-22 06:14:11.000000 molgenis-py-bbmri-eric-1.8.0/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      748 2022-09-22 06:14:11.000000 molgenis-py-bbmri-eric-1.8.0/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-22 06:21:18.000000 molgenis-py-bbmri-eric-1.8.0/tests/resources/
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-22 06:14:11.000000 molgenis-py-bbmri-eric-1.8.0/tests/resources/__init__.py
--rw-r--r--   0 root         (0) root         (0)   100129 2022-09-22 06:14:11.000000 molgenis-py-bbmri-eric-1.8.0/tests/resources/node_data.pkl
--rw-r--r--   0 root         (0) root         (0)      798 2022-09-22 06:14:11.000000 molgenis-py-bbmri-eric-1.8.0/tests/resources/node_data_pickler.py
--rw-r--r--   0 root         (0) root         (0)     3130 2022-09-22 06:14:11.000000 molgenis-py-bbmri-eric-1.8.0/tests/test_categories.py
--rw-r--r--   0 root         (0) root         (0)     3781 2022-09-22 06:14:11.000000 molgenis-py-bbmri-eric-1.8.0/tests/test_eric.py
--rw-r--r--   0 root         (0) root         (0)     1515 2022-09-22 06:14:11.000000 molgenis-py-bbmri-eric-1.8.0/tests/test_errors.py
--rw-r--r--   0 root         (0) root         (0)     2951 2022-09-22 06:14:11.000000 molgenis-py-bbmri-eric-1.8.0/tests/test_model.py
--rw-r--r--   0 root         (0) root         (0)     2773 2022-09-22 06:14:11.000000 molgenis-py-bbmri-eric-1.8.0/tests/test_pid_manager.py
--rw-r--r--   0 root         (0) root         (0)     2902 2022-09-22 06:14:11.000000 molgenis-py-bbmri-eric-1.8.0/tests/test_pid_service.py
--rw-r--r--   0 root         (0) root         (0)     3481 2022-09-22 06:14:11.000000 molgenis-py-bbmri-eric-1.8.0/tests/test_printer.py
--rw-r--r--   0 root         (0) root         (0)     3945 2022-09-22 06:14:11.000000 molgenis-py-bbmri-eric-1.8.0/tests/test_publication_preparer.py
--rw-r--r--   0 root         (0) root         (0)     2979 2022-09-22 06:14:11.000000 molgenis-py-bbmri-eric-1.8.0/tests/test_publisher.py
--rw-r--r--   0 root         (0) root         (0)     2281 2022-09-22 06:14:11.000000 molgenis-py-bbmri-eric-1.8.0/tests/test_stager.py
--rw-r--r--   0 root         (0) root         (0)    10439 2022-09-22 06:14:11.000000 molgenis-py-bbmri-eric-1.8.0/tests/test_transformer.py
--rw-r--r--   0 root         (0) root         (0)     2077 2022-09-22 06:14:11.000000 molgenis-py-bbmri-eric-1.8.0/tests/test_utils.py
--rw-r--r--   0 root         (0) root         (0)     8839 2022-09-22 06:14:11.000000 molgenis-py-bbmri-eric-1.8.0/tests/test_validator.py
--rw-r--r--   0 root         (0) root         (0)     1939 2022-09-22 06:14:11.000000 molgenis-py-bbmri-eric-1.8.0/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 08:07:53.004933 molgenis-py-bbmri-eric-1.9.0/
+-rw-r--r--   0 root         (0) root         (0)      623 2022-11-24 07:54:54.000000 molgenis-py-bbmri-eric-1.9.0/.coveragerc
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 08:07:53.000935 molgenis-py-bbmri-eric-1.9.0/.github/
+-rw-r--r--   0 root         (0) root         (0)      194 2022-11-24 07:54:54.000000 molgenis-py-bbmri-eric-1.9.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 root         (0) root         (0)      585 2022-11-24 07:54:54.000000 molgenis-py-bbmri-eric-1.9.0/.gitignore
+-rw-r--r--   0 root         (0) root         (0)       56 2022-11-24 07:54:54.000000 molgenis-py-bbmri-eric-1.9.0/.isort.cfg
+-rw-r--r--   0 root         (0) root         (0)      752 2022-11-24 07:54:54.000000 molgenis-py-bbmri-eric-1.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)      115 2022-11-24 07:54:54.000000 molgenis-py-bbmri-eric-1.9.0/AUTHORS.md
+-rw-r--r--   0 root         (0) root         (0)     2631 2022-11-24 07:54:54.000000 molgenis-py-bbmri-eric-1.9.0/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     5826 2022-11-24 07:54:54.000000 molgenis-py-bbmri-eric-1.9.0/Jenkinsfile
+-rw-r--r--   0 root         (0) root         (0)     7651 2022-11-24 07:54:54.000000 molgenis-py-bbmri-eric-1.9.0/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     3085 2022-11-24 08:07:53.004933 molgenis-py-bbmri-eric-1.9.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      284 2022-11-24 07:54:54.000000 molgenis-py-bbmri-eric-1.9.0/Pipfile
+-rw-r--r--   0 root         (0) root         (0)    21100 2022-11-24 07:54:54.000000 molgenis-py-bbmri-eric-1.9.0/Pipfile.lock
+-rw-r--r--   0 root         (0) root         (0)     2342 2022-11-24 07:54:54.000000 molgenis-py-bbmri-eric-1.9.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      435 2022-11-24 07:54:54.000000 molgenis-py-bbmri-eric-1.9.0/bump-version.sh
+-rw-r--r--   0 root         (0) root         (0)      311 2022-11-24 07:54:54.000000 molgenis-py-bbmri-eric-1.9.0/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 08:07:53.000935 molgenis-py-bbmri-eric-1.9.0/scripts/
+-rw-r--r--   0 root         (0) root         (0)       25 2022-11-24 07:54:54.000000 molgenis-py-bbmri-eric-1.9.0/scripts/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     1913 2022-11-24 07:54:54.000000 molgenis-py-bbmri-eric-1.9.0/scripts/biobank_pid_assignment.py
+-rw-r--r--   0 root         (0) root         (0)     1331 2022-11-24 07:54:54.000000 molgenis-py-bbmri-eric-1.9.0/scripts/example.py
+-rw-r--r--   0 root         (0) root         (0)     6095 2022-11-24 07:54:54.000000 molgenis-py-bbmri-eric-1.9.0/scripts/hook.py
+-rw-r--r--   0 root         (0) root         (0)     1047 2022-11-24 07:54:54.000000 molgenis-py-bbmri-eric-1.9.0/scripts/sync_DE_qualities.py
+-rw-r--r--   0 root         (0) root         (0)     1576 2022-11-24 08:07:53.008931 molgenis-py-bbmri-eric-1.9.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      719 2022-11-24 07:54:54.000000 molgenis-py-bbmri-eric-1.9.0/setup.py
+-rw-r--r--   0 root         (0) root         (0)      412 2022-11-24 07:54:54.000000 molgenis-py-bbmri-eric-1.9.0/sonar-project.properties
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 08:07:53.000935 molgenis-py-bbmri-eric-1.9.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 08:07:53.000935 molgenis-py-bbmri-eric-1.9.0/src/molgenis/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 08:07:53.004933 molgenis-py-bbmri-eric-1.9.0/src/molgenis/bbmri_eric/
+-rw-r--r--   0 root         (0) root         (0)      508 2022-11-24 07:54:54.000000 molgenis-py-bbmri-eric-1.9.0/src/molgenis/bbmri_eric/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15920 2022-11-24 07:54:54.000000 molgenis-py-bbmri-eric-1.9.0/src/molgenis/bbmri_eric/bbmri_client.py
+-rw-r--r--   0 root         (0) root         (0)     3338 2022-11-24 07:54:54.000000 molgenis-py-bbmri-eric-1.9.0/src/molgenis/bbmri_eric/categories.py
+-rw-r--r--   0 root         (0) root         (0)     5534 2022-11-24 07:54:54.000000 molgenis-py-bbmri-eric-1.9.0/src/molgenis/bbmri_eric/eric.py
+-rw-r--r--   0 root         (0) root         (0)     1915 2022-11-24 07:54:54.000000 molgenis-py-bbmri-eric-1.9.0/src/molgenis/bbmri_eric/errors.py
+-rw-r--r--   0 root         (0) root         (0)    11279 2022-11-24 07:54:54.000000 molgenis-py-bbmri-eric-1.9.0/src/molgenis/bbmri_eric/model.py
+-rw-r--r--   0 root         (0) root         (0)     6323 2022-11-24 07:54:54.000000 molgenis-py-bbmri-eric-1.9.0/src/molgenis/bbmri_eric/model_fitting.py
+-rw-r--r--   0 root         (0) root         (0)     4302 2022-11-24 07:54:54.000000 molgenis-py-bbmri-eric-1.9.0/src/molgenis/bbmri_eric/pid_manager.py
+-rw-r--r--   0 root         (0) root         (0)     6610 2022-11-24 07:54:54.000000 molgenis-py-bbmri-eric-1.9.0/src/molgenis/bbmri_eric/pid_service.py
+-rw-r--r--   0 root         (0) root         (0)     2386 2022-11-24 07:54:54.000000 molgenis-py-bbmri-eric-1.9.0/src/molgenis/bbmri_eric/printer.py
+-rw-r--r--   0 root         (0) root         (0)     3250 2022-11-24 07:54:54.000000 molgenis-py-bbmri-eric-1.9.0/src/molgenis/bbmri_eric/publication_preparer.py
+-rw-r--r--   0 root         (0) root         (0)     4579 2022-11-24 07:54:54.000000 molgenis-py-bbmri-eric-1.9.0/src/molgenis/bbmri_eric/publisher.py
+-rw-r--r--   0 root         (0) root         (0)     2676 2022-11-24 07:54:54.000000 molgenis-py-bbmri-eric-1.9.0/src/molgenis/bbmri_eric/stager.py
+-rw-r--r--   0 root         (0) root         (0)     7477 2022-11-24 07:54:54.000000 molgenis-py-bbmri-eric-1.9.0/src/molgenis/bbmri_eric/transformer.py
+-rw-r--r--   0 root         (0) root         (0)     1200 2022-11-24 07:54:54.000000 molgenis-py-bbmri-eric-1.9.0/src/molgenis/bbmri_eric/utils.py
+-rw-r--r--   0 root         (0) root         (0)     4876 2022-11-24 07:54:54.000000 molgenis-py-bbmri-eric-1.9.0/src/molgenis/bbmri_eric/validation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 08:07:53.004933 molgenis-py-bbmri-eric-1.9.0/src/molgenis_py_bbmri_eric.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3085 2022-11-24 08:07:52.000000 molgenis-py-bbmri-eric-1.9.0/src/molgenis_py_bbmri_eric.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1885 2022-11-24 08:07:52.000000 molgenis-py-bbmri-eric-1.9.0/src/molgenis_py_bbmri_eric.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-24 08:07:52.000000 molgenis-py-bbmri-eric-1.9.0/src/molgenis_py_bbmri_eric.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-24 07:55:40.000000 molgenis-py-bbmri-eric-1.9.0/src/molgenis_py_bbmri_eric.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      121 2022-11-24 08:07:52.000000 molgenis-py-bbmri-eric-1.9.0/src/molgenis_py_bbmri_eric.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2022-11-24 08:07:52.000000 molgenis-py-bbmri-eric-1.9.0/src/molgenis_py_bbmri_eric.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 08:07:53.004933 molgenis-py-bbmri-eric-1.9.0/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-24 07:54:54.000000 molgenis-py-bbmri-eric-1.9.0/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2222 2022-11-24 07:54:54.000000 molgenis-py-bbmri-eric-1.9.0/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 08:07:53.004933 molgenis-py-bbmri-eric-1.9.0/tests/resources/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-24 07:54:54.000000 molgenis-py-bbmri-eric-1.9.0/tests/resources/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      323 2022-11-24 07:54:54.000000 molgenis-py-bbmri-eric-1.9.0/tests/resources/also_known.json
+-rw-r--r--   0 root         (0) root         (0)     1238 2022-11-24 07:54:54.000000 molgenis-py-bbmri-eric-1.9.0/tests/resources/biobanks.json
+-rw-r--r--   0 root         (0) root         (0)     2281 2022-11-24 07:54:54.000000 molgenis-py-bbmri-eric-1.9.0/tests/resources/collections.json
+-rw-r--r--   0 root         (0) root         (0)      626 2022-11-24 07:54:54.000000 molgenis-py-bbmri-eric-1.9.0/tests/resources/networks.json
+-rw-r--r--   0 root         (0) root         (0)   100129 2022-11-24 07:54:54.000000 molgenis-py-bbmri-eric-1.9.0/tests/resources/node_data.pkl
+-rw-r--r--   0 root         (0) root         (0)      798 2022-11-24 07:54:54.000000 molgenis-py-bbmri-eric-1.9.0/tests/resources/node_data_pickler.py
+-rw-r--r--   0 root         (0) root         (0)      446 2022-11-24 07:54:54.000000 molgenis-py-bbmri-eric-1.9.0/tests/resources/persons.json
+-rw-r--r--   0 root         (0) root         (0)     3130 2022-11-24 07:54:54.000000 molgenis-py-bbmri-eric-1.9.0/tests/test_categories.py
+-rw-r--r--   0 root         (0) root         (0)     3876 2022-11-24 07:54:54.000000 molgenis-py-bbmri-eric-1.9.0/tests/test_eric.py
+-rw-r--r--   0 root         (0) root         (0)     1515 2022-11-24 07:54:54.000000 molgenis-py-bbmri-eric-1.9.0/tests/test_errors.py
+-rw-r--r--   0 root         (0) root         (0)     3232 2022-11-24 07:54:54.000000 molgenis-py-bbmri-eric-1.9.0/tests/test_model.py
+-rw-r--r--   0 root         (0) root         (0)     3720 2022-11-24 07:54:54.000000 molgenis-py-bbmri-eric-1.9.0/tests/test_model_fitting.py
+-rw-r--r--   0 root         (0) root         (0)     2773 2022-11-24 07:54:54.000000 molgenis-py-bbmri-eric-1.9.0/tests/test_pid_manager.py
+-rw-r--r--   0 root         (0) root         (0)     2902 2022-11-24 07:54:54.000000 molgenis-py-bbmri-eric-1.9.0/tests/test_pid_service.py
+-rw-r--r--   0 root         (0) root         (0)     3481 2022-11-24 07:54:54.000000 molgenis-py-bbmri-eric-1.9.0/tests/test_printer.py
+-rw-r--r--   0 root         (0) root         (0)     5063 2022-11-24 07:54:54.000000 molgenis-py-bbmri-eric-1.9.0/tests/test_publication_preparer.py
+-rw-r--r--   0 root         (0) root         (0)     3362 2022-11-24 07:54:54.000000 molgenis-py-bbmri-eric-1.9.0/tests/test_publisher.py
+-rw-r--r--   0 root         (0) root         (0)     3137 2022-11-24 07:54:54.000000 molgenis-py-bbmri-eric-1.9.0/tests/test_stager.py
+-rw-r--r--   0 root         (0) root         (0)     9325 2022-11-24 07:54:54.000000 molgenis-py-bbmri-eric-1.9.0/tests/test_transformer.py
+-rw-r--r--   0 root         (0) root         (0)     2077 2022-11-24 07:54:54.000000 molgenis-py-bbmri-eric-1.9.0/tests/test_utils.py
+-rw-r--r--   0 root         (0) root         (0)     5344 2022-11-24 07:54:54.000000 molgenis-py-bbmri-eric-1.9.0/tests/test_validator.py
+-rw-r--r--   0 root         (0) root         (0)     1939 2022-11-24 07:54:54.000000 molgenis-py-bbmri-eric-1.9.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `molgenis-py-bbmri-eric-1.8.0/.coveragerc` & `molgenis-py-bbmri-eric-1.9.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `molgenis-py-bbmri-eric-1.8.0/.gitignore` & `molgenis-py-bbmri-eric-1.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `molgenis-py-bbmri-eric-1.8.0/.pre-commit-config.yaml` & `molgenis-py-bbmri-eric-1.9.0/.pre-commit-config.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 exclude: '^docs/conf.py'
 
 repos:
 - repo: https://github.com/pre-commit/pre-commit-hooks
-  rev: v4.2.0
+  rev: v4.3.0
   hooks:
   - id: trailing-whitespace
   - id: check-added-large-files
   - id: check-ast
   - id: check-json
   - id: check-merge-conflict
   - id: check-xml
@@ -19,16 +19,16 @@
 
 - repo: https://github.com/pycqa/isort
   rev: 5.10.1
   hooks:
   - id: isort
 
 - repo: https://github.com/psf/black
-  rev: 22.3.0
+  rev: 22.10.0
   hooks:
   - id: black
     language_version: python3
 
-- repo: https://gitlab.com/pycqa/flake8
-  rev: 3.9.2
+- repo: https://github.com/pycqa/flake8
+  rev: 5.0.4
   hooks:
   - id: flake8
```

### Comparing `molgenis-py-bbmri-eric-1.8.0/CHANGELOG.md` & `molgenis-py-bbmri-eric-1.9.0/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # Changelog
-## Version 1.8.0 (development)
+## Version 1.10.0 (development)
+
+## Version 1.9.0
+BBMRI-model changes as described in this [document](https://docs.google.com/document/d/1h-xkU6uR8jytDnMm7wT38bk0ZdmXzywZ/edit?usp=sharing&ouid=103886117563984453369&rtpof=true&sd=true).
+Main changes are:
+- Add also_known_in tables and column to staging areas
+- Move head info from biobanks and collections to persons
+
+## Version 1.8.0
 - The 'combined quality' field in collections is automatically filled during publishing
 - The 'biobank_label' field in collections is automatically filled during publishing
 
 ## Version 1.7.0
 - The 'categories' field in collections is automatically filled during publishing
 - The 'covid19biobank' column is merged into the 'capabilities' column during publishing
```

### Comparing `molgenis-py-bbmri-eric-1.8.0/Jenkinsfile` & `molgenis-py-bbmri-eric-1.9.0/Jenkinsfile`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 pipeline {
     agent {
         kubernetes {
             // the shared pod template defined on the Jenkins server config
             inheritFrom 'shared'
             // pod template defined in molgenis/molgenis-jenkins-pipeline repository
-            yaml libraryResource("pod-templates/python.yaml")
+            yaml libraryResource("pod-templates/python-3.10.yaml")
         }
     }
     stages {
         stage('Prepare') {
             steps {
                 script {
                     env.GIT_COMMIT = sh(script: 'git rev-parse HEAD', returnStdout: true).trim()
```

### Comparing `molgenis-py-bbmri-eric-1.8.0/LICENSE.txt` & `molgenis-py-bbmri-eric-1.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `molgenis-py-bbmri-eric-1.8.0/PKG-INFO` & `molgenis-py-bbmri-eric-1.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: molgenis-py-bbmri-eric
-Version: 1.8.0
+Version: 1.9.0
 Summary: MOLGENIS Python tooling for BBMRI-ERIC
 Home-page: https://github.com/molgenis/molgenis-py-bbmri-eric
 Author: Tommy de Boer
 Author-email: t.de.boer01@umcg.nl
 License: LGPL-3.0-only
 Project-URL: Source, https://github.com/molgenis/molgenis-py-bbmri-eric
 Platform: any
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Provides-Extra: testing
 License-File: LICENSE.txt
 License-File: AUTHORS.md
 
 # molgenis-py-bbmri-eric
```

### Comparing `molgenis-py-bbmri-eric-1.8.0/Pipfile.lock` & `molgenis-py-bbmri-eric-1.9.0/Pipfile.lock`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8462016511585477%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'17db686f0c6c16c8d102de5497447a49138e65d50d30820fef767bdd288cc054'}, 'requires': "*

 * *            "{'python_version': '3.10'}}",*

 * * "'default'": "{'certifi': {'hashes': "*

 * *              "['sha256:0d9c601124e5a6ba9712dbc60d9c53c21e34f5f641fe83002317394311bdce14', "*

 * *              "'sha256:90c1a32f1d68f940488354e36370f6cca89f0f106db09518524c88d6ed83f382'], "*

 * *              '\'version\': \'==2022.9.24\', \'markers\': "python_version >= \'3.6\'"}, '*

 * *              "'datacl […]*

```diff
@@ -1,357 +1,315 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "68331fafe22b24d7110a2dfc7a2638bc927c72799a108e74f5e1beff590af6ce"
+            "sha256": "17db686f0c6c16c8d102de5497447a49138e65d50d30820fef767bdd288cc054"
         },
         "pipfile-spec": 6,
         "requires": {
-            "python_version": "3.6"
+            "python_version": "3.10"
         },
         "sources": [
             {
                 "name": "pypi",
                 "url": "https://pypi.org/simple",
                 "verify_ssl": true
             }
         ]
     },
     "default": {
         "certifi": {
             "hashes": [
-                "sha256:78884e7c1d4b00ce3cea67b44566851c4343c120abd683433ce934a68ea58872",
-                "sha256:d62a0163eb4c2344ac042ab2bdf75399a71a2d8c7d47eac2e2ee91b9d6339569"
+                "sha256:0d9c601124e5a6ba9712dbc60d9c53c21e34f5f641fe83002317394311bdce14",
+                "sha256:90c1a32f1d68f940488354e36370f6cca89f0f106db09518524c88d6ed83f382"
             ],
-            "version": "==2021.10.8"
+            "markers": "python_version >= '3.6'",
+            "version": "==2022.9.24"
         },
-        "charset-normalizer": {
+        "chardet": {
             "hashes": [
-                "sha256:1eecaa09422db5be9e29d7fc65664e6c33bd06f9ced7838578ba40d58bdf3721",
-                "sha256:b0b883e8e874edfdece9c28f314e3dd5badf067342e42fb162203335ae61aa2c"
+                "sha256:84ab92ed1c4d4f16916e05906b6b75a6c0fb5db821cc65e70cbd64a3e2a5eaae",
+                "sha256:fc323ffcaeaed0e0a02bf4d117757b98aed530d9ed4531e3e15460124c106691"
             ],
-            "markers": "python_version >= '3'",
-            "version": "==2.0.9"
+            "version": "==3.0.4"
         },
         "dataclasses": {
             "hashes": [
-                "sha256:0201d89fa866f68c8ebd9d08ee6ff50c0b255f8ec63a71c16fda7af82bb887bf",
-                "sha256:8479067f342acf957dc82ec415d355ab5edb7e7646b90dc6e2fd1d96ad084c97"
+                "sha256:454a69d788c7fda44efd71e259be79577822f5e3f53f029a22d08004e951dc9f",
+                "sha256:6988bd2b895eef432d562370bb707d540f32f7360ab13da45340101bc2307d84"
             ],
-            "markers": "python_version >= '3.6' and python_version < '3.7'",
-            "version": "==0.8"
+            "version": "==0.6"
         },
         "datetime": {
             "hashes": [
-                "sha256:371dba07417b929a4fa685c2f7a3eaa6a62d60c02947831f97d4df9a9e70dfd0",
-                "sha256:5cef605bab8259ff61281762cdf3290e459fbf0b4719951d5fab967d5f2ea0ea"
+                "sha256:7ff7c4a857f08b73db17a85fc54f102d065ad16e7db0133e699c5f1b37e41478",
+                "sha256:b8d2d605cfb5fed0da86f9ad64d0973c6f84b21939d49265e135811b33ee8113"
             ],
-            "version": "==4.3"
+            "version": "==4.7"
         },
         "future": {
             "hashes": [
                 "sha256:b1bead90b70cf6ec3f0710ae53a525360fa360d306a86583adc6bf83a4db537d"
             ],
             "markers": "python_version >= '2.6' and python_version not in '3.0, 3.1, 3.2'",
             "version": "==0.18.2"
         },
         "idna": {
             "hashes": [
-                "sha256:84d9dd047ffa80596e0f246e2eab0b391788b0503584e8945f2368256d2735ff",
-                "sha256:9d643ff0a55b762d5cdb124b8eaa99c66322e2157b69160bc32796e824360e6d"
-            ],
-            "markers": "python_version >= '3'",
-            "version": "==3.3"
-        },
-        "importlib-metadata": {
-            "hashes": [
-                "sha256:65a9576a5b2d58ca44d133c42a241905cc45e34d2c06fd5ba2bafa221e5d7b5e",
-                "sha256:766abffff765960fcc18003801f7044eb6755ffae4521c8e8ce8e83b9c9b0668"
+                "sha256:b307872f855b18632ce0c21c5e45be78c0ea7ae4c15c828c20788b26921eb3f6",
+                "sha256:b97d804b1e9b523befed77c48dacec60e6dcb0b5391d57af6a65a312a90648c0"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==4.8.3"
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
+            "version": "==2.10"
         },
         "molgenis-py-bbmri-eric": {
             "editable": true,
             "path": "."
         },
         "molgenis-py-client": {
             "hashes": [
                 "sha256:7c57abb1e6ed05fa72837cc314066bdf6c1dfbbed7e5a080ea65fa2606497c50",
                 "sha256:aa839f0cfe40b7afad071634e7cbb2f01ce4d7daca425256dc4649b0b4332d31"
             ],
             "version": "==2.3.1"
         },
         "pyhandle": {
             "hashes": [
-                "sha256:f3d819e93c2e174730af7b9576c926ffcbd7bc60e24cb033e575cb43935beb1c"
+                "sha256:d2ff59263c061c51ab7e2d0e69e1d8549600da4e64a2cacee11469bb4b67e4ab"
             ],
-            "version": "==1.0.4"
+            "markers": "python_version >= '3.6' and python_version < '3.11'",
+            "version": "==1.1.1"
         },
         "pymysql": {
             "hashes": [
-                "sha256:41fc3a0c5013d5f039639442321185532e3e2c8924687abe6537de157d403641",
-                "sha256:816927a350f38d56072aeca5dfb10221fe1dc653745853d30a216637f5d7ad36"
+                "sha256:04fa19fad017fdb21394fad2878c1d6bd346959d4fbfd1b66050a09fc636a321",
+                "sha256:32da4a66397077d42908e449688f2ec71c2b18892a6cd04f03ab2aa828a70f40"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==1.0.2"
+            "markers": "python_version < '3.11.0'",
+            "version": "==0.8.0"
         },
         "pytz": {
             "hashes": [
-                "sha256:3672058bc3453457b622aab7a1c3bfd5ab0bdae451512f6cf25f64ed37f5b87c",
-                "sha256:acad2d8b20a1af07d4e4c9d2e9285c5ed9104354062f275f3fcd88dcef4f1326"
+                "sha256:222439474e9c98fced559f1709d89e6c9cbf8d79c794ff3eb9f8800064291427",
+                "sha256:e89512406b793ca39f5971bc999cc538ce125c0e51c27941bef4568b460095e2"
             ],
-            "version": "==2021.3"
+            "version": "==2022.6"
         },
         "requests": {
             "hashes": [
-                "sha256:6c1246513ecd5ecd4528a0906f910e8f0f9c6b8ec72030dc9fd154dc1a6efd24",
-                "sha256:b8aa58f8cf793ffd8782d3d8cb19e66ef36f7aba4353eec859e74678b01b07a7"
+                "sha256:43999036bfa82904b6af1d99e4882b560e5e2c68e5c4b0aa03b655f3d7d73fee",
+                "sha256:5d2d0ffbb515f39417009a46c14256291061ac01ba8f875b90cad137de83beb4",
+                "sha256:b3f43d496c6daba4493e7c431722aeb7dbc6288f52a6e04e7b6023b0247817e6"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
-            "version": "==2.26.0"
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
+            "version": "==2.23.0"
         },
         "setuptools": {
             "hashes": [
-                "sha256:22c7348c6d2976a52632c67f7ab0cdf40147db7789f9aed18734643fe9cf3373",
-                "sha256:4ce92f1e1f8f01233ee9952c04f6b81d1e02939d6e1b488428154974a4d0783e"
+                "sha256:6211d2f5eddad8757bd0484923ca7c0a6302ebc4ab32ea5e94357176e0ca0840",
+                "sha256:d1eebf881c6114e51df1664bc2c9133d022f78d12d5f4f665b9191f084e2862d"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==59.6.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==65.6.0"
         },
         "six": {
             "hashes": [
                 "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926",
                 "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2'",
             "version": "==1.16.0"
         },
-        "typing-extensions": {
+        "unidecode": {
             "hashes": [
-                "sha256:4ca091dea149f945ec56afb48dae714f21e8692ef22a395223bcd328961b6a0e",
-                "sha256:7f001e5ac290a0c0401508864c7ec868be4e701886d5b573a9528ed3973d9d3b"
+                "sha256:547d7c479e4f377b430dd91ac1275d593308dce0fc464fb2ab7d41f82ec653be",
+                "sha256:fed09cf0be8cf415b391642c2a5addfc72194407caee4f98719e40ec2a72b830"
             ],
-            "markers": "python_version < '3.8'",
-            "version": "==4.0.1"
+            "markers": "python_version >= '3.5'",
+            "version": "==1.3.6"
         },
         "urllib3": {
             "hashes": [
-                "sha256:4987c65554f7a2dbf30c18fd48778ef124af6fab771a377103da0585e2336ece",
-                "sha256:c4fdf4019605b6e5423637e01bc9fe4daef873709a7973e195ceba0a62bbc844"
+                "sha256:8d7eaa5a82a1cac232164990f04874c594c9453ec55eef02eab885aa02fc17a2",
+                "sha256:f5321fbe4bf3fefa0efd0bfe7fb14e90909eb62a48ccda331726b4319897dd5e"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4' and python_version < '4'",
-            "version": "==1.26.7"
-        },
-        "zipp": {
-            "hashes": [
-                "sha256:71c644c5369f4a6e07636f0aa966270449561fcea2e3d6747b8d23efaa9d7832",
-                "sha256:9fe5ea21568a0a70e50f273397638d39b03353731e6cbbb3fd8502a33fec40bc"
-            ],
-            "markers": "python_version >= '3.6'",
-            "version": "==3.6.0"
+            "version": "==1.25.11"
         },
         "zope.interface": {
             "hashes": [
-                "sha256:08f9636e99a9d5410181ba0729e0408d3d8748026ea938f3b970a0249daa8192",
-                "sha256:0b465ae0962d49c68aa9733ba92a001b2a0933c317780435f00be7ecb959c702",
-                "sha256:0cba8477e300d64a11a9789ed40ee8932b59f9ee05f85276dbb4b59acee5dd09",
-                "sha256:0cee5187b60ed26d56eb2960136288ce91bcf61e2a9405660d271d1f122a69a4",
-                "sha256:0ea1d73b7c9dcbc5080bb8aaffb776f1c68e807767069b9ccdd06f27a161914a",
-                "sha256:0f91b5b948686659a8e28b728ff5e74b1be6bf40cb04704453617e5f1e945ef3",
-                "sha256:15e7d1f7a6ee16572e21e3576d2012b2778cbacf75eb4b7400be37455f5ca8bf",
-                "sha256:17776ecd3a1fdd2b2cd5373e5ef8b307162f581c693575ec62e7c5399d80794c",
-                "sha256:194d0bcb1374ac3e1e023961610dc8f2c78a0f5f634d0c737691e215569e640d",
-                "sha256:1c0e316c9add0db48a5b703833881351444398b04111188069a26a61cfb4df78",
-                "sha256:205e40ccde0f37496904572035deea747390a8b7dc65146d30b96e2dd1359a83",
-                "sha256:273f158fabc5ea33cbc936da0ab3d4ba80ede5351babc4f577d768e057651531",
-                "sha256:2876246527c91e101184f63ccd1d716ec9c46519cc5f3d5375a3351c46467c46",
-                "sha256:2c98384b254b37ce50eddd55db8d381a5c53b4c10ee66e1e7fe749824f894021",
-                "sha256:2e5a26f16503be6c826abca904e45f1a44ff275fdb7e9d1b75c10671c26f8b94",
-                "sha256:334701327f37c47fa628fc8b8d28c7d7730ce7daaf4bda1efb741679c2b087fc",
-                "sha256:3748fac0d0f6a304e674955ab1365d515993b3a0a865e16a11ec9d86fb307f63",
-                "sha256:3c02411a3b62668200910090a0dff17c0b25aaa36145082a5a6adf08fa281e54",
-                "sha256:3dd4952748521205697bc2802e4afac5ed4b02909bb799ba1fe239f77fd4e117",
-                "sha256:3f24df7124c323fceb53ff6168da70dbfbae1442b4f3da439cd441681f54fe25",
-                "sha256:469e2407e0fe9880ac690a3666f03eb4c3c444411a5a5fddfdabc5d184a79f05",
-                "sha256:4de4bc9b6d35c5af65b454d3e9bc98c50eb3960d5a3762c9438df57427134b8e",
-                "sha256:5208ebd5152e040640518a77827bdfcc73773a15a33d6644015b763b9c9febc1",
-                "sha256:52de7fc6c21b419078008f697fd4103dbc763288b1406b4562554bd47514c004",
-                "sha256:5bb3489b4558e49ad2c5118137cfeaf59434f9737fa9c5deefc72d22c23822e2",
-                "sha256:5dba5f530fec3f0988d83b78cc591b58c0b6eb8431a85edd1569a0539a8a5a0e",
-                "sha256:5dd9ca406499444f4c8299f803d4a14edf7890ecc595c8b1c7115c2342cadc5f",
-                "sha256:5f931a1c21dfa7a9c573ec1f50a31135ccce84e32507c54e1ea404894c5eb96f",
-                "sha256:63b82bb63de7c821428d513607e84c6d97d58afd1fe2eb645030bdc185440120",
-                "sha256:66c0061c91b3b9cf542131148ef7ecbecb2690d48d1612ec386de9d36766058f",
-                "sha256:6f0c02cbb9691b7c91d5009108f975f8ffeab5dff8f26d62e21c493060eff2a1",
-                "sha256:71aace0c42d53abe6fc7f726c5d3b60d90f3c5c055a447950ad6ea9cec2e37d9",
-                "sha256:7d97a4306898b05404a0dcdc32d9709b7d8832c0c542b861d9a826301719794e",
-                "sha256:7df1e1c05304f26faa49fa752a8c690126cf98b40b91d54e6e9cc3b7d6ffe8b7",
-                "sha256:8270252effc60b9642b423189a2fe90eb6b59e87cbee54549db3f5562ff8d1b8",
-                "sha256:867a5ad16892bf20e6c4ea2aab1971f45645ff3102ad29bd84c86027fa99997b",
-                "sha256:877473e675fdcc113c138813a5dd440da0769a2d81f4d86614e5d62b69497155",
-                "sha256:8892f89999ffd992208754851e5a052f6b5db70a1e3f7d54b17c5211e37a98c7",
-                "sha256:9a9845c4c6bb56e508651f005c4aeb0404e518c6f000d5a1123ab077ab769f5c",
-                "sha256:a1e6e96217a0f72e2b8629e271e1b280c6fa3fe6e59fa8f6701bec14e3354325",
-                "sha256:a8156e6a7f5e2a0ff0c5b21d6bcb45145efece1909efcbbbf48c56f8da68221d",
-                "sha256:a9506a7e80bcf6eacfff7f804c0ad5350c8c95b9010e4356a4b36f5322f09abb",
-                "sha256:af310ec8335016b5e52cae60cda4a4f2a60a788cbb949a4fbea13d441aa5a09e",
-                "sha256:b0297b1e05fd128d26cc2460c810d42e205d16d76799526dfa8c8ccd50e74959",
-                "sha256:bf68f4b2b6683e52bec69273562df15af352e5ed25d1b6641e7efddc5951d1a7",
-                "sha256:d0c1bc2fa9a7285719e5678584f6b92572a5b639d0e471bb8d4b650a1a910920",
-                "sha256:d4d9d6c1a455d4babd320203b918ccc7fcbefe308615c521062bc2ba1aa4d26e",
-                "sha256:db1fa631737dab9fa0b37f3979d8d2631e348c3b4e8325d6873c2541d0ae5a48",
-                "sha256:dd93ea5c0c7f3e25335ab7d22a507b1dc43976e1345508f845efc573d3d779d8",
-                "sha256:f44e517131a98f7a76696a7b21b164bcb85291cee106a23beccce454e1f433a4",
-                "sha256:f7ee479e96f7ee350db1cf24afa5685a5899e2b34992fb99e1f7c1b0b758d263"
+                "sha256:008b0b65c05993bb08912f644d140530e775cf1c62a072bf9340c2249e613c32",
+                "sha256:0217a9615531c83aeedb12e126611b1b1a3175013bbafe57c702ce40000eb9a0",
+                "sha256:0fb497c6b088818e3395e302e426850f8236d8d9f4ef5b2836feae812a8f699c",
+                "sha256:17ebf6e0b1d07ed009738016abf0d0a0f80388e009d0ac6e0ead26fc162b3b9c",
+                "sha256:311196634bb9333aa06f00fc94f59d3a9fddd2305c2c425d86e406ddc6f2260d",
+                "sha256:3218ab1a7748327e08ef83cca63eea7cf20ea7e2ebcb2522072896e5e2fceedf",
+                "sha256:404d1e284eda9e233c90128697c71acffd55e183d70628aa0bbb0e7a3084ed8b",
+                "sha256:4087e253bd3bbbc3e615ecd0b6dd03c4e6a1e46d152d3be6d2ad08fbad742dcc",
+                "sha256:40f4065745e2c2fa0dff0e7ccd7c166a8ac9748974f960cd39f63d2c19f9231f",
+                "sha256:5334e2ef60d3d9439c08baedaf8b84dc9bb9522d0dacbc10572ef5609ef8db6d",
+                "sha256:604cdba8f1983d0ab78edc29aa71c8df0ada06fb147cea436dc37093a0100a4e",
+                "sha256:6373d7eb813a143cb7795d3e42bd8ed857c82a90571567e681e1b3841a390d16",
+                "sha256:655796a906fa3ca67273011c9805c1e1baa047781fca80feeb710328cdbed87f",
+                "sha256:65c3c06afee96c654e590e046c4a24559e65b0a87dbff256cd4bd6f77e1a33f9",
+                "sha256:696f3d5493eae7359887da55c2afa05acc3db5fc625c49529e84bd9992313296",
+                "sha256:6e972493cdfe4ad0411fd9abfab7d4d800a7317a93928217f1a5de2bb0f0d87a",
+                "sha256:7579960be23d1fddecb53898035a0d112ac858c3554018ce615cefc03024e46d",
+                "sha256:765d703096ca47aa5d93044bf701b00bbce4d903a95b41fff7c3796e747b1f1d",
+                "sha256:7e66f60b0067a10dd289b29dceabd3d0e6d68be1504fc9d0bc209cf07f56d189",
+                "sha256:8a2ffadefd0e7206adc86e492ccc60395f7edb5680adedf17a7ee4205c530df4",
+                "sha256:959697ef2757406bff71467a09d940ca364e724c534efbf3786e86eee8591452",
+                "sha256:9d783213fab61832dbb10d385a319cb0e45451088abd45f95b5bb88ed0acca1a",
+                "sha256:a16025df73d24795a0bde05504911d306307c24a64187752685ff6ea23897cb0",
+                "sha256:a2ad597c8c9e038a5912ac3cf166f82926feff2f6e0dabdab956768de0a258f5",
+                "sha256:bfee1f3ff62143819499e348f5b8a7f3aa0259f9aca5e0ddae7391d059dce671",
+                "sha256:d169ccd0756c15bbb2f1acc012f5aab279dffc334d733ca0d9362c5beaebe88e",
+                "sha256:d514c269d1f9f5cd05ddfed15298d6c418129f3f064765295659798349c43e6f",
+                "sha256:d692374b578360d36568dd05efb8a5a67ab6d1878c29c582e37ddba80e66c396",
+                "sha256:dbaeb9cf0ea0b3bc4b36fae54a016933d64c6d52a94810a63c00f440ecb37dd7",
+                "sha256:dc26c8d44472e035d59d6f1177eb712888447f5799743da9c398b0339ed90b1b",
+                "sha256:e1574980b48c8c74f83578d1e77e701f8439a5d93f36a5a0af31337467c08fcf",
+                "sha256:e74a578172525c20d7223eac5f8ad187f10940dac06e40113d62f14f3adb1e8f",
+                "sha256:e945de62917acbf853ab968d8916290548df18dd62c739d862f359ecd25842a6",
+                "sha256:f0980d44b8aded808bec5059018d64692f0127f10510eca71f2f0ace8fb11188",
+                "sha256:f98d4bd7bbb15ca701d19b93263cc5edfd480c3475d163f137385f49e5b3a3a7",
+                "sha256:fb68d212efd057596dee9e6582daded9f8ef776538afdf5feceb3059df2d2e7b"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
-            "version": "==5.4.0"
+            "version": "==5.5.2"
         }
     },
     "develop": {
         "attrs": {
             "hashes": [
-                "sha256:149e90d6d8ac20db7a955ad60cf0e6881a3f20d37096140088356da6c716b0b1",
-                "sha256:ef6aaac3ca6cd92904cdd0d83f629a15f18053ec84e6432106f7a4d04ae4f5fb"
+                "sha256:29adc2665447e5191d0e7c568fde78b21f9672d344281d0c6e1ab085429b22b6",
+                "sha256:86efa402f67bf2df34f51a335487cf46b1ec130d02b8d39fd248abfd30da551c"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
-            "version": "==21.2.0"
-        },
-        "backports.entry-points-selectable": {
-            "hashes": [
-                "sha256:7fceed9532a7aa2bd888654a7314f864a3c16a4e710b34a58cfc0f08114c663b",
-                "sha256:914b21a479fde881635f7af5adc7f6e38d6b274be32269070c53b698c60d5386"
-            ],
-            "markers": "python_version >= '2.7'",
-            "version": "==1.1.1"
+            "markers": "python_version >= '3.5'",
+            "version": "==22.1.0"
         },
         "coverage": {
             "extras": [
                 "toml"
             ],
             "hashes": [
-                "sha256:01774a2c2c729619760320270e42cd9e797427ecfddd32c2a7b639cdc481f3c0",
-                "sha256:03b20e52b7d31be571c9c06b74746746d4eb82fc260e594dc662ed48145e9efd",
-                "sha256:0a7726f74ff63f41e95ed3a89fef002916c828bb5fcae83b505b49d81a066884",
-                "sha256:1219d760ccfafc03c0822ae2e06e3b1248a8e6d1a70928966bafc6838d3c9e48",
-                "sha256:13362889b2d46e8d9f97c421539c97c963e34031ab0cb89e8ca83a10cc71ac76",
-                "sha256:174cf9b4bef0db2e8244f82059a5a72bd47e1d40e71c68ab055425172b16b7d0",
-                "sha256:17e6c11038d4ed6e8af1407d9e89a2904d573be29d51515f14262d7f10ef0a64",
-                "sha256:215f8afcc02a24c2d9a10d3790b21054b58d71f4b3c6f055d4bb1b15cecce685",
-                "sha256:22e60a3ca5acba37d1d4a2ee66e051f5b0e1b9ac950b5b0cf4aa5366eda41d47",
-                "sha256:2641f803ee9f95b1f387f3e8f3bf28d83d9b69a39e9911e5bfee832bea75240d",
-                "sha256:276651978c94a8c5672ea60a2656e95a3cce2a3f31e9fb2d5ebd4c215d095840",
-                "sha256:3f7c17209eef285c86f819ff04a6d4cbee9b33ef05cbcaae4c0b4e8e06b3ec8f",
-                "sha256:3feac4084291642165c3a0d9eaebedf19ffa505016c4d3db15bfe235718d4971",
-                "sha256:49dbff64961bc9bdd2289a2bda6a3a5a331964ba5497f694e2cbd540d656dc1c",
-                "sha256:4e547122ca2d244f7c090fe3f4b5a5861255ff66b7ab6d98f44a0222aaf8671a",
-                "sha256:5829192582c0ec8ca4a2532407bc14c2f338d9878a10442f5d03804a95fac9de",
-                "sha256:5d6b09c972ce9200264c35a1d53d43ca55ef61836d9ec60f0d44273a31aa9f17",
-                "sha256:600617008aa82032ddeace2535626d1bc212dfff32b43989539deda63b3f36e4",
-                "sha256:619346d57c7126ae49ac95b11b0dc8e36c1dd49d148477461bb66c8cf13bb521",
-                "sha256:63c424e6f5b4ab1cf1e23a43b12f542b0ec2e54f99ec9f11b75382152981df57",
-                "sha256:6dbc1536e105adda7a6312c778f15aaabe583b0e9a0b0a324990334fd458c94b",
-                "sha256:6e1394d24d5938e561fbeaa0cd3d356207579c28bd1792f25a068743f2d5b282",
-                "sha256:86f2e78b1eff847609b1ca8050c9e1fa3bd44ce755b2ec30e70f2d3ba3844644",
-                "sha256:8bdfe9ff3a4ea37d17f172ac0dff1e1c383aec17a636b9b35906babc9f0f5475",
-                "sha256:8e2c35a4c1f269704e90888e56f794e2d9c0262fb0c1b1c8c4ee44d9b9e77b5d",
-                "sha256:92b8c845527eae547a2a6617d336adc56394050c3ed8a6918683646328fbb6da",
-                "sha256:9365ed5cce5d0cf2c10afc6add145c5037d3148585b8ae0e77cc1efdd6aa2953",
-                "sha256:9a29311bd6429be317c1f3fe4bc06c4c5ee45e2fa61b2a19d4d1d6111cb94af2",
-                "sha256:9a2b5b52be0a8626fcbffd7e689781bf8c2ac01613e77feda93d96184949a98e",
-                "sha256:a4bdeb0a52d1d04123b41d90a4390b096f3ef38eee35e11f0b22c2d031222c6c",
-                "sha256:a9c8c4283e17690ff1a7427123ffb428ad6a52ed720d550e299e8291e33184dc",
-                "sha256:b637c57fdb8be84e91fac60d9325a66a5981f8086c954ea2772efe28425eaf64",
-                "sha256:bf154ba7ee2fd613eb541c2bc03d3d9ac667080a737449d1a3fb342740eb1a74",
-                "sha256:c254b03032d5a06de049ce8bca8338a5185f07fb76600afff3c161e053d88617",
-                "sha256:c332d8f8d448ded473b97fefe4a0983265af21917d8b0cdcb8bb06b2afe632c3",
-                "sha256:c7912d1526299cb04c88288e148c6c87c0df600eca76efd99d84396cfe00ef1d",
-                "sha256:cfd9386c1d6f13b37e05a91a8583e802f8059bebfccde61a418c5808dea6bbfa",
-                "sha256:d5d2033d5db1d58ae2d62f095e1aefb6988af65b4b12cb8987af409587cc0739",
-                "sha256:dca38a21e4423f3edb821292e97cec7ad38086f84313462098568baedf4331f8",
-                "sha256:e2cad8093172b7d1595b4ad66f24270808658e11acf43a8f95b41276162eb5b8",
-                "sha256:e3db840a4dee542e37e09f30859f1612da90e1c5239a6a2498c473183a50e781",
-                "sha256:edcada2e24ed68f019175c2b2af2a8b481d3d084798b8c20d15d34f5c733fa58",
-                "sha256:f467bbb837691ab5a8ca359199d3429a11a01e6dfb3d9dcc676dc035ca93c0a9",
-                "sha256:f506af4f27def639ba45789fa6fde45f9a217da0be05f8910458e4557eed020c",
-                "sha256:f614fc9956d76d8a88a88bb41ddc12709caa755666f580af3a688899721efecd",
-                "sha256:f9afb5b746781fc2abce26193d1c817b7eb0e11459510fba65d2bd77fe161d9e",
-                "sha256:fb8b8ee99b3fffe4fd86f4c81b35a6bf7e4462cba019997af2fe679365db0c49"
+                "sha256:027018943386e7b942fa832372ebc120155fd970837489896099f5cfa2890f79",
+                "sha256:11b990d520ea75e7ee8dcab5bc908072aaada194a794db9f6d7d5cfd19661e5a",
+                "sha256:12adf310e4aafddc58afdb04d686795f33f4d7a6fa67a7a9d4ce7d6ae24d949f",
+                "sha256:1431986dac3923c5945271f169f59c45b8802a114c8f548d611f2015133df77a",
+                "sha256:1ef221513e6f68b69ee9e159506d583d31aa3567e0ae84eaad9d6ec1107dddaa",
+                "sha256:20c8ac5386253717e5ccc827caad43ed66fea0efe255727b1053a8154d952398",
+                "sha256:2198ea6fc548de52adc826f62cb18554caedfb1d26548c1b7c88d8f7faa8f6ba",
+                "sha256:255758a1e3b61db372ec2736c8e2a1fdfaf563977eedbdf131de003ca5779b7d",
+                "sha256:265de0fa6778d07de30bcf4d9dc471c3dc4314a23a3c6603d356a3c9abc2dfcf",
+                "sha256:33a7da4376d5977fbf0a8ed91c4dffaaa8dbf0ddbf4c8eea500a2486d8bc4d7b",
+                "sha256:42eafe6778551cf006a7c43153af1211c3aaab658d4d66fa5fcc021613d02518",
+                "sha256:4433b90fae13f86fafff0b326453dd42fc9a639a0d9e4eec4d366436d1a41b6d",
+                "sha256:4a5375e28c5191ac38cca59b38edd33ef4cc914732c916f2929029b4bfb50795",
+                "sha256:4a8dbc1f0fbb2ae3de73eb0bdbb914180c7abfbf258e90b311dcd4f585d44bd2",
+                "sha256:59f53f1dc5b656cafb1badd0feb428c1e7bc19b867479ff72f7a9dd9b479f10e",
+                "sha256:5dbec3b9095749390c09ab7c89d314727f18800060d8d24e87f01fb9cfb40b32",
+                "sha256:633713d70ad6bfc49b34ead4060531658dc6dfc9b3eb7d8a716d5873377ab745",
+                "sha256:6b07130585d54fe8dff3d97b93b0e20290de974dc8177c320aeaf23459219c0b",
+                "sha256:6c4459b3de97b75e3bd6b7d4b7f0db13f17f504f3d13e2a7c623786289dd670e",
+                "sha256:6d4817234349a80dbf03640cec6109cd90cba068330703fa65ddf56b60223a6d",
+                "sha256:723e8130d4ecc8f56e9a611e73b31219595baa3bb252d539206f7bbbab6ffc1f",
+                "sha256:784f53ebc9f3fd0e2a3f6a78b2be1bd1f5575d7863e10c6e12504f240fd06660",
+                "sha256:7b6be138d61e458e18d8e6ddcddd36dd96215edfe5f1168de0b1b32635839b62",
+                "sha256:7ccf362abd726b0410bf8911c31fbf97f09f8f1061f8c1cf03dfc4b6372848f6",
+                "sha256:83516205e254a0cb77d2d7bb3632ee019d93d9f4005de31dca0a8c3667d5bc04",
+                "sha256:851cf4ff24062c6aec510a454b2584f6e998cada52d4cb58c5e233d07172e50c",
+                "sha256:8f830ed581b45b82451a40faabb89c84e1a998124ee4212d440e9c6cf70083e5",
+                "sha256:94e2565443291bd778421856bc975d351738963071e9b8839ca1fc08b42d4bef",
+                "sha256:95203854f974e07af96358c0b261f1048d8e1083f2de9b1c565e1be4a3a48cfc",
+                "sha256:97117225cdd992a9c2a5515db1f66b59db634f59d0679ca1fa3fe8da32749cae",
+                "sha256:98e8a10b7a314f454d9eff4216a9a94d143a7ee65018dd12442e898ee2310578",
+                "sha256:a1170fa54185845505fbfa672f1c1ab175446c887cce8212c44149581cf2d466",
+                "sha256:a6b7d95969b8845250586f269e81e5dfdd8ff828ddeb8567a4a2eaa7313460c4",
+                "sha256:a8fb6cf131ac4070c9c5a3e21de0f7dc5a0fbe8bc77c9456ced896c12fcdad91",
+                "sha256:af4fffaffc4067232253715065e30c5a7ec6faac36f8fc8d6f64263b15f74db0",
+                "sha256:b4a5be1748d538a710f87542f22c2cad22f80545a847ad91ce45e77417293eb4",
+                "sha256:b5604380f3415ba69de87a289a2b56687faa4fe04dbee0754bfcae433489316b",
+                "sha256:b9023e237f4c02ff739581ef35969c3739445fb059b060ca51771e69101efffe",
+                "sha256:bc8ef5e043a2af066fa8cbfc6e708d58017024dc4345a1f9757b329a249f041b",
+                "sha256:c4ed2820d919351f4167e52425e096af41bfabacb1857186c1ea32ff9983ed75",
+                "sha256:cca4435eebea7962a52bdb216dec27215d0df64cf27fc1dd538415f5d2b9da6b",
+                "sha256:d900bb429fdfd7f511f868cedd03a6bbb142f3f9118c09b99ef8dc9bf9643c3c",
+                "sha256:d9ecf0829c6a62b9b573c7bb6d4dcd6ba8b6f80be9ba4fc7ed50bf4ac9aecd72",
+                "sha256:dbdb91cd8c048c2b09eb17713b0c12a54fbd587d79adcebad543bc0cd9a3410b",
+                "sha256:de3001a203182842a4630e7b8d1a2c7c07ec1b45d3084a83d5d227a3806f530f",
+                "sha256:e07f4a4a9b41583d6eabec04f8b68076ab3cd44c20bd29332c6572dda36f372e",
+                "sha256:ef8674b0ee8cc11e2d574e3e2998aea5df5ab242e012286824ea3c6970580e53",
+                "sha256:f4f05d88d9a80ad3cac6244d36dd89a3c00abc16371769f1340101d3cb899fc3",
+                "sha256:f642e90754ee3e06b0e7e51bce3379590e76b7f76b708e1a71ff043f87025c84",
+                "sha256:fc2af30ed0d5ae0b1abdb4ebdce598eafd5b35397d4d75deb341a614d333d987"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==6.2"
+            "markers": "python_version >= '3.7'",
+            "version": "==6.5.0"
         },
         "distlib": {
             "hashes": [
-                "sha256:6564fe0a8f51e734df6333d08b8b94d4ea8ee6b99b5ed50613f731fd4089f34b",
-                "sha256:e4b58818180336dc9c529bfb9a0b58728ffc09ad92027a3f30b7cd91e3458579"
-            ],
-            "version": "==0.3.4"
-        },
-        "filelock": {
-            "hashes": [
-                "sha256:2e139a228bcf56dd8b2274a65174d005c4a6b68540ee0bdbb92c76f43f29f7e8",
-                "sha256:93d512b32a23baf4cac44ffd72ccf70732aeff7b8050fcaf6d3ec406d954baf4"
+                "sha256:14bad2d9b04d3a36127ac97f30b12a19268f211063d8f8ee4f47108896e11b46",
+                "sha256:f35c4b692542ca110de7ef0bea44d73981caeb34ca0b9b6b2e6d7790dda8f80e"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==3.4.0"
+            "version": "==0.3.6"
         },
-        "flake8": {
+        "exceptiongroup": {
             "hashes": [
-                "sha256:479b1304f72536a55948cb40a32dce8bb0ffe3501e26eaf292c7e60eb5e0428d",
-                "sha256:806e034dda44114815e23c16ef92f95c91e4c71100ff52813adf7132a6ad870d"
+                "sha256:542adf9dea4055530d6e1279602fa5cb11dab2395fa650b8674eaec35fc4a828",
+                "sha256:bd14967b79cd9bdb54d97323216f8fdf533e278df937aa2a90089e7d6e06e5ec"
             ],
-            "index": "pypi",
-            "version": "==4.0.1"
+            "markers": "python_version < '3.11'",
+            "version": "==1.0.4"
         },
-        "importlib-metadata": {
+        "filelock": {
             "hashes": [
-                "sha256:65a9576a5b2d58ca44d133c42a241905cc45e34d2c06fd5ba2bafa221e5d7b5e",
-                "sha256:766abffff765960fcc18003801f7044eb6755ffae4521c8e8ce8e83b9c9b0668"
+                "sha256:55447caa666f2198c5b6b13a26d2084d26fa5b115c00d065664b2124680c4edc",
+                "sha256:617eb4e5eedc82fc5f47b6d61e4d11cb837c56cb4544e39081099fa17ad109d4"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==4.8.3"
+            "markers": "python_version >= '3.7'",
+            "version": "==3.8.0"
         },
-        "importlib-resources": {
+        "flake8": {
             "hashes": [
-                "sha256:33a95faed5fc19b4bc16b29a6eeae248a3fe69dd55d4d229d2b480e23eeaad45",
-                "sha256:d756e2f85dd4de2ba89be0b21dba2a3bbec2e871a42a3a16719258a11f87506b"
+                "sha256:6fbe320aad8d6b95cec8b8e47bc933004678dc63095be98528b7bdd2a9f510db",
+                "sha256:7a1cf6b73744f5806ab95e526f6f0d8c01c66d7bbe349562d22dfca20610b248"
             ],
-            "markers": "python_version < '3.7'",
-            "version": "==5.4.0"
+            "index": "pypi",
+            "version": "==5.0.4"
         },
         "iniconfig": {
             "hashes": [
                 "sha256:011e24c64b7f47f6ebd835bb12a743f2fbe9a26d4cecaa7f53bc4f35ee9da8b3",
                 "sha256:bc3af051d7d14b2ee5ef9969666def0cd1a000e121eaea580d4a313df4b37f32"
             ],
             "version": "==1.1.1"
         },
         "mccabe": {
             "hashes": [
-                "sha256:ab8a6258860da4b6677da4bd2fe5dc2c659cff31b3ee4f7f5d64e79735b80d42",
-                "sha256:dd8d182285a0fe56bace7f45b5e7d1a6ebcbf524e8f3bd87eb0f125271b8831f"
+                "sha256:348e0240c33b60bbdf4e523192ef919f28cb2c3d7d5c7794f74009290f236325",
+                "sha256:6c2d30ab6be0e4a46919781807b4f0d834ebdd6c6e3dca0bda5a15f863427b6e"
             ],
-            "version": "==0.6.1"
+            "markers": "python_version >= '3.6'",
+            "version": "==0.7.0"
         },
         "packaging": {
             "hashes": [
                 "sha256:dd47c42927d89ab911e606518907cc2d3a1f38bbd026385970643f9c5b8ecfeb",
                 "sha256:ef103e05f519cdc783ae24ea4e2e0f508a9c99b2d4969652eed6a2e1ea5bd522"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==21.3"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:367a5e80b3d04d2428ffa76d33f124cf11e8fff2acdaa9b43d545f5c7d661ef2",
-                "sha256:8868bbe3c3c80d42f20156f22e7131d2fb321f5bc86a2a345375c6481a67021d"
+                "sha256:1006647646d80f16130f052404c6b901e80ee4ed6bef6792e1f238a8969106f7",
+                "sha256:af0276409f9a02373d540bf8480021a048711d572745aef4b7842dad245eba10"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==2.4.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.5.4"
         },
         "pluggy": {
             "hashes": [
                 "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159",
                 "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"
             ],
             "markers": "python_version >= '3.6'",
@@ -363,118 +321,95 @@
                 "sha256:607c53218732647dff4acdfcd50cb62615cedf612e72d1724fb1a0cc6405b378"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
             "version": "==1.11.0"
         },
         "pycodestyle": {
             "hashes": [
-                "sha256:720f8b39dde8b293825e7ff02c475f3077124006db4f440dcbc9a20b76548a20",
-                "sha256:eddd5847ef438ea1c7870ca7eb78a9d47ce0cdb4851a5523949f2601d0cbbe7f"
+                "sha256:2c9607871d58c76354b697b42f5d57e1ada7d261c261efac224b664affdc5785",
+                "sha256:d1735fc58b418fd7c5f658d28d943854f8a849b01a5d0a1e6f3f3fdd0166804b"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
-            "version": "==2.8.0"
+            "markers": "python_version >= '3.6'",
+            "version": "==2.9.1"
         },
         "pyflakes": {
             "hashes": [
-                "sha256:05a85c2872edf37a4ed30b0cce2f6093e1d0581f8c19d7393122da7e25b2b24c",
-                "sha256:3bb3a3f256f4b7968c9c788781e4ff07dce46bdf12339dcda61053375426ee2e"
+                "sha256:4579f67d887f804e67edb544428f264b7b24f435b263c4614f384135cea553d2",
+                "sha256:491feb020dca48ccc562a8c0cbe8df07ee13078df59813b83959cbdada312ea3"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==2.4.0"
+            "markers": "python_version >= '3.6'",
+            "version": "==2.5.0"
         },
         "pyparsing": {
             "hashes": [
-                "sha256:04ff808a5b90911829c55c4e26f75fa5ca8a2f5f36aa3a51f68e27033341d3e4",
-                "sha256:d9bdec0013ef1eb5a84ab39a3b3868911598afa494f5faa038647101504e2b81"
+                "sha256:2b020ecf7d21b687f219b71ecad3631f644a47f01403fa1d1036b0c6416d70fb",
+                "sha256:5026bae9a10eeaefb61dab2f09052b9f4307d44aee4eda64b309723d8d206bbc"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==3.0.6"
+            "markers": "python_full_version >= '3.6.8'",
+            "version": "==3.0.9"
         },
         "pytest": {
             "hashes": [
-                "sha256:131b36680866a76e6781d13f101efb86cf674ebb9762eb70d3082b6f29889e89",
-                "sha256:7310f8d27bc79ced999e760ca304d69f6ba6c6649c0b60fb0e04a4a77cacc134"
+                "sha256:892f933d339f068883b6fd5a459f03d85bfcb355e4981e146d2c7616c21fef71",
+                "sha256:c4014eb40e10f11f355ad4e3c2fb2c6c6d1919c73f3b5a433de4708202cade59"
             ],
             "index": "pypi",
-            "version": "==6.2.5"
+            "version": "==7.2.0"
         },
         "pytest-cov": {
             "hashes": [
-                "sha256:578d5d15ac4a25e5f961c938b85a05b09fdaae9deef3bb6de9a6e766622ca7a6",
-                "sha256:e7f0f5b1617d2210a2cabc266dfe2f4c75a8d32fb89eafb7ad9d06f6d076d470"
+                "sha256:2feb1b751d66a8bd934e5edfa2e961d11309dc37b73b0eabe73b5945fee20f6b",
+                "sha256:996b79efde6433cdbd0088872dbc5fb3ed7fe1578b68cdbba634f14bb8dd0470"
             ],
             "index": "pypi",
-            "version": "==3.0.0"
+            "version": "==4.0.0"
         },
         "python-dotenv": {
             "hashes": [
-                "sha256:32b2bdc1873fd3a3c346da1c6db83d0053c3c62f28f1f38516070c4c8971b1d3",
-                "sha256:a5de49a31e953b45ff2d2fd434bbc2670e8db5273606c1e737cc6b93eff3655f"
+                "sha256:1684eb44636dd462b66c3ee016599815514527ad99965de77f43e0944634a7e5",
+                "sha256:b77d08274639e3d34145dfa6c7008e66df0f04b7be7a75fd0d5292c191d79045"
             ],
             "index": "pypi",
-            "version": "==0.19.2"
+            "version": "==0.21.0"
         },
         "setuptools": {
             "hashes": [
-                "sha256:22c7348c6d2976a52632c67f7ab0cdf40147db7789f9aed18734643fe9cf3373",
-                "sha256:4ce92f1e1f8f01233ee9952c04f6b81d1e02939d6e1b488428154974a4d0783e"
+                "sha256:6211d2f5eddad8757bd0484923ca7c0a6302ebc4ab32ea5e94357176e0ca0840",
+                "sha256:d1eebf881c6114e51df1664bc2c9133d022f78d12d5f4f665b9191f084e2862d"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==59.6.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==65.6.0"
         },
         "six": {
             "hashes": [
                 "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926",
                 "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2'",
             "version": "==1.16.0"
         },
-        "toml": {
-            "hashes": [
-                "sha256:806143ae5bfb6a3c6e736a764057db0e6a0e05e338b5630894a5f779cabb4f9b",
-                "sha256:b3bda1d108d5dd99f4a20d24d9c348e91c4db7ab1b749200bded2f839ccbe68f"
-            ],
-            "markers": "python_version >= '2.6' and python_version not in '3.0, 3.1, 3.2'",
-            "version": "==0.10.2"
-        },
         "tomli": {
             "hashes": [
-                "sha256:05b6166bff487dc068d322585c7ea4ef78deed501cc124060e0f238e89a9231f",
-                "sha256:e3069e4be3ead9668e21cb9b074cd948f7b3113fd9c8bba083f48247aab8b11c"
+                "sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc",
+                "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"
             ],
-            "version": "==1.2.3"
+            "markers": "python_version < '3.11'",
+            "version": "==2.0.1"
         },
         "tox": {
             "hashes": [
-                "sha256:5e274227a53dc9ef856767c21867377ba395992549f02ce55eb549f9fb9a8d10",
-                "sha256:c30b57fa2477f1fb7c36aa1d83292d5c2336cd0018119e1b1c17340e2c2708ca"
+                "sha256:b2a920e35a668cc06942ffd1cf3a4fb221a4d909ca72191fb6d84b0b18a7be04",
+                "sha256:f52ca66eae115fcfef0e77ef81fd107133d295c97c52df337adedb8dfac6ab84"
             ],
             "index": "pypi",
-            "version": "==3.24.4"
-        },
-        "typing-extensions": {
-            "hashes": [
-                "sha256:4ca091dea149f945ec56afb48dae714f21e8692ef22a395223bcd328961b6a0e",
-                "sha256:7f001e5ac290a0c0401508864c7ec868be4e701886d5b573a9528ed3973d9d3b"
-            ],
-            "markers": "python_version < '3.8'",
-            "version": "==4.0.1"
+            "version": "==3.27.1"
         },
         "virtualenv": {
             "hashes": [
-                "sha256:4b02e52a624336eece99c96e3ab7111f469c24ba226a53ec474e8e787b365814",
-                "sha256:576d05b46eace16a9c348085f7d0dc8ef28713a2cabaa1cf0aea41e8f12c9218"
-            ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
-            "version": "==20.10.0"
-        },
-        "zipp": {
-            "hashes": [
-                "sha256:71c644c5369f4a6e07636f0aa966270449561fcea2e3d6747b8d23efaa9d7832",
-                "sha256:9fe5ea21568a0a70e50f273397638d39b03353731e6cbbb3fd8502a33fec40bc"
+                "sha256:8691e3ff9387f743e00f6bb20f70121f5e4f596cae754531f2b3b3a1b1ac696e",
+                "sha256:efd66b00386fdb7dbe4822d172303f40cd05e50e01740b19ea42425cbe653e29"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==3.6.0"
+            "version": "==20.16.7"
         }
     }
 }
```

### Comparing `molgenis-py-bbmri-eric-1.8.0/README.md` & `molgenis-py-bbmri-eric-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `molgenis-py-bbmri-eric-1.8.0/scripts/biobank_pid_assignment.py` & `molgenis-py-bbmri-eric-1.9.0/scripts/biobank_pid_assignment.py`

 * *Files identical despite different names*

### Comparing `molgenis-py-bbmri-eric-1.8.0/scripts/example.py` & `molgenis-py-bbmri-eric-1.9.0/scripts/example.py`

 * *Files identical despite different names*

### Comparing `molgenis-py-bbmri-eric-1.8.0/scripts/hook.py` & `molgenis-py-bbmri-eric-1.9.0/scripts/hook.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,23 +3,25 @@
 is deployed by copying the production database and this hook transforms the database in
 such a way that is safe to use as an acceptance test environment:
 
 1. Changes the password
 2. Removes production PIDs and replaces them with test PIDs
 3. Disables some scheduled jobs
 4. Removes people from email lists in scheduled jobs (except the support email)
+5. Updates the Google Analytics settings
 
 Requires a .env file next to it to configure. Example:
 
 HOOK_OLD_PASSWORD=oldpassword
 HOOK_NEW_PASSWORD=newpassword
 HOOK_SERVER_URL=https://myserver/
 HOOK_PYHANDLE_CREDS_JSON=pyhandle_creds.json
 HOOK_USE_LIVE_PID_SERVICE=True
 HOOK_MOLGENIS_SUPPORT_EMAIL=molgenis-support@umcg.nl
+HOOK_GA_ID=ga_id
 
 Setting HOOK_USE_LIVE_PID_SERVICE to False will use the DummyPidService instead, which
 will not create actual handles but will fill the column with fake PIDs.
 """
 import json
 import logging
 from unittest.mock import Mock
@@ -34,27 +36,29 @@
 config = dotenv_values(".env")
 old_password = config["HOOK_OLD_PASSWORD"]
 new_password = config["HOOK_NEW_PASSWORD"]
 url = config["HOOK_SERVER_URL"]
 pyhandle_creds = config["HOOK_PYHANDLE_CREDS_JSON"]
 use_live_pid_service = config["HOOK_USE_LIVE_PID_SERVICE"].lower() == "true"
 support_email = config["HOOK_MOLGENIS_SUPPORT_EMAIL"]
+ga_id = config["HOOK_GA_ID"]
 
 
 def run():
     logging.getLogger("pyhandle").setLevel(logging.WARNING)
     logger = logging.getLogger(__name__)
 
     session = EricSession(url)
     session.login("admin", old_password)
 
     change_password(session, logger)
     overwrite_pids(session, logger)
     disable_jobs(session, logger)
     remove_job_emails(session, logger)
+    update_ga_settings(session, logger)
 
     logger.info("Finished!")
 
 
 def change_password(session: EricSession, logger):
     logger.info("Updating admin password")
     admin_user_id = session.get("sys_sec_User", q="username==admin")[0]["id"]
@@ -131,14 +135,49 @@
         if "successEmail" in job and support_email in job["successEmail"]:
             success_email = support_email
 
         session.update_one(job_entity, job["id"], "failureEmail", failure_email)
         session.update_one(job_entity, job["id"], "successEmail", success_email)
 
 
+def update_ga_settings(session: EricSession, logger):
+    logger.info("Update Google Analytics settings")
+
+    settings_entity = "sys_set_app"
+    settings = session.get(settings_entity)
+
+    for setting in settings:
+        ga_acc_privacy_friendly = False
+        tracking_code_footer = f"""</script>
+<!-- Global site tag (gtag.js) - Google Analytics -->
+<script src="https://www.googletagmanager.com/gtag/js?id={ga_id}"></script>
+<script>
+  window.dataLayer = window.dataLayer || [];
+  function gtag(){{dataLayer.push(arguments);}}
+  gtag('js', new Date());
+
+  gtag('config', '{ga_id}');
+</script>"""
+
+        if "ga_tracking_id" in setting:
+            session.update_one(settings_entity, setting["id"], "ga_tracking_id", ga_id)
+            session.update_one(
+                settings_entity,
+                setting["id"],
+                "tracking_code_footer",
+                tracking_code_footer,
+            )
+            session.update_one(
+                settings_entity,
+                setting["id"],
+                "ga_acc_privacy_friendly",
+                ga_acc_privacy_friendly,
+            )
+
+
 if __name__ == "__main__":
     logging.basicConfig(
         format="%(asctime)s : %(message)s",
         datefmt="%Y-%m-%d %H:%M:%S",
         level=logging.INFO,
     )
     run()
```

### Comparing `molgenis-py-bbmri-eric-1.8.0/scripts/sync_DE_qualities.py` & `molgenis-py-bbmri-eric-1.9.0/scripts/sync_DE_qualities.py`

 * *Files identical despite different names*

### Comparing `molgenis-py-bbmri-eric-1.8.0/setup.cfg` & `molgenis-py-bbmri-eric-1.9.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -10,28 +10,29 @@
 project_urls = 
 	Source = https://github.com/molgenis/molgenis-py-bbmri-eric
 platforms = any
 classifiers = 
 	License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 	Programming Language :: Python
 	Programming Language :: Python :: 3 :: Only
+	Programming Language :: Python :: 3.10
 
 [options]
 zip_safe = False
 packages = find_namespace:
 include_package_data = True
 package_dir = 
 	=src
 python_requires = >=3.6
 install_requires = 
-	importlib-metadata; python_version<"3.8"
 	dataclasses
-	molgenis-py-client>=2.3.1
-	pyhandle>=1.0.4
+	molgenis-py-client==2.3.1
+	pyhandle>=1.1.0
 	requests>=2.21.0
+	unidecode
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
 [options.extras_require]
```

### Comparing `molgenis-py-bbmri-eric-1.8.0/setup.py` & `molgenis-py-bbmri-eric-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `molgenis-py-bbmri-eric-1.8.0/src/molgenis/bbmri_eric/bbmri_client.py` & `molgenis-py-bbmri-eric-1.9.0/src/molgenis/bbmri_eric/bbmri_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 from molgenis.client import MolgenisRequestError, Session
 
 
 @dataclass
 class AttributesRequest:
     persons: List[str]
     networks: List[str]
+    also_known_in: List[str]
     biobanks: List[str]
     collections: List[str]
 
 
 class MolgenisImportError(MolgenisRequestError):
     pass
 
@@ -68,14 +69,32 @@
     IMPORT_API_LOC = "plugin/importwizard/importFile/"
 
     def __init__(self, url: str, token: Optional[str] = None):
         super(ExtendedSession, self).__init__(url, token)
         self.url = self._root_url
         self.import_api = self._root_url + self.IMPORT_API_LOC
 
+    def _raise_exception(self, ex):
+        """Raises an exception with error message from molgenis, extends the original
+        one as it does not account for KeyError"""
+        message = ex.args[0]
+        if ex.response.content:
+            try:
+                error = json.loads(ex.response.content.decode("utf-8"))["errors"][0][
+                    "message"
+                ]
+            except ValueError:  # Cannot parse JSON
+                error = ex.response.content
+            except KeyError:  # Cannot parse JSON
+                error = json.loads(ex.response.content.decode("utf-8"))["detail"]
+            error_msg = "{}: {}".format(message, error)
+            raise MolgenisRequestError(error_msg, ex.response)
+        else:
+            raise MolgenisRequestError("{}".format(message))
+
     def get_uploadable_data(self, entity_type_id: str, *args, **kwargs) -> List[dict]:
         """
         Returns all the rows of an entity type, transformed to the uploadable format.
         """
         rows = self.get(entity_type_id, *args, **kwargs)
         return utils.to_upload_format(rows)
 
@@ -287,15 +306,15 @@
                         url=node["dns"],
                     )
                 )
         return result
 
     def get_staging_node_data(self, node: Node) -> NodeData:
         """
-        Gets the four tables that belong to a single node's staging area.
+        Gets the five tables that belong to a single node's staging area.
 
         :param Node node: the node to get the staging data for
         :return: a NodeData object
         """
         tables = dict()
         for table_type in TableType.get_import_order():
             id_ = node.get_staging_id(table_type)
@@ -307,15 +326,15 @@
                 rows=self.get_uploadable_data(id_, batch_size=10000),
             )
 
         return NodeData.from_dict(node=node, source=Source.STAGING, tables=tables)
 
     def get_published_node_data(self, node: Node) -> NodeData:
         """
-        Gets the four tables that belong to a single node from the published tables.
+        Gets the five tables that belong to a single node from the published tables.
         Filters the rows based on the national_node field.
 
         :param Node node: the node to get the published data for
         :return: a NodeData object
         """
 
         tables = dict()
@@ -333,15 +352,15 @@
 
         return NodeData.from_dict(node=node, source=Source.PUBLISHED, tables=tables)
 
     def get_published_data(
         self, nodes: List[Node], attributes: AttributesRequest
     ) -> MixedData:
         """
-        Gets the four tables that belong to one or more nodes from the published tables.
+        Gets the five tables that belong to one or more nodes from the published tables.
         Filters the rows based on the national_node field.
 
         :param List[Node] nodes: the node(s) to get the published data for
         :param AttributesRequest attributes: the attributes to get for each table
         :return: an EricData object
         """
 
@@ -367,15 +386,15 @@
                 ),
             )
 
         return MixedData.from_mixed_dict(source=Source.PUBLISHED, tables=tables)
 
     def import_as_csv(self, data: EricData):
         """
-        Converts the four tables of an EricData object to CSV, bundles them in
+        Converts the five tables of an EricData object to CSV, bundles them in
         a ZIP archive and imports them through the import API.
         :param data: an EricData object
         """
         with tempfile.TemporaryDirectory() as tmpdir:
             archive = self._create_emx_archive(data, tmpdir)
             self.import_emx_file(
                 archive,
@@ -394,15 +413,18 @@
                 archive.write(file_path, file_name)
         return Path(archive_name)
 
     @staticmethod
     def _create_csv(table: Table, file_name: str):
         with open(file_name, "w", encoding="utf-8") as fp:
             writer = csv.DictWriter(
-                fp, fieldnames=table.meta.attributes, quoting=csv.QUOTE_ALL
+                fp,
+                fieldnames=table.meta.attributes,
+                quoting=csv.QUOTE_ALL,
+                extrasaction="ignore",
             )
             writer.writeheader()
             for row in table.rows:
                 for key, value in row.items():
                     if isinstance(value, list):
                         row[key] = ",".join(value)
                 writer.writerow(row)
@@ -415,26 +437,28 @@
 
     def __init__(self, node: ExternalServerNode, *args, **kwargs):
         super(ExternalServerSession, self).__init__(url=node.url, *args, **kwargs)
         self.node = node
 
     def get_node_data(self) -> NodeData:
         """
-        Gets the four tables of this node's external server.
+        Gets the five tables of this node's external server.
 
         :return: a NodeData object
         """
 
         tables = dict()
         for table_type in TableType.get_import_order():
             id_ = table_type.base_id
-            meta = self.get_meta(id_)
-
-            tables[table_type.value] = Table.of(
-                table_type=table_type,
-                meta=meta,
-                rows=self.get_uploadable_data(id_, batch_size=10000),
-            )
+            if not self.get("sys_md_EntityType", q=f"id=={id_}"):
+                tables[table_type.value] = Table.of_placeholder(table_type)
+            else:
+                meta = self.get_meta(id_)
+                tables[table_type.value] = Table.of(
+                    table_type=table_type,
+                    meta=meta,
+                    rows=self.get_uploadable_data(id_, batch_size=10000),
+                )
 
         return NodeData.from_dict(
             node=self.node, source=Source.EXTERNAL_SERVER, tables=tables
         )
```

### Comparing `molgenis-py-bbmri-eric-1.8.0/src/molgenis/bbmri_eric/categories.py` & `molgenis-py-bbmri-eric-1.9.0/src/molgenis/bbmri_eric/categories.py`

 * *Files identical despite different names*

### Comparing `molgenis-py-bbmri-eric-1.8.0/src/molgenis/bbmri_eric/eric.py` & `molgenis-py-bbmri-eric-1.9.0/src/molgenis/bbmri_eric/eric.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         Parameters:
             nodes (List[ExternalServerNode]): The list of external nodes to stage
         """
         report = ErrorReport(nodes)
         for node in nodes:
             self.printer.print_node_title(node)
             try:
-                self._stage_node(node)
+                self._stage_node(node, report)
             except EricError as e:
                 self.printer.print_error(e)
                 report.add_node_error(node, e)
 
         self.printer.print_summary(report)
         return report
 
@@ -84,14 +84,15 @@
 
         self.printer.print("📦 Retrieving existing published data")
         published_data = self.session.get_published_data(
             nodes,
             AttributesRequest(
                 persons=["id", "national_node"],
                 networks=["id", "national_node"],
+                also_known_in=["id", "national_node"],
                 biobanks=["id", "pid", "name", "national_node"],
                 collections=["id", "national_node"],
             ),
         )
 
         self.printer.print("📦 Retrieving quality information")
         quality_info = self.session.get_quality_info()
@@ -112,15 +113,15 @@
         )
 
     def _prepare_nodes(self, nodes, state):
         for node in nodes:
             self.printer.print_node_title(node)
             try:
                 if isinstance(node, ExternalServerNode):
-                    self._stage_node(node)
+                    self._stage_node(node, state.report)
                 node_data = self.preparator.prepare(node, state)
                 state.data_to_publish.merge(node_data)
             except EricError as e:
                 self.printer.print_error(e)
                 state.existing_data.remove_node_rows(node)
                 state.report.add_node_error(node, e)
 
@@ -131,11 +132,13 @@
         try:
             self.publisher.publish(state)
         except EricError as e:
             self.printer.print_error(e)
             state.report.set_global_error(e)
 
     @requests_error_handler
-    def _stage_node(self, node: ExternalServerNode):
+    def _stage_node(self, node: ExternalServerNode, report: ErrorReport):
         self.printer.print(f"📥 Staging data of node {node.code}")
         with self.printer.indentation():
-            self.stager.stage(node)
+            warnings = self.stager.stage(node)
+            if warnings:
+                report.add_node_warnings(node, warnings)
```

### Comparing `molgenis-py-bbmri-eric-1.8.0/src/molgenis/bbmri_eric/errors.py` & `molgenis-py-bbmri-eric-1.9.0/src/molgenis/bbmri_eric/errors.py`

 * *Files identical despite different names*

### Comparing `molgenis-py-bbmri-eric-1.8.0/src/molgenis/bbmri_eric/model.py` & `molgenis-py-bbmri-eric-1.9.0/src/molgenis/bbmri_eric/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,18 +6,19 @@
 from enum import Enum
 from typing import Dict, List, Optional, Set
 
 from molgenis.bbmri_eric.utils import to_ordered_dict
 
 
 class TableType(Enum):
-    """Enum representing the four tables each national node has."""
+    """Enum representing the five tables each national node has."""
 
     PERSONS = "persons"
     NETWORKS = "networks"
+    ALSO_KNOWN = "also_known_in"
     BIOBANKS = "biobanks"
     COLLECTIONS = "collections"
 
     @classmethod
     def get_import_order(cls) -> List["TableType"]:
         return [type_ for type_ in cls]
 
@@ -90,14 +91,29 @@
         ids/rows."""
         return Table(rows_by_id=to_ordered_dict(rows), meta=meta, type=table_type)
 
     @staticmethod
     def of_empty(table_type: TableType, meta: TableMeta):
         return Table(rows_by_id=OrderedDict(), meta=meta, type=table_type)
 
+    @staticmethod
+    def of_placeholder(table_type: TableType):
+        meta = {
+            "data": {
+                "id": table_type.base_id,
+                "attributes": {
+                    "items": [{"data": {"name": "id", "idAttribute": True}}]
+                },
+            }
+        }
+        return Table.of_empty(
+            table_type=table_type,
+            meta=TableMeta(meta=meta),
+        )
+
 
 @dataclass(frozen=True)
 class OntologyTable(BaseTable):
     """
     Simple representation of an ontology table where the parent/child relations are
     persisted with self-references.
     """
@@ -137,14 +153,15 @@
 
     code: str
     description: Optional[str]
 
     _classifiers = {
         TableType.PERSONS: "contactID",
         TableType.NETWORKS: "networkID",
+        TableType.ALSO_KNOWN: "akiID",
         TableType.BIOBANKS: "ID",
         TableType.COLLECTIONS: "ID",
     }
 
     def get_staging_id(self, table_type: TableType) -> str:
         """
         Returns the identifier of a node's staging table.
@@ -203,40 +220,48 @@
     STAGING = "staging"
     PUBLISHED = "published"
     TRANSFORMED = "transformed"
 
 
 @dataclass
 class EricData(ABC):
-    """Abstract base class for containers storing rows from the four ERIC tables:
-    persons, networks, biobanks and collections."""
+    """Abstract base class for containers storing rows from the five ERIC tables:
+    persons, networks, also_known_in, biobanks and collections."""
 
     source: Source
     persons: Table
+    also_known_in: Table
     networks: Table
     biobanks: Table
     collections: Table
     table_by_type: Dict[TableType, Table] = field(init=False)
 
     def __post_init__(self):
         self.table_by_type = {
             TableType.PERSONS: self.persons,
             TableType.NETWORKS: self.networks,
+            TableType.ALSO_KNOWN: self.also_known_in,
             TableType.BIOBANKS: self.biobanks,
             TableType.COLLECTIONS: self.collections,
         }
 
     @property
     def import_order(self) -> List[Table]:
-        return [self.persons, self.networks, self.biobanks, self.collections]
+        return [
+            self.persons,
+            self.networks,
+            self.also_known_in,
+            self.biobanks,
+            self.collections,
+        ]
 
 
 @dataclass
 class NodeData(EricData):
-    """Container object storing the four tables of a single node."""
+    """Container object storing the five tables of a single node."""
 
     node: Node
 
     @staticmethod
     def from_dict(node: Node, source: Source, tables: Dict[str, Table]) -> "NodeData":
         return NodeData(node=node, source=source, **tables)
 
@@ -257,24 +282,25 @@
                 table.rows_by_id, TableMeta(metadata), table.type
             )
 
         return NodeData(node=self.node, source=Source.STAGING, **tables)
 
 
 class MixedData(EricData):
-    """Container object storing the four tables with mixed origins, for example from
+    """Container object storing the five tables with mixed origins, for example from
     the combined tables or from multiple staging areas."""
 
     @staticmethod
     def from_mixed_dict(source: Source, tables: Dict[str, Table]) -> "MixedData":
         return MixedData(source=source, **tables)
 
     def merge(self, other_data: EricData):
         self.persons.rows_by_id.update(other_data.persons.rows_by_id)
         self.networks.rows_by_id.update(other_data.networks.rows_by_id)
+        self.also_known_in.rows_by_id.update(other_data.also_known_in.rows_by_id)
         self.biobanks.rows_by_id.update(other_data.biobanks.rows_by_id)
         self.collections.rows_by_id.update(other_data.collections.rows_by_id)
 
     def remove_node_rows(self, node: Node):
         for table in self.import_order:
             ids_to_remove = [
                 row["id"] for row in table.rows if row["national_node"] == node.code
@@ -282,14 +308,15 @@
             all(table.rows_by_id.pop(id_) for id_ in ids_to_remove)
 
     def copy_empty(self) -> "MixedData":
         return MixedData(
             source=self.source,
             persons=Table.of_empty(TableType.PERSONS, self.persons.meta),
             networks=Table.of_empty(TableType.NETWORKS, self.networks.meta),
+            also_known_in=Table.of_empty(TableType.ALSO_KNOWN, self.also_known_in.meta),
             biobanks=Table.of_empty(TableType.BIOBANKS, self.biobanks.meta),
             collections=Table.of_empty(TableType.COLLECTIONS, self.collections.meta),
         )
 
 
 @dataclass(frozen=True)
 class QualityInfo:
```

### Comparing `molgenis-py-bbmri-eric-1.8.0/src/molgenis/bbmri_eric/pid_manager.py` & `molgenis-py-bbmri-eric-1.9.0/src/molgenis/bbmri_eric/pid_manager.py`

 * *Files identical despite different names*

### Comparing `molgenis-py-bbmri-eric-1.8.0/src/molgenis/bbmri_eric/pid_service.py` & `molgenis-py-bbmri-eric-1.9.0/src/molgenis/bbmri_eric/pid_service.py`

 * *Files identical despite different names*

### Comparing `molgenis-py-bbmri-eric-1.8.0/src/molgenis/bbmri_eric/printer.py` & `molgenis-py-bbmri-eric-1.9.0/src/molgenis/bbmri_eric/printer.py`

 * *Files identical despite different names*

### Comparing `molgenis-py-bbmri-eric-1.8.0/src/molgenis/bbmri_eric/publication_preparer.py` & `molgenis-py-bbmri-eric-1.9.0/src/molgenis/bbmri_eric/publication_preparer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from molgenis.bbmri_eric.bbmri_client import EricSession
 from molgenis.bbmri_eric.errors import ErrorReport, requests_error_handler
 from molgenis.bbmri_eric.model import Node, NodeData
+from molgenis.bbmri_eric.model_fitting import ModelFitter
 from molgenis.bbmri_eric.pid_manager import BasePidManager
 from molgenis.bbmri_eric.printer import Printer
 from molgenis.bbmri_eric.publisher import PublishingState
 from molgenis.bbmri_eric.transformer import Transformer
 from molgenis.bbmri_eric.validation import Validator
 
 
@@ -18,25 +19,36 @@
         self.pid_manager = pid_manager
         self.session = session
 
     @requests_error_handler
     def prepare(self, node: Node, state: PublishingState) -> NodeData:
         node_data = self._get_node_data(node)
         self._validate_node(node_data, state.report)
+        self._fit_node_model(node_data, state.report)
         self._transform_node(node_data, state)
         self._manage_node_pids(node_data, state)
         return node_data
 
     def _validate_node(self, node_data: NodeData, report: ErrorReport):
         self.printer.print(f"🔎 Validating staged data of node {node_data.node.code}")
         with self.printer.indentation():
             warnings = Validator(node_data, self.printer).validate()
             if warnings:
                 report.add_node_warnings(node_data.node, warnings)
 
+    def _fit_node_model(self, node_data: NodeData, report: ErrorReport):
+        self.printer.print(
+            f"⟺ Align staged data of node {node_data.node.code} "
+            f"with the published model"
+        )
+        with self.printer.indentation():
+            warnings = ModelFitter(node_data, self.printer).fit_model()
+            if warnings:
+                report.add_node_warnings(node_data.node, warnings)
+
     def _transform_node(self, node_data: NodeData, state: PublishingState):
         self.printer.print("✏️ Preparing staged data for publishing")
         with self.printer.indentation():
             warnings = Transformer(
                 node_data=node_data,
                 quality=state.quality_info,
                 printer=self.printer,
```

### Comparing `molgenis-py-bbmri-eric-1.8.0/src/molgenis/bbmri_eric/publisher.py` & `molgenis-py-bbmri-eric-1.9.0/src/molgenis/bbmri_eric/publisher.py`

 * *Files identical despite different names*

### Comparing `molgenis-py-bbmri-eric-1.8.0/src/molgenis/bbmri_eric/stager.py` & `molgenis-py-bbmri-eric-1.9.0/src/molgenis/bbmri_eric/stager.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,40 +1,62 @@
+from typing import List
+
 from molgenis.bbmri_eric.bbmri_client import EricSession, ExternalServerSession
-from molgenis.bbmri_eric.errors import requests_error_handler
+from molgenis.bbmri_eric.errors import EricWarning, requests_error_handler
 from molgenis.bbmri_eric.model import ExternalServerNode, NodeData, TableType
 from molgenis.bbmri_eric.printer import Printer
 
 
 class Stager:
     """
     This class is responsible for copying data from a node with an external server to
     its staging area in the BBMRI ERIC directory.
     """
 
     def __init__(self, session: EricSession, printer: Printer):
         self.session = session
         self.printer = printer
 
+        self.warnings: List[EricWarning] = list()
+
     @requests_error_handler
     def stage(self, node: ExternalServerNode):
         """
         Stages all data from the provided external node in the BBMRI-ERIC directory.
         """
+        self.warnings = []
         source_data = self._get_source_data(node)
         self._clear_staging_area(node)
         self._import_node(source_data)
 
+        return self.warnings
+
     def _get_source_data(self, node: ExternalServerNode) -> NodeData:
         """
-        Gets a node's data form an external server.
+        Gets a node's data from an external server.
+        First check if all tables are available
         """
         self.printer.print(f"📦 Retrieving node's data from {node.url}")
         source_session = ExternalServerSession(node=node)
+        self._check_tables(source_session)
         return source_session.get_node_data()
 
+    def _check_tables(self, session: ExternalServerSession):
+        """
+        Check if all tables are available on the external server
+        """
+        for table_type in TableType.get_import_order():
+            id_ = table_type.base_id
+            if not session.get("sys_md_EntityType", q=f"id=={id_}"):
+                warning = EricWarning(
+                    f"Node {session.node.code} has no {table_type.value} table"
+                )
+                self.printer.print_warning(warning, indent=1)
+                self.warnings.append(warning)
+
     def _clear_staging_area(self, node: ExternalServerNode):
         """
         Deletes all data in the staging area of an external node.
         """
         self.printer.print(f"🔥 Clearing staging area of {node.code}")
         for table_type in reversed(TableType.get_import_order()):
             self.session.delete(node.get_staging_id(table_type))
```

### Comparing `molgenis-py-bbmri-eric-1.8.0/src/molgenis/bbmri_eric/transformer.py` & `molgenis-py-bbmri-eric-1.9.0/src/molgenis/bbmri_eric/transformer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from collections import OrderedDict
-
 from molgenis.bbmri_eric.categories import CategoryMapper
 from molgenis.bbmri_eric.errors import EricWarning
 from molgenis.bbmri_eric.model import Node, NodeData, OntologyTable, QualityInfo, Table
 from molgenis.bbmri_eric.printer import Printer
 
 
 class Transformer:
@@ -46,15 +44,14 @@
         self._replace_eu_rows()
         self._set_commercial_use_bool()
         self._set_quality_info()
         self._set_biobank_pids()
         self._set_biobank_labels()
         self._set_combined_networks()
         self._set_combined_qualities()
-        self._merge_covid19_capabilities()
         self._set_collection_categories()
         return self.warnings
 
     def _set_commercial_use_bool(self):
         """
         Takes the data of a Node and sets the commercial_use boolean of all collections
         based on a set of criteria.
@@ -174,42 +171,14 @@
         coll_levels = self.quality.get_levels(self.node_data.collections.type)
         for collection in self.node_data.collections.rows:
             biobank = self.node_data.biobanks.rows_by_id[collection["biobank"]]
             bb_level = bb_levels.get(biobank["id"], [])
             coll_level = coll_levels.get(collection["id"], [])
             collection["combined_quality"] = list(set(bb_level + coll_level))
 
-    def _merge_covid19_capabilities(self):
-        """
-        Merges each biobank's 'covid19biobank' column into its 'capabilities' column and
-        then removes it.
-        """
-        self.printer.print("Merging 'covid19biobank' into 'capabilities'")
-
-        covid = "covid19biobank"
-        caps = "capabilities"
-        for biobank in self.node_data.biobanks.rows:
-            if covid in biobank and biobank[covid]:
-
-                warning = EricWarning(
-                    f"Biobank {biobank['id']} uses deprecated '{covid}' column. "
-                    f"Use '{caps}' instead."
-                )
-                self.printer.print_warning(warning, indent=1)
-                self.warnings.append(warning)
-
-                if not biobank[caps]:
-                    biobank[caps] = []
-
-                biobank[caps] = list(
-                    OrderedDict.fromkeys(biobank[caps] + biobank[covid])
-                )
-
-            biobank.pop(covid, None)
-
     def _set_collection_categories(self):
         """
         Sets the 'categories' field of each collection based on the collection values.
         """
         self.printer.print("Setting collection categories")
         for collection in self.node_data.collections.rows:
             collection["categories"] = self.category_mapper.map(collection)
```

### Comparing `molgenis-py-bbmri-eric-1.8.0/src/molgenis/bbmri_eric/utils.py` & `molgenis-py-bbmri-eric-1.9.0/src/molgenis/bbmri_eric/utils.py`

 * *Files identical despite different names*

### Comparing `molgenis-py-bbmri-eric-1.8.0/src/molgenis/bbmri_eric/validation.py` & `molgenis-py-bbmri-eric-1.9.0/src/molgenis/bbmri_eric/validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,21 +43,23 @@
             self._validate_xref(network, "contact")
             self._validate_mref(network, "parent_network")
 
     def _validate_biobanks(self):
         for biobank in self.node_data.biobanks.rows:
             self._validate_xref(biobank, "contact")
             self._validate_mref(biobank, "network")
+            self._validate_mref(biobank, "also_known_in")
 
     def _validate_collections(self):
         for collection in self.node_data.collections.rows:
             self._validate_xref(collection, "contact")
             self._validate_xref(collection, "biobank")
             self._validate_xref(collection, "parent_collection")
             self._validate_mref(collection, "networks")
+            self._validate_mref(collection, "also_known_in")
             self._validate_ages(
                 collection,
             )
 
     def _validate_ages(self, collection: dict):
         low = collection.get("age_low", None)
         high = collection.get("age_high", None)
```

### Comparing `molgenis-py-bbmri-eric-1.8.0/src/molgenis_py_bbmri_eric.egg-info/PKG-INFO` & `molgenis-py-bbmri-eric-1.9.0/src/molgenis_py_bbmri_eric.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: molgenis-py-bbmri-eric
-Version: 1.8.0
+Version: 1.9.0
 Summary: MOLGENIS Python tooling for BBMRI-ERIC
 Home-page: https://github.com/molgenis/molgenis-py-bbmri-eric
 Author: Tommy de Boer
 Author-email: t.de.boer01@umcg.nl
 License: LGPL-3.0-only
 Project-URL: Source, https://github.com/molgenis/molgenis-py-bbmri-eric
 Platform: any
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Provides-Extra: testing
 License-File: LICENSE.txt
 License-File: AUTHORS.md
 
 # molgenis-py-bbmri-eric
```

### Comparing `molgenis-py-bbmri-eric-1.8.0/src/molgenis_py_bbmri_eric.egg-info/SOURCES.txt` & `molgenis-py-bbmri-eric-1.9.0/src/molgenis_py_bbmri_eric.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 scripts/sync_DE_qualities.py
 src/molgenis/bbmri_eric/__init__.py
 src/molgenis/bbmri_eric/bbmri_client.py
 src/molgenis/bbmri_eric/categories.py
 src/molgenis/bbmri_eric/eric.py
 src/molgenis/bbmri_eric/errors.py
 src/molgenis/bbmri_eric/model.py
+src/molgenis/bbmri_eric/model_fitting.py
 src/molgenis/bbmri_eric/pid_manager.py
 src/molgenis/bbmri_eric/pid_service.py
 src/molgenis/bbmri_eric/printer.py
 src/molgenis/bbmri_eric/publication_preparer.py
 src/molgenis/bbmri_eric/publisher.py
 src/molgenis/bbmri_eric/stager.py
 src/molgenis/bbmri_eric/transformer.py
@@ -44,19 +45,25 @@
 src/molgenis_py_bbmri_eric.egg-info/top_level.txt
 tests/__init__.py
 tests/conftest.py
 tests/test_categories.py
 tests/test_eric.py
 tests/test_errors.py
 tests/test_model.py
+tests/test_model_fitting.py
 tests/test_pid_manager.py
 tests/test_pid_service.py
 tests/test_printer.py
 tests/test_publication_preparer.py
 tests/test_publisher.py
 tests/test_stager.py
 tests/test_transformer.py
 tests/test_utils.py
 tests/test_validator.py
 tests/resources/__init__.py
+tests/resources/also_known.json
+tests/resources/biobanks.json
+tests/resources/collections.json
+tests/resources/networks.json
 tests/resources/node_data.pkl
-tests/resources/node_data_pickler.py
+tests/resources/node_data_pickler.py
+tests/resources/persons.json
```

### Comparing `molgenis-py-bbmri-eric-1.8.0/tests/resources/node_data.pkl` & `molgenis-py-bbmri-eric-1.9.0/tests/resources/node_data.pkl`

 * *Files identical despite different names*

### Comparing `molgenis-py-bbmri-eric-1.8.0/tests/resources/node_data_pickler.py` & `molgenis-py-bbmri-eric-1.9.0/tests/resources/node_data_pickler.py`

 * *Files identical despite different names*

### Comparing `molgenis-py-bbmri-eric-1.8.0/tests/test_categories.py` & `molgenis-py-bbmri-eric-1.9.0/tests/test_categories.py`

 * *Files identical despite different names*

### Comparing `molgenis-py-bbmri-eric-1.8.0/tests/test_eric.py` & `molgenis-py-bbmri-eric-1.9.0/tests/test_eric.py`

 * *Files 6% similar despite different names*

```diff
@@ -79,25 +79,27 @@
 def test_publish_nodes(eric, report_init):
     no = Node("NO", "succeeds")
     nl = ExternalServerNode("NL", "fails during publishing", "url")
     state = _setup_state([no, nl], eric, report_init)
 
     error = EricError("error")
     eric.publisher.publish.side_effect = error
+    eric.stager.stage.return_value = []
 
     report = eric.publish_nodes([no, nl])
 
     assert eric.printer.print_node_title.mock_calls == [call(no), call(nl)]
+    eric.stager.stage.assert_has_calls([call(nl)])
     eric.preparator.prepare.assert_has_calls(
         [call(no, state), call(nl, state)], any_order=True
     )
     eric.publisher.publish.assert_called_with(state)
     assert len(report.node_errors) == 0
     assert report.error == error
-    assert len(report.node_warnings) == 0
+    assert len(report.node_warnings[nl]) == 0
     eric.printer.print_summary.assert_called_once_with(report)
 
 
 # noinspection PyProtectedMember
 def _setup_state(nodes: List[Node], eric: Eric, report_init):
     report = ErrorReport(nodes)
     report_init.return_value = report
```

### Comparing `molgenis-py-bbmri-eric-1.8.0/tests/test_errors.py` & `molgenis-py-bbmri-eric-1.9.0/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `molgenis-py-bbmri-eric-1.8.0/tests/test_model.py` & `molgenis-py-bbmri-eric-1.9.0/tests/test_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,22 +11,24 @@
 )
 
 
 def test_table_type_order():
     assert TableType.get_import_order() == [
         TableType.PERSONS,
         TableType.NETWORKS,
+        TableType.ALSO_KNOWN,
         TableType.BIOBANKS,
         TableType.COLLECTIONS,
     ]
 
 
 def test_table_type_base_ids():
     assert TableType.PERSONS.base_id == "eu_bbmri_eric_persons"
     assert TableType.NETWORKS.base_id == "eu_bbmri_eric_networks"
+    assert TableType.ALSO_KNOWN.base_id == "eu_bbmri_eric_also_known_in"
     assert TableType.BIOBANKS.base_id == "eu_bbmri_eric_biobanks"
     assert TableType.COLLECTIONS.base_id == "eu_bbmri_eric_collections"
 
 
 def test_table_factory_method():
     row1 = {"id": "1"}
     row2 = {"id": "2"}
@@ -72,21 +74,29 @@
     assert node.get_staging_id(TableType.PERSONS) == "eu_bbmri_eric_NL_persons"
     assert node.url == "test.nl"
 
 
 def test_node_data_order():
     persons = Table.of(TableType.PERSONS, MagicMock(), [{"id": "1"}])
     networks = Table.of(TableType.NETWORKS, MagicMock(), [{"id": "1"}])
+    also_known_in = Table.of(TableType.ALSO_KNOWN, MagicMock(), [{"id": "1"}])
     biobanks = Table.of(TableType.BIOBANKS, MagicMock(), [{"id": "1"}])
     collections = Table.of(TableType.COLLECTIONS, MagicMock(), [{"id": "1"}])
     node = Node("NL", "NL")
 
     node_data = NodeData(
         node=node,
         source=Source.STAGING,
         persons=persons,
         networks=networks,
+        also_known_in=also_known_in,
         biobanks=biobanks,
         collections=collections,
     )
 
-    assert node_data.import_order == [persons, networks, biobanks, collections]
+    assert node_data.import_order == [
+        persons,
+        networks,
+        also_known_in,
+        biobanks,
+        collections,
+    ]
```

### Comparing `molgenis-py-bbmri-eric-1.8.0/tests/test_pid_manager.py` & `molgenis-py-bbmri-eric-1.9.0/tests/test_pid_manager.py`

 * *Files identical despite different names*

### Comparing `molgenis-py-bbmri-eric-1.8.0/tests/test_pid_service.py` & `molgenis-py-bbmri-eric-1.9.0/tests/test_pid_service.py`

 * *Files identical despite different names*

### Comparing `molgenis-py-bbmri-eric-1.8.0/tests/test_printer.py` & `molgenis-py-bbmri-eric-1.9.0/tests/test_printer.py`

 * *Files identical despite different names*

### Comparing `molgenis-py-bbmri-eric-1.8.0/tests/test_publication_preparer.py` & `molgenis-py-bbmri-eric-1.9.0/tests/test_publication_preparer.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,22 @@
 @pytest.fixture
 def validator_init():
     with patch("molgenis.bbmri_eric.publication_preparer.Validator") as validator_mock:
         yield validator_mock
 
 
 @pytest.fixture
+def model_fitter_init():
+    with patch(
+        "molgenis.bbmri_eric.publication_preparer.ModelFitter"
+    ) as model_fitter_mock:
+        yield model_fitter_mock
+
+
+@pytest.fixture
 def transformer_init():
     with patch(
         "molgenis.bbmri_eric.publication_preparer.Transformer"
     ) as transformer_mock:
         yield transformer_mock
 
 
@@ -30,14 +38,16 @@
 def preparer(session, printer, pid_manager):
     return PublicationPreparer(printer, pid_manager, session)
 
 
 def test_prepare(preparer, session):
     validate_func = MagicMock()
     preparer._validate_node = validate_func
+    model_fitter_func = MagicMock()
+    preparer._fit_node_model = model_fitter_func
     transform_func = MagicMock()
     preparer._transform_node = transform_func
     manage_pids_func = MagicMock()
     preparer._manage_node_pids = manage_pids_func
     nl = Node.of("NL")
     state = MagicMock()
     report = MagicMock()
@@ -45,14 +55,15 @@
     node_data = MagicMock()
     session.get_staging_node_data.return_value = node_data
 
     preparer.prepare(nl, state)
 
     session.get_staging_node_data.assert_called_with(nl)
     validate_func.assert_called_with(node_data, report)
+    model_fitter_func.assert_called_with(node_data, report)
     transform_func.assert_called_with(node_data, state)
     manage_pids_func.assert_called_with(node_data, state)
 
 
 def test_validate(preparer: PublicationPreparer, validator_init, printer):
     validator = MagicMock()
     validator_init.return_value = validator
@@ -76,14 +87,40 @@
     report: ErrorReport = ErrorReport([nl])
 
     preparer._validate_node(node_data, report)
 
     assert report.node_warnings[nl] == [warning]
 
 
+def test_model_fitting(preparer: PublicationPreparer, model_fitter_init):
+    model_fitter = MagicMock()
+    model_fitter_init.return_value = model_fitter
+
+    preparer._fit_node_model(MagicMock(), MagicMock())
+
+    assert model_fitter_init.called
+    assert model_fitter.fit_model.called
+
+
+def test_model_fitting_warnings(preparer: PublicationPreparer, model_fitter_init):
+    model_fitter = MagicMock()
+    model_fitter_init.return_value = model_fitter
+    warning = EricWarning("warning")
+    model_fitter.fit_model.return_value = [warning]
+    node_data = MagicMock()
+    nl = Node.of("NL")
+    node_data.node = nl
+    state = MagicMock()
+    state.report = ErrorReport(nl)
+
+    preparer._fit_node_model(node_data, state.report)
+
+    assert state.report.node_warnings[nl] == [warning]
+
+
 def test_transform(preparer: PublicationPreparer, transformer_init):
     transformer = MagicMock()
     transformer_init.return_value = transformer
 
     preparer._transform_node(MagicMock(), MagicMock())
 
     assert transformer_init.called
```

### Comparing `molgenis-py-bbmri-eric-1.8.0/tests/test_publisher.py` & `molgenis-py-bbmri-eric-1.9.0/tests/test_publisher.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from unittest import mock
 from unittest.mock import MagicMock, patch
 
 import pytest
 
-from molgenis.bbmri_eric.errors import ErrorReport
+from molgenis.bbmri_eric.errors import EricWarning, ErrorReport
 from molgenis.bbmri_eric.model import (
     MixedData,
     Node,
     NodeData,
     QualityInfo,
     Source,
     Table,
@@ -34,14 +34,15 @@
 
     state = PublishingState(
         nodes=[Node.of("NL"), Node.of("BE")],
         existing_data=MixedData(
             source=Source.TRANSFORMED,
             persons=Table.of_empty(TableType.PERSONS, MagicMock()),
             networks=Table.of_empty(TableType.NETWORKS, MagicMock()),
+            also_known_in=Table.of_empty(TableType.ALSO_KNOWN, MagicMock()),
             biobanks=Table.of_empty(TableType.BIOBANKS, MagicMock()),
             collections=Table.of_empty(TableType.COLLECTIONS, MagicMock()),
         ),
         eu_node_data=MagicMock(),
         quality_info=MagicMock(),
         report=MagicMock(),
         diseases=MagicMock(),
@@ -51,43 +52,55 @@
 
     session.import_as_csv.assert_called_with(state.data_to_publish)
     assert publisher._delete_rows.mock_calls == [
         mock.call(
             state.data_to_publish.collections, state.existing_data.collections, state
         ),
         mock.call(state.data_to_publish.biobanks, state.existing_data.biobanks, state),
+        mock.call(
+            state.data_to_publish.also_known_in,
+            state.existing_data.also_known_in,
+            state,
+        ),
         mock.call(state.data_to_publish.networks, state.existing_data.networks, state),
         mock.call(state.data_to_publish.persons, state.existing_data.persons, state),
     ]
 
 
 def test_delete_rows(publisher, pid_service, node_data: NodeData, session):
-    existing_biobanks_table = MagicMock()
-    existing_biobanks_table.rows_by_id.return_value = {
-        "bbmri-eric:ID:NO_OUS": {"pid": "pid1"},
-        "delete_this_row": {"pid": "pid2"},
-        "undeletable_id": {"pid": "pid3"},
-    }
-    existing_biobanks_table.rows_by_id.keys.return_value = {
-        "bbmri-eric:ID:NO_OUS",
-        "delete_this_row",
-        "undeletable_id",
-    }
+    existing_biobanks_table = Table.of(
+        table_type=TableType.BIOBANKS,
+        meta=MagicMock(),
+        rows=[
+            {
+                "id": "bbmri-eric:ID:NL_valid-biobankID-1",
+                "pid": "pid1",
+                "national_node": "NL",
+            },
+            {"id": "delete_this_row", "pid": "pid2", "national_node": "NL"},
+            {"id": "undeletable_id", "pid": "pid3", "national_node": "NL"},
+        ],
+    )
+
     state: PublishingState = MagicMock()
     state.quality_info = QualityInfo(
         biobanks={"undeletable_id": ["quality"]},
         collections={},
         biobank_levels={},
         collection_levels={},
     )
-    state.report = ErrorReport([Node.of("NO")])
+
+    state.report = ErrorReport([node_data.node])
+
+    warning = EricWarning(
+        "Prevented the deletion of a row that is referenced from "
+        "the quality info: biobanks undeletable_id."
+    )
 
     publisher._delete_rows(node_data.biobanks, existing_biobanks_table, state)
 
-    publisher.pid_manager.terminate_biobanks(["pid2"])
+    publisher.pid_manager.terminate_biobanks.assert_called_with(["pid2"])
     session.delete_list.assert_called_with(
         "eu_bbmri_eric_biobanks", ["delete_this_row"]
     )
-    publisher.warnings = [
-        "Prevented the deletion of a row that is referenced from "
-        "the quality info: biobanks undeletable_id."
-    ]
+
+    assert state.report.node_warnings[node_data.node] == [warning]
```

### Comparing `molgenis-py-bbmri-eric-1.8.0/tests/test_stager.py` & `molgenis-py-bbmri-eric-1.9.0/tests/test_stager.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from unittest import mock
 from unittest.mock import MagicMock, patch
 
 import pytest
 
 from molgenis.bbmri_eric.bbmri_client import EricSession
+from molgenis.bbmri_eric.errors import EricWarning
 from molgenis.bbmri_eric.model import ExternalServerNode, NodeData
 from molgenis.bbmri_eric.printer import Printer
 from molgenis.bbmri_eric.stager import Stager
 
 
 @pytest.fixture
 def external_server_init():
@@ -39,24 +40,45 @@
 
     source_data = Stager(MagicMock(), Printer())._get_source_data(node)
 
     external_server_init.assert_called_with(node=node)
     assert source_data == node_data
 
 
+def test_check_tables(external_server_init):
+    node = ExternalServerNode("NL", "Netherlands", "url.nl")
+    session = external_server_init.return_value
+    session.get.return_value = []
+    session.node = node
+    stager = Stager(MagicMock(), Printer())
+
+    warnings = stager.stage(node)
+
+    external_server_init.assert_called_with(node=node)
+
+    assert session.get.call_count == 5
+
+    assert warnings[0] == EricWarning("Node NL has no persons table")
+    assert warnings[1] == EricWarning("Node NL has no networks table")
+    assert warnings[2] == EricWarning("Node NL has no also_known_in table")
+    assert warnings[3] == EricWarning("Node NL has no biobanks table")
+    assert warnings[4] == EricWarning("Node NL has no collections table")
+
+
 def test_clear_staging_area():
     session = EricSession("url")
     session.delete = MagicMock(name="delete")
     node = ExternalServerNode("NL", "Netherlands", "url.nl")
 
     Stager(session, Printer())._clear_staging_area(node)
 
     assert session.delete.mock_calls == [
         mock.call("eu_bbmri_eric_NL_collections"),
         mock.call("eu_bbmri_eric_NL_biobanks"),
+        mock.call("eu_bbmri_eric_NL_also_known_in"),
         mock.call("eu_bbmri_eric_NL_networks"),
         mock.call("eu_bbmri_eric_NL_persons"),
     ]
 
 
 def test_import_node(session, external_server_init):
     node_data: NodeData = MagicMock()
```

### Comparing `molgenis-py-bbmri-eric-1.8.0/tests/test_transformer.py` & `molgenis-py-bbmri-eric-1.9.0/tests/test_transformer.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     for table in node_data.import_order:
         assert "national_node" not in table.rows[0]
 
     transformer.node_data = node_data
     transformer._set_national_node_code()
 
     for table in node_data.import_order:
-        assert table.rows[0]["national_node"] == "NO"
+        assert table.rows[0]["national_node"] == "NL"
 
 
 def test_transformer_commercial_use(transformer):
     node_data = MagicMock()
     node_data.collections.rows = [
         {"biobank": "biobank1", "collaboration_commercial": True},
         {"biobank": "biobank1", "collaboration_commercial": False},
@@ -62,45 +62,43 @@
     assert node_data.collections.rows[7]["commercial_use"] is False
     assert node_data.collections.rows[8]["commercial_use"] is False
 
 
 def test_transformer_quality(node_data, transformer):
     q_info = QualityInfo(
         biobanks={
-            "bbmri-eric:ID:NO_BIOBANK1": ["quality1", "quality2"],
-            "bbmri-eric:ID:NO_CoronaTrondelag": ["quality3"],
+            "bbmri-eric:ID:NL_test_quality_biobank1": ["quality1", "quality2"],
+            "bbmri-eric:ID:NL_test_quality_biobank2": ["quality3"],
         },
         biobank_levels={},
-        collections={
-            "bbmri-eric:ID:NO_bbmri-eric:ID:NO_CancerBiobankOUH:collection"
-            ":all_samples_samples": ["quality1"]
-        },
+        collections={"bbmri-eric:ID:NL_bb1:collection:test_quality1": ["quality1"]},
         collection_levels={},
     )
     transformer.node_data = node_data
     transformer.quality = q_info
 
     transformer._set_quality_info()
 
-    assert node_data.biobanks.rows_by_id["bbmri-eric:ID:NO_BIOBANK1"]["quality"] == [
-        "quality1",
-        "quality2",
-    ]
-    assert "quality" not in node_data.biobanks.rows_by_id["bbmri-eric:ID:NO_Janus"]
-    assert node_data.biobanks.rows_by_id["bbmri-eric:ID:NO_CoronaTrondelag"][
+    assert node_data.biobanks.rows_by_id["bbmri-eric:ID:NL_test_quality_biobank1"][
+        "quality"
+    ] == ["quality1", "quality2"]
+    assert (
+        "quality"
+        not in node_data.biobanks.rows_by_id["bbmri-eric:ID:NL_biobank_noQual"]
+    )
+    assert node_data.biobanks.rows_by_id["bbmri-eric:ID:NL_test_quality_biobank2"][
         "quality"
     ] == ["quality3"]
     assert node_data.collections.rows_by_id[
-        "bbmri-eric:ID:NO_bbmri-eric:ID:NO_CancerBiobankOUH:collection"
-        ":all_samples_samples"
+        "bbmri-eric:ID:NL_bb1:collection:test_quality1"
     ]["quality"] == ["quality1"]
     assert (
         "quality"
         not in node_data.collections.rows_by_id[
-            "bbmri-eric:ID:NO_moba:collection:all_samples"
+            "bbmri-eric:ID:NL_bb1:collection:test_noQual"
         ]
     )
 
 
 def test_transformer_replace_eu_rows_skip_eu(transformer):
     eu = Node("EU", "Europe")
     node_data = MagicMock()
@@ -215,86 +213,58 @@
     assert set(node_data.collections.rows[5]["combined_network"]) == set()
 
 
 def test_transformer_combined_quality(node_data, transformer):
     q_info = QualityInfo(
         biobanks={},
         biobank_levels={
-            "bbmri-eric:ID:NO_BIOBANK1": ["level_bio1", "level_bio2"],
-            "bbmri-eric:ID:NO_CoronaTrondelag": ["level_bio3"],
-            "bbmri-eric:ID:NO_SorlandetHospital": ["level_bio_col"],
+            "bbmri-eric:ID:NL_test_quality_biobank1": ["level_bio1", "level_bio2"],
+            "bbmri-eric:ID:NL_test_quality_biobank2": ["level_bio3"],
+            "bbmri-eric:ID:NL_test_quality_biobank3": ["level_bio_col"],
         },
         collections={},
         collection_levels={
-            "bbmri-eric:ID:NO_bbmri-eric:ID:NO_CancerBiobankOUH:collection"
-            ":all_samples_samples": ["level_col5"],
-            "bbmri-eric:ID:NO_CoronaTrondelag:collection:COVID19": ["level_col2"],
-            "bbmri-eric:ID:NO_SorlandetHospital:collection:all_ColoRectalCancer": [
-                "level_bio_col"
-            ],
+            "bbmri-eric:ID:NL_bb1:collection:test_quality1": ["level_col5"],
+            "bbmri-eric:ID:NL_bb1:collection:test_quality2": ["level_col2"],
+            "bbmri-eric:ID:NL_bb3:collection:test_quality3": ["level_bio_col"],
         },
     )
     transformer.node_data = node_data
     transformer.quality = q_info
 
     transformer._set_combined_qualities()
 
     assert (
         "combined_quality"
-        not in node_data.biobanks.rows_by_id["bbmri-eric:ID:NO_BIOBANK1"]
+        not in node_data.biobanks.rows_by_id["bbmri-eric:ID:NL_biobank_noQual"]
     )
     assert sorted(
-        node_data.collections.rows_by_id[
-            "bbmri-eric:ID:NO_BIOBANK1:collection:all_samples"
-        ]["combined_quality"]
+        node_data.collections.rows_by_id["bbmri-eric:ID:NL_bb1:collection:test_noQual"][
+            "combined_quality"
+        ]
     ) == sorted(["level_bio1", "level_bio2"])
     assert sorted(
         node_data.collections.rows_by_id[
-            "bbmri-eric:ID:NO_CoronaTrondelag:collection:COVID19"
+            "bbmri-eric:ID:NL_bb1:collection:test_quality2"
         ]["combined_quality"]
     ) == sorted(["level_col2", "level_bio3"])
     assert node_data.collections.rows_by_id[
-        "bbmri-eric:ID:NO_bbmri-eric:ID:NO_CancerBiobankOUH:collection"
-        ":all_samples_samples"
+        "bbmri-eric:ID:NL_bb1:collection:test_quality1"
     ]["combined_quality"] == ["level_col5"]
     assert node_data.collections.rows_by_id[
-        "bbmri-eric:ID:NO_SorlandetHospital:collection:" "all_ColoRectalCancer"
+        "bbmri-eric:ID:NL_bb3:collection:test_quality3"
     ]["combined_quality"] == ["level_bio_col"]
     assert (
-        node_data.collections.rows_by_id[
-            "bbmri-eric:ID:NO_moba:collection:all_samples"
-        ]["combined_quality"]
+        node_data.collections.rows_by_id["bbmri-eric:ID:NL_valid-collectionID-1"][
+            "combined_quality"
+        ]
         == []
     )
 
 
-def test_merge_covid19_capabilities(transformer):
-    node_data = MagicMock()
-    node_data.biobanks.rows = [
-        {"id": "0"},
-        {"id": "1", "covid19biobank": None, "capabilities": None},
-        {"id": "2", "covid19biobank": None, "capabilities": ["a", "b"]},
-        {"id": "3", "covid19biobank": ["c"], "capabilities": ["a", "b"]},
-        {"id": "4", "covid19biobank": ["c"], "capabilities": None},
-        {"id": "5", "covid19biobank": ["a"], "capabilities": ["a", "b"]},
-    ]
-    transformer.node_data = node_data
-
-    transformer._merge_covid19_capabilities()
-
-    assert node_data.biobanks.rows == [
-        {"id": "0"},
-        {"id": "1", "capabilities": None},
-        {"id": "2", "capabilities": ["a", "b"]},
-        {"id": "3", "capabilities": ["a", "b", "c"]},
-        {"id": "4", "capabilities": ["c"]},
-        {"id": "5", "capabilities": ["a", "b"]},
-    ]
-
-
 def test_map_categories(transformer):
     node_data = MagicMock()
     collection1 = MagicMock()
     collection2 = MagicMock()
     node_data.collections.rows = [collection1, collection2]
     category_mapper = MagicMock()
     transformer.node_data = node_data
```

### Comparing `molgenis-py-bbmri-eric-1.8.0/tests/test_utils.py` & `molgenis-py-bbmri-eric-1.9.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `molgenis-py-bbmri-eric-1.8.0/tox.ini` & `molgenis-py-bbmri-eric-1.9.0/tox.ini`

 * *Files identical despite different names*

