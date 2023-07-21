# Comparing `tmp/arcor2-1.0.0rc1.tar.gz` & `tmp/arcor2-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcor2-1.0.0rc1.tar", last modified: Mon Feb  6 09:29:50 2023, max compression
+gzip compressed data, was "arcor2-1.1.0.tar", last modified: Thu Jul 20 11:09:55 2023, max compression
```

## Comparing `arcor2-1.0.0rc1.tar` & `arcor2-1.1.0.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-02-06 09:29:50.190730 arcor2-1.0.0rc1/
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)       12 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/MANIFEST.in
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)    19021 2023-02-06 09:29:50.190730 arcor2-1.0.0rc1/PKG-INFO
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-02-06 09:29:50.182730 arcor2-1.0.0rc1/arcor2/
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)        8 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/VERSION
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)      734 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/__init__.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)    23638 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/cached.py
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-02-06 09:29:50.186730 arcor2-1.0.0rc1/arcor2/clients/
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)        0 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/clients/__init__.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)      508 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/clients/aio_asset.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     2743 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/clients/aio_project_service.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     1409 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/clients/aio_scene_service.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     2043 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/clients/asset.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     8736 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/clients/project_service.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     5498 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/clients/scene_service.py
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-02-06 09:29:50.186730 arcor2-1.0.0rc1/arcor2/data/
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     2309 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/data/__init__.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)      755 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/data/camera.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)    18677 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/data/common.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     4028 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/data/events.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)      268 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/data/execution.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     4058 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/data/object_type.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)      195 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/data/robot.py
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-02-06 09:29:50.186730 arcor2-1.0.0rc1/arcor2/data/rpc/
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)      212 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/data/rpc/__init__.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     2022 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/data/rpc/common.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)      694 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/data/scene.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     3470 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/docstring.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)      971 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/env.py
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-02-06 09:29:50.186730 arcor2-1.0.0rc1/arcor2/exceptions/
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)      152 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/exceptions/__init__.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)      911 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/exceptions/helpers.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     6682 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/flask.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     6331 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/helpers.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     1178 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/image.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)      817 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/json.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     1226 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/logging.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     1475 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/logic.py
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-02-06 09:29:50.186730 arcor2-1.0.0rc1/arcor2/object_types/
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)        0 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/object_types/__init__.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)    14998 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/object_types/abstract.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)      716 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/object_types/flow_actions.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     1037 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/object_types/logic_actions.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     1492 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/object_types/random_actions.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     1393 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/object_types/time_actions.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     4359 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/object_types/upload.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     6817 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/object_types/utils.py
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-02-06 09:29:50.190730 arcor2-1.0.0rc1/arcor2/parameter_plugins/
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)      193 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/parameter_plugins/__init__.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     3760 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/parameter_plugins/base.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     1703 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/parameter_plugins/boolean.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     2220 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/parameter_plugins/double.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     1305 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/parameter_plugins/image.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     3880 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/parameter_plugins/integer.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     3815 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/parameter_plugins/integer_enum.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     2396 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/parameter_plugins/joints.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     1301 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/parameter_plugins/list.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     4538 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/parameter_plugins/pose.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     2187 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/parameter_plugins/position.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     1481 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/parameter_plugins/string.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)      320 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/parameter_plugins/string_enum.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     3169 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/parameter_plugins/utils.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)        0 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/py.typed
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)    10631 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/rest.py
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-02-06 09:29:50.190730 arcor2-1.0.0rc1/arcor2/scripts/
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)        0 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/scripts/__init__.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)      486 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/scripts/upload_builtin_objects.py
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-02-06 09:29:50.190730 arcor2-1.0.0rc1/arcor2/source/
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)      171 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/source/__init__.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     5486 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/source/utils.py
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-02-06 09:29:50.190730 arcor2-1.0.0rc1/arcor2/test_objects/
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)      165 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/test_objects/__init__.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)      625 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/test_objects/box.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)       65 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/test_objects/box2.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     6602 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/test_objects/dummy_multiarm_robot.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)      621 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/test_objects/param_to_return.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)      450 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/test_objects/position_param.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     1982 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/test_objects/tester.py
--rwxr-xr-x   0 zdenal    (1000) zdenal    (1000)      771 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/test_objects/upload.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     7136 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/transformations.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     1882 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/urdf.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     6189 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/arcor2/ws_server.py
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-02-06 09:29:50.186730 arcor2-1.0.0rc1/arcor2.egg-info/
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)    19021 2023-02-06 09:29:50.000000 arcor2-1.0.0rc1/arcor2.egg-info/PKG-INFO
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)     2203 2023-02-06 09:29:50.000000 arcor2-1.0.0rc1/arcor2.egg-info/SOURCES.txt
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)        1 2023-02-06 09:29:50.000000 arcor2-1.0.0rc1/arcor2.egg-info/dependency_links.txt
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)       93 2023-02-06 09:29:50.000000 arcor2-1.0.0rc1/arcor2.egg-info/entry_points.txt
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)        1 2023-02-06 09:29:50.000000 arcor2-1.0.0rc1/arcor2.egg-info/namespace_packages.txt
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)      494 2023-02-06 09:29:50.000000 arcor2-1.0.0rc1/arcor2.egg-info/requires.txt
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)        7 2023-02-06 09:29:50.000000 arcor2-1.0.0rc1/arcor2.egg-info/top_level.txt
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)      698 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/backend_shim.py
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)       38 2023-02-06 09:29:50.190730 arcor2-1.0.0rc1/setup.cfg
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)    20633 2023-02-06 09:29:49.000000 arcor2-1.0.0rc1/setup.py
+drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-07-20 11:09:55.034956 arcor2-1.1.0/
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)       12 2023-07-20 11:09:54.000000 arcor2-1.1.0/MANIFEST.in
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)    19205 2023-07-20 11:09:55.034956 arcor2-1.1.0/PKG-INFO
+drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-07-20 11:09:55.030956 arcor2-1.1.0/arcor2/
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)        5 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/VERSION
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)      732 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/__init__.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)    25186 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/cached.py
+drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-07-20 11:09:55.030956 arcor2-1.1.0/arcor2/clients/
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)        0 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/clients/__init__.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)      508 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/clients/aio_asset.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     2743 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/clients/aio_project_service.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     1409 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/clients/aio_scene_service.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     2039 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/clients/asset.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     8731 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/clients/project_service.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     5495 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/clients/scene_service.py
+drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-07-20 11:09:55.034956 arcor2-1.1.0/arcor2/data/
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     2304 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/data/__init__.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)      752 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/data/camera.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)    21507 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/data/common.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     4026 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/data/events.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)      267 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/data/execution.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     4043 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/data/object_type.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)      194 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/data/robot.py
+drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-07-20 11:09:55.034956 arcor2-1.1.0/arcor2/data/rpc/
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)      212 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/data/rpc/__init__.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     2019 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/data/rpc/common.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)      690 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/data/scene.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     3469 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/docstring.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)      969 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/env.py
+drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-07-20 11:09:55.034956 arcor2-1.1.0/arcor2/exceptions/
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)      152 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/exceptions/__init__.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)      910 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/exceptions/helpers.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     7081 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/flask.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     6328 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/helpers.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     1176 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/image.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)      814 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/json.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     1223 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/logging.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     1472 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/logic.py
+drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-07-20 11:09:55.034956 arcor2-1.1.0/arcor2/object_types/
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)        0 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/object_types/__init__.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)    14792 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/object_types/abstract.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)      716 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/object_types/flow_actions.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     1037 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/object_types/logic_actions.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     1492 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/object_types/random_actions.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     1391 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/object_types/time_actions.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     4355 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/object_types/upload.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     6810 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/object_types/utils.py
+drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-07-20 11:09:55.034956 arcor2-1.1.0/arcor2/parameter_plugins/
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)      193 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/parameter_plugins/__init__.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     3752 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/parameter_plugins/base.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     1702 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/parameter_plugins/boolean.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     2220 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/parameter_plugins/double.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     1305 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/parameter_plugins/image.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     3875 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/parameter_plugins/integer.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     3810 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/parameter_plugins/integer_enum.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     2393 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/parameter_plugins/joints.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     1299 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/parameter_plugins/list.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     4531 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/parameter_plugins/pose.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     2184 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/parameter_plugins/position.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     1481 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/parameter_plugins/string.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)      320 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/parameter_plugins/string_enum.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     3163 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/parameter_plugins/utils.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)        0 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/py.typed
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)    11124 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/rest.py
+drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-07-20 11:09:55.034956 arcor2-1.1.0/arcor2/scripts/
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)        0 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/scripts/__init__.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)      485 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/scripts/upload_builtin_objects.py
+drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-07-20 11:09:55.034956 arcor2-1.1.0/arcor2/source/
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)      171 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/source/__init__.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     5482 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/source/utils.py
+drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-07-20 11:09:55.034956 arcor2-1.1.0/arcor2/test_objects/
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)      165 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/test_objects/__init__.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)      624 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/test_objects/box.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)       64 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/test_objects/box2.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     6599 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/test_objects/dummy_multiarm_robot.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)      620 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/test_objects/param_to_return.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)      449 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/test_objects/position_param.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     1982 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/test_objects/tester.py
+-rwxr-xr-x   0 zdenal    (1000) zdenal    (1000)      770 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/test_objects/upload.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     7129 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/transformations.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     1879 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/urdf.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     6181 2023-07-20 11:09:54.000000 arcor2-1.1.0/arcor2/ws_server.py
+drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-07-20 11:09:55.030956 arcor2-1.1.0/arcor2.egg-info/
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)    19205 2023-07-20 11:09:55.000000 arcor2-1.1.0/arcor2.egg-info/PKG-INFO
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)     2203 2023-07-20 11:09:55.000000 arcor2-1.1.0/arcor2.egg-info/SOURCES.txt
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)        1 2023-07-20 11:09:55.000000 arcor2-1.1.0/arcor2.egg-info/dependency_links.txt
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)       93 2023-07-20 11:09:55.000000 arcor2-1.1.0/arcor2.egg-info/entry_points.txt
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)        1 2023-07-20 11:09:55.000000 arcor2-1.1.0/arcor2.egg-info/namespace_packages.txt
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)      513 2023-07-20 11:09:55.000000 arcor2-1.1.0/arcor2.egg-info/requires.txt
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)        7 2023-07-20 11:09:55.000000 arcor2-1.1.0/arcor2.egg-info/top_level.txt
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)      822 2023-07-20 11:09:54.000000 arcor2-1.1.0/backend_shim.py
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)       38 2023-07-20 11:09:55.034956 arcor2-1.1.0/setup.cfg
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)    20847 2023-07-20 11:09:54.000000 arcor2-1.1.0/setup.py
```

### Comparing `arcor2-1.0.0rc1/PKG-INFO` & `arcor2-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcor2
-Version: 1.0.0rc1
+Version: 1.1.0
 Summary: ARCOR2 base library
 Author: Robo@FIT
 Author-email: imaterna@fit.vut.cz
 License: LGPL
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -16,21 +16,32 @@
 Description-Content-Type: text/markdown
 
 # arcor2
 # Changelog
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 
-## [1.0.0rc1] - 2023-02-06
+## [1.1.0] - 2023-07-20
+
+### Added
+
+- Few new helper functions.
+
+### Changed
+
+- Object pose is now not set using a property setter but using the `set_pose` method.  
+
+## [1.0.0] - 2023-02-14
 
 ### Changed
 
 - Updated dependencies.
-- Compatibility with the newest version of the Project service.
-- Project service client updated to match Project 1.0.0-rc.1.
+- Compatibility with the Project service 1.0.0.
+  - `Mesh` dataclass: `data_id` changed to `asset_id`.
+  - Updated client (some paths were changed).
 
 ### Added
 
 - Method `start` from the Scene service client now allows to specify a timeout. 
 
 ## [0.26.0] - 2022-12-12
```

### Comparing `arcor2-1.0.0rc1/arcor2/__init__.py` & `arcor2-1.1.0/arcor2/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import pkgutil
 import warnings
 from typing import NamedTuple
 
 
 class DynamicParamTuple(NamedTuple):
-
     method_name: str
     parent_parameters: set[str]
 
 
 # key: name of parameter, value: name of method to call (to get set of strings), set of parent parameters
 DynamicParamDict = dict[str, DynamicParamTuple]
 
@@ -17,15 +16,14 @@
 
 
 if __debug__:
     warnings.filterwarnings("error", module="dataclasses_jsonschema")  # make warnings fatal because they are
 
 
 def package_version(package: str, file: str = "VERSION") -> str:
-
     if res := pkgutil.get_data(package, file):
         return res.decode().strip()
     return "unknown"
 
 
 def version() -> str:
     return package_version(__name__)
```

### Comparing `arcor2-1.0.0rc1/arcor2/cached.py` & `arcor2-1.1.0/arcor2/cached.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,30 +15,27 @@
 
 
 class CachedSceneException(Arcor2Exception):
     pass
 
 
 class CachedBase:
-
     __slots__ = "id", "name", "description", "created", "modified", "int_modified"
 
     def __init__(self, data: cmn.Scene | cmn.Project | CachedScene | CachedProject) -> None:
-
         self.id: str = data.id
         self.name: str = data.name
         self.description: str = data.description
 
         self.created: None | datetime = data.created
         self.modified: None | datetime = data.modified
         self.int_modified: None | datetime = data.int_modified
 
 
 class UpdateableMixin:
-
     if TYPE_CHECKING:
         __slots__ = "modified", "int_modified"
 
         modified: None | datetime = None
         int_modified: None | datetime = None
     else:
         __slots__ = ()
@@ -65,99 +62,108 @@
         # if the scene/project was already saved once (modified is not None)
         # and there were some changes (int_modified is not None)
         # let's compare if some change happened (int_modified) after saving to the Project service (modified)
         return self.int_modified > self.modified
 
 
 class CachedScene(CachedBase):
-
     __slots__ = ("_objects", "_object_types")
 
     def __init__(self, scene: cmn.Scene | CachedScene) -> None:
-
         super().__init__(scene)
 
         self._objects: dict[str, cmn.SceneObject] = {}
 
         if isinstance(scene, CachedScene):
             self._objects = scene._objects
         else:
             # TODO deal with children
 
             for obj in scene.objects:
-
                 if obj.id in self._objects:
                     raise CachedSceneException(f"Duplicate object id: {obj.id}.")
 
                 self._objects[obj.id] = obj
 
         self._object_types = {obj.type for obj in self.objects}
 
     @property
     def bare(self) -> cmn.BareScene:
         return cmn.BareScene(self.name, self.description, self.created, self.modified, self.int_modified, id=self.id)
 
     def object_names(self) -> Iterator[str]:
-
         for obj in self._objects.values():
             yield obj.name
 
     @property
     def objects(self) -> Iterator[cmn.SceneObject]:
-
         for obj in self._objects.values():
             yield obj
 
     @property
     def object_ids(self) -> set[str]:
         return set(self._objects)
 
     def object(self, object_id: str) -> cmn.SceneObject:
-
         try:
             return self._objects[object_id]
         except KeyError:
             raise Arcor2Exception(f"Object ID {object_id} not found.")
 
     def objects_of_type(self, obj_type: str) -> Iterator[cmn.SceneObject]:
-
         for obj in self.objects:
             if obj.type == obj_type:
                 yield obj
 
     @property
     def object_types(self) -> set[str]:
         assert self._object_types == {obj.type for obj in self.objects}
         return self._object_types
 
     @property
     def scene(self) -> cmn.Scene:
-
         sc = cmn.Scene.from_bare(self.bare)
         sc.modified = self.modified
         sc.int_modified = self.int_modified
         sc.objects = list(self.objects)
         return sc
 
+    def get_object_by_name(self, object_method: str) -> str:
+        """find object in scene by name and return a json representation of the
+        object with its method, for example dobot_magician.pick ->
+        obj_123456789abc/pick.
 
-class UpdateableCachedScene(UpdateableMixin, CachedScene):
+        :param object_method: Object and Method in str  for example "dobot_magician.pick"
+
+        :return:    Object_id/method for example "obj_123456789abc/pick"
+        """
+
+        # looking for object
+        for scene_object in self.objects:
+            if object_method.find(scene_object.name + ".") != -1:
+                # replace name from code to scene definition
+                object_type = object_method.replace(scene_object.name + ".", (scene_object.id + "/"))
 
+                return object_type
+
+        raise Arcor2Exception(f"Object with method {object_method} was not found")
+
+
+class UpdateableCachedScene(UpdateableMixin, CachedScene):
     __slots__ = ()
 
     def __init__(self, scene: cmn.Scene | CachedScene):
         super(UpdateableCachedScene, self).__init__(copy.deepcopy(scene))
 
     def upsert_object(self, obj: cmn.SceneObject) -> None:
-
         self._objects[obj.id] = obj
         self._object_types.add(obj.type)
         self.update_modified()
 
     def delete_object(self, obj_id: str) -> None:
-
         try:
             obj = self._objects.pop(obj_id)
         except KeyError as e:
             raise Arcor2Exception("Object id not found.") from e
 
         if not any(True for _ in self.objects_of_type(obj.type)):
             self._object_types.discard(obj.type)
@@ -169,46 +175,41 @@
 
 class CachedProjectException(Arcor2Exception):
     pass
 
 
 @dataclass
 class Parent:
-
     __slots__ = ("ap",)
 
     ap: cmn.BareActionPoint
 
 
 @dataclass
 class ApAction(Parent):
-
     __slots__ = ("action",)
 
     action: cmn.Action
 
 
 @dataclass
 class ApJoints(Parent):
-
     __slots__ = ("joints",)
 
     joints: cmn.ProjectRobotJoints
 
 
 @dataclass
 class ApOrientation(Parent):
-
     __slots__ = ("orientation",)
 
     orientation: cmn.NamedOrientation
 
 
 class CachedProject(CachedBase):
-
     __slots__ = (
         "scene_id",
         "has_logic",
         "_action_points",
         "_actions",
         "_joints",
         "_orientations",
@@ -217,15 +218,14 @@
         "_functions",
         "overrides",
         "_childs",
         "project_objects_ids",
     )
 
     def __init__(self, project: cmn.Project | CachedProject):
-
         super().__init__(project)
 
         self.scene_id: str = project.scene_id
         self.has_logic: bool = project.has_logic
         self.project_objects_ids: None | list[str] = project.project_objects_ids
 
         self._action_points: dict[str, cmn.BareActionPoint] = {}
@@ -250,42 +250,37 @@
             self._parameters = project._parameters
             self._logic_items = project._logic_items
             self._functions = project._functions
             self.overrides = project.overrides
             self._childs = project._childs
 
         else:
-
             for ap in project.action_points:
-
                 if ap.id in self._action_points:
                     raise CachedProjectException(f"Duplicate AP id: {ap.id}.")
 
                 bare_ap = cmn.BareActionPoint(ap.name, ap.position, ap.parent, id=ap.id)
                 self._action_points[ap.id] = bare_ap
                 self._upsert_child(ap.parent, ap.id)
 
                 for ac in ap.actions:
-
                     if ac.id in self._actions:
                         raise CachedProjectException(f"Duplicate action id: {ac.id}.")
 
                     self._actions[ac.id] = ApAction(bare_ap, ac)
                     self._upsert_child(ap.id, ac.id)
 
                 for joints in ap.robot_joints:
-
                     if joints.id in self._joints:
                         raise CachedProjectException(f"Duplicate joints id: {joints.id}.")
 
                     self._joints[joints.id] = ApJoints(bare_ap, joints)
                     self._upsert_child(ap.id, joints.id)
 
                 for orientation in ap.orientations:
-
                     if orientation.id in self._orientations:
                         raise CachedProjectException(f"Duplicate orientation id: {orientation.id}.")
 
                     self._orientations[orientation.id] = ApOrientation(bare_ap, orientation)
                     self._upsert_child(ap.id, orientation.id)
 
             for override in project.object_overrides:
@@ -318,19 +313,17 @@
 
     @property
     def functions(self) -> ValuesView[cmn.ProjectFunction]:
         return self._functions.values()
 
     @property
     def project(self) -> cmn.Project:
-
         proj = cmn.Project.from_bare(self.bare)
 
         for bare_ap in self._action_points.values():
-
             ap = cmn.ActionPoint.from_bare(bare_ap)
             ap.actions = self.ap_actions(ap.id)
             ap.robot_joints = self.ap_joints(ap.id)
             ap.orientations = self.ap_orientations(ap.id)
             proj.action_points.append(ap)
 
         proj.object_overrides = [cmn.SceneObjectOverride(k, v) for k, v in self.overrides.items()]
@@ -375,53 +368,46 @@
         return {ap.name for ap in self._action_points.values()}
 
     @property
     def action_points_ids(self) -> set[str]:
         return set(self._action_points)
 
     def ap_and_joints(self, joints_id: str) -> tuple[cmn.BareActionPoint, cmn.ProjectRobotJoints]:
-
         try:
             value = self._joints[joints_id]
         except KeyError:
             raise CachedProjectException("Unknown joints.")
 
         return value.ap, value.joints
 
     def joints(self, joints_id: str) -> cmn.ProjectRobotJoints:
-
         try:
             return self._joints[joints_id].joints
         except KeyError:
             raise CachedProjectException("Unknown joints.")
 
     def bare_ap_and_orientation(self, orientation_id: str) -> tuple[cmn.BareActionPoint, cmn.NamedOrientation]:
-
         try:
             value = self._orientations[orientation_id]
         except KeyError:
             raise CachedProjectException("Unknown orientation.")
 
         return value.ap, value.orientation
 
     def pose(self, orientation_id: str) -> cmn.Pose:
-
         ap, ori = self.bare_ap_and_orientation(orientation_id)
         return cmn.Pose(ap.position, ori.orientation)
 
     def ap_orientations(self, ap_id: str) -> list[cmn.NamedOrientation]:
-
         return [value.orientation for value in self._orientations.values() if ap_id == value.ap.id]
 
     def ap_joints(self, ap_id: str) -> list[cmn.ProjectRobotJoints]:
-
         return [value.joints for value in self._joints.values() if ap_id == value.ap.id]
 
     def ap_actions(self, ap_id: str) -> list[cmn.Action]:
-
         return [value.action for value in self._actions.values() if ap_id == value.ap.id]
 
     def ap_action_ids(self, ap_id: str) -> set[str]:
         return {ac.id for ac in self.ap_actions(ap_id)}
 
     def ap_orientation_names(self, ap_id: str) -> set[str]:
         return {ori.name for ori in self.ap_orientations(ap_id)}
@@ -429,22 +415,20 @@
     def ap_joint_names(self, ap_id: str) -> set[str]:
         return {joints.name for joints in self.ap_joints(ap_id)}
 
     def ap_action_names(self, ap_id: str) -> set[str]:
         return {action.name for action in self.ap_actions(ap_id)}
 
     def orientation(self, orientation_id: str) -> cmn.NamedOrientation:
-
         try:
             return self._orientations[orientation_id].orientation
         except KeyError:
             raise CachedProjectException("Unknown orientation.")
 
     def action(self, action_id: str) -> cmn.Action:
-
         try:
             return self._actions[action_id].action
         except KeyError:
             raise CachedProjectException("Action not found")
 
     def action_io(self, action_id: str) -> tuple[list[cmn.LogicItem], list[cmn.LogicItem]]:
         """Returns list of logical connection ending in the action (its inputs)
@@ -467,30 +451,28 @@
         if __debug__:  # make it a bit harder for tests to succeed
             random.shuffle(inputs)
             random.shuffle(outputs)
 
         return inputs, outputs
 
     def first_action_id(self) -> str:
-
         first_action: None | str = None
 
         for item in self._logic_items.values():
             if item.start == item.START:
                 if first_action:
                     raise CachedProjectException("Duplicate start.")
                 first_action = self.action(item.end).id
 
         if first_action is None:
             raise CachedProjectException("Start action not found.")
 
         return first_action
 
     def action_point_and_action(self, action_id: str) -> tuple[cmn.BareActionPoint, cmn.Action]:
-
         try:
             value = self._actions[action_id]
         except KeyError:
             raise CachedProjectException("Action not found")
 
         return value.ap, value.action
 
@@ -498,29 +480,26 @@
     def actions(self) -> list[cmn.Action]:
         return [value.action for value in self._actions.values()]
 
     def action_ids(self) -> set[str]:
         return set(self._actions)
 
     def bare_action_point(self, action_point_id: str) -> cmn.BareActionPoint:
-
         try:
             return self._action_points[action_point_id]
         except KeyError:
             raise CachedProjectException("Action point not found")
 
     def action_point(self, action_point_id: str) -> cmn.ActionPoint:
-
         ap = cmn.ActionPoint.from_bare(self.bare_action_point(action_point_id))
         ap.orientations = self.ap_orientations(action_point_id)
         ap.robot_joints = self.ap_joints(action_point_id)
         return ap
 
     def logic_item(self, logic_item_id: str) -> cmn.LogicItem:
-
         try:
             return self._logic_items[logic_item_id]
         except KeyError:
             raise CachedProjectException("LogicItem not found.")
 
     def parameter(self, parameter_id: str) -> cmn.ProjectParameter:
         """Gets a project parameter by its ID.
@@ -533,30 +512,28 @@
             return self._parameters[parameter_id]
         except KeyError:
             raise CachedProjectException("Project parameter not found.")
 
     def get_by_id(
         self, obj_id: str
     ) -> cmn.BareActionPoint | cmn.NamedOrientation | cmn.ProjectRobotJoints | cmn.Action | cmn.ProjectParameter:
-
         if obj_id in self._action_points:  # AP
             return self._action_points[obj_id]
         elif obj_id in self._joints:  # Joints
             return self._joints[obj_id].joints
         elif obj_id in self._orientations:  # Orientation
             return self._orientations[obj_id].orientation
         elif obj_id in self._actions:  # Action
             return self._actions[obj_id].action
         elif obj_id in self._parameters:
             return self._parameters[obj_id]
 
         raise CachedProjectException("Object not found.")
 
     def get_parent_id(self, obj_id: str) -> None | str:
-
         if obj_id in self._action_points:  # AP
             return self._action_points[obj_id].parent if self._action_points[obj_id].parent else None
         elif obj_id in self._joints:  # Joints
             return self._joints[obj_id].ap.id
         elif obj_id in self._orientations:  # Orientation
             return self._orientations[obj_id].ap.id
         elif obj_id in self._actions:  # Action
@@ -567,133 +544,140 @@
     def _upsert_child(self, parent: None | str, child: str) -> None:
         if parent:
             if parent not in self._childs:
                 self._childs[parent] = set()
             self._childs[parent].add(child)
 
     def childs(self, obj_id: str, recursive: bool = False) -> set[str]:
-
         try:
             ret = self._childs[obj_id]
         except KeyError:
             return set()  # TODO distinguish between no childs and unknown object
 
         if not recursive:
             return ret
 
         return ret | {c for s in [self.childs(ch, True) for ch in ret] for c in s}
 
     def _remove_child(self, parent: None | str, child: str) -> None:
-
         if parent and parent in self._childs:
             self._childs[parent].remove(child)
             if not self._childs[parent]:
                 del self._childs[parent]
 
     def update_child(self, obj_id: str, old_parent: None | str, new_parent: None | str) -> None:
-
         self._remove_child(old_parent, obj_id)
         self._upsert_child(new_parent, obj_id)
 
+    def find_logic_start_end(self, start: str, end: str) -> cmn.LogicItem:
+        """find specific LogicItem with start parameter and end parameter.
+
+        :param start: Start atribut of LogicItem
+        :param end:   End atribut of LogicItem
+
+        :return:   Found LogicItem
+        """
+
+        for logic_item in self.logic:
+            if start == logic_item.start and end == logic_item.end:
+                return logic_item
+        raise CachedProjectException(f"LogicItem in project {self.name} not found.")
+
+    def action_from_name(self, name: str) -> cmn.Action:
+        for action in self.actions:
+            if name == action.name:
+                return action
+        raise CachedProjectException(f"Action {name} in project {self.name} not found.")
 
-class UpdateableCachedProject(UpdateableMixin, CachedProject):
 
+class UpdateableCachedProject(UpdateableMixin, CachedProject):
     __slots__ = ()
 
     def __init__(self, project: cmn.Project | CachedProject):
         super().__init__(copy.deepcopy(project))
 
     def upsert_action(self, ap_id: str, action: cmn.Action) -> None:
-
         ap = self.bare_action_point(ap_id)
 
         if action.id in self._actions:
             assert self._actions[action.id].ap == ap
             self._actions[action.id].action = action
         else:
             self._actions[action.id] = ApAction(ap, action)
 
         self._upsert_child(ap.id, action.id)
         self.update_modified()
 
     def remove_action(self, action_id: str) -> cmn.Action:
-
         try:
             value = self._actions.pop(action_id)
         except KeyError as e:
             raise CachedProjectException("Action not found.") from e
 
         self._remove_child(value.ap.id, action_id)
         self.update_modified()
         return value.action
 
     def invalidate_joints(self, ap_id: str) -> None:
-
         for joints in self.ap_joints(ap_id):
             joints.is_valid = False
 
     def update_ap_position(self, ap_id: str, position: cmn.Position) -> None:
-
         ap = self.bare_action_point(ap_id)
         ap.position = position
         self.invalidate_joints(ap_id)
         self.update_modified()
 
     def upsert_orientation(self, ap_id: str, orientation: cmn.NamedOrientation) -> None:
-
         ap = self.bare_action_point(ap_id)
 
         if orientation.id in self._orientations:
             assert self._orientations[orientation.id].ap == ap
             self._orientations[orientation.id].orientation = orientation
         else:
             self._orientations[orientation.id] = ApOrientation(ap, orientation)
 
         self._upsert_child(ap_id, orientation.id)
         self.update_modified()
 
     def remove_orientation(self, orientation_id: str) -> cmn.NamedOrientation:
-
         try:
             value = self._orientations.pop(orientation_id)
         except KeyError as e:
             raise CachedProjectException("Orientation not found.") from e
 
         self._remove_child(value.ap.id, orientation_id)
         self.update_modified()
         return value.orientation
 
     def upsert_joints(self, ap_id: str, joints: cmn.ProjectRobotJoints) -> None:
-
         ap = self.bare_action_point(ap_id)
 
         if joints.id in self._joints:
             assert self._joints[joints.id].ap == ap
             self._joints[joints.id].joints = joints
         else:
             self._joints[joints.id] = ApJoints(ap, joints)
 
         self._upsert_child(ap_id, joints.id)
         self.update_modified()
 
     def remove_joints(self, joints_id: str) -> cmn.ProjectRobotJoints:
-
         try:
             value = self._joints.pop(joints_id)
         except KeyError as e:
             raise CachedProjectException("Joints not found.") from e
 
         self._remove_child(value.ap.id, joints_id)
         self.update_modified()
         return value.joints
 
     def upsert_action_point(
         self, ap_id: str, name: str, position: cmn.Position, parent: None | str = None
     ) -> cmn.BareActionPoint:
-
         try:
             ap = self.bare_action_point(ap_id)
             ap.name = name
             if position != ap.position:
                 self.invalidate_joints(ap_id)
             ap.position = position
             ap.parent = parent
@@ -701,15 +685,14 @@
             ap = cmn.BareActionPoint(name, position, parent, id=ap_id)
             self._action_points[ap_id] = ap
         self._upsert_child(parent, ap_id)
         self.update_modified()
         return ap
 
     def remove_action_point(self, ap_id: str) -> cmn.BareActionPoint:
-
         ap = self.bare_action_point(ap_id)
 
         for action in self.ap_actions(ap_id):
             self.remove_action(action.id)
 
         for joints in self.ap_joints(ap_id):
             self.remove_joints(joints.id)
@@ -719,37 +702,33 @@
 
         self._remove_child(ap.parent, ap_id)
         del self._action_points[ap_id]
         self.update_modified()
         return ap
 
     def upsert_logic_item(self, logic_item: cmn.LogicItem) -> None:
-
         self._logic_items[logic_item.id] = logic_item
         self.update_modified()
 
     def remove_logic_item(self, logic_item_id: str) -> cmn.LogicItem:
-
         try:
             logic_item = self._logic_items.pop(logic_item_id)
         except KeyError as e:
             raise CachedProjectException("Logic item not found.") from e
         self.update_modified()
         return logic_item
 
     def clear_logic(self) -> None:
-
         self._logic_items.clear()
         self.update_modified()
 
     def upsert_parameter(self, parameter: cmn.ProjectParameter) -> None:
         self._parameters[parameter.id] = parameter
         self.update_modified()
 
     def remove_parameter(self, parameter_id: str) -> cmn.ProjectParameter:
-
         try:
             param = self._parameters.pop(parameter_id)
         except KeyError as e:
             raise CachedProjectException("Project parameter not found.") from e
         self.update_modified()
         return param
```

### Comparing `arcor2-1.0.0rc1/arcor2/clients/aio_project_service.py` & `arcor2-1.1.0/arcor2/clients/aio_project_service.py`

 * *Files identical despite different names*

### Comparing `arcor2-1.0.0rc1/arcor2/clients/aio_scene_service.py` & `arcor2-1.1.0/arcor2/clients/aio_scene_service.py`

 * *Files identical despite different names*

### Comparing `arcor2-1.0.0rc1/arcor2/clients/asset.py` & `arcor2-1.1.0/arcor2/clients/asset.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from arcor2 import rest
 
 URL = os.getenv("ARCOR2_ASSET_SERVICE_URL", "http://0.0.0.0:10040")
 
 
 @dataclass
 class AssetInfo(JsonSchemaMixin):
-
     id: str
     type: str
     created: datetime
     modified: datetime
     file_path: Optional[str] = None
     file_name: Optional[str] = None
     name: Optional[str] = None
@@ -24,15 +23,14 @@
     directory_path: Optional[str] = None
     description: Optional[str] = None
     tags: Optional[list[str]] = None
     dependencies: Optional[list[str]] = None
 
 
 def asset_info() -> list[AssetInfo]:
-
     return rest.call(rest.Method.GET, f"{URL}/assets/info", list_return_type=AssetInfo)
 
 
 def asset_ids() -> set[str]:
     return {ai.id for ai in asset_info()}
 
 
@@ -65,14 +63,12 @@
         },
         files={"asset_data": (id, asset_data)},
         return_type=AssetInfo,
     )
 
 
 def delete_asset(id: str, remove_dependers: bool = False) -> None:
-
     rest.call(rest.Method.DELETE, f"{URL}/assets/{id}", params={"remove_dependers": remove_dependers})
 
 
 def asset_exists(id: str) -> bool:
-
     return rest.call(rest.Method.GET, f"{URL}/assets/{id}/exists", return_type=bool)
```

### Comparing `arcor2-1.0.0rc1/arcor2/clients/project_service.py` & `arcor2-1.1.0/arcor2/clients/project_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,14 @@
 @handle(ProjectServiceException, logger, message="Failed to list object types.")
 def get_object_type_ids() -> list[IdDesc]:
     return rest.call(rest.Method.GET, f"{URL}/object-types", list_return_type=IdDesc)
 
 
 @handle(ProjectServiceException, logger, message="Failed to add or update the object type.")
 def update_object_type(object_type: ObjectType) -> datetime:
-
     assert object_type.id
     return parse(rest.call(rest.Method.PUT, f"{URL}/object-types", body=object_type, return_type=str))
 
 
 @handle(ProjectServiceException, logger, message="Failed to delete the object type.")
 def delete_object_type(object_type_id: str) -> None:
     rest.call(rest.Method.DELETE, f"{URL}/object-types/{object_type_id}")
@@ -144,36 +143,33 @@
 @handle(ProjectServiceException, logger, message="Failed to get the project sources.")
 def get_project_sources(project_id: str) -> ProjectSources:
     return rest.call(rest.Method.GET, f"{URL}/projects/{project_id}/sources", return_type=ProjectSources)
 
 
 @handle(ProjectServiceException, logger, message="Failed to add or update the project.")
 def update_project(project: Project) -> datetime:
-
     assert project.id
     return parse(rest.call(rest.Method.PUT, f"{URL}/projects", return_type=str, body=project))
 
 
 @handle(ProjectServiceException, logger, message="Failed to add or update the project sources.")
 def update_project_sources(project_sources: ProjectSources) -> None:
-
     assert project_sources.id
     rest.call(rest.Method.PUT, f"{URL}/projects/sources", body=project_sources)
 
 
 @handle(ProjectServiceException, logger, message="Failed to delete the project.")
 def delete_project(project_id: str) -> None:
     rest.call(rest.Method.DELETE, f"{URL}/projects/{project_id}")
 
 
 @handle(ProjectServiceException, logger, message="Failed to clone the project.")
 def clone_project(
     project_id: str, new_project_name: str, new_description: None | str = None, new_project_id: None | str = None
 ) -> Project:
-
     if not new_project_id:
         new_project_id = Project.uid()
 
     params: dict[str, str] = {
         "project_id": project_id,
         "new_project_name": new_project_name,
         "new_project_id": new_project_id,
@@ -198,15 +194,14 @@
 @handle(ProjectServiceException, logger, message="Failed to get the scene.")
 def get_scene(scene_id: str) -> Scene:
     return rest.call(rest.Method.GET, f"{URL}/scenes/{scene_id}", return_type=Scene)
 
 
 @handle(ProjectServiceException, logger, message="Failed to add or update the scene.")
 def update_scene(scene: Scene) -> datetime:
-
     assert scene.id
     return parse(rest.call(rest.Method.PUT, f"{URL}/scenes", return_type=str, body=scene))
 
 
 @handle(ProjectServiceException, logger, message="Failed to delete the scene.")
 def delete_scene(scene_id: str) -> None:
     rest.call(rest.Method.DELETE, f"{URL}/scenes/{scene_id}")
```

### Comparing `arcor2-1.0.0rc1/arcor2/clients/scene_service.py` & `arcor2-1.1.0/arcor2/clients/scene_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,23 +20,21 @@
 
 class SceneServiceException(Arcor2Exception):
     pass
 
 
 @dataclass
 class MeshParameters(JsonSchemaMixin):
-
     mesh_scale_x: float = 1.0
     mesh_scale_y: float = 1.0
     mesh_scale_z: float = 1.0
     transform_id: str = "world"
 
 
 def wait_for(timeout: float = 10.0) -> None:
-
     start_time = time.monotonic()
     while time.monotonic() < start_time + timeout:
         try:
             started()
             return
         except SceneServiceException:
             time.sleep(1.0)
@@ -65,16 +63,15 @@
     params = model.to_dict()
     model_type = model.type().value.lower()
 
     params[f"{model_type}Id"] = model.id
     del params["id"]
 
     if model.type() == Model3dType.MESH:
-
-        params["meshFileId"] = params.pop("data_id")
+        params["meshFileId"] = params.pop("asset_id")
 
         if mesh_parameters:
             params.update(mesh_parameters.to_dict())
 
     rest.call(rest.Method.PUT, f"{URL}/collisions/{model_type}", body=pose, params=params)
 
 
@@ -100,15 +97,14 @@
     :param lc:
     :return:
     """
     return rest.call(rest.Method.PUT, f"{URL}/utils/line-safe", body=lc, return_type=LineCheckResult)
 
 
 def delete_all_collisions() -> None:
-
     for cid in collision_ids():
         delete_collision_id(cid)
 
 
 @handle(SceneServiceException, logger, message="Failed to start the scene.")
 def start(timeout: rest.OptTimeout = None) -> None:
     """To be called after all objects are created."""
```

### Comparing `arcor2-1.0.0rc1/arcor2/data/__init__.py` & `arcor2-1.1.0/arcor2/data/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 
 
 class DataException(Arcor2Exception):
     pass
 
 
 if not TYPE_CHECKING:
-
     # monkey-patch dataclasses_jsonschema to use orjson instead of json
 
     @classmethod
     def from_json(
         cls: type[dataclasses_jsonschema.T], data: str, validate: bool = True, **json_kwargs
     ) -> dataclasses_jsonschema.T:
         return cls.from_dict(orjson.loads(data), validate)
@@ -29,17 +28,15 @@
         return orjson.dumps(self.to_dict(omit_none, validate), **json_kwargs).decode()
 
     JsonSchemaMixin.from_json = from_json
     JsonSchemaMixin.to_json = to_json
 
 
 def resolve_schema_refs(self, data: dict) -> None:
-
     if "schema" in data:
-
         if "$ref" in data["schema"]:
             data["schema"]["$ref"] = _schema_reference(data["schema"]["$ref"], self._schema_type)
         elif "items" in data["schema"] and "$ref" in data["schema"]["items"]:
             data["schema"]["items"]["$ref"] = _schema_reference(data["schema"]["items"]["$ref"], self._schema_type)
     else:
         for key in data:
             if isinstance(data[key], dict):
@@ -55,19 +52,17 @@
     Force compilation of json schema (otherwise it might cause troubles later when executed in parallel)
     :return:
     """
 
     from arcor2 import data
 
     for _, module_name, _ in pkgutil.iter_modules(data.__path__):
-
         module = importlib.import_module(f"{data.__name__}.{module_name}")
 
         for _, obj in inspect.getmembers(module, inspect.isclass):
-
             if not issubclass(obj, JsonSchemaMixin) or obj is JsonSchemaMixin or inspect.isabstract(obj):
                 continue
 
             try:
                 obj.from_dict({})
             except ValidationError:
                 pass
```

### Comparing `arcor2-1.0.0rc1/arcor2/data/camera.py` & `arcor2-1.1.0/arcor2/data/camera.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,28 +4,25 @@
 from dataclasses_jsonschema import JsonSchemaMixin
 
 from arcor2.exceptions import Arcor2Exception
 
 
 @dataclass
 class CameraParameters(JsonSchemaMixin):
-
     fx: float
     fy: float
     cx: float
     cy: float
     dist_coefs: list[float]  # (k1,k2,p1,p2[,k3[,k4,k5,k6],[s1,s2,s3,s4]])
 
     def __post_init__(self) -> None:
-
         if len(self.dist_coefs) not in (4, 5, 8, 12):
             raise Arcor2Exception("Unsupported number of distortion coefficients.")
 
     def as_camera_matrix(self) -> np.ndarray:
-
         return np.array(
             [
                 [self.fx, 0.00000, self.cx],
                 [0.00000, self.fy, self.cy],
                 [0.00000, 0.00000, 1],
             ]
         )
```

### Comparing `arcor2-1.0.0rc1/arcor2/data/common.py` & `arcor2-1.1.0/arcor2/data/common.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 from dataclasses_jsonschema.type_defs import JsonDict, SchemaType
 
 from arcor2 import json
 from arcor2.exceptions import Arcor2Exception
 
 
 def uid(prefix: str) -> str:
-
     if not (prefix and prefix[0].isalpha() and prefix[-1] != "_"):
         raise Arcor2Exception(f"{prefix} is a invalid uid prefix.")
 
     return f"{prefix}_{uuid.uuid4().hex}"
 
 
 @unique
@@ -33,119 +32,106 @@
         return set(map(lambda c: c.value, cls))  # type: ignore
 
 
 @unique
 class IntEnum(int, Enum):
     @classmethod
     def set(cls) -> set[int]:
-        return set(map(lambda c: c.value, cls))  # type: ignore
+        return set(map(lambda c: c.value, cls))
 
 
 class FlowTypes(StrEnum):
-
     DEFAULT: str = "default"
 
 
 class LinkToActionOutput(NamedTuple):
     action_id: str
     flow_name: FlowTypes
     output_index: int
 
 
 def parse_link(val: str) -> LinkToActionOutput:
-
     try:
         action_id, flow_name, output_idx_str = val.split("/")
         return LinkToActionOutput(action_id, FlowTypes(flow_name), int(output_idx_str))
     except ValueError as e:
         raise Arcor2Exception("Invalid link value.") from e
 
 
 class DataClassEncoder(JSONEncoder):
     def default(self, o: Any) -> Any:
-
         if isinstance(o, JsonSchemaMixin):
             return o.to_dict()
 
         return super().default(o)
 
 
 @dataclass
 class IterableIndexable(JsonSchemaMixin):
     def __getitem__(self, item: int) -> float:
-
         attr = getattr(self, tuple(self.__dict__.keys())[item])
         assert isinstance(attr, (float, int))
         return attr
 
     def __iter__(self) -> Iterator[float]:
-
         # filtering items starting with _ is necessary to allow runtime monkey-patching
         # ...otherwise those patched attributes will appear in e.g. list(Position(1,2,3))
         yield from [v for k, v in self.__dict__.items() if not k.startswith("_")]
 
 
 @dataclass
 class Position(IterableIndexable):
-
     x: float = 0.0
     y: float = 0.0
     z: float = 0.0
 
     def rotated(self, ori: Orientation, inverse: bool = False) -> Position:
-
         q = ori.as_quaternion()
 
         if inverse:
             q = q.inverse()
 
         rotated_vector = quaternion.rotate_vectors([q], [list(self)])[0][0]
 
         return Position(rotated_vector[0], rotated_vector[1], rotated_vector[2])
 
     def __eq__(self, other: object) -> bool:
-
         if not isinstance(other, Position):
             return False
 
         return np.allclose(list(self), list(other), rtol=1.0e-6)
 
     def __add__(self, other: object) -> Position:
-
         if not isinstance(other, Position):
             raise Arcor2Exception("Not a position.")
 
         return Position(self.x + other.x, self.y + other.y, self.z + other.z)
 
     def __iadd__(self, other: object) -> Position:
-
         if not isinstance(other, Position):
             raise ValueError
 
         self.x += other.x
         self.y += other.y
         self.z += other.z
         return self
 
     def __sub__(self, other) -> Position:
-
         if not isinstance(other, Position):
             raise Arcor2Exception("Not a position.")
 
         return Position(self.x - other.x, self.y - other.y, self.z - other.z)
 
     def __mul__(self, other: object) -> Position:
-
         if not isinstance(other, (float, int)):
             raise ValueError
 
         return Position(self.x * other, self.y * other, self.z * other)
 
     def __imul__(self, other: object) -> Position:
-
         if not isinstance(other, (float, int)):
             raise ValueError
 
         self.x *= other
         self.y *= other
         self.z *= other
 
@@ -154,22 +140,20 @@
     def to_dict(
         self,
         omit_none: bool = True,
         validate: bool = False,
         validate_enums: bool = True,
         schema_type: SchemaType = DEFAULT_SCHEMA_TYPE,
     ) -> JsonDict:
-
         # orjson does not like numpy.float64
         return {"x": float(self.x), "y": float(self.y), "z": float(self.z)}
 
 
 @dataclass
 class Orientation(IterableIndexable):
-
     x: float = 0.0
     y: float = 0.0
     z: float = 0.0
     w: float = 1.0
 
     @classmethod
     def from_rotation_vector(cls, x: float = 0.0, y: float = 0.0, z: float = 0.0) -> Orientation:
@@ -177,15 +161,14 @@
 
     @classmethod
     def from_quaternion(cls, q: quaternion.quaternion) -> Orientation:
         return Orientation(q.x, q.y, q.z, q.w)
 
     @staticmethod
     def _normalized(q: quaternion.quaternion) -> quaternion.quaternion:
-
         nq = q.normalized()
 
         if nq.isnan():
             raise Arcor2Exception("Invalid quaternion.")
 
         return nq
 
@@ -195,15 +178,14 @@
     def inversed(self) -> Orientation:
         return self.from_quaternion(self.as_quaternion().inverse())
 
     def as_quaternion(self) -> quaternion.quaternion:
         return self._normalized(quaternion.quaternion(self.w, self.x, self.y, self.z))
 
     def set_from_quaternion(self, q: quaternion.quaternion) -> None:
-
         nq = self._normalized(q)
 
         self.x = nq.x
         self.y = nq.y
         self.z = nq.z
         self.w = nq.w
 
@@ -215,52 +197,47 @@
 
         arr = np.empty((4, 4))
         arr[:3, :3] = quaternion.as_rotation_matrix(self.as_quaternion())
         arr[3, :] = [0, 0, 0, 1]
         return arr
 
     def __eq__(self, other: object) -> bool:
-
         if not isinstance(other, Orientation):
             return False
 
         return cast(bool, quaternion.isclose(self.as_quaternion(), other.as_quaternion(), rtol=1.0e-6)[0])
 
     def __mul__(self, other: object) -> Orientation:
-
         if not isinstance(other, Orientation):
             raise ValueError
 
         return self.from_quaternion(self.as_quaternion() * other.as_quaternion())
 
     def __imul__(self, other: object) -> Orientation:
-
         if not isinstance(other, Orientation):
             raise ValueError
 
         self.set_from_quaternion(other.as_quaternion() * self.as_quaternion())
         return self
 
     def __post_init__(self):
-
         nq = self.as_quaternion()  # in order to get normalized quaternion
 
         self.x = nq.x
         self.y = nq.y
         self.z = nq.z
         self.w = nq.w
 
     def to_dict(
         self,
         omit_none: bool = True,
         validate: bool = False,
         validate_enums: bool = True,
         schema_type: SchemaType = DEFAULT_SCHEMA_TYPE,
     ) -> JsonDict:
-
         # orjson does not like numpy.float64
         return {"x": float(self.x), "y": float(self.y), "z": float(self.z), "w": float(self.w)}
 
 
 class ModelMixin(abc.ABC):
     """Mixin for objects with 'id' property that is uuid."""
 
@@ -282,15 +259,14 @@
     def __post_init__(self) -> None:
         if not self.id:
             self.id = self.uid()
 
 
 @dataclass
 class NamedOrientation(JsonSchemaMixin, ModelMixin):
-
     name: str
     orientation: Orientation
     id: str = ""
 
     @classmethod
     def uid_prefix(cls) -> str:
         return "ori"
@@ -299,61 +275,54 @@
         c = copy.deepcopy(self)
         c.id = self.uid()
         return c
 
 
 @dataclass
 class Pose(JsonSchemaMixin):
-
     position: Position = field(default_factory=Position)
     orientation: Orientation = field(default_factory=Orientation)
 
     def as_tr_matrix(self) -> np.ndarray:
-
         arr = np.empty((4, 4))
         arr[:3, :3] = quaternion.as_rotation_matrix(self.orientation.as_quaternion())
         arr[:3, 3] = list(self.position)
         arr[3, :] = [0, 0, 0, 1]
         return arr
 
     @staticmethod
     def from_tr_matrix(matrix: np.ndarray) -> Pose:
-
         tvec = matrix[:3, 3]
         return Pose(
             Position(tvec[0], tvec[1], tvec[2]),
             Orientation.from_quaternion(quaternion.from_rotation_matrix(matrix[:3, :3])),
         )
 
     def inversed(self) -> Pose:
-
         inv = self.orientation.inversed()
         return Pose((self.position * -1).rotated(inv), inv)
 
 
 @dataclass
 class ActionMetadata(JsonSchemaMixin):
-
     composite: bool = field(metadata=dict(description="Should be set for nested actions."), default=False)
     hidden: bool = field(metadata=dict(description="When set, action will be hidden in UIs."), default=False)
     cancellable: bool = field(
         init=False, default=False, metadata=dict(description="Defines whether action execution can be cancelled.")
     )
 
 
 @dataclass
 class Joint(JsonSchemaMixin):
-
     name: str
     value: float
 
 
 @dataclass
 class ProjectRobotJoints(JsonSchemaMixin, ModelMixin):
-
     name: str
     robot_id: str
     joints: list[Joint]
     is_valid: bool = False
     arm_id: Optional[str] = None
     end_effector_id: Optional[str] = None
     id: str = ""
@@ -366,23 +335,21 @@
         c = copy.deepcopy(self)
         c.id = self.uid()
         return c
 
 
 @dataclass
 class Parameter(JsonSchemaMixin):
-
     name: str
     type: str
     value: str
 
 
 @dataclass
 class SceneObject(JsonSchemaMixin, ModelMixin):
-
     name: str
     type: str
     pose: Optional[Pose] = None
     parameters: list[Parameter] = field(default_factory=list)
     id: str = ""
 
     @classmethod
@@ -393,15 +360,14 @@
         c = copy.deepcopy(self)
         c.id = self.uid()
         return c
 
 
 @dataclass
 class BareScene(JsonSchemaMixin, ModelMixin):
-
     name: str
     description: str = field(default_factory=str)
     created: Optional[datetime] = None
     modified: Optional[datetime] = None
     int_modified: Optional[datetime] = None
     id: str = ""
 
@@ -415,42 +381,38 @@
         c = copy.deepcopy(self)
         c.id = self.uid()
         return c
 
 
 @dataclass
 class Scene(BareScene):
-
     objects: list[SceneObject] = field(default_factory=list)
 
     @staticmethod
     def from_bare(bare: BareScene) -> Scene:
         return Scene(bare.name, bare.description, bare.created, bare.modified, bare.int_modified, id=bare.id)
 
 
 @dataclass
 class IdValue(JsonSchemaMixin):
-
     id: str
     value: str
 
 
 class ActionParameterException(Arcor2Exception):
     pass
 
 
 @dataclass
 class ActionParameter(Parameter):
     class TypeEnum(StrEnum):
-
         PROJECT_PARAMETER: str = "project_parameter"
         LINK: str = "link"
 
     def str_from_value(self) -> str:
-
         val = json.loads(self.value)
 
         if not isinstance(val, str):
             raise Arcor2Exception("Value should be string.")
 
         return val
 
@@ -462,27 +424,24 @@
 
     def is_value(self) -> bool:
         return self.type not in self.TypeEnum.set()
 
 
 @dataclass
 class Flow(JsonSchemaMixin):
-
     type: FlowTypes = FlowTypes.DEFAULT
     outputs: list[str] = field(default_factory=list)  # can't be set as it is unordered
 
     def __post_init__(self) -> None:
-
         if len(self.outputs) > len(set(self.outputs)):
             raise Arcor2Exception("Outputs have to be unique.")
 
 
 @dataclass
 class BareAction(JsonSchemaMixin, ModelMixin):
-
     name: str
     type: str
     id: str = ""
 
     @classmethod
     def uid_prefix(cls) -> str:
         return "act"
@@ -494,52 +453,47 @@
         c.id = self.uid()
         return c
 
 
 @dataclass
 class Action(BareAction):
     class ParsedType(NamedTuple):
-
         obj_id: str
         action_type: str
 
     parameters: list[ActionParameter] = field(default_factory=list)
     flows: list[Flow] = field(default_factory=list)
 
     def parse_type(self) -> ParsedType:
-
         try:
             obj_id_str, action = self.type.split("/")
         except ValueError:
             raise Arcor2Exception(f"Action: {self.id} has invalid type: {self.type}.")
         return self.ParsedType(obj_id_str, action)
 
     def parameter(self, parameter_id: str) -> ActionParameter:
-
         for param in self.parameters:
             if parameter_id == param.name:
                 return param
 
         raise Arcor2Exception("Param not found")
 
     @property
     def bare(self) -> BareAction:
         return BareAction(self.name, self.type, id=self.id)
 
     def flow(self, flow_type: FlowTypes = FlowTypes.DEFAULT) -> Flow:
-
         for flow in self.flows:
             if flow.type == flow_type:
                 return flow
         raise Arcor2Exception(f"Flow '{flow_type.value}' not found.")
 
 
 @dataclass
 class BareActionPoint(JsonSchemaMixin, ModelMixin):
-
     name: str
     position: Position
     parent: Optional[str] = None
     display_name: Optional[str] = None
     description: Optional[str] = None
     id: str = ""
 
@@ -553,52 +507,48 @@
         c = copy.deepcopy(self)
         c.id = self.uid()
         return c
 
 
 @dataclass
 class ActionPoint(BareActionPoint):
-
     orientations: list[NamedOrientation] = field(default_factory=list)
     robot_joints: list[ProjectRobotJoints] = field(default_factory=list)
     actions: list[Action] = field(default_factory=list)
 
     @staticmethod
     def from_bare(bare: BareActionPoint) -> ActionPoint:
         return ActionPoint(bare.name, bare.position, bare.parent, bare.display_name, bare.description, id=bare.id)
 
 
 @dataclass
 class ProjectLogicIf(JsonSchemaMixin):
-
     what: str
     value: str
 
     def parse_what(self) -> LinkToActionOutput:
         return parse_link(self.what)
 
 
 @dataclass
 class LogicItem(JsonSchemaMixin, ModelMixin):
     class ParsedStart(NamedTuple):
-
         start_action_id: str
         start_flow: str
 
     # TODO can't be ClassVar because of https://github.com/s-knibbs/dataclasses-jsonschema/issues/176
     START = "START"
     END = "END"
 
     start: str
     end: str
     condition: Optional[ProjectLogicIf] = None
     id: str = ""
 
     def parse_start(self) -> ParsedStart:
-
         try:
             start_action_id, start_flow = self.start.split("/")
         except ValueError:
             return self.ParsedStart(self.start, FlowTypes.DEFAULT)
 
         return self.ParsedStart(start_action_id, start_flow)
 
@@ -618,47 +568,43 @@
 
     min: float
     max: float
 
 
 @dataclass
 class ProjectParameter(Parameter, ModelMixin):
-
     range: Optional[Range] = None  # TODO use it in parameter plugins?
     display_name: Optional[str] = None
     description: Optional[str] = None
     id: str = ""
 
     @classmethod
     def uid_prefix(cls) -> str:
         return "pco"
 
 
 @dataclass
 class FunctionReturns(JsonSchemaMixin):
-
     type: str
     link: str
 
 
 @dataclass
 class ProjectFunction(JsonSchemaMixin, ModelMixin):
-
     name: str
     actions: list[Action] = field(default_factory=list)
     logic: list[LogicItem] = field(default_factory=list)
     parameters: list[ActionParameter] = field(default_factory=list)
     returns: list[FunctionReturns] = field(default_factory=list)
     id: str = ""
 
     def action_ids(self) -> set[str]:
         return {act.id for act in self.actions}
 
     def action(self, action_id: str) -> Action:
-
         for ac in self.actions:
             if ac.id == action_id:
                 return ac
         else:
             raise Arcor2Exception("Action not found")
 
     @classmethod
@@ -669,22 +615,20 @@
         c = copy.deepcopy(self)
         c.id = self.uid()
         return c
 
 
 @dataclass
 class SceneObjectOverride(JsonSchemaMixin):
-
     id: str  # object id
     parameters: list[Parameter]
 
 
 @dataclass
 class BareProject(JsonSchemaMixin, ModelMixin):
-
     name: str
     scene_id: str
     description: str = field(default_factory=str)
     has_logic: bool = True
     created: Optional[datetime] = None
     modified: Optional[datetime] = None
     int_modified: Optional[datetime] = None
@@ -700,15 +644,14 @@
         c = copy.deepcopy(self)
         c.id = self.uid()
         return c
 
 
 @dataclass
 class Project(BareProject):
-
     action_points: list[ActionPoint] = field(default_factory=list)
     parameters: list[ProjectParameter] = field(default_factory=list)
     functions: list[ProjectFunction] = field(default_factory=list)
     logic: list[LogicItem] = field(default_factory=list)
     object_overrides: list[SceneObjectOverride] = field(default_factory=list)
     project_objects_ids: Optional[list[str]] = None  # not used at the moment
 
@@ -721,18 +664,66 @@
             bare.has_logic,
             bare.created,
             bare.modified,
             bare.int_modified,
             id=bare.id,
         )
 
+    def print_actions(self):
+        """Print all actions from project with their specific action_point."""
+
+        count = 1
+        for action_point in self.action_points:
+            print(f"||-----------||{action_point.name}||------------||\n")
+            for action in action_point.actions:
+                print(f"----------------Action {count}-----------------")
+                print("Name:\t" + action.name)
+                print("Type:\t" + action.type)
+                print("Id:\t" + action.id)
+                print("Param:\t")
+                for param in action.parameters:
+                    print("\t", end="")
+                    print(param)
+                print("Flows:\t")
+                for flow in action.flows:
+                    print("\t", end="")
+                    print(flow)
+                print()
+                count += 1
+
+    def print_logic_items(self):
+        """Print all LogicItems from project."""
+
+        count = 1
+        for item in self.logic:
+            print(f"----------------Logic {count}-----------------")
+            print("Start:\t" + item.start)
+            print("End:\t" + item.end)
+            print("Con:\t", end="")
+            print(item.condition)
+            print("Id:\t" + item.id)
+            print()
+            count += 1
+
+    def find_action_point(self, action_point_id: str) -> ActionPoint | None:
+        """find action_point with specific id in project.
+
+        :action_point_id:   Id of action_point
+
+        :return:            Found ActionPoint or None
+        """
+
+        for action_point in self.action_points:
+            if action_point.id == action_point_id:
+                return action_point
+        return None
+
 
 @dataclass
 class ProjectSources(JsonSchemaMixin):
-
     id: str  # project_id
     script: str
 
 
 @dataclass
 class IdDesc(JsonSchemaMixin):
     id: str
@@ -740,15 +731,14 @@
     created: datetime
     modified: datetime
     description: Optional[str] = None
 
 
 @dataclass
 class BroadcastInfo(JsonSchemaMixin):
-
     host: str
     port: int
 
 
 @dataclass
 class Error(JsonSchemaMixin):
     code: int
@@ -763,7 +753,63 @@
     message: str
     type: str
     description: str
     content: Optional[str] = None
 
     def __str__(self):
         return f"{self.service} ({self.type}): {self.message}"
+
+
+@dataclass
+class Direction(JsonSchemaMixin):
+    x: float = 0.0
+    y: float = 0.0
+    z: float = 0.0
+
+    @classmethod
+    def from_position(cls, position: Position) -> Direction:
+        return Direction(position.x, position.y, position.z)
+
+
+class BodyJointId(IntEnum):
+    PELVIS = 0
+    SPINE_NAVEL = 1
+    SPINE_CHEST = 2
+    NECK = 3
+    CLAVICLE_LEFT = 4
+    SHOULDER_LEFT = 5
+    ELBOW_LEFT = 6
+    WRIST_LEFT = 7
+    HAND_LEFT = 8
+    HANDTIP_LEFT = 9
+    THUMB_LEFT = 10
+    CLAVICLE_RIGHT = 11
+    SHOULDER_RIGHT = 12
+    ELBOW_RIGHT = 13
+    WRIST_RIGHT = 14
+    HAND_RIGHT = 15
+    HANDTIP_RIGHT = 16
+    THUMB_RIGHT = 17
+    HIP_LEFT = 18
+    KNEE_LEFT = 19
+    ANKLE_LEFT = 20
+    FOOT_LEFT = 21
+    HIP_RIGHT = 22
+    KNEE_RIGHT = 23
+    ANKLE_RIGHT = 24
+    FOOT_RIGHT = 25
+    HEAD = 26
+    NOSE = 27
+    EYE_LEFT = 28
+    EAR_LEFT = 29
+    EYE_RIGHT = 30
+    EAR_RIGHT = 31
+
+    @classmethod
+    def from_str_or_default(cls, maybe_str: str | None) -> BodyJointId:
+        if maybe_str is None:
+            return cls.SPINE_CHEST
+        try:
+            val = int(maybe_str)
+            return cls(val)
+        except (TypeError, ValueError):
+            return cls.SPINE_CHEST
```

### Comparing `arcor2-1.0.0rc1/arcor2/data/events.py` & `arcor2-1.1.0/arcor2/data/events.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,14 @@
 # ----------------------------------------------------------------------------------------------------------------------
 
 
 @dataclass
 class ActionStateBefore(Event):
     @dataclass
     class Data(JsonSchemaMixin):
-
         # required for projects with logic (where actions are defined in the project)
         # might be also filled for projects without logic
         action_id: Optional[str] = None
         parameters: Optional[list[str]] = None
 
         # required for projects with logic
         # might or might not be set in other cases
@@ -133,12 +132,11 @@
 # ----------------------------------------------------------------------------------------------------------------------
 
 
 @dataclass
 class ActionStateAfter(Event):
     @dataclass
     class Data(JsonSchemaMixin):
-
         action_id: str
         results: Optional[list[str]] = None
 
     data: Data
```

### Comparing `arcor2-1.0.0rc1/arcor2/data/object_type.py` & `arcor2-1.1.0/arcor2/data/object_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,91 +6,81 @@
 from dataclasses_jsonschema import JsonSchemaMixin
 
 from arcor2.data import DataException
 from arcor2.data.common import Pose
 
 
 class Model3dType(Enum):
-
     NONE: str = "None"
     BOX: str = "Box"
     CYLINDER: str = "Cylinder"
     SPHERE: str = "Sphere"
     MESH: str = "Mesh"
 
 
 @dataclass
 class MetaModel3d(JsonSchemaMixin):
-
     id: str
     type: Model3dType
 
     def __post_init__(self) -> None:
-
         if isinstance(self.type, str):
             self.type = Model3dType[self.type.upper()]
 
 
 @dataclass
 class Model(JsonSchemaMixin):
-
     id: str
 
     @classmethod
     def type(cls) -> Model3dType:
         return Model3dType[cls.__name__.upper()]
 
     def metamodel(self) -> MetaModel3d:
         return MetaModel3d(self.id, self.type())
 
 
 @dataclass
 class Box(Model):
-
     size_x: float
     size_y: float
     size_z: float
 
     def __post_init__(self) -> None:
-
         dims = [self.size_x, self.size_y, self.size_z]
 
         if [val for val in dims if val < 0]:
             raise DataException("Dimensions has to be positive.")
 
         if len([val for val in dims if val > 0]) < 2:
             raise DataException("Only one dimension of a box can be zero.")
 
 
 @dataclass
 class Cylinder(Model):
-
     radius: float
     height: float
 
     def __post_init__(self) -> None:
-
         if [val for val in [self.radius, self.height] if val <= 0]:
             raise DataException("Dimensions has to be positive.")
 
 
 @dataclass
 class Sphere(Model):
     radius: float
 
     def __post_init__(self) -> None:
-
         if self.radius <= 0:
             raise DataException("Radius has to be positive.")
 
 
 @dataclass
 class Mesh(Model):
-
-    data_id: str
+    asset_id: str
     focus_points: Optional[list[Pose]] = None
 
 
 MeshList = list[Mesh]
 
 PrimitiveModels = Box | Sphere | Cylinder
 Models = Box | Sphere | Cylinder | Mesh
@@ -114,56 +104,50 @@
     description: Optional[str] = None
     model: Optional[MetaModel3d] = None
 
     created: Optional[datetime] = None
     modified: Optional[datetime] = None
 
     def __post_init__(self) -> None:
-
         self.name = self.id  # name makes no sense for ObjectType but is required by the Project service
 
         # TODO workaround for bug (?) in Project service
         if self.model and self.model.type == Model3dType.NONE:
             self.model = None
 
 
 @dataclass
 class ObjectModel(JsonSchemaMixin):
-
     type: Model3dType
     box: Optional[Box] = None
     cylinder: Optional[Cylinder] = None
     sphere: Optional[Sphere] = None
     mesh: Optional[Mesh] = None
 
     def model(self) -> Models:
-
         assert self.type != Model3dType.NONE
         return getattr(self, str(self.type.value).lower())
 
     def __post_init__(self) -> None:
-
         models_list = [self.box, self.cylinder, self.sphere, self.mesh]
 
         if models_list.count(None) != len(models_list) - 1:
             raise DataException("No model specified!")
 
 
 @dataclass
 class CollisionModels(JsonSchemaMixin):
-
     boxes: list[Box] = field(default_factory=list)
     spheres: list[Sphere] = field(default_factory=list)
     cylinders: list[Cylinder] = field(default_factory=list)
     meshes: list[Mesh] = field(default_factory=list)
 
 
 @dataclass
 class ParameterMeta(JsonSchemaMixin):
-
     name: str
     type: str
     dynamic_value: bool = False  # client should ask for allowed values using RPC
     dynamic_value_parents: Optional[set[str]] = None
     description: Optional[str] = None
     default_value: Optional[str] = None
     extra: Optional[str] = None
```

### Comparing `arcor2-1.0.0rc1/arcor2/data/rpc/common.py` & `arcor2-1.1.0/arcor2/data/rpc/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,24 +11,22 @@
 
 
 class RPC:
     """Base class for all RPCs."""
 
     @dataclass
     class Request(Arcor2Mixin):  # TODO from_dict -> check that request key is == to qualname
-
         id: int
         request: str = field(init=False)
 
         def __post_init__(self) -> None:
             self.request = self.get_qualname()
 
     @dataclass
     class Response(Arcor2Mixin):
-
         id: int = 0
         response: str = field(init=False)
         result: bool = True
         messages: Optional[list[str]] = None
         # TODO define data here somehow? And check that if result==True there are some data
 
         def __post_init__(self) -> None:
@@ -47,15 +45,14 @@
 class IdArgs(JsonSchemaMixin):
     id: str
 
 
 @dataclass
 class RobotArg(JsonSchemaMixin):
     class RobotArgTuple(NamedTuple):
-
         robot_id: str
         end_effector: str
         arm_id: Optional[str] = None
 
     robot_id: str = field(metadata=dict(description="Object id of the robot or robot_id within the robot service."))
     end_effector: str
     arm_id: Optional[str] = None
```

### Comparing `arcor2-1.0.0rc1/arcor2/data/scene.py` & `arcor2-1.1.0/arcor2/data/scene.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,29 +5,25 @@
 
 from arcor2.data.common import Position
 from arcor2.exceptions import Arcor2Exception
 
 
 @dataclass
 class MeshFocusAction(JsonSchemaMixin):
-
     mesh_focus_points: list[Position]
     robot_space_points: list[Position]
 
     def __post_init__(self) -> None:
-
         if len(self.mesh_focus_points) != len(self.robot_space_points):
             raise Arcor2Exception("Invalid MeshFocusAction.")
 
 
 @dataclass
 class LineCheck(JsonSchemaMixin):
-
     pt1: Position
     pt2: Position
 
 
 @dataclass
 class LineCheckResult(JsonSchemaMixin):
-
     safe: bool
     object_id: Optional[str] = None
```

### Comparing `arcor2-1.0.0rc1/arcor2/docstring.py` & `arcor2-1.1.0/arcor2/docstring.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 class Docstring:
     short_description: None | str = None
     long_description: None | str = None
     params: None | dict[str, str] = None
     returns: None | str = None
 
     def param(self, name: str) -> None | str:
-
         if not self.params:
             return None
 
         return self.params.get(name, None)
 
 
 def trim(docstring: str) -> str:
```

### Comparing `arcor2-1.0.0rc1/arcor2/env.py` & `arcor2-1.1.0/arcor2/env.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,28 +8,26 @@
 
 
 def get_bool(variable_name: str, default: bool = False) -> bool:
     return os.getenv(variable_name, str(default)).lower() in ("true", "1")
 
 
 def get_int(variable_name: str, default: None | int = None) -> int:
-
     val = os.getenv(variable_name, default)
 
     if val is None:
         raise Arcor2EnvException(f"Variable {variable_name} is not set.")
 
     try:
         return int(val)
     except ValueError:
         raise Arcor2EnvException(f"Variable {variable_name} has invalid value: {val}.")
 
 
 def get_float(variable_name: str, default: None | float = None) -> float:
-
     val = os.getenv(variable_name, default)
 
     if val is None:
         raise Arcor2EnvException(f"Variable {variable_name} is not set.")
 
     try:
         return float(val)
```

### Comparing `arcor2-1.0.0rc1/arcor2/exceptions/helpers.py` & `arcor2-1.1.0/arcor2/exceptions/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
     logger: logging.Logger,
     except_type: type[Arcor2Exception] = Arcor2Exception,
     message: None | str = None,
 ) -> Callable[[F], F]:
     def _handle_exceptions(func: F) -> F:
         @functools.wraps(func)
         def wrapper(*args, **kwargs) -> Any:
-
             try:
                 return func(*args, **kwargs)
             except except_type as e:
                 if message is not None:
                     logger.error(f"{message} {str(e)}")
                     raise raise_type(message) from e
                 else:
```

### Comparing `arcor2-1.0.0rc1/arcor2/flask.py` & `arcor2-1.1.0/arcor2/flask.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 import logging
 import traceback
 from dataclasses import dataclass, field
+from http import HTTPStatus
 from typing import Optional, Type, TypeAlias, Union, cast
 
 from apispec import APISpec
 from apispec_webframeworks.flask import FlaskPlugin
 from dataclasses_jsonschema import DEFAULT_SCHEMA_TYPE, FieldMeta, JsonSchemaMixin
 from dataclasses_jsonschema.apispec import DataclassesPlugin
 from flask import Flask, Response, jsonify
@@ -110,14 +111,22 @@
                     default=None,
                 ).as_dict
             )
 
         return cast(Type[IWebApiError], WebApiError)
 
 
+class DataclassResponse(Response):
+    """Wrapper around flask.Response that creates Response from provided
+    dataclass as json and sets mimetype to 'application/json'."""
+
+    def __init__(self, dc: JsonSchemaMixin, status: int = HTTPStatus.OK, **kwargs) -> None:
+        super().__init__(response=dc.to_json(), status=status, mimetype="application/json", **kwargs)
+
+
 def create_app(import_name: str) -> Flask:
     app = Flask(import_name)
     CORS(app)
     return app
 
 
 def run_app(
```

### Comparing `arcor2-1.0.0rc1/arcor2/helpers.py` & `arcor2-1.1.0/arcor2/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,14 @@
     # ...not supported by mypy at the moment, see https://github.com/python/mypy/issues/8645
 
     try:
         return await asyncio.get_event_loop().run_in_executor(executor, func, *args)
     except Arcor2Exception:
         raise
     except Exception as e:
-
         if propagate:
             for etp in propagate:
                 if isinstance(e, etp):
                     raise
 
         # all code should raise exceptions based on Arcor2Exception so this is just a guard against a buggy code
         raise Arcor2Exception(f"Unhandled exception in {func.__name__}.") from e
@@ -161,15 +160,14 @@
     if not issubclass(cls, output_type):
         raise ImportClsException(f"{cls.__name__} is not subclass of {output_type.__name__}.")
 
     return cls
 
 
 def check_compatibility(my_version: str, their_version: str) -> None:
-
     try:
         mv = parse(my_version)
         tv = parse(their_version)
     except ValueError as e:
         raise Arcor2Exception from e
 
     if not isinstance(mv, Version):
@@ -206,15 +204,14 @@
 
     def __exit__(self, exc_type, exc_value, traceback) -> None:
         self._lock.release()
         return None
 
 
 def port_from_url(url: str) -> int:
-
     return int(url.strip().split(":")[-1])
 
 
 def find_free_port() -> int:
     with closing(socket.socket(socket.AF_INET, socket.SOCK_STREAM)) as s:
         s.bind(("localhost", 0))
         s.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
```

### Comparing `arcor2-1.0.0rc1/arcor2/image.py` & `arcor2-1.1.0/arcor2/image.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,20 +7,18 @@
 
 from arcor2 import json
 
 ENCODING = "latin-1"
 
 
 def image_to_cv2(pil_image: Image, mode=cv2.COLOR_RGB2BGR) -> np.ndarray:
-
     return cv2.cvtColor(np.array(pil_image), mode)
 
 
 def image_to_bytes_io(value: Image, target_format: str = "jpeg", target_mode: None | str = None) -> io.BytesIO:
-
     output = io.BytesIO()
 
     if target_mode and value.mode != target_mode:
         rgb_im = value.convert(target_mode)
         rgb_im.save(output, target_format)
     else:
         value.save(output, target_format)
```

### Comparing `arcor2-1.0.0rc1/arcor2/json.py` & `arcor2-1.1.0/arcor2/json.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,30 +12,27 @@
 JsonType = bool | str | int | float | dict[str, Any] | Sequence[Any] | None
 
 
 T = TypeVar("T")
 
 
 def loads(value: str) -> JsonType:
-
     try:
         return orjson.loads(value)
     except (ValueError, TypeError) as e:
         raise JsonException(f"Not a JSON. {str(e)}") from e
 
 
 def loads_type(value: str, output_type: type[T]) -> T:
-
     val = loads(value)
 
     if not isinstance(val, output_type):
         raise JsonException("Not an expected type.")
 
     return val
 
 
 def dumps(value: JsonType) -> str:
-
     try:
         return orjson.dumps(value).decode()
     except (ValueError, TypeError) as e:
         raise JsonException(f"Not a JSON. {str(e)}") from e
```

### Comparing `arcor2-1.0.0rc1/arcor2/logging.py` & `arcor2-1.1.0/arcor2/logging.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,32 +17,29 @@
 
 
 DEFAULT_DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 DEFAULT_LOG_FORMAT = "%(asctime)s %(log_color)s%(levelname)-8s%(reset)s %(message)s"
 
 
 def logger_formatter(log_format=DEFAULT_LOG_FORMAT, date_format=DEFAULT_DATE_FORMAT) -> logging.Formatter:
-
     return colorlog.ColoredFormatter(log_format, date_format)
 
 
 def get_aiologger(
     name: str,
     level: aiologger.levels.LogLevel = aiologger.levels.LogLevel.INFO,
     formatter: None | logging.Formatter = None,
 ) -> aiologger.Logger:
-
     if formatter is None:
         formatter = logger_formatter()
 
     return aiologger.Logger.with_default_handlers(name=name, formatter=formatter, level=level)
 
 
 def get_logger(name: str, level: int = logging.INFO) -> logging.Logger:
-
     logger = logging.getLogger(name)
 
     ch = logging.StreamHandler()
     ch.setFormatter(logger_formatter())
     logger.setLevel(level)
     logger.addHandler(ch)
```

### Comparing `arcor2-1.0.0rc1/arcor2/logic.py` & `arcor2-1.1.0/arcor2/logic.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,32 +13,29 @@
 
     :param parent:
     :param first_action_id:
     :return:
     """
 
     def _check_for_loops(action: Action, visited_actions: set[str]) -> None:
-
         if action.id in visited_actions:
             raise Arcor2Exception("Loop detected!")
 
         visited_actions.add(action.id)
 
         _, outputs = parent.action_io(action.id)
 
         for output in outputs:
-
             if output.end == output.END:
                 continue
 
             # each possible execution path have its own set of visited actions
             _check_for_loops(parent.action(output.end), visited_actions.copy())
 
     if first_action_id is None:
-
         try:
             first_action_id = parent.first_action_id()
         except CachedProjectException as e:
             raise Arcor2Exception("Can't check unfinished logic.") from e
 
     first_action = parent.action(first_action_id)
```

### Comparing `arcor2-1.0.0rc1/arcor2/object_types/abstract.py` & `arcor2-1.1.0/arcor2/object_types/abstract.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,14 @@
     """Generic object."""
 
     DYNAMIC_PARAMS: DynamicParamDict = {}
     CANCEL_MAPPING: CancelDict = {}
     _ABSTRACT = True
 
     def __init__(self, obj_id: str, name: str, settings: None | Settings = None) -> None:
-
         self.id = obj_id
         self.name = name
 
         if settings is None:
             settings = Settings()
         self._settings = settings
 
@@ -82,15 +81,14 @@
     def __init__(
         self,
         obj_id: str,
         name: str,
         pose: Pose,
         settings: None | Settings = None,
     ) -> None:
-
         super(GenericWithPose, self).__init__(obj_id, name, settings)
         self._pose = pose
 
     def scene_object(self) -> SceneObject:
         return SceneObject(self.name, self.__class__.__name__, self._pose, id=self.id)
 
     @property
@@ -98,60 +96,52 @@
         """Returns pose of the object.
 
         When set, pose of the collision model is updated on the Scene service.
         :return:
         """
         return self._pose
 
-    @pose.setter
-    def pose(self, pose: Pose) -> None:
+    def set_pose(self, pose: Pose) -> None:
         self._pose = pose
 
     def update_pose(self, new_pose: Pose, *, an: None | str = None) -> None:
         """Enables control over object's pose in the world.
 
         :param new_pose: New pose for the object.
         :return:
         """
 
-        self.pose = new_pose
+        self.set_pose(new_pose)
 
     update_pose.__action__ = ActionMetadata()  # type: ignore
 
 
 class CollisionObject(GenericWithPose):
-
     # name of the file that should be uploaded to the Project service together with this ObjectType
     mesh_filename: None | str = None
 
     def __init__(
         self,
         obj_id: str,
         name: str,
         pose: Pose,
         collision_model: Models,
         settings: None | Settings = None,
     ) -> None:
-
         super().__init__(obj_id, name, pose, settings)
 
         self.collision_model = copy.deepcopy(collision_model)
         self._enabled = True
 
         # originally, each model has id == object type (e.g. BigBox) but here we need to set it to something unique
         self.collision_model.id = self.id
         scene_service.upsert_collision(self.collision_model, pose)
 
-    @property  # workaround for https://github.com/python/mypy/issues/5936
-    def pose(self) -> Pose:
-        return super().pose
-
-    @pose.setter
-    def pose(self, pose: Pose) -> None:
-        self._pose = pose  # TODO how to set it through super() correctly?
+    def set_pose(self, pose: Pose) -> None:
+        super().set_pose(pose)
         if self._enabled:
             scene_service.upsert_collision(self.collision_model, pose)
 
     @property
     def enabled(self) -> bool:
         """If the object has a collision model, this indicates whether the
         model is enabled (set on the Scene service).
@@ -161,15 +151,14 @@
         """
 
         assert self.id in scene_service.collision_ids() == self._enabled
         return self._enabled
 
     @enabled.setter
     def enabled(self, enabled: bool) -> None:
-
         if not self._enabled and enabled:
             assert self.id not in scene_service.collision_ids()
             scene_service.upsert_collision(self.collision_model, self.pose)
         if self._enabled and not enabled:
             scene_service.delete_collision_id(self.id)
         self._enabled = enabled
 
@@ -192,15 +181,14 @@
         self,
         obj_id: str,
         name: str,
         pose: Pose,
         collision_model: PrimitiveModels,
         settings: None | Settings = None,
     ) -> None:
-
         if settings and not isinstance(settings, Settings):
             # TODO rather remove settings from __init__ (requires non-trivial changes in ARServer/Resources)
             raise Arcor2Exception(f"Settings are not supported for {VirtualCollisionObject.__name__}.")  # noqa:PB10
 
         super().__init__(obj_id, name, pose, collision_model)
 
 
@@ -386,15 +374,14 @@
         """
 
         if self.move_in_progress:  # this holds for all arms
             raise RobotException("Already moving.")
 
         # hand-teaching mode is arm specific
         for arm_id in self.get_arm_ids():
-
             try:
                 if self.get_hand_teaching_mode(arm_id):
                     raise RobotException("Can't move in hand teaching mode.")
             except Arcor2NotImplemented:
                 pass
 
     def move_to_pose(
```

### Comparing `arcor2-1.0.0rc1/arcor2/object_types/flow_actions.py` & `arcor2-1.1.0/arcor2/object_types/flow_actions.py`

 * *Files identical despite different names*

### Comparing `arcor2-1.0.0rc1/arcor2/object_types/logic_actions.py` & `arcor2-1.1.0/arcor2/object_types/logic_actions.py`

 * *Files identical despite different names*

### Comparing `arcor2-1.0.0rc1/arcor2/object_types/random_actions.py` & `arcor2-1.1.0/arcor2/object_types/random_actions.py`

 * *Files identical despite different names*

### Comparing `arcor2-1.0.0rc1/arcor2/object_types/time_actions.py` & `arcor2-1.1.0/arcor2/object_types/time_actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,14 @@
     _ABSTRACT = False
 
     def __init__(self, obj_id: str, name: str, settings: None | Settings = None) -> None:
         super(TimeActions, self).__init__(obj_id, name, settings)
         self._last_time: None | float = None
 
     def sleep(self, seconds: float = 1.0, *, an: None | str = None) -> None:
-
         assert 0.0 <= seconds <= 10.0e6
 
         time.sleep(seconds)
 
     def rate(self, period: float = 1.0, *, an: None | str = None) -> None:
         """Can be used to maintain desired rate of the loop. Should be the
         first action.
@@ -28,15 +27,14 @@
         """
 
         assert 0.0 <= period <= 10.0e6
 
         now = time.monotonic()
 
         if self._last_time is not None:
-
             dif = self._last_time + period - now
 
             if dif > 0:
                 time.sleep(dif)
 
         self._last_time = now
```

### Comparing `arcor2-1.0.0rc1/arcor2/object_types/upload.py` & `arcor2-1.1.0/arcor2/object_types/upload.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,21 +12,19 @@
 
 
 class UploadException(Arcor2Exception):
     pass
 
 
 class Urdf(NamedTuple):
-
     path_to_directory: str  # path to a URDF package directory
     archive_name: str  # resulting archive name
 
 
 def upload_whatever(type_def: type[object]) -> None:
-
     obj_type = ObjectType(id=type_def.__name__, source=get_containing_module_sources(type_def))
     print(f"Storing '{obj_type.id}'...")
     ps.update_object_type(obj_type)
 
 
 def upload_def(
     type_def: type[Generic],
@@ -61,15 +59,14 @@
 
         if model.id != obj_type.id:
             raise UploadException("Model id have to be the same as ObjectType id.")
 
         obj_type.model = model.metamodel()
 
         if isinstance(model, Mesh):
-
             if not type_def.mesh_filename:
                 raise UploadException("Mesh filename not set.")
 
             if not file_to_upload:
                 raise UploadException("For mesh collision model, file_to_upload parameter have to be set.")
 
             try:
@@ -86,15 +83,14 @@
         ps.put_model(model)
 
     else:
         if model:
             raise UploadException("Parameter 'model' set for non-CollisionObject.")
 
     if urdf:
-
         if not os.path.isdir(urdf.path_to_directory):
             print(f"{urdf.path_to_directory} is not a directory.")
             return
 
         print(f"Storing URDF package for '{obj_type.id}'.")
 
         paths: list[str] = []
```

### Comparing `arcor2-1.0.0rc1/arcor2/object_types/utils.py` & `arcor2-1.1.0/arcor2/object_types/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,28 +49,26 @@
     # TODO some more (simple) checks here?
 
 
 def built_in_types() -> Iterator[tuple[str, type[Generic]]]:
     """Yields class name and class definition tuple."""
 
     for cls_name, cls_type in inspect.getmembers(arcor2.object_types.abstract, predicate=inspect.isclass):
-
         try:
             if not issubclass(cls_type, Generic):
                 continue
         except TypeError:
             # TODO detect type-hinted generics (e.g. dict[str, str]) instead?
             # CancelDict / issubclass() arg 1 must be a class
             continue
 
         yield cls_name, cls_type
 
 
 def get_built_in_type(name: str) -> type[Generic]:
-
     for bname, cls in built_in_types():
         if name == bname:
             return cls
 
     raise KeyError
 
 
@@ -112,15 +110,14 @@
 
     settings_def = get_settings_def(type_def)
     settings_data: dict[str, Any] = {}
 
     settings_def_type_hints = get_type_hints(settings_def.__init__)
 
     for s in final.values():
-
         try:
             setting_def = settings_def_type_hints[s.name]
         except KeyError as e:
             raise Arcor2Exception(f"Unknown property {s.name}.") from e
 
         try:
             if issubclass(setting_def, JsonSchemaMixin):
@@ -153,15 +150,14 @@
 
     args = typing_inspect.get_args(param.annotation)
 
     # should support all of: 'Optional[Settings]', 'None | Settings', 'Settings, None'
     if typing_inspect.is_optional_type(param.annotation) or (
         typing_inspect.is_union_type(param.annotation) and None in args
     ):
-
         for arg in args:
             if arg != type(None):  # noqa: E721
                 settings_cls = arg
                 break
         else:
             raise Arcor2Exception("Can't find annotation for object settings.")
     else:
@@ -195,27 +191,24 @@
 
     if not cls_def.bases:
         return []
 
     ret: list[str] = []
 
     for base in reversed(cls_def.bases):
-
         assert isinstance(base, ast.Name)
         ret.append(base.id)
 
     return ret
 
 
 def iterate_over_actions(
     type_def: type[Generic],
 ) -> Iterator[tuple[str, Callable[[Any,], Any]]]:
-
     for method_name, method in inspect.getmembers(type_def, inspect.isroutine):
-
         try:
             if not isinstance(method.__action__, ActionMetadata):
                 continue
         except AttributeError:
             continue
 
         yield method_name, method
```

### Comparing `arcor2-1.0.0rc1/arcor2/parameter_plugins/base.py` & `arcor2-1.1.0/arcor2/parameter_plugins/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,27 +11,24 @@
 from arcor2.cached import CachedScene as CScene
 from arcor2.data.object_type import ParameterMeta
 from arcor2.exceptions import Arcor2NotImplemented
 from arcor2.parameter_plugins import ParameterPluginException, TypesDict
 
 
 class ImportTuple(NamedTuple):
-
     module_name: str
     class_name: str
 
 
 class ParameterPlugin(metaclass=abc.ABCMeta):
-
     EXACT_TYPE = True
     COUNTABLE = False
 
     @classmethod
     def _id_from_value(cls, value: str) -> str:
-
         arbitrary_id = cls._value_from_json(value)
 
         if not isinstance(arbitrary_id, str):
             raise ParameterPluginException("String expected.")
 
         return arbitrary_id
 
@@ -44,53 +41,48 @@
     @classmethod
     def type_name(cls) -> str:
         """Returns parameter type as string used in JSON."""
         return humps.depascalize(cls.type().__name__)
 
     @classmethod
     def meta(cls, param_meta: ParameterMeta, action_method: Callable, action_node: ast.FunctionDef) -> None:
-
         assert param_meta.type == cls.type_name()
         assert param_meta.name
 
     @classmethod
     @abc.abstractmethod
     def parameter_value(
         cls, type_defs: TypesDict, scene: CScene, project: CProject, action_id: str, parameter_id: str
     ) -> Any:
-
         action = project.action(action_id)
         param_value = action.parameter(parameter_id).value
 
         try:
             val = cls._value_from_json(param_value)
         except ParameterPluginException as e:
             raise ParameterPluginException(
                 f"Parameter {action.name}/{parameter_id} has invalid value: '{param_value}'."
             ) from e
 
         if not isinstance(val, cls.type()):
-
             raise ParameterPluginException(f"Parameter {action.name}/{parameter_id} has invalid type: '{type(val)}'.")
 
         return val
 
     @classmethod
     def _value_from_json(cls, value: str) -> Any:
-
         try:
             return json.loads(value)
         except json.JsonException as e:
             raise ParameterPluginException(f"Invalid value '{value}'.") from e
 
     @classmethod
     def parameter_execution_value(
         cls, type_defs: TypesDict, scene: CScene, project: CProject, action_id: str, parameter_id: str
     ) -> Any:
-
         # return copy in order to avoid unwanted changes in the original value if an action modifies the parameter
         return copy.deepcopy(cls.parameter_value(type_defs, scene, project, action_id, parameter_id))
 
     @classmethod
     @abc.abstractmethod
     def parameter_ast(
         cls, type_defs: TypesDict, scene: CScene, project: CProject, action_id: str, parameter_id: str
```

### Comparing `arcor2-1.0.0rc1/arcor2/parameter_plugins/boolean.py` & `arcor2-1.1.0/arcor2/parameter_plugins/boolean.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from arcor2.cached import CachedProject as CProject
 from arcor2.cached import CachedScene as CScene
 from arcor2.parameter_plugins.base import ParameterPlugin, TypesDict
 from arcor2.parameter_plugins.list import ListParameterPlugin, get_type_name
 
 
 class BooleanPlugin(ParameterPlugin):
-
     COUNTABLE = True
 
     @classmethod
     def type(cls) -> Any:
         return bool
 
     @classmethod
```

### Comparing `arcor2-1.0.0rc1/arcor2/parameter_plugins/double.py` & `arcor2-1.1.0/arcor2/parameter_plugins/double.py`

 * *Files identical despite different names*

### Comparing `arcor2-1.0.0rc1/arcor2/parameter_plugins/image.py` & `arcor2-1.1.0/arcor2/parameter_plugins/image.py`

 * *Files identical despite different names*

### Comparing `arcor2-1.0.0rc1/arcor2/parameter_plugins/integer.py` & `arcor2-1.1.0/arcor2/parameter_plugins/integer.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,29 +11,26 @@
 from arcor2.parameter_plugins.base import ParameterPlugin, ParameterPluginException, TypesDict
 from arcor2.parameter_plugins.list import ListParameterPlugin, get_type_name
 from arcor2.source.utils import find_asserts
 
 
 @dataclass
 class IntegerParameterExtra(JsonSchemaMixin):
-
     minimum: Any
     maximum: Any
 
 
 class AssertNotFound(ParameterPluginException):
     pass
 
 
 def get_assert_minimum_maximum(asserts: list[ast.Assert], param_name: str) -> tuple[Any, Any]:
-
     # Assert(test=Compare(left=Num(n=0), ops=[LtE(), LtE()], comparators=[Name(id='speed', ctx=Load()), Num(n=100)]))
 
     for ass in asserts:
-
         if not isinstance(ass.test, ast.Compare):
             continue
 
         if len(ass.test.comparators) != 2:
             continue
 
         if len(ass.test.ops) != 2:
@@ -55,15 +52,14 @@
 
     raise AssertNotFound()
 
 
 def get_min_max(
     cls: type[ParameterPlugin], param_meta: ParameterMeta, action_method: Callable, action_node: ast.FunctionDef
 ) -> None:
-
     try:
         minimum, maximum = get_assert_minimum_maximum(find_asserts(action_node), param_meta.name)
     except AssertNotFound:
         return
 
     for var in minimum, maximum:
         if not isinstance(var, cls.type()):
@@ -79,15 +75,14 @@
 
     @classmethod
     def type_name(cls) -> str:
         return "integer"
 
     @classmethod
     def meta(cls, param_meta: ParameterMeta, action_method: Callable, action_node: ast.FunctionDef) -> None:
-
         super(IntegerPlugin, cls).meta(param_meta, action_method, action_node)
         get_min_max(cls, param_meta, action_method, action_node)
 
     @classmethod
     def parameter_value(
         cls, type_defs: TypesDict, scene: CScene, project: CProject, action_id: str, parameter_id: str
     ) -> int:
```

### Comparing `arcor2-1.0.0rc1/arcor2/parameter_plugins/integer_enum.py` & `arcor2-1.1.0/arcor2/parameter_plugins/integer_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,20 +15,18 @@
 from arcor2.parameter_plugins.base import ImportTuple, ParameterPlugin, ParameterPluginException, TypesDict
 
 # TODO move IntEnum definition here?
 
 
 @dataclass
 class IntegerEnumExtra(JsonSchemaMixin):
-
     allowed_values: Optional[set[Any]] = None
 
 
 class IntegerEnumPlugin(ParameterPlugin):
-
     EXACT_TYPE = False
     COUNTABLE = True
 
     @classmethod
     def type(cls) -> Any:
         return IntEnum
 
@@ -46,15 +44,14 @@
 
         param_meta.extra = IntegerEnumExtra(ttype.set()).to_json()
 
     @classmethod
     def parameter_value(
         cls, type_defs: TypesDict, scene: CScene, project: CProject, action_id: str, parameter_id: str
     ) -> Enum:
-
         action = project.action(action_id)
         param = action.parameter(parameter_id)
         obj_id, action_type = action.parse_type()
         obj_type_name = scene.object(obj_id).type
         try:
             obj_type = type_defs[obj_type_name]
         except KeyError:
@@ -78,24 +75,22 @@
         except (ValueError, json.JsonException):
             raise ParameterPluginException(f"Parameter {parameter_id} of action {action.name} has invalid value.")
 
     @classmethod
     def parameter_ast(
         cls, type_defs: TypesDict, scene: CScene, project: CProject, action_id: str, parameter_id: str
     ) -> Attribute:
-
         val = cls.parameter_value(type_defs, scene, project, action_id, parameter_id)
 
         return Attribute(value=Name(id=val.__class__.__name__, ctx=Load()), attr=val.name, ctx=Load())
 
     @classmethod
     def need_to_be_imported(
         cls, type_defs: TypesDict, scene: CScene, project: CProject, action_id: str, parameter_id: str
     ) -> None | list[ImportTuple]:
-
         enum_cls = cls.parameter_value(type_defs, scene, project, action_id, parameter_id).__class__
         # TODO does this work as expected in all cases?
         module = inspect.getmodule(enum_cls)
         if not module:
             raise ParameterPluginException("Failed to get the module.")
 
         # TODO enums are typically defined in the same module as a object type but could be def. elsewhere (arcor2.data)
```

### Comparing `arcor2-1.0.0rc1/arcor2/parameter_plugins/joints.py` & `arcor2-1.1.0/arcor2/parameter_plugins/joints.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     def type_name(cls) -> str:
         return "joints"
 
     @classmethod
     def parameter_value(
         cls, type_defs: TypesDict, scene: CScene, project: CProject, action_id: str, parameter_id: str
     ) -> ProjectRobotJoints:
-
         try:
             ap, action = project.action_point_and_action(action_id)
             param = action.parameter(parameter_id)
             joints_id = cls._id_from_value(param.value)
 
             robot_id, action_method_name = action.parse_type()
 
@@ -40,24 +39,22 @@
 
     @classmethod
     def value_to_json(cls, value: ProjectRobotJoints) -> str:
         return value.to_json()
 
     @classmethod
     def uses_robot_joints(cls, project: CProject, action_id: str, parameter_id: str, robot_joints_id: str) -> bool:
-
         value_id = cls._id_from_value(project.action(action_id).parameter(parameter_id).value)
 
         return value_id == robot_joints_id
 
     @classmethod
     def parameter_ast(
         cls, type_defs: TypesDict, scene: CScene, project: CProject, action_id: str, parameter_id: str
     ) -> Attribute:
-
         ap, action = project.action_point_and_action(action_id)
         joints = project.joints(cls._id_from_value(action.parameter(parameter_id).value))
 
         return Attribute(
             value=Attribute(
                 value=Attribute(
                     value=Name(id="aps", ctx=Load()), attr=ap.name, ctx=Load()  # TODO this should not be hardcoded
```

### Comparing `arcor2-1.0.0rc1/arcor2/parameter_plugins/list.py` & `arcor2-1.1.0/arcor2/parameter_plugins/list.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,26 +14,24 @@
 
 class ListParameterPlugin(ParameterPlugin):
     @classmethod
     @abc.abstractmethod
     def parameter_value(
         cls, type_defs: TypesDict, scene: CScene, project: CProject, action_id: str, parameter_id: str
     ) -> list[Any]:
-
         val = super(ListParameterPlugin, cls).parameter_value(type_defs, scene, project, action_id, parameter_id)
 
         if not isinstance(val, list):
             raise ParameterPluginException("Not a list!")
         if val and not isinstance(val[0], cls.type()):
             raise ParameterPluginException("List content does not have expected type!")
 
         return val
 
     @classmethod
     def _param_value_list(cls, param: ActionParameter) -> list[str]:
-
         lst = json.loads(param.value)
 
         if not isinstance(lst, list):
             raise ParameterPluginException("Parameter value should be list of references to action points.")
 
         return lst
```

### Comparing `arcor2-1.0.0rc1/arcor2/parameter_plugins/pose.py` & `arcor2-1.1.0/arcor2/parameter_plugins/pose.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,45 +22,41 @@
     def orientation_id(cls, project: CProject, action_id: str, parameter_id: str) -> str:
         return cls._id_from_value(project.action(action_id).parameter(parameter_id).value)
 
     @classmethod
     def parameter_value(
         cls, type_defs: TypesDict, scene: CScene, project: CProject, action_id: str, parameter_id: str
     ) -> Pose:
-
         try:
             ap, ori = project.bare_ap_and_orientation(cls.orientation_id(project, action_id, parameter_id))
         except Arcor2Exception as e:
             raise ParameterPluginException("Failed to get scene/project data.") from e
         return Pose(ap.position, ori.orientation)
 
     @classmethod
     def parameter_execution_value(
         cls, type_defs: TypesDict, scene: CScene, project: CProject, action_id: str, parameter_id: str
     ) -> Pose:
-
         # return copy in order to avoid unwanted changes in the original value if an action modifies the parameter
         return copy.deepcopy(
             tr.abs_pose_from_ap_orientation(scene, project, cls.orientation_id(project, action_id, parameter_id))
         )
 
     @classmethod
     def value_to_json(cls, value: Pose) -> str:
         return value.to_json()
 
     @classmethod
     def uses_orientation(cls, project: CProject, action_id: str, parameter_id: str, orientation_id: str) -> bool:
-
         return orientation_id == cls.orientation_id(project, action_id, parameter_id)
 
     @classmethod
     def parameter_ast(
         cls, type_defs: TypesDict, scene: CScene, project: CProject, action_id: str, parameter_id: str
     ) -> Attribute:
-
         ori_ap, ori = project.bare_ap_and_orientation(cls.orientation_id(project, action_id, parameter_id))
 
         return Attribute(
             value=Attribute(
                 value=Attribute(
                     value=Name(id="aps", ctx=Load()), attr=ori_ap.name, ctx=Load()  # TODO this should not be hardcoded
                 ),
@@ -81,30 +77,28 @@
     def type_name(cls) -> str:
         return get_type_name(PosePlugin)
 
     @classmethod
     def parameter_value(
         cls, type_defs: TypesDict, scene: CScene, project: CProject, action_id: str, parameter_id: str
     ) -> list[Pose]:
-
         ret: list[Pose] = []
 
         ap, action = project.action_point_and_action(action_id)
         parameter = action.parameter(parameter_id)
 
         for orientation_id in cls._param_value_list(parameter):
             ret.append(Pose(ap.position, project.orientation(orientation_id).orientation))
 
         return ret
 
     @classmethod
     def parameter_execution_value(
         cls, type_defs: TypesDict, scene: CScene, project: CProject, action_id: str, parameter_id: str
     ) -> list[Pose]:
-
         ap, action = project.action_point_and_action(action_id)
 
         if not ap.parent:
             return copy.deepcopy(cls.parameter_value(type_defs, scene, project, action_id, parameter_id))
 
         parameter = action.parameter(parameter_id)
         ret: list[Pose] = []
@@ -116,15 +110,14 @@
 
     @classmethod
     def value_to_json(cls, value: list[Pose]) -> str:
         return json.dumps([v.to_json() for v in value])
 
     @classmethod
     def uses_orientation(cls, project: CProject, action_id: str, parameter_id: str, orientation_id: str) -> bool:
-
         action = project.action(action_id)
         param = action.parameter(parameter_id)
 
         for ori_id in cls._param_value_list(param):
             if ori_id == orientation_id:
                 return True
         return False
```

### Comparing `arcor2-1.0.0rc1/arcor2/parameter_plugins/position.py` & `arcor2-1.1.0/arcor2/parameter_plugins/position.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,38 +20,35 @@
     def ap_id(cls, project: CProject, action_id: str, parameter_id: str) -> str:
         return cls._id_from_value(project.action(action_id).parameter(parameter_id).value)
 
     @classmethod
     def parameter_value(
         cls, type_defs: TypesDict, scene: CScene, project: CProject, action_id: str, parameter_id: str
     ) -> Position:
-
         try:
             ap = project.bare_action_point(cls.ap_id(project, action_id, parameter_id))
         except Arcor2Exception as e:
             raise ParameterPluginException("Failed to get scene/project data.") from e
         return ap.position
 
     @classmethod
     def parameter_execution_value(
         cls, type_defs: TypesDict, scene: CScene, project: CProject, action_id: str, parameter_id: str
     ) -> Position:
-
         # return copy in order to avoid unwanted changes in the original value if an action modifies the parameter
         return copy.deepcopy(tr.abs_position_from_ap(scene, project, cls.ap_id(project, action_id, parameter_id)))
 
     @classmethod
     def value_to_json(cls, value: Position) -> str:
         return value.to_json()
 
     @classmethod
     def parameter_ast(
         cls, type_defs: TypesDict, scene: CScene, project: CProject, action_id: str, parameter_id: str
     ) -> Attribute:
-
         ap = project.bare_action_point(cls.ap_id(project, action_id, parameter_id))
 
         return Attribute(
             value=Attribute(
                 value=Name(id="aps", ctx=Load()), attr=ap.name, ctx=Load()  # TODO this should not be hardcoded
             ),
             attr="position",  # TODO this should not be hardcoded
```

### Comparing `arcor2-1.0.0rc1/arcor2/parameter_plugins/string.py` & `arcor2-1.1.0/arcor2/parameter_plugins/string.py`

 * *Files identical despite different names*

### Comparing `arcor2-1.0.0rc1/arcor2/parameter_plugins/utils.py` & `arcor2-1.1.0/arcor2/parameter_plugins/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 TypeToPluginDict = dict[type, type[ParameterPlugin]]
 
 _type_name_to_plugin: dict[str, type[ParameterPlugin]] = {}
 _type_to_plugin: TypeToPluginDict = {}
 
 
 def load_plugins() -> None:
-
     if _type_name_to_plugin:
         return
 
     # TODO just temporary solution - allow loading plugins based on env. var
 
     from arcor2.parameter_plugins.boolean import BooleanPlugin
     from arcor2.parameter_plugins.double import DoublePlugin
@@ -56,38 +55,33 @@
 
 
 def non_exact_types() -> TypeToPluginDict:
     return {k: v for k, v in _type_to_plugin.items() if not v.EXACT_TYPE}
 
 
 def known_parameter_types() -> set[str]:
-
     return set(_type_name_to_plugin.keys())
 
 
 def plugin_from_instance(inst: Any) -> type[ParameterPlugin]:
-
     # TODO support for lists (e.g. list[Pose])
     return plugin_from_type(type(inst))
 
 
 def plugin_from_type_name(param_type_name: str) -> type[ParameterPlugin]:
-
     try:
         return _type_name_to_plugin[param_type_name]
     except KeyError:
         raise ParameterPluginException(f"Unknown parameter type {param_type_name}.")
 
 
 def plugin_from_type(param_type: type[Any]) -> type[ParameterPlugin]:
-
     try:
         return _type_to_plugin[param_type]
     except KeyError:
-
         try:
             type_name = param_type.__name__
         except AttributeError:
             type_name = str(param_type)
 
         plugin: None | type[ParameterPlugin] = None
         for k, v in non_exact_types().items():
```

### Comparing `arcor2-1.0.0rc1/arcor2/rest.py` & `arcor2-1.1.0/arcor2/rest.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,24 +69,22 @@
 debug = env.get_bool("ARCOR2_REST_DEBUG", False)
 headers = {"accept": "application/json", "content-type": "application/json; charset=utf-8"}
 session = requests.session()
 logger = get_logger(__name__, logging.DEBUG if debug else logging.INFO)
 
 
 def dataclass_from_json(resp_json: dict[str, Any], return_type: type[DataClass]) -> DataClass:
-
     try:
         return return_type.from_dict(resp_json)
     except ValidationError as e:
         logger.debug(f'{return_type.__name__}: validation error "{e}" while parsing "{resp_json}".')
         raise RestException("Invalid data.", str(e)) from e
 
 
 def primitive_from_json(resp_json: Primitive, return_type: type[Primitive]) -> Primitive:
-
     try:
         return return_type(resp_json)
     except ValueError as e:
         logger.debug(f'{return_type.__name__}: error  "{e}" while parsing "{resp_json}".')
         raise RestException(e) from e
 
 
@@ -94,14 +92,15 @@
 @overload
 def call(
     method: Method,
     url: str,
     *,
     body: OptBody = None,
     params: OptParams = None,
+    raw_params: bool = False,
     files: OptFiles = None,
     timeout: OptTimeout = None,
 ) -> None:
     ...
 
 
 # single value-returning overloads
@@ -109,42 +108,45 @@
 def call(
     method: Method,
     url: str,
     *,
     return_type: type[Primitive],
     body: OptBody = None,
     params: OptParams = None,
+    raw_params: bool = False,
     files: OptFiles = None,
     timeout: OptTimeout = None,
 ) -> Primitive:
     ...
 
 
 @overload
 def call(
     method: Method,
     url: str,
     *,
     return_type: type[DataClass],
     body: OptBody = None,
     params: OptParams = None,
+    raw_params: bool = False,
     files: OptFiles = None,
     timeout: OptTimeout = None,
 ) -> DataClass:
     ...
 
 
 @overload
 def call(
     method: Method,
     url: str,
     *,
     return_type: type[BytesIO],
     body: OptBody = None,
     params: OptParams = None,
+    raw_params: bool = False,
     files: OptFiles = None,
     timeout: OptTimeout = None,
 ) -> BytesIO:
     ...
 
 
 # list-returning overloads
@@ -152,67 +154,73 @@
 def call(
     method: Method,
     url: str,
     *,
     list_return_type: type[Primitive],
     body: OptBody = None,
     params: OptParams = None,
+    raw_params: bool = False,
     files: OptFiles = None,
     timeout: OptTimeout = None,
 ) -> list[Primitive]:
     ...
 
 
 @overload
 def call(
     method: Method,
     url: str,
     *,
     list_return_type: type[DataClass],
     body: OptBody = None,
     params: OptParams = None,
+    raw_params: bool = False,
     files: OptFiles = None,
     timeout: OptTimeout = None,
 ) -> list[DataClass]:
     ...
 
 
 @overload
 def call(
     method: Method,
     url: str,
     *,
     list_return_type: type[BytesIO],
     body: OptBody = None,
     params: OptParams = None,
+    raw_params: bool = False,
     files: OptFiles = None,
     timeout: OptTimeout = None,
 ) -> list[BytesIO]:
     ...
 
 
 def call(
     method: Method,
     url: str,
     *,
     return_type: ReturnType = None,
     list_return_type: ReturnType = None,
     body: OptBody = None,
     params: OptParams = None,
+    raw_params: bool = False,
     files: OptFiles = None,
     timeout: OptTimeout = None,
 ) -> ReturnValue:
     """Universal function for calling REST APIs.
 
     :param method: HTTP method.
     :param url: Resource address.
     :param return_type: If set, function will try to return one value of a given type.
     :param list_return_type: If set, function will try to return list of a given type.
     :param body: Data to be send in the request body.
     :param params: Path parameters.
+    :param raw_params: Parameters are by default converted to camelCase form.
+                       If you do not want this behavior, pass True here
     :param files: Instead of body, it is possible to send files.
     :param timeout: Specific timeout for a call.
     :return: Return value/type is given by return_type/list_return_type. If both are None, nothing will be returned.
     """
     logger.debug(f"{method} {url}, body: {body}, params: {params}, files: {files is not None}, timeout: {timeout}")
 
     if body and files:
@@ -235,15 +243,15 @@
             if isinstance(dd, JsonSchemaMixin):
                 d.append(humps.camelize(dd.to_dict()))
             else:
                 d.append(dd)
     elif body is not None:
         raise RestException("Unsupported type of data.")
 
-    if params:
+    if params and not raw_params:
         params = humps.camelize(params)
 
         # requests just simply stringifies parameters, which does not work for booleans
         for param_name, param_value in params.items():
             if isinstance(param_value, bool):
                 params[param_name] = "true" if param_value else "false"
 
@@ -271,15 +279,14 @@
 
     _handle_response(resp)
 
     if return_type is None:
         return None
 
     if issubclass(return_type, BytesIO):
-
         if list_return_type:
             raise NotImplementedError
 
         return BytesIO(resp.content)
 
     logger.debug(f"Response text: {resp.text}")
 
@@ -295,24 +302,22 @@
     logger.debug(f"Decamelized json: {resp_json}")
 
     if list_return_type and not isinstance(resp_json, list):
         logger.debug(f"Expected list of type {return_type}, but got {resp_json}.")
         raise RestException("Response is not a list.")
 
     if issubclass(return_type, JsonSchemaMixin):
-
         if list_return_type:
             return [dataclass_from_json(item, return_type) for item in resp_json]
 
         else:
             assert not isinstance(resp_json, list)
             return dataclass_from_json(resp_json, return_type)
 
     else:  # probably a primitive
-
         if list_return_type:
             return [primitive_from_json(item, return_type) for item in resp_json]
         else:
             assert not isinstance(resp_json, list)
             return primitive_from_json(resp_json, return_type)
 
 
@@ -334,27 +339,26 @@
     except json.JsonException:
         # response contains invalid JSON
         raise RestException(decoded_content)
 
     if isinstance(cont, str):  # just plain text
         raise RestException(cont)
     elif isinstance(cont, dict):  # this could be WebApiError
-
         try:
             raise WebApiError.from_dict(cont)
         except ValidationError:
             raise RestException(str(cont))
 
 
-def get_image(url: str) -> Image.Image:
+def get_image(url: str, params: OptParams = None, raw_params: bool = False) -> Image.Image:
     """Shortcut for getting an image."""
 
     # TODO check content type?
     try:
-        return Image.open(call(Method.GET, url, return_type=BytesIO))
+        return Image.open(call(Method.GET, url, return_type=BytesIO, params=params, raw_params=raw_params))
     except (UnidentifiedImageError, TypeError) as e:
         raise RestException("Invalid image.") from e
 
 
 def download(url: str, path: str, params: OptParams = None) -> None:
     """Shortcut for saving a file to disk."""
```

### Comparing `arcor2-1.0.0rc1/arcor2/source/utils.py` & `arcor2-1.1.0/arcor2/source/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 
 import autopep8
 
 from arcor2.source import SourceException
 
 
 def parse(source: str) -> AST:
-
     try:
         return ast.parse(source, feature_version=sys.version_info[0:2])
     except (AssertionError, NotImplementedError, SyntaxError, ValueError) as e:
         raise SourceException("Failed to parse the code.") from e
 
 
 def parse_def(type_def: type) -> AST:
@@ -119,27 +118,25 @@
         def __init__(self, module: str, cls: str) -> None:
             self.done = False
             self.module = module
             self.cls = cls
 
         def visit_ImportFrom(self, node: ImportFrom) -> ImportFrom:
             if node.module == self.module:
-
                 for aliass in node.names:
                     if aliass.name == self.cls:
                         self.done = True
                         break
                 else:
                     node.names.append(alias(name=self.cls, asname=None))
                     self.done = True
 
             return node
 
     if try_to_import:
-
         try:
             imported_mod = importlib.import_module(module)
         except ModuleNotFoundError as e:
             raise SourceException(e)
 
         try:
             getattr(imported_mod, cls)
@@ -192,15 +189,14 @@
 
 
 def get_name_attr(name: str, attr: str, ctx: type[Load] | type[Store] = Load) -> Attribute:
     return Attribute(value=get_name(name), attr=attr, ctx=ctx())
 
 
 def tree_to_str(tree: AST) -> str:
-
     fix_missing_locations(tree)
     return autopep8.fix_code(ast.unparse(tree), options={"aggressive": 1, "max_line_length": 120})
 
 
 def dump(tree: Module) -> str:
     return ast.dump(tree)
```

### Comparing `arcor2-1.0.0rc1/arcor2/test_objects/box.py` & `arcor2-1.1.0/arcor2/test_objects/box.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from arcor2.data.common import ActionMetadata
 from arcor2.object_types.abstract import CollisionObject
 
 
 class Box(CollisionObject):
-
     _ABSTRACT = False
 
     def test(self, *, an: None | str = None) -> None:
         """Run test.
 
         :return:
         """
```

### Comparing `arcor2-1.0.0rc1/arcor2/test_objects/dummy_multiarm_robot.py` & `arcor2-1.1.0/arcor2/test_objects/dummy_multiarm_robot.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,28 +39,26 @@
                 self._poses[arm][eef] = Pose()
 
     def get_arm_ids(self) -> set[str]:
         return self.Arms.set()
 
     @staticmethod
     def _get_from_dict(d: dict[str, set[str]], arm_id: None | str = None) -> set[str]:
-
         if arm_id is None:
             raise Arcor2Exception("Arm has to be specified.")
 
         try:
             return d[arm_id]
         except KeyError:
             raise Arcor2Exception("Unknown arm.")
 
     def get_end_effectors_ids(self, arm_id: None | str = None) -> set[str]:
         return self._get_from_dict(self.EEF, arm_id)
 
     def get_end_effector_pose(self, end_effector: str, arm_id: None | str = None) -> Pose:
-
         if end_effector not in self.get_end_effectors_ids(arm_id):
             raise Arcor2Exception("Unknown end effector.")
 
         assert arm_id
 
         return tr.make_pose_abs(self.pose, self._poses[arm_id][end_effector])
 
@@ -188,15 +186,14 @@
 
         try:
             return self._hand_teaching[arm_id]
         except KeyError:
             raise Arcor2Exception("Unknown arm.")
 
     def set_hand_teaching_mode(self, enabled: bool, arm_id: None | str = None) -> None:
-
         if arm_id is None:
             raise Arcor2Exception("Arm has to be specified.")
 
         try:
             state = self._hand_teaching[arm_id]
         except KeyError:
             raise Arcor2Exception("Unknown arm.")
```

### Comparing `arcor2-1.0.0rc1/arcor2/test_objects/param_to_return.py` & `arcor2-1.1.0/arcor2/test_objects/param_to_return.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from arcor2.data.common import ActionMetadata
 from arcor2.object_types.abstract import Generic
 
 
 class ParamToReturn(Generic):
-
     _ABSTRACT = False
 
     def bool_param(self, param: bool, *, an: None | str = None) -> bool:
         return param
 
     def int_param(self, param: int, *, an: None | str = None) -> int:
         return param
```

### Comparing `arcor2-1.0.0rc1/arcor2/test_objects/tester.py` & `arcor2-1.1.0/arcor2/test_objects/tester.py`

 * *Files identical despite different names*

### Comparing `arcor2-1.0.0rc1/arcor2/test_objects/upload.py` & `arcor2-1.1.0/arcor2/test_objects/upload.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from arcor2.test_objects.dummy_multiarm_robot import DummyMultiArmRobot
 from arcor2.test_objects.param_to_return import ParamToReturn
 from arcor2.test_objects.position_param import PositionParam
 from arcor2.test_objects.tester import Tester
 
 
 def main() -> None:
-
     upload_def(PositionParam)
     upload_def(Box, BoxModel("Box", 0.1, 0.1, 0.1))
     upload_def(Box2, BoxModel("Box2", 0.2, 0.2, 0.2))
     upload_def(Tester, BoxModel("Tester", 0.3, 0.3, 0.3))
     upload_def(ParamToReturn)
     upload_def(DummyMultiArmRobot)
```

### Comparing `arcor2-1.0.0rc1/arcor2/transformations.py` & `arcor2-1.1.0/arcor2/transformations.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     return Pose(
         (child.position.rotated(parent.orientation) + parent.position),
         Orientation.from_quaternion(parent.orientation.as_quaternion() * child.orientation.as_quaternion()),
     )
 
 
 class Parent(NamedTuple):
-
     pose: Pose
     parent_id: None | str = None  # parent of the parent
 
 
 def get_parent_pose(scene: CScene, project: CProject, parent_id: str) -> Parent:
     """Returns pose of the parent and parent of the parent (if any).
 
@@ -72,17 +71,15 @@
 
     if not ap.parent:
         raise Arcor2Exception("Action point does not have a parent.")
 
     updated_aps: set[str] = set()
 
     def _update_childs(parent: Parent, ap_id: str) -> None:
-
         for child_id in project.childs(ap_id):
-
             try:
                 child_ap = project.bare_action_point(child_id)
             except CachedProjectException:
                 continue
 
             child_ap.position = child_ap.position.rotated(parent.pose.orientation)
 
@@ -91,15 +88,14 @@
                     parent.pose.orientation.as_quaternion() * ori.orientation.as_quaternion()
                 )
 
             updated_aps.add(child_ap.id)
             _update_childs(parent, child_ap.id)
 
     def _make_relative_ap_global(_ap: BareActionPoint) -> None:
-
         if not _ap.parent:
             return
 
         parent = get_parent_pose(scene, project, _ap.parent)
 
         if parent.pose.orientation != Orientation():
             _update_childs(parent, _ap.id)
@@ -131,17 +127,15 @@
     if ap.parent:
         raise Arcor2Exception("Action point already has a parent.")
 
     updated_aps: set[str] = set()
     updated_orientations: set[str] = set()
 
     def _update_childs(parent: Parent, ap_id: str) -> None:
-
         for child_id in project.childs(ap_id):
-
             try:
                 child_ap = project.bare_action_point(child_id)
             except CachedProjectException:
                 continue
 
             child_ap.position = child_ap.position.rotated(parent.pose.orientation, inverse=True)
 
@@ -152,15 +146,14 @@
 
                 updated_orientations.add(ori.id)
 
             updated_aps.add(child_ap.id)
             _update_childs(parent, child_ap.id)
 
     def _make_global_ap_relative(parent_id: str) -> None:
-
         parent = get_parent_pose(scene, project, parent_id)
 
         if parent.parent_id:
             _make_global_ap_relative(parent.parent_id)
 
         ap.position = make_pose_rel(parent.pose, Pose(ap.position, Orientation())).position
         for ori in project.ap_orientations(ap.id):
```

### Comparing `arcor2-1.0.0rc1/arcor2/urdf.py` & `arcor2-1.1.0/arcor2/urdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,21 +25,19 @@
 
 
 class Arcor2UrdfException(Arcor2Exception):
     pass
 
 
 def is_urdf_file(fname: str) -> bool:
-
     _, ext = os.path.splitext(fname)
     return ext in (".urdf", ".xml")
 
 
 def urdf_from_path(path_to_urdf: str) -> URDF:
-
     for file in os.listdir(path_to_urdf):
         if is_urdf_file(file):
             with open(os.path.join(path_to_urdf, file)) as f:
                 s = f.read()
             break
     else:
         raise Arcor2UrdfException("Failed to find urdf file.")
@@ -52,15 +50,14 @@
     try:
         return URDF.load(buff)
     except (ValueError, TypeError) as e:
         raise Arcor2UrdfException(str(e)) from e
 
 
 def urdf_from_url(url_of_zipped_package: str) -> URDF:
-
     with tempfile.TemporaryDirectory() as tmp_dir:
         path_to_zip = os.path.join(tmp_dir, "urdf.zip")
         rest.download(url_of_zipped_package, path_to_zip)
 
         with zipfile.ZipFile(path_to_zip, "r") as zip_ref:
             zip_ref.extractall(tmp_dir)
```

### Comparing `arcor2-1.0.0rc1/arcor2/ws_server.py` & `arcor2-1.1.0/arcor2/ws_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,24 +23,22 @@
 RPC_DICT_TYPE = dict[str, tuple[type[RPC], RPC_CB]]
 
 EventT = TypeVar("EventT", bound=Event)
 EVENT_DICT_TYPE = dict[str, tuple[type[EventT], Callable[[EventT, WsClient], Coroutine[Any, Any, None]]]]
 
 
 def custom_exception_handler(loop: asyncio.AbstractEventLoop, context: dict[str, Any]) -> None:
-
     # it is also possible to use aiorun.run with stop_on_unhandled_errors=True but this prints much more useful info
     loop.default_exception_handler(context)
 
     if __debug__:  # stop loop while debugging, try to continue in production
         loop.stop()
 
 
 async def send_json_to_client(client: WsClient, data: str) -> None:
-
     try:
         await client.send(data)
     except websockets.exceptions.ConnectionClosed:
         pass
 
 
 async def server(
@@ -49,28 +47,26 @@
     register: Callable[[Any], Awaitable[None]],
     unregister: Callable[[Any], Awaitable[None]],
     rpc_dict: RPC_DICT_TYPE,
     event_dict: None | EVENT_DICT_TYPE = None,
     verbose: bool = False,
 ) -> None:
     async def handle_message(msg: str) -> None:
-
         try:
             data = json.loads(msg)
         except json.JsonException as e:
             logger.error(f"Invalid data: '{msg}'.")
             logger.debug(e)
             return
 
         if not isinstance(data, dict):
             logger.error(f"Invalid data: '{data}'.")
             return
 
         if "request" in data:  # ...then it is RPC
-
             req_type = data["request"]
 
             try:
                 rpc_cls, rpc_cb = rpc_dict[req_type]
             except KeyError:
                 logger.error(f"Unknown RPC request: {data}.")
                 return
@@ -88,15 +84,14 @@
                     await client.send(rpc_cls.Response(data["id"], False, messages=[str(e)]).to_json())
                     logger.debug(e, exc_info=True)
                 except (KeyError, websockets.exceptions.ConnectionClosed):
                     pass
                 return
 
             else:
-
                 try:
                     rpc_start = time.monotonic()
                     resp = await rpc_cb(req, client)
                     rpc_dur = time.monotonic() - rpc_start
                     if rpc_dur > MAX_RPC_DURATION:
                         logger.warn(f"{req.request} callback took {rpc_dur:.3f}s.")
 
@@ -112,15 +107,14 @@
 
             try:
                 await client.send(resp.to_json())
             except websockets.exceptions.ConnectionClosed:
                 return
 
             if logger.level == LogLevel.DEBUG:
-
                 # Silencing of repetitive log messages
                 # ...maybe this could be done better and in a more general way using logging.Filter?
 
                 now = time.monotonic()
                 if req.request not in req_last_ts:
                     req_last_ts[req.request] = deque()
 
@@ -141,15 +135,14 @@
                     if req.request in ignored_reqs:
                         ignored_reqs.remove(req.request)
 
                 if req.request not in ignored_reqs:
                     logger.debug(f"RPC request: {req}, result: {resp}")
 
         elif "event" in data:  # ...event from UI
-
             assert event_dict
 
             try:
                 event_cls, event_cb = event_dict[data["event"]]
             except KeyError as e:
                 logger.error(f"Unknown event type: {e}.")
                 return
@@ -168,15 +161,14 @@
     if event_dict is None:
         event_dict = {}
 
     req_last_ts: dict[str, deque] = {}
     ignored_reqs: set[str] = set()
 
     try:
-
         await register(client)
 
         loop = asyncio.get_event_loop()
 
         async for message in client:
             loop.create_task(handle_message(message))
```

### Comparing `arcor2-1.0.0rc1/arcor2.egg-info/PKG-INFO` & `arcor2-1.1.0/arcor2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcor2
-Version: 1.0.0rc1
+Version: 1.1.0
 Summary: ARCOR2 base library
 Author: Robo@FIT
 Author-email: imaterna@fit.vut.cz
 License: LGPL
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -16,21 +16,32 @@
 Description-Content-Type: text/markdown
 
 # arcor2
 # Changelog
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 
-## [1.0.0rc1] - 2023-02-06
+## [1.1.0] - 2023-07-20
+
+### Added
+
+- Few new helper functions.
+
+### Changed
+
+- Object pose is now not set using a property setter but using the `set_pose` method.  
+
+## [1.0.0] - 2023-02-14
 
 ### Changed
 
 - Updated dependencies.
-- Compatibility with the newest version of the Project service.
-- Project service client updated to match Project 1.0.0-rc.1.
+- Compatibility with the Project service 1.0.0.
+  - `Mesh` dataclass: `data_id` changed to `asset_id`.
+  - Updated client (some paths were changed).
 
 ### Added
 
 - Method `start` from the Scene service client now allows to specify a timeout. 
 
 ## [0.26.0] - 2022-12-12
```

### Comparing `arcor2-1.0.0rc1/arcor2.egg-info/SOURCES.txt` & `arcor2-1.1.0/arcor2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arcor2-1.0.0rc1/setup.py` & `arcor2-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,50 +19,62 @@
     'description': 'ARCOR2 base library',
     'entry_points': {
         'console_scripts': [
             'arcor2_upload_builtin_objects = arcor2.scripts.upload_builtin_objects:main',
         ],
     },
     'install_requires': (
-        'Flask~=2.2.2',
+        'Flask~=2.2.3',
         'Pillow~=9.4.0',
         'aiologger~=0.7.0',
         'apispec-webframeworks~=0.5.2',
-        'apispec[yaml]~=6.0.2',
-        'autopep8~=2.0.1',
+        'apispec[yaml]~=6.3.0',
+        'autopep8~=2.0.2',
         'colorlog~=6.7.0',
         'dataclasses-jsonschema[apispec,fast-dateparsing,fast-uuid,fast-validation]~=2.16.0',
         'fastuuid~=0.8.0',
         'flask-swagger-ui~=4.11.1',
         'flask_cors~=3.0.10',
-        'numpy-quaternion[numba,scipy]~=2022.4.2',
+        'numpy-quaternion[numba,scipy]~=2022.4.3',
         'numpy~=1.23.5',
-        'opencv-contrib-python~=4.7.0.68',
-        'orjson~=3.8.5',
+        'opencv-contrib-python~=4.7.0.72',
+        'orjson~=3.8.8',
         'packaging~=21.3',
         'pyhumps==3.8.0',
         'python-dateutil~=2.8.2',
         'requests~=2.28.2',
+        'setuptools~=66.0.0',
         'typing-inspect~=0.8.0',
         'urdfpy~=0.0.22',
         'websockets~=10.4',
     ),
     'license': 'LGPL',
     'long_description': """# arcor2
 # Changelog
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 
-## [1.0.0rc1] - 2023-02-06
+## [1.1.0] - 2023-07-20
+
+### Added
+
+- Few new helper functions.
+
+### Changed
+
+- Object pose is now not set using a property setter but using the `set_pose` method.  
+
+## [1.0.0] - 2023-02-14
 
 ### Changed
 
 - Updated dependencies.
-- Compatibility with the newest version of the Project service.
-- Project service client updated to match Project 1.0.0-rc.1.
+- Compatibility with the Project service 1.0.0.
+  - `Mesh` dataclass: `data_id` changed to `asset_id`.
+  - Updated client (some paths were changed).
 
 ### Added
 
 - Method `start` from the Scene service client now allows to specify a timeout. 
 
 ## [0.26.0] - 2022-12-12
 
@@ -576,9 +588,9 @@
         'arcor2.object_types',
         'arcor2.parameter_plugins',
         'arcor2.scripts',
         'arcor2.source',
         'arcor2.test_objects',
     ),
     'python_requires': '==3.10.*',
-    'version': '1.0.0rc1',
+    'version': '1.1.0',
 })
```

