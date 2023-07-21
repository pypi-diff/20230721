# Comparing `tmp/django-filer-3.0.2.tar.gz` & `tmp/django-filer-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-filer-3.0.2.tar", last modified: Mon Jul 17 09:10:03 2023, max compression
+gzip compressed data, was "django-filer-3.0.3.tar", last modified: Fri Jul 21 13:47:02 2023, max compression
```

## Comparing `django-filer-3.0.2.tar` & `django-filer-3.0.3.tar`

### file list

```diff
@@ -1,378 +1,378 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.760232 django-filer-3.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-17 09:09:55.000000 django-filer-3.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-17 09:09:55.000000 django-filer-3.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-07-17 09:10:03.760232 django-filer-3.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-07-17 09:09:55.000000 django-filer-3.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.728232 django-filer-3.0.2/django_filer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-07-17 09:10:03.000000 django-filer-3.0.2/django_filer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10531 2023-07-17 09:10:03.000000 django-filer-3.0.2/django_filer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 09:10:03.000000 django-filer-3.0.2/django_filer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 09:10:03.000000 django-filer-3.0.2/django_filer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-17 09:10:03.000000 django-filer-3.0.2/django_filer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-17 09:10:03.000000 django-filer-3.0.2/django_filer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.728232 django-filer-3.0.2/filer/
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.732232 django-filer-3.0.2/filer/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/admin/clipboardadmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/admin/fileadmin.py
--rw-r--r--   0 runner    (1001) docker     (123)    57162 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/admin/folderadmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/admin/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/admin/imageadmin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.732232 django-filer-3.0.2/filer/admin/patched/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/admin/patched/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/admin/patched/admin_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/admin/permissionadmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/admin/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/admin/thumbnailoptionadmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/admin/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/admin/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.732232 django-filer-3.0.2/filer/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.732232 django-filer-3.0.2/filer/contrib/django_cms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/contrib/django_cms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/contrib/django_cms/cms_toolbars.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.732232 django-filer-3.0.2/filer/fields/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/fields/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/fields/folder.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/fields/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/fields/multistorage_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.732232 django-filer-3.0.2/filer/locale/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/README
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.708232 django-filer-3.0.2/filer/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.732232 django-filer-3.0.2/filer/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    31052 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.708232 django-filer-3.0.2/filer/locale/bg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.732232 django-filer-3.0.2/filer/locale/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/bg/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    30552 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/bg/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.708232 django-filer-3.0.2/filer/locale/ca/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.732232 django-filer-3.0.2/filer/locale/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    16835 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/ca/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    36871 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/ca/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.708232 django-filer-3.0.2/filer/locale/cs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.732232 django-filer-3.0.2/filer/locale/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    16655 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    37028 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.708232 django-filer-3.0.2/filer/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.732232 django-filer-3.0.2/filer/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    20130 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    38885 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.708232 django-filer-3.0.2/filer/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.732232 django-filer-3.0.2/filer/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    15886 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    36373 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.708232 django-filer-3.0.2/filer/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.732232 django-filer-3.0.2/filer/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    17750 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    37978 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.708232 django-filer-3.0.2/filer/locale/et/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.732232 django-filer-3.0.2/filer/locale/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/et/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    31970 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/et/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.712233 django-filer-3.0.2/filer/locale/eu/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.732232 django-filer-3.0.2/filer/locale/eu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    11255 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/eu/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    34500 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/eu/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.712233 django-filer-3.0.2/filer/locale/fa/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.736232 django-filer-3.0.2/filer/locale/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/fa/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    31106 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/fa/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.712233 django-filer-3.0.2/filer/locale/fi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.736232 django-filer-3.0.2/filer/locale/fi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    16872 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/fi/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    36774 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/fi/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.712233 django-filer-3.0.2/filer/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.736232 django-filer-3.0.2/filer/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    20427 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    39279 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.712233 django-filer-3.0.2/filer/locale/gl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.736232 django-filer-3.0.2/filer/locale/gl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/gl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    31668 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/gl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.712233 django-filer-3.0.2/filer/locale/he/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.736232 django-filer-3.0.2/filer/locale/he/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    14531 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/he/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    36970 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/he/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.712233 django-filer-3.0.2/filer/locale/hr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.736232 django-filer-3.0.2/filer/locale/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    13564 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/hr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    35907 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/hr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.712233 django-filer-3.0.2/filer/locale/hu/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.736232 django-filer-3.0.2/filer/locale/hu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    17033 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/hu/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    37028 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/hu/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.716233 django-filer-3.0.2/filer/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.736232 django-filer-3.0.2/filer/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    17406 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    37487 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.716233 django-filer-3.0.2/filer/locale/ja/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.736232 django-filer-3.0.2/filer/locale/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    30439 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.716233 django-filer-3.0.2/filer/locale/ja_JP/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.736232 django-filer-3.0.2/filer/locale/ja_JP/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/ja_JP/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    30453 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/ja_JP/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.716233 django-filer-3.0.2/filer/locale/lt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.736232 django-filer-3.0.2/filer/locale/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    17519 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/lt/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    37572 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/lt/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.716233 django-filer-3.0.2/filer/locale/lt_LT/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.736232 django-filer-3.0.2/filer/locale/lt_LT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/lt_LT/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    30912 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/lt_LT/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.716233 django-filer-3.0.2/filer/locale/nb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.736232 django-filer-3.0.2/filer/locale/nb/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    12883 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/nb/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    35169 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/nb/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.716233 django-filer-3.0.2/filer/locale/nl_NL/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.736232 django-filer-3.0.2/filer/locale/nl_NL/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    19709 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/nl_NL/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    38395 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/nl_NL/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.716233 django-filer-3.0.2/filer/locale/nn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.740232 django-filer-3.0.2/filer/locale/nn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    12775 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/nn/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    35104 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/nn/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.716233 django-filer-3.0.2/filer/locale/pl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.740232 django-filer-3.0.2/filer/locale/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    37613 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.720233 django-filer-3.0.2/filer/locale/pt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.740232 django-filer-3.0.2/filer/locale/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/pt/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    30709 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/pt/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.720233 django-filer-3.0.2/filer/locale/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.740232 django-filer-3.0.2/filer/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    17705 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    37766 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.720233 django-filer-3.0.2/filer/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.740232 django-filer-3.0.2/filer/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    21392 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    41615 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.720233 django-filer-3.0.2/filer/locale/sk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.740232 django-filer-3.0.2/filer/locale/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/sk/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    30834 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/sk/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.720233 django-filer-3.0.2/filer/locale/tr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.740232 django-filer-3.0.2/filer/locale/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     7475 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    33015 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.720233 django-filer-3.0.2/filer/locale/vi_VN/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.740232 django-filer-3.0.2/filer/locale/vi_VN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    18287 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/vi_VN/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    38041 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/vi_VN/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.720233 django-filer-3.0.2/filer/locale/zh/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.740232 django-filer-3.0.2/filer/locale/zh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/zh/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    30438 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/zh/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.720233 django-filer-3.0.2/filer/locale/zh-Hans/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.740232 django-filer-3.0.2/filer/locale/zh-Hans/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    15401 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/zh-Hans/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    35158 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/zh-Hans/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.724233 django-filer-3.0.2/filer/locale/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.740232 django-filer-3.0.2/filer/locale/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/zh_CN/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    30452 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/zh_CN/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.724233 django-filer-3.0.2/filer/locale/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.740232 django-filer-3.0.2/filer/locale/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/zh_TW/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    30453 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/locale/zh_TW/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.740232 django-filer-3.0.2/filer/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.740232 django-filer-3.0.2/filer/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/management/commands/filer_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/management/commands/generate_thumbnails.py
--rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/management/commands/import_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.744232 django-filer-3.0.2/filer/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     9951 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/migrations/0002_auto_20150606_2003.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/migrations/0003_thumbnailoption.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/migrations/0004_auto_20160328_1434.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/migrations/0005_auto_20160623_1425.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/migrations/0006_auto_20160623_1627.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/migrations/0007_auto_20161016_1055.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/migrations/0008_auto_20171117_1313.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/migrations/0009_auto_20171220_1635.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/migrations/0010_auto_20180414_2058.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/migrations/0011_auto_20190418_0137.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/migrations/0012_file_mime_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/migrations/0013_image_width_height_to_float.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/migrations/0014_folder_permission_choices.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/migrations/0015_alter_file_owner_alter_file_polymorphic_ctype_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/migrations/0016_alter_folder_index_together_remove_folder_level_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/migrations/0017_image__transparent.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.744232 django-filer-3.0.2/filer/models/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/models/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/models/clipboardmodels.py
--rw-r--r--   0 runner    (1001) docker     (123)    13079 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/models/filemodels.py
--rw-r--r--   0 runner    (1001) docker     (123)    12554 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/models/foldermodels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/models/imagemodels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/models/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/models/thumbnailoptionmodels.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/models/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/models/virtualitems.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.744232 django-filer-3.0.2/filer/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.744232 django-filer-3.0.2/filer/server/backends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/server/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/server/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/server/backends/default.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/server/backends/nginx.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/server/backends/xsendfile.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/server/main_server_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/server/thumbnails_server_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/server/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/server/views.py
--rw-r--r--   0 runner    (1001) docker     (123)    12946 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.724233 django-filer-3.0.2/filer/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.724233 django-filer-3.0.2/filer/static/filer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.748232 django-filer-3.0.2/filer/static/filer/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/css/admin_filer.cms.icons.css
--rwxr-xr-x   0 runner    (1001) docker     (123)    91187 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/css/admin_filer.css
--rw-r--r--   0 runner    (1001) docker     (123)    25479 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/css/admin_filer.fa.icons.css
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/css/admin_folderpermissions.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.748232 django-filer-3.0.2/filer/static/filer/css/maps/
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/css/maps/admin_filer.cms.icons.css.map
--rw-r--r--   0 runner    (1001) docker     (123)    87138 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/css/maps/admin_filer.css.map
--rw-r--r--   0 runner    (1001) docker     (123)    65841 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/css/maps/admin_filer.fa.icons.css.map
--rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/css/maps/admin_filer.icons.css.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.748232 django-filer-3.0.2/filer/static/filer/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   106260 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/fonts/FontAwesome.otf
--rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/fonts/django-filer-iconfont.eot
--rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/fonts/django-filer-iconfont.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/fonts/django-filer-iconfont.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/fonts/django-filer-iconfont.woff
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/fonts/django-filer-iconfont.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    68875 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/fonts/fontawesome-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (123)   355981 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/fonts/fontawesome-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (123)   138204 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    81284 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/fonts/fontawesome-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (123)    64464 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/fonts/fontawesome-webfont.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.752232 django-filer-3.0.2/filer/static/filer/fonts/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/fonts/src/arrow-down.svg
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/fonts/src/caret-down.svg
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/fonts/src/chevron-right.svg
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/fonts/src/download.svg
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/fonts/src/expand.svg
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/fonts/src/link.svg
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/fonts/src/move-to-folder.svg
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/fonts/src/picture.svg
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/fonts/src/remove-selection.svg
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/fonts/src/select.svg
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/fonts/src/th-large.svg
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/fonts/src/th-list.svg
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/fonts/src/upload.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.752232 django-filer-3.0.2/filer/static/filer/icons/
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/icons/cloud-up.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/icons/file-audio.svg
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/icons/file-empty.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/icons/file-font.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/icons/file-missing.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/icons/file-pdf.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/icons/file-picture.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/icons/file-unknown.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/icons/file-video.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/icons/file-zip.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/icons/folder-dropdown.svg
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/icons/folder-root.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/icons/folder-unfiled.svg
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/icons/folder.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.752232 django-filer-3.0.2/filer/static/filer/img/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/img/button-bg.gif
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/img/close.gif
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/img/icon_changelink.gif
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/img/icon_deletelink.gif
--rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/img/loading_animation.gif
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/img/nav-bg.gif
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/img/select_item-hover.gif
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/img/select_item.gif
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/img/upload_button.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.752232 django-filer-3.0.2/filer/static/filer/js/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.756232 django-filer-3.0.2/filer/static/filer/js/addons/
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/js/addons/copy-move-files.js
--rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/js/addons/dropdown-menu.js
--rw-r--r--   0 runner    (1001) docker     (123)     6720 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/js/addons/dropzone.init.js
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/js/addons/filer_popup_response.js
--rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/js/addons/focal-point.js
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/js/addons/popup_handling.js
--rw-r--r--   0 runner    (1001) docker     (123)    10389 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/js/addons/table-dropzone.js
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/js/addons/toggler.js
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/js/addons/tooltip.js
--rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/js/addons/upload-button.js
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/js/addons/widget.js
--rw-r--r--   0 runner    (1001) docker     (123)    11090 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/js/base.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.756232 django-filer-3.0.2/filer/static/filer/js/libs/
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/js/libs/class.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    34316 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/js/libs/dropzone.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    18574 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/js/libs/fileuploader.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   255084 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/js/libs/jquery-ui.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/js/libs/jquery.cookie.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    95957 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/js/libs/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/static/filer/js/libs/mediator.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.728232 django-filer-3.0.2/filer/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.728232 django-filer-3.0.2/filer/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.756232 django-filer-3.0.2/filer/templates/admin/filer/
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/templates/admin/filer/actions.html
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/templates/admin/filer/base_site.html
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/templates/admin/filer/breadcrumbs.html
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/templates/admin/filer/change_form.html
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/templates/admin/filer/delete_confirmation.html
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/templates/admin/filer/delete_selected_files_confirmation.html
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/templates/admin/filer/dismiss_popup.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.756232 django-filer-3.0.2/filer/templates/admin/filer/file/
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/templates/admin/filer/file/change_form.html
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/templates/admin/filer/file/popup_response.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.760232 django-filer-3.0.2/filer/templates/admin/filer/folder/
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/templates/admin/filer/folder/change_form.html
--rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/templates/admin/filer/folder/choose_copy_destination.html
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/templates/admin/filer/folder/choose_images_resize_options.html
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/templates/admin/filer/folder/choose_move_destination.html
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/templates/admin/filer/folder/choose_rename_format.html
--rw-r--r--   0 runner    (1001) docker     (123)    15526 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/templates/admin/filer/folder/directory_listing.html
--rw-r--r--   0 runner    (1001) docker     (123)    17055 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/templates/admin/filer/folder/directory_table_list.html
--rw-r--r--   0 runner    (1001) docker     (123)    13454 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/templates/admin/filer/folder/directory_thumbnail_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/templates/admin/filer/folder/list_type_switcher.html
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/templates/admin/filer/folder/new_folder_form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.760232 django-filer-3.0.2/filer/templates/admin/filer/image/
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/templates/admin/filer/image/change_form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.760232 django-filer-3.0.2/filer/templates/admin/filer/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/templates/admin/filer/templatetags/file_icon.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.760232 django-filer-3.0.2/filer/templates/admin/filer/tools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.760232 django-filer-3.0.2/filer/templates/admin/filer/tools/clipboard/
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/templates/admin/filer/tools/clipboard/clipboard.html
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/templates/admin/filer/tools/clipboard/clipboard_item_rows.html
--rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/templates/admin/filer/tools/detail_info.html
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/templates/admin/filer/tools/search_form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.760232 django-filer-3.0.2/filer/templates/admin/filer/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/templates/admin/filer/widgets/admin_file.html
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/templates/admin/filer/widgets/admin_folder.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.760232 django-filer-3.0.2/filer/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8357 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/templatetags/filer_admin_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/templatetags/filer_image_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/templatetags/filer_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     5840 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/thumbnail_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:10:03.760232 django-filer-3.0.2/filer/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/utils/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/utils/filer_easy_thumbnails.py
--rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/utils/generate_filename.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/utils/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/utils/model_label.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/utils/pil_exif.py
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/utils/recursive_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/utils/zip.py
--rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-17 09:09:55.000000 django-filer-3.0.2/filer/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-17 09:10:03.760232 django-filer-3.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-17 09:09:55.000000 django-filer-3.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.489183 django-filer-3.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-21 13:46:52.000000 django-filer-3.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-21 13:46:52.000000 django-filer-3.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-07-21 13:47:02.489183 django-filer-3.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-07-21 13:46:52.000000 django-filer-3.0.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.449180 django-filer-3.0.3/django_filer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-07-21 13:47:02.000000 django-filer-3.0.3/django_filer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10531 2023-07-21 13:47:02.000000 django-filer-3.0.3/django_filer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 13:47:02.000000 django-filer-3.0.3/django_filer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 13:47:02.000000 django-filer-3.0.3/django_filer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-21 13:47:02.000000 django-filer-3.0.3/django_filer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-21 13:47:02.000000 django-filer-3.0.3/django_filer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.449180 django-filer-3.0.3/filer/
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.449180 django-filer-3.0.3/filer/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/admin/clipboardadmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/admin/fileadmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57077 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/admin/folderadmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/admin/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/admin/imageadmin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.453180 django-filer-3.0.3/filer/admin/patched/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/admin/patched/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/admin/patched/admin_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/admin/permissionadmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/admin/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/admin/thumbnailoptionadmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/admin/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/admin/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.453180 django-filer-3.0.3/filer/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.453180 django-filer-3.0.3/filer/contrib/django_cms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/contrib/django_cms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/contrib/django_cms/cms_toolbars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.453180 django-filer-3.0.3/filer/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/fields/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/fields/folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/fields/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/fields/multistorage_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.453180 django-filer-3.0.3/filer/locale/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/README
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.437179 django-filer-3.0.3/filer/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.453180 django-filer-3.0.3/filer/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    31052 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.437179 django-filer-3.0.3/filer/locale/bg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.453180 django-filer-3.0.3/filer/locale/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/bg/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    30552 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/bg/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.437179 django-filer-3.0.3/filer/locale/ca/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.453180 django-filer-3.0.3/filer/locale/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16835 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/ca/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    36871 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/ca/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.437179 django-filer-3.0.3/filer/locale/cs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.453180 django-filer-3.0.3/filer/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16655 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    37028 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.437179 django-filer-3.0.3/filer/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.453180 django-filer-3.0.3/filer/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    20130 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    38885 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.437179 django-filer-3.0.3/filer/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.453180 django-filer-3.0.3/filer/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    15886 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    36373 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.437179 django-filer-3.0.3/filer/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.453180 django-filer-3.0.3/filer/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    17750 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    37978 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.437179 django-filer-3.0.3/filer/locale/et/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.457181 django-filer-3.0.3/filer/locale/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/et/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    31970 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/et/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.437179 django-filer-3.0.3/filer/locale/eu/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.457181 django-filer-3.0.3/filer/locale/eu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    11255 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/eu/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    34500 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/eu/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.441180 django-filer-3.0.3/filer/locale/fa/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.457181 django-filer-3.0.3/filer/locale/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/fa/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    31106 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/fa/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.441180 django-filer-3.0.3/filer/locale/fi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.457181 django-filer-3.0.3/filer/locale/fi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16872 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/fi/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    36774 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/fi/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.441180 django-filer-3.0.3/filer/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.457181 django-filer-3.0.3/filer/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    20427 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    39279 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.441180 django-filer-3.0.3/filer/locale/gl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.457181 django-filer-3.0.3/filer/locale/gl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/gl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    31668 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/gl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.441180 django-filer-3.0.3/filer/locale/he/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.457181 django-filer-3.0.3/filer/locale/he/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    14531 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/he/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    36970 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/he/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.441180 django-filer-3.0.3/filer/locale/hr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.457181 django-filer-3.0.3/filer/locale/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    13564 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/hr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    35907 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/hr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.441180 django-filer-3.0.3/filer/locale/hu/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.457181 django-filer-3.0.3/filer/locale/hu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    17033 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/hu/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    37028 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/hu/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.441180 django-filer-3.0.3/filer/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.457181 django-filer-3.0.3/filer/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    17406 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    37487 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.441180 django-filer-3.0.3/filer/locale/ja/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.457181 django-filer-3.0.3/filer/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    30439 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.441180 django-filer-3.0.3/filer/locale/ja_JP/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.457181 django-filer-3.0.3/filer/locale/ja_JP/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/ja_JP/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    30453 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/ja_JP/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.441180 django-filer-3.0.3/filer/locale/lt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.461181 django-filer-3.0.3/filer/locale/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    17519 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/lt/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    37572 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/lt/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.441180 django-filer-3.0.3/filer/locale/lt_LT/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.461181 django-filer-3.0.3/filer/locale/lt_LT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/lt_LT/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    30912 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/lt_LT/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.441180 django-filer-3.0.3/filer/locale/nb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.461181 django-filer-3.0.3/filer/locale/nb/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    12883 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/nb/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    35169 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/nb/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.441180 django-filer-3.0.3/filer/locale/nl_NL/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.461181 django-filer-3.0.3/filer/locale/nl_NL/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    19709 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/nl_NL/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    38395 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/nl_NL/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.441180 django-filer-3.0.3/filer/locale/nn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.461181 django-filer-3.0.3/filer/locale/nn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    12775 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/nn/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    35104 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/nn/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.441180 django-filer-3.0.3/filer/locale/pl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.461181 django-filer-3.0.3/filer/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    37613 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.441180 django-filer-3.0.3/filer/locale/pt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.461181 django-filer-3.0.3/filer/locale/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/pt/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    30709 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/pt/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.441180 django-filer-3.0.3/filer/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.461181 django-filer-3.0.3/filer/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    17705 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    37766 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.441180 django-filer-3.0.3/filer/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.461181 django-filer-3.0.3/filer/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    21392 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    41615 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.441180 django-filer-3.0.3/filer/locale/sk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.461181 django-filer-3.0.3/filer/locale/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/sk/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    30834 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/sk/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.441180 django-filer-3.0.3/filer/locale/tr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.461181 django-filer-3.0.3/filer/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     7475 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    33015 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.441180 django-filer-3.0.3/filer/locale/vi_VN/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.465181 django-filer-3.0.3/filer/locale/vi_VN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    18287 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/vi_VN/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    38041 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/vi_VN/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.445180 django-filer-3.0.3/filer/locale/zh/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.465181 django-filer-3.0.3/filer/locale/zh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/zh/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    30438 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/zh/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.441180 django-filer-3.0.3/filer/locale/zh-Hans/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.465181 django-filer-3.0.3/filer/locale/zh-Hans/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    15401 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/zh-Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    35158 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/zh-Hans/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.445180 django-filer-3.0.3/filer/locale/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.465181 django-filer-3.0.3/filer/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/zh_CN/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    30452 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/zh_CN/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.445180 django-filer-3.0.3/filer/locale/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.465181 django-filer-3.0.3/filer/locale/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/zh_TW/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    30453 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/locale/zh_TW/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.465181 django-filer-3.0.3/filer/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.465181 django-filer-3.0.3/filer/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/management/commands/filer_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/management/commands/generate_thumbnails.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/management/commands/import_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.469181 django-filer-3.0.3/filer/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     9951 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/migrations/0002_auto_20150606_2003.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/migrations/0003_thumbnailoption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/migrations/0004_auto_20160328_1434.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/migrations/0005_auto_20160623_1425.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/migrations/0006_auto_20160623_1627.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/migrations/0007_auto_20161016_1055.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/migrations/0008_auto_20171117_1313.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/migrations/0009_auto_20171220_1635.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/migrations/0010_auto_20180414_2058.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/migrations/0011_auto_20190418_0137.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/migrations/0012_file_mime_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/migrations/0013_image_width_height_to_float.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/migrations/0014_folder_permission_choices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/migrations/0015_alter_file_owner_alter_file_polymorphic_ctype_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/migrations/0016_alter_folder_index_together_remove_folder_level_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/migrations/0017_image__transparent.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.469181 django-filer-3.0.3/filer/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/models/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/models/clipboardmodels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13079 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/models/filemodels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12554 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/models/foldermodels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/models/imagemodels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/models/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/models/thumbnailoptionmodels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/models/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/models/virtualitems.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.469181 django-filer-3.0.3/filer/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.469181 django-filer-3.0.3/filer/server/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/server/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/server/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/server/backends/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/server/backends/nginx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/server/backends/xsendfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/server/main_server_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/server/thumbnails_server_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/server/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/server/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12946 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.445180 django-filer-3.0.3/filer/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.445180 django-filer-3.0.3/filer/static/filer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.473182 django-filer-3.0.3/filer/static/filer/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/css/admin_filer.cms.icons.css
+-rwxr-xr-x   0 runner    (1001) docker     (123)    91187 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/css/admin_filer.css
+-rw-r--r--   0 runner    (1001) docker     (123)    25479 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/css/admin_filer.fa.icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/css/admin_folderpermissions.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.473182 django-filer-3.0.3/filer/static/filer/css/maps/
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/css/maps/admin_filer.cms.icons.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)    87138 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/css/maps/admin_filer.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)    65841 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/css/maps/admin_filer.fa.icons.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/css/maps/admin_filer.icons.css.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.473182 django-filer-3.0.3/filer/static/filer/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   106260 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/fonts/FontAwesome.otf
+-rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/fonts/django-filer-iconfont.eot
+-rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/fonts/django-filer-iconfont.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/fonts/django-filer-iconfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/fonts/django-filer-iconfont.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/fonts/django-filer-iconfont.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    68875 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   355981 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   138204 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    81284 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    64464 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/fonts/fontawesome-webfont.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.477182 django-filer-3.0.3/filer/static/filer/fonts/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/fonts/src/arrow-down.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/fonts/src/caret-down.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/fonts/src/chevron-right.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/fonts/src/download.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/fonts/src/expand.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/fonts/src/link.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/fonts/src/move-to-folder.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/fonts/src/picture.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/fonts/src/remove-selection.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/fonts/src/select.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/fonts/src/th-large.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/fonts/src/th-list.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/fonts/src/upload.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.477182 django-filer-3.0.3/filer/static/filer/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/icons/cloud-up.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/icons/file-audio.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/icons/file-empty.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/icons/file-font.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/icons/file-missing.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/icons/file-pdf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/icons/file-picture.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/icons/file-unknown.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/icons/file-video.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/icons/file-zip.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/icons/folder-dropdown.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/icons/folder-root.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/icons/folder-unfiled.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/icons/folder.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.481182 django-filer-3.0.3/filer/static/filer/img/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/img/button-bg.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/img/close.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/img/icon_changelink.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/img/icon_deletelink.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/img/loading_animation.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/img/nav-bg.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/img/select_item-hover.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/img/select_item.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/img/upload_button.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.481182 django-filer-3.0.3/filer/static/filer/js/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.481182 django-filer-3.0.3/filer/static/filer/js/addons/
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/js/addons/copy-move-files.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/js/addons/dropdown-menu.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6720 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/js/addons/dropzone.init.js
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/js/addons/filer_popup_response.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/js/addons/focal-point.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/js/addons/popup_handling.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10389 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/js/addons/table-dropzone.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/js/addons/toggler.js
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/js/addons/tooltip.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/js/addons/upload-button.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/js/addons/widget.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11090 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/js/base.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.485182 django-filer-3.0.3/filer/static/filer/js/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/js/libs/class.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    34316 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/js/libs/dropzone.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18574 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/js/libs/fileuploader.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   255084 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/js/libs/jquery-ui.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/js/libs/jquery.cookie.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    95957 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/js/libs/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/static/filer/js/libs/mediator.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.445180 django-filer-3.0.3/filer/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.445180 django-filer-3.0.3/filer/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.485182 django-filer-3.0.3/filer/templates/admin/filer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/templates/admin/filer/actions.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/templates/admin/filer/base_site.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/templates/admin/filer/breadcrumbs.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/templates/admin/filer/change_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/templates/admin/filer/delete_confirmation.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/templates/admin/filer/delete_selected_files_confirmation.html
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/templates/admin/filer/dismiss_popup.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.485182 django-filer-3.0.3/filer/templates/admin/filer/file/
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/templates/admin/filer/file/change_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/templates/admin/filer/file/popup_response.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.485182 django-filer-3.0.3/filer/templates/admin/filer/folder/
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/templates/admin/filer/folder/change_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/templates/admin/filer/folder/choose_copy_destination.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/templates/admin/filer/folder/choose_images_resize_options.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/templates/admin/filer/folder/choose_move_destination.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/templates/admin/filer/folder/choose_rename_format.html
+-rw-r--r--   0 runner    (1001) docker     (123)    15547 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/templates/admin/filer/folder/directory_listing.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17055 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/templates/admin/filer/folder/directory_table_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13454 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/templates/admin/filer/folder/directory_thumbnail_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/templates/admin/filer/folder/list_type_switcher.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/templates/admin/filer/folder/new_folder_form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.485182 django-filer-3.0.3/filer/templates/admin/filer/image/
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/templates/admin/filer/image/change_form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.485182 django-filer-3.0.3/filer/templates/admin/filer/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/templates/admin/filer/templatetags/file_icon.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.485182 django-filer-3.0.3/filer/templates/admin/filer/tools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.489183 django-filer-3.0.3/filer/templates/admin/filer/tools/clipboard/
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/templates/admin/filer/tools/clipboard/clipboard.html
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/templates/admin/filer/tools/clipboard/clipboard_item_rows.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/templates/admin/filer/tools/detail_info.html
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/templates/admin/filer/tools/search_form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.489183 django-filer-3.0.3/filer/templates/admin/filer/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/templates/admin/filer/widgets/admin_file.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/templates/admin/filer/widgets/admin_folder.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.489183 django-filer-3.0.3/filer/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8795 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/templatetags/filer_admin_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/templatetags/filer_image_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/templatetags/filer_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5840 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/thumbnail_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:47:02.489183 django-filer-3.0.3/filer/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/utils/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/utils/filer_easy_thumbnails.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/utils/generate_filename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/utils/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/utils/model_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/utils/pil_exif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/utils/recursive_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/utils/zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-21 13:46:52.000000 django-filer-3.0.3/filer/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-21 13:47:02.489183 django-filer-3.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-21 13:46:52.000000 django-filer-3.0.3/setup.py
```

### Comparing `django-filer-3.0.2/LICENSE` & `django-filer-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/PKG-INFO` & `django-filer-3.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-filer
-Version: 3.0.2
+Version: 3.0.3
 Summary: A file management application for django that makes handling of files and images a breeze.
 Home-page: https://github.com/django-cms/django-filer
 Author: Divio AG
 Author-email: info@divio.ch
 Maintainer: Django CMS Association and contributors
 Maintainer-email: info@django-cms.org
 License: BSD-3-Clause
```

### Comparing `django-filer-3.0.2/README.rst` & `django-filer-3.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/django_filer.egg-info/PKG-INFO` & `django-filer-3.0.3/django_filer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-filer
-Version: 3.0.2
+Version: 3.0.3
 Summary: A file management application for django that makes handling of files and images a breeze.
 Home-page: https://github.com/django-cms/django-filer
 Author: Divio AG
 Author-email: info@divio.ch
 Maintainer: Django CMS Association and contributors
 Maintainer-email: info@django-cms.org
 License: BSD-3-Clause
```

### Comparing `django-filer-3.0.2/django_filer.egg-info/SOURCES.txt` & `django-filer-3.0.3/django_filer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/__init__.py` & `django-filer-3.0.3/filer/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,10 +9,10 @@
  5. git push
  6. Assure that all tests pass on https://github.com/django-cms/django-filer/actions
  7. Create a new release on github. Create the new tag against the latest master commit and auto generate
     the release notes https://github.com/django-cms/django-filer/releases/new
  8. Publish the release and it will automatically release to pypi
 """
 
-__version__ = '3.0.2'
+__version__ = '3.0.3'
 
 default_app_config = 'filer.apps.FilerConfig'
```

### Comparing `django-filer-3.0.2/filer/admin/__init__.py` & `django-filer-3.0.3/filer/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/admin/clipboardadmin.py` & `django-filer-3.0.3/filer/admin/clipboardadmin.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/admin/fileadmin.py` & `django-filer-3.0.3/filer/admin/fileadmin.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/admin/folderadmin.py` & `django-filer-3.0.3/filer/admin/folderadmin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1072,19 +1072,19 @@
         # TODO: Should we also allow not to overwrite the folder if it exists, but just copy into it?
 
         # TODO: Is this a race-condition? Would this be a problem?
         foldername = self._get_available_name(destination, folder.name)
 
         old_folder = Folder.objects.get(pk=folder.pk)
 
-        # Due to how inheritance works, we have to set both pk and id to None
-        folder.pk = None
-        folder.id = None
-        folder.name = foldername
-        folder.insert_at(destination, 'last-child', True)  # We save folder here
+        folder, _ = Folder.objects.get_or_create(
+            name=foldername,
+            owner=old_folder.owner,
+            parent=destination,
+        )
 
         for perm in FolderPermission.objects.filter(folder=old_folder):
             perm.pk = None
             perm.id = None
             perm.folder = folder
             perm.save()
```

### Comparing `django-filer-3.0.2/filer/admin/forms.py` & `django-filer-3.0.3/filer/admin/forms.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/admin/imageadmin.py` & `django-filer-3.0.3/filer/admin/imageadmin.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/admin/patched/admin_utils.py` & `django-filer-3.0.3/filer/admin/patched/admin_utils.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/admin/permissionadmin.py` & `django-filer-3.0.3/filer/admin/permissionadmin.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/admin/permissions.py` & `django-filer-3.0.3/filer/admin/permissions.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/admin/tools.py` & `django-filer-3.0.3/filer/admin/tools.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/admin/views.py` & `django-filer-3.0.3/filer/admin/views.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/apps.py` & `django-filer-3.0.3/filer/apps.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/contrib/django_cms/cms_toolbars.py` & `django-filer-3.0.3/filer/contrib/django_cms/cms_toolbars.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/fields/file.py` & `django-filer-3.0.3/filer/fields/file.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/fields/folder.py` & `django-filer-3.0.3/filer/fields/folder.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/fields/multistorage_file.py` & `django-filer-3.0.3/filer/fields/multistorage_file.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/ar/LC_MESSAGES/django.mo` & `django-filer-3.0.3/filer/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/ar/LC_MESSAGES/django.po` & `django-filer-3.0.3/filer/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/bg/LC_MESSAGES/django.po` & `django-filer-3.0.3/filer/locale/bg/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/ca/LC_MESSAGES/django.mo` & `django-filer-3.0.3/filer/locale/ca/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/ca/LC_MESSAGES/django.po` & `django-filer-3.0.3/filer/locale/ca/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/cs/LC_MESSAGES/django.mo` & `django-filer-3.0.3/filer/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/cs/LC_MESSAGES/django.po` & `django-filer-3.0.3/filer/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/de/LC_MESSAGES/django.mo` & `django-filer-3.0.3/filer/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/de/LC_MESSAGES/django.po` & `django-filer-3.0.3/filer/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/en/LC_MESSAGES/django.mo` & `django-filer-3.0.3/filer/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/en/LC_MESSAGES/django.po` & `django-filer-3.0.3/filer/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/es/LC_MESSAGES/django.mo` & `django-filer-3.0.3/filer/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/es/LC_MESSAGES/django.po` & `django-filer-3.0.3/filer/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/et/LC_MESSAGES/django.mo` & `django-filer-3.0.3/filer/locale/et/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/et/LC_MESSAGES/django.po` & `django-filer-3.0.3/filer/locale/et/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/eu/LC_MESSAGES/django.mo` & `django-filer-3.0.3/filer/locale/eu/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/eu/LC_MESSAGES/django.po` & `django-filer-3.0.3/filer/locale/eu/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/fa/LC_MESSAGES/django.mo` & `django-filer-3.0.3/filer/locale/fa/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/fa/LC_MESSAGES/django.po` & `django-filer-3.0.3/filer/locale/fa/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/fi/LC_MESSAGES/django.mo` & `django-filer-3.0.3/filer/locale/fi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/fi/LC_MESSAGES/django.po` & `django-filer-3.0.3/filer/locale/fi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/fr/LC_MESSAGES/django.mo` & `django-filer-3.0.3/filer/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/fr/LC_MESSAGES/django.po` & `django-filer-3.0.3/filer/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/gl/LC_MESSAGES/django.mo` & `django-filer-3.0.3/filer/locale/gl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/gl/LC_MESSAGES/django.po` & `django-filer-3.0.3/filer/locale/gl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/he/LC_MESSAGES/django.mo` & `django-filer-3.0.3/filer/locale/he/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/he/LC_MESSAGES/django.po` & `django-filer-3.0.3/filer/locale/he/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/hr/LC_MESSAGES/django.mo` & `django-filer-3.0.3/filer/locale/hr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/hr/LC_MESSAGES/django.po` & `django-filer-3.0.3/filer/locale/hr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/hu/LC_MESSAGES/django.mo` & `django-filer-3.0.3/filer/locale/hu/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/hu/LC_MESSAGES/django.po` & `django-filer-3.0.3/filer/locale/hu/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/it/LC_MESSAGES/django.mo` & `django-filer-3.0.3/filer/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/it/LC_MESSAGES/django.po` & `django-filer-3.0.3/filer/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/ja/LC_MESSAGES/django.po` & `django-filer-3.0.3/filer/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/ja_JP/LC_MESSAGES/django.po` & `django-filer-3.0.3/filer/locale/ja_JP/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/lt/LC_MESSAGES/django.mo` & `django-filer-3.0.3/filer/locale/lt/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/lt/LC_MESSAGES/django.po` & `django-filer-3.0.3/filer/locale/lt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/lt_LT/LC_MESSAGES/django.mo` & `django-filer-3.0.3/filer/locale/lt_LT/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/lt_LT/LC_MESSAGES/django.po` & `django-filer-3.0.3/filer/locale/lt_LT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/nb/LC_MESSAGES/django.mo` & `django-filer-3.0.3/filer/locale/nb/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/nb/LC_MESSAGES/django.po` & `django-filer-3.0.3/filer/locale/nb/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/nl_NL/LC_MESSAGES/django.mo` & `django-filer-3.0.3/filer/locale/nl_NL/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/nl_NL/LC_MESSAGES/django.po` & `django-filer-3.0.3/filer/locale/nl_NL/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/nn/LC_MESSAGES/django.mo` & `django-filer-3.0.3/filer/locale/nn/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/nn/LC_MESSAGES/django.po` & `django-filer-3.0.3/filer/locale/nn/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/pl/LC_MESSAGES/django.mo` & `django-filer-3.0.3/filer/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/pl/LC_MESSAGES/django.po` & `django-filer-3.0.3/filer/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/pt/LC_MESSAGES/django.po` & `django-filer-3.0.3/filer/locale/pt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/pt_BR/LC_MESSAGES/django.mo` & `django-filer-3.0.3/filer/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/pt_BR/LC_MESSAGES/django.po` & `django-filer-3.0.3/filer/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/ru/LC_MESSAGES/django.mo` & `django-filer-3.0.3/filer/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/ru/LC_MESSAGES/django.po` & `django-filer-3.0.3/filer/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/sk/LC_MESSAGES/django.mo` & `django-filer-3.0.3/filer/locale/sk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/sk/LC_MESSAGES/django.po` & `django-filer-3.0.3/filer/locale/sk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/tr/LC_MESSAGES/django.mo` & `django-filer-3.0.3/filer/locale/tr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/tr/LC_MESSAGES/django.po` & `django-filer-3.0.3/filer/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/vi_VN/LC_MESSAGES/django.mo` & `django-filer-3.0.3/filer/locale/vi_VN/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/vi_VN/LC_MESSAGES/django.po` & `django-filer-3.0.3/filer/locale/vi_VN/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/zh/LC_MESSAGES/django.po` & `django-filer-3.0.3/filer/locale/zh/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/zh-Hans/LC_MESSAGES/django.mo` & `django-filer-3.0.3/filer/locale/zh-Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/zh-Hans/LC_MESSAGES/django.po` & `django-filer-3.0.3/filer/locale/zh-Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/zh_CN/LC_MESSAGES/django.po` & `django-filer-3.0.3/filer/locale/zh_CN/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/locale/zh_TW/LC_MESSAGES/django.po` & `django-filer-3.0.3/filer/locale/zh_TW/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/management/commands/filer_check.py` & `django-filer-3.0.3/filer/management/commands/filer_check.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/management/commands/generate_thumbnails.py` & `django-filer-3.0.3/filer/management/commands/generate_thumbnails.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/management/commands/import_files.py` & `django-filer-3.0.3/filer/management/commands/import_files.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/migrations/0001_initial.py` & `django-filer-3.0.3/filer/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/migrations/0002_auto_20150606_2003.py` & `django-filer-3.0.3/filer/migrations/0002_auto_20150606_2003.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/migrations/0003_thumbnailoption.py` & `django-filer-3.0.3/filer/migrations/0003_thumbnailoption.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/migrations/0005_auto_20160623_1425.py` & `django-filer-3.0.3/filer/migrations/0005_auto_20160623_1425.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/migrations/0006_auto_20160623_1627.py` & `django-filer-3.0.3/filer/migrations/0006_auto_20160623_1627.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/migrations/0008_auto_20171117_1313.py` & `django-filer-3.0.3/filer/migrations/0008_auto_20171117_1313.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/migrations/0010_auto_20180414_2058.py` & `django-filer-3.0.3/filer/migrations/0010_auto_20180414_2058.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/migrations/0011_auto_20190418_0137.py` & `django-filer-3.0.3/filer/migrations/0011_auto_20190418_0137.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/migrations/0012_file_mime_type.py` & `django-filer-3.0.3/filer/migrations/0012_file_mime_type.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/migrations/0013_image_width_height_to_float.py` & `django-filer-3.0.3/filer/migrations/0013_image_width_height_to_float.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/migrations/0014_folder_permission_choices.py` & `django-filer-3.0.3/filer/migrations/0014_folder_permission_choices.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/migrations/0015_alter_file_owner_alter_file_polymorphic_ctype_and_more.py` & `django-filer-3.0.3/filer/migrations/0015_alter_file_owner_alter_file_polymorphic_ctype_and_more.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/migrations/0016_alter_folder_index_together_remove_folder_level_and_more.py` & `django-filer-3.0.3/filer/migrations/0016_alter_folder_index_together_remove_folder_level_and_more.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/models/abstract.py` & `django-filer-3.0.3/filer/models/abstract.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/models/clipboardmodels.py` & `django-filer-3.0.3/filer/models/clipboardmodels.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/models/filemodels.py` & `django-filer-3.0.3/filer/models/filemodels.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/models/foldermodels.py` & `django-filer-3.0.3/filer/models/foldermodels.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/models/imagemodels.py` & `django-filer-3.0.3/filer/models/imagemodels.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/models/mixins.py` & `django-filer-3.0.3/filer/models/mixins.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/models/thumbnailoptionmodels.py` & `django-filer-3.0.3/filer/models/thumbnailoptionmodels.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/models/tools.py` & `django-filer-3.0.3/filer/models/tools.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/models/virtualitems.py` & `django-filer-3.0.3/filer/models/virtualitems.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/server/backends/base.py` & `django-filer-3.0.3/filer/server/backends/base.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/server/backends/default.py` & `django-filer-3.0.3/filer/server/backends/default.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/server/backends/nginx.py` & `django-filer-3.0.3/filer/server/backends/nginx.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/server/backends/xsendfile.py` & `django-filer-3.0.3/filer/server/backends/xsendfile.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/server/views.py` & `django-filer-3.0.3/filer/server/views.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/settings.py` & `django-filer-3.0.3/filer/settings.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/static/filer/css/admin_filer.cms.icons.css` & `django-filer-3.0.3/filer/static/filer/css/admin_filer.cms.icons.css`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/static/filer/css/admin_filer.css` & `django-filer-3.0.3/filer/static/filer/css/admin_filer.css`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/static/filer/css/admin_filer.fa.icons.css` & `django-filer-3.0.3/filer/static/filer/css/admin_filer.fa.icons.css`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/static/filer/css/maps/admin_filer.cms.icons.css.map` & `django-filer-3.0.3/filer/static/filer/css/maps/admin_filer.cms.icons.css.map`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/static/filer/css/maps/admin_filer.css.map` & `django-filer-3.0.3/filer/static/filer/css/maps/admin_filer.css.map`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/static/filer/css/maps/admin_filer.fa.icons.css.map` & `django-filer-3.0.3/filer/static/filer/css/maps/admin_filer.fa.icons.css.map`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/static/filer/css/maps/admin_filer.icons.css.map` & `django-filer-3.0.3/filer/static/filer/css/maps/admin_filer.icons.css.map`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/static/filer/fonts/FontAwesome.otf` & `django-filer-3.0.3/filer/static/filer/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/static/filer/fonts/django-filer-iconfont.eot` & `django-filer-3.0.3/filer/static/filer/fonts/django-filer-iconfont.eot`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/static/filer/fonts/django-filer-iconfont.svg` & `django-filer-3.0.3/filer/static/filer/fonts/django-filer-iconfont.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/static/filer/fonts/django-filer-iconfont.ttf` & `django-filer-3.0.3/filer/static/filer/fonts/django-filer-iconfont.ttf`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/static/filer/fonts/django-filer-iconfont.woff` & `django-filer-3.0.3/filer/static/filer/fonts/django-filer-iconfont.woff`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/static/filer/fonts/django-filer-iconfont.woff2` & `django-filer-3.0.3/filer/static/filer/fonts/django-filer-iconfont.woff2`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/static/filer/fonts/fontawesome-webfont.eot` & `django-filer-3.0.3/filer/static/filer/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/static/filer/fonts/fontawesome-webfont.svg` & `django-filer-3.0.3/filer/static/filer/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/static/filer/fonts/fontawesome-webfont.ttf` & `django-filer-3.0.3/filer/static/filer/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/static/filer/fonts/fontawesome-webfont.woff` & `django-filer-3.0.3/filer/static/filer/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/static/filer/fonts/fontawesome-webfont.woff2` & `django-filer-3.0.3/filer/static/filer/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/static/filer/fonts/src/arrow-down.svg` & `django-filer-3.0.3/filer/static/filer/fonts/src/arrow-down.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/static/filer/fonts/src/link.svg` & `django-filer-3.0.3/filer/static/filer/fonts/src/link.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/static/filer/fonts/src/move-to-folder.svg` & `django-filer-3.0.3/filer/static/filer/fonts/src/move-to-folder.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/static/filer/fonts/src/th-list.svg` & `django-filer-3.0.3/filer/static/filer/fonts/src/th-list.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/static/filer/fonts/src/upload.svg` & `django-filer-3.0.3/filer/static/filer/fonts/src/upload.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/static/filer/icons/cloud-up.svg` & `django-filer-3.0.3/filer/static/filer/icons/cloud-up.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/static/filer/icons/file-audio.svg` & `django-filer-3.0.3/filer/static/filer/icons/file-audio.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/static/filer/icons/file-empty.svg` & `django-filer-3.0.3/filer/static/filer/icons/file-empty.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/static/filer/icons/file-font.svg` & `django-filer-3.0.3/filer/static/filer/icons/file-font.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/static/filer/icons/file-missing.svg` & `django-filer-3.0.3/filer/static/filer/icons/file-missing.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/static/filer/icons/file-pdf.svg` & `django-filer-3.0.3/filer/static/filer/icons/file-pdf.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/static/filer/icons/file-picture.svg` & `django-filer-3.0.3/filer/static/filer/icons/file-picture.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/static/filer/icons/file-unknown.svg` & `django-filer-3.0.3/filer/static/filer/icons/file-unknown.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/static/filer/icons/file-video.svg` & `django-filer-3.0.3/filer/static/filer/icons/file-video.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/static/filer/icons/file-zip.svg` & `django-filer-3.0.3/filer/static/filer/icons/file-zip.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/static/filer/icons/folder-dropdown.svg` & `django-filer-3.0.3/filer/static/filer/icons/folder-dropdown.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/static/filer/icons/folder-root.svg` & `django-filer-3.0.3/filer/static/filer/icons/folder-root.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/static/filer/icons/folder-unfiled.svg` & `django-filer-3.0.3/filer/static/filer/icons/folder-unfiled.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/static/filer/icons/folder.svg` & `django-filer-3.0.3/filer/static/filer/icons/folder.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/static/filer/img/icon_changelink.gif` & `django-filer-3.0.3/filer/static/filer/img/icon_changelink.gif`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/static/filer/img/icon_deletelink.gif` & `django-filer-3.0.3/filer/static/filer/img/icon_deletelink.gif`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/static/filer/img/loading_animation.gif` & `django-filer-3.0.3/filer/static/filer/img/loading_animation.gif`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/static/filer/img/upload_button.png` & `django-filer-3.0.3/filer/static/filer/img/upload_button.png`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/static/filer/js/addons/copy-move-files.js` & `django-filer-3.0.3/filer/static/filer/js/addons/copy-move-files.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/static/filer/js/addons/dropdown-menu.js` & `django-filer-3.0.3/filer/static/filer/js/addons/dropdown-menu.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/static/filer/js/addons/dropzone.init.js` & `django-filer-3.0.3/filer/static/filer/js/addons/dropzone.init.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/static/filer/js/addons/filer_popup_response.js` & `django-filer-3.0.3/filer/static/filer/js/addons/filer_popup_response.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/static/filer/js/addons/focal-point.js` & `django-filer-3.0.3/filer/static/filer/js/addons/focal-point.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/static/filer/js/addons/popup_handling.js` & `django-filer-3.0.3/filer/static/filer/js/addons/popup_handling.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/static/filer/js/addons/table-dropzone.js` & `django-filer-3.0.3/filer/static/filer/js/addons/table-dropzone.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/static/filer/js/addons/toggler.js` & `django-filer-3.0.3/filer/static/filer/js/addons/toggler.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/static/filer/js/addons/tooltip.js` & `django-filer-3.0.3/filer/static/filer/js/addons/tooltip.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/static/filer/js/addons/upload-button.js` & `django-filer-3.0.3/filer/static/filer/js/addons/upload-button.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/static/filer/js/addons/widget.js` & `django-filer-3.0.3/filer/static/filer/js/addons/widget.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/static/filer/js/base.js` & `django-filer-3.0.3/filer/static/filer/js/base.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/static/filer/js/libs/class.min.js` & `django-filer-3.0.3/filer/static/filer/js/libs/class.min.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/static/filer/js/libs/dropzone.min.js` & `django-filer-3.0.3/filer/static/filer/js/libs/dropzone.min.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/static/filer/js/libs/fileuploader.min.js` & `django-filer-3.0.3/filer/static/filer/js/libs/fileuploader.min.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/static/filer/js/libs/jquery-ui.min.js` & `django-filer-3.0.3/filer/static/filer/js/libs/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/static/filer/js/libs/jquery.cookie.min.js` & `django-filer-3.0.3/filer/static/filer/js/libs/jquery.cookie.min.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/static/filer/js/libs/jquery.min.js` & `django-filer-3.0.3/filer/static/filer/js/libs/jquery.min.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/static/filer/js/libs/mediator.min.js` & `django-filer-3.0.3/filer/static/filer/js/libs/mediator.min.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/storage.py` & `django-filer-3.0.3/filer/storage.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/templates/admin/filer/actions.html` & `django-filer-3.0.3/filer/templates/admin/filer/actions.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/templates/admin/filer/base_site.html` & `django-filer-3.0.3/filer/templates/admin/filer/base_site.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/templates/admin/filer/breadcrumbs.html` & `django-filer-3.0.3/filer/templates/admin/filer/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/templates/admin/filer/change_form.html` & `django-filer-3.0.3/filer/templates/admin/filer/change_form.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/templates/admin/filer/delete_selected_files_confirmation.html` & `django-filer-3.0.3/filer/templates/admin/filer/delete_selected_files_confirmation.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/templates/admin/filer/file/change_form.html` & `django-filer-3.0.3/filer/templates/admin/filer/file/change_form.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/templates/admin/filer/folder/change_form.html` & `django-filer-3.0.3/filer/templates/admin/filer/folder/change_form.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/templates/admin/filer/folder/choose_copy_destination.html` & `django-filer-3.0.3/filer/templates/admin/filer/folder/choose_copy_destination.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/templates/admin/filer/folder/choose_images_resize_options.html` & `django-filer-3.0.3/filer/templates/admin/filer/folder/choose_images_resize_options.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/templates/admin/filer/folder/choose_move_destination.html` & `django-filer-3.0.3/filer/templates/admin/filer/folder/choose_move_destination.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/templates/admin/filer/folder/choose_rename_format.html` & `django-filer-3.0.3/filer/templates/admin/filer/folder/choose_rename_format.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/templates/admin/filer/folder/directory_listing.html` & `django-filer-3.0.3/filer/templates/admin/filer/folder/directory_listing.html`

 * *Files 2% similar despite different names*

```diff
@@ -242,15 +242,15 @@
                 {% endblock %}
             </div>
         </div>
     </div>
     <div id="content-main">
         {% include "admin/filer/tools/search_form.html" %}
         <div class="js-navigator navigator{% if not actions_on_top and not actions_on_bottom %}navigator-no-actions{% endif %}">
-            <form class="js-navigator-form" method="post">
+            <form class="js-navigator-form" method="post" id="changelist-form">
                 {% csrf_token %}
                 {% filer_admin_context_hidden_formfields %}
                 {% if action_form and actions_on_top and paginator.count and not is_popup %}
                     {% filer_actions %}
                 {% endif %}
                 {% include list_type_template %}
                 {% if action_form and actions_on_bottom and paginator.count and not is_popup %}
```

### Comparing `django-filer-3.0.2/filer/templates/admin/filer/folder/directory_table_list.html` & `django-filer-3.0.3/filer/templates/admin/filer/folder/directory_table_list.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/templates/admin/filer/folder/directory_thumbnail_list.html` & `django-filer-3.0.3/filer/templates/admin/filer/folder/directory_thumbnail_list.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/templates/admin/filer/folder/new_folder_form.html` & `django-filer-3.0.3/filer/templates/admin/filer/folder/new_folder_form.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/templates/admin/filer/image/change_form.html` & `django-filer-3.0.3/filer/templates/admin/filer/image/change_form.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/templates/admin/filer/templatetags/file_icon.html` & `django-filer-3.0.3/filer/templates/admin/filer/templatetags/file_icon.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/templates/admin/filer/tools/clipboard/clipboard.html` & `django-filer-3.0.3/filer/templates/admin/filer/tools/clipboard/clipboard.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/templates/admin/filer/tools/clipboard/clipboard_item_rows.html` & `django-filer-3.0.3/filer/templates/admin/filer/tools/clipboard/clipboard_item_rows.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/templates/admin/filer/tools/detail_info.html` & `django-filer-3.0.3/filer/templates/admin/filer/tools/detail_info.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/templates/admin/filer/tools/search_form.html` & `django-filer-3.0.3/filer/templates/admin/filer/tools/search_form.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/templates/admin/filer/widgets/admin_file.html` & `django-filer-3.0.3/filer/templates/admin/filer/widgets/admin_file.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/templates/admin/filer/widgets/admin_folder.html` & `django-filer-3.0.3/filer/templates/admin/filer/widgets/admin_folder.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/templatetags/filer_admin_tags.py` & `django-filer-3.0.3/filer/templatetags/filer_admin_tags.py`

 * *Files 5% similar despite different names*

```diff
@@ -96,20 +96,15 @@
 
 def file_icon_context(file, detail, width, height):
     mime_maintype, mime_subtype = file.mime_maintype, file.mime_subtype
     context = {
         'mime_maintype': mime_maintype,
         'mime_type': file.mime_type,
     }
-    # Get download_url and aspect ratio right for detail view
-    if detail:
-        context['download_url'] = file.url
-        if file.width:
-            width, height = 210, ceil(210 / file.width * file.height)
-            context['sidebar_image_ratio'] = file.width / 210
+    height, width, context = get_aspect_ratio_and_download_url(context, detail, file, height, width)
     # returned context if icon is not available
     not_available_context = {
         'icon_url': staticfiles_storage.url('filer/icons/file-missing.svg'),
         'alt_text': _("File is missing"),
         'width': width,
         'height': width,  # The icon is a square
     }
@@ -164,14 +159,28 @@
     else:
         icon_url = staticfiles_storage.url('filer/icons/file-unknown.svg')
         height = width  # icon is a square
     context.update(width=width, height=height, icon_url=icon_url)
     return context
 
 
+def get_aspect_ratio_and_download_url(context, detail, file, height, width):
+    # Get download_url and aspect ratio right for detail view
+    if detail:
+        context['download_url'] = file.url
+        if isinstance(file, BaseImage):
+            # only check for file width, if the file
+            # is actually an image and not on other files
+            # because they don't really have width or height
+            if file.width:
+                width, height = 210, ceil(210 / file.width * file.height)
+                context['sidebar_image_ratio'] = file.width / 210
+    return height, width, context
+
+
 @register.inclusion_tag('admin/filer/templatetags/file_icon.html')
 def file_icon(file, detail=False, size=None):
     """
     This templatetag returns a rendered `<img src="..." srcset="..." width="..." height="..." class="..." />
     to be used for rendering thumbnails of files in the directory listing or in the corresponding detail
     views for that image.
     """
```

### Comparing `django-filer-3.0.2/filer/templatetags/filer_image_tags.py` & `django-filer-3.0.3/filer/templatetags/filer_image_tags.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/templatetags/filer_tags.py` & `django-filer-3.0.3/filer/templatetags/filer_tags.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/thumbnail_processors.py` & `django-filer-3.0.3/filer/thumbnail_processors.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/utils/compatibility.py` & `django-filer-3.0.3/filer/utils/compatibility.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/utils/filer_easy_thumbnails.py` & `django-filer-3.0.3/filer/utils/filer_easy_thumbnails.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/utils/files.py` & `django-filer-3.0.3/filer/utils/files.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/utils/generate_filename.py` & `django-filer-3.0.3/filer/utils/generate_filename.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/utils/loader.py` & `django-filer-3.0.3/filer/utils/loader.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/utils/pil_exif.py` & `django-filer-3.0.3/filer/utils/pil_exif.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/utils/recursive_dictionary.py` & `django-filer-3.0.3/filer/utils/recursive_dictionary.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/utils/zip.py` & `django-filer-3.0.3/filer/utils/zip.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/filer/validation.py` & `django-filer-3.0.3/filer/validation.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/setup.cfg` & `django-filer-3.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.2/setup.py` & `django-filer-3.0.3/setup.py`

 * *Files identical despite different names*

