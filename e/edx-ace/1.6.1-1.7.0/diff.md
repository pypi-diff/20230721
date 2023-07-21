# Comparing `tmp/edx-ace-1.6.1.tar.gz` & `tmp/edx-ace-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-ace-1.6.1.tar", last modified: Thu Feb 16 14:37:23 2023, max compression
+gzip compressed data, was "edx-ace-1.7.0.tar", last modified: Fri Jul 21 14:17:04 2023, max compression
```

## Comparing `edx-ace-1.6.1.tar` & `edx-ace-1.7.0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-16 14:37:23.895431 edx-ace-1.6.1/
--rw-r--r--   0 runner    (1001) docker     (122)     3810 2023-02-16 14:37:21.000000 edx-ace-1.6.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    35138 2023-02-16 14:37:21.000000 edx-ace-1.6.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      202 2023-02-16 14:37:21.000000 edx-ace-1.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    11646 2023-02-16 14:37:23.895431 edx-ace-1.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4811 2023-02-16 14:37:21.000000 edx-ace-1.6.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-16 14:37:23.891431 edx-ace-1.6.1/edx_ace/
--rw-r--r--   0 runner    (1001) docker     (122)      684 2023-02-16 14:37:21.000000 edx-ace-1.6.1/edx_ace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1788 2023-02-16 14:37:21.000000 edx-ace-1.6.1/edx_ace/ace.py
--rw-r--r--   0 runner    (1001) docker     (122)      216 2023-02-16 14:37:21.000000 edx-ace-1.6.1/edx_ace/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-16 14:37:23.891431 edx-ace-1.6.1/edx_ace/channel/
--rw-r--r--   0 runner    (1001) docker     (122)     6713 2023-02-16 14:37:21.000000 edx-ace-1.6.1/edx_ace/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10240 2023-02-16 14:37:21.000000 edx-ace-1.6.1/edx_ace/channel/braze.py
--rw-r--r--   0 runner    (1001) docker     (122)     2133 2023-02-16 14:37:21.000000 edx-ace-1.6.1/edx_ace/channel/django_email.py
--rw-r--r--   0 runner    (1001) docker     (122)     3028 2023-02-16 14:37:21.000000 edx-ace-1.6.1/edx_ace/channel/file.py
--rw-r--r--   0 runner    (1001) docker     (122)     1313 2023-02-16 14:37:21.000000 edx-ace-1.6.1/edx_ace/channel/mixins.py
--rw-r--r--   0 runner    (1001) docker     (122)    12699 2023-02-16 14:37:21.000000 edx-ace-1.6.1/edx_ace/channel/sailthru.py
--rw-r--r--   0 runner    (1001) docker     (122)     2690 2023-02-16 14:37:21.000000 edx-ace-1.6.1/edx_ace/delivery.py
--rw-r--r--   0 runner    (1001) docker     (122)     1065 2023-02-16 14:37:21.000000 edx-ace-1.6.1/edx_ace/errors.py
--rw-r--r--   0 runner    (1001) docker     (122)     8182 2023-02-16 14:37:21.000000 edx-ace-1.6.1/edx_ace/message.py
--rw-r--r--   0 runner    (1001) docker     (122)      408 2023-02-16 14:37:21.000000 edx-ace-1.6.1/edx_ace/monitoring.py
--rw-r--r--   0 runner    (1001) docker     (122)     2915 2023-02-16 14:37:21.000000 edx-ace-1.6.1/edx_ace/policy.py
--rw-r--r--   0 runner    (1001) docker     (122)      778 2023-02-16 14:37:21.000000 edx-ace-1.6.1/edx_ace/presentation.py
--rw-r--r--   0 runner    (1001) docker     (122)      576 2023-02-16 14:37:21.000000 edx-ace-1.6.1/edx_ace/recipient.py
--rw-r--r--   0 runner    (1001) docker     (122)      959 2023-02-16 14:37:21.000000 edx-ace-1.6.1/edx_ace/recipient_resolver.py
--rw-r--r--   0 runner    (1001) docker     (122)     2764 2023-02-16 14:37:21.000000 edx-ace-1.6.1/edx_ace/renderers.py
--rw-r--r--   0 runner    (1001) docker     (122)     3775 2023-02-16 14:37:21.000000 edx-ace-1.6.1/edx_ace/serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-16 14:37:23.891431 edx-ace-1.6.1/edx_ace/templatetags/
--rw-r--r--   0 runner    (1001) docker     (122)      472 2023-02-16 14:37:21.000000 edx-ace-1.6.1/edx_ace/templatetags/acetags.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-16 14:37:23.891431 edx-ace-1.6.1/edx_ace/test_utils/
--rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-02-16 14:37:21.000000 edx-ace-1.6.1/edx_ace/test_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-16 14:37:23.891431 edx-ace-1.6.1/edx_ace/tests/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-16 14:37:23.895431 edx-ace-1.6.1/edx_ace/tests/channel/
--rw-r--r--   0 runner    (1001) docker     (122)     7296 2023-02-16 14:37:21.000000 edx-ace-1.6.1/edx_ace/tests/channel/test_braze.py
--rw-r--r--   0 runner    (1001) docker     (122)     2891 2023-02-16 14:37:21.000000 edx-ace-1.6.1/edx_ace/tests/channel/test_channel_helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)     4114 2023-02-16 14:37:21.000000 edx-ace-1.6.1/edx_ace/tests/channel/test_django_email.py
--rw-r--r--   0 runner    (1001) docker     (122)     1795 2023-02-16 14:37:21.000000 edx-ace-1.6.1/edx_ace/tests/channel/test_file_email.py
--rw-r--r--   0 runner    (1001) docker     (122)     3197 2023-02-16 14:37:21.000000 edx-ace-1.6.1/edx_ace/tests/channel/test_sailthru.py
--rw-r--r--   0 runner    (1001) docker     (122)     2044 2023-02-16 14:37:21.000000 edx-ace-1.6.1/edx_ace/tests/test_ace.py
--rw-r--r--   0 runner    (1001) docker     (122)      639 2023-02-16 14:37:21.000000 edx-ace-1.6.1/edx_ace/tests/test_date.py
--rw-r--r--   0 runner    (1001) docker     (122)     4850 2023-02-16 14:37:21.000000 edx-ace-1.6.1/edx_ace/tests/test_delivery.py
--rw-r--r--   0 runner    (1001) docker     (122)     4430 2023-02-16 14:37:21.000000 edx-ace-1.6.1/edx_ace/tests/test_message.py
--rw-r--r--   0 runner    (1001) docker     (122)     1597 2023-02-16 14:37:21.000000 edx-ace-1.6.1/edx_ace/tests/test_policy.py
--rw-r--r--   0 runner    (1001) docker     (122)      572 2023-02-16 14:37:21.000000 edx-ace-1.6.1/edx_ace/tests/test_presentation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-16 14:37:23.887431 edx-ace-1.6.1/edx_ace/tests/test_templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-16 14:37:23.887431 edx-ace-1.6.1/edx_ace/tests/test_templates/testapp/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-16 14:37:23.887431 edx-ace-1.6.1/edx_ace/tests/test_templates/testapp/edx_ace/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-16 14:37:23.887431 edx-ace-1.6.1/edx_ace/tests/test_templates/testapp/edx_ace/testmessage/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-16 14:37:23.895431 edx-ace-1.6.1/edx_ace/tests/test_templates/testapp/edx_ace/testmessage/email/
--rw-r--r--   0 runner    (1001) docker     (122)      646 2023-02-16 14:37:21.000000 edx-ace-1.6.1/edx_ace/tests/test_templates/testapp/edx_ace/testmessage/email/body.html
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-02-16 14:37:21.000000 edx-ace-1.6.1/edx_ace/tests/test_templates/testapp/edx_ace/testmessage/email/head.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-16 14:37:23.895431 edx-ace-1.6.1/edx_ace/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-16 14:37:21.000000 edx-ace-1.6.1/edx_ace/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1483 2023-02-16 14:37:21.000000 edx-ace-1.6.1/edx_ace/utils/date.py
--rw-r--r--   0 runner    (1001) docker     (122)     2024 2023-02-16 14:37:21.000000 edx-ace-1.6.1/edx_ace/utils/once.py
--rw-r--r--   0 runner    (1001) docker     (122)     2090 2023-02-16 14:37:21.000000 edx-ace-1.6.1/edx_ace/utils/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-16 14:37:23.891431 edx-ace-1.6.1/edx_ace.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    11646 2023-02-16 14:37:23.000000 edx-ace-1.6.1/edx_ace.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1454 2023-02-16 14:37:23.000000 edx-ace-1.6.1/edx_ace.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-16 14:37:23.000000 edx-ace-1.6.1/edx_ace.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      254 2023-02-16 14:37:23.000000 edx-ace-1.6.1/edx_ace.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-16 14:37:23.000000 edx-ace-1.6.1/edx_ace.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      124 2023-02-16 14:37:23.000000 edx-ace-1.6.1/edx_ace.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-02-16 14:37:23.000000 edx-ace-1.6.1/edx_ace.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-16 14:37:23.895431 edx-ace-1.6.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      299 2023-02-16 14:37:21.000000 edx-ace-1.6.1/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-02-16 14:37:21.000000 edx-ace-1.6.1/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      435 2023-02-16 14:37:23.895431 edx-ace-1.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     5638 2023-02-16 14:37:21.000000 edx-ace-1.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 14:17:04.861420 edx-ace-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     3978 2023-07-21 14:17:02.000000 edx-ace-1.7.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35138 2023-07-21 14:17:02.000000 edx-ace-1.7.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      202 2023-07-21 14:17:02.000000 edx-ace-1.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    11820 2023-07-21 14:17:04.861420 edx-ace-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4811 2023-07-21 14:17:02.000000 edx-ace-1.7.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 14:17:04.853420 edx-ace-1.7.0/edx_ace/
+-rw-r--r--   0 runner    (1001) docker     (122)      635 2023-07-21 14:17:02.000000 edx-ace-1.7.0/edx_ace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1788 2023-07-21 14:17:02.000000 edx-ace-1.7.0/edx_ace/ace.py
+-rw-r--r--   0 runner    (1001) docker     (122)      216 2023-07-21 14:17:02.000000 edx-ace-1.7.0/edx_ace/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 14:17:04.857420 edx-ace-1.7.0/edx_ace/channel/
+-rw-r--r--   0 runner    (1001) docker     (122)     6713 2023-07-21 14:17:02.000000 edx-ace-1.7.0/edx_ace/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10240 2023-07-21 14:17:02.000000 edx-ace-1.7.0/edx_ace/channel/braze.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2133 2023-07-21 14:17:02.000000 edx-ace-1.7.0/edx_ace/channel/django_email.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3028 2023-07-21 14:17:02.000000 edx-ace-1.7.0/edx_ace/channel/file.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1313 2023-07-21 14:17:02.000000 edx-ace-1.7.0/edx_ace/channel/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12699 2023-07-21 14:17:02.000000 edx-ace-1.7.0/edx_ace/channel/sailthru.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2690 2023-07-21 14:17:02.000000 edx-ace-1.7.0/edx_ace/delivery.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1065 2023-07-21 14:17:02.000000 edx-ace-1.7.0/edx_ace/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8182 2023-07-21 14:17:02.000000 edx-ace-1.7.0/edx_ace/message.py
+-rw-r--r--   0 runner    (1001) docker     (122)      408 2023-07-21 14:17:02.000000 edx-ace-1.7.0/edx_ace/monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2915 2023-07-21 14:17:02.000000 edx-ace-1.7.0/edx_ace/policy.py
+-rw-r--r--   0 runner    (1001) docker     (122)      778 2023-07-21 14:17:02.000000 edx-ace-1.7.0/edx_ace/presentation.py
+-rw-r--r--   0 runner    (1001) docker     (122)      576 2023-07-21 14:17:02.000000 edx-ace-1.7.0/edx_ace/recipient.py
+-rw-r--r--   0 runner    (1001) docker     (122)      959 2023-07-21 14:17:02.000000 edx-ace-1.7.0/edx_ace/recipient_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2764 2023-07-21 14:17:02.000000 edx-ace-1.7.0/edx_ace/renderers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3775 2023-07-21 14:17:02.000000 edx-ace-1.7.0/edx_ace/serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 14:17:04.857420 edx-ace-1.7.0/edx_ace/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (122)      472 2023-07-21 14:17:02.000000 edx-ace-1.7.0/edx_ace/templatetags/acetags.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 14:17:04.857420 edx-ace-1.7.0/edx_ace/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-07-21 14:17:02.000000 edx-ace-1.7.0/edx_ace/test_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 14:17:04.857420 edx-ace-1.7.0/edx_ace/tests/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 14:17:04.857420 edx-ace-1.7.0/edx_ace/tests/channel/
+-rw-r--r--   0 runner    (1001) docker     (122)     7296 2023-07-21 14:17:02.000000 edx-ace-1.7.0/edx_ace/tests/channel/test_braze.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2891 2023-07-21 14:17:02.000000 edx-ace-1.7.0/edx_ace/tests/channel/test_channel_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4114 2023-07-21 14:17:02.000000 edx-ace-1.7.0/edx_ace/tests/channel/test_django_email.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1795 2023-07-21 14:17:02.000000 edx-ace-1.7.0/edx_ace/tests/channel/test_file_email.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3197 2023-07-21 14:17:02.000000 edx-ace-1.7.0/edx_ace/tests/channel/test_sailthru.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2044 2023-07-21 14:17:02.000000 edx-ace-1.7.0/edx_ace/tests/test_ace.py
+-rw-r--r--   0 runner    (1001) docker     (122)      639 2023-07-21 14:17:02.000000 edx-ace-1.7.0/edx_ace/tests/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4850 2023-07-21 14:17:02.000000 edx-ace-1.7.0/edx_ace/tests/test_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4430 2023-07-21 14:17:02.000000 edx-ace-1.7.0/edx_ace/tests/test_message.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1597 2023-07-21 14:17:02.000000 edx-ace-1.7.0/edx_ace/tests/test_policy.py
+-rw-r--r--   0 runner    (1001) docker     (122)      572 2023-07-21 14:17:02.000000 edx-ace-1.7.0/edx_ace/tests/test_presentation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 14:17:04.853420 edx-ace-1.7.0/edx_ace/tests/test_templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 14:17:04.853420 edx-ace-1.7.0/edx_ace/tests/test_templates/testapp/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 14:17:04.853420 edx-ace-1.7.0/edx_ace/tests/test_templates/testapp/edx_ace/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 14:17:04.853420 edx-ace-1.7.0/edx_ace/tests/test_templates/testapp/edx_ace/testmessage/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 14:17:04.857420 edx-ace-1.7.0/edx_ace/tests/test_templates/testapp/edx_ace/testmessage/email/
+-rw-r--r--   0 runner    (1001) docker     (122)      646 2023-07-21 14:17:02.000000 edx-ace-1.7.0/edx_ace/tests/test_templates/testapp/edx_ace/testmessage/email/body.html
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-07-21 14:17:02.000000 edx-ace-1.7.0/edx_ace/tests/test_templates/testapp/edx_ace/testmessage/email/head.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 14:17:04.861420 edx-ace-1.7.0/edx_ace/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-21 14:17:02.000000 edx-ace-1.7.0/edx_ace/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1483 2023-07-21 14:17:02.000000 edx-ace-1.7.0/edx_ace/utils/date.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2024 2023-07-21 14:17:02.000000 edx-ace-1.7.0/edx_ace/utils/once.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2090 2023-07-21 14:17:02.000000 edx-ace-1.7.0/edx_ace/utils/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 14:17:04.857420 edx-ace-1.7.0/edx_ace.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    11820 2023-07-21 14:17:04.000000 edx-ace-1.7.0/edx_ace.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1454 2023-07-21 14:17:04.000000 edx-ace-1.7.0/edx_ace.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-21 14:17:04.000000 edx-ace-1.7.0/edx_ace.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      254 2023-07-21 14:17:04.000000 edx-ace-1.7.0/edx_ace.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-21 14:17:04.000000 edx-ace-1.7.0/edx_ace.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      124 2023-07-21 14:17:04.000000 edx-ace-1.7.0/edx_ace.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-07-21 14:17:04.000000 edx-ace-1.7.0/edx_ace.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 14:17:04.861420 edx-ace-1.7.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      299 2023-07-21 14:17:02.000000 edx-ace-1.7.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-07-21 14:17:02.000000 edx-ace-1.7.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      435 2023-07-21 14:17:04.861420 edx-ace-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     5589 2023-07-21 14:17:02.000000 edx-ace-1.7.0/setup.py
```

### Comparing `edx-ace-1.6.1/CHANGELOG.rst` & `edx-ace-1.7.0/CHANGELOG.rst`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,21 @@
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
+[1.7.0] - 2023-07-21
+~~~~~~~~~~~~~~~~~~~~
+
+* Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
+  deprecated
+* Added support for django 4.2
+
 [1.6.1] - 2023-02-07
 ~~~~~~~~~~~~~~~~~~~~
 
 * Updated code coverage target in https://github.com/openedx/edx-ace/pull/189
 * Updated Python Requirements in https://github.com/openedx/edx-ace/pull/199
 * **Full Changelog**: https://github.com/openedx/edx-ace/compare/v1.6.0...v1.6.1
```

### Comparing `edx-ace-1.6.1/LICENSE.txt` & `edx-ace-1.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx-ace-1.6.1/PKG-INFO` & `edx-ace-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-ace
-Version: 1.6.1
+Version: 1.7.0
 Summary: Framework for Messaging
 Home-page: https://github.com/openedx/edx-ace
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Description: edX Automated Communication Engine (A.C.E.)
         ###########################################
@@ -153,14 +153,21 @@
            This project adheres to Semantic Versioning (http://semver.org/).
         
         .. There should always be an "Unreleased" section for changes pending release.
         
         Unreleased
         ~~~~~~~~~~
         
+        [1.7.0] - 2023-07-21
+        ~~~~~~~~~~~~~~~~~~~~
+        
+        * Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
+          deprecated
+        * Added support for django 4.2
+        
         [1.6.1] - 2023-02-07
         ~~~~~~~~~~~~~~~~~~~~
         
         * Updated code coverage target in https://github.com/openedx/edx-ace/pull/189
         * Updated Python Requirements in https://github.com/openedx/edx-ace/pull/199
         * **Full Changelog**: https://github.com/openedx/edx-ace/compare/v1.6.0...v1.6.1
         
@@ -288,16 +295,15 @@
         * First release on PyPI.
         
 Keywords: Django edx
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: sailthru
```

### Comparing `edx-ace-1.6.1/README.rst` & `edx-ace-1.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `edx-ace-1.6.1/edx_ace/__init__.py` & `edx-ace-1.7.0/edx_ace/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,17 +9,16 @@
 from .ace import send
 from .channel import Channel, ChannelType
 from .message import Message, MessageType
 from .policy import Policy, PolicyResult
 from .recipient import Recipient
 from .recipient_resolver import RecipientResolver
 
-__version__ = '1.6.1'
+__version__ = '1.7.0'
 
-default_app_config = 'edx_ace.apps.EdxAceConfig'
 
 __all__ = [
     'send',
     '__version__',
     'Message',
     'MessageType',
     'Recipient',
```

### Comparing `edx-ace-1.6.1/edx_ace/ace.py` & `edx-ace-1.7.0/edx_ace/ace.py`

 * *Files identical despite different names*

### Comparing `edx-ace-1.6.1/edx_ace/channel/__init__.py` & `edx-ace-1.7.0/edx_ace/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-ace-1.6.1/edx_ace/channel/braze.py` & `edx-ace-1.7.0/edx_ace/channel/braze.py`

 * *Files identical despite different names*

### Comparing `edx-ace-1.6.1/edx_ace/channel/django_email.py` & `edx-ace-1.7.0/edx_ace/channel/django_email.py`

 * *Files identical despite different names*

### Comparing `edx-ace-1.6.1/edx_ace/channel/file.py` & `edx-ace-1.7.0/edx_ace/channel/file.py`

 * *Files identical despite different names*

### Comparing `edx-ace-1.6.1/edx_ace/channel/mixins.py` & `edx-ace-1.7.0/edx_ace/channel/mixins.py`

 * *Files identical despite different names*

### Comparing `edx-ace-1.6.1/edx_ace/channel/sailthru.py` & `edx-ace-1.7.0/edx_ace/channel/sailthru.py`

 * *Files identical despite different names*

### Comparing `edx-ace-1.6.1/edx_ace/delivery.py` & `edx-ace-1.7.0/edx_ace/delivery.py`

 * *Files identical despite different names*

### Comparing `edx-ace-1.6.1/edx_ace/errors.py` & `edx-ace-1.7.0/edx_ace/errors.py`

 * *Files identical despite different names*

### Comparing `edx-ace-1.6.1/edx_ace/message.py` & `edx-ace-1.7.0/edx_ace/message.py`

 * *Files identical despite different names*

### Comparing `edx-ace-1.6.1/edx_ace/policy.py` & `edx-ace-1.7.0/edx_ace/policy.py`

 * *Files identical despite different names*

### Comparing `edx-ace-1.6.1/edx_ace/presentation.py` & `edx-ace-1.7.0/edx_ace/presentation.py`

 * *Files identical despite different names*

### Comparing `edx-ace-1.6.1/edx_ace/recipient.py` & `edx-ace-1.7.0/edx_ace/recipient.py`

 * *Files identical despite different names*

### Comparing `edx-ace-1.6.1/edx_ace/recipient_resolver.py` & `edx-ace-1.7.0/edx_ace/recipient_resolver.py`

 * *Files identical despite different names*

### Comparing `edx-ace-1.6.1/edx_ace/renderers.py` & `edx-ace-1.7.0/edx_ace/renderers.py`

 * *Files identical despite different names*

### Comparing `edx-ace-1.6.1/edx_ace/serialization.py` & `edx-ace-1.7.0/edx_ace/serialization.py`

 * *Files identical despite different names*

### Comparing `edx-ace-1.6.1/edx_ace/test_utils/__init__.py` & `edx-ace-1.7.0/edx_ace/test_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-ace-1.6.1/edx_ace/tests/channel/test_braze.py` & `edx-ace-1.7.0/edx_ace/tests/channel/test_braze.py`

 * *Files identical despite different names*

### Comparing `edx-ace-1.6.1/edx_ace/tests/channel/test_channel_helpers.py` & `edx-ace-1.7.0/edx_ace/tests/channel/test_channel_helpers.py`

 * *Files identical despite different names*

### Comparing `edx-ace-1.6.1/edx_ace/tests/channel/test_django_email.py` & `edx-ace-1.7.0/edx_ace/tests/channel/test_django_email.py`

 * *Files identical despite different names*

### Comparing `edx-ace-1.6.1/edx_ace/tests/channel/test_file_email.py` & `edx-ace-1.7.0/edx_ace/tests/channel/test_file_email.py`

 * *Files identical despite different names*

### Comparing `edx-ace-1.6.1/edx_ace/tests/channel/test_sailthru.py` & `edx-ace-1.7.0/edx_ace/tests/channel/test_sailthru.py`

 * *Files identical despite different names*

### Comparing `edx-ace-1.6.1/edx_ace/tests/test_ace.py` & `edx-ace-1.7.0/edx_ace/tests/test_ace.py`

 * *Files identical despite different names*

### Comparing `edx-ace-1.6.1/edx_ace/tests/test_date.py` & `edx-ace-1.7.0/edx_ace/tests/test_date.py`

 * *Files identical despite different names*

### Comparing `edx-ace-1.6.1/edx_ace/tests/test_delivery.py` & `edx-ace-1.7.0/edx_ace/tests/test_delivery.py`

 * *Files identical despite different names*

### Comparing `edx-ace-1.6.1/edx_ace/tests/test_message.py` & `edx-ace-1.7.0/edx_ace/tests/test_message.py`

 * *Files identical despite different names*

### Comparing `edx-ace-1.6.1/edx_ace/tests/test_policy.py` & `edx-ace-1.7.0/edx_ace/tests/test_policy.py`

 * *Files identical despite different names*

### Comparing `edx-ace-1.6.1/edx_ace/tests/test_presentation.py` & `edx-ace-1.7.0/edx_ace/tests/test_presentation.py`

 * *Files identical despite different names*

### Comparing `edx-ace-1.6.1/edx_ace/tests/test_templates/testapp/edx_ace/testmessage/email/body.html` & `edx-ace-1.7.0/edx_ace/tests/test_templates/testapp/edx_ace/testmessage/email/body.html`

 * *Files identical despite different names*

### Comparing `edx-ace-1.6.1/edx_ace/utils/date.py` & `edx-ace-1.7.0/edx_ace/utils/date.py`

 * *Files identical despite different names*

### Comparing `edx-ace-1.6.1/edx_ace/utils/once.py` & `edx-ace-1.7.0/edx_ace/utils/once.py`

 * *Files identical despite different names*

### Comparing `edx-ace-1.6.1/edx_ace/utils/plugins.py` & `edx-ace-1.7.0/edx_ace/utils/plugins.py`

 * *Files identical despite different names*

### Comparing `edx-ace-1.6.1/edx_ace.egg-info/PKG-INFO` & `edx-ace-1.7.0/edx_ace.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-ace
-Version: 1.6.1
+Version: 1.7.0
 Summary: Framework for Messaging
 Home-page: https://github.com/openedx/edx-ace
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Description: edX Automated Communication Engine (A.C.E.)
         ###########################################
@@ -153,14 +153,21 @@
            This project adheres to Semantic Versioning (http://semver.org/).
         
         .. There should always be an "Unreleased" section for changes pending release.
         
         Unreleased
         ~~~~~~~~~~
         
+        [1.7.0] - 2023-07-21
+        ~~~~~~~~~~~~~~~~~~~~
+        
+        * Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
+          deprecated
+        * Added support for django 4.2
+        
         [1.6.1] - 2023-02-07
         ~~~~~~~~~~~~~~~~~~~~
         
         * Updated code coverage target in https://github.com/openedx/edx-ace/pull/189
         * Updated Python Requirements in https://github.com/openedx/edx-ace/pull/199
         * **Full Changelog**: https://github.com/openedx/edx-ace/compare/v1.6.0...v1.6.1
         
@@ -288,16 +295,15 @@
         * First release on PyPI.
         
 Keywords: Django edx
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: sailthru
```

### Comparing `edx-ace-1.6.1/edx_ace.egg-info/SOURCES.txt` & `edx-ace-1.7.0/edx_ace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx-ace-1.6.1/requirements/constraints.txt` & `edx-ace-1.7.0/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `edx-ace-1.6.1/setup.py` & `edx-ace-1.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,20 +117,19 @@
     license="AGPL 3.0",
     zip_safe=False,
     keywords='Django edx',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Framework :: Django',
         'Framework :: Django :: 3.2',
-        'Framework :: Django :: 4.0',
+        'Framework :: Django :: 4.2',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.8',
     ],
     entry_points={
         'openedx.ace.channel': [
             'braze_email = edx_ace.channel.braze:BrazeEmailChannel',
             'sailthru_email = edx_ace.channel.sailthru:SailthruEmailChannel',
             'file_email = edx_ace.channel.file:FileEmailChannel',
```

