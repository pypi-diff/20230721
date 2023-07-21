# Comparing `tmp/core_oaipmh_common_app-2.3.0.tar.gz` & `tmp/core_oaipmh_common_app-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_oaipmh_common_app-2.3.0.tar", last modified: Tue May  2 19:46:58 2023, max compression
+gzip compressed data, was "core_oaipmh_common_app-2.4.0.tar", last modified: Fri Jul 21 02:16:01 2023, max compression
```

## Comparing `core_oaipmh_common_app-2.3.0.tar` & `core_oaipmh_common_app-2.4.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:58.567983 core_oaipmh_common_app-2.3.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-05-02 19:46:55.000000 core_oaipmh_common_app-2.3.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      177 2023-05-02 19:46:55.000000 core_oaipmh_common_app-2.3.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1089 2023-05-02 19:46:58.563030 core_oaipmh_common_app-2.3.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      593 2023-05-02 19:46:55.000000 core_oaipmh_common_app-2.3.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:58.107177 core_oaipmh_common_app-2.3.0/core_oaipmh_common_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:55.000000 core_oaipmh_common_app-2.3.0/core_oaipmh_common_app/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:58.218639 core_oaipmh_common_app-2.3.0/core_oaipmh_common_app/commons/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:55.000000 core_oaipmh_common_app-2.3.0/core_oaipmh_common_app/commons/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1643 2023-05-02 19:46:55.000000 core_oaipmh_common_app-2.3.0/core_oaipmh_common_app/commons/exceptions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      798 2023-05-02 19:46:55.000000 core_oaipmh_common_app-2.3.0/core_oaipmh_common_app/commons/messages.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:58.233531 core_oaipmh_common_app-2.3.0/core_oaipmh_common_app/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:55.000000 core_oaipmh_common_app-2.3.0/core_oaipmh_common_app/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:58.275369 core_oaipmh_common_app-2.3.0/core_oaipmh_common_app/components/oai_metadata_format/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:55.000000 core_oaipmh_common_app-2.3.0/core_oaipmh_common_app/components/oai_metadata_format/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1094 2023-05-02 19:46:55.000000 core_oaipmh_common_app-2.3.0/core_oaipmh_common_app/components/oai_metadata_format/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2908 2023-05-02 19:46:55.000000 core_oaipmh_common_app-2.3.0/core_oaipmh_common_app/components/oai_metadata_format/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:58.330635 core_oaipmh_common_app-2.3.0/core_oaipmh_common_app/components/oai_set/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:55.000000 core_oaipmh_common_app-2.3.0/core_oaipmh_common_app/components/oai_set/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      795 2023-05-02 19:46:55.000000 core_oaipmh_common_app-2.3.0/core_oaipmh_common_app/components/oai_set/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2033 2023-05-02 19:46:55.000000 core_oaipmh_common_app-2.3.0/core_oaipmh_common_app/components/oai_set/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:58.344536 core_oaipmh_common_app-2.3.0/core_oaipmh_common_app/migrations/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:55.000000 core_oaipmh_common_app-2.3.0/core_oaipmh_common_app/migrations/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:58.370711 core_oaipmh_common_app-2.3.0/core_oaipmh_common_app/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      819 2023-05-02 19:46:55.000000 core_oaipmh_common_app-2.3.0/core_oaipmh_common_app/utils/UTCdatetime.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:55.000000 core_oaipmh_common_app-2.3.0/core_oaipmh_common_app/utils/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:58.176063 core_oaipmh_common_app-2.3.0/core_oaipmh_common_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1089 2023-05-02 19:46:57.000000 core_oaipmh_common_app-2.3.0/core_oaipmh_common_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1372 2023-05-02 19:46:57.000000 core_oaipmh_common_app-2.3.0/core_oaipmh_common_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-05-02 19:46:57.000000 core_oaipmh_common_app-2.3.0/core_oaipmh_common_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       63 2023-05-02 19:46:57.000000 core_oaipmh_common_app-2.3.0/core_oaipmh_common_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       29 2023-05-02 19:46:57.000000 core_oaipmh_common_app-2.3.0/core_oaipmh_common_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-05-02 19:46:56.000000 core_oaipmh_common_app-2.3.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       21 2023-05-02 19:46:56.000000 core_oaipmh_common_app-2.3.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       42 2023-05-02 19:46:56.000000 core_oaipmh_common_app-2.3.0/requirements.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-05-02 19:46:58.569823 core_oaipmh_common_app-2.3.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1420 2023-05-02 19:46:56.000000 core_oaipmh_common_app-2.3.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:58.410889 core_oaipmh_common_app-2.3.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:56.000000 core_oaipmh_common_app-2.3.0/tests/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:58.421177 core_oaipmh_common_app-2.3.0/tests/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:56.000000 core_oaipmh_common_app-2.3.0/tests/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:58.465680 core_oaipmh_common_app-2.3.0/tests/components/oai_metadata_format/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:56.000000 core_oaipmh_common_app-2.3.0/tests/components/oai_metadata_format/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6179 2023-05-02 19:46:56.000000 core_oaipmh_common_app-2.3.0/tests/components/oai_metadata_format/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:58.489570 core_oaipmh_common_app-2.3.0/tests/components/oai_set/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:56.000000 core_oaipmh_common_app-2.3.0/tests/components/oai_set/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:58.521817 core_oaipmh_common_app-2.3.0/tests/components/oai_set/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:56.000000 core_oaipmh_common_app-2.3.0/tests/components/oai_set/tests/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4771 2023-05-02 19:46:56.000000 core_oaipmh_common_app-2.3.0/tests/components/oai_set/tests/tests_unit.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1510 2023-05-02 19:46:56.000000 core_oaipmh_common_app-2.3.0/tests/test_settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:58.552923 core_oaipmh_common_app-2.3.0/tests/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:56.000000 core_oaipmh_common_app-2.3.0/tests/utils/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1286 2023-05-02 19:46:56.000000 core_oaipmh_common_app-2.3.0/tests/utils/tests_iso8601_operation.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:01.382955 core_oaipmh_common_app-2.4.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-07-21 02:15:58.000000 core_oaipmh_common_app-2.4.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      177 2023-07-21 02:15:58.000000 core_oaipmh_common_app-2.4.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1089 2023-07-21 02:16:01.378978 core_oaipmh_common_app-2.4.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      593 2023-07-21 02:15:58.000000 core_oaipmh_common_app-2.4.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:00.968358 core_oaipmh_common_app-2.4.0/core_oaipmh_common_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:15:58.000000 core_oaipmh_common_app-2.4.0/core_oaipmh_common_app/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:01.069396 core_oaipmh_common_app-2.4.0/core_oaipmh_common_app/commons/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:15:58.000000 core_oaipmh_common_app-2.4.0/core_oaipmh_common_app/commons/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1643 2023-07-21 02:15:58.000000 core_oaipmh_common_app-2.4.0/core_oaipmh_common_app/commons/exceptions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      798 2023-07-21 02:15:58.000000 core_oaipmh_common_app-2.4.0/core_oaipmh_common_app/commons/messages.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:01.095811 core_oaipmh_common_app-2.4.0/core_oaipmh_common_app/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:15:58.000000 core_oaipmh_common_app-2.4.0/core_oaipmh_common_app/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:01.148877 core_oaipmh_common_app-2.4.0/core_oaipmh_common_app/components/oai_metadata_format/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:15:58.000000 core_oaipmh_common_app-2.4.0/core_oaipmh_common_app/components/oai_metadata_format/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1094 2023-07-21 02:15:58.000000 core_oaipmh_common_app-2.4.0/core_oaipmh_common_app/components/oai_metadata_format/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2908 2023-07-21 02:15:58.000000 core_oaipmh_common_app-2.4.0/core_oaipmh_common_app/components/oai_metadata_format/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:01.183699 core_oaipmh_common_app-2.4.0/core_oaipmh_common_app/components/oai_set/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:15:58.000000 core_oaipmh_common_app-2.4.0/core_oaipmh_common_app/components/oai_set/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      795 2023-07-21 02:15:59.000000 core_oaipmh_common_app-2.4.0/core_oaipmh_common_app/components/oai_set/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2033 2023-07-21 02:15:59.000000 core_oaipmh_common_app-2.4.0/core_oaipmh_common_app/components/oai_set/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:01.194215 core_oaipmh_common_app-2.4.0/core_oaipmh_common_app/migrations/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:15:59.000000 core_oaipmh_common_app-2.4.0/core_oaipmh_common_app/migrations/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:01.226227 core_oaipmh_common_app-2.4.0/core_oaipmh_common_app/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      865 2023-07-21 02:15:59.000000 core_oaipmh_common_app-2.4.0/core_oaipmh_common_app/utils/UTCdatetime.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:15:59.000000 core_oaipmh_common_app-2.4.0/core_oaipmh_common_app/utils/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:01.028739 core_oaipmh_common_app-2.4.0/core_oaipmh_common_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1089 2023-07-21 02:16:00.000000 core_oaipmh_common_app-2.4.0/core_oaipmh_common_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1372 2023-07-21 02:16:00.000000 core_oaipmh_common_app-2.4.0/core_oaipmh_common_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-07-21 02:16:00.000000 core_oaipmh_common_app-2.4.0/core_oaipmh_common_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       63 2023-07-21 02:16:00.000000 core_oaipmh_common_app-2.4.0/core_oaipmh_common_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       29 2023-07-21 02:16:00.000000 core_oaipmh_common_app-2.4.0/core_oaipmh_common_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-07-21 02:15:59.000000 core_oaipmh_common_app-2.4.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       21 2023-07-21 02:15:59.000000 core_oaipmh_common_app-2.4.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       42 2023-07-21 02:15:59.000000 core_oaipmh_common_app-2.4.0/requirements.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-07-21 02:16:01.384552 core_oaipmh_common_app-2.4.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1420 2023-07-21 02:15:59.000000 core_oaipmh_common_app-2.4.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:01.254290 core_oaipmh_common_app-2.4.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:15:59.000000 core_oaipmh_common_app-2.4.0/tests/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:01.265133 core_oaipmh_common_app-2.4.0/tests/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:15:59.000000 core_oaipmh_common_app-2.4.0/tests/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:01.300282 core_oaipmh_common_app-2.4.0/tests/components/oai_metadata_format/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:15:59.000000 core_oaipmh_common_app-2.4.0/tests/components/oai_metadata_format/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6179 2023-07-21 02:15:59.000000 core_oaipmh_common_app-2.4.0/tests/components/oai_metadata_format/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:01.319075 core_oaipmh_common_app-2.4.0/tests/components/oai_set/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:15:59.000000 core_oaipmh_common_app-2.4.0/tests/components/oai_set/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:01.346330 core_oaipmh_common_app-2.4.0/tests/components/oai_set/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:15:59.000000 core_oaipmh_common_app-2.4.0/tests/components/oai_set/tests/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4771 2023-07-21 02:15:59.000000 core_oaipmh_common_app-2.4.0/tests/components/oai_set/tests/tests_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1510 2023-07-21 02:15:59.000000 core_oaipmh_common_app-2.4.0/tests/test_settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:01.370400 core_oaipmh_common_app-2.4.0/tests/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:15:59.000000 core_oaipmh_common_app-2.4.0/tests/utils/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1389 2023-07-21 02:15:59.000000 core_oaipmh_common_app-2.4.0/tests/utils/tests_iso8601_operation.py
```

### Comparing `core_oaipmh_common_app-2.3.0/LICENSE.md` & `core_oaipmh_common_app-2.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_oaipmh_common_app-2.3.0/PKG-INFO` & `core_oaipmh_common_app-2.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_oaipmh_common_app
-Version: 2.3.0
+Version: 2.4.0
 Summary: Base OAI-PMH functions for the curator core project
 Home-page: https://github.com/usnistgov/core_oaipmh_common_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: ======================
         Core Oaipmh Common App
```

### Comparing `core_oaipmh_common_app-2.3.0/README.rst` & `core_oaipmh_common_app-2.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_oaipmh_common_app-2.3.0/core_oaipmh_common_app/commons/exceptions.py` & `core_oaipmh_common_app-2.4.0/core_oaipmh_common_app/commons/exceptions.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_common_app-2.3.0/core_oaipmh_common_app/commons/messages.py` & `core_oaipmh_common_app-2.4.0/core_oaipmh_common_app/commons/messages.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_common_app-2.3.0/core_oaipmh_common_app/components/oai_metadata_format/api.py` & `core_oaipmh_common_app-2.4.0/core_oaipmh_common_app/components/oai_metadata_format/api.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_common_app-2.3.0/core_oaipmh_common_app/components/oai_metadata_format/models.py` & `core_oaipmh_common_app-2.4.0/core_oaipmh_common_app/components/oai_metadata_format/models.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_common_app-2.3.0/core_oaipmh_common_app/components/oai_set/api.py` & `core_oaipmh_common_app-2.4.0/core_oaipmh_common_app/components/oai_set/api.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_common_app-2.3.0/core_oaipmh_common_app/components/oai_set/models.py` & `core_oaipmh_common_app-2.4.0/core_oaipmh_common_app/components/oai_set/models.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_common_app-2.3.0/core_oaipmh_common_app/utils/UTCdatetime.py` & `core_oaipmh_common_app-2.4.0/core_oaipmh_common_app/utils/UTCdatetime.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """ UTC datetime
 """
+import datetime
 
 import iso8601
 
 
 def datetime_to_utc_datetime_iso8601(datetime, day_granularity=False):
     """Convert a datetime into its iso8601 UTC date.
 
@@ -27,10 +28,11 @@
     """Convert an iso8601 UTC date into datetime.
 
     Parameters:
         utc_datetime: iso8601 UTC date to convert.
 
     Returns:
         Converted date (Datetime).
-
     """
-    return iso8601.parse_date(utc_datetime).replace(tzinfo=None)
+    return iso8601.parse_date(utc_datetime).replace(
+        tzinfo=datetime.timezone.utc
+    )
```

### Comparing `core_oaipmh_common_app-2.3.0/core_oaipmh_common_app.egg-info/PKG-INFO` & `core_oaipmh_common_app-2.4.0/core_oaipmh_common_app.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-oaipmh-common-app
-Version: 2.3.0
+Version: 2.4.0
 Summary: Base OAI-PMH functions for the curator core project
 Home-page: https://github.com/usnistgov/core_oaipmh_common_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: ======================
         Core Oaipmh Common App
```

### Comparing `core_oaipmh_common_app-2.3.0/core_oaipmh_common_app.egg-info/SOURCES.txt` & `core_oaipmh_common_app-2.4.0/core_oaipmh_common_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `core_oaipmh_common_app-2.3.0/setup.py` & `core_oaipmh_common_app-2.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_oaipmh_common_app",
-    version="2.3.0",
+    version="2.4.0",
     description="Base OAI-PMH functions for the curator core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_oaipmh_common_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_oaipmh_common_app-2.3.0/tests/components/oai_metadata_format/tests_unit.py` & `core_oaipmh_common_app-2.4.0/tests/components/oai_metadata_format/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_common_app-2.3.0/tests/components/oai_set/tests/tests_unit.py` & `core_oaipmh_common_app-2.4.0/tests/components/oai_set/tests/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_common_app-2.3.0/tests/test_settings.py` & `core_oaipmh_common_app-2.4.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_common_app-2.3.0/tests/utils/tests_iso8601_operation.py` & `core_oaipmh_common_app-2.4.0/tests/utils/tests_iso8601_operation.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,15 +31,20 @@
         # Arrange
         date_to_convert = "2016-11-18T08:30:00Z"
 
         # Act
         result = UTCdatetime.utc_datetime_iso8601_to_datetime(date_to_convert)
 
         # Assert
-        self.assertEqual(result, datetime.datetime(2016, 11, 18, 8, 30))
+        self.assertEqual(
+            result,
+            datetime.datetime(2016, 11, 18, 8, 30).replace(
+                tzinfo=datetime.timezone.utc
+            ),
+        )
 
     def test_invalid_conversion(self):
         """test_invalid_conversion"""
         # Arrange
         date_to_convert = "20166-11-18T08:30:00Z"
 
         # Act # Assert
```

