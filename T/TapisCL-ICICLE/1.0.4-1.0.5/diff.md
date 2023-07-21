# Comparing `tmp/TapisCL-ICICLE-1.0.4.tar.gz` & `tmp/TapisCL-ICICLE-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TapisCL-ICICLE-1.0.4.tar", last modified: Thu Jul 20 18:45:36 2023, max compression
+gzip compressed data, was "TapisCL-ICICLE-1.0.5.tar", last modified: Fri Jul 21 20:19:37 2023, max compression
```

## Comparing `TapisCL-ICICLE-1.0.4.tar` & `TapisCL-ICICLE-1.0.5.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 18:45:36.940786 TapisCL-ICICLE-1.0.4/
--rw-rw-rw-   0        0        0    35823 2023-04-12 23:35:22.000000 TapisCL-ICICLE-1.0.4/LICENSE
--rw-rw-rw-   0        0        0    58886 2023-07-20 18:45:36.939726 TapisCL-ICICLE-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0    16981 2023-07-18 20:02:58.000000 TapisCL-ICICLE-1.0.4/README.md
--rw-rw-rw-   0        0        0     1249 2023-07-20 18:45:05.000000 TapisCL-ICICLE-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-20 18:45:36.940786 TapisCL-ICICLE-1.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-20 18:45:36.906754 TapisCL-ICICLE-1.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-07-20 18:45:36.908877 TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/
--rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/__init__.py
--rw-rw-rw-   0        0        0      321 2023-06-29 16:14:59.000000 TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-20 18:45:36.911068 TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/client/
--rw-rw-rw-   0        0        0       84 2023-05-23 19:58:53.000000 TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/client/__init__.py
--rw-rw-rw-   0        0        0    10916 2023-07-18 21:38:48.000000 TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/client/cli.py
--rw-rw-rw-   0        0        0    16008 2023-07-17 19:00:49.000000 TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/client/handlers.py
-drwxrwxrwx   0        0        0        0 2023-07-20 18:45:36.917897 TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/commands/
-drwxrwxrwx   0        0        0        0 2023-07-20 18:45:36.920203 TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/commands/Apps/
--rw-rw-rw-   0        0        0        0 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/commands/Apps/__init__.py
--rw-rw-rw-   0        0        0    11096 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/commands/Apps/appCommands.py
--rw-rw-rw-   0        0        0      259 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/commands/Apps/appConfigGenerator.py
--rw-rw-rw-   0        0        0     4859 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/commands/Apps/appForms.py
-drwxrwxrwx   0        0        0        0 2023-07-20 18:45:36.922342 TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/commands/Systems/
--rw-rw-rw-   0        0        0        0 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/commands/Systems/__init__.py
--rw-rw-rw-   0        0        0    23546 2023-07-17 15:51:32.000000 TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/commands/Systems/systemCommands.py
--rw-rw-rw-   0        0        0     3940 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/commands/Systems/systemForms.py
--rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/commands/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-20 18:45:36.924942 TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/commands/arguments/
--rw-rw-rw-   0        0        0        0 2023-06-16 01:12:43.000000 TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/commands/arguments/__init__.py
--rw-rw-rw-   0        0        0     9383 2023-07-18 22:42:58.000000 TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/commands/arguments/argument.py
--rw-rw-rw-   0        0        0     4772 2023-07-18 16:34:22.000000 TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/commands/arguments/argumentValidators.py
--rw-rw-rw-   0        0        0    20942 2023-07-18 20:46:18.000000 TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/commands/baseCommand.py
--rw-rw-rw-   0        0        0    10976 2023-07-18 20:01:13.000000 TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/commands/commandMap.py
--rw-rw-rw-   0        0        0     2221 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/commands/commandOpts.py
--rw-rw-rw-   0        0        0     1828 2023-07-18 22:42:23.000000 TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/commands/dataFormatters.py
--rw-rw-rw-   0        0        0     4947 2023-07-10 21:26:23.000000 TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/commands/decorators.py
--rw-rw-rw-   0        0        0    12824 2023-07-18 20:04:51.000000 TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/commands/fileCommands.py
--rw-rw-rw-   0        0        0     7522 2023-07-18 20:00:48.000000 TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/commands/jobCommands.py
--rw-rw-rw-   0        0        0    13236 2023-07-18 18:01:26.000000 TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/commands/podCommands.py
-drwxrwxrwx   0        0        0        0 2023-07-20 18:45:36.927039 TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/commands/query/
--rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/commands/query/__init__.py
--rw-rw-rw-   0        0        0     1615 2023-07-11 17:42:26.000000 TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/commands/query/neo4j.py
--rw-rw-rw-   0        0        0      871 2023-06-16 01:12:43.000000 TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/commands/query/postgres.py
--rw-rw-rw-   0        0        0     4412 2023-07-17 15:54:36.000000 TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/commands/serverCommands.py
--rw-rw-rw-   0        0        0     7990 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/commands/volumeCommands.py
-drwxrwxrwx   0        0        0        0 2023-07-20 18:45:36.929112 TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/server/
--rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/server/__init__.py
--rw-rw-rw-   0        0        0    10928 2023-07-06 00:52:04.000000 TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/server/auth.py
--rw-rw-rw-   0        0        0    10402 2023-07-17 16:55:28.000000 TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/server/server.py
--rw-rw-rw-   0        0        0      290 2023-07-05 15:04:52.000000 TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/serverRun.py
-drwxrwxrwx   0        0        0        0 2023-07-20 18:45:36.930808 TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/socketopts/
--rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/socketopts/__init__.py
--rw-rw-rw-   0        0        0     2233 2023-07-10 21:26:16.000000 TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/socketopts/schemas.py
--rw-rw-rw-   0        0        0     4810 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/socketopts/socketOpts.py
-drwxrwxrwx   0        0        0        0 2023-07-20 18:45:36.934036 TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/utilities/
--rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/utilities/__init__.py
--rw-rw-rw-   0        0        0     2457 2023-06-16 02:31:56.000000 TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/utilities/exceptions.py
--rw-rw-rw-   0        0        0     1044 2023-06-29 21:33:53.000000 TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/utilities/killableThread.py
--rw-rw-rw-   0        0        0     2328 2023-07-08 04:38:18.000000 TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/utilities/logger.py
-drwxrwxrwx   0        0        0        0 2023-07-20 18:45:36.938658 TapisCL-ICICLE-1.0.4/src/TapisCL_ICICLE.egg-info/
--rw-rw-rw-   0        0        0    58886 2023-07-20 18:45:36.000000 TapisCL-ICICLE-1.0.4/src/TapisCL_ICICLE.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2003 2023-07-20 18:45:36.000000 TapisCL-ICICLE-1.0.4/src/TapisCL_ICICLE.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 18:45:36.000000 TapisCL-ICICLE-1.0.4/src/TapisCL_ICICLE.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-07-20 18:45:36.000000 TapisCL-ICICLE-1.0.4/src/TapisCL_ICICLE.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      164 2023-07-20 18:45:36.000000 TapisCL-ICICLE-1.0.4/src/TapisCL_ICICLE.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-07-20 18:45:36.000000 TapisCL-ICICLE-1.0.4/src/TapisCL_ICICLE.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-06-29 16:14:59.000000 TapisCL-ICICLE-1.0.4/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-20 18:45:36.938658 TapisCL-ICICLE-1.0.4/tests/
--rw-rw-rw-   0        0        0       48 2023-07-18 20:13:22.000000 TapisCL-ICICLE-1.0.4/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-07-21 20:19:37.214107 TapisCL-ICICLE-1.0.5/
+-rw-rw-rw-   0        0        0    35823 2023-04-12 23:35:22.000000 TapisCL-ICICLE-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0    58862 2023-07-21 20:19:37.213106 TapisCL-ICICLE-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0    16957 2023-07-21 17:35:54.000000 TapisCL-ICICLE-1.0.5/README.md
+-rw-rw-rw-   0        0        0     1249 2023-07-21 20:15:37.000000 TapisCL-ICICLE-1.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-21 20:19:37.214107 TapisCL-ICICLE-1.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-21 20:19:37.172550 TapisCL-ICICLE-1.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-07-21 20:19:37.176057 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/
+-rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/__init__.py
+-rw-rw-rw-   0        0        0      321 2023-06-29 16:14:59.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 20:19:37.179057 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/client/
+-rw-rw-rw-   0        0        0       84 2023-05-23 19:58:53.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/client/__init__.py
+-rw-rw-rw-   0        0        0    10916 2023-07-18 21:38:48.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/client/cli.py
+-rw-rw-rw-   0        0        0    16126 2023-07-21 19:28:18.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/client/handlers.py
+drwxrwxrwx   0        0        0        0 2023-07-21 20:19:37.187565 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/
+drwxrwxrwx   0        0        0        0 2023-07-21 20:19:37.190564 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/Apps/
+-rw-rw-rw-   0        0        0        0 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/Apps/__init__.py
+-rw-rw-rw-   0        0        0    11086 2023-07-21 19:35:57.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/Apps/appCommands.py
+-rw-rw-rw-   0        0        0      259 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/Apps/appConfigGenerator.py
+-rw-rw-rw-   0        0        0     4859 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/Apps/appForms.py
+drwxrwxrwx   0        0        0        0 2023-07-21 20:19:37.192567 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/Systems/
+-rw-rw-rw-   0        0        0        0 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/Systems/__init__.py
+-rw-rw-rw-   0        0        0    23546 2023-07-17 15:51:32.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/Systems/systemCommands.py
+-rw-rw-rw-   0        0        0     3938 2023-07-21 19:22:41.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/Systems/systemForms.py
+-rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 20:19:37.195072 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/arguments/
+-rw-rw-rw-   0        0        0        0 2023-06-16 01:12:43.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/arguments/__init__.py
+-rw-rw-rw-   0        0        0     9613 2023-07-21 19:10:55.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/arguments/argument.py
+-rw-rw-rw-   0        0        0     4814 2023-07-21 18:30:09.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/arguments/argumentValidators.py
+-rw-rw-rw-   0        0        0    21343 2023-07-21 19:33:37.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/baseCommand.py
+-rw-rw-rw-   0        0        0    10976 2023-07-18 20:01:13.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/commandMap.py
+-rw-rw-rw-   0        0        0     2221 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/commandOpts.py
+-rw-rw-rw-   0        0        0     1828 2023-07-18 22:42:23.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/dataFormatters.py
+-rw-rw-rw-   0        0        0     4947 2023-07-10 21:26:23.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/decorators.py
+-rw-rw-rw-   0        0        0    12824 2023-07-18 20:04:51.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/fileCommands.py
+-rw-rw-rw-   0        0        0     7522 2023-07-18 20:00:48.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/jobCommands.py
+-rw-rw-rw-   0        0        0    13236 2023-07-18 18:01:26.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/podCommands.py
+drwxrwxrwx   0        0        0        0 2023-07-21 20:19:37.197079 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/query/
+-rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/query/__init__.py
+-rw-rw-rw-   0        0        0     1727 2023-07-21 20:08:39.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/query/neo4j.py
+-rw-rw-rw-   0        0        0      941 2023-07-21 20:10:12.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/query/postgres.py
+-rw-rw-rw-   0        0        0     4412 2023-07-17 15:54:36.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/serverCommands.py
+-rw-rw-rw-   0        0        0     7990 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/volumeCommands.py
+drwxrwxrwx   0        0        0        0 2023-07-21 20:19:37.199085 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/server/
+-rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/server/__init__.py
+-rw-rw-rw-   0        0        0    10928 2023-07-06 00:52:04.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/server/auth.py
+-rw-rw-rw-   0        0        0    10402 2023-07-17 16:55:28.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/server/server.py
+-rw-rw-rw-   0        0        0      290 2023-07-05 15:04:52.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/serverRun.py
+drwxrwxrwx   0        0        0        0 2023-07-21 20:19:37.201085 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/socketopts/
+-rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/socketopts/__init__.py
+-rw-rw-rw-   0        0        0     2233 2023-07-10 21:26:16.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/socketopts/schemas.py
+-rw-rw-rw-   0        0        0     4810 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/socketopts/socketOpts.py
+drwxrwxrwx   0        0        0        0 2023-07-21 20:19:37.203593 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/utilities/
+-rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/utilities/__init__.py
+-rw-rw-rw-   0        0        0     2457 2023-06-16 02:31:56.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/utilities/exceptions.py
+-rw-rw-rw-   0        0        0     1044 2023-06-29 21:33:53.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/utilities/killableThread.py
+-rw-rw-rw-   0        0        0     2328 2023-07-08 04:38:18.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/utilities/logger.py
+drwxrwxrwx   0        0        0        0 2023-07-21 20:19:37.210108 TapisCL-ICICLE-1.0.5/src/TapisCL_ICICLE.egg-info/
+-rw-rw-rw-   0        0        0    58862 2023-07-21 20:19:37.000000 TapisCL-ICICLE-1.0.5/src/TapisCL_ICICLE.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2003 2023-07-21 20:19:37.000000 TapisCL-ICICLE-1.0.5/src/TapisCL_ICICLE.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 20:19:37.000000 TapisCL-ICICLE-1.0.5/src/TapisCL_ICICLE.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-07-21 20:19:37.000000 TapisCL-ICICLE-1.0.5/src/TapisCL_ICICLE.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      164 2023-07-21 20:19:37.000000 TapisCL-ICICLE-1.0.5/src/TapisCL_ICICLE.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-07-21 20:19:37.000000 TapisCL-ICICLE-1.0.5/src/TapisCL_ICICLE.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-06-29 16:14:59.000000 TapisCL-ICICLE-1.0.5/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 20:19:37.211107 TapisCL-ICICLE-1.0.5/tests/
+-rw-rw-rw-   0        0        0       48 2023-07-18 20:13:22.000000 TapisCL-ICICLE-1.0.5/tests/test.py
```

### Comparing `TapisCL-ICICLE-1.0.4/LICENSE` & `TapisCL-ICICLE-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.4/PKG-INFO` & `TapisCL-ICICLE-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TapisCL-ICICLE
-Version: 1.0.4
+Version: 1.0.5
 Summary: Provide good performance command line user interface for Tapis services hosted on HPC clusters
 Author-email: Michael Ray <m.ray37990@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -695,15 +695,15 @@
 Allows you to work with all major Tapis services: Pods, Systems, Files, and Apps in one place. It can also interface directly with services being hosted on Tapis pods, like Neo4j. Although currently Neo4j is the only 3rd party application it can work with, adding support for Postgres and the like will not be difficult.
 
 ### Dependencies
 * Dependencies are listed [here](https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/blob/main/icicle_rel_03_2023/CLI/TapisCL-ICICLE/requirements.txt)
 
 ### Installation
 #### Using PyPi
-1. `pip install TapisCL-ICICLE`. Current version 0.0.24
+1. `pip install TapisCL-ICICLE`
 2. run using `python -m TapisCLICICLE`
 #### Running Python Code Directly
 1. Clone the repository to local machine.
 2. `python -m pip install -r requirements.txt`
 3. from the src folder, run using `python -m TapisCLICICLE`
 
 ### Known Issues
```

### Comparing `TapisCL-ICICLE-1.0.4/README.md` & `TapisCL-ICICLE-1.0.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 Allows you to work with all major Tapis services: Pods, Systems, Files, and Apps in one place. It can also interface directly with services being hosted on Tapis pods, like Neo4j. Although currently Neo4j is the only 3rd party application it can work with, adding support for Postgres and the like will not be difficult.
 
 ### Dependencies
 * Dependencies are listed [here](https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/blob/main/icicle_rel_03_2023/CLI/TapisCL-ICICLE/requirements.txt)
 
 ### Installation
 #### Using PyPi
-1. `pip install TapisCL-ICICLE`. Current version 0.0.24
+1. `pip install TapisCL-ICICLE`
 2. run using `python -m TapisCLICICLE`
 #### Running Python Code Directly
 1. Clone the repository to local machine.
 2. `python -m pip install -r requirements.txt`
 3. from the src folder, run using `python -m TapisCLICICLE`
 
 ### Known Issues
```

### Comparing `TapisCL-ICICLE-1.0.4/pyproject.toml` & `TapisCL-ICICLE-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel", "poetry-core>=1.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "TapisCL-ICICLE"
-version = "1.0.4"
+version = "1.0.5"
 description = "Provide good performance command line user interface for Tapis services hosted on HPC clusters"
 readme = "README.md"
 authors = [{ name = "Michael Ray", email = "m.ray37990@gmail.com" }]
 license = { file = "LICENSE" }
 requires-python = ">=3.6"
 classifiers = [
     "License :: OSI Approved :: GNU General Public License (GPL)",
```

### Comparing `TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/client/cli.py` & `TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/client/cli.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/client/handlers.py` & `TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/client/handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -281,15 +281,17 @@
     def advanced_input_handler(self, form_request: dict, term: Terminal, default=None):
         response = dict()
         for field, attrs in form_request.items():
             arg_type = attrs['arg_type']
             self.validator.enforcer.update_constraints(**attrs)
             if 'description' in attrs and attrs['description']:
                 print(attrs['description'])
-            if default:
+            if default and attrs['part_of']:
+                default_selection = default[attrs['part_of']][field]
+            elif default:
                 default_selection = default[field]
             else:
                 default_selection = None
             try:
                 match arg_type:
                     case 'secure':
                         answer = prompt(f"{attrs['name']}: ", validator=self.validator, is_password=True)
```

### Comparing `TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/commands/Apps/appCommands.py` & `TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/Apps/appCommands.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,15 +141,15 @@
         return 'updated job attributes successfully'
     
 
 class get_apps(baseCommand.BaseCommand):
     """
     @help: get a list of all available apps
     """
-    return_fields = ['id', 'version', 'status']
+    return_fields = ['id', 'version']
     optional_arguments = [
         Argument('listType', choices=[
             'OWNED',
             'SHARED_PUBLIC',
             'SHARED_DIRECT',
             'READ_PERM', 
             'MINE',
```

### Comparing `TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/commands/Apps/appForms.py` & `TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/Apps/appForms.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/commands/Systems/systemCommands.py` & `TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/Systems/systemCommands.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/commands/Systems/systemForms.py` & `TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/Systems/systemForms.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,14 @@
             Argument('value', default_value=''),
         ],
         optional_arguments = [
             Argument('description', size_limit=(0, 2048), arg_type='str_input')
         ]
     ))
 
-
 JOB_CAPABILITIES = Argument('jobCapabilities', arg_type='input_list', data_type=argument.Form(
             'jobCapability', required_arguments=[
                 Argument('name', size_limit=(1, 128)),
                 Argument('value'),
                 Argument('category', choices=['SCHEUDLER', 
                                             'OS', 'HARDWARE', 
                                             'SOFTWARE', 'JOB',
```

### Comparing `TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/commands/arguments/argument.py` & `TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/arguments/argument.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,17 +69,24 @@
 
     def verify_rules_followed(self, value):
         """
         check to make sure the value assigned to the argument follows all existing rules
         """
         if self.required and not value and value != False and self.arg_type != 'silent':
             raise ValueError(f'The argument {self.argument} is required')
-        return_value = self.validator_map[self.arg_type](value)
-        if isinstance(return_value, bool) and self.data_type != 'bool' and self.action != 'store_true' and not return_value:
-            print(f"{self.argument} RETURNING NONE")
+        return_value = value
+        print(f"RETURN VALUE: {return_value}")
+        if self.arg_type in ('standard', 'silent'):
+            return_value = self.validator_map[self.arg_type](value)
+        elif not isinstance(value, bool) and value:
+            try:
+                return_value = self.validator_map[self.arg_type](value[self.argument])
+            except:
+                return_value = self.validator_map[self.arg_type](value)
+        elif isinstance(return_value, bool) and self.data_type != 'bool' and self.action != 'store_true' and not return_value or return_value == None:
             return None
         return return_value
 
     def json(self):
         json = {
             'name':self.argument,
             'arg_type':self.arg_type,
@@ -155,24 +162,21 @@
         self.arguments_list = {argument.argument:argument for argument in arguments_list}
         self.flattening_type = flattening_type
     
     def flatten_form_data(self, value): 
         if value and not isinstance(value, bool):
             if self.flattening_type == 'FLATTEN':
                 flattened_form_info = {self.argument:True}
-                flattened_form_info.update(**{arg_name:arg_value for arg_name, arg_value in value[self.argument].items()})
+                flattened_form_info.update(**{arg_name:arg_value for arg_name, arg_value in value.items()})
                 return flattened_form_info
             if self.flattening_type == 'RETRIEVE':
-                exctracted_form_data = {arg_name:arg for arg_name, arg in value[self.argument].items()}
+                exctracted_form_data = {arg_name:arg for arg_name, arg in value.items()}
                 return exctracted_form_data
             else:
-                try:
-                    return value[self.argument]
-                except:
-                    return value
+                return value
 
     def json(self):
         fields = {argument_name:argument.json() for argument_name, argument in self.arguments_list.items()}
         json = {
             'name':self.argument,
             'arg_type':self.arg_type,
             'data_type':self.data_type,
```

### Comparing `TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/commands/arguments/argumentValidators.py` & `TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/arguments/argumentValidators.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,14 +93,15 @@
         if isinstance(value, bool) and value:
             return True
         else:
             return None
     
     def dict_validator(self, value):
         if value and not isinstance(value, bool):
+            print(f"DICT VALUE {value}")
             processed_values = dict()
             for sub_name, sub_value in value.items():
                 processed_values[sub_name] = self.data_type.verify_rules_followed(sub_value)
             return processed_values
         if isinstance(value, bool) and value:
             return True
         else:
```

### Comparing `TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/commands/baseCommand.py` & `TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/baseCommand.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,24 +202,27 @@
                 request = schemas.FormRequest(request_content={arg_name:argument}, existing_data=existing_values)
                 await kwargs['connection'].send(request)
                 response: schemas.FormResponse = await kwargs['connection'].receive()
                 response_value = response.request_content
                 if response_value == None:
                     raise ValueError(f"No value was received for the argument {arg_name}")
                 response_value = argument.verify_rules_followed(response_value)
-                if argument.arg_type == 'form' and argument.flattening_type in ('FLATTEN', 'RETRIEVE'):
+                if argument.arg_type == 'form' and argument.flattening_type in ('FLATTEN', 'RETRIEVE') and not argument.part_of:
                     kwargs.pop(arg_name)
+                    kwargs.update(**response_value)
+                    continue
                 if argument.part_of:
+                    kwargs.pop(arg_name)
                     if argument.part_of not in kwargs:
                         kwargs[argument.part_of] = dict()
                     kwargs[argument.part_of][argument.argument] = response_value
-                elif argument.arg_type != 'form':
-                    kwargs.update(**{arg_name:response_value})
-                else:
-                    kwargs.update(**response_value)
+                else: 
+                    pprint(response_value)
+                    kwargs[arg_name] = response_value
+                pprint(kwargs)
         return kwargs
 
     async def handle_arg_opts(self, kwargs):
         """
         arg opts handle special operations, like supporting relative file paths, and system entry
         """
         for opt in self.command_opt:
@@ -284,16 +287,20 @@
                 "Optional Arguments":self.help['optional']['verbose']})
         return help_dict
     
     def brief_help(self):
         """
         return non verbose help
         """
-        return {"Command":self.__class__.__name__,
-                "Description":self.help_string_retriever()}
+        help = {"Command":self.__class__.__name__,
+                "Description":self.help_string_retriever(),
+                "help command":f"Enter {self.__class__.__name__} -h for parameters, or {self.__class__.__name__} -h -v for detailed command parameters"}
+        if self.return_fields:
+            help['verbose'] = "add the '-v' flag to view full command results"
+        return help
     
     @abstractmethod
     async def run(self, *args, **kwargs):
         """
         contains the actual command information at command definition
         """
         pass
```

### Comparing `TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/commands/commandMap.py` & `TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/commandMap.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/commands/commandOpts.py` & `TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/commandOpts.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/commands/dataFormatters.py` & `TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/dataFormatters.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/commands/decorators.py` & `TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/decorators.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/commands/fileCommands.py` & `TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/fileCommands.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/commands/jobCommands.py` & `TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/jobCommands.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/commands/podCommands.py` & `TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/podCommands.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/commands/query/neo4j.py` & `TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/query/neo4j.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 from py2neo import Graph
+import py2neo
+import pandas as pd
 
 
 if __name__ != "__main__":
     from .. import baseCommand, decorators
     from ..arguments import argument
-
+    
 
 class neo4j(baseCommand.BaseQuery):
     """
     @help: integrated CLI to interface with Neo4j pods
     """
     required_arguments = [
-        argument.Argument('id'),
+        argument.Argument('id', positional=True),
         argument.Argument('expression', arg_type='expression')
     ]
     async def run(self, *args, **kwargs) -> str: # function to submit queries to a Neo4j knowledge graph
         uname, pword = self.get_pod_credentials(kwargs["id"])
         graph = Graph(f"bolt+ssc://{kwargs['id']}.pods.{self.t.base_url.split('https://')[1]}:443", auth=(uname, pword), secure=True, verify=True)
 
-        return_value = graph.run(kwargs['expression'])
+        return_value = graph.run(kwargs['expression']).to_data_frame().to_dict()
         print(type(return_value))
+        print(return_value)
         if str(return_value) == '(No data)' and 'create' in kwargs['expression'].lower(): # if no data is returned (mostly if something is created) then just say 'success'
             return f'[+][{kwargs["id"]}@pods.{self.t.base_url.split("https://")[1]}:443] Success'
         elif str(return_value) == '(No data)':
             return f'[-][{kwargs["id"]}@pods.{self.t.base_url.split("https://")[1]}:443] KG is empty'
 
         return return_value
```

### Comparing `TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/commands/serverCommands.py` & `TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/serverCommands.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/commands/volumeCommands.py` & `TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/volumeCommands.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/server/auth.py` & `TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/server/auth.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/server/server.py` & `TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/server/server.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/socketopts/schemas.py` & `TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/socketopts/schemas.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/socketopts/socketOpts.py` & `TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/socketopts/socketOpts.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/utilities/exceptions.py` & `TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/utilities/killableThread.py` & `TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/utilities/killableThread.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.4/src/TapisCLICICLE/utilities/logger.py` & `TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/utilities/logger.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.4/src/TapisCL_ICICLE.egg-info/PKG-INFO` & `TapisCL-ICICLE-1.0.5/src/TapisCL_ICICLE.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TapisCL-ICICLE
-Version: 1.0.4
+Version: 1.0.5
 Summary: Provide good performance command line user interface for Tapis services hosted on HPC clusters
 Author-email: Michael Ray <m.ray37990@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -695,15 +695,15 @@
 Allows you to work with all major Tapis services: Pods, Systems, Files, and Apps in one place. It can also interface directly with services being hosted on Tapis pods, like Neo4j. Although currently Neo4j is the only 3rd party application it can work with, adding support for Postgres and the like will not be difficult.
 
 ### Dependencies
 * Dependencies are listed [here](https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/blob/main/icicle_rel_03_2023/CLI/TapisCL-ICICLE/requirements.txt)
 
 ### Installation
 #### Using PyPi
-1. `pip install TapisCL-ICICLE`. Current version 0.0.24
+1. `pip install TapisCL-ICICLE`
 2. run using `python -m TapisCLICICLE`
 #### Running Python Code Directly
 1. Clone the repository to local machine.
 2. `python -m pip install -r requirements.txt`
 3. from the src folder, run using `python -m TapisCLICICLE`
 
 ### Known Issues
```

### Comparing `TapisCL-ICICLE-1.0.4/src/TapisCL_ICICLE.egg-info/SOURCES.txt` & `TapisCL-ICICLE-1.0.5/src/TapisCL_ICICLE.egg-info/SOURCES.txt`

 * *Files identical despite different names*

