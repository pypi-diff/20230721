# Comparing `tmp/iflytekspark-0.0.3.tar.gz` & `tmp/iflytekspark-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iflytekspark-0.0.3.tar", last modified: Fri Jul 21 02:01:47 2023, max compression
+gzip compressed data, was "iflytekspark-0.0.4.tar", last modified: Fri Jul 21 02:08:36 2023, max compression
```

## Comparing `iflytekspark-0.0.3.tar` & `iflytekspark-0.0.4.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 lw         (502) staff       (20)        0 2023-07-21 02:01:47.000000 iflytekspark-0.0.3/
--rw-r--r--   0 lw         (502) staff       (20)     1095 2023-07-19 09:47:31.000000 iflytekspark-0.0.3/LICENSE
--rw-r--r--   0 lw         (502) staff       (20)    13453 2023-07-21 02:01:47.000000 iflytekspark-0.0.3/PKG-INFO
--rw-r--r--   0 lw         (502) staff       (20)    12866 2023-07-19 09:48:24.000000 iflytekspark-0.0.3/README.md
-drwxr-xr-x   0 lw         (502) staff       (20)        0 2023-07-21 02:01:47.000000 iflytekspark-0.0.3/iflytekspark/
--rw-r--r--   0 lw         (502) staff       (20)     3209 2023-07-21 01:55:54.000000 iflytekspark-0.0.3/iflytekspark/__init__.py
--rw-r--r--   0 lw         (502) staff       (20)     2630 2023-07-19 10:04:33.000000 iflytekspark-0.0.3/iflytekspark/_iflytekspark_scripts.py
--rw-r--r--   0 lw         (502) staff       (20)    24702 2023-07-20 11:30:42.000000 iflytekspark-0.0.3/iflytekspark/api_requestor.py
-drwxr-xr-x   0 lw         (502) staff       (20)        0 2023-07-21 02:01:47.000000 iflytekspark-0.0.3/iflytekspark/api_resources/
--rw-r--r--   0 lw         (502) staff       (20)      991 2023-07-19 10:04:33.000000 iflytekspark-0.0.3/iflytekspark/api_resources/__init__.py
-drwxr-xr-x   0 lw         (502) staff       (20)        0 2023-07-21 02:01:47.000000 iflytekspark-0.0.3/iflytekspark/api_resources/abstract/
--rw-r--r--   0 lw         (502) staff       (20)      576 2023-07-19 10:04:33.000000 iflytekspark-0.0.3/iflytekspark/api_resources/abstract/__init__.py
--rw-r--r--   0 lw         (502) staff       (20)     5515 2023-07-19 10:04:33.000000 iflytekspark-0.0.3/iflytekspark/api_resources/abstract/api_resource.py
--rw-r--r--   0 lw         (502) staff       (20)     2603 2023-07-19 10:04:33.000000 iflytekspark-0.0.3/iflytekspark/api_resources/abstract/createable_api_resource.py
--rw-r--r--   0 lw         (502) staff       (20)     1642 2023-07-19 10:04:33.000000 iflytekspark-0.0.3/iflytekspark/api_resources/abstract/deletable_api_resource.py
--rw-r--r--   0 lw         (502) staff       (20)    10097 2023-07-19 10:04:33.000000 iflytekspark-0.0.3/iflytekspark/api_resources/abstract/engine_api_resource.py
--rw-r--r--   0 lw         (502) staff       (20)     2744 2023-07-19 10:04:33.000000 iflytekspark-0.0.3/iflytekspark/api_resources/abstract/listable_api_resource.py
--rw-r--r--   0 lw         (502) staff       (20)     5104 2023-07-19 10:04:33.000000 iflytekspark-0.0.3/iflytekspark/api_resources/abstract/nested_resource_class_methods.py
--rw-r--r--   0 lw         (502) staff       (20)      540 2023-07-19 10:04:33.000000 iflytekspark-0.0.3/iflytekspark/api_resources/abstract/updateable_api_resource.py
--rw-r--r--   0 lw         (502) staff       (20)     7122 2023-07-19 10:04:33.000000 iflytekspark-0.0.3/iflytekspark/api_resources/audio.py
--rw-r--r--   0 lw         (502) staff       (20)     1617 2023-07-19 10:04:33.000000 iflytekspark-0.0.3/iflytekspark/api_resources/chat_completion.py
--rw-r--r--   0 lw         (502) staff       (20)     1646 2023-07-19 10:04:33.000000 iflytekspark-0.0.3/iflytekspark/api_resources/completion.py
--rw-r--r--   0 lw         (502) staff       (20)      563 2023-07-19 10:04:33.000000 iflytekspark-0.0.3/iflytekspark/api_resources/customer.py
--rw-r--r--   0 lw         (502) staff       (20)     4073 2023-07-19 10:04:33.000000 iflytekspark-0.0.3/iflytekspark/api_resources/deployment.py
--rw-r--r--   0 lw         (502) staff       (20)     1993 2023-07-19 10:04:33.000000 iflytekspark-0.0.3/iflytekspark/api_resources/edit.py
--rw-r--r--   0 lw         (502) staff       (20)     3480 2023-07-19 10:04:33.000000 iflytekspark-0.0.3/iflytekspark/api_resources/embedding.py
--rw-r--r--   0 lw         (502) staff       (20)     1683 2023-07-19 10:04:33.000000 iflytekspark-0.0.3/iflytekspark/api_resources/engine.py
--rw-r--r--   0 lw         (502) staff       (20)      922 2023-07-19 10:04:33.000000 iflytekspark-0.0.3/iflytekspark/api_resources/error_object.py
-drwxr-xr-x   0 lw         (502) staff       (20)        0 2023-07-21 02:01:47.000000 iflytekspark-0.0.3/iflytekspark/api_resources/experimental/
--rw-r--r--   0 lw         (502) staff       (20)      110 2023-07-19 10:04:33.000000 iflytekspark-0.0.3/iflytekspark/api_resources/experimental/__init__.py
--rw-r--r--   0 lw         (502) staff       (20)      280 2023-07-19 10:04:33.000000 iflytekspark-0.0.3/iflytekspark/api_resources/experimental/completion_config.py
--rw-r--r--   0 lw         (502) staff       (20)     7797 2023-07-19 10:04:33.000000 iflytekspark-0.0.3/iflytekspark/api_resources/file.py
--rw-r--r--   0 lw         (502) staff       (20)     5329 2023-07-19 10:04:33.000000 iflytekspark-0.0.3/iflytekspark/api_resources/fine_tune.py
--rw-r--r--   0 lw         (502) staff       (20)     6345 2023-07-19 10:04:33.000000 iflytekspark-0.0.3/iflytekspark/api_resources/image.py
--rw-r--r--   0 lw         (502) staff       (20)      175 2023-07-19 10:04:33.000000 iflytekspark-0.0.3/iflytekspark/api_resources/model.py
--rw-r--r--   0 lw         (502) staff       (20)     1400 2023-07-19 10:04:33.000000 iflytekspark-0.0.3/iflytekspark/api_resources/moderation.py
--rw-r--r--   0 lw         (502) staff       (20)    38806 2023-07-19 10:04:33.000000 iflytekspark-0.0.3/iflytekspark/cli.py
-drwxr-xr-x   0 lw         (502) staff       (20)        0 2023-07-21 02:01:47.000000 iflytekspark-0.0.3/iflytekspark/datalib/
--rw-r--r--   0 lw         (502) staff       (20)      657 2023-07-19 10:04:33.000000 iflytekspark-0.0.3/iflytekspark/datalib/__init__.py
--rw-r--r--   0 lw         (502) staff       (20)      270 2023-07-19 10:04:33.000000 iflytekspark-0.0.3/iflytekspark/datalib/common.py
--rw-r--r--   0 lw         (502) staff       (20)      326 2023-07-19 10:04:33.000000 iflytekspark-0.0.3/iflytekspark/datalib/numpy_helper.py
--rw-r--r--   0 lw         (502) staff       (20)      335 2023-07-19 10:04:33.000000 iflytekspark-0.0.3/iflytekspark/datalib/pandas_helper.py
--rw-r--r--   0 lw         (502) staff       (20)     8634 2023-07-19 10:04:33.000000 iflytekspark-0.0.3/iflytekspark/embeddings_utils.py
--rw-r--r--   0 lw         (502) staff       (20)     4406 2023-07-19 10:04:33.000000 iflytekspark-0.0.3/iflytekspark/error.py
--rw-r--r--   0 lw         (502) staff       (20)    10946 2023-07-19 10:04:33.000000 iflytekspark-0.0.3/iflytekspark/iflytekspark_object.py
--rw-r--r--   0 lw         (502) staff       (20)      554 2023-07-19 10:04:33.000000 iflytekspark-0.0.3/iflytekspark/iflytekspark_response.py
--rw-r--r--   0 lw         (502) staff       (20)      391 2023-07-19 10:04:33.000000 iflytekspark-0.0.3/iflytekspark/object_classes.py
--rw-------   0 lw         (502) staff       (20)     6575 2023-07-21 01:54:13.000000 iflytekspark-0.0.3/iflytekspark/sparkwbwrap.py
-drwxr-xr-x   0 lw         (502) staff       (20)        0 2023-07-21 02:01:47.000000 iflytekspark-0.0.3/iflytekspark/tests/
--rw-r--r--   0 lw         (502) staff       (20)        0 2023-07-19 10:04:33.000000 iflytekspark-0.0.3/iflytekspark/tests/__init__.py
-drwxr-xr-x   0 lw         (502) staff       (20)        0 2023-07-21 02:01:47.000000 iflytekspark-0.0.3/iflytekspark/tests/asyncio/
--rw-r--r--   0 lw         (502) staff       (20)        0 2023-07-19 10:04:33.000000 iflytekspark-0.0.3/iflytekspark/tests/asyncio/__init__.py
--rw-r--r--   0 lw         (502) staff       (20)     2434 2023-07-19 10:04:33.000000 iflytekspark-0.0.3/iflytekspark/tests/asyncio/test_endpoints.py
--rw-r--r--   0 lw         (502) staff       (20)     2366 2023-07-19 10:04:33.000000 iflytekspark-0.0.3/iflytekspark/tests/test_api_requestor.py
--rw-r--r--   0 lw         (502) staff       (20)     2963 2023-07-19 10:04:33.000000 iflytekspark-0.0.3/iflytekspark/tests/test_endpoints.py
--rw-r--r--   0 lw         (502) staff       (20)     1234 2023-07-19 10:04:33.000000 iflytekspark-0.0.3/iflytekspark/tests/test_exceptions.py
--rw-r--r--   0 lw         (502) staff       (20)     1430 2023-07-19 10:04:33.000000 iflytekspark-0.0.3/iflytekspark/tests/test_file_cli.py
--rw-r--r--   0 lw         (502) staff       (20)     2034 2023-07-19 10:04:33.000000 iflytekspark-0.0.3/iflytekspark/tests/test_long_examples_validator.py
--rw-r--r--   0 lw         (502) staff       (20)     6572 2023-07-19 10:04:33.000000 iflytekspark-0.0.3/iflytekspark/tests/test_url_composition.py
--rw-r--r--   0 lw         (502) staff       (20)      845 2023-07-19 10:04:33.000000 iflytekspark-0.0.3/iflytekspark/tests/test_util.py
--rw-r--r--   0 lw         (502) staff       (20)     1188 2023-07-19 10:04:33.000000 iflytekspark-0.0.3/iflytekspark/upload_progress.py
--rw-r--r--   0 lw         (502) staff       (20)     5630 2023-07-19 10:04:33.000000 iflytekspark-0.0.3/iflytekspark/util.py
--rw-r--r--   0 lw         (502) staff       (20)    34323 2023-07-19 10:04:33.000000 iflytekspark-0.0.3/iflytekspark/validators.py
--rw-r--r--   0 lw         (502) staff       (20)       18 2023-07-21 02:00:46.000000 iflytekspark-0.0.3/iflytekspark/version.py
--rw-r--r--   0 lw         (502) staff       (20)    10412 2023-07-19 10:04:33.000000 iflytekspark-0.0.3/iflytekspark/wandb_logger.py
-drwxr-xr-x   0 lw         (502) staff       (20)        0 2023-07-21 02:01:47.000000 iflytekspark-0.0.3/iflytekspark.egg-info/
--rw-r--r--   0 lw         (502) staff       (20)    13453 2023-07-21 02:01:47.000000 iflytekspark-0.0.3/iflytekspark.egg-info/PKG-INFO
--rw-r--r--   0 lw         (502) staff       (20)     2441 2023-07-21 02:01:47.000000 iflytekspark-0.0.3/iflytekspark.egg-info/SOURCES.txt
--rw-r--r--   0 lw         (502) staff       (20)        1 2023-07-21 02:01:47.000000 iflytekspark-0.0.3/iflytekspark.egg-info/dependency_links.txt
--rw-r--r--   0 lw         (502) staff       (20)       74 2023-07-21 02:01:47.000000 iflytekspark-0.0.3/iflytekspark.egg-info/entry_points.txt
--rw-r--r--   0 lw         (502) staff       (20)      410 2023-07-21 02:01:47.000000 iflytekspark-0.0.3/iflytekspark.egg-info/requires.txt
--rw-r--r--   0 lw         (502) staff       (20)       13 2023-07-21 02:01:47.000000 iflytekspark-0.0.3/iflytekspark.egg-info/top_level.txt
--rw-r--r--   0 lw         (502) staff       (20)        1 2023-07-21 01:13:29.000000 iflytekspark-0.0.3/iflytekspark.egg-info/zip-safe
--rw-r--r--   0 lw         (502) staff       (20)      244 2023-07-19 09:45:59.000000 iflytekspark-0.0.3/pyproject.toml
--rw-r--r--   0 lw         (502) staff       (20)     1964 2023-07-21 02:01:47.000000 iflytekspark-0.0.3/setup.cfg
--rw-r--r--   0 lw         (502) staff       (20)       38 2023-07-19 09:45:59.000000 iflytekspark-0.0.3/setup.py
+drwxr-xr-x   0 lw         (502) staff       (20)        0 2023-07-21 02:08:36.000000 iflytekspark-0.0.4/
+-rw-r--r--   0 lw         (502) staff       (20)     1095 2023-07-19 09:47:31.000000 iflytekspark-0.0.4/LICENSE
+-rw-r--r--   0 lw         (502) staff       (20)    13453 2023-07-21 02:08:36.000000 iflytekspark-0.0.4/PKG-INFO
+-rw-r--r--   0 lw         (502) staff       (20)    12866 2023-07-19 09:48:24.000000 iflytekspark-0.0.4/README.md
+drwxr-xr-x   0 lw         (502) staff       (20)        0 2023-07-21 02:08:36.000000 iflytekspark-0.0.4/iflytekspark/
+-rw-r--r--   0 lw         (502) staff       (20)     3209 2023-07-21 01:55:54.000000 iflytekspark-0.0.4/iflytekspark/__init__.py
+-rw-r--r--   0 lw         (502) staff       (20)     2630 2023-07-19 10:04:33.000000 iflytekspark-0.0.4/iflytekspark/_iflytekspark_scripts.py
+-rw-r--r--   0 lw         (502) staff       (20)    24702 2023-07-20 11:30:42.000000 iflytekspark-0.0.4/iflytekspark/api_requestor.py
+drwxr-xr-x   0 lw         (502) staff       (20)        0 2023-07-21 02:08:36.000000 iflytekspark-0.0.4/iflytekspark/api_resources/
+-rw-r--r--   0 lw         (502) staff       (20)      991 2023-07-19 10:04:33.000000 iflytekspark-0.0.4/iflytekspark/api_resources/__init__.py
+drwxr-xr-x   0 lw         (502) staff       (20)        0 2023-07-21 02:08:36.000000 iflytekspark-0.0.4/iflytekspark/api_resources/abstract/
+-rw-r--r--   0 lw         (502) staff       (20)      576 2023-07-19 10:04:33.000000 iflytekspark-0.0.4/iflytekspark/api_resources/abstract/__init__.py
+-rw-r--r--   0 lw         (502) staff       (20)     5515 2023-07-19 10:04:33.000000 iflytekspark-0.0.4/iflytekspark/api_resources/abstract/api_resource.py
+-rw-r--r--   0 lw         (502) staff       (20)     2603 2023-07-19 10:04:33.000000 iflytekspark-0.0.4/iflytekspark/api_resources/abstract/createable_api_resource.py
+-rw-r--r--   0 lw         (502) staff       (20)     1642 2023-07-19 10:04:33.000000 iflytekspark-0.0.4/iflytekspark/api_resources/abstract/deletable_api_resource.py
+-rw-r--r--   0 lw         (502) staff       (20)    10097 2023-07-19 10:04:33.000000 iflytekspark-0.0.4/iflytekspark/api_resources/abstract/engine_api_resource.py
+-rw-r--r--   0 lw         (502) staff       (20)     2744 2023-07-19 10:04:33.000000 iflytekspark-0.0.4/iflytekspark/api_resources/abstract/listable_api_resource.py
+-rw-r--r--   0 lw         (502) staff       (20)     5104 2023-07-19 10:04:33.000000 iflytekspark-0.0.4/iflytekspark/api_resources/abstract/nested_resource_class_methods.py
+-rw-r--r--   0 lw         (502) staff       (20)      540 2023-07-19 10:04:33.000000 iflytekspark-0.0.4/iflytekspark/api_resources/abstract/updateable_api_resource.py
+-rw-r--r--   0 lw         (502) staff       (20)     7122 2023-07-19 10:04:33.000000 iflytekspark-0.0.4/iflytekspark/api_resources/audio.py
+-rw-r--r--   0 lw         (502) staff       (20)     1617 2023-07-19 10:04:33.000000 iflytekspark-0.0.4/iflytekspark/api_resources/chat_completion.py
+-rw-r--r--   0 lw         (502) staff       (20)     1646 2023-07-19 10:04:33.000000 iflytekspark-0.0.4/iflytekspark/api_resources/completion.py
+-rw-r--r--   0 lw         (502) staff       (20)      563 2023-07-19 10:04:33.000000 iflytekspark-0.0.4/iflytekspark/api_resources/customer.py
+-rw-r--r--   0 lw         (502) staff       (20)     4073 2023-07-19 10:04:33.000000 iflytekspark-0.0.4/iflytekspark/api_resources/deployment.py
+-rw-r--r--   0 lw         (502) staff       (20)     1993 2023-07-19 10:04:33.000000 iflytekspark-0.0.4/iflytekspark/api_resources/edit.py
+-rw-r--r--   0 lw         (502) staff       (20)     3480 2023-07-19 10:04:33.000000 iflytekspark-0.0.4/iflytekspark/api_resources/embedding.py
+-rw-r--r--   0 lw         (502) staff       (20)     1683 2023-07-19 10:04:33.000000 iflytekspark-0.0.4/iflytekspark/api_resources/engine.py
+-rw-r--r--   0 lw         (502) staff       (20)      922 2023-07-19 10:04:33.000000 iflytekspark-0.0.4/iflytekspark/api_resources/error_object.py
+drwxr-xr-x   0 lw         (502) staff       (20)        0 2023-07-21 02:08:36.000000 iflytekspark-0.0.4/iflytekspark/api_resources/experimental/
+-rw-r--r--   0 lw         (502) staff       (20)      110 2023-07-19 10:04:33.000000 iflytekspark-0.0.4/iflytekspark/api_resources/experimental/__init__.py
+-rw-r--r--   0 lw         (502) staff       (20)      280 2023-07-19 10:04:33.000000 iflytekspark-0.0.4/iflytekspark/api_resources/experimental/completion_config.py
+-rw-r--r--   0 lw         (502) staff       (20)     7797 2023-07-19 10:04:33.000000 iflytekspark-0.0.4/iflytekspark/api_resources/file.py
+-rw-r--r--   0 lw         (502) staff       (20)     5329 2023-07-19 10:04:33.000000 iflytekspark-0.0.4/iflytekspark/api_resources/fine_tune.py
+-rw-r--r--   0 lw         (502) staff       (20)     6345 2023-07-19 10:04:33.000000 iflytekspark-0.0.4/iflytekspark/api_resources/image.py
+-rw-r--r--   0 lw         (502) staff       (20)      175 2023-07-19 10:04:33.000000 iflytekspark-0.0.4/iflytekspark/api_resources/model.py
+-rw-r--r--   0 lw         (502) staff       (20)     1400 2023-07-19 10:04:33.000000 iflytekspark-0.0.4/iflytekspark/api_resources/moderation.py
+-rw-r--r--   0 lw         (502) staff       (20)    38806 2023-07-19 10:04:33.000000 iflytekspark-0.0.4/iflytekspark/cli.py
+drwxr-xr-x   0 lw         (502) staff       (20)        0 2023-07-21 02:08:36.000000 iflytekspark-0.0.4/iflytekspark/datalib/
+-rw-r--r--   0 lw         (502) staff       (20)      657 2023-07-19 10:04:33.000000 iflytekspark-0.0.4/iflytekspark/datalib/__init__.py
+-rw-r--r--   0 lw         (502) staff       (20)      270 2023-07-19 10:04:33.000000 iflytekspark-0.0.4/iflytekspark/datalib/common.py
+-rw-r--r--   0 lw         (502) staff       (20)      326 2023-07-19 10:04:33.000000 iflytekspark-0.0.4/iflytekspark/datalib/numpy_helper.py
+-rw-r--r--   0 lw         (502) staff       (20)      335 2023-07-19 10:04:33.000000 iflytekspark-0.0.4/iflytekspark/datalib/pandas_helper.py
+-rw-r--r--   0 lw         (502) staff       (20)     8634 2023-07-19 10:04:33.000000 iflytekspark-0.0.4/iflytekspark/embeddings_utils.py
+-rw-r--r--   0 lw         (502) staff       (20)     4406 2023-07-19 10:04:33.000000 iflytekspark-0.0.4/iflytekspark/error.py
+-rw-r--r--   0 lw         (502) staff       (20)    10946 2023-07-19 10:04:33.000000 iflytekspark-0.0.4/iflytekspark/iflytekspark_object.py
+-rw-r--r--   0 lw         (502) staff       (20)      554 2023-07-19 10:04:33.000000 iflytekspark-0.0.4/iflytekspark/iflytekspark_response.py
+-rw-r--r--   0 lw         (502) staff       (20)      391 2023-07-19 10:04:33.000000 iflytekspark-0.0.4/iflytekspark/object_classes.py
+-rw-------   0 lw         (502) staff       (20)     6571 2023-07-21 02:07:14.000000 iflytekspark-0.0.4/iflytekspark/sparkwbwrap.py
+drwxr-xr-x   0 lw         (502) staff       (20)        0 2023-07-21 02:08:36.000000 iflytekspark-0.0.4/iflytekspark/tests/
+-rw-r--r--   0 lw         (502) staff       (20)        0 2023-07-19 10:04:33.000000 iflytekspark-0.0.4/iflytekspark/tests/__init__.py
+drwxr-xr-x   0 lw         (502) staff       (20)        0 2023-07-21 02:08:36.000000 iflytekspark-0.0.4/iflytekspark/tests/asyncio/
+-rw-r--r--   0 lw         (502) staff       (20)        0 2023-07-19 10:04:33.000000 iflytekspark-0.0.4/iflytekspark/tests/asyncio/__init__.py
+-rw-r--r--   0 lw         (502) staff       (20)     2434 2023-07-19 10:04:33.000000 iflytekspark-0.0.4/iflytekspark/tests/asyncio/test_endpoints.py
+-rw-r--r--   0 lw         (502) staff       (20)     2366 2023-07-19 10:04:33.000000 iflytekspark-0.0.4/iflytekspark/tests/test_api_requestor.py
+-rw-r--r--   0 lw         (502) staff       (20)     2963 2023-07-19 10:04:33.000000 iflytekspark-0.0.4/iflytekspark/tests/test_endpoints.py
+-rw-r--r--   0 lw         (502) staff       (20)     1234 2023-07-19 10:04:33.000000 iflytekspark-0.0.4/iflytekspark/tests/test_exceptions.py
+-rw-r--r--   0 lw         (502) staff       (20)     1430 2023-07-19 10:04:33.000000 iflytekspark-0.0.4/iflytekspark/tests/test_file_cli.py
+-rw-r--r--   0 lw         (502) staff       (20)     2034 2023-07-19 10:04:33.000000 iflytekspark-0.0.4/iflytekspark/tests/test_long_examples_validator.py
+-rw-r--r--   0 lw         (502) staff       (20)     6572 2023-07-19 10:04:33.000000 iflytekspark-0.0.4/iflytekspark/tests/test_url_composition.py
+-rw-r--r--   0 lw         (502) staff       (20)      845 2023-07-19 10:04:33.000000 iflytekspark-0.0.4/iflytekspark/tests/test_util.py
+-rw-r--r--   0 lw         (502) staff       (20)     1188 2023-07-19 10:04:33.000000 iflytekspark-0.0.4/iflytekspark/upload_progress.py
+-rw-r--r--   0 lw         (502) staff       (20)     5630 2023-07-19 10:04:33.000000 iflytekspark-0.0.4/iflytekspark/util.py
+-rw-r--r--   0 lw         (502) staff       (20)    34323 2023-07-19 10:04:33.000000 iflytekspark-0.0.4/iflytekspark/validators.py
+-rw-r--r--   0 lw         (502) staff       (20)       19 2023-07-21 02:08:01.000000 iflytekspark-0.0.4/iflytekspark/version.py
+-rw-r--r--   0 lw         (502) staff       (20)    10412 2023-07-19 10:04:33.000000 iflytekspark-0.0.4/iflytekspark/wandb_logger.py
+drwxr-xr-x   0 lw         (502) staff       (20)        0 2023-07-21 02:08:36.000000 iflytekspark-0.0.4/iflytekspark.egg-info/
+-rw-r--r--   0 lw         (502) staff       (20)    13453 2023-07-21 02:08:36.000000 iflytekspark-0.0.4/iflytekspark.egg-info/PKG-INFO
+-rw-r--r--   0 lw         (502) staff       (20)     2441 2023-07-21 02:08:36.000000 iflytekspark-0.0.4/iflytekspark.egg-info/SOURCES.txt
+-rw-r--r--   0 lw         (502) staff       (20)        1 2023-07-21 02:08:36.000000 iflytekspark-0.0.4/iflytekspark.egg-info/dependency_links.txt
+-rw-r--r--   0 lw         (502) staff       (20)       74 2023-07-21 02:08:36.000000 iflytekspark-0.0.4/iflytekspark.egg-info/entry_points.txt
+-rw-r--r--   0 lw         (502) staff       (20)      410 2023-07-21 02:08:36.000000 iflytekspark-0.0.4/iflytekspark.egg-info/requires.txt
+-rw-r--r--   0 lw         (502) staff       (20)       13 2023-07-21 02:08:36.000000 iflytekspark-0.0.4/iflytekspark.egg-info/top_level.txt
+-rw-r--r--   0 lw         (502) staff       (20)        1 2023-07-21 01:13:29.000000 iflytekspark-0.0.4/iflytekspark.egg-info/zip-safe
+-rw-r--r--   0 lw         (502) staff       (20)      244 2023-07-19 09:45:59.000000 iflytekspark-0.0.4/pyproject.toml
+-rw-r--r--   0 lw         (502) staff       (20)     1964 2023-07-21 02:08:36.000000 iflytekspark-0.0.4/setup.cfg
+-rw-r--r--   0 lw         (502) staff       (20)       38 2023-07-19 09:45:59.000000 iflytekspark-0.0.4/setup.py
```

### Comparing `iflytekspark-0.0.3/LICENSE` & `iflytekspark-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `iflytekspark-0.0.3/PKG-INFO` & `iflytekspark-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iflytekspark
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python client library for the Iflytekspark API
 Home-page: https://github.com/wljince007/openai-python
 Author: wljince007
 Author-email: liangwang007@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `iflytekspark-0.0.3/README.md` & `iflytekspark-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `iflytekspark-0.0.3/iflytekspark/__init__.py` & `iflytekspark-0.0.4/iflytekspark/__init__.py`

 * *Files identical despite different names*

### Comparing `iflytekspark-0.0.3/iflytekspark/_iflytekspark_scripts.py` & `iflytekspark-0.0.4/iflytekspark/_iflytekspark_scripts.py`

 * *Files identical despite different names*

### Comparing `iflytekspark-0.0.3/iflytekspark/api_requestor.py` & `iflytekspark-0.0.4/iflytekspark/api_requestor.py`

 * *Files identical despite different names*

### Comparing `iflytekspark-0.0.3/iflytekspark/api_resources/__init__.py` & `iflytekspark-0.0.4/iflytekspark/api_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `iflytekspark-0.0.3/iflytekspark/api_resources/abstract/__init__.py` & `iflytekspark-0.0.4/iflytekspark/api_resources/abstract/__init__.py`

 * *Files identical despite different names*

### Comparing `iflytekspark-0.0.3/iflytekspark/api_resources/abstract/api_resource.py` & `iflytekspark-0.0.4/iflytekspark/api_resources/abstract/api_resource.py`

 * *Files identical despite different names*

### Comparing `iflytekspark-0.0.3/iflytekspark/api_resources/abstract/createable_api_resource.py` & `iflytekspark-0.0.4/iflytekspark/api_resources/abstract/createable_api_resource.py`

 * *Files identical despite different names*

### Comparing `iflytekspark-0.0.3/iflytekspark/api_resources/abstract/deletable_api_resource.py` & `iflytekspark-0.0.4/iflytekspark/api_resources/abstract/deletable_api_resource.py`

 * *Files identical despite different names*

### Comparing `iflytekspark-0.0.3/iflytekspark/api_resources/abstract/engine_api_resource.py` & `iflytekspark-0.0.4/iflytekspark/api_resources/abstract/engine_api_resource.py`

 * *Files identical despite different names*

### Comparing `iflytekspark-0.0.3/iflytekspark/api_resources/abstract/listable_api_resource.py` & `iflytekspark-0.0.4/iflytekspark/api_resources/abstract/listable_api_resource.py`

 * *Files identical despite different names*

### Comparing `iflytekspark-0.0.3/iflytekspark/api_resources/abstract/nested_resource_class_methods.py` & `iflytekspark-0.0.4/iflytekspark/api_resources/abstract/nested_resource_class_methods.py`

 * *Files identical despite different names*

### Comparing `iflytekspark-0.0.3/iflytekspark/api_resources/abstract/updateable_api_resource.py` & `iflytekspark-0.0.4/iflytekspark/api_resources/abstract/updateable_api_resource.py`

 * *Files identical despite different names*

### Comparing `iflytekspark-0.0.3/iflytekspark/api_resources/audio.py` & `iflytekspark-0.0.4/iflytekspark/api_resources/audio.py`

 * *Files identical despite different names*

### Comparing `iflytekspark-0.0.3/iflytekspark/api_resources/chat_completion.py` & `iflytekspark-0.0.4/iflytekspark/api_resources/chat_completion.py`

 * *Files identical despite different names*

### Comparing `iflytekspark-0.0.3/iflytekspark/api_resources/completion.py` & `iflytekspark-0.0.4/iflytekspark/api_resources/completion.py`

 * *Files identical despite different names*

### Comparing `iflytekspark-0.0.3/iflytekspark/api_resources/customer.py` & `iflytekspark-0.0.4/iflytekspark/api_resources/customer.py`

 * *Files identical despite different names*

### Comparing `iflytekspark-0.0.3/iflytekspark/api_resources/deployment.py` & `iflytekspark-0.0.4/iflytekspark/api_resources/deployment.py`

 * *Files identical despite different names*

### Comparing `iflytekspark-0.0.3/iflytekspark/api_resources/edit.py` & `iflytekspark-0.0.4/iflytekspark/api_resources/edit.py`

 * *Files identical despite different names*

### Comparing `iflytekspark-0.0.3/iflytekspark/api_resources/embedding.py` & `iflytekspark-0.0.4/iflytekspark/api_resources/embedding.py`

 * *Files identical despite different names*

### Comparing `iflytekspark-0.0.3/iflytekspark/api_resources/engine.py` & `iflytekspark-0.0.4/iflytekspark/api_resources/engine.py`

 * *Files identical despite different names*

### Comparing `iflytekspark-0.0.3/iflytekspark/api_resources/error_object.py` & `iflytekspark-0.0.4/iflytekspark/api_resources/error_object.py`

 * *Files identical despite different names*

### Comparing `iflytekspark-0.0.3/iflytekspark/api_resources/file.py` & `iflytekspark-0.0.4/iflytekspark/api_resources/file.py`

 * *Files identical despite different names*

### Comparing `iflytekspark-0.0.3/iflytekspark/api_resources/fine_tune.py` & `iflytekspark-0.0.4/iflytekspark/api_resources/fine_tune.py`

 * *Files identical despite different names*

### Comparing `iflytekspark-0.0.3/iflytekspark/api_resources/image.py` & `iflytekspark-0.0.4/iflytekspark/api_resources/image.py`

 * *Files identical despite different names*

### Comparing `iflytekspark-0.0.3/iflytekspark/api_resources/moderation.py` & `iflytekspark-0.0.4/iflytekspark/api_resources/moderation.py`

 * *Files identical despite different names*

### Comparing `iflytekspark-0.0.3/iflytekspark/cli.py` & `iflytekspark-0.0.4/iflytekspark/cli.py`

 * *Files identical despite different names*

### Comparing `iflytekspark-0.0.3/iflytekspark/datalib/__init__.py` & `iflytekspark-0.0.4/iflytekspark/datalib/__init__.py`

 * *Files identical despite different names*

### Comparing `iflytekspark-0.0.3/iflytekspark/embeddings_utils.py` & `iflytekspark-0.0.4/iflytekspark/embeddings_utils.py`

 * *Files identical despite different names*

### Comparing `iflytekspark-0.0.3/iflytekspark/error.py` & `iflytekspark-0.0.4/iflytekspark/error.py`

 * *Files identical despite different names*

### Comparing `iflytekspark-0.0.3/iflytekspark/iflytekspark_object.py` & `iflytekspark-0.0.4/iflytekspark/iflytekspark_object.py`

 * *Files identical despite different names*

### Comparing `iflytekspark-0.0.3/iflytekspark/iflytekspark_response.py` & `iflytekspark-0.0.4/iflytekspark/iflytekspark_response.py`

 * *Files identical despite different names*

### Comparing `iflytekspark-0.0.3/iflytekspark/sparkwbwrap.py` & `iflytekspark-0.0.4/iflytekspark/sparkwbwrap.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,17 +62,17 @@
         ws = None
         try:
             # 创建客户端与服务端的连接
             appId     = iflytekspark.app_id
             apiSecret = iflytekspark.api_secret
             apiKey    = iflytekspark.api_key
             addr = iflytekspark.api_base
-            
+
             authAddr = addr
-            if  iflytekspark.api_url_process == '' :
+            if  iflytekspark.api_url_process == 'assemble' :
                 authAddr = assemble_auth_url("GET", addr, apiKey, apiSecret)
             connectionUrl = authAddr
             util.log_debug("Spark url", url=connectionUrl)
             ws = websocket.create_connection(connectionUrl)
 
 
             # params='{"prompt": ["What would be a good company name for a company that makes colorful socks?"], "model": "text-davinci-003", "temperature": 0.9, "max_tokens": 256, "top_p": 1, "frequency_penalty": 0, "presence_penalty": 0, "n": 1, "logit_bias": {}}'
```

### Comparing `iflytekspark-0.0.3/iflytekspark/tests/asyncio/test_endpoints.py` & `iflytekspark-0.0.4/iflytekspark/tests/asyncio/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `iflytekspark-0.0.3/iflytekspark/tests/test_api_requestor.py` & `iflytekspark-0.0.4/iflytekspark/tests/test_api_requestor.py`

 * *Files identical despite different names*

### Comparing `iflytekspark-0.0.3/iflytekspark/tests/test_endpoints.py` & `iflytekspark-0.0.4/iflytekspark/tests/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `iflytekspark-0.0.3/iflytekspark/tests/test_exceptions.py` & `iflytekspark-0.0.4/iflytekspark/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `iflytekspark-0.0.3/iflytekspark/tests/test_file_cli.py` & `iflytekspark-0.0.4/iflytekspark/tests/test_file_cli.py`

 * *Files identical despite different names*

### Comparing `iflytekspark-0.0.3/iflytekspark/tests/test_long_examples_validator.py` & `iflytekspark-0.0.4/iflytekspark/tests/test_long_examples_validator.py`

 * *Files identical despite different names*

### Comparing `iflytekspark-0.0.3/iflytekspark/tests/test_url_composition.py` & `iflytekspark-0.0.4/iflytekspark/tests/test_url_composition.py`

 * *Files identical despite different names*

### Comparing `iflytekspark-0.0.3/iflytekspark/tests/test_util.py` & `iflytekspark-0.0.4/iflytekspark/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `iflytekspark-0.0.3/iflytekspark/upload_progress.py` & `iflytekspark-0.0.4/iflytekspark/upload_progress.py`

 * *Files identical despite different names*

### Comparing `iflytekspark-0.0.3/iflytekspark/util.py` & `iflytekspark-0.0.4/iflytekspark/util.py`

 * *Files identical despite different names*

### Comparing `iflytekspark-0.0.3/iflytekspark/validators.py` & `iflytekspark-0.0.4/iflytekspark/validators.py`

 * *Files identical despite different names*

### Comparing `iflytekspark-0.0.3/iflytekspark/wandb_logger.py` & `iflytekspark-0.0.4/iflytekspark/wandb_logger.py`

 * *Files identical despite different names*

### Comparing `iflytekspark-0.0.3/iflytekspark.egg-info/PKG-INFO` & `iflytekspark-0.0.4/iflytekspark.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iflytekspark
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python client library for the Iflytekspark API
 Home-page: https://github.com/wljince007/openai-python
 Author: wljince007
 Author-email: liangwang007@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `iflytekspark-0.0.3/iflytekspark.egg-info/SOURCES.txt` & `iflytekspark-0.0.4/iflytekspark.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iflytekspark-0.0.3/setup.cfg` & `iflytekspark-0.0.4/setup.cfg`

 * *Files identical despite different names*

