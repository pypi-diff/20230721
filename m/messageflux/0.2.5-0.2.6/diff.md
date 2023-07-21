# Comparing `tmp/messageflux-0.2.5.tar.gz` & `tmp/messageflux-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "messageflux-0.2.5.tar", last modified: Wed May  3 16:31:02 2023, max compression
+gzip compressed data, was "messageflux-0.2.6.tar", last modified: Fri Jul 21 12:02:36 2023, max compression
```

## Comparing `messageflux-0.2.5.tar` & `messageflux-0.2.6.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:31:02.331659 messageflux-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-03 16:30:46.000000 messageflux-0.2.5/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-03 16:30:46.000000 messageflux-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-03 16:30:46.000000 messageflux-0.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-05-03 16:31:02.331659 messageflux-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-05-03 16:30:46.000000 messageflux-0.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-03 16:30:47.000000 messageflux-0.2.5/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:31:02.311658 messageflux-0.2.5/_custom_build/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 16:30:46.000000 messageflux-0.2.5/_custom_build/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-03 16:30:46.000000 messageflux-0.2.5/_custom_build/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-03 16:30:46.000000 messageflux-0.2.5/_custom_build/make_all_extra_requirements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:31:02.311658 messageflux-0.2.5/messageflux/
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/base_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     8837 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/fastmessage_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:31:02.315658 messageflux-0.2.5/messageflux/iodevices/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/iodevices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:31:02.315658 messageflux-0.2.5/messageflux/iodevices/base/
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/iodevices/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/iodevices/base/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     9978 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/iodevices/base/input_devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     6594 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/iodevices/base/input_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/iodevices/base/output_devices.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:31:02.315658 messageflux-0.2.5/messageflux/iodevices/collection_device_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/iodevices/collection_device_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6135 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/iodevices/collection_device_wrapper/collection_input_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/iodevices/collection_device_wrapper/collection_output_device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:31:02.315658 messageflux-0.2.5/messageflux/iodevices/failover_output_device_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/iodevices/failover_output_device_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/iodevices/failover_output_device_wrapper/failover_output_device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:31:02.319658 messageflux-0.2.5/messageflux/iodevices/file_system/
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/iodevices/file_system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/iodevices/file_system/file_system_device_manager_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    24466 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/iodevices/file_system/file_system_input_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/iodevices/file_system/file_system_output_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/iodevices/file_system/file_system_serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:31:02.319658 messageflux-0.2.5/messageflux/iodevices/in_memory_device/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/iodevices/in_memory_device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/iodevices/in_memory_device/in_memory_device_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:31:02.319658 messageflux-0.2.5/messageflux/iodevices/message_store_device_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/iodevices/message_store_device_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/iodevices/message_store_device_wrapper/file_system_message_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/iodevices/message_store_device_wrapper/message_store_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/iodevices/message_store_device_wrapper/message_store_input_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/iodevices/message_store_device_wrapper/message_store_output_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/iodevices/message_store_device_wrapper/message_store_transformer_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:31:02.319658 messageflux-0.2.5/messageflux/iodevices/objectstorage/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/iodevices/objectstorage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11333 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/iodevices/objectstorage/s3_message_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:31:02.323659 messageflux-0.2.5/messageflux/iodevices/objectstorage/s3api/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/iodevices/objectstorage/s3api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14461 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/iodevices/objectstorage/s3api/s3bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/iodevices/objectstorage/s3api/s3client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:31:02.323659 messageflux-0.2.5/messageflux/iodevices/rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/iodevices/rabbitmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/iodevices/rabbitmq/fs_poison_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)    14045 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/iodevices/rabbitmq/rabbitmq_device_manager_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    16736 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/iodevices/rabbitmq/rabbitmq_input_device.py
--rw-r--r--   0 runner    (1001) docker     (123)    15636 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/iodevices/rabbitmq/rabbitmq_output_device.py
--rw-r--r--   0 runner    (1001) docker     (123)    12168 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/iodevices/rabbitmq/rabbitmq_poison_counting_input_device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:31:02.323659 messageflux-0.2.5/messageflux/iodevices/round_robin_device_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/iodevices/round_robin_device_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/iodevices/round_robin_device_wrapper/roundrobin_io_device_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:31:02.323659 messageflux-0.2.5/messageflux/iodevices/short_circuit_device_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/iodevices/short_circuit_device_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/iodevices/short_circuit_device_wrapper/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/iodevices/short_circuit_device_wrapper/short_circuit_input_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/iodevices/short_circuit_device_wrapper/short_circuit_output_device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:31:02.327659 messageflux-0.2.5/messageflux/iodevices/transformer_device_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/iodevices/transformer_device_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/iodevices/transformer_device_wrapper/transformer_input_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/iodevices/transformer_device_wrapper/transformer_output_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/iodevices/transformer_device_wrapper/zlib_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:31:02.327659 messageflux-0.2.5/messageflux/logging/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/logging/LogType.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/logging/bulk_rotating_device_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/logging/bulk_rotating_file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7545 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/logging/bulk_rotating_handler_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/logging/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/message_handling_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/metadata_headers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:31:02.327659 messageflux-0.2.5/messageflux/multiprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/multiprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/multiprocessing/multiprocessrunner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6360 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/multiprocessing/singleprocesshandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/pipeline_service.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/server_loop_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:31:02.327659 messageflux-0.2.5/messageflux/service_addons/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/service_addons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/service_addons/loop_health_addon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:31:02.327659 messageflux-0.2.5/messageflux/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/utils/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-05-03 16:30:46.000000 messageflux-0.2.5/messageflux/utils/filesystem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:31:02.315658 messageflux-0.2.5/messageflux.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-05-03 16:31:02.000000 messageflux-0.2.5/messageflux.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-05-03 16:31:02.000000 messageflux-0.2.5/messageflux.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 16:31:02.000000 messageflux-0.2.5/messageflux.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-03 16:31:02.000000 messageflux-0.2.5/messageflux.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-03 16:31:02.000000 messageflux-0.2.5/messageflux.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-03 16:30:46.000000 messageflux-0.2.5/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-03 16:30:46.000000 messageflux-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-03 16:30:46.000000 messageflux-0.2.5/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-03 16:31:02.000000 messageflux-0.2.5/requirements-all.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-03 16:30:46.000000 messageflux-0.2.5/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-03 16:30:46.000000 messageflux-0.2.5/requirements-fastmessage.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-03 16:30:46.000000 messageflux-0.2.5/requirements-objectstorage.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-03 16:30:46.000000 messageflux-0.2.5/requirements-rabbitmq.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 16:30:46.000000 messageflux-0.2.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 16:31:02.331659 messageflux-0.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:02:36.229842 messageflux-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-21 12:02:23.000000 messageflux-0.2.6/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-21 12:02:23.000000 messageflux-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-21 12:02:23.000000 messageflux-0.2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-07-21 12:02:36.229842 messageflux-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-07-21 12:02:23.000000 messageflux-0.2.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-21 12:02:24.000000 messageflux-0.2.6/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:02:36.213842 messageflux-0.2.6/_custom_build/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 12:02:23.000000 messageflux-0.2.6/_custom_build/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-21 12:02:23.000000 messageflux-0.2.6/_custom_build/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-21 12:02:23.000000 messageflux-0.2.6/_custom_build/make_all_extra_requirements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:02:36.217841 messageflux-0.2.6/messageflux/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/base_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10055 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/fastmessage_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:02:36.217841 messageflux-0.2.6/messageflux/iodevices/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:02:36.217841 messageflux-0.2.6/messageflux/iodevices/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/base/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9978 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/base/input_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6594 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/base/input_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/base/output_devices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:02:36.221841 messageflux-0.2.6/messageflux/iodevices/collection_device_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/collection_device_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6135 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/collection_device_wrapper/collection_input_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/collection_device_wrapper/collection_output_device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:02:36.221841 messageflux-0.2.6/messageflux/iodevices/failover_output_device_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/failover_output_device_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/failover_output_device_wrapper/failover_output_device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:02:36.221841 messageflux-0.2.6/messageflux/iodevices/file_system/
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/file_system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/file_system/file_system_device_manager_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24466 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/file_system/file_system_input_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/file_system/file_system_output_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/file_system/file_system_serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:02:36.221841 messageflux-0.2.6/messageflux/iodevices/in_memory_device/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/in_memory_device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/in_memory_device/in_memory_device_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:02:36.221841 messageflux-0.2.6/messageflux/iodevices/message_store_device_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/message_store_device_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/message_store_device_wrapper/file_system_message_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/message_store_device_wrapper/message_store_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/message_store_device_wrapper/message_store_input_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/message_store_device_wrapper/message_store_output_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/message_store_device_wrapper/message_store_transformer_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:02:36.225842 messageflux-0.2.6/messageflux/iodevices/objectstorage/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/objectstorage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11333 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/objectstorage/s3_message_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:02:36.225842 messageflux-0.2.6/messageflux/iodevices/objectstorage/s3api/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/objectstorage/s3api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14461 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/objectstorage/s3api/s3bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/objectstorage/s3api/s3client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:02:36.225842 messageflux-0.2.6/messageflux/iodevices/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/rabbitmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/rabbitmq/fs_poison_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14045 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/rabbitmq/rabbitmq_device_manager_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16736 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/rabbitmq/rabbitmq_input_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15636 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/rabbitmq/rabbitmq_output_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12168 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/rabbitmq/rabbitmq_poison_counting_input_device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:02:36.225842 messageflux-0.2.6/messageflux/iodevices/round_robin_device_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/round_robin_device_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/round_robin_device_wrapper/roundrobin_io_device_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:02:36.225842 messageflux-0.2.6/messageflux/iodevices/short_circuit_device_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/short_circuit_device_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/short_circuit_device_wrapper/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/short_circuit_device_wrapper/short_circuit_input_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/short_circuit_device_wrapper/short_circuit_output_device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:02:36.229842 messageflux-0.2.6/messageflux/iodevices/transformer_device_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/transformer_device_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/transformer_device_wrapper/transformer_input_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/transformer_device_wrapper/transformer_output_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/transformer_device_wrapper/zlib_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:02:36.229842 messageflux-0.2.6/messageflux/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/logging/LogType.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/logging/bulk_rotating_device_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/logging/bulk_rotating_file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7545 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/logging/bulk_rotating_handler_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/logging/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/message_handling_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/metadata_headers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:02:36.229842 messageflux-0.2.6/messageflux/multiprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/multiprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/multiprocessing/multiprocessrunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6360 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/multiprocessing/singleprocesshandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/pipeline_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/server_loop_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:02:36.229842 messageflux-0.2.6/messageflux/service_addons/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/service_addons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/service_addons/loop_health_addon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:02:36.229842 messageflux-0.2.6/messageflux/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/utils/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/utils/filesystem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:02:36.217841 messageflux-0.2.6/messageflux.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-07-21 12:02:36.000000 messageflux-0.2.6/messageflux.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-07-21 12:02:36.000000 messageflux-0.2.6/messageflux.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 12:02:36.000000 messageflux-0.2.6/messageflux.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-21 12:02:36.000000 messageflux-0.2.6/messageflux.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-21 12:02:36.000000 messageflux-0.2.6/messageflux.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-21 12:02:23.000000 messageflux-0.2.6/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-21 12:02:23.000000 messageflux-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-21 12:02:23.000000 messageflux-0.2.6/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-21 12:02:36.000000 messageflux-0.2.6/requirements-all.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-21 12:02:23.000000 messageflux-0.2.6/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-21 12:02:23.000000 messageflux-0.2.6/requirements-fastmessage.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-21 12:02:23.000000 messageflux-0.2.6/requirements-objectstorage.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-21 12:02:23.000000 messageflux-0.2.6/requirements-rabbitmq.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 12:02:23.000000 messageflux-0.2.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 12:02:36.229842 messageflux-0.2.6/setup.cfg
```

### Comparing `messageflux-0.2.5/LICENSE` & `messageflux-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.5/PKG-INFO` & `messageflux-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: messageflux
-Version: 0.2.5
+Version: 0.2.6
 Author-email: Aviv Salem <avivsalem@gmail.com>
 Maintainer-email: Aviv Salem <avivsalem@gmail.com>, Nir Schulman <narsssx@gmail.com>, Rafael Zilberman <Zilberman.rafi@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Avivsalem/MessageFlux/
 Project-URL: Documentation, https://messageflux.readthedocs.io/
 Platform: win32
 Platform: linux
```

### Comparing `messageflux-0.2.5/README.md` & `messageflux-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.5/_custom_build/make_all_extra_requirements.py` & `messageflux-0.2.6/_custom_build/make_all_extra_requirements.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.5/messageflux/base_service.py` & `messageflux-0.2.6/messageflux/base_service.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.5/messageflux/fastmessage_handler.py` & `messageflux-0.2.6/messageflux/fastmessage_handler.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,59 @@
 import inspect
 import json
 import logging
 from dataclasses import dataclass
-from inspect import Parameter
-from typing import Optional, Callable, Dict, List, Any, TypeVar
+from typing import Optional, Callable, Dict, List, Any, TypeVar, Union
 
 from messageflux import InputDevice
 from messageflux.iodevices.base.common import MessageBundle, Message
 from messageflux.pipeline_service import PipelineHandlerBase, PipelineResult
 
 try:
-    from pydantic import BaseModel, parse_raw_as, create_model, ValidationError
+    from pydantic.typing import get_all_type_hints
+    from pydantic import BaseModel, parse_raw_as, create_model, ValidationError, Extra
+    from pydantic.config import get_config
 except ImportError as ex:
     raise ImportError('Please Install the required extra: messageflux[fastmessage]') from ex
 
 
 class FastMessageException(Exception):
     pass
 
 
 class DuplicateCallbackException(FastMessageException):
     pass
 
 
-class MissingCallbackException(FastMessageException):
+class NotAllowedParamKindException(FastMessageException):
     pass
 
 
-class NonAnnotatedParamException(FastMessageException):
+class MissingCallbackException(FastMessageException):
     pass
 
 
 class SpecialDefaultValueException(FastMessageException):
     pass
 
 
 class InputDeviceName(str):
     """
     a place holder class for input_device name
     """
     pass
 
 
+class MultipleReturnValues(list):
+    """
+    a value that indicates that multiple output values should be returned
+    """
+    pass
+
+
 class _DefaultClass(str):
     pass
 
 
 _DEFAULT = _DefaultClass()
 _CALLABLE_TYPE = TypeVar('_CALLABLE_TYPE', bound=Callable[..., Any])
 
@@ -64,88 +72,106 @@
                  input_device: str,
                  output_device: Optional[str] = None):
         self._callback = callback
         self._input_device = input_device
         self._output_device = output_device
         self._special_params: Dict[str, _ParamInfo] = dict()
         self._params: Dict[str, _ParamInfo] = dict()
+        type_hints = get_all_type_hints(self._callback)
+        extra = Extra.ignore
         for param_name, param in inspect.signature(self._callback).parameters.items():
-            param_info = _ParamInfo(annotation=param.annotation, default=param.default)
-            if param_info.annotation is Parameter.empty:
-                if param_info.default is not Parameter.empty:
-                    param_info.annotation = type(param_info.default)
-                else:
-                    raise NonAnnotatedParamException(
-                        f"method param '{param_name}' is not type annotated and has no default")
-
-            if param_info.annotation in (MessageBundle, Message, InputDeviceName):
-                if param_info.default is not Parameter.empty:
+            if param.kind in (param.POSITIONAL_ONLY, param.VAR_POSITIONAL):
+                raise NotAllowedParamKindException(
+                    f"param '{param_name}' is of '{param.kind}' kind. this is now allowed")
+
+            if param.kind == param.VAR_KEYWORD:  # there's **kwargs param
+                extra = Extra.allow
+                continue
+
+            annotation = Any if param.annotation is param.empty else type_hints[param_name]
+            default = ... if param.default is param.empty else param.default
+
+            param_info = _ParamInfo(annotation=annotation, default=default)
+
+            if param_info.annotation in (MessageBundle, Message, InputDeviceName,
+                                         Optional[MessageBundle], Optional[Message], Optional[InputDeviceName]):
+                if param_info.default is not ...:
                     raise SpecialDefaultValueException(
-                        f"param '{param_name}' is of special type '{param_info.annotation.__name__}' "
+                        f"param '{param_name}' is of special type '{param.annotation.__name__}' "
                         f"but has a default value")
                 self._special_params[param_name] = param_info
 
             else:
                 self._params[param_name] = param_info
 
         self._model = None
         if self._params:
             model_name = self._get_model_name()
-            model_params = {}
+            model_params: Dict[str, Any] = {}
             for param_name, param_info in self._params.items():
-                default_value = param_info.default
-                if default_value is Parameter.empty:
-                    default_value = ...
-                model_params[param_name] = (param_info.annotation, default_value)
-            self._model = create_model(model_name, **model_params)  # type: ignore
+                model_params[param_name] = (param_info.annotation, param_info.default)
+            self._model = create_model(model_name,
+                                       __config__=get_config(dict(extra=extra)),
+                                       **model_params)
 
     def _get_model_name(self) -> str:
         return f"model_{self._callback.__name__}_{self._input_device}"
 
-    def __call__(self, input_device: InputDevice, message_bundle: MessageBundle) -> Optional[PipelineResult]:
+    def __call__(self,
+                 input_device: InputDevice,
+                 message_bundle: MessageBundle) -> Optional[Union[PipelineResult, List[PipelineResult]]]:
         kwargs: Dict[str, Any] = {}
         for param_name, param_info in self._special_params.items():
             if param_info.annotation is InputDeviceName:
                 kwargs[param_name] = input_device.name
             elif param_info.annotation is MessageBundle:
                 kwargs[param_name] = message_bundle
             elif param_info.annotation is Message:
                 kwargs[param_name] = message_bundle.message
 
         if self._model:
             model = parse_raw_as(self._model, message_bundle.message.bytes)
             kwargs.update(dict(model))
 
-        return_value = self._callback(**kwargs)
-        if return_value is None:
+        callback_return = self._callback(**kwargs)
+        if callback_return is None:
             return None
 
         if self._output_device is None:
             _logger.warning(f"callback for input device '{input_device.name}' returned value, "
                             f"but is not mapped to output device")
             return None
-
-        json_encoder = getattr(return_value, '__json_encoder__', BaseModel.__json_encoder__)
-
-        if isinstance(return_value, MessageBundle):
-            output_bundle = return_value
-        elif isinstance(return_value, Message):
-            output_bundle = MessageBundle(message=return_value)
+        results = []
+        if isinstance(callback_return, MultipleReturnValues):
+            return_list: List[Any] = callback_return
         else:
-            output_data = json.dumps(return_value, default=json_encoder).encode()
+            return_list = [callback_return]
+        for return_value in return_list:
+            results.append(self._get_single_pipeline_result(return_value, self._output_device))
+
+        return results
+
+    def _get_single_pipeline_result(self, value: Any, output_device: str):
+        if isinstance(value, MessageBundle):
+            output_bundle = value
+        elif isinstance(value, Message):
+            output_bundle = MessageBundle(message=value)
+        else:
+            json_encoder = getattr(value, '__json_encoder__', BaseModel.__json_encoder__)
+            output_data = json.dumps(value, default=json_encoder).encode()
             output_bundle = MessageBundle(message=Message(data=output_data))
 
-        return PipelineResult(output_device_name=self._output_device,
-                              message_bundle=output_bundle)
+        return PipelineResult(output_device_name=output_device, message_bundle=output_bundle)
 
 
 class FastMessage(PipelineHandlerBase):
     def __init__(self, default_output_device: Optional[str] = None,
-                 validation_error_handler: Optional[
-                     Callable[[InputDevice, MessageBundle, ValidationError], Optional[PipelineResult]]] = None):
+                 validation_error_handler: Optional[Callable[
+                     [InputDevice, MessageBundle, ValidationError],
+                     Optional[PipelineResult]]] = None):
         """
 
         :param default_output_device: an optional default output device to send callaback results to,
         unless mapped otherwise
         :param validation_error_handler: an optional handler that will be called on validation errors,
         in order to give the user a chance to handle them gracefully
         """
@@ -158,23 +184,26 @@
         """
         returns all the input device names that has callbacks
         """
         return list(self._wrappers.keys())
 
     def register_validation_error_handler(self,
                                           handler: Callable[
-                                              [InputDevice, MessageBundle, ValidationError], Optional[PipelineResult]]):
+                                              [InputDevice, MessageBundle, ValidationError],
+                                              Optional[PipelineResult]]):
         """
         registers optional handler that will be called on validation errors,
         in order to give the user a chance to handle them gracefully
         :param handler: the handler to register
         """
         self._validation_error_handler = handler
 
-    def register_callback(self, callback: Callable, input_device: str,
+    def register_callback(self,
+                          callback: Callable,
+                          input_device: str,
                           output_device: Optional[str] = _DEFAULT):
         """
         registers a callback to a device
 
         :param callback: the callback to register
         :param input_device: the input device to register the callback to
         :param output_device:  optional output device to route the return value of the callback to.
@@ -195,25 +224,29 @@
             input_device: str,
             output_device: Optional[str] = _DEFAULT) -> Callable[[_CALLABLE_TYPE], _CALLABLE_TYPE]:
         """
         this is the decorator method
 
         :param input_device: the input device to register the decorated method on
         :param output_device: optional output device to route the return value of the callback to.
-        None means no output routing
         if callback returns None, no routing will be made even if 'output_device' is not None
+        None means no output routing
         """
 
         def _register_callback_decorator(callback: _CALLABLE_TYPE) -> _CALLABLE_TYPE:
-            self.register_callback(callback=callback, input_device=input_device, output_device=output_device)
+            self.register_callback(callback=callback,
+                                   input_device=input_device,
+                                   output_device=output_device)
             return callback
 
         return _register_callback_decorator
 
-    def handle_message(self, input_device: InputDevice, message_bundle: MessageBundle) -> Optional[PipelineResult]:
+    def handle_message(self,
+                       input_device: InputDevice,
+                       message_bundle: MessageBundle) -> Optional[Union[PipelineResult, List[PipelineResult]]]:
         callback_wrapper = self._wrappers.get(input_device.name)
         if callback_wrapper is None:
             raise MissingCallbackException(f"No callback registered for device '{input_device.name}'")
         try:
             return callback_wrapper(input_device=input_device, message_bundle=message_bundle)
         except ValidationError as ve:
             if self._validation_error_handler is None:
```

### Comparing `messageflux-0.2.5/messageflux/iodevices/base/__init__.py` & `messageflux-0.2.6/messageflux/iodevices/base/__init__.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.5/messageflux/iodevices/base/common.py` & `messageflux-0.2.6/messageflux/iodevices/base/common.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.5/messageflux/iodevices/base/input_devices.py` & `messageflux-0.2.6/messageflux/iodevices/base/input_devices.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.5/messageflux/iodevices/base/input_transaction.py` & `messageflux-0.2.6/messageflux/iodevices/base/input_transaction.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.5/messageflux/iodevices/base/output_devices.py` & `messageflux-0.2.6/messageflux/iodevices/base/output_devices.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.5/messageflux/iodevices/collection_device_wrapper/collection_input_device.py` & `messageflux-0.2.6/messageflux/iodevices/collection_device_wrapper/collection_input_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.5/messageflux/iodevices/collection_device_wrapper/collection_output_device.py` & `messageflux-0.2.6/messageflux/iodevices/collection_device_wrapper/collection_output_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.5/messageflux/iodevices/failover_output_device_wrapper/failover_output_device.py` & `messageflux-0.2.6/messageflux/iodevices/failover_output_device_wrapper/failover_output_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.5/messageflux/iodevices/file_system/__init__.py` & `messageflux-0.2.6/messageflux/iodevices/file_system/__init__.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.5/messageflux/iodevices/file_system/file_system_device_manager_base.py` & `messageflux-0.2.6/messageflux/iodevices/file_system/file_system_device_manager_base.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.5/messageflux/iodevices/file_system/file_system_input_device.py` & `messageflux-0.2.6/messageflux/iodevices/file_system/file_system_input_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.5/messageflux/iodevices/file_system/file_system_output_device.py` & `messageflux-0.2.6/messageflux/iodevices/file_system/file_system_output_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.5/messageflux/iodevices/file_system/file_system_serializer.py` & `messageflux-0.2.6/messageflux/iodevices/file_system/file_system_serializer.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.5/messageflux/iodevices/in_memory_device/in_memory_device_manager.py` & `messageflux-0.2.6/messageflux/iodevices/in_memory_device/in_memory_device_manager.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.5/messageflux/iodevices/message_store_device_wrapper/file_system_message_store.py` & `messageflux-0.2.6/messageflux/iodevices/message_store_device_wrapper/file_system_message_store.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.5/messageflux/iodevices/message_store_device_wrapper/message_store_base.py` & `messageflux-0.2.6/messageflux/iodevices/message_store_device_wrapper/message_store_base.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.5/messageflux/iodevices/message_store_device_wrapper/message_store_input_device.py` & `messageflux-0.2.6/messageflux/iodevices/message_store_device_wrapper/message_store_input_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.5/messageflux/iodevices/message_store_device_wrapper/message_store_output_device.py` & `messageflux-0.2.6/messageflux/iodevices/message_store_device_wrapper/message_store_output_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.5/messageflux/iodevices/message_store_device_wrapper/message_store_transformer_base.py` & `messageflux-0.2.6/messageflux/iodevices/message_store_device_wrapper/message_store_transformer_base.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.5/messageflux/iodevices/objectstorage/s3_message_store.py` & `messageflux-0.2.6/messageflux/iodevices/objectstorage/s3_message_store.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.5/messageflux/iodevices/objectstorage/s3api/s3bucket.py` & `messageflux-0.2.6/messageflux/iodevices/objectstorage/s3api/s3bucket.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.5/messageflux/iodevices/objectstorage/s3api/s3client.py` & `messageflux-0.2.6/messageflux/iodevices/objectstorage/s3api/s3client.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.5/messageflux/iodevices/rabbitmq/fs_poison_counter.py` & `messageflux-0.2.6/messageflux/iodevices/rabbitmq/fs_poison_counter.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.5/messageflux/iodevices/rabbitmq/rabbitmq_device_manager_base.py` & `messageflux-0.2.6/messageflux/iodevices/rabbitmq/rabbitmq_device_manager_base.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.5/messageflux/iodevices/rabbitmq/rabbitmq_input_device.py` & `messageflux-0.2.6/messageflux/iodevices/rabbitmq/rabbitmq_input_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.5/messageflux/iodevices/rabbitmq/rabbitmq_output_device.py` & `messageflux-0.2.6/messageflux/iodevices/rabbitmq/rabbitmq_output_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.5/messageflux/iodevices/rabbitmq/rabbitmq_poison_counting_input_device.py` & `messageflux-0.2.6/messageflux/iodevices/rabbitmq/rabbitmq_poison_counting_input_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.5/messageflux/iodevices/round_robin_device_wrapper/roundrobin_io_device_manager.py` & `messageflux-0.2.6/messageflux/iodevices/round_robin_device_wrapper/roundrobin_io_device_manager.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.5/messageflux/iodevices/short_circuit_device_wrapper/common.py` & `messageflux-0.2.6/messageflux/iodevices/short_circuit_device_wrapper/common.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.5/messageflux/iodevices/short_circuit_device_wrapper/short_circuit_input_device.py` & `messageflux-0.2.6/messageflux/iodevices/short_circuit_device_wrapper/short_circuit_input_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.5/messageflux/iodevices/short_circuit_device_wrapper/short_circuit_output_device.py` & `messageflux-0.2.6/messageflux/iodevices/short_circuit_device_wrapper/short_circuit_output_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.5/messageflux/iodevices/transformer_device_wrapper/transformer_input_device.py` & `messageflux-0.2.6/messageflux/iodevices/transformer_device_wrapper/transformer_input_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.5/messageflux/iodevices/transformer_device_wrapper/transformer_output_device.py` & `messageflux-0.2.6/messageflux/iodevices/transformer_device_wrapper/transformer_output_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.5/messageflux/iodevices/transformer_device_wrapper/zlib_transformer.py` & `messageflux-0.2.6/messageflux/iodevices/transformer_device_wrapper/zlib_transformer.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.5/messageflux/logging/bulk_rotating_device_handler.py` & `messageflux-0.2.6/messageflux/logging/bulk_rotating_device_handler.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.5/messageflux/logging/bulk_rotating_file_handler.py` & `messageflux-0.2.6/messageflux/logging/bulk_rotating_file_handler.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.5/messageflux/logging/bulk_rotating_handler_base.py` & `messageflux-0.2.6/messageflux/logging/bulk_rotating_handler_base.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.5/messageflux/message_handling_service.py` & `messageflux-0.2.6/messageflux/message_handling_service.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.5/messageflux/multiprocessing/multiprocessrunner.py` & `messageflux-0.2.6/messageflux/multiprocessing/multiprocessrunner.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.5/messageflux/multiprocessing/singleprocesshandler.py` & `messageflux-0.2.6/messageflux/multiprocessing/singleprocesshandler.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.5/messageflux/pipeline_service.py` & `messageflux-0.2.6/messageflux/pipeline_service.py`

 * *Files 15% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     """
     a pipeline handler base class. used to handle a single message that passes through the pipeline
     """
 
     @abstractmethod
     def handle_message(self,
                        input_device: InputDevice,
-                       message_bundle: MessageBundle) -> Optional[PipelineResult]:
+                       message_bundle: MessageBundle) -> Optional[Union[PipelineResult, List[PipelineResult]]]:
         """
         Handles a message from an input device. and returns a tuple of the output device name, message and headers to
         send to.
 
         :param input_device: The input device that sent the message.
         :param message_bundle: The message that was received.
 
@@ -81,17 +81,21 @@
                  **kwargs):
         super().__init__(**kwargs)
         self._output_device_manager = output_device_manager
         self._pipeline_handler = pipeline_handler
 
     def _handle_message_batch(self, batch: List[Tuple[InputDevice, ReadResult]]):
         for input_device, read_result in batch:
-            pipeline_result = self._pipeline_handler.handle_message(input_device, read_result)
-            if pipeline_result is not None:
-                if self._output_device_manager is None:
-                    _logger.warning("pipeline handler returned a result to output to device: "
-                                    f"'{pipeline_result.output_device_name}', but no output_device_manager was given")
-                    return
-
-                output_device = self._output_device_manager.get_output_device(pipeline_result.output_device_name)
-                output_device.send_message(message=pipeline_result.message_bundle.message,
-                                           device_headers=pipeline_result.message_bundle.device_headers)
+            pipeline_handler_result = self._pipeline_handler.handle_message(input_device, read_result)
+            if pipeline_handler_result is not None:
+                if not isinstance(pipeline_handler_result, List):
+                    pipeline_handler_result = [pipeline_handler_result]
+                for pipeline_result in pipeline_handler_result:
+                    if self._output_device_manager is None:
+                        _logger.warning("pipeline handler returned a result to output to device: "
+                                        f"'{pipeline_result.output_device_name}', "
+                                        f"but no output_device_manager was given")
+                        continue
+
+                    output_device = self._output_device_manager.get_output_device(pipeline_result.output_device_name)
+                    output_device.send_message(message=pipeline_result.message_bundle.message,
+                                               device_headers=pipeline_result.message_bundle.device_headers)
```

### Comparing `messageflux-0.2.5/messageflux/server_loop_service.py` & `messageflux-0.2.6/messageflux/server_loop_service.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.5/messageflux/service_addons/loop_health_addon.py` & `messageflux-0.2.6/messageflux/service_addons/loop_health_addon.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.5/messageflux/utils/__init__.py` & `messageflux-0.2.6/messageflux/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.5/messageflux/utils/context.py` & `messageflux-0.2.6/messageflux/utils/context.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.5/messageflux/utils/filesystem.py` & `messageflux-0.2.6/messageflux/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.5/messageflux.egg-info/PKG-INFO` & `messageflux-0.2.6/messageflux.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: messageflux
-Version: 0.2.5
+Version: 0.2.6
 Author-email: Aviv Salem <avivsalem@gmail.com>
 Maintainer-email: Aviv Salem <avivsalem@gmail.com>, Nir Schulman <narsssx@gmail.com>, Rafael Zilberman <Zilberman.rafi@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Avivsalem/MessageFlux/
 Project-URL: Documentation, https://messageflux.readthedocs.io/
 Platform: win32
 Platform: linux
```

### Comparing `messageflux-0.2.5/messageflux.egg-info/SOURCES.txt` & `messageflux-0.2.6/messageflux.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.5/pyproject.toml` & `messageflux-0.2.6/pyproject.toml`

 * *Files identical despite different names*

