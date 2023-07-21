# Comparing `tmp/wds-client-0.2.92.tar.gz` & `tmp/wds-client-0.2.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wds-client-0.2.92.tar", last modified: Thu Jun 29 17:08:52 2023, max compression
+gzip compressed data, was "wds-client-0.2.93.tar", last modified: Fri Jul 21 18:39:50 2023, max compression
```

## Comparing `wds-client-0.2.92.tar` & `wds-client-0.2.93.tar`

### file list

```diff
@@ -1,94 +1,110 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:08:52.525946 wds-client-0.2.92/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-29 17:08:52.525946 wds-client-0.2.92/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6638 2023-06-29 17:07:35.000000 wds-client-0.2.92/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-29 17:08:52.525946 wds-client-0.2.92/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-29 17:07:35.000000 wds-client-0.2.92/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:08:52.521947 wds-client-0.2.92/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-06-29 17:07:34.000000 wds-client-0.2.92/test/test_attribute_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-06-29 17:07:34.000000 wds-client-0.2.92/test/test_backup_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-29 17:07:34.000000 wds-client-0.2.92/test/test_batch_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-06-29 17:07:34.000000 wds-client-0.2.92/test/test_batch_record_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-29 17:07:34.000000 wds-client-0.2.92/test/test_batch_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-29 17:07:34.000000 wds-client-0.2.92/test/test_build.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-29 17:07:34.000000 wds-client-0.2.92/test/test_cloning_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-29 17:07:34.000000 wds-client-0.2.92/test/test_commit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-06-29 17:07:34.000000 wds-client-0.2.92/test/test_component.py
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-06-29 17:07:34.000000 wds-client-0.2.92/test/test_components.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-29 17:07:34.000000 wds-client-0.2.92/test/test_db_component.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-29 17:07:34.000000 wds-client-0.2.92/test/test_db_validationcomponent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-29 17:07:34.000000 wds-client-0.2.92/test/test_db_validationcomponent_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-29 17:07:34.000000 wds-client-0.2.92/test/test_disk_space_component.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-06-29 17:07:34.000000 wds-client-0.2.92/test/test_disk_space_component_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-29 17:07:34.000000 wds-client-0.2.92/test/test_error_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-29 17:07:34.000000 wds-client-0.2.92/test/test_general_wds_information_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-29 17:07:34.000000 wds-client-0.2.92/test/test_git.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-29 17:07:34.000000 wds-client-0.2.92/test/test_inline_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-29 17:07:34.000000 wds-client-0.2.92/test/test_instances_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-06-29 17:07:34.000000 wds-client-0.2.92/test/test_record_attribute_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-06-29 17:07:34.000000 wds-client-0.2.92/test/test_record_query_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-06-29 17:07:34.000000 wds-client-0.2.92/test/test_record_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-06-29 17:07:34.000000 wds-client-0.2.92/test/test_record_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-06-29 17:07:34.000000 wds-client-0.2.92/test/test_record_type_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-29 17:07:34.000000 wds-client-0.2.92/test/test_records_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-29 17:07:34.000000 wds-client-0.2.92/test/test_request_body_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-29 17:07:35.000000 wds-client-0.2.92/test/test_schema_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-06-29 17:07:34.000000 wds-client-0.2.92/test/test_search_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-29 17:07:34.000000 wds-client-0.2.92/test/test_search_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-29 17:07:34.000000 wds-client-0.2.92/test/test_search_sort_direction.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-29 17:07:35.000000 wds-client-0.2.92/test/test_snapshots_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-06-29 17:07:34.000000 wds-client-0.2.92/test/test_stack_trace_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-06-29 17:07:34.000000 wds-client-0.2.92/test/test_status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-06-29 17:07:34.000000 wds-client-0.2.92/test/test_tsv_upload_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-29 17:07:34.000000 wds-client-0.2.92/test/test_version_response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:08:52.521947 wds-client-0.2.92/wds_client/
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-06-29 17:07:35.000000 wds-client-0.2.92/wds_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:08:52.521947 wds-client-0.2.92/wds_client/api/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-29 17:07:35.000000 wds-client-0.2.92/wds_client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-06-29 17:07:34.000000 wds-client-0.2.92/wds_client/api/cloning_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9761 2023-06-29 17:07:34.000000 wds-client-0.2.92/wds_client/api/general_wds_information_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    17329 2023-06-29 17:07:34.000000 wds-client-0.2.92/wds_client/api/instances_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    61562 2023-06-29 17:07:34.000000 wds-client-0.2.92/wds_client/api/records_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19354 2023-06-29 17:07:35.000000 wds-client-0.2.92/wds_client/api/schema_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6994 2023-06-29 17:07:35.000000 wds-client-0.2.92/wds_client/api/snapshots_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26217 2023-06-29 17:07:35.000000 wds-client-0.2.92/wds_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12795 2023-06-29 17:07:35.000000 wds-client-0.2.92/wds_client/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-06-29 17:07:35.000000 wds-client-0.2.92/wds_client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:08:52.525946 wds-client-0.2.92/wds_client/models/
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-06-29 17:07:35.000000 wds-client-0.2.92/wds_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-06-29 17:07:34.000000 wds-client-0.2.92/wds_client/models/attribute_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-06-29 17:07:34.000000 wds-client-0.2.92/wds_client/models/backup_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-06-29 17:07:34.000000 wds-client-0.2.92/wds_client/models/batch_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-06-29 17:07:34.000000 wds-client-0.2.92/wds_client/models/batch_record_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-06-29 17:07:34.000000 wds-client-0.2.92/wds_client/models/batch_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-06-29 17:07:34.000000 wds-client-0.2.92/wds_client/models/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-06-29 17:07:34.000000 wds-client-0.2.92/wds_client/models/commit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-06-29 17:07:34.000000 wds-client-0.2.92/wds_client/models/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-06-29 17:07:34.000000 wds-client-0.2.92/wds_client/models/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-06-29 17:07:34.000000 wds-client-0.2.92/wds_client/models/db_component.py
--rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-06-29 17:07:34.000000 wds-client-0.2.92/wds_client/models/db_validationcomponent.py
--rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-06-29 17:07:34.000000 wds-client-0.2.92/wds_client/models/db_validationcomponent_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-06-29 17:07:34.000000 wds-client-0.2.92/wds_client/models/disk_space_component.py
--rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-06-29 17:07:34.000000 wds-client-0.2.92/wds_client/models/disk_space_component_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-06-29 17:07:34.000000 wds-client-0.2.92/wds_client/models/error_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-06-29 17:07:34.000000 wds-client-0.2.92/wds_client/models/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-06-29 17:07:34.000000 wds-client-0.2.92/wds_client/models/inline_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-06-29 17:07:34.000000 wds-client-0.2.92/wds_client/models/record_attribute_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-06-29 17:07:34.000000 wds-client-0.2.92/wds_client/models/record_query_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-06-29 17:07:34.000000 wds-client-0.2.92/wds_client/models/record_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-06-29 17:07:34.000000 wds-client-0.2.92/wds_client/models/record_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-06-29 17:07:34.000000 wds-client-0.2.92/wds_client/models/record_type_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-06-29 17:07:34.000000 wds-client-0.2.92/wds_client/models/request_body_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-06-29 17:07:34.000000 wds-client-0.2.92/wds_client/models/search_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6218 2023-06-29 17:07:34.000000 wds-client-0.2.92/wds_client/models/search_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-06-29 17:07:34.000000 wds-client-0.2.92/wds_client/models/search_sort_direction.py
--rw-r--r--   0 runner    (1001) docker     (123)     6496 2023-06-29 17:07:34.000000 wds-client-0.2.92/wds_client/models/stack_trace_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-06-29 17:07:34.000000 wds-client-0.2.92/wds_client/models/status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-06-29 17:07:34.000000 wds-client-0.2.92/wds_client/models/tsv_upload_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-06-29 17:07:34.000000 wds-client-0.2.92/wds_client/models/version_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12309 2023-06-29 17:07:35.000000 wds-client-0.2.92/wds_client/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:08:52.521947 wds-client-0.2.92/wds_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-29 17:08:52.000000 wds-client-0.2.92/wds_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-06-29 17:08:52.000000 wds-client-0.2.92/wds_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 17:08:52.000000 wds-client-0.2.92/wds_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-29 17:08:52.000000 wds-client-0.2.92/wds_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 17:08:52.000000 wds-client-0.2.92/wds_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:39:50.023508 wds-client-0.2.93/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-21 18:39:50.023508 wds-client-0.2.93/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7609 2023-07-21 18:37:28.000000 wds-client-0.2.93/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-21 18:39:50.027508 wds-client-0.2.93/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-21 18:37:28.000000 wds-client-0.2.93/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:39:50.011508 wds-client-0.2.93/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-21 18:37:27.000000 wds-client-0.2.93/test/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-21 18:37:27.000000 wds-client-0.2.93/test/test_attribute_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-21 18:37:27.000000 wds-client-0.2.93/test/test_backup_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-21 18:37:27.000000 wds-client-0.2.93/test/test_backup_job_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-21 18:37:27.000000 wds-client-0.2.93/test/test_backup_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-21 18:37:27.000000 wds-client-0.2.93/test/test_backup_restore_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-07-21 18:37:27.000000 wds-client-0.2.93/test/test_batch_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-07-21 18:37:27.000000 wds-client-0.2.93/test/test_batch_record_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-21 18:37:27.000000 wds-client-0.2.93/test/test_batch_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-21 18:37:27.000000 wds-client-0.2.93/test/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-07-21 18:37:27.000000 wds-client-0.2.93/test/test_clone_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-21 18:37:27.000000 wds-client-0.2.93/test/test_clone_job_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-21 18:37:27.000000 wds-client-0.2.93/test/test_clone_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-21 18:37:28.000000 wds-client-0.2.93/test/test_cloning_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-21 18:37:27.000000 wds-client-0.2.93/test/test_commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-07-21 18:37:27.000000 wds-client-0.2.93/test/test_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-07-21 18:37:27.000000 wds-client-0.2.93/test/test_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-21 18:37:27.000000 wds-client-0.2.93/test/test_db_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-21 18:37:27.000000 wds-client-0.2.93/test/test_db_validationcomponent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-21 18:37:27.000000 wds-client-0.2.93/test/test_db_validationcomponent_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-21 18:37:27.000000 wds-client-0.2.93/test/test_disk_space_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-21 18:37:27.000000 wds-client-0.2.93/test/test_disk_space_component_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-21 18:37:28.000000 wds-client-0.2.93/test/test_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-21 18:37:28.000000 wds-client-0.2.93/test/test_general_wds_information_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-07-21 18:37:28.000000 wds-client-0.2.93/test/test_git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-07-21 18:37:28.000000 wds-client-0.2.93/test/test_inline_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-21 18:37:28.000000 wds-client-0.2.93/test/test_instances_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-21 18:37:28.000000 wds-client-0.2.93/test/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-21 18:37:28.000000 wds-client-0.2.93/test/test_record_attribute_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-07-21 18:37:28.000000 wds-client-0.2.93/test/test_record_query_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-07-21 18:37:28.000000 wds-client-0.2.93/test/test_record_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-07-21 18:37:28.000000 wds-client-0.2.93/test/test_record_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-21 18:37:28.000000 wds-client-0.2.93/test/test_record_type_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-07-21 18:37:28.000000 wds-client-0.2.93/test/test_records_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-21 18:37:28.000000 wds-client-0.2.93/test/test_request_body_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-21 18:37:28.000000 wds-client-0.2.93/test/test_schema_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-21 18:37:28.000000 wds-client-0.2.93/test/test_search_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-21 18:37:28.000000 wds-client-0.2.93/test/test_search_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-07-21 18:37:28.000000 wds-client-0.2.93/test/test_search_sort_direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-21 18:37:28.000000 wds-client-0.2.93/test/test_snapshots_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-07-21 18:37:28.000000 wds-client-0.2.93/test/test_stack_trace_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-07-21 18:37:28.000000 wds-client-0.2.93/test/test_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-21 18:37:28.000000 wds-client-0.2.93/test/test_tsv_upload_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-21 18:37:28.000000 wds-client-0.2.93/test/test_version_response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:39:50.015508 wds-client-0.2.93/wds_client/
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-07-21 18:37:28.000000 wds-client-0.2.93/wds_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:39:50.015508 wds-client-0.2.93/wds_client/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-21 18:37:28.000000 wds-client-0.2.93/wds_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17088 2023-07-21 18:37:28.000000 wds-client-0.2.93/wds_client/api/cloning_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9761 2023-07-21 18:37:28.000000 wds-client-0.2.93/wds_client/api/general_wds_information_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17329 2023-07-21 18:37:28.000000 wds-client-0.2.93/wds_client/api/instances_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61562 2023-07-21 18:37:28.000000 wds-client-0.2.93/wds_client/api/records_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19354 2023-07-21 18:37:28.000000 wds-client-0.2.93/wds_client/api/schema_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6994 2023-07-21 18:37:28.000000 wds-client-0.2.93/wds_client/api/snapshots_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26217 2023-07-21 18:37:28.000000 wds-client-0.2.93/wds_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12795 2023-07-21 18:37:28.000000 wds-client-0.2.93/wds_client/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-07-21 18:37:28.000000 wds-client-0.2.93/wds_client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:39:50.023508 wds-client-0.2.93/wds_client/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-07-21 18:37:28.000000 wds-client-0.2.93/wds_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-07-21 18:37:27.000000 wds-client-0.2.93/wds_client/models/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-07-21 18:37:27.000000 wds-client-0.2.93/wds_client/models/attribute_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8187 2023-07-21 18:37:27.000000 wds-client-0.2.93/wds_client/models/backup_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-07-21 18:37:27.000000 wds-client-0.2.93/wds_client/models/backup_job_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-07-21 18:37:27.000000 wds-client-0.2.93/wds_client/models/backup_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-07-21 18:37:27.000000 wds-client-0.2.93/wds_client/models/backup_restore_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-07-21 18:37:27.000000 wds-client-0.2.93/wds_client/models/batch_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-07-21 18:37:27.000000 wds-client-0.2.93/wds_client/models/batch_record_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-07-21 18:37:27.000000 wds-client-0.2.93/wds_client/models/batch_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-07-21 18:37:27.000000 wds-client-0.2.93/wds_client/models/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8152 2023-07-21 18:37:27.000000 wds-client-0.2.93/wds_client/models/clone_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-07-21 18:37:27.000000 wds-client-0.2.93/wds_client/models/clone_job_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-07-21 18:37:27.000000 wds-client-0.2.93/wds_client/models/clone_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-07-21 18:37:27.000000 wds-client-0.2.93/wds_client/models/commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-07-21 18:37:27.000000 wds-client-0.2.93/wds_client/models/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-07-21 18:37:27.000000 wds-client-0.2.93/wds_client/models/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-07-21 18:37:27.000000 wds-client-0.2.93/wds_client/models/db_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-07-21 18:37:27.000000 wds-client-0.2.93/wds_client/models/db_validationcomponent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-07-21 18:37:27.000000 wds-client-0.2.93/wds_client/models/db_validationcomponent_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-07-21 18:37:27.000000 wds-client-0.2.93/wds_client/models/disk_space_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-07-21 18:37:27.000000 wds-client-0.2.93/wds_client/models/disk_space_component_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-07-21 18:37:28.000000 wds-client-0.2.93/wds_client/models/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-07-21 18:37:28.000000 wds-client-0.2.93/wds_client/models/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-07-21 18:37:28.000000 wds-client-0.2.93/wds_client/models/inline_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7381 2023-07-21 18:37:28.000000 wds-client-0.2.93/wds_client/models/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-07-21 18:37:28.000000 wds-client-0.2.93/wds_client/models/record_attribute_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-07-21 18:37:28.000000 wds-client-0.2.93/wds_client/models/record_query_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-07-21 18:37:28.000000 wds-client-0.2.93/wds_client/models/record_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-07-21 18:37:28.000000 wds-client-0.2.93/wds_client/models/record_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-07-21 18:37:28.000000 wds-client-0.2.93/wds_client/models/record_type_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-07-21 18:37:28.000000 wds-client-0.2.93/wds_client/models/request_body_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-21 18:37:28.000000 wds-client-0.2.93/wds_client/models/search_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6218 2023-07-21 18:37:28.000000 wds-client-0.2.93/wds_client/models/search_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-07-21 18:37:28.000000 wds-client-0.2.93/wds_client/models/search_sort_direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6496 2023-07-21 18:37:28.000000 wds-client-0.2.93/wds_client/models/stack_trace_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-07-21 18:37:28.000000 wds-client-0.2.93/wds_client/models/status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-07-21 18:37:28.000000 wds-client-0.2.93/wds_client/models/tsv_upload_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-07-21 18:37:28.000000 wds-client-0.2.93/wds_client/models/version_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12309 2023-07-21 18:37:28.000000 wds-client-0.2.93/wds_client/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:39:50.015508 wds-client-0.2.93/wds_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-21 18:39:49.000000 wds-client-0.2.93/wds_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-07-21 18:39:49.000000 wds-client-0.2.93/wds_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 18:39:49.000000 wds-client-0.2.93/wds_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-21 18:39:49.000000 wds-client-0.2.93/wds_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-21 18:39:49.000000 wds-client-0.2.93/wds_client.egg-info/top_level.txt
```

### Comparing `wds-client-0.2.92/README.md` & `wds-client-0.2.93/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 This page lists current APIs.
 As of v0.2, all APIs are subject to change without notice.
 
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: v0.2
-- Package version: 0.2.92
+- Package version: 0.2.93
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation & Usage
@@ -56,38 +56,50 @@
 
 # Defining the host is optional and defaults to http://..
 # See configuration.py for a list of all supported configuration parameters.
 configuration = wds_client.Configuration(
     host = "http://.."
 )
 
+# The client must configure the authentication and authorization parameters
+# in accordance with the API server security policy.
+# Examples for each auth method are provided below, use the example that
+# satisfies your auth use case.
+
+# Configure Bearer authorization: bearerAuth
+configuration = wds_client.Configuration(
+    access_token = 'YOUR_BEARER_TOKEN'
+)
 
 
 # Enter a context with an instance of the API client
 with wds_client.ApiClient(configuration) as api_client:
     # Create an instance of the API class
     api_instance = wds_client.CloningApi(api_client)
     v = 'v0.2' # str | API version (default to 'v0.2')
+backup_restore_request = wds_client.BackupRestoreRequest() # BackupRestoreRequest | A backup request
 
     try:
-        # Create a backup of a PostgreSQL instance and upload it to Azure Blob Storage
-        api_response = api_instance.create_backup(v)
+        # Create a backup of all WDS data
+        api_response = api_instance.create_backup(v, backup_restore_request)
         pprint(api_response)
     except ApiException as e:
         print("Exception when calling CloningApi->create_backup: %s\n" % e)
     
 ```
 
 ## Documentation for API Endpoints
 
 All URIs are relative to *http://..*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
-*CloningApi* | [**create_backup**](docs/CloningApi.md#create_backup) | **POST** /backup/{v} | Create a backup of a PostgreSQL instance and upload it to Azure Blob Storage
+*CloningApi* | [**create_backup**](docs/CloningApi.md#create_backup) | **POST** /backup/{v} | Create a backup of all WDS data
+*CloningApi* | [**get_backup_status**](docs/CloningApi.md#get_backup_status) | **GET** /backup/{v}/{trackingId} | Check status of a WDS data backup
+*CloningApi* | [**get_clone_status**](docs/CloningApi.md#get_clone_status) | **GET** /clone/{v} | Check status of a WDS data clone
 *GeneralWDSInformationApi* | [**status_get**](docs/GeneralWDSInformationApi.md#status_get) | **GET** /status | Gets health status for WDS -- generated via Spring Boot Actuator (see https://docs.spring.io/spring-boot/docs/current/actuator-api/htmlsingle/#health for details)
 *GeneralWDSInformationApi* | [**version_get**](docs/GeneralWDSInformationApi.md#version_get) | **GET** /version | Gets related git and build version info for WDS -- generated via Spring Boot Actuator (see https://docs.spring.io/spring-boot/docs/current/actuator-api/htmlsingle/#info for details)
 *InstancesApi* | [**create_wds_instance**](docs/InstancesApi.md#create_wds_instance) | **POST** /instances/{v}/{instanceid} | Create an instance
 *InstancesApi* | [**delete_wds_instance**](docs/InstancesApi.md#delete_wds_instance) | **DELETE** /instances/{v}/{instanceid} | Delete an instance
 *InstancesApi* | [**list_wds_instances**](docs/InstancesApi.md#list_wds_instances) | **GET** /instances/{v} | List instances
 *RecordsApi* | [**batch_write_records**](docs/RecordsApi.md#batch_write_records) | **POST** /{instanceid}/batch/{v}/{type} | Batch write records
 *RecordsApi* | [**create_or_replace_record**](docs/RecordsApi.md#create_or_replace_record) | **PUT** /{instanceid}/records/{v}/{type}/{id} | Create or replace record
@@ -101,31 +113,39 @@
 *SchemaApi* | [**describe_all_record_types**](docs/SchemaApi.md#describe_all_record_types) | **GET** /{instanceid}/types/{v} | Describe all record types
 *SchemaApi* | [**describe_record_type**](docs/SchemaApi.md#describe_record_type) | **GET** /{instanceid}/types/{v}/{type} | Describe record type
 *SnapshotsApi* | [**import_snapshot**](docs/SnapshotsApi.md#import_snapshot) | **POST** /{instanceid}/snapshots/{v}/{snapshotid} | Import a snapshot from Terra Data Repo
 
 
 ## Documentation For Models
 
+ - [App](docs/App.md)
  - [AttributeSchema](docs/AttributeSchema.md)
+ - [BackupJob](docs/BackupJob.md)
+ - [BackupJobAllOf](docs/BackupJobAllOf.md)
  - [BackupResponse](docs/BackupResponse.md)
+ - [BackupRestoreRequest](docs/BackupRestoreRequest.md)
  - [BatchOperation](docs/BatchOperation.md)
  - [BatchRecordRequest](docs/BatchRecordRequest.md)
  - [BatchResponse](docs/BatchResponse.md)
  - [Build](docs/Build.md)
+ - [CloneJob](docs/CloneJob.md)
+ - [CloneJobAllOf](docs/CloneJobAllOf.md)
+ - [CloneResponse](docs/CloneResponse.md)
  - [Commit](docs/Commit.md)
  - [Component](docs/Component.md)
  - [Components](docs/Components.md)
  - [DbComponent](docs/DbComponent.md)
  - [DbValidationcomponent](docs/DbValidationcomponent.md)
  - [DbValidationcomponentDetails](docs/DbValidationcomponentDetails.md)
  - [DiskSpaceComponent](docs/DiskSpaceComponent.md)
  - [DiskSpaceComponentDetails](docs/DiskSpaceComponentDetails.md)
  - [ErrorResponse](docs/ErrorResponse.md)
  - [Git](docs/Git.md)
  - [InlineObject](docs/InlineObject.md)
+ - [Job](docs/Job.md)
  - [RecordAttributeDefinition](docs/RecordAttributeDefinition.md)
  - [RecordQueryResponse](docs/RecordQueryResponse.md)
  - [RecordRequest](docs/RecordRequest.md)
  - [RecordResponse](docs/RecordResponse.md)
  - [RecordTypeSchema](docs/RecordTypeSchema.md)
  - [RequestBodySearch](docs/RequestBodySearch.md)
  - [SearchOperator](docs/SearchOperator.md)
```

### Comparing `wds-client-0.2.92/setup.py` & `wds-client-0.2.93/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "wds-client"
-VERSION = "0.2.92"
+VERSION = "0.2.93"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `wds-client-0.2.92/test/test_attribute_schema.py` & `wds-client-0.2.93/test/test_attribute_schema.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.92/test/test_backup_response.py` & `wds-client-0.2.93/test/test_backup_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,16 +32,17 @@
         """Test BackupResponse
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
         # model = wds_client.models.backup_response.BackupResponse()  # noqa: E501
         if include_optional :
             return BackupResponse(
-                backup_status = True, 
-                message = '0'
+                filename = '0', 
+                requester = '0', 
+                description = '0'
             )
         else :
             return BackupResponse(
         )
 
     def testBackupResponse(self):
         """Test BackupResponse"""
```

### Comparing `wds-client-0.2.92/test/test_batch_operation.py` & `wds-client-0.2.93/test/test_batch_operation.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.92/test/test_batch_record_request.py` & `wds-client-0.2.93/test/test_batch_record_request.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.92/test/test_batch_response.py` & `wds-client-0.2.93/test/test_batch_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.92/test/test_build.py` & `wds-client-0.2.93/test/test_build.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.92/test/test_cloning_api.py` & `wds-client-0.2.93/test/test_cloning_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -27,14 +27,28 @@
 
     def tearDown(self):
         pass
 
     def test_create_backup(self):
         """Test case for create_backup
 
-        Create a backup of a PostgreSQL instance and upload it to Azure Blob Storage  # noqa: E501
+        Create a backup of all WDS data  # noqa: E501
+        """
+        pass
+
+    def test_get_backup_status(self):
+        """Test case for get_backup_status
+
+        Check status of a WDS data backup  # noqa: E501
+        """
+        pass
+
+    def test_get_clone_status(self):
+        """Test case for get_clone_status
+
+        Check status of a WDS data clone  # noqa: E501
         """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `wds-client-0.2.92/test/test_commit.py` & `wds-client-0.2.93/test/test_commit.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.92/test/test_component.py` & `wds-client-0.2.93/test/test_component.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.92/test/test_components.py` & `wds-client-0.2.93/test/test_components.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,16 +41,16 @@
                     components = wds_client.models.component.component(
                         status = '0', 
                         details = '0', ), ), 
                 disk_space = wds_client.models.disk_space_component.diskSpaceComponent(
                     status = '0', 
                     details = wds_client.models.disk_space_component_details.diskSpaceComponentDetails(
                         total = '0', 
-                        free = null, 
-                        threshold = null, 
+                        free = 1.337, 
+                        threshold = 1.337, 
                         exists = True, ), ), 
                 ping = wds_client.models.component.component(
                     status = '0', 
                     details = '0', ), 
                 main_db = wds_client.models.db_validationcomponent.dbValidationcomponent(
                     status = '0', 
                     components = wds_client.models.db_validationcomponent_details.dbValidationcomponentDetails(
```

### Comparing `wds-client-0.2.92/test/test_db_component.py` & `wds-client-0.2.93/test/test_db_component.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.92/test/test_db_validationcomponent.py` & `wds-client-0.2.93/test/test_db_validationcomponent.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.92/test/test_db_validationcomponent_details.py` & `wds-client-0.2.93/test/test_db_validationcomponent_details.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.92/test/test_disk_space_component.py` & `wds-client-0.2.93/test/test_disk_space_component.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,16 +35,16 @@
             optional params are included """
         # model = wds_client.models.disk_space_component.DiskSpaceComponent()  # noqa: E501
         if include_optional :
             return DiskSpaceComponent(
                 status = '0', 
                 details = wds_client.models.disk_space_component_details.diskSpaceComponentDetails(
                     total = '0', 
-                    free = null, 
-                    threshold = null, 
+                    free = 1.337, 
+                    threshold = 1.337, 
                     exists = True, )
             )
         else :
             return DiskSpaceComponent(
         )
 
     def testDiskSpaceComponent(self):
```

### Comparing `wds-client-0.2.92/test/test_disk_space_component_details.py` & `wds-client-0.2.93/test/test_disk_space_component_details.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,16 +33,16 @@
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
         # model = wds_client.models.disk_space_component_details.DiskSpaceComponentDetails()  # noqa: E501
         if include_optional :
             return DiskSpaceComponentDetails(
                 total = '0', 
-                free = null, 
-                threshold = null, 
+                free = 1.337, 
+                threshold = 1.337, 
                 exists = True
             )
         else :
             return DiskSpaceComponentDetails(
         )
 
     def testDiskSpaceComponentDetails(self):
```

### Comparing `wds-client-0.2.92/test/test_error_response.py` & `wds-client-0.2.93/test/test_error_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.92/test/test_general_wds_information_api.py` & `wds-client-0.2.93/test/test_general_wds_information_api.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.92/test/test_git.py` & `wds-client-0.2.93/test/test_git.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.92/test/test_inline_object.py` & `wds-client-0.2.93/test/test_inline_object.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.92/test/test_instances_api.py` & `wds-client-0.2.93/test/test_instances_api.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.92/test/test_record_attribute_definition.py` & `wds-client-0.2.93/test/test_record_attribute_definition.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.92/test/test_record_query_response.py` & `wds-client-0.2.93/test/test_record_query_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.92/test/test_record_request.py` & `wds-client-0.2.93/test/test_record_request.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.92/test/test_record_response.py` & `wds-client-0.2.93/test/test_record_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.92/test/test_record_type_schema.py` & `wds-client-0.2.93/test/test_record_type_schema.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.92/test/test_records_api.py` & `wds-client-0.2.93/test/test_records_api.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.92/test/test_request_body_search.py` & `wds-client-0.2.93/test/test_request_body_search.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.92/test/test_schema_api.py` & `wds-client-0.2.93/test/test_schema_api.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.92/test/test_search_operator.py` & `wds-client-0.2.93/test/test_search_operator.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.92/test/test_search_request.py` & `wds-client-0.2.93/test/test_search_request.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.92/test/test_search_sort_direction.py` & `wds-client-0.2.93/test/test_search_sort_direction.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.92/test/test_snapshots_api.py` & `wds-client-0.2.93/test/test_snapshots_api.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.92/test/test_stack_trace_element.py` & `wds-client-0.2.93/test/test_stack_trace_element.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.92/test/test_status_response.py` & `wds-client-0.2.93/test/test_status_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,16 +40,16 @@
                 components = wds_client.models.components.components(
                     db = wds_client.models.db_component.dbComponent(
                         status = '0', ), 
                     disk_space = wds_client.models.disk_space_component.diskSpaceComponent(
                         status = '0', 
                         details = wds_client.models.disk_space_component_details.diskSpaceComponentDetails(
                             total = '0', 
-                            free = null, 
-                            threshold = null, 
+                            free = 1.337, 
+                            threshold = 1.337, 
                             exists = True, ), ), 
                     ping = wds_client.models.component.component(
                         status = '0', ), 
                     main_db = wds_client.models.db_validationcomponent.dbValidationcomponent(
                         status = '0', ), 
                     streaming_ds = wds_client.models.db_validationcomponent.dbValidationcomponent(
                         status = '0', ), )
```

### Comparing `wds-client-0.2.92/test/test_tsv_upload_response.py` & `wds-client-0.2.93/test/test_tsv_upload_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.92/test/test_version_response.py` & `wds-client-0.2.93/test/test_version_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,17 @@
         """Test VersionResponse
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
         # model = wds_client.models.version_response.VersionResponse()  # noqa: E501
         if include_optional :
             return VersionResponse(
+                app = wds_client.models.app.app(
+                    chart_version = '0', 
+                    image = '0', ), 
                 git = wds_client.models.git.git(
                     branch = '0', 
                     commit = wds_client.models.commit.commit(
                         id = '0', 
                         time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), ), ), 
                 build = wds_client.models.build.build(
                     artifact = '0',
```

### Comparing `wds-client-0.2.92/wds_client/__init__.py` & `wds-client-0.2.93/wds_client/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "0.2.92"
+__version__ = "0.2.93"
 
 # import apis into sdk package
 from wds_client.api.cloning_api import CloningApi
 from wds_client.api.general_wds_information_api import GeneralWDSInformationApi
 from wds_client.api.instances_api import InstancesApi
 from wds_client.api.records_api import RecordsApi
 from wds_client.api.schema_api import SchemaApi
@@ -29,31 +29,39 @@
 from wds_client.configuration import Configuration
 from wds_client.exceptions import OpenApiException
 from wds_client.exceptions import ApiTypeError
 from wds_client.exceptions import ApiValueError
 from wds_client.exceptions import ApiKeyError
 from wds_client.exceptions import ApiException
 # import models into sdk package
+from wds_client.models.app import App
 from wds_client.models.attribute_schema import AttributeSchema
+from wds_client.models.backup_job import BackupJob
+from wds_client.models.backup_job_all_of import BackupJobAllOf
 from wds_client.models.backup_response import BackupResponse
+from wds_client.models.backup_restore_request import BackupRestoreRequest
 from wds_client.models.batch_operation import BatchOperation
 from wds_client.models.batch_record_request import BatchRecordRequest
 from wds_client.models.batch_response import BatchResponse
 from wds_client.models.build import Build
+from wds_client.models.clone_job import CloneJob
+from wds_client.models.clone_job_all_of import CloneJobAllOf
+from wds_client.models.clone_response import CloneResponse
 from wds_client.models.commit import Commit
 from wds_client.models.component import Component
 from wds_client.models.components import Components
 from wds_client.models.db_component import DbComponent
 from wds_client.models.db_validationcomponent import DbValidationcomponent
 from wds_client.models.db_validationcomponent_details import DbValidationcomponentDetails
 from wds_client.models.disk_space_component import DiskSpaceComponent
 from wds_client.models.disk_space_component_details import DiskSpaceComponentDetails
 from wds_client.models.error_response import ErrorResponse
 from wds_client.models.git import Git
 from wds_client.models.inline_object import InlineObject
+from wds_client.models.job import Job
 from wds_client.models.record_attribute_definition import RecordAttributeDefinition
 from wds_client.models.record_query_response import RecordQueryResponse
 from wds_client.models.record_request import RecordRequest
 from wds_client.models.record_response import RecordResponse
 from wds_client.models.record_type_schema import RecordTypeSchema
 from wds_client.models.request_body_search import RequestBodySearch
 from wds_client.models.search_operator import SearchOperator
```

### Comparing `wds-client-0.2.92/wds_client/api/general_wds_information_api.py` & `wds-client-0.2.93/wds_client/api/general_wds_information_api.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.92/wds_client/api/instances_api.py` & `wds-client-0.2.93/wds_client/api/instances_api.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.92/wds_client/api/records_api.py` & `wds-client-0.2.93/wds_client/api/records_api.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.92/wds_client/api/schema_api.py` & `wds-client-0.2.93/wds_client/api/schema_api.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.92/wds_client/api/snapshots_api.py` & `wds-client-0.2.93/wds_client/api/snapshots_api.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.92/wds_client/api_client.py` & `wds-client-0.2.93/wds_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.2.92/python'
+        self.user_agent = 'OpenAPI-Generator/0.2.93/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `wds-client-0.2.92/wds_client/configuration.py` & `wds-client-0.2.93/wds_client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -332,15 +332,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: v0.2\n"\
-               "SDK Package Version: 0.2.92".\
+               "SDK Package Version: 0.2.93".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `wds-client-0.2.92/wds_client/exceptions.py` & `wds-client-0.2.93/wds_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.92/wds_client/models/attribute_schema.py` & `wds-client-0.2.93/wds_client/models/attribute_schema.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.92/wds_client/models/backup_response.py` & `wds-client-0.2.93/wds_client/models/disk_space_component.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,98 +14,94 @@
 import re  # noqa: F401
 
 import six
 
 from wds_client.configuration import Configuration
 
 
-class BackupResponse(object):
+class DiskSpaceComponent(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'backup_status': 'bool',
-        'message': 'str'
+        'status': 'str',
+        'details': 'DiskSpaceComponentDetails'
     }
 
     attribute_map = {
-        'backup_status': 'backupStatus',
-        'message': 'message'
+        'status': 'status',
+        'details': 'details'
     }
 
-    def __init__(self, backup_status=None, message=None, local_vars_configuration=None):  # noqa: E501
-        """BackupResponse - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, status=None, details=None, local_vars_configuration=None):  # noqa: E501
+        """DiskSpaceComponent - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._backup_status = None
-        self._message = None
+        self._status = None
+        self._details = None
         self.discriminator = None
 
-        if backup_status is not None:
-            self.backup_status = backup_status
-        if message is not None:
-            self.message = message
+        if status is not None:
+            self.status = status
+        if details is not None:
+            self.details = details
 
     @property
-    def backup_status(self):
-        """Gets the backup_status of this BackupResponse.  # noqa: E501
+    def status(self):
+        """Gets the status of this DiskSpaceComponent.  # noqa: E501
 
-        status of backup  # noqa: E501
 
-        :return: The backup_status of this BackupResponse.  # noqa: E501
-        :rtype: bool
+        :return: The status of this DiskSpaceComponent.  # noqa: E501
+        :rtype: str
         """
-        return self._backup_status
+        return self._status
 
-    @backup_status.setter
-    def backup_status(self, backup_status):
-        """Sets the backup_status of this BackupResponse.
+    @status.setter
+    def status(self, status):
+        """Sets the status of this DiskSpaceComponent.
 
-        status of backup  # noqa: E501
 
-        :param backup_status: The backup_status of this BackupResponse.  # noqa: E501
-        :type: bool
+        :param status: The status of this DiskSpaceComponent.  # noqa: E501
+        :type: str
         """
 
-        self._backup_status = backup_status
+        self._status = status
 
     @property
-    def message(self):
-        """Gets the message of this BackupResponse.  # noqa: E501
+    def details(self):
+        """Gets the details of this DiskSpaceComponent.  # noqa: E501
 
-        message regarding backup status  # noqa: E501
 
-        :return: The message of this BackupResponse.  # noqa: E501
-        :rtype: str
+        :return: The details of this DiskSpaceComponent.  # noqa: E501
+        :rtype: DiskSpaceComponentDetails
         """
-        return self._message
+        return self._details
 
-    @message.setter
-    def message(self, message):
-        """Sets the message of this BackupResponse.
+    @details.setter
+    def details(self, details):
+        """Sets the details of this DiskSpaceComponent.
 
-        message regarding backup status  # noqa: E501
 
-        :param message: The message of this BackupResponse.  # noqa: E501
-        :type: str
+        :param details: The details of this DiskSpaceComponent.  # noqa: E501
+        :type: DiskSpaceComponentDetails
         """
 
-        self._message = message
+        self._details = details
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -133,18 +129,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, BackupResponse):
+        if not isinstance(other, DiskSpaceComponent):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, BackupResponse):
+        if not isinstance(other, DiskSpaceComponent):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `wds-client-0.2.92/wds_client/models/batch_operation.py` & `wds-client-0.2.93/wds_client/models/batch_operation.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.92/wds_client/models/batch_record_request.py` & `wds-client-0.2.93/wds_client/models/batch_record_request.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.92/wds_client/models/batch_response.py` & `wds-client-0.2.93/wds_client/models/batch_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.92/wds_client/models/build.py` & `wds-client-0.2.93/wds_client/models/build.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.92/wds_client/models/commit.py` & `wds-client-0.2.93/wds_client/models/commit.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.92/wds_client/models/component.py` & `wds-client-0.2.93/wds_client/models/component.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.92/wds_client/models/components.py` & `wds-client-0.2.93/wds_client/models/components.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.92/wds_client/models/db_component.py` & `wds-client-0.2.93/wds_client/models/db_component.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.92/wds_client/models/db_validationcomponent.py` & `wds-client-0.2.93/wds_client/models/db_validationcomponent.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.92/wds_client/models/db_validationcomponent_details.py` & `wds-client-0.2.93/wds_client/models/db_validationcomponent_details.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.92/wds_client/models/disk_space_component.py` & `wds-client-0.2.93/wds_client/models/status_response.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import re  # noqa: F401
 
 import six
 
 from wds_client.configuration import Configuration
 
 
-class DiskSpaceComponent(object):
+class StatusResponse(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -30,78 +30,78 @@
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'status': 'str',
-        'details': 'DiskSpaceComponentDetails'
+        'components': 'Components'
     }
 
     attribute_map = {
         'status': 'status',
-        'details': 'details'
+        'components': 'components'
     }
 
-    def __init__(self, status=None, details=None, local_vars_configuration=None):  # noqa: E501
-        """DiskSpaceComponent - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, status=None, components=None, local_vars_configuration=None):  # noqa: E501
+        """StatusResponse - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._status = None
-        self._details = None
+        self._components = None
         self.discriminator = None
 
         if status is not None:
             self.status = status
-        if details is not None:
-            self.details = details
+        if components is not None:
+            self.components = components
 
     @property
     def status(self):
-        """Gets the status of this DiskSpaceComponent.  # noqa: E501
+        """Gets the status of this StatusResponse.  # noqa: E501
 
 
-        :return: The status of this DiskSpaceComponent.  # noqa: E501
+        :return: The status of this StatusResponse.  # noqa: E501
         :rtype: str
         """
         return self._status
 
     @status.setter
     def status(self, status):
-        """Sets the status of this DiskSpaceComponent.
+        """Sets the status of this StatusResponse.
 
 
-        :param status: The status of this DiskSpaceComponent.  # noqa: E501
+        :param status: The status of this StatusResponse.  # noqa: E501
         :type: str
         """
 
         self._status = status
 
     @property
-    def details(self):
-        """Gets the details of this DiskSpaceComponent.  # noqa: E501
+    def components(self):
+        """Gets the components of this StatusResponse.  # noqa: E501
 
 
-        :return: The details of this DiskSpaceComponent.  # noqa: E501
-        :rtype: DiskSpaceComponentDetails
+        :return: The components of this StatusResponse.  # noqa: E501
+        :rtype: Components
         """
-        return self._details
+        return self._components
 
-    @details.setter
-    def details(self, details):
-        """Sets the details of this DiskSpaceComponent.
+    @components.setter
+    def components(self, components):
+        """Sets the components of this StatusResponse.
 
 
-        :param details: The details of this DiskSpaceComponent.  # noqa: E501
-        :type: DiskSpaceComponentDetails
+        :param components: The components of this StatusResponse.  # noqa: E501
+        :type: Components
         """
 
-        self._details = details
+        self._components = components
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -129,18 +129,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, DiskSpaceComponent):
+        if not isinstance(other, StatusResponse):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, DiskSpaceComponent):
+        if not isinstance(other, StatusResponse):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `wds-client-0.2.92/wds_client/models/disk_space_component_details.py` & `wds-client-0.2.93/wds_client/models/disk_space_component_details.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.92/wds_client/models/error_response.py` & `wds-client-0.2.93/wds_client/models/error_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.92/wds_client/models/git.py` & `wds-client-0.2.93/wds_client/models/git.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.92/wds_client/models/inline_object.py` & `wds-client-0.2.93/wds_client/models/inline_object.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.92/wds_client/models/record_attribute_definition.py` & `wds-client-0.2.93/wds_client/models/record_attribute_definition.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.92/wds_client/models/record_query_response.py` & `wds-client-0.2.93/wds_client/models/record_query_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.92/wds_client/models/record_request.py` & `wds-client-0.2.93/wds_client/models/record_request.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.92/wds_client/models/record_response.py` & `wds-client-0.2.93/wds_client/models/record_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.92/wds_client/models/record_type_schema.py` & `wds-client-0.2.93/wds_client/models/record_type_schema.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.92/wds_client/models/request_body_search.py` & `wds-client-0.2.93/wds_client/models/request_body_search.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.92/wds_client/models/search_operator.py` & `wds-client-0.2.93/wds_client/models/search_operator.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.92/wds_client/models/search_request.py` & `wds-client-0.2.93/wds_client/models/search_request.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.92/wds_client/models/search_sort_direction.py` & `wds-client-0.2.93/wds_client/models/search_sort_direction.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.92/wds_client/models/stack_trace_element.py` & `wds-client-0.2.93/wds_client/models/stack_trace_element.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.92/wds_client/models/status_response.py` & `wds-client-0.2.93/wds_client/models/version_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,94 +14,120 @@
 import re  # noqa: F401
 
 import six
 
 from wds_client.configuration import Configuration
 
 
-class StatusResponse(object):
+class VersionResponse(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'status': 'str',
-        'components': 'Components'
+        'app': 'App',
+        'git': 'Git',
+        'build': 'Build'
     }
 
     attribute_map = {
-        'status': 'status',
-        'components': 'components'
+        'app': 'app',
+        'git': 'git',
+        'build': 'build'
     }
 
-    def __init__(self, status=None, components=None, local_vars_configuration=None):  # noqa: E501
-        """StatusResponse - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, app=None, git=None, build=None, local_vars_configuration=None):  # noqa: E501
+        """VersionResponse - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._status = None
-        self._components = None
+        self._app = None
+        self._git = None
+        self._build = None
         self.discriminator = None
 
-        if status is not None:
-            self.status = status
-        if components is not None:
-            self.components = components
+        if app is not None:
+            self.app = app
+        if git is not None:
+            self.git = git
+        if build is not None:
+            self.build = build
 
     @property
-    def status(self):
-        """Gets the status of this StatusResponse.  # noqa: E501
+    def app(self):
+        """Gets the app of this VersionResponse.  # noqa: E501
 
 
-        :return: The status of this StatusResponse.  # noqa: E501
-        :rtype: str
+        :return: The app of this VersionResponse.  # noqa: E501
+        :rtype: App
         """
-        return self._status
+        return self._app
 
-    @status.setter
-    def status(self, status):
-        """Sets the status of this StatusResponse.
+    @app.setter
+    def app(self, app):
+        """Sets the app of this VersionResponse.
 
 
-        :param status: The status of this StatusResponse.  # noqa: E501
-        :type: str
+        :param app: The app of this VersionResponse.  # noqa: E501
+        :type: App
         """
 
-        self._status = status
+        self._app = app
 
     @property
-    def components(self):
-        """Gets the components of this StatusResponse.  # noqa: E501
+    def git(self):
+        """Gets the git of this VersionResponse.  # noqa: E501
 
 
-        :return: The components of this StatusResponse.  # noqa: E501
-        :rtype: Components
+        :return: The git of this VersionResponse.  # noqa: E501
+        :rtype: Git
         """
-        return self._components
+        return self._git
 
-    @components.setter
-    def components(self, components):
-        """Sets the components of this StatusResponse.
+    @git.setter
+    def git(self, git):
+        """Sets the git of this VersionResponse.
 
 
-        :param components: The components of this StatusResponse.  # noqa: E501
-        :type: Components
+        :param git: The git of this VersionResponse.  # noqa: E501
+        :type: Git
         """
 
-        self._components = components
+        self._git = git
+
+    @property
+    def build(self):
+        """Gets the build of this VersionResponse.  # noqa: E501
+
+
+        :return: The build of this VersionResponse.  # noqa: E501
+        :rtype: Build
+        """
+        return self._build
+
+    @build.setter
+    def build(self, build):
+        """Sets the build of this VersionResponse.
+
+
+        :param build: The build of this VersionResponse.  # noqa: E501
+        :type: Build
+        """
+
+        self._build = build
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -129,18 +155,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, StatusResponse):
+        if not isinstance(other, VersionResponse):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, StatusResponse):
+        if not isinstance(other, VersionResponse):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `wds-client-0.2.92/wds_client/models/tsv_upload_response.py` & `wds-client-0.2.93/wds_client/models/tsv_upload_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.92/wds_client/models/version_response.py` & `wds-client-0.2.93/wds_client/models/clone_job_all_of.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,94 +14,68 @@
 import re  # noqa: F401
 
 import six
 
 from wds_client.configuration import Configuration
 
 
-class VersionResponse(object):
+class CloneJobAllOf(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'git': 'Git',
-        'build': 'Build'
+        'result': 'CloneResponse'
     }
 
     attribute_map = {
-        'git': 'git',
-        'build': 'build'
+        'result': 'result'
     }
 
-    def __init__(self, git=None, build=None, local_vars_configuration=None):  # noqa: E501
-        """VersionResponse - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, result=None, local_vars_configuration=None):  # noqa: E501
+        """CloneJobAllOf - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._git = None
-        self._build = None
+        self._result = None
         self.discriminator = None
 
-        if git is not None:
-            self.git = git
-        if build is not None:
-            self.build = build
+        if result is not None:
+            self.result = result
 
     @property
-    def git(self):
-        """Gets the git of this VersionResponse.  # noqa: E501
+    def result(self):
+        """Gets the result of this CloneJobAllOf.  # noqa: E501
 
 
-        :return: The git of this VersionResponse.  # noqa: E501
-        :rtype: Git
+        :return: The result of this CloneJobAllOf.  # noqa: E501
+        :rtype: CloneResponse
         """
-        return self._git
+        return self._result
 
-    @git.setter
-    def git(self, git):
-        """Sets the git of this VersionResponse.
+    @result.setter
+    def result(self, result):
+        """Sets the result of this CloneJobAllOf.
 
 
-        :param git: The git of this VersionResponse.  # noqa: E501
-        :type: Git
+        :param result: The result of this CloneJobAllOf.  # noqa: E501
+        :type: CloneResponse
         """
 
-        self._git = git
-
-    @property
-    def build(self):
-        """Gets the build of this VersionResponse.  # noqa: E501
-
-
-        :return: The build of this VersionResponse.  # noqa: E501
-        :rtype: Build
-        """
-        return self._build
-
-    @build.setter
-    def build(self, build):
-        """Sets the build of this VersionResponse.
-
-
-        :param build: The build of this VersionResponse.  # noqa: E501
-        :type: Build
-        """
-
-        self._build = build
+        self._result = result
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -129,18 +103,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, VersionResponse):
+        if not isinstance(other, CloneJobAllOf):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, VersionResponse):
+        if not isinstance(other, CloneJobAllOf):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `wds-client-0.2.92/wds_client/rest.py` & `wds-client-0.2.93/wds_client/rest.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.92/wds_client.egg-info/SOURCES.txt` & `wds-client-0.2.93/wds_client.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,38 @@
 README.md
 setup.cfg
 setup.py
+test/test_app.py
 test/test_attribute_schema.py
+test/test_backup_job.py
+test/test_backup_job_all_of.py
 test/test_backup_response.py
+test/test_backup_restore_request.py
 test/test_batch_operation.py
 test/test_batch_record_request.py
 test/test_batch_response.py
 test/test_build.py
+test/test_clone_job.py
+test/test_clone_job_all_of.py
+test/test_clone_response.py
 test/test_cloning_api.py
 test/test_commit.py
 test/test_component.py
 test/test_components.py
 test/test_db_component.py
 test/test_db_validationcomponent.py
 test/test_db_validationcomponent_details.py
 test/test_disk_space_component.py
 test/test_disk_space_component_details.py
 test/test_error_response.py
 test/test_general_wds_information_api.py
 test/test_git.py
 test/test_inline_object.py
 test/test_instances_api.py
+test/test_job.py
 test/test_record_attribute_definition.py
 test/test_record_query_response.py
 test/test_record_request.py
 test/test_record_response.py
 test/test_record_type_schema.py
 test/test_records_api.py
 test/test_request_body_search.py
@@ -51,31 +59,39 @@
 wds_client/api/cloning_api.py
 wds_client/api/general_wds_information_api.py
 wds_client/api/instances_api.py
 wds_client/api/records_api.py
 wds_client/api/schema_api.py
 wds_client/api/snapshots_api.py
 wds_client/models/__init__.py
+wds_client/models/app.py
 wds_client/models/attribute_schema.py
+wds_client/models/backup_job.py
+wds_client/models/backup_job_all_of.py
 wds_client/models/backup_response.py
+wds_client/models/backup_restore_request.py
 wds_client/models/batch_operation.py
 wds_client/models/batch_record_request.py
 wds_client/models/batch_response.py
 wds_client/models/build.py
+wds_client/models/clone_job.py
+wds_client/models/clone_job_all_of.py
+wds_client/models/clone_response.py
 wds_client/models/commit.py
 wds_client/models/component.py
 wds_client/models/components.py
 wds_client/models/db_component.py
 wds_client/models/db_validationcomponent.py
 wds_client/models/db_validationcomponent_details.py
 wds_client/models/disk_space_component.py
 wds_client/models/disk_space_component_details.py
 wds_client/models/error_response.py
 wds_client/models/git.py
 wds_client/models/inline_object.py
+wds_client/models/job.py
 wds_client/models/record_attribute_definition.py
 wds_client/models/record_query_response.py
 wds_client/models/record_request.py
 wds_client/models/record_response.py
 wds_client/models/record_type_schema.py
 wds_client/models/request_body_search.py
 wds_client/models/search_operator.py
```

