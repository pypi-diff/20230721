# Comparing `tmp/PyInventory-0.9.3rc4.tar.gz` & `tmp/PyInventory-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyInventory-0.9.3rc4.tar", max compression
+gzip compressed data, was "PyInventory-0.9.4.tar", max compression
```

## Comparing `PyInventory-0.9.3rc4.tar` & `PyInventory-0.9.4.tar`

### file list

```diff
@@ -1,69 +1,69 @@
--rw-r--r--   0        0        0      361 2020-10-26 17:13:43.715610 PyInventory-0.9.3rc4/AUTHORS
--rw-r--r--   0        0        0    35147 2020-10-15 15:54:51.000000 PyInventory-0.9.3rc4/LICENSE
--rw-r--r--   0        0        0     9848 2021-08-04 07:01:51.887683 PyInventory-0.9.3rc4/README.creole
--rw-r--r--   0        0        0    11859 2021-08-04 07:02:08.355594 PyInventory-0.9.3rc4/README.rst
--rw-r--r--   0        0        0     5537 2021-09-15 18:13:52.629546 PyInventory-0.9.3rc4/pyproject.toml
--rw-r--r--   0        0        0      387 2021-09-15 17:19:53.961818 PyInventory-0.9.3rc4/src/inventory/__init__.py
--rw-r--r--   0        0        0      120 2020-11-14 13:10:21.461293 PyInventory-0.9.3rc4/src/inventory/admin/__init__.py
--rw-r--r--   0        0        0      654 2020-12-20 17:46:40.147068 PyInventory-0.9.3rc4/src/inventory/admin/base.py
--rw-r--r--   0        0        0     4748 2021-09-15 17:42:05.051797 PyInventory-0.9.3rc4/src/inventory/admin/item.py
--rw-r--r--   0        0        0      731 2020-11-14 13:10:21.461293 PyInventory-0.9.3rc4/src/inventory/admin/location.py
--rw-r--r--   0        0        0      492 2020-11-14 13:10:21.461293 PyInventory-0.9.3rc4/src/inventory/apps.py
--rw-r--r--   0        0        0      391 2021-08-16 14:53:28.252959 PyInventory-0.9.3rc4/src/inventory/ckeditor_upload.py
--rw-r--r--   0        0        0      134 2020-11-14 13:10:21.465293 PyInventory-0.9.3rc4/src/inventory/context_processors.py
--rw-r--r--   0        0        0     1323 2020-12-20 17:45:04.743839 PyInventory-0.9.3rc4/src/inventory/forms.py
--rw-r--r--   0        0        0     5155 2021-04-28 17:01:37.190517 PyInventory-0.9.3rc4/src/inventory/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     5268 2021-04-28 17:01:37.190517 PyInventory-0.9.3rc4/src/inventory/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4322 2021-04-28 17:01:37.190517 PyInventory-0.9.3rc4/src/inventory/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     4575 2021-04-28 17:01:37.190517 PyInventory-0.9.3rc4/src/inventory/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2020-11-14 13:10:21.465293 PyInventory-0.9.3rc4/src/inventory/management/__init__.py
--rw-r--r--   0        0        0        0 2020-11-14 13:10:21.465293 PyInventory-0.9.3rc4/src/inventory/management/commands/__init__.py
--rw-r--r--   0        0        0      982 2021-08-04 07:07:28.792505 PyInventory-0.9.3rc4/src/inventory/management/commands/run_testserver.py
--rw-r--r--   0        0        0      530 2020-12-20 17:31:46.482424 PyInventory-0.9.3rc4/src/inventory/middlewares.py
--rw-r--r--   0        0        0    15321 2020-11-14 13:10:21.465293 PyInventory-0.9.3rc4/src/inventory/migrations/0001_initial.py
--rw-r--r--   0        0        0     2215 2020-11-14 13:10:21.465293 PyInventory-0.9.3rc4/src/inventory/migrations/0002_auto_20201017_2211.py
--rw-r--r--   0        0        0      568 2020-11-14 13:10:21.465293 PyInventory-0.9.3rc4/src/inventory/migrations/0003_auto_20201024_1830.py
--rw-r--r--   0        0        0     3352 2020-11-15 11:09:40.199344 PyInventory-0.9.3rc4/src/inventory/migrations/0004_item_user_images.py
--rw-r--r--   0        0        0     2105 2020-12-07 18:14:45.124794 PyInventory-0.9.3rc4/src/inventory/migrations/0005_serve_uploads_by_django_tools.py
--rw-r--r--   0        0        0     1422 2021-04-28 17:01:37.190517 PyInventory-0.9.3rc4/src/inventory/migrations/0006_refactor_image_model.py
--rw-r--r--   0        0        0     3389 2021-04-28 17:01:37.190517 PyInventory-0.9.3rc4/src/inventory/migrations/0007_add_file_attachment.py
--rw-r--r--   0        0        0        0 2020-11-14 13:10:21.465293 PyInventory-0.9.3rc4/src/inventory/migrations/__init__.py
--rw-r--r--   0        0        0      143 2020-11-15 11:04:52.098002 PyInventory-0.9.3rc4/src/inventory/models/__init__.py
--rw-r--r--   0        0        0     2266 2021-08-16 14:53:28.252959 PyInventory-0.9.3rc4/src/inventory/models/base.py
--rw-r--r--   0        0        0     7406 2021-08-16 14:53:28.252959 PyInventory-0.9.3rc4/src/inventory/models/item.py
--rw-r--r--   0        0        0     2694 2021-05-10 17:14:04.484973 PyInventory-0.9.3rc4/src/inventory/models/links.py
--rw-r--r--   0        0        0     1048 2020-11-14 13:10:21.469292 PyInventory-0.9.3rc4/src/inventory/models/location.py
--rw-r--r--   0        0        0     1218 2020-11-15 11:06:27.245044 PyInventory-0.9.3rc4/src/inventory/permissions.py
--rw-r--r--   0        0        0      288 2020-11-14 13:10:21.469292 PyInventory-0.9.3rc4/src/inventory/request_dict.py
--rw-r--r--   0        0        0      537 2020-11-14 13:10:21.469292 PyInventory-0.9.3rc4/src/inventory/signals.py
--rw-r--r--   0        0        0      177 2020-11-14 13:10:21.469292 PyInventory-0.9.3rc4/src/inventory/static/inventory.css
--rw-r--r--   0        0        0      258 2020-11-14 13:10:21.469292 PyInventory-0.9.3rc4/src/inventory/templates/admin/inventory/item/column_item.html
--rw-r--r--   0        0        0        0 2020-11-15 12:17:05.696891 PyInventory-0.9.3rc4/src/inventory/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-11-15 12:19:26.763628 PyInventory-0.9.3rc4/src/inventory/tests/fixtures/__init__.py
--rw-r--r--   0        0        0      482 2020-11-15 13:24:13.459824 PyInventory-0.9.3rc4/src/inventory/tests/fixtures/users.py
--rw-r--r--   0        0        0     2906 2020-12-07 09:16:53.783161 PyInventory-0.9.3rc4/src/inventory/tests/test_item_images.py
--rw-r--r--   0        0        0        0 2021-04-05 13:22:58.396867 PyInventory-0.9.3rc4/src/inventory_project/__init__.py
--rw-r--r--   0        0        0     8002 2021-08-04 07:16:09.440053 PyInventory-0.9.3rc4/src/inventory_project/dev_shell.py
--rw-r--r--   0        0        0     1208 2021-08-04 06:58:55.228667 PyInventory-0.9.3rc4/src/inventory_project/manage.py
--rw-r--r--   0        0        0      534 2020-11-14 13:10:21.469292 PyInventory-0.9.3rc4/src/inventory_project/middlewares.py
--rw-r--r--   0        0        0      938 2020-11-14 13:10:21.469292 PyInventory-0.9.3rc4/src/inventory_project/publish.py
--rw-r--r--   0        0        0        0 2020-11-14 13:06:22.000000 PyInventory-0.9.3rc4/src/inventory_project/settings/__init__.py
--rw-r--r--   0        0        0    10521 2021-09-15 17:28:02.462116 PyInventory-0.9.3rc4/src/inventory_project/settings/base.py
--rw-r--r--   0        0        0     2156 2021-04-28 17:04:48.128954 PyInventory-0.9.3rc4/src/inventory_project/settings/local.py
--rw-r--r--   0        0        0      235 2020-11-14 19:14:37.931280 PyInventory-0.9.3rc4/src/inventory_project/settings/tests.py
--rw-r--r--   0        0        0      715 2020-11-14 13:10:21.469292 PyInventory-0.9.3rc4/src/inventory_project/templates/admin/base_site.html
--rw-r--r--   0        0        0     1062 2020-11-14 13:10:21.469292 PyInventory-0.9.3rc4/src/inventory_project/templates/admin/login.html
--rw-r--r--   0        0        0        0 2020-11-14 13:10:21.469292 PyInventory-0.9.3rc4/src/inventory_project/tests/__init__.py
--rw-r--r--   0        0        0     1958 2021-04-28 17:04:48.128954 PyInventory-0.9.3rc4/src/inventory_project/tests/middleware.py
--rw-r--r--   0        0        0     4293 2020-12-20 17:46:05.819345 PyInventory-0.9.3rc4/src/inventory_project/tests/test_admin.py
--rw-r--r--   0        0        0     5251 2021-08-16 14:53:28.252959 PyInventory-0.9.3rc4/src/inventory_project/tests/test_admin_item.py
--rw-r--r--   0        0        0      873 2021-04-13 06:59:36.174871 PyInventory-0.9.3rc4/src/inventory_project/tests/test_bootstrap.py
--rw-r--r--   0        0        0     1279 2021-04-28 16:37:07.990424 PyInventory-0.9.3rc4/src/inventory_project/tests/test_inventory_commands.py
--rw-r--r--   0        0        0      357 2021-04-05 17:00:50.196709 PyInventory-0.9.3rc4/src/inventory_project/tests/test_lint.py
--rw-r--r--   0        0        0      688 2020-11-14 13:10:21.469292 PyInventory-0.9.3rc4/src/inventory_project/tests/test_migrations.py
--rw-r--r--   0        0        0     2677 2021-04-28 14:36:30.246140 PyInventory-0.9.3rc4/src/inventory_project/tests/test_project_setup.py
--rw-r--r--   0        0        0     1098 2021-08-04 07:15:17.924441 PyInventory-0.9.3rc4/src/inventory_project/tests/test_run_testserver.py
--rw-r--r--   0        0        0      792 2020-12-09 18:52:45.394878 PyInventory-0.9.3rc4/src/inventory_project/urls.py
--rw-r--r--   0        0        0      115 2020-11-14 13:10:21.469292 PyInventory-0.9.3rc4/src/inventory_project/wsgi.py
--rw-r--r--   0        0        0    14213 2021-09-15 18:13:55.940431 PyInventory-0.9.3rc4/setup.py
--rw-r--r--   0        0        0    13863 2021-09-15 18:13:55.941083 PyInventory-0.9.3rc4/PKG-INFO
+-rw-r--r--   0        0        0      361 2020-10-26 17:13:43.715610 PyInventory-0.9.4/AUTHORS
+-rw-r--r--   0        0        0    35147 2020-10-15 15:54:51.000000 PyInventory-0.9.4/LICENSE
+-rw-r--r--   0        0        0    10249 2021-09-15 19:28:39.468039 PyInventory-0.9.4/README.creole
+-rw-r--r--   0        0        0    12331 2021-09-15 19:29:46.851536 PyInventory-0.9.4/README.rst
+-rw-r--r--   0        0        0     5646 2021-09-15 19:30:06.871386 PyInventory-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0      383 2021-09-15 19:28:39.476039 PyInventory-0.9.4/src/inventory/__init__.py
+-rw-r--r--   0        0        0      120 2020-11-14 13:10:21.461293 PyInventory-0.9.4/src/inventory/admin/__init__.py
+-rw-r--r--   0        0        0      654 2020-12-20 17:46:40.147068 PyInventory-0.9.4/src/inventory/admin/base.py
+-rw-r--r--   0        0        0     4748 2021-09-15 17:42:05.051797 PyInventory-0.9.4/src/inventory/admin/item.py
+-rw-r--r--   0        0        0      731 2020-11-14 13:10:21.461293 PyInventory-0.9.4/src/inventory/admin/location.py
+-rw-r--r--   0        0        0      492 2020-11-14 13:10:21.461293 PyInventory-0.9.4/src/inventory/apps.py
+-rw-r--r--   0        0        0      391 2021-08-16 14:53:28.252959 PyInventory-0.9.4/src/inventory/ckeditor_upload.py
+-rw-r--r--   0        0        0      134 2020-11-14 13:10:21.465293 PyInventory-0.9.4/src/inventory/context_processors.py
+-rw-r--r--   0        0        0     1323 2020-12-20 17:45:04.743839 PyInventory-0.9.4/src/inventory/forms.py
+-rw-r--r--   0        0        0     5155 2021-04-28 17:01:37.190517 PyInventory-0.9.4/src/inventory/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     5268 2021-04-28 17:01:37.190517 PyInventory-0.9.4/src/inventory/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4322 2021-04-28 17:01:37.190517 PyInventory-0.9.4/src/inventory/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     4575 2021-04-28 17:01:37.190517 PyInventory-0.9.4/src/inventory/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2020-11-14 13:10:21.465293 PyInventory-0.9.4/src/inventory/management/__init__.py
+-rw-r--r--   0        0        0        0 2020-11-14 13:10:21.465293 PyInventory-0.9.4/src/inventory/management/commands/__init__.py
+-rw-r--r--   0        0        0      982 2021-08-04 07:07:28.792505 PyInventory-0.9.4/src/inventory/management/commands/run_testserver.py
+-rw-r--r--   0        0        0      530 2020-12-20 17:31:46.482424 PyInventory-0.9.4/src/inventory/middlewares.py
+-rw-r--r--   0        0        0    15321 2020-11-14 13:10:21.465293 PyInventory-0.9.4/src/inventory/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2215 2020-11-14 13:10:21.465293 PyInventory-0.9.4/src/inventory/migrations/0002_auto_20201017_2211.py
+-rw-r--r--   0        0        0      568 2020-11-14 13:10:21.465293 PyInventory-0.9.4/src/inventory/migrations/0003_auto_20201024_1830.py
+-rw-r--r--   0        0        0     3352 2020-11-15 11:09:40.199344 PyInventory-0.9.4/src/inventory/migrations/0004_item_user_images.py
+-rw-r--r--   0        0        0     2105 2020-12-07 18:14:45.124794 PyInventory-0.9.4/src/inventory/migrations/0005_serve_uploads_by_django_tools.py
+-rw-r--r--   0        0        0     1422 2021-04-28 17:01:37.190517 PyInventory-0.9.4/src/inventory/migrations/0006_refactor_image_model.py
+-rw-r--r--   0        0        0     3389 2021-04-28 17:01:37.190517 PyInventory-0.9.4/src/inventory/migrations/0007_add_file_attachment.py
+-rw-r--r--   0        0        0        0 2020-11-14 13:10:21.465293 PyInventory-0.9.4/src/inventory/migrations/__init__.py
+-rw-r--r--   0        0        0      143 2020-11-15 11:04:52.098002 PyInventory-0.9.4/src/inventory/models/__init__.py
+-rw-r--r--   0        0        0     2266 2021-08-16 14:53:28.252959 PyInventory-0.9.4/src/inventory/models/base.py
+-rw-r--r--   0        0        0     7406 2021-08-16 14:53:28.252959 PyInventory-0.9.4/src/inventory/models/item.py
+-rw-r--r--   0        0        0     2694 2021-05-10 17:14:04.484973 PyInventory-0.9.4/src/inventory/models/links.py
+-rw-r--r--   0        0        0     1048 2020-11-14 13:10:21.469292 PyInventory-0.9.4/src/inventory/models/location.py
+-rw-r--r--   0        0        0     1218 2020-11-15 11:06:27.245044 PyInventory-0.9.4/src/inventory/permissions.py
+-rw-r--r--   0        0        0      288 2020-11-14 13:10:21.469292 PyInventory-0.9.4/src/inventory/request_dict.py
+-rw-r--r--   0        0        0      537 2020-11-14 13:10:21.469292 PyInventory-0.9.4/src/inventory/signals.py
+-rw-r--r--   0        0        0      177 2020-11-14 13:10:21.469292 PyInventory-0.9.4/src/inventory/static/inventory.css
+-rw-r--r--   0        0        0      258 2020-11-14 13:10:21.469292 PyInventory-0.9.4/src/inventory/templates/admin/inventory/item/column_item.html
+-rw-r--r--   0        0        0        0 2020-11-15 12:17:05.696891 PyInventory-0.9.4/src/inventory/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-11-15 12:19:26.763628 PyInventory-0.9.4/src/inventory/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0      482 2020-11-15 13:24:13.459824 PyInventory-0.9.4/src/inventory/tests/fixtures/users.py
+-rw-r--r--   0        0        0     2906 2020-12-07 09:16:53.783161 PyInventory-0.9.4/src/inventory/tests/test_item_images.py
+-rw-r--r--   0        0        0        0 2021-04-05 13:22:58.396867 PyInventory-0.9.4/src/inventory_project/__init__.py
+-rw-r--r--   0        0        0     8002 2021-08-04 07:16:09.440053 PyInventory-0.9.4/src/inventory_project/dev_shell.py
+-rw-r--r--   0        0        0     1208 2021-08-04 06:58:55.228667 PyInventory-0.9.4/src/inventory_project/manage.py
+-rw-r--r--   0        0        0      534 2020-11-14 13:10:21.469292 PyInventory-0.9.4/src/inventory_project/middlewares.py
+-rw-r--r--   0        0        0      938 2020-11-14 13:10:21.469292 PyInventory-0.9.4/src/inventory_project/publish.py
+-rw-r--r--   0        0        0        0 2020-11-14 13:06:22.000000 PyInventory-0.9.4/src/inventory_project/settings/__init__.py
+-rw-r--r--   0        0        0    10521 2021-09-15 17:28:02.462116 PyInventory-0.9.4/src/inventory_project/settings/base.py
+-rw-r--r--   0        0        0     2156 2021-04-28 17:04:48.128954 PyInventory-0.9.4/src/inventory_project/settings/local.py
+-rw-r--r--   0        0        0      235 2020-11-14 19:14:37.931280 PyInventory-0.9.4/src/inventory_project/settings/tests.py
+-rw-r--r--   0        0        0      715 2020-11-14 13:10:21.469292 PyInventory-0.9.4/src/inventory_project/templates/admin/base_site.html
+-rw-r--r--   0        0        0     1062 2020-11-14 13:10:21.469292 PyInventory-0.9.4/src/inventory_project/templates/admin/login.html
+-rw-r--r--   0        0        0        0 2020-11-14 13:10:21.469292 PyInventory-0.9.4/src/inventory_project/tests/__init__.py
+-rw-r--r--   0        0        0     1958 2021-04-28 17:04:48.128954 PyInventory-0.9.4/src/inventory_project/tests/middleware.py
+-rw-r--r--   0        0        0     4293 2020-12-20 17:46:05.819345 PyInventory-0.9.4/src/inventory_project/tests/test_admin.py
+-rw-r--r--   0        0        0     5251 2021-08-16 14:53:28.252959 PyInventory-0.9.4/src/inventory_project/tests/test_admin_item.py
+-rw-r--r--   0        0        0      873 2021-04-13 06:59:36.174871 PyInventory-0.9.4/src/inventory_project/tests/test_bootstrap.py
+-rw-r--r--   0        0        0     1279 2021-04-28 16:37:07.990424 PyInventory-0.9.4/src/inventory_project/tests/test_inventory_commands.py
+-rw-r--r--   0        0        0      357 2021-04-05 17:00:50.196709 PyInventory-0.9.4/src/inventory_project/tests/test_lint.py
+-rw-r--r--   0        0        0      688 2020-11-14 13:10:21.469292 PyInventory-0.9.4/src/inventory_project/tests/test_migrations.py
+-rw-r--r--   0        0        0     2677 2021-04-28 14:36:30.246140 PyInventory-0.9.4/src/inventory_project/tests/test_project_setup.py
+-rw-r--r--   0        0        0     1098 2021-08-04 07:15:17.924441 PyInventory-0.9.4/src/inventory_project/tests/test_run_testserver.py
+-rw-r--r--   0        0        0      792 2020-12-09 18:52:45.394878 PyInventory-0.9.4/src/inventory_project/urls.py
+-rw-r--r--   0        0        0      115 2020-11-14 13:10:21.469292 PyInventory-0.9.4/src/inventory_project/wsgi.py
+-rw-r--r--   0        0        0    14702 2021-09-15 19:30:10.713269 PyInventory-0.9.4/setup.py
+-rw-r--r--   0        0        0    14346 2021-09-15 19:30:10.713817 PyInventory-0.9.4/PKG-INFO
```

### Comparing `PyInventory-0.9.3rc4/LICENSE` & `PyInventory-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `PyInventory-0.9.3rc4/README.creole` & `PyInventory-0.9.4/README.creole`

 * *Files 2% similar despite different names*

```diff
@@ -152,16 +152,22 @@
 
 Git branches "master" and "deployment" was merged into one.
 Files are separated into: "/src/" and "/development/"
 
 
 == history
 
-* [[https://github.com/jedie/PyInventory/compare/v0.9.2...master|compare v0.9.2...master]] **dev**
+* [[https://github.com/jedie/PyInventory/compare/v0.9.4...master|compare v0.9.4...master]] **dev**
 ** tbc
+* [[https://github.com/jedie/PyInventory/compare/v0.9.3...v0.9.4|v0.9.4 - 15.09.2021]]
+** Pin {{{psycopg < 2.9}}} because of https://github.com/psycopg/psycopg2/issues/1293
+* [[https://github.com/jedie/PyInventory/compare/v0.9.2...v0.9.3|v0.9.3 - 15.09.2021]]
+** Optimize "items" changelist queries
+** Update requirements
+** Expand {{{run_testserver}}} command and recognize address and port argument
 * [[https://github.com/jedie/PyInventory/compare/v0.9.1...v0.9.2|v0.9.2 - 11.05.2021]]
 ** Update requirements
 ** [[https://github.com/jedie/PyInventory/issues/50|Fix error handling if item link is broken]]
 * [[https://github.com/jedie/PyInventory/compare/v0.9.0...v0.9.1|v0.9.1 - 28.04.2021]]
 * NEW: Besides images, it's now possible to add file(s) to items, too.
 * Add a auto login if Django dev. server is used.
 * [[https://github.com/jedie/PyInventory/compare/v0.8.4...v0.9.0|v0.9.0 - 11.04.2021]]
```

### Comparing `PyInventory-0.9.3rc4/README.rst` & `PyInventory-0.9.4/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -214,18 +214,30 @@
 Git branches "master" and "deployment" was merged into one.
 Files are separated into: "/src/" and "/development/"
 
 -------
 history
 -------
 
-* `compare v0.9.2...master <https://github.com/jedie/PyInventory/compare/v0.9.2...master>`_ **dev** 
+* `compare v0.9.4...master <https://github.com/jedie/PyInventory/compare/v0.9.4...master>`_ **dev** 
 
     * tbc
 
+* `v0.9.4 - 15.09.2021 <https://github.com/jedie/PyInventory/compare/v0.9.3...v0.9.4>`_ 
+
+    * Pin ``psycopg < 2.9`` because of `https://github.com/psycopg/psycopg2/issues/1293 <https://github.com/psycopg/psycopg2/issues/1293>`_
+
+* `v0.9.3 - 15.09.2021 <https://github.com/jedie/PyInventory/compare/v0.9.2...v0.9.3>`_ 
+
+    * Optimize "items" changelist queries
+
+    * Update requirements
+
+    * Expand ``run_testserver`` command and recognize address and port argument
+
 * `v0.9.2 - 11.05.2021 <https://github.com/jedie/PyInventory/compare/v0.9.1...v0.9.2>`_ 
 
     * Update requirements
 
     * `Fix error handling if item link is broken <https://github.com/jedie/PyInventory/issues/50>`_
 
 * `v0.9.1 - 28.04.2021 <https://github.com/jedie/PyInventory/compare/v0.9.0...v0.9.1>`_
@@ -385,8 +397,8 @@
 
 * `Flattr This! <https://flattr.com/submit/auto?uid=jedie&url=https%3A%2F%2Fgithub.com%2Fjedie%2FPyInventory%2F>`_
 
 * Send `Bitcoins <http://www.bitcoin.org/>`_ to `1823RZ5Md1Q2X5aSXRC5LRPcYdveCiVX6F <https://blockexplorer.com/address/1823RZ5Md1Q2X5aSXRC5LRPcYdveCiVX6F>`_
 
 ------------
 
-``Note: this file is generated from README.creole 2021-08-04 09:01:51 with "python-creole"``
+``Note: this file is generated from README.creole 2021-09-15 21:28:39 with "python-creole"``
```

### Comparing `PyInventory-0.9.3rc4/pyproject.toml` & `PyInventory-0.9.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PyInventory"
-version = "0.9.3.rc4"
+version = "0.9.4"
 description = "Web based management to catalog things including state and location etc. using Python/Django."
 authors = ["JensDiemer <git@jensdiemer.de>"]
 homepage = "https://github.com/jedie/PyInventory"
 packages = [
     { include = "inventory", from = "src" },
     { include = "inventory_project", from = "src" },
 ]
@@ -49,19 +49,24 @@
 django-ckeditor = "*"  # https://github.com/django-ckeditor/django-ckeditor
 bx_py_utils = "*"  # https://github.com/boxine/bx_py_utils
 bx_django_utils = "*"  # https://github.com/boxine/bx_django_utils
 django-tagulous = "*"  # https://github.com/radiac/django-tagulous
 django-admin-sortable2 = "*"  # https://github.com/jrief/django-admin-sortable2
 django-axes = "*"  # https://github.com/jazzband/django-axes
 requests = "*"  # https://github.com/psf/requests
-docker-compose = { version = "*", optional = true }  # install via: poetry install --extras "docker"
-psycopg2-binary = { version = "*", optional = true }  # install via: poetry install --extras "postgres-binary"
-psycopg2 = { version = "*", optional = true }  # install via: poetry install --extras "psycopg2-source"
 pillow = "*"
 
+docker-compose = { version = "*", optional = true }  # install via: poetry install --extras "docker"
+
+# TODO: Update psycopg2 after Django >2.2 update
+# See: https://github.com/psycopg/psycopg2/issues/1293
+psycopg2-binary = { version = "<2.9", optional = true }  # install via: poetry install --extras "postgres-binary"
+psycopg2 = { version = "<2.9", optional = true }  # install via: poetry install --extras "psycopg2-source"
+
+
 [tool.poetry.extras]
 docker = ["docker-compose"]
 postgres-binary = ["psycopg2-binary"]
 psycopg2-source = ["psycopg2"]
 
 [tool.poetry.dev-dependencies]
 dev_shell = ">=0.2.2"  # https://github.com/jedie/dev-shell
```

### Comparing `PyInventory-0.9.3rc4/src/inventory/admin/base.py` & `PyInventory-0.9.4/src/inventory/admin/base.py`

 * *Files identical despite different names*

### Comparing `PyInventory-0.9.3rc4/src/inventory/admin/item.py` & `PyInventory-0.9.4/src/inventory/admin/item.py`

 * *Files identical despite different names*

### Comparing `PyInventory-0.9.3rc4/src/inventory/admin/location.py` & `PyInventory-0.9.4/src/inventory/admin/location.py`

 * *Files identical despite different names*

### Comparing `PyInventory-0.9.3rc4/src/inventory/forms.py` & `PyInventory-0.9.4/src/inventory/forms.py`

 * *Files identical despite different names*

### Comparing `PyInventory-0.9.3rc4/src/inventory/locale/de/LC_MESSAGES/django.mo` & `PyInventory-0.9.4/src/inventory/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `PyInventory-0.9.3rc4/src/inventory/locale/de/LC_MESSAGES/django.po` & `PyInventory-0.9.4/src/inventory/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `PyInventory-0.9.3rc4/src/inventory/locale/en/LC_MESSAGES/django.mo` & `PyInventory-0.9.4/src/inventory/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `PyInventory-0.9.3rc4/src/inventory/locale/en/LC_MESSAGES/django.po` & `PyInventory-0.9.4/src/inventory/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `PyInventory-0.9.3rc4/src/inventory/management/commands/run_testserver.py` & `PyInventory-0.9.4/src/inventory/management/commands/run_testserver.py`

 * *Files identical despite different names*

### Comparing `PyInventory-0.9.3rc4/src/inventory/middlewares.py` & `PyInventory-0.9.4/src/inventory/middlewares.py`

 * *Files identical despite different names*

### Comparing `PyInventory-0.9.3rc4/src/inventory/migrations/0001_initial.py` & `PyInventory-0.9.4/src/inventory/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `PyInventory-0.9.3rc4/src/inventory/migrations/0002_auto_20201017_2211.py` & `PyInventory-0.9.4/src/inventory/migrations/0002_auto_20201017_2211.py`

 * *Files identical despite different names*

### Comparing `PyInventory-0.9.3rc4/src/inventory/migrations/0003_auto_20201024_1830.py` & `PyInventory-0.9.4/src/inventory/migrations/0003_auto_20201024_1830.py`

 * *Files identical despite different names*

### Comparing `PyInventory-0.9.3rc4/src/inventory/migrations/0004_item_user_images.py` & `PyInventory-0.9.4/src/inventory/migrations/0004_item_user_images.py`

 * *Files identical despite different names*

### Comparing `PyInventory-0.9.3rc4/src/inventory/migrations/0005_serve_uploads_by_django_tools.py` & `PyInventory-0.9.4/src/inventory/migrations/0005_serve_uploads_by_django_tools.py`

 * *Files identical despite different names*

### Comparing `PyInventory-0.9.3rc4/src/inventory/migrations/0006_refactor_image_model.py` & `PyInventory-0.9.4/src/inventory/migrations/0006_refactor_image_model.py`

 * *Files identical despite different names*

### Comparing `PyInventory-0.9.3rc4/src/inventory/migrations/0007_add_file_attachment.py` & `PyInventory-0.9.4/src/inventory/migrations/0007_add_file_attachment.py`

 * *Files identical despite different names*

### Comparing `PyInventory-0.9.3rc4/src/inventory/models/base.py` & `PyInventory-0.9.4/src/inventory/models/base.py`

 * *Files identical despite different names*

### Comparing `PyInventory-0.9.3rc4/src/inventory/models/item.py` & `PyInventory-0.9.4/src/inventory/models/item.py`

 * *Files identical despite different names*

### Comparing `PyInventory-0.9.3rc4/src/inventory/models/links.py` & `PyInventory-0.9.4/src/inventory/models/links.py`

 * *Files identical despite different names*

### Comparing `PyInventory-0.9.3rc4/src/inventory/models/location.py` & `PyInventory-0.9.4/src/inventory/models/location.py`

 * *Files identical despite different names*

### Comparing `PyInventory-0.9.3rc4/src/inventory/permissions.py` & `PyInventory-0.9.4/src/inventory/permissions.py`

 * *Files identical despite different names*

### Comparing `PyInventory-0.9.3rc4/src/inventory/signals.py` & `PyInventory-0.9.4/src/inventory/signals.py`

 * *Files identical despite different names*

### Comparing `PyInventory-0.9.3rc4/src/inventory/tests/test_item_images.py` & `PyInventory-0.9.4/src/inventory/tests/test_item_images.py`

 * *Files identical despite different names*

### Comparing `PyInventory-0.9.3rc4/src/inventory_project/dev_shell.py` & `PyInventory-0.9.4/src/inventory_project/dev_shell.py`

 * *Files identical despite different names*

### Comparing `PyInventory-0.9.3rc4/src/inventory_project/manage.py` & `PyInventory-0.9.4/src/inventory_project/manage.py`

 * *Files identical despite different names*

### Comparing `PyInventory-0.9.3rc4/src/inventory_project/middlewares.py` & `PyInventory-0.9.4/src/inventory_project/middlewares.py`

 * *Files identical despite different names*

### Comparing `PyInventory-0.9.3rc4/src/inventory_project/publish.py` & `PyInventory-0.9.4/src/inventory_project/publish.py`

 * *Files identical despite different names*

### Comparing `PyInventory-0.9.3rc4/src/inventory_project/settings/base.py` & `PyInventory-0.9.4/src/inventory_project/settings/base.py`

 * *Files identical despite different names*

### Comparing `PyInventory-0.9.3rc4/src/inventory_project/settings/local.py` & `PyInventory-0.9.4/src/inventory_project/settings/local.py`

 * *Files identical despite different names*

### Comparing `PyInventory-0.9.3rc4/src/inventory_project/templates/admin/base_site.html` & `PyInventory-0.9.4/src/inventory_project/templates/admin/base_site.html`

 * *Files identical despite different names*

### Comparing `PyInventory-0.9.3rc4/src/inventory_project/templates/admin/login.html` & `PyInventory-0.9.4/src/inventory_project/templates/admin/login.html`

 * *Files identical despite different names*

### Comparing `PyInventory-0.9.3rc4/src/inventory_project/tests/middleware.py` & `PyInventory-0.9.4/src/inventory_project/tests/middleware.py`

 * *Files identical despite different names*

### Comparing `PyInventory-0.9.3rc4/src/inventory_project/tests/test_admin.py` & `PyInventory-0.9.4/src/inventory_project/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `PyInventory-0.9.3rc4/src/inventory_project/tests/test_admin_item.py` & `PyInventory-0.9.4/src/inventory_project/tests/test_admin_item.py`

 * *Files identical despite different names*

### Comparing `PyInventory-0.9.3rc4/src/inventory_project/tests/test_bootstrap.py` & `PyInventory-0.9.4/src/inventory_project/tests/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `PyInventory-0.9.3rc4/src/inventory_project/tests/test_inventory_commands.py` & `PyInventory-0.9.4/src/inventory_project/tests/test_inventory_commands.py`

 * *Files identical despite different names*

### Comparing `PyInventory-0.9.3rc4/src/inventory_project/tests/test_migrations.py` & `PyInventory-0.9.4/src/inventory_project/tests/test_migrations.py`

 * *Files identical despite different names*

### Comparing `PyInventory-0.9.3rc4/src/inventory_project/tests/test_project_setup.py` & `PyInventory-0.9.4/src/inventory_project/tests/test_project_setup.py`

 * *Files identical despite different names*

### Comparing `PyInventory-0.9.3rc4/src/inventory_project/tests/test_run_testserver.py` & `PyInventory-0.9.4/src/inventory_project/tests/test_run_testserver.py`

 * *Files identical despite different names*

### Comparing `PyInventory-0.9.3rc4/src/inventory_project/urls.py` & `PyInventory-0.9.4/src/inventory_project/urls.py`

 * *Files identical despite different names*

### Comparing `PyInventory-0.9.3rc4/setup.py` & `PyInventory-0.9.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,27 +42,27 @@
  'django>=2.2.0,<2.3.0',
  'gunicorn',
  'pillow',
  'requests']
 
 extras_require = \
 {'docker': ['docker-compose'],
- 'postgres-binary': ['psycopg2-binary'],
- 'psycopg2-source': ['psycopg2']}
+ 'postgres-binary': ['psycopg2-binary<2.9'],
+ 'psycopg2-source': ['psycopg2<2.9']}
 
 entry_points = \
 {'console_scripts': ['devshell = inventory_project.dev_shell:devshell_cmdloop',
                      'run_testserver = '
                      'inventory_project.manage:start_test_server']}
 
 setup_kwargs = {
     'name': 'pyinventory',
-    'version': '0.9.3rc4',
+    'version': '0.9.4',
     'description': 'Web based management to catalog things including state and location etc. using Python/Django.',
-    'long_description': '===========\nPyInventory\n===========\n\nWeb based management to catalog things including state and location etc. using Python/Django.\n\nThe project is in an early stage of development. Some things are already implemented and usable. But there is still a lot to do.\n\nPull requests welcome!\n\n+---------------------------------+-----------------------------------------+\n| |Build Status on github|        | `github.com/jedie/PyInventory/actions`_ |\n+---------------------------------+-----------------------------------------+\n| |Coverage Status on codecov.io| | `codecov.io/gh/jedie/PyInventory`_      |\n+---------------------------------+-----------------------------------------+\n\n.. |Build Status on github| image:: https://github.com/jedie/PyInventory/workflows/test/badge.svg?branch=master\n.. _github.com/jedie/PyInventory/actions: https://github.com/jedie/PyInventory/actions\n.. |Coverage Status on codecov.io| image:: https://codecov.io/gh/jedie/PyInventory/branch/master/graph/badge.svg\n.. _codecov.io/gh/jedie/PyInventory: https://codecov.io/gh/jedie/PyInventory\n\n-----\nabout\n-----\n\nThe focus of this project is on the management of retro computing hardware.\n\nPlan:\n\n* Web-based\n\n* Multiuser ready\n\n* Chaotic warehousing\n\n    * Grouped "Storage": Graphics card is in computer XY\n\n* Data structure kept as general as possible\n\n* You should be able to add the following to the items:\n\n    * Storage location\n\n    * State\n\n    * Pictures and Files\n\n    * URLs\n\n    * receiving and delivering (when, from whom, at what price, etc.)\n\n    * Information: Publicly visible yes/no\n\n* A public list of existing items (think about it, you can set in your profile if you want to)\n\n* administration a wish & exchange list\n\nany many more... ;)\n\n-----------------\nProject structure\n-----------------\n\nThere are two main directories:\n\n+---------------------+--------------------------------------------+\n| directory           | description                                |\n+=====================+============================================+\n| **`/src/`_**        | The main PyInventory source code           |\n+---------------------+--------------------------------------------+\n| **`/deployment/`_** | deploy PyInventory for production use case |\n+---------------------+--------------------------------------------+\n\n.. _/src/: https://github.com/jedie/PyInventory/tree/master/src\n.. _/deployment/: https://github.com/jedie/PyInventory/tree/master/deployment\n\n-------\ninstall\n-------\n\nThere exists these kind of installation/usage:\n\n* local development installation using poetry\n\n* production use with docker-compose on a root server\n\n* Install as `YunoHost <https://yunohost.org>`_ App via `pyinventory_ynh <https://github.com/YunoHost-Apps/pyinventory_ynh>`_\n\nThis README contains only the information about local development installation.\n\nRead `/deployment/README <https://github.com/jedie/PyInventory/tree/master/deployment#readme>`_ for instruction to install PyInventory on a root server.\n\nlocal development installation\n==============================\n\ne.g.:\n\n::\n\n    # Clone project (Use your fork SSH url!):\n    ~$ git clone https://github.com/jedie/PyInventory.git\n    ~$ cd PyInventory\n    ~/PyInventory$ ./devshell.py\n\nHelpful for writing and debugging unittests is to run a local test server.\ne.g.:\n\n::\n\n    ~/PyInventory$ ./devshell.py run_testserver\n\nThe web page is available via: ``http://127.0.0.1:8000/``\n\nYou can also pass a other port number or ``ipaddr:port`` combination. See: ``./devshell.py run_testserver --help``\n\nCall manage commands from test project, e.g.:\n\n::\n\n    ~/PyInventory$ ./devshell.py manage --help\n\nlocal docker dev run\n====================\n\nYou can run the deployment docker containers with current source code with:\n\n::\n\n    ~/PyInventory$ make run-docker-dev-server\n\nJust hit Cntl-C to stop the containers\n\nThe web page is available via: ``https://localhost/``\n\n-----------\nScreenshots\n-----------\n\n|PyInventory v0.2.0 screenshot 1.png|\n\n.. |PyInventory v0.2.0 screenshot 1.png| image:: https://raw.githubusercontent.com/jedie/jedie.github.io/master/screenshots/PyInventory/PyInventory v0.2.0 screenshot 1.png\n\n----\n\n|PyInventory v0.1.0 screenshot 2.png|\n\n.. |PyInventory v0.1.0 screenshot 2.png| image:: https://raw.githubusercontent.com/jedie/jedie.github.io/master/screenshots/PyInventory/PyInventory v0.1.0 screenshot 2.png\n\n----\n\n|PyInventory v0.1.0 screenshot 3.png|\n\n.. |PyInventory v0.1.0 screenshot 3.png| image:: https://raw.githubusercontent.com/jedie/jedie.github.io/master/screenshots/PyInventory/PyInventory v0.1.0 screenshot 3.png\n\n----\n\n------------------\nMulti user support\n------------------\n\nPyInventory supports multiple users. The idea:\n\n* Every normal user sees only his own created database entries\n\n* All users used the Django admin\n\nNote: All created Tags are shared for all existing users!\n\nSo setup a normal user:\n\n* Set "Staff status"\n\n* Unset "Superuser status"\n\n* Add user to "normal_user" group\n\n* Don\'t add any additional permissions\n\ne.g.:\n\n|normal user example|\n\n.. |normal user example| image:: https://raw.githubusercontent.com/jedie/jedie.github.io/master/screenshots/PyInventory/PyInventory normal user example.png\n\n------------------------------\nBackwards-incompatible changes\n------------------------------\n\nv0.7.0\n======\n\nDocker-Compose usage: The MEDIA files was not stored on a docker volumes.\n\nYou should backup rhe media files **before** update the containers!\n\ne.g.:\n\n::\n\n    ~/PyInventory/deployment$ make shell_inventory\n    root@inventory:/django# cp -Rfv /media/ /django_volumes/media/\n\nThe files are stored locally here:\n\n::\n\n    ~/PyInventory/deployment$ ls -la volumes/django/media/\n\nNow, update the containers and copy the files back.\n\nv0.5.0\n======\n\nGit branches "master" and "deployment" was merged into one.\nFiles are separated into: "/src/" and "/development/"\n\n-------\nhistory\n-------\n\n* `compare v0.9.2...master <https://github.com/jedie/PyInventory/compare/v0.9.2...master>`_ **dev** \n\n    * tbc\n\n* `v0.9.2 - 11.05.2021 <https://github.com/jedie/PyInventory/compare/v0.9.1...v0.9.2>`_ \n\n    * Update requirements\n\n    * `Fix error handling if item link is broken <https://github.com/jedie/PyInventory/issues/50>`_\n\n* `v0.9.1 - 28.04.2021 <https://github.com/jedie/PyInventory/compare/v0.9.0...v0.9.1>`_\n\n* NEW: Besides images, it\'s now possible to add file(s) to items, too.\n\n* Add a auto login if Django dev. server is used.\n\n* `v0.9.0 - 11.04.2021 <https://github.com/jedie/PyInventory/compare/v0.8.4...v0.9.0>`_ \n\n    * Use `https://github.com/jedie/dev-shell <https://github.com/jedie/dev-shell>`_ for development\n\n* `v0.8.4 - 19.01.2021 <https://github.com/jedie/PyInventory/compare/v0.8.3...v0.8.4>`_ \n\n    * Search items in change list by "kind" and "tags", too\n\n    * update requirements\n\n* `v0.8.3 - 29.12.2020 <https://github.com/jedie/PyInventory/compare/v0.8.2...v0.8.3>`_ \n\n    * update requirements\n\n    * remove colorama from direct dependencies\n\n    * Small project setup changes\n\n* `v0.8.2 - 20.12.2020 <https://github.com/jedie/PyInventory/compare/v0.8.1...v0.8.2>`_ \n\n    * Bugfix `#33 <https://github.com/jedie/PyInventory/issues/33>`_: Upload images to new created Items\n\n* `v0.8.1 - 09.12.2020 <https://github.com/jedie/PyInventory/compare/v0.8.0...v0.8.1>`_ \n\n    * Fix migration: Don\'t create "/media/migrate.log" if there is nothing to migrate\n\n    * Fix admin redirect by using the url pattern name\n\n    * YunoHost app package created\n\n    * update requirements\n\n* `v0.8.0 - 06.12.2020 <https://github.com/jedie/PyInventory/compare/v0.7.0...v0.8.0>`_ \n\n    * Outsource the "MEDIA file serve" part into `django.tools.serve_media_app <https://github.com/jedie/django-tools/tree/master/django_tools/serve_media_app#readme>`_\n\n* `v0.7.0 - 23.11.2020 <https://github.com/jedie/PyInventory/compare/v0.6.0...v0.7.0>`_ \n\n    * Change deployment setup:\n\n        * Replace uwsgi with gunicorn\n\n        * make deploy setup more generic by renaming "inventory" to "django"\n\n        * Bugfix MEDIA path: store the files on a docker volumes\n\n        * run app server as normal user and not root\n\n        * pull all docker images before build\n\n* `v0.6.0 - 15.11.2020 <https://github.com/jedie/PyInventory/compare/v0.5.0...v0.6.0>`_ \n\n    * User can store images to every item: The image can only be accessed by the same user.\n\n* `v0.5.0 - 14.11.2020 <https://github.com/jedie/PyInventory/compare/v0.4.2...v0.5.0>`_ \n\n    * Merge separate git branches into one: "/src/" and "/development/" `#19 <https://github.com/jedie/PyInventory/issues/19>`_\n\n* `v0.4.2 - 13.11.2020 <https://github.com/jedie/PyInventory/compare/v0.4.1...v0.4.2>`_ \n\n    * Serve static files by Caddy\n\n    * Setup CKEditor file uploads: Store files into random sub directory\n\n    * reduce CKEditor plugins\n\n* `v0.4.1 - 2.11.2020 <https://github.com/jedie/PyInventory/compare/v0.4.0...v0.4.1>`_ \n\n    * Small bugfixes\n\n* `v0.4.0 - 1.11.2020 <https://github.com/jedie/PyInventory/compare/v0.3.2...v0.4.0>`_ \n\n    * Move docker stuff and production use information into separate git branch\n\n    * Add django-axes: keeping track of suspicious logins and brute-force attack blocking\n\n    * Add django-processinfo: collect information about the running server processes\n\n* `v0.3.2 - 26.10.2020 <https://github.com/jedie/PyInventory/compare/v0.3.0...v0.3.2>`_ \n\n    * Bugfix missing translations\n\n* `v0.3.0 - 26.10.2020 <https://github.com/jedie/PyInventory/compare/v0.2.0...v0.3.0>`_ \n\n    * setup production usage:\n\n        * Use `caddy server <https://caddyserver.com/>`_ as reverse proxy\n\n        * Use uWSGI as application server\n\n        * autogenerate ``secret.txt`` file for ``settings.SECRET_KEY``\n\n        * Fix settings\n\n    * split settings for local development and production use\n\n    * Bugfix init: move "setup user group" from checks into "post migrate" signal handler\n\n    * Bugfix for using manage commands ``dumpdata`` and ``loaddata``\n\n* `v0.2.0 - 24.10.2020 <https://github.com/jedie/PyInventory/compare/v0.1.0...v0.2.0>`_ \n\n    * Simplify item change list by nested item\n\n    * Activate Django-Import/Export\n\n    * Implement multi user usage\n\n    * Add Django-dbbackup\n\n    * Add docker-compose usage\n\n* `v0.1.0 - 17.10.2020 <https://github.com/jedie/PyInventory/compare/v0.0.1...v0.1.0>`_ \n\n    * Enhance models, admin and finish project setup\n\n* v0.0.1 - 14.10.2020\n\n    * Just create a pre-alpha release to save the PyPi package name ;)\n\n-----\nlinks\n-----\n\n+----------+------------------------------------------+\n| Homepage | `http://github.com/jedie/PyInventory`_   |\n+----------+------------------------------------------+\n| PyPi     | `https://pypi.org/project/PyInventory/`_ |\n+----------+------------------------------------------+\n\n.. _http://github.com/jedie/PyInventory: http://github.com/jedie/PyInventory\n.. _https://pypi.org/project/PyInventory/: https://pypi.org/project/PyInventory/\n\nDiscuss here:\n\n* `vogons.org Forum Thread (en) <https://www.vogons.org/viewtopic.php?f=5&t=77285>`_\n\n* `Python-Forum (de) <https://www.python-forum.de/viewtopic.php?f=9&t=50024>`_\n\n* `VzEkC e. V. Forum Thread (de) <https://forum.classic-computing.de/forum/index.php?thread/21738-opensource-projekt-pyinventory-web-basierte-verwaltung-um-seine-dinge-zu-katalog/>`_\n\n* `dosreloaded.de Forum Thread (de) <https://dosreloaded.de/forum/index.php?thread/3702-pyinventory-retro-sammlung-katalogisieren/>`_\n\n--------\ndonation\n--------\n\n* `paypal.me/JensDiemer <https://www.paypal.me/JensDiemer>`_\n\n* `Flattr This! <https://flattr.com/submit/auto?uid=jedie&url=https%3A%2F%2Fgithub.com%2Fjedie%2FPyInventory%2F>`_\n\n* Send `Bitcoins <http://www.bitcoin.org/>`_ to `1823RZ5Md1Q2X5aSXRC5LRPcYdveCiVX6F <https://blockexplorer.com/address/1823RZ5Md1Q2X5aSXRC5LRPcYdveCiVX6F>`_\n\n------------\n\n``Note: this file is generated from README.creole 2021-08-04 09:01:51 with "python-creole"``',
+    'long_description': '===========\nPyInventory\n===========\n\nWeb based management to catalog things including state and location etc. using Python/Django.\n\nThe project is in an early stage of development. Some things are already implemented and usable. But there is still a lot to do.\n\nPull requests welcome!\n\n+---------------------------------+-----------------------------------------+\n| |Build Status on github|        | `github.com/jedie/PyInventory/actions`_ |\n+---------------------------------+-----------------------------------------+\n| |Coverage Status on codecov.io| | `codecov.io/gh/jedie/PyInventory`_      |\n+---------------------------------+-----------------------------------------+\n\n.. |Build Status on github| image:: https://github.com/jedie/PyInventory/workflows/test/badge.svg?branch=master\n.. _github.com/jedie/PyInventory/actions: https://github.com/jedie/PyInventory/actions\n.. |Coverage Status on codecov.io| image:: https://codecov.io/gh/jedie/PyInventory/branch/master/graph/badge.svg\n.. _codecov.io/gh/jedie/PyInventory: https://codecov.io/gh/jedie/PyInventory\n\n-----\nabout\n-----\n\nThe focus of this project is on the management of retro computing hardware.\n\nPlan:\n\n* Web-based\n\n* Multiuser ready\n\n* Chaotic warehousing\n\n    * Grouped "Storage": Graphics card is in computer XY\n\n* Data structure kept as general as possible\n\n* You should be able to add the following to the items:\n\n    * Storage location\n\n    * State\n\n    * Pictures and Files\n\n    * URLs\n\n    * receiving and delivering (when, from whom, at what price, etc.)\n\n    * Information: Publicly visible yes/no\n\n* A public list of existing items (think about it, you can set in your profile if you want to)\n\n* administration a wish & exchange list\n\nany many more... ;)\n\n-----------------\nProject structure\n-----------------\n\nThere are two main directories:\n\n+---------------------+--------------------------------------------+\n| directory           | description                                |\n+=====================+============================================+\n| **`/src/`_**        | The main PyInventory source code           |\n+---------------------+--------------------------------------------+\n| **`/deployment/`_** | deploy PyInventory for production use case |\n+---------------------+--------------------------------------------+\n\n.. _/src/: https://github.com/jedie/PyInventory/tree/master/src\n.. _/deployment/: https://github.com/jedie/PyInventory/tree/master/deployment\n\n-------\ninstall\n-------\n\nThere exists these kind of installation/usage:\n\n* local development installation using poetry\n\n* production use with docker-compose on a root server\n\n* Install as `YunoHost <https://yunohost.org>`_ App via `pyinventory_ynh <https://github.com/YunoHost-Apps/pyinventory_ynh>`_\n\nThis README contains only the information about local development installation.\n\nRead `/deployment/README <https://github.com/jedie/PyInventory/tree/master/deployment#readme>`_ for instruction to install PyInventory on a root server.\n\nlocal development installation\n==============================\n\ne.g.:\n\n::\n\n    # Clone project (Use your fork SSH url!):\n    ~$ git clone https://github.com/jedie/PyInventory.git\n    ~$ cd PyInventory\n    ~/PyInventory$ ./devshell.py\n\nHelpful for writing and debugging unittests is to run a local test server.\ne.g.:\n\n::\n\n    ~/PyInventory$ ./devshell.py run_testserver\n\nThe web page is available via: ``http://127.0.0.1:8000/``\n\nYou can also pass a other port number or ``ipaddr:port`` combination. See: ``./devshell.py run_testserver --help``\n\nCall manage commands from test project, e.g.:\n\n::\n\n    ~/PyInventory$ ./devshell.py manage --help\n\nlocal docker dev run\n====================\n\nYou can run the deployment docker containers with current source code with:\n\n::\n\n    ~/PyInventory$ make run-docker-dev-server\n\nJust hit Cntl-C to stop the containers\n\nThe web page is available via: ``https://localhost/``\n\n-----------\nScreenshots\n-----------\n\n|PyInventory v0.2.0 screenshot 1.png|\n\n.. |PyInventory v0.2.0 screenshot 1.png| image:: https://raw.githubusercontent.com/jedie/jedie.github.io/master/screenshots/PyInventory/PyInventory v0.2.0 screenshot 1.png\n\n----\n\n|PyInventory v0.1.0 screenshot 2.png|\n\n.. |PyInventory v0.1.0 screenshot 2.png| image:: https://raw.githubusercontent.com/jedie/jedie.github.io/master/screenshots/PyInventory/PyInventory v0.1.0 screenshot 2.png\n\n----\n\n|PyInventory v0.1.0 screenshot 3.png|\n\n.. |PyInventory v0.1.0 screenshot 3.png| image:: https://raw.githubusercontent.com/jedie/jedie.github.io/master/screenshots/PyInventory/PyInventory v0.1.0 screenshot 3.png\n\n----\n\n------------------\nMulti user support\n------------------\n\nPyInventory supports multiple users. The idea:\n\n* Every normal user sees only his own created database entries\n\n* All users used the Django admin\n\nNote: All created Tags are shared for all existing users!\n\nSo setup a normal user:\n\n* Set "Staff status"\n\n* Unset "Superuser status"\n\n* Add user to "normal_user" group\n\n* Don\'t add any additional permissions\n\ne.g.:\n\n|normal user example|\n\n.. |normal user example| image:: https://raw.githubusercontent.com/jedie/jedie.github.io/master/screenshots/PyInventory/PyInventory normal user example.png\n\n------------------------------\nBackwards-incompatible changes\n------------------------------\n\nv0.7.0\n======\n\nDocker-Compose usage: The MEDIA files was not stored on a docker volumes.\n\nYou should backup rhe media files **before** update the containers!\n\ne.g.:\n\n::\n\n    ~/PyInventory/deployment$ make shell_inventory\n    root@inventory:/django# cp -Rfv /media/ /django_volumes/media/\n\nThe files are stored locally here:\n\n::\n\n    ~/PyInventory/deployment$ ls -la volumes/django/media/\n\nNow, update the containers and copy the files back.\n\nv0.5.0\n======\n\nGit branches "master" and "deployment" was merged into one.\nFiles are separated into: "/src/" and "/development/"\n\n-------\nhistory\n-------\n\n* `compare v0.9.4...master <https://github.com/jedie/PyInventory/compare/v0.9.4...master>`_ **dev** \n\n    * tbc\n\n* `v0.9.4 - 15.09.2021 <https://github.com/jedie/PyInventory/compare/v0.9.3...v0.9.4>`_ \n\n    * Pin ``psycopg < 2.9`` because of `https://github.com/psycopg/psycopg2/issues/1293 <https://github.com/psycopg/psycopg2/issues/1293>`_\n\n* `v0.9.3 - 15.09.2021 <https://github.com/jedie/PyInventory/compare/v0.9.2...v0.9.3>`_ \n\n    * Optimize "items" changelist queries\n\n    * Update requirements\n\n    * Expand ``run_testserver`` command and recognize address and port argument\n\n* `v0.9.2 - 11.05.2021 <https://github.com/jedie/PyInventory/compare/v0.9.1...v0.9.2>`_ \n\n    * Update requirements\n\n    * `Fix error handling if item link is broken <https://github.com/jedie/PyInventory/issues/50>`_\n\n* `v0.9.1 - 28.04.2021 <https://github.com/jedie/PyInventory/compare/v0.9.0...v0.9.1>`_\n\n* NEW: Besides images, it\'s now possible to add file(s) to items, too.\n\n* Add a auto login if Django dev. server is used.\n\n* `v0.9.0 - 11.04.2021 <https://github.com/jedie/PyInventory/compare/v0.8.4...v0.9.0>`_ \n\n    * Use `https://github.com/jedie/dev-shell <https://github.com/jedie/dev-shell>`_ for development\n\n* `v0.8.4 - 19.01.2021 <https://github.com/jedie/PyInventory/compare/v0.8.3...v0.8.4>`_ \n\n    * Search items in change list by "kind" and "tags", too\n\n    * update requirements\n\n* `v0.8.3 - 29.12.2020 <https://github.com/jedie/PyInventory/compare/v0.8.2...v0.8.3>`_ \n\n    * update requirements\n\n    * remove colorama from direct dependencies\n\n    * Small project setup changes\n\n* `v0.8.2 - 20.12.2020 <https://github.com/jedie/PyInventory/compare/v0.8.1...v0.8.2>`_ \n\n    * Bugfix `#33 <https://github.com/jedie/PyInventory/issues/33>`_: Upload images to new created Items\n\n* `v0.8.1 - 09.12.2020 <https://github.com/jedie/PyInventory/compare/v0.8.0...v0.8.1>`_ \n\n    * Fix migration: Don\'t create "/media/migrate.log" if there is nothing to migrate\n\n    * Fix admin redirect by using the url pattern name\n\n    * YunoHost app package created\n\n    * update requirements\n\n* `v0.8.0 - 06.12.2020 <https://github.com/jedie/PyInventory/compare/v0.7.0...v0.8.0>`_ \n\n    * Outsource the "MEDIA file serve" part into `django.tools.serve_media_app <https://github.com/jedie/django-tools/tree/master/django_tools/serve_media_app#readme>`_\n\n* `v0.7.0 - 23.11.2020 <https://github.com/jedie/PyInventory/compare/v0.6.0...v0.7.0>`_ \n\n    * Change deployment setup:\n\n        * Replace uwsgi with gunicorn\n\n        * make deploy setup more generic by renaming "inventory" to "django"\n\n        * Bugfix MEDIA path: store the files on a docker volumes\n\n        * run app server as normal user and not root\n\n        * pull all docker images before build\n\n* `v0.6.0 - 15.11.2020 <https://github.com/jedie/PyInventory/compare/v0.5.0...v0.6.0>`_ \n\n    * User can store images to every item: The image can only be accessed by the same user.\n\n* `v0.5.0 - 14.11.2020 <https://github.com/jedie/PyInventory/compare/v0.4.2...v0.5.0>`_ \n\n    * Merge separate git branches into one: "/src/" and "/development/" `#19 <https://github.com/jedie/PyInventory/issues/19>`_\n\n* `v0.4.2 - 13.11.2020 <https://github.com/jedie/PyInventory/compare/v0.4.1...v0.4.2>`_ \n\n    * Serve static files by Caddy\n\n    * Setup CKEditor file uploads: Store files into random sub directory\n\n    * reduce CKEditor plugins\n\n* `v0.4.1 - 2.11.2020 <https://github.com/jedie/PyInventory/compare/v0.4.0...v0.4.1>`_ \n\n    * Small bugfixes\n\n* `v0.4.0 - 1.11.2020 <https://github.com/jedie/PyInventory/compare/v0.3.2...v0.4.0>`_ \n\n    * Move docker stuff and production use information into separate git branch\n\n    * Add django-axes: keeping track of suspicious logins and brute-force attack blocking\n\n    * Add django-processinfo: collect information about the running server processes\n\n* `v0.3.2 - 26.10.2020 <https://github.com/jedie/PyInventory/compare/v0.3.0...v0.3.2>`_ \n\n    * Bugfix missing translations\n\n* `v0.3.0 - 26.10.2020 <https://github.com/jedie/PyInventory/compare/v0.2.0...v0.3.0>`_ \n\n    * setup production usage:\n\n        * Use `caddy server <https://caddyserver.com/>`_ as reverse proxy\n\n        * Use uWSGI as application server\n\n        * autogenerate ``secret.txt`` file for ``settings.SECRET_KEY``\n\n        * Fix settings\n\n    * split settings for local development and production use\n\n    * Bugfix init: move "setup user group" from checks into "post migrate" signal handler\n\n    * Bugfix for using manage commands ``dumpdata`` and ``loaddata``\n\n* `v0.2.0 - 24.10.2020 <https://github.com/jedie/PyInventory/compare/v0.1.0...v0.2.0>`_ \n\n    * Simplify item change list by nested item\n\n    * Activate Django-Import/Export\n\n    * Implement multi user usage\n\n    * Add Django-dbbackup\n\n    * Add docker-compose usage\n\n* `v0.1.0 - 17.10.2020 <https://github.com/jedie/PyInventory/compare/v0.0.1...v0.1.0>`_ \n\n    * Enhance models, admin and finish project setup\n\n* v0.0.1 - 14.10.2020\n\n    * Just create a pre-alpha release to save the PyPi package name ;)\n\n-----\nlinks\n-----\n\n+----------+------------------------------------------+\n| Homepage | `http://github.com/jedie/PyInventory`_   |\n+----------+------------------------------------------+\n| PyPi     | `https://pypi.org/project/PyInventory/`_ |\n+----------+------------------------------------------+\n\n.. _http://github.com/jedie/PyInventory: http://github.com/jedie/PyInventory\n.. _https://pypi.org/project/PyInventory/: https://pypi.org/project/PyInventory/\n\nDiscuss here:\n\n* `vogons.org Forum Thread (en) <https://www.vogons.org/viewtopic.php?f=5&t=77285>`_\n\n* `Python-Forum (de) <https://www.python-forum.de/viewtopic.php?f=9&t=50024>`_\n\n* `VzEkC e. V. Forum Thread (de) <https://forum.classic-computing.de/forum/index.php?thread/21738-opensource-projekt-pyinventory-web-basierte-verwaltung-um-seine-dinge-zu-katalog/>`_\n\n* `dosreloaded.de Forum Thread (de) <https://dosreloaded.de/forum/index.php?thread/3702-pyinventory-retro-sammlung-katalogisieren/>`_\n\n--------\ndonation\n--------\n\n* `paypal.me/JensDiemer <https://www.paypal.me/JensDiemer>`_\n\n* `Flattr This! <https://flattr.com/submit/auto?uid=jedie&url=https%3A%2F%2Fgithub.com%2Fjedie%2FPyInventory%2F>`_\n\n* Send `Bitcoins <http://www.bitcoin.org/>`_ to `1823RZ5Md1Q2X5aSXRC5LRPcYdveCiVX6F <https://blockexplorer.com/address/1823RZ5Md1Q2X5aSXRC5LRPcYdveCiVX6F>`_\n\n------------\n\n``Note: this file is generated from README.creole 2021-09-15 21:28:39 with "python-creole"``',
     'author': 'JensDiemer',
     'author_email': 'git@jensdiemer.de',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/jedie/PyInventory',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `PyInventory-0.9.3rc4/PKG-INFO` & `PyInventory-0.9.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinventory
-Version: 0.9.3rc4
+Version: 0.9.4
 Summary: Web based management to catalog things including state and location etc. using Python/Django.
 Home-page: https://github.com/jedie/PyInventory
 Keywords: inventory,django
 Author: JensDiemer
 Author-email: git@jensdiemer.de
 Requires-Python: >=3.7,<4.0.0
 Classifier: Development Status :: 4 - Beta
@@ -40,16 +40,16 @@
 Requires-Dist: django-processinfo
 Requires-Dist: django-reversion-compare
 Requires-Dist: django-tagulous
 Requires-Dist: django-tools (>=0.48.2)
 Requires-Dist: docker-compose; extra == "docker"
 Requires-Dist: gunicorn
 Requires-Dist: pillow
-Requires-Dist: psycopg2-binary; extra == "postgres-binary"
-Requires-Dist: psycopg2; extra == "psycopg2-source"
+Requires-Dist: psycopg2 (<2.9); extra == "psycopg2-source"
+Requires-Dist: psycopg2-binary (<2.9); extra == "postgres-binary"
 Requires-Dist: requests
 Description-Content-Type: text/x-rst
 
 ===========
 PyInventory
 ===========
 
@@ -265,18 +265,30 @@
 Git branches "master" and "deployment" was merged into one.
 Files are separated into: "/src/" and "/development/"
 
 -------
 history
 -------
 
-* `compare v0.9.2...master <https://github.com/jedie/PyInventory/compare/v0.9.2...master>`_ **dev** 
+* `compare v0.9.4...master <https://github.com/jedie/PyInventory/compare/v0.9.4...master>`_ **dev** 
 
     * tbc
 
+* `v0.9.4 - 15.09.2021 <https://github.com/jedie/PyInventory/compare/v0.9.3...v0.9.4>`_ 
+
+    * Pin ``psycopg < 2.9`` because of `https://github.com/psycopg/psycopg2/issues/1293 <https://github.com/psycopg/psycopg2/issues/1293>`_
+
+* `v0.9.3 - 15.09.2021 <https://github.com/jedie/PyInventory/compare/v0.9.2...v0.9.3>`_ 
+
+    * Optimize "items" changelist queries
+
+    * Update requirements
+
+    * Expand ``run_testserver`` command and recognize address and port argument
+
 * `v0.9.2 - 11.05.2021 <https://github.com/jedie/PyInventory/compare/v0.9.1...v0.9.2>`_ 
 
     * Update requirements
 
     * `Fix error handling if item link is broken <https://github.com/jedie/PyInventory/issues/50>`_
 
 * `v0.9.1 - 28.04.2021 <https://github.com/jedie/PyInventory/compare/v0.9.0...v0.9.1>`_
@@ -436,8 +448,8 @@
 
 * `Flattr This! <https://flattr.com/submit/auto?uid=jedie&url=https%3A%2F%2Fgithub.com%2Fjedie%2FPyInventory%2F>`_
 
 * Send `Bitcoins <http://www.bitcoin.org/>`_ to `1823RZ5Md1Q2X5aSXRC5LRPcYdveCiVX6F <https://blockexplorer.com/address/1823RZ5Md1Q2X5aSXRC5LRPcYdveCiVX6F>`_
 
 ------------
 
-``Note: this file is generated from README.creole 2021-08-04 09:01:51 with "python-creole"``
+``Note: this file is generated from README.creole 2021-09-15 21:28:39 with "python-creole"``
```

