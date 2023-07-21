# Comparing `tmp/funding-service-design-utils-2.0.8.tar.gz` & `tmp/funding-service-design-utils-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funding-service-design-utils-2.0.8.tar", last modified: Fri Jun 30 10:27:47 2023, max compression
+gzip compressed data, was "funding-service-design-utils-2.0.9.tar", last modified: Mon Jul 10 09:40:16 2023, max compression
```

## Comparing `funding-service-design-utils-2.0.8.tar` & `funding-service-design-utils-2.0.9.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:27:47.457517 funding-service-design-utils-2.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17295 2023-06-30 10:27:47.457517 funding-service-design-utils-2.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15464 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:27:47.449517 funding-service-design-utils-2.0.8/fsd_test_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_test_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:27:47.449517 funding-service-design-utils-2.0.8/fsd_test_utils/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_test_utils/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_test_utils/fixtures/db_fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:27:47.449517 funding-service-design-utils-2.0.8/fsd_test_utils/test_config/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_test_utils/test_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_test_utils/test_config/useful_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:27:47.449517 funding-service-design-utils-2.0.8/fsd_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:27:47.449517 funding-service-design-utils-2.0.8/fsd_utils/authentication/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/authentication/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/authentication/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/authentication/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/authentication/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:27:47.449517 funding-service-design-utils-2.0.8/fsd_utils/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/config/commonconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/config/configclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/config/notify_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:27:47.449517 funding-service-design-utils-2.0.8/fsd_utils/gunicorn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/gunicorn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:27:47.449517 funding-service-design-utils-2.0.8/fsd_utils/gunicorn/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/gunicorn/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/gunicorn/config/devtest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7032 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/gunicorn/config/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:27:47.449517 funding-service-design-utils-2.0.8/fsd_utils/healthchecks/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/healthchecks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/healthchecks/checkers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/healthchecks/healthcheck.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:27:47.453517 funding-service-design-utils-2.0.8/fsd_utils/locale_selector/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/locale_selector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/locale_selector/get_lang.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/locale_selector/set_lang.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:27:47.453517 funding-service-design-utils-2.0.8/fsd_utils/logging/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/logging/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:27:47.453517 funding-service-design-utils-2.0.8/fsd_utils/mapping/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/mapping/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:27:47.453517 funding-service-design-utils-2.0.8/fsd_utils/mapping/application/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/mapping/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/mapping/application/application_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/mapping/application/free_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     5920 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/mapping/application/multi_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/mapping/application/qa_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:27:47.453517 funding-service-design-utils-2.0.8/fsd_utils/sentry/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/sentry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/sentry/init_sentry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:27:47.453517 funding-service-design-utils-2.0.8/fsd_utils/simple_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/simple_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/simple_utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/simple_utils/date_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:27:47.457517 funding-service-design-utils-2.0.8/fsd_utils/toggles/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/toggles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/fsd_utils/toggles/toggles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:27:47.457517 funding-service-design-utils-2.0.8/funding_service_design_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17295 2023-06-30 10:27:47.000000 funding-service-design-utils-2.0.8/funding_service_design_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-30 10:27:47.000000 funding-service-design-utils-2.0.8/funding_service_design_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 10:27:47.000000 funding-service-design-utils-2.0.8/funding_service_design_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-30 10:27:47.000000 funding-service-design-utils-2.0.8/funding_service_design_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-30 10:27:47.000000 funding-service-design-utils-2.0.8/funding_service_design_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 10:27:47.457517 funding-service-design-utils-2.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:27:47.457517 funding-service-design-utils-2.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8717 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/tests/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/tests/test_checkers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/tests/test_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/tests/test_get_lang.py
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/tests/test_healthcheck.py
--rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/tests/test_mapping_application.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/tests/test_set_lang.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-30 10:27:34.000000 funding-service-design-utils-2.0.8/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:40:16.137238 funding-service-design-utils-2.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-10 09:40:02.000000 funding-service-design-utils-2.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17295 2023-07-10 09:40:16.133237 funding-service-design-utils-2.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15464 2023-07-10 09:40:02.000000 funding-service-design-utils-2.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:40:16.125237 funding-service-design-utils-2.0.9/fsd_test_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-10 09:40:02.000000 funding-service-design-utils-2.0.9/fsd_test_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:40:16.125237 funding-service-design-utils-2.0.9/fsd_test_utils/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-10 09:40:02.000000 funding-service-design-utils-2.0.9/fsd_test_utils/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-07-10 09:40:02.000000 funding-service-design-utils-2.0.9/fsd_test_utils/fixtures/db_fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:40:16.125237 funding-service-design-utils-2.0.9/fsd_test_utils/test_config/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-10 09:40:02.000000 funding-service-design-utils-2.0.9/fsd_test_utils/test_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-10 09:40:02.000000 funding-service-design-utils-2.0.9/fsd_test_utils/test_config/useful_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:40:16.125237 funding-service-design-utils-2.0.9/fsd_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-10 09:40:02.000000 funding-service-design-utils-2.0.9/fsd_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:40:16.125237 funding-service-design-utils-2.0.9/fsd_utils/authentication/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 09:40:02.000000 funding-service-design-utils-2.0.9/fsd_utils/authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-10 09:40:02.000000 funding-service-design-utils-2.0.9/fsd_utils/authentication/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-07-10 09:40:02.000000 funding-service-design-utils-2.0.9/fsd_utils/authentication/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-10 09:40:02.000000 funding-service-design-utils-2.0.9/fsd_utils/authentication/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-10 09:40:02.000000 funding-service-design-utils-2.0.9/fsd_utils/authentication/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:40:16.129237 funding-service-design-utils-2.0.9/fsd_utils/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 09:40:02.000000 funding-service-design-utils-2.0.9/fsd_utils/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-07-10 09:40:02.000000 funding-service-design-utils-2.0.9/fsd_utils/config/commonconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-10 09:40:02.000000 funding-service-design-utils-2.0.9/fsd_utils/config/configclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-10 09:40:02.000000 funding-service-design-utils-2.0.9/fsd_utils/config/notify_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:40:16.129237 funding-service-design-utils-2.0.9/fsd_utils/gunicorn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 09:40:02.000000 funding-service-design-utils-2.0.9/fsd_utils/gunicorn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:40:16.129237 funding-service-design-utils-2.0.9/fsd_utils/gunicorn/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 09:40:02.000000 funding-service-design-utils-2.0.9/fsd_utils/gunicorn/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-07-10 09:40:02.000000 funding-service-design-utils-2.0.9/fsd_utils/gunicorn/config/devtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7032 2023-07-10 09:40:02.000000 funding-service-design-utils-2.0.9/fsd_utils/gunicorn/config/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:40:16.129237 funding-service-design-utils-2.0.9/fsd_utils/healthchecks/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-10 09:40:02.000000 funding-service-design-utils-2.0.9/fsd_utils/healthchecks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-10 09:40:02.000000 funding-service-design-utils-2.0.9/fsd_utils/healthchecks/checkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-10 09:40:02.000000 funding-service-design-utils-2.0.9/fsd_utils/healthchecks/healthcheck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:40:16.129237 funding-service-design-utils-2.0.9/fsd_utils/locale_selector/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-10 09:40:02.000000 funding-service-design-utils-2.0.9/fsd_utils/locale_selector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-10 09:40:02.000000 funding-service-design-utils-2.0.9/fsd_utils/locale_selector/get_lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-10 09:40:02.000000 funding-service-design-utils-2.0.9/fsd_utils/locale_selector/set_lang.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:40:16.129237 funding-service-design-utils-2.0.9/fsd_utils/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-10 09:40:02.000000 funding-service-design-utils-2.0.9/fsd_utils/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-07-10 09:40:02.000000 funding-service-design-utils-2.0.9/fsd_utils/logging/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:40:16.129237 funding-service-design-utils-2.0.9/fsd_utils/mapping/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 09:40:02.000000 funding-service-design-utils-2.0.9/fsd_utils/mapping/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:40:16.129237 funding-service-design-utils-2.0.9/fsd_utils/mapping/application/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 09:40:02.000000 funding-service-design-utils-2.0.9/fsd_utils/mapping/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-07-10 09:40:02.000000 funding-service-design-utils-2.0.9/fsd_utils/mapping/application/application_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-10 09:40:02.000000 funding-service-design-utils-2.0.9/fsd_utils/mapping/application/free_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-07-10 09:40:02.000000 funding-service-design-utils-2.0.9/fsd_utils/mapping/application/multi_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-07-10 09:40:02.000000 funding-service-design-utils-2.0.9/fsd_utils/mapping/application/qa_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:40:16.129237 funding-service-design-utils-2.0.9/fsd_utils/sentry/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 09:40:02.000000 funding-service-design-utils-2.0.9/fsd_utils/sentry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-10 09:40:02.000000 funding-service-design-utils-2.0.9/fsd_utils/sentry/init_sentry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:40:16.133237 funding-service-design-utils-2.0.9/fsd_utils/simple_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 09:40:02.000000 funding-service-design-utils-2.0.9/fsd_utils/simple_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-10 09:40:02.000000 funding-service-design-utils-2.0.9/fsd_utils/simple_utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-10 09:40:02.000000 funding-service-design-utils-2.0.9/fsd_utils/simple_utils/date_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:40:16.133237 funding-service-design-utils-2.0.9/fsd_utils/toggles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 09:40:02.000000 funding-service-design-utils-2.0.9/fsd_utils/toggles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-10 09:40:02.000000 funding-service-design-utils-2.0.9/fsd_utils/toggles/toggles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:40:16.133237 funding-service-design-utils-2.0.9/funding_service_design_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17295 2023-07-10 09:40:16.000000 funding-service-design-utils-2.0.9/funding_service_design_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-10 09:40:16.000000 funding-service-design-utils-2.0.9/funding_service_design_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 09:40:16.000000 funding-service-design-utils-2.0.9/funding_service_design_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-10 09:40:16.000000 funding-service-design-utils-2.0.9/funding_service_design_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-10 09:40:16.000000 funding-service-design-utils-2.0.9/funding_service_design_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-07-10 09:40:02.000000 funding-service-design-utils-2.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 09:40:16.137238 funding-service-design-utils-2.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-10 09:40:02.000000 funding-service-design-utils-2.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:40:16.133237 funding-service-design-utils-2.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 09:40:02.000000 funding-service-design-utils-2.0.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8717 2023-07-10 09:40:02.000000 funding-service-design-utils-2.0.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-07-10 09:40:02.000000 funding-service-design-utils-2.0.9/tests/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-07-10 09:40:02.000000 funding-service-design-utils-2.0.9/tests/test_checkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-07-10 09:40:02.000000 funding-service-design-utils-2.0.9/tests/test_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-10 09:40:02.000000 funding-service-design-utils-2.0.9/tests/test_get_lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-07-10 09:40:02.000000 funding-service-design-utils-2.0.9/tests/test_healthcheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6713 2023-07-10 09:40:02.000000 funding-service-design-utils-2.0.9/tests/test_mapping_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-10 09:40:02.000000 funding-service-design-utils-2.0.9/tests/test_set_lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-10 09:40:02.000000 funding-service-design-utils-2.0.9/tests/test_utils.py
```

### Comparing `funding-service-design-utils-2.0.8/LICENSE` & `funding-service-design-utils-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.8/PKG-INFO` & `funding-service-design-utils-2.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funding-service-design-utils
-Version: 2.0.8
+Version: 2.0.9
 Summary: Utilities used by the DLUHC Funding Service Design Team
 Author-email: DLUHC <FundingServiceDesignTeam@levellingup.gov.uk>
 License: MIT License
         
         Copyright (c) 2022 Crown Copyright (Department for Levelling Up, Housing and Communities)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `funding-service-design-utils-2.0.8/README.md` & `funding-service-design-utils-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.8/fsd_test_utils/fixtures/db_fixtures.py` & `funding-service-design-utils-2.0.9/fsd_test_utils/fixtures/db_fixtures.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.8/fsd_utils/__init__.py` & `funding-service-design-utils-2.0.9/fsd_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.8/fsd_utils/authentication/config.py` & `funding-service-design-utils-2.0.9/fsd_utils/authentication/config.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.8/fsd_utils/authentication/decorators.py` & `funding-service-design-utils-2.0.9/fsd_utils/authentication/decorators.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.8/fsd_utils/authentication/models.py` & `funding-service-design-utils-2.0.9/fsd_utils/authentication/models.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.8/fsd_utils/authentication/utils.py` & `funding-service-design-utils-2.0.9/fsd_utils/authentication/utils.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.8/fsd_utils/config/commonconfig.py` & `funding-service-design-utils-2.0.9/fsd_utils/config/commonconfig.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.8/fsd_utils/config/configclass.py` & `funding-service-design-utils-2.0.9/fsd_utils/config/configclass.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.8/fsd_utils/config/notify_constants.py` & `funding-service-design-utils-2.0.9/fsd_utils/config/notify_constants.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.8/fsd_utils/gunicorn/config/devtest.py` & `funding-service-design-utils-2.0.9/fsd_utils/gunicorn/config/devtest.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.8/fsd_utils/gunicorn/config/local.py` & `funding-service-design-utils-2.0.9/fsd_utils/gunicorn/config/local.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.8/fsd_utils/healthchecks/checkers.py` & `funding-service-design-utils-2.0.9/fsd_utils/healthchecks/checkers.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.8/fsd_utils/healthchecks/healthcheck.py` & `funding-service-design-utils-2.0.9/fsd_utils/healthchecks/healthcheck.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.8/fsd_utils/locale_selector/get_lang.py` & `funding-service-design-utils-2.0.9/fsd_utils/locale_selector/get_lang.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.8/fsd_utils/locale_selector/set_lang.py` & `funding-service-design-utils-2.0.9/fsd_utils/locale_selector/set_lang.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.8/fsd_utils/logging/logging.py` & `funding-service-design-utils-2.0.9/fsd_utils/logging/logging.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.8/fsd_utils/mapping/application/application_utils.py` & `funding-service-design-utils-2.0.9/fsd_utils/mapping/application/application_utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import calendar
 import re
 from io import StringIO
 
 from flask import current_app
 
 
 def convert_bool_value(data):
@@ -36,20 +37,32 @@
     try:
         if answer is None:
             return "Not provided"
 
         if "null" in answer:
             return re.sub(r"\s*null\s*,?", "", answer)
 
+        if isinstance(answer, str):
+            if answer.startswith("http") or answer.startswith("https"):
+                return answer
+            elif "-" in answer:
+                return answer.replace("-", " ")
+
         if isinstance(answer, list):
-            return [a.replace("'", "") for a in answer if isinstance(a, str)]
+            return [
+                a.replace("'", "").replace("-", " ")
+                if isinstance(a, str) and "-" in a
+                else a
+                for a in answer
+            ]
+        else:
 
-        return answer
+            return answer
     except Exception as e:
-        current_app.logger.error(f"Could not format the answer, {e}")
+        current_app.logger.error(f"Could not format the answer: {e}")
 
 
 def simplify_title(section_name, remove_text: list):
     try:
         section = section_name.split("-")
         simplified_title = []
 
@@ -66,15 +79,15 @@
         current_app.logger.error(f"Could not simplify the section title, {e}")
 
 
 def format_checkbox(answer):
     formatted_elements = []
     indent = " " * 5
     for index, element in enumerate(answer, start=1):
-        separator = f"{indent}-" if index > 1 else "-"
+        separator = f"{indent}." if index > 1 else "."
         if "-" in element:
             sub_elements = element.split("-")
             formatted_sub_elements = " ".join(sub_elements).strip()
             formatted_elements.append(f"{separator} {formatted_sub_elements}")
         else:
             formatted_elements.append(f"{separator} {element}")
 
@@ -87,9 +100,22 @@
     output.write(f"********* {fund_name} **********\n")
 
     for section_name, values in q_and_a.items():
         title = simplify_title(section_name, remove_text=["cof", "ns"])
         output.write(f"\n* {' '.join(title).capitalize()}\n\n")
         for questions, answers in values.items():
             output.write(f"  Q) {questions}\n")
-            output.write(f"  A) {answers}\n\n")
+            output.write(f"  A) {format_answer(answers)}\n\n")
     return output.getvalue()
+
+
+def number_to_month(number, iso_key):
+    """Converts a month number to its corresponding month name."""
+    try:
+        if iso_key == "month":
+            month_name = calendar.month_name[number]
+            return month_name
+        else:
+            return number
+    except IndexError:
+        current_app.logger.warn("Invalid month number")
+        return number
```

### Comparing `funding-service-design-utils-2.0.8/fsd_utils/mapping/application/free_text.py` & `funding-service-design-utils-2.0.9/fsd_utils/mapping/application/free_text.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.8/fsd_utils/mapping/application/multi_input.py` & `funding-service-design-utils-2.0.9/fsd_utils/mapping/application/multi_input.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 import uuid
 
 from flask import current_app
 from fsd_utils.mapping.application.application_utils import convert_bool_value
+from fsd_utils.mapping.application.application_utils import number_to_month
 
 
 class MultiInput:
     indent = " " * 5
 
     @classmethod
     def format_values(cls, value, index):
@@ -14,15 +15,15 @@
         Format the given value based on the specified conditions.
         Args:
             value: The value to be formatted.
             index: The index of the value in the processing sequence.
         Returns:
             str: The formatted string representation of the value.
         """
-        return f"{cls.indent}- {value}" if index != 1 else f"- {value}"
+        return f"{cls.indent}. {value}" if index != 1 else f". {value}"
 
     @classmethod
     def format_keys_and_values(cls, key, value, index):
 
         """
         Format the given key-value pair based on specified conditions.
         Args:
@@ -44,58 +45,66 @@
                     )
                 )
                 if isinstance(value, list)
                 else convert_bool_value(value)
             )
 
         return (
-            f"{cls.indent}- {key}: {formatted_values(value)}"  # noqa
+            f"{cls.indent}. {key}: {formatted_values(value)}"  # noqa
             if index != 1
-            else (f"- {key}: {formatted_values(value)}")  # noqa
+            else (f". {key}: {formatted_values(value)}")  # noqa
         )
 
     @classmethod
     def format_nested_data(cls, value):
+        """
+        Formats nested data based on specific keys and data and returns the formatted result.
+        Args:
+            value: A nested data structure to be processed and formatted.
 
-        formatted_nested_values = []
-        for inner_items in value:
+        Returns:
+            str: The formatted result obtained from the nested data.
+        """
 
-            for k, v in inner_items.items():
-                for iso_keys in ["date", "month", "year"]:
-                    try:
+        formatted_nested_values = []
+        try:
+            for inner_items in value:
+                for k, v in inner_items.items():
+                    for iso_keys in ["date", "month", "year"]:
                         if iso_keys in k.split("__"):
-                            formatted_nested_values.append(f"{iso_keys}: {v}")
+                            v = number_to_month(v, iso_keys)
+                            formatted_nested_values.append(f"{v}")
                             break
 
                     # handles all other nested multiple values
-                    except:  # noqa
-                        formatted_nested_values.append(
-                            ", ".join(
-                                map(
-                                    lambda item: ", ".join(
-                                        [f"{k}: {v}" for k, v in item.items()]
-                                    ),
-                                    value,
-                                )
-                            )
-                        )
-        return formatted_nested_values
+        except:  # noqa
+            formatted_nested_values.append(
+                ", ".join(
+                    map(
+                        lambda item: ", ".join([f"{k}: {v}" for k, v in item.items()]),
+                        value,
+                    )
+                )
+            )
+        return " ".join(formatted_nested_values)
 
     @classmethod
     def process_data(cls, data):
         """
         Process the data dictionary and generate a formatted output list.
         Args:
             data (dict): The dictionary to be processed.
         Returns:
             list: The formatted output list generated from the data.
         """
         output = []
 
         for index, (key, value) in enumerate(data.items(), start=1):
+            if isinstance(key, int):
+                key = str(key)
 
             # handles single value/answer containing uuid and excludes uuid key
             # & display the value only.
             try:
                 if isinstance(key, str) and uuid.UUID(key, version=4):
                     output.append(cls.format_values(value, index))
 
@@ -104,17 +113,17 @@
                 if (
                     isinstance(value, list)
                     and len(value) > 0
                     and isinstance(value[0], dict)
                 ):
                     formatted_nested_values = cls.format_nested_data(value)
                     output.append(
-                        f"{cls.indent}- {key}: {formatted_nested_values}"
+                        f"{cls.indent}. {key}: {formatted_nested_values}"
                         if index != 1
-                        else f"- {key}: {formatted_nested_values}"
+                        else f". {key}: {formatted_nested_values}"
                     )
                 # handles all other multiple values
                 else:
                     output.append(cls.format_keys_and_values(key, value, index))
 
         return output
```

### Comparing `funding-service-design-utils-2.0.8/fsd_utils/mapping/application/qa_mapping.py` & `funding-service-design-utils-2.0.9/fsd_utils/mapping/application/qa_mapping.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.8/fsd_utils/sentry/init_sentry.py` & `funding-service-design-utils-2.0.9/fsd_utils/sentry/init_sentry.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.8/fsd_utils/simple_utils/date_utils.py` & `funding-service-design-utils-2.0.9/fsd_utils/simple_utils/date_utils.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.8/fsd_utils/toggles/toggles.py` & `funding-service-design-utils-2.0.9/fsd_utils/toggles/toggles.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.8/funding_service_design_utils.egg-info/PKG-INFO` & `funding-service-design-utils-2.0.9/funding_service_design_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funding-service-design-utils
-Version: 2.0.8
+Version: 2.0.9
 Summary: Utilities used by the DLUHC Funding Service Design Team
 Author-email: DLUHC <FundingServiceDesignTeam@levellingup.gov.uk>
 License: MIT License
         
         Copyright (c) 2022 Crown Copyright (Department for Levelling Up, Housing and Communities)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `funding-service-design-utils-2.0.8/funding_service_design_utils.egg-info/SOURCES.txt` & `funding-service-design-utils-2.0.9/funding_service_design_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.8/pyproject.toml` & `funding-service-design-utils-2.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "funding-service-design-utils"
-version = "2.0.8"
+version = "2.0.9"
 authors = [
   { name="DLUHC", email="FundingServiceDesignTeam@levellingup.gov.uk" },
 ]
 description = "Utilities used by the DLUHC Funding Service Design Team"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.10,<4.0"
```

### Comparing `funding-service-design-utils-2.0.8/tests/conftest.py` & `funding-service-design-utils-2.0.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.8/tests/test_authentication.py` & `funding-service-design-utils-2.0.9/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.8/tests/test_checkers.py` & `funding-service-design-utils-2.0.9/tests/test_checkers.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.8/tests/test_get_lang.py` & `funding-service-design-utils-2.0.9/tests/test_get_lang.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.8/tests/test_healthcheck.py` & `funding-service-design-utils-2.0.9/tests/test_healthcheck.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.8/tests/test_mapping_application.py` & `funding-service-design-utils-2.0.9/tests/test_mapping_application.py`

 * *Files 13% similar despite different names*

```diff
@@ -28,14 +28,25 @@
 
 
 @pytest.mark.parametrize(
     "input_data, expected_response",
     [
         ("null", ""),
         (None, "Not provided"),
+        (
+            "555 dummy road, null, beautiful town, optional county, UU8 8UU",
+            "555 dummy road, beautiful town, optional county, UU8 8UU",
+        ),
+        ("https://example.com/test-the-link", "https://example.com/test-the-link"),
+        (["one-two-three"], ["one two three"]),
+        (["four five six"], ["four five six"]),
+        ("seven-eight-nine", "seven eight nine"),
+        ("seven-eight-nine", "seven eight nine"),
+        ("ten eleven twelve", "ten eleven twelve"),
+        ({"title": ["one-two-three"]}, {"title": ["one-two-three"]}),
     ],
 )
 def test_format_answer(input_data, expected_response):
     response = format_answer(input_data)
     assert response == expected_response
 
 
@@ -82,15 +93,14 @@
     assert response == expected_response
 
 
 def test_sort_questions_and_answers(app_context):
     forms = test_data_sort_questions_answers["forms"]
 
     response = extract_questions_and_answers(forms)
-
     assert response == test_data_sort_questions_answers["questions_answers"]
 
 
 def test_sort_questions_and_answers_fail(app_context):
     forms = test_data_sort_questions_answers["incorrect_form_data"]
 
     with pytest.raises(Exception) as exc:
@@ -103,19 +113,19 @@
     "input_value, expected_response",
     [
         (
             [
                 "health-interventions",
                 "employment-support",
             ],
-            "- health interventions\n     - employment support",
+            ". health interventions\n     . employment support",
         ),
         (
             ["Survivors of domestic abuse", "ethnic minorities"],
-            "- Survivors of domestic abuse\n     - ethnic minorities",
+            ". Survivors of domestic abuse\n     . ethnic minorities",
         ),
     ],
 )
 def test_format_checkbox(input_value, expected_response):
 
     response = format_checkbox(input_value)
     assert response == expected_response
```

### Comparing `funding-service-design-utils-2.0.8/tests/test_set_lang.py` & `funding-service-design-utils-2.0.9/tests/test_set_lang.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.8/tests/test_utils.py` & `funding-service-design-utils-2.0.9/tests/test_utils.py`

 * *Files identical despite different names*

