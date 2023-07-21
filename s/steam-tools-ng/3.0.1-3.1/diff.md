# Comparing `tmp/steam-tools-ng-3.0.1.tar.gz` & `tmp/steam-tools-ng-3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "steam-tools-ng-3.0.1.tar", last modified: Sat Apr 15 21:17:06 2023, max compression
+gzip compressed data, was "steam-tools-ng-3.1.tar", last modified: Fri Jul 21 18:46:33 2023, max compression
```

## Comparing `steam-tools-ng-3.0.1.tar` & `steam-tools-ng-3.1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:17:06.851235 steam-tools-ng-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-04-15 21:17:06.851235 steam-tools-ng-3.0.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     3438 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:17:06.847234 steam-tools-ng-3.0.1/i18n/
--rw-r--r--   0 runner    (1001) docker     (123)    35901 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/i18n/fr.po
--rwxr-xr-x   0 runner    (1001) docker     (123)    45277 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/i18n/pt_BR.po
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 21:17:06.851235 steam-tools-ng-3.0.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     6250 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:17:06.847234 steam-tools-ng-3.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:17:06.847234 steam-tools-ng-3.0.1/src/steam_tools_ng/
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      788 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    10618 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:17:06.847234 steam-tools-ng-3.0.1/src/steam_tools_ng/console/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/console/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/console/authenticator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7993 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/console/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8708 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/console/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/console/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:17:06.851235 steam-tools-ng-3.0.1/src/steam_tools_ng/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11325 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/core/cardfarming.py
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/core/confirmations.py
--rw-r--r--   0 runner    (1001) docker     (123)     6863 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/core/coupons.py
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/core/fakerun.py
--rw-r--r--   0 runner    (1001) docker     (123)     8914 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/core/steamgifts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/core/steamguard.py
--rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/core/steamtrades.py
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:17:06.851235 steam-tools-ng-3.0.1/src/steam_tools_ng/gtk/
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/gtk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/gtk/about.py
--rw-r--r--   0 runner    (1001) docker     (123)    14992 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/gtk/application.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/gtk/async_gtk.py
--rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/gtk/authenticator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/gtk/confirmation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10369 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/gtk/coupon.py
--rw-r--r--   0 runner    (1001) docker     (123)    14558 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/gtk/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     7532 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/gtk/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    24019 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/gtk/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    38037 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/gtk/window.py
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/i18n.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:17:06.851235 steam-tools-ng-3.0.1/src/steam_tools_ng/icons/
--rw-r--r--   0 runner    (1001) docker     (123)   245142 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/icons/stng.ico
--rw-r--r--   0 runner    (1001) docker     (123)    97830 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/icons/stng.png
--rw-r--r--   0 runner    (1001) docker     (123)   231041 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/icons/stng_console.ico
--rw-r--r--   0 runner    (1001) docker     (123)    31925 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/icons/stng_console.png
--rw-r--r--   0 runner    (1001) docker     (123)   229900 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/icons/stng_nc.ico
--rw-r--r--   0 runner    (1001) docker     (123)    66900 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/icons/stng_nc.png
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/logger_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/src/steam_tools_ng/steam_api_executor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:17:06.847234 steam-tools-ng-3.0.1/src/steam_tools_ng.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-04-15 21:17:06.000000 steam-tools-ng-3.0.1/src/steam_tools_ng.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-15 21:17:06.000000 steam-tools-ng-3.0.1/src/steam_tools_ng.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 21:17:06.000000 steam-tools-ng-3.0.1/src/steam_tools_ng.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-15 21:17:06.000000 steam-tools-ng-3.0.1/src/steam_tools_ng.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-15 21:17:06.000000 steam-tools-ng-3.0.1/src/steam_tools_ng.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-15 21:17:06.000000 steam-tools-ng-3.0.1/src/steam_tools_ng.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/steam-tools-ng.desktop
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:17:06.851235 steam-tools-ng-3.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-15 21:16:53.000000 steam-tools-ng-3.0.1/tests/test_placeholder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:33.663149 steam-tools-ng-3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-07-21 18:46:33.663149 steam-tools-ng-3.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3438 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:33.655149 steam-tools-ng-3.1/i18n/
+-rw-r--r--   0 runner    (1001) docker     (123)    35901 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/i18n/fr.po
+-rwxr-xr-x   0 runner    (1001) docker     (123)    45277 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/i18n/pt_BR.po
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 18:46:33.663149 steam-tools-ng-3.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6010 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:33.651148 steam-tools-ng-3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:33.655149 steam-tools-ng-3.1/src/steam_tools_ng/
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      788 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10598 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:33.655149 steam-tools-ng-3.1/src/steam_tools_ng/console/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/console/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6221 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/console/authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8338 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/console/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6948 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/console/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/console/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:33.659149 steam-tools-ng-3.1/src/steam_tools_ng/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9996 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/core/cardfarming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/core/confirmations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7445 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/core/coupons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/core/fakerun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8881 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/core/steamgifts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/core/steamguard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/core/steamtrades.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:33.659149 steam-tools-ng-3.1/src/steam_tools_ng/gtk/
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/gtk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/gtk/about.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15637 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/gtk/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/gtk/async_gtk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11015 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/gtk/authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7068 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/gtk/confirmation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9423 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/gtk/coupon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12574 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/gtk/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/gtk/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28209 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/gtk/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38713 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/gtk/window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/i18n.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:33.663149 steam-tools-ng-3.1/src/steam_tools_ng/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)   245142 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/icons/stng.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    97830 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/icons/stng.png
+-rw-r--r--   0 runner    (1001) docker     (123)   231041 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/icons/stng_console.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    31925 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/icons/stng_console.png
+-rw-r--r--   0 runner    (1001) docker     (123)   229900 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/icons/stng_nc.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    66900 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/icons/stng_nc.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/logger_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:33.655149 steam-tools-ng-3.1/src/steam_tools_ng.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-07-21 18:46:33.000000 steam-tools-ng-3.1/src/steam_tools_ng.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-21 18:46:33.000000 steam-tools-ng-3.1/src/steam_tools_ng.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 18:46:33.000000 steam-tools-ng-3.1/src/steam_tools_ng.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-21 18:46:33.000000 steam-tools-ng-3.1/src/steam_tools_ng.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 18:46:33.000000 steam-tools-ng-3.1/src/steam_tools_ng.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-21 18:46:33.000000 steam-tools-ng-3.1/src/steam_tools_ng.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-21 18:46:33.000000 steam-tools-ng-3.1/src/steam_tools_ng.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/steam-tools-ng.desktop
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:33.663149 steam-tools-ng-3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/tests/test_placeholder.py
```

### Comparing `steam-tools-ng-3.0.1/LICENSE` & `steam-tools-ng-3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.0.1/PKG-INFO` & `steam-tools-ng-3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: steam-tools-ng
-Version: 3.0.1
+Version: 3.1
 Summary: Steam Tools NG
 Author: Lara Maia
 Author-email: dev@lara.monster
 License: GPLv3
 Project-URL: homepage, https://github.com/calendulish/steam-tools-ng
 Project-URL: repository, https://github.com
 Project-URL: changelog, https://github.com/calendulish/steam-tools-ng/releases
 Keywords: steam,valve
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Games/Entertainment
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Environment :: X11 Applications :: GTK
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [STNG] Steam Tools NG (formerly Steam Tools)
 ========================================
```

### Comparing `steam-tools-ng-3.0.1/README.md` & `steam-tools-ng-3.1/README.md`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.0.1/i18n/fr.po` & `steam-tools-ng-3.1/i18n/fr.po`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.0.1/i18n/pt_BR.po` & `steam-tools-ng-3.1/i18n/pt_BR.po`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.0.1/pyproject.toml` & `steam-tools-ng-3.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 [build-system]
 requires = ["setuptools", "wheel", "certifi", "cx_Freeze; sys_platform == 'win32'"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "steam-tools-ng"
-version = "3.0.1"
+version = "3.1"
 description = "Steam Tools NG"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {text = "GPLv3"}
 keywords = ["steam", "valve"]
 authors = [{email = "dev@lara.monster"}, {name = "Lara Maia"}]
 classifiers = [
-  "Development Status :: 5 - Production/Stable",
+  "Development Status :: 4 - Beta",
   "Intended Audience :: End Users/Desktop",
   "Topic :: Games/Entertainment",
   "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
   "Operating System :: POSIX :: Linux",
   "Operating System :: Microsoft :: Windows :: Windows 10",
   "Environment :: X11 Applications :: GTK",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
   "Typing :: Typed"
 ]
 
 dependencies = [
   "pywin32; sys_platform == 'win32'",
-  "psutil; sys_platform == 'win32'",
-  "stlib~=1.3.0",
+  "stlib~=2.0",
   "stlib-plugins~=1.2.0",
   "aiohttp",
   "certifi"
 ]
 
 [project.urls]
 homepage = "https://github.com/calendulish/steam-tools-ng"
@@ -42,14 +42,15 @@
 
 [project.scripts]
 steam-tools-ng = "steam_tools_ng.cli:main"
 steam-tools-ng-gui = "steam_tools_ng.gui:main"
 
 [tool.setuptools]
 include-package-data = true
+zip-safe = false
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.distutils.build_exe]
 packages = ["steam_tools_ng", "stlib-plugins", "gi", "win32com.client"]
 excludes = [
```

### Comparing `steam-tools-ng-3.0.1/setup.py` & `steam-tools-ng-3.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,24 +12,24 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 # See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see http://www.gnu.org/licenses/.
 #
 
-import certifi
 import os
 import subprocess
 import sys
 import sysconfig
 from pathlib import Path
-from setuptools import find_packages
-from setuptools.command.build_py import build_py
 from typing import Any, List, Mapping, Tuple
 
+import certifi
+from setuptools.command.build_py import build_py
+
 if os.name == 'nt' and not os.getenv('NO_FREEZE'):
     # noinspection PyPackageRequirements
     from cx_Freeze import setup, Executable
 else:
     from setuptools import setup
 
 
@@ -69,22 +69,18 @@
         'GdkPixbuf-2.0',
         'GModule-2.0',
         'HarfBuzz-0.0',
         'Graphene-1.0',
         'freetype2-2.0',
     ]
 
-    includes = []
-
     if 'MSC ' in sys.version:
         # windows
         from gi.repository import Gtk
         lib_path = Path(Gtk.__path__[0]).parent.parent.resolve()
-        bin_path = lib_path.parent.resolve() / 'bin'
-
         required_dlls = [
             'gtk-4-1',
             'pango-1.0-0',
             'pangocairo-1.0-0',
             'pangowin32-1.0-0',
             'Rsvg-2.0-vs17',
             'graphene-1.0-0',
@@ -93,16 +89,14 @@
 
         pixbuf_loaders = [
             'libpixbufloader-svg',
         ]
     else:
         # mingw
         lib_path = Path(sysconfig.get_path('platlib')).parent.parent.resolve()
-        bin_path = lib_path.parent.resolve() / 'bin'
-
         required_dlls = [
             'libgtk-4-1',
             'libpango-1.0-0',
             'libpangocairo-1.0-0',
             'libpangowin32-1.0-0',
             'librsvg-2-2',
             'libgraphene-1.0-0',
@@ -110,42 +104,45 @@
         ]
 
         pixbuf_loaders = [
             'libpixbufloader-png',
             'libpixbufloader-svg',
         ]
 
-    for package in namespace_packages:
-        includes.append((
+    bin_path = lib_path.parent.resolve() / 'bin'
+
+    includes = [
+        (
             str(lib_path / 'girepository-1.0' / f'{package}.typelib'),
             str(Path('lib', 'girepository-1.0', f'{package}.typelib')),
-        ))
-
-    for dll in required_dlls:
-        includes.append((
-            str(bin_path / f'{dll}.dll'),
-            f'{dll}.dll',
-        ))
-
-    for loader in pixbuf_loaders:
-        includes.append((
+        )
+        for package in namespace_packages
+    ]
+    includes.extend(
+        (str(bin_path / f'{dll}.dll'), f'{dll}.dll') for dll in required_dlls
+    )
+    includes.extend(
+        (
             str(lib_path / 'gdk-pixbuf-2.0' / '2.10.0' / 'loaders' / f'{loader}.dll'),
             str(Path('lib', 'gdk-pixbuf-2.0', '2.10.0', 'loaders', f'{loader}.dll')),
-        ))
-
-    includes.append((
-        str(lib_path / 'gdk-pixbuf-2.0' / '2.10.0' / 'loaders.cache'),
-        str(Path('lib', 'gdk-pixbuf-2.0', '2.10.0', 'loaders.cache')),
-    ))
-
-    includes.append((
-        str(Path('src', 'steam_tools_ng', 'icons', 'settings.ini')),
-        str(Path('etc', 'gtk-4.0', 'settings.ini')),
-    ))
-
+        )
+        for loader in pixbuf_loaders
+    )
+    includes.extend(
+        (
+            (
+                str(lib_path / 'gdk-pixbuf-2.0' / '2.10.0' / 'loaders.cache'),
+                str(Path('lib', 'gdk-pixbuf-2.0', '2.10.0', 'loaders.cache')),
+            ),
+            (
+                str(Path('src', 'steam_tools_ng', 'icons', 'settings.ini')),
+                str(Path('etc', 'gtk-4.0', 'settings.ini')),
+            ),
+        )
+    )
     return includes
 
 
 def freeze_options() -> Mapping[str, Any]:
     if os.name != 'nt' or os.getenv('NO_FREEZE'):
         return {}
 
@@ -165,31 +162,26 @@
             Path("src", "steam_tools_ng", "gui.py"),
             target_name='steam-tools-ng-gui',
             base=None,
             icon=Path(icons_path, 'stng.ico'),
             shortcut_name='Steam Tools NG GUI',
             copyright=copyright_,
         ),
-        Executable(
-            Path("src", "steam_tools_ng", "steam_api_executor.py"),
-            target_name='steam-api-executor',
-            base=None,
-            copyright=copyright_,
-        )
     ]
 
     paths = ['src']
     paths.extend(sys.path)
 
     includes = [*fix_gtk(), (certifi.where(), Path('etc', 'cacert.pem'))]
 
-    for file in Path(icons_path, 'Default').iterdir():
-        if file != 'settings.ini':
-            includes.append((file, Path('share', 'icons', 'Default', file.name)))
-
+    includes.extend(
+        (file, Path('share', 'icons', 'Default', file.name))
+        for file in Path(icons_path, 'Default').iterdir()
+        if file != 'settings.ini'
+    )
     for language in ['fr', 'pt_BR']:
         language_directory = Path('lib', 'steam_tools_ng', 'locale', language, 'LC_MESSAGES')
         includes.append((
             Path('build', language_directory, 'steam-tools-ng.mo'),
             language_directory / 'steam-tools-ng.mo',
         ))
 
@@ -203,8 +195,9 @@
     }
 
     return {
         "options": options,
         "executables": executables,
     }
 
+
 setup(cmdclass={'build_py': BuildTranslations}, **freeze_options())
```

### Comparing `steam-tools-ng-3.0.1/src/steam_tools_ng/__init__.py` & `steam-tools-ng-3.1/src/steam_tools_ng/__init__.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.0.1/src/steam_tools_ng/__main__.py` & `steam-tools-ng-3.1/src/steam_tools_ng/__main__.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.0.1/src/steam_tools_ng/cli.py` & `steam-tools-ng-3.1/src/steam_tools_ng/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,20 +12,19 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 # See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see http://www.gnu.org/licenses/.
 #
 
-from multiprocessing import freeze_support
-
 import argparse
 import logging
 import sys
 import textwrap
+from multiprocessing import freeze_support
 from pathlib import Path
 
 from steam_tools_ng import config, i18n, __version__
 from steam_tools_ng.console import cli
 
 _ = i18n.get_translation
 log = logging.getLogger(__name__)
@@ -52,14 +51,28 @@
         metavar='<module>',
         action='store',
         nargs='?',
         help='Start a module',
     )
 
     command_parser.add_argument(
+        '--config-dir',
+        action='store_true',
+        help='Shows directory used to save config files',
+        dest='config_dir'
+    )
+
+    command_parser.add_argument(
+        '--log-dir',
+        action='store_true',
+        help='Shows directory used to save log files',
+        dest='log_dir',
+    )
+
+    command_parser.add_argument(
         '--reset',
         action='store_true',
         help='Clean up settings and log files',
         dest='reset',
     )
 
     command_parser.add_argument(
@@ -73,14 +86,21 @@
         '--add-authenticator',
         action='store_true',
         help='Use STNG as your Steam Authenticator',
         dest='add_authenticator',
     )
 
     command_parser.add_argument(
+        '--remove-authenticator',
+        action='store_true',
+        help='Remove STNG Autenticator from your account',
+        dest='remove_authenticator',
+    )
+
+    command_parser.add_argument(
         '-v', '--version',
         action='store_true',
         help='Show version',
         dest='version',
     )
 
     command_parser.add_argument(
@@ -93,14 +113,22 @@
     console_params = command_parser.parse_args()
     config.init_logger()
 
     if console_params.version:
         print(__version__)
         sys.exit(0)
 
+    if console_params.config_dir:
+        print(config.config_file_directory)
+        sys.exit(0)
+
+    if console_params.log_dir:
+        print(config.parser.get("logger", "log_directory"))
+        sys.exit(0)
+
     if console_params.reset:
         config.config_file.unlink(missing_ok=True)
         logging.root.removeHandler(logging.root.handlers[0])
 
         log_directory = config.parser.get("logger", "log_directory")
         Path(log_directory, 'steam-tools-ng.log').unlink()
         Path(log_directory, 'steam-tools-ng.log.1').unlink()
@@ -112,23 +140,23 @@
         config.new("login", "password", "")
         log.info(_('Done!'))
         sys.exit(0)
 
     print(f'Steam Tools NG version {__version__} (Made with Girl Power <33)')
     print('Copyright (C) 2015 ~ 2023 Lara Maia - <dev@lara.monster>')
 
-    if console_params.add_authenticator:
-        app = cli.SteamToolsNG('add_authenticator', '')
-        app.run()
-        sys.exit(0)
-
     if not console_params.module:
-        log.critical('No module has scheduled to run.')
-        log.critical("Use 'steam-tools-ng-gui' for the graphical user interface.")
-        sys.exit(1)
+        if console_params.add_authenticator:
+            console_params.module = "add_authenticator"
+        elif console_params.remove_authenticator:
+            console_params.module = "remove_authenticator"
+        else:
+            log.critical('No module has scheduled to run.')
+            log.critical("Use 'steam-tools-ng-gui' for the graphical user interface.")
+            sys.exit(1)
 
     module_name = console_params.module
     module_options = console_params.options
 
     app = cli.SteamToolsNG(module_name, module_options)
     app.run()
```

### Comparing `steam-tools-ng-3.0.1/src/steam_tools_ng/config.py` & `steam-tools-ng-3.1/src/steam_tools_ng/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,17 +185,16 @@
         'theme': 'light',
         'show_close_button': True,
         'language': str(locale.getdefaultlocale()[0]),
     },
     'login': {
         'steamid': 0,
         'deviceid': '',
-        'token': '',
-        'token_secure': '',
-        'oauth_token': '',
+        'refresh_token': '',
+        'access_token': '',
         'account_name': '',
         'shared_secret': '',
         'identity_secret': '',
         'password': '',
     },
 }
 
@@ -334,13 +333,13 @@
         with open(config_file, 'w', encoding="utf8") as config_file_object:
             parser.write(config_file_object)
     else:
         log.debug(_('Not saving {}:{} because values are already updated').format(section, option))
 
 
 def remove(section: str, option: str) -> None:
-    # Some GUI checks will fail if option doesn't exists
+    # Some GUI checks will fail if option doesn't exist
     new(section, option, '')
     # parser.remove_option(section, option)
 
     # with open(config_file, 'w', encoding="utf8") as config_file_object:
     #    parser.write(config_file_object)
```

### Comparing `steam-tools-ng-3.0.1/src/steam_tools_ng/console/authenticator.py` & `steam-tools-ng-3.1/src/steam_tools_ng/console/authenticator.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,77 +11,74 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 # See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see http://www.gnu.org/licenses/.
 #
-import aiohttp
 import asyncio
 import logging
 import sys
 from typing import Optional, TYPE_CHECKING
 
-from stlib import universe, webapi, login
+import aiohttp
+
+from stlib import universe, webapi
 from . import utils
 from .. import i18n, config
 
 if TYPE_CHECKING:
     from . import cli
 
 log = logging.getLogger(__name__)
 _ = i18n.get_translation
 
 
 # noinspection PyUnusedLocal
-class NewAuthenticator:
+class ManageAuthenticator:
     def __init__(self, cli_: 'cli.SteamToolsNG') -> None:
         self.cli = cli_
         self.webapi_session = webapi.SteamWebAPI.get_session(0)
-        self._login_data: Optional[login.LoginData] = None
+        self.authenticator_data: Optional[webapi.AuthenticatorData] = None
         self._sms_code = ''
 
     @property
     def sms_code(self) -> str:
         return self._sms_code
 
     @property
-    def oauth_token(self) -> str:
-        return config.parser.get("login", "oauth_token")
+    def access_token(self) -> str:
+        return config.parser.get("login", "access_token")
 
     @property
     def steamid(self) -> Optional[universe.SteamId]:
-        steamid = config.parser.getint("login", "steamid")
-
-        if steamid:
+        if steamid := config.parser.getint("login", "steamid"):
             try:
                 return universe.generate_steamid(steamid)
             except ValueError:
                 log.warning(_("SteamId is invalid"))
 
         return None
 
     async def add_authenticator(self) -> None:
         utils.set_console(info=_("Retrieving user data"))
 
-        if not self.oauth_token or not self.steamid:
+        if not self.access_token or not self.steamid:
             log.error(_(
                 "Some login data is missing. If the problem persists, run:\n"
                 "{} --reset"
             ).format(sys.argv[0]))
 
             self.cli.on_quit(1)
 
         assert isinstance(self.steamid, universe.SteamId)
-        oauth = {'steamid': self.steamid.id64, 'oauth_token': self.oauth_token}
-        login_data = login.LoginData(auth={}, oauth=oauth)
 
-        if not self._login_data or not self.sms_code:
+        if not self.authenticator_data or not self.sms_code:
             try:
-                self._login_data = await self.webapi_session.new_authenticator(self.steamid, self.oauth_token)
+                self.authenticator_data = await self.webapi_session.new_authenticator(self.steamid, self.access_token)
             except aiohttp.ClientError:
                 log.error(_("Check your connection. (server down?)"))
                 self.cli.on_quit(1)
             except webapi.AuthenticatorExists:
                 log.error(_(
                     "There's already an authenticator active for that account.\n"
                     "Remove your current steam authenticator and try again."
@@ -98,43 +95,75 @@
                 self.cli.on_quit(1)
             else:
                 user_input = utils.safe_input(_("Enter the code received by SMS"))
                 assert isinstance(user_input, str)
                 self._sms_code = user_input
 
         utils.set_console(info=_("Adding authenticator"))
-        assert isinstance(self._login_data, login.LoginData)
 
         try:
             await self.webapi_session.add_authenticator(
                 self.steamid,
-                self.oauth_token,
-                self._login_data.auth['shared_secret'],
+                self.access_token,
+                self.authenticator_data.shared_secret,
                 self.sms_code,
             )
         except webapi.SMSCodeError:
             log.error(_("Invalid SMS Code. Please, check the code and try again."))
             self.cli.on_quit(1)
         except aiohttp.ClientError:
             log.error(_("Check your connection. (server down?)"))
             self.cli.on_quit(1)
         except Exception as exception:
             log.critical("%s: %s", type(exception).__name__, str(exception))
             self.cli.on_quit(1)
 
         utils.set_console(info=_("Saving new secrets"))
-        config.new("login", "shared_secret", self._login_data.auth['shared_secret'])
-        config.new("login", "identity_secret", self._login_data.auth['identity_secret'])
+        config.new("login", "shared_secret", self.authenticator_data.shared_secret)
+        config.new("login", "identity_secret", self.authenticator_data.identity_secret)
         config.new("steamguard", "enable", True)
         config.new("confirmations", "enable", True)
 
         utils.set_console(info=_(
             "RECOVERY CODE\n\n"
             "You will need this code to recovery your Steam Account\n"
             "if you lose access to STNG Authenticator. So, write"
             "down this recovery code.\n\n"
             "YOU WILL NOT ABLE TO VIEW IT AGAIN!\n"
         ))
 
-        revocation_code = self._login_data.auth['revocation_code']
-        utils.set_console(info=revocation_code)
+        utils.set_console(info=self.authenticator_data.revocation_code)
         await asyncio.sleep(30)
+
+    async def remove_authenticator(self) -> None:
+        utils.set_console(info=_("Retrieving user data"))
+
+        if not self.access_token or not self.steamid:
+            log.error(_(
+                "Some login data is missing. If the problem persists, run:\n"
+                "{} --reset"
+            ).format(sys.argv[0]))
+
+            self.cli.on_quit(1)
+
+        user_input = utils.safe_input(_("Enter the revocation code"))
+        assert isinstance(user_input, str)
+
+        utils.set_console(info=_("Removing authenticator"))
+
+        try:
+            removed = await self.webapi_session.remove_authenticator(
+                self.steamid,
+                self.access_token,
+                user_input,
+            )
+        except aiohttp.ClientError:
+            log.error(_("Check your connection. (server down?)"))
+            self.cli.on_quit(1)
+        except webapi.RevocationError:
+            log.error(_("Too many attempts, try again later."))
+            self.cli.on_quit(1)
+        else:
+            if removed:
+                utils.set_console(info=_("Authenticator has been removed."))
+            else:
+                utils.set_console(error=_("Unable to remove the authenticator."))
```

### Comparing `steam-tools-ng-3.0.1/src/steam_tools_ng/console/cli.py` & `steam-tools-ng-3.1/src/steam_tools_ng/console/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -51,38 +51,41 @@
 class SteamToolsNG:
     def __init__(self, module_name: str, module_options: str) -> None:
         self.module_name = module_name
         self.stop = False
         self.custom_gameid = 0
         self.extra_gameid = None
 
-        if module_name in ['cardfarming', 'fakerun'] and not stlib.steamworks_available:
+        if (
+            module_name in {'cardfarming', 'fakerun'}
+            and not stlib.steamworks_available
+        ):
             log.critical(_(
                 "{} module has been disabled because you have "
                 "a stlib built without SteamWorks support. To enable it again, "
                 "reinstall stlib with SteamWorks support"
             ).format(module_name))
             sys.exit(1)
 
-        if module_name in ['steamtrades', 'steamgifts']:
+        if module_name in {'steamtrades', 'steamgifts'}:
             if not plugins.has_plugin(module_name):
                 log.critical(_(
                     "{0} module has been disabled because you don't "
                     "have {0} plugin installed. To enable it again, "
                     "install the {0} plugin."
                 ).format(module_name))
                 sys.exit(1)
 
         try:
             if module_name == 'fakerun' and not module_options:
                 raise ValueError
 
-            for index, option in enumerate(module_options):
-                self.stop = True
+            self.stop = True
 
+            for index, option in enumerate(module_options):
                 if option != 'oneshot':
                     self.custom_gameid = int(option)
 
                     if module_name == 'fakerun':
                         if self.custom_gameid == 34:
                             if len(module_options) < 2:
                                 raise ValueError
@@ -94,17 +97,15 @@
             logging.critical("Wrong command line params!")
             sys.exit(1)
 
         self.api_url = config.parser.get("steam", "api_url")
 
     @property
     def steamid(self) -> Optional[universe.SteamId]:
-        steamid = config.parser.getint("login", "steamid")
-
-        if steamid:
+        if steamid := config.parser.getint("login", "steamid"):
             try:
                 return universe.generate_steamid(steamid)
             except ValueError:
                 log.warning(_("SteamId is invalid"))
 
         return None
 
@@ -120,35 +121,35 @@
 
     async def do_login(self, *, block: bool = True, auto: bool = False) -> None:
         login_session = cli_login.Login(self)
         await login_session.do_login(auto)
 
     async def async_activate(self) -> None:
         login_session = await login.Login.new_session(0, api_url=self.api_url)
-
         utils.set_console(info=_("Logging on Steam. Please wait!"))
+        try_count = 3
 
-        token = config.parser.get("login", "token")
-        token_secure = config.parser.get("login", "token_secure")
-
-        if not token or not token_secure or not self.steamid:
-            await self.do_login()
-
-        login_session.restore_login(self.steamid, token, token_secure)
+        for login_count in range(try_count):
+            try:
+                if login_count == 0:
+                    await self.do_login(auto=True)
+                else:
+                    await self.do_login()
+            except aiohttp.ClientError as exception:
+                log.exception(str(exception))
+                log.error(_("Check your connection. (server down?)"))
+
+                if login_count == 2:
+                    return
+                log.error(_("Waiting 10 seconds to try again"))
+                await asyncio.sleep(10)
 
-        try:
-            if await login_session.is_logged_in(self.steamid):
+            if await login_session.is_logged_in():
                 utils.set_console(info=_("Steam login Successful"))
-            else:
-                await self.do_login(auto=True)
-        except aiohttp.ClientError as exception:
-            log.exception(str(exception))
-            log.error(_("Check your connection. (server down?)"))
-            await asyncio.sleep(10)
-            return  # FIXME: RETRY ###
+                break
 
         community_session = await community.Community.new_session(0, api_url=self.api_url)
 
         try:
             api_key = await community_session.get_api_key()
             log.debug(_('SteamAPI key found: %s'), api_key)
 
@@ -159,14 +160,17 @@
             await asyncio.sleep(3)
             await community_session.revoke_api_key()
             await asyncio.sleep(3)
             api_key = await community_session.register_api_key('Steam Tools NG')
 
             if not api_key:
                 raise ValueError(_('Something wrong with your SteamAPI dev key'))
+        except PermissionError:
+            log.error(_("Limited account! Using dummy API key"))
+            api_key = (0, 'Steam Tools NG')
 
         await webapi.SteamWebAPI.new_session(0, api_key=api_key[0], api_url=self.api_url)
         await internals.Internals.new_session(0)
 
         if self.module_name in ['steamtrades', 'steamgifts']:
             plugin = plugins.get_plugin(self.module_name)
             await plugin.Main.new_session(0)
@@ -174,27 +178,31 @@
         log.debug(_("Initializing module %s"), self.module_name)
         module = getattr(self, f"run_{self.module_name}")
         task = asyncio.create_task(module())
         log.debug(_("Adding a new callback for %s"), task)
         task.add_done_callback(utils.safe_task_callback)
 
     async def run_add_authenticator(self) -> None:
-        authenticator_config = authenticator.NewAuthenticator(self)
-        await authenticator_config.add_authenticator()
+        authenticator_manage = authenticator.ManageAuthenticator(self)
+        await authenticator_manage.add_authenticator()
+
+    async def run_remove_authenticator(self) -> None:
+        authenticator_manage = authenticator.ManageAuthenticator(self)
+        await authenticator_manage.remove_authenticator()
 
     @while_running
     async def run_steamguard(self) -> None:
         steamguard = core.steamguard.main()
 
         async for module_data in steamguard:
             utils.set_console(module_data)
 
     @while_running
     async def run_cardfarming(self) -> None:
-        cardfarming = core.cardfarming.main(self.steamid, self.custom_gameid)
+        cardfarming = core.cardfarming.main(self.steamid, custom_game_id=self.custom_gameid)
 
         async for module_data in cardfarming:
             utils.set_console(module_data)
 
     @while_running
     async def run_fakerun(self) -> None:
         fakerun = core.fakerun.main(self.steamid, self.custom_gameid, self.extra_gameid)
```

### Comparing `steam-tools-ng-3.0.1/src/steam_tools_ng/console/login.py` & `steam-tools-ng-3.1/src/steam_tools_ng/console/login.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,205 +11,162 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 # See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see http://www.gnu.org/licenses/.
 #
-import aiohttp
 import asyncio
 import binascii
-import codecs
 import getpass
 import logging
-import tempfile
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Optional
+
+import aiohttp
 
-from stlib import login, universe
+from stlib import login
+from stlib.login import AuthCodeType
 from . import utils
-from .. import i18n, config
+from .. import i18n, config, core
 
 if TYPE_CHECKING:
     from . import cli
 
 log = logging.getLogger(__name__)
 _ = i18n.get_translation
 
 
 # noinspection PyUnusedLocal
 class Login:
     def __init__(self, cli_: 'cli.SteamToolsNG', mobile_login: bool = True) -> None:
         self.cli = cli_
         self.mobile_login = mobile_login
         self.has_user_data = False
-        self.captcha_gid = -1
         self._username = ''
         self.__password = ''
-        self._mail_code = ''
-        self._steam_code = ''
-        self._captcha_text = ''
 
     @property
     def username(self) -> str:
         return self._username
 
     def set_password(self, encrypted_password: str) -> None:
         try:
-            key = codecs.decode(encrypted_password, 'rot13')
-            raw = codecs.decode(key.encode(), 'base64')
-            self.__password = raw.decode()
+            __password = core.utils.decode_password(encrypted_password)
+            self.__password = __password
         except (binascii.Error, UnicodeError, TypeError):
             log.warning(_("Password decode failed. Trying RAW."))
             self.__password = encrypted_password
 
     @property
-    def mail_code(self) -> str:
-        return self._mail_code
-
-    @property
-    def steam_code(self) -> str:
-        return self._steam_code
-
-    @property
-    def captcha_text(self) -> str:
-        return self._captcha_text
-
-    @property
     def shared_secret(self) -> str:
         return config.parser.get("login", "shared_secret")
 
     @property
     def identity_secret(self) -> str:
         return config.parser.get("login", "identity_secret")
 
-    async def do_login(self, auto: bool) -> None:
+    async def do_login(
+            self,
+            auto: bool,
+            auth_code: str = '',
+            auth_code_type: Optional[AuthCodeType] = AuthCodeType.device,
+    ) -> None:
         utils.set_console(info=_("Retrieving user data"))
 
         if auto:
             self._username = config.parser.get("login", "account_name")
             encrypted_password = config.parser.get("login", "password")
             self.set_password(encrypted_password)
 
         if not self.username or not self.__password:
             user_input = utils.safe_input(_("Please, write your username"))
             assert isinstance(user_input, str), "Safe input is returning bool when it should return str"
             config.new("login", "account_name", user_input)
             self._username = user_input
 
             self.__password = getpass.getpass(_("Please, write your password (IT'S HIDDEN, and will be encrypted)"))
-            password_key = codecs.encode(self.__password.encode(), 'base64')
-            encrypted_password = codecs.encode(password_key.decode(), 'rot13')
-            config.new("login", "password", encrypted_password.replace('\n', ''))
+            encrypted_password = core.utils.encode_password(self.__password)
+            config.new("login", "password", encrypted_password)
 
         _login_session = login.Login.get_session(0)
         _login_session.username = self.username
         _login_session.password = self.__password
 
-        kwargs = {'emailauth': self.mail_code, 'mobile_login': self.mobile_login}
-
-        # no reason to send captcha_text if no gid is found
-        if self.captcha_gid != -1:
-            kwargs['captcha_text'] = self.captcha_text
-            kwargs['captcha_gid'] = self.captcha_gid
-            # if login fails for any reason, gid must be unset
-            # CaptchaError exception will reset it if needed
-            self.captcha_gid = -1
-
-        if not self.shared_secret or not self.identity_secret:
+        if not self.shared_secret:
             log.warning(_("No shared secret found. Trying to log-in without two-factor authentication."))
-            # self.code_item.show()
-
-        kwargs['shared_secret'] = self.shared_secret
-        kwargs['authenticator_code'] = self.steam_code
 
         utils.set_console(info=_("Logging in"))
         try_count = 3
 
         while True:
             try:
-                login_data = await _login_session.do_login(**kwargs)
+                login_data = await _login_session.do_login(
+                    self.shared_secret,
+                    auth_code,
+                    auth_code_type,
+                    self.mobile_login,
+                )
             except login.MailCodeError:
                 user_input = utils.safe_input(_("Write code received by email"))
                 assert isinstance(user_input, str), "safe_input is returning bool when it should return str"
-                self._mail_code = user_input
-                await self.do_login(True)
+                await self.do_login(True, user_input, AuthCodeType.email)
             except login.TwoFactorCodeError:
                 if self.shared_secret:
                     if try_count > 0:
                         log.warning(_("Retrying login in 10 seconds"))
                         await asyncio.sleep(10)
                         try_count -= 1
                         continue
                     else:
                         log.error(_("shared secret is invalid!"))
                         self.cli.on_quit()
 
                 user_input = utils.safe_input(_("Write Steam Code"))
                 assert isinstance(user_input, str), "safe_input is returning bool when it should return str"
-                self._steam_code = user_input
-                await self.do_login(True)
+                await self.do_login(True, user_input)
             except login.LoginBlockedError:
                 log.error(_(
                     "Your network is blocked!\n"
                     "It'll take some time until unblocked. Please, try again later\n"
                 ))
                 self.cli.on_quit()
             except login.CaptchaError as exception:
-                self.captcha_gid = exception.captcha_gid
-
                 utils.set_console(info=_("Steam server is requesting a captcha code."))
-
-                with tempfile.NamedTemporaryFile(buffering=0, prefix='stng_', suffix='.captcha.png') as temp_file:
-                    temp_file.write(exception.captcha)
-                    temp_file.flush()
-
-                    user_input = utils.safe_input(
-                        _("Open {} in an image view and write captcha code that it shows").format(temp_file.name),
-                    )
-
+                # TODO: Captcha gid?? (where did you go? where did you go?)
+                # with tempfile.NamedTemporaryFile(buffering=0, prefix='stng_', suffix='.captcha.png') as temp_file:
+                #    temp_file.write(exception.captcha)
+                #    temp_file.flush()
+                user_input = utils.safe_input(_("Write Captcha Code"))
                 assert isinstance(user_input, str)
-                self._captcha_text = user_input
-                await self.do_login(True)
+                await self.do_login(True, user_input, AuthCodeType.machine)
             except binascii.Error:
                 log.error(_("shared secret is invalid!"))
                 self.cli.on_quit()
             except login.LoginError as exception:
                 log.error(str(exception))
-                config.remove('login', 'token')
-                config.remove('login', 'token_secure')
-                config.remove('login', 'oauth_token')
+                config.remove('login', 'refresh_token')
+                config.remove('login', 'access_token')
+                log.warning(_(
+                    "If your previous authenticator has been removed,"
+                    "\nopen your config file and remove the old secrets."
+                ))
                 self.cli.on_quit()
             except (aiohttp.ClientError, ValueError):
                 log.error(_("Check your connection. (server down?)"))
                 await asyncio.sleep(15)
                 continue
             else:
-                new_configs = {}
-
-                if "shared_secret" in login_data.auth:
-                    new_configs["shared_secret"] = login_data.auth["shared_secret"]
-                elif self.shared_secret:
-                    new_configs["shared_secret"] = self.shared_secret
-
-                if "identity_secret" in login_data.auth:
-                    new_configs['identity_secret'] = login_data.auth['identity_secret']
-                elif self.identity_secret:
-                    new_configs["identity_secret"] = self.identity_secret
-
-                if login_data.oauth:
-                    new_configs['steamid'] = login_data.oauth['steamid']
-                    new_configs['token'] = login_data.oauth['wgtoken']
-                    new_configs['token_secure'] = login_data.oauth['wgtoken_secure']
-                    new_configs['oauth_token'] = login_data.oauth['oauth_token']
-                else:
-                    new_configs['steamid'] = login_data.auth['transfer_parameters']['steamid']
-                    new_configs['token'] = login_data.auth['transfer_parameters']['webcookie']
-                    new_configs['token_secure'] = login_data.auth['transfer_parameters']['token_secure']
+                new_configs = {
+                    "account_name": self.username,
+                    'steamid': login_data.steamid,
+                    'refresh_token': login_data.refresh_token,
+                    'access_token': login_data.access_token,
+                }
 
                 for key, value in new_configs.items():
                     config.new("login", key, value)
 
-                steamid = universe.generate_steamid(new_configs['steamid'])
-                _login_session.restore_login(steamid, new_configs['token'], new_configs['token_secure'])
+                # steamid = universe.generate_steamid(new_configs['steamid'])
+                # _login_session.restore_login(steamid, new_configs['token'], new_configs['token_secure'])
                 self.has_user_data = True
 
             break
```

### Comparing `steam-tools-ng-3.0.1/src/steam_tools_ng/console/utils.py` & `steam-tools-ng-3.1/src/steam_tools_ng/console/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,19 +115,15 @@
         print(module_data.display, end=' ')
 
     if module_data.level:
         progress = module_data.level[0] + 1
         total = module_data.level[1]
         bar_size = 20
 
-        if total > 0:
-            total = int(progress * bar_size / total)
-        else:
-            total = bar_size
-
+        total = int(progress * bar_size / total) if total > 0 else bar_size
         print(f"┌{'█' * total:{bar_size}}┐", end=' ')
 
     if module_data.info:
         if not module_data.suppress_logging:
             log.info(module_data.info)
 
         print(module_data.info, sep=' ', end=' ')
```

### Comparing `steam-tools-ng-3.0.1/src/steam_tools_ng/core/__init__.py` & `steam-tools-ng-3.1/src/steam_tools_ng/core/__init__.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.0.1/src/steam_tools_ng/core/cardfarming.py` & `steam-tools-ng-3.1/src/steam_tools_ng/core/cardfarming.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,107 +11,49 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 # See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see http://www.gnu.org/licenses/.
 #
-import aiohttp
 import asyncio
-import atexit
 import contextlib
 import random
-import sys
 import time
-from pathlib import Path
 from subprocess import call
 from typing import AsyncGenerator, Dict, Optional, Any
 
+import aiohttp
+
 from stlib import webapi, client, universe, community
 from . import utils
 from .. import i18n, config
 
-if sys.platform == 'win32':
-    from psutil import Popen, NoSuchProcess
-
 _ = i18n.get_translation
-
-
-# FIXME: Workaround for keyboard lag when running games on GUI on Windows
-# FIXME: https://gitlab.gnome.org/GNOME/gtk/-/issues/2015
-# FIXME: L36:91
-def killall(process: 'Popen') -> None:
-    if not process.is_running():
-        return
-
-    for child in process.children(recursive=True):
-        with contextlib.suppress(NoSuchProcess):
-            child.kill()
-            child.wait()
-
-    process.kill()
-    process.wait()
-
-
-class SteamAPIExecutorWorkaround:
-    def __init__(self, appid: int, *args: Any, **kwargs: Any) -> None:
-        self.process = None
-        self.appid = appid
-        self._is_running = False
-
-        if sys.platform == 'win32':
-            if getattr(sys, 'frozen', False):
-                executor_path = [str(Path(sys.executable).parent / 'steam-api-executor.exe'), str(self.appid)]
-            else:
-                executor_path = [sys.executable, '-m', 'steam_tools_ng.steam_api_executor', str(self.appid)]
-
-            self.process = Popen(executor_path, creationflags=0x08000000)
-            self._is_running = True
-            atexit.register(killall, self.process)
-        else:
-            self.executor = _SteamAPIExecutor(appid, *args, **kwargs)
-
-    def is_running(self) -> bool:
-        if sys.platform == 'win32':
-            return self._is_running
-        else:
-            return self.executor.is_running()
-
-    def shutdown(self, *args: Any, **kwargs: Any) -> None:
-        if sys.platform == 'win32':
-            killall(self.process)
-            self._is_running = False
-        else:
-            self.executor.shutdown(*args, **kwargs)
-
-
-if 'gtk' in sys.modules:
-    _SteamAPIExecutor = client.SteamAPIExecutor
-    client.SteamAPIExecutor = SteamAPIExecutorWorkaround
-
-# FIXME: L36:91
-# FIXME: ---- #
-
 executors = {}
-total_cards_remaining = 0
 
 
 def safe_exit(*args: Any, **kwargs: Any) -> None:
     for executor in executors.values():
-        executor.shutdown(*args, **kwargs)
+        with contextlib.suppress(RuntimeError):
+            executor.shutdown(*args, **kwargs)
 
 
 async def while_has_cards(
         steamid: universe.SteamId,
         badge: community.Badge,
+        play_event: Optional[asyncio.Event] = None,
 ) -> AsyncGenerator[utils.ModuleData, None]:
     webapi_session = webapi.SteamWebAPI.get_session(0)
     community_session = community.Community.get_session(0)
 
     while badge.cards != 0:
+        if play_event:
+            await play_event.wait()
+
         mandatory_waiting = config.parser.getint("cardfarming", "mandatory_waiting")
         wait_while_running = config.parser.getint("cardfarming", "wait_while_running")
         wait_for_drops = config.parser.getint("cardfarming", "wait_for_drops")
 
         try:
             game_list = await webapi_session.get_owned_games(steamid, appids_filter=[badge.appid])
             game_info = game_list[0]
@@ -146,14 +88,20 @@
             info=badge.name,
             status=_("Running {}").format(badge.name),
             raw_data=executor,
             action="check",
         )
 
         async for data in utils.timed_module_data(wait_offset, module_data):
+            if play_event and not play_event.is_set():
+                executor.shutdown()
+                await asyncio.sleep(1)
+                await play_event.wait()
+                executor.__init__(executor.appid)
+
             yield data
 
         executor.shutdown()
         wait_offset = random.randint(wait_for_drops, int(wait_for_drops / 100 * 125))
 
         module_data = utils.ModuleData(
             display=str(badge.appid),
@@ -172,33 +120,40 @@
                 await asyncio.sleep(10)
             except community.BadgeError:
                 yield utils.ModuleData(error=_("Steam Server is busy"), info=_("Waiting Changes"))
                 await asyncio.sleep(20)
             else:
                 break
 
-        global total_cards_remaining
-        total_cards_remaining -= badge.cards - cards
+        yield utils.ModuleData(action="update_drops", raw_data=badge.cards - cards)
+
         # noinspection PyProtectedMember
         badge = badge._replace(cards=cards)
 
     utils.ModuleData(
         display=str(badge.appid),
         info=_("{} ({})").format(_("Done"), badge.name),
     )
 
 
-async def main(steamid: universe.SteamId, custom_game_id: int = 0) -> AsyncGenerator[utils.ModuleData, None]:
+async def main(
+        steamid: universe.SteamId,
+        play_event: Optional[asyncio.Event] = None,
+        custom_game_id: int = 0,
+) -> AsyncGenerator[utils.ModuleData, None]:
+    if play_event:
+        await play_event.wait()
+
     asyncio.current_task().add_done_callback(safe_exit)
 
     reverse_sorting = config.parser.getboolean("cardfarming", "reverse_sorting")
     max_concurrency = config.parser.getint("cardfarming", "max_concurrency")
     invisible = config.parser.getboolean("cardfarming", "invisible")
     community_session = community.Community.get_session(0)
-    global total_cards_remaining
+    total_cards_remaining = 0
 
     try:
         badges = sorted(
             await community_session.get_badges(steamid),
             key=lambda badge_: badge_.cards,  # type: ignore
             reverse=reverse_sorting
         )
@@ -230,23 +185,23 @@
             status=_("Loading {}").format(badge.name),
         )
 
         if custom_game_id and badge.appid != custom_game_id:
             yield utils.ModuleData(info=_("Skipping {}").format(badge.appid))
             continue
 
-        generators[badge.appid] = while_has_cards(steamid, badge)
+        generators[badge.appid] = while_has_cards(steamid, badge, play_event)
         total_cards_remaining += badge.cards
 
     tasks: Dict[int, Optional[asyncio.Task[Any]]] = {}
     semaphore = asyncio.Semaphore(max_concurrency)
     last_update = 0
 
     while True:
-        for appid in generators.keys():
+        for appid in generators:
             progress_coro = anext(generators[appid])
             assert asyncio.iscoroutine(progress_coro)
 
             if appid not in tasks:
                 if semaphore.locked():
                     break
 
@@ -283,23 +238,24 @@
             if task and task.done() and not task.exception():
                 global executors
                 data: utils.ModuleData = task.result()
 
                 if data.action == 'check':
                     executors[appid] = data.raw_data
 
+                if data.action == "update_drops":
+                    total_cards_remaining -= data.raw_data
+
                 if int(time.time()) > last_update + 3:
                     current_running_limit = len(tasks)
                     total_remaining = len(generators) - len([task for task in tasks.values() if not task])
                     running_executors = [executor for executor in executors.values() if executor.is_running()]
                     extra_info = ''
 
-                    if current_running_limit > total_remaining:
-                        current_running_limit = total_remaining
-
+                    current_running_limit = min(current_running_limit, total_remaining)
                     if current_running_limit == 2:
                         extra_info = _(" +{} other").format(current_running_limit - 1)
                     elif current_running_limit > 2:
                         extra_info = _(" +{} others").format(current_running_limit - 1)
 
                     yield utils.ModuleData(
                         display=' : '.join([str(executor.appid) for executor in running_executors]),
```

### Comparing `steam-tools-ng-3.0.1/src/steam_tools_ng/core/confirmations.py` & `steam-tools-ng-3.1/src/steam_tools_ng/core/confirmations.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,9 +64,9 @@
     except login.LoginError:
         module_data = utils.ModuleData(error=_("Not logged in"), action="login")
     except aiohttp.ClientError:
         module_data = utils.ModuleData(error=_("Check your connection. (server down?)"), info=_("Waiting Changes"))
     else:
         module_data = utils.ModuleData(action="update", raw_data=confirmations)
 
-    async for data in utils.timed_module_data(20, module_data):
+    async for data in utils.timed_module_data(30, module_data):
         yield data
```

### Comparing `steam-tools-ng-3.0.1/src/steam_tools_ng/core/coupons.py` & `steam-tools-ng-3.1/src/steam_tools_ng/core/coupons.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         await asyncio.sleep(5)
         return
 
     try:
         owned_games = await webapi_session.get_owned_games(steamid)
     except aiohttp.ClientError:
         yield utils.ModuleData(error=_("Failed when trying to get owned games"))
-        await asyncio.sleep(15)
+        await asyncio.sleep(30)
         return
 
     yield utils.ModuleData(action="clear")
     package_count = 1
 
     for botid, token in zip(bot_list, token_list):
         try:
@@ -77,49 +77,59 @@
             return
 
         try:
             inventory = await community_session.get_inventory(steamid, appid, contextid)
         except AttributeError:
             module_data = utils.ModuleData(error=_("Error when fetch inventory"), info=_("Waiting Changes"))
 
-            async for data in utils.timed_module_data(15, module_data):
+            async for data in utils.timed_module_data(30, module_data):
                 yield data
 
             return
         except aiohttp.ClientError:
             module_data = utils.ModuleData(error=_("Check your connection. (server down?)"), info=_("Waiting Changes"))
 
-            async for data in utils.timed_module_data(60, module_data):
+            async for data in utils.timed_module_data(120, module_data):
                 yield data
 
             return
 
         if not inventory:
             module_data = utils.ModuleData(error=_("The botid {} has no coupons available"), info=_("Skipping"))
 
-            async for data in utils.timed_module_data(15, module_data):
+            async for data in utils.timed_module_data(30, module_data):
                 yield data
 
             continue
 
         for index, coupon_ in enumerate(inventory):
             yield utils.ModuleData(action="update_level", raw_data=(index, len(inventory)))
             package_link = coupon_.actions[0]['link']
             packageids = [int(id_) for id_ in package_link.split('=')[1].split(',')]
             blacklist = config.parser.get('coupons', 'blacklist')
-            ignored_list = [coupon.split('% OFF')[-1].split('- Coupon')[0].strip() for coupon in blacklist.split(',')]
-            ignored_list += [game.name for game in owned_games]
+            ignored_list = [name.split('% OFF')[-1].split('- Coupon')[0].strip() for name in blacklist.split(',')]
+            ignored_list.extend([game.name for game in owned_games])
             minimum_discount = config.parser.getint('coupons', 'minimum_discount')
+            game_name = coupon_.name.split('% OFF')[-1].split('- Coupon')[0].strip()
 
             for package_id in packageids:
                 if not fetch_coupon_event.is_set():
                     log.warning(_("Stopping fetching coupons (requested by user)"))
                     yield utils.ModuleData(action="update_level", raw_data=(0, 0))
                     return
 
+                if any(
+                        ignored == game_name or
+                        (ignored.startswith('*') and game_name.endswith(ignored[1:])) or
+                        (ignored.endswith('*') and game_name.startswith(ignored[:-1]))
+                        for ignored in blacklist
+                ):
+                    log.info(_('Ignoring coupon %s due blacklist'), coupon_.name)
+                    continue
+
                 if coupon_.name.split('% OFF')[-1].split('- Coupon')[0].strip() in ignored_list:
                     log.info(_('Ignoring coupon %s due blacklist'), coupon_.name)
                     continue
 
                 coupon_discount = int(coupon_.name.split('%')[0])
 
                 if coupon_discount < minimum_discount:
@@ -167,8 +177,9 @@
 
             if index and not package_count % 130:
                 module_data = utils.ModuleData(error=_("Api rate limit reached. Waiting."), info=_("Waiting Changes"))
 
                 async for data in utils.timed_module_data(120, module_data):
                     yield data
 
+    yield utils.ModuleData(action="update_level", raw_data=(0, 0))
     fetch_coupon_event.clear()
```

### Comparing `steam-tools-ng-3.0.1/src/steam_tools_ng/core/fakerun.py` & `steam-tools-ng-3.1/src/steam_tools_ng/core/fakerun.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.0.1/src/steam_tools_ng/core/steamgifts.py` & `steam-tools-ng-3.1/src/steam_tools_ng/core/steamgifts.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,20 +29,19 @@
 _ = i18n.get_translation
 log = logging.getLogger(__name__)
 
 
 async def main() -> AsyncGenerator[utils.ModuleData, None]:
     yield utils.ModuleData(status=_("Loading"))
 
-    if plugins.has_plugin("steamgifts"):
-        steamgifts = plugins.get_plugin("steamgifts")
-        steamgifts_session = steamgifts.Main.get_session(0)
-    else:
+    if not plugins.has_plugin("steamgifts"):
         raise ImportError(_("Unable to find Steamgifts plugin."))
 
+    steamgifts = plugins.get_plugin("steamgifts")
+    steamgifts_session = steamgifts.Main.get_session(0)
     try:
         await steamgifts_session.do_login()
     except aiohttp.ClientError:
         yield utils.ModuleData(error=_("Check your connection. (server down?)"), info=_("Waiting Changes"))
         await asyncio.sleep(15)
         return
     except steamgifts.TooFast:
@@ -127,15 +126,15 @@
             sort_type = config.parser.get(strategy, "sort_type")
             sort_name = sort_type[:-1]
             sort_direction = sort_type[-1]
 
             giveaways = sorted(
                 giveaways,
                 key=lambda giveaway_: getattr(giveaway_, sort_name),
-                reverse=True if sort_direction == '-' else False,
+                reverse=sort_direction == '-',
             )
         else:
             yield utils.ModuleData(status=_("No giveaways to join for strategy {}. Skipping.").format(strategy_index))
             continue
 
         restart = False
```

### Comparing `steam-tools-ng-3.0.1/src/steam_tools_ng/core/steamguard.py` & `steam-tools-ng-3.1/src/steam_tools_ng/core/steamguard.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.0.1/src/steam_tools_ng/core/steamtrades.py` & `steam-tools-ng-3.1/src/steam_tools_ng/core/steamtrades.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,20 +28,19 @@
 _ = i18n.get_translation
 log = logging.getLogger(__name__)
 
 
 async def main() -> AsyncGenerator[utils.ModuleData, None]:
     yield utils.ModuleData(status=_("Loading"))
 
-    if plugins.has_plugin("steamtrades"):
-        steamtrades = plugins.get_plugin("steamtrades")
-        steamtrades_session = steamtrades.Main.get_session(0)
-    else:
+    if not plugins.has_plugin("steamtrades"):
         raise ImportError(_("Unable to find Steamtrades plugin"))
 
+    steamtrades = plugins.get_plugin("steamtrades")
+    steamtrades_session = steamtrades.Main.get_session(0)
     trade_ids = config.parser.get("steamtrades", "trade_ids")
     wait_for_bump = config.parser.getint("steamtrades", "wait_for_bump")
 
     if not trade_ids:
         yield utils.ModuleData(error=_("No trade ID found"), info=_("Waiting Changes"))
         await asyncio.sleep(5)
         return
```

### Comparing `steam-tools-ng-3.0.1/src/steam_tools_ng/gtk/__init__.py` & `steam-tools-ng-3.1/src/steam_tools_ng/gtk/__init__.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.0.1/src/steam_tools_ng/gtk/about.py` & `steam-tools-ng-3.1/src/steam_tools_ng/gtk/about.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,25 +13,26 @@
 # See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see http://www.gnu.org/licenses/.
 #
 
 from importlib import resources
+from typing import Optional
 
 from gi.repository import Gdk, Gtk
 
 from .. import __version__, i18n
 
 _ = i18n.get_translation
 
 
 # noinspection PyUnusedLocal
 class AboutDialog(Gtk.AboutDialog):
-    def __init__(self, parent_window: Gtk.Window) -> None:
+    def __init__(self, parent_window: Optional[Gtk.Window]) -> None:
         super().__init__()
         self.set_transient_for(parent_window)
         self.set_modal(True)
         self.set_program_name("Steam Tools NG")
 
         self.set_authors([
             "Lara Maia",
```

### Comparing `steam-tools-ng-3.0.1/src/steam_tools_ng/gtk/application.py` & `steam-tools-ng-3.1/src/steam_tools_ng/gtk/application.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,23 +54,19 @@
         self.api_login: Optional[login.Login] = None
         self.api_url = config.parser.get("steam", "api_url")
 
         self.old_confirmations: List[community.Confirmation] = []
 
     @property
     def main_window(self) -> Optional[window.Main]:
-        current_window = self.get_window_by_id(self._main_window_id)
-
-        return current_window
+        return self.get_window_by_id(self._main_window_id)
 
     @property
     def steamid(self) -> Optional[universe.SteamId]:
-        steamid = config.parser.getint("login", "steamid")
-
-        if steamid:
+        if steamid := config.parser.getint("login", "steamid"):
             try:
                 return universe.generate_steamid(steamid)
             except ValueError:
                 log.warning(_("SteamId is invalid"))
 
         return None
 
@@ -87,74 +83,75 @@
 
         exit_action = Gio.SimpleAction.new("exit")
         exit_action.connect("activate", self.on_exit_activate)
         self.add_action(exit_action)
 
         theme = config.parser.get("general", "theme")
 
-        if theme == 'dark':
-            self.gtk_settings.props.gtk_application_prefer_dark_theme = True
-        else:
-            self.gtk_settings.props.gtk_application_prefer_dark_theme = False
+        self.gtk_settings.props.gtk_application_prefer_dark_theme = theme == 'dark'
 
     def do_activate(self) -> None:
         if self._main_window_id != 0:
             self.main_window.present()
             return
 
         current_window = window.Main(application=self, title="Steam Tools NG")
         self._main_window_id = current_window.get_id()
-        current_window.show()
+        current_window.present()
 
         loop = asyncio.get_event_loop()
         task = loop.create_task(self.async_activate())
         task.add_done_callback(utils.safe_task_callback)
 
     async def do_login(self, *, block: bool = True, auto: bool = False) -> None:
-        login_dialog = gtk_login.LoginDialog(self.main_window, self)
-        login_dialog.set_deletable(False)
-        login_dialog.show()
+        login_window = gtk_login.LoginWindow(self.main_window, self)
+        login_window.set_deletable(False)
+        login_window.present()
 
         if auto:
             encrypted_password = config.parser.get("login", "password")
-            login_dialog.set_password(encrypted_password)
-            login_dialog.login_button.emit('clicked')
+            login_window.set_password(encrypted_password)
+            login_window.login_button.emit('clicked')
 
         if block:
             while self.main_window.get_realized():
-                if login_dialog.has_user_data:
+                if login_window.has_user_data:
                     break
 
                 await asyncio.sleep(1)
 
     async def async_activate(self) -> None:
         assert isinstance(self.main_window, window.Main)
         login_session = await login.Login.new_session(0, api_url=self.api_url)
 
         self.main_window.statusbar.set_warning("steamguard", _("Logging on Steam. Please wait!"))
         log.info(_("Logging on Steam"))
+        try_count = 3
 
-        token = config.parser.get("login", "token")
-        token_secure = config.parser.get("login", "token_secure")
-
-        if not token or not token_secure or not self.steamid:
-            await self.do_login()
-
-        login_session.restore_login(self.steamid, token, token_secure)
+        for login_count in range(try_count):
+            try:
+                if login_count == 0:
+                    await self.do_login(auto=True)
+                else:
+                    await self.do_login()
+            except aiohttp.ClientError as error:
+                log.exception(str(error))
+                self.main_window.statusbar.set_critical(
+                    "steamguard",
+                    _("Check your connection. (server down?)"),
+                )
+
+                if login_count == 2:
+                    return
+                log.error(_("Waiting 10 seconds to try again"))
+                await asyncio.sleep(10)
 
-        try:
-            if await login_session.is_logged_in(self.steamid):
+            if await login_session.is_logged_in():
                 log.info("Steam login Successful")
-            else:
-                await self.do_login(auto=True)
-        except aiohttp.ClientError as error:
-            log.exception(str(error))
-            self.main_window.statusbar.set_critical("steamguard", _("Check your connection. (server down?)"))
-            await asyncio.sleep(10)
-            return  # FIXME: RETRY ###
+                break
 
         self.main_window.statusbar.clear("steamguard")
 
         community_session = await community.Community.new_session(0, api_url=self.api_url)
 
         try:
             api_key = await community_session.get_api_key()
@@ -168,25 +165,34 @@
             await community_session.revoke_api_key()
             await asyncio.sleep(3)
             api_key = await community_session.register_api_key('Steam Tools NG')
             self.main_window.statusbar.clear('steamguard')
 
             if not api_key:
                 utils.fatal_error_dialog(ValueError(_('Something wrong with your SteamAPI dev key')), [])
+        except PermissionError:
+            log.error(_("Limited account! Using dummy API key"))
+            self.main_window.limited_label.set_visible(True)
+            api_key = (0, 'Steam Tools NG')
 
         webapi_session = await webapi.SteamWebAPI.new_session(0, api_key=api_key[0], api_url=self.api_url)
         internals_session = await internals.Internals.new_session(0)
 
         modules: Dict[str, asyncio.Task[Any]] = {}
 
         while self.main_window.get_realized():
             for module_name in config.plugins.keys():
                 task = modules.get(module_name, None)
 
-                if config.parser.getboolean(module_name, "enable"):
+                if module_name == "confirmations":
+                    enabled = config.parser.getboolean("steamguard", "enable_confirmations")
+                else:
+                    enabled = config.parser.getboolean(module_name, "enable")
+
+                if enabled:
                     if task:
                         if task.cancelled() and not task._exception:  # why task.exception() is raising?
                             log.debug(_("%s is requesting a reinitialization."), module_name)
                             modules.pop(module_name)
 
                         await asyncio.sleep(1)
                     else:
@@ -230,15 +236,15 @@
         steamguard = core.steamguard.main()
 
         async for module_data in steamguard:
             self.main_window.set_status("steamguard", module_data)
 
     @while_window_realized
     async def run_cardfarming(self, play_event: asyncio.Event) -> None:
-        cardfarming = core.cardfarming.main(self.steamid)
+        cardfarming = core.cardfarming.main(self.steamid, play_event)
 
         async for module_data in cardfarming:
             self.main_window.set_status("cardfarming", module_data)
 
             if module_data.action == "check":
                 executors = module_data.raw_data
 
@@ -273,33 +279,41 @@
             if module_data.action == "update":
                 self.main_window.statusbar.set_warning("confirmations", "Updating now!")
                 if module_data.raw_data == self.old_confirmations:
                     log.debug(_("Skipping confirmations update because data doesn't seem to have changed"))
                     self.main_window.statusbar.clear('confirmations')
                     continue
 
-                self.main_window.confirmations_tree.store.clear()
+                self.main_window.confirmations_tree.clear()
 
                 for confirmation_ in module_data.raw_data:
                     # translatable strings
                     t_give = utils.sanitize_confirmation(confirmation_.give)
                     t_receive = utils.sanitize_confirmation(confirmation_.receive)
 
-                    iter_ = self.main_window.confirmations_tree.store.append(None, [
-                        str(confirmation_.confid),
+                    item = self.main_window.confirmations_tree.new_item(
+                        str(confirmation_.id),
                         str(confirmation_.creatorid),
-                        str(confirmation_.key),
+                        str(confirmation_.nonce),
                         utils.markup(t_give),
                         utils.markup(confirmation_.to),
                         utils.markup(t_receive),
-                    ])
+                        '. '.join(confirmation_.summary),
+                    )
 
-                    for item in itertools.zip_longest(confirmation_.give, confirmation_.receive):
-                        row = ['', '', '', item[0], '-->', item[1] if item[1] else 'Nothing']
-                        self.main_window.confirmations_tree.store.append(iter_, row)
+                    for give, receive in itertools.zip_longest(confirmation_.give, confirmation_.receive):
+                        child = self.main_window.confirmations_tree.new_item(
+                            give=give if give else _("Nothing"),
+                            to='-->',
+                            receive=receive if receive else _("Nothing"),
+                        )
+
+                        item.children.append(child)
+
+                    self.main_window.confirmations_tree.append_row(item)
 
                 self.old_confirmations = module_data.raw_data
                 self.main_window.statusbar.clear('confirmations')
 
     @while_window_realized
     async def run_coupons(self) -> None:
         fetch_coupon_event = self.main_window.fetch_coupon_event
@@ -317,25 +331,27 @@
             if module_data.info:
                 self.main_window.statusbar.set_warning("coupons", module_data.info)
 
             if not any([module_data.info, module_data.error]):
                 self.main_window.statusbar.clear("coupons")
 
             if module_data.action == "update":
-                iter_ = self.main_window.coupons_tree.store.append([
+                item = self.main_window.coupons_tree.new_item(
                     f"{module_data.raw_data['price']:.2f}",
                     utils.markup(module_data.raw_data['name'], foreground='blue', underline='single'),
                     module_data.raw_data['link'],
                     module_data.raw_data['botid'],
                     module_data.raw_data['token'],
                     str(module_data.raw_data['assetid']),
-                ])
+                )
+
+                self.main_window.coupons_tree.append_row(item)
 
             if module_data.action == "clear":
-                self.main_window.coupons_tree.store.clear()
+                self.main_window.coupons_tree.clear()
 
             if module_data.action == "update_level":
                 self.main_window.coupon_progress.set_value(module_data.raw_data[0])
                 self.main_window.coupon_progress.set_max_value(module_data.raw_data[1])
 
     @while_window_realized
     async def run_steamtrades(self, play_event: asyncio.Event) -> None:
@@ -358,19 +374,19 @@
             self.main_window.set_status("steamgifts", module_data)
 
             if module_data.action == "login":
                 await self.do_login(auto=True)
                 continue
 
     def on_settings_activate(self, *args: Any) -> None:
-        settings_dialog = settings.SettingsDialog(self.main_window, self)
-        settings_dialog.show()
+        settings_window = settings.SettingsWindow(self.main_window, self)
+        settings_window.present()
 
     def on_about_activate(self, *args: Any) -> None:
-        dialog = about.AboutDialog(self.main_window)
-        dialog.show()
+        about_dialog = about.AboutDialog(self.main_window)
+        about_dialog.present()
 
     # noinspection PyMethodMayBeStatic
     def on_exit_activate(self, *args: Any) -> None:
         loop = asyncio.get_running_loop()
         loop.stop()
         # self.main_window.destroy()
```

### Comparing `steam-tools-ng-3.0.1/src/steam_tools_ng/gtk/async_gtk.py` & `steam-tools-ng-3.1/src/steam_tools_ng/gtk/async_gtk.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.0.1/src/steam_tools_ng/gtk/authenticator.py` & `steam-tools-ng-3.1/src/steam_tools_ng/gtk/coupon.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,205 +11,230 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 # See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see http://www.gnu.org/licenses/.
 #
-import aiohttp
 import asyncio
 import logging
-from gi.repository import Gtk, Gdk
-from typing import Optional
+import time
+from typing import Any
 
-from stlib import universe, webapi
-from . import utils
-from .. import i18n, config
+from gi.repository import Gtk
+
+from stlib import community
+from stlib import universe
+from . import utils, confirmation
+from .. import config, i18n
 
 log = logging.getLogger(__name__)
 _ = i18n.get_translation
 
 
 # noinspection PyUnusedLocal
-class NewAuthenticatorDialog(Gtk.Dialog):
-    def __init__(self, parent_window: Gtk.Window, application: Gtk.Application) -> None:
-        super().__init__(use_header_bar=True)
-        self.application = application
-        self._login_data = None
-        self.webapi_session = webapi.SteamWebAPI.get_session(0)
-
-        self.header_bar = self.get_header_bar()
-
-        self.add_authenticator_button = utils.AsyncButton()
-        self.add_authenticator_button.set_label(_("Add Authenticator"))
-        self.add_authenticator_button.connect("clicked", self.on_add_authenticator_clicked)
-        self.header_bar.pack_end(self.add_authenticator_button)
-
-        self.parent_window = parent_window
-        self.set_default_size(400, 100)
-        self.set_title(_('New Authenticator'))
-        self.set_transient_for(parent_window)
-        self.set_modal(True)
-        self.set_destroy_with_parent(True)
-        self.set_resizable(False)
-
-        self.content_area = self.get_content_area()
-        self.content_area.set_orientation(Gtk.Orientation.VERTICAL)
-        self.content_area.set_spacing(10)
-        self.content_area.set_margin_start(10)
-        self.content_area.set_margin_end(10)
-        self.content_area.set_margin_top(10)
-        self.content_area.set_margin_bottom(10)
+class CouponWindow(utils.PopupWindowBase):
+    def __init__(
+            self,
+            parent_window: Gtk.Window,
+            application: Gtk.Application,
+            coupons_tree: utils.SimpleTextTree,
+            action: str
+    ) -> None:
+        super().__init__(parent_window, application)
+        self.community_session = community.Community.get_session(0)
+        self.coupons_tree = coupons_tree
+        self.selection = self.coupons_tree.model.get_selected_item()
+        self.has_status = False
+        self.action = action
+        self.header_bar.set_show_title_buttons(False)
+
+        self.yes_button = Gtk.Button()
+        self.yes_button.set_label(_("Continue"))
+        self.header_bar.pack_end(self.yes_button)
+
+        self.no_button = Gtk.Button()
+        self.no_button.set_label(_("Cancel"))
+        self.no_button.connect("clicked", lambda button: self.destroy())
+        self.header_bar.pack_start(self.no_button)
 
         self.status = utils.SimpleStatus()
-        self.content_area.append(self.status)
+        self.content_grid.attach(self.status, 0, 0, 1, 1)
 
-        self.user_details_section = utils.Section("Login")
-        self.content_area.append(self.user_details_section)
+        if self.action == 'get':
+            self.set_title(_('Get Coupon'))
 
-        self.sms_code_item = self.user_details_section.new_item("_sms_code", _("SMS Code:"), Gtk.Entry, 0, 1)
+            trade_time = int(time.time()) - config.parser.getint('coupons', 'last_trade_time')
+            if trade_time < 120:
+                self.status.error(_("You must wait {} seconds to get another coupon").format(120 - trade_time))
+                self.header_bar.set_show_title_buttons(True)
+                self.yes_button.set_visible(False)
+                self.no_button.set_visible(False)
+                return
+
+            if self.selection:
+                self.status.info(
+                    _(
+                        "You are about to request {}\n"
+                        "The item will be automatically added at your inventory in 1 minute"
+                    ).format(utils.unmarkup(self.selection.get_item().name))
+                )
+            else:
+                self.status.error(_("You must select something"))
+                self.header_bar.set_show_title_buttons(True)
+                self.yes_button.set_visible(False)
+                self.no_button.set_visible(False)
+        else:
+            self.set_title(_('Send Coupon'))
 
-        self.connect('response', lambda dialog, _action: dialog.destroy())
+            self.status.info(
+                _(
+                    "You are about to giveaway all coupons in your inventory\n"
+                    "The items will be automatically accepted and transferred in 1 minute"
+                )
+            )
 
-        key_event = Gtk.EventControllerKey()
-        key_event.connect('key-released', self.on_key_release_event)
-        self.add_controller(key_event)
+        self.yes_button.connect("clicked", self.on_yes_button_clicked)
 
-        self.add_authenticator_button.emit('clicked')
+    def on_yes_button_clicked(self, button: Gtk.Button) -> None:
+        button.set_visible(False)
+        self.no_button.set_visible(False)
+        self.set_size_request(0, 0)
+        self.header_bar.set_show_title_buttons(False)
+        self.coupons_tree.lock = True
 
-    @property
-    def sms_code(self) -> str:
-        return self.sms_code_item.get_text()
+        loop = asyncio.get_event_loop()
+        task = loop.create_task(self.send_trade_offer())
+        task.add_done_callback(self.on_task_finish)
+
+    def on_task_finish(self, task: asyncio.Task[Any]) -> None:
+        self.coupons_tree.lock = False
+        exception = task.exception()
 
-    @property
-    def oauth_token(self) -> str:
-        return config.parser.get("login", "oauth_token")
+        if exception and not isinstance(exception, asyncio.CancelledError):
+            try:
+                current_exception = task.exception()
+                assert isinstance(current_exception, BaseException)
+                raise current_exception
+            except community.InventoryEmptyError:
+                self.status.error(_("Inventory is empty."))
+                self.header_bar.set_show_title_buttons(True)
+            except Exception as exception:
+                stack = task.get_stack()
+
+                for frame in stack:
+                    log.error(f"{type(exception).__name__} at {frame}")
+
+                log.error(f"Steam Server is slow. {str(exception)}")
+
+                self.status.error(
+                    _(
+                        "Unable to complete this trade. The reason is one of the following:\n\n"
+                        "1. The item you choose already gone. Try another one.\n"
+                        "2. You wrote a wrong token in config. Update you config.\n"
+                        "3. The Steam server is slow. Wait a minute and try again.\n\n"
+                        "If you keep seeing this error, please update the coupon list."
+                    )
+                )
 
-    @property
-    def steamid(self) -> Optional[universe.SteamId]:
-        steamid = config.parser.getint("login", "steamid")
+                self.header_bar.set_show_title_buttons(True)
+                self.yes_button.set_visible(False)
+        else:
+            config.new("coupons", "last_trade_time", int(time.time()))
+            self.confirmations_tree.remove_row(self.selection)
 
-        if steamid:
-            try:
-                return universe.generate_steamid(steamid)
-            except ValueError:
-                log.warning(_("SteamId is invalid"))
+            if not self.has_status:
+                self.destroy()
 
-        return None
+    async def send_trade_offer(self) -> None:
+        self.status.info(_("Waiting Steam Server"))
+        contextid = config.parser.getint('coupons', 'contextid')
+        appid = config.parser.getint('coupons', 'appid')
+        botid_raw = config.parser.get('coupons', 'botid_to_donate')
+        token = config.parser.get('coupons', 'token_to_donate')
+        steamid_raw = config.parser.getint('login', 'steamid')
 
-    def on_key_release_event(
-            self,
-            controller: Gtk.EventControllerKey,
-            keyval: int,
-            keycode: int,
-            state: Gdk.ModifierType,
-    ) -> None:
-        if keyval == Gdk.KEY_Return:
-            self.add_authenticator_button.emit('clicked')
+        try:
+            steamid = universe.generate_steamid(steamid_raw)
+        except ValueError:
+            self.status.info(_("Your steamid is invalid. (are you logged in?)"))
+            self.header_bar.set_show_title_buttons(True)
+            self.yes_button.set_visible(False)
+            self.has_status = True
+            return
 
-    async def on_add_authenticator_clicked(self, button: Gtk.Button) -> None:
-        self.status.info(_("Retrieving user data"))
-        button.set_sensitive(False)
-        self.user_details_section.hide()
-        self.set_size_request(0, 0)
+        give = []
+        receive = []
 
-        if not self.oauth_token or not self.steamid:
-            self.status.error(_(
-                "Some login data is missing. If the problem persists, go to:\n"
-                "Settings -> Login -> Advanced -> and click on RESET Everything."
-            ))
+        if self.action == 'get':
+            botid_raw = self.selection.get_item().botid
+            token = self.selection.get_item().token
+            assetid = int(self.selection.get_item().assetid)
+            receive = [(appid, assetid, 1)]
+        else:
+            json_data = await self.community_session.get_inventory(steamid, appid, contextid)
 
+            give.extend(
+                (coupon.appid, coupon.assetid, coupon.amount)
+                for coupon in json_data
+            )
+        try:
+            botid = universe.generate_steamid(botid_raw)
+        except ValueError:
+            self.status.info(_("botid to donation is invalid. Check your config."))
+            self.header_bar.set_show_title_buttons(True)
+            self.yes_button.set_visible(False)
+            self.has_status = True
             return
 
-        if not self._login_data or not self.sms_code:
-            try:
-                self._login_data = await self.webapi_session.new_authenticator(self.steamid, self.oauth_token)
-            except aiohttp.ClientError:
-                self.status.error(_("Check your connection. (server down?)"))
-            except webapi.AuthenticatorExists:
-                self.status.error(_(
-                    "There's already an authenticator active for that account.\n"
-                    "Remove your current steam authenticator and try again."
-                ))
-            except webapi.PhoneNotRegistered:
-                self.status.error(_(
-                    "You must have a phone registered on your steam account to proceed.\n"
-                    "Go to your Steam Account Settings, add a Phone Number, and try again."
-                ))
-            except NotImplementedError as exception:
-                import sys
-                import traceback
-                traceback_info = sys.exc_info()[2]
-                utils.fatal_error_dialog(exception, traceback.extract_tb(traceback_info), self.parent_window)
-                self.application.on_exit_activate()
-            else:
-                self.status.info(_("Enter bellow the code received by SMS\nand click on 'Add Authenticator' button"))
-                self.user_details_section.show()
-                self.sms_code_item.set_text('')
-                self.sms_code_item.grab_focus()
-            finally:
-                button.set_sensitive(True)
+        json_data = await self.community_session.send_trade_offer(botid, token, contextid, give, receive)
 
+        if len(json_data) == 1 and 'tradeofferid' in json_data:
             return
 
-        self.status.info(_("Adding authenticator"))
+        if 'needs_email_confirmation' in json_data and json_data['needs_email_confirmation']:
+            self.status.info(_('You will need to manually confirm the trade offer. Check your email.'))
+            self.header_bar.set_show_title_buttons(True)
+            self.yes_button.set_visible(False)
 
-        try:
-            await self.webapi_session.add_authenticator(
-                self.steamid,
-                self.oauth_token,
-                self._login_data.auth['shared_secret'],
-                self.sms_code,
+            # FIXME: track tradeoffer and wait for email confirmation
+            self.has_status = True
+            return
+
+        if 'needs_mobile_confirmation' in json_data and json_data['needs_mobile_confirmation']:
+            if not config.parser.getboolean('confirmations', 'enable'):
+                self.status.info(_(
+                    "Mobile confirmation is needed but the confirmation module isn't enabled.\n"
+                    "You will need to manually confirm the trade offer."
+                ))
+
+                self.header_bar.set_show_title_buttons(True)
+                self.yes_button.set_visible(False)
+                # FIXME: track and wait for manual confirmation
+                self.has_status = True
+                return
+
+            confirmations_tree = self.parent_window.confirmations_tree
+            target = None
+
+            while True:
+                for index in range(confirmations_tree.store.get_n_items()):
+                    item = confirmations_tree.store.get_item(index)
+
+                    if item.creatorid == json_data['tradeofferid']:
+                        confirmations_tree.model.set_selected(index)
+                        break
+
+                if target:
+                    break
+                self.status.info(_('Waiting trade confirmation'))
+                await asyncio.sleep(5)
+
+            finalize_window = confirmation.FinalizeWindow(
+                self.parent_window,
+                self.application,
+                confirmations_tree,
+                'allow',
             )
-        except webapi.SMSCodeError:
-            self.status.info(_("Invalid SMS Code. Please,\ncheck the code and try again."))
-            self.user_details_section.show()
-            self.sms_code_item.set_text('')
-            self.sms_code_item.grab_focus()
-        except aiohttp.ClientError:
-            self.status.error(_("Check your connection. (server down?)"))
-            self.user_details_section.show()
-            self.sms_code_item.set_text('')
-            self.sms_code_item.grab_focus()
-        except Exception as exception:
-            import sys
-            import traceback
-            traceback_info = sys.exc_info()[2]
-            utils.fatal_error_dialog(exception, traceback.extract_tb(traceback_info), self.parent_window)
-            self.application.on_exit_activate()
-        else:
-            self.status.info(_("Saving new secrets"))
-            config.new("login", "shared_secret", self._login_data.auth['shared_secret'])
-            config.new("login", "identity_secret", self._login_data.auth['identity_secret'])
-            config.new("steamguard", "enable", True)
-            config.new("confirmations", "enable", True)
-
-            self.status.info(_(
-                "RECOVERY CODE\n\n"
-                "You will need this code to recovery your Steam Account\n"
-                "if you lose access to STNG Authenticator. So, write"
-                "down this recovery code.\n\n"
-                "YOU WILL NOT ABLE TO VIEW IT AGAIN!\n"
-            ))
-
-            revocation_code = self._login_data.auth['revocation_code']
-
-            self.add_authenticator_button.hide()
-
-            revocation_status = utils.Status(6)
-            revocation_status.set_pausable(False)
-            revocation_status.set_display(revocation_code)
-            revocation_status.set_status('')
-            self.content_area.append(revocation_status)
-
-            revocation_status.show()
-
-            self.set_deletable(False)
-
-            max_value = 30 * 3
-            for offset in range(max_value):
-                revocation_status.set_level(offset, max_value)
-                await asyncio.sleep(0.3)
-
-            self.set_deletable(True)
-        finally:
-            button.set_sensitive(True)
+
+            finalize_window.present()
+            finalize_window.yes_button.emit('clicked')
```

### Comparing `steam-tools-ng-3.0.1/src/steam_tools_ng/gtk/confirmation.py` & `steam-tools-ng-3.1/src/steam_tools_ng/gtk/confirmation.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,153 +12,103 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 # See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see http://www.gnu.org/licenses/.
 #
 import asyncio
-import contextlib
 import logging
-from typing import Any, Dict, List, Tuple, Union
+from typing import Any, Dict, List, Tuple
 
 from gi.repository import Gtk
 
 from stlib import universe, community
 from . import utils
 from .. import config, i18n
 
 log = logging.getLogger(__name__)
 _ = i18n.get_translation
 
 
 # noinspection PyUnusedLocal
-class FinalizeDialog(Gtk.Dialog):
+class FinalizeWindow(utils.PopupWindowBase):
     def __init__(
             self,
             parent_window: Gtk.Window,
             application: Gtk.Application,
+            confirmations_tree: utils.SimpleTextTree,
             action: str,
-            model: Gtk.TreeModel,
-            iter_: Union[Gtk.TreeIter, bool, None] = False,
+            batch: bool = False,
     ) -> None:
-        super().__init__(use_header_bar=True)
-        self.parent_window = parent_window
-        self.application = application
+        super().__init__(parent_window, application)
         self.community_session = community.Community.get_session(0)
+        self.confirmations_tree = confirmations_tree
+        self.selection = self.confirmations_tree.model.get_selected_item()
+        self.batch = batch
 
-        if action == "allow":
-            self.action = _("accept")
-        else:
-            self.action = _("cancel")
-
+        self.action = _("accept") if action == "allow" else _("cancel")
         self.raw_action = action
-        self.model = model
-        self.iter = iter_
-
-        self.header_bar = self.get_header_bar()
         self.header_bar.set_show_title_buttons(False)
-
-        self.set_default_size(300, 60)
         self.set_title(_('Finalize Confirmation'))
-        self.set_transient_for(self.parent_window)
-        self.set_modal(True)
-        self.set_destroy_with_parent(True)
-        self.set_resizable(False)
-
-        self.content_area = self.get_content_area()
-        self.content_area.set_orientation(Gtk.Orientation.VERTICAL)
-        self.content_area.set_spacing(10)
-        self.content_area.set_margin_start(10)
-        self.content_area.set_margin_end(10)
-        self.content_area.set_margin_top(10)
-        self.content_area.set_margin_bottom(10)
 
         self.status = utils.SimpleStatus()
-        self.content_area.append(self.status)
+        self.content_grid.attach(self.status, 0, 0, 1, 1)
 
         self.progress = Gtk.LevelBar()
-        self.content_area.append(self.progress)
+        self.progress.set_visible(False)
+        self.content_grid.attach(self.progress, 0, 1, 1, 1)
 
         self.yes_button = Gtk.Button()
         self.yes_button.set_label(_("Continue"))
         self.yes_button.connect("clicked", self.on_yes_button_clicked)
         self.header_bar.pack_end(self.yes_button)
 
         self.no_button = Gtk.Button()
         self.no_button.set_label(_("Cancel"))
         self.no_button.connect("clicked", lambda button: self.destroy())
         self.header_bar.pack_start(self.no_button)
 
-        if self.iter is None or not model:
-            self.status.error(_("You must select something"))
-            self.header_bar.set_show_title_buttons(True)
-            self.yes_button.hide()
-            self.no_button.hide()
-        elif self.iter is False:
+        if self.batch:
             self.status.info(
                 _("Do you really want to {} ALL confirmations?\nIt can't be undone!").format(self.action.upper())
             )
-        else:
-            self.set_size_request(600, 400)
-
-            self.give_label = Gtk.Label()
-            self.content_area.append(self.give_label)
-
-            self.receive_label = Gtk.Label()
-            self.content_area.append(self.receive_label)
-
-            self.give_label.set_markup(
-                utils.markup(
-                    _("You are trading the following items with {}:").format(utils.unmarkup(self.model[self.iter][4])),
-                    color='blue',
+        elif self.selection:
+            self.status.info(
+                _("{}\nDo you want to {} the offer?\nIt can't be undone!").format(
+                    self.selection.get_item().summary,
+                    self.action.upper(),
+                    utils.unmarkup(self.selection.get_item().to),
                 )
             )
-
-            self.status.info(_("Do you really want to {} that?\nIt can't be undone!").format(self.action.upper()))
-
-            self.grid = Gtk.Grid()
-            self.content_area.append(self.grid)
-
-            self.give_tree = utils.SimpleTextTree(_("You will give"), fixed_width=300, model=Gtk.ListStore)
-            self.grid.attach(self.give_tree, 0, 0, 1, 1)
-
-            self.arrow = Gtk.Image()
-            self.arrow.set_from_icon_name('emblem-synchronizing-symbolic')
-            self.grid.attach(self.arrow, 1, 0, 1, 1)
-
-            self.receive_tree = utils.SimpleTextTree(_("You will receive"), fixed_width=300, model=Gtk.ListStore)
-            self.grid.attach(self.receive_tree, 2, 0, 1, 1)
-
-            utils.copy_childrens(self.model, self.give_tree.store, self.iter, 3)
-            utils.copy_childrens(self.model, self.receive_tree.store, self.iter, 5)
-
-        self.connect('response', lambda dialog, response_id: self.destroy())
+        else:
+            self.status.error(_("You must select something"))
+            self.header_bar.set_show_title_buttons(True)
+            self.yes_button.set_visible(False)
+            self.no_button.set_visible(False)
 
     def on_yes_button_clicked(self, button: Gtk.Button) -> None:
-        button.hide()
-        self.no_button.hide()
-        self.set_size_request(300, 60)
+        button.set_visible(False)
+        self.no_button.set_visible(False)
+        self.progress.set_visible(True)
+        self.set_size_request(0, 0)
         self.header_bar.set_show_title_buttons(False)
-        self.parent_window.confirmations_tree.lock = True
+        self.confirmations_tree.lock = True
 
         loop = asyncio.get_event_loop()
-        task: asyncio.Task[Union[Dict[str, Any], List[Tuple[Gtk.TreeIter, Dict[str, Any]]]]]
 
-        if self.iter:
-            self.content_area.remove(self.grid)
-            self.content_area.remove(self.give_label)
-            self.content_area.remove(self.receive_label)
-            task = loop.create_task(self.finalize())
-        else:
+        if self.batch:
             task = loop.create_task(self.batch_finalize())
+        else:
+            task = loop.create_task(self.single_finalize())
 
         task.add_done_callback(self.on_task_finish)
 
     def on_task_finish(self, task: asyncio.Task[Any]) -> None:
-        self.parent_window.confirmations_tree.lock = False
+        self.progress.set_visible(False)
+        self.confirmations_tree.lock = False
         exception = task.exception()
 
         if exception and not isinstance(exception, asyncio.CancelledError):
             try:
                 current_exception = task.exception()
                 assert isinstance(current_exception, BaseException)
                 raise current_exception
@@ -167,70 +117,74 @@
 
                 for frame in stack:
                     log.error("%s at %s", type(exception).__name__, frame)
 
                 log.error("Steam Server is slow. (%s)", str(exception))
 
                 self.status.error(
-                    _("Steam Server is slow. Please, try again.")
+                    _(
+                        "Unable to complete this confirmation. The reason is one of the following:\n\n"
+                        "1. The confirmation you choose already gone. Try another one.\n"
+                        "2. You wrote a wrong token in config. Update you config.\n"
+                        "3. The Steam server is slow. Wait a minute and try again.\n\n"
+                        "If you keep seeing this error, please update the confirmation list."
+                    )
                 )
 
                 self.header_bar.set_show_title_buttons(True)
-                self.yes_button.hide()
+                self.yes_button.set_visible(False)
         else:
             self.destroy()
 
-    async def finalize(self, keep_iter: bool = False) -> Dict[str, Any]:
+    async def do_finalize(self, item: Gtk.ListItem) -> Dict[str, Any]:
         identity_secret = config.parser.get("login", "identity_secret")
         deviceid = config.parser.get("login", "deviceid")
         steamid_raw = config.parser.getint("login", "steamid")
 
         try:
             steamid = universe.generate_steamid(steamid_raw)
         except ValueError:
             self.status.info(_("Your steam is invalid. (are you logged in?)"))
             await asyncio.sleep(5)
             return {}
 
-        self.status.info(_("Waiting Steam Server (OP: {})").format(self.model[self.iter][1]))
+        self.status.info(_("Waiting Steam Server (OP: {})").format(item.creatorid))
         result: Dict[str, Any] = {}
 
         # steam confirmation server isn't reliable
         for i in range(2):
             result = await self.community_session.send_confirmation(
                 identity_secret,
                 steamid,
                 deviceid,
-                self.model[self.iter][0],
-                self.model[self.iter][2],
+                item.id,
+                item.nonce,
                 self.raw_action,
             )
             await asyncio.sleep(0.5)
 
-        if not keep_iter:
-            try:
-                self.model.remove(self.iter)
-            except IndexError:
-                log.debug(_("Unable to remove tree path %s (already removed?). Ignoring."), self.iter)
+        assert isinstance(result, dict)
+        return result
+
+    async def single_finalize(self) -> Dict[str, Any]:
+        item = self.selection.get_item()
+        result = await self.do_finalize(item)
+        self.confirmations_tree.remove_row(self.selection)
 
         assert isinstance(result, dict)
         return result
 
     async def batch_finalize(self) -> List[Tuple[Gtk.TreeIter, Dict[str, Any]]]:
         results = []
+        n_items = self.confirmations_tree.store.get_n_items()
         self.status.info(_("Waiting Steam Server response"))
-        confirmation_count = len(self.model)
-
-        for index in range(confirmation_count):
-            self.iter = self.model[index].iter
 
+        for index in range(n_items):
             self.progress.set_value(index)
-            self.progress.set_max_value(confirmation_count)
-
-            result = await self.finalize(True)
-            results.append((self.iter, result))
+            self.progress.set_max_value(n_items)
+            item = self.confirmations_tree.store.get_item(index)
+            result = await self.do_finalize(item)
+            results.append((item, result))
 
-        self.status.info(_("Updating tree"))
-        for iter_, result in results:
-            self.model.remove(iter_)
+        self.confirmations_tree.clear()
 
         return results
```

### Comparing `steam-tools-ng-3.0.1/src/steam_tools_ng/gtk/login.py` & `steam-tools-ng-3.1/src/steam_tools_ng/gtk/login.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,100 +11,81 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 # See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see http://www.gnu.org/licenses/.
 #
-import aiohttp
 import asyncio
 import binascii
-import codecs
 import logging
-from gi.repository import Gtk, Gdk, GdkPixbuf
-from typing import Any
+from typing import Any, Optional
+
+import aiohttp
+from gi.repository import Gtk, Gdk
 
-from stlib import login, universe
+from stlib import login
+from stlib.login import AuthCodeType
 from . import utils
-from .. import i18n, config
+from .. import i18n, config, core
 
 log = logging.getLogger(__name__)
 _ = i18n.get_translation
 
 
 # noinspection PyUnusedLocal
-class LoginDialog(Gtk.Dialog):
+class LoginWindow(utils.PopupWindowBase):
     def __init__(
             self,
             parent_window: Gtk.Window,
             application: Gtk.Application,
             mobile_login: bool = True,
     ) -> None:
-        super().__init__(use_header_bar=True)
-        self.application = application
+        super().__init__(parent_window, application)
         self.mobile_login = mobile_login
         self.has_user_data = False
 
-        self.header_bar = self.get_header_bar()
-
         self.login_button = utils.AsyncButton()
         self.login_button.set_label(_("Log-in"))
         self.login_button.connect("clicked", self.on_login_button_clicked)
         self.header_bar.pack_end(self.login_button)
-
-        self.parent_window = parent_window
-        self.set_default_size(400, 100)
         self.set_title(_('Login'))
-        self.set_transient_for(parent_window)
-        self.set_modal(True)
-        self.set_destroy_with_parent(True)
-        self.set_resizable(False)
-
-        self.content_area = self.get_content_area()
-        self.content_area.set_orientation(Gtk.Orientation.VERTICAL)
-        self.content_area.set_spacing(10)
-        self.content_area.set_margin_start(10)
-        self.content_area.set_margin_end(10)
-        self.content_area.set_margin_top(10)
-        self.content_area.set_margin_bottom(10)
 
         self.status = utils.SimpleStatus()
-        self.content_area.append(self.status)
+        self.content_grid.attach(self.status, 0, 0, 1, 1)
 
         self.user_details_section = utils.Section("login")
-        self.content_area.append(self.user_details_section)
+        self.content_grid.attach(self.user_details_section, 0, 1, 1, 1)
 
         self.username_item = self.user_details_section.new_item("account_name", _("Username:"), Gtk.Entry, 0, 0)
 
         self.__password_item = self.user_details_section.new_item("_password", _("Password:"), Gtk.Entry, 0, 1)
         self.__password_item.set_visibility(False)
         self.__password_item.set_invisible_char('*')
 
-        self.steam_code_item = self.user_details_section.new_item("_steam_code", _("Steam Code:"), Gtk.Entry, 0, 2)
-        self.mail_code_item = self.user_details_section.new_item("_mail_code", _("Mail Code:"), Gtk.Entry, 0, 2)
+        self.auth_code_item = self.user_details_section.new_item("_auth_code", _("Code:"), Gtk.Entry, 0, 2)
 
-        self.captcha_gid = -1
-        self.captcha_item = self.user_details_section.new_item("_captcha", _("Code:"), Gtk.Image, 0, 3)
-        self.captcha_item.set_size_request(140, 140)
-        self.captcha_text_item = self.user_details_section.new_item(
-            "_captcha_text", _("Captcha Text:"), Gtk.Entry, 0, 4,
+        self.save_password_item = self.user_details_section.new_item(
+            "_savepwd",
+            _("Save Password:"),
+            Gtk.CheckButton,
+            0, 5,
         )
-
-        self.save_password_item = self.user_details_section.new_item("_savepwd", _("Save Password:"), Gtk.CheckButton,
-                                                                     0, 5)
         self.save_password_item.set_active(True)
 
         self.advanced_login = utils.ClickableLabel()
         self.advanced_login.set_markup(utils.markup(_("Advanced Login"), font_size='x-small', color='blue'))
         self.advanced_login.set_halign(Gtk.Align.END)
+        self.advanced_login.set_margin_end(10)
+        self.advanced_login.set_margin_bottom(10)
         self.advanced_login.connect("clicked", self.on_advanced_login_clicked)
-        self.content_area.append(self.advanced_login)
+        self.content_grid.attach(self.advanced_login, 0, 2, 1, 1)
 
         self.advanced_login_section = utils.Section("login")
-        self.content_area.append(self.advanced_login_section)
+        self.content_grid.attach(self.advanced_login_section, 0, 3, 1, 1)
 
         self.identity_secret_item = self.advanced_login_section.new_item(
             'identity_secret',
             _("Identity Secret:"),
             Gtk.Entry,
             0, 0,
         )
@@ -112,56 +93,40 @@
         self.shared_secret_item = self.advanced_login_section.new_item(
             'shared_secret',
             _("Shared Secret:"),
             Gtk.Entry,
             0, 1,
         )
 
-        self.connect('response', self.on_quit)
-
-        key_event = Gtk.EventControllerKey()
-        key_event.connect('key-released', self.on_key_release_event)
-        self.add_controller(key_event)
-
-        self.steam_code_item.hide()
-        self.mail_code_item.hide()
-        self.captcha_item.hide()
-        self.captcha_text_item.hide()
-        self.advanced_login_section.hide()
+        self.connect('destroy', self.on_quit)
+        self.connect('close-request', self.on_quit)
 
+        self.auth_code_item.set_visible(False)
+        self.advanced_login_section.set_visible(False)
         self.check_login_availability()
 
     @property
     def username(self) -> str:
         return self.username_item.get_text()
 
     @property
     def __password(self) -> str:
         return self.__password_item.get_text()
 
     def set_password(self, encrypted_password: str) -> None:
         try:
-            key = codecs.decode(encrypted_password, 'rot13')
-            raw = codecs.decode(key.encode(), 'base64')
-            self.__password_item.set_text(raw.decode())
+            __password = core.utils.decode_password(encrypted_password)
+            self.__password_item.set_text(__password)
         except (binascii.Error, UnicodeError, TypeError):
             log.warning(_("Password decode failed. Trying RAW."))
             self.__password_item.set_text(encrypted_password)
 
     @property
-    def mail_code(self) -> str:
-        return self.mail_code_item.get_text()
-
-    @property
-    def steam_code(self) -> str:
-        return self.steam_code_item.get_text()
-
-    @property
-    def captcha_text(self) -> str:
-        return self.captcha_text_item.get_text()
+    def auth_code(self) -> str:
+        return self.auth_code_item.get_text()
 
     @property
     def shared_secret(self) -> str:
         return self.shared_secret_item.get_text()
 
     @property
     def identity_secret(self) -> str:
@@ -176,171 +141,164 @@
     def on_quit(self, *args: Any, **kwargs: Any) -> None:
         self.application.main_window.statusbar.set_warning(
             'steamguard',
             _("Login cancelled! Modules will not work correctly!"),
         )
         self.destroy()
 
-    def on_key_release_event(
+    def on_key_released_event(
             self,
             controller: Gtk.EventControllerKey,
             keyval: int,
             keycode: int,
             state: Gdk.ModifierType
     ) -> None:
+        super().on_key_released_event(controller, keyval, keycode, state)
+
         self.check_login_availability()
 
         if keyval == Gdk.KEY_Return:
-            if not self.username or not self.__password:
-                self.status.error(_("Username or Password is blank!"))
-            else:
+            if self.username and self.__password:
                 self.login_button.emit('clicked')
+            else:
+                self.status.error(_("Username or Password is blank!"))
 
-    async def on_login_button_clicked(self, *args: Any) -> None:
+    async def on_login_button_clicked(
+            self,
+            auto: bool,
+            auth_code: str = '',
+            auth_code_type: Optional[AuthCodeType] = AuthCodeType.device,
+    ) -> None:
         self.status.info(_("Retrieving user data"))
         self.application.main_window.statusbar.set_warning("steamguard", _("Not logged in"))
         self.username_item.set_sensitive(False)
         self.__password_item.set_sensitive(False)
         self.save_password_item.set_sensitive(False)
         self.login_button.set_sensitive(False)
 
         _login_session = login.Login.get_session(0)
         _login_session.username = self.username
         _login_session.password = self.__password
 
-        kwargs = {'emailauth': self.mail_code, 'mobile_login': self.mobile_login}
-
-        # no reason to send captcha_text if no gid is found
-        if self.captcha_gid != -1:
-            kwargs['captcha_text'] = self.captcha_text
-            kwargs['captcha_gid'] = self.captcha_gid
-            # if login fails for any reason, gid must be unset
-            # CaptchaError exception will reset it if needed
-            self.captcha_gid = -1
-
-        if not self.shared_secret or not self.identity_secret:
+        if not self.shared_secret:
             log.warning(_("No shared secret found. Trying to log-in without two-factor authentication."))
-            # self.code_item.show()
-
-        kwargs['shared_secret'] = self.shared_secret
-        kwargs['authenticator_code'] = self.steam_code
+            # self.code_item.set_visible(True)
 
         self.status.info(_("Logging in"))
-        self.captcha_item.hide()
-        self.captcha_text_item.hide()
-        self.steam_code_item.hide()
-        self.mail_code_item.hide()
+        self.auth_code_item.set_visible(False)
 
         try_count = 3
 
         while True:
             try:
-                login_data = await _login_session.do_login(**kwargs)
+                login_data = await _login_session.do_login(
+                    self.shared_secret,
+                    self.auth_code if self.auth_code else auth_code,
+                    auth_code_type,
+                    self.mobile_login,
+                )
             except login.MailCodeError:
                 self.status.info(_("Write code received by email\nand click on 'Log-in' button"))
-                self.mail_code_item.set_text("")
-                self.mail_code_item.show()
-                self.mail_code_item.grab_focus()
+                self.auth_code_item.set_text("")
+                self.auth_code_item.set_visible(True)
+                self.auth_code_item.grab_focus()
+                auth_code_type = AuthCodeType.email
             except login.TwoFactorCodeError:
                 if self.shared_secret:
                     if try_count > 0:
-                        log.warning(_("Retrying login in 10 seconds"))
-                        await asyncio.sleep(10)
+                        for count in range(10, 0):
+                            self.status.info(_("Retrying login in {} seconds").format(count))
+                            await asyncio.sleep(1)
+
                         try_count -= 1
                         continue
                     else:
                         self.status.error(_("shared secret is invalid!"))
                         self.username_item.set_sensitive(True)
                         self.__password_item.set_sensitive(True)
                         self.shared_secret_item.grab_focus()
                         break
 
                 self.status.error(_("Write Steam Code bellow and click on 'Log-in'"))
-                self.steam_code_item.set_text("")
-                self.steam_code_item.show()
-                self.steam_code_item.grab_focus()
+                self.auth_code_item.set_text("")
+                self.auth_code_item.set_visible(True)
+                self.auth_code_item.grab_focus()
+                auth_code_type = AuthCodeType.device
             except login.LoginBlockedError:
                 self.status.error(_(
                     "Your network is blocked!\n"
                     "It'll take some time until unblocked. Please, try again later\n"
                 ))
-                self.user_details_section.hide()
-                self.advanced_login.hide()
-                self.advanced_login_section.hide()
-                self.login_button.hide()
+                self.user_details_section.set_visible(False)
+                self.advanced_login.set_visible(False)
+                self.advanced_login_section.set_visible(False)
+                self.login_button.set_visible(False)
                 self.set_deletable(True)
             except login.CaptchaError as exception:
+                # TODO: Captcha gid?? (where did you go? where did you go?)
                 self.status.info(_("Write captcha code as shown bellow\nand click on 'Log-in' button"))
-                self.captcha_gid = exception.captcha_gid
 
-                pixbuf_loader = GdkPixbuf.PixbufLoader()
-                pixbuf_loader.set_size(140, 50)
-                pixbuf_loader.write(exception.captcha)
-                pixbuf_loader.close()
-                self.captcha_item.set_from_pixbuf(pixbuf_loader.get_pixbuf())
+                # pixbuf_loader = GdkPixbuf.PixbufLoader()
+                # pixbuf_loader.set_size(140, 50)
+                # pixbuf_loader.write(exception.captcha)
+                # pixbuf_loader.close()
+                # self.captcha_item.set_from_pixbuf(pixbuf_loader.get_pixbuf())
 
-                self.captcha_item.show()
+                # self.captcha_item.set_visible(True)
                 self.captcha_text_item.set_text("")
-                self.captcha_text_item.show()
+                self.captcha_text_item.set_visible(True)
                 self.captcha_text_item.grab_focus()
             except (login.LoginError, AttributeError) as exception:
                 log.error(str(exception))
                 # self.__password_item.set_text('')
                 self.__password_item.grab_focus()
-                config.remove('login', 'token')
-                config.remove('login', 'token_secure')
-                config.remove('login', 'oauth_token')
+                config.remove('login', 'refresh_token')
+                config.remove('login', 'access_token')
+
+                self.status.error(
+                    ':\n'.join(str(exception).split(': ')) +
+                    _(
+                        '\n\nIf your previous authenticator has been removed,'
+                        '\nopen advanced login bellow and remove the old secrets.'
+                    ),
+                )
 
-                self.status.error(':\n'.join(str(exception).split(': ')))
                 self.username_item.set_sensitive(True)
                 self.__password_item.set_sensitive(True)
                 self.__password_item.grab_focus()
             except binascii.Error:
                 self.status.error(_("shared secret is invalid!"))
                 self.username_item.set_sensitive(True)
                 self.__password_item.set_sensitive(True)
                 self.shared_secret_item.grab_focus()
             except (aiohttp.ClientError, ValueError):
-                self.status.error(_("Check your connection. (server down?)"))
-                await asyncio.sleep(15)
-                continue
-            else:
-                new_configs = {"account_name": self.username}
+                for count in range(20, 0):
+                    self.status.error(_("Check your connection. (server down? blocked?)\nWaiting {}").format(count))
+                    await asyncio.sleep(1)
 
-                if "shared_secret" in login_data.auth:
-                    new_configs["shared_secret"] = login_data.auth["shared_secret"]
-                elif self.shared_secret:
-                    new_configs["shared_secret"] = self.shared_secret
-
-                if "identity_secret" in login_data.auth:
-                    new_configs['identity_secret'] = login_data.auth['identity_secret']
-                elif self.identity_secret:
-                    new_configs["identity_secret"] = self.identity_secret
+                self.username_item.set_sensitive(True)
+                self.__password_item.set_sensitive(True)
+                self.login_button.grab_focus()
+            else:
+                new_configs = {
+                    "account_name": self.username,
+                    'steamid': login_data.steamid,
+                    'refresh_token': login_data.refresh_token,
+                    'access_token': login_data.access_token,
+                }
 
                 if self.save_password_item.get_active():
-                    # Just for curious people. It's not even safe.
-                    key = codecs.encode(self.__password.encode(), 'base64')
-                    out = codecs.encode(key.decode(), 'rot13')
-                    new_configs["password"] = out.replace('\n', '')
-
-                if login_data.oauth:
-                    new_configs['steamid'] = login_data.oauth['steamid']
-                    new_configs['token'] = login_data.oauth['wgtoken']
-                    new_configs['token_secure'] = login_data.oauth['wgtoken_secure']
-                    new_configs['oauth_token'] = login_data.oauth['oauth_token']
-                else:
-                    new_configs['steamid'] = login_data.auth['transfer_parameters']['steamid']
-                    new_configs['token'] = login_data.auth['transfer_parameters']['webcookie']
-                    new_configs['token_secure'] = login_data.auth['transfer_parameters']['token_secure']
+                    encrypted_password = core.utils.encode_password(self.__password)
+                    new_configs["password"] = encrypted_password
 
                 for key_, value_ in new_configs.items():
                     config.new("login", key_, value_)
 
-                steamid = universe.generate_steamid(new_configs['steamid'])
-                _login_session.restore_login(steamid, new_configs['token'], new_configs['token_secure'])
+                # steamid = universe.generate_steamid(new_configs['steamid'])
+                # _login_session.restore_login(steamid, new_configs['token'], new_configs['token_secure'])
 
                 self.application.main_window.statusbar.clear('steamguard')
 
                 self.has_user_data = True
                 self.destroy()
             finally:
                 self.save_password_item.set_sensitive(True)
@@ -349,11 +307,11 @@
 
             break
 
     def on_advanced_login_clicked(self, *args: Any) -> None:
         if self.advanced_login_section.props.visible:
             self.identity_secret_item.set_text('')
             self.shared_secret_item.set_text('')
-            self.advanced_login_section.hide()
+            self.advanced_login_section.set_visible(False)
             self.set_size_request(400, 100)
         else:
-            self.advanced_login_section.show()
+            self.advanced_login_section.set_visible(True)
```

### Comparing `steam-tools-ng-3.0.1/src/steam_tools_ng/gtk/utils.py` & `steam-tools-ng-3.1/src/steam_tools_ng/gtk/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,26 +11,26 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 # See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see http://www.gnu.org/licenses/.
 #
-from collections import OrderedDict
-from xml.etree import ElementTree
-
 import asyncio
 import functools
 import html
 import logging
 import traceback
-from gi.repository import Gtk, Gdk
+from collections import OrderedDict
 from traceback import StackSummary
 from types import FrameType
 from typing import Any, Callable, List, Optional, Union, Type, Tuple
+from xml.etree import ElementTree
+
+from gi.repository import Gtk, Gdk, Gio, GObject
 
 from stlib import internals
 from . import async_gtk
 from .. import i18n, config
 
 log = logging.getLogger(__name__)
 _ = i18n.get_translation
@@ -149,39 +149,91 @@
     def set_critical(self, module: str, message: str) -> None:
         self.messages[module]["critical"] = message
 
     def clear(self, module: str) -> None:
         self.messages[module] = {"warning": "", "critical": ""}
 
 
+class SimpleTextTreeItem(GObject.Object):
+    def __init__(self, *args: str, headers: Tuple[str], **kwargs) -> None:
+        for name, value in kwargs.items():
+            setattr(self, name, value)
+
+        for index, header in enumerate(headers):
+            name = header.replace('_', '').replace(' ', '_').lower()
+
+            try:
+                setattr(self, name, args[index])
+            except IndexError:
+                log.debug(f'{name} param not set in {self}')
+
+        super(GObject.Object, self).__init__()
+        self.children = []
+
+
 class SimpleTextTree(Gtk.Grid):
     def __init__(
             self,
-            *elements: str,
-            overlay_scrolling: bool = True,
+            *headers: str,
+            overlay_scrolling: bool = False,
             resizable: bool = True,
             fixed_width: int = 0,
-            model: Callable[..., Union[Gtk.TreeStore, Gtk.ListStore]] = Gtk.TreeStore,
     ) -> None:
         super().__init__()
+        self.headers = headers
+
         self._scrolled_window = Gtk.ScrolledWindow()
         self._scrolled_window.set_overlay_scrolling(overlay_scrolling)
         self.attach(self._scrolled_window, 0, 0, 1, 1)
 
-        # noinspection PyUnusedLocal
-        self._store = model(*[str for header in elements])
-        self._view = Gtk.TreeView()
-        self._view.set_model(self._store)
+        self._view = Gtk.ColumnView()
+        self._view.set_show_column_separators(True)
         self._view.set_hexpand(True)
         self._view.set_vexpand(True)
         self._scrolled_window.set_child(self._view)
 
+        expander_column = Gtk.ColumnViewColumn()
+        expander_column.set_resizable(False)
+        expander_column.set_fixed_width(25)
+        expander_factory = Gtk.SignalListItemFactory()
+        expander_factory.connect('setup', self.setup, False)
+        expander_factory.connect('bind', self.bind)
+        expander_column.set_factory(expander_factory)
+        self._view.append_column(expander_column)
+
+        for element in self.headers:
+            column = Gtk.ColumnViewColumn()
+            column.set_resizable(resizable)
+
+            if element.startswith('_'):
+                element = element[1:]
+                column.set_title(_(element))
+
+            if fixed_width:
+                column.set_fixed_width(fixed_width)
+
+            factory = Gtk.SignalListItemFactory()
+            factory.connect('setup', self.setup)
+            factory.connect('bind', self.bind, element)
+            column.set_factory(factory)
+            self._view.append_column(column)
+
+        self._store = Gio.ListStore.new(SimpleTextTreeItem)
+        self._tree = Gtk.TreeListModel.new(self._store, False, False, self.item_factory)
+        self._tree_sort = Gtk.TreeListRowSorter()
+        self._tree_sort.set_sorter(self._view.get_sorter())
+        self._list_sort = Gtk.SortListModel()
+        self._list_sort.set_sorter(self._tree_sort)
+        self._list_sort.set_model(self._tree)
+        self._model = Gtk.SingleSelection.new(self._list_sort)
+        self._view.set_model(self._model)
+
         self._lock = False
         self._lock_label = Gtk.Label()
-        self._lock_label.hide()
+        self._lock_label.set_visible(False)
         self._lock_label.set_vexpand(True)
         self._lock_label.set_hexpand(True)
 
         self._lock_label.set_markup(
             markup(
                 _("Waiting another process"),
                 background="#0000FF77",
@@ -190,39 +242,87 @@
             )
         )
 
         self.attach(self._lock_label, 0, 0, 1, 1)
 
         self._disabled = False
         self._disabled_label = Gtk.Label()
-        self._disabled_label.hide()
+        self._disabled_label.set_visible(False)
         self._disabled_label.set_vexpand(True)
         self._disabled_label.set_hexpand(True)
 
         self._disabled_label.set_markup(
             markup(
                 _("Disabled"),
                 background="#FF000077",
                 color="white",
                 font_size="xx-large",
             )
         )
 
         self.attach(self._disabled_label, 0, 0, 1, 1)
 
-        renderer = Gtk.CellRendererText()
+    def setup(self, view: Gtk.ListView, item: Gtk.ListItem, hide_expander: bool = True) -> None:
+        expander = Gtk.TreeExpander()
+        expander.set_hide_expander(hide_expander)
+        label = Gtk.Label()
+        expander.set_child(label)
+        item.set_child(expander)
 
-        for index, header in enumerate(elements):
-            column = Gtk.TreeViewColumn(header, renderer, markup=index)
-            column.set_resizable(resizable)
+    def bind(self, view: Gtk.ListView, item: Gtk.ListItem, element: Optional[str] = None) -> None:
+        expander = item.get_child()
+        assert isinstance(expander, Gtk.TreeExpander)
 
-            if fixed_width:
-                column.set_fixed_width(fixed_width)
+        label = expander.get_child()
+        assert isinstance(label, Gtk.Label)
 
-            self._view.append_column(column)
+        list_row = item.get_item()
+        expander.set_list_row(list_row)
+        data = list_row.get_item()
+
+        if isinstance(data, Gtk.TreeListRow):
+            data = data.get_item()
+
+        if element:
+            column_text = getattr(data, element.replace(' ', '_').lower())
+            label.set_markup(column_text)
+            label.set_hexpand(True)
+
+    def item_factory(self, item: Gtk.ListItem) -> Optional[Gtk.TreeListModel]:
+        store = Gio.ListStore.new(SimpleTextTreeItem)
+
+        if type(item) == Gtk.TreeListRow:
+            item = item.get_item()
+
+        if item.children:
+            for child in item.children:
+                store.append(child)
+
+            return Gtk.TreeListModel.new(store, False, False, self.item_factory)
+
+        return None
+
+    def new_item(self, *data: List[str], **kwargs) -> SimpleTextTreeItem:
+        return SimpleTextTreeItem(*data, headers=self.headers, **kwargs)
+
+    def append_row(self, row: Gtk.TreeListRow) -> None:
+        self._store.append(row)
+
+    def remove_row(self, row: Gtk.TreeListRow) -> bool:
+        item = row.get_item()
+        found, position = self._store.find(item)
+
+        if found:
+            self._store.remove(position)
+            return True
+        else:
+            return False
+
+    def clear(self) -> None:
+        self._store.remove_all()
 
     async def wait_available(self) -> None:
         while self.lock or self.disabled:
             await asyncio.sleep(1)
 
     @property
     def lock(self) -> bool:
@@ -230,47 +330,55 @@
 
     @lock.setter
     def lock(self, enable_lock: bool) -> None:
         if enable_lock:
             log.debug(_("Waiting another process"))
             self.set_focusable(False)
             self.set_sensitive(False)
-            self._lock_label.show()
+            self._lock_label.set_visible(True)
             self._lock = True
         else:
             self.set_focusable(True)
             self.set_sensitive(True)
-            self._lock_label.hide()
+            self._lock_label.set_visible(False)
             self._lock = False
 
     @property
     def disabled(self) -> bool:
         return self._disabled
 
     @disabled.setter
     def disabled(self, disabled: bool) -> None:
         if disabled:
             self.set_focusable(False)
             self.set_sensitive(False)
-            self._disabled_label.show()
+            self._disabled_label.set_visible(True)
             self._disabled = True
         else:
             self.set_focusable(True)
             self.set_sensitive(True)
-            self._disabled_label.hide()
+            self._disabled_label.set_visible(False)
             self._disabled = False
 
     @property
-    def store(self) -> Union[Gtk.TreeStore, Gtk.ListStore]:
+    def tree(self) -> Gtk.TreeListModel:
+        return self._tree
+
+    @property
+    def store(self) -> Gio.ListStore:
         return self._store
 
     @property
-    def view(self) -> Gtk.TreeView:
+    def view(self) -> Gtk.ColumnView:
         return self._view
 
+    @property
+    def model(self) -> Gtk.SingleSelection:
+        return self._model
+
 
 class SimpleStatus(Gtk.Frame):
     def __init__(self) -> None:
         super().__init__()
         self._style_context = self.get_style_context()
         self._style_provider = Gtk.CssProvider()
         self._style_provider.load_from_data(b"frame { background-color: black; }")
@@ -284,15 +392,15 @@
         self.set_child(self._grid)
 
         self._label = Gtk.Label()
         self._label.set_halign(Gtk.Align.START)
         self._grid.attach(self._label, 0, 0, 1, 1)
 
         self.info(_("Waiting"))
-        self.set_size_request(100, 60)
+        self.set_hexpand(True)
 
     def error(self, text: str) -> None:
         self._label.set_markup(markup(text, color='hotpink', face='monospace'))
 
     def info(self, text: str) -> None:
         self._label.set_markup(markup(text, color='cyan', face='monospace'))
 
@@ -352,25 +460,22 @@
 
     @property
     def play_event(self) -> asyncio.Event:
         return self._play_event
 
     @play_event.setter
     def play_event(self, value: bool) -> None:
-        if value is True:
+        if value:
             self._play_event.set()
         else:
             self._play_event.clear()
 
     @staticmethod
     def __sanitize_text(text: str, max_length: int) -> str:
-        if len(text) >= max_length:
-            return text[:max_length] + '...'
-
-        return text
+        return f'{text[:max_length]}...' if len(text) >= max_length else text
 
     def __disable_tooltip(self, event_status: Gtk.Label) -> None:
         self._grid.remove(event_status)
         self._grid.attach(self._status, 0, 1, 1, 1)
         self._display.set_has_tooltip(False)
         self._display.set_sensitive(True)
 
@@ -400,18 +505,18 @@
             button.set_icon_name("media-playback-pause")
             self.play_event.set()
         else:
             button.set_icon_name("media-playback-start")
             self.play_event.clear()
 
     def set_pausable(self, value: bool = True) -> None:
-        if value is True:
-            self._play_pause_button.show()
+        if value:
+            self._play_pause_button.set_visible(True)
         else:
-            self._play_pause_button.hide()
+            self._play_pause_button.set_visible(False)
 
     @when_running
     def set_display(self, text: str) -> None:
         text = self.__sanitize_text(text, 25)
         self._display.set_markup(markup(text, font_size='large', font_weight='bold'))
 
     @when_running
@@ -454,40 +559,76 @@
 
     def unset_level(self) -> None:
         self._level_bar.set_value(0)
         self._level_bar.set_max_value(0)
 
 
 class Section(Gtk.Grid):
+    items = []
+
     def __init__(self, name: str) -> None:
         super().__init__()
         # for backward compatibility
         self.grid = self
 
         self.set_name(name)
         self.set_row_spacing(10)
         self.set_column_spacing(10)
         self.set_margin_top(10)
         self.set_margin_bottom(10)
+        self.set_margin_start(10)
+        self.set_margin_end(10)
 
     # noinspection PyProtectedMember
     @staticmethod
     def __get_section_name(item: 'Item') -> str:
         assert isinstance(item._section_name, str)
         return item._section_name
 
     @staticmethod
-    def __show(item: 'Item') -> None:
-        item.label.show()
-        super(item.__class__, item).show()
+    def __set_visible(item: 'Item', state: bool) -> None:
+        item.label.set_visible(state)
+        super(item.__class__, item).set_visible(state)
 
     @staticmethod
-    def __hide(item: 'Item') -> None:
-        item.label.hide()
-        super(item.__class__, item).hide()
+    def __update_values(item: 'Item', items: Optional[OrderedDict[str, str]] = None) -> None:
+        if isinstance(item, Gtk.DropDown):
+            assert isinstance(items, OrderedDict), "DropDown needs items mapping"
+            value = config.parser.get(item.get_section_name(), item.get_name())
+            string_list = Gtk.StringList()
+
+            for option_label in items.values():
+                string_list.append(_(option_label))
+
+            item.set_model(string_list)
+
+            try:
+                current_option = list(items).index(value)
+            except ValueError:
+                import sys
+
+                error_message = _("Please, fix your config file. Accepted values for {} are:\n{}").format(
+                    item.get_name(),
+                    ', '.join(items.keys()),
+                )
+                log.exception(error_message)
+                traceback_info = sys.exc_info()[2]
+                fatal_error_dialog(ValueError(error_message), traceback.extract_tb(traceback_info))
+                # unset active item
+                current_option = -1
+
+            item.set_selected(current_option)
+
+        if isinstance(item, (Gtk.CheckButton, Gtk.Switch)):
+            value = config.parser.getboolean(item.get_section_name(), item.get_name())
+            item.set_active(value)
+
+        if isinstance(item, Gtk.Entry):
+            if value := config.parser.get(item.get_section_name(), item.get_name()):
+                item.set_text(value)
 
     def new_item(
             self,
             name: str,
             label: Optional[str],
             widget: Type[Gtk.Widget],
             *grid_position: int,
@@ -496,23 +637,22 @@
         bases = (widget,)
 
         body = {
             'label': None,
             '_section_name': None,
             '__init__': lambda item_: super(item_.__class__, item_).__init__(),
             'get_section_name': self.__get_section_name,
-            'show': self.__show,
-            'hide': self.__hide,
+            'set_visible': self.__set_visible,
+            'update_values': lambda item_: self.__update_values(item_, items)
         }
 
         if label:
             body['label'] = Gtk.Label()
 
         section = self.get_name()
-        option = name
         value: Union[str, bool, int]
 
         item = type('Item', bases, body)()
         assert isinstance(item, Gtk.Widget)
 
         item.set_hexpand(True)
         item.set_name(name)
@@ -524,50 +664,18 @@
             item.label.set_halign(Gtk.Align.START)
 
             self.grid.attach(item.label, *grid_position, 1, 1)
             self.grid.attach_next_to(item, item.label, Gtk.PositionType.RIGHT, 1, 1)
         else:
             self.grid.attach(item, *grid_position, 1, 1)
 
-        if name.startswith('_'):
-            return item
-
-        if isinstance(item, Gtk.ComboBoxText):
-            assert isinstance(items, OrderedDict), "ComboBox needs items mapping"
-            value = config.parser.get(section, option)
-
-            for option_label in items.values():
-                item.append_text(_(option_label))
-
-            try:
-                current_option = list(items).index(value)
-            except ValueError:
-                import sys
+        self.items.append(item)
 
-                error_message = _("Please, fix your config file. Accepted values for {} are:\n{}").format(
-                    option,
-                    ', '.join(items.keys()),
-                )
-                log.exception(error_message)
-                traceback_info = sys.exc_info()[2]
-                fatal_error_dialog(ValueError(error_message), traceback.extract_tb(traceback_info))
-                # unset active item
-                current_option = -1
-
-            item.set_active(current_option)
-
-        if isinstance(item, Gtk.CheckButton) or isinstance(item, Gtk.Switch):
-            value = config.parser.getboolean(section, option)
-            item.set_active(value)
-
-        if isinstance(item, Gtk.Entry):
-            value = config.parser.get(section, option)
-
-            if value:
-                item.set_text(value)
+        if not name.startswith('_'):
+            item.update_values()
 
         return item
 
     def stackup_section(self, text: str, stack: Gtk.Stack, *, scroll: bool = False) -> None:
         name = self.get_name()
 
         if scroll:
@@ -575,63 +683,77 @@
             scroll.set_overlay_scrolling(True)
             scroll.set_child(self)
             stack.add_titled(scroll, name, text)
         else:
             stack.add_titled(self, name, text)
 
 
+class PopupWindowBase(Gtk.Window):
+    def __init__(self, parent_window: Gtk.Window, application: Gtk.Application) -> None:
+        super().__init__()
+        self.parent_window = parent_window
+        self.application = application
+
+        self.set_default_size(400, 50)
+        self.set_transient_for(parent_window)
+        self.set_destroy_with_parent(True)
+        self.set_modal(True)
+        self.set_resizable(False)
+
+        self.header_bar = Gtk.HeaderBar()
+        self.set_titlebar(self.header_bar)
+
+        self.gtk_settings_class = Gtk.Settings.get_default()
+
+        self.content_grid = Gtk.Grid()
+        self.content_grid.set_row_spacing(10)
+        self.content_grid.set_column_spacing(10)
+        self.set_child(self.content_grid)
+
+        self.connect('destroy', lambda *args: self.destroy())
+        self.connect('close-request', lambda *args: self.destroy())
+
+        self.key_event = Gtk.EventControllerKey()
+        self.add_controller(self.key_event)
+
+        self.key_event.connect('key-released', self.on_key_released_event)
+
+    def on_key_released_event(
+            self,
+            controller: Gtk.EventControllerKey,
+            keyval: int,
+            keycode: int,
+            state: Gdk.ModifierType
+    ) -> None:
+        if keyval == Gdk.KEY_Escape:
+            self.destroy()
+
+
 def markup(text: str, **kwargs: Any) -> str:
     markup_string = ['<span']
 
-    for key, value in kwargs.items():
-        markup_string.append(f'{key}="{value}"')
-
+    markup_string.extend(f'{key}="{value}"' for key, value in kwargs.items())
     markup_string.append(f'>{html.escape(text)}</span>')
 
     return ' '.join(markup_string)
 
 
 def unmarkup(text: str) -> str:
     tree = ElementTree.fromstring(text)
     assert isinstance(tree.text, str)
     return tree.text
 
 
-def copy_childrens(from_model: Gtk.TreeModel, to_model: Gtk.TreeModel, iter_: Gtk.TreeIter, column: int) -> None:
-    childrens = from_model.iter_n_children(iter_)
-
-    if childrens:
-        for index in range(childrens):
-            children_iter = from_model.iter_nth_child(iter_, index)
-            value = from_model.get_value(children_iter, column)
-
-            if value:
-                to_model.append([value])
-            else:
-                log.debug(
-                    _("Ignoring value from {} on column {} item {} because value is empty").format(
-                        children_iter,
-                        column,
-                        index
-                    )
-                )
-    else:
-        value = from_model.get_value(iter_, column)
-        to_model.append([value])
-
-
 def sanitize_confirmation(value: Optional[List[str]]) -> str:
     if not value:
-        result = _("Nothing")
+        return _("Nothing")
     elif len(value) == 1:
-        result = value[0]
+        return value[0]
     else:
-        result = _("Various")
-
-    return result
+        return _("Various")
 
 
 def sanitize_package_details(package_details: List[internals.Package]) -> List[internals.Package]:
     previous: Optional[Tuple[internals.Package, int, int]] = None
 
     for package in package_details:
         for index, app in enumerate(package.apps):
@@ -643,57 +765,44 @@
                 return package_details
 
     assert isinstance(previous, tuple)
     return [previous[0]]
 
 
 def remove_letters(text: str) -> str:
-    new_text = []
-
-    for char in text:
-        if char.isdigit():
-            new_text.append(char)
-
+    new_text = [char for char in text if char.isdigit()]
     return ''.join(new_text)
 
 
 def fatal_error_dialog(
         exception: BaseException,
         stack: Optional[Union[StackSummary, List[FrameType]]] = None,
-        transient: Optional[Gtk.Window] = None,
+        parent: Optional[Gtk.Window] = None,
 ) -> None:
     log.critical("%s: %s", type(exception).__name__, str(exception))
 
-    error_dialog = Gtk.MessageDialog()
-    error_dialog.set_transient_for(transient)
-    error_dialog.set_title(_("Fatal Error"))
-    error_dialog.set_markup(f"{type(exception).__name__}: {str(exception)}")
+    error_dialog = Gtk.AlertDialog()
+    error_dialog.set_buttons([_("Ok")])
+    error_dialog.set_message(f"{type(exception).__name__} > {str(exception)}")
     error_dialog.set_modal(True)
 
-    message_area = error_dialog.get_message_area()
-    secondary_text = Gtk.Label()
-    message_area.append(secondary_text)
-
     if stack:
         log.critical("\n".join([str(frame) for frame in stack]))
-        secondary_text.set_text("\n".join([str(frame) for frame in stack]))
+        error_dialog.set_detail("\n".join([str(frame) for frame in stack]))
 
-    def callback(dialog: Any, _action: Any) -> None:
+    def callback(*args: Any) -> None:
         loop = asyncio.get_event_loop()
         loop.stop()
 
         application = Gtk.Application.get_default()
 
         if application:
             application.quit()
 
-    error_dialog.add_button(_('Ok'), Gtk.ResponseType.OK)
-    error_dialog.connect("response", callback)
-
-    error_dialog.show()
+    error_dialog.choose(parent=parent, callback=callback)
 
     # main application can be not available (like on initialization process)
     if not Gtk.Application.get_default():
         async_gtk.run()
 
 
 def safe_task_callback(task: asyncio.Task[Any]) -> None:
@@ -734,13 +843,13 @@
         config.new(section, option, int(current_value))
     else:
         entry.handler_block_by_func(on_digit_only_setting_changed)
         entry.set_text(remove_letters(current_value))
         entry.handler_unblock_by_func(on_digit_only_setting_changed)
 
 
-def on_combo_setting_changed(combo: Gtk.ComboBoxText, items: OrderedDict[str, str]) -> None:
-    current_value = list(items)[combo.get_active()]
-    section = combo.get_section_name()
-    option = combo.get_name()
+def on_dropdown_setting_changed(dropdown: 'Item', _spec: Any, items: OrderedDict[str, str]) -> None:
+    current_value = list(items)[dropdown.get_selected()]
+    section = dropdown.get_section_name()
+    option = dropdown.get_name()
 
     config.new(section, option, current_value)
```

### Comparing `steam-tools-ng-3.0.1/src/steam_tools_ng/gtk/window.py` & `steam-tools-ng-3.1/src/steam_tools_ng/gtk/window.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,23 +15,23 @@
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see http://www.gnu.org/licenses/.
 #
 
 import asyncio
 import contextlib
 import logging
-from gi.repository import Gio, Gtk, Gdk
 from subprocess import call
-from typing import Union, Optional, Tuple, Any, List
+from typing import Optional, Tuple, Any
+
+from gi.repository import Gio, Gtk, Gdk
 
 import stlib
-from stlib import login, universe, plugins
-from . import confirmation, utils, coupon
-from .authenticator import NewAuthenticatorDialog
-from .login import LoginDialog
+from stlib import login, plugins
+from . import confirmation, utils, coupon, authenticator
+from .login import LoginWindow
 from .. import config, i18n, core
 
 _ = i18n.get_translation
 log = logging.getLogger(__name__)
 
 if stlib.steamworks_available:
     from stlib import client
@@ -68,15 +68,15 @@
         menu.append(_("Exit"), "app.exit")
 
         menu_button = Gtk.MenuButton()
         menu_button.set_icon_name("open-menu")
         menu_button.set_menu_model(menu)
         header_bar.pack_end(menu_button)
 
-        self.set_default_size(650, 10)
+        self.set_default_size(750, 10)
         self.set_resizable(False)
 
         if config.parser.getboolean("general", "show_close_button"):
             self.set_deletable(True)
         else:
             self.set_deletable(False)
 
@@ -86,40 +86,52 @@
         main_grid = Gtk.Grid()
         main_grid.set_margin_start(10)
         main_grid.set_margin_end(10)
         main_grid.set_margin_top(10)
         main_grid.set_margin_bottom(10)
         self.set_child(main_grid)
 
+        self.limited_label = Gtk.Label()
+        self.limited_label.set_visible(False)
+        self.limited_label.set_markup(
+            utils.markup(
+                _("Limited Account! Some modules will not work!"),
+                background='red',
+                color='white',
+            )
+        )
+        main_grid.attach(self.limited_label, 1, 0, 1, 1)
+
         self.user_info_label = Gtk.Label()
         self.user_info_label.set_halign(Gtk.Align.END)
         header_bar.pack_start(self.user_info_label)
 
-        main_tabs = Gtk.Stack()
-        main_tabs.set_hhomogeneous(True)
-        main_grid.attach(main_tabs, 1, 2, 1, 1)
+        self.main_tabs = Gtk.Stack()
+        self.main_tabs.set_hhomogeneous(True)
+        self.main_tabs.connect("notify::visible-child", self.on_stack_child_changed)
+        main_grid.attach(self.main_tabs, 1, 2, 1, 1)
 
         switcher = Gtk.StackSwitcher()
-        switcher.set_stack(main_tabs)
+        switcher.set_stack(self.main_tabs)
         main_grid.attach(switcher, 1, 1, 1, 1)
 
         steamguard_section = utils.Section("steamguard")
-        steamguard_section.stackup_section("SteamGuard", main_tabs)
+        steamguard_section.stackup_section("SteamGuard", self.main_tabs)
 
         cardfarming_section = utils.Section("cardfarming")
-        cardfarming_section.stackup_section("CardFarming", main_tabs)
+        cardfarming_section.stackup_section("CardFarming", self.main_tabs)
 
         steamgifts_section = utils.Section("steamgifts")
-        steamgifts_section.stackup_section("SteamGifts", main_tabs)
+        steamgifts_section.stackup_section("SteamGifts", self.main_tabs)
 
         steamtrades_section = utils.Section("steamtrades")
-        steamtrades_section.stackup_section("SteamTrades", main_tabs)
+        steamtrades_section.stackup_section("SteamTrades", self.main_tabs)
 
         coupons_section = utils.Section("coupons")
-        coupons_section.stackup_section(_("Coupons"), main_tabs)
+        coupons_section.stackup_section(_("Coupons"), self.main_tabs)
 
         # grid managed by plugin switch
         self.steamguard_status = utils.Status(4)
         self.cardfarming_status = utils.Status(6)
         self.steamgifts_status = utils.Status(5)
         self.steamtrades_status = utils.Status(5)
 
@@ -134,169 +146,167 @@
         steamguard_sidebar.set_size_request(150, -1)
         steamguard_section.grid.attach(steamguard_sidebar, 0, 1, 1, 1)
 
         self.confirmations_grid = Gtk.Grid()
         self.confirmations_grid.set_row_spacing(10)
         steamguard_stack.add_titled(self.confirmations_grid, "confirmations", _("Confirmations"))
 
-        self.confirmations_tree = utils.SimpleTextTree(
-            _('confid'), _('creatorid'), _('key'), _('give'), _('to'), _('receive'),
-            overlay_scrolling=False,
-        )
-
+        confirmation_tree_headers = 'id', 'creatorid', 'nonce', '_give', '_to', '_receive', 'summary',
+        self.confirmations_tree = utils.SimpleTextTree(*confirmation_tree_headers)
         self.confirmations_grid.attach(self.confirmations_tree, 0, 0, 4, 1)
 
         for index, column in enumerate(self.confirmations_tree.view.get_columns()):
-            if index in (0, 1, 2):
+            column.set_resizable(True)
+
+            if index in (1, 2, 3, 7):
                 column.set_visible(False)
 
-            if index == 4:
-                column.set_fixed_width(100)
-            else:
-                column.set_fixed_width(200)
+            if index in (4, 6):
+                column.set_fixed_width(190)
 
-        self.confirmations_tree.view.set_has_tooltip(True)
-        self.confirmations_tree.view.connect('query-tooltip', self.on_query_confirmations_tooltip)
+            if index == 5:
+                column.set_fixed_width(100)
 
-        confirmation_tree_selection = self.confirmations_tree.view.get_selection()
-        confirmation_tree_selection.connect("changed", self.on_tree_selection_changed)
+        self.confirmations_tree.model.connect("selection-changed", self.on_tree_selection_changed)
 
         accept_button = Gtk.Button()
         accept_button.set_margin_start(3)
         accept_button.set_margin_end(3)
         accept_button.set_label(_('Accept'))
-        accept_button.connect('clicked', self.on_validate_confirmations, "allow", confirmation_tree_selection)
+        accept_button.connect('clicked', self.on_validate_confirmations, "allow")
         self.confirmations_grid.attach(accept_button, 0, 1, 1, 1)
 
         cancel_button = Gtk.Button()
         cancel_button.set_margin_start(3)
         cancel_button.set_margin_end(3)
         cancel_button.set_label(_('Cancel'))
-        cancel_button.connect('clicked', self.on_validate_confirmations, "cancel", confirmation_tree_selection)
+        cancel_button.connect('clicked', self.on_validate_confirmations, "cancel")
         self.confirmations_grid.attach(cancel_button, 1, 1, 1, 1)
 
         accept_all_button = Gtk.Button()
         accept_all_button.set_margin_start(3)
         accept_all_button.set_margin_end(3)
         accept_all_button.set_label(_('Accept All'))
-        accept_all_button.connect('clicked', self.on_validate_confirmations, "allow", self.confirmations_tree.store)
+        accept_all_button.connect('clicked', self.on_validate_confirmations, "allow", True)
         self.confirmations_grid.attach(accept_all_button, 2, 1, 1, 1)
 
         cancel_all_button = Gtk.Button()
         cancel_all_button.set_margin_start(3)
         cancel_all_button.set_margin_end(3)
         cancel_all_button.set_label(_('Cancel All'))
-        cancel_all_button.connect('clicked', self.on_validate_confirmations, "cancel", self.confirmations_tree.store)
+        cancel_all_button.connect('clicked', self.on_validate_confirmations, "cancel", True)
         self.confirmations_grid.attach(cancel_all_button, 3, 1, 1, 1)
 
         steamguard_settings = utils.Section("steamguard")
         steamguard_settings.stackup_section(_("Settings"), steamguard_stack)
         steamguard_settings.grid.set_halign(Gtk.Align.CENTER)
 
-        steamguard_enable = steamguard_settings.new_item("enable", _("Enable:"), Gtk.Switch, 0, 0)
-        steamguard_enable.set_margin_top(40)
-        steamguard_enable.label.set_margin_top(40)
-        steamguard_enable.set_halign(Gtk.Align.END)
-        steamguard_enable.connect("state-set", utils.on_setting_state_set)
-
-        if not config.parser.get("login", "shared_secret"):
-            self.steamguard_status.set_sensitive(False)
-            steamguard_enable.set_active(False)
-            _steamguard_disabled = Gtk.Label()
-            _steamguard_disabled.set_justify(Gtk.Justification.CENTER)
-            _steamguard_disabled.set_halign(Gtk.Align.CENTER)
-
-            _message = _(
-                "steamguard module has been disabled because you have\n"
-                "logged in but no shared secret is found. To enable it again,\n"
-                "go to Advanced and add a valid shared secret\n"
-                "or use STNG as your Steam Authenticator\n"
-            )
-
-            _steamguard_disabled.set_markup(utils.markup(_message, color="hotpink", background="black"))
-            steamguard_section.grid.attach(_steamguard_disabled, 0, 0, 2, 1)
+        self.steamguard_enable = steamguard_settings.new_item("enable", _("Enable:"), Gtk.Switch, 0, 0)
+        self.steamguard_enable.set_margin_top(40)
+        self.steamguard_enable.label.set_margin_top(40)
+        self.steamguard_enable.set_halign(Gtk.Align.END)
+        self.steamguard_enable.connect("state-set", utils.on_setting_state_set)
+
+        self.steamguard_disabled = Gtk.Label()
+        self.steamguard_disabled.set_justify(Gtk.Justification.CENTER)
+        self.steamguard_disabled.set_halign(Gtk.Align.CENTER)
+
+        _message = _(
+            "steamguard module has been disabled because you have\n"
+            "logged in but no shared secret is found. To enable it again,\n"
+            "go to Advanced and add a valid shared secret\n"
+            "or use STNG as your Steam Authenticator\n"
+        )
+
+        self.steamguard_disabled.set_markup(utils.markup(_message, color="hotpink", background="black"))
+        self.steamguard_disabled.set_visible(False)
+        steamguard_section.grid.attach(self.steamguard_disabled, 0, 0, 2, 1)
 
-        confirmations_enable = steamguard_settings.new_item(
+        self.confirmations_enable = steamguard_settings.new_item(
             "enable_confirmations", _("Enable Confirmations:"),
             Gtk.Switch,
             0, 1,
         )
 
-        confirmations_enable.set_halign(Gtk.Align.END)
-        confirmations_enable.connect("state-set", utils.on_setting_state_set)
+        self.confirmations_enable.set_halign(Gtk.Align.END)
+        self.confirmations_enable.connect("state-set", utils.on_setting_state_set)
 
-        if not config.parser.get("login", "identity_secret"):
-            self.confirmations_grid.set_sensitive(False)
-            confirmations_enable.set_active(False)
-            _confirmations_disabled = Gtk.Label()
-            _confirmations_disabled.set_justify(Gtk.Justification.CENTER)
-            _confirmations_disabled.set_halign(Gtk.Align.CENTER)
-
-            _message = _(
-                "confirmations module has been disabled because you have\n"
-                "logged in but no identity secret is found. To enable it again,\n"
-                "go to login -> advanced and add a valid identity secret\n"
-                "or use STNG as your Steam Authenticator\n"
-            )
-
-            _confirmations_disabled.set_markup(utils.markup(_message, color="hotpink", background="black"))
-            self.confirmations_grid.attach(_confirmations_disabled, 0, 0, 4, 1)
+        self.confirmations_disabled = Gtk.Label()
+        self.confirmations_disabled.set_justify(Gtk.Justification.CENTER)
+        self.confirmations_disabled.set_halign(Gtk.Align.CENTER)
+
+        _message = _(
+            "confirmations module has been disabled because you have\n"
+            "logged in but no identity secret is found. To enable it again,\n"
+            "go to login -> advanced and add a valid identity secret\n"
+            "or use STNG as your Steam Authenticator\n"
+        )
+
+        self.confirmations_disabled.set_markup(utils.markup(_message, color="hotpink", background="black"))
+        self.confirmations_disabled.set_visible(False)
+        self.confirmations_grid.attach(self.confirmations_disabled, 0, 0, 4, 1)
 
         login_button = Gtk.Button()
         login_button.set_margin_top(40)
         login_button.set_label(_("Login with another account"))
         login_button.set_name("login_button")
         login_button.connect('clicked', self.on_login_button_clicked)
         steamguard_settings.grid.attach(login_button, 0, 2, 2, 1)
 
         new_authenticator_button = Gtk.Button()
-        new_authenticator_button.set_label(_("Use STNG as your Steam Authenticator"))
+        new_authenticator_button.set_label(_("Add STNG as your Steam Authenticator"))
         new_authenticator_button.set_name("new_authenticator_button")
         new_authenticator_button.connect("clicked", self.on_new_authenticator_clicked)
         steamguard_settings.grid.attach(new_authenticator_button, 0, 3, 2, 1)
 
+        remove_authenticator_button = Gtk.Button()
+        remove_authenticator_button.set_label(_("Remove STNG Authenticator from your Steam Account"))
+        remove_authenticator_button.set_name("remove_authenticator_button")
+        remove_authenticator_button.connect("clicked", self.on_remove_authenticator_clicked)
+        steamguard_settings.grid.attach(remove_authenticator_button, 0, 4, 2, 1)
+
         reset_password_button = Gtk.Button()
         reset_password_button.set_label(_("Remove Saved Password"))
         reset_password_button.set_name("reset_password_button")
         reset_password_button.connect("clicked", self.on_reset_password_clicked)
-        steamguard_settings.grid.attach(reset_password_button, 0, 4, 2, 1)
+        steamguard_settings.grid.attach(reset_password_button, 0, 5, 2, 1)
 
         steamguard_advanced = utils.Section("login")
         steamguard_advanced.stackup_section(_("Advanced"), steamguard_stack, scroll=True)
 
         warning_label = Gtk.Label()
         warning_label.set_markup(utils.markup(
             _("Warning: Don't mess up these settings unless you know what you are doing!"),
             color='darkred' if self.theme == 'light' else 'red',
         ))
         steamguard_advanced.grid.attach(warning_label, 0, 0, 2, 1)
 
         shared_secret = steamguard_advanced.new_item('shared_secret', _("Shared Secret:"), Gtk.Entry, 0, 1)
         shared_secret.connect('changed', utils.on_setting_changed)
 
-        token_item = steamguard_advanced.new_item("token", _("Token:"), Gtk.Entry, 0, 2)
-        token_item.connect("changed", utils.on_setting_changed)
+        access_token_item = steamguard_advanced.new_item("access_token", _("Access Token:"), Gtk.Entry, 0, 2)
+        access_token_item.connect("changed", utils.on_setting_changed)
 
-        token_secure_item = steamguard_advanced.new_item("token_secure", _("Token Secure:"), Gtk.Entry, 0, 3)
-        token_secure_item.connect("changed", utils.on_setting_changed)
+        refresh_token_item = steamguard_advanced.new_item("refresh_token", _("Refresh Token:"), Gtk.Entry, 0, 3)
+        refresh_token_item.connect("changed", utils.on_setting_changed)
 
         identity_secret = steamguard_advanced.new_item('identity_secret', _("Identity Secret:"), Gtk.Entry, 0, 4)
         identity_secret.connect('changed', utils.on_setting_changed)
 
         deviceid = steamguard_advanced.new_item('deviceid', _("Device ID:"), Gtk.Entry, 0, 5)
         deviceid.connect('changed', utils.on_setting_changed)
 
         steamid_item = steamguard_advanced.new_item("steamid", _("Steam ID:"), Gtk.Entry, 0, 6)
         steamid_item.set_input_purpose(Gtk.InputPurpose.DIGITS)
         steamid_item.connect("changed", utils.on_digit_only_setting_changed)
 
         account_name = steamguard_advanced.new_item('account_name', _("Username:"), Gtk.Entry, 0, 7)
         account_name.connect('changed', utils.on_setting_changed)
 
-        reset_button = utils.AsyncButton()
+        reset_button = Gtk.Button()
         reset_button.set_label(_("Reset Everything (USE WITH CAUTION!!!)"))
         reset_button.set_name("reset_button")
         reset_button.connect("clicked", self.on_reset_clicked)
         steamguard_advanced.grid.attach(reset_button, 0, 8, 2, 1)
 
         cardfarming_section.grid.attach(self.cardfarming_status, 0, 0, 2, 1)
 
@@ -353,15 +363,14 @@
                 "a stlib built without SteamWorks support. To enable it again,\n"
                 "reinstall stlib with SteamWorks support\n"
             )
 
             _cardfarming_disabled.set_markup(utils.markup(_message, color="hotpink", background="black"))
             cardfarming_section.attach(_cardfarming_disabled, 0, 0, 2, 1)
 
-        # TODO: Maintain plugin switch?
         steamgifts_section.grid.attach(self.steamgifts_status, 0, 0, 2, 1)
 
         steamgifts_stack = Gtk.Stack()
         steamgifts_stack.set_vexpand(True)
         steamgifts_section.grid.attach(steamgifts_stack, 1, 1, 1, 1)
 
         steamgifts_sidebar = Gtk.StackSidebar()
@@ -382,19 +391,19 @@
             0, 1,
         )
         developer_giveaways.set_halign(Gtk.Align.END)
         developer_giveaways.connect("state-set", utils.on_setting_state_set)
 
         steamgifts_mode = steamgifts_settings.new_item(
             "mode", _("Mode:"),
-            Gtk.ComboBoxText,
+            Gtk.DropDown,
             0, 2,
             items=config.steamgifts_modes,
         )
-        steamgifts_mode.connect("changed", utils.on_combo_setting_changed, config.steamgifts_modes)
+        steamgifts_mode.connect("notify::selected", utils.on_dropdown_setting_changed, config.steamgifts_modes)
 
         wait_after_each_strategy = steamgifts_settings.new_item(
             "wait_after_each_strategy", _("Wait after each strategy:"),
             Gtk.Entry,
             0, 3,
         )
         wait_after_each_strategy.connect("changed", utils.on_digit_only_setting_changed)
@@ -439,28 +448,28 @@
 
                 maximum = strategy_section.new_item(f"maximum_{item}", None, Gtk.Entry, 2, tree_level + 2)
                 maximum.connect("changed", utils.on_digit_only_setting_changed)
 
             restrict_type = strategy_section.new_item(
                 "restrict_type",
                 _("Restrict Type:"),
-                Gtk.ComboBoxText,
+                Gtk.DropDown,
                 0, 7,
                 items=config.giveaway_types,
             )
-            restrict_type.connect("changed", utils.on_combo_setting_changed, config.giveaway_types)
+            restrict_type.connect("notify::selected", utils.on_dropdown_setting_changed, config.giveaway_types)
 
             sort_type = strategy_section.new_item(
                 "sort_type",
                 _("Sort Type:"),
-                Gtk.ComboBoxText,
+                Gtk.DropDown,
                 0, 8,
                 items=config.giveaway_sort_types,
             )
-            sort_type.connect("changed", utils.on_combo_setting_changed, config.giveaway_sort_types)
+            sort_type.connect("notify::selected", utils.on_dropdown_setting_changed, config.giveaway_sort_types)
 
             # setattr(self, f"steamgifts_strategy{index}", strategy_section)
 
         if not plugins.has_plugin("steamgifts"):
             steamgifts_section.set_sensitive(False)
             steamgifts_enable.set_active(False)
             _steamgifts_disabled = Gtk.Label()
@@ -537,32 +546,40 @@
         coupons_sidebar.set_size_request(150, -1)
         coupons_section.grid.attach(coupons_sidebar, 0, 1, 1, 1)
 
         self.coupons_grid = Gtk.Grid()
         self.coupons_grid.set_row_spacing(10)
         coupons_stack.add_titled(self.coupons_grid, "coupons_list", _("Coupon List"))
 
-        self.coupons_tree = utils.SimpleTextTree(
-            _('price'), _('name'), 'link', 'botid', 'token', 'assetid',
-            overlay_scrolling=False,
-            model=Gtk.ListStore,
-        )
+        coupons_tree_headers = '_price', '_name', 'link', 'botid', 'token', 'assetid'
+        self.coupons_tree = utils.SimpleTextTree(*coupons_tree_headers)
+
+        price_sorter = Gtk.CustomSorter()
+        price_sorter.set_sort_func(self.coupon_sorting)
+
+        price_column = self.coupons_tree.view.get_columns()[1]
+        price_column.set_sorter(price_sorter)
 
-        self.coupons_tree.store.set_sort_column_id(0, Gtk.SortType.ASCENDING)
-        self.coupons_tree.store.set_sort_func(0, self.coupon_sorting)
+        self.coupons_tree.view.sort_by_column(price_column, Gtk.SortType.ASCENDING)
         self.coupons_grid.attach(self.coupons_tree, 0, 0, 4, 2)
 
         for index, column in enumerate(self.coupons_tree.view.get_columns()):
-            if index in (2, 3, 4, 5):
+            column.set_resizable(True)
+
+            if index in (0, 3, 4, 5, 6):
                 column.set_visible(False)
 
-        self.coupons_tree.view.connect('row-activated', self.on_coupon_double_clicked)
+            if index == 1:
+                column.set_fixed_width(80)
+
+            if index == 2:
+                column.set_fixed_width(400)
 
-        coupon_tree_selection = self.coupons_tree.view.get_selection()
-        coupon_tree_selection.connect("changed", self.on_tree_selection_changed)
+        self.coupons_tree.view.connect("activate", self.on_coupon_double_clicked)
+        self.coupons_tree.model.connect("selection-changed", self.on_tree_selection_changed)
 
         self.coupon_progress = Gtk.LevelBar()
         self.coupons_grid.attach(self.coupon_progress, 0, 3, 4, 1)
 
         fetch_coupons_button = Gtk.Button()
         fetch_coupons_button.set_margin_start(3)
         fetch_coupons_button.set_margin_end(3)
@@ -579,22 +596,22 @@
         stop_fetching_coupons_button.connect('clicked', self.on_stop_fetching_coupons)
         self.coupons_grid.attach(stop_fetching_coupons_button, 1, 4, 1, 1)
 
         get_coupon_button = Gtk.Button()
         get_coupon_button.set_margin_start(3)
         get_coupon_button.set_margin_end(3)
         get_coupon_button.set_label(_('Get selected'))
-        get_coupon_button.connect('clicked', self.on_coupon_action, coupon_tree_selection)
+        get_coupon_button.connect('clicked', self.on_coupon_action, 'get')
         self.coupons_grid.attach(get_coupon_button, 2, 4, 1, 1)
 
         give_coupon_button = Gtk.Button()
         give_coupon_button.set_margin_start(3)
         give_coupon_button.set_margin_end(3)
         give_coupon_button.set_label(_('Send'))
-        give_coupon_button.connect('clicked', self.on_coupon_action)
+        give_coupon_button.connect('clicked', self.on_coupon_action, 'give')
         self.coupons_grid.attach(give_coupon_button, 3, 4, 1, 1)
 
         coupons_settings = utils.Section("coupons")
         coupons_settings.stackup_section(_("Settings"), coupons_stack)
 
         coupon_botids = coupons_settings.new_item("botids", _("BotIDs:"), Gtk.Entry, 0, 1)
         coupon_botids.set_placeholder_text('12345, asdfg, ...')
@@ -612,19 +629,19 @@
 
         coupon_blacklist = coupons_settings.new_item("blacklist", _("Blacklist:"), Gtk.Entry, 0, 5)
         coupon_blacklist.connect("changed", utils.on_setting_changed)
 
         coupon_discount = coupons_settings.new_item(
             "minimum_discount",
             _("Minimum Discount:"),
-            Gtk.ComboBoxText,
+            Gtk.DropDown,
             0, 6,
             items=config.coupon_discounts,
         )
-        coupon_discount.connect("changed", utils.on_combo_setting_changed, config.coupon_discounts)
+        coupon_discount.connect("notify::selected", utils.on_dropdown_setting_changed, config.coupon_discounts)
 
         self.statusbar = utils.StatusBar()
         main_grid.attach(self.statusbar, 1, 3, 1, 1)
 
         self.connect("destroy", self.application.on_exit_activate)
         self.connect("close-request", self.application.on_exit_activate)
 
@@ -640,27 +657,20 @@
     def theme(self) -> str:
         return config.parser.get('general', 'theme')
 
     async def user_info(self) -> None:
         while self.get_realized():
             account_name = config.parser.get('login', 'account_name')
             steamid_raw = config.parser.get('login', 'steamid')
-
-            try:
-                steamid = universe.generate_steamid(steamid_raw)
-            except ValueError:
-                log.warning(_("SteamId is invalid"))
-                steamid = None
-
             login_session = None
 
             with contextlib.suppress(IndexError):
                 login_session = login.Login.get_session(0)
 
-            if not steamid or not login_session or not await login_session.is_logged_in(steamid):
+            if not login_session or not await login_session.is_logged_in():
                 self.application.main_window.user_info_label.set_markup(
                     utils.markup(
                         _('Not logged in'),
                         color='darkred' if self.theme == 'light' else 'red',
                         size='small',
                     )
                 )
@@ -682,14 +692,31 @@
                 utils.markup(
                     f" {self.application.steamid.id3_string}",
                     color='grey',
                     size='small',
                 )
             )
 
+            if config.parser.get("login", "shared_secret"):
+                self.steamguard_disabled.set_visible(False)
+                self.steamguard_status.set_sensitive(True)
+            else:
+                self.steamguard_disabled.set_visible(True)
+                self.steamguard_status.set_sensitive(False)
+                self.steamguard_enable.set_active(False)
+
+            if config.parser.get("login", "identity_secret"):
+                self.confirmations_disabled.set_visible(False)
+                self.confirmations_grid.set_sensitive(True)
+            else:
+                self.confirmations_disabled.set_visible(True)
+                self.confirmations_grid.set_sensitive(False)
+                self.confirmations_enable.set_active(False)
+
+            self.on_stack_child_changed(self.main_tabs)
             await asyncio.sleep(30)
 
     async def plugin_status(self) -> None:
         while self.get_realized():
             for plugin_name in config.plugins.keys():
                 if plugin_name in ["coupons", "confirmations"]:
                     if plugin_name == "confirmations":
@@ -715,116 +742,69 @@
                             status_.set_status(_("Disabled"))
                             status_.set_info("")
 
                         self.loop.call_later(3, disabled_callback, status)
 
             await asyncio.sleep(3)
 
-    @staticmethod
-    def on_query_confirmations_tooltip(
-            tree_view: Gtk.TreeView,
-            x_coord: int,
-            y_coord: int,
-            keyboard_tip: bool,
-            tooltip: Gtk.Tooltip,
-    ) -> bool:
-        context = tree_view.get_tooltip_context(x_coord, y_coord, keyboard_tip)
-
-        if context[0]:
-            if context.model.iter_depth(context.iter) != 0:
-                return False
-
-            tooltip.set_text(
-                f'ConfID:{context.model.get_value(context.iter, 0)}\n'
-                f'CreatorID{context.model.get_value(context.iter, 1)}\n'
-                f'Key:{context.model.get_value(context.iter, 2)}'
-            )
-
-            return True
-
-        return False
-
     def on_fetch_coupons(self, button: Gtk.Button) -> None:
         self.fetch_coupon_event.set()
 
     def on_stop_fetching_coupons(self, button: Gtk.Button) -> None:
         self.fetch_coupon_event.clear()
         self.coupon_progress.set_value(0)
         self.coupon_progress.set_max_value(0)
 
-    def on_coupon_action(self, button: Gtk.Button, model: Union[Gtk.TreeModel, Gtk.TreeSelection] = None) -> None:
-        if model:
-            coupon_dialog = coupon.CouponDialog(self, self.application, *model.get_selected())
-        else:
-            coupon_dialog = coupon.CouponDialog(self, self.application)
-
-        coupon_dialog.show()
-
-    def on_validate_confirmations(
-            self,
-            button: Gtk.Button,
-            action: str,
-            model: Union[Gtk.TreeModel, Gtk.TreeSelection]) -> None:
-        if isinstance(model, Gtk.TreeModel):
-            finalize_dialog = confirmation.FinalizeDialog(
-                self,
-                self.application,
-                action,
-                model,
-                False
-            )
-        else:
-            finalize_dialog = confirmation.FinalizeDialog(
-                self,
-                self.application,
-                action,
-                *model.get_selected()
-            )
-
-        finalize_dialog.show()
-
-    @staticmethod
-    def on_coupon_double_clicked(view: Gtk.TreeView, path: Gtk.TreePath, column: Gtk.TreeViewColumn) -> None:
-        model = view.get_model()
-        url = model[path][2]
+    def on_coupon_action(self, button: Gtk.Button, action: str) -> None:
+        coupon_window = coupon.CouponWindow(self, self.application, self.coupons_tree, action)
+        coupon_window.present()
+
+    def on_validate_confirmations(self, button: Gtk.Button, action: str, batch: bool = False) -> None:
+        finalize_window = confirmation.FinalizeWindow(self, self.application, self.confirmations_tree, action, batch)
+        finalize_window.present()
+
+    def on_coupon_double_clicked(self, view: Gtk.ColumnView, position: int) -> None:
+        row = self.coupons_tree.model.get_item(position)
+        item = row.get_item()
+        url = f"steam://openurl/{item.link}"
         steam_running = False
 
         if stlib.steamworks_available:
             with contextlib.suppress(ProcessLookupError):
                 with client.SteamGameServer() as server:
                     steam_running = True
 
-        if steam_running:
-            url = f"steam://openurl/{url}"
+        if not steam_running:
+            url = item.link
 
         call(f'{config.file_manager} "{url}"')
 
     @staticmethod
-    def on_tree_selection_changed(selection: Gtk.TreeSelection) -> None:
-        model, iter_ = selection.get_selected()
+    def on_tree_selection_changed(view: Gtk.SingleSelection, position, item_count: int) -> None:
+        item = view.get_selected_item()
+        if parent := item.get_parent():
+            view.set_selected(parent.get_position())
 
-        if iter_:
-            parent = model.iter_parent(iter_)
+    @staticmethod
+    def on_stack_child_changed(stack: Gtk.Stack, *args) -> None:
+        section = stack.get_visible_child()
+
+        for item in section.items:
+            if item.get_name().startswith('_'):
+                continue
 
-            if parent:
-                selection.select_iter(parent)
+            log.debug(f'Reading {section.get_name()}:{item.get_name()} from config file')
+            item.update_values()
 
     @staticmethod
-    def coupon_sorting(model: Gtk.TreeModel, iter1: Gtk.TreeIter, iter2: Gtk.TreeIter, user_data: Any) -> Any:
-        column, _ = model.get_sort_column_id()
-        price1 = model.get_value(iter1, column)
-        price2 = model.get_value(iter2, column)
-
-        if float(price1) < float(price2):
+    def coupon_sorting(item1: utils.SimpleTextTreeItem, item2: utils.SimpleTextTreeItem, *data: Any) -> Any:
+        if float(item1.price) < float(item2.price):
             return -1
 
-        if price1 == price2:
-            return 0
-
-        return 1
+        return 0 if item1.price == item2.price else 1
 
     def set_status(
             self,
             module: str,
             module_data: Optional[core.utils.ModuleData] = None,
             *,
             display: str = '',
@@ -869,48 +849,63 @@
             _status.set_level(*module_data.level)
 
     def get_play_event(self, module: str) -> asyncio.Event:
         _status = getattr(self, f'{module}_status')
         assert isinstance(_status, utils.Status)
         return _status.play_event
 
-    async def on_reset_clicked(self, button: Gtk.Button) -> None:
-        login_dialog = LoginDialog(self, self.application)
-        login_dialog.status.info(_("Reseting... Please wait!"))
-        login_dialog.set_deletable(False)
-        login_dialog.user_details_section.hide()
-        login_dialog.advanced_login.hide()
-        login_dialog.show()
-        await asyncio.sleep(3)
+    def on_login_button_clicked(self, button: Gtk.Button) -> None:
+        login_window = LoginWindow(self, self.application)
+        login_window.shared_secret_item.set_text('')
+        login_window.identity_secret_item.set_text('')
+        login_window.present()
+
+    def on_new_authenticator_clicked(self, button: Gtk.Button) -> None:
+        authenticator_window = authenticator.AuthenticatorWindow(self, self.application)
+        authenticator_window.present()
+
+        self.loop.create_task(authenticator_window.on_add_authenticator())
+
+    def on_remove_authenticator_clicked(self, button: Gtk.Button) -> None:
+        authenticator_window = authenticator.AuthenticatorWindow(self, self.application)
+        authenticator_window.present()
+
+        self.loop.create_task(authenticator_window.on_remove_authenticator())
+
+    def on_reset_clicked(self, button: Gtk.Button) -> None:
+        login_window = LoginWindow(self, self.application)
+        login_window.status.info(_("Reseting... Please wait!"))
+        login_window.set_deletable(False)
+        login_window.user_details_section.set_visible(False)
+        login_window.advanced_login.set_visible(False)
+        login_window.present()
 
         config.config_file.unlink(missing_ok=True)
 
         config.parser.clear()
         config.init()
-        self.destroy()
 
-    def on_login_button_clicked(self, button: Gtk.Button) -> None:
-        login_dialog = LoginDialog(self, self.application)
-        login_dialog.shared_secret_item.set_text('')
-        login_dialog.identity_secret_item.set_text('')
-        login_dialog.show()
+        def reset_callback() -> None:
+            login_window.destroy()
+            self.destroy()
 
-    def on_new_authenticator_clicked(self, button: Gtk.Button) -> None:
-        new_authenticator_dialog = NewAuthenticatorDialog(self, self.application)
-        new_authenticator_dialog.show()
+        login_window.status.info(_("Successful!\nExiting..."))
+        self.loop.call_later(3, reset_callback)
 
     def on_reset_password_clicked(self, button: Gtk.Button) -> None:
-        login_dialog = LoginDialog(self, self.application)
-        login_dialog.status.info(_("Removing saved password..."))
-        login_dialog.user_details_section.hide()
-        login_dialog.advanced_login.hide()
-        login_dialog.set_deletable(False)
-        login_dialog.show()
+        reseting_window = utils.PopupWindowBase(self, self.application)
+
+        reseting_status = utils.SimpleStatus()
+        reseting_status.info(_("Removing saved password..."))
+
+        reseting_window.content_grid.attach(reseting_status, 0, 0, 1, 1)
+        reseting_window.set_deletable(False)
+        reseting_window.present()
 
         config.new("login", "password", "")
 
         def reset_password_callback() -> None:
-            login_dialog.destroy()
+            reseting_window.destroy()
             self.destroy()
 
-        login_dialog.status.info(_("Successful!\nExiting..."))
+        reseting_status.info(_("Successful!\nExiting..."))
         self.loop.call_later(3, reset_password_callback)
```

### Comparing `steam-tools-ng-3.0.1/src/steam_tools_ng/gui.py` & `steam-tools-ng-3.1/src/steam_tools_ng/gui.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 # See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see http://www.gnu.org/licenses/.
 #
-
+import asyncio
 import os
 import sys
 
 # FIXME: Temporary workaround for cx_freeze
 #  not running from Win32GUI correctly
 if os.name == 'nt' and hasattr(sys, 'frozen'):
     import ctypes
@@ -34,25 +34,26 @@
 import configparser
 import logging
 from pathlib import Path
 from subprocess import call
 from typing import Optional, Any
 
 from steam_tools_ng import config, i18n
-from steam_tools_ng.gtk import application
+from steam_tools_ng.gtk import application, about
 from steam_tools_ng.gtk import async_gtk, utils
+from gi.repository import Gtk
 
 _ = i18n.get_translation
 log = logging.getLogger(__name__)
 
 
 class GraphicalArgParser(argparse.ArgumentParser):
     def _print_message(self, message: str, file: Optional[Any] = None) -> None:
         if message:
-            utils.fatal_error_dialog(Exception(message), [])
+            utils.fatal_error_dialog(type('Info', (Exception,), {})(message))
 
 
 def main() -> None:
     freeze_support()
     try:
         config.init()
     except configparser.Error as exception:
@@ -85,16 +86,34 @@
     command_parser.add_argument(
         '--reset-password',
         action='store_true',
         help='Clean up saved password',
         dest='reset_password',
     )
 
+    command_parser.add_argument(
+        '-v', '--version',
+        action='store_true',
+        help='Show version',
+        dest='version',
+    )
+
     console_params = command_parser.parse_args()
 
+    if console_params.version:
+        about_dialog = about.AboutDialog(parent_window=None)
+        about_dialog.present()
+        about_dialog.connect("close-request", lambda *args: asyncio.get_event_loop().stop())
+        about_dialog.connect("destroy", lambda *args: asyncio.get_event_loop().stop())
+
+        if not Gtk.Application.get_default():
+            async_gtk.run()
+
+        sys.exit(0)
+
     if console_params.config_dir:
         call(f'{config.file_manager} {config.config_file_directory}')
         sys.exit(0)
 
     if console_params.log_dir:
         call(f'{config.file_manager} {config.parser.get("logger", "log_directory")}')
         sys.exit(0)
```

### Comparing `steam-tools-ng-3.0.1/src/steam_tools_ng/i18n.py` & `steam-tools-ng-3.1/src/steam_tools_ng/i18n.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,40 +12,28 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 # See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see http://www.gnu.org/licenses/.
 #
 
-from importlib import resources
-
 # Never use VHL methods in this file to avoid infinite recursion:
 # [method>get_translation->vhlm->get_translation->vhlm] IT'S NOT A BUG!
 import configparser
 import gettext
-import hashlib
-from typing import Dict
+from importlib import resources
 
 from . import config
 
-cache: Dict[bytes, str] = {}
-
-
-def new_hash(text: str) -> bytes:
-    sums = hashlib.sha256(text.encode())
-
-    return sums.digest()
-
 
 def get_translation(text: str) -> str:
     try:
         language = config.parser.get('general', 'language')
     except configparser.NoSectionError:
         # assume that config is not fully loaded yet
         return text
 
     with resources.as_file(resources.files('steam_tools_ng')) as path:
         translation = gettext.translation("steam-tools-ng", path / 'locale', languages=[language], fallback=True)
         translated_text = translation.gettext(text)
-        cache[new_hash(translated_text)] = text
 
     return translated_text
```

### Comparing `steam-tools-ng-3.0.1/src/steam_tools_ng/icons/stng.ico` & `steam-tools-ng-3.1/src/steam_tools_ng/icons/stng.ico`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.0.1/src/steam_tools_ng/icons/stng.png` & `steam-tools-ng-3.1/src/steam_tools_ng/icons/stng.png`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.0.1/src/steam_tools_ng/icons/stng_console.ico` & `steam-tools-ng-3.1/src/steam_tools_ng/icons/stng_console.ico`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.0.1/src/steam_tools_ng/icons/stng_console.png` & `steam-tools-ng-3.1/src/steam_tools_ng/icons/stng_console.png`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.0.1/src/steam_tools_ng/icons/stng_nc.ico` & `steam-tools-ng-3.1/src/steam_tools_ng/icons/stng_nc.ico`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.0.1/src/steam_tools_ng/icons/stng_nc.png` & `steam-tools-ng-3.1/src/steam_tools_ng/icons/stng_nc.png`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.0.1/src/steam_tools_ng/logger_handlers.py` & `steam-tools-ng-3.1/src/steam_tools_ng/logger_handlers.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.0.1/src/steam_tools_ng.egg-info/PKG-INFO` & `steam-tools-ng-3.1/src/steam_tools_ng.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: steam-tools-ng
-Version: 3.0.1
+Version: 3.1
 Summary: Steam Tools NG
 Author: Lara Maia
 Author-email: dev@lara.monster
 License: GPLv3
 Project-URL: homepage, https://github.com/calendulish/steam-tools-ng
 Project-URL: repository, https://github.com
 Project-URL: changelog, https://github.com/calendulish/steam-tools-ng/releases
 Keywords: steam,valve
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Games/Entertainment
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Environment :: X11 Applications :: GTK
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [STNG] Steam Tools NG (formerly Steam Tools)
 ========================================
```

### Comparing `steam-tools-ng-3.0.1/src/steam_tools_ng.egg-info/SOURCES.txt` & `steam-tools-ng-3.1/src/steam_tools_ng.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 src/steam_tools_ng/__main__.py
 src/steam_tools_ng/cli.py
 src/steam_tools_ng/config.py
 src/steam_tools_ng/gui.py
 src/steam_tools_ng/i18n.py
 src/steam_tools_ng/logger_handlers.py
 src/steam_tools_ng/py.typed
-src/steam_tools_ng/steam_api_executor.py
 src/steam_tools_ng.egg-info/PKG-INFO
 src/steam_tools_ng.egg-info/SOURCES.txt
 src/steam_tools_ng.egg-info/dependency_links.txt
 src/steam_tools_ng.egg-info/entry_points.txt
+src/steam_tools_ng.egg-info/not-zip-safe
 src/steam_tools_ng.egg-info/requires.txt
 src/steam_tools_ng.egg-info/top_level.txt
 src/steam_tools_ng/console/__init__.py
 src/steam_tools_ng/console/authenticator.py
 src/steam_tools_ng/console/cli.py
 src/steam_tools_ng/console/login.py
 src/steam_tools_ng/console/utils.py
```

