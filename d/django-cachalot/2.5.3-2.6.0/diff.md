# Comparing `tmp/django-cachalot-2.5.3.tar.gz` & `tmp/django-cachalot-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-cachalot-2.5.3.tar", last modified: Mon Mar 13 09:16:11 2023, max compression
+gzip compressed data, was "django-cachalot-2.6.0.tar", last modified: Fri Jul 21 09:55:41 2023, max compression
```

## Comparing `django-cachalot-2.5.3.tar` & `django-cachalot-2.6.0.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 09:16:11.188505 django-cachalot-2.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)    13527 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-03-13 09:16:11.188505 django-cachalot-2.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6023 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 09:16:11.180504 django-cachalot-2.5.3/cachalot/
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/cachalot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 09:16:11.180504 django-cachalot-2.5.3/cachalot/admin_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/cachalot/admin_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/cachalot/admin_tests/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 09:16:11.180504 django-cachalot-2.5.3/cachalot/admin_tests/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/cachalot/admin_tests/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/cachalot/admin_tests/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/cachalot/admin_tests/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/cachalot/admin_tests/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/cachalot/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/cachalot/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/cachalot/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/cachalot/jinja2ext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 09:16:11.180504 django-cachalot-2.5.3/cachalot/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/cachalot/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 09:16:11.180504 django-cachalot-2.5.3/cachalot/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/cachalot/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/cachalot/management/commands/invalidate_cachalot.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/cachalot/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6888 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/cachalot/monkey_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/cachalot/panels.py
--rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/cachalot/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/cachalot/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 09:16:11.176504 django-cachalot-2.5.3/cachalot/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 09:16:11.180504 django-cachalot-2.5.3/cachalot/templates/cachalot/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/cachalot/templates/cachalot/panel.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 09:16:11.180504 django-cachalot-2.5.3/cachalot/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/cachalot/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/cachalot/templatetags/cachalot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 09:16:11.184505 django-cachalot-2.5.3/cachalot/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/cachalot/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16213 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/cachalot/tests/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/cachalot/tests/db_router.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/cachalot/tests/debug_toolbar.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/cachalot/tests/loaddata_fixture.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 09:16:11.184505 django-cachalot-2.5.3/cachalot/tests/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/cachalot/tests/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/cachalot/tests/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/cachalot/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/cachalot/tests/multi_db.py
--rw-r--r--   0 runner    (1001) docker     (123)    17804 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/cachalot/tests/postgres.py
--rw-r--r--   0 runner    (1001) docker     (123)    51739 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/cachalot/tests/read.py
--rw-r--r--   0 runner    (1001) docker     (123)    14319 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/cachalot/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/cachalot/tests/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/cachalot/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/cachalot/tests/tests_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/cachalot/tests/thread_safety.py
--rw-r--r--   0 runner    (1001) docker     (123)     8305 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/cachalot/tests/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    39764 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/cachalot/tests/write.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/cachalot/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    10121 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/cachalot/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 09:16:11.188505 django-cachalot-2.5.3/django_cachalot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-03-13 09:16:11.000000 django-cachalot-2.5.3/django_cachalot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-03-13 09:16:11.000000 django-cachalot-2.5.3/django_cachalot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 09:16:11.000000 django-cachalot-2.5.3/django_cachalot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 09:16:11.000000 django-cachalot-2.5.3/django_cachalot.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-13 09:16:11.000000 django-cachalot-2.5.3/django_cachalot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-13 09:16:11.000000 django-cachalot-2.5.3/django_cachalot.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 09:16:11.188505 django-cachalot-2.5.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6798 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/docs/benchmark.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8766 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/docs/how.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7807 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/docs/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/docs/legacy.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/docs/limits.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14828 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/docs/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/docs/reporting.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/docs/todo.rst
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      409 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/runtests.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/runtests_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-13 09:16:11.188505 django-cachalot-2.5.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1434 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-03-13 09:15:59.000000 django-cachalot-2.5.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:55:41.088571 django-cachalot-2.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    13789 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-07-21 09:55:41.088571 django-cachalot-2.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:55:41.080571 django-cachalot-2.6.0/cachalot/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:55:41.080571 django-cachalot-2.6.0/cachalot/admin_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/admin_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/admin_tests/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:55:41.080571 django-cachalot-2.6.0/cachalot/admin_tests/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/admin_tests/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/admin_tests/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/admin_tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/admin_tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/jinja2ext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:55:41.080571 django-cachalot-2.6.0/cachalot/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:55:41.080571 django-cachalot-2.6.0/cachalot/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/management/commands/invalidate_cachalot.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6888 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/monkey_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/panels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:55:41.076571 django-cachalot-2.6.0/cachalot/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:55:41.080571 django-cachalot-2.6.0/cachalot/templates/cachalot/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/templates/cachalot/panel.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:55:41.080571 django-cachalot-2.6.0/cachalot/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/templatetags/cachalot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:55:41.084571 django-cachalot-2.6.0/cachalot/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16213 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/tests/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/tests/db_router.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/tests/debug_toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/tests/loaddata_fixture.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:55:41.084571 django-cachalot-2.6.0/cachalot/tests/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/tests/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/tests/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/tests/multi_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18053 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/tests/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51433 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/tests/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14319 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/tests/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/tests/tests_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/tests/thread_safety.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8020 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/tests/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39198 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/tests/write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10555 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:55:41.088571 django-cachalot-2.6.0/django_cachalot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-07-21 09:55:41.000000 django-cachalot-2.6.0/django_cachalot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-07-21 09:55:41.000000 django-cachalot-2.6.0/django_cachalot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 09:55:41.000000 django-cachalot-2.6.0/django_cachalot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 09:55:41.000000 django-cachalot-2.6.0/django_cachalot.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-21 09:55:41.000000 django-cachalot-2.6.0/django_cachalot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 09:55:41.000000 django-cachalot-2.6.0/django_cachalot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:55:41.088571 django-cachalot-2.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6798 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/docs/benchmark.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8766 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/docs/how.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7807 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/docs/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/docs/legacy.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8140 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/docs/limits.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14824 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/docs/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/docs/reporting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/docs/todo.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      409 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/runtests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/runtests_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 09:55:41.088571 django-cachalot-2.6.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1446 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/tox.ini
```

### Comparing `django-cachalot-2.5.3/CHANGELOG.rst` & `django-cachalot-2.6.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,27 @@
 What’s new in django-cachalot?
 ==============================
 
+2.6.0
+-----
+
+- Dropped Django 2.2 and 4.0 support
+- Added Django 4.2 and Python 3.11 support
+- Added psycopg support (#229)
+- Updated tests to account for the `BEGIN` and `COMMIT` query changes in Django 4.2
+- Standardized django version comparisons in tests
+
 2.5.3
 -----
+
 - Verify get_meta isn't none before requesting db_table (#225 #226)
 
 2.5.2
 -----
+
 - Added Django 4.1 support (#217)
 
 2.5.1
 -----
 
 - Table invalidation condition enhanced (#213)
 - Add test settings to sdist (#203)
```

### Comparing `django-cachalot-2.5.3/LICENSE` & `django-cachalot-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.5.3/PKG-INFO` & `django-cachalot-2.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: django-cachalot
-Version: 2.5.3
+Version: 2.6.0
 Summary: Caches your Django ORM queries and automatically invalidates them.
 Home-page: https://github.com/noripyt/django-cachalot
 Author: Bertrand Bordage, Andrew Chen Wang
 Author-email: acwangpython@gmail.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 License-File: LICENSE
 
 Django Cachalot
 ===============
 
 Caches your Django ORM queries and automatically invalidates them.
@@ -60,15 +60,15 @@
 - Benchmark
 - Third-Party Cache Comparison
 - Discussion
 
 Quickstart
 ----------
 
-Cachalot officially supports Python 3.7-3.10 and Django 2.2, 3.2, and 4.0-4.1 with the databases PostgreSQL, SQLite, and MySQL.
+Cachalot officially supports Python 3.7-3.11 and Django 3.2, 4.1, 4.2 with the databases PostgreSQL, SQLite, and MySQL.
 
 Note: an upper limit on Django version is set for your safety. Please do not ignore it.
 
 Usage
 -----
 
 #. ``pip install django-cachalot``
```

### Comparing `django-cachalot-2.5.3/README.rst` & `django-cachalot-2.6.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 - Benchmark
 - Third-Party Cache Comparison
 - Discussion
 
 Quickstart
 ----------
 
-Cachalot officially supports Python 3.7-3.10 and Django 2.2, 3.2, and 4.0-4.1 with the databases PostgreSQL, SQLite, and MySQL.
+Cachalot officially supports Python 3.7-3.11 and Django 3.2, 4.1, 4.2 with the databases PostgreSQL, SQLite, and MySQL.
 
 Note: an upper limit on Django version is set for your safety. Please do not ignore it.
 
 Usage
 -----
 
 #. ``pip install django-cachalot``
```

### Comparing `django-cachalot-2.5.3/cachalot/admin_tests/migrations/0001_initial.py` & `django-cachalot-2.6.0/cachalot/admin_tests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.5.3/cachalot/admin_tests/models.py` & `django-cachalot-2.6.0/cachalot/admin_tests/models.py`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.5.3/cachalot/admin_tests/test_admin.py` & `django-cachalot-2.6.0/cachalot/admin_tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.5.3/cachalot/api.py` & `django-cachalot-2.6.0/cachalot/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from contextlib import contextmanager
+from typing import Any, Optional, Tuple, Union
 
 from django.apps import apps
 from django.conf import settings
 from django.db import connections
 
 from .cache import cachalot_caches
 from .settings import cachalot_settings
@@ -41,15 +42,19 @@
                 table_or_model = apps.get_model(table_or_model)
             except LookupError:
                 pass
         yield (table_or_model if isinstance(table_or_model, str)
                else table_or_model._meta.db_table)
 
 
-def invalidate(*tables_or_models, **kwargs):
+def invalidate(
+    *tables_or_models: Tuple[Union[str, Any], ...],
+    cache_alias: Optional[str] = None,
+    db_alias: Optional[str] = None,
+) -> None:
     """
     Clears what was cached by django-cachalot implying one or more SQL tables
     or models from ``tables_or_models``.
     If ``tables_or_models`` is not specified, all tables found in the database
     (including those outside Django) are invalidated.
 
     If ``cache_alias`` is specified, it only clears the SQL queries stored
@@ -58,27 +63,17 @@
     If ``db_alias`` is specified, it only clears the SQL queries executed
     on this database, otherwise queries from all databases are cleared.
 
     :arg tables_or_models: SQL tables names, models or models lookups
                            (or a combination)
     :type tables_or_models: tuple of strings or models
     :arg cache_alias: Alias from the Django ``CACHES`` setting
-    :type cache_alias: string or NoneType
     :arg db_alias: Alias from the Django ``DATABASES`` setting
-    :type db_alias: string or NoneType
     :returns: Nothing
-    :rtype: NoneType
     """
-    # TODO: Replace with positional arguments when we drop Python 2 support.
-    cache_alias = kwargs.pop('cache_alias', None)
-    db_alias = kwargs.pop('db_alias', None)
-    for k in kwargs:
-        raise TypeError(
-            "invalidate() got an unexpected keyword argument '%s'" % k)
-
     send_signal = False
     invalidated = set()
     for cache_alias, db_alias, tables in _cache_db_tables_iterator(
             list(_get_tables(tables_or_models)), cache_alias, db_alias):
         cache = cachalot_caches.get_cache(cache_alias, db_alias)
         if not isinstance(cache, AtomicCache):
             send_signal = True
@@ -86,15 +81,19 @@
         invalidated.update(tables)
 
     if send_signal:
         for table in invalidated:
             post_invalidation.send(table, db_alias=db_alias)
 
 
-def get_last_invalidation(*tables_or_models, **kwargs):
+def get_last_invalidation(
+    *tables_or_models: Tuple[Union[str, Any], ...],
+    cache_alias: Optional[str] = None,
+    db_alias: Optional[str] = None,
+) -> float:
     """
     Returns the timestamp of the most recent invalidation of the given
     ``tables_or_models``.  If ``tables_or_models`` is not specified,
     all tables found in the database (including those outside Django) are used.
 
     If ``cache_alias`` is specified, it only fetches invalidations
     in this cache, otherwise invalidations in all caches are fetched.
@@ -102,27 +101,17 @@
     If ``db_alias`` is specified, it only fetches invalidations
     for this database, otherwise invalidations for all databases are fetched.
 
     :arg tables_or_models: SQL tables names, models or models lookups
                            (or a combination)
     :type tables_or_models: tuple of strings or models
     :arg cache_alias: Alias from the Django ``CACHES`` setting
-    :type cache_alias: string or NoneType
     :arg db_alias: Alias from the Django ``DATABASES`` setting
-    :type db_alias: string or NoneType
     :returns: The timestamp of the most recent invalidation
-    :rtype: float
     """
-    # TODO: Replace with positional arguments when we drop Python 2 support.
-    cache_alias = kwargs.pop('cache_alias', None)
-    db_alias = kwargs.pop('db_alias', None)
-    for k in kwargs:
-        raise TypeError("get_last_invalidation() got an unexpected "
-                        "keyword argument '%s'" % k)
-
     last_invalidation = 0.0
     for cache_alias, db_alias, tables in _cache_db_tables_iterator(
             list(_get_tables(tables_or_models)), cache_alias, db_alias):
         get_table_cache_key = cachalot_settings.CACHALOT_TABLE_KEYGEN
         table_cache_keys = [get_table_cache_key(db_alias, t) for t in tables]
         invalidations = cachalot_caches.get_cache(
             cache_alias, db_alias).get_many(table_cache_keys).values()
@@ -130,15 +119,15 @@
             current_last_invalidation = max(invalidations)
             if current_last_invalidation > last_invalidation:
                 last_invalidation = current_last_invalidation
     return last_invalidation
 
 
 @contextmanager
-def cachalot_disabled(all_queries=False):
+def cachalot_disabled(all_queries: bool = False):
     """
     Context manager for temporarily disabling cachalot.
     If you evaluate the same queryset a second time,
     like normally for Django querysets, this will access
     the variable that saved it in-memory. For example:
 
     .. code-block:: python
@@ -154,14 +143,13 @@
             list(Test.objects.filter(blah=blah))
 
     If you evaluate the queryset outside the context manager, any duplicate
     query will use the cached result unless an object creation happens in between
     the original and duplicate query.
 
     :arg all_queries: Any query, including already evaluated queries, are re-evaluated.
-    :type all_queries: bool
     """
     was_enabled = getattr(LOCAL_STORAGE, "cachalot_enabled", cachalot_settings.CACHALOT_ENABLED)
     LOCAL_STORAGE.cachalot_enabled = False
     LOCAL_STORAGE.disable_on_all = all_queries
     yield
     LOCAL_STORAGE.cachalot_enabled = was_enabled
```

### Comparing `django-cachalot-2.5.3/cachalot/apps.py` & `django-cachalot-2.6.0/cachalot/apps.py`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.5.3/cachalot/cache.py` & `django-cachalot-2.6.0/cachalot/cache.py`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.5.3/cachalot/jinja2ext.py` & `django-cachalot-2.6.0/cachalot/jinja2ext.py`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.5.3/cachalot/management/commands/invalidate_cachalot.py` & `django-cachalot-2.6.0/cachalot/management/commands/invalidate_cachalot.py`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.5.3/cachalot/monkey_patch.py` & `django-cachalot-2.6.0/cachalot/monkey_patch.py`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.5.3/cachalot/panels.py` & `django-cachalot-2.6.0/cachalot/panels.py`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.5.3/cachalot/settings.py` & `django-cachalot-2.6.0/cachalot/settings.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,27 +5,23 @@
 from django.utils.module_loading import import_string
 
 
 SUPPORTED_DATABASE_ENGINES = {
     'django.db.backends.sqlite3',
     'django.db.backends.postgresql',
     'django.db.backends.mysql',
-    # TODO: Remove when we drop Django 2.x support.
-    'django.db.backends.postgresql_psycopg2',
 
     # GeoDjango
     'django.contrib.gis.db.backends.spatialite',
     'django.contrib.gis.db.backends.postgis',
     'django.contrib.gis.db.backends.mysql',
 
     # django-transaction-hooks
     'transaction_hooks.backends.sqlite3',
     'transaction_hooks.backends.postgis',
-    # TODO: Remove when we drop Django 2.x support.
-    'transaction_hooks.backends.postgresql_psycopg2',
     'transaction_hooks.backends.mysql',
 
     # django-prometheus wrapped engines
     'django_prometheus.db.backends.sqlite3',
     'django_prometheus.db.backends.postgresql',
     'django_prometheus.db.backends.mysql',
 }
```

### Comparing `django-cachalot-2.5.3/cachalot/templates/cachalot/panel.html` & `django-cachalot-2.6.0/cachalot/templates/cachalot/panel.html`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.5.3/cachalot/tests/__init__.py` & `django-cachalot-2.6.0/cachalot/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.5.3/cachalot/tests/api.py` & `django-cachalot-2.6.0/cachalot/tests/api.py`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.5.3/cachalot/tests/db_router.py` & `django-cachalot-2.6.0/cachalot/tests/db_router.py`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.5.3/cachalot/tests/debug_toolbar.py` & `django-cachalot-2.6.0/cachalot/tests/debug_toolbar.py`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.5.3/cachalot/tests/migrations/0001_initial.py` & `django-cachalot-2.6.0/cachalot/tests/migrations/0001_initial.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from django import VERSION as DJANGO_VERSION
 from django.conf import settings
 from django.contrib.postgres.fields import (
     ArrayField, HStoreField, IntegerRangeField,
-    DateRangeField, DateTimeRangeField)
+    DateRangeField, DateTimeRangeField, DecimalRangeField)
 from django.contrib.postgres.operations import (
     HStoreExtension, UnaccentExtension)
 from django.db import models, migrations
 
 
 def extra_regular_available_fields():
     fields = []
@@ -17,27 +17,14 @@
         pass
 
     return fields
 
 
 def extra_postgres_available_fields():
     fields = []
-    try:
-        # TODO Remove when Dj31 support is dropped
-        from django.contrib.postgres.fields import FloatRangeField
-        fields.append(('float_range', FloatRangeField(null=True, blank=True)))
-    except ImportError:
-        pass
-
-    try:
-        # TODO Add to module import when Dj31 is dropped
-        from django.contrib.postgres.fields import DecimalRangeField
-        fields.append(('decimal_range', DecimalRangeField(null=True, blank=True)))
-    except ImportError:
-        pass
 
     # Future proofing with Django 40 deprecation
     if DJANGO_VERSION[0] < 4:
         # TODO Remove when Dj40 support is dropped
         from django.contrib.postgres.fields import JSONField
         fields.append(('json', JSONField(null=True, blank=True)))
 
@@ -99,12 +86,13 @@
                 ('int_array', ArrayField(
                     models.IntegerField(null=True, blank=True), size=3,
                     null=True, blank=True)),
                 ('hstore', HStoreField(null=True, blank=True)),
                 ('int_range', IntegerRangeField(null=True, blank=True)),
                 ('date_range', DateRangeField(null=True, blank=True)),
                 ('datetime_range', DateTimeRangeField(null=True, blank=True)),
+                ('decimal_range', DecimalRangeField(null=True, blank=True))
             ] + extra_postgres_available_fields(),
         ),
         migrations.RunSQL('CREATE TABLE cachalot_unmanagedmodel '
                           '(id SERIAL PRIMARY KEY, name VARCHAR(50));'),
     ]
```

### Comparing `django-cachalot-2.5.3/cachalot/tests/models.py` & `django-cachalot-2.6.0/cachalot/tests/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
 
 class PostgresModel(Model):
     int_array = ArrayField(IntegerField(null=True, blank=True), size=3,
                            null=True, blank=True)
 
     hstore = HStoreField(null=True, blank=True)
-    if DJANGO_VERSION[0] < 4:
+    if DJANGO_VERSION < (4, 0):
         from django.contrib.postgres.fields import JSONField
         json = JSONField(null=True, blank=True)
 
     int_range = IntegerRangeField(null=True, blank=True)
     try:
         from django.contrib.postgres.fields import FloatRangeField
         float_range = FloatRangeField(null=True, blank=True)
```

### Comparing `django-cachalot-2.5.3/cachalot/tests/multi_db.py` & `django-cachalot-2.6.0/cachalot/tests/multi_db.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from unittest import skipIf
 
-from django import VERSION as DJANGO_VERSION
 from django.conf import settings
 from django.db import DEFAULT_DB_ALIAS, connections, transaction
 from django.test import TransactionTestCase
 
 from .models import Test
 
 
@@ -23,32 +22,14 @@
         self.is_sqlite2 = connection2.vendor == 'sqlite'
         self.is_mysql2 = connection2.vendor == 'mysql'
         if connection2.vendor in ('mysql', 'postgresql'):
             # We need to reopen the connection or Django
             # will execute an extra SQL request below.
             connection2.cursor()
 
-    def is_django_21_below_and_sqlite2(self):
-        """
-        Note: See test_utils.py with this function name
-        Checks if Django 2.1 or below and SQLite2
-        """
-        django_version = DJANGO_VERSION
-        if not self.is_sqlite2:
-            # Immediately know if SQLite
-            return False
-        if django_version[0] < 2:
-            # Takes Django 0 and 1 out of the picture
-            return True
-        else:
-            if django_version[0] == 2 and django_version[1] < 2:
-                # Takes Django 2.0-2.1 out
-                return True
-            return False
-
     def test_read(self):
         with self.assertNumQueries(1):
             data1 = list(Test.objects.all())
             self.assertListEqual(data1, [self.t1, self.t2])
 
         with self.assertNumQueries(1, using=self.db_alias2):
             data2 = list(Test.objects.using(self.db_alias2))
@@ -62,32 +43,30 @@
         """
         Tests if the non-default database is invalidated when modified.
         """
         with self.assertNumQueries(1, using=self.db_alias2):
             data1 = list(Test.objects.using(self.db_alias2))
             self.assertListEqual(data1, [])
 
-        with self.assertNumQueries(2 if self.is_django_21_below_and_sqlite2() else 1,
-                                   using=self.db_alias2):
+        with self.assertNumQueries(1, using=self.db_alias2):
             t3 = Test.objects.using(self.db_alias2).create(name='test3')
 
         with self.assertNumQueries(1, using=self.db_alias2):
             data2 = list(Test.objects.using(self.db_alias2))
             self.assertListEqual(data2, [t3])
 
     def test_invalidation_independence(self):
         """
         Tests if invalidation doesn’t affect the unmodified databases.
         """
         with self.assertNumQueries(1):
             data1 = list(Test.objects.all())
             self.assertListEqual(data1, [self.t1, self.t2])
 
-        with self.assertNumQueries(2 if self.is_django_21_below_and_sqlite2() else 1,
-                                   using=self.db_alias2):
+        with self.assertNumQueries(1, using=self.db_alias2):
             Test.objects.using(self.db_alias2).create(name='test3')
 
         with self.assertNumQueries(0):
             data2 = list(Test.objects.all())
             self.assertListEqual(data2, [self.t1, self.t2])
 
     def test_heterogeneous_atomics(self):
```

### Comparing `django-cachalot-2.5.3/cachalot/tests/postgres.py` & `django-cachalot-2.6.0/cachalot/tests/postgres.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,26 @@
 from datetime import date, datetime
 from decimal import Decimal
 from unittest import skipUnless
 
+from django import VERSION
 from django.contrib.postgres.functions import TransactionNow
 from django.db import connection
 from django.test import TransactionTestCase, override_settings
-from psycopg2.extras import DateRange, DateTimeTZRange, NumericRange
+
+# If we are using Django 4.2 or higher, we need to use:
+if VERSION >= (4, 2):
+    from django.db.backends.postgresql.psycopg_any import (
+        DateRange,
+        DateTimeTZRange,
+        NumericRange,
+    )
+else:
+    from psycopg2.extras import DateRange, DateTimeTZRange, NumericRange
+
 from pytz import timezone
 
 from ..utils import UncachableQuery
 from .api import invalidate
 from .models import PostgresModel, Test
 from .test_utils import TestUtilsMixin
 from .tests_decorators import all_final_sql_checks, no_final_sql_check, with_final_sql_check
```

### Comparing `django-cachalot-2.5.3/cachalot/tests/read.py` & `django-cachalot-2.6.0/cachalot/tests/read.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import datetime
 from unittest import skipIf
 from uuid import UUID
 from decimal import Decimal
 
-from django import VERSION as django_version
+from django import VERSION as DJANGO_VERSION
 from django.conf import settings
 from django.contrib.auth.models import Group, Permission, User
 from django.contrib.contenttypes.models import ContentType
 from django.db import (
     connection, transaction, DEFAULT_DB_ALIAS, ProgrammingError,
     OperationalError)
 from django.db.models import Case, Count, Q, Value, When
@@ -17,30 +17,30 @@
 from django.test import TransactionTestCase, skipUnlessDBFeature, override_settings
 from pytz import UTC
 
 from cachalot.cache import cachalot_caches
 from ..settings import cachalot_settings
 from ..utils import UncachableQuery
 from .models import Test, TestChild, TestParent, UnmanagedModel
-from .test_utils import TestUtilsMixin
+from .test_utils import TestUtilsMixin, FilteredTransactionTestCase
 
 from .tests_decorators import all_final_sql_checks, with_final_sql_check, no_final_sql_check
 
 
 def is_field_available(name):
     fields = []
     try:
         from django.db.models import JSONField
         fields.append("JSONField")
     except ImportError:
         pass
     return name in fields
 
 
-class ReadTestCase(TestUtilsMixin, TransactionTestCase):
+class ReadTestCase(TestUtilsMixin, FilteredTransactionTestCase):
     """
     Tests if every SQL request that only reads data is cached.
 
     The only exception is for requests that don’t go through the ORM, using
     ``QuerySet.extra`` with ``select`` or ``where`` arguments,
      ``Model.objects.raw``, or ``cursor.execute``.
     """
@@ -349,15 +349,15 @@
         qs = self._test_many_to_many()
         self.assert_tables(qs, User, User.user_permissions.through, Permission)
         self.assert_query_cached(qs, ['cuddle', 'discuss', 'touch'])
 
     @all_final_sql_checks
     def test_subquery(self):
         additional_tables = []
-        if django_version[0] == 4 and django_version[1] < 1 and settings.CACHALOT_FINAL_SQL_CHECK:
+        if DJANGO_VERSION >= (4, 0) and DJANGO_VERSION < (4, 1) and settings.CACHALOT_FINAL_SQL_CHECK:
             # with Django 4.0 comes some query optimalizations that do selects little differently.
             additional_tables.append('django_content_type')
         qs = Test.objects.filter(owner__in=User.objects.all())
         self.assert_tables(qs, Test, User)
         self.assert_query_cached(qs, [self.t1, self.t2])
 
         qs = Test.objects.filter(
@@ -690,15 +690,15 @@
             Test.objects.filter(pk__lt=5)
             | Test.objects.filter(permission__name__contains='a')
         )
         self.assert_tables(qs, Test, Permission)
         self.assert_query_cached(qs)
 
         with self.assertRaisesMessage(
-            AssertionError if django_version[0] < 4 else TypeError,
+            AssertionError if DJANGO_VERSION < (4, 0) else TypeError,
             'Cannot combine queries on two different base models.'
         ):
             Test.objects.all() | Permission.objects.all()
 
         qs = Test.objects.filter(pk__lt=5)
         sub_qs = Test.objects.filter(permission__name__contains='a')
         if self.is_sqlite:
@@ -735,15 +735,15 @@
     def _test_intersection(self, check: bool):
         qs = (Test.objects.filter(pk__lt=5)
               & Test.objects.filter(permission__name__contains='a'))
         self.assert_tables(qs, Test, Permission)
         self.assert_query_cached(qs)
 
         with self.assertRaisesMessage(
-                AssertionError if django_version[0] < 4 else TypeError,
+                AssertionError if DJANGO_VERSION < (4, 0) else TypeError,
                 'Cannot combine queries on two different base models.'):
             Test.objects.all() & Permission.objects.all()
 
         qs = Test.objects.filter(pk__lt=5)
         sub_qs = Test.objects.filter(permission__name__contains='a')
         if self.is_sqlite:
             qs = qs.order_by()
@@ -892,38 +892,33 @@
     @all_final_sql_checks
     def test_extra_order_by(self):
         qs = Test.objects.extra(order_by=['-cachalot_test.name'])
         self.assert_tables(qs, Test)
         self.assert_query_cached(qs, [self.t2, self.t1])
 
     def test_table_inheritance(self):
-        with self.assertNumQueries(3 if self.is_sqlite else 2):
+        with self.assertNumQueries(2):
             t_child = TestChild.objects.create(name='test_child')
 
         with self.assertNumQueries(1):
             self.assertEqual(TestChild.objects.get(), t_child)
 
         with self.assertNumQueries(0):
             self.assertEqual(TestChild.objects.get(), t_child)
 
     def test_explain(self):
         explain_kwargs = {}
         if self.is_sqlite:
             expected = (r'\d+ 0 0 SCAN cachalot_test\n'
                         r'\d+ 0 0 USE TEMP B-TREE FOR ORDER BY')
         elif self.is_mysql:
-            if self.django_version < (3, 1):
-                expected = (
-                    r'1 SIMPLE cachalot_test '
-                    r'(?:None )?ALL None None None None 2 100\.0 Using filesort')
-            else:
-                expected = (
-                    r'-> Sort row IDs: cachalot_test.`name`  \(cost=[\d\.]+ rows=\d\)\n    '
-                    r'-> Table scan on cachalot_test  \(cost=[\d\.]+ rows=\d\)\n'
-                )
+            expected = (
+                r'-> Sort row IDs: cachalot_test.`name`  \(cost=[\d\.]+ rows=\d\)\n    '
+                r'-> Table scan on cachalot_test  \(cost=[\d\.]+ rows=\d\)\n'
+            )
         else:
             explain_kwargs.update(
                 analyze=True,
                 costs=False,
             )
             operation_detail = (r'\(actual time=[\d\.]+..[\d\.]+\ '
                                 r'rows=\d+ loops=\d+\)')
@@ -931,17 +926,15 @@
                 r'^Sort %s\n'
                 r'  Sort Key: name\n'
                 r'  Sort Method: quicksort  Memory: \d+kB\n'
                 r'  ->  Seq Scan on cachalot_test %s\n'
                 r'Planning Time: [\d\.]+ ms\n'
                 r'Execution Time: [\d\.]+ ms$') % (operation_detail,
                                                    operation_detail)
-        with self.assertNumQueries(
-                2 if self.is_mysql and django_version[0] < 3
-                else 1):
+        with self.assertNumQueries(1):
             explanation1 = Test.objects.explain(**explain_kwargs)
         self.assertRegex(explanation1, expected)
         with self.assertNumQueries(0):
             explanation2 = Test.objects.explain(**explain_kwargs)
         self.assertEqual(explanation2, explanation1)
 
     def test_raw(self):
@@ -1216,23 +1209,23 @@
 
         test1.delete()
         test2.delete()
 
     @all_final_sql_checks
     def test_ipv6_address(self):
         with self.assertNumQueries(1):
-            test1 = Test.objects.create(name='test1', ip='2001:db8:a0b:12f0::1/64')
+            test1 = Test.objects.create(name='test1', ip='2001:db8:a0b:12f0::1')
         with self.assertNumQueries(1):
             test2 = Test.objects.create(name='test2', ip='2001:db8:0:85a3::ac1f:8001')
 
         qs = Test.objects.values_list('ip', flat=True).filter(
             ip__isnull=False).order_by('ip')
         self.assert_tables(qs, Test)
         self.assert_query_cached(qs, ['2001:db8:0:85a3::ac1f:8001',
-                                      '2001:db8:a0b:12f0::1/64'])
+                                      '2001:db8:a0b:12f0::1'])
 
         with self.assertNumQueries(1):
             Test.objects.get(ip='2001:db8:0:85a3::ac1f:8001')
         with self.assertNumQueries(0):
             Test.objects.get(ip='2001:db8:0:85a3::ac1f:8001')
 
         test1.delete()
```

### Comparing `django-cachalot-2.5.3/cachalot/tests/settings.py` & `django-cachalot-2.6.0/cachalot/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.5.3/cachalot/tests/signals.py` & `django-cachalot-2.6.0/cachalot/tests/signals.py`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.5.3/cachalot/tests/tests_decorators.py` & `django-cachalot-2.6.0/cachalot/tests/tests_decorators.py`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.5.3/cachalot/tests/thread_safety.py` & `django-cachalot-2.6.0/cachalot/tests/thread_safety.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from threading import Thread
 
 from django.db import connection, transaction
-from django.test import TransactionTestCase, skipUnlessDBFeature
+from django.test import skipUnlessDBFeature
 
 from .models import Test
-from .test_utils import TestUtilsMixin
+from .test_utils import TestUtilsMixin, FilteredTransactionTestCase
 
 
 class TestThread(Thread):
     def start_and_join(self):
         self.start()
         self.join()
         return self.t
 
     def run(self):
         self.t = Test.objects.first()
         connection.close()
 
 
 @skipUnlessDBFeature('test_db_allows_multiple_connections')
-class ThreadSafetyTestCase(TestUtilsMixin, TransactionTestCase):
+class ThreadSafetyTestCase(TestUtilsMixin, FilteredTransactionTestCase):
     def test_concurrent_caching(self):
         t1 = TestThread().start_and_join()
         t = Test.objects.create(name='test')
         t2 = TestThread().start_and_join()
 
         self.assertEqual(t1, None)
         self.assertEqual(t2, t)
```

### Comparing `django-cachalot-2.5.3/cachalot/tests/transaction.py` & `django-cachalot-2.6.0/cachalot/tests/transaction.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 from cachalot.transaction import AtomicCache
+
 from django.contrib.auth.models import User
 from django.core.cache import cache
 from django.db import transaction, connection, IntegrityError
-from django.test import SimpleTestCase, TransactionTestCase, skipUnlessDBFeature
+from django.test import SimpleTestCase, skipUnlessDBFeature
 
 from .models import Test
-from .test_utils import TestUtilsMixin
+from .test_utils import TestUtilsMixin, FilteredTransactionTestCase
 
 
-class AtomicTestCase(TestUtilsMixin, TransactionTestCase):
+class AtomicTestCase(TestUtilsMixin, FilteredTransactionTestCase):
     def test_successful_read_atomic(self):
-        with self.assertNumQueries(2 if self.is_sqlite else 1):
+        with self.assertNumQueries(1):
             with transaction.atomic():
                 data1 = list(Test.objects.all())
         self.assertListEqual(data1, [])
 
         with self.assertNumQueries(0):
             data2 = list(Test.objects.all())
         self.assertListEqual(data2, [])
 
     def test_unsuccessful_read_atomic(self):
-        with self.assertNumQueries(2 if self.is_sqlite else 1):
+        with self.assertNumQueries(1):
             try:
                 with transaction.atomic():
                     data1 = list(Test.objects.all())
                     raise ZeroDivisionError
             except ZeroDivisionError:
                 pass
         self.assertListEqual(data1, [])
@@ -34,104 +35,104 @@
         self.assertListEqual(data2, [])
 
     def test_successful_write_atomic(self):
         with self.assertNumQueries(1):
             data1 = list(Test.objects.all())
         self.assertListEqual(data1, [])
 
-        with self.assertNumQueries(2 if self.is_sqlite else 1):
+        with self.assertNumQueries(1):
             with transaction.atomic():
                 t1 = Test.objects.create(name='test1')
         with self.assertNumQueries(1):
             data2 = list(Test.objects.all())
         self.assertListEqual(data2, [t1])
 
-        with self.assertNumQueries(2 if self.is_sqlite else 1):
+        with self.assertNumQueries(1):
             with transaction.atomic():
                 t2 = Test.objects.create(name='test2')
         with self.assertNumQueries(1):
             data3 = list(Test.objects.all())
         self.assertListEqual(data3, [t1, t2])
 
-        with self.assertNumQueries(4 if self.is_sqlite else 3):
+        with self.assertNumQueries(3):
             with transaction.atomic():
                 data4 = list(Test.objects.all())
                 t3 = Test.objects.create(name='test3')
                 t4 = Test.objects.create(name='test4')
                 data5 = list(Test.objects.all())
         self.assertListEqual(data4, [t1, t2])
         self.assertListEqual(data5, [t1, t2, t3, t4])
         self.assertNotEqual(t4, t3)
 
     def test_unsuccessful_write_atomic(self):
         with self.assertNumQueries(1):
             data1 = list(Test.objects.all())
         self.assertListEqual(data1, [])
 
-        with self.assertNumQueries(2 if self.is_sqlite else 1):
+        with self.assertNumQueries(1):
             try:
                 with transaction.atomic():
                     Test.objects.create(name='test')
                     raise ZeroDivisionError
             except ZeroDivisionError:
                 pass
         with self.assertNumQueries(0):
             data2 = list(Test.objects.all())
         self.assertListEqual(data2, [])
         with self.assertNumQueries(1):
             with self.assertRaises(Test.DoesNotExist):
                 Test.objects.get(name='test')
 
     def test_cache_inside_atomic(self):
-        with self.assertNumQueries(2 if self.is_sqlite else 1):
+        with self.assertNumQueries(1):
             with transaction.atomic():
                 data1 = list(Test.objects.all())
                 data2 = list(Test.objects.all())
         self.assertListEqual(data2, data1)
         self.assertListEqual(data2, [])
 
     def test_invalidation_inside_atomic(self):
-        with self.assertNumQueries(4 if self.is_sqlite else 3):
+        with self.assertNumQueries(3):
             with transaction.atomic():
                 data1 = list(Test.objects.all())
                 t = Test.objects.create(name='test')
                 data2 = list(Test.objects.all())
         self.assertListEqual(data1, [])
         self.assertListEqual(data2, [t])
 
     def test_successful_nested_read_atomic(self):
-        with self.assertNumQueries(7 if self.is_sqlite else 6):
+        with self.assertNumQueries(6):
             with transaction.atomic():
                 list(Test.objects.all())
                 with transaction.atomic():
                     list(User.objects.all())
                     with self.assertNumQueries(2):
                         with transaction.atomic():
                             list(User.objects.all())
                 with self.assertNumQueries(0):
                     list(User.objects.all())
         with self.assertNumQueries(0):
             list(Test.objects.all())
             list(User.objects.all())
 
     def test_unsuccessful_nested_read_atomic(self):
-        with self.assertNumQueries(6 if self.is_sqlite else 5):
+        with self.assertNumQueries(5):
             with transaction.atomic():
                 try:
                     with transaction.atomic():
                         with self.assertNumQueries(1):
                             list(Test.objects.all())
                         raise ZeroDivisionError
                 except ZeroDivisionError:
                     pass
                 with self.assertNumQueries(1):
                     list(Test.objects.all())
 
     def test_successful_nested_write_atomic(self):
-        with self.assertNumQueries(13 if self.is_sqlite else 12):
+        with self.assertNumQueries(12):
             with transaction.atomic():
                 t1 = Test.objects.create(name='test1')
                 with transaction.atomic():
                     t2 = Test.objects.create(name='test2')
                 data1 = list(Test.objects.all())
                 self.assertListEqual(data1, [t1, t2])
                 with transaction.atomic():
@@ -140,15 +141,15 @@
                         data2 = list(Test.objects.all())
                         self.assertListEqual(data2, [t1, t2, t3])
                         t4 = Test.objects.create(name='test4')
         data3 = list(Test.objects.all())
         self.assertListEqual(data3, [t1, t2, t3, t4])
 
     def test_unsuccessful_nested_write_atomic(self):
-        with self.assertNumQueries(16 if self.is_sqlite else 15):
+        with self.assertNumQueries(15):
             with transaction.atomic():
                 t1 = Test.objects.create(name='test1')
                 try:
                     with transaction.atomic():
                         t2 = Test.objects.create(name='test2')
                         data1 = list(Test.objects.all())
                         self.assertListEqual(data1, [t1, t2])
```

### Comparing `django-cachalot-2.5.3/cachalot/tests/write.py` & `django-cachalot-2.6.0/cachalot/tests/write.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 from unittest import skipIf, skipUnless
 
-from django import VERSION as DJANGO_VERSION
 from django.contrib.auth.models import User, Permission, Group
 from django.contrib.contenttypes.models import ContentType
 from django.core.exceptions import MultipleObjectsReturned
 from django.core.management import call_command
 from django.db import (
     connection, transaction, ProgrammingError, OperationalError)
 from django.db.models import Count
 from django.db.models.expressions import RawSQL
 from django.test import TransactionTestCase, skipUnlessDBFeature
 
 from .models import Test, TestParent, TestChild
-from .test_utils import TestUtilsMixin
+from .test_utils import TestUtilsMixin, FilteredTransactionTestCase
 
 
-class WriteTestCase(TestUtilsMixin, TransactionTestCase):
+class WriteTestCase(TestUtilsMixin, FilteredTransactionTestCase):
     """
     Tests if every SQL request writing data is not cached and invalidates the
     implied data.
     """
 
     def test_create(self):
         with self.assertNumQueries(1):
@@ -52,15 +51,15 @@
         Tests if the ``SELECT`` query of a ``QuerySet.get_or_create``
         is cached, but not the ``INSERT`` one.
         """
         with self.assertNumQueries(1):
             data1 = list(Test.objects.all())
         self.assertListEqual(data1, [])
 
-        with self.assertNumQueries(3 if self.is_sqlite else 2):
+        with self.assertNumQueries(2):
             t, created = Test.objects.get_or_create(name='test')
         self.assertTrue(created)
 
         with self.assertNumQueries(1):
             t_clone, created = Test.objects.get_or_create(name='test')
         self.assertFalse(created)
         self.assertEqual(t_clone, t)
@@ -74,51 +73,51 @@
             data2 = list(Test.objects.all())
         self.assertListEqual(data2, [t])
 
     def test_update_or_create(self):
         with self.assertNumQueries(1):
             self.assertListEqual(list(Test.objects.all()), [])
 
-        with self.assertNumQueries(5 if self.is_sqlite else 4):
+        with self.assertNumQueries(4):
             t, created = Test.objects.update_or_create(
                 name='test', defaults={'public': True})
             self.assertTrue(created)
             self.assertEqual(t.name, 'test')
             self.assertEqual(t.public, True)
 
-        with self.assertNumQueries(3 if self.is_sqlite else 2):
+        with self.assertNumQueries(2):
             t, created = Test.objects.update_or_create(
                 name='test', defaults={'public': False})
             self.assertFalse(created)
             self.assertEqual(t.name, 'test')
             self.assertEqual(t.public, False)
 
         # The number of SQL queries doesn’t decrease because update_or_create
         # always calls an UPDATE, even when data wasn’t changed.
-        with self.assertNumQueries(3 if self.is_sqlite else 2):
+        with self.assertNumQueries(2):
             t, created = Test.objects.update_or_create(
                 name='test', defaults={'public': False})
             self.assertFalse(created)
             self.assertEqual(t.name, 'test')
             self.assertEqual(t.public, False)
 
         with self.assertNumQueries(1):
             self.assertListEqual(list(Test.objects.all()), [t])
 
     def test_bulk_create(self):
         with self.assertNumQueries(1):
             data1 = list(Test.objects.all())
         self.assertListEqual(data1, [])
 
-        with self.assertNumQueries(2 if self.is_sqlite else 1):
+        with self.assertNumQueries(1):
             unsaved_tests = [Test(name='test%02d' % i) for i in range(1, 11)]
             Test.objects.bulk_create(unsaved_tests)
         self.assertEqual(Test.objects.count(), 10)
 
-        with self.assertNumQueries(2 if self.is_sqlite else 1):
+        with self.assertNumQueries(1):
             unsaved_tests = [Test(name='test%02d' % i) for i in range(1, 11)]
             Test.objects.bulk_create(unsaved_tests)
         self.assertEqual(Test.objects.count(), 20)
 
         with self.assertNumQueries(1):
             data2 = list(Test.objects.all())
         self.assertEqual(len(data2), 20)
@@ -156,20 +155,20 @@
         with self.assertNumQueries(1):
             t2.delete()
         with self.assertNumQueries(1):
             data2 = list(Test.objects.values_list('name', flat=True))
         self.assertListEqual(data1, [t1.name, t2.name])
         self.assertListEqual(data2, [t1.name])
 
-        with self.assertNumQueries(2 if self.is_sqlite else 1):
+        with self.assertNumQueries(1):
             Test.objects.bulk_create([Test(name='test%s' % i)
                                       for i in range(2, 11)])
         with self.assertNumQueries(1):
             self.assertEqual(Test.objects.count(), 10)
-        with self.assertNumQueries(2 if self.is_sqlite else 1):
+        with self.assertNumQueries(1):
             Test.objects.all().delete()
         with self.assertNumQueries(1):
             self.assertEqual(Test.objects.count(), 0)
 
     def test_invalidate_exists(self):
         with self.assertNumQueries(1):
             self.assertFalse(Test.objects.exists())
@@ -356,15 +355,15 @@
         with self.assertNumQueries(1):
             Test.objects.create(name='test2', owner=user1)
         with self.assertNumQueries(1):
             data4 = list(User.objects.annotate(n=Count('test')).order_by('pk'))
         self.assertListEqual(data4, [user1, user2])
         self.assertListEqual([u.n for u in data4], [1, 0])
 
-        with self.assertNumQueries(2 if self.is_sqlite else 1):
+        with self.assertNumQueries(1):
             Test.objects.bulk_create([
                 Test(name='test3', owner=user1),
                 Test(name='test4', owner=user2),
                 Test(name='test5', owner=user1),
                 Test(name='test6', owner=user2),
             ])
         with self.assertNumQueries(1):
@@ -584,29 +583,29 @@
         with self.assertNumQueries(2):
             u1 = User.objects.create_user('test1')
             u2 = User.objects.create_user('test2')
         with self.assertNumQueries(1):
             data2 = list(Test.objects.select_related('owner'))
         self.assertListEqual(data2, [])
 
-        with self.assertNumQueries(2 if self.is_sqlite else 1):
+        with self.assertNumQueries(1):
             Test.objects.bulk_create([
                 Test(name='test1', owner=u1),
                 Test(name='test2', owner=u2),
                 Test(name='test3', owner=u2),
                 Test(name='test4', owner=u1),
             ])
         with self.assertNumQueries(1):
             data3 = list(Test.objects.select_related('owner'))
             self.assertEqual(data3[0].owner, u1)
             self.assertEqual(data3[1].owner, u2)
             self.assertEqual(data3[2].owner, u2)
             self.assertEqual(data3[3].owner, u1)
 
-        with self.assertNumQueries(2 if self.is_sqlite else 1):
+        with self.assertNumQueries(1):
             Test.objects.filter(name__in=['test1', 'test2']).delete()
         with self.assertNumQueries(1):
             data4 = list(Test.objects.select_related('owner'))
             self.assertEqual(data4[0].owner, u2)
             self.assertEqual(data4[1].owner, u1)
 
     def test_invalidate_prefetch_related(self):
@@ -630,20 +629,15 @@
         with self.assertNumQueries(2):
             data3 = list(Test.objects.select_related('owner')
                          .prefetch_related('owner__groups__permissions'))
             self.assertListEqual(data3, [t1])
             self.assertEqual(data3[0].owner, u)
             self.assertListEqual(list(data3[0].owner.groups.all()), [])
 
-        with self.assertNumQueries(
-                8 if self.is_sqlite and DJANGO_VERSION[0] == 2 and DJANGO_VERSION[1] == 2
-                else 4 if self.is_postgresql and DJANGO_VERSION[0] > 2
-                else 4 if self.is_mysql and DJANGO_VERSION[0] > 2
-                else 6
-        ):
+        with self.assertNumQueries(4):
             group = Group.objects.create(name='test_group')
             permissions = list(Permission.objects.all()[:5])
             group.permissions.add(*permissions)
             u.groups.add(group)
         with self.assertNumQueries(2):
             data4 = list(Test.objects.select_related('owner')
                          .prefetch_related('owner__groups__permissions'))
@@ -848,15 +842,15 @@
             self.assertListEqual(data2, [t2, t1])
 
     def test_invalidate_table_inheritance(self):
         with self.assertNumQueries(1):
             with self.assertRaises(TestChild.DoesNotExist):
                 TestChild.objects.get()
 
-        with self.assertNumQueries(3 if self.is_sqlite else 2):
+        with self.assertNumQueries(2):
             t_child = TestChild.objects.create(name='test_child')
 
         with self.assertNumQueries(1):
             self.assertEqual(TestChild.objects.get(), t_child)
 
         with self.assertNumQueries(1):
             TestParent.objects.filter(pk=t_child.pk).update(name='modified')
```

### Comparing `django-cachalot-2.5.3/cachalot/transaction.py` & `django-cachalot-2.6.0/cachalot/transaction.py`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.5.3/cachalot/utils.py` & `django-cachalot-2.6.0/cachalot/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from decimal import Decimal
 from hashlib import sha1
 from time import time
 from typing import TYPE_CHECKING
 from uuid import UUID
 
 from django.contrib.postgres.functions import TransactionNow
-from django.db import connections
+from django.db import connections, connection
 from django.db.models import Exists, QuerySet, Subquery
 from django.db.models.expressions import RawSQL
 from django.db.models.functions import Now
 from django.db.models.sql import Query, AggregateQuery
 from django.db.models.sql.where import ExtraWhere, WhereNode, NothingNode
 
 from .settings import ITERABLES, cachalot_settings
@@ -31,32 +31,50 @@
 
 CACHABLE_PARAM_TYPES = {
     bool, int, float, Decimal, bytearray, bytes, str, type(None),
     datetime.date, datetime.time, datetime.datetime, datetime.timedelta, UUID,
 }
 UNCACHABLE_FUNCS = {Now, TransactionNow}
 
-try:
-    # TODO Drop after Dj30 drop
-    from django.contrib.postgres.fields.jsonb import JsonAdapter
-    CACHABLE_PARAM_TYPES.update((JsonAdapter,))
-except ImportError:
-    pass
+# Check if psycopg2 or 3 is used
+connection.ensure_connection()
+underlying_connection = connection.connection
 
-try:
+if underlying_connection.__class__.__module__.startswith('psycopg2'):
     from psycopg2 import Binary
     from psycopg2.extras import (
         NumericRange, DateRange, DateTimeRange, DateTimeTZRange, Inet, Json)
-except ImportError:
-    pass
-else:
     CACHABLE_PARAM_TYPES.update((
         Binary, NumericRange, DateRange, DateTimeRange, DateTimeTZRange, Inet,
         Json,))
+elif underlying_connection.__class__.__module__.startswith('psycopg'):
+    from django.db.backends.postgresql.psycopg_any import (
+        NumericRange, DateRange, DateTimeRange, DateTimeTZRange, Inet,
+    )
+
+    from psycopg.dbapi20 import Binary
+
+    from psycopg.types.numeric import (
+        Int2, Int4, Int8, Float4, Float8,
+    )
+
+    from ipaddress import (
+        IPv4Address,
+        IPv6Address,
+    )
+
+    from psycopg.types.json import (
+        Json, Jsonb,
+    )
 
+    CACHABLE_PARAM_TYPES.update((
+        NumericRange, DateRange, DateTimeRange, DateTimeTZRange, Inet, Json, Jsonb,
+        Int2, Int4, Int8, Float4, Float8, IPv4Address, IPv6Address,
+        Binary,
+    ))
 
 def check_parameter_types(params):
     for p in params:
         cl = p.__class__
         if cl not in CACHABLE_PARAM_TYPES:
             if cl in ITERABLES:
                 check_parameter_types(p)
@@ -127,21 +145,15 @@
 def _find_rhs_lhs_subquery(side):
     h_class = side.__class__
     if h_class is Query:
         return side
     elif h_class is QuerySet:
         return side.query
     elif h_class in (Subquery, Exists):  # Subquery allows QuerySet & Query
-        try:
-            return side.query.query if side.query.__class__ is QuerySet else side.query
-        except AttributeError:  # TODO Remove try/except closure after drop Django 2.2
-            try:
-                return side.queryset.query
-            except AttributeError:
-                return None
+        return side.query.query if side.query.__class__ is QuerySet else side.query
     elif h_class in UNCACHABLE_FUNCS:
         raise UncachableQuery
 
 
 def _find_subqueries_in_where(children):
     for child in children:
         child_class = child.__class__
```

### Comparing `django-cachalot-2.5.3/django_cachalot.egg-info/PKG-INFO` & `django-cachalot-2.6.0/django_cachalot.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: django-cachalot
-Version: 2.5.3
+Version: 2.6.0
 Summary: Caches your Django ORM queries and automatically invalidates them.
 Home-page: https://github.com/noripyt/django-cachalot
 Author: Bertrand Bordage, Andrew Chen Wang
 Author-email: acwangpython@gmail.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 License-File: LICENSE
 
 Django Cachalot
 ===============
 
 Caches your Django ORM queries and automatically invalidates them.
@@ -60,15 +60,15 @@
 - Benchmark
 - Third-Party Cache Comparison
 - Discussion
 
 Quickstart
 ----------
 
-Cachalot officially supports Python 3.7-3.10 and Django 2.2, 3.2, and 4.0-4.1 with the databases PostgreSQL, SQLite, and MySQL.
+Cachalot officially supports Python 3.7-3.11 and Django 3.2, 4.1, 4.2 with the databases PostgreSQL, SQLite, and MySQL.
 
 Note: an upper limit on Django version is set for your safety. Please do not ignore it.
 
 Usage
 -----
 
 #. ``pip install django-cachalot``
```

### Comparing `django-cachalot-2.5.3/django_cachalot.egg-info/SOURCES.txt` & `django-cachalot-2.6.0/django_cachalot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.5.3/docs/Makefile` & `django-cachalot-2.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.5.3/docs/benchmark.rst` & `django-cachalot-2.6.0/docs/benchmark.rst`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.5.3/docs/conf.py` & `django-cachalot-2.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.5.3/docs/how.rst` & `django-cachalot-2.6.0/docs/how.rst`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.5.3/docs/index.rst` & `django-cachalot-2.6.0/docs/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 .. image:: https://raw.github.com/noripyt/django-cachalot/master/django-cachalot.jpg
 
 ----
 
 .. image:: http://img.shields.io/pypi/v/django-cachalot.svg?style=flat-square&maxAge=3600
    :target: https://pypi.python.org/pypi/django-cachalot
 
-.. image:: http://img.shields.io/travis/noripyt/django-cachalot/master.svg?style=flat-square&maxAge=3600
-   :target: https://travis-ci.org/noripyt/django-cachalot
+.. image:: https://github.com/noripyt/django-cachalot/actions/workflows/ci.yml/badge.svg
+   :target: https://github.com/noripyt/django-cachalot/actions/workflows/ci.yml
 
 .. image:: http://img.shields.io/coveralls/noripyt/django-cachalot/master.svg?style=flat-square&maxAge=3600
    :target: https://coveralls.io/r/noripyt/django-cachalot?branch=master
 
 .. image:: http://img.shields.io/scrutinizer/g/noripyt/django-cachalot/master.svg?style=flat-square&maxAge=3600
    :target: https://scrutinizer-ci.com/g/noripyt/django-cachalot/
```

### Comparing `django-cachalot-2.5.3/docs/introduction.rst` & `django-cachalot-2.6.0/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.5.3/docs/legacy.rst` & `django-cachalot-2.6.0/docs/legacy.rst`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.5.3/docs/limits.rst` & `django-cachalot-2.6.0/docs/limits.rst`

 * *Files 2% similar despite different names*

```diff
@@ -61,19 +61,17 @@
 Locmem is a just a ``dict`` stored in a single Python process.
 It’s not shared between processes, so don’t use locmem with django-cachalot
 in a multi-processes project, if you use RQ or Celery for instance.
 
 Filebased
 .........
 
-Filebased, a simple persistent cache implemented in Django, has a small bug
+Filebased, a simple persistent cache implemented in Django, had a small bug
 (`#25501 <https://code.djangoproject.com/ticket/25501>`_):
-it cannot cache some objects, like psycopg2 ranges.
-If you use range fields from `django.contrib.postgres` and your Django
-version is affected by this bug, you need to add the tables using range fields
+it cannot cache some objects, like psycopg2 ranges. This bug was fixed in 2015, if you sill use an affected Django version and you use range fields from `django.contrib.postgres`, you need to add the tables using range fields
 to :ref:`CACHALOT_UNCACHABLE_TABLES`.
 
 .. _MySQL:
 
 MySQL
 .....
```

### Comparing `django-cachalot-2.5.3/docs/quickstart.rst` & `django-cachalot-2.6.0/docs/quickstart.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Quick start
 -----------
 
 Requirements
 ............
 
-- Django 2.2, 3.2, 4.0-4.1
-- Python 3.7-3.10
+- Django 3.2, 4.1, 4.2
+- Python 3.7-3.11
 - a cache configured as ``'default'`` with one of these backends:
 
   - `django-redis <https://github.com/niwinz/django-redis>`_
   - `memcached <https://docs.djangoproject.com/en/dev/topics/cache/#memcached>`_
     (using either python-memcached or pylibmc)
   - `filebased <https://docs.djangoproject.com/en/dev/topics/cache/#filesystem-caching>`_
   - `locmem <https://docs.djangoproject.com/en/dev/topics/cache/#local-memory-caching>`_
```

### Comparing `django-cachalot-2.5.3/docs/reporting.rst` & `django-cachalot-2.6.0/docs/reporting.rst`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.5.3/docs/todo.rst` & `django-cachalot-2.6.0/docs/todo.rst`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.5.3/settings.py` & `django-cachalot-2.6.0/settings.py`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.5.3/setup.py` & `django-cachalot-2.6.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,23 +21,23 @@
     long_description=open('README.rst').read(),
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Framework :: Django',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',
         'Operating System :: OS Independent',
-        'Framework :: Django :: 2.2',
         'Framework :: Django :: 3.2',
-        'Framework :: Django :: 4.0',
         'Framework :: Django :: 4.1',
+        'Framework :: Django :: 4.2',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Internet :: WWW/HTTP',
     ],
     license='BSD',
     packages=find_packages(),
     install_requires=required,
     include_package_data=True,
     zip_safe=False,
```

