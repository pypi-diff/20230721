# Comparing `tmp/leanit-mweb-23.7.3.tar.gz` & `tmp/leanit-mweb-23.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leanit-mweb-23.7.3.tar", last modified: Mon Jul 10 12:26:12 2023, max compression
+gzip compressed data, was "leanit-mweb-23.7.4.tar", last modified: Fri Jul 21 14:00:03 2023, max compression
```

## Comparing `leanit-mweb-23.7.3.tar` & `leanit-mweb-23.7.4.tar`

### file list

```diff
@@ -1,94 +1,104 @@
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-10 12:26:12.015071 leanit-mweb-23.7.3/
--rw-rw-r--   0 martin    (1000) martin    (1000)      962 2023-05-08 15:13:45.000000 leanit-mweb-23.7.3/LICENSE
--rw-rw-r--   0 martin    (1000) martin    (1000)     2430 2023-07-10 12:26:12.015071 leanit-mweb-23.7.3/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)     1921 2023-06-21 11:11:08.000000 leanit-mweb-23.7.3/README.md
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-10 12:26:11.995072 leanit-mweb-23.7.3/leanit_mweb.egg-info/
--rw-rw-r--   0 martin    (1000) martin    (1000)     2430 2023-07-10 12:26:11.000000 leanit-mweb-23.7.3/leanit_mweb.egg-info/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)     1676 2023-07-10 12:26:11.000000 leanit-mweb-23.7.3/leanit_mweb.egg-info/SOURCES.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-07-10 12:26:11.000000 leanit-mweb-23.7.3/leanit_mweb.egg-info/dependency_links.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)      549 2023-07-10 12:26:11.000000 leanit-mweb-23.7.3/leanit_mweb.egg-info/requires.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       11 2023-07-10 12:26:11.000000 leanit-mweb-23.7.3/leanit_mweb.egg-info/top_level.txt
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-10 12:26:11.999072 leanit-mweb-23.7.3/mweb/
--rw-rw-r--   0 martin    (1000) martin    (1000)    15058 2023-07-05 16:14:36.000000 leanit-mweb-23.7.3/mweb/__init__.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-10 12:26:11.999072 leanit-mweb-23.7.3/mweb/auth/
--rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-06-30 09:18:02.000000 leanit-mweb-23.7.3/mweb/auth/__init__.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-10 12:26:11.999072 leanit-mweb-23.7.3/mweb/auth/sso/
--rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-06-30 09:23:33.000000 leanit-mweb-23.7.3/mweb/auth/sso/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      381 2023-06-30 09:43:07.000000 leanit-mweb-23.7.3/mweb/auth/sso/base.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-10 12:26:11.999072 leanit-mweb-23.7.3/mweb/auth/sso/microsoft/
--rw-rw-r--   0 martin    (1000) martin    (1000)     7847 2023-07-05 14:34:14.000000 leanit-mweb-23.7.3/mweb/auth/sso/microsoft/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      449 2023-05-08 06:49:29.000000 leanit-mweb-23.7.3/mweb/form.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-10 12:26:11.999072 leanit-mweb-23.7.3/mweb/jinja_template/
--rw-rw-r--   0 martin    (1000) martin    (1000)     2671 2023-07-05 15:16:21.000000 leanit-mweb-23.7.3/mweb/jinja_template/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     4134 2023-05-01 18:09:47.000000 leanit-mweb-23.7.3/mweb/jinja_template/loaders.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1995 2023-06-30 11:57:20.000000 leanit-mweb-23.7.3/mweb/manage.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-10 12:26:11.999072 leanit-mweb-23.7.3/mweb/messaging/
--rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-05-19 13:00:21.000000 leanit-mweb-23.7.3/mweb/messaging/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-05-19 13:00:37.000000 leanit-mweb-23.7.3/mweb/messaging/base.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-10 12:26:12.003072 leanit-mweb-23.7.3/mweb/orm/
--rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-05-07 11:08:10.000000 leanit-mweb-23.7.3/mweb/orm/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      205 2023-05-07 11:45:37.000000 leanit-mweb-23.7.3/mweb/orm/exception.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-10 12:26:12.003072 leanit-mweb-23.7.3/mweb/orm/fields/
--rw-rw-r--   0 martin    (1000) martin    (1000)     2921 2023-07-07 08:58:44.000000 leanit-mweb-23.7.3/mweb/orm/fields/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      402 2023-06-30 11:55:37.000000 leanit-mweb-23.7.3/mweb/orm/fields/snowflake.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    17596 2023-07-07 08:55:19.000000 leanit-mweb-23.7.3/mweb/orm/model.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      914 2023-05-07 12:15:52.000000 leanit-mweb-23.7.3/mweb/orm/password.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-10 12:26:12.003072 leanit-mweb-23.7.3/mweb/security/
--rw-rw-r--   0 martin    (1000) martin    (1000)      564 2023-06-27 15:25:35.000000 leanit-mweb-23.7.3/mweb/security/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2135 2023-06-30 09:59:15.000000 leanit-mweb-23.7.3/mweb/security/jwt.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1060 2023-05-01 12:48:02.000000 leanit-mweb-23.7.3/mweb/staticfiles.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     3372 2023-07-07 08:33:20.000000 leanit-mweb-23.7.3/mweb/testutils.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2241 2023-06-06 11:14:00.000000 leanit-mweb-23.7.3/mweb/thread.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-10 12:26:12.003072 leanit-mweb-23.7.3/mweb/utils/
--rw-rw-r--   0 martin    (1000) martin    (1000)     2910 2023-07-07 09:14:22.000000 leanit-mweb-23.7.3/mweb/utils/__init__.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-10 12:26:12.007072 leanit-mweb-23.7.3/mweb/utils/id/
--rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-06-30 09:02:22.000000 leanit-mweb-23.7.3/mweb/utils/id/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1345 2023-06-30 09:04:34.000000 leanit-mweb-23.7.3/mweb/utils/id/snowflakeid.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      663 2023-07-07 09:14:55.000000 leanit-mweb-23.7.3/mweb/utils/log.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      931 2023-07-05 09:13:08.000000 leanit-mweb-23.7.3/mweb/utils/log_catcher.py
--rw-rw-r--   0 martin    (1000) martin    (1000)       19 2023-07-10 12:26:11.000000 leanit-mweb-23.7.3/mweb/version.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-10 12:26:12.007072 leanit-mweb-23.7.3/mweb/views/
--rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-05-17 08:14:19.000000 leanit-mweb-23.7.3/mweb/views/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1092 2023-06-30 11:57:20.000000 leanit-mweb-23.7.3/mweb/views/auth.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     6900 2023-07-05 10:05:44.000000 leanit-mweb-23.7.3/mweb/views/model.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    10602 2023-07-05 10:55:32.000000 leanit-mweb-23.7.3/mweb/yuga.py
--rw-rw-r--   0 martin    (1000) martin    (1000)       38 2023-07-10 12:26:12.015071 leanit-mweb-23.7.3/setup.cfg
--rw-rw-r--   0 martin    (1000) martin    (1000)     1912 2023-07-10 12:26:11.000000 leanit-mweb-23.7.3/setup.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-10 12:26:12.007072 leanit-mweb-23.7.3/tests/
--rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-06-30 12:07:34.000000 leanit-mweb-23.7.3/tests/__init__.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-10 12:26:12.007072 leanit-mweb-23.7.3/tests/auth/
--rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-06-30 09:29:21.000000 leanit-mweb-23.7.3/tests/auth/__init__.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-10 12:26:12.007072 leanit-mweb-23.7.3/tests/auth/sso/
--rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-06-30 09:29:21.000000 leanit-mweb-23.7.3/tests/auth/sso/__init__.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-10 12:26:12.011072 leanit-mweb-23.7.3/tests/auth/sso/microsoft/
--rw-rw-r--   0 martin    (1000) martin    (1000)      210 2023-06-30 09:30:02.000000 leanit-mweb-23.7.3/tests/auth/sso/microsoft/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1824 2023-06-30 09:36:45.000000 leanit-mweb-23.7.3/tests/auth/sso/microsoft/test_auth_callback.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1797 2023-06-30 09:36:45.000000 leanit-mweb-23.7.3/tests/auth/sso/microsoft/test_build_auth_url.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      591 2023-06-30 09:30:07.000000 leanit-mweb-23.7.3/tests/auth/sso/microsoft/test_code.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-10 12:26:12.011072 leanit-mweb-23.7.3/tests/orm/
--rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-06-14 06:24:31.000000 leanit-mweb-23.7.3/tests/orm/__init__.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-10 12:26:12.011072 leanit-mweb-23.7.3/tests/orm/fields/
--rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-06-14 07:10:28.000000 leanit-mweb-23.7.3/tests/orm/fields/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      873 2023-07-07 08:53:27.000000 leanit-mweb-23.7.3/tests/orm/fields/test_StringField.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-10 12:26:12.011072 leanit-mweb-23.7.3/tests/orm/model/
--rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-06-14 06:24:39.000000 leanit-mweb-23.7.3/tests/orm/model/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1158 2023-06-30 12:03:34.000000 leanit-mweb-23.7.3/tests/orm/model/test_delete_all.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-10 12:26:12.011072 leanit-mweb-23.7.3/tests/resources/
--rw-rw-r--   0 martin    (1000) martin    (1000)       76 2023-07-02 16:02:44.000000 leanit-mweb-23.7.3/tests/resources/__init__.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-10 12:26:12.011072 leanit-mweb-23.7.3/tests/security/
--rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-06-28 15:18:34.000000 leanit-mweb-23.7.3/tests/security/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1110 2023-06-29 11:38:56.000000 leanit-mweb-23.7.3/tests/security/test_jwt.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      685 2023-06-29 11:18:38.000000 leanit-mweb-23.7.3/tests/security/test_sign.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-10 12:26:12.015071 leanit-mweb-23.7.3/tests/utils/
--rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-06-29 11:22:08.000000 leanit-mweb-23.7.3/tests/utils/__init__.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-10 12:26:12.015071 leanit-mweb-23.7.3/tests/utils/log/
--rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-07-07 09:15:39.000000 leanit-mweb-23.7.3/tests/utils/log/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      402 2023-07-07 09:16:21.000000 leanit-mweb-23.7.3/tests/utils/log/test_hide_secrets.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1836 2023-06-30 11:57:20.000000 leanit-mweb-23.7.3/tests/utils/test_form.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      537 2023-06-30 09:05:14.000000 leanit-mweb-23.7.3/tests/utils/test_snowflake.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      469 2023-07-01 08:58:49.000000 leanit-mweb-23.7.3/tests/utils/test_unflatten.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-10 12:26:12.015071 leanit-mweb-23.7.3/tests/views/
--rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-07-02 15:26:48.000000 leanit-mweb-23.7.3/tests/views/__init__.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-10 12:26:12.015071 leanit-mweb-23.7.3/tests/views/model/
--rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-07-02 15:26:56.000000 leanit-mweb-23.7.3/tests/views/model/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     9069 2023-07-03 08:51:42.000000 leanit-mweb-23.7.3/tests/views/model/test_paging.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-21 14:00:03.666194 leanit-mweb-23.7.4/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      962 2023-05-08 15:13:45.000000 leanit-mweb-23.7.4/LICENSE
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2472 2023-07-21 14:00:03.666194 leanit-mweb-23.7.4/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1921 2023-06-21 11:11:08.000000 leanit-mweb-23.7.4/README.md
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-21 14:00:03.658194 leanit-mweb-23.7.4/leanit_mweb.egg-info/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2472 2023-07-21 14:00:03.000000 leanit-mweb-23.7.4/leanit_mweb.egg-info/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1866 2023-07-21 14:00:03.000000 leanit-mweb-23.7.4/leanit_mweb.egg-info/SOURCES.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-07-21 14:00:03.000000 leanit-mweb-23.7.4/leanit_mweb.egg-info/dependency_links.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)      579 2023-07-21 14:00:03.000000 leanit-mweb-23.7.4/leanit_mweb.egg-info/requires.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       11 2023-07-21 14:00:03.000000 leanit-mweb-23.7.4/leanit_mweb.egg-info/top_level.txt
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-21 14:00:03.662194 leanit-mweb-23.7.4/mweb/
+-rw-rw-r--   0 martin    (1000) martin    (1000)    18334 2023-07-21 09:36:09.000000 leanit-mweb-23.7.4/mweb/__init__.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-21 14:00:03.662194 leanit-mweb-23.7.4/mweb/auth/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-06-30 09:18:02.000000 leanit-mweb-23.7.4/mweb/auth/__init__.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-21 14:00:03.662194 leanit-mweb-23.7.4/mweb/auth/sso/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-06-30 09:23:33.000000 leanit-mweb-23.7.4/mweb/auth/sso/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      381 2023-06-30 09:43:07.000000 leanit-mweb-23.7.4/mweb/auth/sso/base.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-21 14:00:03.662194 leanit-mweb-23.7.4/mweb/auth/sso/microsoft/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     7847 2023-07-05 14:34:14.000000 leanit-mweb-23.7.4/mweb/auth/sso/microsoft/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      449 2023-05-08 06:49:29.000000 leanit-mweb-23.7.4/mweb/form.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-21 14:00:03.662194 leanit-mweb-23.7.4/mweb/jinja_template/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2671 2023-07-05 15:16:21.000000 leanit-mweb-23.7.4/mweb/jinja_template/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4134 2023-05-01 18:09:47.000000 leanit-mweb-23.7.4/mweb/jinja_template/loaders.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1995 2023-06-30 11:57:20.000000 leanit-mweb-23.7.4/mweb/manage.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-21 14:00:03.662194 leanit-mweb-23.7.4/mweb/messaging/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-05-19 13:00:21.000000 leanit-mweb-23.7.4/mweb/messaging/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-05-19 13:00:37.000000 leanit-mweb-23.7.4/mweb/messaging/base.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-21 14:00:03.662194 leanit-mweb-23.7.4/mweb/orm/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-05-07 11:08:10.000000 leanit-mweb-23.7.4/mweb/orm/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      205 2023-05-07 11:45:37.000000 leanit-mweb-23.7.4/mweb/orm/exception.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-21 14:00:03.662194 leanit-mweb-23.7.4/mweb/orm/fields/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3050 2023-07-12 12:02:57.000000 leanit-mweb-23.7.4/mweb/orm/fields/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      406 2023-07-21 09:36:09.000000 leanit-mweb-23.7.4/mweb/orm/fields/snowflake.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    20581 2023-07-13 12:27:46.000000 leanit-mweb-23.7.4/mweb/orm/model.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      914 2023-05-07 12:15:52.000000 leanit-mweb-23.7.4/mweb/orm/password.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-21 14:00:03.662194 leanit-mweb-23.7.4/mweb/security/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      564 2023-06-27 15:25:35.000000 leanit-mweb-23.7.4/mweb/security/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2148 2023-07-21 13:56:27.000000 leanit-mweb-23.7.4/mweb/security/jwt.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-21 14:00:03.662194 leanit-mweb-23.7.4/mweb/state/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-07-13 14:27:30.000000 leanit-mweb-23.7.4/mweb/state/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4649 2023-07-21 13:59:54.000000 leanit-mweb-23.7.4/mweb/state/client.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1060 2023-05-01 12:48:02.000000 leanit-mweb-23.7.4/mweb/staticfiles.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3515 2023-07-13 09:23:02.000000 leanit-mweb-23.7.4/mweb/testutils.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2241 2023-06-06 11:14:00.000000 leanit-mweb-23.7.4/mweb/thread.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-21 14:00:03.662194 leanit-mweb-23.7.4/mweb/utils/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3594 2023-07-11 12:34:48.000000 leanit-mweb-23.7.4/mweb/utils/__init__.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-21 14:00:03.662194 leanit-mweb-23.7.4/mweb/utils/id/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-06-30 09:02:22.000000 leanit-mweb-23.7.4/mweb/utils/id/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1437 2023-07-21 09:36:09.000000 leanit-mweb-23.7.4/mweb/utils/id/snowflakeid.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      663 2023-07-07 09:14:55.000000 leanit-mweb-23.7.4/mweb/utils/log.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      931 2023-07-05 09:13:08.000000 leanit-mweb-23.7.4/mweb/utils/log_catcher.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)       19 2023-07-21 14:00:03.000000 leanit-mweb-23.7.4/mweb/version.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-21 14:00:03.662194 leanit-mweb-23.7.4/mweb/views/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-05-17 08:14:19.000000 leanit-mweb-23.7.4/mweb/views/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1092 2023-06-30 11:57:20.000000 leanit-mweb-23.7.4/mweb/views/auth.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      347 2023-07-13 15:19:02.000000 leanit-mweb-23.7.4/mweb/views/dependencies.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     8907 2023-07-12 12:23:38.000000 leanit-mweb-23.7.4/mweb/views/model.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    10722 2023-07-21 09:36:09.000000 leanit-mweb-23.7.4/mweb/yuga.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)       38 2023-07-21 14:00:03.666194 leanit-mweb-23.7.4/setup.cfg
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2014 2023-07-21 14:00:03.000000 leanit-mweb-23.7.4/setup.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-21 14:00:03.662194 leanit-mweb-23.7.4/tests/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-06-30 12:07:34.000000 leanit-mweb-23.7.4/tests/__init__.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-21 14:00:03.662194 leanit-mweb-23.7.4/tests/auth/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-06-30 09:29:21.000000 leanit-mweb-23.7.4/tests/auth/__init__.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-21 14:00:03.662194 leanit-mweb-23.7.4/tests/auth/sso/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-06-30 09:29:21.000000 leanit-mweb-23.7.4/tests/auth/sso/__init__.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-21 14:00:03.666194 leanit-mweb-23.7.4/tests/auth/sso/microsoft/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      210 2023-06-30 09:30:02.000000 leanit-mweb-23.7.4/tests/auth/sso/microsoft/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1824 2023-06-30 09:36:45.000000 leanit-mweb-23.7.4/tests/auth/sso/microsoft/test_auth_callback.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1797 2023-06-30 09:36:45.000000 leanit-mweb-23.7.4/tests/auth/sso/microsoft/test_build_auth_url.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      591 2023-06-30 09:30:07.000000 leanit-mweb-23.7.4/tests/auth/sso/microsoft/test_code.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-21 14:00:03.666194 leanit-mweb-23.7.4/tests/orm/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-06-14 06:24:31.000000 leanit-mweb-23.7.4/tests/orm/__init__.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-21 14:00:03.666194 leanit-mweb-23.7.4/tests/orm/fields/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-06-14 07:10:28.000000 leanit-mweb-23.7.4/tests/orm/fields/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      873 2023-07-07 08:53:27.000000 leanit-mweb-23.7.4/tests/orm/fields/test_StringField.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-21 14:00:03.666194 leanit-mweb-23.7.4/tests/orm/model/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-06-14 06:24:39.000000 leanit-mweb-23.7.4/tests/orm/model/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1158 2023-06-30 12:03:34.000000 leanit-mweb-23.7.4/tests/orm/model/test_delete_all.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1709 2023-07-13 09:42:33.000000 leanit-mweb-23.7.4/tests/orm/model/test_update.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-21 14:00:03.666194 leanit-mweb-23.7.4/tests/resources/
+-rw-rw-r--   0 martin    (1000) martin    (1000)       76 2023-07-02 16:02:44.000000 leanit-mweb-23.7.4/tests/resources/__init__.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-21 14:00:03.666194 leanit-mweb-23.7.4/tests/security/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-06-28 15:18:34.000000 leanit-mweb-23.7.4/tests/security/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1110 2023-06-29 11:38:56.000000 leanit-mweb-23.7.4/tests/security/test_jwt.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      685 2023-06-29 11:18:38.000000 leanit-mweb-23.7.4/tests/security/test_sign.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-21 14:00:03.666194 leanit-mweb-23.7.4/tests/state/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-07-13 14:32:33.000000 leanit-mweb-23.7.4/tests/state/__init__.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-21 14:00:03.666194 leanit-mweb-23.7.4/tests/state/client/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-07-13 14:32:39.000000 leanit-mweb-23.7.4/tests/state/client/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1584 2023-07-14 08:53:14.000000 leanit-mweb-23.7.4/tests/state/client/test_state.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-21 14:00:03.666194 leanit-mweb-23.7.4/tests/utils/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-06-29 11:22:08.000000 leanit-mweb-23.7.4/tests/utils/__init__.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-21 14:00:03.666194 leanit-mweb-23.7.4/tests/utils/log/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-07-07 09:15:39.000000 leanit-mweb-23.7.4/tests/utils/log/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      402 2023-07-11 07:42:20.000000 leanit-mweb-23.7.4/tests/utils/log/test_hide_secrets.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1836 2023-06-30 11:57:20.000000 leanit-mweb-23.7.4/tests/utils/test_form.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      537 2023-06-30 09:05:14.000000 leanit-mweb-23.7.4/tests/utils/test_snowflake.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      469 2023-07-01 08:58:49.000000 leanit-mweb-23.7.4/tests/utils/test_unflatten.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-21 14:00:03.666194 leanit-mweb-23.7.4/tests/views/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-07-02 15:26:48.000000 leanit-mweb-23.7.4/tests/views/__init__.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-21 14:00:03.666194 leanit-mweb-23.7.4/tests/views/model/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-07-02 15:26:56.000000 leanit-mweb-23.7.4/tests/views/model/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     9069 2023-07-03 08:51:42.000000 leanit-mweb-23.7.4/tests/views/model/test_paging.py
```

### Comparing `leanit-mweb-23.7.3/LICENSE` & `leanit-mweb-23.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.7.3/PKG-INFO` & `leanit-mweb-23.7.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: leanit-mweb
-Version: 23.7.3
+Version: 23.7.4
 Summary: Web framework
 Author: Martin Klapproth
 Author-email: martin.klapproth@staxnet.de
 Keywords: python,web
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
+Provides-Extra: psql
+Provides-Extra: ysql
 License-File: LICENSE
 
 
 Lean IT Mweb Framework
 
 write a python function which gets a html input. The function should return a Form objects. The Form objects represents data parsed from the html <form> tag. The following code should work:
```

### Comparing `leanit-mweb-23.7.3/README.md` & `leanit-mweb-23.7.4/README.md`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.7.3/leanit_mweb.egg-info/PKG-INFO` & `leanit-mweb-23.7.4/leanit_mweb.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: leanit-mweb
-Version: 23.7.3
+Version: 23.7.4
 Summary: Web framework
 Author: Martin Klapproth
 Author-email: martin.klapproth@staxnet.de
 Keywords: python,web
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
+Provides-Extra: psql
+Provides-Extra: ysql
 License-File: LICENSE
 
 
 Lean IT Mweb Framework
 
 write a python function which gets a html input. The function should return a Form objects. The Form objects represents data parsed from the html <form> tag. The following code should work:
```

### Comparing `leanit-mweb-23.7.3/leanit_mweb.egg-info/SOURCES.txt` & `leanit-mweb-23.7.4/leanit_mweb.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -26,38 +26,45 @@
 mweb/orm/exception.py
 mweb/orm/model.py
 mweb/orm/password.py
 mweb/orm/fields/__init__.py
 mweb/orm/fields/snowflake.py
 mweb/security/__init__.py
 mweb/security/jwt.py
+mweb/state/__init__.py
+mweb/state/client.py
 mweb/utils/__init__.py
 mweb/utils/log.py
 mweb/utils/log_catcher.py
 mweb/utils/id/__init__.py
 mweb/utils/id/snowflakeid.py
 mweb/views/__init__.py
 mweb/views/auth.py
+mweb/views/dependencies.py
 mweb/views/model.py
 tests/__init__.py
 tests/auth/__init__.py
 tests/auth/sso/__init__.py
 tests/auth/sso/microsoft/__init__.py
 tests/auth/sso/microsoft/test_auth_callback.py
 tests/auth/sso/microsoft/test_build_auth_url.py
 tests/auth/sso/microsoft/test_code.py
 tests/orm/__init__.py
 tests/orm/fields/__init__.py
 tests/orm/fields/test_StringField.py
 tests/orm/model/__init__.py
 tests/orm/model/test_delete_all.py
+tests/orm/model/test_update.py
 tests/resources/__init__.py
 tests/security/__init__.py
 tests/security/test_jwt.py
 tests/security/test_sign.py
+tests/state/__init__.py
+tests/state/client/__init__.py
+tests/state/client/test_state.py
 tests/utils/__init__.py
 tests/utils/test_form.py
 tests/utils/test_snowflake.py
 tests/utils/test_unflatten.py
 tests/utils/log/__init__.py
 tests/utils/log/test_hide_secrets.py
 tests/views/__init__.py
```

### Comparing `leanit-mweb-23.7.3/leanit_mweb.egg-info/requires.txt` & `leanit-mweb-23.7.4/leanit_mweb.egg-info/requires.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 fastapi~=0.95
 uvicorn~=0.22
-uvloop~=0.17
 jinja2~=3.1
 python-multipart~=0.0
 wtforms~=3.0
 email_validator~=2.0
 multidict~=6.0
-psycopg2-yugabytedb~=2.9
 PyYAML~=6.0
 python-ulid~=1.1
 snowflake-id~=0.0
 aiohttp~=3.7
 aioresponses~=0.7
 bcrypt~=4.0
 passlib~=1.7
@@ -20,7 +18,14 @@
 opentelemetry-instrumentation-aiohttp-client~=0.39b0
 opentelemetry-instrumentation-fastapi~=0.39b0
 opentelemetry-instrumentation-logging~=0.39b0
 opentelemetry-exporter-otlp~=1.18
 sentry-sdk[fastapi]~=1.25
 pytest
 httpx
+uvloop~=0.17
+
+[psql]
+psycopg2~=2.9
+
+[ysql]
+psycopg2-yugabytedb~=2.9
```

### Comparing `leanit-mweb-23.7.3/mweb/__init__.py` & `leanit-mweb-23.7.4/mweb/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 from __future__ import annotations
 import logging
+from inspect import isclass
 from pprint import pprint
 
+from fastapi.types import DecoratedCallable
+from starlette.requests import Request
+
 from mweb.version import VERSION
 
 logger = logging.getLogger(__name__)
 
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Callable, Optional, Sequence
 
 if TYPE_CHECKING:
     pass
 
 import base64
 import importlib
 import logging
 import os
 import pkgutil
 import sys
 from collections import defaultdict
 from os.path import isdir
 
 import yaml
-from fastapi import FastAPI
+from fastapi import FastAPI, Depends
 
 from mweb.jinja_template import Jinja2Templates
 from mweb.jinja_template.loaders import FileSystemLoader
 from mweb.utils import merge_dict
 from mweb.yuga import YugabytedbThreadPool
 
 logger = logging.getLogger(__name__)
@@ -48,27 +52,27 @@
 oauth2_scheme = None
 auth_user_model = None
 
 app = None
 
 class App(FastAPI):
 
-    def __init__(self, app_root: str):
+    def __init__(self, app_root: str, **kwargs):
         logger.info(f"Initializing mweb app version={VERSION}")
 
         global config, app
         app = self
 
         self.app_root = app_root
         self.db: YugabytedbThreadPool = None
 
         config = self.config = self._read_config()
         self.secret_key = config.get("mweb", {}).get("secret_key", None)
 
-        super().__init__()
+        super().__init__(**kwargs)
 
         # static files
         static_dir = f"{app_root}/static"
         if isdir(static_dir):
             # mount static files
             from mweb.staticfiles import StaticFiles
             self.mount("/static", StaticFiles(directory=static_dir), name="static")
@@ -116,15 +120,19 @@
 
         # loader
         module_name = self.__module__ # "mium_frontend"
         models_module_name = f"{module_name}.model"
         models_module = None
         try:
             models_module = importlib.import_module(models_module_name)
-        except ImportError:
+        except ImportError as e:
+            error_message = str(e)
+            raise e
+            if "partially initialized" in error_message:
+                raise e
             logger.debug(f"no models package found for {module_name} ({models_module_name})")
         if models_module:
             for importer, modname, ispkg in pkgutil.walk_packages(path=models_module.__path__, prefix=models_module.__name__+'.'):
                 module = importlib.import_module(modname)
 
         # initialize all models
         for cls in Model.__subclasses__():  # type: Model
@@ -397,13 +405,85 @@
         # validate views
         from mweb.views.model import ModelView
         model_views = ModelView.__subclasses__()
 
         for model_view_class in model_views:
             self._validate_model_view(model_view_class)
 
+    def register(
+        self,
+        path: str,
+        *,
+        name: Optional[str] = None,
+        dependencies: Optional[Sequence[Depends]] = None,
+    ) -> Callable[[DecoratedCallable], DecoratedCallable]:
+
+        from mweb.views.model import ModelView
+
+        def decorator(func: DecoratedCallable) -> DecoratedCallable:
+            if isclass(func):
+                if issubclass(func, ModelView):
+                    model_view: ModelView = func
+
+                    view_list_func = getattr(func, "view_list")
+                    view_detail_func = getattr(func, "view_detail")
+
+                    route_name = f"{name}_list"
+                    self.add_api_route(
+                        path,
+                        view_list_func,
+                        summary=f"{func.__name__}.view_list name={route_name}",
+                        name=route_name,
+                        dependencies=dependencies,
+                    )
+
+                    route_name = f"{name}_detail"
+                    self.add_api_route(
+                        model_view._build_url(path),
+                        view_detail_func,
+                        summary=f"{func.__name__}.view_detail name={route_name}",
+                        name=f"{name}_detail",
+                        dependencies=dependencies,
+                    )
+
+                    # find action methods
+                    for key, value in model_view.__dict__.items():
+                        if key.startswith("on_action_"):
+                            action_name = key[10:].replace("_", "-")
+                            callable = getattr(model_view, key)
+
+                            methods = ["GET"]
+                            if hasattr(callable, "methods"):
+                                methods = callable.methods
+
+                            logger.debug(f"registering action {action_name} for {model_view} ({callable}) with methods {methods}")
+
+                            async def wrap(request: Request, callable=callable):
+                                view = model_view(request)
+                                logger.debug(f"calling {callable} on {view}")
+                                return await callable(view)
+
+                            route_name = f"{name}_{action_name}"
+                            self.add_api_route(
+                                model_view._build_url(path) + "/" + action_name,
+                                wrap,
+                                summary=f"{func.__name__}.{key} name={route_name}",
+                                name=route_name,
+                                methods=methods,
+                                dependencies=dependencies,
+                            )
+                else:
+                    raise NotImplementedError(f"registering of {func} not implemented")
+            else:
+                raise NotImplementedError(f"{func} must be a class")
+
+
+            return func
+
+        return decorator
+
     def _validate_model_view(self, model_view_class):
         # check if every primary key property is in the list of fields
         if model_view_class.list_fields:
             for pk_field_name in model_view_class.model._pk:
                 if pk_field_name not in model_view_class.list_fields:
                     raise ValueError(f"primary key field {pk_field_name} of model {model_view_class.model.__name__} is not in list_fields of {model_view_class.__name__} defined in {model_view_class.__module__}")
```

### Comparing `leanit-mweb-23.7.3/mweb/auth/sso/microsoft/__init__.py` & `leanit-mweb-23.7.4/mweb/auth/sso/microsoft/__init__.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.7.3/mweb/jinja_template/__init__.py` & `leanit-mweb-23.7.4/mweb/jinja_template/__init__.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.7.3/mweb/jinja_template/loaders.py` & `leanit-mweb-23.7.4/mweb/jinja_template/loaders.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.7.3/mweb/manage.py` & `leanit-mweb-23.7.4/mweb/manage.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.7.3/mweb/orm/fields/__init__.py` & `leanit-mweb-23.7.4/mweb/orm/fields/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,22 +60,27 @@
         super().__init__(default=default)
         self.min_length = min_length
         self.max_length = max_length
         self.alphabet = alphabet
         self.choices = choices
 
     def validate(self, value):
-        if self.min_length is not None and len(value) < self.min_length:
-            raise ValidationFailedException(f"String is too short: '{value}' (min: {self.min_length})")
-        if self.max_length is not None and len(value) > self.max_length:
-            raise ValidationFailedException(f"String is too long: '{value}' (max: {self.max_length})")
-        if self.alphabet is not None and not set(value).issubset(set(self.alphabet)):
-            raise ValidationFailedException(f"String contains invalid characters: '{value}' (alphabet: {self.alphabet})")
-        if self.choices is not None and value not in self.choices:
-            raise ValidationFailedException(f"String '{value}' of field is not in choices: {','.join(self.choices)}")
+        if value:
+            if self.min_length is not None and len(value) < self.min_length:
+                raise ValidationFailedException(f"String is too short: '{value}' (min: {self.min_length})")
+            if self.max_length is not None and len(value) > self.max_length:
+                raise ValidationFailedException(f"String is too long: '{value}' (max: {self.max_length})")
+            if self.alphabet is not None and not set(value).issubset(set(self.alphabet)):
+                raise ValidationFailedException(f"String contains invalid characters: '{value}' (alphabet: {self.alphabet})")
+            if self.choices is not None and value not in self.choices:
+                raise ValidationFailedException(f"String '{value}' of field is not in choices: {','.join(self.choices)}")
+        else:
+            # TODO: check if field is nullable
+            pass
+
         return super().validate(value)
 
 
 class EmailField(StringField):
     pattern = re.compile(r'^[\w\.-]+@[\w\.-]+\.\w+$')
 
     def validate(self, value):
```

### Comparing `leanit-mweb-23.7.3/mweb/orm/model.py` & `leanit-mweb-23.7.4/mweb/orm/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -244,14 +244,42 @@
             create_doc.update(defaults)
 
             new_object = cls.create(**create_doc)
             # new_object.save()
             return new_object
 
     @classmethod
+    async def get_or_create_async(cls: T, query: Dict[str, any], defaults: Dict[str, any]) -> T:
+        """
+        This method takes two dictionaries as arguments. The first one is used to query the database,
+        and the second one is used to create the object if it does not exist.
+
+        :param query: A dictionary containing the query parameters.
+        :param defaults: A dictionary containing the default values for creating a new object.
+        :return: An instance of the Model.
+
+        Example usage:
+
+        author = Author.get_or_create(
+            query={"tenant_id": 1, "id": 1},
+            defaults={"name": "John Doe", "email": "john.doe@example.com"}
+        )
+        """
+        results = await cls.filter_async(**query)
+        if results:
+            return results[0]
+        else:
+            create_doc = query.copy()
+            create_doc.update(defaults)
+
+            new_object = await cls.create_async(**create_doc)
+            # new_object.save()
+            return new_object
+
+    @classmethod
     def filter(cls, _only=None, **kwargs):
         field_names = [*cls.fields.keys()]
 
         sql, values = cls._get_select_query_and_values(_only=field_names, **kwargs)
         # logger.debug(f"SQL: {sql}")
 
         result = []
@@ -412,35 +440,63 @@
         """
         Async wrapper for save
         :return:
         """
         tracing_context = context.get_current()
         await asyncio.get_event_loop().run_in_executor(self._db, self.save, tracing_context)
 
-    def _get_update_query_and_values(self, update_doc: Dict):
+    @classmethod
+    def _build_update_query_and_values(cls, query_doc: Dict, update_doc: Dict):
         set_values = []
         set_args = []
         for key, value in update_doc.items():
             set_values.append(f"{key}=%s")
-            field = self.fields[key]
+            field = cls.fields[key]
             field.validate(value)
             set_args.append(field.to_db(value))
         set_values = ",".join(set_values)
 
         where_values = []
         where_args = []
-        for key in self._pk:
+        for key, value in query_doc.items():
             where_values.append(f"{key}=%s")
-            where_args.append(getattr(self, key))
+            where_args.append(value)
         where_values = " AND ".join(where_values)
 
-        query = f"UPDATE \"{self._table}\" SET {set_values} WHERE {where_values}"
+        query = f"UPDATE \"{cls._table}\" SET {set_values} WHERE {where_values}"
         args = set_args + where_args
         return [query, args]
 
+    def _get_update_query_and_values(self, update_doc: Dict):
+        query_doc = {}
+        for key in self._pk:
+            query_doc[key] = getattr(self, key)
+
+        return self._build_update_query_and_values(query_doc, update_doc)
+        #
+        # set_values = []
+        # set_args = []
+        # for key, value in update_doc.items():
+        #     set_values.append(f"{key}=%s")
+        #     field = self.fields[key]
+        #     field.validate(value)
+        #     set_args.append(field.to_db(value))
+        # set_values = ",".join(set_values)
+        #
+        # where_values = []
+        # where_args = []
+        # for key in self._pk:
+        #     where_values.append(f"{key}=%s")
+        #     where_args.append(getattr(self, key))
+        # where_values = " AND ".join(where_values)
+        #
+        # query = f"UPDATE \"{self._table}\" SET {set_values} WHERE {where_values}"
+        # args = set_args + where_args
+        # return [query, args]
+
     def on_pre_create(self):
         pass
 
     def on_post_create(self):
         pass
 
     def on_pre_update(self):
@@ -469,14 +525,17 @@
         where_clause = " AND ".join([f"{field_name} = %s" for field_name in self._pk])
         values = [getattr(self, field_name) for field_name in self._pk]
         if _limit:
             fields = _limit
         else:
             fields = self.fields.keys()
 
+        # ignore primary key fields as they could not have been changed
+        fields = [field_name for field_name in fields if field_name not in self._pk]
+
         select_fields = ",".join(fields)
 
         query = f"SELECT {select_fields} FROM \"{self._table}\" WHERE {where_clause} LIMIT 1"
 
         tracing_context = context.get_current()
         result = self._db.execute(query, values, tracing_context)
 
@@ -484,14 +543,32 @@
             raise RuntimeError(f"Record not found for {self._table} with {self._pk} = {values}")
 
         row = result[0]
         for i, field_name in enumerate(fields):
             setattr(self, field_name, row[i])
 
     @classmethod
+    async def update_async(cls, query: Dict[str, any], update: Dict[str, any]):
+        """
+        This method takes two dictionaries as arguments. The first one is used to query the database,
+        and the second one is used to update the object if it exists.
+
+        :param query: A dictionary containing the query parameters.
+        :param update: A dictionary containing the values to update.
+        :return: An instance of the Model or None if query did not change anything.
+        """
+        sql, values = cls._build_update_query_and_values(query, update)
+
+        tracing_context = context.get_current()
+        result = await asyncio.get_event_loop().run_in_executor(cls._db, cls._db.submit_sql, sql, values, tracing_context)
+
+        return result
+
+
+    @classmethod
     def upsert(cls: T, query: Dict[str, any], update: Dict[str, any]) -> Union[T, None]:
         """
         This method takes two dictionaries as arguments. The first one is used to query the database,
         and the second one is used to update the object if it exists.
 
         :param query: A dictionary containing the query parameters.
         :param update: A dictionary containing the values to update.
```

### Comparing `leanit-mweb-23.7.3/mweb/orm/password.py` & `leanit-mweb-23.7.4/mweb/orm/password.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.7.3/mweb/security/__init__.py` & `leanit-mweb-23.7.4/mweb/security/__init__.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.7.3/mweb/security/jwt.py` & `leanit-mweb-23.7.4/mweb/security/jwt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 import logging
 from calendar import timegm
 from datetime import timedelta, datetime
-from mweb import config
+
 from jose import jwt, JWTError
 from jose.jwk import construct
 
 logger = logging.getLogger(__name__)
 
 from typing import TYPE_CHECKING, Dict
 
@@ -32,14 +32,15 @@
         """
         Returns a singleton instance of TokenService. The JWT keys are read from the config file. They must
         be configured in the mweb.jwt section.
 
         :return: TokenService
         """
         if cls._instance is None:
+            from mweb import config
             jwt_config = config["mweb"]["jwt"]
 
             cls._instance = cls(public_key_pem=jwt_config["public_key"], private_key_pem=jwt_config["private_key"])
         return cls._instance
 
     def encode_jwt(self, data: Dict, expires_delta: timedelta | None = None) -> str:
         if expires_delta:
```

### Comparing `leanit-mweb-23.7.3/mweb/staticfiles.py` & `leanit-mweb-23.7.4/mweb/staticfiles.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.7.3/mweb/testutils.py` & `leanit-mweb-23.7.4/mweb/testutils.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
         self.action = action
         # always lowercase
         self.method = method
         self.data = data
 
     def fill(self, **kwargs):
         self.data.update(kwargs)
+        return self
 
     @classmethod
     def from_response(cls, response: Response, index=None, name=None, id=None):
         return cls.parse(response.text, index=index, name=name, id=id)
 
     @classmethod
     def parse(cls, html, index=None, name=None, id=None):
@@ -97,7 +98,9 @@
         self._fix_redirect_kwargs(kwargs)
         return super().get(*args, **kwargs)
 
     def post(self, *args, **kwargs):
         self._fix_redirect_kwargs(kwargs)
         return super().post(*args, **kwargs)
 
+    def follow_redirect(self, redirect_response: Response):
+        return self.get(redirect_response.headers["location"])
```

### Comparing `leanit-mweb-23.7.3/mweb/thread.py` & `leanit-mweb-23.7.4/mweb/thread.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.7.3/mweb/utils/__init__.py` & `leanit-mweb-23.7.4/mweb/utils/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import logging
 
 from starlette.requests import Request
 
 logger = logging.getLogger(__name__)
 
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Dict
 
 if TYPE_CHECKING:
     pass
 
 def camelCaseToSnakeCase(name):
     return ''.join(['_'+i.lower() if i.isupper() else i for i in name]).lstrip('_')
 
@@ -82,7 +82,25 @@
     :return: A tuple of pairs, where each pair contains two elements from the input list.
     :rtype: tuple
     """
     split_data = data.split(delimiter)
     result = tuple((split_data[i], split_data[i+1]) for i in range(0, len(split_data), 2))
     return result
 
+
+def unnest_query_params(input_dict: Dict[str, str]) -> Dict:
+    """
+    Convert a dictionary of query parameters with nested keys to a dictionary with a single level of keys.
+
+    :param input_dict: {'filter[tenant]': 'all', 'filter[foo]': 'bar'}
+    :return: {'filter': {'tenant': 'all', 'foo': 'bar'}}
+    """
+    output_dict = {}
+    for key, value in input_dict.items():
+        if '[' in key and ']' in key:
+            outer_key, inner_key = key.split('[')
+            inner_key = inner_key.rstrip(']')
+            if outer_key not in output_dict:
+                output_dict[outer_key] = {}
+            output_dict[outer_key][inner_key] = value
+    return output_dict
+
```

### Comparing `leanit-mweb-23.7.3/mweb/utils/id/snowflakeid.py` & `leanit-mweb-23.7.4/mweb/utils/id/snowflakeid.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from __future__ import annotations
 
 import hashlib
 import logging
 import os
+import uuid
+from time import perf_counter
 
 from snowflake import SnowflakeGenerator as UpSnowflakeGenerator, Snowflake
+from ulid import ULID
 
 logger = logging.getLogger(__name__)
 
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     pass
@@ -43,8 +46,9 @@
         super().__init__(instance=instance_id, epoch=self.start_epoch)
 
     def parse(self, sf: int) -> Snowflake:
         return Snowflake.parse(sf, epoch=self.start_epoch)
 
 if __name__ == '__main__':
     s = SnowflakeGenerator.get_instance()
-    print(s.next())
+    for i in range(10):
+        print(s.next())
```

### Comparing `leanit-mweb-23.7.3/mweb/utils/log.py` & `leanit-mweb-23.7.4/mweb/utils/log.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.7.3/mweb/utils/log_catcher.py` & `leanit-mweb-23.7.4/mweb/utils/log_catcher.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.7.3/mweb/views/auth.py` & `leanit-mweb-23.7.4/mweb/views/auth.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.7.3/mweb/views/model.py` & `leanit-mweb-23.7.4/mweb/views/model.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 import json
 import logging
 from pprint import pprint
 from urllib.parse import quote, urlencode
 
 from fastapi import HTTPException
 from starlette.requests import Request
-from starlette.responses import Response
+from starlette.responses import Response, RedirectResponse
 
 from mweb import templates
 from mweb.orm.model import Model
-from mweb.utils import flatten, unflatten
+from mweb.utils import flatten, unflatten, unnest_query_params
 
 logger = logging.getLogger(__name__)
 
 from typing import TYPE_CHECKING, List
 
 if TYPE_CHECKING:
     pass
@@ -23,14 +23,18 @@
 def _flip_order_by(order_by: str) -> str:
     """
     "tenant_id,id" -> "-tenant_id,-id"
     "-tenant_id,-id" -> "tenant_id,id"
     """
     return ",".join([f"-{field}" if not field.startswith("-") else field[1:] for field in order_by.split(",")])
 
+
+
+
+
 class ModelView:
     model: Model
     template_directory: str
     list_limit = 10
     list_fields = []
     list_order_by = "ASC"
 
@@ -40,14 +44,38 @@
         # merge query params and path params (path params take precedence)
         self.params = dict(self.request.query_params)
         self.params.update(dict(self.request.path_params))
 
         self.object = None
         self.object_list = None
 
+    @classmethod
+    def _build_url(cls, path: str) -> str:
+        """
+        This function takes in a path string and a model class as arguments. It first gets the _pk attribute of the model class, which is a list of primary keys. Then, for each primary key in the list, it checks if the key is already in the path string. If it’s not, it appends the key to the path string. Finally, it returns the updated path string with a leading forward slash.
+
+        class Post(Model):
+            _pk = ["tenant", "id"]
+
+        print(build_url("post", Post)) # returns /post/{tenant}/{id}
+        print(build_url("post/{tenant}", Post)) # returns /post/{tenant}/{id} because the tenant is already in the path
+
+        @param path:
+        @param model:
+        @return:
+        """
+        for key in cls.model._pk:
+            if f'{{{key}}}' not in path:
+                path += f'/{{{key}}}'
+
+        if not path.startswith("/"):
+            path = f"/{path}"
+
+        return path
+
     async def get_context(self, **kwargs):
         template_context = {
             "request": self.request,
         }
 
         template_context.update(kwargs)
 
@@ -70,14 +98,21 @@
     async def get_object_list(self) -> List[Model]:
         _only = None
         if self.list_fields:
             _only = self.list_fields
 
         filter = {}
 
+        filter_query_parameters = unnest_query_params(self.request.query_params).get("filter", {})
+        if filter_query_parameters:
+            for key, value in filter_query_parameters.items():
+                if value == "null" or value == "":
+                    continue
+                filter[key] = value
+
         order_by = ",".join(self.model._pk)
         if self.list_order_by == "DESC":
             order_by = _flip_order_by(order_by)
 
         page_direction = self.request.query_params.get('page-direction', "gt")
 
         order_flipped = False
@@ -122,14 +157,22 @@
 
     def get_edit_template(self):
         return f"{self.template_directory}/edit.html"
 
     def get_list_template(self):
         return f"{self.template_directory}/list.html"
 
+    def redirect(self, route_name: str, status_code: int = 303, **kwargs) -> RedirectResponse:
+        router = self.request.scope["router"]
+        path_params = dict(self.request.path_params)
+        path_params.update(kwargs)
+
+        url = router.url_path_for(route_name, **path_params)
+        return RedirectResponse(url, status_code=status_code)
+
     async def render_detail(self, **kwargs) -> Response:
         await self.get_object()
 
         template_context = await self.get_context(object=self.object, **kwargs)
 
         return templates.TemplateResponse(self.get_detail_template(), template_context)
 
@@ -182,7 +225,17 @@
 
             pagination["previous_url"] = self.request.url.path + "?" + urlencode(previous_url_params)
 
         template_context = await self.get_context(object_list=object_list, **kwargs)
         template_context["pagination"] = pagination
 
         return templates.TemplateResponse(self.get_list_template(), template_context)
+
+    @classmethod
+    async def view_list(cls, request: Request) -> Response:
+        instance = cls(request)
+        return await instance.render_list()
+
+    @classmethod
+    async def view_detail(cls, request: Request) -> Response:
+        instance = cls(request)
+        return await instance.render_detail()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `leanit-mweb-23.7.3/mweb/yuga.py` & `leanit-mweb-23.7.4/mweb/yuga.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,20 @@
 from time import time, perf_counter
 
 import asyncio
 import psycopg2
 from opentelemetry import trace, context
 from opentelemetry.semconv.trace import SpanAttributes
 from opentelemetry.trace import SpanKind
-from psycopg2 import connection, InterfaceError
+try:
+    from psycopg2 import connection
+except ImportError:
+    from psycopg2._psycopg import connection
+
+from psycopg2 import InterfaceError
 from psycopg2.extensions import ISOLATION_LEVEL_SERIALIZABLE, ISOLATION_LEVEL_REPEATABLE_READ
 from psycopg2.pool import ThreadedConnectionPool
 import psycopg2.errors
 
 import mweb
 import mweb
 from mweb.thread import AdvancedThreadPoolExecutor
@@ -146,15 +151,15 @@
         return f.result()
 
     async def execute_async(self, sql: str, vars: Union[Dict, Iterable]=None, tracing_context=None):
         if not tracing_context:
             tracing_context = context.get_current()
         return await asyncio.get_event_loop().run_in_executor(self, self.submit_sql, sql, vars, tracing_context)
 
-    def submit_sql(self, sql: str, vars: Union[Dict, Iterable]=None, tracing_context=None):
+    def submit_sql(self, sql: str, vars: Union[Dict, Iterable]=None, tracing_context=None) -> Union[None, Iterable]:
         """
         This function is executed in a thread. It is blocking.
 
         :param sql: might contain %s placeholders (vars=Iterable) or %(name)s placeholders (vars=Dict)
         :param vars: Iterable or Dict
         :return:
         """
```

### Comparing `leanit-mweb-23.7.3/setup.py` & `leanit-mweb-23.7.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,62 +1,74 @@
+import sys
+
 from setuptools import setup, find_packages
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '23.7.3'
+VERSION = '23.7.4'
 DESCRIPTION = 'Web framework'
 LONG_DESCRIPTION = 'Web framework'
 
+install_requires = [
+    'fastapi~=0.95',
+    'uvicorn~=0.22',
+    'jinja2~=3.1',
+    'python-multipart~=0.0',
+    'wtforms~=3.0',
+    'email_validator~=2.0',
+    'multidict~=6.0',
+    # 'psycopg2-yugabytedb~=2.9',
+    'PyYAML~=6.0',
+    'python-ulid~=1.1',
+    'snowflake-id~=0.0',
+    'aiohttp~=3.7',
+    'aioresponses~=0.7',
+    # for authentication / crypto
+    'bcrypt~=4.0',
+    'passlib~=1.7',
+    'python-jose[cryptography]~=3.3',  # JWT
+    # telemetry
+    'opentelemetry-api~=1.18',
+    'opentelemetry-sdk~=1.18',
+    'opentelemetry-instrumentation-aiohttp-client~=0.39b0',
+    'opentelemetry-instrumentation-fastapi~=0.39b0',
+    'opentelemetry-instrumentation-logging~=0.39b0',
+    'opentelemetry-exporter-otlp~=1.18',
+    # tracing
+    'sentry-sdk[fastapi]~=1.25',
+    # for testing
+    'pytest',
+    'httpx',
+]
+
+if sys.platform == 'linux':
+    install_requires += [
+        'uvloop~=0.17',
+    ]
+
 # Setting up
 setup(
     name="leanit-mweb",
     version=VERSION,
     author="Martin Klapproth",
     author_email="martin.klapproth@staxnet.de",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
-    install_requires=[
-        'fastapi~=0.95',
-        'uvicorn~=0.22',
-        'uvloop~=0.17',
-        'jinja2~=3.1',
-        'python-multipart~=0.0',
-        'wtforms~=3.0',
-        'email_validator~=2.0',
-        'multidict~=6.0',
-        'psycopg2-yugabytedb~=2.9',
-        'PyYAML~=6.0',
-        'python-ulid~=1.1',
-        'snowflake-id~=0.0',
-        'aiohttp~=3.7',
-        'aioresponses~=0.7',
-        # for authentication / crypto
-        'bcrypt~=4.0',
-        'passlib~=1.7',
-        'python-jose[cryptography]~=3.3', # JWT
-        # telemetry
-        'opentelemetry-api~=1.18',
-        'opentelemetry-sdk~=1.18',
-        'opentelemetry-instrumentation-aiohttp-client~=0.39b0',
-        'opentelemetry-instrumentation-fastapi~=0.39b0',
-        'opentelemetry-instrumentation-logging~=0.39b0',
-        'opentelemetry-exporter-otlp~=1.18',
-        # tracing
-        'sentry-sdk[fastapi]~=1.25',
-        # for testing
-        'pytest',
-        'httpx',
-    ],
+    install_requires=install_requires,
+    extras_require={
+        'psql': ['psycopg2~=2.9'],
+        'ysql': ['psycopg2-yugabytedb~=2.9'],
+    },
     keywords=['python', 'web'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

### Comparing `leanit-mweb-23.7.3/tests/auth/sso/microsoft/test_auth_callback.py` & `leanit-mweb-23.7.4/tests/auth/sso/microsoft/test_auth_callback.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.7.3/tests/auth/sso/microsoft/test_build_auth_url.py` & `leanit-mweb-23.7.4/tests/auth/sso/microsoft/test_build_auth_url.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.7.3/tests/auth/sso/microsoft/test_code.py` & `leanit-mweb-23.7.4/tests/auth/sso/microsoft/test_code.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.7.3/tests/orm/fields/test_StringField.py` & `leanit-mweb-23.7.4/tests/orm/fields/test_StringField.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.7.3/tests/orm/model/test_delete_all.py` & `leanit-mweb-23.7.4/tests/orm/model/test_delete_all.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.7.3/tests/security/test_jwt.py` & `leanit-mweb-23.7.4/tests/security/test_jwt.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.7.3/tests/security/test_sign.py` & `leanit-mweb-23.7.4/tests/security/test_sign.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.7.3/tests/utils/test_form.py` & `leanit-mweb-23.7.4/tests/utils/test_form.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.7.3/tests/utils/test_snowflake.py` & `leanit-mweb-23.7.4/tests/utils/test_snowflake.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.7.3/tests/views/model/test_paging.py` & `leanit-mweb-23.7.4/tests/views/model/test_paging.py`

 * *Files identical despite different names*

