# Comparing `tmp/devcycle-python-server-sdk-3.3.2.tar.gz` & `tmp/devcycle-python-server-sdk-3.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/devcycle-python-server-sdk-3.3.2.tar", last modified: Thu Jul 20 20:27:10 2023, max compression
+gzip compressed data, was "dist/devcycle-python-server-sdk-3.3.3.tar", last modified: Fri Jul 21 20:44:11 2023, max compression
```

## Comparing `devcycle-python-server-sdk-3.3.2.tar` & `devcycle-python-server-sdk-3.3.3.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:27:10.000000 devcycle-python-server-sdk-3.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-20 20:27:10.000000 devcycle-python-server-sdk-3.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-07-20 20:26:52.000000 devcycle-python-server-sdk-3.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:27:10.000000 devcycle-python-server-sdk-3.3.2/devcycle_python_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-20 20:26:52.000000 devcycle-python-server-sdk-3.3.2/devcycle_python_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:27:10.000000 devcycle-python-server-sdk-3.3.2/devcycle_python_sdk/api/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 20:26:52.000000 devcycle-python-server-sdk-3.3.2/devcycle_python_sdk/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-20 20:26:52.000000 devcycle-python-server-sdk-3.3.2/devcycle_python_sdk/api/backoff.py
--rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-07-20 20:26:52.000000 devcycle-python-server-sdk-3.3.2/devcycle_python_sdk/api/bucketing_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-07-20 20:26:52.000000 devcycle-python-server-sdk-3.3.2/devcycle_python_sdk/api/config_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-07-20 20:26:52.000000 devcycle-python-server-sdk-3.3.2/devcycle_python_sdk/api/event_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16322 2023-07-20 20:26:52.000000 devcycle-python-server-sdk-3.3.2/devcycle_python_sdk/api/local_bucketing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-07-20 20:26:52.000000 devcycle-python-server-sdk-3.3.2/devcycle_python_sdk/cloud_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-20 20:26:52.000000 devcycle-python-server-sdk-3.3.2/devcycle_python_sdk/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8605 2023-07-20 20:26:52.000000 devcycle-python-server-sdk-3.3.2/devcycle_python_sdk/local_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:27:10.000000 devcycle-python-server-sdk-3.3.2/devcycle_python_sdk/managers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:26:52.000000 devcycle-python-server-sdk-3.3.2/devcycle_python_sdk/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-07-20 20:26:52.000000 devcycle-python-server-sdk-3.3.2/devcycle_python_sdk/managers/config_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-07-20 20:26:52.000000 devcycle-python-server-sdk-3.3.2/devcycle_python_sdk/managers/event_queue_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:27:10.000000 devcycle-python-server-sdk-3.3.2/devcycle_python_sdk/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:26:52.000000 devcycle-python-server-sdk-3.3.2/devcycle_python_sdk/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-20 20:26:52.000000 devcycle-python-server-sdk-3.3.2/devcycle_python_sdk/models/bucketed_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-20 20:26:52.000000 devcycle-python-server-sdk-3.3.2/devcycle_python_sdk/models/error_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-07-20 20:26:52.000000 devcycle-python-server-sdk-3.3.2/devcycle_python_sdk/models/event.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-20 20:26:52.000000 devcycle-python-server-sdk-3.3.2/devcycle_python_sdk/models/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-20 20:26:52.000000 devcycle-python-server-sdk-3.3.2/devcycle_python_sdk/models/platform_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-07-20 20:26:52.000000 devcycle-python-server-sdk-3.3.2/devcycle_python_sdk/models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-20 20:26:52.000000 devcycle-python-server-sdk-3.3.2/devcycle_python_sdk/models/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-07-20 20:26:52.000000 devcycle-python-server-sdk-3.3.2/devcycle_python_sdk/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:27:10.000000 devcycle-python-server-sdk-3.3.2/devcycle_python_sdk/protobuf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:26:52.000000 devcycle-python-server-sdk-3.3.2/devcycle_python_sdk/protobuf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-07-20 20:26:52.000000 devcycle-python-server-sdk-3.3.2/devcycle_python_sdk/protobuf/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-07-20 20:26:52.000000 devcycle-python-server-sdk-3.3.2/devcycle_python_sdk/protobuf/variableForUserParams_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:27:10.000000 devcycle-python-server-sdk-3.3.2/devcycle_python_sdk/util/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 20:26:52.000000 devcycle-python-server-sdk-3.3.2/devcycle_python_sdk/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-20 20:26:52.000000 devcycle-python-server-sdk-3.3.2/devcycle_python_sdk/util/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:27:10.000000 devcycle-python-server-sdk-3.3.2/devcycle_python_server_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-20 20:27:10.000000 devcycle-python-server-sdk-3.3.2/devcycle_python_server_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-20 20:27:10.000000 devcycle-python-server-sdk-3.3.2/devcycle_python_server_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 20:27:10.000000 devcycle-python-server-sdk-3.3.2/devcycle_python_server_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-20 20:27:10.000000 devcycle-python-server-sdk-3.3.2/devcycle_python_server_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-20 20:27:10.000000 devcycle-python-server-sdk-3.3.2/devcycle_python_server_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:27:10.000000 devcycle-python-server-sdk-3.3.2/example/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:26:52.000000 devcycle-python-server-sdk-3.3.2/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-07-20 20:26:52.000000 devcycle-python-server-sdk-3.3.2/example/cloud_client_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-07-20 20:26:52.000000 devcycle-python-server-sdk-3.3.2/example/local_bucketing_client_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-20 20:26:52.000000 devcycle-python-server-sdk-3.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-20 20:27:10.000000 devcycle-python-server-sdk-3.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-20 20:26:52.000000 devcycle-python-server-sdk-3.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:27:10.000000 devcycle-python-server-sdk-3.3.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:26:52.000000 devcycle-python-server-sdk-3.3.2/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:27:10.000000 devcycle-python-server-sdk-3.3.2/test/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:26:52.000000 devcycle-python-server-sdk-3.3.2/test/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-07-20 20:26:52.000000 devcycle-python-server-sdk-3.3.2/test/api/test_bucketing_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-07-20 20:26:52.000000 devcycle-python-server-sdk-3.3.2/test/api/test_config_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-07-20 20:26:52.000000 devcycle-python-server-sdk-3.3.2/test/api/test_event_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15156 2023-07-20 20:26:52.000000 devcycle-python-server-sdk-3.3.2/test/api/test_local_bucketing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:27:10.000000 devcycle-python-server-sdk-3.3.2/test/fixture/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:26:52.000000 devcycle-python-server-sdk-3.3.2/test/fixture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-20 20:26:52.000000 devcycle-python-server-sdk-3.3.2/test/fixture/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:27:10.000000 devcycle-python-server-sdk-3.3.2/test/managers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:26:52.000000 devcycle-python-server-sdk-3.3.2/test/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-07-20 20:26:52.000000 devcycle-python-server-sdk-3.3.2/test/managers/test_config_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    11053 2023-07-20 20:26:52.000000 devcycle-python-server-sdk-3.3.2/test/managers/test_event_queue_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:27:10.000000 devcycle-python-server-sdk-3.3.2/test/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:26:52.000000 devcycle-python-server-sdk-3.3.2/test/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-20 20:26:52.000000 devcycle-python-server-sdk-3.3.2/test/models/test_bucketed_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11442 2023-07-20 20:26:52.000000 devcycle-python-server-sdk-3.3.2/test/test_cloud_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12671 2023-07-20 20:26:52.000000 devcycle-python-server-sdk-3.3.2/test/test_local_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:27:10.000000 devcycle-python-server-sdk-3.3.2/test/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:26:52.000000 devcycle-python-server-sdk-3.3.2/test/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-07-20 20:26:52.000000 devcycle-python-server-sdk-3.3.2/test/util/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-20 20:26:52.000000 devcycle-python-server-sdk-3.3.2/test/util/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:44:11.000000 devcycle-python-server-sdk-3.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-21 20:44:11.000000 devcycle-python-server-sdk-3.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:44:11.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:44:11.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/api/backoff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/api/bucketing_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/api/config_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/api/event_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16322 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/api/local_bucketing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/cloud_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8605 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/local_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:44:11.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/managers/config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/managers/event_queue_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:44:11.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/models/bucketed_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/models/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/models/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/models/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/models/platform_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/models/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:44:11.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/protobuf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/protobuf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/protobuf/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/protobuf/variableForUserParams_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:44:11.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/util/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:44:11.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_server_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-21 20:44:11.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_server_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-21 20:44:11.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_server_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 20:44:11.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_server_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-21 20:44:11.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_server_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-21 20:44:11.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_server_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:44:11.000000 devcycle-python-server-sdk-3.3.3/example/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/example/cloud_client_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/example/local_bucketing_client_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-21 20:44:11.000000 devcycle-python-server-sdk-3.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:44:11.000000 devcycle-python-server-sdk-3.3.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:44:11.000000 devcycle-python-server-sdk-3.3.3/test/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/test/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/test/api/test_bucketing_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/test/api/test_config_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/test/api/test_event_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15156 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/test/api/test_local_bucketing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:44:11.000000 devcycle-python-server-sdk-3.3.3/test/fixture/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/test/fixture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/test/fixture/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:44:11.000000 devcycle-python-server-sdk-3.3.3/test/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/test/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/test/managers/test_config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11053 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/test/managers/test_event_queue_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:44:11.000000 devcycle-python-server-sdk-3.3.3/test/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/test/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/test/models/test_bucketed_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11442 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/test/test_cloud_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12671 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/test/test_local_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:44:11.000000 devcycle-python-server-sdk-3.3.3/test/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/test/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/test/util/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/test/util/test_version.py
```

### Comparing `devcycle-python-server-sdk-3.3.2/README.md` & `devcycle-python-server-sdk-3.3.3/README.md`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.2/devcycle_python_sdk/api/bucketing_client.py` & `devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/api/bucketing_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.2/devcycle_python_sdk/api/config_client.py` & `devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/api/config_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.2/devcycle_python_sdk/api/event_client.py` & `devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/api/event_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.2/devcycle_python_sdk/api/local_bucketing.py` & `devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/api/local_bucketing.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.2/devcycle_python_sdk/cloud_client.py` & `devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/cloud_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.2/devcycle_python_sdk/exceptions.py` & `devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.2/devcycle_python_sdk/local_client.py` & `devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/local_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.2/devcycle_python_sdk/managers/config_manager.py` & `devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/managers/config_manager.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.2/devcycle_python_sdk/managers/event_queue_manager.py` & `devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/managers/event_queue_manager.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.2/devcycle_python_sdk/models/bucketed_config.py` & `devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/models/bucketed_config.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.2/devcycle_python_sdk/models/event.py` & `devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/models/event.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.2/devcycle_python_sdk/models/feature.py` & `devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/models/feature.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.2/devcycle_python_sdk/models/platform_data.py` & `devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/models/platform_data.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.2/devcycle_python_sdk/models/user.py` & `devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/models/user.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.2/devcycle_python_sdk/models/variable.py` & `devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/models/variable.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.2/devcycle_python_sdk/options.py` & `devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/options.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.2/devcycle_python_sdk/protobuf/utils.py` & `devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/protobuf/utils.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.2/devcycle_python_sdk/protobuf/variableForUserParams_pb2.py` & `devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/protobuf/variableForUserParams_pb2.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.2/devcycle_python_server_sdk.egg-info/SOURCES.txt` & `devcycle-python-server-sdk-3.3.3/devcycle_python_server_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.2/example/cloud_client_example.py` & `devcycle-python-server-sdk-3.3.3/example/cloud_client_example.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.2/example/local_bucketing_client_example.py` & `devcycle-python-server-sdk-3.3.3/example/local_bucketing_client_example.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.2/pyproject.toml` & `devcycle-python-server-sdk-3.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.2/setup.py` & `devcycle-python-server-sdk-3.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.2/test/api/test_bucketing_client.py` & `devcycle-python-server-sdk-3.3.3/test/api/test_bucketing_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.2/test/api/test_config_client.py` & `devcycle-python-server-sdk-3.3.3/test/api/test_config_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.2/test/api/test_event_client.py` & `devcycle-python-server-sdk-3.3.3/test/api/test_event_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.2/test/api/test_local_bucketing.py` & `devcycle-python-server-sdk-3.3.3/test/api/test_local_bucketing.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.2/test/fixture/data.py` & `devcycle-python-server-sdk-3.3.3/test/fixture/data.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.2/test/managers/test_config_manager.py` & `devcycle-python-server-sdk-3.3.3/test/managers/test_config_manager.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.2/test/managers/test_event_queue_manager.py` & `devcycle-python-server-sdk-3.3.3/test/managers/test_event_queue_manager.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.2/test/models/test_bucketed_config.py` & `devcycle-python-server-sdk-3.3.3/test/models/test_bucketed_config.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.2/test/test_cloud_client.py` & `devcycle-python-server-sdk-3.3.3/test/test_cloud_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.2/test/test_local_client.py` & `devcycle-python-server-sdk-3.3.3/test/test_local_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.2/test/util/test_utils.py` & `devcycle-python-server-sdk-3.3.3/test/util/test_utils.py`

 * *Files identical despite different names*

