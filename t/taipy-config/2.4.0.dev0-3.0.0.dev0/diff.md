# Comparing `tmp/taipy-config-2.4.0.dev0.tar.gz` & `tmp/taipy-config-3.0.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taipy-config-2.4.0.dev0.tar", last modified: Fri Jul 21 10:27:19 2023, max compression
+gzip compressed data, was "taipy-config-3.0.0.dev0.tar", last modified: Fri Jun 23 08:48:48 2023, max compression
```

## Comparing `taipy-config-2.4.0.dev0.tar` & `taipy-config-3.0.0.dev0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:27:19.361830 taipy-config-2.4.0.dev0/
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-07-21 10:27:03.000000 taipy-config-2.4.0.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-21 10:27:03.000000 taipy-config-2.4.0.dev0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-07-21 10:27:19.361830 taipy-config-2.4.0.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-07-21 10:27:03.000000 taipy-config-2.4.0.dev0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 10:27:19.361830 taipy-config-2.4.0.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-07-21 10:27:03.000000 taipy-config-2.4.0.dev0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:27:19.349830 taipy-config-2.4.0.dev0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:27:19.353830 taipy-config-2.4.0.dev0/src/taipy/
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-21 10:27:03.000000 taipy-config-2.4.0.dev0/src/taipy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:27:19.353830 taipy-config-2.4.0.dev0/src/taipy/_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-21 10:27:03.000000 taipy-config-2.4.0.dev0/src/taipy/_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:27:19.353830 taipy-config-2.4.0.dev0/src/taipy/_cli/_base_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-21 10:27:03.000000 taipy-config-2.4.0.dev0/src/taipy/_cli/_base_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-07-21 10:27:03.000000 taipy-config-2.4.0.dev0/src/taipy/_cli/_base_cli/_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:27:19.353830 taipy-config-2.4.0.dev0/src/taipy/config/
--rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-07-21 10:27:03.000000 taipy-config-2.4.0.dev0/src/taipy/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-07-21 10:27:03.000000 taipy-config-2.4.0.dev0/src/taipy/config/_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:27:19.357830 taipy-config-2.4.0.dev0/src/taipy/config/_config_comparator/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-21 10:27:03.000000 taipy-config-2.4.0.dev0/src/taipy/config/_config_comparator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-07-21 10:27:03.000000 taipy-config-2.4.0.dev0/src/taipy/config/_config_comparator/_comparator_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     7617 2023-07-21 10:27:03.000000 taipy-config-2.4.0.dev0/src/taipy/config/_config_comparator/_config_comparator.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-21 10:27:03.000000 taipy-config-2.4.0.dev0/src/taipy/config/_init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:27:19.357830 taipy-config-2.4.0.dev0/src/taipy/config/_serializer/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-21 10:27:03.000000 taipy-config-2.4.0.dev0/src/taipy/config/_serializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-07-21 10:27:03.000000 taipy-config-2.4.0.dev0/src/taipy/config/_serializer/_base_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-07-21 10:27:03.000000 taipy-config-2.4.0.dev0/src/taipy/config/_serializer/_json_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-21 10:27:03.000000 taipy-config-2.4.0.dev0/src/taipy/config/_serializer/_toml_serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:27:19.357830 taipy-config-2.4.0.dev0/src/taipy/config/checker/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-21 10:27:03.000000 taipy-config-2.4.0.dev0/src/taipy/config/checker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-21 10:27:03.000000 taipy-config-2.4.0.dev0/src/taipy/config/checker/_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:27:19.357830 taipy-config-2.4.0.dev0/src/taipy/config/checker/_checkers/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-21 10:27:03.000000 taipy-config-2.4.0.dev0/src/taipy/config/checker/_checkers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-07-21 10:27:03.000000 taipy-config-2.4.0.dev0/src/taipy/config/checker/_checkers/_auth_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-07-21 10:27:03.000000 taipy-config-2.4.0.dev0/src/taipy/config/checker/_checkers/_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-07-21 10:27:03.000000 taipy-config-2.4.0.dev0/src/taipy/config/checker/_checkers/_global_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-21 10:27:03.000000 taipy-config-2.4.0.dev0/src/taipy/config/checker/issue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-21 10:27:03.000000 taipy-config-2.4.0.dev0/src/taipy/config/checker/issue_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:27:19.361830 taipy-config-2.4.0.dev0/src/taipy/config/common/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-21 10:27:03.000000 taipy-config-2.4.0.dev0/src/taipy/config/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-21 10:27:03.000000 taipy-config-2.4.0.dev0/src/taipy/config/common/_classproperty.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-07-21 10:27:03.000000 taipy-config-2.4.0.dev0/src/taipy/config/common/_config_blocker.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-21 10:27:03.000000 taipy-config-2.4.0.dev0/src/taipy/config/common/_repr_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-07-21 10:27:03.000000 taipy-config-2.4.0.dev0/src/taipy/config/common/_template_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-21 10:27:03.000000 taipy-config-2.4.0.dev0/src/taipy/config/common/_validate_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-21 10:27:03.000000 taipy-config-2.4.0.dev0/src/taipy/config/common/frequency.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-21 10:27:03.000000 taipy-config-2.4.0.dev0/src/taipy/config/common/scope.py
--rw-r--r--   0 runner    (1001) docker     (123)    10597 2023-07-21 10:27:03.000000 taipy-config-2.4.0.dev0/src/taipy/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    42027 2023-07-21 10:27:03.000000 taipy-config-2.4.0.dev0/src/taipy/config/config.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:27:19.361830 taipy-config-2.4.0.dev0/src/taipy/config/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-21 10:27:03.000000 taipy-config-2.4.0.dev0/src/taipy/config/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-21 10:27:03.000000 taipy-config-2.4.0.dev0/src/taipy/config/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:27:19.361830 taipy-config-2.4.0.dev0/src/taipy/config/global_app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 10:27:03.000000 taipy-config-2.4.0.dev0/src/taipy/config/global_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7368 2023-07-21 10:27:03.000000 taipy-config-2.4.0.dev0/src/taipy/config/global_app/global_app_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-21 10:27:03.000000 taipy-config-2.4.0.dev0/src/taipy/config/section.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-21 10:27:03.000000 taipy-config-2.4.0.dev0/src/taipy/config/unique_section.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-21 10:27:03.000000 taipy-config-2.4.0.dev0/src/taipy/config/version.json
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-21 10:27:03.000000 taipy-config-2.4.0.dev0/src/taipy/config/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:27:19.361830 taipy-config-2.4.0.dev0/src/taipy/logger/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-21 10:27:03.000000 taipy-config-2.4.0.dev0/src/taipy/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-07-21 10:27:03.000000 taipy-config-2.4.0.dev0/src/taipy/logger/_taipy_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:27:19.361830 taipy-config-2.4.0.dev0/src/taipy_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-07-21 10:27:19.000000 taipy-config-2.4.0.dev0/src/taipy_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-07-21 10:27:19.000000 taipy-config-2.4.0.dev0/src/taipy_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 10:27:19.000000 taipy-config-2.4.0.dev0/src/taipy_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 10:27:12.000000 taipy-config-2.4.0.dev0/src/taipy_config.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-21 10:27:19.000000 taipy-config-2.4.0.dev0/src/taipy_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-21 10:27:19.000000 taipy-config-2.4.0.dev0/src/taipy_config.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:48:48.865157 taipy-config-3.0.0.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-06-23 08:48:34.000000 taipy-config-3.0.0.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-23 08:48:34.000000 taipy-config-3.0.0.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-06-23 08:48:48.865157 taipy-config-3.0.0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-23 08:48:34.000000 taipy-config-3.0.0.dev0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 08:48:48.865157 taipy-config-3.0.0.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-06-23 08:48:34.000000 taipy-config-3.0.0.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:48:48.849157 taipy-config-3.0.0.dev0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:48:48.849157 taipy-config-3.0.0.dev0/src/taipy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-23 08:48:34.000000 taipy-config-3.0.0.dev0/src/taipy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:48:48.849157 taipy-config-3.0.0.dev0/src/taipy/_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-23 08:48:34.000000 taipy-config-3.0.0.dev0/src/taipy/_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:48:48.849157 taipy-config-3.0.0.dev0/src/taipy/_cli/_base_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-23 08:48:34.000000 taipy-config-3.0.0.dev0/src/taipy/_cli/_base_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-06-23 08:48:34.000000 taipy-config-3.0.0.dev0/src/taipy/_cli/_base_cli/_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:48:48.853157 taipy-config-3.0.0.dev0/src/taipy/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-06-23 08:48:34.000000 taipy-config-3.0.0.dev0/src/taipy/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-06-23 08:48:34.000000 taipy-config-3.0.0.dev0/src/taipy/config/_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:48:48.853157 taipy-config-3.0.0.dev0/src/taipy/config/_config_comparator/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-23 08:48:34.000000 taipy-config-3.0.0.dev0/src/taipy/config/_config_comparator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-06-23 08:48:34.000000 taipy-config-3.0.0.dev0/src/taipy/config/_config_comparator/_comparator_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7617 2023-06-23 08:48:34.000000 taipy-config-3.0.0.dev0/src/taipy/config/_config_comparator/_config_comparator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-23 08:48:34.000000 taipy-config-3.0.0.dev0/src/taipy/config/_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:48:48.857157 taipy-config-3.0.0.dev0/src/taipy/config/_serializer/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-23 08:48:34.000000 taipy-config-3.0.0.dev0/src/taipy/config/_serializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-06-23 08:48:34.000000 taipy-config-3.0.0.dev0/src/taipy/config/_serializer/_base_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-23 08:48:34.000000 taipy-config-3.0.0.dev0/src/taipy/config/_serializer/_json_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-06-23 08:48:34.000000 taipy-config-3.0.0.dev0/src/taipy/config/_serializer/_toml_serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:48:48.857157 taipy-config-3.0.0.dev0/src/taipy/config/checker/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-23 08:48:34.000000 taipy-config-3.0.0.dev0/src/taipy/config/checker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-06-23 08:48:34.000000 taipy-config-3.0.0.dev0/src/taipy/config/checker/_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:48:48.857157 taipy-config-3.0.0.dev0/src/taipy/config/checker/_checkers/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-23 08:48:34.000000 taipy-config-3.0.0.dev0/src/taipy/config/checker/_checkers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-06-23 08:48:34.000000 taipy-config-3.0.0.dev0/src/taipy/config/checker/_checkers/_auth_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-06-23 08:48:34.000000 taipy-config-3.0.0.dev0/src/taipy/config/checker/_checkers/_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-06-23 08:48:34.000000 taipy-config-3.0.0.dev0/src/taipy/config/checker/_checkers/_global_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-23 08:48:34.000000 taipy-config-3.0.0.dev0/src/taipy/config/checker/issue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-23 08:48:34.000000 taipy-config-3.0.0.dev0/src/taipy/config/checker/issue_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:48:48.861157 taipy-config-3.0.0.dev0/src/taipy/config/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-23 08:48:34.000000 taipy-config-3.0.0.dev0/src/taipy/config/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-23 08:48:34.000000 taipy-config-3.0.0.dev0/src/taipy/config/common/_classproperty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-23 08:48:34.000000 taipy-config-3.0.0.dev0/src/taipy/config/common/_config_blocker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-23 08:48:34.000000 taipy-config-3.0.0.dev0/src/taipy/config/common/_repr_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-06-23 08:48:34.000000 taipy-config-3.0.0.dev0/src/taipy/config/common/_template_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-23 08:48:34.000000 taipy-config-3.0.0.dev0/src/taipy/config/common/_validate_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-06-23 08:48:34.000000 taipy-config-3.0.0.dev0/src/taipy/config/common/frequency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-23 08:48:34.000000 taipy-config-3.0.0.dev0/src/taipy/config/common/scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10597 2023-06-23 08:48:34.000000 taipy-config-3.0.0.dev0/src/taipy/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42213 2023-06-23 08:48:34.000000 taipy-config-3.0.0.dev0/src/taipy/config/config.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:48:48.861157 taipy-config-3.0.0.dev0/src/taipy/config/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-23 08:48:34.000000 taipy-config-3.0.0.dev0/src/taipy/config/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-23 08:48:34.000000 taipy-config-3.0.0.dev0/src/taipy/config/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:48:48.861157 taipy-config-3.0.0.dev0/src/taipy/config/global_app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 08:48:34.000000 taipy-config-3.0.0.dev0/src/taipy/config/global_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7368 2023-06-23 08:48:34.000000 taipy-config-3.0.0.dev0/src/taipy/config/global_app/global_app_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-23 08:48:34.000000 taipy-config-3.0.0.dev0/src/taipy/config/section.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-23 08:48:34.000000 taipy-config-3.0.0.dev0/src/taipy/config/unique_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-23 08:48:34.000000 taipy-config-3.0.0.dev0/src/taipy/config/version.json
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-23 08:48:34.000000 taipy-config-3.0.0.dev0/src/taipy/config/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:48:48.861157 taipy-config-3.0.0.dev0/src/taipy/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-23 08:48:34.000000 taipy-config-3.0.0.dev0/src/taipy/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-23 08:48:34.000000 taipy-config-3.0.0.dev0/src/taipy/logger/_taipy_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:48:48.865157 taipy-config-3.0.0.dev0/src/taipy_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-06-23 08:48:48.000000 taipy-config-3.0.0.dev0/src/taipy_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-06-23 08:48:48.000000 taipy-config-3.0.0.dev0/src/taipy_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 08:48:48.000000 taipy-config-3.0.0.dev0/src/taipy_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 08:48:42.000000 taipy-config-3.0.0.dev0/src/taipy_config.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-23 08:48:48.000000 taipy-config-3.0.0.dev0/src/taipy_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-23 08:48:48.000000 taipy-config-3.0.0.dev0/src/taipy_config.egg-info/top_level.txt
```

### Comparing `taipy-config-2.4.0.dev0/LICENSE` & `taipy-config-3.0.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `taipy-config-2.4.0.dev0/PKG-INFO` & `taipy-config-3.0.0.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: taipy-config
-Version: 2.4.0.dev0
+Version: 3.0.0.dev0
 Summary: A Taipy package dedicated to easily configure a Taipy application.
 Home-page: https://github.com/avaiga/taipy-config
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy-config
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Taipy config
 
 ## License
```

### Comparing `taipy-config-2.4.0.dev0/README.md` & `taipy-config-3.0.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `taipy-config-2.4.0.dev0/setup.py` & `taipy-config-3.0.0.dev0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,15 +38,14 @@
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
     ],
     description="A Taipy package dedicated to easily configure a Taipy application.",
     install_requires=requirements,
     long_description=readme,
     long_description_content_type="text/markdown",
     include_package_data=True,
     license="Apache License 2.0",
```

### Comparing `taipy-config-2.4.0.dev0/src/taipy/__init__.py` & `taipy-config-3.0.0.dev0/src/taipy/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.4.0.dev0/src/taipy/_cli/__init__.py` & `taipy-config-3.0.0.dev0/src/taipy/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.4.0.dev0/src/taipy/_cli/_base_cli/__init__.py` & `taipy-config-3.0.0.dev0/src/taipy/_cli/_base_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.4.0.dev0/src/taipy/_cli/_base_cli/_cli.py` & `taipy-config-3.0.0.dev0/src/taipy/_cli/_base_cli/_cli.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.4.0.dev0/src/taipy/config/__init__.py` & `taipy-config-3.0.0.dev0/src/taipy/config/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.4.0.dev0/src/taipy/config/_config.py` & `taipy-config-3.0.0.dev0/src/taipy/config/_config.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.4.0.dev0/src/taipy/config/_config_comparator/__init__.py` & `taipy-config-3.0.0.dev0/src/taipy/config/_config_comparator/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.4.0.dev0/src/taipy/config/_config_comparator/_comparator_result.py` & `taipy-config-3.0.0.dev0/src/taipy/config/_config_comparator/_comparator_result.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.4.0.dev0/src/taipy/config/_config_comparator/_config_comparator.py` & `taipy-config-3.0.0.dev0/src/taipy/config/_config_comparator/_config_comparator.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.4.0.dev0/src/taipy/config/_init.py` & `taipy-config-3.0.0.dev0/src/taipy/config/_init.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.4.0.dev0/src/taipy/config/_serializer/__init__.py` & `taipy-config-3.0.0.dev0/src/taipy/config/_serializer/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.4.0.dev0/src/taipy/config/_serializer/_base_serializer.py` & `taipy-config-3.0.0.dev0/src/taipy/config/_serializer/_base_serializer.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.4.0.dev0/src/taipy/config/_serializer/_json_serializer.py` & `taipy-config-3.0.0.dev0/src/taipy/config/_serializer/_json_serializer.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.4.0.dev0/src/taipy/config/_serializer/_toml_serializer.py` & `taipy-config-3.0.0.dev0/src/taipy/config/_serializer/_toml_serializer.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.4.0.dev0/src/taipy/config/checker/__init__.py` & `taipy-config-3.0.0.dev0/src/taipy/config/checker/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.4.0.dev0/src/taipy/config/checker/_checker.py` & `taipy-config-3.0.0.dev0/src/taipy/config/checker/_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.4.0.dev0/src/taipy/config/checker/_checkers/__init__.py` & `taipy-config-3.0.0.dev0/src/taipy/config/checker/_checkers/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.4.0.dev0/src/taipy/config/checker/_checkers/_auth_config_checker.py` & `taipy-config-3.0.0.dev0/src/taipy/config/checker/_checkers/_auth_config_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.4.0.dev0/src/taipy/config/checker/_checkers/_config_checker.py` & `taipy-config-3.0.0.dev0/src/taipy/config/checker/_checkers/_config_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.4.0.dev0/src/taipy/config/checker/_checkers/_global_config_checker.py` & `taipy-config-3.0.0.dev0/src/taipy/config/checker/_checkers/_global_config_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.4.0.dev0/src/taipy/config/checker/issue.py` & `taipy-config-3.0.0.dev0/src/taipy/config/checker/issue.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.4.0.dev0/src/taipy/config/checker/issue_collector.py` & `taipy-config-3.0.0.dev0/src/taipy/config/checker/issue_collector.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.4.0.dev0/src/taipy/config/common/__init__.py` & `taipy-config-3.0.0.dev0/src/taipy/config/common/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.4.0.dev0/src/taipy/config/common/_classproperty.py` & `taipy-config-3.0.0.dev0/src/taipy/config/common/_classproperty.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.4.0.dev0/src/taipy/config/common/_config_blocker.py` & `taipy-config-3.0.0.dev0/src/taipy/config/common/_config_blocker.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.4.0.dev0/src/taipy/config/common/_repr_enum.py` & `taipy-config-3.0.0.dev0/src/taipy/config/common/_repr_enum.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.4.0.dev0/src/taipy/config/common/_template_handler.py` & `taipy-config-3.0.0.dev0/src/taipy/config/common/_template_handler.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.4.0.dev0/src/taipy/config/common/_validate_id.py` & `taipy-config-3.0.0.dev0/src/taipy/config/common/_validate_id.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.4.0.dev0/src/taipy/config/common/frequency.py` & `taipy-config-3.0.0.dev0/src/taipy/config/common/frequency.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.4.0.dev0/src/taipy/config/common/scope.py` & `taipy-config-3.0.0.dev0/src/taipy/config/common/scope.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.4.0.dev0/src/taipy/config/config.py` & `taipy-config-3.0.0.dev0/src/taipy/config/config.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.4.0.dev0/src/taipy/config/config.pyi` & `taipy-config-3.0.0.dev0/src/taipy/config/config.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -159,29 +159,41 @@
     def _to_json(cls, _config: _Config) -> str:
         """"""
 
     @classmethod
     def _from_json(cls, config_as_str: str) -> _Config:
         """"""
 
+    @classmethod
+    @property
     def job_config(cls) -> JobConfig:
         """"""
 
+    @classmethod
+    @property
     def data_nodes(cls) -> Dict[str, DataNodeConfig]:
         """"""
 
+    @classmethod
+    @property
     def tasks(cls) -> Dict[str, TaskConfig]:
         """"""
 
+    @classmethod
+    @property
     def pipelines(cls) -> Dict[str, PipelineConfig]:
         """"""
 
+    @classmethod
+    @property
     def scenarios(cls) -> Dict[str, ScenarioConfig]:
         """"""
 
+    @classmethod
+    @property
     def core(cls) -> Dict[str, CoreSection]:
         """"""
 
     @staticmethod
     def configure_scenario(
         id: str,
         pipeline_configs: List[PipelineConfig],
```

### Comparing `taipy-config-2.4.0.dev0/src/taipy/config/exceptions/__init__.py` & `taipy-config-3.0.0.dev0/src/taipy/config/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.4.0.dev0/src/taipy/config/exceptions/exceptions.py` & `taipy-config-3.0.0.dev0/src/taipy/config/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.4.0.dev0/src/taipy/config/global_app/global_app_config.py` & `taipy-config-3.0.0.dev0/src/taipy/config/global_app/global_app_config.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.4.0.dev0/src/taipy/config/section.py` & `taipy-config-3.0.0.dev0/src/taipy/config/section.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.4.0.dev0/src/taipy/config/unique_section.py` & `taipy-config-3.0.0.dev0/src/taipy/config/unique_section.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.4.0.dev0/src/taipy/logger/__init__.py` & `taipy-config-3.0.0.dev0/src/taipy/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.4.0.dev0/src/taipy/logger/_taipy_logger.py` & `taipy-config-3.0.0.dev0/src/taipy/logger/_taipy_logger.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.4.0.dev0/src/taipy_config.egg-info/PKG-INFO` & `taipy-config-3.0.0.dev0/src/taipy_config.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: taipy-config
-Version: 2.4.0.dev0
+Version: 3.0.0.dev0
 Summary: A Taipy package dedicated to easily configure a Taipy application.
 Home-page: https://github.com/avaiga/taipy-config
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy-config
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Taipy config
 
 ## License
```

### Comparing `taipy-config-2.4.0.dev0/src/taipy_config.egg-info/SOURCES.txt` & `taipy-config-3.0.0.dev0/src/taipy_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

