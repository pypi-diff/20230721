# Comparing `tmp/crypto_licensing-3.0.4.tar.gz` & `tmp/crypto_licensing-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto_licensing-3.0.4.tar", last modified: Sun Feb  5 15:28:10 2023, max compression
+gzip compressed data, was "crypto_licensing-3.3.0.tar", last modified: Tue Feb 21 16:53:47 2023, max compression
```

## Comparing `crypto_licensing-3.0.4.tar` & `crypto_licensing-3.3.0.tar`

### file list

```diff
@@ -1,100 +1,49 @@
-drwxrwxr-x   0 perry      (501) staff       (20)        0 2023-02-05 15:28:10.614963 crypto_licensing-3.0.4/
--rw-rw-r--   0 perry      (501) staff       (20)    35147 2022-01-25 19:29:48.000000 crypto_licensing-3.0.4/COPYING
--rw-rw-r--   0 perry      (501) staff       (20)     1184 2023-02-05 15:25:14.000000 crypto_licensing-3.0.4/LICENSE
--rw-rw-r--   0 perry      (501) staff       (20)      138 2022-02-23 17:37:17.000000 crypto_licensing-3.0.4/MANIFEST.in
--rw-rw-r--   0 perry      (501) staff       (20)     1392 2023-02-05 15:28:10.614517 crypto_licensing-3.0.4/PKG-INFO
--rw-rw-r--   0 perry      (501) staff       (20)     4468 2023-02-05 15:25:14.000000 crypto_licensing-3.0.4/README.org
--rw-rw-r--   0 perry      (501) staff       (20)     7177 2023-02-05 15:25:14.000000 crypto_licensing-3.0.4/README.txt
-drwxrwxr-x   0 perry      (501) staff       (20)        0 2023-02-05 15:28:10.551943 crypto_licensing-3.0.4/crypto_licensing/
--rw-rw-r--   0 perry      (501) staff       (20)     1280 2023-02-05 15:25:14.000000 crypto_licensing-3.0.4/crypto_licensing/__init__.py
--rw-rw-r--   0 perry      (501) staff       (20)     9560 2023-02-05 15:25:14.000000 crypto_licensing-3.0.4/crypto_licensing/__main__.py
--rw-rw-r--   0 perry      (501) staff       (20)     5264 2023-02-05 15:25:14.000000 crypto_licensing-3.0.4/crypto_licensing/crypto_test.py
-drwxrwxr-x   0 perry      (501) staff       (20)        0 2023-02-05 15:28:10.552445 crypto_licensing-3.0.4/crypto_licensing/ed25519/
--rw-rw-r--   0 perry      (501) staff       (20)     1570 2023-02-05 15:25:14.000000 crypto_licensing-3.0.4/crypto_licensing/ed25519/__init__.py
--rw-rw-r--   0 perry      (501) staff       (20)     5033 2022-01-24 17:18:08.000000 crypto_licensing-3.0.4/crypto_licensing/ed25519_djb.py
-drwxrwxr-x   0 perry      (501) staff       (20)        0 2023-02-05 15:28:10.553428 crypto_licensing-3.0.4/crypto_licensing/ed25519ll_pyonly/
--rw-rw-r--   0 perry      (501) staff       (20)     2319 2023-02-05 15:25:14.000000 crypto_licensing-3.0.4/crypto_licensing/ed25519ll_pyonly/__init__.py
--rw-rw-r--   0 perry      (501) staff       (20)     6905 2022-01-19 19:14:43.000000 crypto_licensing-3.0.4/crypto_licensing/ed25519ll_pyonly/djbec.py
-drwxrwxr-x   0 perry      (501) staff       (20)        0 2023-02-05 15:28:10.574404 crypto_licensing-3.0.4/crypto_licensing/licensing/
--rw-rw-r--   0 perry      (501) staff       (20)     1494 2023-02-05 15:25:14.000000 crypto_licensing-3.0.4/crypto_licensing/licensing/__init__.py
--rw-rw-r--   0 perry      (501) staff       (20)     1090 2023-02-05 15:25:14.000000 crypto_licensing-3.0.4/crypto_licensing/licensing/__main__.py
--rw-rw-r--   0 perry      (501) staff       (20)     1942 2023-02-05 15:25:14.000000 crypto_licensing-3.0.4/crypto_licensing/licensing/bitquery_test.py
--rw-rw-r--   0 perry      (501) staff       (20)     2109 2023-02-05 15:25:14.000000 crypto_licensing-3.0.4/crypto_licensing/licensing/defaults.py
-drwxrwxr-x   0 perry      (501) staff       (20)        0 2023-02-05 15:28:10.575527 crypto_licensing-3.0.4/crypto_licensing/licensing/doh/
--rw-rw-r--   0 perry      (501) staff       (20)     4426 2023-02-05 15:25:14.000000 crypto_licensing-3.0.4/crypto_licensing/licensing/doh/__init__.py
--rw-rw-r--   0 perry      (501) staff       (20)     2737 2023-02-05 15:25:14.000000 crypto_licensing-3.0.4/crypto_licensing/licensing/doh/__main__.py
--rw-rw-r--   0 perry      (501) staff       (20)     3035 2023-02-05 15:25:14.000000 crypto_licensing-3.0.4/crypto_licensing/licensing/doh_test.py
--rw-rw-r--   0 perry      (501) staff       (20)    17971 2023-02-05 15:25:14.000000 crypto_licensing-3.0.4/crypto_licensing/licensing/grant_test.py
--rw-rw-r--   0 perry      (501) staff       (20)      418 2022-01-19 19:14:43.000000 crypto_licensing-3.0.4/crypto_licensing/licensing/licensing.sql
--rw-rw-r--   0 perry      (501) staff       (20)      454 2022-01-19 19:14:43.000000 crypto_licensing-3.0.4/crypto_licensing/licensing/licensing.sql.authors
--rw-rw-r--   0 perry      (501) staff       (20)     1950 2023-02-05 15:25:14.000000 crypto_licensing-3.0.4/crypto_licensing/licensing/licensing.sql.coins
--rw-rw-r--   0 perry      (501) staff       (20)      301 2022-01-19 19:14:43.000000 crypto_licensing-3.0.4/crypto_licensing/licensing/licensing.sql.licenses
--rw-rw-r--   0 perry      (501) staff       (20)      235 2022-01-19 19:14:43.000000 crypto_licensing-3.0.4/crypto_licensing/licensing/licensing.sql.statics
--rw-rw-r--   0 perry      (501) staff       (20)      402 2022-01-19 19:14:43.000000 crypto_licensing-3.0.4/crypto_licensing/licensing/licensing.sql.users
-drwxrwxr-x   0 perry      (501) staff       (20)        0 2023-02-05 15:28:10.580117 crypto_licensing-3.0.4/crypto_licensing/licensing/licensing_test/
--rw-rw-r--   0 perry      (501) staff       (20)      158 2023-02-05 15:25:14.000000 crypto_licensing-3.0.4/crypto_licensing/licensing/licensing_test/crypto-licensing-server.crypto-keypair-end-user
--rw-rw-r--   0 perry      (501) staff       (20)     2094 2023-02-05 15:25:14.000000 crypto_licensing-3.0.4/crypto_licensing/licensing/licensing_test/crypto-licensing-server.crypto-license
--rw-rw-r--   0 perry      (501) staff       (20)      153 2022-01-19 19:14:43.000000 crypto_licensing-3.0.4/crypto_licensing/licensing/licensing_test/licensing.cpppo-keypair-awesome-inc
--rw-rw-r--   0 perry      (501) staff       (20)       43 2022-01-19 19:14:43.000000 crypto_licensing-3.0.4/crypto_licensing/licensing/licensing_test/licensing.credentials-example
--rw-rw-r--   0 perry      (501) staff       (20)      464 2022-01-19 19:14:43.000000 crypto_licensing-3.0.4/crypto_licensing/licensing/licensing_test/licensing.sql.authors
--rw-rw-r--   0 perry      (501) staff       (20)     1317 2023-02-05 15:25:14.000000 crypto_licensing-3.0.4/crypto_licensing/licensing/licensing_test/licensing.sql.licenses
--rw-rw-r--   0 perry      (501) staff       (20)     7469 2023-02-05 15:25:14.000000 crypto_licensing-3.0.4/crypto_licensing/licensing/licensing_test.py
--rw-rw-r--   0 perry      (501) staff       (20)    95927 2023-02-05 15:25:14.000000 crypto_licensing-3.0.4/crypto_licensing/licensing/main.py
-drwxrwxr-x   0 perry      (501) staff       (20)        0 2023-02-05 15:28:10.583865 crypto_licensing-3.0.4/crypto_licensing/licensing/static/
-drwxrwxr-x   0 perry      (501) staff       (20)        0 2023-02-05 15:28:10.534646 crypto_licensing-3.0.4/crypto_licensing/licensing/static/bootstrap-3.3.1-dist/
-drwxrwxr-x   0 perry      (501) staff       (20)        0 2023-02-05 15:28:10.591580 crypto_licensing-3.0.4/crypto_licensing/licensing/static/bootstrap-3.3.1-dist/css/
--rw-rw-r--   0 perry      (501) staff       (20)    22474 2022-01-19 19:14:43.000000 crypto_licensing-3.0.4/crypto_licensing/licensing/static/bootstrap-3.3.1-dist/css/bootstrap-theme.css
--rw-rw-r--   0 perry      (501) staff       (20)    43029 2022-01-19 19:14:43.000000 crypto_licensing-3.0.4/crypto_licensing/licensing/static/bootstrap-3.3.1-dist/css/bootstrap-theme.css.map
--rw-rw-r--   0 perry      (501) staff       (20)    19835 2022-01-19 19:14:43.000000 crypto_licensing-3.0.4/crypto_licensing/licensing/static/bootstrap-3.3.1-dist/css/bootstrap-theme.min.css
--rw-rw-r--   0 perry      (501) staff       (20)   137067 2022-01-19 19:14:43.000000 crypto_licensing-3.0.4/crypto_licensing/licensing/static/bootstrap-3.3.1-dist/css/bootstrap.css
--rw-rw-r--   0 perry      (501) staff       (20)   366144 2022-01-19 19:14:43.000000 crypto_licensing-3.0.4/crypto_licensing/licensing/static/bootstrap-3.3.1-dist/css/bootstrap.css.map
--rw-rw-r--   0 perry      (501) staff       (20)   113498 2022-01-19 19:14:43.000000 crypto_licensing-3.0.4/crypto_licensing/licensing/static/bootstrap-3.3.1-dist/css/bootstrap.min.css
-drwxrwxr-x   0 perry      (501) staff       (20)        0 2023-02-05 15:28:10.593436 crypto_licensing-3.0.4/crypto_licensing/licensing/static/bootstrap-3.3.1-dist/fonts/
--rw-rw-r--   0 perry      (501) staff       (20)    20335 2022-01-19 19:14:43.000000 crypto_licensing-3.0.4/crypto_licensing/licensing/static/bootstrap-3.3.1-dist/fonts/glyphicons-halflings-regular.eot
--rw-rw-r--   0 perry      (501) staff       (20)    41280 2022-01-19 19:14:43.000000 crypto_licensing-3.0.4/crypto_licensing/licensing/static/bootstrap-3.3.1-dist/fonts/glyphicons-halflings-regular.ttf
--rw-rw-r--   0 perry      (501) staff       (20)    23320 2022-01-19 19:14:43.000000 crypto_licensing-3.0.4/crypto_licensing/licensing/static/bootstrap-3.3.1-dist/fonts/glyphicons-halflings-regular.woff
-drwxrwxr-x   0 perry      (501) staff       (20)        0 2023-02-05 15:28:10.602856 crypto_licensing-3.0.4/crypto_licensing/licensing/static/bootstrap-3.3.1-dist/js/
--rw-rw-r--   0 perry      (501) staff       (20)    67155 2022-01-19 19:14:43.000000 crypto_licensing-3.0.4/crypto_licensing/licensing/static/bootstrap-3.3.1-dist/js/bootstrap.js
--rw-rw-r--   0 perry      (501) staff       (20)    35601 2022-01-19 19:14:43.000000 crypto_licensing-3.0.4/crypto_licensing/licensing/static/bootstrap-3.3.1-dist/js/bootstrap.min.js
--rw-rw-r--   0 perry      (501) staff       (20)      484 2022-01-19 19:14:43.000000 crypto_licensing-3.0.4/crypto_licensing/licensing/static/bootstrap-3.3.1-dist/js/npm.js
-drwxrwxr-x   0 perry      (501) staff       (20)        0 2023-02-05 15:28:10.603806 crypto_licensing-3.0.4/crypto_licensing/licensing/static/css/
--rw-rw-r--   0 perry      (501) staff       (20)     7184 2022-01-19 19:14:43.000000 crypto_licensing-3.0.4/crypto_licensing/licensing/static/css/bootstrap-switch.css
--rw-rw-r--   0 perry      (501) staff       (20)      975 2022-01-19 19:14:43.000000 crypto_licensing-3.0.4/crypto_licensing/licensing/static/css/style.css
-drwxrwxr-x   0 perry      (501) staff       (20)        0 2023-02-05 15:28:10.606084 crypto_licensing-3.0.4/crypto_licensing/licensing/static/images/
--rw-rw-r--   0 perry      (501) staff       (20)   209557 2022-01-19 19:14:43.000000 crypto_licensing-3.0.4/crypto_licensing/licensing/static/images/55c649caa8e21dc6c4d75d08677fc6d0.ico.zip
--rw-rw-r--   0 perry      (501) staff       (20)    12653 2022-01-19 19:14:43.000000 crypto_licensing-3.0.4/crypto_licensing/licensing/static/images/apple-icon-180x180.png
--rw-rw-r--   0 perry      (501) staff       (20)     7604 2022-01-19 19:14:43.000000 crypto_licensing-3.0.4/crypto_licensing/licensing/static/images/favicon-96x96.png
--rw-rw-r--   0 perry      (501) staff       (20)     1150 2022-01-19 19:14:43.000000 crypto_licensing-3.0.4/crypto_licensing/licensing/static/images/favicon.ico
-drwxrwxr-x   0 perry      (501) staff       (20)        0 2023-02-05 15:28:10.607243 crypto_licensing-3.0.4/crypto_licensing/licensing/static/js/
--rw-rw-r--   0 perry      (501) staff       (20)    84320 2022-01-19 19:14:43.000000 crypto_licensing-3.0.4/crypto_licensing/licensing/static/js/jquery-2.1.3.min.js
--rw-rw-r--   0 perry      (501) staff       (20)     3761 2022-01-19 19:14:43.000000 crypto_licensing-3.0.4/crypto_licensing/licensing/static/js/yepnope.1.5.4-min.js
--rw-rw-r--   0 perry      (501) staff       (20)   730924 2022-03-16 17:52:55.000000 crypto_licensing-3.0.4/crypto_licensing/licensing/static/licensing.access
--rw-r--r--   0 perry      (501) staff       (20)    69632 2022-03-16 17:52:55.000000 crypto_licensing-3.0.4/crypto_licensing/licensing/static/licensing.db
-drwxrwxr-x   0 perry      (501) staff       (20)        0 2023-02-05 15:28:10.535523 crypto_licensing-3.0.4/crypto_licensing/licensing/static/resources/
-drwxrwxr-x   0 perry      (501) staff       (20)        0 2023-02-05 15:28:10.609555 crypto_licensing-3.0.4/crypto_licensing/licensing/static/resources/templates/
--rw-rw-r--   0 perry      (501) staff       (20)      239 2022-01-19 19:14:43.000000 crypto_licensing-3.0.4/crypto_licensing/licensing/static/resources/templates/index.html
--rw-rw-r--   0 perry      (501) staff       (20)     2892 2022-01-19 19:14:43.000000 crypto_licensing-3.0.4/crypto_licensing/licensing/static/resources/templates/keylist.html
--rw-rw-r--   0 perry      (501) staff       (20)     6272 2022-01-19 19:14:43.000000 crypto_licensing-3.0.4/crypto_licensing/licensing/static/resources/templates/layout.html
--rw-rw-r--   0 perry      (501) staff       (20)     4082 2022-01-19 19:14:43.000000 crypto_licensing-3.0.4/crypto_licensing/licensing/static/resources/templates/login.html
--rw-rw-r--   0 perry      (501) staff       (20)     7266 2022-01-19 19:14:43.000000 crypto_licensing-3.0.4/crypto_licensing/licensing/static/resources/templates/relay.html
-drwxrwxr-x   0 perry      (501) staff       (20)        0 2023-02-05 15:28:10.610521 crypto_licensing-3.0.4/crypto_licensing/licensing/static/txt/
--rw-rw-r--   0 perry      (501) staff       (20)      684 2023-02-05 15:25:14.000000 crypto_licensing-3.0.4/crypto_licensing/licensing/static/txt/CL-KEYPAIR-MISSING.org
--rw-rw-r--   0 perry      (501) staff       (20)      670 2023-02-05 15:25:14.000000 crypto_licensing-3.0.4/crypto_licensing/licensing/static/txt/CL-KEYPAIR-MISSING.txt
--rw-rw-r--   0 perry      (501) staff       (20)   140258 2023-02-05 15:25:14.000000 crypto_licensing-3.0.4/crypto_licensing/licensing/verification.py
--rw-rw-r--   0 perry      (501) staff       (20)    39633 2023-02-05 15:25:14.000000 crypto_licensing-3.0.4/crypto_licensing/licensing/verification_test.py
--rw-rw-r--   0 perry      (501) staff       (20)    40683 2023-02-05 15:25:17.000000 crypto_licensing-3.0.4/crypto_licensing/misc.py
--rw-rw-r--   0 perry      (501) staff       (20)     9528 2023-02-05 15:25:17.000000 crypto_licensing-3.0.4/crypto_licensing/misc_test.py
--rw-rw-r--   0 perry      (501) staff       (20)       88 2023-02-05 15:25:17.000000 crypto_licensing-3.0.4/crypto_licensing/version.py
-drwxrwxr-x   0 perry      (501) staff       (20)        0 2023-02-05 15:28:10.613788 crypto_licensing-3.0.4/crypto_licensing.egg-info/
--rw-rw-r--   0 perry      (501) staff       (20)     1392 2023-02-05 15:28:10.000000 crypto_licensing-3.0.4/crypto_licensing.egg-info/PKG-INFO
--rw-rw-r--   0 perry      (501) staff       (20)     4082 2023-02-05 15:28:10.000000 crypto_licensing-3.0.4/crypto_licensing.egg-info/SOURCES.txt
--rw-rw-r--   0 perry      (501) staff       (20)        1 2023-02-05 15:28:10.000000 crypto_licensing-3.0.4/crypto_licensing.egg-info/dependency_links.txt
--rw-rw-r--   0 perry      (501) staff       (20)       74 2023-02-05 15:28:10.000000 crypto_licensing-3.0.4/crypto_licensing.egg-info/entry_points.txt
--rw-rw-r--   0 perry      (501) staff       (20)        1 2023-02-05 15:28:10.000000 crypto_licensing-3.0.4/crypto_licensing.egg-info/not-zip-safe
--rw-rw-r--   0 perry      (501) staff       (20)      263 2023-02-05 15:28:10.000000 crypto_licensing-3.0.4/crypto_licensing.egg-info/requires.txt
--rw-rw-r--   0 perry      (501) staff       (20)      134 2023-02-05 15:28:10.000000 crypto_licensing-3.0.4/crypto_licensing.egg-info/top_level.txt
--rw-rw-r--   0 perry      (501) staff       (20)       48 2023-02-05 15:25:14.000000 crypto_licensing-3.0.4/requirements-dev.txt
--rw-rw-r--   0 perry      (501) staff       (20)       21 2023-02-05 15:25:14.000000 crypto_licensing-3.0.4/requirements-tests.txt
--rw-rw-r--   0 perry      (501) staff       (20)      312 2023-02-05 15:25:14.000000 crypto_licensing-3.0.4/requirements.txt
--rw-rw-r--   0 perry      (501) staff       (20)       38 2023-02-05 15:28:10.615099 crypto_licensing-3.0.4/setup.cfg
--rw-rw-r--   0 perry      (501) staff       (20)     4767 2023-02-05 15:25:14.000000 crypto_licensing-3.0.4/setup.py
+drwxrwxr-x   0 perry      (501) staff       (20)        0 2023-02-21 16:53:47.467643 crypto_licensing-3.3.0/
+-rw-rw-r--   0 perry      (501) staff       (20)    35147 2022-01-25 19:29:48.000000 crypto_licensing-3.3.0/COPYING
+-rw-rw-r--   0 perry      (501) staff       (20)     1184 2023-02-05 15:25:14.000000 crypto_licensing-3.3.0/LICENSE
+-rw-rw-r--   0 perry      (501) staff       (20)      138 2022-02-23 17:37:17.000000 crypto_licensing-3.3.0/MANIFEST.in
+-rw-rw-r--   0 perry      (501) staff       (20)     1392 2023-02-21 16:53:47.466894 crypto_licensing-3.3.0/PKG-INFO
+-rw-rw-r--   0 perry      (501) staff       (20)     4468 2023-02-05 15:25:14.000000 crypto_licensing-3.3.0/README.org
+-rw-rw-r--   0 perry      (501) staff       (20)     7177 2023-02-05 15:25:14.000000 crypto_licensing-3.3.0/README.txt
+drwxrwxr-x   0 perry      (501) staff       (20)        0 2023-02-21 16:53:47.440753 crypto_licensing-3.3.0/crypto_licensing/
+-rw-rw-r--   0 perry      (501) staff       (20)     1364 2023-02-14 14:06:11.000000 crypto_licensing-3.3.0/crypto_licensing/__init__.py
+-rw-rw-r--   0 perry      (501) staff       (20)     1365 2023-02-14 14:41:09.000000 crypto_licensing-3.3.0/crypto_licensing/__main__.py
+-rw-rw-r--   0 perry      (501) staff       (20)    10632 2023-02-16 18:04:11.000000 crypto_licensing-3.3.0/crypto_licensing/cli.py
+-rw-rw-r--   0 perry      (501) staff       (20)     3993 2023-02-15 19:50:25.000000 crypto_licensing-3.3.0/crypto_licensing/cli_test.py
+-rw-rw-r--   0 perry      (501) staff       (20)     5264 2023-02-05 15:25:14.000000 crypto_licensing-3.3.0/crypto_licensing/crypto_test.py
+drwxrwxr-x   0 perry      (501) staff       (20)        0 2023-02-21 16:53:47.441386 crypto_licensing-3.3.0/crypto_licensing/ed25519/
+-rw-rw-r--   0 perry      (501) staff       (20)     1655 2023-02-14 14:07:01.000000 crypto_licensing-3.3.0/crypto_licensing/ed25519/__init__.py
+-rw-rw-r--   0 perry      (501) staff       (20)     5033 2022-01-24 17:18:08.000000 crypto_licensing-3.3.0/crypto_licensing/ed25519_djb.py
+drwxrwxr-x   0 perry      (501) staff       (20)        0 2023-02-21 16:53:47.443278 crypto_licensing-3.3.0/crypto_licensing/ed25519ll_pyonly/
+-rw-rw-r--   0 perry      (501) staff       (20)     2319 2023-02-05 15:25:14.000000 crypto_licensing-3.3.0/crypto_licensing/ed25519ll_pyonly/__init__.py
+-rw-rw-r--   0 perry      (501) staff       (20)     6905 2022-01-19 19:14:43.000000 crypto_licensing-3.3.0/crypto_licensing/ed25519ll_pyonly/djbec.py
+drwxrwxr-x   0 perry      (501) staff       (20)        0 2023-02-21 16:53:47.453781 crypto_licensing-3.3.0/crypto_licensing/licensing/
+-rw-rw-r--   0 perry      (501) staff       (20)     1606 2023-02-21 15:58:27.000000 crypto_licensing-3.3.0/crypto_licensing/licensing/__init__.py
+-rw-rw-r--   0 perry      (501) staff       (20)     1196 2023-02-14 14:07:40.000000 crypto_licensing-3.3.0/crypto_licensing/licensing/__main__.py
+-rw-rw-r--   0 perry      (501) staff       (20)     1942 2023-02-05 15:25:14.000000 crypto_licensing-3.3.0/crypto_licensing/licensing/bitquery_test.py
+-rw-rw-r--   0 perry      (501) staff       (20)     2194 2023-02-14 14:08:13.000000 crypto_licensing-3.3.0/crypto_licensing/licensing/defaults.py
+drwxrwxr-x   0 perry      (501) staff       (20)        0 2023-02-21 16:53:47.459384 crypto_licensing-3.3.0/crypto_licensing/licensing/doh/
+-rw-rw-r--   0 perry      (501) staff       (20)     4511 2023-02-14 14:08:34.000000 crypto_licensing-3.3.0/crypto_licensing/licensing/doh/__init__.py
+-rw-rw-r--   0 perry      (501) staff       (20)     1362 2023-02-14 14:15:34.000000 crypto_licensing-3.3.0/crypto_licensing/licensing/doh/__main__.py
+-rw-rw-r--   0 perry      (501) staff       (20)     2731 2023-02-14 14:16:10.000000 crypto_licensing-3.3.0/crypto_licensing/licensing/doh/cli.py
+-rw-rw-r--   0 perry      (501) staff       (20)     3035 2023-02-05 15:25:14.000000 crypto_licensing-3.3.0/crypto_licensing/licensing/doh_test.py
+-rw-rw-r--   0 perry      (501) staff       (20)    17971 2023-02-05 15:25:14.000000 crypto_licensing-3.3.0/crypto_licensing/licensing/grant_test.py
+-rw-rw-r--   0 perry      (501) staff       (20)     7469 2023-02-05 15:25:14.000000 crypto_licensing-3.3.0/crypto_licensing/licensing/licensing_test.py
+-rw-rw-r--   0 perry      (501) staff       (20)    96445 2023-02-14 14:08:47.000000 crypto_licensing-3.3.0/crypto_licensing/licensing/main.py
+-rw-rw-r--   0 perry      (501) staff       (20)   143017 2023-02-21 16:50:37.000000 crypto_licensing-3.3.0/crypto_licensing/licensing/verification.py
+-rw-rw-r--   0 perry      (501) staff       (20)    40362 2023-02-21 15:30:21.000000 crypto_licensing-3.3.0/crypto_licensing/licensing/verification_test.py
+-rw-rw-r--   0 perry      (501) staff       (20)    43408 2023-02-17 20:51:56.000000 crypto_licensing-3.3.0/crypto_licensing/misc.py
+-rw-rw-r--   0 perry      (501) staff       (20)     9528 2023-02-05 15:25:17.000000 crypto_licensing-3.3.0/crypto_licensing/misc_test.py
+-rw-rw-r--   0 perry      (501) staff       (20)       88 2023-02-21 16:33:34.000000 crypto_licensing-3.3.0/crypto_licensing/version.py
+drwxrwxr-x   0 perry      (501) staff       (20)        0 2023-02-21 16:53:47.465934 crypto_licensing-3.3.0/crypto_licensing.egg-info/
+-rw-rw-r--   0 perry      (501) staff       (20)     1392 2023-02-21 16:53:47.000000 crypto_licensing-3.3.0/crypto_licensing.egg-info/PKG-INFO
+-rw-rw-r--   0 perry      (501) staff       (20)     1331 2023-02-21 16:53:47.000000 crypto_licensing-3.3.0/crypto_licensing.egg-info/SOURCES.txt
+-rw-rw-r--   0 perry      (501) staff       (20)        1 2023-02-21 16:53:47.000000 crypto_licensing-3.3.0/crypto_licensing.egg-info/dependency_links.txt
+-rw-rw-r--   0 perry      (501) staff       (20)       74 2023-02-21 16:53:47.000000 crypto_licensing-3.3.0/crypto_licensing.egg-info/entry_points.txt
+-rw-rw-r--   0 perry      (501) staff       (20)      263 2023-02-21 16:53:47.000000 crypto_licensing-3.3.0/crypto_licensing.egg-info/requires.txt
+-rw-rw-r--   0 perry      (501) staff       (20)      134 2023-02-21 16:53:47.000000 crypto_licensing-3.3.0/crypto_licensing.egg-info/top_level.txt
+-rw-rw-r--   0 perry      (501) staff       (20)       48 2023-02-05 15:25:14.000000 crypto_licensing-3.3.0/requirements-dev.txt
+-rw-rw-r--   0 perry      (501) staff       (20)       21 2023-02-05 15:25:14.000000 crypto_licensing-3.3.0/requirements-tests.txt
+-rw-rw-r--   0 perry      (501) staff       (20)      312 2023-02-05 15:25:14.000000 crypto_licensing-3.3.0/requirements.txt
+-rw-rw-r--   0 perry      (501) staff       (20)       38 2023-02-21 16:53:47.467853 crypto_licensing-3.3.0/setup.cfg
+-rw-rw-r--   0 perry      (501) staff       (20)     3157 2023-02-21 16:32:39.000000 crypto_licensing-3.3.0/setup.py
```

### Comparing `crypto_licensing-3.0.4/COPYING` & `crypto_licensing-3.3.0/COPYING`

 * *Files identical despite different names*

### Comparing `crypto_licensing-3.0.4/LICENSE` & `crypto_licensing-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `crypto_licensing-3.0.4/PKG-INFO` & `crypto_licensing-3.3.0/crypto_licensing.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: crypto_licensing
-Version: 3.0.4
+Name: crypto-licensing
+Version: 3.3.0
 Summary: The crypto-licensing module implements Ed25519-signed license checking and automatic issuance after cryptocurrency payment
 Home-page: https://github.com/pjkundert/crypto-licensing
 Author: Perry Kundert
 Author-email: perry@dominionrnd.com
 License: Dual License; GPLv3 and Proprietary
 Project-URL: Bug Tracker, https://github.com/pjkundert/crypto-licensing/issues
 Keywords: licensing Bitcoin Ethereum cryptocurrency payments Ed25519 signatures
```

### Comparing `crypto_licensing-3.0.4/README.org` & `crypto_licensing-3.3.0/README.org`

 * *Files identical despite different names*

### Comparing `crypto_licensing-3.0.4/README.txt` & `crypto_licensing-3.3.0/README.txt`

 * *Files identical despite different names*

### Comparing `crypto_licensing-3.0.4/crypto_licensing/__init__.py` & `crypto_licensing-3.3.0/crypto_licensing/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-
 #
 # Crypto-licensing -- Cryptographically signed licensing, w/ Cryptocurrency payments
 #
 # Copyright (c) 2022, Dominion Research & Development Corp.
 #
 # Crypto-licensing is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
-# later version.  See the LICENSE file at the top of the source tree.
+# later version.  It is also available under alternative (eg. Commercial)
+# licenses, at your option.  See the LICENSE file at the top of the source tree.
 #
 # It is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
 # A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
 #
 
 from __future__ import absolute_import, print_function, division
```

### Comparing `crypto_licensing-3.0.4/crypto_licensing/__main__.py` & `crypto_licensing-3.3.0/crypto_licensing/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,17 +18,16 @@
 from __future__ import absolute_import, print_function, division
 
 import click
 import codecs
 import json
 import logging
 import os
-import sys
 
-from .misc	import log_cfg, log_level
+from .misc	import log_cfg, log_level, CONFIG_BASE
 from .		import licensing
 
 
 __author__                      = "Perry Kundert"
 __email__                       = "perry@dominionrnd.com"
 __copyright__                   = "Copyright (c) 2022, Dominion Research & Development Corp."
 __license__                     = "Dual License: GPLv3 (or later) and Commercial (see LICENSE)"
@@ -36,144 +35,166 @@
 
 log				= logging.getLogger( __package__ )
 
 
 #
 # Generate Agent Keypairs and Licenses
 #
-# --filename	The name of the Keypair or License, eg. Some Name ==> some-name.crypto-key
+# --name	The name of the Keypair or License; recommend eg. Some Name ==> some-name.crypto-key
 #
 @click.group()
 @click.option('-v', '--verbose', count=True)
 @click.option('-q', '--quiet', count=True)
 @click.option('-p', '--private/--no-private', default=False, help="Disclose Private Key material")
 @click.option('-l', '--log-file', help="Log file name")
 @click.option('-w', '--why', help="What is being done (for logging details)")
-def cli( verbose, quiet, private, log_file, why ):
+@click.option('-n', '--name', help="Defines the file name loaded/saved (default: {base})".format( base=CONFIG_BASE ))
+@click.option('-r', '--reverse-save/--no-reverse-save', default=None, help="Reverse the search for saving Keypair/License files; from most specific to most general" )
+@click.option('-e', '--extra', multiple=True, help="Extra config directories to use, from most general to most specific" )
+def cli( verbose, quiet, private, log_file, why, name, reverse_save, extra ):
     cli.verbosity		= verbose - quiet
     log_cfg['level']		= log_level( cli.verbosity )
     if log_file:
         log_cfg['filename']	= log_file
     logging.basicConfig( **log_cfg )
     if verbose or quiet:
         logging.getLogger().setLevel( log_cfg['level'] )
     if private:
         cli.private	= True
     if why:
         cli.why		= why
+    cli.name		= name or CONFIG_BASE
+    if extra:
+        cli.extra	= list( extra )
+    if reverse_save is not None:
+        cli.reverse_save = reverse_save
 cli.private		= False  # noqa: E305
 cli.verbosity		= 0
 cli.why			= None
+cli.name		= None
+cli.extra		= None
+cli.reverse_save	= None
 
 
 @click.command()
-@click.option( "--name", help="Defines the file name Keypair is saved under" )
 @click.option( "--username", help="The email address (if encrypted Keypair desired))" )
 @click.option( "--password", help="The password" )
-def check( name, username, password ):
+def check( username, password ):
     """Check for Agent ID Ed25519 Key, and any associated License(s).  If neither Keypair nor
     License(s) are found, an Exception is raised.
 
     If not -q, outputs JSON { <key>: [ <lic>, ...], }
 
     """
     username		= username or os.getenv( licensing.ENVUSERNAME )
     password		= password or os.getenv( licensing.ENVPASSWORD )
     log.info( "Checking {why} w/ {username}: {password!r}".format(
-        why		= cli.why or name,
+        why		= cli.why or cli.name,
         username	= username,
         password	= '*' * len( password ) if password else password,
     ))
 
     i			= None
     licenses		= {}
     for i,(keypair_raw,lic) in enumerate( licensing.check(
-        basename	= name,
+        basename	= cli.name,
         username	= username,
         password	= password,
-        package		= __package__,
+        extra		= cli.extra,
     )):
         if not keypair_raw:
-            log.warning( "No Agent ID Keypair {name}".format( name=name or ''))
+            log.warning( "No Agent ID Keypair {name}".format( name=cli.name ))
         else:
             key		= licensing.into_hex( keypair_raw.sk ) if cli.private else licensing.into_b64( keypair_raw.vk )
             licenses.setdefault( key, [] )
             if lic:
                 licenses[key].append( lic )
     if cli.verbosity >= 0 and licenses:
         click.echo( licensing.into_JSON( licenses, indent=4, prefix=' ' * 4 ))
     assert licenses, \
-        "Failed to find any Agent ID Keypairs or Licenses for {}".format( name )
+        "Failed to find any Agent ID Keypairs or Licenses for {}".format( cli.name )
 
 
 @click.command()
-@click.option( "--name", help="Defines the file name Keypair is saved under" )
 @click.option( "--username", help="The email address (if encrypted Keypair desired))" )
 @click.option( "--password", help="The password" )
+@click.option( "--extension", help="A specific extension to look for" )
 @click.option( "--registering/--no-registering", default=True, help="If no Keypair found, create and register a new one" )
 @click.option( "--seed", help="A 32-byte (256-bit) Seed, in Hex (default: random)" )
-def registered( name, username, password, registering, seed ):
-    """Determine if the specified name and credentials are registerd.  Locate (or create and save,
-    by default) an Agent ID Ed25519 Keypair.
+def registered( username, password, extension, registering, seed ):
+    """Determine if the specified name and credentials are registered.  Locate (or create and save, by
+    default) an Agent ID Ed25519 Keypair.
 
-    If not -q, outputs JSON "<Pubkey>" (or "<Privkey>" if --private)
+    If not -q, outputs JSON "<Pubkey>" (or "<Privkey>" if --private).  If -v, the filename will also
+    be output.
+
+    If {ENVUSERNAME} and/or {ENVPASSWORD} environment variables are available, they will be used as
+    default values for --username / --password.
 
     """
     username		= username or os.getenv( licensing.ENVUSERNAME )
     password		= password or os.getenv( licensing.ENVPASSWORD )
     log.info( "Registering {why} w/ {username}: {password!r}".format(
-        why		= cli.why or name,
+        why		= cli.why or cli.name,
         username	= username,
         password	= '*' * len( password ) if password else password,
     ))
 
     keypair			= licensing.registered(
         seed		= codecs.decode( seed, 'hex_codec' ) if seed else None,
         why		= cli.why or username,
+        basename	= cli.name,
+        extension	= extension,
         username	= username,
         password	= password,
-        filename	= name,
-        package		= __package__,
         registering	= registering,
+        reverse_save	= cli.reverse_save,
+        extra		= cli.extra,
     )
+
     keypair_raw		= keypair.into_keypair(
         username	= username,
         password	= password,
     )
-    key			= licensing.into_hex( keypair_raw.sk ) if cli.private else licensing.into_b64( keypair_raw.vk )
+
+    val				= [ keypair._from ]
     if cli.verbosity >= 0:
-        click.echo( licensing.into_JSON( key, indent=4 ))
+        val.append( licensing.into_b64( keypair_raw.sk ) if cli.private else licensing.into_b64( keypair_raw.vk ))
+    if cli.verbosity >= 1:
+        assert cli.private or isinstance( keypair, licensing.KeypairEncrypted ), \
+            "Cannot display un-encrypted Keypair without --private option"
+        val.append( dict( keypair ))
+    click.echo( licensing.into_JSON( val, indent=4 ))
 
 
 @click.command()
-@click.option( "--name", help="Defines the file name author Keypair read from, License is saved under" )
 @click.option( "--username", help="The email address (if encrypted Keypair))" )
 @click.option( "--password", help="The password" )
 @click.option( "--registering/--no-registering", default=True, help="If no Keypair found, create and register a new one" )
 @click.option( "--author", help="The author's name (eg. 'Awesome, Inc.'" )
 @click.option( "--domain", help="The company's DNS domain (eg. 'awesome.com'" )
 @click.option( "--product", help="The product name, (eg. 'Awesome Product')" )
 @click.option( "--service", help="The DKIM/License Grant key, (default is derived from product, eg. 'awesome-product')" )
 @click.option( "--grant", help="The License's Grants (as JSON)" )
 @click.option( "--dependency", multiple=True, help="Sub-license the specified License (by filename) as one of this License's dependencies" )
 @click.option( "--confirm/--no-confirm", default=True, help="Confirm the signatures via DKIM (default: True)" )
 @click.option( "--client", help="The client's name (eg. 'Example, Inc.'" )
 @click.option( "--client-domain", help="The client's DNS domain (eg. 'example.com'" )
 @click.option( "--client-pubkey", help="The client's Ed25519 Agent ID" )
-def license( name, username, password, registering, author, domain, product, service, grant, dependency, confirm, client, client_domain, client_pubkey ):
+def license( username, password, registering, author, domain, product, service, grant, dependency, confirm, client, client_domain, client_pubkey ):
     """Load/create an Author ID, create/save a LicenseSigned for the specified product.
 
     Won't overwrite existing keypair or license files.
 
     Appends any specified dependencies without confirming signatures.
     """
     username		= username or os.getenv( licensing.ENVUSERNAME )
     password		= password or os.getenv( licensing.ENVPASSWORD )
     log.info( "Licensing {why} w/ {username}: {password!r}".format(
-        why		= cli.why or name,
+        why		= cli.why or cli.name,
         username	= username,
         password	= '*' * len( password ) if password else password,
     ))
 
     dependencies		= []
     for f in ( open( dep, 'r' ) for dep in dependency ):
         with f:
@@ -182,24 +203,26 @@
             prov		= licensing.LicenseSigned( confirm=confirm, _from=f.name, **prov_dict )
             log.detail( "Dependency: {prov!r}".format( prov=prov ))
         dependencies.append( prov )
 
     # Locate the Agent ID Keypair to use to author the License.  Default to create if not found.
     keypair			= licensing.registered(
         why		= cli.why or product,
-        basename	= name,
+        basename	= cli.name,
         username	= username,
         password	= password,
         registering	= registering,
+        reverse_save	= cli.reverse_save,
+        extra		= cli.extra,
     )
     keypair_raw			= keypair.into_keypair(
         username	= username,
         password	= password,
     )
-    key				= licensing.into_hex( keypair_raw.sk ) if cli.private else licensing.into_b64( keypair_raw.vk )
+    key				= licensing.into_b64( keypair_raw.sk ) if cli.private else licensing.into_b64( keypair_raw.vk )
     log.detail( "Authoring Agent ID {what}: {key}, from {path}".format(
         what	= "Keypair" if cli.private else "Pubkey",
         key	= key,
         path	= keypair._from,
     ))
     lic				= licensing.license(
         author		= licensing.Agent(
@@ -213,26 +236,22 @@
             name	= client or "End-User",
             domain	= client_domain,
             pubkey	= client_pubkey
         ),
         dependencies	= dependencies,
         grant		= grant,
         why		= cli.why or product,
-        basename	= name,
+        basename	= cli.name,
         confirm		= confirm,
+        reverse_save	= cli.reverse_save,
+        extra		= cli.extra,
     )
     log.normal( "Created License {!r} in {}".format( lic, lic._from ))
+    val				= [ lic._from ]
     if cli.verbosity >= 0:
-        click.echo( licensing.into_JSON( lic, indent=4 ))
+        val.append( dict( lic ))
+    click.echo( licensing.into_JSON( val, indent=4 ))
 
 
 cli.add_command( registered )
 cli.add_command( license )
 cli.add_command( check )
-
-try:
-    cli()
-except Exception as exc:
-    log.warning( "Failed: {exc}".format( exc=exc ))
-    sys.exit( 1 )
-else:
-    sys.exit( 0 )
```

### Comparing `crypto_licensing-3.0.4/crypto_licensing/crypto_test.py` & `crypto_licensing-3.3.0/crypto_licensing/crypto_test.py`

 * *Files identical despite different names*

### Comparing `crypto_licensing-3.0.4/crypto_licensing/ed25519/__init__.py` & `crypto_licensing-3.3.0/crypto_licensing/ed25519/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 # Crypto-licensing -- Cryptographically signed licensing, w/ Cryptocurrency payments
 #
 # Copyright (c) 2022, Dominion Research & Development Corp.
 #
 # Crypto-licensing is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
-# later version.  See the LICENSE file at the top of the source tree.
+# later version.  It is also available under alternative (eg. Commercial)
+# licenses, at your option.  See the LICENSE file at the top of the source tree.
 #
 # It is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
 # A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
 #
 
 import warnings
```

### Comparing `crypto_licensing-3.0.4/crypto_licensing/ed25519_djb.py` & `crypto_licensing-3.3.0/crypto_licensing/ed25519_djb.py`

 * *Files identical despite different names*

### Comparing `crypto_licensing-3.0.4/crypto_licensing/ed25519ll_pyonly/__init__.py` & `crypto_licensing-3.3.0/crypto_licensing/ed25519ll_pyonly/__init__.py`

 * *Files identical despite different names*

### Comparing `crypto_licensing-3.0.4/crypto_licensing/ed25519ll_pyonly/djbec.py` & `crypto_licensing-3.3.0/crypto_licensing/ed25519ll_pyonly/djbec.py`

 * *Files identical despite different names*

### Comparing `crypto_licensing-3.0.4/crypto_licensing/licensing/__init__.py` & `crypto_licensing-3.3.0/crypto_licensing/licensing/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,31 +3,32 @@
 # Crypto-licensing -- Cryptographically signed licensing, w/ Cryptocurrency payments
 #
 # Copyright (c) 2022, Dominion Research & Development Corp.
 #
 # Crypto-licensing is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
-# later version.  See the LICENSE file at the top of the source tree.
+# later version.  It is also available under alternative (eg. Commercial)
+# licenses, at your option.  See the LICENSE file at the top of the source tree.
 #
 # It is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
 # A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
 #
 
 from __future__ import absolute_import, print_function, division
 
 __author__                      = "Perry Kundert"
 __email__                       = "perry@dominionrnd.com"
-__copyright__                   = "Copyright (c) 2022, Dominion Research & Development Corp."
+__copyright__                   = "Copyright (c) 2022 Dominion Research & Development Corp."
 __license__                     = "Dual License: GPLv3 (or later) and Commercial (see LICENSE)"
 
 __all__				= [
     'Serializable', 'LicenseIncompatibility', 'License', 'LicenseSigned', 'Agent',
-    'domainkey', 'authoring', 'issue', 'verify', 'load', 'load_keys',
+    'domainkey', 'authoring', 'issue', 'verify', 'load', 'load_keypairs', 'save', 'save_keypair',
     'check', 'license',  'registered', 'authorized', 'machine_UUIDv4',
     'KeypairEncrypted', 'KeypairPlaintext',
     'KEYPATTERN', 'KEYEXTENSION', 'LICPATTERN', 'LICEXTENSION',
     'ENVPASSWORD', 'ENVUSERNAME',
 ]
 
 from .defaults		import *
```

### Comparing `crypto_licensing-3.0.4/crypto_licensing/licensing/__main__.py` & `crypto_licensing-3.3.0/crypto_licensing/licensing/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 
 #
-# Cpppo -- Communication Protocol Python Parser and Originator
+# Crypto-licensing -- Cryptographically signed licensing, w/ Cryptocurrency payments
 #
 # Copyright (c) 2022, Dominion Research & Development Corp.
 #
 # Crypto-licensing is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
-# later version.  See the LICENSE file at the top of the source tree.
+# later version.  It is also available under alternative (eg. Commercial)
+# licenses, at your option.  See the LICENSE file at the top of the source tree.
 #
 # It is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
 # A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
 #
 
 from __future__ import absolute_import, print_function, division
 
 import sys
 
 from .main import main
 
 __author__                      = "Perry Kundert"
 __email__                       = "perry@dominionrnd.com"
-__copyright__                   = "Copyright (c) 2022, Dominion Research & Development Corp."
+__copyright__                   = "Copyright (c) 2022 Dominion Research & Development Corp."
 __license__                     = "Dual License: GPLv3 (or later) and Commercial (see LICENSE)"
 
 sys.exit( main() )
```

### Comparing `crypto_licensing-3.0.4/crypto_licensing/licensing/bitquery_test.py` & `crypto_licensing-3.3.0/crypto_licensing/licensing/bitquery_test.py`

 * *Files identical despite different names*

### Comparing `crypto_licensing-3.0.4/crypto_licensing/licensing/defaults.py` & `crypto_licensing-3.3.0/crypto_licensing/licensing/defaults.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 # Crypto-licensing -- Cryptographically signed licensing, w/ Cryptocurrency payments
 #
 # Copyright (c) 2022, Dominion Research & Development Corp.
 #
 # Crypto-licensing is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
-# later version.  See the LICENSE file at the top of the source tree.
+# later version.  It is also available under alternative (eg. Commercial)
+# licenses, at your option.  See the LICENSE file at the top of the source tree.
 #
 # It is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
 # A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
 #
 
 from __future__ import absolute_import, print_function, division
```

### Comparing `crypto_licensing-3.0.4/crypto_licensing/licensing/doh/__init__.py` & `crypto_licensing-3.3.0/crypto_licensing/licensing/doh/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 # Crypto-licensing -- Cryptographically signed licensing, w/ Cryptocurrency payments
 #
 # Copyright (c) 2022, Dominion Research & Development Corp.
 #
 # Crypto-licensing is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
-# later version.  See the LICENSE file at the top of the source tree.
+# later version.  It is also available under alternative (eg. Commercial)
+# licenses, at your option.  See the LICENSE file at the top of the source tree.
 #
 # It is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
 # A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
 #
 
 """
```

### Comparing `crypto_licensing-3.0.4/crypto_licensing/licensing/doh/__main__.py` & `crypto_licensing-3.3.0/crypto_licensing/licensing/doh/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,8 +69,7 @@
             else:
                 click.echo( "{rec}".format( rec=rec['data'] ))
     if cli.json:
         click.echo( "\n]" if cli.verbosity != 0 else "]" )
 
 
 cli.add_command( dig )
-cli()
```

### Comparing `crypto_licensing-3.0.4/crypto_licensing/licensing/doh_test.py` & `crypto_licensing-3.3.0/crypto_licensing/licensing/doh_test.py`

 * *Files identical despite different names*

### Comparing `crypto_licensing-3.0.4/crypto_licensing/licensing/grant_test.py` & `crypto_licensing-3.3.0/crypto_licensing/licensing/grant_test.py`

 * *Files identical despite different names*

### Comparing `crypto_licensing-3.0.4/crypto_licensing/licensing/licensing_test.py` & `crypto_licensing-3.3.0/crypto_licensing/licensing/licensing_test.py`

 * *Files identical despite different names*

### Comparing `crypto_licensing-3.0.4/crypto_licensing/licensing/main.py` & `crypto_licensing-3.3.0/crypto_licensing/licensing/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,5975 +22,6007 @@
 00000150: 6c69 7368 6564 2062 7920 7468 6520 4672  lished by the Fr
 00000160: 6565 0a23 2053 6f66 7477 6172 6520 466f  ee.# Software Fo
 00000170: 756e 6461 7469 6f6e 2c20 6569 7468 6572  undation, either
 00000180: 2076 6572 7369 6f6e 2033 206f 6620 7468   version 3 of th
 00000190: 6520 4c69 6365 6e73 652c 206f 7220 2861  e License, or (a
 000001a0: 7420 796f 7572 206f 7074 696f 6e29 2061  t your option) a
 000001b0: 6e79 0a23 206c 6174 6572 2076 6572 7369  ny.# later versi
-000001c0: 6f6e 2e20 2053 6565 2074 6865 204c 4943  on.  See the LIC
-000001d0: 454e 5345 2066 696c 6520 6174 2074 6865  ENSE file at the
-000001e0: 2074 6f70 206f 6620 7468 6520 736f 7572   top of the sour
-000001f0: 6365 2074 7265 652e 0a23 0a23 2049 7420  ce tree..#.# It 
-00000200: 6973 2064 6973 7472 6962 7574 6564 2069  is distributed i
-00000210: 6e20 7468 6520 686f 7065 2074 6861 7420  n the hope that 
-00000220: 6974 2077 696c 6c20 6265 2075 7365 6675  it will be usefu
-00000230: 6c2c 2062 7574 2057 4954 484f 5554 2041  l, but WITHOUT A
-00000240: 4e59 0a23 2057 4152 5241 4e54 593b 2077  NY.# WARRANTY; w
-00000250: 6974 686f 7574 2065 7665 6e20 7468 6520  ithout even the 
-00000260: 696d 706c 6965 6420 7761 7272 616e 7479  implied warranty
-00000270: 206f 6620 4d45 5243 4841 4e54 4142 494c   of MERCHANTABIL
-00000280: 4954 5920 6f72 2046 4954 4e45 5353 2046  ITY or FITNESS F
-00000290: 4f52 0a23 2041 2050 4152 5449 4355 4c41  OR.# A PARTICULA
-000002a0: 5220 5055 5250 4f53 452e 2020 5365 6520  R PURPOSE.  See 
-000002b0: 7468 6520 474e 5520 4765 6e65 7261 6c20  the GNU General 
-000002c0: 5075 626c 6963 204c 6963 656e 7365 2066  Public License f
-000002d0: 6f72 206d 6f72 6520 6465 7461 696c 732e  or more details.
-000002e0: 0a23 0a0a 2222 220a 2020 2020 496d 706c  .#..""".    Impl
-000002f0: 656d 656e 7473 2074 6865 2043 7279 7074  ements the Crypt
-00000300: 6f20 4c69 6365 6e73 696e 6720 7365 7276  o Licensing serv
-00000310: 6572 0a22 2222 0a0a 6672 6f6d 205f 5f66  er."""..from __f
-00000320: 7574 7572 655f 5f20 696d 706f 7274 2070  uture__ import p
-00000330: 7269 6e74 5f66 756e 6374 696f 6e2c 2061  rint_function, a
-00000340: 6273 6f6c 7574 655f 696d 706f 7274 2c20  bsolute_import, 
-00000350: 6469 7669 7369 6f6e 0a0a 696d 706f 7274  division..import
-00000360: 2061 7267 7061 7273 650a 696d 706f 7274   argparse.import
-00000370: 2063 7572 7365 732c 2063 7572 7365 732e   curses, curses.
-00000380: 6173 6369 692c 2063 7572 7365 732e 7061  ascii, curses.pa
-00000390: 6e65 6c20 2023 206e 6f71 613a 2045 3430  nel  # noqa: E40
-000003a0: 310a 696d 706f 7274 2066 6e6d 6174 6368  1.import fnmatch
-000003b0: 0a69 6d70 6f72 7420 6a73 6f6e 0a69 6d70  .import json.imp
-000003c0: 6f72 7420 6c6f 6767 696e 670a 696d 706f  ort logging.impo
-000003d0: 7274 206f 730a 696d 706f 7274 2070 6f73  rt os.import pos
-000003e0: 6978 7061 7468 0a69 6d70 6f72 7420 7369  ixpath.import si
-000003f0: 676e 616c 0a69 6d70 6f72 7420 7371 6c69  gnal.import sqli
-00000400: 7465 330a 696d 706f 7274 2073 7973 0a69  te3.import sys.i
-00000410: 6d70 6f72 7420 7468 7265 6164 696e 670a  mport threading.
-00000420: 696d 706f 7274 2074 696d 650a 696d 706f  import time.impo
-00000430: 7274 2074 7261 6365 6261 636b 0a69 6d70  rt traceback.imp
-00000440: 6f72 7420 7761 726e 696e 6773 0a0a 2320  ort warnings..# 
-00000450: 5573 6564 2066 6f72 2057 6562 2047 5549  Used for Web GUI
-00000460: 2c20 616e 6420 666f 7220 6c69 6365 6e73  , and for licens
-00000470: 696e 6720 6461 7461 6261 7365 2e20 2049  ing database.  I
-00000480: 6e20 7468 6520 6675 7475 7265 2c20 6d75  n the future, mu
-00000490: 6368 206f 6620 7468 6973 2077 696c 6c20  ch of this will 
-000004a0: 7472 616e 7369 7469 6f6e 2074 6f0a 2320  transition to.# 
-000004b0: 486f 6c6f 6368 6169 6e2d 6261 7365 6420  Holochain-based 
-000004c0: 696e 6672 6173 7472 7563 7475 7265 2e0a  infrastructure..
-000004d0: 696d 706f 7274 2077 6562 0a69 6d70 6f72  import web.impor
-000004e0: 7420 7765 622e 6874 7470 7365 7276 6572  t web.httpserver
-000004f0: 0a69 6d70 6f72 7420 7773 6769 6c6f 670a  .import wsgilog.
-00000500: 0a66 726f 6d20 2e2e 6d69 7363 0909 696d  .from ..misc..im
-00000510: 706f 7274 2028 0a20 2020 2074 696d 6572  port (.    timer
-00000520: 2c20 5469 6d65 7374 616d 702c 0a20 2020  , Timestamp,.   
-00000530: 206c 6f67 5f63 6667 2c20 6c6f 675f 6c65   log_cfg, log_le
-00000540: 7665 6c6d 6170 2c20 6c6f 675f 6c65 7665  velmap, log_leve
-00000550: 6c2c 0a20 2020 2063 6f6e 6669 675f 7061  l,.    config_pa
-00000560: 7468 732c 2063 6f6e 6669 675f 6f70 656e  ths, config_open
-00000570: 2c20 436f 6e66 6967 4e6f 7446 6f75 6e64  , ConfigNotFound
-00000580: 4572 726f 722c 0a20 2020 2075 6e71 756f  Error,.    unquo
-00000590: 7465 0a29 0a66 726f 6d20 2e2e 0909 0969  te.).from .....i
-000005a0: 6d70 6f72 7420 6c69 6365 6e73 696e 670a  mport licensing.
-000005b0: 6672 6f6d 202e 2e6d 6973 6309 0969 6d70  from ..misc..imp
-000005c0: 6f72 7420 696e 7075 745f 7365 6375 7265  ort input_secure
-000005d0: 0a0a 5f5f 6175 7468 6f72 5f5f 2020 2020  ..__author__    
-000005e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000005f0: 2020 3d20 2250 6572 7279 204b 756e 6465    = "Perry Kunde
-00000600: 7274 220a 5f5f 656d 6169 6c5f 5f20 2020  rt".__email__   
-00000610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000620: 2020 2020 3d20 2270 6572 7279 4064 6f6d      = "perry@dom
-00000630: 696e 696f 6e72 6e64 2e63 6f6d 220a 5f5f  inionrnd.com".__
-00000640: 636f 7079 7269 6768 745f 5f20 2020 2020  copyright__     
-00000650: 2020 2020 2020 2020 2020 2020 2020 3d20                = 
-00000660: 2243 6f70 7972 6967 6874 2028 6329 2032  "Copyright (c) 2
-00000670: 3032 3220 446f 6d69 6e69 6f6e 2052 6573  022 Dominion Res
-00000680: 6561 7263 6820 2620 4465 7665 6c6f 706d  earch & Developm
-00000690: 656e 7420 436f 7270 2e22 0a5f 5f6c 6963  ent Corp.".__lic
-000006a0: 656e 7365 5f5f 2020 2020 2020 2020 2020  ense__          
-000006b0: 2020 2020 2020 2020 2020 203d 2022 4475             = "Du
-000006c0: 616c 204c 6963 656e 7365 3a20 4750 4c76  al License: GPLv
-000006d0: 3320 286f 7220 6c61 7465 7229 2061 6e64  3 (or later) and
-000006e0: 2043 6f6d 6d65 7263 6961 6c20 2873 6565   Commercial (see
-000006f0: 204c 4943 454e 5345 2922 0a0a 7765 622e   LICENSE)"..web.
-00000700: 636f 6e66 6967 2e64 6562 7567 2009 093d  config.debug ..=
-00000710: 2046 616c 7365 0a77 6562 2e63 6f6e 6669   False.web.confi
-00000720: 672e 7365 7373 696f 6e5f 7061 7261 6d65  g.session_parame
-00000730: 7465 7273 2e75 7064 6174 6528 207b 0a20  ters.update( {. 
-00000740: 2020 2027 636f 6f6b 6965 5f6e 616d 6527     'cookie_name'
-00000750: 3a09 2773 6573 7369 6f6e 272c 0a20 2020  :.'session',.   
-00000760: 2027 6967 6e6f 7265 5f65 7870 6972 7927   'ignore_expiry'
-00000770: 3a09 5472 7565 2c0a 2020 2020 2769 676e  :.True,.    'ign
-00000780: 6f72 655f 6368 616e 6765 5f69 7027 3a09  ore_change_ip':.
-00000790: 5472 7565 2c0a 2020 2020 2774 696d 656f  True,.    'timeo
-000007a0: 7574 273a 0909 372a 3234 2a36 302a 3630  ut':..7*24*60*60
-000007b0: 2c20 2020 2020 2320 3120 7765 656b 0a7d  ,     # 1 week.}
-000007c0: 2029 0a0a 7365 7373 696f 6e5f 696e 6974   )..session_init
-000007d0: 6961 6c69 7a65 7209 093d 207b 0a20 2020  ializer..= {.   
-000007e0: 2027 7573 6572 5f69 6427 3a09 302c 0a20   'user_id':.0,. 
-000007f0: 2020 2027 6e61 6d65 273a 0927 272c 0a20     'name':.'',. 
-00000800: 2020 2027 7069 6e27 3a09 302c 0a20 2020     'pin':.0,.   
-00000810: 2027 6c6f 6769 6e27 3a09 302c 0909 0923   'login':.0,...#
-00000820: 2030 2067 7565 7374 2c20 3120 7573 6572   0 guest, 1 user
-00000830: 2c20 3220 6164 6d69 6e0a 7d0a 0a0a 6c6f  , 2 admin.}...lo
-00000840: 6709 0909 093d 206c 6f67 6769 6e67 2e67  g....= logging.g
-00000850: 6574 4c6f 6767 6572 2820 226c 6963 656e  etLogger( "licen
-00000860: 7369 6e67 2220 290a 0a23 204f 7574 7075  sing" )..# Outpu
-00000870: 7420 6669 6c65 7320 6172 6520 7374 6f72  t files are stor
-00000880: 6564 2069 6e20 7468 6520 4357 440a 4c4f  ed in the CWD.LO
-00000890: 4746 494c 4509 0909 093d 2022 6c69 6365  GFILE....= "lice
-000008a0: 6e73 696e 672e 6c6f 6722 0a44 425f 4649  nsing.log".DB_FI
-000008b0: 4c45 0909 0909 3d20 226c 6963 656e 7369  LE....= "licensi
-000008c0: 6e67 2e64 6222 0a41 4343 4649 4c45 0909  ng.db".ACCFILE..
-000008d0: 0909 3d20 226c 6963 656e 7369 6e67 2e61  ..= "licensing.a
-000008e0: 6363 6573 7322 0a0a 4352 4446 494c 4509  ccess"..CRDFILE.
-000008f0: 0909 093d 2022 6c69 6365 6e73 696e 672e  ...= "licensing.
-00000900: 6372 6564 656e 7469 616c 7322 2020 2020  credentials"    
-00000910: 2020 2023 2041 6e79 2061 7574 686f 7220     # Any author 
-00000920: 6372 6564 656e 7469 616c 7320 6176 6169  credentials avai
-00000930: 6c61 626c 6520 7065 7273 6973 7465 6e74  lable persistent
-00000940: 6c79 0a4b 4559 4649 4c45 0909 0909 3d20  ly.KEYFILE....= 
-00000950: 226c 6963 656e 7369 6e67 2e22 202b 206c  "licensing." + l
-00000960: 6963 656e 7369 6e67 2e4b 4559 5041 5454  icensing.KEYPATT
-00000970: 4552 4e0a 4c49 4346 494c 4509 0909 093d  ERN.LICFILE....=
-00000980: 2022 6c69 6365 6e73 696e 672e 2220 2b20   "licensing." + 
-00000990: 6c69 6365 6e73 696e 672e 4c49 4350 4154  licensing.LICPAT
-000009a0: 5445 524e 0a0a 2320 5351 4c20 636f 6e66  TERN..# SQL conf
-000009b0: 6967 7572 6174 696f 6e73 2061 7265 2074  igurations are t
-000009c0: 7970 6963 616c 6c79 2066 6f75 6e64 2069  ypically found i
-000009d0: 6e20 6372 7970 746f 5f6c 6963 656e 7369  n crypto_licensi
-000009e0: 6e67 2f6c 6963 656e 7369 6e67 2c20 6275  ng/licensing, bu
-000009f0: 7420 6d61 7920 6265 2063 7573 746f 6d69  t may be customi
-00000a00: 7a65 6420 616e 640a 2320 706c 6163 6564  zed and.# placed
-00000a10: 2069 6e20 616e 7920 6f66 2074 6865 2043   in any of the C
-00000a20: 7070 706f 2063 6f6e 6669 6775 7261 7469  pppo configurati
-00000a30: 6f6e 2066 696c 6520 7061 7468 7320 2865  on file paths (e
-00000a40: 672e 207e 2f2e 6370 7070 6f2f 2c20 2f65  g. ~/.cpppo/, /e
-00000a50: 7463 2f63 7070 706f 2f2c 206f 7220 7468  tc/cpppo/, or th
-00000a60: 6520 6375 7272 656e 740a 2320 776f 726b  e current.# work
-00000a70: 696e 6720 6469 7265 6374 6f72 7929 0a53  ing directory).S
-00000a80: 514c 4649 4c45 0909 0909 3d20 226c 6963  QLFILE....= "lic
-00000a90: 656e 7369 6e67 2e73 716c 2209 0923 2074  ensing.sql"..# t
-00000aa0: 6869 7320 2b20 2e2a 2061 7265 206c 6f61  his + .* are loa
-00000ab0: 6465 640a 0a4f 5552 5041 5448 0909 0909  ded..OURPATH....
-00000ac0: 3d20 6f73 2e70 6174 682e 6469 726e 616d  = os.path.dirnam
-00000ad0: 6528 206f 732e 7061 7468 2e61 6273 7061  e( os.path.abspa
-00000ae0: 7468 2820 5f5f 6669 6c65 5f5f 2029 290a  th( __file__ )).
-00000af0: 5450 4c50 4154 4809 0909 093d 206f 732e  TPLPATH....= os.
-00000b00: 7061 7468 2e6a 6f69 6e28 204f 5552 5041  path.join( OURPA
-00000b10: 5448 2c20 2273 7461 7469 632f 7265 736f  TH, "static/reso
-00000b20: 7572 6365 732f 7465 6d70 6c61 7465 732f  urces/templates/
-00000b30: 2220 290a 4c4f 4350 4154 4809 0909 093d  " ).LOCPATH....=
-00000b40: 206f 732e 7061 7468 2e61 6273 7061 7468   os.path.abspath
-00000b50: 286f 732e 7061 7468 2e63 7572 6469 7229  (os.path.curdir)
-00000b60: 0a0a 2320 4c69 6365 6e73 6520 5365 7276  ..# License Serv
-00000b70: 6572 2043 6f6e 6669 6775 7261 7469 6f6e  er Configuration
-00000b80: 0a0a 636f 6e66 6967 5f65 7874 7261 7309  ..config_extras.
-00000b90: 0909 3d20 5b4f 5552 5041 5448 5d20 2023  ..= [OURPATH]  #
-00000ba0: 2041 6e79 2065 7874 7261 2068 6967 6865   Any extra highe
-00000bb0: 722d 7072 696f 7269 7479 2063 6f6e 6669  r-priority confi
-00000bc0: 6775 7261 7469 6f6e 2070 6174 6873 2074  guration paths t
-00000bd0: 6f20 6c6f 6f6b 2069 6e0a 0a0a 2320 5468  o look in...# Th
-00000be0: 6520 6461 7461 6261 7365 3a20 676c 6f62  e database: glob
-00000bf0: 616c 2027 6462 272c 2077 6869 6368 2069  al 'db', which i
-00000c00: 7320 6120 7765 622e 6461 7461 6261 7365  s a web.database
-00000c10: 2063 6f6e 6e65 6374 696f 6e2e 2020 416c   connection.  Al
-00000c20: 736f 2027 6462 5f6c 6f63 6b27 2c20 7369  so 'db_lock', si
-00000c30: 6e63 6520 7371 6c69 7465 3320 6973 0a23  nce sqlite3 is.#
-00000c40: 2074 6872 6561 642d 7361 6665 2c20 6275   thread-safe, bu
-00000c50: 7420 7769 6c6c 2072 6169 7365 2061 6e20  t will raise an 
-00000c60: 6578 6365 7074 696f 6e20 6966 206d 756c  exception if mul
-00000c70: 7469 706c 6520 7468 7265 6164 7320 6174  tiple threads at
-00000c80: 7465 6d70 7420 746f 2077 7269 7465 2c20  tempt to write, 
-00000c90: 7072 6f76 6964 6520 610a 2320 7468 7265  provide a.# thre
-00000ca0: 6164 696e 672e 4c6f 636b 2829 2074 6f20  ading.Lock() to 
-00000cb0: 616c 6c6f 7720 7365 7269 616c 697a 696e  allow serializin
-00000cc0: 6720 6f66 2061 6c6c 2064 6220 696e 7365  g of all db inse
-00000cd0: 7274 2c20 7570 6461 7465 2c20 6574 632e  rt, update, etc.
-00000ce0: 2062 6574 7765 656e 2074 6872 6561 6473   between threads
-00000cf0: 2e0a 0a23 2057 6520 7769 6c6c 202a 616c  ...# We will *al
-00000d00: 7761 7973 2a20 6578 6563 7574 6520 616c  ways* execute al
-00000d10: 6c20 6f66 2074 6865 2061 7661 696c 6162  l of the availab
-00000d20: 6c65 202e 2e2e 7371 6c2a 2073 6372 6970  le ...sql* scrip
-00000d30: 7473 2e20 2054 6865 7365 2063 6f6e 7461  ts.  These conta
-00000d40: 696e 2027 4352 4541 5445 2054 4142 4c45  in 'CREATE TABLE
-00000d50: 2720 616e 640a 2320 2749 4e53 4552 5427  ' and.# 'INSERT'
-00000d60: 2063 6f6d 6d61 6e64 732c 2077 6869 6368   commands, which
-00000d70: 2077 696c 6c20 6661 696c 2069 6620 7468   will fail if th
-00000d80: 6520 7370 6563 6966 6965 6420 7461 626c  e specified tabl
-00000d90: 652f 726f 7720 616c 7265 6164 7920 6578  e/row already ex
-00000da0: 6973 7473 2c20 736f 2061 7265 2073 6166  ists, so are saf
-00000db0: 6520 746f 2072 756e 0a23 2072 6570 6561  e to run.# repea
-00000dc0: 7465 646c 792e 2020 5768 656e 2077 6520  tedly.  When we 
-00000dd0: 6164 6420 7461 626c 6573 2061 6e64 2f6f  add tables and/o
-00000de0: 7220 726f 7773 2074 6861 7420 646f 6e27  r rows that don'
-00000df0: 7420 616c 7265 6164 7920 6578 6973 742c  t already exist,
-00000e00: 2074 6865 7927 6c6c 2062 6520 6372 6561   they'll be crea
-00000e10: 7465 6420 6279 2074 6865 7365 0a23 2073  ted by these.# s
-00000e20: 6372 6970 7473 2e20 2054 6869 7320 7072  cripts.  This pr
-00000e30: 6f76 6964 6573 2075 7320 7769 7468 2061  ovides us with a
-00000e40: 2072 7564 696d 656e 7461 7279 2064 6174   rudimentary dat
-00000e50: 6162 6173 6520 7570 6461 7465 206d 6563  abase update mec
-00000e60: 6861 6e69 736d 2062 6574 7765 656e 2072  hanism between r
-00000e70: 656c 6561 7365 732c 2061 7320 6c6f 6e67  eleases, as long
-00000e80: 0a23 2061 7320 7765 2063 6172 6566 756c  .# as we careful
-00000e90: 6c79 206d 6967 7261 7465 2064 6174 6120  ly migrate data 
-00000ea0: 6672 6f6d 206f 6c64 2074 6f20 6e65 7720  from old to new 
-00000eb0: 7461 626c 6573 2e0a 0a0a 6462 5f73 7461  tables....db_sta
-00000ec0: 7469 6373 0909 093d 207b 7d0a 6462 5f6c  tics...= {}.db_l
-00000ed0: 6f63 6b09 0909 093d 2074 6872 6561 6469  ock....= threadi
-00000ee0: 6e67 2e4c 6f63 6b28 290a 6462 0909 0909  ng.Lock().db....
-00000ef0: 3d20 4e6f 6e65 0a0a 0a64 6566 2064 625f  = None...def db_
-00000f00: 7365 7475 7028 293a 0a20 2020 2022 2222  setup():.    """
-00000f10: 5365 7420 7570 2061 7070 6c69 6361 7469  Set up applicati
-00000f20: 6f6e 2d67 6c6f 6261 6c20 6462 2c20 6462  on-global db, db
-00000f30: 5f6c 6f63 6b2c 202e 2e2e 2020 5368 6f75  _lock, ...  Shou
-00000f40: 6c64 2062 6520 646f 6e65 2061 6674 6572  ld be done after
-00000f50: 2063 6f6e 6669 675f 6578 7472 6173 2069   config_extras i
-00000f60: 7320 696e 6974 6961 6c69 7a65 642e 2222  s initialized.""
-00000f70: 220a 0a20 2020 2069 6e69 745f 6462 0909  "..    init_db..
-00000f80: 093d 204e 6f6e 650a 2020 2020 6462 5f66  .= None.    db_f
-00000f90: 696c 655f 7061 7468 0909 3d20 4442 5f46  ile_path..= DB_F
-00000fa0: 494c 450a 2020 2020 7371 6c66 696c 655f  ILE.    sqlfile_
-00000fb0: 7061 7468 0909 3d20 5351 4c46 494c 450a  path..= SQLFILE.
-00000fc0: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-00000fd0: 2023 204c 6f61 6420 7468 6520 6c69 6365   # Load the lice
-00000fe0: 6e73 696e 672e 6462 2066 696c 652e 2020  nsing.db file.  
-00000ff0: 4966 2069 7420 6361 6e20 6265 2066 6f75  If it can be fou
-00001000: 6e64 2073 6f6d 6577 6865 7265 2069 6e20  nd somewhere in 
-00001010: 7468 6520 636f 6e66 6967 7572 6174 696f  the configuratio
-00001020: 6e20 7061 7468 2c20 7573 6520 6974 202d  n path, use it -
-00001030: 2d0a 2020 2020 2020 2020 2320 6f74 6865  -.        # othe
-00001040: 7277 6973 652c 2061 7373 756d 6520 6974  rwise, assume it
-00001050: 2773 2073 7570 706f 7365 6420 746f 2062  's supposed to b
-00001060: 6520 6865 7265 2069 6e20 7468 6520 4357  e here in the CW
-00001070: 442e 0a20 2020 2020 2020 2074 7279 3a0a  D..        try:.
-00001080: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00001090: 6620 696e 2063 6f6e 6669 675f 6f70 656e  f in config_open
-000010a0: 2820 4442 5f46 494c 4520 293a 0a20 2020  ( DB_FILE ):.   
-000010b0: 2020 2020 2020 2020 2020 2020 2077 6974               wit
-000010c0: 6820 663a 0a20 2020 2020 2020 2020 2020  h f:.           
-000010d0: 2020 2020 2020 2020 2064 625f 6669 6c65           db_file
-000010e0: 5f70 6174 6820 3d20 662e 6e61 6d65 0a20  _path = f.name. 
-000010f0: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-00001100: 7265 616b 0a20 2020 2020 2020 2065 7863  reak.        exc
-00001110: 6570 7420 436f 6e66 6967 4e6f 7446 6f75  ept ConfigNotFou
-00001120: 6e64 4572 726f 723a 0a20 2020 2020 2020  ndError:.       
-00001130: 2020 2020 2070 6173 730a 2020 2020 2020       pass.      
-00001140: 2020 696e 6974 5f64 6209 0909 3d20 7371    init_db...= sq
-00001150: 6c69 7465 332e 636f 6e6e 6563 7428 2064  lite3.connect( d
-00001160: 625f 6669 6c65 5f70 6174 6820 290a 0a20  b_file_path ).. 
-00001170: 2020 2020 2020 2023 204c 6f61 6420 616c         # Load al
-00001180: 6c20 6c69 6365 6e73 696e 672e 7371 6c2a  l licensing.sql*
-00001190: 2063 6f6e 6669 6720 6669 6c65 7320 696e   config files in
-000011a0: 746f 2074 6865 206c 6963 656e 7369 6e67  to the licensing
-000011b0: 2e64 6220 5371 6c69 7465 3320 6669 6c65  .db Sqlite3 file
-000011c0: 2e20 2057 6520 7761 6e74 2074 6f20 6c6f  .  We want to lo
-000011d0: 6164 0a20 2020 2020 2020 2023 2053 514c  ad.        # SQL
-000011e0: 2066 696c 6573 2066 726f 6d20 6d6f 7374   files from most
-000011f0: 2067 656e 6572 616c 2f64 6973 7461 6e74   general/distant
-00001200: 2074 6f20 6d6f 7374 2073 7065 6369 6669   to most specifi
-00001210: 632f 6e65 6172 6573 742c 2073 6f20 6d61  c/nearest, so ma
-00001220: 6b65 2072 6576 6572 7365 3d46 616c 7365  ke reverse=False
-00001230: 2e0a 2020 2020 2020 2020 676c 6f62 616c  ..        global
-00001240: 2063 6f6e 6669 675f 6578 7472 610a 2020   config_extra.  
-00001250: 2020 2020 2020 666f 7220 6620 696e 2063        for f in c
-00001260: 6f6e 6669 675f 6f70 656e 2820 5351 4c46  onfig_open( SQLF
-00001270: 494c 452b 272a 272c 2065 7874 7261 3d63  ILE+'*', extra=c
-00001280: 6f6e 6669 675f 6578 7472 6173 2c20 736b  onfig_extras, sk
-00001290: 6970 3d27 2a7e 272c 2072 6576 6572 7365  ip='*~', reverse
-000012a0: 3d46 616c 7365 2029 3a0a 2020 2020 2020  =False ):.      
-000012b0: 2020 2020 2020 7769 7468 2066 3a0a 2020        with f:.  
-000012c0: 2020 2020 2020 2020 2020 2020 2020 7371                sq
-000012d0: 6c09 093d 2066 2e72 6561 6428 290a 2020  l..= f.read().  
-000012e0: 2020 2020 2020 2020 2020 2020 2020 7371                sq
-000012f0: 6c5f 6669 6c65 093d 2066 2e6e 616d 650a  l_file.= f.name.
-00001300: 2020 2020 2020 2020 2020 2020 7472 793a              try:
-00001310: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001320: 206c 6f67 2e69 6e66 6f28 2022 4c6f 6164   log.info( "Load
-00001330: 696e 6720 5351 4c20 6672 6f6d 207b 7d22  ing SQL from {}"
-00001340: 2e66 6f72 6d61 7428 2073 716c 5f66 696c  .format( sql_fil
-00001350: 6520 2929 0a20 2020 2020 2020 2020 2020  e )).           
-00001360: 2020 2020 2069 6e69 745f 6462 2e65 7865       init_db.exe
-00001370: 6375 7465 7363 7269 7074 2820 7371 6c20  cutescript( sql 
-00001380: 290a 2020 2020 2020 2020 2020 2020 6578  ).            ex
-00001390: 6365 7074 2028 7371 6c69 7465 332e 4f70  cept (sqlite3.Op
-000013a0: 6572 6174 696f 6e61 6c45 7272 6f72 2c73  erationalError,s
-000013b0: 716c 6974 6533 2e49 6e74 6567 7269 7479  qlite3.Integrity
-000013c0: 4572 726f 7229 2061 7320 6578 633a 0a20  Error) as exc:. 
-000013d0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-000013e0: 6f67 2e69 6e66 6f28 2022 4661 696c 6564  og.info( "Failed
-000013f0: 2074 6f20 6c6f 6164 2025 7320 2870 726f   to load %s (pro
-00001400: 6261 626c 7920 616c 7265 6164 7920 636f  bably already co
-00001410: 6e66 6967 7572 6564 2c20 636f 6e74 696e  nfigured, contin
-00001420: 7569 6e67 293a 2025 7322 2c20 7371 6c5f  uing): %s", sql_
-00001430: 6669 6c65 2c20 6578 6320 290a 2020 2020  file, exc ).    
-00001440: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
-00001450: 2061 7320 6578 633a 0a20 2020 2020 2020   as exc:.       
-00001460: 206c 6f67 2e77 6172 6e69 6e67 2820 2246   log.warning( "F
-00001470: 6169 6c65 6420 746f 2065 7865 6375 7465  ailed to execute
-00001480: 207b 7d2a 2073 6372 6970 7473 2069 6e74   {}* scripts int
-00001490: 6f20 4442 207b 7d3a 207b 7d22 2e66 6f72  o DB {}: {}".for
-000014a0: 6d61 7428 0a20 2020 2020 2020 2020 2020  mat(.           
-000014b0: 2073 716c 6669 6c65 5f70 6174 682c 2064   sqlfile_path, d
-000014c0: 625f 6669 6c65 5f70 6174 682c 2065 7863  b_file_path, exc
-000014d0: 2029 290a 2020 2020 2020 2020 7261 6973   )).        rais
-000014e0: 650a 2020 2020 6669 6e61 6c6c 793a 0a20  e.    finally:. 
-000014f0: 2020 2020 2020 2069 6620 696e 6974 5f64         if init_d
-00001500: 623a 0a20 2020 2020 2020 2020 2020 2069  b:.            i
-00001510: 6e69 745f 6462 2e63 6c6f 7365 2829 0a20  nit_db.close(). 
-00001520: 2020 2061 7373 6572 7420 6f73 2e61 6363     assert os.acc
-00001530: 6573 7328 2064 625f 6669 6c65 5f70 6174  ess( db_file_pat
-00001540: 682c 206f 732e 575f 4f4b 2029 2c20 5c0a  h, os.W_OK ), \.
-00001550: 2020 2020 2020 2020 2243 616e 6e6f 7420          "Cannot 
-00001560: 6163 6365 7373 206c 6963 656e 7369 6e67  access licensing
-00001570: 2044 423a 207b 7d22 2e66 6f72 6d61 7428   DB: {}".format(
-00001580: 2064 625f 6669 6c65 5f70 6174 6820 290a   db_file_path ).
-00001590: 0a20 2020 2023 204f 4b2c 2074 6865 2044  .    # OK, the D
-000015a0: 4220 6861 7320 6265 656e 2069 6e69 7469  B has been initi
-000015b0: 616c 697a 6564 2c20 616e 6420 6973 2061  alized, and is a
-000015c0: 7420 6462 5f66 696c 655f 7061 7468 2e0a  t db_file_path..
-000015d0: 2020 2020 6c6f 672e 7761 726e 696e 6728      log.warning(
-000015e0: 2022 4f70 656e 696e 6720 4442 2061 7420   "Opening DB at 
-000015f0: 7b70 6174 687d 222e 666f 726d 6174 2820  {path}".format( 
-00001600: 7061 7468 3d64 625f 6669 6c65 5f70 6174  path=db_file_pat
-00001610: 6820 2929 0a20 2020 2067 6c6f 6261 6c20  h )).    global 
-00001620: 6462 0a20 2020 2064 6209 0909 093d 2077  db.    db....= w
-00001630: 6562 2e64 6174 6162 6173 6528 2064 626e  eb.database( dbn
-00001640: 3d27 7371 6c69 7465 272c 2064 623d 6462  ='sqlite', db=db
-00001650: 5f66 696c 655f 7061 7468 2029 0a20 2020  _file_path ).   
-00001660: 2061 7373 6572 7420 6861 7361 7474 7228   assert hasattr(
-00001670: 2064 622c 2027 7175 6572 7927 2029 2c20   db, 'query' ), 
-00001680: 5c0a 2020 2020 2020 2020 2255 6e72 6563  \.        "Unrec
-00001690: 6f67 6e69 7a65 6420 6c69 6365 6e73 696e  ognized licensin
-000016a0: 6720 4442 2063 6f6e 6e65 6374 696f 6e3a  g DB connection:
-000016b0: 207b 2172 7d22 2025 2028 2064 6220 290a   {!r}" % ( db ).
-000016c0: 0a20 2020 2023 2056 6172 696f 7573 2073  .    # Various s
-000016d0: 7461 7469 6320 7661 6c75 6573 2074 6861  tatic values tha
-000016e0: 7420 7368 6f75 6c64 2062 6520 7361 7665  t should be save
-000016f0: 642f 7265 7374 6f72 6564 2e20 2041 6c77  d/restored.  Alw
-00001700: 6179 7320 6265 6769 6e73 2061 7420 6465  ays begins at de
-00001710: 6661 756c 7473 206f 6e20 7374 6172 742d  faults on start-
-00001720: 7570 210a 2020 2020 2320 4275 742c 2061  up!.    # But, a
-00001730: 6c73 6f20 7265 6164 2066 726f 6d20 6461  lso read from da
-00001740: 7461 6261 7365 2e20 2041 6c6c 2066 6c6f  tabase.  All flo
-00001750: 6174 696e 6720 706f 696e 742e 0a20 2020  ating point..   
-00001760: 2067 6c6f 6261 6c20 6462 5f73 7461 7469   global db_stati
-00001770: 6373 0a20 2020 2064 625f 7374 6174 6963  cs.    db_static
-00001780: 7309 0909 3d20 7b7d 0a20 2020 2066 6f72  s...= {}.    for
-00001790: 2072 2069 6e20 6462 2e73 656c 6563 7428   r in db.select(
-000017a0: 2027 7374 6174 6963 7327 2029 3a0a 2020   'statics' ):.  
-000017b0: 2020 2020 2020 6462 5f73 7461 7469 6373        db_statics
-000017c0: 5b72 2e6b 6579 5d09 093d 2066 6c6f 6174  [r.key]..= float
-000017d0: 2820 722e 7661 6c75 6520 290a 0a0a 6465  ( r.value )...de
-000017e0: 6620 6462 5f73 7461 7465 5f73 6176 6528  f db_state_save(
-000017f0: 293a 0a20 2020 2022 2222 4475 6d70 206f  ):.    """Dump o
-00001800: 7574 2061 6e79 2070 6572 7369 7374 656e  ut any persisten
-00001810: 7420 6c69 6365 6e73 696e 6720 6461 7461  t licensing data
-00001820: 2c20 6574 632e 2074 6861 7420 7368 6f75  , etc. that shou
-00001830: 6c64 2062 6520 6c6f 6164 6564 206e 6578  ld be loaded nex
-00001840: 7420 7469 6d65 2e20 2054 6869 7320 7368  t time.  This sh
-00001850: 6f75 6c64 2062 6520 646f 6e65 0a20 2020  ould be done.   
-00001860: 2066 726f 6d20 7469 6d65 2074 6f20 7469   from time to ti
-00001870: 6d65 2c20 736f 2077 6520 646f 6e27 7420  me, so we don't 
-00001880: 6765 7420 746f 6f20 6661 7220 6265 6869  get too far behi
-00001890: 6e64 2c20 696e 2063 6173 6520 6f66 2061  nd, in case of a
-000018a0: 2063 6f6c 6420 7265 626f 6f74 2e20 204f   cold reboot.  O
-000018b0: 6620 636f 7572 7365 2c20 7361 7665 0a20  f course, save. 
-000018c0: 2020 2069 6d6d 6564 6961 7465 6c79 2075     immediately u
-000018d0: 706f 6e20 6c69 6365 6e73 6520 6372 6561  pon license crea
-000018e0: 7469 6f6e 2c20 6574 632e 0a0a 2020 2020  tion, etc...    
-000018f0: 4d61 6b65 2063 6572 7461 696e 2074 6861  Make certain tha
-00001900: 7420 616c 6c20 7371 6c69 7465 3320 6461  t all sqlite3 da
-00001910: 7461 6261 7365 2063 616c 6c73 2061 7265  tabase calls are
-00001920: 2072 756e 2069 6e20 6120 7369 6e67 6c65   run in a single
-00001930: 2054 6872 6561 642e 2020 5765 276c 6c20   Thread.  We'll 
-00001940: 646f 2074 6865 206c 6f61 6469 6e67 0a20  do the loading. 
-00001950: 2020 2072 6967 6874 2062 656c 6f77 2028     right below (
-00001960: 6865 7265 2c20 696e 2074 6865 204d 6169  here, in the Mai
-00001970: 6e20 5468 7265 6164 292c 2062 7574 2061  n Thread), but a
-00001980: 6c6c 206f 7468 6572 2064 6174 6162 6173  ll other databas
-00001990: 6520 492f 4f20 2869 6e63 6c75 6469 6e67  e I/O (including
-000019a0: 2073 7461 7465 5f73 6176 6528 2929 206d   state_save()) m
-000019b0: 7573 740a 2020 2020 6f63 6375 7220 696e  ust.    occur in
-000019c0: 2074 6865 2077 6562 7079 2054 6872 6561   the webpy Threa
-000019d0: 642e 2e2e 0a0a 2020 2020 4672 6f6d 2068  d.....    From h
-000019e0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000019f0: 6d2f 7361 6d70 7379 6f2f 6265 6574 730a  m/sampsyo/beets.
-00001a00: 2020 2020 2222 220a 2020 2020 7769 7468      """.    with
-00001a10: 2064 625f 6c6f 636b 3a0a 2020 2020 2020   db_lock:.      
-00001a20: 2020 6c6f 672e 696e 666f 2820 2253 6176    log.info( "Sav
-00001a30: 696e 6720 7374 6174 6520 2874 6872 6561  ing state (threa
-00001a40: 643a 2025 7329 222c 2074 6872 6561 6469  d: %s)", threadi
-00001a50: 6e67 2e63 7572 7265 6e74 5f74 6872 6561  ng.current_threa
-00001a60: 6428 292e 6964 656e 7420 290a 0a20 2020  d().ident )..   
-00001a70: 2020 2020 2066 6f72 206b 2069 6e20 6462       for k in db
-00001a80: 5f73 7461 7469 6373 3a0a 2020 2020 2020  _statics:.      
-00001a90: 2020 2020 2020 6966 206e 6f74 2064 622e        if not db.
-00001aa0: 7570 6461 7465 2820 2773 7461 7469 6373  update( 'statics
-00001ab0: 272c 2077 6865 7265 3d22 6b65 7920 3d20  ', where="key = 
-00001ac0: 246b 6579 222c 2076 6172 733d 7b20 226b  $key", vars={ "k
-00001ad0: 6579 223a 206b 207d 2c20 7661 6c75 653d  ey": k }, value=
-00001ae0: 6462 5f73 7461 7469 6373 5b6b 5d20 293a  db_statics[k] ):
-00001af0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001b00: 2069 6620 6e6f 7420 6462 2e69 6e73 6572   if not db.inser
-00001b10: 7428 2027 7374 6174 6963 7327 2c20 6b65  t( 'statics', ke
-00001b20: 793d 6b2c 2076 616c 7565 3d64 625f 7374  y=k, value=db_st
-00001b30: 6174 6963 735b 6b5d 2029 3a0a 2020 2020  atics[k] ):.    
-00001b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b50: 6c6f 672e 7761 726e 696e 6728 2022 4661  log.warning( "Fa
-00001b60: 696c 6564 2074 6f20 7374 6f72 6520 7374  iled to store st
-00001b70: 6174 6963 7320 6b65 7920 2573 2076 616c  atics key %s val
-00001b80: 7565 2025 7322 2025 2028 206b 2c20 6462  ue %s" % ( k, db
-00001b90: 5f73 7461 7469 6373 5b6b 5d20 2929 0a0a  _statics[k] ))..
-00001ba0: 0a64 6566 206c 6963 656e 7365 7328 2063  .def licenses( c
-00001bb0: 6f6e 6669 726d 3d4e 6f6e 652c 2073 746f  onfirm=None, sto
-00001bc0: 7265 643d 4e6f 6e65 2029 3a0a 2020 2020  red=None ):.    
-00001bd0: 2222 224f 6274 6169 6e20 616c 6c20 4c69  """Obtain all Li
-00001be0: 6365 6e73 6520 7072 6f76 656e 616e 6365  cense provenance
-00001bf0: 7320 6375 7272 656e 746c 7920 6176 6169  s currently avai
-00001c00: 6c61 626c 6520 6672 6f6d 2074 6865 2044  lable from the D
-00001c10: 4220 616e 6420 6669 6c65 732c 2061 7320  B and files, as 
-00001c20: 6120 7365 7175 656e 6365 206f 660a 2020  a sequence of.  
-00001c30: 2020 2873 6967 6e61 7475 7265 2c20 4c69    (signature, Li
-00001c40: 6365 6e73 6529 2070 726f 7665 6e61 6e63  cense) provenanc
-00001c50: 6520 7061 6972 733b 2073 6967 6e61 7475  e pairs; signatu
-00001c60: 7265 2069 7320 6120 3531 322d 6269 7420  re is a 512-bit 
-00001c70: 4564 3235 3531 3920 5369 676e 6174 7572  Ed25519 Signatur
-00001c80: 6520 6173 2062 7974 6573 2e0a 0a20 2020  e as bytes...   
-00001c90: 2045 6163 6820 6c69 6365 6e73 6520 7072   Each license pr
-00001ca0: 6f76 656e 616e 6365 2063 6f6d 7072 6973  ovenance compris
-00001cb0: 6573 2061 204c 6963 656e 7365 2061 6e64  es a License and
-00001cc0: 2061 6e20 4564 3235 3531 3920 5369 676e   an Ed25519 Sign
-00001cd0: 6174 7572 652c 2061 6e64 206d 6179 2063  ature, and may c
-00001ce0: 6f6e 7461 696e 2064 6570 656e 6465 6e63  ontain dependenc
-00001cf0: 6965 732e 0a0a 2020 2020 416c 6c20 756e  ies...    All un
-00001d00: 6971 7565 206c 6963 656e 7365 7320 6172  ique licenses ar
-00001d10: 6520 666f 756e 6420 616e 6420 7969 656c  e found and yiel
-00001d20: 6465 642c 2069 6e64 6578 6564 2062 7920  ded, indexed by 
-00001d30: 7468 6569 7220 7369 676e 6174 7572 6573  their signatures
-00001d40: 2e0a 0a20 2020 2041 6e79 204c 6963 656e  ...    Any Licen
-00001d50: 7365 2066 6f72 2077 6869 6368 2079 6f75  se for which you
-00001d60: 2068 6f6c 6420 7468 6520 4175 7468 6f72   hold the Author
-00001d70: 2073 6967 6e69 6e67 206b 6579 7061 6972   signing keypair
-00001d80: 206d 6174 6368 696e 6720 7468 6520 4c69   matching the Li
-00001d90: 6365 6e73 6573 2720 6465 7369 676e 6564  censes' designed
-00001da0: 2063 6c69 656e 740a 2020 2020 2f20 636c   client.    / cl
-00001db0: 6965 6e74 5f70 7562 6b65 7920 286f 7220  ient_pubkey (or 
-00001dc0: 7468 6579 2061 7265 206e 756c 6c2f 4e6f  they are null/No
-00001dd0: 6e65 2920 6d61 7920 6265 2069 6e63 6c75  ne) may be inclu
-00001de0: 6465 6420 696e 2061 206e 6577 204c 6963  ded in a new Lic
-00001df0: 656e 7365 2773 2064 6570 656e 6465 6e63  ense's dependenc
-00001e00: 6965 732e 0a0a 2020 2020 496e 206f 7468  ies...    In oth
-00001e10: 6572 2077 6f72 6473 2c20 796f 7520 6d61  er words, you ma
-00001e20: 7920 6372 6561 7465 2061 6e64 2061 7574  y create and aut
-00001e30: 686f 7220 2873 6967 6e29 2061 2062 7261  hor (sign) a bra
-00001e40: 6e64 206e 6577 204c 6963 656e 7365 2077  nd new License w
-00001e50: 6974 6820 6e6f 2064 6570 656e 6465 6e63  ith no dependenc
-00001e60: 6965 732c 206f 720a 2020 2020 7769 7468  ies, or.    with
-00001e70: 2064 6570 656e 6465 6e63 6965 7320 7468   dependencies th
-00001e80: 6174 2068 6176 6520 6120 636c 6965 6e74  at have a client
-00001e90: 202f 2063 6c69 656e 745f 7075 626b 6579   / client_pubkey
-00001ea0: 206d 6174 6368 696e 6720 796f 7572 2061   matching your a
-00001eb0: 7574 686f 7269 6e67 206b 6579 7061 6972  uthoring keypair
-00001ec0: 2070 7562 6b65 792e 0a0a 2020 2020 544f   pubkey...    TO
-00001ed0: 444f 3a20 4c69 6365 6e73 6573 2073 7065  DO: Licenses spe
-00001ee0: 6369 6679 696e 6720 6120 2a6e 756d 6265  cifying a *numbe
-00001ef0: 722a 206f 6620 7468 696e 6773 206d 6179  r* of things may
-00001f00: 2062 6520 7573 6564 2061 7320 6465 7065   be used as depe
-00001f10: 6e64 656e 6369 6573 2069 6e20 6175 7468  ndencies in auth
-00001f20: 6f72 6564 204c 6963 656e 7365 730a 2020  ored Licenses.  
-00001f30: 2020 756e 7469 6c20 7468 6520 7375 6d20    until the sum 
-00001f40: 6f66 2074 686f 7365 2074 6869 6e67 7320  of those things 
-00001f50: 616c 6c6f 6361 7465 6420 746f 2074 6865  allocated to the
-00001f60: 2061 7574 686f 7265 6420 6c69 6365 6e73   authored licens
-00001f70: 6573 206d 6565 7473 2074 6865 204c 6963  es meets the Lic
-00001f80: 656e 7365 2064 6570 656e 6465 6e63 6965  ense dependencie
-00001f90: 7327 0a20 2020 206e 756d 6265 7220 6c69  s'.    number li
-00001fa0: 6d69 742e 0a0a 2020 2020 2222 220a 2020  mit...    """.  
-00001fb0: 2020 656d 6974 7465 6409 0909 3d20 7365    emitted...= se
-00001fc0: 7428 290a 0a20 2020 2064 6566 2065 6d69  t()..    def emi
-00001fd0: 7428 202a 7072 6f76 7320 293a 0a20 2020  t( *provs ):.   
-00001fe0: 2020 2020 2066 6f72 2070 2069 6e20 7072       for p in pr
-00001ff0: 6f76 733a 0a20 2020 2020 2020 2020 2020  ovs:.           
-00002000: 2069 6620 702e 7369 676e 6174 7572 6520   if p.signature 
-00002010: 696e 2065 6d69 7474 6564 3a0a 2020 2020  in emitted:.    
-00002020: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
-00002030: 696e 7565 0a20 2020 2020 2020 2020 2020  inue.           
-00002040: 2079 6965 6c64 2070 2e73 6967 6e61 7475   yield p.signatu
-00002050: 7265 2c20 702e 6c69 6365 6e73 650a 2020  re, p.license.  
-00002060: 2020 2020 2020 2020 2020 656d 6974 7465            emitte
-00002070: 642e 6164 6428 2070 2e73 6967 6e61 7475  d.add( p.signatu
-00002080: 7265 2029 0a20 2020 2020 2020 2020 2020  re ).           
-00002090: 2066 6f72 2073 6967 2c20 6c69 6320 696e   for sig, lic in
-000020a0: 2065 6d69 7428 202a 5b20 6c69 6365 6e73   emit( *[ licens
-000020b0: 696e 672e 4c69 6365 6e73 6553 6967 6e65  ing.LicenseSigne
-000020c0: 6428 2063 6f6e 6669 726d 3d63 6f6e 6669  d( confirm=confi
-000020d0: 726d 2c20 6d61 6368 696e 655f 6964 5f70  rm, machine_id_p
-000020e0: 6174 683d 4661 6c73 652c 202a 2a70 6420  ath=False, **pd 
-000020f0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00002100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002110: 2020 2020 2020 2066 6f72 2070 6420 696e         for pd in
-00002120: 2070 2e6c 6963 656e 7365 2e64 6570 656e   p.license.depen
-00002130: 6465 6e63 6965 7320 6f72 205b 5d20 5d20  dencies or [] ] 
-00002140: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00002150: 2020 2079 6965 6c64 2073 6967 2c20 6c69     yield sig, li
-00002160: 630a 0a20 2020 2023 2046 6972 7374 2c20  c..    # First, 
-00002170: 7072 6f63 6573 7320 616e 7920 7374 6f72  process any stor
-00002180: 6564 2070 726f 7665 6e61 6e63 6573 2e20  ed provenances. 
-00002190: 2054 6865 7365 2061 7265 2061 7373 756d   These are assum
-000021a0: 6564 2074 6f20 636f 6e74 6169 6e20 2e6c  ed to contain .l
-000021b0: 6963 656e 7365 2061 6e64 202e 7369 676e  icense and .sign
-000021c0: 6174 7572 650a 2020 2020 2320 6174 7472  ature.    # attr
-000021d0: 6962 7574 6573 2e20 2043 6f75 6c64 2062  ibutes.  Could b
-000021e0: 6520 6120 7365 7175 656e 6365 206f 6620  e a sequence of 
-000021f0: 4c69 6365 6e73 6553 6967 6e65 642c 206f  LicenseSigned, o
-00002200: 7220 6120 6461 7461 6261 7365 2071 7565  r a database que
-00002210: 7279 2079 6965 6c64 696e 6720 7265 636f  ry yielding reco
-00002220: 7264 7320 7769 7468 0a20 2020 2023 202e  rds with.    # .
-00002230: 7369 676e 6174 7572 6520 616e 6420 2e6c  signature and .l
-00002240: 6963 656e 7365 2e20 2054 6865 7365 206d  icense.  These m
-00002250: 6179 2062 6520 6675 6c6c 204c 6963 656e  ay be full Licen
-00002260: 7365 7320 7374 7275 6374 7320 616e 6420  ses structs and 
-00002270: 7369 676e 6174 7572 6573 2062 7974 6573  signatures bytes
-00002280: 2064 6174 612c 206f 720a 2020 2020 2320   data, or.    # 
-00002290: 7365 7269 616c 697a 6564 2066 6f72 6d73  serialized forms
-000022a0: 2e0a 2020 2020 666f 756e 6409 0909 3d20  ..    found...= 
-000022b0: 300a 2020 2020 666f 7220 7220 696e 2073  0.    for r in s
-000022c0: 746f 7265 6420 6f72 205b 5d3a 0a20 2020  tored or []:.   
-000022d0: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
-000022e0: 2020 2020 2020 7072 6f76 0909 3d20 6c69        prov..= li
-000022f0: 6365 6e73 696e 672e 4c69 6365 6e73 6553  censing.LicenseS
-00002300: 6967 6e65 6428 0a20 2020 2020 2020 2020  igned(.         
-00002310: 2020 2020 2020 206c 6963 656e 7365 3d72         license=r
-00002320: 2e6c 6963 656e 7365 2c20 7369 676e 6174  .license, signat
-00002330: 7572 653d 722e 7369 676e 6174 7572 652c  ure=r.signature,
-00002340: 2063 6f6e 6669 726d 3d63 6f6e 6669 726d   confirm=confirm
-00002350: 2c20 6d61 6368 696e 655f 6964 5f70 6174  , machine_id_pat
-00002360: 683d 4661 6c73 6520 290a 2020 2020 2020  h=False ).      
-00002370: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
-00002380: 6f6e 2061 7320 6578 633a 0a20 2020 2020  on as exc:.     
-00002390: 2020 2020 2020 206c 6f67 2e64 6562 7567         log.debug
-000023a0: 2820 2246 6169 6c65 6420 746f 206c 6f61  ( "Failed to loa
-000023b0: 6420 7374 6f72 6564 204c 6963 656e 7365  d stored License
-000023c0: 2070 726f 7665 6e61 6e63 653a 207b 6578   provenance: {ex
-000023d0: 637d 2066 726f 6d3a 207b 6c69 637d 222e  c} from: {lic}".
-000023e0: 666f 726d 6174 280a 2020 2020 2020 2020  format(.        
-000023f0: 2020 2020 2020 2020 6578 633d 2727 2e6a          exc=''.j
-00002400: 6f69 6e28 2074 7261 6365 6261 636b 2e66  oin( traceback.f
-00002410: 6f72 6d61 745f 6578 6365 7074 696f 6e28  ormat_exception(
-00002420: 202a 7379 732e 6578 635f 696e 666f 2829   *sys.exc_info()
-00002430: 2029 2920 6966 206c 6f67 2e69 7345 6e61   )) if log.isEna
-00002440: 626c 6564 466f 7228 206c 6f67 6769 6e67  bledFor( logging
-00002450: 2e54 5241 4345 2029 2065 6c73 6520 6578  .TRACE ) else ex
-00002460: 632c 0a20 2020 2020 2020 2020 2020 2020  c,.             
-00002470: 2020 206c 6963 3d72 2e6c 6963 656e 7365     lic=r.license
-00002480: 2029 290a 2020 2020 2020 2020 2020 2020   )).            
-00002490: 7261 6973 650a 2020 2020 2020 2020 666f  raise.        fo
-000024a0: 7220 7369 672c 206c 6963 2069 6e20 656d  r sig, lic in em
-000024b0: 6974 2820 7072 6f76 2029 3a0a 2020 2020  it( prov ):.    
-000024c0: 2020 2020 2020 2020 7969 656c 6420 7369          yield si
-000024d0: 672c 206c 6963 0a20 2020 2020 2020 2020  g, lic.         
-000024e0: 2020 2066 6f75 6e64 0920 2020 2020 2020     found.       
-000024f0: 2b3d 2031 0a20 2020 206c 6f67 2e69 6e66  += 1.    log.inf
-00002500: 6f28 2022 4c69 6365 6e73 6573 2020 2020  o( "Licenses    
-00002510: 2073 6176 6564 3a20 7b7d 222e 666f 726d   saved: {}".form
-00002520: 6174 2820 666f 756e 6420 2929 0a0a 2020  at( found ))..  
-00002530: 2020 666f 756e 6409 0909 3d20 300a 2020    found...= 0.  
-00002540: 2020 7061 7468 0909 093d 204e 6f6e 650a    path...= None.
-00002550: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-00002560: 2023 204c 6f61 6420 6d6f 7374 2067 656e   # Load most gen
-00002570: 6572 616c 2f64 6973 7461 6e74 204c 6963  eral/distant Lic
-00002580: 656e 7365 7320 6669 7273 742c 2069 6e63  enses first, inc
-00002590: 6c75 6469 6e67 2074 6865 206f 7074 696f  luding the optio
-000025a0: 6e61 6c20 6578 7472 6120 636f 6e66 6967  nal extra config
-000025b0: 2064 6972 730a 2020 2020 2020 2020 676c   dirs.        gl
-000025c0: 6f62 616c 2063 6f6e 6669 675f 6578 7472  obal config_extr
-000025d0: 6173 0a20 2020 2020 2020 2066 6f72 2070  as.        for p
-000025e0: 6174 682c 2070 726f 7620 696e 206c 6963  ath, prov in lic
-000025f0: 656e 7369 6e67 2e6c 6f61 6428 2070 6163  ensing.load( pac
-00002600: 6b61 6765 3d5f 5f70 6163 6b61 6765 5f5f  kage=__package__
-00002610: 2c20 6578 7472 613d 636f 6e66 6967 5f65  , extra=config_e
-00002620: 7874 7261 732c 2072 6576 6572 7365 3d46  xtras, reverse=F
-00002630: 616c 7365 2029 3a0a 2020 2020 2020 2020  alse ):.        
-00002640: 2020 2020 666f 7220 7369 672c 206c 6963      for sig, lic
-00002650: 2069 6e20 656d 6974 2820 7072 6f76 2029   in emit( prov )
-00002660: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00002670: 2020 7969 656c 6420 7369 672c 206c 6963    yield sig, lic
-00002680: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002690: 2066 6f75 6e64 0920 2020 2020 2020 2b3d   found.       +=
-000026a0: 2031 0a20 2020 2065 7863 6570 7420 4578   1.    except Ex
-000026b0: 6365 7074 696f 6e20 6173 2065 7863 3a0a  ception as exc:.
-000026c0: 2020 2020 2020 2020 6c6f 672e 6572 726f          log.erro
-000026d0: 7228 2022 4661 696c 6564 2074 6f20 6c6f  r( "Failed to lo
-000026e0: 6164 206c 6963 656e 7365 2066 726f 6d20  ad license from 
-000026f0: 7b7d 3a20 7b7d 222e 666f 726d 6174 2820  {}: {}".format( 
-00002700: 7061 7468 206f 7220 5f5f 7061 636b 6167  path or __packag
-00002710: 655f 5f2c 2065 7863 2029 290a 2020 2020  e__, exc )).    
-00002720: 2020 2020 7061 7373 0a20 2020 206c 6f67      pass.    log
-00002730: 2e69 6e66 6f28 2022 4c69 6365 6e73 6573  .info( "Licenses
-00002740: 2020 2020 6c6f 6164 6564 3a20 7b7d 222e      loaded: {}".
-00002750: 666f 726d 6174 2820 666f 756e 6420 2929  format( found ))
-00002760: 0a0a 0a64 6566 2063 7265 6465 6e74 6961  ...def credentia
-00002770: 6c73 2820 2a61 6464 2029 3a0a 2020 2020  ls( *add ):.    
-00002780: 2222 224c 6f61 6420 616e 7920 6176 6169  """Load any avai
-00002790: 6c61 626c 6520 6372 6564 656e 7469 616c  lable credential
-000027a0: 732c 2061 6e64 2061 6464 2061 6e79 2070  s, and add any p
-000027b0: 6173 7365 6420 2864 6573 6372 6970 7469  assed (descripti
-000027c0: 6f6e 2c20 2875 7365 726e 616d 652c 2070  on, (username, p
-000027d0: 6173 7377 6f72 6429 292c 0a20 2020 202e  assword)),.    .
-000027e0: 2e2e 2063 6f6e 7461 696e 696e 6720 6e65  .. containing ne
-000027f0: 7720 6372 6564 656e 7469 616c 7320 7375  w credentials su
-00002800: 7070 6c69 6564 2062 7920 7468 6520 4c69  pplied by the Li
-00002810: 6365 6e73 6520 5365 7276 6572 2061 646d  cense Server adm
-00002820: 696e 6973 7472 6174 6f72 2064 7572 696e  inistrator durin
-00002830: 6720 6f70 6572 6174 696f 6e2e 0a0a 2020  g operation...  
-00002840: 2020 4561 6368 2054 6872 6561 6420 6f66    Each Thread of
-00002850: 2074 6869 7320 4c69 6365 6e73 6520 5365   this License Se
-00002860: 7276 6572 2074 6861 7420 6d75 7374 2064  rver that must d
-00002870: 6563 7279 7074 2065 6e63 7279 7074 6564  ecrypt encrypted
-00002880: 206b 6579 7320 7368 6f75 6c64 2075 7365   keys should use
-00002890: 2074 6865 7365 2063 7265 6465 6e74 6961   these credentia
-000028a0: 6c73 0a20 2020 2074 6f20 6163 6365 7373  ls.    to access
-000028b0: 2074 6865 206b 6579 732e 0a0a 2020 2020   the keys...    
-000028c0: 544f 444f 3a20 5368 6f75 6c64 2074 6869  TODO: Should thi
-000028d0: 7320 6265 2065 6e63 7279 7074 6564 2061  s be encrypted a
-000028e0: 742d 7265 7374 2064 7572 696e 6720 6f70  t-rest during op
-000028f0: 6572 6174 696f 6e3f 2020 4974 2063 6f75  eration?  It cou
-00002900: 6c64 2062 6520 696e 7370 6563 7465 6420  ld be inspected 
-00002910: 6279 2061 6e79 0a20 2020 2075 7365 722f  by any.    user/
-00002920: 726f 6f74 206c 6576 656c 2070 726f 6365  root level proce
-00002930: 7373 2c20 616e 6420 7573 6564 2074 6f20  ss, and used to 
-00002940: 756e 6c6f 636b 2074 6865 2065 6e63 7279  unlock the encry
-00002950: 7074 6564 2061 7574 686f 7220 7369 676e  pted author sign
-00002960: 696e 6720 6b65 7970 6169 7273 2e0a 0a20  ing keypairs... 
-00002970: 2020 2022 2222 0a20 2020 2079 6965 6c64     """.    yield
-00002980: 2022 284e 6f20 4372 6564 656e 7469 616c   "(No Credential
-00002990: 7329 222c 2028 4e6f 6e65 2c20 4e6f 6e65  s)", (None, None
-000029a0: 290a 0a20 2020 2063 7265 6465 6e74 6961  )..    credentia
-000029b0: 6c73 2e6c 6f63 616c 2e75 7064 6174 6528  ls.local.update(
-000029c0: 2061 6464 2029 0a20 2020 2066 6f72 206e   add ).    for n
-000029d0: 616d 652c 2028 7573 6572 6e61 6d65 2c20  ame, (username, 
-000029e0: 7061 7373 776f 7264 2920 696e 2063 7265  password) in cre
-000029f0: 6465 6e74 6961 6c73 2e6c 6f63 616c 2e69  dentials.local.i
-00002a00: 7465 6d73 2829 3a0a 2020 2020 2020 2020  tems():.        
-00002a10: 7969 656c 6420 6e61 6d65 2c20 2875 7365  yield name, (use
-00002a20: 726e 616d 652c 2070 6173 7377 6f72 6429  rname, password)
-00002a30: 0a20 2020 206c 6f67 2e69 6e66 6f28 2022  .    log.info( "
-00002a40: 4372 6564 656e 7469 616c 7320 6361 6368  Credentials cach
-00002a50: 6564 3a20 7b7d 222e 666f 726d 6174 2820  ed: {}".format( 
-00002a60: 6c65 6e28 2063 7265 6465 6e74 6961 6c73  len( credentials
-00002a70: 2e6c 6f63 616c 2029 2929 0a0a 2020 2020  .local )))..    
-00002a80: 666f 756e 6409 0909 3d20 300a 2020 2020  found...= 0.    
-00002a90: 7061 7468 0909 093d 204e 6f6e 650a 2020  path...= None.  
-00002aa0: 2020 7472 793a 0a20 2020 2020 2020 2023    try:.        #
-00002ab0: 204f 7065 6e20 616e 7920 6c69 6365 6e73   Open any licens
-00002ac0: 696e 672e 6372 6564 656e 7469 616c 732a  ing.credentials*
-00002ad0: 2069 6e20 636f 6e66 6967 7572 6174 696f   in configuratio
-00002ae0: 6e20 7061 7468 2e20 2057 6520 7761 6e74  n path.  We want
-00002af0: 2074 6f20 6c6f 6164 206d 6f73 740a 2020   to load most.  
-00002b00: 2020 2020 2020 2320 6765 6e65 7261 6c2f        # general/
-00002b10: 6469 7374 616e 7420 6669 6c65 7320 6669  distant files fi
-00002b20: 7273 7420 736f 206d 616b 6520 7265 7665  rst so make reve
-00002b30: 7273 653d 5472 7565 2e0a 2020 2020 2020  rse=True..      
-00002b40: 2020 676c 6f62 616c 2063 6f6e 6669 675f    global config_
-00002b50: 6578 7472 6173 0a20 2020 2020 2020 2066  extras.        f
-00002b60: 6f72 2066 2069 6e20 636f 6e66 6967 5f6f  or f in config_o
-00002b70: 7065 6e28 2043 5244 4649 4c45 2b27 2a27  pen( CRDFILE+'*'
-00002b80: 2c20 6578 7472 613d 636f 6e66 6967 5f65  , extra=config_e
-00002b90: 7874 7261 732c 2073 6b69 703d 272a 7e27  xtras, skip='*~'
-00002ba0: 2c20 7265 7665 7273 653d 4661 6c73 6520  , reverse=False 
-00002bb0: 293a 0a20 2020 2020 2020 2020 2020 2077  ):.            w
-00002bc0: 6974 6820 663a 0a20 2020 2020 2020 2020  ith f:.         
-00002bd0: 2020 2020 2020 2023 2045 6163 6820 6c69         # Each li
-00002be0: 6365 6e73 696e 672e 6372 6564 656e 7469  censing.credenti
-00002bf0: 616c 732a 2066 696c 6520 7368 6f75 6c64  als* file should
-00002c00: 2062 6520 6120 7365 7175 656e 6365 206f   be a sequence o
-00002c10: 663a 0a20 2020 2020 2020 2020 2020 2020  f:.             
-00002c20: 2020 2023 2020 2020 205b 2028 2022 6465     #     [ ( "de
-00002c30: 7363 7269 7074 696f 6e22 2c20 5b20 2275  scription", [ "u
-00002c40: 7365 726e 616d 6522 3a20 2270 6173 7377  sername": "passw
-00002c50: 6f72 6422 205d 2029 2c20 2e2e 2e20 5d0a  ord" ] ), ... ].
-00002c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c70: 2320 736f 2063 6f6e 7665 7274 2061 2064  # so convert a d
-00002c80: 6963 7420 696e 746f 2073 7563 6820 6120  ict into such a 
-00002c90: 7365 7175 656e 6365 2e20 2048 6f77 6576  sequence.  Howev
-00002ca0: 6572 2c20 7265 7665 7273 6520 7468 6520  er, reverse the 
-00002cb0: 2e75 7064 6174 6520 736f 206d 6f72 650a  .update so more.
-00002cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002cd0: 2320 6561 726c 6965 7220 286d 6f72 6520  # earlier (more 
-00002ce0: 7370 6563 6966 6963 2920 636f 6e66 6967  specific) config
-00002cf0: 7572 6174 696f 6e73 2061 7265 206e 6f74  urations are not
-00002d00: 206f 7665 7272 6964 656e 2062 7920 6c61   overriden by la
-00002d10: 7465 7220 286d 6f72 6520 6765 6e65 7261  ter (more genera
-00002d20: 6c29 0a20 2020 2020 2020 2020 2020 2020  l).             
-00002d30: 2020 2023 206f 6e65 732e 0a20 2020 2020     # ones..     
-00002d40: 2020 2020 2020 2020 2020 2070 6174 6809             path.
-00002d50: 093d 2066 2e6e 616d 650a 2020 2020 2020  .= f.name.      
-00002d60: 2020 2020 2020 2020 2020 6372 6564 7309            creds.
-00002d70: 093d 206a 736f 6e2e 6c6f 6164 7328 2066  .= json.loads( f
-00002d80: 2e72 6561 6428 2920 290a 2020 2020 2020  .read() ).      
-00002d90: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
-00002da0: 6e63 6528 2063 7265 6473 2c20 6469 6374  nce( creds, dict
-00002db0: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
-00002dc0: 2020 2020 6372 6564 7309 093d 2063 7265      creds..= cre
-00002dd0: 6473 2e69 7465 6d73 2829 0a20 2020 2020  ds.items().     
-00002de0: 2020 2020 2020 2066 6f72 206e 616d 652c         for name,
-00002df0: 2028 7573 6572 6e61 6d65 2c20 7061 7373   (username, pass
-00002e00: 776f 7264 2920 696e 2063 7265 6473 3a0a  word) in creds:.
-00002e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e20: 6c6f 672e 696e 666f 2820 2220 207b 6e3a  log.info( "  {n:
-00002e30: 3c32 307d 3a20 7b75 3a3e 3230 7d20 2f20  <20}: {u:>20} / 
-00002e40: 7b70 7d22 2e66 6f72 6d61 7428 206e 3d6e  {p}".format( n=n
-00002e50: 616d 652c 2075 3d75 7365 726e 616d 652c  ame, u=username,
-00002e60: 2070 3d27 2a27 202a 206c 656e 2820 7061   p='*' * len( pa
-00002e70: 7373 776f 7264 2029 2929 0a20 2020 2020  ssword ))).     
-00002e80: 2020 2020 2020 2020 2020 2079 6965 6c64             yield
-00002e90: 206e 616d 652c 2028 7573 6572 6e61 6d65   name, (username
-00002ea0: 2c20 7061 7373 776f 7264 290a 2020 2020  , password).    
-00002eb0: 2020 2020 2020 2020 2020 2020 666f 756e              foun
-00002ec0: 6409 2020 2020 2020 202b 3d20 310a 2020  d.       += 1.  
-00002ed0: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
-00002ee0: 6f6e 2061 7320 6578 633a 0a20 2020 2020  on as exc:.     
-00002ef0: 2020 206c 6f67 2e65 7272 6f72 2820 2246     log.error( "F
-00002f00: 6169 6c65 6420 746f 206c 6f61 6420 7b7d  ailed to load {}
-00002f10: 2a3a 207b 7d22 2e66 6f72 6d61 7428 2070  *: {}".format( p
-00002f20: 6174 6820 6f72 2043 5244 4649 4c45 2c20  ath or CRDFILE, 
-00002f30: 6578 6320 2929 0a20 2020 2020 2020 2070  exc )).        p
-00002f40: 6173 730a 2020 2020 6c6f 672e 696e 666f  ass.    log.info
-00002f50: 2820 2243 7265 6465 6e74 6961 6c73 206c  ( "Credentials l
-00002f60: 6f61 6465 643a 207b 7d22 2e66 6f72 6d61  oaded: {}".forma
-00002f70: 7428 2066 6f75 6e64 2029 290a 0a0a 6372  t( found ))...cr
-00002f80: 6564 656e 7469 616c 732e 6c6f 6361 6c09  edentials.local.
-00002f90: 093d 207b 7d20 2023 207b 2064 6573 6372  .= {}  # { descr
-00002fa0: 6970 7469 6f6e 3a20 2875 7365 726e 616d  iption: (usernam
-00002fb0: 652c 2070 6173 7377 6f72 6429 2c20 2e2e  e, password), ..
-00002fc0: 2e20 7d0a 0a0a 6465 6620 6b65 7970 6169  . }...def keypai
-00002fd0: 7273 2829 3a0a 2020 2020 2222 224c 6f61  rs():.    """Loa
-00002fe0: 6420 616c 6c20 6176 6169 6c61 626c 6520  d all available 
-00002ff0: 6b65 7970 6169 7273 2061 7661 696c 6162  keypairs availab
-00003000: 6c65 2066 6f72 2061 7574 686f 7269 6e67  le for authoring
-00003010: 204c 6963 656e 7365 732c 2075 7369 6e67   Licenses, using
-00003020: 2061 6c6c 2063 7572 7265 6e74 6c79 2061   all currently a
-00003030: 7661 696c 6162 6c65 0a20 2020 2063 7265  vailable.    cre
-00003040: 6465 6e74 6961 6c73 2e20 2054 6869 7320  dentials.  This 
-00003050: 696e 636c 7564 6573 2061 6c6c 2045 6e63  includes all Enc
-00003060: 7279 7074 6564 2061 6e64 2050 6c61 696e  rypted and Plain
-00003070: 7465 7874 206b 6579 7320 696e 2066 696c  text keys in fil
-00003080: 6573 2c20 616e 6420 616c 6c20 456e 6372  es, and all Encr
-00003090: 7970 7465 6420 6b65 7973 2069 6e0a 2020  ypted keys in.  
-000030a0: 2020 6461 7461 6261 7365 2022 6175 7468    database "auth
-000030b0: 6f72 7322 2074 6162 6c65 2e20 2045 6163  ors" table.  Eac
-000030c0: 6820 7469 6d65 2077 6520 6164 6420 6120  h time we add a 
-000030d0: 6e65 7720 6372 6564 656e 7469 616c 2c20  new credential, 
-000030e0: 7468 6973 202a 6d61 792a 206d 616b 6520  this *may* make 
-000030f0: 6176 6169 6c61 626c 6520 6d6f 7265 0a20  available more. 
-00003100: 2020 206b 6579 7320 656e 6372 7970 7465     keys encrypte
-00003110: 6420 7769 7468 2074 686f 7365 2063 7265  d with those cre
-00003120: 6465 6e74 6961 6c73 2e0a 0a20 2020 2059  dentials...    Y
-00003130: 6965 6c64 2073 6571 7565 6e63 6520 6f66  ield sequence of
-00003140: 2061 6c6c 2061 7661 696c 6162 6c65 2028   all available (
-00003150: 6e61 6d65 2c20 2e2e 2e4b 6579 7061 6972  name, ...Keypair
-00003160: 2c20 6372 6564 656e 7469 616c 2920 6672  , credential) fr
-00003170: 6f6d 2022 6175 7468 6f72 7322 2074 6162  om "authors" tab
-00003180: 6c65 2061 6e64 2066 696c 6573 2e0a 2020  le and files..  
-00003190: 2020 4d61 7920 636f 6e74 6169 6e20 6475    May contain du
-000031a0: 706c 6963 6174 6573 2e20 2043 616c 6c65  plicates.  Calle
-000031b0: 7220 6d61 7920 6163 6375 6d75 6c61 7465  r may accumulate
-000031c0: 2074 6865 6d2c 206f 7220 7369 6d70 6c79   them, or simply
-000031d0: 2073 6361 6e20 666f 7220 6465 7369 7265   scan for desire
-000031e0: 6420 656e 7472 792e 0a0a 2020 2020 2222  d entry...    ""
-000031f0: 220a 2020 2020 6c6f 6164 6564 0909 093d  ".    loaded...=
-00003200: 2073 6574 2829 0a20 2020 2073 6176 6564   set().    saved
-00003210: 0909 093d 2030 0a20 2020 2066 6f72 2063  ...= 0.    for c
-00003220: 7265 646e 616d 652c 2875 7365 726e 616d  redname,(usernam
-00003230: 652c 7061 7373 776f 7264 2920 696e 2063  e,password) in c
-00003240: 7265 6465 6e74 6961 6c73 2829 3a0a 2020  redentials():.  
-00003250: 2020 2020 2020 6c6f 672e 696e 666f 2820        log.info( 
-00003260: 224b 6579 7061 6972 7320 666f 7220 7b7d  "Keypairs for {}
-00003270: 2773 2063 7265 6465 6e74 6961 6c3a 222e  's credential:".
-00003280: 666f 726d 6174 2820 7573 6572 6e61 6d65  format( username
-00003290: 2029 290a 2020 2020 2020 2020 666f 7220   )).        for 
-000032a0: 7220 696e 2064 622e 7365 6c65 6374 2820  r in db.select( 
-000032b0: 2761 7574 686f 7273 2720 293a 0a20 2020  'authors' ):.   
-000032c0: 2020 2020 2020 2020 2063 7265 6409 093d           cred..=
-000032d0: 2064 6963 7428 2075 7365 726e 616d 653d   dict( username=
-000032e0: 7573 6572 6e61 6d65 2c20 7061 7373 776f  username, passwo
-000032f0: 7264 3d70 6173 7377 6f72 6420 290a 2020  rd=password ).  
-00003300: 2020 2020 2020 2020 2020 7472 793a 0a20            try:. 
-00003310: 2020 2020 2020 2020 2020 2020 2020 206b                 k
-00003320: 6579 7061 6972 0909 3d20 6c69 6365 6e73  eypair..= licens
-00003330: 696e 672e 4b65 7970 6169 7245 6e63 7279  ing.KeypairEncry
-00003340: 7074 6564 2820 6369 7068 6572 7465 7874  pted( ciphertext
-00003350: 3d72 2e63 6970 6865 7274 6578 742c 2073  =r.ciphertext, s
-00003360: 616c 743d 722e 7361 6c74 2029 0a20 2020  alt=r.salt ).   
-00003370: 2020 2020 2020 2020 2020 2020 206b 6579               key
-00003380: 7061 6972 2e69 6e74 6f5f 6b65 7970 6169  pair.into_keypai
-00003390: 7228 202a 2a63 7265 6420 2920 2023 2045  r( **cred )  # E
-000033a0: 6e73 7572 6520 7468 6520 7375 7070 6c69  nsure the suppli
-000033b0: 6564 2063 7265 6465 6e74 6961 6c73 2063  ed credentials c
-000033c0: 616e 2064 6563 7279 7074 2069 740a 2020  an decrypt it.  
-000033d0: 2020 2020 2020 2020 2020 2020 2020 7969                yi
-000033e0: 656c 6420 722e 6e61 6d65 2c20 6b65 7970  eld r.name, keyp
-000033f0: 6169 722c 2063 7265 640a 2020 2020 2020  air, cred.      
-00003400: 2020 2020 2020 2020 2020 7361 7665 6409            saved.
-00003410: 2020 2020 2020 202b 3d20 310a 2020 2020         += 1.    
-00003420: 2020 2020 2020 2020 6578 6365 7074 2045          except E
-00003430: 7863 6570 7469 6f6e 2061 7320 6578 633a  xception as exc:
-00003440: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003450: 2023 204d 6f73 7420 6b65 7970 6169 7273   # Most keypairs
-00003460: 2077 696c 6c20 6661 696c 2074 6f20 6465   will fail to de
-00003470: 6372 7970 7420 7769 7468 206d 6f73 7420  crypt with most 
-00003480: 6372 6564 656e 7469 616c 732e 2e2e 0a20  credentials.... 
-00003490: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-000034a0: 6f67 2e64 6562 7567 2820 227b 6e3a 3c32  og.debug( "{n:<2
-000034b0: 307d 3a20 4661 696c 6564 2074 6f20 6465  0}: Failed to de
-000034c0: 6372 7970 7420 772f 207b 753a 3e32 307d  crypt w/ {u:>20}
-000034d0: 202f 207b 707d 3a20 7b65 7863 7d22 2e66   / {p}: {exc}".f
-000034e0: 6f72 6d61 7428 0a20 2020 2020 2020 2020  ormat(.         
-000034f0: 2020 2020 2020 2020 2020 206e 3d72 2e6e             n=r.n
-00003500: 616d 652c 2075 3d63 7265 645b 2775 7365  ame, u=cred['use
-00003510: 726e 616d 6527 5d20 6f72 2027 2865 6d70  rname'] or '(emp
-00003520: 7479 2927 2c20 703d 272a 2720 2a20 6c65  ty)', p='*' * le
-00003530: 6e28 2063 7265 645b 2770 6173 7377 6f72  n( cred['passwor
-00003540: 6427 5d20 6f72 2027 2865 6d70 7479 2927  d'] or '(empty)'
-00003550: 2029 2c0a 2020 2020 2020 2020 2020 2020   ),.            
-00003560: 2020 2020 2020 2020 6578 633d 6578 6320          exc=exc 
-00003570: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
-00003580: 2020 2070 6173 730a 2020 2020 2020 2020     pass.        
-00003590: 2320 416e 7920 506c 6169 6e74 6578 7420  # Any Plaintext 
-000035a0: 4b65 7970 6169 7273 2028 616e 6420 7065  Keypairs (and pe
-000035b0: 7268 6170 7320 736f 6d65 2045 6e63 7279  rhaps some Encry
-000035c0: 7074 6564 206f 6e65 732c 2069 6620 6475  pted ones, if du
-000035d0: 706c 6963 6174 6520 6372 6564 656e 7469  plicate credenti
-000035e0: 616c 7320 6172 650a 2020 2020 2020 2020  als are.        
-000035f0: 2320 7375 7070 6c69 6564 2920 7769 6c6c  # supplied) will
-00003600: 2062 6520 666f 756e 6420 6d75 6c74 6970   be found multip
-00003610: 6c65 2074 696d 6573 2e20 2052 6570 6f72  le times.  Repor
-00003620: 7420 6b65 7970 6169 7273 2061 7420 7468  t keypairs at th
-00003630: 6520 7361 6d65 2070 6174 6820 6f6e 6c79  e same path only
-00003640: 206f 6e63 652e 2020 5765 0a20 2020 2020   once.  We.     
-00003650: 2020 2023 2077 616e 7420 746f 206c 6f61     # want to loa
-00003660: 6420 7468 6520 6d6f 7374 2067 656e 6572  d the most gener
-00003670: 616c 2f64 6973 7461 6e74 206b 6579 7320  al/distant keys 
-00003680: 6669 7273 742c 2073 6f20 7265 7665 7273  first, so revers
-00003690: 653d 4661 6c73 652e 0a20 2020 2020 2020  e=False..       
-000036a0: 2070 6174 6809 0909 3d20 4e6f 6e65 0a20   path...= None. 
-000036b0: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
-000036c0: 2020 2020 2020 2020 676c 6f62 616c 2063          global c
-000036d0: 6f6e 6669 675f 6578 7472 6173 0a20 2020  onfig_extras.   
-000036e0: 2020 2020 2020 2020 2066 6f72 2070 6174           for pat
-000036f0: 682c 206b 6579 7061 6972 2c20 6372 6564  h, keypair, cred
-00003700: 2069 6e20 6c69 6365 6e73 696e 672e 6c6f   in licensing.lo
-00003710: 6164 5f6b 6579 7328 0a20 2020 2020 2020  ad_keys(.       
-00003720: 2020 2020 2020 2020 2020 2020 2070 6163               pac
-00003730: 6b61 6765 3d5f 5f70 6163 6b61 6765 5f5f  kage=__package__
-00003740: 2c20 7573 6572 6e61 6d65 3d75 7365 726e  , username=usern
-00003750: 616d 652c 2070 6173 7377 6f72 643d 7061  ame, password=pa
-00003760: 7373 776f 7264 2c0a 2020 2020 2020 2020  ssword,.        
-00003770: 2020 2020 2020 2020 2020 2020 6578 7472              extr
-00003780: 613d 636f 6e66 6967 5f65 7874 7261 732c  a=config_extras,
-00003790: 2072 6576 6572 7365 3d46 616c 7365 2029   reverse=False )
-000037a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000037b0: 2020 6966 2070 6174 6820 6e6f 7420 696e    if path not in
-000037c0: 206c 6f61 6465 643a 0a20 2020 2020 2020   loaded:.       
-000037d0: 2020 2020 2020 2020 2020 2020 2079 6965               yie
-000037e0: 6c64 2070 6174 682c 206b 6579 7061 6972  ld path, keypair
-000037f0: 2c20 6372 6564 0a20 2020 2020 2020 2020  , cred.         
-00003800: 2020 2020 2020 2020 2020 206c 6f61 6465             loade
-00003810: 642e 6164 6428 2070 6174 6820 290a 2020  d.add( path ).  
-00003820: 2020 2020 2020 6578 6365 7074 2045 7863        except Exc
-00003830: 6570 7469 6f6e 2061 7320 6578 633a 0a20  eption as exc:. 
-00003840: 2020 2020 2020 2020 2020 206c 6f67 2e65             log.e
-00003850: 7272 6f72 2820 2246 6169 6c65 6420 746f  rror( "Failed to
-00003860: 206c 6f61 6420 6b65 7970 6169 7220 6672   load keypair fr
-00003870: 6f6d 207b 7d3a 207b 7d22 2e66 6f72 6d61  om {}: {}".forma
-00003880: 7428 2070 6174 6820 6f72 205f 5f70 6163  t( path or __pac
-00003890: 6b61 6765 5f5f 2c20 6578 6320 2929 0a20  kage__, exc )). 
-000038a0: 2020 2020 2020 2020 2020 2070 6173 730a             pass.
-000038b0: 2020 2020 6c6f 672e 696e 666f 2820 224b      log.info( "K
-000038c0: 6579 7061 6972 7320 2020 2020 7361 7665  eypairs     save
-000038d0: 643a 207b 7d22 2e66 6f72 6d61 7428 2073  d: {}".format( s
-000038e0: 6176 6564 2029 290a 2020 2020 6c6f 672e  aved )).    log.
-000038f0: 696e 666f 2820 224b 6579 7061 6972 7320  info( "Keypairs 
-00003900: 2020 206c 6f61 6465 643a 207b 7d22 2e66     loaded: {}".f
-00003910: 6f72 6d61 7428 206c 656e 2820 6c6f 6164  ormat( len( load
-00003920: 6564 2029 2929 0a0a 0a64 6566 206c 6963  ed )))...def lic
-00003930: 656e 7365 735f 6461 7461 2820 7061 7468  enses_data( path
-00003940: 2c20 7374 6f72 6564 3d4e 6f6e 652c 2063  , stored=None, c
-00003950: 6f6e 6669 726d 3d4e 6f6e 652c 2061 7574  onfirm=None, aut
-00003960: 686f 723d 4e6f 6e65 2c20 636c 6965 6e74  hor=None, client
-00003970: 3d4e 6f6e 652c 2070 726f 6475 6374 3d4e  =None, product=N
-00003980: 6f6e 6520 293a 0a20 2020 2022 2222 5265  one ):.    """Re
-00003990: 7475 726e 7320 616c 6c20 6669 6c74 6572  turns all filter
-000039a0: 6564 206c 6963 656e 7365 7320 6173 2064  ed licenses as d
-000039b0: 6174 615b 276c 6973 7427 5d20 7265 636f  ata['list'] reco
-000039c0: 7264 732c 206d 6179 6265 2077 2f20 636f  rds, maybe w/ co
-000039d0: 6e66 6972 6d20 6f66 2044 4b49 4d2c 2066  nfirm of DKIM, f
-000039e0: 696c 7465 7265 6420 6279 0a20 2020 2061  iltered by.    a
-000039f0: 7574 686f 7220 2f20 636c 6965 6e74 2028  uthor / client (
-00003a00: 6d61 7962 6520 7061 7373 6564 2076 6961  maybe passed via
-00003a10: 2070 6174 6829 2e20 2046 6f72 2065 7861   path).  For exa
-00003a20: 6d70 6c65 2c0a 0a20 2020 2020 2020 206c  mple,..        l
-00003a30: 6963 656e 7365 732f 446f 6d2a 2f41 7765  icenses/Dom*/Awe
-00003a40: 736f 6d65 2a20 2020 2d2d 3e20 2041 6c6c  some*   -->  All
-00003a50: 2044 6f6d 696e 696f 6e20 5226 4420 436f   Dominion R&D Co
-00003a60: 7270 2e20 6175 7468 6f72 6564 204c 6963  rp. authored Lic
-00003a70: 656e 7365 7320 746f 2041 7765 736f 6d65  enses to Awesome
-00003a80: 2c20 496e 632e 0a0a 2020 2020 5468 6520  , Inc...    The 
-00003a90: 7361 6d65 2072 6573 756c 7420 776f 756c  same result woul
-00003aa0: 6420 6265 2072 6561 6368 6564 2069 6620  d be reached if 
-00003ab0: 6c69 6365 7365 733f 6175 7468 6f72 3d44  liceses?author=D
-00003ac0: 6f6d 2a26 636c 6965 6e74 3d41 7765 2a2e  om*&client=Awe*.
-00003ad0: 0a0a 2020 2020 2222 220a 2020 2020 6461  ..    """.    da
-00003ae0: 7461 0909 093d 207b 7d0a 2020 2020 6461  ta...= {}.    da
-00003af0: 7461 5b22 7469 746c 6522 5d09 093d 2022  ta["title"]..= "
-00003b00: 4c69 6365 6e73 6573 220a 2020 2020 6461  Licenses".    da
-00003b10: 7461 5b22 7061 7468 225d 0909 3d20 7061  ta["path"]..= pa
-00003b20: 7468 0a20 2020 2064 6174 615b 226c 6973  th.    data["lis
-00003b30: 7422 5d20 3d20 6c6c 0909 3d20 5b5d 0a20  t"] = ll..= []. 
-00003b40: 2020 2064 6174 615b 226b 6579 7322 5d09     data["keys"].
-00003b50: 093d 205b 2261 7574 686f 7222 2c20 2263  .= ["author", "c
-00003b60: 6c69 656e 7422 2c20 2270 726f 6475 6374  lient", "product
-00003b70: 222c 2022 7369 676e 6174 7572 6522 2c20  ", "signature", 
-00003b80: 2263 6f6e 6669 726d 222c 2022 6c69 6365  "confirm", "lice
-00003b90: 6e73 6522 5d0a 0a20 2020 2070 6174 6873  nse"]..    paths
-00003ba0: 6567 7309 0909 3d20 7061 7468 2e73 7472  egs...= path.str
-00003bb0: 6970 2827 2f27 292e 7370 6c69 7428 272f  ip('/').split('/
-00003bc0: 2729 2069 6620 7061 7468 2065 6c73 6520  ') if path else 
-00003bd0: 5b5d 0a20 2020 2061 7373 6572 7420 3020  [].    assert 0 
-00003be0: 3c3d 206c 656e 2820 7061 7468 7365 6773  <= len( pathsegs
-00003bf0: 2029 203c 3d20 322c 205c 0a20 2020 2020   ) <= 2, \.     
-00003c00: 2020 2022 496e 7661 6c69 6420 6c69 6365     "Invalid lice
-00003c10: 6e73 6573 2067 6c6f 6220 7061 7468 207b  nses glob path {
-00003c20: 7d3b 206c 6963 656e 7365 732f 3c61 7574  }; licenses/<aut
-00003c30: 686f 723e 2f3c 636c 6965 6e74 3e2f 3c70  hor>/<client>/<p
-00003c40: 726f 6475 6374 3e22 2e66 6f72 6d61 7428  roduct>".format(
-00003c50: 2070 6174 6820 290a 0a20 2020 2023 2049   path )..    # I
-00003c60: 7465 7261 7465 2061 6c6c 2061 7661 696c  terate all avail
-00003c70: 6162 6c65 206c 6963 656e 7365 732c 2066  able licenses, f
-00003c80: 696c 7465 7269 6e67 2069 6620 6164 6469  iltering if addi
-00003c90: 7469 6f6e 616c 206c 6963 656e 7365 2061  tional license a
-00003ca0: 7574 686f 7220 6e61 6d65 2070 6174 6820  uthor name path 
-00003cb0: 636f 6d70 6f6e 656e 7420 7375 7070 6c69  component suppli
-00003cc0: 6564 0a20 2020 2066 6f72 2073 6967 6e61  ed.    for signa
-00003cd0: 7475 7265 2c20 6c69 6320 696e 206c 6963  ture, lic in lic
-00003ce0: 656e 7365 7328 2063 6f6e 6669 726d 3d46  enses( confirm=F
-00003cf0: 616c 7365 2c20 7374 6f72 6564 3d73 746f  alse, stored=sto
-00003d00: 7265 6420 293a 0a20 2020 2020 2020 2072  red ):.        r
-00003d10: 6563 6f72 6409 0909 3d20 6469 6374 280a  ecord...= dict(.
-00003d20: 2020 2020 2020 2020 2020 2020 6175 7468              auth
-00003d30: 6f72 0909 3d20 6c69 635b 2761 7574 686f  or..= lic['autho
-00003d40: 7227 5d5b 276e 616d 6527 5d2c 0a20 2020  r']['name'],.   
-00003d50: 2020 2020 2020 2020 2063 6c69 656e 7409           client.
-00003d60: 093d 206c 6963 5b27 636c 6965 6e74 275d  .= lic['client']
-00003d70: 5b27 6e61 6d65 275d 2c0a 2020 2020 2020  ['name'],.      
-00003d80: 2020 2020 2020 7072 6f64 7563 7409 093d        product..=
-00003d90: 206c 6963 5b27 6175 7468 6f72 275d 5b27   lic['author']['
-00003da0: 7072 6f64 7563 7427 5d2c 0a20 2020 2020  product'],.     
-00003db0: 2020 2020 2020 2073 6967 6e61 7475 7265         signature
-00003dc0: 0909 3d20 6c69 6365 6e73 696e 672e 696e  ..= licensing.in
-00003dd0: 746f 5f62 3634 2820 7369 676e 6174 7572  to_b64( signatur
-00003de0: 6520 292c 0a20 2020 2020 2020 2020 2020  e ),.           
-00003df0: 2063 6f6e 6669 726d 0909 3d20 4e6f 6e65   confirm..= None
-00003e00: 2c0a 2020 2020 2020 2020 2020 2020 6c69  ,.            li
-00003e10: 6365 6e73 6509 093d 2073 7472 2820 6c69  cense..= str( li
-00003e20: 6320 292c 0a20 2020 2020 2020 2029 0a20  c ),.        ). 
-00003e30: 2020 2020 2020 2061 7574 686f 7209 0909         author...
-00003e40: 3d20 6175 7468 6f72 206f 7220 6c65 6e28  = author or len(
-00003e50: 2070 6174 6873 6567 7320 2920 3e20 3020   pathsegs ) > 0 
-00003e60: 616e 6420 7061 7468 7365 6773 5b30 5d0a  and pathsegs[0].
-00003e70: 2020 2020 2020 2020 6966 2061 7574 686f          if autho
-00003e80: 7220 616e 6420 6e6f 7420 666e 6d61 7463  r and not fnmatc
-00003e90: 682e 666e 6d61 7463 6828 2072 6563 6f72  h.fnmatch( recor
-00003ea0: 645b 2761 7574 686f 7227 5d2c 2061 7574  d['author'], aut
-00003eb0: 686f 7220 293a 0a20 2020 2020 2020 2020  hor ):.         
-00003ec0: 2020 2063 6f6e 7469 6e75 650a 2020 2020     continue.    
-00003ed0: 2020 2020 636c 6965 6e74 0909 093d 2063      client...= c
-00003ee0: 6c69 656e 7420 6f72 206c 656e 2820 7061  lient or len( pa
-00003ef0: 7468 7365 6773 2029 203e 2031 2061 6e64  thsegs ) > 1 and
-00003f00: 2070 6174 6873 6567 735b 315d 0a20 2020   pathsegs[1].   
-00003f10: 2020 2020 2069 6620 636c 6965 6e74 2061       if client a
-00003f20: 6e64 206e 6f74 2066 6e6d 6174 6368 2e66  nd not fnmatch.f
-00003f30: 6e6d 6174 6368 2820 7265 636f 7264 5b27  nmatch( record['
-00003f40: 636c 6965 6e74 275d 2c20 636c 6965 6e74  client'], client
-00003f50: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
-00003f60: 636f 6e74 696e 7565 0a20 2020 2020 2020  continue.       
-00003f70: 2070 726f 6475 6374 0909 093d 2070 726f   product...= pro
-00003f80: 6475 6374 206f 7220 6c65 6e28 2070 6174  duct or len( pat
-00003f90: 6873 6567 7320 2920 3e20 3220 616e 6420  hsegs ) > 2 and 
-00003fa0: 7061 7468 7365 6773 5b32 5d0a 2020 2020  pathsegs[2].    
-00003fb0: 2020 2020 6966 2070 726f 6475 6374 2061      if product a
-00003fc0: 6e64 206e 6f74 2066 6e6d 6174 6368 2e66  nd not fnmatch.f
-00003fd0: 6e6d 6174 6368 2820 7265 636f 7264 5b27  nmatch( record['
-00003fe0: 7072 6f64 7563 7427 5d2c 2070 726f 6475  product'], produ
-00003ff0: 6374 2029 3a0a 2020 2020 2020 2020 2020  ct ):.          
-00004000: 2020 636f 6e74 696e 7565 0a20 2020 2020    continue.     
-00004010: 2020 2023 2041 6674 6572 2066 696c 7465     # After filte
-00004020: 7269 6e67 206f 7574 2075 6e69 6e74 6572  ring out uninter
-00004030: 6573 7469 6e67 204c 6963 656e 7365 732c  esting Licenses,
-00004040: 2063 6f6e 6669 726d 2069 6620 6465 7369   confirm if desi
-00004050: 7265 640a 2020 2020 2020 2020 6966 2063  red.        if c
-00004060: 6f6e 6669 726d 3a0a 2020 2020 2020 2020  onfirm:.        
-00004070: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-00004080: 2020 2020 2020 2020 206c 6963 2e76 6572           lic.ver
-00004090: 6966 7928 2063 6f6e 6669 726d 3d63 6f6e  ify( confirm=con
-000040a0: 6669 726d 2029 0a20 2020 2020 2020 2020  firm ).         
-000040b0: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
-000040c0: 696f 6e20 6173 2065 7863 3a0a 2020 2020  ion as exc:.    
-000040d0: 2020 2020 2020 2020 2020 2020 7265 636f              reco
-000040e0: 7264 2e75 7064 6174 6528 2063 6f6e 6669  rd.update( confi
-000040f0: 726d 3d73 7472 2820 6578 6320 2929 0a20  rm=str( exc )). 
-00004100: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00004110: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004120: 2072 6563 6f72 642e 7570 6461 7465 2820   record.update( 
-00004130: 636f 6e66 6972 6d3d 5472 7565 2029 0a20  confirm=True ). 
-00004140: 2020 2020 2020 206c 6c2e 6170 7065 6e64         ll.append
-00004150: 2820 7265 636f 7264 2029 0a0a 2020 2020  ( record )..    
-00004160: 7265 7475 726e 2064 6174 610a 0a0a 6465  return data...de
-00004170: 6620 6372 6564 656e 7469 616c 735f 6461  f credentials_da
-00004180: 7461 2820 7061 7468 2029 3a0a 2020 2020  ta( path ):.    
-00004190: 6461 7461 0909 093d 207b 7d0a 2020 2020  data...= {}.    
-000041a0: 6461 7461 5b22 7469 746c 6522 5d09 093d  data["title"]..=
-000041b0: 2022 4372 6564 656e 7469 616c 7322 0a20   "Credentials". 
-000041c0: 2020 2064 6174 615b 2270 6174 6822 5d09     data["path"].
-000041d0: 093d 2070 6174 680a 2020 2020 6461 7461  .= path.    data
-000041e0: 5b22 6c69 7374 225d 203d 206c 6c09 093d  ["list"] = ll..=
-000041f0: 205b 5d0a 2020 2020 6461 7461 5b22 6b65   [].    data["ke
-00004200: 7973 225d 0909 3d20 5b22 6e61 6d65 222c  ys"]..= ["name",
-00004210: 2022 7573 6572 6e61 6d65 222c 2022 7061   "username", "pa
-00004220: 7373 776f 7264 225d 0a0a 2020 2020 7061  ssword"]..    pa
-00004230: 7468 7365 6773 0909 093d 2070 6174 682e  thsegs...= path.
-00004240: 7374 7269 7028 272f 2729 2e73 706c 6974  strip('/').split
-00004250: 2827 2f27 2920 6966 2070 6174 6820 656c  ('/') if path el
-00004260: 7365 205b 5d0a 2020 2020 6173 7365 7274  se [].    assert
-00004270: 2030 203c 3d20 6c65 6e28 2070 6174 6873   0 <= len( paths
-00004280: 6567 7320 2920 3c3d 2031 2c20 2249 6e76  egs ) <= 1, "Inv
-00004290: 616c 6964 2063 7265 6465 6e74 6961 6c73  alid credentials
-000042a0: 2070 6174 6820 7b7d 222e 666f 726d 6174   path {}".format
-000042b0: 2820 7061 7468 2029 0a0a 2020 2020 666f  ( path )..    fo
-000042c0: 7220 6e61 6d65 2c28 7573 6572 6e61 6d65  r name,(username
-000042d0: 2c70 6173 7377 6f72 6429 2069 6e20 6372  ,password) in cr
-000042e0: 6564 656e 7469 616c 7328 293a 0a20 2020  edentials():.   
-000042f0: 2020 2020 2069 6620 7061 7468 7365 6773       if pathsegs
-00004300: 2061 6e64 2070 6174 6873 6567 735b 305d   and pathsegs[0]
-00004310: 2061 6e64 206e 6f74 2066 6e6d 6174 6368   and not fnmatch
-00004320: 2e66 6e6d 6174 6368 2820 6e61 6d65 2c20  .fnmatch( name, 
-00004330: 7061 7468 7365 6773 5b30 5d20 293a 0a20  pathsegs[0] ):. 
-00004340: 2020 2020 2020 2020 2020 206c 6f67 2e69             log.i
-00004350: 6e66 6f28 2022 4372 6564 656e 7469 616c  nfo( "Credential
-00004360: 207b 7d20 6469 646e 2774 206d 6174 6368   {} didn't match
-00004370: 207b 7d22 2e66 6f72 6d61 7428 206e 616d   {}".format( nam
-00004380: 652c 2070 6174 6820 2929 0a20 2020 2020  e, path )).     
-00004390: 2020 2020 2020 2063 6f6e 7469 6e75 650a         continue.
-000043a0: 2020 2020 2020 2020 7265 636f 7264 0909          record..
-000043b0: 093d 2064 6963 7428 0a20 2020 2020 2020  .= dict(.       
-000043c0: 2020 2020 206e 616d 6509 3d20 6e61 6d65       name.= name
-000043d0: 2c0a 2020 2020 2020 2020 2020 2020 7573  ,.            us
-000043e0: 6572 6e61 6d65 093d 2075 7365 726e 616d  ername.= usernam
-000043f0: 652c 0a20 2020 2020 2020 2020 2020 2070  e,.            p
-00004400: 6173 7377 6f72 6409 3d20 7061 7373 776f  assword.= passwo
-00004410: 7264 2c0a 2020 2020 2020 2020 290a 2020  rd,.        ).  
-00004420: 2020 2020 2020 6c6c 2e61 7070 656e 6428        ll.append(
-00004430: 2072 6563 6f72 6420 290a 0a20 2020 2072   record )..    r
-00004440: 6574 7572 6e20 6461 7461 0a0a 0a64 6566  eturn data...def
-00004450: 206b 6579 7061 6972 735f 6461 7461 2820   keypairs_data( 
-00004460: 7061 7468 2029 3a0a 2020 2020 6461 7461  path ):.    data
-00004470: 0909 093d 207b 7d0a 2020 2020 6461 7461  ...= {}.    data
-00004480: 5b22 7469 746c 6522 5d09 093d 2022 4b65  ["title"]..= "Ke
-00004490: 7970 6169 7273 220a 2020 2020 6461 7461  ypairs".    data
-000044a0: 5b22 7061 7468 225d 0909 3d20 7061 7468  ["path"]..= path
-000044b0: 0a20 2020 2064 6174 615b 226c 6973 7422  .    data["list"
-000044c0: 5d20 3d20 6c6c 0909 3d20 5b5d 0a20 2020  ] = ll..= [].   
-000044d0: 2064 6174 615b 226b 6579 7322 5d09 093d   data["keys"]..=
-000044e0: 205b 226e 616d 6522 2c20 2270 7562 6c69   ["name", "publi
-000044f0: 635f 6b65 7922 2c20 2263 7265 6465 6e74  c_key", "credent
-00004500: 6961 6c73 225d 0a0a 2020 2020 7061 7468  ials"]..    path
-00004510: 7365 6773 0909 093d 2070 6174 682e 7374  segs...= path.st
-00004520: 7269 7028 272f 2729 2e73 706c 6974 2827  rip('/').split('
-00004530: 2f27 2920 6966 2070 6174 6820 656c 7365  /') if path else
-00004540: 205b 5d0a 2020 2020 6173 7365 7274 2030   [].    assert 0
-00004550: 203c 3d20 6c65 6e28 2070 6174 6873 6567   <= len( pathseg
-00004560: 7320 2920 3c3d 2031 2c20 2249 6e76 616c  s ) <= 1, "Inval
-00004570: 6964 206b 6579 7061 6972 7320 7061 7468  id keypairs path
-00004580: 207b 7d22 2e66 6f72 6d61 7428 2070 6174   {}".format( pat
-00004590: 6820 290a 0a20 2020 2023 2047 6574 2061  h )..    # Get a
-000045a0: 6c6c 2063 7265 6465 6e74 6961 6c73 2069  ll credentials i
-000045b0: 6e74 6f20 6372 6564 733a 207b 206e 616d  nto creds: { nam
-000045c0: 653a 2028 7573 6572 6e61 6d65 2c70 6173  e: (username,pas
-000045d0: 7377 6f72 6429 2c20 2e2e 2e20 7d2c 2061  sword), ... }, a
-000045e0: 6e64 2062 7569 6c64 2061 2072 6576 6572  nd build a rever
-000045f0: 7365 2d6c 6f6f 6b75 7020 6469 6374 0a20  se-lookup dict. 
-00004600: 2020 2023 2063 7265 6473 5f72 6576 6572     # creds_rever
-00004610: 7365 3a20 7b20 2875 7365 726e 616d 652c  se: { (username,
-00004620: 7061 7373 776f 7264 293a 206e 616d 652c  password): name,
-00004630: 202e 2e2e 207d 0a20 2020 2063 7265 6473   ... }.    creds
-00004640: 0909 093d 2064 6963 7428 2063 7265 6465  ...= dict( crede
-00004650: 6e74 6961 6c73 2829 2029 0a20 2020 2063  ntials() ).    c
-00004660: 7265 6473 5f72 6576 6572 7365 0909 3d20  reds_reverse..= 
-00004670: 7b20 763a 206b 2066 6f72 206b 2c76 2069  { v: k for k,v i
-00004680: 6e20 6372 6564 732e 6974 656d 7328 2920  n creds.items() 
-00004690: 7d0a 0a20 2020 206c 6f67 2e69 6e66 6f28  }..    log.info(
-000046a0: 2022 4b65 7970 6169 7273 2064 6174 6120   "Keypairs data 
-000046b0: 772f 207b 7d20 6372 6564 656e 7469 616c  w/ {} credential
-000046c0: 3a22 2e66 6f72 6d61 7428 206c 656e 2820  :".format( len( 
-000046d0: 6372 6564 735f 7265 7665 7273 6520 2929  creds_reverse ))
-000046e0: 290a 2020 2020 666f 7220 6e61 6d65 2c6b  ).    for name,k
-000046f0: 6579 7061 6972 2c63 7265 6420 696e 206b  eypair,cred in k
-00004700: 6579 7061 6972 7328 293a 0a20 2020 2020  eypairs():.     
-00004710: 2020 206c 6f67 2e69 6e66 6f28 2246 6f75     log.info("Fou
-00004720: 6e64 206b 6579 7061 6972 3a20 7b21 727d  nd keypair: {!r}
-00004730: 222e 666f 726d 6174 2820 286e 616d 652c  ".format( (name,
-00004740: 6b65 7970 6169 722c 6372 6564 2920 2929  keypair,cred) ))
-00004750: 0a20 2020 2020 2020 2069 6620 7061 7468  .        if path
-00004760: 7365 6773 2061 6e64 2070 6174 6873 6567  segs and pathseg
-00004770: 735b 305d 2061 6e64 206e 6f74 2066 6e6d  s[0] and not fnm
-00004780: 6174 6368 2e66 6e6d 6174 6368 2820 6e61  atch.fnmatch( na
-00004790: 6d65 2c20 7061 7468 7365 6773 5b30 5d20  me, pathsegs[0] 
-000047a0: 293a 0a20 2020 2020 2020 2020 2020 206c  ):.            l
-000047b0: 6f67 2e69 6e66 6f28 2022 4372 6564 656e  og.info( "Creden
-000047c0: 7469 616c 207b 7d20 6469 646e 2774 206d  tial {} didn't m
-000047d0: 6174 6368 207b 7d22 2e66 6f72 6d61 7428  atch {}".format(
-000047e0: 206e 616d 652c 2070 6174 6820 2929 0a20   name, path )). 
-000047f0: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
-00004800: 6e75 650a 2020 2020 2020 2020 7265 636f  nue.        reco
-00004810: 7264 0909 093d 2064 6963 7428 0a20 2020  rd...= dict(.   
-00004820: 2020 2020 2020 2020 206e 616d 6509 3d20           name.= 
-00004830: 6e61 6d65 2c0a 2020 2020 2020 2020 2020  name,.          
-00004840: 2020 7075 626c 6963 5f6b 6579 093d 206c    public_key.= l
-00004850: 6963 656e 7369 6e67 2e69 6e74 6f5f 6236  icensing.into_b6
-00004860: 3428 206b 6579 7061 6972 2e69 6e74 6f5f  4( keypair.into_
-00004870: 6b65 7970 6169 7228 202a 2a63 7265 6420  keypair( **cred 
-00004880: 292e 766b 2029 2c0a 2020 2020 2020 2020  ).vk ),.        
-00004890: 2020 2020 6372 6564 656e 7469 616c 7309      credentials.
-000048a0: 3d20 6372 6564 735f 7265 7665 7273 652e  = creds_reverse.
-000048b0: 6765 7428 2028 6372 6564 5b27 7573 6572  get( (cred['user
-000048c0: 6e61 6d65 275d 2c20 6372 6564 5b27 7061  name'], cred['pa
-000048d0: 7373 776f 7264 275d 292c 2027 2875 6e6b  ssword']), '(unk
-000048e0: 6e6f 776e 2927 2029 2c0a 2020 2020 2020  nown)' ),.      
-000048f0: 2020 290a 2020 2020 2020 2020 6c6c 2e61    ).        ll.a
-00004900: 7070 656e 6428 2072 6563 6f72 6420 290a  ppend( record ).
-00004910: 0a20 2020 2072 6574 7572 6e20 6461 7461  .    return data
-00004920: 0a0a 0a23 2053 6574 2075 7020 7369 676e  ...# Set up sign
-00004930: 616c 2068 616e 646c 696e 6720 286c 6f67  al handling (log
-00004940: 2072 6f74 6174 696f 6e2c 206c 6f67 206c   rotation, log l
-00004950: 6576 656c 2c20 6574 632e 290a 2320 4f75  evel, etc.).# Ou
-00004960: 7470 7574 206c 6f67 6769 6e67 2074 6f20  tput logging to 
-00004970: 6120 6669 6c65 2c20 616e 6420 6861 6e64  a file, and hand
-00004980: 6c65 2055 4e49 582d 7920 6c6f 6720 6669  le UNIX-y log fi
-00004990: 6c65 2072 6f74 6174 696f 6e20 7669 6120  le rotation via 
-000049a0: 276c 6f67 726f 7461 7465 272c 2077 6869  'logrotate', whi
-000049b0: 6368 2073 656e 6473 0a23 2073 6967 6e61  ch sends.# signa
-000049c0: 6c73 2074 6f20 696e 6469 6361 7465 2074  ls to indicate t
-000049d0: 6861 7420 6120 7365 7276 6963 6527 7320  hat a service's 
-000049e0: 6c6f 6720 6669 6c65 2068 6173 2062 6565  log file has bee
-000049f0: 6e20 6d6f 7665 642f 7265 6e61 6d65 6420  n moved/renamed 
-00004a00: 616e 6420 6974 2073 686f 756c 6420 7265  and it should re
-00004a10: 2d6f 7065 6e0a 0a75 7074 696d 655f 6261  -open..uptime_ba
-00004a20: 7369 7309 0909 3d20 7469 6d65 7228 290a  sis...= timer().
-00004a30: 7570 7469 6d65 5f73 6967 6e61 6c6c 6564  uptime_signalled
-00004a40: 0909 3d20 4661 6c73 650a 7368 7574 646f  ..= False.shutdo
-00004a50: 776e 5f73 6967 6e61 6c6c 6564 0909 3d20  wn_signalled..= 
-00004a60: 4661 6c73 650a 6c6f 6772 6f74 6174 655f  False.logrotate_
-00004a70: 7369 676e 616c 6c65 6409 093d 2046 616c  signalled..= Fal
-00004a80: 7365 0a6c 6576 656c 6d61 705f 6368 616e  se.levelmap_chan
-00004a90: 6765 0909 093d 2030 2020 2320 6d61 7920  ge...= 0  # may 
-00004aa0: 6265 636f 6d65 202b 2776 652f 2d27 7665  become +'ve/-'ve
-00004ab0: 0a0a 0a64 6566 2075 7074 696d 655f 7265  ...def uptime_re
-00004ac0: 7175 6573 7428 2073 6967 6e75 6d2c 2066  quest( signum, f
-00004ad0: 7261 6d65 2029 3a0a 2020 2020 676c 6f62  rame ):.    glob
-00004ae0: 616c 2075 7074 696d 655f 7369 676e 616c  al uptime_signal
-00004af0: 6c65 640a 2020 2020 7570 7469 6d65 5f73  led.    uptime_s
-00004b00: 6967 6e61 6c6c 6564 0909 3d20 5472 7565  ignalled..= True
-00004b10: 0a0a 0a64 6566 2073 6875 7464 6f77 6e5f  ...def shutdown_
-00004b20: 7265 7175 6573 7428 2073 6967 6e75 6d2c  request( signum,
-00004b30: 2066 7261 6d65 2029 3a0a 2020 2020 676c   frame ):.    gl
-00004b40: 6f62 616c 2073 6875 7464 6f77 6e5f 7369  obal shutdown_si
-00004b50: 676e 616c 6c65 640a 2020 2020 7368 7574  gnalled.    shut
-00004b60: 646f 776e 5f73 6967 6e61 6c6c 6564 0909  down_signalled..
-00004b70: 3d20 5472 7565 0a0a 0a64 6566 206c 6f67  = True...def log
-00004b80: 726f 7461 7465 5f72 6571 7565 7374 2820  rotate_request( 
-00004b90: 7369 676e 756d 2c20 6672 616d 6520 293a  signum, frame ):
-00004ba0: 0a20 2020 2067 6c6f 6261 6c20 6c6f 6772  .    global logr
-00004bb0: 6f74 6174 655f 7369 676e 616c 6c65 640a  otate_signalled.
-00004bc0: 2020 2020 6c6f 6772 6f74 6174 655f 7369      logrotate_si
-00004bd0: 676e 616c 6c65 6409 093d 2054 7275 650a  gnalled..= True.
-00004be0: 0a0a 6465 6620 6c6f 676c 6576 656c 7570  ..def loglevelup
-00004bf0: 5f72 6571 7565 7374 2820 7369 676e 756d  _request( signum
-00004c00: 2c20 6672 616d 6520 293a 0a20 2020 2067  , frame ):.    g
-00004c10: 6c6f 6261 6c20 6c65 7665 6c6d 6170 5f63  lobal levelmap_c
-00004c20: 6861 6e67 650a 2020 2020 6c65 7665 6c6d  hange.    levelm
-00004c30: 6170 5f63 6861 6e67 6509 2020 2020 2020  ap_change.      
-00004c40: 202b 3d20 310a 0a0a 6465 6620 6c6f 676c   += 1...def logl
-00004c50: 6576 656c 646e 5f72 6571 7565 7374 2820  eveldn_request( 
-00004c60: 7369 676e 756d 2c20 6672 616d 6520 293a  signum, frame ):
-00004c70: 0a20 2020 2067 6c6f 6261 6c20 6c65 7665  .    global leve
-00004c80: 6c6d 6170 5f63 6861 6e67 650a 2020 2020  lmap_change.    
-00004c90: 6c65 7665 6c6d 6170 5f63 6861 6e67 6509  levelmap_change.
-00004ca0: 2020 2020 2020 202d 3d20 310a 0a0a 6465         -= 1...de
-00004cb0: 6620 7369 676e 616c 5f73 6572 7669 6365  f signal_service
-00004cc0: 2829 3a0a 2020 2020 2222 2253 6572 7669  ():.    """Servi
-00004cd0: 6365 206b 6e6f 776e 2073 6967 6e61 6c73  ce known signals
-00004ce0: 2e20 2057 6865 6e20 6c6f 6767 696e 672c  .  When logging,
-00004cf0: 2064 6566 6175 6c74 2074 6f20 6c6f 6720   default to log 
-00004d00: 6174 2057 4152 4e49 4e47 2c20 6275 7420  at WARNING, but 
-00004d10: 656e 7375 7265 2074 6865 0a20 2020 206d  ensure the.    m
-00004d20: 6573 7361 6765 2069 7320 7365 656e 2069  essage is seen i
-00004d30: 6620 6869 6768 6572 2028 6567 2e20 5741  f higher (eg. WA
-00004d40: 524e 494e 4729 2e20 2053 7570 706f 7274  RNING).  Support
-00004d50: 2062 6569 6e67 2069 6e20 756e 6b6e 6f77   being in unknow
-00004d60: 6e20 6c6f 6767 696e 670a 2020 2020 6c65  n logging.    le
-00004d70: 7665 6c73 2077 6865 6e20 696e 2f64 6563  vels when in/dec
-00004d80: 7265 6173 696e 672e 0a0a 2020 2020 2222  reasing...    ""
-00004d90: 220a 2020 2020 676c 6f62 616c 206c 6576  ".    global lev
-00004da0: 656c 6d61 705f 6368 616e 6765 0a20 2020  elmap_change.   
-00004db0: 2069 6620 6c65 7665 6c6d 6170 5f63 6861   if levelmap_cha
-00004dc0: 6e67 653a 0a20 2020 2020 2020 2072 6f6f  nge:.        roo
-00004dd0: 746c 6f67 0909 093d 206c 6f67 6769 6e67  tlog...= logging
-00004de0: 2e67 6574 4c6f 6767 6572 2829 0a20 2020  .getLogger().   
-00004df0: 2020 2020 2061 6374 7561 6c09 0909 3d20       actual...= 
-00004e00: 726f 6f74 6c6f 672e 6765 7445 6666 6563  rootlog.getEffec
-00004e10: 7469 7665 4c65 7665 6c28 290a 2020 2020  tiveLevel().    
-00004e20: 2020 2020 2320 4669 6e64 2074 6865 2063      # Find the c
-00004e30: 7572 7265 6e74 206c 6f67 5f6c 6576 656c  urrent log_level
-00004e40: 6d61 7020 6b65 7920 772f 2061 206c 6576  map key w/ a lev
-00004e50: 656c 2076 616c 7565 206e 6561 7265 7374  el value nearest
-00004e60: 206f 7572 2063 7572 7265 6e74 2061 6374   our current act
-00004e70: 7561 6c20 6c65 7665 6c2e 2020 4465 6661  ual level.  Defa
-00004e80: 756c 7420 746f 2030 2e0a 2020 2020 2020  ult to 0..      
-00004e90: 2020 6b65 792c 6469 6609 0909 3d20 302c    key,dif...= 0,
-00004ea0: 3130 3030 0a20 2020 2020 2020 2066 6f72  1000.        for
-00004eb0: 206b 2c6c 766c 2069 6e20 6c6f 675f 6c65   k,lvl in log_le
-00004ec0: 7665 6c6d 6170 2e69 7465 6d73 2829 3a0a  velmap.items():.
-00004ed0: 2020 2020 2020 2020 2020 2020 6966 2061              if a
-00004ee0: 6273 2820 6c76 6c20 2d20 6163 7475 616c  bs( lvl - actual
-00004ef0: 2029 203c 2064 6966 3a0a 2020 2020 2020   ) < dif:.      
-00004f00: 2020 2020 2020 2020 2020 6b65 7909 093d            key..=
-00004f10: 206b 0a20 2020 2020 2020 2023 2047 6574   k.        # Get
-00004f20: 2061 6e20 6176 6169 6c61 626c 6520 6c6f   an available lo
-00004f30: 675f 6c65 7665 6c20 7570 2f64 6f77 6e20  g_level up/down 
-00004f40: 6672 6f6d 2074 6865 2063 7572 7265 6e74  from the current
-00004f50: 6c79 2061 6374 6976 6520 6f6e 650a 2020  ly active one.  
-00004f60: 2020 2020 2020 6465 7369 7265 6409 0909        desired...
-00004f70: 3d20 6c6f 675f 6c65 7665 6c28 206b 6579  = log_level( key
-00004f80: 202b 206c 6576 656c 6d61 705f 6368 616e   + levelmap_chan
-00004f90: 6765 2029 0a20 2020 2020 2020 2069 6620  ge ).        if 
-00004fa0: 6163 7475 616c 2021 3d20 6465 7369 7265  actual != desire
-00004fb0: 643a 0a20 2020 2020 2020 2020 2020 2072  d:.            r
-00004fc0: 6f6f 746c 6f67 2e73 6574 4c65 7665 6c28  ootlog.setLevel(
-00004fd0: 2064 6573 6972 6564 2029 0a20 2020 2020   desired ).     
-00004fe0: 2020 206c 6576 656c 6d61 705f 6368 616e     levelmap_chan
-00004ff0: 6765 0909 3d20 300a 0a20 2020 2067 6c6f  ge..= 0..    glo
-00005000: 6261 6c20 6c6f 6772 6f74 6174 655f 7369  bal logrotate_si
-00005010: 676e 616c 6c65 640a 2020 2020 676c 6f62  gnalled.    glob
-00005020: 616c 2075 7074 696d 655f 7369 676e 616c  al uptime_signal
-00005030: 6c65 640a 2020 2020 6966 206c 6f67 726f  led.    if logro
-00005040: 7461 7465 5f73 6967 6e61 6c6c 6564 3a0a  tate_signalled:.
-00005050: 2020 2020 2020 2020 6c6f 6772 6f74 6174          logrotat
-00005060: 655f 7369 676e 616c 6c65 6409 3d20 4661  e_signalled.= Fa
-00005070: 6c73 650a 2020 2020 2020 2020 7570 7469  lse.        upti
-00005080: 6d65 5f73 6967 6e61 6c6c 6564 093d 2054  me_signalled.= T
-00005090: 7275 650a 0a20 2020 2020 2020 2072 6f6f  rue..        roo
-000050a0: 746c 6f67 0909 093d 206c 6f67 6769 6e67  tlog...= logging
-000050b0: 2e67 6574 4c6f 6767 6572 2829 0a20 2020  .getLogger().   
-000050c0: 2020 2020 2061 6374 7561 6c09 0909 3d20       actual...= 
-000050d0: 726f 6f74 6c6f 672e 6765 7445 6666 6563  rootlog.getEffec
-000050e0: 7469 7665 4c65 7665 6c28 290a 2020 2020  tiveLevel().    
-000050f0: 2020 2020 726f 6f74 6c6f 672e 6c6f 6728      rootlog.log(
-00005100: 206d 6178 2820 6c6f 6767 696e 672e 5741   max( logging.WA
-00005110: 524e 494e 472c 2061 6374 7561 6c20 292c  RNING, actual ),
-00005120: 2022 526f 7461 7469 6e67 206c 6f67 2066   "Rotating log f
-00005130: 696c 6573 2064 7565 2074 6f20 7369 676e  iles due to sign
-00005140: 616c 2220 290a 2020 2020 2020 2020 666f  al" ).        fo
-00005150: 7220 6864 6c72 2069 6e20 6c6f 6767 696e  r hdlr in loggin
-00005160: 672e 726f 6f74 2e68 616e 646c 6572 733a  g.root.handlers:
-00005170: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00005180: 6973 696e 7374 616e 6365 2820 6864 6c72  isinstance( hdlr
-00005190: 2c20 6c6f 6767 696e 672e 4669 6c65 4861  , logging.FileHa
-000051a0: 6e64 6c65 7220 293a 0a20 2020 2020 2020  ndler ):.       
-000051b0: 2020 2020 2020 2020 2068 646c 722e 636c           hdlr.cl
-000051c0: 6f73 6528 290a 0a20 2020 2067 6c6f 6261  ose()..    globa
-000051d0: 6c20 7570 7469 6d65 5f62 6173 6973 0a20  l uptime_basis. 
-000051e0: 2020 2069 6620 7570 7469 6d65 5f73 6967     if uptime_sig
-000051f0: 6e61 6c6c 6564 3a0a 2020 2020 2020 2020  nalled:.        
-00005200: 7570 7469 6d65 5f73 6967 6e61 6c6c 6564  uptime_signalled
-00005210: 093d 2046 616c 7365 0a20 2020 2020 2020  .= False.       
-00005220: 2075 7074 696d 6509 0909 3d20 7469 6d65   uptime...= time
-00005230: 7228 2920 2d20 7570 7469 6d65 5f62 6173  r() - uptime_bas
-00005240: 6973 0a0a 2020 2020 2020 2020 726f 6f74  is..        root
-00005250: 6c6f 6709 0909 3d20 6c6f 6767 696e 672e  log...= logging.
-00005260: 6765 744c 6f67 6765 7228 290a 2020 2020  getLogger().    
-00005270: 2020 2020 6163 7475 616c 0909 093d 2072      actual...= r
-00005280: 6f6f 746c 6f67 2e67 6574 4566 6665 6374  ootlog.getEffect
-00005290: 6976 654c 6576 656c 2829 0a20 2020 2020  iveLevel().     
-000052a0: 2020 2072 6f6f 746c 6f67 2e6c 6f67 2820     rootlog.log( 
-000052b0: 6d61 7828 206c 6f67 6769 6e67 2e57 4152  max( logging.WAR
-000052c0: 4e49 4e47 2c20 6163 7475 616c 2029 2c20  NING, actual ), 
-000052d0: 2255 7074 696d 653a 2025 3364 3a25 3032  "Uptime: %3d:%02
-000052e0: 643a 2530 362e 3366 222c 0a20 2020 2020  d:%06.3f",.     
-000052f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005300: 696e 7428 2075 7074 696d 6520 2f2f 2033  int( uptime // 3
-00005310: 3630 3020 292c 2069 6e74 2820 7570 7469  600 ), int( upti
-00005320: 6d65 2025 2033 3630 3020 2f2f 2036 3020  me % 3600 // 60 
-00005330: 292c 2075 7074 696d 6520 2520 3630 2029  ), uptime % 60 )
-00005340: 0a0a 0a73 6967 6e61 6c2e 7369 676e 616c  ...signal.signal
-00005350: 2820 7369 676e 616c 2e53 4947 4855 502c  ( signal.SIGHUP,
-00005360: 2020 6c6f 6772 6f74 6174 655f 7265 7175    logrotate_requ
-00005370: 6573 7420 290a 7369 676e 616c 2e73 6967  est ).signal.sig
-00005380: 6e61 6c28 2073 6967 6e61 6c2e 5349 4755  nal( signal.SIGU
-00005390: 5352 312c 206c 6f67 6c65 7665 6c75 705f  SR1, loglevelup_
-000053a0: 7265 7175 6573 7420 290a 7369 676e 616c  request ).signal
-000053b0: 2e73 6967 6e61 6c28 2073 6967 6e61 6c2e  .signal( signal.
-000053c0: 5349 4755 5352 322c 206c 6f67 6c65 7665  SIGUSR2, logleve
-000053d0: 6c64 6e5f 7265 7175 6573 7420 290a 7369  ldn_request ).si
-000053e0: 676e 616c 2e73 6967 6e61 6c28 2073 6967  gnal.signal( sig
-000053f0: 6e61 6c2e 5349 4754 4552 4d2c 2073 6875  nal.SIGTERM, shu
-00005400: 7464 6f77 6e5f 7265 7175 6573 7420 290a  tdown_request ).
-00005410: 7369 676e 616c 2e73 6967 6e61 6c28 2073  signal.signal( s
-00005420: 6967 6e61 6c2e 5349 4755 5247 2c20 2075  ignal.SIGURG,  u
-00005430: 7074 696d 655f 7265 7175 6573 7420 290a  ptime_request ).
-00005440: 0a6e 6f77 0909 0909 3d20 7469 6d65 7228  .now....= timer(
-00005450: 290a 0a0a 6465 6620 6461 7974 696d 6528  )...def daytime(
-00005460: 2074 7320 293a 0a20 2020 2072 6574 7572   ts ):.    retur
-00005470: 6e20 5469 6d65 7374 616d 7028 2074 7320  n Timestamp( ts 
-00005480: 290a 0a23 0a23 2043 7572 7365 732d 6261  )..#.# Curses-ba
-00005490: 7365 6420 5465 7874 7561 6c20 5549 2e0a  sed Textual UI..
-000054a0: 230a 0a0a 6465 6620 6d65 7373 6167 6528  #...def message(
-000054b0: 2077 696e 646f 772c 2074 6578 742c 2072   window, text, r
-000054c0: 6f77 203d 2032 332c 2063 6f6c 203d 2030  ow = 23, col = 0
-000054d0: 2c20 636c 6561 7220 3d20 5472 7565 2029  , clear = True )
-000054e0: 3a0a 2020 2020 726f 7773 2c63 6f6c 7309  :.    rows,cols.
-000054f0: 0909 3d20 7769 6e64 6f77 2e67 6574 6d61  ..= window.getma
-00005500: 7879 7828 290a 2020 2020 6966 2063 6f6c  xyx().    if col
-00005510: 203c 202d 6c65 6e28 2074 6578 7420 2920   < -len( text ) 
-00005520: 6f72 2072 6f77 203c 2030 206f 7220 726f  or row < 0 or ro
-00005530: 7720 3e3d 2072 6f77 7320 6f72 2063 6f6c  w >= rows or col
-00005540: 203e 3d20 636f 6c73 3a0a 2020 2020 2020   >= cols:.      
-00005550: 2020 7265 7475 726e 0a20 2020 2069 6620    return.    if 
-00005560: 636f 6c20 3c20 303a 0a20 2020 2020 2020  col < 0:.       
-00005570: 2074 6578 7409 0909 3d20 7465 7874 5b2d   text...= text[-
-00005580: 636f 6c3a 5d0a 2020 2020 2020 2020 636f  col:].        co
-00005590: 6c09 0909 3d20 300a 2020 2020 7472 793a  l...= 0.    try:
-000055a0: 0a20 2020 2020 2020 2077 696e 646f 772e  .        window.
-000055b0: 6164 6473 7472 2820 696e 7428 2072 6f77  addstr( int( row
-000055c0: 2029 2c20 696e 7428 2063 6f6c 2029 2c20   ), int( col ), 
-000055d0: 7465 7874 5b3a 636f 6c73 2d63 6f6c 5d20  text[:cols-col] 
-000055e0: 290a 2020 2020 2020 2020 6966 2063 6c65  ).        if cle
-000055f0: 6172 3a0a 2020 2020 2020 2020 2020 2020  ar:.            
-00005600: 7769 6e64 6f77 2e63 6c72 746f 656f 6c28  window.clrtoeol(
-00005610: 290a 2020 2020 6578 6365 7074 2045 7863  ).    except Exc
-00005620: 6570 7469 6f6e 3a0a 2020 2020 2020 2020  eption:.        
-00005630: 7061 7373 0a0a 0a23 0a23 2070 616e 7b73  pass...#.# pan{s
-00005640: 697a 2c6c 6f63 7d20 2d2d 2063 6f6d 7075  iz,loc} -- compu
-00005650: 7465 2061 7070 726f 7072 6961 7465 2073  te appropriate s
-00005660: 697a 6520 616e 6420 6c6f 6361 7469 6f6e  ize and location
-00005670: 2066 6f72 2073 656e 736f 7220 6465 7461   for sensor deta
-00005680: 696c 2070 616e 656c 0a23 0a64 6566 2070  il panel.#.def p
-00005690: 616e 7369 7a28 2072 6f77 732c 2063 6f6c  ansiz( rows, col
-000056a0: 7320 293a 0a20 2020 2072 6574 7572 6e20  s ):.    return 
-000056b0: 726f 7773 202a 2039 202f 2f20 3130 2c20  rows * 9 // 10, 
-000056c0: 636f 6c73 202f 2f20 330a 0a0a 6465 6620  cols // 3...def 
-000056d0: 7061 6e6c 6f63 2820 632c 2072 6f77 732c  panloc( c, rows,
-000056e0: 2063 6f6c 7320 293a 0a20 2020 2072 6574   cols ):.    ret
-000056f0: 7572 6e20 726f 7773 2f2f 3135 2c20 2820  urn rows//15, ( 
-00005700: 6320 3c20 636f 6c73 2f2f 3220 2920 616e  c < cols//2 ) an
-00005710: 6420 2820 636f 6c73 2f2f 3220 2b20 636f  d ( cols//2 + co
-00005720: 6c73 2f2f 3130 2029 206f 7220 2820 3020  ls//10 ) or ( 0 
-00005730: 2b20 636f 6c73 2f2f 3130 2029 0a0a 0a64  + cols//10 )...d
-00005740: 6566 2074 7874 2820 7769 6e2c 2063 6f6e  ef txt( win, con
-00005750: 6669 6720 293a 0a0a 2020 2020 676c 6f62  fig ):..    glob
-00005760: 616c 206e 6f77 0a20 2020 206c 6173 7409  al now.    last.
-00005770: 0909 3d20 6e6f 770a 2020 2020 7365 6c65  ..= now.    sele
-00005780: 6374 6564 0909 093d 2030 0a0a 2020 2020  cted...= 0..    
-00005790: 726f 7773 2c20 636f 6c73 0909 093d 2030  rows, cols...= 0
-000057a0: 2c20 300a 0a20 2020 206c 6f67 2e69 6e66  , 0..    log.inf
-000057b0: 6f28 2274 6872 6561 6473 3a20 2532 643a  o("threads: %2d:
-000057c0: 2025 7322 2025 2028 0a20 2020 2020 2020   %s" % (.       
-000057d0: 2074 6872 6561 6469 6e67 2e61 6374 6976   threading.activ
-000057e0: 655f 636f 756e 7428 292c 0a20 2020 2020  e_count(),.     
-000057f0: 2020 2027 2c20 272e 6a6f 696e 2820 5b20     ', '.join( [ 
-00005800: 742e 6e61 6d65 2066 6f72 2074 2069 6e20  t.name for t in 
-00005810: 7468 7265 6164 696e 672e 656e 756d 6572  threading.enumer
-00005820: 6174 6528 2920 5d20 2929 290a 0a20 2020  ate() ] )))..   
-00005830: 2064 6973 706c 6179 0909 093d 2027 6c69   display...= 'li
-00005840: 6365 6e73 6573 2709 0923 2053 7461 7274  censes'..# Start
-00005850: 206f 6666 2064 6973 706c 6179 696e 6720   off displaying 
-00005860: 4c69 6365 6e73 6573 0a20 2020 2069 6e70  Licenses.    inp
-00005870: 7574 0909 093d 2030 0a20 2020 2064 656c  ut...= 0.    del
-00005880: 7461 0909 093d 2030 2e30 0a20 2020 2070  ta...= 0.0.    p
-00005890: 616e 7365 6c09 0909 3d20 4e6f 6e65 0a20  ansel...= None. 
-000058a0: 2020 2077 6869 6c65 206e 6f74 2063 6f6e     while not con
-000058b0: 6669 672e 6765 7428 2027 646f 6e65 2720  fig.get( 'done' 
-000058c0: 293a 0a20 2020 2020 2020 206d 6573 7361  ):.        messa
-000058d0: 6765 2820 7769 6e2c 2022 2573 2028 2537  ge( win, "%s (%7
-000058e0: 2e33 6629 3a20 2825 3364 203d 3d20 2725  .3f): (%3d == '%
-000058f0: 6327 2920 5175 6974 205b 7179 2f6e 5d3f  c') Quit [qy/n]?
-00005900: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00005910: 2020 2025 2028 2020 6461 7974 696d 6528     % (  daytime(
-00005920: 206e 6f77 2029 2c20 6465 6c74 612c 0a20   now ), delta,. 
-00005930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005940: 2020 2020 2069 6e70 7574 2c20 6375 7273       input, curs
-00005950: 6573 2e61 7363 6969 2e69 7370 7269 6e74  es.ascii.isprint
-00005960: 2820 696e 7075 7420 2920 616e 6420 6368  ( input ) and ch
-00005970: 7228 2069 6e70 7574 2029 206f 7220 273f  r( input ) or '?
-00005980: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
-00005990: 2020 2020 2072 6f77 203d 2030 2c20 636c       row = 0, cl
-000059a0: 6561 7220 3d20 4661 6c73 6520 290a 0a20  ear = False ).. 
-000059b0: 2020 2020 2020 2063 7572 7365 732e 7061         curses.pa
-000059c0: 6e65 6c2e 7570 6461 7465 5f70 616e 656c  nel.update_panel
-000059d0: 7328 290a 2020 2020 2020 2020 6375 7273  s().        curs
-000059e0: 6573 2e64 6f75 7064 6174 6528 290a 0a20  es.doupdate().. 
-000059f0: 2020 2020 2020 2023 2045 6e64 206f 6620         # End of 
-00005a00: 6469 7370 6c61 7920 6c6f 6f70 3b20 6469  display loop; di
-00005a10: 7370 6c61 7920 7570 6461 7465 643b 2042  splay updated; B
-00005a20: 6567 696e 6e69 6e67 206f 6620 6e65 7874  eginning of next
-00005a30: 206c 6f6f 703b 2061 7761 6974 2069 6e70   loop; await inp
-00005a40: 7574 0a20 2020 2020 2020 2069 6e70 7574  ut.        input
-00005a50: 0909 093d 2077 696e 2e67 6574 6368 2829  ...= win.getch()
-00005a60: 0a0a 2020 2020 2020 2020 2320 5265 6672  ..        # Refr
-00005a70: 6573 6820 7468 6520 7468 696e 6773 2074  esh the things t
-00005a80: 6f20 696e 636c 7564 6520 696e 2074 6865  o include in the
-00005a90: 2073 656c 6563 7465 6420 6469 7370 6c61   selected displa
-00005aa0: 792e 0a20 2020 2020 2020 2069 6e63 6c75  y..        inclu
-00005ab0: 6465 0909 093d 2063 6f6e 6669 675b 6469  de...= config[di
-00005ac0: 7370 6c61 795d 0a20 2020 2020 2020 2069  splay].        i
-00005ad0: 6620 6861 7361 7474 7228 2069 6e63 6c75  f hasattr( inclu
-00005ae0: 6465 2c20 275f 5f63 616c 6c5f 5f27 2029  de, '__call__' )
-00005af0: 3a0a 2020 2020 2020 2020 2020 2020 696e  :.            in
-00005b00: 636c 7564 6509 093d 206c 6973 7428 2069  clude..= list( i
-00005b10: 6e63 6c75 6465 2829 2029 0a0a 2020 2020  nclude() )..    
-00005b20: 2020 2020 2320 436f 6d70 7574 6520 7469      # Compute ti
-00005b30: 6d65 2061 6476 616e 6365 2073 696e 6365  me advance since
-00005b40: 206c 6173 7420 7468 6572 6d6f 6479 6e61   last thermodyna
-00005b50: 6d69 6320 7570 6461 7465 0a20 2020 2020  mic update.     
-00005b60: 2020 2072 6561 6c09 0909 3d20 7469 6d65     real...= time
-00005b70: 7228 290a 2020 2020 2020 2020 6465 6c74  r().        delt
-00005b80: 6109 0909 3d20 7265 616c 202d 206c 6173  a...= real - las
-00005b90: 740a 0a20 2020 2020 2020 2023 2044 6574  t..        # Det
-00005ba0: 6563 7420 7769 6e64 6f77 2073 697a 6520  ect window size 
-00005bb0: 6368 616e 6765 732c 2061 6e64 2061 646a  changes, and adj
-00005bc0: 7573 7420 6465 7461 696c 2070 616e 656c  ust detail panel
-00005bd0: 2061 6363 6f72 6469 6e67 6c79 2028 6372   accordingly (cr
-00005be0: 6561 7469 6e67 2069 6620 6e65 6365 7373  eating if necess
-00005bf0: 6172 7929 0a20 2020 2020 2020 2069 6620  ary).        if 
-00005c00: 2872 6f77 732c 2063 6f6c 7329 2021 3d20  (rows, cols) != 
-00005c10: 7769 6e2e 6765 746d 6178 7978 2829 3a0a  win.getmaxyx():.
-00005c20: 2020 2020 2020 2020 2020 2020 726f 7773              rows
-00005c30: 2c20 636f 6c73 0909 3d20 7769 6e2e 6765  , cols..= win.ge
-00005c40: 746d 6178 7978 2829 0a20 2020 2020 2020  tmaxyx().       
-00005c50: 2020 2020 2077 696e 7365 6c09 093d 2063       winsel..= c
-00005c60: 7572 7365 732e 6e65 7777 696e 2820 2a20  urses.newwin( * 
-00005c70: 7061 6e73 697a 2820 726f 7773 2c20 636f  pansiz( rows, co
-00005c80: 6c73 2029 202b 2070 616e 6c6f 6328 2030  ls ) + panloc( 0
-00005c90: 2c20 726f 7773 2c20 636f 6c73 2029 290a  , rows, cols )).
-00005ca0: 2020 2020 2020 2020 2020 2020 7472 793a              try:
-00005cb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005cc0: 2070 616e 7365 6c2e 7265 706c 6163 6528   pansel.replace(
-00005cd0: 2077 696e 7365 6c20 290a 2020 2020 2020   winsel ).      
-00005ce0: 2020 2020 2020 6578 6365 7074 2045 7863        except Exc
-00005cf0: 6570 7469 6f6e 3a0a 2020 2020 2020 2020  eption:.        
-00005d00: 2020 2020 2020 2020 7061 6e73 656c 0909          pansel..
-00005d10: 3d20 6375 7273 6573 2e70 616e 656c 2e6e  = curses.panel.n
-00005d20: 6577 5f70 616e 656c 2820 7769 6e73 656c  ew_panel( winsel
-00005d30: 2029 0a0a 2020 2020 2020 2020 2320 5072   )..        # Pr
-00005d40: 6f63 6573 7320 696e 7075 742c 2061 646a  ocess input, adj
-00005d50: 7573 7469 6e67 2070 6172 616d 6574 6572  usting parameter
-00005d60: 730a 2020 2020 2020 2020 6966 2030 203c  s.        if 0 <
-00005d70: 2069 6e70 7574 203c 3d20 3235 3520 616e   input <= 255 an
-00005d80: 6420 6368 7228 2069 6e70 7574 2029 203d  d chr( input ) =
-00005d90: 3d20 2771 273a 0a20 2020 2020 2020 2020  = 'q':.         
-00005da0: 2020 2063 6f6e 6669 675b 2763 6f6e 7472     config['contr
-00005db0: 6f6c 275d 5b27 646f 6e65 275d 203d 2054  ol']['done'] = T
-00005dc0: 7275 650a 2020 2020 2020 2020 2020 2020  rue.            
-00005dd0: 7265 7475 726e 0a0a 2020 2020 2020 2020  return..        
-00005de0: 6966 2030 203c 2069 6e70 7574 203c 3d20  if 0 < input <= 
-00005df0: 3235 3520 616e 6420 6368 7228 2069 6e70  255 and chr( inp
-00005e00: 7574 2029 203d 3d20 275c 6627 3a09 0909  ut ) == '\f':...
-00005e10: 2320 4646 2c20 5e4c 0a20 2020 2020 2020  # FF, ^L.       
-00005e20: 2020 2020 2023 205e 4c20 2d2d 2063 6c65       # ^L -- cle
-00005e30: 6172 2073 6372 6565 6e0a 2020 2020 2020  ar screen.      
-00005e40: 2020 2020 2020 7769 6e73 656c 2e63 6c65        winsel.cle
-00005e50: 6172 2829 0a0a 2020 2020 2020 2020 2320  ar()..        # 
-00005e60: 5365 6c65 6374 206e 6578 7420 7370 6163  Select next spac
-00005e70: 652c 2061 646a 7573 7420 7461 7267 6574  e, adjust target
-00005e80: 2074 656d 700a 2020 2020 2020 2020 6966   temp.        if
-00005e90: 2069 6e70 7574 203d 3d20 6375 7273 6573   input == curses
-00005ea0: 2e61 7363 6969 2e53 503a 0909 0909 0923  .ascii.SP:.....#
-00005eb0: 2027 2027 0a20 2020 2020 2020 2020 2020   ' '.           
-00005ec0: 2069 6620 7061 6e73 656c 2e68 6964 6465   if pansel.hidde
-00005ed0: 6e28 293a 0a20 2020 2020 2020 2020 2020  n():.           
-00005ee0: 2020 2020 2070 616e 7365 6c2e 7368 6f77       pansel.show
-00005ef0: 2829 0a20 2020 2020 2020 2020 2020 2065  ().            e
-00005f00: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00005f10: 2020 2020 2070 616e 7365 6c2e 6869 6465       pansel.hide
-00005f20: 2829 0a0a 2020 2020 2020 2020 6966 2069  ()..        if i
-00005f30: 6e70 7574 2069 6e20 2820 6375 7273 6573  nput in ( curses
-00005f40: 2e61 7363 6969 2e53 5458 2c20 6375 7273  .ascii.STX, curs
-00005f50: 6573 2e4b 4559 5f4c 4546 542c 2032 3630  es.KEY_LEFT, 260
-00005f60: 2029 3a09 0923 205e 622c 203c 2d2d 0a20   ):..# ^b, <--. 
-00005f70: 2020 2020 2020 2020 2020 2073 656c 6563             selec
-00005f80: 7465 6409 093d 2028 2073 656c 6563 7465  ted..= ( selecte
-00005f90: 6420 2d20 3120 2920 2520 6c65 6e28 2069  d - 1 ) % len( i
-00005fa0: 6e63 6c75 6465 2029 0a20 2020 2020 2020  nclude ).       
-00005fb0: 2069 6620 696e 7075 7420 696e 2028 2063   if input in ( c
-00005fc0: 7572 7365 732e 6173 6369 692e 4143 4b2c  urses.ascii.ACK,
-00005fd0: 2063 7572 7365 732e 4b45 595f 5249 4748   curses.KEY_RIGH
-00005fe0: 542c 2032 3631 2029 3a20 2020 2020 2020  T, 261 ):       
-00005ff0: 2023 205e 662c 202d 2d3e 0a20 2020 2020   # ^f, -->.     
-00006000: 2020 2020 2020 2073 656c 6563 7465 6409         selected.
-00006010: 093d 2028 2073 656c 6563 7465 6420 2b20  .= ( selected + 
-00006020: 3120 2920 2520 6c65 6e28 2069 6e63 6c75  1 ) % len( inclu
-00006030: 6465 2029 0a20 2020 2020 2020 2069 6620  de ).        if 
-00006040: 696e 7075 7420 696e 2028 2063 7572 7365  input in ( curse
-00006050: 732e 6173 6369 692e 444c 452c 2063 7572  s.ascii.DLE, cur
-00006060: 7365 732e 4b45 595f 5550 2c20 3235 3920  ses.KEY_UP, 259 
-00006070: 293a 0909 2320 5e2c 205e 700a 2020 2020  ):..# ^, ^p.    
-00006080: 2020 2020 2020 2020 6966 2069 6e63 6c75          if inclu
-00006090: 6465 5b73 656c 6563 7465 645d 203d 3d20  de[selected] == 
-000060a0: 2777 6f72 6c64 273a 0909 0909 2320 7c0a  'world':....# |.
-000060b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000060c0: 2320 646f 2073 6f6d 6574 6869 6e67 2074  # do something t
-000060d0: 6f20 776f 726c 642e 2e2e 0a20 2020 2020  o world....     
-000060e0: 2020 2020 2020 2020 2020 2070 6173 730a             pass.
-000060f0: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00006100: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00006110: 2020 6375 7273 6573 2e62 6565 7028 290a    curses.beep().
-00006120: 2020 2020 2020 2020 6966 2069 6e70 7574          if input
-00006130: 2069 6e20 2820 6375 7273 6573 2e61 7363   in ( curses.asc
-00006140: 6969 2e53 4f2c 2063 7572 7365 732e 4b45  ii.SO, curses.KE
-00006150: 595f 444f 574e 2c20 3235 3820 293a 0909  Y_DOWN, 258 ):..
-00006160: 2320 7c0a 2020 2020 2020 2020 2020 2020  # |.            
-00006170: 6966 2069 6e63 6c75 6465 5b73 656c 6563  if include[selec
-00006180: 7465 645d 203d 3d20 2777 6f72 6c64 273a  ted] == 'world':
-00006190: 0909 0909 2320 762c 205e 6e0a 2020 2020  ....# v, ^n.    
-000061a0: 2020 2020 2020 2020 2020 2020 7061 7373              pass
-000061b0: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-000061c0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-000061d0: 2020 2063 7572 7365 732e 6265 6570 2829     curses.beep()
-000061e0: 0a0a 2020 2020 2020 2020 6966 2030 203c  ..        if 0 <
-000061f0: 2069 6e70 7574 203c 3d20 3235 3520 616e   input <= 255 an
-00006200: 6420 6368 7228 2069 6e70 7574 2029 2069  d chr( input ) i
-00006210: 6e20 2820 2743 272c 2027 6327 2c20 274d  n ( 'C', 'c', 'M
-00006220: 272c 2027 6d27 2029 3a0a 2020 2020 2020  ', 'm' ):.      
-00006230: 2020 2020 2020 2320 4368 6172 6163 7465        # Characte
-00006240: 7220 6b65 7970 7265 7373 6573 0a20 2020  r keypresses.   
-00006250: 2020 2020 2020 2020 2070 6173 730a 0a20           pass.. 
-00006260: 2020 2020 2020 2023 2057 6865 6e20 6120         # When a 
-00006270: 6b65 7970 7265 7373 2069 7320 6465 7465  keypress is dete
-00006280: 6374 6564 2c20 616c 7761 7973 206c 6f6f  cted, always loo
-00006290: 7020 6261 636b 2061 6e64 2067 6574 2061  p back and get a
-000062a0: 6e6f 7468 6572 206b 6579 2c20 746f 2061  nother key, to a
-000062b0: 6273 6f72 6220 6d75 6c74 6970 6c65 0a20  bsorb multiple. 
-000062c0: 2020 2020 2020 2023 206b 6579 7072 6573         # keypres
-000062d0: 7365 7320 2865 672e 2064 7565 2074 6f20  ses (eg. due to 
-000062e0: 6b65 7920 7265 7065 6174 292c 2062 7574  key repeat), but
-000062f0: 206f 6e6c 7920 646f 2069 7420 6966 206c   only do it if l
-00006300: 6573 7320 7468 656e 2031 2f33 2073 6563  ess then 1/3 sec
-00006310: 6f6e 6420 6861 7320 7061 7373 6564 2e0a  ond has passed..
-00006320: 2020 2020 2020 2020 6966 2030 203c 2069          if 0 < i
-00006330: 6e70 7574 2061 6e64 2064 656c 7461 203c  nput and delta <
-00006340: 202e 333a 0a20 2020 2020 2020 2020 2020   .3:.           
-00006350: 2063 6f6e 7469 6e75 650a 0a20 2020 2020   continue..     
-00006360: 2020 2023 2057 6527 6c6c 2062 6520 636f     # We'll be co
-00006370: 6d70 7574 696e 6720 6120 6e65 7720 6d6f  mputing a new mo
-00006380: 6465 6c3b 2061 6476 616e 6365 2028 616e  del; advance (an
-00006390: 6420 7265 6d65 6d62 6572 2920 7469 6d65  d remember) time
-000063a0: 0a20 2020 2020 2020 206c 6173 7409 0909  .        last...
-000063b0: 3d20 7265 616c 0a20 2020 2020 2020 206e  = real.        n
-000063c0: 6f77 2020 2020 2020 2020 2020 2020 2020  ow              
-000063d0: 2020 2020 2020 203d 2072 6561 6c0a 0a20         = real.. 
-000063e0: 2020 2020 2020 2023 204e 6578 7420 6672         # Next fr
-000063f0: 616d 6520 6f66 2061 6e69 6d61 7469 6f6e  ame of animation
-00006400: 0a20 2020 2020 2020 2077 696e 2e65 7261  .        win.era
-00006410: 7365 2829 0a0a 2020 2020 2020 2020 746f  se()..        to
-00006420: 706d 6172 6769 6e20 2020 2020 2020 2020  pmargin         
-00006430: 2020 2020 2020 3d20 320a 2020 2020 2020        = 2.      
-00006440: 2020 2362 6f74 6d61 7267 696e 0909 3d20    #botmargin..= 
-00006450: 390a 2020 2020 2020 2020 2362 6f74 726f  9.        #botro
-00006460: 7709 0909 3d20 726f 7773 202d 2062 6f74  w...= rows - bot
-00006470: 6d61 7267 696e 0a0a 2020 2020 2020 2020  margin..        
-00006480: 2320 436f 6d70 7574 6520 7363 7265 656e  # Compute screen
-00006490: 2073 697a 6520 616e 6420 6469 7370 6c61   size and displa
-000064a0: 7920 6865 6164 6572 732e 2020 5765 2077  y headers.  We w
-000064b0: 616e 7420 6365 6c6c 7320 6120 6269 7420  ant cells a bit 
-000064c0: 6869 6768 6572 2074 6861 6e20 7769 6465  higher than wide
-000064d0: 2c20 616e 6420 6174 0a20 2020 2020 2020  , and at.       
-000064e0: 2023 206c 6561 7374 2032 3020 6368 6172   # least 20 char
-000064f0: 6163 7465 7273 2077 6964 652e 2020 4b65  acters wide.  Ke
-00006500: 6570 2070 696c 696e 6720 2774 696c 2077  ep piling 'til w
-00006510: 6520 6172 6520 6569 7468 6572 206f 7665  e are either ove
-00006520: 7220 3230 2063 6861 7261 6374 6572 7320  r 20 characters 
-00006530: 7769 6465 2c20 6f72 206c 6573 730a 2020  wide, or less.  
-00006540: 2020 2020 2020 2320 7468 616e 2035 2f34        # than 5/4
-00006550: 7468 7320 6173 2068 6967 6820 6173 2077  ths as high as w
-00006560: 6964 652e 2020 4966 2077 6520 6361 6e27  ide.  If we can'
-00006570: 7420 6669 6e64 2061 2077 6179 2074 6f20  t find a way to 
-00006580: 6765 7420 6365 6c6c 7320 3e3d 2031 3020  get cells >= 10 
-00006590: 726f 7773 2068 6967 682c 2066 6169 6c0a  rows high, fail.
-000065a0: 2020 2020 2020 2020 2320 616e 6420 6c6f          # and lo
-000065b0: 6f70 2027 7469 6c20 7468 6579 2066 6978  op 'til they fix
-000065c0: 2074 6865 2064 6973 706c 6179 2073 697a   the display siz
-000065d0: 652e 0a20 2020 2020 2020 2074 7279 3a0a  e..        try:.
-000065e0: 2020 2020 2020 2020 2020 2020 6172 6561              area
-000065f0: 7309 093d 206c 656e 2820 696e 636c 7564  s..= len( includ
-00006600: 6520 290a 2020 2020 2020 2020 2020 2020  e ).            
-00006610: 6163 726f 7373 0909 3d20 310a 2020 2020  across..= 1.    
-00006620: 2020 2020 2020 2020 7261 6e6b 0909 3d20          rank..= 
-00006630: 310a 0a20 2020 2020 2020 2020 2020 2064  1..            d
-00006640: 6566 2063 656c 6c79 7828 293a 0a20 2020  ef cellyx():.   
-00006650: 2020 2020 2020 2020 2020 2020 2079 0909               y..
-00006660: 3d20 2820 726f 7773 202d 2074 6f70 6d61  = ( rows - topma
-00006670: 7267 696e 2029 202f 2f20 7261 6e6b 0a20  rgin ) // rank. 
-00006680: 2020 2020 2020 2020 2020 2020 2020 2078                 x
-00006690: 0909 3d20 636f 6c73 202f 2f20 6163 726f  ..= cols // acro
-000066a0: 7373 0a20 2020 2020 2020 2020 2020 2020  ss.             
-000066b0: 2020 2072 6574 7572 6e20 792c 780a 0a20     return y,x.. 
-000066c0: 2020 2020 2020 2020 2020 2068 6569 6768             heigh
-000066d0: 742c 7769 6474 6809 3d20 6365 6c6c 7978  t,width.= cellyx
-000066e0: 2829 0a20 2020 2020 2020 2020 2020 2077  ().            w
-000066f0: 6869 6c65 2077 6964 7468 203e 2036 303a  hile width > 60:
-00006700: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006710: 2061 6372 6f73 7309 2020 2020 2020 202b   across.       +
-00006720: 3d20 310a 2020 2020 2020 2020 2020 2020  = 1.            
-00006730: 2020 2020 6865 6967 6874 2c77 6964 7468      height,width
-00006740: 093d 2063 656c 6c79 7828 290a 2020 2020  .= cellyx().    
-00006750: 2020 2020 2020 2020 7768 696c 6520 6865          while he
-00006760: 6967 6874 203e 2032 303a 0a20 2020 2020  ight > 20:.     
-00006770: 2020 2020 2020 2020 2020 2072 616e 6b09             rank.
-00006780: 2020 2020 2020 202b 3d20 310a 2020 2020         += 1.    
-00006790: 2020 2020 2020 2020 2020 2020 6865 6967              heig
-000067a0: 6874 2c77 6964 7468 093d 2063 656c 6c79  ht,width.= celly
-000067b0: 7828 290a 2020 2020 2020 2020 2020 2020  x().            
-000067c0: 6173 7365 7274 2068 6569 6768 7420 3e3d  assert height >=
-000067d0: 2031 3020 616e 6420 7769 6474 6820 3e3d   10 and width >=
-000067e0: 2033 300a 2020 2020 2020 2020 6578 6365   30.        exce
-000067f0: 7074 2045 7863 6570 7469 6f6e 3a0a 2020  pt Exception:.  
-00006800: 2020 2020 2020 2020 2020 6d65 7373 6167            messag
-00006810: 6528 2077 696e 2c20 2249 6e73 7566 6669  e( win, "Insuffi
-00006820: 6369 656e 7420 7363 7265 656e 2073 697a  cient screen siz
-00006830: 6520 2825 6420 6172 6561 732c 2025 6420  e (%d areas, %d 
-00006840: 7261 6e6b 7320 6f66 2025 6420 2025 6478  ranks of %d  %dx
-00006850: 2564 2063 656c 6c73 293b 2069 6e63 7265  %d cells); incre
-00006860: 6173 6520 6865 6967 6874 2f77 6964 7468  ase height/width
-00006870: 2c20 6f72 2072 6564 7563 6520 666f 6e74  , or reduce font
-00006880: 2073 697a 6522 2025 2028 0a20 2020 2020   size" % (.     
-00006890: 2020 2020 2020 2020 2020 2061 7265 6173             areas
-000068a0: 2c20 7261 6e6b 2c20 6163 726f 7373 2c20  , rank, across, 
-000068b0: 7769 6474 682c 2068 6569 6768 7420 292c  width, height ),
-000068c0: 2063 6f6c 203d 2030 2c20 726f 7720 3d20   col = 0, row = 
-000068d0: 3020 290a 2020 2020 2020 2020 2020 2020  0 ).            
-000068e0: 7769 6e2e 7265 6672 6573 6828 290a 2020  win.refresh().  
-000068f0: 2020 2020 2020 2020 2020 7469 6d65 2e73            time.s
-00006900: 6c65 6570 2820 3220 290a 2020 2020 2020  leep( 2 ).      
-00006910: 2020 2020 2020 636f 6e74 696e 7565 0a0a        continue..
-00006920: 2020 2020 2020 2020 2320 4d61 6b65 2068          # Make h
-00006930: 2d20 616e 6420 762d 6261 7273 2c20 6576  - and v-bars, ev
-00006940: 6572 7977 6865 7265 2065 7863 6570 7420  erywhere except 
-00006950: 746f 7020 6d61 7267 696e 0a20 2020 2020  top margin.     
-00006960: 2020 2066 6f72 2072 2069 6e20 7261 6e67     for r in rang
-00006970: 6528 2074 6f70 6d61 7267 696e 2c20 726f  e( topmargin, ro
-00006980: 7773 2029 3a0a 2020 2020 2020 2020 2020  ws ):.          
-00006990: 2020 6966 2028 2072 6f77 7320 2d20 7220    if ( rows - r 
-000069a0: 2920 2520 6865 6967 6874 203d 3d20 303a  ) % height == 0:
-000069b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000069c0: 2077 696e 2e68 6c69 6e65 2820 722c 2030   win.hline( r, 0
-000069d0: 2c20 6375 7273 6573 2e41 4353 5f48 4c49  , curses.ACS_HLI
-000069e0: 4e45 2c20 636f 6c73 2029 0a20 2020 2020  NE, cols ).     
-000069f0: 2020 2066 6f72 2063 2069 6e20 7261 6e67     for c in rang
-00006a00: 6528 2077 6964 7468 2c20 636f 6c73 2c20  e( width, cols, 
-00006a10: 7769 6474 6829 3a0a 2020 2020 2020 2020  width):.        
-00006a20: 2020 2020 7769 6e2e 766c 696e 6528 2074      win.vline( t
-00006a30: 6f70 6d61 7267 696e 2c20 632c 2063 7572  opmargin, c, cur
-00006a40: 7365 732e 4143 535f 564c 494e 452c 2072  ses.ACS_VLINE, r
-00006a50: 6f77 7320 2d20 746f 706d 6172 6769 6e20  ows - topmargin 
-00006a60: 290a 0a20 2020 2020 2020 2023 2055 7064  )..        # Upd
-00006a70: 6174 650a 2020 2020 2020 2020 7769 6e73  ate.        wins
-00006a80: 656c 2e65 7261 7365 2829 0a20 2020 2020  el.erase().     
-00006a90: 2020 2077 7372 6f77 732c 2077 7363 6f6c     wsrows, wscol
-00006aa0: 7309 093d 2077 696e 7365 6c2e 6765 746d  s..= winsel.getm
-00006ab0: 6178 7978 2829 0a0a 2020 2020 2020 2020  axyx()..        
-00006ac0: 7209 0909 3d20 320a 2020 2020 2020 2020  r...= 2.        
-00006ad0: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
-00006ae0: 2077 696e 7365 6c2e 686c 696e 6528 2072   winsel.hline( r
-00006af0: 2c20 312c 2063 7572 7365 732e 4143 535f  , 1, curses.ACS_
-00006b00: 484c 494e 452c 2077 7363 6f6c 7320 2d20  HLINE, wscols - 
-00006b10: 3220 290a 2020 2020 2020 2020 6578 6365  2 ).        exce
-00006b20: 7074 2045 7863 6570 7469 6f6e 3a0a 2020  pt Exception:.  
-00006b30: 2020 2020 2020 2020 2020 7061 7373 0a20            pass. 
-00006b40: 2020 2020 2020 2072 2020 2020 2020 2020         r        
-00006b50: 2020 2020 2020 2020 2020 2020 2020 2b3d                +=
-00006b60: 2031 0a0a 2020 2020 2020 2020 7472 793a   1..        try:
-00006b70: 0a20 2020 2020 2020 2020 2020 2077 696e  .            win
-00006b80: 7365 6c2e 686c 696e 6528 2072 2c20 312c  sel.hline( r, 1,
-00006b90: 2063 7572 7365 732e 4143 535f 484c 494e   curses.ACS_HLIN
-00006ba0: 452c 2077 7363 6f6c 7320 2d20 3220 290a  E, wscols - 2 ).
-00006bb0: 2020 2020 2020 2020 6578 6365 7074 2045          except E
-00006bc0: 7863 6570 7469 6f6e 3a0a 2020 2020 2020  xception:.      
-00006bd0: 2020 2020 2020 7061 7373 0a20 2020 2020        pass.     
-00006be0: 2020 2072 2020 2020 2020 2020 2020 2020     r            
-00006bf0: 2020 2020 2020 2020 2020 2b3d 2031 0a0a            += 1..
-00006c00: 2020 2020 2020 2020 7769 6e73 656c 2e62          winsel.b
-00006c10: 6f72 6465 7228 2030 2029 0a0a 2020 2020  order( 0 )..    
-00006c20: 2320 4669 6e61 6c20 7265 6672 6573 6820  # Final refresh 
-00006c30: 2869 6e20 6361 7365 206f 6620 6572 726f  (in case of erro
-00006c40: 7220 6d65 7373 6167 6529 0a20 2020 2077  r message).    w
-00006c50: 696e 2e72 6566 7265 7368 2829 0a0a 0a64  in.refresh()...d
-00006c60: 6566 2064 6564 7563 655f 656e 636f 6469  ef deduce_encodi
-00006c70: 6e67 2820 6176 6169 6c61 626c 652c 2065  ng( available, e
-00006c80: 6e76 6972 6f6e 2c20 6163 6365 7074 3d4e  nviron, accept=N
-00006c90: 6f6e 6520 293a 0a20 2020 2022 2222 4465  one ):.    """De
-00006ca0: 6475 6365 2061 6363 6570 7461 626c 6520  duce acceptable 
-00006cb0: 656e 636f 6469 6e67 2066 726f 6d20 4854  encoding from HT
-00006cc0: 5450 2041 6363 6570 743a 2068 6561 6465  TP Accept: heade
-00006cd0: 723a 0a0a 2020 2020 2020 2020 4163 6365  r:..        Acce
-00006ce0: 7074 3a20 7465 7874 2f68 746d 6c2c 6170  pt: text/html,ap
-00006cf0: 706c 6963 6174 696f 6e2f 7868 746d 6c2b  plication/xhtml+
-00006d00: 786d 6c2c 6170 706c 6963 6174 696f 6e2f  xml,application/
-00006d10: 786d 6c3b 713d 302e 392c 2a2f 2a3b 713d  xml;q=0.9,*/*;q=
-00006d20: 302e 380a 0a20 2020 2049 6620 6974 2072  0.8..    If it r
-00006d30: 656d 6169 6e73 204e 6f6e 6520 286f 7220  emains None (or 
-00006d40: 7468 6520 7375 7070 6c69 6564 206f 6e65  the supplied one
-00006d50: 2069 7320 756e 7265 636f 676e 697a 6564   is unrecognized
-00006d60: 292c 2074 6865 0a20 2020 2063 616c 6c65  ), the.    calle
-00006d70: 7220 7368 6f75 6c64 2066 6169 6c20 746f  r should fail to
-00006d80: 2070 726f 6475 6365 2074 6865 2064 6573   produce the des
-00006d90: 6972 6564 2063 6f6e 7465 6e74 2c20 616e  ired content, an
-00006da0: 6420 7265 7475 726e 2061 6e0a 2020 2020  d return an.    
-00006db0: 4854 4d4c 2073 7461 7475 7320 636f 6465  HTML status code
-00006dc0: 2034 3036 204e 6f74 2041 6363 6570 7461   406 Not Accepta
-00006dd0: 626c 652e 0a0a 2020 2020 4966 206e 6f20  ble...    If no 
-00006de0: 4163 6365 7074 3a20 656e 636f 6469 6e67  Accept: encoding
-00006df0: 2069 7320 7375 7070 6c69 6564 2069 6e20   is supplied in 
-00006e00: 7468 6520 656e 7669 726f 6e2c 2074 6865  the environ, the
-00006e10: 2064 6566 6175 6c74 0a20 2020 2028 6669   default.    (fi
-00006e20: 7273 7429 2065 6e63 6f64 696e 6720 696e  rst) encoding in
-00006e30: 206f 7264 6572 2069 7320 7573 6564 2e0a   order is used..
-00006e40: 0a20 2020 2057 6520 646f 6e27 7420 7465  .    We don't te
-00006e50: 7374 2061 2073 7570 706c 6965 6420 2761  st a supplied 'a
-00006e60: 6363 6570 7427 2065 6e63 6f64 696e 6720  ccept' encoding 
-00006e70: 6167 6169 6e73 7420 7468 6520 4854 5450  against the HTTP
-00006e80: 5f41 4343 4550 540a 2020 2020 7365 7474  _ACCEPT.    sett
-00006e90: 696e 6773 2c20 6265 6361 7573 6520 6365  ings, because ce
-00006ea0: 7274 6169 6e20 5552 4c73 2068 6176 6520  rtain URLs have 
-00006eb0: 6120 6669 7865 6420 656e 636f 6469 6e67  a fixed encoding
-00006ec0: 2e20 2046 6f72 0a20 2020 2065 7861 6d70  .  For.    examp
-00006ed0: 6c65 2c20 2f73 6f6d 652f 7572 6c2f 626c  le, /some/url/bl
-00006ee0: 6168 2e6a 736f 6e20 616c 7761 7973 2077  ah.json always w
-00006ef0: 616e 7473 2074 6f20 7265 7475 726e 0a20  ants to return. 
-00006f00: 2020 2022 6170 706c 6963 6174 696f 6e2f     "application/
-00006f10: 6a73 6f6e 222c 2072 6567 6172 646c 6573  json", regardles
-00006f20: 7320 6f66 2077 6865 7468 6572 2074 6865  s of whether the
-00006f30: 2062 726f 7773 6572 2773 2041 6363 6570   browser's Accep
-00006f40: 743a 0a20 2020 2068 6561 6465 7220 696e  t:.    header in
-00006f50: 6469 6361 7465 7320 6974 2069 7320 6163  dicates it is ac
-00006f60: 6365 7074 6162 6c65 2e20 2057 6520 2a64  ceptable.  We *d
-00006f70: 6f2a 2068 6f77 6576 6572 2074 6573 7420  o* however test 
-00006f80: 7468 650a 2020 2020 7375 7070 6c69 6564  the.    supplied
-00006f90: 2027 6163 6365 7074 2720 656e 636f 6469   'accept' encodi
-00006fa0: 6e67 2061 6761 696e 7374 2074 6865 2027  ng against the '
-00006fb0: 6176 6169 6c61 626c 6527 2065 6e63 6f64  available' encod
-00006fc0: 696e 6773 2c0a 2020 2020 6265 6361 7573  ings,.    becaus
-00006fd0: 6520 7468 6573 6520 6172 6520 7468 6520  e these are the 
-00006fe0: 6f6e 6c79 206f 6e65 7320 6b6e 6f77 6e20  only ones known 
-00006ff0: 746f 2074 6865 2063 616c 6c65 722e 0a0a  to the caller...
-00007000: 2020 2020 4f74 6865 7277 6973 652c 2072      Otherwise, r
-00007010: 6574 7572 6e20 7468 6520 6669 7273 7420  eturn the first 
-00007020: 6163 6365 7074 6162 6c65 2065 6e63 6f64  acceptable encod
-00007030: 696e 6720 696e 2027 6176 6169 6c61 626c  ing in 'availabl
-00007040: 6527 2e0a 0a20 2020 2022 2222 0a20 2020  e'...    """.   
-00007050: 2069 6620 6163 6365 7074 3a0a 2020 2020   if accept:.    
-00007060: 2020 2020 2320 4120 6465 7369 7265 6420      # A desired 
-00007070: 656e 636f 6469 6e67 3b20 6d61 6b65 2073  encoding; make s
-00007080: 7572 6520 6974 2069 7320 6176 6169 6c61  ure it is availa
-00007090: 626c 650a 2020 2020 2020 2020 6163 6365  ble.        acce
-000070a0: 7074 0909 3d20 6163 6365 7074 2e6c 6f77  pt..= accept.low
-000070b0: 6572 2829 0a20 2020 2020 2020 2069 6620  er().        if 
-000070c0: 6163 6365 7074 206e 6f74 2069 6e20 6176  accept not in av
-000070d0: 6169 6c61 626c 653a 0a20 2020 2020 2020  ailable:.       
-000070e0: 2020 2020 2061 6363 6570 7409 3d20 4e6f       accept.= No
-000070f0: 6e65 0a20 2020 2020 2020 2072 6574 7572  ne.        retur
-00007100: 6e20 6163 6365 7074 0a0a 2020 2020 2320  n accept..    # 
-00007110: 4e6f 2070 7265 6465 6669 6e65 6420 6163  No predefined ac
-00007120: 6365 7074 2065 6e63 6f64 696e 673b 2064  cept encoding; d
-00007130: 6564 7563 6520 7072 6566 6572 7265 6420  educe preferred 
-00007140: 6176 6169 6c61 626c 6520 6f6e 652e 0a20  available one.. 
-00007150: 2020 2023 2041 6363 6570 743a 206d 6179     # Accept: may
-00007160: 2063 6f6e 7461 696e 202a 2f2a 2c20 2a2f   contain */*, */
-00007170: 6a73 6f6e 2c20 6574 632e 2020 4966 206d  json, etc.  If m
-00007180: 756c 7469 706c 6520 6d61 7463 6865 732c  ultiple matches,
-00007190: 0a20 2020 2023 2073 656c 6563 7420 7468  .    # select th
-000071a0: 6520 6f6e 6520 7769 7468 2074 6865 2068  e one with the h
-000071b0: 6967 6865 7374 2041 6363 6570 743a 2071  ighest Accept: q
-000071c0: 7561 6c69 7479 2076 616c 7565 2028 6f75  uality value (ou
-000071d0: 720a 2020 2020 2320 7072 6573 656e 7420  r.    # present 
-000071e0: 4e6f 6e65 2073 7461 7274 7320 7769 7468  None starts with
-000071f0: 2061 2071 7561 6c69 7479 206d 6574 7269   a quality metri
-00007200: 6320 6f66 2030 2e30 292e 2020 5465 7374  c of 0.0).  Test
-00007210: 0a20 2020 2023 2061 7661 696c 6162 6c65  .    # available
-00007220: 3a20 5b22 6170 706c 6963 6174 696f 6e2f  : ["application/
-00007230: 6a73 6f6e 222c 2022 7465 7874 2f68 746d  json", "text/htm
-00007240: 6c22 5d2c 2076 732e 2048 5454 505f 4143  l"], vs. HTTP_AC
-00007250: 4345 5054 0a20 2020 2023 2022 7465 7874  CEPT.    # "text
-00007260: 2f68 746d 6c2c 6170 706c 6963 6174 696f  /html,applicatio
-00007270: 6e2f 7868 746d 6c2b 786d 6c2c 6170 706c  n/xhtml+xml,appl
-00007280: 6963 6174 696f 6e2f 786d 6c3b 713d 302e  ication/xml;q=0.
-00007290: 392c 2a2f 2a3b 713d 302e 3822 0a20 2020  9,*/*;q=0.8".   
-000072a0: 2023 2053 696e 6365 2065 6172 6c69 6572   # Since earlier
-000072b0: 206d 6174 6368 6573 2061 7265 2074 6865   matches are the
-000072c0: 2066 6f72 206d 6f72 6520 7072 6566 6572   for more prefer
-000072d0: 7265 6420 656e 636f 6469 6e67 732c 0a20  red encodings,. 
-000072e0: 2020 2023 206c 6174 6572 206d 6174 6368     # later match
-000072f0: 6573 206d 7573 7420 2a65 7863 6565 642a  es must *exceed*
-00007300: 2074 6865 2071 7561 6c69 7479 206d 6574   the quality met
-00007310: 7269 6320 6f66 2074 6865 2065 6172 6c69  ric of the earli
-00007320: 6572 2e0a 2020 2020 4854 5450 5f41 4343  er..    HTTP_ACC
-00007330: 4550 5409 093d 2065 6e76 6972 6f6e 2e67  EPT..= environ.g
-00007340: 6574 2820 2248 5454 505f 4143 4345 5054  et( "HTTP_ACCEPT
-00007350: 222c 2022 2a2f 2a22 2029 2e6c 6f77 6572  ", "*/*" ).lower
-00007360: 2829 2069 6620 656e 7669 726f 6e20 656c  () if environ el
-00007370: 7365 2022 2a2f 2a22 0a20 2020 2071 7561  se "*/*".    qua
-00007380: 6c69 7479 0909 3d20 302e 300a 2020 2020  lity..= 0.0.    
-00007390: 666f 7220 7374 616e 7a61 2069 6e20 4854  for stanza in HT
-000073a0: 5450 5f41 4343 4550 542e 7370 6c69 7428  TP_ACCEPT.split(
-000073b0: 2027 2c27 2029 3a0a 2020 2020 2020 2020   ',' ):.        
-000073c0: 2320 6170 706c 6963 6174 696f 6e2f 786d  # application/xm
-000073d0: 6c3b 713d 302e 390a 2020 2020 2020 2020  l;q=0.9.        
-000073e0: 7109 093d 2031 2e30 0a20 2020 2020 2020  q..= 1.0.       
-000073f0: 2066 6f72 2065 6e63 6f64 696e 6720 696e   for encoding in
-00007400: 2072 6576 6572 7365 6428 2073 7461 6e7a   reversed( stanz
-00007410: 612e 7370 6c69 7428 2027 3b27 2029 293a  a.split( ';' )):
-00007420: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00007430: 656e 636f 6469 6e67 2e73 7461 7274 7377  encoding.startsw
-00007440: 6974 6828 2022 713d 2220 293a 0a20 2020  ith( "q=" ):.   
-00007450: 2020 2020 2020 2020 2020 2020 2071 093d               q.=
-00007460: 2066 6c6f 6174 2820 656e 636f 6469 6e67   float( encoding
-00007470: 5b32 3a5d 2029 0a20 2020 2020 2020 2066  [2:] ).        f
-00007480: 6f72 2061 7661 696c 2069 6e20 6176 6169  or avail in avai
-00007490: 6c61 626c 653a 0a20 2020 2020 2020 2020  lable:.         
-000074a0: 2020 206d 6174 6368 093d 2054 7275 650a     match.= True.
-000074b0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-000074c0: 612c 2074 2069 6e20 7a69 7028 2061 7661  a, t in zip( ava
-000074d0: 696c 2e73 706c 6974 2820 272f 2720 292c  il.split( '/' ),
-000074e0: 2065 6e63 6f64 696e 672e 7370 6c69 7428   encoding.split(
-000074f0: 2027 2f27 2029 293a 0a20 2020 2020 2020   '/' )):.       
-00007500: 2020 2020 2020 2020 2069 6620 6120 213d           if a !=
-00007510: 2074 2061 6e64 2074 2021 3d20 272a 273a   t and t != '*':
-00007520: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007530: 2020 2020 206d 6174 6368 203d 2046 616c       match = Fal
-00007540: 7365 0a20 2020 2020 2020 2020 2020 2069  se.            i
-00007550: 6620 6d61 7463 683a 0a20 2020 2020 2020  f match:.       
-00007560: 2020 2020 2020 2020 2069 6620 7120 3e20           if q > 
-00007570: 7175 616c 6974 793a 0a20 2020 2020 2020  quality:.       
-00007580: 2020 2020 2020 2020 2020 2020 2071 7561               qua
-00007590: 6c69 7479 093d 2071 0a20 2020 2020 2020  lity.= q.       
-000075a0: 2020 2020 2020 2020 2020 2020 2061 6363               acc
-000075b0: 6570 7409 3d20 6176 6169 6c0a 2020 2020  ept.= avail.    
-000075c0: 7265 7475 726e 2061 6363 6570 740a 0a0a  return accept...
-000075d0: 6465 6620 6874 7470 5f65 7863 6570 7469  def http_excepti
-000075e0: 6f6e 2820 6672 616d 6577 6f72 6b2c 2073  on( framework, s
-000075f0: 7461 7475 732c 206d 6573 7361 6765 2029  tatus, message )
-00007600: 3a0a 2020 2020 2222 2252 6574 7572 6e20  :.    """Return 
-00007610: 616e 2065 7863 6570 7469 6f6e 2061 7070  an exception app
-00007620: 726f 7072 6961 7465 2066 6f72 2074 6865  ropriate for the
-00007630: 2067 6976 656e 2077 6562 2066 7261 6d65   given web frame
-00007640: 776f 726b 2c0a 2020 2020 656e 636f 6469  work,.    encodi
-00007650: 6e67 2074 6865 2048 5454 5020 7374 6174  ng the HTTP stat
-00007660: 7573 2063 6f64 6520 616e 6420 6d65 7373  us code and mess
-00007670: 6167 6520 7072 6f76 6964 6564 2e0a 2020  age provided..  
-00007680: 2020 2222 220a 2020 2020 6966 2066 7261    """.    if fra
-00007690: 6d65 776f 726b 2061 6e64 2066 7261 6d65  mework and frame
-000076a0: 776f 726b 2e5f 5f6e 616d 655f 5f20 3d3d  work.__name__ ==
-000076b0: 2022 7765 6222 3a0a 2020 2020 2020 2020   "web":.        
-000076c0: 6966 2073 7461 7475 7320 3d3d 2034 3034  if status == 404
-000076d0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-000076e0: 7475 726e 2066 7261 6d65 776f 726b 2e4e  turn framework.N
-000076f0: 6f74 466f 756e 6428 206d 6573 7361 6765  otFound( message
-00007700: 2029 0a0a 2020 2020 2020 2020 6966 2073   )..        if s
-00007710: 7461 7475 7320 3d3d 2034 3036 3a0a 2020  tatus == 406:.  
-00007720: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00007730: 2066 7261 6d65 776f 726b 2e4e 6f74 4163   framework.NotAc
-00007740: 6365 7074 6162 6c65 2829 0909 0923 2057  ceptable()...# W
-00007750: 696c 6c20 6e6f 7420 6163 6365 7074 2061  ill not accept a
-00007760: 206d 6573 7361 6765 0a0a 2020 2020 7265   message..    re
-00007770: 7475 726e 2045 7863 6570 7469 6f6e 2820  turn Exception( 
-00007780: 2225 6420 2573 2220 2520 2820 7374 6174  "%d %s" % ( stat
-00007790: 7573 2c20 6d65 7373 6167 6520 2929 0a0a  us, message ))..
-000077a0: 0a64 6566 206c 6963 656e 7365 735f 7265  .def licenses_re
-000077b0: 7175 6573 7428 2072 656e 6465 722c 2070  quest( render, p
-000077c0: 6174 682c 2065 6e76 6972 6f6e 2c20 6163  ath, environ, ac
-000077d0: 6365 7074 2c20 6672 616d 6577 6f72 6b2c  cept, framework,
-000077e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000077f0: 2020 2020 2020 2020 2020 7175 6572 6965            querie
-00007800: 733d 4e6f 6e65 2c20 706f 7374 6564 3d4e  s=None, posted=N
-00007810: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
-00007820: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00007830: 7373 696f 6e3d 4e6f 6e65 2c20 6c6f 6767  ssion=None, logg
-00007840: 6564 3d4e 6f6e 652c 0909 2320 5468 6520  ed=None,..# The 
-00007850: 7573 6572 2073 6573 7369 6f6e 0a20 2020  user session.   
-00007860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007870: 2020 2020 2020 7072 6f78 793d 4e6f 6e65        proxy=None
-00007880: 2029 3a0a 0a20 2020 2022 2222 0a20 2020   ):..    """.   
-00007890: 2020 2020 2061 7069 2f6c 6963 656e 7365       api/license
-000078a0: 732f 3c6e 616d 653e 2f0a 0a20 2020 2022  s/<name>/..    "
-000078b0: 2222 0a20 2020 2076 6172 6961 626c 6573  "".    variables
-000078c0: 0909 093d 2071 7565 7269 6573 206f 7220  ...= queries or 
-000078d0: 706f 7374 6564 206f 7220 7b7d 0a20 2020  posted or {}.   
-000078e0: 2063 6f6e 7465 6e74 0909 093d 2064 6564   content...= ded
-000078f0: 7563 655f 656e 636f 6469 6e67 2820 5b20  uce_encoding( [ 
-00007900: 2274 6578 742f 6874 6d6c 222c 0a20 2020  "text/html",.   
-00007910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007940: 2020 2261 7070 6c69 6361 7469 6f6e 2f6a    "application/j
-00007950: 736f 6e22 2c20 2274 6578 742f 6a61 7661  son", "text/java
-00007960: 7363 7269 7074 222c 0a20 2020 2020 2020  script",.       
+000001c0: 6f6e 2e20 2049 7420 6973 2061 6c73 6f20  on.  It is also 
+000001d0: 6176 6169 6c61 626c 6520 756e 6465 7220  available under 
+000001e0: 616c 7465 726e 6174 6976 6520 2865 672e  alternative (eg.
+000001f0: 2043 6f6d 6d65 7263 6961 6c29 0a23 206c   Commercial).# l
+00000200: 6963 656e 7365 732c 2061 7420 796f 7572  icenses, at your
+00000210: 206f 7074 696f 6e2e 2020 5365 6520 7468   option.  See th
+00000220: 6520 4c49 4345 4e53 4520 6669 6c65 2061  e LICENSE file a
+00000230: 7420 7468 6520 746f 7020 6f66 2074 6865  t the top of the
+00000240: 2073 6f75 7263 6520 7472 6565 2e0a 230a   source tree..#.
+00000250: 2320 4974 2069 7320 6469 7374 7269 6275  # It is distribu
+00000260: 7465 6420 696e 2074 6865 2068 6f70 6520  ted in the hope 
+00000270: 7468 6174 2069 7420 7769 6c6c 2062 6520  that it will be 
+00000280: 7573 6566 756c 2c20 6275 7420 5749 5448  useful, but WITH
+00000290: 4f55 5420 414e 590a 2320 5741 5252 414e  OUT ANY.# WARRAN
+000002a0: 5459 3b20 7769 7468 6f75 7420 6576 656e  TY; without even
+000002b0: 2074 6865 2069 6d70 6c69 6564 2077 6172   the implied war
+000002c0: 7261 6e74 7920 6f66 204d 4552 4348 414e  ranty of MERCHAN
+000002d0: 5441 4249 4c49 5459 206f 7220 4649 544e  TABILITY or FITN
+000002e0: 4553 5320 464f 520a 2320 4120 5041 5254  ESS FOR.# A PART
+000002f0: 4943 554c 4152 2050 5552 504f 5345 2e20  ICULAR PURPOSE. 
+00000300: 2053 6565 2074 6865 2047 4e55 2047 656e   See the GNU Gen
+00000310: 6572 616c 2050 7562 6c69 6320 4c69 6365  eral Public Lice
+00000320: 6e73 6520 666f 7220 6d6f 7265 2064 6574  nse for more det
+00000330: 6169 6c73 2e0a 230a 0a22 2222 0a20 2020  ails..#..""".   
+00000340: 2049 6d70 6c65 6d65 6e74 7320 7468 6520   Implements the 
+00000350: 4372 7970 746f 204c 6963 656e 7369 6e67  Crypto Licensing
+00000360: 2073 6572 7665 720a 2222 220a 0a66 726f   server."""..fro
+00000370: 6d20 5f5f 6675 7475 7265 5f5f 2069 6d70  m __future__ imp
+00000380: 6f72 7420 7072 696e 745f 6675 6e63 7469  ort print_functi
+00000390: 6f6e 2c20 6162 736f 6c75 7465 5f69 6d70  on, absolute_imp
+000003a0: 6f72 742c 2064 6976 6973 696f 6e0a 0a69  ort, division..i
+000003b0: 6d70 6f72 7420 6172 6770 6172 7365 0a69  mport argparse.i
+000003c0: 6d70 6f72 7420 6375 7273 6573 2c20 6375  mport curses, cu
+000003d0: 7273 6573 2e61 7363 6969 2c20 6375 7273  rses.ascii, curs
+000003e0: 6573 2e70 616e 656c 2020 2320 6e6f 7161  es.panel  # noqa
+000003f0: 3a20 4534 3031 0a69 6d70 6f72 7420 666e  : E401.import fn
+00000400: 6d61 7463 680a 696d 706f 7274 206a 736f  match.import jso
+00000410: 6e0a 696d 706f 7274 206c 6f67 6769 6e67  n.import logging
+00000420: 0a69 6d70 6f72 7420 6f73 0a69 6d70 6f72  .import os.impor
+00000430: 7420 706f 7369 7870 6174 680a 696d 706f  t posixpath.impo
+00000440: 7274 2073 6967 6e61 6c0a 696d 706f 7274  rt signal.import
+00000450: 2073 716c 6974 6533 0a69 6d70 6f72 7420   sqlite3.import 
+00000460: 7379 730a 696d 706f 7274 2074 6872 6561  sys.import threa
+00000470: 6469 6e67 0a69 6d70 6f72 7420 7469 6d65  ding.import time
+00000480: 0a69 6d70 6f72 7420 7472 6163 6562 6163  .import tracebac
+00000490: 6b0a 696d 706f 7274 2077 6172 6e69 6e67  k.import warning
+000004a0: 730a 0a23 2055 7365 6420 666f 7220 5765  s..# Used for We
+000004b0: 6220 4755 492c 2061 6e64 2066 6f72 206c  b GUI, and for l
+000004c0: 6963 656e 7369 6e67 2064 6174 6162 6173  icensing databas
+000004d0: 652e 2020 496e 2074 6865 2066 7574 7572  e.  In the futur
+000004e0: 652c 206d 7563 6820 6f66 2074 6869 7320  e, much of this 
+000004f0: 7769 6c6c 2074 7261 6e73 6974 696f 6e20  will transition 
+00000500: 746f 0a23 2048 6f6c 6f63 6861 696e 2d62  to.# Holochain-b
+00000510: 6173 6564 2069 6e66 7261 7374 7275 6374  ased infrastruct
+00000520: 7572 652e 0a69 6d70 6f72 7420 7765 620a  ure..import web.
+00000530: 696d 706f 7274 2077 6562 2e68 7474 7073  import web.https
+00000540: 6572 7665 720a 696d 706f 7274 2077 7367  erver.import wsg
+00000550: 696c 6f67 0a0a 6672 6f6d 202e 2e6d 6973  ilog..from ..mis
+00000560: 6309 0969 6d70 6f72 7420 280a 2020 2020  c..import (.    
+00000570: 7469 6d65 722c 2054 696d 6573 7461 6d70  timer, Timestamp
+00000580: 2c0a 2020 2020 6c6f 675f 6366 672c 206c  ,.    log_cfg, l
+00000590: 6f67 5f6c 6576 656c 6d61 702c 206c 6f67  og_levelmap, log
+000005a0: 5f6c 6576 656c 2c0a 2020 2020 636f 6e66  _level,.    conf
+000005b0: 6967 5f70 6174 6873 2c20 636f 6e66 6967  ig_paths, config
+000005c0: 5f6f 7065 6e2c 2043 6f6e 6669 674e 6f74  _open, ConfigNot
+000005d0: 466f 756e 6445 7272 6f72 2c0a 2020 2020  FoundError,.    
+000005e0: 756e 7175 6f74 650a 290a 6672 6f6d 202e  unquote.).from .
+000005f0: 2e09 0909 696d 706f 7274 206c 6963 656e  ....import licen
+00000600: 7369 6e67 0a66 726f 6d20 2e2e 6d69 7363  sing.from ..misc
+00000610: 0909 696d 706f 7274 2069 6e70 7574 5f73  ..import input_s
+00000620: 6563 7572 650a 0a5f 5f61 7574 686f 725f  ecure..__author_
+00000630: 5f20 2020 2020 2020 2020 2020 2020 2020  _               
+00000640: 2020 2020 2020 203d 2022 5065 7272 7920         = "Perry 
+00000650: 4b75 6e64 6572 7422 0a5f 5f65 6d61 696c  Kundert".__email
+00000660: 5f5f 2020 2020 2020 2020 2020 2020 2020  __              
+00000670: 2020 2020 2020 2020 203d 2022 7065 7272           = "perr
+00000680: 7940 646f 6d69 6e69 6f6e 726e 642e 636f  y@dominionrnd.co
+00000690: 6d22 0a5f 5f63 6f70 7972 6967 6874 5f5f  m".__copyright__
+000006a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000006b0: 2020 203d 2022 436f 7079 7269 6768 7420     = "Copyright 
+000006c0: 2863 2920 3230 3232 2044 6f6d 696e 696f  (c) 2022 Dominio
+000006d0: 6e20 5265 7365 6172 6368 2026 2044 6576  n Research & Dev
+000006e0: 656c 6f70 6d65 6e74 2043 6f72 702e 220a  elopment Corp.".
+000006f0: 5f5f 6c69 6365 6e73 655f 5f20 2020 2020  __license__     
+00000700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000710: 3d20 2244 7561 6c20 4c69 6365 6e73 653a  = "Dual License:
+00000720: 2047 504c 7633 2028 6f72 206c 6174 6572   GPLv3 (or later
+00000730: 2920 616e 6420 436f 6d6d 6572 6369 616c  ) and Commercial
+00000740: 2028 7365 6520 4c49 4345 4e53 4529 220a   (see LICENSE)".
+00000750: 0a77 6562 2e63 6f6e 6669 672e 6465 6275  .web.config.debu
+00000760: 6720 0909 3d20 4661 6c73 650a 7765 622e  g ..= False.web.
+00000770: 636f 6e66 6967 2e73 6573 7369 6f6e 5f70  config.session_p
+00000780: 6172 616d 6574 6572 732e 7570 6461 7465  arameters.update
+00000790: 2820 7b0a 2020 2020 2763 6f6f 6b69 655f  ( {.    'cookie_
+000007a0: 6e61 6d65 273a 0927 7365 7373 696f 6e27  name':.'session'
+000007b0: 2c0a 2020 2020 2769 676e 6f72 655f 6578  ,.    'ignore_ex
+000007c0: 7069 7279 273a 0954 7275 652c 0a20 2020  piry':.True,.   
+000007d0: 2027 6967 6e6f 7265 5f63 6861 6e67 655f   'ignore_change_
+000007e0: 6970 273a 0954 7275 652c 0a20 2020 2027  ip':.True,.    '
+000007f0: 7469 6d65 6f75 7427 3a09 0937 2a32 342a  timeout':..7*24*
+00000800: 3630 2a36 302c 2020 2020 2023 2031 2077  60*60,     # 1 w
+00000810: 6565 6b0a 7d20 290a 0a73 6573 7369 6f6e  eek.} )..session
+00000820: 5f69 6e69 7469 616c 697a 6572 0909 3d20  _initializer..= 
+00000830: 7b0a 2020 2020 2775 7365 725f 6964 273a  {.    'user_id':
+00000840: 0930 2c0a 2020 2020 276e 616d 6527 3a09  .0,.    'name':.
+00000850: 2727 2c0a 2020 2020 2770 696e 273a 0930  '',.    'pin':.0
+00000860: 2c0a 2020 2020 276c 6f67 696e 273a 0930  ,.    'login':.0
+00000870: 2c09 0909 2320 3020 6775 6573 742c 2031  ,...# 0 guest, 1
+00000880: 2075 7365 722c 2032 2061 646d 696e 0a7d   user, 2 admin.}
+00000890: 0a0a 0a6c 6f67 0909 0909 3d20 6c6f 6767  ...log....= logg
+000008a0: 696e 672e 6765 744c 6f67 6765 7228 2022  ing.getLogger( "
+000008b0: 6c69 6365 6e73 696e 6722 2029 0a0a 2320  licensing" )..# 
+000008c0: 4f75 7470 7574 2066 696c 6573 2061 7265  Output files are
+000008d0: 2073 746f 7265 6420 696e 2074 6865 2043   stored in the C
+000008e0: 5744 0a4c 4f47 4649 4c45 0909 0909 3d20  WD.LOGFILE....= 
+000008f0: 226c 6963 656e 7369 6e67 2e6c 6f67 220a  "licensing.log".
+00000900: 4442 5f46 494c 4509 0909 093d 2022 6c69  DB_FILE....= "li
+00000910: 6365 6e73 696e 672e 6462 220a 4143 4346  censing.db".ACCF
+00000920: 494c 4509 0909 093d 2022 6c69 6365 6e73  ILE....= "licens
+00000930: 696e 672e 6163 6365 7373 220a 0a43 5244  ing.access"..CRD
+00000940: 4649 4c45 0909 0909 3d20 226c 6963 656e  FILE....= "licen
+00000950: 7369 6e67 2e63 7265 6465 6e74 6961 6c73  sing.credentials
+00000960: 2220 2020 2020 2020 2320 416e 7920 6175  "       # Any au
+00000970: 7468 6f72 2063 7265 6465 6e74 6961 6c73  thor credentials
+00000980: 2061 7661 696c 6162 6c65 2070 6572 7369   available persi
+00000990: 7374 656e 746c 790a 4b45 5946 494c 4509  stently.KEYFILE.
+000009a0: 0909 093d 2022 6c69 6365 6e73 696e 672e  ...= "licensing.
+000009b0: 2220 2b20 6c69 6365 6e73 696e 672e 4b45  " + licensing.KE
+000009c0: 5950 4154 5445 524e 0a4c 4943 4649 4c45  YPATTERN.LICFILE
+000009d0: 0909 0909 3d20 226c 6963 656e 7369 6e67  ....= "licensing
+000009e0: 2e22 202b 206c 6963 656e 7369 6e67 2e4c  ." + licensing.L
+000009f0: 4943 5041 5454 4552 4e0a 0a23 2053 514c  ICPATTERN..# SQL
+00000a00: 2063 6f6e 6669 6775 7261 7469 6f6e 7320   configurations 
+00000a10: 6172 6520 7479 7069 6361 6c6c 7920 666f  are typically fo
+00000a20: 756e 6420 696e 2063 7279 7074 6f5f 6c69  und in crypto_li
+00000a30: 6365 6e73 696e 672f 6c69 6365 6e73 696e  censing/licensin
+00000a40: 672c 2062 7574 206d 6179 2062 6520 6375  g, but may be cu
+00000a50: 7374 6f6d 697a 6564 2061 6e64 0a23 2070  stomized and.# p
+00000a60: 6c61 6365 6420 696e 2061 6e79 206f 6620  laced in any of 
+00000a70: 7468 6520 4370 7070 6f20 636f 6e66 6967  the Cpppo config
+00000a80: 7572 6174 696f 6e20 6669 6c65 2070 6174  uration file pat
+00000a90: 6873 2028 6567 2e20 7e2f 2e63 7070 706f  hs (eg. ~/.cpppo
+00000aa0: 2f2c 202f 6574 632f 6370 7070 6f2f 2c20  /, /etc/cpppo/, 
+00000ab0: 6f72 2074 6865 2063 7572 7265 6e74 0a23  or the current.#
+00000ac0: 2077 6f72 6b69 6e67 2064 6972 6563 746f   working directo
+00000ad0: 7279 290a 5351 4c46 494c 4509 0909 093d  ry).SQLFILE....=
+00000ae0: 2022 6c69 6365 6e73 696e 672e 7371 6c22   "licensing.sql"
+00000af0: 0909 2320 7468 6973 202b 202e 2a20 6172  ..# this + .* ar
+00000b00: 6520 6c6f 6164 6564 0a0a 4f55 5250 4154  e loaded..OURPAT
+00000b10: 4809 0909 093d 206f 732e 7061 7468 2e64  H....= os.path.d
+00000b20: 6972 6e61 6d65 2820 6f73 2e70 6174 682e  irname( os.path.
+00000b30: 6162 7370 6174 6828 205f 5f66 696c 655f  abspath( __file_
+00000b40: 5f20 2929 0a54 504c 5041 5448 0909 0909  _ )).TPLPATH....
+00000b50: 3d20 6f73 2e70 6174 682e 6a6f 696e 2820  = os.path.join( 
+00000b60: 4f55 5250 4154 482c 2022 7374 6174 6963  OURPATH, "static
+00000b70: 2f72 6573 6f75 7263 6573 2f74 656d 706c  /resources/templ
+00000b80: 6174 6573 2f22 2029 0a4c 4f43 5041 5448  ates/" ).LOCPATH
+00000b90: 0909 0909 3d20 6f73 2e70 6174 682e 6162  ....= os.path.ab
+00000ba0: 7370 6174 6828 6f73 2e70 6174 682e 6375  spath(os.path.cu
+00000bb0: 7264 6972 290a 0a23 204c 6963 656e 7365  rdir)..# License
+00000bc0: 2053 6572 7665 7220 436f 6e66 6967 7572   Server Configur
+00000bd0: 6174 696f 6e0a 0a63 6f6e 6669 675f 6578  ation..config_ex
+00000be0: 7472 6173 0909 093d 205b 4f55 5250 4154  tras...= [OURPAT
+00000bf0: 485d 2020 2320 416e 7920 6578 7472 6120  H]  # Any extra 
+00000c00: 6869 6768 6572 2d70 7269 6f72 6974 7920  higher-priority 
+00000c10: 636f 6e66 6967 7572 6174 696f 6e20 7061  configuration pa
+00000c20: 7468 7320 746f 206c 6f6f 6b20 696e 0a0a  ths to look in..
+00000c30: 0a23 2054 6865 2064 6174 6162 6173 653a  .# The database:
+00000c40: 2067 6c6f 6261 6c20 2764 6227 2c20 7768   global 'db', wh
+00000c50: 6963 6820 6973 2061 2077 6562 2e64 6174  ich is a web.dat
+00000c60: 6162 6173 6520 636f 6e6e 6563 7469 6f6e  abase connection
+00000c70: 2e20 2041 6c73 6f20 2764 625f 6c6f 636b  .  Also 'db_lock
+00000c80: 272c 2073 696e 6365 2073 716c 6974 6533  ', since sqlite3
+00000c90: 2069 730a 2320 7468 7265 6164 2d73 6166   is.# thread-saf
+00000ca0: 652c 2062 7574 2077 696c 6c20 7261 6973  e, but will rais
+00000cb0: 6520 616e 2065 7863 6570 7469 6f6e 2069  e an exception i
+00000cc0: 6620 6d75 6c74 6970 6c65 2074 6872 6561  f multiple threa
+00000cd0: 6473 2061 7474 656d 7074 2074 6f20 7772  ds attempt to wr
+00000ce0: 6974 652c 2070 726f 7669 6465 2061 0a23  ite, provide a.#
+00000cf0: 2074 6872 6561 6469 6e67 2e4c 6f63 6b28   threading.Lock(
+00000d00: 2920 746f 2061 6c6c 6f77 2073 6572 6961  ) to allow seria
+00000d10: 6c69 7a69 6e67 206f 6620 616c 6c20 6462  lizing of all db
+00000d20: 2069 6e73 6572 742c 2075 7064 6174 652c   insert, update,
+00000d30: 2065 7463 2e20 6265 7477 6565 6e20 7468   etc. between th
+00000d40: 7265 6164 732e 0a0a 2320 5765 2077 696c  reads...# We wil
+00000d50: 6c20 2a61 6c77 6179 732a 2065 7865 6375  l *always* execu
+00000d60: 7465 2061 6c6c 206f 6620 7468 6520 6176  te all of the av
+00000d70: 6169 6c61 626c 6520 2e2e 2e73 716c 2a20  ailable ...sql* 
+00000d80: 7363 7269 7074 732e 2020 5468 6573 6520  scripts.  These 
+00000d90: 636f 6e74 6169 6e20 2743 5245 4154 4520  contain 'CREATE 
+00000da0: 5441 424c 4527 2061 6e64 0a23 2027 494e  TABLE' and.# 'IN
+00000db0: 5345 5254 2720 636f 6d6d 616e 6473 2c20  SERT' commands, 
+00000dc0: 7768 6963 6820 7769 6c6c 2066 6169 6c20  which will fail 
+00000dd0: 6966 2074 6865 2073 7065 6369 6669 6564  if the specified
+00000de0: 2074 6162 6c65 2f72 6f77 2061 6c72 6561   table/row alrea
+00000df0: 6479 2065 7869 7374 732c 2073 6f20 6172  dy exists, so ar
+00000e00: 6520 7361 6665 2074 6f20 7275 6e0a 2320  e safe to run.# 
+00000e10: 7265 7065 6174 6564 6c79 2e20 2057 6865  repeatedly.  Whe
+00000e20: 6e20 7765 2061 6464 2074 6162 6c65 7320  n we add tables 
+00000e30: 616e 642f 6f72 2072 6f77 7320 7468 6174  and/or rows that
+00000e40: 2064 6f6e 2774 2061 6c72 6561 6479 2065   don't already e
+00000e50: 7869 7374 2c20 7468 6579 276c 6c20 6265  xist, they'll be
+00000e60: 2063 7265 6174 6564 2062 7920 7468 6573   created by thes
+00000e70: 650a 2320 7363 7269 7074 732e 2020 5468  e.# scripts.  Th
+00000e80: 6973 2070 726f 7669 6465 7320 7573 2077  is provides us w
+00000e90: 6974 6820 6120 7275 6469 6d65 6e74 6172  ith a rudimentar
+00000ea0: 7920 6461 7461 6261 7365 2075 7064 6174  y database updat
+00000eb0: 6520 6d65 6368 616e 6973 6d20 6265 7477  e mechanism betw
+00000ec0: 6565 6e20 7265 6c65 6173 6573 2c20 6173  een releases, as
+00000ed0: 206c 6f6e 670a 2320 6173 2077 6520 6361   long.# as we ca
+00000ee0: 7265 6675 6c6c 7920 6d69 6772 6174 6520  refully migrate 
+00000ef0: 6461 7461 2066 726f 6d20 6f6c 6420 746f  data from old to
+00000f00: 206e 6577 2074 6162 6c65 732e 0a0a 0a64   new tables....d
+00000f10: 625f 7374 6174 6963 7309 0909 3d20 7b7d  b_statics...= {}
+00000f20: 0a64 625f 6c6f 636b 0909 0909 3d20 7468  .db_lock....= th
+00000f30: 7265 6164 696e 672e 4c6f 636b 2829 0a64  reading.Lock().d
+00000f40: 6209 0909 093d 204e 6f6e 650a 0a0a 6465  b....= None...de
+00000f50: 6620 6462 5f73 6574 7570 2829 3a0a 2020  f db_setup():.  
+00000f60: 2020 2222 2253 6574 2075 7020 6170 706c    """Set up appl
+00000f70: 6963 6174 696f 6e2d 676c 6f62 616c 2064  ication-global d
+00000f80: 622c 2064 625f 6c6f 636b 2c20 2e2e 2e20  b, db_lock, ... 
+00000f90: 2053 686f 756c 6420 6265 2064 6f6e 6520   Should be done 
+00000fa0: 6166 7465 7220 636f 6e66 6967 5f65 7874  after config_ext
+00000fb0: 7261 7320 6973 2069 6e69 7469 616c 697a  ras is initializ
+00000fc0: 6564 2e22 2222 0a0a 2020 2020 696e 6974  ed."""..    init
+00000fd0: 5f64 6209 0909 3d20 4e6f 6e65 0a20 2020  _db...= None.   
+00000fe0: 2064 625f 6669 6c65 5f70 6174 6809 093d   db_file_path..=
+00000ff0: 2044 425f 4649 4c45 0a20 2020 2073 716c   DB_FILE.    sql
+00001000: 6669 6c65 5f70 6174 6809 093d 2053 514c  file_path..= SQL
+00001010: 4649 4c45 0a20 2020 2074 7279 3a0a 2020  FILE.    try:.  
+00001020: 2020 2020 2020 2320 4c6f 6164 2074 6865        # Load the
+00001030: 206c 6963 656e 7369 6e67 2e64 6220 6669   licensing.db fi
+00001040: 6c65 2e20 2049 6620 6974 2063 616e 2062  le.  If it can b
+00001050: 6520 666f 756e 6420 736f 6d65 7768 6572  e found somewher
+00001060: 6520 696e 2074 6865 2063 6f6e 6669 6775  e in the configu
+00001070: 7261 7469 6f6e 2070 6174 682c 2075 7365  ration path, use
+00001080: 2069 7420 2d2d 0a20 2020 2020 2020 2023   it --.        #
+00001090: 206f 7468 6572 7769 7365 2c20 6173 7375   otherwise, assu
+000010a0: 6d65 2069 7427 7320 7375 7070 6f73 6564  me it's supposed
+000010b0: 2074 6f20 6265 2068 6572 6520 696e 2074   to be here in t
+000010c0: 6865 2043 5744 2e0a 2020 2020 2020 2020  he CWD..        
+000010d0: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+000010e0: 2066 6f72 2066 2069 6e20 636f 6e66 6967   for f in config
+000010f0: 5f6f 7065 6e28 2044 425f 4649 4c45 2029  _open( DB_FILE )
+00001100: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00001110: 2020 7769 7468 2066 3a0a 2020 2020 2020    with f:.      
+00001120: 2020 2020 2020 2020 2020 2020 2020 6462                db
+00001130: 5f66 696c 655f 7061 7468 203d 2066 2e6e  _file_path = f.n
+00001140: 616d 650a 2020 2020 2020 2020 2020 2020  ame.            
+00001150: 2020 2020 6272 6561 6b0a 2020 2020 2020      break.      
+00001160: 2020 6578 6365 7074 2043 6f6e 6669 674e    except ConfigN
+00001170: 6f74 466f 756e 6445 7272 6f72 3a0a 2020  otFoundError:.  
+00001180: 2020 2020 2020 2020 2020 7061 7373 0a20            pass. 
+00001190: 2020 2020 2020 2069 6e69 745f 6462 0909         init_db..
+000011a0: 093d 2073 716c 6974 6533 2e63 6f6e 6e65  .= sqlite3.conne
+000011b0: 6374 2820 6462 5f66 696c 655f 7061 7468  ct( db_file_path
+000011c0: 2029 0a0a 2020 2020 2020 2020 2320 4c6f   )..        # Lo
+000011d0: 6164 2061 6c6c 206c 6963 656e 7369 6e67  ad all licensing
+000011e0: 2e73 716c 2a20 636f 6e66 6967 2066 696c  .sql* config fil
+000011f0: 6573 2069 6e74 6f20 7468 6520 6c69 6365  es into the lice
+00001200: 6e73 696e 672e 6462 2053 716c 6974 6533  nsing.db Sqlite3
+00001210: 2066 696c 652e 2020 5765 2077 616e 7420   file.  We want 
+00001220: 746f 206c 6f61 640a 2020 2020 2020 2020  to load.        
+00001230: 2320 5351 4c20 6669 6c65 7320 6672 6f6d  # SQL files from
+00001240: 206d 6f73 7420 6765 6e65 7261 6c2f 6469   most general/di
+00001250: 7374 616e 7420 746f 206d 6f73 7420 7370  stant to most sp
+00001260: 6563 6966 6963 2f6e 6561 7265 7374 2c20  ecific/nearest, 
+00001270: 736f 206d 616b 6520 7265 7665 7273 653d  so make reverse=
+00001280: 4661 6c73 652e 0a20 2020 2020 2020 2067  False..        g
+00001290: 6c6f 6261 6c20 636f 6e66 6967 5f65 7874  lobal config_ext
+000012a0: 7261 0a20 2020 2020 2020 2066 6f72 2066  ra.        for f
+000012b0: 2069 6e20 636f 6e66 6967 5f6f 7065 6e28   in config_open(
+000012c0: 2053 514c 4649 4c45 2b27 2a27 2c20 6578   SQLFILE+'*', ex
+000012d0: 7472 613d 636f 6e66 6967 5f65 7874 7261  tra=config_extra
+000012e0: 732c 2073 6b69 703d 272a 7e27 2c20 7265  s, skip='*~', re
+000012f0: 7665 7273 653d 4661 6c73 6520 293a 0a20  verse=False ):. 
+00001300: 2020 2020 2020 2020 2020 2077 6974 6820             with 
+00001310: 663a 0a20 2020 2020 2020 2020 2020 2020  f:.             
+00001320: 2020 2073 716c 0909 3d20 662e 7265 6164     sql..= f.read
+00001330: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+00001340: 2020 2073 716c 5f66 696c 6509 3d20 662e     sql_file.= f.
+00001350: 6e61 6d65 0a20 2020 2020 2020 2020 2020  name.           
+00001360: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+00001370: 2020 2020 2020 6c6f 672e 696e 666f 2820        log.info( 
+00001380: 224c 6f61 6469 6e67 2053 514c 2066 726f  "Loading SQL fro
+00001390: 6d20 7b7d 222e 666f 726d 6174 2820 7371  m {}".format( sq
+000013a0: 6c5f 6669 6c65 2029 290a 2020 2020 2020  l_file )).      
+000013b0: 2020 2020 2020 2020 2020 696e 6974 5f64            init_d
+000013c0: 622e 6578 6563 7574 6573 6372 6970 7428  b.executescript(
+000013d0: 2073 716c 2029 0a20 2020 2020 2020 2020   sql ).         
+000013e0: 2020 2065 7863 6570 7420 2873 716c 6974     except (sqlit
+000013f0: 6533 2e4f 7065 7261 7469 6f6e 616c 4572  e3.OperationalEr
+00001400: 726f 722c 7371 6c69 7465 332e 496e 7465  ror,sqlite3.Inte
+00001410: 6772 6974 7945 7272 6f72 2920 6173 2065  grityError) as e
+00001420: 7863 3a0a 2020 2020 2020 2020 2020 2020  xc:.            
+00001430: 2020 2020 6c6f 672e 696e 666f 2820 2246      log.info( "F
+00001440: 6169 6c65 6420 746f 206c 6f61 6420 2573  ailed to load %s
+00001450: 2028 7072 6f62 6162 6c79 2061 6c72 6561   (probably alrea
+00001460: 6479 2063 6f6e 6669 6775 7265 642c 2063  dy configured, c
+00001470: 6f6e 7469 6e75 696e 6729 3a20 2573 222c  ontinuing): %s",
+00001480: 2073 716c 5f66 696c 652c 2065 7863 2029   sql_file, exc )
+00001490: 0a20 2020 2065 7863 6570 7420 4578 6365  .    except Exce
+000014a0: 7074 696f 6e20 6173 2065 7863 3a0a 2020  ption as exc:.  
+000014b0: 2020 2020 2020 6c6f 672e 7761 726e 696e        log.warnin
+000014c0: 6728 2022 4661 696c 6564 2074 6f20 6578  g( "Failed to ex
+000014d0: 6563 7574 6520 7b7d 2a20 7363 7269 7074  ecute {}* script
+000014e0: 7320 696e 746f 2044 4220 7b7d 3a20 7b7d  s into DB {}: {}
+000014f0: 222e 666f 726d 6174 280a 2020 2020 2020  ".format(.      
+00001500: 2020 2020 2020 7371 6c66 696c 655f 7061        sqlfile_pa
+00001510: 7468 2c20 6462 5f66 696c 655f 7061 7468  th, db_file_path
+00001520: 2c20 6578 6320 2929 0a20 2020 2020 2020  , exc )).       
+00001530: 2072 6169 7365 0a20 2020 2066 696e 616c   raise.    final
+00001540: 6c79 3a0a 2020 2020 2020 2020 6966 2069  ly:.        if i
+00001550: 6e69 745f 6462 3a0a 2020 2020 2020 2020  nit_db:.        
+00001560: 2020 2020 696e 6974 5f64 622e 636c 6f73      init_db.clos
+00001570: 6528 290a 2020 2020 6173 7365 7274 206f  e().    assert o
+00001580: 732e 6163 6365 7373 2820 6462 5f66 696c  s.access( db_fil
+00001590: 655f 7061 7468 2c20 6f73 2e57 5f4f 4b20  e_path, os.W_OK 
+000015a0: 292c 205c 0a20 2020 2020 2020 2022 4361  ), \.        "Ca
+000015b0: 6e6e 6f74 2061 6363 6573 7320 6c69 6365  nnot access lice
+000015c0: 6e73 696e 6720 4442 3a20 7b7d 222e 666f  nsing DB: {}".fo
+000015d0: 726d 6174 2820 6462 5f66 696c 655f 7061  rmat( db_file_pa
+000015e0: 7468 2029 0a0a 2020 2020 2320 4f4b 2c20  th )..    # OK, 
+000015f0: 7468 6520 4442 2068 6173 2062 6565 6e20  the DB has been 
+00001600: 696e 6974 6961 6c69 7a65 642c 2061 6e64  initialized, and
+00001610: 2069 7320 6174 2064 625f 6669 6c65 5f70   is at db_file_p
+00001620: 6174 682e 0a20 2020 206c 6f67 2e77 6172  ath..    log.war
+00001630: 6e69 6e67 2820 224f 7065 6e69 6e67 2044  ning( "Opening D
+00001640: 4220 6174 207b 7061 7468 7d22 2e66 6f72  B at {path}".for
+00001650: 6d61 7428 2070 6174 683d 6462 5f66 696c  mat( path=db_fil
+00001660: 655f 7061 7468 2029 290a 2020 2020 676c  e_path )).    gl
+00001670: 6f62 616c 2064 620a 2020 2020 6462 0909  obal db.    db..
+00001680: 0909 3d20 7765 622e 6461 7461 6261 7365  ..= web.database
+00001690: 2820 6462 6e3d 2773 716c 6974 6527 2c20  ( dbn='sqlite', 
+000016a0: 6462 3d64 625f 6669 6c65 5f70 6174 6820  db=db_file_path 
+000016b0: 290a 2020 2020 6173 7365 7274 2068 6173  ).    assert has
+000016c0: 6174 7472 2820 6462 2c20 2771 7565 7279  attr( db, 'query
+000016d0: 2720 292c 205c 0a20 2020 2020 2020 2022  ' ), \.        "
+000016e0: 556e 7265 636f 676e 697a 6564 206c 6963  Unrecognized lic
+000016f0: 656e 7369 6e67 2044 4220 636f 6e6e 6563  ensing DB connec
+00001700: 7469 6f6e 3a20 7b21 727d 2220 2520 2820  tion: {!r}" % ( 
+00001710: 6462 2029 0a0a 2020 2020 2320 5661 7269  db )..    # Vari
+00001720: 6f75 7320 7374 6174 6963 2076 616c 7565  ous static value
+00001730: 7320 7468 6174 2073 686f 756c 6420 6265  s that should be
+00001740: 2073 6176 6564 2f72 6573 746f 7265 642e   saved/restored.
+00001750: 2020 416c 7761 7973 2062 6567 696e 7320    Always begins 
+00001760: 6174 2064 6566 6175 6c74 7320 6f6e 2073  at defaults on s
+00001770: 7461 7274 2d75 7021 0a20 2020 2023 2042  tart-up!.    # B
+00001780: 7574 2c20 616c 736f 2072 6561 6420 6672  ut, also read fr
+00001790: 6f6d 2064 6174 6162 6173 652e 2020 416c  om database.  Al
+000017a0: 6c20 666c 6f61 7469 6e67 2070 6f69 6e74  l floating point
+000017b0: 2e0a 2020 2020 676c 6f62 616c 2064 625f  ..    global db_
+000017c0: 7374 6174 6963 730a 2020 2020 6462 5f73  statics.    db_s
+000017d0: 7461 7469 6373 0909 093d 207b 7d0a 2020  tatics...= {}.  
+000017e0: 2020 666f 7220 7220 696e 2064 622e 7365    for r in db.se
+000017f0: 6c65 6374 2820 2773 7461 7469 6373 2720  lect( 'statics' 
+00001800: 293a 0a20 2020 2020 2020 2064 625f 7374  ):.        db_st
+00001810: 6174 6963 735b 722e 6b65 795d 0909 3d20  atics[r.key]..= 
+00001820: 666c 6f61 7428 2072 2e76 616c 7565 2029  float( r.value )
+00001830: 0a0a 0a64 6566 2064 625f 7374 6174 655f  ...def db_state_
+00001840: 7361 7665 2829 3a0a 2020 2020 2222 2244  save():.    """D
+00001850: 756d 7020 6f75 7420 616e 7920 7065 7273  ump out any pers
+00001860: 6973 7465 6e74 206c 6963 656e 7369 6e67  istent licensing
+00001870: 2064 6174 612c 2065 7463 2e20 7468 6174   data, etc. that
+00001880: 2073 686f 756c 6420 6265 206c 6f61 6465   should be loade
+00001890: 6420 6e65 7874 2074 696d 652e 2020 5468  d next time.  Th
+000018a0: 6973 2073 686f 756c 6420 6265 2064 6f6e  is should be don
+000018b0: 650a 2020 2020 6672 6f6d 2074 696d 6520  e.    from time 
+000018c0: 746f 2074 696d 652c 2073 6f20 7765 2064  to time, so we d
+000018d0: 6f6e 2774 2067 6574 2074 6f6f 2066 6172  on't get too far
+000018e0: 2062 6568 696e 642c 2069 6e20 6361 7365   behind, in case
+000018f0: 206f 6620 6120 636f 6c64 2072 6562 6f6f   of a cold reboo
+00001900: 742e 2020 4f66 2063 6f75 7273 652c 2073  t.  Of course, s
+00001910: 6176 650a 2020 2020 696d 6d65 6469 6174  ave.    immediat
+00001920: 656c 7920 7570 6f6e 206c 6963 656e 7365  ely upon license
+00001930: 2063 7265 6174 696f 6e2c 2065 7463 2e0a   creation, etc..
+00001940: 0a20 2020 204d 616b 6520 6365 7274 6169  .    Make certai
+00001950: 6e20 7468 6174 2061 6c6c 2073 716c 6974  n that all sqlit
+00001960: 6533 2064 6174 6162 6173 6520 6361 6c6c  e3 database call
+00001970: 7320 6172 6520 7275 6e20 696e 2061 2073  s are run in a s
+00001980: 696e 676c 6520 5468 7265 6164 2e20 2057  ingle Thread.  W
+00001990: 6527 6c6c 2064 6f20 7468 6520 6c6f 6164  e'll do the load
+000019a0: 696e 670a 2020 2020 7269 6768 7420 6265  ing.    right be
+000019b0: 6c6f 7720 2868 6572 652c 2069 6e20 7468  low (here, in th
+000019c0: 6520 4d61 696e 2054 6872 6561 6429 2c20  e Main Thread), 
+000019d0: 6275 7420 616c 6c20 6f74 6865 7220 6461  but all other da
+000019e0: 7461 6261 7365 2049 2f4f 2028 696e 636c  tabase I/O (incl
+000019f0: 7564 696e 6720 7374 6174 655f 7361 7665  uding state_save
+00001a00: 2829 2920 6d75 7374 0a20 2020 206f 6363  ()) must.    occ
+00001a10: 7572 2069 6e20 7468 6520 7765 6270 7920  ur in the webpy 
+00001a20: 5468 7265 6164 2e2e 2e0a 0a20 2020 2046  Thread.....    F
+00001a30: 726f 6d20 6874 7470 733a 2f2f 6769 7468  rom https://gith
+00001a40: 7562 2e63 6f6d 2f73 616d 7073 796f 2f62  ub.com/sampsyo/b
+00001a50: 6565 7473 0a20 2020 2022 2222 0a20 2020  eets.    """.   
+00001a60: 2077 6974 6820 6462 5f6c 6f63 6b3a 0a20   with db_lock:. 
+00001a70: 2020 2020 2020 206c 6f67 2e69 6e66 6f28         log.info(
+00001a80: 2022 5361 7669 6e67 2073 7461 7465 2028   "Saving state (
+00001a90: 7468 7265 6164 3a20 2573 2922 2c20 7468  thread: %s)", th
+00001aa0: 7265 6164 696e 672e 6375 7272 656e 745f  reading.current_
+00001ab0: 7468 7265 6164 2829 2e69 6465 6e74 2029  thread().ident )
+00001ac0: 0a0a 2020 2020 2020 2020 666f 7220 6b20  ..        for k 
+00001ad0: 696e 2064 625f 7374 6174 6963 733a 0a20  in db_statics:. 
+00001ae0: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+00001af0: 7420 6462 2e75 7064 6174 6528 2027 7374  t db.update( 'st
+00001b00: 6174 6963 7327 2c20 7768 6572 653d 226b  atics', where="k
+00001b10: 6579 203d 2024 6b65 7922 2c20 7661 7273  ey = $key", vars
+00001b20: 3d7b 2022 6b65 7922 3a20 6b20 7d2c 2076  ={ "key": k }, v
+00001b30: 616c 7565 3d64 625f 7374 6174 6963 735b  alue=db_statics[
+00001b40: 6b5d 2029 3a0a 2020 2020 2020 2020 2020  k] ):.          
+00001b50: 2020 2020 2020 6966 206e 6f74 2064 622e        if not db.
+00001b60: 696e 7365 7274 2820 2773 7461 7469 6373  insert( 'statics
+00001b70: 272c 206b 6579 3d6b 2c20 7661 6c75 653d  ', key=k, value=
+00001b80: 6462 5f73 7461 7469 6373 5b6b 5d20 293a  db_statics[k] ):
+00001b90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001ba0: 2020 2020 206c 6f67 2e77 6172 6e69 6e67       log.warning
+00001bb0: 2820 2246 6169 6c65 6420 746f 2073 746f  ( "Failed to sto
+00001bc0: 7265 2073 7461 7469 6373 206b 6579 2025  re statics key %
+00001bd0: 7320 7661 6c75 6520 2573 2220 2520 2820  s value %s" % ( 
+00001be0: 6b2c 2064 625f 7374 6174 6963 735b 6b5d  k, db_statics[k]
+00001bf0: 2029 290a 0a0a 6465 6620 6c69 6365 6e73   ))...def licens
+00001c00: 6573 2820 636f 6e66 6972 6d3d 4e6f 6e65  es( confirm=None
+00001c10: 2c20 7374 6f72 6564 3d4e 6f6e 6520 293a  , stored=None ):
+00001c20: 0a20 2020 2022 2222 4f62 7461 696e 2061  .    """Obtain a
+00001c30: 6c6c 204c 6963 656e 7365 2070 726f 7665  ll License prove
+00001c40: 6e61 6e63 6573 2063 7572 7265 6e74 6c79  nances currently
+00001c50: 2061 7661 696c 6162 6c65 2066 726f 6d20   available from 
+00001c60: 7468 6520 4442 2061 6e64 2066 696c 6573  the DB and files
+00001c70: 2c20 6173 2061 2073 6571 7565 6e63 6520  , as a sequence 
+00001c80: 6f66 0a20 2020 2028 7369 676e 6174 7572  of.    (signatur
+00001c90: 652c 204c 6963 656e 7365 2920 7072 6f76  e, License) prov
+00001ca0: 656e 616e 6365 2070 6169 7273 3b20 7369  enance pairs; si
+00001cb0: 676e 6174 7572 6520 6973 2061 2035 3132  gnature is a 512
+00001cc0: 2d62 6974 2045 6432 3535 3139 2053 6967  -bit Ed25519 Sig
+00001cd0: 6e61 7475 7265 2061 7320 6279 7465 732e  nature as bytes.
+00001ce0: 0a0a 2020 2020 4561 6368 206c 6963 656e  ..    Each licen
+00001cf0: 7365 2070 726f 7665 6e61 6e63 6520 636f  se provenance co
+00001d00: 6d70 7269 7365 7320 6120 4c69 6365 6e73  mprises a Licens
+00001d10: 6520 616e 6420 616e 2045 6432 3535 3139  e and an Ed25519
+00001d20: 2053 6967 6e61 7475 7265 2c20 616e 6420   Signature, and 
+00001d30: 6d61 7920 636f 6e74 6169 6e20 6465 7065  may contain depe
+00001d40: 6e64 656e 6369 6573 2e0a 0a20 2020 2041  ndencies...    A
+00001d50: 6c6c 2075 6e69 7175 6520 6c69 6365 6e73  ll unique licens
+00001d60: 6573 2061 7265 2066 6f75 6e64 2061 6e64  es are found and
+00001d70: 2079 6965 6c64 6564 2c20 696e 6465 7865   yielded, indexe
+00001d80: 6420 6279 2074 6865 6972 2073 6967 6e61  d by their signa
+00001d90: 7475 7265 732e 0a0a 2020 2020 416e 7920  tures...    Any 
+00001da0: 4c69 6365 6e73 6520 666f 7220 7768 6963  License for whic
+00001db0: 6820 796f 7520 686f 6c64 2074 6865 2041  h you hold the A
+00001dc0: 7574 686f 7220 7369 676e 696e 6720 6b65  uthor signing ke
+00001dd0: 7970 6169 7220 6d61 7463 6869 6e67 2074  ypair matching t
+00001de0: 6865 204c 6963 656e 7365 7327 2064 6573  he Licenses' des
+00001df0: 6967 6e65 6420 636c 6965 6e74 0a20 2020  igned client.   
+00001e00: 202f 2063 6c69 656e 745f 7075 626b 6579   / client_pubkey
+00001e10: 2028 6f72 2074 6865 7920 6172 6520 6e75   (or they are nu
+00001e20: 6c6c 2f4e 6f6e 6529 206d 6179 2062 6520  ll/None) may be 
+00001e30: 696e 636c 7564 6564 2069 6e20 6120 6e65  included in a ne
+00001e40: 7720 4c69 6365 6e73 6527 7320 6465 7065  w License's depe
+00001e50: 6e64 656e 6369 6573 2e0a 0a20 2020 2049  ndencies...    I
+00001e60: 6e20 6f74 6865 7220 776f 7264 732c 2079  n other words, y
+00001e70: 6f75 206d 6179 2063 7265 6174 6520 616e  ou may create an
+00001e80: 6420 6175 7468 6f72 2028 7369 676e 2920  d author (sign) 
+00001e90: 6120 6272 616e 6420 6e65 7720 4c69 6365  a brand new Lice
+00001ea0: 6e73 6520 7769 7468 206e 6f20 6465 7065  nse with no depe
+00001eb0: 6e64 656e 6369 6573 2c20 6f72 0a20 2020  ndencies, or.   
+00001ec0: 2077 6974 6820 6465 7065 6e64 656e 6369   with dependenci
+00001ed0: 6573 2074 6861 7420 6861 7665 2061 2063  es that have a c
+00001ee0: 6c69 656e 7420 2f20 636c 6965 6e74 5f70  lient / client_p
+00001ef0: 7562 6b65 7920 6d61 7463 6869 6e67 2079  ubkey matching y
+00001f00: 6f75 7220 6175 7468 6f72 696e 6720 6b65  our authoring ke
+00001f10: 7970 6169 7220 7075 626b 6579 2e0a 0a20  ypair pubkey... 
+00001f20: 2020 2054 4f44 4f3a 204c 6963 656e 7365     TODO: License
+00001f30: 7320 7370 6563 6966 7969 6e67 2061 202a  s specifying a *
+00001f40: 6e75 6d62 6572 2a20 6f66 2074 6869 6e67  number* of thing
+00001f50: 7320 6d61 7920 6265 2075 7365 6420 6173  s may be used as
+00001f60: 2064 6570 656e 6465 6e63 6965 7320 696e   dependencies in
+00001f70: 2061 7574 686f 7265 6420 4c69 6365 6e73   authored Licens
+00001f80: 6573 0a20 2020 2075 6e74 696c 2074 6865  es.    until the
+00001f90: 2073 756d 206f 6620 7468 6f73 6520 7468   sum of those th
+00001fa0: 696e 6773 2061 6c6c 6f63 6174 6564 2074  ings allocated t
+00001fb0: 6f20 7468 6520 6175 7468 6f72 6564 206c  o the authored l
+00001fc0: 6963 656e 7365 7320 6d65 6574 7320 7468  icenses meets th
+00001fd0: 6520 4c69 6365 6e73 6520 6465 7065 6e64  e License depend
+00001fe0: 656e 6369 6573 270a 2020 2020 6e75 6d62  encies'.    numb
+00001ff0: 6572 206c 696d 6974 2e0a 0a20 2020 2022  er limit...    "
+00002000: 2222 0a20 2020 2065 6d69 7474 6564 0909  "".    emitted..
+00002010: 093d 2073 6574 2829 0a0a 2020 2020 6465  .= set()..    de
+00002020: 6620 656d 6974 2820 2a70 726f 7673 2029  f emit( *provs )
+00002030: 3a0a 2020 2020 2020 2020 666f 7220 7020  :.        for p 
+00002040: 696e 2070 726f 7673 3a0a 2020 2020 2020  in provs:.      
+00002050: 2020 2020 2020 6966 2070 2e73 6967 6e61        if p.signa
+00002060: 7475 7265 2069 6e20 656d 6974 7465 643a  ture in emitted:
+00002070: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002080: 2063 6f6e 7469 6e75 650a 2020 2020 2020   continue.      
+00002090: 2020 2020 2020 7969 656c 6420 702e 7369        yield p.si
+000020a0: 676e 6174 7572 652c 2070 2e6c 6963 656e  gnature, p.licen
+000020b0: 7365 0a20 2020 2020 2020 2020 2020 2065  se.            e
+000020c0: 6d69 7474 6564 2e61 6464 2820 702e 7369  mitted.add( p.si
+000020d0: 676e 6174 7572 6520 290a 2020 2020 2020  gnature ).      
+000020e0: 2020 2020 2020 666f 7220 7369 672c 206c        for sig, l
+000020f0: 6963 2069 6e20 656d 6974 2820 2a5b 206c  ic in emit( *[ l
+00002100: 6963 656e 7369 6e67 2e4c 6963 656e 7365  icensing.License
+00002110: 5369 676e 6564 2820 636f 6e66 6972 6d3d  Signed( confirm=
+00002120: 636f 6e66 6972 6d2c 206d 6163 6869 6e65  confirm, machine
+00002130: 5f69 645f 7061 7468 3d46 616c 7365 2c20  _id_path=False, 
+00002140: 2a2a 7064 2029 0a20 2020 2020 2020 2020  **pd ).         
+00002150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002160: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00002170: 7064 2069 6e20 702e 6c69 6365 6e73 652e  pd in p.license.
+00002180: 6465 7065 6e64 656e 6369 6573 206f 7220  dependencies or 
+00002190: 5b5d 205d 2029 3a0a 2020 2020 2020 2020  [] ] ):.        
+000021a0: 2020 2020 2020 2020 7969 656c 6420 7369          yield si
+000021b0: 672c 206c 6963 0a0a 2020 2020 2320 4669  g, lic..    # Fi
+000021c0: 7273 742c 2070 726f 6365 7373 2061 6e79  rst, process any
+000021d0: 2073 746f 7265 6420 7072 6f76 656e 616e   stored provenan
+000021e0: 6365 732e 2020 5468 6573 6520 6172 6520  ces.  These are 
+000021f0: 6173 7375 6d65 6420 746f 2063 6f6e 7461  assumed to conta
+00002200: 696e 202e 6c69 6365 6e73 6520 616e 6420  in .license and 
+00002210: 2e73 6967 6e61 7475 7265 0a20 2020 2023  .signature.    #
+00002220: 2061 7474 7269 6275 7465 732e 2020 436f   attributes.  Co
+00002230: 756c 6420 6265 2061 2073 6571 7565 6e63  uld be a sequenc
+00002240: 6520 6f66 204c 6963 656e 7365 5369 676e  e of LicenseSign
+00002250: 6564 2c20 6f72 2061 2064 6174 6162 6173  ed, or a databas
+00002260: 6520 7175 6572 7920 7969 656c 6469 6e67  e query yielding
+00002270: 2072 6563 6f72 6473 2077 6974 680a 2020   records with.  
+00002280: 2020 2320 2e73 6967 6e61 7475 7265 2061    # .signature a
+00002290: 6e64 202e 6c69 6365 6e73 652e 2020 5468  nd .license.  Th
+000022a0: 6573 6520 6d61 7920 6265 2066 756c 6c20  ese may be full 
+000022b0: 4c69 6365 6e73 6573 2073 7472 7563 7473  Licenses structs
+000022c0: 2061 6e64 2073 6967 6e61 7475 7265 7320   and signatures 
+000022d0: 6279 7465 7320 6461 7461 2c20 6f72 0a20  bytes data, or. 
+000022e0: 2020 2023 2073 6572 6961 6c69 7a65 6420     # serialized 
+000022f0: 666f 726d 732e 0a20 2020 2066 6f75 6e64  forms..    found
+00002300: 0909 093d 2030 0a20 2020 2066 6f72 2072  ...= 0.    for r
+00002310: 2069 6e20 7374 6f72 6564 206f 7220 5b5d   in stored or []
+00002320: 3a0a 2020 2020 2020 2020 7472 793a 0a20  :.        try:. 
+00002330: 2020 2020 2020 2020 2020 2070 726f 7609             prov.
+00002340: 093d 206c 6963 656e 7369 6e67 2e4c 6963  .= licensing.Lic
+00002350: 656e 7365 5369 676e 6564 280a 2020 2020  enseSigned(.    
+00002360: 2020 2020 2020 2020 2020 2020 6c69 6365              lice
+00002370: 6e73 653d 722e 6c69 6365 6e73 652c 2073  nse=r.license, s
+00002380: 6967 6e61 7475 7265 3d72 2e73 6967 6e61  ignature=r.signa
+00002390: 7475 7265 2c20 636f 6e66 6972 6d3d 636f  ture, confirm=co
+000023a0: 6e66 6972 6d2c 206d 6163 6869 6e65 5f69  nfirm, machine_i
+000023b0: 645f 7061 7468 3d46 616c 7365 2029 0a20  d_path=False ). 
+000023c0: 2020 2020 2020 2065 7863 6570 7420 4578         except Ex
+000023d0: 6365 7074 696f 6e20 6173 2065 7863 3a0a  ception as exc:.
+000023e0: 2020 2020 2020 2020 2020 2020 6c6f 672e              log.
+000023f0: 6465 6275 6728 2022 4661 696c 6564 2074  debug( "Failed t
+00002400: 6f20 6c6f 6164 2073 746f 7265 6420 4c69  o load stored Li
+00002410: 6365 6e73 6520 7072 6f76 656e 616e 6365  cense provenance
+00002420: 3a20 7b65 7863 7d20 6672 6f6d 3a20 7b6c  : {exc} from: {l
+00002430: 6963 7d22 2e66 6f72 6d61 7428 0a20 2020  ic}".format(.   
+00002440: 2020 2020 2020 2020 2020 2020 2065 7863               exc
+00002450: 3d27 272e 6a6f 696e 2820 7472 6163 6562  =''.join( traceb
+00002460: 6163 6b2e 666f 726d 6174 5f65 7863 6570  ack.format_excep
+00002470: 7469 6f6e 2820 2a73 7973 2e65 7863 5f69  tion( *sys.exc_i
+00002480: 6e66 6f28 2920 2929 2069 6620 6c6f 672e  nfo() )) if log.
+00002490: 6973 456e 6162 6c65 6446 6f72 2820 6c6f  isEnabledFor( lo
+000024a0: 6767 696e 672e 5452 4143 4520 2920 656c  gging.TRACE ) el
+000024b0: 7365 2065 7863 2c0a 2020 2020 2020 2020  se exc,.        
+000024c0: 2020 2020 2020 2020 6c69 633d 722e 6c69          lic=r.li
+000024d0: 6365 6e73 6520 2929 0a20 2020 2020 2020  cense )).       
+000024e0: 2020 2020 2072 6169 7365 0a20 2020 2020       raise.     
+000024f0: 2020 2066 6f72 2073 6967 2c20 6c69 6320     for sig, lic 
+00002500: 696e 2065 6d69 7428 2070 726f 7620 293a  in emit( prov ):
+00002510: 0a20 2020 2020 2020 2020 2020 2079 6965  .            yie
+00002520: 6c64 2073 6967 2c20 6c69 630a 2020 2020  ld sig, lic.    
+00002530: 2020 2020 2020 2020 666f 756e 6409 2020          found.  
+00002540: 2020 2020 202b 3d20 310a 2020 2020 6c6f       += 1.    lo
+00002550: 672e 696e 666f 2820 224c 6963 656e 7365  g.info( "License
+00002560: 7320 2020 2020 7361 7665 643a 207b 7d22  s     saved: {}"
+00002570: 2e66 6f72 6d61 7428 2066 6f75 6e64 2029  .format( found )
+00002580: 290a 0a20 2020 2066 6f75 6e64 0909 093d  )..    found...=
+00002590: 2030 0a20 2020 2070 6174 6809 0909 3d20   0.    path...= 
+000025a0: 4e6f 6e65 0a20 2020 2074 7279 3a0a 2020  None.    try:.  
+000025b0: 2020 2020 2020 2320 4c6f 6164 206d 6f73        # Load mos
+000025c0: 7420 6765 6e65 7261 6c2f 6469 7374 616e  t general/distan
+000025d0: 7420 4c69 6365 6e73 6573 2066 6972 7374  t Licenses first
+000025e0: 2c20 696e 636c 7564 696e 6720 7468 6520  , including the 
+000025f0: 6f70 7469 6f6e 616c 2065 7874 7261 2063  optional extra c
+00002600: 6f6e 6669 6720 6469 7273 0a20 2020 2020  onfig dirs.     
+00002610: 2020 2067 6c6f 6261 6c20 636f 6e66 6967     global config
+00002620: 5f65 7874 7261 730a 2020 2020 2020 2020  _extras.        
+00002630: 666f 7220 7061 7468 2c20 7072 6f76 2069  for path, prov i
+00002640: 6e20 6c69 6365 6e73 696e 672e 6c6f 6164  n licensing.load
+00002650: 2820 7061 636b 6167 653d 5f5f 7061 636b  ( package=__pack
+00002660: 6167 655f 5f2c 2065 7874 7261 3d63 6f6e  age__, extra=con
+00002670: 6669 675f 6578 7472 6173 2c20 7265 7665  fig_extras, reve
+00002680: 7273 653d 4661 6c73 6520 293a 0a20 2020  rse=False ):.   
+00002690: 2020 2020 2020 2020 2066 6f72 2073 6967           for sig
+000026a0: 2c20 6c69 6320 696e 2065 6d69 7428 2070  , lic in emit( p
+000026b0: 726f 7620 293a 0a20 2020 2020 2020 2020  rov ):.         
+000026c0: 2020 2020 2020 2079 6965 6c64 2073 6967         yield sig
+000026d0: 2c20 6c69 630a 2020 2020 2020 2020 2020  , lic.          
+000026e0: 2020 2020 2020 666f 756e 6409 2020 2020        found.    
+000026f0: 2020 202b 3d20 310a 2020 2020 6578 6365     += 1.    exce
+00002700: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
+00002710: 6578 633a 0a20 2020 2020 2020 206c 6f67  exc:.        log
+00002720: 2e65 7272 6f72 2820 2246 6169 6c65 6420  .error( "Failed 
+00002730: 746f 206c 6f61 6420 6c69 6365 6e73 6520  to load license 
+00002740: 6672 6f6d 207b 7d3a 207b 7d22 2e66 6f72  from {}: {}".for
+00002750: 6d61 7428 2070 6174 6820 6f72 205f 5f70  mat( path or __p
+00002760: 6163 6b61 6765 5f5f 2c20 6578 6320 2929  ackage__, exc ))
+00002770: 0a20 2020 2020 2020 2070 6173 730a 2020  .        pass.  
+00002780: 2020 6c6f 672e 696e 666f 2820 224c 6963    log.info( "Lic
+00002790: 656e 7365 7320 2020 206c 6f61 6465 643a  enses    loaded:
+000027a0: 207b 7d22 2e66 6f72 6d61 7428 2066 6f75   {}".format( fou
+000027b0: 6e64 2029 290a 0a0a 6465 6620 6372 6564  nd ))...def cred
+000027c0: 656e 7469 616c 7328 202a 6164 6420 293a  entials( *add ):
+000027d0: 0a20 2020 2022 2222 4c6f 6164 2061 6e79  .    """Load any
+000027e0: 2061 7661 696c 6162 6c65 2063 7265 6465   available crede
+000027f0: 6e74 6961 6c73 2c20 616e 6420 6164 6420  ntials, and add 
+00002800: 616e 7920 7061 7373 6564 2028 6465 7363  any passed (desc
+00002810: 7269 7074 696f 6e2c 2028 7573 6572 6e61  ription, (userna
+00002820: 6d65 2c20 7061 7373 776f 7264 2929 2c0a  me, password)),.
+00002830: 2020 2020 2e2e 2e20 636f 6e74 6169 6e69      ... containi
+00002840: 6e67 206e 6577 2063 7265 6465 6e74 6961  ng new credentia
+00002850: 6c73 2073 7570 706c 6965 6420 6279 2074  ls supplied by t
+00002860: 6865 204c 6963 656e 7365 2053 6572 7665  he License Serve
+00002870: 7220 6164 6d69 6e69 7374 7261 746f 7220  r administrator 
+00002880: 6475 7269 6e67 206f 7065 7261 7469 6f6e  during operation
+00002890: 2e0a 0a20 2020 2045 6163 6820 5468 7265  ...    Each Thre
+000028a0: 6164 206f 6620 7468 6973 204c 6963 656e  ad of this Licen
+000028b0: 7365 2053 6572 7665 7220 7468 6174 206d  se Server that m
+000028c0: 7573 7420 6465 6372 7970 7420 656e 6372  ust decrypt encr
+000028d0: 7970 7465 6420 6b65 7973 2073 686f 756c  ypted keys shoul
+000028e0: 6420 7573 6520 7468 6573 6520 6372 6564  d use these cred
+000028f0: 656e 7469 616c 730a 2020 2020 746f 2061  entials.    to a
+00002900: 6363 6573 7320 7468 6520 6b65 7973 2e0a  ccess the keys..
+00002910: 0a20 2020 2054 4f44 4f3a 2053 686f 756c  .    TODO: Shoul
+00002920: 6420 7468 6973 2062 6520 656e 6372 7970  d this be encryp
+00002930: 7465 6420 6174 2d72 6573 7420 6475 7269  ted at-rest duri
+00002940: 6e67 206f 7065 7261 7469 6f6e 3f20 2049  ng operation?  I
+00002950: 7420 636f 756c 6420 6265 2069 6e73 7065  t could be inspe
+00002960: 6374 6564 2062 7920 616e 790a 2020 2020  cted by any.    
+00002970: 7573 6572 2f72 6f6f 7420 6c65 7665 6c20  user/root level 
+00002980: 7072 6f63 6573 732c 2061 6e64 2075 7365  process, and use
+00002990: 6420 746f 2075 6e6c 6f63 6b20 7468 6520  d to unlock the 
+000029a0: 656e 6372 7970 7465 6420 6175 7468 6f72  encrypted author
+000029b0: 2073 6967 6e69 6e67 206b 6579 7061 6972   signing keypair
+000029c0: 732e 0a0a 2020 2020 2222 220a 2020 2020  s...    """.    
+000029d0: 7969 656c 6420 2228 4e6f 2043 7265 6465  yield "(No Crede
+000029e0: 6e74 6961 6c73 2922 2c20 284e 6f6e 652c  ntials)", (None,
+000029f0: 204e 6f6e 6529 0a0a 2020 2020 6372 6564   None)..    cred
+00002a00: 656e 7469 616c 732e 6c6f 6361 6c2e 7570  entials.local.up
+00002a10: 6461 7465 2820 6164 6420 290a 2020 2020  date( add ).    
+00002a20: 666f 7220 6e61 6d65 2c20 2875 7365 726e  for name, (usern
+00002a30: 616d 652c 2070 6173 7377 6f72 6429 2069  ame, password) i
+00002a40: 6e20 6372 6564 656e 7469 616c 732e 6c6f  n credentials.lo
+00002a50: 6361 6c2e 6974 656d 7328 293a 0a20 2020  cal.items():.   
+00002a60: 2020 2020 2079 6965 6c64 206e 616d 652c       yield name,
+00002a70: 2028 7573 6572 6e61 6d65 2c20 7061 7373   (username, pass
+00002a80: 776f 7264 290a 2020 2020 6c6f 672e 696e  word).    log.in
+00002a90: 666f 2820 2243 7265 6465 6e74 6961 6c73  fo( "Credentials
+00002aa0: 2063 6163 6865 643a 207b 7d22 2e66 6f72   cached: {}".for
+00002ab0: 6d61 7428 206c 656e 2820 6372 6564 656e  mat( len( creden
+00002ac0: 7469 616c 732e 6c6f 6361 6c20 2929 290a  tials.local ))).
+00002ad0: 0a20 2020 2066 6f75 6e64 0909 093d 2030  .    found...= 0
+00002ae0: 0a20 2020 2070 6174 6809 0909 3d20 4e6f  .    path...= No
+00002af0: 6e65 0a20 2020 2074 7279 3a0a 2020 2020  ne.    try:.    
+00002b00: 2020 2020 2320 4f70 656e 2061 6e79 206c      # Open any l
+00002b10: 6963 656e 7369 6e67 2e63 7265 6465 6e74  icensing.credent
+00002b20: 6961 6c73 2a20 696e 2063 6f6e 6669 6775  ials* in configu
+00002b30: 7261 7469 6f6e 2070 6174 682e 2020 5765  ration path.  We
+00002b40: 2077 616e 7420 746f 206c 6f61 6420 6d6f   want to load mo
+00002b50: 7374 0a20 2020 2020 2020 2023 2067 656e  st.        # gen
+00002b60: 6572 616c 2f64 6973 7461 6e74 2066 696c  eral/distant fil
+00002b70: 6573 2066 6972 7374 2073 6f20 6d61 6b65  es first so make
+00002b80: 2072 6576 6572 7365 3d54 7275 652e 0a20   reverse=True.. 
+00002b90: 2020 2020 2020 2067 6c6f 6261 6c20 636f         global co
+00002ba0: 6e66 6967 5f65 7874 7261 730a 2020 2020  nfig_extras.    
+00002bb0: 2020 2020 666f 7220 6620 696e 2063 6f6e      for f in con
+00002bc0: 6669 675f 6f70 656e 2820 4352 4446 494c  fig_open( CRDFIL
+00002bd0: 452b 272a 272c 2065 7874 7261 3d63 6f6e  E+'*', extra=con
+00002be0: 6669 675f 6578 7472 6173 2c20 736b 6970  fig_extras, skip
+00002bf0: 3d27 2a7e 272c 2072 6576 6572 7365 3d46  ='*~', reverse=F
+00002c00: 616c 7365 2029 3a0a 2020 2020 2020 2020  alse ):.        
+00002c10: 2020 2020 7769 7468 2066 3a0a 2020 2020      with f:.    
+00002c20: 2020 2020 2020 2020 2020 2020 2320 4561              # Ea
+00002c30: 6368 206c 6963 656e 7369 6e67 2e63 7265  ch licensing.cre
+00002c40: 6465 6e74 6961 6c73 2a20 6669 6c65 2073  dentials* file s
+00002c50: 686f 756c 6420 6265 2061 2073 6571 7565  hould be a seque
+00002c60: 6e63 6520 6f66 3a0a 2020 2020 2020 2020  nce of:.        
+00002c70: 2020 2020 2020 2020 2320 2020 2020 5b20          #     [ 
+00002c80: 2820 2264 6573 6372 6970 7469 6f6e 222c  ( "description",
+00002c90: 205b 2022 7573 6572 6e61 6d65 223a 2022   [ "username": "
+00002ca0: 7061 7373 776f 7264 2220 5d20 292c 202e  password" ] ), .
+00002cb0: 2e2e 205d 0a20 2020 2020 2020 2020 2020  .. ].           
+00002cc0: 2020 2020 2023 2073 6f20 636f 6e76 6572       # so conver
+00002cd0: 7420 6120 6469 6374 2069 6e74 6f20 7375  t a dict into su
+00002ce0: 6368 2061 2073 6571 7565 6e63 652e 2020  ch a sequence.  
+00002cf0: 486f 7765 7665 722c 2072 6576 6572 7365  However, reverse
+00002d00: 2074 6865 202e 7570 6461 7465 2073 6f20   the .update so 
+00002d10: 6d6f 7265 0a20 2020 2020 2020 2020 2020  more.           
+00002d20: 2020 2020 2023 2065 6172 6c69 6572 2028       # earlier (
+00002d30: 6d6f 7265 2073 7065 6369 6669 6329 2063  more specific) c
+00002d40: 6f6e 6669 6775 7261 7469 6f6e 7320 6172  onfigurations ar
+00002d50: 6520 6e6f 7420 6f76 6572 7269 6465 6e20  e not overriden 
+00002d60: 6279 206c 6174 6572 2028 6d6f 7265 2067  by later (more g
+00002d70: 656e 6572 616c 290a 2020 2020 2020 2020  eneral).        
+00002d80: 2020 2020 2020 2020 2320 6f6e 6573 2e0a          # ones..
+00002d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002da0: 7061 7468 0909 3d20 662e 6e61 6d65 0a20  path..= f.name. 
+00002db0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00002dc0: 7265 6473 0909 3d20 6a73 6f6e 2e6c 6f61  reds..= json.loa
+00002dd0: 6473 2820 662e 7265 6164 2829 2029 0a20  ds( f.read() ). 
+00002de0: 2020 2020 2020 2020 2020 2069 6620 6973             if is
+00002df0: 696e 7374 616e 6365 2820 6372 6564 732c  instance( creds,
+00002e00: 2064 6963 7420 293a 0a20 2020 2020 2020   dict ):.       
+00002e10: 2020 2020 2020 2020 2063 7265 6473 0909           creds..
+00002e20: 3d20 6372 6564 732e 6974 656d 7328 290a  = creds.items().
+00002e30: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00002e40: 6e61 6d65 2c20 2875 7365 726e 616d 652c  name, (username,
+00002e50: 2070 6173 7377 6f72 6429 2069 6e20 6372   password) in cr
+00002e60: 6564 733a 0a20 2020 2020 2020 2020 2020  eds:.           
+00002e70: 2020 2020 206c 6f67 2e69 6e66 6f28 2022       log.info( "
+00002e80: 2020 7b6e 3a3c 3230 7d3a 207b 753a 3e32    {n:<20}: {u:>2
+00002e90: 307d 202f 207b 707d 222e 666f 726d 6174  0} / {p}".format
+00002ea0: 2820 6e3d 6e61 6d65 2c20 753d 7573 6572  ( n=name, u=user
+00002eb0: 6e61 6d65 2c20 703d 272a 2720 2a20 6c65  name, p='*' * le
+00002ec0: 6e28 2070 6173 7377 6f72 6420 2929 290a  n( password ))).
+00002ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ee0: 7969 656c 6420 6e61 6d65 2c20 2875 7365  yield name, (use
+00002ef0: 726e 616d 652c 2070 6173 7377 6f72 6429  rname, password)
+00002f00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002f10: 2066 6f75 6e64 0920 2020 2020 2020 2b3d   found.       +=
+00002f20: 2031 0a20 2020 2065 7863 6570 7420 4578   1.    except Ex
+00002f30: 6365 7074 696f 6e20 6173 2065 7863 3a0a  ception as exc:.
+00002f40: 2020 2020 2020 2020 6c6f 672e 6572 726f          log.erro
+00002f50: 7228 2022 4661 696c 6564 2074 6f20 6c6f  r( "Failed to lo
+00002f60: 6164 207b 7d2a 3a20 7b7d 222e 666f 726d  ad {}*: {}".form
+00002f70: 6174 2820 7061 7468 206f 7220 4352 4446  at( path or CRDF
+00002f80: 494c 452c 2065 7863 2029 290a 2020 2020  ILE, exc )).    
+00002f90: 2020 2020 7061 7373 0a20 2020 206c 6f67      pass.    log
+00002fa0: 2e69 6e66 6f28 2022 4372 6564 656e 7469  .info( "Credenti
+00002fb0: 616c 7320 6c6f 6164 6564 3a20 7b7d 222e  als loaded: {}".
+00002fc0: 666f 726d 6174 2820 666f 756e 6420 2929  format( found ))
+00002fd0: 0a0a 0a63 7265 6465 6e74 6961 6c73 2e6c  ...credentials.l
+00002fe0: 6f63 616c 0909 3d20 7b7d 2020 2320 7b20  ocal..= {}  # { 
+00002ff0: 6465 7363 7269 7074 696f 6e3a 2028 7573  description: (us
+00003000: 6572 6e61 6d65 2c20 7061 7373 776f 7264  ername, password
+00003010: 292c 202e 2e2e 207d 0a0a 0a64 6566 206b  ), ... }...def k
+00003020: 6579 7061 6972 7328 293a 0a20 2020 2022  eypairs():.    "
+00003030: 2222 4c6f 6164 2061 6c6c 2061 7661 696c  ""Load all avail
+00003040: 6162 6c65 206b 6579 7061 6972 7320 6176  able keypairs av
+00003050: 6169 6c61 626c 6520 666f 7220 6175 7468  ailable for auth
+00003060: 6f72 696e 6720 4c69 6365 6e73 6573 2c20  oring Licenses, 
+00003070: 7573 696e 6720 616c 6c20 6375 7272 656e  using all curren
+00003080: 746c 7920 6176 6169 6c61 626c 650a 2020  tly available.  
+00003090: 2020 6372 6564 656e 7469 616c 732e 2020    credentials.  
+000030a0: 5468 6973 2069 6e63 6c75 6465 7320 616c  This includes al
+000030b0: 6c20 456e 6372 7970 7465 6420 616e 6420  l Encrypted and 
+000030c0: 506c 6169 6e74 6578 7420 6b65 7973 2069  Plaintext keys i
+000030d0: 6e20 6669 6c65 732c 2061 6e64 2061 6c6c  n files, and all
+000030e0: 2045 6e63 7279 7074 6564 206b 6579 7320   Encrypted keys 
+000030f0: 696e 0a20 2020 2064 6174 6162 6173 6520  in.    database 
+00003100: 2261 7574 686f 7273 2220 7461 626c 652e  "authors" table.
+00003110: 2020 4561 6368 2074 696d 6520 7765 2061    Each time we a
+00003120: 6464 2061 206e 6577 2063 7265 6465 6e74  dd a new credent
+00003130: 6961 6c2c 2074 6869 7320 2a6d 6179 2a20  ial, this *may* 
+00003140: 6d61 6b65 2061 7661 696c 6162 6c65 206d  make available m
+00003150: 6f72 650a 2020 2020 6b65 7973 2065 6e63  ore.    keys enc
+00003160: 7279 7074 6564 2077 6974 6820 7468 6f73  rypted with thos
+00003170: 6520 6372 6564 656e 7469 616c 732e 0a0a  e credentials...
+00003180: 2020 2020 5969 656c 6420 7365 7175 656e      Yield sequen
+00003190: 6365 206f 6620 616c 6c20 6176 6169 6c61  ce of all availa
+000031a0: 626c 6520 286e 616d 652c 202e 2e2e 4b65  ble (name, ...Ke
+000031b0: 7970 6169 722c 2063 7265 6465 6e74 6961  ypair, credentia
+000031c0: 6c29 2066 726f 6d20 2261 7574 686f 7273  l) from "authors
+000031d0: 2220 7461 626c 6520 616e 6420 6669 6c65  " table and file
+000031e0: 732e 0a20 2020 204d 6179 2063 6f6e 7461  s..    May conta
+000031f0: 696e 2064 7570 6c69 6361 7465 732e 2020  in duplicates.  
+00003200: 4361 6c6c 6572 206d 6179 2061 6363 756d  Caller may accum
+00003210: 756c 6174 6520 7468 656d 2c20 6f72 2073  ulate them, or s
+00003220: 696d 706c 7920 7363 616e 2066 6f72 2064  imply scan for d
+00003230: 6573 6972 6564 2065 6e74 7279 2e0a 0a20  esired entry... 
+00003240: 2020 2022 2222 0a20 2020 206c 6f61 6465     """.    loade
+00003250: 6409 0909 3d20 7365 7428 290a 2020 2020  d...= set().    
+00003260: 7361 7665 6409 0909 3d20 300a 2020 2020  saved...= 0.    
+00003270: 666f 7220 6372 6564 6e61 6d65 2c28 7573  for credname,(us
+00003280: 6572 6e61 6d65 2c70 6173 7377 6f72 6429  ername,password)
+00003290: 2069 6e20 6372 6564 656e 7469 616c 7328   in credentials(
+000032a0: 293a 0a20 2020 2020 2020 206c 6f67 2e69  ):.        log.i
+000032b0: 6e66 6f28 2022 4b65 7970 6169 7273 2066  nfo( "Keypairs f
+000032c0: 6f72 207b 7d27 7320 6372 6564 656e 7469  or {}'s credenti
+000032d0: 616c 3a22 2e66 6f72 6d61 7428 2075 7365  al:".format( use
+000032e0: 726e 616d 6520 2929 0a20 2020 2020 2020  rname )).       
+000032f0: 2066 6f72 2072 2069 6e20 6462 2e73 656c   for r in db.sel
+00003300: 6563 7428 2027 6175 7468 6f72 7327 2029  ect( 'authors' )
+00003310: 3a0a 2020 2020 2020 2020 2020 2020 6372  :.            cr
+00003320: 6564 0909 3d20 6469 6374 2820 7573 6572  ed..= dict( user
+00003330: 6e61 6d65 3d75 7365 726e 616d 652c 2070  name=username, p
+00003340: 6173 7377 6f72 643d 7061 7373 776f 7264  assword=password
+00003350: 2029 0a20 2020 2020 2020 2020 2020 2074   ).            t
+00003360: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+00003370: 2020 2020 6b65 7970 6169 7209 093d 206c      keypair..= l
+00003380: 6963 656e 7369 6e67 2e4b 6579 7061 6972  icensing.Keypair
+00003390: 456e 6372 7970 7465 6428 2063 6970 6865  Encrypted( ciphe
+000033a0: 7274 6578 743d 722e 6369 7068 6572 7465  rtext=r.cipherte
+000033b0: 7874 2c20 7361 6c74 3d72 2e73 616c 7420  xt, salt=r.salt 
+000033c0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000033d0: 2020 6b65 7970 6169 722e 696e 746f 5f6b    keypair.into_k
+000033e0: 6579 7061 6972 2820 2a2a 6372 6564 2029  eypair( **cred )
+000033f0: 2020 2320 456e 7375 7265 2074 6865 2073    # Ensure the s
+00003400: 7570 706c 6965 6420 6372 6564 656e 7469  upplied credenti
+00003410: 616c 7320 6361 6e20 6465 6372 7970 7420  als can decrypt 
+00003420: 6974 0a20 2020 2020 2020 2020 2020 2020  it.             
+00003430: 2020 2079 6965 6c64 2072 2e6e 616d 652c     yield r.name,
+00003440: 206b 6579 7061 6972 2c20 6372 6564 0a20   keypair, cred. 
+00003450: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00003460: 6176 6564 0920 2020 2020 2020 2b3d 2031  aved.       += 1
+00003470: 0a20 2020 2020 2020 2020 2020 2065 7863  .            exc
+00003480: 6570 7420 4578 6365 7074 696f 6e20 6173  ept Exception as
+00003490: 2065 7863 3a0a 2020 2020 2020 2020 2020   exc:.          
+000034a0: 2020 2020 2020 2320 4d6f 7374 206b 6579        # Most key
+000034b0: 7061 6972 7320 7769 6c6c 2066 6169 6c20  pairs will fail 
+000034c0: 746f 2064 6563 7279 7074 2077 6974 6820  to decrypt with 
+000034d0: 6d6f 7374 2063 7265 6465 6e74 6961 6c73  most credentials
+000034e0: 2e2e 2e0a 2020 2020 2020 2020 2020 2020  ....            
+000034f0: 2020 2020 6c6f 672e 6465 6275 6728 2022      log.debug( "
+00003500: 7b6e 3a3c 3230 7d3a 2046 6169 6c65 6420  {n:<20}: Failed 
+00003510: 746f 2064 6563 7279 7074 2077 2f20 7b75  to decrypt w/ {u
+00003520: 3a3e 3230 7d20 2f20 7b70 7d3a 207b 6578  :>20} / {p}: {ex
+00003530: 637d 222e 666f 726d 6174 280a 2020 2020  c}".format(.    
+00003540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003550: 6e3d 722e 6e61 6d65 2c20 753d 6372 6564  n=r.name, u=cred
+00003560: 5b27 7573 6572 6e61 6d65 275d 206f 7220  ['username'] or 
+00003570: 2728 656d 7074 7929 272c 2070 3d27 2a27  '(empty)', p='*'
+00003580: 202a 206c 656e 2820 6372 6564 5b27 7061   * len( cred['pa
+00003590: 7373 776f 7264 275d 206f 7220 2728 656d  ssword'] or '(em
+000035a0: 7074 7929 2720 292c 0a20 2020 2020 2020  pty)' ),.       
+000035b0: 2020 2020 2020 2020 2020 2020 2065 7863               exc
+000035c0: 3d65 7863 2029 290a 2020 2020 2020 2020  =exc )).        
+000035d0: 2020 2020 2020 2020 7061 7373 0a20 2020          pass.   
+000035e0: 2020 2020 2023 2041 6e79 2050 6c61 696e       # Any Plain
+000035f0: 7465 7874 204b 6579 7061 6972 7320 2861  text Keypairs (a
+00003600: 6e64 2070 6572 6861 7073 2073 6f6d 6520  nd perhaps some 
+00003610: 456e 6372 7970 7465 6420 6f6e 6573 2c20  Encrypted ones, 
+00003620: 6966 2064 7570 6c69 6361 7465 2063 7265  if duplicate cre
+00003630: 6465 6e74 6961 6c73 2061 7265 0a20 2020  dentials are.   
+00003640: 2020 2020 2023 2073 7570 706c 6965 6429       # supplied)
+00003650: 2077 696c 6c20 6265 2066 6f75 6e64 206d   will be found m
+00003660: 756c 7469 706c 6520 7469 6d65 732e 2020  ultiple times.  
+00003670: 5265 706f 7274 206b 6579 7061 6972 7320  Report keypairs 
+00003680: 6174 2074 6865 2073 616d 6520 7061 7468  at the same path
+00003690: 206f 6e6c 7920 6f6e 6365 2e20 2057 650a   only once.  We.
+000036a0: 2020 2020 2020 2020 2320 7761 6e74 2074          # want t
+000036b0: 6f20 6c6f 6164 2074 6865 206d 6f73 7420  o load the most 
+000036c0: 6765 6e65 7261 6c2f 6469 7374 616e 7420  general/distant 
+000036d0: 6b65 7973 2066 6972 7374 2c20 736f 2072  keys first, so r
+000036e0: 6576 6572 7365 3d46 616c 7365 2e0a 2020  everse=False..  
+000036f0: 2020 2020 2020 7061 7468 0909 093d 204e        path...= N
+00003700: 6f6e 650a 2020 2020 2020 2020 7472 793a  one.        try:
+00003710: 0a20 2020 2020 2020 2020 2020 2067 6c6f  .            glo
+00003720: 6261 6c20 636f 6e66 6967 5f65 7874 7261  bal config_extra
+00003730: 730a 2020 2020 2020 2020 2020 2020 666f  s.            fo
+00003740: 7220 7061 7468 2c20 6b65 7970 6169 722c  r path, keypair,
+00003750: 2063 7265 6420 696e 206c 6963 656e 7369   cred in licensi
+00003760: 6e67 2e6c 6f61 645f 6b65 7973 280a 2020  ng.load_keys(.  
+00003770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003780: 2020 7061 636b 6167 653d 5f5f 7061 636b    package=__pack
+00003790: 6167 655f 5f2c 2075 7365 726e 616d 653d  age__, username=
+000037a0: 7573 6572 6e61 6d65 2c20 7061 7373 776f  username, passwo
+000037b0: 7264 3d70 6173 7377 6f72 642c 0a20 2020  rd=password,.   
+000037c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000037d0: 2065 7874 7261 3d63 6f6e 6669 675f 6578   extra=config_ex
+000037e0: 7472 6173 2c20 7265 7665 7273 653d 4661  tras, reverse=Fa
+000037f0: 6c73 6520 293a 0a20 2020 2020 2020 2020  lse ):.         
+00003800: 2020 2020 2020 2069 6620 7061 7468 206e         if path n
+00003810: 6f74 2069 6e20 6c6f 6164 6564 3a0a 2020  ot in loaded:.  
+00003820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003830: 2020 7969 656c 6420 7061 7468 2c20 6b65    yield path, ke
+00003840: 7970 6169 722c 2063 7265 640a 2020 2020  ypair, cred.    
+00003850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003860: 6c6f 6164 6564 2e61 6464 2820 7061 7468  loaded.add( path
+00003870: 2029 0a20 2020 2020 2020 2065 7863 6570   ).        excep
+00003880: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
+00003890: 7863 3a0a 2020 2020 2020 2020 2020 2020  xc:.            
+000038a0: 6c6f 672e 6572 726f 7228 2022 4661 696c  log.error( "Fail
+000038b0: 6564 2074 6f20 6c6f 6164 206b 6579 7061  ed to load keypa
+000038c0: 6972 2066 726f 6d20 7b7d 3a20 7b7d 222e  ir from {}: {}".
+000038d0: 666f 726d 6174 2820 7061 7468 206f 7220  format( path or 
+000038e0: 5f5f 7061 636b 6167 655f 5f2c 2065 7863  __package__, exc
+000038f0: 2029 290a 2020 2020 2020 2020 2020 2020   )).            
+00003900: 7061 7373 0a20 2020 206c 6f67 2e69 6e66  pass.    log.inf
+00003910: 6f28 2022 4b65 7970 6169 7273 2020 2020  o( "Keypairs    
+00003920: 2073 6176 6564 3a20 7b7d 222e 666f 726d   saved: {}".form
+00003930: 6174 2820 7361 7665 6420 2929 0a20 2020  at( saved )).   
+00003940: 206c 6f67 2e69 6e66 6f28 2022 4b65 7970   log.info( "Keyp
+00003950: 6169 7273 2020 2020 6c6f 6164 6564 3a20  airs    loaded: 
+00003960: 7b7d 222e 666f 726d 6174 2820 6c65 6e28  {}".format( len(
+00003970: 206c 6f61 6465 6420 2929 290a 0a0a 6465   loaded )))...de
+00003980: 6620 6c69 6365 6e73 6573 5f64 6174 6128  f licenses_data(
+00003990: 2070 6174 682c 2073 746f 7265 643d 4e6f   path, stored=No
+000039a0: 6e65 2c20 636f 6e66 6972 6d3d 4e6f 6e65  ne, confirm=None
+000039b0: 2c20 6175 7468 6f72 3d4e 6f6e 652c 2063  , author=None, c
+000039c0: 6c69 656e 743d 4e6f 6e65 2c20 7072 6f64  lient=None, prod
+000039d0: 7563 743d 4e6f 6e65 2029 3a0a 2020 2020  uct=None ):.    
+000039e0: 2222 2252 6574 7572 6e73 2061 6c6c 2066  """Returns all f
+000039f0: 696c 7465 7265 6420 6c69 6365 6e73 6573  iltered licenses
+00003a00: 2061 7320 6461 7461 5b27 6c69 7374 275d   as data['list']
+00003a10: 2072 6563 6f72 6473 2c20 6d61 7962 6520   records, maybe 
+00003a20: 772f 2063 6f6e 6669 726d 206f 6620 444b  w/ confirm of DK
+00003a30: 494d 2c20 6669 6c74 6572 6564 2062 790a  IM, filtered by.
+00003a40: 2020 2020 6175 7468 6f72 202f 2063 6c69      author / cli
+00003a50: 656e 7420 286d 6179 6265 2070 6173 7365  ent (maybe passe
+00003a60: 6420 7669 6120 7061 7468 292e 2020 466f  d via path).  Fo
+00003a70: 7220 6578 616d 706c 652c 0a0a 2020 2020  r example,..    
+00003a80: 2020 2020 6c69 6365 6e73 6573 2f44 6f6d      licenses/Dom
+00003a90: 2a2f 4177 6573 6f6d 652a 2020 202d 2d3e  */Awesome*   -->
+00003aa0: 2020 416c 6c20 446f 6d69 6e69 6f6e 2052    All Dominion R
+00003ab0: 2644 2043 6f72 702e 2061 7574 686f 7265  &D Corp. authore
+00003ac0: 6420 4c69 6365 6e73 6573 2074 6f20 4177  d Licenses to Aw
+00003ad0: 6573 6f6d 652c 2049 6e63 2e0a 0a20 2020  esome, Inc...   
+00003ae0: 2054 6865 2073 616d 6520 7265 7375 6c74   The same result
+00003af0: 2077 6f75 6c64 2062 6520 7265 6163 6865   would be reache
+00003b00: 6420 6966 206c 6963 6573 6573 3f61 7574  d if liceses?aut
+00003b10: 686f 723d 446f 6d2a 2663 6c69 656e 743d  hor=Dom*&client=
+00003b20: 4177 652a 2e0a 0a20 2020 2022 2222 0a20  Awe*...    """. 
+00003b30: 2020 2064 6174 6109 0909 3d20 7b7d 0a20     data...= {}. 
+00003b40: 2020 2064 6174 615b 2274 6974 6c65 225d     data["title"]
+00003b50: 0909 3d20 224c 6963 656e 7365 7322 0a20  ..= "Licenses". 
+00003b60: 2020 2064 6174 615b 2270 6174 6822 5d09     data["path"].
+00003b70: 093d 2070 6174 680a 2020 2020 6461 7461  .= path.    data
+00003b80: 5b22 6c69 7374 225d 203d 206c 6c09 093d  ["list"] = ll..=
+00003b90: 205b 5d0a 2020 2020 6461 7461 5b22 6b65   [].    data["ke
+00003ba0: 7973 225d 0909 3d20 5b22 6175 7468 6f72  ys"]..= ["author
+00003bb0: 222c 2022 636c 6965 6e74 222c 2022 7072  ", "client", "pr
+00003bc0: 6f64 7563 7422 2c20 2273 6967 6e61 7475  oduct", "signatu
+00003bd0: 7265 222c 2022 636f 6e66 6972 6d22 2c20  re", "confirm", 
+00003be0: 226c 6963 656e 7365 225d 0a0a 2020 2020  "license"]..    
+00003bf0: 7061 7468 7365 6773 0909 093d 2070 6174  pathsegs...= pat
+00003c00: 682e 7374 7269 7028 272f 2729 2e73 706c  h.strip('/').spl
+00003c10: 6974 2827 2f27 2920 6966 2070 6174 6820  it('/') if path 
+00003c20: 656c 7365 205b 5d0a 2020 2020 6173 7365  else [].    asse
+00003c30: 7274 2030 203c 3d20 6c65 6e28 2070 6174  rt 0 <= len( pat
+00003c40: 6873 6567 7320 2920 3c3d 2032 2c20 5c0a  hsegs ) <= 2, \.
+00003c50: 2020 2020 2020 2020 2249 6e76 616c 6964          "Invalid
+00003c60: 206c 6963 656e 7365 7320 676c 6f62 2070   licenses glob p
+00003c70: 6174 6820 7b7d 3b20 6c69 6365 6e73 6573  ath {}; licenses
+00003c80: 2f3c 6175 7468 6f72 3e2f 3c63 6c69 656e  /<author>/<clien
+00003c90: 743e 2f3c 7072 6f64 7563 743e 222e 666f  t>/<product>".fo
+00003ca0: 726d 6174 2820 7061 7468 2029 0a0a 2020  rmat( path )..  
+00003cb0: 2020 2320 4974 6572 6174 6520 616c 6c20    # Iterate all 
+00003cc0: 6176 6169 6c61 626c 6520 6c69 6365 6e73  available licens
+00003cd0: 6573 2c20 6669 6c74 6572 696e 6720 6966  es, filtering if
+00003ce0: 2061 6464 6974 696f 6e61 6c20 6c69 6365   additional lice
+00003cf0: 6e73 6520 6175 7468 6f72 206e 616d 6520  nse author name 
+00003d00: 7061 7468 2063 6f6d 706f 6e65 6e74 2073  path component s
+00003d10: 7570 706c 6965 640a 2020 2020 666f 7220  upplied.    for 
+00003d20: 7369 676e 6174 7572 652c 206c 6963 2069  signature, lic i
+00003d30: 6e20 6c69 6365 6e73 6573 2820 636f 6e66  n licenses( conf
+00003d40: 6972 6d3d 4661 6c73 652c 2073 746f 7265  irm=False, store
+00003d50: 643d 7374 6f72 6564 2029 3a0a 2020 2020  d=stored ):.    
+00003d60: 2020 2020 7265 636f 7264 0909 093d 2064      record...= d
+00003d70: 6963 7428 0a20 2020 2020 2020 2020 2020  ict(.           
+00003d80: 2061 7574 686f 7209 093d 206c 6963 5b27   author..= lic['
+00003d90: 6175 7468 6f72 275d 5b27 6e61 6d65 275d  author']['name']
+00003da0: 2c0a 2020 2020 2020 2020 2020 2020 636c  ,.            cl
+00003db0: 6965 6e74 0909 3d20 6c69 635b 2763 6c69  ient..= lic['cli
+00003dc0: 656e 7427 5d5b 276e 616d 6527 5d2c 0a20  ent']['name'],. 
+00003dd0: 2020 2020 2020 2020 2020 2070 726f 6475             produ
+00003de0: 6374 0909 3d20 6c69 635b 2761 7574 686f  ct..= lic['autho
+00003df0: 7227 5d5b 2770 726f 6475 6374 275d 2c0a  r']['product'],.
+00003e00: 2020 2020 2020 2020 2020 2020 7369 676e              sign
+00003e10: 6174 7572 6509 093d 206c 6963 656e 7369  ature..= licensi
+00003e20: 6e67 2e69 6e74 6f5f 6236 3428 2073 6967  ng.into_b64( sig
+00003e30: 6e61 7475 7265 2029 2c0a 2020 2020 2020  nature ),.      
+00003e40: 2020 2020 2020 636f 6e66 6972 6d09 093d        confirm..=
+00003e50: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
+00003e60: 2020 206c 6963 656e 7365 0909 3d20 7374     license..= st
+00003e70: 7228 206c 6963 2029 2c0a 2020 2020 2020  r( lic ),.      
+00003e80: 2020 290a 2020 2020 2020 2020 6175 7468    ).        auth
+00003e90: 6f72 0909 093d 2061 7574 686f 7220 6f72  or...= author or
+00003ea0: 206c 656e 2820 7061 7468 7365 6773 2029   len( pathsegs )
+00003eb0: 203e 2030 2061 6e64 2070 6174 6873 6567   > 0 and pathseg
+00003ec0: 735b 305d 0a20 2020 2020 2020 2069 6620  s[0].        if 
+00003ed0: 6175 7468 6f72 2061 6e64 206e 6f74 2066  author and not f
+00003ee0: 6e6d 6174 6368 2e66 6e6d 6174 6368 2820  nmatch.fnmatch( 
+00003ef0: 7265 636f 7264 5b27 6175 7468 6f72 275d  record['author']
+00003f00: 2c20 6175 7468 6f72 2029 3a0a 2020 2020  , author ):.    
+00003f10: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
+00003f20: 0a20 2020 2020 2020 2063 6c69 656e 7409  .        client.
+00003f30: 0909 3d20 636c 6965 6e74 206f 7220 6c65  ..= client or le
+00003f40: 6e28 2070 6174 6873 6567 7320 2920 3e20  n( pathsegs ) > 
+00003f50: 3120 616e 6420 7061 7468 7365 6773 5b31  1 and pathsegs[1
+00003f60: 5d0a 2020 2020 2020 2020 6966 2063 6c69  ].        if cli
+00003f70: 656e 7420 616e 6420 6e6f 7420 666e 6d61  ent and not fnma
+00003f80: 7463 682e 666e 6d61 7463 6828 2072 6563  tch.fnmatch( rec
+00003f90: 6f72 645b 2763 6c69 656e 7427 5d2c 2063  ord['client'], c
+00003fa0: 6c69 656e 7420 293a 0a20 2020 2020 2020  lient ):.       
+00003fb0: 2020 2020 2063 6f6e 7469 6e75 650a 2020       continue.  
+00003fc0: 2020 2020 2020 7072 6f64 7563 7409 0909        product...
+00003fd0: 3d20 7072 6f64 7563 7420 6f72 206c 656e  = product or len
+00003fe0: 2820 7061 7468 7365 6773 2029 203e 2032  ( pathsegs ) > 2
+00003ff0: 2061 6e64 2070 6174 6873 6567 735b 325d   and pathsegs[2]
+00004000: 0a20 2020 2020 2020 2069 6620 7072 6f64  .        if prod
+00004010: 7563 7420 616e 6420 6e6f 7420 666e 6d61  uct and not fnma
+00004020: 7463 682e 666e 6d61 7463 6828 2072 6563  tch.fnmatch( rec
+00004030: 6f72 645b 2770 726f 6475 6374 275d 2c20  ord['product'], 
+00004040: 7072 6f64 7563 7420 293a 0a20 2020 2020  product ):.     
+00004050: 2020 2020 2020 2063 6f6e 7469 6e75 650a         continue.
+00004060: 2020 2020 2020 2020 2320 4166 7465 7220          # After 
+00004070: 6669 6c74 6572 696e 6720 6f75 7420 756e  filtering out un
+00004080: 696e 7465 7265 7374 696e 6720 4c69 6365  interesting Lice
+00004090: 6e73 6573 2c20 636f 6e66 6972 6d20 6966  nses, confirm if
+000040a0: 2064 6573 6972 6564 0a20 2020 2020 2020   desired.       
+000040b0: 2069 6620 636f 6e66 6972 6d3a 0a20 2020   if confirm:.   
+000040c0: 2020 2020 2020 2020 2074 7279 3a0a 2020           try:.  
+000040d0: 2020 2020 2020 2020 2020 2020 2020 6c69                li
+000040e0: 632e 7665 7269 6679 2820 636f 6e66 6972  c.verify( confir
+000040f0: 6d3d 636f 6e66 6972 6d20 290a 2020 2020  m=confirm ).    
+00004100: 2020 2020 2020 2020 6578 6365 7074 2045          except E
+00004110: 7863 6570 7469 6f6e 2061 7320 6578 633a  xception as exc:
+00004120: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004130: 2072 6563 6f72 642e 7570 6461 7465 2820   record.update( 
+00004140: 636f 6e66 6972 6d3d 7374 7228 2065 7863  confirm=str( exc
+00004150: 2029 290a 2020 2020 2020 2020 2020 2020   )).            
+00004160: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00004170: 2020 2020 2020 7265 636f 7264 2e75 7064        record.upd
+00004180: 6174 6528 2063 6f6e 6669 726d 3d54 7275  ate( confirm=Tru
+00004190: 6520 290a 2020 2020 2020 2020 6c6c 2e61  e ).        ll.a
+000041a0: 7070 656e 6428 2072 6563 6f72 6420 290a  ppend( record ).
+000041b0: 0a20 2020 2072 6574 7572 6e20 6461 7461  .    return data
+000041c0: 0a0a 0a64 6566 2063 7265 6465 6e74 6961  ...def credentia
+000041d0: 6c73 5f64 6174 6128 2070 6174 6820 293a  ls_data( path ):
+000041e0: 0a20 2020 2064 6174 6109 0909 3d20 7b7d  .    data...= {}
+000041f0: 0a20 2020 2064 6174 615b 2274 6974 6c65  .    data["title
+00004200: 225d 0909 3d20 2243 7265 6465 6e74 6961  "]..= "Credentia
+00004210: 6c73 220a 2020 2020 6461 7461 5b22 7061  ls".    data["pa
+00004220: 7468 225d 0909 3d20 7061 7468 0a20 2020  th"]..= path.   
+00004230: 2064 6174 615b 226c 6973 7422 5d20 3d20   data["list"] = 
+00004240: 6c6c 0909 3d20 5b5d 0a20 2020 2064 6174  ll..= [].    dat
+00004250: 615b 226b 6579 7322 5d09 093d 205b 226e  a["keys"]..= ["n
+00004260: 616d 6522 2c20 2275 7365 726e 616d 6522  ame", "username"
+00004270: 2c20 2270 6173 7377 6f72 6422 5d0a 0a20  , "password"].. 
+00004280: 2020 2070 6174 6873 6567 7309 0909 3d20     pathsegs...= 
+00004290: 7061 7468 2e73 7472 6970 2827 2f27 292e  path.strip('/').
+000042a0: 7370 6c69 7428 272f 2729 2069 6620 7061  split('/') if pa
+000042b0: 7468 2065 6c73 6520 5b5d 0a20 2020 2061  th else [].    a
+000042c0: 7373 6572 7420 3020 3c3d 206c 656e 2820  ssert 0 <= len( 
+000042d0: 7061 7468 7365 6773 2029 203c 3d20 312c  pathsegs ) <= 1,
+000042e0: 2022 496e 7661 6c69 6420 6372 6564 656e   "Invalid creden
+000042f0: 7469 616c 7320 7061 7468 207b 7d22 2e66  tials path {}".f
+00004300: 6f72 6d61 7428 2070 6174 6820 290a 0a20  ormat( path ).. 
+00004310: 2020 2066 6f72 206e 616d 652c 2875 7365     for name,(use
+00004320: 726e 616d 652c 7061 7373 776f 7264 2920  rname,password) 
+00004330: 696e 2063 7265 6465 6e74 6961 6c73 2829  in credentials()
+00004340: 3a0a 2020 2020 2020 2020 6966 2070 6174  :.        if pat
+00004350: 6873 6567 7320 616e 6420 7061 7468 7365  hsegs and pathse
+00004360: 6773 5b30 5d20 616e 6420 6e6f 7420 666e  gs[0] and not fn
+00004370: 6d61 7463 682e 666e 6d61 7463 6828 206e  match.fnmatch( n
+00004380: 616d 652c 2070 6174 6873 6567 735b 305d  ame, pathsegs[0]
+00004390: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
+000043a0: 6c6f 672e 696e 666f 2820 2243 7265 6465  log.info( "Crede
+000043b0: 6e74 6961 6c20 7b7d 2064 6964 6e27 7420  ntial {} didn't 
+000043c0: 6d61 7463 6820 7b7d 222e 666f 726d 6174  match {}".format
+000043d0: 2820 6e61 6d65 2c20 7061 7468 2029 290a  ( name, path )).
+000043e0: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
+000043f0: 696e 7565 0a20 2020 2020 2020 2072 6563  inue.        rec
+00004400: 6f72 6409 0909 3d20 6469 6374 280a 2020  ord...= dict(.  
+00004410: 2020 2020 2020 2020 2020 6e61 6d65 093d            name.=
+00004420: 206e 616d 652c 0a20 2020 2020 2020 2020   name,.         
+00004430: 2020 2075 7365 726e 616d 6509 3d20 7573     username.= us
+00004440: 6572 6e61 6d65 2c0a 2020 2020 2020 2020  ername,.        
+00004450: 2020 2020 7061 7373 776f 7264 093d 2070      password.= p
+00004460: 6173 7377 6f72 642c 0a20 2020 2020 2020  assword,.       
+00004470: 2029 0a20 2020 2020 2020 206c 6c2e 6170   ).        ll.ap
+00004480: 7065 6e64 2820 7265 636f 7264 2029 0a0a  pend( record )..
+00004490: 2020 2020 7265 7475 726e 2064 6174 610a      return data.
+000044a0: 0a0a 6465 6620 6b65 7970 6169 7273 5f64  ..def keypairs_d
+000044b0: 6174 6128 2070 6174 6820 293a 0a20 2020  ata( path ):.   
+000044c0: 2064 6174 6109 0909 3d20 7b7d 0a20 2020   data...= {}.   
+000044d0: 2064 6174 615b 2274 6974 6c65 225d 0909   data["title"]..
+000044e0: 3d20 224b 6579 7061 6972 7322 0a20 2020  = "Keypairs".   
+000044f0: 2064 6174 615b 2270 6174 6822 5d09 093d   data["path"]..=
+00004500: 2070 6174 680a 2020 2020 6461 7461 5b22   path.    data["
+00004510: 6c69 7374 225d 203d 206c 6c09 093d 205b  list"] = ll..= [
+00004520: 5d0a 2020 2020 6461 7461 5b22 6b65 7973  ].    data["keys
+00004530: 225d 0909 3d20 5b22 6e61 6d65 222c 2022  "]..= ["name", "
+00004540: 7075 626c 6963 5f6b 6579 222c 2022 6372  public_key", "cr
+00004550: 6564 656e 7469 616c 7322 5d0a 0a20 2020  edentials"]..   
+00004560: 2070 6174 6873 6567 7309 0909 3d20 7061   pathsegs...= pa
+00004570: 7468 2e73 7472 6970 2827 2f27 292e 7370  th.strip('/').sp
+00004580: 6c69 7428 272f 2729 2069 6620 7061 7468  lit('/') if path
+00004590: 2065 6c73 6520 5b5d 0a20 2020 2061 7373   else [].    ass
+000045a0: 6572 7420 3020 3c3d 206c 656e 2820 7061  ert 0 <= len( pa
+000045b0: 7468 7365 6773 2029 203c 3d20 312c 2022  thsegs ) <= 1, "
+000045c0: 496e 7661 6c69 6420 6b65 7970 6169 7273  Invalid keypairs
+000045d0: 2070 6174 6820 7b7d 222e 666f 726d 6174   path {}".format
+000045e0: 2820 7061 7468 2029 0a0a 2020 2020 2320  ( path )..    # 
+000045f0: 4765 7420 616c 6c20 6372 6564 656e 7469  Get all credenti
+00004600: 616c 7320 696e 746f 2063 7265 6473 3a20  als into creds: 
+00004610: 7b20 6e61 6d65 3a20 2875 7365 726e 616d  { name: (usernam
+00004620: 652c 7061 7373 776f 7264 292c 202e 2e2e  e,password), ...
+00004630: 207d 2c20 616e 6420 6275 696c 6420 6120   }, and build a 
+00004640: 7265 7665 7273 652d 6c6f 6f6b 7570 2064  reverse-lookup d
+00004650: 6963 740a 2020 2020 2320 6372 6564 735f  ict.    # creds_
+00004660: 7265 7665 7273 653a 207b 2028 7573 6572  reverse: { (user
+00004670: 6e61 6d65 2c70 6173 7377 6f72 6429 3a20  name,password): 
+00004680: 6e61 6d65 2c20 2e2e 2e20 7d0a 2020 2020  name, ... }.    
+00004690: 6372 6564 7309 0909 3d20 6469 6374 2820  creds...= dict( 
+000046a0: 6372 6564 656e 7469 616c 7328 2920 290a  credentials() ).
+000046b0: 2020 2020 6372 6564 735f 7265 7665 7273      creds_revers
+000046c0: 6509 093d 207b 2076 3a20 6b20 666f 7220  e..= { v: k for 
+000046d0: 6b2c 7620 696e 2063 7265 6473 2e69 7465  k,v in creds.ite
+000046e0: 6d73 2829 207d 0a0a 2020 2020 6c6f 672e  ms() }..    log.
+000046f0: 696e 666f 2820 224b 6579 7061 6972 7320  info( "Keypairs 
+00004700: 6461 7461 2077 2f20 7b7d 2063 7265 6465  data w/ {} crede
+00004710: 6e74 6961 6c3a 222e 666f 726d 6174 2820  ntial:".format( 
+00004720: 6c65 6e28 2063 7265 6473 5f72 6576 6572  len( creds_rever
+00004730: 7365 2029 2929 0a20 2020 2066 6f72 206e  se ))).    for n
+00004740: 616d 652c 6b65 7970 6169 722c 6372 6564  ame,keypair,cred
+00004750: 2069 6e20 6b65 7970 6169 7273 2829 3a0a   in keypairs():.
+00004760: 2020 2020 2020 2020 6c6f 672e 696e 666f          log.info
+00004770: 2822 466f 756e 6420 6b65 7970 6169 723a  ("Found keypair:
+00004780: 207b 2172 7d22 2e66 6f72 6d61 7428 2028   {!r}".format( (
+00004790: 6e61 6d65 2c6b 6579 7061 6972 2c63 7265  name,keypair,cre
+000047a0: 6429 2029 290a 2020 2020 2020 2020 6966  d) )).        if
+000047b0: 2070 6174 6873 6567 7320 616e 6420 7061   pathsegs and pa
+000047c0: 7468 7365 6773 5b30 5d20 616e 6420 6e6f  thsegs[0] and no
+000047d0: 7420 666e 6d61 7463 682e 666e 6d61 7463  t fnmatch.fnmatc
+000047e0: 6828 206e 616d 652c 2070 6174 6873 6567  h( name, pathseg
+000047f0: 735b 305d 2029 3a0a 2020 2020 2020 2020  s[0] ):.        
+00004800: 2020 2020 6c6f 672e 696e 666f 2820 2243      log.info( "C
+00004810: 7265 6465 6e74 6961 6c20 7b7d 2064 6964  redential {} did
+00004820: 6e27 7420 6d61 7463 6820 7b7d 222e 666f  n't match {}".fo
+00004830: 726d 6174 2820 6e61 6d65 2c20 7061 7468  rmat( name, path
+00004840: 2029 290a 2020 2020 2020 2020 2020 2020   )).            
+00004850: 636f 6e74 696e 7565 0a20 2020 2020 2020  continue.       
+00004860: 2072 6563 6f72 6409 0909 3d20 6469 6374   record...= dict
+00004870: 280a 2020 2020 2020 2020 2020 2020 6e61  (.            na
+00004880: 6d65 093d 206e 616d 652c 0a20 2020 2020  me.= name,.     
+00004890: 2020 2020 2020 2070 7562 6c69 635f 6b65         public_ke
+000048a0: 7909 3d20 6c69 6365 6e73 696e 672e 696e  y.= licensing.in
+000048b0: 746f 5f62 3634 2820 6b65 7970 6169 722e  to_b64( keypair.
+000048c0: 696e 746f 5f6b 6579 7061 6972 2820 2a2a  into_keypair( **
+000048d0: 6372 6564 2029 2e76 6b20 292c 0a20 2020  cred ).vk ),.   
+000048e0: 2020 2020 2020 2020 2063 7265 6465 6e74           credent
+000048f0: 6961 6c73 093d 2063 7265 6473 5f72 6576  ials.= creds_rev
+00004900: 6572 7365 2e67 6574 2820 2863 7265 645b  erse.get( (cred[
+00004910: 2775 7365 726e 616d 6527 5d2c 2063 7265  'username'], cre
+00004920: 645b 2770 6173 7377 6f72 6427 5d29 2c20  d['password']), 
+00004930: 2728 756e 6b6e 6f77 6e29 2720 292c 0a20  '(unknown)' ),. 
+00004940: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00004950: 206c 6c2e 6170 7065 6e64 2820 7265 636f   ll.append( reco
+00004960: 7264 2029 0a0a 2020 2020 7265 7475 726e  rd )..    return
+00004970: 2064 6174 610a 0a0a 2320 5365 7420 7570   data...# Set up
+00004980: 2073 6967 6e61 6c20 6861 6e64 6c69 6e67   signal handling
+00004990: 2028 6c6f 6720 726f 7461 7469 6f6e 2c20   (log rotation, 
+000049a0: 6c6f 6720 6c65 7665 6c2c 2065 7463 2e29  log level, etc.)
+000049b0: 0a23 204f 7574 7075 7420 6c6f 6767 696e  .# Output loggin
+000049c0: 6720 746f 2061 2066 696c 652c 2061 6e64  g to a file, and
+000049d0: 2068 616e 646c 6520 554e 4958 2d79 206c   handle UNIX-y l
+000049e0: 6f67 2066 696c 6520 726f 7461 7469 6f6e  og file rotation
+000049f0: 2076 6961 2027 6c6f 6772 6f74 6174 6527   via 'logrotate'
+00004a00: 2c20 7768 6963 6820 7365 6e64 730a 2320  , which sends.# 
+00004a10: 7369 676e 616c 7320 746f 2069 6e64 6963  signals to indic
+00004a20: 6174 6520 7468 6174 2061 2073 6572 7669  ate that a servi
+00004a30: 6365 2773 206c 6f67 2066 696c 6520 6861  ce's log file ha
+00004a40: 7320 6265 656e 206d 6f76 6564 2f72 656e  s been moved/ren
+00004a50: 616d 6564 2061 6e64 2069 7420 7368 6f75  amed and it shou
+00004a60: 6c64 2072 652d 6f70 656e 0a0a 7570 7469  ld re-open..upti
+00004a70: 6d65 5f62 6173 6973 0909 093d 2074 696d  me_basis...= tim
+00004a80: 6572 2829 0a75 7074 696d 655f 7369 676e  er().uptime_sign
+00004a90: 616c 6c65 6409 093d 2046 616c 7365 0a73  alled..= False.s
+00004aa0: 6875 7464 6f77 6e5f 7369 676e 616c 6c65  hutdown_signalle
+00004ab0: 6409 093d 2046 616c 7365 0a6c 6f67 726f  d..= False.logro
+00004ac0: 7461 7465 5f73 6967 6e61 6c6c 6564 0909  tate_signalled..
+00004ad0: 3d20 4661 6c73 650a 6c65 7665 6c6d 6170  = False.levelmap
+00004ae0: 5f63 6861 6e67 6509 0909 3d20 3020 2023  _change...= 0  #
+00004af0: 206d 6179 2062 6563 6f6d 6520 2b27 7665   may become +'ve
+00004b00: 2f2d 2776 650a 0a0a 6465 6620 7570 7469  /-'ve...def upti
+00004b10: 6d65 5f72 6571 7565 7374 2820 7369 676e  me_request( sign
+00004b20: 756d 2c20 6672 616d 6520 293a 0a20 2020  um, frame ):.   
+00004b30: 2067 6c6f 6261 6c20 7570 7469 6d65 5f73   global uptime_s
+00004b40: 6967 6e61 6c6c 6564 0a20 2020 2075 7074  ignalled.    upt
+00004b50: 696d 655f 7369 676e 616c 6c65 6409 093d  ime_signalled..=
+00004b60: 2054 7275 650a 0a0a 6465 6620 7368 7574   True...def shut
+00004b70: 646f 776e 5f72 6571 7565 7374 2820 7369  down_request( si
+00004b80: 676e 756d 2c20 6672 616d 6520 293a 0a20  gnum, frame ):. 
+00004b90: 2020 2067 6c6f 6261 6c20 7368 7574 646f     global shutdo
+00004ba0: 776e 5f73 6967 6e61 6c6c 6564 0a20 2020  wn_signalled.   
+00004bb0: 2073 6875 7464 6f77 6e5f 7369 676e 616c   shutdown_signal
+00004bc0: 6c65 6409 093d 2054 7275 650a 0a0a 6465  led..= True...de
+00004bd0: 6620 6c6f 6772 6f74 6174 655f 7265 7175  f logrotate_requ
+00004be0: 6573 7428 2073 6967 6e75 6d2c 2066 7261  est( signum, fra
+00004bf0: 6d65 2029 3a0a 2020 2020 676c 6f62 616c  me ):.    global
+00004c00: 206c 6f67 726f 7461 7465 5f73 6967 6e61   logrotate_signa
+00004c10: 6c6c 6564 0a20 2020 206c 6f67 726f 7461  lled.    logrota
+00004c20: 7465 5f73 6967 6e61 6c6c 6564 0909 3d20  te_signalled..= 
+00004c30: 5472 7565 0a0a 0a64 6566 206c 6f67 6c65  True...def logle
+00004c40: 7665 6c75 705f 7265 7175 6573 7428 2073  velup_request( s
+00004c50: 6967 6e75 6d2c 2066 7261 6d65 2029 3a0a  ignum, frame ):.
+00004c60: 2020 2020 676c 6f62 616c 206c 6576 656c      global level
+00004c70: 6d61 705f 6368 616e 6765 0a20 2020 206c  map_change.    l
+00004c80: 6576 656c 6d61 705f 6368 616e 6765 0920  evelmap_change. 
+00004c90: 2020 2020 2020 2b3d 2031 0a0a 0a64 6566        += 1...def
+00004ca0: 206c 6f67 6c65 7665 6c64 6e5f 7265 7175   logleveldn_requ
+00004cb0: 6573 7428 2073 6967 6e75 6d2c 2066 7261  est( signum, fra
+00004cc0: 6d65 2029 3a0a 2020 2020 676c 6f62 616c  me ):.    global
+00004cd0: 206c 6576 656c 6d61 705f 6368 616e 6765   levelmap_change
+00004ce0: 0a20 2020 206c 6576 656c 6d61 705f 6368  .    levelmap_ch
+00004cf0: 616e 6765 0920 2020 2020 2020 2d3d 2031  ange.       -= 1
+00004d00: 0a0a 0a64 6566 2073 6967 6e61 6c5f 7365  ...def signal_se
+00004d10: 7276 6963 6528 293a 0a20 2020 2022 2222  rvice():.    """
+00004d20: 5365 7276 6963 6520 6b6e 6f77 6e20 7369  Service known si
+00004d30: 676e 616c 732e 2020 5768 656e 206c 6f67  gnals.  When log
+00004d40: 6769 6e67 2c20 6465 6661 756c 7420 746f  ging, default to
+00004d50: 206c 6f67 2061 7420 5741 524e 494e 472c   log at WARNING,
+00004d60: 2062 7574 2065 6e73 7572 6520 7468 650a   but ensure the.
+00004d70: 2020 2020 6d65 7373 6167 6520 6973 2073      message is s
+00004d80: 6565 6e20 6966 2068 6967 6865 7220 2865  een if higher (e
+00004d90: 672e 2057 4152 4e49 4e47 292e 2020 5375  g. WARNING).  Su
+00004da0: 7070 6f72 7420 6265 696e 6720 696e 2075  pport being in u
+00004db0: 6e6b 6e6f 776e 206c 6f67 6769 6e67 0a20  nknown logging. 
+00004dc0: 2020 206c 6576 656c 7320 7768 656e 2069     levels when i
+00004dd0: 6e2f 6465 6372 6561 7369 6e67 2e0a 0a20  n/decreasing... 
+00004de0: 2020 2022 2222 0a20 2020 2067 6c6f 6261     """.    globa
+00004df0: 6c20 6c65 7665 6c6d 6170 5f63 6861 6e67  l levelmap_chang
+00004e00: 650a 2020 2020 6966 206c 6576 656c 6d61  e.    if levelma
+00004e10: 705f 6368 616e 6765 3a0a 2020 2020 2020  p_change:.      
+00004e20: 2020 726f 6f74 6c6f 6709 0909 3d20 6c6f    rootlog...= lo
+00004e30: 6767 696e 672e 6765 744c 6f67 6765 7228  gging.getLogger(
+00004e40: 290a 2020 2020 2020 2020 6163 7475 616c  ).        actual
+00004e50: 0909 093d 2072 6f6f 746c 6f67 2e67 6574  ...= rootlog.get
+00004e60: 4566 6665 6374 6976 654c 6576 656c 2829  EffectiveLevel()
+00004e70: 0a20 2020 2020 2020 2023 2046 696e 6420  .        # Find 
+00004e80: 7468 6520 6375 7272 656e 7420 6c6f 675f  the current log_
+00004e90: 6c65 7665 6c6d 6170 206b 6579 2077 2f20  levelmap key w/ 
+00004ea0: 6120 6c65 7665 6c20 7661 6c75 6520 6e65  a level value ne
+00004eb0: 6172 6573 7420 6f75 7220 6375 7272 656e  arest our curren
+00004ec0: 7420 6163 7475 616c 206c 6576 656c 2e20  t actual level. 
+00004ed0: 2044 6566 6175 6c74 2074 6f20 302e 0a20   Default to 0.. 
+00004ee0: 2020 2020 2020 206b 6579 2c64 6966 0909         key,dif..
+00004ef0: 093d 2030 2c31 3030 300a 2020 2020 2020  .= 0,1000.      
+00004f00: 2020 666f 7220 6b2c 6c76 6c20 696e 206c    for k,lvl in l
+00004f10: 6f67 5f6c 6576 656c 6d61 702e 6974 656d  og_levelmap.item
+00004f20: 7328 293a 0a20 2020 2020 2020 2020 2020  s():.           
+00004f30: 2069 6620 6162 7328 206c 766c 202d 2061   if abs( lvl - a
+00004f40: 6374 7561 6c20 2920 3c20 6469 663a 0a20  ctual ) < dif:. 
+00004f50: 2020 2020 2020 2020 2020 2020 2020 206b                 k
+00004f60: 6579 0909 3d20 6b0a 2020 2020 2020 2020  ey..= k.        
+00004f70: 2320 4765 7420 616e 2061 7661 696c 6162  # Get an availab
+00004f80: 6c65 206c 6f67 5f6c 6576 656c 2075 702f  le log_level up/
+00004f90: 646f 776e 2066 726f 6d20 7468 6520 6375  down from the cu
+00004fa0: 7272 656e 746c 7920 6163 7469 7665 206f  rrently active o
+00004fb0: 6e65 0a20 2020 2020 2020 2064 6573 6972  ne.        desir
+00004fc0: 6564 0909 093d 206c 6f67 5f6c 6576 656c  ed...= log_level
+00004fd0: 2820 6b65 7920 2b20 6c65 7665 6c6d 6170  ( key + levelmap
+00004fe0: 5f63 6861 6e67 6520 290a 2020 2020 2020  _change ).      
+00004ff0: 2020 6966 2061 6374 7561 6c20 213d 2064    if actual != d
+00005000: 6573 6972 6564 3a0a 2020 2020 2020 2020  esired:.        
+00005010: 2020 2020 726f 6f74 6c6f 672e 7365 744c      rootlog.setL
+00005020: 6576 656c 2820 6465 7369 7265 6420 290a  evel( desired ).
+00005030: 2020 2020 2020 2020 6c65 7665 6c6d 6170          levelmap
+00005040: 5f63 6861 6e67 6509 093d 2030 0a0a 2020  _change..= 0..  
+00005050: 2020 676c 6f62 616c 206c 6f67 726f 7461    global logrota
+00005060: 7465 5f73 6967 6e61 6c6c 6564 0a20 2020  te_signalled.   
+00005070: 2067 6c6f 6261 6c20 7570 7469 6d65 5f73   global uptime_s
+00005080: 6967 6e61 6c6c 6564 0a20 2020 2069 6620  ignalled.    if 
+00005090: 6c6f 6772 6f74 6174 655f 7369 676e 616c  logrotate_signal
+000050a0: 6c65 643a 0a20 2020 2020 2020 206c 6f67  led:.        log
+000050b0: 726f 7461 7465 5f73 6967 6e61 6c6c 6564  rotate_signalled
+000050c0: 093d 2046 616c 7365 0a20 2020 2020 2020  .= False.       
+000050d0: 2075 7074 696d 655f 7369 676e 616c 6c65   uptime_signalle
+000050e0: 6409 3d20 5472 7565 0a0a 2020 2020 2020  d.= True..      
+000050f0: 2020 726f 6f74 6c6f 6709 0909 3d20 6c6f    rootlog...= lo
+00005100: 6767 696e 672e 6765 744c 6f67 6765 7228  gging.getLogger(
+00005110: 290a 2020 2020 2020 2020 6163 7475 616c  ).        actual
+00005120: 0909 093d 2072 6f6f 746c 6f67 2e67 6574  ...= rootlog.get
+00005130: 4566 6665 6374 6976 654c 6576 656c 2829  EffectiveLevel()
+00005140: 0a20 2020 2020 2020 2072 6f6f 746c 6f67  .        rootlog
+00005150: 2e6c 6f67 2820 6d61 7828 206c 6f67 6769  .log( max( loggi
+00005160: 6e67 2e57 4152 4e49 4e47 2c20 6163 7475  ng.WARNING, actu
+00005170: 616c 2029 2c20 2252 6f74 6174 696e 6720  al ), "Rotating 
+00005180: 6c6f 6720 6669 6c65 7320 6475 6520 746f  log files due to
+00005190: 2073 6967 6e61 6c22 2029 0a20 2020 2020   signal" ).     
+000051a0: 2020 2066 6f72 2068 646c 7220 696e 206c     for hdlr in l
+000051b0: 6f67 6769 6e67 2e72 6f6f 742e 6861 6e64  ogging.root.hand
+000051c0: 6c65 7273 3a0a 2020 2020 2020 2020 2020  lers:.          
+000051d0: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+000051e0: 2068 646c 722c 206c 6f67 6769 6e67 2e46   hdlr, logging.F
+000051f0: 696c 6548 616e 646c 6572 2029 3a0a 2020  ileHandler ):.  
+00005200: 2020 2020 2020 2020 2020 2020 2020 6864                hd
+00005210: 6c72 2e63 6c6f 7365 2829 0a0a 2020 2020  lr.close()..    
+00005220: 676c 6f62 616c 2075 7074 696d 655f 6261  global uptime_ba
+00005230: 7369 730a 2020 2020 6966 2075 7074 696d  sis.    if uptim
+00005240: 655f 7369 676e 616c 6c65 643a 0a20 2020  e_signalled:.   
+00005250: 2020 2020 2075 7074 696d 655f 7369 676e       uptime_sign
+00005260: 616c 6c65 6409 3d20 4661 6c73 650a 2020  alled.= False.  
+00005270: 2020 2020 2020 7570 7469 6d65 0909 093d        uptime...=
+00005280: 2074 696d 6572 2829 202d 2075 7074 696d   timer() - uptim
+00005290: 655f 6261 7369 730a 0a20 2020 2020 2020  e_basis..       
+000052a0: 2072 6f6f 746c 6f67 0909 093d 206c 6f67   rootlog...= log
+000052b0: 6769 6e67 2e67 6574 4c6f 6767 6572 2829  ging.getLogger()
+000052c0: 0a20 2020 2020 2020 2061 6374 7561 6c09  .        actual.
+000052d0: 0909 3d20 726f 6f74 6c6f 672e 6765 7445  ..= rootlog.getE
+000052e0: 6666 6563 7469 7665 4c65 7665 6c28 290a  ffectiveLevel().
+000052f0: 2020 2020 2020 2020 726f 6f74 6c6f 672e          rootlog.
+00005300: 6c6f 6728 206d 6178 2820 6c6f 6767 696e  log( max( loggin
+00005310: 672e 5741 524e 494e 472c 2061 6374 7561  g.WARNING, actua
+00005320: 6c20 292c 2022 5570 7469 6d65 3a20 2533  l ), "Uptime: %3
+00005330: 643a 2530 3264 3a25 3036 2e33 6622 2c0a  d:%02d:%06.3f",.
+00005340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005350: 2020 2020 2069 6e74 2820 7570 7469 6d65       int( uptime
+00005360: 202f 2f20 3336 3030 2029 2c20 696e 7428   // 3600 ), int(
+00005370: 2075 7074 696d 6520 2520 3336 3030 202f   uptime % 3600 /
+00005380: 2f20 3630 2029 2c20 7570 7469 6d65 2025  / 60 ), uptime %
+00005390: 2036 3020 290a 0a0a 7369 676e 616c 2e73   60 )...signal.s
+000053a0: 6967 6e61 6c28 2073 6967 6e61 6c2e 5349  ignal( signal.SI
+000053b0: 4748 5550 2c20 206c 6f67 726f 7461 7465  GHUP,  logrotate
+000053c0: 5f72 6571 7565 7374 2029 0a73 6967 6e61  _request ).signa
+000053d0: 6c2e 7369 676e 616c 2820 7369 676e 616c  l.signal( signal
+000053e0: 2e53 4947 5553 5231 2c20 6c6f 676c 6576  .SIGUSR1, loglev
+000053f0: 656c 7570 5f72 6571 7565 7374 2029 0a73  elup_request ).s
+00005400: 6967 6e61 6c2e 7369 676e 616c 2820 7369  ignal.signal( si
+00005410: 676e 616c 2e53 4947 5553 5232 2c20 6c6f  gnal.SIGUSR2, lo
+00005420: 676c 6576 656c 646e 5f72 6571 7565 7374  gleveldn_request
+00005430: 2029 0a73 6967 6e61 6c2e 7369 676e 616c   ).signal.signal
+00005440: 2820 7369 676e 616c 2e53 4947 5445 524d  ( signal.SIGTERM
+00005450: 2c20 7368 7574 646f 776e 5f72 6571 7565  , shutdown_reque
+00005460: 7374 2029 0a73 6967 6e61 6c2e 7369 676e  st ).signal.sign
+00005470: 616c 2820 7369 676e 616c 2e53 4947 5552  al( signal.SIGUR
+00005480: 472c 2020 7570 7469 6d65 5f72 6571 7565  G,  uptime_reque
+00005490: 7374 2029 0a0a 6e6f 7709 0909 093d 2074  st )..now....= t
+000054a0: 696d 6572 2829 0a0a 0a64 6566 2064 6179  imer()...def day
+000054b0: 7469 6d65 2820 7473 2029 3a0a 2020 2020  time( ts ):.    
+000054c0: 7265 7475 726e 2054 696d 6573 7461 6d70  return Timestamp
+000054d0: 2820 7473 2029 0a0a 230a 2320 4375 7273  ( ts )..#.# Curs
+000054e0: 6573 2d62 6173 6564 2054 6578 7475 616c  es-based Textual
+000054f0: 2055 492e 0a23 0a0a 0a64 6566 206d 6573   UI..#...def mes
+00005500: 7361 6765 2820 7769 6e64 6f77 2c20 7465  sage( window, te
+00005510: 7874 2c20 726f 7720 3d20 3233 2c20 636f  xt, row = 23, co
+00005520: 6c20 3d20 302c 2063 6c65 6172 203d 2054  l = 0, clear = T
+00005530: 7275 6520 293a 0a20 2020 2072 6f77 732c  rue ):.    rows,
+00005540: 636f 6c73 0909 093d 2077 696e 646f 772e  cols...= window.
+00005550: 6765 746d 6178 7978 2829 0a20 2020 2069  getmaxyx().    i
+00005560: 6620 636f 6c20 3c20 2d6c 656e 2820 7465  f col < -len( te
+00005570: 7874 2029 206f 7220 726f 7720 3c20 3020  xt ) or row < 0 
+00005580: 6f72 2072 6f77 203e 3d20 726f 7773 206f  or row >= rows o
+00005590: 7220 636f 6c20 3e3d 2063 6f6c 733a 0a20  r col >= cols:. 
+000055a0: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
+000055b0: 2020 6966 2063 6f6c 203c 2030 3a0a 2020    if col < 0:.  
+000055c0: 2020 2020 2020 7465 7874 0909 093d 2074        text...= t
+000055d0: 6578 745b 2d63 6f6c 3a5d 0a20 2020 2020  ext[-col:].     
+000055e0: 2020 2063 6f6c 0909 093d 2030 0a20 2020     col...= 0.   
+000055f0: 2074 7279 3a0a 2020 2020 2020 2020 7769   try:.        wi
+00005600: 6e64 6f77 2e61 6464 7374 7228 2069 6e74  ndow.addstr( int
+00005610: 2820 726f 7720 292c 2069 6e74 2820 636f  ( row ), int( co
+00005620: 6c20 292c 2074 6578 745b 3a63 6f6c 732d  l ), text[:cols-
+00005630: 636f 6c5d 2029 0a20 2020 2020 2020 2069  col] ).        i
+00005640: 6620 636c 6561 723a 0a20 2020 2020 2020  f clear:.       
+00005650: 2020 2020 2077 696e 646f 772e 636c 7274       window.clrt
+00005660: 6f65 6f6c 2829 0a20 2020 2065 7863 6570  oeol().    excep
+00005670: 7420 4578 6365 7074 696f 6e3a 0a20 2020  t Exception:.   
+00005680: 2020 2020 2070 6173 730a 0a0a 230a 2320       pass...#.# 
+00005690: 7061 6e7b 7369 7a2c 6c6f 637d 202d 2d20  pan{siz,loc} -- 
+000056a0: 636f 6d70 7574 6520 6170 7072 6f70 7269  compute appropri
+000056b0: 6174 6520 7369 7a65 2061 6e64 206c 6f63  ate size and loc
+000056c0: 6174 696f 6e20 666f 7220 7365 6e73 6f72  ation for sensor
+000056d0: 2064 6574 6169 6c20 7061 6e65 6c0a 230a   detail panel.#.
+000056e0: 6465 6620 7061 6e73 697a 2820 726f 7773  def pansiz( rows
+000056f0: 2c20 636f 6c73 2029 3a0a 2020 2020 7265  , cols ):.    re
+00005700: 7475 726e 2072 6f77 7320 2a20 3920 2f2f  turn rows * 9 //
+00005710: 2031 302c 2063 6f6c 7320 2f2f 2033 0a0a   10, cols // 3..
+00005720: 0a64 6566 2070 616e 6c6f 6328 2063 2c20  .def panloc( c, 
+00005730: 726f 7773 2c20 636f 6c73 2029 3a0a 2020  rows, cols ):.  
+00005740: 2020 7265 7475 726e 2072 6f77 732f 2f31    return rows//1
+00005750: 352c 2028 2063 203c 2063 6f6c 732f 2f32  5, ( c < cols//2
+00005760: 2029 2061 6e64 2028 2063 6f6c 732f 2f32   ) and ( cols//2
+00005770: 202b 2063 6f6c 732f 2f31 3020 2920 6f72   + cols//10 ) or
+00005780: 2028 2030 202b 2063 6f6c 732f 2f31 3020   ( 0 + cols//10 
+00005790: 290a 0a0a 6465 6620 7478 7428 2077 696e  )...def txt( win
+000057a0: 2c20 636f 6e66 6967 2029 3a0a 0a20 2020  , config ):..   
+000057b0: 2067 6c6f 6261 6c20 6e6f 770a 2020 2020   global now.    
+000057c0: 6c61 7374 0909 093d 206e 6f77 0a20 2020  last...= now.   
+000057d0: 2073 656c 6563 7465 6409 0909 3d20 300a   selected...= 0.
+000057e0: 0a20 2020 2072 6f77 732c 2063 6f6c 7309  .    rows, cols.
+000057f0: 0909 3d20 302c 2030 0a0a 2020 2020 6c6f  ..= 0, 0..    lo
+00005800: 672e 696e 666f 2822 7468 7265 6164 733a  g.info("threads:
+00005810: 2025 3264 3a20 2573 2220 2520 280a 2020   %2d: %s" % (.  
+00005820: 2020 2020 2020 7468 7265 6164 696e 672e        threading.
+00005830: 6163 7469 7665 5f63 6f75 6e74 2829 2c0a  active_count(),.
+00005840: 2020 2020 2020 2020 272c 2027 2e6a 6f69          ', '.joi
+00005850: 6e28 205b 2074 2e6e 616d 6520 666f 7220  n( [ t.name for 
+00005860: 7420 696e 2074 6872 6561 6469 6e67 2e65  t in threading.e
+00005870: 6e75 6d65 7261 7465 2829 205d 2029 2929  numerate() ] )))
+00005880: 0a0a 2020 2020 6469 7370 6c61 7909 0909  ..    display...
+00005890: 3d20 276c 6963 656e 7365 7327 0909 2320  = 'licenses'..# 
+000058a0: 5374 6172 7420 6f66 6620 6469 7370 6c61  Start off displa
+000058b0: 7969 6e67 204c 6963 656e 7365 730a 2020  ying Licenses.  
+000058c0: 2020 696e 7075 7409 0909 3d20 300a 2020    input...= 0.  
+000058d0: 2020 6465 6c74 6109 0909 3d20 302e 300a    delta...= 0.0.
+000058e0: 2020 2020 7061 6e73 656c 0909 093d 204e      pansel...= N
+000058f0: 6f6e 650a 2020 2020 7768 696c 6520 6e6f  one.    while no
+00005900: 7420 636f 6e66 6967 2e67 6574 2820 2764  t config.get( 'd
+00005910: 6f6e 6527 2029 3a0a 2020 2020 2020 2020  one' ):.        
+00005920: 6d65 7373 6167 6528 2077 696e 2c20 2225  message( win, "%
+00005930: 7320 2825 372e 3366 293a 2028 2533 6420  s (%7.3f): (%3d 
+00005940: 3d3d 2027 2563 2729 2051 7569 7420 5b71  == '%c') Quit [q
+00005950: 792f 6e5d 3f22 0a20 2020 2020 2020 2020  y/n]?".         
+00005960: 2020 2020 2020 2020 2520 2820 2064 6179          % (  day
+00005970: 7469 6d65 2820 6e6f 7720 292c 2064 656c  time( now ), del
+00005980: 7461 2c0a 2020 2020 2020 2020 2020 2020  ta,.            
+00005990: 2020 2020 2020 2020 2020 696e 7075 742c            input,
+000059a0: 2063 7572 7365 732e 6173 6369 692e 6973   curses.ascii.is
+000059b0: 7072 696e 7428 2069 6e70 7574 2029 2061  print( input ) a
+000059c0: 6e64 2063 6872 2820 696e 7075 7420 2920  nd chr( input ) 
+000059d0: 6f72 2027 3f27 292c 0a20 2020 2020 2020  or '?'),.       
+000059e0: 2020 2020 2020 2020 2020 726f 7720 3d20            row = 
+000059f0: 302c 2063 6c65 6172 203d 2046 616c 7365  0, clear = False
+00005a00: 2029 0a0a 2020 2020 2020 2020 6375 7273   )..        curs
+00005a10: 6573 2e70 616e 656c 2e75 7064 6174 655f  es.panel.update_
+00005a20: 7061 6e65 6c73 2829 0a20 2020 2020 2020  panels().       
+00005a30: 2063 7572 7365 732e 646f 7570 6461 7465   curses.doupdate
+00005a40: 2829 0a0a 2020 2020 2020 2020 2320 456e  ()..        # En
+00005a50: 6420 6f66 2064 6973 706c 6179 206c 6f6f  d of display loo
+00005a60: 703b 2064 6973 706c 6179 2075 7064 6174  p; display updat
+00005a70: 6564 3b20 4265 6769 6e6e 696e 6720 6f66  ed; Beginning of
+00005a80: 206e 6578 7420 6c6f 6f70 3b20 6177 6169   next loop; awai
+00005a90: 7420 696e 7075 740a 2020 2020 2020 2020  t input.        
+00005aa0: 696e 7075 7409 0909 3d20 7769 6e2e 6765  input...= win.ge
+00005ab0: 7463 6828 290a 0a20 2020 2020 2020 2023  tch()..        #
+00005ac0: 2052 6566 7265 7368 2074 6865 2074 6869   Refresh the thi
+00005ad0: 6e67 7320 746f 2069 6e63 6c75 6465 2069  ngs to include i
+00005ae0: 6e20 7468 6520 7365 6c65 6374 6564 2064  n the selected d
+00005af0: 6973 706c 6179 2e0a 2020 2020 2020 2020  isplay..        
+00005b00: 696e 636c 7564 6509 0909 3d20 636f 6e66  include...= conf
+00005b10: 6967 5b64 6973 706c 6179 5d0a 2020 2020  ig[display].    
+00005b20: 2020 2020 6966 2068 6173 6174 7472 2820      if hasattr( 
+00005b30: 696e 636c 7564 652c 2027 5f5f 6361 6c6c  include, '__call
+00005b40: 5f5f 2720 293a 0a20 2020 2020 2020 2020  __' ):.         
+00005b50: 2020 2069 6e63 6c75 6465 0909 3d20 6c69     include..= li
+00005b60: 7374 2820 696e 636c 7564 6528 2920 290a  st( include() ).
+00005b70: 0a20 2020 2020 2020 2023 2043 6f6d 7075  .        # Compu
+00005b80: 7465 2074 696d 6520 6164 7661 6e63 6520  te time advance 
+00005b90: 7369 6e63 6520 6c61 7374 2074 6865 726d  since last therm
+00005ba0: 6f64 796e 616d 6963 2075 7064 6174 650a  odynamic update.
+00005bb0: 2020 2020 2020 2020 7265 616c 0909 093d          real...=
+00005bc0: 2074 696d 6572 2829 0a20 2020 2020 2020   timer().       
+00005bd0: 2064 656c 7461 0909 093d 2072 6561 6c20   delta...= real 
+00005be0: 2d20 6c61 7374 0a0a 2020 2020 2020 2020  - last..        
+00005bf0: 2320 4465 7465 6374 2077 696e 646f 7720  # Detect window 
+00005c00: 7369 7a65 2063 6861 6e67 6573 2c20 616e  size changes, an
+00005c10: 6420 6164 6a75 7374 2064 6574 6169 6c20  d adjust detail 
+00005c20: 7061 6e65 6c20 6163 636f 7264 696e 676c  panel accordingl
+00005c30: 7920 2863 7265 6174 696e 6720 6966 206e  y (creating if n
+00005c40: 6563 6573 7361 7279 290a 2020 2020 2020  ecessary).      
+00005c50: 2020 6966 2028 726f 7773 2c20 636f 6c73    if (rows, cols
+00005c60: 2920 213d 2077 696e 2e67 6574 6d61 7879  ) != win.getmaxy
+00005c70: 7828 293a 0a20 2020 2020 2020 2020 2020  x():.           
+00005c80: 2072 6f77 732c 2063 6f6c 7309 093d 2077   rows, cols..= w
+00005c90: 696e 2e67 6574 6d61 7879 7828 290a 2020  in.getmaxyx().  
+00005ca0: 2020 2020 2020 2020 2020 7769 6e73 656c            winsel
+00005cb0: 0909 3d20 6375 7273 6573 2e6e 6577 7769  ..= curses.newwi
+00005cc0: 6e28 202a 2070 616e 7369 7a28 2072 6f77  n( * pansiz( row
+00005cd0: 732c 2063 6f6c 7320 2920 2b20 7061 6e6c  s, cols ) + panl
+00005ce0: 6f63 2820 302c 2072 6f77 732c 2063 6f6c  oc( 0, rows, col
+00005cf0: 7320 2929 0a20 2020 2020 2020 2020 2020  s )).           
+00005d00: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+00005d10: 2020 2020 2020 7061 6e73 656c 2e72 6570        pansel.rep
+00005d20: 6c61 6365 2820 7769 6e73 656c 2029 0a20  lace( winsel ). 
+00005d30: 2020 2020 2020 2020 2020 2065 7863 6570             excep
+00005d40: 7420 4578 6365 7074 696f 6e3a 0a20 2020  t Exception:.   
+00005d50: 2020 2020 2020 2020 2020 2020 2070 616e               pan
+00005d60: 7365 6c09 093d 2063 7572 7365 732e 7061  sel..= curses.pa
+00005d70: 6e65 6c2e 6e65 775f 7061 6e65 6c28 2077  nel.new_panel( w
+00005d80: 696e 7365 6c20 290a 0a20 2020 2020 2020  insel )..       
+00005d90: 2023 2050 726f 6365 7373 2069 6e70 7574   # Process input
+00005da0: 2c20 6164 6a75 7374 696e 6720 7061 7261  , adjusting para
+00005db0: 6d65 7465 7273 0a20 2020 2020 2020 2069  meters.        i
+00005dc0: 6620 3020 3c20 696e 7075 7420 3c3d 2032  f 0 < input <= 2
+00005dd0: 3535 2061 6e64 2063 6872 2820 696e 7075  55 and chr( inpu
+00005de0: 7420 2920 3d3d 2027 7127 3a0a 2020 2020  t ) == 'q':.    
+00005df0: 2020 2020 2020 2020 636f 6e66 6967 5b27          config['
+00005e00: 636f 6e74 726f 6c27 5d5b 2764 6f6e 6527  control']['done'
+00005e10: 5d20 3d20 5472 7565 0a20 2020 2020 2020  ] = True.       
+00005e20: 2020 2020 2072 6574 7572 6e0a 0a20 2020       return..   
+00005e30: 2020 2020 2069 6620 3020 3c20 696e 7075       if 0 < inpu
+00005e40: 7420 3c3d 2032 3535 2061 6e64 2063 6872  t <= 255 and chr
+00005e50: 2820 696e 7075 7420 2920 3d3d 2027 5c66  ( input ) == '\f
+00005e60: 273a 0909 0923 2046 462c 205e 4c0a 2020  ':...# FF, ^L.  
+00005e70: 2020 2020 2020 2020 2020 2320 5e4c 202d            # ^L -
+00005e80: 2d20 636c 6561 7220 7363 7265 656e 0a20  - clear screen. 
+00005e90: 2020 2020 2020 2020 2020 2077 696e 7365             winse
+00005ea0: 6c2e 636c 6561 7228 290a 0a20 2020 2020  l.clear()..     
+00005eb0: 2020 2023 2053 656c 6563 7420 6e65 7874     # Select next
+00005ec0: 2073 7061 6365 2c20 6164 6a75 7374 2074   space, adjust t
+00005ed0: 6172 6765 7420 7465 6d70 0a20 2020 2020  arget temp.     
+00005ee0: 2020 2069 6620 696e 7075 7420 3d3d 2063     if input == c
+00005ef0: 7572 7365 732e 6173 6369 692e 5350 3a09  urses.ascii.SP:.
+00005f00: 0909 0909 2320 2720 270a 2020 2020 2020  ....# ' '.      
+00005f10: 2020 2020 2020 6966 2070 616e 7365 6c2e        if pansel.
+00005f20: 6869 6464 656e 2829 3a0a 2020 2020 2020  hidden():.      
+00005f30: 2020 2020 2020 2020 2020 7061 6e73 656c            pansel
+00005f40: 2e73 686f 7728 290a 2020 2020 2020 2020  .show().        
+00005f50: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00005f60: 2020 2020 2020 2020 2020 7061 6e73 656c            pansel
+00005f70: 2e68 6964 6528 290a 0a20 2020 2020 2020  .hide()..       
+00005f80: 2069 6620 696e 7075 7420 696e 2028 2063   if input in ( c
+00005f90: 7572 7365 732e 6173 6369 692e 5354 582c  urses.ascii.STX,
+00005fa0: 2063 7572 7365 732e 4b45 595f 4c45 4654   curses.KEY_LEFT
+00005fb0: 2c20 3236 3020 293a 0909 2320 5e62 2c20  , 260 ):..# ^b, 
+00005fc0: 3c2d 2d0a 2020 2020 2020 2020 2020 2020  <--.            
+00005fd0: 7365 6c65 6374 6564 0909 3d20 2820 7365  selected..= ( se
+00005fe0: 6c65 6374 6564 202d 2031 2029 2025 206c  lected - 1 ) % l
+00005ff0: 656e 2820 696e 636c 7564 6520 290a 2020  en( include ).  
+00006000: 2020 2020 2020 6966 2069 6e70 7574 2069        if input i
+00006010: 6e20 2820 6375 7273 6573 2e61 7363 6969  n ( curses.ascii
+00006020: 2e41 434b 2c20 6375 7273 6573 2e4b 4559  .ACK, curses.KEY
+00006030: 5f52 4947 4854 2c20 3236 3120 293a 2020  _RIGHT, 261 ):  
+00006040: 2020 2020 2020 2320 5e66 2c20 2d2d 3e0a        # ^f, -->.
+00006050: 2020 2020 2020 2020 2020 2020 7365 6c65              sele
+00006060: 6374 6564 0909 3d20 2820 7365 6c65 6374  cted..= ( select
+00006070: 6564 202b 2031 2029 2025 206c 656e 2820  ed + 1 ) % len( 
+00006080: 696e 636c 7564 6520 290a 2020 2020 2020  include ).      
+00006090: 2020 6966 2069 6e70 7574 2069 6e20 2820    if input in ( 
+000060a0: 6375 7273 6573 2e61 7363 6969 2e44 4c45  curses.ascii.DLE
+000060b0: 2c20 6375 7273 6573 2e4b 4559 5f55 502c  , curses.KEY_UP,
+000060c0: 2032 3539 2029 3a09 0923 205e 2c20 5e70   259 ):..# ^, ^p
+000060d0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+000060e0: 696e 636c 7564 655b 7365 6c65 6374 6564  include[selected
+000060f0: 5d20 3d3d 2027 776f 726c 6427 3a09 0909  ] == 'world':...
+00006100: 0923 207c 0a20 2020 2020 2020 2020 2020  .# |.           
+00006110: 2020 2020 2023 2064 6f20 736f 6d65 7468       # do someth
+00006120: 696e 6720 746f 2077 6f72 6c64 2e2e 2e0a  ing to world....
+00006130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006140: 7061 7373 0a20 2020 2020 2020 2020 2020  pass.           
+00006150: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00006160: 2020 2020 2020 2063 7572 7365 732e 6265         curses.be
+00006170: 6570 2829 0a20 2020 2020 2020 2069 6620  ep().        if 
+00006180: 696e 7075 7420 696e 2028 2063 7572 7365  input in ( curse
+00006190: 732e 6173 6369 692e 534f 2c20 6375 7273  s.ascii.SO, curs
+000061a0: 6573 2e4b 4559 5f44 4f57 4e2c 2032 3538  es.KEY_DOWN, 258
+000061b0: 2029 3a09 0923 207c 0a20 2020 2020 2020   ):..# |.       
+000061c0: 2020 2020 2069 6620 696e 636c 7564 655b       if include[
+000061d0: 7365 6c65 6374 6564 5d20 3d3d 2027 776f  selected] == 'wo
+000061e0: 726c 6427 3a09 0909 0923 2076 2c20 5e6e  rld':....# v, ^n
+000061f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006200: 2070 6173 730a 2020 2020 2020 2020 2020   pass.          
+00006210: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00006220: 2020 2020 2020 2020 6375 7273 6573 2e62          curses.b
+00006230: 6565 7028 290a 0a20 2020 2020 2020 2069  eep()..        i
+00006240: 6620 3020 3c20 696e 7075 7420 3c3d 2032  f 0 < input <= 2
+00006250: 3535 2061 6e64 2063 6872 2820 696e 7075  55 and chr( inpu
+00006260: 7420 2920 696e 2028 2027 4327 2c20 2763  t ) in ( 'C', 'c
+00006270: 272c 2027 4d27 2c20 276d 2720 293a 0a20  ', 'M', 'm' ):. 
+00006280: 2020 2020 2020 2020 2020 2023 2043 6861             # Cha
+00006290: 7261 6374 6572 206b 6579 7072 6573 7365  racter keypresse
+000062a0: 730a 2020 2020 2020 2020 2020 2020 7061  s.            pa
+000062b0: 7373 0a0a 2020 2020 2020 2020 2320 5768  ss..        # Wh
+000062c0: 656e 2061 206b 6579 7072 6573 7320 6973  en a keypress is
+000062d0: 2064 6574 6563 7465 642c 2061 6c77 6179   detected, alway
+000062e0: 7320 6c6f 6f70 2062 6163 6b20 616e 6420  s loop back and 
+000062f0: 6765 7420 616e 6f74 6865 7220 6b65 792c  get another key,
+00006300: 2074 6f20 6162 736f 7262 206d 756c 7469   to absorb multi
+00006310: 706c 650a 2020 2020 2020 2020 2320 6b65  ple.        # ke
+00006320: 7970 7265 7373 6573 2028 6567 2e20 6475  ypresses (eg. du
+00006330: 6520 746f 206b 6579 2072 6570 6561 7429  e to key repeat)
+00006340: 2c20 6275 7420 6f6e 6c79 2064 6f20 6974  , but only do it
+00006350: 2069 6620 6c65 7373 2074 6865 6e20 312f   if less then 1/
+00006360: 3320 7365 636f 6e64 2068 6173 2070 6173  3 second has pas
+00006370: 7365 642e 0a20 2020 2020 2020 2069 6620  sed..        if 
+00006380: 3020 3c20 696e 7075 7420 616e 6420 6465  0 < input and de
+00006390: 6c74 6120 3c20 2e33 3a0a 2020 2020 2020  lta < .3:.      
+000063a0: 2020 2020 2020 636f 6e74 696e 7565 0a0a        continue..
+000063b0: 2020 2020 2020 2020 2320 5765 276c 6c20          # We'll 
+000063c0: 6265 2063 6f6d 7075 7469 6e67 2061 206e  be computing a n
+000063d0: 6577 206d 6f64 656c 3b20 6164 7661 6e63  ew model; advanc
+000063e0: 6520 2861 6e64 2072 656d 656d 6265 7229  e (and remember)
+000063f0: 2074 696d 650a 2020 2020 2020 2020 6c61   time.        la
+00006400: 7374 0909 093d 2072 6561 6c0a 2020 2020  st...= real.    
+00006410: 2020 2020 6e6f 7720 2020 2020 2020 2020      now         
+00006420: 2020 2020 2020 2020 2020 2020 3d20 7265              = re
+00006430: 616c 0a0a 2020 2020 2020 2020 2320 4e65  al..        # Ne
+00006440: 7874 2066 7261 6d65 206f 6620 616e 696d  xt frame of anim
+00006450: 6174 696f 6e0a 2020 2020 2020 2020 7769  ation.        wi
+00006460: 6e2e 6572 6173 6528 290a 0a20 2020 2020  n.erase()..     
+00006470: 2020 2074 6f70 6d61 7267 696e 2020 2020     topmargin    
+00006480: 2020 2020 2020 2020 2020 203d 2032 0a20             = 2. 
+00006490: 2020 2020 2020 2023 626f 746d 6172 6769         #botmargi
+000064a0: 6e09 093d 2039 0a20 2020 2020 2020 2023  n..= 9.        #
+000064b0: 626f 7472 6f77 0909 093d 2072 6f77 7320  botrow...= rows 
+000064c0: 2d20 626f 746d 6172 6769 6e0a 0a20 2020  - botmargin..   
+000064d0: 2020 2020 2023 2043 6f6d 7075 7465 2073       # Compute s
+000064e0: 6372 6565 6e20 7369 7a65 2061 6e64 2064  creen size and d
+000064f0: 6973 706c 6179 2068 6561 6465 7273 2e20  isplay headers. 
+00006500: 2057 6520 7761 6e74 2063 656c 6c73 2061   We want cells a
+00006510: 2062 6974 2068 6967 6865 7220 7468 616e   bit higher than
+00006520: 2077 6964 652c 2061 6e64 2061 740a 2020   wide, and at.  
+00006530: 2020 2020 2020 2320 6c65 6173 7420 3230        # least 20
+00006540: 2063 6861 7261 6374 6572 7320 7769 6465   characters wide
+00006550: 2e20 204b 6565 7020 7069 6c69 6e67 2027  .  Keep piling '
+00006560: 7469 6c20 7765 2061 7265 2065 6974 6865  til we are eithe
+00006570: 7220 6f76 6572 2032 3020 6368 6172 6163  r over 20 charac
+00006580: 7465 7273 2077 6964 652c 206f 7220 6c65  ters wide, or le
+00006590: 7373 0a20 2020 2020 2020 2023 2074 6861  ss.        # tha
+000065a0: 6e20 352f 3474 6873 2061 7320 6869 6768  n 5/4ths as high
+000065b0: 2061 7320 7769 6465 2e20 2049 6620 7765   as wide.  If we
+000065c0: 2063 616e 2774 2066 696e 6420 6120 7761   can't find a wa
+000065d0: 7920 746f 2067 6574 2063 656c 6c73 203e  y to get cells >
+000065e0: 3d20 3130 2072 6f77 7320 6869 6768 2c20  = 10 rows high, 
+000065f0: 6661 696c 0a20 2020 2020 2020 2023 2061  fail.        # a
+00006600: 6e64 206c 6f6f 7020 2774 696c 2074 6865  nd loop 'til the
+00006610: 7920 6669 7820 7468 6520 6469 7370 6c61  y fix the displa
+00006620: 7920 7369 7a65 2e0a 2020 2020 2020 2020  y size..        
+00006630: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+00006640: 2061 7265 6173 0909 3d20 6c65 6e28 2069   areas..= len( i
+00006650: 6e63 6c75 6465 2029 0a20 2020 2020 2020  nclude ).       
+00006660: 2020 2020 2061 6372 6f73 7309 093d 2031       across..= 1
+00006670: 0a20 2020 2020 2020 2020 2020 2072 616e  .            ran
+00006680: 6b09 093d 2031 0a0a 2020 2020 2020 2020  k..= 1..        
+00006690: 2020 2020 6465 6620 6365 6c6c 7978 2829      def cellyx()
+000066a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000066b0: 2020 7909 093d 2028 2072 6f77 7320 2d20    y..= ( rows - 
+000066c0: 746f 706d 6172 6769 6e20 2920 2f2f 2072  topmargin ) // r
+000066d0: 616e 6b0a 2020 2020 2020 2020 2020 2020  ank.            
+000066e0: 2020 2020 7809 093d 2063 6f6c 7320 2f2f      x..= cols //
+000066f0: 2061 6372 6f73 730a 2020 2020 2020 2020   across.        
+00006700: 2020 2020 2020 2020 7265 7475 726e 2079          return y
+00006710: 2c78 0a0a 2020 2020 2020 2020 2020 2020  ,x..            
+00006720: 6865 6967 6874 2c77 6964 7468 093d 2063  height,width.= c
+00006730: 656c 6c79 7828 290a 2020 2020 2020 2020  ellyx().        
+00006740: 2020 2020 7768 696c 6520 7769 6474 6820      while width 
+00006750: 3e20 3630 3a0a 2020 2020 2020 2020 2020  > 60:.          
+00006760: 2020 2020 2020 6163 726f 7373 0920 2020        across.   
+00006770: 2020 2020 2b3d 2031 0a20 2020 2020 2020      += 1.       
+00006780: 2020 2020 2020 2020 2068 6569 6768 742c           height,
+00006790: 7769 6474 6809 3d20 6365 6c6c 7978 2829  width.= cellyx()
+000067a0: 0a20 2020 2020 2020 2020 2020 2077 6869  .            whi
+000067b0: 6c65 2068 6569 6768 7420 3e20 3230 3a0a  le height > 20:.
+000067c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000067d0: 7261 6e6b 0920 2020 2020 2020 2b3d 2031  rank.       += 1
+000067e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000067f0: 2068 6569 6768 742c 7769 6474 6809 3d20   height,width.= 
+00006800: 6365 6c6c 7978 2829 0a20 2020 2020 2020  cellyx().       
+00006810: 2020 2020 2061 7373 6572 7420 6865 6967       assert heig
+00006820: 6874 203e 3d20 3130 2061 6e64 2077 6964  ht >= 10 and wid
+00006830: 7468 203e 3d20 3330 0a20 2020 2020 2020  th >= 30.       
+00006840: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
+00006850: 6e3a 0a20 2020 2020 2020 2020 2020 206d  n:.            m
+00006860: 6573 7361 6765 2820 7769 6e2c 2022 496e  essage( win, "In
+00006870: 7375 6666 6963 6965 6e74 2073 6372 6565  sufficient scree
+00006880: 6e20 7369 7a65 2028 2564 2061 7265 6173  n size (%d areas
+00006890: 2c20 2564 2072 616e 6b73 206f 6620 2564  , %d ranks of %d
+000068a0: 2020 2564 7825 6420 6365 6c6c 7329 3b20    %dx%d cells); 
+000068b0: 696e 6372 6561 7365 2068 6569 6768 742f  increase height/
+000068c0: 7769 6474 682c 206f 7220 7265 6475 6365  width, or reduce
+000068d0: 2066 6f6e 7420 7369 7a65 2220 2520 280a   font size" % (.
+000068e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000068f0: 6172 6561 732c 2072 616e 6b2c 2061 6372  areas, rank, acr
+00006900: 6f73 732c 2077 6964 7468 2c20 6865 6967  oss, width, heig
+00006910: 6874 2029 2c20 636f 6c20 3d20 302c 2072  ht ), col = 0, r
+00006920: 6f77 203d 2030 2029 0a20 2020 2020 2020  ow = 0 ).       
+00006930: 2020 2020 2077 696e 2e72 6566 7265 7368       win.refresh
+00006940: 2829 0a20 2020 2020 2020 2020 2020 2074  ().            t
+00006950: 696d 652e 736c 6565 7028 2032 2029 0a20  ime.sleep( 2 ). 
+00006960: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
+00006970: 6e75 650a 0a20 2020 2020 2020 2023 204d  nue..        # M
+00006980: 616b 6520 682d 2061 6e64 2076 2d62 6172  ake h- and v-bar
+00006990: 732c 2065 7665 7279 7768 6572 6520 6578  s, everywhere ex
+000069a0: 6365 7074 2074 6f70 206d 6172 6769 6e0a  cept top margin.
+000069b0: 2020 2020 2020 2020 666f 7220 7220 696e          for r in
+000069c0: 2072 616e 6765 2820 746f 706d 6172 6769   range( topmargi
+000069d0: 6e2c 2072 6f77 7320 293a 0a20 2020 2020  n, rows ):.     
+000069e0: 2020 2020 2020 2069 6620 2820 726f 7773         if ( rows
+000069f0: 202d 2072 2029 2025 2068 6569 6768 7420   - r ) % height 
+00006a00: 3d3d 2030 3a0a 2020 2020 2020 2020 2020  == 0:.          
+00006a10: 2020 2020 2020 7769 6e2e 686c 696e 6528        win.hline(
+00006a20: 2072 2c20 302c 2063 7572 7365 732e 4143   r, 0, curses.AC
+00006a30: 535f 484c 494e 452c 2063 6f6c 7320 290a  S_HLINE, cols ).
+00006a40: 2020 2020 2020 2020 666f 7220 6320 696e          for c in
+00006a50: 2072 616e 6765 2820 7769 6474 682c 2063   range( width, c
+00006a60: 6f6c 732c 2077 6964 7468 293a 0a20 2020  ols, width):.   
+00006a70: 2020 2020 2020 2020 2077 696e 2e76 6c69           win.vli
+00006a80: 6e65 2820 746f 706d 6172 6769 6e2c 2063  ne( topmargin, c
+00006a90: 2c20 6375 7273 6573 2e41 4353 5f56 4c49  , curses.ACS_VLI
+00006aa0: 4e45 2c20 726f 7773 202d 2074 6f70 6d61  NE, rows - topma
+00006ab0: 7267 696e 2029 0a0a 2020 2020 2020 2020  rgin )..        
+00006ac0: 2320 5570 6461 7465 0a20 2020 2020 2020  # Update.       
+00006ad0: 2077 696e 7365 6c2e 6572 6173 6528 290a   winsel.erase().
+00006ae0: 2020 2020 2020 2020 7773 726f 7773 2c20          wsrows, 
+00006af0: 7773 636f 6c73 0909 3d20 7769 6e73 656c  wscols..= winsel
+00006b00: 2e67 6574 6d61 7879 7828 290a 0a20 2020  .getmaxyx()..   
+00006b10: 2020 2020 2072 0909 093d 2032 0a20 2020       r...= 2.   
+00006b20: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+00006b30: 2020 2020 2020 7769 6e73 656c 2e68 6c69        winsel.hli
+00006b40: 6e65 2820 722c 2031 2c20 6375 7273 6573  ne( r, 1, curses
+00006b50: 2e41 4353 5f48 4c49 4e45 2c20 7773 636f  .ACS_HLINE, wsco
+00006b60: 6c73 202d 2032 2029 0a20 2020 2020 2020  ls - 2 ).       
+00006b70: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
+00006b80: 6e3a 0a20 2020 2020 2020 2020 2020 2070  n:.            p
+00006b90: 6173 730a 2020 2020 2020 2020 7220 2020  ass.        r   
+00006ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006bb0: 2020 202b 3d20 310a 0a20 2020 2020 2020     += 1..       
+00006bc0: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+00006bd0: 2020 7769 6e73 656c 2e68 6c69 6e65 2820    winsel.hline( 
+00006be0: 722c 2031 2c20 6375 7273 6573 2e41 4353  r, 1, curses.ACS
+00006bf0: 5f48 4c49 4e45 2c20 7773 636f 6c73 202d  _HLINE, wscols -
+00006c00: 2032 2029 0a20 2020 2020 2020 2065 7863   2 ).        exc
+00006c10: 6570 7420 4578 6365 7074 696f 6e3a 0a20  ept Exception:. 
+00006c20: 2020 2020 2020 2020 2020 2070 6173 730a             pass.
+00006c30: 2020 2020 2020 2020 7220 2020 2020 2020          r       
+00006c40: 2020 2020 2020 2020 2020 2020 2020 202b                 +
+00006c50: 3d20 310a 0a20 2020 2020 2020 2077 696e  = 1..        win
+00006c60: 7365 6c2e 626f 7264 6572 2820 3020 290a  sel.border( 0 ).
+00006c70: 0a20 2020 2023 2046 696e 616c 2072 6566  .    # Final ref
+00006c80: 7265 7368 2028 696e 2063 6173 6520 6f66  resh (in case of
+00006c90: 2065 7272 6f72 206d 6573 7361 6765 290a   error message).
+00006ca0: 2020 2020 7769 6e2e 7265 6672 6573 6828      win.refresh(
+00006cb0: 290a 0a0a 6465 6620 6465 6475 6365 5f65  )...def deduce_e
+00006cc0: 6e63 6f64 696e 6728 2061 7661 696c 6162  ncoding( availab
+00006cd0: 6c65 2c20 656e 7669 726f 6e2c 2061 6363  le, environ, acc
+00006ce0: 6570 743d 4e6f 6e65 2029 3a0a 2020 2020  ept=None ):.    
+00006cf0: 2222 2244 6564 7563 6520 6163 6365 7074  """Deduce accept
+00006d00: 6162 6c65 2065 6e63 6f64 696e 6720 6672  able encoding fr
+00006d10: 6f6d 2048 5454 5020 4163 6365 7074 3a20  om HTTP Accept: 
+00006d20: 6865 6164 6572 3a0a 0a20 2020 2020 2020  header:..       
+00006d30: 2041 6363 6570 743a 2074 6578 742f 6874   Accept: text/ht
+00006d40: 6d6c 2c61 7070 6c69 6361 7469 6f6e 2f78  ml,application/x
+00006d50: 6874 6d6c 2b78 6d6c 2c61 7070 6c69 6361  html+xml,applica
+00006d60: 7469 6f6e 2f78 6d6c 3b71 3d30 2e39 2c2a  tion/xml;q=0.9,*
+00006d70: 2f2a 3b71 3d30 2e38 0a0a 2020 2020 4966  /*;q=0.8..    If
+00006d80: 2069 7420 7265 6d61 696e 7320 4e6f 6e65   it remains None
+00006d90: 2028 6f72 2074 6865 2073 7570 706c 6965   (or the supplie
+00006da0: 6420 6f6e 6520 6973 2075 6e72 6563 6f67  d one is unrecog
+00006db0: 6e69 7a65 6429 2c20 7468 650a 2020 2020  nized), the.    
+00006dc0: 6361 6c6c 6572 2073 686f 756c 6420 6661  caller should fa
+00006dd0: 696c 2074 6f20 7072 6f64 7563 6520 7468  il to produce th
+00006de0: 6520 6465 7369 7265 6420 636f 6e74 656e  e desired conten
+00006df0: 742c 2061 6e64 2072 6574 7572 6e20 616e  t, and return an
+00006e00: 0a20 2020 2048 544d 4c20 7374 6174 7573  .    HTML status
+00006e10: 2063 6f64 6520 3430 3620 4e6f 7420 4163   code 406 Not Ac
+00006e20: 6365 7074 6162 6c65 2e0a 0a20 2020 2049  ceptable...    I
+00006e30: 6620 6e6f 2041 6363 6570 743a 2065 6e63  f no Accept: enc
+00006e40: 6f64 696e 6720 6973 2073 7570 706c 6965  oding is supplie
+00006e50: 6420 696e 2074 6865 2065 6e76 6972 6f6e  d in the environ
+00006e60: 2c20 7468 6520 6465 6661 756c 740a 2020  , the default.  
+00006e70: 2020 2866 6972 7374 2920 656e 636f 6469    (first) encodi
+00006e80: 6e67 2069 6e20 6f72 6465 7220 6973 2075  ng in order is u
+00006e90: 7365 642e 0a0a 2020 2020 5765 2064 6f6e  sed...    We don
+00006ea0: 2774 2074 6573 7420 6120 7375 7070 6c69  't test a suppli
+00006eb0: 6564 2027 6163 6365 7074 2720 656e 636f  ed 'accept' enco
+00006ec0: 6469 6e67 2061 6761 696e 7374 2074 6865  ding against the
+00006ed0: 2048 5454 505f 4143 4345 5054 0a20 2020   HTTP_ACCEPT.   
+00006ee0: 2073 6574 7469 6e67 732c 2062 6563 6175   settings, becau
+00006ef0: 7365 2063 6572 7461 696e 2055 524c 7320  se certain URLs 
+00006f00: 6861 7665 2061 2066 6978 6564 2065 6e63  have a fixed enc
+00006f10: 6f64 696e 672e 2020 466f 720a 2020 2020  oding.  For.    
+00006f20: 6578 616d 706c 652c 202f 736f 6d65 2f75  example, /some/u
+00006f30: 726c 2f62 6c61 682e 6a73 6f6e 2061 6c77  rl/blah.json alw
+00006f40: 6179 7320 7761 6e74 7320 746f 2072 6574  ays wants to ret
+00006f50: 7572 6e0a 2020 2020 2261 7070 6c69 6361  urn.    "applica
+00006f60: 7469 6f6e 2f6a 736f 6e22 2c20 7265 6761  tion/json", rega
+00006f70: 7264 6c65 7373 206f 6620 7768 6574 6865  rdless of whethe
+00006f80: 7220 7468 6520 6272 6f77 7365 7227 7320  r the browser's 
+00006f90: 4163 6365 7074 3a0a 2020 2020 6865 6164  Accept:.    head
+00006fa0: 6572 2069 6e64 6963 6174 6573 2069 7420  er indicates it 
+00006fb0: 6973 2061 6363 6570 7461 626c 652e 2020  is acceptable.  
+00006fc0: 5765 202a 646f 2a20 686f 7765 7665 7220  We *do* however 
+00006fd0: 7465 7374 2074 6865 0a20 2020 2073 7570  test the.    sup
+00006fe0: 706c 6965 6420 2761 6363 6570 7427 2065  plied 'accept' e
+00006ff0: 6e63 6f64 696e 6720 6167 6169 6e73 7420  ncoding against 
+00007000: 7468 6520 2761 7661 696c 6162 6c65 2720  the 'available' 
+00007010: 656e 636f 6469 6e67 732c 0a20 2020 2062  encodings,.    b
+00007020: 6563 6175 7365 2074 6865 7365 2061 7265  ecause these are
+00007030: 2074 6865 206f 6e6c 7920 6f6e 6573 206b   the only ones k
+00007040: 6e6f 776e 2074 6f20 7468 6520 6361 6c6c  nown to the call
+00007050: 6572 2e0a 0a20 2020 204f 7468 6572 7769  er...    Otherwi
+00007060: 7365 2c20 7265 7475 726e 2074 6865 2066  se, return the f
+00007070: 6972 7374 2061 6363 6570 7461 626c 6520  irst acceptable 
+00007080: 656e 636f 6469 6e67 2069 6e20 2761 7661  encoding in 'ava
+00007090: 696c 6162 6c65 272e 0a0a 2020 2020 2222  ilable'...    ""
+000070a0: 220a 2020 2020 6966 2061 6363 6570 743a  ".    if accept:
+000070b0: 0a20 2020 2020 2020 2023 2041 2064 6573  .        # A des
+000070c0: 6972 6564 2065 6e63 6f64 696e 673b 206d  ired encoding; m
+000070d0: 616b 6520 7375 7265 2069 7420 6973 2061  ake sure it is a
+000070e0: 7661 696c 6162 6c65 0a20 2020 2020 2020  vailable.       
+000070f0: 2061 6363 6570 7409 093d 2061 6363 6570   accept..= accep
+00007100: 742e 6c6f 7765 7228 290a 2020 2020 2020  t.lower().      
+00007110: 2020 6966 2061 6363 6570 7420 6e6f 7420    if accept not 
+00007120: 696e 2061 7661 696c 6162 6c65 3a0a 2020  in available:.  
+00007130: 2020 2020 2020 2020 2020 6163 6365 7074            accept
+00007140: 093d 204e 6f6e 650a 2020 2020 2020 2020  .= None.        
+00007150: 7265 7475 726e 2061 6363 6570 740a 0a20  return accept.. 
+00007160: 2020 2023 204e 6f20 7072 6564 6566 696e     # No predefin
+00007170: 6564 2061 6363 6570 7420 656e 636f 6469  ed accept encodi
+00007180: 6e67 3b20 6465 6475 6365 2070 7265 6665  ng; deduce prefe
+00007190: 7272 6564 2061 7661 696c 6162 6c65 206f  rred available o
+000071a0: 6e65 2e0a 2020 2020 2320 4163 6365 7074  ne..    # Accept
+000071b0: 3a20 6d61 7920 636f 6e74 6169 6e20 2a2f  : may contain */
+000071c0: 2a2c 202a 2f6a 736f 6e2c 2065 7463 2e20  *, */json, etc. 
+000071d0: 2049 6620 6d75 6c74 6970 6c65 206d 6174   If multiple mat
+000071e0: 6368 6573 2c0a 2020 2020 2320 7365 6c65  ches,.    # sele
+000071f0: 6374 2074 6865 206f 6e65 2077 6974 6820  ct the one with 
+00007200: 7468 6520 6869 6768 6573 7420 4163 6365  the highest Acce
+00007210: 7074 3a20 7175 616c 6974 7920 7661 6c75  pt: quality valu
+00007220: 6520 286f 7572 0a20 2020 2023 2070 7265  e (our.    # pre
+00007230: 7365 6e74 204e 6f6e 6520 7374 6172 7473  sent None starts
+00007240: 2077 6974 6820 6120 7175 616c 6974 7920   with a quality 
+00007250: 6d65 7472 6963 206f 6620 302e 3029 2e20  metric of 0.0). 
+00007260: 2054 6573 740a 2020 2020 2320 6176 6169   Test.    # avai
+00007270: 6c61 626c 653a 205b 2261 7070 6c69 6361  lable: ["applica
+00007280: 7469 6f6e 2f6a 736f 6e22 2c20 2274 6578  tion/json", "tex
+00007290: 742f 6874 6d6c 225d 2c20 7673 2e20 4854  t/html"], vs. HT
+000072a0: 5450 5f41 4343 4550 540a 2020 2020 2320  TP_ACCEPT.    # 
+000072b0: 2274 6578 742f 6874 6d6c 2c61 7070 6c69  "text/html,appli
+000072c0: 6361 7469 6f6e 2f78 6874 6d6c 2b78 6d6c  cation/xhtml+xml
+000072d0: 2c61 7070 6c69 6361 7469 6f6e 2f78 6d6c  ,application/xml
+000072e0: 3b71 3d30 2e39 2c2a 2f2a 3b71 3d30 2e38  ;q=0.9,*/*;q=0.8
+000072f0: 220a 2020 2020 2320 5369 6e63 6520 6561  ".    # Since ea
+00007300: 726c 6965 7220 6d61 7463 6865 7320 6172  rlier matches ar
+00007310: 6520 7468 6520 666f 7220 6d6f 7265 2070  e the for more p
+00007320: 7265 6665 7272 6564 2065 6e63 6f64 696e  referred encodin
+00007330: 6773 2c0a 2020 2020 2320 6c61 7465 7220  gs,.    # later 
+00007340: 6d61 7463 6865 7320 6d75 7374 202a 6578  matches must *ex
+00007350: 6365 6564 2a20 7468 6520 7175 616c 6974  ceed* the qualit
+00007360: 7920 6d65 7472 6963 206f 6620 7468 6520  y metric of the 
+00007370: 6561 726c 6965 722e 0a20 2020 2048 5454  earlier..    HTT
+00007380: 505f 4143 4345 5054 0909 3d20 656e 7669  P_ACCEPT..= envi
+00007390: 726f 6e2e 6765 7428 2022 4854 5450 5f41  ron.get( "HTTP_A
+000073a0: 4343 4550 5422 2c20 222a 2f2a 2220 292e  CCEPT", "*/*" ).
+000073b0: 6c6f 7765 7228 2920 6966 2065 6e76 6972  lower() if envir
+000073c0: 6f6e 2065 6c73 6520 222a 2f2a 220a 2020  on else "*/*".  
+000073d0: 2020 7175 616c 6974 7909 093d 2030 2e30    quality..= 0.0
+000073e0: 0a20 2020 2066 6f72 2073 7461 6e7a 6120  .    for stanza 
+000073f0: 696e 2048 5454 505f 4143 4345 5054 2e73  in HTTP_ACCEPT.s
+00007400: 706c 6974 2820 272c 2720 293a 0a20 2020  plit( ',' ):.   
+00007410: 2020 2020 2023 2061 7070 6c69 6361 7469       # applicati
+00007420: 6f6e 2f78 6d6c 3b71 3d30 2e39 0a20 2020  on/xml;q=0.9.   
+00007430: 2020 2020 2071 0909 3d20 312e 300a 2020       q..= 1.0.  
+00007440: 2020 2020 2020 666f 7220 656e 636f 6469        for encodi
+00007450: 6e67 2069 6e20 7265 7665 7273 6564 2820  ng in reversed( 
+00007460: 7374 616e 7a61 2e73 706c 6974 2820 273b  stanza.split( ';
+00007470: 2720 2929 3a0a 2020 2020 2020 2020 2020  ' )):.          
+00007480: 2020 6966 2065 6e63 6f64 696e 672e 7374    if encoding.st
+00007490: 6172 7473 7769 7468 2820 2271 3d22 2029  artswith( "q=" )
+000074a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000074b0: 2020 7109 3d20 666c 6f61 7428 2065 6e63    q.= float( enc
+000074c0: 6f64 696e 675b 323a 5d20 290a 2020 2020  oding[2:] ).    
+000074d0: 2020 2020 666f 7220 6176 6169 6c20 696e      for avail in
+000074e0: 2061 7661 696c 6162 6c65 3a0a 2020 2020   available:.    
+000074f0: 2020 2020 2020 2020 6d61 7463 6809 3d20          match.= 
+00007500: 5472 7565 0a20 2020 2020 2020 2020 2020  True.           
+00007510: 2066 6f72 2061 2c20 7420 696e 207a 6970   for a, t in zip
+00007520: 2820 6176 6169 6c2e 7370 6c69 7428 2027  ( avail.split( '
+00007530: 2f27 2029 2c20 656e 636f 6469 6e67 2e73  /' ), encoding.s
+00007540: 706c 6974 2820 272f 2720 2929 3a0a 2020  plit( '/' )):.  
+00007550: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00007560: 2061 2021 3d20 7420 616e 6420 7420 213d   a != t and t !=
+00007570: 2027 2a27 3a0a 2020 2020 2020 2020 2020   '*':.          
+00007580: 2020 2020 2020 2020 2020 6d61 7463 6820            match 
+00007590: 3d20 4661 6c73 650a 2020 2020 2020 2020  = False.        
+000075a0: 2020 2020 6966 206d 6174 6368 3a0a 2020      if match:.  
+000075b0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+000075c0: 2071 203e 2071 7561 6c69 7479 3a0a 2020   q > quality:.  
+000075d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000075e0: 2020 7175 616c 6974 7909 3d20 710a 2020    quality.= q.  
+000075f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007600: 2020 6163 6365 7074 093d 2061 7661 696c    accept.= avail
+00007610: 0a20 2020 2072 6574 7572 6e20 6163 6365  .    return acce
+00007620: 7074 0a0a 0a64 6566 2068 7474 705f 6578  pt...def http_ex
+00007630: 6365 7074 696f 6e28 2066 7261 6d65 776f  ception( framewo
+00007640: 726b 2c20 7374 6174 7573 2c20 6d65 7373  rk, status, mess
+00007650: 6167 6520 293a 0a20 2020 2022 2222 5265  age ):.    """Re
+00007660: 7475 726e 2061 6e20 6578 6365 7074 696f  turn an exceptio
+00007670: 6e20 6170 7072 6f70 7269 6174 6520 666f  n appropriate fo
+00007680: 7220 7468 6520 6769 7665 6e20 7765 6220  r the given web 
+00007690: 6672 616d 6577 6f72 6b2c 0a20 2020 2065  framework,.    e
+000076a0: 6e63 6f64 696e 6720 7468 6520 4854 5450  ncoding the HTTP
+000076b0: 2073 7461 7475 7320 636f 6465 2061 6e64   status code and
+000076c0: 206d 6573 7361 6765 2070 726f 7669 6465   message provide
+000076d0: 642e 0a20 2020 2022 2222 0a20 2020 2069  d..    """.    i
+000076e0: 6620 6672 616d 6577 6f72 6b20 616e 6420  f framework and 
+000076f0: 6672 616d 6577 6f72 6b2e 5f5f 6e61 6d65  framework.__name
+00007700: 5f5f 203d 3d20 2277 6562 223a 0a20 2020  __ == "web":.   
+00007710: 2020 2020 2069 6620 7374 6174 7573 203d       if status =
+00007720: 3d20 3430 343a 0a20 2020 2020 2020 2020  = 404:.         
+00007730: 2020 2072 6574 7572 6e20 6672 616d 6577     return framew
+00007740: 6f72 6b2e 4e6f 7446 6f75 6e64 2820 6d65  ork.NotFound( me
+00007750: 7373 6167 6520 290a 0a20 2020 2020 2020  ssage )..       
+00007760: 2069 6620 7374 6174 7573 203d 3d20 3430   if status == 40
+00007770: 363a 0a20 2020 2020 2020 2020 2020 2072  6:.            r
+00007780: 6574 7572 6e20 6672 616d 6577 6f72 6b2e  eturn framework.
+00007790: 4e6f 7441 6363 6570 7461 626c 6528 2909  NotAcceptable().
+000077a0: 0909 2320 5769 6c6c 206e 6f74 2061 6363  ..# Will not acc
+000077b0: 6570 7420 6120 6d65 7373 6167 650a 0a20  ept a message.. 
+000077c0: 2020 2072 6574 7572 6e20 4578 6365 7074     return Except
+000077d0: 696f 6e28 2022 2564 2025 7322 2025 2028  ion( "%d %s" % (
+000077e0: 2073 7461 7475 732c 206d 6573 7361 6765   status, message
+000077f0: 2029 290a 0a0a 6465 6620 6c69 6365 6e73   ))...def licens
+00007800: 6573 5f72 6571 7565 7374 2820 7265 6e64  es_request( rend
+00007810: 6572 2c20 7061 7468 2c20 656e 7669 726f  er, path, enviro
+00007820: 6e2c 2061 6363 6570 742c 2066 7261 6d65  n, accept, frame
+00007830: 776f 726b 2c0a 2020 2020 2020 2020 2020  work,.          
+00007840: 2020 2020 2020 2020 2020 2020 2020 2071                 q
+00007850: 7565 7269 6573 3d4e 6f6e 652c 2070 6f73  ueries=None, pos
+00007860: 7465 643d 4e6f 6e65 2c0a 2020 2020 2020  ted=None,.      
+00007870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007880: 2020 2073 6573 7369 6f6e 3d4e 6f6e 652c     session=None,
+00007890: 206c 6f67 6765 643d 4e6f 6e65 2c09 0923   logged=None,..#
+000078a0: 2054 6865 2075 7365 7220 7365 7373 696f   The user sessio
+000078b0: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
+000078c0: 2020 2020 2020 2020 2020 2070 726f 7879             proxy
+000078d0: 3d4e 6f6e 6520 293a 0a0a 2020 2020 2222  =None ):..    ""
+000078e0: 220a 2020 2020 2020 2020 6170 692f 6c69  ".        api/li
+000078f0: 6365 6e73 6573 2f3c 6e61 6d65 3e2f 0a0a  censes/<name>/..
+00007900: 2020 2020 2222 220a 2020 2020 7661 7269      """.    vari
+00007910: 6162 6c65 7309 0909 3d20 7175 6572 6965  ables...= querie
+00007920: 7320 6f72 2070 6f73 7465 6420 6f72 207b  s or posted or {
+00007930: 7d0a 2020 2020 636f 6e74 656e 7409 0909  }.    content...
+00007940: 3d20 6465 6475 6365 5f65 6e63 6f64 696e  = deduce_encodin
+00007950: 6728 205b 2022 7465 7874 2f68 746d 6c22  g( [ "text/html"
+00007960: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
 00007970: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007990: 2020 2020 2020 2020 2020 2020 2020 2274                "t
-000079a0: 6578 742f 706c 6169 6e22 205d 2c0a 2020  ext/plain" ],.  
-000079b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007990: 2020 2020 2020 2022 6170 706c 6963 6174         "applicat
+000079a0: 696f 6e2f 6a73 6f6e 222c 2022 7465 7874  ion/json", "text
+000079b0: 2f6a 6176 6173 6372 6970 7422 2c0a 2020  /javascript",.  
 000079c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000079d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000079e0: 2065 6e76 6972 6f6e 3d65 6e76 6972 6f6e   environ=environ
-000079f0: 2c20 6163 6365 7074 3d61 6363 6570 7420  , accept=accept 
-00007a00: 290a 2020 2020 7265 7370 6f6e 7365 0909  ).    response..
-00007a10: 093d 2022 220a 0a20 2020 2023 2041 2055  .= ""..    # A U
-00007a20: 524c 2077 2f20 616e 2065 6d70 7479 202e  RL w/ an empty .
-00007a30: 2e2e 3f63 6f6e 6669 726d 2069 7320 6173  ..?confirm is as
-00007a40: 7375 6d65 6420 746f 2062 6520 5472 7565  sumed to be True
-00007a50: 2e0a 2020 2020 636f 6e66 6972 6d09 0909  ..    confirm...
-00007a60: 3d20 6c69 6365 6e73 696e 672e 696e 746f  = licensing.into
-00007a70: 5f62 6f6f 6c65 616e 2820 7661 7269 6162  _boolean( variab
-00007a80: 6c65 732e 6765 7428 2027 636f 6e66 6972  les.get( 'confir
-00007a90: 6d27 2c20 4661 6c73 6520 292c 2074 7275  m', False ), tru
-00007aa0: 7468 793d 2827 272c 2920 290a 2020 2020  thy=('',) ).    
-00007ab0: 6175 7468 6f72 0909 093d 206c 6963 656e  author...= licen
-00007ac0: 7369 6e67 2e69 6e74 6f5f 7374 7228 2076  sing.into_str( v
-00007ad0: 6172 6961 626c 6573 2e67 6574 2820 2761  ariables.get( 'a
-00007ae0: 7574 686f 7227 2029 290a 2020 2020 636c  uthor' )).    cl
-00007af0: 6965 6e74 0909 093d 206c 6963 656e 7369  ient...= licensi
-00007b00: 6e67 2e69 6e74 6f5f 7374 7228 2076 6172  ng.into_str( var
-00007b10: 6961 626c 6573 2e67 6574 2820 2763 6c69  iables.get( 'cli
-00007b20: 656e 7427 2029 290a 2020 2020 7072 6f64  ent' )).    prod
-00007b30: 7563 7409 0909 3d20 6c69 6365 6e73 696e  uct...= licensin
-00007b40: 672e 696e 746f 5f73 7472 2820 7661 7269  g.into_str( vari
-00007b50: 6162 6c65 732e 6765 7428 2027 7072 6f64  ables.get( 'prod
-00007b60: 7563 7427 2029 290a 2020 2020 7374 6f72  uct' )).    stor
-00007b70: 6564 0909 093d 206c 6973 7428 2064 622e  ed...= list( db.
-00007b80: 7365 6c65 6374 2820 276c 6963 656e 7365  select( 'license
-00007b90: 7327 2029 290a 2020 2020 6461 7461 0909  s' )).    data..
-00007ba0: 093d 206c 6963 656e 7365 735f 6461 7461  .= licenses_data
-00007bb0: 2820 7061 7468 2c20 7374 6f72 6564 3d73  ( path, stored=s
-00007bc0: 746f 7265 642c 2063 6f6e 6669 726d 3d63  tored, confirm=c
-00007bd0: 6f6e 6669 726d 2c0a 2020 2020 2020 2020  onfirm,.        
-00007be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c00: 2020 2020 2020 2020 2061 7574 686f 723d           author=
-00007c10: 6175 7468 6f72 2c20 636c 6965 6e74 3d63  author, client=c
-00007c20: 6c69 656e 742c 2070 726f 6475 6374 3d70  lient, product=p
-00007c30: 726f 6475 6374 2029 0a0a 2020 2020 6966  roduct )..    if
-00007c40: 2063 6f6e 7465 6e74 2061 6e64 2063 6f6e   content and con
-00007c50: 7465 6e74 2069 6e20 2820 2261 7070 6c69  tent in ( "appli
-00007c60: 6361 7469 6f6e 2f6a 736f 6e22 2c20 2274  cation/json", "t
-00007c70: 6578 742f 6a61 7661 7363 7269 7074 222c  ext/javascript",
-00007c80: 2022 7465 7874 2f70 6c61 696e 2220 293a   "text/plain" ):
-00007c90: 0a20 2020 2020 2020 2063 616c 6c62 6163  .        callbac
-00007ca0: 6b09 093d 2076 6172 6961 626c 6573 2e67  k..= variables.g
-00007cb0: 6574 2820 2763 616c 6c62 6163 6b27 2c20  et( 'callback', 
-00007cc0: 2222 2029 0a20 2020 2020 2020 2069 6620  "" ).        if 
-00007cd0: 6361 6c6c 6261 636b 3a0a 2020 2020 2020  callback:.      
-00007ce0: 2020 2020 2020 7265 7370 6f6e 7365 2020        response  
-00007cf0: 2020 2020 2020 2020 202b 3d20 6361 6c6c           += call
-00007d00: 6261 636b 202b 2022 2820 220a 2020 2020  back + "( ".    
-00007d10: 2020 2020 7265 7370 6f6e 7365 2020 2020      response    
-00007d20: 2020 2020 2020 2020 2020 202b 3d20 6c69             += li
-00007d30: 6365 6e73 696e 672e 696e 746f 5f4a 534f  censing.into_JSO
-00007d40: 4e28 2064 6174 612c 2069 6e64 656e 743d  N( data, indent=
-00007d50: 3420 290a 2020 2020 2020 2020 6966 2063  4 ).        if c
-00007d60: 616c 6c62 6163 6b3a 0a20 2020 2020 2020  allback:.       
-00007d70: 2020 2020 2072 6573 706f 6e73 6520 2020       response   
-00007d80: 2020 2020 2020 2020 2b3d 2022 2029 220a          += " )".
-00007d90: 2020 2020 656c 6966 2063 6f6e 7465 6e74      elif content
-00007da0: 2061 6e64 2063 6f6e 7465 6e74 2069 6e20   and content in 
-00007db0: 2820 2274 6578 742f 6874 6d6c 2220 293a  ( "text/html" ):
-00007dc0: 0a20 2020 2020 2020 2072 6573 706f 6e73  .        respons
-00007dd0: 6509 093d 2072 656e 6465 722e 6b65 796c  e..= render.keyl
-00007de0: 6973 7428 2064 6174 6120 290a 2020 2020  ist( data ).    
-00007df0: 656c 7365 3a0a 2020 2020 2020 2020 7261  else:.        ra
-00007e00: 6973 6520 6874 7470 5f65 7863 6570 7469  ise http_excepti
-00007e10: 6f6e 2820 6672 616d 6577 6f72 6b2c 2034  on( framework, 4
-00007e20: 3036 2c20 2255 6e61 626c 6520 746f 2070  06, "Unable to p
-00007e30: 726f 6475 6365 2025 7320 636f 6e74 656e  roduce %s conten
-00007e40: 7422 2025 2028 0a20 2020 2020 2020 2020  t" % (.         
-00007e50: 2020 2063 6f6e 7465 6e74 206f 7220 6163     content or ac
-00007e60: 6365 7074 206f 7220 2275 6e6b 6e6f 776e  cept or "unknown
-00007e70: 2220 2929 0a20 2020 2072 6574 7572 6e20  " )).    return 
-00007e80: 636f 6e74 656e 742c 2072 6573 706f 6e73  content, respons
-00007e90: 650a 0a0a 6465 6620 6372 6564 656e 7469  e...def credenti
-00007ea0: 616c 735f 7265 7175 6573 7428 2072 656e  als_request( ren
-00007eb0: 6465 722c 2070 6174 682c 2065 6e76 6972  der, path, envir
-00007ec0: 6f6e 2c20 6163 6365 7074 2c20 6672 616d  on, accept, fram
-00007ed0: 6577 6f72 6b2c 0a20 2020 2020 2020 2020  ework,.         
-00007ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ef0: 7175 6572 6965 733d 4e6f 6e65 2c20 706f  queries=None, po
-00007f00: 7374 6564 3d4e 6f6e 652c 0a20 2020 2020  sted=None,.     
-00007f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f20: 2020 2020 7365 7373 696f 6e3d 4e6f 6e65      session=None
-00007f30: 2c20 6c6f 6767 6564 3d4e 6f6e 652c 0909  , logged=None,..
-00007f40: 2320 5468 6520 7573 6572 2073 6573 7369  # The user sessi
-00007f50: 6f6e 0a20 2020 2020 2020 2020 2020 2020  on.             
-00007f60: 2020 2020 2020 2020 2020 2020 7072 6f78              prox
-00007f70: 793d 4e6f 6e65 2029 3a0a 0a20 2020 2022  y=None ):..    "
-00007f80: 2222 0a20 2020 2020 2020 2061 7069 2f63  "".        api/c
-00007f90: 7265 6465 6e74 6961 6c73 2f3c 6e61 6d65  redentials/<name
-00007fa0: 3e2f 0a0a 2020 2020 2222 220a 2020 2020  >/..    """.    
-00007fb0: 7661 7269 6162 6c65 7309 0909 3d20 7175  variables...= qu
-00007fc0: 6572 6965 7320 6f72 2070 6f73 7465 6420  eries or posted 
-00007fd0: 6f72 207b 7d0a 2020 2020 636f 6e74 656e  or {}.    conten
-00007fe0: 7409 0909 3d20 6465 6475 6365 5f65 6e63  t...= deduce_enc
-00007ff0: 6f64 696e 6728 205b 2022 7465 7874 2f68  oding( [ "text/h
-00008000: 746d 6c22 2c0a 2020 2020 2020 2020 2020  tml",.          
-00008010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008030: 2020 2020 2020 2020 2020 2022 6170 706c             "appl
-00008040: 6963 6174 696f 6e2f 6a73 6f6e 222c 2022  ication/json", "
-00008050: 7465 7874 2f6a 6176 6173 6372 6970 7422  text/javascript"
-00008060: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000079e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000079f0: 2020 2022 7465 7874 2f70 6c61 696e 2220     "text/plain" 
+00007a00: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+00007a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a30: 2020 2020 2020 656e 7669 726f 6e3d 656e        environ=en
+00007a40: 7669 726f 6e2c 2061 6363 6570 743d 6163  viron, accept=ac
+00007a50: 6365 7074 2029 0a20 2020 2072 6573 706f  cept ).    respo
+00007a60: 6e73 6509 0909 3d20 2222 0a0a 2020 2020  nse...= ""..    
+00007a70: 2320 4120 5552 4c20 772f 2061 6e20 656d  # A URL w/ an em
+00007a80: 7074 7920 2e2e 2e3f 636f 6e66 6972 6d20  pty ...?confirm 
+00007a90: 6973 2061 7373 756d 6564 2074 6f20 6265  is assumed to be
+00007aa0: 2054 7275 652e 0a20 2020 2063 6f6e 6669   True..    confi
+00007ab0: 726d 0909 093d 206c 6963 656e 7369 6e67  rm...= licensing
+00007ac0: 2e69 6e74 6f5f 626f 6f6c 6561 6e28 2076  .into_boolean( v
+00007ad0: 6172 6961 626c 6573 2e67 6574 2820 2763  ariables.get( 'c
+00007ae0: 6f6e 6669 726d 272c 2046 616c 7365 2029  onfirm', False )
+00007af0: 2c20 7472 7574 6879 3d28 2727 2c29 2029  , truthy=('',) )
+00007b00: 0a20 2020 2061 7574 686f 7209 0909 3d20  .    author...= 
+00007b10: 6c69 6365 6e73 696e 672e 696e 746f 5f73  licensing.into_s
+00007b20: 7472 2820 7661 7269 6162 6c65 732e 6765  tr( variables.ge
+00007b30: 7428 2027 6175 7468 6f72 2720 2929 0a20  t( 'author' )). 
+00007b40: 2020 2063 6c69 656e 7409 0909 3d20 6c69     client...= li
+00007b50: 6365 6e73 696e 672e 696e 746f 5f73 7472  censing.into_str
+00007b60: 2820 7661 7269 6162 6c65 732e 6765 7428  ( variables.get(
+00007b70: 2027 636c 6965 6e74 2720 2929 0a20 2020   'client' )).   
+00007b80: 2070 726f 6475 6374 0909 093d 206c 6963   product...= lic
+00007b90: 656e 7369 6e67 2e69 6e74 6f5f 7374 7228  ensing.into_str(
+00007ba0: 2076 6172 6961 626c 6573 2e67 6574 2820   variables.get( 
+00007bb0: 2770 726f 6475 6374 2720 2929 0a20 2020  'product' )).   
+00007bc0: 2073 746f 7265 6409 0909 3d20 6c69 7374   stored...= list
+00007bd0: 2820 6462 2e73 656c 6563 7428 2027 6c69  ( db.select( 'li
+00007be0: 6365 6e73 6573 2720 2929 0a20 2020 2064  censes' )).    d
+00007bf0: 6174 6109 0909 3d20 6c69 6365 6e73 6573  ata...= licenses
+00007c00: 5f64 6174 6128 2070 6174 682c 2073 746f  _data( path, sto
+00007c10: 7265 643d 7374 6f72 6564 2c20 636f 6e66  red=stored, conf
+00007c20: 6972 6d3d 636f 6e66 6972 6d2c 0a20 2020  irm=confirm,.   
+00007c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007c50: 2020 2020 2020 2020 2020 2020 2020 6175                au
+00007c60: 7468 6f72 3d61 7574 686f 722c 2063 6c69  thor=author, cli
+00007c70: 656e 743d 636c 6965 6e74 2c20 7072 6f64  ent=client, prod
+00007c80: 7563 743d 7072 6f64 7563 7420 290a 0a20  uct=product ).. 
+00007c90: 2020 2069 6620 636f 6e74 656e 7420 616e     if content an
+00007ca0: 6420 636f 6e74 656e 7420 696e 2028 2022  d content in ( "
+00007cb0: 6170 706c 6963 6174 696f 6e2f 6a73 6f6e  application/json
+00007cc0: 222c 2022 7465 7874 2f6a 6176 6173 6372  ", "text/javascr
+00007cd0: 6970 7422 2c20 2274 6578 742f 706c 6169  ipt", "text/plai
+00007ce0: 6e22 2029 3a0a 2020 2020 2020 2020 6361  n" ):.        ca
+00007cf0: 6c6c 6261 636b 0909 3d20 7661 7269 6162  llback..= variab
+00007d00: 6c65 732e 6765 7428 2027 6361 6c6c 6261  les.get( 'callba
+00007d10: 636b 272c 2022 2220 290a 2020 2020 2020  ck', "" ).      
+00007d20: 2020 6966 2063 616c 6c62 6163 6b3a 0a20    if callback:. 
+00007d30: 2020 2020 2020 2020 2020 2072 6573 706f             respo
+00007d40: 6e73 6520 2020 2020 2020 2020 2020 2b3d  nse           +=
+00007d50: 2063 616c 6c62 6163 6b20 2b20 2228 2022   callback + "( "
+00007d60: 0a20 2020 2020 2020 2072 6573 706f 6e73  .        respons
+00007d70: 6520 2020 2020 2020 2020 2020 2020 2020  e               
+00007d80: 2b3d 206c 6963 656e 7369 6e67 2e69 6e74  += licensing.int
+00007d90: 6f5f 4a53 4f4e 2820 6461 7461 2c20 696e  o_JSON( data, in
+00007da0: 6465 6e74 3d34 2029 0a20 2020 2020 2020  dent=4 ).       
+00007db0: 2069 6620 6361 6c6c 6261 636b 3a0a 2020   if callback:.  
+00007dc0: 2020 2020 2020 2020 2020 7265 7370 6f6e            respon
+00007dd0: 7365 2020 2020 2020 2020 2020 202b 3d20  se           += 
+00007de0: 2220 2922 0a20 2020 2065 6c69 6620 636f  " )".    elif co
+00007df0: 6e74 656e 7420 616e 6420 636f 6e74 656e  ntent and conten
+00007e00: 7420 696e 2028 2022 7465 7874 2f68 746d  t in ( "text/htm
+00007e10: 6c22 2029 3a0a 2020 2020 2020 2020 7265  l" ):.        re
+00007e20: 7370 6f6e 7365 0909 3d20 7265 6e64 6572  sponse..= render
+00007e30: 2e6b 6579 6c69 7374 2820 6461 7461 2029  .keylist( data )
+00007e40: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
+00007e50: 2020 2072 6169 7365 2068 7474 705f 6578     raise http_ex
+00007e60: 6365 7074 696f 6e28 2066 7261 6d65 776f  ception( framewo
+00007e70: 726b 2c20 3430 362c 2022 556e 6162 6c65  rk, 406, "Unable
+00007e80: 2074 6f20 7072 6f64 7563 6520 2573 2063   to produce %s c
+00007e90: 6f6e 7465 6e74 2220 2520 280a 2020 2020  ontent" % (.    
+00007ea0: 2020 2020 2020 2020 636f 6e74 656e 7420          content 
+00007eb0: 6f72 2061 6363 6570 7420 6f72 2022 756e  or accept or "un
+00007ec0: 6b6e 6f77 6e22 2029 290a 2020 2020 7265  known" )).    re
+00007ed0: 7475 726e 2063 6f6e 7465 6e74 2c20 7265  turn content, re
+00007ee0: 7370 6f6e 7365 0a0a 0a64 6566 2063 7265  sponse...def cre
+00007ef0: 6465 6e74 6961 6c73 5f72 6571 7565 7374  dentials_request
+00007f00: 2820 7265 6e64 6572 2c20 7061 7468 2c20  ( render, path, 
+00007f10: 656e 7669 726f 6e2c 2061 6363 6570 742c  environ, accept,
+00007f20: 2066 7261 6d65 776f 726b 2c0a 2020 2020   framework,.    
+00007f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007f40: 2020 2020 2071 7565 7269 6573 3d4e 6f6e       queries=Non
+00007f50: 652c 2070 6f73 7465 643d 4e6f 6e65 2c0a  e, posted=None,.
+00007f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007f70: 2020 2020 2020 2020 2073 6573 7369 6f6e           session
+00007f80: 3d4e 6f6e 652c 206c 6f67 6765 643d 4e6f  =None, logged=No
+00007f90: 6e65 2c09 0923 2054 6865 2075 7365 7220  ne,..# The user 
+00007fa0: 7365 7373 696f 6e0a 2020 2020 2020 2020  session.        
+00007fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007fc0: 2070 726f 7879 3d4e 6f6e 6520 293a 0a0a   proxy=None ):..
+00007fd0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00007fe0: 6170 692f 6372 6564 656e 7469 616c 732f  api/credentials/
+00007ff0: 3c6e 616d 653e 2f0a 0a20 2020 2022 2222  <name>/..    """
+00008000: 0a20 2020 2076 6172 6961 626c 6573 0909  .    variables..
+00008010: 093d 2071 7565 7269 6573 206f 7220 706f  .= queries or po
+00008020: 7374 6564 206f 7220 7b7d 0a20 2020 2063  sted or {}.    c
+00008030: 6f6e 7465 6e74 0909 093d 2064 6564 7563  ontent...= deduc
+00008040: 655f 656e 636f 6469 6e67 2820 5b20 2274  e_encoding( [ "t
+00008050: 6578 742f 6874 6d6c 222c 0a20 2020 2020  ext/html",.     
+00008060: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008070: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008090: 2020 2020 2020 2022 7465 7874 2f70 6c61         "text/pla
-000080a0: 696e 2220 5d2c 0a20 2020 2020 2020 2020  in" ],.         
-000080b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008090: 2261 7070 6c69 6361 7469 6f6e 2f6a 736f  "application/jso
+000080a0: 6e22 2c20 2274 6578 742f 6a61 7661 7363  n", "text/javasc
+000080b0: 7269 7074 222c 0a20 2020 2020 2020 2020  ript",.         
 000080c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000080d0: 2020 2020 2020 2020 2020 656e 7669 726f            enviro
-000080e0: 6e3d 656e 7669 726f 6e2c 2061 6363 6570  n=environ, accep
-000080f0: 743d 6163 6365 7074 2029 0a20 2020 2072  t=accept ).    r
-00008100: 6573 706f 6e73 6509 0909 3d20 2222 0a0a  esponse...= ""..
-00008110: 2020 2020 6461 7461 0909 093d 2063 7265      data...= cre
-00008120: 6465 6e74 6961 6c73 5f64 6174 6128 2070  dentials_data( p
-00008130: 6174 6820 290a 0a20 2020 2069 6620 636f  ath )..    if co
-00008140: 6e74 656e 7420 616e 6420 636f 6e74 656e  ntent and conten
-00008150: 7420 696e 2028 2022 6170 706c 6963 6174  t in ( "applicat
-00008160: 696f 6e2f 6a73 6f6e 222c 2022 7465 7874  ion/json", "text
-00008170: 2f6a 6176 6173 6372 6970 7422 2c20 2274  /javascript", "t
-00008180: 6578 742f 706c 6169 6e22 2029 3a0a 2020  ext/plain" ):.  
-00008190: 2020 2020 2020 6361 6c6c 6261 636b 0909        callback..
-000081a0: 3d20 7661 7269 6162 6c65 732e 6765 7428  = variables.get(
-000081b0: 2027 6361 6c6c 6261 636b 272c 2022 2220   'callback', "" 
-000081c0: 290a 2020 2020 2020 2020 6966 2063 616c  ).        if cal
-000081d0: 6c62 6163 6b3a 0a20 2020 2020 2020 2020  lback:.         
-000081e0: 2020 2072 6573 706f 6e73 6520 2020 2020     response     
-000081f0: 2020 2020 2020 2b3d 2063 616c 6c62 6163        += callbac
-00008200: 6b20 2b20 2228 2022 0a20 2020 2020 2020  k + "( ".       
-00008210: 2072 6573 706f 6e73 6520 2020 2020 2020   response       
-00008220: 2020 2020 2020 2020 2b3d 206c 6963 656e          += licen
-00008230: 7369 6e67 2e69 6e74 6f5f 4a53 4f4e 2820  sing.into_JSON( 
-00008240: 6461 7461 2c20 696e 6465 6e74 3d34 2029  data, indent=4 )
-00008250: 0a20 2020 2020 2020 2069 6620 6361 6c6c  .        if call
-00008260: 6261 636b 3a0a 2020 2020 2020 2020 2020  back:.          
-00008270: 2020 7265 7370 6f6e 7365 2020 2020 2020    response      
-00008280: 2020 2020 202b 3d20 2220 2922 0a20 2020       += " )".   
-00008290: 2065 6c69 6620 636f 6e74 656e 7420 616e   elif content an
-000082a0: 6420 636f 6e74 656e 7420 696e 2028 2022  d content in ( "
-000082b0: 7465 7874 2f68 746d 6c22 2029 3a0a 2020  text/html" ):.  
-000082c0: 2020 2020 2020 7265 7370 6f6e 7365 0909        response..
-000082d0: 3d20 7265 6e64 6572 2e6b 6579 6c69 7374  = render.keylist
-000082e0: 2820 6461 7461 2029 0a20 2020 2065 6c73  ( data ).    els
-000082f0: 653a 0a20 2020 2020 2020 2072 6169 7365  e:.        raise
-00008300: 2068 7474 705f 6578 6365 7074 696f 6e28   http_exception(
-00008310: 2066 7261 6d65 776f 726b 2c20 3430 362c   framework, 406,
-00008320: 2022 556e 6162 6c65 2074 6f20 7072 6f64   "Unable to prod
-00008330: 7563 6520 2573 2063 6f6e 7465 6e74 2220  uce %s content" 
-00008340: 2520 280a 2020 2020 2020 2020 2020 2020  % (.            
-00008350: 636f 6e74 656e 7420 6f72 2061 6363 6570  content or accep
-00008360: 7420 6f72 2022 756e 6b6e 6f77 6e22 2029  t or "unknown" )
-00008370: 290a 2020 2020 7265 7475 726e 2063 6f6e  ).    return con
-00008380: 7465 6e74 2c20 7265 7370 6f6e 7365 0a0a  tent, response..
-00008390: 0a64 6566 206b 6579 7061 6972 735f 7265  .def keypairs_re
-000083a0: 7175 6573 7428 2072 656e 6465 722c 2070  quest( render, p
-000083b0: 6174 682c 2065 6e76 6972 6f6e 2c20 6163  ath, environ, ac
-000083c0: 6365 7074 2c20 6672 616d 6577 6f72 6b2c  cept, framework,
-000083d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000083e0: 2020 2020 2020 2020 2020 7175 6572 6965            querie
-000083f0: 733d 4e6f 6e65 2c20 706f 7374 6564 3d4e  s=None, posted=N
-00008400: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
-00008410: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00008420: 7373 696f 6e3d 4e6f 6e65 2c20 6c6f 6767  ssion=None, logg
-00008430: 6564 3d4e 6f6e 652c 0909 2320 5468 6520  ed=None,..# The 
-00008440: 7573 6572 2073 6573 7369 6f6e 0a20 2020  user session.   
-00008450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008460: 2020 2020 2020 7072 6f78 793d 4e6f 6e65        proxy=None
-00008470: 2029 3a0a 0a20 2020 2022 2222 0a20 2020   ):..    """.   
-00008480: 2020 2020 2061 7069 2f6b 6579 7061 6972       api/keypair
-00008490: 732f 3c6e 616d 653e 2f0a 0a20 2020 2022  s/<name>/..    "
-000084a0: 2222 0a20 2020 2076 6172 6961 626c 6573  "".    variables
-000084b0: 0909 093d 2071 7565 7269 6573 206f 7220  ...= queries or 
-000084c0: 706f 7374 6564 206f 7220 7b7d 0a20 2020  posted or {}.   
-000084d0: 2063 6f6e 7465 6e74 0909 093d 2064 6564   content...= ded
-000084e0: 7563 655f 656e 636f 6469 6e67 2820 5b20  uce_encoding( [ 
-000084f0: 2274 6578 742f 6874 6d6c 222c 0a20 2020  "text/html",.   
-00008500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008530: 2020 2261 7070 6c69 6361 7469 6f6e 2f6a    "application/j
-00008540: 736f 6e22 2c20 2274 6578 742f 6a61 7661  son", "text/java
-00008550: 7363 7269 7074 222c 0a20 2020 2020 2020  script",.       
+000080d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000080e0: 2020 2020 2020 2020 2020 2020 2274 6578              "tex
+000080f0: 742f 706c 6169 6e22 205d 2c0a 2020 2020  t/plain" ],.    
+00008100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008120: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00008130: 6e76 6972 6f6e 3d65 6e76 6972 6f6e 2c20  nviron=environ, 
+00008140: 6163 6365 7074 3d61 6363 6570 7420 290a  accept=accept ).
+00008150: 2020 2020 7265 7370 6f6e 7365 0909 093d      response...=
+00008160: 2022 220a 0a20 2020 2064 6174 6109 0909   ""..    data...
+00008170: 3d20 6372 6564 656e 7469 616c 735f 6461  = credentials_da
+00008180: 7461 2820 7061 7468 2029 0a0a 2020 2020  ta( path )..    
+00008190: 6966 2063 6f6e 7465 6e74 2061 6e64 2063  if content and c
+000081a0: 6f6e 7465 6e74 2069 6e20 2820 2261 7070  ontent in ( "app
+000081b0: 6c69 6361 7469 6f6e 2f6a 736f 6e22 2c20  lication/json", 
+000081c0: 2274 6578 742f 6a61 7661 7363 7269 7074  "text/javascript
+000081d0: 222c 2022 7465 7874 2f70 6c61 696e 2220  ", "text/plain" 
+000081e0: 293a 0a20 2020 2020 2020 2063 616c 6c62  ):.        callb
+000081f0: 6163 6b09 093d 2076 6172 6961 626c 6573  ack..= variables
+00008200: 2e67 6574 2820 2763 616c 6c62 6163 6b27  .get( 'callback'
+00008210: 2c20 2222 2029 0a20 2020 2020 2020 2069  , "" ).        i
+00008220: 6620 6361 6c6c 6261 636b 3a0a 2020 2020  f callback:.    
+00008230: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
+00008240: 2020 2020 2020 2020 2020 202b 3d20 6361             += ca
+00008250: 6c6c 6261 636b 202b 2022 2820 220a 2020  llback + "( ".  
+00008260: 2020 2020 2020 7265 7370 6f6e 7365 2020        response  
+00008270: 2020 2020 2020 2020 2020 2020 202b 3d20               += 
+00008280: 6c69 6365 6e73 696e 672e 696e 746f 5f4a  licensing.into_J
+00008290: 534f 4e28 2064 6174 612c 2069 6e64 656e  SON( data, inden
+000082a0: 743d 3420 290a 2020 2020 2020 2020 6966  t=4 ).        if
+000082b0: 2063 616c 6c62 6163 6b3a 0a20 2020 2020   callback:.     
+000082c0: 2020 2020 2020 2072 6573 706f 6e73 6520         response 
+000082d0: 2020 2020 2020 2020 2020 2b3d 2022 2029            += " )
+000082e0: 220a 2020 2020 656c 6966 2063 6f6e 7465  ".    elif conte
+000082f0: 6e74 2061 6e64 2063 6f6e 7465 6e74 2069  nt and content i
+00008300: 6e20 2820 2274 6578 742f 6874 6d6c 2220  n ( "text/html" 
+00008310: 293a 0a20 2020 2020 2020 2072 6573 706f  ):.        respo
+00008320: 6e73 6509 093d 2072 656e 6465 722e 6b65  nse..= render.ke
+00008330: 796c 6973 7428 2064 6174 6120 290a 2020  ylist( data ).  
+00008340: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00008350: 7261 6973 6520 6874 7470 5f65 7863 6570  raise http_excep
+00008360: 7469 6f6e 2820 6672 616d 6577 6f72 6b2c  tion( framework,
+00008370: 2034 3036 2c20 2255 6e61 626c 6520 746f   406, "Unable to
+00008380: 2070 726f 6475 6365 2025 7320 636f 6e74   produce %s cont
+00008390: 656e 7422 2025 2028 0a20 2020 2020 2020  ent" % (.       
+000083a0: 2020 2020 2063 6f6e 7465 6e74 206f 7220       content or 
+000083b0: 6163 6365 7074 206f 7220 2275 6e6b 6e6f  accept or "unkno
+000083c0: 776e 2220 2929 0a20 2020 2072 6574 7572  wn" )).    retur
+000083d0: 6e20 636f 6e74 656e 742c 2072 6573 706f  n content, respo
+000083e0: 6e73 650a 0a0a 6465 6620 6b65 7970 6169  nse...def keypai
+000083f0: 7273 5f72 6571 7565 7374 2820 7265 6e64  rs_request( rend
+00008400: 6572 2c20 7061 7468 2c20 656e 7669 726f  er, path, enviro
+00008410: 6e2c 2061 6363 6570 742c 2066 7261 6d65  n, accept, frame
+00008420: 776f 726b 2c0a 2020 2020 2020 2020 2020  work,.          
+00008430: 2020 2020 2020 2020 2020 2020 2020 2071                 q
+00008440: 7565 7269 6573 3d4e 6f6e 652c 2070 6f73  ueries=None, pos
+00008450: 7465 643d 4e6f 6e65 2c0a 2020 2020 2020  ted=None,.      
+00008460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008470: 2020 2073 6573 7369 6f6e 3d4e 6f6e 652c     session=None,
+00008480: 206c 6f67 6765 643d 4e6f 6e65 2c09 0923   logged=None,..#
+00008490: 2054 6865 2075 7365 7220 7365 7373 696f   The user sessio
+000084a0: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
+000084b0: 2020 2020 2020 2020 2020 2070 726f 7879             proxy
+000084c0: 3d4e 6f6e 6520 293a 0a0a 2020 2020 2222  =None ):..    ""
+000084d0: 220a 2020 2020 2020 2020 6170 692f 6b65  ".        api/ke
+000084e0: 7970 6169 7273 2f3c 6e61 6d65 3e2f 0a0a  ypairs/<name>/..
+000084f0: 2020 2020 2222 220a 2020 2020 7661 7269      """.    vari
+00008500: 6162 6c65 7309 0909 3d20 7175 6572 6965  ables...= querie
+00008510: 7320 6f72 2070 6f73 7465 6420 6f72 207b  s or posted or {
+00008520: 7d0a 2020 2020 636f 6e74 656e 7409 0909  }.    content...
+00008530: 3d20 6465 6475 6365 5f65 6e63 6f64 696e  = deduce_encodin
+00008540: 6728 205b 2022 7465 7874 2f68 746d 6c22  g( [ "text/html"
+00008550: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
 00008560: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008580: 2020 2020 2020 2020 2020 2020 2020 2274                "t
-00008590: 6578 742f 706c 6169 6e22 205d 2c0a 2020  ext/plain" ],.  
-000085a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008580: 2020 2020 2020 2022 6170 706c 6963 6174         "applicat
+00008590: 696f 6e2f 6a73 6f6e 222c 2022 7465 7874  ion/json", "text
+000085a0: 2f6a 6176 6173 6372 6970 7422 2c0a 2020  /javascript",.  
 000085b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000085c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000085d0: 2065 6e76 6972 6f6e 3d65 6e76 6972 6f6e   environ=environ
-000085e0: 2c20 6163 6365 7074 3d61 6363 6570 7420  , accept=accept 
-000085f0: 290a 2020 2020 7265 7370 6f6e 7365 0909  ).    response..
-00008600: 093d 2022 220a 2020 2020 6461 7461 0909  .= "".    data..
-00008610: 093d 206b 6579 7061 6972 735f 6461 7461  .= keypairs_data
-00008620: 2820 7061 7468 2029 0a0a 2020 2020 6966  ( path )..    if
-00008630: 2063 6f6e 7465 6e74 2061 6e64 2063 6f6e   content and con
-00008640: 7465 6e74 2069 6e20 2820 2261 7070 6c69  tent in ( "appli
-00008650: 6361 7469 6f6e 2f6a 736f 6e22 2c20 2274  cation/json", "t
-00008660: 6578 742f 6a61 7661 7363 7269 7074 222c  ext/javascript",
-00008670: 2022 7465 7874 2f70 6c61 696e 2220 293a   "text/plain" ):
-00008680: 0a20 2020 2020 2020 2063 616c 6c62 6163  .        callbac
-00008690: 6b09 093d 2076 6172 6961 626c 6573 2e67  k..= variables.g
-000086a0: 6574 2820 2763 616c 6c62 6163 6b27 2c20  et( 'callback', 
-000086b0: 2222 2029 0a20 2020 2020 2020 2069 6620  "" ).        if 
-000086c0: 6361 6c6c 6261 636b 3a0a 2020 2020 2020  callback:.      
-000086d0: 2020 2020 2020 7265 7370 6f6e 7365 2020        response  
-000086e0: 2020 2020 2020 2020 202b 3d20 6361 6c6c           += call
-000086f0: 6261 636b 202b 2022 2820 220a 2020 2020  back + "( ".    
-00008700: 2020 2020 7265 7370 6f6e 7365 2020 2020      response    
-00008710: 2020 2020 2020 2020 2020 202b 3d20 6c69             += li
-00008720: 6365 6e73 696e 672e 696e 746f 5f4a 534f  censing.into_JSO
-00008730: 4e28 2064 6174 612c 2069 6e64 656e 743d  N( data, indent=
-00008740: 3420 290a 2020 2020 2020 2020 6966 2063  4 ).        if c
-00008750: 616c 6c62 6163 6b3a 0a20 2020 2020 2020  allback:.       
-00008760: 2020 2020 2072 6573 706f 6e73 6520 2020       response   
-00008770: 2020 2020 2020 2020 2b3d 2022 2029 220a          += " )".
-00008780: 2020 2020 656c 6966 2063 6f6e 7465 6e74      elif content
-00008790: 2061 6e64 2063 6f6e 7465 6e74 2069 6e20   and content in 
-000087a0: 2820 2274 6578 742f 6874 6d6c 2220 293a  ( "text/html" ):
-000087b0: 0a20 2020 2020 2020 2072 6573 706f 6e73  .        respons
-000087c0: 6509 093d 2072 656e 6465 722e 6b65 796c  e..= render.keyl
-000087d0: 6973 7428 2064 6174 6120 290a 2020 2020  ist( data ).    
-000087e0: 656c 7365 3a0a 2020 2020 2020 2020 7261  else:.        ra
-000087f0: 6973 6520 6874 7470 5f65 7863 6570 7469  ise http_excepti
-00008800: 6f6e 2820 6672 616d 6577 6f72 6b2c 2034  on( framework, 4
-00008810: 3036 2c20 2255 6e61 626c 6520 746f 2070  06, "Unable to p
-00008820: 726f 6475 6365 2025 7320 636f 6e74 656e  roduce %s conten
-00008830: 7422 2025 2028 0a20 2020 2020 2020 2020  t" % (.         
-00008840: 2020 2063 6f6e 7465 6e74 206f 7220 6163     content or ac
-00008850: 6365 7074 206f 7220 2275 6e6b 6e6f 776e  cept or "unknown
-00008860: 2220 2929 0a20 2020 2072 6574 7572 6e20  " )).    return 
-00008870: 636f 6e74 656e 742c 2072 6573 706f 6e73  content, respons
-00008880: 650a 0a0a 6465 6620 6973 7375 655f 7265  e...def issue_re
-00008890: 7175 6573 7428 2072 656e 6465 722c 2070  quest( render, p
-000088a0: 6174 682c 2065 6e76 6972 6f6e 2c20 6163  ath, environ, ac
-000088b0: 6365 7074 2c20 6672 616d 6577 6f72 6b2c  cept, framework,
-000088c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000088d0: 2020 2020 2071 7565 7269 6573 3d4e 6f6e       queries=Non
-000088e0: 652c 2070 6f73 7465 643d 4e6f 6e65 2c20  e, posted=None, 
-000088f0: 6c6f 6767 6564 3d4e 6f6e 652c 2070 726f  logged=None, pro
-00008900: 7879 3d4e 6f6e 6520 293a 0a20 2020 2022  xy=None ):.    "
-00008910: 2222 5265 7475 726e 7320 6120 4c69 6365  ""Returns a Lice
-00008920: 6e73 6520 6973 7375 616e 6365 2072 6573  nse issuance res
-00008930: 706f 6e73 652c 2061 7320 4854 4d4c 206f  ponse, as HTML o
-00008940: 7220 4a53 4f4e 2e0a 0a20 2020 2020 2020  r JSON...       
-00008950: 2061 7069 2f69 7373 7565 0909 2d2d 2061   api/issue..-- a
-00008960: 6c6c 206c 6963 656e 7365 730a 0a20 2020  ll licenses..   
-00008970: 2057 6865 6e20 616e 2061 7070 6c69 6361   When an applica
-00008980: 7469 6f6e 2072 756e 6e69 6e67 206f 6e20  tion running on 
-00008990: 6120 686f 7374 2066 696e 6473 2074 6861  a host finds tha
-000089a0: 7420 6974 2064 6f65 7320 6e6f 7420 6861  t it does not ha
-000089b0: 7665 2061 6e20 6170 7072 6f70 7269 6174  ve an appropriat
-000089c0: 6520 7369 676e 6564 204c 6963 656e 7365  e signed License
-000089d0: 0a20 2020 2061 7661 696c 6162 6c65 2c20  .    available, 
-000089e0: 6974 206d 6179 2072 6571 7565 7374 206f  it may request o
-000089f0: 6e65 2066 726f 6d20 6120 6370 7070 6f2e  ne from a cpppo.
-00008a00: 6372 7970 746f 2e6c 6963 656e 7369 6e67  crypto.licensing
-00008a10: 2073 6572 7665 722e 2020 4966 2073 7563   server.  If suc
-00008a20: 6820 6120 4c69 6365 6e73 6520 6973 0a20  h a License is. 
-00008a30: 2020 2061 7661 696c 6162 6c65 2074 6f20     available to 
-00008a40: 6973 7375 652c 2069 7420 7769 6c6c 2062  issue, it will b
-00008a50: 6520 7265 7475 726e 6564 2e0a 0a20 2020  e returned...   
-00008a60: 2049 6620 6e6f 7420 6176 6169 6c61 626c   If not availabl
-00008a70: 652c 2069 6e73 7472 7563 7469 6f6e 7320  e, instructions 
-00008a80: 6f6e 2068 6f77 2074 6f20 6765 7420 7468  on how to get th
-00008a90: 6520 4c69 6365 6e73 6520 6973 7375 6564  e License issued
-00008aa0: 2061 7265 2072 6574 7572 6e65 6420 2865   are returned (e
-00008ab0: 672e 2061 6772 6565 2074 6f0a 2020 2020  g. agree to.    
-00008ac0: 6c69 6365 6e73 696e 6720 7465 726d 7320  licensing terms 
-00008ad0: 6279 2070 6179 696e 6720 5553 4443 2431  by paying USDC$1
-00008ae0: 3030 2e30 3020 746f 2045 7468 6572 6575  00.00 to Ethereu
-00008af0: 6d20 6164 6472 6573 7320 3078 3331 3933  m address 0x3193
-00008b00: 2e2e 2e31 6565 3329 2e20 2041 7320 736f  ...1ee3).  As so
-00008b10: 6f6e 2061 7320 7468 650a 2020 2020 4c69  on as the.    Li
-00008b20: 6365 6e73 6520 7365 7276 6572 2073 6565  cense server see
-00008b30: 7320 7468 6174 2074 6865 2063 6f6e 7472  s that the contr
-00008b40: 6163 7475 616c 2072 6571 7569 7265 6d65  actual requireme
-00008b50: 6e74 2068 6173 2062 6565 6e20 6d65 742c  nt has been met,
-00008b60: 2074 6865 206c 6963 656e 7365 2069 7320   the license is 
-00008b70: 6973 7375 6564 2061 6e64 2074 6865 0a20  issued and the. 
-00008b80: 2020 206e 6578 7420 6361 6c6c 2074 6f20     next call to 
-00008b90: 7468 6520 7361 6d65 2061 7069 2f69 7373  the same api/iss
-00008ba0: 7565 2e2e 2e20 656e 6470 6f69 6e74 2077  ue... endpoint w
-00008bb0: 696c 6c20 7265 7475 726e 2074 6865 206e  ill return the n
-00008bc0: 6577 6c79 2045 6432 3535 3931 2d73 6967  ewly Ed25591-sig
-00008bd0: 6e65 6420 4c69 6365 6e73 652e 0a0a 2020  ned License...  
-00008be0: 2020 4966 2074 6865 204c 6963 656e 7365    If the License
-00008bf0: 2073 7065 6369 6669 6573 2061 2063 6572   specifies a cer
-00008c00: 7461 696e 2043 6c69 656e 7420 5075 626c  tain Client Publ
-00008c10: 6963 206b 6579 2c20 7468 656e 2074 6865  ic key, then the
-00008c20: 2072 6571 7565 7374 206d 7573 7420 6265   request must be
-00008c30: 2073 6967 6e65 6420 6279 2074 6865 0a20   signed by the. 
-00008c40: 2020 2063 6f72 7265 7370 6f6e 6469 6e67     corresponding
-00008c50: 2045 6432 3535 3139 2053 6967 6e69 6e67   Ed25519 Signing
-00008c60: 206b 6579 2e20 2054 6869 7320 6973 2061   key.  This is a
-00008c70: 6c6d 6f73 7420 6365 7274 6169 6e6c 7920  lmost certainly 
-00008c80: 7468 6520 6361 7365 3b20 6973 7375 696e  the case; issuin
-00008c90: 6720 4c69 6365 6e73 6573 2077 6974 6820  g Licenses with 
-00008ca0: 610a 2020 2020 226e 756c 6c22 2f4e 6f6e  a.    "null"/Non
-00008cb0: 6520 636c 6965 6e74 202d 2d20 7468 6174  e client -- that
-00008cc0: 2061 6c6c 6f77 2073 7562 2d4c 6963 656e   allow sub-Licen
-00008cd0: 7369 6e67 2074 6f20 6f74 6865 7220 636c  sing to other cl
-00008ce0: 6965 6e74 7320 2d2d 2069 7320 6e6f 7420  ients -- is not 
-00008cf0: 6c69 6b65 6c79 2073 6f6d 6574 6869 6e67  likely something
-00008d00: 2079 6f75 0a20 2020 2077 616e 7420 746f   you.    want to
-00008d10: 2064 6f20 6175 746f 6d61 7469 6361 6c6c   do automaticall
-00008d20: 792e 2020 5468 6973 2070 726f 7665 7320  y.  This proves 
-00008d30: 7468 6174 2074 6865 2072 6571 7565 7374  that the request
-00008d40: 6572 2069 7320 6163 7475 616c 6c79 2074  er is actually t
-00008d50: 6865 2043 6c69 656e 743b 206e 6f74 206a  he Client; not j
-00008d60: 7573 740a 2020 2020 736f 6d65 6f6e 6520  ust.    someone 
-00008d70: 7768 6f20 6b6e 6f77 7320 7468 6520 436c  who knows the Cl
-00008d80: 6965 6e74 2773 2070 7562 6c69 6320 6b65  ient's public ke
-00008d90: 792e 0a0a 2020 2020 4f6e 6c79 2069 6620  y...    Only if 
-00008da0: 7375 6666 6963 6965 6e74 204c 6963 656e  sufficient Licen
-00008db0: 7365 2873 2920 6172 6520 6176 6169 6c61  se(s) are availa
-00008dc0: 626c 6520 696e 2074 6865 2073 6572 7665  ble in the serve
-00008dd0: 7220 7769 6c6c 2074 6865 7920 6265 2069  r will they be i
-00008de0: 7373 7565 642e 0a0a 2020 2020 2222 220a  ssued...    """.
-00008df0: 2020 2020 2320 5768 656e 2075 7369 6e67      # When using
-00008e00: 206a 5175 6572 7920 242e 616a 6178 2829   jQuery $.ajax()
-00008e10: 2077 2f64 6174 6154 7970 653a 2027 6a73   w/dataType: 'js
-00008e20: 6f6e 7027 2c20 6974 2061 7070 656e 6473  onp', it appends
-00008e30: 2061 0a20 2020 2023 203f 6361 6c6c 6261   a.    # ?callba
-00008e40: 636b 3d2e 2e2e 2071 7565 7279 2c20 616e  ck=... query, an
-00008e50: 6420 7365 6e64 7320 616e 2041 6363 6570  d sends an Accep
-00008e60: 743a 202e 2e2e 2074 6578 742f 6a61 7661  t: ... text/java
-00008e70: 7363 7269 7074 0a20 2020 2023 2068 6561  script.    # hea
-00008e80: 6465 722e 2020 4865 6e63 652c 2061 6363  der.  Hence, acc
-00008e90: 6570 7420 6569 7468 6572 2066 6f72 6d2e  ept either form.
-00008ea0: 0a20 2020 2063 6f6e 7465 6e74 0909 093d  .    content...=
-00008eb0: 2064 6564 7563 655f 656e 636f 6469 6e67   deduce_encoding
-00008ec0: 2820 5b20 2274 6578 742f 6874 6d6c 222c  ( [ "text/html",
-00008ed0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008f00: 2020 2020 2020 2261 7070 6c69 6361 7469        "applicati
-00008f10: 6f6e 2f6a 736f 6e22 2c20 2274 6578 742f  on/json", "text/
-00008f20: 6a61 7661 7363 7269 7074 222c 0a20 2020  javascript",.   
+000085d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000085e0: 2020 2022 7465 7874 2f70 6c61 696e 2220     "text/plain" 
+000085f0: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+00008600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008620: 2020 2020 2020 656e 7669 726f 6e3d 656e        environ=en
+00008630: 7669 726f 6e2c 2061 6363 6570 743d 6163  viron, accept=ac
+00008640: 6365 7074 2029 0a20 2020 2072 6573 706f  cept ).    respo
+00008650: 6e73 6509 0909 3d20 2222 0a20 2020 2064  nse...= "".    d
+00008660: 6174 6109 0909 3d20 6b65 7970 6169 7273  ata...= keypairs
+00008670: 5f64 6174 6128 2070 6174 6820 290a 0a20  _data( path ).. 
+00008680: 2020 2069 6620 636f 6e74 656e 7420 616e     if content an
+00008690: 6420 636f 6e74 656e 7420 696e 2028 2022  d content in ( "
+000086a0: 6170 706c 6963 6174 696f 6e2f 6a73 6f6e  application/json
+000086b0: 222c 2022 7465 7874 2f6a 6176 6173 6372  ", "text/javascr
+000086c0: 6970 7422 2c20 2274 6578 742f 706c 6169  ipt", "text/plai
+000086d0: 6e22 2029 3a0a 2020 2020 2020 2020 6361  n" ):.        ca
+000086e0: 6c6c 6261 636b 0909 3d20 7661 7269 6162  llback..= variab
+000086f0: 6c65 732e 6765 7428 2027 6361 6c6c 6261  les.get( 'callba
+00008700: 636b 272c 2022 2220 290a 2020 2020 2020  ck', "" ).      
+00008710: 2020 6966 2063 616c 6c62 6163 6b3a 0a20    if callback:. 
+00008720: 2020 2020 2020 2020 2020 2072 6573 706f             respo
+00008730: 6e73 6520 2020 2020 2020 2020 2020 2b3d  nse           +=
+00008740: 2063 616c 6c62 6163 6b20 2b20 2228 2022   callback + "( "
+00008750: 0a20 2020 2020 2020 2072 6573 706f 6e73  .        respons
+00008760: 6520 2020 2020 2020 2020 2020 2020 2020  e               
+00008770: 2b3d 206c 6963 656e 7369 6e67 2e69 6e74  += licensing.int
+00008780: 6f5f 4a53 4f4e 2820 6461 7461 2c20 696e  o_JSON( data, in
+00008790: 6465 6e74 3d34 2029 0a20 2020 2020 2020  dent=4 ).       
+000087a0: 2069 6620 6361 6c6c 6261 636b 3a0a 2020   if callback:.  
+000087b0: 2020 2020 2020 2020 2020 7265 7370 6f6e            respon
+000087c0: 7365 2020 2020 2020 2020 2020 202b 3d20  se           += 
+000087d0: 2220 2922 0a20 2020 2065 6c69 6620 636f  " )".    elif co
+000087e0: 6e74 656e 7420 616e 6420 636f 6e74 656e  ntent and conten
+000087f0: 7420 696e 2028 2022 7465 7874 2f68 746d  t in ( "text/htm
+00008800: 6c22 2029 3a0a 2020 2020 2020 2020 7265  l" ):.        re
+00008810: 7370 6f6e 7365 0909 3d20 7265 6e64 6572  sponse..= render
+00008820: 2e6b 6579 6c69 7374 2820 6461 7461 2029  .keylist( data )
+00008830: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
+00008840: 2020 2072 6169 7365 2068 7474 705f 6578     raise http_ex
+00008850: 6365 7074 696f 6e28 2066 7261 6d65 776f  ception( framewo
+00008860: 726b 2c20 3430 362c 2022 556e 6162 6c65  rk, 406, "Unable
+00008870: 2074 6f20 7072 6f64 7563 6520 2573 2063   to produce %s c
+00008880: 6f6e 7465 6e74 2220 2520 280a 2020 2020  ontent" % (.    
+00008890: 2020 2020 2020 2020 636f 6e74 656e 7420          content 
+000088a0: 6f72 2061 6363 6570 7420 6f72 2022 756e  or accept or "un
+000088b0: 6b6e 6f77 6e22 2029 290a 2020 2020 7265  known" )).    re
+000088c0: 7475 726e 2063 6f6e 7465 6e74 2c20 7265  turn content, re
+000088d0: 7370 6f6e 7365 0a0a 0a64 6566 2069 7373  sponse...def iss
+000088e0: 7565 5f72 6571 7565 7374 2820 7265 6e64  ue_request( rend
+000088f0: 6572 2c20 7061 7468 2c20 656e 7669 726f  er, path, enviro
+00008900: 6e2c 2061 6363 6570 742c 2066 7261 6d65  n, accept, frame
+00008910: 776f 726b 2c0a 2020 2020 2020 2020 2020  work,.          
+00008920: 2020 2020 2020 2020 2020 7175 6572 6965            querie
+00008930: 733d 4e6f 6e65 2c20 706f 7374 6564 3d4e  s=None, posted=N
+00008940: 6f6e 652c 206c 6f67 6765 643d 4e6f 6e65  one, logged=None
+00008950: 2c20 7072 6f78 793d 4e6f 6e65 2029 3a0a  , proxy=None ):.
+00008960: 2020 2020 2222 2252 6574 7572 6e73 2061      """Returns a
+00008970: 204c 6963 656e 7365 2069 7373 7561 6e63   License issuanc
+00008980: 6520 7265 7370 6f6e 7365 2c20 6173 2048  e response, as H
+00008990: 544d 4c20 6f72 204a 534f 4e2e 0a0a 2020  TML or JSON...  
+000089a0: 2020 2020 2020 6170 692f 6973 7375 6509        api/issue.
+000089b0: 092d 2d20 616c 6c20 6c69 6365 6e73 6573  .-- all licenses
+000089c0: 0a0a 2020 2020 5768 656e 2061 6e20 6170  ..    When an ap
+000089d0: 706c 6963 6174 696f 6e20 7275 6e6e 696e  plication runnin
+000089e0: 6720 6f6e 2061 2068 6f73 7420 6669 6e64  g on a host find
+000089f0: 7320 7468 6174 2069 7420 646f 6573 206e  s that it does n
+00008a00: 6f74 2068 6176 6520 616e 2061 7070 726f  ot have an appro
+00008a10: 7072 6961 7465 2073 6967 6e65 6420 4c69  priate signed Li
+00008a20: 6365 6e73 650a 2020 2020 6176 6169 6c61  cense.    availa
+00008a30: 626c 652c 2069 7420 6d61 7920 7265 7175  ble, it may requ
+00008a40: 6573 7420 6f6e 6520 6672 6f6d 2061 2063  est one from a c
+00008a50: 7070 706f 2e63 7279 7074 6f2e 6c69 6365  pppo.crypto.lice
+00008a60: 6e73 696e 6720 7365 7276 6572 2e20 2049  nsing server.  I
+00008a70: 6620 7375 6368 2061 204c 6963 656e 7365  f such a License
+00008a80: 2069 730a 2020 2020 6176 6169 6c61 626c   is.    availabl
+00008a90: 6520 746f 2069 7373 7565 2c20 6974 2077  e to issue, it w
+00008aa0: 696c 6c20 6265 2072 6574 7572 6e65 642e  ill be returned.
+00008ab0: 0a0a 2020 2020 4966 206e 6f74 2061 7661  ..    If not ava
+00008ac0: 696c 6162 6c65 2c20 696e 7374 7275 6374  ilable, instruct
+00008ad0: 696f 6e73 206f 6e20 686f 7720 746f 2067  ions on how to g
+00008ae0: 6574 2074 6865 204c 6963 656e 7365 2069  et the License i
+00008af0: 7373 7565 6420 6172 6520 7265 7475 726e  ssued are return
+00008b00: 6564 2028 6567 2e20 6167 7265 6520 746f  ed (eg. agree to
+00008b10: 0a20 2020 206c 6963 656e 7369 6e67 2074  .    licensing t
+00008b20: 6572 6d73 2062 7920 7061 7969 6e67 2055  erms by paying U
+00008b30: 5344 4324 3130 302e 3030 2074 6f20 4574  SDC$100.00 to Et
+00008b40: 6865 7265 756d 2061 6464 7265 7373 2030  hereum address 0
+00008b50: 7833 3139 332e 2e2e 3165 6533 292e 2020  x3193...1ee3).  
+00008b60: 4173 2073 6f6f 6e20 6173 2074 6865 0a20  As soon as the. 
+00008b70: 2020 204c 6963 656e 7365 2073 6572 7665     License serve
+00008b80: 7220 7365 6573 2074 6861 7420 7468 6520  r sees that the 
+00008b90: 636f 6e74 7261 6374 7561 6c20 7265 7175  contractual requ
+00008ba0: 6972 656d 656e 7420 6861 7320 6265 656e  irement has been
+00008bb0: 206d 6574 2c20 7468 6520 6c69 6365 6e73   met, the licens
+00008bc0: 6520 6973 2069 7373 7565 6420 616e 6420  e is issued and 
+00008bd0: 7468 650a 2020 2020 6e65 7874 2063 616c  the.    next cal
+00008be0: 6c20 746f 2074 6865 2073 616d 6520 6170  l to the same ap
+00008bf0: 692f 6973 7375 652e 2e2e 2065 6e64 706f  i/issue... endpo
+00008c00: 696e 7420 7769 6c6c 2072 6574 7572 6e20  int will return 
+00008c10: 7468 6520 6e65 776c 7920 4564 3235 3539  the newly Ed2559
+00008c20: 312d 7369 676e 6564 204c 6963 656e 7365  1-signed License
+00008c30: 2e0a 0a20 2020 2049 6620 7468 6520 4c69  ...    If the Li
+00008c40: 6365 6e73 6520 7370 6563 6966 6965 7320  cense specifies 
+00008c50: 6120 6365 7274 6169 6e20 436c 6965 6e74  a certain Client
+00008c60: 2050 7562 6c69 6320 6b65 792c 2074 6865   Public key, the
+00008c70: 6e20 7468 6520 7265 7175 6573 7420 6d75  n the request mu
+00008c80: 7374 2062 6520 7369 676e 6564 2062 7920  st be signed by 
+00008c90: 7468 650a 2020 2020 636f 7272 6573 706f  the.    correspo
+00008ca0: 6e64 696e 6720 4564 3235 3531 3920 5369  nding Ed25519 Si
+00008cb0: 676e 696e 6720 6b65 792e 2020 5468 6973  gning key.  This
+00008cc0: 2069 7320 616c 6d6f 7374 2063 6572 7461   is almost certa
+00008cd0: 696e 6c79 2074 6865 2063 6173 653b 2069  inly the case; i
+00008ce0: 7373 7569 6e67 204c 6963 656e 7365 7320  ssuing Licenses 
+00008cf0: 7769 7468 2061 0a20 2020 2022 6e75 6c6c  with a.    "null
+00008d00: 222f 4e6f 6e65 2063 6c69 656e 7420 2d2d  "/None client --
+00008d10: 2074 6861 7420 616c 6c6f 7720 7375 622d   that allow sub-
+00008d20: 4c69 6365 6e73 696e 6720 746f 206f 7468  Licensing to oth
+00008d30: 6572 2063 6c69 656e 7473 202d 2d20 6973  er clients -- is
+00008d40: 206e 6f74 206c 696b 656c 7920 736f 6d65   not likely some
+00008d50: 7468 696e 6720 796f 750a 2020 2020 7761  thing you.    wa
+00008d60: 6e74 2074 6f20 646f 2061 7574 6f6d 6174  nt to do automat
+00008d70: 6963 616c 6c79 2e20 2054 6869 7320 7072  ically.  This pr
+00008d80: 6f76 6573 2074 6861 7420 7468 6520 7265  oves that the re
+00008d90: 7175 6573 7465 7220 6973 2061 6374 7561  quester is actua
+00008da0: 6c6c 7920 7468 6520 436c 6965 6e74 3b20  lly the Client; 
+00008db0: 6e6f 7420 6a75 7374 0a20 2020 2073 6f6d  not just.    som
+00008dc0: 656f 6e65 2077 686f 206b 6e6f 7773 2074  eone who knows t
+00008dd0: 6865 2043 6c69 656e 7427 7320 7075 626c  he Client's publ
+00008de0: 6963 206b 6579 2e0a 0a20 2020 204f 6e6c  ic key...    Onl
+00008df0: 7920 6966 2073 7566 6669 6369 656e 7420  y if sufficient 
+00008e00: 4c69 6365 6e73 6528 7329 2061 7265 2061  License(s) are a
+00008e10: 7661 696c 6162 6c65 2069 6e20 7468 6520  vailable in the 
+00008e20: 7365 7276 6572 2077 696c 6c20 7468 6579  server will they
+00008e30: 2062 6520 6973 7375 6564 2e0a 0a20 2020   be issued...   
+00008e40: 2022 2222 0a20 2020 2023 2057 6865 6e20   """.    # When 
+00008e50: 7573 696e 6720 6a51 7565 7279 2024 2e61  using jQuery $.a
+00008e60: 6a61 7828 2920 772f 6461 7461 5479 7065  jax() w/dataType
+00008e70: 3a20 276a 736f 6e70 272c 2069 7420 6170  : 'jsonp', it ap
+00008e80: 7065 6e64 7320 610a 2020 2020 2320 3f63  pends a.    # ?c
+00008e90: 616c 6c62 6163 6b3d 2e2e 2e20 7175 6572  allback=... quer
+00008ea0: 792c 2061 6e64 2073 656e 6473 2061 6e20  y, and sends an 
+00008eb0: 4163 6365 7074 3a20 2e2e 2e20 7465 7874  Accept: ... text
+00008ec0: 2f6a 6176 6173 6372 6970 740a 2020 2020  /javascript.    
+00008ed0: 2320 6865 6164 6572 2e20 2048 656e 6365  # header.  Hence
+00008ee0: 2c20 6163 6365 7074 2065 6974 6865 7220  , accept either 
+00008ef0: 666f 726d 2e0a 2020 2020 636f 6e74 656e  form..    conten
+00008f00: 7409 0909 3d20 6465 6475 6365 5f65 6e63  t...= deduce_enc
+00008f10: 6f64 696e 6728 205b 2022 7465 7874 2f68  oding( [ "text/h
+00008f20: 746d 6c22 2c0a 2020 2020 2020 2020 2020  tml",.          
 00008f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008f60: 2020 2274 6578 742f 706c 6169 6e22 205d    "text/plain" ]
-00008f70: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00008f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008f50: 2020 2020 2020 2020 2020 2022 6170 706c             "appl
+00008f60: 6963 6174 696f 6e2f 6a73 6f6e 222c 2022  ication/json", "
+00008f70: 7465 7874 2f6a 6176 6173 6372 6970 7422  text/javascript"
+00008f80: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
 00008f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008fa0: 2020 2020 2065 6e76 6972 6f6e 3d65 6e76       environ=env
-00008fb0: 6972 6f6e 2c20 6163 6365 7074 3d61 6363  iron, accept=acc
-00008fc0: 6570 7420 290a 2020 2020 7265 7370 6f6e  ept ).    respon
-00008fd0: 7365 0909 093d 2022 220a 0a20 2020 2076  se...= ""..    v
-00008fe0: 6172 6961 626c 6573 0909 093d 2071 7565  ariables...= que
-00008ff0: 7269 6573 206f 7220 706f 7374 6564 206f  ries or posted o
-00009000: 7220 7b7d 0a0a 2020 2020 2320 4675 6c6c  r {}..    # Full
-00009010: 2073 7065 6369 6669 6361 7469 6f6e 7320   specifications 
-00009020: 6f66 2064 6573 6972 6564 204c 6963 656e  of desired Licen
-00009030: 7365 2e20 204d 7573 7420 696e 636c 7564  se.  Must includ
-00009040: 6520 636c 6965 6e74 5f70 7562 6b65 792e  e client_pubkey.
-00009050: 0a20 2020 2063 6f6e 6669 726d 0909 093d  .    confirm...=
-00009060: 206c 6963 656e 7369 6e67 2e69 6e74 6f5f   licensing.into_
-00009070: 626f 6f6c 6561 6e28 2076 6172 6961 626c  boolean( variabl
-00009080: 6573 2e67 6574 2820 2763 6f6e 6669 726d  es.get( 'confirm
-00009090: 272c 2046 616c 7365 2029 2c20 7472 7574  ', False ), trut
-000090a0: 6879 3d28 2727 2c29 2029 0a20 2020 2061  hy=('',) ).    a
-000090b0: 7574 686f 7209 0909 3d20 7661 7269 6162  uthor...= variab
-000090c0: 6c65 732e 6765 7428 2027 6175 7468 6f72  les.get( 'author
-000090d0: 2720 290a 2020 2020 6175 7468 6f72 5f70  ' ).    author_p
-000090e0: 7562 6b65 7909 093d 2076 6172 6961 626c  ubkey..= variabl
-000090f0: 6573 2e67 6574 2820 2761 7574 686f 725f  es.get( 'author_
-00009100: 7075 626b 6579 2720 290a 2020 2020 7072  pubkey' ).    pr
-00009110: 6f64 7563 7409 0909 3d20 7661 7269 6162  oduct...= variab
-00009120: 6c65 732e 6765 7428 2027 7072 6f64 7563  les.get( 'produc
-00009130: 7427 2029 0a20 2020 2063 6c69 656e 7409  t' ).    client.
-00009140: 0909 3d20 7661 7269 6162 6c65 732e 6765  ..= variables.ge
-00009150: 7428 2027 636c 6965 6e74 2720 290a 2020  t( 'client' ).  
-00009160: 2020 636c 6965 6e74 5f70 7562 6b65 7909    client_pubkey.
-00009170: 093d 2076 6172 6961 626c 6573 2e67 6574  .= variables.get
-00009180: 2820 2763 6c69 656e 745f 7075 626b 6579  ( 'client_pubkey
-00009190: 2720 2909 0923 204d 7573 7420 7369 676e  ' )..# Must sign
-000091a0: 2074 6865 2069 7373 7565 2072 6571 7565   the issue reque
-000091b0: 7374 0a20 2020 206d 6163 6869 6e65 0909  st.    machine..
-000091c0: 093d 2076 6172 6961 626c 6573 2e67 6574  .= variables.get
-000091d0: 2820 276d 6163 6869 6e65 2720 290a 2020  ( 'machine' ).  
-000091e0: 2020 7369 676e 6174 7572 6509 0909 3d20    signature...= 
-000091f0: 7661 7269 6162 6c65 732e 6765 7428 2027  variables.get( '
-00009200: 7369 676e 6174 7572 6527 2029 0a20 2020  signature' ).   
-00009210: 206e 756d 6265 7209 0909 3d20 7661 7269   number...= vari
-00009220: 6162 6c65 732e 6765 7428 2027 6e75 6d62  ables.get( 'numb
-00009230: 6572 2720 2909 0909 2320 6f70 7469 6f6e  er' )...# option
-00009240: 616c 2063 6c69 656e 742d 7375 7070 6c69  al client-suppli
-00009250: 6564 2073 6572 6961 6c69 7a61 7469 6f6e  ed serialization
-00009260: 0a0a 2020 2020 2320 544f 444f 3a20 7665  ..    # TODO: ve
-00009270: 7269 6679 2074 6865 2073 6967 6e61 7475  rify the signatu
-00009280: 7265 2069 7320 7468 6174 206f 6620 7468  re is that of th
-00009290: 6520 6f72 6967 696e 616c 2063 616e 6f6e  e original canon
-000092a0: 6963 616c 697a 6564 2c20 7365 7269 616c  icalized, serial
-000092b0: 697a 6564 2049 7373 7565 5265 7175 6573  ized IssueReques
-000092c0: 7420 7061 796c 6f61 640a 2020 2020 230a  t payload.    #.
-000092d0: 2020 2020 2320 2020 2020 2e2e 2e3f 6175      #     ...?au
-000092e0: 7468 6f72 3d42 6c61 682c 2532 3049 6e63  thor=Blah,%20Inc
-000092f0: 2663 6c69 656e 745f 7075 626b 6579 3d2e  &client_pubkey=.
-00009300: 2e2e 266d 6163 6869 6e65 3d30 3030 3130  ..&machine=00010
-00009310: 3230 332d 2e2e 2e30 6530 6626 7369 676e  203-...0e0f&sign
-00009320: 6174 7572 653d 3944 6261 2e2e 2e43 673d  ature=9Dba...Cg=
-00009330: 3d0a 2020 2020 2320 2020 2020 2020 2020  =.    #         
-00009340: 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e  ^^^^^^^^^^^^^^^^
-00009350: 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e  ^^^^^^^^^^^^^^^^
-00009360: 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e  ^^^^^^^^^^^^^^^^
-00009370: 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e0a 2020  ^^^^^^^^^^^^^.  
-00009380: 2020 230a 2020 2020 2320 5765 206d 7573    #.    # We mus
-00009390: 7420 7365 7269 616c 697a 6520 7468 6520  t serialize the 
-000093a0: 7265 7175 6573 7420 696e 2061 2073 7461  request in a sta
-000093b0: 6e64 6172 6420 7761 7920 696e 2074 6865  ndard way in the
-000093c0: 2073 656e 6465 7220 616e 6420 7468 6520   sender and the 
-000093d0: 7265 6365 6976 6572 2c20 6265 6361 7573  receiver, becaus
-000093e0: 6520 7468 650a 2020 2020 2320 6461 7461  e the.    # data
-000093f0: 206d 6179 2062 6520 7365 6e74 2061 7320   may be sent as 
-00009400: 5552 4c20 6172 6775 6d65 6e74 7320 6f72  URL arguments or
-00009410: 2050 4f53 5420 6865 6164 6572 2076 6172   POST header var
-00009420: 6961 626c 6573 2e0a 2020 2020 6973 7375  iables..    issu
-00009430: 655f 7265 7175 6573 7409 093d 206c 6963  e_request..= lic
-00009440: 656e 7369 6e67 2e49 7373 7565 5265 7175  ensing.IssueRequ
-00009450: 6573 7428 0a20 2020 2020 2020 2061 7574  est(.        aut
-00009460: 686f 723d 6175 7468 6f72 2c20 6175 7468  hor=author, auth
-00009470: 6f72 5f70 7562 6b65 793d 6175 7468 6f72  or_pubkey=author
-00009480: 5f70 7562 6b65 792c 2070 726f 6475 6374  _pubkey, product
-00009490: 3d70 726f 6475 6374 2c0a 2020 2020 2020  =product,.      
-000094a0: 2020 636c 6965 6e74 3d63 6c69 656e 742c    client=client,
-000094b0: 2063 6c69 656e 745f 7075 626b 6579 3d63   client_pubkey=c
-000094c0: 6c69 656e 745f 7075 626b 6579 2c20 6d61  lient_pubkey, ma
-000094d0: 6368 696e 653d 6d61 6368 696e 6520 290a  chine=machine ).
-000094e0: 2020 2020 6c6f 672e 696e 666f 2820 2249      log.info( "I
-000094f0: 7373 7565 2072 6571 7565 7374 206e 756d  ssue request num
-00009500: 6265 723d 7b6e 756d 6265 727d 3b20 7b72  ber={number}; {r
-00009510: 6571 7d2c 2077 2f20 7369 676e 6174 7572  eq}, w/ signatur
-00009520: 653a 207b 7369 6721 727d 222e 666f 726d  e: {sig!r}".form
-00009530: 6174 280a 2020 2020 2020 2020 6e75 6d62  at(.        numb
-00009540: 6572 3d6e 756d 6265 722c 2072 6571 3d73  er=number, req=s
-00009550: 7472 2820 6973 7375 655f 7265 7175 6573  tr( issue_reques
-00009560: 7420 292c 2073 6967 3d73 6967 6e61 7475  t ), sig=signatu
-00009570: 7265 2029 290a 2020 2020 7472 793a 0a20  re )).    try:. 
-00009580: 2020 2020 2020 2069 7373 7565 5f72 6571         issue_req
-00009590: 7565 7374 2e76 6572 6966 7928 2070 7562  uest.verify( pub
-000095a0: 6b65 793d 636c 6965 6e74 5f70 7562 6b65  key=client_pubke
-000095b0: 792c 2073 6967 6e61 7475 7265 3d73 6967  y, signature=sig
-000095c0: 6e61 7475 7265 2029 0a20 2020 2065 7863  nature ).    exc
-000095d0: 6570 7420 4578 6365 7074 696f 6e20 6173  ept Exception as
-000095e0: 2065 7863 3a0a 2020 2020 2020 2020 7261   exc:.        ra
-000095f0: 6973 6520 6874 7470 5f65 7863 6570 7469  ise http_excepti
-00009600: 6f6e 2820 6672 616d 6577 6f72 6b2c 2034  on( framework, 4
-00009610: 3031 2c20 2245 6432 3535 3139 2053 6967  01, "Ed25519 Sig
-00009620: 6e61 7475 7265 206f 6620 7265 7175 6573  nature of reques
-00009630: 7420 6973 2069 6e63 6f72 7265 6374 3a20  t is incorrect: 
-00009640: 7b65 7863 7d22 2e66 6f72 6d61 7428 0a20  {exc}".format(. 
-00009650: 2020 2020 2020 2020 2020 2065 7863 3d65             exc=e
-00009660: 7863 2029 290a 0a20 2020 2023 2053 6565  xc ))..    # See
-00009670: 2069 6620 7468 6572 6520 6172 6520 4c69   if there are Li
-00009680: 6365 6e73 6528 7329 2074 6861 7420 6d61  cense(s) that ma
-00009690: 7463 6820 6120 6365 7274 6169 6e20 706f  tch a certain po
-000096a0: 7274 696f 6e20 6f66 2074 6865 2072 6571  rtion of the req
-000096b0: 7569 7265 6d65 6e74 732e 2020 416e 2065  uirements.  An e
-000096c0: 7861 6374 206d 6174 6368 0a20 2020 2023  xact match.    #
-000096d0: 2063 616e 2062 6520 6469 7265 6374 6c79   can be directly
-000096e0: 2072 6574 7572 6e65 642e 2020 4120 7061   returned.  A pa
-000096f0: 7274 6961 6c20 6d61 7463 6820 6361 6e20  rtial match can 
-00009700: 6265 2073 7562 2d6c 6963 656e 7365 642e  be sub-licensed.
-00009710: 0a20 2020 2073 6b69 705f 7461 6220 3d20  .    skip_tab = 
-00009720: 7b0a 2020 2020 2020 2020 2763 6c69 656e  {.        'clien
-00009730: 7427 3a09 6c61 6d62 6461 206c 6963 3a20  t':.lambda lic: 
-00009740: 6c69 632e 636c 6965 6e74 2061 6e64 2069  lic.client and i
-00009750: 7373 7565 5f72 6571 7565 7374 5b27 636c  ssue_request['cl
-00009760: 6965 6e74 275d 2061 6e64 206c 6963 2e63  ient'] and lic.c
-00009770: 6c69 656e 745b 276e 616d 6527 5d20 213d  lient['name'] !=
-00009780: 2069 7373 7565 5f72 6571 7565 7374 5b27   issue_request['
-00009790: 636c 6965 6e74 275d 2c0a 2020 2020 2020  client'],.      
-000097a0: 2020 2763 6c69 656e 745f 7075 626b 6579    'client_pubkey
-000097b0: 273a 6c61 6d62 6461 206c 6963 3a20 6c69  ':lambda lic: li
-000097c0: 632e 636c 6965 6e74 2061 6e64 2069 7373  c.client and iss
-000097d0: 7565 5f72 6571 7565 7374 5b27 636c 6965  ue_request['clie
-000097e0: 6e74 5f70 7562 6b65 7927 5d20 616e 6420  nt_pubkey'] and 
-000097f0: 6c69 632e 636c 6965 6e74 5b27 7075 626b  lic.client['pubk
-00009800: 6579 275d 2021 3d20 6973 7375 655f 7265  ey'] != issue_re
-00009810: 7175 6573 745b 2763 6c69 656e 745f 7075  quest['client_pu
-00009820: 626b 6579 275d 2c0a 2020 2020 2020 2020  bkey'],.        
-00009830: 2761 7574 686f 7227 3a09 6c61 6d62 6461  'author':.lambda
-00009840: 206c 6963 3a20 6973 7375 655f 7265 7175   lic: issue_requ
-00009850: 6573 745b 2761 7574 686f 7227 5d20 616e  est['author'] an
-00009860: 6420 6c69 632e 6175 7468 6f72 5b27 6e61  d lic.author['na
-00009870: 6d65 275d 2021 3d20 6973 7375 655f 7265  me'] != issue_re
-00009880: 7175 6573 745b 2761 7574 686f 7227 5d2c  quest['author'],
-00009890: 0a20 2020 2020 2020 2027 6175 7468 6f72  .        'author
-000098a0: 5f70 7562 6b65 7927 3a6c 616d 6264 6120  _pubkey':lambda 
-000098b0: 6c69 633a 2069 7373 7565 5f72 6571 7565  lic: issue_reque
-000098c0: 7374 5b27 6175 7468 6f72 5f70 7562 6b65  st['author_pubke
-000098d0: 7927 5d20 616e 6420 6c69 632e 6175 7468  y'] and lic.auth
-000098e0: 6f72 5b27 7075 626b 6579 275d 2021 3d20  or['pubkey'] != 
-000098f0: 6973 7375 655f 7265 7175 6573 745b 2761  issue_request['a
-00009900: 7574 686f 725f 7075 626b 6579 275d 2c0a  uthor_pubkey'],.
-00009910: 2020 2020 2020 2020 2770 726f 6475 6374          'product
-00009920: 273a 096c 616d 6264 6120 6c69 633a 2069  ':.lambda lic: i
-00009930: 7373 7565 5f72 6571 7565 7374 5b27 7072  ssue_request['pr
-00009940: 6f64 7563 7427 5d20 616e 6420 6c69 632e  oduct'] and lic.
-00009950: 6175 7468 6f72 5b27 7072 6f64 7563 7427  author['product'
-00009960: 5d20 213d 2069 7373 7565 5f72 6571 7565  ] != issue_reque
-00009970: 7374 5b27 7072 6f64 7563 7427 5d2c 0a20  st['product'],. 
-00009980: 2020 2020 2020 2027 6d61 6368 696e 6527         'machine'
-00009990: 3a09 6c61 6d62 6461 206c 6963 3a20 6973  :.lambda lic: is
-000099a0: 7375 655f 7265 7175 6573 745b 276d 6163  sue_request['mac
-000099b0: 6869 6e65 275d 2061 6e64 206c 6963 5b27  hine'] and lic['
-000099c0: 6d61 6368 696e 6527 5d20 213d 2069 7373  machine'] != iss
-000099d0: 7565 5f72 6571 7565 7374 5b27 6d61 6368  ue_request['mach
-000099e0: 696e 6527 5d2c 0a20 2020 207d 0a0a 2020  ine'],.    }..  
-000099f0: 2020 6465 6620 7072 6f76 5f74 6f5f 6973    def prov_to_is
-00009a00: 7375 6528 293a 0a20 2020 2020 2020 2022  sue():.        "
-00009a10: 2222 5072 6f64 7563 6520 6120 4c69 6365  ""Produce a Lice
-00009a20: 6e73 6553 6967 6e65 6420 7375 6974 6162  nseSigned suitab
-00009a30: 6c65 2066 6f72 2074 6865 2063 6c69 656e  le for the clien
-00009a40: 7420 746f 2072 6563 6569 7665 2c20 7573  t to receive, us
-00009a50: 6520 6173 2061 2064 6570 656e 6465 6e63  e as a dependenc
-00009a60: 7920 6f66 2061 206e 6577 0a20 2020 2020  y of a new.     
-00009a70: 2020 204c 6963 656e 7365 2073 7065 6369     License speci
-00009a80: 6669 6320 746f 2074 6865 6972 206d 6163  fic to their mac
-00009a90: 6869 6e65 2c20 616e 6420 7369 676e 2061  hine, and sign a
-00009aa0: 6e64 2069 6e73 7461 6c6c 2e0a 0a20 2020  nd install...   
-00009ab0: 2020 2020 2053 696e 6365 2077 6520 7363       Since we sc
-00009ac0: 616e 2074 6865 2064 6174 6162 6173 6520  an the database 
-00009ad0: 276c 6963 656e 7365 7327 2074 6162 6c65  'licenses' table
-00009ae0: 2c20 646f 2073 6f6d 6520 636f 6d70 7574  , do some comput
-00009af0: 6174 696f 6e73 2061 6e64 2074 6865 6e20  ations and then 
-00009b00: 7570 6461 7465 2074 6865 2074 6162 6c65  update the table
-00009b10: 2c0a 2020 2020 2020 2020 7765 206e 6565  ,.        we nee
-00009b20: 6420 746f 2064 625f 6c6f 636b 2061 726f  d to db_lock aro
-00009b30: 756e 6420 7468 6973 2065 6e74 6972 6520  und this entire 
-00009b40: 7072 6f63 6573 732c 2074 6f20 6176 6f69  process, to avoi
-00009b50: 6420 6d75 6c74 6970 6c65 2073 696d 756c  d multiple simul
-00009b60: 7461 6e65 6f75 7320 7265 7175 6573 7473  taneous requests
-00009b70: 0a20 2020 2020 2020 2069 7373 7569 6e67  .        issuing
-00009b80: 2074 6865 2073 616d 6520 4c69 6365 6e73   the same Licens
-00009b90: 652e 2020 5369 6e63 6520 7765 2064 6f20  e.  Since we do 
-00009ba0: 6e6f 2044 4b49 4d20 636f 6e66 6972 6d61  no DKIM confirma
-00009bb0: 7469 6f6e 206f 7220 6f74 6865 7220 6e65  tion or other ne
-00009bc0: 7477 6f72 6b20 492f 4f20 6865 7265 2028  twork I/O here (
-00009bd0: 6f6e 6c79 0a20 2020 2020 2020 2066 696c  only.        fil
-00009be0: 6520 7265 6164 696e 6729 2c20 6974 2073  e reading), it s
-00009bf0: 686f 756c 6420 6265 2071 7569 636b 2e0a  hould be quick..
-00009c00: 0a20 2020 2020 2020 2022 2222 0a0a 2020  .        """..  
-00009c10: 2020 2020 2020 6465 6620 6c69 6373 5f66        def lics_f
-00009c20: 696c 7465 7265 6428 202a 6e61 6d65 7320  iltered( *names 
-00009c30: 293a 0a20 2020 2020 2020 2020 2020 2022  ):.            "
-00009c40: 2222 5363 616e 2074 6865 206c 6f61 6465  ""Scan the loade
-00009c50: 642f 7374 6f72 6564 204c 6963 656e 7365  d/stored License
-00009c60: 7320 666f 7220 2022 2222 0a20 2020 2020  s for  """.     
-00009c70: 2020 2020 2020 2073 746f 7265 6409 0909         stored...
-00009c80: 3d20 6c69 7374 2820 6462 2e73 656c 6563  = list( db.selec
-00009c90: 7428 2027 6c69 6365 6e73 6573 2720 2929  t( 'licenses' ))
-00009ca0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-00009cb0: 2073 6967 2c20 6c69 6320 696e 206c 6963   sig, lic in lic
-00009cc0: 656e 7365 7328 2063 6f6e 6669 726d 3d46  enses( confirm=F
-00009cd0: 616c 7365 2c20 7374 6f72 6564 3d73 746f  alse, stored=sto
-00009ce0: 7265 6420 293a 0a20 2020 2020 2020 2020  red ):.         
-00009cf0: 2020 2020 2020 206c 6f67 2e69 6e66 6f28         log.info(
-00009d00: 2022 4973 7375 6520 7265 7175 6573 7420   "Issue request 
-00009d10: 6e75 6d62 6572 3d7b 6e75 6d62 6572 7d3b  number={number};
-00009d20: 207b 6e61 6d65 7d27 7320 7b70 726f 6475   {name}'s {produ
-00009d30: 6374 7d3a 206d 6973 6d61 7463 6865 6420  ct}: mismatched 
-00009d40: 6b65 7973 3a20 7b6b 6579 737d 222e 666f  keys: {keys}".fo
-00009d50: 726d 6174 280a 2020 2020 2020 2020 2020  rmat(.          
-00009d60: 2020 2020 2020 2020 2020 6e75 6d62 6572            number
-00009d70: 3d6e 756d 6265 722c 206e 616d 653d 6c69  =number, name=li
-00009d80: 632e 6175 7468 6f72 5b27 6e61 6d65 275d  c.author['name']
-00009d90: 2c20 7072 6f64 7563 743d 6c69 632e 6175  , product=lic.au
-00009da0: 7468 6f72 5b27 7072 6f64 7563 7427 5d2c  thor['product'],
-00009db0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009dc0: 2020 2020 206b 6579 733d 272c 2027 2e6a       keys=', '.j
-00009dd0: 6f69 6e28 206e 2066 6f72 206e 2069 6e20  oin( n for n in 
-00009de0: 6e61 6d65 7320 6966 2073 6b69 705f 7461  names if skip_ta
-00009df0: 625b 6e5d 2820 6c69 6320 2920 2929 290a  b[n]( lic ) ))).
-00009e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009e10: 6966 2061 6e79 2820 736b 6970 5f74 6162  if any( skip_tab
-00009e20: 5b6e 5d28 206c 6963 2029 2066 6f72 206e  [n]( lic ) for n
-00009e30: 2069 6e20 6e61 6d65 7320 293a 0a20 2020   in names ):.   
-00009e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009e50: 2063 6f6e 7469 6e75 650a 2020 2020 2020   continue.      
-00009e60: 2020 2020 2020 2020 2020 6c6f 672e 696e            log.in
-00009e70: 666f 2820 2249 7373 7565 2072 6571 7565  fo( "Issue reque
-00009e80: 7374 206e 756d 6265 723d 7b6e 756d 6265  st number={numbe
-00009e90: 727d 3b20 7b6e 616d 657d 2773 207b 7072  r}; {name}'s {pr
-00009ea0: 6f64 7563 747d 2061 6363 6570 7465 643a  oduct} accepted:
-00009eb0: 207b 6c69 637d 222e 666f 726d 6174 280a   {lic}".format(.
-00009ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ed0: 2020 2020 6e75 6d62 6572 3d6e 756d 6265      number=numbe
-00009ee0: 722c 206e 616d 653d 6c69 632e 6175 7468  r, name=lic.auth
-00009ef0: 6f72 5b27 6e61 6d65 275d 2c20 7072 6f64  or['name'], prod
-00009f00: 7563 743d 6c69 632e 6175 7468 6f72 5b27  uct=lic.author['
-00009f10: 7072 6f64 7563 7427 5d2c 206c 6963 3d6c  product'], lic=l
-00009f20: 6963 2029 290a 2020 2020 2020 2020 2020  ic )).          
-00009f30: 2020 2020 2020 7969 656c 6420 7369 672c        yield sig,
-00009f40: 206c 6963 0a0a 2020 2020 2020 2020 2320   lic..        # 
-00009f50: 4964 6561 6c6c 792c 2065 7665 7279 7468  Ideally, everyth
-00009f60: 696e 6720 6d61 7463 6865 7320 6578 6163  ing matches exac
-00009f70: 746c 7920 6f6e 6520 7370 6563 6966 6963  tly one specific
-00009f80: 204c 6963 656e 7365 2061 6c72 6561 6479   License already
-00009f90: 2069 7373 7565 6420 746f 2074 6869 7320   issued to this 
-00009fa0: 436c 6965 6e74 2066 6f72 0a20 2020 2020  Client for.     
-00009fb0: 2020 2023 2074 6869 7320 6d61 6368 696e     # this machin
-00009fc0: 652e 2020 4966 2077 6527 7665 2061 6c72  e.  If we've alr
-00009fd0: 6561 6479 2069 7373 7565 6420 7468 6520  eady issued the 
-00009fe0: 4c69 6365 6e73 6520 2861 6e64 2070 6572  License (and per
-00009ff0: 6861 7073 2074 6865 2063 6c69 656e 7420  haps the client 
-0000a000: 666f 7267 6f74 2074 6f0a 2020 2020 2020  forgot to.      
-0000a010: 2020 2320 696e 7374 616c 6c20 6974 2c20    # install it, 
-0000a020: 6f72 2072 652d 696e 7374 616c 6c65 6420  or re-installed 
-0000a030: 7468 6520 736f 6674 7761 7265 292c 2061  the software), a
-0000a040: 6e64 206e 6565 6473 2069 7420 6167 6169  nd needs it agai
-0000a050: 6e2e 0a20 2020 2020 2020 2074 7279 3a0a  n..        try:.
-0000a060: 2020 2020 2020 2020 2020 2020 2873 6967              (sig
-0000a070: 2c20 6c69 6329 2c09 093d 206c 6963 735f  , lic),..= lics_
-0000a080: 6669 6c74 6572 6564 2820 2761 7574 686f  filtered( 'autho
-0000a090: 7227 2c20 2761 7574 686f 725f 7075 626b  r', 'author_pubk
-0000a0a0: 6579 272c 2027 7072 6f64 7563 7427 2c20  ey', 'product', 
-0000a0b0: 2763 6c69 656e 7427 2c20 2763 6c69 656e  'client', 'clien
-0000a0c0: 745f 7075 626b 6579 272c 2027 6d61 6368  t_pubkey', 'mach
-0000a0d0: 696e 6527 2029 0a20 2020 2020 2020 2065  ine' ).        e
-0000a0e0: 7863 6570 7420 5661 6c75 6545 7272 6f72  xcept ValueError
-0000a0f0: 2061 7320 6578 633a 0a20 2020 2020 2020   as exc:.       
-0000a100: 2020 2020 206c 6f67 2e77 6172 6e69 6e67       log.warning
-0000a110: 2820 2246 6169 6c65 643a 207b 6578 637d  ( "Failed: {exc}
-0000a120: 222e 666f 726d 6174 2820 6578 633d 6578  ".format( exc=ex
-0000a130: 6320 2929 0a20 2020 2020 2020 2020 2020  c )).           
-0000a140: 2070 6173 730a 2020 2020 2020 2020 656c   pass.        el
-0000a150: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0000a160: 6966 206c 6963 2e63 6c69 656e 7420 616e  if lic.client an
-0000a170: 6420 6c69 632e 6d61 6368 696e 653a 2020  d lic.machine:  
-0000a180: 2320 4578 6163 7420 6d61 7463 682c 2077  # Exact match, w
-0000a190: 6974 6820 7370 6563 6966 6963 2063 6c69  ith specific cli
-0000a1a0: 656e 7420 616e 6420 6d61 6368 696e 650a  ent and machine.
-0000a1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a1c0: 6c6f 672e 7761 726e 696e 6728 2022 4973  log.warning( "Is
-0000a1d0: 7375 6520 7265 7175 6573 7420 6e75 6d62  sue request numb
-0000a1e0: 6572 3d7b 6e75 6d62 6572 7d3b 2052 6569  er={number}; Rei
-0000a1f0: 7373 7569 6e67 2065 7869 7374 696e 6720  ssuing existing 
-0000a200: 4c69 6365 6e73 653a 207b 6c69 637d 222e  License: {lic}".
-0000a210: 666f 726d 6174 280a 2020 2020 2020 2020  format(.        
-0000a220: 2020 2020 2020 2020 2020 2020 6e75 6d62              numb
-0000a230: 6572 3d6e 756d 6265 722c 206c 6963 3d6c  er=number, lic=l
-0000a240: 6963 2069 6620 6c6f 672e 6973 456e 6162  ic if log.isEnab
-0000a250: 6c65 6446 6f72 2820 6c6f 6767 696e 672e  ledFor( logging.
-0000a260: 494e 464f 2029 2065 6c73 6520 6c69 6365  INFO ) else lice
-0000a270: 6e73 696e 672e 696e 746f 5f62 3634 2820  nsing.into_b64( 
-0000a280: 7369 6720 2929 290a 2020 2020 2020 2020  sig ))).        
-0000a290: 2020 2020 2020 2020 7265 7475 726e 206c          return l
-0000a2a0: 6963 656e 7369 6e67 2e4c 6963 656e 7365  icensing.License
-0000a2b0: 5369 676e 6564 280a 2020 2020 2020 2020  Signed(.        
-0000a2c0: 2020 2020 2020 2020 2020 2020 6c69 6365              lice
-0000a2d0: 6e73 653d 6c69 632c 2073 6967 6e61 7475  nse=lic, signatu
-0000a2e0: 7265 3d73 6967 2c20 636f 6e66 6972 6d3d  re=sig, confirm=
-0000a2f0: 4661 6c73 652c 206d 6163 6869 6e65 5f69  False, machine_i
-0000a300: 645f 7061 7468 3d46 616c 7365 2029 0a0a  d_path=False )..
-0000a310: 2020 2020 2020 2020 2320 4f4b 2c20 6e6f          # OK, no
-0000a320: 7420 616c 7265 6164 7920 6973 7375 6564  t already issued
-0000a330: 2e20 2046 696e 6420 6120 4c69 6365 6e73  .  Find a Licens
-0000a340: 6520 746f 2073 7065 6369 616c 697a 652e  e to specialize.
-0000a350: 2020 4966 206f 6e65 206d 6174 6368 6573    If one matches
-0000a360: 2074 6865 2061 7574 686f 7220 616e 640a   the author and.
-0000a370: 2020 2020 2020 2020 2320 636c 6965 6e74          # client
-0000a380: 2028 6f72 2073 7065 6369 6669 6573 206e   (or specifies n
-0000a390: 6f20 636c 6965 6e74 2920 616e 6420 6861  o client) and ha
-0000a3a0: 7320 6e6f 206d 6163 6869 6e65 2c20 7573  s no machine, us
-0000a3b0: 6520 6974 2074 6f20 6175 7468 6f72 2061  e it to author a
-0000a3c0: 206e 6577 204c 6963 656e 7365 2c20 7369   new License, si
-0000a3d0: 6d70 6c79 0a20 2020 2020 2020 2023 2073  mply.        # s
-0000a3e0: 7065 6369 616c 697a 6564 2077 6974 6820  pecialized with 
-0000a3f0: 7468 6520 636c 6965 6e74 2061 6e64 206d  the client and m
-0000a400: 6163 6869 6e65 2073 7065 6369 6669 6564  achine specified
-0000a410: 2e20 2054 6865 2063 6c69 656e 7420 7769  .  The client wi
-0000a420: 6c6c 2072 6563 6569 7665 2061 6e64 0a20  ll receive and. 
-0000a430: 2020 2020 2020 2023 2073 7562 2d4c 6963         # sub-Lic
-0000a440: 656e 7365 2069 7420 6279 2063 7265 6174  ense it by creat
-0000a450: 696e 6720 6120 6e65 7720 4c69 6365 6e73  ing a new Licens
-0000a460: 6520 7769 7468 2074 6869 7320 6120 6f6e  e with this a on
-0000a470: 6520 6f66 2069 7473 2064 6570 656e 6465  e of its depende
-0000a480: 6e63 6965 732c 2074 6865 6e20 7369 676e  ncies, then sign
-0000a490: 2069 740a 2020 2020 2020 2020 2320 7769   it.        # wi
-0000a4a0: 7468 2074 6865 2063 6c69 656e 7420 7369  th the client si
-0000a4b0: 676e 696e 6720 6b65 7920 7468 6579 2068  gning key they h
-0000a4c0: 6f6c 642c 2061 6e64 2069 6e73 7461 6c6c  old, and install
-0000a4d0: 2069 742e 0a20 2020 2020 2020 2074 7279   it..        try
-0000a4e0: 3a0a 2020 2020 2020 2020 2020 2020 2873  :.            (s
-0000a4f0: 6967 2c20 6c69 6329 2c09 093d 206c 6963  ig, lic),..= lic
-0000a500: 735f 6669 6c74 6572 6564 2820 2761 7574  s_filtered( 'aut
-0000a510: 686f 7227 2c20 2761 7574 686f 725f 7075  hor', 'author_pu
-0000a520: 626b 6579 272c 2027 7072 6f64 7563 7427  bkey', 'product'
-0000a530: 2c20 2763 6c69 656e 7427 2c20 2763 6c69  , 'client', 'cli
-0000a540: 656e 745f 7075 626b 6579 2720 290a 2020  ent_pubkey' ).  
-0000a550: 2020 2020 2020 6578 6365 7074 2056 616c        except Val
-0000a560: 7565 4572 726f 7220 6173 2065 7863 3a0a  ueError as exc:.
-0000a570: 2020 2020 2020 2020 2020 2020 6c6f 672e              log.
-0000a580: 7761 726e 696e 6728 2022 4661 696c 6564  warning( "Failed
-0000a590: 3a20 7b65 7863 7d22 2e66 6f72 6d61 7428  : {exc}".format(
-0000a5a0: 2065 7863 3d65 7863 2029 290a 2020 2020   exc=exc )).    
-0000a5b0: 2020 2020 2020 2020 7061 7373 0a20 2020          pass.   
-0000a5c0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000a5d0: 2020 2020 2020 2069 6620 6e6f 7420 6c69         if not li
-0000a5e0: 632e 6d61 6368 696e 6520 6f72 206c 6963  c.machine or lic
-0000a5f0: 5b27 6d61 6368 696e 6527 5d20 3d3d 2069  ['machine'] == i
-0000a600: 7373 7565 5f72 6571 7565 7374 5b27 6d61  ssue_request['ma
-0000a610: 6368 696e 6527 5d3a 0a20 2020 2020 2020  chine']:.       
-0000a620: 2020 2020 2020 2020 206c 6f67 2e69 6e66           log.inf
-0000a630: 6f28 2022 4973 7375 6520 7265 7175 6573  o( "Issue reques
-0000a640: 7420 6e75 6d62 6572 3d7b 6e75 6d62 6572  t number={number
-0000a650: 7d3b 2053 7065 6369 616c 697a 696e 6720  }; Specializing 
-0000a660: 6578 6973 7469 6e67 204c 6963 656e 7365  existing License
-0000a670: 3a20 7b6c 6963 7d22 2e66 6f72 6d61 7428  : {lic}".format(
-0000a680: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a690: 2020 2020 206e 756d 6265 723d 6e75 6d62       number=numb
-0000a6a0: 6572 2c20 6c69 633d 6c69 6320 6966 206c  er, lic=lic if l
-0000a6b0: 6f67 2e69 7345 6e61 626c 6564 466f 7228  og.isEnabledFor(
-0000a6c0: 206c 6f67 6769 6e67 2e49 4e46 4f20 2920   logging.INFO ) 
-0000a6d0: 656c 7365 206c 6963 656e 7369 6e67 2e69  else licensing.i
-0000a6e0: 6e74 6f5f 6236 3428 2073 6967 2929 290a  nto_b64( sig))).
-0000a6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a700: 6175 7468 6f72 5f73 6967 6b65 7909 3d20  author_sigkey.= 
-0000a710: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
-0000a720: 2020 2020 2066 6f72 206e 616d 652c 6b65       for name,ke
-0000a730: 7970 6169 722c 6372 6564 2069 6e20 6b65  ypair,cred in ke
-0000a740: 7970 6169 7273 2829 3a0a 2020 2020 2020  ypairs():.      
-0000a750: 2020 2020 2020 2020 2020 2020 2020 766b                vk
-0000a760: 2c20 736b 093d 206b 6579 7061 6972 2e69  , sk.= keypair.i
-0000a770: 6e74 6f5f 6b65 7970 6169 7228 202a 2a63  nto_keypair( **c
-0000a780: 7265 6420 290a 2020 2020 2020 2020 2020  red ).          
-0000a790: 2020 2020 2020 2020 2020 7075 626b 6579            pubkey
-0000a7a0: 093d 206c 6963 656e 7369 6e67 2e69 6e74  .= licensing.int
-0000a7b0: 6f5f 6236 3428 2076 6b20 290a 2020 2020  o_b64( vk ).    
-0000a7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a7d0: 6966 206e 616d 6520 3d3d 206c 6963 2e61  if name == lic.a
-0000a7e0: 7574 686f 725b 276e 616d 6527 5d20 616e  uthor['name'] an
-0000a7f0: 6420 7075 626b 6579 203d 3d20 6973 7375  d pubkey == issu
-0000a800: 655f 7265 7175 6573 745b 2761 7574 686f  e_request['autho
-0000a810: 725f 7075 626b 6579 275d 3a0a 2020 2020  r_pubkey']:.    
-0000a820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a830: 2020 2020 6175 7468 6f72 5f73 6967 6b65      author_sigke
-0000a840: 7920 3d20 736b 0a20 2020 2020 2020 2020  y = sk.         
-0000a850: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-0000a860: 7265 616b 0a20 2020 2020 2020 2020 2020  reak.           
-0000a870: 2020 2020 2023 2049 7373 7565 2061 206e       # Issue a n
-0000a880: 6577 2073 7065 6369 616c 697a 6564 204c  ew specialized L
-0000a890: 6963 656e 7365 2066 6f72 2043 6c69 656e  icense for Clien
-0000a8a0: 742c 2073 6967 6e65 6420 7769 7468 2041  t, signed with A
-0000a8b0: 7574 686f 7227 7320 7072 6976 6174 6520  uthor's private 
-0000a8c0: 7369 676e 696e 6720 6b65 792e 0a20 2020  signing key..   
-0000a8d0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000a8e0: 6e6f 7420 6c69 632e 636c 6965 6e74 3a0a  not lic.client:.
-0000a8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a900: 2020 2020 6c69 632e 636c 6965 6e74 093d      lic.client.=
-0000a910: 206c 6963 656e 7369 6e67 2e41 6765 6e74   licensing.Agent
-0000a920: 2820 6e61 6d65 3d69 7373 7565 5f72 6571  ( name=issue_req
-0000a930: 7565 7374 5b27 636c 6965 6e74 275d 2c20  uest['client'], 
-0000a940: 7075 626b 6579 3d69 7373 7565 5f72 6571  pubkey=issue_req
-0000a950: 7565 7374 5b27 636c 6965 6e74 5f70 7562  uest['client_pub
-0000a960: 6b65 7927 5d20 290a 2020 2020 2020 2020  key'] ).        
-0000a970: 2020 2020 2020 2020 6c69 632e 6d61 6368          lic.mach
-0000a980: 696e 6509 3d20 6c69 6365 6e73 696e 672e  ine.= licensing.
-0000a990: 696e 746f 5f55 5549 4476 3428 2069 7373  into_UUIDv4( iss
-0000a9a0: 7565 5f72 6571 7565 7374 5b27 6d61 6368  ue_request['mach
-0000a9b0: 696e 6527 5d20 290a 2020 2020 2020 2020  ine'] ).        
-0000a9c0: 2020 2020 2020 2020 7072 6f76 0909 3d20          prov..= 
-0000a9d0: 6c69 6365 6e73 696e 672e 6973 7375 6528  licensing.issue(
-0000a9e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a9f0: 2020 2020 206c 6963 656e 7365 3d6c 6963       license=lic
-0000aa00: 2c20 6175 7468 6f72 5f73 6967 6b65 793d  , author_sigkey=
-0000aa10: 6175 7468 6f72 5f73 6967 6b65 792c 2063  author_sigkey, c
-0000aa20: 6f6e 6669 726d 3d46 616c 7365 2c20 6d61  onfirm=False, ma
-0000aa30: 6368 696e 655f 6964 5f70 6174 683d 4661  chine_id_path=Fa
-0000aa40: 6c73 6520 290a 2020 2020 2020 2020 2020  lse ).          
-0000aa50: 2020 2020 2020 696e 7365 7274 203d 2064        insert = d
-0000aa60: 622e 696e 7365 7274 2820 276c 6963 656e  b.insert( 'licen
-0000aa70: 7365 7327 2c0a 2020 2020 2020 2020 2020  ses',.          
-0000aa80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aa90: 2020 2020 2020 2020 2020 7369 676e 6174            signat
-0000aaa0: 7572 653d 7072 6f76 5b27 7369 676e 6174  ure=prov['signat
-0000aab0: 7572 6527 5d2c 0a20 2020 2020 2020 2020  ure'],.         
-0000aac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aad0: 2020 2020 2020 2020 2020 206c 6963 656e             licen
-0000aae0: 7365 3d73 7472 2820 7072 6f76 2e6c 6963  se=str( prov.lic
-0000aaf0: 656e 7365 2029 290a 2020 2020 2020 2020  ense )).        
-0000ab00: 2020 2020 2020 2020 6173 7365 7274 2069          assert i
-0000ab10: 6e73 6572 742c 2022 5370 6563 6961 6c69  nsert, "Speciali
-0000ab20: 7a69 6e67 206c 6963 656e 7365 2069 6e73  zing license ins
-0000ab30: 6572 7420 6661 696c 6564 220a 2020 2020  ert failed".    
-0000ab40: 2020 2020 2020 2020 2020 2020 6c6f 672e              log.
-0000ab50: 7761 726e 696e 6728 2022 4973 7375 6520  warning( "Issue 
-0000ab60: 7265 7175 6573 7420 6e75 6d62 6572 3d7b  request number={
-0000ab70: 6e75 6d62 6572 7d3b 2049 7373 7565 6420  number}; Issued 
-0000ab80: 7370 6563 6961 6c69 7a65 6420 4c69 6365  specialized Lice
-0000ab90: 6e73 653a 207b 6c69 637d 222e 666f 726d  nse: {lic}".form
-0000aba0: 6174 280a 2020 2020 2020 2020 2020 2020  at(.            
-0000abb0: 2020 2020 2020 2020 6e75 6d62 6572 3d6e          number=n
-0000abc0: 756d 6265 722c 206c 6963 3d70 726f 762e  umber, lic=prov.
-0000abd0: 6c69 6365 6e73 6520 6966 206c 6f67 2e69  license if log.i
-0000abe0: 7345 6e61 626c 6564 466f 7228 206c 6f67  sEnabledFor( log
-0000abf0: 6769 6e67 2e49 4e46 4f20 2920 656c 7365  ging.INFO ) else
-0000ac00: 206c 6963 656e 7369 6e67 2e69 6e74 6f5f   licensing.into_
-0000ac10: 6236 3428 2070 726f 762e 7369 676e 6174  b64( prov.signat
-0000ac20: 7572 6520 2929 290a 2020 2020 2020 2020  ure ))).        
-0000ac30: 2020 2020 2020 2020 7265 7475 726e 2070          return p
-0000ac40: 726f 760a 0a20 2020 2020 2020 2072 6169  rov..        rai
-0000ac50: 7365 2068 7474 705f 6578 6365 7074 696f  se http_exceptio
-0000ac60: 6e28 2066 7261 6d65 776f 726b 2c20 3430  n( framework, 40
-0000ac70: 392c 2022 4e6f 206d 6174 6368 696e 6720  9, "No matching 
-0000ac80: 4c69 6365 6e73 6573 2066 6f75 6e64 206d  Licenses found m
-0000ac90: 6174 6368 696e 6720 7265 7175 6573 743a  atching request:
-0000aca0: 207b 7d22 2e66 6f72 6d61 7428 0a20 2020   {}".format(.   
-0000acb0: 2020 2020 2020 2020 2069 7373 7565 5f72           issue_r
-0000acc0: 6571 7565 7374 2029 290a 0a20 2020 2077  equest ))..    w
-0000acd0: 6974 6820 6462 5f6c 6f63 6b3a 0a20 2020  ith db_lock:.   
-0000ace0: 2020 2020 2070 726f 7609 0909 3d20 7072       prov...= pr
-0000acf0: 6f76 5f74 6f5f 6973 7375 6528 290a 2020  ov_to_issue().  
-0000ad00: 2020 6c6f 672e 696e 666f 2820 2249 7373    log.info( "Iss
-0000ad10: 7565 2072 6571 7565 7374 206e 756d 6265  ue request numbe
-0000ad20: 723d 7b6e 756d 6265 727d 3b20 4973 7375  r={number}; Issu
-0000ad30: 696e 6720 4c69 6365 6e73 6520 666f 7220  ing License for 
-0000ad40: 7b6e 616d 657d 2720 7b70 726f 6475 6374  {name}' {product
-0000ad50: 7d22 2e66 6f72 6d61 7428 0a20 2020 2020  }".format(.     
-0000ad60: 2020 206e 756d 6265 723d 6e75 6d62 6572     number=number
-0000ad70: 2c20 6e61 6d65 3d70 726f 762e 6c69 6365  , name=prov.lice
-0000ad80: 6e73 652e 6175 7468 6f72 5b27 6e61 6d65  nse.author['name
-0000ad90: 275d 2c20 7072 6f64 7563 743d 7072 6f76  '], product=prov
-0000ada0: 2e6c 6963 656e 7365 2e61 7574 686f 725b  .license.author[
-0000adb0: 2770 726f 6475 6374 275d 2029 290a 0a20  'product'] )).. 
-0000adc0: 2020 2064 6174 6109 0909 3d20 7b7d 0a20     data...= {}. 
-0000add0: 2020 2064 6174 615b 2274 6974 6c65 225d     data["title"]
-0000ade0: 0909 3d20 7061 7468 206f 7220 2249 7373  ..= path or "Iss
-0000adf0: 7565 220a 2020 2020 6461 7461 5b22 7061  ue".    data["pa
-0000ae00: 7468 225d 0909 3d20 7061 7468 0a20 2020  th"]..= path.   
-0000ae10: 2064 6174 615b 226c 6973 7422 5d20 3d20   data["list"] = 
-0000ae20: 6c6c 0909 3d20 5b5d 0a20 2020 2064 6174  ll..= [].    dat
-0000ae30: 615b 226b 6579 7322 5d09 093d 205b 2261  a["keys"]..= ["a
-0000ae40: 7574 686f 7222 2c20 2263 6c69 656e 7422  uthor", "client"
-0000ae50: 2c20 2270 726f 6475 6374 222c 2022 7369  , "product", "si
-0000ae60: 676e 6174 7572 6522 2c20 2263 6f6e 6669  gnature", "confi
-0000ae70: 726d 222c 2022 6c69 6365 6e73 6522 5d0a  rm", "license"].
-0000ae80: 0a20 2020 2072 6563 6f72 6409 0909 3d20  .    record...= 
-0000ae90: 6469 6374 280a 2020 2020 2020 2020 6175  dict(.        au
-0000aea0: 7468 6f72 0909 3d20 7072 6f76 2e6c 6963  thor..= prov.lic
-0000aeb0: 656e 7365 5b27 6175 7468 6f72 275d 5b27  ense['author']['
-0000aec0: 6e61 6d65 275d 2c0a 2020 2020 2020 2020  name'],.        
-0000aed0: 636c 6965 6e74 0909 3d20 7072 6f76 2e6c  client..= prov.l
-0000aee0: 6963 656e 7365 5b27 636c 6965 6e74 275d  icense['client']
-0000aef0: 5b27 6e61 6d65 275d 2c0a 2020 2020 2020  ['name'],.      
-0000af00: 2020 7072 6f64 7563 7409 093d 2070 726f    product..= pro
-0000af10: 762e 6c69 6365 6e73 655b 2761 7574 686f  v.license['autho
-0000af20: 7227 5d5b 2770 726f 6475 6374 275d 2c0a  r']['product'],.
-0000af30: 2020 2020 2020 2020 7369 676e 6174 7572          signatur
-0000af40: 6509 3d20 6c69 6365 6e73 696e 672e 696e  e.= licensing.in
-0000af50: 746f 5f62 3634 2820 7072 6f76 2e73 6967  to_b64( prov.sig
-0000af60: 6e61 7475 7265 2029 2c0a 2020 2020 2020  nature ),.      
-0000af70: 2020 636f 6e66 6972 6d09 093d 204e 6f6e    confirm..= Non
-0000af80: 652c 0a20 2020 2020 2020 206c 6963 656e  e,.        licen
-0000af90: 7365 0909 3d20 7072 6f76 2e6c 6963 656e  se..= prov.licen
-0000afa0: 7365 2c0a 2020 2020 290a 2020 2020 6966  se,.    ).    if
-0000afb0: 2063 6f6e 6669 726d 3a0a 2020 2020 2020   confirm:.      
-0000afc0: 2020 6c6f 672e 7761 726e 696e 6728 2022    log.warning( "
-0000afd0: 4973 7375 6520 7265 7175 6573 7420 6e75  Issue request nu
-0000afe0: 6d62 6572 3d7b 6e75 6d62 6572 7d3b 2043  mber={number}; C
-0000aff0: 6f6e 6669 726d 696e 6720 444b 494d 2066  onfirming DKIM f
-0000b000: 6f72 207b 6e61 6d65 7d27 207b 7072 6f64  or {name}' {prod
-0000b010: 7563 747d 222e 666f 726d 6174 280a 2020  uct}".format(.  
-0000b020: 2020 2020 2020 2020 2020 6e75 6d62 6572            number
-0000b030: 3d6e 756d 6265 722c 206e 616d 653d 7072  =number, name=pr
-0000b040: 6f76 2e6c 6963 656e 7365 2e61 7574 686f  ov.license.autho
-0000b050: 725b 276e 616d 6527 5d2c 2070 726f 6475  r['name'], produ
-0000b060: 6374 3d70 726f 762e 6c69 6365 6e73 652e  ct=prov.license.
-0000b070: 6175 7468 6f72 5b27 7072 6f64 7563 7427  author['product'
-0000b080: 5d20 2929 0a20 2020 2020 2020 2074 7279  ] )).        try
-0000b090: 3a0a 2020 2020 2020 2020 2020 2020 6c69  :.            li
-0000b0a0: 6365 6e73 696e 672e 7665 7269 6679 2820  censing.verify( 
-0000b0b0: 7072 6f76 2c20 636f 6e66 6972 6d3d 636f  prov, confirm=co
-0000b0c0: 6e66 6972 6d2c 206d 6163 6869 6e65 5f69  nfirm, machine_i
-0000b0d0: 645f 7061 7468 3d46 616c 7365 2029 0a20  d_path=False ). 
-0000b0e0: 2020 2020 2020 2065 7863 6570 7420 4578         except Ex
-0000b0f0: 6365 7074 696f 6e20 6173 2065 7863 3a0a  ception as exc:.
-0000b100: 2020 2020 2020 2020 2020 2020 7265 636f              reco
-0000b110: 7264 2e75 7064 6174 6528 2063 6f6e 6669  rd.update( confi
-0000b120: 726d 3d73 7472 2820 6578 6320 2929 0a20  rm=str( exc )). 
-0000b130: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-0000b140: 2020 2020 2020 2020 2072 6563 6f72 642e           record.
-0000b150: 7570 6461 7465 2820 636f 6e66 6972 6d3d  update( confirm=
-0000b160: 5472 7565 2029 0a20 2020 206c 6c2e 6170  True ).    ll.ap
-0000b170: 7065 6e64 2820 7265 636f 7264 2029 0a0a  pend( record )..
-0000b180: 2020 2020 6966 2063 6f6e 7465 6e74 2061      if content a
-0000b190: 6e64 2063 6f6e 7465 6e74 2069 6e20 2820  nd content in ( 
-0000b1a0: 2261 7070 6c69 6361 7469 6f6e 2f6a 736f  "application/jso
-0000b1b0: 6e22 2c20 2274 6578 742f 6a61 7661 7363  n", "text/javasc
-0000b1c0: 7269 7074 222c 2022 7465 7874 2f70 6c61  ript", "text/pla
-0000b1d0: 696e 2220 293a 0a20 2020 2020 2020 2063  in" ):.        c
-0000b1e0: 616c 6c62 6163 6b09 093d 2076 6172 6961  allback..= varia
-0000b1f0: 626c 6573 2e67 6574 2820 2763 616c 6c62  bles.get( 'callb
-0000b200: 6163 6b27 2c20 2222 2029 0a20 2020 2020  ack', "" ).     
-0000b210: 2020 2069 6620 6361 6c6c 6261 636b 3a0a     if callback:.
-0000b220: 2020 2020 2020 2020 2020 2020 7265 7370              resp
-0000b230: 6f6e 7365 2020 2020 2020 2020 2020 202b  onse           +
-0000b240: 3d20 6361 6c6c 6261 636b 202b 2022 2820  = callback + "( 
-0000b250: 220a 2020 2020 2020 2020 7265 7370 6f6e  ".        respon
-0000b260: 7365 2020 2020 2020 2020 2020 2020 2020  se              
-0000b270: 202b 3d20 6c69 6365 6e73 696e 672e 696e   += licensing.in
-0000b280: 746f 5f4a 534f 4e28 2064 6174 612c 2069  to_JSON( data, i
-0000b290: 6e64 656e 743d 3420 290a 2020 2020 2020  ndent=4 ).      
-0000b2a0: 2020 6966 2063 616c 6c62 6163 6b3a 0a20    if callback:. 
-0000b2b0: 2020 2020 2020 2020 2020 2072 6573 706f             respo
-0000b2c0: 6e73 6520 2020 2020 2020 2020 2020 2b3d  nse           +=
-0000b2d0: 2022 2029 220a 2020 2020 656c 6966 2063   " )".    elif c
-0000b2e0: 6f6e 7465 6e74 2061 6e64 2063 6f6e 7465  ontent and conte
-0000b2f0: 6e74 2069 6e20 2820 2274 6578 742f 6874  nt in ( "text/ht
-0000b300: 6d6c 2220 293a 0a20 2020 2020 2020 2072  ml" ):.        r
-0000b310: 6573 706f 6e73 6509 093d 2072 656e 6465  esponse..= rende
-0000b320: 722e 6b65 796c 6973 7428 2064 6174 6120  r.keylist( data 
-0000b330: 290a 2020 2020 656c 7365 3a0a 2020 2020  ).    else:.    
-0000b340: 2020 2020 7261 6973 6520 6874 7470 5f65      raise http_e
-0000b350: 7863 6570 7469 6f6e 2820 6672 616d 6577  xception( framew
-0000b360: 6f72 6b2c 2034 3036 2c20 2255 6e61 626c  ork, 406, "Unabl
-0000b370: 6520 746f 2070 726f 6475 6365 2025 7320  e to produce %s 
-0000b380: 636f 6e74 656e 7422 2025 2028 0a20 2020  content" % (.   
-0000b390: 2020 2020 2020 2020 2063 6f6e 7465 6e74           content
-0000b3a0: 206f 7220 6163 6365 7074 206f 7220 2275   or accept or "u
-0000b3b0: 6e6b 6e6f 776e 2220 2929 0a20 2020 206c  nknown" )).    l
-0000b3c0: 6f67 2e69 6e66 6f28 2249 7373 7565 2072  og.info("Issue r
-0000b3d0: 6571 7565 7374 206e 756d 6265 723d 7b6e  equest number={n
-0000b3e0: 756d 6265 727d 3b20 646f 6e65 222e 666f  umber}; done".fo
-0000b3f0: 726d 6174 2820 6e75 6d62 6572 3d6e 756d  rmat( number=num
-0000b400: 6265 7220 2929 0a20 2020 2072 6574 7572  ber )).    retur
-0000b410: 6e20 636f 6e74 656e 742c 2072 6573 706f  n content, respo
-0000b420: 6e73 650a 0a0a 6465 6620 696e 6c69 6e65  nse...def inline
-0000b430: 2820 6669 6c65 6e61 6d65 2029 3a0a 2020  ( filename ):.  
-0000b440: 2020 2222 2241 2077 6562 2e70 7920 7465    """A web.py te
-0000b450: 6d70 6c65 746f 7220 676c 6f62 616c 2066  mpletor global f
-0000b460: 756e 6374 696f 6e20 746f 2069 6e6c 696e  unction to inlin
-0000b470: 6520 6669 6c65 732c 2072 656c 6174 6976  e files, relativ
-0000b480: 6520 746f 2074 6865 0a20 2020 2064 6972  e to the.    dir
-0000b490: 6563 746f 7279 206f 6620 7468 6973 2070  ectory of this p
-0000b4a0: 7974 686f 6e20 6669 6c65 2e20 2055 7365  ython file.  Use
-0000b4b0: 3a0a 0a20 2020 2024 3a69 6e6c 696e 6528  :..    $:inline(
-0000b4c0: 2022 736f 6d65 2f6a 6176 6173 6372 6970   "some/javascrip
-0000b4d0: 742f 6669 6c65 2e6a 7322 2029 0a0a 2020  t/file.js" )..  
-0000b4e0: 2020 2222 220a 2020 2020 7769 7468 206f    """.    with o
-0000b4f0: 7065 6e28 206f 732e 7061 7468 2e6a 6f69  pen( os.path.joi
-0000b500: 6e28 204f 5552 5041 5448 2c20 6669 6c65  n( OURPATH, file
-0000b510: 6e61 6d65 2029 2c20 2772 2720 2920 6173  name ), 'r' ) as
-0000b520: 2066 3a0a 2020 2020 2020 2020 7265 7475   f:.        retu
-0000b530: 726e 2066 2e72 6561 6428 290a 0a0a 6465  rn f.read()...de
-0000b540: 6620 7765 6270 7928 2063 6f6e 6669 6720  f webpy( config 
-0000b550: 293a 0a20 2020 2022 2222 7765 622e 7079  ):.    """web.py
-0000b560: 2069 6e74 6572 6661 6365 2e20 2044 6564   interface.  Ded
-0000b570: 7563 6573 2061 6363 6570 7420 656e 636f  uces accept enco
-0000b580: 6469 6e67 2066 726f 6d20 4163 6365 7074  ding from Accept
-0000b590: 3a20 6865 6164 6572 2c20 6f72 2066 6f72  : header, or for
-0000b5a0: 6365 0a20 2020 204a 534f 4e20 436f 6e74  ce.    JSON Cont
-0000b5b0: 656e 742d 5479 7065 3a20 6966 202e 6a73  ent-Type: if .js
-0000b5c0: 6f6e 2070 6174 6820 7761 7320 6578 706c  on path was expl
-0000b5d0: 6963 6974 6c79 2072 6571 7565 7374 6564  icitly requested
-0000b5e0: 2e0a 0a20 2020 2022 2222 0a20 2020 2063  ...    """.    c
-0000b5f0: 6f6e 6669 672e 7365 7464 6566 6175 6c74  onfig.setdefault
-0000b600: 2820 2761 6464 7265 7373 272c 2822 302e  ( 'address',("0.
-0000b610: 302e 302e 3022 2c20 3830 3030 2920 290a  0.0.0", 8000) ).
-0000b620: 0a20 2020 2073 6573 7369 6f6e 0909 093d  .    session...=
-0000b630: 204e 6f6e 6509 0923 2057 696c 6c20 6265   None..# Will be
-0000b640: 636f 6d65 2061 2077 6562 2e73 6573 7369  come a web.sessi
-0000b650: 6f6e 2e53 6573 7369 6f6e 0a0a 2020 2020  on.Session..    
-0000b660: 6465 6620 6c6f 6767 6564 2820 6164 6d69  def logged( admi
-0000b670: 6e3d 4661 6c73 6520 293a 0a20 2020 2020  n=False ):.     
-0000b680: 2020 2022 2222 4368 6563 6b65 6420 7468     """Checked th
-0000b690: 6174 2074 6865 2073 6573 7369 6f6e 2773  at the session's
-0000b6a0: 2075 7365 7220 6973 206c 6f67 6765 6420   user is logged 
-0000b6b0: 696e 2e20 2045 7665 6e20 6966 2061 2075  in.  Even if a u
-0000b6c0: 7365 7220 6175 7468 656e 7469 6361 7465  ser authenticate
-0000b6d0: 732c 2074 6865 6972 2061 6363 6f75 6e74  s, their account
-0000b6e0: 0a20 2020 2020 2020 206d 6179 2062 6520  .        may be 
-0000b6f0: 6469 7361 626c 6564 2e0a 0a20 2020 2020  disabled...     
-0000b700: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
-0000b710: 6574 7572 6e20 7365 7373 696f 6e20 616e  eturn session an
-0000b720: 6420 7365 7373 696f 6e2e 6c6f 6769 6e20  d session.login 
-0000b730: 3e3d 2028 2032 2069 6620 6164 6d69 6e20  >= ( 2 if admin 
-0000b740: 656c 7365 2031 2029 0a0a 2020 2020 6465  else 1 )..    de
-0000b750: 6620 7072 6f78 7928 2065 6e76 2029 3a0a  f proxy( env ):.
-0000b760: 2020 2020 2020 2020 2222 2244 6574 6563          """Detec
-0000b770: 7473 2069 6620 7765 2061 7265 2062 6568  ts if we are beh
-0000b780: 696e 6420 6120 7072 6f78 792c 2061 6e64  ind a proxy, and
-0000b790: 2063 7265 6174 6573 2063 6f72 7265 6374   creates correct
-0000b7a0: 2070 6174 6820 6966 0a20 2020 2020 2020   path if.       
-0000b7b0: 206e 6563 6573 7361 7279 2c20 746f 2075   necessary, to u
-0000b7c0: 7365 2074 6865 206f 7269 6769 6e61 6c20  se the original 
-0000b7d0: 666f 7277 6172 6465 6420 686f 7374 2e0a  forwarded host..
-0000b7e0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000b7f0: 2020 2020 2070 726f 7879 0909 093d 2065       proxy...= e
-0000b800: 6e76 2e67 6574 2820 2248 5454 505f 585f  nv.get( "HTTP_X_
-0000b810: 464f 5257 4152 4445 445f 484f 5354 222c  FORWARDED_HOST",
-0000b820: 2022 2220 290a 2020 2020 2020 2020 6966   "" ).        if
-0000b830: 2070 726f 7879 3a0a 2020 2020 2020 2020   proxy:.        
-0000b840: 2020 2020 7072 6f78 7909 093d 2022 6874      proxy..= "ht
-0000b850: 7470 3a2f 2f22 202b 2070 726f 7879 0a20  tp://" + proxy. 
-0000b860: 2020 2020 2020 2072 6574 7572 6e20 7072         return pr
-0000b870: 6f78 790a 0a20 2020 2075 726c 7309 0909  oxy..    urls...
-0000b880: 3d20 280a 2020 2020 2020 2020 222f 222c  = (.        "/",
-0000b890: 0909 0909 2269 6e64 6578 222c 0a20 2020  ...."index",.   
-0000b8a0: 2020 2020 2072 222f 696e 6465 7828 5c2e       r"/index(\.
-0000b8b0: 6874 6d6c 293f 222c 0909 2269 6e64 6578  html)?",.."index
-0000b8c0: 222c 0a20 2020 2020 2020 2022 2f28 2e2a  ",.        "/(.*
-0000b8d0: 292f 222c 0909 0922 7472 6169 6c69 6e67  )/",..."trailing
-0000b8e0: 5f73 7475 6666 222c 0a20 2020 2020 2020  _stuff",.       
-0000b8f0: 2072 222f 282e 2a29 5c2e 6874 6d6c 222c   r"/(.*)\.html",
-0000b900: 0909 0922 7472 6169 6c69 6e67 5f73 7475  ..."trailing_stu
-0000b910: 6666 222c 0a20 2020 2020 2020 2022 2f66  ff",.        "/f
-0000b920: 6176 6963 6f6e 2e69 636f 222c 0909 0922  avicon.ico",..."
-0000b930: 6661 7669 636f 6e22 2c0a 2020 2020 2020  favicon",.      
-0000b940: 2020 222f 726f 626f 7473 2e74 7874 222c    "/robots.txt",
-0000b950: 0909 0922 726f 626f 7473 222c 0a20 2020  ..."robots",.   
-0000b960: 2020 2020 2022 2f6c 6f67 696e 222c 0909       "/login",..
-0000b970: 0922 6c6f 6769 6e22 2c0a 2020 2020 2020  ."login",.      
-0000b980: 2020 222f 6c6f 676f 7574 222c 0909 0922    "/logout",..."
-0000b990: 6c6f 676f 7574 222c 0a20 2020 2020 2020  logout",.       
-0000b9a0: 2072 222f 6170 692f 6973 7375 6528 5c2e   r"/api/issue(\.
-0000b9b0: 6a73 6f6e 293f 222c 0909 2261 7069 5f69  json)?",.."api_i
-0000b9c0: 7373 7565 222c 0909 2320 7061 7468 3a20  ssue",..# path: 
-0000b9d0: 2222 2c20 222e 6a73 6f6e 220a 2020 2020  "", ".json".    
-0000b9e0: 2020 2020 222f 6170 692f 6973 7375 652f      "/api/issue/
-0000b9f0: 282e 2b29 3f22 2c09 0922 6170 695f 6973  (.+)?",.."api_is
-0000ba00: 7375 6522 2c09 0923 2070 6174 683a 2022  sue",..# path: "
-0000ba10: 2e2e 2e22 2c20 222e 2e2e 2e6a 736f 6e22  ...", "....json"
-0000ba20: 0a20 2020 2020 2020 2072 222f 6170 692f  .        r"/api/
-0000ba30: 6c69 6365 6e73 6573 285c 2e6a 736f 6e29  licenses(\.json)
-0000ba40: 3f22 2c09 2261 7069 5f6c 6963 656e 7365  ?",."api_license
-0000ba50: 7322 2c0a 2020 2020 2020 2020 222f 6170  s",.        "/ap
-0000ba60: 692f 6c69 6365 6e73 6573 2f28 2e2b 293f  i/licenses/(.+)?
-0000ba70: 222c 0909 2261 7069 5f6c 6963 656e 7365  ",.."api_license
-0000ba80: 7322 2c0a 2020 2020 2020 2020 7222 2f61  s",.        r"/a
-0000ba90: 7069 2f63 7265 6465 6e74 6961 6c73 285c  pi/credentials(\
-0000baa0: 2e6a 736f 6e29 3f22 2c09 2261 7069 5f63  .json)?",."api_c
-0000bab0: 7265 6465 6e74 6961 6c73 222c 0a20 2020  redentials",.   
-0000bac0: 2020 2020 2022 2f61 7069 2f63 7265 6465       "/api/crede
-0000bad0: 6e74 6961 6c73 2f28 2e2b 293f 222c 0922  ntials/(.+)?",."
-0000bae0: 6170 695f 6372 6564 656e 7469 616c 7322  api_credentials"
-0000baf0: 2c0a 2020 2020 2020 2020 7222 2f61 7069  ,.        r"/api
-0000bb00: 2f6b 6579 7061 6972 7328 5c2e 6a73 6f6e  /keypairs(\.json
-0000bb10: 293f 222c 0922 6170 695f 6b65 7970 6169  )?",."api_keypai
-0000bb20: 7273 222c 0a20 2020 2020 2020 2022 2f61  rs",.        "/a
-0000bb30: 7069 2f6b 6579 7061 6972 732f 282e 2b29  pi/keypairs/(.+)
-0000bb40: 3f22 2c09 0922 6170 695f 6b65 7970 6169  ?",.."api_keypai
-0000bb50: 7273 222c 0a20 2020 2029 0a0a 2020 2020  rs",.    )..    
-0000bb60: 636c 6173 7320 7472 6169 6c69 6e67 5f73  class trailing_s
-0000bb70: 7475 6666 3a0a 2020 2020 2020 2020 6465  tuff:.        de
-0000bb80: 6620 4745 5428 2073 656c 662c 2070 6174  f GET( self, pat
-0000bb90: 6820 293a 0a20 2020 2020 2020 2020 2020  h ):.           
-0000bba0: 2077 6562 2e73 6565 6f74 6865 7228 2070   web.seeother( p
-0000bbb0: 726f 7879 2820 7765 622e 6374 782e 656e  roxy( web.ctx.en
-0000bbc0: 7669 726f 6e20 2920 2b20 272f 2720 2b20  viron ) + '/' + 
-0000bbd0: 7061 7468 2029 0a0a 2020 2020 636c 6173  path )..    clas
-0000bbe0: 7320 6661 7669 636f 6e3a 0a20 2020 2020  s favicon:.     
-0000bbf0: 2020 2064 6566 2047 4554 2820 7365 6c66     def GET( self
-0000bc00: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
-0000bc10: 2222 2241 6c77 6179 7320 7065 726d 616e  """Always perman
-0000bc20: 656e 746c 7920 7265 6469 7265 6374 2066  ently redirect f
-0000bc30: 6176 6963 6f6e 2e69 636f 2072 6571 7565  avicon.ico reque
-0000bc40: 7374 7320 746f 206f 7572 2066 6176 6963  sts to our favic
-0000bc50: 6f6e 2e70 6e67 2e0a 2020 2020 2020 2020  on.png..        
-0000bc60: 2020 2020 5468 6520 7265 6173 6f6e 2077      The reason w
-0000bc70: 6520 646f 2074 6869 7320 696e 7374 6561  e do this instea
-0000bc80: 6420 6f66 2070 7574 7469 6e67 2061 203c  d of putting a <
-0000bc90: 6c69 6e6b 2022 6963 6f6e 222e 2e2e 3e20  link "icon"...> 
-0000bca0: 6973 2062 6563 6175 7365 0a20 2020 2020  is because.     
-0000bcb0: 2020 2020 2020 2061 6c6c 202a 6f74 6865         all *othe
-0000bcc0: 722a 2072 6571 7565 7374 7320 6672 6f6d  r* requests from
-0000bcd0: 2062 726f 7773 6572 7320 2869 652e 2061   browsers (ie. a
-0000bce0: 7069 2f2e 2e2e 2029 2072 6574 7572 6e69  pi/... ) returni
-0000bcf0: 6e67 206e 6f6e 2d48 544d 4c0a 2020 2020  ng non-HTML.    
-0000bd00: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
-0000bd10: 2043 6f6e 7465 6e74 2d54 7970 6573 2073   Content-Types s
-0000bd20: 7563 6820 6173 2061 7070 6c69 6361 7469  uch as applicati
-0000bd30: 6f6e 2f6a 736f 6e20 2a61 6c73 6f2a 2072  on/json *also* r
-0000bd40: 6571 7565 7374 0a20 2020 2020 2020 2020  equest.         
-0000bd50: 2020 2066 6176 6963 6f6e 2e69 636f 2c20     favicon.ico, 
-0000bd60: 616e 6420 7765 2064 6f6e 2774 2068 6176  and we don't hav
-0000bd70: 6520 616e 2048 544d 4c20 3c68 6561 643e  e an HTML <head>
-0000bd80: 2074 6f20 7370 6563 6966 7920 616e 7920   to specify any 
-0000bd90: 6963 6f6e 206c 696e 6b2e 0a20 2020 2020  icon link..     
-0000bda0: 2020 2020 2020 2046 7572 7468 6572 6d6f         Furthermo
-0000bdb0: 7265 2c20 7468 6579 2063 6f6e 7469 6e75  re, they continu
-0000bdc0: 6520 746f 2072 6571 7565 7374 2069 7420  e to request it 
-0000bdd0: 2774 696c 2073 6174 6973 6669 6564 2c20  'til satisfied, 
-0000bde0: 736f 2077 6520 646f 2061 2033 3031 0a20  so we do a 301. 
-0000bdf0: 2020 2020 2020 2020 2020 2050 6572 6d61             Perma
-0000be00: 6e65 6e74 2052 6564 6972 6563 7420 746f  nent Redirect to
-0000be10: 2073 6174 6973 6679 2074 6865 2062 726f   satisfy the bro
-0000be20: 7773 6572 2061 6e64 2070 7265 7665 6e74  wser and prevent
-0000be30: 2066 7574 7572 6520 7265 7175 6573 7473   future requests
-0000be40: 2e0a 2020 2020 2020 2020 2020 2020 536f  ..            So
-0000be50: 2c20 7468 6973 2069 7320 7468 6520 6d6f  , this is the mo
-0000be60: 7374 2067 656e 6572 616c 2077 6179 2074  st general way t
-0000be70: 6f20 6861 6e64 6c65 2074 6865 2066 6176  o handle the fav
-0000be80: 6963 6f6e 2e69 636f 2222 220a 2020 2020  icon.ico""".    
-0000be90: 2020 2020 2020 2020 7765 622e 7265 6469          web.redi
-0000bea0: 7265 6374 2820 272f 7374 6174 6963 2f69  rect( '/static/i
-0000beb0: 6d61 6765 732f 6661 7669 636f 6e2e 6963  mages/favicon.ic
-0000bec0: 6f27 2029 0a0a 2020 2020 636c 6173 7320  o' )..    class 
-0000bed0: 726f 626f 7473 3a0a 2020 2020 2020 2020  robots:.        
-0000bee0: 6465 6620 4745 5428 2073 656c 6620 293a  def GET( self ):
-0000bef0: 0a20 2020 2020 2020 2020 2020 2077 6562  .            web
-0000bf00: 2e68 6561 6465 7228 2022 436f 6e74 656e  .header( "Conten
-0000bf10: 742d 5479 7065 222c 2022 7465 7874 2f70  t-Type", "text/p
-0000bf20: 6c61 696e 2220 290a 2020 2020 2020 2020  lain" ).        
-0000bf30: 2020 2020 7265 7475 726e 2022 2222 5c0a      return """\.
-0000bf40: 5573 6572 2d61 6765 6e74 3a20 2a0a 4469  User-agent: *.Di
-0000bf50: 7361 6c6c 6f77 3a20 2f0a 2222 220a 0a20  sallow: /.""".. 
-0000bf60: 2020 2063 6c61 7373 2069 6e64 6578 3a0a     class index:.
-0000bf70: 2020 2020 2020 2020 6465 6620 4745 5428          def GET(
-0000bf80: 2073 656c 662c 2070 6174 683d 4e6f 6e65   self, path=None
-0000bf90: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
-0000bfa0: 7265 6e64 6572 0909 3d20 7765 622e 7465  render..= web.te
-0000bfb0: 6d70 6c61 7465 2e72 656e 6465 7228 0a20  mplate.render(. 
-0000bfc0: 2020 2020 2020 2020 2020 2020 2020 2054                 T
-0000bfd0: 504c 5041 5448 2c20 6261 7365 3d22 6c61  PLPATH, base="la
-0000bfe0: 796f 7574 222c 2067 6c6f 6261 6c73 3d7b  yout", globals={
-0000bff0: 2769 6e6c 696e 6527 3a20 696e 6c69 6e65  'inline': inline
-0000c000: 2c20 2773 6573 7369 6f6e 273a 2073 6573  , 'session': ses
-0000c010: 7369 6f6e 7d20 290a 2020 2020 2020 2020  sion} ).        
-0000c020: 2020 2020 7265 7370 6f6e 7365 0909 3d20      response..= 
-0000c030: 7265 6e64 6572 2e69 6e64 6578 2820 7b0a  render.index( {.
-0000c040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c050: 2274 6974 6c65 223a 2009 224c 6963 656e  "title": ."Licen
-0000c060: 7369 6e67 222c 0a20 2020 2020 2020 2020  sing",.         
-0000c070: 2020 2020 2020 2022 7465 7874 223a 0909         "text":..
-0000c080: 2248 656c 6c6f 2c20 776f 726c 6421 222c  "Hello, world!",
-0000c090: 0a20 2020 2020 2020 2020 2020 207d 2029  .            } )
-0000c0a0: 0a20 2020 2020 2020 2020 2020 2077 6562  .            web
-0000c0b0: 2e68 6561 6465 7228 2022 436f 6e74 656e  .header( "Conten
-0000c0c0: 742d 5479 7065 222c 2022 7465 7874 2f68  t-Type", "text/h
-0000c0d0: 746d 6c22 2029 0a20 2020 2020 2020 2020  tml" ).         
-0000c0e0: 2020 2072 6574 7572 6e20 7265 7370 6f6e     return respon
-0000c0f0: 7365 0a0a 2020 2020 636c 6173 7320 6c6f  se..    class lo
-0000c100: 676f 7574 3a0a 2020 2020 2020 2020 6465  gout:.        de
-0000c110: 6620 4745 5428 2073 656c 6620 293a 0a20  f GET( self ):. 
-0000c120: 2020 2020 2020 2020 2020 2073 6573 7369             sessi
-0000c130: 6f6e 2e6c 6f67 696e 093d 2030 0a20 2020  on.login.= 0.   
-0000c140: 2020 2020 2020 2020 2077 6562 2e73 6565           web.see
-0000c150: 6f74 6865 7228 2070 726f 7879 2820 7765  other( proxy( we
-0000c160: 622e 6374 782e 656e 7669 726f 6e20 2920  b.ctx.environ ) 
-0000c170: 2b20 272f 6c6f 6769 6e27 2029 0a0a 2020  + '/login' )..  
-0000c180: 2020 6465 6620 7573 6572 5f68 6572 6974    def user_herit
-0000c190: 6167 6528 2075 7365 725f 6964 2029 3a0a  age( user_id ):.
-0000c1a0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000c1b0: 2020 2020 5265 7475 726e 2061 2064 6963      Return a dic
-0000c1c0: 7420 636f 6e74 6169 6e69 6e67 2074 6865  t containing the
-0000c1d0: 2068 6569 7261 7263 6879 206f 6620 7573   heirarchy of us
-0000c1e0: 6572 206e 616d 6573 2063 7265 6174 6564  er names created
-0000c1f0: 2062 7920 7468 6520 7370 6563 6966 6965   by the specifie
-0000c200: 6420 7573 6572 2e0a 2020 2020 2020 2020  d user..        
-0000c210: 2222 220a 2020 2020 2020 2020 7265 7375  """.        resu
-0000c220: 6c74 0909 093d 207b 7d0a 0a20 2020 2020  lt...= {}..     
-0000c230: 2020 2073 7061 776e 0909 093d 2064 622e     spawn...= db.
-0000c240: 7365 6c65 6374 2820 2775 7365 7273 272c  select( 'users',
-0000c250: 2077 6865 7265 3d27 6372 6561 746f 7220   where='creator 
-0000c260: 3d20 2475 7365 725f 6964 272c 2076 6172  = $user_id', var
-0000c270: 733d 7b20 2275 7365 725f 6964 223a 2075  s={ "user_id": u
-0000c280: 7365 725f 6964 207d 290a 2020 2020 2020  ser_id }).      
-0000c290: 2020 666f 7220 6368 696c 6420 696e 2073    for child in s
-0000c2a0: 7061 776e 3a0a 2020 2020 2020 2020 2020  pawn:.          
-0000c2b0: 2020 6966 2063 6869 6c64 2e75 7365 725f    if child.user_
-0000c2c0: 6964 203d 3d20 7573 6572 5f69 643a 0a20  id == user_id:. 
-0000c2d0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0000c2e0: 6f6e 7469 6e75 650a 0a20 2020 2020 2020  ontinue..       
-0000c2f0: 2020 2020 206b 6579 0909 093d 2028 6368       key...= (ch
-0000c300: 696c 642e 6e61 6d65 2c20 6368 696c 642e  ild.name, child.
-0000c310: 7573 6572 5f69 6429 0a20 2020 2020 2020  user_id).       
-0000c320: 2020 2020 2072 6573 756c 745b 6b65 795d       result[key]
-0000c330: 0909 3d20 7573 6572 5f68 6572 6974 6167  ..= user_heritag
-0000c340: 6528 2063 6869 6c64 2e75 7365 725f 6964  e( child.user_id
-0000c350: 2029 0a0a 2020 2020 2020 2020 7265 7475   )..        retu
-0000c360: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
-0000c370: 6566 2075 7365 725f 6865 7269 7461 6765  ef user_heritage
-0000c380: 5f70 7269 6e74 2820 682c 206c 6576 656c  _print( h, level
-0000c390: 3d30 2029 3a0a 2020 2020 2020 2020 6966  =0 ):.        if
-0000c3a0: 206e 6f74 2068 3a0a 2020 2020 2020 2020   not h:.        
-0000c3b0: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
-0000c3c0: 2020 2066 6f72 206b 6579 2069 6e20 683a     for key in h:
-0000c3d0: 0a20 2020 2020 2020 2020 2020 206e 616d  .            nam
-0000c3e0: 652c 7573 6572 5f69 6409 3d20 6b65 790a  e,user_id.= key.
-0000c3f0: 2020 2020 2020 2020 2020 2020 6c6f 672e              log.
-0000c400: 696e 666f 2822 2573 2025 7322 2025 2028  info("%s %s" % (
-0000c410: 2027 2027 2a6c 6576 656c 2c20 6e61 6d65   ' '*level, name
-0000c420: 2029 290a 2020 2020 2020 2020 2020 2020   )).            
-0000c430: 6966 2068 5b6b 6579 5d3a 0a20 2020 2020  if h[key]:.     
-0000c440: 2020 2020 2020 2020 2020 2075 7365 725f             user_
-0000c450: 6865 7269 7461 6765 5f70 7269 6e74 2820  heritage_print( 
-0000c460: 685b 6b65 795d 2c20 6c65 7665 6c2b 3120  h[key], level+1 
-0000c470: 290a 0a20 2020 2063 6c61 7373 206c 6f67  )..    class log
-0000c480: 696e 3a0a 2020 2020 2020 2020 2222 220a  in:.        """.
-0000c490: 2020 2020 2020 2020 5461 6b65 7320 616e          Takes an
-0000c4a0: 206f 7074 696f 6e61 6c20 3f72 6564 6972   optional ?redir
-0000c4b0: 6563 743d 7572 6c20 616e 6420 7061 7373  ect=url and pass
-0000c4c0: 6573 2069 7420 7669 6120 7468 6520 504f  es it via the PO
-0000c4d0: 5354 2e0a 2020 2020 2020 2020 2222 220a  ST..        """.
-0000c4e0: 2020 2020 2020 2020 6465 6620 4745 5428          def GET(
-0000c4f0: 2073 656c 6620 293a 0a20 2020 2020 2020   self ):.       
-0000c500: 2020 2020 2022 2222 416c 6c6f 7720 6c6f       """Allow lo
-0000c510: 6769 6e3b 2069 6620 7365 7373 696f 6e2e  gin; if session.
-0000c520: 6c6f 6769 6e20 616c 7265 6164 7920 7472  login already tr
-0000c530: 7565 2c20 7468 656e 2064 6973 706c 6179  ue, then display
-0000c540: 2050 494e 2063 6861 6e67 6520 6469 616c   PIN change dial
-0000c550: 6f67 2e22 2222 0a20 2020 2020 2020 2020  og.""".         
-0000c560: 2020 206c 6f67 2e69 6e66 6f28 2022 5365     log.info( "Se
-0000c570: 7373 696f 6e3a 2025 7222 2025 2028 2073  ssion: %r" % ( s
-0000c580: 6573 7369 6f6e 2e69 7465 6d73 2829 2029  ession.items() )
-0000c590: 290a 2020 2020 2020 2020 2020 2020 6368  ).            ch
-0000c5a0: 696c 6472 656e 0909 3d20 4e6f 6e65 0a20  ildren..= None. 
-0000c5b0: 2020 2020 2020 2020 2020 2069 6620 6c6f             if lo
-0000c5c0: 6767 6564 2829 3a0a 2020 2020 2020 2020  gged():.        
-0000c5d0: 2020 2020 2020 2020 6368 696c 6472 656e          children
-0000c5e0: 093d 2075 7365 725f 6865 7269 7461 6765  .= user_heritage
-0000c5f0: 2820 7365 7373 696f 6e2e 7573 6572 5f69  ( session.user_i
-0000c600: 6420 290a 2020 2020 2020 2020 2020 2020  d ).            
-0000c610: 2020 2020 7573 6572 5f68 6572 6974 6167      user_heritag
-0000c620: 655f 7072 696e 7428 2063 6869 6c64 7265  e_print( childre
-0000c630: 6e20 290a 0a20 2020 2020 2020 2020 2020  n )..           
-0000c640: 2072 656e 6465 7209 093d 2077 6562 2e74   render..= web.t
-0000c650: 656d 706c 6174 652e 7265 6e64 6572 280a  emplate.render(.
-0000c660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c670: 5450 4c50 4154 482c 2062 6173 653d 226c  TPLPATH, base="l
-0000c680: 6179 6f75 7422 2c20 676c 6f62 616c 733d  ayout", globals=
-0000c690: 7b27 696e 6c69 6e65 273a 2069 6e6c 696e  {'inline': inlin
-0000c6a0: 652c 2027 7365 7373 696f 6e27 3a20 7365  e, 'session': se
-0000c6b0: 7373 696f 6e7d 2029 0a20 2020 2020 2020  ssion} ).       
-0000c6c0: 2020 2020 2072 6573 706f 6e73 6509 093d       response..=
-0000c6d0: 2072 656e 6465 722e 6c6f 6769 6e28 0a20   render.login(. 
-0000c6e0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-0000c6f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c700: 2020 2020 2022 7469 746c 6522 3a09 2820       "title":.( 
-0000c710: 224c 6f67 696e 220a 2020 2020 2020 2020  "Login".        
-0000c720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c730: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-0000c740: 206c 6f67 6765 6428 2920 656c 7365 0a20   logged() else. 
-0000c750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c770: 2022 5765 6c63 6f6d 6520 2573 2220 2520   "Welcome %s" % 
-0000c780: 2820 7365 7373 696f 6e2e 6e61 6d65 2e63  ( session.name.c
-0000c790: 6170 6974 616c 697a 6528 2920 2929 2c0a  apitalize() )),.
-0000c7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c7b0: 2020 2020 2272 6564 6972 6563 7422 3a09      "redirect":.
-0000c7c0: 7765 622e 696e 7075 7428 292e 6765 7428  web.input().get(
-0000c7d0: 2022 7265 6469 7265 6374 222c 2022 2220   "redirect", "" 
-0000c7e0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-0000c7f0: 2020 2020 2020 2022 6368 696c 6472 656e         "children
-0000c800: 223a 2063 6869 6c64 7265 6e2c 0a20 2020  ": children,.   
-0000c810: 2020 2020 2020 2020 2020 2020 207d 290a               }).
-0000c820: 2020 2020 2020 2020 2020 2020 7765 622e              web.
-0000c830: 6865 6164 6572 2820 2243 6163 6865 2d43  header( "Cache-C
-0000c840: 6f6e 7472 6f6c 222c 2022 6e6f 2d63 6163  ontrol", "no-cac
-0000c850: 6865 2220 290a 2020 2020 2020 2020 2020  he" ).          
-0000c860: 2020 7765 622e 6865 6164 6572 2820 2243    web.header( "C
-0000c870: 6f6e 7465 6e74 2d54 7970 6522 2c20 2274  ontent-Type", "t
-0000c880: 6578 742f 6874 6d6c 2220 290a 2020 2020  ext/html" ).    
-0000c890: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-0000c8a0: 6573 706f 6e73 650a 0a20 2020 2020 2020  esponse..       
-0000c8b0: 2064 6566 2050 4f53 5428 2073 656c 6620   def POST( self 
-0000c8c0: 293a 0a20 2020 2020 2020 2020 2020 2022  ):.            "
-0000c8d0: 2222 5573 6520 7468 6520 7072 6f76 6964  ""Use the provid
-0000c8e0: 6564 2050 494e 2074 6f20 6175 7468 656e  ed PIN to authen
-0000c8f0: 7469 6361 7465 2061 2075 7365 722c 2061  ticate a user, a
-0000c900: 6e64 2074 6865 6e20 7265 6d65 6d62 6572  nd then remember
-0000c910: 2074 6865 2063 7265 6465 6e74 6961 6c73   the credentials
-0000c920: 2069 6e20 7468 650a 2020 2020 2020 2020   in the.        
-0000c930: 2020 2020 7365 7373 696f 6e2e 2020 4966      session.  If
-0000c940: 2061 6c72 6561 6479 206c 6f67 6765 6420   already logged 
-0000c950: 696e 2c20 616e 6420 7468 6520 2770 696e  in, and the 'pin
-0000c960: 6e65 7727 2076 616c 7565 2061 6e64 2027  new' value and '
-0000c970: 6368 616e 6765 2720 6275 7474 6f6e 2077  change' button w
-0000c980: 6173 2073 7570 706c 6965 642c 0a20 2020  as supplied,.   
-0000c990: 2020 2020 2020 2020 2074 6865 6e20 6368           then ch
-0000c9a0: 616e 6765 2074 6865 2075 7365 7227 7320  ange the user's 
-0000c9b0: 5049 4e2e 0a0a 2020 2020 2020 2020 2020  PIN...          
-0000c9c0: 2020 2222 220a 2020 2020 2020 2020 2020    """.          
-0000c9d0: 2020 6c6f 672e 696e 666f 2820 2253 6573    log.info( "Ses
-0000c9e0: 7369 6f6e 3a20 2572 2c20 696e 7075 743a  sion: %r, input:
-0000c9f0: 2025 7222 2025 2028 2073 6573 7369 6f6e   %r" % ( session
-0000ca00: 2e69 7465 6d73 2829 2c20 7765 622e 696e  .items(), web.in
-0000ca10: 7075 7428 292e 6974 656d 7328 2920 2929  put().items() ))
-0000ca20: 0a20 2020 2020 2020 2020 2020 2072 656e  .            ren
-0000ca30: 6465 7209 093d 2077 6562 2e74 656d 706c  der..= web.templ
-0000ca40: 6174 652e 7265 6e64 6572 280a 2020 2020  ate.render(.    
-0000ca50: 2020 2020 2020 2020 2020 2020 5450 4c50              TPLP
-0000ca60: 4154 482c 2062 6173 653d 226c 6179 6f75  ATH, base="layou
-0000ca70: 7422 2c20 676c 6f62 616c 733d 7b27 696e  t", globals={'in
-0000ca80: 6c69 6e65 273a 2069 6e6c 696e 652c 2027  line': inline, '
-0000ca90: 7365 7373 696f 6e27 3a20 7365 7373 696f  session': sessio
-0000caa0: 6e7d 2029 0a0a 2020 2020 2020 2020 2020  n} )..          
-0000cab0: 2020 6966 2022 6164 6422 2069 6e20 7765    if "add" in we
-0000cac0: 622e 696e 7075 7428 293a 0a20 2020 2020  b.input():.     
-0000cad0: 2020 2020 2020 2020 2020 2023 2050 6f73             # Pos
-0000cae0: 7420 7669 6120 2261 6464 2220 6275 7474  t via "add" butt
-0000caf0: 6f6e 3b20 6164 6420 6120 6e65 7720 7573  on; add a new us
-0000cb00: 6572 2f50 494e 2077 2f20 6120 7365 6c65  er/PIN w/ a sele
-0000cb10: 6374 6564 2073 7562 7365 7420 6f66 2063  cted subset of c
-0000cb20: 7572 7265 6e74 2075 7365 7227 730a 2020  urrent user's.  
-0000cb30: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-0000cb40: 7a6f 6e65 732e 2020 5472 7920 7570 6461  zones.  Try upda
-0000cb50: 7465 2066 6972 7374 2028 6f66 2065 7869  te first (of exi
-0000cb60: 7374 696e 6720 7573 6572 2f50 494e 2069  sting user/PIN i
-0000cb70: 6e20 7468 6520 7365 7373 696f 6e20 7573  n the session us
-0000cb80: 6572 7320 6865 7269 7461 6765 292c 0a20  ers heritage),. 
-0000cb90: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0000cba0: 2074 6865 6e20 696e 7365 7274 2e0a 2020   then insert..  
-0000cbb0: 2020 2020 2020 2020 2020 2020 2020 6572                er
-0000cbc0: 726f 7209 093d 204e 6f6e 650a 2020 2020  ror..= None.    
-0000cbd0: 2020 2020 2020 2020 2020 2020 7472 793a              try:
-0000cbe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000cbf0: 2020 2020 2061 7373 6572 7420 6c6f 6767       assert logg
-0000cc00: 6564 2829 2c20 224e 6f74 206c 6f67 6765  ed(), "Not logge
-0000cc10: 6420 696e 220a 2020 2020 2020 2020 2020  d in".          
-0000cc20: 2020 2020 2020 2020 2020 6e61 6d65 093d            name.=
-0000cc30: 2077 6562 2e69 6e70 7574 2829 2e67 6574   web.input().get
-0000cc40: 2820 226e 616d 6522 2029 0a20 2020 2020  ( "name" ).     
-0000cc50: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-0000cc60: 7373 6572 7420 6e61 6d65 2c20 2245 6d70  ssert name, "Emp
-0000cc70: 7479 206e 616d 6522 0a20 2020 2020 2020  ty name".       
-0000cc80: 2020 2020 2020 2020 2020 2020 206c 6f67               log
-0000cc90: 696e 093d 2077 6562 2e69 6e70 7574 2829  in.= web.input()
-0000cca0: 2e67 6574 2820 226c 6f67 696e 222c 2031  .get( "login", 1
-0000ccb0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-0000ccc0: 2020 2020 2020 2061 7373 6572 7420 3020         assert 0 
-0000ccd0: 3c3d 2069 6e74 2820 6c6f 6769 6e20 2920  <= int( login ) 
-0000cce0: 3c3d 2032 2c20 2249 6e76 616c 6964 206c  <= 2, "Invalid l
-0000ccf0: 6f67 696e 2044 6973 6162 6c65 2830 292f  ogin Disable(0)/
-0000cd00: 4e6f 726d 616c 2831 292f 4164 6d69 6e28  Normal(1)/Admin(
-0000cd10: 3229 220a 2020 2020 2020 2020 2020 2020  2)".            
-0000cd20: 2020 2020 2020 2020 7069 6e09 093d 2077          pin..= w
-0000cd30: 6562 2e69 6e70 7574 2829 2e67 6574 2820  eb.input().get( 
-0000cd40: 2270 696e 2220 290a 0a20 2020 2020 2020  "pin" )..       
-0000cd50: 2020 2020 2020 2020 2020 2020 2075 7064               upd
-0000cd60: 6174 6509 3d20 4e6f 6e65 0a20 2020 2020  ate.= None.     
-0000cd70: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000cd80: 6620 6c6f 6767 6564 2820 6164 6d69 6e3d  f logged( admin=
-0000cd90: 5472 7565 2029 3a0a 2020 2020 2020 2020  True ):.        
+00008fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008fb0: 2020 2020 2020 2022 7465 7874 2f70 6c61         "text/pla
+00008fc0: 696e 2220 5d2c 0a20 2020 2020 2020 2020  in" ],.         
+00008fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ff0: 2020 2020 2020 2020 2020 656e 7669 726f            enviro
+00009000: 6e3d 656e 7669 726f 6e2c 2061 6363 6570  n=environ, accep
+00009010: 743d 6163 6365 7074 2029 0a20 2020 2072  t=accept ).    r
+00009020: 6573 706f 6e73 6509 0909 3d20 2222 0a0a  esponse...= ""..
+00009030: 2020 2020 7661 7269 6162 6c65 7309 0909      variables...
+00009040: 3d20 7175 6572 6965 7320 6f72 2070 6f73  = queries or pos
+00009050: 7465 6420 6f72 207b 7d0a 0a20 2020 2023  ted or {}..    #
+00009060: 2046 756c 6c20 7370 6563 6966 6963 6174   Full specificat
+00009070: 696f 6e73 206f 6620 6465 7369 7265 6420  ions of desired 
+00009080: 4c69 6365 6e73 652e 2020 4d75 7374 2069  License.  Must i
+00009090: 6e63 6c75 6465 2063 6c69 656e 745f 7075  nclude client_pu
+000090a0: 626b 6579 2e0a 2020 2020 636f 6e66 6972  bkey..    confir
+000090b0: 6d09 0909 3d20 6c69 6365 6e73 696e 672e  m...= licensing.
+000090c0: 696e 746f 5f62 6f6f 6c65 616e 2820 7661  into_boolean( va
+000090d0: 7269 6162 6c65 732e 6765 7428 2027 636f  riables.get( 'co
+000090e0: 6e66 6972 6d27 2c20 4661 6c73 6520 292c  nfirm', False ),
+000090f0: 2074 7275 7468 793d 2827 272c 2920 290a   truthy=('',) ).
+00009100: 2020 2020 6175 7468 6f72 0909 093d 2076      author...= v
+00009110: 6172 6961 626c 6573 2e67 6574 2820 2761  ariables.get( 'a
+00009120: 7574 686f 7227 2029 0a20 2020 2061 7574  uthor' ).    aut
+00009130: 686f 725f 7075 626b 6579 0909 3d20 7661  hor_pubkey..= va
+00009140: 7269 6162 6c65 732e 6765 7428 2027 6175  riables.get( 'au
+00009150: 7468 6f72 5f70 7562 6b65 7927 2029 0a20  thor_pubkey' ). 
+00009160: 2020 2070 726f 6475 6374 0909 093d 2076     product...= v
+00009170: 6172 6961 626c 6573 2e67 6574 2820 2770  ariables.get( 'p
+00009180: 726f 6475 6374 2720 290a 2020 2020 636c  roduct' ).    cl
+00009190: 6965 6e74 0909 093d 2076 6172 6961 626c  ient...= variabl
+000091a0: 6573 2e67 6574 2820 2763 6c69 656e 7427  es.get( 'client'
+000091b0: 2029 0a20 2020 2063 6c69 656e 745f 7075   ).    client_pu
+000091c0: 626b 6579 0909 3d20 7661 7269 6162 6c65  bkey..= variable
+000091d0: 732e 6765 7428 2027 636c 6965 6e74 5f70  s.get( 'client_p
+000091e0: 7562 6b65 7927 2029 0909 2320 4d75 7374  ubkey' )..# Must
+000091f0: 2073 6967 6e20 7468 6520 6973 7375 6520   sign the issue 
+00009200: 7265 7175 6573 740a 2020 2020 6d61 6368  request.    mach
+00009210: 696e 6509 0909 3d20 7661 7269 6162 6c65  ine...= variable
+00009220: 732e 6765 7428 2027 6d61 6368 696e 6527  s.get( 'machine'
+00009230: 2029 0a20 2020 2073 6967 6e61 7475 7265   ).    signature
+00009240: 0909 093d 2076 6172 6961 626c 6573 2e67  ...= variables.g
+00009250: 6574 2820 2773 6967 6e61 7475 7265 2720  et( 'signature' 
+00009260: 290a 2020 2020 6e75 6d62 6572 0909 093d  ).    number...=
+00009270: 2076 6172 6961 626c 6573 2e67 6574 2820   variables.get( 
+00009280: 276e 756d 6265 7227 2029 0909 0923 206f  'number' )...# o
+00009290: 7074 696f 6e61 6c20 636c 6965 6e74 2d73  ptional client-s
+000092a0: 7570 706c 6965 6420 7365 7269 616c 697a  upplied serializ
+000092b0: 6174 696f 6e0a 0a20 2020 2023 2054 4f44  ation..    # TOD
+000092c0: 4f3a 2076 6572 6966 7920 7468 6520 7369  O: verify the si
+000092d0: 676e 6174 7572 6520 6973 2074 6861 7420  gnature is that 
+000092e0: 6f66 2074 6865 206f 7269 6769 6e61 6c20  of the original 
+000092f0: 6361 6e6f 6e69 6361 6c69 7a65 642c 2073  canonicalized, s
+00009300: 6572 6961 6c69 7a65 6420 4973 7375 6552  erialized IssueR
+00009310: 6571 7565 7374 2070 6179 6c6f 6164 0a20  equest payload. 
+00009320: 2020 2023 0a20 2020 2023 2020 2020 202e     #.    #     .
+00009330: 2e2e 3f61 7574 686f 723d 426c 6168 2c25  ..?author=Blah,%
+00009340: 3230 496e 6326 636c 6965 6e74 5f70 7562  20Inc&client_pub
+00009350: 6b65 793d 2e2e 2e26 6d61 6368 696e 653d  key=...&machine=
+00009360: 3030 3031 3032 3033 2d2e 2e2e 3065 3066  00010203-...0e0f
+00009370: 2673 6967 6e61 7475 7265 3d39 4462 612e  &signature=9Dba.
+00009380: 2e2e 4367 3d3d 0a20 2020 2023 2020 2020  ..Cg==.    #    
+00009390: 2020 2020 205e 5e5e 5e5e 5e5e 5e5e 5e5e       ^^^^^^^^^^^
+000093a0: 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e  ^^^^^^^^^^^^^^^^
+000093b0: 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e  ^^^^^^^^^^^^^^^^
+000093c0: 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e  ^^^^^^^^^^^^^^^^
+000093d0: 5e5e 0a20 2020 2023 0a20 2020 2023 2057  ^^.    #.    # W
+000093e0: 6520 6d75 7374 2073 6572 6961 6c69 7a65  e must serialize
+000093f0: 2074 6865 2072 6571 7565 7374 2069 6e20   the request in 
+00009400: 6120 7374 616e 6461 7264 2077 6179 2069  a standard way i
+00009410: 6e20 7468 6520 7365 6e64 6572 2061 6e64  n the sender and
+00009420: 2074 6865 2072 6563 6569 7665 722c 2062   the receiver, b
+00009430: 6563 6175 7365 2074 6865 0a20 2020 2023  ecause the.    #
+00009440: 2064 6174 6120 6d61 7920 6265 2073 656e   data may be sen
+00009450: 7420 6173 2055 524c 2061 7267 756d 656e  t as URL argumen
+00009460: 7473 206f 7220 504f 5354 2068 6561 6465  ts or POST heade
+00009470: 7220 7661 7269 6162 6c65 732e 0a20 2020  r variables..   
+00009480: 2069 7373 7565 5f72 6571 7565 7374 0909   issue_request..
+00009490: 3d20 6c69 6365 6e73 696e 672e 4973 7375  = licensing.Issu
+000094a0: 6552 6571 7565 7374 280a 2020 2020 2020  eRequest(.      
+000094b0: 2020 6175 7468 6f72 3d61 7574 686f 722c    author=author,
+000094c0: 2061 7574 686f 725f 7075 626b 6579 3d61   author_pubkey=a
+000094d0: 7574 686f 725f 7075 626b 6579 2c20 7072  uthor_pubkey, pr
+000094e0: 6f64 7563 743d 7072 6f64 7563 742c 0a20  oduct=product,. 
+000094f0: 2020 2020 2020 2063 6c69 656e 743d 636c         client=cl
+00009500: 6965 6e74 2c20 636c 6965 6e74 5f70 7562  ient, client_pub
+00009510: 6b65 793d 636c 6965 6e74 5f70 7562 6b65  key=client_pubke
+00009520: 792c 206d 6163 6869 6e65 3d6d 6163 6869  y, machine=machi
+00009530: 6e65 2029 0a20 2020 206c 6f67 2e69 6e66  ne ).    log.inf
+00009540: 6f28 2022 4973 7375 6520 7265 7175 6573  o( "Issue reques
+00009550: 7420 6e75 6d62 6572 3d7b 6e75 6d62 6572  t number={number
+00009560: 7d3b 207b 7265 717d 2c20 772f 2073 6967  }; {req}, w/ sig
+00009570: 6e61 7475 7265 3a20 7b73 6967 2172 7d22  nature: {sig!r}"
+00009580: 2e66 6f72 6d61 7428 0a20 2020 2020 2020  .format(.       
+00009590: 206e 756d 6265 723d 6e75 6d62 6572 2c20   number=number, 
+000095a0: 7265 713d 7374 7228 2069 7373 7565 5f72  req=str( issue_r
+000095b0: 6571 7565 7374 2029 2c20 7369 673d 7369  equest ), sig=si
+000095c0: 676e 6174 7572 6520 2929 0a20 2020 2074  gnature )).    t
+000095d0: 7279 3a0a 2020 2020 2020 2020 6973 7375  ry:.        issu
+000095e0: 655f 7265 7175 6573 742e 7665 7269 6679  e_request.verify
+000095f0: 2820 7075 626b 6579 3d63 6c69 656e 745f  ( pubkey=client_
+00009600: 7075 626b 6579 2c20 7369 676e 6174 7572  pubkey, signatur
+00009610: 653d 7369 676e 6174 7572 6520 290a 2020  e=signature ).  
+00009620: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
+00009630: 6f6e 2061 7320 6578 633a 0a20 2020 2020  on as exc:.     
+00009640: 2020 2072 6169 7365 2068 7474 705f 6578     raise http_ex
+00009650: 6365 7074 696f 6e28 2066 7261 6d65 776f  ception( framewo
+00009660: 726b 2c20 3430 312c 2022 4564 3235 3531  rk, 401, "Ed2551
+00009670: 3920 5369 676e 6174 7572 6520 6f66 2072  9 Signature of r
+00009680: 6571 7565 7374 2069 7320 696e 636f 7272  equest is incorr
+00009690: 6563 743a 207b 6578 637d 222e 666f 726d  ect: {exc}".form
+000096a0: 6174 280a 2020 2020 2020 2020 2020 2020  at(.            
+000096b0: 6578 633d 6578 6320 2929 0a0a 2020 2020  exc=exc ))..    
+000096c0: 2320 5365 6520 6966 2074 6865 7265 2061  # See if there a
+000096d0: 7265 204c 6963 656e 7365 2873 2920 7468  re License(s) th
+000096e0: 6174 206d 6174 6368 2061 2063 6572 7461  at match a certa
+000096f0: 696e 2070 6f72 7469 6f6e 206f 6620 7468  in portion of th
+00009700: 6520 7265 7175 6972 656d 656e 7473 2e20  e requirements. 
+00009710: 2041 6e20 6578 6163 7420 6d61 7463 680a   An exact match.
+00009720: 2020 2020 2320 6361 6e20 6265 2064 6972      # can be dir
+00009730: 6563 746c 7920 7265 7475 726e 6564 2e20  ectly returned. 
+00009740: 2041 2070 6172 7469 616c 206d 6174 6368   A partial match
+00009750: 2063 616e 2062 6520 7375 622d 6c69 6365   can be sub-lice
+00009760: 6e73 6564 2e0a 2020 2020 736b 6970 5f74  nsed..    skip_t
+00009770: 6162 203d 207b 0a20 2020 2020 2020 2027  ab = {.        '
+00009780: 636c 6965 6e74 273a 096c 616d 6264 6120  client':.lambda 
+00009790: 6c69 633a 206c 6963 2e63 6c69 656e 7420  lic: lic.client 
+000097a0: 616e 6420 6973 7375 655f 7265 7175 6573  and issue_reques
+000097b0: 745b 2763 6c69 656e 7427 5d20 616e 6420  t['client'] and 
+000097c0: 6c69 632e 636c 6965 6e74 5b27 6e61 6d65  lic.client['name
+000097d0: 275d 2021 3d20 6973 7375 655f 7265 7175  '] != issue_requ
+000097e0: 6573 745b 2763 6c69 656e 7427 5d2c 0a20  est['client'],. 
+000097f0: 2020 2020 2020 2027 636c 6965 6e74 5f70         'client_p
+00009800: 7562 6b65 7927 3a6c 616d 6264 6120 6c69  ubkey':lambda li
+00009810: 633a 206c 6963 2e63 6c69 656e 7420 616e  c: lic.client an
+00009820: 6420 6973 7375 655f 7265 7175 6573 745b  d issue_request[
+00009830: 2763 6c69 656e 745f 7075 626b 6579 275d  'client_pubkey']
+00009840: 2061 6e64 206c 6963 2e63 6c69 656e 745b   and lic.client[
+00009850: 2770 7562 6b65 7927 5d20 213d 2069 7373  'pubkey'] != iss
+00009860: 7565 5f72 6571 7565 7374 5b27 636c 6965  ue_request['clie
+00009870: 6e74 5f70 7562 6b65 7927 5d2c 0a20 2020  nt_pubkey'],.   
+00009880: 2020 2020 2027 6175 7468 6f72 273a 096c       'author':.l
+00009890: 616d 6264 6120 6c69 633a 2069 7373 7565  ambda lic: issue
+000098a0: 5f72 6571 7565 7374 5b27 6175 7468 6f72  _request['author
+000098b0: 275d 2061 6e64 206c 6963 2e61 7574 686f  '] and lic.autho
+000098c0: 725b 276e 616d 6527 5d20 213d 2069 7373  r['name'] != iss
+000098d0: 7565 5f72 6571 7565 7374 5b27 6175 7468  ue_request['auth
+000098e0: 6f72 275d 2c0a 2020 2020 2020 2020 2761  or'],.        'a
+000098f0: 7574 686f 725f 7075 626b 6579 273a 6c61  uthor_pubkey':la
+00009900: 6d62 6461 206c 6963 3a20 6973 7375 655f  mbda lic: issue_
+00009910: 7265 7175 6573 745b 2761 7574 686f 725f  request['author_
+00009920: 7075 626b 6579 275d 2061 6e64 206c 6963  pubkey'] and lic
+00009930: 2e61 7574 686f 725b 2770 7562 6b65 7927  .author['pubkey'
+00009940: 5d20 213d 2069 7373 7565 5f72 6571 7565  ] != issue_reque
+00009950: 7374 5b27 6175 7468 6f72 5f70 7562 6b65  st['author_pubke
+00009960: 7927 5d2c 0a20 2020 2020 2020 2027 7072  y'],.        'pr
+00009970: 6f64 7563 7427 3a09 6c61 6d62 6461 206c  oduct':.lambda l
+00009980: 6963 3a20 6973 7375 655f 7265 7175 6573  ic: issue_reques
+00009990: 745b 2770 726f 6475 6374 275d 2061 6e64  t['product'] and
+000099a0: 206c 6963 2e61 7574 686f 725b 2770 726f   lic.author['pro
+000099b0: 6475 6374 275d 2021 3d20 6973 7375 655f  duct'] != issue_
+000099c0: 7265 7175 6573 745b 2770 726f 6475 6374  request['product
+000099d0: 275d 2c0a 2020 2020 2020 2020 276d 6163  '],.        'mac
+000099e0: 6869 6e65 273a 096c 616d 6264 6120 6c69  hine':.lambda li
+000099f0: 633a 2069 7373 7565 5f72 6571 7565 7374  c: issue_request
+00009a00: 5b27 6d61 6368 696e 6527 5d20 616e 6420  ['machine'] and 
+00009a10: 6c69 635b 276d 6163 6869 6e65 275d 2021  lic['machine'] !
+00009a20: 3d20 6973 7375 655f 7265 7175 6573 745b  = issue_request[
+00009a30: 276d 6163 6869 6e65 275d 2c0a 2020 2020  'machine'],.    
+00009a40: 7d0a 0a20 2020 2064 6566 2070 726f 765f  }..    def prov_
+00009a50: 746f 5f69 7373 7565 2829 3a0a 2020 2020  to_issue():.    
+00009a60: 2020 2020 2222 2250 726f 6475 6365 2061      """Produce a
+00009a70: 204c 6963 656e 7365 5369 676e 6564 2073   LicenseSigned s
+00009a80: 7569 7461 626c 6520 666f 7220 7468 6520  uitable for the 
+00009a90: 636c 6965 6e74 2074 6f20 7265 6365 6976  client to receiv
+00009aa0: 652c 2075 7365 2061 7320 6120 6465 7065  e, use as a depe
+00009ab0: 6e64 656e 6379 206f 6620 6120 6e65 770a  ndency of a new.
+00009ac0: 2020 2020 2020 2020 4c69 6365 6e73 6520          License 
+00009ad0: 7370 6563 6966 6963 2074 6f20 7468 6569  specific to thei
+00009ae0: 7220 6d61 6368 696e 652c 2061 6e64 2073  r machine, and s
+00009af0: 6967 6e20 616e 6420 696e 7374 616c 6c2e  ign and install.
+00009b00: 0a0a 2020 2020 2020 2020 5369 6e63 6520  ..        Since 
+00009b10: 7765 2073 6361 6e20 7468 6520 6461 7461  we scan the data
+00009b20: 6261 7365 2027 6c69 6365 6e73 6573 2720  base 'licenses' 
+00009b30: 7461 626c 652c 2064 6f20 736f 6d65 2063  table, do some c
+00009b40: 6f6d 7075 7461 7469 6f6e 7320 616e 6420  omputations and 
+00009b50: 7468 656e 2075 7064 6174 6520 7468 6520  then update the 
+00009b60: 7461 626c 652c 0a20 2020 2020 2020 2077  table,.        w
+00009b70: 6520 6e65 6564 2074 6f20 6462 5f6c 6f63  e need to db_loc
+00009b80: 6b20 6172 6f75 6e64 2074 6869 7320 656e  k around this en
+00009b90: 7469 7265 2070 726f 6365 7373 2c20 746f  tire process, to
+00009ba0: 2061 766f 6964 206d 756c 7469 706c 6520   avoid multiple 
+00009bb0: 7369 6d75 6c74 616e 656f 7573 2072 6571  simultaneous req
+00009bc0: 7565 7374 730a 2020 2020 2020 2020 6973  uests.        is
+00009bd0: 7375 696e 6720 7468 6520 7361 6d65 204c  suing the same L
+00009be0: 6963 656e 7365 2e20 2053 696e 6365 2077  icense.  Since w
+00009bf0: 6520 646f 206e 6f20 444b 494d 2063 6f6e  e do no DKIM con
+00009c00: 6669 726d 6174 696f 6e20 6f72 206f 7468  firmation or oth
+00009c10: 6572 206e 6574 776f 726b 2049 2f4f 2068  er network I/O h
+00009c20: 6572 6520 286f 6e6c 790a 2020 2020 2020  ere (only.      
+00009c30: 2020 6669 6c65 2072 6561 6469 6e67 292c    file reading),
+00009c40: 2069 7420 7368 6f75 6c64 2062 6520 7175   it should be qu
+00009c50: 6963 6b2e 0a0a 2020 2020 2020 2020 2222  ick...        ""
+00009c60: 220a 0a20 2020 2020 2020 2064 6566 206c  "..        def l
+00009c70: 6963 735f 6669 6c74 6572 6564 2820 2a6e  ics_filtered( *n
+00009c80: 616d 6573 2029 3a0a 2020 2020 2020 2020  ames ):.        
+00009c90: 2020 2020 2222 2253 6361 6e20 7468 6520      """Scan the 
+00009ca0: 6c6f 6164 6564 2f73 746f 7265 6420 4c69  loaded/stored Li
+00009cb0: 6365 6e73 6573 2066 6f72 2020 2222 220a  censes for  """.
+00009cc0: 2020 2020 2020 2020 2020 2020 7374 6f72              stor
+00009cd0: 6564 0909 093d 206c 6973 7428 2064 622e  ed...= list( db.
+00009ce0: 7365 6c65 6374 2820 276c 6963 656e 7365  select( 'license
+00009cf0: 7327 2029 290a 2020 2020 2020 2020 2020  s' )).          
+00009d00: 2020 666f 7220 7369 672c 206c 6963 2069    for sig, lic i
+00009d10: 6e20 6c69 6365 6e73 6573 2820 636f 6e66  n licenses( conf
+00009d20: 6972 6d3d 4661 6c73 652c 2073 746f 7265  irm=False, store
+00009d30: 643d 7374 6f72 6564 2029 3a0a 2020 2020  d=stored ):.    
+00009d40: 2020 2020 2020 2020 2020 2020 6c6f 672e              log.
+00009d50: 696e 666f 2820 2249 7373 7565 2072 6571  info( "Issue req
+00009d60: 7565 7374 206e 756d 6265 723d 7b6e 756d  uest number={num
+00009d70: 6265 727d 3b20 7b6e 616d 657d 2773 207b  ber}; {name}'s {
+00009d80: 7072 6f64 7563 747d 3a20 6d69 736d 6174  product}: mismat
+00009d90: 6368 6564 206b 6579 733a 207b 6b65 7973  ched keys: {keys
+00009da0: 7d22 2e66 6f72 6d61 7428 0a20 2020 2020  }".format(.     
+00009db0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00009dc0: 756d 6265 723d 6e75 6d62 6572 2c20 6e61  umber=number, na
+00009dd0: 6d65 3d6c 6963 2e61 7574 686f 725b 276e  me=lic.author['n
+00009de0: 616d 6527 5d2c 2070 726f 6475 6374 3d6c  ame'], product=l
+00009df0: 6963 2e61 7574 686f 725b 2770 726f 6475  ic.author['produ
+00009e00: 6374 275d 2c0a 2020 2020 2020 2020 2020  ct'],.          
+00009e10: 2020 2020 2020 2020 2020 6b65 7973 3d27            keys='
+00009e20: 2c20 272e 6a6f 696e 2820 6e20 666f 7220  , '.join( n for 
+00009e30: 6e20 696e 206e 616d 6573 2069 6620 736b  n in names if sk
+00009e40: 6970 5f74 6162 5b6e 5d28 206c 6963 2029  ip_tab[n]( lic )
+00009e50: 2029 2929 0a20 2020 2020 2020 2020 2020   ))).           
+00009e60: 2020 2020 2069 6620 616e 7928 2073 6b69       if any( ski
+00009e70: 705f 7461 625b 6e5d 2820 6c69 6320 2920  p_tab[n]( lic ) 
+00009e80: 666f 7220 6e20 696e 206e 616d 6573 2029  for n in names )
+00009e90: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00009ea0: 2020 2020 2020 636f 6e74 696e 7565 0a20        continue. 
+00009eb0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00009ec0: 6f67 2e69 6e66 6f28 2022 4973 7375 6520  og.info( "Issue 
+00009ed0: 7265 7175 6573 7420 6e75 6d62 6572 3d7b  request number={
+00009ee0: 6e75 6d62 6572 7d3b 207b 6e61 6d65 7d27  number}; {name}'
+00009ef0: 7320 7b70 726f 6475 6374 7d20 6163 6365  s {product} acce
+00009f00: 7074 6564 3a20 7b6c 6963 7d22 2e66 6f72  pted: {lic}".for
+00009f10: 6d61 7428 0a20 2020 2020 2020 2020 2020  mat(.           
+00009f20: 2020 2020 2020 2020 206e 756d 6265 723d           number=
+00009f30: 6e75 6d62 6572 2c20 6e61 6d65 3d6c 6963  number, name=lic
+00009f40: 2e61 7574 686f 725b 276e 616d 6527 5d2c  .author['name'],
+00009f50: 2070 726f 6475 6374 3d6c 6963 2e61 7574   product=lic.aut
+00009f60: 686f 725b 2770 726f 6475 6374 275d 2c20  hor['product'], 
+00009f70: 6c69 633d 6c69 6320 2929 0a20 2020 2020  lic=lic )).     
+00009f80: 2020 2020 2020 2020 2020 2079 6965 6c64             yield
+00009f90: 2073 6967 2c20 6c69 630a 0a20 2020 2020   sig, lic..     
+00009fa0: 2020 2023 2049 6465 616c 6c79 2c20 6576     # Ideally, ev
+00009fb0: 6572 7974 6869 6e67 206d 6174 6368 6573  erything matches
+00009fc0: 2065 7861 6374 6c79 206f 6e65 2073 7065   exactly one spe
+00009fd0: 6369 6669 6320 4c69 6365 6e73 6520 616c  cific License al
+00009fe0: 7265 6164 7920 6973 7375 6564 2074 6f20  ready issued to 
+00009ff0: 7468 6973 2043 6c69 656e 7420 666f 720a  this Client for.
+0000a000: 2020 2020 2020 2020 2320 7468 6973 206d          # this m
+0000a010: 6163 6869 6e65 2e20 2049 6620 7765 2776  achine.  If we'v
+0000a020: 6520 616c 7265 6164 7920 6973 7375 6564  e already issued
+0000a030: 2074 6865 204c 6963 656e 7365 2028 616e   the License (an
+0000a040: 6420 7065 7268 6170 7320 7468 6520 636c  d perhaps the cl
+0000a050: 6965 6e74 2066 6f72 676f 7420 746f 0a20  ient forgot to. 
+0000a060: 2020 2020 2020 2023 2069 6e73 7461 6c6c         # install
+0000a070: 2069 742c 206f 7220 7265 2d69 6e73 7461   it, or re-insta
+0000a080: 6c6c 6564 2074 6865 2073 6f66 7477 6172  lled the softwar
+0000a090: 6529 2c20 616e 6420 6e65 6564 7320 6974  e), and needs it
+0000a0a0: 2061 6761 696e 2e0a 2020 2020 2020 2020   again..        
+0000a0b0: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+0000a0c0: 2028 7369 672c 206c 6963 292c 0909 3d20   (sig, lic),..= 
+0000a0d0: 6c69 6373 5f66 696c 7465 7265 6428 2027  lics_filtered( '
+0000a0e0: 6175 7468 6f72 272c 2027 6175 7468 6f72  author', 'author
+0000a0f0: 5f70 7562 6b65 7927 2c20 2770 726f 6475  _pubkey', 'produ
+0000a100: 6374 272c 2027 636c 6965 6e74 272c 2027  ct', 'client', '
+0000a110: 636c 6965 6e74 5f70 7562 6b65 7927 2c20  client_pubkey', 
+0000a120: 276d 6163 6869 6e65 2720 290a 2020 2020  'machine' ).    
+0000a130: 2020 2020 6578 6365 7074 2056 616c 7565      except Value
+0000a140: 4572 726f 7220 6173 2065 7863 3a0a 2020  Error as exc:.  
+0000a150: 2020 2020 2020 2020 2020 6c6f 672e 7761            log.wa
+0000a160: 726e 696e 6728 2022 4661 696c 6564 3a20  rning( "Failed: 
+0000a170: 7b65 7863 7d22 2e66 6f72 6d61 7428 2065  {exc}".format( e
+0000a180: 7863 3d65 7863 2029 290a 2020 2020 2020  xc=exc )).      
+0000a190: 2020 2020 2020 7061 7373 0a20 2020 2020        pass.     
+0000a1a0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000a1b0: 2020 2020 2069 6620 6c69 632e 636c 6965       if lic.clie
+0000a1c0: 6e74 2061 6e64 206c 6963 2e6d 6163 6869  nt and lic.machi
+0000a1d0: 6e65 3a20 2023 2045 7861 6374 206d 6174  ne:  # Exact mat
+0000a1e0: 6368 2c20 7769 7468 2073 7065 6369 6669  ch, with specifi
+0000a1f0: 6320 636c 6965 6e74 2061 6e64 206d 6163  c client and mac
+0000a200: 6869 6e65 0a20 2020 2020 2020 2020 2020  hine.           
+0000a210: 2020 2020 206c 6f67 2e77 6172 6e69 6e67       log.warning
+0000a220: 2820 2249 7373 7565 2072 6571 7565 7374  ( "Issue request
+0000a230: 206e 756d 6265 723d 7b6e 756d 6265 727d   number={number}
+0000a240: 3b20 5265 6973 7375 696e 6720 6578 6973  ; Reissuing exis
+0000a250: 7469 6e67 204c 6963 656e 7365 3a20 7b6c  ting License: {l
+0000a260: 6963 7d22 2e66 6f72 6d61 7428 0a20 2020  ic}".format(.   
+0000a270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a280: 206e 756d 6265 723d 6e75 6d62 6572 2c20   number=number, 
+0000a290: 6c69 633d 6c69 6320 6966 206c 6f67 2e69  lic=lic if log.i
+0000a2a0: 7345 6e61 626c 6564 466f 7228 206c 6f67  sEnabledFor( log
+0000a2b0: 6769 6e67 2e49 4e46 4f20 2920 656c 7365  ging.INFO ) else
+0000a2c0: 206c 6963 656e 7369 6e67 2e69 6e74 6f5f   licensing.into_
+0000a2d0: 6236 3428 2073 6967 2029 2929 0a20 2020  b64( sig ))).   
+0000a2e0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+0000a2f0: 7572 6e20 6c69 6365 6e73 696e 672e 4c69  urn licensing.Li
+0000a300: 6365 6e73 6553 6967 6e65 6428 0a20 2020  censeSigned(.   
+0000a310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a320: 206c 6963 656e 7365 3d6c 6963 2c20 7369   license=lic, si
+0000a330: 676e 6174 7572 653d 7369 672c 2063 6f6e  gnature=sig, con
+0000a340: 6669 726d 3d46 616c 7365 2c20 6d61 6368  firm=False, mach
+0000a350: 696e 655f 6964 5f70 6174 683d 4661 6c73  ine_id_path=Fals
+0000a360: 6520 290a 0a20 2020 2020 2020 2023 204f  e )..        # O
+0000a370: 4b2c 206e 6f74 2061 6c72 6561 6479 2069  K, not already i
+0000a380: 7373 7565 642e 2020 4669 6e64 2061 204c  ssued.  Find a L
+0000a390: 6963 656e 7365 2074 6f20 7370 6563 6961  icense to specia
+0000a3a0: 6c69 7a65 2e20 2049 6620 6f6e 6520 6d61  lize.  If one ma
+0000a3b0: 7463 6865 7320 7468 6520 6175 7468 6f72  tches the author
+0000a3c0: 2061 6e64 0a20 2020 2020 2020 2023 2063   and.        # c
+0000a3d0: 6c69 656e 7420 286f 7220 7370 6563 6966  lient (or specif
+0000a3e0: 6965 7320 6e6f 2063 6c69 656e 7429 2061  ies no client) a
+0000a3f0: 6e64 2068 6173 206e 6f20 6d61 6368 696e  nd has no machin
+0000a400: 652c 2075 7365 2069 7420 746f 2061 7574  e, use it to aut
+0000a410: 686f 7220 6120 6e65 7720 4c69 6365 6e73  hor a new Licens
+0000a420: 652c 2073 696d 706c 790a 2020 2020 2020  e, simply.      
+0000a430: 2020 2320 7370 6563 6961 6c69 7a65 6420    # specialized 
+0000a440: 7769 7468 2074 6865 2063 6c69 656e 7420  with the client 
+0000a450: 616e 6420 6d61 6368 696e 6520 7370 6563  and machine spec
+0000a460: 6966 6965 642e 2020 5468 6520 636c 6965  ified.  The clie
+0000a470: 6e74 2077 696c 6c20 7265 6365 6976 6520  nt will receive 
+0000a480: 616e 640a 2020 2020 2020 2020 2320 7375  and.        # su
+0000a490: 622d 4c69 6365 6e73 6520 6974 2062 7920  b-License it by 
+0000a4a0: 6372 6561 7469 6e67 2061 206e 6577 204c  creating a new L
+0000a4b0: 6963 656e 7365 2077 6974 6820 7468 6973  icense with this
+0000a4c0: 2061 206f 6e65 206f 6620 6974 7320 6465   a one of its de
+0000a4d0: 7065 6e64 656e 6369 6573 2c20 7468 656e  pendencies, then
+0000a4e0: 2073 6967 6e20 6974 0a20 2020 2020 2020   sign it.       
+0000a4f0: 2023 2077 6974 6820 7468 6520 636c 6965   # with the clie
+0000a500: 6e74 2073 6967 6e69 6e67 206b 6579 2074  nt signing key t
+0000a510: 6865 7920 686f 6c64 2c20 616e 6420 696e  hey hold, and in
+0000a520: 7374 616c 6c20 6974 2e0a 2020 2020 2020  stall it..      
+0000a530: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+0000a540: 2020 2028 7369 672c 206c 6963 292c 0909     (sig, lic),..
+0000a550: 3d20 6c69 6373 5f66 696c 7465 7265 6428  = lics_filtered(
+0000a560: 2027 6175 7468 6f72 272c 2027 6175 7468   'author', 'auth
+0000a570: 6f72 5f70 7562 6b65 7927 2c20 2770 726f  or_pubkey', 'pro
+0000a580: 6475 6374 272c 2027 636c 6965 6e74 272c  duct', 'client',
+0000a590: 2027 636c 6965 6e74 5f70 7562 6b65 7927   'client_pubkey'
+0000a5a0: 2029 0a20 2020 2020 2020 2065 7863 6570   ).        excep
+0000a5b0: 7420 5661 6c75 6545 7272 6f72 2061 7320  t ValueError as 
+0000a5c0: 6578 633a 0a20 2020 2020 2020 2020 2020  exc:.           
+0000a5d0: 206c 6f67 2e77 6172 6e69 6e67 2820 2246   log.warning( "F
+0000a5e0: 6169 6c65 643a 207b 6578 637d 222e 666f  ailed: {exc}".fo
+0000a5f0: 726d 6174 2820 6578 633d 6578 6320 2929  rmat( exc=exc ))
+0000a600: 0a20 2020 2020 2020 2020 2020 2070 6173  .            pas
+0000a610: 730a 2020 2020 2020 2020 656c 7365 3a0a  s.        else:.
+0000a620: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+0000a630: 6f74 206c 6963 2e6d 6163 6869 6e65 206f  ot lic.machine o
+0000a640: 7220 6c69 635b 276d 6163 6869 6e65 275d  r lic['machine']
+0000a650: 203d 3d20 6973 7375 655f 7265 7175 6573   == issue_reques
+0000a660: 745b 276d 6163 6869 6e65 275d 3a0a 2020  t['machine']:.  
+0000a670: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+0000a680: 672e 696e 666f 2820 2249 7373 7565 2072  g.info( "Issue r
+0000a690: 6571 7565 7374 206e 756d 6265 723d 7b6e  equest number={n
+0000a6a0: 756d 6265 727d 3b20 5370 6563 6961 6c69  umber}; Speciali
+0000a6b0: 7a69 6e67 2065 7869 7374 696e 6720 4c69  zing existing Li
+0000a6c0: 6365 6e73 653a 207b 6c69 637d 222e 666f  cense: {lic}".fo
+0000a6d0: 726d 6174 280a 2020 2020 2020 2020 2020  rmat(.          
+0000a6e0: 2020 2020 2020 2020 2020 6e75 6d62 6572            number
+0000a6f0: 3d6e 756d 6265 722c 206c 6963 3d6c 6963  =number, lic=lic
+0000a700: 2069 6620 6c6f 672e 6973 456e 6162 6c65   if log.isEnable
+0000a710: 6446 6f72 2820 6c6f 6767 696e 672e 494e  dFor( logging.IN
+0000a720: 464f 2029 2065 6c73 6520 6c69 6365 6e73  FO ) else licens
+0000a730: 696e 672e 696e 746f 5f62 3634 2820 7369  ing.into_b64( si
+0000a740: 6729 2929 0a20 2020 2020 2020 2020 2020  g))).           
+0000a750: 2020 2020 2061 7574 686f 725f 7369 676b       author_sigk
+0000a760: 6579 093d 204e 6f6e 650a 2020 2020 2020  ey.= None.      
+0000a770: 2020 2020 2020 2020 2020 666f 7220 6e61            for na
+0000a780: 6d65 2c6b 6579 7061 6972 2c63 7265 6420  me,keypair,cred 
+0000a790: 696e 206b 6579 7061 6972 7328 293a 0a20  in keypairs():. 
+0000a7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a7b0: 2020 2076 6b2c 2073 6b09 3d20 6b65 7970     vk, sk.= keyp
+0000a7c0: 6169 722e 696e 746f 5f6b 6579 7061 6972  air.into_keypair
+0000a7d0: 2820 2a2a 6372 6564 2029 0a20 2020 2020  ( **cred ).     
+0000a7e0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0000a7f0: 7562 6b65 7909 3d20 6c69 6365 6e73 696e  ubkey.= licensin
+0000a800: 672e 696e 746f 5f62 3634 2820 766b 2029  g.into_b64( vk )
+0000a810: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a820: 2020 2020 2069 6620 6e61 6d65 203d 3d20       if name == 
+0000a830: 6c69 632e 6175 7468 6f72 5b27 6e61 6d65  lic.author['name
+0000a840: 275d 2061 6e64 2070 7562 6b65 7920 3d3d  '] and pubkey ==
+0000a850: 2069 7373 7565 5f72 6571 7565 7374 5b27   issue_request['
+0000a860: 6175 7468 6f72 5f70 7562 6b65 7927 5d3a  author_pubkey']:
+0000a870: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a880: 2020 2020 2020 2020 2061 7574 686f 725f           author_
+0000a890: 7369 676b 6579 203d 2073 6b0a 2020 2020  sigkey = sk.    
+0000a8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a8b0: 2020 2020 6272 6561 6b0a 2020 2020 2020      break.      
+0000a8c0: 2020 2020 2020 2020 2020 2320 4973 7375            # Issu
+0000a8d0: 6520 6120 6e65 7720 7370 6563 6961 6c69  e a new speciali
+0000a8e0: 7a65 6420 4c69 6365 6e73 6520 666f 7220  zed License for 
+0000a8f0: 436c 6965 6e74 2c20 7369 676e 6564 2077  Client, signed w
+0000a900: 6974 6820 4175 7468 6f72 2773 2070 7269  ith Author's pri
+0000a910: 7661 7465 2073 6967 6e69 6e67 206b 6579  vate signing key
+0000a920: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000a930: 2020 6966 206e 6f74 206c 6963 2e63 6c69    if not lic.cli
+0000a940: 656e 743a 0a20 2020 2020 2020 2020 2020  ent:.           
+0000a950: 2020 2020 2020 2020 206c 6963 2e63 6c69           lic.cli
+0000a960: 656e 7409 3d20 6c69 6365 6e73 696e 672e  ent.= licensing.
+0000a970: 4167 656e 7428 206e 616d 653d 6973 7375  Agent( name=issu
+0000a980: 655f 7265 7175 6573 745b 2763 6c69 656e  e_request['clien
+0000a990: 7427 5d2c 2070 7562 6b65 793d 6973 7375  t'], pubkey=issu
+0000a9a0: 655f 7265 7175 6573 745b 2763 6c69 656e  e_request['clien
+0000a9b0: 745f 7075 626b 6579 275d 2029 0a20 2020  t_pubkey'] ).   
+0000a9c0: 2020 2020 2020 2020 2020 2020 206c 6963               lic
+0000a9d0: 2e6d 6163 6869 6e65 093d 206c 6963 656e  .machine.= licen
+0000a9e0: 7369 6e67 2e69 6e74 6f5f 5555 4944 7634  sing.into_UUIDv4
+0000a9f0: 2820 6973 7375 655f 7265 7175 6573 745b  ( issue_request[
+0000aa00: 276d 6163 6869 6e65 275d 2029 0a20 2020  'machine'] ).   
+0000aa10: 2020 2020 2020 2020 2020 2020 2070 726f               pro
+0000aa20: 7609 093d 206c 6963 656e 7369 6e67 2e69  v..= licensing.i
+0000aa30: 7373 7565 280a 2020 2020 2020 2020 2020  ssue(.          
+0000aa40: 2020 2020 2020 2020 2020 6c69 6365 6e73            licens
+0000aa50: 653d 6c69 632c 2061 7574 686f 725f 7369  e=lic, author_si
+0000aa60: 676b 6579 3d61 7574 686f 725f 7369 676b  gkey=author_sigk
+0000aa70: 6579 2c20 636f 6e66 6972 6d3d 4661 6c73  ey, confirm=Fals
+0000aa80: 652c 206d 6163 6869 6e65 5f69 645f 7061  e, machine_id_pa
+0000aa90: 7468 3d46 616c 7365 2029 0a20 2020 2020  th=False ).     
+0000aaa0: 2020 2020 2020 2020 2020 2069 6e73 6572             inser
+0000aab0: 7420 3d20 6462 2e69 6e73 6572 7428 2027  t = db.insert( '
+0000aac0: 6c69 6365 6e73 6573 272c 0a20 2020 2020  licenses',.     
+0000aad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aae0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000aaf0: 6967 6e61 7475 7265 3d70 726f 765b 2773  ignature=prov['s
+0000ab00: 6967 6e61 7475 7265 275d 2c0a 2020 2020  ignature'],.    
+0000ab10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ab20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ab30: 6c69 6365 6e73 653d 7374 7228 2070 726f  license=str( pro
+0000ab40: 762e 6c69 6365 6e73 6520 2929 0a20 2020  v.license )).   
+0000ab50: 2020 2020 2020 2020 2020 2020 2061 7373               ass
+0000ab60: 6572 7420 696e 7365 7274 2c20 2253 7065  ert insert, "Spe
+0000ab70: 6369 616c 697a 696e 6720 6c69 6365 6e73  cializing licens
+0000ab80: 6520 696e 7365 7274 2066 6169 6c65 6422  e insert failed"
+0000ab90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000aba0: 206c 6f67 2e77 6172 6e69 6e67 2820 2249   log.warning( "I
+0000abb0: 7373 7565 2072 6571 7565 7374 206e 756d  ssue request num
+0000abc0: 6265 723d 7b6e 756d 6265 727d 3b20 4973  ber={number}; Is
+0000abd0: 7375 6564 2073 7065 6369 616c 697a 6564  sued specialized
+0000abe0: 204c 6963 656e 7365 3a20 7b6c 6963 7d22   License: {lic}"
+0000abf0: 2e66 6f72 6d61 7428 0a20 2020 2020 2020  .format(.       
+0000ac00: 2020 2020 2020 2020 2020 2020 206e 756d               num
+0000ac10: 6265 723d 6e75 6d62 6572 2c20 6c69 633d  ber=number, lic=
+0000ac20: 7072 6f76 2e6c 6963 656e 7365 2069 6620  prov.license if 
+0000ac30: 6c6f 672e 6973 456e 6162 6c65 6446 6f72  log.isEnabledFor
+0000ac40: 2820 6c6f 6767 696e 672e 494e 464f 2029  ( logging.INFO )
+0000ac50: 2065 6c73 6520 6c69 6365 6e73 696e 672e   else licensing.
+0000ac60: 696e 746f 5f62 3634 2820 7072 6f76 2e73  into_b64( prov.s
+0000ac70: 6967 6e61 7475 7265 2029 2929 0a20 2020  ignature ))).   
+0000ac80: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+0000ac90: 7572 6e20 7072 6f76 0a0a 2020 2020 2020  urn prov..      
+0000aca0: 2020 7261 6973 6520 6874 7470 5f65 7863    raise http_exc
+0000acb0: 6570 7469 6f6e 2820 6672 616d 6577 6f72  eption( framewor
+0000acc0: 6b2c 2034 3039 2c20 224e 6f20 6d61 7463  k, 409, "No matc
+0000acd0: 6869 6e67 204c 6963 656e 7365 7320 666f  hing Licenses fo
+0000ace0: 756e 6420 6d61 7463 6869 6e67 2072 6571  und matching req
+0000acf0: 7565 7374 3a20 7b7d 222e 666f 726d 6174  uest: {}".format
+0000ad00: 280a 2020 2020 2020 2020 2020 2020 6973  (.            is
+0000ad10: 7375 655f 7265 7175 6573 7420 2929 0a0a  sue_request ))..
+0000ad20: 2020 2020 7769 7468 2064 625f 6c6f 636b      with db_lock
+0000ad30: 3a0a 2020 2020 2020 2020 7072 6f76 0909  :.        prov..
+0000ad40: 093d 2070 726f 765f 746f 5f69 7373 7565  .= prov_to_issue
+0000ad50: 2829 0a20 2020 206c 6f67 2e69 6e66 6f28  ().    log.info(
+0000ad60: 2022 4973 7375 6520 7265 7175 6573 7420   "Issue request 
+0000ad70: 6e75 6d62 6572 3d7b 6e75 6d62 6572 7d3b  number={number};
+0000ad80: 2049 7373 7569 6e67 204c 6963 656e 7365   Issuing License
+0000ad90: 2066 6f72 207b 6e61 6d65 7d27 207b 7072   for {name}' {pr
+0000ada0: 6f64 7563 747d 222e 666f 726d 6174 280a  oduct}".format(.
+0000adb0: 2020 2020 2020 2020 6e75 6d62 6572 3d6e          number=n
+0000adc0: 756d 6265 722c 206e 616d 653d 7072 6f76  umber, name=prov
+0000add0: 2e6c 6963 656e 7365 2e61 7574 686f 725b  .license.author[
+0000ade0: 276e 616d 6527 5d2c 2070 726f 6475 6374  'name'], product
+0000adf0: 3d70 726f 762e 6c69 6365 6e73 652e 6175  =prov.license.au
+0000ae00: 7468 6f72 5b27 7072 6f64 7563 7427 5d20  thor['product'] 
+0000ae10: 2929 0a0a 2020 2020 6461 7461 0909 093d  ))..    data...=
+0000ae20: 207b 7d0a 2020 2020 6461 7461 5b22 7469   {}.    data["ti
+0000ae30: 746c 6522 5d09 093d 2070 6174 6820 6f72  tle"]..= path or
+0000ae40: 2022 4973 7375 6522 0a20 2020 2064 6174   "Issue".    dat
+0000ae50: 615b 2270 6174 6822 5d09 093d 2070 6174  a["path"]..= pat
+0000ae60: 680a 2020 2020 6461 7461 5b22 6c69 7374  h.    data["list
+0000ae70: 225d 203d 206c 6c09 093d 205b 5d0a 2020  "] = ll..= [].  
+0000ae80: 2020 6461 7461 5b22 6b65 7973 225d 0909    data["keys"]..
+0000ae90: 3d20 5b22 6175 7468 6f72 222c 2022 636c  = ["author", "cl
+0000aea0: 6965 6e74 222c 2022 7072 6f64 7563 7422  ient", "product"
+0000aeb0: 2c20 2273 6967 6e61 7475 7265 222c 2022  , "signature", "
+0000aec0: 636f 6e66 6972 6d22 2c20 226c 6963 656e  confirm", "licen
+0000aed0: 7365 225d 0a0a 2020 2020 7265 636f 7264  se"]..    record
+0000aee0: 0909 093d 2064 6963 7428 0a20 2020 2020  ...= dict(.     
+0000aef0: 2020 2061 7574 686f 7209 093d 2070 726f     author..= pro
+0000af00: 762e 6c69 6365 6e73 655b 2761 7574 686f  v.license['autho
+0000af10: 7227 5d5b 276e 616d 6527 5d2c 0a20 2020  r']['name'],.   
+0000af20: 2020 2020 2063 6c69 656e 7409 093d 2070       client..= p
+0000af30: 726f 762e 6c69 6365 6e73 655b 2763 6c69  rov.license['cli
+0000af40: 656e 7427 5d5b 276e 616d 6527 5d2c 0a20  ent']['name'],. 
+0000af50: 2020 2020 2020 2070 726f 6475 6374 0909         product..
+0000af60: 3d20 7072 6f76 2e6c 6963 656e 7365 5b27  = prov.license['
+0000af70: 6175 7468 6f72 275d 5b27 7072 6f64 7563  author']['produc
+0000af80: 7427 5d2c 0a20 2020 2020 2020 2073 6967  t'],.        sig
+0000af90: 6e61 7475 7265 093d 206c 6963 656e 7369  nature.= licensi
+0000afa0: 6e67 2e69 6e74 6f5f 6236 3428 2070 726f  ng.into_b64( pro
+0000afb0: 762e 7369 676e 6174 7572 6520 292c 0a20  v.signature ),. 
+0000afc0: 2020 2020 2020 2063 6f6e 6669 726d 0909         confirm..
+0000afd0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+0000afe0: 6c69 6365 6e73 6509 093d 2070 726f 762e  license..= prov.
+0000aff0: 6c69 6365 6e73 652c 0a20 2020 2029 0a20  license,.    ). 
+0000b000: 2020 2069 6620 636f 6e66 6972 6d3a 0a20     if confirm:. 
+0000b010: 2020 2020 2020 206c 6f67 2e77 6172 6e69         log.warni
+0000b020: 6e67 2820 2249 7373 7565 2072 6571 7565  ng( "Issue reque
+0000b030: 7374 206e 756d 6265 723d 7b6e 756d 6265  st number={numbe
+0000b040: 727d 3b20 436f 6e66 6972 6d69 6e67 2044  r}; Confirming D
+0000b050: 4b49 4d20 666f 7220 7b6e 616d 657d 2720  KIM for {name}' 
+0000b060: 7b70 726f 6475 6374 7d22 2e66 6f72 6d61  {product}".forma
+0000b070: 7428 0a20 2020 2020 2020 2020 2020 206e  t(.            n
+0000b080: 756d 6265 723d 6e75 6d62 6572 2c20 6e61  umber=number, na
+0000b090: 6d65 3d70 726f 762e 6c69 6365 6e73 652e  me=prov.license.
+0000b0a0: 6175 7468 6f72 5b27 6e61 6d65 275d 2c20  author['name'], 
+0000b0b0: 7072 6f64 7563 743d 7072 6f76 2e6c 6963  product=prov.lic
+0000b0c0: 656e 7365 2e61 7574 686f 725b 2770 726f  ense.author['pro
+0000b0d0: 6475 6374 275d 2029 290a 2020 2020 2020  duct'] )).      
+0000b0e0: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+0000b0f0: 2020 206c 6963 656e 7369 6e67 2e76 6572     licensing.ver
+0000b100: 6966 7928 2070 726f 762c 2063 6f6e 6669  ify( prov, confi
+0000b110: 726d 3d63 6f6e 6669 726d 2c20 6d61 6368  rm=confirm, mach
+0000b120: 696e 655f 6964 5f70 6174 683d 4661 6c73  ine_id_path=Fals
+0000b130: 6520 290a 2020 2020 2020 2020 6578 6365  e ).        exce
+0000b140: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
+0000b150: 6578 633a 0a20 2020 2020 2020 2020 2020  exc:.           
+0000b160: 2072 6563 6f72 642e 7570 6461 7465 2820   record.update( 
+0000b170: 636f 6e66 6972 6d3d 7374 7228 2065 7863  confirm=str( exc
+0000b180: 2029 290a 2020 2020 2020 2020 656c 7365   )).        else
+0000b190: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0000b1a0: 636f 7264 2e75 7064 6174 6528 2063 6f6e  cord.update( con
+0000b1b0: 6669 726d 3d54 7275 6520 290a 2020 2020  firm=True ).    
+0000b1c0: 6c6c 2e61 7070 656e 6428 2072 6563 6f72  ll.append( recor
+0000b1d0: 6420 290a 0a20 2020 2069 6620 636f 6e74  d )..    if cont
+0000b1e0: 656e 7420 616e 6420 636f 6e74 656e 7420  ent and content 
+0000b1f0: 696e 2028 2022 6170 706c 6963 6174 696f  in ( "applicatio
+0000b200: 6e2f 6a73 6f6e 222c 2022 7465 7874 2f6a  n/json", "text/j
+0000b210: 6176 6173 6372 6970 7422 2c20 2274 6578  avascript", "tex
+0000b220: 742f 706c 6169 6e22 2029 3a0a 2020 2020  t/plain" ):.    
+0000b230: 2020 2020 6361 6c6c 6261 636b 0909 3d20      callback..= 
+0000b240: 7661 7269 6162 6c65 732e 6765 7428 2027  variables.get( '
+0000b250: 6361 6c6c 6261 636b 272c 2022 2220 290a  callback', "" ).
+0000b260: 2020 2020 2020 2020 6966 2063 616c 6c62          if callb
+0000b270: 6163 6b3a 0a20 2020 2020 2020 2020 2020  ack:.           
+0000b280: 2072 6573 706f 6e73 6520 2020 2020 2020   response       
+0000b290: 2020 2020 2b3d 2063 616c 6c62 6163 6b20      += callback 
+0000b2a0: 2b20 2228 2022 0a20 2020 2020 2020 2072  + "( ".        r
+0000b2b0: 6573 706f 6e73 6520 2020 2020 2020 2020  esponse         
+0000b2c0: 2020 2020 2020 2b3d 206c 6963 656e 7369        += licensi
+0000b2d0: 6e67 2e69 6e74 6f5f 4a53 4f4e 2820 6461  ng.into_JSON( da
+0000b2e0: 7461 2c20 696e 6465 6e74 3d34 2029 0a20  ta, indent=4 ). 
+0000b2f0: 2020 2020 2020 2069 6620 6361 6c6c 6261         if callba
+0000b300: 636b 3a0a 2020 2020 2020 2020 2020 2020  ck:.            
+0000b310: 7265 7370 6f6e 7365 2020 2020 2020 2020  response        
+0000b320: 2020 202b 3d20 2220 2922 0a20 2020 2065     += " )".    e
+0000b330: 6c69 6620 636f 6e74 656e 7420 616e 6420  lif content and 
+0000b340: 636f 6e74 656e 7420 696e 2028 2022 7465  content in ( "te
+0000b350: 7874 2f68 746d 6c22 2029 3a0a 2020 2020  xt/html" ):.    
+0000b360: 2020 2020 7265 7370 6f6e 7365 0909 3d20      response..= 
+0000b370: 7265 6e64 6572 2e6b 6579 6c69 7374 2820  render.keylist( 
+0000b380: 6461 7461 2029 0a20 2020 2065 6c73 653a  data ).    else:
+0000b390: 0a20 2020 2020 2020 2072 6169 7365 2068  .        raise h
+0000b3a0: 7474 705f 6578 6365 7074 696f 6e28 2066  ttp_exception( f
+0000b3b0: 7261 6d65 776f 726b 2c20 3430 362c 2022  ramework, 406, "
+0000b3c0: 556e 6162 6c65 2074 6f20 7072 6f64 7563  Unable to produc
+0000b3d0: 6520 2573 2063 6f6e 7465 6e74 2220 2520  e %s content" % 
+0000b3e0: 280a 2020 2020 2020 2020 2020 2020 636f  (.            co
+0000b3f0: 6e74 656e 7420 6f72 2061 6363 6570 7420  ntent or accept 
+0000b400: 6f72 2022 756e 6b6e 6f77 6e22 2029 290a  or "unknown" )).
+0000b410: 2020 2020 6c6f 672e 696e 666f 2822 4973      log.info("Is
+0000b420: 7375 6520 7265 7175 6573 7420 6e75 6d62  sue request numb
+0000b430: 6572 3d7b 6e75 6d62 6572 7d3b 2064 6f6e  er={number}; don
+0000b440: 6522 2e66 6f72 6d61 7428 206e 756d 6265  e".format( numbe
+0000b450: 723d 6e75 6d62 6572 2029 290a 2020 2020  r=number )).    
+0000b460: 7265 7475 726e 2063 6f6e 7465 6e74 2c20  return content, 
+0000b470: 7265 7370 6f6e 7365 0a0a 0a64 6566 2069  response...def i
+0000b480: 6e6c 696e 6528 2066 696c 656e 616d 6520  nline( filename 
+0000b490: 293a 0a20 2020 2022 2222 4120 7765 622e  ):.    """A web.
+0000b4a0: 7079 2074 656d 706c 6574 6f72 2067 6c6f  py templetor glo
+0000b4b0: 6261 6c20 6675 6e63 7469 6f6e 2074 6f20  bal function to 
+0000b4c0: 696e 6c69 6e65 2066 696c 6573 2c20 7265  inline files, re
+0000b4d0: 6c61 7469 7665 2074 6f20 7468 650a 2020  lative to the.  
+0000b4e0: 2020 6469 7265 6374 6f72 7920 6f66 2074    directory of t
+0000b4f0: 6869 7320 7079 7468 6f6e 2066 696c 652e  his python file.
+0000b500: 2020 5573 653a 0a0a 2020 2020 243a 696e    Use:..    $:in
+0000b510: 6c69 6e65 2820 2273 6f6d 652f 6a61 7661  line( "some/java
+0000b520: 7363 7269 7074 2f66 696c 652e 6a73 2220  script/file.js" 
+0000b530: 290a 0a20 2020 2022 2222 0a20 2020 2077  )..    """.    w
+0000b540: 6974 6820 6f70 656e 2820 6f73 2e70 6174  ith open( os.pat
+0000b550: 682e 6a6f 696e 2820 4f55 5250 4154 482c  h.join( OURPATH,
+0000b560: 2066 696c 656e 616d 6520 292c 2027 7227   filename ), 'r'
+0000b570: 2029 2061 7320 663a 0a20 2020 2020 2020   ) as f:.       
+0000b580: 2072 6574 7572 6e20 662e 7265 6164 2829   return f.read()
+0000b590: 0a0a 0a64 6566 2077 6562 7079 2820 636f  ...def webpy( co
+0000b5a0: 6e66 6967 2029 3a0a 2020 2020 2222 2277  nfig ):.    """w
+0000b5b0: 6562 2e70 7920 696e 7465 7266 6163 652e  eb.py interface.
+0000b5c0: 2020 4465 6475 6365 7320 6163 6365 7074    Deduces accept
+0000b5d0: 2065 6e63 6f64 696e 6720 6672 6f6d 2041   encoding from A
+0000b5e0: 6363 6570 743a 2068 6561 6465 722c 206f  ccept: header, o
+0000b5f0: 7220 666f 7263 650a 2020 2020 4a53 4f4e  r force.    JSON
+0000b600: 2043 6f6e 7465 6e74 2d54 7970 653a 2069   Content-Type: i
+0000b610: 6620 2e6a 736f 6e20 7061 7468 2077 6173  f .json path was
+0000b620: 2065 7870 6c69 6369 746c 7920 7265 7175   explicitly requ
+0000b630: 6573 7465 642e 0a0a 2020 2020 2222 220a  ested...    """.
+0000b640: 2020 2020 636f 6e66 6967 2e73 6574 6465      config.setde
+0000b650: 6661 756c 7428 2027 6164 6472 6573 7327  fault( 'address'
+0000b660: 2c28 2230 2e30 2e30 2e30 222c 2038 3030  ,("0.0.0.0", 800
+0000b670: 3029 2029 0a0a 2020 2020 7365 7373 696f  0) )..    sessio
+0000b680: 6e09 0909 3d20 4e6f 6e65 0909 2320 5769  n...= None..# Wi
+0000b690: 6c6c 2062 6563 6f6d 6520 6120 7765 622e  ll become a web.
+0000b6a0: 7365 7373 696f 6e2e 5365 7373 696f 6e0a  session.Session.
+0000b6b0: 0a20 2020 2064 6566 206c 6f67 6765 6428  .    def logged(
+0000b6c0: 2061 646d 696e 3d46 616c 7365 2029 3a0a   admin=False ):.
+0000b6d0: 2020 2020 2020 2020 2222 2243 6865 636b          """Check
+0000b6e0: 6564 2074 6861 7420 7468 6520 7365 7373  ed that the sess
+0000b6f0: 696f 6e27 7320 7573 6572 2069 7320 6c6f  ion's user is lo
+0000b700: 6767 6564 2069 6e2e 2020 4576 656e 2069  gged in.  Even i
+0000b710: 6620 6120 7573 6572 2061 7574 6865 6e74  f a user authent
+0000b720: 6963 6174 6573 2c20 7468 6569 7220 6163  icates, their ac
+0000b730: 636f 756e 740a 2020 2020 2020 2020 6d61  count.        ma
+0000b740: 7920 6265 2064 6973 6162 6c65 642e 0a0a  y be disabled...
+0000b750: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000b760: 2020 2020 7265 7475 726e 2073 6573 7369      return sessi
+0000b770: 6f6e 2061 6e64 2073 6573 7369 6f6e 2e6c  on and session.l
+0000b780: 6f67 696e 203e 3d20 2820 3220 6966 2061  ogin >= ( 2 if a
+0000b790: 646d 696e 2065 6c73 6520 3120 290a 0a20  dmin else 1 ).. 
+0000b7a0: 2020 2064 6566 2070 726f 7879 2820 656e     def proxy( en
+0000b7b0: 7620 293a 0a20 2020 2020 2020 2022 2222  v ):.        """
+0000b7c0: 4465 7465 6374 7320 6966 2077 6520 6172  Detects if we ar
+0000b7d0: 6520 6265 6869 6e64 2061 2070 726f 7879  e behind a proxy
+0000b7e0: 2c20 616e 6420 6372 6561 7465 7320 636f  , and creates co
+0000b7f0: 7272 6563 7420 7061 7468 2069 660a 2020  rrect path if.  
+0000b800: 2020 2020 2020 6e65 6365 7373 6172 792c        necessary,
+0000b810: 2074 6f20 7573 6520 7468 6520 6f72 6967   to use the orig
+0000b820: 696e 616c 2066 6f72 7761 7264 6564 2068  inal forwarded h
+0000b830: 6f73 742e 0a0a 2020 2020 2020 2020 2222  ost...        ""
+0000b840: 220a 2020 2020 2020 2020 7072 6f78 7909  ".        proxy.
+0000b850: 0909 3d20 656e 762e 6765 7428 2022 4854  ..= env.get( "HT
+0000b860: 5450 5f58 5f46 4f52 5741 5244 4544 5f48  TP_X_FORWARDED_H
+0000b870: 4f53 5422 2c20 2222 2029 0a20 2020 2020  OST", "" ).     
+0000b880: 2020 2069 6620 7072 6f78 793a 0a20 2020     if proxy:.   
+0000b890: 2020 2020 2020 2020 2070 726f 7879 0909           proxy..
+0000b8a0: 3d20 2268 7474 703a 2f2f 2220 2b20 7072  = "http://" + pr
+0000b8b0: 6f78 790a 2020 2020 2020 2020 7265 7475  oxy.        retu
+0000b8c0: 726e 2070 726f 7879 0a0a 2020 2020 7572  rn proxy..    ur
+0000b8d0: 6c73 0909 093d 2028 0a20 2020 2020 2020  ls...= (.       
+0000b8e0: 2022 2f22 2c09 0909 0922 696e 6465 7822   "/",...."index"
+0000b8f0: 2c0a 2020 2020 2020 2020 7222 2f69 6e64  ,.        r"/ind
+0000b900: 6578 285c 2e68 746d 6c29 3f22 2c09 0922  ex(\.html)?",.."
+0000b910: 696e 6465 7822 2c0a 2020 2020 2020 2020  index",.        
+0000b920: 222f 282e 2a29 2f22 2c09 0909 2274 7261  "/(.*)/",..."tra
+0000b930: 696c 696e 675f 7374 7566 6622 2c0a 2020  iling_stuff",.  
+0000b940: 2020 2020 2020 7222 2f28 2e2a 295c 2e68        r"/(.*)\.h
+0000b950: 746d 6c22 2c09 0909 2274 7261 696c 696e  tml",..."trailin
+0000b960: 675f 7374 7566 6622 2c0a 2020 2020 2020  g_stuff",.      
+0000b970: 2020 222f 6661 7669 636f 6e2e 6963 6f22    "/favicon.ico"
+0000b980: 2c09 0909 2266 6176 6963 6f6e 222c 0a20  ,..."favicon",. 
+0000b990: 2020 2020 2020 2022 2f72 6f62 6f74 732e         "/robots.
+0000b9a0: 7478 7422 2c09 0909 2272 6f62 6f74 7322  txt",..."robots"
+0000b9b0: 2c0a 2020 2020 2020 2020 222f 6c6f 6769  ,.        "/logi
+0000b9c0: 6e22 2c09 0909 226c 6f67 696e 222c 0a20  n",..."login",. 
+0000b9d0: 2020 2020 2020 2022 2f6c 6f67 6f75 7422         "/logout"
+0000b9e0: 2c09 0909 226c 6f67 6f75 7422 2c0a 2020  ,..."logout",.  
+0000b9f0: 2020 2020 2020 7222 2f61 7069 2f69 7373        r"/api/iss
+0000ba00: 7565 285c 2e6a 736f 6e29 3f22 2c09 0922  ue(\.json)?",.."
+0000ba10: 6170 695f 6973 7375 6522 2c09 0923 2070  api_issue",..# p
+0000ba20: 6174 683a 2022 222c 2022 2e6a 736f 6e22  ath: "", ".json"
+0000ba30: 0a20 2020 2020 2020 2022 2f61 7069 2f69  .        "/api/i
+0000ba40: 7373 7565 2f28 2e2b 293f 222c 0909 2261  ssue/(.+)?",.."a
+0000ba50: 7069 5f69 7373 7565 222c 0909 2320 7061  pi_issue",..# pa
+0000ba60: 7468 3a20 222e 2e2e 222c 2022 2e2e 2e2e  th: "...", "....
+0000ba70: 6a73 6f6e 220a 2020 2020 2020 2020 7222  json".        r"
+0000ba80: 2f61 7069 2f6c 6963 656e 7365 7328 5c2e  /api/licenses(\.
+0000ba90: 6a73 6f6e 293f 222c 0922 6170 695f 6c69  json)?",."api_li
+0000baa0: 6365 6e73 6573 222c 0a20 2020 2020 2020  censes",.       
+0000bab0: 2022 2f61 7069 2f6c 6963 656e 7365 732f   "/api/licenses/
+0000bac0: 282e 2b29 3f22 2c09 0922 6170 695f 6c69  (.+)?",.."api_li
+0000bad0: 6365 6e73 6573 222c 0a20 2020 2020 2020  censes",.       
+0000bae0: 2072 222f 6170 692f 6372 6564 656e 7469   r"/api/credenti
+0000baf0: 616c 7328 5c2e 6a73 6f6e 293f 222c 0922  als(\.json)?",."
+0000bb00: 6170 695f 6372 6564 656e 7469 616c 7322  api_credentials"
+0000bb10: 2c0a 2020 2020 2020 2020 222f 6170 692f  ,.        "/api/
+0000bb20: 6372 6564 656e 7469 616c 732f 282e 2b29  credentials/(.+)
+0000bb30: 3f22 2c09 2261 7069 5f63 7265 6465 6e74  ?",."api_credent
+0000bb40: 6961 6c73 222c 0a20 2020 2020 2020 2072  ials",.        r
+0000bb50: 222f 6170 692f 6b65 7970 6169 7273 285c  "/api/keypairs(\
+0000bb60: 2e6a 736f 6e29 3f22 2c09 2261 7069 5f6b  .json)?",."api_k
+0000bb70: 6579 7061 6972 7322 2c0a 2020 2020 2020  eypairs",.      
+0000bb80: 2020 222f 6170 692f 6b65 7970 6169 7273    "/api/keypairs
+0000bb90: 2f28 2e2b 293f 222c 0909 2261 7069 5f6b  /(.+)?",.."api_k
+0000bba0: 6579 7061 6972 7322 2c0a 2020 2020 290a  eypairs",.    ).
+0000bbb0: 0a20 2020 2063 6c61 7373 2074 7261 696c  .    class trail
+0000bbc0: 696e 675f 7374 7566 663a 0a20 2020 2020  ing_stuff:.     
+0000bbd0: 2020 2064 6566 2047 4554 2820 7365 6c66     def GET( self
+0000bbe0: 2c20 7061 7468 2029 3a0a 2020 2020 2020  , path ):.      
+0000bbf0: 2020 2020 2020 7765 622e 7365 656f 7468        web.seeoth
+0000bc00: 6572 2820 7072 6f78 7928 2077 6562 2e63  er( proxy( web.c
+0000bc10: 7478 2e65 6e76 6972 6f6e 2029 202b 2027  tx.environ ) + '
+0000bc20: 2f27 202b 2070 6174 6820 290a 0a20 2020  /' + path )..   
+0000bc30: 2063 6c61 7373 2066 6176 6963 6f6e 3a0a   class favicon:.
+0000bc40: 2020 2020 2020 2020 6465 6620 4745 5428          def GET(
+0000bc50: 2073 656c 6620 293a 0a20 2020 2020 2020   self ):.       
+0000bc60: 2020 2020 2022 2222 416c 7761 7973 2070       """Always p
+0000bc70: 6572 6d61 6e65 6e74 6c79 2072 6564 6972  ermanently redir
+0000bc80: 6563 7420 6661 7669 636f 6e2e 6963 6f20  ect favicon.ico 
+0000bc90: 7265 7175 6573 7473 2074 6f20 6f75 7220  requests to our 
+0000bca0: 6661 7669 636f 6e2e 706e 672e 0a20 2020  favicon.png..   
+0000bcb0: 2020 2020 2020 2020 2054 6865 2072 6561           The rea
+0000bcc0: 736f 6e20 7765 2064 6f20 7468 6973 2069  son we do this i
+0000bcd0: 6e73 7465 6164 206f 6620 7075 7474 696e  nstead of puttin
+0000bce0: 6720 6120 3c6c 696e 6b20 2269 636f 6e22  g a <link "icon"
+0000bcf0: 2e2e 2e3e 2069 7320 6265 6361 7573 650a  ...> is because.
+0000bd00: 2020 2020 2020 2020 2020 2020 616c 6c20              all 
+0000bd10: 2a6f 7468 6572 2a20 7265 7175 6573 7473  *other* requests
+0000bd20: 2066 726f 6d20 6272 6f77 7365 7273 2028   from browsers (
+0000bd30: 6965 2e20 6170 692f 2e2e 2e20 2920 7265  ie. api/... ) re
+0000bd40: 7475 726e 696e 6720 6e6f 6e2d 4854 4d4c  turning non-HTML
+0000bd50: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+0000bd60: 706f 6e73 6520 436f 6e74 656e 742d 5479  ponse Content-Ty
+0000bd70: 7065 7320 7375 6368 2061 7320 6170 706c  pes such as appl
+0000bd80: 6963 6174 696f 6e2f 6a73 6f6e 202a 616c  ication/json *al
+0000bd90: 736f 2a20 7265 7175 6573 740a 2020 2020  so* request.    
+0000bda0: 2020 2020 2020 2020 6661 7669 636f 6e2e          favicon.
+0000bdb0: 6963 6f2c 2061 6e64 2077 6520 646f 6e27  ico, and we don'
+0000bdc0: 7420 6861 7665 2061 6e20 4854 4d4c 203c  t have an HTML <
+0000bdd0: 6865 6164 3e20 746f 2073 7065 6369 6679  head> to specify
+0000bde0: 2061 6e79 2069 636f 6e20 6c69 6e6b 2e0a   any icon link..
+0000bdf0: 2020 2020 2020 2020 2020 2020 4675 7274              Furt
+0000be00: 6865 726d 6f72 652c 2074 6865 7920 636f  hermore, they co
+0000be10: 6e74 696e 7565 2074 6f20 7265 7175 6573  ntinue to reques
+0000be20: 7420 6974 2027 7469 6c20 7361 7469 7366  t it 'til satisf
+0000be30: 6965 642c 2073 6f20 7765 2064 6f20 6120  ied, so we do a 
+0000be40: 3330 310a 2020 2020 2020 2020 2020 2020  301.            
+0000be50: 5065 726d 616e 656e 7420 5265 6469 7265  Permanent Redire
+0000be60: 6374 2074 6f20 7361 7469 7366 7920 7468  ct to satisfy th
+0000be70: 6520 6272 6f77 7365 7220 616e 6420 7072  e browser and pr
+0000be80: 6576 656e 7420 6675 7475 7265 2072 6571  event future req
+0000be90: 7565 7374 732e 0a20 2020 2020 2020 2020  uests..         
+0000bea0: 2020 2053 6f2c 2074 6869 7320 6973 2074     So, this is t
+0000beb0: 6865 206d 6f73 7420 6765 6e65 7261 6c20  he most general 
+0000bec0: 7761 7920 746f 2068 616e 646c 6520 7468  way to handle th
+0000bed0: 6520 6661 7669 636f 6e2e 6963 6f22 2222  e favicon.ico"""
+0000bee0: 0a20 2020 2020 2020 2020 2020 2077 6562  .            web
+0000bef0: 2e72 6564 6972 6563 7428 2027 2f73 7461  .redirect( '/sta
+0000bf00: 7469 632f 696d 6167 6573 2f66 6176 6963  tic/images/favic
+0000bf10: 6f6e 2e69 636f 2720 290a 0a20 2020 2063  on.ico' )..    c
+0000bf20: 6c61 7373 2072 6f62 6f74 733a 0a20 2020  lass robots:.   
+0000bf30: 2020 2020 2064 6566 2047 4554 2820 7365       def GET( se
+0000bf40: 6c66 2029 3a0a 2020 2020 2020 2020 2020  lf ):.          
+0000bf50: 2020 7765 622e 6865 6164 6572 2820 2243    web.header( "C
+0000bf60: 6f6e 7465 6e74 2d54 7970 6522 2c20 2274  ontent-Type", "t
+0000bf70: 6578 742f 706c 6169 6e22 2029 0a20 2020  ext/plain" ).   
+0000bf80: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000bf90: 2222 225c 0a55 7365 722d 6167 656e 743a  """\.User-agent:
+0000bfa0: 202a 0a44 6973 616c 6c6f 773a 202f 0a22   *.Disallow: /."
+0000bfb0: 2222 0a0a 2020 2020 636c 6173 7320 696e  ""..    class in
+0000bfc0: 6465 783a 0a20 2020 2020 2020 2064 6566  dex:.        def
+0000bfd0: 2047 4554 2820 7365 6c66 2c20 7061 7468   GET( self, path
+0000bfe0: 3d4e 6f6e 6520 293a 0a20 2020 2020 2020  =None ):.       
+0000bff0: 2020 2020 2072 656e 6465 7209 093d 2077       render..= w
+0000c000: 6562 2e74 656d 706c 6174 652e 7265 6e64  eb.template.rend
+0000c010: 6572 280a 2020 2020 2020 2020 2020 2020  er(.            
+0000c020: 2020 2020 5450 4c50 4154 482c 2062 6173      TPLPATH, bas
+0000c030: 653d 226c 6179 6f75 7422 2c20 676c 6f62  e="layout", glob
+0000c040: 616c 733d 7b27 696e 6c69 6e65 273a 2069  als={'inline': i
+0000c050: 6e6c 696e 652c 2027 7365 7373 696f 6e27  nline, 'session'
+0000c060: 3a20 7365 7373 696f 6e7d 2029 0a20 2020  : session} ).   
+0000c070: 2020 2020 2020 2020 2072 6573 706f 6e73           respons
+0000c080: 6509 093d 2072 656e 6465 722e 696e 6465  e..= render.inde
+0000c090: 7828 207b 0a20 2020 2020 2020 2020 2020  x( {.           
+0000c0a0: 2020 2020 2022 7469 746c 6522 3a20 0922       "title": ."
+0000c0b0: 4c69 6365 6e73 696e 6722 2c0a 2020 2020  Licensing",.    
+0000c0c0: 2020 2020 2020 2020 2020 2020 2274 6578              "tex
+0000c0d0: 7422 3a09 0922 4865 6c6c 6f2c 2077 6f72  t":.."Hello, wor
+0000c0e0: 6c64 2122 2c0a 2020 2020 2020 2020 2020  ld!",.          
+0000c0f0: 2020 7d20 290a 2020 2020 2020 2020 2020    } ).          
+0000c100: 2020 7765 622e 6865 6164 6572 2820 2243    web.header( "C
+0000c110: 6f6e 7465 6e74 2d54 7970 6522 2c20 2274  ontent-Type", "t
+0000c120: 6578 742f 6874 6d6c 2220 290a 2020 2020  ext/html" ).    
+0000c130: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+0000c140: 6573 706f 6e73 650a 0a20 2020 2063 6c61  esponse..    cla
+0000c150: 7373 206c 6f67 6f75 743a 0a20 2020 2020  ss logout:.     
+0000c160: 2020 2064 6566 2047 4554 2820 7365 6c66     def GET( self
+0000c170: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
+0000c180: 7365 7373 696f 6e2e 6c6f 6769 6e09 3d20  session.login.= 
+0000c190: 300a 2020 2020 2020 2020 2020 2020 7765  0.            we
+0000c1a0: 622e 7365 656f 7468 6572 2820 7072 6f78  b.seeother( prox
+0000c1b0: 7928 2077 6562 2e63 7478 2e65 6e76 6972  y( web.ctx.envir
+0000c1c0: 6f6e 2029 202b 2027 2f6c 6f67 696e 2720  on ) + '/login' 
+0000c1d0: 290a 0a20 2020 2064 6566 2075 7365 725f  )..    def user_
+0000c1e0: 6865 7269 7461 6765 2820 7573 6572 5f69  heritage( user_i
+0000c1f0: 6420 293a 0a20 2020 2020 2020 2022 2222  d ):.        """
+0000c200: 0a20 2020 2020 2020 2052 6574 7572 6e20  .        Return 
+0000c210: 6120 6469 6374 2063 6f6e 7461 696e 696e  a dict containin
+0000c220: 6720 7468 6520 6865 6972 6172 6368 7920  g the heirarchy 
+0000c230: 6f66 2075 7365 7220 6e61 6d65 7320 6372  of user names cr
+0000c240: 6561 7465 6420 6279 2074 6865 2073 7065  eated by the spe
+0000c250: 6369 6669 6564 2075 7365 722e 0a20 2020  cified user..   
+0000c260: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000c270: 2072 6573 756c 7409 0909 3d20 7b7d 0a0a   result...= {}..
+0000c280: 2020 2020 2020 2020 7370 6177 6e09 0909          spawn...
+0000c290: 3d20 6462 2e73 656c 6563 7428 2027 7573  = db.select( 'us
+0000c2a0: 6572 7327 2c20 7768 6572 653d 2763 7265  ers', where='cre
+0000c2b0: 6174 6f72 203d 2024 7573 6572 5f69 6427  ator = $user_id'
+0000c2c0: 2c20 7661 7273 3d7b 2022 7573 6572 5f69  , vars={ "user_i
+0000c2d0: 6422 3a20 7573 6572 5f69 6420 7d29 0a20  d": user_id }). 
+0000c2e0: 2020 2020 2020 2066 6f72 2063 6869 6c64         for child
+0000c2f0: 2069 6e20 7370 6177 6e3a 0a20 2020 2020   in spawn:.     
+0000c300: 2020 2020 2020 2069 6620 6368 696c 642e         if child.
+0000c310: 7573 6572 5f69 6420 3d3d 2075 7365 725f  user_id == user_
+0000c320: 6964 3a0a 2020 2020 2020 2020 2020 2020  id:.            
+0000c330: 2020 2020 636f 6e74 696e 7565 0a0a 2020      continue..  
+0000c340: 2020 2020 2020 2020 2020 6b65 7909 0909            key...
+0000c350: 3d20 2863 6869 6c64 2e6e 616d 652c 2063  = (child.name, c
+0000c360: 6869 6c64 2e75 7365 725f 6964 290a 2020  hild.user_id).  
+0000c370: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+0000c380: 5b6b 6579 5d09 093d 2075 7365 725f 6865  [key]..= user_he
+0000c390: 7269 7461 6765 2820 6368 696c 642e 7573  ritage( child.us
+0000c3a0: 6572 5f69 6420 290a 0a20 2020 2020 2020  er_id )..       
+0000c3b0: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
+0000c3c0: 2020 2020 6465 6620 7573 6572 5f68 6572      def user_her
+0000c3d0: 6974 6167 655f 7072 696e 7428 2068 2c20  itage_print( h, 
+0000c3e0: 6c65 7665 6c3d 3020 293a 0a20 2020 2020  level=0 ):.     
+0000c3f0: 2020 2069 6620 6e6f 7420 683a 0a20 2020     if not h:.   
+0000c400: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
+0000c410: 2020 2020 2020 2020 666f 7220 6b65 7920          for key 
+0000c420: 696e 2068 3a0a 2020 2020 2020 2020 2020  in h:.          
+0000c430: 2020 6e61 6d65 2c75 7365 725f 6964 093d    name,user_id.=
+0000c440: 206b 6579 0a20 2020 2020 2020 2020 2020   key.           
+0000c450: 206c 6f67 2e69 6e66 6f28 2225 7320 2573   log.info("%s %s
+0000c460: 2220 2520 2820 2720 272a 6c65 7665 6c2c  " % ( ' '*level,
+0000c470: 206e 616d 6520 2929 0a20 2020 2020 2020   name )).       
+0000c480: 2020 2020 2069 6620 685b 6b65 795d 3a0a       if h[key]:.
+0000c490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c4a0: 7573 6572 5f68 6572 6974 6167 655f 7072  user_heritage_pr
+0000c4b0: 696e 7428 2068 5b6b 6579 5d2c 206c 6576  int( h[key], lev
+0000c4c0: 656c 2b31 2029 0a0a 2020 2020 636c 6173  el+1 )..    clas
+0000c4d0: 7320 6c6f 6769 6e3a 0a20 2020 2020 2020  s login:.       
+0000c4e0: 2022 2222 0a20 2020 2020 2020 2054 616b   """.        Tak
+0000c4f0: 6573 2061 6e20 6f70 7469 6f6e 616c 203f  es an optional ?
+0000c500: 7265 6469 7265 6374 3d75 726c 2061 6e64  redirect=url and
+0000c510: 2070 6173 7365 7320 6974 2076 6961 2074   passes it via t
+0000c520: 6865 2050 4f53 542e 0a20 2020 2020 2020  he POST..       
+0000c530: 2022 2222 0a20 2020 2020 2020 2064 6566   """.        def
+0000c540: 2047 4554 2820 7365 6c66 2029 3a0a 2020   GET( self ):.  
+0000c550: 2020 2020 2020 2020 2020 2222 2241 6c6c            """All
+0000c560: 6f77 206c 6f67 696e 3b20 6966 2073 6573  ow login; if ses
+0000c570: 7369 6f6e 2e6c 6f67 696e 2061 6c72 6561  sion.login alrea
+0000c580: 6479 2074 7275 652c 2074 6865 6e20 6469  dy true, then di
+0000c590: 7370 6c61 7920 5049 4e20 6368 616e 6765  splay PIN change
+0000c5a0: 2064 6961 6c6f 672e 2222 220a 2020 2020   dialog.""".    
+0000c5b0: 2020 2020 2020 2020 6c6f 672e 696e 666f          log.info
+0000c5c0: 2820 2253 6573 7369 6f6e 3a20 2572 2220  ( "Session: %r" 
+0000c5d0: 2520 2820 7365 7373 696f 6e2e 6974 656d  % ( session.item
+0000c5e0: 7328 2920 2929 0a20 2020 2020 2020 2020  s() )).         
+0000c5f0: 2020 2063 6869 6c64 7265 6e09 093d 204e     children..= N
+0000c600: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
+0000c610: 6966 206c 6f67 6765 6428 293a 0a20 2020  if logged():.   
+0000c620: 2020 2020 2020 2020 2020 2020 2063 6869               chi
+0000c630: 6c64 7265 6e09 3d20 7573 6572 5f68 6572  ldren.= user_her
+0000c640: 6974 6167 6528 2073 6573 7369 6f6e 2e75  itage( session.u
+0000c650: 7365 725f 6964 2029 0a20 2020 2020 2020  ser_id ).       
+0000c660: 2020 2020 2020 2020 2075 7365 725f 6865           user_he
+0000c670: 7269 7461 6765 5f70 7269 6e74 2820 6368  ritage_print( ch
+0000c680: 696c 6472 656e 2029 0a0a 2020 2020 2020  ildren )..      
+0000c690: 2020 2020 2020 7265 6e64 6572 0909 3d20        render..= 
+0000c6a0: 7765 622e 7465 6d70 6c61 7465 2e72 656e  web.template.ren
+0000c6b0: 6465 7228 0a20 2020 2020 2020 2020 2020  der(.           
+0000c6c0: 2020 2020 2054 504c 5041 5448 2c20 6261       TPLPATH, ba
+0000c6d0: 7365 3d22 6c61 796f 7574 222c 2067 6c6f  se="layout", glo
+0000c6e0: 6261 6c73 3d7b 2769 6e6c 696e 6527 3a20  bals={'inline': 
+0000c6f0: 696e 6c69 6e65 2c20 2773 6573 7369 6f6e  inline, 'session
+0000c700: 273a 2073 6573 7369 6f6e 7d20 290a 2020  ': session} ).  
+0000c710: 2020 2020 2020 2020 2020 7265 7370 6f6e            respon
+0000c720: 7365 0909 3d20 7265 6e64 6572 2e6c 6f67  se..= render.log
+0000c730: 696e 280a 2020 2020 2020 2020 2020 2020  in(.            
+0000c740: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
+0000c750: 2020 2020 2020 2020 2020 2274 6974 6c65            "title
+0000c760: 223a 0928 2022 4c6f 6769 6e22 0a20 2020  ":.( "Login".   
+0000c770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c780: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000c790: 6620 6e6f 7420 6c6f 6767 6564 2829 2065  f not logged() e
+0000c7a0: 6c73 650a 2020 2020 2020 2020 2020 2020  lse.            
+0000c7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c7c0: 2020 2020 2020 2257 656c 636f 6d65 2025        "Welcome %
+0000c7d0: 7322 2025 2028 2073 6573 7369 6f6e 2e6e  s" % ( session.n
+0000c7e0: 616d 652e 6361 7069 7461 6c69 7a65 2829  ame.capitalize()
+0000c7f0: 2029 292c 0a20 2020 2020 2020 2020 2020   )),.           
+0000c800: 2020 2020 2020 2020 2022 7265 6469 7265           "redire
+0000c810: 6374 223a 0977 6562 2e69 6e70 7574 2829  ct":.web.input()
+0000c820: 2e67 6574 2820 2272 6564 6972 6563 7422  .get( "redirect"
+0000c830: 2c20 2222 2029 2c0a 2020 2020 2020 2020  , "" ),.        
+0000c840: 2020 2020 2020 2020 2020 2020 2263 6869              "chi
+0000c850: 6c64 7265 6e22 3a20 6368 696c 6472 656e  ldren": children
+0000c860: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000c870: 2020 7d29 0a20 2020 2020 2020 2020 2020    }).           
+0000c880: 2077 6562 2e68 6561 6465 7228 2022 4361   web.header( "Ca
+0000c890: 6368 652d 436f 6e74 726f 6c22 2c20 226e  che-Control", "n
+0000c8a0: 6f2d 6361 6368 6522 2029 0a20 2020 2020  o-cache" ).     
+0000c8b0: 2020 2020 2020 2077 6562 2e68 6561 6465         web.heade
+0000c8c0: 7228 2022 436f 6e74 656e 742d 5479 7065  r( "Content-Type
+0000c8d0: 222c 2022 7465 7874 2f68 746d 6c22 2029  ", "text/html" )
+0000c8e0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0000c8f0: 7572 6e20 7265 7370 6f6e 7365 0a0a 2020  urn response..  
+0000c900: 2020 2020 2020 6465 6620 504f 5354 2820        def POST( 
+0000c910: 7365 6c66 2029 3a0a 2020 2020 2020 2020  self ):.        
+0000c920: 2020 2020 2222 2255 7365 2074 6865 2070      """Use the p
+0000c930: 726f 7669 6465 6420 5049 4e20 746f 2061  rovided PIN to a
+0000c940: 7574 6865 6e74 6963 6174 6520 6120 7573  uthenticate a us
+0000c950: 6572 2c20 616e 6420 7468 656e 2072 656d  er, and then rem
+0000c960: 656d 6265 7220 7468 6520 6372 6564 656e  ember the creden
+0000c970: 7469 616c 7320 696e 2074 6865 0a20 2020  tials in the.   
+0000c980: 2020 2020 2020 2020 2073 6573 7369 6f6e           session
+0000c990: 2e20 2049 6620 616c 7265 6164 7920 6c6f  .  If already lo
+0000c9a0: 6767 6564 2069 6e2c 2061 6e64 2074 6865  gged in, and the
+0000c9b0: 2027 7069 6e6e 6577 2720 7661 6c75 6520   'pinnew' value 
+0000c9c0: 616e 6420 2763 6861 6e67 6527 2062 7574  and 'change' but
+0000c9d0: 746f 6e20 7761 7320 7375 7070 6c69 6564  ton was supplied
+0000c9e0: 2c0a 2020 2020 2020 2020 2020 2020 7468  ,.            th
+0000c9f0: 656e 2063 6861 6e67 6520 7468 6520 7573  en change the us
+0000ca00: 6572 2773 2050 494e 2e0a 0a20 2020 2020  er's PIN...     
+0000ca10: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000ca20: 2020 2020 2020 206c 6f67 2e69 6e66 6f28         log.info(
+0000ca30: 2022 5365 7373 696f 6e3a 2025 722c 2069   "Session: %r, i
+0000ca40: 6e70 7574 3a20 2572 2220 2520 2820 7365  nput: %r" % ( se
+0000ca50: 7373 696f 6e2e 6974 656d 7328 292c 2077  ssion.items(), w
+0000ca60: 6562 2e69 6e70 7574 2829 2e69 7465 6d73  eb.input().items
+0000ca70: 2829 2029 290a 2020 2020 2020 2020 2020  () )).          
+0000ca80: 2020 7265 6e64 6572 0909 3d20 7765 622e    render..= web.
+0000ca90: 7465 6d70 6c61 7465 2e72 656e 6465 7228  template.render(
+0000caa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000cab0: 2054 504c 5041 5448 2c20 6261 7365 3d22   TPLPATH, base="
+0000cac0: 6c61 796f 7574 222c 2067 6c6f 6261 6c73  layout", globals
+0000cad0: 3d7b 2769 6e6c 696e 6527 3a20 696e 6c69  ={'inline': inli
+0000cae0: 6e65 2c20 2773 6573 7369 6f6e 273a 2073  ne, 'session': s
+0000caf0: 6573 7369 6f6e 7d20 290a 0a20 2020 2020  ession} )..     
+0000cb00: 2020 2020 2020 2069 6620 2261 6464 2220         if "add" 
+0000cb10: 696e 2077 6562 2e69 6e70 7574 2829 3a0a  in web.input():.
+0000cb20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cb30: 2320 506f 7374 2076 6961 2022 6164 6422  # Post via "add"
+0000cb40: 2062 7574 746f 6e3b 2061 6464 2061 206e   button; add a n
+0000cb50: 6577 2075 7365 722f 5049 4e20 772f 2061  ew user/PIN w/ a
+0000cb60: 2073 656c 6563 7465 6420 7375 6273 6574   selected subset
+0000cb70: 206f 6620 6375 7272 656e 7420 7573 6572   of current user
+0000cb80: 2773 0a20 2020 2020 2020 2020 2020 2020  's.             
+0000cb90: 2020 2023 207a 6f6e 6573 2e20 2054 7279     # zones.  Try
+0000cba0: 2075 7064 6174 6520 6669 7273 7420 286f   update first (o
+0000cbb0: 6620 6578 6973 7469 6e67 2075 7365 722f  f existing user/
+0000cbc0: 5049 4e20 696e 2074 6865 2073 6573 7369  PIN in the sessi
+0000cbd0: 6f6e 2075 7365 7273 2068 6572 6974 6167  on users heritag
+0000cbe0: 6529 2c0a 2020 2020 2020 2020 2020 2020  e),.            
+0000cbf0: 2020 2020 2320 7468 656e 2069 6e73 6572      # then inser
+0000cc00: 742e 0a20 2020 2020 2020 2020 2020 2020  t..             
+0000cc10: 2020 2065 7272 6f72 0909 3d20 4e6f 6e65     error..= None
+0000cc20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000cc30: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+0000cc40: 2020 2020 2020 2020 2020 6173 7365 7274            assert
+0000cc50: 206c 6f67 6765 6428 292c 2022 4e6f 7420   logged(), "Not 
+0000cc60: 6c6f 6767 6564 2069 6e22 0a20 2020 2020  logged in".     
+0000cc70: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+0000cc80: 616d 6509 3d20 7765 622e 696e 7075 7428  ame.= web.input(
+0000cc90: 292e 6765 7428 2022 6e61 6d65 2220 290a  ).get( "name" ).
+0000cca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ccb0: 2020 2020 6173 7365 7274 206e 616d 652c      assert name,
+0000ccc0: 2022 456d 7074 7920 6e61 6d65 220a 2020   "Empty name".  
+0000ccd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cce0: 2020 6c6f 6769 6e09 3d20 7765 622e 696e    login.= web.in
+0000ccf0: 7075 7428 292e 6765 7428 2022 6c6f 6769  put().get( "logi
+0000cd00: 6e22 2c20 3120 290a 2020 2020 2020 2020  n", 1 ).        
+0000cd10: 2020 2020 2020 2020 2020 2020 6173 7365              asse
+0000cd20: 7274 2030 203c 3d20 696e 7428 206c 6f67  rt 0 <= int( log
+0000cd30: 696e 2029 203c 3d20 322c 2022 496e 7661  in ) <= 2, "Inva
+0000cd40: 6c69 6420 6c6f 6769 6e20 4469 7361 626c  lid login Disabl
+0000cd50: 6528 3029 2f4e 6f72 6d61 6c28 3129 2f41  e(0)/Normal(1)/A
+0000cd60: 646d 696e 2832 2922 0a20 2020 2020 2020  dmin(2)".       
+0000cd70: 2020 2020 2020 2020 2020 2020 2070 696e               pin
+0000cd80: 0909 3d20 7765 622e 696e 7075 7428 292e  ..= web.input().
+0000cd90: 6765 7428 2022 7069 6e22 2029 0a0a 2020  get( "pin" )..  
 0000cda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cdb0: 2320 4966 2074 6865 2063 7572 7265 6e74  # If the current
-0000cdc0: 2075 7365 7220 6973 2061 6e20 6164 6d69   user is an admi
-0000cdd0: 6e20 7573 6572 2c20 7765 2063 616e 2061  n user, we can a
-0000cde0: 6c74 6572 2061 6e20 6578 6973 7469 6e67  lter an existing
-0000cdf0: 2075 7365 720a 2020 2020 2020 2020 2020   user.          
-0000ce00: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-0000ce10: 7468 6174 2077 6527 7665 2063 7265 6174  that we've creat
-0000ce20: 6564 3b20 6368 616e 6765 2061 2070 696e  ed; change a pin
-0000ce30: 206f 7220 6c6f 6769 6e20 7072 6976 696c   or login privil
-0000ce40: 6567 6573 0a20 2020 2020 2020 2020 2020  eges.           
-0000ce50: 2020 2020 2020 2020 2020 2020 2065 7661               eva
-0000ce60: 6c75 6174 6509 093d 2075 7365 725f 6865  luate..= user_he
-0000ce70: 7269 7461 6765 2820 7365 7373 696f 6e2e  ritage( session.
-0000ce80: 7573 6572 5f69 6420 292e 6974 656d 7328  user_id ).items(
-0000ce90: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000cea0: 2020 2020 2020 2020 2020 7461 7267 6574            target
-0000ceb0: 0909 093d 204e 6f6e 650a 2020 2020 2020  ...= None.      
-0000cec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ced0: 2020 7768 696c 6520 6576 616c 7561 7465    while evaluate
-0000cee0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000cef0: 2020 2020 2020 2020 2020 2020 2020 6974                it
-0000cf00: 656d 0909 3d20 6576 616c 7561 7465 2e70  em..= evaluate.p
-0000cf10: 6f70 2829 0a20 2020 2020 2020 2020 2020  op().           
-0000cf20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf30: 2028 696e 616d 2c69 7569 6429 2c73 7562   (inam,iuid),sub
-0000cf40: 7309 3d20 6974 656d 0a20 2020 2020 2020  s.= item.       
-0000cf50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf60: 2020 2020 2069 6620 696e 616d 203d 3d20       if inam == 
-0000cf70: 6e61 6d65 3a0a 2020 2020 2020 2020 2020  name:.          
-0000cf80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf90: 2020 2020 2020 7461 7267 6574 0909 3d20        target..= 
-0000cfa0: 6975 6964 0a20 2020 2020 2020 2020 2020  iuid.           
-0000cfb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cfc0: 2020 2020 2062 7265 616b 0a20 2020 2020       break.     
+0000cdb0: 2020 7570 6461 7465 093d 204e 6f6e 650a    update.= None.
+0000cdc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cdd0: 2020 2020 6966 206c 6f67 6765 6428 2061      if logged( a
+0000cde0: 646d 696e 3d54 7275 6520 293a 0a20 2020  dmin=True ):.   
+0000cdf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ce00: 2020 2020 2023 2049 6620 7468 6520 6375       # If the cu
+0000ce10: 7272 656e 7420 7573 6572 2069 7320 616e  rrent user is an
+0000ce20: 2061 646d 696e 2075 7365 722c 2077 6520   admin user, we 
+0000ce30: 6361 6e20 616c 7465 7220 616e 2065 7869  can alter an exi
+0000ce40: 7374 696e 6720 7573 6572 0a20 2020 2020  sting user.     
+0000ce50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ce60: 2020 2023 2074 6861 7420 7765 2776 6520     # that we've 
+0000ce70: 6372 6561 7465 643b 2063 6861 6e67 6520  created; change 
+0000ce80: 6120 7069 6e20 6f72 206c 6f67 696e 2070  a pin or login p
+0000ce90: 7269 7669 6c65 6765 730a 2020 2020 2020  rivileges.      
+0000cea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ceb0: 2020 6576 616c 7561 7465 0909 3d20 7573    evaluate..= us
+0000cec0: 6572 5f68 6572 6974 6167 6528 2073 6573  er_heritage( ses
+0000ced0: 7369 6f6e 2e75 7365 725f 6964 2029 2e69  sion.user_id ).i
+0000cee0: 7465 6d73 2829 0a20 2020 2020 2020 2020  tems().         
+0000cef0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0000cf00: 6172 6765 7409 0909 3d20 4e6f 6e65 0a20  arget...= None. 
+0000cf10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cf20: 2020 2020 2020 2077 6869 6c65 2065 7661         while eva
+0000cf30: 6c75 6174 653a 0a20 2020 2020 2020 2020  luate:.         
+0000cf40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cf50: 2020 2069 7465 6d09 093d 2065 7661 6c75     item..= evalu
+0000cf60: 6174 652e 706f 7028 290a 2020 2020 2020  ate.pop().      
+0000cf70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cf80: 2020 2020 2020 2869 6e61 6d2c 6975 6964        (inam,iuid
+0000cf90: 292c 7375 6273 093d 2069 7465 6d0a 2020  ),subs.= item.  
+0000cfa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cfb0: 2020 2020 2020 2020 2020 6966 2069 6e61            if ina
+0000cfc0: 6d20 3d3d 206e 616d 653a 0a20 2020 2020  m == name:.     
 0000cfd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cfe0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-0000cff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d000: 2020 2020 2020 2020 2020 2020 2023 204e               # N
-0000d010: 6f74 2075 7064 6174 696e 6720 7468 6973  ot updating this
-0000d020: 2075 7365 723b 2070 6572 6861 7073 206f   user; perhaps o
-0000d030: 6e65 206f 6620 7468 6569 7220 7375 622d  ne of their sub-
-0000d040: 7573 6572 733f 0a20 2020 2020 2020 2020  users?.         
+0000cfe0: 2020 2020 2020 2020 2020 2074 6172 6765             targe
+0000cff0: 7409 093d 2069 7569 640a 2020 2020 2020  t..= iuid.      
+0000d000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d010: 2020 2020 2020 2020 2020 6272 6561 6b0a            break.
+0000d020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d030: 2020 2020 2020 2020 2020 2020 656c 7365              else
+0000d040: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
 0000d050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d060: 2020 2020 2020 2065 7661 6c75 6174 6520         evaluate 
-0000d070: 2020 2020 2020 2b3d 2073 7562 732e 6974        += subs.it
-0000d080: 656d 7328 290a 2020 2020 2020 2020 2020  ems().          
-0000d090: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0000d0a0: 2074 6172 6765 743a 0a20 2020 2020 2020   target:.       
-0000d0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d0c0: 2020 2020 206c 6f67 2e69 6e66 6f28 2022       log.info( "
-0000d0d0: 5570 6461 7469 6e67 2075 7365 723a 2025  Updating user: %
-0000d0e0: 7222 2025 2028 206e 616d 6520 2929 0a20  r" % ( name )). 
-0000d0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d100: 2020 2020 2020 2020 2020 206b 7764 7309             kwds.
-0000d110: 093d 207b 7d0a 2020 2020 2020 2020 2020  .= {}.          
-0000d120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d130: 2020 6b77 6473 5b22 6c6f 6769 6e22 5d09    kwds["login"].
-0000d140: 3d20 6c6f 6769 6e0a 2020 2020 2020 2020  = login.        
+0000d060: 2020 2320 4e6f 7420 7570 6461 7469 6e67    # Not updating
+0000d070: 2074 6869 7320 7573 6572 3b20 7065 7268   this user; perh
+0000d080: 6170 7320 6f6e 6520 6f66 2074 6865 6972  aps one of their
+0000d090: 2073 7562 2d75 7365 7273 3f0a 2020 2020   sub-users?.    
+0000d0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d0b0: 2020 2020 2020 2020 2020 2020 6576 616c              eval
+0000d0c0: 7561 7465 2020 2020 2020 202b 3d20 7375  uate       += su
+0000d0d0: 6273 2e69 7465 6d73 2829 0a20 2020 2020  bs.items().     
+0000d0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d0f0: 2020 2069 6620 7461 7267 6574 3a0a 2020     if target:.  
+0000d100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d110: 2020 2020 2020 2020 2020 6c6f 672e 696e            log.in
+0000d120: 666f 2820 2255 7064 6174 696e 6720 7573  fo( "Updating us
+0000d130: 6572 3a20 2572 2220 2520 2820 6e61 6d65  er: %r" % ( name
+0000d140: 2029 290a 2020 2020 2020 2020 2020 2020   )).            
 0000d150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d160: 2020 2020 6966 2070 696e 3a20 2020 2023      if pin:    #
-0000d170: 2055 7064 6174 6520 7069 6e20 746f 6f2c   Update pin too,
-0000d180: 2069 6620 7375 7070 6c69 6564 0a20 2020   if supplied.   
-0000d190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d1a0: 2020 2020 2020 2020 2020 2020 206b 7764               kwd
-0000d1b0: 735b 2270 696e 225d 093d 2070 696e 0a20  s["pin"].= pin. 
-0000d1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d1d0: 2020 2020 2020 2020 2020 2077 6974 6820             with 
-0000d1e0: 6462 5f6c 6f63 6b3a 0a20 2020 2020 2020  db_lock:.       
+0000d160: 6b77 6473 0909 3d20 7b7d 0a20 2020 2020  kwds..= {}.     
+0000d170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d180: 2020 2020 2020 206b 7764 735b 226c 6f67         kwds["log
+0000d190: 696e 225d 093d 206c 6f67 696e 0a20 2020  in"].= login.   
+0000d1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d1b0: 2020 2020 2020 2020 2069 6620 7069 6e3a           if pin:
+0000d1c0: 2020 2020 2320 5570 6461 7465 2070 696e      # Update pin
+0000d1d0: 2074 6f6f 2c20 6966 2073 7570 706c 6965   too, if supplie
+0000d1e0: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
 0000d1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d200: 2020 2020 2020 2020 2075 7064 6174 6520           update 
-0000d210: 3d20 6462 2e75 7064 6174 6528 2027 7573  = db.update( 'us
-0000d220: 6572 7327 2c20 7768 6572 653d 2775 7365  ers', where='use
-0000d230: 725f 6964 203d 2024 7573 6572 5f69 6427  r_id = $user_id'
-0000d240: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000d250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d270: 2020 2020 2020 7661 7273 3d7b 2022 7573        vars={ "us
-0000d280: 6572 5f69 6422 3a20 7461 7267 6574 207d  er_id": target }
-0000d290: 2c20 2a2a 6b77 6473 2029 0a20 2020 2020  , **kwds ).     
+0000d200: 2020 6b77 6473 5b22 7069 6e22 5d09 3d20    kwds["pin"].= 
+0000d210: 7069 6e0a 2020 2020 2020 2020 2020 2020  pin.            
+0000d220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d230: 7769 7468 2064 625f 6c6f 636b 3a0a 2020  with db_lock:.  
+0000d240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d250: 2020 2020 2020 2020 2020 2020 2020 7570                up
+0000d260: 6461 7465 203d 2064 622e 7570 6461 7465  date = db.update
+0000d270: 2820 2775 7365 7273 272c 2077 6865 7265  ( 'users', where
+0000d280: 3d27 7573 6572 5f69 6420 3d20 2475 7365  ='user_id = $use
+0000d290: 725f 6964 272c 0a20 2020 2020 2020 2020  r_id',.         
 0000d2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d2b0: 2020 2020 2020 2061 7373 6572 7420 7570         assert up
-0000d2c0: 6461 7465 2c20 2255 7064 6174 6520 6661  date, "Update fa
-0000d2d0: 696c 6564 220a 2020 2020 2020 2020 2020  iled".          
-0000d2e0: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-0000d2f0: 2075 7064 6174 653a 0a20 2020 2020 2020   update:.       
-0000d300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d310: 2023 2045 7869 7374 696e 6720 7573 6572   # Existing user
-0000d320: 206e 6f74 2066 6f75 6e64 2061 6e64 2075   not found and u
-0000d330: 7064 6174 6564 3b20 696e 7365 7274 2061  pdated; insert a
-0000d340: 206e 6577 206f 6e65 0a20 2020 2020 2020   new one.       
+0000d2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d2c0: 2020 2020 2020 2020 2020 2076 6172 733d             vars=
+0000d2d0: 7b20 2275 7365 725f 6964 223a 2074 6172  { "user_id": tar
+0000d2e0: 6765 7420 7d2c 202a 2a6b 7764 7320 290a  get }, **kwds ).
+0000d2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d300: 2020 2020 2020 2020 2020 2020 6173 7365              asse
+0000d310: 7274 2075 7064 6174 652c 2022 5570 6461  rt update, "Upda
+0000d320: 7465 2066 6169 6c65 6422 0a20 2020 2020  te failed".     
+0000d330: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000d340: 6620 6e6f 7420 7570 6461 7465 3a0a 2020  f not update:.  
 0000d350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d360: 2061 7373 6572 7420 7069 6e2c 2022 456d   assert pin, "Em
-0000d370: 7074 7920 5049 4e22 0a20 2020 2020 2020  pty PIN".       
-0000d380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d390: 206c 6f67 2e69 6e66 6f28 2022 4164 6469   log.info( "Addi
-0000d3a0: 6e67 2055 7365 723a 2025 7222 2025 2028  ng User: %r" % (
-0000d3b0: 206e 616d 6520 2929 0a20 2020 2020 2020   name )).       
-0000d3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d3d0: 2077 6974 6820 6462 5f6c 6f63 6b3a 0a20   with db_lock:. 
-0000d3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d3f0: 2020 2020 2020 2020 2020 2069 6e73 6572             inser
-0000d400: 7420 3d20 6462 2e69 6e73 6572 7428 2027  t = db.insert( '
-0000d410: 7573 6572 7327 2c0a 2020 2020 2020 2020  users',.        
-0000d420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d440: 2020 2020 2020 2020 6372 6561 746f 723d          creator=
-0000d450: 7365 7373 696f 6e2e 7573 6572 5f69 642c  session.user_id,
-0000d460: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d360: 2020 2020 2020 2320 4578 6973 7469 6e67        # Existing
+0000d370: 2075 7365 7220 6e6f 7420 666f 756e 6420   user not found 
+0000d380: 616e 6420 7570 6461 7465 643b 2069 6e73  and updated; ins
+0000d390: 6572 7420 6120 6e65 7720 6f6e 650a 2020  ert a new one.  
+0000d3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d3b0: 2020 2020 2020 6173 7365 7274 2070 696e        assert pin
+0000d3c0: 2c20 2245 6d70 7479 2050 494e 220a 2020  , "Empty PIN".  
+0000d3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d3e0: 2020 2020 2020 6c6f 672e 696e 666f 2820        log.info( 
+0000d3f0: 2241 6464 696e 6720 5573 6572 3a20 2572  "Adding User: %r
+0000d400: 2220 2520 2820 6e61 6d65 2029 290a 2020  " % ( name )).  
+0000d410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d420: 2020 2020 2020 7769 7468 2064 625f 6c6f        with db_lo
+0000d430: 636b 3a0a 2020 2020 2020 2020 2020 2020  ck:.            
+0000d440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d450: 696e 7365 7274 203d 2064 622e 696e 7365  insert = db.inse
+0000d460: 7274 2820 2775 7365 7273 272c 0a20 2020  rt( 'users',.   
 0000d470: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000d480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d490: 206e 616d 653d 6e61 6d65 2e6c 6f77 6572   name=name.lower
-0000d4a0: 2829 2c0a 2020 2020 2020 2020 2020 2020  (),.            
-0000d4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d490: 2020 2020 2020 2020 2020 2020 2063 7265               cre
+0000d4a0: 6174 6f72 3d73 6573 7369 6f6e 2e75 7365  ator=session.use
+0000d4b0: 725f 6964 2c0a 2020 2020 2020 2020 2020  r_id,.          
 0000d4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d4d0: 2020 2020 7069 6e3d 7069 6e2c 0a20 2020      pin=pin,.   
-0000d4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d500: 2020 2020 2020 2020 2020 2020 206c 6f67               log
-0000d510: 696e 3d6c 6f67 696e 2029 0a20 2020 2020  in=login ).     
-0000d520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d530: 2020 2061 7373 6572 7420 696e 7365 7274     assert insert
-0000d540: 2c20 2249 6e73 6572 7420 6661 696c 6564  , "Insert failed
-0000d550: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-0000d560: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
-0000d570: 6f6e 2061 7320 6578 633a 0a20 2020 2020  on as exc:.     
-0000d580: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-0000d590: 6f67 2e69 6e66 6f28 2022 4164 642f 5570  og.info( "Add/Up
-0000d5a0: 6461 7465 2075 7365 7220 6661 696c 7572  date user failur
-0000d5b0: 653a 2025 733a 2025 7322 2025 2028 2065  e: %s: %s" % ( e
-0000d5c0: 7863 2c20 7472 6163 6562 6163 6b2e 666f  xc, traceback.fo
-0000d5d0: 726d 6174 5f65 7863 2829 2029 290a 2020  rmat_exc() )).  
-0000d5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d5f0: 2020 6572 726f 7209 3d20 7374 7228 2065    error.= str( e
-0000d600: 7863 2029 0a20 2020 2020 2020 2020 2020  xc ).           
-0000d610: 2020 2020 2072 6573 706f 6e73 6509 3d20       response.= 
-0000d620: 7265 6e64 6572 2e6c 6f67 696e 280a 2020  render.login(.  
-0000d630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d640: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
-0000d650: 2020 2020 2020 2020 2020 2020 2274 6974              "tit
-0000d660: 6c65 223a 0928 2022 4164 6420 5573 6572  le":.( "Add User
-0000d670: 2046 6169 6c65 643a 2025 7322 2025 2028   Failed: %s" % (
-0000d680: 2065 7272 6f72 2029 0a20 2020 2020 2020   error ).       
-0000d690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d4e0: 2020 2020 2020 6e61 6d65 3d6e 616d 652e        name=name.
+0000d4f0: 6c6f 7765 7228 292c 0a20 2020 2020 2020  lower(),.       
+0000d500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d520: 2020 2020 2020 2020 2070 696e 3d70 696e           pin=pin
+0000d530: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000d540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d560: 2020 6c6f 6769 6e3d 6c6f 6769 6e20 290a    login=login ).
+0000d570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d580: 2020 2020 2020 2020 6173 7365 7274 2069          assert i
+0000d590: 6e73 6572 742c 2022 496e 7365 7274 2066  nsert, "Insert f
+0000d5a0: 6169 6c65 6422 0a20 2020 2020 2020 2020  ailed".         
+0000d5b0: 2020 2020 2020 2065 7863 6570 7420 4578         except Ex
+0000d5c0: 6365 7074 696f 6e20 6173 2065 7863 3a0a  ception as exc:.
+0000d5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d5e0: 2020 2020 6c6f 672e 696e 666f 2820 2241      log.info( "A
+0000d5f0: 6464 2f55 7064 6174 6520 7573 6572 2066  dd/Update user f
+0000d600: 6169 6c75 7265 3a20 2573 3a20 2573 2220  ailure: %s: %s" 
+0000d610: 2520 2820 6578 632c 2074 7261 6365 6261  % ( exc, traceba
+0000d620: 636b 2e66 6f72 6d61 745f 6578 6328 2920  ck.format_exc() 
+0000d630: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
+0000d640: 2020 2020 2020 2065 7272 6f72 093d 2073         error.= s
+0000d650: 7472 2820 6578 6320 290a 2020 2020 2020  tr( exc ).      
+0000d660: 2020 2020 2020 2020 2020 7265 7370 6f6e            respon
+0000d670: 7365 093d 2072 656e 6465 722e 6c6f 6769  se.= render.logi
+0000d680: 6e28 0a20 2020 2020 2020 2020 2020 2020  n(.             
+0000d690: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
 0000d6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d6b0: 2020 2069 6620 6572 726f 7220 656c 7365     if error else
-0000d6c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d6e0: 2020 2020 2020 2020 2020 2022 5570 6461             "Upda
-0000d6f0: 7465 6420 5573 6572 2025 7322 2025 2028  ted User %s" % (
-0000d700: 206e 616d 6520 290a 2020 2020 2020 2020   name ).        
-0000d710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d6b0: 2022 7469 746c 6522 3a09 2820 2241 6464   "title":.( "Add
+0000d6c0: 2055 7365 7220 4661 696c 6564 3a20 2573   User Failed: %s
+0000d6d0: 2220 2520 2820 6572 726f 7220 290a 2020  " % ( error ).  
+0000d6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d700: 2020 2020 2020 2020 6966 2065 7272 6f72          if error
+0000d710: 2065 6c73 650a 2020 2020 2020 2020 2020   else.          
 0000d720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d730: 2020 6966 2075 7064 6174 6520 656c 7365    if update else
-0000d740: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d760: 2020 2020 2020 2020 2020 2022 4164 6465             "Adde
-0000d770: 6420 5573 6572 2025 7322 2025 2028 206e  d User %s" % ( n
-0000d780: 616d 6520 2929 2c0a 2020 2020 2020 2020  ame )),.        
-0000d790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d7a0: 2272 6564 6972 6563 7422 3a09 7765 622e  "redirect":.web.
-0000d7b0: 696e 7075 7428 292e 6765 7428 2022 7265  input().get( "re
-0000d7c0: 6469 7265 6374 222c 2022 2220 292c 0a20  direct", "" ),. 
-0000d7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d7e0: 2020 2020 2020 2022 6368 696c 6472 656e         "children
-0000d7f0: 223a 0975 7365 725f 6865 7269 7461 6765  ":.user_heritage
-0000d800: 2820 7365 7373 696f 6e2e 7573 6572 5f69  ( session.user_i
-0000d810: 6420 292c 0a20 2020 2020 2020 2020 2020  d ),.           
-0000d820: 2020 2020 2020 2020 207d 290a 2020 2020           }).    
-0000d830: 2020 2020 2020 2020 2020 2020 7765 622e              web.
-0000d840: 6865 6164 6572 2820 2243 6163 6865 2d43  header( "Cache-C
-0000d850: 6f6e 7472 6f6c 222c 2022 6e6f 2d63 6163  ontrol", "no-cac
-0000d860: 6865 2220 290a 2020 2020 2020 2020 2020  he" ).          
-0000d870: 2020 2020 2020 7765 622e 6865 6164 6572        web.header
-0000d880: 2820 2243 6f6e 7465 6e74 2d54 7970 6522  ( "Content-Type"
-0000d890: 2c20 2274 6578 742f 6874 6d6c 2220 290a  , "text/html" ).
-0000d8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d8b0: 7265 7475 726e 2072 6573 706f 6e73 650a  return response.
-0000d8c0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000d8d0: 2263 6861 6e67 6522 2069 6e20 7765 622e  "change" in web.
-0000d8e0: 696e 7075 7428 293a 0a20 2020 2020 2020  input():.       
-0000d8f0: 2020 2020 2020 2020 2023 2050 6f73 7420           # Post 
-0000d900: 7669 6120 2263 6861 6e67 6522 2062 7574  via "change" but
-0000d910: 746f 6e2c 2061 6e64 2061 206e 6577 2050  ton, and a new P
-0000d920: 494e 2070 726f 7669 6465 643b 2075 7064  IN provided; upd
-0000d930: 6174 6520 7468 6520 7265 636f 7264 2066  ate the record f
-0000d940: 6f72 2074 6865 206c 6f67 6765 640a 2020  or the logged.  
-0000d950: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-0000d960: 696e 2075 7365 722f 5049 4e2c 2077 686f  in user/PIN, who
-0000d970: 206d 6179 2068 6176 6520 7365 7665 7261   may have severa
-0000d980: 6c20 7769 7468 2064 6966 6665 7265 6e74  l with different
-0000d990: 2050 494e 7320 616e 6420 6361 7061 6269   PINs and capabi
-0000d9a0: 6c69 7469 6573 2e0a 2020 2020 2020 2020  lities..        
-0000d9b0: 2020 2020 2020 2020 6572 726f 7209 093d          error..=
-0000d9c0: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
-0000d9d0: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-0000d9e0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-0000d9f0: 7373 6572 7420 6c6f 6767 6564 2829 2c20  ssert logged(), 
-0000da00: 224e 6f74 206c 6f67 6765 6420 696e 220a  "Not logged in".
-0000da10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000da20: 2020 2020 7069 6e09 093d 2077 6562 2e69      pin..= web.i
-0000da30: 6e70 7574 2829 2e67 6574 2820 2270 696e  nput().get( "pin
-0000da40: 2220 290a 2020 2020 2020 2020 2020 2020  " ).            
-0000da50: 2020 2020 2020 2020 6173 7365 7274 2070          assert p
-0000da60: 696e 2c20 2245 6d70 7479 2050 494e 220a  in, "Empty PIN".
-0000da70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000da80: 2020 2020 7769 7468 2064 625f 6c6f 636b      with db_lock
-0000da90: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000daa0: 2020 2020 2020 2020 2020 7175 6572 7909            query.
-0000dab0: 3d20 6462 2e75 7064 6174 6528 2027 7573  = db.update( 'us
-0000dac0: 6572 7327 2c20 7768 6572 653d 276e 616d  ers', where='nam
-0000dad0: 6520 3d20 246e 616d 6520 414e 4420 7069  e = $name AND pi
-0000dae0: 6e20 3d20 2470 696e 272c 0a20 2020 2020  n = $pin',.     
-0000daf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000db00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000db10: 2020 2020 2020 2020 7069 6e3d 7765 622e          pin=web.
-0000db20: 696e 7075 7428 292e 6765 7428 2027 7069  input().get( 'pi
-0000db30: 6e27 2029 2c0a 2020 2020 2020 2020 2020  n' ),.          
+0000d730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d740: 2255 7064 6174 6564 2055 7365 7220 2573  "Updated User %s
+0000d750: 2220 2520 2820 6e61 6d65 2029 0a20 2020  " % ( name ).   
+0000d760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d780: 2020 2020 2020 2069 6620 7570 6461 7465         if update
+0000d790: 2065 6c73 650a 2020 2020 2020 2020 2020   else.          
+0000d7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d7c0: 2241 6464 6564 2055 7365 7220 2573 2220  "Added User %s" 
+0000d7d0: 2520 2820 6e61 6d65 2029 292c 0a20 2020  % ( name )),.   
+0000d7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d7f0: 2020 2020 2022 7265 6469 7265 6374 223a       "redirect":
+0000d800: 0977 6562 2e69 6e70 7574 2829 2e67 6574  .web.input().get
+0000d810: 2820 2272 6564 6972 6563 7422 2c20 2222  ( "redirect", ""
+0000d820: 2029 2c0a 2020 2020 2020 2020 2020 2020   ),.            
+0000d830: 2020 2020 2020 2020 2020 2020 2263 6869              "chi
+0000d840: 6c64 7265 6e22 3a09 7573 6572 5f68 6572  ldren":.user_her
+0000d850: 6974 6167 6528 2073 6573 7369 6f6e 2e75  itage( session.u
+0000d860: 7365 725f 6964 2029 2c0a 2020 2020 2020  ser_id ),.      
+0000d870: 2020 2020 2020 2020 2020 2020 2020 7d29                })
+0000d880: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d890: 2077 6562 2e68 6561 6465 7228 2022 4361   web.header( "Ca
+0000d8a0: 6368 652d 436f 6e74 726f 6c22 2c20 226e  che-Control", "n
+0000d8b0: 6f2d 6361 6368 6522 2029 0a20 2020 2020  o-cache" ).     
+0000d8c0: 2020 2020 2020 2020 2020 2077 6562 2e68             web.h
+0000d8d0: 6561 6465 7228 2022 436f 6e74 656e 742d  eader( "Content-
+0000d8e0: 5479 7065 222c 2022 7465 7874 2f68 746d  Type", "text/htm
+0000d8f0: 6c22 2029 0a20 2020 2020 2020 2020 2020  l" ).           
+0000d900: 2020 2020 2072 6574 7572 6e20 7265 7370       return resp
+0000d910: 6f6e 7365 0a0a 2020 2020 2020 2020 2020  onse..          
+0000d920: 2020 6966 2022 6368 616e 6765 2220 696e    if "change" in
+0000d930: 2077 6562 2e69 6e70 7574 2829 3a0a 2020   web.input():.  
+0000d940: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+0000d950: 506f 7374 2076 6961 2022 6368 616e 6765  Post via "change
+0000d960: 2220 6275 7474 6f6e 2c20 616e 6420 6120  " button, and a 
+0000d970: 6e65 7720 5049 4e20 7072 6f76 6964 6564  new PIN provided
+0000d980: 3b20 7570 6461 7465 2074 6865 2072 6563  ; update the rec
+0000d990: 6f72 6420 666f 7220 7468 6520 6c6f 6767  ord for the logg
+0000d9a0: 6564 0a20 2020 2020 2020 2020 2020 2020  ed.             
+0000d9b0: 2020 2023 2069 6e20 7573 6572 2f50 494e     # in user/PIN
+0000d9c0: 2c20 7768 6f20 6d61 7920 6861 7665 2073  , who may have s
+0000d9d0: 6576 6572 616c 2077 6974 6820 6469 6666  everal with diff
+0000d9e0: 6572 656e 7420 5049 4e73 2061 6e64 2063  erent PINs and c
+0000d9f0: 6170 6162 696c 6974 6965 732e 0a20 2020  apabilities..   
+0000da00: 2020 2020 2020 2020 2020 2020 2065 7272               err
+0000da10: 6f72 0909 3d20 4e6f 6e65 0a20 2020 2020  or..= None.     
+0000da20: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
+0000da30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000da40: 2020 2020 6173 7365 7274 206c 6f67 6765      assert logge
+0000da50: 6428 292c 2022 4e6f 7420 6c6f 6767 6564  d(), "Not logged
+0000da60: 2069 6e22 0a20 2020 2020 2020 2020 2020   in".           
+0000da70: 2020 2020 2020 2020 2070 696e 0909 3d20           pin..= 
+0000da80: 7765 622e 696e 7075 7428 292e 6765 7428  web.input().get(
+0000da90: 2022 7069 6e22 2029 0a20 2020 2020 2020   "pin" ).       
+0000daa0: 2020 2020 2020 2020 2020 2020 2061 7373               ass
+0000dab0: 6572 7420 7069 6e2c 2022 456d 7074 7920  ert pin, "Empty 
+0000dac0: 5049 4e22 0a20 2020 2020 2020 2020 2020  PIN".           
+0000dad0: 2020 2020 2020 2020 2077 6974 6820 6462           with db
+0000dae0: 5f6c 6f63 6b3a 0a20 2020 2020 2020 2020  _lock:.         
+0000daf0: 2020 2020 2020 2020 2020 2020 2020 2071                 q
+0000db00: 7565 7279 093d 2064 622e 7570 6461 7465  uery.= db.update
+0000db10: 2820 2775 7365 7273 272c 2077 6865 7265  ( 'users', where
+0000db20: 3d27 6e61 6d65 203d 2024 6e61 6d65 2041  ='name = $name A
+0000db30: 4e44 2070 696e 203d 2024 7069 6e27 2c0a  ND pin = $pin',.
 0000db40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000db50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000db60: 2020 2076 6172 733d 7b0a 2020 2020 2020     vars={.      
-0000db70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000db80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000db90: 2020 2020 2020 2020 2020 2022 6e61 6d65             "name
-0000dba0: 223a 2073 6573 7369 6f6e 2e6e 616d 652e  ": session.name.
-0000dbb0: 6c6f 7765 7228 292c 0a20 2020 2020 2020  lower(),.       
+0000db60: 2020 2020 2020 2020 2020 2020 2070 696e               pin
+0000db70: 3d77 6562 2e69 6e70 7574 2829 2e67 6574  =web.input().get
+0000db80: 2820 2770 696e 2720 292c 0a20 2020 2020  ( 'pin' ),.     
+0000db90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dbb0: 2020 2020 2020 2020 7661 7273 3d7b 0a20          vars={. 
 0000dbc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000dbd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dbe0: 2020 2020 2020 2020 2020 2270 696e 223a            "pin":
-0000dbf0: 2073 6573 7369 6f6e 2e70 696e 2c0a 2020   session.pin,.  
-0000dc00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dbf0: 226e 616d 6522 3a20 7365 7373 696f 6e2e  "name": session.
+0000dc00: 6e61 6d65 2e6c 6f77 6572 2829 2c0a 2020  name.lower(),.  
 0000dc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc20: 2020 2020 2020 2020 2020 207d 290a 2020             }).  
-0000dc30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc40: 2020 6173 7365 7274 2071 7565 7279 2c20    assert query, 
-0000dc50: 2255 7064 6174 6520 6661 696c 6564 3a20  "Update failed: 
-0000dc60: 2572 2220 2520 2820 7175 6572 7920 290a  %r" % ( query ).
+0000dc20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dc30: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0000dc40: 7069 6e22 3a20 7365 7373 696f 6e2e 7069  pin": session.pi
+0000dc50: 6e2c 0a20 2020 2020 2020 2020 2020 2020  n,.             
+0000dc60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000dc70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc80: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
-0000dc90: 2061 7320 6578 633a 0a20 2020 2020 2020   as exc:.       
-0000dca0: 2020 2020 2020 2020 2020 2020 206c 6f67               log
-0000dcb0: 6769 6e67 2e69 6e66 6f28 2022 5049 4e20  ging.info( "PIN 
-0000dcc0: 6368 616e 6765 2066 6169 6c75 7265 3a20  change failure: 
-0000dcd0: 2573 3a20 2573 2220 2520 2820 6578 632c  %s: %s" % ( exc,
-0000dce0: 2074 7261 6365 6261 636b 2e66 6f72 6d61   traceback.forma
-0000dcf0: 745f 6578 6328 2920 2929 0a20 2020 2020  t_exc() )).     
-0000dd00: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0000dd10: 7272 6f72 093d 2073 7472 2820 6578 6320  rror.= str( exc 
-0000dd20: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000dd30: 2020 7265 7370 6f6e 7365 093d 2072 656e    response.= ren
-0000dd40: 6465 722e 6c6f 6769 6e28 0a20 2020 2020  der.login(.     
-0000dd50: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-0000dd60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000dd70: 2020 2020 2020 2020 2022 7469 746c 6522           "title"
-0000dd80: 3a09 2820 2250 494e 2043 6861 6e67 6564  :.( "PIN Changed
-0000dd90: 2066 6f72 2025 7322 2025 2028 2073 6573   for %s" % ( ses
-0000dda0: 7369 6f6e 2e6e 616d 6520 290a 2020 2020  sion.name ).    
-0000ddb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ddc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ddd0: 2020 2020 2020 6966 206e 6f74 2065 7272        if not err
-0000dde0: 6f72 2065 6c73 650a 2020 2020 2020 2020  or else.        
-0000ddf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000de00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000de10: 2020 2250 494e 2043 6861 6e67 6520 4661    "PIN Change Fa
-0000de20: 696c 6564 3a20 2573 2220 2520 2820 6572  iled: %s" % ( er
-0000de30: 726f 7220 2929 2c0a 2020 2020 2020 2020  ror )),.        
+0000dc80: 7d29 0a20 2020 2020 2020 2020 2020 2020  }).             
+0000dc90: 2020 2020 2020 2061 7373 6572 7420 7175         assert qu
+0000dca0: 6572 792c 2022 5570 6461 7465 2066 6169  ery, "Update fai
+0000dcb0: 6c65 643a 2025 7222 2025 2028 2071 7565  led: %r" % ( que
+0000dcc0: 7279 2029 0a20 2020 2020 2020 2020 2020  ry ).           
+0000dcd0: 2020 2020 2065 7863 6570 7420 4578 6365       except Exce
+0000dce0: 7074 696f 6e20 6173 2065 7863 3a0a 2020  ption as exc:.  
+0000dcf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dd00: 2020 6c6f 6767 696e 672e 696e 666f 2820    logging.info( 
+0000dd10: 2250 494e 2063 6861 6e67 6520 6661 696c  "PIN change fail
+0000dd20: 7572 653a 2025 733a 2025 7322 2025 2028  ure: %s: %s" % (
+0000dd30: 2065 7863 2c20 7472 6163 6562 6163 6b2e   exc, traceback.
+0000dd40: 666f 726d 6174 5f65 7863 2829 2029 290a  format_exc() )).
+0000dd50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dd60: 2020 2020 6572 726f 7209 3d20 7374 7228      error.= str(
+0000dd70: 2065 7863 2029 0a20 2020 2020 2020 2020   exc ).         
+0000dd80: 2020 2020 2020 2072 6573 706f 6e73 6509         response.
+0000dd90: 3d20 7265 6e64 6572 2e6c 6f67 696e 280a  = render.login(.
+0000dda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ddb0: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
+0000ddc0: 2020 2020 2020 2020 2020 2020 2020 2274                "t
+0000ddd0: 6974 6c65 223a 0928 2022 5049 4e20 4368  itle":.( "PIN Ch
+0000dde0: 616e 6765 6420 666f 7220 2573 2220 2520  anged for %s" % 
+0000ddf0: 2820 7365 7373 696f 6e2e 6e61 6d65 2029  ( session.name )
+0000de00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000de10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000de20: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+0000de30: 7420 6572 726f 7220 656c 7365 0a20 2020  t error else.   
 0000de40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000de50: 2272 6564 6972 6563 7422 3a09 7765 622e  "redirect":.web.
-0000de60: 696e 7075 7428 292e 6765 7428 2022 7265  input().get( "re
-0000de70: 6469 7265 6374 222c 2022 2220 292c 0a20  direct", "" ),. 
-0000de80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000de90: 2020 2020 2020 2022 6368 696c 6472 656e         "children
-0000dea0: 223a 0975 7365 725f 6865 7269 7461 6765  ":.user_heritage
-0000deb0: 2820 7365 7373 696f 6e2e 7573 6572 5f69  ( session.user_i
-0000dec0: 6420 292c 0a20 2020 2020 2020 2020 2020  d ),.           
-0000ded0: 2020 2020 2020 2020 207d 290a 2020 2020           }).    
-0000dee0: 2020 2020 2020 2020 2020 2020 7765 622e              web.
-0000def0: 6865 6164 6572 2820 2243 6163 6865 2d43  header( "Cache-C
-0000df00: 6f6e 7472 6f6c 222c 2022 6e6f 2d63 6163  ontrol", "no-cac
-0000df10: 6865 2220 290a 2020 2020 2020 2020 2020  he" ).          
-0000df20: 2020 2020 2020 7765 622e 6865 6164 6572        web.header
-0000df30: 2820 2243 6f6e 7465 6e74 2d54 7970 6522  ( "Content-Type"
-0000df40: 2c20 2274 6578 742f 6874 6d6c 2220 290a  , "text/html" ).
-0000df50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000df60: 7265 7475 726e 2072 6573 706f 6e73 650a  return response.
-0000df70: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000df80: 2264 656c 6574 6522 2069 6e20 7765 622e  "delete" in web.
-0000df90: 696e 7075 7428 293a 0a20 2020 2020 2020  input():.       
-0000dfa0: 2020 2020 2020 2020 2023 2044 656c 6574           # Delet
-0000dfb0: 6520 7573 6572 732e 2020 5765 2063 616e  e users.  We can
-0000dfc0: 206f 6e6c 7920 6465 6c65 7465 2075 7365   only delete use
-0000dfd0: 7273 2077 6527 7665 2063 7265 6174 6564  rs we've created
-0000dfe0: 2e20 2047 6574 206f 7572 2075 7365 7220  .  Get our user 
-0000dff0: 6865 7269 7461 6765 2c20 616e 640a 2020  heritage, and.  
-0000e000: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-0000e010: 7365 6520 6966 206d 6174 6368 696e 6720  see if matching 
-0000e020: 2264 656c 6574 652d 3c75 7365 723e 2d3c  "delete-<user>-<
-0000e030: 7573 6572 5f69 643e 2220 6368 6563 6b62  user_id>" checkb
-0000e040: 6f78 6573 2073 686f 7720 7570 2069 6e20  oxes show up in 
-0000e050: 7468 6520 666f 726d 2e0a 2020 2020 2020  the form..      
-0000e060: 2020 2020 2020 2020 2020 6572 726f 7209            error.
-0000e070: 093d 204e 6f6e 650a 2020 2020 2020 2020  .= None.        
-0000e080: 2020 2020 2020 2020 7265 6d6f 7665 6409          removed.
-0000e090: 093d 205b 5d0a 2020 2020 2020 2020 2020  .= [].          
-0000e0a0: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-0000e0b0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-0000e0c0: 7373 6572 7420 6c6f 6767 6564 2829 2c20  ssert logged(), 
-0000e0d0: 224e 6f74 206c 6f67 6765 6420 696e 220a  "Not logged in".
-0000e0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e0f0: 2020 2020 2320 5b28 286e 616d 652c 7573      # [((name,us
-0000e100: 6572 5f69 6429 2c7b 2e2e 2e7d 292c 202e  er_id),{...}), .
-0000e110: 2e2e 5d0a 2020 2020 2020 2020 2020 2020  ..].            
-0000e120: 2020 2020 2020 2020 6576 616c 7561 7465          evaluate
-0000e130: 093d 2075 7365 725f 6865 7269 7461 6765  .= user_heritage
-0000e140: 2820 7365 7373 696f 6e2e 7573 6572 5f69  ( session.user_i
-0000e150: 6420 292e 6974 656d 7328 290a 2020 2020  d ).items().    
-0000e160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e170: 6578 7465 726d 696e 6174 6509 3d20 5b5d  exterminate.= []
-0000e180: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e190: 2020 2020 2077 6869 6c65 2065 7661 6c75       while evalu
-0000e1a0: 6174 653a 0a20 2020 2020 2020 2020 2020  ate:.           
-0000e1b0: 2020 2020 2020 2020 2020 2020 2069 7465               ite
-0000e1c0: 6d09 093d 2065 7661 6c75 6174 652e 706f  m..= evaluate.po
-0000e1d0: 7028 290a 2020 2020 2020 2020 2020 2020  p().            
-0000e1e0: 2020 2020 2020 2020 2020 2020 286e 616d              (nam
-0000e1f0: 652c 7569 6429 2c73 7562 7309 3d20 6974  e,uid),subs.= it
-0000e200: 656d 0a20 2020 2020 2020 2020 2020 2020  em.             
-0000e210: 2020 2020 2020 2020 2020 2063 6865 636b             check
-0000e220: 626f 7809 3d20 2264 656c 6574 652d 2573  box.= "delete-%s
-0000e230: 2d25 7322 2025 2028 206e 616d 652c 2075  -%s" % ( name, u
-0000e240: 6964 2029 0a20 2020 2020 2020 2020 2020  id ).           
-0000e250: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000e260: 6368 6563 6b62 6f78 2069 6e20 7765 622e  checkbox in web.
-0000e270: 696e 7075 7428 293a 0a20 2020 2020 2020  input():.       
-0000e280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e290: 2020 2020 2023 2059 7570 3b20 7468 6973       # Yup; this
-0000e2a0: 2028 616e 6420 616c 6c20 7468 6569 7220   (and all their 
-0000e2b0: 6b69 6473 2920 6172 6520 676f 6e65 2e0a  kids) are gone..
-0000e2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e2d0: 2020 2020 2020 2020 2020 2020 6578 7465              exte
-0000e2e0: 726d 696e 6174 652e 6170 7065 6e64 2820  rminate.append( 
-0000e2f0: 6974 656d 2029 0a20 2020 2020 2020 2020  item ).         
-0000e300: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0000e310: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0000de50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000de60: 2020 2020 2020 2022 5049 4e20 4368 616e         "PIN Chan
+0000de70: 6765 2046 6169 6c65 643a 2025 7322 2025  ge Failed: %s" %
+0000de80: 2028 2065 7272 6f72 2029 292c 0a20 2020   ( error )),.   
+0000de90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dea0: 2020 2020 2022 7265 6469 7265 6374 223a       "redirect":
+0000deb0: 0977 6562 2e69 6e70 7574 2829 2e67 6574  .web.input().get
+0000dec0: 2820 2272 6564 6972 6563 7422 2c20 2222  ( "redirect", ""
+0000ded0: 2029 2c0a 2020 2020 2020 2020 2020 2020   ),.            
+0000dee0: 2020 2020 2020 2020 2020 2020 2263 6869              "chi
+0000def0: 6c64 7265 6e22 3a09 7573 6572 5f68 6572  ldren":.user_her
+0000df00: 6974 6167 6528 2073 6573 7369 6f6e 2e75  itage( session.u
+0000df10: 7365 725f 6964 2029 2c0a 2020 2020 2020  ser_id ),.      
+0000df20: 2020 2020 2020 2020 2020 2020 2020 7d29                })
+0000df30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000df40: 2077 6562 2e68 6561 6465 7228 2022 4361   web.header( "Ca
+0000df50: 6368 652d 436f 6e74 726f 6c22 2c20 226e  che-Control", "n
+0000df60: 6f2d 6361 6368 6522 2029 0a20 2020 2020  o-cache" ).     
+0000df70: 2020 2020 2020 2020 2020 2077 6562 2e68             web.h
+0000df80: 6561 6465 7228 2022 436f 6e74 656e 742d  eader( "Content-
+0000df90: 5479 7065 222c 2022 7465 7874 2f68 746d  Type", "text/htm
+0000dfa0: 6c22 2029 0a20 2020 2020 2020 2020 2020  l" ).           
+0000dfb0: 2020 2020 2072 6574 7572 6e20 7265 7370       return resp
+0000dfc0: 6f6e 7365 0a0a 2020 2020 2020 2020 2020  onse..          
+0000dfd0: 2020 6966 2022 6465 6c65 7465 2220 696e    if "delete" in
+0000dfe0: 2077 6562 2e69 6e70 7574 2829 3a0a 2020   web.input():.  
+0000dff0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+0000e000: 4465 6c65 7465 2075 7365 7273 2e20 2057  Delete users.  W
+0000e010: 6520 6361 6e20 6f6e 6c79 2064 656c 6574  e can only delet
+0000e020: 6520 7573 6572 7320 7765 2776 6520 6372  e users we've cr
+0000e030: 6561 7465 642e 2020 4765 7420 6f75 7220  eated.  Get our 
+0000e040: 7573 6572 2068 6572 6974 6167 652c 2061  user heritage, a
+0000e050: 6e64 0a20 2020 2020 2020 2020 2020 2020  nd.             
+0000e060: 2020 2023 2073 6565 2069 6620 6d61 7463     # see if matc
+0000e070: 6869 6e67 2022 6465 6c65 7465 2d3c 7573  hing "delete-<us
+0000e080: 6572 3e2d 3c75 7365 725f 6964 3e22 2063  er>-<user_id>" c
+0000e090: 6865 636b 626f 7865 7320 7368 6f77 2075  heckboxes show u
+0000e0a0: 7020 696e 2074 6865 2066 6f72 6d2e 0a20  p in the form.. 
+0000e0b0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+0000e0c0: 7272 6f72 0909 3d20 4e6f 6e65 0a20 2020  rror..= None.   
+0000e0d0: 2020 2020 2020 2020 2020 2020 2072 656d               rem
+0000e0e0: 6f76 6564 0909 3d20 5b5d 0a20 2020 2020  oved..= [].     
+0000e0f0: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
+0000e100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e110: 2020 2020 6173 7365 7274 206c 6f67 6765      assert logge
+0000e120: 6428 292c 2022 4e6f 7420 6c6f 6767 6564  d(), "Not logged
+0000e130: 2069 6e22 0a20 2020 2020 2020 2020 2020   in".           
+0000e140: 2020 2020 2020 2020 2023 205b 2828 6e61           # [((na
+0000e150: 6d65 2c75 7365 725f 6964 292c 7b2e 2e2e  me,user_id),{...
+0000e160: 7d29 2c20 2e2e 2e5d 0a20 2020 2020 2020  }), ...].       
+0000e170: 2020 2020 2020 2020 2020 2020 2065 7661               eva
+0000e180: 6c75 6174 6509 3d20 7573 6572 5f68 6572  luate.= user_her
+0000e190: 6974 6167 6528 2073 6573 7369 6f6e 2e75  itage( session.u
+0000e1a0: 7365 725f 6964 2029 2e69 7465 6d73 2829  ser_id ).items()
+0000e1b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e1c0: 2020 2020 2065 7874 6572 6d69 6e61 7465       exterminate
+0000e1d0: 093d 205b 5d0a 2020 2020 2020 2020 2020  .= [].          
+0000e1e0: 2020 2020 2020 2020 2020 7768 696c 6520            while 
+0000e1f0: 6576 616c 7561 7465 3a0a 2020 2020 2020  evaluate:.      
+0000e200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e210: 2020 6974 656d 0909 3d20 6576 616c 7561    item..= evalua
+0000e220: 7465 2e70 6f70 2829 0a20 2020 2020 2020  te.pop().       
+0000e230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e240: 2028 6e61 6d65 2c75 6964 292c 7375 6273   (name,uid),subs
+0000e250: 093d 2069 7465 6d0a 2020 2020 2020 2020  .= item.        
+0000e260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e270: 6368 6563 6b62 6f78 093d 2022 6465 6c65  checkbox.= "dele
+0000e280: 7465 2d25 732d 2573 2220 2520 2820 6e61  te-%s-%s" % ( na
+0000e290: 6d65 2c20 7569 6420 290a 2020 2020 2020  me, uid ).      
+0000e2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e2b0: 2020 6966 2063 6865 636b 626f 7820 696e    if checkbox in
+0000e2c0: 2077 6562 2e69 6e70 7574 2829 3a0a 2020   web.input():.  
+0000e2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e2e0: 2020 2020 2020 2020 2020 2320 5975 703b            # Yup;
+0000e2f0: 2074 6869 7320 2861 6e64 2061 6c6c 2074   this (and all t
+0000e300: 6865 6972 206b 6964 7329 2061 7265 2067  heir kids) are g
+0000e310: 6f6e 652e 0a20 2020 2020 2020 2020 2020  one..           
 0000e320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e330: 2023 204e 6f74 2064 656c 6574 696e 6720   # Not deleting 
-0000e340: 7468 6973 2075 7365 723b 2070 6572 6861  this user; perha
-0000e350: 7073 206f 6e65 206f 6620 7468 6569 7220  ps one of their 
-0000e360: 7375 622d 7573 6572 733f 0a20 2020 2020  sub-users?.     
+0000e330: 2065 7874 6572 6d69 6e61 7465 2e61 7070   exterminate.app
+0000e340: 656e 6428 2069 7465 6d20 290a 2020 2020  end( item ).    
+0000e350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e360: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
 0000e370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e380: 2020 2020 2020 2065 7661 6c75 6174 6520         evaluate 
-0000e390: 2020 2b3d 2073 7562 732e 6974 656d 7328    += subs.items(
-0000e3a0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000e3b0: 2020 2020 2020 7768 696c 6520 6578 7465        while exte
-0000e3c0: 726d 696e 6174 653a 0a20 2020 2020 2020  rminate:.       
-0000e3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e3e0: 2069 7465 6d09 093d 2065 7874 6572 6d69   item..= extermi
-0000e3f0: 6e61 7465 2e70 6f70 2829 0a20 2020 2020  nate.pop().     
-0000e400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e410: 2020 2028 6e61 6d65 2c75 6964 292c 7375     (name,uid),su
-0000e420: 6273 093d 2069 7465 6d0a 2020 2020 2020  bs.= item.      
-0000e430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e440: 2020 6578 7465 726d 696e 6174 6520 2020    exterminate   
-0000e450: 202b 3d20 7375 6273 2e69 7465 6d73 2829   += subs.items()
-0000e460: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e470: 2020 2020 2020 2020 206c 6f67 6769 6e67           logging
-0000e480: 2e77 6172 6e69 6e67 2822 4465 6c65 7465  .warning("Delete
-0000e490: 2075 7365 7220 2573 2028 2573 2922 2025   user %s (%s)" %
-0000e4a0: 2028 206e 616d 652c 2075 6964 2029 290a   ( name, uid )).
-0000e4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e4c0: 2020 2020 2020 2020 7769 7468 2064 625f          with db_
-0000e4d0: 6c6f 636b 3a0a 2020 2020 2020 2020 2020  lock:.          
-0000e4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e4f0: 2020 6462 2e64 656c 6574 6528 2027 7573    db.delete( 'us
-0000e500: 6572 7327 2c20 7768 6572 653d 2775 7365  ers', where='use
-0000e510: 725f 6964 203d 2024 7573 6572 5f69 6427  r_id = $user_id'
-0000e520: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000e380: 2020 2020 2020 2320 4e6f 7420 6465 6c65        # Not dele
+0000e390: 7469 6e67 2074 6869 7320 7573 6572 3b20  ting this user; 
+0000e3a0: 7065 7268 6170 7320 6f6e 6520 6f66 2074  perhaps one of t
+0000e3b0: 6865 6972 2073 7562 2d75 7365 7273 3f0a  heir sub-users?.
+0000e3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e3d0: 2020 2020 2020 2020 2020 2020 6576 616c              eval
+0000e3e0: 7561 7465 2020 202b 3d20 7375 6273 2e69  uate   += subs.i
+0000e3f0: 7465 6d73 2829 0a20 2020 2020 2020 2020  tems().         
+0000e400: 2020 2020 2020 2020 2020 2077 6869 6c65             while
+0000e410: 2065 7874 6572 6d69 6e61 7465 3a0a 2020   exterminate:.  
+0000e420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e430: 2020 2020 2020 6974 656d 0909 3d20 6578        item..= ex
+0000e440: 7465 726d 696e 6174 652e 706f 7028 290a  terminate.pop().
+0000e450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e460: 2020 2020 2020 2020 286e 616d 652c 7569          (name,ui
+0000e470: 6429 2c73 7562 7309 3d20 6974 656d 0a20  d),subs.= item. 
+0000e480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e490: 2020 2020 2020 2065 7874 6572 6d69 6e61         extermina
+0000e4a0: 7465 2020 2020 2b3d 2073 7562 732e 6974  te    += subs.it
+0000e4b0: 656d 7328 290a 2020 2020 2020 2020 2020  ems().          
+0000e4c0: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+0000e4d0: 6767 696e 672e 7761 726e 696e 6728 2244  gging.warning("D
+0000e4e0: 656c 6574 6520 7573 6572 2025 7320 2825  elete user %s (%
+0000e4f0: 7329 2220 2520 2820 6e61 6d65 2c20 7569  s)" % ( name, ui
+0000e500: 6420 2929 0a20 2020 2020 2020 2020 2020  d )).           
+0000e510: 2020 2020 2020 2020 2020 2020 2077 6974               wit
+0000e520: 6820 6462 5f6c 6f63 6b3a 0a20 2020 2020  h db_lock:.     
 0000e530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e540: 2020 2020 2020 2020 2076 6172 733d 7b0a           vars={.
-0000e550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e570: 2020 2020 2020 2020 2020 2022 7573 6572             "user
-0000e580: 5f69 6422 3a20 7569 642c 0a20 2020 2020  _id": uid,.     
-0000e590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e5b0: 2020 7d29 0a20 2020 2020 2020 2020 2020    }).           
-0000e5c0: 2020 2020 2020 2020 2020 2020 2072 656d               rem
-0000e5d0: 6f76 6564 2e61 7070 656e 6428 206e 616d  oved.append( nam
-0000e5e0: 6520 290a 0a20 2020 2020 2020 2020 2020  e )..           
-0000e5f0: 2020 2020 2065 7863 6570 7420 4578 6365       except Exce
-0000e600: 7074 696f 6e20 6173 2065 7863 3a0a 2020  ption as exc:.  
+0000e540: 2020 2020 2020 2064 622e 6465 6c65 7465         db.delete
+0000e550: 2820 2775 7365 7273 272c 2077 6865 7265  ( 'users', where
+0000e560: 3d27 7573 6572 5f69 6420 3d20 2475 7365  ='user_id = $use
+0000e570: 725f 6964 272c 0a20 2020 2020 2020 2020  r_id',.         
+0000e580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e590: 2020 2020 2020 2020 2020 2020 2020 7661                va
+0000e5a0: 7273 3d7b 0a20 2020 2020 2020 2020 2020  rs={.           
+0000e5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e5d0: 2275 7365 725f 6964 223a 2075 6964 2c0a  "user_id": uid,.
+0000e5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e600: 2020 2020 2020 207d 290a 2020 2020 2020         }).      
 0000e610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e620: 2020 6c6f 6767 696e 672e 696e 666f 2820    logging.info( 
-0000e630: 2244 656c 6574 6520 7573 6572 2066 6169  "Delete user fai
-0000e640: 6c75 7265 3a20 2573 3a20 2573 2220 2520  lure: %s: %s" % 
-0000e650: 2820 6578 632c 2074 7261 6365 6261 636b  ( exc, traceback
-0000e660: 2e66 6f72 6d61 745f 6578 6328 2920 2929  .format_exc() ))
-0000e670: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e680: 2020 2020 2065 7272 6f72 093d 2073 7472       error.= str
-0000e690: 2820 6578 6320 290a 2020 2020 2020 2020  ( exc ).        
-0000e6a0: 2020 2020 2020 2020 7265 6d6f 7665 6409          removed.
-0000e6b0: 093d 2022 2c20 222e 6a6f 696e 2820 7374  .= ", ".join( st
-0000e6c0: 7228 7529 2066 6f72 2075 2069 6e20 7265  r(u) for u in re
-0000e6d0: 6d6f 7665 6420 2920 6966 2072 656d 6f76  moved ) if remov
-0000e6e0: 6564 2065 6c73 6520 226e 6f62 6f64 7922  ed else "nobody"
-0000e6f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e700: 2072 6573 706f 6e73 6509 3d20 7265 6e64   response.= rend
-0000e710: 6572 2e6c 6f67 696e 280a 2020 2020 2020  er.login(.      
-0000e720: 2020 2020 2020 2020 2020 2020 2020 7b0a                {.
-0000e730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e740: 2020 2020 2020 2020 2274 6974 6c65 223a          "title":
-0000e750: 0928 2022 4465 6c65 7465 6420 2573 2220  .( "Deleted %s" 
-0000e760: 2520 2820 7265 6d6f 7665 6420 290a 2020  % ( removed ).  
+0000e620: 2020 7265 6d6f 7665 642e 6170 7065 6e64    removed.append
+0000e630: 2820 6e61 6d65 2029 0a0a 2020 2020 2020  ( name )..      
+0000e640: 2020 2020 2020 2020 2020 6578 6365 7074            except
+0000e650: 2045 7863 6570 7469 6f6e 2061 7320 6578   Exception as ex
+0000e660: 633a 0a20 2020 2020 2020 2020 2020 2020  c:.             
+0000e670: 2020 2020 2020 206c 6f67 6769 6e67 2e69         logging.i
+0000e680: 6e66 6f28 2022 4465 6c65 7465 2075 7365  nfo( "Delete use
+0000e690: 7220 6661 696c 7572 653a 2025 733a 2025  r failure: %s: %
+0000e6a0: 7322 2025 2028 2065 7863 2c20 7472 6163  s" % ( exc, trac
+0000e6b0: 6562 6163 6b2e 666f 726d 6174 5f65 7863  eback.format_exc
+0000e6c0: 2829 2029 290a 2020 2020 2020 2020 2020  () )).          
+0000e6d0: 2020 2020 2020 2020 2020 6572 726f 7209            error.
+0000e6e0: 3d20 7374 7228 2065 7863 2029 0a20 2020  = str( exc ).   
+0000e6f0: 2020 2020 2020 2020 2020 2020 2072 656d               rem
+0000e700: 6f76 6564 0909 3d20 222c 2022 2e6a 6f69  oved..= ", ".joi
+0000e710: 6e28 2073 7472 2875 2920 666f 7220 7520  n( str(u) for u 
+0000e720: 696e 2072 656d 6f76 6564 2029 2069 6620  in removed ) if 
+0000e730: 7265 6d6f 7665 6420 656c 7365 2022 6e6f  removed else "no
+0000e740: 626f 6479 220a 2020 2020 2020 2020 2020  body".          
+0000e750: 2020 2020 2020 7265 7370 6f6e 7365 093d        response.=
+0000e760: 2072 656e 6465 722e 6c6f 6769 6e28 0a20   render.login(. 
 0000e770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e790: 2020 2020 2020 2020 6966 206e 6f74 2065          if not e
-0000e7a0: 7272 6f72 2065 6c73 650a 2020 2020 2020  rror else.      
-0000e7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e7d0: 2020 2020 2244 656c 6574 6564 2025 733b      "Deleted %s;
-0000e7e0: 2046 6169 6c65 643a 2025 7322 2025 2028   Failed: %s" % (
-0000e7f0: 2072 656d 6f76 6564 2c20 6572 726f 7220   removed, error 
-0000e800: 2929 2c0a 2020 2020 2020 2020 2020 2020  )),.            
-0000e810: 2020 2020 2020 2020 2020 2020 2272 6564              "red
-0000e820: 6972 6563 7422 3a09 7765 622e 696e 7075  irect":.web.inpu
-0000e830: 7428 292e 6765 7428 2022 7265 6469 7265  t().get( "redire
-0000e840: 6374 222c 2022 2220 292c 0a20 2020 2020  ct", "" ),.     
-0000e850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e860: 2020 2022 6368 696c 6472 656e 223a 0975     "children":.u
-0000e870: 7365 725f 6865 7269 7461 6765 2820 7365  ser_heritage( se
-0000e880: 7373 696f 6e2e 7573 6572 5f69 6420 292c  ssion.user_id ),
-0000e890: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e8a0: 2020 2020 207d 290a 2020 2020 2020 2020       }).        
-0000e8b0: 2020 2020 2020 2020 7765 622e 6865 6164          web.head
-0000e8c0: 6572 2820 2243 6163 6865 2d43 6f6e 7472  er( "Cache-Contr
-0000e8d0: 6f6c 222c 2022 6e6f 2d63 6163 6865 2220  ol", "no-cache" 
-0000e8e0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000e8f0: 2020 7765 622e 6865 6164 6572 2820 2243    web.header( "C
-0000e900: 6f6e 7465 6e74 2d54 7970 6522 2c20 2274  ontent-Type", "t
-0000e910: 6578 742f 6874 6d6c 2220 290a 2020 2020  ext/html" ).    
-0000e920: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000e930: 726e 2072 6573 706f 6e73 650a 0a20 2020  rn response..   
-0000e940: 2020 2020 2020 2020 2023 2050 6f73 7420           # Post 
-0000e950: 7669 6120 2267 6f22 2062 7574 746f 6e20  via "go" button 
-0000e960: 286f 7220 7669 6120 6576 656e 7420 6f6e  (or via event on
-0000e970: 2050 494e 2069 6e70 7574 293b 2061 7474   PIN input); att
-0000e980: 656d 7074 2074 6f20 6c6f 6769 6e0a 2020  empt to login.  
-0000e990: 2020 2020 2020 2020 2020 6964 656e 7409            ident.
-0000e9a0: 093d 204e 6f6e 650a 2020 2020 2020 2020  .= None.        
-0000e9b0: 2020 2020 6572 726f 7209 093d 204e 6f6e      error..= Non
-0000e9c0: 650a 2020 2020 2020 2020 2020 2020 7472  e.            tr
-0000e9d0: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
-0000e9e0: 2020 206e 616d 6509 093d 2077 6562 2e69     name..= web.i
-0000e9f0: 6e70 7574 2829 2e67 6574 2820 226e 616d  nput().get( "nam
-0000ea00: 6522 2029 0a20 2020 2020 2020 2020 2020  e" ).           
-0000ea10: 2020 2020 2070 696e 0909 3d20 7765 622e       pin..= web.
-0000ea20: 696e 7075 7428 292e 6765 7428 2022 7069  input().get( "pi
-0000ea30: 6e22 2029 0a20 2020 2020 2020 2020 2020  n" ).           
-0000ea40: 2020 2020 2061 7373 6572 7420 6e61 6d65       assert name
-0000ea50: 2061 6e64 2070 696e 2c20 2249 6e76 616c   and pin, "Inval
-0000ea60: 6964 2075 7365 722f 5049 4e22 0a20 2020  id user/PIN".   
-0000ea70: 2020 2020 2020 2020 2020 2020 2071 7565               que
-0000ea80: 7279 0909 3d20 6462 2e73 656c 6563 7428  ry..= db.select(
-0000ea90: 2027 7573 6572 7327 2c20 7768 6572 653d   'users', where=
-0000eaa0: 276e 616d 653d 246e 616d 6527 2c20 7661  'name=$name', va
-0000eab0: 7273 3d7b 226e 616d 6522 3a20 6e61 6d65  rs={"name": name
-0000eac0: 2e73 7472 6970 2829 2e6c 6f77 6572 2829  .strip().lower()
-0000ead0: 7d20 290a 2020 2020 2020 2020 2020 2020  } ).            
-0000eae0: 2020 2020 6173 7365 7274 2071 7565 7279      assert query
-0000eaf0: 2c20 2255 7365 7220 6e6f 7420 666f 756e  , "User not foun
-0000eb00: 643a 2025 7222 2025 2028 2071 7565 7279  d: %r" % ( query
-0000eb10: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-0000eb20: 2020 2066 6f72 2069 2069 6e20 7175 6572     for i in quer
-0000eb30: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
-0000eb40: 2020 2020 2020 206c 6f67 6769 6e67 2e69         logging.i
-0000eb50: 6e66 6f28 2022 6e61 6d65 3a20 2572 2076  nfo( "name: %r v
-0000eb60: 732e 2025 722c 2070 696e 3a20 2572 2076  s. %r, pin: %r v
-0000eb70: 7320 2572 2220 2520 2820 695b 276e 616d  s %r" % ( i['nam
-0000eb80: 6527 5d2c 206e 616d 652c 2069 5b27 7069  e'], name, i['pi
-0000eb90: 6e27 5d2c 2070 696e 2029 290a 2020 2020  n'], pin )).    
-0000eba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ebb0: 6966 2069 5b27 7069 6e27 5d20 3d3d 2069  if i['pin'] == i
-0000ebc0: 6e74 2820 7069 6e20 293a 0a20 2020 2020  nt( pin ):.     
-0000ebd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ebe0: 2020 2069 6465 6e74 093d 2069 0a20 2020     ident.= i.   
-0000ebf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ec00: 2020 2020 2062 7265 616b 0a20 2020 2020       break.     
-0000ec10: 2020 2020 2020 2020 2020 2061 7373 6572             asser
-0000ec20: 7420 6964 656e 742c 2022 556e 7265 636f  t ident, "Unreco
-0000ec30: 676e 697a 6564 2075 7365 722f 5049 4e22  gnized user/PIN"
-0000ec40: 0a20 2020 2020 2020 2020 2020 2065 7863  .            exc
-0000ec50: 6570 7420 4578 6365 7074 696f 6e20 6173  ept Exception as
-0000ec60: 2065 7863 3a0a 2020 2020 2020 2020 2020   exc:.          
-0000ec70: 2020 2020 2020 6c6f 6767 696e 672e 7761        logging.wa
-0000ec80: 726e 696e 6728 2022 4c6f 6769 6e20 6661  rning( "Login fa
-0000ec90: 696c 6564 3a20 6e61 6d65 3a20 2572 2c20  iled: name: %r, 
-0000eca0: 7069 6e3a 2025 723a 2025 733a 2025 7322  pin: %r: %s: %s"
-0000ecb0: 2025 2028 206e 616d 652c 2070 696e 2c20   % ( name, pin, 
-0000ecc0: 6578 632c 2074 7261 6365 6261 636b 2e66  exc, traceback.f
-0000ecd0: 6f72 6d61 745f 6578 6328 2920 2929 0a20  ormat_exc() )). 
-0000ece0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0000ecf0: 7272 6f72 0909 3d20 7374 7228 2065 7863  rror..= str( exc
-0000ed00: 2029 0a20 2020 2020 2020 2020 2020 2069   ).            i
-0000ed10: 6620 6964 656e 743a 0a20 2020 2020 2020  f ident:.       
-0000ed20: 2020 2020 2020 2020 206c 6f67 6769 6e67           logging
-0000ed30: 2e69 6e66 6f28 2022 4c6f 6769 6e20 6964  .info( "Login id
-0000ed40: 656e 743a 2020 2025 7222 2025 2028 2069  ent:   %r" % ( i
-0000ed50: 6465 6e74 2e69 7465 6d73 2829 2029 290a  dent.items() )).
-0000ed60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ed70: 7365 7373 696f 6e2e 7570 6461 7465 2820  session.update( 
-0000ed80: 6964 656e 7420 290a 2020 2020 2020 2020  ident ).        
-0000ed90: 2020 2020 2020 2020 6c6f 6767 696e 672e          logging.
-0000eda0: 696e 666f 2820 224c 6f67 696e 2073 6573  info( "Login ses
-0000edb0: 7369 6f6e 3a20 2572 2220 2520 2820 7365  sion: %r" % ( se
-0000edc0: 7373 696f 6e2e 6974 656d 7328 2920 2929  ssion.items() ))
-0000edd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ede0: 2077 6562 2e73 6565 6f74 6865 7228 2070   web.seeother( p
-0000edf0: 726f 7879 2820 7765 622e 6374 782e 656e  roxy( web.ctx.en
-0000ee00: 7669 726f 6e20 2920 2b20 7765 622e 696e  viron ) + web.in
-0000ee10: 7075 7428 292e 6765 7428 2022 7265 6469  put().get( "redi
-0000ee20: 7265 6374 222c 2022 2220 2929 0a20 2020  rect", "" )).   
-0000ee30: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-0000ee40: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0000ee50: 204e 6f20 6964 656e 7420 666f 756e 643b   No ident found;
-0000ee60: 2065 7272 6f72 2063 6f6e 7461 696e 7320   error contains 
-0000ee70: 6578 706c 616e 6174 6f72 7920 7374 7269  explanatory stri
-0000ee80: 6e67 2e20 2054 7279 2061 6761 696e 2e0a  ng.  Try again..
-0000ee90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eea0: 7365 7373 696f 6e2e 6c6f 6769 6e09 3d20  session.login.= 
-0000eeb0: 300a 2020 2020 2020 2020 2020 2020 2020  0.              
-0000eec0: 2020 7265 7370 6f6e 7365 093d 2072 656e    response.= ren
-0000eed0: 6465 722e 6c6f 6769 6e28 0a20 2020 2020  der.login(.     
-0000eee0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-0000eef0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ef00: 2020 2020 2020 2020 2022 7469 746c 6522           "title"
-0000ef10: 3a09 224c 6f67 696e 2046 6169 6c65 643a  :."Login Failed:
-0000ef20: 2025 7322 2025 2065 7272 6f72 2c0a 2020   %s" % error,.  
+0000e780: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
+0000e790: 2020 2020 2020 2020 2020 2020 2022 7469               "ti
+0000e7a0: 746c 6522 3a09 2820 2244 656c 6574 6564  tle":.( "Deleted
+0000e7b0: 2025 7322 2025 2028 2072 656d 6f76 6564   %s" % ( removed
+0000e7c0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+0000e7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e7e0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000e7f0: 6e6f 7420 6572 726f 7220 656c 7365 0a20  not error else. 
+0000e800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e820: 2020 2020 2020 2020 2022 4465 6c65 7465           "Delete
+0000e830: 6420 2573 3b20 4661 696c 6564 3a20 2573  d %s; Failed: %s
+0000e840: 2220 2520 2820 7265 6d6f 7665 642c 2065  " % ( removed, e
+0000e850: 7272 6f72 2029 292c 0a20 2020 2020 2020  rror )),.       
+0000e860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e870: 2022 7265 6469 7265 6374 223a 0977 6562   "redirect":.web
+0000e880: 2e69 6e70 7574 2829 2e67 6574 2820 2272  .input().get( "r
+0000e890: 6564 6972 6563 7422 2c20 2222 2029 2c0a  edirect", "" ),.
+0000e8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e8b0: 2020 2020 2020 2020 2263 6869 6c64 7265          "childre
+0000e8c0: 6e22 3a09 7573 6572 5f68 6572 6974 6167  n":.user_heritag
+0000e8d0: 6528 2073 6573 7369 6f6e 2e75 7365 725f  e( session.user_
+0000e8e0: 6964 2029 2c0a 2020 2020 2020 2020 2020  id ),.          
+0000e8f0: 2020 2020 2020 2020 2020 7d29 0a20 2020            }).   
+0000e900: 2020 2020 2020 2020 2020 2020 2077 6562               web
+0000e910: 2e68 6561 6465 7228 2022 4361 6368 652d  .header( "Cache-
+0000e920: 436f 6e74 726f 6c22 2c20 226e 6f2d 6361  Control", "no-ca
+0000e930: 6368 6522 2029 0a20 2020 2020 2020 2020  che" ).         
+0000e940: 2020 2020 2020 2077 6562 2e68 6561 6465         web.heade
+0000e950: 7228 2022 436f 6e74 656e 742d 5479 7065  r( "Content-Type
+0000e960: 222c 2022 7465 7874 2f68 746d 6c22 2029  ", "text/html" )
+0000e970: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e980: 2072 6574 7572 6e20 7265 7370 6f6e 7365   return response
+0000e990: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+0000e9a0: 506f 7374 2076 6961 2022 676f 2220 6275  Post via "go" bu
+0000e9b0: 7474 6f6e 2028 6f72 2076 6961 2065 7665  tton (or via eve
+0000e9c0: 6e74 206f 6e20 5049 4e20 696e 7075 7429  nt on PIN input)
+0000e9d0: 3b20 6174 7465 6d70 7420 746f 206c 6f67  ; attempt to log
+0000e9e0: 696e 0a20 2020 2020 2020 2020 2020 2069  in.            i
+0000e9f0: 6465 6e74 0909 3d20 4e6f 6e65 0a20 2020  dent..= None.   
+0000ea00: 2020 2020 2020 2020 2065 7272 6f72 0909           error..
+0000ea10: 3d20 4e6f 6e65 0a20 2020 2020 2020 2020  = None.         
+0000ea20: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+0000ea30: 2020 2020 2020 2020 6e61 6d65 0909 3d20          name..= 
+0000ea40: 7765 622e 696e 7075 7428 292e 6765 7428  web.input().get(
+0000ea50: 2022 6e61 6d65 2220 290a 2020 2020 2020   "name" ).      
+0000ea60: 2020 2020 2020 2020 2020 7069 6e09 093d            pin..=
+0000ea70: 2077 6562 2e69 6e70 7574 2829 2e67 6574   web.input().get
+0000ea80: 2820 2270 696e 2220 290a 2020 2020 2020  ( "pin" ).      
+0000ea90: 2020 2020 2020 2020 2020 6173 7365 7274            assert
+0000eaa0: 206e 616d 6520 616e 6420 7069 6e2c 2022   name and pin, "
+0000eab0: 496e 7661 6c69 6420 7573 6572 2f50 494e  Invalid user/PIN
+0000eac0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+0000ead0: 2020 7175 6572 7909 093d 2064 622e 7365    query..= db.se
+0000eae0: 6c65 6374 2820 2775 7365 7273 272c 2077  lect( 'users', w
+0000eaf0: 6865 7265 3d27 6e61 6d65 3d24 6e61 6d65  here='name=$name
+0000eb00: 272c 2076 6172 733d 7b22 6e61 6d65 223a  ', vars={"name":
+0000eb10: 206e 616d 652e 7374 7269 7028 292e 6c6f   name.strip().lo
+0000eb20: 7765 7228 297d 2029 0a20 2020 2020 2020  wer()} ).       
+0000eb30: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
+0000eb40: 7175 6572 792c 2022 5573 6572 206e 6f74  query, "User not
+0000eb50: 2066 6f75 6e64 3a20 2572 2220 2520 2820   found: %r" % ( 
+0000eb60: 7175 6572 7920 290a 2020 2020 2020 2020  query ).        
+0000eb70: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
+0000eb80: 2071 7565 7279 3a0a 2020 2020 2020 2020   query:.        
+0000eb90: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
+0000eba0: 696e 672e 696e 666f 2820 226e 616d 653a  ing.info( "name:
+0000ebb0: 2025 7220 7673 2e20 2572 2c20 7069 6e3a   %r vs. %r, pin:
+0000ebc0: 2025 7220 7673 2025 7222 2025 2028 2069   %r vs %r" % ( i
+0000ebd0: 5b27 6e61 6d65 275d 2c20 6e61 6d65 2c20  ['name'], name, 
+0000ebe0: 695b 2770 696e 275d 2c20 7069 6e20 2929  i['pin'], pin ))
+0000ebf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ec00: 2020 2020 2069 6620 695b 2770 696e 275d       if i['pin']
+0000ec10: 203d 3d20 696e 7428 2070 696e 2029 3a0a   == int( pin ):.
+0000ec20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ec30: 2020 2020 2020 2020 6964 656e 7409 3d20          ident.= 
+0000ec40: 690a 2020 2020 2020 2020 2020 2020 2020  i.              
+0000ec50: 2020 2020 2020 2020 2020 6272 6561 6b0a            break.
+0000ec60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ec70: 6173 7365 7274 2069 6465 6e74 2c20 2255  assert ident, "U
+0000ec80: 6e72 6563 6f67 6e69 7a65 6420 7573 6572  nrecognized user
+0000ec90: 2f50 494e 220a 2020 2020 2020 2020 2020  /PIN".          
+0000eca0: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
+0000ecb0: 6f6e 2061 7320 6578 633a 0a20 2020 2020  on as exc:.     
+0000ecc0: 2020 2020 2020 2020 2020 206c 6f67 6769             loggi
+0000ecd0: 6e67 2e77 6172 6e69 6e67 2820 224c 6f67  ng.warning( "Log
+0000ece0: 696e 2066 6169 6c65 643a 206e 616d 653a  in failed: name:
+0000ecf0: 2025 722c 2070 696e 3a20 2572 3a20 2573   %r, pin: %r: %s
+0000ed00: 3a20 2573 2220 2520 2820 6e61 6d65 2c20  : %s" % ( name, 
+0000ed10: 7069 6e2c 2065 7863 2c20 7472 6163 6562  pin, exc, traceb
+0000ed20: 6163 6b2e 666f 726d 6174 5f65 7863 2829  ack.format_exc()
+0000ed30: 2029 290a 2020 2020 2020 2020 2020 2020   )).            
+0000ed40: 2020 2020 6572 726f 7209 093d 2073 7472      error..= str
+0000ed50: 2820 6578 6320 290a 2020 2020 2020 2020  ( exc ).        
+0000ed60: 2020 2020 6966 2069 6465 6e74 3a0a 2020      if ident:.  
+0000ed70: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+0000ed80: 6767 696e 672e 696e 666f 2820 224c 6f67  gging.info( "Log
+0000ed90: 696e 2069 6465 6e74 3a20 2020 2572 2220  in ident:   %r" 
+0000eda0: 2520 2820 6964 656e 742e 6974 656d 7328  % ( ident.items(
+0000edb0: 2920 2929 0a20 2020 2020 2020 2020 2020  ) )).           
+0000edc0: 2020 2020 2073 6573 7369 6f6e 2e75 7064       session.upd
+0000edd0: 6174 6528 2069 6465 6e74 2029 0a20 2020  ate( ident ).   
+0000ede0: 2020 2020 2020 2020 2020 2020 206c 6f67               log
+0000edf0: 6769 6e67 2e69 6e66 6f28 2022 4c6f 6769  ging.info( "Logi
+0000ee00: 6e20 7365 7373 696f 6e3a 2025 7222 2025  n session: %r" %
+0000ee10: 2028 2073 6573 7369 6f6e 2e69 7465 6d73   ( session.items
+0000ee20: 2829 2029 290a 2020 2020 2020 2020 2020  () )).          
+0000ee30: 2020 2020 2020 7765 622e 7365 656f 7468        web.seeoth
+0000ee40: 6572 2820 7072 6f78 7928 2077 6562 2e63  er( proxy( web.c
+0000ee50: 7478 2e65 6e76 6972 6f6e 2029 202b 2077  tx.environ ) + w
+0000ee60: 6562 2e69 6e70 7574 2829 2e67 6574 2820  eb.input().get( 
+0000ee70: 2272 6564 6972 6563 7422 2c20 2222 2029  "redirect", "" )
+0000ee80: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
+0000ee90: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0000eea0: 2020 2020 2320 4e6f 2069 6465 6e74 2066      # No ident f
+0000eeb0: 6f75 6e64 3b20 6572 726f 7220 636f 6e74  ound; error cont
+0000eec0: 6169 6e73 2065 7870 6c61 6e61 746f 7279  ains explanatory
+0000eed0: 2073 7472 696e 672e 2020 5472 7920 6167   string.  Try ag
+0000eee0: 6169 6e2e 0a20 2020 2020 2020 2020 2020  ain..           
+0000eef0: 2020 2020 2073 6573 7369 6f6e 2e6c 6f67       session.log
+0000ef00: 696e 093d 2030 0a20 2020 2020 2020 2020  in.= 0.         
+0000ef10: 2020 2020 2020 2072 6573 706f 6e73 6509         response.
+0000ef20: 3d20 7265 6e64 6572 2e6c 6f67 696e 280a  = render.login(.
 0000ef30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ef40: 2020 2020 2020 2272 6564 6972 6563 7422        "redirect"
-0000ef50: 3a09 7765 622e 696e 7075 7428 292e 6765  :.web.input().ge
-0000ef60: 7428 2022 7265 6469 7265 6374 222c 2022  t( "redirect", "
-0000ef70: 2220 292c 0a20 2020 2020 2020 2020 2020  " ),.           
-0000ef80: 2020 2020 2020 2020 207d 290a 2020 2020           }).    
-0000ef90: 2020 2020 2020 2020 2020 2020 7765 622e              web.
-0000efa0: 6865 6164 6572 2820 2243 6163 6865 2d43  header( "Cache-C
-0000efb0: 6f6e 7472 6f6c 222c 2022 6e6f 2d63 6163  ontrol", "no-cac
-0000efc0: 6865 2220 290a 2020 2020 2020 2020 2020  he" ).          
-0000efd0: 2020 2020 2020 7765 622e 6865 6164 6572        web.header
-0000efe0: 2820 2243 6f6e 7465 6e74 2d54 7970 6522  ( "Content-Type"
-0000eff0: 2c20 2274 6578 742f 6874 6d6c 2220 290a  , "text/html" ).
-0000f000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f010: 7265 7475 726e 2072 6573 706f 6e73 650a  return response.
-0000f020: 0a20 2020 2063 6c61 7373 2061 7069 5f69  .    class api_i
-0000f030: 7373 7565 3a0a 2020 2020 2020 2020 6465  ssue:.        de
-0000f040: 6620 4745 5428 2073 656c 662c 2070 6174  f GET( self, pat
-0000f050: 682c 2069 6e70 7574 5f76 6172 6961 626c  h, input_variabl
-0000f060: 653d 2271 7565 7269 6573 2220 293a 0a20  e="queries" ):. 
-0000f070: 2020 2020 2020 2020 2020 2072 656e 6465             rende
-0000f080: 7209 093d 2077 6562 2e74 656d 706c 6174  r..= web.templat
-0000f090: 652e 7265 6e64 6572 280a 2020 2020 2020  e.render(.      
-0000f0a0: 2020 2020 2020 2020 2020 5450 4c50 4154            TPLPAT
-0000f0b0: 482c 2062 6173 653d 226c 6179 6f75 7422  H, base="layout"
-0000f0c0: 2c20 676c 6f62 616c 733d 7b27 696e 6c69  , globals={'inli
-0000f0d0: 6e65 273a 2069 6e6c 696e 652c 2027 7365  ne': inline, 'se
-0000f0e0: 7373 696f 6e27 3a20 7365 7373 696f 6e7d  ssion': session}
-0000f0f0: 2029 0a20 2020 2020 2020 2020 2020 2061   ).            a
-0000f100: 6363 6570 7409 093d 204e 6f6e 650a 2020  ccept..= None.  
-0000f110: 2020 2020 2020 2020 2020 6966 2070 6174            if pat
-0000f120: 6820 616e 6420 7061 7468 2e65 6e64 7377  h and path.endsw
-0000f130: 6974 6828 2022 2e6a 736f 6e22 2029 3a0a  ith( ".json" ):.
-0000f140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f150: 7061 7468 0909 3d20 7061 7468 5b3a 2d35  path..= path[:-5
-0000f160: 5d09 0923 2063 6c69 7020 6f66 6620 222e  ]..# clip off ".
-0000f170: 6a73 6f6e 220a 2020 2020 2020 2020 2020  json".          
-0000f180: 2020 2020 2020 6163 6365 7074 0909 3d20        accept..= 
-0000f190: 2261 7070 6c69 6361 7469 6f6e 2f6a 736f  "application/jso
-0000f1a0: 6e22 0a0a 2020 2020 2020 2020 2020 2020  n"..            
-0000f1b0: 2320 416c 7761 7973 2072 6574 7572 6e73  # Always returns
-0000f1c0: 2061 2063 6f6e 7465 6e74 2d74 7970 6520   a content-type 
-0000f1d0: 616e 6420 7265 7370 6f6e 7365 2e20 2049  and response.  I
-0000f1e0: 6620 616e 2065 7863 6570 7469 6f6e 2069  f an exception i
-0000f1f0: 730a 2020 2020 2020 2020 2020 2020 2320  s.            # 
-0000f200: 7261 6973 6564 2c20 6974 2073 686f 756c  raised, it shoul
-0000f210: 6420 6265 2061 6e20 6170 7072 6f70 7269  d be an appropri
-0000f220: 6174 6520 6f6e 6520 6672 6f6d 2074 6865  ate one from the
-0000f230: 2073 7570 706c 6965 6420 6672 616d 6577   supplied framew
-0000f240: 6f72 6b20 746f 0a20 2020 2020 2020 2020  ork to.         
-0000f250: 2020 2023 2063 6172 7279 2061 206d 6561     # carry a mea
-0000f260: 6e69 6e67 6675 6c20 4854 5450 2073 7461  ningful HTTP sta
-0000f270: 7475 7320 636f 6465 2e20 204f 7468 6572  tus code.  Other
-0000f280: 7769 7365 2c20 6120 6765 6e65 7269 6320  wise, a generic 
-0000f290: 3530 3020 5365 7276 6572 0a20 2020 2020  500 Server.     
-0000f2a0: 2020 2020 2020 2023 2045 7272 6f72 2077         # Error w
-0000f2b0: 696c 6c20 6265 2070 726f 6475 6365 642e  ill be produced.
-0000f2c0: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
-0000f2d0: 7465 6e74 2c20 7265 7370 6f6e 7365 093d  tent, response.=
-0000f2e0: 2069 7373 7565 5f72 6571 7565 7374 280a   issue_request(.
-0000f2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f300: 7265 6e64 6572 3d72 656e 6465 722c 2070  render=render, p
-0000f310: 6174 683d 7061 7468 2c20 656e 7669 726f  ath=path, enviro
-0000f320: 6e3d 7765 622e 6374 782e 656e 7669 726f  n=web.ctx.enviro
-0000f330: 6e2c 0a20 2020 2020 2020 2020 2020 2020  n,.             
-0000f340: 2020 2061 6363 6570 743d 6163 6365 7074     accept=accept
-0000f350: 2c20 6672 616d 6577 6f72 6b3d 7765 622c  , framework=web,
-0000f360: 206c 6f67 6765 643d 6c6f 6767 6564 2c0a   logged=logged,.
-0000f370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f380: 2a2a 7b20 696e 7075 745f 7661 7269 6162  **{ input_variab
-0000f390: 6c65 3a20 7765 622e 696e 7075 7428 2920  le: web.input() 
-0000f3a0: 7d20 290a 2020 2020 2020 2020 2020 2020  } ).            
-0000f3b0: 7765 622e 6865 6164 6572 2820 2243 6163  web.header( "Cac
-0000f3c0: 6865 2d43 6f6e 7472 6f6c 222c 2022 6e6f  he-Control", "no
-0000f3d0: 2d63 6163 6865 2220 290a 2020 2020 2020  -cache" ).      
-0000f3e0: 2020 2020 2020 7765 622e 6865 6164 6572        web.header
-0000f3f0: 2820 2243 6f6e 7465 6e74 2d54 7970 6522  ( "Content-Type"
-0000f400: 2c20 636f 6e74 656e 7420 290a 2020 2020  , content ).    
-0000f410: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-0000f420: 6573 706f 6e73 650a 0a20 2020 2020 2020  esponse..       
-0000f430: 2064 6566 2050 4f53 5428 2073 656c 662c   def POST( self,
-0000f440: 2070 6174 6820 293a 0a20 2020 2020 2020   path ):.       
-0000f450: 2020 2020 2023 2066 6f72 6d20 6461 7461       # form data
-0000f460: 2070 6f73 7465 6420 696e 2077 6562 2e69   posted in web.i
-0000f470: 6e70 7574 2829 2c20 6a75 7374 206c 696b  nput(), just lik
-0000f480: 6520 7175 6572 6965 730a 2020 2020 2020  e queries.      
-0000f490: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0000f4a0: 662e 4745 5428 2070 6174 682c 2069 6e70  f.GET( path, inp
-0000f4b0: 7574 5f76 6172 6961 626c 653d 2270 6f73  ut_variable="pos
-0000f4c0: 7465 6422 2029 0a0a 2020 2020 636c 6173  ted" )..    clas
-0000f4d0: 7320 7461 6275 6c61 725f 7265 7175 6573  s tabular_reques
-0000f4e0: 745f 6261 7365 3a0a 2020 2020 2020 2020  t_base:.        
-0000f4f0: 2320 5365 7420 7265 7175 6573 7420 3d20  # Set request = 
-0000f500: 3c66 756e 6374 696f 6e20 7265 7475 726e  <function return
-0000f510: 696e 6720 2863 6f6e 7465 6e74 2c20 7265  ing (content, re
-0000f520: 7370 6f6e 7365 293e 0a20 2020 2020 2020  sponse)>.       
-0000f530: 2064 6566 2047 4554 2820 7365 6c66 2c20   def GET( self, 
-0000f540: 7061 7468 2c20 696e 7075 745f 7661 7269  path, input_vari
-0000f550: 6162 6c65 3d22 7175 6572 6965 7322 2029  able="queries" )
-0000f560: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
-0000f570: 6966 206e 6f74 206c 6f67 6765 6428 293a  if not logged():
-0000f580: 0a20 2020 2020 2020 2020 2020 2023 2020  .            #  
-0000f590: 2020 2077 6562 2e73 6565 6f74 6865 7228     web.seeother(
-0000f5a0: 2070 726f 7879 2820 7765 622e 6374 782e   proxy( web.ctx.
-0000f5b0: 656e 7669 726f 6e20 2920 2b20 272f 6c6f  environ ) + '/lo
-0000f5c0: 6769 6e3f 7265 6469 7265 6374 3d27 202b  gin?redirect=' +
-0000f5d0: 2077 6562 2e63 7478 2e65 6e76 6972 6f6e   web.ctx.environ
-0000f5e0: 2e67 6574 2820 2750 4154 485f 494e 464f  .get( 'PATH_INFO
-0000f5f0: 272c 2027 2720 2929 0a20 2020 2020 2020  ', '' )).       
-0000f600: 2020 2020 2023 2020 2020 2072 6574 7572       #     retur
-0000f610: 6e0a 2020 2020 2020 2020 2020 2020 7265  n.            re
-0000f620: 6e64 6572 0909 3d20 7765 622e 7465 6d70  nder..= web.temp
-0000f630: 6c61 7465 2e72 656e 6465 7228 0a20 2020  late.render(.   
-0000f640: 2020 2020 2020 2020 2020 2020 2054 504c               TPL
-0000f650: 5041 5448 2c20 6261 7365 3d22 6c61 796f  PATH, base="layo
-0000f660: 7574 222c 2067 6c6f 6261 6c73 3d7b 2769  ut", globals={'i
-0000f670: 6e6c 696e 6527 3a20 696e 6c69 6e65 2c20  nline': inline, 
-0000f680: 2773 6573 7369 6f6e 273a 2073 6573 7369  'session': sessi
-0000f690: 6f6e 7d20 290a 2020 2020 2020 2020 2020  on} ).          
-0000f6a0: 2020 6163 6365 7074 0909 3d20 4e6f 6e65    accept..= None
-0000f6b0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000f6c0: 7061 7468 2061 6e64 2070 6174 682e 656e  path and path.en
-0000f6d0: 6473 7769 7468 2820 222e 6a73 6f6e 2220  dswith( ".json" 
-0000f6e0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000f6f0: 2020 2070 6174 6809 093d 2070 6174 685b     path..= path[
-0000f700: 3a2d 355d 0909 2320 636c 6970 206f 6666  :-5]..# clip off
-0000f710: 2022 2e6a 736f 6e22 0a20 2020 2020 2020   ".json".       
-0000f720: 2020 2020 2020 2020 2061 6363 6570 7409           accept.
-0000f730: 093d 2022 6170 706c 6963 6174 696f 6e2f  .= "application/
-0000f740: 6a73 6f6e 220a 0a20 2020 2020 2020 2020  json"..         
-0000f750: 2020 2023 2041 6c77 6179 7320 7265 7475     # Always retu
-0000f760: 726e 7320 6120 636f 6e74 656e 742d 7479  rns a content-ty
-0000f770: 7065 2061 6e64 2072 6573 706f 6e73 652e  pe and response.
-0000f780: 2020 4966 2061 6e20 6578 6365 7074 696f    If an exceptio
-0000f790: 6e20 6973 0a20 2020 2020 2020 2020 2020  n is.           
-0000f7a0: 2023 2072 6169 7365 642c 2069 7420 7368   # raised, it sh
-0000f7b0: 6f75 6c64 2062 6520 616e 2061 7070 726f  ould be an appro
-0000f7c0: 7072 6961 7465 206f 6e65 2066 726f 6d20  priate one from 
-0000f7d0: 7468 6520 7375 7070 6c69 6564 2066 7261  the supplied fra
-0000f7e0: 6d65 776f 726b 2074 6f0a 2020 2020 2020  mework to.      
-0000f7f0: 2020 2020 2020 2320 6361 7272 7920 6120        # carry a 
-0000f800: 6d65 616e 696e 6766 756c 2048 5454 5020  meaningful HTTP 
-0000f810: 7374 6174 7573 2063 6f64 652e 2020 4f74  status code.  Ot
-0000f820: 6865 7277 6973 652c 2061 2067 656e 6572  herwise, a gener
-0000f830: 6963 2035 3030 2053 6572 7665 720a 2020  ic 500 Server.  
-0000f840: 2020 2020 2020 2020 2020 2320 4572 726f            # Erro
-0000f850: 7220 7769 6c6c 2062 6520 7072 6f64 7563  r will be produc
-0000f860: 6564 2e0a 2020 2020 2020 2020 2020 2020  ed..            
-0000f870: 7265 7175 6573 7409 093d 2073 656c 662e  request..= self.
-0000f880: 5f5f 636c 6173 735f 5f2e 5f5f 6469 6374  __class__.__dict
-0000f890: 5f5f 5b27 7265 7175 6573 7427 5d0a 2020  __['request'].  
-0000f8a0: 2020 2020 2020 2020 2020 6c6f 672e 696e            log.in
-0000f8b0: 666f 2820 2254 6162 756c 6172 2041 5049  fo( "Tabular API
-0000f8c0: 2063 616c 6c3a 207b 2172 7d22 2e66 6f72   call: {!r}".for
-0000f8d0: 6d61 7428 2072 6571 7565 7374 2029 290a  mat( request )).
-0000f8e0: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
-0000f8f0: 656e 742c 2072 6573 706f 6e73 6509 3d20  ent, response.= 
-0000f900: 7265 7175 6573 7428 0a20 2020 2020 2020  request(.       
-0000f910: 2020 2020 2020 2020 2072 656e 6465 723d           render=
-0000f920: 7265 6e64 6572 2c20 7061 7468 3d70 6174  render, path=pat
-0000f930: 682c 2065 6e76 6972 6f6e 3d77 6562 2e63  h, environ=web.c
-0000f940: 7478 2e65 6e76 6972 6f6e 2c0a 2020 2020  tx.environ,.    
-0000f950: 2020 2020 2020 2020 2020 2020 6163 6365              acce
-0000f960: 7074 3d61 6363 6570 742c 2066 7261 6d65  pt=accept, frame
-0000f970: 776f 726b 3d77 6562 2c20 6c6f 6767 6564  work=web, logged
-0000f980: 3d6c 6f67 6765 642c 0a20 2020 2020 2020  =logged,.       
-0000f990: 2020 2020 2020 2020 202a 2a7b 2069 6e70           **{ inp
-0000f9a0: 7574 5f76 6172 6961 626c 653a 2077 6562  ut_variable: web
-0000f9b0: 2e69 6e70 7574 2829 207d 2029 0a20 2020  .input() } ).   
-0000f9c0: 2020 2020 2020 2020 2077 6562 2e68 6561           web.hea
-0000f9d0: 6465 7228 2022 4361 6368 652d 436f 6e74  der( "Cache-Cont
-0000f9e0: 726f 6c22 2c20 226e 6f2d 6361 6368 6522  rol", "no-cache"
-0000f9f0: 2029 0a20 2020 2020 2020 2020 2020 2077   ).            w
-0000fa00: 6562 2e68 6561 6465 7228 2022 436f 6e74  eb.header( "Cont
-0000fa10: 656e 742d 5479 7065 222c 2063 6f6e 7465  ent-Type", conte
-0000fa20: 6e74 2029 0a20 2020 2020 2020 2020 2020  nt ).           
-0000fa30: 2072 6574 7572 6e20 7265 7370 6f6e 7365   return response
-0000fa40: 0a0a 2020 2020 2020 2020 6465 6620 504f  ..        def PO
-0000fa50: 5354 2820 7365 6c66 2c20 7061 7468 2029  ST( self, path )
-0000fa60: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
-0000fa70: 666f 726d 2064 6174 6120 706f 7374 6564  form data posted
-0000fa80: 2069 6e20 7765 622e 696e 7075 7428 292c   in web.input(),
-0000fa90: 206a 7573 7420 6c69 6b65 2071 7565 7269   just like queri
-0000faa0: 6573 0a20 2020 2020 2020 2020 2020 2072  es.            r
-0000fab0: 6574 7572 6e20 7365 6c66 2e47 4554 2820  eturn self.GET( 
-0000fac0: 7061 7468 2c20 696e 7075 745f 7661 7269  path, input_vari
-0000fad0: 6162 6c65 3d22 706f 7374 6564 2220 290a  able="posted" ).
-0000fae0: 0a20 2020 2063 6c61 7373 2061 7069 5f6c  .    class api_l
-0000faf0: 6963 656e 7365 7328 2074 6162 756c 6172  icenses( tabular
-0000fb00: 5f72 6571 7565 7374 5f62 6173 6520 293a  _request_base ):
-0000fb10: 0a20 2020 2020 2020 2072 6571 7565 7374  .        request
-0000fb20: 0909 093d 206c 6963 656e 7365 735f 7265  ...= licenses_re
-0000fb30: 7175 6573 740a 0a20 2020 2063 6c61 7373  quest..    class
-0000fb40: 2061 7069 5f63 7265 6465 6e74 6961 6c73   api_credentials
-0000fb50: 2820 7461 6275 6c61 725f 7265 7175 6573  ( tabular_reques
-0000fb60: 745f 6261 7365 2029 3a0a 2020 2020 2020  t_base ):.      
-0000fb70: 2020 7265 7175 6573 7409 0909 3d20 6372    request...= cr
-0000fb80: 6564 656e 7469 616c 735f 7265 7175 6573  edentials_reques
-0000fb90: 740a 0a20 2020 2063 6c61 7373 2061 7069  t..    class api
-0000fba0: 5f6b 6579 7061 6972 7328 2074 6162 756c  _keypairs( tabul
-0000fbb0: 6172 5f72 6571 7565 7374 5f62 6173 6520  ar_request_base 
-0000fbc0: 293a 0a20 2020 2020 2020 2072 6571 7565  ):.        reque
-0000fbd0: 7374 0909 093d 206b 6579 7061 6972 735f  st...= keypairs_
-0000fbe0: 7265 7175 6573 740a 0a20 2020 2063 6c61  request..    cla
-0000fbf0: 7373 2053 7461 7469 6341 7070 4469 7228  ss StaticAppDir(
-0000fc00: 2077 6562 2e68 7474 7073 6572 7665 722e   web.httpserver.
-0000fc10: 5374 6174 6963 4170 702c 206f 626a 6563  StaticApp, objec
-0000fc20: 7420 293a 0a20 2020 2020 2020 2022 2222  t ):.        """
-0000fc30: 496d 706c 656d 656e 7420 6f75 7220 6f77  Implement our ow
-0000fc40: 6e20 7665 7273 696f 6e20 6f66 2053 7461  n version of Sta
-0000fc50: 7469 6341 7070 2061 6e64 2053 7461 7469  ticApp and Stati
-0000fc60: 634d 6964 646c 6577 6172 6520 736f 2077  cMiddleware so w
-0000fc70: 6520 6361 6e20 7265 7475 726e 2070 726f  e can return pro
-0000fc80: 7065 7220 6361 6368 696e 670a 2020 2020  per caching.    
-0000fc90: 2020 2020 6865 6164 6572 732c 2061 6e64      headers, and
-0000fca0: 2073 7065 6369 6679 2061 2073 7065 6369   specify a speci
-0000fcb0: 6669 6320 6261 7365 6469 7220 666f 7220  fic basedir for 
-0000fcc0: 7374 6174 6963 2066 696c 6520 6163 6365  static file acce
-0000fcd0: 7373 2e20 466f 7263 6520 6e65 772d 7374  ss. Force new-st
-0000fce0: 796c 6520 636c 6173 7365 7320 696e 0a20  yle classes in. 
-0000fcf0: 2020 2020 2020 2050 7974 686f 6e32 2073         Python2 s
-0000fd00: 6f20 7375 7065 7220 776f 726b 732e 2020  o super works.  
-0000fd10: 556e 666f 7274 756e 6174 656c 792c 2074  Unfortunately, t
-0000fd20: 6865 2050 7974 686f 6e32 2053 696d 706c  he Python2 Simpl
-0000fd30: 6548 5454 5052 6571 7565 7374 2069 6d70  eHTTPRequest imp
-0000fd40: 6c65 6d65 6e74 6174 696f 6e20 6261 6b65  lementation bake
-0000fd50: 640a 2020 2020 2020 2020 696e 206f 732e  d.        in os.
-0000fd60: 6765 7463 7764 2073 6f20 7765 2068 6176  getcwd so we hav
-0000fd70: 6520 746f 2074 7261 6e73 706c 616e 7420  e to transplant 
-0000fd80: 6120 5079 7468 6f6e 322f 3320 636f 6d70  a Python2/3 comp
-0000fd90: 6174 6962 6c65 2074 7261 6e73 6c61 7465  atible translate
-0000fda0: 5f70 6174 682c 2074 6f6f 2e0a 0a20 2020  _path, too...   
-0000fdb0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000fdc0: 2064 6566 205f 5f69 6e69 745f 5f28 2073   def __init__( s
-0000fdd0: 656c 662c 2065 6e76 6972 6f6e 2c20 7374  elf, environ, st
-0000fde0: 6172 745f 7265 7370 6f6e 7365 2c20 6469  art_response, di
-0000fdf0: 7265 6374 6f72 7920 293a 0a20 2020 2020  rectory ):.     
-0000fe00: 2020 2020 2020 2073 7570 6572 2820 5374         super( St
-0000fe10: 6174 6963 4170 7044 6972 2c20 7365 6c66  aticAppDir, self
-0000fe20: 2029 2e5f 5f69 6e69 745f 5f28 2065 6e76   ).__init__( env
-0000fe30: 6972 6f6e 2c20 7374 6172 745f 7265 7370  iron, start_resp
-0000fe40: 6f6e 7365 2029 0a20 2020 2020 2020 2020  onse ).         
-0000fe50: 2020 2073 656c 662e 6469 7265 6374 6f72     self.director
-0000fe60: 7909 3d20 6469 7265 6374 6f72 790a 0a20  y.= directory.. 
-0000fe70: 2020 2020 2020 2064 6566 2074 7261 6e73         def trans
-0000fe80: 6c61 7465 5f70 6174 6828 7365 6c66 2c20  late_path(self, 
-0000fe90: 7061 7468 293a 0a20 2020 2020 2020 2020  path):.         
-0000fea0: 2020 2022 2222 5472 616e 736c 6174 6520     """Translate 
-0000feb0: 6120 2f2d 7365 7061 7261 7465 6420 5041  a /-separated PA
-0000fec0: 5448 2074 6f20 7468 6520 6c6f 6361 6c20  TH to the local 
-0000fed0: 6669 6c65 6e61 6d65 2073 796e 7461 782e  filename syntax.
-0000fee0: 0a0a 2020 2020 2020 2020 2020 2020 436f  ..            Co
-0000fef0: 6d70 6f6e 656e 7473 2074 6861 7420 6d65  mponents that me
-0000ff00: 616e 2073 7065 6369 616c 2074 6869 6e67  an special thing
-0000ff10: 7320 746f 2074 6865 206c 6f63 616c 2066  s to the local f
-0000ff20: 696c 6520 7379 7374 656d 0a20 2020 2020  ile system.     
-0000ff30: 2020 2020 2020 2028 652e 672e 2064 7269         (e.g. dri
-0000ff40: 7665 206f 7220 6469 7265 6374 6f72 7920  ve or directory 
-0000ff50: 6e61 6d65 7329 2061 7265 2069 676e 6f72  names) are ignor
-0000ff60: 6564 2e20 2028 5858 5820 5468 6579 2073  ed.  (XXX They s
-0000ff70: 686f 756c 640a 2020 2020 2020 2020 2020  hould.          
-0000ff80: 2020 7072 6f62 6162 6c79 2062 6520 6469    probably be di
-0000ff90: 6167 6e6f 7365 642e 290a 0a20 2020 2020  agnosed.)..     
-0000ffa0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000ffb0: 2020 2020 2020 2023 2061 6261 6e64 6f6e         # abandon
-0000ffc0: 2071 7565 7279 2070 6172 616d 6574 6572   query parameter
-0000ffd0: 730a 2020 2020 2020 2020 2020 2020 7061  s.            pa
-0000ffe0: 7468 203d 2070 6174 682e 7370 6c69 7428  th = path.split(
-0000fff0: 273f 272c 3129 5b30 5d0a 2020 2020 2020  '?',1)[0].      
-00010000: 2020 2020 2020 7061 7468 203d 2070 6174        path = pat
-00010010: 682e 7370 6c69 7428 2723 272c 3129 5b30  h.split('#',1)[0
-00010020: 5d0a 2020 2020 2020 2020 2020 2020 2320  ].            # 
-00010030: 446f 6e27 7420 666f 7267 6574 2065 7870  Don't forget exp
-00010040: 6c69 6369 7420 7472 6169 6c69 6e67 2073  licit trailing s
-00010050: 6c61 7368 2077 6865 6e20 6e6f 726d 616c  lash when normal
-00010060: 697a 696e 672e 2049 7373 7565 3137 3332  izing. Issue1732
-00010070: 340a 2020 2020 2020 2020 2020 2020 7472  4.            tr
-00010080: 6169 6c69 6e67 5f73 6c61 7368 203d 2070  ailing_slash = p
-00010090: 6174 682e 7273 7472 6970 2829 2e65 6e64  ath.rstrip().end
-000100a0: 7377 6974 6828 272f 2729 0a20 2020 2020  swith('/').     
-000100b0: 2020 2020 2020 2070 6174 6820 3d20 706f         path = po
-000100c0: 7369 7870 6174 682e 6e6f 726d 7061 7468  sixpath.normpath
-000100d0: 2875 6e71 756f 7465 2870 6174 6829 290a  (unquote(path)).
-000100e0: 2020 2020 2020 2020 2020 2020 776f 7264              word
-000100f0: 7320 3d20 7061 7468 2e73 706c 6974 2827  s = path.split('
-00010100: 2f27 290a 2020 2020 2020 2020 2020 2020  /').            
-00010110: 776f 7264 7320 3d20 6669 6c74 6572 284e  words = filter(N
-00010120: 6f6e 652c 2077 6f72 6473 290a 2020 2020  one, words).    
-00010130: 2020 2020 2020 2020 7061 7468 203d 2073          path = s
-00010140: 656c 662e 6469 7265 6374 6f72 7920 2023  elf.directory  #
-00010150: 203c 3c20 4427 6f68 210a 2020 2020 2020   << D'oh!.      
-00010160: 2020 2020 2020 666f 7220 776f 7264 2069        for word i
-00010170: 6e20 776f 7264 733a 0a20 2020 2020 2020  n words:.       
-00010180: 2020 2020 2020 2020 2069 6620 6f73 2e70           if os.p
-00010190: 6174 682e 6469 726e 616d 6528 776f 7264  ath.dirname(word
-000101a0: 2920 6f72 2077 6f72 6420 696e 2028 6f73  ) or word in (os
-000101b0: 2e63 7572 6469 722c 206f 732e 7061 7264  .curdir, os.pard
-000101c0: 6972 293a 0a20 2020 2020 2020 2020 2020  ir):.           
-000101d0: 2020 2020 2020 2020 2023 2049 676e 6f72           # Ignor
-000101e0: 6520 636f 6d70 6f6e 656e 7473 2074 6861  e components tha
-000101f0: 7420 6172 6520 6e6f 7420 6120 7369 6d70  t are not a simp
-00010200: 6c65 2066 696c 652f 6469 7265 6374 6f72  le file/director
-00010210: 7920 6e61 6d65 0a20 2020 2020 2020 2020  y name.         
-00010220: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
-00010230: 6e75 650a 2020 2020 2020 2020 2020 2020  nue.            
-00010240: 2020 2020 7061 7468 203d 206f 732e 7061      path = os.pa
-00010250: 7468 2e6a 6f69 6e28 7061 7468 2c20 776f  th.join(path, wo
-00010260: 7264 290a 2020 2020 2020 2020 2020 2020  rd).            
-00010270: 6966 2074 7261 696c 696e 675f 736c 6173  if trailing_slas
-00010280: 683a 0a20 2020 2020 2020 2020 2020 2020  h:.             
-00010290: 2020 2070 6174 6820 2b3d 2027 2f27 0a20     path += '/'. 
-000102a0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000102b0: 6e20 7061 7468 0a0a 2020 2020 6361 6368  n path..    cach
-000102c0: 655f 6d61 785f 6167 6509 093d 2033 302a  e_max_age..= 30*
-000102d0: 3234 2a36 302a 3630 0a0a 2020 2020 636c  24*60*60..    cl
-000102e0: 6173 7320 5374 6174 6963 4d69 6464 6c65  ass StaticMiddle
-000102f0: 7761 7265 4469 7228 2077 6562 2e68 7474  wareDir( web.htt
-00010300: 7073 6572 7665 722e 5374 6174 6963 4d69  pserver.StaticMi
-00010310: 6464 6c65 7761 7265 2c20 6f62 6a65 6374  ddleware, object
-00010320: 2029 3a0a 2020 2020 2020 2020 2222 2257   ):.        """W
-00010330: 5347 4920 6d69 6464 6c65 7761 7265 2066  SGI middleware f
-00010340: 6f72 2073 6572 7669 6e67 2073 7461 7469  or serving stati
-00010350: 6320 6669 6c65 7320 6672 6f6d 2074 6865  c files from the
-00010360: 2073 7065 6369 6669 6564 2062 6173 6564   specified based
-00010370: 6972 2e22 2222 0a20 2020 2020 2020 2064  ir.""".        d
-00010380: 6566 205f 5f69 6e69 745f 5f28 2073 656c  ef __init__( sel
-00010390: 662c 2061 7070 2c20 7072 6566 6978 3d22  f, app, prefix="
-000103a0: 2f73 7461 7469 632f 222c 2062 6173 6564  /static/", based
-000103b0: 6972 3d6f 732e 6765 7463 7764 2829 2029  ir=os.getcwd() )
-000103c0: 3a0a 2020 2020 2020 2020 2020 2020 7375  :.            su
-000103d0: 7065 7228 2053 7461 7469 634d 6964 646c  per( StaticMiddl
-000103e0: 6577 6172 6544 6972 2c20 7365 6c66 2029  ewareDir, self )
-000103f0: 2e5f 5f69 6e69 745f 5f28 2061 7070 2c20  .__init__( app, 
-00010400: 7072 6566 6978 3d70 7265 6669 7820 290a  prefix=prefix ).
-00010410: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00010420: 2e62 6173 6564 6972 093d 2062 6173 6564  .basedir.= based
-00010430: 6972 0a20 2020 2020 2020 2020 2020 206c  ir.            l
-00010440: 6f67 6769 6e67 2e69 6e66 6f28 2022 5365  ogging.info( "Se
-00010450: 7276 696e 6720 7374 6174 6963 2066 696c  rving static fil
-00010460: 6573 206f 7574 206f 6620 7b7d 222e 666f  es out of {}".fo
-00010470: 726d 6174 2820 6261 7365 6469 7220 2b20  rmat( basedir + 
-00010480: 7072 6566 6978 2029 290a 0a20 2020 2020  prefix ))..     
-00010490: 2020 2064 6566 205f 5f63 616c 6c5f 5f28     def __call__(
-000104a0: 2073 656c 662c 2065 6e76 6972 6f6e 2c20   self, environ, 
-000104b0: 7374 6172 745f 7265 7370 6f6e 7365 2029  start_response )
-000104c0: 3a0a 2020 2020 2020 2020 2020 2020 7061  :.            pa
-000104d0: 7468 2009 093d 2065 6e76 6972 6f6e 2e67  th ..= environ.g
-000104e0: 6574 2820 2750 4154 485f 494e 464f 272c  et( 'PATH_INFO',
-000104f0: 2027 2720 290a 2020 2020 2020 2020 2020   '' ).          
-00010500: 2020 7061 7468 2009 093d 2073 656c 662e    path ..= self.
-00010510: 6e6f 726d 7061 7468 2820 7061 7468 2029  normpath( path )
-00010520: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00010530: 7061 7468 2e73 7461 7274 7377 6974 6828  path.startswith(
-00010540: 7365 6c66 2e70 7265 6669 7829 3a0a 2020  self.prefix):.  
-00010550: 2020 2020 2020 2020 2020 2020 2020 6170                ap
-00010560: 7020 0909 3d20 5374 6174 6963 4170 7044  p ..= StaticAppD
-00010570: 6972 2820 656e 7669 726f 6e2c 2073 7461  ir( environ, sta
-00010580: 7274 5f72 6573 706f 6e73 652c 2073 656c  rt_response, sel
-00010590: 662e 6261 7365 6469 7220 290a 2020 2020  f.basedir ).    
-000105a0: 2020 2020 2020 2020 2020 2020 6170 702e              app.
-000105b0: 7365 6e64 5f68 6561 6465 7228 2027 4361  send_header( 'Ca
-000105c0: 6368 652d 436f 6e74 726f 6c27 2c20 2770  che-Control', 'p
-000105d0: 7562 6c69 632c 206d 6178 2d61 6765 3d25  ublic, max-age=%
-000105e0: 6427 2025 2028 2063 6163 6865 5f6d 6178  d' % ( cache_max
-000105f0: 5f61 6765 2029 290a 2020 2020 2020 2020  _age )).        
-00010600: 2020 2020 2020 2020 7265 7475 726e 2061          return a
-00010610: 7070 0a20 2020 2020 2020 2020 2020 2065  pp.            e
-00010620: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00010630: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00010640: 2e61 7070 2820 656e 7669 726f 6e2c 2073  .app( environ, s
-00010650: 7461 7274 5f72 6573 706f 6e73 6520 290a  tart_response ).
-00010660: 0a20 2020 2063 6c61 7373 204c 6f67 4d69  .    class LogMi
-00010670: 6464 6c65 7761 7265 4346 2820 7765 622e  ddlewareCF( web.
-00010680: 6874 7470 7365 7276 6572 2e4c 6f67 4d69  httpserver.LogMi
-00010690: 6464 6c65 7761 7265 2c20 6f62 6a65 6374  ddleware, object
-000106a0: 2029 3a0a 2020 2020 2020 2020 6465 6620   ):.        def 
-000106b0: 6c6f 6728 2073 656c 662c 2073 7461 7475  log( self, statu
-000106c0: 732c 2065 6e76 6972 6f6e 2029 3a0a 2020  s, environ ):.  
-000106d0: 2020 2020 2020 2020 2020 6366 5f69 7009            cf_ip.
-000106e0: 093d 2065 6e76 6972 6f6e 2e67 6574 2820  .= environ.get( 
-000106f0: 2748 5454 505f 4346 5f43 4f4e 4e45 4354  'HTTP_CF_CONNECT
-00010700: 494e 475f 4950 2720 290a 2020 2020 2020  ING_IP' ).      
-00010710: 2020 2020 2020 6966 2063 665f 6970 2069        if cf_ip i
-00010720: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-00010730: 2020 2020 2020 2020 6366 5f69 7009 093d          cf_ip..=
-00010740: 2065 6e76 6972 6f6e 2e67 6574 2820 2748   environ.get( 'H
-00010750: 5454 505f 585f 464f 5257 4152 4445 445f  TTP_X_FORWARDED_
-00010760: 464f 5227 2029 0a20 2020 2020 2020 2020  FOR' ).         
-00010770: 2020 2069 6620 6366 5f69 7020 6973 206e     if cf_ip is n
-00010780: 6f74 204e 6f6e 6520 616e 6420 272c 2720  ot None and ',' 
-00010790: 696e 2063 665f 6970 3a0a 2020 2020 2020  in cf_ip:.      
-000107a0: 2020 2020 2020 2020 2020 2320 4346 2061            # CF a
-000107b0: 7070 656e 6473 2063 6f6e 6e65 6374 696e  ppends connectin
-000107c0: 6720 4950 2074 6f20 585f 464f 5257 4152  g IP to X_FORWAR
-000107d0: 4445 445f 464f 520a 2020 2020 2020 2020  DED_FOR.        
-000107e0: 2020 2020 2020 2020 6366 5f69 7009 093d          cf_ip..=
-000107f0: 2063 665f 6970 2e73 706c 6974 2820 272c   cf_ip.split( ',
-00010800: 2720 295b 2d31 5d2e 7374 7269 7028 290a  ' )[-1].strip().
-00010810: 2020 2020 2020 2020 2020 2020 6366 5f63              cf_c
-00010820: 6f75 6e74 7279 0909 3d20 656e 7669 726f  ountry..= enviro
-00010830: 6e2e 6765 7428 2027 4854 5450 5f43 465f  n.get( 'HTTP_CF_
-00010840: 4950 434f 554e 5452 5927 2029 0a0a 2020  IPCOUNTRY' )..  
-00010850: 2020 2020 2020 2020 2020 2369 702c 706f            #ip,po
-00010860: 7274 0909 3d20 656e 7669 726f 6e2e 6765  rt..= environ.ge
-00010870: 7428 2027 5245 4d4f 5445 5f41 4444 5227  t( 'REMOTE_ADDR'
-00010880: 2029 2c65 6e76 6972 6f6e 2e67 6574 2820   ),environ.get( 
-00010890: 2752 454d 4f54 455f 504f 5254 2720 290a  'REMOTE_PORT' ).
-000108a0: 2020 2020 2020 2020 2020 2020 6966 2063              if c
-000108b0: 665f 6970 3a0a 2020 2020 2020 2020 2020  f_ip:.          
-000108c0: 2020 2020 2020 656e 7669 726f 6e5b 2752        environ['R
-000108d0: 454d 4f54 455f 4144 4452 275d 203d 2063  EMOTE_ADDR'] = c
-000108e0: 665f 6970 0a20 2020 2020 2020 2020 2020  f_ip.           
-000108f0: 2069 6620 6366 5f63 6f75 6e74 7279 3a0a   if cf_country:.
-00010900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010910: 656e 7669 726f 6e5b 2752 454d 4f54 455f  environ['REMOTE_
-00010920: 504f 5254 275d 203d 2063 665f 636f 756e  PORT'] = cf_coun
-00010930: 7472 790a 2020 2020 2020 2020 2020 2020  try.            
-00010940: 7265 7475 726e 2073 7570 6572 2820 4c6f  return super( Lo
-00010950: 674d 6964 646c 6577 6172 6543 462c 2073  gMiddlewareCF, s
-00010960: 656c 6620 292e 6c6f 6728 2073 7461 7475  elf ).log( statu
-00010970: 732c 2065 6e76 6972 6f6e 2029 0a0a 2020  s, environ )..  
-00010980: 2020 2320 4765 7420 7468 6520 7265 7175    # Get the requ
-00010990: 6972 6564 2077 6562 2e70 7920 636c 6173  ired web.py clas
-000109a0: 7365 7320 6672 6f6d 2074 6865 206c 6f63  ses from the loc
-000109b0: 616c 206e 616d 6573 7061 6365 2e20 2054  al namespace.  T
-000109c0: 6865 2069 6661 6365 3a70 6f72 7420 6d75  he iface:port mu
-000109d0: 7374 2061 6c77 6179 7320 7061 7373 6564  st always passed
-000109e0: 0a20 2020 2023 206f 6e20 6172 6776 5b31  .    # on argv[1
-000109f0: 5d20 746f 2075 7365 2061 7070 2e72 756e  ] to use app.run
-00010a00: 2829 2c20 736f 2075 7365 206c 6f77 6572  (), so use lower
-00010a10: 2d6c 6576 656c 2077 6562 2e68 7474 7073  -level web.https
-00010a20: 6572 7665 722e 7275 6e73 696d 706c 6520  erver.runsimple 
-00010a30: 696e 7465 7266 6163 652e 2020 5468 6973  interface.  This
-00010a40: 2073 6574 730a 2020 2020 2320 7570 2074   sets.    # up t
-00010a50: 6865 2057 5347 4920 6d69 6464 6c65 7761  he WSGI middlewa
-00010a60: 7265 2063 6861 696e 2c20 7072 696e 7473  re chain, prints
-00010a70: 2074 6865 2061 6464 7265 7373 2061 6e64   the address and
-00010a80: 2074 6865 6e20 696e 766f 6b65 730a 2020   then invokes.  
-00010a90: 2020 2320 6874 7470 7365 7276 6572 2e57    # httpserver.W
-00010aa0: 5347 4973 6572 7665 722e 7374 6172 7428  SGIserver.start(
-00010ab0: 292c 2077 6869 6368 2064 6f65 7320 7468  ), which does th
-00010ac0: 6520 6269 6e64 2c20 616e 6420 7468 656e  e bind, and then
-00010ad0: 206d 616b 6573 2057 5347 4920 6361 6c6c   makes WSGI call
-00010ae0: 730a 2020 2020 6170 7009 0909 093d 2077  s.    app....= w
-00010af0: 6562 2e61 7070 6c69 6361 7469 6f6e 2820  eb.application( 
-00010b00: 7572 6c73 2c20 6c6f 6361 6c73 2829 2029  urls, locals() )
-00010b10: 0a0a 2020 2020 2320 5365 7373 696f 6e73  ..    # Sessions
-00010b20: 0a20 2020 2067 6c6f 6261 6c20 7365 7373  .    global sess
-00010b30: 696f 6e5f 696e 6974 6961 6c69 7a65 720a  ion_initializer.
-00010b40: 2020 2020 7365 7373 696f 6e09 0909 3d20      session...= 
-00010b50: 7765 622e 7365 7373 696f 6e2e 5365 7373  web.session.Sess
-00010b60: 696f 6e28 0a20 2020 2020 2020 2061 7070  ion(.        app
-00010b70: 2c20 7765 622e 7365 7373 696f 6e2e 4442  , web.session.DB
-00010b80: 5374 6f72 6528 2064 622c 2027 7365 7373  Store( db, 'sess
-00010b90: 696f 6e73 2720 292c 2069 6e69 7469 616c  ions' ), initial
-00010ba0: 697a 6572 3d73 6573 7369 6f6e 5f69 6e69  izer=session_ini
-00010bb0: 7469 616c 697a 6572 2029 0a0a 2020 2020  tializer )..    
-00010bc0: 2320 5765 2063 616e 2774 2075 7365 2074  # We can't use t
-00010bd0: 6865 2073 746f 636b 2072 756e 7369 6d70  he stock runsimp
-00010be0: 6c65 3b20 7765 2068 6176 6520 746f 2062  le; we have to b
-00010bf0: 7569 6c64 2075 7020 6f75 7220 6f77 6e20  uild up our own 
-00010c00: 6368 6169 6e20 6f66 2057 5347 4920 6d69  chain of WSGI mi
-00010c10: 6464 6c65 7761 7265 2061 6e64 2072 756e  ddleware and run
-00010c20: 0a20 2020 2023 2069 7473 2073 6572 7665  .    # its serve
-00010c30: 722c 2069 6e20 6f72 6465 7220 746f 2067  r, in order to g
-00010c40: 6574 206f 7572 2063 7573 746f 6d20 5374  et our custom St
-00010c50: 6174 6963 4d69 6464 6c65 7761 7265 2f53  aticMiddleware/S
-00010c60: 7461 7469 6341 7070 2074 6f20 7365 7276  taticApp to serv
-00010c70: 6520 7374 6174 6963 2066 696c 6573 2066  e static files f
-00010c80: 726f 6d0a 2020 2020 2320 7468 6520 5079  rom.    # the Py
-00010c90: 7468 6f6e 206d 6f64 756c 6520 696e 7374  thon module inst
-00010ca0: 616c 6c61 7469 6f6e 2064 6972 6563 746f  allation directo
-00010cb0: 7279 2e0a 2020 2020 6163 6365 7373 0909  ry..    access..
-00010cc0: 093d 2063 6f6e 6669 672e 6765 7428 2027  .= config.get( '
-00010cd0: 6163 6365 7373 2720 290a 0a20 2020 2023  access' )..    #
-00010ce0: 204c 6f67 2077 6562 2e70 7920 4854 5450   Log web.py HTTP
-00010cf0: 2072 6571 7565 7374 7320 746f 206c 6963   requests to lic
-00010d00: 656e 7369 6e67 2e61 6363 6573 730a 2020  ensing.access.  
-00010d10: 2020 636c 6173 7320 4c6f 6753 7464 6f75    class LogStdou
-00010d20: 7428 2077 7367 696c 6f67 2e4c 6f67 5374  t( wsgilog.LogSt
-00010d30: 646f 7574 2029 3a0a 2020 2020 2020 2020  dout ):.        
-00010d40: 2222 2249 6d70 6c65 6d65 6e74 2074 6865  """Implement the
-00010d50: 206d 6973 7369 6e67 2066 6c75 7368 2041   missing flush A
-00010d60: 5049 2074 6f20 6176 6f69 6420 7761 726e  PI to avoid warn
-00010d70: 696e 6773 2222 220a 2020 2020 2020 2020  ings""".        
-00010d80: 6465 6620 666c 7573 6828 7365 6c66 293a  def flush(self):
-00010d90: 0a20 2020 2020 2020 2020 2020 2070 6173  .            pas
-00010da0: 730a 0a20 2020 2063 6c61 7373 204c 6f67  s..    class Log
-00010db0: 2820 7773 6769 6c6f 672e 5773 6769 4c6f  ( wsgilog.WsgiLo
-00010dc0: 672c 206f 626a 6563 7420 293a 0a20 2020  g, object ):.   
-00010dd0: 2020 2020 2022 2222 4469 7265 6374 206c       """Direct l
-00010de0: 6f67 206d 6573 7361 6765 7320 746f 2074  og messages to t
-00010df0: 6865 2063 6f72 7265 6374 206c 6f67 2066  he correct log f
-00010e00: 696c 652c 2069 6e63 6c75 6469 6e67 2073  ile, including s
-00010e10: 7464 6f75 742f 7374 6465 7272 2e20 2042  tdout/stderr.  B
-00010e20: 6563 6175 7365 2077 6527 7265 2072 756e  ecause we're run
-00010e30: 6e69 6e67 0a20 2020 2020 2020 2061 2063  ning.        a c
-00010e40: 7572 7365 7320 7465 7874 7561 6c20 5549  urses textual UI
-00010e50: 2c20 7765 2064 6f6e 2774 2077 616e 7420  , we don't want 
-00010e60: 7374 7566 6620 6265 696e 6720 7072 696e  stuff being prin
-00010e70: 7465 6420 746f 2074 6865 2073 6372 6565  ted to the scree
-00010e80: 6e20 6163 6369 6465 6e74 616c 6c79 202d  n accidentally -
-00010e90: 2d20 6d61 6b65 0a20 2020 2020 2020 2073  - make.        s
-00010ea0: 7572 6520 6974 2061 6c6c 2067 6f65 7320  ure it all goes 
-00010eb0: 746f 2074 6865 206c 6f67 2066 696c 652e  to the log file.
-00010ec0: 0a0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-00010ed0: 2020 2020 2020 6465 6620 5f5f 696e 6974        def __init
-00010ee0: 5f5f 2820 7365 6c66 2c20 6170 706c 6963  __( self, applic
-00010ef0: 6174 696f 6e20 293a 0a20 2020 2020 2020  ation ):.       
-00010f00: 2020 2020 2022 2222 5365 7420 7570 206c       """Set up l
-00010f10: 6f67 6769 6e67 2c20 616e 6420 7468 656e  ogging, and then
-00010f20: 206d 616b 6520 7375 7265 2073 7973 2e73   make sure sys.s
-00010f30: 7464 6572 7220 676f 6573 2074 6f20 7768  tderr goes to wh
-00010f40: 6572 6565 7665 7220 7379 732e 7374 646f  ereever sys.stdo
-00010f50: 7574 2069 7320 6e6f 7720 676f 696e 672e  ut is now going.
-00010f60: 2020 5468 6973 0a20 2020 2020 2020 2020    This.         
-00010f70: 2020 2065 6e73 7572 6573 2074 6861 7420     ensures that 
-00010f80: 656e 7669 726f 6e5b 2777 7367 692e 6572  environ['wsgi.er
-00010f90: 726f 7273 275d 2028 7768 6963 6820 6973  rors'] (which is
-00010fa0: 2061 6c77 6179 7320 7365 7420 746f 2073   always set to s
-00010fb0: 7973 2e73 7464 6572 7220 6279 2077 6562  ys.stderr by web
-00010fc0: 2e70 7929 2067 6f65 730a 2020 2020 2020  .py) goes.      
-00010fd0: 2020 2020 2020 746f 2074 6865 202e 6163        to the .ac
-00010fe0: 6365 7373 206c 6f67 2066 696c 653b 2074  cess log file; t
-00010ff0: 6869 7320 6973 2075 7365 6420 746f 206c  his is used to l
-00011000: 6f67 2065 6163 6820 696e 636f 6d69 6e67  og each incoming
-00011010: 2048 5454 5020 7265 7175 6573 742e 0a0a   HTTP request...
-00011020: 2020 2020 2020 2020 2020 2020 2222 220a              """.
-00011030: 2020 2020 2020 2020 2020 2020 6966 2061              if a
-00011040: 6363 6573 733a 0a20 2020 2020 2020 2020  ccess:.         
-00011050: 2020 2020 2020 2073 7570 6572 2820 4c6f         super( Lo
-00011060: 672c 2073 656c 6620 292e 5f5f 696e 6974  g, self ).__init
-00011070: 5f5f 280a 2020 2020 2020 2020 2020 2020  __(.            
-00011080: 2020 2020 2020 2020 6170 706c 6963 6174          applicat
-00011090: 696f 6e2c 0a20 2020 2020 2020 2020 2020  ion,.           
-000110a0: 2020 2020 2020 2020 206c 6f67 666f 726d           logform
-000110b0: 6174 093d 2022 2528 6d65 7373 6167 6529  at.= "%(message)
-000110c0: 7322 2c0a 2020 2020 2020 2020 2020 2020  s",.            
-000110d0: 2020 2020 2020 2020 6c6f 6709 093d 2054          log..= T
-000110e0: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
-000110f0: 2020 2020 2020 2020 2074 6f68 746d 6c09           tohtml.
-00011100: 3d20 5472 7565 2c09 0909 0923 2045 7863  = True,....# Exc
-00011110: 6570 7469 6f6e 7320 6765 6e65 7261 7465  eptions generate
-00011120: 2048 544d 4c0a 2020 2020 2020 2020 2020   HTML.          
-00011130: 2020 2020 2020 2020 2020 746f 6669 6c65            tofile
-00011140: 093d 2054 7275 652c 0909 0909 2320 4c6f  .= True,....# Lo
-00011150: 6767 696e 6720 676f 6573 2074 6f20 6163  gging goes to ac
-00011160: 6365 7373 206c 6f67 2066 696c 650a 2020  cess log file.  
-00011170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011180: 2020 6669 6c65 093d 2061 6363 6573 732c    file.= access,
-00011190: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000111a0: 2020 2020 2069 6e74 6572 7661 6c09 3d20       interval.= 
-000111b0: 2764 272c 0a20 2020 2020 2020 2020 2020  'd',.           
-000111c0: 2020 2020 2020 2020 2062 6163 6b75 7073           backups
-000111d0: 093d 2037 2c0a 2020 2020 2020 2020 2020  .= 7,.          
-000111e0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-000111f0: 2020 2020 2020 2020 2320 746f 7072 696e          # toprin
-00011200: 7420 646f 6573 2074 6869 7320 6175 746f  t does this auto
-00011210: 6d61 7469 6361 6c6c 7920 666f 7220 7379  matically for sy
-00011220: 732e 7374 646f 7574 3b20 7379 732e 7374  s.stdout; sys.st
-00011230: 6465 7272 2072 656d 6169 6e73 2075 6e63  derr remains unc
-00011240: 6861 6e67 6564 2e0a 2020 2020 2020 2020  hanged..        
-00011250: 2020 2020 2020 2020 2320 486f 7765 7665          # Howeve
-00011260: 722c 2074 6865 2064 6566 6175 6c74 204c  r, the default L
-00011270: 6f67 5374 646f 7574 2069 7320 6d69 7373  ogStdout is miss
-00011280: 696e 6720 6120 7265 7175 6972 6564 202e  ing a required .
-00011290: 666c 7573 6820 6d65 7468 6f64 2c20 736f  flush method, so
-000112a0: 2077 6527 6c6c 2073 6574 0a20 2020 2020   we'll set.     
-000112b0: 2020 2020 2020 2020 2020 2023 2074 6869             # thi
-000112c0: 7320 7570 206d 616e 7561 6c6c 7920 696e  s up manually in
-000112d0: 7374 6561 640a 2020 2020 2020 2020 2020  stead.          
-000112e0: 2020 2020 2020 7379 732e 7374 646f 7574        sys.stdout
-000112f0: 203d 2073 7973 2e73 7464 6572 7220 3d20   = sys.stderr = 
-00011300: 4c6f 6753 7464 6f75 7428 2073 656c 662e  LogStdout( self.
-00011310: 6c6f 6767 6572 2c20 6c6f 6767 696e 672e  logger, logging.
-00011320: 494e 464f 2029 0a20 2020 2020 2020 2020  INFO ).         
-00011330: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00011340: 2020 2020 2020 2020 2073 7570 6572 2820           super( 
-00011350: 4c6f 672c 2073 656c 6620 292e 5f5f 696e  Log, self ).__in
-00011360: 6974 5f5f 280a 2020 2020 2020 2020 2020  it__(.          
-00011370: 2020 2020 2020 2020 2020 6170 706c 6963            applic
-00011380: 6174 696f 6e2c 0a20 2020 2020 2020 2020  ation,.         
-00011390: 2020 2020 2020 2020 2020 206c 6f67 666f             logfo
-000113a0: 726d 6174 093d 2022 2528 6d65 7373 6167  rmat.= "%(messag
-000113b0: 6529 7322 2c0a 2020 2020 2020 2020 2020  e)s",.          
-000113c0: 2020 2020 2020 2020 2020 6c6f 6709 093d            log..=
-000113d0: 2054 7275 652c 0a20 2020 2020 2020 2020   True,.         
-000113e0: 2020 2020 2020 2020 2020 2074 6f68 746d             tohtm
-000113f0: 6c09 3d20 5472 7565 2c09 0909 0923 2045  l.= True,....# E
-00011400: 7863 6570 7469 6f6e 7320 6765 6e65 7261  xceptions genera
-00011410: 7465 2048 544d 4c0a 2020 2020 2020 2020  te HTML.        
-00011420: 2020 2020 2020 2020 2020 2020 746f 7374              tost
-00011430: 7265 616d 093d 2054 7275 652c 0909 0909  ream.= True,....
-00011440: 2320 4c6f 6767 696e 6720 676f 6573 2074  # Logging goes t
-00011450: 6f20 7374 646f 7574 0a20 2020 2020 2020  o stdout.       
-00011460: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
-00011470: 6675 6e63 0909 093d 2061 7070 2e77 7367  func...= app.wsg
-00011480: 6966 756e 6328 204c 6f67 2029 0a20 2020  ifunc( Log ).   
-00011490: 2066 756e 6309 0909 3d20 5374 6174 6963   func...= Static
-000114a0: 4d69 6464 6c65 7761 7265 4469 7228 2066  MiddlewareDir( f
-000114b0: 756e 632c 2022 2f73 7461 7469 632f 222c  unc, "/static/",
-000114c0: 206f 732e 7061 7468 2e64 6972 6e61 6d65   os.path.dirname
-000114d0: 2820 5f5f 6669 6c65 5f5f 2029 290a 2020  ( __file__ )).  
-000114e0: 2020 6675 6e63 0909 093d 204c 6f67 4d69    func...= LogMi
-000114f0: 6464 6c65 7761 7265 4346 2820 6675 6e63  ddlewareCF( func
-00011500: 2029 2020 2020 2020 2023 2077 6562 2e68   )       # web.h
-00011510: 7474 7073 6572 7665 722e 4c6f 674d 6964  ttpserver.LogMid
-00011520: 646c 6577 6172 6528 2061 7070 2029 0a0a  dleware( app )..
-00011530: 2020 2020 2320 7765 6270 792e 7365 7276      # webpy.serv
-00011540: 6572 0909 3d20 7765 622e 6874 7470 7365  er..= web.httpse
-00011550: 7276 6572 2e57 5347 4953 6572 7665 7228  rver.WSGIServer(
-00011560: 2063 6f6e 6669 675b 2761 6464 7265 7373   config['address
-00011570: 275d 2c20 6170 7020 290a 0a20 2020 2023  '], app )..    #
-00011580: 2054 6869 7320 6973 2061 2043 6865 7272   This is a Cherr
-00011590: 7950 7920 2863 6865 726f 6f74 2920 5365  yPy (cheroot) Se
-000115a0: 7276 6572 2e20 2057 6520 6861 7665 2074  rver.  We have t
-000115b0: 6f20 696e 7465 7263 6570 7420 2e73 6572  o intercept .ser
-000115c0: 7665 2829 2c20 746f 2070 7269 6e74 2074  ve(), to print t
-000115d0: 6865 2061 6374 7561 6c6c 790a 2020 2020  he actually.    
-000115e0: 2320 626f 756e 6420 7765 6220 7365 7276  # bound web serv
-000115f0: 6572 2061 6464 7265 7373 2028 6567 2e20  er address (eg. 
-00011600: 6966 2075 7369 6e67 2061 2064 796e 616d  if using a dynam
-00011610: 6963 616c 6c79 2061 6c6c 6f63 6174 6564  ically allocated
-00011620: 2070 6f72 7429 2e20 2054 6869 7320 7769   port).  This wi
-00011630: 6c6c 2062 6520 7265 6469 7265 6374 6564  ll be redirected
-00011640: 0a20 2020 2023 2074 6f20 7468 6520 6163  .    # to the ac
-00011650: 6365 7373 206c 6f67 6669 6c65 2c20 756e  cess logfile, un
-00011660: 6c65 7373 2064 6973 6162 6c65 6420 7669  less disabled vi
-00011670: 6120 2d2d 6e6f 2d61 6363 6573 732e 2020  a --no-access.  
-00011680: 416c 736f 2c20 7468 6973 2063 6c61 7373  Also, this class
-00011690: 2077 6569 7264 6c79 2063 6170 7475 7265   weirdly capture
-000116a0: 7320 636f 6e66 6967 2c20 736f 2077 6520  s config, so we 
-000116b0: 6361 6e20 7570 6461 7465 0a20 2020 2066  can update.    f
-000116c0: 726f 6d20 6368 6572 6f6f 7420 696d 706f  rom cheroot impo
-000116d0: 7274 2077 7367 690a 0a20 2020 2063 6c61  rt wsgi..    cla
-000116e0: 7373 2053 6572 7665 7228 2077 7367 692e  ss Server( wsgi.
-000116f0: 5365 7276 6572 2c20 6f62 6a65 6374 2029  Server, object )
-00011700: 3a0a 2020 2020 2020 2020 6465 6620 7365  :.        def se
-00011710: 7276 6528 2073 656c 6620 293a 0a20 2020  rve( self ):.   
-00011720: 2020 2020 2020 2020 2073 6f63 6b6e 616d           socknam
-00011730: 6509 093d 2073 656c 662e 736f 636b 6574  e..= self.socket
-00011740: 2e67 6574 736f 636b 6e61 6d65 2829 0a20  .getsockname(). 
-00011750: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-00011760: 2820 2257 6562 2049 6e74 6572 6661 6365  ( "Web Interface
-00011770: 2054 4350 2061 6464 7265 7373 203d 207b   TCP address = {
-00011780: 736f 636b 6e61 6d65 2172 7d22 2e66 6f72  sockname!r}".for
-00011790: 6d61 7428 2073 6f63 6b6e 616d 653d 736f  mat( sockname=so
-000117a0: 636b 6e61 6d65 2029 290a 2020 2020 2020  ckname )).      
-000117b0: 2020 2020 2020 7379 732e 7374 646f 7574        sys.stdout
-000117c0: 2e66 6c75 7368 2829 0a20 2020 2020 2020  .flush().       
-000117d0: 2020 2020 2063 6f6e 6669 675b 2763 6f6e       config['con
-000117e0: 7472 6f6c 275d 5b27 6164 6472 6573 7327  trol']['address'
-000117f0: 5d20 3d20 736f 636b 6e61 6d65 0a20 2020  ] = sockname.   
-00011800: 2020 2020 2020 2020 2073 7570 6572 2820           super( 
-00011810: 5365 7276 6572 2c20 7365 6c66 2029 2e73  Server, self ).s
-00011820: 6572 7665 2829 0a0a 2020 2020 2320 4669  erve()..    # Fi
-00011830: 6e61 6c6c 792c 206d 616b 6520 7468 6520  nally, make the 
-00011840: 5365 7276 6572 2061 7661 696c 6162 6c65  Server available
-00011850: 206f 6e20 7468 6520 6675 6e63 7469 6f6e   on the function
-00011860: 2773 2077 6562 7079 2e73 6572 7665 7220  's webpy.server 
-00011870: 666f 7220 6578 7465 726e 616c 2061 6363  for external acc
-00011880: 6573 730a 2020 2020 7765 6270 792e 7365  ess.    webpy.se
-00011890: 7276 6572 0909 3d20 5365 7276 6572 2820  rver..= Server( 
-000118a0: 636f 6e66 6967 5b27 6164 6472 6573 7327  config['address'
-000118b0: 5d2c 2066 756e 632c 2073 6572 7665 725f  ], func, server_
-000118c0: 6e61 6d65 3d22 6c6f 6361 6c68 6f73 7422  name="localhost"
-000118d0: 2029 0a20 2020 2077 6562 7079 2e73 6572   ).    webpy.ser
-000118e0: 7665 722e 6e6f 6465 6c61 7909 3d20 5472  ver.nodelay.= Tr
-000118f0: 7565 0a0a 2020 2020 7472 793a 0a20 2020  ue..    try:.   
-00011900: 2020 2020 206c 6f67 2e77 6172 6e69 6e67       log.warning
-00011910: 2820 2257 6562 2049 6e74 6572 6661 6365  ( "Web Interface
-00011920: 2073 7461 7274 696e 6722 2029 0a20 2020   starting" ).   
-00011930: 2020 2020 2077 6562 7079 2e73 6572 7665       webpy.serve
-00011940: 722e 7374 6172 7428 290a 2020 2020 6578  r.start().    ex
-00011950: 6365 7074 2028 4b65 7962 6f61 7264 496e  cept (KeyboardIn
-00011960: 7465 7272 7570 742c 2053 7973 7465 6d45  terrupt, SystemE
-00011970: 7869 7429 2061 7320 6578 633a 0a20 2020  xit) as exc:.   
-00011980: 2020 2020 206c 6f67 6769 6e67 2e77 6172       logging.war
-00011990: 6e69 6e67 2820 2257 6562 2049 6e74 6572  ning( "Web Inter
-000119a0: 6661 6365 2054 6872 6561 6420 756e 636f  face Thread unco
-000119b0: 6e74 726f 6c6c 6564 2073 6875 7464 6f77  ntrolled shutdow
-000119c0: 6e3a 2025 7322 2c20 6578 6320 290a 2020  n: %s", exc ).  
-000119d0: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
-000119e0: 6f6e 2061 7320 6578 633a 0a20 2020 2020  on as exc:.     
-000119f0: 2020 206c 6f67 6769 6e67 2e77 6172 6e69     logging.warni
-00011a00: 6e67 2820 2257 6562 2049 6e74 6572 6661  ng( "Web Interfa
-00011a10: 6365 2054 6872 6561 6420 6578 6365 7074  ce Thread except
-00011a20: 696f 6e20 7368 7574 646f 776e 3a20 2573  ion shutdown: %s
-00011a30: 222c 2065 7863 2029 0a20 2020 2066 696e  ", exc ).    fin
-00011a40: 616c 6c79 3a0a 2020 2020 2020 2020 6c6f  ally:.        lo
-00011a50: 6767 696e 672e 696e 666f 2820 2257 6562  gging.info( "Web
-00011a60: 2049 6e74 6572 6661 6365 2054 6872 6561   Interface Threa
-00011a70: 6420 7374 6f70 7069 6e67 2e2e 2e22 2029  d stopping..." )
-00011a80: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
-00011a90: 2020 2020 2020 2020 2020 7765 6270 792e            webpy.
-00011aa0: 7365 7276 6572 2e73 746f 7028 290a 2020  server.stop().  
-00011ab0: 2020 2020 2020 6578 6365 7074 2045 7863        except Exc
-00011ac0: 6570 7469 6f6e 2061 7320 6578 633a 0a20  eption as exc:. 
-00011ad0: 2020 2020 2020 2020 2020 206c 6f67 6769             loggi
-00011ae0: 6e67 2e77 6172 6e69 6e67 2820 2257 6562  ng.warning( "Web
-00011af0: 2049 6e74 6572 6661 6365 2054 6872 6561   Interface Threa
-00011b00: 6420 7374 6f70 2066 6169 6c75 7265 3a20  d stop failure: 
-00011b10: 2573 222c 2065 7863 2029 0a20 2020 2020  %s", exc ).     
-00011b20: 2020 2077 6562 7079 2e73 6572 7665 7209     webpy.server.
-00011b30: 093d 204e 6f6e 650a 2020 2020 2020 2020  .= None.        
-00011b40: 6c6f 6767 696e 672e 7761 726e 696e 6728  logging.warning(
-00011b50: 2022 5765 6220 496e 7465 7266 6163 6520   "Web Interface 
-00011b60: 5468 7265 6164 2065 7869 7469 6e67 2220  Thread exiting" 
-00011b70: 290a 0a0a 2320 546f 2073 746f 7020 7468  )...# To stop th
-00011b80: 6520 7365 7276 6572 2065 7874 6572 6e61  e server externa
-00011b90: 6c6c 792c 2068 6974 2077 6562 7079 2e73  lly, hit webpy.s
-00011ba0: 6572 7665 722e 7374 6f70 0a77 6562 7079  erver.stop.webpy
-00011bb0: 2e73 6572 7665 7209 0909 3d20 4e6f 6e65  .server...= None
-00011bc0: 0a0a 0a64 6566 2074 7874 6775 6928 2063  ...def txtgui( c
-00011bd0: 6f6e 6669 6720 293a 0a20 2020 2022 2222  onfig ):.    """
-00011be0: 5275 6e20 6375 7273 6573 2055 492c 2063  Run curses UI, c
-00011bf0: 6174 6368 696e 6720 616c 6c20 6578 6365  atching all exce
-00011c00: 7074 696f 6e73 2e20 2052 6574 7572 6e73  ptions.  Returns
-00011c10: 2054 7275 6520 6f6e 2066 6169 6c75 7265   True on failure
-00011c20: 2e22 2222 0a20 2020 2066 6169 6c75 7265  .""".    failure
-00011c30: 0909 093d 204e 6f6e 650a 2020 2020 7472  ...= None.    tr
-00011c40: 793a 2020 2020 2020 2020 2320 496e 6974  y:        # Init
-00011c50: 6961 6c69 7a65 2063 7572 7365 730a 2020  ialize curses.  
-00011c60: 2020 2020 2020 7374 6473 6372 0909 093d        stdscr...=
-00011c70: 2063 7572 7365 732e 696e 6974 7363 7228   curses.initscr(
-00011c80: 290a 2020 2020 2020 2020 6375 7273 6573  ).        curses
-00011c90: 2e6e 6f65 6368 6f28 290a 2020 2020 2020  .noecho().      
-00011ca0: 2020 6375 7273 6573 2e63 6272 6561 6b28    curses.cbreak(
-00011cb0: 290a 2020 2020 2020 2020 6375 7273 6573  ).        curses
-00011cc0: 2e68 616c 6664 656c 6179 2820 3120 290a  .halfdelay( 1 ).
-00011cd0: 2020 2020 2020 2020 7374 6473 6372 2e6b          stdscr.k
-00011ce0: 6579 7061 6428 2031 2029 0a0a 2020 2020  eypad( 1 )..    
-00011cf0: 2020 2020 7478 7428 2073 7464 7363 722c      txt( stdscr,
-00011d00: 2063 6f6e 6669 6720 2920 2020 2020 2020   config )       
-00011d10: 2020 2020 2020 2020 2320 456e 7465 7220          # Enter 
-00011d20: 7468 6520 4375 7273 6573 206d 6169 6e6c  the Curses mainl
-00011d30: 6f6f 700a 2020 2020 6578 6365 7074 2045  oop.    except E
-00011d40: 7863 6570 7469 6f6e 3a0a 2020 2020 2020  xception:.      
-00011d50: 2020 6661 696c 7572 6509 0909 3d20 7472    failure...= tr
-00011d60: 6163 6562 6163 6b2e 666f 726d 6174 5f65  aceback.format_e
-00011d70: 7863 2829 0a20 2020 2066 696e 616c 6c79  xc().    finally
-00011d80: 3a0a 2020 2020 2020 2020 636f 6e66 6967  :.        config
-00011d90: 2e73 6574 6465 6661 756c 7428 2027 636f  .setdefault( 'co
-00011da0: 6e74 726f 6c27 2c20 7b7d 2029 5b27 646f  ntrol', {} )['do
-00011db0: 6e65 275d 203d 2054 7275 650a 2020 2020  ne'] = True.    
-00011dc0: 2020 2020 7374 6473 6372 2e6b 6579 7061      stdscr.keypa
-00011dd0: 6428 3029 0a20 2020 2020 2020 2063 7572  d(0).        cur
-00011de0: 7365 732e 6563 686f 2829 0a20 2020 2020  ses.echo().     
-00011df0: 2020 2063 7572 7365 732e 6e6f 6362 7265     curses.nocbre
-00011e00: 616b 2829 0a20 2020 2020 2020 2063 7572  ak().        cur
-00011e10: 7365 732e 656e 6477 696e 2829 0a20 2020  ses.endwin().   
-00011e20: 2020 2020 2074 696d 652e 736c 6565 7028       time.sleep(
-00011e30: 2e32 3529 0a20 2020 2069 6620 6661 696c  .25).    if fail
-00011e40: 7572 653a 0a20 2020 2020 2020 206c 6f67  ure:.        log
-00011e50: 6769 6e67 2e65 7272 6f72 2820 2243 7572  ging.error( "Cur
-00011e60: 7365 7320 4755 4920 4578 6365 7074 696f  ses GUI Exceptio
-00011e70: 6e3a 2025 7322 2c20 6661 696c 7572 6520  n: %s", failure 
-00011e80: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00011e90: 2054 7275 650a 2020 2020 7265 7475 726e   True.    return
-00011ea0: 2046 616c 7365 0a0a 0a64 6566 2063 746c   False...def ctl
-00011eb0: 6c6f 6f70 2820 6265 672c 2063 6e66 2029  loop( beg, cnf )
-00011ec0: 3a0a 2020 2020 2222 2245 7865 6375 7465  :.    """Execute
-00011ed0: 206f 6e65 206c 6f6f 7020 6f66 2074 6865   one loop of the
-00011ee0: 2063 6f6e 7472 6f6c 2073 7973 7465 6d22   control system"
-00011ef0: 2222 0a20 2020 2070 6173 730a 0a0a 6465  "".    pass...de
-00011f00: 6620 6d61 696e 2820 6172 6776 3d4e 6f6e  f main( argv=Non
-00011f10: 652c 202a 2a6c 6963 656e 7369 6e67 5f6b  e, **licensing_k
-00011f20: 7764 7320 293a 0a20 2020 2022 2222 5061  wds ):.    """Pa
-00011f30: 7373 2074 6865 2064 6573 6972 6564 2061  ss the desired a
-00011f40: 7267 7620 2865 7863 6c75 6469 6e67 2074  rgv (excluding t
-00011f50: 6865 2070 726f 6772 616d 206e 616d 6520  he program name 
-00011f60: 696e 2073 7973 2e61 7267 5b30 5d3b 2074  in sys.arg[0]; t
-00011f70: 7970 6963 616c 6c79 2070 6173 7320 6172  ypically pass ar
-00011f80: 6776 3d4e 6f6e 652c 2077 6869 6368 0a20  gv=None, which. 
-00011f90: 2020 2069 7320 6571 7569 7661 6c65 6e74     is equivalent
-00011fa0: 2074 6f20 6172 6776 3d73 7973 2e61 7267   to argv=sys.arg
-00011fb0: 765b 313a 5d2c 2074 6865 2064 6566 6175  v[1:], the defau
-00011fc0: 6c74 2066 6f72 2061 7267 7061 7273 652e  lt for argparse.
-00011fd0: 2020 5265 7175 6972 6573 2061 7420 6c65    Requires at le
-00011fe0: 6173 7420 6f6e 6520 7461 6720 746f 2062  ast one tag to b
-00011ff0: 650a 2020 2020 6465 6669 6e65 642e 0a20  e.    defined.. 
-00012000: 2020 2022 2222 0a0a 2020 2020 6170 0909     """..    ap..
-00012010: 0909 3d20 6172 6770 6172 7365 2e41 7267  ..= argparse.Arg
-00012020: 756d 656e 7450 6172 7365 7228 0a20 2020  umentParser(.   
-00012030: 2020 2020 2064 6573 6372 6970 7469 6f6e       description
-00012040: 093d 2022 4120 4370 7070 6f20 4372 7970  .= "A Cpppo Cryp
-00012050: 746f 204c 6963 656e 7369 6e67 2053 6572  to Licensing Ser
-00012060: 7665 7222 2c0a 2020 2020 2020 2020 666f  ver",.        fo
-00012070: 726d 6174 7465 725f 636c 6173 7320 3d20  rmatter_class = 
-00012080: 6172 6770 6172 7365 2e52 6177 4465 7363  argparse.RawDesc
-00012090: 7269 7074 696f 6e48 656c 7046 6f72 6d61  riptionHelpForma
-000120a0: 7474 6572 2c0a 2020 2020 2020 2020 6570  tter,.        ep
-000120b0: 696c 6f67 0909 3d20 2222 225c 0a49 6d70  ilog..= """\.Imp
-000120c0: 6c65 6d65 6e74 7320 4564 3235 3531 392d  lements Ed25519-
-000120d0: 7369 676e 6564 2063 7279 7074 6f67 7261  signed cryptogra
-000120e0: 7068 6963 206c 6963 656e 7369 6e67 2077  phic licensing w
-000120f0: 6562 2073 6572 7669 6365 2061 6e64 2041  eb service and A
-00012100: 5049 2e0a 0a49 7373 7565 7320 6c69 6365  PI...Issues lice
-00012110: 6e73 6528 7329 2066 6f72 2070 726f 6475  nse(s) for produ
-00012120: 6374 7320 616e 6420 6361 7061 6269 6c69  cts and capabili
-00012130: 7469 6573 2061 7661 696c 6162 6c65 2074  ties available t
-00012140: 6f20 7468 6520 636c 6965 6e74 2c20 7768  o the client, wh
-00012150: 6572 6520 6569 7468 6572 0a0a 2020 4129  ere either..  A)
-00012160: 2074 6865 2073 6572 7665 7220 6861 7320   the server has 
-00012170: 6372 6564 656e 7469 616c 7320 696e 6469  credentials indi
-00012180: 6361 7469 6e67 206f 776e 6572 7368 6970  cating ownership
-00012190: 206f 6620 7468 6520 4c69 6365 6e73 6573   of the Licenses
-000121a0: 2c20 616e 6420 6865 6e63 650a 2020 2020  , and hence.    
-000121b0: 2061 7574 686f 7269 7479 2074 6f20 7375   authority to su
-000121c0: 622d 6c69 6365 6e73 6520 7468 656d 2c20  b-license them, 
-000121d0: 6f72 0a0a 2020 4229 2074 6865 204c 6963  or..  B) the Lic
-000121e0: 656e 7365 2069 7473 656c 6620 6772 616e  ense itself gran
-000121f0: 7473 2061 7574 686f 7269 7479 2074 6f20  ts authority to 
-00012200: 6265 2073 7562 2d6c 6963 656e 7365 6420  be sub-licensed 
-00012210: 746f 2061 6e79 2041 6765 6e74 0a20 2020  to any Agent.   
-00012220: 2020 6173 6b69 6e67 2066 6f72 2061 204c    asking for a L
-00012230: 6963 656e 7365 0a0a 5072 6f64 7563 6573  icense..Produces
-00012240: 2069 6e76 6f69 6365 7320 666f 7220 6561   invoices for ea
-00012250: 6368 2074 7261 6e73 6163 7469 6f6e 0a0a  ch transaction..
-00012260: 5065 7266 6f72 6d61 6e63 6520 6265 6e65  Performance bene
-00012270: 6669 7473 2067 7265 6174 6c79 2066 726f  fits greatly fro
-00012280: 6d20 696e 7374 616c 6c61 7469 6f6e 206f  m installation o
-00012290: 6620 286f 7074 696f 6e61 6c29 2065 6432  f (optional) ed2
-000122a0: 3535 3139 6c6c 2070 6163 6b61 6765 3a0a  5519ll package:.
-000122b0: 0a20 2020 2070 7974 686f 6e33 202d 6d20  .    python3 -m 
-000122c0: 7069 7020 696e 7374 616c 6c20 6564 3235  pip install ed25
-000122d0: 3531 396c 6c0a 2222 220a 2020 2020 290a  519ll.""".    ).
-000122e0: 2020 2020 6170 2e61 6464 5f61 7267 756d      ap.add_argum
-000122f0: 656e 7428 2027 2d76 272c 2027 2d2d 7665  ent( '-v', '--ve
-00012300: 7262 6f73 6527 2c20 6163 7469 6f6e 3d22  rbose', action="
-00012310: 636f 756e 7422 2c0a 2020 2020 2020 2020  count",.        
-00012320: 2020 2020 2020 2020 2020 2020 2064 6566               def
-00012330: 6175 6c74 3d30 2c0a 2020 2020 2020 2020  ault=0,.        
-00012340: 2020 2020 2020 2020 2020 2020 2068 656c               hel
-00012350: 703d 2244 6973 706c 6179 206c 6f67 6769  p="Display loggi
-00012360: 6e67 2069 6e66 6f72 6d61 7469 6f6e 2e22  ng information."
-00012370: 2029 0a20 2020 2061 702e 6164 645f 6172   ).    ap.add_ar
-00012380: 6775 6d65 6e74 2820 272d 7127 2c20 272d  gument( '-q', '-
-00012390: 2d71 7569 6574 272c 2061 6374 696f 6e3d  -quiet', action=
-000123a0: 2263 6f75 6e74 222c 0a20 2020 2020 2020  "count",.       
-000123b0: 2020 2020 2020 2020 2020 2020 2020 6465                de
-000123c0: 6661 756c 743d 302c 0a20 2020 2020 2020  fault=0,.       
-000123d0: 2020 2020 2020 2020 2020 2020 2020 6865                he
-000123e0: 6c70 3d22 5265 6475 6365 206c 6f67 6769  lp="Reduce loggi
-000123f0: 6e67 206f 7574 7075 742e 2220 290a 2020  ng output." ).  
-00012400: 2020 6170 2e61 6464 5f61 7267 756d 656e    ap.add_argumen
-00012410: 7428 2027 2d77 272c 2027 2d2d 7765 6227  t( '-w', '--web'
-00012420: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00012430: 2020 2020 2020 2064 6566 6175 6c74 3d22         default="
-00012440: 302e 302e 302e 303a 3830 3030 222c 0a20  0.0.0.0:8000",. 
-00012450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012460: 2020 2020 6865 6c70 3d27 656e 6162 6c65      help='enable
-00012470: 2077 6562 2073 6572 7665 7220 6f6e 2069   web server on i
-00012480: 6e74 6572 6661 6365 2028 6465 6661 756c  nterface (defaul
-00012490: 743a 2030 2e30 2e30 2e30 3a38 3030 3029  t: 0.0.0.0:8000)
-000124a0: 2720 290a 2020 2020 6170 2e61 6464 5f61  ' ).    ap.add_a
-000124b0: 7267 756d 656e 7428 2027 2d2d 6e6f 2d77  rgument( '--no-w
-000124c0: 6562 272c 2064 6573 743d 2777 6562 272c  eb', dest='web',
-000124d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000124e0: 2020 2020 2020 6163 7469 6f6e 3d22 7374        action="st
-000124f0: 6f72 655f 6661 6c73 6522 2c0a 2020 2020  ore_false",.    
-00012500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012510: 2068 656c 703d 2744 6973 6162 6c65 2077   help='Disable w
-00012520: 6562 2069 6e74 6572 6661 6365 2061 6e64  eb interface and
-00012530: 2061 6363 6573 7320 6c6f 6720 6669 6c65   access log file
-00012540: 2028 6465 6661 756c 743a 2046 616c 7365   (default: False
-00012550: 2927 2029 0a20 2020 2061 702e 6164 645f  )' ).    ap.add_
-00012560: 6172 6775 6d65 6e74 2820 272d 2d61 6363  argument( '--acc
-00012570: 6573 7327 2c0a 2020 2020 2020 2020 2020  ess',.          
-00012580: 2020 2020 2020 2020 2020 2064 6566 6175             defau
-00012590: 6c74 3d41 4343 4649 4c45 2c0a 2020 2020  lt=ACCFILE,.    
-000125a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000125b0: 2068 656c 703d 224c 6f67 2061 6c6c 2077   help="Log all w
-000125c0: 6562 2073 6572 7665 7220 6163 6365 7373  eb server access
-000125d0: 2074 6f20 6c6f 6720 6669 6c65 2028 6465   to log file (de
-000125e0: 6661 756c 743a 207b 4143 4346 494c 457d  fault: {ACCFILE}
-000125f0: 222e 666f 726d 6174 280a 2020 2020 2020  ".format(.      
-00012600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012610: 2020 2041 4343 4649 4c45 3d41 4343 4649     ACCFILE=ACCFI
-00012620: 4c45 2029 290a 2020 2020 6170 2e61 6464  LE )).    ap.add
-00012630: 5f61 7267 756d 656e 7428 2027 2d2d 6e6f  _argument( '--no
-00012640: 2d61 6363 6573 7327 2c20 6465 7374 3d27  -access', dest='
-00012650: 6163 6365 7373 272c 0a20 2020 2020 2020  access',.       
-00012660: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00012670: 6e73 743d 4e6f 6e65 2c20 6163 7469 6f6e  nst=None, action
-00012680: 3d22 7374 6f72 655f 636f 6e73 7422 2c0a  ="store_const",.
-00012690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000126a0: 2020 2020 2068 656c 703d 2744 6973 6162       help='Disab
-000126b0: 6c65 2077 6562 2073 6572 7665 7220 6163  le web server ac
-000126c0: 6365 7373 206c 6f67 2066 696c 652c 2069  cess log file, i
-000126d0: 6e63 6c75 6469 6e67 2073 7464 6f75 742f  ncluding stdout/
-000126e0: 7374 6465 7272 2072 6564 6972 6563 7469  stderr redirecti
-000126f0: 6f6e 2720 290a 2020 2020 6170 2e61 6464  on' ).    ap.add
-00012700: 5f61 7267 756d 656e 7428 2027 2d2d 6e6f  _argument( '--no
-00012710: 2d67 7569 272c 2064 6573 743d 2767 7569  -gui', dest='gui
-00012720: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
-00012730: 2020 2020 2020 2020 6465 6661 756c 743d          default=
-00012740: 5472 7565 2c20 6163 7469 6f6e 3d22 7374  True, action="st
-00012750: 6f72 655f 6661 6c73 6522 2c0a 2020 2020  ore_false",.    
-00012760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012770: 2068 656c 703d 2744 6973 6162 6c65 2043   help='Disable C
-00012780: 7572 7365 7320 4755 4920 696e 7465 7266  urses GUI interf
-00012790: 6163 6520 2864 6566 6175 6c74 3a20 4661  ace (default: Fa
-000127a0: 6c73 6529 2720 290a 2020 2020 6170 2e61  lse)' ).    ap.a
-000127b0: 6464 5f61 7267 756d 656e 7428 2027 2d63  dd_argument( '-c
-000127c0: 272c 2027 2d2d 636f 6e66 6967 272c 0a20  ', '--config',. 
-000127d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000127e0: 2020 2020 6163 7469 6f6e 3d27 6170 7065      action='appe
-000127f0: 6e64 272c 0a20 2020 2020 2020 2020 2020  nd',.           
-00012800: 2020 2020 2020 2020 2020 6865 6c70 3d22            help="
-00012810: 4164 6420 616e 6f74 6865 7220 2868 6967  Add another (hig
-00012820: 6865 7220 7072 696f 7269 7479 2920 636f  her priority) co
-00012830: 6e66 6967 2066 696c 6520 7061 7468 2e22  nfig file path."
-00012840: 2029 0a20 2020 2061 702e 6164 645f 6172   ).    ap.add_ar
-00012850: 6775 6d65 6e74 2820 272d 6c27 2c20 272d  gument( '-l', '-
-00012860: 2d6c 6f67 272c 0a20 2020 2020 2020 2020  -log',.         
-00012870: 2020 2020 2020 2020 2020 2020 6465 6661              defa
-00012880: 756c 743d 4e6f 6e65 2c0a 2020 2020 2020  ult=None,.      
-00012890: 2020 2020 2020 2020 2020 2020 2020 2068                 h
-000128a0: 656c 703d 224c 6f67 2066 696c 652c 2069  elp="Log file, i
-000128b0: 6620 6465 7369 7265 6420 2864 6566 6175  f desired (defau
-000128c0: 6c74 2c20 6966 2074 6578 7420 6775 693a  lt, if text gui:
-000128d0: 207b 4c4f 4746 494c 457d 2922 2e66 6f72   {LOGFILE})".for
-000128e0: 6d61 7428 204c 4f47 4649 4c45 3d4c 4f47  mat( LOGFILE=LOG
-000128f0: 4649 4c45 2029 290a 2020 2020 6170 2e61  FILE )).    ap.a
-00012900: 6464 5f61 7267 756d 656e 7428 2027 2d2d  dd_argument( '--
-00012910: 7072 6f66 696c 6527 2c0a 2020 2020 2020  profile',.      
-00012920: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00012930: 6566 6175 6c74 3d4e 6f6e 652c 0a20 2020  efault=None,.   
-00012940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012950: 2020 6865 6c70 3d22 5072 6f66 696c 6520    help="Profile 
-00012960: 746f 2073 7464 6572 7220 286f 6e6c 792c  to stderr (only,
-00012970: 2069 6620 272d 2720 7370 6563 6966 6965   if '-' specifie
-00012980: 6429 2c20 6f70 7469 6f6e 616c 6c79 2073  d), optionally s
-00012990: 6176 696e 6720 6461 7461 2074 6f20 6120  aving data to a 
-000129a0: 6669 6c65 2028 6465 6661 756c 743a 204e  file (default: N
-000129b0: 6f6e 6529 2220 290a 2020 2020 6170 2e61  one)" ).    ap.a
-000129c0: 6464 5f61 7267 756d 656e 7428 2027 2d2d  dd_argument( '--
-000129d0: 636c 6965 6e74 272c 0a20 2020 2020 2020  client',.       
-000129e0: 2020 2020 2020 2020 2020 2020 2020 6465                de
-000129f0: 6661 756c 743d 4e6f 6e65 2c0a 2020 2020  fault=None,.    
-00012a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012a10: 2068 656c 703d 2254 6869 7320 7b44 4953   help="This {DIS
-00012a20: 5452 4942 5554 494f 4e7d 7365 7276 6572  TRIBUTION}server
-00012a30: 2773 2063 6c69 656e 7420 6c69 6365 6e73  's client licens
-00012a40: 6565 2773 2063 6f6d 7061 6e79 206e 616d  ee's company nam
-00012a50: 6522 2e66 6f72 6d61 7428 0a20 2020 2020  e".format(.     
-00012a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012a70: 2020 2020 4449 5354 5249 4255 5449 4f4e      DISTRIBUTION
-00012a80: 3d6c 6963 656e 7369 6e67 2e44 4953 5452  =licensing.DISTR
-00012a90: 4942 5554 494f 4e20 2929 0a20 2020 2061  IBUTION )).    a
-00012aa0: 702e 6164 645f 6172 6775 6d65 6e74 2820  p.add_argument( 
-00012ab0: 272d 2d64 6f6d 6169 6e27 2c0a 2020 2020  '--domain',.    
-00012ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ad0: 2064 6566 6175 6c74 3d4e 6f6e 652c 0a20   default=None,. 
-00012ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012af0: 2020 2020 6865 6c70 3d22 5468 6973 207b      help="This {
-00012b00: 4449 5354 5249 4255 5449 4f4e 7d20 7365  DISTRIBUTION} se
-00012b10: 7276 6572 2773 2063 6c69 656e 7420 6c69  rver's client li
-00012b20: 6365 6e73 6565 2773 2064 6f6d 6169 6e3b  censee's domain;
-00012b30: 2063 616e 2062 6520 7573 6564 2074 6f20   can be used to 
-00012b40: 6765 7420 7075 626c 6963 206b 6579 2076  get public key v
-00012b50: 6961 2044 4b49 4d22 2e66 6f72 6d61 7428  ia DKIM".format(
-00012b60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012b70: 2020 2020 2020 2020 2020 4449 5354 5249            DISTRI
-00012b80: 4255 5449 4f4e 3d6c 6963 656e 7369 6e67  BUTION=licensing
-00012b90: 2e44 4953 5452 4942 5554 494f 4e20 2929  .DISTRIBUTION ))
-00012ba0: 0a20 2020 2061 702e 6164 645f 6172 6775  .    ap.add_argu
-00012bb0: 6d65 6e74 2820 272d 2d70 726f 6475 6374  ment( '--product
-00012bc0: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
-00012bd0: 2020 2020 2020 2020 6465 6661 756c 743d          default=
-00012be0: 6c69 6365 6e73 696e 672e 5052 4f44 5543  licensing.PRODUC
-00012bf0: 545f 5345 5256 4552 2c0a 2020 2020 2020  T_SERVER,.      
-00012c00: 2020 2020 2020 2020 2020 2020 2020 2068                 h
-00012c10: 656c 703d 2254 6869 7320 7b44 4953 5452  elp="This {DISTR
-00012c20: 4942 5554 494f 4e7d 2073 6572 7665 7227  IBUTION} server'
-00012c30: 7320 636c 6965 6e74 206c 6963 656e 7365  s client license
-00012c40: 6527 7320 7072 6f64 7563 7420 6e61 6d65  e's product name
-00012c50: 2028 6966 2061 6e79 3b20 6465 6661 756c   (if any; defaul
-00012c60: 743a 207b 5052 4f44 5543 547d 2922 2e66  t: {PRODUCT})".f
-00012c70: 6f72 6d61 7428 0a20 2020 2020 2020 2020  ormat(.         
-00012c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012c90: 4449 5354 5249 4255 5449 4f4e 3d6c 6963  DISTRIBUTION=lic
-00012ca0: 656e 7369 6e67 2e44 4953 5452 4942 5554  ensing.DISTRIBUT
-00012cb0: 494f 4e2c 2050 524f 4455 4354 3d6c 6963  ION, PRODUCT=lic
-00012cc0: 656e 7369 6e67 2e50 524f 4455 4354 5f53  ensing.PRODUCT_S
-00012cd0: 4552 5645 5220 2929 0a20 2020 2061 702e  ERVER )).    ap.
-00012ce0: 6164 645f 6172 6775 6d65 6e74 2820 272d  add_argument( '-
-00012cf0: 5527 2c20 272d 2d75 7365 726e 616d 6527  U', '--username'
-00012d00: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00012d10: 2020 2020 2020 2064 6566 6175 6c74 3d4e         default=N
-00012d20: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
-00012d30: 2020 2020 2020 2020 2020 6865 6c70 3d22            help="
-00012d40: 7b44 4953 5452 4942 5554 494f 4e7d 2041  {DISTRIBUTION} A
-00012d50: 6765 6e74 2063 7265 6465 6e74 6961 6c73  gent credentials
-00012d60: 2075 7365 726e 616d 653b 206c 696b 656c   username; likel
-00012d70: 7920 616e 2065 6d61 696c 2061 6464 7265  y an email addre
-00012d80: 7373 2028 272d 2720 746f 2072 6561 6420  ss ('-' to read 
-00012d90: 6672 6f6d 2069 6e70 7574 2922 2e66 6f72  from input)".for
-00012da0: 6d61 7428 0a20 2020 2020 2020 2020 2020  mat(.           
-00012db0: 2020 2020 2020 2020 2020 2020 2020 4449                DI
-00012dc0: 5354 5249 4255 5449 4f4e 3d6c 6963 656e  STRIBUTION=licen
-00012dd0: 7369 6e67 2e44 4953 5452 4942 5554 494f  sing.DISTRIBUTIO
-00012de0: 4e20 2929 0a20 2020 2061 702e 6164 645f  N )).    ap.add_
-00012df0: 6172 6775 6d65 6e74 2820 272d 5027 2c20  argument( '-P', 
-00012e00: 272d 2d70 6173 7377 6f72 6427 2c0a 2020  '--password',.  
-00012e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012e20: 2020 2064 6566 6175 6c74 3d4e 6f6e 652c     default=None,
-00012e30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012e40: 2020 2020 2020 6865 6c70 3d22 7b44 4953        help="{DIS
-00012e50: 5452 4942 5554 494f 4e7d 2041 6765 6e74  TRIBUTION} Agent
-00012e60: 2063 7265 6465 6e74 6961 6c73 2070 6173   credentials pas
-00012e70: 7377 6f72 6420 2827 2d27 2074 6f20 7265  sword ('-' to re
-00012e80: 6164 2066 726f 6d20 696e 7075 7429 222e  ad from input)".
-00012e90: 666f 726d 6174 280a 2020 2020 2020 2020  format(.        
-00012ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012eb0: 2044 4953 5452 4942 5554 494f 4e3d 6c69   DISTRIBUTION=li
-00012ec0: 6365 6e73 696e 672e 4449 5354 5249 4255  censing.DISTRIBU
-00012ed0: 5449 4f4e 2029 290a 2020 2020 6170 2e61  TION )).    ap.a
-00012ee0: 6464 5f61 7267 756d 656e 7428 2027 2d52  dd_argument( '-R
-00012ef0: 272c 2027 2d2d 7265 6769 7374 6572 272c  ', '--register',
-00012f00: 2061 6374 696f 6e3d 2773 746f 7265 5f74   action='store_t
-00012f10: 7275 6527 2c0a 2020 2020 2020 2020 2020  rue',.          
-00012f20: 2020 2020 2020 2020 2020 2064 6566 6175             defau
-00012f30: 6c74 3d46 616c 7365 2c0a 2020 2020 2020  lt=False,.      
-00012f40: 2020 2020 2020 2020 2020 2020 2020 2068                 h
-00012f50: 656c 703d 2249 6620 6e65 6365 7373 6172  elp="If necessar
-00012f60: 792c 2063 7265 6174 6520 616e 6420 7361  y, create and sa
-00012f70: 7665 2061 206e 6577 2063 6c69 656e 7420  ve a new client 
-00012f80: 4b65 7970 6169 7222 2029 0a20 2020 2061  Keypair" ).    a
-00012f90: 702e 6164 645f 6172 6775 6d65 6e74 2820  p.add_argument( 
-00012fa0: 272d 4127 2c20 272d 2d61 6371 7569 7265  '-A', '--acquire
-00012fb0: 272c 2061 6374 696f 6e3d 2773 746f 7265  ', action='store
-00012fc0: 5f74 7275 6527 2c0a 2020 2020 2020 2020  _true',.        
-00012fd0: 2020 2020 2020 2020 2020 2020 2064 6566               def
-00012fe0: 6175 6c74 3d46 616c 7365 2c0a 2020 2020  ault=False,.    
-00012ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013000: 2068 656c 703d 2249 6620 6e6f 2041 6765   help="If no Age
-00013010: 6e74 204b 6579 7061 6972 206f 7220 4c69  nt Keypair or Li
-00013020: 6365 6e73 6520 6973 2061 7661 696c 6162  cense is availab
-00013030: 6c65 2c20 6174 7465 6d70 7420 746f 2063  le, attempt to c
-00013040: 7265 6174 6520 616e 642f 6f72 206f 6274  reate and/or obt
-00013050: 6169 6e20 6f6e 653b 2070 726f 7669 6465  ain one; provide
-00013060: 202d 2d75 7365 726e 616d 652f 2d2d 7061   --username/--pa
-00013070: 7373 776f 7264 2074 6f20 656e 6372 7970  ssword to encryp
-00013080: 7422 0a20 2020 2020 2020 2020 2020 2020  t".             
-00013090: 2020 2020 2020 2020 222c 2074 6865 6e20          ", then 
-000130a0: 7573 6520 7b45 4e56 5553 4552 4e41 4d45  use {ENVUSERNAME
-000130b0: 7d2f 7b45 4e56 5041 5353 574f 5244 7d20  }/{ENVPASSWORD} 
-000130c0: 656e 7669 726f 6e6d 656e 7420 7661 7273  environment vars
-000130d0: 2074 6f20 6465 6372 7970 7422 2e66 6f72   to decrypt".for
-000130e0: 6d61 7428 0a20 2020 2020 2020 2020 2020  mat(.           
-000130f0: 2020 2020 2020 2020 2020 2020 2020 454e                EN
-00013100: 5655 5345 524e 414d 453d 6c69 6365 6e73  VUSERNAME=licens
-00013110: 696e 672e 454e 5655 5345 524e 414d 452c  ing.ENVUSERNAME,
-00013120: 2045 4e56 5041 5353 574f 5244 3d6c 6963   ENVPASSWORD=lic
-00013130: 656e 7369 6e67 2e45 4e56 5041 5353 574f  ensing.ENVPASSWO
-00013140: 5244 0a20 2020 2020 2020 2020 2020 2020  RD.             
-00013150: 2020 2020 2020 2020 2929 0a20 2020 2061          )).    a
-00013160: 7267 7320 3d20 6170 2e70 6172 7365 5f61  rgs = ap.parse_a
-00013170: 7267 7328 2061 7267 7620 290a 0a20 2020  rgs( argv )..   
-00013180: 2023 2053 6574 2075 7020 6c6f 6767 696e   # Set up loggin
-00013190: 673b 2061 6c73 6f2c 2068 616e 646c 6520  g; also, handle 
-000131a0: 7468 6520 6465 6765 6e65 7261 7465 2063  the degenerate c
-000131b0: 6173 6520 7768 6572 6520 6c6f 6767 696e  ase where loggin
-000131c0: 6720 6861 7320 2a61 6c72 6561 6479 2a20  g has *already* 
-000131d0: 6265 656e 2073 6574 2075 7020 2861 6e64  been set up (and
-000131e0: 0a20 2020 2023 2062 6173 6963 436f 6e66  .    # basicConf
-000131f0: 6967 2069 7320 6120 4e4f 2d4f 5029 2c20  ig is a NO-OP), 
-00013200: 6279 2028 616c 736f 2920 7365 7474 696e  by (also) settin
-00013210: 6720 7468 6520 6c6f 6767 696e 6720 6c65  g the logging le
-00013220: 7665 6c2e 0a20 2020 206c 6f67 5f63 6667  vel..    log_cfg
-00013230: 5b27 6c65 7665 6c27 5d09 093d 206c 6f67  ['level']..= log
-00013240: 5f6c 6576 656c 2820 6172 6773 2e76 6572  _level( args.ver
-00013250: 626f 7365 202d 2061 7267 732e 7175 6965  bose - args.quie
-00013260: 7420 290a 2020 2020 6966 2061 7267 732e  t ).    if args.
-00013270: 6c6f 6720 6f72 2061 7267 732e 6775 693a  log or args.gui:
-00013280: 0a20 2020 2020 2020 206c 6f67 5f63 6667  .        log_cfg
-00013290: 5b27 6669 6c65 6e61 6d65 275d 093d 2061  ['filename'].= a
-000132a0: 7267 732e 6c6f 6720 6f72 204c 4f47 4649  rgs.log or LOGFI
-000132b0: 4c45 0a20 2020 206c 6f67 6769 6e67 2e62  LE.    logging.b
-000132c0: 6173 6963 436f 6e66 6967 2820 2a2a 6c6f  asicConfig( **lo
-000132d0: 675f 6366 6720 290a 2020 2020 6966 2061  g_cfg ).    if a
-000132e0: 7267 732e 7665 7262 6f73 6520 6f72 2061  rgs.verbose or a
-000132f0: 7267 732e 7175 6965 743a 0a20 2020 2020  rgs.quiet:.     
-00013300: 2020 206c 6f67 6769 6e67 2e67 6574 4c6f     logging.getLo
-00013310: 6767 6572 2829 2e73 6574 4c65 7665 6c28  gger().setLevel(
-00013320: 206c 6f67 5f63 6667 5b27 6c65 7665 6c27   log_cfg['level'
-00013330: 5d20 290a 0a20 2020 2070 726f 6669 6c65  ] )..    profile
-00013340: 7209 0909 3d20 4e6f 6e65 0a20 2020 2070  r...= None.    p
-00013350: 726f 6669 6c65 725f 6c69 6d69 7409 093d  rofiler_limit..=
-00013360: 2032 350a 2020 2020 6966 2061 7267 732e   25.    if args.
-00013370: 7072 6f66 696c 653a 0a20 2020 2020 2020  profile:.       
-00013380: 2069 6d70 6f72 7420 7073 7461 7473 0a20   import pstats. 
-00013390: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
-000133a0: 2020 2020 2020 2020 6672 6f6d 206d 7470          from mtp
-000133b0: 726f 6620 696d 706f 7274 2050 726f 6669  rof import Profi
-000133c0: 6c65 0a20 2020 2020 2020 2065 7863 6570  le.        excep
-000133d0: 7420 496d 706f 7274 4572 726f 723a 0a20  t ImportError:. 
-000133e0: 2020 2020 2020 2020 2020 2066 726f 6d20             from 
-000133f0: 6350 726f 6669 6c65 2069 6d70 6f72 7420  cProfile import 
-00013400: 5072 6f66 696c 650a 0a20 2020 2020 2020  Profile..       
-00013410: 2070 726f 6669 6c65 7209 093d 2050 726f   profiler..= Pro
-00013420: 6669 6c65 2829 0a20 2020 2020 2020 2070  file().        p
-00013430: 726f 6669 6c65 722e 656e 6162 6c65 2829  rofiler.enable()
-00013440: 0a0a 2020 2020 2320 416e 7920 636f 6e66  ..    # Any conf
-00013450: 6967 7572 6174 696f 6e20 6669 6c65 7320  iguration files 
-00013460: 616e 6420 6c69 6365 6e73 696e 672e 6c6f  and licensing.lo
-00013470: 6164 2f6c 6f61 645f 6b65 7973 2073 686f  ad/load_keys sho
-00013480: 756c 6420 696e 7370 6563 7420 7468 6573  uld inspect thes
-00013490: 6520 6578 7472 6120 6469 7273 0a20 2020  e extra dirs.   
-000134a0: 2067 6c6f 6261 6c20 636f 6e66 6967 5f65   global config_e
-000134b0: 7874 7261 730a 2020 2020 636f 6e66 6967  xtras.    config
-000134c0: 5f65 7874 7261 7309 2020 2020 2020 202b  _extras.       +
-000134d0: 3d20 6172 6773 2e63 6f6e 6669 6720 6f72  = args.config or
-000134e0: 205b 5d0a 2020 2020 6c6f 672e 696e 666f   [].    log.info
-000134f0: 2820 224c 6963 656e 7369 6e67 2063 6f6e  ( "Licensing con
-00013500: 6669 6775 7261 7469 6f6e 2070 6174 6873  figuration paths
-00013510: 3a20 7b7d 222e 666f 726d 6174 2820 272c  : {}".format( ',
-00013520: 2027 2e6a 6f69 6e28 2063 6f6e 6669 675f   '.join( config_
-00013530: 7061 7468 7328 2027 3c66 696c 653e 272c  paths( '<file>',
-00013540: 2065 7874 7261 3d63 6f6e 6669 675f 6578   extra=config_ex
-00013550: 7472 6173 2029 2929 290a 0a20 2020 2023  tras ))))..    #
-00013560: 2047 6574 2073 6f6d 6520 6465 7461 696c   Get some detail
-00013570: 7320 6162 6f75 7420 7468 6520 4564 3235  s about the Ed25
-00013580: 3531 3920 7665 7273 696f 6e20 7765 2772  519 version we'r
-00013590: 6520 7573 696e 672c 2061 6e64 2073 7570  e using, and sup
-000135a0: 7072 6573 7320 736f 6d65 206e 6167 6769  press some naggi
-000135b0: 6e67 2061 626f 7574 0a20 2020 2023 206c  ng about.    # l
-000135c0: 6574 7469 6e67 2069 7420 6765 6e65 7261  etting it genera
-000135d0: 7465 2072 616e 646f 6d20 7365 6564 732e  te random seeds.
-000135e0: 0a20 2020 2077 6172 6e69 6e67 732e 7369  .    warnings.si
-000135f0: 6d70 6c65 6669 6c74 6572 2827 6967 6e6f  mplefilter('igno
-00013600: 7265 2729 2020 2320 5765 206b 6e6f 7720  re')  # We know 
-00013610: 6162 6f75 7420 6861 6e64 6c69 6e67 2045  about handling E
-00013620: 6432 3535 3139 2072 616e 646f 6d20 7365  d25519 random se
-00013630: 6564 732e 2e2e 0a0a 2020 2020 6c6f 672e  eds.....    log.
-00013640: 696e 666f 2820 2245 6432 3535 3139 2056  info( "Ed25519 V
-00013650: 6572 7369 6f6e 3a20 7b7d 202f 207b 7d20  ersion: {} / {} 
-00013660: 2f20 7b7d 222e 666f 726d 6174 280a 2020  / {}".format(.  
-00013670: 2020 2020 2020 6765 7461 7474 7228 206c        getattr( l
-00013680: 6963 656e 7369 6e67 2e65 6432 3535 3139  icensing.ed25519
-00013690: 2c20 275f 5f76 6572 7369 6f6e 5f5f 272c  , '__version__',
-000136a0: 204e 6f6e 6520 292c 206c 6963 656e 7369   None ), licensi
-000136b0: 6e67 2e65 6432 3535 3139 2e5f 5f70 6163  ng.ed25519.__pac
-000136c0: 6b61 6765 5f5f 2c20 6c69 6365 6e73 696e  kage__, licensin
-000136d0: 672e 6564 3235 3531 392e 5f5f 7061 7468  g.ed25519.__path
-000136e0: 5f5f 2029 290a 0a20 2020 2023 204c 6f61  __ ))..    # Loa
-000136f0: 6420 6f75 7220 4372 7970 746f 204c 6963  d our Crypto Lic
-00013700: 656e 7369 6e67 2073 6572 7665 7220 4167  ensing server Ag
-00013710: 656e 7427 7320 2e63 7279 7074 6f2d 6b65  ent's .crypto-ke
-00013720: 792a 2061 6e64 202e 6372 7970 746f 2d6c  y* and .crypto-l
-00013730: 6963 2a20 6669 6c65 732e 0a20 2020 2023  ic* files..    #
-00013740: 0a20 2020 2023 2054 6869 7320 6973 2074  .    # This is t
-00013750: 6865 2041 6765 6e74 2773 204b 6579 7061  he Agent's Keypa
-00013760: 6972 2074 6861 7420 7769 6c6c 2062 6520  ir that will be 
-00013770: 6173 7369 676e 6564 2061 204c 6963 656e  assigned a Licen
-00013780: 7365 2074 6f20 2a72 756e 2a20 6120 4372  se to *run* a Cr
-00013790: 7970 746f 204c 6963 656e 7369 6e67 0a20  ypto Licensing. 
-000137a0: 2020 2023 2073 6572 7665 722c 206f 6e20     # server, on 
-000137b0: 6120 7061 7274 6963 756c 6172 204d 6163  a particular Mac
-000137c0: 6869 6e65 2049 442e 0a20 2020 2023 0a20  hine ID..    #. 
-000137d0: 2020 2023 2054 6869 7320 6973 202a 6e6f     # This is *no
-000137e0: 742a 2061 6e20 6175 7468 6f72 6974 7920  t* an authority 
-000137f0: 746f 2073 6967 6e20 616e 6420 2a69 7373  to sign and *iss
-00013800: 7565 2a20 4372 7970 746f 204c 6963 656e  ue* Crypto Licen
-00013810: 7369 6e67 2073 6572 7665 7220 6c69 6365  sing server lice
-00013820: 6e73 6573 2e20 2054 6861 7420 4b65 7970  nses.  That Keyp
-00013830: 6169 720a 2020 2020 2320 6973 2064 6966  air.    # is dif
-00013840: 6665 7265 6e74 2c20 616e 6420 6973 206c  ferent, and is l
-00013850: 6f61 6465 6420 2a69 6e74 6f2a 2074 6865  oaded *into* the
-00013860: 2043 7279 7074 6f20 4c69 6365 6e73 696e   Crypto Licensin
-00013870: 6720 7365 7276 6572 2c20 616e 6420 6973  g server, and is
-00013880: 2075 7365 6420 746f 2073 6967 6e20 6e65   used to sign ne
-00013890: 770a 2020 2020 2320 4c69 6365 6e73 6573  w.    # Licenses
-000138a0: 2074 6861 7420 6172 6520 6973 7375 6564   that are issued
-000138b0: 2074 6f20 6f74 6865 7220 7061 7274 6965   to other partie
-000138c0: 732e 0a20 2020 2023 0a20 2020 2023 2049  s..    #.    # I
-000138d0: 6620 6e65 6365 7373 6172 792c 2077 6527  f necessary, we'
-000138e0: 6c6c 2061 736b 2066 6f72 2061 204c 6963  ll ask for a Lic
-000138f0: 656e 7365 2074 6f20 6265 2069 7373 7565  ense to be issue
-00013900: 6420 6279 2044 6f6d 696e 696f 6e20 5226  d by Dominion R&
-00013910: 4420 436f 7270 2c20 746f 2074 6869 7320  D Corp, to this 
-00013920: 4167 656e 742c 2066 6f72 0a20 2020 2023  Agent, for.    #
-00013930: 2061 7574 686f 7269 7a61 7469 6f6e 2074   authorization t
-00013940: 6f20 7275 6e20 6f6e 2074 6869 7320 6d61  o run on this ma
-00013950: 6368 696e 652e 2020 5468 6973 204c 6963  chine.  This Lic
-00013960: 656e 7365 2077 696c 6c20 6772 616e 7420  ense will grant 
-00013970: 7573 2074 6865 2063 6170 6162 696c 6974  us the capabilit
-00013980: 7920 746f 2069 7373 7565 0a20 2020 2023  y to issue.    #
-00013990: 2073 7562 2d4c 6963 656e 7365 7320 666f   sub-Licenses fo
-000139a0: 7220 6120 6365 7274 6169 6e20 6e75 6d62  r a certain numb
-000139b0: 6572 206f 6620 226d 6173 7465 7222 204c  er of "master" L
-000139c0: 6963 656e 7365 7320 284c 6963 656e 7365  icenses (License
-000139d0: 7320 7468 6174 2064 6f20 6e6f 7420 6861  s that do not ha
-000139e0: 7665 2061 0a20 2020 2023 2070 7265 2d64  ve a.    # pre-d
-000139f0: 6566 696e 6564 2063 6c69 656e 7420 6261  efined client ba
-00013a00: 6b65 6420 696e 746f 2074 6865 6d2c 2061  ked into them, a
-00013a10: 6e64 2074 6875 7320 636f 756c 6420 6265  nd thus could be
-00013a20: 2073 7562 2d6c 6963 656e 7365 6420 746f   sub-licensed to
-00013a30: 2061 6e79 2063 6c69 656e 7429 2e20 2054   any client).  T
-00013a40: 6865 2043 7279 7074 6f0a 2020 2020 2320  he Crypto.    # 
-00013a50: 4c69 6365 6e73 696e 6720 7365 7276 6572  Licensing server
-00013a60: 2069 7320 6578 7065 6374 6564 2074 6f20   is expected to 
-00013a70: 6973 7375 6520 4c69 6365 6e73 6573 2074  issue Licenses t
-00013a80: 6861 7420 636f 6d70 6c79 2077 6974 6820  hat comply with 
-00013a90: 7468 6520 7275 6c65 7320 6573 7461 626c  the rules establ
-00013aa0: 6973 6865 6420 6279 2074 6865 0a20 2020  ished by the.   
-00013ab0: 2023 2022 6d61 7374 6572 2220 4c69 6365   # "master" Lice
-00013ac0: 6e73 653b 2069 6620 6974 2069 7320 666f  nse; if it is fo
-00013ad0: 756e 6420 7468 6174 206f 6e65 2069 7320  und that one is 
-00013ae0: 6973 7375 696e 6720 696e 7661 6c69 6420  issuing invalid 
-00013af0: 4c69 6365 6e73 6573 2028 6965 2e20 7468  Licenses (ie. th
-00013b00: 6520 226d 6173 7465 7222 2067 7261 6e74  e "master" grant
-00013b10: 730a 2020 2020 2320 3130 206d 6163 6869  s.    # 10 machi
-00013b20: 6e65 732c 2062 7574 206d 6f72 6520 7468  nes, but more th
-00013b30: 616e 2031 3020 7375 622d 4c69 6365 6e73  an 10 sub-Licens
-00013b40: 6573 2068 6176 6520 6265 656e 2069 7373  es have been iss
-00013b50: 7565 6429 2c20 7468 656e 2069 7473 206c  ued), then its l
-00013b60: 6963 656e 7365 2077 696c 6c20 6265 2072  icense will be r
-00013b70: 6576 6f6b 6564 0a20 2020 2023 2062 7920  evoked.    # by 
-00013b80: 626c 6163 6b6c 6973 7469 6e67 2069 7473  blacklisting its
-00013b90: 2070 7562 6c69 6320 6b65 792e 0a20 2020   public key..   
-00013ba0: 2023 0a20 2020 2023 2054 6865 2073 6563   #.    # The sec
-00013bb0: 7265 7473 2072 6571 7569 7265 6420 746f  rets required to
-00013bc0: 2064 6563 7279 7074 2074 6865 206c 6963   decrypt the lic
-00013bd0: 656e 7369 6e67 2e4b 6579 7061 6972 456e  ensing.KeypairEn
-00013be0: 6372 7970 7465 6420 6172 6520 6578 7065  crypted are expe
-00013bf0: 6374 6564 2074 6f20 6265 2069 6e0a 2020  cted to be in.  
-00013c00: 2020 2320 656e 7669 726f 6e6d 656e 7420    # environment 
-00013c10: 7661 7269 6162 6c65 7320 2873 7065 6369  variables (speci
-00013c20: 6679 2027 2d27 2074 6f20 7265 6164 2066  fy '-' to read f
-00013c30: 726f 6d20 696e 7075 7429 3a0a 2020 2020  rom input):.    
-00013c40: 230a 2020 2020 2320 2020 2020 4352 5950  #.    #     CRYP
-00013c50: 544f 5f4c 4943 5f55 5345 524e 414d 4520  TO_LIC_USERNAME 
-00013c60: 2023 206f 7220 2d2d 7573 6572 6e61 6d65   # or --username
-00013c70: 0a20 2020 2023 2020 2020 2043 5259 5054  .    #     CRYPT
-00013c80: 4f5f 4c49 435f 5041 5353 574f 5244 2020  O_LIC_PASSWORD  
-00013c90: 2320 6f72 202d 2d70 6173 7377 6f72 6420  # or --password 
-00013ca0: 2875 6e73 6166 6529 0a20 2020 2023 0a20  (unsafe).    #. 
-00013cb0: 2020 2023 2054 6865 6e2c 2066 696e 6420     # Then, find 
-00013cc0: 616e 6420 6c6f 6164 2074 6865 204b 6579  and load the Key
-00013cd0: 7061 6172 2061 6e64 204c 6963 656e 7365  paar and License
-00013ce0: 202d 2d70 726f 6475 6374 2028 7370 6c69   --product (spli
-00013cf0: 7420 6f6e 2073 7061 6365 7329 2c20 6a6f  t on spaces), jo
-00013d00: 696e 6564 2062 7920 272d 2729 3a0a 2020  ined by '-'):.  
-00013d10: 2020 230a 2020 2020 2320 2020 2020 6372    #.    #     cr
-00013d20: 7970 746f 2d6c 6963 656e 7369 6e67 2d73  ypto-licensing-s
-00013d30: 6572 7665 722e 6372 7970 746f 2d7b 6b65  erver.crypto-{ke
-00013d40: 7970 6169 722c 6c69 6365 6e73 657d 0a20  ypair,license}. 
-00013d50: 2020 2023 0a20 2020 2062 6173 656e 616d     #.    basenam
-00013d60: 6509 0909 3d20 272d 272e 6a6f 696e 2820  e...= '-'.join( 
-00013d70: 5b20 7365 676d 656e 742e 6c6f 7765 7228  [ segment.lower(
-00013d80: 2920 666f 7220 7365 676d 656e 7420 696e  ) for segment in
-00013d90: 2061 7267 732e 7072 6f64 7563 742e 7370   args.product.sp
-00013da0: 6c69 7428 2920 5d20 290a 2020 2020 6c6f  lit() ] ).    lo
-00013db0: 672e 6c6f 6728 206c 6f67 6769 6e67 2e44  g.log( logging.D
-00013dc0: 4554 4149 4c2c 2022 4c6f 6164 696e 6720  ETAIL, "Loading 
-00013dd0: 4167 656e 7420 4564 3235 3531 3920 4b65  Agent Ed25519 Ke
-00013de0: 7970 6169 7220 6672 6f6d 207b 7d2e 2e2e  ypair from {}...
-00013df0: 222e 666f 726d 6174 2820 6261 7365 6e61  ".format( basena
-00013e00: 6d65 2029 290a 2020 2020 2320 4c6f 6164  me )).    # Load
-00013e10: 2041 6765 6e74 204b 6579 7061 6972 2c20   Agent Keypair, 
-00013e20: 6966 2061 6e79 2c20 7573 696e 6720 616e  if any, using an
-00013e30: 7920 6372 6564 656e 7469 616c 7320 7375  y credentials su
-00013e40: 7070 6c69 6564 2069 6e20 7468 6520 656e  pplied in the en
-00013e50: 7669 726f 6e6d 656e 740a 2020 2020 636c  vironment.    cl
-00013e60: 5f75 7365 726e 616d 6509 0909 3d20 6172  _username...= ar
-00013e70: 6773 2e75 7365 726e 616d 6520 6f72 206f  gs.username or o
-00013e80: 732e 6765 7465 6e76 2820 6c69 6365 6e73  s.getenv( licens
-00013e90: 696e 672e 454e 5655 5345 524e 414d 4520  ing.ENVUSERNAME 
-00013ea0: 290a 2020 2020 636c 5f70 6173 7377 6f72  ).    cl_passwor
-00013eb0: 6409 0909 3d20 6172 6773 2e70 6173 7377  d...= args.passw
-00013ec0: 6f72 6420 6f72 206f 732e 6765 7465 6e76  ord or os.getenv
-00013ed0: 2820 6c69 6365 6e73 696e 672e 454e 5650  ( licensing.ENVP
-00013ee0: 4153 5357 4f52 4420 290a 2020 2020 6966  ASSWORD ).    if
-00013ef0: 2061 7267 732e 7061 7373 776f 7264 2061   args.password a
-00013f00: 6e64 2061 7267 732e 7061 7373 776f 7264  nd args.password
-00013f10: 2021 3d20 272d 273a 0a20 2020 2020 2020   != '-':.       
-00013f20: 206c 6f67 2e77 6172 6e69 6e67 2820 2249   log.warning( "I
-00013f30: 7420 6973 2072 6563 6f6d 6d65 6e64 6564  t is recommended
-00013f40: 2074 6f20 6e6f 7420 7573 6520 272d 507c   to not use '-P|
-00013f50: 2d2d 7061 7373 776f 7264 202e 2e2e 273b  --password ...';
-00013f60: 2073 7065 6369 6679 2027 2d27 2074 6f20   specify '-' to 
-00013f70: 7265 6164 2066 726f 6d20 696e 7075 7422  read from input"
-00013f80: 2029 0a0a 2020 2020 2320 4379 636c 6520   )..    # Cycle 
-00013f90: 7468 726f 7567 6820 7468 6520 6176 6169  through the avai
-00013fa0: 6c61 626c 6520 4167 656e 7420 4944 206b  lable Agent ID k
-00013fb0: 6579 732c 2061 6e64 2061 6e79 204c 6963  eys, and any Lic
-00013fc0: 656e 7365 2873 2920 666f 7220 446f 6d69  ense(s) for Domi
-00013fd0: 6e69 6f6e 2052 2644 2773 2043 7279 7074  nion R&D's Crypt
-00013fe0: 6f0a 2020 2020 2320 4c69 6365 6e73 696e  o.    # Licensin
-00013ff0: 672e 2020 546f 2063 7265 6174 6520 616e  g.  To create an
-00014000: 2075 6e65 6e63 7279 7074 6564 204b 6579   unencrypted Key
-00014010: 7061 6972 2c20 6e6f 202d 2d75 7365 726e  pair, no --usern
-00014020: 616d 652f 2d2d 7061 7373 776f 7264 206d  ame/--password m
-00014030: 6179 2062 6520 7370 6563 6966 6965 642e  ay be specified.
-00014040: 0a20 2020 2023 204f 7468 6572 7769 7365  .    # Otherwise
-00014050: 2c20 7765 206d 7573 7420 626c 6f63 6b20  , we must block 
-00014060: 6865 7265 2061 7761 6974 696e 6720 696e  here awaiting in
-00014070: 7075 742e 0a20 2020 2075 7365 726e 616d  put..    usernam
-00014080: 6509 0909 3d20 696e 7075 745f 7365 6375  e...= input_secu
-00014090: 7265 2820 2245 6e74 6572 207b 7d20 7573  re( "Enter {} us
-000140a0: 6572 6e61 6d65 3a20 222e 666f 726d 6174  ername: ".format
-000140b0: 2820 6261 7365 6e61 6d65 2029 2920 6966  ( basename )) if
-000140c0: 2063 6c5f 7573 6572 6e61 6d65 203d 3d20   cl_username == 
-000140d0: 272d 2720 656c 7365 2063 6c5f 7573 6572  '-' else cl_user
-000140e0: 6e61 6d65 0a20 2020 2070 6173 7377 6f72  name.    passwor
-000140f0: 6409 0909 3d20 696e 7075 745f 7365 6375  d...= input_secu
-00014100: 7265 2820 2245 6e74 6572 207b 7d20 7061  re( "Enter {} pa
-00014110: 7373 776f 7264 3a20 222e 666f 726d 6174  ssword: ".format
-00014120: 2820 6261 7365 6e61 6d65 2029 2920 6966  ( basename )) if
-00014130: 2063 6c5f 7061 7373 776f 7264 203d 3d20   cl_password == 
-00014140: 272d 2720 656c 7365 2063 6c5f 7061 7373  '-' else cl_pass
-00014150: 776f 7264 0a20 2020 2075 7365 7270 6173  word.    userpas
-00014160: 735f 696e 7075 7409 093d 2063 6c5f 7573  s_input..= cl_us
-00014170: 6572 6e61 6d65 203d 3d20 272d 2720 6f72  ername == '-' or
-00014180: 2063 6c5f 7061 7373 776f 7264 203d 3d20   cl_password == 
-00014190: 272d 270a 2020 2020 7472 793a 0a20 2020  '-'.    try:.   
-000141a0: 2020 2020 2023 2057 6527 7265 206c 6f6f       # We're loo
-000141b0: 6b69 6e67 2066 6f72 2061 204c 6963 656e  king for a Licen
-000141c0: 7365 2061 7574 686f 7265 6420 6279 2044  se authored by D
-000141d0: 6f6d 696e 696f 6e20 5226 4420 436f 7270  ominion R&D Corp
-000141e0: 2e20 2054 6869 7320 6d69 6768 7420 6265  .  This might be
-000141f0: 2065 6e63 6170 7375 6c61 7465 6420 6173   encapsulated as
-00014200: 0a20 2020 2020 2020 2023 206f 6e65 206f  .        # one o
-00014210: 6620 7468 6520 6465 7065 6e64 656e 6369  f the dependenci
-00014220: 6573 206f 6620 7468 6520 4c69 6365 6e73  es of the Licens
-00014230: 6520 7765 2066 696e 6420 2865 672e 2069  e we find (eg. i
-00014240: 6620 446f 6d69 6e69 6f6e 2069 7373 7565  f Dominion issue
-00014250: 7320 6120 4c69 6365 6e73 6520 746f 2073  s a License to s
-00014260: 6f6d 650a 2020 2020 2020 2020 2320 636f  ome.        # co
-00014270: 6d70 616e 792c 2077 6869 6368 2069 6e63  mpany, which inc
-00014280: 6c75 6465 7320 7468 6520 6162 696c 6974  ludes the abilit
-00014290: 7920 746f 2072 756e 2061 2063 7279 7074  y to run a crypt
-000142a0: 6f2d 6c69 6365 6e73 696e 6720 7365 7276  o-licensing serv
-000142b0: 6572 292c 2062 7574 2077 6527 6c6c 2076  er), but we'll v
-000142c0: 616c 6964 6174 650a 2020 2020 2020 2020  alidate.        
-000142d0: 2320 7468 6174 2074 6865 2047 7261 6e74  # that the Grant
-000142e0: 2077 6173 2069 7373 7565 6420 6279 2044   was issued by D
-000142f0: 6f6d 696e 696f 6e20 5226 4420 436f 7270  ominion R&D Corp
-00014300: 2e20 2046 6f72 2065 7861 6d70 6c65 2c20  .  For example, 
-00014310: 446f 6d69 6e69 6f6e 2069 7373 7565 7320  Dominion issues 
-00014320: 6120 4c69 6365 6e73 6520 746f 0a20 2020  a License to.   
-00014330: 2020 2020 2023 2061 7765 736f 6d65 2d69       # awesome-i
-00014340: 6e63 2e63 6f6d 2074 6f20 7375 622d 4c69  nc.com to sub-Li
-00014350: 6365 6e73 6520 6372 7970 746f 2d6c 6963  cense crypto-lic
-00014360: 656e 7369 6e67 2073 6572 7665 7273 2e20  ensing servers. 
-00014370: 2054 6865 792c 2069 6e20 7475 726e 2c20   They, in turn, 
-00014380: 6973 7375 6520 6120 4c69 6365 6e73 650a  issue a License.
-00014390: 2020 2020 2020 2020 2320 746f 20d0 9bd0          # to ...
-000143a0: b0d0 b9d0 bad0 b02e 7275 2074 6f20 7275  ........ru to ru
-000143b0: 6e20 6120 6372 7970 746f 2d6c 6963 656e  n a crypto-licen
-000143c0: 7369 6e67 2073 6572 7665 722c 2061 6e64  sing server, and
-000143d0: 2068 656c 7020 7468 656d 2073 6574 2069   help them set i
-000143e0: 7420 7570 2e20 2057 6865 6e0a 2020 2020  t up.  When.    
-000143f0: 2020 2020 2320 6874 7470 3a2f 2f63 7279      # http://cry
-00014400: 7074 6f2d 6c69 6365 6e73 696e 672e 786e  pto-licensing.xn
-00014410: 2d2d 3830 6161 3061 6563 2e72 752f 2028  --80aa0aec.ru/ (
-00014420: 6372 7970 746f 2d6c 6963 656e 7369 6e67  crypto-licensing
-00014430: 2ed0 9bd0 b0d0 b9d0 bad0 b02e 7275 2920  ............ru) 
-00014440: 6973 7375 6573 2061 204c 6963 656e 7365  issues a License
-00014450: 2066 6f72 0a20 2020 2020 2020 2023 2074   for.        # t
-00014460: 6865 6972 2073 6f66 7477 6172 652c 2070  heir software, p
-00014470: 6172 7420 6f66 2074 6865 2066 6565 7320  art of the fees 
-00014480: 6172 6520 7061 6964 2074 6f20 6177 6573  are paid to awes
-00014490: 6f6d 652d 696e 632e 636f 6d20 616e 6420  ome-inc.com and 
-000144a0: 736f 6d65 2074 6f20 646f 6d69 6e69 6f6e  some to dominion
-000144b0: 726e 642e 636f 6d2e 0a20 2020 2020 2020  rnd.com..       
-000144c0: 2023 2054 6865 2066 696e 616c 2073 6f66   # The final sof
-000144d0: 7477 6172 6520 696e 7374 616c 6c61 7469  tware installati
-000144e0: 6f6e 2075 7365 7320 6372 7970 746f 2d6c  on uses crypto-l
-000144f0: 6963 656e 7369 6e67 2773 2061 7574 686f  icensing's autho
-00014500: 7269 7a65 6428 2920 6675 6e63 7469 6f6e  rized() function
-00014510: 2c20 7768 6963 6820 6368 6563 6b73 0a20  , which checks. 
-00014520: 2020 2020 2020 2023 2074 6861 7420 6561         # that ea
-00014530: 6368 2073 7563 6365 7373 6976 6520 4c69  ch successive Li
-00014540: 6365 6e73 6527 7320 6465 7065 6e64 656e  cense's dependen
-00014550: 6369 6573 2061 7265 2063 6f72 7265 6374  cies are correct
-00014560: 6c79 2073 6967 6e65 642c 2061 6e64 2063  ly signed, and c
-00014570: 6172 7269 6573 2074 6865 206f 7269 6769  arries the origi
-00014580: 6e61 6c0a 2020 2020 2020 2020 2320 2763  nal.        # 'c
-00014590: 7279 7074 6f2d 6c69 6365 6e73 696e 6727  rypto-licensing'
-000145a0: 2047 7261 6e74 2074 6872 6f75 6768 2074   Grant through t
-000145b0: 6f20 7468 6520 7265 6369 7069 656e 742e  o the recipient.
-000145c0: 0a20 2020 2020 2020 2064 6f6d 696e 696f  .        dominio
-000145d0: 6e09 093d 206c 6963 656e 7369 6e67 2e41  n..= licensing.A
-000145e0: 6765 6e74 280a 2020 2020 2020 2020 2020  gent(.          
-000145f0: 2020 6e61 6d65 093d 206c 6963 656e 7369    name.= licensi
-00014600: 6e67 2e43 4f4d 5041 4e59 2c0a 2020 2020  ng.COMPANY,.    
-00014610: 2020 2020 2020 2020 646f 6d61 696e 093d          domain.=
-00014620: 206c 6963 656e 7369 6e67 2e44 4f4d 4149   licensing.DOMAI
-00014630: 4e2c 0a20 2020 2020 2020 2020 2020 2070  N,.            p
-00014640: 726f 6475 6374 093d 206c 6963 656e 7369  roduct.= licensi
-00014650: 6e67 2e50 524f 4455 4354 2c0a 2020 2020  ng.PRODUCT,.    
-00014660: 2020 2020 2020 2020 7075 626b 6579 093d          pubkey.=
-00014670: 206c 6963 656e 7369 6e67 2e50 5542 4b45   licensing.PUBKE
-00014680: 592c 0a20 2020 2020 2020 2029 0a20 2020  Y,.        ).   
-00014690: 2020 2020 2073 6572 7665 7209 0909 3d20       server...= 
-000146a0: 4e6f 6e65 0a20 2020 2020 2020 2069 6620  None.        if 
-000146b0: 6172 6773 2e70 726f 6475 6374 2061 6e64  args.product and
-000146c0: 2061 7267 732e 646f 6d61 696e 3a0a 2020   args.domain:.  
-000146d0: 2020 2020 2020 2020 2020 7365 7276 6572            server
-000146e0: 0909 3d20 6c69 6365 6e73 696e 672e 4167  ..= licensing.Ag
-000146f0: 656e 7428 0a20 2020 2020 2020 2020 2020  ent(.           
-00014700: 2020 2020 206e 616d 6509 3d20 6172 6773       name.= args
-00014710: 2e63 6c69 656e 742c 0a20 2020 2020 2020  .client,.       
-00014720: 2020 2020 2020 2020 2064 6f6d 6169 6e09           domain.
-00014730: 3d20 6172 6773 2e64 6f6d 6169 6e2c 0a20  = args.domain,. 
-00014740: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00014750: 726f 6475 6374 093d 2061 7267 732e 7072  roduct.= args.pr
-00014760: 6f64 7563 742c 0a20 2020 2020 2020 2020  oduct,.         
-00014770: 2020 2029 0a0a 2020 2020 2020 2020 6175     )..        au
-00014780: 7468 6f72 697a 6174 696f 6e09 093d 206c  thorization..= l
-00014790: 6963 656e 7369 6e67 2e61 7574 686f 7269  icensing.authori
-000147a0: 7a65 6428 0a20 2020 2020 2020 2020 2020  zed(.           
-000147b0: 2061 7574 686f 7209 3d20 646f 6d69 6e69   author.= domini
-000147c0: 6f6e 2c0a 2020 2020 2020 2020 2020 2020  on,.            
-000147d0: 636c 6965 6e74 093d 2073 6572 7665 722c  client.= server,
-000147e0: 0a20 2020 2020 2020 2020 2020 2062 6173  .            bas
-000147f0: 656e 616d 6509 3d20 6261 7365 6e61 6d65  ename.= basename
-00014800: 2c0a 2020 2020 2020 2020 2020 2020 7573  ,.            us
-00014810: 6572 6e61 6d65 093d 2075 7365 726e 616d  ername.= usernam
-00014820: 652c 0a20 2020 2020 2020 2020 2020 2070  e,.            p
-00014830: 6173 7377 6f72 6409 3d20 7061 7373 776f  assword.= passwo
-00014840: 7264 2c0a 2020 2020 2020 2020 2020 2020  rd,.            
-00014850: 7265 6769 7374 6572 696e 6709 3d20 6172  registering.= ar
-00014860: 6773 2e72 6567 6973 7465 722c 2020 2020  gs.register,    
-00014870: 2020 2020 2320 4973 7375 6520 616e 2041      # Issue an A
-00014880: 6765 6e74 2049 4420 6966 206e 6f6e 6520  gent ID if none 
-00014890: 666f 756e 643f 0a20 2020 2020 2020 2020  found?.         
-000148a0: 2020 2061 6371 7569 7269 6e67 093d 2061     acquiring.= a
-000148b0: 7267 732e 6163 7175 6972 652c 0909 2320  rgs.acquire,..# 
-000148c0: 4163 7175 6972 6520 6120 4c69 6365 6e73  Acquire a Licens
-000148d0: 6520 6966 206e 6f6e 6520 666f 756e 643f  e if none found?
-000148e0: 0a20 2020 2020 2020 2020 2020 2065 7874  .            ext
-000148f0: 7261 093d 2063 6f6e 6669 675f 6578 7472  ra.= config_extr
-00014900: 6173 2c20 2020 2020 2020 2023 2069 6e63  as,        # inc
-00014910: 6c75 6469 6e67 2061 6e79 206c 6f63 616c  luding any local
-00014920: 6c79 2064 6566 696e 6564 2063 6f6e 6669  ly defined confi
-00014930: 6720 6469 7273 0a20 2020 2020 2020 2029  g dirs.        )
-00014940: 0a0a 2020 2020 2020 2020 6c6f 6164 6564  ..        loaded
-00014950: 0909 093d 205b 5d0a 2020 2020 2020 2020  ...= [].        
-00014960: 666f 7220 6b65 792c 6c69 6320 696e 2061  for key,lic in a
-00014970: 7574 686f 7269 7a61 7469 6f6e 3a0a 2020  uthorization:.  
-00014980: 2020 2020 2020 2020 2020 6966 206b 6579            if key
-00014990: 2069 7320 4e6f 6e65 206f 7220 6c69 6320   is None or lic 
-000149a0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-000149b0: 2020 2020 2020 2020 2077 6861 7409 093d           what..=
-000149c0: 2022 4e6f 204c 6963 656e 7365 2066 6f75   "No License fou
-000149d0: 6e64 2066 6f72 2041 6765 6e74 2049 4420  nd for Agent ID 
-000149e0: 7b7d 222e 666f 726d 6174 280a 2020 2020  {}".format(.    
-000149f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014a00: 6c69 6365 6e73 696e 672e 696e 746f 5f62  licensing.into_b
-00014a10: 3634 2820 6b65 792e 766b 2029 2920 6966  64( key.vk )) if
-00014a20: 206b 6579 2065 6c73 6520 224e 6f20 4167   key else "No Ag
-00014a30: 656e 7420 4944 204b 6579 7061 6972 2066  ent ID Keypair f
-00014a40: 6f75 6e64 220a 2020 2020 2020 2020 2020  ound".          
-00014a50: 2020 2020 2020 6966 2075 7365 7270 6173        if userpas
-00014a60: 735f 696e 7075 743a 0a20 2020 2020 2020  s_input:.       
-00014a70: 2020 2020 2020 2020 2020 2020 2077 6861               wha
-00014a80: 7420 2020 2020 2020 2b3d 2022 3b20 656e  t       += "; en
-00014a90: 7465 7220 6372 6564 656e 7469 616c 7322  ter credentials"
-00014aa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014ab0: 2020 2020 2069 6620 7061 7373 776f 7264       if password
-00014ac0: 2021 3d20 222d 223a 0a20 2020 2020 2020   != "-":.       
-00014ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014ae0: 2077 6861 7420 2020 2b3d 2022 2028 6c65   what   += " (le
-00014af0: 6176 6520 626c 616e 6b20 746f 2072 6567  ave blank to reg
-00014b00: 6973 7465 7220 772f 207b 7d3a 207b 7d22  ister w/ {}: {}"
-00014b10: 2e66 6f72 6d61 7428 0a20 2020 2020 2020  .format(.       
-00014b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014b30: 2020 2020 2075 7365 726e 616d 6520 6f72       username or
-00014b40: 2022 286e 6f20 7573 6572 6e61 6d65 2922   "(no username)"
-00014b50: 2c20 272a 2720 2a20 6c65 6e28 2070 6173  , '*' * len( pas
-00014b60: 7377 6f72 6420 6f72 2027 2720 2920 6f72  sword or '' ) or
-00014b70: 2022 286e 6f20 7061 7373 776f 7264 2922   "(no password)"
-00014b80: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-00014b90: 2020 206c 6f67 2e77 6172 6e69 6e67 2820     log.warning( 
-00014ba0: 7768 6174 2029 0a20 2020 2020 2020 2020  what ).         
-00014bb0: 2020 2020 2020 2069 6620 6e6f 7420 7573         if not us
-00014bc0: 6572 7061 7373 5f69 6e70 7574 3a0a 2020  erpass_input:.  
-00014bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014be0: 2020 636f 6e74 696e 7565 0a20 2020 2020    continue.     
-00014bf0: 2020 2020 2020 2020 2020 2023 204e 6f20             # No 
-00014c00: 4167 656e 7420 4944 2f4c 6963 656e 7365  Agent ID/License
-00014c10: 206c 6f61 6465 643b 2075 7365 726e 616d   loaded; usernam
-00014c20: 652f 7061 7373 776f 7264 206d 6179 2062  e/password may b
-00014c30: 6520 696e 636f 7272 6563 742e 2020 4966  e incorrect.  If
-00014c40: 206e 6f6e 6520 7072 6f76 6964 6564 2c0a   none provided,.
+0000ef40: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
+0000ef50: 2020 2020 2020 2020 2020 2020 2020 2274                "t
+0000ef60: 6974 6c65 223a 0922 4c6f 6769 6e20 4661  itle":."Login Fa
+0000ef70: 696c 6564 3a20 2573 2220 2520 6572 726f  iled: %s" % erro
+0000ef80: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
+0000ef90: 2020 2020 2020 2020 2020 2022 7265 6469             "redi
+0000efa0: 7265 6374 223a 0977 6562 2e69 6e70 7574  rect":.web.input
+0000efb0: 2829 2e67 6574 2820 2272 6564 6972 6563  ().get( "redirec
+0000efc0: 7422 2c20 2222 2029 2c0a 2020 2020 2020  t", "" ),.      
+0000efd0: 2020 2020 2020 2020 2020 2020 2020 7d29                })
+0000efe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000eff0: 2077 6562 2e68 6561 6465 7228 2022 4361   web.header( "Ca
+0000f000: 6368 652d 436f 6e74 726f 6c22 2c20 226e  che-Control", "n
+0000f010: 6f2d 6361 6368 6522 2029 0a20 2020 2020  o-cache" ).     
+0000f020: 2020 2020 2020 2020 2020 2077 6562 2e68             web.h
+0000f030: 6561 6465 7228 2022 436f 6e74 656e 742d  eader( "Content-
+0000f040: 5479 7065 222c 2022 7465 7874 2f68 746d  Type", "text/htm
+0000f050: 6c22 2029 0a20 2020 2020 2020 2020 2020  l" ).           
+0000f060: 2020 2020 2072 6574 7572 6e20 7265 7370       return resp
+0000f070: 6f6e 7365 0a0a 2020 2020 636c 6173 7320  onse..    class 
+0000f080: 6170 695f 6973 7375 653a 0a20 2020 2020  api_issue:.     
+0000f090: 2020 2064 6566 2047 4554 2820 7365 6c66     def GET( self
+0000f0a0: 2c20 7061 7468 2c20 696e 7075 745f 7661  , path, input_va
+0000f0b0: 7269 6162 6c65 3d22 7175 6572 6965 7322  riable="queries"
+0000f0c0: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
+0000f0d0: 7265 6e64 6572 0909 3d20 7765 622e 7465  render..= web.te
+0000f0e0: 6d70 6c61 7465 2e72 656e 6465 7228 0a20  mplate.render(. 
+0000f0f0: 2020 2020 2020 2020 2020 2020 2020 2054                 T
+0000f100: 504c 5041 5448 2c20 6261 7365 3d22 6c61  PLPATH, base="la
+0000f110: 796f 7574 222c 2067 6c6f 6261 6c73 3d7b  yout", globals={
+0000f120: 2769 6e6c 696e 6527 3a20 696e 6c69 6e65  'inline': inline
+0000f130: 2c20 2773 6573 7369 6f6e 273a 2073 6573  , 'session': ses
+0000f140: 7369 6f6e 7d20 290a 2020 2020 2020 2020  sion} ).        
+0000f150: 2020 2020 6163 6365 7074 0909 3d20 4e6f      accept..= No
+0000f160: 6e65 0a20 2020 2020 2020 2020 2020 2069  ne.            i
+0000f170: 6620 7061 7468 2061 6e64 2070 6174 682e  f path and path.
+0000f180: 656e 6473 7769 7468 2820 222e 6a73 6f6e  endswith( ".json
+0000f190: 2220 293a 0a20 2020 2020 2020 2020 2020  " ):.           
+0000f1a0: 2020 2020 2070 6174 6809 093d 2070 6174       path..= pat
+0000f1b0: 685b 3a2d 355d 0909 2320 636c 6970 206f  h[:-5]..# clip o
+0000f1c0: 6666 2022 2e6a 736f 6e22 0a20 2020 2020  ff ".json".     
+0000f1d0: 2020 2020 2020 2020 2020 2061 6363 6570             accep
+0000f1e0: 7409 093d 2022 6170 706c 6963 6174 696f  t..= "applicatio
+0000f1f0: 6e2f 6a73 6f6e 220a 0a20 2020 2020 2020  n/json"..       
+0000f200: 2020 2020 2023 2041 6c77 6179 7320 7265       # Always re
+0000f210: 7475 726e 7320 6120 636f 6e74 656e 742d  turns a content-
+0000f220: 7479 7065 2061 6e64 2072 6573 706f 6e73  type and respons
+0000f230: 652e 2020 4966 2061 6e20 6578 6365 7074  e.  If an except
+0000f240: 696f 6e20 6973 0a20 2020 2020 2020 2020  ion is.         
+0000f250: 2020 2023 2072 6169 7365 642c 2069 7420     # raised, it 
+0000f260: 7368 6f75 6c64 2062 6520 616e 2061 7070  should be an app
+0000f270: 726f 7072 6961 7465 206f 6e65 2066 726f  ropriate one fro
+0000f280: 6d20 7468 6520 7375 7070 6c69 6564 2066  m the supplied f
+0000f290: 7261 6d65 776f 726b 2074 6f0a 2020 2020  ramework to.    
+0000f2a0: 2020 2020 2020 2020 2320 6361 7272 7920          # carry 
+0000f2b0: 6120 6d65 616e 696e 6766 756c 2048 5454  a meaningful HTT
+0000f2c0: 5020 7374 6174 7573 2063 6f64 652e 2020  P status code.  
+0000f2d0: 4f74 6865 7277 6973 652c 2061 2067 656e  Otherwise, a gen
+0000f2e0: 6572 6963 2035 3030 2053 6572 7665 720a  eric 500 Server.
+0000f2f0: 2020 2020 2020 2020 2020 2020 2320 4572              # Er
+0000f300: 726f 7220 7769 6c6c 2062 6520 7072 6f64  ror will be prod
+0000f310: 7563 6564 2e0a 2020 2020 2020 2020 2020  uced..          
+0000f320: 2020 636f 6e74 656e 742c 2072 6573 706f    content, respo
+0000f330: 6e73 6509 3d20 6973 7375 655f 7265 7175  nse.= issue_requ
+0000f340: 6573 7428 0a20 2020 2020 2020 2020 2020  est(.           
+0000f350: 2020 2020 2072 656e 6465 723d 7265 6e64       render=rend
+0000f360: 6572 2c20 7061 7468 3d70 6174 682c 2065  er, path=path, e
+0000f370: 6e76 6972 6f6e 3d77 6562 2e63 7478 2e65  nviron=web.ctx.e
+0000f380: 6e76 6972 6f6e 2c0a 2020 2020 2020 2020  nviron,.        
+0000f390: 2020 2020 2020 2020 6163 6365 7074 3d61          accept=a
+0000f3a0: 6363 6570 742c 2066 7261 6d65 776f 726b  ccept, framework
+0000f3b0: 3d77 6562 2c20 6c6f 6767 6564 3d6c 6f67  =web, logged=log
+0000f3c0: 6765 642c 0a20 2020 2020 2020 2020 2020  ged,.           
+0000f3d0: 2020 2020 202a 2a7b 2069 6e70 7574 5f76       **{ input_v
+0000f3e0: 6172 6961 626c 653a 2077 6562 2e69 6e70  ariable: web.inp
+0000f3f0: 7574 2829 207d 2029 0a20 2020 2020 2020  ut() } ).       
+0000f400: 2020 2020 2077 6562 2e68 6561 6465 7228       web.header(
+0000f410: 2022 4361 6368 652d 436f 6e74 726f 6c22   "Cache-Control"
+0000f420: 2c20 226e 6f2d 6361 6368 6522 2029 0a20  , "no-cache" ). 
+0000f430: 2020 2020 2020 2020 2020 2077 6562 2e68             web.h
+0000f440: 6561 6465 7228 2022 436f 6e74 656e 742d  eader( "Content-
+0000f450: 5479 7065 222c 2063 6f6e 7465 6e74 2029  Type", content )
+0000f460: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0000f470: 7572 6e20 7265 7370 6f6e 7365 0a0a 2020  urn response..  
+0000f480: 2020 2020 2020 6465 6620 504f 5354 2820        def POST( 
+0000f490: 7365 6c66 2c20 7061 7468 2029 3a0a 2020  self, path ):.  
+0000f4a0: 2020 2020 2020 2020 2020 2320 666f 726d            # form
+0000f4b0: 2064 6174 6120 706f 7374 6564 2069 6e20   data posted in 
+0000f4c0: 7765 622e 696e 7075 7428 292c 206a 7573  web.input(), jus
+0000f4d0: 7420 6c69 6b65 2071 7565 7269 6573 0a20  t like queries. 
+0000f4e0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000f4f0: 6e20 7365 6c66 2e47 4554 2820 7061 7468  n self.GET( path
+0000f500: 2c20 696e 7075 745f 7661 7269 6162 6c65  , input_variable
+0000f510: 3d22 706f 7374 6564 2220 290a 0a20 2020  ="posted" )..   
+0000f520: 2063 6c61 7373 2074 6162 756c 6172 5f72   class tabular_r
+0000f530: 6571 7565 7374 5f62 6173 653a 0a20 2020  equest_base:.   
+0000f540: 2020 2020 2023 2053 6574 2072 6571 7565       # Set reque
+0000f550: 7374 203d 203c 6675 6e63 7469 6f6e 2072  st = <function r
+0000f560: 6574 7572 6e69 6e67 2028 636f 6e74 656e  eturning (conten
+0000f570: 742c 2072 6573 706f 6e73 6529 3e0a 2020  t, response)>.  
+0000f580: 2020 2020 2020 6465 6620 4745 5428 2073        def GET( s
+0000f590: 656c 662c 2070 6174 682c 2069 6e70 7574  elf, path, input
+0000f5a0: 5f76 6172 6961 626c 653d 2271 7565 7269  _variable="queri
+0000f5b0: 6573 2220 293a 0a20 2020 2020 2020 2020  es" ):.         
+0000f5c0: 2020 2023 2069 6620 6e6f 7420 6c6f 6767     # if not logg
+0000f5d0: 6564 2829 3a0a 2020 2020 2020 2020 2020  ed():.          
+0000f5e0: 2020 2320 2020 2020 7765 622e 7365 656f    #     web.seeo
+0000f5f0: 7468 6572 2820 7072 6f78 7928 2077 6562  ther( proxy( web
+0000f600: 2e63 7478 2e65 6e76 6972 6f6e 2029 202b  .ctx.environ ) +
+0000f610: 2027 2f6c 6f67 696e 3f72 6564 6972 6563   '/login?redirec
+0000f620: 743d 2720 2b20 7765 622e 6374 782e 656e  t=' + web.ctx.en
+0000f630: 7669 726f 6e2e 6765 7428 2027 5041 5448  viron.get( 'PATH
+0000f640: 5f49 4e46 4f27 2c20 2727 2029 290a 2020  _INFO', '' )).  
+0000f650: 2020 2020 2020 2020 2020 2320 2020 2020            #     
+0000f660: 7265 7475 726e 0a20 2020 2020 2020 2020  return.         
+0000f670: 2020 2072 656e 6465 7209 093d 2077 6562     render..= web
+0000f680: 2e74 656d 706c 6174 652e 7265 6e64 6572  .template.render
+0000f690: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0000f6a0: 2020 5450 4c50 4154 482c 2062 6173 653d    TPLPATH, base=
+0000f6b0: 226c 6179 6f75 7422 2c20 676c 6f62 616c  "layout", global
+0000f6c0: 733d 7b27 696e 6c69 6e65 273a 2069 6e6c  s={'inline': inl
+0000f6d0: 696e 652c 2027 7365 7373 696f 6e27 3a20  ine, 'session': 
+0000f6e0: 7365 7373 696f 6e7d 2029 0a20 2020 2020  session} ).     
+0000f6f0: 2020 2020 2020 2061 6363 6570 7409 093d         accept..=
+0000f700: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
+0000f710: 2020 6966 2070 6174 6820 616e 6420 7061    if path and pa
+0000f720: 7468 2e65 6e64 7377 6974 6828 2022 2e6a  th.endswith( ".j
+0000f730: 736f 6e22 2029 3a0a 2020 2020 2020 2020  son" ):.        
+0000f740: 2020 2020 2020 2020 7061 7468 0909 3d20          path..= 
+0000f750: 7061 7468 5b3a 2d35 5d09 0923 2063 6c69  path[:-5]..# cli
+0000f760: 7020 6f66 6620 222e 6a73 6f6e 220a 2020  p off ".json".  
+0000f770: 2020 2020 2020 2020 2020 2020 2020 6163                ac
+0000f780: 6365 7074 0909 3d20 2261 7070 6c69 6361  cept..= "applica
+0000f790: 7469 6f6e 2f6a 736f 6e22 0a0a 2020 2020  tion/json"..    
+0000f7a0: 2020 2020 2020 2020 2320 416c 7761 7973          # Always
+0000f7b0: 2072 6574 7572 6e73 2061 2063 6f6e 7465   returns a conte
+0000f7c0: 6e74 2d74 7970 6520 616e 6420 7265 7370  nt-type and resp
+0000f7d0: 6f6e 7365 2e20 2049 6620 616e 2065 7863  onse.  If an exc
+0000f7e0: 6570 7469 6f6e 2069 730a 2020 2020 2020  eption is.      
+0000f7f0: 2020 2020 2020 2320 7261 6973 6564 2c20        # raised, 
+0000f800: 6974 2073 686f 756c 6420 6265 2061 6e20  it should be an 
+0000f810: 6170 7072 6f70 7269 6174 6520 6f6e 6520  appropriate one 
+0000f820: 6672 6f6d 2074 6865 2073 7570 706c 6965  from the supplie
+0000f830: 6420 6672 616d 6577 6f72 6b20 746f 0a20  d framework to. 
+0000f840: 2020 2020 2020 2020 2020 2023 2063 6172             # car
+0000f850: 7279 2061 206d 6561 6e69 6e67 6675 6c20  ry a meaningful 
+0000f860: 4854 5450 2073 7461 7475 7320 636f 6465  HTTP status code
+0000f870: 2e20 204f 7468 6572 7769 7365 2c20 6120  .  Otherwise, a 
+0000f880: 6765 6e65 7269 6320 3530 3020 5365 7276  generic 500 Serv
+0000f890: 6572 0a20 2020 2020 2020 2020 2020 2023  er.            #
+0000f8a0: 2045 7272 6f72 2077 696c 6c20 6265 2070   Error will be p
+0000f8b0: 726f 6475 6365 642e 0a20 2020 2020 2020  roduced..       
+0000f8c0: 2020 2020 2072 6571 7565 7374 0909 3d20       request..= 
+0000f8d0: 7365 6c66 2e5f 5f63 6c61 7373 5f5f 2e5f  self.__class__._
+0000f8e0: 5f64 6963 745f 5f5b 2772 6571 7565 7374  _dict__['request
+0000f8f0: 275d 0a20 2020 2020 2020 2020 2020 206c  '].            l
+0000f900: 6f67 2e69 6e66 6f28 2022 5461 6275 6c61  og.info( "Tabula
+0000f910: 7220 4150 4920 6361 6c6c 3a20 7b21 727d  r API call: {!r}
+0000f920: 222e 666f 726d 6174 2820 7265 7175 6573  ".format( reques
+0000f930: 7420 2929 0a20 2020 2020 2020 2020 2020  t )).           
+0000f940: 2063 6f6e 7465 6e74 2c20 7265 7370 6f6e   content, respon
+0000f950: 7365 093d 2072 6571 7565 7374 280a 2020  se.= request(.  
+0000f960: 2020 2020 2020 2020 2020 2020 2020 7265                re
+0000f970: 6e64 6572 3d72 656e 6465 722c 2070 6174  nder=render, pat
+0000f980: 683d 7061 7468 2c20 656e 7669 726f 6e3d  h=path, environ=
+0000f990: 7765 622e 6374 782e 656e 7669 726f 6e2c  web.ctx.environ,
+0000f9a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f9b0: 2061 6363 6570 743d 6163 6365 7074 2c20   accept=accept, 
+0000f9c0: 6672 616d 6577 6f72 6b3d 7765 622c 206c  framework=web, l
+0000f9d0: 6f67 6765 643d 6c6f 6767 6564 2c0a 2020  ogged=logged,.  
+0000f9e0: 2020 2020 2020 2020 2020 2020 2020 2a2a                **
+0000f9f0: 7b20 696e 7075 745f 7661 7269 6162 6c65  { input_variable
+0000fa00: 3a20 7765 622e 696e 7075 7428 2920 7d20  : web.input() } 
+0000fa10: 290a 2020 2020 2020 2020 2020 2020 7765  ).            we
+0000fa20: 622e 6865 6164 6572 2820 2243 6163 6865  b.header( "Cache
+0000fa30: 2d43 6f6e 7472 6f6c 222c 2022 6e6f 2d63  -Control", "no-c
+0000fa40: 6163 6865 2220 290a 2020 2020 2020 2020  ache" ).        
+0000fa50: 2020 2020 7765 622e 6865 6164 6572 2820      web.header( 
+0000fa60: 2243 6f6e 7465 6e74 2d54 7970 6522 2c20  "Content-Type", 
+0000fa70: 636f 6e74 656e 7420 290a 2020 2020 2020  content ).      
+0000fa80: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+0000fa90: 706f 6e73 650a 0a20 2020 2020 2020 2064  ponse..        d
+0000faa0: 6566 2050 4f53 5428 2073 656c 662c 2070  ef POST( self, p
+0000fab0: 6174 6820 293a 0a20 2020 2020 2020 2020  ath ):.         
+0000fac0: 2020 2023 2066 6f72 6d20 6461 7461 2070     # form data p
+0000fad0: 6f73 7465 6420 696e 2077 6562 2e69 6e70  osted in web.inp
+0000fae0: 7574 2829 2c20 6a75 7374 206c 696b 6520  ut(), just like 
+0000faf0: 7175 6572 6965 730a 2020 2020 2020 2020  queries.        
+0000fb00: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+0000fb10: 4745 5428 2070 6174 682c 2069 6e70 7574  GET( path, input
+0000fb20: 5f76 6172 6961 626c 653d 2270 6f73 7465  _variable="poste
+0000fb30: 6422 2029 0a0a 2020 2020 636c 6173 7320  d" )..    class 
+0000fb40: 6170 695f 6c69 6365 6e73 6573 2820 7461  api_licenses( ta
+0000fb50: 6275 6c61 725f 7265 7175 6573 745f 6261  bular_request_ba
+0000fb60: 7365 2029 3a0a 2020 2020 2020 2020 7265  se ):.        re
+0000fb70: 7175 6573 7409 0909 3d20 6c69 6365 6e73  quest...= licens
+0000fb80: 6573 5f72 6571 7565 7374 0a0a 2020 2020  es_request..    
+0000fb90: 636c 6173 7320 6170 695f 6372 6564 656e  class api_creden
+0000fba0: 7469 616c 7328 2074 6162 756c 6172 5f72  tials( tabular_r
+0000fbb0: 6571 7565 7374 5f62 6173 6520 293a 0a20  equest_base ):. 
+0000fbc0: 2020 2020 2020 2072 6571 7565 7374 0909         request..
+0000fbd0: 093d 2063 7265 6465 6e74 6961 6c73 5f72  .= credentials_r
+0000fbe0: 6571 7565 7374 0a0a 2020 2020 636c 6173  equest..    clas
+0000fbf0: 7320 6170 695f 6b65 7970 6169 7273 2820  s api_keypairs( 
+0000fc00: 7461 6275 6c61 725f 7265 7175 6573 745f  tabular_request_
+0000fc10: 6261 7365 2029 3a0a 2020 2020 2020 2020  base ):.        
+0000fc20: 7265 7175 6573 7409 0909 3d20 6b65 7970  request...= keyp
+0000fc30: 6169 7273 5f72 6571 7565 7374 0a0a 2020  airs_request..  
+0000fc40: 2020 636c 6173 7320 5374 6174 6963 4170    class StaticAp
+0000fc50: 7044 6972 2820 7765 622e 6874 7470 7365  pDir( web.httpse
+0000fc60: 7276 6572 2e53 7461 7469 6341 7070 2c20  rver.StaticApp, 
+0000fc70: 6f62 6a65 6374 2029 3a0a 2020 2020 2020  object ):.      
+0000fc80: 2020 2222 2249 6d70 6c65 6d65 6e74 206f    """Implement o
+0000fc90: 7572 206f 776e 2076 6572 7369 6f6e 206f  ur own version o
+0000fca0: 6620 5374 6174 6963 4170 7020 616e 6420  f StaticApp and 
+0000fcb0: 5374 6174 6963 4d69 6464 6c65 7761 7265  StaticMiddleware
+0000fcc0: 2073 6f20 7765 2063 616e 2072 6574 7572   so we can retur
+0000fcd0: 6e20 7072 6f70 6572 2063 6163 6869 6e67  n proper caching
+0000fce0: 0a20 2020 2020 2020 2068 6561 6465 7273  .        headers
+0000fcf0: 2c20 616e 6420 7370 6563 6966 7920 6120  , and specify a 
+0000fd00: 7370 6563 6966 6963 2062 6173 6564 6972  specific basedir
+0000fd10: 2066 6f72 2073 7461 7469 6320 6669 6c65   for static file
+0000fd20: 2061 6363 6573 732e 2046 6f72 6365 206e   access. Force n
+0000fd30: 6577 2d73 7479 6c65 2063 6c61 7373 6573  ew-style classes
+0000fd40: 2069 6e0a 2020 2020 2020 2020 5079 7468   in.        Pyth
+0000fd50: 6f6e 3220 736f 2073 7570 6572 2077 6f72  on2 so super wor
+0000fd60: 6b73 2e20 2055 6e66 6f72 7475 6e61 7465  ks.  Unfortunate
+0000fd70: 6c79 2c20 7468 6520 5079 7468 6f6e 3220  ly, the Python2 
+0000fd80: 5369 6d70 6c65 4854 5450 5265 7175 6573  SimpleHTTPReques
+0000fd90: 7420 696d 706c 656d 656e 7461 7469 6f6e  t implementation
+0000fda0: 2062 616b 6564 0a20 2020 2020 2020 2069   baked.        i
+0000fdb0: 6e20 6f73 2e67 6574 6377 6420 736f 2077  n os.getcwd so w
+0000fdc0: 6520 6861 7665 2074 6f20 7472 616e 7370  e have to transp
+0000fdd0: 6c61 6e74 2061 2050 7974 686f 6e32 2f33  lant a Python2/3
+0000fde0: 2063 6f6d 7061 7469 626c 6520 7472 616e   compatible tran
+0000fdf0: 736c 6174 655f 7061 7468 2c20 746f 6f2e  slate_path, too.
+0000fe00: 0a0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+0000fe10: 2020 2020 2020 6465 6620 5f5f 696e 6974        def __init
+0000fe20: 5f5f 2820 7365 6c66 2c20 656e 7669 726f  __( self, enviro
+0000fe30: 6e2c 2073 7461 7274 5f72 6573 706f 6e73  n, start_respons
+0000fe40: 652c 2064 6972 6563 746f 7279 2029 3a0a  e, directory ):.
+0000fe50: 2020 2020 2020 2020 2020 2020 7375 7065              supe
+0000fe60: 7228 2053 7461 7469 6341 7070 4469 722c  r( StaticAppDir,
+0000fe70: 2073 656c 6620 292e 5f5f 696e 6974 5f5f   self ).__init__
+0000fe80: 2820 656e 7669 726f 6e2c 2073 7461 7274  ( environ, start
+0000fe90: 5f72 6573 706f 6e73 6520 290a 2020 2020  _response ).    
+0000fea0: 2020 2020 2020 2020 7365 6c66 2e64 6972          self.dir
+0000feb0: 6563 746f 7279 093d 2064 6972 6563 746f  ectory.= directo
+0000fec0: 7279 0a0a 2020 2020 2020 2020 6465 6620  ry..        def 
+0000fed0: 7472 616e 736c 6174 655f 7061 7468 2873  translate_path(s
+0000fee0: 656c 662c 2070 6174 6829 3a0a 2020 2020  elf, path):.    
+0000fef0: 2020 2020 2020 2020 2222 2254 7261 6e73          """Trans
+0000ff00: 6c61 7465 2061 202f 2d73 6570 6172 6174  late a /-separat
+0000ff10: 6564 2050 4154 4820 746f 2074 6865 206c  ed PATH to the l
+0000ff20: 6f63 616c 2066 696c 656e 616d 6520 7379  ocal filename sy
+0000ff30: 6e74 6178 2e0a 0a20 2020 2020 2020 2020  ntax...         
+0000ff40: 2020 2043 6f6d 706f 6e65 6e74 7320 7468     Components th
+0000ff50: 6174 206d 6561 6e20 7370 6563 6961 6c20  at mean special 
+0000ff60: 7468 696e 6773 2074 6f20 7468 6520 6c6f  things to the lo
+0000ff70: 6361 6c20 6669 6c65 2073 7973 7465 6d0a  cal file system.
+0000ff80: 2020 2020 2020 2020 2020 2020 2865 2e67              (e.g
+0000ff90: 2e20 6472 6976 6520 6f72 2064 6972 6563  . drive or direc
+0000ffa0: 746f 7279 206e 616d 6573 2920 6172 6520  tory names) are 
+0000ffb0: 6967 6e6f 7265 642e 2020 2858 5858 2054  ignored.  (XXX T
+0000ffc0: 6865 7920 7368 6f75 6c64 0a20 2020 2020  hey should.     
+0000ffd0: 2020 2020 2020 2070 726f 6261 626c 7920         probably 
+0000ffe0: 6265 2064 6961 676e 6f73 6564 2e29 0a0a  be diagnosed.)..
+0000fff0: 2020 2020 2020 2020 2020 2020 2222 220a              """.
+00010000: 2020 2020 2020 2020 2020 2020 2320 6162              # ab
+00010010: 616e 646f 6e20 7175 6572 7920 7061 7261  andon query para
+00010020: 6d65 7465 7273 0a20 2020 2020 2020 2020  meters.         
+00010030: 2020 2070 6174 6820 3d20 7061 7468 2e73     path = path.s
+00010040: 706c 6974 2827 3f27 2c31 295b 305d 0a20  plit('?',1)[0]. 
+00010050: 2020 2020 2020 2020 2020 2070 6174 6820             path 
+00010060: 3d20 7061 7468 2e73 706c 6974 2827 2327  = path.split('#'
+00010070: 2c31 295b 305d 0a20 2020 2020 2020 2020  ,1)[0].         
+00010080: 2020 2023 2044 6f6e 2774 2066 6f72 6765     # Don't forge
+00010090: 7420 6578 706c 6963 6974 2074 7261 696c  t explicit trail
+000100a0: 696e 6720 736c 6173 6820 7768 656e 206e  ing slash when n
+000100b0: 6f72 6d61 6c69 7a69 6e67 2e20 4973 7375  ormalizing. Issu
+000100c0: 6531 3733 3234 0a20 2020 2020 2020 2020  e17324.         
+000100d0: 2020 2074 7261 696c 696e 675f 736c 6173     trailing_slas
+000100e0: 6820 3d20 7061 7468 2e72 7374 7269 7028  h = path.rstrip(
+000100f0: 292e 656e 6473 7769 7468 2827 2f27 290a  ).endswith('/').
+00010100: 2020 2020 2020 2020 2020 2020 7061 7468              path
+00010110: 203d 2070 6f73 6978 7061 7468 2e6e 6f72   = posixpath.nor
+00010120: 6d70 6174 6828 756e 7175 6f74 6528 7061  mpath(unquote(pa
+00010130: 7468 2929 0a20 2020 2020 2020 2020 2020  th)).           
+00010140: 2077 6f72 6473 203d 2070 6174 682e 7370   words = path.sp
+00010150: 6c69 7428 272f 2729 0a20 2020 2020 2020  lit('/').       
+00010160: 2020 2020 2077 6f72 6473 203d 2066 696c       words = fil
+00010170: 7465 7228 4e6f 6e65 2c20 776f 7264 7329  ter(None, words)
+00010180: 0a20 2020 2020 2020 2020 2020 2070 6174  .            pat
+00010190: 6820 3d20 7365 6c66 2e64 6972 6563 746f  h = self.directo
+000101a0: 7279 2020 2320 3c3c 2044 276f 6821 0a20  ry  # << D'oh!. 
+000101b0: 2020 2020 2020 2020 2020 2066 6f72 2077             for w
+000101c0: 6f72 6420 696e 2077 6f72 6473 3a0a 2020  ord in words:.  
+000101d0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+000101e0: 206f 732e 7061 7468 2e64 6972 6e61 6d65   os.path.dirname
+000101f0: 2877 6f72 6429 206f 7220 776f 7264 2069  (word) or word i
+00010200: 6e20 286f 732e 6375 7264 6972 2c20 6f73  n (os.curdir, os
+00010210: 2e70 6172 6469 7229 3a0a 2020 2020 2020  .pardir):.      
+00010220: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00010230: 4967 6e6f 7265 2063 6f6d 706f 6e65 6e74  Ignore component
+00010240: 7320 7468 6174 2061 7265 206e 6f74 2061  s that are not a
+00010250: 2073 696d 706c 6520 6669 6c65 2f64 6972   simple file/dir
+00010260: 6563 746f 7279 206e 616d 650a 2020 2020  ectory name.    
+00010270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010280: 636f 6e74 696e 7565 0a20 2020 2020 2020  continue.       
+00010290: 2020 2020 2020 2020 2070 6174 6820 3d20           path = 
+000102a0: 6f73 2e70 6174 682e 6a6f 696e 2870 6174  os.path.join(pat
+000102b0: 682c 2077 6f72 6429 0a20 2020 2020 2020  h, word).       
+000102c0: 2020 2020 2069 6620 7472 6169 6c69 6e67       if trailing
+000102d0: 5f73 6c61 7368 3a0a 2020 2020 2020 2020  _slash:.        
+000102e0: 2020 2020 2020 2020 7061 7468 202b 3d20          path += 
+000102f0: 272f 270a 2020 2020 2020 2020 2020 2020  '/'.            
+00010300: 7265 7475 726e 2070 6174 680a 0a20 2020  return path..   
+00010310: 2063 6163 6865 5f6d 6178 5f61 6765 0909   cache_max_age..
+00010320: 3d20 3330 2a32 342a 3630 2a36 300a 0a20  = 30*24*60*60.. 
+00010330: 2020 2063 6c61 7373 2053 7461 7469 634d     class StaticM
+00010340: 6964 646c 6577 6172 6544 6972 2820 7765  iddlewareDir( we
+00010350: 622e 6874 7470 7365 7276 6572 2e53 7461  b.httpserver.Sta
+00010360: 7469 634d 6964 646c 6577 6172 652c 206f  ticMiddleware, o
+00010370: 626a 6563 7420 293a 0a20 2020 2020 2020  bject ):.       
+00010380: 2022 2222 5753 4749 206d 6964 646c 6577   """WSGI middlew
+00010390: 6172 6520 666f 7220 7365 7276 696e 6720  are for serving 
+000103a0: 7374 6174 6963 2066 696c 6573 2066 726f  static files fro
+000103b0: 6d20 7468 6520 7370 6563 6966 6965 6420  m the specified 
+000103c0: 6261 7365 6469 722e 2222 220a 2020 2020  basedir.""".    
+000103d0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+000103e0: 2820 7365 6c66 2c20 6170 702c 2070 7265  ( self, app, pre
+000103f0: 6669 783d 222f 7374 6174 6963 2f22 2c20  fix="/static/", 
+00010400: 6261 7365 6469 723d 6f73 2e67 6574 6377  basedir=os.getcw
+00010410: 6428 2920 293a 0a20 2020 2020 2020 2020  d() ):.         
+00010420: 2020 2073 7570 6572 2820 5374 6174 6963     super( Static
+00010430: 4d69 6464 6c65 7761 7265 4469 722c 2073  MiddlewareDir, s
+00010440: 656c 6620 292e 5f5f 696e 6974 5f5f 2820  elf ).__init__( 
+00010450: 6170 702c 2070 7265 6669 783d 7072 6566  app, prefix=pref
+00010460: 6978 2029 0a20 2020 2020 2020 2020 2020  ix ).           
+00010470: 2073 656c 662e 6261 7365 6469 7209 3d20   self.basedir.= 
+00010480: 6261 7365 6469 720a 2020 2020 2020 2020  basedir.        
+00010490: 2020 2020 6c6f 6767 696e 672e 696e 666f      logging.info
+000104a0: 2820 2253 6572 7669 6e67 2073 7461 7469  ( "Serving stati
+000104b0: 6320 6669 6c65 7320 6f75 7420 6f66 207b  c files out of {
+000104c0: 7d22 2e66 6f72 6d61 7428 2062 6173 6564  }".format( based
+000104d0: 6972 202b 2070 7265 6669 7820 2929 0a0a  ir + prefix ))..
+000104e0: 2020 2020 2020 2020 6465 6620 5f5f 6361          def __ca
+000104f0: 6c6c 5f5f 2820 7365 6c66 2c20 656e 7669  ll__( self, envi
+00010500: 726f 6e2c 2073 7461 7274 5f72 6573 706f  ron, start_respo
+00010510: 6e73 6520 293a 0a20 2020 2020 2020 2020  nse ):.         
+00010520: 2020 2070 6174 6820 0909 3d20 656e 7669     path ..= envi
+00010530: 726f 6e2e 6765 7428 2027 5041 5448 5f49  ron.get( 'PATH_I
+00010540: 4e46 4f27 2c20 2727 2029 0a20 2020 2020  NFO', '' ).     
+00010550: 2020 2020 2020 2070 6174 6820 0909 3d20         path ..= 
+00010560: 7365 6c66 2e6e 6f72 6d70 6174 6828 2070  self.normpath( p
+00010570: 6174 6820 290a 2020 2020 2020 2020 2020  ath ).          
+00010580: 2020 6966 2070 6174 682e 7374 6172 7473    if path.starts
+00010590: 7769 7468 2873 656c 662e 7072 6566 6978  with(self.prefix
+000105a0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+000105b0: 2020 2061 7070 2009 093d 2053 7461 7469     app ..= Stati
+000105c0: 6341 7070 4469 7228 2065 6e76 6972 6f6e  cAppDir( environ
+000105d0: 2c20 7374 6172 745f 7265 7370 6f6e 7365  , start_response
+000105e0: 2c20 7365 6c66 2e62 6173 6564 6972 2029  , self.basedir )
+000105f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010600: 2061 7070 2e73 656e 645f 6865 6164 6572   app.send_header
+00010610: 2820 2743 6163 6865 2d43 6f6e 7472 6f6c  ( 'Cache-Control
+00010620: 272c 2027 7075 626c 6963 2c20 6d61 782d  ', 'public, max-
+00010630: 6167 653d 2564 2720 2520 2820 6361 6368  age=%d' % ( cach
+00010640: 655f 6d61 785f 6167 6520 2929 0a20 2020  e_max_age )).   
+00010650: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00010660: 7572 6e20 6170 700a 2020 2020 2020 2020  urn app.        
+00010670: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00010680: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00010690: 2073 656c 662e 6170 7028 2065 6e76 6972   self.app( envir
+000106a0: 6f6e 2c20 7374 6172 745f 7265 7370 6f6e  on, start_respon
+000106b0: 7365 2029 0a0a 2020 2020 636c 6173 7320  se )..    class 
+000106c0: 4c6f 674d 6964 646c 6577 6172 6543 4628  LogMiddlewareCF(
+000106d0: 2077 6562 2e68 7474 7073 6572 7665 722e   web.httpserver.
+000106e0: 4c6f 674d 6964 646c 6577 6172 652c 206f  LogMiddleware, o
+000106f0: 626a 6563 7420 293a 0a20 2020 2020 2020  bject ):.       
+00010700: 2064 6566 206c 6f67 2820 7365 6c66 2c20   def log( self, 
+00010710: 7374 6174 7573 2c20 656e 7669 726f 6e20  status, environ 
+00010720: 293a 0a20 2020 2020 2020 2020 2020 2063  ):.            c
+00010730: 665f 6970 0909 3d20 656e 7669 726f 6e2e  f_ip..= environ.
+00010740: 6765 7428 2027 4854 5450 5f43 465f 434f  get( 'HTTP_CF_CO
+00010750: 4e4e 4543 5449 4e47 5f49 5027 2029 0a20  NNECTING_IP' ). 
+00010760: 2020 2020 2020 2020 2020 2069 6620 6366             if cf
+00010770: 5f69 7020 6973 204e 6f6e 653a 0a20 2020  _ip is None:.   
+00010780: 2020 2020 2020 2020 2020 2020 2063 665f               cf_
+00010790: 6970 0909 3d20 656e 7669 726f 6e2e 6765  ip..= environ.ge
+000107a0: 7428 2027 4854 5450 5f58 5f46 4f52 5741  t( 'HTTP_X_FORWA
+000107b0: 5244 4544 5f46 4f52 2720 290a 2020 2020  RDED_FOR' ).    
+000107c0: 2020 2020 2020 2020 6966 2063 665f 6970          if cf_ip
+000107d0: 2069 7320 6e6f 7420 4e6f 6e65 2061 6e64   is not None and
+000107e0: 2027 2c27 2069 6e20 6366 5f69 703a 0a20   ',' in cf_ip:. 
+000107f0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00010800: 2043 4620 6170 7065 6e64 7320 636f 6e6e   CF appends conn
+00010810: 6563 7469 6e67 2049 5020 746f 2058 5f46  ecting IP to X_F
+00010820: 4f52 5741 5244 4544 5f46 4f52 0a20 2020  ORWARDED_FOR.   
+00010830: 2020 2020 2020 2020 2020 2020 2063 665f               cf_
+00010840: 6970 0909 3d20 6366 5f69 702e 7370 6c69  ip..= cf_ip.spli
+00010850: 7428 2027 2c27 2029 5b2d 315d 2e73 7472  t( ',' )[-1].str
+00010860: 6970 2829 0a20 2020 2020 2020 2020 2020  ip().           
+00010870: 2063 665f 636f 756e 7472 7909 093d 2065   cf_country..= e
+00010880: 6e76 6972 6f6e 2e67 6574 2820 2748 5454  nviron.get( 'HTT
+00010890: 505f 4346 5f49 5043 4f55 4e54 5259 2720  P_CF_IPCOUNTRY' 
+000108a0: 290a 0a20 2020 2020 2020 2020 2020 2023  )..            #
+000108b0: 6970 2c70 6f72 7409 093d 2065 6e76 6972  ip,port..= envir
+000108c0: 6f6e 2e67 6574 2820 2752 454d 4f54 455f  on.get( 'REMOTE_
+000108d0: 4144 4452 2720 292c 656e 7669 726f 6e2e  ADDR' ),environ.
+000108e0: 6765 7428 2027 5245 4d4f 5445 5f50 4f52  get( 'REMOTE_POR
+000108f0: 5427 2029 0a20 2020 2020 2020 2020 2020  T' ).           
+00010900: 2069 6620 6366 5f69 703a 0a20 2020 2020   if cf_ip:.     
+00010910: 2020 2020 2020 2020 2020 2065 6e76 6972             envir
+00010920: 6f6e 5b27 5245 4d4f 5445 5f41 4444 5227  on['REMOTE_ADDR'
+00010930: 5d20 3d20 6366 5f69 700a 2020 2020 2020  ] = cf_ip.      
+00010940: 2020 2020 2020 6966 2063 665f 636f 756e        if cf_coun
+00010950: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+00010960: 2020 2020 2065 6e76 6972 6f6e 5b27 5245       environ['RE
+00010970: 4d4f 5445 5f50 4f52 5427 5d20 3d20 6366  MOTE_PORT'] = cf
+00010980: 5f63 6f75 6e74 7279 0a20 2020 2020 2020  _country.       
+00010990: 2020 2020 2072 6574 7572 6e20 7375 7065       return supe
+000109a0: 7228 204c 6f67 4d69 6464 6c65 7761 7265  r( LogMiddleware
+000109b0: 4346 2c20 7365 6c66 2029 2e6c 6f67 2820  CF, self ).log( 
+000109c0: 7374 6174 7573 2c20 656e 7669 726f 6e20  status, environ 
+000109d0: 290a 0a20 2020 2023 2047 6574 2074 6865  )..    # Get the
+000109e0: 2072 6571 7569 7265 6420 7765 622e 7079   required web.py
+000109f0: 2063 6c61 7373 6573 2066 726f 6d20 7468   classes from th
+00010a00: 6520 6c6f 6361 6c20 6e61 6d65 7370 6163  e local namespac
+00010a10: 652e 2020 5468 6520 6966 6163 653a 706f  e.  The iface:po
+00010a20: 7274 206d 7573 7420 616c 7761 7973 2070  rt must always p
+00010a30: 6173 7365 640a 2020 2020 2320 6f6e 2061  assed.    # on a
+00010a40: 7267 765b 315d 2074 6f20 7573 6520 6170  rgv[1] to use ap
+00010a50: 702e 7275 6e28 292c 2073 6f20 7573 6520  p.run(), so use 
+00010a60: 6c6f 7765 722d 6c65 7665 6c20 7765 622e  lower-level web.
+00010a70: 6874 7470 7365 7276 6572 2e72 756e 7369  httpserver.runsi
+00010a80: 6d70 6c65 2069 6e74 6572 6661 6365 2e20  mple interface. 
+00010a90: 2054 6869 7320 7365 7473 0a20 2020 2023   This sets.    #
+00010aa0: 2075 7020 7468 6520 5753 4749 206d 6964   up the WSGI mid
+00010ab0: 646c 6577 6172 6520 6368 6169 6e2c 2070  dleware chain, p
+00010ac0: 7269 6e74 7320 7468 6520 6164 6472 6573  rints the addres
+00010ad0: 7320 616e 6420 7468 656e 2069 6e76 6f6b  s and then invok
+00010ae0: 6573 0a20 2020 2023 2068 7474 7073 6572  es.    # httpser
+00010af0: 7665 722e 5753 4749 7365 7276 6572 2e73  ver.WSGIserver.s
+00010b00: 7461 7274 2829 2c20 7768 6963 6820 646f  tart(), which do
+00010b10: 6573 2074 6865 2062 696e 642c 2061 6e64  es the bind, and
+00010b20: 2074 6865 6e20 6d61 6b65 7320 5753 4749   then makes WSGI
+00010b30: 2063 616c 6c73 0a20 2020 2061 7070 0909   calls.    app..
+00010b40: 0909 3d20 7765 622e 6170 706c 6963 6174  ..= web.applicat
+00010b50: 696f 6e28 2075 726c 732c 206c 6f63 616c  ion( urls, local
+00010b60: 7328 2920 290a 0a20 2020 2023 2053 6573  s() )..    # Ses
+00010b70: 7369 6f6e 730a 2020 2020 676c 6f62 616c  sions.    global
+00010b80: 2073 6573 7369 6f6e 5f69 6e69 7469 616c   session_initial
+00010b90: 697a 6572 0a20 2020 2073 6573 7369 6f6e  izer.    session
+00010ba0: 0909 093d 2077 6562 2e73 6573 7369 6f6e  ...= web.session
+00010bb0: 2e53 6573 7369 6f6e 280a 2020 2020 2020  .Session(.      
+00010bc0: 2020 6170 702c 2077 6562 2e73 6573 7369    app, web.sessi
+00010bd0: 6f6e 2e44 4253 746f 7265 2820 6462 2c20  on.DBStore( db, 
+00010be0: 2773 6573 7369 6f6e 7327 2029 2c20 696e  'sessions' ), in
+00010bf0: 6974 6961 6c69 7a65 723d 7365 7373 696f  itializer=sessio
+00010c00: 6e5f 696e 6974 6961 6c69 7a65 7220 290a  n_initializer ).
+00010c10: 0a20 2020 2023 2057 6520 6361 6e27 7420  .    # We can't 
+00010c20: 7573 6520 7468 6520 7374 6f63 6b20 7275  use the stock ru
+00010c30: 6e73 696d 706c 653b 2077 6520 6861 7665  nsimple; we have
+00010c40: 2074 6f20 6275 696c 6420 7570 206f 7572   to build up our
+00010c50: 206f 776e 2063 6861 696e 206f 6620 5753   own chain of WS
+00010c60: 4749 206d 6964 646c 6577 6172 6520 616e  GI middleware an
+00010c70: 6420 7275 6e0a 2020 2020 2320 6974 7320  d run.    # its 
+00010c80: 7365 7276 6572 2c20 696e 206f 7264 6572  server, in order
+00010c90: 2074 6f20 6765 7420 6f75 7220 6375 7374   to get our cust
+00010ca0: 6f6d 2053 7461 7469 634d 6964 646c 6577  om StaticMiddlew
+00010cb0: 6172 652f 5374 6174 6963 4170 7020 746f  are/StaticApp to
+00010cc0: 2073 6572 7665 2073 7461 7469 6320 6669   serve static fi
+00010cd0: 6c65 7320 6672 6f6d 0a20 2020 2023 2074  les from.    # t
+00010ce0: 6865 2050 7974 686f 6e20 6d6f 6475 6c65  he Python module
+00010cf0: 2069 6e73 7461 6c6c 6174 696f 6e20 6469   installation di
+00010d00: 7265 6374 6f72 792e 0a20 2020 2061 6363  rectory..    acc
+00010d10: 6573 7309 0909 3d20 636f 6e66 6967 2e67  ess...= config.g
+00010d20: 6574 2820 2761 6363 6573 7327 2029 0a0a  et( 'access' )..
+00010d30: 2020 2020 2320 4c6f 6720 7765 622e 7079      # Log web.py
+00010d40: 2048 5454 5020 7265 7175 6573 7473 2074   HTTP requests t
+00010d50: 6f20 6c69 6365 6e73 696e 672e 6163 6365  o licensing.acce
+00010d60: 7373 0a20 2020 2063 6c61 7373 204c 6f67  ss.    class Log
+00010d70: 5374 646f 7574 2820 7773 6769 6c6f 672e  Stdout( wsgilog.
+00010d80: 4c6f 6753 7464 6f75 7420 293a 0a20 2020  LogStdout ):.   
+00010d90: 2020 2020 2022 2222 496d 706c 656d 656e       """Implemen
+00010da0: 7420 7468 6520 6d69 7373 696e 6720 666c  t the missing fl
+00010db0: 7573 6820 4150 4920 746f 2061 766f 6964  ush API to avoid
+00010dc0: 2077 6172 6e69 6e67 7322 2222 0a20 2020   warnings""".   
+00010dd0: 2020 2020 2064 6566 2066 6c75 7368 2873       def flush(s
+00010de0: 656c 6629 3a0a 2020 2020 2020 2020 2020  elf):.          
+00010df0: 2020 7061 7373 0a0a 2020 2020 636c 6173    pass..    clas
+00010e00: 7320 4c6f 6728 2077 7367 696c 6f67 2e57  s Log( wsgilog.W
+00010e10: 7367 694c 6f67 2c20 6f62 6a65 6374 2029  sgiLog, object )
+00010e20: 3a0a 2020 2020 2020 2020 2222 2244 6972  :.        """Dir
+00010e30: 6563 7420 6c6f 6720 6d65 7373 6167 6573  ect log messages
+00010e40: 2074 6f20 7468 6520 636f 7272 6563 7420   to the correct 
+00010e50: 6c6f 6720 6669 6c65 2c20 696e 636c 7564  log file, includ
+00010e60: 696e 6720 7374 646f 7574 2f73 7464 6572  ing stdout/stder
+00010e70: 722e 2020 4265 6361 7573 6520 7765 2772  r.  Because we'r
+00010e80: 6520 7275 6e6e 696e 670a 2020 2020 2020  e running.      
+00010e90: 2020 6120 6375 7273 6573 2074 6578 7475    a curses textu
+00010ea0: 616c 2055 492c 2077 6520 646f 6e27 7420  al UI, we don't 
+00010eb0: 7761 6e74 2073 7475 6666 2062 6569 6e67  want stuff being
+00010ec0: 2070 7269 6e74 6564 2074 6f20 7468 6520   printed to the 
+00010ed0: 7363 7265 656e 2061 6363 6964 656e 7461  screen accidenta
+00010ee0: 6c6c 7920 2d2d 206d 616b 650a 2020 2020  lly -- make.    
+00010ef0: 2020 2020 7375 7265 2069 7420 616c 6c20      sure it all 
+00010f00: 676f 6573 2074 6f20 7468 6520 6c6f 6720  goes to the log 
+00010f10: 6669 6c65 2e0a 0a20 2020 2020 2020 2022  file...        "
+00010f20: 2222 0a20 2020 2020 2020 2064 6566 205f  "".        def _
+00010f30: 5f69 6e69 745f 5f28 2073 656c 662c 2061  _init__( self, a
+00010f40: 7070 6c69 6361 7469 6f6e 2029 3a0a 2020  pplication ):.  
+00010f50: 2020 2020 2020 2020 2020 2222 2253 6574            """Set
+00010f60: 2075 7020 6c6f 6767 696e 672c 2061 6e64   up logging, and
+00010f70: 2074 6865 6e20 6d61 6b65 2073 7572 6520   then make sure 
+00010f80: 7379 732e 7374 6465 7272 2067 6f65 7320  sys.stderr goes 
+00010f90: 746f 2077 6865 7265 6576 6572 2073 7973  to whereever sys
+00010fa0: 2e73 7464 6f75 7420 6973 206e 6f77 2067  .stdout is now g
+00010fb0: 6f69 6e67 2e20 2054 6869 730a 2020 2020  oing.  This.    
+00010fc0: 2020 2020 2020 2020 656e 7375 7265 7320          ensures 
+00010fd0: 7468 6174 2065 6e76 6972 6f6e 5b27 7773  that environ['ws
+00010fe0: 6769 2e65 7272 6f72 7327 5d20 2877 6869  gi.errors'] (whi
+00010ff0: 6368 2069 7320 616c 7761 7973 2073 6574  ch is always set
+00011000: 2074 6f20 7379 732e 7374 6465 7272 2062   to sys.stderr b
+00011010: 7920 7765 622e 7079 2920 676f 6573 0a20  y web.py) goes. 
+00011020: 2020 2020 2020 2020 2020 2074 6f20 7468             to th
+00011030: 6520 2e61 6363 6573 7320 6c6f 6720 6669  e .access log fi
+00011040: 6c65 3b20 7468 6973 2069 7320 7573 6564  le; this is used
+00011050: 2074 6f20 6c6f 6720 6561 6368 2069 6e63   to log each inc
+00011060: 6f6d 696e 6720 4854 5450 2072 6571 7565  oming HTTP reque
+00011070: 7374 2e0a 0a20 2020 2020 2020 2020 2020  st...           
+00011080: 2022 2222 0a20 2020 2020 2020 2020 2020   """.           
+00011090: 2069 6620 6163 6365 7373 3a0a 2020 2020   if access:.    
+000110a0: 2020 2020 2020 2020 2020 2020 7375 7065              supe
+000110b0: 7228 204c 6f67 2c20 7365 6c66 2029 2e5f  r( Log, self )._
+000110c0: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
+000110d0: 2020 2020 2020 2020 2020 2020 2061 7070               app
+000110e0: 6c69 6361 7469 6f6e 2c0a 2020 2020 2020  lication,.      
+000110f0: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+00011100: 6766 6f72 6d61 7409 3d20 2225 286d 6573  gformat.= "%(mes
+00011110: 7361 6765 2973 222c 0a20 2020 2020 2020  sage)s",.       
+00011120: 2020 2020 2020 2020 2020 2020 206c 6f67               log
+00011130: 0909 3d20 5472 7565 2c0a 2020 2020 2020  ..= True,.      
+00011140: 2020 2020 2020 2020 2020 2020 2020 746f                to
+00011150: 6874 6d6c 093d 2054 7275 652c 0909 0909  html.= True,....
+00011160: 2320 4578 6365 7074 696f 6e73 2067 656e  # Exceptions gen
+00011170: 6572 6174 6520 4854 4d4c 0a20 2020 2020  erate HTML.     
+00011180: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00011190: 6f66 696c 6509 3d20 5472 7565 2c09 0909  ofile.= True,...
+000111a0: 0923 204c 6f67 6769 6e67 2067 6f65 7320  .# Logging goes 
+000111b0: 746f 2061 6363 6573 7320 6c6f 6720 6669  to access log fi
+000111c0: 6c65 0a20 2020 2020 2020 2020 2020 2020  le.             
+000111d0: 2020 2020 2020 2066 696c 6509 3d20 6163         file.= ac
+000111e0: 6365 7373 2c0a 2020 2020 2020 2020 2020  cess,.          
+000111f0: 2020 2020 2020 2020 2020 696e 7465 7276            interv
+00011200: 616c 093d 2027 6427 2c0a 2020 2020 2020  al.= 'd',.      
+00011210: 2020 2020 2020 2020 2020 2020 2020 6261                ba
+00011220: 636b 7570 7309 3d20 372c 0a20 2020 2020  ckups.= 7,.     
+00011230: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00011240: 2020 2020 2020 2020 2020 2020 2023 2074               # t
+00011250: 6f70 7269 6e74 2064 6f65 7320 7468 6973  oprint does this
+00011260: 2061 7574 6f6d 6174 6963 616c 6c79 2066   automatically f
+00011270: 6f72 2073 7973 2e73 7464 6f75 743b 2073  or sys.stdout; s
+00011280: 7973 2e73 7464 6572 7220 7265 6d61 696e  ys.stderr remain
+00011290: 7320 756e 6368 616e 6765 642e 0a20 2020  s unchanged..   
+000112a0: 2020 2020 2020 2020 2020 2020 2023 2048               # H
+000112b0: 6f77 6576 6572 2c20 7468 6520 6465 6661  owever, the defa
+000112c0: 756c 7420 4c6f 6753 7464 6f75 7420 6973  ult LogStdout is
+000112d0: 206d 6973 7369 6e67 2061 2072 6571 7569   missing a requi
+000112e0: 7265 6420 2e66 6c75 7368 206d 6574 686f  red .flush metho
+000112f0: 642c 2073 6f20 7765 276c 6c20 7365 740a  d, so we'll set.
+00011300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011310: 2320 7468 6973 2075 7020 6d61 6e75 616c  # this up manual
+00011320: 6c79 2069 6e73 7465 6164 0a20 2020 2020  ly instead.     
+00011330: 2020 2020 2020 2020 2020 2073 7973 2e73             sys.s
+00011340: 7464 6f75 7420 3d20 7379 732e 7374 6465  tdout = sys.stde
+00011350: 7272 203d 204c 6f67 5374 646f 7574 2820  rr = LogStdout( 
+00011360: 7365 6c66 2e6c 6f67 6765 722c 206c 6f67  self.logger, log
+00011370: 6769 6e67 2e49 4e46 4f20 290a 2020 2020  ging.INFO ).    
+00011380: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00011390: 2020 2020 2020 2020 2020 2020 2020 7375                su
+000113a0: 7065 7228 204c 6f67 2c20 7365 6c66 2029  per( Log, self )
+000113b0: 2e5f 5f69 6e69 745f 5f28 0a20 2020 2020  .__init__(.     
+000113c0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+000113d0: 7070 6c69 6361 7469 6f6e 2c0a 2020 2020  pplication,.    
+000113e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000113f0: 6c6f 6766 6f72 6d61 7409 3d20 2225 286d  logformat.= "%(m
+00011400: 6573 7361 6765 2973 222c 0a20 2020 2020  essage)s",.     
+00011410: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00011420: 6f67 0909 3d20 5472 7565 2c0a 2020 2020  og..= True,.    
+00011430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011440: 746f 6874 6d6c 093d 2054 7275 652c 0909  tohtml.= True,..
+00011450: 0909 2320 4578 6365 7074 696f 6e73 2067  ..# Exceptions g
+00011460: 656e 6572 6174 6520 4854 4d4c 0a20 2020  enerate HTML.   
+00011470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011480: 2074 6f73 7472 6561 6d09 3d20 5472 7565   tostream.= True
+00011490: 2c09 0909 0923 204c 6f67 6769 6e67 2067  ,....# Logging g
+000114a0: 6f65 7320 746f 2073 7464 6f75 740a 2020  oes to stdout.  
+000114b0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+000114c0: 0a20 2020 2066 756e 6309 0909 3d20 6170  .    func...= ap
+000114d0: 702e 7773 6769 6675 6e63 2820 4c6f 6720  p.wsgifunc( Log 
+000114e0: 290a 2020 2020 6675 6e63 0909 093d 2053  ).    func...= S
+000114f0: 7461 7469 634d 6964 646c 6577 6172 6544  taticMiddlewareD
+00011500: 6972 2820 6675 6e63 2c20 222f 7374 6174  ir( func, "/stat
+00011510: 6963 2f22 2c20 6f73 2e70 6174 682e 6469  ic/", os.path.di
+00011520: 726e 616d 6528 205f 5f66 696c 655f 5f20  rname( __file__ 
+00011530: 2929 0a20 2020 2066 756e 6309 0909 3d20  )).    func...= 
+00011540: 4c6f 674d 6964 646c 6577 6172 6543 4628  LogMiddlewareCF(
+00011550: 2066 756e 6320 2920 2020 2020 2020 2320   func )       # 
+00011560: 7765 622e 6874 7470 7365 7276 6572 2e4c  web.httpserver.L
+00011570: 6f67 4d69 6464 6c65 7761 7265 2820 6170  ogMiddleware( ap
+00011580: 7020 290a 0a20 2020 2023 2077 6562 7079  p )..    # webpy
+00011590: 2e73 6572 7665 7209 093d 2077 6562 2e68  .server..= web.h
+000115a0: 7474 7073 6572 7665 722e 5753 4749 5365  ttpserver.WSGISe
+000115b0: 7276 6572 2820 636f 6e66 6967 5b27 6164  rver( config['ad
+000115c0: 6472 6573 7327 5d2c 2061 7070 2029 0a0a  dress'], app )..
+000115d0: 2020 2020 2320 5468 6973 2069 7320 6120      # This is a 
+000115e0: 4368 6572 7279 5079 2028 6368 6572 6f6f  CherryPy (cheroo
+000115f0: 7429 2053 6572 7665 722e 2020 5765 2068  t) Server.  We h
+00011600: 6176 6520 746f 2069 6e74 6572 6365 7074  ave to intercept
+00011610: 202e 7365 7276 6528 292c 2074 6f20 7072   .serve(), to pr
+00011620: 696e 7420 7468 6520 6163 7475 616c 6c79  int the actually
+00011630: 0a20 2020 2023 2062 6f75 6e64 2077 6562  .    # bound web
+00011640: 2073 6572 7665 7220 6164 6472 6573 7320   server address 
+00011650: 2865 672e 2069 6620 7573 696e 6720 6120  (eg. if using a 
+00011660: 6479 6e61 6d69 6361 6c6c 7920 616c 6c6f  dynamically allo
+00011670: 6361 7465 6420 706f 7274 292e 2020 5468  cated port).  Th
+00011680: 6973 2077 696c 6c20 6265 2072 6564 6972  is will be redir
+00011690: 6563 7465 640a 2020 2020 2320 746f 2074  ected.    # to t
+000116a0: 6865 2061 6363 6573 7320 6c6f 6766 696c  he access logfil
+000116b0: 652c 2075 6e6c 6573 7320 6469 7361 626c  e, unless disabl
+000116c0: 6564 2076 6961 202d 2d6e 6f2d 6163 6365  ed via --no-acce
+000116d0: 7373 2e20 2041 6c73 6f2c 2074 6869 7320  ss.  Also, this 
+000116e0: 636c 6173 7320 7765 6972 646c 7920 6361  class weirdly ca
+000116f0: 7074 7572 6573 2063 6f6e 6669 672c 2073  ptures config, s
+00011700: 6f20 7765 2063 616e 2075 7064 6174 650a  o we can update.
+00011710: 2020 2020 6672 6f6d 2063 6865 726f 6f74      from cheroot
+00011720: 2069 6d70 6f72 7420 7773 6769 0a0a 2020   import wsgi..  
+00011730: 2020 636c 6173 7320 5365 7276 6572 2820    class Server( 
+00011740: 7773 6769 2e53 6572 7665 722c 206f 626a  wsgi.Server, obj
+00011750: 6563 7420 293a 0a20 2020 2020 2020 2064  ect ):.        d
+00011760: 6566 2073 6572 7665 2820 7365 6c66 2029  ef serve( self )
+00011770: 3a0a 2020 2020 2020 2020 2020 2020 736f  :.            so
+00011780: 636b 6e61 6d65 0909 3d20 7365 6c66 2e73  ckname..= self.s
+00011790: 6f63 6b65 742e 6765 7473 6f63 6b6e 616d  ocket.getsocknam
+000117a0: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
+000117b0: 7072 696e 7428 2022 5765 6220 496e 7465  print( "Web Inte
+000117c0: 7266 6163 6520 5443 5020 6164 6472 6573  rface TCP addres
+000117d0: 7320 3d20 7b73 6f63 6b6e 616d 6521 727d  s = {sockname!r}
+000117e0: 222e 666f 726d 6174 2820 736f 636b 6e61  ".format( sockna
+000117f0: 6d65 3d73 6f63 6b6e 616d 6520 2929 0a20  me=sockname )). 
+00011800: 2020 2020 2020 2020 2020 2073 7973 2e73             sys.s
+00011810: 7464 6f75 742e 666c 7573 6828 290a 2020  tdout.flush().  
+00011820: 2020 2020 2020 2020 2020 636f 6e66 6967            config
+00011830: 5b27 636f 6e74 726f 6c27 5d5b 2761 6464  ['control']['add
+00011840: 7265 7373 275d 203d 2073 6f63 6b6e 616d  ress'] = socknam
+00011850: 650a 2020 2020 2020 2020 2020 2020 7375  e.            su
+00011860: 7065 7228 2053 6572 7665 722c 2073 656c  per( Server, sel
+00011870: 6620 292e 7365 7276 6528 290a 0a20 2020  f ).serve()..   
+00011880: 2023 2046 696e 616c 6c79 2c20 6d61 6b65   # Finally, make
+00011890: 2074 6865 2053 6572 7665 7220 6176 6169   the Server avai
+000118a0: 6c61 626c 6520 6f6e 2074 6865 2066 756e  lable on the fun
+000118b0: 6374 696f 6e27 7320 7765 6270 792e 7365  ction's webpy.se
+000118c0: 7276 6572 2066 6f72 2065 7874 6572 6e61  rver for externa
+000118d0: 6c20 6163 6365 7373 0a20 2020 2077 6562  l access.    web
+000118e0: 7079 2e73 6572 7665 7209 093d 2053 6572  py.server..= Ser
+000118f0: 7665 7228 2063 6f6e 6669 675b 2761 6464  ver( config['add
+00011900: 7265 7373 275d 2c20 6675 6e63 2c20 7365  ress'], func, se
+00011910: 7276 6572 5f6e 616d 653d 226c 6f63 616c  rver_name="local
+00011920: 686f 7374 2220 290a 2020 2020 7765 6270  host" ).    webp
+00011930: 792e 7365 7276 6572 2e6e 6f64 656c 6179  y.server.nodelay
+00011940: 093d 2054 7275 650a 0a20 2020 2074 7279  .= True..    try
+00011950: 3a0a 2020 2020 2020 2020 6c6f 672e 7761  :.        log.wa
+00011960: 726e 696e 6728 2022 5765 6220 496e 7465  rning( "Web Inte
+00011970: 7266 6163 6520 7374 6172 7469 6e67 2220  rface starting" 
+00011980: 290a 2020 2020 2020 2020 7765 6270 792e  ).        webpy.
+00011990: 7365 7276 6572 2e73 7461 7274 2829 0a20  server.start(). 
+000119a0: 2020 2065 7863 6570 7420 284b 6579 626f     except (Keybo
+000119b0: 6172 6449 6e74 6572 7275 7074 2c20 5379  ardInterrupt, Sy
+000119c0: 7374 656d 4578 6974 2920 6173 2065 7863  stemExit) as exc
+000119d0: 3a0a 2020 2020 2020 2020 6c6f 6767 696e  :.        loggin
+000119e0: 672e 7761 726e 696e 6728 2022 5765 6220  g.warning( "Web 
+000119f0: 496e 7465 7266 6163 6520 5468 7265 6164  Interface Thread
+00011a00: 2075 6e63 6f6e 7472 6f6c 6c65 6420 7368   uncontrolled sh
+00011a10: 7574 646f 776e 3a20 2573 222c 2065 7863  utdown: %s", exc
+00011a20: 2029 0a20 2020 2065 7863 6570 7420 4578   ).    except Ex
+00011a30: 6365 7074 696f 6e20 6173 2065 7863 3a0a  ception as exc:.
+00011a40: 2020 2020 2020 2020 6c6f 6767 696e 672e          logging.
+00011a50: 7761 726e 696e 6728 2022 5765 6220 496e  warning( "Web In
+00011a60: 7465 7266 6163 6520 5468 7265 6164 2065  terface Thread e
+00011a70: 7863 6570 7469 6f6e 2073 6875 7464 6f77  xception shutdow
+00011a80: 6e3a 2025 7322 2c20 6578 6320 290a 2020  n: %s", exc ).  
+00011a90: 2020 6669 6e61 6c6c 793a 0a20 2020 2020    finally:.     
+00011aa0: 2020 206c 6f67 6769 6e67 2e69 6e66 6f28     logging.info(
+00011ab0: 2022 5765 6220 496e 7465 7266 6163 6520   "Web Interface 
+00011ac0: 5468 7265 6164 2073 746f 7070 696e 672e  Thread stopping.
+00011ad0: 2e2e 2220 290a 2020 2020 2020 2020 7472  .." ).        tr
+00011ae0: 793a 0a20 2020 2020 2020 2020 2020 2077  y:.            w
+00011af0: 6562 7079 2e73 6572 7665 722e 7374 6f70  ebpy.server.stop
+00011b00: 2829 0a20 2020 2020 2020 2065 7863 6570  ().        excep
+00011b10: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
+00011b20: 7863 3a0a 2020 2020 2020 2020 2020 2020  xc:.            
+00011b30: 6c6f 6767 696e 672e 7761 726e 696e 6728  logging.warning(
+00011b40: 2022 5765 6220 496e 7465 7266 6163 6520   "Web Interface 
+00011b50: 5468 7265 6164 2073 746f 7020 6661 696c  Thread stop fail
+00011b60: 7572 653a 2025 7322 2c20 6578 6320 290a  ure: %s", exc ).
+00011b70: 2020 2020 2020 2020 7765 6270 792e 7365          webpy.se
+00011b80: 7276 6572 0909 3d20 4e6f 6e65 0a20 2020  rver..= None.   
+00011b90: 2020 2020 206c 6f67 6769 6e67 2e77 6172       logging.war
+00011ba0: 6e69 6e67 2820 2257 6562 2049 6e74 6572  ning( "Web Inter
+00011bb0: 6661 6365 2054 6872 6561 6420 6578 6974  face Thread exit
+00011bc0: 696e 6722 2029 0a0a 0a23 2054 6f20 7374  ing" )...# To st
+00011bd0: 6f70 2074 6865 2073 6572 7665 7220 6578  op the server ex
+00011be0: 7465 726e 616c 6c79 2c20 6869 7420 7765  ternally, hit we
+00011bf0: 6270 792e 7365 7276 6572 2e73 746f 700a  bpy.server.stop.
+00011c00: 7765 6270 792e 7365 7276 6572 0909 093d  webpy.server...=
+00011c10: 204e 6f6e 650a 0a0a 6465 6620 7478 7467   None...def txtg
+00011c20: 7569 2820 636f 6e66 6967 2029 3a0a 2020  ui( config ):.  
+00011c30: 2020 2222 2252 756e 2063 7572 7365 7320    """Run curses 
+00011c40: 5549 2c20 6361 7463 6869 6e67 2061 6c6c  UI, catching all
+00011c50: 2065 7863 6570 7469 6f6e 732e 2020 5265   exceptions.  Re
+00011c60: 7475 726e 7320 5472 7565 206f 6e20 6661  turns True on fa
+00011c70: 696c 7572 652e 2222 220a 2020 2020 6661  ilure.""".    fa
+00011c80: 696c 7572 6509 0909 3d20 4e6f 6e65 0a20  ilure...= None. 
+00011c90: 2020 2074 7279 3a20 2020 2020 2020 2023     try:        #
+00011ca0: 2049 6e69 7469 616c 697a 6520 6375 7273   Initialize curs
+00011cb0: 6573 0a20 2020 2020 2020 2073 7464 7363  es.        stdsc
+00011cc0: 7209 0909 3d20 6375 7273 6573 2e69 6e69  r...= curses.ini
+00011cd0: 7473 6372 2829 0a20 2020 2020 2020 2063  tscr().        c
+00011ce0: 7572 7365 732e 6e6f 6563 686f 2829 0a20  urses.noecho(). 
+00011cf0: 2020 2020 2020 2063 7572 7365 732e 6362         curses.cb
+00011d00: 7265 616b 2829 0a20 2020 2020 2020 2063  reak().        c
+00011d10: 7572 7365 732e 6861 6c66 6465 6c61 7928  urses.halfdelay(
+00011d20: 2031 2029 0a20 2020 2020 2020 2073 7464   1 ).        std
+00011d30: 7363 722e 6b65 7970 6164 2820 3120 290a  scr.keypad( 1 ).
+00011d40: 0a20 2020 2020 2020 2074 7874 2820 7374  .        txt( st
+00011d50: 6473 6372 2c20 636f 6e66 6967 2029 2020  dscr, config )  
+00011d60: 2020 2020 2020 2020 2020 2020 2023 2045               # E
+00011d70: 6e74 6572 2074 6865 2043 7572 7365 7320  nter the Curses 
+00011d80: 6d61 696e 6c6f 6f70 0a20 2020 2065 7863  mainloop.    exc
+00011d90: 6570 7420 4578 6365 7074 696f 6e3a 0a20  ept Exception:. 
+00011da0: 2020 2020 2020 2066 6169 6c75 7265 0909         failure..
+00011db0: 093d 2074 7261 6365 6261 636b 2e66 6f72  .= traceback.for
+00011dc0: 6d61 745f 6578 6328 290a 2020 2020 6669  mat_exc().    fi
+00011dd0: 6e61 6c6c 793a 0a20 2020 2020 2020 2063  nally:.        c
+00011de0: 6f6e 6669 672e 7365 7464 6566 6175 6c74  onfig.setdefault
+00011df0: 2820 2763 6f6e 7472 6f6c 272c 207b 7d20  ( 'control', {} 
+00011e00: 295b 2764 6f6e 6527 5d20 3d20 5472 7565  )['done'] = True
+00011e10: 0a20 2020 2020 2020 2073 7464 7363 722e  .        stdscr.
+00011e20: 6b65 7970 6164 2830 290a 2020 2020 2020  keypad(0).      
+00011e30: 2020 6375 7273 6573 2e65 6368 6f28 290a    curses.echo().
+00011e40: 2020 2020 2020 2020 6375 7273 6573 2e6e          curses.n
+00011e50: 6f63 6272 6561 6b28 290a 2020 2020 2020  ocbreak().      
+00011e60: 2020 6375 7273 6573 2e65 6e64 7769 6e28    curses.endwin(
+00011e70: 290a 2020 2020 2020 2020 7469 6d65 2e73  ).        time.s
+00011e80: 6c65 6570 282e 3235 290a 2020 2020 6966  leep(.25).    if
+00011e90: 2066 6169 6c75 7265 3a0a 2020 2020 2020   failure:.      
+00011ea0: 2020 6c6f 6767 696e 672e 6572 726f 7228    logging.error(
+00011eb0: 2022 4375 7273 6573 2047 5549 2045 7863   "Curses GUI Exc
+00011ec0: 6570 7469 6f6e 3a20 2573 222c 2066 6169  eption: %s", fai
+00011ed0: 6c75 7265 2029 0a20 2020 2020 2020 2072  lure ).        r
+00011ee0: 6574 7572 6e20 5472 7565 0a20 2020 2072  eturn True.    r
+00011ef0: 6574 7572 6e20 4661 6c73 650a 0a0a 6465  eturn False...de
+00011f00: 6620 6374 6c6c 6f6f 7028 2062 6567 2c20  f ctlloop( beg, 
+00011f10: 636e 6620 293a 0a20 2020 2022 2222 4578  cnf ):.    """Ex
+00011f20: 6563 7574 6520 6f6e 6520 6c6f 6f70 206f  ecute one loop o
+00011f30: 6620 7468 6520 636f 6e74 726f 6c20 7379  f the control sy
+00011f40: 7374 656d 2222 220a 2020 2020 7061 7373  stem""".    pass
+00011f50: 0a0a 0a64 6566 206d 6169 6e28 2061 7267  ...def main( arg
+00011f60: 763d 4e6f 6e65 2c20 2a2a 6c69 6365 6e73  v=None, **licens
+00011f70: 696e 675f 6b77 6473 2029 3a0a 2020 2020  ing_kwds ):.    
+00011f80: 2222 2250 6173 7320 7468 6520 6465 7369  """Pass the desi
+00011f90: 7265 6420 6172 6776 2028 6578 636c 7564  red argv (exclud
+00011fa0: 696e 6720 7468 6520 7072 6f67 7261 6d20  ing the program 
+00011fb0: 6e61 6d65 2069 6e20 7379 732e 6172 675b  name in sys.arg[
+00011fc0: 305d 3b20 7479 7069 6361 6c6c 7920 7061  0]; typically pa
+00011fd0: 7373 2061 7267 763d 4e6f 6e65 2c20 7768  ss argv=None, wh
+00011fe0: 6963 680a 2020 2020 6973 2065 7175 6976  ich.    is equiv
+00011ff0: 616c 656e 7420 746f 2061 7267 763d 7379  alent to argv=sy
+00012000: 732e 6172 6776 5b31 3a5d 2c20 7468 6520  s.argv[1:], the 
+00012010: 6465 6661 756c 7420 666f 7220 6172 6770  default for argp
+00012020: 6172 7365 2e20 2052 6571 7569 7265 7320  arse.  Requires 
+00012030: 6174 206c 6561 7374 206f 6e65 2074 6167  at least one tag
+00012040: 2074 6f20 6265 0a20 2020 2064 6566 696e   to be.    defin
+00012050: 6564 2e0a 2020 2020 2222 220a 0a20 2020  ed..    """..   
+00012060: 2061 7009 0909 093d 2061 7267 7061 7273   ap....= argpars
+00012070: 652e 4172 6775 6d65 6e74 5061 7273 6572  e.ArgumentParser
+00012080: 280a 2020 2020 2020 2020 6465 7363 7269  (.        descri
+00012090: 7074 696f 6e09 3d20 2241 2043 7070 706f  ption.= "A Cpppo
+000120a0: 2043 7279 7074 6f20 4c69 6365 6e73 696e   Crypto Licensin
+000120b0: 6720 5365 7276 6572 222c 0a20 2020 2020  g Server",.     
+000120c0: 2020 2066 6f72 6d61 7474 6572 5f63 6c61     formatter_cla
+000120d0: 7373 203d 2061 7267 7061 7273 652e 5261  ss = argparse.Ra
+000120e0: 7744 6573 6372 6970 7469 6f6e 4865 6c70  wDescriptionHelp
+000120f0: 466f 726d 6174 7465 722c 0a20 2020 2020  Formatter,.     
+00012100: 2020 2065 7069 6c6f 6709 093d 2022 2222     epilog..= """
+00012110: 5c0a 496d 706c 656d 656e 7473 2045 6432  \.Implements Ed2
+00012120: 3535 3139 2d73 6967 6e65 6420 6372 7970  5519-signed cryp
+00012130: 746f 6772 6170 6869 6320 6c69 6365 6e73  tographic licens
+00012140: 696e 6720 7765 6220 7365 7276 6963 6520  ing web service 
+00012150: 616e 6420 4150 492e 0a0a 4973 7375 6573  and API...Issues
+00012160: 206c 6963 656e 7365 2873 2920 666f 7220   license(s) for 
+00012170: 7072 6f64 7563 7473 2061 6e64 2063 6170  products and cap
+00012180: 6162 696c 6974 6965 7320 6176 6169 6c61  abilities availa
+00012190: 626c 6520 746f 2074 6865 2063 6c69 656e  ble to the clien
+000121a0: 742c 2077 6865 7265 2065 6974 6865 720a  t, where either.
+000121b0: 0a20 2041 2920 7468 6520 7365 7276 6572  .  A) the server
+000121c0: 2068 6173 2063 7265 6465 6e74 6961 6c73   has credentials
+000121d0: 2069 6e64 6963 6174 696e 6720 6f77 6e65   indicating owne
+000121e0: 7273 6869 7020 6f66 2074 6865 204c 6963  rship of the Lic
+000121f0: 656e 7365 732c 2061 6e64 2068 656e 6365  enses, and hence
+00012200: 0a20 2020 2020 6175 7468 6f72 6974 7920  .     authority 
+00012210: 746f 2073 7562 2d6c 6963 656e 7365 2074  to sub-license t
+00012220: 6865 6d2c 206f 720a 0a20 2042 2920 7468  hem, or..  B) th
+00012230: 6520 4c69 6365 6e73 6520 6974 7365 6c66  e License itself
+00012240: 2067 7261 6e74 7320 6175 7468 6f72 6974   grants authorit
+00012250: 7920 746f 2062 6520 7375 622d 6c69 6365  y to be sub-lice
+00012260: 6e73 6564 2074 6f20 616e 7920 4167 656e  nsed to any Agen
+00012270: 740a 2020 2020 2061 736b 696e 6720 666f  t.     asking fo
+00012280: 7220 6120 4c69 6365 6e73 650a 0a50 726f  r a License..Pro
+00012290: 6475 6365 7320 696e 766f 6963 6573 2066  duces invoices f
+000122a0: 6f72 2065 6163 6820 7472 616e 7361 6374  or each transact
+000122b0: 696f 6e0a 0a50 6572 666f 726d 616e 6365  ion..Performance
+000122c0: 2062 656e 6566 6974 7320 6772 6561 746c   benefits greatl
+000122d0: 7920 6672 6f6d 2069 6e73 7461 6c6c 6174  y from installat
+000122e0: 696f 6e20 6f66 2028 6f70 7469 6f6e 616c  ion of (optional
+000122f0: 2920 6564 3235 3531 396c 6c20 7061 636b  ) ed25519ll pack
+00012300: 6167 653a 0a0a 2020 2020 7079 7468 6f6e  age:..    python
+00012310: 3320 2d6d 2070 6970 2069 6e73 7461 6c6c  3 -m pip install
+00012320: 2065 6432 3535 3139 6c6c 0a22 2222 0a20   ed25519ll.""". 
+00012330: 2020 2029 0a20 2020 2061 702e 6164 645f     ).    ap.add_
+00012340: 6172 6775 6d65 6e74 2820 272d 7627 2c20  argument( '-v', 
+00012350: 272d 2d76 6572 626f 7365 272c 2061 6374  '--verbose', act
+00012360: 696f 6e3d 2263 6f75 6e74 222c 0a20 2020  ion="count",.   
+00012370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012380: 2020 6465 6661 756c 743d 302c 0a20 2020    default=0,.   
+00012390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000123a0: 2020 6865 6c70 3d22 4469 7370 6c61 7920    help="Display 
+000123b0: 6c6f 6767 696e 6720 696e 666f 726d 6174  logging informat
+000123c0: 696f 6e2e 2220 290a 2020 2020 6170 2e61  ion." ).    ap.a
+000123d0: 6464 5f61 7267 756d 656e 7428 2027 2d71  dd_argument( '-q
+000123e0: 272c 2027 2d2d 7175 6965 7427 2c20 6163  ', '--quiet', ac
+000123f0: 7469 6f6e 3d22 636f 756e 7422 2c0a 2020  tion="count",.  
+00012400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012410: 2020 2064 6566 6175 6c74 3d30 2c0a 2020     default=0,.  
+00012420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012430: 2020 2068 656c 703d 2252 6564 7563 6520     help="Reduce 
+00012440: 6c6f 6767 696e 6720 6f75 7470 7574 2e22  logging output."
+00012450: 2029 0a20 2020 2061 702e 6164 645f 6172   ).    ap.add_ar
+00012460: 6775 6d65 6e74 2820 272d 7727 2c20 272d  gument( '-w', '-
+00012470: 2d77 6562 272c 0a20 2020 2020 2020 2020  -web',.         
+00012480: 2020 2020 2020 2020 2020 2020 6465 6661              defa
+00012490: 756c 743d 2230 2e30 2e30 2e30 3a38 3030  ult="0.0.0.0:800
+000124a0: 3022 2c0a 2020 2020 2020 2020 2020 2020  0",.            
+000124b0: 2020 2020 2020 2020 2068 656c 703d 2765           help='e
+000124c0: 6e61 626c 6520 7765 6220 7365 7276 6572  nable web server
+000124d0: 206f 6e20 696e 7465 7266 6163 6520 2864   on interface (d
+000124e0: 6566 6175 6c74 3a20 302e 302e 302e 303a  efault: 0.0.0.0:
+000124f0: 3830 3030 2927 2029 0a20 2020 2061 702e  8000)' ).    ap.
+00012500: 6164 645f 6172 6775 6d65 6e74 2820 272d  add_argument( '-
+00012510: 2d6e 6f2d 7765 6227 2c20 6465 7374 3d27  -no-web', dest='
+00012520: 7765 6227 2c0a 2020 2020 2020 2020 2020  web',.          
+00012530: 2020 2020 2020 2020 2020 2061 6374 696f             actio
+00012540: 6e3d 2273 746f 7265 5f66 616c 7365 222c  n="store_false",
+00012550: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012560: 2020 2020 2020 6865 6c70 3d27 4469 7361        help='Disa
+00012570: 626c 6520 7765 6220 696e 7465 7266 6163  ble web interfac
+00012580: 6520 616e 6420 6163 6365 7373 206c 6f67  e and access log
+00012590: 2066 696c 6520 2864 6566 6175 6c74 3a20   file (default: 
+000125a0: 4661 6c73 6529 2720 290a 2020 2020 6170  False)' ).    ap
+000125b0: 2e61 6464 5f61 7267 756d 656e 7428 2027  .add_argument( '
+000125c0: 2d2d 6163 6365 7373 272c 0a20 2020 2020  --access',.     
+000125d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000125e0: 6465 6661 756c 743d 4143 4346 494c 452c  default=ACCFILE,
+000125f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012600: 2020 2020 2020 6865 6c70 3d22 4c6f 6720        help="Log 
+00012610: 616c 6c20 7765 6220 7365 7276 6572 2061  all web server a
+00012620: 6363 6573 7320 746f 206c 6f67 2066 696c  ccess to log fil
+00012630: 6520 2864 6566 6175 6c74 3a20 7b41 4343  e (default: {ACC
+00012640: 4649 4c45 7d22 2e66 6f72 6d61 7428 0a20  FILE}".format(. 
+00012650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012660: 2020 2020 2020 2020 4143 4346 494c 453d          ACCFILE=
+00012670: 4143 4346 494c 4520 2929 0a20 2020 2061  ACCFILE )).    a
+00012680: 702e 6164 645f 6172 6775 6d65 6e74 2820  p.add_argument( 
+00012690: 272d 2d6e 6f2d 6163 6365 7373 272c 2064  '--no-access', d
+000126a0: 6573 743d 2761 6363 6573 7327 2c0a 2020  est='access',.  
+000126b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000126c0: 2020 2063 6f6e 7374 3d4e 6f6e 652c 2061     const=None, a
+000126d0: 6374 696f 6e3d 2273 746f 7265 5f63 6f6e  ction="store_con
+000126e0: 7374 222c 0a20 2020 2020 2020 2020 2020  st",.           
+000126f0: 2020 2020 2020 2020 2020 6865 6c70 3d27            help='
+00012700: 4469 7361 626c 6520 7765 6220 7365 7276  Disable web serv
+00012710: 6572 2061 6363 6573 7320 6c6f 6720 6669  er access log fi
+00012720: 6c65 2c20 696e 636c 7564 696e 6720 7374  le, including st
+00012730: 646f 7574 2f73 7464 6572 7220 7265 6469  dout/stderr redi
+00012740: 7265 6374 696f 6e27 2029 0a20 2020 2061  rection' ).    a
+00012750: 702e 6164 645f 6172 6775 6d65 6e74 2820  p.add_argument( 
+00012760: 272d 2d6e 6f2d 6775 6927 2c20 6465 7374  '--no-gui', dest
+00012770: 3d27 6775 6927 2c0a 2020 2020 2020 2020  ='gui',.        
+00012780: 2020 2020 2020 2020 2020 2020 2064 6566               def
+00012790: 6175 6c74 3d54 7275 652c 2061 6374 696f  ault=True, actio
+000127a0: 6e3d 2273 746f 7265 5f66 616c 7365 222c  n="store_false",
+000127b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000127c0: 2020 2020 2020 6865 6c70 3d27 4469 7361        help='Disa
+000127d0: 626c 6520 4375 7273 6573 2047 5549 2069  ble Curses GUI i
+000127e0: 6e74 6572 6661 6365 2028 6465 6661 756c  nterface (defaul
+000127f0: 743a 2046 616c 7365 2927 2029 0a20 2020  t: False)' ).   
+00012800: 2061 702e 6164 645f 6172 6775 6d65 6e74   ap.add_argument
+00012810: 2820 272d 6327 2c20 272d 2d63 6f6e 6669  ( '-c', '--confi
+00012820: 6727 2c0a 2020 2020 2020 2020 2020 2020  g',.            
+00012830: 2020 2020 2020 2020 2061 6374 696f 6e3d           action=
+00012840: 2761 7070 656e 6427 2c0a 2020 2020 2020  'append',.      
+00012850: 2020 2020 2020 2020 2020 2020 2020 2068                 h
+00012860: 656c 703d 2241 6464 2061 6e6f 7468 6572  elp="Add another
+00012870: 2028 6869 6768 6572 2070 7269 6f72 6974   (higher priorit
+00012880: 7929 2063 6f6e 6669 6720 6669 6c65 2070  y) config file p
+00012890: 6174 682e 2220 290a 2020 2020 6170 2e61  ath." ).    ap.a
+000128a0: 6464 5f61 7267 756d 656e 7428 2027 2d6c  dd_argument( '-l
+000128b0: 272c 2027 2d2d 6c6f 6727 2c0a 2020 2020  ', '--log',.    
+000128c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000128d0: 2064 6566 6175 6c74 3d4e 6f6e 652c 0a20   default=None,. 
+000128e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000128f0: 2020 2020 6865 6c70 3d22 4c6f 6720 6669      help="Log fi
+00012900: 6c65 2c20 6966 2064 6573 6972 6564 2028  le, if desired (
+00012910: 6465 6661 756c 742c 2069 6620 7465 7874  default, if text
+00012920: 2067 7569 3a20 7b4c 4f47 4649 4c45 7d29   gui: {LOGFILE})
+00012930: 222e 666f 726d 6174 2820 4c4f 4746 494c  ".format( LOGFIL
+00012940: 453d 4c4f 4746 494c 4520 2929 0a20 2020  E=LOGFILE )).   
+00012950: 2061 702e 6164 645f 6172 6775 6d65 6e74   ap.add_argument
+00012960: 2820 272d 2d70 726f 6669 6c65 272c 0a20  ( '--profile',. 
+00012970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012980: 2020 2020 6465 6661 756c 743d 4e6f 6e65      default=None
+00012990: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000129a0: 2020 2020 2020 2068 656c 703d 2250 726f         help="Pro
+000129b0: 6669 6c65 2074 6f20 7374 6465 7272 2028  file to stderr (
+000129c0: 6f6e 6c79 2c20 6966 2027 2d27 2073 7065  only, if '-' spe
+000129d0: 6369 6669 6564 292c 206f 7074 696f 6e61  cified), optiona
+000129e0: 6c6c 7920 7361 7669 6e67 2064 6174 6120  lly saving data 
+000129f0: 746f 2061 2066 696c 6520 2864 6566 6175  to a file (defau
+00012a00: 6c74 3a20 4e6f 6e65 2922 2029 0a20 2020  lt: None)" ).   
+00012a10: 2061 702e 6164 645f 6172 6775 6d65 6e74   ap.add_argument
+00012a20: 2820 272d 2d63 6c69 656e 7427 2c0a 2020  ( '--client',.  
+00012a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012a40: 2020 2064 6566 6175 6c74 3d4e 6f6e 652c     default=None,
+00012a50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012a60: 2020 2020 2020 6865 6c70 3d22 5468 6973        help="This
+00012a70: 207b 4449 5354 5249 4255 5449 4f4e 7d73   {DISTRIBUTION}s
+00012a80: 6572 7665 7227 7320 636c 6965 6e74 206c  erver's client l
+00012a90: 6963 656e 7365 6527 7320 636f 6d70 616e  icensee's compan
+00012aa0: 7920 6e61 6d65 222e 666f 726d 6174 280a  y name".format(.
+00012ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012ac0: 2020 2020 2020 2020 2044 4953 5452 4942           DISTRIB
+00012ad0: 5554 494f 4e3d 6c69 6365 6e73 696e 672e  UTION=licensing.
+00012ae0: 4449 5354 5249 4255 5449 4f4e 2029 290a  DISTRIBUTION )).
+00012af0: 2020 2020 6170 2e61 6464 5f61 7267 756d      ap.add_argum
+00012b00: 656e 7428 2027 2d2d 646f 6d61 696e 272c  ent( '--domain',
+00012b10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012b20: 2020 2020 2020 6465 6661 756c 743d 4e6f        default=No
+00012b30: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
+00012b40: 2020 2020 2020 2020 2068 656c 703d 2254           help="T
+00012b50: 6869 7320 7b44 4953 5452 4942 5554 494f  his {DISTRIBUTIO
+00012b60: 4e7d 2073 6572 7665 7227 7320 636c 6965  N} server's clie
+00012b70: 6e74 206c 6963 656e 7365 6527 7320 646f  nt licensee's do
+00012b80: 6d61 696e 3b20 6361 6e20 6265 2075 7365  main; can be use
+00012b90: 6420 746f 2067 6574 2070 7562 6c69 6320  d to get public 
+00012ba0: 6b65 7920 7669 6120 444b 494d 222e 666f  key via DKIM".fo
+00012bb0: 726d 6174 280a 2020 2020 2020 2020 2020  rmat(.          
+00012bc0: 2020 2020 2020 2020 2020 2020 2020 2044                 D
+00012bd0: 4953 5452 4942 5554 494f 4e3d 6c69 6365  ISTRIBUTION=lice
+00012be0: 6e73 696e 672e 4449 5354 5249 4255 5449  nsing.DISTRIBUTI
+00012bf0: 4f4e 2029 290a 2020 2020 6170 2e61 6464  ON )).    ap.add
+00012c00: 5f61 7267 756d 656e 7428 2027 2d2d 7072  _argument( '--pr
+00012c10: 6f64 7563 7427 2c0a 2020 2020 2020 2020  oduct',.        
+00012c20: 2020 2020 2020 2020 2020 2020 2064 6566               def
+00012c30: 6175 6c74 3d6c 6963 656e 7369 6e67 2e50  ault=licensing.P
+00012c40: 524f 4455 4354 5f53 4552 5645 522c 0a20  RODUCT_SERVER,. 
+00012c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c60: 2020 2020 6865 6c70 3d22 5468 6973 207b      help="This {
+00012c70: 4449 5354 5249 4255 5449 4f4e 7d20 7365  DISTRIBUTION} se
+00012c80: 7276 6572 2773 2063 6c69 656e 7420 6c69  rver's client li
+00012c90: 6365 6e73 6565 2773 2070 726f 6475 6374  censee's product
+00012ca0: 206e 616d 6520 2869 6620 616e 793b 2064   name (if any; d
+00012cb0: 6566 6175 6c74 3a20 7b50 524f 4455 4354  efault: {PRODUCT
+00012cc0: 7d29 222e 666f 726d 6174 280a 2020 2020  })".format(.    
+00012cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012ce0: 2020 2020 2044 4953 5452 4942 5554 494f       DISTRIBUTIO
+00012cf0: 4e3d 6c69 6365 6e73 696e 672e 4449 5354  N=licensing.DIST
+00012d00: 5249 4255 5449 4f4e 2c20 5052 4f44 5543  RIBUTION, PRODUC
+00012d10: 543d 6c69 6365 6e73 696e 672e 5052 4f44  T=licensing.PROD
+00012d20: 5543 545f 5345 5256 4552 2029 290a 2020  UCT_SERVER )).  
+00012d30: 2020 6170 2e61 6464 5f61 7267 756d 656e    ap.add_argumen
+00012d40: 7428 2027 2d55 272c 2027 2d2d 7573 6572  t( '-U', '--user
+00012d50: 6e61 6d65 272c 0a20 2020 2020 2020 2020  name',.         
+00012d60: 2020 2020 2020 2020 2020 2020 6465 6661              defa
+00012d70: 756c 743d 4e6f 6e65 2c0a 2020 2020 2020  ult=None,.      
+00012d80: 2020 2020 2020 2020 2020 2020 2020 2068                 h
+00012d90: 656c 703d 227b 4449 5354 5249 4255 5449  elp="{DISTRIBUTI
+00012da0: 4f4e 7d20 4167 656e 7420 6372 6564 656e  ON} Agent creden
+00012db0: 7469 616c 7320 7573 6572 6e61 6d65 3b20  tials username; 
+00012dc0: 6c69 6b65 6c79 2061 6e20 656d 6169 6c20  likely an email 
+00012dd0: 6164 6472 6573 7320 2827 2d27 2074 6f20  address ('-' to 
+00012de0: 7265 6164 2066 726f 6d20 696e 7075 7429  read from input)
+00012df0: 222e 666f 726d 6174 280a 2020 2020 2020  ".format(.      
+00012e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012e10: 2020 2044 4953 5452 4942 5554 494f 4e3d     DISTRIBUTION=
+00012e20: 6c69 6365 6e73 696e 672e 4449 5354 5249  licensing.DISTRI
+00012e30: 4255 5449 4f4e 2029 290a 2020 2020 6170  BUTION )).    ap
+00012e40: 2e61 6464 5f61 7267 756d 656e 7428 2027  .add_argument( '
+00012e50: 2d50 272c 2027 2d2d 7061 7373 776f 7264  -P', '--password
+00012e60: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
+00012e70: 2020 2020 2020 2020 6465 6661 756c 743d          default=
+00012e80: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
+00012e90: 2020 2020 2020 2020 2020 2068 656c 703d             help=
+00012ea0: 227b 4449 5354 5249 4255 5449 4f4e 7d20  "{DISTRIBUTION} 
+00012eb0: 4167 656e 7420 6372 6564 656e 7469 616c  Agent credential
+00012ec0: 7320 7061 7373 776f 7264 2028 272d 2720  s password ('-' 
+00012ed0: 746f 2072 6561 6420 6672 6f6d 2069 6e70  to read from inp
+00012ee0: 7574 2922 2e66 6f72 6d61 7428 0a20 2020  ut)".format(.   
+00012ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012f00: 2020 2020 2020 4449 5354 5249 4255 5449        DISTRIBUTI
+00012f10: 4f4e 3d6c 6963 656e 7369 6e67 2e44 4953  ON=licensing.DIS
+00012f20: 5452 4942 5554 494f 4e20 2929 0a20 2020  TRIBUTION )).   
+00012f30: 2061 702e 6164 645f 6172 6775 6d65 6e74   ap.add_argument
+00012f40: 2820 272d 5227 2c20 272d 2d72 6567 6973  ( '-R', '--regis
+00012f50: 7465 7227 2c20 6163 7469 6f6e 3d27 7374  ter', action='st
+00012f60: 6f72 655f 7472 7565 272c 0a20 2020 2020  ore_true',.     
+00012f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012f80: 6465 6661 756c 743d 4661 6c73 652c 0a20  default=False,. 
+00012f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012fa0: 2020 2020 6865 6c70 3d22 4966 206e 6563      help="If nec
+00012fb0: 6573 7361 7279 2c20 6372 6561 7465 2061  essary, create a
+00012fc0: 6e64 2073 6176 6520 6120 6e65 7720 636c  nd save a new cl
+00012fd0: 6965 6e74 204b 6579 7061 6972 2220 290a  ient Keypair" ).
+00012fe0: 2020 2020 6170 2e61 6464 5f61 7267 756d      ap.add_argum
+00012ff0: 656e 7428 2027 2d41 272c 2027 2d2d 6163  ent( '-A', '--ac
+00013000: 7175 6972 6527 2c20 6163 7469 6f6e 3d27  quire', action='
+00013010: 7374 6f72 655f 7472 7565 272c 0a20 2020  store_true',.   
+00013020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013030: 2020 6465 6661 756c 743d 4661 6c73 652c    default=False,
+00013040: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013050: 2020 2020 2020 6865 6c70 3d22 4966 206e        help="If n
+00013060: 6f20 4167 656e 7420 4b65 7970 6169 7220  o Agent Keypair 
+00013070: 6f72 204c 6963 656e 7365 2069 7320 6176  or License is av
+00013080: 6169 6c61 626c 652c 2061 7474 656d 7074  ailable, attempt
+00013090: 2074 6f20 6372 6561 7465 2061 6e64 2f6f   to create and/o
+000130a0: 7220 6f62 7461 696e 206f 6e65 3b20 7072  r obtain one; pr
+000130b0: 6f76 6964 6520 2d2d 7573 6572 6e61 6d65  ovide --username
+000130c0: 2f2d 2d70 6173 7377 6f72 6420 746f 2065  /--password to e
+000130d0: 6e63 7279 7074 220a 2020 2020 2020 2020  ncrypt".        
+000130e0: 2020 2020 2020 2020 2020 2020 2022 2c20               ", 
+000130f0: 7468 656e 2075 7365 207b 454e 5655 5345  then use {ENVUSE
+00013100: 524e 414d 457d 2f7b 454e 5650 4153 5357  RNAME}/{ENVPASSW
+00013110: 4f52 447d 2065 6e76 6972 6f6e 6d65 6e74  ORD} environment
+00013120: 2076 6172 7320 746f 2064 6563 7279 7074   vars to decrypt
+00013130: 222e 666f 726d 6174 280a 2020 2020 2020  ".format(.      
+00013140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013150: 2020 2045 4e56 5553 4552 4e41 4d45 3d6c     ENVUSERNAME=l
+00013160: 6963 656e 7369 6e67 2e45 4e56 5553 4552  icensing.ENVUSER
+00013170: 4e41 4d45 2c20 454e 5650 4153 5357 4f52  NAME, ENVPASSWOR
+00013180: 443d 6c69 6365 6e73 696e 672e 454e 5650  D=licensing.ENVP
+00013190: 4153 5357 4f52 440a 2020 2020 2020 2020  ASSWORD.        
+000131a0: 2020 2020 2020 2020 2020 2020 2029 290a               )).
+000131b0: 2020 2020 6172 6773 203d 2061 702e 7061      args = ap.pa
+000131c0: 7273 655f 6172 6773 2820 6172 6776 2029  rse_args( argv )
+000131d0: 0a0a 2020 2020 2320 5365 7420 7570 206c  ..    # Set up l
+000131e0: 6f67 6769 6e67 3b20 616c 736f 2c20 6861  ogging; also, ha
+000131f0: 6e64 6c65 2074 6865 2064 6567 656e 6572  ndle the degener
+00013200: 6174 6520 6361 7365 2077 6865 7265 206c  ate case where l
+00013210: 6f67 6769 6e67 2068 6173 202a 616c 7265  ogging has *alre
+00013220: 6164 792a 2062 6565 6e20 7365 7420 7570  ady* been set up
+00013230: 2028 616e 640a 2020 2020 2320 6261 7369   (and.    # basi
+00013240: 6343 6f6e 6669 6720 6973 2061 204e 4f2d  cConfig is a NO-
+00013250: 4f50 292c 2062 7920 2861 6c73 6f29 2073  OP), by (also) s
+00013260: 6574 7469 6e67 2074 6865 206c 6f67 6769  etting the loggi
+00013270: 6e67 206c 6576 656c 2e0a 2020 2020 6c6f  ng level..    lo
+00013280: 675f 6366 675b 276c 6576 656c 275d 0909  g_cfg['level']..
+00013290: 3d20 6c6f 675f 6c65 7665 6c28 2061 7267  = log_level( arg
+000132a0: 732e 7665 7262 6f73 6520 2d20 6172 6773  s.verbose - args
+000132b0: 2e71 7569 6574 2029 0a20 2020 2069 6620  .quiet ).    if 
+000132c0: 6172 6773 2e6c 6f67 206f 7220 6172 6773  args.log or args
+000132d0: 2e67 7569 3a0a 2020 2020 2020 2020 6c6f  .gui:.        lo
+000132e0: 675f 6366 675b 2766 696c 656e 616d 6527  g_cfg['filename'
+000132f0: 5d09 3d20 6172 6773 2e6c 6f67 206f 7220  ].= args.log or 
+00013300: 4c4f 4746 494c 450a 2020 2020 6c6f 6767  LOGFILE.    logg
+00013310: 696e 672e 6261 7369 6343 6f6e 6669 6728  ing.basicConfig(
+00013320: 202a 2a6c 6f67 5f63 6667 2029 0a20 2020   **log_cfg ).   
+00013330: 2069 6620 6172 6773 2e76 6572 626f 7365   if args.verbose
+00013340: 206f 7220 6172 6773 2e71 7569 6574 3a0a   or args.quiet:.
+00013350: 2020 2020 2020 2020 6c6f 6767 696e 672e          logging.
+00013360: 6765 744c 6f67 6765 7228 292e 7365 744c  getLogger().setL
+00013370: 6576 656c 2820 6c6f 675f 6366 675b 276c  evel( log_cfg['l
+00013380: 6576 656c 275d 2029 0a0a 2020 2020 7072  evel'] )..    pr
+00013390: 6f66 696c 6572 0909 093d 204e 6f6e 650a  ofiler...= None.
+000133a0: 2020 2020 7072 6f66 696c 6572 5f6c 696d      profiler_lim
+000133b0: 6974 0909 3d20 3235 0a20 2020 2069 6620  it..= 25.    if 
+000133c0: 6172 6773 2e70 726f 6669 6c65 3a0a 2020  args.profile:.  
+000133d0: 2020 2020 2020 696d 706f 7274 2070 7374        import pst
+000133e0: 6174 730a 2020 2020 2020 2020 7472 793a  ats.        try:
+000133f0: 0a20 2020 2020 2020 2020 2020 2066 726f  .            fro
+00013400: 6d20 6d74 7072 6f66 2069 6d70 6f72 7420  m mtprof import 
+00013410: 5072 6f66 696c 650a 2020 2020 2020 2020  Profile.        
+00013420: 6578 6365 7074 2049 6d70 6f72 7445 7272  except ImportErr
+00013430: 6f72 3a0a 2020 2020 2020 2020 2020 2020  or:.            
+00013440: 6672 6f6d 2063 5072 6f66 696c 6520 696d  from cProfile im
+00013450: 706f 7274 2050 726f 6669 6c65 0a0a 2020  port Profile..  
+00013460: 2020 2020 2020 7072 6f66 696c 6572 0909        profiler..
+00013470: 3d20 5072 6f66 696c 6528 290a 2020 2020  = Profile().    
+00013480: 2020 2020 7072 6f66 696c 6572 2e65 6e61      profiler.ena
+00013490: 626c 6528 290a 0a20 2020 2023 2041 6e79  ble()..    # Any
+000134a0: 2063 6f6e 6669 6775 7261 7469 6f6e 2066   configuration f
+000134b0: 696c 6573 2061 6e64 206c 6963 656e 7369  iles and licensi
+000134c0: 6e67 2e6c 6f61 642f 6c6f 6164 5f6b 6579  ng.load/load_key
+000134d0: 7320 7368 6f75 6c64 2069 6e73 7065 6374  s should inspect
+000134e0: 2074 6865 7365 2065 7874 7261 2064 6972   these extra dir
+000134f0: 730a 2020 2020 676c 6f62 616c 2063 6f6e  s.    global con
+00013500: 6669 675f 6578 7472 6173 0a20 2020 2063  fig_extras.    c
+00013510: 6f6e 6669 675f 6578 7472 6173 0920 2020  onfig_extras.   
+00013520: 2020 2020 2b3d 2061 7267 732e 636f 6e66      += args.conf
+00013530: 6967 206f 7220 5b5d 0a20 2020 206c 6f67  ig or [].    log
+00013540: 2e69 6e66 6f28 2022 4c69 6365 6e73 696e  .info( "Licensin
+00013550: 6720 636f 6e66 6967 7572 6174 696f 6e20  g configuration 
+00013560: 7061 7468 733a 207b 7d22 2e66 6f72 6d61  paths: {}".forma
+00013570: 7428 2027 2c20 272e 6a6f 696e 2820 636f  t( ', '.join( co
+00013580: 6e66 6967 5f70 6174 6873 2820 273c 6669  nfig_paths( '<fi
+00013590: 6c65 3e27 2c20 6578 7472 613d 636f 6e66  le>', extra=conf
+000135a0: 6967 5f65 7874 7261 7320 2929 2929 0a0a  ig_extras ))))..
+000135b0: 2020 2020 2320 4765 7420 736f 6d65 2064      # Get some d
+000135c0: 6574 6169 6c73 2061 626f 7574 2074 6865  etails about the
+000135d0: 2045 6432 3535 3139 2076 6572 7369 6f6e   Ed25519 version
+000135e0: 2077 6527 7265 2075 7369 6e67 2c20 616e   we're using, an
+000135f0: 6420 7375 7070 7265 7373 2073 6f6d 6520  d suppress some 
+00013600: 6e61 6767 696e 6720 6162 6f75 740a 2020  nagging about.  
+00013610: 2020 2320 6c65 7474 696e 6720 6974 2067    # letting it g
+00013620: 656e 6572 6174 6520 7261 6e64 6f6d 2073  enerate random s
+00013630: 6565 6473 2e0a 2020 2020 7761 726e 696e  eeds..    warnin
+00013640: 6773 2e73 696d 706c 6566 696c 7465 7228  gs.simplefilter(
+00013650: 2769 676e 6f72 6527 2920 2023 2057 6520  'ignore')  # We 
+00013660: 6b6e 6f77 2061 626f 7574 2068 616e 646c  know about handl
+00013670: 696e 6720 4564 3235 3531 3920 7261 6e64  ing Ed25519 rand
+00013680: 6f6d 2073 6565 6473 2e2e 2e0a 0a20 2020  om seeds.....   
+00013690: 206c 6f67 2e69 6e66 6f28 2022 4564 3235   log.info( "Ed25
+000136a0: 3531 3920 5665 7273 696f 6e3a 207b 7d20  519 Version: {} 
+000136b0: 2f20 7b7d 202f 207b 7d22 2e66 6f72 6d61  / {} / {}".forma
+000136c0: 7428 0a20 2020 2020 2020 2067 6574 6174  t(.        getat
+000136d0: 7472 2820 6c69 6365 6e73 696e 672e 6564  tr( licensing.ed
+000136e0: 3235 3531 392c 2027 5f5f 7665 7273 696f  25519, '__versio
+000136f0: 6e5f 5f27 2c20 4e6f 6e65 2029 2c20 6c69  n__', None ), li
+00013700: 6365 6e73 696e 672e 6564 3235 3531 392e  censing.ed25519.
+00013710: 5f5f 7061 636b 6167 655f 5f2c 206c 6963  __package__, lic
+00013720: 656e 7369 6e67 2e65 6432 3535 3139 2e5f  ensing.ed25519._
+00013730: 5f70 6174 685f 5f20 2929 0a0a 2020 2020  _path__ ))..    
+00013740: 2320 4c6f 6164 206f 7572 2043 7279 7074  # Load our Crypt
+00013750: 6f20 4c69 6365 6e73 696e 6720 7365 7276  o Licensing serv
+00013760: 6572 2041 6765 6e74 2773 202e 6372 7970  er Agent's .cryp
+00013770: 746f 2d6b 6579 2a20 616e 6420 2e63 7279  to-key* and .cry
+00013780: 7074 6f2d 6c69 632a 2066 696c 6573 2e0a  pto-lic* files..
+00013790: 2020 2020 230a 2020 2020 2320 5468 6973      #.    # This
+000137a0: 2069 7320 7468 6520 4167 656e 7427 7320   is the Agent's 
+000137b0: 4b65 7970 6169 7220 7468 6174 2077 696c  Keypair that wil
+000137c0: 6c20 6265 2061 7373 6967 6e65 6420 6120  l be assigned a 
+000137d0: 4c69 6365 6e73 6520 746f 202a 7275 6e2a  License to *run*
+000137e0: 2061 2043 7279 7074 6f20 4c69 6365 6e73   a Crypto Licens
+000137f0: 696e 670a 2020 2020 2320 7365 7276 6572  ing.    # server
+00013800: 2c20 6f6e 2061 2070 6172 7469 6375 6c61  , on a particula
+00013810: 7220 4d61 6368 696e 6520 4944 2e0a 2020  r Machine ID..  
+00013820: 2020 230a 2020 2020 2320 5468 6973 2069    #.    # This i
+00013830: 7320 2a6e 6f74 2a20 616e 2061 7574 686f  s *not* an autho
+00013840: 7269 7479 2074 6f20 7369 676e 2061 6e64  rity to sign and
+00013850: 202a 6973 7375 652a 2043 7279 7074 6f20   *issue* Crypto 
+00013860: 4c69 6365 6e73 696e 6720 7365 7276 6572  Licensing server
+00013870: 206c 6963 656e 7365 732e 2020 5468 6174   licenses.  That
+00013880: 204b 6579 7061 6972 0a20 2020 2023 2069   Keypair.    # i
+00013890: 7320 6469 6666 6572 656e 742c 2061 6e64  s different, and
+000138a0: 2069 7320 6c6f 6164 6564 202a 696e 746f   is loaded *into
+000138b0: 2a20 7468 6520 4372 7970 746f 204c 6963  * the Crypto Lic
+000138c0: 656e 7369 6e67 2073 6572 7665 722c 2061  ensing server, a
+000138d0: 6e64 2069 7320 7573 6564 2074 6f20 7369  nd is used to si
+000138e0: 676e 206e 6577 0a20 2020 2023 204c 6963  gn new.    # Lic
+000138f0: 656e 7365 7320 7468 6174 2061 7265 2069  enses that are i
+00013900: 7373 7565 6420 746f 206f 7468 6572 2070  ssued to other p
+00013910: 6172 7469 6573 2e0a 2020 2020 230a 2020  arties..    #.  
+00013920: 2020 2320 4966 206e 6563 6573 7361 7279    # If necessary
+00013930: 2c20 7765 276c 6c20 6173 6b20 666f 7220  , we'll ask for 
+00013940: 6120 4c69 6365 6e73 6520 746f 2062 6520  a License to be 
+00013950: 6973 7375 6564 2062 7920 446f 6d69 6e69  issued by Domini
+00013960: 6f6e 2052 2644 2043 6f72 702c 2074 6f20  on R&D Corp, to 
+00013970: 7468 6973 2041 6765 6e74 2c20 666f 720a  this Agent, for.
+00013980: 2020 2020 2320 6175 7468 6f72 697a 6174      # authorizat
+00013990: 696f 6e20 746f 2072 756e 206f 6e20 7468  ion to run on th
+000139a0: 6973 206d 6163 6869 6e65 2e20 2054 6869  is machine.  Thi
+000139b0: 7320 4c69 6365 6e73 6520 7769 6c6c 2067  s License will g
+000139c0: 7261 6e74 2075 7320 7468 6520 6361 7061  rant us the capa
+000139d0: 6269 6c69 7479 2074 6f20 6973 7375 650a  bility to issue.
+000139e0: 2020 2020 2320 7375 622d 4c69 6365 6e73      # sub-Licens
+000139f0: 6573 2066 6f72 2061 2063 6572 7461 696e  es for a certain
+00013a00: 206e 756d 6265 7220 6f66 2022 6d61 7374   number of "mast
+00013a10: 6572 2220 4c69 6365 6e73 6573 2028 4c69  er" Licenses (Li
+00013a20: 6365 6e73 6573 2074 6861 7420 646f 206e  censes that do n
+00013a30: 6f74 2068 6176 6520 610a 2020 2020 2320  ot have a.    # 
+00013a40: 7072 652d 6465 6669 6e65 6420 636c 6965  pre-defined clie
+00013a50: 6e74 2062 616b 6564 2069 6e74 6f20 7468  nt baked into th
+00013a60: 656d 2c20 616e 6420 7468 7573 2063 6f75  em, and thus cou
+00013a70: 6c64 2062 6520 7375 622d 6c69 6365 6e73  ld be sub-licens
+00013a80: 6564 2074 6f20 616e 7920 636c 6965 6e74  ed to any client
+00013a90: 292e 2020 5468 6520 4372 7970 746f 0a20  ).  The Crypto. 
+00013aa0: 2020 2023 204c 6963 656e 7369 6e67 2073     # Licensing s
+00013ab0: 6572 7665 7220 6973 2065 7870 6563 7465  erver is expecte
+00013ac0: 6420 746f 2069 7373 7565 204c 6963 656e  d to issue Licen
+00013ad0: 7365 7320 7468 6174 2063 6f6d 706c 7920  ses that comply 
+00013ae0: 7769 7468 2074 6865 2072 756c 6573 2065  with the rules e
+00013af0: 7374 6162 6c69 7368 6564 2062 7920 7468  stablished by th
+00013b00: 650a 2020 2020 2320 226d 6173 7465 7222  e.    # "master"
+00013b10: 204c 6963 656e 7365 3b20 6966 2069 7420   License; if it 
+00013b20: 6973 2066 6f75 6e64 2074 6861 7420 6f6e  is found that on
+00013b30: 6520 6973 2069 7373 7569 6e67 2069 6e76  e is issuing inv
+00013b40: 616c 6964 204c 6963 656e 7365 7320 2869  alid Licenses (i
+00013b50: 652e 2074 6865 2022 6d61 7374 6572 2220  e. the "master" 
+00013b60: 6772 616e 7473 0a20 2020 2023 2031 3020  grants.    # 10 
+00013b70: 6d61 6368 696e 6573 2c20 6275 7420 6d6f  machines, but mo
+00013b80: 7265 2074 6861 6e20 3130 2073 7562 2d4c  re than 10 sub-L
+00013b90: 6963 656e 7365 7320 6861 7665 2062 6565  icenses have bee
+00013ba0: 6e20 6973 7375 6564 292c 2074 6865 6e20  n issued), then 
+00013bb0: 6974 7320 6c69 6365 6e73 6520 7769 6c6c  its license will
+00013bc0: 2062 6520 7265 766f 6b65 640a 2020 2020   be revoked.    
+00013bd0: 2320 6279 2062 6c61 636b 6c69 7374 696e  # by blacklistin
+00013be0: 6720 6974 7320 7075 626c 6963 206b 6579  g its public key
+00013bf0: 2e0a 2020 2020 230a 2020 2020 2320 5468  ..    #.    # Th
+00013c00: 6520 7365 6372 6574 7320 7265 7175 6972  e secrets requir
+00013c10: 6564 2074 6f20 6465 6372 7970 7420 7468  ed to decrypt th
+00013c20: 6520 6c69 6365 6e73 696e 672e 4b65 7970  e licensing.Keyp
+00013c30: 6169 7245 6e63 7279 7074 6564 2061 7265  airEncrypted are
+00013c40: 2065 7870 6563 7465 6420 746f 2062 6520   expected to be 
+00013c50: 696e 0a20 2020 2023 2065 6e76 6972 6f6e  in.    # environ
+00013c60: 6d65 6e74 2076 6172 6961 626c 6573 2028  ment variables (
+00013c70: 7370 6563 6966 7920 272d 2720 746f 2072  specify '-' to r
+00013c80: 6561 6420 6672 6f6d 2069 6e70 7574 293a  ead from input):
+00013c90: 0a20 2020 2023 0a20 2020 2023 2020 2020  .    #.    #    
+00013ca0: 2043 5259 5054 4f5f 4c49 435f 5553 4552   CRYPTO_LIC_USER
+00013cb0: 4e41 4d45 2020 2320 6f72 202d 2d75 7365  NAME  # or --use
+00013cc0: 726e 616d 650a 2020 2020 2320 2020 2020  rname.    #     
+00013cd0: 4352 5950 544f 5f4c 4943 5f50 4153 5357  CRYPTO_LIC_PASSW
+00013ce0: 4f52 4420 2023 206f 7220 2d2d 7061 7373  ORD  # or --pass
+00013cf0: 776f 7264 2028 756e 7361 6665 290a 2020  word (unsafe).  
+00013d00: 2020 230a 2020 2020 2320 5468 656e 2c20    #.    # Then, 
+00013d10: 6669 6e64 2061 6e64 206c 6f61 6420 7468  find and load th
+00013d20: 6520 4b65 7970 6161 7220 616e 6420 4c69  e Keypaar and Li
+00013d30: 6365 6e73 6520 2d2d 7072 6f64 7563 7420  cense --product 
+00013d40: 2873 706c 6974 206f 6e20 7370 6163 6573  (split on spaces
+00013d50: 292c 206a 6f69 6e65 6420 6279 2027 2d27  ), joined by '-'
+00013d60: 293a 0a20 2020 2023 0a20 2020 2023 2020  ):.    #.    #  
+00013d70: 2020 2063 7279 7074 6f2d 6c69 6365 6e73     crypto-licens
+00013d80: 696e 672d 7365 7276 6572 2e63 7279 7074  ing-server.crypt
+00013d90: 6f2d 7b6b 6579 7061 6972 2c6c 6963 656e  o-{keypair,licen
+00013da0: 7365 7d0a 2020 2020 230a 2020 2020 6261  se}.    #.    ba
+00013db0: 7365 6e61 6d65 0909 093d 2027 2d27 2e6a  sename...= '-'.j
+00013dc0: 6f69 6e28 205b 2073 6567 6d65 6e74 2e6c  oin( [ segment.l
+00013dd0: 6f77 6572 2829 2066 6f72 2073 6567 6d65  ower() for segme
+00013de0: 6e74 2069 6e20 6172 6773 2e70 726f 6475  nt in args.produ
+00013df0: 6374 2e73 706c 6974 2829 205d 2029 0a20  ct.split() ] ). 
+00013e00: 2020 206c 6f67 2e6c 6f67 2820 6c6f 6767     log.log( logg
+00013e10: 696e 672e 4445 5441 494c 2c20 224c 6f61  ing.DETAIL, "Loa
+00013e20: 6469 6e67 2041 6765 6e74 2045 6432 3535  ding Agent Ed255
+00013e30: 3139 204b 6579 7061 6972 2066 726f 6d20  19 Keypair from 
+00013e40: 7b7d 2e2e 2e22 2e66 6f72 6d61 7428 2062  {}...".format( b
+00013e50: 6173 656e 616d 6520 2929 0a20 2020 2023  asename )).    #
+00013e60: 204c 6f61 6420 4167 656e 7420 4b65 7970   Load Agent Keyp
+00013e70: 6169 722c 2069 6620 616e 792c 2075 7369  air, if any, usi
+00013e80: 6e67 2061 6e79 2063 7265 6465 6e74 6961  ng any credentia
+00013e90: 6c73 2073 7570 706c 6965 6420 696e 2074  ls supplied in t
+00013ea0: 6865 2065 6e76 6972 6f6e 6d65 6e74 0a20  he environment. 
+00013eb0: 2020 2063 6c5f 7573 6572 6e61 6d65 0909     cl_username..
+00013ec0: 093d 2061 7267 732e 7573 6572 6e61 6d65  .= args.username
+00013ed0: 206f 7220 6f73 2e67 6574 656e 7628 206c   or os.getenv( l
+00013ee0: 6963 656e 7369 6e67 2e45 4e56 5553 4552  icensing.ENVUSER
+00013ef0: 4e41 4d45 2029 0a20 2020 2063 6c5f 7061  NAME ).    cl_pa
+00013f00: 7373 776f 7264 0909 093d 2061 7267 732e  ssword...= args.
+00013f10: 7061 7373 776f 7264 206f 7220 6f73 2e67  password or os.g
+00013f20: 6574 656e 7628 206c 6963 656e 7369 6e67  etenv( licensing
+00013f30: 2e45 4e56 5041 5353 574f 5244 2029 0a20  .ENVPASSWORD ). 
+00013f40: 2020 2069 6620 6172 6773 2e70 6173 7377     if args.passw
+00013f50: 6f72 6420 616e 6420 6172 6773 2e70 6173  ord and args.pas
+00013f60: 7377 6f72 6420 213d 2027 2d27 3a0a 2020  sword != '-':.  
+00013f70: 2020 2020 2020 6c6f 672e 7761 726e 696e        log.warnin
+00013f80: 6728 2022 4974 2069 7320 7265 636f 6d6d  g( "It is recomm
+00013f90: 656e 6465 6420 746f 206e 6f74 2075 7365  ended to not use
+00013fa0: 2027 2d50 7c2d 2d70 6173 7377 6f72 6420   '-P|--password 
+00013fb0: 2e2e 2e27 3b20 7370 6563 6966 7920 272d  ...'; specify '-
+00013fc0: 2720 746f 2072 6561 6420 6672 6f6d 2069  ' to read from i
+00013fd0: 6e70 7574 2220 290a 0a20 2020 2023 2043  nput" )..    # C
+00013fe0: 7963 6c65 2074 6872 6f75 6768 2074 6865  ycle through the
+00013ff0: 2061 7661 696c 6162 6c65 2041 6765 6e74   available Agent
+00014000: 2049 4420 6b65 7973 2c20 616e 6420 616e   ID keys, and an
+00014010: 7920 4c69 6365 6e73 6528 7329 2066 6f72  y License(s) for
+00014020: 2044 6f6d 696e 696f 6e20 5226 4427 7320   Dominion R&D's 
+00014030: 4372 7970 746f 0a20 2020 2023 204c 6963  Crypto.    # Lic
+00014040: 656e 7369 6e67 2e20 2054 6f20 6372 6561  ensing.  To crea
+00014050: 7465 2061 6e20 756e 656e 6372 7970 7465  te an unencrypte
+00014060: 6420 4b65 7970 6169 722c 206e 6f20 2d2d  d Keypair, no --
+00014070: 7573 6572 6e61 6d65 2f2d 2d70 6173 7377  username/--passw
+00014080: 6f72 6420 6d61 7920 6265 2073 7065 6369  ord may be speci
+00014090: 6669 6564 2e0a 2020 2020 2320 4f74 6865  fied..    # Othe
+000140a0: 7277 6973 652c 2077 6520 6d75 7374 2062  rwise, we must b
+000140b0: 6c6f 636b 2068 6572 6520 6177 6169 7469  lock here awaiti
+000140c0: 6e67 2069 6e70 7574 2e0a 2020 2020 7573  ng input..    us
+000140d0: 6572 6e61 6d65 0909 093d 2069 6e70 7574  ername...= input
+000140e0: 5f73 6563 7572 6528 2022 456e 7465 7220  _secure( "Enter 
+000140f0: 7b7d 2075 7365 726e 616d 653a 2022 2e66  {} username: ".f
+00014100: 6f72 6d61 7428 2062 6173 656e 616d 6520  ormat( basename 
+00014110: 2929 2069 6620 636c 5f75 7365 726e 616d  )) if cl_usernam
+00014120: 6520 3d3d 2027 2d27 2065 6c73 6520 636c  e == '-' else cl
+00014130: 5f75 7365 726e 616d 650a 2020 2020 7061  _username.    pa
+00014140: 7373 776f 7264 0909 093d 2069 6e70 7574  ssword...= input
+00014150: 5f73 6563 7572 6528 2022 456e 7465 7220  _secure( "Enter 
+00014160: 7b7d 2070 6173 7377 6f72 643a 2022 2e66  {} password: ".f
+00014170: 6f72 6d61 7428 2062 6173 656e 616d 6520  ormat( basename 
+00014180: 2929 2069 6620 636c 5f70 6173 7377 6f72  )) if cl_passwor
+00014190: 6420 3d3d 2027 2d27 2065 6c73 6520 636c  d == '-' else cl
+000141a0: 5f70 6173 7377 6f72 640a 2020 2020 7573  _password.    us
+000141b0: 6572 7061 7373 5f69 6e70 7574 0909 3d20  erpass_input..= 
+000141c0: 636c 5f75 7365 726e 616d 6520 3d3d 2027  cl_username == '
+000141d0: 2d27 206f 7220 636c 5f70 6173 7377 6f72  -' or cl_passwor
+000141e0: 6420 3d3d 2027 2d27 0a20 2020 2074 7279  d == '-'.    try
+000141f0: 3a0a 2020 2020 2020 2020 2320 5765 2772  :.        # We'r
+00014200: 6520 6c6f 6f6b 696e 6720 666f 7220 6120  e looking for a 
+00014210: 4c69 6365 6e73 6520 6175 7468 6f72 6564  License authored
+00014220: 2062 7920 446f 6d69 6e69 6f6e 2052 2644   by Dominion R&D
+00014230: 2043 6f72 702e 2020 5468 6973 206d 6967   Corp.  This mig
+00014240: 6874 2062 6520 656e 6361 7073 756c 6174  ht be encapsulat
+00014250: 6564 2061 730a 2020 2020 2020 2020 2320  ed as.        # 
+00014260: 6f6e 6520 6f66 2074 6865 2064 6570 656e  one of the depen
+00014270: 6465 6e63 6965 7320 6f66 2074 6865 204c  dencies of the L
+00014280: 6963 656e 7365 2077 6520 6669 6e64 2028  icense we find (
+00014290: 6567 2e20 6966 2044 6f6d 696e 696f 6e20  eg. if Dominion 
+000142a0: 6973 7375 6573 2061 204c 6963 656e 7365  issues a License
+000142b0: 2074 6f20 736f 6d65 0a20 2020 2020 2020   to some.       
+000142c0: 2023 2063 6f6d 7061 6e79 2c20 7768 6963   # company, whic
+000142d0: 6820 696e 636c 7564 6573 2074 6865 2061  h includes the a
+000142e0: 6269 6c69 7479 2074 6f20 7275 6e20 6120  bility to run a 
+000142f0: 6372 7970 746f 2d6c 6963 656e 7369 6e67  crypto-licensing
+00014300: 2073 6572 7665 7229 2c20 6275 7420 7765   server), but we
+00014310: 276c 6c20 7661 6c69 6461 7465 0a20 2020  'll validate.   
+00014320: 2020 2020 2023 2074 6861 7420 7468 6520       # that the 
+00014330: 4772 616e 7420 7761 7320 6973 7375 6564  Grant was issued
+00014340: 2062 7920 446f 6d69 6e69 6f6e 2052 2644   by Dominion R&D
+00014350: 2043 6f72 702e 2020 466f 7220 6578 616d   Corp.  For exam
+00014360: 706c 652c 2044 6f6d 696e 696f 6e20 6973  ple, Dominion is
+00014370: 7375 6573 2061 204c 6963 656e 7365 2074  sues a License t
+00014380: 6f0a 2020 2020 2020 2020 2320 6177 6573  o.        # awes
+00014390: 6f6d 652d 696e 632e 636f 6d20 746f 2073  ome-inc.com to s
+000143a0: 7562 2d4c 6963 656e 7365 2063 7279 7074  ub-License crypt
+000143b0: 6f2d 6c69 6365 6e73 696e 6720 7365 7276  o-licensing serv
+000143c0: 6572 732e 2020 5468 6579 2c20 696e 2074  ers.  They, in t
+000143d0: 7572 6e2c 2069 7373 7565 2061 204c 6963  urn, issue a Lic
+000143e0: 656e 7365 0a20 2020 2020 2020 2023 2074  ense.        # t
+000143f0: 6f20 d09b d0b0 d0b9 d0ba d0b0 2e72 7520  o ...........ru 
+00014400: 746f 2072 756e 2061 2063 7279 7074 6f2d  to run a crypto-
+00014410: 6c69 6365 6e73 696e 6720 7365 7276 6572  licensing server
+00014420: 2c20 616e 6420 6865 6c70 2074 6865 6d20  , and help them 
+00014430: 7365 7420 6974 2075 702e 2020 5768 656e  set it up.  When
+00014440: 0a20 2020 2020 2020 2023 2068 7474 703a  .        # http:
+00014450: 2f2f 6372 7970 746f 2d6c 6963 656e 7369  //crypto-licensi
+00014460: 6e67 2e78 6e2d 2d38 3061 6130 6165 632e  ng.xn--80aa0aec.
+00014470: 7275 2f20 2863 7279 7074 6f2d 6c69 6365  ru/ (crypto-lice
+00014480: 6e73 696e 672e d09b d0b0 d0b9 d0ba d0b0  nsing...........
+00014490: 2e72 7529 2069 7373 7565 7320 6120 4c69  .ru) issues a Li
+000144a0: 6365 6e73 6520 666f 720a 2020 2020 2020  cense for.      
+000144b0: 2020 2320 7468 6569 7220 736f 6674 7761    # their softwa
+000144c0: 7265 2c20 7061 7274 206f 6620 7468 6520  re, part of the 
+000144d0: 6665 6573 2061 7265 2070 6169 6420 746f  fees are paid to
+000144e0: 2061 7765 736f 6d65 2d69 6e63 2e63 6f6d   awesome-inc.com
+000144f0: 2061 6e64 2073 6f6d 6520 746f 2064 6f6d   and some to dom
+00014500: 696e 696f 6e72 6e64 2e63 6f6d 2e0a 2020  inionrnd.com..  
+00014510: 2020 2020 2020 2320 5468 6520 6669 6e61        # The fina
+00014520: 6c20 736f 6674 7761 7265 2069 6e73 7461  l software insta
+00014530: 6c6c 6174 696f 6e20 7573 6573 2063 7279  llation uses cry
+00014540: 7074 6f2d 6c69 6365 6e73 696e 6727 7320  pto-licensing's 
+00014550: 6175 7468 6f72 697a 6564 2829 2066 756e  authorized() fun
+00014560: 6374 696f 6e2c 2077 6869 6368 2063 6865  ction, which che
+00014570: 636b 730a 2020 2020 2020 2020 2320 7468  cks.        # th
+00014580: 6174 2065 6163 6820 7375 6363 6573 7369  at each successi
+00014590: 7665 204c 6963 656e 7365 2773 2064 6570  ve License's dep
+000145a0: 656e 6465 6e63 6965 7320 6172 6520 636f  endencies are co
+000145b0: 7272 6563 746c 7920 7369 676e 6564 2c20  rrectly signed, 
+000145c0: 616e 6420 6361 7272 6965 7320 7468 6520  and carries the 
+000145d0: 6f72 6967 696e 616c 0a20 2020 2020 2020  original.       
+000145e0: 2023 2027 6372 7970 746f 2d6c 6963 656e   # 'crypto-licen
+000145f0: 7369 6e67 2720 4772 616e 7420 7468 726f  sing' Grant thro
+00014600: 7567 6820 746f 2074 6865 2072 6563 6970  ugh to the recip
+00014610: 6965 6e74 2e0a 2020 2020 2020 2020 646f  ient..        do
+00014620: 6d69 6e69 6f6e 0909 3d20 6c69 6365 6e73  minion..= licens
+00014630: 696e 672e 4167 656e 7428 0a20 2020 2020  ing.Agent(.     
+00014640: 2020 2020 2020 206e 616d 6509 3d20 6c69         name.= li
+00014650: 6365 6e73 696e 672e 434f 4d50 414e 592c  censing.COMPANY,
+00014660: 0a20 2020 2020 2020 2020 2020 2064 6f6d  .            dom
+00014670: 6169 6e09 3d20 6c69 6365 6e73 696e 672e  ain.= licensing.
+00014680: 444f 4d41 494e 2c0a 2020 2020 2020 2020  DOMAIN,.        
+00014690: 2020 2020 7072 6f64 7563 7409 3d20 6c69      product.= li
+000146a0: 6365 6e73 696e 672e 5052 4f44 5543 542c  censing.PRODUCT,
+000146b0: 0a20 2020 2020 2020 2020 2020 2070 7562  .            pub
+000146c0: 6b65 7909 3d20 6c69 6365 6e73 696e 672e  key.= licensing.
+000146d0: 5055 424b 4559 2c0a 2020 2020 2020 2020  PUBKEY,.        
+000146e0: 290a 2020 2020 2020 2020 7365 7276 6572  ).        server
+000146f0: 0909 093d 204e 6f6e 650a 2020 2020 2020  ...= None.      
+00014700: 2020 6966 2061 7267 732e 7072 6f64 7563    if args.produc
+00014710: 7420 616e 6420 6172 6773 2e64 6f6d 6169  t and args.domai
+00014720: 6e3a 0a20 2020 2020 2020 2020 2020 2073  n:.            s
+00014730: 6572 7665 7209 093d 206c 6963 656e 7369  erver..= licensi
+00014740: 6e67 2e41 6765 6e74 280a 2020 2020 2020  ng.Agent(.      
+00014750: 2020 2020 2020 2020 2020 6e61 6d65 093d            name.=
+00014760: 2061 7267 732e 636c 6965 6e74 2c0a 2020   args.client,.  
+00014770: 2020 2020 2020 2020 2020 2020 2020 646f                do
+00014780: 6d61 696e 093d 2061 7267 732e 646f 6d61  main.= args.doma
+00014790: 696e 2c0a 2020 2020 2020 2020 2020 2020  in,.            
+000147a0: 2020 2020 7072 6f64 7563 7409 3d20 6172      product.= ar
+000147b0: 6773 2e70 726f 6475 6374 2c0a 2020 2020  gs.product,.    
+000147c0: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+000147d0: 2020 2061 7574 686f 7269 7a61 7469 6f6e     authorization
+000147e0: 0909 3d20 6c69 6365 6e73 696e 672e 6175  ..= licensing.au
+000147f0: 7468 6f72 697a 6564 280a 2020 2020 2020  thorized(.      
+00014800: 2020 2020 2020 6175 7468 6f72 093d 2064        author.= d
+00014810: 6f6d 696e 696f 6e2c 0a20 2020 2020 2020  ominion,.       
+00014820: 2020 2020 2063 6c69 656e 7409 3d20 7365       client.= se
+00014830: 7276 6572 2c0a 2020 2020 2020 2020 2020  rver,.          
+00014840: 2020 6261 7365 6e61 6d65 093d 2062 6173    basename.= bas
+00014850: 656e 616d 652c 0a20 2020 2020 2020 2020  ename,.         
+00014860: 2020 2075 7365 726e 616d 6509 3d20 7573     username.= us
+00014870: 6572 6e61 6d65 2c0a 2020 2020 2020 2020  ername,.        
+00014880: 2020 2020 7061 7373 776f 7264 093d 2070      password.= p
+00014890: 6173 7377 6f72 642c 0a20 2020 2020 2020  assword,.       
+000148a0: 2020 2020 2072 6567 6973 7465 7269 6e67       registering
+000148b0: 093d 2061 7267 732e 7265 6769 7374 6572  .= args.register
+000148c0: 2c20 2020 2020 2020 2023 2049 7373 7565  ,        # Issue
+000148d0: 2061 6e20 4167 656e 7420 4944 2069 6620   an Agent ID if 
+000148e0: 6e6f 6e65 2066 6f75 6e64 3f0a 2020 2020  none found?.    
+000148f0: 2020 2020 2020 2020 6163 7175 6972 696e          acquirin
+00014900: 6709 3d20 6172 6773 2e61 6371 7569 7265  g.= args.acquire
+00014910: 2c09 0923 2041 6371 7569 7265 2061 204c  ,..# Acquire a L
+00014920: 6963 656e 7365 2069 6620 6e6f 6e65 2066  icense if none f
+00014930: 6f75 6e64 3f0a 2020 2020 2020 2020 2020  ound?.          
+00014940: 2020 6578 7472 6109 3d20 636f 6e66 6967    extra.= config
+00014950: 5f65 7874 7261 732c 2020 2020 2020 2020  _extras,        
+00014960: 2320 696e 636c 7564 696e 6720 616e 7920  # including any 
+00014970: 6c6f 6361 6c6c 7920 6465 6669 6e65 6420  locally defined 
+00014980: 636f 6e66 6967 2064 6972 730a 2020 2020  config dirs.    
+00014990: 2020 2020 290a 0a20 2020 2020 2020 206c      )..        l
+000149a0: 6f61 6465 6409 0909 3d20 5b5d 0a20 2020  oaded...= [].   
+000149b0: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+000149c0: 2020 2020 2020 6b65 792c 6c69 6309 093d        key,lic..=
+000149d0: 206e 6578 7428 2061 7574 686f 7269 7a61   next( authoriza
+000149e0: 7469 6f6e 2029 0a20 2020 2020 2020 2020  tion ).         
+000149f0: 2020 2077 6869 6c65 2054 7275 653a 0a20     while True:. 
+00014a00: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00014a10: 6620 6b65 7920 6973 204e 6f6e 6520 6f72  f key is None or
+00014a20: 206c 6963 2069 7320 4e6f 6e65 3a0a 2020   lic is None:.  
+00014a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014a40: 2020 7768 6174 0909 3d20 224e 6f20 4c69    what..= "No Li
+00014a50: 6365 6e73 6520 666f 756e 6420 666f 7220  cense found for 
+00014a60: 4167 656e 7420 4944 207b 7d22 2e66 6f72  Agent ID {}".for
+00014a70: 6d61 7428 0a20 2020 2020 2020 2020 2020  mat(.           
+00014a80: 2020 2020 2020 2020 2020 2020 206c 6963               lic
+00014a90: 656e 7369 6e67 2e69 6e74 6f5f 6236 3428  ensing.into_b64(
+00014aa0: 206b 6579 2e76 6b20 2929 2069 6620 6b65   key.vk )) if ke
+00014ab0: 7920 656c 7365 2022 4e6f 2041 6765 6e74  y else "No Agent
+00014ac0: 2049 4420 4b65 7970 6169 7220 666f 756e   ID Keypair foun
+00014ad0: 6422 0a20 2020 2020 2020 2020 2020 2020  d".             
+00014ae0: 2020 2020 2020 2069 6620 7573 6572 7061         if userpa
+00014af0: 7373 5f69 6e70 7574 3a0a 2020 2020 2020  ss_input:.      
+00014b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014b10: 2020 7768 6174 2020 2020 2020 202b 3d20    what       += 
+00014b20: 223b 2065 6e74 6572 2063 7265 6465 6e74  "; enter credent
+00014b30: 6961 6c73 220a 2020 2020 2020 2020 2020  ials".          
+00014b40: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00014b50: 2070 6173 7377 6f72 6420 213d 2022 2d22   password != "-"
+00014b60: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00014b70: 2020 2020 2020 2020 2020 2020 2020 7768                wh
+00014b80: 6174 2020 202b 3d20 2220 286c 6561 7665  at   += " (leave
+00014b90: 2062 6c61 6e6b 2074 6f20 7265 6769 7374   blank to regist
+00014ba0: 6572 2077 2f20 7b7d 3a20 7b7d 222e 666f  er w/ {}: {}".fo
+00014bb0: 726d 6174 280a 2020 2020 2020 2020 2020  rmat(.          
+00014bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014bd0: 2020 2020 2020 7573 6572 6e61 6d65 206f        username o
+00014be0: 7220 2228 6e6f 2075 7365 726e 616d 6529  r "(no username)
+00014bf0: 222c 2027 2a27 202a 206c 656e 2820 7061  ", '*' * len( pa
+00014c00: 7373 776f 7264 206f 7220 2727 2029 206f  ssword or '' ) o
+00014c10: 7220 2228 6e6f 2070 6173 7377 6f72 6429  r "(no password)
+00014c20: 2220 290a 2020 2020 2020 2020 2020 2020  " ).            
+00014c30: 2020 2020 2020 2020 6c6f 672e 7761 726e          log.warn
+00014c40: 696e 6728 2077 6861 7420 290a 2020 2020  ing( what ).    
 00014c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014c60: 2320 7468 656e 2061 7574 686f 7269 7a61  # then authoriza
-00014c70: 7469 6f6e 206d 6179 2067 6f20 6f6e 2074  tion may go on t
-00014c80: 6f20 7265 6769 7374 6572 2077 2f20 7468  o register w/ th
-00014c90: 6520 6c61 7374 2d65 6e74 6572 6564 2075  e last-entered u
-00014ca0: 7365 726e 616d 652f 7061 7373 776f 7264  sername/password
-00014cb0: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00014cc0: 2020 2320 4569 7468 6572 2075 7365 726e    # Either usern
-00014cd0: 616d 6520 6f72 2070 6173 7377 6f72 6420  ame or password 
-00014ce0: 6d61 7920 6265 2075 7064 6174 6564 2c20  may be updated, 
-00014cf0: 6966 2064 6573 6972 6564 2e20 2055 7375  if desired.  Usu
-00014d00: 616c 6c79 2c20 6372 6564 656e 7469 616c  ally, credential
-00014d10: 2069 6e70 7574 0a20 2020 2020 2020 2020   input.         
-00014d20: 2020 2020 2020 2023 2066 6f72 6365 7320         # forces 
-00014d30: 796f 7520 746f 2072 652d 656e 7465 7220  you to re-enter 
-00014d40: 736f 6d65 7468 696e 6720 796f 7520 6b6e  something you kn
-00014d50: 6f77 2074 6f20 6265 2063 6f72 7265 6374  ow to be correct
-00014d60: 3b20 7468 6973 206c 6f6f 7020 646f 6573  ; this loop does
-00014d70: 206e 6f74 2e0a 2020 2020 2020 2020 2020   not..          
-00014d80: 2020 2020 2020 2320 4661 696c 696e 6720        # Failing 
-00014d90: 746f 2065 6e74 6572 2062 6f74 6820 6372  to enter both cr
-00014da0: 6564 656e 7469 616c 7320 696e 6469 6361  edentials indica
-00014db0: 7465 7320 7361 7469 7366 6163 7469 6f6e  tes satisfaction
-00014dc0: 202d 2d20 676f 6573 206f 6e20 746f 2072   -- goes on to r
-00014dd0: 6567 6973 7465 7220 610a 2020 2020 2020  egister a.      
-00014de0: 2020 2020 2020 2020 2020 2320 6e65 7720            # new 
-00014df0: 4167 656e 7420 4944 2077 2f20 6372 6564  Agent ID w/ cred
-00014e00: 656e 7469 616c 732c 2069 6620 736f 2e0a  entials, if so..
-00014e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014e20: 7573 6572 7061 7373 5f75 7064 6174 6564  userpass_updated
-00014e30: 203d 2046 616c 7365 0a20 2020 2020 2020   = False.       
-00014e40: 2020 2020 2020 2020 2069 6620 636c 5f75           if cl_u
-00014e50: 7365 726e 616d 6520 3d3d 2027 2d27 3a0a  sername == '-':.
-00014e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014e70: 2020 2020 7573 6572 6e61 6d65 5f75 7064      username_upd
-00014e80: 6174 6509 3d20 696e 7075 745f 7365 6375  ate.= input_secu
-00014e90: 7265 2820 2245 6e74 6572 207b 7d20 7573  re( "Enter {} us
-00014ea0: 6572 6e61 6d65 2028 6c65 6176 6520 656d  ername (leave em
-00014eb0: 7074 7920 666f 7220 6e6f 2063 6861 6e67  pty for no chang
-00014ec0: 6529 3a20 222e 666f 726d 6174 2820 6261  e): ".format( ba
-00014ed0: 7365 6e61 6d65 2029 290a 2020 2020 2020  sename )).      
-00014ee0: 2020 2020 2020 2020 2020 2020 2020 7573                us
-00014ef0: 6572 7061 7373 5f75 7064 6174 6564 207c  erpass_updated |
-00014f00: 3d20 626f 6f6c 2820 7573 6572 6e61 6d65  = bool( username
-00014f10: 5f75 7064 6174 6520 290a 2020 2020 2020  _update ).      
-00014f20: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00014f30: 2075 7365 726e 616d 655f 7570 6461 7465   username_update
-00014f40: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00014f50: 2020 2020 2020 2020 2020 7573 6572 6e61            userna
-00014f60: 6d65 093d 2075 7365 726e 616d 655f 7570  me.= username_up
-00014f70: 6461 7465 0a20 2020 2020 2020 2020 2020  date.           
-00014f80: 2020 2020 2069 6620 636c 5f70 6173 7377       if cl_passw
-00014f90: 6f72 6420 3d3d 2027 2d27 3a0a 2020 2020  ord == '-':.    
-00014fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014fb0: 7061 7373 776f 7264 5f75 7064 6174 6509  password_update.
-00014fc0: 3d20 696e 7075 745f 7365 6375 7265 2820  = input_secure( 
-00014fd0: 2245 6e74 6572 207b 7d20 7061 7373 776f  "Enter {} passwo
-00014fe0: 7264 2028 6c65 6176 6520 656d 7074 7920  rd (leave empty 
-00014ff0: 666f 7220 6e6f 2063 6861 6e67 6529 3a20  for no change): 
-00015000: 222e 666f 726d 6174 2820 6261 7365 6e61  ".format( basena
-00015010: 6d65 2029 290a 2020 2020 2020 2020 2020  me )).          
-00015020: 2020 2020 2020 2020 2020 7573 6572 7061            userpa
-00015030: 7373 5f75 7064 6174 6564 207c 3d20 626f  ss_updated |= bo
-00015040: 6f6c 2820 7061 7373 776f 7264 5f75 7064  ol( password_upd
-00015050: 6174 6520 290a 2020 2020 2020 2020 2020  ate ).          
-00015060: 2020 2020 2020 2020 2020 6966 2070 6173            if pas
-00015070: 7377 6f72 645f 7570 6461 7465 3a0a 2020  sword_update:.  
+00014c60: 6966 206e 6f74 2075 7365 7270 6173 735f  if not userpass_
+00014c70: 696e 7075 743a 0a20 2020 2020 2020 2020  input:.         
+00014c80: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00014c90: 6f6e 7469 6e75 650a 2020 2020 2020 2020  ontinue.        
+00014ca0: 2020 2020 2020 2020 2020 2020 2320 4e6f              # No
+00014cb0: 2041 6765 6e74 2049 442f 4c69 6365 6e73   Agent ID/Licens
+00014cc0: 6520 6c6f 6164 6564 3b20 7573 6572 6e61  e loaded; userna
+00014cd0: 6d65 2f70 6173 7377 6f72 6420 6d61 7920  me/password may 
+00014ce0: 6265 2069 6e63 6f72 7265 6374 2e20 2049  be incorrect.  I
+00014cf0: 6620 6e6f 6e65 2070 726f 7669 6465 642c  f none provided,
+00014d00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014d10: 2020 2020 2023 2074 6865 6e20 6175 7468       # then auth
+00014d20: 6f72 697a 6174 696f 6e20 6d61 7920 676f  orization may go
+00014d30: 206f 6e20 746f 2072 6567 6973 7465 7220   on to register 
+00014d40: 772f 2074 6865 206c 6173 742d 656e 7465  w/ the last-ente
+00014d50: 7265 6420 7573 6572 6e61 6d65 2f70 6173  red username/pas
+00014d60: 7377 6f72 642e 0a20 2020 2020 2020 2020  sword..         
+00014d70: 2020 2020 2020 2020 2020 2023 2045 6974             # Eit
+00014d80: 6865 7220 7573 6572 6e61 6d65 206f 7220  her username or 
+00014d90: 7061 7373 776f 7264 206d 6179 2062 6520  password may be 
+00014da0: 7570 6461 7465 642c 2069 6620 6465 7369  updated, if desi
+00014db0: 7265 642e 2020 5573 7561 6c6c 792c 2063  red.  Usually, c
+00014dc0: 7265 6465 6e74 6961 6c20 696e 7075 740a  redential input.
+00014dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014de0: 2020 2020 2320 666f 7263 6573 2079 6f75      # forces you
+00014df0: 2074 6f20 7265 2d65 6e74 6572 2073 6f6d   to re-enter som
+00014e00: 6574 6869 6e67 2079 6f75 206b 6e6f 7720  ething you know 
+00014e10: 746f 2062 6520 636f 7272 6563 743b 2074  to be correct; t
+00014e20: 6869 7320 6c6f 6f70 2064 6f65 7320 6e6f  his loop does no
+00014e30: 742e 0a20 2020 2020 2020 2020 2020 2020  t..             
+00014e40: 2020 2020 2020 2023 2046 6169 6c69 6e67         # Failing
+00014e50: 2074 6f20 656e 7465 7220 626f 7468 2063   to enter both c
+00014e60: 7265 6465 6e74 6961 6c73 2069 6e64 6963  redentials indic
+00014e70: 6174 6573 2073 6174 6973 6661 6374 696f  ates satisfactio
+00014e80: 6e20 2d2d 2067 6f65 7320 6f6e 2074 6f20  n -- goes on to 
+00014e90: 7265 6769 7374 6572 2061 0a20 2020 2020  register a.     
+00014ea0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00014eb0: 206e 6577 2041 6765 6e74 2049 4420 772f   new Agent ID w/
+00014ec0: 2063 7265 6465 6e74 6961 6c73 2c20 6966   credentials, if
+00014ed0: 2073 6f2e 0a20 2020 2020 2020 2020 2020   so..           
+00014ee0: 2020 2020 2020 2020 2075 7365 7270 6173           userpas
+00014ef0: 735f 7570 6461 7465 6420 3d20 4661 6c73  s_updated = Fals
+00014f00: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+00014f10: 2020 2020 2020 6966 2063 6c5f 7573 6572        if cl_user
+00014f20: 6e61 6d65 203d 3d20 272d 273a 0a20 2020  name == '-':.   
+00014f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014f40: 2020 2020 2075 7365 726e 616d 655f 7570       username_up
+00014f50: 6461 7465 093d 2069 6e70 7574 5f73 6563  date.= input_sec
+00014f60: 7572 6528 2022 456e 7465 7220 7b7d 2075  ure( "Enter {} u
+00014f70: 7365 726e 616d 6520 286c 6561 7665 2065  sername (leave e
+00014f80: 6d70 7479 2066 6f72 206e 6f20 6368 616e  mpty for no chan
+00014f90: 6765 293a 2022 2e66 6f72 6d61 7428 2062  ge): ".format( b
+00014fa0: 6173 656e 616d 6520 2929 0a20 2020 2020  asename )).     
+00014fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014fc0: 2020 2075 7365 7270 6173 735f 7570 6461     userpass_upda
+00014fd0: 7465 6420 7c3d 2062 6f6f 6c28 2075 7365  ted |= bool( use
+00014fe0: 726e 616d 655f 7570 6461 7465 2029 0a20  rname_update ). 
+00014ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015000: 2020 2020 2020 2069 6620 7573 6572 6e61         if userna
+00015010: 6d65 5f75 7064 6174 653a 0a20 2020 2020  me_update:.     
+00015020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015030: 2020 2020 2020 2075 7365 726e 616d 6509         username.
+00015040: 3d20 7573 6572 6e61 6d65 5f75 7064 6174  = username_updat
+00015050: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+00015060: 2020 2020 2020 6966 2063 6c5f 7061 7373        if cl_pass
+00015070: 776f 7264 203d 3d20 272d 273a 0a20 2020  word == '-':.   
 00015080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015090: 2020 2020 2020 7061 7373 776f 7264 093d        password.=
-000150a0: 2070 6173 7377 6f72 645f 7570 6461 7465   password_update
-000150b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000150c0: 2069 6620 7573 6572 7061 7373 5f75 7064   if userpass_upd
-000150d0: 6174 6564 3a0a 2020 2020 2020 2020 2020  ated:.          
-000150e0: 2020 2020 2020 2020 2020 6c6f 672e 6465            log.de
-000150f0: 7461 696c 2820 2253 7570 706c 7969 6e67  tail( "Supplying
-00015100: 206e 6577 2063 7265 6465 6e74 6961 6c73   new credentials
-00015110: 2066 6f72 207b 7d3a 207b 7d22 2e66 6f72   for {}: {}".for
-00015120: 6d61 7428 0a20 2020 2020 2020 2020 2020  mat(.           
-00015130: 2020 2020 2020 2020 2020 2020 2075 7365               use
-00015140: 726e 616d 6520 6f72 2022 286e 6f20 7573  rname or "(no us
-00015150: 6572 6e61 6d65 2922 2c20 272a 2720 2a20  ername)", '*' * 
-00015160: 6c65 6e28 2070 6173 7377 6f72 6420 6f72  len( password or
-00015170: 2027 2720 2920 6f72 2022 286e 6f20 7061   '' ) or "(no pa
-00015180: 7373 776f 7264 2922 2029 290a 2020 2020  ssword)" )).    
-00015190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000151a0: 6175 7468 6f72 697a 6174 696f 6e2e 7365  authorization.se
-000151b0: 6e64 2820 2875 7365 726e 616d 652c 7061  nd( (username,pa
-000151c0: 7373 776f 7264 2920 290a 2020 2020 2020  ssword) ).      
-000151d0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-000151e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000151f0: 2020 2020 6c6f 672e 6465 7461 696c 2820      log.detail( 
-00015200: 224e 6f20 6e65 7720 6372 6564 656e 7469  "No new credenti
-00015210: 616c 2873 2920 666f 7220 7b7d 3a20 7b7d  al(s) for {}: {}
-00015220: 7b7d 222e 666f 726d 6174 280a 2020 2020  {}".format(.    
-00015230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015240: 2020 2020 7573 6572 6e61 6d65 206f 7220      username or 
-00015250: 2228 6e6f 2075 7365 726e 616d 6529 222c  "(no username)",
-00015260: 2027 2a27 202a 206c 656e 2820 7061 7373   '*' * len( pass
-00015270: 776f 7264 206f 7220 2727 2029 206f 7220  word or '' ) or 
-00015280: 2228 6e6f 2070 6173 7377 6f72 6429 222c  "(no password)",
-00015290: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000152a0: 2020 2020 2020 2020 2022 2028 6174 7465           " (atte
-000152b0: 6d70 7469 6e67 2074 6f20 7265 6769 7374  mpting to regist
-000152c0: 6572 206e 6577 2041 6765 6e74 2049 4429  er new Agent ID)
-000152d0: 2220 6966 2061 7267 732e 7265 6769 7374  " if args.regist
-000152e0: 6572 2065 6c73 6520 2220 2861 7574 686f  er else " (autho
-000152f0: 7269 7a61 7469 6f6e 2066 6169 6c65 6429  rization failed)
-00015300: 2220 2929 0a20 2020 2020 2020 2020 2020  " )).           
-00015310: 2020 2020 2023 204e 6f20 4b65 7970 6169       # No Keypai
-00015320: 7220 286f 7220 7065 7268 6170 7320 6120  r (or perhaps a 
-00015330: 4b65 7970 6169 722c 2062 7574 206e 6f20  Keypair, but no 
-00015340: 4c69 6365 6e73 6529 2066 6f75 6e64 3b20  License) found; 
-00015350: 6d61 7962 6520 6372 6564 656e 7469 616c  maybe credential
-00015360: 7320 7570 6461 7465 640a 2020 2020 2020  s updated.      
-00015370: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
-00015380: 7565 0a20 2020 2020 2020 2020 2020 2023  ue.            #
-00015390: 2041 204b 6579 7061 6972 2061 6e64 204c   A Keypair and L
-000153a0: 6963 656e 7365 2077 6173 2066 6f75 6e64  icense was found
-000153b0: 3b20 7265 6d65 6d62 6572 2069 740a 2020  ; remember it.  
-000153c0: 2020 2020 2020 2020 2020 6c6f 6164 6564            loaded
-000153d0: 2e61 7070 656e 6428 2028 6b65 792c 6c69  .append( (key,li
-000153e0: 6329 2029 0a0a 2020 2020 2020 2020 2320  c) )..        # 
-000153f0: 436f 6c6c 6563 7420 7570 2061 6c6c 2074  Collect up all t
-00015400: 6865 204c 6963 656e 7365 2067 7261 6e74  he License grant
-00015410: 733b 2074 6865 7265 206d 6179 2062 6520  s; there may be 
-00015420: 6d6f 7265 2074 6861 6e20 6f6e 652c 2069  more than one, i
-00015430: 6620 7468 6520 7573 6572 2068 6173 2070  f the user has p
-00015440: 7572 6368 6173 6564 0a20 2020 2020 2020  urchased.       
-00015450: 2023 206d 756c 7469 706c 6520 4c69 6365   # multiple Lice
-00015460: 6e73 6573 2061 7420 6469 6666 6572 656e  nses at differen
-00015470: 7420 7469 6d65 732e 2020 456e 7375 7265  t times.  Ensure
-00015480: 7320 7765 206f 6e6c 7920 696e 636c 7564  s we only includ
-00015490: 6520 6120 7370 6563 6966 6963 204c 6963  e a specific Lic
-000154a0: 656e 7365 206f 6e63 652e 0a20 2020 2020  ense once..     
-000154b0: 2020 2067 7261 6e74 7309 0909 3d20 6c69     grants...= li
-000154c0: 6365 6e73 696e 672e 4772 616e 7428 290a  censing.Grant().
-000154d0: 2020 2020 2020 2020 6f6e 6365 0909 093d          once...=
-000154e0: 2073 6574 2829 0a20 2020 2020 2020 2066   set().        f
-000154f0: 6f72 206b 6579 2c6c 6963 2069 6e20 6c6f  or key,lic in lo
-00015500: 6164 6564 3a0a 2020 2020 2020 2020 2020  aded:.          
-00015510: 2020 6772 616e 7473 5f6c 6963 0909 3d20    grants_lic..= 
-00015520: 6c69 632e 6772 616e 7473 2820 6f6e 6365  lic.grants( once
-00015530: 3d6f 6e63 6520 290a 2020 2020 2020 2020  =once ).        
-00015540: 2020 2020 6c6f 672e 6e6f 726d 616c 2820      log.normal( 
-00015550: 224c 6f63 6174 6564 2041 6765 6e74 2045  "Located Agent E
-00015560: 6432 3535 3139 204b 6579 7061 6972 207b  d25519 Keypair {
-00015570: 7075 626b 6579 7d20 772f 207b 7072 6f64  pubkey} w/ {prod
-00015580: 7563 747d 204c 6963 656e 7365 2028 6672  uct} License (fr
-00015590: 6f6d 207b 5f66 726f 6d7d 297b 6578 7472  om {_from}){extr
-000155a0: 617d 222e 666f 726d 6174 280a 2020 2020  a}".format(.    
-000155b0: 2020 2020 2020 2020 2020 2020 7075 626b              pubk
-000155c0: 6579 093d 206c 6963 656e 7369 6e67 2e69  ey.= licensing.i
-000155d0: 6e74 6f5f 6236 3428 206b 6579 2e76 6b20  nto_b64( key.vk 
-000155e0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-000155f0: 2020 2070 726f 6475 6374 093d 206c 6963     product.= lic
-00015600: 2061 6e64 206c 6963 2e6c 6963 656e 7365   and lic.license
-00015610: 2e61 7574 686f 722e 7072 6f64 7563 7420  .author.product 
-00015620: 6f72 2022 456e 642d 5573 6572 222c 0a20  or "End-User",. 
-00015630: 2020 2020 2020 2020 2020 2020 2020 205f                 _
-00015640: 6672 6f6d 093d 2022 6672 6f6d 207b 7d22  from.= "from {}"
-00015650: 2e66 6f72 6d61 7428 206c 6963 2e5f 6672  .format( lic._fr
-00015660: 6f6d 2029 2069 6620 6c69 632e 5f66 726f  om ) if lic._fro
-00015670: 6d20 656c 7365 2022 6c6f 6361 6c6c 7920  m else "locally 
-00015680: 6973 7375 6564 222c 0a20 2020 2020 2020  issued",.       
-00015690: 2020 2020 2020 2020 2065 7874 7261 093d           extra.=
-000156a0: 2028 2820 2220 772f 2067 7261 6e74 733a   (( " w/ grants:
-000156b0: 207b 7d22 2e66 6f72 6d61 7428 2067 7261   {}".format( gra
-000156c0: 6e74 735f 6c69 6320 2920 6966 206c 6f67  nts_lic ) if log
-000156d0: 2e69 7345 6e61 626c 6564 466f 7228 206c  .isEnabledFor( l
-000156e0: 6f67 6769 6e67 2e44 4542 5547 2029 2065  ogging.DEBUG ) e
-000156f0: 6c73 6520 2222 2029 0a20 2020 2020 2020  lse "" ).       
-00015700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015710: 2020 2020 2b20 2820 2220 6d65 7267 696e      + ( " mergin
-00015720: 6720 772f 2067 7261 6e74 733a 207b 7d22  g w/ grants: {}"
-00015730: 2e66 6f72 6d61 7428 2067 7261 6e74 7320  .format( grants 
-00015740: 2920 6966 206c 6f67 2e69 7345 6e61 626c  ) if log.isEnabl
-00015750: 6564 466f 7228 206c 6f67 6769 6e67 2e54  edFor( logging.T
-00015760: 5241 4345 2029 2065 6c73 6520 2222 2029  RACE ) else "" )
-00015770: 292c 0a20 2020 2020 2020 2020 2020 2029  ),.            )
-00015780: 290a 2020 2020 2020 2020 2020 2020 6772  ).            gr
-00015790: 616e 7473 0920 2020 2020 2020 7c3d 2067  ants.       |= g
-000157a0: 7261 6e74 735f 6c69 630a 0a20 2020 2020  rants_lic..     
-000157b0: 2020 2023 2041 6e64 2c20 6669 6e61 6c6c     # And, finall
-000157c0: 793a 2061 7363 6572 7461 696e 2077 6865  y: ascertain whe
-000157d0: 7468 6572 2077 6520 6861 7665 2061 2047  ther we have a G
-000157e0: 7261 6e74 2074 6f20 7275 6e20 446f 6d69  rant to run Domi
-000157f0: 6e69 6f6e 2052 2644 2043 6f72 7027 7320  nion R&D Corp's 
-00015800: 4372 7970 746f 204c 6963 656e 7369 6e67  Crypto Licensing
-00015810: 2053 6572 7665 7221 0a20 2020 2020 2020   Server!.       
-00015820: 2061 7373 6572 7420 646f 6d69 6e69 6f6e   assert dominion
-00015830: 2e73 6572 7669 6365 6b65 7920 696e 2067  .servicekey in g
-00015840: 7261 6e74 732c 205c 0a20 2020 2020 2020  rants, \.       
-00015850: 2020 2020 2022 556e 6162 6c65 2074 6f20       "Unable to 
-00015860: 6669 6e64 207b 7d27 7320 7072 6f64 7563  find {}'s produc
-00015870: 7420 7b21 727d 2073 6572 7669 6365 206b  t {!r} service k
-00015880: 6579 207b 2172 7d20 696e 204c 6963 656e  ey {!r} in Licen
-00015890: 7365 2047 7261 6e74 7320 7b7d 222e 666f  se Grants {}".fo
-000158a0: 726d 6174 280a 2020 2020 2020 2020 2020  rmat(.          
-000158b0: 2020 2020 2020 646f 6d69 6e69 6f6e 2e6e        dominion.n
-000158c0: 616d 652c 2064 6f6d 696e 696f 6e2e 7072  ame, dominion.pr
-000158d0: 6f64 7563 742c 2064 6f6d 696e 696f 6e2e  oduct, dominion.
-000158e0: 7365 7276 6963 656b 6579 2c20 6772 616e  servicekey, gran
-000158f0: 7473 2029 0a0a 2020 2020 6578 6365 7074  ts )..    except
-00015900: 2045 7863 6570 7469 6f6e 2061 7320 6578   Exception as ex
-00015910: 633a 0a20 2020 2020 2020 206c 6f67 2e65  c:.        log.e
-00015920: 7272 6f72 2820 2246 6169 6c65 6420 6c6f  rror( "Failed lo
-00015930: 6164 696e 6720 4167 656e 7420 4b65 7970  ading Agent Keyp
-00015940: 6169 7220 616e 642f 6f72 204c 6963 656e  air and/or Licen
-00015950: 7365 3a20 7b65 7863 7d22 2e66 6f72 6d61  se: {exc}".forma
-00015960: 7428 0a20 2020 2020 2020 2020 2020 2065  t(.            e
-00015970: 7863 3d27 272e 6a6f 696e 2820 7472 6163  xc=''.join( trac
-00015980: 6562 6163 6b2e 666f 726d 6174 5f65 7863  eback.format_exc
-00015990: 6570 7469 6f6e 2820 2a73 7973 2e65 7863  eption( *sys.exc
-000159a0: 5f69 6e66 6f28 2920 2929 2069 6620 6c6f  _info() )) if lo
-000159b0: 672e 6973 456e 6162 6c65 6446 6f72 2820  g.isEnabledFor( 
-000159c0: 6c6f 6767 696e 672e 5452 4143 4520 2920  logging.TRACE ) 
-000159d0: 656c 7365 2065 7863 2029 290a 2020 2020  else exc )).    
-000159e0: 2020 2020 7769 7468 206f 7065 6e28 206f      with open( o
-000159f0: 732e 7061 7468 2e6a 6f69 6e28 206f 732e  s.path.join( os.
-00015a00: 7061 7468 2e64 6972 6e61 6d65 2820 5f5f  path.dirname( __
-00015a10: 6669 6c65 5f5f 2029 2c20 2773 7461 7469  file__ ), 'stati
-00015a20: 6327 2c20 2774 7874 272c 2027 434c 2d4b  c', 'txt', 'CL-K
-00015a30: 4559 5041 4952 2d4d 4953 5349 4e47 2e74  EYPAIR-MISSING.t
-00015a40: 7874 2720 292c 2027 7227 2029 2061 7320  xt' ), 'r' ) as 
-00015a50: 663a 0a20 2020 2020 2020 2020 2020 2070  f:.            p
-00015a60: 7269 6e74 2820 662e 7265 6164 2829 2e66  rint( f.read().f
-00015a70: 6f72 6d61 7428 0a20 2020 2020 2020 2020  ormat(.         
-00015a80: 2020 2020 2020 2044 4953 5452 4942 5554         DISTRIBUT
-00015a90: 494f 4e09 3d20 6c69 6365 6e73 696e 672e  ION.= licensing.
-00015aa0: 4449 5354 5249 4255 5449 4f4e 2c0a 2020  DISTRIBUTION,.  
-00015ab0: 2020 2020 2020 2020 2020 2020 2020 4b45                KE
-00015ac0: 5950 4154 5445 524e 093d 206c 6963 656e  YPATTERN.= licen
-00015ad0: 7369 6e67 2e4b 4559 5041 5454 4552 4e2c  sing.KEYPATTERN,
-00015ae0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015af0: 204c 4943 454e 5345 5f4f 5054 494f 4e09   LICENSE_OPTION.
-00015b00: 3d20 272d 2d6c 6963 656e 7365 272c 0a20  = '--license',. 
-00015b10: 2020 2020 2020 2020 2020 2029 2c20 6669             ), fi
-00015b20: 6c65 3d73 7973 2e73 7464 6572 7220 290a  le=sys.stderr ).
-00015b30: 2020 2020 2020 2020 7379 732e 6578 6974          sys.exit
-00015b40: 2820 3120 290a 0a20 2020 2023 2053 6574  ( 1 )..    # Set
-00015b50: 2075 7020 7468 6520 676c 6f62 616c 2064   up the global d
-00015b60: 622c 2065 7463 2e0a 2020 2020 6462 5f73  b, etc..    db_s
-00015b70: 6574 7570 2829 0a0a 2020 2020 2320 5375  etup()..    # Su
-00015b80: 6d6d 6172 697a 6520 7468 6520 696e 6974  mmarize the init
-00015b90: 6961 6c20 4c69 6365 6e73 6573 2061 6e64  ial Licenses and
-00015ba0: 204b 6579 7061 6972 7320 6176 6169 6c61   Keypairs availa
-00015bb0: 626c 653b 2074 6865 7365 2061 7265 2072  ble; these are r
-00015bc0: 652d 6f62 7461 696e 6564 2069 6e20 7265  e-obtained in re
-00015bd0: 616c 2d74 696d 6520 6279 2074 6865 2055  al-time by the U
-00015be0: 4973 2c20 6162 6f76 650a 2020 2020 7374  Is, above.    st
-00015bf0: 6f72 6564 0909 093d 2064 622e 7365 6c65  ored...= db.sele
-00015c00: 6374 2820 276c 6963 656e 7365 7327 2029  ct( 'licenses' )
-00015c10: 0a20 2020 2073 746f 7265 6409 0909 3d20  .    stored...= 
-00015c20: 6c69 7374 2820 7374 6f72 6564 2029 0a20  list( stored ). 
-00015c30: 2020 2066 6f72 2073 6967 2c20 6c69 6320     for sig, lic 
-00015c40: 696e 206c 6963 656e 7365 7328 2063 6f6e  in licenses( con
-00015c50: 6669 726d 3d46 616c 7365 2c20 7374 6f72  firm=False, stor
-00015c60: 6564 3d73 746f 7265 6420 293a 0a20 2020  ed=stored ):.   
-00015c70: 2020 2020 206c 6f67 2e69 6e66 6f28 2022       log.info( "
-00015c80: 7b73 3a3c 3634 7d3a 207b 6c69 637d 222e  {s:<64}: {lic}".
-00015c90: 666f 726d 6174 280a 2020 2020 2020 2020  format(.        
-00015ca0: 2020 2020 733d 6c69 6365 6e73 696e 672e      s=licensing.
-00015cb0: 696e 746f 5f62 3634 2820 7369 6720 292c  into_b64( sig ),
-00015cc0: 206c 6963 3d73 7472 2820 6c69 6320 2920   lic=str( lic ) 
-00015cd0: 2929 0a0a 2020 2020 666f 7220 6e61 6d65  ))..    for name
-00015ce0: 2c20 6b65 7970 6169 722c 2028 7573 6572  , keypair, (user
-00015cf0: 6e61 6d65 2c20 7061 7373 776f 7264 2920  name, password) 
-00015d00: 696e 206b 6579 7061 6972 7328 293a 0a20  in keypairs():. 
-00015d10: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
-00015d20: 2020 2020 2020 2020 766b 0909 093d 206c          vk...= l
-00015d30: 6963 656e 7369 6e67 2e69 6e74 6f5f 6236  icensing.into_b6
-00015d40: 3428 206b 6579 7061 6972 2e69 6e74 6f5f  4( keypair.into_
-00015d50: 6b65 7970 6169 7228 2075 7365 726e 616d  keypair( usernam
-00015d60: 653d 7573 6572 6e61 6d65 2c20 7061 7373  e=username, pass
-00015d70: 776f 7264 3d70 6173 7377 6f72 6420 292e  word=password ).
-00015d80: 766b 2029 0a20 2020 2020 2020 2065 7863  vk ).        exc
-00015d90: 6570 7420 4578 6365 7074 696f 6e20 6173  ept Exception as
-00015da0: 2065 7863 3a0a 2020 2020 2020 2020 2020   exc:.          
-00015db0: 2020 766b 0909 093d 2073 7472 2820 6578    vk...= str( ex
-00015dc0: 6320 290a 2020 2020 2020 2020 6c6f 672e  c ).        log.
-00015dd0: 696e 666f 2820 227b 6e3a 3c32 307d 3a20  info( "{n:<20}: 
-00015de0: 7b76 6b7d 2077 2f20 7b75 3a3e 3230 7d20  {vk} w/ {u:>20} 
-00015df0: 2f20 7b70 7d22 2e66 6f72 6d61 7428 0a20  / {p}".format(. 
-00015e00: 2020 2020 2020 2020 2020 206e 3d6e 616d             n=nam
-00015e10: 652c 2076 6b3d 766b 2c20 753d 7573 6572  e, vk=vk, u=user
-00015e20: 6e61 6d65 2c20 703d 272a 2720 2a20 6c65  name, p='*' * le
-00015e30: 6e28 2070 6173 7377 6f72 6420 2929 290a  n( password ))).
-00015e40: 0a20 2020 2063 6c61 7373 2064 6165 6d6f  .    class daemo
-00015e50: 6e28 2074 6872 6561 6469 6e67 2e54 6872  n( threading.Thr
-00015e60: 6561 6420 293a 0a20 2020 2020 2020 2022  ead ):.        "
-00015e70: 2222 4576 6572 7920 6461 656d 6f6e 206d  ""Every daemon m
-00015e80: 7573 7420 6861 7665 2061 2063 6f6e 6669  ust have a confi
-00015e90: 675b 2763 6f6e 7472 6f6c 275d 3b20 7365  g['control']; se
-00015ea0: 7473 2069 7473 2064 6f6e 6520 3d20 5472  ts its done = Tr
-00015eb0: 7565 2074 6f20 7374 6f70 2e22 2222 0a20  ue to stop.""". 
-00015ec0: 2020 2020 2020 2064 6566 205f 5f69 6e69         def __ini
-00015ed0: 745f 5f28 2073 656c 662c 2063 6f6e 6669  t__( self, confi
-00015ee0: 673d 4e6f 6e65 2c20 2a2a 6b77 6473 2029  g=None, **kwds )
-00015ef0: 3a0a 2020 2020 2020 2020 2020 2020 7375  :.            su
-00015f00: 7065 7228 2064 6165 6d6f 6e2c 2073 656c  per( daemon, sel
-00015f10: 6620 292e 5f5f 696e 6974 5f5f 2820 2a2a  f ).__init__( **
-00015f20: 6b77 6473 2029 0a20 2020 2020 2020 2020  kwds ).         
-00015f30: 2020 2073 656c 662e 6461 656d 6f6e 0909     self.daemon..
-00015f40: 3d20 5472 7565 0a20 2020 2020 2020 2020  = True.         
-00015f50: 2020 2073 656c 662e 636f 6e66 6967 0909     self.config..
-00015f60: 3d20 636f 6e66 6967 206f 7220 7b7d 0a20  = config or {}. 
-00015f70: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00015f80: 636f 6e66 6967 2e73 6574 6465 6661 756c  config.setdefaul
-00015f90: 7428 2027 636f 6e74 726f 6c27 2c20 7b7d  t( 'control', {}
-00015fa0: 2029 2e73 6574 6465 6661 756c 7428 2027   ).setdefault( '
-00015fb0: 646f 6e65 272c 2046 616c 7365 2029 0a0a  done', False )..
-00015fc0: 2020 2020 2020 2020 6465 6620 7374 6f70          def stop
-00015fd0: 2820 7365 6c66 2029 3a0a 2020 2020 2020  ( self ):.      
-00015fe0: 2020 2020 2020 6c6f 6767 696e 672e 696e        logging.in
-00015ff0: 666f 2820 2253 746f 7070 696e 6720 2573  fo( "Stopping %s
-00016000: 2054 6872 6561 6422 2c20 7365 6c66 2e6e   Thread", self.n
-00016010: 616d 6520 290a 2020 2020 2020 2020 2020  ame ).          
-00016020: 2020 7365 6c66 2e63 6f6e 6669 675b 2763    self.config['c
-00016030: 6f6e 7472 6f6c 275d 5b27 646f 6e65 275d  ontrol']['done']
-00016040: 203d 2054 7275 650a 0a20 2020 2020 2020   = True..       
-00016050: 2064 6566 206a 6f69 6e28 2073 656c 662c   def join( self,
-00016060: 202a 6172 6773 2c20 2a2a 6b77 6473 2029   *args, **kwds )
-00016070: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00016080: 6c66 2e73 746f 7028 290a 2020 2020 2020  lf.stop().      
-00016090: 2020 2020 2020 6c6f 6767 696e 672e 696e        logging.in
-000160a0: 666f 2820 224a 6f69 6e69 6e67 2025 7320  fo( "Joining %s 
-000160b0: 5468 7265 6164 2e2e 2e22 2c20 7365 6c66  Thread...", self
-000160c0: 2e6e 616d 6520 290a 2020 2020 2020 2020  .name ).        
-000160d0: 2020 2020 7375 7065 7228 2064 6165 6d6f      super( daemo
-000160e0: 6e2c 2073 656c 6620 292e 6a6f 696e 2820  n, self ).join( 
-000160f0: 2a61 7267 732c 202a 2a6b 7764 7320 290a  *args, **kwds ).
-00016100: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
-00016110: 696e 672e 696e 666f 2820 224a 6f69 6e65  ing.info( "Joine
-00016120: 6420 2573 2054 6872 6561 6422 2c20 7365  d %s Thread", se
-00016130: 6c66 2e6e 616d 6520 290a 0a20 2020 2063  lf.name )..    c
-00016140: 6c61 7373 2074 7874 7468 7265 6164 2820  lass txtthread( 
-00016150: 6461 656d 6f6e 2029 3a0a 2020 2020 2020  daemon ):.      
-00016160: 2020 6465 6620 7275 6e28 2073 656c 6620    def run( self 
-00016170: 293a 0a20 2020 2020 2020 2020 2020 2074  ):.            t
-00016180: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-00016190: 2020 2020 7768 696c 6520 6e6f 7420 7365      while not se
-000161a0: 6c66 2e63 6f6e 6669 672e 6765 7428 2027  lf.config.get( '
-000161b0: 636f 6e74 726f 6c27 2c20 7b7d 2029 2e67  control', {} ).g
-000161c0: 6574 2820 2764 6f6e 6527 2029 3a0a 2020  et( 'done' ):.  
-000161d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000161e0: 2020 6966 2074 7874 6775 6928 2073 656c    if txtgui( sel
-000161f0: 662e 636f 6e66 6967 2029 3a0a 2020 2020  f.config ):.    
-00016200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016210: 2020 2020 2320 5465 7874 7561 6c20 4755      # Textual GU
-00016220: 4920 6861 7320 6661 696c 6564 2120 2044  I has failed!  D
-00016230: 6f6e 2774 2072 6573 7461 7274 2e0a 2020  on't restart..  
-00016240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016250: 2020 2020 2020 6272 6561 6b0a 2020 2020        break.    
-00016260: 2020 2020 2020 2020 6578 6365 7074 2045          except E
-00016270: 7863 6570 7469 6f6e 2061 7320 6578 633a  xception as exc:
-00016280: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016290: 206c 6f67 6769 6e67 2e65 7272 6f72 2822   logging.error("
-000162a0: 5465 7874 2047 5549 2066 6169 6c65 643a  Text GUI failed:
-000162b0: 2025 735c 6e25 7322 2c20 6578 632c 2074   %s\n%s", exc, t
-000162c0: 7261 6365 6261 636b 2e66 6f72 6d61 745f  raceback.format_
-000162d0: 6578 6328 2929 0a20 2020 2020 2020 2020  exc()).         
-000162e0: 2020 2066 696e 616c 6c79 3a0a 2020 2020     finally:.    
-000162f0: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
-00016300: 696e 672e 7761 726e 696e 6728 2022 5465  ing.warning( "Te
-00016310: 7874 2047 5549 2065 7869 7469 6e67 2220  xt GUI exiting" 
-00016320: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00016330: 2020 7365 6c66 2e73 746f 7028 290a 0a20    self.stop().. 
-00016340: 2020 2063 6c61 7373 2077 6562 7468 7265     class webthre
-00016350: 6164 2820 6461 656d 6f6e 2029 3a0a 2020  ad( daemon ):.  
-00016360: 2020 2020 2020 6465 6620 7275 6e28 2073        def run( s
-00016370: 656c 6620 293a 0a20 2020 2020 2020 2020  elf ):.         
-00016380: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-00016390: 2020 2020 2020 2020 7765 6270 7928 2073          webpy( s
-000163a0: 656c 662e 636f 6e66 6967 2029 0a20 2020  elf.config ).   
-000163b0: 2020 2020 2020 2020 2065 7863 6570 7420           except 
-000163c0: 4578 6365 7074 696f 6e20 6173 2065 7863  Exception as exc
-000163d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000163e0: 2020 6c6f 6767 696e 672e 6572 726f 7228    logging.error(
-000163f0: 2022 5765 6220 4755 4920 6661 696c 6564   "Web GUI failed
-00016400: 3a20 2573 5c6e 2573 222c 2065 7863 2c20  : %s\n%s", exc, 
-00016410: 7472 6163 6562 6163 6b2e 666f 726d 6174  traceback.format
-00016420: 5f65 7863 2829 2029 0a20 2020 2020 2020  _exc() ).       
-00016430: 2020 2020 2066 696e 616c 6c79 3a0a 2020       finally:.  
-00016440: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00016450: 6c66 2e73 746f 7028 290a 2020 2020 2020  lf.stop().      
-00016460: 2020 2020 2020 2020 2020 6c6f 6767 696e            loggin
-00016470: 672e 7761 726e 696e 6728 2022 5765 6220  g.warning( "Web 
-00016480: 4755 4920 6578 6974 696e 6722 2029 0a0a  GUI exiting" )..
-00016490: 2020 2020 2020 2020 6465 6620 7374 6f70          def stop
-000164a0: 2820 7365 6c66 2029 3a0a 2020 2020 2020  ( self ):.      
-000164b0: 2020 2020 2020 2222 2249 6e20 6164 6469        """In addi
-000164c0: 7469 6f6e 2074 6f20 7468 6520 6e6f 726d  tion to the norm
-000164d0: 616c 2073 746f 7020 7072 6f63 6564 7572  al stop procedur
-000164e0: 6520 2870 6572 6861 7073 2073 6967 6e61  e (perhaps signa
-000164f0: 6c69 6e67 206f 7468 6572 2054 6872 6561  ling other Threa
-00016500: 6473 2076 6961 2061 2073 6861 7265 640a  ds via a shared.
-00016510: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
-00016520: 726f 6c20 6469 6374 292c 2077 6562 7079  rol dict), webpy
-00016530: 2e73 6572 7665 7220 6861 7320 6974 7320  .server has its 
-00016540: 6f77 6e20 7374 6f70 206d 6563 6861 6e69  own stop mechani
-00016550: 736d 2e0a 0a20 2020 2020 2020 2020 2020  sm...           
-00016560: 2022 2222 0a20 2020 2020 2020 2020 2020   """.           
-00016570: 2073 7570 6572 2820 7765 6274 6872 6561   super( webthrea
-00016580: 642c 2073 656c 6620 292e 7374 6f70 2829  d, self ).stop()
-00016590: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000165a0: 7765 6270 792e 7365 7276 6572 3a0a 2020  webpy.server:.  
-000165b0: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-000165c0: 6767 696e 672e 696e 666f 2820 2257 6562  gging.info( "Web
-000165d0: 2047 5549 2073 746f 7070 696e 672e 2e2e   GUI stopping...
-000165e0: 2220 290a 2020 2020 2020 2020 2020 2020  " ).            
-000165f0: 2020 2020 7765 6270 792e 7365 7276 6572      webpy.server
-00016600: 2e73 746f 7028 290a 2020 2020 2020 2020  .stop().        
-00016610: 2020 2020 2020 2020 6c6f 6767 696e 672e          logging.
-00016620: 696e 666f 2820 2257 6562 2047 5549 2073  info( "Web GUI s
-00016630: 746f 7070 6564 2220 290a 0a20 2020 2063  topped" )..    c
-00016640: 6c61 7373 2063 746c 7468 7265 6164 2820  lass ctlthread( 
-00016650: 6461 656d 6f6e 2029 3a0a 2020 2020 2020  daemon ):.      
-00016660: 2020 6465 6620 7275 6e28 2073 656c 6620    def run( self 
-00016670: 293a 0a20 2020 2020 2020 2020 2020 2074  ):.            t
-00016680: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-00016690: 2020 2020 7768 696c 6520 6e6f 7420 7365      while not se
-000166a0: 6c66 2e63 6f6e 6669 672e 6765 7428 2027  lf.config.get( '
-000166b0: 636f 6e74 726f 6c27 2c20 7b7d 2029 2e67  control', {} ).g
-000166c0: 6574 2820 2764 6f6e 6527 2029 3a0a 2020  et( 'done' ):.  
-000166d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000166e0: 2020 6265 6709 093d 2074 696d 6572 2829    beg..= timer()
-000166f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016700: 2020 2020 2063 746c 6c6f 6f70 2820 6265       ctlloop( be
-00016710: 672c 2073 656c 662e 636f 6e66 6967 2029  g, self.config )
-00016720: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016730: 2020 2020 2064 7572 0909 3d20 7469 6d65       dur..= time
-00016740: 7228 2920 2d20 6265 670a 2020 2020 2020  r() - beg.      
-00016750: 2020 2020 2020 2020 2020 2020 2020 6379                cy
-00016760: 6309 093d 2073 656c 662e 636f 6e66 6967  c..= self.config
-00016770: 2e67 6574 2820 2763 7963 6c65 272c 2031  .get( 'cycle', 1
-00016780: 2e30 2029 0a20 2020 2020 2020 2020 2020  .0 ).           
-00016790: 2020 2020 2020 2020 2069 6620 6475 7220           if dur 
-000167a0: 3c20 6379 633a 0a20 2020 2020 2020 2020  < cyc:.         
-000167b0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-000167c0: 696d 652e 736c 6565 7028 2063 7963 202d  ime.sleep( cyc -
-000167d0: 2064 7572 2029 0a20 2020 2020 2020 2020   dur ).         
-000167e0: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
-000167f0: 696f 6e20 6173 2065 7863 3a0a 2020 2020  ion as exc:.    
-00016800: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
-00016810: 696e 672e 6572 726f 7228 2022 436f 6e74  ing.error( "Cont
-00016820: 726f 6c20 7379 7374 656d 2066 6169 6c65  rol system faile
-00016830: 643a 2025 735c 6e25 7322 2c20 6578 632c  d: %s\n%s", exc,
-00016840: 2074 7261 6365 6261 636b 2e66 6f72 6d61   traceback.forma
-00016850: 745f 6578 6328 2920 290a 2020 2020 2020  t_exc() ).      
-00016860: 2020 2020 2020 6669 6e61 6c6c 793a 0a20        finally:. 
-00016870: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00016880: 6f67 6769 6e67 2e77 6172 6e69 6e67 2820  ogging.warning( 
-00016890: 2243 6f6e 7472 6f6c 2073 7973 7465 6d20  "Control system 
-000168a0: 6578 6974 696e 6722 2029 0a20 2020 2020  exiting" ).     
-000168b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000168c0: 7374 6f70 2829 0a0a 2020 2020 2320 536f  stop()..    # So
-000168d0: 6d65 206f 6620 7468 6573 6520 7468 7265  me of these thre
-000168e0: 6164 7320 6d61 7920 6e65 6564 2074 6f20  ads may need to 
-000168f0: 7265 6469 7265 6374 2073 7973 2e73 7464  redirect sys.std
-00016900: 6f75 742f 7374 6465 7272 3b20 7361 7665  out/stderr; save
-00016910: 2061 6e64 2072 6573 746f 7265 0a20 2020   and restore.   
-00016920: 2073 7973 5f73 7472 6561 6d5f 7361 7665   sys_stream_save
-00016930: 0909 3d20 7379 732e 7374 646f 7574 2c20  ..= sys.stdout, 
-00016940: 7379 732e 7374 6465 7272 0a20 2020 2074  sys.stderr.    t
-00016950: 6872 6561 6473 0909 093d 205b 5d0a 0a20  hreads...= [].. 
-00016960: 2020 2073 6572 7665 7209 0909 3d20 6c69     server...= li
-00016970: 6365 6e73 696e 675f 6b77 6473 2e70 6f70  censing_kwds.pop
-00016980: 2820 2773 6572 7665 7227 2c20 7b7d 2029  ( 'server', {} )
-00016990: 0a20 2020 2063 6f6e 7472 6f6c 0909 093d  .    control...=
-000169a0: 2073 6572 7665 722e 706f 7028 2027 636f   server.pop( 'co
-000169b0: 6e74 726f 6c27 2c20 7b7d 2029 0a20 2020  ntrol', {} ).   
-000169c0: 2074 7279 3a0a 2020 2020 2020 2020 2320   try:.        # 
-000169d0: 5374 6172 7420 7468 6520 636f 6e74 726f  Start the contro
-000169e0: 6c20 7379 7374 656d 2054 6872 6561 642e  l system Thread.
-000169f0: 0a20 2020 2020 2020 2063 746c 636e 6609  .        ctlcnf.
-00016a00: 0909 3d20 6c69 6365 6e73 696e 675f 6b77  ..= licensing_kw
-00016a10: 6473 2e70 6f70 2820 2763 746c 272c 207b  ds.pop( 'ctl', {
-00016a20: 7d20 290a 2020 2020 2020 2020 6374 6c63  } ).        ctlc
-00016a30: 6e66 2e73 6574 6465 6661 756c 7428 2027  nf.setdefault( '
-00016a40: 6379 636c 6527 2c20 312e 3020 290a 2020  cycle', 1.0 ).  
-00016a50: 2020 2020 2020 6374 6c63 6e66 2e73 6574        ctlcnf.set
-00016a60: 6465 6661 756c 7428 2027 636f 6e74 726f  default( 'contro
-00016a70: 6c27 2c20 636f 6e74 726f 6c20 290a 2020  l', control ).  
-00016a80: 2020 2020 2020 6374 6c74 6872 0909 093d        ctlthr...=
-00016a90: 2063 746c 7468 7265 6164 2820 636f 6e66   ctlthread( conf
-00016aa0: 6967 3d63 746c 636e 662c 206e 616d 653d  ig=ctlcnf, name=
-00016ab0: 2763 6f6e 7472 6f6c 2720 290a 2020 2020  'control' ).    
-00016ac0: 2020 2020 6374 6c74 6872 2e73 7461 7274      ctlthr.start
-00016ad0: 2829 0a20 2020 2020 2020 2074 6872 6561  ().        threa
-00016ae0: 6473 2e61 7070 656e 6428 2063 746c 7468  ds.append( ctlth
-00016af0: 7220 290a 0a20 2020 2020 2020 2023 2053  r )..        # S
-00016b00: 7461 7274 2074 6865 2043 7572 7365 7320  tart the Curses 
-00016b10: 5465 7874 2047 5549 2028 6966 2064 6573  Text GUI (if des
-00016b20: 6972 6564 290a 2020 2020 2020 2020 7478  ired).        tx
-00016b30: 7463 6e66 0909 093d 206c 6963 656e 7369  tcnf...= licensi
-00016b40: 6e67 5f6b 7764 732e 706f 7028 2027 7478  ng_kwds.pop( 'tx
-00016b50: 7427 2c20 7b7d 2029 0a20 2020 2020 2020  t', {} ).       
-00016b60: 2074 7874 636e 662e 7365 7464 6566 6175   txtcnf.setdefau
-00016b70: 6c74 2820 2763 6f6e 7472 6f6c 272c 2063  lt( 'control', c
-00016b80: 6f6e 7472 6f6c 2029 0a20 2020 2020 2020  ontrol ).       
-00016b90: 2074 7874 636e 662e 7365 7464 6566 6175   txtcnf.setdefau
-00016ba0: 6c74 2820 2774 6974 6c65 272c 2027 4c69  lt( 'title', 'Li
-00016bb0: 6365 6e73 696e 6727 2029 0a20 2020 2020  censing' ).     
-00016bc0: 2020 2023 2042 7920 6465 6661 756c 742c     # By default,
-00016bd0: 2061 6363 6573 7365 7320 7468 6520 6c6f   accesses the lo
-00016be0: 6361 6c20 6675 6e63 7469 6f6e 7320 7969  cal functions yi
-00016bf0: 656c 6469 6e67 2074 6865 2073 746f 7265  elding the store
-00016c00: 6420 6c69 6365 6e73 6573 2c20 6372 6564  d licenses, cred
-00016c10: 656e 7469 616c 7320 616e 6420 6b65 7970  entials and keyp
-00016c20: 6169 7273 0a20 2020 2020 2020 2074 7874  airs.        txt
-00016c30: 636e 662e 7365 7464 6566 6175 6c74 2820  cnf.setdefault( 
-00016c40: 276c 6963 656e 7365 7327 2c09 096c 6963  'licenses',..lic
-00016c50: 656e 7365 7320 290a 2020 2020 2020 2020  enses ).        
-00016c60: 7478 7463 6e66 2e73 6574 6465 6661 756c  txtcnf.setdefaul
-00016c70: 7428 2027 6372 6564 656e 7469 616c 7327  t( 'credentials'
-00016c80: 2c09 6372 6564 656e 7469 616c 7320 290a  ,.credentials ).
-00016c90: 2020 2020 2020 2020 7478 7463 6e66 2e73          txtcnf.s
-00016ca0: 6574 6465 6661 756c 7428 2027 6b65 7970  etdefault( 'keyp
-00016cb0: 6169 7273 272c 0909 6b65 7970 6169 7273  airs',..keypairs
-00016cc0: 2029 0a20 2020 2020 2020 2074 7874 7468   ).        txtth
-00016cd0: 7209 0909 3d20 4e6f 6e65 0a20 2020 2020  r...= None.     
-00016ce0: 2020 2069 6620 6172 6773 2e67 7569 3a0a     if args.gui:.
-00016cf0: 2020 2020 2020 2020 2020 2020 7478 7474              txtt
-00016d00: 6872 0909 3d20 7478 7474 6872 6561 6428  hr..= txtthread(
-00016d10: 2074 7874 636e 662c 206e 616d 653d 2763   txtcnf, name='c
-00016d20: 7572 7365 7327 2029 0a20 2020 2020 2020  urses' ).       
-00016d30: 2020 2020 2074 7874 7468 722e 7374 6172       txtthr.star
-00016d40: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
-00016d50: 7468 7265 6164 732e 6170 7065 6e64 2820  threads.append( 
-00016d60: 7478 7474 6872 2029 0a0a 2020 2020 2020  txtthr )..      
-00016d70: 2020 2320 5374 6172 7420 7468 6520 7765    # Start the we
-00016d80: 6220 5549 2028 6966 2064 6573 6972 6564  b UI (if desired
-00016d90: 290a 2020 2020 2020 2020 7765 6274 6872  ).        webthr
-00016da0: 0909 093d 204e 6f6e 650a 2020 2020 2020  ...= None.      
-00016db0: 2020 6966 2061 7267 732e 7765 623a 0a20    if args.web:. 
-00016dc0: 2020 2020 2020 2020 2020 2023 2044 6564             # Ded
-00016dd0: 7563 6520 696e 7465 7266 6163 653a 706f  uce interface:po
-00016de0: 7274 2074 6f20 6269 6e64 2c20 616e 6420  rt to bind, and 
-00016df0: 636f 7272 6563 7420 7479 7065 730a 2020  correct types.  
-00016e00: 2020 2020 2020 2020 2020 6164 6472 6573            addres
-00016e10: 7309 093d 2061 7267 732e 7765 622e 7370  s..= args.web.sp
-00016e20: 6c69 7428 2027 3a27 2029 0a20 2020 2020  lit( ':' ).     
-00016e30: 2020 2020 2020 2061 7373 6572 7420 3120         assert 1 
-00016e40: 3c3d 206c 656e 2820 6164 6472 6573 7320  <= len( address 
-00016e50: 2920 3c3d 2032 2c20 2257 6562 2061 6464  ) <= 2, "Web add
-00016e60: 7265 7373 206d 7573 7420 6265 2069 6e20  ress must be in 
-00016e70: 7468 6520 666f 726d 203c 696e 7465 7266  the form <interf
-00016e80: 6163 653e 3a3c 706f 7274 3e22 0a20 2020  ace>:<port>".   
-00016e90: 2020 2020 2020 2020 2061 6464 7265 7373           address
-00016ea0: 0909 3d20 2820 7374 7228 2061 6464 7265  ..= ( str( addre
-00016eb0: 7373 5b30 5d20 292c 0a20 2020 2020 2020  ss[0] ),.       
-00016ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ed0: 2020 2020 2020 2020 2020 2020 2069 6e74               int
-00016ee0: 2820 6164 6472 6573 735b 315d 2029 2069  ( address[1] ) i
-00016ef0: 6620 6c65 6e28 2061 6464 7265 7373 2029  f len( address )
-00016f00: 203e 2031 2065 6c73 6520 3830 3030 2029   > 1 else 8000 )
-00016f10: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-00016f20: 436f 6d6d 616e 642d 6c69 6e65 2070 6172  Command-line par
-00016f30: 616d 6574 6572 7320 696e 2061 7267 7620  ameters in argv 
-00016f40: 6172 6520 6f76 6572 7269 6464 656e 2062  are overridden b
-00016f50: 7920 7370 6563 6966 6963 2063 6f6e 6669  y specific confi
-00016f60: 6775 7261 7469 6f6e 730a 2020 2020 2020  gurations.      
-00016f70: 2020 2020 2020 2320 7061 7373 6564 2069        # passed i
-00016f80: 6e20 6c69 6365 6e73 696e 675f 6b77 6473  n licensing_kwds
-00016f90: 5b27 7765 6227 5d0a 2020 2020 2020 2020  ['web'].        
-00016fa0: 2020 2020 7765 6263 6e66 0909 3d20 6c69      webcnf..= li
-00016fb0: 6365 6e73 696e 675f 6b77 6473 2e70 6f70  censing_kwds.pop
-00016fc0: 2820 2777 6562 272c 207b 7d20 290a 2020  ( 'web', {} ).  
-00016fd0: 2020 2020 2020 2020 2020 7765 6263 6e66            webcnf
-00016fe0: 2e73 6574 6465 6661 756c 7428 2027 636f  .setdefault( 'co
-00016ff0: 6e74 726f 6c27 2c20 636f 6e74 726f 6c20  ntrol', control 
-00017000: 290a 2020 2020 2020 2020 2020 2020 7765  ).            we
-00017010: 6263 6e66 2e73 6574 6465 6661 756c 7428  bcnf.setdefault(
-00017020: 2027 6164 6472 6573 7327 2c20 6164 6472   'address', addr
-00017030: 6573 7320 290a 2020 2020 2020 2020 2020  ess ).          
-00017040: 2020 7765 6263 6e66 2e73 6574 6465 6661    webcnf.setdefa
-00017050: 756c 7428 2027 6163 6365 7373 272c 2061  ult( 'access', a
-00017060: 7267 732e 6163 6365 7373 2029 0a0a 2020  rgs.access )..  
-00017070: 2020 2020 2020 2020 2020 2320 4966 2061            # If a
-00017080: 6c6c 2073 7973 2e73 7464 6f75 742f 7374  ll sys.stdout/st
-00017090: 6465 7272 2073 686f 756c 6420 676f 7420  derr should got 
-000170a0: 746f 2074 6865 2077 6562 2073 6572 7665  to the web serve
-000170b0: 7227 7320 6163 6365 7373 206c 6f67 2066  r's access log f
-000170c0: 696c 652c 2028 7468 650a 2020 2020 2020  ile, (the.      
-000170d0: 2020 2020 2020 2320 6465 6661 756c 7429        # default)
-000170e0: 2c20 7468 656e 2073 6574 2069 7420 6865  , then set it he
-000170f0: 7265 2e20 2049 6620 6e6f 7420 2865 672e  re.  If not (eg.
-00017100: 2077 6520 7761 6e74 2074 6f20 6265 2061   we want to be a
-00017110: 626c 6520 746f 2068 6172 7665 7374 2074  ble to harvest t
-00017120: 6865 2061 6374 7561 6c0a 2020 2020 2020  he actual.      
-00017130: 2020 2020 2020 2320 6479 6e61 6d69 6320        # dynamic 
-00017140: 4950 2061 6464 7265 7373 3a70 6f72 7420  IP address:port 
-00017150: 6f66 2074 6865 2062 6f75 6e64 2077 6562  of the bound web
-00017160: 2073 6572 7665 7220 736f 636b 6574 292c   server socket),
-00017170: 2074 6865 6e20 7061 7373 2046 616c 7365   then pass False
-00017180: 7920 666f 7220 6163 6365 7373 2e0a 2020  y for access..  
-00017190: 2020 2020 2020 2020 2020 7765 6274 6872            webthr
-000171a0: 0909 3d20 7765 6274 6872 6561 6428 2077  ..= webthread( w
-000171b0: 6562 636e 662c 2020 6e61 6d65 3d27 7765  ebcnf,  name='we
-000171c0: 6227 2029 0a20 2020 2020 2020 2020 2020  b' ).           
-000171d0: 2077 6562 7468 722e 7374 6172 7428 290a   webthr.start().
-000171e0: 2020 2020 2020 2020 2020 2020 7468 7265              thre
-000171f0: 6164 732e 6170 7065 6e64 2820 7765 6274  ads.append( webt
-00017200: 6872 2029 0a0a 2020 2020 2020 2020 2320  hr )..        # 
-00017210: 4a75 7374 2077 6169 7420 666f 7220 616e  Just wait for an
-00017220: 7920 7468 7265 6164 2028 7765 6220 6f72  y thread (web or
-00017230: 2074 6578 7420 4755 492c 2063 6f6e 7472   text GUI, contr
-00017240: 6f6c 2920 746f 2066 696e 6973 680a 2020  ol) to finish.  
-00017250: 2020 2020 2020 7768 696c 6520 6e6f 7420        while not 
-00017260: 7368 7574 646f 776e 5f73 6967 6e61 6c6c  shutdown_signall
-00017270: 6564 2061 6e64 2061 6c6c 2820 742e 6973  ed and all( t.is
-00017280: 5f61 6c69 7665 2829 2066 6f72 2074 2069  _alive() for t i
-00017290: 6e20 7468 7265 6164 7320 293a 0a20 2020  n threads ):.   
-000172a0: 2020 2020 2020 2020 2073 6967 6e61 6c5f           signal_
-000172b0: 7365 7276 6963 6528 290a 2020 2020 2020  service().      
-000172c0: 2020 2020 2020 7469 6d65 2e73 6c65 6570        time.sleep
-000172d0: 2820 2e31 2029 0a20 2020 2065 7863 6570  ( .1 ).    excep
-000172e0: 7420 4578 6365 7074 696f 6e3a 0a20 2020  t Exception:.   
-000172f0: 2020 2020 206c 6f67 6769 6e67 2e65 7272       logging.err
-00017300: 6f72 2820 224d 6169 6e20 7468 7265 6164  or( "Main thread
-00017310: 2045 7863 6570 7469 6f6e 3a20 2573 222c   Exception: %s",
-00017320: 2074 7261 6365 6261 636b 2e66 6f72 6d61   traceback.forma
-00017330: 745f 6578 6328 2920 290a 2020 2020 6669  t_exc() ).    fi
-00017340: 6e61 6c6c 793a 0a20 2020 2020 2020 2023  nally:.        #
-00017350: 2045 6974 6865 7220 7468 6520 5765 6220   Either the Web 
-00017360: 6f72 2074 6865 2043 7572 7365 7320 4755  or the Curses GU
-00017370: 4920 636f 6d70 6c65 7465 642c 206f 7220  I completed, or 
-00017380: 736f 6d65 7468 696e 6720 626c 6577 2075  something blew u
-00017390: 702e 2020 5368 7574 2061 6c6c 2074 6865  p.  Shut all the
-000173a0: 0a20 2020 2020 2020 2023 2074 6872 6561  .        # threa
-000173b0: 6473 2064 6f77 6e2c 2072 6573 746f 7265  ds down, restore
-000173c0: 2073 7973 2e73 7464 6f75 742f 7374 6465   sys.stdout/stde
-000173d0: 7272 2061 6e64 2073 6176 6520 7374 6174  rr and save stat
-000173e0: 652e 0a20 2020 2020 2020 206c 6f67 6769  e..        loggi
-000173f0: 6e67 2e77 6172 6e69 6e67 2820 2243 6c65  ng.warning( "Cle
-00017400: 616e 696e 6720 7570 2074 6872 6561 6473  aning up threads
-00017410: 2220 290a 2020 2020 2020 2020 666f 7220  " ).        for 
-00017420: 7420 696e 2074 6872 6561 6473 3a0a 2020  t in threads:.  
-00017430: 2020 2020 2020 2020 2020 742e 6a6f 696e            t.join
-00017440: 2820 7469 6d65 6f75 743d 312e 3020 290a  ( timeout=1.0 ).
-00017450: 2020 2020 2020 2020 7379 732e 7374 646f          sys.stdo
-00017460: 7574 2c20 7379 732e 7374 6465 7272 093d  ut, sys.stderr.=
-00017470: 2073 7973 5f73 7472 6561 6d5f 7361 7665   sys_stream_save
-00017480: 0a0a 2020 2020 2020 2020 6c6f 6767 696e  ..        loggin
-00017490: 672e 696e 666f 2820 2253 6176 696e 6720  g.info( "Saving 
-000174a0: 7374 6174 652e 2e2e 2220 290a 2020 2020  state..." ).    
-000174b0: 2020 2020 6462 5f73 7461 7465 5f73 6176      db_state_sav
-000174c0: 6528 290a 0a20 2020 2020 2020 2069 6620  e()..        if 
-000174d0: 6172 6773 2e70 726f 6669 6c65 3a0a 2020  args.profile:.  
-000174e0: 2020 2020 2020 2020 2020 7072 6f66 696c            profil
-000174f0: 6572 2e64 6973 6162 6c65 2829 0a20 2020  er.disable().   
-00017500: 2020 2020 2020 2020 2069 6620 6172 6773           if args
-00017510: 2e70 726f 6669 6c65 2021 3d20 272d 273a  .profile != '-':
-00017520: 2020 2320 6f70 7469 6f6e 616c 6c79 2064    # optionally d
-00017530: 756d 7020 7374 6174 7320 746f 2061 2066  ump stats to a f
-00017540: 696c 656e 616d 650a 2020 2020 2020 2020  ilename.        
-00017550: 2020 2020 2020 2020 7072 6f66 696c 6572          profiler
-00017560: 2e64 756d 705f 7374 6174 7328 2061 7267  .dump_stats( arg
-00017570: 732e 7072 6f66 696c 6520 290a 2020 2020  s.profile ).    
-00017580: 2020 2020 2020 2020 7072 6f66 0909 3d20          prof..= 
-00017590: 7073 7461 7473 2e53 7461 7473 2820 7072  pstats.Stats( pr
-000175a0: 6f66 696c 6572 2c20 7374 7265 616d 3d73  ofiler, stream=s
-000175b0: 7973 2e73 7464 6572 7220 290a 2020 2020  ys.stderr ).    
-000175c0: 2020 2020 2020 2020 7072 696e 7428 2022          print( "
-000175d0: 5c6e 5c6e 5449 4d45 3a22 2c20 6669 6c65  \n\nTIME:", file
-000175e0: 3d73 7973 2e73 7464 6572 7220 290a 2020  =sys.stderr ).  
-000175f0: 2020 2020 2020 2020 2020 7072 6f66 2e73            prof.s
-00017600: 6f72 745f 7374 6174 7328 2020 2774 696d  ort_stats(  'tim
-00017610: 6527 2029 2e70 7269 6e74 5f73 7461 7473  e' ).print_stats
-00017620: 2820 7072 6f66 696c 6572 5f6c 696d 6974  ( profiler_limit
-00017630: 2029 0a0a 2020 2020 2020 2020 2020 2020   )..            
-00017640: 7072 696e 7428 2022 5c6e 5c6e 4355 4d55  print( "\n\nCUMU
-00017650: 4c41 5449 5645 3a22 2c20 6669 6c65 3d73  LATIVE:", file=s
-00017660: 7973 2e73 7464 6572 7220 290a 2020 2020  ys.stderr ).    
-00017670: 2020 2020 2020 2020 7072 6f66 2e73 6f72          prof.sor
-00017680: 745f 7374 6174 7328 2020 2763 756d 756c  t_stats(  'cumul
-00017690: 6174 6976 6527 2029 2e70 7269 6e74 5f73  ative' ).print_s
-000176a0: 7461 7473 2820 7072 6f66 696c 6572 5f6c  tats( profiler_l
-000176b0: 696d 6974 2029 0a                        imit ).
+00015090: 2020 2020 2070 6173 7377 6f72 645f 7570       password_up
+000150a0: 6461 7465 093d 2069 6e70 7574 5f73 6563  date.= input_sec
+000150b0: 7572 6528 2022 456e 7465 7220 7b7d 2070  ure( "Enter {} p
+000150c0: 6173 7377 6f72 6420 286c 6561 7665 2065  assword (leave e
+000150d0: 6d70 7479 2066 6f72 206e 6f20 6368 616e  mpty for no chan
+000150e0: 6765 293a 2022 2e66 6f72 6d61 7428 2062  ge): ".format( b
+000150f0: 6173 656e 616d 6520 2929 0a20 2020 2020  asename )).     
+00015100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015110: 2020 2075 7365 7270 6173 735f 7570 6461     userpass_upda
+00015120: 7465 6420 7c3d 2062 6f6f 6c28 2070 6173  ted |= bool( pas
+00015130: 7377 6f72 645f 7570 6461 7465 2029 0a20  sword_update ). 
+00015140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015150: 2020 2020 2020 2069 6620 7061 7373 776f         if passwo
+00015160: 7264 5f75 7064 6174 653a 0a20 2020 2020  rd_update:.     
+00015170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015180: 2020 2020 2020 2070 6173 7377 6f72 6409         password.
+00015190: 3d20 7061 7373 776f 7264 5f75 7064 6174  = password_updat
+000151a0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+000151b0: 2020 2020 2020 6966 2075 7365 7270 6173        if userpas
+000151c0: 735f 7570 6461 7465 643a 0a20 2020 2020  s_updated:.     
+000151d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000151e0: 2020 206c 6f67 2e64 6574 6169 6c28 2022     log.detail( "
+000151f0: 5375 7070 6c79 696e 6720 6e65 7720 6372  Supplying new cr
+00015200: 6564 656e 7469 616c 7320 666f 7220 7b7d  edentials for {}
+00015210: 3a20 7b7d 222e 666f 726d 6174 280a 2020  : {}".format(.  
+00015220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015230: 2020 2020 2020 2020 2020 7573 6572 6e61            userna
+00015240: 6d65 206f 7220 2228 6e6f 2075 7365 726e  me or "(no usern
+00015250: 616d 6529 222c 2027 2a27 202a 206c 656e  ame)", '*' * len
+00015260: 2820 7061 7373 776f 7264 206f 7220 2727  ( password or ''
+00015270: 2029 206f 7220 2228 6e6f 2070 6173 7377   ) or "(no passw
+00015280: 6f72 6429 2220 2929 0a20 2020 2020 2020  ord)" )).       
+00015290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000152a0: 206b 6579 2c6c 6963 093d 2061 7574 686f   key,lic.= autho
+000152b0: 7269 7a61 7469 6f6e 2e73 656e 6428 2028  rization.send( (
+000152c0: 7573 6572 6e61 6d65 2c70 6173 7377 6f72  username,passwor
+000152d0: 6429 2029 0a20 2020 2020 2020 2020 2020  d) ).           
+000152e0: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
+000152f0: 7469 6e75 650a 2020 2020 2020 2020 2020  tinue.          
+00015300: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00015310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015320: 2020 2020 2020 2020 6c6f 672e 6465 7461          log.deta
+00015330: 696c 2820 224e 6f20 6e65 7720 6372 6564  il( "No new cred
+00015340: 656e 7469 616c 2873 2920 666f 7220 7b7d  ential(s) for {}
+00015350: 3a20 7b7d 7b7d 222e 666f 726d 6174 280a  : {}{}".format(.
+00015360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015370: 2020 2020 2020 2020 2020 2020 7573 6572              user
+00015380: 6e61 6d65 206f 7220 2228 6e6f 2075 7365  name or "(no use
+00015390: 726e 616d 6529 222c 2027 2a27 202a 206c  rname)", '*' * l
+000153a0: 656e 2820 7061 7373 776f 7264 206f 7220  en( password or 
+000153b0: 2727 2029 206f 7220 2228 6e6f 2070 6173  '' ) or "(no pas
+000153c0: 7377 6f72 6429 222c 0a20 2020 2020 2020  sword)",.       
+000153d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000153e0: 2020 2020 2022 2028 6174 7465 6d70 7469       " (attempti
+000153f0: 6e67 2074 6f20 7265 6769 7374 6572 206e  ng to register n
+00015400: 6577 2041 6765 6e74 2049 4429 2220 6966  ew Agent ID)" if
+00015410: 2061 7267 732e 7265 6769 7374 6572 2065   args.register e
+00015420: 6c73 6520 2220 2861 7574 686f 7269 7a61  lse " (authoriza
+00015430: 7469 6f6e 2066 6169 6c65 6429 2220 2929  tion failed)" ))
+00015440: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015450: 2020 2020 2023 204e 6f20 4b65 7970 6169       # No Keypai
+00015460: 7220 286f 7220 7065 7268 6170 7320 6120  r (or perhaps a 
+00015470: 4b65 7970 6169 722c 2062 7574 206e 6f20  Keypair, but no 
+00015480: 4c69 6365 6e73 6529 2066 6f75 6e64 3b20  License) found; 
+00015490: 6372 6564 656e 7469 616c 7320 4e4f 5475  credentials NOTu
+000154a0: 7064 6174 6564 0a20 2020 2020 2020 2020  pdated.         
+000154b0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+000154c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000154d0: 2023 2041 204b 6579 7061 6972 2061 6e64   # A Keypair and
+000154e0: 204c 6963 656e 7365 2077 6173 2066 6f75   License was fou
+000154f0: 6e64 3b20 7265 6d65 6d62 6572 2069 740a  nd; remember it.
+00015500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015510: 2020 2020 6c6f 6164 6564 2e61 7070 656e      loaded.appen
+00015520: 6428 2028 6b65 792c 6c69 6329 2029 0a20  d( (key,lic) ). 
+00015530: 2020 2020 2020 2020 2020 2020 2020 206b                 k
+00015540: 6579 2c6c 6963 0909 3d20 6e65 7874 2820  ey,lic..= next( 
+00015550: 6175 7468 6f72 697a 6174 696f 6e20 290a  authorization ).
+00015560: 2020 2020 2020 2020 6578 6365 7074 2053          except S
+00015570: 746f 7049 7465 7261 7469 6f6e 3a0a 2020  topIteration:.  
+00015580: 2020 2020 2020 2020 2020 6c6f 672e 6465            log.de
+00015590: 7461 696c 2820 2243 6f6d 706c 6574 6564  tail( "Completed
+000155a0: 206c 6963 656e 7369 6e67 2e61 7574 686f   licensing.autho
+000155b0: 7269 7a65 6420 772f 207b 7d20 4b65 7970  rized w/ {} Keyp
+000155c0: 6169 722f 4c69 6365 6e73 6573 2066 6f75  air/Licenses fou
+000155d0: 6e64 222e 666f 726d 6174 2820 6c65 6e28  nd".format( len(
+000155e0: 6c6f 6164 6564 2920 2929 0a0a 2020 2020  loaded) ))..    
+000155f0: 2020 2020 2320 436f 6c6c 6563 7420 7570      # Collect up
+00015600: 2061 6c6c 2074 6865 204c 6963 656e 7365   all the License
+00015610: 2067 7261 6e74 733b 2074 6865 7265 206d   grants; there m
+00015620: 6179 2062 6520 6d6f 7265 2074 6861 6e20  ay be more than 
+00015630: 6f6e 652c 2069 6620 7468 6520 7573 6572  one, if the user
+00015640: 2068 6173 2070 7572 6368 6173 6564 0a20   has purchased. 
+00015650: 2020 2020 2020 2023 206d 756c 7469 706c         # multipl
+00015660: 6520 4c69 6365 6e73 6573 2061 7420 6469  e Licenses at di
+00015670: 6666 6572 656e 7420 7469 6d65 732e 2020  fferent times.  
+00015680: 456e 7375 7265 7320 7765 206f 6e6c 7920  Ensures we only 
+00015690: 696e 636c 7564 6520 6120 7370 6563 6966  include a specif
+000156a0: 6963 204c 6963 656e 7365 206f 6e63 652e  ic License once.
+000156b0: 0a20 2020 2020 2020 2067 7261 6e74 7309  .        grants.
+000156c0: 0909 3d20 6c69 6365 6e73 696e 672e 4772  ..= licensing.Gr
+000156d0: 616e 7428 290a 2020 2020 2020 2020 6f6e  ant().        on
+000156e0: 6365 0909 093d 2073 6574 2829 0a20 2020  ce...= set().   
+000156f0: 2020 2020 2066 6f72 206b 6579 2c6c 6963       for key,lic
+00015700: 2069 6e20 6c6f 6164 6564 3a0a 2020 2020   in loaded:.    
+00015710: 2020 2020 2020 2020 6772 616e 7473 5f6c          grants_l
+00015720: 6963 0909 3d20 6c69 632e 6772 616e 7473  ic..= lic.grants
+00015730: 2820 6f6e 6365 3d6f 6e63 6520 290a 2020  ( once=once ).  
+00015740: 2020 2020 2020 2020 2020 6c6f 672e 6e6f            log.no
+00015750: 726d 616c 2820 224c 6f63 6174 6564 2041  rmal( "Located A
+00015760: 6765 6e74 2045 6432 3535 3139 204b 6579  gent Ed25519 Key
+00015770: 7061 6972 207b 7075 626b 6579 7d20 772f  pair {pubkey} w/
+00015780: 207b 7072 6f64 7563 747d 204c 6963 656e   {product} Licen
+00015790: 7365 2028 6672 6f6d 207b 5f66 726f 6d7d  se (from {_from}
+000157a0: 297b 6578 7472 617d 222e 666f 726d 6174  ){extra}".format
+000157b0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+000157c0: 2020 7075 626b 6579 093d 206c 6963 656e    pubkey.= licen
+000157d0: 7369 6e67 2e69 6e74 6f5f 6236 3428 206b  sing.into_b64( k
+000157e0: 6579 2e76 6b20 292c 0a20 2020 2020 2020  ey.vk ),.       
+000157f0: 2020 2020 2020 2020 2070 726f 6475 6374           product
+00015800: 093d 206c 6963 2061 6e64 206c 6963 2e6c  .= lic and lic.l
+00015810: 6963 656e 7365 2e61 7574 686f 722e 7072  icense.author.pr
+00015820: 6f64 7563 7420 6f72 2022 456e 642d 5573  oduct or "End-Us
+00015830: 6572 222c 0a20 2020 2020 2020 2020 2020  er",.           
+00015840: 2020 2020 205f 6672 6f6d 093d 2022 6672       _from.= "fr
+00015850: 6f6d 207b 7d22 2e66 6f72 6d61 7428 206c  om {}".format( l
+00015860: 6963 2e5f 6672 6f6d 2029 2069 6620 6c69  ic._from ) if li
+00015870: 632e 5f66 726f 6d20 656c 7365 2022 6c6f  c._from else "lo
+00015880: 6361 6c6c 7920 6973 7375 6564 222c 0a20  cally issued",. 
+00015890: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+000158a0: 7874 7261 093d 2028 2820 2220 772f 2067  xtra.= (( " w/ g
+000158b0: 7261 6e74 733a 207b 7d22 2e66 6f72 6d61  rants: {}".forma
+000158c0: 7428 2067 7261 6e74 735f 6c69 6320 2920  t( grants_lic ) 
+000158d0: 6966 206c 6f67 2e69 7345 6e61 626c 6564  if log.isEnabled
+000158e0: 466f 7228 206c 6f67 6769 6e67 2e44 4542  For( logging.DEB
+000158f0: 5547 2029 2065 6c73 6520 2222 2029 0a20  UG ) else "" ). 
+00015900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015910: 2020 2020 2020 2020 2020 2b20 2820 2220            + ( " 
+00015920: 6d65 7267 696e 6720 772f 2067 7261 6e74  merging w/ grant
+00015930: 733a 207b 7d22 2e66 6f72 6d61 7428 2067  s: {}".format( g
+00015940: 7261 6e74 7320 2920 6966 206c 6f67 2e69  rants ) if log.i
+00015950: 7345 6e61 626c 6564 466f 7228 206c 6f67  sEnabledFor( log
+00015960: 6769 6e67 2e54 5241 4345 2029 2065 6c73  ging.TRACE ) els
+00015970: 6520 2222 2029 292c 0a20 2020 2020 2020  e "" )),.       
+00015980: 2020 2020 2029 290a 2020 2020 2020 2020       )).        
+00015990: 2020 2020 6772 616e 7473 0920 2020 2020      grants.     
+000159a0: 2020 7c3d 2067 7261 6e74 735f 6c69 630a    |= grants_lic.
+000159b0: 0a20 2020 2020 2020 2023 2041 6e64 2c20  .        # And, 
+000159c0: 6669 6e61 6c6c 793a 2061 7363 6572 7461  finally: ascerta
+000159d0: 696e 2077 6865 7468 6572 2077 6520 6861  in whether we ha
+000159e0: 7665 2061 2047 7261 6e74 2074 6f20 7275  ve a Grant to ru
+000159f0: 6e20 446f 6d69 6e69 6f6e 2052 2644 2043  n Dominion R&D C
+00015a00: 6f72 7027 7320 4372 7970 746f 204c 6963  orp's Crypto Lic
+00015a10: 656e 7369 6e67 2053 6572 7665 7221 0a20  ensing Server!. 
+00015a20: 2020 2020 2020 2061 7373 6572 7420 646f         assert do
+00015a30: 6d69 6e69 6f6e 2e73 6572 7669 6365 6b65  minion.serviceke
+00015a40: 7920 696e 2067 7261 6e74 732c 205c 0a20  y in grants, \. 
+00015a50: 2020 2020 2020 2020 2020 2022 556e 6162             "Unab
+00015a60: 6c65 2074 6f20 6669 6e64 207b 7d27 7320  le to find {}'s 
+00015a70: 7072 6f64 7563 7420 7b21 727d 2073 6572  product {!r} ser
+00015a80: 7669 6365 206b 6579 207b 2172 7d20 696e  vice key {!r} in
+00015a90: 204c 6963 656e 7365 2047 7261 6e74 7320   License Grants 
+00015aa0: 7b7d 222e 666f 726d 6174 280a 2020 2020  {}".format(.    
+00015ab0: 2020 2020 2020 2020 2020 2020 646f 6d69              domi
+00015ac0: 6e69 6f6e 2e6e 616d 652c 2064 6f6d 696e  nion.name, domin
+00015ad0: 696f 6e2e 7072 6f64 7563 742c 2064 6f6d  ion.product, dom
+00015ae0: 696e 696f 6e2e 7365 7276 6963 656b 6579  inion.servicekey
+00015af0: 2c20 6772 616e 7473 2029 0a0a 2020 2020  , grants )..    
+00015b00: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
+00015b10: 2061 7320 6578 633a 0a20 2020 2020 2020   as exc:.       
+00015b20: 206c 6f67 2e65 7272 6f72 2820 2246 6169   log.error( "Fai
+00015b30: 6c65 6420 6c6f 6164 696e 6720 4167 656e  led loading Agen
+00015b40: 7420 4b65 7970 6169 7220 616e 642f 6f72  t Keypair and/or
+00015b50: 204c 6963 656e 7365 3a20 7b65 7863 7d22   License: {exc}"
+00015b60: 2e66 6f72 6d61 7428 0a20 2020 2020 2020  .format(.       
+00015b70: 2020 2020 2065 7863 3d27 272e 6a6f 696e       exc=''.join
+00015b80: 2820 7472 6163 6562 6163 6b2e 666f 726d  ( traceback.form
+00015b90: 6174 5f65 7863 6570 7469 6f6e 2820 2a73  at_exception( *s
+00015ba0: 7973 2e65 7863 5f69 6e66 6f28 2920 2929  ys.exc_info() ))
+00015bb0: 2069 6620 6c6f 672e 6973 456e 6162 6c65   if log.isEnable
+00015bc0: 6446 6f72 2820 6c6f 6767 696e 672e 5452  dFor( logging.TR
+00015bd0: 4143 4520 2920 656c 7365 2065 7863 2029  ACE ) else exc )
+00015be0: 290a 2020 2020 2020 2020 7769 7468 206f  ).        with o
+00015bf0: 7065 6e28 206f 732e 7061 7468 2e6a 6f69  pen( os.path.joi
+00015c00: 6e28 206f 732e 7061 7468 2e64 6972 6e61  n( os.path.dirna
+00015c10: 6d65 2820 5f5f 6669 6c65 5f5f 2029 2c20  me( __file__ ), 
+00015c20: 2773 7461 7469 6327 2c20 2774 7874 272c  'static', 'txt',
+00015c30: 2027 434c 2d4b 4559 5041 4952 2d4d 4953   'CL-KEYPAIR-MIS
+00015c40: 5349 4e47 2e74 7874 2720 292c 2027 7227  SING.txt' ), 'r'
+00015c50: 2029 2061 7320 663a 0a20 2020 2020 2020   ) as f:.       
+00015c60: 2020 2020 2070 7269 6e74 2820 662e 7265       print( f.re
+00015c70: 6164 2829 2e66 6f72 6d61 7428 0a20 2020  ad().format(.   
+00015c80: 2020 2020 2020 2020 2020 2020 2044 4953               DIS
+00015c90: 5452 4942 5554 494f 4e09 3d20 6c69 6365  TRIBUTION.= lice
+00015ca0: 6e73 696e 672e 4449 5354 5249 4255 5449  nsing.DISTRIBUTI
+00015cb0: 4f4e 2c0a 2020 2020 2020 2020 2020 2020  ON,.            
+00015cc0: 2020 2020 4b45 5950 4154 5445 524e 093d      KEYPATTERN.=
+00015cd0: 206c 6963 656e 7369 6e67 2e4b 4559 5041   licensing.KEYPA
+00015ce0: 5454 4552 4e2c 0a20 2020 2020 2020 2020  TTERN,.         
+00015cf0: 2020 2020 2020 204c 4943 454e 5345 5f4f         LICENSE_O
+00015d00: 5054 494f 4e09 3d20 272d 2d6c 6963 656e  PTION.= '--licen
+00015d10: 7365 272c 0a20 2020 2020 2020 2020 2020  se',.           
+00015d20: 2029 2c20 6669 6c65 3d73 7973 2e73 7464   ), file=sys.std
+00015d30: 6572 7220 290a 2020 2020 2020 2020 7379  err ).        sy
+00015d40: 732e 6578 6974 2820 3120 290a 0a20 2020  s.exit( 1 )..   
+00015d50: 2023 2053 6574 2075 7020 7468 6520 676c   # Set up the gl
+00015d60: 6f62 616c 2064 622c 2065 7463 2e0a 2020  obal db, etc..  
+00015d70: 2020 6462 5f73 6574 7570 2829 0a0a 2020    db_setup()..  
+00015d80: 2020 2320 5375 6d6d 6172 697a 6520 7468    # Summarize th
+00015d90: 6520 696e 6974 6961 6c20 4c69 6365 6e73  e initial Licens
+00015da0: 6573 2061 6e64 204b 6579 7061 6972 7320  es and Keypairs 
+00015db0: 6176 6169 6c61 626c 653b 2074 6865 7365  available; these
+00015dc0: 2061 7265 2072 652d 6f62 7461 696e 6564   are re-obtained
+00015dd0: 2069 6e20 7265 616c 2d74 696d 6520 6279   in real-time by
+00015de0: 2074 6865 2055 4973 2c20 6162 6f76 650a   the UIs, above.
+00015df0: 2020 2020 7374 6f72 6564 0909 093d 2064      stored...= d
+00015e00: 622e 7365 6c65 6374 2820 276c 6963 656e  b.select( 'licen
+00015e10: 7365 7327 2029 0a20 2020 2073 746f 7265  ses' ).    store
+00015e20: 6409 0909 3d20 6c69 7374 2820 7374 6f72  d...= list( stor
+00015e30: 6564 2029 0a20 2020 2066 6f72 2073 6967  ed ).    for sig
+00015e40: 2c20 6c69 6320 696e 206c 6963 656e 7365  , lic in license
+00015e50: 7328 2063 6f6e 6669 726d 3d46 616c 7365  s( confirm=False
+00015e60: 2c20 7374 6f72 6564 3d73 746f 7265 6420  , stored=stored 
+00015e70: 293a 0a20 2020 2020 2020 206c 6f67 2e69  ):.        log.i
+00015e80: 6e66 6f28 2022 7b73 3a3c 3634 7d3a 207b  nfo( "{s:<64}: {
+00015e90: 6c69 637d 222e 666f 726d 6174 280a 2020  lic}".format(.  
+00015ea0: 2020 2020 2020 2020 2020 733d 6c69 6365            s=lice
+00015eb0: 6e73 696e 672e 696e 746f 5f62 3634 2820  nsing.into_b64( 
+00015ec0: 7369 6720 292c 206c 6963 3d73 7472 2820  sig ), lic=str( 
+00015ed0: 6c69 6320 2920 2929 0a0a 2020 2020 666f  lic ) ))..    fo
+00015ee0: 7220 6e61 6d65 2c20 6b65 7970 6169 722c  r name, keypair,
+00015ef0: 2028 7573 6572 6e61 6d65 2c20 7061 7373   (username, pass
+00015f00: 776f 7264 2920 696e 206b 6579 7061 6972  word) in keypair
+00015f10: 7328 293a 0a20 2020 2020 2020 2074 7279  s():.        try
+00015f20: 3a0a 2020 2020 2020 2020 2020 2020 766b  :.            vk
+00015f30: 0909 093d 206c 6963 656e 7369 6e67 2e69  ...= licensing.i
+00015f40: 6e74 6f5f 6236 3428 206b 6579 7061 6972  nto_b64( keypair
+00015f50: 2e69 6e74 6f5f 6b65 7970 6169 7228 2075  .into_keypair( u
+00015f60: 7365 726e 616d 653d 7573 6572 6e61 6d65  sername=username
+00015f70: 2c20 7061 7373 776f 7264 3d70 6173 7377  , password=passw
+00015f80: 6f72 6420 292e 766b 2029 0a20 2020 2020  ord ).vk ).     
+00015f90: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
+00015fa0: 696f 6e20 6173 2065 7863 3a0a 2020 2020  ion as exc:.    
+00015fb0: 2020 2020 2020 2020 766b 0909 093d 2073          vk...= s
+00015fc0: 7472 2820 6578 6320 290a 2020 2020 2020  tr( exc ).      
+00015fd0: 2020 6c6f 672e 696e 666f 2820 227b 6e3a    log.info( "{n:
+00015fe0: 3c32 307d 3a20 7b76 6b7d 2077 2f20 7b75  <20}: {vk} w/ {u
+00015ff0: 3a3e 3230 7d20 2f20 7b70 7d22 2e66 6f72  :>20} / {p}".for
+00016000: 6d61 7428 0a20 2020 2020 2020 2020 2020  mat(.           
+00016010: 206e 3d6e 616d 652c 2076 6b3d 766b 2c20   n=name, vk=vk, 
+00016020: 753d 7573 6572 6e61 6d65 2c20 703d 272a  u=username, p='*
+00016030: 2720 2a20 6c65 6e28 2070 6173 7377 6f72  ' * len( passwor
+00016040: 6420 2929 290a 0a20 2020 2063 6c61 7373  d )))..    class
+00016050: 2064 6165 6d6f 6e28 2074 6872 6561 6469   daemon( threadi
+00016060: 6e67 2e54 6872 6561 6420 293a 0a20 2020  ng.Thread ):.   
+00016070: 2020 2020 2022 2222 4576 6572 7920 6461       """Every da
+00016080: 656d 6f6e 206d 7573 7420 6861 7665 2061  emon must have a
+00016090: 2063 6f6e 6669 675b 2763 6f6e 7472 6f6c   config['control
+000160a0: 275d 3b20 7365 7473 2069 7473 2064 6f6e  ']; sets its don
+000160b0: 6520 3d20 5472 7565 2074 6f20 7374 6f70  e = True to stop
+000160c0: 2e22 2222 0a20 2020 2020 2020 2064 6566  .""".        def
+000160d0: 205f 5f69 6e69 745f 5f28 2073 656c 662c   __init__( self,
+000160e0: 2063 6f6e 6669 673d 4e6f 6e65 2c20 2a2a   config=None, **
+000160f0: 6b77 6473 2029 3a0a 2020 2020 2020 2020  kwds ):.        
+00016100: 2020 2020 7375 7065 7228 2064 6165 6d6f      super( daemo
+00016110: 6e2c 2073 656c 6620 292e 5f5f 696e 6974  n, self ).__init
+00016120: 5f5f 2820 2a2a 6b77 6473 2029 0a20 2020  __( **kwds ).   
+00016130: 2020 2020 2020 2020 2073 656c 662e 6461           self.da
+00016140: 656d 6f6e 0909 3d20 5472 7565 0a20 2020  emon..= True.   
+00016150: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
+00016160: 6e66 6967 0909 3d20 636f 6e66 6967 206f  nfig..= config o
+00016170: 7220 7b7d 0a20 2020 2020 2020 2020 2020  r {}.           
+00016180: 2073 656c 662e 636f 6e66 6967 2e73 6574   self.config.set
+00016190: 6465 6661 756c 7428 2027 636f 6e74 726f  default( 'contro
+000161a0: 6c27 2c20 7b7d 2029 2e73 6574 6465 6661  l', {} ).setdefa
+000161b0: 756c 7428 2027 646f 6e65 272c 2046 616c  ult( 'done', Fal
+000161c0: 7365 2029 0a0a 2020 2020 2020 2020 6465  se )..        de
+000161d0: 6620 7374 6f70 2820 7365 6c66 2029 3a0a  f stop( self ):.
+000161e0: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
+000161f0: 696e 672e 696e 666f 2820 2253 746f 7070  ing.info( "Stopp
+00016200: 696e 6720 2573 2054 6872 6561 6422 2c20  ing %s Thread", 
+00016210: 7365 6c66 2e6e 616d 6520 290a 2020 2020  self.name ).    
+00016220: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
+00016230: 6669 675b 2763 6f6e 7472 6f6c 275d 5b27  fig['control']['
+00016240: 646f 6e65 275d 203d 2054 7275 650a 0a20  done'] = True.. 
+00016250: 2020 2020 2020 2064 6566 206a 6f69 6e28         def join(
+00016260: 2073 656c 662c 202a 6172 6773 2c20 2a2a   self, *args, **
+00016270: 6b77 6473 2029 3a0a 2020 2020 2020 2020  kwds ):.        
+00016280: 2020 2020 7365 6c66 2e73 746f 7028 290a      self.stop().
+00016290: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
+000162a0: 696e 672e 696e 666f 2820 224a 6f69 6e69  ing.info( "Joini
+000162b0: 6e67 2025 7320 5468 7265 6164 2e2e 2e22  ng %s Thread..."
+000162c0: 2c20 7365 6c66 2e6e 616d 6520 290a 2020  , self.name ).  
+000162d0: 2020 2020 2020 2020 2020 7375 7065 7228            super(
+000162e0: 2064 6165 6d6f 6e2c 2073 656c 6620 292e   daemon, self ).
+000162f0: 6a6f 696e 2820 2a61 7267 732c 202a 2a6b  join( *args, **k
+00016300: 7764 7320 290a 2020 2020 2020 2020 2020  wds ).          
+00016310: 2020 6c6f 6767 696e 672e 696e 666f 2820    logging.info( 
+00016320: 224a 6f69 6e65 6420 2573 2054 6872 6561  "Joined %s Threa
+00016330: 6422 2c20 7365 6c66 2e6e 616d 6520 290a  d", self.name ).
+00016340: 0a20 2020 2063 6c61 7373 2074 7874 7468  .    class txtth
+00016350: 7265 6164 2820 6461 656d 6f6e 2029 3a0a  read( daemon ):.
+00016360: 2020 2020 2020 2020 6465 6620 7275 6e28          def run(
+00016370: 2073 656c 6620 293a 0a20 2020 2020 2020   self ):.       
+00016380: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+00016390: 2020 2020 2020 2020 2020 7768 696c 6520            while 
+000163a0: 6e6f 7420 7365 6c66 2e63 6f6e 6669 672e  not self.config.
+000163b0: 6765 7428 2027 636f 6e74 726f 6c27 2c20  get( 'control', 
+000163c0: 7b7d 2029 2e67 6574 2820 2764 6f6e 6527  {} ).get( 'done'
+000163d0: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
+000163e0: 2020 2020 2020 2020 6966 2074 7874 6775          if txtgu
+000163f0: 6928 2073 656c 662e 636f 6e66 6967 2029  i( self.config )
+00016400: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00016410: 2020 2020 2020 2020 2020 2320 5465 7874            # Text
+00016420: 7561 6c20 4755 4920 6861 7320 6661 696c  ual GUI has fail
+00016430: 6564 2120 2044 6f6e 2774 2072 6573 7461  ed!  Don't resta
+00016440: 7274 2e0a 2020 2020 2020 2020 2020 2020  rt..            
+00016450: 2020 2020 2020 2020 2020 2020 6272 6561              brea
+00016460: 6b0a 2020 2020 2020 2020 2020 2020 6578  k.            ex
+00016470: 6365 7074 2045 7863 6570 7469 6f6e 2061  cept Exception a
+00016480: 7320 6578 633a 0a20 2020 2020 2020 2020  s exc:.         
+00016490: 2020 2020 2020 206c 6f67 6769 6e67 2e65         logging.e
+000164a0: 7272 6f72 2822 5465 7874 2047 5549 2066  rror("Text GUI f
+000164b0: 6169 6c65 643a 2025 735c 6e25 7322 2c20  ailed: %s\n%s", 
+000164c0: 6578 632c 2074 7261 6365 6261 636b 2e66  exc, traceback.f
+000164d0: 6f72 6d61 745f 6578 6328 2929 0a20 2020  ormat_exc()).   
+000164e0: 2020 2020 2020 2020 2066 696e 616c 6c79           finally
+000164f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00016500: 2020 6c6f 6767 696e 672e 7761 726e 696e    logging.warnin
+00016510: 6728 2022 5465 7874 2047 5549 2065 7869  g( "Text GUI exi
+00016520: 7469 6e67 2220 290a 2020 2020 2020 2020  ting" ).        
+00016530: 2020 2020 2020 2020 7365 6c66 2e73 746f          self.sto
+00016540: 7028 290a 0a20 2020 2063 6c61 7373 2077  p()..    class w
+00016550: 6562 7468 7265 6164 2820 6461 656d 6f6e  ebthread( daemon
+00016560: 2029 3a0a 2020 2020 2020 2020 6465 6620   ):.        def 
+00016570: 7275 6e28 2073 656c 6620 293a 0a20 2020  run( self ):.   
+00016580: 2020 2020 2020 2020 2074 7279 3a0a 2020           try:.  
+00016590: 2020 2020 2020 2020 2020 2020 2020 7765                we
+000165a0: 6270 7928 2073 656c 662e 636f 6e66 6967  bpy( self.config
+000165b0: 2029 0a20 2020 2020 2020 2020 2020 2065   ).            e
+000165c0: 7863 6570 7420 4578 6365 7074 696f 6e20  xcept Exception 
+000165d0: 6173 2065 7863 3a0a 2020 2020 2020 2020  as exc:.        
+000165e0: 2020 2020 2020 2020 6c6f 6767 696e 672e          logging.
+000165f0: 6572 726f 7228 2022 5765 6220 4755 4920  error( "Web GUI 
+00016600: 6661 696c 6564 3a20 2573 5c6e 2573 222c  failed: %s\n%s",
+00016610: 2065 7863 2c20 7472 6163 6562 6163 6b2e   exc, traceback.
+00016620: 666f 726d 6174 5f65 7863 2829 2029 0a20  format_exc() ). 
+00016630: 2020 2020 2020 2020 2020 2066 696e 616c             final
+00016640: 6c79 3a0a 2020 2020 2020 2020 2020 2020  ly:.            
+00016650: 2020 2020 7365 6c66 2e73 746f 7028 290a      self.stop().
+00016660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016670: 6c6f 6767 696e 672e 7761 726e 696e 6728  logging.warning(
+00016680: 2022 5765 6220 4755 4920 6578 6974 696e   "Web GUI exitin
+00016690: 6722 2029 0a0a 2020 2020 2020 2020 6465  g" )..        de
+000166a0: 6620 7374 6f70 2820 7365 6c66 2029 3a0a  f stop( self ):.
+000166b0: 2020 2020 2020 2020 2020 2020 2222 2249              """I
+000166c0: 6e20 6164 6469 7469 6f6e 2074 6f20 7468  n addition to th
+000166d0: 6520 6e6f 726d 616c 2073 746f 7020 7072  e normal stop pr
+000166e0: 6f63 6564 7572 6520 2870 6572 6861 7073  ocedure (perhaps
+000166f0: 2073 6967 6e61 6c69 6e67 206f 7468 6572   signaling other
+00016700: 2054 6872 6561 6473 2076 6961 2061 2073   Threads via a s
+00016710: 6861 7265 640a 2020 2020 2020 2020 2020  hared.          
+00016720: 2020 636f 6e74 726f 6c20 6469 6374 292c    control dict),
+00016730: 2077 6562 7079 2e73 6572 7665 7220 6861   webpy.server ha
+00016740: 7320 6974 7320 6f77 6e20 7374 6f70 206d  s its own stop m
+00016750: 6563 6861 6e69 736d 2e0a 0a20 2020 2020  echanism...     
+00016760: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00016770: 2020 2020 2020 2073 7570 6572 2820 7765         super( we
+00016780: 6274 6872 6561 642c 2073 656c 6620 292e  bthread, self ).
+00016790: 7374 6f70 2829 0a20 2020 2020 2020 2020  stop().         
+000167a0: 2020 2069 6620 7765 6270 792e 7365 7276     if webpy.serv
+000167b0: 6572 3a0a 2020 2020 2020 2020 2020 2020  er:.            
+000167c0: 2020 2020 6c6f 6767 696e 672e 696e 666f      logging.info
+000167d0: 2820 2257 6562 2047 5549 2073 746f 7070  ( "Web GUI stopp
+000167e0: 696e 672e 2e2e 2220 290a 2020 2020 2020  ing..." ).      
+000167f0: 2020 2020 2020 2020 2020 7765 6270 792e            webpy.
+00016800: 7365 7276 6572 2e73 746f 7028 290a 2020  server.stop().  
+00016810: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+00016820: 6767 696e 672e 696e 666f 2820 2257 6562  gging.info( "Web
+00016830: 2047 5549 2073 746f 7070 6564 2220 290a   GUI stopped" ).
+00016840: 0a20 2020 2063 6c61 7373 2063 746c 7468  .    class ctlth
+00016850: 7265 6164 2820 6461 656d 6f6e 2029 3a0a  read( daemon ):.
+00016860: 2020 2020 2020 2020 6465 6620 7275 6e28          def run(
+00016870: 2073 656c 6620 293a 0a20 2020 2020 2020   self ):.       
+00016880: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+00016890: 2020 2020 2020 2020 2020 7768 696c 6520            while 
+000168a0: 6e6f 7420 7365 6c66 2e63 6f6e 6669 672e  not self.config.
+000168b0: 6765 7428 2027 636f 6e74 726f 6c27 2c20  get( 'control', 
+000168c0: 7b7d 2029 2e67 6574 2820 2764 6f6e 6527  {} ).get( 'done'
+000168d0: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
+000168e0: 2020 2020 2020 2020 6265 6709 093d 2074          beg..= t
+000168f0: 696d 6572 2829 0a20 2020 2020 2020 2020  imer().         
+00016900: 2020 2020 2020 2020 2020 2063 746c 6c6f             ctllo
+00016910: 6f70 2820 6265 672c 2073 656c 662e 636f  op( beg, self.co
+00016920: 6e66 6967 2029 0a20 2020 2020 2020 2020  nfig ).         
+00016930: 2020 2020 2020 2020 2020 2064 7572 0909             dur..
+00016940: 3d20 7469 6d65 7228 2920 2d20 6265 670a  = timer() - beg.
+00016950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016960: 2020 2020 6379 6309 093d 2073 656c 662e      cyc..= self.
+00016970: 636f 6e66 6967 2e67 6574 2820 2763 7963  config.get( 'cyc
+00016980: 6c65 272c 2031 2e30 2029 0a20 2020 2020  le', 1.0 ).     
+00016990: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000169a0: 6620 6475 7220 3c20 6379 633a 0a20 2020  f dur < cyc:.   
+000169b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000169c0: 2020 2020 2074 696d 652e 736c 6565 7028       time.sleep(
+000169d0: 2063 7963 202d 2064 7572 2029 0a20 2020   cyc - dur ).   
+000169e0: 2020 2020 2020 2020 2065 7863 6570 7420           except 
+000169f0: 4578 6365 7074 696f 6e20 6173 2065 7863  Exception as exc
+00016a00: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00016a10: 2020 6c6f 6767 696e 672e 6572 726f 7228    logging.error(
+00016a20: 2022 436f 6e74 726f 6c20 7379 7374 656d   "Control system
+00016a30: 2066 6169 6c65 643a 2025 735c 6e25 7322   failed: %s\n%s"
+00016a40: 2c20 6578 632c 2074 7261 6365 6261 636b  , exc, traceback
+00016a50: 2e66 6f72 6d61 745f 6578 6328 2920 290a  .format_exc() ).
+00016a60: 2020 2020 2020 2020 2020 2020 6669 6e61              fina
+00016a70: 6c6c 793a 0a20 2020 2020 2020 2020 2020  lly:.           
+00016a80: 2020 2020 206c 6f67 6769 6e67 2e77 6172       logging.war
+00016a90: 6e69 6e67 2820 2243 6f6e 7472 6f6c 2073  ning( "Control s
+00016aa0: 7973 7465 6d20 6578 6974 696e 6722 2029  ystem exiting" )
+00016ab0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016ac0: 2073 656c 662e 7374 6f70 2829 0a0a 2020   self.stop()..  
+00016ad0: 2020 2320 536f 6d65 206f 6620 7468 6573    # Some of thes
+00016ae0: 6520 7468 7265 6164 7320 6d61 7920 6e65  e threads may ne
+00016af0: 6564 2074 6f20 7265 6469 7265 6374 2073  ed to redirect s
+00016b00: 7973 2e73 7464 6f75 742f 7374 6465 7272  ys.stdout/stderr
+00016b10: 3b20 7361 7665 2061 6e64 2072 6573 746f  ; save and resto
+00016b20: 7265 0a20 2020 2073 7973 5f73 7472 6561  re.    sys_strea
+00016b30: 6d5f 7361 7665 0909 3d20 7379 732e 7374  m_save..= sys.st
+00016b40: 646f 7574 2c20 7379 732e 7374 6465 7272  dout, sys.stderr
+00016b50: 0a20 2020 2074 6872 6561 6473 0909 093d  .    threads...=
+00016b60: 205b 5d0a 0a20 2020 2073 6572 7665 7209   []..    server.
+00016b70: 0909 3d20 6c69 6365 6e73 696e 675f 6b77  ..= licensing_kw
+00016b80: 6473 2e70 6f70 2820 2773 6572 7665 7227  ds.pop( 'server'
+00016b90: 2c20 7b7d 2029 0a20 2020 2063 6f6e 7472  , {} ).    contr
+00016ba0: 6f6c 0909 093d 2073 6572 7665 722e 706f  ol...= server.po
+00016bb0: 7028 2027 636f 6e74 726f 6c27 2c20 7b7d  p( 'control', {}
+00016bc0: 2029 0a20 2020 2074 7279 3a0a 2020 2020   ).    try:.    
+00016bd0: 2020 2020 2320 5374 6172 7420 7468 6520      # Start the 
+00016be0: 636f 6e74 726f 6c20 7379 7374 656d 2054  control system T
+00016bf0: 6872 6561 642e 0a20 2020 2020 2020 2063  hread..        c
+00016c00: 746c 636e 6609 0909 3d20 6c69 6365 6e73  tlcnf...= licens
+00016c10: 696e 675f 6b77 6473 2e70 6f70 2820 2763  ing_kwds.pop( 'c
+00016c20: 746c 272c 207b 7d20 290a 2020 2020 2020  tl', {} ).      
+00016c30: 2020 6374 6c63 6e66 2e73 6574 6465 6661    ctlcnf.setdefa
+00016c40: 756c 7428 2027 6379 636c 6527 2c20 312e  ult( 'cycle', 1.
+00016c50: 3020 290a 2020 2020 2020 2020 6374 6c63  0 ).        ctlc
+00016c60: 6e66 2e73 6574 6465 6661 756c 7428 2027  nf.setdefault( '
+00016c70: 636f 6e74 726f 6c27 2c20 636f 6e74 726f  control', contro
+00016c80: 6c20 290a 2020 2020 2020 2020 6374 6c74  l ).        ctlt
+00016c90: 6872 0909 093d 2063 746c 7468 7265 6164  hr...= ctlthread
+00016ca0: 2820 636f 6e66 6967 3d63 746c 636e 662c  ( config=ctlcnf,
+00016cb0: 206e 616d 653d 2763 6f6e 7472 6f6c 2720   name='control' 
+00016cc0: 290a 2020 2020 2020 2020 6374 6c74 6872  ).        ctlthr
+00016cd0: 2e73 7461 7274 2829 0a20 2020 2020 2020  .start().       
+00016ce0: 2074 6872 6561 6473 2e61 7070 656e 6428   threads.append(
+00016cf0: 2063 746c 7468 7220 290a 0a20 2020 2020   ctlthr )..     
+00016d00: 2020 2023 2053 7461 7274 2074 6865 2043     # Start the C
+00016d10: 7572 7365 7320 5465 7874 2047 5549 2028  urses Text GUI (
+00016d20: 6966 2064 6573 6972 6564 290a 2020 2020  if desired).    
+00016d30: 2020 2020 7478 7463 6e66 0909 093d 206c      txtcnf...= l
+00016d40: 6963 656e 7369 6e67 5f6b 7764 732e 706f  icensing_kwds.po
+00016d50: 7028 2027 7478 7427 2c20 7b7d 2029 0a20  p( 'txt', {} ). 
+00016d60: 2020 2020 2020 2074 7874 636e 662e 7365         txtcnf.se
+00016d70: 7464 6566 6175 6c74 2820 2763 6f6e 7472  tdefault( 'contr
+00016d80: 6f6c 272c 2063 6f6e 7472 6f6c 2029 0a20  ol', control ). 
+00016d90: 2020 2020 2020 2074 7874 636e 662e 7365         txtcnf.se
+00016da0: 7464 6566 6175 6c74 2820 2774 6974 6c65  tdefault( 'title
+00016db0: 272c 2027 4c69 6365 6e73 696e 6727 2029  ', 'Licensing' )
+00016dc0: 0a20 2020 2020 2020 2023 2042 7920 6465  .        # By de
+00016dd0: 6661 756c 742c 2061 6363 6573 7365 7320  fault, accesses 
+00016de0: 7468 6520 6c6f 6361 6c20 6675 6e63 7469  the local functi
+00016df0: 6f6e 7320 7969 656c 6469 6e67 2074 6865  ons yielding the
+00016e00: 2073 746f 7265 6420 6c69 6365 6e73 6573   stored licenses
+00016e10: 2c20 6372 6564 656e 7469 616c 7320 616e  , credentials an
+00016e20: 6420 6b65 7970 6169 7273 0a20 2020 2020  d keypairs.     
+00016e30: 2020 2074 7874 636e 662e 7365 7464 6566     txtcnf.setdef
+00016e40: 6175 6c74 2820 276c 6963 656e 7365 7327  ault( 'licenses'
+00016e50: 2c09 096c 6963 656e 7365 7320 290a 2020  ,..licenses ).  
+00016e60: 2020 2020 2020 7478 7463 6e66 2e73 6574        txtcnf.set
+00016e70: 6465 6661 756c 7428 2027 6372 6564 656e  default( 'creden
+00016e80: 7469 616c 7327 2c09 6372 6564 656e 7469  tials',.credenti
+00016e90: 616c 7320 290a 2020 2020 2020 2020 7478  als ).        tx
+00016ea0: 7463 6e66 2e73 6574 6465 6661 756c 7428  tcnf.setdefault(
+00016eb0: 2027 6b65 7970 6169 7273 272c 0909 6b65   'keypairs',..ke
+00016ec0: 7970 6169 7273 2029 0a20 2020 2020 2020  ypairs ).       
+00016ed0: 2074 7874 7468 7209 0909 3d20 4e6f 6e65   txtthr...= None
+00016ee0: 0a20 2020 2020 2020 2069 6620 6172 6773  .        if args
+00016ef0: 2e67 7569 3a0a 2020 2020 2020 2020 2020  .gui:.          
+00016f00: 2020 7478 7474 6872 0909 3d20 7478 7474    txtthr..= txtt
+00016f10: 6872 6561 6428 2074 7874 636e 662c 206e  hread( txtcnf, n
+00016f20: 616d 653d 2763 7572 7365 7327 2029 0a20  ame='curses' ). 
+00016f30: 2020 2020 2020 2020 2020 2074 7874 7468             txtth
+00016f40: 722e 7374 6172 7428 290a 2020 2020 2020  r.start().      
+00016f50: 2020 2020 2020 7468 7265 6164 732e 6170        threads.ap
+00016f60: 7065 6e64 2820 7478 7474 6872 2029 0a0a  pend( txtthr )..
+00016f70: 2020 2020 2020 2020 2320 5374 6172 7420          # Start 
+00016f80: 7468 6520 7765 6220 5549 2028 6966 2064  the web UI (if d
+00016f90: 6573 6972 6564 290a 2020 2020 2020 2020  esired).        
+00016fa0: 7765 6274 6872 0909 093d 204e 6f6e 650a  webthr...= None.
+00016fb0: 2020 2020 2020 2020 6966 2061 7267 732e          if args.
+00016fc0: 7765 623a 0a20 2020 2020 2020 2020 2020  web:.           
+00016fd0: 2023 2044 6564 7563 6520 696e 7465 7266   # Deduce interf
+00016fe0: 6163 653a 706f 7274 2074 6f20 6269 6e64  ace:port to bind
+00016ff0: 2c20 616e 6420 636f 7272 6563 7420 7479  , and correct ty
+00017000: 7065 730a 2020 2020 2020 2020 2020 2020  pes.            
+00017010: 6164 6472 6573 7309 093d 2061 7267 732e  address..= args.
+00017020: 7765 622e 7370 6c69 7428 2027 3a27 2029  web.split( ':' )
+00017030: 0a20 2020 2020 2020 2020 2020 2061 7373  .            ass
+00017040: 6572 7420 3120 3c3d 206c 656e 2820 6164  ert 1 <= len( ad
+00017050: 6472 6573 7320 2920 3c3d 2032 2c20 2257  dress ) <= 2, "W
+00017060: 6562 2061 6464 7265 7373 206d 7573 7420  eb address must 
+00017070: 6265 2069 6e20 7468 6520 666f 726d 203c  be in the form <
+00017080: 696e 7465 7266 6163 653e 3a3c 706f 7274  interface>:<port
+00017090: 3e22 0a20 2020 2020 2020 2020 2020 2061  >".            a
+000170a0: 6464 7265 7373 0909 3d20 2820 7374 7228  ddress..= ( str(
+000170b0: 2061 6464 7265 7373 5b30 5d20 292c 0a20   address[0] ),. 
+000170c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000170d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000170e0: 2020 2069 6e74 2820 6164 6472 6573 735b     int( address[
+000170f0: 315d 2029 2069 6620 6c65 6e28 2061 6464  1] ) if len( add
+00017100: 7265 7373 2029 203e 2031 2065 6c73 6520  ress ) > 1 else 
+00017110: 3830 3030 2029 0a0a 2020 2020 2020 2020  8000 )..        
+00017120: 2020 2020 2320 436f 6d6d 616e 642d 6c69      # Command-li
+00017130: 6e65 2070 6172 616d 6574 6572 7320 696e  ne parameters in
+00017140: 2061 7267 7620 6172 6520 6f76 6572 7269   argv are overri
+00017150: 6464 656e 2062 7920 7370 6563 6966 6963  dden by specific
+00017160: 2063 6f6e 6669 6775 7261 7469 6f6e 730a   configurations.
+00017170: 2020 2020 2020 2020 2020 2020 2320 7061              # pa
+00017180: 7373 6564 2069 6e20 6c69 6365 6e73 696e  ssed in licensin
+00017190: 675f 6b77 6473 5b27 7765 6227 5d0a 2020  g_kwds['web'].  
+000171a0: 2020 2020 2020 2020 2020 7765 6263 6e66            webcnf
+000171b0: 0909 3d20 6c69 6365 6e73 696e 675f 6b77  ..= licensing_kw
+000171c0: 6473 2e70 6f70 2820 2777 6562 272c 207b  ds.pop( 'web', {
+000171d0: 7d20 290a 2020 2020 2020 2020 2020 2020  } ).            
+000171e0: 7765 6263 6e66 2e73 6574 6465 6661 756c  webcnf.setdefaul
+000171f0: 7428 2027 636f 6e74 726f 6c27 2c20 636f  t( 'control', co
+00017200: 6e74 726f 6c20 290a 2020 2020 2020 2020  ntrol ).        
+00017210: 2020 2020 7765 6263 6e66 2e73 6574 6465      webcnf.setde
+00017220: 6661 756c 7428 2027 6164 6472 6573 7327  fault( 'address'
+00017230: 2c20 6164 6472 6573 7320 290a 2020 2020  , address ).    
+00017240: 2020 2020 2020 2020 7765 6263 6e66 2e73          webcnf.s
+00017250: 6574 6465 6661 756c 7428 2027 6163 6365  etdefault( 'acce
+00017260: 7373 272c 2061 7267 732e 6163 6365 7373  ss', args.access
+00017270: 2029 0a0a 2020 2020 2020 2020 2020 2020   )..            
+00017280: 2320 4966 2061 6c6c 2073 7973 2e73 7464  # If all sys.std
+00017290: 6f75 742f 7374 6465 7272 2073 686f 756c  out/stderr shoul
+000172a0: 6420 676f 7420 746f 2074 6865 2077 6562  d got to the web
+000172b0: 2073 6572 7665 7227 7320 6163 6365 7373   server's access
+000172c0: 206c 6f67 2066 696c 652c 2028 7468 650a   log file, (the.
+000172d0: 2020 2020 2020 2020 2020 2020 2320 6465              # de
+000172e0: 6661 756c 7429 2c20 7468 656e 2073 6574  fault), then set
+000172f0: 2069 7420 6865 7265 2e20 2049 6620 6e6f   it here.  If no
+00017300: 7420 2865 672e 2077 6520 7761 6e74 2074  t (eg. we want t
+00017310: 6f20 6265 2061 626c 6520 746f 2068 6172  o be able to har
+00017320: 7665 7374 2074 6865 2061 6374 7561 6c0a  vest the actual.
+00017330: 2020 2020 2020 2020 2020 2020 2320 6479              # dy
+00017340: 6e61 6d69 6320 4950 2061 6464 7265 7373  namic IP address
+00017350: 3a70 6f72 7420 6f66 2074 6865 2062 6f75  :port of the bou
+00017360: 6e64 2077 6562 2073 6572 7665 7220 736f  nd web server so
+00017370: 636b 6574 292c 2074 6865 6e20 7061 7373  cket), then pass
+00017380: 2046 616c 7365 7920 666f 7220 6163 6365   Falsey for acce
+00017390: 7373 2e0a 2020 2020 2020 2020 2020 2020  ss..            
+000173a0: 7765 6274 6872 0909 3d20 7765 6274 6872  webthr..= webthr
+000173b0: 6561 6428 2077 6562 636e 662c 2020 6e61  ead( webcnf,  na
+000173c0: 6d65 3d27 7765 6227 2029 0a20 2020 2020  me='web' ).     
+000173d0: 2020 2020 2020 2077 6562 7468 722e 7374         webthr.st
+000173e0: 6172 7428 290a 2020 2020 2020 2020 2020  art().          
+000173f0: 2020 7468 7265 6164 732e 6170 7065 6e64    threads.append
+00017400: 2820 7765 6274 6872 2029 0a0a 2020 2020  ( webthr )..    
+00017410: 2020 2020 2320 4a75 7374 2077 6169 7420      # Just wait 
+00017420: 666f 7220 616e 7920 7468 7265 6164 2028  for any thread (
+00017430: 7765 6220 6f72 2074 6578 7420 4755 492c  web or text GUI,
+00017440: 2063 6f6e 7472 6f6c 2920 746f 2066 696e   control) to fin
+00017450: 6973 680a 2020 2020 2020 2020 7768 696c  ish.        whil
+00017460: 6520 6e6f 7420 7368 7574 646f 776e 5f73  e not shutdown_s
+00017470: 6967 6e61 6c6c 6564 2061 6e64 2061 6c6c  ignalled and all
+00017480: 2820 742e 6973 5f61 6c69 7665 2829 2066  ( t.is_alive() f
+00017490: 6f72 2074 2069 6e20 7468 7265 6164 7320  or t in threads 
+000174a0: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
+000174b0: 6967 6e61 6c5f 7365 7276 6963 6528 290a  ignal_service().
+000174c0: 2020 2020 2020 2020 2020 2020 7469 6d65              time
+000174d0: 2e73 6c65 6570 2820 2e31 2029 0a20 2020  .sleep( .1 ).   
+000174e0: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
+000174f0: 6e3a 0a20 2020 2020 2020 206c 6f67 6769  n:.        loggi
+00017500: 6e67 2e65 7272 6f72 2820 224d 6169 6e20  ng.error( "Main 
+00017510: 7468 7265 6164 2045 7863 6570 7469 6f6e  thread Exception
+00017520: 3a20 2573 222c 2074 7261 6365 6261 636b  : %s", traceback
+00017530: 2e66 6f72 6d61 745f 6578 6328 2920 290a  .format_exc() ).
+00017540: 2020 2020 6669 6e61 6c6c 793a 0a20 2020      finally:.   
+00017550: 2020 2020 2023 2045 6974 6865 7220 7468       # Either th
+00017560: 6520 5765 6220 6f72 2074 6865 2043 7572  e Web or the Cur
+00017570: 7365 7320 4755 4920 636f 6d70 6c65 7465  ses GUI complete
+00017580: 642c 206f 7220 736f 6d65 7468 696e 6720  d, or something 
+00017590: 626c 6577 2075 702e 2020 5368 7574 2061  blew up.  Shut a
+000175a0: 6c6c 2074 6865 0a20 2020 2020 2020 2023  ll the.        #
+000175b0: 2074 6872 6561 6473 2064 6f77 6e2c 2072   threads down, r
+000175c0: 6573 746f 7265 2073 7973 2e73 7464 6f75  estore sys.stdou
+000175d0: 742f 7374 6465 7272 2061 6e64 2073 6176  t/stderr and sav
+000175e0: 6520 7374 6174 652e 0a20 2020 2020 2020  e state..       
+000175f0: 206c 6f67 6769 6e67 2e77 6172 6e69 6e67   logging.warning
+00017600: 2820 2243 6c65 616e 696e 6720 7570 2074  ( "Cleaning up t
+00017610: 6872 6561 6473 2220 290a 2020 2020 2020  hreads" ).      
+00017620: 2020 666f 7220 7420 696e 2074 6872 6561    for t in threa
+00017630: 6473 3a0a 2020 2020 2020 2020 2020 2020  ds:.            
+00017640: 742e 6a6f 696e 2820 7469 6d65 6f75 743d  t.join( timeout=
+00017650: 312e 3020 290a 2020 2020 2020 2020 7379  1.0 ).        sy
+00017660: 732e 7374 646f 7574 2c20 7379 732e 7374  s.stdout, sys.st
+00017670: 6465 7272 093d 2073 7973 5f73 7472 6561  derr.= sys_strea
+00017680: 6d5f 7361 7665 0a0a 2020 2020 2020 2020  m_save..        
+00017690: 6c6f 6767 696e 672e 696e 666f 2820 2253  logging.info( "S
+000176a0: 6176 696e 6720 7374 6174 652e 2e2e 2220  aving state..." 
+000176b0: 290a 2020 2020 2020 2020 6462 5f73 7461  ).        db_sta
+000176c0: 7465 5f73 6176 6528 290a 0a20 2020 2020  te_save()..     
+000176d0: 2020 2069 6620 6172 6773 2e70 726f 6669     if args.profi
+000176e0: 6c65 3a0a 2020 2020 2020 2020 2020 2020  le:.            
+000176f0: 7072 6f66 696c 6572 2e64 6973 6162 6c65  profiler.disable
+00017700: 2829 0a20 2020 2020 2020 2020 2020 2069  ().            i
+00017710: 6620 6172 6773 2e70 726f 6669 6c65 2021  f args.profile !
+00017720: 3d20 272d 273a 2020 2320 6f70 7469 6f6e  = '-':  # option
+00017730: 616c 6c79 2064 756d 7020 7374 6174 7320  ally dump stats 
+00017740: 746f 2061 2066 696c 656e 616d 650a 2020  to a filename.  
+00017750: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00017760: 6f66 696c 6572 2e64 756d 705f 7374 6174  ofiler.dump_stat
+00017770: 7328 2061 7267 732e 7072 6f66 696c 6520  s( args.profile 
+00017780: 290a 2020 2020 2020 2020 2020 2020 7072  ).            pr
+00017790: 6f66 0909 3d20 7073 7461 7473 2e53 7461  of..= pstats.Sta
+000177a0: 7473 2820 7072 6f66 696c 6572 2c20 7374  ts( profiler, st
+000177b0: 7265 616d 3d73 7973 2e73 7464 6572 7220  ream=sys.stderr 
+000177c0: 290a 2020 2020 2020 2020 2020 2020 7072  ).            pr
+000177d0: 696e 7428 2022 5c6e 5c6e 5449 4d45 3a22  int( "\n\nTIME:"
+000177e0: 2c20 6669 6c65 3d73 7973 2e73 7464 6572  , file=sys.stder
+000177f0: 7220 290a 2020 2020 2020 2020 2020 2020  r ).            
+00017800: 7072 6f66 2e73 6f72 745f 7374 6174 7328  prof.sort_stats(
+00017810: 2020 2774 696d 6527 2029 2e70 7269 6e74    'time' ).print
+00017820: 5f73 7461 7473 2820 7072 6f66 696c 6572  _stats( profiler
+00017830: 5f6c 696d 6974 2029 0a0a 2020 2020 2020  _limit )..      
+00017840: 2020 2020 2020 7072 696e 7428 2022 5c6e        print( "\n
+00017850: 5c6e 4355 4d55 4c41 5449 5645 3a22 2c20  \nCUMULATIVE:", 
+00017860: 6669 6c65 3d73 7973 2e73 7464 6572 7220  file=sys.stderr 
+00017870: 290a 2020 2020 2020 2020 2020 2020 7072  ).            pr
+00017880: 6f66 2e73 6f72 745f 7374 6174 7328 2020  of.sort_stats(  
+00017890: 2763 756d 756c 6174 6976 6527 2029 2e70  'cumulative' ).p
+000178a0: 7269 6e74 5f73 7461 7473 2820 7072 6f66  rint_stats( prof
+000178b0: 696c 6572 5f6c 696d 6974 2029 0a         iler_limit ).
```

### Comparing `crypto_licensing-3.0.4/crypto_licensing/licensing/verification.py` & `crypto_licensing-3.3.0/crypto_licensing/licensing/verification.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 # Crypto-licensing -- Cryptographically signed licensing, w/ Cryptocurrency payments
 #
 # Copyright (c) 2022, Dominion Research & Development Corp.
 #
 # Crypto-licensing is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
-# later version.  See the LICENSE file at the top of the source tree.
+# later version.  It is also available under alternative (eg. Commercial)
+# licenses, at your option.  See the LICENSE file at the top of the source tree.
 #
 # It is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
 # A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
 #
 
 from __future__ import absolute_import, print_function, division
@@ -38,15 +39,15 @@
 from . 			import doh
 from .defaults		import (
     DISTRIBUTION, LICPATTERN, LICEXTENSION, KEYPATTERN, KEYEXTENSION,
 )
 from ..misc		import (
     type_str_base, type_num_base, urlencode,
     parse_datetime, parse_seconds, Timestamp, Duration,
-    deduce_name, config_open, config_open_deduced,
+    config_open_deduced,
     token_bytes, is_mapping, is_listlike,
 )
 
 # Get Ed25519 support. Try a globally installed ed25519ll possibly with a CTypes binding, Otherwise,
 # try our local Python-only ed25519ll derivation, or fall back to the very slow D.J.Bernstein Python
 # reference implementation
 from .. import ed25519
@@ -390,15 +391,15 @@
     if machine is not None:
         if not isinstance( machine, uuid.UUID ):
             machine		= uuid.UUID( machine )
         assert machine.version == 4
     return machine
 
 
-def machine_UUIDv4( machine_id_path=None):
+def machine_UUIDv4( machine_id_path=None ):
     """Identify the machine-id as an RFC 4122 UUID v4. On Linux systems w/ systemd, get from
     /etc/machine-id, as a UUID v4: https://www.man7.org/linux/man-pages/man5/machine-id.5.html.
     On MacOS and Windows, use uuid.getnode(), which derives from host-specific data (eg. MAC
     addresses, serial number, ...).
 
     This UUID should be reasonably unique across hosts, but is not guaranteed to be.
 
@@ -1640,15 +1641,15 @@
 
     def verify(
         self,
         author_pubkey	= None,
         signature	= None,
         confirm		= None,
         machine_id_path	= None,
-        dependencies	= False,  # Default to not include this LicenseSigned in returned constraints['dependencies']
+        dependencies	= None,  # Defaults to not include this LicenseSigned in returned constraints['dependencies']
         **constraints
     ):
         """Verify that the License is valid:
 
             - Has properly signed License dependencies
               - Each public key can be confirmed, if desired
             - Complies with the bounds of any License dependencies
@@ -1736,15 +1737,16 @@
                     ))
 
         # Enforce all constraints, returning a dict suitable for creating a specialized License, if
         # a signature was provided; if not, we cannot produce a specialized sub-License, and must
         # fail.
 
         # First, scan the constraints to see if any are callable
-
+        if constraints:
+            log.info( "Enforcing constraints: {}".format( constraints ))
         # Verify all sub-license start/length durations comply with this License' duration.
         # Remember, these start/length specify the validity period of the License to be
         # sub-licensed, not the execution time of the installation!
         try:
             # Collect any things with .start/.length; all sub-Licenses dependencies, and a Timespan
             # representing any supplied start/length constraints in order to validate their
             # consistency with the sub-License start/lengths.
@@ -1993,22 +1995,25 @@
 
     def verify(
         self,
         author_pubkey	= None,
         signature	= None,
         confirm		= None,
         machine_id_path	= None,
+        dependencies	= None,
         **constraints
     ):
         return self.license.verify(
             author_pubkey	= author_pubkey or self.license.author.pubkey,
             signature		= signature or self.signature,
             confirm		= confirm,
             machine_id_path	= machine_id_path,
-            **constraints )
+            dependencies	= dependencies,
+            **constraints
+        )
 
 
 class KeypairPlaintext( Serializable ):
     """De/serialize the plaintext Ed25519 private and public key material.  Order of arguments is
     NOT the same as ed25519.Keypair, b/c the public vk is optional.
 
     """
@@ -2077,70 +2082,113 @@
     The 256-bit Ed25519 Keypair seed is encrypted using ChaCha20Poly1305 w/ the salt and derived
     key.  The salt and ciphertext are always serialized in hex, to illustrate that it is not Ed25519
     Keypair data.
 
     Can be supplied w/ a raw signing key or an ed25519.Keypair as an unencrypted key, along with
     username/password.  If no signing key at all is provided, one will be generated.
 
+    If possible, derives the public key and signs it, proving that the author did, indeed, have the
+    signing key corresponding to the public key.
+
     """
-    __slots__			= ('salt', 'ciphertext')
+    __slots__			= ('salt', 'ciphertext', 'vk', 'vk_signature')
     serializers			= dict(
         salt		= into_hex,
         ciphertext	= into_hex,
+        vk		= into_b64,
+        vk_signature	= into_b64,
     )
 
-    def __init__( self, sk=None, vk=None, salt=None, ciphertext=None, username=None, password=None,
+    def __init__( self, sk=None, vk=None, vk_signature=None, salt=None, ciphertext=None, username=None, password=None,
                   **kwds ):
-        if not ( bool( ciphertext and salt ) ^ bool( password and username )):
-            raise TypeError( "Insufficient arguments to create an Encrypted Keypair" )
-        if not ( ciphertext and salt ) and not sk:
+        has_encrypted		= ciphertext is not None and salt is not None
+        has_credentials		= password is not None and username is not None
+        if not ( has_encrypted or has_credentials ):
+            raise TypeError( "Insufficient arguments to create an Encrypted Keypair; either ciphertext/salt or password/username required" )
+        if not has_encrypted and not sk:
+            # Neither ciphertext supplied, nor plaintext signing key; must want a new Keypair
             sk			= authoring( why="No Keypair supplied to KeypairEncrypted" )
-        if hasattr( sk, 'sk' ):
-            # Provided with a raw ed25519.Keypair or KeypairPlaintext; extract its sk, and use any supplied vk for confirmation
-            _,edsk		= into_keys( sk )
-            sk			= into_b64( edsk )
+        elif sk:
+            # A signing key provided (and maybe also encrypted); lets get the private key bytes
+            if hasattr( sk, 'sk' ):
+                # Provided with a raw ed25519.Keypair or KeypairPlaintext; extract its sk, and use any supplied vk for confirmation
+                _,edsk		= into_keys( sk )
+                sk		= into_b64( edsk )
+            else:
+                sk		= into_bytes( sk, ('base64',) )
         if salt:
             self.salt		= into_bytes( salt, ('hex',) )
         else:
             # If salt not supplied, supply one -- but we obviously can't be given an encrypted seed!
             assert sk and not ciphertext, \
                 "Expected unencrypted keypair if no is salt provided"
             self.salt		= os.urandom( 12 )
         assert len( self.salt ) == 12, \
             "Expected 96-bit salt, not {!r}".format( self.salt )
+        # And, if a pubkey and/or pubkey signature provided, also get their bytes
+        vk			= into_bytes( vk, ('base64',) )
+        vk_signature		= into_bytes( vk_signature, ('base64',) )
+
+        # We've normalized everything provided into bytes; now produce/verify ciphertext
         if ciphertext:
             # We are provided with the encrypted seed (tag + ciphertext).  Done!  But, we don't know
             # the original Keypair, here, so we can't verify below.
             self.ciphertext	= into_bytes( ciphertext, ('hex',) )
             assert len( self.ciphertext ) * 8 == 384, \
                 "Expected 384-bit ChaCha20Poly1305-encrypted seed, not a {}-bit {!r}".format(
                     len( self.ciphertext ) * 8, self.ciphtertext )
             keypair		= None
         else:
             # We are provided with the unencrypted signing key.  We must encrypt the 256-bit private
             # key material to produce the seed ciphertext.  Remember, the Ed25519 private signing
             # key always includes the 256-bit public key appended to the raw 256-bit private key
             # material.
-            sk			= into_bytes( sk, ('base64',) )
             seed		= sk[:32]
-            keypair		= authoring( seed=seed, why="provided unencrypted signing key" )
+            keypair		= authoring( seed=seed, why="Signing key supplied to KeypairEncrypted" )
             if vk:
-                vk		= into_bytes( vk, ('base64',) )
                 assert keypair.vk == vk, \
                     "Failed to derive Ed25519 signing key from supplied data"
             key			= self.key( username=username, password=password )
             cipher		= ChaCha20Poly1305( key )
             plaintext		= bytearray( seed )
             nonce		= self.salt
             self.ciphertext	= bytes( cipher.encrypt( nonce, plaintext ))
         if username and password:
             # Verify MAC by decrypting w/ username and password, if provided
             keypair_rec		= self.into_keypair( username=username, password=password )
             assert keypair is None or keypair_rec == keypair, \
                 "Failed to recover original key after decryption"
+            if vk:
+                assert keypair_rec.vk == vk, \
+                    "Failed deriving Ed25519 signing key {} matching claimed public key {}".format(
+                        into_b64( keypair_rec.vk ), into_b64( vk ))
+            if sk:
+                assert keypair_rec.sk == sk, \
+                    "Failed deriving Ed25519 signing key {} matching claimed signing key {}".format(
+                        into_b64( keypair_rec.sk ), into_b64( sk ))
+            vk,sk		= keypair_rec
+        if vk:
+            if vk_signature:
+                # Verify supplied/deduced vk with provided vk_signature.  This allows us to validate
+                # that the supplied vk was self-signed, even if we never decrypt the ciphertext.
+                try:
+                    ed25519.crypto_sign_open( vk_signature + vk, vk )
+                except Exception as exc:
+                    raise_from( ValueError( "Failed to verify Ed25519 pubkey {} signature".format( into_b64( vk ))), exc )
+            elif sk:
+                # We have both vk and sk, either supplied or deduced, but no vk_signature.  Produce it.
+                vk_signature	= ed25519.crypto_sign( vk, sk )[:64]
+
+        # If an encrypted (ciphertext-only) is supplied, we will not be able to deduce the
+        # vk/vk_signature, and these will remain None.  Thus, only iff no username/password.
+        self.vk			= vk
+        self.vk_signature	= vk_signature
+        assert vk_signature or not has_credentials, \
+            "No pubkey signature deduced, but credentials are available: {}".format( self )
+
         super( KeypairEncrypted, self ).__init__( **kwds )
 
     def key( self, username, password ):
         # The username, which is often an email address, should be case-insensitive.
         username		= username.lower()
         username		= username.encode( 'UTF-8' )
         password		= password.encode( 'UTF-8' )
@@ -2180,122 +2228,125 @@
         how	= "Recover" if seed else "Created",
         pubkey	= into_b64( keypair.vk ),
         why	= " ({})".format( why ) if why else "",
     ))
     return keypair
 
 
+def save_keypair(
+    keypair,
+    why			= None,
+    extension		= None,
+    reverse_save	= None,
+    **kwds  # eg. {base,file}name, package, extra=["..."], reverse_save, other open() args; see config_open
+):
+    """
+    Successfully created new Keypair; now, try to create file; will not overwrite.
+    """
+    if why is None:
+        why			= "the"
+    for f in config_open_deduced(
+        mode		= "wb",
+        extension	= extension or KEYEXTENSION,  # But uses default extension on creation
+        reverse		= reverse_save,
+        skip		= False,  # For writing/creating, of course we don't want to "skip" anything...
+        **kwds
+    ):
+        try:
+            with f:
+                keypair.save( f )  # keypair._from preserves f.name
+        except Exception as exc:
+            log.detail( "Writing {why} Keypair to {path} failed: {exc}".format( why=why, path=f.name, exc=exc ))
+            raise NotRegistered( "Failed to register {why} Keypair: {exc}".format( why=why, exc=exc ))
+        else:
+            log.normal( "Wrote {why} Keypair to {path}: {pubkey}".format( why=why, path=keypair._from, pubkey=keypair['vk'] ))
+            break
+    else:
+        raise NotRegistered( "Failed to find a place to save {why} Keypair".format( why=why ))
+    return keypair._from
+
+
 def registered(
     seed		= None,
     why			= None,
     username		= None,		# The credentials for our agent's Keypair
     password		= None,
-    extension		= None,		# Defaults to exactly match KEYEXTENSION
-    basename		= None,
-    filename		= None,
-    package		= None,
-    registering		= True,		# By default, create a new Keypair if none found
-    reverse		= False,        # Default to save from most general location to most specific
-    extra		= None,		# any extra path(s) to consider
+    extension		= None,		# Use exactly this extension for searching/registering
+    registering		= None,		# True by default, create a new Keypair if none found
+    reverse_save	= None,		# None (False by default); saves from most general location to most specific
+    **kwds  # eg. {base,file}name, package, extra=["..."], reverse_save, other open() args; see config_open
 ):
     """Find an existing Keypair w/ the given basename and extension, or create an authoring Keypair
-    and save it, returning the Keypair.  By default, attempts to save in the most general (writable)
-    location possible, but will use the CWD if necessary.  Unlike load_keys, looks for an exact
-    match on the extension, not a pattern -- since that's exactly what we're trying to create.
+    and save it, returning the Keypair.  Always searches from the most specific to the most general
+    config location.  However, defaults to save in the most general (writable) location possible,
+    but will use the CWD if necessary.
 
     Will not overwrite an existing file of the same name, if found!  If the Keypair can be loaded
     with the given credentials, it is considered as registered and returned.  Otherwise, this is
     considered an error; you already have a Keypair regsitered with perhaps different credentials,
-    and you should probably be trying to 'load_keys' before you register a new Agent ID...
+    and you should probably be trying to 'load_keypairs' before you register a new Agent ID...
 
     Returns the resultant KeypairEntryped or KeypairPlaintext, w/ a ._from property == path.
 
     """
     if not why:
         why			= "End-user"
+    if registering is None:
+        registering		= True
     # See if the target Keypair already exists somewhere; if so, we don't want to overwrite it -- if
     # we can successfully load it, then consider the Keypair already registered.
     log.debug( "Looking for existing {why} Keypair...".format(
         why	= why,
     ))
     try:
-        (_,keypair,_,keypair_raw), = load_keys(
-            extension	= extension or KEYEXTENSION,  # Only files with exactly matching extension
+        _,keypair,_,keypair_raw = next( load_keypairs(
+            extension	= extension or KEYPATTERN,  # Uses the glob pattern for searching
             username	= username,
             password	= password,
-            basename	= basename,
-            filename	= filename,
-            package	= package,
-            reverse	= reverse,
-            extra	= extra,
             detail	= True,
-        )
-    except ValueError as exc:
-        log.info( "Looking for existing {why} Keypair failed: {exc}".format(
+            **kwds
+        ))
+    except StopIteration:
+        log.info( "Looking for existing {why} Keypair failed: no Keypair found".format(
             why		= why,
-            exc		= exc,
         ))
         pass
     else:
         log.normal( "Found {why} Keypair at {path}: {pubkey}".format(
             why		= why,
             path	= keypair._from,
             pubkey	= into_b64( keypair_raw.vk ),
         ))
         return keypair
+
     if not registering:
         raise NotRegistered( "Failed to find a {why} Keypair; registering a new one was declined".format(
             why		= why,
         ))
 
     # Not already registered, and registering is desired; create one.
-    keypair_raw			= authoring( seed=seed, why=why )
+    keypair_raw			= authoring(
+        seed		= seed,
+        why		= why )
     if username and password:
         keypair			= KeypairEncrypted(
             sk		= keypair_raw.sk,
             username	= username,
             password	= password,
         )
     else:
         keypair			= KeypairPlaintext(
             sk		= keypair_raw.sk,
         )
 
-    # Successfully created new Keypair; now, try to create file; will not overwrite
-    for f in config_open_deduced(
-        basename	= basename,
-        mode		= "wb",
-        extension	= extension or KEYEXTENSION,
-        filename	= filename,
-        package		= package,
-        reverse		= reverse,
-        extra		= extra,
-        skip		= None,  # For writing/creating, of course we don't want to "skip" anything...
-    ):
-        try:
-            with f:
-                keypair.save( f )  # keypair._from preserves f.name
-        except Exception as exc:
-            log.detail( "Writing {why} Keypair to {path} failed: {exc}".format(
-                why	= why,
-                path	= f.name,
-                exc	= exc,
-            ))
-            raise NotRegistered( "Failed to register new Keypair: {exc}".format( exc=exc ))
-        else:
-            log.normal( "Wrote {why} Keypair to {path}: {pubkey}".format(
-                why	= why,
-                path	= keypair._from,
-                pubkey	= into_b64( keypair_raw.vk ),
-            ))
-            break
-    else:
-        raise NotRegistered( "Failed to find a place to save a new {why} Keypair".format(
-            why		= why,
-        ))
+    save_keypair(
+        keypair,
+        reverse_save	= reverse_save,
+        **kwds
+    )
     return keypair
 
 
 def issue(
     license,
     author_sigkey,
     signature		= None,
@@ -2325,31 +2376,60 @@
         license,
         author_sigkey,
         signature	= signature,
         confirm		= confirm,
         machine_id_path	= machine_id_path )
 
 
+def save(
+    provenance,
+    why			= None,
+    extension		= None,
+    reverse_save	= None,
+    **kwds  # eg. {base,file}name, package, extra=["..."], reverse_save, other open() args; see config_open
+):
+    """
+    Successfully created License; now, try to create file; will not overwrite.  Returns the saved License's path.
+    """
+    if why is None:
+        why			= "the"
+    for f in config_open_deduced(
+        mode		= "wb",
+        extension	= extension or LICEXTENSION,
+        skip		= False,  # For writing/creating, of course we don't want to "skip" anything...
+        reverse		= reverse_save,
+        **kwds
+    ):
+        try:
+            with f:
+                provenance.save( f )  # LicenseSigned._from preserves f.name
+        except Exception as exc:
+            log.detail( "Writing {why} License to {path} failed: {exc}".format( why=why, path=f.name, exc=exc ))
+            raise NotLicensed( "Failed to save {why} License: {exc}".format( why=why, exc=exc ))
+        else:
+            log.normal( "Wrote {why} License to {path}".format( why=why, path=provenance._from ))
+            break
+    else:
+        raise NotLicensed( "Failed to find a place to save {why} License".format( why=why ))
+    return provenance._from
+
+
 def license(
     author,				# w/ a .keypair, or
     author_sigkey	= None,		# an separate signing key
     why			= None,
     client		= None,		# If no designated client, allow anyone to sub-License
     dependencies	= None,		# Any Licenses this License depends on
     machine		= None,
     timespan		= None,
     grant		= None,
     machine_id_path	= None,
     confirm		= None,		# Validate License' author.pubkey from DNS
     extension		= None,		# Defaults to exactly match LICEXTENSION
-    basename		= None,
-    filename		= None,
-    package		= None,
-    reverse		= False,        # Default to save from most general location to most specific
-    extra		= None,		# any extra path(s) to consider
+    **kwds  # eg. {base,file}name, package, extra=["..."], reverse_save, other open() args; see config_open
 ):
     """Create a License w/ the specified author and grant(s), and save it, returning the path.  By
     default, attempts to save in the most general (writable) location possible, but will use the CWD
     if necessary.
 
     Will not overwrite an existing file of the same name, if found!  This is considered an error;
     you should probably be trying to 'check' before you save a License w/ the same basename and extension.
@@ -2379,127 +2459,105 @@
     except Exception as exc:
         log.detail( "Creating {why} License failed: {exc}".format(
             why		= why,
             exc		= exc,
         ))
         raise NotLicensed( "Failed to save a new License: {exc}".format( exc=exc ))
     else:
-        # Successfully created License; now, try to create file; will not overwrite
-        for f in config_open_deduced(
-            basename		= basename,
-            mode		= "wb",
-            extension		= extension or LICEXTENSION,
-            filename		= filename,
-            package		= package,
-            reverse		= reverse,
-            extra		= extra,
-            skip		= None,  # For writing/creating, of course we don't want to "skip" anything...
-        ):
-            try:
-                with f:
-                    provenance.save( f )  # LicenseSigned._from preserves f.name
-            except Exception as exc:
-                log.detail( "Writing {why} License to {path} failed: {exc}".format(
-                    why		= why,
-                    path	= f.name,
-                    exc		= exc,
-                ))
-                raise NotLicensed( "Failed to issue new License: {exc}".format( exc=exc ))
-            else:
-                log.normal( "Wrote {why} License to {path}".format(
-                    why		= why,
-                    path	= provenance._from,
-                ))
-                break
-        else:
-            raise NotLicensed( "Failed to find a place to save a new {why} License".format(
-                why	= why,
-            ))
-        return provenance
+        log.detail( "Created License provenance {}".format( provenance ))
+
+    save(
+        provenance,
+        extension	= extension,
+        why		= why,
+        **kwds
+    )
+    return provenance
 
 
 def verify(
     provenance,
     author_pubkey	= None,
     signature		= None,
     confirm		= None,
     machine_id_path	= None,
-    dependencies	= True,
+    dependencies	= None,
     **constraints
 ):
     """Verify that the supplied License or LicenseSigned contains a valid signature, and that the
     License follows the rules in all of its License dependencies.  Optionally, 'confirm' the
     validity of any public keys.
 
     Apply any additional constraints, returning a License serialization dict satisfying them.  If
     you plan to issue a new LicenseSigned, it is recommended to include your author, author_domain
     and product names, and perhaps also the client and client_pubkey of the intended License
     recipient.
 
     Works with either a License and signature= keyword parameter, or a LicenseSigned provenance.
 
-    Defaults to demands that any LicenseSigned dependencies are included in the resultant remaining
-    constraints, so that a sub-License can be produced.
+    Defaults to demand that any supplied LicenseSigned dependencies are included in the resultant
+    remaining constraints.  If None, by default (unlike the License{Signed}.verify), includes the
+    target LicenseSigned in the returned constraints required, so that a sub-License for the
+    verified License can be produced.
+
+    Therefore, when you have a LicenseSigned or a License + a signature, calling verify( <lic> ... )
+    will return a requirements dict ready to pass to License, along with an author and (optionally)
+    designated client Agent, with the target verified License itself in the dependencies list,
+    producing a new License which sub-licenses the just verified License.
 
     """
     return provenance.verify(
         author_pubkey	= author_pubkey,
         signature	= signature or provenance.signature,
         confirm		= confirm,
         machine_id_path	= machine_id_path,
-        dependencies	= dependencies,
-        **constraints )
+        dependencies	= True if dependencies is None else dependencies,
+        **constraints
+    )
 
 
 def load(
-    basename		= None,
-    mode		= None,
-    extension		= None,
-    confirm		= None,
-    machine_id_path	= None,
-    filename		= None,
-    package		= None,
-    skip		= "*~",
-    **kwds  # eg. extra=["..."], reverse=False, other open() args; see config_open
+    mode	= None,
+    extension	= None,
+    confirm	= None,
+    machine_id_path = None,
+    **kwds  # eg. {base,file}name, package, extra=["..."], reverse_save, other open() args; see config_open
 ):
     """Open and load all crypto-lic[ens{e,ing}] file(s) found on the config path(s) (and any
     extra=[...,...]  paths) containing a LicenseSigned provenance record.  By default, use the
     provided package's (your __package__) name, or the executable filename's (your __file__)
     basename.  Assumes '<basename>.crypto-lic*', if no extension provided.
 
     Applies glob pattern matching via config_open....
 
     Yields the resultant (filename, LicenseSigned) provenance(s), or an Exception if any
     glob-matching file is found that doesn't contain a serialized LicenseSigned.
 
     """
-    name		= deduce_name(
-        basename=basename, extension=extension or LICPATTERN,
-        filename=filename, package=package )
-    for f in config_open( name=name, mode=mode, skip=skip, **kwds ):
+    for f in config_open_deduced(
+        extension	= extension or LICPATTERN,
+        mode		= mode,
+        **kwds
+    ):
         with f:
             prov_ser		= f.read()
             prov_dict		= json.loads( prov_ser )
             prov		= LicenseSigned(
                 confirm=confirm, machine_id_path=machine_id_path, _from=f.name, **prov_dict )
         yield prov._from, prov
 
 
-def load_keys(
-    basename	= None,
+def load_keypairs(
     mode	= None,
     extension	= None,
-    filename	= None,
-    package	= None,		# For deduction of basename
     username	= None,
     password	= None,		# Decryption credentials to use
     every	= False,
     detail	= False,        # Yield every file w/ origin + credentials info or exception?
-    skip	= "*~",
-    **kwds                      # eg. extra=["..."], reverse=False, other open() args; see config_open
+    **kwds  # eg. {base,file}name, package, extra=["..."], reverse_save, other open() args; see config_open
 ):
     """Load Ed25519 signing Keypair(s) from glob-matching file(s) with any supplied credentials.
     Yields all Encrypted/Plaintext Keypairs successfully opened (may be none at all), as a sequence
     of:
 
         <filename>, <Keypair/Exception>
 
@@ -2536,22 +2594,14 @@
     Unencrypted Keypair:
 
         {
             "sk":"bw58LSvuadS76jFBCWxkK+KkmAqLrfuzEv7ly0Y3lCLSE2Y01EiPyZjxirwSjHoUf9kz9meeEEziwk358jthBw=="
             "vk":"qZERnjDZZTmnDNNJg90AcUJZ+LYKIWO9t0jz/AzwNsk="
         }
 
-    Unencrypted Keypair from just 256-bit seed (which is basically the first half of a full .sk
-    signing key with a few bits normalized), and optional public key .vk to verify:
-
-        {
-            "seed":"bw58LSvuadS76jFBCWxkK+KkmAqLrfuzEv7ly0Y3lC=",
-            "vk":"qZERnjDZZTmnDNNJg90AcUJZ+LYKIWO9t0jz/AzwNsk="
-        }
-
     384-bit ChaCha20Poly1503-Encrypted seed (ya, don't use a non-random salt...):
         {
             "salt":"000000000000000000000000",
             "ciphertext":"d211f72ba97e9cdb68d864e362935a5170383e70ea10e2307118c6d955b814918ad7e28415e2bfe66a5b34dddf12d275"
         }
 
     NOTE: For encrypted Keypairs, we do not need to save the "derivation" we use to arrive at
@@ -2561,20 +2611,16 @@
     If NO ...Keypairs at all are found, TODO
 
     """
     issues			= {}		# { "name": [ <Exception>, ... ]
     tried			= 0		# How many files seen and tried
     found			= 0		# How many Keypairs successfully found
     for f in config_open_deduced(
-        basename	= basename,
         extension	= extension or KEYPATTERN,
-        filename	= filename,
-        package		= package,
         mode		= mode,
-        skip		= skip,
         **kwds
     ):
         tried		       += 1
         f_name			= f.name
         try:
             with f:
                 f_ser		= f.read()
@@ -2586,15 +2632,15 @@
             issues.setdefault( f_name, [] )
             issues[f_name].append( exc )
             continue
         # Attempt to recover the different Keypair...() types, from most stringent requirements to least.
         encrypted		= None
         try:
             try:
-                encrypted	= KeypairEncrypted( **keypair_dict )  # accepts ciphertext, salt
+                encrypted	= KeypairEncrypted( username=username, password=password, **keypair_dict )
             except TypeError as exc:  # Incorrect arguments, ...
                 raise_from( TypeError( "Keypair w/ keywords {} probably isn't a KeypairEncrypted: {}".format(
                     ', '.join( keypair_dict ), exc
                 )), exc )
             keypair		= encrypted.into_keypair( username=username, password=password )
             log.info( "Recover Ed25519 KeypairEncrypted w/ Public key: {} (from {}) w/ credentials {} / {}".format(
                 into_b64( keypair.vk ), f_name, username, '*' * len( password )))
@@ -2660,47 +2706,49 @@
 
 
 def key_lic_sequence_logger( func ):
     """Logs a sequence of <Keypair>,<License>, including _from (if available)"""
     @wraps( func )
     def wrapper( *args, **kwds ):
         labelled		= False
-        for key,lic in func( *args, **kwds ):
-            level		= logging.NORMAL if key and lic else logging.DETAIL
-            if log.isEnabledFor( level ):
-                if not labelled:
-                    log.normal( "{:56} {:20} {:20} {:16}: {}".format(
-                        'License', 'Client', 'Author', 'Product', 'Keypair'
+        func_iter		= func( *args, **kwds )
+        try:
+            payload		= None
+            while True:
+                key,lic		= func_iter.send( payload )
+                level		= logging.NORMAL if key and lic else logging.DETAIL
+                if log.isEnabledFor( level ):
+                    if not labelled:
+                        log.normal( "{:56} {:20} {:20} {:16}: {}".format(
+                            'License', 'Client', 'Author', 'Product', 'Keypair'
+                        ))
+                        labelled	= True
+                    log.log( level, "{:56} {:20.20} {:20.20} {:16.16}: {}{}".format(
+                        'N/A' if not hasattr( lic, '_from' ) or not lic._from else os.path.basename( lic._from ),
+                        'N/A' if not lic or not lic.license.client else "{}/{}".format( lic.license.client.name, into_b64( lic.license.client.pubkey )),
+                        'N/A' if not lic else "{}/{}".format( lic.license.author.name, into_b64( lic.license.author.pubkey )),
+                        'N/A' if not lic or not lic.license.author.product else lic.license.author.product,
+                        'N/A' if not key else into_b64( key.vk ), key._from if hasattr( key, '_from' ) else '',
                     ))
-                    labelled	= True
-                log.log( level, "{:56} {:20.20} {:20.20} {:16.16}: {}{}".format(
-                    'N/A' if not hasattr( lic, '_from' ) or not lic._from else os.path.basename( lic._from ),
-                    'N/A' if not lic or not lic.license.client else "{}/{}".format( lic.license.client.name, into_b64( lic.license.client.pubkey )),
-                    'N/A' if not lic else "{}/{}".format( lic.license.author.name, into_b64( lic.license.author.pubkey )),
-                    'N/A' if not lic or not lic.license.author.product else lic.license.author.product,
-                    'N/A' if not key else into_b64( key.vk ), key._from if hasattr( key, '_from' ) else '',
-                ))
-            yield key,lic
+                payload		= ( yield key,lic )
+        except StopIteration:
+            pass
     return wrapper
 
 
 def check_nolog(
-    basename		= None,			# Keypair/License file basename and open mode
     mode		= None,
     extension_keypair	= None,
     extension_license	= None,
-    filename		= None,			# ...or, deduce basename from supplied data
-    package		= None,
     username		= None,			# Keypair protected w/ supplied credentials
     password		= None,
     confirm		= None,
     machine_id_path	= None,
     constraints		= None,
-    skip		= "*~",
-    **kwds					# eg. extra=["..."], reverse=False, other open() args; see config_open
+    **kwds  # eg. {base,file}name, package, extra=["..."], reverse_save, other open() args; see config_open
 ):
     """Load our agent key(s), check that License(s) have been (or can be) issued to our agent, for
     this machine and/or username, yielding a sequence of:
 
         (None,None)			- nothing, if no Keypair could be found w/ given credentials
         (<Keypair>,None,)		- if Keypair found, but no Licenses available
         (<Keypair>,<LicenseSigned>)	- if Keypair and issued License(s) found
@@ -2723,31 +2771,35 @@
     one machine and/or for one username usually doesn't transfer to another machine/username.
 
         <basename>-<machine-id>.crypto-key...
         <basename>-<machine-id>.crypto-lic...
 
     """
     # Load any Keypair{Plaintext,Encrypted} available, and convert to a ed25519.Keypair,
-    # ready for signing/verification.  Retains orders of load_keys / load.
+    # ready for signing/verification.  Retains orders of load_keypairs / load.
     keypairs			= list(
         (key_path, keypair_or_error)
-        for key_path, keypair_typed, cred, keypair_or_error in load_keys(
-            basename=basename, mode=mode, extension=extension_keypair,
-            filename=filename, package=package,
-            every=True, detail=True,
-            username=username, password=password,
-            skip=skip, **kwds
+        for key_path, keypair_typed, cred, keypair_or_error in load_keypairs(
+            username	= username,
+            password	= password,
+            mode	= mode,
+            extension	= extension_keypair,
+            every	= True,
+            detail	= True,
+            **kwds
         )
         if isinstance( keypair_or_error, ed25519.Keypair )
     )
 
     licenses			= list( load(
-        basename=basename, mode=mode, extension=extension_license,
-        filename=filename, package=package,
-        confirm=confirm, machine_id_path=machine_id_path, skip=skip, **kwds
+        mode		= mode,
+        extension	= extension_license,
+        confirm		= confirm,
+        machine_id_path	= machine_id_path,
+        **kwds
     ))
 
     # See if license(s) has been (or can be) issued to our Agent keypair(s) (ie. was issued to this
     # keypair as a specific client_pubkey or was non-client-specific, and then was signed by our
     # Keypair), for this Machine ID.
     matches			= 0
     key_seen			= set()  # of Ed25519.Keypair.vk.  No keys loaded --> yield None,None
@@ -2857,26 +2909,21 @@
 
 @key_lic_sequence_logger
 def authorized(
     author,					# Details of the author's product we're licensing
     client		= None,			# ..and the intended specific client Agent
     username		= None,			# The credentials for our client Agent's Keypair
     password		= None,
-    basename		= None,
-    filename		= None,
-    package		= None,
     confirm		= None,
     machine_id_path	= None,
     constraints		= None,			# The additional constraints required of the author's license (if any)
-    registering		= True,			# If necessary, create a new Keypair (register a new License client)
-    acquiring		= True,			# If necessary, obtain/create a new License
-    reverse		= True,			# Default to look from most specific, to most general location
-    reverse_save	= None,			# Default to save in the opposite of look-up (most general, to most specific location)
-    extra		= None,
-    skip		= "*~",
+    registering		= None,			# Default (to True) if necessary, create a new Keypair (register a new License client)
+    acquiring		= None,			# Default (to True) if necessary, obtain/create a new License
+    reverse_save	= None,
+    **kwds  # eg. {base,file}name, package, extra=["..."], reverse_save, other open() args; see config_open
 ):
     """If possible, load and verify the agent's KeyPair (creating one if necessary).
 
     Obtain any LicenseSigned provenances, and sift through them for any that authorize usage of the
     given author's domain and product, to the given client, for a certain space and time, and
     satisfying any constraints.
 
@@ -2900,43 +2947,43 @@
 
     Otherwise, use the agent's Keypair to obtain a License for the specified remaining capability/constraints.
 
     Yields the discovered sequence of KeyPair, License found.
         - (None, None): No Keypair found
 
     """
+    if registering is None:
+        registering		= True
+    if acquiring is None:
+        acquiring		= True
+
     class State( Enum ):
         INITIAL		= 0
         CHECKING	= 1
         REGISTERING	= 2
         LICENSING	= 3
         DONE		= 4
 
+    credentials_seen		= { (username,password) }
     licenses			= dict()        # Remember all Keypair... --> [ License, ... ] under current credentials
     state			= State.INITIAL
     while state is not State.DONE:
         state			= State( state.value + 1 )
         log.detail( "{state}".format( state=state ))
         if state is State.CHECKING:
             # Look for Agent Keypairs and any associated Licenses issued to it, filtered by the
             # Author we're looking for.  We want to keep CHECKING, again and again, while the
             # caller provides new credentials.
-            credentials			= None
             for key,lic in check_nolog(
                 username	= username,
                 password	= password,
-                basename	= basename,
-                filename	= filename,
-                package		= package,
                 confirm		= confirm,
                 constraints	= constraints,
                 machine_id_path	= machine_id_path,
-                reverse		= reverse,
-                extra		= extra,
-                skip		= skip,
+                **kwds
             ):
                 if key is None:
                     assert lic is None, \
                         "No Agent ID KeyPair; should not have found a License {}".format( lic )
                     # No KeyPair, and no new credentials provided.  Give them the opportunity to
                     # enter new Credentials by falling to end of loop; if none provided, then assume
                     # they want to go through the proceess; advance to REGISTERING.
@@ -2994,22 +3041,24 @@
                     licenses[key].append( lic )
 
                 # Otherwise, we've found at least one passable license (or <key>,None or None,None).
                 # Keep yielding them 'til the caller finds one that satisfies their requirements --
                 # they might have purchased multiple licenses, and could be accumulating their
                 # grants.  If we're back here, they haven't (yet) found one; yield the next
                 # (collecting any .send( (username,password) )
-                credentials		= yield key,lic
-                if credentials:
+                credentials		= ( yield key,lic )
+                if credentials and credentials not in credentials_seen:
                     # The caller supplied new credentials via .send( (username,password) ).  Restart
-                    # the License authorization process using the new credentials.  (We do this test
-                    # here (not at the start of the loop), to catch the case where only None,None is
-                    # yielded from check).
+                    # the License authorization process using the new credentials, IFF they are
+                    # different from previously seen credentials.  (We do this test here (not at the
+                    # start of the loop), to catch the case where only None,None is yielded from
+                    # check).
                     licenses		= dict()
                     username,password	= credentials
+                    credentials_seen.add( credentials )
                     state		= State.INITIAL
                     break
             else:
                 # Out of licenses; none satisfactory, but if we do have an Agent ID, continue as if we've
                 # just completed REGISTER, and proceed to LICENSE.  Otherwise, fall thru to REGISTERING.
                 if licenses:
                     state	= State.REGISTERING
@@ -3019,19 +3068,17 @@
             # None/'' is supplied for either credential, an unencrypted Keypair will be produced.
             if not registering:
                 raise NotRegistered( "No Keypair found; request registering one, or provide different credentials" )
             key			= registered(
                 why		= "End-user Keypair",
                 username	= username,
                 password	= password,
-                basename	= basename,
-                filename	= filename,
-                package		= package,
-                reverse		= not reverse if reverse_save is None else reverse_save,
                 registering	= True,
+                reverse_save	= reverse_save,
+                **kwds
             )
             log.detail( "{state}: {action} {key}".format(
                 state	= state,
                 action	= "Loaded " if key._from else "Created",
                 key	= key ))
             licenses		= { key: [] }
 
@@ -3040,18 +3087,19 @@
             # the caller is trying to accumulate all available Licenses, and can't know when no more
             # are available.  As they accumulate Licenses, looking for a certain accumulation of
             # License.grants(), the final remaining required Grant should be supplied.
             if acquiring and len( licenses ) != 1:
                 log.normal( "{state}, w/ {keys} Agent IDs available -- enter different credentials?".format(
                     state	= state,
                     keys	= len( licenses )))
-                credentials	= yield None, None
-                if credentials:
+                credentials	= ( yield None, None )
+                if credentials and credentials not in credentials_seen:
                     licenses		= dict()
                     username,password	= credentials
+                    credentials_seen.add( credentials )
                     state		= State.INITIAL
                 else:
                     # No keypairs (or too many), no new credentials.  We're done the authorize process.
                     log.warning( "{state}: {which} Agent Keypair; Not acquiring a License".format(
                         state	= state,
                         which	= "No" if not license else "Ambiguous",
                     ))
@@ -3064,15 +3112,17 @@
                 continue
             # One Agent Keypair; try to obtain a License
             key,	= licenses.keys()
             log.normal( "{state}, w/ Agent ID {agent}; attempting licensing".format(
                 state	= state,
                 agent	= into_b64( key.vk ),
             ))
-            # TODO
 
+            #
+            # TODO: obtain a License
+            #
         else:
             log.normal( "{state}, w/ {keys} Agent IDs and {lics} Licenses found".format(
                 state	= state,
                 keys	= len( licenses ),
                 lics	= sum( len( licenses ) for _,licenses in licenses.items() ),
             ))
```

### Comparing `crypto_licensing-3.0.4/crypto_licensing/licensing/verification_test.py` & `crypto_licensing-3.3.0/crypto_licensing/licensing/verification_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from dns.exception	import DNSException
 from .verification	import (
     License, LicenseSigned, LicenseIncompatibility, Timespan, Agent,
     KeypairPlaintext, KeypairEncrypted, machine_UUIDv4,
     domainkey, domainkey_service, overlap_intersect,
     into_b64, into_hex, into_str, into_str_UTC, into_JSON, into_keys, into_bytes,
     into_Timestamp, into_Duration,
-    authoring, issue, verify, load, load_keys, check, authorized,
+    authoring, issue, verify, load, load_keypairs, check, authorized,
     DKIM_pubkey, DKIMError,
 )
 from ..			import ed25519
 
 from ..misc 		import (
     deduce_name, Timestamp
 )
@@ -160,22 +160,29 @@
     )
     assert kp_e.into_keypair( username=username, password=password ) == enduser_keypair
 
     kp_e_ser			= str( kp_e )
     assert kp_e_ser == """\
 {
     "ciphertext":"d211f72ba97e9cdb68d864e362935a5170383e70ea10e2307118c6d955b814918ad7e28415e2bfe66a5b34dddf12d275",
-    "salt":"000000000000000000000000"
+    "salt":"000000000000000000000000",
+    "vk":"O2onvM62pC1io6jQKm8Nc2UyFXcd4kOmOsBIoYtZ2ik=",
+    "vk_signature":"YxRSIqHzZs5lfmWYm09wdKS8QJPSunH/Gjty/MQN5PQ3B+HkDeMtspXLWE9qbwYPGcNd1pBGaGpWAxW10l6RBg=="
 }"""
     kp_r			= KeypairEncrypted( **json.loads( kp_e_ser ))
     assert str( kp_r ) == kp_e_ser
 
-    # We can also reconstruct from just seed and salt
+    # We can also reconstruct from just seed and salt (but no kv/vk_signature will be available
     kp_e2			= KeypairEncrypted( salt=salt, ciphertext=kp_e.ciphertext )
-    assert str( kp_e2 ) == kp_e_ser
+    assert str( kp_e2 ) == """\
+{
+    "ciphertext":"d211f72ba97e9cdb68d864e362935a5170383e70ea10e2307118c6d955b814918ad7e28415e2bfe66a5b34dddf12d275",
+    "salt":"000000000000000000000000"
+}"""
+
     assert kp_e.into_keypair( username=username, password=password ) \
         == kp_r.into_keypair( username=username, password=password ) \
         == kp_e2.into_keypair( username=username, password=password )
 
     awesome_keypair		= into_keys( awesome_sigkey )
     kp_a			= KeypairEncrypted(
         salt		= b'\x01' * 12,
@@ -185,32 +192,34 @@
     )
     assert kp_a.into_keypair( username=username, password=password )[1] == awesome_keypair[1]
 
     kp_a_ser			= str( kp_a )
     assert kp_a_ser == """\
 {
     "ciphertext":"aea5129b033c3072be503b91957dbac0e4c672ab49bb1cc981a8955ec01dc47280effc21092403509086caa8684003c7",
-    "salt":"010101010101010101010101"
+    "salt":"010101010101010101010101",
+    "vk":"cyHOei+4c5X+D/niQWvDG5olR1qi4jddcPTDJv/UfrQ=",
+    "vk_signature":"yaxxz6ZxCWFdtgRF1JnK+k46UYjv650f/J1yHHf9olUpLXR/KrBOrAD71cC/dAc2FVOTqzCv1S5IXhULho2QAg=="
 }"""
 
 
 @pytest.mark.skipif( not chacha20poly1305, reason="Needs ChaCha20Poly1305" )
-def test_KeypairEncrypted_load_keys():
+def test_KeypairEncrypted_load_keypairs():
     enduser_keypair		= authoring( seed=enduser_seed, why="from enduser seed" )
-    # load just the one encrypted cpppo-keypair (no glob wildcard on extension)
-    (keyname,keypair_encrypted,keycred,keypair), = load_keys(
+    # load just the one encrypted crypto-keypair (no glob wildcard on extension)
+    (keyname,keypair_encrypted,keycred,keypair), = load_keypairs(
         extension="crypto-keypair", username=username, password=password,
         extra=[os.path.dirname( __file__ )], filename=__file__, detail=True )
     assert keycred == dict( username=username, password=password )
     assert enduser_keypair == keypair_encrypted.into_keypair( **keycred ) == keypair
 
 
-def test_KeypairPlaintext_load_keys():
+def test_KeypairPlaintext_load_keypairs():
     enduser_keypair		= authoring( seed=enduser_seed, why="from enduser seed" )
-    (keyname,keypair_plaintext,keycred,keypair), = load_keys(
+    (keyname,keypair_plaintext,keycred,keypair), = load_keypairs(
         extension="crypto-keypair-plaintext",
         extra=[os.path.dirname( __file__ )], filename=__file__, detail=True )
     assert keycred == {}
     assert enduser_keypair == keypair_plaintext.into_keypair( **keycred ) == keypair
 
 
 def test_License_serialization():
@@ -482,18 +491,22 @@
     #    - This is normally done in a company License Server, which holds the
     #      master license and issues specialized ones up to the purchased limits (eg. 10 machines)
     # 3) Derive a new License, specialized for the host's machine-id UUID
     #    - This will be a LicenseSigned by the company License server using the company's key,
     #    - Its client_pubkey will match this software installation's private key, and machine-id UUID
     # 4) Save to <application>.crypto-license in application's config path
 
-    # Lets specialize the license for a specific machine, and with a specific start time
+    # Lets specialize the license for a specific machine, and with a specific start time.  The
+    # default will include the just-verified license in the resultant dependencies (ie. same as if
+    # dependencies=[drv_prov] was provided)
     lic_host_dict		= verify(
-        drv_prov, confirm=False, machine_id_path=machine_id_path,
-        machine	= True,
+        drv_prov,
+        confirm		= False,
+        machine_id_path	= machine_id_path,
+        machine		= True,
         timespan	= Timespan( "2022-09-28 08:00:00 Canada/Mountain" ),
     )
     lic_host_dict_str = into_JSON( lic_host_dict, indent=4, default=str )
     print( lic_host_dict_str )
     assert lic_host_dict_str == """\
 {
     "dependencies":[
```

### Comparing `crypto_licensing-3.0.4/crypto_licensing/misc.py` & `crypto_licensing-3.3.0/crypto_licensing/misc.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 # Crypto-licensing -- Cryptographically signed licensing, w/ Cryptocurrency payments
 #
 # Copyright (c) 2022, Dominion Research & Development Corp.
 #
 # Crypto-licensing is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
-# later version.  See the LICENSE file at the top of the source tree.
+# later version.  It is also available under alternative (eg. Commercial)
+# licenses, at your option.  See the LICENSE file at the top of the source tree.
 #
 # It is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
 # A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
 #
 
 from __future__ import absolute_import, print_function, division
@@ -868,127 +869,165 @@
 
     This is the order that is required by configparser; settings configured in "later" files
     override those in "earlier" ones.
 
     For other purposes (eg. loading complete files), the order is likely reversed!  The caller must
     do this manually.
 
+    By default, the "current" directory '.' will be used last, in the absence of any specific
+    'extra' directories.  For example, when searching for things, the current directory (most
+    specific) might be searched first, then most general directories.  However, for writing/saving
+    things, the most general writable directory might be used, and then (finally) the 'extra' or
+    current directory if that's the only writable place.  The reason we don't *always* use '.' if
+    other 'extra' directories are provided, is to allow the caller to *avoid* searching/writing
+    in/to the current directory!  Include '.' somewhere in 'extras' if this is appropriate.
+
     """
     yield os.path.join( os.getenv( 'APPDATA', os.sep + 'etc' ), filename )      # global app data dir, eg. /etc/ (most general)
     yield os.path.join( os.path.expanduser( '~' ), '.'+CONFIG_BASE, filename )  # user dir, ~username/.crypto-licensing/name
     yield os.path.join( os.path.expanduser( '~' ), '.' + filename )		# user dir, ~username/.name
-    for e in extra or []:							# any extra dirs...
-        yield os.path.join( e, filename )
-    yield filename								# relative to current working dir (most specific)
-
+    for e in ( [ '.' ] if extra is None else extra ):				# any extra dirs...
+        yield os.path.join( e, filename )					# default; relative to current working dir (most specific)
 
-# Default configuration files path, In 'configparser' expected order (most general to most specific)
-config_files			= list( config_paths( CONFIG_FILE ))
 
 try:
     ConfigNotFoundError		= FileNotFoundError
 except NameError:
     ConfigNotFoundError		= IOError		# Python2 compatibility
 
 
 class ConfigFoundError( KeyError ):
     pass
 
 
-def config_open( name, mode=None, extra=None, skip=None, reverse=True, overwrite=False, **kwds ):
-    """Find and open all glob-matched file name(s) found on the standard or provided configuration file
-    paths (plus any extra), in most general to most specific order.  Yield the open file(s), or
-    raise a ConfigNotFoundError (a FileNotFoundError or IOError in Python3/2 if no matching file(s)
-    at all were found, to be somewhat consistent with a raw open() call).
-
-    We traverse these in reverse order by default: nearest and most specific, to furthest and most
-    general, and any matching file(s) in ascending sorted order; specify reverse=False to obtain the
-    files in the most general/distant configuration first.
+def config_open( name, mode=None, extra=None, skip=None, reverse=None, overwrite=None, **kwds ):
+    """Find and open all glob-matched file name(s) found on the standard or provided configuration
+    file paths (plus any extra), for reading in most specific to most general order (or in 'reverse'
+    for writing).  Yield the open file(s), or raise a ConfigNotFoundError (a FileNotFoundError or
+    IOError in Python3/2 if no matching file(s) at all were found, to be somewhat consistent with a
+    raw open() call).
+
+    If an absolute path is provided, only it (or those matching any glob pattern provided) are
+    traversed; otherwise, we search the config_paths + extras.
+
+    We traverse these in reverse order by default for "reading" mode: nearest and most specific, to
+    furthest and most general, and any matching file(s) in ascending sorted order; specify
+    reverse=False to obtain the files in the most general/distant configuration first.  The default
+    for 'reverse' is True for writing ('w' or 'a') modes, False for reading modes.  Since we
+    normally attempt to open any available file first, we'll generally only be writing a new file;
+    putting it by default in the most generic writable place by default makes sense.
 
     By default, we assume the matching target file(s) are UTF-8/ASCII text files, and default to
     open in 'r' mode.
 
     A 'skip' glob pattern or predicate function taking a single name and returning True/False may be
-    supplied.
+    supplied.  By default, skips files w/ a trailing "~".
 
     When reading and writing to *existing* files, skip and the glob pattern matching is supported.
     When creating *new* files, of course skip (fnmatch) and glob patterns must be avoided (because
     they only interact with already existing files).  So, avoid using any globbing characters "*?[]"
     in the filename, or it will be impossible to create a file.
 
     Writing to existing files will (by default) raise a ConfigFoundError, unless overwrite=True.
+
     """
+    mode			= mode.lower() if mode else 'r'
+    is_writing			= 'w' in mode or 'a' in mode
+    is_globbing			= glob.has_magic( name )
+    assert not is_globbing or not is_writing, \
+        "Cannot use file name \"globbing\" while writing to {}".format( name )
+    if overwrite is None:
+        overwrite		= False
+    if reverse is None:
+        reverse			= False if is_writing else True
+    if skip in (None, True):  # By default, skips any filename ending in "~"; prevents writing such a file unless skip=False
+        skip			= "*~"
     if isinstance( skip, type_str_base ):
         filtered		= lambda names: (n for n in names if not fnmatch.fnmatch( n, skip ))  # noqa: E731
     elif hasattr( skip, '__call__' ):
         filtered		= lambda names: (n for n in names if not skip( n ))  # noqa: E731
-    elif skip is None:
+    elif skip is False:
         filtered		= lambda names: names  # noqa: E731
     else:
         raise AssertionError( "Invalid skip={!r} provided".format( skip ))
-
-    search			= list( config_paths( name, extra=extra ))
-    if reverse:
-        search			= reversed( search )
-    is_globbing			= glob.has_magic( name )
+    # If an absolute or ~[user] path is provided, ignore config search paths and extras; otherwise,
+    # forward/reverse search for the name relative to the config_paths + extra.
+    name			= os.path.expanduser( name )
+    if os.path.isabs( name ):
+        search			= [ name ]
+        if extra:
+            log.warning( "Ignoring specified extra search paths: {extra}".format( extra=', '.join( extra )))
+    else:
+        search			= list( config_paths( name, extra=extra ))
+        if reverse:
+            search.reverse()
+    log.debug( "config_open {}ing paths: {}".format( 'Writ' if is_writing else 'Read', ', '.join( search )))
     for fn in search:
         log.trace( "config_open search {fn!r}{globbing}".format(
             fn=fn, globbing=" w/ globbing" if is_globbing else "" ))
         for gn in sorted( filtered( glob.iglob( fn ) if is_globbing else [ fn ] )):
-            mode		= mode or 'r'
-            if 'w' in mode and ( not overwrite ) and os.path.exists( gn ):
+            if is_writing and ( not overwrite ) and os.path.exists( gn ):
+                log.info( "config_open refuse {fn!r} in mode {mode!r}; will not overwrite existing file".format(
+                    fn=fn, mode=mode ))
                 raise ConfigFoundError( gn )
             try:
                 f		= open( gn, mode=mode or 'r', **kwds )
             except Exception as exc:
-                # The file couldn't be opened (eg. permissions)
-                log.debug( "config_open failed {fn!r} in mode {mode!r}: {exc}".format(
-                    fn=fn, mode=mode,
+                # The file couldn't be opened (eg. permissions, bad open args/kwds)
+                log.debug( "config_open failed {fn!r} in mode {mode!r} w/ {kwds}: {exc}".format(
+                    fn=fn, mode=mode, kwds=', '.join( '{}={!r}'.format( k, v ) for k,v in kwds.items() ),
                     exc=''.join( traceback.format_exception( *sys.exc_info() )) if log.isEnabledFor( logging.TRACE ) else exc ))
                 pass
             else:
                 log.info( "config_open opened {fn!r} in mode {mode!r}".format(
                     fn=f.name, mode=mode ))
                 yield f
 
 
 def deduce_name( basename=None, extension=None, filename=None, package=None ):
+    """If no basename, use filename  .../<basename>.py, or package <basename>.submodule.
+
+    An absolute path 'basename' will remain unchanged.  If no extension is present, the supplied
+    'extension' will be appended.
+
+    """
     assert basename or ( filename or package ), \
         "Cannot deduce basename without either filename (__file__) or package (__package__)"
     if basename is None:
         if filename:
-            basename		= os.path.basename( filename )      # eg. '/a/b/c/d.py' --> 'd.py'
-            if '.' in basename:
-                basename	= basename[:basename.rfind( '.' )]  # up to last '.'
+            basename		= os.path.basename( filename )		# eg. '/a/b/c/d.py' --> 'd.py'
+            basename,_		= os.path.splitext( basename )		# up to last '.' in filename (the extension)
         else:
             basename		= package
             if '.' in basename:
-                basename	= basename[:basename.find( '.' )]   # up to first '.'
+                basename	= basename[:basename.find( '.' )]       # up to first '.' in package name
     name			= basename
-    if extension and '.' not in name:
+    if extension and not os.path.splitext( name )[1]:
+        # No identifiable extension on root; this safely ignores path components containing '.'
         if extension[0] != '.':
             name	       += '.'
         name		       += extension
     return name
 
 
-def config_open_deduced( basename=None, mode=None, extension=None, filename=None, package=None, overwrite=False, **kwds ):
+def config_open_deduced( basename=None, extension=None, filename=None, package=None, **kwds ):
     """Find any glob-matched configuration file(s), optionally deducing the basename from the provided
     __file__ filename or __package__ package name, returning the open file or raising a ConfigNotFoundError
     (a FileNotFoundError, or IOError in Python2).
 
     If writing, will default to not overwrite an existing file; will raise a ConfigFoundError instead.
     """
-    for f in config_open(
-            name	= deduce_name(
-                basename=basename, extension=extension, filename=filename, package=package ),
-            mode	= mode or 'r',
-            overwrite	= overwrite,
-            **kwds
-    ):
+    name			= deduce_name(
+        basename	= basename,
+        extension	= extension,
+        filename	= filename,
+        package		= package,
+    )
+    log.info( "Opening {} w/ {}".format( name, kwds ))
+    for f in config_open( name, **kwds ):
         yield f
 
 
 def input_secure( prompt, secret=True, file=None ):
     """When getting secure (optionally secret) input from standard input, we don't want to use getpass, which
     attempts to read from /dev/tty.
```

### Comparing `crypto_licensing-3.0.4/crypto_licensing/misc_test.py` & `crypto_licensing-3.3.0/crypto_licensing/misc_test.py`

 * *Files identical despite different names*

### Comparing `crypto_licensing-3.0.4/crypto_licensing.egg-info/PKG-INFO` & `crypto_licensing-3.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: crypto-licensing
-Version: 3.0.4
+Name: crypto_licensing
+Version: 3.3.0
 Summary: The crypto-licensing module implements Ed25519-signed license checking and automatic issuance after cryptocurrency payment
 Home-page: https://github.com/pjkundert/crypto-licensing
 Author: Perry Kundert
 Author-email: perry@dominionrnd.com
 License: Dual License; GPLv3 and Proprietary
 Project-URL: Bug Tracker, https://github.com/pjkundert/crypto-licensing/issues
 Keywords: licensing Bitcoin Ethereum cryptocurrency payments Ed25519 signatures
```

