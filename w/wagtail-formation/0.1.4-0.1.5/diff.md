# Comparing `tmp/wagtail_formation-0.1.4.tar.gz` & `tmp/wagtail_formation-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_formation-0.1.4.tar", last modified: Tue Jul 11 09:15:52 2023, max compression
+gzip compressed data, was "wagtail_formation-0.1.5.tar", last modified: Fri Jul 21 12:42:38 2023, max compression
```

## Comparing `wagtail_formation-0.1.4.tar` & `wagtail_formation-0.1.5.tar`

### file list

```diff
@@ -1,114 +1,115 @@
-drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.319411 wagtail_formation-0.1.4/
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     3634 2023-03-06 10:30:05.000000 wagtail_formation-0.1.4/CONTRIBUTING.rst
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      336 2023-07-11 08:36:32.000000 wagtail_formation-0.1.4/HISTORY.rst
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     1074 2023-03-06 10:30:05.000000 wagtail_formation-0.1.4/LICENSE
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      272 2023-03-21 16:47:55.000000 wagtail_formation-0.1.4/MANIFEST.in
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     1672 2023-07-11 09:15:52.319494 wagtail_formation-0.1.4/PKG-INFO
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      953 2023-03-06 10:30:05.000000 wagtail_formation-0.1.4/README.rst
-drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.288680 wagtail_formation-0.1.4/docs/
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)       65 2023-03-06 16:36:34.000000 wagtail_formation-0.1.4/docs/Makefile
-drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.280991 wagtail_formation-0.1.4/docs/docs/
-drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.293606 wagtail_formation-0.1.4/docs/docs/images/
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)    39962 2023-03-14 16:42:18.000000 wagtail_formation-0.1.4/docs/docs/images/simpleform_basic.png
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)   475616 2023-03-14 16:43:07.000000 wagtail_formation-0.1.4/docs/docs/images/simpleform_silly.png
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)   145908 2023-03-14 16:55:35.000000 wagtail_formation-0.1.4/docs/docs/images/simpleform_verysilly.png
-drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.297576 wagtail_formation-0.1.4/formation/
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)       22 2023-07-11 08:32:24.000000 wagtail_formation-0.1.4/formation/__init__.py
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      150 2023-03-06 10:32:38.000000 wagtail_formation-0.1.4/formation/apps.py
-drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.298719 wagtail_formation-0.1.4/formation/blocks/
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      871 2023-03-06 10:32:38.000000 wagtail_formation-0.1.4/formation/blocks/__init__.py
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     4330 2023-07-11 08:29:47.000000 wagtail_formation-0.1.4/formation/blocks/fields.py
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     3349 2023-07-11 08:29:47.000000 wagtail_formation-0.1.4/formation/blocks/forms.py
-drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.299948 wagtail_formation-0.1.4/formation/migrations/
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      545 2023-03-06 10:32:38.000000 wagtail_formation-0.1.4/formation/migrations/0001_initial.py
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     2460 2023-03-06 10:32:38.000000 wagtail_formation-0.1.4/formation/migrations/0002_reusableform_name_alter_reusableform_form_content.py
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      465 2023-06-30 08:58:46.000000 wagtail_formation-0.1.4/formation/migrations/0003_alter_reusableform_form_content.py
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-03-06 10:32:38.000000 wagtail_formation-0.1.4/formation/migrations/__init__.py
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      457 2023-06-30 08:57:28.000000 wagtail_formation-0.1.4/formation/models.py
-drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.281555 wagtail_formation-0.1.4/formation/static/
-drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.300130 wagtail_formation-0.1.4/formation/static/js/
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      712 2023-03-15 14:38:38.000000 wagtail_formation-0.1.4/formation/static/js/formation.js
-drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.281749 wagtail_formation-0.1.4/formation/templates/
-drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.300609 wagtail_formation-0.1.4/formation/templates/formation/
-drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.303673 wagtail_formation-0.1.4/formation/templates/formation/blocks/
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      392 2023-03-06 10:32:38.000000 wagtail_formation-0.1.4/formation/templates/formation/blocks/base_field.html
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      343 2023-07-11 08:29:47.000000 wagtail_formation-0.1.4/formation/templates/formation/blocks/base_form.html
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      182 2023-03-06 10:32:38.000000 wagtail_formation-0.1.4/formation/templates/formation/blocks/boolean_field.html
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      178 2023-03-06 10:32:38.000000 wagtail_formation-0.1.4/formation/templates/formation/blocks/date_field.html
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      188 2023-03-06 10:32:38.000000 wagtail_formation-0.1.4/formation/templates/formation/blocks/datetime_field.html
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      178 2023-03-06 10:32:38.000000 wagtail_formation-0.1.4/formation/templates/formation/blocks/email_field.html
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      180 2023-03-06 10:32:38.000000 wagtail_formation-0.1.4/formation/templates/formation/blocks/integer_field.html
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      439 2023-03-06 10:32:38.000000 wagtail_formation-0.1.4/formation/templates/formation/blocks/radio_field.html
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      269 2023-03-06 10:32:38.000000 wagtail_formation-0.1.4/formation/templates/formation/blocks/select_field.html
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)       66 2023-03-06 10:32:38.000000 wagtail_formation-0.1.4/formation/templates/formation/blocks/submit_button.html
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      178 2023-03-06 10:32:38.000000 wagtail_formation-0.1.4/formation/templates/formation/blocks/text_field.html
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      169 2023-03-06 10:32:38.000000 wagtail_formation-0.1.4/formation/templates/formation/blocks/textarea_field.html
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      121 2023-03-06 10:32:38.000000 wagtail_formation-0.1.4/formation/templates/formation/reusable_form.html
-drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.304419 wagtail_formation-0.1.4/formation/templatetags/
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-03-06 10:32:38.000000 wagtail_formation-0.1.4/formation/templatetags/__init__.py
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      729 2023-03-15 15:40:50.000000 wagtail_formation-0.1.4/formation/templatetags/formation_tags.py
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      190 2023-03-15 14:42:53.000000 wagtail_formation-0.1.4/formation/urls.py
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     2917 2023-03-17 13:04:05.000000 wagtail_formation-0.1.4/formation/utils.py
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     1169 2023-06-30 12:51:44.000000 wagtail_formation-0.1.4/formation/views.py
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      464 2023-03-06 10:32:38.000000 wagtail_formation-0.1.4/formation/wagtail_hooks.py
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      366 2023-03-06 10:32:38.000000 wagtail_formation-0.1.4/formation/widgets.py
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      429 2023-07-11 09:15:52.321385 wagtail_formation-0.1.4/setup.cfg
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     1328 2023-07-11 09:13:33.000000 wagtail_formation-0.1.4/setup.py
-drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.304747 wagtail_formation-0.1.4/tests/
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)       47 2023-03-06 10:30:05.000000 wagtail_formation-0.1.4/tests/__init__.py
-drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.306627 wagtail_formation-0.1.4/tests/testproject/
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      376 2023-03-17 08:55:07.000000 wagtail_formation-0.1.4/tests/testproject/.dockerignore
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     2034 2023-03-17 08:55:07.000000 wagtail_formation-0.1.4/tests/testproject/Dockerfile
-drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.307628 wagtail_formation-0.1.4/tests/testproject/home/
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-03-17 08:55:07.000000 wagtail_formation-0.1.4/tests/testproject/home/__init__.py
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     1048 2023-03-17 09:56:24.000000 wagtail_formation-0.1.4/tests/testproject/home/blocks.py
-drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.308869 wagtail_formation-0.1.4/tests/testproject/home/migrations/
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      830 2023-03-17 08:55:07.000000 wagtail_formation-0.1.4/tests/testproject/home/migrations/0001_initial.py
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     1741 2023-03-17 11:53:14.000000 wagtail_formation-0.1.4/tests/testproject/home/migrations/0002_create_homepage.py
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     1306 2023-03-17 11:57:04.000000 wagtail_formation-0.1.4/tests/testproject/home/migrations/0003_homepage_content.py
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-03-17 08:55:07.000000 wagtail_formation-0.1.4/tests/testproject/home/migrations/__init__.py
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      392 2023-03-17 09:55:52.000000 wagtail_formation-0.1.4/tests/testproject/home/models.py
-drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.282860 wagtail_formation-0.1.4/tests/testproject/home/static/
-drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.309146 wagtail_formation-0.1.4/tests/testproject/home/static/css/
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     2522 2023-03-17 08:55:07.000000 wagtail_formation-0.1.4/tests/testproject/home/static/css/welcome_page.css
-drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.283098 wagtail_formation-0.1.4/tests/testproject/home/templates/
-drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.309823 wagtail_formation-0.1.4/tests/testproject/home/templates/home/
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      232 2023-03-17 12:27:18.000000 wagtail_formation-0.1.4/tests/testproject/home/templates/home/home_page.html
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     6421 2023-03-17 08:55:07.000000 wagtail_formation-0.1.4/tests/testproject/home/templates/home/welcome_page.html
--rwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      388 2023-03-17 09:40:47.000000 wagtail_formation-0.1.4/tests/testproject/manage.py
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)       35 2023-03-17 08:55:07.000000 wagtail_formation-0.1.4/tests/testproject/requirements.txt
-drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.310735 wagtail_formation-0.1.4/tests/testproject/search/
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-03-17 08:55:07.000000 wagtail_formation-0.1.4/tests/testproject/search/__init__.py
-drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.283548 wagtail_formation-0.1.4/tests/testproject/search/templates/
-drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.311258 wagtail_formation-0.1.4/tests/testproject/search/templates/search/
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     1097 2023-03-17 08:55:07.000000 wagtail_formation-0.1.4/tests/testproject/search/templates/search/search.html
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     1019 2023-03-17 08:55:07.000000 wagtail_formation-0.1.4/tests/testproject/search/views.py
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      662 2023-03-17 12:18:02.000000 wagtail_formation-0.1.4/tests/testproject/testbed.json
-drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.312126 wagtail_formation-0.1.4/tests/testproject/testproject/
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-03-17 08:55:07.000000 wagtail_formation-0.1.4/tests/testproject/testproject/__init__.py
-drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.313093 wagtail_formation-0.1.4/tests/testproject/testproject/settings/
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-03-17 08:55:07.000000 wagtail_formation-0.1.4/tests/testproject/testproject/settings/__init__.py
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     4510 2023-03-17 12:33:26.000000 wagtail_formation-0.1.4/tests/testproject/testproject/settings/base.py
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      460 2023-03-17 08:55:07.000000 wagtail_formation-0.1.4/tests/testproject/testproject/settings/dev.py
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)       95 2023-03-17 08:55:07.000000 wagtail_formation-0.1.4/tests/testproject/testproject/settings/production.py
-drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.284369 wagtail_formation-0.1.4/tests/testproject/testproject/static/
-drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.313320 wagtail_formation-0.1.4/tests/testproject/testproject/static/css/
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-03-17 08:55:07.000000 wagtail_formation-0.1.4/tests/testproject/testproject/static/css/testproject.css
-drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.313529 wagtail_formation-0.1.4/tests/testproject/testproject/static/js/
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-03-17 08:55:07.000000 wagtail_formation-0.1.4/tests/testproject/testproject/static/js/testproject.js
-drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.314307 wagtail_formation-0.1.4/tests/testproject/testproject/templates/
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      230 2023-03-17 08:55:07.000000 wagtail_formation-0.1.4/tests/testproject/testproject/templates/404.html
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      369 2023-03-17 08:55:07.000000 wagtail_formation-0.1.4/tests/testproject/testproject/templates/500.html
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     1607 2023-03-17 12:27:41.000000 wagtail_formation-0.1.4/tests/testproject/testproject/templates/base.html
-drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.314830 wagtail_formation-0.1.4/tests/testproject/testproject/tests/
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-03-17 09:47:40.000000 wagtail_formation-0.1.4/tests/testproject/testproject/tests/__init__.py
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     1289 2023-03-17 12:55:57.000000 wagtail_formation-0.1.4/tests/testproject/testproject/tests/test_basic.py
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     1340 2023-03-17 12:13:58.000000 wagtail_formation-0.1.4/tests/testproject/testproject/urls.py
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      403 2023-03-17 08:55:07.000000 wagtail_formation-0.1.4/tests/testproject/testproject/wsgi.py
-drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.319298 wagtail_formation-0.1.4/wagtail_formation.egg-info/
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     1672 2023-07-11 09:15:52.000000 wagtail_formation-0.1.4/wagtail_formation.egg-info/PKG-INFO
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     3169 2023-07-11 09:15:52.000000 wagtail_formation-0.1.4/wagtail_formation.egg-info/SOURCES.txt
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        1 2023-07-11 09:15:52.000000 wagtail_formation-0.1.4/wagtail_formation.egg-info/dependency_links.txt
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        1 2023-07-11 09:15:52.000000 wagtail_formation-0.1.4/wagtail_formation.egg-info/not-zip-safe
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)       52 2023-07-11 09:15:52.000000 wagtail_formation-0.1.4/wagtail_formation.egg-info/requires.txt
--rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)       10 2023-07-11 09:15:52.000000 wagtail_formation-0.1.4/wagtail_formation.egg-info/top_level.txt
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-21 12:42:38.016143 wagtail_formation-0.1.5/
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     3634 2023-03-06 10:30:05.000000 wagtail_formation-0.1.5/CONTRIBUTING.rst
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      483 2023-07-21 12:40:23.000000 wagtail_formation-0.1.5/HISTORY.rst
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     1074 2023-03-06 10:30:05.000000 wagtail_formation-0.1.5/LICENSE
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      272 2023-03-21 16:47:55.000000 wagtail_formation-0.1.5/MANIFEST.in
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     1672 2023-07-21 12:42:38.016253 wagtail_formation-0.1.5/PKG-INFO
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      953 2023-03-06 10:30:05.000000 wagtail_formation-0.1.5/README.rst
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-21 12:42:37.988880 wagtail_formation-0.1.5/docs/
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)       65 2023-03-06 16:36:34.000000 wagtail_formation-0.1.5/docs/Makefile
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-21 12:42:37.981238 wagtail_formation-0.1.5/docs/docs/
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-21 12:42:37.989991 wagtail_formation-0.1.5/docs/docs/images/
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)    39962 2023-03-14 16:42:18.000000 wagtail_formation-0.1.5/docs/docs/images/simpleform_basic.png
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)   475616 2023-03-14 16:43:07.000000 wagtail_formation-0.1.5/docs/docs/images/simpleform_silly.png
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)   145908 2023-03-14 16:55:35.000000 wagtail_formation-0.1.5/docs/docs/images/simpleform_verysilly.png
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-21 12:42:37.991922 wagtail_formation-0.1.5/formation/
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)       22 2023-07-21 12:38:41.000000 wagtail_formation-0.1.5/formation/__init__.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      150 2023-03-06 10:32:38.000000 wagtail_formation-0.1.5/formation/apps.py
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-21 12:42:37.992528 wagtail_formation-0.1.5/formation/blocks/
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      871 2023-03-06 10:32:38.000000 wagtail_formation-0.1.5/formation/blocks/__init__.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     4819 2023-07-13 16:22:09.000000 wagtail_formation-0.1.5/formation/blocks/fields.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     4098 2023-07-18 14:52:15.000000 wagtail_formation-0.1.5/formation/blocks/forms.py
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-21 12:42:37.993328 wagtail_formation-0.1.5/formation/migrations/
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      545 2023-03-06 10:32:38.000000 wagtail_formation-0.1.5/formation/migrations/0001_initial.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     2460 2023-03-06 10:32:38.000000 wagtail_formation-0.1.5/formation/migrations/0002_reusableform_name_alter_reusableform_form_content.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      465 2023-06-30 08:58:46.000000 wagtail_formation-0.1.5/formation/migrations/0003_alter_reusableform_form_content.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-03-06 10:32:38.000000 wagtail_formation-0.1.5/formation/migrations/__init__.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      457 2023-06-30 08:57:28.000000 wagtail_formation-0.1.5/formation/models.py
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-21 12:42:37.982051 wagtail_formation-0.1.5/formation/static/
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-21 12:42:37.993538 wagtail_formation-0.1.5/formation/static/js/
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     1055 2023-07-21 12:37:01.000000 wagtail_formation-0.1.5/formation/static/js/formation.js
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-21 12:42:37.982334 wagtail_formation-0.1.5/formation/templates/
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-21 12:42:37.993841 wagtail_formation-0.1.5/formation/templates/formation/
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-21 12:42:37.997425 wagtail_formation-0.1.5/formation/templates/formation/blocks/
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      392 2023-03-06 10:32:38.000000 wagtail_formation-0.1.5/formation/templates/formation/blocks/base_field.html
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      405 2023-07-18 15:01:30.000000 wagtail_formation-0.1.5/formation/templates/formation/blocks/base_form.html
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      182 2023-03-06 10:32:38.000000 wagtail_formation-0.1.5/formation/templates/formation/blocks/boolean_field.html
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      178 2023-03-06 10:32:38.000000 wagtail_formation-0.1.5/formation/templates/formation/blocks/date_field.html
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      188 2023-03-06 10:32:38.000000 wagtail_formation-0.1.5/formation/templates/formation/blocks/datetime_field.html
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      178 2023-03-06 10:32:38.000000 wagtail_formation-0.1.5/formation/templates/formation/blocks/email_field.html
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      152 2023-07-13 16:28:43.000000 wagtail_formation-0.1.5/formation/templates/formation/blocks/file_field.html
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      180 2023-03-06 10:32:38.000000 wagtail_formation-0.1.5/formation/templates/formation/blocks/integer_field.html
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      439 2023-03-06 10:32:38.000000 wagtail_formation-0.1.5/formation/templates/formation/blocks/radio_field.html
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      269 2023-03-06 10:32:38.000000 wagtail_formation-0.1.5/formation/templates/formation/blocks/select_field.html
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)       66 2023-03-06 10:32:38.000000 wagtail_formation-0.1.5/formation/templates/formation/blocks/submit_button.html
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      178 2023-03-06 10:32:38.000000 wagtail_formation-0.1.5/formation/templates/formation/blocks/text_field.html
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      169 2023-03-06 10:32:38.000000 wagtail_formation-0.1.5/formation/templates/formation/blocks/textarea_field.html
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      121 2023-03-06 10:32:38.000000 wagtail_formation-0.1.5/formation/templates/formation/reusable_form.html
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-21 12:42:37.997849 wagtail_formation-0.1.5/formation/templatetags/
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-03-06 10:32:38.000000 wagtail_formation-0.1.5/formation/templatetags/__init__.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      729 2023-03-15 15:40:50.000000 wagtail_formation-0.1.5/formation/templatetags/formation_tags.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      190 2023-03-15 14:42:53.000000 wagtail_formation-0.1.5/formation/urls.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     2917 2023-03-17 13:04:05.000000 wagtail_formation-0.1.5/formation/utils.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     1701 2023-07-21 12:35:47.000000 wagtail_formation-0.1.5/formation/views.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      464 2023-03-06 10:32:38.000000 wagtail_formation-0.1.5/formation/wagtail_hooks.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      366 2023-03-06 10:32:38.000000 wagtail_formation-0.1.5/formation/widgets.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      429 2023-07-21 12:42:38.018720 wagtail_formation-0.1.5/setup.cfg
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     1328 2023-07-21 12:38:46.000000 wagtail_formation-0.1.5/setup.py
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-21 12:42:37.998387 wagtail_formation-0.1.5/tests/
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)       47 2023-03-06 10:30:05.000000 wagtail_formation-0.1.5/tests/__init__.py
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-21 12:42:37.999814 wagtail_formation-0.1.5/tests/testproject/
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      376 2023-03-17 08:55:07.000000 wagtail_formation-0.1.5/tests/testproject/.dockerignore
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     2034 2023-03-17 08:55:07.000000 wagtail_formation-0.1.5/tests/testproject/Dockerfile
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-21 12:42:38.001180 wagtail_formation-0.1.5/tests/testproject/home/
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-03-17 08:55:07.000000 wagtail_formation-0.1.5/tests/testproject/home/__init__.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     1048 2023-03-17 09:56:24.000000 wagtail_formation-0.1.5/tests/testproject/home/blocks.py
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-21 12:42:38.002246 wagtail_formation-0.1.5/tests/testproject/home/migrations/
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      830 2023-03-17 08:55:07.000000 wagtail_formation-0.1.5/tests/testproject/home/migrations/0001_initial.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     1741 2023-03-17 11:53:14.000000 wagtail_formation-0.1.5/tests/testproject/home/migrations/0002_create_homepage.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     1306 2023-03-17 11:57:04.000000 wagtail_formation-0.1.5/tests/testproject/home/migrations/0003_homepage_content.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-03-17 08:55:07.000000 wagtail_formation-0.1.5/tests/testproject/home/migrations/__init__.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      392 2023-03-17 09:55:52.000000 wagtail_formation-0.1.5/tests/testproject/home/models.py
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-21 12:42:37.983648 wagtail_formation-0.1.5/tests/testproject/home/static/
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-21 12:42:38.002417 wagtail_formation-0.1.5/tests/testproject/home/static/css/
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     2522 2023-03-17 08:55:07.000000 wagtail_formation-0.1.5/tests/testproject/home/static/css/welcome_page.css
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-21 12:42:37.983961 wagtail_formation-0.1.5/tests/testproject/home/templates/
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-21 12:42:38.002831 wagtail_formation-0.1.5/tests/testproject/home/templates/home/
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      232 2023-03-17 12:27:18.000000 wagtail_formation-0.1.5/tests/testproject/home/templates/home/home_page.html
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     6421 2023-03-17 08:55:07.000000 wagtail_formation-0.1.5/tests/testproject/home/templates/home/welcome_page.html
+-rwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      388 2023-03-17 09:40:47.000000 wagtail_formation-0.1.5/tests/testproject/manage.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)       35 2023-03-17 08:55:07.000000 wagtail_formation-0.1.5/tests/testproject/requirements.txt
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-21 12:42:38.003208 wagtail_formation-0.1.5/tests/testproject/search/
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-03-17 08:55:07.000000 wagtail_formation-0.1.5/tests/testproject/search/__init__.py
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-21 12:42:37.984421 wagtail_formation-0.1.5/tests/testproject/search/templates/
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-21 12:42:38.003414 wagtail_formation-0.1.5/tests/testproject/search/templates/search/
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     1097 2023-03-17 08:55:07.000000 wagtail_formation-0.1.5/tests/testproject/search/templates/search/search.html
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     1019 2023-03-17 08:55:07.000000 wagtail_formation-0.1.5/tests/testproject/search/views.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      662 2023-03-17 12:18:02.000000 wagtail_formation-0.1.5/tests/testproject/testbed.json
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-21 12:42:38.005404 wagtail_formation-0.1.5/tests/testproject/testproject/
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-03-17 08:55:07.000000 wagtail_formation-0.1.5/tests/testproject/testproject/__init__.py
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-21 12:42:38.010766 wagtail_formation-0.1.5/tests/testproject/testproject/settings/
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-03-17 08:55:07.000000 wagtail_formation-0.1.5/tests/testproject/testproject/settings/__init__.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     4510 2023-03-17 12:33:26.000000 wagtail_formation-0.1.5/tests/testproject/testproject/settings/base.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      460 2023-03-17 08:55:07.000000 wagtail_formation-0.1.5/tests/testproject/testproject/settings/dev.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)       95 2023-03-17 08:55:07.000000 wagtail_formation-0.1.5/tests/testproject/testproject/settings/production.py
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-21 12:42:37.985355 wagtail_formation-0.1.5/tests/testproject/testproject/static/
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-21 12:42:38.011887 wagtail_formation-0.1.5/tests/testproject/testproject/static/css/
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-03-17 08:55:07.000000 wagtail_formation-0.1.5/tests/testproject/testproject/static/css/testproject.css
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-21 12:42:38.012046 wagtail_formation-0.1.5/tests/testproject/testproject/static/js/
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-03-17 08:55:07.000000 wagtail_formation-0.1.5/tests/testproject/testproject/static/js/testproject.js
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-21 12:42:38.012616 wagtail_formation-0.1.5/tests/testproject/testproject/templates/
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      230 2023-03-17 08:55:07.000000 wagtail_formation-0.1.5/tests/testproject/testproject/templates/404.html
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      369 2023-03-17 08:55:07.000000 wagtail_formation-0.1.5/tests/testproject/testproject/templates/500.html
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     1607 2023-03-17 12:27:41.000000 wagtail_formation-0.1.5/tests/testproject/testproject/templates/base.html
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-21 12:42:38.013072 wagtail_formation-0.1.5/tests/testproject/testproject/tests/
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-03-17 09:47:40.000000 wagtail_formation-0.1.5/tests/testproject/testproject/tests/__init__.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     1289 2023-03-17 12:55:57.000000 wagtail_formation-0.1.5/tests/testproject/testproject/tests/test_basic.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     1340 2023-03-17 12:13:58.000000 wagtail_formation-0.1.5/tests/testproject/testproject/urls.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      403 2023-03-17 08:55:07.000000 wagtail_formation-0.1.5/tests/testproject/testproject/wsgi.py
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-21 12:42:38.016035 wagtail_formation-0.1.5/wagtail_formation.egg-info/
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     1672 2023-07-21 12:42:37.000000 wagtail_formation-0.1.5/wagtail_formation.egg-info/PKG-INFO
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     3222 2023-07-21 12:42:37.000000 wagtail_formation-0.1.5/wagtail_formation.egg-info/SOURCES.txt
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        1 2023-07-21 12:42:37.000000 wagtail_formation-0.1.5/wagtail_formation.egg-info/dependency_links.txt
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        1 2023-07-21 12:42:37.000000 wagtail_formation-0.1.5/wagtail_formation.egg-info/not-zip-safe
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)       52 2023-07-21 12:42:37.000000 wagtail_formation-0.1.5/wagtail_formation.egg-info/requires.txt
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)       10 2023-07-21 12:42:37.000000 wagtail_formation-0.1.5/wagtail_formation.egg-info/top_level.txt
```

### Comparing `wagtail_formation-0.1.4/CONTRIBUTING.rst` & `wagtail_formation-0.1.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `wagtail_formation-0.1.4/LICENSE` & `wagtail_formation-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_formation-0.1.4/PKG-INFO` & `wagtail_formation-0.1.5/wagtail_formation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: wagtail_formation
-Version: 0.1.4
+Name: wagtail-formation
+Version: 0.1.5
 Summary: Build forms from wagtail blocks
 Home-page: https://github.com/mwesterhof/wagtail_formation
 Author: Marco Westerhof
 Author-email: m.westerhof@lukkien.com
 License: MIT license
 Keywords: wagtail_formation
 Platform: UNKNOWN
```

### Comparing `wagtail_formation-0.1.4/README.rst` & `wagtail_formation-0.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `wagtail_formation-0.1.4/docs/docs/images/simpleform_basic.png` & `wagtail_formation-0.1.5/docs/docs/images/simpleform_basic.png`

 * *Files identical despite different names*

### Comparing `wagtail_formation-0.1.4/docs/docs/images/simpleform_silly.png` & `wagtail_formation-0.1.5/docs/docs/images/simpleform_silly.png`

 * *Files identical despite different names*

### Comparing `wagtail_formation-0.1.4/docs/docs/images/simpleform_verysilly.png` & `wagtail_formation-0.1.5/docs/docs/images/simpleform_verysilly.png`

 * *Files identical despite different names*

### Comparing `wagtail_formation-0.1.4/formation/blocks/__init__.py` & `wagtail_formation-0.1.5/formation/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `wagtail_formation-0.1.4/formation/blocks/fields.py` & `wagtail_formation-0.1.5/formation/blocks/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,40 @@
 import uuid
+from collections import namedtuple
 
 from django import forms
 from wagtail import blocks
 
 
+FieldSpec = namedtuple('FieldSpec', ['name', 'field', 'block'])
+
+
 class FieldBlockBase(blocks.StructBlock):
     is_field_block = True
 
     name = blocks.CharBlock()
     label = blocks.CharBlock()
     is_required = blocks.BooleanBlock(required=False, default=True)
 
     def __init__(self, *args, **kwargs):
         self.field_kwargs = kwargs.pop('field_kwargs', {})
         super().__init__(*args, **kwargs)
 
-    def get_named_field(self, value):
+    def get_field_spec(self, value):
         kwargs = self.field_kwargs.copy()
         kwargs['required'] = value['is_required']
-        return value['name'], self.get_field(value, kwargs)
+
+        return FieldSpec(
+            name=value['name'],
+            field=self.get_field(value, kwargs),
+            block=self
+        )
+
+    def clean_field(self, value):
+        return value
 
     def get_field(self, value, field_kwargs):
         return forms.Field(label=value['label'], required=value['is_required'], **field_kwargs)
 
     def get_context(self, value, parent_context=None):
         context = super().get_context(value, parent_context=parent_context)
         form = context['form']
@@ -136,14 +148,23 @@
         return forms.EmailField(label=value['label'], **field_kwargs)
 
     class Meta:
         template = 'formation/blocks/email_field.html'
         icon = 'mail'
 
 
+class FileFieldBlock(FieldBlockBase):
+    def get_field(self, value, field_kwargs):
+        return forms.FileField(label=value['label'], **field_kwargs)
+
+    class Meta:
+        template = 'formation/blocks/file_field.html'
+        icon = 'doc-full'
+
+
 BASIC_FIELD_SPEC = [
     ('text', TextFieldBlock()),
     ('textarea', TextareaFieldBlock()),
     ('integer', IntegerFieldBlock()),
     ('select', SelectFieldBlock()),
     ('radio', RadioFieldBlock()),
 ]
```

### Comparing `wagtail_formation-0.1.4/formation/blocks/forms.py` & `wagtail_formation-0.1.5/formation/blocks/forms.py`

 * *Files 12% similar despite different names*

```diff
@@ -65,31 +65,52 @@
 
         def _input_block_check(element):
             return getattr(element.block, 'is_field_block', False)
 
         extract_elements_recursive(fields, blocks, _input_block_check, False)
         return blocks
 
+    def clean_form(cls, cleaned_data):
+        return cleaned_data
+
     def _get_form_class(cls, value):
-        blocks = cls._get_fields(value)
+        named_fieldblocks = [
+            element.block.get_field_spec(element)
+            for element in cls._get_fields(value)
+        ]
+
+        def _wrap_clean_field_method(fieldblock):
+            def clean_field(form):
+                return fieldblock.block.clean_field(form.cleaned_data[fieldblock.name])
+            return clean_field
+
+        def clean_form(form):
+            return cls.clean_form(form.cleaned_data)
 
         return type(
             cls._get_form_class_name(),
             (forms.Form,),
             dict(
                 [
-                    element.block.get_named_field(element)
-                    for element in blocks
+                    (fieldblock.name, fieldblock.field)
+                    for fieldblock in named_fieldblocks
+                ] +
+                [
+                    (f'clean_{fieldblock.name}', _wrap_clean_field_method(fieldblock))
+                    for fieldblock in named_fieldblocks
+                ] +
+                [
+                    ('clean', clean_form),
                 ]
             )
         )
 
-    def get_form_instance(cls, value, data=None):
+    def get_form_instance(cls, value, data=None, files=None):
         form_class = cls._get_form_class(value)
-        return form_class(data)
+        return form_class(data, files)
 
     def get_context(self, value, parent_context=None):
         self.id = self._get_block_id(parent_context)
         context = super().get_context(value, parent_context=parent_context)
         form_data = context.get('form_data', None)
         context.update({
             'form': self.get_form_instance(value, form_data),
```

### Comparing `wagtail_formation-0.1.4/formation/migrations/0001_initial.py` & `wagtail_formation-0.1.5/formation/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_formation-0.1.4/formation/migrations/0002_reusableform_name_alter_reusableform_form_content.py` & `wagtail_formation-0.1.5/formation/migrations/0002_reusableform_name_alter_reusableform_form_content.py`

 * *Files identical despite different names*

### Comparing `wagtail_formation-0.1.4/formation/static/js/formation.js` & `wagtail_formation-0.1.5/formation/static/js/formation.js`

 * *Files 25% similar despite different names*

#### js-beautify {}

```diff
@@ -3,24 +3,34 @@
         const csrftoken = Cookies.get('csrftoken');
         var form = $(this);
         var url = form.attr('action');
 
         event.stopPropagation();
         event.preventDefault();
 
+        var formData = new FormData(this);
+
         $.ajax({
             type: "POST",
             url: url,
-            data: form.serialize(),
+            data: formData,
             headers: {
                 'X-CSRFToken': csrftoken
             },
-            success: function(data) {
-                $('form.formation').unbind('submit', handleFormSubmit);
-                form.replaceWith(data);
-                $('form.formation').on('submit', handleFormSubmit);
+            cache: false,
+            processData: false,
+            contentType: false,
+            success: function(data, statusText, response) {
+                if (response.getResponseHeader('formationReplace') == 0) {
+                    window.location.href = data;
+                } else {
+                    $('form.formation').unbind('submit', handleFormSubmit);
+                    form.replaceWith(data);
+                    $('form.formation').on('submit', handleFormSubmit);
+                }
+
             }
         });
     }
 
     $('form.formation').on('submit', handleFormSubmit);
 });
```

### Comparing `wagtail_formation-0.1.4/formation/templatetags/formation_tags.py` & `wagtail_formation-0.1.5/formation/templatetags/formation_tags.py`

 * *Files identical despite different names*

### Comparing `wagtail_formation-0.1.4/formation/utils.py` & `wagtail_formation-0.1.5/formation/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail_formation-0.1.4/formation/views.py` & `wagtail_formation-0.1.5/formation/views.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,45 @@
-from django.http import HttpResponse
+from django.http import HttpResponse, HttpResponseRedirect, HttpResponsePermanentRedirect
 from django.views.generic import View
 from generic_chooser.views import ModelChooserViewSet
 
 from formation.models import ReusableForm
 from formation.utils import find_block_value, token_processor
 
 
+def is_redirect(response):
+    return isinstance(response, HttpResponseRedirect) or isinstance(response, HttpResponsePermanentRedirect)
+
+
 class ProcessBlockFormView(View):
     def post(self, request, *args, **kwargs):
         form_token = request.POST['form_token']
         content_type_id, object_id, block_id = token_processor.unpack_token(form_token)
         block_value = find_block_value(content_type_id, object_id, block_id)
         block = block_value.block
-        form = block.get_form_instance(block_value, request.POST)
+        form = block.get_form_instance(block_value, request.POST, request.FILES)
 
         if form.is_valid():
             form_success = True
-            block.form_valid(block_value, form)
+            block_response = block.form_valid(block_value, form)
         else:
             form_success = False
-            block.form_invalid(block_value, form)
+            block_response = block.form_invalid(block_value, form)
+
+        if is_redirect(block_response):  # block form handler decided to bypass AJAX
+            response = HttpResponse(block_response.url)
+            response['formationReplace'] = 0
+            return response
 
         result = block_value.render_as_block({
             'form_success': form_success,
             'form_data': request.POST,
             'form_token': form_token,
         })
-        return HttpResponse(result)
+        response = HttpResponse(result)
+        response.headers['formationReplace'] = 1
+        return response
 
 
 class ReusableFormChooserViewSet(ModelChooserViewSet):
     model = ReusableForm
     fields = ['name', 'form_content']
```

### Comparing `wagtail_formation-0.1.4/setup.py` & `wagtail_formation-0.1.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -39,10 +39,10 @@
     include_package_data=True,
     keywords='wagtail_formation',
     name='wagtail_formation',
     packages=find_packages(include=['formation', 'formation.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/mwesterhof/wagtail_formation',
-    version='0.1.4',
+    version='0.1.5',
     zip_safe=False,
 )
```

### Comparing `wagtail_formation-0.1.4/tests/testproject/Dockerfile` & `wagtail_formation-0.1.5/tests/testproject/Dockerfile`

 * *Files identical despite different names*

### Comparing `wagtail_formation-0.1.4/tests/testproject/home/blocks.py` & `wagtail_formation-0.1.5/tests/testproject/home/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_formation-0.1.4/tests/testproject/home/migrations/0001_initial.py` & `wagtail_formation-0.1.5/tests/testproject/home/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_formation-0.1.4/tests/testproject/home/migrations/0002_create_homepage.py` & `wagtail_formation-0.1.5/tests/testproject/home/migrations/0002_create_homepage.py`

 * *Files identical despite different names*

### Comparing `wagtail_formation-0.1.4/tests/testproject/home/migrations/0003_homepage_content.py` & `wagtail_formation-0.1.5/tests/testproject/home/migrations/0003_homepage_content.py`

 * *Files identical despite different names*

### Comparing `wagtail_formation-0.1.4/tests/testproject/home/static/css/welcome_page.css` & `wagtail_formation-0.1.5/tests/testproject/home/static/css/welcome_page.css`

 * *Files identical despite different names*

### Comparing `wagtail_formation-0.1.4/tests/testproject/home/templates/home/welcome_page.html` & `wagtail_formation-0.1.5/tests/testproject/home/templates/home/welcome_page.html`

 * *Files identical despite different names*

### Comparing `wagtail_formation-0.1.4/tests/testproject/search/templates/search/search.html` & `wagtail_formation-0.1.5/tests/testproject/search/templates/search/search.html`

 * *Files identical despite different names*

### Comparing `wagtail_formation-0.1.4/tests/testproject/search/views.py` & `wagtail_formation-0.1.5/tests/testproject/search/views.py`

 * *Files identical despite different names*

### Comparing `wagtail_formation-0.1.4/tests/testproject/testbed.json` & `wagtail_formation-0.1.5/tests/testproject/testbed.json`

 * *Files identical despite different names*

### Comparing `wagtail_formation-0.1.4/tests/testproject/testproject/settings/base.py` & `wagtail_formation-0.1.5/tests/testproject/testproject/settings/base.py`

 * *Files identical despite different names*

### Comparing `wagtail_formation-0.1.4/tests/testproject/testproject/templates/base.html` & `wagtail_formation-0.1.5/tests/testproject/testproject/templates/base.html`

 * *Files identical despite different names*

### Comparing `wagtail_formation-0.1.4/tests/testproject/testproject/tests/test_basic.py` & `wagtail_formation-0.1.5/tests/testproject/testproject/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `wagtail_formation-0.1.4/tests/testproject/testproject/urls.py` & `wagtail_formation-0.1.5/tests/testproject/testproject/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_formation-0.1.4/wagtail_formation.egg-info/PKG-INFO` & `wagtail_formation-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: wagtail-formation
-Version: 0.1.4
+Name: wagtail_formation
+Version: 0.1.5
 Summary: Build forms from wagtail blocks
 Home-page: https://github.com/mwesterhof/wagtail_formation
 Author: Marco Westerhof
 Author-email: m.westerhof@lukkien.com
 License: MIT license
 Keywords: wagtail_formation
 Platform: UNKNOWN
```

### Comparing `wagtail_formation-0.1.4/wagtail_formation.egg-info/SOURCES.txt` & `wagtail_formation-0.1.5/wagtail_formation.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 formation/templates/formation/reusable_form.html
 formation/templates/formation/blocks/base_field.html
 formation/templates/formation/blocks/base_form.html
 formation/templates/formation/blocks/boolean_field.html
 formation/templates/formation/blocks/date_field.html
 formation/templates/formation/blocks/datetime_field.html
 formation/templates/formation/blocks/email_field.html
+formation/templates/formation/blocks/file_field.html
 formation/templates/formation/blocks/integer_field.html
 formation/templates/formation/blocks/radio_field.html
 formation/templates/formation/blocks/select_field.html
 formation/templates/formation/blocks/submit_button.html
 formation/templates/formation/blocks/text_field.html
 formation/templates/formation/blocks/textarea_field.html
 formation/templatetags/__init__.py
```

