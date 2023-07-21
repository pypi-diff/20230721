# Comparing `tmp/arcor2_arserver-1.0.0.tar.gz` & `tmp/arcor2_arserver-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcor2_arserver-1.0.0.tar", last modified: Tue Feb 14 12:55:49 2023, max compression
+gzip compressed data, was "arcor2_arserver-1.1.0.tar", last modified: Thu Jul 20 11:09:55 2023, max compression
```

## Comparing `arcor2_arserver-1.0.0.tar` & `arcor2_arserver-1.1.0.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-02-14 12:55:49.499360 arcor2_arserver-1.0.0/
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)       12 2023-02-14 12:55:48.000000 arcor2_arserver-1.0.0/MANIFEST.in
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)    14125 2023-02-14 12:55:49.499360 arcor2_arserver-1.0.0/PKG-INFO
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-02-14 12:55:49.495360 arcor2_arserver-1.0.0/arcor2_arserver/
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)        5 2023-02-14 12:55:48.000000 arcor2_arserver-1.0.0/arcor2_arserver/VERSION
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)      173 2023-02-14 12:55:48.000000 arcor2_arserver-1.0.0/arcor2_arserver/__init__.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)    13633 2023-02-14 12:55:48.000000 arcor2_arserver-1.0.0/arcor2_arserver/checks.py
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-02-14 12:55:49.499360 arcor2_arserver-1.0.0/arcor2_arserver/clients/
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)        0 2023-02-14 12:55:48.000000 arcor2_arserver-1.0.0/arcor2_arserver/clients/__init__.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     9641 2023-02-14 12:55:48.000000 arcor2_arserver-1.0.0/arcor2_arserver/clients/project_service.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     4139 2023-02-14 12:55:48.000000 arcor2_arserver-1.0.0/arcor2_arserver/common.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     1439 2023-02-14 12:55:48.000000 arcor2_arserver-1.0.0/arcor2_arserver/decorators.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)       84 2023-02-14 12:55:48.000000 arcor2_arserver-1.0.0/arcor2_arserver/events.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     5317 2023-02-14 12:55:48.000000 arcor2_arserver-1.0.0/arcor2_arserver/execution.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     1654 2023-02-14 12:55:48.000000 arcor2_arserver-1.0.0/arcor2_arserver/globals.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     3484 2023-02-14 12:55:48.000000 arcor2_arserver-1.0.0/arcor2_arserver/helpers.py
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-02-14 12:55:49.499360 arcor2_arserver-1.0.0/arcor2_arserver/lock/
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)      207 2023-02-14 12:55:48.000000 arcor2_arserver-1.0.0/arcor2_arserver/lock/__init__.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)      244 2023-02-14 12:55:48.000000 arcor2_arserver-1.0.0/arcor2_arserver/lock/common.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)      194 2023-02-14 12:55:48.000000 arcor2_arserver-1.0.0/arcor2_arserver/lock/exceptions.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)    25362 2023-02-14 12:55:48.000000 arcor2_arserver-1.0.0/arcor2_arserver/lock/lock.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)      611 2023-02-14 12:55:48.000000 arcor2_arserver-1.0.0/arcor2_arserver/lock/notifications.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     3883 2023-02-14 12:55:48.000000 arcor2_arserver-1.0.0/arcor2_arserver/lock/structures.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     1932 2023-02-14 12:55:48.000000 arcor2_arserver-1.0.0/arcor2_arserver/models.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)      622 2023-02-14 12:55:48.000000 arcor2_arserver-1.0.0/arcor2_arserver/notifications.py
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-02-14 12:55:49.499360 arcor2_arserver-1.0.0/arcor2_arserver/object_types/
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)        0 2023-02-14 12:55:48.000000 arcor2_arserver-1.0.0/arcor2_arserver/object_types/__init__.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)      978 2023-02-14 12:55:48.000000 arcor2_arserver-1.0.0/arcor2_arserver/object_types/data.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     2222 2023-02-14 12:55:48.000000 arcor2_arserver-1.0.0/arcor2_arserver/object_types/source.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     9553 2023-02-14 12:55:48.000000 arcor2_arserver-1.0.0/arcor2_arserver/object_types/utils.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)    10478 2023-02-14 12:55:48.000000 arcor2_arserver-1.0.0/arcor2_arserver/objects_actions.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     5098 2023-02-14 12:55:48.000000 arcor2_arserver-1.0.0/arcor2_arserver/project.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)        0 2023-02-14 12:55:48.000000 arcor2_arserver-1.0.0/arcor2_arserver/py.typed
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)    14607 2023-02-14 12:55:48.000000 arcor2_arserver-1.0.0/arcor2_arserver/robot.py
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-02-14 12:55:49.499360 arcor2_arserver-1.0.0/arcor2_arserver/rpc/
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)      276 2023-02-14 12:55:48.000000 arcor2_arserver-1.0.0/arcor2_arserver/rpc/__init__.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     3060 2023-02-14 12:55:48.000000 arcor2_arserver-1.0.0/arcor2_arserver/rpc/camera.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     1546 2023-02-14 12:55:48.000000 arcor2_arserver-1.0.0/arcor2_arserver/rpc/execution.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     1320 2023-02-14 12:55:48.000000 arcor2_arserver-1.0.0/arcor2_arserver/rpc/lock.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)    18307 2023-02-14 12:55:48.000000 arcor2_arserver-1.0.0/arcor2_arserver/rpc/objects.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)    54356 2023-02-14 12:55:48.000000 arcor2_arserver-1.0.0/arcor2_arserver/rpc/project.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)    24486 2023-02-14 12:55:48.000000 arcor2_arserver-1.0.0/arcor2_arserver/rpc/robot.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)    25722 2023-02-14 12:55:48.000000 arcor2_arserver-1.0.0/arcor2_arserver/rpc/scene.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     1192 2023-02-14 12:55:48.000000 arcor2_arserver-1.0.0/arcor2_arserver/rpc/user.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)    17315 2023-02-14 12:55:48.000000 arcor2_arserver-1.0.0/arcor2_arserver/scene.py
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-02-14 12:55:49.499360 arcor2_arserver-1.0.0/arcor2_arserver/scripts/
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)        0 2023-02-14 12:55:48.000000 arcor2_arserver-1.0.0/arcor2_arserver/scripts/__init__.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)    12036 2023-02-14 12:55:48.000000 arcor2_arserver-1.0.0/arcor2_arserver/scripts/arserver.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     1803 2023-02-14 12:55:48.000000 arcor2_arserver-1.0.0/arcor2_arserver/scripts/broadcaster.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)       98 2023-02-14 12:55:48.000000 arcor2_arserver-1.0.0/arcor2_arserver/settings.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     2545 2023-02-14 12:55:48.000000 arcor2_arserver-1.0.0/arcor2_arserver/user.py
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-02-14 12:55:49.499360 arcor2_arserver-1.0.0/arcor2_arserver.egg-info/
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)    14125 2023-02-14 12:55:49.000000 arcor2_arserver-1.0.0/arcor2_arserver.egg-info/PKG-INFO
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)     1628 2023-02-14 12:55:49.000000 arcor2_arserver-1.0.0/arcor2_arserver.egg-info/SOURCES.txt
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)        1 2023-02-14 12:55:49.000000 arcor2_arserver-1.0.0/arcor2_arserver.egg-info/dependency_links.txt
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)      136 2023-02-14 12:55:49.000000 arcor2_arserver-1.0.0/arcor2_arserver.egg-info/entry_points.txt
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)        1 2023-02-14 12:55:49.000000 arcor2_arserver-1.0.0/arcor2_arserver.egg-info/namespace_packages.txt
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)      458 2023-02-14 12:55:49.000000 arcor2_arserver-1.0.0/arcor2_arserver.egg-info/requires.txt
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)       16 2023-02-14 12:55:49.000000 arcor2_arserver-1.0.0/arcor2_arserver.egg-info/top_level.txt
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)      698 2023-02-14 12:55:48.000000 arcor2_arserver-1.0.0/backend_shim.py
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)       38 2023-02-14 12:55:49.499360 arcor2_arserver-1.0.0/setup.cfg
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)    15670 2023-02-14 12:55:48.000000 arcor2_arserver-1.0.0/setup.py
+drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-07-20 11:09:55.066956 arcor2_arserver-1.1.0/
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)       12 2023-07-20 11:09:54.000000 arcor2_arserver-1.1.0/MANIFEST.in
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)    14259 2023-07-20 11:09:55.066956 arcor2_arserver-1.1.0/PKG-INFO
+drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-07-20 11:09:55.062956 arcor2_arserver-1.1.0/arcor2_arserver/
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)        5 2023-07-20 11:09:54.000000 arcor2_arserver-1.1.0/arcor2_arserver/VERSION
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)      173 2023-07-20 11:09:54.000000 arcor2_arserver-1.1.0/arcor2_arserver/__init__.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)    13611 2023-07-20 11:09:54.000000 arcor2_arserver-1.1.0/arcor2_arserver/checks.py
+drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-07-20 11:09:55.062956 arcor2_arserver-1.1.0/arcor2_arserver/clients/
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)        0 2023-07-20 11:09:54.000000 arcor2_arserver-1.1.0/arcor2_arserver/clients/__init__.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     9622 2023-07-20 11:09:54.000000 arcor2_arserver-1.1.0/arcor2_arserver/clients/project_service.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     4128 2023-07-20 11:09:54.000000 arcor2_arserver-1.1.0/arcor2_arserver/common.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     1439 2023-07-20 11:09:54.000000 arcor2_arserver-1.1.0/arcor2_arserver/decorators.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)       84 2023-07-20 11:09:54.000000 arcor2_arserver-1.1.0/arcor2_arserver/events.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     5310 2023-07-20 11:09:54.000000 arcor2_arserver-1.1.0/arcor2_arserver/execution.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     1653 2023-07-20 11:09:54.000000 arcor2_arserver-1.1.0/arcor2_arserver/globals.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     3481 2023-07-20 11:09:54.000000 arcor2_arserver-1.1.0/arcor2_arserver/helpers.py
+drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-07-20 11:09:55.062956 arcor2_arserver-1.1.0/arcor2_arserver/lock/
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)      207 2023-07-20 11:09:54.000000 arcor2_arserver-1.1.0/arcor2_arserver/lock/__init__.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)      243 2023-07-20 11:09:54.000000 arcor2_arserver-1.1.0/arcor2_arserver/lock/common.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)      194 2023-07-20 11:09:54.000000 arcor2_arserver-1.1.0/arcor2_arserver/lock/exceptions.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)    25357 2023-07-20 11:09:54.000000 arcor2_arserver-1.1.0/arcor2_arserver/lock/lock.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)      611 2023-07-20 11:09:54.000000 arcor2_arserver-1.1.0/arcor2_arserver/lock/notifications.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     3882 2023-07-20 11:09:54.000000 arcor2_arserver-1.1.0/arcor2_arserver/lock/structures.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     1925 2023-07-20 11:09:54.000000 arcor2_arserver-1.1.0/arcor2_arserver/models.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)      621 2023-07-20 11:09:54.000000 arcor2_arserver-1.1.0/arcor2_arserver/notifications.py
+drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-07-20 11:09:55.062956 arcor2_arserver-1.1.0/arcor2_arserver/object_types/
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)        0 2023-07-20 11:09:54.000000 arcor2_arserver-1.1.0/arcor2_arserver/object_types/__init__.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)      977 2023-07-20 11:09:54.000000 arcor2_arserver-1.1.0/arcor2_arserver/object_types/data.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     2221 2023-07-20 11:09:54.000000 arcor2_arserver-1.1.0/arcor2_arserver/object_types/source.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     9541 2023-07-20 11:09:54.000000 arcor2_arserver-1.1.0/arcor2_arserver/object_types/utils.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)    10466 2023-07-20 11:09:54.000000 arcor2_arserver-1.1.0/arcor2_arserver/objects_actions.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     5090 2023-07-20 11:09:54.000000 arcor2_arserver-1.1.0/arcor2_arserver/project.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)        0 2023-07-20 11:09:54.000000 arcor2_arserver-1.1.0/arcor2_arserver/py.typed
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)    14586 2023-07-20 11:09:54.000000 arcor2_arserver-1.1.0/arcor2_arserver/robot.py
+drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-07-20 11:09:55.066956 arcor2_arserver-1.1.0/arcor2_arserver/rpc/
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)      276 2023-07-20 11:09:54.000000 arcor2_arserver-1.1.0/arcor2_arserver/rpc/__init__.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     3056 2023-07-20 11:09:54.000000 arcor2_arserver-1.1.0/arcor2_arserver/rpc/camera.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     1544 2023-07-20 11:09:54.000000 arcor2_arserver-1.1.0/arcor2_arserver/rpc/execution.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     1315 2023-07-20 11:09:54.000000 arcor2_arserver-1.1.0/arcor2_arserver/rpc/lock.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)    18292 2023-07-20 11:09:54.000000 arcor2_arserver-1.1.0/arcor2_arserver/rpc/objects.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)    54287 2023-07-20 11:09:54.000000 arcor2_arserver-1.1.0/arcor2_arserver/rpc/project.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)    24447 2023-07-20 11:09:54.000000 arcor2_arserver-1.1.0/arcor2_arserver/rpc/robot.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)    25695 2023-07-20 11:09:54.000000 arcor2_arserver-1.1.0/arcor2_arserver/rpc/scene.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     1191 2023-07-20 11:09:54.000000 arcor2_arserver-1.1.0/arcor2_arserver/rpc/user.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)    17277 2023-07-20 11:09:54.000000 arcor2_arserver-1.1.0/arcor2_arserver/scene.py
+drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-07-20 11:09:55.066956 arcor2_arserver-1.1.0/arcor2_arserver/scripts/
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)        0 2023-07-20 11:09:54.000000 arcor2_arserver-1.1.0/arcor2_arserver/scripts/__init__.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)    12021 2023-07-20 11:09:54.000000 arcor2_arserver-1.1.0/arcor2_arserver/scripts/arserver.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     1800 2023-07-20 11:09:54.000000 arcor2_arserver-1.1.0/arcor2_arserver/scripts/broadcaster.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)       98 2023-07-20 11:09:54.000000 arcor2_arserver-1.1.0/arcor2_arserver/settings.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     2539 2023-07-20 11:09:54.000000 arcor2_arserver-1.1.0/arcor2_arserver/user.py
+drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-07-20 11:09:55.062956 arcor2_arserver-1.1.0/arcor2_arserver.egg-info/
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)    14259 2023-07-20 11:09:55.000000 arcor2_arserver-1.1.0/arcor2_arserver.egg-info/PKG-INFO
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)     1628 2023-07-20 11:09:55.000000 arcor2_arserver-1.1.0/arcor2_arserver.egg-info/SOURCES.txt
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)        1 2023-07-20 11:09:55.000000 arcor2_arserver-1.1.0/arcor2_arserver.egg-info/dependency_links.txt
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)      136 2023-07-20 11:09:55.000000 arcor2_arserver-1.1.0/arcor2_arserver.egg-info/entry_points.txt
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)        1 2023-07-20 11:09:55.000000 arcor2_arserver-1.1.0/arcor2_arserver.egg-info/namespace_packages.txt
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)      490 2023-07-20 11:09:55.000000 arcor2_arserver-1.1.0/arcor2_arserver.egg-info/requires.txt
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)       16 2023-07-20 11:09:55.000000 arcor2_arserver-1.1.0/arcor2_arserver.egg-info/top_level.txt
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)      822 2023-07-20 11:09:54.000000 arcor2_arserver-1.1.0/backend_shim.py
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)       38 2023-07-20 11:09:55.066956 arcor2_arserver-1.1.0/setup.cfg
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)    15858 2023-07-20 11:09:54.000000 arcor2_arserver-1.1.0/setup.py
```

### Comparing `arcor2_arserver-1.0.0/PKG-INFO` & `arcor2_arserver-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcor2_arserver
-Version: 1.0.0
+Version: 1.1.0
 Summary: ARCOR2 ARServer
 Author: Robo@FIT
 Author-email: imaterna@fit.vut.cz
 License: LGPL
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -42,14 +42,20 @@
 - `ARCOR2_ARSERVER_DEBUG=1` - switches logger to the `DEBUG` level. 
 - `ARCOR2_ARSERVER_ASYNCIO_DEBUG=1` - turns on `asyncio` debug output (helpful to debug problems related to concurrency). 
 - `ARCOR2_REST_DEBUG=1` - may be used to debug problems related to communication with the Project, Scene Build and Calibration services.
 # Changelog
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 
+## [1.1.0] - 2023-07-20
+
+### Changed
+
+- Compatibility with arcor2 1.1.0 (object pose must now be updated with `obj.set_pose(pose)`).
+
 ## [1.0.0] - 2023-02-14
 
 ### Changed
 
 - Dependency on arcor2 1.0.0.
 - Compatibility with the newest version of the Project service.
 - ARServer now also talks to Asset service (checks whether mesh/URDF exists).
```

### Comparing `arcor2_arserver-1.0.0/arcor2_arserver/checks.py` & `arcor2_arserver-1.1.0/arcor2_arserver/checks.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 from arcor2_arserver.objects_actions import get_types_dict
 from arcor2_arserver_data.objects import ObjectAction
 
 # TODO refactor the module somewhere, so it can be also used within arcor2_build?
 
 
 def find_object_action(obj_types: ObjectTypeDict, scene: CachedScene, action: Action) -> ObjectAction:
-
     obj_id, action_type = action.parse_type()
     obj = scene.object(obj_id)
     obj_type = obj_types[obj.type]
 
     try:
         act = obj_type.actions[action_type]
     except KeyError:
@@ -50,33 +49,30 @@
 
     action_ids = parent.action_ids()
 
     if logic_item.start == LogicItem.START and logic_item.end == LogicItem.END:
         raise Arcor2Exception("This does not make sense.")
 
     if logic_item.start != LogicItem.START:
-
         start_action_id, start_flow = logic_item.parse_start()
 
         if start_action_id == logic_item.end:
             raise Arcor2Exception("Start and end can't be the same.")
 
         if start_action_id not in action_ids:
             raise Arcor2Exception("Logic item has unknown start.")
 
         if start_flow != "default":  # TODO enum
             raise Arcor2Exception("Only flow 'default' is supported so far.'")
 
     if logic_item.end != LogicItem.END:
-
         if logic_item.end not in action_ids:
             raise Arcor2Exception("Logic item has unknown end.")
 
     if logic_item.condition is not None:
-
         what = logic_item.condition.parse_what()
         action = parent.action(what.action_id)  # action that produced the result which we depend on here
         flow = action.flow(what.flow_name)
         try:
             flow.outputs[what.output_index]
         except IndexError:
             raise Arcor2Exception(f"Flow {flow.type} does not have output with index {what.output_index}.")
@@ -101,68 +97,61 @@
         # TODO perform this check using plugin
         from arcor2 import json
 
         if not isinstance(json.loads(logic_item.condition.value), bool):
             raise Arcor2Exception("Invalid condition value.")
 
     for existing_item in parent.logic:
-
         if existing_item.id == logic_item.id:  # item is updated
             continue
 
         if logic_item.start == logic_item.START and existing_item.start == logic_item.START:
             raise Arcor2Exception("START already defined.")
 
         if logic_item.start == existing_item.start:
-
             if None in (logic_item.condition, existing_item.condition):
                 raise Arcor2Exception("Two junctions has the same start action without condition.")
 
             # when there are more logical connections from A to B, their condition values must be different
             if logic_item.condition == existing_item.condition:
                 raise Arcor2Exception("Two junctions with the same start should have different conditions.")
 
         if logic_item.end == existing_item.end:
             if logic_item.start == existing_item.start:
                 raise Arcor2Exception("Junctions can't have the same start and end.")
 
 
 def check_parameter(parameter: Parameter) -> None:
-
     # TODO check using (some) plugin
     from arcor2 import json
 
     val = json.loads(parameter.value)
 
     # however, analysis in get_dataclass_params() can handle also (nested) dataclasses, etc.
     if not isinstance(val, (int, float, str, bool)):
         raise Arcor2Exception("Only basic types are supported so far.")
 
 
 def check_object_parameters(obj_type: ObjectTypeData, parameters: list[Parameter]) -> None:
-
     if {s.name for s in obj_type.meta.settings if s.default_value is None} > {s.name for s in parameters}:
         raise Arcor2Exception("Some required parameter is missing.")
 
     param_dict = obj_type.meta.parameters_dict()
 
     for param in parameters:
-
         if param_dict[param.name].type != param.type:
             raise Arcor2Exception(f"Type mismatch for parameter {param}.")
 
         check_parameter(param)
 
 
 def check_project_parameter(proj: CachedProject, parameter: ProjectParameter) -> None:
-
     hlp.is_valid_identifier(parameter.name)
 
     for pparam in proj.parameters:
-
         if parameter.id == pparam.id:
             continue
 
         if parameter.name == pparam.name:
             raise Arcor2Exception(f"Project parameter name {parameter.name} is duplicate.")
 
     check_parameter(parameter)
@@ -191,49 +180,44 @@
     if not obj_type.meta.has_pose and obj.pose is not None:
         raise Arcor2Exception(f"Object {obj.name} should not have pose.")
 
     if obj_type.meta.abstract:
         raise Arcor2Exception(f"ObjectType {obj.type} is abstract.")
 
     if new_one:
-
         if obj.id in scene.object_ids:
             raise Arcor2Exception(f"Object {obj.name} has duplicate id.")
 
         if obj.name in scene.object_names():
             raise Arcor2Exception(f"Object name {obj.name} is duplicate.")
 
     hlp.is_valid_identifier(obj.name)
 
 
 def check_action_params(
     obj_types: ObjectTypeDict, scene: CachedScene, project: CachedProject, action: Action, object_action: ObjectAction
 ) -> None:
-
     _, action_type = action.parse_type()
 
     assert action_type == object_action.name
 
     if len(object_action.parameters) != len(action.parameters):
         raise Arcor2Exception("Unexpected number of parameters.")
 
     for req_param in object_action.parameters:
-
         param = action.parameter(req_param.name)
 
         if param.type == ActionParameter.TypeEnum.PROJECT_PARAMETER:
-
             pparam = project.parameter(param.str_from_value())
 
             param_meta = object_action.parameter(param.name)
             if param_meta.type != pparam.type:
                 raise Arcor2Exception("Action parameter type does not match project parameter type.")
 
         elif param.type == ActionParameter.TypeEnum.LINK:
-
             parsed_link = param.parse_link()
 
             if parsed_link.action_id == action.id:
                 raise Arcor2Exception("Can't use own result as a parameter.")
 
             parent_action = project.action(parsed_link.action_id)
             source_action_pt = parent_action.parse_type()
@@ -253,15 +237,14 @@
             except IndexError:
                 raise Arcor2Exception(
                     f"Index {parsed_link.output_index} is invalid for action {object_action.name},"
                     f" which returns {len(object_action.returns)} values."
                 )
 
         else:
-
             if param.type not in known_parameter_types():
                 raise Arcor2Exception(f"Parameter {param.name} of action {action.name} has unknown type: {param.type}.")
 
             try:
                 plugin_from_type_name(param.type).parameter_value(
                     get_types_dict(), scene, project, action.id, param.name
                 )
@@ -298,66 +281,61 @@
         for fl in act.flows:
             for output in fl.outputs:
                 if output in outputs:
                     raise Arcor2Exception(f"Output '{output}' is not unique.")
 
 
 def scene_problems(obj_types: ObjectTypeDict, scene: CachedScene) -> list[str]:
-
     problems: list[str] = []
 
     for scene_obj in scene.objects:
         try:
             check_object(obj_types, scene, scene_obj)
         except Arcor2Exception as e:
             problems.append(str(e))
 
     return problems
 
 
 def check_ap_parent(scene: CachedScene, proj: CachedProject, parent: None | str) -> None:
-
     if not parent:
         return
 
     if parent in scene.object_ids:
         if scene.object(parent).pose is None:
             raise Arcor2Exception("AP can't have object without pose as parent.")
     elif parent not in proj.action_points_ids:
         raise Arcor2Exception("AP has invalid parent ID (not an object or another AP).")
 
 
 def project_problems(obj_types: ObjectTypeDict, scene: CachedScene, project: CachedProject) -> list[str]:
-
     if project.scene_id != scene.id:
         return ["Project/scene mismatch."]
 
     problems: list[str] = scene_problems(obj_types, scene)
 
     for proj_param in project.parameters:
         try:
             check_project_parameter(project, proj_param)
         except Arcor2Exception as e:
             problems.append(str(e))
 
     for ap in project.action_points:
-
         try:
             check_ap_parent(scene, project, ap.parent)
         except Arcor2Exception:
             problems.append(f"Action point {ap.name} has invalid parent: {ap.parent}.")
 
         for joints in project.ap_joints(ap.id):
             if joints.robot_id not in scene.object_ids:
                 problems.append(
                     f"Action point {ap.name} has joints ({joints.name}) for an unknown robot: {joints.robot_id}."
                 )
 
         for action in project.actions:
-
             # check if objects have used actions
             obj_id, action_type = action.parse_type()
 
             if obj_id not in scene.object_ids:
                 problems.append(f"Object ID {obj_id} which action is used in {action.name} does not exist in scene.")
                 continue
```

### Comparing `arcor2_arserver-1.0.0/arcor2_arserver/clients/project_service.py` & `arcor2_arserver-1.1.0/arcor2_arserver/clients/project_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 from arcor2.data.common import IdDesc
 from arcor2.data.object_type import ObjectType
 from arcor2.exceptions import Arcor2Exception
 
 
 @dataclass
 class CachedListing:
-
     __slots__ = "listing", "ts"
 
     listing: dict[str, IdDesc]
     ts: float
 
     def time_to_update(self) -> bool:
         return time.monotonic() - self.ts > _cache_timeout
@@ -68,92 +67,82 @@
     _projects = LRU(_cache_projects)
     _object_types = LRU(_cache_object_types)
 
 
 async def _update_list(
     getter: Callable[..., Awaitable[list[IdDesc]]], cached_listing: CachedListing, cache: dict[str, Any]
 ) -> None:
-
     if not cached_listing.time_to_update():
         return
 
     updated = {it.id: it for it in (await getter())}
     for deleted in cached_listing.listing.keys() - updated.keys():  # remove outdated items from the cache
         cache.pop(deleted, None)
     cached_listing.listing = updated
     cached_listing.ts = time.monotonic()
 
 
 async def initialize_module() -> None:
-
     await asyncio.gather(
         _update_list(ps.get_projects, _projects_list, _projects),
         _update_list(ps.get_scenes, _scenes_list, _scenes),
         _update_list(ps.get_object_type_ids, _object_type_list, _object_types),
     )
 
     _scenes.clear()
     _projects.clear()
     _object_types.clear()
 
 
 async def get_project_ids() -> set[str]:
-
     async with _projects_list_lock:
         await _update_list(ps.get_projects, _projects_list, _projects)
     return set(_projects_list.listing)
 
 
 async def get_projects() -> list[IdDesc]:
-
     async with _projects_list_lock:
         await _update_list(ps.get_projects, _projects_list, _projects)
     return list(_projects_list.listing.values())
 
 
 async def get_scene_ids() -> set[str]:
-
     async with _scenes_list_lock:
         await _update_list(ps.get_scenes, _scenes_list, _scenes)
     return set(_scenes_list.listing)
 
 
 async def get_scenes() -> list[IdDesc]:
-
     async with _scenes_list_lock:
         await _update_list(ps.get_scenes, _scenes_list, _scenes)
     return list(_scenes_list.listing.values())
 
 
 async def get_object_type_ids() -> set[str]:
-
     async with _object_type_lock:
         await _update_list(ps.get_object_type_ids, _object_type_list, _object_types)
     return set(_object_type_list.listing)
 
 
 async def get_object_types() -> list[IdDesc]:
-
     async with _object_type_lock:
         await _update_list(ps.get_object_type_ids, _object_type_list, _object_types)
     return list(_object_type_list.listing.values())
 
 
 async def get_object_type_iddesc(object_type_id: str) -> IdDesc:
-
     async with _object_type_lock:
         await _update_list(ps.get_object_type_ids, _object_type_list, _object_types)
     try:
         return _object_type_list.listing[object_type_id]
     except KeyError:
         raise ProjectServiceException("Unknown object type.")
 
 
 async def get_project(project_id: str) -> CachedProject:
-
     async with _projects_list_lock:
         try:
             project = _projects[project_id]
             assert project.modified
         except KeyError:
             project = CachedProject(await ps.get_project(project_id))
             _projects[project_id] = project
@@ -169,15 +158,14 @@
                 project = CachedProject(await ps.get_project(project_id))
                 _projects[project_id] = project
 
     return project
 
 
 async def get_scene(scene_id: str) -> CachedScene:
-
     async with _scenes_list_lock:
         try:
             scene = _scenes[scene_id]
             assert scene.modified
         except KeyError:
             scene = CachedScene(await ps.get_scene(scene_id))
             _scenes[scene_id] = scene
@@ -193,15 +181,14 @@
                 scene = CachedScene(await ps.get_scene(scene_id))
                 _scenes[scene_id] = scene
 
     return scene
 
 
 async def get_object_type(object_type_id: str) -> ObjectType:
-
     async with _object_type_lock:
         try:
             ot = _object_types[object_type_id]
             assert ot.modified
         except KeyError:
             ot = await ps.get_object_type(object_type_id)
             _object_types[object_type_id] = ot
@@ -217,15 +204,14 @@
                 ot = await ps.get_object_type(object_type_id)
                 _object_types[object_type_id] = ot
 
     return ot
 
 
 async def update_project(project: CachedProject) -> datetime:
-
     assert project.id
 
     ret = await ps.update_project(project.project)
     project.modified = ret
 
     if not project.created:
         project.created = project.modified
@@ -236,15 +222,14 @@
     _projects[project.id] = deepcopy(project)
     _projects[project.id].int_modified = None
 
     return ret
 
 
 async def update_scene(scene: CachedScene) -> datetime:
-
     assert scene.id
 
     ret = await ps.update_scene(scene.scene)
     scene.modified = ret
 
     if not scene.created:
         scene.created = scene.modified
@@ -253,15 +238,14 @@
     _scenes[scene.id] = deepcopy(scene)
     _scenes[scene.id].int_modified = None
 
     return ret
 
 
 async def update_object_type(object_type: ObjectType) -> datetime:
-
     assert object_type.id
 
     ret = await ps.update_object_type(object_type)
     object_type.modified = ret
 
     if not object_type.created:
         object_type.created = object_type.modified
@@ -271,29 +255,26 @@
     )
     _object_types[object_type.id] = deepcopy(object_type)
 
     return ret
 
 
 async def delete_scene(scene_id: str) -> None:
-
     await ps.delete_scene(scene_id)
     _scenes_list.listing.pop(scene_id, None)
     _scenes.pop(scene_id, None)
 
 
 async def delete_project(project_id: str) -> None:
-
     await ps.delete_project(project_id)
     _projects_list.listing.pop(project_id, None)
     _projects.pop(project_id, None)
 
 
 async def delete_object_type(object_type_id: str) -> None:
-
     await ps.delete_object_type(object_type_id)
     _object_type_list.listing.pop(object_type_id, None)
     _object_types.pop(object_type_id, None)
 
 
 __all__ = [
     initialize_module.__name__,
```

### Comparing `arcor2_arserver-1.0.0/arcor2_arserver/common.py` & `arcor2_arserver-1.1.0/arcor2_arserver/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,21 +16,19 @@
 
 
 async def associated_projects(scene_id: str) -> set[str]:
     return {project.id async for project in projects(scene_id)}
 
 
 async def remove_object_references_from_projects(obj_id: str) -> None:
-
     assert glob.LOCK.scene
 
     updated_project_ids: set[str] = set()
 
     async for project in projects_using_object_as_parent(glob.LOCK.scene.id, obj_id):
-
         # action_ids: set[str] = set()
 
         # delete actions using the object
         for action_to_delete in {act.id for act in project.actions if act.parse_type()[0] == obj_id}:
             project.remove_action(action_to_delete)
 
         # delete actions using obj's action points as parameters
@@ -54,36 +52,32 @@
         await storage.update_project(project)
         updated_project_ids.add(project.id)
 
     logger.info("Updated projects: {}".format(updated_project_ids))
 
 
 async def projects(scene_id: str) -> AsyncIterator[UpdateableCachedProject]:
-
     for project_meta in await storage.get_projects():
-
         project = await storage.get_project(project_meta.id)
 
         if project.scene_id != scene_id:
             continue
 
         yield UpdateableCachedProject(project)
 
 
 def _project_using_object_as_parent(project: CachedProject, obj_id: str) -> bool:
-
     for ap in project.action_points:
         if ap.parent == obj_id:
             return True
 
     return False
 
 
 def _project_referencing_object(project: CachedProject, obj_id: str) -> bool:
-
     for action in project.actions:
         action_obj_id, _ = action.parse_type()
 
         if action_obj_id == obj_id:
             return True
 
     return False
@@ -100,36 +94,31 @@
 
     async for project in projects(scene_id):
         if _project_using_object_as_parent(project, obj_id) or _project_referencing_object(project, obj_id):
             yield project
 
 
 async def projects_using_object_as_parent(scene_id: str, obj_id: str) -> AsyncIterator[UpdateableCachedProject]:
-
     async for project in projects(scene_id):
         if _project_using_object_as_parent(project, obj_id):
             yield project
 
 
 async def invalidate_joints_using_object_as_parent(obj: common.SceneObject) -> None:
-
     assert glob.LOCK.scene
 
     # Invalidates robot joints if action point's parent has changed its pose.
     async for project in projects_using_object_as_parent(glob.LOCK.scene.id, obj.id):
-
         for ap in project.action_points:
-
             if ap.parent != obj.id:
                 continue
 
             logger.debug(f"Invalidating joints for {project.name}/{ap.name}.")
             project.invalidate_joints(ap.id)
 
         await storage.update_project(project)
 
 
 async def projects_referencing_object(scene_id: str, obj_id: str) -> AsyncIterator[CachedProject]:
-
     async for project in projects(scene_id):
         if _project_referencing_object(project, obj_id):
             yield project
```

### Comparing `arcor2_arserver-1.0.0/arcor2_arserver/decorators.py` & `arcor2_arserver-1.1.0/arcor2_arserver/decorators.py`

 * *Files identical despite different names*

### Comparing `arcor2_arserver-1.0.0/arcor2_arserver/execution.py` & `arcor2_arserver-1.1.0/arcor2_arserver/execution.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,14 @@
     RespQueue = asyncio.Queue
 
 MANAGER_RPC_REQUEST_QUEUE: ReqQueue = ReqQueue()
 MANAGER_RPC_RESPONSES: dict[int, RespQueue] = {}
 
 
 async def run_temp_package(package_id: str, start_paused: bool = False, breakpoints: None | set[str] = None) -> None:
-
     # TODO lock scene and project?
 
     assert glob.LOCK.scene
     assert glob.LOCK.project
     project_id = glob.LOCK.project.id
     glob.TEMPORARY_PACKAGE = True
 
@@ -116,40 +115,34 @@
             raise Arcor2Exception("Upload to the Execution unit failed.")
         raise Arcor2Exception("\n".join(exe_resp.messages))
 
     return package_id
 
 
 async def manager_request(req: rpc.common.RPC.Request, ui: None | WsClient = None) -> rpc.common.RPC.Response:
-
     assert req.id not in MANAGER_RPC_RESPONSES
 
     MANAGER_RPC_RESPONSES[req.id] = RespQueue(maxsize=1)
     await MANAGER_RPC_REQUEST_QUEUE.put(req)
     resp = await MANAGER_RPC_RESPONSES[req.id].get()
     del MANAGER_RPC_RESPONSES[req.id]
     return resp
 
 
 async def project_manager_client(handle_manager_incoming_messages) -> None:
-
     while True:
-
         logger.info("Attempting connection to manager...")
 
         try:
-
             async with websockets.connect(EXE_URL) as manager_client:  # type: ignore  # TODO not sure what is wrong
-
                 logger.info("Connected to manager.")
 
                 future = asyncio.ensure_future(handle_manager_incoming_messages(manager_client))
 
                 while True:
-
                     if future.done():
                         break
 
                     try:
                         msg = await asyncio.wait_for(MANAGER_RPC_REQUEST_QUEUE.get(), 1.0)
                     except asyncio.TimeoutError:
                         continue
```

### Comparing `arcor2_arserver-1.0.0/arcor2_arserver/globals.py` & `arcor2_arserver-1.1.0/arcor2_arserver/globals.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,12 +43,11 @@
 
 USERS: Users = Users()
 
 PREV_RESULTS: dict[str, tuple[Any] | Any] = {}
 
 
 def remove_prev_result(action_id: str) -> None:
-
     try:
         del PREV_RESULTS[action_id]
     except KeyError:
         pass
```

### Comparing `arcor2_arserver-1.0.0/arcor2_arserver/helpers.py` & `arcor2_arserver-1.1.0/arcor2_arserver/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,24 +5,22 @@
 from arcor2_arserver import globals as glob
 from arcor2_arserver.decorators import retry
 from arcor2_arserver.lock.common import ObjIds, obj_ids_to_list
 from arcor2_arserver.lock.exceptions import CannotLock, LockingException
 
 
 def unique_name(name: str, existing_names: set[str]) -> None:
-
     if not name:
         raise Arcor2Exception("Name has to be set.")
 
     if name in existing_names:
         raise Arcor2Exception("Name already exists.")
 
 
 def make_name_unique(orig_name: str, names: set[str]) -> str:
-
     cnt = 1
     name = orig_name
 
     while name in names:
         name = f"{orig_name}_{cnt}"
         cnt += 1
 
@@ -62,15 +60,14 @@
     :param auto_unlock:
     :param dry_run:
     :return:
     """
 
     @retry(exc=CannotLock, tries=glob.LOCK._lock_retries, delay=glob.LOCK._retry_wait)
     async def lock() -> None:
-
         if not await glob.LOCK.read_lock(obj_ids, owner):
             raise CannotLock(glob.LOCK.ErrMessages.LOCK_FAIL.value)
 
     already_locked = False
 
     obj_ids = obj_ids_to_list(obj_ids)
```

### Comparing `arcor2_arserver-1.0.0/arcor2_arserver/lock/lock.py` & `arcor2_arserver-1.1.0/arcor2_arserver/lock/lock.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,15 +172,14 @@
     def _read_lock(self, roots: list[str], obj_ids: Iterable[str], owner: str) -> bool:
         """Private method when lock is already acquired."""
 
         assert self._lock.locked()
 
         locked: list[str] = []
         for i, obj_id in enumerate(obj_ids):
-
             if self._get_lock_record(roots[i]).read_lock(obj_id, owner):
                 locked.append(obj_id)
             else:
                 self._read_unlock(roots, locked, owner)
                 return False
         return True
 
@@ -244,15 +243,14 @@
     def _write_lock(self, roots: list[str], obj_ids: Iterable[str], owner: str, lock_tree: bool = False) -> bool:
         """Private method when lock is already acquired."""
 
         assert self._lock.locked()
 
         locked: list[str] = []
         for i, obj_id in enumerate(obj_ids):
-
             if self._get_lock_record(roots[i]).write_lock(obj_id, owner, lock_tree):
                 locked.append(obj_id)
             else:
                 self._write_unlock(roots, locked, owner)
                 return False
         return True
 
@@ -317,15 +315,14 @@
 
     def _is_write_locked(self, root_id: str, obj_id: str, owner: str, check_tree_locked: bool) -> bool:
         """Private method when lock is already acquired."""
 
         assert self._lock.locked()
 
         if lock_record := self._locked_objects.get(root_id):
-
             if obj_id in lock_record.write and owner == lock_record.write[obj_id]:
                 if check_tree_locked:
                     return lock_record.tree
                 return True
 
             if lock_record.tree:
                 write_locks = lock_record.write.values()
@@ -592,15 +589,14 @@
 
         root_id = await self.get_root_id(obj_id)
         children = self.get_all_children(obj_id)
         children.add(obj_id)
 
         async with self._lock:
             if lock_record := self._locked_objects.get(root_id):
-
                 if lock_record.tree and owner != next(iter(lock_record.write.values())):
                     return False
 
                 if not check_children(root_id, children.intersection(lock_record.write)):
                     return False
                 if not check_children(root_id, children.intersection(lock_record.read), True):
                     return False
@@ -682,15 +678,14 @@
 
         root_id = await self.get_root_id(obj_id)
         children = self.get_all_children(root_id)
         children.add(root_id)
 
         async with self._lock:
             if lock_record := self._locked_objects.get(root_id):
-
                 for lock in children.intersection(lock_record.write):
                     if owner != lock_record.write[lock]:
                         raise CannotLock(self.ErrMessages.SOMETHING_LOCKED_IN_TREE.value)
 
                 for lock in children.intersection(lock_record.read):
                     if len(lock_record.read[lock]) > 1 or owner not in lock_record.read[lock]:
                         raise CannotLock(self.ErrMessages.SOMETHING_LOCKED_IN_TREE.value)
```

### Comparing `arcor2_arserver-1.0.0/arcor2_arserver/lock/notifications.py` & `arcor2_arserver-1.1.0/arcor2_arserver/lock/notifications.py`

 * *Files identical despite different names*

### Comparing `arcor2_arserver-1.0.0/arcor2_arserver/lock/structures.py` & `arcor2_arserver-1.1.0/arcor2_arserver/lock/structures.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
         self.client = client
 
 
 class LockedObject:
     __slots__ = "read", "write", "tree"
 
     def __init__(self) -> None:
-
         # object id: owners
         self.read: dict[str, list[str]] = {}
         self.write: dict[str, str] = {}
 
         self.tree: bool = False
 
     def __repr__(self) -> str:
```

### Comparing `arcor2_arserver-1.0.0/arcor2_arserver/models.py` & `arcor2_arserver-1.1.0/arcor2_arserver/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,31 +8,27 @@
 from dataclasses_jsonschema.apispec import DataclassesPlugin
 
 from arcor2.data.events import Event
 from arcor2.data.rpc.common import RPC
 
 
 def _rename_childs(obj: type[JsonSchemaMixin] | type[Enum]) -> None:
-
     for _, child_obj in inspect.getmembers(obj, inspect.isclass):
-
         if issubclass(child_obj, (JsonSchemaMixin, Enum)):
-
             if hasattr(child_obj, "__renamed__"):
                 continue
 
             if "." in child_obj.__qualname__:
                 child_obj.__name__ = "".join(child_obj.__qualname__.split("."))
                 child_obj.__renamed__ = None
 
             _rename_childs(child_obj)
 
 
 def _add_to_spec(spec, obj) -> None:
-
     try:
         spec.components.schema(obj.__name__, schema=obj)
     except DuplicateComponentNameError:
         pass
 
 
 def generate_openapi(service_name: str, version: str, rpcs: list[type[RPC]], events: list[type[Event]]) -> str:
@@ -46,27 +42,24 @@
         title=f"{service_name} Data Models",
         version=version,
         openapi_version="3.0.2",
         plugins=[FlaskPlugin(), DataclassesPlugin()],
     )
 
     for obj in events:
-
         if obj is Event:
             continue
 
         _rename_childs(obj)
 
     for rpc in rpcs:
-
         if rpc is RPC:
             continue
 
         for cls in (rpc.Request, rpc.Response):
-
             cls.__name__ = rpc.__name__ + cls.__name__
             _rename_childs(cls)
 
     for obj in events:
         _add_to_spec(spec, obj)
     for rpc in rpcs:
         for cls in (rpc.Request, rpc.Response):
```

### Comparing `arcor2_arserver-1.0.0/arcor2_arserver/notifications.py` & `arcor2_arserver-1.1.0/arcor2_arserver/notifications.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from arcor2 import ws_server
 from arcor2.data import events
 from arcor2_arserver import globals as glob
 from arcor2_arserver import logger
 
 
 async def broadcast_event(event: events.Event) -> None:
-
     logger.debug(event)
 
     if glob.USERS.interfaces:
         message = event.to_json()
         await asyncio.gather(*[ws_server.send_json_to_client(intf, message) for intf in glob.USERS.interfaces])
```

### Comparing `arcor2_arserver-1.0.0/arcor2_arserver/object_types/data.py` & `arcor2_arserver-1.1.0/arcor2_arserver/object_types/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from arcor2.object_types.abstract import Generic
 from arcor2_arserver_data.objects import ObjectAction, ObjectTypeMeta
 from arcor2_arserver_data.robot import RobotMeta
 
 
 @dataclass
 class ObjectTypeData:
-
     meta: ObjectTypeMeta
     type_def: None | type[Generic] = None
     actions: dict[str, ObjectAction] = field(default_factory=dict)
     ast: None | AST = None
     robot_meta: None | RobotMeta = None
 
     def __post_init__(self) -> None:
```

### Comparing `arcor2_arserver-1.0.0/arcor2_arserver/object_types/source.py` & `arcor2_arserver-1.1.0/arcor2_arserver/object_types/source.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from arcor2.source import SourceException
 from arcor2.source.utils import find_function, find_raises, get_name
 from arcor2_arserver_data.objects import ObjectTypeMeta
 
 
 # TODO could this be done like this https://stackoverflow.com/a/9269964/3142796 ??
 def new_object_type(parent: ObjectTypeMeta, child: ObjectTypeMeta) -> AST:
-
     assert parent.type == child.base
 
     tree = Module(body=[], type_ignores=[])
 
     if parent.type in built_in_types_names():
         import_from = arcor2.object_types.abstract.__name__
     else:
```

### Comparing `arcor2_arserver-1.0.0/arcor2_arserver/object_types/utils.py` & `arcor2_arserver-1.1.0/arcor2_arserver/object_types/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,26 +24,24 @@
 
 
 class ObjectTypeException(Arcor2Exception):
     pass
 
 
 async def remove_object_type(obj_type_id: str) -> None:
-
     path = os.path.join(settings.OBJECT_TYPE_PATH, settings.OBJECT_TYPE_MODULE, f"{humps.depascalize(obj_type_id)}.py")
     logger.debug(f"Deleting {path}.")
 
     try:
         await hlp.run_in_executor(os.remove, path, propagate=[FileNotFoundError])
     except FileNotFoundError as e:
         raise Arcor2Exception(f"File for {obj_type_id} was not found.") from e
 
 
 def obj_description_from_base(data: ObjectTypeDict, obj_type: ObjectTypeMeta) -> str:
-
     try:
         obj = data[obj_type.base]
     except KeyError:
         raise Arcor2Exception(f"Unknown object type: {obj_type}.")
 
     if obj.meta.description:
         return obj.meta.description
@@ -89,15 +87,14 @@
 
         ret.append(pm)
 
     return ret
 
 
 def meta_from_def(type_def: type[Generic], built_in: bool = False) -> ObjectTypeMeta:
-
     obj = ObjectTypeMeta(
         type_def.__name__,
         type_def.description(),
         built_in=built_in,
         abstract=type_def.abstract(),
         has_pose=issubclass(type_def, GenericWithPose),
     )
@@ -109,20 +106,18 @@
 
     obj.settings = get_dataclass_params(get_settings_def(type_def))
 
     return obj
 
 
 def built_in_types_data() -> ObjectTypeDict:
-
     ret: ObjectTypeDict = {}
 
     # built-in object types / services
     for _, type_def in built_in_types():
-
         assert issubclass(type_def, Generic)
 
         ast = parse_def(type_def)
 
         d = ObjectTypeData(meta_from_def(type_def, built_in=True), type_def, object_actions(type_def, ast), ast)
 
         ret[d.meta.type] = d
@@ -131,33 +126,30 @@
 
 
 class IgnoreActionException(Arcor2Exception):
     pass
 
 
 def object_actions(type_def: type[Generic], tree: AST) -> dict[str, ObjectAction]:
-
     ret: dict[str, ObjectAction] = {}
 
     # ...inspect.ismethod does not work on un-initialized classes
     for method_name, method_def in iterate_over_actions(type_def):
-
         meta: ActionMetadata = method_def.__action__  # type: ignore
 
         if meta.hidden:
             logger.debug(f"Action {method_name} of {type_def.__name__} is hidden.")
             continue
 
         data = ObjectAction(name=method_name, meta=meta)
 
         if method_name in type_def.CANCEL_MAPPING:
             meta.cancellable = True
 
         try:
-
             docstring = parse_docstring(method_def.__doc__)
             data.description = docstring.short_description
 
             signature = inspect.signature(method_def)  # sig.parameters is OrderedDict
 
             try:
                 method_tree = find_function(method_name, tree)
@@ -185,27 +177,25 @@
             try:
                 return_ttype = hints["return"]
             except KeyError:
                 raise IgnoreActionException("Action is missing return type annotation.")
 
             # ...just ignore NoneType for returns
             if return_ttype != type(None):  # noqa: E721
-
                 if typing_inspect.is_tuple_type(return_ttype):
                     for arg in typing_inspect.get_args(return_ttype):
                         resolved_param = plugin_from_type(arg)
                         if resolved_param is None:
                             raise IgnoreActionException("None in return tuple is not supported.")
                         data.returns.append(resolved_param.type_name())
                 else:
                     # TODO resolving needed for e.g. enums - add possible values to action metadata somewhere?
                     data.returns = [plugin_from_type(return_ttype).type_name()]
 
             for name in parameter_names_without_self[:-1]:  # omit also an
-
                 try:
                     ttype = hints[name]
                 except KeyError:
                     raise IgnoreActionException(f"Parameter {name} is missing type annotation.")
 
                 param_type = plugin_from_type(ttype)
 
@@ -237,29 +227,27 @@
 
         ret[data.name] = data
 
     return ret
 
 
 def add_ancestor_actions(obj_type_name: str, object_types: ObjectTypeDict) -> None:
-
     base_name = object_types[obj_type_name].meta.base
 
     if not base_name:
         return
 
     if object_types[base_name].meta.base:
         add_ancestor_actions(base_name, object_types)
 
     # do not add action from base if it is overridden in child
     # TODO rewrite (use adv. of dict!)
     for base_action in object_types[base_name].actions.values():
         for obj_action in object_types[obj_type_name].actions.values():
             if base_action.name == obj_action.name:
-
                 # built-in object has no "origins" yet
                 if not obj_action.origins:
                     obj_action.origins = base_name
                 break
         else:
             action = copy.deepcopy(base_action)
             if not action.origins:
```

### Comparing `arcor2_arserver-1.0.0/arcor2_arserver/objects_actions.py` & `arcor2_arserver-1.1.0/arcor2_arserver/objects_actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 )
 from arcor2_arserver.robot import get_robot_meta
 from arcor2_arserver_data.events.objects import ChangedObjectTypes
 from arcor2_arserver_data.objects import ObjectTypeMeta
 
 
 def get_types_dict() -> TypesDict:
-
     return {k: v.type_def for k, v in glob.OBJECT_TYPES.items() if v.type_def is not None}
 
 
 def get_obj_type_data(scene: CachedScene, object_id: str) -> ObjectTypeData:
     return glob.OBJECT_TYPES[scene.object(object_id).type]
 
 
@@ -47,25 +46,23 @@
     :return:
     """
 
     return {obj_type: obj for obj_type, obj in glob.OBJECT_TYPES.items() if not obj.meta.disabled}
 
 
 async def get_object_data(object_types: ObjectTypeDict, obj_id: str) -> None:
-
     logger.debug(f"Processing {obj_id}.")
 
     if obj_id in object_types:
         logger.debug(f"{obj_id} already processed, skipping...")
         return
 
     obj_iddesc = await storage.get_object_type_iddesc(obj_id)
 
     if obj_id in glob.OBJECT_TYPES:
-
         assert obj_iddesc.modified
         assert glob.OBJECT_TYPES[obj_id].meta.modified, f"Object {obj_id} does not have 'modified' in its meta."
 
         if obj_iddesc.modified == glob.OBJECT_TYPES[obj_id].meta.modified:
             logger.debug(f"No need to update {obj_id}.")
             return
 
@@ -155,15 +152,14 @@
     ast = parse(obj.source)
     otd = ObjectTypeData(meta, type_def, object_actions(type_def, ast), ast)
 
     object_types[obj_id] = otd
 
 
 class UpdatedObjectTypes(NamedTuple):
-
     new: set[str]
     updated: set[str]
     removed: set[str]
 
     @property
     def all(self) -> set[str]:
         return self.new | self.updated | self.removed
@@ -204,15 +200,14 @@
     new_object_ids = {k for k in updated_object_types.keys() if k not in glob.OBJECT_TYPES}
 
     logger.debug(f"Removed ids: {removed_object_ids}")
     logger.debug(f"Updated ids: {updated_object_ids}")
     logger.debug(f"New ids: {new_object_ids}")
 
     if not initialization and removed_object_ids:
-
         # TODO remove it from sys.modules
 
         remove_evt = ChangedObjectTypes([v.meta for k, v in glob.OBJECT_TYPES.items() if k in removed_object_ids])
         remove_evt.change_type = Event.Type.REMOVE
         asyncio.ensure_future(notif.broadcast_event(remove_evt))
 
         for removed in removed_object_ids:
@@ -221,65 +216,58 @@
             await remove_object_type(removed)
 
     glob.OBJECT_TYPES.update(updated_object_types)
 
     logger.debug(f"All known ids: {glob.OBJECT_TYPES.keys()}")
 
     for obj_type in updated_object_types.values():
-
         # if description is missing, try to get it from ancestor(s)
         if not obj_type.meta.description:
-
             try:
                 obj_type.meta.description = obj_description_from_base(glob.OBJECT_TYPES, obj_type.meta)
             except otu.DataError as e:
                 logger.error(f"Failed to get info from base for {obj_type}, error: '{e}'.")
 
         if not obj_type.meta.disabled and not obj_type.meta.built_in:
             add_ancestor_actions(obj_type.meta.type, glob.OBJECT_TYPES)
 
     if not initialization:
-
         if updated_object_ids:
             update_evt = ChangedObjectTypes([v.meta for k, v in glob.OBJECT_TYPES.items() if k in updated_object_ids])
             update_evt.change_type = Event.Type.UPDATE
             asyncio.ensure_future(notif.broadcast_event(update_evt))
 
         if new_object_ids:
             add_evt = ChangedObjectTypes([v.meta for k, v in glob.OBJECT_TYPES.items() if k in new_object_ids])
             add_evt.change_type = Event.Type.ADD
             asyncio.ensure_future(notif.broadcast_event(add_evt))
 
     for obj_type in updated_object_types.values():
-
         if obj_type.type_def and issubclass(obj_type.type_def, Robot) and not obj_type.type_def.abstract():
             await get_robot_meta(obj_type)
 
     # if object does not change but its base has changed, it has to be reloaded
     for obj_id, obj in glob.OBJECT_TYPES.items():
-
         if obj_id in updated_object_ids:
             continue
 
         if obj.type_def and obj.meta.base in updated_object_ids:
-
             logger.debug(f"Re-importing {obj.meta.type} because its base {obj.meta.base} type has changed.")
             obj.type_def = await hlp.run_in_executor(
                 hlp.import_type_def,
                 obj.meta.type,
                 Generic,
                 settings.OBJECT_TYPE_PATH,
                 settings.OBJECT_TYPE_MODULE,
             )
 
     return UpdatedObjectTypes(new_object_ids, updated_object_ids, removed_object_ids)
 
 
 async def update_object_model(meta: ObjectTypeMeta, om: ObjectModel) -> None:
-
     if not meta.object_model:
         return
 
     model = om.model()
 
     if model.id != meta.type:
         raise Arcor2Exception("Model id must be equal to ObjectType id.")
```

### Comparing `arcor2_arserver-1.0.0/arcor2_arserver/project.py` & `arcor2_arserver-1.1.0/arcor2_arserver/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 
     if (
         project.id not in _project_problems
         or _project_problems[project.id].scene_modified < scene.modified
         or _project_problems[project.id].project_modified < project.modified
         or _project_problems[project.id].ot_modified != ot_modified
     ):
-
         logger.debug(f"Updating project_problems for {project.name}.")
 
         _project_problems[project.id] = ProjectProblems(
             scene.modified,
             project_problems(glob.OBJECT_TYPES, scene, project),
             ot_modified,
             project.modified,
@@ -60,58 +59,52 @@
 
     sp = _project_problems[project.id].problems
 
     return sp if sp else None
 
 
 async def notify_project_opened(evt: OpenProject) -> None:
-
     await notif.broadcast_event(evt)
     await notif.broadcast_event(get_scene_state())
 
 
 async def notify_project_closed(project_id: str, show_mainscreen_after_that: bool = True) -> None:
-
     proj_list = ShowMainScreen.Data.WhatEnum.ProjectsList
 
     await notif.broadcast_event(ProjectClosed())
     if show_mainscreen_after_that:  # mainscreen is not shown when running a temporary package
         glob.MAIN_SCREEN = ShowMainScreen.Data(proj_list)
         await notif.broadcast_event(ShowMainScreen(ShowMainScreen.Data(proj_list, project_id)))
 
 
 async def close_project(show_mainscreen_after_that: bool = True) -> None:
-
     assert glob.LOCK.project
 
     project_id = glob.LOCK.project.project.id
     glob.LOCK.scene = None
     glob.LOCK.project = None
     glob.PREV_RESULTS.clear()
     asyncio.ensure_future(notify_project_closed(project_id, show_mainscreen_after_that))
 
 
 async def execute_action(action_method: Callable, params: list[Any]) -> None:
-
     assert glob.RUNNING_ACTION
 
     await notif.broadcast_event(ActionExecution(ActionExecution.Data(glob.RUNNING_ACTION)))
 
     evt = ActionResult(ActionResult.Data(glob.RUNNING_ACTION))
 
     try:
         action_result = await hlp.run_in_executor(action_method, *params)
     except Arcor2Exception as e:
         logger.error(f"Failed to run method {action_method.__name__} with params {params}. {str(e)}")
         logger.debug(str(e), exc_info=True)
         evt.data.error = str(e)
     else:
-
         if action_result is not None:
-
             glob.PREV_RESULTS[glob.RUNNING_ACTION] = action_result
 
             try:
                 evt.data.results = results_to_json(action_result)
             except Arcor2Exception:
                 logger.error(f"Method {action_method.__name__} returned unsupported type of result: {action_result}.")
 
@@ -121,15 +114,14 @@
 
     glob.RUNNING_ACTION = None
     glob.RUNNING_ACTION_PARAMS = None
     await notif.broadcast_event(evt)
 
 
 async def open_project(project_id: str) -> None:
-
     project = await storage.get_project(project_id)
 
     if glob.LOCK.scene:
         if glob.LOCK.scene.id != project.scene_id:
             raise Arcor2Exception("Required project is associated to another scene.")
     else:
         await open_scene(project.scene_id)
```

### Comparing `arcor2_arserver-1.0.0/arcor2_arserver/robot.py` & `arcor2_arserver-1.1.0/arcor2_arserver/robot.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 
 
 class SingleArmRobotException(Arcor2Exception):
     pass
 
 
 def prepare_args(robot_inst: Robot, args: list[Any], arm_id: None | str) -> list[Any]:
-
     if isinstance(robot_inst, MultiArmRobot):
         args.append(arm_id)
     elif arm_id:
         raise SingleArmRobotException("Single arm robot.")
 
     return args
 
@@ -74,15 +73,14 @@
 
     return await hlp.run_in_executor(robot_inst.suctions, *prepare_args(robot_inst, [], arm_id))
 
 
 async def get_pose_and_joints(
     robot_inst: Robot, end_effector: str, arm_id: None | str
 ) -> tuple[common.Pose, list[common.Joint]]:
-
     return await asyncio.gather(
         hlp.run_in_executor(robot_inst.get_end_effector_pose, *prepare_args(robot_inst, [end_effector], arm_id)),
         hlp.run_in_executor(robot_inst.robot_joints, *prepare_args(robot_inst, [False], arm_id)),
     )
 
 
 async def get_end_effector_pose(robot_inst: Robot, end_effector: str, arm_id: None | str) -> common.Pose:
@@ -103,15 +101,14 @@
     :return: List of joints
     """
 
     return await hlp.run_in_executor(robot_inst.robot_joints, *prepare_args(robot_inst, [include_gripper], arm_id))
 
 
 def _feature(type_def: type[Robot], method_name: str, base_class: type[Robot]) -> bool:
-
     assert glob.OBJECT_TYPES
 
     method = getattr(type_def, method_name)
     where_it_is_defined = glob.OBJECT_TYPES.get(method.__qualname__.split(".")[0], None)
 
     if where_it_is_defined is None:
         raise Arcor2Exception(f"Can't get origin for {type_def.__name__}/{method_name}.")
@@ -137,15 +134,14 @@
     sign = inspect.signature(getattr(where_it_is_defined.type_def, method_name))
     if not (res := inspect.signature(getattr(base_class, method_name)) == sign):
         logger.debug(f"{type_def.__name__}/{method_name} has invalid signature.")
     return res
 
 
 async def get_robot_meta(obj_type: ObjectTypeData) -> None:
-
     if obj_type.meta.disabled:
         raise Arcor2Exception("Disabled object type.")
 
     assert obj_type.type_def is not None
 
     if not issubclass(obj_type.type_def, Robot):
         raise Arcor2Exception("Not a robot.")
@@ -168,80 +164,73 @@
         obj_type.type_def, Robot.forward_kinematics.__name__, base_class
     )
     obj_type.robot_meta.features.hand_teaching = _feature(
         obj_type.type_def, Robot.set_hand_teaching_mode.__name__, base_class
     )
 
     if urdf_name := obj_type.type_def.urdf_package_name:
-
         if not await asset.asset_exists(urdf_name):
             logger.error(f"URDF package {urdf_name} for {obj_type.meta.type} does not exist.")
         else:
             obj_type.robot_meta.urdf_package_filename = urdf_name
             # TODO check if URDF is valid?
 
     logger.debug(obj_type.robot_meta)
 
 
 async def stop(robot_inst: Robot) -> None:
-
     if not robot_inst.move_in_progress:
         raise Arcor2Exception("Robot is not moving.")
 
     await hlp.run_in_executor(robot_inst.stop)
 
 
 async def ik(
     robot_inst: Robot,
     end_effector_id: str,
     arm_id: None | str,
     pose: common.Pose,
     start_joints: None | list[common.Joint] = None,
     avoid_collisions: bool = True,
 ) -> list[common.Joint]:
-
     return await hlp.run_in_executor(
         robot_inst.inverse_kinematics,
         *prepare_args(robot_inst, [end_effector_id, pose, start_joints, avoid_collisions], arm_id),
     )
 
 
 async def fk(robot_inst: Robot, end_effector_id: str, arm_id: None | str, joints: list[common.Joint]) -> common.Pose:
-
     return await hlp.run_in_executor(
         robot_inst.forward_kinematics, *prepare_args(robot_inst, [end_effector_id, joints], arm_id)
     )
 
 
 async def check_reachability(
     scene: CachedScene,
     robot_inst: Robot,
     end_effector_id: str,
     arm_id: None | str,
     pose: common.Pose,
     safe: bool = True,
 ) -> None:
-
     otd = osa.get_obj_type_data(scene, robot_inst.id)
     if otd.robot_meta and otd.robot_meta.features.inverse_kinematics:
         try:
             await ik(robot_inst, end_effector_id, arm_id, pose, avoid_collisions=safe)
         except Robot.KinematicsException:
             raise Arcor2Exception("Unreachable pose.")
         except Arcor2Exception as e:
             logger.exception("Failed to check reachability.")
             raise Arcor2Exception("Error on getting IK.") from e
 
 
 async def check_robot_before_move(robot_inst: Robot) -> None:
-
     robot_inst.check_if_ready_to_move()
 
     if glob.RUNNING_ACTION:
-
         assert glob.LOCK.project
         action = glob.LOCK.project.action(glob.RUNNING_ACTION)
         obj_id_str, _ = action.parse_type()
 
         if robot_inst.id == obj_id_str:
             raise Arcor2Exception("Robot is executing action.")
 
@@ -272,15 +261,14 @@
     arm_id: None | str,
     pose: common.Pose,
     speed: float,
     safe: bool,
     linear: bool,
     lock_owner: None | str = None,
 ) -> None:
-
     try:
         Data = sevts.r.RobotMoveToPose.Data
 
         await notif.broadcast_event(
             sevts.r.RobotMoveToPose(
                 Data(Data.MoveEventType.START, robot_inst.id, end_effector_id, pose, safe, linear, arm_id=arm_id)
             )
@@ -313,15 +301,14 @@
     arm_id: None | str,
     pose: common.Pose,
     speed: float,
     orientation_id: str,
     safe: bool,
     linear: bool,
 ) -> None:
-
     Data = sevts.r.RobotMoveToActionPointOrientation.Data
 
     await notif.broadcast_event(
         sevts.r.RobotMoveToActionPointOrientation(
             Data(Data.MoveEventType.START, robot_inst.id, end_effector_id, orientation_id, safe, linear, arm_id=arm_id)
         )
     )
@@ -352,15 +339,14 @@
         )
     )
 
 
 async def _move_to_joints(
     robot_inst: Robot, joints: list[common.Joint], speed: float, safe: bool, arm_id: None | str
 ) -> None:
-
     # TODO newly connected interface should be notified somehow (general solution for such cases would be great!)
 
     try:
         await hlp.run_in_executor(robot_inst.move_to_joints, *prepare_args(robot_inst, [joints, speed, safe], arm_id))
     except Arcor2Exception as e:
         logger.error(f"Robot movement failed with: {str(e)}")
         raise
@@ -370,28 +356,25 @@
     robot_inst: Robot,
     joints: list[common.Joint],
     speed: float,
     safe: bool,
     arm_id: None | str,
     lock_owner: None | str = None,
 ) -> None:
-
     try:
         Data = sevts.r.RobotMoveToJoints.Data
 
         await notif.broadcast_event(
             sevts.r.RobotMoveToJoints(Data(Data.MoveEventType.START, robot_inst.id, joints, safe, arm_id=arm_id))
         )
 
         try:
-
             await _move_to_joints(robot_inst, joints, speed, safe, arm_id)
 
         except Arcor2Exception as e:
-
             await notif.broadcast_event(
                 sevts.r.RobotMoveToJoints(
                     Data(Data.MoveEventType.FAILED, robot_inst.id, joints, safe, str(e), arm_id=arm_id)
                 )
             )
 
             return
@@ -408,29 +391,26 @@
     robot_inst: Robot,
     joints: list[common.Joint],
     speed: float,
     joints_id: str,
     safe: bool,
     arm_id: None | str,
 ) -> None:
-
     Data = sevts.r.RobotMoveToActionPointJoints.Data
 
     await notif.broadcast_event(
         sevts.r.RobotMoveToActionPointJoints(
             Data(Data.MoveEventType.START, robot_inst.id, joints_id, safe, arm_id=arm_id)
         )
     )
 
     try:
-
         await _move_to_joints(robot_inst, joints, speed, safe, arm_id)
 
     except Arcor2Exception as e:
-
         await notif.broadcast_event(
             sevts.r.RobotMoveToActionPointJoints(
                 Data(Data.MoveEventType.FAILED, robot_inst.id, joints_id, safe, str(e), arm_id)
             )
         )
 
         return
@@ -439,15 +419,14 @@
         sevts.r.RobotMoveToActionPointJoints(
             Data(Data.MoveEventType.END, robot_inst.id, joints_id, safe, arm_id=arm_id)
         )
     )
 
 
 async def check_eef_arm(robot_inst: Robot, arm_id: None | str, eef_id: None | str = None) -> None:
-
     if isinstance(robot_inst, MultiArmRobot):
         if not arm_id:
             raise Arcor2Exception("Arm has to be specified.")
 
         if eef_id is not None and eef_id not in await hlp.run_in_executor(robot_inst.get_end_effectors_ids, arm_id):
             raise Arcor2Exception("Unknown end effector.")
```

### Comparing `arcor2_arserver-1.0.0/arcor2_arserver/rpc/camera.py` & `arcor2_arserver-1.1.0/arcor2_arserver/rpc/camera.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,30 +14,28 @@
 from arcor2_arserver.scene import ensure_scene_started, get_instance, update_scene_object_pose
 from arcor2_arserver_data.events.common import ProcessState
 from arcor2_arserver_data.rpc.camera import CalibrateCamera, CameraColorImage, CameraColorParameters
 from arcor2_calibration_data import client as calib_client
 
 
 async def camera_color_image_cb(req: CameraColorImage.Request, ui: WsClient) -> CameraColorImage.Response:
-
     glob.LOCK.scene_or_exception()
 
     await ensure_write_locked(req.args.id, glob.USERS.user_name(ui))
 
     ensure_scene_started()
     camera = get_instance(req.args.id, Camera)
     resp = CameraColorImage.Response()
     resp.data = image_to_str(camera.color_image())
     return resp
 
 
 async def camera_color_parameters_cb(
     req: CameraColorParameters.Request, ui: WsClient
 ) -> CameraColorParameters.Response:
-
     glob.LOCK.scene_or_exception()
 
     await ensure_write_locked(req.args.id, glob.USERS.user_name(ui))
 
     ensure_scene_started()
     camera = get_instance(req.args.id, Camera)
     resp = CameraColorParameters.Response()
@@ -45,15 +43,14 @@
     return resp
 
 
 CAMERA_CALIB = "CameraCalibration"
 
 
 async def calibrate_camera(scene: UpdateableCachedScene, camera: Camera) -> None:
-
     assert camera.color_camera_params
 
     await notif.broadcast_event(ProcessState(ProcessState.Data(CAMERA_CALIB, ProcessState.Data.StateEnum.Started)))
     try:
         img = await run_in_executor(camera.color_image)
         estimated_pose = await run_in_executor(calib_client.estimate_camera_pose, camera.color_camera_params, img)
     except Arcor2Exception as e:
@@ -64,15 +61,14 @@
         return
 
     await update_scene_object_pose(scene, scene.object(camera.id), estimated_pose.pose, camera)
     await notif.broadcast_event(ProcessState(ProcessState.Data(CAMERA_CALIB, ProcessState.Data.StateEnum.Finished)))
 
 
 async def calibrate_camera_cb(req: CalibrateCamera.Request, ui: WsClient) -> None:
-
     scene = glob.LOCK.scene_or_exception()
 
     ensure_scene_started()
     camera = get_instance(req.args.id, Camera)
 
     # TODO check camera features / meta if it supports getting color image
     if not camera.color_camera_params:
```

### Comparing `arcor2_arserver-1.0.0/arcor2_arserver/rpc/execution.py` & `arcor2_arserver-1.1.0/arcor2_arserver/rpc/execution.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,17 +22,15 @@
 
         resp = rpc.b.BuildProject.Response()
         resp.data = resp.Data(package_id)
         return resp
 
 
 async def temporary_package_cb(req: rpc.b.TemporaryPackage.Request, ui: WsClient) -> None:
-
     async with glob.LOCK.get_lock():
-
         project = glob.LOCK.project_or_exception()
 
         if project.has_changes:
             raise Arcor2Exception("Project has unsaved changes.")
 
         package_id = await build_and_upload_package(project.id, f"Temporary package for project '{project.name}'.")
```

### Comparing `arcor2_arserver-1.0.0/arcor2_arserver/rpc/lock.py` & `arcor2_arserver-1.1.0/arcor2_arserver/rpc/lock.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,33 +2,28 @@
 
 from arcor2_arserver import globals as glob
 from arcor2_arserver.lock.exceptions import CannotLock
 from arcor2_arserver_data import rpc as srpc
 
 
 async def write_lock_cb(req: srpc.lock.WriteLock.Request, ui: WsClient) -> None:
-
     if not await glob.LOCK.write_lock(req.args.object_id, glob.USERS.user_name(ui), req.args.lock_tree, notify=True):
         raise CannotLock(glob.LOCK.ErrMessages.LOCK_FAIL.value)
 
 
 async def write_unlock_cb(req: srpc.lock.WriteUnlock.Request, ui: WsClient) -> None:
-
     await glob.LOCK.write_unlock(req.args.object_id, glob.USERS.user_name(ui), notify=True)
 
 
 async def read_lock_cb(req: srpc.lock.ReadLock.Request, ui: WsClient) -> None:
-
     # TODO currently unused, maybe delete?
     if not await glob.LOCK.read_lock(req.args.object_id, glob.USERS.user_name(ui)):
         raise CannotLock(glob.LOCK.ErrMessages.LOCK_FAIL.value)
 
 
 async def read_unlock_cb(req: srpc.lock.ReadUnlock.Request, ui: WsClient) -> None:
-
     # TODO currently unused, maybe delete?
     await glob.LOCK.read_unlock(req.args.object_id, glob.USERS.user_name(ui))
 
 
 async def update_lock_cb(req: srpc.lock.UpdateLock.Request, ui: WsClient) -> None:
-
     await glob.LOCK.update_lock(req.args.object_id, glob.USERS.user_name(ui), req.args.new_type)
```

### Comparing `arcor2_arserver-1.0.0/arcor2_arserver/rpc/objects.py` & `arcor2_arserver-1.1.0/arcor2_arserver/rpc/objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 )
 from arcor2_arserver_data import events as sevts
 from arcor2_arserver_data import rpc as srpc
 
 
 @dataclass
 class AimedObject:
-
     obj_id: str
     robot: rpc.common.RobotArg
     poses: dict[int, Pose] = field(default_factory=dict)
 
 
 _objects_being_aimed: dict[str, AimedObject] = {}  # key == user_name
 
@@ -113,15 +112,14 @@
     :return:
     """
 
     to_delete: list[str] = []
 
     # users in db but not holding a lock for the object should be deleted
     for un, fo in _objects_being_aimed.items():
-
         if not await glob.LOCK.is_write_locked(fo.obj_id, un):
             logger.info(f"Object aiming cancelled for {un}.")
             to_delete.append(un)
 
     for td in to_delete:
         _objects_being_aimed.pop(td, None)
 
@@ -163,15 +161,14 @@
     if glob.LOCK.scene:
         logger.info(f"Aiming for {glob.LOCK.scene.object(fo.obj_id).name} cancelled by {user_name}.")
 
 
 async def object_aiming_add_point_cb(
     req: srpc.o.ObjectAimingAddPoint.Request, ui: WsClient
 ) -> srpc.o.ObjectAimingAddPoint.Response:
-
     scene = glob.LOCK.scene_or_exception()
     fo, user_name = await object_aiming_check(ui)
 
     pt_idx = req.args.point_idx
     scene_obj = scene.object(fo.obj_id)
     obj_type = glob.OBJECT_TYPES[scene_obj.type].meta
 
@@ -236,15 +233,14 @@
     if req.dry_run:
         return
 
     fp: list[Position] = []
     rp: list[Position] = []
 
     for idx, pose in fo.poses.items():
-
         fp.append(focus_points[idx].position)
         rp.append(pose.position)
 
     mfa = MeshFocusAction(fp, rp)
 
     logger.debug(f"Attempt to aim object {obj_inst.name}, data: {mfa}")
 
@@ -258,15 +254,14 @@
 
     _objects_being_aimed.pop(user_name, None)
     asyncio.create_task(update_scene_object_pose(scene, obj, new_pose, obj_inst))
     return None
 
 
 async def new_object_type_cb(req: srpc.o.NewObjectType.Request, ui: WsClient) -> None:
-
     async with ctx_write_lock(glob.LOCK.SpecialValues.ADDING_OBJECT, glob.USERS.user_name(ui)):
         meta = req.args
 
         if meta.type in glob.OBJECT_TYPES:
             raise Arcor2Exception("Object type already exists.")
 
         hlp.is_valid_type(meta.type)
@@ -324,15 +319,14 @@
         evt = sevts.o.ChangedObjectTypes([meta])
         evt.change_type = events.Event.Type.ADD
         asyncio.ensure_future(notif.broadcast_event(evt))
         return None
 
 
 async def update_object_model_cb(req: srpc.o.UpdateObjectModel.Request, ui: WsClient) -> None:
-
     can_modify_scene()
     glob.LOCK.scene_or_exception(True)  # only allow while editing scene
 
     obj_data = glob.OBJECT_TYPES[req.args.object_type_id]
 
     if not obj_data.type_def:
         raise Arcor2Exception("ObjectType disabled.")
@@ -369,35 +363,32 @@
 
 
 async def get_object_types_cb(req: srpc.o.GetObjectTypes.Request, ui: WsClient) -> srpc.o.GetObjectTypes.Response:
     return srpc.o.GetObjectTypes.Response(data=[obj.meta for obj in glob.OBJECT_TYPES.values()])
 
 
 def check_scene_for_object_type(scene: CachedScene, object_type: str) -> None:
-
     if object_type in scene.object_types:
         raise Arcor2Exception(f"Used in scene {scene.name}.")
 
 
 async def delete_object_type_cb(
     req: srpc.o.DeleteObjectTypes.Request, ui: WsClient
 ) -> srpc.o.DeleteObjectTypes.Response:
     async def _delete_model(obj_type: ObjectTypeData) -> None:
-
         # do not care so much if delete_model fails
         if not obj_type.meta.object_model:
             return
 
         try:
             await storage.delete_model(obj_type.meta.object_model.model().id)
         except storage.ProjectServiceException as e:
             logger.error(str(e))
 
     async def _delete_ot(ot: str) -> None:
-
         obj_type = glob.OBJECT_TYPES[ot]
 
         if obj_type.meta.built_in:
             raise Arcor2Exception("Can't delete built-in type.")
 
         for obj in glob.OBJECT_TYPES.values():
             if obj.meta.base == ot:
@@ -429,15 +420,14 @@
         else [obj.meta.type for obj in glob.OBJECT_TYPES.values() if not obj.meta.built_in]
     )
 
     response = srpc.o.DeleteObjectTypes.Response()
     response.data = []
 
     async with ctx_write_lock(obj_types_to_delete, user_name, auto_unlock=False, dry_run=req.dry_run):
-
         res = await asyncio.gather(*[_delete_ot(ot) for ot in obj_types_to_delete], return_exceptions=True)
 
         for idx, r in enumerate(res):
             if isinstance(r, Arcor2Exception):
                 response.data.append(srpc.o.DeleteObjectTypes.Response.Data(obj_types_to_delete[idx], str(r)))
             else:
                 assert r is None
@@ -452,15 +442,14 @@
 
     return response
 
 
 def check_override(
     scene: CachedScene, project: CachedProject, obj_id: str, override: Parameter, add_new_one: bool = False
 ) -> SceneObject:
-
     obj = scene.object(obj_id)
 
     for par in glob.OBJECT_TYPES[obj.type].meta.settings:
         if par.name == override.name:
             if par.type != override.type:
                 raise Arcor2Exception("Override can't change parameter type.")
             break
@@ -484,15 +473,14 @@
         else:
             raise Arcor2Exception("Override not found.")
 
     return obj
 
 
 async def add_override_cb(req: srpc.o.AddOverride.Request, ui: WsClient) -> None:
-
     scene = glob.LOCK.scene_or_exception()
     project = glob.LOCK.project_or_exception()
 
     obj = check_override(scene, project, req.args.id, req.args.override, add_new_one=True)
 
     await ensure_write_locked(req.args.id, glob.USERS.user_name(ui))
 
@@ -508,15 +496,14 @@
     evt = sevts.o.OverrideUpdated(req.args.override)
     evt.change_type = events.Event.Type.ADD
     evt.parent_id = req.args.id
     asyncio.ensure_future(notif.broadcast_event(evt))
 
 
 async def update_override_cb(req: srpc.o.UpdateOverride.Request, ui: WsClient) -> None:
-
     scene = glob.LOCK.scene_or_exception()
     project = glob.LOCK.project_or_exception()
 
     obj = check_override(scene, project, req.args.id, req.args.override)
 
     await ensure_write_locked(req.args.id, glob.USERS.user_name(ui))
 
@@ -531,15 +518,14 @@
     evt = sevts.o.OverrideUpdated(req.args.override)
     evt.change_type = events.Event.Type.UPDATE
     evt.parent_id = req.args.id
     asyncio.ensure_future(notif.broadcast_event(evt))
 
 
 async def delete_override_cb(req: srpc.o.DeleteOverride.Request, ui: WsClient) -> None:
-
     scene = glob.LOCK.scene_or_exception()
     project = glob.LOCK.project_or_exception()
 
     obj = check_override(scene, project, req.args.id, req.args.override)
 
     await ensure_write_locked(req.args.id, glob.USERS.user_name(ui))
 
@@ -556,15 +542,14 @@
     evt = sevts.o.OverrideUpdated(req.args.override)
     evt.change_type = events.Event.Type.REMOVE
     evt.parent_id = req.args.id
     asyncio.ensure_future(notif.broadcast_event(evt))
 
 
 async def object_type_usage_cb(req: srpc.o.ObjectTypeUsage.Request, ui: WsClient) -> srpc.o.ObjectTypeUsage.Response:
-
     resp = srpc.o.ObjectTypeUsage.Response()
     resp.data = set()  # mypy does not recognize it correctly with Response(data=set())
 
     async for scene in scenes():
         if req.args.id in scene.object_types:
             resp.data.add(scene.id)
```

### Comparing `arcor2_arserver-1.0.0/arcor2_arserver/rpc/project.py` & `arcor2_arserver-1.1.0/arcor2_arserver/rpc/project.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,15 +51,14 @@
 )
 from arcor2_arserver_data import events as sevts
 from arcor2_arserver_data import rpc as srpc
 
 
 @asynccontextmanager
 async def managed_project(project_id: str, make_copy: bool = False) -> AsyncGenerator[UpdateableCachedProject, None]:
-
     save_back = False
 
     if glob.LOCK.project and glob.LOCK.project.id == project_id:
         if make_copy:
             project = copy.deepcopy(glob.LOCK.project)
             save_back = True
         else:
@@ -75,15 +74,14 @@
         yield project
     finally:
         if save_back:
             asyncio.ensure_future(storage.update_project(project))
 
 
 async def cancel_action_cb(req: srpc.p.CancelAction.Request, ui: WsClient) -> None:
-
     scene = glob.LOCK.scene_or_exception()
     proj = glob.LOCK.project_or_exception()
 
     if not glob.RUNNING_ACTION:
         raise Arcor2Exception("No action is running.")
 
     action = proj.action(glob.RUNNING_ACTION)
@@ -118,38 +116,34 @@
 
     asyncio.ensure_future(notif.broadcast_event(sevts.a.ActionCancelled()))
     glob.RUNNING_ACTION = None
     glob.RUNNING_ACTION_PARAMS = None
 
 
 async def execute_action_cb(req: srpc.p.ExecuteAction.Request, ui: WsClient) -> None:
-
     scene = glob.LOCK.scene_or_exception()
     proj = glob.LOCK.project_or_exception()
 
     # TODO rather lock the project and release the lock once execution is finished?
     async with ctx_write_lock(glob.LOCK.SpecialValues.RUNNING_ACTION, glob.USERS.user_name(ui)):
-
         ensure_scene_started()
 
         if glob.RUNNING_ACTION:
             raise Arcor2Exception(
                 f"Action {glob.RUNNING_ACTION} is being executed. " f"Only one action can be executed at a time."
             )
 
         action = proj.action(req.args.action_id)
 
         obj_id, action_name = action.parse_type()
 
         params: list[Any] = []
 
         for param in action.parameters:
-
             if param.type == common.ActionParameter.TypeEnum.LINK:
-
                 parsed_link = param.parse_link()
                 try:
                     results = glob.PREV_RESULTS[parsed_link.action_id]
                 except KeyError:
                     prev_action = proj.action(parsed_link.action_id)
                     raise Arcor2Exception(f"Action '{prev_action.name}' has to be executed first.")
 
@@ -163,15 +157,14 @@
             elif param.type == common.ActionParameter.TypeEnum.PROJECT_PARAMETER:
                 pparam = proj.parameter(param.str_from_value())
                 # TODO use plugin to get the value
                 from arcor2 import json
 
                 params.append(json.loads(pparam.value))
             else:
-
                 try:
                     params.append(
                         plugin_from_type_name(param.type).parameter_execution_value(
                             get_types_dict(), scene, proj, action.id, param.name
                         )
                     )
                 except ParameterPluginException as e:
@@ -198,15 +191,14 @@
         # schedule execution and return success
         asyncio.ensure_future(project.execute_action(getattr(obj, action_name), params))
         return None
 
 
 async def list_projects_cb(req: srpc.p.ListProjects.Request, ui: WsClient) -> srpc.p.ListProjects.Response:
     async def project_info(project_id: str) -> srpc.p.ListProjects.Response.Data:
-
         project = await storage.get_project(project_id)
 
         assert project.created
         assert project.modified
 
         pd = srpc.p.ListProjects.Response.Data(
             project.name,
@@ -229,33 +221,30 @@
 
     resp = srpc.p.ListProjects.Response()
 
     resp.data = []
     for res in await asyncio.gather(
         *[project_info(proj_id) for proj_id in (await storage.get_project_ids())], return_exceptions=True
     ):
-
         if isinstance(res, Arcor2Exception):
             logger.error(str(res))
         elif isinstance(res, Exception):
             raise res  # zero toleration for other exceptions
         else:
             resp.data.append(res)
 
     return resp
 
 
 async def get_project_cb(req: srpc.p.GetProject.Request, ui: WsClient) -> srpc.p.GetProject.Response:
-
     return srpc.p.GetProject.Response(data=(await storage.get_project(req.args.id)).project)
 
 
 async def add_ap_using_robot_cb(req: srpc.p.AddApUsingRobot.Request, ui: WsClient) -> None:
     async def notify(ap: common.BareActionPoint, ori: common.NamedOrientation, joi: common.ProjectRobotJoints) -> None:
-
         ap_evt = sevts.p.ActionPointChanged(ap)
         ap_evt.change_type = Event.Type.ADD
         await notif.broadcast_event(ap_evt)
 
         ori_evt = sevts.p.OrientationChanged(ori)
         ori_evt.change_type = Event.Type.ADD
         ori_evt.parent_id = ap.id
@@ -266,15 +255,14 @@
 
         await asyncio.gather(notif.broadcast_event(ori_evt), notif.broadcast_event(joi_evt))
 
     hlp.is_valid_identifier(req.args.name)
     proj = glob.LOCK.project_or_exception()
 
     async with ctx_read_lock(req.args.robot_id, glob.USERS.user_name(ui)):
-
         ensure_scene_started()
 
         unique_name(req.args.name, proj.action_points_names)
 
         robot_inst = get_robot_instance(req.args.robot_id)
         await check_eef_arm(robot_inst, req.args.arm_id, req.args.end_effector_id)
 
@@ -294,20 +282,18 @@
         asyncio.ensure_future(notify(ap, ori, joi))
         return None
 
 
 async def add_action_point_joints_using_robot_cb(
     req: srpc.p.AddActionPointJointsUsingRobot.Request, ui: WsClient
 ) -> None:
-
     hlp.is_valid_identifier(req.args.name)
     proj = glob.LOCK.project_or_exception()
 
     async with ctx_read_lock(req.args.robot_id, glob.USERS.user_name(ui)):
-
         ensure_scene_started()
 
         robot_inst = get_robot_instance(req.args.robot_id)
         await check_eef_arm(robot_inst, req.args.arm_id)
 
         ap = proj.bare_action_point(req.args.action_point_id)
 
@@ -331,15 +317,14 @@
         asyncio.ensure_future(notif.broadcast_event(evt))
         return None
 
 
 async def update_action_point_joints_using_robot_cb(
     req: srpc.p.UpdateActionPointJointsUsingRobot.Request, ui: WsClient
 ) -> None:
-
     proj = glob.LOCK.project_or_exception()
 
     ensure_scene_started()
 
     ap, robot_joints = proj.ap_and_joints(req.args.joints_id)
 
     user_name = glob.USERS.user_name(ui)
@@ -355,15 +340,14 @@
         evt = sevts.p.JointsChanged(robot_joints)
         evt.change_type = Event.Type.UPDATE
         asyncio.ensure_future(notif.broadcast_event(evt))
         return None
 
 
 async def update_action_point_joints_cb(req: srpc.p.UpdateActionPointJoints.Request, ui: WsClient) -> None:
-
     proj = glob.LOCK.project_or_exception()
 
     ap, robot_joints = proj.ap_and_joints(req.args.joints_id)
 
     if {joint.name for joint in req.args.joints} != {joint.name for joint in robot_joints.joints}:
         raise Arcor2Exception("Joint names does not match the robot.")
 
@@ -404,15 +388,14 @@
     evt = sevts.p.JointsChanged(joints_to_be_removed)
     evt.change_type = Event.Type.REMOVE
     asyncio.ensure_future(notif.broadcast_event(evt))
     return None
 
 
 async def rename_action_point_cb(req: srpc.p.RenameActionPoint.Request, ui: WsClient) -> None:
-
     proj = glob.LOCK.project_or_exception()
 
     ap = proj.bare_action_point(req.args.action_point_id)
 
     if req.args.new_name == ap.name:
         raise Arcor2Exception("Name unchanged")
 
@@ -435,20 +418,18 @@
     evt.change_type = Event.Type.UPDATE_BASE
     asyncio.ensure_future(notif.broadcast_event(evt))
 
     return None
 
 
 def detect_ap_loop(proj: CachedProject, ap: common.BareActionPoint, new_parent_id: str) -> None:
-
     visited_ids: set[str] = set()
     ap = copy.deepcopy(ap)
     ap.parent = new_parent_id
     while True:
-
         if ap.id in visited_ids:
             raise Arcor2Exception("Loop detected!")
 
         visited_ids.add(ap.id)
 
         if ap.parent is None:
             break  # type: ignore  # this is certainly reachable
@@ -456,15 +437,14 @@
         try:
             ap = proj.bare_action_point(ap.parent)
         except Arcor2Exception:
             break
 
 
 async def update_action_point_parent_cb(req: srpc.p.UpdateActionPointParent.Request, ui: WsClient) -> None:
-
     scene = glob.LOCK.scene_or_exception()
     proj = glob.LOCK.project_or_exception()
     user_name = glob.USERS.user_name(ui)
     ap = proj.bare_action_point(req.args.action_point_id)
 
     # some super basic checks (not involving other objects) are performed before locking anything
     if req.args.new_parent_id == ap.parent:
@@ -474,15 +454,14 @@
         raise Arcor2Exception("AP can't be its own parent.")
 
     to_lock = await get_unlocked_objects(ap.parent, user_name) if ap.parent else set()
     if req.args.new_parent_id:
         to_lock.add(req.args.new_parent_id)
 
     async with ctx_write_lock(to_lock, user_name):
-
         check_ap_parent(scene, proj, req.args.new_parent_id)
         detect_ap_loop(proj, ap, req.args.new_parent_id)
 
         await ensure_write_locked(ap.id, user_name)  # TODO should require locked tree?
 
         if req.dry_run:
             return
@@ -495,15 +474,14 @@
             # AP position and all orientations will become relative to the parent
             updated_aps = tr.make_global_ap_relative(scene, proj, ap, req.args.new_parent_id)
 
         elif ap.parent and not req.args.new_parent_id:
             # AP position and all orientations will become absolute
             updated_aps = tr.make_relative_ap_global(scene, proj, ap)
         else:
-
             assert ap.parent
             # AP position and all orientations will become relative to another parent
             _updated_aps = tr.make_relative_ap_global(scene, proj, ap)
             updated_aps = tr.make_global_ap_relative(scene, proj, ap, req.args.new_parent_id)
 
             updated_aps = set.union(updated_aps, _updated_aps)
 
@@ -545,29 +523,27 @@
     :return:
     """
 
     valid_joints = [joints for joints in proj.ap_joints(ap.id) if joints.is_valid]
     proj.update_ap_position(ap.id, position)
 
     for joints in valid_joints:  # those are now invalid, so let's notify UI about the change
-
         assert not joints.is_valid
 
         evt = sevts.p.JointsChanged(joints)
         evt.change_type = Event.Type.UPDATE
         evt.parent_id = ap.id
         asyncio.ensure_future(notif.broadcast_event(evt))
 
     ap_evt = sevts.p.ActionPointChanged(ap)
     ap_evt.change_type = Event.Type.UPDATE_BASE
     asyncio.ensure_future(notif.broadcast_event(ap_evt))
 
 
 async def update_action_point_position_cb(req: srpc.p.UpdateActionPointPosition.Request, ui: WsClient) -> None:
-
     proj = glob.LOCK.project_or_exception()
     ap = proj.bare_action_point(req.args.action_point_id)
     user_name = glob.USERS.user_name(ui)
 
     if req.dry_run:
         await glob.LOCK.check_lock_tree(req.args.action_point_id, user_name)
     else:
@@ -576,15 +552,14 @@
     if req.dry_run:
         return
 
     await update_ap_position(proj, ap, req.args.new_position)
 
 
 async def update_action_point_using_robot_cb(req: srpc.p.UpdateActionPointUsingRobot.Request, ui: WsClient) -> None:
-
     scene = glob.LOCK.scene_or_exception()
     proj = glob.LOCK.project_or_exception()
     ensure_scene_started()
     user_name = glob.USERS.user_name(ui)
 
     ap = proj.bare_action_point(req.args.action_point_id)
     await ensure_write_locked(ap.id, user_name)
@@ -660,15 +635,14 @@
     """
 
     scene = glob.LOCK.scene_or_exception()
     proj = glob.LOCK.project_or_exception()
     user_name = glob.USERS.user_name(ui)
 
     async with ctx_read_lock(req.args.robot.robot_id, user_name):
-
         ensure_scene_started()
 
         ap = proj.bare_action_point(req.args.action_point_id)
         hlp.is_valid_identifier(req.args.name)
         unique_name(req.args.name, proj.ap_orientation_names(ap.id))
         robot_inst = get_robot_instance(req.args.robot.robot_id)
         await check_eef_arm(robot_inst, req.args.robot.arm_id, req.args.robot.end_effector)
@@ -703,15 +677,14 @@
     """
 
     scene = glob.LOCK.scene_or_exception()
     proj = glob.LOCK.project_or_exception()
     user_name = glob.USERS.user_name(ui)
 
     async with ctx_read_lock(req.args.robot.robot_id, user_name):
-
         ensure_scene_started()
         robot_inst = get_robot_instance(req.args.robot.robot_id)
         await check_eef_arm(robot_inst, req.args.robot.arm_id, req.args.robot.end_effector)
 
         ap, ori = proj.bare_ap_and_orientation(req.args.orientation_id)
 
         await ensure_write_locked(ori.id, user_name)
@@ -770,15 +743,14 @@
 
     :param req:
     :param ui:
     :return:
     """
 
     async with glob.LOCK.get_lock():
-
         if glob.PACKAGE_STATE.state in PackageState.RUN_STATES:
             raise Arcor2Exception("Can't open project while package runs.")
 
         await open_project(req.args.id)
 
         assert glob.LOCK.scene
         assert glob.LOCK.project
@@ -789,17 +761,15 @@
             )
         )
 
         return None
 
 
 async def save_project_cb(req: srpc.p.SaveProject.Request, ui: WsClient) -> None:
-
     async with glob.LOCK.get_lock(req.dry_run):
-
         proj = glob.LOCK.project_or_exception()
 
         if proj.modified and not proj.has_changes:
             raise Arcor2Exception("No changes to save.")
 
         if req.dry_run:
             return None
@@ -812,15 +782,14 @@
         logger.info(f"Updating the project took {time.monotonic()-start:.3f}s.")
 
     asyncio.ensure_future(notif.broadcast_event(sevts.p.ProjectSaved()))
     return None
 
 
 async def new_project_cb(req: srpc.p.NewProject.Request, ui: WsClient) -> None:
-
     if glob.LOCK.project:
         raise Arcor2Exception("Project has to be closed first.")
 
     async with ctx_write_lock(glob.LOCK.SpecialValues.PROJECT, glob.USERS.user_name(ui), dry_run=req.dry_run):
         if glob.PACKAGE_STATE.state in PackageState.RUN_STATES:
             raise Arcor2Exception("Can't create project while package runs.")
 
@@ -843,15 +812,14 @@
             # TODO workaround for https://gitlab.com/kinalisoft/test-it-off/project/-/issues/16
             if req.args.name == glob.LOCK.scene.name:
                 raise Arcor2Exception("A project can't have the same name as the scene.")
 
             if glob.LOCK.scene.has_changes:
                 await save_scene()
         else:
-
             if req.args.scene_id not in (await storage.get_scene_ids()):
                 raise Arcor2Exception("Unknown scene id.")
 
             await open_scene(req.args.scene_id)
 
         glob.PREV_RESULTS.clear()
         glob.LOCK.project = UpdateableCachedProject(
@@ -877,37 +845,33 @@
                 sevts.p.OpenProject(sevts.p.OpenProject.Data(glob.LOCK.scene.scene, glob.LOCK.project.project))
             )
         )
         return None
 
 
 async def close_project_cb(req: srpc.p.CloseProject.Request, ui: WsClient) -> None:
-
     async with glob.LOCK.get_lock(req.dry_run):
-
         proj = glob.LOCK.project_or_exception()
         can_modify_scene()
 
         if not req.args.force and proj.has_changes:
             raise Arcor2Exception("Project has unsaved changes.")
 
         if req.dry_run:
             return None
 
         await close_project()
         return None
 
 
 async def add_action_point_cb(req: srpc.p.AddActionPoint.Request, ui: WsClient) -> None:
-
     scene = glob.LOCK.scene_or_exception()
     proj = glob.LOCK.project_or_exception()
 
     async with ctx_write_lock(glob.LOCK.SpecialValues.PROJECT, glob.USERS.user_name(ui)):
-
         hlp.is_valid_identifier(req.args.name)
         unique_name(req.args.name, proj.action_points_names)
         check_ap_parent(scene, proj, req.args.parent)
 
         if req.dry_run:
             return None
 
@@ -916,21 +880,19 @@
         evt = sevts.p.ActionPointChanged(ap)
         evt.change_type = Event.Type.ADD
         asyncio.ensure_future(notif.broadcast_event(evt))
         return None
 
 
 async def remove_action_point_cb(req: srpc.p.RemoveActionPoint.Request, ui: WsClient) -> None:
-
     proj = glob.LOCK.project_or_exception()
 
     user_name = glob.USERS.user_name(ui)
     to_lock = await get_unlocked_objects(req.args.id, user_name)
     async with ctx_write_lock(to_lock, user_name, auto_unlock=req.dry_run):
-
         ap = proj.bare_action_point(req.args.id)
 
         for proj_ap in proj.action_points_with_parent:
             if proj_ap.parent == ap.id:
                 raise Arcor2Exception(f"Can't remove parent of '{proj_ap.name}' AP.")
 
         ap_action_ids = proj.ap_action_ids(ap.id)
@@ -942,15 +904,14 @@
                 logic.start in ap_action_ids
                 or logic.end in ap_action_ids
                 or (logic.condition and logic.condition.parse_what().action_id in ap_action_ids)
             ):
                 raise Arcor2Exception("Remove logic connections first.")
 
         for act in proj.actions:
-
             if act.id in ap_action_ids:
                 continue
 
             for param in act.parameters:
                 if param.type == common.ActionParameter.TypeEnum.LINK:
                     parsed_link = param.parse_link()
                     linking_action = proj.action(parsed_link.action_id)
@@ -987,51 +948,47 @@
         evt = sevts.p.ActionPointChanged(ap)
         evt.change_type = Event.Type.REMOVE
         asyncio.ensure_future(notif.broadcast_event(evt))
         return None
 
 
 async def copy_action_point_cb(req: srpc.p.CopyActionPoint.Request, ui: WsClient) -> None:
-
     proj = glob.LOCK.project_or_exception()
 
     async def copy_action_point(
         orig_ap: common.BareActionPoint,
         new_parent_id: None | str = None,
         position: None | common.Position = None,
     ) -> None:
-
         assert await glob.LOCK.is_read_locked(orig_ap.id, user_name)
 
         ap = proj.upsert_action_point(
             common.ActionPoint.uid(),
             make_name_unique(f"{orig_ap.name}_copy", proj.action_points_names),
             orig_ap.position if position is None else position,
             orig_ap.parent if new_parent_id is None else new_parent_id,
         )
 
         ap_added_evt = sevts.p.ActionPointChanged(ap)
         ap_added_evt.change_type = Event.Type.ADD
         await notif.broadcast_event(ap_added_evt)
 
         for ori in proj.ap_orientations(orig_ap.id):
-
             assert await glob.LOCK.is_read_locked(ori.id, user_name)
 
             new_ori = ori.copy()
             old_ori_to_new_ori[ori.id] = new_ori.id
             proj.upsert_orientation(ap.id, new_ori)
 
             ori_added_evt = sevts.p.OrientationChanged(new_ori)
             ori_added_evt.change_type = Event.Type.ADD
             ori_added_evt.parent_id = ap.id
             await notif.broadcast_event(ori_added_evt)
 
         for joints in proj.ap_joints(orig_ap.id):
-
             assert await glob.LOCK.is_read_locked(joints.id, user_name)
 
             new_joints = joints.copy()
             proj.upsert_joints(ap.id, new_joints)
 
             joints_added_evt = sevts.p.JointsChanged(new_joints)
             joints_added_evt.change_type = Event.Type.ADD
@@ -1056,15 +1013,14 @@
             ]
         )
 
     user_name = glob.USERS.user_name(ui)
     childs_of_original_ap = glob.LOCK.get_all_children(req.args.id)
 
     async with ctx_read_lock(childs_of_original_ap | {req.args.id}, user_name):
-
         # filter out only APs
         child_aps = {ch for ch in childs_of_original_ap if ch in proj.action_points_ids} | {req.args.id}
         logger.debug(f"Child action points of the original AP: {child_aps}")
 
         original_ap = proj.bare_action_point(req.args.id)
 
         if req.dry_run:
@@ -1072,19 +1028,17 @@
 
         old_ori_to_new_ori: dict[str, str] = {}
         new_action_ids: set[str] = set()
         # let's do it within the RPC, should not take long time...
         await copy_action_point(original_ap, position=req.args.position)
 
         for act_id in new_action_ids:  # this has to be done once old_ori_to_new_ori is complete
-
             ap, new_act = proj.action_point_and_action(act_id)
 
             for param in new_act.parameters:
-
                 if param.type != PosePlugin.type_name():  # TODO also handle joints and positions!
                     continue
 
                 old_ori = proj.bare_ap_and_orientation(PosePlugin.orientation_id(proj, new_act.id, param.name))[1]
                 child_orientations = {ori.id for ap_id in child_aps for ori in proj.ap_orientations(ap_id)}
                 logger.debug(f"Child orientations of the original AP: {child_orientations}")
 
@@ -1150,15 +1104,14 @@
         evt.change_type = Event.Type.ADD
         evt.parent_id = ap.id
         asyncio.ensure_future(notif.broadcast_event(evt))
         return None
 
 
 async def update_action_cb(req: srpc.p.UpdateAction.Request, ui: WsClient) -> None:
-
     scene = glob.LOCK.scene_or_exception()
     proj = glob.LOCK.project_or_exception()
 
     updated_project = copy.deepcopy(proj)
 
     updated_action = updated_project.action(req.args.action_id)
 
@@ -1185,40 +1138,37 @@
     evt.change_type = Event.Type.UPDATE
     asyncio.ensure_future(notif.broadcast_event(evt))
     return None
 
 
 async def remove_action_cb(req: srpc.p.RemoveAction.Request, ui: WsClient) -> None:
     def check_action_usage(proj: CachedProject, action: common.Action) -> None:
-
         # check parameters
         for act in proj.actions:
             for param in act.parameters:
                 if param.type == common.ActionParameter.TypeEnum.LINK:
                     link = param.parse_link()
                     if action.id == link.action_id:
                         raise Arcor2Exception(f"Action output used as parameter of {act.name}/{param.name}.")
 
         # check logic
         for log in proj.logic:
-
             if log.start == action.id or log.end == action.id:
                 raise Arcor2Exception("Action used in logic.")
 
             if log.condition:
                 action_id, _, _ = log.condition.what.split("/")
 
                 if action_id == action.id:
                     raise Arcor2Exception("Action used in condition.")
 
     proj = glob.LOCK.project_or_exception()
     user_name = glob.USERS.user_name(ui)
     to_lock = await get_unlocked_objects(req.args.id, user_name)
     async with ctx_write_lock(to_lock, user_name, auto_unlock=req.dry_run):
-
         ap, action = proj.action_point_and_action(req.args.id)
         check_action_usage(proj, action)
 
         if req.dry_run:
             return None
 
         await glob.LOCK.write_unlock(req.args.id, user_name)
@@ -1229,15 +1179,14 @@
         evt = sevts.p.ActionChanged(action.bare)
         evt.change_type = Event.Type.REMOVE
         asyncio.ensure_future(notif.broadcast_event(evt))
         return None
 
 
 async def add_logic_item_cb(req: srpc.p.AddLogicItem.Request, ui: WsClient) -> None:
-
     scene = glob.LOCK.scene_or_exception()
     proj = glob.LOCK.project_or_exception(must_have_logic=True)
     user_name = glob.USERS.user_name(ui)
 
     to_lock = await get_unlocked_objects([req.args.start, req.args.end], user_name)
     async with ctx_write_lock(to_lock, user_name):
         logic_item = common.LogicItem(req.args.start, req.args.end, req.args.condition)
@@ -1289,15 +1238,14 @@
     evt = sevts.p.LogicItemChanged(updated_logic_item)
     evt.change_type = Event.Type.UPDATE
     asyncio.ensure_future(notif.broadcast_event(evt))
     return None
 
 
 async def remove_logic_item_cb(req: srpc.p.RemoveLogicItem.Request, ui: WsClient) -> None:
-
     proj = glob.LOCK.project_or_exception(must_have_logic=True)
     logic_item = proj.logic_item(req.args.logic_item_id)
 
     user_name = glob.USERS.user_name(ui)
     to_lock = await get_unlocked_objects([logic_item.start, logic_item.end], user_name)
     async with ctx_write_lock(to_lock, user_name):
         # TODO is it necessary to check something here?
@@ -1310,19 +1258,17 @@
     await glob.LOCK.write_unlock(
         [item for item in (logic_item.start, logic_item.end) if item not in to_lock], user_name, True
     )
     return None
 
 
 async def add_project_parameter_cb(req: srpc.p.AddProjectParameter.Request, ui: WsClient) -> None:
-
     proj = glob.LOCK.project_or_exception()
 
     async with ctx_write_lock(glob.LOCK.SpecialValues.PROJECT, glob.USERS.user_name(ui)):
-
         pparam = common.ProjectParameter(req.args.name, req.args.type, req.args.value)
         check_project_parameter(proj, pparam)
 
         if req.dry_run:
             return
 
         proj.upsert_parameter(pparam)
@@ -1330,15 +1276,14 @@
         evt = sevts.p.ProjectParameterChanged(pparam)
         evt.change_type = Event.Type.ADD
         asyncio.ensure_future(notif.broadcast_event(evt))
         return None
 
 
 async def update_project_parameter_cb(req: srpc.p.UpdateProjectParameter.Request, ui: WsClient) -> None:
-
     proj = glob.LOCK.project_or_exception()
     param = proj.parameter(req.args.id)
     user_name = glob.USERS.user_name(ui)
 
     await ensure_write_locked(req.args.id, user_name)
 
     updated_param = copy.deepcopy(param)
@@ -1359,22 +1304,20 @@
     evt.change_type = Event.Type.UPDATE
     asyncio.create_task(notif.broadcast_event(evt))
 
     await glob.LOCK.write_unlock(param.id, user_name, True)
 
 
 async def remove_project_parameter_cb(req: srpc.p.RemoveProjectParameter.Request, ui: WsClient) -> None:
-
     proj = glob.LOCK.project_or_exception()
     pparam = proj.parameter(req.args.id)
 
     user_name = glob.USERS.user_name(ui)
     to_lock = await get_unlocked_objects(req.args.id, user_name)
     async with ctx_write_lock(to_lock, user_name, auto_unlock=req.dry_run):
-
         # check for usage
         for act in proj.actions:
             for param in act.parameters:
                 if (
                     param.type == common.ActionParameter.TypeEnum.PROJECT_PARAMETER
                     and param.str_from_value() == pparam.id
                 ):
@@ -1389,15 +1332,14 @@
 
         evt = sevts.p.ProjectParameterChanged(pparam)
         evt.change_type = Event.Type.REMOVE
         asyncio.ensure_future(notif.broadcast_event(evt))
 
 
 async def delete_project_cb(req: srpc.p.DeleteProject.Request, ui: WsClient) -> None:
-
     if glob.LOCK.project:
         raise Arcor2Exception("Project has to be closed first.")
 
     user_name = glob.USERS.user_name(ui)
 
     async with ctx_write_lock(req.args.id, user_name, auto_unlock=False):
         project = await storage.get_project(req.args.id)
@@ -1407,78 +1349,70 @@
         evt = sevts.p.ProjectChanged(project.bare)
         evt.change_type = Event.Type.REMOVE
         asyncio.ensure_future(notif.broadcast_event(evt))
         return None
 
 
 async def rename_project_cb(req: srpc.p.RenameProject.Request, ui: WsClient) -> None:
-
     unique_name(req.args.new_name, (await project_names()))
 
     # TODO workaround for https://gitlab.com/kinalisoft/test-it-off/project/-/issues/16
     unique_name(req.args.new_name, (await scene_names()))
 
     user_name = glob.USERS.user_name(ui)
 
     await ensure_write_locked(req.args.project_id, user_name)
 
     if req.dry_run:
         return None
 
     async with managed_project(req.args.project_id) as project:
-
         project.name = req.args.new_name
         project.update_modified()
 
         evt = sevts.p.ProjectChanged(project.bare)
         evt.change_type = Event.Type.UPDATE_BASE
         asyncio.ensure_future(notif.broadcast_event(evt))
 
     await glob.LOCK.write_unlock(req.args.project_id, user_name)
     return None
 
 
 async def copy_project_cb(req: srpc.p.CopyProject.Request, ui: WsClient) -> None:
-
     async with ctx_write_lock(req.args.source_id, glob.USERS.user_name(ui)):
         unique_name(req.args.target_name, (await project_names()))
 
         if req.dry_run:
             return None
 
         async with managed_project(req.args.source_id, make_copy=True) as project:
-
             project.name = req.args.target_name
 
             evt = sevts.p.ProjectChanged(project.bare)
             evt.change_type = Event.Type.UPDATE_BASE
             asyncio.ensure_future(notif.broadcast_event(evt))
 
         return None
 
 
 async def update_project_description_cb(req: srpc.p.UpdateProjectDescription.Request, ui: WsClient) -> None:
-
     async with ctx_write_lock(req.args.project_id, glob.USERS.user_name(ui)):
         async with managed_project(req.args.project_id) as project:
-
             project.description = req.args.new_description
             project.update_modified()
 
             evt = sevts.p.ProjectChanged(project.bare)
             evt.change_type = Event.Type.UPDATE_BASE
             asyncio.ensure_future(notif.broadcast_event(evt))
         return None
 
 
 async def update_project_has_logic_cb(req: srpc.p.UpdateProjectHasLogic.Request, ui: WsClient) -> None:
-
     async with ctx_write_lock(req.args.project_id, glob.USERS.user_name(ui)):
         async with managed_project(req.args.project_id) as project:
-
             if project.has_logic and not req.args.new_has_logic:
                 project.clear_logic()
 
                 """
                 TODO
 
                 if glob.LOCK.project and glob.LOCK.project.id == req.args.project_id:
@@ -1491,15 +1425,14 @@
             evt = sevts.p.ProjectChanged(project.bare)
             evt.change_type = Event.Type.UPDATE_BASE
             asyncio.ensure_future(notif.broadcast_event(evt))
         return None
 
 
 async def rename_action_point_joints_cb(req: srpc.p.RenameActionPointJoints.Request, ui: WsClient) -> None:
-
     proj = glob.LOCK.project_or_exception()
     ap, joints = proj.ap_and_joints(req.args.joints_id)
 
     hlp.is_valid_identifier(req.args.new_name)
     unique_name(req.args.new_name, proj.ap_joint_names(ap.id))
 
     await ensure_write_locked(ap.id, glob.USERS.user_name(ui))
@@ -1514,15 +1447,14 @@
     evt.change_type = Event.Type.UPDATE_BASE
     asyncio.ensure_future(notif.broadcast_event(evt))
 
     return None
 
 
 async def rename_action_point_orientation_cb(req: srpc.p.RenameActionPointOrientation.Request, ui: WsClient) -> None:
-
     proj = glob.LOCK.project_or_exception()
     ap, ori = proj.bare_ap_and_orientation(req.args.orientation_id)
 
     hlp.is_valid_identifier(req.args.new_name)
     unique_name(req.args.new_name, proj.ap_orientation_names(ap.id))
 
     await ensure_write_locked(ori.id, glob.USERS.user_name(ui))
@@ -1537,15 +1469,14 @@
     evt.change_type = Event.Type.UPDATE_BASE
     asyncio.ensure_future(notif.broadcast_event(evt))
 
     return None
 
 
 async def rename_action_cb(req: srpc.p.RenameAction.Request, ui: WsClient) -> None:
-
     proj = glob.LOCK.project_or_exception()
     unique_name(req.args.new_name, proj.action_names)
     user_name = glob.USERS.user_name(ui)
 
     await ensure_write_locked(req.args.action_id, user_name)
 
     if req.dry_run:
```

### Comparing `arcor2_arserver-1.0.0/arcor2_arserver/rpc/robot.py` & `arcor2_arserver-1.1.0/arcor2_arserver/rpc/robot.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,18 +43,16 @@
 EVENT_PERIOD = env.get_float("ARCOR2_STREAMING_PERIOD", 0.1)
 
 if EVENT_PERIOD <= 0:
     EVENT_PERIOD = 0.1
 
 
 async def robot_joints_event(robot_inst: Robot) -> None:
-
     logger.info(f"Sending joints for {robot_inst.name} started.")
     while scene_started() and glob.ROBOT_JOINTS_REGISTERED_UIS[robot_inst.id]:
-
         start = time.monotonic()
 
         try:
             evt = RobotJoints(RobotJoints.Data(robot_inst.id, (await robot.get_robot_joints(robot_inst, None, True))))
         except Arcor2Exception as e:
             logger.error(f"Failed to get joints for {robot_inst.name}. {str(e)}")
             await asyncio.sleep(1)
@@ -73,36 +71,32 @@
     # TODO notify UIs that registration was cancelled
     glob.ROBOT_JOINTS_REGISTERED_UIS.pop(robot_inst.id, None)
 
     logger.info(f"Sending joints for {robot_inst.name} stopped.")
 
 
 async def eef_pose(robot_inst: Robot, eef_id: str, arm_id: None | str = None) -> RobotEef.Data.EefPose:
-
     return RobotEef.Data.EefPose(eef_id, (await robot.get_end_effector_pose(robot_inst, eef_id, arm_id)), arm_id)
 
 
 async def robot_eef_pose_event(robot_inst: Robot) -> None:
-
     eefs: dict[None | str, set[str]] = {}
 
     try:
         try:
             for arm_id in await robot.get_arms(robot_inst):
                 eefs[arm_id] = await robot.get_end_effectors(robot_inst, arm_id)
         except robot.SingleArmRobotException:
             eefs = {None: await robot.get_end_effectors(robot_inst, None)}
     except Arcor2Exception as e:
         logger.error(f"Failed to start sending poses for {robot_inst.name}. {str(e)}")
     else:
-
         logger.info(f"Sending poses for {robot_inst.name} started. Arms/EEFs: {eefs}.")
 
         while scene_started() and glob.ROBOT_EEF_REGISTERED_UIS[robot_inst.id]:
-
             start = time.monotonic()
 
             evt = RobotEef(RobotEef.Data(robot_inst.id))
 
             try:
                 evt.data.end_effectors = await asyncio.gather(
                     *[eef_pose(robot_inst, eef_id, arm_id) for arm_id in eefs.keys() for eef_id in eefs[arm_id]]
@@ -125,79 +119,72 @@
     # TODO notify UIs that registration was cancelled
     glob.ROBOT_EEF_REGISTERED_UIS.pop(robot_inst.id, None)
 
     logger.info(f"Sending poses for {robot_inst.name} stopped.")
 
 
 async def get_robot_meta_cb(req: srpc.r.GetRobotMeta.Request, ui: WsClient) -> srpc.r.GetRobotMeta.Response:
-
     return srpc.r.GetRobotMeta.Response(
         data=[obj.robot_meta for obj in glob.OBJECT_TYPES.values() if obj.robot_meta is not None]
     )
 
 
 async def get_robot_joints_cb(req: srpc.r.GetRobotJoints.Request, ui: WsClient) -> srpc.r.GetRobotJoints.Response:
-
     glob.LOCK.scene_or_exception()
 
     async with ctx_read_lock(req.args.robot_id, glob.USERS.user_name(ui)):
         ensure_scene_started()
         return srpc.r.GetRobotJoints.Response(
             data=await robot.get_robot_joints(get_robot_instance(req.args.robot_id), req.args.arm_id)
         )
 
 
 async def get_end_effector_pose_cb(
     req: srpc.r.GetEndEffectorPose.Request, ui: WsClient
 ) -> srpc.r.GetEndEffectorPose.Response:
-
     glob.LOCK.scene_or_exception()
 
     async with ctx_read_lock(req.args.robot_id, glob.USERS.user_name(ui)):
         ensure_scene_started()
         return srpc.r.GetEndEffectorPose.Response(
             data=await robot.get_end_effector_pose(
                 get_robot_instance(req.args.robot_id), req.args.end_effector_id, req.args.arm_id
             )
         )
 
 
 async def get_end_effectors_cb(req: srpc.r.GetEndEffectors.Request, ui: WsClient) -> srpc.r.GetEndEffectors.Response:
-
     glob.LOCK.scene_or_exception()
 
     async with ctx_read_lock(req.args.robot_id, glob.USERS.user_name(ui)):
         ensure_scene_started()
         return srpc.r.GetEndEffectors.Response(
             data=await robot.get_end_effectors(get_robot_instance(req.args.robot_id), req.args.arm_id)
         )
 
 
 async def get_robot_arms_cb(req: srpc.r.GetRobotArms.Request, ui: WsClient) -> srpc.r.GetRobotArms.Response:
-
     glob.LOCK.scene_or_exception()
 
     async with ctx_read_lock(req.args.robot_id, glob.USERS.user_name(ui)):
         ensure_scene_started()
         return srpc.r.GetRobotArms.Response(data=await robot.get_arms(get_robot_instance(req.args.robot_id)))
 
 
 async def get_grippers_cb(req: srpc.r.GetGrippers.Request, ui: WsClient) -> srpc.r.GetGrippers.Response:
-
     glob.LOCK.scene_or_exception()
 
     async with ctx_read_lock(req.args.robot_id, glob.USERS.user_name(ui)):
         ensure_scene_started()
         return srpc.r.GetGrippers.Response(
             data=await robot.get_grippers(get_robot_instance(req.args.robot_id), req.args.arm_id)
         )
 
 
 async def get_suctions_cb(req: srpc.r.GetSuctions.Request, ui: WsClient) -> srpc.r.GetSuctions.Response:
-
     glob.LOCK.scene_or_exception()
 
     async with ctx_read_lock(req.args.robot_id, glob.USERS.user_name(ui)):
         ensure_scene_started()
         return srpc.r.GetSuctions.Response(
             data=await robot.get_suctions(get_robot_instance(req.args.robot_id), req.args.arm_id)
         )
@@ -207,17 +194,15 @@
     req: srpc.r.RegisterForRobotEvent.Request,
     robot_inst: Robot,
     ui: WsClient,
     tasks: TaskDict,
     reg_uis: glob.RegisteredUiDict,
     coro: Callable[[Robot], Awaitable[None]],
 ) -> None:
-
     if req.args.send:
-
         reg_uis[req.args.robot_id].add(ui)
 
         if req.args.robot_id not in tasks:
             # start task
             tasks[req.args.robot_id] = asyncio.create_task(coro(robot_inst))  # type: ignore   # TODO figure it out
 
     else:
@@ -233,29 +218,27 @@
             if not task.cancelled():
                 task.cancel()
 
             del tasks[req.args.robot_id]
 
 
 async def register_for_robot_event_cb(req: srpc.r.RegisterForRobotEvent.Request, ui: WsClient) -> None:
-
     glob.LOCK.scene_or_exception()
 
     async with ctx_read_lock(req.args.robot_id, glob.USERS.user_name(ui)):
         ensure_scene_started()
 
         # check if robot exists
         robot_inst = get_robot_instance(req.args.robot_id)
 
         if req.args.what == req.args.RegisterEnum.JOINTS:
             await register(
                 req, robot_inst, ui, ROBOT_JOINTS_TASKS, glob.ROBOT_JOINTS_REGISTERED_UIS, robot_joints_event
             )
         elif req.args.what == req.args.RegisterEnum.EEF_POSE:
-
             if isinstance(robot_inst, MultiArmRobot):
                 for arm_id in await robot.get_arms(robot_inst):
                     if await robot.get_end_effectors(robot_inst, arm_id):
                         break
                 else:
                     raise Arcor2Exception("Robot does not have any end effector.")
 
@@ -266,43 +249,40 @@
         else:
             raise Arcor2Exception(f"Option '{req.args.what.value}' not implemented.")
 
         return None
 
 
 async def check_feature(robot_inst: Robot, feature_name: str) -> None:
-
     obj_type = glob.OBJECT_TYPES[robot_inst.__class__.__name__]
 
     if obj_type.robot_meta is None:
         raise Arcor2Exception("Not a robot.")
 
     try:
         if not getattr(obj_type.robot_meta.features, feature_name):
             raise Arcor2Exception(f"Robot does not support '{feature_name}' feature.")
     except AttributeError:
         raise Arcor2Exception(f"Unknown robot feature: {feature_name}.")
 
 
 async def move_to_pose_cb(req: srpc.r.MoveToPose.Request, ui: WsClient) -> None:
-
     glob.LOCK.scene_or_exception()
     user_name = glob.USERS.user_name(ui)
 
     async with ctx_write_lock(req.args.robot_id, user_name, auto_unlock=False):
         ensure_scene_started()
 
         robot_inst = get_robot_instance(req.args.robot_id)
         await robot.check_eef_arm(robot_inst, req.args.arm_id, req.args.end_effector_id)
 
         await check_feature(robot_inst, Robot.move_to_pose.__name__)
         await robot.check_robot_before_move(robot_inst)
 
         if (req.args.position is None) != (req.args.orientation is None):
-
             target_pose = await robot.get_end_effector_pose(robot_inst, req.args.end_effector_id, req.args.arm_id)
 
             if req.args.position:
                 target_pose.position = req.args.position
             elif req.args.orientation:
                 target_pose.orientation = req.args.orientation
 
@@ -323,58 +303,52 @@
                 req.args.linear,
                 user_name,
             )
         )
 
 
 async def move_to_joints_cb(req: srpc.r.MoveToJoints.Request, ui: WsClient) -> None:
-
     glob.LOCK.scene_or_exception()
     user_name = glob.USERS.user_name(ui)
 
     async with ctx_write_lock(req.args.robot_id, user_name, auto_unlock=False):
-
         ensure_scene_started()
         robot_inst = get_robot_instance(req.args.robot_id)
         await check_feature(robot_inst, Robot.move_to_joints.__name__)
         await robot.check_robot_before_move(robot_inst)
 
         asyncio.ensure_future(
             robot.move_to_joints(robot_inst, req.args.joints, req.args.speed, req.args.safe, user_name, req.args.arm_id)
         )
 
 
 async def stop_robot_cb(req: srpc.r.StopRobot.Request, ui: WsClient) -> None:
-
     glob.LOCK.scene_or_exception()
 
     # Stop robot cannot use lock, because robot is locked when action is called. Stop will also release lock.
     ensure_scene_started()
     robot_inst = get_robot_instance(req.args.robot_id)
     await check_feature(robot_inst, Robot.stop.__name__)
     await robot.stop(robot_inst)
 
 
 async def move_to_action_point_cb(req: srpc.r.MoveToActionPoint.Request, ui: WsClient) -> None:
-
     scene = glob.LOCK.scene_or_exception()
     project = glob.LOCK.project_or_exception()
 
     async with ctx_write_lock(req.args.robot_id, glob.USERS.user_name(ui)):
-
         ensure_scene_started()
         robot_inst = get_robot_instance(req.args.robot_id)
 
         await robot.check_robot_before_move(robot_inst)
 
         if (req.args.orientation_id is None) == (req.args.joints_id is None):
             raise Arcor2Exception("Set orientation or joints. Not both.")
 
         if req.args.orientation_id:
-
             await check_feature(robot_inst, Robot.move_to_pose.__name__)
 
             if req.args.end_effector_id is None:
                 raise Arcor2Exception("eef id has to be set.")
 
             pose = tr.abs_pose_from_ap_orientation(scene, project, req.args.orientation_id)
 
@@ -389,34 +363,31 @@
                     req.args.orientation_id,
                     req.args.safe,
                     req.args.linear,
                 )
             )
 
         elif req.args.joints_id:
-
             await check_feature(robot_inst, Robot.move_to_joints.__name__)
 
             # TODO add arm_id to ProjectRobotJoints and use it as a parameter for move_to_ap_joints
             joints = project.joints(req.args.joints_id)
 
             # TODO check if the joints are within limits and reachable (dry_run)
             asyncio.ensure_future(
                 robot.move_to_ap_joints(
                     robot_inst, joints.joints, req.args.speed, req.args.joints_id, req.args.safe, req.args.arm_id
                 )
             )
 
 
 async def ik_cb(req: srpc.r.InverseKinematics.Request, ui: WsClient) -> srpc.r.InverseKinematics.Response:
-
     glob.LOCK.scene_or_exception()
 
     async with ctx_read_lock([req.args.robot_id, req.args.end_effector_id], glob.USERS.user_name(ui)):
-
         ensure_scene_started()
         robot_inst = get_robot_instance(req.args.robot_id)
         await check_feature(robot_inst, Robot.inverse_kinematics.__name__)
 
         joints = await robot.ik(
             robot_inst,
             req.args.end_effector_id,
@@ -427,42 +398,38 @@
         )
         resp = srpc.r.InverseKinematics.Response()
         resp.data = joints
         return resp
 
 
 async def fk_cb(req: srpc.r.ForwardKinematics.Request, ui: WsClient) -> srpc.r.ForwardKinematics.Response:
-
     glob.LOCK.scene_or_exception()
 
     async with ctx_read_lock([req.args.robot_id, req.args.end_effector_id], glob.USERS.user_name(ui)):
-
         ensure_scene_started()
         robot_inst = get_robot_instance(req.args.robot_id)
         await check_feature(robot_inst, Robot.forward_kinematics.__name__)
 
         pose = await robot.fk(robot_inst, req.args.end_effector_id, req.args.arm_id, req.args.joints)
         resp = srpc.r.ForwardKinematics.Response()
         resp.data = pose
         return resp
 
 
 async def calibrate_robot(
     robot_inst: Robot, camera_inst: Camera, move_to_calibration_pose: bool, user_name: str
 ) -> None:
-
     try:
         scene = glob.LOCK.scene_or_exception()
 
         assert camera_inst.color_camera_params
 
         await notif.broadcast_event(ProcessState(ProcessState.Data(RBT_CALIB, ProcessState.Data.StateEnum.Started)))
 
         try:
-
             if move_to_calibration_pose:
                 await run_in_executor(robot_inst.move_to_calibration_pose)
             robot_joints = await run_in_executor(robot_inst.robot_joints)
             depth_image = await run_in_executor(camera_inst.depth_image, 128)
 
             args = CalibrateRobotArgs(
                 robot_joints,
@@ -484,30 +451,28 @@
         await update_scene_object_pose(scene, scene.object(robot_inst.id), new_pose, robot_inst)
         await notif.broadcast_event(ProcessState(ProcessState.Data(RBT_CALIB, ProcessState.Data.StateEnum.Finished)))
     finally:
         await glob.LOCK.write_unlock(camera_inst.id, user_name)
 
 
 async def calibrate_robot_cb(req: srpc.r.CalibrateRobot.Request, ui: WsClient) -> None:
-
     glob.LOCK.scene_or_exception()
     user_name = glob.USERS.user_name(ui)
 
     ensure_scene_started()
 
     if not req.args.camera_id:
         for obj in glob.SCENE_OBJECT_INSTANCES.values():
             if isinstance(obj, Camera):
                 req.args.camera_id = obj.id
                 break
         else:
             raise Arcor2Exception("No camera found.")
 
     async with ctx_write_lock(req.args.camera_id, user_name, auto_unlock=False):
-
         robot_inst = get_robot_instance(req.args.robot_id)
 
         if not robot_inst.urdf_package_name:
             raise Arcor2Exception("Robot with model required!")
 
         camera_inst = get_instance(req.args.camera_id, Camera)
 
@@ -518,15 +483,14 @@
 
         asyncio.ensure_future(calibrate_robot(robot_inst, camera_inst, req.args.move_to_calibration_pose, user_name))
 
         return None
 
 
 async def hand_teaching_mode_cb(req: srpc.r.HandTeachingMode.Request, ui: WsClient) -> None:
-
     glob.LOCK.scene_or_exception()
 
     ensure_scene_started()
     robot_inst = get_robot_instance(req.args.robot_id)
 
     # in this case, method name does not correspond to feature name
     await check_feature(robot_inst, "hand_teaching")
@@ -555,15 +519,14 @@
 
     await run_in_executor(robot_inst.set_hand_teaching_mode, req.args.enable, *params)
     evt = HandTeachingMode(HandTeachingMode.Data(req.args.robot_id, req.args.enable, req.args.arm_id))
     asyncio.ensure_future(notif.broadcast_event(evt))
 
 
 async def step_robot_eef_cb(req: srpc.r.StepRobotEef.Request, ui: WsClient) -> None:
-
     scene = glob.LOCK.scene_or_exception()
 
     ensure_scene_started()
     robot_inst = get_robot_instance(req.args.robot_id)
 
     await check_feature(robot_inst, Robot.move_to_pose.__name__)
     await robot.check_robot_before_move(robot_inst)
@@ -611,15 +574,14 @@
         robot.move_to_pose(
             robot_inst, req.args.end_effector_id, req.args.arm_id, tp, req.args.speed, req.args.safe, req.args.linear
         )
     )
 
 
 async def set_eef_perpendicular_to_world_cb(req: srpc.r.SetEefPerpendicularToWorld.Request, ui: WsClient) -> None:
-
     glob.LOCK.scene_or_exception()
 
     ensure_scene_started()
     robot_inst = get_robot_instance(req.args.robot_id)
 
     await check_feature(robot_inst, Robot.move_to_pose.__name__)
     await check_feature(robot_inst, Robot.inverse_kinematics.__name__)
@@ -648,15 +610,14 @@
     tasks = [
         robot.ik(robot_inst, req.args.end_effector_id, req.args.arm_id, pose, current_joints, req.args.safe)
         for pose in poses
     ]
 
     # order of results from gather corresponds to order of tasks
     for idx, res in enumerate(await asyncio.gather(*tasks, return_exceptions=True)):
-
         if not isinstance(res, list):
             continue
 
         diff = 0.0
 
         for f, b in zip(current_joints, res):
             assert (
```

### Comparing `arcor2_arserver-1.0.0/arcor2_arserver/rpc/scene.py` & `arcor2_arserver-1.1.0/arcor2_arserver/rpc/scene.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,14 @@
 from arcor2_arserver_data import rpc as srpc
 from arcor2_arserver_data.objects import ObjectTypeMeta
 from arcor2_calibration_data import client as calibration
 
 
 @asynccontextmanager
 async def managed_scene(scene_id: str, make_copy: bool = False) -> AsyncGenerator[UpdateableCachedScene, None]:
-
     save_back = False
 
     if glob.LOCK.scene and glob.LOCK.scene.id == scene_id:
         if make_copy:
             scene = copy.deepcopy(glob.LOCK.scene)
             save_back = True
         else:
@@ -131,15 +130,14 @@
     """Closes scene on the server.
 
     :param req:
     :return:
     """
 
     async with ctx_write_lock(glob.LOCK.SpecialValues.SCENE, glob.USERS.user_name(ui), dry_run=req.dry_run):
-
         scene = glob.LOCK.scene_or_exception()
 
         if glob.LOCK.project:
             raise Arcor2Exception("Project has to be closed first.")
 
         if not req.args.force and scene.has_changes:
             raise Arcor2Exception("Scene has unsaved changes.")
@@ -156,31 +154,28 @@
         glob.LOCK.scene = None
         glob.OBJECTS_WITH_UPDATED_POSE.clear()
         await clear_auto_remove_schedule()
         asyncio.ensure_future(notify_scene_closed(scene_id))
 
 
 async def save_scene_cb(req: srpc.s.SaveScene.Request, ui: WsClient) -> None:
-
     async with glob.LOCK.get_lock(req.dry_run):
-
         scene = glob.LOCK.scene_or_exception()
 
         if glob.LOCK.project:
             raise Arcor2Exception("Project has to be closed first.")
 
         if req.dry_run:
             return None
 
         await save_scene(scene)
         return None
 
 
 async def open_scene_cb(req: srpc.s.OpenScene.Request, ui: WsClient) -> None:
-
     async with glob.LOCK.get_lock():
         if glob.PACKAGE_STATE.state in PackageState.RUN_STATES:
             raise Arcor2Exception("Can't open scene while package runs.")
 
         if glob.LOCK.scene:
             raise Arcor2Exception("Scene already opened.")
 
@@ -191,15 +186,14 @@
         asyncio.ensure_future(
             notify_scene_opened(sevts.s.OpenScene(data=sevts.s.OpenScene.Data(glob.LOCK.scene.scene)))
         )
         return None
 
 
 async def list_scenes_cb(req: srpc.s.ListScenes.Request, ui: WsClient) -> srpc.s.ListScenes.Response:
-
     resp = srpc.s.ListScenes.Response()
     resp.data = []
 
     async for scene in scenes():
         assert scene.created
         assert scene.modified
         resp.data.append(
@@ -208,22 +202,19 @@
             )
         )
 
     return resp
 
 
 async def get_scene_cb(req: srpc.s.GetScene.Request, ui: WsClient) -> srpc.s.GetScene.Response:
-
     return srpc.s.GetScene.Response(data=(await storage.get_scene(req.args.id)).scene)
 
 
 async def add_object_to_scene_cb(req: srpc.s.AddObjectToScene.Request, ui: WsClient) -> None:
-
     async with ctx_write_lock(glob.LOCK.SpecialValues.SCENE, glob.USERS.user_name(ui)):
-
         scene = glob.LOCK.scene_or_exception()
 
         if glob.LOCK.project:
             raise Arcor2Exception("Project has to be closed first.")
 
         can_modify_scene()
 
@@ -241,15 +232,14 @@
         evt = sevts.s.SceneObjectChanged(obj)
         evt.change_type = Event.Type.ADD
         asyncio.ensure_future(notif.broadcast_event(evt))
         return None
 
 
 async def update_object_parameters_cb(req: srpc.s.UpdateObjectParameters.Request, ui: WsClient) -> None:
-
     scene = glob.LOCK.scene_or_exception(ensure_project_closed=True)
 
     can_modify_scene()
 
     obj = scene.object(req.args.id)
 
     if obj.type not in glob.OBJECT_TYPES:
@@ -297,15 +287,14 @@
         return resp
 
 
 # TODO move to objects
 async def action_param_values_cb(
     req: srpc.o.ActionParamValues.Request, ui: WsClient
 ) -> srpc.o.ActionParamValues.Response:
-
     glob.LOCK.scene_or_exception()
 
     async with ctx_read_lock(req.args.id, glob.USERS.user_name(ui)):
         ensure_scene_started()
 
         inst = get_instance(req.args.id, Generic)
 
@@ -337,21 +326,19 @@
 
         # TODO update hlp.run_in_executor to support kwargs
         resp.data = await asyncio.get_event_loop().run_in_executor(None, functools.partial(method, **parent_params))
         return resp
 
 
 async def remove_from_scene_cb(req: srpc.s.RemoveFromScene.Request, ui: WsClient) -> None:
-
     scene = glob.LOCK.scene_or_exception(ensure_project_closed=True)
     user_name = glob.USERS.user_name(ui)
 
     to_lock = await get_unlocked_objects(req.args.id, user_name)
     async with ctx_write_lock(to_lock, user_name, auto_unlock=req.dry_run):
-
         can_modify_scene()
 
         if not req.args.force and {proj.name async for proj in projects_using_object(scene.id, req.args.id)}:
             raise Arcor2Exception("Can't remove object that is used in project(s).")
 
         if req.dry_run:
             return None
@@ -447,15 +434,14 @@
         )
 
         asyncio.ensure_future(update_scene_object_pose(scene, scene_object))
         return None
 
 
 async def update_object_pose_cb(req: srpc.s.UpdateObjectPose.Request, ui: WsClient) -> None:
-
     scene = glob.LOCK.scene_or_exception(ensure_project_closed=True)
 
     if scene_started():
         try:
             get_robot_instance(req.args.object_id)
         except Arcor2Exception:
             pass  # ok, it should not be a robot
@@ -473,15 +459,14 @@
         return
 
     asyncio.ensure_future(update_scene_object_pose(scene, obj, req.args.pose))
     return None
 
 
 async def rename_object_cb(req: srpc.s.RenameObject.Request, ui: WsClient) -> None:
-
     scene = glob.LOCK.scene_or_exception(ensure_project_closed=True)
     target_obj = scene.object(req.args.id)
 
     if target_obj.name == req.args.new_name:
         raise Arcor2Exception("Name unchanged")
 
     for obj_name in scene.object_names():
@@ -505,15 +490,14 @@
     asyncio.ensure_future(notif.broadcast_event(evt))
 
     await glob.LOCK.write_unlock(req.args.id, user_name, True)
     return None
 
 
 async def rename_scene_cb(req: srpc.s.RenameScene.Request, ui: WsClient) -> None:
-
     unique_name(req.args.new_name, (await scene_names()))
 
     # TODO workaround for https://gitlab.com/kinalisoft/test-it-off/project/-/issues/16
     unique_name(req.args.new_name, (await project_names()))
 
     user_name = glob.USERS.user_name(ui)
     await ensure_write_locked(req.args.id, user_name)
@@ -529,22 +513,20 @@
         asyncio.ensure_future(notif.broadcast_event(evt))
 
     await glob.LOCK.write_unlock(req.args.id, user_name, True)
     return None
 
 
 async def delete_scene_cb(req: srpc.s.DeleteScene.Request, ui: WsClient) -> None | srpc.s.DeleteScene.Response:
-
     if glob.LOCK.scene:
         raise Arcor2Exception("Scene has to be closed first.")
 
     user_name = glob.USERS.user_name(ui)
 
     async with ctx_write_lock(req.args.id, user_name, auto_unlock=req.dry_run):
-
         if assoc_projects := await associated_projects(req.args.id):
             resp = srpc.s.DeleteScene.Response(result=False)
             resp.messages = ["Scene has associated projects."]
             resp.data = assoc_projects
             await glob.LOCK.write_unlock(req.args.id, user_name)
             return resp
 
@@ -565,51 +547,47 @@
         asyncio.ensure_future(notif.broadcast_event(evt))
         return None
 
 
 async def projects_with_scene_cb(
     req: srpc.s.ProjectsWithScene.Request, ui: WsClient
 ) -> srpc.s.ProjectsWithScene.Response:
-
     async with ctx_read_lock(req.args.id, glob.USERS.user_name(ui)):
         resp = srpc.s.ProjectsWithScene.Response()
         resp.data = await associated_projects(req.args.id)
         return resp
 
 
 async def update_scene_description_cb(req: srpc.s.UpdateSceneDescription.Request, ui: WsClient) -> None:
-
     async with ctx_write_lock(req.args.scene_id, glob.USERS.user_name(ui)):
         async with managed_scene(req.args.scene_id) as scene:
             scene.description = req.args.new_description
             scene.update_modified()
 
             evt = sevts.s.SceneChanged(scene.bare)
             evt.change_type = Event.Type.UPDATE_BASE
             asyncio.ensure_future(notif.broadcast_event(evt))
         return None
 
 
 async def copy_scene_cb(req: srpc.s.CopyScene.Request, ui: WsClient) -> None:
-
     async with ctx_write_lock(req.args.source_id, glob.USERS.user_name(ui)):
         # TODO check if target_name is unique
         async with managed_scene(req.args.source_id, make_copy=True) as scene:
             scene.name = req.args.target_name
 
             evt = sevts.s.SceneChanged(scene.bare)
             evt.change_type = Event.Type.UPDATE_BASE
             asyncio.ensure_future(notif.broadcast_event(evt))
 
         return None
 
 
 # TODO maybe this would better fit into another category of RPCs? Like common/misc?
 async def get_camera_pose_cb(req: srpc.c.GetCameraPose.Request, ui: WsClient) -> srpc.c.GetCameraPose.Response:
-
     try:
         return srpc.c.GetCameraPose.Response(
             data=await hlp.run_in_executor(
                 calibration.estimate_camera_pose,
                 req.args.camera_parameters,
                 image_from_str(req.args.image),
                 req.args.inverse,
@@ -620,24 +598,22 @@
     except calibration.CalibrationException as e:  # this means a serious problem and should be logged
         logger.warn(f"Failed to get camera pose. {str(e)}")
         raise
 
 
 # TODO maybe this would better fit into another category of RPCs? Like common/misc?
 async def marker_corners_cb(req: srpc.c.MarkersCorners.Request, ui: WsClient) -> srpc.c.MarkersCorners.Response:
-
     return srpc.c.MarkersCorners.Response(
         data=await hlp.run_in_executor(
             calibration.markers_corners, req.args.camera_parameters, image_from_str(req.args.image)
         )
     )
 
 
 async def start_scene_cb(req: srpc.s.StartScene.Request, ui: WsClient) -> None:
-
     scene = glob.LOCK.scene_or_exception()
 
     if get_scene_state().data.state != sevts.s.SceneState.Data.StateEnum.Stopped:
         raise Arcor2Exception("Scene not stopped.")
 
     # online scene can't be modified so we demand that UIs free all their locks first
     # when editing project, changes can be done both online and offline
@@ -653,15 +629,14 @@
     if req.dry_run:
         return
 
     asyncio.ensure_future(start_scene(scene))
 
 
 async def stop_scene_cb(req: srpc.s.StopScene.Request, ui: WsClient) -> None:
-
     scene = glob.LOCK.scene_or_exception()
 
     if get_scene_state().data.state != sevts.s.SceneState.Data.StateEnum.Started:
         raise Arcor2Exception("Scene not started.")
 
     if await glob.LOCK.is_write_locked(glob.LOCK.SpecialValues.SCENE, glob.LOCK.Owners.SERVER):
         raise Arcor2Exception("Scene locked.")
@@ -677,19 +652,17 @@
 
     asyncio.ensure_future(stop_scene(scene))
 
 
 async def add_virtual_collision_object_to_scene_cb(
     req: srpc.s.AddVirtualCollisionObjectToScene.Request, ui: WsClient
 ) -> None:
-
     async with ctx_write_lock(
         (glob.LOCK.SpecialValues.SCENE, glob.LOCK.SpecialValues.ADDING_OBJECT), glob.USERS.user_name(ui)
     ):
-
         scene = glob.LOCK.scene_or_exception()
 
         if glob.LOCK.project:
             raise Arcor2Exception("Project has to be closed first.")
 
         can_modify_scene()
```

### Comparing `arcor2_arserver-1.0.0/arcor2_arserver/rpc/user.py` & `arcor2_arserver-1.1.0/arcor2_arserver/rpc/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from arcor2_arserver import logger
 from arcor2_arserver.lock.structures import LockEventData
 from arcor2_arserver.rpc.objects import object_aiming_prune
 from arcor2_arserver_data import rpc as srpc
 
 
 async def register_user_cb(req: srpc.u.RegisterUser.Request, ui: WsClient) -> None:
-
     await glob.USERS.login(req.args.user_name, ui)
     logger.debug(f"User {req.args.user_name} just logged in. Known user names are: {glob.USERS.user_names}")
 
     await glob.LOCK.cancel_auto_release(req.args.user_name)
 
     # those are locks that are known for all users
     for user, user_objects in glob.LOCK.all_ui_locks.items():
```

### Comparing `arcor2_arserver-1.0.0/arcor2_arserver/scene.py` & `arcor2_arserver-1.1.0/arcor2_arserver/scene.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,34 +53,31 @@
 
 
 async def scheduled_to_be_auto_removed() -> set[str]:
     return _objects_to_auto_remove
 
 
 async def unschedule_auto_remove(obj_type: str) -> None:
-
     try:
         _objects_to_auto_remove.remove(obj_type)
     except KeyError:
         pass
     else:
         logger.debug(f"OT {obj_type} unscheduled to be auto-removed.")
 
 
 async def remove_scheduled() -> None:
-
     logger.debug(f"Going to auto-remove following types: {_objects_to_auto_remove}")
     for ot_id in _objects_to_auto_remove:
         if ot_id in glob.OBJECT_TYPES:
             asyncio.create_task(delete_if_not_used(glob.OBJECT_TYPES[ot_id].meta))
     _objects_to_auto_remove.clear()
 
 
 async def delete_if_not_used(meta: ObjectTypeMeta) -> None:
-
     if meta.base != VirtualCollisionObject.__name__:
         logger.debug(f"{meta.type} is not a VCO!")
         return
 
     assert meta.object_model
     assert meta.type == meta.object_model.model().id, f"meta.type={meta.type}, model.id={meta.object_model.model().id}"
 
@@ -106,15 +103,14 @@
 
     evtr = sevts.o.ChangedObjectTypes([meta])
     evtr.change_type = Event.Type.REMOVE
     await notif.broadcast_event(evtr)
 
 
 async def save_scene(scene: None | UpdateableCachedScene = None) -> None:
-
     if not scene:
         scene = glob.LOCK.scene_or_exception()
 
     scene.modified = await storage.update_scene(scene)
     asyncio.ensure_future(notif.broadcast_event(sevts.s.SceneSaved()))
     asyncio.create_task(remove_scheduled())
 
@@ -137,15 +133,14 @@
     ot_modified = get_ot_modified(ots)
 
     if (
         scene.id not in _scene_problems
         or _scene_problems[scene.id].scene_modified < scene.modified
         or _scene_problems[scene.id].ot_modified != ot_modified
     ):
-
         logger.debug(f"Updating scene_problems for {scene.name}.")
 
         _scene_problems[scene.id] = SceneProblems(
             scene.modified,
             scene_problems(glob.OBJECT_TYPES, scene),
             get_ot_modified(ots),
         )
@@ -188,29 +183,27 @@
     evt = SceneObjectChanged(obj)
     evt.change_type = Event.Type.UPDATE
     await notif.broadcast_event(evt)
 
     glob.OBJECTS_WITH_UPDATED_POSE.add(obj.id)
 
     if scene_started():
-
         if obj_inst is None:
             obj_inst = get_instance(obj.id, GenericWithPose)
 
         assert pose is not None
 
-        # Object pose is property that might call scene service - that's why it has to be called using executor.
-        await hlp.run_in_executor(setattr, obj_inst, "pose", pose)
+        # Setting object pose might call scene service - that's why it has to be called using executor.
+        await hlp.run_in_executor(obj_inst.set_pose, pose)
 
     if lock_owner:
         await glob.LOCK.write_unlock(obj.id, lock_owner, True)
 
 
 async def set_scene_state(state: SceneState.Data.StateEnum, message: None | str = None) -> None:
-
     global _scene_state
     _scene_state = SceneState(SceneState.Data(state, message))
     asyncio.create_task(notif.broadcast_event(_scene_state))
 
 
 def get_scene_state() -> SceneState:
     return _scene_state
@@ -231,33 +224,30 @@
     """Raises exception if scene is not started."""
 
     if _scene_state.data.state != SceneState.Data.StateEnum.Started:
         raise Arcor2Exception("Scene offline.")
 
 
 async def notify_scene_opened(evt: OpenScene) -> None:
-
     await notif.broadcast_event(evt)
     ss = get_scene_state()
     assert ss.data.state == ss.Data.StateEnum.Stopped
     await notif.broadcast_event(ss)
 
 
 async def scenes() -> AsyncIterator[CachedScene]:
-
     for scene_id in await storage.get_scene_ids():
         yield await storage.get_scene(scene_id)
 
 
 async def scene_names() -> set[str]:
     return {scene.name for scene in (await storage.get_scenes())}
 
 
 async def notify_scene_closed(scene_id: str) -> None:
-
     assert get_scene_state().data.state == SceneState.Data.StateEnum.Stopped
 
     await notif.broadcast_event(SceneClosed())
     glob.MAIN_SCREEN = ShowMainScreen.Data(ShowMainScreen.Data.WhatEnum.ScenesList)
     await notif.broadcast_event(
         ShowMainScreen(data=ShowMainScreen.Data(ShowMainScreen.Data.WhatEnum.ScenesList, scene_id))
     )
@@ -277,31 +267,28 @@
         return None
 
     scene.upsert_object(obj)
     logger.debug(f"Object {obj.id} ({obj.type}) added to scene.")
 
 
 async def create_object_instance(obj: SceneObject, overrides: None | list[Parameter] = None) -> None:
-
     obj_type = glob.OBJECT_TYPES[obj.type]
 
     # settings -> dataclass
     assert obj_type.type_def
     logger.debug(
         f"Creating instance of {obj_type.type_def.__name__} with name {obj.name}. "
         f"Parameters: {obj.parameters}, overrides: {overrides}."
     )
     settings = settings_from_params(obj_type.type_def, obj.parameters, overrides)
 
     assert obj_type.type_def is not None
 
     try:
-
         try:
-
             # the order must be from specific to the generic types
             if issubclass(obj_type.type_def, Robot):
                 assert obj.pose is not None
                 glob.SCENE_OBJECT_INSTANCES[obj.id] = await hlp.run_in_executor(
                     obj_type.type_def, obj.id, obj.name, obj.pose, settings
                 )
             elif issubclass(obj_type.type_def, CollisionObject):
@@ -335,66 +322,61 @@
         # make the exception a bit more user-friendly by including the object's name
         raise Arcor2Exception(f"Failed to initialize {obj.name}. {str(e)}") from e
 
     return None
 
 
 async def open_scene(scene_id: str) -> None:
-
     scene = await storage.get_scene(scene_id)
 
     if sp := await get_scene_problems(scene):  # this also refreshes ObjectTypes / calls get_object_types()
         logger.warning(f"Scene {scene.name} can't be opened due to the following problem(s)...")
         for spp in sp:
             logger.warning(spp)
         raise Arcor2Exception("Scene has some problems.")
 
     glob.LOCK.scene = UpdateableCachedScene(scene)
 
 
 def get_robot_instance(obj_id: str) -> Robot:  # TODO remove once https://github.com/python/mypy/issues/5374 is solved
-
     robot_inst = get_instance(obj_id, Robot)  # type: ignore
     assert isinstance(robot_inst, Robot)
     return robot_inst
 
 
 T = TypeVar("T", bound=Generic)
 
 
 # TODO "thanks" to https://github.com/python/mypy/issues/3737, `expected_type: type[T] = Generic` can't be used
 def get_instance(obj_id: str, expected_type: type[T]) -> T:
-
     assert scene_started()
 
     try:
         inst = glob.SCENE_OBJECT_INSTANCES[obj_id]
     except KeyError:
         raise Arcor2Exception("Unknown object ID.")
 
     if not isinstance(inst, expected_type):
         raise Arcor2Exception(f"{inst.name} is not of {expected_type.__name__} type.")
 
     return inst
 
 
 async def cleanup_object(obj: Generic) -> None:
-
     try:
         await hlp.run_in_executor(obj.cleanup)
     except Arcor2Exception as e:
         # make the exception a bit more user-friendly by including the object's name
         raise Arcor2Exception(f"Failed to cleanup {obj.name}. {str(e)}") from e
 
 
 async def stop_scene(scene: CachedScene, message: None | str = None, already_locked: bool = False) -> None:
     """Destroys scene object instances."""
 
     async def _stop_scene() -> None:
-
         await set_scene_state(SceneState.Data.StateEnum.Stopping, message)
 
         try:
             await scene_srv.stop()
         except Arcor2Exception as e:
             logger.exception("Failed to go offline.")
             await set_scene_state(SceneState.Data.StateEnum.Started, str(e))
@@ -408,25 +390,23 @@
         else:
             await set_scene_state(SceneState.Data.StateEnum.Stopped)
 
         glob.SCENE_OBJECT_INSTANCES.clear()
         glob.PREV_RESULTS.clear()
 
     if already_locked:
-
         logger.info(f"Stopping the {scene.name} scene after unsuccessful start.")
 
         assert await glob.LOCK.is_write_locked(glob.LOCK.SpecialValues.SCENE, glob.LOCK.Owners.SERVER)
         assert (glob.LOCK.project is not None) == await glob.LOCK.is_write_locked(
             glob.LOCK.SpecialValues.PROJECT, glob.LOCK.Owners.SERVER
         )
 
         await _stop_scene()
     else:
-
         to_lock = [glob.LOCK.SpecialValues.SCENE]
 
         if glob.LOCK.project:
             to_lock.append(glob.LOCK.SpecialValues.PROJECT)
 
         try:
             async with ctx_write_lock(to_lock, glob.LOCK.Owners.SERVER):
@@ -445,15 +425,14 @@
     logger.info("Scene stopped.")
 
 
 async def start_scene(scene: CachedScene) -> None:
     """Creates instances of scene objects."""
 
     async def _start_scene() -> bool:
-
         logger.info(f"Starting the {scene.name} scene.")
 
         await set_scene_state(SceneState.Data.StateEnum.Starting)
 
         # in order to prepare a clear environment
         try:
             # stop deletes all configurations and clears all collisions
```

### Comparing `arcor2_arserver-1.0.0/arcor2_arserver/scripts/arserver.py` & `arcor2_arserver-1.1.0/arcor2_arserver/scripts/arserver.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,29 +40,25 @@
 from arcor2_execution_data import EVENTS as EXE_EVENTS
 from arcor2_execution_data import EXPOSED_RPCS
 from arcor2_execution_data import RPCS as EXE_RPCS
 from arcor2_runtime import events as runtime_events
 
 
 async def handle_manager_incoming_messages(manager_client) -> None:
-
     event_mapping: dict[str, type[events.Event]] = {evt.__name__: evt for evt in EXE_EVENTS}
     rpc_mapping: dict[str, type[rpc.common.RPC]] = {r.__name__: r for r in EXE_RPCS}
 
     try:
-
         async for message in manager_client:
-
             msg = json.loads(message)
 
             if not isinstance(msg, dict):
                 continue
 
             if "event" in msg:
-
                 if glob.USERS.interfaces:
                     await asyncio.gather(
                         *[ws_server.send_json_to_client(intf, message) for intf in glob.USERS.interfaces]
                     )
 
                 try:
                     evt = event_mapping[msg["event"]].from_dict(msg)
@@ -72,15 +68,14 @@
 
                 if isinstance(evt, events.PackageInfo):
                     glob.PACKAGE_INFO = evt.data
                 elif isinstance(evt, events.PackageState):
                     glob.PACKAGE_STATE = evt.data
 
                     if evt.data.state == events.PackageState.Data.StateEnum.STOPPED:
-
                         if not glob.TEMPORARY_PACKAGE:
                             # after (ordinary) package is finished, show list of packages
                             glob.MAIN_SCREEN = evts.c.ShowMainScreen.Data(
                                 evts.c.ShowMainScreen.Data.WhatEnum.PackagesList
                             )
                             await notif.broadcast_event(
                                 evts.c.ShowMainScreen(
@@ -101,26 +96,24 @@
                         server_events.package_stopped.clear()
                         server_events.package_started.set()
 
                 elif isinstance(evt, events.ActionStateBefore):
                     glob.ACTION_STATE_BEFORE = evt.data
 
             elif "response" in msg:
-
                 # TODO handle potential errors
                 rpc_cls = rpc_mapping[msg["response"]]
                 resp = rpc_cls.Response.from_dict(msg)
                 exe.MANAGER_RPC_RESPONSES[resp.id].put_nowait(resp)
 
     except websockets.exceptions.ConnectionClosed as e:
         logger.error(f"Connection to manager closed. {str(e)}")
 
 
 async def _initialize_server() -> None:
-
     exe_version = await exe.manager_request(rpc.common.Version.Request(exe.get_id()))
     assert isinstance(exe_version, rpc.common.Version.Response)
     if not exe_version.result:
         raise Arcor2Exception("Failed to get Execution version.")
 
     assert exe_version.data is not None
 
@@ -172,27 +165,25 @@
 
 
 async def list_meshes_cb(req: obj_rpc.ListMeshes.Request, ui: WsClient) -> obj_rpc.ListMeshes.Response:
     return obj_rpc.ListMeshes.Response(data=await storage.get_meshes())
 
 
 async def register(websocket: WsClient) -> None:
-
     logger.info("Registering new ui")
     glob.USERS.add_interface(websocket)
 
     if glob.LOCK.project:
         assert glob.LOCK.scene
         await notif.event(
             websocket, evts.p.OpenProject(evts.p.OpenProject.Data(glob.LOCK.scene.scene, glob.LOCK.project.project))
         )
     elif glob.LOCK.scene:
         await notif.event(websocket, evts.s.OpenScene(evts.s.OpenScene.Data(glob.LOCK.scene.scene)))
     elif glob.PACKAGE_INFO:
-
         # this can't be done in parallel - ui expects this order of events
         await websocket.send(events.PackageState(glob.PACKAGE_STATE).to_json())
         await websocket.send(events.PackageInfo(glob.PACKAGE_INFO).to_json())
 
         if glob.ACTION_STATE_BEFORE:
             await websocket.send(events.ActionStateBefore(glob.ACTION_STATE_BEFORE).to_json())
     else:
@@ -200,15 +191,14 @@
         await notif.event(websocket, evts.c.ShowMainScreen(glob.MAIN_SCREEN))
 
     if glob.LOCK.project or glob.LOCK.scene:
         await notif.event(websocket, scene.get_scene_state())
 
 
 async def unregister(websocket: WsClient) -> None:
-
     try:
         user_name = glob.USERS.user_name(websocket)
     except Arcor2Exception:
         logger.info("Unregistering ui")
     else:
         await glob.LOCK.schedule_auto_release(user_name)
         logger.info(f"Unregistering ui {user_name}")
@@ -222,15 +212,14 @@
             registered_uis.remove(websocket)
     for registered_uis in glob.ROBOT_EEF_REGISTERED_UIS.values():
         if websocket in registered_uis:
             registered_uis.remove(websocket)
 
 
 async def system_info_cb(req: srpc.c.SystemInfo.Request, ui: WsClient) -> srpc.c.SystemInfo.Response:
-
     resp = srpc.c.SystemInfo.Response()
     resp.data = resp.Data(
         arcor2_arserver.version(),
         arcor2_arserver_data.version(),
         known_parameter_types(),
         {key for key in RPC_DICT.keys()},
     )
@@ -239,15 +228,14 @@
 
 RPC_DICT: ws_server.RPC_DICT_TYPE = {srpc.c.SystemInfo.__name__: (srpc.c.SystemInfo, system_info_cb)}
 
 # discovery of RPC callbacks
 # TODO refactor it into arcor2 package (to be used by arcor2_execution)
 for _, rpc_module in inspect.getmembers(srpc_callbacks, inspect.ismodule):
     for rpc_cb_name, rpc_cb in inspect.getmembers(rpc_module):
-
         if not rpc_cb_name.endswith("_cb"):
             continue
 
         hints = get_type_hints(rpc_cb)
 
         req_cls = hints["req"]
         rpc_cls = getattr(sys.modules[req_cls.__module__], req_cls.__qualname__.split(".")[0])
@@ -260,20 +248,18 @@
 
 
 # events from clients
 EVENT_DICT: ws_server.EVENT_DICT_TYPE = {}
 
 
 async def aio_main() -> None:
-
     await asyncio.gather(exe.project_manager_client(handle_manager_incoming_messages), _initialize_server())
 
 
 def print_openapi_models() -> None:
-
     modules = [arcor2_execution_data.events, events, runtime_events]
 
     for _, mod in inspect.getmembers(evts, inspect.ismodule):
         modules.append(mod)
 
     event_types: list[type[events.Event]] = []
 
@@ -286,15 +272,14 @@
         models.generate_openapi(
             "ARCOR2 ARServer", arcor2_arserver.version(), [v[0] for k, v in RPC_DICT.items()], event_types
         )
     )
 
 
 def main() -> None:
-
     parser = argparse.ArgumentParser()
 
     parser.add_argument("-v", "--verbose", help="Increase verbosity.", action="store_const", const=True, default=False)
     parser.add_argument(
         "-d",
         "--debug",
         help="Set logging level to debug.",
```

### Comparing `arcor2_arserver-1.0.0/arcor2_arserver/scripts/broadcaster.py` & `arcor2_arserver-1.1.0/arcor2_arserver/scripts/broadcaster.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,27 @@
 from arcor2.data.common import BroadcastInfo
 from arcor2_arserver.globals import PORT
 
 BROADCAST_PORT: int = 6006
 
 
 def get_ip() -> str:
-
     s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
     try:
         # doesn't even have to be reachable
         s.connect(("10.255.255.255", 1))
         ip = s.getsockname()[0]
     except socket.error:
         ip = "127.0.0.1"
     finally:
         s.close()
     return ip
 
 
 def get_broadcast() -> str:
-
     ip = get_ip()
     ip_arr = ip.split(".")
     ip_arr[-1] = "255"
     return ".".join(ip_arr)
 
 
 Address = tuple[str, int]
@@ -50,15 +48,14 @@
 
     def broadcast(self) -> None:
         self.transport.sendto(BroadcastInfo(socket.gethostname(), PORT).to_json().encode(), self.target)
         self.loop.call_later(1, self.broadcast)
 
 
 def main() -> None:
-
     loop = asyncio.get_event_loop()
 
     broadcast_coro = loop.create_datagram_endpoint(
         lambda: BroadcastProtocol((get_broadcast(), BROADCAST_PORT), loop=loop), local_addr=("0.0.0.0", BROADCAST_PORT)
     )
 
     loop.run_until_complete(broadcast_coro)
```

### Comparing `arcor2_arserver-1.0.0/arcor2_arserver/user.py` & `arcor2_arserver-1.1.0/arcor2_arserver/user.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,48 +7,43 @@
 
 
 class UsersException(Arcor2Exception):
     pass
 
 
 class Users:
-
     __slots__ = ("_interfaces", "_users_ui", "_ui_users")
 
     def __init__(self) -> None:
-
         self._interfaces: set[WsClient] = set()
         self._users_ui: dict[str, WsClient] = {}
         self._ui_users: dict[WsClient, str] = {}
 
     def _assert_consistency(self) -> None:
-
         assert list(self._ui_users.keys()) == list(self._users_ui.values())
         assert list(self._ui_users.values()) == list(self._users_ui.keys())
         assert set(self._ui_users).issubset(self._interfaces)
 
     @property
     def interfaces(self) -> set[WsClient]:
         return self._interfaces
 
     def add_interface(self, ui: WsClient) -> None:
         self._interfaces.add(ui)
 
     async def login(self, user_name: str, ui: WsClient) -> None:
-
         self._assert_consistency()
 
         if not user_name:
             raise UsersException("Empty user name.")
 
         if ui not in self._interfaces:
             raise UsersException("Unknown ui.")
 
         if user_name in self._users_ui:
-
             old_ui = self._users_ui[user_name]
 
             try:
                 pong_waiter = await old_ui.ping()
                 await asyncio.wait_for(pong_waiter, 1.0)
             except (WebSocketException, asyncio.TimeoutError):
                 self._users_ui.pop(user_name, None)
@@ -81,14 +76,13 @@
         self._assert_consistency()
 
     @property
     def user_names(self) -> set[str]:
         return set(self._users_ui)
 
     def user_name(self, ui: WsClient) -> str:
-
         self._assert_consistency()
 
         try:
             return self._ui_users[ui]
         except KeyError:
             raise UsersException("User not logged in.")
```

### Comparing `arcor2_arserver-1.0.0/arcor2_arserver.egg-info/PKG-INFO` & `arcor2_arserver-1.1.0/arcor2_arserver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcor2-arserver
-Version: 1.0.0
+Version: 1.1.0
 Summary: ARCOR2 ARServer
 Author: Robo@FIT
 Author-email: imaterna@fit.vut.cz
 License: LGPL
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -42,14 +42,20 @@
 - `ARCOR2_ARSERVER_DEBUG=1` - switches logger to the `DEBUG` level. 
 - `ARCOR2_ARSERVER_ASYNCIO_DEBUG=1` - turns on `asyncio` debug output (helpful to debug problems related to concurrency). 
 - `ARCOR2_REST_DEBUG=1` - may be used to debug problems related to communication with the Project, Scene Build and Calibration services.
 # Changelog
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 
+## [1.1.0] - 2023-07-20
+
+### Changed
+
+- Compatibility with arcor2 1.1.0 (object pose must now be updated with `obj.set_pose(pose)`).
+
 ## [1.0.0] - 2023-02-14
 
 ### Changed
 
 - Dependency on arcor2 1.0.0.
 - Compatibility with the newest version of the Project service.
 - ARServer now also talks to Asset service (checks whether mesh/URDF exists).
```

### Comparing `arcor2_arserver-1.0.0/arcor2_arserver.egg-info/SOURCES.txt` & `arcor2_arserver-1.1.0/arcor2_arserver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arcor2_arserver-1.0.0/setup.py` & `arcor2_arserver-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,30 +20,32 @@
     'entry_points': {
         'console_scripts': [
             'arcor2_arserver = arcor2_arserver.scripts.arserver:main',
             'arcor2_broadcaster = arcor2_arserver.scripts.broadcaster:main',
         ],
     },
     'install_requires': (
-        'aiofiles~=22.1.0',
+        'Flask~=2.2.3',
+        'aiofiles~=23.1.0',
         'aiologger~=0.7.0',
         'aiorun~=2022.11.1',
         'apispec-webframeworks~=0.5.2',
-        'apispec[yaml]~=6.0.2',
+        'apispec[yaml]~=6.3.0',
         'arcor2_arserver_data~=1.0.0',
         'arcor2_build_data~=1.0.0',
         'arcor2_calibration_data~=1.0.0',
         'arcor2_execution_data~=1.0.0',
         'arcor2_runtime~=1.0.0',
-        'arcor2~=1.0.0',
+        'arcor2~=1.1.0',
         'dataclasses-jsonschema[apispec,fast-dateparsing,fast-uuid,fast-validation]~=2.16.0',
         'lru-dict~=1.1.8',
-        'numpy-quaternion[numba,scipy]~=2022.4.2',
+        'numpy-quaternion[numba,scipy]~=2022.4.3',
         'numpy~=1.23.5',
         'pyhumps==3.8.0',
+        'setuptools~=66.0.0',
         'typing-inspect~=0.8.0',
         'websockets~=10.4',
     ),
     'license': 'LGPL',
     'long_description': """# arcor2_arserver
 
 ## Environment variables
@@ -71,14 +73,20 @@
 - `ARCOR2_ARSERVER_DEBUG=1` - switches logger to the `DEBUG` level. 
 - `ARCOR2_ARSERVER_ASYNCIO_DEBUG=1` - turns on `asyncio` debug output (helpful to debug problems related to concurrency). 
 - `ARCOR2_REST_DEBUG=1` - may be used to debug problems related to communication with the Project, Scene Build and Calibration services.
 # Changelog
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 
+## [1.1.0] - 2023-07-20
+
+### Changed
+
+- Compatibility with arcor2 1.1.0 (object pose must now be updated with `obj.set_pose(pose)`).
+
 ## [1.0.0] - 2023-02-14
 
 ### Changed
 
 - Dependency on arcor2 1.0.0.
 - Compatibility with the newest version of the Project service.
 - ARServer now also talks to Asset service (checks whether mesh/URDF exists).
@@ -419,9 +427,9 @@
         'arcor2_arserver.clients',
         'arcor2_arserver.lock',
         'arcor2_arserver.object_types',
         'arcor2_arserver.rpc',
         'arcor2_arserver.scripts',
     ),
     'python_requires': '==3.10.*',
-    'version': '1.0.0',
+    'version': '1.1.0',
 })
```

