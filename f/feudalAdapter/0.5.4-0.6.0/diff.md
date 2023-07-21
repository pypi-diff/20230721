# Comparing `tmp/feudalAdapter-0.5.4.tar.gz` & `tmp/feudalAdapter-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feudalAdapter-0.5.4.tar", last modified: Tue Jun 20 08:15:16 2023, max compression
+gzip compressed data, was "feudalAdapter-0.6.0.tar", last modified: Fri Jul 21 09:04:51 2023, max compression
```

## Comparing `feudalAdapter-0.5.4.tar` & `feudalAdapter-0.6.0.tar`

### file list

```diff
@@ -1,105 +1,106 @@
-drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-06-20 08:15:16.777137 feudalAdapter-0.5.4/
--rw-r--r--   0 diana     (1000) diana     (1000)     1212 2023-06-16 10:14:56.000000 feudalAdapter-0.5.4/.gitlab-ci.yml
--rw-r--r--   0 diana     (1000) diana     (1000)      409 2023-06-20 08:15:13.000000 feudalAdapter-0.5.4/AUTHORS
--rw-r--r--   0 diana     (1000) diana     (1000)    20780 2023-06-20 08:15:13.000000 feudalAdapter-0.5.4/ChangeLog
--rw-r--r--   0 diana     (1000) diana     (1000)     8427 2022-02-17 10:03:18.000000 feudalAdapter-0.5.4/LDAP.md
--rw-r--r--   0 diana     (1000) diana     (1000)     1130 2020-12-22 11:09:29.000000 feudalAdapter-0.5.4/LICENSE
--rw-r--r--   0 diana     (1000) diana     (1000)    17562 2023-06-20 08:15:16.777137 feudalAdapter-0.5.4/PKG-INFO
--rw-r--r--   0 diana     (1000) diana     (1000)    16606 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/README.md
--rw-r--r--   0 diana     (1000) diana     (1000)     2672 2020-12-22 11:09:29.000000 feudalAdapter-0.5.4/conftest.py
--rw-r--r--   0 diana     (1000) diana     (1000)      403 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/devel-requirements.txt
-drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-06-20 08:15:16.730471 feudalAdapter-0.5.4/examples/
--rw-r--r--   0 diana     (1000) diana     (1000)      206 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/examples/diana-accept.json
--rw-r--r--   0 diana     (1000) diana     (1000)     2238 2022-11-07 10:43:24.000000 feudalAdapter-0.5.4/examples/diana-deploy-punch4nfdi.json
--rw-r--r--   0 diana     (1000) diana     (1000)     1193 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/examples/diana-deploy.json
--rw-r--r--   0 diana     (1000) diana     (1000)      208 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/examples/diana-get_status.json
--rw-r--r--   0 diana     (1000) diana     (1000)      206 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/examples/diana-reject.json
--rw-r--r--   0 diana     (1000) diana     (1000)      129 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/examples/diana-test-approval.json
--rw-r--r--   0 diana     (1000) diana     (1000)     2565 2020-12-22 11:09:29.000000 feudalAdapter-0.5.4/examples/lukas_deply.json
--rw-r--r--   0 diana     (1000) diana     (1000)     7306 2022-02-17 10:03:18.000000 feudalAdapter-0.5.4/examples/marcus-deploy-egi.json
--rw-r--r--   0 diana     (1000) diana     (1000)     1990 2021-01-26 21:58:12.000000 feudalAdapter-0.5.4/examples/marcus-deploy-iam-groups.json
--rw-r--r--   0 diana     (1000) diana     (1000)     1791 2021-01-26 21:58:12.000000 feudalAdapter-0.5.4/examples/marcus-deploy-no-groups.json
--rw-r--r--   0 diana     (1000) diana     (1000)     2657 2021-01-08 15:30:24.000000 feudalAdapter-0.5.4/examples/marcus-deploy-no-pref-username.json
--rw-r--r--   0 diana     (1000) diana     (1000)     2786 2022-02-17 10:03:18.000000 feudalAdapter-0.5.4/examples/marcus-deploy-other-id.json
--rw-r--r--   0 diana     (1000) diana     (1000)      205 2021-01-08 15:30:24.000000 feudalAdapter-0.5.4/examples/marcus-get_status.json
--rw-r--r--   0 diana     (1000) diana     (1000)     7310 2022-02-17 10:03:18.000000 feudalAdapter-0.5.4/examples/marcus-undeploy-egi.json
--rw-r--r--   0 diana     (1000) diana     (1000)      207 2022-02-17 10:03:18.000000 feudalAdapter-0.5.4/examples/marcus-undeploy-minimal.json
--rw-r--r--   0 diana     (1000) diana     (1000)      223 2022-02-17 10:03:18.000000 feudalAdapter-0.5.4/examples/marcus-undeploy-old.json
--rw-r--r--   0 diana     (1000) diana     (1000)     1217 2022-02-17 10:03:18.000000 feudalAdapter-0.5.4/examples/marcus-undeploy-other-id.json
--rw-r--r--   0 diana     (1000) diana     (1000)      760 2021-01-08 15:30:24.000000 feudalAdapter-0.5.4/examples/marcus-undeploy.json
-drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-06-20 08:15:16.733804 feudalAdapter-0.5.4/feudalAdapter.egg-info/
--rw-r--r--   0 diana     (1000) diana     (1000)    17562 2023-06-20 08:15:13.000000 feudalAdapter-0.5.4/feudalAdapter.egg-info/PKG-INFO
--rw-r--r--   0 diana     (1000) diana     (1000)     2458 2023-06-20 08:15:16.000000 feudalAdapter-0.5.4/feudalAdapter.egg-info/SOURCES.txt
--rw-r--r--   0 diana     (1000) diana     (1000)        1 2023-06-20 08:15:13.000000 feudalAdapter-0.5.4/feudalAdapter.egg-info/dependency_links.txt
--rw-r--r--   0 diana     (1000) diana     (1000)      103 2023-06-20 08:15:13.000000 feudalAdapter-0.5.4/feudalAdapter.egg-info/entry_points.txt
--rw-r--r--   0 diana     (1000) diana     (1000)        1 2020-12-22 14:42:04.000000 feudalAdapter-0.5.4/feudalAdapter.egg-info/not-zip-safe
--rw-r--r--   0 diana     (1000) diana     (1000)       47 2023-06-20 08:15:13.000000 feudalAdapter-0.5.4/feudalAdapter.egg-info/pbr.json
--rw-r--r--   0 diana     (1000) diana     (1000)      412 2023-06-20 08:15:13.000000 feudalAdapter-0.5.4/feudalAdapter.egg-info/requires.txt
--rw-r--r--   0 diana     (1000) diana     (1000)       32 2023-06-20 08:15:13.000000 feudalAdapter-0.5.4/feudalAdapter.egg-info/top_level.txt
--rw-r--r--   0 diana     (1000) diana     (1000)    12589 2022-11-07 10:43:24.000000 feudalAdapter-0.5.4/feudal_adapter_template.conf
-drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-06-20 08:15:16.733804 feudalAdapter-0.5.4/feudal_globalconfig/
--rw-r--r--   0 diana     (1000) diana     (1000)        0 2021-01-15 14:31:35.000000 feudalAdapter-0.5.4/feudal_globalconfig/__init__.py
--rw-r--r--   0 diana     (1000) diana     (1000)       89 2022-02-17 10:03:18.000000 feudalAdapter-0.5.4/feudal_globalconfig/globalconfig.py
-drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-06-20 08:15:16.737137 feudalAdapter-0.5.4/ldf_adapter/
--rw-r--r--   0 diana     (1000) diana     (1000)    35785 2023-06-16 10:05:18.000000 feudalAdapter-0.5.4/ldf_adapter/__init__.py
-drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-06-20 08:15:16.737137 feudalAdapter-0.5.4/ldf_adapter/approval/
--rw-r--r--   0 diana     (1000) diana     (1000)    12504 2023-06-16 10:06:16.000000 feudalAdapter-0.5.4/ldf_adapter/approval/__init__.py
-drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-06-20 08:15:16.737137 feudalAdapter-0.5.4/ldf_adapter/approval/db/
--rw-r--r--   0 diana     (1000) diana     (1000)      185 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/ldf_adapter/approval/db/__init__.py
--rw-r--r--   0 diana     (1000) diana     (1000)     3289 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/ldf_adapter/approval/db/generic.py
--rw-r--r--   0 diana     (1000) diana     (1000)    20008 2023-06-16 10:06:16.000000 feudalAdapter-0.5.4/ldf_adapter/approval/db/sqlite.py
--rw-r--r--   0 diana     (1000) diana     (1000)     1843 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/ldf_adapter/approval/models.py
-drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-06-20 08:15:16.740471 feudalAdapter-0.5.4/ldf_adapter/backend/
--rw-r--r--   0 diana     (1000) diana     (1000)      407 2023-06-16 10:05:17.000000 feudalAdapter-0.5.4/ldf_adapter/backend/__init__.py
--rw-r--r--   0 diana     (1000) diana     (1000)    18388 2023-06-16 10:05:17.000000 feudalAdapter-0.5.4/ldf_adapter/backend/bwidm.py
--rw-r--r--   0 diana     (1000) diana     (1000)     6172 2022-11-07 10:43:24.000000 feudalAdapter-0.5.4/ldf_adapter/backend/generic.py
--rw-r--r--   0 diana     (1000) diana     (1000)    35962 2023-06-16 10:06:16.000000 feudalAdapter-0.5.4/ldf_adapter/backend/ldap.py
--rw-r--r--   0 diana     (1000) diana     (1000)    33784 2023-06-16 10:06:34.000000 feudalAdapter-0.5.4/ldf_adapter/backend/local_unix.py
--rw-r--r--   0 diana     (1000) diana     (1000)     1343 2023-06-16 10:05:17.000000 feudalAdapter-0.5.4/ldf_adapter/cmdline_params.py
--rw-r--r--   0 diana     (1000) diana     (1000)    12853 2023-06-16 10:07:10.000000 feudalAdapter-0.5.4/ldf_adapter/config.py
--rw-r--r--   0 diana     (1000) diana     (1000)     3330 2023-06-16 10:05:17.000000 feudalAdapter-0.5.4/ldf_adapter/eduperson.py
--rwxr-xr-x   0 diana     (1000) diana     (1000)     2381 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/ldf_adapter/interface.py
--rw-r--r--   0 diana     (1000) diana     (1000)     4052 2023-06-16 10:05:17.000000 feudalAdapter-0.5.4/ldf_adapter/logsetup.py
--rw-r--r--   0 diana     (1000) diana     (1000)     4833 2023-06-16 10:06:33.000000 feudalAdapter-0.5.4/ldf_adapter/name_generators.py
-drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-06-20 08:15:16.747137 feudalAdapter-0.5.4/ldf_adapter/notifier/
--rw-r--r--   0 diana     (1000) diana     (1000)      184 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/ldf_adapter/notifier/__init__.py
--rw-r--r--   0 diana     (1000) diana     (1000)     1486 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/ldf_adapter/notifier/courier.py
--rw-r--r--   0 diana     (1000) diana     (1000)     6348 2023-06-16 10:06:16.000000 feudalAdapter-0.5.4/ldf_adapter/notifier/email.py
--rw-r--r--   0 diana     (1000) diana     (1000)     2259 2023-06-16 10:05:17.000000 feudalAdapter-0.5.4/ldf_adapter/notifier/generic.py
--rw-r--r--   0 diana     (1000) diana     (1000)     5241 2023-06-16 10:05:17.000000 feudalAdapter-0.5.4/ldf_adapter/results.py
--rw-r--r--   0 diana     (1000) diana     (1000)    16459 2023-06-16 10:06:34.000000 feudalAdapter-0.5.4/ldf_adapter/userinfo.py
--rw-r--r--   0 diana     (1000) diana     (1000)     6987 2023-06-16 10:05:17.000000 feudalAdapter-0.5.4/ldf_adapter/utils.py
--rw-r--r--   0 diana     (1000) diana     (1000)      182 2022-02-17 10:03:18.000000 feudalAdapter-0.5.4/pytest.ini
--rw-r--r--   0 diana     (1000) diana     (1000)      412 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/requirements.txt
--rw-r--r--   0 diana     (1000) diana     (1000)     1391 2023-06-20 08:15:16.780470 feudalAdapter-0.5.4/setup.cfg
--rwxr-xr-x   0 diana     (1000) diana     (1000)      110 2020-12-22 11:09:29.000000 feudalAdapter-0.5.4/setup.py
--rw-r--r--   0 diana     (1000) diana     (1000)     6217 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/states.md
--rwxr-xr-x   0 diana     (1000) diana     (1000)     6539 2020-11-06 10:06:35.000000 feudalAdapter-0.5.4/subiss-to-unix.py
-drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-06-20 08:15:16.757137 feudalAdapter-0.5.4/templates/
--rw-r--r--   0 diana     (1000) diana     (1000)     1084 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/templates/admin.deploy.template
--rw-r--r--   0 diana     (1000) diana     (1000)     1051 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/templates/admin.deploy.update.template
--rw-r--r--   0 diana     (1000) diana     (1000)      302 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/templates/admin.test.template
--rw-r--r--   0 diana     (1000) diana     (1000)      991 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/templates/admin.update.template
--rw-r--r--   0 diana     (1000) diana     (1000)      255 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/templates/unknown.template
--rw-r--r--   0 diana     (1000) diana     (1000)      380 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/templates/user.deploy.template
--rw-r--r--   0 diana     (1000) diana     (1000)      417 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/templates/user.deploy.update.template
--rw-r--r--   0 diana     (1000) diana     (1000)      395 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/templates/user.update.template
-drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-06-20 08:15:16.767137 feudalAdapter-0.5.4/tests/
--rw-r--r--   0 diana     (1000) diana     (1000)        0 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/tests/__init__.py
-drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-06-20 08:15:16.767137 feudalAdapter-0.5.4/tests/approval/
-drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-06-20 08:15:16.770470 feudalAdapter-0.5.4/tests/approval/db/
--rw-r--r--   0 diana     (1000) diana     (1000)     7601 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/tests/approval/db/generic.py
--rw-r--r--   0 diana     (1000) diana     (1000)    23145 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/tests/approval/db/sqlite.py
--rw-r--r--   0 diana     (1000) diana     (1000)        0 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/tests/approval/pending_deployment.py
-drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-06-20 08:15:16.777137 feudalAdapter-0.5.4/tests/backend/
--rw-r--r--   0 diana     (1000) diana     (1000)        0 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/tests/backend/__init__.py
--rw-r--r--   0 diana     (1000) diana     (1000)    18764 2022-11-07 10:43:24.000000 feudalAdapter-0.5.4/tests/backend/ldap.py
--rw-r--r--   0 diana     (1000) diana     (1000)    19654 2022-11-07 10:43:24.000000 feudalAdapter-0.5.4/tests/backend/local_unix.py
--rw-r--r--   0 diana     (1000) diana     (1000)      217 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/tests/conftest.py
--rw-r--r--   0 diana     (1000) diana     (1000)     5778 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/tests/eduperson.py
--rw-r--r--   0 diana     (1000) diana     (1000)    11209 2022-11-07 10:43:24.000000 feudalAdapter-0.5.4/tests/feudal_adapter.conf
--rw-r--r--   0 diana     (1000) diana     (1000)    17765 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/tests/name_generators.py
--rw-r--r--   0 diana     (1000) diana     (1000)     5645 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/tests/settings.py
--rw-r--r--   0 diana     (1000) diana     (1000)    13297 2022-11-07 10:43:24.000000 feudalAdapter-0.5.4/tests/user.py
--rw-r--r--   0 diana     (1000) diana     (1000)    14757 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/tests/userinfo.py
--rw-r--r--   0 diana     (1000) diana     (1000)     1218 2023-06-16 10:00:21.000000 feudalAdapter-0.5.4/tox.ini
+drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-07-21 09:04:51.210094 feudalAdapter-0.6.0/
+-rw-r--r--   0 diana     (1000) diana     (1000)     1212 2023-06-16 10:14:56.000000 feudalAdapter-0.6.0/.gitlab-ci.yml
+-rw-r--r--   0 diana     (1000) diana     (1000)      457 2023-07-21 09:04:49.000000 feudalAdapter-0.6.0/AUTHORS
+-rw-r--r--   0 diana     (1000) diana     (1000)    21223 2023-07-21 09:04:49.000000 feudalAdapter-0.6.0/ChangeLog
+-rw-r--r--   0 diana     (1000) diana     (1000)     8427 2022-02-17 10:03:18.000000 feudalAdapter-0.6.0/LDAP.md
+-rw-r--r--   0 diana     (1000) diana     (1000)     1130 2020-12-22 11:09:29.000000 feudalAdapter-0.6.0/LICENSE
+-rw-r--r--   0 diana     (1000) diana     (1000)    17562 2023-07-21 09:04:51.210094 feudalAdapter-0.6.0/PKG-INFO
+-rw-r--r--   0 diana     (1000) diana     (1000)    16606 2022-09-21 14:19:00.000000 feudalAdapter-0.6.0/README.md
+-rw-r--r--   0 diana     (1000) diana     (1000)     2672 2020-12-22 11:09:29.000000 feudalAdapter-0.6.0/conftest.py
+-rw-r--r--   0 diana     (1000) diana     (1000)      403 2022-09-21 14:19:00.000000 feudalAdapter-0.6.0/devel-requirements.txt
+drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-07-21 09:04:51.196761 feudalAdapter-0.6.0/examples/
+-rw-r--r--   0 diana     (1000) diana     (1000)      206 2022-09-21 14:19:00.000000 feudalAdapter-0.6.0/examples/diana-accept.json
+-rw-r--r--   0 diana     (1000) diana     (1000)     2238 2022-11-07 10:43:24.000000 feudalAdapter-0.6.0/examples/diana-deploy-punch4nfdi.json
+-rw-r--r--   0 diana     (1000) diana     (1000)     1193 2022-09-21 14:19:00.000000 feudalAdapter-0.6.0/examples/diana-deploy.json
+-rw-r--r--   0 diana     (1000) diana     (1000)      208 2022-09-21 14:19:00.000000 feudalAdapter-0.6.0/examples/diana-get_status.json
+-rw-r--r--   0 diana     (1000) diana     (1000)      206 2022-09-21 14:19:00.000000 feudalAdapter-0.6.0/examples/diana-reject.json
+-rw-r--r--   0 diana     (1000) diana     (1000)      129 2022-09-21 14:19:00.000000 feudalAdapter-0.6.0/examples/diana-test-approval.json
+-rw-r--r--   0 diana     (1000) diana     (1000)     2565 2020-12-22 11:09:29.000000 feudalAdapter-0.6.0/examples/lukas_deply.json
+-rw-r--r--   0 diana     (1000) diana     (1000)     7306 2022-02-17 10:03:18.000000 feudalAdapter-0.6.0/examples/marcus-deploy-egi.json
+-rw-r--r--   0 diana     (1000) diana     (1000)     1990 2021-01-26 21:58:12.000000 feudalAdapter-0.6.0/examples/marcus-deploy-iam-groups.json
+-rw-r--r--   0 diana     (1000) diana     (1000)     1791 2021-01-26 21:58:12.000000 feudalAdapter-0.6.0/examples/marcus-deploy-no-groups.json
+-rw-r--r--   0 diana     (1000) diana     (1000)     2657 2021-01-08 15:30:24.000000 feudalAdapter-0.6.0/examples/marcus-deploy-no-pref-username.json
+-rw-r--r--   0 diana     (1000) diana     (1000)     2786 2022-02-17 10:03:18.000000 feudalAdapter-0.6.0/examples/marcus-deploy-other-id.json
+-rw-r--r--   0 diana     (1000) diana     (1000)      205 2021-01-08 15:30:24.000000 feudalAdapter-0.6.0/examples/marcus-get_status.json
+-rw-r--r--   0 diana     (1000) diana     (1000)     7310 2022-02-17 10:03:18.000000 feudalAdapter-0.6.0/examples/marcus-undeploy-egi.json
+-rw-r--r--   0 diana     (1000) diana     (1000)      207 2022-02-17 10:03:18.000000 feudalAdapter-0.6.0/examples/marcus-undeploy-minimal.json
+-rw-r--r--   0 diana     (1000) diana     (1000)      223 2022-02-17 10:03:18.000000 feudalAdapter-0.6.0/examples/marcus-undeploy-old.json
+-rw-r--r--   0 diana     (1000) diana     (1000)     1217 2022-02-17 10:03:18.000000 feudalAdapter-0.6.0/examples/marcus-undeploy-other-id.json
+-rw-r--r--   0 diana     (1000) diana     (1000)      760 2021-01-08 15:30:24.000000 feudalAdapter-0.6.0/examples/marcus-undeploy.json
+drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-07-21 09:04:51.196761 feudalAdapter-0.6.0/feudalAdapter.egg-info/
+-rw-r--r--   0 diana     (1000) diana     (1000)    17562 2023-07-21 09:04:49.000000 feudalAdapter-0.6.0/feudalAdapter.egg-info/PKG-INFO
+-rw-r--r--   0 diana     (1000) diana     (1000)     2487 2023-07-21 09:04:51.000000 feudalAdapter-0.6.0/feudalAdapter.egg-info/SOURCES.txt
+-rw-r--r--   0 diana     (1000) diana     (1000)        1 2023-07-21 09:04:49.000000 feudalAdapter-0.6.0/feudalAdapter.egg-info/dependency_links.txt
+-rw-r--r--   0 diana     (1000) diana     (1000)      103 2023-07-21 09:04:49.000000 feudalAdapter-0.6.0/feudalAdapter.egg-info/entry_points.txt
+-rw-r--r--   0 diana     (1000) diana     (1000)        1 2020-12-22 14:42:04.000000 feudalAdapter-0.6.0/feudalAdapter.egg-info/not-zip-safe
+-rw-r--r--   0 diana     (1000) diana     (1000)       47 2023-07-21 09:04:49.000000 feudalAdapter-0.6.0/feudalAdapter.egg-info/pbr.json
+-rw-r--r--   0 diana     (1000) diana     (1000)      412 2023-07-21 09:04:49.000000 feudalAdapter-0.6.0/feudalAdapter.egg-info/requires.txt
+-rw-r--r--   0 diana     (1000) diana     (1000)       32 2023-07-21 09:04:49.000000 feudalAdapter-0.6.0/feudalAdapter.egg-info/top_level.txt
+-rw-r--r--   0 diana     (1000) diana     (1000)    13595 2023-07-21 08:56:12.000000 feudalAdapter-0.6.0/feudal_adapter_template.conf
+drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-07-21 09:04:51.200094 feudalAdapter-0.6.0/feudal_globalconfig/
+-rw-r--r--   0 diana     (1000) diana     (1000)        0 2021-01-15 14:31:35.000000 feudalAdapter-0.6.0/feudal_globalconfig/__init__.py
+-rw-r--r--   0 diana     (1000) diana     (1000)       89 2022-02-17 10:03:18.000000 feudalAdapter-0.6.0/feudal_globalconfig/globalconfig.py
+drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-07-21 09:04:51.200094 feudalAdapter-0.6.0/ldf_adapter/
+-rw-r--r--   0 diana     (1000) diana     (1000)    37164 2023-07-21 09:02:36.000000 feudalAdapter-0.6.0/ldf_adapter/__init__.py
+drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-07-21 09:04:51.200094 feudalAdapter-0.6.0/ldf_adapter/approval/
+-rw-r--r--   0 diana     (1000) diana     (1000)    12663 2023-07-21 09:02:36.000000 feudalAdapter-0.6.0/ldf_adapter/approval/__init__.py
+drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-07-21 09:04:51.200094 feudalAdapter-0.6.0/ldf_adapter/approval/db/
+-rw-r--r--   0 diana     (1000) diana     (1000)      185 2022-09-21 14:19:00.000000 feudalAdapter-0.6.0/ldf_adapter/approval/db/__init__.py
+-rw-r--r--   0 diana     (1000) diana     (1000)     3289 2022-09-21 14:19:00.000000 feudalAdapter-0.6.0/ldf_adapter/approval/db/generic.py
+-rw-r--r--   0 diana     (1000) diana     (1000)    20956 2023-07-21 09:02:36.000000 feudalAdapter-0.6.0/ldf_adapter/approval/db/sqlite.py
+-rw-r--r--   0 diana     (1000) diana     (1000)     1843 2022-09-21 14:19:00.000000 feudalAdapter-0.6.0/ldf_adapter/approval/models.py
+drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-07-21 09:04:51.203428 feudalAdapter-0.6.0/ldf_adapter/backend/
+-rw-r--r--   0 diana     (1000) diana     (1000)      419 2023-07-21 09:02:36.000000 feudalAdapter-0.6.0/ldf_adapter/backend/__init__.py
+-rw-r--r--   0 diana     (1000) diana     (1000)    19144 2023-07-21 08:56:12.000000 feudalAdapter-0.6.0/ldf_adapter/backend/bwidm.py
+-rw-r--r--   0 diana     (1000) diana     (1000)     6133 2023-07-21 08:56:12.000000 feudalAdapter-0.6.0/ldf_adapter/backend/generic.py
+-rw-r--r--   0 diana     (1000) diana     (1000)     1463 2023-07-21 08:56:12.000000 feudalAdapter-0.6.0/ldf_adapter/backend/hooks.py
+-rw-r--r--   0 diana     (1000) diana     (1000)    36460 2023-07-21 08:56:12.000000 feudalAdapter-0.6.0/ldf_adapter/backend/ldap.py
+-rw-r--r--   0 diana     (1000) diana     (1000)    34848 2023-07-21 08:56:12.000000 feudalAdapter-0.6.0/ldf_adapter/backend/local_unix.py
+-rw-r--r--   0 diana     (1000) diana     (1000)     1357 2023-07-21 09:02:36.000000 feudalAdapter-0.6.0/ldf_adapter/cmdline_params.py
+-rw-r--r--   0 diana     (1000) diana     (1000)    13055 2023-07-21 08:56:12.000000 feudalAdapter-0.6.0/ldf_adapter/config.py
+-rw-r--r--   0 diana     (1000) diana     (1000)     3422 2023-07-21 09:02:36.000000 feudalAdapter-0.6.0/ldf_adapter/eduperson.py
+-rwxr-xr-x   0 diana     (1000) diana     (1000)     2381 2022-09-21 14:19:00.000000 feudalAdapter-0.6.0/ldf_adapter/interface.py
+-rw-r--r--   0 diana     (1000) diana     (1000)     4072 2023-07-21 09:02:36.000000 feudalAdapter-0.6.0/ldf_adapter/logsetup.py
+-rw-r--r--   0 diana     (1000) diana     (1000)     4833 2023-06-16 10:06:33.000000 feudalAdapter-0.6.0/ldf_adapter/name_generators.py
+drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-07-21 09:04:51.203428 feudalAdapter-0.6.0/ldf_adapter/notifier/
+-rw-r--r--   0 diana     (1000) diana     (1000)      184 2022-09-21 14:19:00.000000 feudalAdapter-0.6.0/ldf_adapter/notifier/__init__.py
+-rw-r--r--   0 diana     (1000) diana     (1000)     1486 2022-09-21 14:19:00.000000 feudalAdapter-0.6.0/ldf_adapter/notifier/courier.py
+-rw-r--r--   0 diana     (1000) diana     (1000)     6493 2023-07-21 09:02:36.000000 feudalAdapter-0.6.0/ldf_adapter/notifier/email.py
+-rw-r--r--   0 diana     (1000) diana     (1000)     2281 2023-07-21 09:02:36.000000 feudalAdapter-0.6.0/ldf_adapter/notifier/generic.py
+-rw-r--r--   0 diana     (1000) diana     (1000)     5263 2023-07-21 09:02:36.000000 feudalAdapter-0.6.0/ldf_adapter/results.py
+-rw-r--r--   0 diana     (1000) diana     (1000)    16815 2023-07-21 09:02:36.000000 feudalAdapter-0.6.0/ldf_adapter/userinfo.py
+-rw-r--r--   0 diana     (1000) diana     (1000)     7153 2023-07-21 09:02:36.000000 feudalAdapter-0.6.0/ldf_adapter/utils.py
+-rw-r--r--   0 diana     (1000) diana     (1000)      182 2022-02-17 10:03:18.000000 feudalAdapter-0.6.0/pytest.ini
+-rw-r--r--   0 diana     (1000) diana     (1000)      412 2022-09-21 14:19:00.000000 feudalAdapter-0.6.0/requirements.txt
+-rw-r--r--   0 diana     (1000) diana     (1000)     1391 2023-07-21 09:04:51.213428 feudalAdapter-0.6.0/setup.cfg
+-rwxr-xr-x   0 diana     (1000) diana     (1000)      110 2020-12-22 11:09:29.000000 feudalAdapter-0.6.0/setup.py
+-rw-r--r--   0 diana     (1000) diana     (1000)     6217 2022-09-21 14:19:00.000000 feudalAdapter-0.6.0/states.md
+-rwxr-xr-x   0 diana     (1000) diana     (1000)     6539 2020-11-06 10:06:35.000000 feudalAdapter-0.6.0/subiss-to-unix.py
+drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-07-21 09:04:51.206761 feudalAdapter-0.6.0/templates/
+-rw-r--r--   0 diana     (1000) diana     (1000)     1084 2022-09-21 14:19:00.000000 feudalAdapter-0.6.0/templates/admin.deploy.template
+-rw-r--r--   0 diana     (1000) diana     (1000)     1051 2022-09-21 14:19:00.000000 feudalAdapter-0.6.0/templates/admin.deploy.update.template
+-rw-r--r--   0 diana     (1000) diana     (1000)      302 2022-09-21 14:19:00.000000 feudalAdapter-0.6.0/templates/admin.test.template
+-rw-r--r--   0 diana     (1000) diana     (1000)      991 2022-09-21 14:19:00.000000 feudalAdapter-0.6.0/templates/admin.update.template
+-rw-r--r--   0 diana     (1000) diana     (1000)      255 2022-09-21 14:19:00.000000 feudalAdapter-0.6.0/templates/unknown.template
+-rw-r--r--   0 diana     (1000) diana     (1000)      380 2022-09-21 14:19:00.000000 feudalAdapter-0.6.0/templates/user.deploy.template
+-rw-r--r--   0 diana     (1000) diana     (1000)      417 2022-09-21 14:19:00.000000 feudalAdapter-0.6.0/templates/user.deploy.update.template
+-rw-r--r--   0 diana     (1000) diana     (1000)      395 2022-09-21 14:19:00.000000 feudalAdapter-0.6.0/templates/user.update.template
+drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-07-21 09:04:51.210094 feudalAdapter-0.6.0/tests/
+-rw-r--r--   0 diana     (1000) diana     (1000)        0 2022-09-21 14:19:00.000000 feudalAdapter-0.6.0/tests/__init__.py
+drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-07-21 09:04:51.210094 feudalAdapter-0.6.0/tests/approval/
+drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-07-21 09:04:51.210094 feudalAdapter-0.6.0/tests/approval/db/
+-rw-r--r--   0 diana     (1000) diana     (1000)     7686 2023-07-21 09:02:41.000000 feudalAdapter-0.6.0/tests/approval/db/generic.py
+-rw-r--r--   0 diana     (1000) diana     (1000)    24024 2023-07-21 09:02:42.000000 feudalAdapter-0.6.0/tests/approval/db/sqlite.py
+-rw-r--r--   0 diana     (1000) diana     (1000)        0 2022-09-21 14:19:00.000000 feudalAdapter-0.6.0/tests/approval/pending_deployment.py
+drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-07-21 09:04:51.210094 feudalAdapter-0.6.0/tests/backend/
+-rw-r--r--   0 diana     (1000) diana     (1000)        0 2022-09-21 14:19:00.000000 feudalAdapter-0.6.0/tests/backend/__init__.py
+-rw-r--r--   0 diana     (1000) diana     (1000)    19009 2023-07-21 09:02:41.000000 feudalAdapter-0.6.0/tests/backend/ldap.py
+-rw-r--r--   0 diana     (1000) diana     (1000)    19841 2023-07-21 09:02:41.000000 feudalAdapter-0.6.0/tests/backend/local_unix.py
+-rw-r--r--   0 diana     (1000) diana     (1000)      217 2022-09-21 14:19:00.000000 feudalAdapter-0.6.0/tests/conftest.py
+-rw-r--r--   0 diana     (1000) diana     (1000)     6303 2023-07-21 09:02:41.000000 feudalAdapter-0.6.0/tests/eduperson.py
+-rw-r--r--   0 diana     (1000) diana     (1000)    11209 2022-11-07 10:43:24.000000 feudalAdapter-0.6.0/tests/feudal_adapter.conf
+-rw-r--r--   0 diana     (1000) diana     (1000)    17765 2022-09-21 14:19:00.000000 feudalAdapter-0.6.0/tests/name_generators.py
+-rw-r--r--   0 diana     (1000) diana     (1000)     5645 2022-09-21 14:19:00.000000 feudalAdapter-0.6.0/tests/settings.py
+-rw-r--r--   0 diana     (1000) diana     (1000)    14084 2023-07-21 09:02:41.000000 feudalAdapter-0.6.0/tests/user.py
+-rw-r--r--   0 diana     (1000) diana     (1000)    14763 2023-07-21 09:02:41.000000 feudalAdapter-0.6.0/tests/userinfo.py
+-rw-r--r--   0 diana     (1000) diana     (1000)     1211 2023-07-21 09:02:13.000000 feudalAdapter-0.6.0/tox.ini
```

### Comparing `feudalAdapter-0.5.4/.gitlab-ci.yml` & `feudalAdapter-0.6.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.4/ChangeLog` & `feudalAdapter-0.6.0/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,26 @@
 CHANGES
 =======
 
+v0.6.0
+------
+
+* use black with default line length
+* add execute method to mock backend in tests
+* optional backend methods should not be abstract
+* check if hook is configured for backend
+* check if hook supported by backend
+* make backend hooks generic
+* update template
+* set ldap protocol based on tls option in config
+* black
+* add post create hook for all backends
+* black
+* add functionalty to run a script after the account creation
+
 v0.5.4
 ------
 
 * add tests for python 3.11 to gitlab ci
 * apply black
 * add python 3.11 to test envs in tox
 * use default\_factory for fields of custom types
```

### Comparing `feudalAdapter-0.5.4/LDAP.md` & `feudalAdapter-0.6.0/LDAP.md`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.4/LICENSE` & `feudalAdapter-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.4/PKG-INFO` & `feudalAdapter-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feudalAdapter
-Version: 0.5.4
+Version: 0.6.0
 Summary: Adapter to connect provisioning events with a backend
 Home-page: https://git.scc.kit.edu/feudal/feudal_adapter_ldf
 Author: Joshua Bachmeier
 Author-email: joshua.bachmeier@student.kit.edu
 License: MIT
 Project-URL: Bug Tracker, https://git.scc.kit.edu/feudal/feudal_adapter_ldf/issues
 Project-URL: Documentation, https://git.scc.kit.edu/feudal/feudal_adapter_ldf
```

### Comparing `feudalAdapter-0.5.4/README.md` & `feudalAdapter-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.4/conftest.py` & `feudalAdapter-0.6.0/conftest.py`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.4/examples/diana-deploy-punch4nfdi.json` & `feudalAdapter-0.6.0/examples/diana-deploy-punch4nfdi.json`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.4/examples/diana-deploy.json` & `feudalAdapter-0.6.0/examples/diana-deploy.json`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.4/examples/lukas_deply.json` & `feudalAdapter-0.6.0/examples/lukas_deply.json`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.4/examples/marcus-deploy-egi.json` & `feudalAdapter-0.6.0/examples/marcus-deploy-egi.json`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.4/examples/marcus-deploy-iam-groups.json` & `feudalAdapter-0.6.0/examples/marcus-deploy-iam-groups.json`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.4/examples/marcus-deploy-no-groups.json` & `feudalAdapter-0.6.0/examples/marcus-deploy-no-groups.json`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.4/examples/marcus-deploy-no-pref-username.json` & `feudalAdapter-0.6.0/examples/marcus-deploy-no-pref-username.json`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.4/examples/marcus-deploy-other-id.json` & `feudalAdapter-0.6.0/examples/marcus-deploy-other-id.json`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.4/examples/marcus-undeploy-egi.json` & `feudalAdapter-0.6.0/examples/marcus-undeploy-egi.json`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.4/examples/marcus-undeploy-other-id.json` & `feudalAdapter-0.6.0/examples/marcus-undeploy-other-id.json`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.4/examples/marcus-undeploy.json` & `feudalAdapter-0.6.0/examples/marcus-undeploy.json`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.4/feudalAdapter.egg-info/PKG-INFO` & `feudalAdapter-0.6.0/feudalAdapter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feudalAdapter
-Version: 0.5.4
+Version: 0.6.0
 Summary: Adapter to connect provisioning events with a backend
 Home-page: https://git.scc.kit.edu/feudal/feudal_adapter_ldf
 Author: Joshua Bachmeier
 Author-email: joshua.bachmeier@student.kit.edu
 License: MIT
 Project-URL: Bug Tracker, https://git.scc.kit.edu/feudal/feudal_adapter_ldf/issues
 Project-URL: Documentation, https://git.scc.kit.edu/feudal/feudal_adapter_ldf
```

### Comparing `feudalAdapter-0.5.4/feudalAdapter.egg-info/SOURCES.txt` & `feudalAdapter-0.6.0/feudalAdapter.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 ldf_adapter/approval/models.py
 ldf_adapter/approval/db/__init__.py
 ldf_adapter/approval/db/generic.py
 ldf_adapter/approval/db/sqlite.py
 ldf_adapter/backend/__init__.py
 ldf_adapter/backend/bwidm.py
 ldf_adapter/backend/generic.py
+ldf_adapter/backend/hooks.py
 ldf_adapter/backend/ldap.py
 ldf_adapter/backend/local_unix.py
 ldf_adapter/notifier/__init__.py
 ldf_adapter/notifier/courier.py
 ldf_adapter/notifier/email.py
 ldf_adapter/notifier/generic.py
 templates/admin.deploy.template
```

### Comparing `feudalAdapter-0.5.4/feudal_adapter_template.conf` & `feudalAdapter-0.6.0/feudal_adapter_template.conf`

 * *Files 6% similar despite different names*

```diff
@@ -271,14 +271,21 @@
 # Allows using ssh keys, when they are found in the deployment request
 # deploy_user_ssh_keys = yes
 
 # punch4nfdi -- default: no
 # If set to yes, we will use the punch4nfdi-specific method to translate group names
 # punch4nfdi = no
 
+## post_create_script -- default: None
+## A script to be executed after a user has been created
+# this script can be a shell script or a python script
+# and will be run with root privileges
+# the script will be called with the username as the first and only argument
+# post_create_script = /path/to/script.sh
+
 [backend.bwidm]
 # Configuration for the bwidm backend
 
 ### url
 # The base URL of the bwidm API
 url = https://bwidm-test.scc.kit.edu/rest
 
@@ -292,14 +299,21 @@
 # HTTP basic auth to connect to BWIDM API
 http_user = foo
 http_pass = bar
 
 # The name of the service the user should be added to on BWIDM:
 service_name = sshtest
 
+## post_create_script -- default: None
+## A script to be executed after a user has been created
+# this script can be a shell script or a python script
+# and will be run with root privileges
+# the script will be called with the username as the first and only argument
+# post_create_script = /path/to/script.sh
+
 [backend.ldap]
 # Configuration for the ldap backend
 
 # The ldap backend can function in 3 different modes:
 # - read_only (default): there is read only access to the LDAP, therefore the local accounts
 #       need to already be created in the LDAP and mapped to the federated accounts;
 #       read the docs for more on how to map local <-> federated accounts.
@@ -320,15 +334,16 @@
 # NEEDED for modifying the LDAP
 # when not provided, anonymous bind is used
 # admin user should be fully qualified
 # admin_user = cn=admin,dc=cesga,dc=es
 # admin_password = adminpassword
 
 # set to true if tls is enabled; default: False
-# not supported yet
+# if set to true, the protocol will be ldaps://
+# if set to false, the protocol will be ldap://
 # tls = False
 
 # ldap base for user namespace; default: ou=users,dc=example
 # can include any number of ou / o / dc entries separated by commas
 # user_base = ou=users,dc=example
 
 # user entry attributes containing uids for mapping a user; defaults: gecos & uid
@@ -353,7 +368,14 @@
 ## UID range -- default 1000 -> 60000
 # uid_min = 1000
 # uid_max = 60000
 
 ## GID range -- default 1000 -> 60000
 # gid_min = 1000
 # gid_max = 60000
+
+## post_create_script -- default: None
+## A script to be executed after a user has been created
+# this script can be a shell script or a python script
+# and will be run with root privileges
+# the script will be called with the username as the first and only argument
+# post_create_script = /path/to/script.sh
```

### Comparing `feudalAdapter-0.5.4/ldf_adapter/__init__.py` & `feudalAdapter-0.6.0/ldf_adapter/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,17 +79,29 @@
                         )
                     os.chmod(filename, 0o0666)
                     # os.chmod(filename, stat.S_IREAD || stat.S_IWRITE ||stat.S_IRGRP || stat.S_IWGRP
                     #         || stat.S_IROTH || stat.S_IWOTH)
             except Exception as e:
                 logger.error(f"Got an exception in uncritical code: {e}")
 
+        hooks = {}
+        backend_config = CONFIG.backend.__getattribute__(CONFIG.ldf_adapter.backend)
+        if (
+            hasattr(backend_config, "post_create_script")
+            and backend_config.post_create_script
+        ):
+            hooks["post_create"] = backend_config.post_create_script
+        else:
+            logger.debug(
+                f"post_create_script not supported for backend {CONFIG.ldf_adapter.backend}"
+            )
+
         # Proceed as normal
         self.data = data if isinstance(data, UserInfo) else UserInfo(data)
-        self.service_user = backend.User(self.data)
+        self.service_user = backend.User(self.data, **hooks)
         self.service_groups = [backend.Group(grp) for grp in self.data.groups]
 
         # add additional groups from config
         self.additional_groups = [
             backend.Group(grp)
             for grp in CONFIG.ldf_adapter.additional_groups
             if grp not in self.data.groups
@@ -101,15 +113,17 @@
                 self.update_username_from_existing()
 
         if CONFIG.approval.enabled:
             # initialise pending deployment and notification system
             self.pending_deployment = PendingDeployment(userinfo=self.data)
 
         # apply fixes to group names for unix backend
-        if CONFIG.ldf_adapter.backend == "local_unix" and hasattr(backend.User, "fix_group_names"):
+        if CONFIG.ldf_adapter.backend == "local_unix" and hasattr(
+            backend.User, "fix_group_names"
+        ):
             for grp in self.service_groups + self.additional_groups:
                 grp.fix_group_names()
 
     def assurance_verifier(self):
         """Produce a suitably function to check if a user is allowed.
 
         Relevant config:
@@ -235,17 +249,21 @@
 
             logger.debug(f"User comes with these groups")
             for g in self.service_groups:
                 logger.debug(f"    {g.name}")
 
             return self.deploy()
         elif target == "not_deployed":
-            if not CONFIG.assurance.skip and not self.assurance_verifier()(self.data.assurance):
+            if not CONFIG.assurance.skip and not self.assurance_verifier()(
+                self.data.assurance
+            ):
                 if not CONFIG.assurance.verified_undeploy:
-                    logger.warning("Assurance level is insufficient. Undeploying anyway.")
+                    logger.warning(
+                        "Assurance level is insufficient. Undeploying anyway."
+                    )
                 else:
                     raise Rejection(
                         message="Your assurance level is insufficient to access this resource"
                     )
             return self.undeploy()
         elif target == "get_status":
             return self.get_status()
@@ -278,43 +296,51 @@
                 message="User deployment was rejected. No new deployment request will be sent.",
             )
 
         self.ensure_groups_exist()
         was_created = self.ensure_exists()
         new_memberships, removed_memberships = self.ensure_group_memberships()
         new_credentials = self.ensure_credentials_active()
+        if was_created:
+            self.service_user.execute("post_create", self.service_user.get_username())
 
         if CONFIG.approval.enabled:
             self.pending_deployment.notify()
             # if user existed
             if self.service_user.exists():
                 what_changed = "User already existed"
                 if new_memberships != [] or removed_memberships != []:
                     what_changed += ", but groups changed. A request for updating user groups was submitted for approval"
                 what_changed += "."
                 return Deployed(message=what_changed, credentials=self.credentials)
             # user is pending
             if was_created:
                 what_changed = "Request for deployment was submitted for approval."
             elif new_memberships != [] or removed_memberships != []:
-                what_changed = "Updated request for deployment was submitted for approval."
+                what_changed = (
+                    "Updated request for deployment was submitted for approval."
+                )
             else:
                 what_changed = "Request for deployment was already submitted for approval. No new request was sent."
             return Status(state="pending", message=what_changed)
         else:
             what_changed = "User was created" if was_created else "User already existed"
             if new_memberships != []:
-                what_changed += " and was added to groups {}".format(",".join(new_memberships))
+                what_changed += " and was added to groups {}".format(
+                    ",".join(new_memberships)
+                )
             if removed_memberships != []:
                 what_changed += " and was removed from groups {}".format(
                     ",".join(removed_memberships)
                 )
             what_changed += "."
             if new_credentials:
-                what_changed += " Credentials {} were activated.".format(",".join(new_credentials))
+                what_changed += " Credentials {} were activated.".format(
+                    ",".join(new_credentials)
+                )
 
             return Deployed(credentials=self.credentials, message=what_changed)
 
     def undeploy(self):
         """Ensure that the user dosen't exist.
 
         Return a NotDeployed result with a message saying if the user previously existed.
@@ -409,15 +435,18 @@
         return Status(state, message=what_changed)
 
     def accept(self):
         """Ensure that a pending request is accepted and the user is in state 'deployed'.
 
         Return a Status result with a message describing what was done.
         """
-        if self.pending_deployment.is_pending() or self.pending_deployment.mod_pending():
+        if (
+            self.pending_deployment.is_pending()
+            or self.pending_deployment.mod_pending()
+        ):
             if not hasattr(backend.User, "create_fromstring"):
                 raise Failure(
                     message=(
                         "Backend does not support automatic user creation from string."
                         "Follow the instructions in the notification you received to manually create the user."
                     )
                 )
@@ -432,30 +461,35 @@
                 raise Failure(
                     message=(
                         "Backend does not support automatic user modification from string."
                         "Follow the instructions in the notification you received to manually add the user to groups."
                     )
                 )
             self.pending_deployment.accept()
-            return Deployed(credentials=self.credentials, message="User request was accepted.")
+            return Deployed(
+                credentials=self.credentials, message="User request was accepted."
+            )
         elif self.pending_deployment.is_rejected():
             what_changed = "User request was already rejected, cannot accept it."
             logger.debug(what_changed)
             return Status(state="rejected", message=what_changed)
         else:
             what_changed = f"No pending request for user {self.data.unique_id} exists."
             logger.debug(what_changed)
             return Status(state=self.get_status().state, message=what_changed)
 
     def reject(self):
         """Ensure that a pending request is rejected and the user is in state 'not_deployed'.
 
         Return a Status result with a message describing what was done.
         """
-        if self.pending_deployment.is_pending() or self.pending_deployment.mod_pending():
+        if (
+            self.pending_deployment.is_pending()
+            or self.pending_deployment.mod_pending()
+        ):
             self.pending_deployment.reject()
             what_changed = "User deployment request was rejected."
             logger.debug(what_changed)
             return Status(state="rejected", message=what_changed)
         else:
             what_changed = f"No pending request for user {self.data.unique_id} exists."
             logger.debug(what_changed)
@@ -487,17 +521,21 @@
         """
 
         msg = "No message"
         try:
             if not self.service_user.exists():
                 if CONFIG.approval.enabled:
                     if self.pending_deployment.is_pending():
-                        return Status("pending", message="User deployment is pending approval.")
+                        return Status(
+                            "pending", message="User deployment is pending approval."
+                        )
                     if self.pending_deployment.is_rejected():
-                        return Status("rejected", message="User deployment was rejected.")
+                        return Status(
+                            "rejected", message="User deployment was rejected."
+                        )
                 return Status("not_deployed", message=msg)
             msg = f"username {self.service_user.get_username()}"
             if hasattr(self.service_user, "is_suspended"):
                 if self.service_user.is_suspended():
                     return Status("suspended", message=msg)
             if hasattr(self.service_user, "is_limited"):
                 if self.service_user.is_limited():
@@ -543,15 +581,17 @@
                         text=f'Username "{username}" already taken on this service. Please enter another one.',
                     )
 
             else:  # non-interactive
                 logger.debug("noninteractive mode")
                 username_mode = CONFIG.username_generator.mode
                 logger.debug(f"username_mode: {username_mode}")
-                pool_prefix = CONFIG.username_generator.pool_prefix or primary_group_name
+                pool_prefix = (
+                    CONFIG.username_generator.pool_prefix or primary_group_name
+                )
 
                 name_generator = NameGenerator(
                     username_mode, userinfo=self.data, pool_prefix=pool_prefix
                 )
                 proposed_name = name_generator.suggest_name()
                 logger.debug(f"initially proposed_name: {proposed_name}")
 
@@ -585,15 +625,17 @@
                 logger.error(message)
                 raise FatalError(message=message)
 
             if CONFIG.approval.enabled:
                 self.pending_deployment.create_user(self.service_user)
             else:
                 self.service_user.create()
-        elif CONFIG.approval.enabled and self.pending_deployment.exists():  # the user is pending
+        elif (
+            CONFIG.approval.enabled and self.pending_deployment.exists()
+        ):  # the user is pending
             username = self.pending_deployment.username
             self.service_user.set_username(username)
             logger.info(
                 f"Username {username} already assigned to '{self.data.unique_id}' in pending request."
             )
         else:  # The user exists
             # Update service_user.name if unique_id already points to a username:
@@ -610,15 +652,17 @@
         """Update self.service_user.name, if a user with matching
         unique_id can be found, and if the backend implements 'set_username'
         """
         try:
             existing_username = self.service_user.get_username()
             if existing_username is not None:
                 if hasattr(self.service_user, "set_username"):
-                    logger.debug(f"Setting username to {existing_username} ({self.data.unique_id})")
+                    logger.debug(
+                        f"Setting username to {existing_username} ({self.data.unique_id})"
+                    )
                     if hasattr(self.service_user, "set_prefixed_username"):
                         logger.debug("calling set_prefixed_username")
                         self.service_user.set_prefixed_username(existing_username)
                     else:
                         logger.debug("calling set_username")
                         self.service_user.set_username(existing_username)
                 logger.debug(f"Found an existing username: {existing_username}")
@@ -631,15 +675,17 @@
 
         Before deleting them, uninstall all SSH keys, to be sure that they are really gone.
 
         Return True, if the user existed before.
         """
         if self.service_user.exists():
             self.service_user.username = self.service_user.get_username()
-            logger.info(f"Deleting user '{self.service_user.username}' ({self.data.unique_id})")
+            logger.info(
+                f"Deleting user '{self.service_user.username}' ({self.data.unique_id})"
+            )
             # bwIDM requires prior removal of the user, because ssh-key removal triggers an
             # asyncronous process. If user is removed during that, the user might be only partially
             # removed...
             if CONFIG.ldf_adapter.backend == "bwidm":
                 self.service_user.delete()
                 self.service_user.uninstall_ssh_keys()
             else:
@@ -661,65 +707,78 @@
         Return True if the user has been suspended.
         """
         status = self.get_status()
         if status.state in ["deployed", "limited"]:
             if hasattr(self.service_user, "suspend"):
                 self.service_user.suspend()
                 return True
-        logger.debug(f"User {self.data.unique_id} in state {status.state}. Suspending not allowed.")
+        logger.debug(
+            f"User {self.data.unique_id} in state {status.state}. Suspending not allowed."
+        )
         return False
 
     def ensure_limited(self):
         """Ensure that a user has limited access.
         Return True if setting the user is limited.
         """
         status = self.get_status()
         if status.state == "deployed":
             if hasattr(self.service_user, "limit"):
                 self.service_user.limit()
                 return True
-        logger.debug(f"User {self.data.unique_id} in state {status.state}. Limiting not allowed.")
+        logger.debug(
+            f"User {self.data.unique_id} in state {status.state}. Limiting not allowed."
+        )
         return False
 
     def ensure_resumed(self):
         """Ensure that a user is resumed.
         Return True is the user
         """
         status = self.get_status()
         if status.state == "suspended":
             if hasattr(self.service_user, "resume"):
                 self.service_user.resume()
                 return True
-        logger.debug(f"User {self.data.unique_id} in state {status.state}. Resuming not allowed.")
+        logger.debug(
+            f"User {self.data.unique_id} in state {status.state}. Resuming not allowed."
+        )
         return False
 
     def ensure_unlimited(self):
         """Ensure that a user is not limited anymore.
         Return True is the user
         """
         status = self.get_status()
         if status.state == "limited":
             if hasattr(self.service_user, "unlimit"):
                 self.service_user.unlimit()
                 return True
-        logger.debug(f"User {self.data.unique_id} in state {status.state}. Unlimit not allowed.")
+        logger.debug(
+            f"User {self.data.unique_id} in state {status.state}. Unlimit not allowed."
+        )
         return False
 
     def ensure_groups_exist(self):
         """Ensure that all the necessary groups exist.
 
         Create the groups on the service, if necessary.
         Return the names of the groups that were created (or requested to be created).
         """
         group_list = self.service_groups + self.additional_groups
-        if self.data.primary_group not in self.data.groups + CONFIG.ldf_adapter.additional_groups:
+        if (
+            self.data.primary_group
+            not in self.data.groups + CONFIG.ldf_adapter.additional_groups
+        ):
             group_list.append(self.service_user.primary_group)
 
         new_groups = []
-        for group in filter(lambda grp: not grp.exists() and grp.name is not None, group_list):
+        for group in filter(
+            lambda grp: not grp.exists() and grp.name is not None, group_list
+        ):
             logger.info("Creating group '{}'".format(group.name))
             if CONFIG.approval.enabled:
                 if self.pending_deployment.create_group(group):
                     new_groups.append(group.name)
             else:
                 group.create()
                 new_groups.append(group.name)
@@ -731,15 +790,18 @@
         Return two lists:
         - the names of all groups the user was added to
         - the names of all groups the user was removed from
         """
         username = self.service_user.get_username()
 
         group_list = self.service_groups + self.additional_groups
-        if self.data.primary_group not in self.data.groups + CONFIG.ldf_adapter.additional_groups:
+        if (
+            self.data.primary_group
+            not in self.data.groups + CONFIG.ldf_adapter.additional_groups
+        ):
             group_list.append(self.service_user.primary_group)
 
         logger.info(
             f"Ensuring user '{username}' ({self.data.unique_id}) is member of these groups: "
             f"{[grp.name for grp in group_list]}"
         )
 
@@ -751,16 +813,20 @@
                 f"User '{username}' has to be added to the following groups: {groups_added}"
             )
             logger.info(
                 f"User '{username}' has to be removed from the following groups: {groups_removed}"
             )
             return groups_added, groups_removed
         else:
-            groups_added, groups_removed = self.service_user.mod(supplementary_groups=group_list)
-            logger.info(f"User '{username}' was added to the following groups: {groups_added}")
+            groups_added, groups_removed = self.service_user.mod(
+                supplementary_groups=group_list
+            )
+            logger.info(
+                f"User '{username}' was added to the following groups: {groups_added}"
+            )
             logger.info(
                 f"User '{username}' was removed from the following groups: {groups_removed}"
             )
             return groups_added, groups_removed
 
     def ensure_credentials_active(self):
         """Install all SSH Keys on the service.
```

### Comparing `feudalAdapter-0.5.4/ldf_adapter/approval/__init__.py` & `feudalAdapter-0.6.0/ldf_adapter/approval/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,18 @@
 
         self._user = self._pending_db.get_user(userinfo.unique_id)
         self._memberships = self._pending_db.get_memberships(userinfo.unique_id)
         if self._memberships:
             self._groups = list(
                 filter(
                     None,
-                    [self._pending_db.get_group(m) for m in self._memberships.supplementary_groups],
+                    [
+                        self._pending_db.get_group(m)
+                        for m in self._memberships.supplementary_groups
+                    ],
                 )
             )
         else:
             self._groups = []
 
     @property
     def user(self) -> Optional[PendingUser]:
@@ -146,15 +149,18 @@
     def create_group(self, group: backend.Group) -> bool:  # type: ignore
         """Create new pending group entry and add it to db.
         Return False if the entry already exists for this user in pending db.
         """
         if group.name in [g.name for g in self.groups]:
             return False
         pending_group = PendingGroup(
-            name=group.name, state=DeploymentState.PENDING, cmd=group.create_tostring(), infodict={}
+            name=group.name,
+            state=DeploymentState.PENDING,
+            cmd=group.create_tostring(),
+            infodict={},
         )
         self._pending_db.add_group(pending_group)
         self._groups.append(pending_group)
         return True
 
     def mod(
         self, service_user: backend.User, supplementary_groups: List[backend.Group]
@@ -184,15 +190,17 @@
         )
 
         if self._memberships is None:
             if groups_to_add != [] or groups_to_remove != []:
                 self._pending_db.add_memberships(memberships)
                 self._memberships = memberships
             return groups_to_add, groups_to_remove
-        elif set(self._memberships.supplementary_groups) != set(supplementary_groups_names):
+        elif set(self._memberships.supplementary_groups) != set(
+            supplementary_groups_names
+        ):
             self._pending_db.update_memberships(memberships)
             self._memberships = memberships
             return groups_to_add, groups_to_remove
         return [], []
 
     def remove_data(self):
         """Remove from pending db all data associated to this user."""
@@ -288,15 +296,17 @@
             "groups_cmd": groups_cmd,
             "memberships_cmd": memberships_cmd,
             "sub": self.sub,
             "iss": self.iss,
             "username": self.username,
         }
         try:
-            notified = self._notifier.notify(notification_type=admin_notification, data=data)
+            notified = self._notifier.notify(
+                notification_type=admin_notification, data=data
+            )
             if self.email:
                 self._notifier.notify(notification_type=user_notification, data=data)
             else:
                 logger.warning(
                     "No email found in deployment request: user will not receive email notification."
                 )
             if notified:
```

### Comparing `feudalAdapter-0.5.4/ldf_adapter/approval/db/generic.py` & `feudalAdapter-0.6.0/ldf_adapter/approval/db/generic.py`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.4/ldf_adapter/approval/db/sqlite.py` & `feudalAdapter-0.6.0/ldf_adapter/approval/db/sqlite.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,21 +33,29 @@
         except TypeError:
             return pytype.__name__
 
     type_name = get_type_name(pytype)
     module_name = pytype.__module__
     # types from typing module supported by sqlite
     if module_name == "typing":
-        if type_name.startswith("typing.Optional") or type_name.startswith("typing.Union"):
+        if type_name.startswith("typing.Optional") or type_name.startswith(
+            "typing.Union"
+        ):
             # Union only when it's used to represent an optional field
             # in python 3.7, __repr__() for the Optional type returns the Union representation
             # in python >= 3.9, __repr__() for a Union of a type and NoneType returns the Optional representation
-            if len(pytype.__args__) == 2 and get_type_name(pytype.__args__[0]) == "NoneType":
+            if (
+                len(pytype.__args__) == 2
+                and get_type_name(pytype.__args__[0]) == "NoneType"
+            ):
                 return pytype_to_sqltype(pytype.__args__[1])
-            elif len(pytype.__args__) == 2 and get_type_name(pytype.__args__[1]) == "NoneType":
+            elif (
+                len(pytype.__args__) == 2
+                and get_type_name(pytype.__args__[1]) == "NoneType"
+            ):
                 return pytype_to_sqltype(pytype.__args__[0])
             else:
                 return "text"
         elif type_name.startswith("typing.Literal"):
             return "text"
         elif type_name.startswith("typing.Dict"):
             return "dict"
@@ -95,15 +103,18 @@
         table_name (str): the table name
         primary_key (Union[str, List[str]]): name(s) of column(s) to be used as primary key
 
     Returns:
         str: a string representation of the sql command
     """
     columns_with_types = ", ".join(
-        [" ".join([field.name, pytype_to_sqltype(field.type)]) for field in fields(data_model)]
+        [
+            " ".join([field.name, pytype_to_sqltype(field.type)])
+            for field in fields(data_model)
+        ]
     )
     if isinstance(primary_key, List):
         primary_key = ", ".join(primary_key)
     return (
         f"create table if not exists {table_name}"
         f"({columns_with_types}, primary key ({primary_key}))"
     )
@@ -123,15 +134,17 @@
         str: a string representation of the sql command
     """
     column_names = ", ".join([field.name for field in fields(data_model)])
     column_values = ",".join(["?" for _ in fields(data_model)])
     return f"insert into {table_name}({column_names}) values ({column_values})"
 
 
-def sql_command_update(table_name: str, columns: List[str], key: Union[str, List[str]]) -> str:
+def sql_command_update(
+    table_name: str, columns: List[str], key: Union[str, List[str]]
+) -> str:
     """Return an sql command for updating a set of fields for an entry in a given table.
 
     The sql command will require the following arguments, in this order:
     - the new values for each column
     - the key value(s) of the entry to be updated
 
     Args:
@@ -139,15 +152,19 @@
         columns (list[str]): the columns to update
         key (list | str): the key to search on for update; a column name or a list of column names
 
     Returns:
         str: a string representation of the sql command
     """
     column_names = ", ".join([f"{col} = ?" for col in columns])
-    condition = " and ".join([f"{k} = ?" for k in key]) if isinstance(key, list) else f"{key} = ?"
+    condition = (
+        " and ".join([f"{k} = ?" for k in key])
+        if isinstance(key, list)
+        else f"{key} = ?"
+    )
     return f"update {table_name} set {column_names} where {condition}"
 
 
 def sql_command_remove(table_name: str, key: Union[str, List[str]]) -> str:
     """Return an sql command for removing an entry from a table.
 
     The sql command will require the following arguments:
@@ -156,15 +173,19 @@
     Args:
         table_name (str): the table name
         key (list | str): the key to search on for removal; a column name or a list of column names
 
     Returns:
         str: a string representation of the sql command
     """
-    condition = " and ".join([f"{k} = ?" for k in key]) if isinstance(key, list) else f"{key} = ?"
+    condition = (
+        " and ".join([f"{k} = ?" for k in key])
+        if isinstance(key, list)
+        else f"{key} = ?"
+    )
     return f"delete from {table_name} where {condition}"
 
 
 def sql_command_select(table_name: str, key: Union[str, List[str]]) -> str:
     """Return an sql command for selecting an entry from a table.
 
     The sql command will require the following arguments:
@@ -173,15 +194,19 @@
     Args:
         table_name (str): the table name
         key (list | str): the key to search on for selection; a column name or a list of column names
 
     Returns:
         str: a string representation of the sql command
     """
-    condition = " and ".join([f"{k} = ?" for k in key]) if isinstance(key, list) else f"{key} = ?"
+    condition = (
+        " and ".join([f"{k} = ?" for k in key])
+        if isinstance(key, list)
+        else f"{key} = ?"
+    )
     return f"select * from {table_name} where {condition}"
 
 
 # register the functions for manipulating custom types in sqlite db
 sqlite3.register_adapter(dict, lambda x: json.dumps(x).encode("utf-8"))
 sqlite3.register_converter("dict", lambda x: json.loads(x.decode("utf-8")))
 
@@ -206,45 +231,56 @@
         return Path(self.location).exists()
 
     def connect(self) -> None:
         """Connect to the DB.
         Initialise self.connection object.
         """
         try:
-            self.connection = sqlite3.connect(self.location, detect_types=sqlite3.PARSE_DECLTYPES)
+            self.connection = sqlite3.connect(
+                self.location, detect_types=sqlite3.PARSE_DECLTYPES
+            )
         except sqlite3.Error as ex:
-            message = f"Could not connect to sqlite db at location {self.location}: {ex}"
+            message = (
+                f"Could not connect to sqlite db at location {self.location}: {ex}"
+            )
             logger.error(message)
             raise FatalError(message=message)
 
     def create(
-        self, data_model: Type[PendingModel], table_name: str, primary_key: Union[str, List[str]]
+        self,
+        data_model: Type[PendingModel],
+        table_name: str,
+        primary_key: Union[str, List[str]],
     ) -> None:
         """Create a table for a given data model.
 
         Args:
             data_model (Type[PendingModel]): dataclass containing the fields that will become the table columns
             table_name (str): the table name
             primary_key (Union[str, List[str]]): name(s) of column(s) to be used as primary key
         """
         try:
             with self.connection:  # con.commit() is called automatically afterwards on success
                 logger.debug("Creating table: %s", table_name)
                 self.connection.execute(
                     sql_command_create_table(
-                        data_model=data_model, table_name=table_name, primary_key=primary_key
+                        data_model=data_model,
+                        table_name=table_name,
+                        primary_key=primary_key,
                     )
                 )
                 logger.debug("Successfully created table '%s'.", table_name)
         except sqlite3.Error as ex:
             message = f"Failed to create table {table_name}: {ex}"
             logger.error(message)
             raise FatalError(message=message)
 
-    def insert(self, data_model: Type[PendingModel], table_name: str, entry: tuple) -> bool:
+    def insert(
+        self, data_model: Type[PendingModel], table_name: str, entry: tuple
+    ) -> bool:
         """Insert an entry of a given data model into a table.
 
         Args:
             data_model (Type[PendingModel]): dataclass containing the fields that are the same as the table columns
             table_name (str): the table name
             entry (tuple): the values of the dataclass fields to be inserted
 
@@ -254,28 +290,34 @@
         try:
             with self.connection:
                 logger.debug("Inserting to table: %s", table_name)
                 self.connection.execute(
                     sql_command_insert(data_model=data_model, table_name=table_name),
                     entry,
                 )
-                logger.debug("Successfully inserted to table '%s': %s", table_name, entry)
+                logger.debug(
+                    "Successfully inserted to table '%s': %s", table_name, entry
+                )
             return True
         except sqlite3.IntegrityError as ex:
             if ex.args[0].startswith("UNIQUE constraint failed: "):
                 logger.info(f"Entry {entry} already exists in table {table_name}.")
                 return False
             raise ex
         except sqlite3.Error as ex:
             message = f"Failed to insert entry to table {table_name}: {ex}"
             logger.error(message)
             raise Failure(message=message)
 
     def update(
-        self, table_name: str, columns: List[str], key: Union[str, List[str]], entry: tuple
+        self,
+        table_name: str,
+        columns: List[str],
+        key: Union[str, List[str]],
+        entry: tuple,
     ) -> None:
         """Update an entry in a table.
 
         Args:
             table_name (str): the table name
             columns (list[str]): the columns to update
             key (str | list[str]): the key to search on for update
@@ -285,15 +327,17 @@
         try:
             with self.connection:
                 logger.debug("Updating entry in table: %s", table_name)
                 self.connection.execute(
                     sql_command_update(table_name=table_name, columns=columns, key=key),
                     entry,
                 )
-                logger.debug("Successfully updated entry in table '%s': %s", table_name, entry)
+                logger.debug(
+                    "Successfully updated entry in table '%s': %s", table_name, entry
+                )
         except sqlite3.Error as ex:
             message = f"Failed to update table {table_name}: {ex}"
             logger.error(message)
             raise Failure(message=message)
 
     def select(
         self,
@@ -316,41 +360,51 @@
         try:
             with self.connection:
                 logger.debug("Getting from table: %s", table_name)
                 result = self.connection.execute(
                     sql_command_select(table_name=table_name, key=key), value
                 ).fetchall()
                 logger.debug(
-                    "Successfully got entry from table '%s' for value %s.", table_name, value
+                    "Successfully got entry from table '%s' for value %s.",
+                    table_name,
+                    value,
                 )
                 if len(result) == 0:
                     return None
                 if len(result) > 1:
                     logger.warning(
-                        "Multiple entries found in table %s for value: %s", table_name, value
+                        "Multiple entries found in table %s for value: %s",
+                        table_name,
+                        value,
                     )
                 return data_model(*result[0])
         except sqlite3.Error as ex:
-            message = f"Failed to get entry from table {table_name} for value {value}: {ex}"
+            message = (
+                f"Failed to get entry from table {table_name} for value {value}: {ex}"
+            )
             logger.error(message)
             raise Failure(message=message)
 
     def delete(self, table_name: str, key: Union[str, List[str]], value: tuple) -> None:
         """Remove an entry from a table.
 
         Args:
             table_name (str): the table name
             key (Union[str, List[str]]): name(s) of column(s) to be used search key
             value (tuple): value(s) of key(s) for entry to be removed
         """
         try:
             with self.connection:
                 logger.debug("Removing from table: %s", table_name)
-                self.connection.execute(sql_command_remove(table_name=table_name, key=key), value)
-                logger.debug("Successfully removed entry %s from table '%s'.", value, table_name)
+                self.connection.execute(
+                    sql_command_remove(table_name=table_name, key=key), value
+                )
+                logger.debug(
+                    "Successfully removed entry %s from table '%s'.", value, table_name
+                )
         except sqlite3.Error as ex:
             message = f"Failed to remove entry {value} from table {table_name}: {ex}"
             logger.error(message)
             raise Failure(message=message)
 
 
 class PendingDB(generic.PendingDB):
@@ -358,18 +412,21 @@
 
     def __init__(self) -> None:
         """Initialise sqlite-based DB for managing users and groups pending approval."""
         self.connector = SQLiteConnector(CONFIG.approval.user_db_location)
         if not self.connector.exists():
             self.connector.connect()
             logger.debug(
-                "No sqlite DB found at %s, creating it...", CONFIG.approval.user_db_location
+                "No sqlite DB found at %s, creating it...",
+                CONFIG.approval.user_db_location,
             )
             self.connector.create(
-                data_model=PendingUser, table_name="pending_users", primary_key="unique_id"
+                data_model=PendingUser,
+                table_name="pending_users",
+                primary_key="unique_id",
             )
             self.connector.create(
                 data_model=PendingGroup, table_name="pending_groups", primary_key="name"
             )
             self.connector.create(
                 data_model=PendingMemberships,
                 table_name="pending_memberships",
@@ -388,15 +445,17 @@
             data_model=PendingUser,
             table_name="pending_users",
             entry=tuple(getattr(user, field.name) for field in fields(PendingUser)),
         )
 
     def remove_user(self, unique_id: str) -> None:
         """Remove user entry for unique_id."""
-        self.connector.delete(table_name="pending_users", key="unique_id", value=(unique_id,))
+        self.connector.delete(
+            table_name="pending_users", key="unique_id", value=(unique_id,)
+        )
 
     def get_user(self, unique_id: str) -> Optional[PendingUser]:
         """Get a user entry that is up for approval by the user's unique_id."""
         return self.connector.select(
             data_model=PendingUser,
             table_name="pending_users",
             key="unique_id",
@@ -441,15 +500,18 @@
     def remove_group(self, name: str) -> None:
         """Remove group entry for name."""
         self.connector.delete(table_name="pending_groups", key="name", value=(name,))
 
     def get_group(self, name: str) -> Optional[PendingGroup]:
         """Get an entry that is up for approval by the group's name."""
         return self.connector.select(
-            data_model=PendingGroup, table_name="pending_groups", key="name", value=(name,)
+            data_model=PendingGroup,
+            table_name="pending_groups",
+            key="name",
+            value=(name,),
         )
 
     def notify_group(self, name: str) -> None:
         """Change the state of group given by name to NOTIFIED."""
         self.connector.update(
             table_name="pending_groups",
             columns=["state"],
@@ -458,30 +520,40 @@
         )
 
     def add_memberships(self, membership: PendingMemberships) -> bool:
         """Add a new entry for a user's pending group memberships. Returns False if entry already exists."""
         return self.connector.insert(
             data_model=PendingMemberships,
             table_name="pending_memberships",
-            entry=tuple(getattr(membership, field.name) for field in fields(PendingMemberships)),
+            entry=tuple(
+                getattr(membership, field.name) for field in fields(PendingMemberships)
+            ),
         )
 
     def update_memberships(self, membership: PendingMemberships) -> None:
         """Update a user's pending group memberships by replacing them with the given memberships."""
-        columns = [field.name for field in fields(PendingMemberships) if field.name != "unique_id"]
+        columns = [
+            field.name
+            for field in fields(PendingMemberships)
+            if field.name != "unique_id"
+        ]
         self.connector.update(
             table_name="pending_memberships",
             columns=columns,
             key="unique_id",
-            entry=tuple([getattr(membership, col) for col in columns] + [membership.unique_id]),
+            entry=tuple(
+                [getattr(membership, col) for col in columns] + [membership.unique_id]
+            ),
         )
 
     def remove_memberships(self, unique_id: str) -> None:
         """Remove all pending group memberships of a given user."""
-        self.connector.delete(table_name="pending_memberships", key="unique_id", value=(unique_id,))
+        self.connector.delete(
+            table_name="pending_memberships", key="unique_id", value=(unique_id,)
+        )
 
     def get_memberships(self, unique_id: str) -> Optional[PendingMemberships]:
         """Get a given user's pending group memberships."""
         return self.connector.select(
             data_model=PendingMemberships,
             table_name="pending_memberships",
             key="unique_id",
```

### Comparing `feudalAdapter-0.5.4/ldf_adapter/approval/models.py` & `feudalAdapter-0.6.0/ldf_adapter/approval/models.py`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.4/ldf_adapter/backend/bwidm.py` & `feudalAdapter-0.6.0/ldf_adapter/backend/bwidm.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import requests
 import os
 from urllib.parse import urljoin
 
 from ldf_adapter.config import CONFIG
 from ldf_adapter import utils
 from ldf_adapter.logsetup import jsonlogger
+from ldf_adapter.backend import generic
 
 logger = logging.getLogger(__name__)
 
 
 class BwIdmConnection:
     """Connection to the BWIDM API."""
 
@@ -53,47 +54,55 @@
                          joined with '/'
         fail=True -- Raise exception on non-200 HTTP status
         **kwargs -- Passed to `requests.Request.__init__`
         """
         fail = kwargs.pop("fail", True)
 
         url_fragments = map(str, url_fragments)
-        url_fragments = map(lambda frag: requests.utils.quote(frag, safe=""), url_fragments)
+        url_fragments = map(
+            lambda frag: requests.utils.quote(frag, safe=""), url_fragments
+        )
         url = reduce(
-            lambda acc, frag: urljoin(acc, frag) if acc.endswith("/") else urljoin(acc + "/", frag),
+            lambda acc, frag: urljoin(acc, frag)
+            if acc.endswith("/")
+            else urljoin(acc + "/", frag),
             url_fragments,
             CONFIG.backend.bwidm.url,
         )
 
         # logger.debug(f"BWIDM: {url}")
         # logger.debug(f"BWIDM: {kwargs}")
         req = requests.Request(method, url, **kwargs)
         rsp = self.session.send(self.session.prepare_request(req))
 
         if fail:
             if not rsp.ok:
-                logger.error("Server responded with: {}".format(rsp.content.decode("utf-8")))
+                logger.error(
+                    "Server responded with: {}".format(rsp.content.decode("utf-8"))
+                )
             rsp.raise_for_status()
 
         return rsp
 
 
 BWIDM = BwIdmConnection(CONFIG)
 
 
-class User:
+class User(generic.User):
     ATTR_USERNAME = "urn:oid:0.9.2342.19200300.100.1.1"
     ATTR_ORG_ID = "http://bwidm.de/bwidmOrgId"
     VALUE_USER_ACTIVE = "ACTIVE"
     VALUE_USER_INACTIVE = "ON_HOLD"
 
-    def __init__(self, userinfo):
+    def __init__(self, userinfo, **hooks):
+        super().__init__(userinfo, **hooks)
         self.info = userinfo
         self.primary_group = Group(userinfo.primary_group)
         self.force_username = None
+        self.post_create_script = CONFIG.backend.bwidm.post_create_script
 
     def exists(self):
         """
         Inactive users ('ON_HOLD') are treated as nonexistent.
         """
         return self._exists() and self._is_active()
 
@@ -104,31 +113,37 @@
                 self.info.unique_id, "exists" if exists else "doesn't exist"
             )
         )
         return exists
 
     def _is_active(self):
         status = self.reg_info()["userStatus"]
-        logger.debug("User {} is {} on service BWIDM".format(self.info.unique_id, status))
+        logger.debug(
+            "User {} is {} on service BWIDM".format(self.info.unique_id, status)
+        )
         return status == self.VALUE_USER_ACTIVE
 
     def _is_registered(self):
         """
         find if the user is already registered for a given
         service, identified by its service short name
         """
         # FIXME: Consider putting this request into the global user object (to reduce load on regapp)
         ssn = CONFIG.backend.bwidm.service_name
-        registrations = BWIDM.get("external-reg", "find", "externalId", self.info.unique_id)
+        registrations = BWIDM.get(
+            "external-reg", "find", "externalId", self.info.unique_id
+        )
         # find registrations
         number_of_registrations = 0
         try:
             logger.debug("logging registrations to jsonlog")
             jsonlogger.debug(
-                json.dumps(registrations.json, sort_keys=True, indent=4, separators=(",", ": "))
+                json.dumps(
+                    registrations.json, sort_keys=True, indent=4, separators=(",", ": ")
+                )
             )
         except TypeError:
             pass
         for reg in registrations.json():
             if reg["serviceShortName"] == ssn:
                 if reg["registryStatus"] == "ACTIVE":
                     number_of_registrations += 1
@@ -145,42 +160,47 @@
         # TODO: argument "name" was added, check if given "name" (instead of info.username) is taken by *another* user
         logger.debug(f"checking for name taken of {name}")
         users_with_name = BWIDM.get(
             "external-user", "find", "attribute", self.ATTR_USERNAME, name
         ).json()
 
         other_users_with_name = [
-            user for user in users_with_name if user["externalId"] != self.info.unique_id
+            user
+            for user in users_with_name
+            if user["externalId"] != self.info.unique_id
         ]
         # logger.debug (F"other_users: {other_users_with_name}")
         logger.debug(f"Found {len(other_users_with_name)} with same username")
         # FIXME: Why < ?
         if len(other_users_with_name) < len(users_with_name):
             logger.debug("Username '{}' is reserved for us".format(self.info.username))
 
         if other_users_with_name:
             logger.error(
                 "Username '{}' is already used by\n    {}".format(
                     self.info.username,
-                    ",\n    ".join(map(lambda u: u["externalId"], other_users_with_name)),
+                    ",\n    ".join(
+                        map(lambda u: u["externalId"], other_users_with_name)
+                    ),
                 )
             )
         else:
             logger.debug("Username '{}' is available".format(name))
 
         return bool(other_users_with_name)
 
     def get_username(self):
         """Check if a user exists based on unique_id and return the name"""
 
         def safe_resp_conversion(resp):
             """Safely convert a response to json"""
             if resp.status_code != 200:
                 logger.debug(
-                    "Error %d reading from remote: \n%s\n" % (resp.status_code, str(resp.text))
+                    "Error %d reading from remote: \n%s\n"
+                    % (resp.status_code, str(resp.text))
                 )
                 os._exit(1)  # or raise or return None?
             try:
                 resp_json = resp.json()
             except json.JSONDecodeError:
                 logging.error("Could not decode json that I obtained from rest server")
                 raise
@@ -196,15 +216,17 @@
             bwIdmOrgId = resp_json["attributeStore"]["http://bwidm.de/bwidmOrgId"]
             logger.debug(f"retuning username: {bwIdmOrgId}_{username}")
             return f"{bwIdmOrgId}_{username}"
         except KeyError as e:
             logger.error("Error: I could not find the username in the database.")
             logger.error("  Most likely the user is not registered for this service\n")
             logger.error(f"  {e}")
-            logger.error(json.dumps(resp_json, sort_keys=True, indent=4, separators=(",", ": ")))
+            logger.error(
+                json.dumps(resp_json, sort_keys=True, indent=4, separators=(",", ": "))
+            )
         return None
 
     def set_username(self, username):
         """Update the internal representation of the user with the incoming username"""
         logger.debug(f"set_username: setting {username}")
         self.force_username = username
 
@@ -217,24 +239,28 @@
     def create(self):
         """Create or activate user."""
         if self._exists() and not self._is_active():
             logger.info("Activating user {unique_id}".format(**self.info))
             BWIDM.get("external-user", "activate", "externalId", self.info.unique_id)
         else:
             logger.info("Creating user {unique_id}".format(**self.info))
-            BWIDM.post("external-user", "create", json={"externalId": self.info.unique_id})
+            BWIDM.post(
+                "external-user", "create", json={"externalId": self.info.unique_id}
+            )
 
     def register(self):
         """register user for the configured service"""
 
         def get_active_reg_info(ext_id):
             rsp = BWIDM.get("external-reg", "find", "externalId", ext_id)
 
             try:
-                return next(filter(lambda reg: reg["registryStatus"] == "ACTIVE", rsp.json()))
+                return next(
+                    filter(lambda reg: reg["registryStatus"] == "ACTIVE", rsp.json())
+                )
             except StopIteration:
                 return {"lastReconcile": None}
 
         old_reg = get_active_reg_info(self.info.unique_id)
         # We wait until the 'lastReconciled' timestamp changes, which means that our update was sucessfully deployed
         reg = old_reg
         while reg["lastReconcile"] == old_reg["lastReconcile"]:
@@ -318,20 +344,24 @@
             # NL = "\n    "
             # logger.debug(
             #     f"Incoming groups: {NL}{NL.join([g['name'] for g in new_groups])}"
             # )
 
             # Remove user from groups he should not be a member of
             to_be_removed_from = [
-                g for g in current_groups if g["id"] not in (ng["id"] for ng in new_groups)
+                g
+                for g in current_groups
+                if g["id"] not in (ng["id"] for ng in new_groups)
             ]
 
             # Only add user to groups she is not already a member of
             to_be_added_to = [
-                g for g in new_groups if g["id"] not in (cg["id"] for cg in current_groups)
+                g
+                for g in new_groups
+                if g["id"] not in (cg["id"] for cg in current_groups)
             ]
 
             if to_be_removed_from:
                 logger.info(
                     "Remove user {} from groups {}".format(
                         self.info.username,
                         ",".join(g["name"] for g in to_be_removed_from),
@@ -400,15 +430,17 @@
         {..., k: val={...}, ...} means `state[k]=merge state[k] with val`
 
         This is applied recursivly.
 
         """
         current_state = self.reg_info()
         new_state = utils.dictmerge(current_state, state_updates)
-        utils.log_dictdiff(utils.dictdiff(current_state, new_state), log_function=logger.info)
+        utils.log_dictdiff(
+            utils.dictdiff(current_state, new_state), log_function=logger.info
+        )
         try:
             logger.debug(
                 f"current_state: {current_state['attributeStore']['urn:oid:0.9.2342.19200300.100.1.1']}"
             )
 
             logger.debug(
                 f"new_state:     {new_state['attributeStore']['urn:oid:0.9.2342.19200300.100.1.1']}    "
@@ -434,46 +466,54 @@
             formatted_json = json.dumps(
                 current_state, sort_keys=True, indent=4, separators=(",", ": ")
             )
             logger.debug("  logging current_state_updates to jsonlog")
             jsonlogger.debug(f"current_state: {formatted_json}")
 
             logger.debug("  logging new_to jsonlog")
-            formatted_json = json.dumps(new_state, sort_keys=True, indent=4, separators=(",", ": "))
+            formatted_json = json.dumps(
+                new_state, sort_keys=True, indent=4, separators=(",", ": ")
+            )
             jsonlogger.debug(f"new state for regapp:  {formatted_json}")
         except:
             pass
         BWIDM.post("external-user", "update", json=new_state)
 
     def reg_info(self, json=True, **kwargs):
         # FIXME: Cache this functions results!
-        rsp = BWIDM.get("external-user", "find", "externalId", self.info.unique_id, **kwargs)
+        rsp = BWIDM.get(
+            "external-user", "find", "externalId", self.info.unique_id, **kwargs
+        )
         return rsp.json() if json else rsp.content
 
 
-class Group:
+class Group(generic.Group):
     def __init__(self, name):
         self.name = name
 
     def exists(self):
         # FIXME: Group existence needs to be checked with using also
         # CONFIG.backend.bwidm.service_name
         return (
             b"no such group"
-            not in BWIDM.get("group-admin", "find", "name", self.name, fail=False).content
+            not in BWIDM.get(
+                "group-admin", "find", "name", self.name, fail=False
+            ).content
         )
 
     def create(self):
         rsp = BWIDM.get(
             "group-admin", "create", CONFIG.backend.bwidm.service_name, self.name
         ).json()
 
         if self.name != rsp["name"]:
             logger.warning(
-                "Groupname changed from {} to {} by BWIDM".format(self.name, rsp["name"])
+                "Groupname changed from {} to {} by BWIDM".format(
+                    self.name, rsp["name"]
+                )
             )
             self.name = rsp["name"]
 
         self.id = rsp["id"]
 
     def delete(self):
         # groupdel
```

### Comparing `feudalAdapter-0.5.4/ldf_adapter/backend/generic.py` & `feudalAdapter-0.6.0/ldf_adapter/backend/generic.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """Generic backend User and Group, to be implemented by all backends."""
 from abc import ABC, abstractmethod
+from ldf_adapter.backend.hooks import Hooks
 
 
-class User(ABC):
+class User(ABC, Hooks):
     """Manages the user object on the service."""
 
-    def __init__(self, userinfo):
+    def __init__(self, userinfo, **hooks):
         """
         Arguments:
         userinfo -- (type: UserInfo)
         """
-        pass
+        super().__init__(**hooks)
 
     @abstractmethod
     def exists(self):
         """Return whether the user exists on the service.
 
         If this returns True,  calling `create` should have no effect or raise an error.
         """
@@ -151,45 +152,39 @@
         pass
 
     @abstractmethod
     def get_primary_group(self):
         """Check if a user exists based on unique_id and return the primary group name."""
         pass
 
-    @abstractmethod
     def is_suspended(self):
         """Optional, only if the backend supports it.
         Return whether the user was suspended (e.g. due to a security incident)"""
         return False
 
-    @abstractmethod
     def is_limited(self):
         """Optional, only if the backend supports it.
         Return whether the user has limited access"""
         return False
 
-    @abstractmethod
     def suspend(self):
         """Optional, only if the backend supports it.
         Suspends the user such that no access to the service is possible"""
         pass
 
-    @abstractmethod
     def resume(self):
         """Optional, only if the backend supports it.
         Restores the suspended user"""
         pass
 
-    @abstractmethod
     def limit(self):
         """Optional, only if the backend supports it.
         Limits the user's capabilities on the service (e.g. read-only access)"""
         pass
 
-    @abstractmethod
     def unlimit(self):
         """Optional, only if the backend supports it.
         Restores a user with limited access to full capabilities"""
         pass
 
 
 class Group(ABC):
```

### Comparing `feudalAdapter-0.5.4/ldf_adapter/backend/ldap.py` & `feudalAdapter-0.6.0/ldf_adapter/backend/ldap.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     SAFE_SYNC,
     LDIF,
 )
 from enum import Enum, auto
 
 from ldf_adapter.config import CONFIG
 from ldf_adapter.results import Failure, Rejection, FatalError
-
+from ldf_adapter.backend import generic
 
 logger = logging.getLogger(__name__)
 
 
 class Mode(Enum):
     READ_ONLY = auto()
     PRE_CREATED = auto()
@@ -131,18 +131,22 @@
         self.uid_max = CONFIG.backend.ldap.uid_max
         self.gid_min = CONFIG.backend.ldap.gid_min
         self.gid_max = CONFIG.backend.ldap.gid_max
 
         # initialise connection used to generate LDIFs
         self.ldif_connection = Connection(server=None, client_strategy=LDIF)
         self.ldif_connection.bind()
+        self.protocol = "ldap"
+        if CONFIG.backend.ldap.tls:
+            self.protocol = "ldaps"
         # initialise and bind connection to LDAP server
         try:
             server = Server(
-                f"ldap://{CONFIG.backend.ldap.host}:{CONFIG.backend.ldap.port}", get_info=ALL
+                f"{self.protocol}://{CONFIG.backend.ldap.host}:{CONFIG.backend.ldap.port}",
+                get_info=ALL,
             )
             if CONFIG.backend.ldap.admin_user and CONFIG.backend.ldap.admin_password:
                 # add SAFE_SYNC, so we get more return values
                 self.connection = Connection(
                     server,
                     CONFIG.backend.ldap.admin_user,
                     CONFIG.backend.ldap.admin_password,
@@ -150,15 +154,15 @@
                     auto_bind=AUTO_BIND_NO_TLS,
                 )
             else:
                 self.connection = Connection(
                     server, client_strategy=SAFE_SYNC, auto_bind=AUTO_BIND_NO_TLS
                 )
         except Exception as e:
-            msg = f"Could not connect to server ldap://{CONFIG.backend.ldap.host}:{CONFIG.backend.ldap.port}/"
+            msg = f"Could not connect to server {self.protocol}://{CONFIG.backend.ldap.host}:{CONFIG.backend.ldap.port}/"
             logger.error(f"{msg}: {e}")
             raise Failure(message=msg)
 
     def init_nextuidgid(self):
         """Initialise uidNext and gidNext entries in FULL_ACCESS mode
         with values starting in configured range.
         """
@@ -186,15 +190,17 @@
                     )
                     search_gid = self.search_next_gid()
                 else:
                     logger.info(
                         f"gidNext already initialised: {search_gid.get_attribute('gidNumber')}."
                     )
         except Exception as e:
-            msg = "Error adding entries in LDAP for tracking available UID and GID values"
+            msg = (
+                "Error adding entries in LDAP for tracking available UID and GID values"
+            )
             logger.error(f"{msg}: {e}")
             raise Failure(message=msg)
 
     def search_user_by_oidc_uid(self, oidc_uid, attributes=[]):
         return LdapSearchResult(
             self.connection,
             [
@@ -451,15 +457,17 @@
     def update_user(self, userinfo, local_username):
         """Update the LDAP entry for given `local_username` with
         all information in `userinfo`.
         If user doesn't exist, nothing happens.
         """
         try:
             changes = {
-                "homeDirectory": [(MODIFY_REPLACE, [f"{self.home_base}/{local_username}"])],
+                "homeDirectory": [
+                    (MODIFY_REPLACE, [f"{self.home_base}/{local_username}"])
+                ],
                 "loginShell": [(MODIFY_REPLACE, [self.shell])],
                 self.attr_local_uid: [(MODIFY_REPLACE, [local_username])],
                 self.attr_oidc_uid: [(MODIFY_REPLACE, [userinfo.unique_id])],
             }
             if userinfo.family_name is not None:
                 changes["sn"] = [(MODIFY_REPLACE, [userinfo.family_name])]
             if userinfo.given_name is not None:
@@ -480,15 +488,17 @@
     def delete_user(self, local_username):
         """Delete the LDAP entry for given `local_username`.
         If user doesn't exist, no failure is raised.
         """
         try:
             return self.connection.delete(f"uid={local_username},{self.user_base}")
         except Exception as e:
-            msg = f"Failed to delete the LDAP entry for local username {local_username}."
+            msg = (
+                f"Failed to delete the LDAP entry for local username {local_username}."
+            )
             logger.error(f"{msg}: {e}")
             raise Failure(message=msg)
 
     def add_user_to_group(self, local_username, group_name):
         """Add a user to group.
         If either of them does not exist, a Failure exception is raised.
         """
@@ -596,22 +606,23 @@
         ldap.init_nextuidgid()
         return ldap
 
 
 LDAP = LdapConnection.load()
 
 
-class User:
+class User(generic.User):
     """Manages the user object on the service."""
 
-    def __init__(self, userinfo):
+    def __init__(self, userinfo, **hooks):
         """
         Arguments:
         userinfo -- (type: UserInfo)
         """
+        super().__init__(userinfo, **hooks)
         self.userinfo = userinfo
         self.unique_id = userinfo.unique_id
         logger.debug(f"backend processing: {userinfo.unique_id}")
         if self.exists():
             username = self.get_username()
             primary_group = self.get_primary_group()
             logger.debug(
@@ -620,14 +631,15 @@
             self.set_username(username)
             self.primary_group = Group(primary_group)
         else:
             self.set_username(userinfo.username)
             self.primary_group = Group(userinfo.primary_group)
 
         self.ssh_keys = [key["value"] for key in userinfo.ssh_keys]
+        self.post_create_script = CONFIG.backend.ldap.post_create_script
 
     def exists(self):
         """Return whether the user exists on the service.
 
         If this returns True,  calling `create` should have no effect or raise an error.
         """
         logger.info(f"Check if user exists: {self.unique_id}")
@@ -640,15 +652,17 @@
         In 'pre_created' mode, taken means that the username has been mapped to another oidc uid.
         """
         search_result = LDAP.search_user_by_local_username(name, get_unique_id=True)
         if search_result.found():  # there is an entry for name in LDAP
             oidc_uid = search_result.get_attribute(
                 LDAP.attr_oidc_uid
             )  # this is the oidc_uid mapped to name
-            if LDAP.mode == Mode.PRE_CREATED and oidc_uid is None:  # pre-created but not mapped
+            if (
+                LDAP.mode == Mode.PRE_CREATED and oidc_uid is None
+            ):  # pre-created but not mapped
                 return False
             return oidc_uid != self.unique_id  # name already mapped to another oidc uid
         else:  # no entry for name found in LDAP
             return False
 
     def get_username(self):
         """Check if a user exists based on unique_id and return the name"""
@@ -658,17 +672,17 @@
 
     def set_username(self, username):
         """Set local username on the service."""
         self.name = username
 
     def get_primary_group(self):
         """Check if a user exists based on unique_id and return the primary group name."""
-        gid = LDAP.search_user_by_oidc_uid(self.unique_id, attributes=["gidNumber"]).get_attribute(
-            "gidNumber"
-        )
+        gid = LDAP.search_user_by_oidc_uid(
+            self.unique_id, attributes=["gidNumber"]
+        ).get_attribute("gidNumber")
         return LDAP.search_group_by_gid(gid).get_attribute("cn")
 
     def get_groups(self):
         """Get a list of names of all service groups that the user belongs to.
 
         If the user doesn't exist, return an empty list.
         """
@@ -689,15 +703,17 @@
                 f" (local username {self.name})"
             )
             logger.error(msg)
             raise Rejection(
                 message=f"{msg} Please contact an administrator to create an account for you."
             )
         elif LDAP.mode == Mode.PRE_CREATED:
-            if not LDAP.search_user_by_local_username(self.name, get_unique_id=False).found():
+            if not LDAP.search_user_by_local_username(
+                self.name, get_unique_id=False
+            ).found():
                 msg = f"Local username {self.name} not found in LDAP for user {self.unique_id}."
                 logger.error(msg)
                 raise Rejection(
                     message=f"{msg} Please contact an administrator to pre-create this account for you."
                 )
             else:
                 # we assume that it was checked via name_taken that the username is not already mapped
@@ -707,15 +723,17 @@
 
     def create_tostring(self):
         """Return command (LDIF) for creating user in LDAP.
         If in pre_created mode and a local username exists, only map the user to it.
         """
         if (
             LDAP.mode == Mode.PRE_CREATED
-            and LDAP.search_user_by_local_username(self.name, get_unique_id=False).found()
+            and LDAP.search_user_by_local_username(
+                self.name, get_unique_id=False
+            ).found()
         ):
             return LDAP.map_user_ldif(self.userinfo, self.name)
         return LDAP.add_user_ldif(self.userinfo, self.name, self.primary_group.name)
 
     def update(self):
         """Update all relevant information about the user on the service.
 
@@ -859,15 +877,15 @@
 
         If the user doesn't exists, behaviour is undefined.
         """
         # TODO: use ldapPublicKey schema (sshPublicKey attribute) for storing ssh key in LDAP
         pass
 
 
-class Group:
+class Group(generic.Group):
     """Manages the group object on the service."""
 
     def __init__(self, name):
         """
         Arguments:
         name -- The name of the group
         """
@@ -887,17 +905,15 @@
         """Create the group on the service.
 
         If the group already exists, nothing happens.
         """
         if self.exists():
             logger.info(f"Group {self.name} exists.")
         elif LDAP.mode == Mode.READ_ONLY:
-            msg = (
-                f"LDAP backend in read_only mode, new entry cannot be added for group {self.name}."
-            )
+            msg = f"LDAP backend in read_only mode, new entry cannot be added for group {self.name}."
             logger.warning(msg)
         elif LDAP.mode == Mode.PRE_CREATED:
             msg = f"LDAP backend in pre_created mode, new entry cannot be added for group {self.name}."
             logger.warning(msg)
         else:  # Mode.FULL_ACCESS
             LDAP.add_group(self.name)
```

### Comparing `feudalAdapter-0.5.4/ldf_adapter/backend/local_unix.py` & `feudalAdapter-0.6.0/ldf_adapter/backend/local_unix.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,27 +22,30 @@
 from ldf_adapter.results import Failure
 from ldf_adapter.backend import generic
 
 logger = logging.getLogger(__name__)
 
 
 class User(generic.User):
-    def __init__(self, userinfo):
+    def __init__(self, userinfo, **hooks):
         """
         Arguments:
         userinfo -- Only these attributes are used:
                 `username` (which is passed through `make_shadow_compatible`),
                 `primary_group`
                 `unique_id`  stored in gecos, used to find the user
                 `ssh_keys`
         """
+        super().__init__(userinfo, **hooks)
         self.unique_id = userinfo.unique_id
         logger.debug(f"backend processing: {userinfo.unique_id}")
         if self.exists():
-            logger.debug(f"This user does actually exist. The name is: {self.get_username()}")
+            logger.debug(
+                f"This user does actually exist. The name is: {self.get_username()}"
+            )
             self.set_username(self.get_username())
         else:
             self.set_username(userinfo.username)
 
         # should be Group(self.get_primary_group()) when user exists?
         self.primary_group = Group(userinfo.primary_group)
         self.ssh_keys = [key["value"] for key in userinfo.ssh_keys]
@@ -58,30 +61,35 @@
         return bool(
             self.unique_id
             in [entry["gecos"] for entry in User.__all_passwd_entries("gecos").values()]
         )
 
     def is_suspended(self):
         """Optional, only if the backend supports it.
-        Inform the user whether a user was suspended (e.g. due to a security incident)"""
+        Inform the user whether a user was suspended (e.g. due to a security incident)
+        """
         if self.exists():
             options = ["-l"]
             try:
                 result = subprocess.run(
                     ["chage"] + options + [self.name],
                     stdout=subprocess.PIPE,
                     stderr=subprocess.PIPE,
                     check=True,
                 )
             except CalledProcessError as e:
                 msg = (e.stderr or e.stdout or b"").decode("utf-8").strip()
                 logger.error(
-                    "Error executing '{}': {}".format(" ".join(e.cmd), msg or "<no output>")
+                    "Error executing '{}': {}".format(
+                        " ".join(e.cmd), msg or "<no output>"
+                    )
+                )
+                raise Failure(
+                    message=f"Cannot get info for user: {msg or '<no output>'}"
                 )
-                raise Failure(message=f"Cannot get info for user: {msg or '<no output>'}")
             try:
                 pattern = regex.compile(r"Account expires\s+: (.*)")
                 match = pattern.search(result.stdout.decode("utf-8"))
                 if match:
                     expiration_date = match.group(1)
                     if expiration_date == "never":
                         return False
@@ -104,15 +112,17 @@
             return shell in ["/sbin/nologin", "/usr/bin/nologin", "/bin/nologin"]
         except KeyError:
             return False
 
     def name_taken(self, name):
         """Check if a username is already taken by *another* user"""
         name = make_shadow_compatible(name)
-        taken = name in [entry["login"] for entry in User.__all_passwd_entries("login").values()]
+        taken = name in [
+            entry["login"] for entry in User.__all_passwd_entries("login").values()
+        ]
         logger.debug(f"name_taken: {taken}")
         return taken and name != self.get_username()
 
     def get_username(self):
         """Return username based on unique_id"""
         try:
             return User.__all_passwd_entries("gecos")[self.unique_id]["login"]
@@ -149,61 +159,75 @@
                 self._create_cmd(),
                 stdout=subprocess.PIPE,
                 stderr=subprocess.PIPE,
                 check=True,
             )
         except CalledProcessError as e:
             msg = (e.stderr or e.stdout or b"").decode("utf-8").strip()
-            logger.error("Error executing '{}': {}".format(" ".join(e.cmd), msg or "<no output>"))
+            logger.error(
+                "Error executing '{}': {}".format(" ".join(e.cmd), msg or "<no output>")
+            )
             raise Failure(message=f"Cannot create user ({msg or '<no output>'})")
 
     def create_tostring(self):
         return " ".join(self._create_cmd())
 
     @staticmethod
     def create_fromstring(create_cmd):
         # some sanity checks
         if not create_cmd.startswith("useradd"):
             raise Failure(
                 message=f"Cannot create user (command is not applicable to this backend): {create_cmd}"
             )
         try:
             subprocess.run(
-                create_cmd.split(" "), stdout=subprocess.PIPE, stderr=subprocess.PIPE, check=True
+                create_cmd.split(" "),
+                stdout=subprocess.PIPE,
+                stderr=subprocess.PIPE,
+                check=True,
             )
         except CalledProcessError as e:
             msg = (e.stderr or e.stdout or b"").decode("utf-8").strip()
-            logger.error("Error executing '{}': {}".format(" ".join(e.cmd), msg or "<no output>"))
+            logger.error(
+                "Error executing '{}': {}".format(" ".join(e.cmd), msg or "<no output>")
+            )
             raise Failure(message=f"Cannot create user ({msg or '<no output>'})")
 
     def update(self):
         pass
 
     def delete(self):
         if not self.exists():
-            raise Failure(message=f"Cannot delete user: no user found for {self.unique_id}.")
+            raise Failure(
+                message=f"Cannot delete user: no user found for {self.unique_id}."
+            )
 
         name = self.__passwd_entry["login"]
 
         try:
             subprocess.run(
                 ["/usr/bin/pkill", "-u", name],
                 stdout=subprocess.PIPE,
                 stderr=subprocess.PIPE,
                 check=True,
             )
         except CalledProcessError:
             pass
         try:
             subprocess.run(
-                ["userdel", name], stdout=subprocess.PIPE, stderr=subprocess.PIPE, check=True
+                ["userdel", name],
+                stdout=subprocess.PIPE,
+                stderr=subprocess.PIPE,
+                check=True,
             )
         except CalledProcessError as e:
             msg = (e.stderr or e.stdout or b"").decode("utf-8").strip()
-            logger.error("Error executing '{}': {}".format(" ".join(e.cmd), msg or "<no output>"))
+            logger.error(
+                "Error executing '{}': {}".format(" ".join(e.cmd), msg or "<no output>")
+            )
             raise Failure(message=f"Cannot delete user: {msg or '<no output>'}")
 
     def _mod_cmd(self, supplementary_groups=None):
         """Create command to modify unix user with given groups.
 
         The user's current groups are merged with the given additional groups,
         and the removal_groups are removed from the list, to generate a list of groups
@@ -248,65 +272,81 @@
             )
             groups_after = self.get_groups()
             groups_added = list(set(groups_after) - set(group_before))
             groups_removed = list(set(group_before) - set(groups_after))
             return groups_added, groups_removed
         except CalledProcessError as e:
             msg = (e.stderr or e.stdout or b"").decode("utf-8").strip()
-            logger.error("Error executing '{}': {}".format(" ".join(e.cmd), msg or "<no output>"))
+            logger.error(
+                "Error executing '{}': {}".format(" ".join(e.cmd), msg or "<no output>")
+            )
             raise Failure(message=f"Cannot modify user: {msg or '<no output>'}")
 
     def mod_tostring(self, supplementary_groups=None):
         return " ".join(self._mod_cmd(supplementary_groups=supplementary_groups))
 
     @staticmethod
     def mod_fromstring(mod_cmd):
         # some sanity checks
         if not mod_cmd.startswith("usermod"):
             raise Failure(
                 message=f"Cannot modify user (command is not applicable to this backend): {mod_cmd}"
             )
         try:
             subprocess.run(
-                mod_cmd.split(" "), stdout=subprocess.PIPE, stderr=subprocess.PIPE, check=True
+                mod_cmd.split(" "),
+                stdout=subprocess.PIPE,
+                stderr=subprocess.PIPE,
+                check=True,
             )
         except CalledProcessError as e:
             msg = (e.stderr or e.stdout or b"").decode("utf-8").strip()
-            logger.error("Error executing '{}': {}".format(" ".join(e.cmd), msg or "<no output>"))
+            logger.error(
+                "Error executing '{}': {}".format(" ".join(e.cmd), msg or "<no output>")
+            )
             raise Failure(message=f"Cannot create user ({msg or '<no output>'})")
 
     def get_groups(self):
         """Get a list of names of all service groups that the user belongs to.
 
         If the user doesn't exist, return an empty list.
         """
         try:
             result = subprocess.run(
-                ["id", "-Gn", self.name], stdout=subprocess.PIPE, stderr=subprocess.PIPE, check=True
+                ["id", "-Gn", self.name],
+                stdout=subprocess.PIPE,
+                stderr=subprocess.PIPE,
+                check=True,
             )
             return result.stdout.decode("utf-8").strip().split()
         except CalledProcessError as e:
             msg = (e.stderr or e.stdout or b"").decode("utf-8").strip()
-            logger.warning("Error executing '{}': {}".format(" ".join(e.cmd), msg or "<no output>"))
+            logger.warning(
+                "Error executing '{}': {}".format(" ".join(e.cmd), msg or "<no output>")
+            )
             logger.info("Returning empty group list for user %s", self.name)
             return []
 
     def __expire(self, expiration_date=datetime.today().strftime("%Y-%m-%d")):
         options = ["-E", expiration_date]
         try:
             subprocess.run(
                 ["chage"] + options + [self.name],
                 stdout=subprocess.PIPE,
                 stderr=subprocess.PIPE,
                 check=True,
             )
         except CalledProcessError as e:
             msg = (e.stderr or e.stdout or b"").decode("utf-8").strip()
-            logger.error("Error executing '{}': {}".format(" ".join(e.cmd), msg or "<no output>"))
-            raise Failure(message=f"Cannot set expiration date for user: {msg or '<no output>'}")
+            logger.error(
+                "Error executing '{}': {}".format(" ".join(e.cmd), msg or "<no output>")
+            )
+            raise Failure(
+                message=f"Cannot set expiration date for user: {msg or '<no output>'}"
+            )
 
     def suspend(self):
         self.__expire(datetime.today().strftime("%Y-%m-%d"))
 
     def resume(self):
         self.__expire("-1")
 
@@ -316,15 +356,17 @@
                 ["usermod", "-s", shell, self.name],
                 stdout=subprocess.PIPE,
                 stderr=subprocess.PIPE,
                 check=True,
             )
         except CalledProcessError as e:
             msg = (e.stderr or e.stdout or b"").decode("utf-8").strip()
-            logger.error("Error executing '{}': {}".format(" ".join(e.cmd), msg or "<no output>"))
+            logger.error(
+                "Error executing '{}': {}".format(" ".join(e.cmd), msg or "<no output>")
+            )
             raise Failure(message=f"Cannot modify user: {msg or '<no output>'}")
 
     def limit(self):
         self.__set_shell("/sbin/nologin")  # or /usr/sbin/nologin ?
 
     def unlimit(self):
         self.__set_shell(CONFIG.backend.local_unix.shell)
@@ -342,15 +384,17 @@
                     self.__authorized_keys.chmod(0o600)
                     chown(self.__authorized_keys, self.__uid, self.__gid)
         except IOError as e:
             logger.error(e)
             raise Failure(message=f"Could not write new ssh keys: {e or '<no output>'}")
         except Exception as e:
             logger.error(e)
-            raise Failure(message=f"Cannot change owner or permissions: {e or '<no output>'}")
+            raise Failure(
+                message=f"Cannot change owner or permissions: {e or '<no output>'}"
+            )
 
     def uninstall_ssh_keys(self):
         """Remove any SSH keys stored in the users .authorized_keys file."""
         try:
             self.__authorized_keys.unlink()
         except FileNotFoundError:
             pass
@@ -399,15 +443,18 @@
                 message="Could not get information about "
                 f"existing users on system: {e or '<no output>'}"
             )
         else:
             # for empty file return empty dict
             if raw.strip() == "":
                 return {}
-            users = [dict(zip(PASSWD_FIELDS, line.split(":"))) for line in raw.strip().split("\n")]
+            users = [
+                dict(zip(PASSWD_FIELDS, line.split(":")))
+                for line in raw.strip().split("\n")
+            ]
 
             # import json
             # thedata={user[ID_FIELD]: user for user in users}
             # str_str = json.dumps(thedata, sort_keys=True, indent=4, separators=(',', ': '))
             # logger.debug(str_str)
             # x = {user[ID_FIELD]: user for user in users}
             # logger.debug(F"whattttt: {x}")
@@ -438,38 +485,48 @@
 
     def _create_cmd(self):
         return ["groupadd", self.name]
 
     def create(self):
         try:
             subprocess.run(
-                self._create_cmd(), stdout=subprocess.PIPE, stderr=subprocess.PIPE, check=True
+                self._create_cmd(),
+                stdout=subprocess.PIPE,
+                stderr=subprocess.PIPE,
+                check=True,
             )
         except CalledProcessError as e:
             msg = (e.stderr or e.stdout or b"").decode("utf-8").strip()
-            logger.error("Error executing '{}': {}".format(" ".join(e.cmd), msg or "<no output>"))
+            logger.error(
+                "Error executing '{}': {}".format(" ".join(e.cmd), msg or "<no output>")
+            )
             raise Failure(message=f"Cannot create group: {msg or '<no output>'}")
 
     def create_tostring(self):
         return " ".join(self._create_cmd())
 
     @staticmethod
     def create_fromstring(create_cmd):
         # some sanity checks
         if not create_cmd.startswith("groupadd"):
             raise Failure(
                 message=f"Cannot create group (command is not applicable to this backend): {create_cmd}"
             )
         try:
             subprocess.run(
-                create_cmd.split(" "), stdout=subprocess.PIPE, stderr=subprocess.PIPE, check=True
+                create_cmd.split(" "),
+                stdout=subprocess.PIPE,
+                stderr=subprocess.PIPE,
+                check=True,
             )
         except CalledProcessError as e:
             msg = (e.stderr or e.stdout or b"").decode("utf-8").strip()
-            logger.error("Error executing '{}': {}".format(" ".join(e.cmd), msg or "<no output>"))
+            logger.error(
+                "Error executing '{}': {}".format(" ".join(e.cmd), msg or "<no output>")
+            )
             raise Failure(message=f"Cannot create group ({msg or '<no output>'})")
 
     def delete(self):
         # groupdel
         raise NotImplementedError("Do we even need this function?")
 
     def mod(self):
@@ -492,15 +549,17 @@
             f"Local group already exists for {original_name} with an old naming convention."
         )
         logger.warning(f"Renaming group {old_name} to {new_name}.")
         try:
             subprocess.run(["groupmod", "--new-name", new_name, old_name], check=True)
         except CalledProcessError as e:
             msg = (e.stderr or e.stdout or b"").decode("utf-8").strip()
-            logger.error("Error executing '{}': {}".format(" ".join(e.cmd), msg or "<no output>"))
+            logger.error(
+                "Error executing '{}': {}".format(" ".join(e.cmd), msg or "<no output>")
+            )
             raise Failure(message=f"Cannot create group: {msg or '<no output>'}")
 
     @staticmethod
     def __fix_duplicates(fix_id, original_name, old_name, new_name):
         logger.error(
             f"{fix_id}: Two local groups exist for {original_name}, created with different versions of make_shadow_compatible."
         )
@@ -521,15 +580,17 @@
         if self.name == self.name_v004:
             return
         all_groups = Group.__all_group_entries()
         if self.name_v004 in all_groups:
             if self.name not in all_groups:
                 Group.__rename(self.original_name, self.name_v004, self.name)
             else:
-                Group.__fix_duplicates("FIX v0.4.4", self.original_name, self.name_v004, self.name)
+                Group.__fix_duplicates(
+                    "FIX v0.4.4", self.original_name, self.name_v004, self.name
+                )
 
     @staticmethod
     def get_group_by_id(gid):
         """Gets the group name for a given GID."""
         try:
             return Group.__all_group_entries(ID_FIELD="gid")[str(gid)]["name"]
         except KeyError:
@@ -556,15 +617,18 @@
                 message="Could not get information about "
                 f"existing users on system: {e or '<no output>'}"
             )
         else:
             # for empty file return empty dict
             if raw.strip() == "":
                 return {}
-            groups = [dict(zip(GROUP_FIELDS, line.split(":"))) for line in raw.strip().split("\n")]
+            groups = [
+                dict(zip(GROUP_FIELDS, line.split(":")))
+                for line in raw.strip().split("\n")
+            ]
 
             for group in groups:
                 group[LIST_FIELD] = group[LIST_FIELD].split(",")  # type: ignore
 
             return {group[ID_FIELD]: group for group in groups}
 
 
@@ -648,15 +712,17 @@
                 raise (ValueError)
                 # TODO: fix case when removing chars from one fragment is not enough
                 # to shorten the word
                 # i.e. len(fragments[1] <= excess_chars)
             # logger.warning(F"shortened {orig_word} to {word}")
 
     if word != orig_word:
-        logger.debug("Name '{}' changed to '{}' for shadow compatibilty".format(orig_word, word))
+        logger.debug(
+            "Name '{}' changed to '{}' for shadow compatibilty".format(orig_word, word)
+        )
 
     return word
 
 
 def make_shadow_compatible_punch4nfdi(orig_word) -> str:
     """Ensure that orig_word is a valid user/group name for standard shadow utils.
     Special use case for punch4nfdi.
```

### Comparing `feudalAdapter-0.5.4/ldf_adapter/cmdline_params.py` & `feudalAdapter-0.6.0/ldf_adapter/cmdline_params.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,14 +36,16 @@
         "--config",
         "-c",
         "--conf",
         default="/etc/feudal/feudal_adapter.conf",
         help="Default: /etc/feudal/feudal_adapter.conf",
     )
 
-    parser.add_argument("--test", action="store_true", help="Test notifier configuration")
+    parser.add_argument(
+        "--test", action="store_true", help="Test notifier configuration"
+    )
 
     return parser
 
 
 # reparse args on import
 args = parseOptions().parse_args()
```

### Comparing `feudalAdapter-0.5.4/ldf_adapter/config.py` & `feudalAdapter-0.6.0/ldf_adapter/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,17 @@
     if PARSE_CMDLINE_PARAMETERS:
         files.insert(0, Path(args.config_file))
 
     # If the caller of the library has provided a configfile: prefer it:
     logger.debug(f"Files: {files}")
     try:
         globalconf_conf_file = Path(globalconfig.config["CONFIGFILE"])
-        logger.debug(f"Trying config of globalconfig: {globalconfig.config['CONFIGFILE']}")
+        logger.debug(
+            f"Trying config of globalconfig: {globalconfig.config['CONFIGFILE']}"
+        )
         if globalconf_conf_file.exists():
             files.insert(0, globalconf_conf_file)
     except KeyError:
         pass
 
     # Finally, check the environment (last means highes priority)
     filename = os.environ.get("FEUDAL_ADAPTER_CONFIG")
@@ -111,15 +113,16 @@
     @classmethod
     def load(cls, config: ConfigParser):
         """Sets only the fields that are present in the config file"""
         try:
             return cls(**config[cls.__section__name__()])
         except KeyError:
             logger.debug(
-                "Missing config section %s, using default values.", cls.__section__name__()
+                "Missing config section %s, using default values.",
+                cls.__section__name__(),
             )
             return cls()
 
     def __post_init__(self):
         """Converts some of the fields to the correct type"""
         for field in fields(self):
             value = getattr(self, field.name)
@@ -295,14 +298,15 @@
 class ConfigLocalUnix(ConfigSection):
     """Config section for local unix backend"""
 
     shell: str = "/bin/sh"
     home_base: str = "/home"
     deploy_user_ssh_keys: bool = True
     punch4nfdi: bool = False
+    post_create_script: Optional[str] = None
 
     @classmethod
     def __section__name__(cls):
         return "backend.local_unix"
 
     def __post_init__(self):
         super().__post_init__()
@@ -315,14 +319,15 @@
 
     url: str = "https://bwidm-test.scc.kit.edu/rest"
     org_id: str = "fdl"
     http_user: str = "foo"
     http_pass: str = "bar"
     service_name: str = "sshtest"
     log_outgoing_http_requests: bool = False
+    post_create_script: Optional[str] = None
 
     @classmethod
     def __section__name__(cls):
         return "backend.bwidm"
 
 
 @dataclass
@@ -337,14 +342,15 @@
     tls: bool = False
     user_base: str = "ou=users,dc=example"
     group_base: str = "ou=groups,dc=example"
     attribute_oidc_uid: str = "gecos"
     attribute_local_uid: str = "uid"
     shell: str = "/bin/sh"
     home_base: str = "/home"
+    post_create_script: Optional[str] = None
     uid_min: int = 1000
     uid_max: int = 60000
     gid_min: int = 1000
     gid_max: int = 60000
 
     def __post_init__(self):
         super().__post_init__()
@@ -398,18 +404,22 @@
     """All configuration settings for the feudal adapter"""
 
     ldf_adapter: ConfigLdfAdapter = field(default_factory=ConfigLdfAdapter)
     messages: ConfigMessages = field(default_factory=ConfigMessages)
     approval: ConfigApproval = field(default_factory=ConfigApproval)
     notifier: ConfigNotifiers = field(default_factory=ConfigNotifiers)
     assurance: ConfigAssurance = field(default_factory=ConfigAssurance)
-    username_generator: ConfigUsernameGenerator = field(default_factory=ConfigUsernameGenerator)
+    username_generator: ConfigUsernameGenerator = field(
+        default_factory=ConfigUsernameGenerator
+    )
     login_info: ConfigLoginInfo = field(default_factory=ConfigLoginInfo)
     backend: ConfigBackends = field(default_factory=ConfigBackends)
-    verbose_info_plugin: ConfigVerboseInfoPlugin = field(default_factory=ConfigVerboseInfoPlugin)
+    verbose_info_plugin: ConfigVerboseInfoPlugin = field(
+        default_factory=ConfigVerboseInfoPlugin
+    )
 
     @classmethod
     def load(cls, config: ConfigParser):
         """Loads all config settings from the given config parser"""
         return cls(**{f.name: f.type.load(config) for f in fields(cls)})
```

### Comparing `feudalAdapter-0.5.4/ldf_adapter/eduperson.py` & `feudalAdapter-0.6.0/ldf_adapter/eduperson.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,17 @@
             "urn:{namespace_id}:{delegated_namespace}{subnamespaces}"
             + ":group:{group}{subgroups}{role}"
             + "#{group_authority}"
         ).format(
             **{
                 **self.__dict__,
                 **{
-                    "subnamespaces": "".join([":{}".format(ns) for ns in self.subnamespaces]),
+                    "subnamespaces": "".join(
+                        [":{}".format(ns) for ns in self.subnamespaces]
+                    ),
                     "subgroups": "".join([":{}".format(grp) for grp in self.subgroups]),
                     "role": ":role={}".format(self.role) if self.role else "",
                 },
             }
         )
 
     def __str__(self):
@@ -73,15 +75,17 @@
             + " group={group}{subgroups}"
             + "{role}"
             + " auth={group_authority}>"
         ).format(
             **{
                 **self.__dict__,
                 **{
-                    "subnamespaces": "".join([",{}".format(ns) for ns in self.subnamespaces]),
+                    "subnamespaces": "".join(
+                        [",{}".format(ns) for ns in self.subnamespaces]
+                    ),
                     "subgroups": "".join([",{}".format(grp) for grp in self.subgroups]),
                     "role": " role={}".format(self.role) if self.role else "",
                 },
             }
         )
 
     @property
```

### Comparing `feudalAdapter-0.5.4/ldf_adapter/interface.py` & `feudalAdapter-0.6.0/ldf_adapter/interface.py`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.4/ldf_adapter/logsetup.py` & `feudalAdapter-0.6.0/ldf_adapter/logsetup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 # pylint: disable=missing-docstring, trailing-whitespace, trailing-newlines, too-few-public-methods
 
 import logging
 import os
 import sys
 from logging.handlers import RotatingFileHandler
 
-logger = logging.getLogger("ldf_adapter")  # => This is the key to allow logging from other modules
+logger = logging.getLogger(
+    "ldf_adapter"
+)  # => This is the key to allow logging from other modules
 jsonlogger = logging.getLogger("jsonlog.ldf_adapter")
 
 
 class PathTruncatingFormatter(logging.Formatter):
     """formatter for logging"""
 
     def format(self, record):
@@ -102,15 +104,17 @@
     )
     logger.debug(f'         {" ".join(sys.argv)} ')
 
     # JSON LOGGER
     # FIXME: jsonlogger name
     jsonlogfile = f"{logfile.rstrip('.log')}-json.log"
     jsonlogger = logging.getLogger("jsondata")
-    jsonfile_handler = RotatingFileHandler(jsonlogfile, maxBytes=100**6, backupCount=2)
+    jsonfile_handler = RotatingFileHandler(
+        jsonlogfile, maxBytes=100**6, backupCount=2
+    )
     jsonfile_handler.setFormatter(formatter)
     jsonfile_handler.setLevel(loglevel)
     jsonlogger.setLevel(loglevel)
     jsonlogger.addHandler(jsonfile_handler)
 
     return (logger, jsonlogger)
```

### Comparing `feudalAdapter-0.5.4/ldf_adapter/name_generators.py` & `feudalAdapter-0.6.0/ldf_adapter/name_generators.py`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.4/ldf_adapter/notifier/courier.py` & `feudalAdapter-0.6.0/ldf_adapter/notifier/courier.py`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.4/ldf_adapter/notifier/email.py` & `feudalAdapter-0.6.0/ldf_adapter/notifier/email.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,24 +100,30 @@
         msg["To"] = send_to
         return msg
 
     def _send_email(self, email: EmailMessage):
         """Send an email using the configured SMTP settings."""
         try:
             if self.use_ssl:
-                server = smtplib.SMTP_SSL(self.smtp_server, self.smtp_port, timeout=NOTIFY_TIMEOUT)
+                server = smtplib.SMTP_SSL(
+                    self.smtp_server, self.smtp_port, timeout=NOTIFY_TIMEOUT
+                )
             else:
-                server = smtplib.SMTP(self.smtp_server, self.smtp_port, timeout=NOTIFY_TIMEOUT)
+                server = smtplib.SMTP(
+                    self.smtp_server, self.smtp_port, timeout=NOTIFY_TIMEOUT
+                )
             server.ehlo()
             if self.sent_from_password:
                 server.login(self.sent_from, self.sent_from_password)
             server.send_message(email)
             server.close()
             logger.debug(
-                "Email with subject '%s' sent successfully to '%s'!", email["Subject"], email["To"]
+                "Email with subject '%s' sent successfully to '%s'!",
+                email["Subject"],
+                email["To"],
             )
         except Exception as ex:
             raise Exception("Could not send email to {%s}: %s", email["To"], ex)
 
     def notify(
         self,
         notification_type: generic.NotificationType,
@@ -139,26 +145,29 @@
         send_to = generic.NotificationTemplate(
             EMAIL_SETTINGS[notification_type].send_to_template
         ).fill(**data)
         subject = generic.NotificationTemplate(
             EMAIL_SETTINGS[notification_type].subject_template
         ).fill(**data)
         content = generic.NotificationTemplate.load(
-            Path(self.templates_dir) / EMAIL_SETTINGS[notification_type].body_template_file
+            Path(self.templates_dir)
+            / EMAIL_SETTINGS[notification_type].body_template_file
         ).fill(**data)
         email = self._build_email(send_to, subject, content)
         self._send_email(email)
         return True
 
     def test(self):
         """Send test notification to admin to make sure the configured set-up works."""
         if CONFIG.notifier.email is None:
             raise FatalError("Email notifier is not configured")
         settings = CONFIG.notifier.email.to_dict()
-        settings["sent_from_password"] = "*****" if settings["sent_from_password"] else None
+        settings["sent_from_password"] = (
+            "*****" if settings["sent_from_password"] else None
+        )
         data = {
             "admin_email": CONFIG.notifier.email.admin_email,
             "hostname": CONFIG.login_info.ssh_host,
             "notifier": "email",
             "settings": json.dumps(settings, indent=4),
         }
         self.notify(notification_type=generic.NotificationType.ADMIN_TEST, data=data)
```

### Comparing `feudalAdapter-0.5.4/ldf_adapter/notifier/generic.py` & `feudalAdapter-0.6.0/ldf_adapter/notifier/generic.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,17 @@
             template_id (str, optional): id of the template. Defaults to "".
         """
         self.template_body = template_body
         self.template_id = template_id
 
     def get_variables(self) -> list:
         """Returns list of variables in the template."""
-        return [var for var in Template(self.template_body).pattern.split("$") if var != ""]
+        return [
+            var for var in Template(self.template_body).pattern.split("$") if var != ""
+        ]
 
     def fill(self, **kwargs):
         """Fills template with given variables.
 
         Args:
             **kwargs: variables to fill template with.
         """
```

### Comparing `feudalAdapter-0.5.4/ldf_adapter/results.py` & `feudalAdapter-0.6.0/ldf_adapter/results.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,17 @@
                 default value of the named question. The type of thing determines the input of the
                 answer. Possible are strings, numbers or lists to provide the user with a selection
                 of the given values.
     **kwargs -- Any additional keyword arguments ar passed to ExceptionalResult.__init__
     """
 
     def __init__(self, questions, defaults, **kwargs):
-        super().__init__(state="questionnaire", message="There are unanswered questions.", **kwargs)
+        super().__init__(
+            state="questionnaire", message="There are unanswered questions.", **kwargs
+        )
         self.questionnaire = questions
         self.questionnaire_answers = defaults
 
 
 class Question(Questionnaire):
     """Convenience class to ask a single question."""
```

### Comparing `feudalAdapter-0.5.4/ldf_adapter/userinfo.py` & `feudalAdapter-0.6.0/ldf_adapter/userinfo.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,15 +113,17 @@
         # FIXME: Changing the sub of a user is potentially terrible
         sub = self.userinfo["sub"]
 
         sub = regex.sub("[^a-zA-Z0-9_!#$%&*+/=?{|}~^.-]", "-", sub)
 
         if sub != self.userinfo["sub"]:
             logger.warning(
-                "sub '{}' changed to '{}' to avoid confusion".format(self.userinfo["sub"], sub)
+                "sub '{}' changed to '{}' to avoid confusion".format(
+                    self.userinfo["sub"], sub
+                )
             )
         return sub
 
     def _iss_masked_for_bwidm_eppn(self):
         """Strip URI-scheme, transliterate to ASCII and replace invalid characters with a dash ('-').
 
         Usually there is only one issuer per FQDN (which is mostly left untouched, apart from
@@ -133,15 +135,17 @@
         iss = regex.sub("[^a-zA-Z0-9.-]", "-", iss)
 
         # We don't consider stripping the http[s]-prefix a change, since we always do that anyway,
         # and there shouldn't be two different issuers `http://example.org' and `https://example.org'.
         if iss != stripped_iss:
             if CONFIG.messages.log_name_changes:
                 logger.warning(
-                    "Issuer '{}' changed to '{}' for general compatibilty".format(stripped_iss, iss)
+                    "Issuer '{}' changed to '{}' for general compatibilty".format(
+                        stripped_iss, iss
+                    )
                 )
         return iss
 
     @property
     @lru_cache(maxsize=None)
     def username(self):
         """Return the user's name, this may be:
@@ -192,15 +196,19 @@
             family_name_from_name = None
 
         try:
             family_name_from_name = self.userinfo["name"].split(" ")[-1]
         except KeyError:
             family_name_from_name = None
 
-        return self.userinfo.get("family_name") or family_name_from_sn or family_name_from_name
+        return (
+            self.userinfo.get("family_name")
+            or family_name_from_sn
+            or family_name_from_name
+        )
 
     @property
     @lru_cache(maxsize=None)
     def full_name(self):
         """Return the user's full name. If none is provided, try to assemple it from the first and given name."""
         return self.userinfo.get("name") or " ".join(
             filter(None, [self.given_name, self.family_name])
@@ -259,15 +267,17 @@
                 filter(
                     None,
                     [
                         "{}_{}".format(ns, grp)
                         for (ns, grp) in chain.from_iterable(
                             (
                                 (
-                                    "-".join([ent.delegated_namespace] + ent.subnamespaces),
+                                    "-".join(
+                                        [ent.delegated_namespace] + ent.subnamespaces
+                                    ),
                                     grp,
                                 )
                                 for grp in ent.all_toplevel_groups
                             )
                             for ent in self.entitlement
                         )
                     ],
@@ -325,15 +335,17 @@
         grp = regex.sub("^7", "seven_", grp)
         grp = regex.sub("^8", "eight_", grp)
         grp = regex.sub("^9", "nine_", grp)
 
         if grp != orig_grp:
             if CONFIG.messages.log_name_changes:
                 logger.warning(
-                    "Group name '{}' changed to '{}' for general compatibilty".format(orig_grp, grp)
+                    "Group name '{}' changed to '{}' for general compatibilty".format(
+                        orig_grp, grp
+                    )
                 )
 
         return grp
 
     @property
     @lru_cache(maxsize=None)
     def assurance(self):
@@ -398,15 +410,17 @@
 
     @property
     @lru_cache(maxsize=None)
     def preferred_username(self):
         """Return the prefrred username of the user."""
         return self.userinfo.get("preferred_username", None)
 
-    def value_or_ask(self, value, answer_name, question_text, allow_question, default=None):
+    def value_or_ask(
+        self, value, answer_name, question_text, allow_question, default=None
+    ):
         """Return the submitted answer, the default value or raise a questionaire."""
         previous_answer = self.answers.get(answer_name)
         return (
             previous_answer
             or value
             or (
                 allow_question
@@ -415,24 +429,31 @@
                     text=question_text,
                     default=default,
                 )
             )
         )
 
     def __str__(self):
-        attrs = ("{} = {}".format(k, getattr(UserInfo, k).fget(self)) for k in iter(self))
+        attrs = (
+            "{} = {}".format(k, getattr(UserInfo, k).fget(self)) for k in iter(self)
+        )
 
-        return "<UserInfo\n{}\n>".format("\n".join("\t{}".format(attr) for attr in attrs))
+        return "<UserInfo\n{}\n>".format(
+            "\n".join("\t{}".format(attr) for attr in attrs)
+        )
 
     def __getitem__(self, key):
         return getattr(self, key, lambda: (_ for _ in ()).throw(KeyError(key)))
 
     def __iter__(self):
         return (k for k in dir(UserInfo) if type(getattr(UserInfo, k)) is property)
 
     def __len__(self):
         return sum(
-            1 for _ in filter(lambda k: type(getattr(UserInfo, k)) is property, dir(UserInfo))
+            1
+            for _ in filter(
+                lambda k: type(getattr(UserInfo, k)) is property, dir(UserInfo)
+            )
         )
 
     def __hash__(self):
         return id(self)  # Good enough for lru_cache
```

### Comparing `feudalAdapter-0.5.4/ldf_adapter/utils.py` & `feudalAdapter-0.6.0/ldf_adapter/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,17 @@
     """
     for k, v in diff.items():
         if isinstance(v, dict):
             log_dictdiff(v, log_function, "{}/".format(k))
         else:
             (old, new) = v
             if old:
-                log_function("Updating {}{} from '{}' to '{}'".format(prefix, k, old, new))
+                log_function(
+                    "Updating {}{} from '{}' to '{}'".format(prefix, k, old, new)
+                )
             else:
                 log_function("Setting {}{} to '{}'".format(prefix, k, new))
 
 
 def dictmerge(lhs, rhs):
     """Merge two dicts recusively."""
     res = copy.deepcopy(lhs)
@@ -67,35 +69,41 @@
     """Convert a string to bool.
     Raise a FatalError if the string cannot be converted.
     """
     if bool_str.lower() in ["true", "yes", "yes, do as i say!"]:
         return True
     if bool_str.lower() in ["false", "no"]:
         return False
-    raise FatalError(f"Error converting to bool: unrecognised boolean value {bool_str}.")
+    raise FatalError(
+        f"Error converting to bool: unrecognised boolean value {bool_str}."
+    )
 
 
 def to_int(int_str):
     """Convert a string to int.
     Raise a FatalError if the string cannot be converted.
     """
     try:
         return int(int_str)
     except ValueError:
-        raise FatalError(f"Error converting to int: unrecognised integer value {int_str}.")
+        raise FatalError(
+            f"Error converting to int: unrecognised integer value {int_str}."
+        )
 
 
 def to_list(list_str):
     """Convert a string containing comma-separated strings to list of strings.
     Raise a FatalError if the string cannot be converted.
     """
     try:
         return list(set(list_str.split()))
     except ValueError:
-        raise FatalError(f"Error converting to list: unrecognised list value {list_str}.")
+        raise FatalError(
+            f"Error converting to list: unrecognised list value {list_str}."
+        )
 
 
 def dynamic_import(fq_module_name: str, class_name: str) -> Type:
     """Import a class dynamically.
 
     Args:
         fq_module_name: The fully qualified name of the module to import.
@@ -103,15 +111,17 @@
     Returns:
         The imported class.
     """
     module = __import__(fq_module_name, fromlist=[class_name])
     try:
         return getattr(module, class_name)
     except AttributeError:
-        raise FatalError(message=f"Module {fq_module_name} does not contain class {class_name}")
+        raise FatalError(
+            message=f"Module {fq_module_name} does not contain class {class_name}"
+        )
 
 
 @dataclass
 class BuilderConfig:
     fq_module_name: str
     class_name: str
 
@@ -189,12 +199,16 @@
         class_name (str): name of class to provide objects for.
 
     Returns:
         ObjectFactory: factory for the given class.
     """
     factory = ObjectFactory()
     for file in glob.glob(join(dir_name, "*.py")):
-        if isfile(file) and not file.endswith("__init__.py") and not file.endswith("generic.py"):
+        if (
+            isfile(file)
+            and not file.endswith("__init__.py")
+            and not file.endswith("generic.py")
+        ):
             module_name = basename(file)[:-3]
             fq_module_name = f"{parent_module}.{module_name}"
             factory.register_builder(module_name, fq_module_name, class_name)
     return factory
```

### Comparing `feudalAdapter-0.5.4/setup.cfg` & `feudalAdapter-0.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.4/states.md` & `feudalAdapter-0.6.0/states.md`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.4/subiss-to-unix.py` & `feudalAdapter-0.6.0/subiss-to-unix.py`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.4/templates/admin.deploy.template` & `feudalAdapter-0.6.0/templates/admin.deploy.template`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.4/templates/admin.deploy.update.template` & `feudalAdapter-0.6.0/templates/admin.deploy.update.template`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.4/templates/admin.update.template` & `feudalAdapter-0.6.0/templates/admin.update.template`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.4/tests/approval/db/generic.py` & `feudalAdapter-0.6.0/tests/approval/db/generic.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,16 @@
 
 
 @pytest.fixture(scope="function")
 def pending_db(db_type):
     databases._builders = {}
     if db_type == "sqlite":
         with mock.patch(
-            "ldf_adapter.approval.db.sqlite.CONFIG.approval.user_db_location", ":memory:"
+            "ldf_adapter.approval.db.sqlite.CONFIG.approval.user_db_location",
+            ":memory:",
         ):
             yield databases.get(db_type)
     else:
         yield databases.get(db_type)
 
 
 @pytest.mark.parametrize("db_type", ["sqlite"])
@@ -194,18 +195,24 @@
     assert pending_db.get_memberships(MOCK_MEMBERSHIPS.unique_id) == None
     # notify memberships that don't exist
     pending_db.notify_memberships(MOCK_MEMBERSHIPS.unique_id)
 
     # notify memberships that do exist
     pending_db.add_memberships(MOCK_MEMBERSHIPS)
     # get_memberships returns memberships in PENDING state
-    assert pending_db.get_memberships(MOCK_MEMBERSHIPS.unique_id).state == DeploymentState.PENDING
+    assert (
+        pending_db.get_memberships(MOCK_MEMBERSHIPS.unique_id).state
+        == DeploymentState.PENDING
+    )
     pending_db.notify_memberships(MOCK_MEMBERSHIPS.unique_id)
     # get memberships returns memberships in NOTIFIED state
-    assert pending_db.get_memberships(MOCK_MEMBERSHIPS.unique_id).state == DeploymentState.NOTIFIED
+    assert (
+        pending_db.get_memberships(MOCK_MEMBERSHIPS.unique_id).state
+        == DeploymentState.NOTIFIED
+    )
 
 
 @pytest.mark.parametrize("db_type", ["sqlite"])
 def test_update_memberships(pending_db):
     # get_memberships returns None
     assert pending_db.get_memberships(MOCK_MEMBERSHIPS.unique_id) == None
     # update memberships that don't exist: doesn't fail, but nothing changes
@@ -213,8 +220,11 @@
     # get_memberships returns None
     assert pending_db.get_memberships(MOCK_MEMBERSHIPS.unique_id) == None
 
     # update memberships that do exist
     pending_db.add_memberships(MOCK_MEMBERSHIPS)
     pending_db.update_memberships(MOCK_MEMBERSHIPS_UPDATED)
     # get_memberships returns updated value
-    assert pending_db.get_memberships(MOCK_MEMBERSHIPS.unique_id) == MOCK_MEMBERSHIPS_UPDATED
+    assert (
+        pending_db.get_memberships(MOCK_MEMBERSHIPS.unique_id)
+        == MOCK_MEMBERSHIPS_UPDATED
+    )
```

### Comparing `feudalAdapter-0.5.4/tests/approval/db/sqlite.py` & `feudalAdapter-0.6.0/tests/approval/db/sqlite.py`

 * *Files 4% similar despite different names*

```diff
@@ -179,28 +179,35 @@
     )
 """
 
 
 @pytest.mark.parametrize(
     "data_model,table_name,primary_key,expected_cmd",
     [
-        (MyDataModel, "my_data_model", ["id", "address"], create_my_data_model_table_cmd),
+        (
+            MyDataModel,
+            "my_data_model",
+            ["id", "address"],
+            create_my_data_model_table_cmd,
+        ),
         (PendingUser, "pending_users", "unique_id", create_pending_users_table_cmd),
         (PendingGroup, "pending_groups", "name", create_pending_groups_table_cmd),
         (
             PendingMemberships,
             "pending_memberships",
             "unique_id",
             create_pending_memberships_table_cmd,
         ),
     ],
 )
 def test_sql_command_create_table(data_model, table_name, primary_key, expected_cmd):
     assert (
-        "".join(sql_command_create_table(data_model, table_name, primary_key).split()).lower()
+        "".join(
+            sql_command_create_table(data_model, table_name, primary_key).split()
+        ).lower()
         == "".join(expected_cmd.split()).lower()
     )
 
 
 insert_my_data_model_cmd = """
     insert into my_data_model
     (id, name, age, height, weight, is_married, children, address, deployment_state)
@@ -285,16 +292,26 @@
         (
             "my_data_model",
             ["name", "age", "height", "weight"],
             ["id", "address"],
             update_my_data_model_cmd,
         ),
         ("pending_users", ["state"], "unique_id", update_pending_users_cmd),
-        ("pending_groups", ["state", "cmd", "infodict"], ["name"], update_pending_groups_cmd),
-        ("pending_memberships", ["unique_id"], "unique_id", update_pending_memberships_cmd),
+        (
+            "pending_groups",
+            ["state", "cmd", "infodict"],
+            ["name"],
+            update_pending_groups_cmd,
+        ),
+        (
+            "pending_memberships",
+            ["unique_id"],
+            "unique_id",
+            update_pending_memberships_cmd,
+        ),
         ("pending_users", ["unknown_field"], "unique_id", update_pending_users_cmd2),
         ("pending_users", ["unique_id"], "unknown_key", update_pending_users_cmd3),
     ],
 )
 def test_sql_command_update(table_name, columns, key, expected_cmd):
     assert (
         "".join(sql_command_update(table_name, columns, key).split()).lower()
@@ -339,72 +356,94 @@
     connector.connect()
     connector.create(data_model, table_name, primary_key)
     entry = tuple(getattr(mock_object, field.name) for field in fields(data_model))
     connector.insert(data_model, table_name, entry)
     yield connector
 
 
-@pytest.mark.parametrize("data_model,table_name,primary_key,mock_object", sample_data_sqlite)
-def test_create_unknown_key(mock_connector, data_model, table_name, primary_key, mock_object):
+@pytest.mark.parametrize(
+    "data_model,table_name,primary_key,mock_object", sample_data_sqlite
+)
+def test_create_unknown_key(
+    mock_connector, data_model, table_name, primary_key, mock_object
+):
     with pytest.raises(SystemExit) as excinfo:
         mock_connector.create(data_model, table_name, "unknown_key")
     assert excinfo.value.code == FatalError.exit_code
 
 
-@pytest.mark.parametrize("data_model,table_name,primary_key,mock_object", sample_data_sqlite)
-def test_create_successful(mock_connector, data_model, table_name, primary_key, mock_object):
+@pytest.mark.parametrize(
+    "data_model,table_name,primary_key,mock_object", sample_data_sqlite
+)
+def test_create_successful(
+    mock_connector, data_model, table_name, primary_key, mock_object
+):
     mock_connector.create(data_model, table_name, primary_key)
     c = mock_connector.connection.cursor()
     # check if table exists
-    c.execute(f"SELECT name FROM sqlite_master WHERE type='table' AND name='{table_name}';")
+    c.execute(
+        f"SELECT name FROM sqlite_master WHERE type='table' AND name='{table_name}';"
+    )
     assert c.fetchone()[0] == table_name
     # check if table has the correct columns
     c.execute(f"PRAGMA table_info({table_name});")
     columns = [row[1] for row in c.fetchall()]
     assert columns == [f.name for f in fields(data_model)]
     # check if table has the correct primary key
     c.execute(f"PRAGMA table_info({table_name});")
     primary_key_set = [row[1] for row in c.fetchall() if row[5] != 0]
     assert primary_key_set == primary_key
 
 
-@pytest.mark.parametrize("data_model,table_name,primary_key,mock_object", sample_data_sqlite)
-def test_create_if_not_exists(mock_connector, data_model, table_name, primary_key, mock_object):
+@pytest.mark.parametrize(
+    "data_model,table_name,primary_key,mock_object", sample_data_sqlite
+)
+def test_create_if_not_exists(
+    mock_connector, data_model, table_name, primary_key, mock_object
+):
     mock_connector.create(data_model, table_name, primary_key)
     mock_connector.create(data_model, table_name, primary_key)
     # check that second create didn't raise any exception, but didn't create a new table
     result = (
         mock_connector.connection.cursor()
-        .execute(f"SELECT name FROM sqlite_master WHERE type='table' AND name='{table_name}';")
+        .execute(
+            f"SELECT name FROM sqlite_master WHERE type='table' AND name='{table_name}';"
+        )
         .fetchall()
     )
     assert len(result) == 1
     assert result[0][0] == table_name
 
 
-@pytest.mark.parametrize("data_model,table_name,primary_key,mock_object", sample_data_sqlite)
+@pytest.mark.parametrize(
+    "data_model,table_name,primary_key,mock_object", sample_data_sqlite
+)
 def test_insert_table_doesnt_exist(
     mock_connector, data_model, table_name, primary_key, mock_object
 ):
     entry = tuple(getattr(mock_object, field.name) for field in fields(data_model))
     with pytest.raises(Failure):
         mock_connector.insert(data_model, table_name, entry)
 
 
-@pytest.mark.parametrize("data_model,table_name,primary_key,mock_object", sample_data_sqlite)
+@pytest.mark.parametrize(
+    "data_model,table_name,primary_key,mock_object", sample_data_sqlite
+)
 def test_insert_wrong_number_of_columns(
     mock_connector_with_table, data_model, table_name, primary_key, mock_object
 ):
     entry = tuple(getattr(mock_object, field.name) for field in fields(data_model))
     wrong_entry = entry + ("wrong",)
     with pytest.raises(Failure):
         mock_connector_with_table.insert(data_model, table_name, wrong_entry)
 
 
-@pytest.mark.parametrize("data_model,table_name,primary_key,mock_object", sample_data_sqlite)
+@pytest.mark.parametrize(
+    "data_model,table_name,primary_key,mock_object", sample_data_sqlite
+)
 def test_insert_successful(
     mock_connector_with_table, data_model, table_name, primary_key, mock_object
 ):
     entry = tuple(getattr(mock_object, field.name) for field in fields(data_model))
     assert mock_connector_with_table.insert(data_model, table_name, entry) == True
     # check that inserted entry is the same as the mock object
     result = (
@@ -412,84 +451,104 @@
         .execute(f"SELECT * FROM {table_name};")
         .fetchall()
     )
     assert len(result) == 1
     assert result[0] == entry
 
 
-@pytest.mark.parametrize("data_model,table_name,primary_key,mock_object", sample_data_sqlite)
+@pytest.mark.parametrize(
+    "data_model,table_name,primary_key,mock_object", sample_data_sqlite
+)
 def test_insert_entry_exists(
     mock_connector_with_entry, data_model, table_name, primary_key, mock_object
 ):
     entry = tuple(getattr(mock_object, field.name) for field in fields(data_model))
     assert mock_connector_with_entry.insert(data_model, table_name, entry) == False
 
 
-@pytest.mark.parametrize("data_model,table_name,primary_key,mock_object", sample_data_sqlite)
+@pytest.mark.parametrize(
+    "data_model,table_name,primary_key,mock_object", sample_data_sqlite
+)
 def test_select_table_doesnt_exist(
     mock_connector, data_model, table_name, primary_key, mock_object
 ):
     if isinstance(primary_key, list):
         primary_key_value = tuple([getattr(mock_object, key) for key in primary_key])
     else:
         primary_key_value = (getattr(mock_object, primary_key),)
     with pytest.raises(Failure):
         mock_connector.select(data_model, table_name, primary_key, primary_key_value)
 
 
-@pytest.mark.parametrize("data_model,table_name,primary_key,mock_object", sample_data_sqlite)
+@pytest.mark.parametrize(
+    "data_model,table_name,primary_key,mock_object", sample_data_sqlite
+)
 def test_select_entry_not_found(
     mock_connector_with_table, data_model, table_name, primary_key, mock_object
 ):
     if isinstance(primary_key, list):
         primary_key_value = tuple([getattr(mock_object, key) for key in primary_key])
     else:
         primary_key_value = (getattr(mock_object, primary_key),)
     assert (
-        mock_connector_with_table.select(data_model, table_name, primary_key, primary_key_value)
+        mock_connector_with_table.select(
+            data_model, table_name, primary_key, primary_key_value
+        )
         is None
     )
 
 
-@pytest.mark.parametrize("data_model,table_name,primary_key,mock_object", sample_data_sqlite)
-def test_select_found(mock_connector_with_entry, data_model, table_name, primary_key, mock_object):
+@pytest.mark.parametrize(
+    "data_model,table_name,primary_key,mock_object", sample_data_sqlite
+)
+def test_select_found(
+    mock_connector_with_entry, data_model, table_name, primary_key, mock_object
+):
     if isinstance(primary_key, list):
         primary_key_value = tuple([getattr(mock_object, key) for key in primary_key])
     else:
         primary_key_value = (getattr(mock_object, primary_key),)
     assert (
-        mock_connector_with_entry.select(data_model, table_name, primary_key, primary_key_value)
+        mock_connector_with_entry.select(
+            data_model, table_name, primary_key, primary_key_value
+        )
         == mock_object
     )
 
 
-@pytest.mark.parametrize("data_model,table_name,primary_key,mock_object", sample_data_sqlite)
+@pytest.mark.parametrize(
+    "data_model,table_name,primary_key,mock_object", sample_data_sqlite
+)
 def test_delete_table_doesnt_exist(
     mock_connector, data_model, table_name, primary_key, mock_object
 ):
     if isinstance(primary_key, list):
         primary_key_value = tuple([getattr(mock_object, key) for key in primary_key])
     else:
         primary_key_value = (getattr(mock_object, primary_key),)
     with pytest.raises(Failure):
         mock_connector.delete(table_name, primary_key, primary_key_value)
 
 
-@pytest.mark.parametrize("data_model,table_name,primary_key,mock_object", sample_data_sqlite)
+@pytest.mark.parametrize(
+    "data_model,table_name,primary_key,mock_object", sample_data_sqlite
+)
 def test_delete_entry_doesnt_exist(
     mock_connector_with_table, data_model, table_name, primary_key, mock_object
 ):
     if isinstance(primary_key, list):
         primary_key_value = tuple([getattr(mock_object, key) for key in primary_key])
     else:
         primary_key_value = (getattr(mock_object, primary_key),)
     mock_connector_with_table.delete(table_name, primary_key, primary_key_value)
 
 
-@pytest.mark.parametrize("data_model,table_name,primary_key,mock_object", sample_data_sqlite)
+@pytest.mark.parametrize(
+    "data_model,table_name,primary_key,mock_object", sample_data_sqlite
+)
 def test_delete_successful(
     mock_connector_with_entry, data_model, table_name, primary_key, mock_object
 ):
     if isinstance(primary_key, list):
         primary_key_value = tuple([getattr(mock_object, key) for key in primary_key])
     else:
         primary_key_value = (getattr(mock_object, primary_key),)
@@ -500,16 +559,32 @@
         .fetchall()
     )
     assert len(result) == 0
 
 
 # "data_model,table_name,primary_key,mock_object,column,value,second_value"
 sample_data_sqlite_select_on_column = [
-    (PendingUser, "pending_users", ["unique_id"], MOCK_USER, "cmd", "cmd", "another_unique_id"),
-    (PendingGroup, "pending_groups", ["name"], MOCK_GROUP, "cmd", "cmd", "another_name"),
+    (
+        PendingUser,
+        "pending_users",
+        ["unique_id"],
+        MOCK_USER,
+        "cmd",
+        "cmd",
+        "another_unique_id",
+    ),
+    (
+        PendingGroup,
+        "pending_groups",
+        ["name"],
+        MOCK_GROUP,
+        "cmd",
+        "cmd",
+        "another_name",
+    ),
     (
         PendingMemberships,
         "pending_memberships",
         ["unique_id"],
         MOCK_MEMBERSHIPS,
         "cmd",
         "cmd",
@@ -528,15 +603,22 @@
 
 
 @pytest.mark.parametrize(
     "data_model,table_name,primary_key,mock_object,column,value,second_value",
     sample_data_sqlite_select_on_column,
 )
 def test_select_on_column_table_doesnt_exist(
-    mock_connector, data_model, table_name, primary_key, mock_object, column, value, second_value
+    mock_connector,
+    data_model,
+    table_name,
+    primary_key,
+    mock_object,
+    column,
+    value,
+    second_value,
 ):
     with pytest.raises(Failure):
         mock_connector.select(data_model, table_name, column, (value,))
 
 
 @pytest.mark.parametrize(
     "data_model,table_name,primary_key,mock_object,column,value,second_value",
@@ -548,15 +630,18 @@
     table_name,
     primary_key,
     mock_object,
     column,
     value,
     second_value,
 ):
-    assert mock_connector_with_table.select(data_model, table_name, column, (value,)) is None
+    assert (
+        mock_connector_with_table.select(data_model, table_name, column, (value,))
+        is None
+    )
 
 
 @pytest.mark.parametrize(
     "data_model,table_name,primary_key,mock_object,column,value,second_value",
     sample_data_sqlite_select_on_column,
 )
 def test_select_on_column_found(
@@ -565,15 +650,18 @@
     table_name,
     primary_key,
     mock_object,
     column,
     value,
     second_value,
 ):
-    assert mock_connector_with_entry.select(data_model, table_name, column, (value,)) == mock_object
+    assert (
+        mock_connector_with_entry.select(data_model, table_name, column, (value,))
+        == mock_object
+    )
 
 
 @pytest.mark.parametrize(
     "data_model,table_name,primary_key,mock_object,column,value,second_value",
     sample_data_sqlite_select_on_column,
 )
 def test_select_on_column_multiple_entries(
@@ -587,49 +675,76 @@
     second_value,
 ):
     # insert a second entry with same column value
     mock_object2 = copy.copy(mock_object)
     mock_object2.__setattr__(
         primary_key[0] if isinstance(primary_key, list) else primary_key, second_value
     )
-    second_entry = tuple(getattr(mock_object2, field.name) for field in fields(data_model))
+    second_entry = tuple(
+        getattr(mock_object2, field.name) for field in fields(data_model)
+    )
     mock_connector_with_entry.insert(data_model, table_name, second_entry)
     # check that select returns first entry when multiple entries are found
-    assert mock_connector_with_entry.select(data_model, table_name, column, (value,)) == mock_object
+    assert (
+        mock_connector_with_entry.select(data_model, table_name, column, (value,))
+        == mock_object
+    )
 
 
 # "data_model,table_name,primary_key,mock_object,column,value"
 sample_data_sqlite_update = [
     (PendingUser, "pending_users", "unique_id", MOCK_USER, "cmd", "cmd2"),
     (PendingGroup, "pending_groups", "name", MOCK_GROUP, "cmd", "cmd2"),
-    (PendingMemberships, "pending_memberships", "unique_id", MOCK_MEMBERSHIPS, "cmd", "cmd2"),
-    (MyDataModel, "my_data_model", ["id", "address"], MOCK_MY_DATA_MODEL, "name", "name2"),
+    (
+        PendingMemberships,
+        "pending_memberships",
+        "unique_id",
+        MOCK_MEMBERSHIPS,
+        "cmd",
+        "cmd2",
+    ),
+    (
+        MyDataModel,
+        "my_data_model",
+        ["id", "address"],
+        MOCK_MY_DATA_MODEL,
+        "name",
+        "name2",
+    ),
 ]
 
 
 @pytest.mark.parametrize(
-    "data_model,table_name,primary_key,mock_object,column,value", sample_data_sqlite_update
+    "data_model,table_name,primary_key,mock_object,column,value",
+    sample_data_sqlite_update,
 )
 def test_update_table_doesnt_exist(
     mock_connector, data_model, table_name, primary_key, mock_object, column, value
 ):
     if isinstance(primary_key, list):
         primary_key_value = tuple([getattr(mock_object, key) for key in primary_key])
     else:
         primary_key_value = (getattr(mock_object, primary_key),)
     entry = (value,) + primary_key_value
     with pytest.raises(Failure):
         mock_connector.update(table_name, [column], primary_key, entry)
 
 
 @pytest.mark.parametrize(
-    "data_model,table_name,primary_key,mock_object,column,value", sample_data_sqlite_update
+    "data_model,table_name,primary_key,mock_object,column,value",
+    sample_data_sqlite_update,
 )
 def test_update_entry_doesnt_exist(
-    mock_connector_with_table, data_model, table_name, primary_key, mock_object, column, value
+    mock_connector_with_table,
+    data_model,
+    table_name,
+    primary_key,
+    mock_object,
+    column,
+    value,
 ):
     if isinstance(primary_key, list):
         primary_key_value = tuple([getattr(mock_object, key) for key in primary_key])
     else:
         primary_key_value = (getattr(mock_object, primary_key),)
     entry = (value,) + primary_key_value
     # does not fail, but does not modify anything
@@ -645,48 +760,71 @@
         .execute(f"SELECT * FROM {table_name};")
         .fetchall()
     )
     assert result_before == result_after
 
 
 @pytest.mark.parametrize(
-    "data_model,table_name,primary_key,mock_object,column,value", sample_data_sqlite_update
+    "data_model,table_name,primary_key,mock_object,column,value",
+    sample_data_sqlite_update,
 )
 def test_update_wrong_number_of_columns(
-    mock_connector_with_entry, data_model, table_name, primary_key, mock_object, column, value
+    mock_connector_with_entry,
+    data_model,
+    table_name,
+    primary_key,
+    mock_object,
+    column,
+    value,
 ):
     if isinstance(primary_key, list):
         primary_key_value = tuple([getattr(mock_object, key) for key in primary_key])
     else:
         primary_key_value = (getattr(mock_object, primary_key),)
     entry = (value,) + primary_key_value
     with pytest.raises(Failure):
-        mock_connector_with_entry.update(table_name, [column, column], primary_key, entry)
+        mock_connector_with_entry.update(
+            table_name, [column, column], primary_key, entry
+        )
 
 
 @pytest.mark.parametrize(
-    "data_model,table_name,primary_key,mock_object,column,value", sample_data_sqlite_update
+    "data_model,table_name,primary_key,mock_object,column,value",
+    sample_data_sqlite_update,
 )
 def test_update_wrong_number_of_values(
-    mock_connector_with_entry, data_model, table_name, primary_key, mock_object, column, value
+    mock_connector_with_entry,
+    data_model,
+    table_name,
+    primary_key,
+    mock_object,
+    column,
+    value,
 ):
     if isinstance(primary_key, list):
         primary_key_value = tuple([getattr(mock_object, key) for key in primary_key])
     else:
         primary_key_value = (getattr(mock_object, primary_key),)
     entry = (value,) + primary_key_value
     with pytest.raises(Failure):
         mock_connector_with_entry.update(table_name, [column], primary_key, entry[:-1])
 
 
 @pytest.mark.parametrize(
-    "data_model,table_name,primary_key,mock_object,column,value", sample_data_sqlite_update
+    "data_model,table_name,primary_key,mock_object,column,value",
+    sample_data_sqlite_update,
 )
 def test_update_successful(
-    mock_connector_with_entry, data_model, table_name, primary_key, mock_object, column, value
+    mock_connector_with_entry,
+    data_model,
+    table_name,
+    primary_key,
+    mock_object,
+    column,
+    value,
 ):
     if isinstance(primary_key, list):
         primary_key_value = tuple([getattr(mock_object, key) for key in primary_key])
     else:
         primary_key_value = (getattr(mock_object, primary_key),)
     entry = (value,) + primary_key_value
     mock_connector_with_entry.update(table_name, [column], primary_key, entry)
```

### Comparing `feudalAdapter-0.5.4/tests/backend/ldap.py` & `feudalAdapter-0.6.0/tests/backend/ldap.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,17 @@
         mp.setattr("ldf_adapter.backend.ldap.CONFIG.backend.ldap.mode", mode)
 
         import ldf_adapter.backend.ldap
 
         service_user = ldf_adapter.backend.ldap.User(MockUserInfo(userinfo))
         for entry in existing_entries:
             ldf_adapter.backend.ldap.LDAP.connection.add(
-                entry["dn"], object_class=entry["object_class"], attributes=entry["attributes"]
+                entry["dn"],
+                object_class=entry["object_class"],
+                attributes=entry["attributes"],
             )
         yield service_user
         # module needs to be reloaded on next test so that LDAP object is recreated
         del sys.modules["ldf_adapter.backend.ldap"]
 
 
 @pytest.fixture(scope="function")
@@ -57,22 +59,26 @@
         mp.setattr("ldf_adapter.backend.ldap.CONFIG.backend.ldap.mode", mode)
 
         import ldf_adapter.backend.ldap
 
         service_group = ldf_adapter.backend.ldap.Group(name)
         for entry in existing_entries:
             ldf_adapter.backend.ldap.LDAP.connection.add(
-                entry["dn"], object_class=entry["object_class"], attributes=entry["attributes"]
+                entry["dn"],
+                object_class=entry["object_class"],
+                attributes=entry["attributes"],
             )
         yield service_group
         del sys.modules["ldf_adapter.backend.ldap"]
 
 
 @pytest.fixture(scope="function")
-def ldap_mod_entry(mode, userinfo, supplementary_group_names, existing_entries, monkeypatch):
+def ldap_mod_entry(
+    mode, userinfo, supplementary_group_names, existing_entries, monkeypatch
+):
     """Creates a backend user and groups from provided data.
     'userinfo' should contain: unique_id, username, primary_group.
     'supplementary_group_names' is a list of group names
     'existing_entries' are LDAP entries to be added beforehand;
         each entry contains a dn and a dict of attributes.
     """
     with monkeypatch.context() as mp:
@@ -83,15 +89,17 @@
 
         service_user = ldf_adapter.backend.ldap.User(MockUserInfo(userinfo))
         supplementary_groups = []
         for name in supplementary_group_names:
             supplementary_groups.append(ldf_adapter.backend.ldap.Group(name))
         for entry in existing_entries:
             ldf_adapter.backend.ldap.LDAP.connection.add(
-                entry["dn"], object_class=entry["object_class"], attributes=entry["attributes"]
+                entry["dn"],
+                object_class=entry["object_class"],
+                attributes=entry["attributes"],
             )
         yield {"user": service_user, "supplementary_groups": supplementary_groups}
         del sys.modules["ldf_adapter.backend.ldap"]
 
 
 @pytest.fixture(scope="function")
 def ldap_connection(uid_min, uid_max, gid_min, gid_max, monkeypatch):
@@ -229,15 +237,19 @@
     with pytest.raises(Rejection):
         ldap_user.create()
 
 
 @pytest.mark.parametrize(
     "mode,userinfo,existing_entries",
     [
-        ("pre_created", USERINFO, [LDAP_PRECREATED_USER_ENTRY, LDAP_PRECREATED_TESTGROUP_ENTRY]),
+        (
+            "pre_created",
+            USERINFO,
+            [LDAP_PRECREATED_USER_ENTRY, LDAP_PRECREATED_TESTGROUP_ENTRY],
+        ),
     ],
 )
 def test_create_user_precreated_exists(ldap_user):
     """In pre_created mode, create succeeds if entry for username exists by mapping entry to unique_id.
     Will not check if entry already mapped to something else, since ldf_adapter user checks if
     user exists or if name_taken beforehand.
     """
@@ -472,15 +484,20 @@
 @pytest.mark.parametrize("mode", ["pre_created", "full_access"])
 @pytest.mark.parametrize("userinfo", [USERINFO])
 @pytest.mark.parametrize(
     "existing_entries,removed_from",
     [
         ([LDAP_TESTGROUP_ENTRY, LDAP_GROUP1_ENTRY, LDAP_GROUP2_ENTRY], ["testgroup"]),
         (
-            [LDAP_USER_ENTRY, LDAP_TESTGROUP_ENTRY, LDAP_GROUP1_ENTRY, LDAP_GROUP2_ENTRY],
+            [
+                LDAP_USER_ENTRY,
+                LDAP_TESTGROUP_ENTRY,
+                LDAP_GROUP1_ENTRY,
+                LDAP_GROUP2_ENTRY,
+            ],
             ["testgroup"],
         ),
         (
             [
                 LDAP_USER_ENTRY,
                 LDAP_PRECREATED_TESTGROUP_ENTRY,
                 LDAP_GROUP1_ENTRY,
@@ -490,15 +507,17 @@
         ),
     ],
 )
 @pytest.mark.parametrize("supplementary_group_names", [["group1", "group2"], []])
 def test_mod_user_success(ldap_mod_entry, userinfo, removed_from):
     added, removed = ldap_mod_entry["user"].mod(ldap_mod_entry["supplementary_groups"])
 
-    assert set(added) == set([grp.name for grp in ldap_mod_entry["supplementary_groups"]])
+    assert set(added) == set(
+        [grp.name for grp in ldap_mod_entry["supplementary_groups"]]
+    )
     assert set(removed) == set(removed_from)
 
     for group in ldap_mod_entry["supplementary_groups"]:
         members = group.get_ldap_entry().get("memberUid") or []
         assert userinfo["username"] in members
         assert userinfo["username"] in members
```

### Comparing `feudalAdapter-0.5.4/tests/backend/local_unix.py` & `feudalAdapter-0.6.0/tests/backend/local_unix.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,18 @@
         else:
             new_command = command
         return old_subprocess_run(new_command, *args[1:], **kwargs)
 
     with monkeypatch.context() as mp:
         # patch root used by local_unix.User and subprocess.run to use this root for creating users
         mp.setattr("subprocess.run", mock_subprocess_run)
-        mp.setattr("ldf_adapter.backend.local_unix.CONFIG.backend.local_unix.shell", "/bin/bash")
+        mp.setattr(
+            "ldf_adapter.backend.local_unix.CONFIG.backend.local_unix.shell",
+            "/bin/bash",
+        )
         mp.setattr("ldf_adapter.backend.local_unix.User.ROOT", mock_root)
         mp.setattr("ldf_adapter.backend.local_unix.Group.ROOT", mock_root)
         if input.get("home_base"):
             mp.setattr(
                 "ldf_adapter.backend.local_unix.CONFIG.backend.local_unix.home_base",
                 input["home_base"].rstrip("/"),
             )
@@ -65,15 +68,17 @@
         (Path(mock_root()) / "etc" / "shadow").touch()
         if exists:
             (Path(mock_root()) / "etc" / "passwd").write_text(input["passwd_entry"])
         elif taken:
             (Path(mock_root()) / "etc" / "passwd").write_text(input["passwd_taken"])
         (Path(mock_root()) / "etc" / "group").write_text(input["group_entry"])
         # init service user from unix backend
-        service_user = ldf_adapter.backend.local_unix.User(MockUserInfo(input["userinfo"]))
+        service_user = ldf_adapter.backend.local_unix.User(
+            MockUserInfo(input["userinfo"])
+        )
         yield service_user
         # clean up files
         old_subprocess_run(["rm", "-rf", mock_root()])
 
 
 @pytest.fixture(scope="function")
 def local_unix_group(input, exists, monkeypatch):
@@ -161,15 +166,18 @@
 }
 
 
 @pytest.mark.parametrize("input,exists,taken", [(INPUT_UNIX, False, False)])
 def test_create(local_unix_user, input):
     """Test that create method adds the appropriate entry in /etc/passwd."""
     local_unix_user.create()
-    assert input["passwd_entry"] in (Path(input["new_root"]) / "etc" / "passwd").read_text()
+    assert (
+        input["passwd_entry"]
+        in (Path(input["new_root"]) / "etc" / "passwd").read_text()
+    )
 
 
 @pytest.mark.parametrize("input,exists,taken", [(INPUT_UNIX, False, True)])
 def test_create_taken(local_unix_user, input):
     """Test that create raises a Failure if the username is already taken.
     User's primary group needs to exist.
     """
@@ -177,23 +185,27 @@
         local_unix_user.create()
 
 
 @pytest.mark.parametrize("input,exists,taken", [(INPUT_CUSTOM_HOME_BASE, False, False)])
 def test_create_custom_home_base(local_unix_user, input):
     """Test that create method adds the appropriate entry in /etc/passwd with custom home dir"""
     local_unix_user.create()
-    assert input["passwd_entry"] in (Path(input["new_root"]) / "etc" / "passwd").read_text()
+    assert (
+        input["passwd_entry"]
+        in (Path(input["new_root"]) / "etc" / "passwd").read_text()
+    )
 
 
 @pytest.mark.parametrize(
     "input,exists,taken", [(INPUT_UNIX, False, False), (INPUT_UNIX, False, True)]
 )
 def test_doesnt_exist(local_unix_user):
     """Tests that exists returns False on a clean system, or even if username is taken by another user.
-    (i.e. username exists, but the gecos field does not contain this user's unique_id)."""
+    (i.e. username exists, but the gecos field does not contain this user's unique_id).
+    """
     assert not local_unix_user.exists()
 
 
 @pytest.mark.parametrize("input,exists,taken", [(INPUT_UNIX, True, False)])
 def test_exists(local_unix_user, input):
     """Tests that exists returns True if there is an entry in passwd for this unique_id."""
     assert local_unix_user.exists()
@@ -224,15 +236,17 @@
 
 
 @pytest.mark.parametrize("input,exists,taken", [(INPUT_UNIX, False, False)])
 def test_get_username_different(local_unix_user, input):
     """Tests that get_username returns the username in passwd.
     Case 2: username in userinfo is different than the one in passwd.
     """
-    passwd_mapped = "testuser2:x:1000:1000:subuid@issuer.domain:/home/testuser:/bin/bash"
+    passwd_mapped = (
+        "testuser2:x:1000:1000:subuid@issuer.domain:/home/testuser:/bin/bash"
+    )
     (Path(input["new_root"]) / "etc" / "passwd").write_text(passwd_mapped)
     assert local_unix_user.get_username() == "testuser2"
 
 
 @pytest.mark.parametrize(
     "input,exists,taken", [(INPUT_UNIX, False, False), (INPUT_UNIX, False, True)]
 )
@@ -274,25 +288,29 @@
 }
 
 
 @pytest.mark.parametrize("input,exists", [(INPUT_UNIX_GROUP, False)])
 def test_group_create(local_unix_group, input):
     """Test that create method adds the appropriate entry in /etc/group."""
     local_unix_group.create()
-    assert input["group_entry"] in (Path(input["new_root"]) / "etc" / "group").read_text()
+    assert (
+        input["group_entry"] in (Path(input["new_root"]) / "etc" / "group").read_text()
+    )
 
 
 @pytest.mark.parametrize("input,exists", [(INPUT_UNIX_GROUP, True)])
 def test_group_create_exists(local_unix_group):
     """Test that create raises a Failure if the group exists."""
     with pytest.raises(Failure):
         local_unix_group.create()
 
 
-@pytest.mark.parametrize("input,exists", [(INPUT_UNIX_GROUP, False), (INPUT_UNIX_GROUP, True)])
+@pytest.mark.parametrize(
+    "input,exists", [(INPUT_UNIX_GROUP, False), (INPUT_UNIX_GROUP, True)]
+)
 def test_group_exist(local_unix_group, exists):
     """Tests that exists returns True if there is an entry for the given name,
     and False otherwise.
     """
     assert local_unix_group.exists() == exists
 
 
@@ -339,15 +357,18 @@
     ),  # all other special chars replaced with _, when first char is special
     (
         "u#%^&()=+[]{}\\|;:'\",<.>/?",
         "u________________________",
     ),  # all other special chars replaced with _, when first char is a letter
     ("\u5317\u4EB0", "bei_jing_"),  # unicode
     ("\u20AC", "eur"),  # unicode
-    ("user$", "users"),  # $ replaced with s even ar the end (although valid shadow name)
+    (
+        "user$",
+        "users",
+    ),  # $ replaced with s even ar the end (although valid shadow name)
     ("-user", "_user"),  # - as first character replaced with _
     (
         "-aaaaaaaaaaaaaaaaaaaaaaaaaaaaaa",
         "_aaaaaaaaaaaaaaaaaaaaaaaaaaaaaa",
     ),  # - as first character replaced with _
     # from here on, length > 32 needs to be shortened to 32; fragments are defined as substrings separated by _
     (
@@ -462,8 +483,10 @@
 }
 
 
 @pytest.mark.parametrize("input,exists", [(INPUT_UNIX_GROUP_PUNCH, False)])
 def test_create_group_punch4nfdi_enabled(local_unix_group, input):
     """Test that create method adds the appropriate entry in /etc/group when punch4nfdi flag is enabled."""
     local_unix_group.create()
-    assert input["group_entry"] in (Path(input["new_root"]) / "etc" / "group").read_text()
+    assert (
+        input["group_entry"] in (Path(input["new_root"]) / "etc" / "group").read_text()
+    )
```

### Comparing `feudalAdapter-0.5.4/tests/eduperson.py` & `feudalAdapter-0.6.0/tests/eduperson.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,21 +2,30 @@
 
 from ldf_adapter.eduperson import Entitlement
 
 
 @pytest.mark.parametrize(
     "raw,group",
     [
-        ("urn:nid:namespace:group:group:subgroup1:subgroup2:role=admin#authority", "group"),
-        ("urn:geant:h-df.de:group:IMK-TRO-EWCC#login.helmholtz-data-federation.de", "IMK-TRO-EWCC"),
+        (
+            "urn:nid:namespace:group:group:subgroup1:subgroup2:role=admin#authority",
+            "group",
+        ),
+        (
+            "urn:geant:h-df.de:group:IMK-TRO-EWCC#login.helmholtz-data-federation.de",
+            "IMK-TRO-EWCC",
+        ),
         (
             "urn:geant:h-df.de:group:MyExampleColab#login.helmholtz-data-federation.de",
             "MyExampleColab",
         ),
-        ("urn:geant:h-df.de:group:wlcg-test#login.helmholtz-data-federation.de", "wlcg-test"),
+        (
+            "urn:geant:h-df.de:group:wlcg-test#login.helmholtz-data-federation.de",
+            "wlcg-test",
+        ),
         ("urn:geant:h-df.de:group:HDF#login.helmholtz-data-federation.de", "HDF"),
     ],
 )
 def test_entitlement_group(raw, group):
     ent = Entitlement(raw)
     assert ent.group == group
 
@@ -36,46 +45,70 @@
     ent = Entitlement(raw)
     assert ent.subgroups == subgroup
 
 
 @pytest.mark.parametrize(
     "raw,full_namespace",
     [
-        ("urn:nid:namespace:group:group:subgroup1:subgroup2:role=admin#authority", ["namespace"]),
+        (
+            "urn:nid:namespace:group:group:subgroup1:subgroup2:role=admin#authority",
+            ["namespace"],
+        ),
         (
             "urn:nid:ns1:ns2:ns3:group:group:subgroup1:subgroup2:role=admin#authority",
             ["ns1", "ns2", "ns3"],
         ),
-        ("urn:geant:h-df.de:group:IMK-TRO-EWCC#login.helmholtz-data-federation.de", ["h-df.de"]),
+        (
+            "urn:geant:h-df.de:group:IMK-TRO-EWCC#login.helmholtz-data-federation.de",
+            ["h-df.de"],
+        ),
     ],
 )
 def test_entitlement_full_namespace(raw, full_namespace):
     ent = Entitlement(raw)
     assert ent.full_namespace == full_namespace
 
 
 @pytest.mark.parametrize(
     "raw,namespace_id",
     [
-        ("urn:nid:namespace:group:group:subgroup1:subgroup2:role=admin#authority", "nid"),
-        ("urn:nid:ns1:ns2:ns3:group:group:subgroup1:subgroup2:role=admin#authority", "nid"),
-        ("urn:geant:h-df.de:group:IMK-TRO-EWCC#login.helmholtz-data-federation.de", "geant"),
+        (
+            "urn:nid:namespace:group:group:subgroup1:subgroup2:role=admin#authority",
+            "nid",
+        ),
+        (
+            "urn:nid:ns1:ns2:ns3:group:group:subgroup1:subgroup2:role=admin#authority",
+            "nid",
+        ),
+        (
+            "urn:geant:h-df.de:group:IMK-TRO-EWCC#login.helmholtz-data-federation.de",
+            "geant",
+        ),
     ],
 )
 def test_entitlement_namespace_id(raw, namespace_id):
     ent = Entitlement(raw)
     assert ent.namespace_id == namespace_id
 
 
 @pytest.mark.parametrize(
     "raw,delegated_namespace",
     [
-        ("urn:nid:namespace:group:group:subgroup1:subgroup2:role=admin#authority", "namespace"),
-        ("urn:nid:ns1:ns2:ns3:group:group:subgroup1:subgroup2:role=admin#authority", "ns1"),
-        ("urn:geant:h-df.de:group:IMK-TRO-EWCC#login.helmholtz-data-federation.de", "h-df.de"),
+        (
+            "urn:nid:namespace:group:group:subgroup1:subgroup2:role=admin#authority",
+            "namespace",
+        ),
+        (
+            "urn:nid:ns1:ns2:ns3:group:group:subgroup1:subgroup2:role=admin#authority",
+            "ns1",
+        ),
+        (
+            "urn:geant:h-df.de:group:IMK-TRO-EWCC#login.helmholtz-data-federation.de",
+            "h-df.de",
+        ),
     ],
 )
 def test_entitlement_delegated_namespace(raw, delegated_namespace):
     ent = Entitlement(raw)
     assert ent.delegated_namespace == delegated_namespace
 
 
@@ -94,28 +127,40 @@
     ent = Entitlement(raw)
     assert ent.subnamespaces == subnamespaces
 
 
 @pytest.mark.parametrize(
     "raw,role",
     [
-        ("urn:nid:namespace:group:group:subgroup1:subgroup2:role=admin#authority", "admin"),
-        ("urn:nid:namespace:group:group:subgroup1:subgroup2:role=user#authority", "user"),
-        ("urn:geant:h-df.de:group:IMK-TRO-EWCC#login.helmholtz-data-federation.de", None),
+        (
+            "urn:nid:namespace:group:group:subgroup1:subgroup2:role=admin#authority",
+            "admin",
+        ),
+        (
+            "urn:nid:namespace:group:group:subgroup1:subgroup2:role=user#authority",
+            "user",
+        ),
+        (
+            "urn:geant:h-df.de:group:IMK-TRO-EWCC#login.helmholtz-data-federation.de",
+            None,
+        ),
     ],
 )
 def test_entitlement_role(raw, role):
     ent = Entitlement(raw)
     assert ent.role == role
 
 
 @pytest.mark.parametrize(
     "raw,group_authority",
     [
-        ("urn:nid:namespace:group:group:subgroup1:subgroup2:role=admin#authority", "authority"),
+        (
+            "urn:nid:namespace:group:group:subgroup1:subgroup2:role=admin#authority",
+            "authority",
+        ),
         ("urn:nid:ns1:ns2:ns3:group:group:subgroup1:subgroup2:role=admin#.", "."),
         (
             "urn:geant:h-df.de:group:IMK-TRO-EWCC#login.helmholtz-data-federation.de",
             "login.helmholtz-data-federation.de",
         ),
     ],
 )
```

### Comparing `feudalAdapter-0.5.4/tests/feudal_adapter.conf` & `feudalAdapter-0.6.0/tests/feudal_adapter.conf`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.4/tests/name_generators.py` & `feudalAdapter-0.6.0/tests/name_generators.py`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.4/tests/settings.py` & `feudalAdapter-0.6.0/tests/settings.py`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.4/tests/user.py` & `feudalAdapter-0.6.0/tests/user.py`

 * *Files 19% similar despite different names*

```diff
@@ -172,14 +172,17 @@
 
     def limit(self):
         MOCK_DB.users[self.unique_id].limited = True
 
     def unlimit(self):
         MOCK_DB.users[self.unique_id].limited = False
 
+    def execute(self, hook, *hook_args):
+        pass
+
 
 class MockBackendGroup:
     def __init__(self, name):
         self.name = name
 
     def exists(self):
         return MOCK_DB.has_group(name=self.name)
@@ -223,15 +226,18 @@
 )
 def test_assurance_verifier(user, assurance_verified):
     assert user.assurance_verifier()(user.data.assurance) == assurance_verified
 
 
 @pytest.mark.parametrize("data", settings.ALL_INPUT)
 def test_get_status(user):
-    assert user.get_status().attributes == {"state": "not_deployed", "message": "No message"}
+    assert user.get_status().attributes == {
+        "state": "not_deployed",
+        "message": "No message",
+    }
 
 
 @pytest.mark.parametrize("data", [settings.INPUT_EGI])
 def test_deploy_fails_no_primary_group(user):
     with pytest.raises(SystemExit):
         user.deploy()
 
@@ -246,15 +252,18 @@
     ],
 )
 def test_deploy_name_taken(user, username, monkeypatch):
     monkeypatch.setattr(
         MockBackendUser, "name_taken", lambda x, n: True if n == "marcus" else False
     )
     assert user.deploy().attributes["state"] == "deployed"
-    assert user.get_status().attributes == {"state": "deployed", "message": f"username {username}"}
+    assert user.get_status().attributes == {
+        "state": "deployed",
+        "message": f"username {username}",
+    }
 
 
 @pytest.mark.parametrize(
     "data,username",
     [
         (settings.INPUT_UNITY, "marcus"),
         (settings.INPUT_DEEP_IAM, "marcus"),
@@ -262,195 +271,283 @@
         (settings.INPUT_KIT, "lo0018"),
     ],
 )
 def test_deploy(user, username):
     result = user.deploy()
     assert result.attributes["state"] == "deployed"
     assert result.attributes["message"].startswith("User was created")
-    assert user.get_status().attributes == {"state": "deployed", "message": f"username {username}"}
+    assert user.get_status().attributes == {
+        "state": "deployed",
+        "message": f"username {username}",
+    }
 
 
 # test deploy_pooled_user
 # test deploy groups
 # test deploy group changes
 
 
 @pytest.mark.parametrize(
     "data",
-    [settings.INPUT_UNITY, settings.INPUT_DEEP_IAM, settings.INPUT_INDIGO_IAM, settings.INPUT_KIT],
+    [
+        settings.INPUT_UNITY,
+        settings.INPUT_DEEP_IAM,
+        settings.INPUT_INDIGO_IAM,
+        settings.INPUT_KIT,
+    ],
 )
 def test_suspend(user):
     user.deploy()
     assert user.suspend().attributes["state"] == "suspended"
     assert user.get_status().attributes["state"] == "suspended"
 
 
 @pytest.mark.parametrize(
     "data",
-    [settings.INPUT_UNITY, settings.INPUT_DEEP_IAM, settings.INPUT_INDIGO_IAM, settings.INPUT_KIT],
+    [
+        settings.INPUT_UNITY,
+        settings.INPUT_DEEP_IAM,
+        settings.INPUT_INDIGO_IAM,
+        settings.INPUT_KIT,
+    ],
 )
 def test_suspend_not_deployed(user):
     assert user.suspend().attributes["state"] == "not_deployed"
     assert user.get_status().attributes["state"] == "not_deployed"
 
 
 @pytest.mark.parametrize(
     "data",
-    [settings.INPUT_UNITY, settings.INPUT_DEEP_IAM, settings.INPUT_INDIGO_IAM, settings.INPUT_KIT],
+    [
+        settings.INPUT_UNITY,
+        settings.INPUT_DEEP_IAM,
+        settings.INPUT_INDIGO_IAM,
+        settings.INPUT_KIT,
+    ],
 )
 def test_resume_after_suspend(user):
     user.deploy()
     user.suspend()
     assert user.resume().attributes["state"] == "deployed"
     assert user.get_status().attributes["state"] == "deployed"
 
 
 @pytest.mark.parametrize(
     "data",
-    [settings.INPUT_UNITY, settings.INPUT_DEEP_IAM, settings.INPUT_INDIGO_IAM, settings.INPUT_KIT],
+    [
+        settings.INPUT_UNITY,
+        settings.INPUT_DEEP_IAM,
+        settings.INPUT_INDIGO_IAM,
+        settings.INPUT_KIT,
+    ],
 )
 def test_resume_not_suspended(user):
     user.deploy()
     assert user.resume().attributes["state"] == "deployed"
     assert user.get_status().attributes["state"] == "deployed"
 
 
 @pytest.mark.parametrize(
     "data",
-    [settings.INPUT_UNITY, settings.INPUT_DEEP_IAM, settings.INPUT_INDIGO_IAM, settings.INPUT_KIT],
+    [
+        settings.INPUT_UNITY,
+        settings.INPUT_DEEP_IAM,
+        settings.INPUT_INDIGO_IAM,
+        settings.INPUT_KIT,
+    ],
 )
 def test_suspend_after_limit(user):
     user.deploy()
     user.limit()
     assert user.suspend().attributes["state"] == "suspended"
     assert user.get_status().attributes["state"] == "suspended"
 
 
 @pytest.mark.parametrize(
     "data",
-    [settings.INPUT_UNITY, settings.INPUT_DEEP_IAM, settings.INPUT_INDIGO_IAM, settings.INPUT_KIT],
+    [
+        settings.INPUT_UNITY,
+        settings.INPUT_DEEP_IAM,
+        settings.INPUT_INDIGO_IAM,
+        settings.INPUT_KIT,
+    ],
 )
 def test_resume_after_limit(user):
     user.deploy()
     user.limit()
     assert user.resume().attributes["state"] == "limited"
     assert user.get_status().attributes["state"] == "limited"
 
 
 @pytest.mark.parametrize(
     "data",
-    [settings.INPUT_UNITY, settings.INPUT_DEEP_IAM, settings.INPUT_INDIGO_IAM, settings.INPUT_KIT],
+    [
+        settings.INPUT_UNITY,
+        settings.INPUT_DEEP_IAM,
+        settings.INPUT_INDIGO_IAM,
+        settings.INPUT_KIT,
+    ],
 )
 def test_limit(user):
     user.deploy()
     assert user.limit().attributes["state"] == "limited"
     assert user.get_status().attributes["state"] == "limited"
 
 
 @pytest.mark.parametrize(
     "data",
-    [settings.INPUT_UNITY, settings.INPUT_DEEP_IAM, settings.INPUT_INDIGO_IAM, settings.INPUT_KIT],
+    [
+        settings.INPUT_UNITY,
+        settings.INPUT_DEEP_IAM,
+        settings.INPUT_INDIGO_IAM,
+        settings.INPUT_KIT,
+    ],
 )
 def test_limit_not_deployed(user):
     assert user.limit().attributes["state"] == "not_deployed"
     assert user.get_status().attributes["state"] == "not_deployed"
 
 
 @pytest.mark.parametrize(
     "data",
-    [settings.INPUT_UNITY, settings.INPUT_DEEP_IAM, settings.INPUT_INDIGO_IAM, settings.INPUT_KIT],
+    [
+        settings.INPUT_UNITY,
+        settings.INPUT_DEEP_IAM,
+        settings.INPUT_INDIGO_IAM,
+        settings.INPUT_KIT,
+    ],
 )
 def test_unlimit(user):
     user.deploy()
     user.limit()
     assert user.unlimit().attributes["state"] == "deployed"
     assert user.get_status().attributes["state"] == "deployed"
 
 
 @pytest.mark.parametrize(
     "data",
-    [settings.INPUT_UNITY, settings.INPUT_DEEP_IAM, settings.INPUT_INDIGO_IAM, settings.INPUT_KIT],
+    [
+        settings.INPUT_UNITY,
+        settings.INPUT_DEEP_IAM,
+        settings.INPUT_INDIGO_IAM,
+        settings.INPUT_KIT,
+    ],
 )
 def test_unlimit_not_limited(user):
     user.deploy()
     assert user.unlimit().attributes["state"] == "deployed"
     assert user.get_status().attributes["state"] == "deployed"
 
 
 @pytest.mark.parametrize(
     "data",
-    [settings.INPUT_UNITY, settings.INPUT_DEEP_IAM, settings.INPUT_INDIGO_IAM, settings.INPUT_KIT],
+    [
+        settings.INPUT_UNITY,
+        settings.INPUT_DEEP_IAM,
+        settings.INPUT_INDIGO_IAM,
+        settings.INPUT_KIT,
+    ],
 )
 def test_limit_after_suspend(user):
     user.deploy()
     user.suspend()
     assert user.limit().attributes["state"] == "suspended"
     assert user.get_status().attributes["state"] == "suspended"
 
 
 @pytest.mark.parametrize(
     "data",
-    [settings.INPUT_UNITY, settings.INPUT_DEEP_IAM, settings.INPUT_INDIGO_IAM, settings.INPUT_KIT],
+    [
+        settings.INPUT_UNITY,
+        settings.INPUT_DEEP_IAM,
+        settings.INPUT_INDIGO_IAM,
+        settings.INPUT_KIT,
+    ],
 )
 def test_unlimit_after_limit_and_suspend(user):
     user.deploy()
     user.suspend()
     user.limit()
     assert user.unlimit().attributes["state"] == "suspended"
     assert user.get_status().attributes["state"] == "suspended"
 
 
 @pytest.mark.parametrize(
     "data",
-    [settings.INPUT_UNITY, settings.INPUT_DEEP_IAM, settings.INPUT_INDIGO_IAM, settings.INPUT_KIT],
+    [
+        settings.INPUT_UNITY,
+        settings.INPUT_DEEP_IAM,
+        settings.INPUT_INDIGO_IAM,
+        settings.INPUT_KIT,
+    ],
 )
 def test_undeploy_doesnt_exist(user):
     result = user.undeploy()
     assert result.attributes["state"] == "not_deployed"
     assert result.attributes["message"].startswith("No user for")
     assert user.get_status().attributes["state"] == "not_deployed"
 
 
 @pytest.mark.parametrize(
     "data",
-    [settings.INPUT_UNITY, settings.INPUT_DEEP_IAM, settings.INPUT_INDIGO_IAM, settings.INPUT_KIT],
+    [
+        settings.INPUT_UNITY,
+        settings.INPUT_DEEP_IAM,
+        settings.INPUT_INDIGO_IAM,
+        settings.INPUT_KIT,
+    ],
 )
 def test_undeploy(user):
     user.deploy()
     result = user.undeploy()
     assert result.attributes["state"] == "not_deployed"
     assert result.attributes["message"].endswith("was removed.")
     assert user.get_status().attributes["state"] == "not_deployed"
 
 
 @pytest.mark.parametrize(
     "data",
-    [settings.INPUT_UNITY, settings.INPUT_DEEP_IAM, settings.INPUT_INDIGO_IAM, settings.INPUT_KIT],
+    [
+        settings.INPUT_UNITY,
+        settings.INPUT_DEEP_IAM,
+        settings.INPUT_INDIGO_IAM,
+        settings.INPUT_KIT,
+    ],
 )
 def test_undeploy_after_suspend(user):
     user.deploy()
     user.suspend()
     assert user.undeploy().attributes["state"] == "not_deployed"
     assert user.get_status().attributes["state"] == "not_deployed"
 
 
 @pytest.mark.parametrize(
     "data",
-    [settings.INPUT_UNITY, settings.INPUT_DEEP_IAM, settings.INPUT_INDIGO_IAM, settings.INPUT_KIT],
+    [
+        settings.INPUT_UNITY,
+        settings.INPUT_DEEP_IAM,
+        settings.INPUT_INDIGO_IAM,
+        settings.INPUT_KIT,
+    ],
 )
 def test_undeploy_after_limit(user):
     user.deploy()
     user.limit()
     assert user.undeploy().attributes["state"] == "not_deployed"
     assert user.get_status().attributes["state"] == "not_deployed"
 
 
 @pytest.mark.parametrize(
     "data",
-    [settings.INPUT_UNITY, settings.INPUT_DEEP_IAM, settings.INPUT_INDIGO_IAM, settings.INPUT_KIT],
+    [
+        settings.INPUT_UNITY,
+        settings.INPUT_DEEP_IAM,
+        settings.INPUT_INDIGO_IAM,
+        settings.INPUT_KIT,
+    ],
 )
 def test_deploy_exists(user):
     user.deploy()
     result = user.deploy()
     assert result.attributes["state"] == "deployed"
     assert result.attributes["message"].startswith("User already existed")
     assert user.get_status().attributes["state"] == "deployed"
```

### Comparing `feudalAdapter-0.5.4/tests/userinfo.py` & `feudalAdapter-0.6.0/tests/userinfo.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,17 @@
     ],
 )
 def test_sub_masked_for_bwidm_eppn_rnd(sub):
     info = UserInfo({"user": {"userinfo": {"sub": sub}}})
     assert info._sub_masked_for_bwidm_eppn() == "".join(repeat("-", 80))
 
 
-@pytest.mark.parametrize("iss", ["example.org", "http://example.org", "https://example.org"])
+@pytest.mark.parametrize(
+    "iss", ["example.org", "http://example.org", "https://example.org"]
+)
 def test_iss_masked_for_bwidm_eppn_fixes_prefix(iss):
     info = UserInfo({"user": {"userinfo": {"iss": iss}}})
     assert info._iss_masked_for_bwidm_eppn() == "example.org"
 
 
 @pytest.mark.parametrize(
     "raw,cooked",
```

### Comparing `feudalAdapter-0.5.4/tox.ini` & `feudalAdapter-0.6.0/tox.ini`

 * *Files 13% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 [testenv:pylint]
 deps = pylint>=2.6
 commands =
     pylint -E {[base]module}
 
 [testenv:black]
 deps = black
-commands = black -l 100 --check --diff {[base]module}
+commands = black --check --diff {[base]module}
 
 [testenv:pyright]
 deps =
         {[base]deps}
         pyright
 commands = pyright {[base]module}
```

