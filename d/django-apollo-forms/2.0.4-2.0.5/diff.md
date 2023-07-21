# Comparing `tmp/django-apollo-forms-2.0.4.tar.gz` & `tmp/django-apollo-forms-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-apollo-forms-2.0.4.tar", last modified: Wed May  3 14:00:33 2023, max compression
+gzip compressed data, was "django-apollo-forms-2.0.5.tar", last modified: Fri Jul 21 19:23:34 2023, max compression
```

## Comparing `django-apollo-forms-2.0.4.tar` & `django-apollo-forms-2.0.5.tar`

### file list

```diff
@@ -1,67 +1,68 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 14:00:33.103440 django-apollo-forms-2.0.4/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      328 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8303 2023-05-03 14:00:33.103440 django-apollo-forms-2.0.4/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6387 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 14:00:33.095440 django-apollo-forms-2.0.4/apollo/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      135 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      406 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/admin.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 14:00:33.095440 django-apollo-forms-2.0.4/apollo/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      241 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/api/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 14:00:33.095440 django-apollo-forms-2.0.4/apollo/api/v1/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/api/v1/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6983 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/api/v1/api_views.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      676 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/api/v1/permissions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6130 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/api/v1/serializers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      878 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/api/v1/urls.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      279 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/apps.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      135 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/exceptions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1116 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/factories.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1667 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/forms.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 14:00:33.095440 django-apollo-forms-2.0.4/apollo/lib/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/lib/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      724 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/lib/emails.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1411 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/lib/recaptcha.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 14:00:33.095440 django-apollo-forms-2.0.4/apollo/migrations/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7912 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/migrations/0001_initial.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1129 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/migrations/0002_auto_20180214_2053.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      513 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/migrations/0003_externalwebhook_service.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1122 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/migrations/0004_auto_20220816_2013.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2286 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/migrations/0005_alter_apiuser_id_alter_externalwebhook_id_and_more.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      680 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/migrations/0006_formfield_validation_message_and_more.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/migrations/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16608 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/models.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3287 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/settings.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2113 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/signals.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 14:00:33.095440 django-apollo-forms-2.0.4/apollo/static/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 14:00:33.095440 django-apollo-forms-2.0.4/apollo/static/build/
--rw-r--r--   0 circleci  (1001) circleci  (1002)  2688857 2023-05-03 13:59:54.000000 django-apollo-forms-2.0.4/apollo/static/build/app.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 14:00:33.099440 django-apollo-forms-2.0.4/apollo/static/images/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      778 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/static/images/grid-cell-bg.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4635 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/static/images/logo.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)   799937 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/static/package-lock.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1356 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/static/package.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 14:00:33.091440 django-apollo-forms-2.0.4/apollo/static/src/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 14:00:33.091440 django-apollo-forms-2.0.4/apollo/static/src/js/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 14:00:33.099440 django-apollo-forms-2.0.4/apollo/static/src/js/vendor/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    86659 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/static/src/js/vendor/jquery-3.2.1.min.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1494 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/static/webpack.config.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 14:00:33.099440 django-apollo-forms-2.0.4/apollo/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1416 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/templates/forms_manager.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1271 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/templates/noscript.html
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 14:00:33.099440 django-apollo-forms-2.0.4/apollo/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    25799 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/tests/test_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5029 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/tests/test_forms.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1959 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/tests/test_lib.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15470 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/tests/test_models.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1790 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/tests/test_signals.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1169 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/urls.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3471 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/views.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 14:00:33.099440 django-apollo-forms-2.0.4/django_apollo_forms.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8303 2023-05-03 14:00:33.000000 django-apollo-forms-2.0.4/django_apollo_forms.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1465 2023-05-03 14:00:33.000000 django-apollo-forms-2.0.4/django_apollo_forms.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-03 14:00:33.000000 django-apollo-forms-2.0.4/django_apollo_forms.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       76 2023-05-03 14:00:33.000000 django-apollo-forms-2.0.4/django_apollo_forms.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       74 2023-05-03 14:00:33.000000 django-apollo-forms-2.0.4/django_apollo_forms.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-05-03 14:00:33.103440 django-apollo-forms-2.0.4/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1748 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 19:23:34.192771 django-apollo-forms-2.0.5/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      328 2023-07-21 19:22:11.000000 django-apollo-forms-2.0.5/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7305 2023-07-21 19:23:34.192771 django-apollo-forms-2.0.5/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6387 2023-07-21 19:22:11.000000 django-apollo-forms-2.0.5/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 19:23:34.184771 django-apollo-forms-2.0.5/apollo/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      135 2023-07-21 19:22:11.000000 django-apollo-forms-2.0.5/apollo/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      406 2023-07-21 19:22:11.000000 django-apollo-forms-2.0.5/apollo/admin.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 19:23:34.184771 django-apollo-forms-2.0.5/apollo/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      241 2023-07-21 19:22:11.000000 django-apollo-forms-2.0.5/apollo/api/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 19:23:34.184771 django-apollo-forms-2.0.5/apollo/api/v1/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-21 19:22:11.000000 django-apollo-forms-2.0.5/apollo/api/v1/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6983 2023-07-21 19:22:11.000000 django-apollo-forms-2.0.5/apollo/api/v1/api_views.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      676 2023-07-21 19:22:11.000000 django-apollo-forms-2.0.5/apollo/api/v1/permissions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6130 2023-07-21 19:22:11.000000 django-apollo-forms-2.0.5/apollo/api/v1/serializers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      878 2023-07-21 19:22:11.000000 django-apollo-forms-2.0.5/apollo/api/v1/urls.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      279 2023-07-21 19:22:11.000000 django-apollo-forms-2.0.5/apollo/apps.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      135 2023-07-21 19:22:11.000000 django-apollo-forms-2.0.5/apollo/exceptions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1116 2023-07-21 19:22:11.000000 django-apollo-forms-2.0.5/apollo/factories.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1667 2023-07-21 19:22:11.000000 django-apollo-forms-2.0.5/apollo/forms.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 19:23:34.184771 django-apollo-forms-2.0.5/apollo/lib/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-21 19:22:11.000000 django-apollo-forms-2.0.5/apollo/lib/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      724 2023-07-21 19:22:11.000000 django-apollo-forms-2.0.5/apollo/lib/emails.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1411 2023-07-21 19:22:11.000000 django-apollo-forms-2.0.5/apollo/lib/recaptcha.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 19:23:34.184771 django-apollo-forms-2.0.5/apollo/migrations/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7912 2023-07-21 19:22:11.000000 django-apollo-forms-2.0.5/apollo/migrations/0001_initial.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1129 2023-07-21 19:22:11.000000 django-apollo-forms-2.0.5/apollo/migrations/0002_auto_20180214_2053.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      513 2023-07-21 19:22:11.000000 django-apollo-forms-2.0.5/apollo/migrations/0003_externalwebhook_service.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1122 2023-07-21 19:22:11.000000 django-apollo-forms-2.0.5/apollo/migrations/0004_auto_20220816_2013.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2286 2023-07-21 19:22:11.000000 django-apollo-forms-2.0.5/apollo/migrations/0005_alter_apiuser_id_alter_externalwebhook_id_and_more.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      680 2023-07-21 19:22:11.000000 django-apollo-forms-2.0.5/apollo/migrations/0006_formfield_validation_message_and_more.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      661 2023-07-21 19:22:11.000000 django-apollo-forms-2.0.5/apollo/migrations/0007_alter_formfield_default_value_and_more.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-21 19:22:11.000000 django-apollo-forms-2.0.5/apollo/migrations/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16608 2023-07-21 19:22:11.000000 django-apollo-forms-2.0.5/apollo/models.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3287 2023-07-21 19:22:11.000000 django-apollo-forms-2.0.5/apollo/settings.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2113 2023-07-21 19:22:11.000000 django-apollo-forms-2.0.5/apollo/signals.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 19:23:34.188771 django-apollo-forms-2.0.5/apollo/static/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 19:23:34.188771 django-apollo-forms-2.0.5/apollo/static/build/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)  2688857 2023-07-21 19:22:59.000000 django-apollo-forms-2.0.5/apollo/static/build/app.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 19:23:34.188771 django-apollo-forms-2.0.5/apollo/static/images/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      778 2023-07-21 19:22:11.000000 django-apollo-forms-2.0.5/apollo/static/images/grid-cell-bg.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4635 2023-07-21 19:22:11.000000 django-apollo-forms-2.0.5/apollo/static/images/logo.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   799937 2023-07-21 19:22:11.000000 django-apollo-forms-2.0.5/apollo/static/package-lock.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1356 2023-07-21 19:22:11.000000 django-apollo-forms-2.0.5/apollo/static/package.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 19:23:34.180770 django-apollo-forms-2.0.5/apollo/static/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 19:23:34.180770 django-apollo-forms-2.0.5/apollo/static/src/js/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 19:23:34.188771 django-apollo-forms-2.0.5/apollo/static/src/js/vendor/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    86659 2023-07-21 19:22:11.000000 django-apollo-forms-2.0.5/apollo/static/src/js/vendor/jquery-3.2.1.min.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1494 2023-07-21 19:22:11.000000 django-apollo-forms-2.0.5/apollo/static/webpack.config.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 19:23:34.188771 django-apollo-forms-2.0.5/apollo/templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1416 2023-07-21 19:22:11.000000 django-apollo-forms-2.0.5/apollo/templates/forms_manager.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1271 2023-07-21 19:22:11.000000 django-apollo-forms-2.0.5/apollo/templates/noscript.html
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 19:23:34.192771 django-apollo-forms-2.0.5/apollo/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-21 19:22:11.000000 django-apollo-forms-2.0.5/apollo/tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25799 2023-07-21 19:22:11.000000 django-apollo-forms-2.0.5/apollo/tests/test_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5029 2023-07-21 19:22:11.000000 django-apollo-forms-2.0.5/apollo/tests/test_forms.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1959 2023-07-21 19:22:11.000000 django-apollo-forms-2.0.5/apollo/tests/test_lib.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15470 2023-07-21 19:22:11.000000 django-apollo-forms-2.0.5/apollo/tests/test_models.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1790 2023-07-21 19:22:11.000000 django-apollo-forms-2.0.5/apollo/tests/test_signals.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1169 2023-07-21 19:22:11.000000 django-apollo-forms-2.0.5/apollo/urls.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3471 2023-07-21 19:22:11.000000 django-apollo-forms-2.0.5/apollo/views.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 19:23:34.192771 django-apollo-forms-2.0.5/django_apollo_forms.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7305 2023-07-21 19:23:34.000000 django-apollo-forms-2.0.5/django_apollo_forms.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1530 2023-07-21 19:23:34.000000 django-apollo-forms-2.0.5/django_apollo_forms.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-21 19:23:34.000000 django-apollo-forms-2.0.5/django_apollo_forms.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       76 2023-07-21 19:23:34.000000 django-apollo-forms-2.0.5/django_apollo_forms.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       74 2023-07-21 19:23:34.000000 django-apollo-forms-2.0.5/django_apollo_forms.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-07-21 19:23:34.192771 django-apollo-forms-2.0.5/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1748 2023-07-21 19:22:11.000000 django-apollo-forms-2.0.5/setup.py
```

### Comparing `django-apollo-forms-2.0.4/PKG-INFO` & `django-apollo-forms-2.0.5/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,146 +1,122 @@
-Metadata-Version: 2.1
-Name: django-apollo-forms
-Version: 2.0.4
-Summary: Simple CMS for forms
-Home-page: https://morgan-and-morgan.github.io/apollo/
-Author: Morgan & Morgan Developers
-Author-email: developers@forthepeople.com
-License: BSD License
-Description: ### What Apollo Is
-        At [Morgan & Morgan](https://www.forthepeople.com/), the development team builds lots of forms. A lot. While most of the
-        heavy lifting for form management was done for us by the marketing platform, Hubspot, there were some major gaps that forced us to consider
-        a switch:
-        
-        1. Cost. Our Hubspot license was > $50,000 yearly where the only utility came from the form management tooling.
-        2. Lack of flexibility. While defining basic validation rules and field layouts was OK, doing anything more complex 
-        (e.g. email blacklists, geo-based submission filtering, etc.) was impossible. In fact, since their switch to React rendered
-        forms, [custom validation in a Hubspot form doesn't work at all](https://integrate.hubspot.com/t/integration-with-jquery-validator-customized-validation/1172/9).
-        3. Lack of control. The Hubspot JS library is 300kb+ in size before gzip and sets short-term cache expiration headers. Why? It's hard to say without access to the unminified source.  
-        ![more than 300kb](http://static.forthepeople.com/engineering/apollo/big_hubspot.png)
-        4. Lack of transparency. Hubspot provides Salesforce syncing out of the box. However, having a highly customized Salesforce Org,
-        our Hubspot sync process was anything but straightforward. 
-        
-        
-        With these problems in mind, we built **Apollo** as a solution. 
-        
-        Apollo is a Django application which - in conjunction with the [Icarus Javascript Library](https://github.com/Morgan-and-Morgan/icarus) -
-        aims to act as a plug-and-play solution for the busy engineer. In addition to providing a management interface for building
-        form fields, designing forms, and viewing form submissions, Apollo makes the assumption that it should make no assumptions about
-        domain specific requirements of the host application. Thus, it decouples form management from submission processing,
-        leaving the job of reacting to events within the host. To facilitate this architecture, Apollo opts for a Pub/Sub design, notifying listeners
-        on key events:
-        
-        * _form submitted_
-        * _form submission validated_
-        * _form submission error_
-        
-        See more details on signals in the [signals reference](https://morgan-and-morgan.github.io/apollo/signals)
-        
-        
-        ### Why Apollo
-        1. It is - and always will be - free and open source
-        2. Plug-and-play architecture
-        3. Utility in a wide variety of use case
-        4. Integration with native Django permissions, allowing for role assignment when delegating API / form builder access.
-        
-        
-        ### Installation
-        ```bash
-        pip install django-apollo-forms
-        
-        # add the App to the list of INSTALLED_APPS
-        INSTALLED_APPS = {
-          ...  
-          'django_filters',
-          'rest_framework',
-          'rest_framework_swagger', # optional, creates browsable API docs
-          'apollo',
-          ...
-        }
-        
-        # run the migrations to generate DB tables
-        python manage.py makemigrations apollo
-        python manage.py migrate apollo
-        
-        # collectstatic to generate the static files for the form builder interface
-        python manage.py collectstatic
-        ```
-        
-        
-        ### Customization
-        You can customize the behavior of Apollo by overriding the defaults of the `APOLLO` variable in your settings.py. Below
-        are the parameters which may be controlled in this setting.
-        
-        | Parameter                 | Default                                                         | Description                                                                       | 
-        | ------------------------- | --------------------------------------------------------------- | --------------------------------------------------------------------------------- |
-        | BUILDER_ROOT_PREFIX       | ""                                                              | The path at which the Apollo form builder is mounted in the host application      | 
-        | BUILDER_REQUIRES_IS_STAFF | True                                                            | If True, then only users with `is_staff` permissions can access the form builder  |
-        | DOWNLOAD_REQUIRES_IS_STAFF| True                                                            | If True, then only users with `is_staff` permissions can download form submissions|
-        | API_ROOT                  | /api                                                            | The path to the API root on the server                                            |
-        | API_VERSION               | v1                                                              | The Apollo API version                                                            |
-        | ICARUS_THEMES_URL         | //static.forthepeople.com/engineering/icarus/v1.0-latest/themes | Location where icarus themes are located                                          |
-        | SUBMISSION_EMAIL_FROM     | None                                                            | Email address to send submission notifications from                               |
-        | EXTERNAL_HOOKS_SIGNAL_ONLY| True                                                            | If True, then we we do not send webhooks notifications, only trigger a signal     |
-        
-        *Example*
-        ```python
-        APOLLO = {
-            "BUILDER_ROOT_PREFIX": "/apollo"
-        }
-        ```
-        
-        
-        ### Features
-        
-        ###### Setup field templates for your forms. These define the default configurations for fields and can be overridden on a per-form basis. 
-        ![](http://static.forthepeople.com/engineering/apollo/feature_create_field-min.png)
-        
-        ---
-        
-        ###### Step-by-step form builder interface.
-        ![](http://static.forthepeople.com/engineering/apollo/feature_create_form_step_1-min.png)
-        
-        ---
-        
-        ###### Powerful layout creator with the ability to apply different layouts for desktop and mobile screens.
-        ![](http://static.forthepeople.com/engineering/apollo/feature_build_layouts-min.png)
-        
-        ---
-        
-        
-        ### Form Usage
-        When it comes to actually using the forms built by Apollo, you have two options:
-         
-        1. Use the [Icarus Javascript Library](https://github.com/Morgan-and-Morgan/icarus) (_Recommended_)
-        2. DIY.
-        
-        If you decide to pursue (2), you'll want to consult the Browsable API, mounted at `/<API_ROOT>/<API_VERSION>/docs` for details on authentication, request format,
-        and available resources.
-        
-        ### Development
-        
-        #### Getting Started
-        
-        Bringing up a new dev environment should be fairly straightforward. Run `docker-compose up -d` to bring up a complete development
-        environment.
-        
-        #### Building Releases
-        
-        Create a virtualenv then run `pip install -r requirements.txt` in order to install versioning utilities. Run `bumpversion <SEMVER>`
-        to create a buildable version then push upstream to trigger CI.
-Platform: UNKNOWN
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Django
-Classifier: Framework :: Django :: 1.9
-Classifier: Framework :: Django :: 1.10
-Classifier: Framework :: Django :: 1.11
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Description-Content-Type: text/markdown
+### What Apollo Is
+At [Morgan & Morgan](https://www.forthepeople.com/), the development team builds lots of forms. A lot. While most of the
+heavy lifting for form management was done for us by the marketing platform, Hubspot, there were some major gaps that forced us to consider
+a switch:
+
+1. Cost. Our Hubspot license was > $50,000 yearly where the only utility came from the form management tooling.
+2. Lack of flexibility. While defining basic validation rules and field layouts was OK, doing anything more complex 
+(e.g. email blacklists, geo-based submission filtering, etc.) was impossible. In fact, since their switch to React rendered
+forms, [custom validation in a Hubspot form doesn't work at all](https://integrate.hubspot.com/t/integration-with-jquery-validator-customized-validation/1172/9).
+3. Lack of control. The Hubspot JS library is 300kb+ in size before gzip and sets short-term cache expiration headers. Why? It's hard to say without access to the unminified source.  
+![more than 300kb](http://static.forthepeople.com/engineering/apollo/big_hubspot.png)
+4. Lack of transparency. Hubspot provides Salesforce syncing out of the box. However, having a highly customized Salesforce Org,
+our Hubspot sync process was anything but straightforward. 
+
+
+With these problems in mind, we built **Apollo** as a solution. 
+
+Apollo is a Django application which - in conjunction with the [Icarus Javascript Library](https://github.com/Morgan-and-Morgan/icarus) -
+aims to act as a plug-and-play solution for the busy engineer. In addition to providing a management interface for building
+form fields, designing forms, and viewing form submissions, Apollo makes the assumption that it should make no assumptions about
+domain specific requirements of the host application. Thus, it decouples form management from submission processing,
+leaving the job of reacting to events within the host. To facilitate this architecture, Apollo opts for a Pub/Sub design, notifying listeners
+on key events:
+
+* _form submitted_
+* _form submission validated_
+* _form submission error_
+
+See more details on signals in the [signals reference](https://morgan-and-morgan.github.io/apollo/signals)
+
+
+### Why Apollo
+1. It is - and always will be - free and open source
+2. Plug-and-play architecture
+3. Utility in a wide variety of use case
+4. Integration with native Django permissions, allowing for role assignment when delegating API / form builder access.
+
+
+### Installation
+```bash
+pip install django-apollo-forms
+
+# add the App to the list of INSTALLED_APPS
+INSTALLED_APPS = {
+  ...  
+  'django_filters',
+  'rest_framework',
+  'rest_framework_swagger', # optional, creates browsable API docs
+  'apollo',
+  ...
+}
+
+# run the migrations to generate DB tables
+python manage.py makemigrations apollo
+python manage.py migrate apollo
+
+# collectstatic to generate the static files for the form builder interface
+python manage.py collectstatic
+```
+
+
+### Customization
+You can customize the behavior of Apollo by overriding the defaults of the `APOLLO` variable in your settings.py. Below
+are the parameters which may be controlled in this setting.
+
+| Parameter                 | Default                                                         | Description                                                                       | 
+| ------------------------- | --------------------------------------------------------------- | --------------------------------------------------------------------------------- |
+| BUILDER_ROOT_PREFIX       | ""                                                              | The path at which the Apollo form builder is mounted in the host application      | 
+| BUILDER_REQUIRES_IS_STAFF | True                                                            | If True, then only users with `is_staff` permissions can access the form builder  |
+| DOWNLOAD_REQUIRES_IS_STAFF| True                                                            | If True, then only users with `is_staff` permissions can download form submissions|
+| API_ROOT                  | /api                                                            | The path to the API root on the server                                            |
+| API_VERSION               | v1                                                              | The Apollo API version                                                            |
+| ICARUS_THEMES_URL         | //static.forthepeople.com/engineering/icarus/v1.0-latest/themes | Location where icarus themes are located                                          |
+| SUBMISSION_EMAIL_FROM     | None                                                            | Email address to send submission notifications from                               |
+| EXTERNAL_HOOKS_SIGNAL_ONLY| True                                                            | If True, then we we do not send webhooks notifications, only trigger a signal     |
+
+*Example*
+```python
+APOLLO = {
+    "BUILDER_ROOT_PREFIX": "/apollo"
+}
+```
+
+
+### Features
+
+###### Setup field templates for your forms. These define the default configurations for fields and can be overridden on a per-form basis. 
+![](http://static.forthepeople.com/engineering/apollo/feature_create_field-min.png)
+
+---
+
+###### Step-by-step form builder interface.
+![](http://static.forthepeople.com/engineering/apollo/feature_create_form_step_1-min.png)
+
+---
+
+###### Powerful layout creator with the ability to apply different layouts for desktop and mobile screens.
+![](http://static.forthepeople.com/engineering/apollo/feature_build_layouts-min.png)
+
+---
+
+
+### Form Usage
+When it comes to actually using the forms built by Apollo, you have two options:
+ 
+1. Use the [Icarus Javascript Library](https://github.com/Morgan-and-Morgan/icarus) (_Recommended_)
+2. DIY.
+
+If you decide to pursue (2), you'll want to consult the Browsable API, mounted at `/<API_ROOT>/<API_VERSION>/docs` for details on authentication, request format,
+and available resources.
+
+### Development
+
+#### Getting Started
+
+Bringing up a new dev environment should be fairly straightforward. Run `docker-compose up -d` to bring up a complete development
+environment.
+
+#### Building Releases
+
+Create a virtualenv then run `pip install -r requirements.txt` in order to install versioning utilities. Run `bumpversion <SEMVER>`
+to create a buildable version then push upstream to trigger CI.
```

### Comparing `django-apollo-forms-2.0.4/README.md` & `django-apollo-forms-2.0.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+Metadata-Version: 2.1
+Name: django-apollo-forms
+Version: 2.0.5
+Summary: Simple CMS for forms
+Home-page: https://morgan-and-morgan.github.io/apollo/
+Author: Morgan & Morgan Developers
+Author-email: developers@forthepeople.com
+License: BSD License
+Classifier: Environment :: Web Environment
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 1.9
+Classifier: Framework :: Django :: 1.10
+Classifier: Framework :: Django :: 1.11
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+Description-Content-Type: text/markdown
+
 ### What Apollo Is
 At [Morgan & Morgan](https://www.forthepeople.com/), the development team builds lots of forms. A lot. While most of the
 heavy lifting for form management was done for us by the marketing platform, Hubspot, there were some major gaps that forced us to consider
 a switch:
 
 1. Cost. Our Hubspot license was > $50,000 yearly where the only utility came from the form management tooling.
 2. Lack of flexibility. While defining basic validation rules and field layouts was OK, doing anything more complex 
@@ -115,8 +139,8 @@
 
 Bringing up a new dev environment should be fairly straightforward. Run `docker-compose up -d` to bring up a complete development
 environment.
 
 #### Building Releases
 
 Create a virtualenv then run `pip install -r requirements.txt` in order to install versioning utilities. Run `bumpversion <SEMVER>`
-to create a buildable version then push upstream to trigger CI.
+to create a buildable version then push upstream to trigger CI.
```

### Comparing `django-apollo-forms-2.0.4/apollo/api/v1/api_views.py` & `django-apollo-forms-2.0.5/apollo/api/v1/api_views.py`

 * *Files identical despite different names*

### Comparing `django-apollo-forms-2.0.4/apollo/api/v1/permissions.py` & `django-apollo-forms-2.0.5/apollo/api/v1/permissions.py`

 * *Files identical despite different names*

### Comparing `django-apollo-forms-2.0.4/apollo/api/v1/serializers.py` & `django-apollo-forms-2.0.5/apollo/api/v1/serializers.py`

 * *Files identical despite different names*

### Comparing `django-apollo-forms-2.0.4/apollo/api/v1/urls.py` & `django-apollo-forms-2.0.5/apollo/api/v1/urls.py`

 * *Files identical despite different names*

### Comparing `django-apollo-forms-2.0.4/apollo/factories.py` & `django-apollo-forms-2.0.5/apollo/factories.py`

 * *Files identical despite different names*

### Comparing `django-apollo-forms-2.0.4/apollo/forms.py` & `django-apollo-forms-2.0.5/apollo/forms.py`

 * *Files identical despite different names*

### Comparing `django-apollo-forms-2.0.4/apollo/lib/emails.py` & `django-apollo-forms-2.0.5/apollo/lib/emails.py`

 * *Files identical despite different names*

### Comparing `django-apollo-forms-2.0.4/apollo/lib/recaptcha.py` & `django-apollo-forms-2.0.5/apollo/lib/recaptcha.py`

 * *Files identical despite different names*

### Comparing `django-apollo-forms-2.0.4/apollo/migrations/0001_initial.py` & `django-apollo-forms-2.0.5/apollo/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-apollo-forms-2.0.4/apollo/migrations/0002_auto_20180214_2053.py` & `django-apollo-forms-2.0.5/apollo/migrations/0002_auto_20180214_2053.py`

 * *Files identical despite different names*

### Comparing `django-apollo-forms-2.0.4/apollo/migrations/0003_externalwebhook_service.py` & `django-apollo-forms-2.0.5/apollo/migrations/0003_externalwebhook_service.py`

 * *Files identical despite different names*

### Comparing `django-apollo-forms-2.0.4/apollo/migrations/0004_auto_20220816_2013.py` & `django-apollo-forms-2.0.5/apollo/migrations/0004_auto_20220816_2013.py`

 * *Files identical despite different names*

### Comparing `django-apollo-forms-2.0.4/apollo/migrations/0005_alter_apiuser_id_alter_externalwebhook_id_and_more.py` & `django-apollo-forms-2.0.5/apollo/migrations/0005_alter_apiuser_id_alter_externalwebhook_id_and_more.py`

 * *Files identical despite different names*

### Comparing `django-apollo-forms-2.0.4/apollo/migrations/0006_formfield_validation_message_and_more.py` & `django-apollo-forms-2.0.5/apollo/migrations/0006_formfield_validation_message_and_more.py`

 * *Files identical despite different names*

### Comparing `django-apollo-forms-2.0.4/apollo/models.py` & `django-apollo-forms-2.0.5/apollo/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -218,15 +218,15 @@
     name = models.CharField(max_length=100, unique=True)
     input_type = models.CharField(max_length=50, choices=FIELD_TYPES, default='text')
     is_visible = models.BooleanField(default=True)
 
     label = models.CharField(max_length=100, null=True, blank=True, default=None)
     label_position = models.CharField(max_length=50, choices=LABEL_POSITIONS, default=LABEL_TOP)
     placeholder = models.CharField(max_length=150, null=True, blank=True, default=None)
-    default_value = models.CharField(max_length=300, null=True, blank=True, default=None)
+    default_value = models.CharField(max_length=500, null=True, blank=True, default=None)
 
     value_choices = ArrayField(
         ArrayField(models.CharField(max_length=100), size=2),
         null=True,
         blank=True,
         default=None
     )
@@ -244,15 +244,15 @@
     """
     form = models.ForeignKey(Form, related_name='fields', on_delete=models.CASCADE)
     template = models.ForeignKey(FormFieldTemplate, related_name='instances', on_delete=models.CASCADE)
     layout = models.ForeignKey(LayoutField, null=True, blank=True, default=None, on_delete=models.SET_NULL)
 
     label = models.CharField(max_length=100, null=True, blank=True, default=None)
     label_position = models.CharField(max_length=50, null=True, blank=True, default=FormFieldTemplate.LABEL_TOP, choices=FormFieldTemplate.LABEL_POSITIONS)
-    default_value = models.CharField(max_length=300, null=True, blank=True, default=None)
+    default_value = models.CharField(max_length=500, null=True, blank=True, default=None)
     placeholder = models.CharField(max_length=150, null=True, blank=True, default=None)
 
     index = models.IntegerField(default=0)
 
     value_choices = ArrayField(
         ArrayField(models.CharField(max_length=100), size=2),
         null=True,
```

### Comparing `django-apollo-forms-2.0.4/apollo/settings.py` & `django-apollo-forms-2.0.5/apollo/settings.py`

 * *Files identical despite different names*

### Comparing `django-apollo-forms-2.0.4/apollo/signals.py` & `django-apollo-forms-2.0.5/apollo/signals.py`

 * *Files identical despite different names*

### Comparing `django-apollo-forms-2.0.4/apollo/static/build/app.js` & `django-apollo-forms-2.0.5/apollo/static/build/app.js`

 * *Files identical despite different names*

### Comparing `django-apollo-forms-2.0.4/apollo/static/images/grid-cell-bg.png` & `django-apollo-forms-2.0.5/apollo/static/images/grid-cell-bg.png`

 * *Files identical despite different names*

### Comparing `django-apollo-forms-2.0.4/apollo/static/images/logo.png` & `django-apollo-forms-2.0.5/apollo/static/images/logo.png`

 * *Files identical despite different names*

### Comparing `django-apollo-forms-2.0.4/apollo/static/package-lock.json` & `django-apollo-forms-2.0.5/apollo/static/package-lock.json`

 * *Files identical despite different names*

### Comparing `django-apollo-forms-2.0.4/apollo/static/package.json` & `django-apollo-forms-2.0.5/apollo/static/package.json`

 * *Files identical despite different names*

### Comparing `django-apollo-forms-2.0.4/apollo/static/src/js/vendor/jquery-3.2.1.min.js` & `django-apollo-forms-2.0.5/apollo/static/src/js/vendor/jquery-3.2.1.min.js`

 * *Files identical despite different names*

### Comparing `django-apollo-forms-2.0.4/apollo/static/webpack.config.js` & `django-apollo-forms-2.0.5/apollo/static/webpack.config.js`

 * *Files identical despite different names*

### Comparing `django-apollo-forms-2.0.4/apollo/templates/forms_manager.html` & `django-apollo-forms-2.0.5/apollo/templates/forms_manager.html`

 * *Files identical despite different names*

### Comparing `django-apollo-forms-2.0.4/apollo/templates/noscript.html` & `django-apollo-forms-2.0.5/apollo/templates/noscript.html`

 * *Files identical despite different names*

### Comparing `django-apollo-forms-2.0.4/apollo/tests/test_api.py` & `django-apollo-forms-2.0.5/apollo/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `django-apollo-forms-2.0.4/apollo/tests/test_forms.py` & `django-apollo-forms-2.0.5/apollo/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `django-apollo-forms-2.0.4/apollo/tests/test_lib.py` & `django-apollo-forms-2.0.5/apollo/tests/test_lib.py`

 * *Files identical despite different names*

### Comparing `django-apollo-forms-2.0.4/apollo/tests/test_models.py` & `django-apollo-forms-2.0.5/apollo/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django-apollo-forms-2.0.4/apollo/tests/test_signals.py` & `django-apollo-forms-2.0.5/apollo/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `django-apollo-forms-2.0.4/apollo/urls.py` & `django-apollo-forms-2.0.5/apollo/urls.py`

 * *Files identical despite different names*

### Comparing `django-apollo-forms-2.0.4/apollo/views.py` & `django-apollo-forms-2.0.5/apollo/views.py`

 * *Files identical despite different names*

### Comparing `django-apollo-forms-2.0.4/django_apollo_forms.egg-info/SOURCES.txt` & `django-apollo-forms-2.0.5/django_apollo_forms.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 apollo/lib/recaptcha.py
 apollo/migrations/0001_initial.py
 apollo/migrations/0002_auto_20180214_2053.py
 apollo/migrations/0003_externalwebhook_service.py
 apollo/migrations/0004_auto_20220816_2013.py
 apollo/migrations/0005_alter_apiuser_id_alter_externalwebhook_id_and_more.py
 apollo/migrations/0006_formfield_validation_message_and_more.py
+apollo/migrations/0007_alter_formfield_default_value_and_more.py
 apollo/migrations/__init__.py
 apollo/static/package-lock.json
 apollo/static/package.json
 apollo/static/webpack.config.js
 apollo/static/build/app.js
 apollo/static/images/grid-cell-bg.png
 apollo/static/images/logo.png
```

### Comparing `django-apollo-forms-2.0.4/setup.py` & `django-apollo-forms-2.0.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 def get_packages(package):
     """
     Return root package and all sub-packages.
     """
     return [dirpath for dirpath, dirnames, filenames in os.walk(package) if os.path.exists(os.path.join(dirpath, '__init__.py'))]
 
 
-version = '2.0.4'
+version = '2.0.5'
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='django-apollo-forms',
     version=version,
```

