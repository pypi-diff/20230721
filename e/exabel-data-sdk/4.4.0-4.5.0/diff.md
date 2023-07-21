# Comparing `tmp/exabel-data-sdk-4.4.0.tar.gz` & `tmp/exabel-data-sdk-4.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/exabel-data-sdk-4.4.0.tar", last modified: Thu May 25 12:39:31 2023, max compression
+gzip compressed data, was "dist/exabel-data-sdk-4.5.0.tar", last modified: Fri Jul 21 09:24:36 2023, max compression
```

## Comparing `exabel-data-sdk-4.4.0.tar` & `exabel-data-sdk-4.5.0.tar`

### file list

```diff
@@ -1,411 +1,412 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:39:31.000000 exabel-data-sdk-4.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-05-25 12:39:31.000000 exabel-data-sdk-4.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:39:31.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:39:31.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:39:31.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:39:31.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/api_client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/api_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/api_client/data_set_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/api_client/derived_signal_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/api_client/entity_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/api_client/exabel_api_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:39:31.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/api_client/grpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/api_client/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/api_client/grpc/base_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/api_client/grpc/data_set_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/api_client/grpc/derived_signal_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/api_client/grpc/entity_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/api_client/grpc/library_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/api_client/grpc/namespace_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/api_client/grpc/prediction_model_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/api_client/grpc/relationship_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/api_client/grpc/signal_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/api_client/grpc/tag_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/api_client/grpc/time_series_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/api_client/grpc/user_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/api_client/library_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/api_client/namespace_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/api_client/prediction_model_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/api_client/relationship_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/api_client/signal_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/api_client/tag_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/api_client/time_series_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/api_client/user_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10905 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/bulk_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/bulk_insert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:39:31.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/data_classes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/data_classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/data_classes/data_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     7661 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/data_classes/derived_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/data_classes/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/data_classes/entity_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/data_classes/folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/data_classes/folder_accessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/data_classes/folder_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/data_classes/group.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/data_classes/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/data_classes/paging_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/data_classes/prediction_model_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/data_classes/relationship.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/data_classes/relationship_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/data_classes/request_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/data_classes/signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/data_classes/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/data_classes/time_series.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/data_classes/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/data_set_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/derived_signal_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11318 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/entity_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/error_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12035 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/export_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7417 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/library_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/namespace_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/pageable_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/prediction_model_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/proto_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16290 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/relationship_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8795 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/resource_creation_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/search_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/signal_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/tag_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25470 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/time_series_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/user_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/client_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/exabel_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13319 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/client/user_login.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:39:31.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/examples/create_time_series_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/examples/get_company_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:39:31.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/query/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/query/column.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/query/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/query/literal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/query/predicate.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/query/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/query/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/query/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:39:31.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/base_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/check_company_identifiers_in_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/command_line_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/create_derived_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/create_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     8448 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/create_entity_mapping_from_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/create_entity_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/create_folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/create_prediction_model_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/create_relationship.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/create_relationship_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/create_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/csv_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/csv_script_with_entity_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/delete_entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/delete_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/delete_entity_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/delete_folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/delete_relationship.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/delete_relationship_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/delete_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/export_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/get_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/get_entity_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/get_folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/get_relationship.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/get_relationship_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/get_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/get_time_series.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/list_entities.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/list_entity_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/list_folder_accessors.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/list_folders.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/list_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/list_items.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/list_relationship_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/list_relationships.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/list_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/list_time_series.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/list_users.py
--rw-r--r--   0 runner    (1001) docker     (123)     5984 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/load_entities_from_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     9550 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/load_relationships_from_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/load_time_series_from_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/load_time_series_from_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/move_items.py
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/search_entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/share_folder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:39:31.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/sql/read_athena.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/sql/read_bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/sql/read_snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/sql/sql_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/unshare_folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/update_entity_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/update_folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/update_relationship_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:39:31.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10835 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/services/csv_entity_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/services/csv_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/services/csv_loading_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/services/csv_loading_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/services/csv_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    22322 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/services/csv_relationship_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/services/csv_time_series_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/services/csv_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/services/entity_mapping_file_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/services/excel_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/services/file_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/services/file_loading_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/services/file_loading_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    18693 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/services/file_time_series_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    34306 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/services/file_time_series_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/services/file_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/services/file_writer_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:39:31.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/services/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/services/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/services/sql/athena_reader_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/services/sql/bigquery_reader_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/services/sql/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/services/sql/snowflake_reader_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/services/sql/sql_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/services/sql/sql_reader_configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:39:31.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:39:31.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:39:31.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/all_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/all_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:39:31.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/analytics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/analytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/analytics/all_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/analytics/all_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:39:31.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/all_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/all_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_messages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_messages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9751 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/item_messages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/item_messages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_messages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_messages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_messages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_messages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8946 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14383 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:39:31.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/data/all_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/data/all_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:39:31.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/data/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/data/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/data/v1/all_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/data/v1/all_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_messages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_messages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10371 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_messages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_messages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14438 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    21787 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/data/v1/import_job_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/data/v1/import_job_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespace_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespace_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespaces_messages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespaces_messages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_messages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_messages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14070 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    18779 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/data/v1/search_messages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/data/v1/search_messages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/data/v1/service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/data/v1/service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_messages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_messages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9149 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_messages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_messages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11807 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    16187 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:39:31.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/management/all_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/management/all_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:39:31.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/management/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/management/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/management/v1/all_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/management/v1/all_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/management/v1/folder_messages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/management/v1/folder_messages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    13228 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/management/v1/library_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    20539 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/management/v1/library_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/management/v1/service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/management/v1/service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_messages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_messages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:39:31.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/math/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/math/aggregation_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/math/aggregation_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/math/all_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/math/all_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:39:31.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/time/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/time/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/time/all_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/time/all_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/time/time_range_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/time/time_range_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:39:31.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:39:31.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/annotations_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/annotations_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14731 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/openapiv2_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/openapiv2_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:39:31.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:39:31.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:39:31.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:39:31.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/api_client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/api_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/api_client/test_exabel_api_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:39:31.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/data_classes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/data_classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/data_classes/test_data_set.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/data_classes/test_derived_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/data_classes/test_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/data_classes/test_entity_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/data_classes/test_folder.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/data_classes/test_folder_accessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/data_classes/test_folder_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/data_classes/test_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/data_classes/test_namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/data_classes/test_prediction_model_run.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/data_classes/test_relationship.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/data_classes/test_relationship_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/data_classes/test_request_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/data_classes/test_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/data_classes/test_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/data_classes/test_time_series.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/data_classes/test_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/mock_entity_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/mock_relationship_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/mock_resource_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/mock_signal_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7262 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/test_bulk_insert_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/test_entity_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/test_error_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/test_export_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/test_namespace_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/test_pageable_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/test_proto_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6528 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/test_relationship_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/test_resource_creation_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/test_signal_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8784 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/test_time_series_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/exabel_mock_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:39:31.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/query/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/query/test_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/test_client_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/test_exabel_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/test_user_login.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:39:31.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/scripts/common_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:39:31.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/scripts/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/scripts/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/scripts/sql/test_read_snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/scripts/sql/test_sql_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/scripts/test_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/scripts/test_command_line_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/scripts/test_create_entity_mapping_from_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/scripts/test_create_entity_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/scripts/test_create_relationship_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/scripts/test_delete_entity_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/scripts/test_export_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/scripts/test_load_entities_from_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     7969 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/scripts/test_load_relationships_from_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/scripts/test_load_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)    35797 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/scripts/test_load_time_series_from_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)    23337 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/scripts/test_load_time_series_from_excel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/scripts/test_update_entity_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/scripts/test_update_relationship_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:39:31.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:39:31.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/services/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/services/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/services/sql/test_athena_reader_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/services/sql/test_bigquery_reader_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/services/sql/test_snowflake_reader_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/services/sql/test_sql_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/services/sql/test_sql_reader_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/services/test_csv_entity_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/services/test_csv_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    27281 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/services/test_csv_relationship_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/services/test_csv_time_series_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/services/test_csv_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/services/test_entity_mapping_file_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/services/test_excel_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/services/test_file_loading_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    11826 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/services/test_file_time_series_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     8177 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/services/test_file_time_series_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/services/test_file_writer_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/test_decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:39:31.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/util/test_batcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/util/test_deprecate_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/util/test_handle_missing_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/util/test_parse_property_columns.py
--rw-r--r--   0 runner    (1001) docker     (123)    16285 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/util/test_resource_name_normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/tests/util/test_type_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:39:31.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/util/batcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/util/case_insensitive_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/util/deprecate_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/util/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/util/handle_missing_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/util/import_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/util/parse_property_columns.py
--rw-r--r--   0 runner    (1001) docker     (123)    16285 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/util/resource_name_normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/util/type_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/exabel_data_sdk/util/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:39:31.000000 exabel-data-sdk-4.4.0/exabel_data_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-05-25 12:39:31.000000 exabel-data-sdk-4.4.0/exabel_data_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19860 2023-05-25 12:39:31.000000 exabel-data-sdk-4.4.0/exabel_data_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 12:39:31.000000 exabel-data-sdk-4.4.0/exabel_data_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-25 12:39:31.000000 exabel-data-sdk-4.4.0/exabel_data_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-25 12:39:31.000000 exabel-data-sdk-4.4.0/exabel_data_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 12:39:31.000000 exabel-data-sdk-4.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-25 12:37:21.000000 exabel-data-sdk-4.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:24:36.000000 exabel-data-sdk-4.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-07-21 09:24:36.000000 exabel-data-sdk-4.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:24:36.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:24:36.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:24:36.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:24:36.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/api_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/api_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/api_client/data_set_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/api_client/derived_signal_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/api_client/entity_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/api_client/exabel_api_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:24:36.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/api_client/grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/api_client/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/api_client/grpc/base_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/api_client/grpc/data_set_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/api_client/grpc/derived_signal_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/api_client/grpc/entity_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/api_client/grpc/library_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/api_client/grpc/namespace_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/api_client/grpc/prediction_model_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/api_client/grpc/relationship_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/api_client/grpc/signal_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/api_client/grpc/tag_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/api_client/grpc/time_series_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/api_client/grpc/user_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/api_client/library_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/api_client/namespace_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/api_client/prediction_model_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/api_client/relationship_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/api_client/signal_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/api_client/tag_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/api_client/time_series_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/api_client/user_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10905 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/bulk_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/bulk_insert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:24:36.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/data_classes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/data_classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/data_classes/data_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7661 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/data_classes/derived_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/data_classes/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/data_classes/entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/data_classes/folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/data_classes/folder_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6170 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/data_classes/folder_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/data_classes/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/data_classes/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/data_classes/paging_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/data_classes/prediction_model_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/data_classes/relationship.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/data_classes/relationship_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/data_classes/request_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/data_classes/signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/data_classes/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/data_classes/time_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/data_classes/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/data_set_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/derived_signal_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11318 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/entity_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12035 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/export_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7417 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/library_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/namespace_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/pageable_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/prediction_model_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/proto_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16290 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/relationship_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8795 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/resource_creation_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/search_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/signal_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/tag_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26852 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/time_series_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/client_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/exabel_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13319 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/client/user_login.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:24:36.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/examples/create_time_series_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/examples/get_company_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:24:36.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/query/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/query/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/query/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/query/literal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/query/predicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/query/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/query/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/query/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:24:36.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/base_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/check_company_identifiers_in_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/command_line_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/create_derived_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/create_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8448 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/create_entity_mapping_from_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/create_entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/create_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/create_prediction_model_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/create_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/create_relationship_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/create_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/csv_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/csv_script_with_entity_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/delete_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/delete_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/delete_entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/delete_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/delete_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/delete_relationship_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/delete_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/export_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/get_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/get_entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/get_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/get_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/get_relationship_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/get_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/get_time_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/list_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/list_entity_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/list_folder_accessors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/list_folders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/list_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/list_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/list_relationship_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/list_relationships.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/list_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/list_time_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/list_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5984 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/load_entities_from_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9550 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/load_relationships_from_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/load_time_series_from_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6969 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/load_time_series_from_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/move_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/search_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/share_folder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:24:36.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/sql/read_athena.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/sql/read_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/sql/read_snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/sql/sql_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/unshare_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/update_entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/update_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/update_relationship_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:24:36.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10835 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/services/csv_entity_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/services/csv_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/services/csv_loading_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/services/csv_loading_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/services/csv_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22322 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/services/csv_relationship_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/services/csv_time_series_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/services/csv_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/services/entity_mapping_file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/services/excel_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/services/file_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/services/file_loading_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/services/file_loading_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22073 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/services/file_time_series_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34306 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/services/file_time_series_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/services/file_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/services/file_writer_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:24:36.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/services/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/services/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/services/sql/athena_reader_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/services/sql/bigquery_reader_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/services/sql/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/services/sql/snowflake_reader_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/services/sql/sql_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/services/sql/sql_reader_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:24:36.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:24:36.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:24:36.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/all_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/all_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:24:36.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/analytics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/analytics/all_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/analytics/all_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:24:36.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/all_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/all_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_messages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_messages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9751 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/item_messages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/item_messages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_messages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_messages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_messages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_messages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9333 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14383 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:24:36.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/data/all_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/data/all_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:24:36.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/data/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/data/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/data/v1/all_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/data/v1/all_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_messages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_messages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10371 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_messages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_messages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14969 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21787 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/data/v1/import_job_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/data/v1/import_job_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespace_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespace_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespaces_messages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespaces_messages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_messages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_messages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14512 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18779 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/data/v1/search_messages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/data/v1/search_messages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/data/v1/service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/data/v1/service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_messages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_messages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9149 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_messages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_messages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12207 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16187 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:24:36.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/management/all_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/management/all_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:24:36.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/management/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/management/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/management/v1/all_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/management/v1/all_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/management/v1/folder_messages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/management/v1/folder_messages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13735 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/management/v1/library_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20539 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/management/v1/library_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/management/v1/service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/management/v1/service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_messages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_messages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:24:36.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/math/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/math/aggregation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/math/aggregation_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/math/all_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/math/all_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:24:36.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/time/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/time/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/time/all_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/time/all_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/time/time_range_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/time/time_range_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:24:36.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:24:36.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/annotations_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/annotations_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15566 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/openapiv2_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/openapiv2_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:24:36.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:24:36.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:24:36.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:24:36.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/api_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/api_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/api_client/test_exabel_api_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:24:36.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/data_classes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/data_classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/data_classes/test_data_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/data_classes/test_derived_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/data_classes/test_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/data_classes/test_entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/data_classes/test_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/data_classes/test_folder_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/data_classes/test_folder_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/data_classes/test_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/data_classes/test_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/data_classes/test_prediction_model_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/data_classes/test_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/data_classes/test_relationship_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/data_classes/test_request_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/data_classes/test_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/data_classes/test_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/data_classes/test_time_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/data_classes/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/mock_entity_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/mock_relationship_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/mock_resource_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/mock_signal_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7262 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/test_bulk_insert_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/test_entity_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/test_error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/test_export_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/test_namespace_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/test_pageable_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/test_proto_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6528 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/test_relationship_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/test_resource_creation_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/test_signal_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8784 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/test_time_series_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/exabel_mock_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:24:36.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/query/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/query/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/test_client_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/test_exabel_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/test_user_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:24:36.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/scripts/common_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:24:36.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/scripts/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/scripts/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/scripts/sql/test_read_snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/scripts/sql/test_sql_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/scripts/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/scripts/test_command_line_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/scripts/test_create_entity_mapping_from_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/scripts/test_create_entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/scripts/test_create_relationship_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/scripts/test_csv_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/scripts/test_delete_entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/scripts/test_export_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/scripts/test_load_entities_from_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7969 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/scripts/test_load_relationships_from_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/scripts/test_load_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38073 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/scripts/test_load_time_series_from_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23337 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/scripts/test_load_time_series_from_excel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/scripts/test_update_entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/scripts/test_update_relationship_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:24:36.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:24:36.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/services/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/services/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/services/sql/test_athena_reader_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/services/sql/test_bigquery_reader_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/services/sql/test_snowflake_reader_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/services/sql/test_sql_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/services/sql/test_sql_reader_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/services/test_csv_entity_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/services/test_csv_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27281 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/services/test_csv_relationship_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/services/test_csv_time_series_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/services/test_csv_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/services/test_entity_mapping_file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/services/test_excel_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/services/test_file_loading_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11826 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/services/test_file_time_series_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8177 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/services/test_file_time_series_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/services/test_file_writer_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/test_decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:24:36.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/util/test_batcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/util/test_deprecate_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/util/test_handle_missing_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/util/test_parse_property_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16285 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/util/test_resource_name_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/tests/util/test_type_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:24:36.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/util/batcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/util/case_insensitive_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/util/deprecate_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/util/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/util/handle_missing_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/util/import_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/util/parse_property_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16285 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/util/resource_name_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/util/type_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/exabel_data_sdk/util/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:24:36.000000 exabel-data-sdk-4.5.0/exabel_data_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-07-21 09:24:36.000000 exabel-data-sdk-4.5.0/exabel_data_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19909 2023-07-21 09:24:36.000000 exabel-data-sdk-4.5.0/exabel_data_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 09:24:36.000000 exabel-data-sdk-4.5.0/exabel_data_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-21 09:24:36.000000 exabel-data-sdk-4.5.0/exabel_data_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-21 09:24:36.000000 exabel-data-sdk-4.5.0/exabel_data_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 09:24:36.000000 exabel-data-sdk-4.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-21 09:22:23.000000 exabel-data-sdk-4.5.0/setup.py
```

### Comparing `exabel-data-sdk-4.4.0/LICENSE` & `exabel-data-sdk-4.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/PKG-INFO` & `exabel-data-sdk-4.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exabel-data-sdk
-Version: 4.4.0
+Version: 4.5.0
 Summary: Python SDK for the Exabel Data API
 Home-page: https://github.com/Exabel/python-sdk
 Author: Exabel
 Author-email: support@exabel.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Financial and Insurance Industry
```

### Comparing `exabel-data-sdk-4.4.0/README.md` & `exabel-data-sdk-4.5.0/README.md`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/api_client/data_set_api_client.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/api_client/data_set_api_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/api_client/derived_signal_api_client.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/api_client/derived_signal_api_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/api_client/entity_api_client.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/api_client/entity_api_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/api_client/exabel_api_group.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/api_client/exabel_api_group.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/api_client/grpc/base_grpc_client.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/api_client/grpc/base_grpc_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/api_client/grpc/data_set_grpc_client.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/api_client/grpc/data_set_grpc_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/api_client/grpc/derived_signal_grpc_client.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/api_client/grpc/derived_signal_grpc_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/api_client/grpc/entity_grpc_client.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/api_client/grpc/entity_grpc_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/api_client/grpc/library_grpc_client.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/api_client/grpc/library_grpc_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/api_client/grpc/namespace_grpc_client.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/api_client/grpc/namespace_grpc_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/api_client/grpc/prediction_model_grpc_client.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/api_client/grpc/prediction_model_grpc_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/api_client/grpc/relationship_grpc_client.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/api_client/grpc/relationship_grpc_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/api_client/grpc/signal_grpc_client.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/api_client/grpc/signal_grpc_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/api_client/grpc/tag_grpc_client.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/api_client/grpc/tag_grpc_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/api_client/grpc/time_series_grpc_client.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/api_client/grpc/time_series_grpc_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/api_client/grpc/user_grpc_client.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/api_client/grpc/user_grpc_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/api_client/library_api_client.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/api_client/library_api_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/api_client/relationship_api_client.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/api_client/relationship_api_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/api_client/signal_api_client.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/api_client/signal_api_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/api_client/tag_api_client.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/api_client/tag_api_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/api_client/time_series_api_client.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/api_client/time_series_api_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/api_client/user_api_client.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/api_client/user_api_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/bulk_import.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/bulk_import.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/bulk_insert.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/bulk_insert.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/data_classes/data_set.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/data_classes/data_set.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/data_classes/derived_signal.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/data_classes/derived_signal.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/data_classes/entity.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/data_classes/entity.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/data_classes/entity_type.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/data_classes/entity_type.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/data_classes/folder.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/data_classes/folder.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/data_classes/folder_accessor.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/data_classes/folder_accessor.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/data_classes/folder_item.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/data_classes/folder_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,18 +24,20 @@
     DASHBOARD = ProtoFolderItemType.DASHBOARD
     # Entity drill down view.
     DRILL_DOWN = ProtoFolderItemType.DRILL_DOWN
     # Static tag.
     TAG = ProtoFolderItemType.TAG
     # Screen.
     SCREEN = ProtoFolderItemType.SCREEN
-    # Financial Model
+    # Financial Model.
     FINANCIAL_MODEL = ProtoFolderItemType.FINANCIAL_MODEL
-    # Chart
+    # Chart.
     CHART = ProtoFolderItemType.CHART
+    # KPI mapping.
+    KPI_MAPPING = ProtoFolderItemType.KPI_MAPPING
 
 
 class FolderItem:
     """
     A folder item resource in the Management API.
 
     Attributes:
```

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/data_classes/group.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/data_classes/group.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/data_classes/namespace.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/data_classes/namespace.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/data_classes/paging_result.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/data_classes/paging_result.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/data_classes/prediction_model_run.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/data_classes/prediction_model_run.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/data_classes/relationship.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/data_classes/relationship.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/data_classes/relationship_type.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/data_classes/relationship_type.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/data_classes/request_error.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/data_classes/request_error.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/data_classes/signal.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/data_classes/signal.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/data_classes/tag.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/data_classes/tag.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/data_classes/time_series.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/data_classes/time_series.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/data_classes/user.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/data_classes/user.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/data_set_api.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/data_set_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/derived_signal_api.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/derived_signal_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/entity_api.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/entity_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/error_handler.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/error_handler.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/export_api.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/export_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/library_api.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/library_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/namespace_api.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/namespace_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/pageable_resource.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/pageable_resource.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/prediction_model_api.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/prediction_model_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/proto_utils.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/proto_utils.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/relationship_api.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/relationship_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/resource_creation_result.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/resource_creation_result.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/search_service.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/search_service.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/signal_api.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/signal_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/tag_api.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/tag_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/time_series_api.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/time_series_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -280,14 +280,15 @@
         self,
         parent: str,
         series: Sequence[pd.Series],
         default_known_time: Optional[DefaultKnownTime] = None,
         allow_missing: bool = False,
         create_tag: bool = False,
         status_in_response: bool = False,
+        replace_existing_time_series: bool = False,
     ) -> Optional[Sequence[ResourceCreationResult]]:
         """
         Import multiple time series.
 
         If the time series contains data points that already exist, these data points will be
         overwritten.
 
@@ -305,14 +306,21 @@
                             series for. If a tag already exists, it will be updated when time series
                             are created (or deleted) regardless of the value of this flag.
             status_in_response:
                             If set to true, the status of each time series will be reported as a
                             ResourceCreationResult.
                             If set to false, a failure for one time series will fail the entire
                             request, and a sample of the failures will be reported in the exception.
+            replace_existing_time_series:
+                            Set to true to first delete all data from existing time series. This
+                            means that all historical and point-in-time data for the time series
+                            will be destroyed and replaced with the data in this call.
+                            Use with care! For instance: If this flag is set, and an import job
+                            splits one time series over multiple calls, only the data in the last
+                            call will be kept.
         Returns:
             If status_in_response is set to true, a list of ResourceCreationResult will be returned.
             Otherwise, None is returned.
         """
         response = self.client.import_time_series(
             ImportTimeSeriesRequest(
                 parent=parent,
@@ -320,14 +328,15 @@
                     ProtoTimeSeries(name=ts.name, points=self._series_to_time_series_points(ts))
                     for ts in series
                 ],
                 default_known_time=default_known_time,
                 allow_missing=allow_missing,
                 create_tag=create_tag,
                 status_in_response=status_in_response,
+                replace_existing_time_series=replace_existing_time_series,
             ),
         )
 
         if status_in_response:
             time_series_results = []
             for single_time_series_response, single_time_series in zip(response.responses, series):
                 # The code (integer) given in the response corresponds to google.rpc.Code enum.
@@ -420,14 +429,15 @@
     @deprecate_arguments(threads_for_import=None)
     def bulk_upsert_time_series(
         self,
         series: Sequence[pd.Series],
         create_tag: bool = False,
         threads: int = DEFAULT_NUMBER_OF_THREADS_FOR_IMPORT,
         default_known_time: Optional[DefaultKnownTime] = None,
+        replace_existing_time_series: bool = False,
         retries: int = DEFAULT_NUMBER_OF_RETRIES,
         abort_threshold: Optional[float] = 0.5,
         # Deprecated arguments
         threads_for_import: int = 4,  # pylint: disable=unused-argument
     ) -> ResourceCreationResults[pd.Series]:
         """Import the provided time series in batches.
 
@@ -446,14 +456,21 @@
             threads:        The number of parallel upload threads to use, when falling back to
                             uploading time series individually.
             default_known_time:
                             Specify a default known time policy. This is used to determine
                             the Known Time for data points where a specific known time timestamp
                             has not been given. If not provided, the Exabel API defaults to the
                             current time (upload time) as the Known Time.
+            replace_existing_time_series:
+                            Set to true to first delete all data from existing time series. This
+                            means that all historical and point-in-time data for the time series
+                            will be destroyed and replaced with the data in this call.
+                            Use with care! For instance: If this flag is set, and an import job
+                            splits one time series over multiple calls, only the data in the last
+                            call will be kept.
             retries:        Maximum number of retries to make for each failed request.
             abort_threshold:
                             The threshold for the proportion of failed requests that will cause the
                             upload to be aborted; if it is `None`, the upload is never aborted.
 
         Returns:
             ResourceCreationResults containing the status for each time series that was imported.
@@ -463,14 +480,15 @@
             result = self.import_time_series(
                 parent="signals/-",
                 series=ts_sequence,
                 default_known_time=default_known_time,
                 allow_missing=True,
                 create_tag=create_tag,
                 status_in_response=True,
+                replace_existing_time_series=replace_existing_time_series,
             )
             assert result is not None
             return result
 
         return bulk_import(
             series,
             import_func,
```

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/client/api/user_api.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/client/api/user_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/client/client_config.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/client/client_config.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/client/exabel_client.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/client/exabel_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/client/user_login.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/client/user_login.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/examples/create_time_series_example.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/examples/create_time_series_example.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/examples/get_company_example.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/examples/get_company_example.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/query/column.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/query/column.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/query/dashboard.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/query/dashboard.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/query/literal.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/query/literal.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/query/predicate.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/query/predicate.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/query/query.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/query/query.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/query/signals.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/query/signals.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/actions.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/actions.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/base_script.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/base_script.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/check_company_identifiers_in_csv.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/check_company_identifiers_in_csv.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/command_line_script.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/command_line_script.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/create_derived_signal.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/create_derived_signal.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/create_entity.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/create_entity.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/create_entity_mapping_from_csv.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/create_entity_mapping_from_csv.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/create_entity_type.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/create_entity_type.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/create_folder.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/create_folder.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/create_prediction_model_run.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/create_prediction_model_run.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/create_relationship.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/create_relationship.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/create_relationship_type.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/create_relationship_type.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/create_signal.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/create_signal.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/csv_script.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/csv_script.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/csv_script_with_entity_mapping.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/csv_script_with_entity_mapping.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/delete_entities.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/delete_entities.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/delete_entity.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/delete_entity.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/delete_entity_type.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/delete_entity_type.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/delete_folder.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/delete_folder.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/delete_relationship.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/delete_relationship.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/delete_relationship_type.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/delete_relationship_type.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/delete_signal.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/delete_signal.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/export_data.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/export_data.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/get_entity.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/get_entity.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/get_entity_type.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/get_entity_type.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/get_folder.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/get_folder.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/get_relationship.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/get_relationship.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/get_relationship_type.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/get_relationship_type.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/get_signal.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/get_signal.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/get_time_series.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/get_time_series.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/list_entities.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/list_entities.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/list_entity_types.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/list_entity_types.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/list_folder_accessors.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/list_folder_accessors.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/list_folders.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/list_folders.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/list_items.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/list_items.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/list_relationship_types.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/list_relationship_types.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/list_relationships.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/list_relationships.py`

 * *Files 16% similar despite different names*

```diff
@@ -31,42 +31,46 @@
         )
         self.parser.add_argument(
             "--to-entity",
             required=False,
             type=str,
             help="The resource name of the entity the relationships go to",
         )
+        self.parser.add_argument(
+            "--page-size",
+            required=False,
+            type=int,
+            default=1000,
+            help="The page size to use for retrieving all relationships"
+            " (not applicable when specifying an entity)",
+        )
 
     def run_script(self, client: ExabelClient, args: argparse.Namespace) -> None:
         if args.from_entity and args.to_entity:
             raise ValueError("Specify either the from entity or the to entity, not both.")
         entity = args.from_entity or args.to_entity
         if entity:
             # Check that the entity actually exists
             try:
                 client.entity_api.get_entity(entity)
             except RequestError as error:
                 print(error.message)
                 return
         relationship_type = args.relationship_type
         if args.from_entity is not None:
-            all_relationships = list(
-                client.relationship_api.get_relationships_from_entity_iterator(
-                    relationship_type, entity
-                )
+            all_relationships = client.relationship_api.get_relationships_from_entity_iterator(
+                relationship_type, entity
             )
         elif args.to_entity is not None:
-            all_relationships = list(
-                client.relationship_api.get_relationships_to_entity_iterator(
-                    relationship_type, entity
-                )
+            all_relationships = client.relationship_api.get_relationships_to_entity_iterator(
+                relationship_type, entity
             )
         else:
-            all_relationships = list(
-                client.relationship_api.get_relationships_iterator(relationship_type)
+            all_relationships = client.relationship_api.get_relationships_iterator(
+                relationship_type, page_size=args.page_size
             )
 
         if not all_relationships:
             print("No relationships found")
 
         for relationship in all_relationships:
             print(relationship)
```

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/list_signals.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/list_signals.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/list_time_series.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/list_time_series.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/load_entities_from_csv.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/load_entities_from_csv.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/load_relationships_from_csv.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/load_relationships_from_csv.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/load_time_series_from_file.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/load_time_series_from_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -125,14 +125,21 @@
             action="store_true",
             default=False,
             help="If set, signal names are treated case sensitive. Note that this will disable "
             "lowercasing of other column headers as well, as entities, 'date', and "
             "'known_time'. Take care to maintain correct casing in the file when using this "
             "option.",
         )
+        self.parser.add_argument(
+            "--replace-existing-time-series",
+            required=False,
+            action="store_true",
+            default=False,
+            help="Replace any existing time series when importing",
+        )
 
     def run_script(self, client: ExabelClient, args: argparse.Namespace) -> None:
         try:
             FileTimeSeriesLoader(client).load_time_series(
                 filename=args.filename,
                 entity_mapping_filename=args.entity_mapping_filename,
                 separator=args.sep,
@@ -146,14 +153,15 @@
                 threads=args.threads,
                 dry_run=args.dry_run,
                 retries=args.retries,
                 batch_size=args.batch_size,
                 skip_validation=args.skip_validation,
                 case_sensitive_signals=args.case_sensitive_signals,
                 abort_threshold=args.abort_threshold,
+                replace_existing_time_series=args.replace_existing_time_series,
             )
         except FileLoadingException as e:
             print(e)
             sys.exit(1)
 
 
 if __name__ == "__main__":
```

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/login.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/login.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/move_items.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/move_items.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/search_entities.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/search_entities.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/share_folder.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/share_folder.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/sql/read_athena.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/sql/read_athena.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/sql/read_bigquery.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/sql/read_bigquery.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/sql/read_snowflake.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/sql/read_snowflake.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/sql/sql_script.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/sql/sql_script.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/unshare_folder.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/unshare_folder.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/update_entity_type.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/update_entity_type.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/update_folder.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/update_folder.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/scripts/update_relationship_type.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/scripts/update_relationship_type.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/services/csv_entity_loader.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/services/csv_entity_loader.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/services/csv_reader.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/services/csv_reader.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/services/csv_relationship_loader.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/services/csv_relationship_loader.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/services/csv_time_series_loader.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/services/csv_time_series_loader.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/services/csv_writer.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/services/csv_writer.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/services/entity_mapping_file_reader.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/services/entity_mapping_file_reader.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/services/file_loading_exception.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/services/file_loading_exception.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/services/file_loading_result.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/services/file_loading_result.py`

 * *Files 12% similar despite different names*

```diff
@@ -74,34 +74,38 @@
         aborted:                whether uploading was aborted
         entity_mapping_result:  results of mapping entities in the input file
         created_data_signals:   resource names of data API signals which did not exist from before
         dry_run_results:        resource names of resources which would be created in case of a dry
                                 run
         sheet_name:             the name of the sheet, when applicable
         has_known_time:         whether the file contained a column specifying the known time
+        replaced:               the names of time series requested to be replaced; `None` if
+                                uploading was aborted or it was a dry run
     """
 
     def __init__(
         self,
         results: Optional[ResourceCreationResults[pd.Series]] = None,
         *,
         warnings: Optional[Sequence[str]] = None,
         aborted: bool = False,
         entity_mapping_result: Optional[EntityMappingResult] = None,
         created_data_signals: Optional[Sequence[str]] = None,
         dry_run_results: Optional[Sequence[str]] = None,
         sheet_name: Optional[str] = None,
         has_known_time: bool = False,
+        replaced: Optional[Sequence[str]] = None,
     ):
         super().__init__(results, warnings=warnings, aborted=aborted)
         if entity_mapping_result is None:
             raise ValueError("Entity mapping result must be set.")
         self.entity_mapping_result = entity_mapping_result
         if created_data_signals is None:
             raise ValueError("List of created data API signals must be set.")
         self.created_data_signals = created_data_signals
         self.dry_run_results = dry_run_results
         self.sheet_name = sheet_name
         self.has_known_time = has_known_time
+        self.replaced = replaced
 
     def update(self, other: FileLoadingResult[ResourceT]) -> None:
         raise NotImplementedError("TimeSeriesFileLoadingResult cannot be updated.")
```

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/services/file_time_series_loader.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/services/file_time_series_loader.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import List, Mapping, MutableSequence, Optional, Sequence, Type
 
 from google.protobuf.duration_pb2 import Duration
 
 from exabel_data_sdk import ExabelClient
 from exabel_data_sdk.client.api.bulk_insert import BulkInsertFailedError
 from exabel_data_sdk.client.api.data_classes.signal import Signal
+from exabel_data_sdk.client.api.resource_creation_result import ResourceCreationResults
 from exabel_data_sdk.services.csv_loading_constants import (
     DEFAULT_NUMBER_OF_RETRIES,
     DEFAULT_NUMBER_OF_THREADS,
     DEFAULT_NUMBER_OF_THREADS_FOR_IMPORT,
 )
 from exabel_data_sdk.services.entity_mapping_file_reader import EntityMappingFileReader
 from exabel_data_sdk.services.file_constants import GLOBAL_ENTITY_NAME
@@ -61,14 +62,15 @@
         dry_run: bool = False,
         error_on_any_failure: bool = False,
         retries: int = DEFAULT_NUMBER_OF_RETRIES,
         abort_threshold: Optional[float] = 0.5,
         batch_size: Optional[int] = None,
         skip_validation: bool = False,
         case_sensitive_signals: bool = False,
+        replace_existing_time_series: bool = False,
         return_results: bool = True,
         # Deprecated arguments
         namespace: Optional[str] = None,  # pylint: disable=unused-argument
     ) -> Sequence[TimeSeriesFileLoadingResult]:
         """
         Load a file and upload the time series to the Exabel Data API
 
@@ -102,25 +104,27 @@
             retries: the maximum number of retries to make for each failed request
             abort_threshold: the threshold for the proportion of failed requests that will cause the
                  upload to be aborted; if it is `None`, the upload is never aborted
             batch_size: the number of rows to read and upload in each batch; if not specified, the
                 entire file will be read into memory and uploaded in a single batch
             skip_validation: if True, the time series are not validated before uploading
             case_sensitive_signals: if True, signals are case sensitive
+            replace_existing_time_series: if True, any existing time series are replaced
         """
         if batch_size is not None:
             logger.info(
                 "Reading input data in batches of %d rows. File format with entities in columns is "
                 "not supported. Duplicate detection is best effort.",
                 batch_size,
             )
         entity_mapping = EntityMappingFileReader.read_entity_mapping_file(
             entity_mapping_filename, separator=separator
         )
         results = []
+        replaced_time_series: List[str] = []
         for batch_no, parser in enumerate(
             TimeSeriesFileParser.from_file(filename, separator, batch_size), 1
         ):
             if parser.sheet_name():
                 logger.info("Uploading sheet: %s", parser.sheet_name())
             elif batch_size is not None:
                 logger.info("Uploading batch no: %d", batch_no)
@@ -138,15 +142,19 @@
                 threads=threads,
                 dry_run=dry_run,
                 error_on_any_failure=error_on_any_failure,
                 retries=retries,
                 abort_threshold=abort_threshold,
                 skip_validation=skip_validation,
                 case_sensitive_signals=case_sensitive_signals,
+                replace_existing_time_series=replace_existing_time_series,
+                replaced_time_series=replaced_time_series,
             )
+            if replace_existing_time_series and result.replaced:
+                replaced_time_series.extend(result.replaced)
             if return_results:
                 results.append(result)
         return results
 
     def _load_time_series(
         self,
         *,
@@ -163,14 +171,16 @@
         threads: int = DEFAULT_NUMBER_OF_THREADS,
         dry_run: bool = False,
         error_on_any_failure: bool = False,
         retries: int = DEFAULT_NUMBER_OF_RETRIES,
         abort_threshold: Optional[float] = 0.5,
         skip_validation: bool = False,
         case_sensitive_signals: bool = False,
+        replace_existing_time_series: bool = False,
+        replaced_time_series: Optional[Sequence[str]] = None,
     ) -> TimeSeriesFileLoadingResult:
         """
         Load time series from a parser.
         """
         if dry_run:
             logger.info("Running dry-run...")
         if identifier_type and not entity_type:
@@ -337,34 +347,84 @@
                 entity_mapping_result=entity_mapping_result,
                 created_data_signals=missing_signals,
                 dry_run_results=[str(ts.name) for ts in series],
                 sheet_name=parser.sheet_name(),
                 has_known_time=parsed_file.has_known_time(),
             )
         try:
-            result = self._client.time_series_api.bulk_upsert_time_series(
-                series,
-                create_tag=create_tag,
-                threads=threads,
-                default_known_time=default_known_time,
-                retries=retries,
-                abort_threshold=abort_threshold,
-            )
-            if error_on_any_failure and (result.has_failure() or invalid_series):
-                raise FileLoadingException(
-                    "An error occurred while uploading time series.",
-                    failures=[*result.get_failures(), *invalid_series],
+            replaced_in_this_batch = []
+            if replace_existing_time_series:
+                if replaced_time_series is None:
+                    replaced_time_series = []
+                series_to_replace = []
+                series_to_not_replace = []
+                result = ResourceCreationResults(0, abort_threshold=abort_threshold)
+                for ts in series:
+                    if ts.name in replaced_time_series:
+                        series_to_not_replace.append(ts)
+                    else:
+                        series_to_replace.append(ts)
+                if series_to_not_replace:
+                    logger.info("Uploading already replaced time series")
+                    dont_replace_result = self._client.time_series_api.bulk_upsert_time_series(
+                        series_to_not_replace,
+                        create_tag=create_tag,
+                        threads=threads,
+                        default_known_time=default_known_time,
+                        retries=retries,
+                        abort_threshold=abort_threshold,
+                    )
+                    if error_on_any_failure and (
+                        dont_replace_result.has_failure() or invalid_series
+                    ):
+                        raise FileLoadingException(
+                            "An error occurred while uploading time series.",
+                            failures=[*dont_replace_result.get_failures(), *invalid_series],
+                        )
+                    result.update(dont_replace_result)
+                if series_to_replace:
+                    logger.info("Uploading time series to be replaced")
+                    replace_result = self._client.time_series_api.bulk_upsert_time_series(
+                        series_to_replace,
+                        create_tag=create_tag,
+                        threads=threads,
+                        default_known_time=default_known_time,
+                        retries=retries,
+                        abort_threshold=abort_threshold,
+                        replace_existing_time_series=True,
+                    )
+                    if error_on_any_failure and (replace_result.has_failure() or invalid_series):
+                        raise FileLoadingException(
+                            "An error occurred while uploading time series.",
+                            failures=[*replace_result.get_failures(), *invalid_series],
+                        )
+                    replaced_in_this_batch = [series.name for series in series_to_replace]
+                    result.update(replace_result)
+            else:
+                result = self._client.time_series_api.bulk_upsert_time_series(
+                    series,
+                    create_tag=create_tag,
+                    threads=threads,
+                    default_known_time=default_known_time,
+                    retries=retries,
+                    abort_threshold=abort_threshold,
                 )
+                if error_on_any_failure and (result.has_failure() or invalid_series):
+                    raise FileLoadingException(
+                        "An error occurred while uploading time series.",
+                        failures=[*result.get_failures(), *invalid_series],
+                    )
             return TimeSeriesFileLoadingResult(
                 result,
                 warnings=warnings,
                 entity_mapping_result=entity_mapping_result,
                 created_data_signals=missing_signals,
                 sheet_name=parser.sheet_name(),
                 has_known_time=parsed_file.has_known_time(),
+                replaced=replaced_in_this_batch,
             )
         except BulkInsertFailedError as e:
             # An error summary has already been printed.
             if error_on_any_failure:
                 raise FileLoadingException("An error occurred while uploading time series.") from e
             return TimeSeriesFileLoadingResult(
                 warnings=warnings,
```

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/services/file_time_series_parser.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/services/file_time_series_parser.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/services/file_writer_provider.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/services/file_writer_provider.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/services/sql/athena_reader_configuration.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/services/sql/athena_reader_configuration.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/services/sql/bigquery_reader_configuration.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/services/sql/bigquery_reader_configuration.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/services/sql/snowflake_reader_configuration.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/services/sql/snowflake_reader_configuration.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/services/sql/sql_reader.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/services/sql/sql_reader.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/services/sql/sql_reader_configuration.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/services/sql/sql_reader_configuration.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_messages_pb2.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_messages_pb2.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 _sym_db = _symbol_database.Default()
 from google.api import field_behavior_pb2 as google_dot_api_dot_field__behavior__pb2
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from .....protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n5exabel/api/analytics/v1/derived_signal_messages.proto\x12\x17exabel.api.analytics.v1\x1a\x1fgoogle/api/field_behavior.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a.protoc_gen_openapiv2/options/annotations.proto"\xcb\x02\n\rDerivedSignal\x12A\n\x04name\x18\x01 \x01(\tB3\xe0A\x05\x92A-J\x14"derivedSignals/123"\xca>\x14\xfa\x02\x11derivedSignalName\x12;\n\x05label\x18\x02 \x01(\tB,\x92A)J\x11"close_price_ma7"\x8a\x01\x13^[a-zA-Z_]\\w{0,99}$\x12:\n\nexpression\x18\x03 \x01(\tB&\x92A#J!"close_price().moving_average(7)"\x12<\n\x0bdescription\x18\x04 \x01(\tB\'\x92A$J""Close price 7 day moving average"\x12@\n\x08metadata\x18\x05 \x01(\x0b2..exabel.api.analytics.v1.DerivedSignalMetadata"\xbf\x01\n\x15DerivedSignalMetadata\x12-\n\x08decimals\x18\x01 \x01(\x0b2\x1b.google.protobuf.Int32Value\x128\n\x04unit\x18\x02 \x01(\x0e2*.exabel.api.analytics.v1.DerivedSignalUnit\x12=\n\x04type\x18\x03 \x01(\x0e2*.exabel.api.analytics.v1.DerivedSignalTypeB\x03\xe0A\x03*a\n\x11DerivedSignalUnit\x12\x1f\n\x1bDERIVED_SIGNAL_UNIT_INVALID\x10\x00\x12\n\n\x06NUMBER\x10\x01\x12\t\n\x05RATIO\x10\x02\x12\x14\n\x10RATIO_DIFFERENCE\x10\x03*\x9a\x01\n\x11DerivedSignalType\x12\x1f\n\x1bDERIVED_SIGNAL_TYPE_INVALID\x10\x00\x12\x12\n\x0eDERIVED_SIGNAL\x10\x01\x12\x18\n\x14FILE_UPLOADED_SIGNAL\x10\x02\x12 \n\x1cFILE_UPLOADED_COMPANY_SIGNAL\x10\x03\x12\x14\n\x10PERSISTED_SIGNAL\x10\x04BX\n\x1bcom.exabel.api.analytics.v1B\x1aDerivedSignalMessagesProtoP\x01Z\x1bexabel.com/api/analytics/v1b\x06proto3')
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.analytics.v1.derived_signal_messages_pb2', globals())
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n5exabel/api/analytics/v1/derived_signal_messages.proto\x12\x17exabel.api.analytics.v1\x1a\x1fgoogle/api/field_behavior.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a.protoc_gen_openapiv2/options/annotations.proto"\xcc\x02\n\rDerivedSignal\x12B\n\x04name\x18\x01 \x01(\tB4\x92A-J\x14"derivedSignals/123"\xca>\x14\xfa\x02\x11derivedSignalName\xe2A\x01\x05\x12;\n\x05label\x18\x02 \x01(\tB,\x92A)J\x11"close_price_ma7"\x8a\x01\x13^[a-zA-Z_]\\w{0,99}$\x12:\n\nexpression\x18\x03 \x01(\tB&\x92A#J!"close_price().moving_average(7)"\x12<\n\x0bdescription\x18\x04 \x01(\tB\'\x92A$J""Close price 7 day moving average"\x12@\n\x08metadata\x18\x05 \x01(\x0b2..exabel.api.analytics.v1.DerivedSignalMetadata"\xc0\x01\n\x15DerivedSignalMetadata\x12-\n\x08decimals\x18\x01 \x01(\x0b2\x1b.google.protobuf.Int32Value\x128\n\x04unit\x18\x02 \x01(\x0e2*.exabel.api.analytics.v1.DerivedSignalUnit\x12>\n\x04type\x18\x03 \x01(\x0e2*.exabel.api.analytics.v1.DerivedSignalTypeB\x04\xe2A\x01\x03*a\n\x11DerivedSignalUnit\x12\x1f\n\x1bDERIVED_SIGNAL_UNIT_INVALID\x10\x00\x12\n\n\x06NUMBER\x10\x01\x12\t\n\x05RATIO\x10\x02\x12\x14\n\x10RATIO_DIFFERENCE\x10\x03*\x9a\x01\n\x11DerivedSignalType\x12\x1f\n\x1bDERIVED_SIGNAL_TYPE_INVALID\x10\x00\x12\x12\n\x0eDERIVED_SIGNAL\x10\x01\x12\x18\n\x14FILE_UPLOADED_SIGNAL\x10\x02\x12 \n\x1cFILE_UPLOADED_COMPANY_SIGNAL\x10\x03\x12\x14\n\x10PERSISTED_SIGNAL\x10\x04BX\n\x1bcom.exabel.api.analytics.v1B\x1aDerivedSignalMessagesProtoP\x01Z\x1bexabel.com/api/analytics/v1b\x06proto3')
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.analytics.v1.derived_signal_messages_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b'\n\x1bcom.exabel.api.analytics.v1B\x1aDerivedSignalMessagesProtoP\x01Z\x1bexabel.com/api/analytics/v1'
     _DERIVEDSIGNAL.fields_by_name['name']._options = None
-    _DERIVEDSIGNAL.fields_by_name['name']._serialized_options = b'\xe0A\x05\x92A-J\x14"derivedSignals/123"\xca>\x14\xfa\x02\x11derivedSignalName'
+    _DERIVEDSIGNAL.fields_by_name['name']._serialized_options = b'\x92A-J\x14"derivedSignals/123"\xca>\x14\xfa\x02\x11derivedSignalName\xe2A\x01\x05'
     _DERIVEDSIGNAL.fields_by_name['label']._options = None
     _DERIVEDSIGNAL.fields_by_name['label']._serialized_options = b'\x92A)J\x11"close_price_ma7"\x8a\x01\x13^[a-zA-Z_]\\w{0,99}$'
     _DERIVEDSIGNAL.fields_by_name['expression']._options = None
     _DERIVEDSIGNAL.fields_by_name['expression']._serialized_options = b'\x92A#J!"close_price().moving_average(7)"'
     _DERIVEDSIGNAL.fields_by_name['description']._options = None
     _DERIVEDSIGNAL.fields_by_name['description']._serialized_options = b'\x92A$J""Close price 7 day moving average"'
     _DERIVEDSIGNALMETADATA.fields_by_name['type']._options = None
-    _DERIVEDSIGNALMETADATA.fields_by_name['type']._serialized_options = b'\xe0A\x03'
-    _DERIVEDSIGNALUNIT._serialized_start = 723
-    _DERIVEDSIGNALUNIT._serialized_end = 820
-    _DERIVEDSIGNALTYPE._serialized_start = 823
-    _DERIVEDSIGNALTYPE._serialized_end = 977
-    _DERIVEDSIGNAL._serialized_start = 196
-    _DERIVEDSIGNAL._serialized_end = 527
-    _DERIVEDSIGNALMETADATA._serialized_start = 530
-    _DERIVEDSIGNALMETADATA._serialized_end = 721
+    _DERIVEDSIGNALMETADATA.fields_by_name['type']._serialized_options = b'\xe2A\x01\x03'
+    _globals['_DERIVEDSIGNALUNIT']._serialized_start = 725
+    _globals['_DERIVEDSIGNALUNIT']._serialized_end = 822
+    _globals['_DERIVEDSIGNALTYPE']._serialized_start = 825
+    _globals['_DERIVEDSIGNALTYPE']._serialized_end = 979
+    _globals['_DERIVEDSIGNAL']._serialized_start = 196
+    _globals['_DERIVEDSIGNAL']._serialized_end = 528
+    _globals['_DERIVEDSIGNALMETADATA']._serialized_start = 531
+    _globals['_DERIVEDSIGNALMETADATA']._serialized_end = 723
```

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_service_pb2.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_service_pb2.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 _sym_db = _symbol_database.Default()
 from .....exabel.api.analytics.v1 import derived_signal_messages_pb2 as exabel_dot_api_dot_analytics_dot_v1_dot_derived__signal__messages__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from google.api import field_behavior_pb2 as google_dot_api_dot_field__behavior__pb2
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 from google.protobuf import field_mask_pb2 as google_dot_protobuf_dot_field__mask__pb2
 from .....protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n4exabel/api/analytics/v1/derived_signal_service.proto\x12\x17exabel.api.analytics.v1\x1a5exabel/api/analytics/v1/derived_signal_messages.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1fgoogle/api/field_behavior.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a google/protobuf/field_mask.proto\x1a.protoc_gen_openapiv2/options/annotations.proto"F\n\x17GetDerivedSignalRequest\x12+\n\x04name\x18\x01 \x01(\tB\x1d\xe0A\x02\x92A\x17\xca>\x14\xfa\x02\x11derivedSignalName"i\n\x1aCreateDerivedSignalRequest\x12;\n\x06signal\x18\x01 \x01(\x0b2&.exabel.api.analytics.v1.DerivedSignalB\x03\xe0A\x02\x12\x0e\n\x06folder\x18\x02 \x01(\t"\x8a\x01\n\x1aUpdateDerivedSignalRequest\x12;\n\x06signal\x18\x01 \x01(\x0b2&.exabel.api.analytics.v1.DerivedSignalB\x03\xe0A\x02\x12/\n\x0bupdate_mask\x18\x02 \x01(\x0b2\x1a.google.protobuf.FieldMask"I\n\x1aDeleteDerivedSignalRequest\x12+\n\x04name\x18\x01 \x01(\tB\x1d\xe0A\x02\x92A\x17\xca>\x14\xfa\x02\x11derivedSignalName2\xdb\x05\n\x14DerivedSignalService\x12\xa8\x01\n\x10GetDerivedSignal\x120.exabel.api.analytics.v1.GetDerivedSignalRequest\x1a&.exabel.api.analytics.v1.DerivedSignal":\x82\xd3\xe4\x93\x02\x1d\x12\x1b/v1/{name=derivedSignals/*}\x92A\x14\x12\x12Get derived signal\x12\xb0\x01\n\x13CreateDerivedSignal\x123.exabel.api.analytics.v1.CreateDerivedSignalRequest\x1a&.exabel.api.analytics.v1.DerivedSignal"<\x82\xd3\xe4\x93\x02\x1c"\x12/v1/derivedSignals:\x06signal\x92A\x17\x12\x15Create derived signal\x12\xc0\x01\n\x13UpdateDerivedSignal\x123.exabel.api.analytics.v1.UpdateDerivedSignalRequest\x1a&.exabel.api.analytics.v1.DerivedSignal"L\x82\xd3\xe4\x93\x02,2"/v1/{signal.name=derivedSignals/*}:\x06signal\x92A\x17\x12\x15Update derived signal\x12\xa1\x01\n\x13DeleteDerivedSignal\x123.exabel.api.analytics.v1.DeleteDerivedSignalRequest\x1a\x16.google.protobuf.Empty"=\x82\xd3\xe4\x93\x02\x1d*\x1b/v1/{name=derivedSignals/*}\x92A\x17\x12\x15Delete derived signalBW\n\x1bcom.exabel.api.analytics.v1B\x19DerivedSignalServiceProtoP\x01Z\x1bexabel.com/api/analytics/v1b\x06proto3')
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.analytics.v1.derived_signal_service_pb2', globals())
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n4exabel/api/analytics/v1/derived_signal_service.proto\x12\x17exabel.api.analytics.v1\x1a5exabel/api/analytics/v1/derived_signal_messages.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1fgoogle/api/field_behavior.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a google/protobuf/field_mask.proto\x1a.protoc_gen_openapiv2/options/annotations.proto"G\n\x17GetDerivedSignalRequest\x12,\n\x04name\x18\x01 \x01(\tB\x1e\x92A\x17\xca>\x14\xfa\x02\x11derivedSignalName\xe2A\x01\x02"j\n\x1aCreateDerivedSignalRequest\x12<\n\x06signal\x18\x01 \x01(\x0b2&.exabel.api.analytics.v1.DerivedSignalB\x04\xe2A\x01\x02\x12\x0e\n\x06folder\x18\x02 \x01(\t"\x8b\x01\n\x1aUpdateDerivedSignalRequest\x12<\n\x06signal\x18\x01 \x01(\x0b2&.exabel.api.analytics.v1.DerivedSignalB\x04\xe2A\x01\x02\x12/\n\x0bupdate_mask\x18\x02 \x01(\x0b2\x1a.google.protobuf.FieldMask"J\n\x1aDeleteDerivedSignalRequest\x12,\n\x04name\x18\x01 \x01(\tB\x1e\x92A\x17\xca>\x14\xfa\x02\x11derivedSignalName\xe2A\x01\x022\xdb\x05\n\x14DerivedSignalService\x12\xa8\x01\n\x10GetDerivedSignal\x120.exabel.api.analytics.v1.GetDerivedSignalRequest\x1a&.exabel.api.analytics.v1.DerivedSignal":\x92A\x14\x12\x12Get derived signal\x82\xd3\xe4\x93\x02\x1d\x12\x1b/v1/{name=derivedSignals/*}\x12\xb0\x01\n\x13CreateDerivedSignal\x123.exabel.api.analytics.v1.CreateDerivedSignalRequest\x1a&.exabel.api.analytics.v1.DerivedSignal"<\x92A\x17\x12\x15Create derived signal\x82\xd3\xe4\x93\x02\x1c"\x12/v1/derivedSignals:\x06signal\x12\xc0\x01\n\x13UpdateDerivedSignal\x123.exabel.api.analytics.v1.UpdateDerivedSignalRequest\x1a&.exabel.api.analytics.v1.DerivedSignal"L\x92A\x17\x12\x15Update derived signal\x82\xd3\xe4\x93\x02,2"/v1/{signal.name=derivedSignals/*}:\x06signal\x12\xa1\x01\n\x13DeleteDerivedSignal\x123.exabel.api.analytics.v1.DeleteDerivedSignalRequest\x1a\x16.google.protobuf.Empty"=\x92A\x17\x12\x15Delete derived signal\x82\xd3\xe4\x93\x02\x1d*\x1b/v1/{name=derivedSignals/*}BW\n\x1bcom.exabel.api.analytics.v1B\x19DerivedSignalServiceProtoP\x01Z\x1bexabel.com/api/analytics/v1b\x06proto3')
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.analytics.v1.derived_signal_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b'\n\x1bcom.exabel.api.analytics.v1B\x19DerivedSignalServiceProtoP\x01Z\x1bexabel.com/api/analytics/v1'
     _GETDERIVEDSIGNALREQUEST.fields_by_name['name']._options = None
-    _GETDERIVEDSIGNALREQUEST.fields_by_name['name']._serialized_options = b'\xe0A\x02\x92A\x17\xca>\x14\xfa\x02\x11derivedSignalName'
+    _GETDERIVEDSIGNALREQUEST.fields_by_name['name']._serialized_options = b'\x92A\x17\xca>\x14\xfa\x02\x11derivedSignalName\xe2A\x01\x02'
     _CREATEDERIVEDSIGNALREQUEST.fields_by_name['signal']._options = None
-    _CREATEDERIVEDSIGNALREQUEST.fields_by_name['signal']._serialized_options = b'\xe0A\x02'
+    _CREATEDERIVEDSIGNALREQUEST.fields_by_name['signal']._serialized_options = b'\xe2A\x01\x02'
     _UPDATEDERIVEDSIGNALREQUEST.fields_by_name['signal']._options = None
-    _UPDATEDERIVEDSIGNALREQUEST.fields_by_name['signal']._serialized_options = b'\xe0A\x02'
+    _UPDATEDERIVEDSIGNALREQUEST.fields_by_name['signal']._serialized_options = b'\xe2A\x01\x02'
     _DELETEDERIVEDSIGNALREQUEST.fields_by_name['name']._options = None
-    _DELETEDERIVEDSIGNALREQUEST.fields_by_name['name']._serialized_options = b'\xe0A\x02\x92A\x17\xca>\x14\xfa\x02\x11derivedSignalName'
+    _DELETEDERIVEDSIGNALREQUEST.fields_by_name['name']._serialized_options = b'\x92A\x17\xca>\x14\xfa\x02\x11derivedSignalName\xe2A\x01\x02'
     _DERIVEDSIGNALSERVICE.methods_by_name['GetDerivedSignal']._options = None
-    _DERIVEDSIGNALSERVICE.methods_by_name['GetDerivedSignal']._serialized_options = b'\x82\xd3\xe4\x93\x02\x1d\x12\x1b/v1/{name=derivedSignals/*}\x92A\x14\x12\x12Get derived signal'
+    _DERIVEDSIGNALSERVICE.methods_by_name['GetDerivedSignal']._serialized_options = b'\x92A\x14\x12\x12Get derived signal\x82\xd3\xe4\x93\x02\x1d\x12\x1b/v1/{name=derivedSignals/*}'
     _DERIVEDSIGNALSERVICE.methods_by_name['CreateDerivedSignal']._options = None
-    _DERIVEDSIGNALSERVICE.methods_by_name['CreateDerivedSignal']._serialized_options = b'\x82\xd3\xe4\x93\x02\x1c"\x12/v1/derivedSignals:\x06signal\x92A\x17\x12\x15Create derived signal'
+    _DERIVEDSIGNALSERVICE.methods_by_name['CreateDerivedSignal']._serialized_options = b'\x92A\x17\x12\x15Create derived signal\x82\xd3\xe4\x93\x02\x1c"\x12/v1/derivedSignals:\x06signal'
     _DERIVEDSIGNALSERVICE.methods_by_name['UpdateDerivedSignal']._options = None
-    _DERIVEDSIGNALSERVICE.methods_by_name['UpdateDerivedSignal']._serialized_options = b'\x82\xd3\xe4\x93\x02,2"/v1/{signal.name=derivedSignals/*}:\x06signal\x92A\x17\x12\x15Update derived signal'
+    _DERIVEDSIGNALSERVICE.methods_by_name['UpdateDerivedSignal']._serialized_options = b'\x92A\x17\x12\x15Update derived signal\x82\xd3\xe4\x93\x02,2"/v1/{signal.name=derivedSignals/*}:\x06signal'
     _DERIVEDSIGNALSERVICE.methods_by_name['DeleteDerivedSignal']._options = None
-    _DERIVEDSIGNALSERVICE.methods_by_name['DeleteDerivedSignal']._serialized_options = b'\x82\xd3\xe4\x93\x02\x1d*\x1b/v1/{name=derivedSignals/*}\x92A\x17\x12\x15Delete derived signal'
-    _GETDERIVEDSIGNALREQUEST._serialized_start = 310
-    _GETDERIVEDSIGNALREQUEST._serialized_end = 380
-    _CREATEDERIVEDSIGNALREQUEST._serialized_start = 382
-    _CREATEDERIVEDSIGNALREQUEST._serialized_end = 487
-    _UPDATEDERIVEDSIGNALREQUEST._serialized_start = 490
-    _UPDATEDERIVEDSIGNALREQUEST._serialized_end = 628
-    _DELETEDERIVEDSIGNALREQUEST._serialized_start = 630
-    _DELETEDERIVEDSIGNALREQUEST._serialized_end = 703
-    _DERIVEDSIGNALSERVICE._serialized_start = 706
-    _DERIVEDSIGNALSERVICE._serialized_end = 1437
+    _DERIVEDSIGNALSERVICE.methods_by_name['DeleteDerivedSignal']._serialized_options = b'\x92A\x17\x12\x15Delete derived signal\x82\xd3\xe4\x93\x02\x1d*\x1b/v1/{name=derivedSignals/*}'
+    _globals['_GETDERIVEDSIGNALREQUEST']._serialized_start = 310
+    _globals['_GETDERIVEDSIGNALREQUEST']._serialized_end = 381
+    _globals['_CREATEDERIVEDSIGNALREQUEST']._serialized_start = 383
+    _globals['_CREATEDERIVEDSIGNALREQUEST']._serialized_end = 489
+    _globals['_UPDATEDERIVEDSIGNALREQUEST']._serialized_start = 492
+    _globals['_UPDATEDERIVEDSIGNALREQUEST']._serialized_end = 631
+    _globals['_DELETEDERIVEDSIGNALREQUEST']._serialized_start = 633
+    _globals['_DELETEDERIVEDSIGNALREQUEST']._serialized_end = 707
+    _globals['_DERIVEDSIGNALSERVICE']._serialized_start = 710
+    _globals['_DERIVEDSIGNALSERVICE']._serialized_end = 1441
```

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_service_pb2_grpc.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/item_messages_pb2.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/item_messages_pb2.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 _sym_db = _symbol_database.Default()
 from google.api import field_behavior_pb2 as google_dot_api_dot_field__behavior__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n+exabel/api/analytics/v1/item_messages.proto\x12\x17exabel.api.analytics.v1\x1a\x1fgoogle/api/field_behavior.proto\x1a\x1fgoogle/protobuf/timestamp.proto"\xdd\x01\n\x0cItemMetadata\x124\n\x0bcreate_time\x18\x01 \x01(\x0b2\x1a.google.protobuf.TimestampB\x03\xe0A\x03\x124\n\x0bupdate_time\x18\x02 \x01(\x0b2\x1a.google.protobuf.TimestampB\x03\xe0A\x03\x12\x17\n\ncreated_by\x18\x03 \x01(\tB\x03\xe0A\x03\x12\x17\n\nupdated_by\x18\x04 \x01(\tB\x03\xe0A\x03\x12\x1e\n\x0cwrite_access\x18\x05 \x01(\x08B\x03\xe0A\x03H\x00\x88\x01\x01B\x0f\n\r_write_accessBO\n\x1bcom.exabel.api.analytics.v1B\x11ItemMessagesProtoP\x01Z\x1bexabel.com/api/analytics/v1b\x06proto3')
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.analytics.v1.item_messages_pb2', globals())
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n+exabel/api/analytics/v1/item_messages.proto\x12\x17exabel.api.analytics.v1\x1a\x1fgoogle/api/field_behavior.proto\x1a\x1fgoogle/protobuf/timestamp.proto"\xe2\x01\n\x0cItemMetadata\x125\n\x0bcreate_time\x18\x01 \x01(\x0b2\x1a.google.protobuf.TimestampB\x04\xe2A\x01\x03\x125\n\x0bupdate_time\x18\x02 \x01(\x0b2\x1a.google.protobuf.TimestampB\x04\xe2A\x01\x03\x12\x18\n\ncreated_by\x18\x03 \x01(\tB\x04\xe2A\x01\x03\x12\x18\n\nupdated_by\x18\x04 \x01(\tB\x04\xe2A\x01\x03\x12\x1f\n\x0cwrite_access\x18\x05 \x01(\x08B\x04\xe2A\x01\x03H\x00\x88\x01\x01B\x0f\n\r_write_accessBO\n\x1bcom.exabel.api.analytics.v1B\x11ItemMessagesProtoP\x01Z\x1bexabel.com/api/analytics/v1b\x06proto3')
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.analytics.v1.item_messages_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b'\n\x1bcom.exabel.api.analytics.v1B\x11ItemMessagesProtoP\x01Z\x1bexabel.com/api/analytics/v1'
     _ITEMMETADATA.fields_by_name['create_time']._options = None
-    _ITEMMETADATA.fields_by_name['create_time']._serialized_options = b'\xe0A\x03'
+    _ITEMMETADATA.fields_by_name['create_time']._serialized_options = b'\xe2A\x01\x03'
     _ITEMMETADATA.fields_by_name['update_time']._options = None
-    _ITEMMETADATA.fields_by_name['update_time']._serialized_options = b'\xe0A\x03'
+    _ITEMMETADATA.fields_by_name['update_time']._serialized_options = b'\xe2A\x01\x03'
     _ITEMMETADATA.fields_by_name['created_by']._options = None
-    _ITEMMETADATA.fields_by_name['created_by']._serialized_options = b'\xe0A\x03'
+    _ITEMMETADATA.fields_by_name['created_by']._serialized_options = b'\xe2A\x01\x03'
     _ITEMMETADATA.fields_by_name['updated_by']._options = None
-    _ITEMMETADATA.fields_by_name['updated_by']._serialized_options = b'\xe0A\x03'
+    _ITEMMETADATA.fields_by_name['updated_by']._serialized_options = b'\xe2A\x01\x03'
     _ITEMMETADATA.fields_by_name['write_access']._options = None
-    _ITEMMETADATA.fields_by_name['write_access']._serialized_options = b'\xe0A\x03'
-    _ITEMMETADATA._serialized_start = 139
-    _ITEMMETADATA._serialized_end = 360
+    _ITEMMETADATA.fields_by_name['write_access']._serialized_options = b'\xe2A\x01\x03'
+    _globals['_ITEMMETADATA']._serialized_start = 139
+    _globals['_ITEMMETADATA']._serialized_end = 365
```

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_messages_pb2.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_messages_pb2.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 _sym_db = _symbol_database.Default()
 from google.api import field_behavior_pb2 as google_dot_api_dot_field__behavior__pb2
 from .....protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n7exabel/api/analytics/v1/prediction_model_messages.proto\x12\x17exabel.api.analytics.v1\x1a\x1fgoogle/api/field_behavior.proto\x1a.protoc_gen_openapiv2/options/annotations.proto"\x96\x02\n\x12PredictionModelRun\x123\n\x04name\x18\x01 \x01(\tB%\xe0A\x03\x92A\x1fJ\x1d"predictionModels/123/runs/3"\x124\n\x0bdescription\x18\x02 \x01(\tB\x1f\x92A\x1cJ\x1a"Initiated by API request"\x12B\n\rconfiguration\x18\x03 \x01(\x0e2+.exabel.api.analytics.v1.ModelConfiguration\x12!\n\x14configuration_source\x18\x04 \x01(\x05H\x00\x88\x01\x01\x12\x15\n\rauto_activate\x18\x05 \x01(\x08B\x17\n\x15_configuration_source*e\n\x12ModelConfiguration\x12%\n!MODEL_CONFIGURATION_NOT_SPECIFIED\x10\x00\x12\n\n\x06LATEST\x10\x01\x12\n\n\x06ACTIVE\x10\x02\x12\x10\n\x0cSPECIFIC_RUN\x10\x03BZ\n\x1bcom.exabel.api.analytics.v1B\x1cPredictionModelMessagesProtoP\x01Z\x1bexabel.com/api/analytics/v1b\x06proto3')
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.analytics.v1.prediction_model_messages_pb2', globals())
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n7exabel/api/analytics/v1/prediction_model_messages.proto\x12\x17exabel.api.analytics.v1\x1a\x1fgoogle/api/field_behavior.proto\x1a.protoc_gen_openapiv2/options/annotations.proto"\x97\x02\n\x12PredictionModelRun\x124\n\x04name\x18\x01 \x01(\tB&\x92A\x1fJ\x1d"predictionModels/123/runs/3"\xe2A\x01\x03\x124\n\x0bdescription\x18\x02 \x01(\tB\x1f\x92A\x1cJ\x1a"Initiated by API request"\x12B\n\rconfiguration\x18\x03 \x01(\x0e2+.exabel.api.analytics.v1.ModelConfiguration\x12!\n\x14configuration_source\x18\x04 \x01(\x05H\x00\x88\x01\x01\x12\x15\n\rauto_activate\x18\x05 \x01(\x08B\x17\n\x15_configuration_source*e\n\x12ModelConfiguration\x12%\n!MODEL_CONFIGURATION_NOT_SPECIFIED\x10\x00\x12\n\n\x06LATEST\x10\x01\x12\n\n\x06ACTIVE\x10\x02\x12\x10\n\x0cSPECIFIC_RUN\x10\x03BZ\n\x1bcom.exabel.api.analytics.v1B\x1cPredictionModelMessagesProtoP\x01Z\x1bexabel.com/api/analytics/v1b\x06proto3')
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.analytics.v1.prediction_model_messages_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b'\n\x1bcom.exabel.api.analytics.v1B\x1cPredictionModelMessagesProtoP\x01Z\x1bexabel.com/api/analytics/v1'
     _PREDICTIONMODELRUN.fields_by_name['name']._options = None
-    _PREDICTIONMODELRUN.fields_by_name['name']._serialized_options = b'\xe0A\x03\x92A\x1fJ\x1d"predictionModels/123/runs/3"'
+    _PREDICTIONMODELRUN.fields_by_name['name']._serialized_options = b'\x92A\x1fJ\x1d"predictionModels/123/runs/3"\xe2A\x01\x03'
     _PREDICTIONMODELRUN.fields_by_name['description']._options = None
     _PREDICTIONMODELRUN.fields_by_name['description']._serialized_options = b'\x92A\x1cJ\x1a"Initiated by API request"'
-    _MODELCONFIGURATION._serialized_start = 446
-    _MODELCONFIGURATION._serialized_end = 547
-    _PREDICTIONMODELRUN._serialized_start = 166
-    _PREDICTIONMODELRUN._serialized_end = 444
+    _globals['_MODELCONFIGURATION']._serialized_start = 447
+    _globals['_MODELCONFIGURATION']._serialized_end = 548
+    _globals['_PREDICTIONMODELRUN']._serialized_start = 166
+    _globals['_PREDICTIONMODELRUN']._serialized_end = 445
```

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_service_pb2.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_service_pb2.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 _sym_db = _symbol_database.Default()
 from .....exabel.api.analytics.v1 import prediction_model_messages_pb2 as exabel_dot_api_dot_analytics_dot_v1_dot_prediction__model__messages__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from google.api import field_behavior_pb2 as google_dot_api_dot_field__behavior__pb2
 from .....protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n6exabel/api/analytics/v1/prediction_model_service.proto\x12\x17exabel.api.analytics.v1\x1a7exabel/api/analytics/v1/prediction_model_messages.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1fgoogle/api/field_behavior.proto\x1a.protoc_gen_openapiv2/options/annotations.proto"\x91\x01\n\x1fCreatePredictionModelRunRequest\x12/\n\x06parent\x18\x01 \x01(\tB\x1f\xe0A\x02\x92A\x19\xca>\x16\xfa\x02\x13predictionModelName\x12=\n\x03run\x18\x02 \x01(\x0b2+.exabel.api.analytics.v1.PredictionModelRunB\x03\xe0A\x022\xe8\x01\n\x16PredictionModelService\x12\xcd\x01\n\x18CreatePredictionModelRun\x128.exabel.api.analytics.v1.CreatePredictionModelRunRequest\x1a+.exabel.api.analytics.v1.PredictionModelRun"J\x82\xd3\xe4\x93\x02+"$/v1/{parent=predictionModels/*}/runs:\x03run\x92A\x16\x12\x14Run prediction modelBY\n\x1bcom.exabel.api.analytics.v1B\x1bPredictionModelServiceProtoP\x01Z\x1bexabel.com/api/analytics/v1b\x06proto3')
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.analytics.v1.prediction_model_service_pb2', globals())
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n6exabel/api/analytics/v1/prediction_model_service.proto\x12\x17exabel.api.analytics.v1\x1a7exabel/api/analytics/v1/prediction_model_messages.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1fgoogle/api/field_behavior.proto\x1a.protoc_gen_openapiv2/options/annotations.proto"\x93\x01\n\x1fCreatePredictionModelRunRequest\x120\n\x06parent\x18\x01 \x01(\tB \x92A\x19\xca>\x16\xfa\x02\x13predictionModelName\xe2A\x01\x02\x12>\n\x03run\x18\x02 \x01(\x0b2+.exabel.api.analytics.v1.PredictionModelRunB\x04\xe2A\x01\x022\xe8\x01\n\x16PredictionModelService\x12\xcd\x01\n\x18CreatePredictionModelRun\x128.exabel.api.analytics.v1.CreatePredictionModelRunRequest\x1a+.exabel.api.analytics.v1.PredictionModelRun"J\x92A\x16\x12\x14Run prediction model\x82\xd3\xe4\x93\x02+"$/v1/{parent=predictionModels/*}/runs:\x03runBY\n\x1bcom.exabel.api.analytics.v1B\x1bPredictionModelServiceProtoP\x01Z\x1bexabel.com/api/analytics/v1b\x06proto3')
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.analytics.v1.prediction_model_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b'\n\x1bcom.exabel.api.analytics.v1B\x1bPredictionModelServiceProtoP\x01Z\x1bexabel.com/api/analytics/v1'
     _CREATEPREDICTIONMODELRUNREQUEST.fields_by_name['parent']._options = None
-    _CREATEPREDICTIONMODELRUNREQUEST.fields_by_name['parent']._serialized_options = b'\xe0A\x02\x92A\x19\xca>\x16\xfa\x02\x13predictionModelName'
+    _CREATEPREDICTIONMODELRUNREQUEST.fields_by_name['parent']._serialized_options = b'\x92A\x19\xca>\x16\xfa\x02\x13predictionModelName\xe2A\x01\x02'
     _CREATEPREDICTIONMODELRUNREQUEST.fields_by_name['run']._options = None
-    _CREATEPREDICTIONMODELRUNREQUEST.fields_by_name['run']._serialized_options = b'\xe0A\x02'
+    _CREATEPREDICTIONMODELRUNREQUEST.fields_by_name['run']._serialized_options = b'\xe2A\x01\x02'
     _PREDICTIONMODELSERVICE.methods_by_name['CreatePredictionModelRun']._options = None
-    _PREDICTIONMODELSERVICE.methods_by_name['CreatePredictionModelRun']._serialized_options = b'\x82\xd3\xe4\x93\x02+"$/v1/{parent=predictionModels/*}/runs:\x03run\x92A\x16\x12\x14Run prediction model'
-    _CREATEPREDICTIONMODELRUNREQUEST._serialized_start = 252
-    _CREATEPREDICTIONMODELRUNREQUEST._serialized_end = 397
-    _PREDICTIONMODELSERVICE._serialized_start = 400
-    _PREDICTIONMODELSERVICE._serialized_end = 632
+    _PREDICTIONMODELSERVICE.methods_by_name['CreatePredictionModelRun']._serialized_options = b'\x92A\x16\x12\x14Run prediction model\x82\xd3\xe4\x93\x02+"$/v1/{parent=predictionModels/*}/runs:\x03run'
+    _globals['_CREATEPREDICTIONMODELRUNREQUEST']._serialized_start = 252
+    _globals['_CREATEPREDICTIONMODELRUNREQUEST']._serialized_end = 399
+    _globals['_PREDICTIONMODELSERVICE']._serialized_start = 402
+    _globals['_PREDICTIONMODELSERVICE']._serialized_end = 634
```

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_service_pb2_grpc.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/service_pb2.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/service_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 _sym_db = _symbol_database.Default()
 from .....protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n%exabel/api/analytics/v1/service.proto\x12\x17exabel.api.analytics.v1\x1a.protoc_gen_openapiv2/options/annotations.protoB\xe5\x02\n\x1bcom.exabel.api.analytics.v1B\x0cServiceProtoP\x01Z\x1bexabel.com/api/analytics/v1\x92A\x97\x02\x12T\n\x14Exabel Analytics API"5\n\x06Exabel\x12\x17https://www.exabel.com/\x1a\x12support@exabel.com2\x051.0.0\x1a\x18analytics.api.exabel.com*\x01\x022\x10application/json:\x10application/jsonZ\x1c\n\x1a\n\x07API key\x12\x0f\x08\x02\x1a\tx-api-key \x02b\r\n\x0b\n\x07API key\x12\x00rQ\n#More about the Exabel Analytics API\x12*https://help.exabel.com/docs/analytics-apib\x06proto3')
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.analytics.v1.service_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.analytics.v1.service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b'\n\x1bcom.exabel.api.analytics.v1B\x0cServiceProtoP\x01Z\x1bexabel.com/api/analytics/v1\x92A\x97\x02\x12T\n\x14Exabel Analytics API"5\n\x06Exabel\x12\x17https://www.exabel.com/\x1a\x12support@exabel.com2\x051.0.0\x1a\x18analytics.api.exabel.com*\x01\x022\x10application/json:\x10application/jsonZ\x1c\n\x1a\n\x07API key\x12\x0f\x08\x02\x1a\tx-api-key \x02b\r\n\x0b\n\x07API key\x12\x00rQ\n#More about the Exabel Analytics API\x12*https://help.exabel.com/docs/analytics-api'
```

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_messages_pb2.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_messages_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 _sym_db = _symbol_database.Default()
 from .....exabel.api.analytics.v1 import item_messages_pb2 as exabel_dot_api_dot_analytics_dot_v1_dot_item__messages__pb2
 from google.api import field_behavior_pb2 as google_dot_api_dot_field__behavior__pb2
 from .....protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n*exabel/api/analytics/v1/tag_messages.proto\x12\x17exabel.api.analytics.v1\x1a+exabel/api/analytics/v1/item_messages.proto\x1a\x1fgoogle/api/field_behavior.proto\x1a.protoc_gen_openapiv2/options/annotations.proto"\xc5\x01\n\x03Tag\x12\x11\n\x04name\x18\x01 \x01(\tB\x03\xe0A\x03\x12#\n\x0cdisplay_name\x18\x02 \x01(\tB\r\x92A\nJ\x08"My tag"\x12.\n\x0bdescription\x18\x03 \x01(\tB\x19\x92A\x16J\x14"My tag description"\x12\x18\n\x0bentity_type\x18\x04 \x01(\tB\x03\xe0A\x03\x12<\n\x08metadata\x18\x05 \x01(\x0b2%.exabel.api.analytics.v1.ItemMetadataB\x03\xe0A\x03BN\n\x1bcom.exabel.api.analytics.v1B\x10TagMessagesProtoP\x01Z\x1bexabel.com/api/analytics/v1b\x06proto3')
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.analytics.v1.tag_messages_pb2', globals())
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n*exabel/api/analytics/v1/tag_messages.proto\x12\x17exabel.api.analytics.v1\x1a+exabel/api/analytics/v1/item_messages.proto\x1a\x1fgoogle/api/field_behavior.proto\x1a.protoc_gen_openapiv2/options/annotations.proto"\xc8\x01\n\x03Tag\x12\x12\n\x04name\x18\x01 \x01(\tB\x04\xe2A\x01\x03\x12#\n\x0cdisplay_name\x18\x02 \x01(\tB\r\x92A\nJ\x08"My tag"\x12.\n\x0bdescription\x18\x03 \x01(\tB\x19\x92A\x16J\x14"My tag description"\x12\x19\n\x0bentity_type\x18\x04 \x01(\tB\x04\xe2A\x01\x03\x12=\n\x08metadata\x18\x05 \x01(\x0b2%.exabel.api.analytics.v1.ItemMetadataB\x04\xe2A\x01\x03BN\n\x1bcom.exabel.api.analytics.v1B\x10TagMessagesProtoP\x01Z\x1bexabel.com/api/analytics/v1b\x06proto3')
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.analytics.v1.tag_messages_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b'\n\x1bcom.exabel.api.analytics.v1B\x10TagMessagesProtoP\x01Z\x1bexabel.com/api/analytics/v1'
     _TAG.fields_by_name['name']._options = None
-    _TAG.fields_by_name['name']._serialized_options = b'\xe0A\x03'
+    _TAG.fields_by_name['name']._serialized_options = b'\xe2A\x01\x03'
     _TAG.fields_by_name['display_name']._options = None
     _TAG.fields_by_name['display_name']._serialized_options = b'\x92A\nJ\x08"My tag"'
     _TAG.fields_by_name['description']._options = None
     _TAG.fields_by_name['description']._serialized_options = b'\x92A\x16J\x14"My tag description"'
     _TAG.fields_by_name['entity_type']._options = None
-    _TAG.fields_by_name['entity_type']._serialized_options = b'\xe0A\x03'
+    _TAG.fields_by_name['entity_type']._serialized_options = b'\xe2A\x01\x03'
     _TAG.fields_by_name['metadata']._options = None
-    _TAG.fields_by_name['metadata']._serialized_options = b'\xe0A\x03'
-    _TAG._serialized_start = 198
-    _TAG._serialized_end = 395
+    _TAG.fields_by_name['metadata']._serialized_options = b'\xe2A\x01\x03'
+    _globals['_TAG']._serialized_start = 198
+    _globals['_TAG']._serialized_end = 398
```

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_service_pb2.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_service_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,74 +1,75 @@
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 _sym_db = _symbol_database.Default()
 from .....exabel.api.analytics.v1 import tag_messages_pb2 as exabel_dot_api_dot_analytics_dot_v1_dot_tag__messages__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from google.api import field_behavior_pb2 as google_dot_api_dot_field__behavior__pb2
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 from google.protobuf import field_mask_pb2 as google_dot_protobuf_dot_field__mask__pb2
 from .....protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n)exabel/api/analytics/v1/tag_service.proto\x12\x17exabel.api.analytics.v1\x1a*exabel/api/analytics/v1/tag_messages.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1fgoogle/api/field_behavior.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a google/protobuf/field_mask.proto\x1a.protoc_gen_openapiv2/options/annotations.proto"R\n\x10CreateTagRequest\x12.\n\x03tag\x18\x01 \x01(\x0b2\x1c.exabel.api.analytics.v1.TagB\x03\xe0A\x02\x12\x0e\n\x06folder\x18\x02 \x01(\t"2\n\rGetTagRequest\x12!\n\x04name\x18\x01 \x01(\tB\x13\xe0A\x02\x92A\r\xca>\n\xfa\x02\x07tagName"s\n\x10UpdateTagRequest\x12.\n\x03tag\x18\x01 \x01(\x0b2\x1c.exabel.api.analytics.v1.TagB\x03\xe0A\x02\x12/\n\x0bupdate_mask\x18\x02 \x01(\x0b2\x1a.google.protobuf.FieldMask"5\n\x10DeleteTagRequest\x12!\n\x04name\x18\x01 \x01(\tB\x13\xe0A\x02\x92A\r\xca>\n\xfa\x02\x07tagName"8\n\x0fListTagsRequest\x12\x11\n\tpage_size\x18\x01 \x01(\x05\x12\x12\n\npage_token\x18\x02 \x01(\t"k\n\x10ListTagsResponse\x12*\n\x04tags\x18\x01 \x03(\x0b2\x1c.exabel.api.analytics.v1.Tag\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\x12\x12\n\ntotal_size\x18\x03 \x01(\x05"M\n\x12AddEntitiesRequest\x12!\n\x04name\x18\x01 \x01(\tB\x13\xe0A\x02\x92A\r\xca>\n\xfa\x02\x07tagName\x12\x14\n\x0centity_names\x18\x02 \x03(\t"\x15\n\x13AddEntitiesResponse"P\n\x15RemoveEntitiesRequest\x12!\n\x04name\x18\x01 \x01(\tB\x13\xe0A\x02\x92A\r\xca>\n\xfa\x02\x07tagName\x12\x14\n\x0centity_names\x18\x02 \x03(\t"\x18\n\x16RemoveEntitiesResponse"d\n\x16ListTagEntitiesRequest\x12#\n\x06parent\x18\x01 \x01(\tB\x13\xe0A\x02\x92A\r\xca>\n\xfa\x02\x07tagName\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12\x12\n\npage_token\x18\x03 \x01(\t"\\\n\x17ListTagEntitiesResponse\x12\x14\n\x0centity_names\x18\x01 \x03(\t\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\x12\x12\n\ntotal_size\x18\x03 \x01(\x052\xa5\t\n\nTagService\x12z\n\tCreateTag\x12).exabel.api.analytics.v1.CreateTagRequest\x1a\x1c.exabel.api.analytics.v1.Tag"$\x82\xd3\xe4\x93\x02\x0f"\x08/v1/tags:\x03tag\x92A\x0c\x12\nCreate tag\x12u\n\x06GetTag\x12&.exabel.api.analytics.v1.GetTagRequest\x1a\x1c.exabel.api.analytics.v1.Tag"%\x82\xd3\xe4\x93\x02\x13\x12\x11/v1/{name=tags/*}\x92A\t\x12\x07Get tag\x12\x87\x01\n\tUpdateTag\x12).exabel.api.analytics.v1.UpdateTagRequest\x1a\x1c.exabel.api.analytics.v1.Tag"1\x82\xd3\xe4\x93\x02\x1c2\x15/v1/{tag.name=tags/*}:\x03tag\x92A\x0c\x12\nUpdate tag\x12x\n\tDeleteTag\x12).exabel.api.analytics.v1.DeleteTagRequest\x1a\x16.google.protobuf.Empty"(\x82\xd3\xe4\x93\x02\x13*\x11/v1/{name=tags/*}\x92A\x0c\x12\nDelete tag\x12\x7f\n\x08ListTags\x12(.exabel.api.analytics.v1.ListTagsRequest\x1a).exabel.api.analytics.v1.ListTagsResponse"\x1e\x82\xd3\xe4\x93\x02\n\x12\x08/v1/tags\x92A\x0b\x12\tList tags\x12\xaa\x01\n\x0bAddEntities\x12+.exabel.api.analytics.v1.AddEntitiesRequest\x1a,.exabel.api.analytics.v1.AddEntitiesResponse"@\x82\xd3\xe4\x93\x02""\x1d/v1/{name=tags/*}:addEntities:\x01*\x92A\x15\x12\x13Add entities to tag\x12\xbb\x01\n\x0eRemoveEntities\x12..exabel.api.analytics.v1.RemoveEntitiesRequest\x1a/.exabel.api.analytics.v1.RemoveEntitiesResponse"H\x82\xd3\xe4\x93\x02%" /v1/{name=tags/*}:removeEntities:\x01*\x92A\x1a\x12\x18Remove entities from tag\x12\xb3\x01\n\x0fListTagEntities\x12/.exabel.api.analytics.v1.ListTagEntitiesRequest\x1a0.exabel.api.analytics.v1.ListTagEntitiesResponse"=\x82\xd3\xe4\x93\x02\x1e\x12\x1c/v1/{parent=tags/*}/entities\x92A\x16\x12\x14List entities in tagBM\n\x1bcom.exabel.api.analytics.v1B\x0fTagServiceProtoP\x01Z\x1bexabel.com/api/analytics/v1b\x06proto3')
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.analytics.v1.tag_service_pb2', globals())
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n)exabel/api/analytics/v1/tag_service.proto\x12\x17exabel.api.analytics.v1\x1a*exabel/api/analytics/v1/tag_messages.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1fgoogle/api/field_behavior.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a google/protobuf/field_mask.proto\x1a.protoc_gen_openapiv2/options/annotations.proto"S\n\x10CreateTagRequest\x12/\n\x03tag\x18\x01 \x01(\x0b2\x1c.exabel.api.analytics.v1.TagB\x04\xe2A\x01\x02\x12\x0e\n\x06folder\x18\x02 \x01(\t"3\n\rGetTagRequest\x12"\n\x04name\x18\x01 \x01(\tB\x14\x92A\r\xca>\n\xfa\x02\x07tagName\xe2A\x01\x02"t\n\x10UpdateTagRequest\x12/\n\x03tag\x18\x01 \x01(\x0b2\x1c.exabel.api.analytics.v1.TagB\x04\xe2A\x01\x02\x12/\n\x0bupdate_mask\x18\x02 \x01(\x0b2\x1a.google.protobuf.FieldMask"6\n\x10DeleteTagRequest\x12"\n\x04name\x18\x01 \x01(\tB\x14\x92A\r\xca>\n\xfa\x02\x07tagName\xe2A\x01\x02"8\n\x0fListTagsRequest\x12\x11\n\tpage_size\x18\x01 \x01(\x05\x12\x12\n\npage_token\x18\x02 \x01(\t"k\n\x10ListTagsResponse\x12*\n\x04tags\x18\x01 \x03(\x0b2\x1c.exabel.api.analytics.v1.Tag\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\x12\x12\n\ntotal_size\x18\x03 \x01(\x05"N\n\x12AddEntitiesRequest\x12"\n\x04name\x18\x01 \x01(\tB\x14\x92A\r\xca>\n\xfa\x02\x07tagName\xe2A\x01\x02\x12\x14\n\x0centity_names\x18\x02 \x03(\t"\x15\n\x13AddEntitiesResponse"Q\n\x15RemoveEntitiesRequest\x12"\n\x04name\x18\x01 \x01(\tB\x14\x92A\r\xca>\n\xfa\x02\x07tagName\xe2A\x01\x02\x12\x14\n\x0centity_names\x18\x02 \x03(\t"\x18\n\x16RemoveEntitiesResponse"e\n\x16ListTagEntitiesRequest\x12$\n\x06parent\x18\x01 \x01(\tB\x14\x92A\r\xca>\n\xfa\x02\x07tagName\xe2A\x01\x02\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12\x12\n\npage_token\x18\x03 \x01(\t"\\\n\x17ListTagEntitiesResponse\x12\x14\n\x0centity_names\x18\x01 \x03(\t\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\x12\x12\n\ntotal_size\x18\x03 \x01(\x052\xa5\t\n\nTagService\x12z\n\tCreateTag\x12).exabel.api.analytics.v1.CreateTagRequest\x1a\x1c.exabel.api.analytics.v1.Tag"$\x92A\x0c\x12\nCreate tag\x82\xd3\xe4\x93\x02\x0f"\x08/v1/tags:\x03tag\x12u\n\x06GetTag\x12&.exabel.api.analytics.v1.GetTagRequest\x1a\x1c.exabel.api.analytics.v1.Tag"%\x92A\t\x12\x07Get tag\x82\xd3\xe4\x93\x02\x13\x12\x11/v1/{name=tags/*}\x12\x87\x01\n\tUpdateTag\x12).exabel.api.analytics.v1.UpdateTagRequest\x1a\x1c.exabel.api.analytics.v1.Tag"1\x92A\x0c\x12\nUpdate tag\x82\xd3\xe4\x93\x02\x1c2\x15/v1/{tag.name=tags/*}:\x03tag\x12x\n\tDeleteTag\x12).exabel.api.analytics.v1.DeleteTagRequest\x1a\x16.google.protobuf.Empty"(\x92A\x0c\x12\nDelete tag\x82\xd3\xe4\x93\x02\x13*\x11/v1/{name=tags/*}\x12\x7f\n\x08ListTags\x12(.exabel.api.analytics.v1.ListTagsRequest\x1a).exabel.api.analytics.v1.ListTagsResponse"\x1e\x92A\x0b\x12\tList tags\x82\xd3\xe4\x93\x02\n\x12\x08/v1/tags\x12\xaa\x01\n\x0bAddEntities\x12+.exabel.api.analytics.v1.AddEntitiesRequest\x1a,.exabel.api.analytics.v1.AddEntitiesResponse"@\x92A\x15\x12\x13Add entities to tag\x82\xd3\xe4\x93\x02""\x1d/v1/{name=tags/*}:addEntities:\x01*\x12\xbb\x01\n\x0eRemoveEntities\x12..exabel.api.analytics.v1.RemoveEntitiesRequest\x1a/.exabel.api.analytics.v1.RemoveEntitiesResponse"H\x92A\x1a\x12\x18Remove entities from tag\x82\xd3\xe4\x93\x02%" /v1/{name=tags/*}:removeEntities:\x01*\x12\xb3\x01\n\x0fListTagEntities\x12/.exabel.api.analytics.v1.ListTagEntitiesRequest\x1a0.exabel.api.analytics.v1.ListTagEntitiesResponse"=\x92A\x16\x12\x14List entities in tag\x82\xd3\xe4\x93\x02\x1e\x12\x1c/v1/{parent=tags/*}/entitiesBM\n\x1bcom.exabel.api.analytics.v1B\x0fTagServiceProtoP\x01Z\x1bexabel.com/api/analytics/v1b\x06proto3')
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.analytics.v1.tag_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b'\n\x1bcom.exabel.api.analytics.v1B\x0fTagServiceProtoP\x01Z\x1bexabel.com/api/analytics/v1'
     _CREATETAGREQUEST.fields_by_name['tag']._options = None
-    _CREATETAGREQUEST.fields_by_name['tag']._serialized_options = b'\xe0A\x02'
+    _CREATETAGREQUEST.fields_by_name['tag']._serialized_options = b'\xe2A\x01\x02'
     _GETTAGREQUEST.fields_by_name['name']._options = None
-    _GETTAGREQUEST.fields_by_name['name']._serialized_options = b'\xe0A\x02\x92A\r\xca>\n\xfa\x02\x07tagName'
+    _GETTAGREQUEST.fields_by_name['name']._serialized_options = b'\x92A\r\xca>\n\xfa\x02\x07tagName\xe2A\x01\x02'
     _UPDATETAGREQUEST.fields_by_name['tag']._options = None
-    _UPDATETAGREQUEST.fields_by_name['tag']._serialized_options = b'\xe0A\x02'
+    _UPDATETAGREQUEST.fields_by_name['tag']._serialized_options = b'\xe2A\x01\x02'
     _DELETETAGREQUEST.fields_by_name['name']._options = None
-    _DELETETAGREQUEST.fields_by_name['name']._serialized_options = b'\xe0A\x02\x92A\r\xca>\n\xfa\x02\x07tagName'
+    _DELETETAGREQUEST.fields_by_name['name']._serialized_options = b'\x92A\r\xca>\n\xfa\x02\x07tagName\xe2A\x01\x02'
     _ADDENTITIESREQUEST.fields_by_name['name']._options = None
-    _ADDENTITIESREQUEST.fields_by_name['name']._serialized_options = b'\xe0A\x02\x92A\r\xca>\n\xfa\x02\x07tagName'
+    _ADDENTITIESREQUEST.fields_by_name['name']._serialized_options = b'\x92A\r\xca>\n\xfa\x02\x07tagName\xe2A\x01\x02'
     _REMOVEENTITIESREQUEST.fields_by_name['name']._options = None
-    _REMOVEENTITIESREQUEST.fields_by_name['name']._serialized_options = b'\xe0A\x02\x92A\r\xca>\n\xfa\x02\x07tagName'
+    _REMOVEENTITIESREQUEST.fields_by_name['name']._serialized_options = b'\x92A\r\xca>\n\xfa\x02\x07tagName\xe2A\x01\x02'
     _LISTTAGENTITIESREQUEST.fields_by_name['parent']._options = None
-    _LISTTAGENTITIESREQUEST.fields_by_name['parent']._serialized_options = b'\xe0A\x02\x92A\r\xca>\n\xfa\x02\x07tagName'
+    _LISTTAGENTITIESREQUEST.fields_by_name['parent']._serialized_options = b'\x92A\r\xca>\n\xfa\x02\x07tagName\xe2A\x01\x02'
     _TAGSERVICE.methods_by_name['CreateTag']._options = None
-    _TAGSERVICE.methods_by_name['CreateTag']._serialized_options = b'\x82\xd3\xe4\x93\x02\x0f"\x08/v1/tags:\x03tag\x92A\x0c\x12\nCreate tag'
+    _TAGSERVICE.methods_by_name['CreateTag']._serialized_options = b'\x92A\x0c\x12\nCreate tag\x82\xd3\xe4\x93\x02\x0f"\x08/v1/tags:\x03tag'
     _TAGSERVICE.methods_by_name['GetTag']._options = None
-    _TAGSERVICE.methods_by_name['GetTag']._serialized_options = b'\x82\xd3\xe4\x93\x02\x13\x12\x11/v1/{name=tags/*}\x92A\t\x12\x07Get tag'
+    _TAGSERVICE.methods_by_name['GetTag']._serialized_options = b'\x92A\t\x12\x07Get tag\x82\xd3\xe4\x93\x02\x13\x12\x11/v1/{name=tags/*}'
     _TAGSERVICE.methods_by_name['UpdateTag']._options = None
-    _TAGSERVICE.methods_by_name['UpdateTag']._serialized_options = b'\x82\xd3\xe4\x93\x02\x1c2\x15/v1/{tag.name=tags/*}:\x03tag\x92A\x0c\x12\nUpdate tag'
+    _TAGSERVICE.methods_by_name['UpdateTag']._serialized_options = b'\x92A\x0c\x12\nUpdate tag\x82\xd3\xe4\x93\x02\x1c2\x15/v1/{tag.name=tags/*}:\x03tag'
     _TAGSERVICE.methods_by_name['DeleteTag']._options = None
-    _TAGSERVICE.methods_by_name['DeleteTag']._serialized_options = b'\x82\xd3\xe4\x93\x02\x13*\x11/v1/{name=tags/*}\x92A\x0c\x12\nDelete tag'
+    _TAGSERVICE.methods_by_name['DeleteTag']._serialized_options = b'\x92A\x0c\x12\nDelete tag\x82\xd3\xe4\x93\x02\x13*\x11/v1/{name=tags/*}'
     _TAGSERVICE.methods_by_name['ListTags']._options = None
-    _TAGSERVICE.methods_by_name['ListTags']._serialized_options = b'\x82\xd3\xe4\x93\x02\n\x12\x08/v1/tags\x92A\x0b\x12\tList tags'
+    _TAGSERVICE.methods_by_name['ListTags']._serialized_options = b'\x92A\x0b\x12\tList tags\x82\xd3\xe4\x93\x02\n\x12\x08/v1/tags'
     _TAGSERVICE.methods_by_name['AddEntities']._options = None
-    _TAGSERVICE.methods_by_name['AddEntities']._serialized_options = b'\x82\xd3\xe4\x93\x02""\x1d/v1/{name=tags/*}:addEntities:\x01*\x92A\x15\x12\x13Add entities to tag'
+    _TAGSERVICE.methods_by_name['AddEntities']._serialized_options = b'\x92A\x15\x12\x13Add entities to tag\x82\xd3\xe4\x93\x02""\x1d/v1/{name=tags/*}:addEntities:\x01*'
     _TAGSERVICE.methods_by_name['RemoveEntities']._options = None
-    _TAGSERVICE.methods_by_name['RemoveEntities']._serialized_options = b'\x82\xd3\xe4\x93\x02%" /v1/{name=tags/*}:removeEntities:\x01*\x92A\x1a\x12\x18Remove entities from tag'
+    _TAGSERVICE.methods_by_name['RemoveEntities']._serialized_options = b'\x92A\x1a\x12\x18Remove entities from tag\x82\xd3\xe4\x93\x02%" /v1/{name=tags/*}:removeEntities:\x01*'
     _TAGSERVICE.methods_by_name['ListTagEntities']._options = None
-    _TAGSERVICE.methods_by_name['ListTagEntities']._serialized_options = b'\x82\xd3\xe4\x93\x02\x1e\x12\x1c/v1/{parent=tags/*}/entities\x92A\x16\x12\x14List entities in tag'
-    _CREATETAGREQUEST._serialized_start = 288
-    _CREATETAGREQUEST._serialized_end = 370
-    _GETTAGREQUEST._serialized_start = 372
-    _GETTAGREQUEST._serialized_end = 422
-    _UPDATETAGREQUEST._serialized_start = 424
-    _UPDATETAGREQUEST._serialized_end = 539
-    _DELETETAGREQUEST._serialized_start = 541
-    _DELETETAGREQUEST._serialized_end = 594
-    _LISTTAGSREQUEST._serialized_start = 596
-    _LISTTAGSREQUEST._serialized_end = 652
-    _LISTTAGSRESPONSE._serialized_start = 654
-    _LISTTAGSRESPONSE._serialized_end = 761
-    _ADDENTITIESREQUEST._serialized_start = 763
-    _ADDENTITIESREQUEST._serialized_end = 840
-    _ADDENTITIESRESPONSE._serialized_start = 842
-    _ADDENTITIESRESPONSE._serialized_end = 863
-    _REMOVEENTITIESREQUEST._serialized_start = 865
-    _REMOVEENTITIESREQUEST._serialized_end = 945
-    _REMOVEENTITIESRESPONSE._serialized_start = 947
-    _REMOVEENTITIESRESPONSE._serialized_end = 971
-    _LISTTAGENTITIESREQUEST._serialized_start = 973
-    _LISTTAGENTITIESREQUEST._serialized_end = 1073
-    _LISTTAGENTITIESRESPONSE._serialized_start = 1075
-    _LISTTAGENTITIESRESPONSE._serialized_end = 1167
-    _TAGSERVICE._serialized_start = 1170
-    _TAGSERVICE._serialized_end = 2359
+    _TAGSERVICE.methods_by_name['ListTagEntities']._serialized_options = b'\x92A\x16\x12\x14List entities in tag\x82\xd3\xe4\x93\x02\x1e\x12\x1c/v1/{parent=tags/*}/entities'
+    _globals['_CREATETAGREQUEST']._serialized_start = 288
+    _globals['_CREATETAGREQUEST']._serialized_end = 371
+    _globals['_GETTAGREQUEST']._serialized_start = 373
+    _globals['_GETTAGREQUEST']._serialized_end = 424
+    _globals['_UPDATETAGREQUEST']._serialized_start = 426
+    _globals['_UPDATETAGREQUEST']._serialized_end = 542
+    _globals['_DELETETAGREQUEST']._serialized_start = 544
+    _globals['_DELETETAGREQUEST']._serialized_end = 598
+    _globals['_LISTTAGSREQUEST']._serialized_start = 600
+    _globals['_LISTTAGSREQUEST']._serialized_end = 656
+    _globals['_LISTTAGSRESPONSE']._serialized_start = 658
+    _globals['_LISTTAGSRESPONSE']._serialized_end = 765
+    _globals['_ADDENTITIESREQUEST']._serialized_start = 767
+    _globals['_ADDENTITIESREQUEST']._serialized_end = 845
+    _globals['_ADDENTITIESRESPONSE']._serialized_start = 847
+    _globals['_ADDENTITIESRESPONSE']._serialized_end = 868
+    _globals['_REMOVEENTITIESREQUEST']._serialized_start = 870
+    _globals['_REMOVEENTITIESREQUEST']._serialized_end = 951
+    _globals['_REMOVEENTITIESRESPONSE']._serialized_start = 953
+    _globals['_REMOVEENTITIESRESPONSE']._serialized_end = 977
+    _globals['_LISTTAGENTITIESREQUEST']._serialized_start = 979
+    _globals['_LISTTAGENTITIESREQUEST']._serialized_end = 1080
+    _globals['_LISTTAGENTITIESRESPONSE']._serialized_start = 1082
+    _globals['_LISTTAGENTITIESRESPONSE']._serialized_end = 1174
+    _globals['_TAGSERVICE']._serialized_start = 1177
+    _globals['_TAGSERVICE']._serialized_end = 2366
```

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_service_pb2_grpc.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/data/v1/all_pb2.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/data/v1/all_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/data/v1/all_pb2_grpc.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/data/v1/all_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_messages_pb2.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_messages_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 _sym_db = _symbol_database.Default()
 from google.api import field_behavior_pb2 as google_dot_api_dot_field__behavior__pb2
 from .....protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n*exabel/api/data/v1/data_set_messages.proto\x12\x12exabel.api.data.v1\x1a\x1fgoogle/api/field_behavior.proto\x1a.protoc_gen_openapiv2/options/annotations.proto"\xa0\x02\n\x07DataSet\x12>\n\x04name\x18\x01 \x01(\tB0\xe0A\x05\xe0A\x02\x92A\'J\x14"dataSets/ns.stores"\xca>\x0e\xfa\x02\x0bdataSetName\x12#\n\x0cdisplay_name\x18\x02 \x01(\tB\r\x92A\nJ\x08"Stores"\x12>\n\x0bdescription\x18\x03 \x01(\tB)\x92A&J$"The data set of all store entities"\x12N\n\x07signals\x18\x04 \x03(\tB=\xe0A\x06\x92A7J5["signals/ns.customer_amount", "signals/ns.visitors"]\x12 \n\tread_only\x18\x05 \x01(\x08B\r\xe0A\x03\x92A\x07J\x05falseBH\n\x16com.exabel.api.data.v1B\x14DataSetMessagesProtoP\x01Z\x16exabel.com/api/data/v1b\x06proto3')
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.data.v1.data_set_messages_pb2', globals())
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n*exabel/api/data/v1/data_set_messages.proto\x12\x12exabel.api.data.v1\x1a\x1fgoogle/api/field_behavior.proto\x1a.protoc_gen_openapiv2/options/annotations.proto"\xa1\x02\n\x07DataSet\x12=\n\x04name\x18\x01 \x01(\tB/\x92A\'J\x14"dataSets/ns.stores"\xca>\x0e\xfa\x02\x0bdataSetName\xe2A\x02\x05\x02\x12#\n\x0cdisplay_name\x18\x02 \x01(\tB\r\x92A\nJ\x08"Stores"\x12>\n\x0bdescription\x18\x03 \x01(\tB)\x92A&J$"The data set of all store entities"\x12O\n\x07signals\x18\x04 \x03(\tB>\x92A7J5["signals/ns.customer_amount", "signals/ns.visitors"]\xe2A\x01\x06\x12!\n\tread_only\x18\x05 \x01(\x08B\x0e\x92A\x07J\x05false\xe2A\x01\x03BH\n\x16com.exabel.api.data.v1B\x14DataSetMessagesProtoP\x01Z\x16exabel.com/api/data/v1b\x06proto3')
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.data.v1.data_set_messages_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b'\n\x16com.exabel.api.data.v1B\x14DataSetMessagesProtoP\x01Z\x16exabel.com/api/data/v1'
     _DATASET.fields_by_name['name']._options = None
-    _DATASET.fields_by_name['name']._serialized_options = b'\xe0A\x05\xe0A\x02\x92A\'J\x14"dataSets/ns.stores"\xca>\x0e\xfa\x02\x0bdataSetName'
+    _DATASET.fields_by_name['name']._serialized_options = b'\x92A\'J\x14"dataSets/ns.stores"\xca>\x0e\xfa\x02\x0bdataSetName\xe2A\x02\x05\x02'
     _DATASET.fields_by_name['display_name']._options = None
     _DATASET.fields_by_name['display_name']._serialized_options = b'\x92A\nJ\x08"Stores"'
     _DATASET.fields_by_name['description']._options = None
     _DATASET.fields_by_name['description']._serialized_options = b'\x92A&J$"The data set of all store entities"'
     _DATASET.fields_by_name['signals']._options = None
-    _DATASET.fields_by_name['signals']._serialized_options = b'\xe0A\x06\x92A7J5["signals/ns.customer_amount", "signals/ns.visitors"]'
+    _DATASET.fields_by_name['signals']._serialized_options = b'\x92A7J5["signals/ns.customer_amount", "signals/ns.visitors"]\xe2A\x01\x06'
     _DATASET.fields_by_name['read_only']._options = None
-    _DATASET.fields_by_name['read_only']._serialized_options = b'\xe0A\x03\x92A\x07J\x05false'
-    _DATASET._serialized_start = 148
-    _DATASET._serialized_end = 436
+    _DATASET.fields_by_name['read_only']._serialized_options = b'\x92A\x07J\x05false\xe2A\x01\x03'
+    _globals['_DATASET']._serialized_start = 148
+    _globals['_DATASET']._serialized_end = 437
```

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_service_pb2.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_service_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,50 +1,51 @@
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 _sym_db = _symbol_database.Default()
 from .....exabel.api.data.v1 import data_set_messages_pb2 as exabel_dot_api_dot_data_dot_v1_dot_data__set__messages__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from google.api import field_behavior_pb2 as google_dot_api_dot_field__behavior__pb2
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 from google.protobuf import field_mask_pb2 as google_dot_protobuf_dot_field__mask__pb2
 from .....protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n)exabel/api/data/v1/data_set_service.proto\x12\x12exabel.api.data.v1\x1a*exabel/api/data/v1/data_set_messages.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1fgoogle/api/field_behavior.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a google/protobuf/field_mask.proto\x1a.protoc_gen_openapiv2/options/annotations.proto"\x15\n\x13ListDataSetsRequest"F\n\x14ListDataSetsResponse\x12.\n\tdata_sets\x18\x01 \x03(\x0b2\x1b.exabel.api.data.v1.DataSet":\n\x11GetDataSetRequest\x12%\n\x04name\x18\x01 \x01(\tB\x17\xe0A\x02\x92A\x11\xca>\x0e\xfa\x02\x0bdataSetName"J\n\x14CreateDataSetRequest\x122\n\x08data_set\x18\x01 \x01(\x0b2\x1b.exabel.api.data.v1.DataSetB\x03\xe0A\x02"\x92\x01\n\x14UpdateDataSetRequest\x122\n\x08data_set\x18\x01 \x01(\x0b2\x1b.exabel.api.data.v1.DataSetB\x03\xe0A\x02\x12/\n\x0bupdate_mask\x18\x02 \x01(\x0b2\x1a.google.protobuf.FieldMask\x12\x15\n\rallow_missing\x18\x03 \x01(\x08"=\n\x14DeleteDataSetRequest\x12%\n\x04name\x18\x01 \x01(\tB\x17\xe0A\x02\x92A\x11\xca>\x0e\xfa\x02\x0bdataSetName2\xd3\x05\n\x0eDataSetService\x12\x8a\x01\n\x0cListDataSets\x12\'.exabel.api.data.v1.ListDataSetsRequest\x1a(.exabel.api.data.v1.ListDataSetsResponse"\'\x82\xd3\xe4\x93\x02\x0e\x12\x0c/v1/dataSets\x92A\x10\x12\x0eList data sets\x12\x80\x01\n\nGetDataSet\x12%.exabel.api.data.v1.GetDataSetRequest\x1a\x1b.exabel.api.data.v1.DataSet".\x82\xd3\xe4\x93\x02\x17\x12\x15/v1/{name=dataSets/*}\x92A\x0e\x12\x0cGet data set\x12\x8a\x01\n\rCreateDataSet\x12(.exabel.api.data.v1.CreateDataSetRequest\x1a\x1b.exabel.api.data.v1.DataSet"2\x82\xd3\xe4\x93\x02\x18"\x0c/v1/dataSets:\x08data_set\x92A\x11\x12\x0fCreate data set\x12\x9c\x01\n\rUpdateDataSet\x12(.exabel.api.data.v1.UpdateDataSetRequest\x1a\x1b.exabel.api.data.v1.DataSet"D\x82\xd3\xe4\x93\x02*2\x1e/v1/{data_set.name=dataSets/*}:\x08data_set\x92A\x11\x12\x0fUpdate data set\x12\x84\x01\n\rDeleteDataSet\x12(.exabel.api.data.v1.DeleteDataSetRequest\x1a\x16.google.protobuf.Empty"1\x82\xd3\xe4\x93\x02\x17*\x15/v1/{name=dataSets/*}\x92A\x11\x12\x0fDelete data setBG\n\x16com.exabel.api.data.v1B\x13DataSetServiceProtoP\x01Z\x16exabel.com/api/data/v1b\x06proto3')
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.data.v1.data_set_service_pb2', globals())
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n)exabel/api/data/v1/data_set_service.proto\x12\x12exabel.api.data.v1\x1a*exabel/api/data/v1/data_set_messages.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1fgoogle/api/field_behavior.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a google/protobuf/field_mask.proto\x1a.protoc_gen_openapiv2/options/annotations.proto"\x15\n\x13ListDataSetsRequest"F\n\x14ListDataSetsResponse\x12.\n\tdata_sets\x18\x01 \x03(\x0b2\x1b.exabel.api.data.v1.DataSet";\n\x11GetDataSetRequest\x12&\n\x04name\x18\x01 \x01(\tB\x18\x92A\x11\xca>\x0e\xfa\x02\x0bdataSetName\xe2A\x01\x02"K\n\x14CreateDataSetRequest\x123\n\x08data_set\x18\x01 \x01(\x0b2\x1b.exabel.api.data.v1.DataSetB\x04\xe2A\x01\x02"\x93\x01\n\x14UpdateDataSetRequest\x123\n\x08data_set\x18\x01 \x01(\x0b2\x1b.exabel.api.data.v1.DataSetB\x04\xe2A\x01\x02\x12/\n\x0bupdate_mask\x18\x02 \x01(\x0b2\x1a.google.protobuf.FieldMask\x12\x15\n\rallow_missing\x18\x03 \x01(\x08">\n\x14DeleteDataSetRequest\x12&\n\x04name\x18\x01 \x01(\tB\x18\x92A\x11\xca>\x0e\xfa\x02\x0bdataSetName\xe2A\x01\x022\xd3\x05\n\x0eDataSetService\x12\x8a\x01\n\x0cListDataSets\x12\'.exabel.api.data.v1.ListDataSetsRequest\x1a(.exabel.api.data.v1.ListDataSetsResponse"\'\x92A\x10\x12\x0eList data sets\x82\xd3\xe4\x93\x02\x0e\x12\x0c/v1/dataSets\x12\x80\x01\n\nGetDataSet\x12%.exabel.api.data.v1.GetDataSetRequest\x1a\x1b.exabel.api.data.v1.DataSet".\x92A\x0e\x12\x0cGet data set\x82\xd3\xe4\x93\x02\x17\x12\x15/v1/{name=dataSets/*}\x12\x8a\x01\n\rCreateDataSet\x12(.exabel.api.data.v1.CreateDataSetRequest\x1a\x1b.exabel.api.data.v1.DataSet"2\x92A\x11\x12\x0fCreate data set\x82\xd3\xe4\x93\x02\x18"\x0c/v1/dataSets:\x08data_set\x12\x9c\x01\n\rUpdateDataSet\x12(.exabel.api.data.v1.UpdateDataSetRequest\x1a\x1b.exabel.api.data.v1.DataSet"D\x92A\x11\x12\x0fUpdate data set\x82\xd3\xe4\x93\x02*2\x1e/v1/{data_set.name=dataSets/*}:\x08data_set\x12\x84\x01\n\rDeleteDataSet\x12(.exabel.api.data.v1.DeleteDataSetRequest\x1a\x16.google.protobuf.Empty"1\x92A\x11\x12\x0fDelete data set\x82\xd3\xe4\x93\x02\x17*\x15/v1/{name=dataSets/*}BG\n\x16com.exabel.api.data.v1B\x13DataSetServiceProtoP\x01Z\x16exabel.com/api/data/v1b\x06proto3')
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.data.v1.data_set_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b'\n\x16com.exabel.api.data.v1B\x13DataSetServiceProtoP\x01Z\x16exabel.com/api/data/v1'
     _GETDATASETREQUEST.fields_by_name['name']._options = None
-    _GETDATASETREQUEST.fields_by_name['name']._serialized_options = b'\xe0A\x02\x92A\x11\xca>\x0e\xfa\x02\x0bdataSetName'
+    _GETDATASETREQUEST.fields_by_name['name']._serialized_options = b'\x92A\x11\xca>\x0e\xfa\x02\x0bdataSetName\xe2A\x01\x02'
     _CREATEDATASETREQUEST.fields_by_name['data_set']._options = None
-    _CREATEDATASETREQUEST.fields_by_name['data_set']._serialized_options = b'\xe0A\x02'
+    _CREATEDATASETREQUEST.fields_by_name['data_set']._serialized_options = b'\xe2A\x01\x02'
     _UPDATEDATASETREQUEST.fields_by_name['data_set']._options = None
-    _UPDATEDATASETREQUEST.fields_by_name['data_set']._serialized_options = b'\xe0A\x02'
+    _UPDATEDATASETREQUEST.fields_by_name['data_set']._serialized_options = b'\xe2A\x01\x02'
     _DELETEDATASETREQUEST.fields_by_name['name']._options = None
-    _DELETEDATASETREQUEST.fields_by_name['name']._serialized_options = b'\xe0A\x02\x92A\x11\xca>\x0e\xfa\x02\x0bdataSetName'
+    _DELETEDATASETREQUEST.fields_by_name['name']._serialized_options = b'\x92A\x11\xca>\x0e\xfa\x02\x0bdataSetName\xe2A\x01\x02'
     _DATASETSERVICE.methods_by_name['ListDataSets']._options = None
-    _DATASETSERVICE.methods_by_name['ListDataSets']._serialized_options = b'\x82\xd3\xe4\x93\x02\x0e\x12\x0c/v1/dataSets\x92A\x10\x12\x0eList data sets'
+    _DATASETSERVICE.methods_by_name['ListDataSets']._serialized_options = b'\x92A\x10\x12\x0eList data sets\x82\xd3\xe4\x93\x02\x0e\x12\x0c/v1/dataSets'
     _DATASETSERVICE.methods_by_name['GetDataSet']._options = None
-    _DATASETSERVICE.methods_by_name['GetDataSet']._serialized_options = b'\x82\xd3\xe4\x93\x02\x17\x12\x15/v1/{name=dataSets/*}\x92A\x0e\x12\x0cGet data set'
+    _DATASETSERVICE.methods_by_name['GetDataSet']._serialized_options = b'\x92A\x0e\x12\x0cGet data set\x82\xd3\xe4\x93\x02\x17\x12\x15/v1/{name=dataSets/*}'
     _DATASETSERVICE.methods_by_name['CreateDataSet']._options = None
-    _DATASETSERVICE.methods_by_name['CreateDataSet']._serialized_options = b'\x82\xd3\xe4\x93\x02\x18"\x0c/v1/dataSets:\x08data_set\x92A\x11\x12\x0fCreate data set'
+    _DATASETSERVICE.methods_by_name['CreateDataSet']._serialized_options = b'\x92A\x11\x12\x0fCreate data set\x82\xd3\xe4\x93\x02\x18"\x0c/v1/dataSets:\x08data_set'
     _DATASETSERVICE.methods_by_name['UpdateDataSet']._options = None
-    _DATASETSERVICE.methods_by_name['UpdateDataSet']._serialized_options = b'\x82\xd3\xe4\x93\x02*2\x1e/v1/{data_set.name=dataSets/*}:\x08data_set\x92A\x11\x12\x0fUpdate data set'
+    _DATASETSERVICE.methods_by_name['UpdateDataSet']._serialized_options = b'\x92A\x11\x12\x0fUpdate data set\x82\xd3\xe4\x93\x02*2\x1e/v1/{data_set.name=dataSets/*}:\x08data_set'
     _DATASETSERVICE.methods_by_name['DeleteDataSet']._options = None
-    _DATASETSERVICE.methods_by_name['DeleteDataSet']._serialized_options = b'\x82\xd3\xe4\x93\x02\x17*\x15/v1/{name=dataSets/*}\x92A\x11\x12\x0fDelete data set'
-    _LISTDATASETSREQUEST._serialized_start = 283
-    _LISTDATASETSREQUEST._serialized_end = 304
-    _LISTDATASETSRESPONSE._serialized_start = 306
-    _LISTDATASETSRESPONSE._serialized_end = 376
-    _GETDATASETREQUEST._serialized_start = 378
-    _GETDATASETREQUEST._serialized_end = 436
-    _CREATEDATASETREQUEST._serialized_start = 438
-    _CREATEDATASETREQUEST._serialized_end = 512
-    _UPDATEDATASETREQUEST._serialized_start = 515
-    _UPDATEDATASETREQUEST._serialized_end = 661
-    _DELETEDATASETREQUEST._serialized_start = 663
-    _DELETEDATASETREQUEST._serialized_end = 724
-    _DATASETSERVICE._serialized_start = 727
-    _DATASETSERVICE._serialized_end = 1450
+    _DATASETSERVICE.methods_by_name['DeleteDataSet']._serialized_options = b'\x92A\x11\x12\x0fDelete data set\x82\xd3\xe4\x93\x02\x17*\x15/v1/{name=dataSets/*}'
+    _globals['_LISTDATASETSREQUEST']._serialized_start = 283
+    _globals['_LISTDATASETSREQUEST']._serialized_end = 304
+    _globals['_LISTDATASETSRESPONSE']._serialized_start = 306
+    _globals['_LISTDATASETSRESPONSE']._serialized_end = 376
+    _globals['_GETDATASETREQUEST']._serialized_start = 378
+    _globals['_GETDATASETREQUEST']._serialized_end = 437
+    _globals['_CREATEDATASETREQUEST']._serialized_start = 439
+    _globals['_CREATEDATASETREQUEST']._serialized_end = 514
+    _globals['_UPDATEDATASETREQUEST']._serialized_start = 517
+    _globals['_UPDATEDATASETREQUEST']._serialized_end = 664
+    _globals['_DELETEDATASETREQUEST']._serialized_start = 666
+    _globals['_DELETEDATASETREQUEST']._serialized_end = 728
+    _globals['_DATASETSERVICE']._serialized_start = 731
+    _globals['_DATASETSERVICE']._serialized_end = 1454
```

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_service_pb2_grpc.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_messages_pb2.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_messages_pb2.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 _sym_db = _symbol_database.Default()
 from google.api import field_behavior_pb2 as google_dot_api_dot_field__behavior__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from .....protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(exabel/api/data/v1/entity_messages.proto\x12\x12exabel.api.data.v1\x1a\x1fgoogle/api/field_behavior.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a.protoc_gen_openapiv2/options/annotations.proto"\xe2\x01\n\nEntityType\x12B\n\x04name\x18\x01 \x01(\tB4\xe0A\x05\xe0A\x02\x92A+J\x15"entityTypes/company"\xca>\x11\xfa\x02\x0eentityTypeName\x12&\n\x0cdisplay_name\x18\x02 \x01(\tB\x10\x92A\rJ\x0b"Companies"\x12,\n\x0bdescription\x18\x03 \x01(\tB\x17\x92A\x14J\x12"Public companies"\x12\x16\n\tread_only\x18\x04 \x01(\x08B\x03\xe0A\x03\x12"\n\x0eis_associative\x18\x05 \x01(\x08B\n\x92A\x07J\x05false"\xf7\x01\n\x06Entity\x12@\n\x04name\x18\x01 \x01(\tB2\xe0A\x05\xe0A\x02\x92A)J\x17"entities/ns.my_entity"\xca>\r\xfa\x02\nentityName\x12&\n\x0cdisplay_name\x18\x02 \x01(\tB\x10\x92A\rJ\x0b"My Entity"\x12>\n\x0bdescription\x18\x03 \x01(\tB)\x92A&J$"This is a description of My Entity"\x12\x16\n\tread_only\x18\x04 \x01(\x08B\x03\xe0A\x03\x12+\n\nproperties\x18d \x01(\x0b2\x17.google.protobuf.StructBG\n\x16com.exabel.api.data.v1B\x13EntityMessagesProtoP\x01Z\x16exabel.com/api/data/v1b\x06proto3')
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.data.v1.entity_messages_pb2', globals())
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(exabel/api/data/v1/entity_messages.proto\x12\x12exabel.api.data.v1\x1a\x1fgoogle/api/field_behavior.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a.protoc_gen_openapiv2/options/annotations.proto"\xe2\x01\n\nEntityType\x12A\n\x04name\x18\x01 \x01(\tB3\x92A+J\x15"entityTypes/company"\xca>\x11\xfa\x02\x0eentityTypeName\xe2A\x02\x05\x02\x12&\n\x0cdisplay_name\x18\x02 \x01(\tB\x10\x92A\rJ\x0b"Companies"\x12,\n\x0bdescription\x18\x03 \x01(\tB\x17\x92A\x14J\x12"Public companies"\x12\x17\n\tread_only\x18\x04 \x01(\x08B\x04\xe2A\x01\x03\x12"\n\x0eis_associative\x18\x05 \x01(\x08B\n\x92A\x07J\x05false"\xf7\x01\n\x06Entity\x12?\n\x04name\x18\x01 \x01(\tB1\x92A)J\x17"entities/ns.my_entity"\xca>\r\xfa\x02\nentityName\xe2A\x02\x05\x02\x12&\n\x0cdisplay_name\x18\x02 \x01(\tB\x10\x92A\rJ\x0b"My Entity"\x12>\n\x0bdescription\x18\x03 \x01(\tB)\x92A&J$"This is a description of My Entity"\x12\x17\n\tread_only\x18\x04 \x01(\x08B\x04\xe2A\x01\x03\x12+\n\nproperties\x18d \x01(\x0b2\x17.google.protobuf.StructBG\n\x16com.exabel.api.data.v1B\x13EntityMessagesProtoP\x01Z\x16exabel.com/api/data/v1b\x06proto3')
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.data.v1.entity_messages_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b'\n\x16com.exabel.api.data.v1B\x13EntityMessagesProtoP\x01Z\x16exabel.com/api/data/v1'
     _ENTITYTYPE.fields_by_name['name']._options = None
-    _ENTITYTYPE.fields_by_name['name']._serialized_options = b'\xe0A\x05\xe0A\x02\x92A+J\x15"entityTypes/company"\xca>\x11\xfa\x02\x0eentityTypeName'
+    _ENTITYTYPE.fields_by_name['name']._serialized_options = b'\x92A+J\x15"entityTypes/company"\xca>\x11\xfa\x02\x0eentityTypeName\xe2A\x02\x05\x02'
     _ENTITYTYPE.fields_by_name['display_name']._options = None
     _ENTITYTYPE.fields_by_name['display_name']._serialized_options = b'\x92A\rJ\x0b"Companies"'
     _ENTITYTYPE.fields_by_name['description']._options = None
     _ENTITYTYPE.fields_by_name['description']._serialized_options = b'\x92A\x14J\x12"Public companies"'
     _ENTITYTYPE.fields_by_name['read_only']._options = None
-    _ENTITYTYPE.fields_by_name['read_only']._serialized_options = b'\xe0A\x03'
+    _ENTITYTYPE.fields_by_name['read_only']._serialized_options = b'\xe2A\x01\x03'
     _ENTITYTYPE.fields_by_name['is_associative']._options = None
     _ENTITYTYPE.fields_by_name['is_associative']._serialized_options = b'\x92A\x07J\x05false'
     _ENTITY.fields_by_name['name']._options = None
-    _ENTITY.fields_by_name['name']._serialized_options = b'\xe0A\x05\xe0A\x02\x92A)J\x17"entities/ns.my_entity"\xca>\r\xfa\x02\nentityName'
+    _ENTITY.fields_by_name['name']._serialized_options = b'\x92A)J\x17"entities/ns.my_entity"\xca>\r\xfa\x02\nentityName\xe2A\x02\x05\x02'
     _ENTITY.fields_by_name['display_name']._options = None
     _ENTITY.fields_by_name['display_name']._serialized_options = b'\x92A\rJ\x0b"My Entity"'
     _ENTITY.fields_by_name['description']._options = None
     _ENTITY.fields_by_name['description']._serialized_options = b'\x92A&J$"This is a description of My Entity"'
     _ENTITY.fields_by_name['read_only']._options = None
-    _ENTITY.fields_by_name['read_only']._serialized_options = b'\xe0A\x03'
-    _ENTITYTYPE._serialized_start = 176
-    _ENTITYTYPE._serialized_end = 402
-    _ENTITY._serialized_start = 405
-    _ENTITY._serialized_end = 652
+    _ENTITY.fields_by_name['read_only']._serialized_options = b'\xe2A\x01\x03'
+    _globals['_ENTITYTYPE']._serialized_start = 176
+    _globals['_ENTITYTYPE']._serialized_end = 402
+    _globals['_ENTITY']._serialized_start = 405
+    _globals['_ENTITY']._serialized_end = 652
```

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_service_pb2.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_service_pb2.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,103 +1,104 @@
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 _sym_db = _symbol_database.Default()
 from .....exabel.api.data.v1 import entity_messages_pb2 as exabel_dot_api_dot_data_dot_v1_dot_entity__messages__pb2
 from .....exabel.api.data.v1 import search_messages_pb2 as exabel_dot_api_dot_data_dot_v1_dot_search__messages__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from google.api import field_behavior_pb2 as google_dot_api_dot_field__behavior__pb2
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 from google.protobuf import field_mask_pb2 as google_dot_protobuf_dot_field__mask__pb2
 from .....protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\'exabel/api/data/v1/entity_service.proto\x12\x12exabel.api.data.v1\x1a(exabel/api/data/v1/entity_messages.proto\x1a(exabel/api/data/v1/search_messages.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1fgoogle/api/field_behavior.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a google/protobuf/field_mask.proto\x1a.protoc_gen_openapiv2/options/annotations.proto"?\n\x16ListEntityTypesRequest\x12\x11\n\tpage_size\x18\x01 \x01(\x05\x12\x12\n\npage_token\x18\x02 \x01(\t"|\n\x17ListEntityTypesResponse\x124\n\x0centity_types\x18\x01 \x03(\x0b2\x1e.exabel.api.data.v1.EntityType\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\x12\x12\n\ntotal_size\x18\x03 \x01(\x05"@\n\x14GetEntityTypeRequest\x12(\n\x04name\x18\x01 \x01(\tB\x1a\xe0A\x02\x92A\x14\xca>\x11\xfa\x02\x0eentityTypeName"j\n\x17CreateEntityTypeRequest\x12O\n\x0bentity_type\x18\x01 \x01(\x0b2\x1e.exabel.api.data.v1.EntityTypeB\x1a\xe0A\x02\x92A\x14\xca>\x11\xfa\x02\x0eentityTypeName"\xb2\x01\n\x17UpdateEntityTypeRequest\x12O\n\x0bentity_type\x18\x01 \x01(\x0b2\x1e.exabel.api.data.v1.EntityTypeB\x1a\xe0A\x02\x92A\x14\xca>\x11\xfa\x02\x0eentityTypeName\x12/\n\x0bupdate_mask\x18\x02 \x01(\x0b2\x1a.google.protobuf.FieldMask\x12\x15\n\rallow_missing\x18\x03 \x01(\x08"C\n\x17DeleteEntityTypeRequest\x12(\n\x04name\x18\x01 \x01(\tB\x1a\xe0A\x02\x92A\x14\xca>\x11\xfa\x02\x0eentityTypeName"h\n\x13ListEntitiesRequest\x12*\n\x06parent\x18\x01 \x01(\tB\x1a\xe0A\x02\x92A\x14\xca>\x11\xfa\x02\x0eentityTypeName\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12\x12\n\npage_token\x18\x03 \x01(\t"q\n\x14ListEntitiesResponse\x12,\n\x08entities\x18\x01 \x03(\x0b2\x1a.exabel.api.data.v1.Entity\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\x12\x12\n\ntotal_size\x18\x03 \x01(\x05"T\n\x15DeleteEntitiesRequest\x12*\n\x06parent\x18\x01 \x01(\tB\x1a\xe0A\x02\x92A\x14\xca>\x11\xfa\x02\x0eentityTypeName\x12\x0f\n\x07confirm\x18\x02 \x01(\x08"8\n\x10GetEntityRequest\x12$\n\x04name\x18\x01 \x01(\tB\x16\xe0A\x02\x92A\x10\xca>\r\xfa\x02\nentityName"r\n\x13CreateEntityRequest\x12*\n\x06parent\x18\x01 \x01(\tB\x1a\xe0A\x02\x92A\x14\xca>\x11\xfa\x02\x0eentityTypeName\x12/\n\x06entity\x18\x02 \x01(\x0b2\x1a.exabel.api.data.v1.EntityB\x03\xe0A\x02"\xa1\x01\n\x13UpdateEntityRequest\x12B\n\x06entity\x18\x01 \x01(\x0b2\x1a.exabel.api.data.v1.EntityB\x16\xe0A\x02\x92A\x10\xca>\r\xfa\x02\nentityName\x12/\n\x0bupdate_mask\x18\x02 \x01(\x0b2\x1a.google.protobuf.FieldMask\x12\x15\n\rallow_missing\x18\x03 \x01(\x08";\n\x13DeleteEntityRequest\x12$\n\x04name\x18\x01 \x01(\tB\x16\xe0A\x02\x92A\x10\xca>\r\xfa\x02\nentityName"\xd2\x01\n\x15SearchEntitiesRequest\x12*\n\x06parent\x18\x04 \x01(\tB\x1a\xe0A\x02\x92A\x14\xca>\x11\xfa\x02\x0eentityTypeName\x122\n\x05terms\x18\x01 \x03(\x0b2\x1e.exabel.api.data.v1.SearchTermB\x03\xe0A\x02\x122\n\x07options\x18\x05 \x01(\x0b2!.exabel.api.data.v1.SearchOptions\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12\x12\n\npage_token\x18\x03 \x01(\t"\x96\x02\n\x16SearchEntitiesResponse\x12H\n\x07results\x18\x03 \x03(\x0b27.exabel.api.data.v1.SearchEntitiesResponse.SearchResult\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\x12,\n\x08entities\x18\x01 \x03(\x0b2\x1a.exabel.api.data.v1.Entity\x1ak\n\x0cSearchResult\x12-\n\x05terms\x18\x01 \x03(\x0b2\x1e.exabel.api.data.v1.SearchTerm\x12,\n\x08entities\x18\x02 \x03(\x0b2\x1a.exabel.api.data.v1.Entity2\xf7\x0e\n\rEntityService\x12\x99\x01\n\x0fListEntityTypes\x12*.exabel.api.data.v1.ListEntityTypesRequest\x1a+.exabel.api.data.v1.ListEntityTypesResponse"-\x82\xd3\xe4\x93\x02\x11\x12\x0f/v1/entityTypes\x92A\x13\x12\x11List entity types\x12\x8f\x01\n\rGetEntityType\x12(.exabel.api.data.v1.GetEntityTypeRequest\x1a\x1e.exabel.api.data.v1.EntityType"4\x82\xd3\xe4\x93\x02\x1a\x12\x18/v1/{name=entityTypes/*}\x92A\x11\x12\x0fGet entity type\x12\x9c\x01\n\x10CreateEntityType\x12+.exabel.api.data.v1.CreateEntityTypeRequest\x1a\x1e.exabel.api.data.v1.EntityType";\x82\xd3\xe4\x93\x02\x1e"\x0f/v1/entityTypes:\x0bentity_type\x92A\x14\x12\x12Create entity type\x12\xb1\x01\n\x10UpdateEntityType\x12+.exabel.api.data.v1.UpdateEntityTypeRequest\x1a\x1e.exabel.api.data.v1.EntityType"P\x82\xd3\xe4\x93\x0232$/v1/{entity_type.name=entityTypes/*}:\x0bentity_type\x92A\x14\x12\x12Update entity type\x12\x90\x01\n\x10DeleteEntityType\x12+.exabel.api.data.v1.DeleteEntityTypeRequest\x1a\x16.google.protobuf.Empty"7\x82\xd3\xe4\x93\x02\x1a*\x18/v1/{name=entityTypes/*}\x92A\x14\x12\x12Delete entity type\x12\xa0\x01\n\x0cListEntities\x12\'.exabel.api.data.v1.ListEntitiesRequest\x1a(.exabel.api.data.v1.ListEntitiesResponse"=\x82\xd3\xe4\x93\x02%\x12#/v1/{parent=entityTypes/*}/entities\x92A\x0f\x12\rList entities\x12\x9b\x01\n\x0eDeleteEntities\x12).exabel.api.data.v1.DeleteEntitiesRequest\x1a\x16.google.protobuf.Empty"F\x82\xd3\xe4\x93\x02%*#/v1/{parent=entityTypes/*}/entities\x92A\x18\x12\x16Delete entities (bulk)\x12\x89\x01\n\tGetEntity\x12$.exabel.api.data.v1.GetEntityRequest\x1a\x1a.exabel.api.data.v1.Entity":\x82\xd3\xe4\x93\x02%\x12#/v1/{name=entityTypes/*/entities/*}\x92A\x0c\x12\nGet entity\x12\x9a\x01\n\x0cCreateEntity\x12\'.exabel.api.data.v1.CreateEntityRequest\x1a\x1a.exabel.api.data.v1.Entity"E\x82\xd3\xe4\x93\x02-"#/v1/{parent=entityTypes/*}/entities:\x06entity\x92A\x0f\x12\rCreate entity\x12\xa1\x01\n\x0cUpdateEntity\x12\'.exabel.api.data.v1.UpdateEntityRequest\x1a\x1a.exabel.api.data.v1.Entity"L\x82\xd3\xe4\x93\x0242*/v1/{entity.name=entityTypes/*/entities/*}:\x06entity\x92A\x0f\x12\rUpdate entity\x12\x8e\x01\n\x0cDeleteEntity\x12\'.exabel.api.data.v1.DeleteEntityRequest\x1a\x16.google.protobuf.Empty"=\x82\xd3\xe4\x93\x02%*#/v1/{name=entityTypes/*/entities/*}\x92A\x0f\x12\rDelete entity\x12\xb2\x01\n\x0eSearchEntities\x12).exabel.api.data.v1.SearchEntitiesRequest\x1a*.exabel.api.data.v1.SearchEntitiesResponse"I\x82\xd3\xe4\x93\x02/"*/v1/{parent=entityTypes/*}/entities:search:\x01*\x92A\x11\x12\x0fSearch entitiesBF\n\x16com.exabel.api.data.v1B\x12EntityServiceProtoP\x01Z\x16exabel.com/api/data/v1b\x06proto3')
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.data.v1.entity_service_pb2', globals())
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\'exabel/api/data/v1/entity_service.proto\x12\x12exabel.api.data.v1\x1a(exabel/api/data/v1/entity_messages.proto\x1a(exabel/api/data/v1/search_messages.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1fgoogle/api/field_behavior.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a google/protobuf/field_mask.proto\x1a.protoc_gen_openapiv2/options/annotations.proto"?\n\x16ListEntityTypesRequest\x12\x11\n\tpage_size\x18\x01 \x01(\x05\x12\x12\n\npage_token\x18\x02 \x01(\t"|\n\x17ListEntityTypesResponse\x124\n\x0centity_types\x18\x01 \x03(\x0b2\x1e.exabel.api.data.v1.EntityType\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\x12\x12\n\ntotal_size\x18\x03 \x01(\x05"A\n\x14GetEntityTypeRequest\x12)\n\x04name\x18\x01 \x01(\tB\x1b\x92A\x14\xca>\x11\xfa\x02\x0eentityTypeName\xe2A\x01\x02"k\n\x17CreateEntityTypeRequest\x12P\n\x0bentity_type\x18\x01 \x01(\x0b2\x1e.exabel.api.data.v1.EntityTypeB\x1b\x92A\x14\xca>\x11\xfa\x02\x0eentityTypeName\xe2A\x01\x02"\xb3\x01\n\x17UpdateEntityTypeRequest\x12P\n\x0bentity_type\x18\x01 \x01(\x0b2\x1e.exabel.api.data.v1.EntityTypeB\x1b\x92A\x14\xca>\x11\xfa\x02\x0eentityTypeName\xe2A\x01\x02\x12/\n\x0bupdate_mask\x18\x02 \x01(\x0b2\x1a.google.protobuf.FieldMask\x12\x15\n\rallow_missing\x18\x03 \x01(\x08"D\n\x17DeleteEntityTypeRequest\x12)\n\x04name\x18\x01 \x01(\tB\x1b\x92A\x14\xca>\x11\xfa\x02\x0eentityTypeName\xe2A\x01\x02"i\n\x13ListEntitiesRequest\x12+\n\x06parent\x18\x01 \x01(\tB\x1b\x92A\x14\xca>\x11\xfa\x02\x0eentityTypeName\xe2A\x01\x02\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12\x12\n\npage_token\x18\x03 \x01(\t"q\n\x14ListEntitiesResponse\x12,\n\x08entities\x18\x01 \x03(\x0b2\x1a.exabel.api.data.v1.Entity\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\x12\x12\n\ntotal_size\x18\x03 \x01(\x05"U\n\x15DeleteEntitiesRequest\x12+\n\x06parent\x18\x01 \x01(\tB\x1b\x92A\x14\xca>\x11\xfa\x02\x0eentityTypeName\xe2A\x01\x02\x12\x0f\n\x07confirm\x18\x02 \x01(\x08"9\n\x10GetEntityRequest\x12%\n\x04name\x18\x01 \x01(\tB\x17\x92A\x10\xca>\r\xfa\x02\nentityName\xe2A\x01\x02"t\n\x13CreateEntityRequest\x12+\n\x06parent\x18\x01 \x01(\tB\x1b\x92A\x14\xca>\x11\xfa\x02\x0eentityTypeName\xe2A\x01\x02\x120\n\x06entity\x18\x02 \x01(\x0b2\x1a.exabel.api.data.v1.EntityB\x04\xe2A\x01\x02"\xa2\x01\n\x13UpdateEntityRequest\x12C\n\x06entity\x18\x01 \x01(\x0b2\x1a.exabel.api.data.v1.EntityB\x17\x92A\x10\xca>\r\xfa\x02\nentityName\xe2A\x01\x02\x12/\n\x0bupdate_mask\x18\x02 \x01(\x0b2\x1a.google.protobuf.FieldMask\x12\x15\n\rallow_missing\x18\x03 \x01(\x08"<\n\x13DeleteEntityRequest\x12%\n\x04name\x18\x01 \x01(\tB\x17\x92A\x10\xca>\r\xfa\x02\nentityName\xe2A\x01\x02"\xd4\x01\n\x15SearchEntitiesRequest\x12+\n\x06parent\x18\x04 \x01(\tB\x1b\x92A\x14\xca>\x11\xfa\x02\x0eentityTypeName\xe2A\x01\x02\x123\n\x05terms\x18\x01 \x03(\x0b2\x1e.exabel.api.data.v1.SearchTermB\x04\xe2A\x01\x02\x122\n\x07options\x18\x05 \x01(\x0b2!.exabel.api.data.v1.SearchOptions\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12\x12\n\npage_token\x18\x03 \x01(\t"\x96\x02\n\x16SearchEntitiesResponse\x12H\n\x07results\x18\x03 \x03(\x0b27.exabel.api.data.v1.SearchEntitiesResponse.SearchResult\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\x12,\n\x08entities\x18\x01 \x03(\x0b2\x1a.exabel.api.data.v1.Entity\x1ak\n\x0cSearchResult\x12-\n\x05terms\x18\x01 \x03(\x0b2\x1e.exabel.api.data.v1.SearchTerm\x12,\n\x08entities\x18\x02 \x03(\x0b2\x1a.exabel.api.data.v1.Entity2\xf7\x0e\n\rEntityService\x12\x99\x01\n\x0fListEntityTypes\x12*.exabel.api.data.v1.ListEntityTypesRequest\x1a+.exabel.api.data.v1.ListEntityTypesResponse"-\x92A\x13\x12\x11List entity types\x82\xd3\xe4\x93\x02\x11\x12\x0f/v1/entityTypes\x12\x8f\x01\n\rGetEntityType\x12(.exabel.api.data.v1.GetEntityTypeRequest\x1a\x1e.exabel.api.data.v1.EntityType"4\x92A\x11\x12\x0fGet entity type\x82\xd3\xe4\x93\x02\x1a\x12\x18/v1/{name=entityTypes/*}\x12\x9c\x01\n\x10CreateEntityType\x12+.exabel.api.data.v1.CreateEntityTypeRequest\x1a\x1e.exabel.api.data.v1.EntityType";\x92A\x14\x12\x12Create entity type\x82\xd3\xe4\x93\x02\x1e"\x0f/v1/entityTypes:\x0bentity_type\x12\xb1\x01\n\x10UpdateEntityType\x12+.exabel.api.data.v1.UpdateEntityTypeRequest\x1a\x1e.exabel.api.data.v1.EntityType"P\x92A\x14\x12\x12Update entity type\x82\xd3\xe4\x93\x0232$/v1/{entity_type.name=entityTypes/*}:\x0bentity_type\x12\x90\x01\n\x10DeleteEntityType\x12+.exabel.api.data.v1.DeleteEntityTypeRequest\x1a\x16.google.protobuf.Empty"7\x92A\x14\x12\x12Delete entity type\x82\xd3\xe4\x93\x02\x1a*\x18/v1/{name=entityTypes/*}\x12\xa0\x01\n\x0cListEntities\x12\'.exabel.api.data.v1.ListEntitiesRequest\x1a(.exabel.api.data.v1.ListEntitiesResponse"=\x92A\x0f\x12\rList entities\x82\xd3\xe4\x93\x02%\x12#/v1/{parent=entityTypes/*}/entities\x12\x9b\x01\n\x0eDeleteEntities\x12).exabel.api.data.v1.DeleteEntitiesRequest\x1a\x16.google.protobuf.Empty"F\x92A\x18\x12\x16Delete entities (bulk)\x82\xd3\xe4\x93\x02%*#/v1/{parent=entityTypes/*}/entities\x12\x89\x01\n\tGetEntity\x12$.exabel.api.data.v1.GetEntityRequest\x1a\x1a.exabel.api.data.v1.Entity":\x92A\x0c\x12\nGet entity\x82\xd3\xe4\x93\x02%\x12#/v1/{name=entityTypes/*/entities/*}\x12\x9a\x01\n\x0cCreateEntity\x12\'.exabel.api.data.v1.CreateEntityRequest\x1a\x1a.exabel.api.data.v1.Entity"E\x92A\x0f\x12\rCreate entity\x82\xd3\xe4\x93\x02-"#/v1/{parent=entityTypes/*}/entities:\x06entity\x12\xa1\x01\n\x0cUpdateEntity\x12\'.exabel.api.data.v1.UpdateEntityRequest\x1a\x1a.exabel.api.data.v1.Entity"L\x92A\x0f\x12\rUpdate entity\x82\xd3\xe4\x93\x0242*/v1/{entity.name=entityTypes/*/entities/*}:\x06entity\x12\x8e\x01\n\x0cDeleteEntity\x12\'.exabel.api.data.v1.DeleteEntityRequest\x1a\x16.google.protobuf.Empty"=\x92A\x0f\x12\rDelete entity\x82\xd3\xe4\x93\x02%*#/v1/{name=entityTypes/*/entities/*}\x12\xb2\x01\n\x0eSearchEntities\x12).exabel.api.data.v1.SearchEntitiesRequest\x1a*.exabel.api.data.v1.SearchEntitiesResponse"I\x92A\x11\x12\x0fSearch entities\x82\xd3\xe4\x93\x02/"*/v1/{parent=entityTypes/*}/entities:search:\x01*BF\n\x16com.exabel.api.data.v1B\x12EntityServiceProtoP\x01Z\x16exabel.com/api/data/v1b\x06proto3')
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.data.v1.entity_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b'\n\x16com.exabel.api.data.v1B\x12EntityServiceProtoP\x01Z\x16exabel.com/api/data/v1'
     _GETENTITYTYPEREQUEST.fields_by_name['name']._options = None
-    _GETENTITYTYPEREQUEST.fields_by_name['name']._serialized_options = b'\xe0A\x02\x92A\x14\xca>\x11\xfa\x02\x0eentityTypeName'
+    _GETENTITYTYPEREQUEST.fields_by_name['name']._serialized_options = b'\x92A\x14\xca>\x11\xfa\x02\x0eentityTypeName\xe2A\x01\x02'
     _CREATEENTITYTYPEREQUEST.fields_by_name['entity_type']._options = None
-    _CREATEENTITYTYPEREQUEST.fields_by_name['entity_type']._serialized_options = b'\xe0A\x02\x92A\x14\xca>\x11\xfa\x02\x0eentityTypeName'
+    _CREATEENTITYTYPEREQUEST.fields_by_name['entity_type']._serialized_options = b'\x92A\x14\xca>\x11\xfa\x02\x0eentityTypeName\xe2A\x01\x02'
     _UPDATEENTITYTYPEREQUEST.fields_by_name['entity_type']._options = None
-    _UPDATEENTITYTYPEREQUEST.fields_by_name['entity_type']._serialized_options = b'\xe0A\x02\x92A\x14\xca>\x11\xfa\x02\x0eentityTypeName'
+    _UPDATEENTITYTYPEREQUEST.fields_by_name['entity_type']._serialized_options = b'\x92A\x14\xca>\x11\xfa\x02\x0eentityTypeName\xe2A\x01\x02'
     _DELETEENTITYTYPEREQUEST.fields_by_name['name']._options = None
-    _DELETEENTITYTYPEREQUEST.fields_by_name['name']._serialized_options = b'\xe0A\x02\x92A\x14\xca>\x11\xfa\x02\x0eentityTypeName'
+    _DELETEENTITYTYPEREQUEST.fields_by_name['name']._serialized_options = b'\x92A\x14\xca>\x11\xfa\x02\x0eentityTypeName\xe2A\x01\x02'
     _LISTENTITIESREQUEST.fields_by_name['parent']._options = None
-    _LISTENTITIESREQUEST.fields_by_name['parent']._serialized_options = b'\xe0A\x02\x92A\x14\xca>\x11\xfa\x02\x0eentityTypeName'
+    _LISTENTITIESREQUEST.fields_by_name['parent']._serialized_options = b'\x92A\x14\xca>\x11\xfa\x02\x0eentityTypeName\xe2A\x01\x02'
     _DELETEENTITIESREQUEST.fields_by_name['parent']._options = None
-    _DELETEENTITIESREQUEST.fields_by_name['parent']._serialized_options = b'\xe0A\x02\x92A\x14\xca>\x11\xfa\x02\x0eentityTypeName'
+    _DELETEENTITIESREQUEST.fields_by_name['parent']._serialized_options = b'\x92A\x14\xca>\x11\xfa\x02\x0eentityTypeName\xe2A\x01\x02'
     _GETENTITYREQUEST.fields_by_name['name']._options = None
-    _GETENTITYREQUEST.fields_by_name['name']._serialized_options = b'\xe0A\x02\x92A\x10\xca>\r\xfa\x02\nentityName'
+    _GETENTITYREQUEST.fields_by_name['name']._serialized_options = b'\x92A\x10\xca>\r\xfa\x02\nentityName\xe2A\x01\x02'
     _CREATEENTITYREQUEST.fields_by_name['parent']._options = None
-    _CREATEENTITYREQUEST.fields_by_name['parent']._serialized_options = b'\xe0A\x02\x92A\x14\xca>\x11\xfa\x02\x0eentityTypeName'
+    _CREATEENTITYREQUEST.fields_by_name['parent']._serialized_options = b'\x92A\x14\xca>\x11\xfa\x02\x0eentityTypeName\xe2A\x01\x02'
     _CREATEENTITYREQUEST.fields_by_name['entity']._options = None
-    _CREATEENTITYREQUEST.fields_by_name['entity']._serialized_options = b'\xe0A\x02'
+    _CREATEENTITYREQUEST.fields_by_name['entity']._serialized_options = b'\xe2A\x01\x02'
     _UPDATEENTITYREQUEST.fields_by_name['entity']._options = None
-    _UPDATEENTITYREQUEST.fields_by_name['entity']._serialized_options = b'\xe0A\x02\x92A\x10\xca>\r\xfa\x02\nentityName'
+    _UPDATEENTITYREQUEST.fields_by_name['entity']._serialized_options = b'\x92A\x10\xca>\r\xfa\x02\nentityName\xe2A\x01\x02'
     _DELETEENTITYREQUEST.fields_by_name['name']._options = None
-    _DELETEENTITYREQUEST.fields_by_name['name']._serialized_options = b'\xe0A\x02\x92A\x10\xca>\r\xfa\x02\nentityName'
+    _DELETEENTITYREQUEST.fields_by_name['name']._serialized_options = b'\x92A\x10\xca>\r\xfa\x02\nentityName\xe2A\x01\x02'
     _SEARCHENTITIESREQUEST.fields_by_name['parent']._options = None
-    _SEARCHENTITIESREQUEST.fields_by_name['parent']._serialized_options = b'\xe0A\x02\x92A\x14\xca>\x11\xfa\x02\x0eentityTypeName'
+    _SEARCHENTITIESREQUEST.fields_by_name['parent']._serialized_options = b'\x92A\x14\xca>\x11\xfa\x02\x0eentityTypeName\xe2A\x01\x02'
     _SEARCHENTITIESREQUEST.fields_by_name['terms']._options = None
-    _SEARCHENTITIESREQUEST.fields_by_name['terms']._serialized_options = b'\xe0A\x02'
+    _SEARCHENTITIESREQUEST.fields_by_name['terms']._serialized_options = b'\xe2A\x01\x02'
     _ENTITYSERVICE.methods_by_name['ListEntityTypes']._options = None
-    _ENTITYSERVICE.methods_by_name['ListEntityTypes']._serialized_options = b'\x82\xd3\xe4\x93\x02\x11\x12\x0f/v1/entityTypes\x92A\x13\x12\x11List entity types'
+    _ENTITYSERVICE.methods_by_name['ListEntityTypes']._serialized_options = b'\x92A\x13\x12\x11List entity types\x82\xd3\xe4\x93\x02\x11\x12\x0f/v1/entityTypes'
     _ENTITYSERVICE.methods_by_name['GetEntityType']._options = None
-    _ENTITYSERVICE.methods_by_name['GetEntityType']._serialized_options = b'\x82\xd3\xe4\x93\x02\x1a\x12\x18/v1/{name=entityTypes/*}\x92A\x11\x12\x0fGet entity type'
+    _ENTITYSERVICE.methods_by_name['GetEntityType']._serialized_options = b'\x92A\x11\x12\x0fGet entity type\x82\xd3\xe4\x93\x02\x1a\x12\x18/v1/{name=entityTypes/*}'
     _ENTITYSERVICE.methods_by_name['CreateEntityType']._options = None
-    _ENTITYSERVICE.methods_by_name['CreateEntityType']._serialized_options = b'\x82\xd3\xe4\x93\x02\x1e"\x0f/v1/entityTypes:\x0bentity_type\x92A\x14\x12\x12Create entity type'
+    _ENTITYSERVICE.methods_by_name['CreateEntityType']._serialized_options = b'\x92A\x14\x12\x12Create entity type\x82\xd3\xe4\x93\x02\x1e"\x0f/v1/entityTypes:\x0bentity_type'
     _ENTITYSERVICE.methods_by_name['UpdateEntityType']._options = None
-    _ENTITYSERVICE.methods_by_name['UpdateEntityType']._serialized_options = b'\x82\xd3\xe4\x93\x0232$/v1/{entity_type.name=entityTypes/*}:\x0bentity_type\x92A\x14\x12\x12Update entity type'
+    _ENTITYSERVICE.methods_by_name['UpdateEntityType']._serialized_options = b'\x92A\x14\x12\x12Update entity type\x82\xd3\xe4\x93\x0232$/v1/{entity_type.name=entityTypes/*}:\x0bentity_type'
     _ENTITYSERVICE.methods_by_name['DeleteEntityType']._options = None
-    _ENTITYSERVICE.methods_by_name['DeleteEntityType']._serialized_options = b'\x82\xd3\xe4\x93\x02\x1a*\x18/v1/{name=entityTypes/*}\x92A\x14\x12\x12Delete entity type'
+    _ENTITYSERVICE.methods_by_name['DeleteEntityType']._serialized_options = b'\x92A\x14\x12\x12Delete entity type\x82\xd3\xe4\x93\x02\x1a*\x18/v1/{name=entityTypes/*}'
     _ENTITYSERVICE.methods_by_name['ListEntities']._options = None
-    _ENTITYSERVICE.methods_by_name['ListEntities']._serialized_options = b'\x82\xd3\xe4\x93\x02%\x12#/v1/{parent=entityTypes/*}/entities\x92A\x0f\x12\rList entities'
+    _ENTITYSERVICE.methods_by_name['ListEntities']._serialized_options = b'\x92A\x0f\x12\rList entities\x82\xd3\xe4\x93\x02%\x12#/v1/{parent=entityTypes/*}/entities'
     _ENTITYSERVICE.methods_by_name['DeleteEntities']._options = None
-    _ENTITYSERVICE.methods_by_name['DeleteEntities']._serialized_options = b'\x82\xd3\xe4\x93\x02%*#/v1/{parent=entityTypes/*}/entities\x92A\x18\x12\x16Delete entities (bulk)'
+    _ENTITYSERVICE.methods_by_name['DeleteEntities']._serialized_options = b'\x92A\x18\x12\x16Delete entities (bulk)\x82\xd3\xe4\x93\x02%*#/v1/{parent=entityTypes/*}/entities'
     _ENTITYSERVICE.methods_by_name['GetEntity']._options = None
-    _ENTITYSERVICE.methods_by_name['GetEntity']._serialized_options = b'\x82\xd3\xe4\x93\x02%\x12#/v1/{name=entityTypes/*/entities/*}\x92A\x0c\x12\nGet entity'
+    _ENTITYSERVICE.methods_by_name['GetEntity']._serialized_options = b'\x92A\x0c\x12\nGet entity\x82\xd3\xe4\x93\x02%\x12#/v1/{name=entityTypes/*/entities/*}'
     _ENTITYSERVICE.methods_by_name['CreateEntity']._options = None
-    _ENTITYSERVICE.methods_by_name['CreateEntity']._serialized_options = b'\x82\xd3\xe4\x93\x02-"#/v1/{parent=entityTypes/*}/entities:\x06entity\x92A\x0f\x12\rCreate entity'
+    _ENTITYSERVICE.methods_by_name['CreateEntity']._serialized_options = b'\x92A\x0f\x12\rCreate entity\x82\xd3\xe4\x93\x02-"#/v1/{parent=entityTypes/*}/entities:\x06entity'
     _ENTITYSERVICE.methods_by_name['UpdateEntity']._options = None
-    _ENTITYSERVICE.methods_by_name['UpdateEntity']._serialized_options = b'\x82\xd3\xe4\x93\x0242*/v1/{entity.name=entityTypes/*/entities/*}:\x06entity\x92A\x0f\x12\rUpdate entity'
+    _ENTITYSERVICE.methods_by_name['UpdateEntity']._serialized_options = b'\x92A\x0f\x12\rUpdate entity\x82\xd3\xe4\x93\x0242*/v1/{entity.name=entityTypes/*/entities/*}:\x06entity'
     _ENTITYSERVICE.methods_by_name['DeleteEntity']._options = None
-    _ENTITYSERVICE.methods_by_name['DeleteEntity']._serialized_options = b'\x82\xd3\xe4\x93\x02%*#/v1/{name=entityTypes/*/entities/*}\x92A\x0f\x12\rDelete entity'
+    _ENTITYSERVICE.methods_by_name['DeleteEntity']._serialized_options = b'\x92A\x0f\x12\rDelete entity\x82\xd3\xe4\x93\x02%*#/v1/{name=entityTypes/*/entities/*}'
     _ENTITYSERVICE.methods_by_name['SearchEntities']._options = None
-    _ENTITYSERVICE.methods_by_name['SearchEntities']._serialized_options = b'\x82\xd3\xe4\x93\x02/"*/v1/{parent=entityTypes/*}/entities:search:\x01*\x92A\x11\x12\x0fSearch entities'
-    _LISTENTITYTYPESREQUEST._serialized_start = 321
-    _LISTENTITYTYPESREQUEST._serialized_end = 384
-    _LISTENTITYTYPESRESPONSE._serialized_start = 386
-    _LISTENTITYTYPESRESPONSE._serialized_end = 510
-    _GETENTITYTYPEREQUEST._serialized_start = 512
-    _GETENTITYTYPEREQUEST._serialized_end = 576
-    _CREATEENTITYTYPEREQUEST._serialized_start = 578
-    _CREATEENTITYTYPEREQUEST._serialized_end = 684
-    _UPDATEENTITYTYPEREQUEST._serialized_start = 687
-    _UPDATEENTITYTYPEREQUEST._serialized_end = 865
-    _DELETEENTITYTYPEREQUEST._serialized_start = 867
-    _DELETEENTITYTYPEREQUEST._serialized_end = 934
-    _LISTENTITIESREQUEST._serialized_start = 936
-    _LISTENTITIESREQUEST._serialized_end = 1040
-    _LISTENTITIESRESPONSE._serialized_start = 1042
-    _LISTENTITIESRESPONSE._serialized_end = 1155
-    _DELETEENTITIESREQUEST._serialized_start = 1157
-    _DELETEENTITIESREQUEST._serialized_end = 1241
-    _GETENTITYREQUEST._serialized_start = 1243
-    _GETENTITYREQUEST._serialized_end = 1299
-    _CREATEENTITYREQUEST._serialized_start = 1301
-    _CREATEENTITYREQUEST._serialized_end = 1415
-    _UPDATEENTITYREQUEST._serialized_start = 1418
-    _UPDATEENTITYREQUEST._serialized_end = 1579
-    _DELETEENTITYREQUEST._serialized_start = 1581
-    _DELETEENTITYREQUEST._serialized_end = 1640
-    _SEARCHENTITIESREQUEST._serialized_start = 1643
-    _SEARCHENTITIESREQUEST._serialized_end = 1853
-    _SEARCHENTITIESRESPONSE._serialized_start = 1856
-    _SEARCHENTITIESRESPONSE._serialized_end = 2134
-    _SEARCHENTITIESRESPONSE_SEARCHRESULT._serialized_start = 2027
-    _SEARCHENTITIESRESPONSE_SEARCHRESULT._serialized_end = 2134
-    _ENTITYSERVICE._serialized_start = 2137
-    _ENTITYSERVICE._serialized_end = 4048
+    _ENTITYSERVICE.methods_by_name['SearchEntities']._serialized_options = b'\x92A\x11\x12\x0fSearch entities\x82\xd3\xe4\x93\x02/"*/v1/{parent=entityTypes/*}/entities:search:\x01*'
+    _globals['_LISTENTITYTYPESREQUEST']._serialized_start = 321
+    _globals['_LISTENTITYTYPESREQUEST']._serialized_end = 384
+    _globals['_LISTENTITYTYPESRESPONSE']._serialized_start = 386
+    _globals['_LISTENTITYTYPESRESPONSE']._serialized_end = 510
+    _globals['_GETENTITYTYPEREQUEST']._serialized_start = 512
+    _globals['_GETENTITYTYPEREQUEST']._serialized_end = 577
+    _globals['_CREATEENTITYTYPEREQUEST']._serialized_start = 579
+    _globals['_CREATEENTITYTYPEREQUEST']._serialized_end = 686
+    _globals['_UPDATEENTITYTYPEREQUEST']._serialized_start = 689
+    _globals['_UPDATEENTITYTYPEREQUEST']._serialized_end = 868
+    _globals['_DELETEENTITYTYPEREQUEST']._serialized_start = 870
+    _globals['_DELETEENTITYTYPEREQUEST']._serialized_end = 938
+    _globals['_LISTENTITIESREQUEST']._serialized_start = 940
+    _globals['_LISTENTITIESREQUEST']._serialized_end = 1045
+    _globals['_LISTENTITIESRESPONSE']._serialized_start = 1047
+    _globals['_LISTENTITIESRESPONSE']._serialized_end = 1160
+    _globals['_DELETEENTITIESREQUEST']._serialized_start = 1162
+    _globals['_DELETEENTITIESREQUEST']._serialized_end = 1247
+    _globals['_GETENTITYREQUEST']._serialized_start = 1249
+    _globals['_GETENTITYREQUEST']._serialized_end = 1306
+    _globals['_CREATEENTITYREQUEST']._serialized_start = 1308
+    _globals['_CREATEENTITYREQUEST']._serialized_end = 1424
+    _globals['_UPDATEENTITYREQUEST']._serialized_start = 1427
+    _globals['_UPDATEENTITYREQUEST']._serialized_end = 1589
+    _globals['_DELETEENTITYREQUEST']._serialized_start = 1591
+    _globals['_DELETEENTITYREQUEST']._serialized_end = 1651
+    _globals['_SEARCHENTITIESREQUEST']._serialized_start = 1654
+    _globals['_SEARCHENTITIESREQUEST']._serialized_end = 1866
+    _globals['_SEARCHENTITIESRESPONSE']._serialized_start = 1869
+    _globals['_SEARCHENTITIESRESPONSE']._serialized_end = 2147
+    _globals['_SEARCHENTITIESRESPONSE_SEARCHRESULT']._serialized_start = 2040
+    _globals['_SEARCHENTITIESRESPONSE_SEARCHRESULT']._serialized_end = 2147
+    _globals['_ENTITYSERVICE']._serialized_start = 2150
+    _globals['_ENTITYSERVICE']._serialized_end = 4061
```

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_service_pb2_grpc.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/data/v1/import_job_service_pb2.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/data/v1/import_job_service_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 _sym_db = _symbol_database.Default()
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from google.api import field_behavior_pb2 as google_dot_api_dot_field__behavior__pb2
 from .....protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n+exabel/api/data/v1/import_job_service.proto\x12\x12exabel.api.data.v1\x1a\x1cgoogle/api/annotations.proto\x1a\x1fgoogle/api/field_behavior.proto\x1a.protoc_gen_openapiv2/options/annotations.proto"4\n\x0eRunTaskRequest\x12"\n\x04name\x18\x01 \x01(\tB\x14\xe0A\x02\x92A\x0e\xca>\x0b\xfa\x02\x08taskName"\x11\n\x0fRunTaskResponse2\x9e\x01\n\x10ImportJobService\x12\x89\x01\n\x07RunTask\x12".exabel.api.data.v1.RunTaskRequest\x1a#.exabel.api.data.v1.RunTaskResponse"5\x82\xd3\xe4\x93\x02\x1b"\x16/v1/{name=tasks/*}:run:\x01*\x92A\x11\x12\x0fRun import taskBJ\n\x16com.exabel.api.data.v1B\x16ImportJobsServiceProtoP\x01Z\x16exabel.com/api/data/v1b\x06proto3')
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.data.v1.import_job_service_pb2', globals())
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n+exabel/api/data/v1/import_job_service.proto\x12\x12exabel.api.data.v1\x1a\x1cgoogle/api/annotations.proto\x1a\x1fgoogle/api/field_behavior.proto\x1a.protoc_gen_openapiv2/options/annotations.proto"5\n\x0eRunTaskRequest\x12#\n\x04name\x18\x01 \x01(\tB\x15\x92A\x0e\xca>\x0b\xfa\x02\x08taskName\xe2A\x01\x02"\x11\n\x0fRunTaskResponse2\x9e\x01\n\x10ImportJobService\x12\x89\x01\n\x07RunTask\x12".exabel.api.data.v1.RunTaskRequest\x1a#.exabel.api.data.v1.RunTaskResponse"5\x92A\x11\x12\x0fRun import task\x82\xd3\xe4\x93\x02\x1b"\x16/v1/{name=tasks/*}:run:\x01*BJ\n\x16com.exabel.api.data.v1B\x16ImportJobsServiceProtoP\x01Z\x16exabel.com/api/data/v1b\x06proto3')
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.data.v1.import_job_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b'\n\x16com.exabel.api.data.v1B\x16ImportJobsServiceProtoP\x01Z\x16exabel.com/api/data/v1'
     _RUNTASKREQUEST.fields_by_name['name']._options = None
-    _RUNTASKREQUEST.fields_by_name['name']._serialized_options = b'\xe0A\x02\x92A\x0e\xca>\x0b\xfa\x02\x08taskName'
+    _RUNTASKREQUEST.fields_by_name['name']._serialized_options = b'\x92A\x0e\xca>\x0b\xfa\x02\x08taskName\xe2A\x01\x02'
     _IMPORTJOBSERVICE.methods_by_name['RunTask']._options = None
-    _IMPORTJOBSERVICE.methods_by_name['RunTask']._serialized_options = b'\x82\xd3\xe4\x93\x02\x1b"\x16/v1/{name=tasks/*}:run:\x01*\x92A\x11\x12\x0fRun import task'
-    _RUNTASKREQUEST._serialized_start = 178
-    _RUNTASKREQUEST._serialized_end = 230
-    _RUNTASKRESPONSE._serialized_start = 232
-    _RUNTASKRESPONSE._serialized_end = 249
-    _IMPORTJOBSERVICE._serialized_start = 252
-    _IMPORTJOBSERVICE._serialized_end = 410
+    _IMPORTJOBSERVICE.methods_by_name['RunTask']._serialized_options = b'\x92A\x11\x12\x0fRun import task\x82\xd3\xe4\x93\x02\x1b"\x16/v1/{name=tasks/*}:run:\x01*'
+    _globals['_RUNTASKREQUEST']._serialized_start = 178
+    _globals['_RUNTASKREQUEST']._serialized_end = 231
+    _globals['_RUNTASKRESPONSE']._serialized_start = 233
+    _globals['_RUNTASKRESPONSE']._serialized_end = 250
+    _globals['_IMPORTJOBSERVICE']._serialized_start = 253
+    _globals['_IMPORTJOBSERVICE']._serialized_end = 411
```

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/data/v1/import_job_service_pb2_grpc.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/data/v1/import_job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespace_service_pb2.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespaces_messages_pb2.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 _sym_db = _symbol_database.Default()
-from .....exabel.api.data.v1 import namespaces_messages_pb2 as exabel_dot_api_dot_data_dot_v1_dot_namespaces__messages__pb2
-from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
-from .....protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n*exabel/api/data/v1/namespace_service.proto\x12\x12exabel.api.data.v1\x1a,exabel/api/data/v1/namespaces_messages.proto\x1a\x1cgoogle/api/annotations.proto\x1a.protoc_gen_openapiv2/options/annotations.proto"\x17\n\x15ListNamespacesRequest"K\n\x16ListNamespacesResponse\x121\n\nnamespaces\x18\x01 \x03(\x0b2\x1d.exabel.api.data.v1.Namespace2\xa8\x01\n\x10NamespaceService\x12\x93\x01\n\x0eListNamespaces\x12).exabel.api.data.v1.ListNamespacesRequest\x1a*.exabel.api.data.v1.ListNamespacesResponse"*\x82\xd3\xe4\x93\x02\x10\x12\x0e/v1/namespaces\x92A\x11\x12\x0fList namespacesBI\n\x16com.exabel.api.data.v1B\x15NamespaceServiceProtoP\x01Z\x16exabel.com/api/data/v1b\x06proto3')
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.data.v1.namespace_service_pb2', globals())
+from google.api import field_behavior_pb2 as google_dot_api_dot_field__behavior__pb2
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n,exabel/api/data/v1/namespaces_messages.proto\x12\x12exabel.api.data.v1\x1a\x1fgoogle/api/field_behavior.proto"8\n\tNamespace\x12\x12\n\x04name\x18\x01 \x01(\tB\x04\xe2A\x01\x03\x12\x17\n\twriteable\x18\x02 \x01(\x08B\x04\xe2A\x01\x03BK\n\x16com.exabel.api.data.v1B\x17NamespacesMessagesProtoP\x01Z\x16exabel.com/api/data/v1b\x06proto3')
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.data.v1.namespaces_messages_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    DESCRIPTOR._serialized_options = b'\n\x16com.exabel.api.data.v1B\x15NamespaceServiceProtoP\x01Z\x16exabel.com/api/data/v1'
-    _NAMESPACESERVICE.methods_by_name['ListNamespaces']._options = None
-    _NAMESPACESERVICE.methods_by_name['ListNamespaces']._serialized_options = b'\x82\xd3\xe4\x93\x02\x10\x12\x0e/v1/namespaces\x92A\x11\x12\x0fList namespaces'
-    _LISTNAMESPACESREQUEST._serialized_start = 190
-    _LISTNAMESPACESREQUEST._serialized_end = 213
-    _LISTNAMESPACESRESPONSE._serialized_start = 215
-    _LISTNAMESPACESRESPONSE._serialized_end = 290
-    _NAMESPACESERVICE._serialized_start = 293
-    _NAMESPACESERVICE._serialized_end = 461
+    DESCRIPTOR._serialized_options = b'\n\x16com.exabel.api.data.v1B\x17NamespacesMessagesProtoP\x01Z\x16exabel.com/api/data/v1'
+    _NAMESPACE.fields_by_name['name']._options = None
+    _NAMESPACE.fields_by_name['name']._serialized_options = b'\xe2A\x01\x03'
+    _NAMESPACE.fields_by_name['writeable']._options = None
+    _NAMESPACE.fields_by_name['writeable']._serialized_options = b'\xe2A\x01\x03'
+    _globals['_NAMESPACE']._serialized_start = 101
+    _globals['_NAMESPACE']._serialized_end = 157
```

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespace_service_pb2_grpc.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespace_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespaces_messages_pb2.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_messages_pb2.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 _sym_db = _symbol_database.Default()
 from google.api import field_behavior_pb2 as google_dot_api_dot_field__behavior__pb2
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n,exabel/api/data/v1/namespaces_messages.proto\x12\x12exabel.api.data.v1\x1a\x1fgoogle/api/field_behavior.proto"6\n\tNamespace\x12\x11\n\x04name\x18\x01 \x01(\tB\x03\xe0A\x03\x12\x16\n\twriteable\x18\x02 \x01(\x08B\x03\xe0A\x03BK\n\x16com.exabel.api.data.v1B\x17NamespacesMessagesProtoP\x01Z\x16exabel.com/api/data/v1b\x06proto3')
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.data.v1.namespaces_messages_pb2', globals())
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n,exabel/api/management/v1/user_messages.proto\x12\x18exabel.api.management.v1\x1a\x1fgoogle/api/field_behavior.proto":\n\x04User\x12\x12\n\x04name\x18\x01 \x01(\tB\x04\xe2A\x01\x03\x12\r\n\x05email\x18\x02 \x01(\t\x12\x0f\n\x07blocked\x18\x03 \x01(\x08"`\n\x05Group\x12\x12\n\x04name\x18\x01 \x01(\tB\x04\xe2A\x01\x03\x12\x14\n\x0cdisplay_name\x18\x02 \x01(\t\x12-\n\x05users\x18\x03 \x03(\x0b2\x1e.exabel.api.management.v1.UserBQ\n\x1ccom.exabel.api.management.v1B\x11UserMessagesProtoP\x01Z\x1cexabel.com/api/management/v1b\x06proto3')
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.management.v1.user_messages_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    DESCRIPTOR._serialized_options = b'\n\x16com.exabel.api.data.v1B\x17NamespacesMessagesProtoP\x01Z\x16exabel.com/api/data/v1'
-    _NAMESPACE.fields_by_name['name']._options = None
-    _NAMESPACE.fields_by_name['name']._serialized_options = b'\xe0A\x03'
-    _NAMESPACE.fields_by_name['writeable']._options = None
-    _NAMESPACE.fields_by_name['writeable']._serialized_options = b'\xe0A\x03'
-    _NAMESPACE._serialized_start = 101
-    _NAMESPACE._serialized_end = 155
+    DESCRIPTOR._serialized_options = b'\n\x1ccom.exabel.api.management.v1B\x11UserMessagesProtoP\x01Z\x1cexabel.com/api/management/v1'
+    _USER.fields_by_name['name']._options = None
+    _USER.fields_by_name['name']._serialized_options = b'\xe2A\x01\x03'
+    _GROUP.fields_by_name['name']._options = None
+    _GROUP.fields_by_name['name']._serialized_options = b'\xe2A\x01\x03'
+    _globals['_USER']._serialized_start = 107
+    _globals['_USER']._serialized_end = 165
+    _globals['_GROUP']._serialized_start = 167
+    _globals['_GROUP']._serialized_end = 263
```

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_messages_pb2.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_messages_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 _sym_db = _symbol_database.Default()
 from google.api import field_behavior_pb2 as google_dot_api_dot_field__behavior__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from .....protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n.exabel/api/data/v1/relationship_messages.proto\x12\x12exabel.api.data.v1\x1a\x1fgoogle/api/field_behavior.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a.protoc_gen_openapiv2/options/annotations.proto"\x85\x02\n\x10RelationshipType\x12S\n\x04name\x18\x01 \x01(\tBE\xe0A\x05\xe0A\x02\x92A<J "relationshipTypes/ns.HAS_STORE"\xca>\x17\xfa\x02\x14relationshipTypeName\x12A\n\x0bdescription\x18\x02 \x01(\tB,\x92A)J\'"Indicates that an entity owns a store"\x12\x16\n\tread_only\x18\x03 \x01(\x08B\x03\xe0A\x03\x12\x14\n\x0cis_ownership\x18\x04 \x01(\x08\x12+\n\nproperties\x18d \x01(\x0b2\x17.google.protobuf.Struct"\xf5\x02\n\x0cRelationship\x12R\n\x06parent\x18\x01 \x01(\tBB\xe0A\x02\x92A<J "relationshipTypes/ns.HAS_STORE"\xca>\x17\xfa\x02\x14relationshipTypeName\x12E\n\x0bfrom_entity\x18\x02 \x01(\tB0\xe0A\x02\x92A*J("entityTypes/company/entities/F_12345-E"\x12K\n\tto_entity\x18\x03 \x01(\tB8\xe0A\x02\x92A2J0"entityTypes/ns.store/entities/ns.some_store_id"\x128\n\x0bdescription\x18\x04 \x01(\tB#\x92A J\x1e"F_12345-E owns some_store_id"\x12\x16\n\tread_only\x18\x05 \x01(\x08B\x03\xe0A\x03\x12+\n\nproperties\x18d \x01(\x0b2\x17.google.protobuf.StructBM\n\x16com.exabel.api.data.v1B\x19RelationshipMessagesProtoP\x01Z\x16exabel.com/api/data/v1b\x06proto3')
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.data.v1.relationship_messages_pb2', globals())
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n.exabel/api/data/v1/relationship_messages.proto\x12\x12exabel.api.data.v1\x1a\x1fgoogle/api/field_behavior.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a.protoc_gen_openapiv2/options/annotations.proto"\x85\x02\n\x10RelationshipType\x12R\n\x04name\x18\x01 \x01(\tBD\x92A<J "relationshipTypes/ns.HAS_STORE"\xca>\x17\xfa\x02\x14relationshipTypeName\xe2A\x02\x05\x02\x12A\n\x0bdescription\x18\x02 \x01(\tB,\x92A)J\'"Indicates that an entity owns a store"\x12\x17\n\tread_only\x18\x03 \x01(\x08B\x04\xe2A\x01\x03\x12\x14\n\x0cis_ownership\x18\x04 \x01(\x08\x12+\n\nproperties\x18d \x01(\x0b2\x17.google.protobuf.Struct"\xf9\x02\n\x0cRelationship\x12S\n\x06parent\x18\x01 \x01(\tBC\x92A<J "relationshipTypes/ns.HAS_STORE"\xca>\x17\xfa\x02\x14relationshipTypeName\xe2A\x01\x02\x12F\n\x0bfrom_entity\x18\x02 \x01(\tB1\x92A*J("entityTypes/company/entities/F_12345-E"\xe2A\x01\x02\x12L\n\tto_entity\x18\x03 \x01(\tB9\x92A2J0"entityTypes/ns.store/entities/ns.some_store_id"\xe2A\x01\x02\x128\n\x0bdescription\x18\x04 \x01(\tB#\x92A J\x1e"F_12345-E owns some_store_id"\x12\x17\n\tread_only\x18\x05 \x01(\x08B\x04\xe2A\x01\x03\x12+\n\nproperties\x18d \x01(\x0b2\x17.google.protobuf.StructBM\n\x16com.exabel.api.data.v1B\x19RelationshipMessagesProtoP\x01Z\x16exabel.com/api/data/v1b\x06proto3')
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.data.v1.relationship_messages_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b'\n\x16com.exabel.api.data.v1B\x19RelationshipMessagesProtoP\x01Z\x16exabel.com/api/data/v1'
     _RELATIONSHIPTYPE.fields_by_name['name']._options = None
-    _RELATIONSHIPTYPE.fields_by_name['name']._serialized_options = b'\xe0A\x05\xe0A\x02\x92A<J "relationshipTypes/ns.HAS_STORE"\xca>\x17\xfa\x02\x14relationshipTypeName'
+    _RELATIONSHIPTYPE.fields_by_name['name']._serialized_options = b'\x92A<J "relationshipTypes/ns.HAS_STORE"\xca>\x17\xfa\x02\x14relationshipTypeName\xe2A\x02\x05\x02'
     _RELATIONSHIPTYPE.fields_by_name['description']._options = None
     _RELATIONSHIPTYPE.fields_by_name['description']._serialized_options = b'\x92A)J\'"Indicates that an entity owns a store"'
     _RELATIONSHIPTYPE.fields_by_name['read_only']._options = None
-    _RELATIONSHIPTYPE.fields_by_name['read_only']._serialized_options = b'\xe0A\x03'
+    _RELATIONSHIPTYPE.fields_by_name['read_only']._serialized_options = b'\xe2A\x01\x03'
     _RELATIONSHIP.fields_by_name['parent']._options = None
-    _RELATIONSHIP.fields_by_name['parent']._serialized_options = b'\xe0A\x02\x92A<J "relationshipTypes/ns.HAS_STORE"\xca>\x17\xfa\x02\x14relationshipTypeName'
+    _RELATIONSHIP.fields_by_name['parent']._serialized_options = b'\x92A<J "relationshipTypes/ns.HAS_STORE"\xca>\x17\xfa\x02\x14relationshipTypeName\xe2A\x01\x02'
     _RELATIONSHIP.fields_by_name['from_entity']._options = None
-    _RELATIONSHIP.fields_by_name['from_entity']._serialized_options = b'\xe0A\x02\x92A*J("entityTypes/company/entities/F_12345-E"'
+    _RELATIONSHIP.fields_by_name['from_entity']._serialized_options = b'\x92A*J("entityTypes/company/entities/F_12345-E"\xe2A\x01\x02'
     _RELATIONSHIP.fields_by_name['to_entity']._options = None
-    _RELATIONSHIP.fields_by_name['to_entity']._serialized_options = b'\xe0A\x02\x92A2J0"entityTypes/ns.store/entities/ns.some_store_id"'
+    _RELATIONSHIP.fields_by_name['to_entity']._serialized_options = b'\x92A2J0"entityTypes/ns.store/entities/ns.some_store_id"\xe2A\x01\x02'
     _RELATIONSHIP.fields_by_name['description']._options = None
     _RELATIONSHIP.fields_by_name['description']._serialized_options = b'\x92A J\x1e"F_12345-E owns some_store_id"'
     _RELATIONSHIP.fields_by_name['read_only']._options = None
-    _RELATIONSHIP.fields_by_name['read_only']._serialized_options = b'\xe0A\x03'
-    _RELATIONSHIPTYPE._serialized_start = 182
-    _RELATIONSHIPTYPE._serialized_end = 443
-    _RELATIONSHIP._serialized_start = 446
-    _RELATIONSHIP._serialized_end = 819
+    _RELATIONSHIP.fields_by_name['read_only']._serialized_options = b'\xe2A\x01\x03'
+    _globals['_RELATIONSHIPTYPE']._serialized_start = 182
+    _globals['_RELATIONSHIPTYPE']._serialized_end = 443
+    _globals['_RELATIONSHIP']._serialized_start = 446
+    _globals['_RELATIONSHIP']._serialized_end = 823
```

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_service_pb2.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_service_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,90 +1,91 @@
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 _sym_db = _symbol_database.Default()
 from .....exabel.api.data.v1 import relationship_messages_pb2 as exabel_dot_api_dot_data_dot_v1_dot_relationship__messages__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from google.api import field_behavior_pb2 as google_dot_api_dot_field__behavior__pb2
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 from google.protobuf import field_mask_pb2 as google_dot_protobuf_dot_field__mask__pb2
 from .....protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n-exabel/api/data/v1/relationship_service.proto\x12\x12exabel.api.data.v1\x1a.exabel/api/data/v1/relationship_messages.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1fgoogle/api/field_behavior.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a google/protobuf/field_mask.proto\x1a.protoc_gen_openapiv2/options/annotations.proto"E\n\x1cListRelationshipTypesRequest\x12\x11\n\tpage_size\x18\x01 \x01(\x05\x12\x12\n\npage_token\x18\x02 \x01(\t"\x8e\x01\n\x1dListRelationshipTypesResponse\x12@\n\x12relationship_types\x18\x01 \x03(\x0b2$.exabel.api.data.v1.RelationshipType\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\x12\x12\n\ntotal_size\x18\x03 \x01(\x05"e\n\x1dCreateRelationshipTypeRequest\x12D\n\x11relationship_type\x18\x01 \x01(\x0b2$.exabel.api.data.v1.RelationshipTypeB\x03\xe0A\x02"\xad\x01\n\x1dUpdateRelationshipTypeRequest\x12D\n\x11relationship_type\x18\x01 \x01(\x0b2$.exabel.api.data.v1.RelationshipTypeB\x03\xe0A\x02\x12/\n\x0bupdate_mask\x18\x02 \x01(\x0b2\x1a.google.protobuf.FieldMask\x12\x15\n\rallow_missing\x18\x03 \x01(\x08"O\n\x1dDeleteRelationshipTypeRequest\x12.\n\x04name\x18\x01 \x01(\tB \xe0A\x02\x92A\x1a\xca>\x17\xfa\x02\x14relationshipTypeName"L\n\x1aGetRelationshipTypeRequest\x12.\n\x04name\x18\x01 \x01(\tB \xe0A\x02\x92A\x1a\xca>\x17\xfa\x02\x14relationshipTypeName"\x9b\x01\n\x18ListRelationshipsRequest\x120\n\x06parent\x18\x01 \x01(\tB \xe0A\x02\x92A\x1a\xca>\x17\xfa\x02\x14relationshipTypeName\x12\x13\n\x0bfrom_entity\x18\x02 \x01(\t\x12\x11\n\tto_entity\x18\x03 \x01(\t\x12\x11\n\tpage_size\x18\x04 \x01(\x05\x12\x12\n\npage_token\x18\x05 \x01(\t"\x81\x01\n\x19ListRelationshipsResponse\x127\n\rrelationships\x18\x01 \x03(\x0b2 .exabel.api.data.v1.Relationship\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\x12\x12\n\ntotal_size\x18\x03 \x01(\x05"|\n\x16GetRelationshipRequest\x120\n\x06parent\x18\x01 \x01(\tB \xe0A\x02\x92A\x1a\xca>\x17\xfa\x02\x14relationshipTypeName\x12\x18\n\x0bfrom_entity\x18\x02 \x01(\tB\x03\xe0A\x02\x12\x16\n\tto_entity\x18\x03 \x01(\tB\x03\xe0A\x02"X\n\x19CreateRelationshipRequest\x12;\n\x0crelationship\x18\x01 \x01(\x0b2 .exabel.api.data.v1.RelationshipB\x03\xe0A\x02"\xa0\x01\n\x19UpdateRelationshipRequest\x12;\n\x0crelationship\x18\x01 \x01(\x0b2 .exabel.api.data.v1.RelationshipB\x03\xe0A\x02\x12/\n\x0bupdate_mask\x18\x02 \x01(\x0b2\x1a.google.protobuf.FieldMask\x12\x15\n\rallow_missing\x18\x03 \x01(\x08"\x7f\n\x19DeleteRelationshipRequest\x120\n\x06parent\x18\x01 \x01(\tB \xe0A\x02\x92A\x1a\xca>\x17\xfa\x02\x14relationshipTypeName\x12\x18\n\x0bfrom_entity\x18\x02 \x01(\tB\x03\xe0A\x02\x12\x16\n\tto_entity\x18\x03 \x01(\tB\x03\xe0A\x022\x94\x12\n\x13RelationshipService\x12\xb7\x01\n\x15ListRelationshipTypes\x120.exabel.api.data.v1.ListRelationshipTypesRequest\x1a1.exabel.api.data.v1.ListRelationshipTypesResponse"9\x82\xd3\xe4\x93\x02\x17\x12\x15/v1/relationshipTypes\x92A\x19\x12\x17List relationship types\x12\xad\x01\n\x13GetRelationshipType\x12..exabel.api.data.v1.GetRelationshipTypeRequest\x1a$.exabel.api.data.v1.RelationshipType"@\x82\xd3\xe4\x93\x02 \x12\x1e/v1/{name=relationshipTypes/*}\x92A\x17\x12\x15Get relationship type\x12\xc0\x01\n\x16CreateRelationshipType\x121.exabel.api.data.v1.CreateRelationshipTypeRequest\x1a$.exabel.api.data.v1.RelationshipType"M\x82\xd3\xe4\x93\x02*"\x15/v1/relationshipTypes:\x11relationship_type\x92A\x1a\x12\x18Create relationship type\x12\xdb\x01\n\x16UpdateRelationshipType\x121.exabel.api.data.v1.UpdateRelationshipTypeRequest\x1a$.exabel.api.data.v1.RelationshipType"h\x82\xd3\xe4\x93\x02E20/v1/{relationship_type.name=relationshipTypes/*}:\x11relationship_type\x92A\x1a\x12\x18Update relationship type\x12\xa8\x01\n\x16DeleteRelationshipType\x121.exabel.api.data.v1.DeleteRelationshipTypeRequest\x1a\x16.google.protobuf.Empty"C\x82\xd3\xe4\x93\x02 *\x1e/v1/{name=relationshipTypes/*}\x92A\x1a\x12\x18Delete relationship type\x12\xbf\x01\n\x11ListRelationships\x12,.exabel.api.data.v1.ListRelationshipsRequest\x1a-.exabel.api.data.v1.ListRelationshipsResponse"M\x82\xd3\xe4\x93\x020\x12./v1/{parent=relationshipTypes/*}/relationships\x92A\x14\x12\x12List relationships\x12\xf9\x01\n\x0fGetRelationship\x12*.exabel.api.data.v1.GetRelationshipRequest\x1a .exabel.api.data.v1.Relationship"\x97\x01\x82\xd3\xe4\x93\x02|\x12z/v1/{parent=relationshipTypes/*}/relationships/{from_entity=entityTypes/*/entities/*}/{to_entity=entityTypes/*/entities/*}\x92A\x12\x12\x10Get relationship\x12\xd0\x01\n\x12CreateRelationship\x12-.exabel.api.data.v1.CreateRelationshipRequest\x1a .exabel.api.data.v1.Relationship"i\x82\xd3\xe4\x93\x02K";/v1/{relationship.parent=relationshipTypes/*}/relationships:\x0crelationship\x92A\x15\x12\x13Create relationship\x12\x87\x03\n\x12UpdateRelationship\x12-.exabel.api.data.v1.UpdateRelationshipRequest\x1a .exabel.api.data.v1.Relationship"\x9f\x02\x82\xd3\xe4\x93\x02\x80\x022;/v1/{relationship.parent=relationshipTypes/*}/relationships:\x0crelationshipZ\xb2\x012\xa1\x01/v1/{relationship.parent=relationshipTypes/*}/relationships/{relationship.from_entity=entityTypes/*/entities/*}/{relationship.to_entity=entityTypes/*/entities/*}:\x0crelationship\x92A\x15\x12\x13Update relationship\x12\xab\x02\n\x12DeleteRelationship\x12-.exabel.api.data.v1.DeleteRelationshipRequest\x1a\x16.google.protobuf.Empty"\xcd\x01\x82\xd3\xe4\x93\x02\xae\x01*./v1/{parent=relationshipTypes/*}/relationshipsZ|*z/v1/{parent=relationshipTypes/*}/relationships/{from_entity=entityTypes/*/entities/*}/{to_entity=entityTypes/*/entities/*}\x92A\x15\x12\x13Delete relationshipBL\n\x16com.exabel.api.data.v1B\x18RelationshipServiceProtoP\x01Z\x16exabel.com/api/data/v1b\x06proto3')
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.data.v1.relationship_service_pb2', globals())
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n-exabel/api/data/v1/relationship_service.proto\x12\x12exabel.api.data.v1\x1a.exabel/api/data/v1/relationship_messages.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1fgoogle/api/field_behavior.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a google/protobuf/field_mask.proto\x1a.protoc_gen_openapiv2/options/annotations.proto"E\n\x1cListRelationshipTypesRequest\x12\x11\n\tpage_size\x18\x01 \x01(\x05\x12\x12\n\npage_token\x18\x02 \x01(\t"\x8e\x01\n\x1dListRelationshipTypesResponse\x12@\n\x12relationship_types\x18\x01 \x03(\x0b2$.exabel.api.data.v1.RelationshipType\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\x12\x12\n\ntotal_size\x18\x03 \x01(\x05"f\n\x1dCreateRelationshipTypeRequest\x12E\n\x11relationship_type\x18\x01 \x01(\x0b2$.exabel.api.data.v1.RelationshipTypeB\x04\xe2A\x01\x02"\xae\x01\n\x1dUpdateRelationshipTypeRequest\x12E\n\x11relationship_type\x18\x01 \x01(\x0b2$.exabel.api.data.v1.RelationshipTypeB\x04\xe2A\x01\x02\x12/\n\x0bupdate_mask\x18\x02 \x01(\x0b2\x1a.google.protobuf.FieldMask\x12\x15\n\rallow_missing\x18\x03 \x01(\x08"P\n\x1dDeleteRelationshipTypeRequest\x12/\n\x04name\x18\x01 \x01(\tB!\x92A\x1a\xca>\x17\xfa\x02\x14relationshipTypeName\xe2A\x01\x02"M\n\x1aGetRelationshipTypeRequest\x12/\n\x04name\x18\x01 \x01(\tB!\x92A\x1a\xca>\x17\xfa\x02\x14relationshipTypeName\xe2A\x01\x02"\x9c\x01\n\x18ListRelationshipsRequest\x121\n\x06parent\x18\x01 \x01(\tB!\x92A\x1a\xca>\x17\xfa\x02\x14relationshipTypeName\xe2A\x01\x02\x12\x13\n\x0bfrom_entity\x18\x02 \x01(\t\x12\x11\n\tto_entity\x18\x03 \x01(\t\x12\x11\n\tpage_size\x18\x04 \x01(\x05\x12\x12\n\npage_token\x18\x05 \x01(\t"\x81\x01\n\x19ListRelationshipsResponse\x127\n\rrelationships\x18\x01 \x03(\x0b2 .exabel.api.data.v1.Relationship\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\x12\x12\n\ntotal_size\x18\x03 \x01(\x05"\x7f\n\x16GetRelationshipRequest\x121\n\x06parent\x18\x01 \x01(\tB!\x92A\x1a\xca>\x17\xfa\x02\x14relationshipTypeName\xe2A\x01\x02\x12\x19\n\x0bfrom_entity\x18\x02 \x01(\tB\x04\xe2A\x01\x02\x12\x17\n\tto_entity\x18\x03 \x01(\tB\x04\xe2A\x01\x02"Y\n\x19CreateRelationshipRequest\x12<\n\x0crelationship\x18\x01 \x01(\x0b2 .exabel.api.data.v1.RelationshipB\x04\xe2A\x01\x02"\xa1\x01\n\x19UpdateRelationshipRequest\x12<\n\x0crelationship\x18\x01 \x01(\x0b2 .exabel.api.data.v1.RelationshipB\x04\xe2A\x01\x02\x12/\n\x0bupdate_mask\x18\x02 \x01(\x0b2\x1a.google.protobuf.FieldMask\x12\x15\n\rallow_missing\x18\x03 \x01(\x08"\x82\x01\n\x19DeleteRelationshipRequest\x121\n\x06parent\x18\x01 \x01(\tB!\x92A\x1a\xca>\x17\xfa\x02\x14relationshipTypeName\xe2A\x01\x02\x12\x19\n\x0bfrom_entity\x18\x02 \x01(\tB\x04\xe2A\x01\x02\x12\x17\n\tto_entity\x18\x03 \x01(\tB\x04\xe2A\x01\x022\x94\x12\n\x13RelationshipService\x12\xb7\x01\n\x15ListRelationshipTypes\x120.exabel.api.data.v1.ListRelationshipTypesRequest\x1a1.exabel.api.data.v1.ListRelationshipTypesResponse"9\x92A\x19\x12\x17List relationship types\x82\xd3\xe4\x93\x02\x17\x12\x15/v1/relationshipTypes\x12\xad\x01\n\x13GetRelationshipType\x12..exabel.api.data.v1.GetRelationshipTypeRequest\x1a$.exabel.api.data.v1.RelationshipType"@\x92A\x17\x12\x15Get relationship type\x82\xd3\xe4\x93\x02 \x12\x1e/v1/{name=relationshipTypes/*}\x12\xc0\x01\n\x16CreateRelationshipType\x121.exabel.api.data.v1.CreateRelationshipTypeRequest\x1a$.exabel.api.data.v1.RelationshipType"M\x92A\x1a\x12\x18Create relationship type\x82\xd3\xe4\x93\x02*"\x15/v1/relationshipTypes:\x11relationship_type\x12\xdb\x01\n\x16UpdateRelationshipType\x121.exabel.api.data.v1.UpdateRelationshipTypeRequest\x1a$.exabel.api.data.v1.RelationshipType"h\x92A\x1a\x12\x18Update relationship type\x82\xd3\xe4\x93\x02E20/v1/{relationship_type.name=relationshipTypes/*}:\x11relationship_type\x12\xa8\x01\n\x16DeleteRelationshipType\x121.exabel.api.data.v1.DeleteRelationshipTypeRequest\x1a\x16.google.protobuf.Empty"C\x92A\x1a\x12\x18Delete relationship type\x82\xd3\xe4\x93\x02 *\x1e/v1/{name=relationshipTypes/*}\x12\xbf\x01\n\x11ListRelationships\x12,.exabel.api.data.v1.ListRelationshipsRequest\x1a-.exabel.api.data.v1.ListRelationshipsResponse"M\x92A\x14\x12\x12List relationships\x82\xd3\xe4\x93\x020\x12./v1/{parent=relationshipTypes/*}/relationships\x12\xf9\x01\n\x0fGetRelationship\x12*.exabel.api.data.v1.GetRelationshipRequest\x1a .exabel.api.data.v1.Relationship"\x97\x01\x92A\x12\x12\x10Get relationship\x82\xd3\xe4\x93\x02|\x12z/v1/{parent=relationshipTypes/*}/relationships/{from_entity=entityTypes/*/entities/*}/{to_entity=entityTypes/*/entities/*}\x12\xd0\x01\n\x12CreateRelationship\x12-.exabel.api.data.v1.CreateRelationshipRequest\x1a .exabel.api.data.v1.Relationship"i\x92A\x15\x12\x13Create relationship\x82\xd3\xe4\x93\x02K";/v1/{relationship.parent=relationshipTypes/*}/relationships:\x0crelationship\x12\x87\x03\n\x12UpdateRelationship\x12-.exabel.api.data.v1.UpdateRelationshipRequest\x1a .exabel.api.data.v1.Relationship"\x9f\x02\x92A\x15\x12\x13Update relationship\x82\xd3\xe4\x93\x02\x80\x022;/v1/{relationship.parent=relationshipTypes/*}/relationships:\x0crelationshipZ\xb2\x012\xa1\x01/v1/{relationship.parent=relationshipTypes/*}/relationships/{relationship.from_entity=entityTypes/*/entities/*}/{relationship.to_entity=entityTypes/*/entities/*}:\x0crelationship\x12\xab\x02\n\x12DeleteRelationship\x12-.exabel.api.data.v1.DeleteRelationshipRequest\x1a\x16.google.protobuf.Empty"\xcd\x01\x92A\x15\x12\x13Delete relationship\x82\xd3\xe4\x93\x02\xae\x01*./v1/{parent=relationshipTypes/*}/relationshipsZ|*z/v1/{parent=relationshipTypes/*}/relationships/{from_entity=entityTypes/*/entities/*}/{to_entity=entityTypes/*/entities/*}BL\n\x16com.exabel.api.data.v1B\x18RelationshipServiceProtoP\x01Z\x16exabel.com/api/data/v1b\x06proto3')
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.data.v1.relationship_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b'\n\x16com.exabel.api.data.v1B\x18RelationshipServiceProtoP\x01Z\x16exabel.com/api/data/v1'
     _CREATERELATIONSHIPTYPEREQUEST.fields_by_name['relationship_type']._options = None
-    _CREATERELATIONSHIPTYPEREQUEST.fields_by_name['relationship_type']._serialized_options = b'\xe0A\x02'
+    _CREATERELATIONSHIPTYPEREQUEST.fields_by_name['relationship_type']._serialized_options = b'\xe2A\x01\x02'
     _UPDATERELATIONSHIPTYPEREQUEST.fields_by_name['relationship_type']._options = None
-    _UPDATERELATIONSHIPTYPEREQUEST.fields_by_name['relationship_type']._serialized_options = b'\xe0A\x02'
+    _UPDATERELATIONSHIPTYPEREQUEST.fields_by_name['relationship_type']._serialized_options = b'\xe2A\x01\x02'
     _DELETERELATIONSHIPTYPEREQUEST.fields_by_name['name']._options = None
-    _DELETERELATIONSHIPTYPEREQUEST.fields_by_name['name']._serialized_options = b'\xe0A\x02\x92A\x1a\xca>\x17\xfa\x02\x14relationshipTypeName'
+    _DELETERELATIONSHIPTYPEREQUEST.fields_by_name['name']._serialized_options = b'\x92A\x1a\xca>\x17\xfa\x02\x14relationshipTypeName\xe2A\x01\x02'
     _GETRELATIONSHIPTYPEREQUEST.fields_by_name['name']._options = None
-    _GETRELATIONSHIPTYPEREQUEST.fields_by_name['name']._serialized_options = b'\xe0A\x02\x92A\x1a\xca>\x17\xfa\x02\x14relationshipTypeName'
+    _GETRELATIONSHIPTYPEREQUEST.fields_by_name['name']._serialized_options = b'\x92A\x1a\xca>\x17\xfa\x02\x14relationshipTypeName\xe2A\x01\x02'
     _LISTRELATIONSHIPSREQUEST.fields_by_name['parent']._options = None
-    _LISTRELATIONSHIPSREQUEST.fields_by_name['parent']._serialized_options = b'\xe0A\x02\x92A\x1a\xca>\x17\xfa\x02\x14relationshipTypeName'
+    _LISTRELATIONSHIPSREQUEST.fields_by_name['parent']._serialized_options = b'\x92A\x1a\xca>\x17\xfa\x02\x14relationshipTypeName\xe2A\x01\x02'
     _GETRELATIONSHIPREQUEST.fields_by_name['parent']._options = None
-    _GETRELATIONSHIPREQUEST.fields_by_name['parent']._serialized_options = b'\xe0A\x02\x92A\x1a\xca>\x17\xfa\x02\x14relationshipTypeName'
+    _GETRELATIONSHIPREQUEST.fields_by_name['parent']._serialized_options = b'\x92A\x1a\xca>\x17\xfa\x02\x14relationshipTypeName\xe2A\x01\x02'
     _GETRELATIONSHIPREQUEST.fields_by_name['from_entity']._options = None
-    _GETRELATIONSHIPREQUEST.fields_by_name['from_entity']._serialized_options = b'\xe0A\x02'
+    _GETRELATIONSHIPREQUEST.fields_by_name['from_entity']._serialized_options = b'\xe2A\x01\x02'
     _GETRELATIONSHIPREQUEST.fields_by_name['to_entity']._options = None
-    _GETRELATIONSHIPREQUEST.fields_by_name['to_entity']._serialized_options = b'\xe0A\x02'
+    _GETRELATIONSHIPREQUEST.fields_by_name['to_entity']._serialized_options = b'\xe2A\x01\x02'
     _CREATERELATIONSHIPREQUEST.fields_by_name['relationship']._options = None
-    _CREATERELATIONSHIPREQUEST.fields_by_name['relationship']._serialized_options = b'\xe0A\x02'
+    _CREATERELATIONSHIPREQUEST.fields_by_name['relationship']._serialized_options = b'\xe2A\x01\x02'
     _UPDATERELATIONSHIPREQUEST.fields_by_name['relationship']._options = None
-    _UPDATERELATIONSHIPREQUEST.fields_by_name['relationship']._serialized_options = b'\xe0A\x02'
+    _UPDATERELATIONSHIPREQUEST.fields_by_name['relationship']._serialized_options = b'\xe2A\x01\x02'
     _DELETERELATIONSHIPREQUEST.fields_by_name['parent']._options = None
-    _DELETERELATIONSHIPREQUEST.fields_by_name['parent']._serialized_options = b'\xe0A\x02\x92A\x1a\xca>\x17\xfa\x02\x14relationshipTypeName'
+    _DELETERELATIONSHIPREQUEST.fields_by_name['parent']._serialized_options = b'\x92A\x1a\xca>\x17\xfa\x02\x14relationshipTypeName\xe2A\x01\x02'
     _DELETERELATIONSHIPREQUEST.fields_by_name['from_entity']._options = None
-    _DELETERELATIONSHIPREQUEST.fields_by_name['from_entity']._serialized_options = b'\xe0A\x02'
+    _DELETERELATIONSHIPREQUEST.fields_by_name['from_entity']._serialized_options = b'\xe2A\x01\x02'
     _DELETERELATIONSHIPREQUEST.fields_by_name['to_entity']._options = None
-    _DELETERELATIONSHIPREQUEST.fields_by_name['to_entity']._serialized_options = b'\xe0A\x02'
+    _DELETERELATIONSHIPREQUEST.fields_by_name['to_entity']._serialized_options = b'\xe2A\x01\x02'
     _RELATIONSHIPSERVICE.methods_by_name['ListRelationshipTypes']._options = None
-    _RELATIONSHIPSERVICE.methods_by_name['ListRelationshipTypes']._serialized_options = b'\x82\xd3\xe4\x93\x02\x17\x12\x15/v1/relationshipTypes\x92A\x19\x12\x17List relationship types'
+    _RELATIONSHIPSERVICE.methods_by_name['ListRelationshipTypes']._serialized_options = b'\x92A\x19\x12\x17List relationship types\x82\xd3\xe4\x93\x02\x17\x12\x15/v1/relationshipTypes'
     _RELATIONSHIPSERVICE.methods_by_name['GetRelationshipType']._options = None
-    _RELATIONSHIPSERVICE.methods_by_name['GetRelationshipType']._serialized_options = b'\x82\xd3\xe4\x93\x02 \x12\x1e/v1/{name=relationshipTypes/*}\x92A\x17\x12\x15Get relationship type'
+    _RELATIONSHIPSERVICE.methods_by_name['GetRelationshipType']._serialized_options = b'\x92A\x17\x12\x15Get relationship type\x82\xd3\xe4\x93\x02 \x12\x1e/v1/{name=relationshipTypes/*}'
     _RELATIONSHIPSERVICE.methods_by_name['CreateRelationshipType']._options = None
-    _RELATIONSHIPSERVICE.methods_by_name['CreateRelationshipType']._serialized_options = b'\x82\xd3\xe4\x93\x02*"\x15/v1/relationshipTypes:\x11relationship_type\x92A\x1a\x12\x18Create relationship type'
+    _RELATIONSHIPSERVICE.methods_by_name['CreateRelationshipType']._serialized_options = b'\x92A\x1a\x12\x18Create relationship type\x82\xd3\xe4\x93\x02*"\x15/v1/relationshipTypes:\x11relationship_type'
     _RELATIONSHIPSERVICE.methods_by_name['UpdateRelationshipType']._options = None
-    _RELATIONSHIPSERVICE.methods_by_name['UpdateRelationshipType']._serialized_options = b'\x82\xd3\xe4\x93\x02E20/v1/{relationship_type.name=relationshipTypes/*}:\x11relationship_type\x92A\x1a\x12\x18Update relationship type'
+    _RELATIONSHIPSERVICE.methods_by_name['UpdateRelationshipType']._serialized_options = b'\x92A\x1a\x12\x18Update relationship type\x82\xd3\xe4\x93\x02E20/v1/{relationship_type.name=relationshipTypes/*}:\x11relationship_type'
     _RELATIONSHIPSERVICE.methods_by_name['DeleteRelationshipType']._options = None
-    _RELATIONSHIPSERVICE.methods_by_name['DeleteRelationshipType']._serialized_options = b'\x82\xd3\xe4\x93\x02 *\x1e/v1/{name=relationshipTypes/*}\x92A\x1a\x12\x18Delete relationship type'
+    _RELATIONSHIPSERVICE.methods_by_name['DeleteRelationshipType']._serialized_options = b'\x92A\x1a\x12\x18Delete relationship type\x82\xd3\xe4\x93\x02 *\x1e/v1/{name=relationshipTypes/*}'
     _RELATIONSHIPSERVICE.methods_by_name['ListRelationships']._options = None
-    _RELATIONSHIPSERVICE.methods_by_name['ListRelationships']._serialized_options = b'\x82\xd3\xe4\x93\x020\x12./v1/{parent=relationshipTypes/*}/relationships\x92A\x14\x12\x12List relationships'
+    _RELATIONSHIPSERVICE.methods_by_name['ListRelationships']._serialized_options = b'\x92A\x14\x12\x12List relationships\x82\xd3\xe4\x93\x020\x12./v1/{parent=relationshipTypes/*}/relationships'
     _RELATIONSHIPSERVICE.methods_by_name['GetRelationship']._options = None
-    _RELATIONSHIPSERVICE.methods_by_name['GetRelationship']._serialized_options = b'\x82\xd3\xe4\x93\x02|\x12z/v1/{parent=relationshipTypes/*}/relationships/{from_entity=entityTypes/*/entities/*}/{to_entity=entityTypes/*/entities/*}\x92A\x12\x12\x10Get relationship'
+    _RELATIONSHIPSERVICE.methods_by_name['GetRelationship']._serialized_options = b'\x92A\x12\x12\x10Get relationship\x82\xd3\xe4\x93\x02|\x12z/v1/{parent=relationshipTypes/*}/relationships/{from_entity=entityTypes/*/entities/*}/{to_entity=entityTypes/*/entities/*}'
     _RELATIONSHIPSERVICE.methods_by_name['CreateRelationship']._options = None
-    _RELATIONSHIPSERVICE.methods_by_name['CreateRelationship']._serialized_options = b'\x82\xd3\xe4\x93\x02K";/v1/{relationship.parent=relationshipTypes/*}/relationships:\x0crelationship\x92A\x15\x12\x13Create relationship'
+    _RELATIONSHIPSERVICE.methods_by_name['CreateRelationship']._serialized_options = b'\x92A\x15\x12\x13Create relationship\x82\xd3\xe4\x93\x02K";/v1/{relationship.parent=relationshipTypes/*}/relationships:\x0crelationship'
     _RELATIONSHIPSERVICE.methods_by_name['UpdateRelationship']._options = None
-    _RELATIONSHIPSERVICE.methods_by_name['UpdateRelationship']._serialized_options = b'\x82\xd3\xe4\x93\x02\x80\x022;/v1/{relationship.parent=relationshipTypes/*}/relationships:\x0crelationshipZ\xb2\x012\xa1\x01/v1/{relationship.parent=relationshipTypes/*}/relationships/{relationship.from_entity=entityTypes/*/entities/*}/{relationship.to_entity=entityTypes/*/entities/*}:\x0crelationship\x92A\x15\x12\x13Update relationship'
+    _RELATIONSHIPSERVICE.methods_by_name['UpdateRelationship']._serialized_options = b'\x92A\x15\x12\x13Update relationship\x82\xd3\xe4\x93\x02\x80\x022;/v1/{relationship.parent=relationshipTypes/*}/relationships:\x0crelationshipZ\xb2\x012\xa1\x01/v1/{relationship.parent=relationshipTypes/*}/relationships/{relationship.from_entity=entityTypes/*/entities/*}/{relationship.to_entity=entityTypes/*/entities/*}:\x0crelationship'
     _RELATIONSHIPSERVICE.methods_by_name['DeleteRelationship']._options = None
-    _RELATIONSHIPSERVICE.methods_by_name['DeleteRelationship']._serialized_options = b'\x82\xd3\xe4\x93\x02\xae\x01*./v1/{parent=relationshipTypes/*}/relationshipsZ|*z/v1/{parent=relationshipTypes/*}/relationships/{from_entity=entityTypes/*/entities/*}/{to_entity=entityTypes/*/entities/*}\x92A\x15\x12\x13Delete relationship'
-    _LISTRELATIONSHIPTYPESREQUEST._serialized_start = 291
-    _LISTRELATIONSHIPTYPESREQUEST._serialized_end = 360
-    _LISTRELATIONSHIPTYPESRESPONSE._serialized_start = 363
-    _LISTRELATIONSHIPTYPESRESPONSE._serialized_end = 505
-    _CREATERELATIONSHIPTYPEREQUEST._serialized_start = 507
-    _CREATERELATIONSHIPTYPEREQUEST._serialized_end = 608
-    _UPDATERELATIONSHIPTYPEREQUEST._serialized_start = 611
-    _UPDATERELATIONSHIPTYPEREQUEST._serialized_end = 784
-    _DELETERELATIONSHIPTYPEREQUEST._serialized_start = 786
-    _DELETERELATIONSHIPTYPEREQUEST._serialized_end = 865
-    _GETRELATIONSHIPTYPEREQUEST._serialized_start = 867
-    _GETRELATIONSHIPTYPEREQUEST._serialized_end = 943
-    _LISTRELATIONSHIPSREQUEST._serialized_start = 946
-    _LISTRELATIONSHIPSREQUEST._serialized_end = 1101
-    _LISTRELATIONSHIPSRESPONSE._serialized_start = 1104
-    _LISTRELATIONSHIPSRESPONSE._serialized_end = 1233
-    _GETRELATIONSHIPREQUEST._serialized_start = 1235
-    _GETRELATIONSHIPREQUEST._serialized_end = 1359
-    _CREATERELATIONSHIPREQUEST._serialized_start = 1361
-    _CREATERELATIONSHIPREQUEST._serialized_end = 1449
-    _UPDATERELATIONSHIPREQUEST._serialized_start = 1452
-    _UPDATERELATIONSHIPREQUEST._serialized_end = 1612
-    _DELETERELATIONSHIPREQUEST._serialized_start = 1614
-    _DELETERELATIONSHIPREQUEST._serialized_end = 1741
-    _RELATIONSHIPSERVICE._serialized_start = 1744
-    _RELATIONSHIPSERVICE._serialized_end = 4068
+    _RELATIONSHIPSERVICE.methods_by_name['DeleteRelationship']._serialized_options = b'\x92A\x15\x12\x13Delete relationship\x82\xd3\xe4\x93\x02\xae\x01*./v1/{parent=relationshipTypes/*}/relationshipsZ|*z/v1/{parent=relationshipTypes/*}/relationships/{from_entity=entityTypes/*/entities/*}/{to_entity=entityTypes/*/entities/*}'
+    _globals['_LISTRELATIONSHIPTYPESREQUEST']._serialized_start = 291
+    _globals['_LISTRELATIONSHIPTYPESREQUEST']._serialized_end = 360
+    _globals['_LISTRELATIONSHIPTYPESRESPONSE']._serialized_start = 363
+    _globals['_LISTRELATIONSHIPTYPESRESPONSE']._serialized_end = 505
+    _globals['_CREATERELATIONSHIPTYPEREQUEST']._serialized_start = 507
+    _globals['_CREATERELATIONSHIPTYPEREQUEST']._serialized_end = 609
+    _globals['_UPDATERELATIONSHIPTYPEREQUEST']._serialized_start = 612
+    _globals['_UPDATERELATIONSHIPTYPEREQUEST']._serialized_end = 786
+    _globals['_DELETERELATIONSHIPTYPEREQUEST']._serialized_start = 788
+    _globals['_DELETERELATIONSHIPTYPEREQUEST']._serialized_end = 868
+    _globals['_GETRELATIONSHIPTYPEREQUEST']._serialized_start = 870
+    _globals['_GETRELATIONSHIPTYPEREQUEST']._serialized_end = 947
+    _globals['_LISTRELATIONSHIPSREQUEST']._serialized_start = 950
+    _globals['_LISTRELATIONSHIPSREQUEST']._serialized_end = 1106
+    _globals['_LISTRELATIONSHIPSRESPONSE']._serialized_start = 1109
+    _globals['_LISTRELATIONSHIPSRESPONSE']._serialized_end = 1238
+    _globals['_GETRELATIONSHIPREQUEST']._serialized_start = 1240
+    _globals['_GETRELATIONSHIPREQUEST']._serialized_end = 1367
+    _globals['_CREATERELATIONSHIPREQUEST']._serialized_start = 1369
+    _globals['_CREATERELATIONSHIPREQUEST']._serialized_end = 1458
+    _globals['_UPDATERELATIONSHIPREQUEST']._serialized_start = 1461
+    _globals['_UPDATERELATIONSHIPREQUEST']._serialized_end = 1622
+    _globals['_DELETERELATIONSHIPREQUEST']._serialized_start = 1625
+    _globals['_DELETERELATIONSHIPREQUEST']._serialized_end = 1755
+    _globals['_RELATIONSHIPSERVICE']._serialized_start = 1758
+    _globals['_RELATIONSHIPSERVICE']._serialized_end = 4082
```

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_service_pb2_grpc.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/data/v1/search_messages_pb2.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/data/v1/search_messages_pb2.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 _sym_db = _symbol_database.Default()
 from google.api import field_behavior_pb2 as google_dot_api_dot_field__behavior__pb2
 from .....protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(exabel/api/data/v1/search_messages.proto\x12\x12exabel.api.data.v1\x1a\x1fgoogle/api/field_behavior.proto\x1a.protoc_gen_openapiv2/options/annotations.proto"O\n\nSearchTerm\x12\x1d\n\x05field\x18\x01 \x01(\tB\x0e\xe0A\x02\x92A\x08J\x06"text"\x12"\n\x05query\x18\x02 \x01(\tB\x13\xe0A\x02\x92A\rJ\x0b"microsoft""E\n\rSearchOptions\x124\n\x08universe\x18\x01 \x01(\x0e2".exabel.api.data.v1.SearchUniverse*Z\n\x0eSearchUniverse\x12\x1f\n\x1bSEARCH_UNIVERSE_UNSPECIFIED\x10\x00\x12\x14\n\x10EXABEL_COMPANIES\x10\x01\x12\x11\n\rALL_COMPANIES\x10\x02BG\n\x16com.exabel.api.data.v1B\x13SearchMessagesProtoP\x01Z\x16exabel.com/api/data/v1b\x06proto3')
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.data.v1.search_messages_pb2', globals())
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(exabel/api/data/v1/search_messages.proto\x12\x12exabel.api.data.v1\x1a\x1fgoogle/api/field_behavior.proto\x1a.protoc_gen_openapiv2/options/annotations.proto"Q\n\nSearchTerm\x12\x1e\n\x05field\x18\x01 \x01(\tB\x0f\x92A\x08J\x06"text"\xe2A\x01\x02\x12#\n\x05query\x18\x02 \x01(\tB\x14\x92A\rJ\x0b"microsoft"\xe2A\x01\x02"E\n\rSearchOptions\x124\n\x08universe\x18\x01 \x01(\x0e2".exabel.api.data.v1.SearchUniverse*Z\n\x0eSearchUniverse\x12\x1f\n\x1bSEARCH_UNIVERSE_UNSPECIFIED\x10\x00\x12\x14\n\x10EXABEL_COMPANIES\x10\x01\x12\x11\n\rALL_COMPANIES\x10\x02BG\n\x16com.exabel.api.data.v1B\x13SearchMessagesProtoP\x01Z\x16exabel.com/api/data/v1b\x06proto3')
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.data.v1.search_messages_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b'\n\x16com.exabel.api.data.v1B\x13SearchMessagesProtoP\x01Z\x16exabel.com/api/data/v1'
     _SEARCHTERM.fields_by_name['field']._options = None
-    _SEARCHTERM.fields_by_name['field']._serialized_options = b'\xe0A\x02\x92A\x08J\x06"text"'
+    _SEARCHTERM.fields_by_name['field']._serialized_options = b'\x92A\x08J\x06"text"\xe2A\x01\x02'
     _SEARCHTERM.fields_by_name['query']._options = None
-    _SEARCHTERM.fields_by_name['query']._serialized_options = b'\xe0A\x02\x92A\rJ\x0b"microsoft"'
-    _SEARCHUNIVERSE._serialized_start = 297
-    _SEARCHUNIVERSE._serialized_end = 387
-    _SEARCHTERM._serialized_start = 145
-    _SEARCHTERM._serialized_end = 224
-    _SEARCHOPTIONS._serialized_start = 226
-    _SEARCHOPTIONS._serialized_end = 295
+    _SEARCHTERM.fields_by_name['query']._serialized_options = b'\x92A\rJ\x0b"microsoft"\xe2A\x01\x02'
+    _globals['_SEARCHUNIVERSE']._serialized_start = 299
+    _globals['_SEARCHUNIVERSE']._serialized_end = 389
+    _globals['_SEARCHTERM']._serialized_start = 145
+    _globals['_SEARCHTERM']._serialized_end = 226
+    _globals['_SEARCHOPTIONS']._serialized_start = 228
+    _globals['_SEARCHOPTIONS']._serialized_end = 297
```

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/data/v1/service_pb2.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/data/v1/service_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 _sym_db = _symbol_database.Default()
 from .....protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n exabel/api/data/v1/service.proto\x12\x12exabel.api.data.v1\x1a.protoc_gen_openapiv2/options/annotations.protoB\xc8\x02\n\x16com.exabel.api.data.v1B\x0cServiceProtoP\x01Z\x16exabel.com/api/data/v1\x92A\x84\x02\x12P\n\x0fExabel Data API"5\n\x06Exabel\x12\x17https://www.exabel.com/\x1a\x12support@exabel.com2\x061.0.25\x1a\x13data.api.exabel.com*\x01\x022\x10application/json:\x10application/jsonZ\x1c\n\x1a\n\x07API key\x12\x0f\x08\x02\x1a\tx-api-key \x02b\r\n\x0b\n\x07API key\x12\x00rG\n\x1eMore about the Exabel Data API\x12%https://help.exabel.com/docs/data-apib\x06proto3')
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.data.v1.service_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.data.v1.service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b'\n\x16com.exabel.api.data.v1B\x0cServiceProtoP\x01Z\x16exabel.com/api/data/v1\x92A\x84\x02\x12P\n\x0fExabel Data API"5\n\x06Exabel\x12\x17https://www.exabel.com/\x1a\x12support@exabel.com2\x061.0.25\x1a\x13data.api.exabel.com*\x01\x022\x10application/json:\x10application/jsonZ\x1c\n\x1a\n\x07API key\x12\x0f\x08\x02\x1a\tx-api-key \x02b\r\n\x0b\n\x07API key\x12\x00rG\n\x1eMore about the Exabel Data API\x12%https://help.exabel.com/docs/data-api'
```

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_messages_pb2.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_messages_pb2.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 _sym_db = _symbol_database.Default()
 from .....exabel.api.math import aggregation_pb2 as exabel_dot_api_dot_math_dot_aggregation__pb2
 from google.api import field_behavior_pb2 as google_dot_api_dot_field__behavior__pb2
 from .....protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(exabel/api/data/v1/signal_messages.proto\x12\x12exabel.api.data.v1\x1a!exabel/api/math/aggregation.proto\x1a\x1fgoogle/api/field_behavior.proto\x1a.protoc_gen_openapiv2/options/annotations.proto"\xdb\x02\n\x06Signal\x12<\n\x04name\x18\x01 \x01(\tB.\xe0A\x05\xe0A\x02\x92A%J\x13"signals/ns.signal"\xca>\r\xfa\x02\nsignalName\x12\x17\n\x0bentity_type\x18\x02 \x01(\tB\x02\x18\x01\x12&\n\x0cdisplay_name\x18\x03 \x01(\tB\x10\x92A\rJ\x0b"My signal"\x12/\n\x0bdescription\x18\x04 \x01(\tB\x1a\x92A\x17J\x15"Describes my signal"\x129\n\x13downsampling_method\x18\x05 \x01(\x0e2\x1c.exabel.api.math.Aggregation\x12\x16\n\tread_only\x18\x06 \x01(\x08B\x03\xe0A\x03\x12N\n\x0centity_types\x18\x07 \x03(\tB8\xe0A\x03\x92A2J0["entityTypes/ns.type1", "entityTypes/ns.type2"]BG\n\x16com.exabel.api.data.v1B\x13SignalMessagesProtoP\x01Z\x16exabel.com/api/data/v1b\x06proto3')
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.data.v1.signal_messages_pb2', globals())
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(exabel/api/data/v1/signal_messages.proto\x12\x12exabel.api.data.v1\x1a!exabel/api/math/aggregation.proto\x1a\x1fgoogle/api/field_behavior.proto\x1a.protoc_gen_openapiv2/options/annotations.proto"\xdc\x02\n\x06Signal\x12;\n\x04name\x18\x01 \x01(\tB-\x92A%J\x13"signals/ns.signal"\xca>\r\xfa\x02\nsignalName\xe2A\x02\x05\x02\x12\x17\n\x0bentity_type\x18\x02 \x01(\tB\x02\x18\x01\x12&\n\x0cdisplay_name\x18\x03 \x01(\tB\x10\x92A\rJ\x0b"My signal"\x12/\n\x0bdescription\x18\x04 \x01(\tB\x1a\x92A\x17J\x15"Describes my signal"\x129\n\x13downsampling_method\x18\x05 \x01(\x0e2\x1c.exabel.api.math.Aggregation\x12\x17\n\tread_only\x18\x06 \x01(\x08B\x04\xe2A\x01\x03\x12O\n\x0centity_types\x18\x07 \x03(\tB9\x92A2J0["entityTypes/ns.type1", "entityTypes/ns.type2"]\xe2A\x01\x03BG\n\x16com.exabel.api.data.v1B\x13SignalMessagesProtoP\x01Z\x16exabel.com/api/data/v1b\x06proto3')
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.data.v1.signal_messages_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b'\n\x16com.exabel.api.data.v1B\x13SignalMessagesProtoP\x01Z\x16exabel.com/api/data/v1'
     _SIGNAL.fields_by_name['name']._options = None
-    _SIGNAL.fields_by_name['name']._serialized_options = b'\xe0A\x05\xe0A\x02\x92A%J\x13"signals/ns.signal"\xca>\r\xfa\x02\nsignalName'
+    _SIGNAL.fields_by_name['name']._serialized_options = b'\x92A%J\x13"signals/ns.signal"\xca>\r\xfa\x02\nsignalName\xe2A\x02\x05\x02'
     _SIGNAL.fields_by_name['entity_type']._options = None
     _SIGNAL.fields_by_name['entity_type']._serialized_options = b'\x18\x01'
     _SIGNAL.fields_by_name['display_name']._options = None
     _SIGNAL.fields_by_name['display_name']._serialized_options = b'\x92A\rJ\x0b"My signal"'
     _SIGNAL.fields_by_name['description']._options = None
     _SIGNAL.fields_by_name['description']._serialized_options = b'\x92A\x17J\x15"Describes my signal"'
     _SIGNAL.fields_by_name['read_only']._options = None
-    _SIGNAL.fields_by_name['read_only']._serialized_options = b'\xe0A\x03'
+    _SIGNAL.fields_by_name['read_only']._serialized_options = b'\xe2A\x01\x03'
     _SIGNAL.fields_by_name['entity_types']._options = None
-    _SIGNAL.fields_by_name['entity_types']._serialized_options = b'\xe0A\x03\x92A2J0["entityTypes/ns.type1", "entityTypes/ns.type2"]'
-    _SIGNAL._serialized_start = 181
-    _SIGNAL._serialized_end = 528
+    _SIGNAL.fields_by_name['entity_types']._serialized_options = b'\x92A2J0["entityTypes/ns.type1", "entityTypes/ns.type2"]\xe2A\x01\x03'
+    _globals['_SIGNAL']._serialized_start = 181
+    _globals['_SIGNAL']._serialized_end = 529
```

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_service_pb2.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_service_pb2.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,51 @@
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 _sym_db = _symbol_database.Default()
 from .....exabel.api.data.v1 import signal_messages_pb2 as exabel_dot_api_dot_data_dot_v1_dot_signal__messages__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from google.api import field_behavior_pb2 as google_dot_api_dot_field__behavior__pb2
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 from google.protobuf import field_mask_pb2 as google_dot_protobuf_dot_field__mask__pb2
 from .....protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\'exabel/api/data/v1/signal_service.proto\x12\x12exabel.api.data.v1\x1a(exabel/api/data/v1/signal_messages.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1fgoogle/api/field_behavior.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a google/protobuf/field_mask.proto\x1a.protoc_gen_openapiv2/options/annotations.proto";\n\x12ListSignalsRequest\x12\x11\n\tpage_size\x18\x01 \x01(\x05\x12\x12\n\npage_token\x18\x02 \x01(\t"o\n\x13ListSignalsResponse\x12+\n\x07signals\x18\x01 \x03(\x0b2\x1a.exabel.api.data.v1.Signal\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\x12\x12\n\ntotal_size\x18\x03 \x01(\x05"8\n\x10GetSignalRequest\x12$\n\x04name\x18\x01 \x01(\tB\x16\xe0A\x02\x92A\x10\xca>\r\xfa\x02\nsignalName"e\n\x13CreateSignalRequest\x12/\n\x06signal\x18\x01 \x01(\x0b2\x1a.exabel.api.data.v1.SignalB\x03\xe0A\x02\x12\x1d\n\x15create_library_signal\x18\x02 \x01(\x08"\xad\x01\n\x13UpdateSignalRequest\x12/\n\x06signal\x18\x01 \x01(\x0b2\x1a.exabel.api.data.v1.SignalB\x03\xe0A\x02\x12/\n\x0bupdate_mask\x18\x02 \x01(\x0b2\x1a.google.protobuf.FieldMask\x12\x15\n\rallow_missing\x18\x03 \x01(\x08\x12\x1d\n\x15create_library_signal\x18\x04 \x01(\x08";\n\x13DeleteSignalRequest\x12$\n\x04name\x18\x01 \x01(\tB\x16\xe0A\x02\x92A\x10\xca>\r\xfa\x02\nsignalName2\xad\x05\n\rSignalService\x12\x84\x01\n\x0bListSignals\x12&.exabel.api.data.v1.ListSignalsRequest\x1a\'.exabel.api.data.v1.ListSignalsResponse"$\x82\xd3\xe4\x93\x02\r\x12\x0b/v1/signals\x92A\x0e\x12\x0cList signals\x12z\n\tGetSignal\x12$.exabel.api.data.v1.GetSignalRequest\x1a\x1a.exabel.api.data.v1.Signal"+\x82\xd3\xe4\x93\x02\x16\x12\x14/v1/{name=signals/*}\x92A\x0c\x12\nGet signal\x12\x82\x01\n\x0cCreateSignal\x12\'.exabel.api.data.v1.CreateSignalRequest\x1a\x1a.exabel.api.data.v1.Signal"-\x82\xd3\xe4\x93\x02\x15"\x0b/v1/signals:\x06signal\x92A\x0f\x12\rCreate signal\x12\x92\x01\n\x0cUpdateSignal\x12\'.exabel.api.data.v1.UpdateSignalRequest\x1a\x1a.exabel.api.data.v1.Signal"=\x82\xd3\xe4\x93\x02%2\x1b/v1/{signal.name=signals/*}:\x06signal\x92A\x0f\x12\rUpdate signal\x12\x7f\n\x0cDeleteSignal\x12\'.exabel.api.data.v1.DeleteSignalRequest\x1a\x16.google.protobuf.Empty".\x82\xd3\xe4\x93\x02\x16*\x14/v1/{name=signals/*}\x92A\x0f\x12\rDelete signalBF\n\x16com.exabel.api.data.v1B\x12SignalServiceProtoP\x01Z\x16exabel.com/api/data/v1b\x06proto3')
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.data.v1.signal_service_pb2', globals())
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\'exabel/api/data/v1/signal_service.proto\x12\x12exabel.api.data.v1\x1a(exabel/api/data/v1/signal_messages.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1fgoogle/api/field_behavior.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a google/protobuf/field_mask.proto\x1a.protoc_gen_openapiv2/options/annotations.proto";\n\x12ListSignalsRequest\x12\x11\n\tpage_size\x18\x01 \x01(\x05\x12\x12\n\npage_token\x18\x02 \x01(\t"o\n\x13ListSignalsResponse\x12+\n\x07signals\x18\x01 \x03(\x0b2\x1a.exabel.api.data.v1.Signal\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\x12\x12\n\ntotal_size\x18\x03 \x01(\x05"9\n\x10GetSignalRequest\x12%\n\x04name\x18\x01 \x01(\tB\x17\x92A\x10\xca>\r\xfa\x02\nsignalName\xe2A\x01\x02"f\n\x13CreateSignalRequest\x120\n\x06signal\x18\x01 \x01(\x0b2\x1a.exabel.api.data.v1.SignalB\x04\xe2A\x01\x02\x12\x1d\n\x15create_library_signal\x18\x02 \x01(\x08"\xae\x01\n\x13UpdateSignalRequest\x120\n\x06signal\x18\x01 \x01(\x0b2\x1a.exabel.api.data.v1.SignalB\x04\xe2A\x01\x02\x12/\n\x0bupdate_mask\x18\x02 \x01(\x0b2\x1a.google.protobuf.FieldMask\x12\x15\n\rallow_missing\x18\x03 \x01(\x08\x12\x1d\n\x15create_library_signal\x18\x04 \x01(\x08"<\n\x13DeleteSignalRequest\x12%\n\x04name\x18\x01 \x01(\tB\x17\x92A\x10\xca>\r\xfa\x02\nsignalName\xe2A\x01\x022\xad\x05\n\rSignalService\x12\x84\x01\n\x0bListSignals\x12&.exabel.api.data.v1.ListSignalsRequest\x1a\'.exabel.api.data.v1.ListSignalsResponse"$\x92A\x0e\x12\x0cList signals\x82\xd3\xe4\x93\x02\r\x12\x0b/v1/signals\x12z\n\tGetSignal\x12$.exabel.api.data.v1.GetSignalRequest\x1a\x1a.exabel.api.data.v1.Signal"+\x92A\x0c\x12\nGet signal\x82\xd3\xe4\x93\x02\x16\x12\x14/v1/{name=signals/*}\x12\x82\x01\n\x0cCreateSignal\x12\'.exabel.api.data.v1.CreateSignalRequest\x1a\x1a.exabel.api.data.v1.Signal"-\x92A\x0f\x12\rCreate signal\x82\xd3\xe4\x93\x02\x15"\x0b/v1/signals:\x06signal\x12\x92\x01\n\x0cUpdateSignal\x12\'.exabel.api.data.v1.UpdateSignalRequest\x1a\x1a.exabel.api.data.v1.Signal"=\x92A\x0f\x12\rUpdate signal\x82\xd3\xe4\x93\x02%2\x1b/v1/{signal.name=signals/*}:\x06signal\x12\x7f\n\x0cDeleteSignal\x12\'.exabel.api.data.v1.DeleteSignalRequest\x1a\x16.google.protobuf.Empty".\x92A\x0f\x12\rDelete signal\x82\xd3\xe4\x93\x02\x16*\x14/v1/{name=signals/*}BF\n\x16com.exabel.api.data.v1B\x12SignalServiceProtoP\x01Z\x16exabel.com/api/data/v1b\x06proto3')
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.data.v1.signal_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b'\n\x16com.exabel.api.data.v1B\x12SignalServiceProtoP\x01Z\x16exabel.com/api/data/v1'
     _GETSIGNALREQUEST.fields_by_name['name']._options = None
-    _GETSIGNALREQUEST.fields_by_name['name']._serialized_options = b'\xe0A\x02\x92A\x10\xca>\r\xfa\x02\nsignalName'
+    _GETSIGNALREQUEST.fields_by_name['name']._serialized_options = b'\x92A\x10\xca>\r\xfa\x02\nsignalName\xe2A\x01\x02'
     _CREATESIGNALREQUEST.fields_by_name['signal']._options = None
-    _CREATESIGNALREQUEST.fields_by_name['signal']._serialized_options = b'\xe0A\x02'
+    _CREATESIGNALREQUEST.fields_by_name['signal']._serialized_options = b'\xe2A\x01\x02'
     _UPDATESIGNALREQUEST.fields_by_name['signal']._options = None
-    _UPDATESIGNALREQUEST.fields_by_name['signal']._serialized_options = b'\xe0A\x02'
+    _UPDATESIGNALREQUEST.fields_by_name['signal']._serialized_options = b'\xe2A\x01\x02'
     _DELETESIGNALREQUEST.fields_by_name['name']._options = None
-    _DELETESIGNALREQUEST.fields_by_name['name']._serialized_options = b'\xe0A\x02\x92A\x10\xca>\r\xfa\x02\nsignalName'
+    _DELETESIGNALREQUEST.fields_by_name['name']._serialized_options = b'\x92A\x10\xca>\r\xfa\x02\nsignalName\xe2A\x01\x02'
     _SIGNALSERVICE.methods_by_name['ListSignals']._options = None
-    _SIGNALSERVICE.methods_by_name['ListSignals']._serialized_options = b'\x82\xd3\xe4\x93\x02\r\x12\x0b/v1/signals\x92A\x0e\x12\x0cList signals'
+    _SIGNALSERVICE.methods_by_name['ListSignals']._serialized_options = b'\x92A\x0e\x12\x0cList signals\x82\xd3\xe4\x93\x02\r\x12\x0b/v1/signals'
     _SIGNALSERVICE.methods_by_name['GetSignal']._options = None
-    _SIGNALSERVICE.methods_by_name['GetSignal']._serialized_options = b'\x82\xd3\xe4\x93\x02\x16\x12\x14/v1/{name=signals/*}\x92A\x0c\x12\nGet signal'
+    _SIGNALSERVICE.methods_by_name['GetSignal']._serialized_options = b'\x92A\x0c\x12\nGet signal\x82\xd3\xe4\x93\x02\x16\x12\x14/v1/{name=signals/*}'
     _SIGNALSERVICE.methods_by_name['CreateSignal']._options = None
-    _SIGNALSERVICE.methods_by_name['CreateSignal']._serialized_options = b'\x82\xd3\xe4\x93\x02\x15"\x0b/v1/signals:\x06signal\x92A\x0f\x12\rCreate signal'
+    _SIGNALSERVICE.methods_by_name['CreateSignal']._serialized_options = b'\x92A\x0f\x12\rCreate signal\x82\xd3\xe4\x93\x02\x15"\x0b/v1/signals:\x06signal'
     _SIGNALSERVICE.methods_by_name['UpdateSignal']._options = None
-    _SIGNALSERVICE.methods_by_name['UpdateSignal']._serialized_options = b'\x82\xd3\xe4\x93\x02%2\x1b/v1/{signal.name=signals/*}:\x06signal\x92A\x0f\x12\rUpdate signal'
+    _SIGNALSERVICE.methods_by_name['UpdateSignal']._serialized_options = b'\x92A\x0f\x12\rUpdate signal\x82\xd3\xe4\x93\x02%2\x1b/v1/{signal.name=signals/*}:\x06signal'
     _SIGNALSERVICE.methods_by_name['DeleteSignal']._options = None
-    _SIGNALSERVICE.methods_by_name['DeleteSignal']._serialized_options = b'\x82\xd3\xe4\x93\x02\x16*\x14/v1/{name=signals/*}\x92A\x0f\x12\rDelete signal'
-    _LISTSIGNALSREQUEST._serialized_start = 279
-    _LISTSIGNALSREQUEST._serialized_end = 338
-    _LISTSIGNALSRESPONSE._serialized_start = 340
-    _LISTSIGNALSRESPONSE._serialized_end = 451
-    _GETSIGNALREQUEST._serialized_start = 453
-    _GETSIGNALREQUEST._serialized_end = 509
-    _CREATESIGNALREQUEST._serialized_start = 511
-    _CREATESIGNALREQUEST._serialized_end = 612
-    _UPDATESIGNALREQUEST._serialized_start = 615
-    _UPDATESIGNALREQUEST._serialized_end = 788
-    _DELETESIGNALREQUEST._serialized_start = 790
-    _DELETESIGNALREQUEST._serialized_end = 849
-    _SIGNALSERVICE._serialized_start = 852
-    _SIGNALSERVICE._serialized_end = 1537
+    _SIGNALSERVICE.methods_by_name['DeleteSignal']._serialized_options = b'\x92A\x0f\x12\rDelete signal\x82\xd3\xe4\x93\x02\x16*\x14/v1/{name=signals/*}'
+    _globals['_LISTSIGNALSREQUEST']._serialized_start = 279
+    _globals['_LISTSIGNALSREQUEST']._serialized_end = 338
+    _globals['_LISTSIGNALSRESPONSE']._serialized_start = 340
+    _globals['_LISTSIGNALSRESPONSE']._serialized_end = 451
+    _globals['_GETSIGNALREQUEST']._serialized_start = 453
+    _globals['_GETSIGNALREQUEST']._serialized_end = 510
+    _globals['_CREATESIGNALREQUEST']._serialized_start = 512
+    _globals['_CREATESIGNALREQUEST']._serialized_end = 614
+    _globals['_UPDATESIGNALREQUEST']._serialized_start = 617
+    _globals['_UPDATESIGNALREQUEST']._serialized_end = 791
+    _globals['_DELETESIGNALREQUEST']._serialized_start = 793
+    _globals['_DELETESIGNALREQUEST']._serialized_end = 853
+    _globals['_SIGNALSERVICE']._serialized_start = 856
+    _globals['_SIGNALSERVICE']._serialized_end = 1541
```

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_service_pb2_grpc.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_messages_pb2.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_messages_pb2.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 _sym_db = _symbol_database.Default()
 from .....exabel.api.time import time_range_pb2 as exabel_dot_api_dot_time_dot_time__range__pb2
 from google.api import field_behavior_pb2 as google_dot_api_dot_field__behavior__pb2
 from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from .....protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n-exabel/api/data/v1/time_series_messages.proto\x12\x12exabel.api.data.v1\x1a exabel/api/time/time_range.proto\x1a\x1fgoogle/api/field_behavior.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a.protoc_gen_openapiv2/options/annotations.proto"\xd4\x01\n\nTimeSeries\x12y\n\x04name\x18\x01 \x01(\tBk\xe0A\x05\xe0A\x02\x92AbJL"entityTypes/store/entities/ns.apple_store_fifth_avenue/signals/ns.visitors"\xca>\x11\xfa\x02\x0etimeSeriesName\x123\n\x06points\x18\x02 \x03(\x0b2#.exabel.api.data.v1.TimeSeriesPoint\x12\x16\n\tread_only\x18\x03 \x01(\x08B\x03\xe0A\x03"\x9d\x01\n\x0fTimeSeriesPoint\x12-\n\x04time\x18\x01 \x01(\x0b2\x1a.google.protobuf.TimestampB\x03\xe0A\x02\x12+\n\x05value\x18\x02 \x01(\x0b2\x1c.google.protobuf.DoubleValue\x12.\n\nknown_time\x18\x03 \x01(\x0b2\x1a.google.protobuf.Timestamp"u\n\x0eTimeSeriesView\x12.\n\ntime_range\x18\x01 \x01(\x0b2\x1a.exabel.api.time.TimeRange\x123\n\nknown_time\x18\x02 \x01(\x0b2\x1a.google.protobuf.TimestampB\x03\xe0A\x01"\x9f\x01\n\x10DefaultKnownTime\x12\x16\n\x0ccurrent_time\x18\x01 \x01(\x08H\x00\x120\n\nknown_time\x18\x02 \x01(\x0b2\x1a.google.protobuf.TimestampH\x00\x120\n\x0btime_offset\x18\x03 \x01(\x0b2\x19.google.protobuf.DurationH\x00B\x0f\n\rspecificationBK\n\x16com.exabel.api.data.v1B\x17TimeSeriesMessagesProtoP\x01Z\x16exabel.com/api/data/v1b\x06proto3')
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.data.v1.time_series_messages_pb2', globals())
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n-exabel/api/data/v1/time_series_messages.proto\x12\x12exabel.api.data.v1\x1a exabel/api/time/time_range.proto\x1a\x1fgoogle/api/field_behavior.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a.protoc_gen_openapiv2/options/annotations.proto"\xd4\x01\n\nTimeSeries\x12x\n\x04name\x18\x01 \x01(\tBj\x92AbJL"entityTypes/store/entities/ns.apple_store_fifth_avenue/signals/ns.visitors"\xca>\x11\xfa\x02\x0etimeSeriesName\xe2A\x02\x05\x02\x123\n\x06points\x18\x02 \x03(\x0b2#.exabel.api.data.v1.TimeSeriesPoint\x12\x17\n\tread_only\x18\x03 \x01(\x08B\x04\xe2A\x01\x03"\x9e\x01\n\x0fTimeSeriesPoint\x12.\n\x04time\x18\x01 \x01(\x0b2\x1a.google.protobuf.TimestampB\x04\xe2A\x01\x02\x12+\n\x05value\x18\x02 \x01(\x0b2\x1c.google.protobuf.DoubleValue\x12.\n\nknown_time\x18\x03 \x01(\x0b2\x1a.google.protobuf.Timestamp"v\n\x0eTimeSeriesView\x12.\n\ntime_range\x18\x01 \x01(\x0b2\x1a.exabel.api.time.TimeRange\x124\n\nknown_time\x18\x02 \x01(\x0b2\x1a.google.protobuf.TimestampB\x04\xe2A\x01\x01"\x9f\x01\n\x10DefaultKnownTime\x12\x16\n\x0ccurrent_time\x18\x01 \x01(\x08H\x00\x120\n\nknown_time\x18\x02 \x01(\x0b2\x1a.google.protobuf.TimestampH\x00\x120\n\x0btime_offset\x18\x03 \x01(\x0b2\x19.google.protobuf.DurationH\x00B\x0f\n\rspecificationBK\n\x16com.exabel.api.data.v1B\x17TimeSeriesMessagesProtoP\x01Z\x16exabel.com/api/data/v1b\x06proto3')
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.data.v1.time_series_messages_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b'\n\x16com.exabel.api.data.v1B\x17TimeSeriesMessagesProtoP\x01Z\x16exabel.com/api/data/v1'
     _TIMESERIES.fields_by_name['name']._options = None
-    _TIMESERIES.fields_by_name['name']._serialized_options = b'\xe0A\x05\xe0A\x02\x92AbJL"entityTypes/store/entities/ns.apple_store_fifth_avenue/signals/ns.visitors"\xca>\x11\xfa\x02\x0etimeSeriesName'
+    _TIMESERIES.fields_by_name['name']._serialized_options = b'\x92AbJL"entityTypes/store/entities/ns.apple_store_fifth_avenue/signals/ns.visitors"\xca>\x11\xfa\x02\x0etimeSeriesName\xe2A\x02\x05\x02'
     _TIMESERIES.fields_by_name['read_only']._options = None
-    _TIMESERIES.fields_by_name['read_only']._serialized_options = b'\xe0A\x03'
+    _TIMESERIES.fields_by_name['read_only']._serialized_options = b'\xe2A\x01\x03'
     _TIMESERIESPOINT.fields_by_name['time']._options = None
-    _TIMESERIESPOINT.fields_by_name['time']._serialized_options = b'\xe0A\x02'
+    _TIMESERIESPOINT.fields_by_name['time']._serialized_options = b'\xe2A\x01\x02'
     _TIMESERIESVIEW.fields_by_name['known_time']._options = None
-    _TIMESERIESVIEW.fields_by_name['known_time']._serialized_options = b'\xe0A\x01'
-    _TIMESERIES._serialized_start = 282
-    _TIMESERIES._serialized_end = 494
-    _TIMESERIESPOINT._serialized_start = 497
-    _TIMESERIESPOINT._serialized_end = 654
-    _TIMESERIESVIEW._serialized_start = 656
-    _TIMESERIESVIEW._serialized_end = 773
-    _DEFAULTKNOWNTIME._serialized_start = 776
-    _DEFAULTKNOWNTIME._serialized_end = 935
+    _TIMESERIESVIEW.fields_by_name['known_time']._serialized_options = b'\xe2A\x01\x01'
+    _globals['_TIMESERIES']._serialized_start = 282
+    _globals['_TIMESERIES']._serialized_end = 494
+    _globals['_TIMESERIESPOINT']._serialized_start = 497
+    _globals['_TIMESERIESPOINT']._serialized_end = 655
+    _globals['_TIMESERIESVIEW']._serialized_start = 657
+    _globals['_TIMESERIESVIEW']._serialized_end = 775
+    _globals['_DEFAULTKNOWNTIME']._serialized_start = 778
+    _globals['_DEFAULTKNOWNTIME']._serialized_end = 937
```

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_service_pb2.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_service_pb2.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,72 +1,73 @@
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 _sym_db = _symbol_database.Default()
 from .....exabel.api.data.v1 import time_series_messages_pb2 as exabel_dot_api_dot_data_dot_v1_dot_time__series__messages__pb2
 from .....exabel.api.time import time_range_pb2 as exabel_dot_api_dot_time_dot_time__range__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from google.api import field_behavior_pb2 as google_dot_api_dot_field__behavior__pb2
 from google.api import visibility_pb2 as google_dot_api_dot_visibility__pb2
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 from google.rpc import status_pb2 as google_dot_rpc_dot_status__pb2
 from .....protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n,exabel/api/data/v1/time_series_service.proto\x12\x12exabel.api.data.v1\x1a-exabel/api/data/v1/time_series_messages.proto\x1a exabel/api/time/time_range.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1fgoogle/api/field_behavior.proto\x1a\x1bgoogle/api/visibility.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a\x17google/rpc/status.proto\x1a.protoc_gen_openapiv2/options/annotations.proto"l\n\x15ListTimeSeriesRequest\x12,\n\x06parent\x18\x01 \x01(\tB\x1c\xe0A\x02\x92A\x16\xca>\x13\xfa\x02\x10timeSeriesParent\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12\x12\n\npage_token\x18\x03 \x01(\t"z\n\x16ListTimeSeriesResponse\x123\n\x0btime_series\x18\x01 \x03(\x0b2\x1e.exabel.api.data.v1.TimeSeries\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\x12\x12\n\ntotal_size\x18\x03 \x01(\x05"r\n\x14GetTimeSeriesRequest\x12(\n\x04name\x18\x01 \x01(\tB\x1a\xe0A\x02\x92A\x14\xca>\x11\xfa\x02\x0etimeSeriesName\x120\n\x04view\x18\x02 \x01(\x0b2".exabel.api.data.v1.TimeSeriesView"\xdb\x01\n\x17CreateTimeSeriesRequest\x128\n\x0btime_series\x18\x01 \x01(\x0b2\x1e.exabel.api.data.v1.TimeSeriesB\x03\xe0A\x02\x120\n\x04view\x18\x02 \x01(\x0b2".exabel.api.data.v1.TimeSeriesView\x12@\n\x12default_known_time\x18\x03 \x01(\x0b2$.exabel.api.data.v1.DefaultKnownTime\x12\x12\n\ncreate_tag\x18\x04 \x01(\x08"\xf2\x01\n\x17UpdateTimeSeriesRequest\x128\n\x0btime_series\x18\x01 \x01(\x0b2\x1e.exabel.api.data.v1.TimeSeriesB\x03\xe0A\x02\x120\n\x04view\x18\x02 \x01(\x0b2".exabel.api.data.v1.TimeSeriesView\x12@\n\x12default_known_time\x18\x03 \x01(\x0b2$.exabel.api.data.v1.DefaultKnownTime\x12\x15\n\rallow_missing\x18\x04 \x01(\x08\x12\x12\n\ncreate_tag\x18\x05 \x01(\x08"\xec\x01\n\x17ImportTimeSeriesRequest\x12\x13\n\x06parent\x18\x01 \x01(\tB\x03\xe0A\x02\x123\n\x0btime_series\x18\x02 \x03(\x0b2\x1e.exabel.api.data.v1.TimeSeries\x12@\n\x12default_known_time\x18\x03 \x01(\x0b2$.exabel.api.data.v1.DefaultKnownTime\x12\x15\n\rallow_missing\x18\x04 \x01(\x08\x12\x12\n\ncreate_tag\x18\x05 \x01(\x08\x12\x1a\n\x12status_in_response\x18\x06 \x01(\x08"\xa2\x02\n\x18ImportTimeSeriesResponse\x12X\n\tresponses\x18\x01 \x03(\x0b2E.exabel.api.data.v1.ImportTimeSeriesResponse.SingleTimeSeriesResponse\x1a\xab\x01\n\x18SingleTimeSeriesResponse\x12k\n\x10time_series_name\x18\x01 \x01(\tBQ\x92ANJL"entityTypes/store/entities/ns.apple_store_fifth_avenue/signals/ns.visitors"\x12"\n\x06status\x18\x02 \x01(\x0b2\x12.google.rpc.Status"C\n\x17DeleteTimeSeriesRequest\x12(\n\x04name\x18\x01 \x01(\tB\x1a\xe0A\x02\x92A\x14\xca>\x11\xfa\x02\x0etimeSeriesName"\x7f\n"BatchDeleteTimeSeriesPointsRequest\x12(\n\x04name\x18\x01 \x01(\tB\x1a\xe0A\x02\x92A\x14\xca>\x11\xfa\x02\x0etimeSeriesName\x12/\n\x0btime_ranges\x18\x02 \x03(\x0b2\x1a.exabel.api.time.TimeRange2\x80\x0e\n\x11TimeSeriesService\x12\xdb\x01\n\x0eListTimeSeries\x12).exabel.api.data.v1.ListTimeSeriesRequest\x1a*.exabel.api.data.v1.ListTimeSeriesResponse"r\x82\xd3\xe4\x93\x02W\x120/v1/{parent=entityTypes/*/entities/*}/timeSeriesZ#\x12!/v1/{parent=signals/*}/timeSeries\x92A\x12\x12\x10List time series\x12\xd5\x01\n\rGetTimeSeries\x12(.exabel.api.data.v1.GetTimeSeriesRequest\x1a\x1e.exabel.api.data.v1.TimeSeries"z\x82\xd3\xe4\x93\x02`\x12-/v1/{name=entityTypes/*/entities/*/signals/*}Z/\x12-/v1/{name=signals/*/entityTypes/*/entities/*}\x92A\x11\x12\x0fGet time series\x12\x92\x02\n\x10CreateTimeSeries\x12+.exabel.api.data.v1.CreateTimeSeriesRequest\x1a\x1e.exabel.api.data.v1.TimeSeries"\xb0\x01\x82\xd3\xe4\x93\x02\x92\x01"9/v1/{time_series.name=entityTypes/*/entities/*/signals/*}:\x0btime_seriesZH"9/v1/{time_series.name=signals/*/entityTypes/*/entities/*}:\x0btime_series\x92A\x14\x12\x12Create time series\x12\x92\x02\n\x10UpdateTimeSeries\x12+.exabel.api.data.v1.UpdateTimeSeriesRequest\x1a\x1e.exabel.api.data.v1.TimeSeries"\xb0\x01\x82\xd3\xe4\x93\x02\x92\x0129/v1/{time_series.name=entityTypes/*/entities/*/signals/*}:\x0btime_seriesZH29/v1/{time_series.name=signals/*/entityTypes/*/entities/*}:\x0btime_series\x92A\x14\x12\x12Update time series\x12\xf8\x01\n\x10ImportTimeSeries\x12+.exabel.api.data.v1.ImportTimeSeriesRequest\x1a,.exabel.api.data.v1.ImportTimeSeriesResponse"\x88\x01\x82\xd3\xe4\x93\x02k"7/v1/{parent=entityTypes/*/entities/*}/timeSeries:import:\x01*Z-"(/v1/{parent=signals/*}/timeSeries:import:\x01*\x92A\x14\x12\x12Import time series\x12\xd6\x01\n\x10DeleteTimeSeries\x12+.exabel.api.data.v1.DeleteTimeSeriesRequest\x1a\x16.google.protobuf.Empty"}\x82\xd3\xe4\x93\x02`*-/v1/{name=entityTypes/*/entities/*/signals/*}Z/*-/v1/{name=signals/*/entityTypes/*/entities/*}\x92A\x14\x12\x12Delete time series\x12\xb6\x02\n\x1bBatchDeleteTimeSeriesPoints\x126.exabel.api.data.v1.BatchDeleteTimeSeriesPointsRequest\x1a\x16.google.protobuf.Empty"\xc6\x01\xfa\xd2\xe4\x93\x02\n\x12\x08INTERNAL\x82\xd3\xe4\x93\x02\x8c\x01"@/v1/{name=entityTypes/*/entities/*/signals/*}/points:batchDelete:\x01*ZE"@/v1/{name=signals/*/entityTypes/*/entities/*}/points:batchDelete:\x01*\x92A \x12\x1eDelete time series data pointsBJ\n\x16com.exabel.api.data.v1B\x16TimeSeriesServiceProtoP\x01Z\x16exabel.com/api/data/v1b\x06proto3')
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.data.v1.time_series_service_pb2', globals())
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n,exabel/api/data/v1/time_series_service.proto\x12\x12exabel.api.data.v1\x1a-exabel/api/data/v1/time_series_messages.proto\x1a exabel/api/time/time_range.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1fgoogle/api/field_behavior.proto\x1a\x1bgoogle/api/visibility.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a\x17google/rpc/status.proto\x1a.protoc_gen_openapiv2/options/annotations.proto"m\n\x15ListTimeSeriesRequest\x12-\n\x06parent\x18\x01 \x01(\tB\x1d\x92A\x16\xca>\x13\xfa\x02\x10timeSeriesParent\xe2A\x01\x02\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12\x12\n\npage_token\x18\x03 \x01(\t"z\n\x16ListTimeSeriesResponse\x123\n\x0btime_series\x18\x01 \x03(\x0b2\x1e.exabel.api.data.v1.TimeSeries\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\x12\x12\n\ntotal_size\x18\x03 \x01(\x05"s\n\x14GetTimeSeriesRequest\x12)\n\x04name\x18\x01 \x01(\tB\x1b\x92A\x14\xca>\x11\xfa\x02\x0etimeSeriesName\xe2A\x01\x02\x120\n\x04view\x18\x02 \x01(\x0b2".exabel.api.data.v1.TimeSeriesView"\xdc\x01\n\x17CreateTimeSeriesRequest\x129\n\x0btime_series\x18\x01 \x01(\x0b2\x1e.exabel.api.data.v1.TimeSeriesB\x04\xe2A\x01\x02\x120\n\x04view\x18\x02 \x01(\x0b2".exabel.api.data.v1.TimeSeriesView\x12@\n\x12default_known_time\x18\x03 \x01(\x0b2$.exabel.api.data.v1.DefaultKnownTime\x12\x12\n\ncreate_tag\x18\x04 \x01(\x08"\xf3\x01\n\x17UpdateTimeSeriesRequest\x129\n\x0btime_series\x18\x01 \x01(\x0b2\x1e.exabel.api.data.v1.TimeSeriesB\x04\xe2A\x01\x02\x120\n\x04view\x18\x02 \x01(\x0b2".exabel.api.data.v1.TimeSeriesView\x12@\n\x12default_known_time\x18\x03 \x01(\x0b2$.exabel.api.data.v1.DefaultKnownTime\x12\x15\n\rallow_missing\x18\x04 \x01(\x08\x12\x12\n\ncreate_tag\x18\x05 \x01(\x08"\x93\x02\n\x17ImportTimeSeriesRequest\x12\x14\n\x06parent\x18\x01 \x01(\tB\x04\xe2A\x01\x02\x123\n\x0btime_series\x18\x02 \x03(\x0b2\x1e.exabel.api.data.v1.TimeSeries\x12@\n\x12default_known_time\x18\x03 \x01(\x0b2$.exabel.api.data.v1.DefaultKnownTime\x12\x15\n\rallow_missing\x18\x04 \x01(\x08\x12\x12\n\ncreate_tag\x18\x05 \x01(\x08\x12\x1a\n\x12status_in_response\x18\x06 \x01(\x08\x12$\n\x1creplace_existing_time_series\x18\x07 \x01(\x08"\xa2\x02\n\x18ImportTimeSeriesResponse\x12X\n\tresponses\x18\x01 \x03(\x0b2E.exabel.api.data.v1.ImportTimeSeriesResponse.SingleTimeSeriesResponse\x1a\xab\x01\n\x18SingleTimeSeriesResponse\x12k\n\x10time_series_name\x18\x01 \x01(\tBQ\x92ANJL"entityTypes/store/entities/ns.apple_store_fifth_avenue/signals/ns.visitors"\x12"\n\x06status\x18\x02 \x01(\x0b2\x12.google.rpc.Status"D\n\x17DeleteTimeSeriesRequest\x12)\n\x04name\x18\x01 \x01(\tB\x1b\x92A\x14\xca>\x11\xfa\x02\x0etimeSeriesName\xe2A\x01\x02"\x80\x01\n"BatchDeleteTimeSeriesPointsRequest\x12)\n\x04name\x18\x01 \x01(\tB\x1b\x92A\x14\xca>\x11\xfa\x02\x0etimeSeriesName\xe2A\x01\x02\x12/\n\x0btime_ranges\x18\x02 \x03(\x0b2\x1a.exabel.api.time.TimeRange2\x80\x0e\n\x11TimeSeriesService\x12\xdb\x01\n\x0eListTimeSeries\x12).exabel.api.data.v1.ListTimeSeriesRequest\x1a*.exabel.api.data.v1.ListTimeSeriesResponse"r\x92A\x12\x12\x10List time series\x82\xd3\xe4\x93\x02W\x120/v1/{parent=entityTypes/*/entities/*}/timeSeriesZ#\x12!/v1/{parent=signals/*}/timeSeries\x12\xd5\x01\n\rGetTimeSeries\x12(.exabel.api.data.v1.GetTimeSeriesRequest\x1a\x1e.exabel.api.data.v1.TimeSeries"z\x92A\x11\x12\x0fGet time series\x82\xd3\xe4\x93\x02`\x12-/v1/{name=entityTypes/*/entities/*/signals/*}Z/\x12-/v1/{name=signals/*/entityTypes/*/entities/*}\x12\x92\x02\n\x10CreateTimeSeries\x12+.exabel.api.data.v1.CreateTimeSeriesRequest\x1a\x1e.exabel.api.data.v1.TimeSeries"\xb0\x01\x92A\x14\x12\x12Create time series\x82\xd3\xe4\x93\x02\x92\x01"9/v1/{time_series.name=entityTypes/*/entities/*/signals/*}:\x0btime_seriesZH"9/v1/{time_series.name=signals/*/entityTypes/*/entities/*}:\x0btime_series\x12\x92\x02\n\x10UpdateTimeSeries\x12+.exabel.api.data.v1.UpdateTimeSeriesRequest\x1a\x1e.exabel.api.data.v1.TimeSeries"\xb0\x01\x92A\x14\x12\x12Update time series\x82\xd3\xe4\x93\x02\x92\x0129/v1/{time_series.name=entityTypes/*/entities/*/signals/*}:\x0btime_seriesZH29/v1/{time_series.name=signals/*/entityTypes/*/entities/*}:\x0btime_series\x12\xf8\x01\n\x10ImportTimeSeries\x12+.exabel.api.data.v1.ImportTimeSeriesRequest\x1a,.exabel.api.data.v1.ImportTimeSeriesResponse"\x88\x01\x92A\x14\x12\x12Import time series\x82\xd3\xe4\x93\x02k"7/v1/{parent=entityTypes/*/entities/*}/timeSeries:import:\x01*Z-"(/v1/{parent=signals/*}/timeSeries:import:\x01*\x12\xd6\x01\n\x10DeleteTimeSeries\x12+.exabel.api.data.v1.DeleteTimeSeriesRequest\x1a\x16.google.protobuf.Empty"}\x92A\x14\x12\x12Delete time series\x82\xd3\xe4\x93\x02`*-/v1/{name=entityTypes/*/entities/*/signals/*}Z/*-/v1/{name=signals/*/entityTypes/*/entities/*}\x12\xb6\x02\n\x1bBatchDeleteTimeSeriesPoints\x126.exabel.api.data.v1.BatchDeleteTimeSeriesPointsRequest\x1a\x16.google.protobuf.Empty"\xc6\x01\x92A \x12\x1eDelete time series data points\xfa\xd2\xe4\x93\x02\n\x12\x08INTERNAL\x82\xd3\xe4\x93\x02\x8c\x01"@/v1/{name=entityTypes/*/entities/*/signals/*}/points:batchDelete:\x01*ZE"@/v1/{name=signals/*/entityTypes/*/entities/*}/points:batchDelete:\x01*BJ\n\x16com.exabel.api.data.v1B\x16TimeSeriesServiceProtoP\x01Z\x16exabel.com/api/data/v1b\x06proto3')
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.data.v1.time_series_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b'\n\x16com.exabel.api.data.v1B\x16TimeSeriesServiceProtoP\x01Z\x16exabel.com/api/data/v1'
     _LISTTIMESERIESREQUEST.fields_by_name['parent']._options = None
-    _LISTTIMESERIESREQUEST.fields_by_name['parent']._serialized_options = b'\xe0A\x02\x92A\x16\xca>\x13\xfa\x02\x10timeSeriesParent'
+    _LISTTIMESERIESREQUEST.fields_by_name['parent']._serialized_options = b'\x92A\x16\xca>\x13\xfa\x02\x10timeSeriesParent\xe2A\x01\x02'
     _GETTIMESERIESREQUEST.fields_by_name['name']._options = None
-    _GETTIMESERIESREQUEST.fields_by_name['name']._serialized_options = b'\xe0A\x02\x92A\x14\xca>\x11\xfa\x02\x0etimeSeriesName'
+    _GETTIMESERIESREQUEST.fields_by_name['name']._serialized_options = b'\x92A\x14\xca>\x11\xfa\x02\x0etimeSeriesName\xe2A\x01\x02'
     _CREATETIMESERIESREQUEST.fields_by_name['time_series']._options = None
-    _CREATETIMESERIESREQUEST.fields_by_name['time_series']._serialized_options = b'\xe0A\x02'
+    _CREATETIMESERIESREQUEST.fields_by_name['time_series']._serialized_options = b'\xe2A\x01\x02'
     _UPDATETIMESERIESREQUEST.fields_by_name['time_series']._options = None
-    _UPDATETIMESERIESREQUEST.fields_by_name['time_series']._serialized_options = b'\xe0A\x02'
+    _UPDATETIMESERIESREQUEST.fields_by_name['time_series']._serialized_options = b'\xe2A\x01\x02'
     _IMPORTTIMESERIESREQUEST.fields_by_name['parent']._options = None
-    _IMPORTTIMESERIESREQUEST.fields_by_name['parent']._serialized_options = b'\xe0A\x02'
+    _IMPORTTIMESERIESREQUEST.fields_by_name['parent']._serialized_options = b'\xe2A\x01\x02'
     _IMPORTTIMESERIESRESPONSE_SINGLETIMESERIESRESPONSE.fields_by_name['time_series_name']._options = None
     _IMPORTTIMESERIESRESPONSE_SINGLETIMESERIESRESPONSE.fields_by_name['time_series_name']._serialized_options = b'\x92ANJL"entityTypes/store/entities/ns.apple_store_fifth_avenue/signals/ns.visitors"'
     _DELETETIMESERIESREQUEST.fields_by_name['name']._options = None
-    _DELETETIMESERIESREQUEST.fields_by_name['name']._serialized_options = b'\xe0A\x02\x92A\x14\xca>\x11\xfa\x02\x0etimeSeriesName'
+    _DELETETIMESERIESREQUEST.fields_by_name['name']._serialized_options = b'\x92A\x14\xca>\x11\xfa\x02\x0etimeSeriesName\xe2A\x01\x02'
     _BATCHDELETETIMESERIESPOINTSREQUEST.fields_by_name['name']._options = None
-    _BATCHDELETETIMESERIESPOINTSREQUEST.fields_by_name['name']._serialized_options = b'\xe0A\x02\x92A\x14\xca>\x11\xfa\x02\x0etimeSeriesName'
+    _BATCHDELETETIMESERIESPOINTSREQUEST.fields_by_name['name']._serialized_options = b'\x92A\x14\xca>\x11\xfa\x02\x0etimeSeriesName\xe2A\x01\x02'
     _TIMESERIESSERVICE.methods_by_name['ListTimeSeries']._options = None
-    _TIMESERIESSERVICE.methods_by_name['ListTimeSeries']._serialized_options = b'\x82\xd3\xe4\x93\x02W\x120/v1/{parent=entityTypes/*/entities/*}/timeSeriesZ#\x12!/v1/{parent=signals/*}/timeSeries\x92A\x12\x12\x10List time series'
+    _TIMESERIESSERVICE.methods_by_name['ListTimeSeries']._serialized_options = b'\x92A\x12\x12\x10List time series\x82\xd3\xe4\x93\x02W\x120/v1/{parent=entityTypes/*/entities/*}/timeSeriesZ#\x12!/v1/{parent=signals/*}/timeSeries'
     _TIMESERIESSERVICE.methods_by_name['GetTimeSeries']._options = None
-    _TIMESERIESSERVICE.methods_by_name['GetTimeSeries']._serialized_options = b'\x82\xd3\xe4\x93\x02`\x12-/v1/{name=entityTypes/*/entities/*/signals/*}Z/\x12-/v1/{name=signals/*/entityTypes/*/entities/*}\x92A\x11\x12\x0fGet time series'
+    _TIMESERIESSERVICE.methods_by_name['GetTimeSeries']._serialized_options = b'\x92A\x11\x12\x0fGet time series\x82\xd3\xe4\x93\x02`\x12-/v1/{name=entityTypes/*/entities/*/signals/*}Z/\x12-/v1/{name=signals/*/entityTypes/*/entities/*}'
     _TIMESERIESSERVICE.methods_by_name['CreateTimeSeries']._options = None
-    _TIMESERIESSERVICE.methods_by_name['CreateTimeSeries']._serialized_options = b'\x82\xd3\xe4\x93\x02\x92\x01"9/v1/{time_series.name=entityTypes/*/entities/*/signals/*}:\x0btime_seriesZH"9/v1/{time_series.name=signals/*/entityTypes/*/entities/*}:\x0btime_series\x92A\x14\x12\x12Create time series'
+    _TIMESERIESSERVICE.methods_by_name['CreateTimeSeries']._serialized_options = b'\x92A\x14\x12\x12Create time series\x82\xd3\xe4\x93\x02\x92\x01"9/v1/{time_series.name=entityTypes/*/entities/*/signals/*}:\x0btime_seriesZH"9/v1/{time_series.name=signals/*/entityTypes/*/entities/*}:\x0btime_series'
     _TIMESERIESSERVICE.methods_by_name['UpdateTimeSeries']._options = None
-    _TIMESERIESSERVICE.methods_by_name['UpdateTimeSeries']._serialized_options = b'\x82\xd3\xe4\x93\x02\x92\x0129/v1/{time_series.name=entityTypes/*/entities/*/signals/*}:\x0btime_seriesZH29/v1/{time_series.name=signals/*/entityTypes/*/entities/*}:\x0btime_series\x92A\x14\x12\x12Update time series'
+    _TIMESERIESSERVICE.methods_by_name['UpdateTimeSeries']._serialized_options = b'\x92A\x14\x12\x12Update time series\x82\xd3\xe4\x93\x02\x92\x0129/v1/{time_series.name=entityTypes/*/entities/*/signals/*}:\x0btime_seriesZH29/v1/{time_series.name=signals/*/entityTypes/*/entities/*}:\x0btime_series'
     _TIMESERIESSERVICE.methods_by_name['ImportTimeSeries']._options = None
-    _TIMESERIESSERVICE.methods_by_name['ImportTimeSeries']._serialized_options = b'\x82\xd3\xe4\x93\x02k"7/v1/{parent=entityTypes/*/entities/*}/timeSeries:import:\x01*Z-"(/v1/{parent=signals/*}/timeSeries:import:\x01*\x92A\x14\x12\x12Import time series'
+    _TIMESERIESSERVICE.methods_by_name['ImportTimeSeries']._serialized_options = b'\x92A\x14\x12\x12Import time series\x82\xd3\xe4\x93\x02k"7/v1/{parent=entityTypes/*/entities/*}/timeSeries:import:\x01*Z-"(/v1/{parent=signals/*}/timeSeries:import:\x01*'
     _TIMESERIESSERVICE.methods_by_name['DeleteTimeSeries']._options = None
-    _TIMESERIESSERVICE.methods_by_name['DeleteTimeSeries']._serialized_options = b'\x82\xd3\xe4\x93\x02`*-/v1/{name=entityTypes/*/entities/*/signals/*}Z/*-/v1/{name=signals/*/entityTypes/*/entities/*}\x92A\x14\x12\x12Delete time series'
+    _TIMESERIESSERVICE.methods_by_name['DeleteTimeSeries']._serialized_options = b'\x92A\x14\x12\x12Delete time series\x82\xd3\xe4\x93\x02`*-/v1/{name=entityTypes/*/entities/*/signals/*}Z/*-/v1/{name=signals/*/entityTypes/*/entities/*}'
     _TIMESERIESSERVICE.methods_by_name['BatchDeleteTimeSeriesPoints']._options = None
-    _TIMESERIESSERVICE.methods_by_name['BatchDeleteTimeSeriesPoints']._serialized_options = b'\xfa\xd2\xe4\x93\x02\n\x12\x08INTERNAL\x82\xd3\xe4\x93\x02\x8c\x01"@/v1/{name=entityTypes/*/entities/*/signals/*}/points:batchDelete:\x01*ZE"@/v1/{name=signals/*/entityTypes/*/entities/*}/points:batchDelete:\x01*\x92A \x12\x1eDelete time series data points'
-    _LISTTIMESERIESREQUEST._serialized_start = 343
-    _LISTTIMESERIESREQUEST._serialized_end = 451
-    _LISTTIMESERIESRESPONSE._serialized_start = 453
-    _LISTTIMESERIESRESPONSE._serialized_end = 575
-    _GETTIMESERIESREQUEST._serialized_start = 577
-    _GETTIMESERIESREQUEST._serialized_end = 691
-    _CREATETIMESERIESREQUEST._serialized_start = 694
-    _CREATETIMESERIESREQUEST._serialized_end = 913
-    _UPDATETIMESERIESREQUEST._serialized_start = 916
-    _UPDATETIMESERIESREQUEST._serialized_end = 1158
-    _IMPORTTIMESERIESREQUEST._serialized_start = 1161
-    _IMPORTTIMESERIESREQUEST._serialized_end = 1397
-    _IMPORTTIMESERIESRESPONSE._serialized_start = 1400
-    _IMPORTTIMESERIESRESPONSE._serialized_end = 1690
-    _IMPORTTIMESERIESRESPONSE_SINGLETIMESERIESRESPONSE._serialized_start = 1519
-    _IMPORTTIMESERIESRESPONSE_SINGLETIMESERIESRESPONSE._serialized_end = 1690
-    _DELETETIMESERIESREQUEST._serialized_start = 1692
-    _DELETETIMESERIESREQUEST._serialized_end = 1759
-    _BATCHDELETETIMESERIESPOINTSREQUEST._serialized_start = 1761
-    _BATCHDELETETIMESERIESPOINTSREQUEST._serialized_end = 1888
-    _TIMESERIESSERVICE._serialized_start = 1891
-    _TIMESERIESSERVICE._serialized_end = 3683
+    _TIMESERIESSERVICE.methods_by_name['BatchDeleteTimeSeriesPoints']._serialized_options = b'\x92A \x12\x1eDelete time series data points\xfa\xd2\xe4\x93\x02\n\x12\x08INTERNAL\x82\xd3\xe4\x93\x02\x8c\x01"@/v1/{name=entityTypes/*/entities/*/signals/*}/points:batchDelete:\x01*ZE"@/v1/{name=signals/*/entityTypes/*/entities/*}/points:batchDelete:\x01*'
+    _globals['_LISTTIMESERIESREQUEST']._serialized_start = 343
+    _globals['_LISTTIMESERIESREQUEST']._serialized_end = 452
+    _globals['_LISTTIMESERIESRESPONSE']._serialized_start = 454
+    _globals['_LISTTIMESERIESRESPONSE']._serialized_end = 576
+    _globals['_GETTIMESERIESREQUEST']._serialized_start = 578
+    _globals['_GETTIMESERIESREQUEST']._serialized_end = 693
+    _globals['_CREATETIMESERIESREQUEST']._serialized_start = 696
+    _globals['_CREATETIMESERIESREQUEST']._serialized_end = 916
+    _globals['_UPDATETIMESERIESREQUEST']._serialized_start = 919
+    _globals['_UPDATETIMESERIESREQUEST']._serialized_end = 1162
+    _globals['_IMPORTTIMESERIESREQUEST']._serialized_start = 1165
+    _globals['_IMPORTTIMESERIESREQUEST']._serialized_end = 1440
+    _globals['_IMPORTTIMESERIESRESPONSE']._serialized_start = 1443
+    _globals['_IMPORTTIMESERIESRESPONSE']._serialized_end = 1733
+    _globals['_IMPORTTIMESERIESRESPONSE_SINGLETIMESERIESRESPONSE']._serialized_start = 1562
+    _globals['_IMPORTTIMESERIESRESPONSE_SINGLETIMESERIESRESPONSE']._serialized_end = 1733
+    _globals['_DELETETIMESERIESREQUEST']._serialized_start = 1735
+    _globals['_DELETETIMESERIESREQUEST']._serialized_end = 1803
+    _globals['_BATCHDELETETIMESERIESPOINTSREQUEST']._serialized_start = 1806
+    _globals['_BATCHDELETETIMESERIESPOINTSREQUEST']._serialized_end = 1934
+    _globals['_TIMESERIESSERVICE']._serialized_start = 1937
+    _globals['_TIMESERIESSERVICE']._serialized_end = 3729
```

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_service_pb2_grpc.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/management/v1/folder_messages_pb2.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/management/v1/folder_messages_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 _sym_db = _symbol_database.Default()
 from .....exabel.api.management.v1 import user_messages_pb2 as exabel_dot_api_dot_management_dot_v1_dot_user__messages__pb2
 from google.api import field_behavior_pb2 as google_dot_api_dot_field__behavior__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from .....protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n.exabel/api/management/v1/folder_messages.proto\x12\x18exabel.api.management.v1\x1a,exabel/api/management/v1/user_messages.proto\x1a\x1fgoogle/api/field_behavior.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a.protoc_gen_openapiv2/options/annotations.proto"\xf3\x01\n\x06Folder\x120\n\x04name\x18\x01 \x01(\tB"\x92A\x1fJ\r"folders/123"\xca>\r\xfa\x02\nfolderName\x120\n\x0cdisplay_name\x18\x02 \x01(\tB\x1a\xe0A\x02\x92A\x14J\x12"My shared folder"\x124\n\x0bdescription\x18\x05 \x01(\tB\x1f\x92A\x1cJ\x1a"This is my shared folder"\x12\x12\n\x05write\x18\x03 \x01(\x08B\x03\xe0A\x03\x12;\n\x05items\x18\x04 \x03(\x0b2$.exabel.api.management.v1.FolderItemB\x06\xe0A\x06\xe0A\x03"\xf0\x02\n\nFolderItem\x122\n\x06parent\x18\x01 \x01(\tB"\x92A\x1fJ\r"folders/123"\xca>\r\xfa\x02\nfolderName\x12*\n\x04name\x18\x02 \x01(\tB\x1c\xe0A\x03\x92A\x16J\x14"derivedSignals/123"\x12&\n\x0cdisplay_name\x18\x03 \x01(\tB\x10\x92A\rJ\x0b"my_signal"\x12\x13\n\x0bdescription\x18\t \x01(\t\x12;\n\titem_type\x18\x04 \x01(\x0e2(.exabel.api.management.v1.FolderItemType\x12/\n\x0bcreate_time\x18\x05 \x01(\x0b2\x1a.google.protobuf.Timestamp\x12/\n\x0bupdate_time\x18\x06 \x01(\x0b2\x1a.google.protobuf.Timestamp\x12\x12\n\ncreated_by\x18\x07 \x01(\t\x12\x12\n\nupdated_by\x18\x08 \x01(\t"O\n\x0eFolderAccessor\x12.\n\x05group\x18\x01 \x01(\x0b2\x1f.exabel.api.management.v1.Group\x12\r\n\x05write\x18\x02 \x01(\x08"B\n\x0cSearchResult\x122\n\x04item\x18\x01 \x01(\x0b2$.exabel.api.management.v1.FolderItem*\xc4\x01\n\x0eFolderItemType\x12\x1c\n\x18FOLDER_ITEM_TYPE_INVALID\x10\x00\x12\x12\n\x0eDERIVED_SIGNAL\x10\x01\x12\x14\n\x10PREDICTION_MODEL\x10\x02\x12\x16\n\x12PORTFOLIO_STRATEGY\x10\x03\x12\r\n\tDASHBOARD\x10\x04\x12\x0e\n\nDRILL_DOWN\x10\x05\x12\x07\n\x03TAG\x10\x06\x12\n\n\x06SCREEN\x10\x07\x12\x13\n\x0fFINANCIAL_MODEL\x10\x08\x12\t\n\x05CHART\x10\tBS\n\x1ccom.exabel.api.management.v1B\x13FolderMessagesProtoP\x01Z\x1cexabel.com/api/management/v1b\x06proto3')
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.management.v1.folder_messages_pb2', globals())
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n.exabel/api/management/v1/folder_messages.proto\x12\x18exabel.api.management.v1\x1a,exabel/api/management/v1/user_messages.proto\x1a\x1fgoogle/api/field_behavior.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a.protoc_gen_openapiv2/options/annotations.proto"\xf4\x01\n\x06Folder\x120\n\x04name\x18\x01 \x01(\tB"\x92A\x1fJ\r"folders/123"\xca>\r\xfa\x02\nfolderName\x121\n\x0cdisplay_name\x18\x02 \x01(\tB\x1b\x92A\x14J\x12"My shared folder"\xe2A\x01\x02\x124\n\x0bdescription\x18\x05 \x01(\tB\x1f\x92A\x1cJ\x1a"This is my shared folder"\x12\x13\n\x05write\x18\x03 \x01(\x08B\x04\xe2A\x01\x03\x12:\n\x05items\x18\x04 \x03(\x0b2$.exabel.api.management.v1.FolderItemB\x05\xe2A\x02\x06\x03"\xf1\x02\n\nFolderItem\x122\n\x06parent\x18\x01 \x01(\tB"\x92A\x1fJ\r"folders/123"\xca>\r\xfa\x02\nfolderName\x12+\n\x04name\x18\x02 \x01(\tB\x1d\x92A\x16J\x14"derivedSignals/123"\xe2A\x01\x03\x12&\n\x0cdisplay_name\x18\x03 \x01(\tB\x10\x92A\rJ\x0b"my_signal"\x12\x13\n\x0bdescription\x18\t \x01(\t\x12;\n\titem_type\x18\x04 \x01(\x0e2(.exabel.api.management.v1.FolderItemType\x12/\n\x0bcreate_time\x18\x05 \x01(\x0b2\x1a.google.protobuf.Timestamp\x12/\n\x0bupdate_time\x18\x06 \x01(\x0b2\x1a.google.protobuf.Timestamp\x12\x12\n\ncreated_by\x18\x07 \x01(\t\x12\x12\n\nupdated_by\x18\x08 \x01(\t"O\n\x0eFolderAccessor\x12.\n\x05group\x18\x01 \x01(\x0b2\x1f.exabel.api.management.v1.Group\x12\r\n\x05write\x18\x02 \x01(\x08"B\n\x0cSearchResult\x122\n\x04item\x18\x01 \x01(\x0b2$.exabel.api.management.v1.FolderItem*\xd5\x01\n\x0eFolderItemType\x12\x1c\n\x18FOLDER_ITEM_TYPE_INVALID\x10\x00\x12\x12\n\x0eDERIVED_SIGNAL\x10\x01\x12\x14\n\x10PREDICTION_MODEL\x10\x02\x12\x16\n\x12PORTFOLIO_STRATEGY\x10\x03\x12\r\n\tDASHBOARD\x10\x04\x12\x0e\n\nDRILL_DOWN\x10\x05\x12\x07\n\x03TAG\x10\x06\x12\n\n\x06SCREEN\x10\x07\x12\x13\n\x0fFINANCIAL_MODEL\x10\x08\x12\t\n\x05CHART\x10\t\x12\x0f\n\x0bKPI_MAPPING\x10\nBS\n\x1ccom.exabel.api.management.v1B\x13FolderMessagesProtoP\x01Z\x1cexabel.com/api/management/v1b\x06proto3')
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.management.v1.folder_messages_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b'\n\x1ccom.exabel.api.management.v1B\x13FolderMessagesProtoP\x01Z\x1cexabel.com/api/management/v1'
     _FOLDER.fields_by_name['name']._options = None
     _FOLDER.fields_by_name['name']._serialized_options = b'\x92A\x1fJ\r"folders/123"\xca>\r\xfa\x02\nfolderName'
     _FOLDER.fields_by_name['display_name']._options = None
-    _FOLDER.fields_by_name['display_name']._serialized_options = b'\xe0A\x02\x92A\x14J\x12"My shared folder"'
+    _FOLDER.fields_by_name['display_name']._serialized_options = b'\x92A\x14J\x12"My shared folder"\xe2A\x01\x02'
     _FOLDER.fields_by_name['description']._options = None
     _FOLDER.fields_by_name['description']._serialized_options = b'\x92A\x1cJ\x1a"This is my shared folder"'
     _FOLDER.fields_by_name['write']._options = None
-    _FOLDER.fields_by_name['write']._serialized_options = b'\xe0A\x03'
+    _FOLDER.fields_by_name['write']._serialized_options = b'\xe2A\x01\x03'
     _FOLDER.fields_by_name['items']._options = None
-    _FOLDER.fields_by_name['items']._serialized_options = b'\xe0A\x06\xe0A\x03'
+    _FOLDER.fields_by_name['items']._serialized_options = b'\xe2A\x02\x06\x03'
     _FOLDERITEM.fields_by_name['parent']._options = None
     _FOLDERITEM.fields_by_name['parent']._serialized_options = b'\x92A\x1fJ\r"folders/123"\xca>\r\xfa\x02\nfolderName'
     _FOLDERITEM.fields_by_name['name']._options = None
-    _FOLDERITEM.fields_by_name['name']._serialized_options = b'\xe0A\x03\x92A\x16J\x14"derivedSignals/123"'
+    _FOLDERITEM.fields_by_name['name']._serialized_options = b'\x92A\x16J\x14"derivedSignals/123"\xe2A\x01\x03'
     _FOLDERITEM.fields_by_name['display_name']._options = None
     _FOLDERITEM.fields_by_name['display_name']._serialized_options = b'\x92A\rJ\x0b"my_signal"'
-    _FOLDERITEMTYPE._serialized_start = 1003
-    _FOLDERITEMTYPE._serialized_end = 1199
-    _FOLDER._serialized_start = 237
-    _FOLDER._serialized_end = 480
-    _FOLDERITEM._serialized_start = 483
-    _FOLDERITEM._serialized_end = 851
-    _FOLDERACCESSOR._serialized_start = 853
-    _FOLDERACCESSOR._serialized_end = 932
-    _SEARCHRESULT._serialized_start = 934
-    _SEARCHRESULT._serialized_end = 1000
+    _globals['_FOLDERITEMTYPE']._serialized_start = 1005
+    _globals['_FOLDERITEMTYPE']._serialized_end = 1218
+    _globals['_FOLDER']._serialized_start = 237
+    _globals['_FOLDER']._serialized_end = 481
+    _globals['_FOLDERITEM']._serialized_start = 484
+    _globals['_FOLDERITEM']._serialized_end = 853
+    _globals['_FOLDERACCESSOR']._serialized_start = 855
+    _globals['_FOLDERACCESSOR']._serialized_end = 934
+    _globals['_SEARCHRESULT']._serialized_start = 936
+    _globals['_SEARCHRESULT']._serialized_end = 1002
```

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/management/v1/library_service_pb2.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/management/v1/library_service_pb2.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,104 +1,105 @@
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 _sym_db = _symbol_database.Default()
 from .....exabel.api.management.v1 import folder_messages_pb2 as exabel_dot_api_dot_management_dot_v1_dot_folder__messages__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from google.api import field_behavior_pb2 as google_dot_api_dot_field__behavior__pb2
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 from google.protobuf import field_mask_pb2 as google_dot_protobuf_dot_field__mask__pb2
 from .....protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n.exabel/api/management/v1/library_service.proto\x12\x18exabel.api.management.v1\x1a.exabel/api/management/v1/folder_messages.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1fgoogle/api/field_behavior.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a google/protobuf/field_mask.proto\x1a.protoc_gen_openapiv2/options/annotations.proto"\x14\n\x12ListFoldersRequest"H\n\x13ListFoldersResponse\x121\n\x07folders\x18\x01 \x03(\x0b2 .exabel.api.management.v1.Folder"8\n\x10GetFolderRequest\x12$\n\x04name\x18\x01 \x01(\tB\x16\xe0A\x02\x92A\x10\xca>\r\xfa\x02\nfolderName"L\n\x13CreateFolderRequest\x125\n\x06folder\x18\x01 \x01(\x0b2 .exabel.api.management.v1.FolderB\x03\xe0A\x02"\x94\x01\n\x13UpdateFolderRequest\x125\n\x06folder\x18\x01 \x01(\x0b2 .exabel.api.management.v1.FolderB\x03\xe0A\x02\x12/\n\x0bupdate_mask\x18\x02 \x01(\x0b2\x1a.google.protobuf.FieldMask\x12\x15\n\rallow_missing\x18\x03 \x01(\x08";\n\x13DeleteFolderRequest\x12$\n\x04name\x18\x01 \x01(\tB\x16\xe0A\x02\x92A\x10\xca>\r\xfa\x02\nfolderName"\x86\x01\n\x10ListItemsRequest\x125\n\x06parent\x18\x01 \x01(\tB%\xe0A\x01\x92A\x1fJ\r"folders/123"\xca>\r\xfa\x02\nfolderName\x12;\n\titem_type\x18\x02 \x01(\x0e2(.exabel.api.management.v1.FolderItemType"H\n\x11ListItemsResponse\x123\n\x05items\x18\x01 \x03(\x0b2$.exabel.api.management.v1.FolderItem"U\n\x10MoveItemsRequest\x12\x12\n\x05items\x18\x01 \x03(\tB\x03\xe0A\x02\x12-\n\rtarget_folder\x18\x02 \x01(\tB\x16\xe0A\x02\x92A\x10\xca>\r\xfa\x02\nfolderName"\x13\n\x11MoveItemsResponse"?\n\x1aListFolderAccessorsRequest\x12!\n\x04name\x18\x01 \x01(\tB\x13\x92A\x10\xca>\r\xfa\x02\nfolderName"a\n\x1bListFolderAccessorsResponse\x12B\n\x10folder_accessors\x18\x01 \x03(\x0b2(.exabel.api.management.v1.FolderAccessor"y\n\x12ShareFolderRequest\x122\n\x06folder\x18\x01 \x01(\tB"\x92A\x1fJ\r"folders/123"\xca>\r\xfa\x02\nfolderName\x12 \n\x05group\x18\x02 \x01(\tB\x11\x92A\x0eJ\x0c"groups/123"\x12\r\n\x05write\x18\x03 \x01(\x08"l\n\x14UnshareFolderRequest\x122\n\x06folder\x18\x01 \x01(\tB"\x92A\x1fJ\r"folders/123"\xca>\r\xfa\x02\nfolderName\x12 \n\x05group\x18\x02 \x01(\tB\x11\x92A\x0eJ\x0c"groups/123""\xd0\x01\n\x12SearchItemsRequest\x12=\n\x06folder\x18\x01 \x01(\tB-\xe0A\x02\x92A\'J\x0b"folders/-"\xca>\x17\xfa\x02\x14folderNameAllFolders\x12\x12\n\x05query\x18\x02 \x01(\tB\x03\xe0A\x02\x12@\n\titem_type\x18\x03 \x01(\x0e2(.exabel.api.management.v1.FolderItemTypeB\x03\xe0A\x01\x12\x12\n\npage_token\x18\x04 \x01(\t\x12\x11\n\tpage_size\x18\x05 \x01(\x05"g\n\x13SearchItemsResponse\x127\n\x07results\x18\x01 \x03(\x0b2&.exabel.api.management.v1.SearchResult\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t2\xdc\r\n\x0eLibraryService\x12\x90\x01\n\x0bListFolders\x12,.exabel.api.management.v1.ListFoldersRequest\x1a-.exabel.api.management.v1.ListFoldersResponse"$\x82\xd3\xe4\x93\x02\r\x12\x0b/v1/folders\x92A\x0e\x12\x0cList folders\x12\x86\x01\n\tGetFolder\x12*.exabel.api.management.v1.GetFolderRequest\x1a .exabel.api.management.v1.Folder"+\x82\xd3\xe4\x93\x02\x16\x12\x14/v1/{name=folders/*}\x92A\x0c\x12\nGet folder\x12\x8e\x01\n\x0cCreateFolder\x12-.exabel.api.management.v1.CreateFolderRequest\x1a .exabel.api.management.v1.Folder"-\x82\xd3\xe4\x93\x02\x15"\x0b/v1/folders:\x06folder\x92A\x0f\x12\rCreate folder\x12\x9e\x01\n\x0cUpdateFolder\x12-.exabel.api.management.v1.UpdateFolderRequest\x1a .exabel.api.management.v1.Folder"=\x82\xd3\xe4\x93\x02%2\x1b/v1/{folder.name=folders/*}:\x06folder\x92A\x0f\x12\rUpdate folder\x12\x85\x01\n\x0cDeleteFolder\x12-.exabel.api.management.v1.DeleteFolderRequest\x1a\x16.google.protobuf.Empty".\x82\xd3\xe4\x93\x02\x16*\x14/v1/{name=folders/*}\x92A\x0f\x12\rDelete folder\x12\xa0\x01\n\tListItems\x12*.exabel.api.management.v1.ListItemsRequest\x1a+.exabel.api.management.v1.ListItemsResponse":\x82\xd3\xe4\x93\x02\x1e\x12\x1c/v1/{parent=folders/*}/items\x92A\x13\x12\x11List folder items\x12\xab\x01\n\tMoveItems\x12*.exabel.api.management.v1.MoveItemsRequest\x1a+.exabel.api.management.v1.MoveItemsResponse"E\x82\xd3\xe4\x93\x02)"\'/v1/{target_folder=folders/*}:moveItems\x92A\x13\x12\x11Move folder items\x12\xc4\x01\n\x13ListFolderAccessors\x124.exabel.api.management.v1.ListFolderAccessorsRequest\x1a5.exabel.api.management.v1.ListFolderAccessorsResponse"@\x82\xd3\xe4\x93\x02 \x12\x1e/v1/{name=folders/*}/accessors\x92A\x17\x12\x15List folder accessors\x12\x8d\x01\n\x0bShareFolder\x12,.exabel.api.management.v1.ShareFolderRequest\x1a\x16.google.protobuf.Empty"8\x82\xd3\xe4\x93\x02!"\x1c/v1/{folder=folders/*}:share:\x01*\x92A\x0e\x12\x0cShare folder\x12\x95\x01\n\rUnshareFolder\x12..exabel.api.management.v1.UnshareFolderRequest\x1a\x16.google.protobuf.Empty"<\x82\xd3\xe4\x93\x02#"\x1e/v1/{folder=folders/*}:unshare:\x01*\x92A\x10\x12\x0eUnshare folder\x12\xb3\x01\n\x0bSearchItems\x12,.exabel.api.management.v1.SearchItemsRequest\x1a-.exabel.api.management.v1.SearchItemsResponse"G\x82\xd3\xe4\x93\x02%\x12#/v1/{folder=folders/*}/items:search\x92A\x19\x12\x17Search for folder itemsBS\n\x1ccom.exabel.api.management.v1B\x13LibraryServiceProtoP\x01Z\x1cexabel.com/api/management/v1b\x06proto3')
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.management.v1.library_service_pb2', globals())
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n.exabel/api/management/v1/library_service.proto\x12\x18exabel.api.management.v1\x1a.exabel/api/management/v1/folder_messages.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1fgoogle/api/field_behavior.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a google/protobuf/field_mask.proto\x1a.protoc_gen_openapiv2/options/annotations.proto"\x14\n\x12ListFoldersRequest"H\n\x13ListFoldersResponse\x121\n\x07folders\x18\x01 \x03(\x0b2 .exabel.api.management.v1.Folder"9\n\x10GetFolderRequest\x12%\n\x04name\x18\x01 \x01(\tB\x17\x92A\x10\xca>\r\xfa\x02\nfolderName\xe2A\x01\x02"M\n\x13CreateFolderRequest\x126\n\x06folder\x18\x01 \x01(\x0b2 .exabel.api.management.v1.FolderB\x04\xe2A\x01\x02"\x95\x01\n\x13UpdateFolderRequest\x126\n\x06folder\x18\x01 \x01(\x0b2 .exabel.api.management.v1.FolderB\x04\xe2A\x01\x02\x12/\n\x0bupdate_mask\x18\x02 \x01(\x0b2\x1a.google.protobuf.FieldMask\x12\x15\n\rallow_missing\x18\x03 \x01(\x08"<\n\x13DeleteFolderRequest\x12%\n\x04name\x18\x01 \x01(\tB\x17\x92A\x10\xca>\r\xfa\x02\nfolderName\xe2A\x01\x02"\x87\x01\n\x10ListItemsRequest\x126\n\x06parent\x18\x01 \x01(\tB&\x92A\x1fJ\r"folders/123"\xca>\r\xfa\x02\nfolderName\xe2A\x01\x01\x12;\n\titem_type\x18\x02 \x01(\x0e2(.exabel.api.management.v1.FolderItemType"H\n\x11ListItemsResponse\x123\n\x05items\x18\x01 \x03(\x0b2$.exabel.api.management.v1.FolderItem"W\n\x10MoveItemsRequest\x12\x13\n\x05items\x18\x01 \x03(\tB\x04\xe2A\x01\x02\x12.\n\rtarget_folder\x18\x02 \x01(\tB\x17\x92A\x10\xca>\r\xfa\x02\nfolderName\xe2A\x01\x02"\x13\n\x11MoveItemsResponse"?\n\x1aListFolderAccessorsRequest\x12!\n\x04name\x18\x01 \x01(\tB\x13\x92A\x10\xca>\r\xfa\x02\nfolderName"a\n\x1bListFolderAccessorsResponse\x12B\n\x10folder_accessors\x18\x01 \x03(\x0b2(.exabel.api.management.v1.FolderAccessor"y\n\x12ShareFolderRequest\x122\n\x06folder\x18\x01 \x01(\tB"\x92A\x1fJ\r"folders/123"\xca>\r\xfa\x02\nfolderName\x12 \n\x05group\x18\x02 \x01(\tB\x11\x92A\x0eJ\x0c"groups/123"\x12\r\n\x05write\x18\x03 \x01(\x08"l\n\x14UnshareFolderRequest\x122\n\x06folder\x18\x01 \x01(\tB"\x92A\x1fJ\r"folders/123"\xca>\r\xfa\x02\nfolderName\x12 \n\x05group\x18\x02 \x01(\tB\x11\x92A\x0eJ\x0c"groups/123""\xd3\x01\n\x12SearchItemsRequest\x12>\n\x06folder\x18\x01 \x01(\tB.\x92A\'J\x0b"folders/-"\xca>\x17\xfa\x02\x14folderNameAllFolders\xe2A\x01\x02\x12\x13\n\x05query\x18\x02 \x01(\tB\x04\xe2A\x01\x02\x12A\n\titem_type\x18\x03 \x01(\x0e2(.exabel.api.management.v1.FolderItemTypeB\x04\xe2A\x01\x01\x12\x12\n\npage_token\x18\x04 \x01(\t\x12\x11\n\tpage_size\x18\x05 \x01(\x05"g\n\x13SearchItemsResponse\x127\n\x07results\x18\x01 \x03(\x0b2&.exabel.api.management.v1.SearchResult\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t2\xdc\r\n\x0eLibraryService\x12\x90\x01\n\x0bListFolders\x12,.exabel.api.management.v1.ListFoldersRequest\x1a-.exabel.api.management.v1.ListFoldersResponse"$\x92A\x0e\x12\x0cList folders\x82\xd3\xe4\x93\x02\r\x12\x0b/v1/folders\x12\x86\x01\n\tGetFolder\x12*.exabel.api.management.v1.GetFolderRequest\x1a .exabel.api.management.v1.Folder"+\x92A\x0c\x12\nGet folder\x82\xd3\xe4\x93\x02\x16\x12\x14/v1/{name=folders/*}\x12\x8e\x01\n\x0cCreateFolder\x12-.exabel.api.management.v1.CreateFolderRequest\x1a .exabel.api.management.v1.Folder"-\x92A\x0f\x12\rCreate folder\x82\xd3\xe4\x93\x02\x15"\x0b/v1/folders:\x06folder\x12\x9e\x01\n\x0cUpdateFolder\x12-.exabel.api.management.v1.UpdateFolderRequest\x1a .exabel.api.management.v1.Folder"=\x92A\x0f\x12\rUpdate folder\x82\xd3\xe4\x93\x02%2\x1b/v1/{folder.name=folders/*}:\x06folder\x12\x85\x01\n\x0cDeleteFolder\x12-.exabel.api.management.v1.DeleteFolderRequest\x1a\x16.google.protobuf.Empty".\x92A\x0f\x12\rDelete folder\x82\xd3\xe4\x93\x02\x16*\x14/v1/{name=folders/*}\x12\xa0\x01\n\tListItems\x12*.exabel.api.management.v1.ListItemsRequest\x1a+.exabel.api.management.v1.ListItemsResponse":\x92A\x13\x12\x11List folder items\x82\xd3\xe4\x93\x02\x1e\x12\x1c/v1/{parent=folders/*}/items\x12\xab\x01\n\tMoveItems\x12*.exabel.api.management.v1.MoveItemsRequest\x1a+.exabel.api.management.v1.MoveItemsResponse"E\x92A\x13\x12\x11Move folder items\x82\xd3\xe4\x93\x02)"\'/v1/{target_folder=folders/*}:moveItems\x12\xc4\x01\n\x13ListFolderAccessors\x124.exabel.api.management.v1.ListFolderAccessorsRequest\x1a5.exabel.api.management.v1.ListFolderAccessorsResponse"@\x92A\x17\x12\x15List folder accessors\x82\xd3\xe4\x93\x02 \x12\x1e/v1/{name=folders/*}/accessors\x12\x8d\x01\n\x0bShareFolder\x12,.exabel.api.management.v1.ShareFolderRequest\x1a\x16.google.protobuf.Empty"8\x92A\x0e\x12\x0cShare folder\x82\xd3\xe4\x93\x02!"\x1c/v1/{folder=folders/*}:share:\x01*\x12\x95\x01\n\rUnshareFolder\x12..exabel.api.management.v1.UnshareFolderRequest\x1a\x16.google.protobuf.Empty"<\x92A\x10\x12\x0eUnshare folder\x82\xd3\xe4\x93\x02#"\x1e/v1/{folder=folders/*}:unshare:\x01*\x12\xb3\x01\n\x0bSearchItems\x12,.exabel.api.management.v1.SearchItemsRequest\x1a-.exabel.api.management.v1.SearchItemsResponse"G\x92A\x19\x12\x17Search for folder items\x82\xd3\xe4\x93\x02%\x12#/v1/{folder=folders/*}/items:searchBS\n\x1ccom.exabel.api.management.v1B\x13LibraryServiceProtoP\x01Z\x1cexabel.com/api/management/v1b\x06proto3')
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.management.v1.library_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b'\n\x1ccom.exabel.api.management.v1B\x13LibraryServiceProtoP\x01Z\x1cexabel.com/api/management/v1'
     _GETFOLDERREQUEST.fields_by_name['name']._options = None
-    _GETFOLDERREQUEST.fields_by_name['name']._serialized_options = b'\xe0A\x02\x92A\x10\xca>\r\xfa\x02\nfolderName'
+    _GETFOLDERREQUEST.fields_by_name['name']._serialized_options = b'\x92A\x10\xca>\r\xfa\x02\nfolderName\xe2A\x01\x02'
     _CREATEFOLDERREQUEST.fields_by_name['folder']._options = None
-    _CREATEFOLDERREQUEST.fields_by_name['folder']._serialized_options = b'\xe0A\x02'
+    _CREATEFOLDERREQUEST.fields_by_name['folder']._serialized_options = b'\xe2A\x01\x02'
     _UPDATEFOLDERREQUEST.fields_by_name['folder']._options = None
-    _UPDATEFOLDERREQUEST.fields_by_name['folder']._serialized_options = b'\xe0A\x02'
+    _UPDATEFOLDERREQUEST.fields_by_name['folder']._serialized_options = b'\xe2A\x01\x02'
     _DELETEFOLDERREQUEST.fields_by_name['name']._options = None
-    _DELETEFOLDERREQUEST.fields_by_name['name']._serialized_options = b'\xe0A\x02\x92A\x10\xca>\r\xfa\x02\nfolderName'
+    _DELETEFOLDERREQUEST.fields_by_name['name']._serialized_options = b'\x92A\x10\xca>\r\xfa\x02\nfolderName\xe2A\x01\x02'
     _LISTITEMSREQUEST.fields_by_name['parent']._options = None
-    _LISTITEMSREQUEST.fields_by_name['parent']._serialized_options = b'\xe0A\x01\x92A\x1fJ\r"folders/123"\xca>\r\xfa\x02\nfolderName'
+    _LISTITEMSREQUEST.fields_by_name['parent']._serialized_options = b'\x92A\x1fJ\r"folders/123"\xca>\r\xfa\x02\nfolderName\xe2A\x01\x01'
     _MOVEITEMSREQUEST.fields_by_name['items']._options = None
-    _MOVEITEMSREQUEST.fields_by_name['items']._serialized_options = b'\xe0A\x02'
+    _MOVEITEMSREQUEST.fields_by_name['items']._serialized_options = b'\xe2A\x01\x02'
     _MOVEITEMSREQUEST.fields_by_name['target_folder']._options = None
-    _MOVEITEMSREQUEST.fields_by_name['target_folder']._serialized_options = b'\xe0A\x02\x92A\x10\xca>\r\xfa\x02\nfolderName'
+    _MOVEITEMSREQUEST.fields_by_name['target_folder']._serialized_options = b'\x92A\x10\xca>\r\xfa\x02\nfolderName\xe2A\x01\x02'
     _LISTFOLDERACCESSORSREQUEST.fields_by_name['name']._options = None
     _LISTFOLDERACCESSORSREQUEST.fields_by_name['name']._serialized_options = b'\x92A\x10\xca>\r\xfa\x02\nfolderName'
     _SHAREFOLDERREQUEST.fields_by_name['folder']._options = None
     _SHAREFOLDERREQUEST.fields_by_name['folder']._serialized_options = b'\x92A\x1fJ\r"folders/123"\xca>\r\xfa\x02\nfolderName'
     _SHAREFOLDERREQUEST.fields_by_name['group']._options = None
     _SHAREFOLDERREQUEST.fields_by_name['group']._serialized_options = b'\x92A\x0eJ\x0c"groups/123"'
     _UNSHAREFOLDERREQUEST.fields_by_name['folder']._options = None
     _UNSHAREFOLDERREQUEST.fields_by_name['folder']._serialized_options = b'\x92A\x1fJ\r"folders/123"\xca>\r\xfa\x02\nfolderName'
     _UNSHAREFOLDERREQUEST.fields_by_name['group']._options = None
     _UNSHAREFOLDERREQUEST.fields_by_name['group']._serialized_options = b'\x92A\x0eJ\x0c"groups/123"'
     _SEARCHITEMSREQUEST.fields_by_name['folder']._options = None
-    _SEARCHITEMSREQUEST.fields_by_name['folder']._serialized_options = b'\xe0A\x02\x92A\'J\x0b"folders/-"\xca>\x17\xfa\x02\x14folderNameAllFolders'
+    _SEARCHITEMSREQUEST.fields_by_name['folder']._serialized_options = b'\x92A\'J\x0b"folders/-"\xca>\x17\xfa\x02\x14folderNameAllFolders\xe2A\x01\x02'
     _SEARCHITEMSREQUEST.fields_by_name['query']._options = None
-    _SEARCHITEMSREQUEST.fields_by_name['query']._serialized_options = b'\xe0A\x02'
+    _SEARCHITEMSREQUEST.fields_by_name['query']._serialized_options = b'\xe2A\x01\x02'
     _SEARCHITEMSREQUEST.fields_by_name['item_type']._options = None
-    _SEARCHITEMSREQUEST.fields_by_name['item_type']._serialized_options = b'\xe0A\x01'
+    _SEARCHITEMSREQUEST.fields_by_name['item_type']._serialized_options = b'\xe2A\x01\x01'
     _LIBRARYSERVICE.methods_by_name['ListFolders']._options = None
-    _LIBRARYSERVICE.methods_by_name['ListFolders']._serialized_options = b'\x82\xd3\xe4\x93\x02\r\x12\x0b/v1/folders\x92A\x0e\x12\x0cList folders'
+    _LIBRARYSERVICE.methods_by_name['ListFolders']._serialized_options = b'\x92A\x0e\x12\x0cList folders\x82\xd3\xe4\x93\x02\r\x12\x0b/v1/folders'
     _LIBRARYSERVICE.methods_by_name['GetFolder']._options = None
-    _LIBRARYSERVICE.methods_by_name['GetFolder']._serialized_options = b'\x82\xd3\xe4\x93\x02\x16\x12\x14/v1/{name=folders/*}\x92A\x0c\x12\nGet folder'
+    _LIBRARYSERVICE.methods_by_name['GetFolder']._serialized_options = b'\x92A\x0c\x12\nGet folder\x82\xd3\xe4\x93\x02\x16\x12\x14/v1/{name=folders/*}'
     _LIBRARYSERVICE.methods_by_name['CreateFolder']._options = None
-    _LIBRARYSERVICE.methods_by_name['CreateFolder']._serialized_options = b'\x82\xd3\xe4\x93\x02\x15"\x0b/v1/folders:\x06folder\x92A\x0f\x12\rCreate folder'
+    _LIBRARYSERVICE.methods_by_name['CreateFolder']._serialized_options = b'\x92A\x0f\x12\rCreate folder\x82\xd3\xe4\x93\x02\x15"\x0b/v1/folders:\x06folder'
     _LIBRARYSERVICE.methods_by_name['UpdateFolder']._options = None
-    _LIBRARYSERVICE.methods_by_name['UpdateFolder']._serialized_options = b'\x82\xd3\xe4\x93\x02%2\x1b/v1/{folder.name=folders/*}:\x06folder\x92A\x0f\x12\rUpdate folder'
+    _LIBRARYSERVICE.methods_by_name['UpdateFolder']._serialized_options = b'\x92A\x0f\x12\rUpdate folder\x82\xd3\xe4\x93\x02%2\x1b/v1/{folder.name=folders/*}:\x06folder'
     _LIBRARYSERVICE.methods_by_name['DeleteFolder']._options = None
-    _LIBRARYSERVICE.methods_by_name['DeleteFolder']._serialized_options = b'\x82\xd3\xe4\x93\x02\x16*\x14/v1/{name=folders/*}\x92A\x0f\x12\rDelete folder'
+    _LIBRARYSERVICE.methods_by_name['DeleteFolder']._serialized_options = b'\x92A\x0f\x12\rDelete folder\x82\xd3\xe4\x93\x02\x16*\x14/v1/{name=folders/*}'
     _LIBRARYSERVICE.methods_by_name['ListItems']._options = None
-    _LIBRARYSERVICE.methods_by_name['ListItems']._serialized_options = b'\x82\xd3\xe4\x93\x02\x1e\x12\x1c/v1/{parent=folders/*}/items\x92A\x13\x12\x11List folder items'
+    _LIBRARYSERVICE.methods_by_name['ListItems']._serialized_options = b'\x92A\x13\x12\x11List folder items\x82\xd3\xe4\x93\x02\x1e\x12\x1c/v1/{parent=folders/*}/items'
     _LIBRARYSERVICE.methods_by_name['MoveItems']._options = None
-    _LIBRARYSERVICE.methods_by_name['MoveItems']._serialized_options = b'\x82\xd3\xe4\x93\x02)"\'/v1/{target_folder=folders/*}:moveItems\x92A\x13\x12\x11Move folder items'
+    _LIBRARYSERVICE.methods_by_name['MoveItems']._serialized_options = b'\x92A\x13\x12\x11Move folder items\x82\xd3\xe4\x93\x02)"\'/v1/{target_folder=folders/*}:moveItems'
     _LIBRARYSERVICE.methods_by_name['ListFolderAccessors']._options = None
-    _LIBRARYSERVICE.methods_by_name['ListFolderAccessors']._serialized_options = b'\x82\xd3\xe4\x93\x02 \x12\x1e/v1/{name=folders/*}/accessors\x92A\x17\x12\x15List folder accessors'
+    _LIBRARYSERVICE.methods_by_name['ListFolderAccessors']._serialized_options = b'\x92A\x17\x12\x15List folder accessors\x82\xd3\xe4\x93\x02 \x12\x1e/v1/{name=folders/*}/accessors'
     _LIBRARYSERVICE.methods_by_name['ShareFolder']._options = None
-    _LIBRARYSERVICE.methods_by_name['ShareFolder']._serialized_options = b'\x82\xd3\xe4\x93\x02!"\x1c/v1/{folder=folders/*}:share:\x01*\x92A\x0e\x12\x0cShare folder'
+    _LIBRARYSERVICE.methods_by_name['ShareFolder']._serialized_options = b'\x92A\x0e\x12\x0cShare folder\x82\xd3\xe4\x93\x02!"\x1c/v1/{folder=folders/*}:share:\x01*'
     _LIBRARYSERVICE.methods_by_name['UnshareFolder']._options = None
-    _LIBRARYSERVICE.methods_by_name['UnshareFolder']._serialized_options = b'\x82\xd3\xe4\x93\x02#"\x1e/v1/{folder=folders/*}:unshare:\x01*\x92A\x10\x12\x0eUnshare folder'
+    _LIBRARYSERVICE.methods_by_name['UnshareFolder']._serialized_options = b'\x92A\x10\x12\x0eUnshare folder\x82\xd3\xe4\x93\x02#"\x1e/v1/{folder=folders/*}:unshare:\x01*'
     _LIBRARYSERVICE.methods_by_name['SearchItems']._options = None
-    _LIBRARYSERVICE.methods_by_name['SearchItems']._serialized_options = b'\x82\xd3\xe4\x93\x02%\x12#/v1/{folder=folders/*}/items:search\x92A\x19\x12\x17Search for folder items'
-    _LISTFOLDERSREQUEST._serialized_start = 298
-    _LISTFOLDERSREQUEST._serialized_end = 318
-    _LISTFOLDERSRESPONSE._serialized_start = 320
-    _LISTFOLDERSRESPONSE._serialized_end = 392
-    _GETFOLDERREQUEST._serialized_start = 394
-    _GETFOLDERREQUEST._serialized_end = 450
-    _CREATEFOLDERREQUEST._serialized_start = 452
-    _CREATEFOLDERREQUEST._serialized_end = 528
-    _UPDATEFOLDERREQUEST._serialized_start = 531
-    _UPDATEFOLDERREQUEST._serialized_end = 679
-    _DELETEFOLDERREQUEST._serialized_start = 681
-    _DELETEFOLDERREQUEST._serialized_end = 740
-    _LISTITEMSREQUEST._serialized_start = 743
-    _LISTITEMSREQUEST._serialized_end = 877
-    _LISTITEMSRESPONSE._serialized_start = 879
-    _LISTITEMSRESPONSE._serialized_end = 951
-    _MOVEITEMSREQUEST._serialized_start = 953
-    _MOVEITEMSREQUEST._serialized_end = 1038
-    _MOVEITEMSRESPONSE._serialized_start = 1040
-    _MOVEITEMSRESPONSE._serialized_end = 1059
-    _LISTFOLDERACCESSORSREQUEST._serialized_start = 1061
-    _LISTFOLDERACCESSORSREQUEST._serialized_end = 1124
-    _LISTFOLDERACCESSORSRESPONSE._serialized_start = 1126
-    _LISTFOLDERACCESSORSRESPONSE._serialized_end = 1223
-    _SHAREFOLDERREQUEST._serialized_start = 1225
-    _SHAREFOLDERREQUEST._serialized_end = 1346
-    _UNSHAREFOLDERREQUEST._serialized_start = 1348
-    _UNSHAREFOLDERREQUEST._serialized_end = 1456
-    _SEARCHITEMSREQUEST._serialized_start = 1459
-    _SEARCHITEMSREQUEST._serialized_end = 1667
-    _SEARCHITEMSRESPONSE._serialized_start = 1669
-    _SEARCHITEMSRESPONSE._serialized_end = 1772
-    _LIBRARYSERVICE._serialized_start = 1775
-    _LIBRARYSERVICE._serialized_end = 3531
+    _LIBRARYSERVICE.methods_by_name['SearchItems']._serialized_options = b'\x92A\x19\x12\x17Search for folder items\x82\xd3\xe4\x93\x02%\x12#/v1/{folder=folders/*}/items:search'
+    _globals['_LISTFOLDERSREQUEST']._serialized_start = 298
+    _globals['_LISTFOLDERSREQUEST']._serialized_end = 318
+    _globals['_LISTFOLDERSRESPONSE']._serialized_start = 320
+    _globals['_LISTFOLDERSRESPONSE']._serialized_end = 392
+    _globals['_GETFOLDERREQUEST']._serialized_start = 394
+    _globals['_GETFOLDERREQUEST']._serialized_end = 451
+    _globals['_CREATEFOLDERREQUEST']._serialized_start = 453
+    _globals['_CREATEFOLDERREQUEST']._serialized_end = 530
+    _globals['_UPDATEFOLDERREQUEST']._serialized_start = 533
+    _globals['_UPDATEFOLDERREQUEST']._serialized_end = 682
+    _globals['_DELETEFOLDERREQUEST']._serialized_start = 684
+    _globals['_DELETEFOLDERREQUEST']._serialized_end = 744
+    _globals['_LISTITEMSREQUEST']._serialized_start = 747
+    _globals['_LISTITEMSREQUEST']._serialized_end = 882
+    _globals['_LISTITEMSRESPONSE']._serialized_start = 884
+    _globals['_LISTITEMSRESPONSE']._serialized_end = 956
+    _globals['_MOVEITEMSREQUEST']._serialized_start = 958
+    _globals['_MOVEITEMSREQUEST']._serialized_end = 1045
+    _globals['_MOVEITEMSRESPONSE']._serialized_start = 1047
+    _globals['_MOVEITEMSRESPONSE']._serialized_end = 1066
+    _globals['_LISTFOLDERACCESSORSREQUEST']._serialized_start = 1068
+    _globals['_LISTFOLDERACCESSORSREQUEST']._serialized_end = 1131
+    _globals['_LISTFOLDERACCESSORSRESPONSE']._serialized_start = 1133
+    _globals['_LISTFOLDERACCESSORSRESPONSE']._serialized_end = 1230
+    _globals['_SHAREFOLDERREQUEST']._serialized_start = 1232
+    _globals['_SHAREFOLDERREQUEST']._serialized_end = 1353
+    _globals['_UNSHAREFOLDERREQUEST']._serialized_start = 1355
+    _globals['_UNSHAREFOLDERREQUEST']._serialized_end = 1463
+    _globals['_SEARCHITEMSREQUEST']._serialized_start = 1466
+    _globals['_SEARCHITEMSREQUEST']._serialized_end = 1677
+    _globals['_SEARCHITEMSRESPONSE']._serialized_start = 1679
+    _globals['_SEARCHITEMSRESPONSE']._serialized_end = 1782
+    _globals['_LIBRARYSERVICE']._serialized_start = 1785
+    _globals['_LIBRARYSERVICE']._serialized_end = 3541
```

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/management/v1/library_service_pb2_grpc.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/management/v1/library_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/management/v1/service_pb2.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/management/v1/service_pb2.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 _sym_db = _symbol_database.Default()
 from .....protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n&exabel/api/management/v1/service.proto\x12\x18exabel.api.management.v1\x1a.protoc_gen_openapiv2/options/annotations.protoB\xeb\x02\n\x1ccom.exabel.api.management.v1B\x0cServiceProtoP\x01Z\x1cexabel.com/api/management/v1\x92A\x9b\x02\x12U\n\x15Exabel Management API"5\n\x06Exabel\x12\x17https://www.exabel.com/\x1a\x12support@exabel.com2\x051.0.0\x1a\x19management.api.exabel.com*\x01\x022\x10application/json:\x10application/jsonZ\x1c\n\x1a\n\x07API key\x12\x0f\x08\x02\x1a\tx-api-key \x02b\r\n\x0b\n\x07API key\x12\x00rS\n$More about the Exabel Management API\x12+https://help.exabel.com/docs/management-apib\x06proto3')
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.management.v1.service_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.management.v1.service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b'\n\x1ccom.exabel.api.management.v1B\x0cServiceProtoP\x01Z\x1cexabel.com/api/management/v1\x92A\x9b\x02\x12U\n\x15Exabel Management API"5\n\x06Exabel\x12\x17https://www.exabel.com/\x1a\x12support@exabel.com2\x051.0.0\x1a\x19management.api.exabel.com*\x01\x022\x10application/json:\x10application/jsonZ\x1c\n\x1a\n\x07API key\x12\x0f\x08\x02\x1a\tx-api-key \x02b\r\n\x0b\n\x07API key\x12\x00rS\n$More about the Exabel Management API\x12+https://help.exabel.com/docs/management-api'
```

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_messages_pb2.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/time/time_range_pb2.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 _sym_db = _symbol_database.Default()
-from google.api import field_behavior_pb2 as google_dot_api_dot_field__behavior__pb2
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n,exabel/api/management/v1/user_messages.proto\x12\x18exabel.api.management.v1\x1a\x1fgoogle/api/field_behavior.proto"9\n\x04User\x12\x11\n\x04name\x18\x01 \x01(\tB\x03\xe0A\x03\x12\r\n\x05email\x18\x02 \x01(\t\x12\x0f\n\x07blocked\x18\x03 \x01(\x08"_\n\x05Group\x12\x11\n\x04name\x18\x01 \x01(\tB\x03\xe0A\x03\x12\x14\n\x0cdisplay_name\x18\x02 \x01(\t\x12-\n\x05users\x18\x03 \x03(\x0b2\x1e.exabel.api.management.v1.UserBQ\n\x1ccom.exabel.api.management.v1B\x11UserMessagesProtoP\x01Z\x1cexabel.com/api/management/v1b\x06proto3')
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.management.v1.user_messages_pb2', globals())
+from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n exabel/api/time/time_range.proto\x12\x0fexabel.api.time\x1a\x1fgoogle/protobuf/timestamp.proto"\x91\x01\n\tTimeRange\x12-\n\tfrom_time\x18\x01 \x01(\x0b2\x1a.google.protobuf.Timestamp\x12\x14\n\x0cexclude_from\x18\x02 \x01(\x08\x12+\n\x07to_time\x18\x03 \x01(\x0b2\x1a.google.protobuf.Timestamp\x12\x12\n\ninclude_to\x18\x04 \x01(\x08B<\n\x13com.exabel.api.timeB\x0eTimeRangeProtoP\x01Z\x13exabel.com/api/timeb\x06proto3')
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.time.time_range_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    DESCRIPTOR._serialized_options = b'\n\x1ccom.exabel.api.management.v1B\x11UserMessagesProtoP\x01Z\x1cexabel.com/api/management/v1'
-    _USER.fields_by_name['name']._options = None
-    _USER.fields_by_name['name']._serialized_options = b'\xe0A\x03'
-    _GROUP.fields_by_name['name']._options = None
-    _GROUP.fields_by_name['name']._serialized_options = b'\xe0A\x03'
-    _USER._serialized_start = 107
-    _USER._serialized_end = 164
-    _GROUP._serialized_start = 166
-    _GROUP._serialized_end = 261
+    DESCRIPTOR._serialized_options = b'\n\x13com.exabel.api.timeB\x0eTimeRangeProtoP\x01Z\x13exabel.com/api/time'
+    _globals['_TIMERANGE']._serialized_start = 87
+    _globals['_TIMERANGE']._serialized_end = 232
```

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_service_pb2.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_service_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 _sym_db = _symbol_database.Default()
 from .....exabel.api.management.v1 import user_messages_pb2 as exabel_dot_api_dot_management_dot_v1_dot_user__messages__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from .....protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n+exabel/api/management/v1/user_service.proto\x12\x18exabel.api.management.v1\x1a,exabel/api/management/v1/user_messages.proto\x1a\x1cgoogle/api/annotations.proto\x1a.protoc_gen_openapiv2/options/annotations.proto"\x13\n\x11ListGroupsRequest"E\n\x12ListGroupsResponse\x12/\n\x06groups\x18\x01 \x03(\x0b2\x1f.exabel.api.management.v1.Group"\x12\n\x10ListUsersRequest"B\n\x11ListUsersResponse\x12-\n\x05users\x18\x01 \x03(\x0b2\x1e.exabel.api.management.v1.User2\xa4\x02\n\x0bUserService\x12\x8b\x01\n\nListGroups\x12+.exabel.api.management.v1.ListGroupsRequest\x1a,.exabel.api.management.v1.ListGroupsResponse""\x82\xd3\xe4\x93\x02\x0c\x12\n/v1/groups\x92A\r\x12\x0bList groups\x12\x86\x01\n\tListUsers\x12*.exabel.api.management.v1.ListUsersRequest\x1a+.exabel.api.management.v1.ListUsersResponse" \x82\xd3\xe4\x93\x02\x0b\x12\t/v1/users\x92A\x0c\x12\nList usersBP\n\x1ccom.exabel.api.management.v1B\x10UserServiceProtoP\x01Z\x1cexabel.com/api/management/v1b\x06proto3')
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.management.v1.user_service_pb2', globals())
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n+exabel/api/management/v1/user_service.proto\x12\x18exabel.api.management.v1\x1a,exabel/api/management/v1/user_messages.proto\x1a\x1cgoogle/api/annotations.proto\x1a.protoc_gen_openapiv2/options/annotations.proto"\x13\n\x11ListGroupsRequest"E\n\x12ListGroupsResponse\x12/\n\x06groups\x18\x01 \x03(\x0b2\x1f.exabel.api.management.v1.Group"\x12\n\x10ListUsersRequest"B\n\x11ListUsersResponse\x12-\n\x05users\x18\x01 \x03(\x0b2\x1e.exabel.api.management.v1.User2\xa4\x02\n\x0bUserService\x12\x8b\x01\n\nListGroups\x12+.exabel.api.management.v1.ListGroupsRequest\x1a,.exabel.api.management.v1.ListGroupsResponse""\x92A\r\x12\x0bList groups\x82\xd3\xe4\x93\x02\x0c\x12\n/v1/groups\x12\x86\x01\n\tListUsers\x12*.exabel.api.management.v1.ListUsersRequest\x1a+.exabel.api.management.v1.ListUsersResponse" \x92A\x0c\x12\nList users\x82\xd3\xe4\x93\x02\x0b\x12\t/v1/usersBP\n\x1ccom.exabel.api.management.v1B\x10UserServiceProtoP\x01Z\x1cexabel.com/api/management/v1b\x06proto3')
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.management.v1.user_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b'\n\x1ccom.exabel.api.management.v1B\x10UserServiceProtoP\x01Z\x1cexabel.com/api/management/v1'
     _USERSERVICE.methods_by_name['ListGroups']._options = None
-    _USERSERVICE.methods_by_name['ListGroups']._serialized_options = b'\x82\xd3\xe4\x93\x02\x0c\x12\n/v1/groups\x92A\r\x12\x0bList groups'
+    _USERSERVICE.methods_by_name['ListGroups']._serialized_options = b'\x92A\r\x12\x0bList groups\x82\xd3\xe4\x93\x02\x0c\x12\n/v1/groups'
     _USERSERVICE.methods_by_name['ListUsers']._options = None
-    _USERSERVICE.methods_by_name['ListUsers']._serialized_options = b'\x82\xd3\xe4\x93\x02\x0b\x12\t/v1/users\x92A\x0c\x12\nList users'
-    _LISTGROUPSREQUEST._serialized_start = 197
-    _LISTGROUPSREQUEST._serialized_end = 216
-    _LISTGROUPSRESPONSE._serialized_start = 218
-    _LISTGROUPSRESPONSE._serialized_end = 287
-    _LISTUSERSREQUEST._serialized_start = 289
-    _LISTUSERSREQUEST._serialized_end = 307
-    _LISTUSERSRESPONSE._serialized_start = 309
-    _LISTUSERSRESPONSE._serialized_end = 375
-    _USERSERVICE._serialized_start = 378
-    _USERSERVICE._serialized_end = 670
+    _USERSERVICE.methods_by_name['ListUsers']._serialized_options = b'\x92A\x0c\x12\nList users\x82\xd3\xe4\x93\x02\x0b\x12\t/v1/users'
+    _globals['_LISTGROUPSREQUEST']._serialized_start = 197
+    _globals['_LISTGROUPSREQUEST']._serialized_end = 216
+    _globals['_LISTGROUPSRESPONSE']._serialized_start = 218
+    _globals['_LISTGROUPSRESPONSE']._serialized_end = 287
+    _globals['_LISTUSERSREQUEST']._serialized_start = 289
+    _globals['_LISTUSERSREQUEST']._serialized_end = 307
+    _globals['_LISTUSERSRESPONSE']._serialized_start = 309
+    _globals['_LISTUSERSRESPONSE']._serialized_end = 375
+    _globals['_USERSERVICE']._serialized_start = 378
+    _globals['_USERSERVICE']._serialized_end = 670
```

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_service_pb2_grpc.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/exabel/api/math/aggregation_pb2.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/exabel/api/math/aggregation_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 _sym_db = _symbol_database.Default()
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!exabel/api/math/aggregation.proto\x12\x0fexabel.api.math*`\n\x0bAggregation\x12\x17\n\x13AGGREGATION_INVALID\x10\x00\x12\x08\n\x04MEAN\x10\x01\x12\t\n\x05FIRST\x10\x02\x12\x08\n\x04LAST\x10\x03\x12\x07\n\x03SUM\x10\x04\x12\x07\n\x03MIN\x10\x05\x12\x07\n\x03MAX\x10\x06B>\n\x13com.exabel.api.mathB\x10AggregationProtoP\x01Z\x13exabel.com/api/mathb\x06proto3')
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.math.aggregation_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.math.aggregation_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b'\n\x13com.exabel.api.mathB\x10AggregationProtoP\x01Z\x13exabel.com/api/math'
-    _AGGREGATION._serialized_start = 54
-    _AGGREGATION._serialized_end = 150
+    _globals['_AGGREGATION']._serialized_start = 54
+    _globals['_AGGREGATION']._serialized_end = 150
```

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/annotations_pb2.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/annotations_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 _sym_db = _symbol_database.Default()
 from google.protobuf import descriptor_pb2 as google_dot_protobuf_dot_descriptor__pb2
 from ...protoc_gen_openapiv2.options import openapiv2_pb2 as protoc__gen__openapiv2_dot_options_dot_openapiv2__pb2
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n.protoc_gen_openapiv2/options/annotations.proto\x12)grpc.gateway.protoc_gen_openapiv2.options\x1a google/protobuf/descriptor.proto\x1a,protoc_gen_openapiv2/options/openapiv2.proto:l\n\x11openapiv2_swagger\x12\x1c.google.protobuf.FileOptions\x18\x92\x08 \x01(\x0b22.grpc.gateway.protoc_gen_openapiv2.options.Swagger:r\n\x13openapiv2_operation\x12\x1e.google.protobuf.MethodOptions\x18\x92\x08 \x01(\x0b24.grpc.gateway.protoc_gen_openapiv2.options.Operation:m\n\x10openapiv2_schema\x12\x1f.google.protobuf.MessageOptions\x18\x92\x08 \x01(\x0b21.grpc.gateway.protoc_gen_openapiv2.options.Schema:g\n\ropenapiv2_tag\x12\x1f.google.protobuf.ServiceOptions\x18\x92\x08 \x01(\x0b2..grpc.gateway.protoc_gen_openapiv2.options.Tag:n\n\x0fopenapiv2_field\x12\x1d.google.protobuf.FieldOptions\x18\x92\x08 \x01(\x0b25.grpc.gateway.protoc_gen_openapiv2.options.JSONSchemaBHZFgithub.com/grpc-ecosystem/grpc-gateway/v2/protoc-gen-openapiv2/optionsb\x06proto3')
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'protoc_gen_openapiv2.options.annotations_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'protoc_gen_openapiv2.options.annotations_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     google_dot_protobuf_dot_descriptor__pb2.FileOptions.RegisterExtension(openapiv2_swagger)
     google_dot_protobuf_dot_descriptor__pb2.MethodOptions.RegisterExtension(openapiv2_operation)
     google_dot_protobuf_dot_descriptor__pb2.MessageOptions.RegisterExtension(openapiv2_schema)
     google_dot_protobuf_dot_descriptor__pb2.ServiceOptions.RegisterExtension(openapiv2_tag)
     google_dot_protobuf_dot_descriptor__pb2.FieldOptions.RegisterExtension(openapiv2_field)
     DESCRIPTOR._options = None
```

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/openapiv2_pb2.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/openapiv2_pb2.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 _sym_db = _symbol_database.Default()
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n,protoc_gen_openapiv2/options/openapiv2.proto\x12)grpc.gateway.protoc_gen_openapiv2.options\x1a\x1cgoogle/protobuf/struct.proto"\xdd\x06\n\x07Swagger\x12\x0f\n\x07swagger\x18\x01 \x01(\t\x12=\n\x04info\x18\x02 \x01(\x0b2/.grpc.gateway.protoc_gen_openapiv2.options.Info\x12\x0c\n\x04host\x18\x03 \x01(\t\x12\x11\n\tbase_path\x18\x04 \x01(\t\x12B\n\x07schemes\x18\x05 \x03(\x0e21.grpc.gateway.protoc_gen_openapiv2.options.Scheme\x12\x10\n\x08consumes\x18\x06 \x03(\t\x12\x10\n\x08produces\x18\x07 \x03(\t\x12T\n\tresponses\x18\n \x03(\x0b2A.grpc.gateway.protoc_gen_openapiv2.options.Swagger.ResponsesEntry\x12\\\n\x14security_definitions\x18\x0b \x01(\x0b2>.grpc.gateway.protoc_gen_openapiv2.options.SecurityDefinitions\x12P\n\x08security\x18\x0c \x03(\x0b2>.grpc.gateway.protoc_gen_openapiv2.options.SecurityRequirement\x12W\n\rexternal_docs\x18\x0e \x01(\x0b2@.grpc.gateway.protoc_gen_openapiv2.options.ExternalDocumentation\x12V\n\nextensions\x18\x0f \x03(\x0b2B.grpc.gateway.protoc_gen_openapiv2.options.Swagger.ExtensionsEntry\x1ae\n\x0eResponsesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12B\n\x05value\x18\x02 \x01(\x0b23.grpc.gateway.protoc_gen_openapiv2.options.Response:\x028\x01\x1aI\n\x0fExtensionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12%\n\x05value\x18\x02 \x01(\x0b2\x16.google.protobuf.Value:\x028\x01J\x04\x08\x08\x10\tJ\x04\x08\t\x10\nJ\x04\x08\r\x10\x0e"\xe6\x05\n\tOperation\x12\x0c\n\x04tags\x18\x01 \x03(\t\x12\x0f\n\x07summary\x18\x02 \x01(\t\x12\x13\n\x0bdescription\x18\x03 \x01(\t\x12W\n\rexternal_docs\x18\x04 \x01(\x0b2@.grpc.gateway.protoc_gen_openapiv2.options.ExternalDocumentation\x12\x14\n\x0coperation_id\x18\x05 \x01(\t\x12\x10\n\x08consumes\x18\x06 \x03(\t\x12\x10\n\x08produces\x18\x07 \x03(\t\x12V\n\tresponses\x18\t \x03(\x0b2C.grpc.gateway.protoc_gen_openapiv2.options.Operation.ResponsesEntry\x12B\n\x07schemes\x18\n \x03(\x0e21.grpc.gateway.protoc_gen_openapiv2.options.Scheme\x12\x12\n\ndeprecated\x18\x0b \x01(\x08\x12P\n\x08security\x18\x0c \x03(\x0b2>.grpc.gateway.protoc_gen_openapiv2.options.SecurityRequirement\x12X\n\nextensions\x18\r \x03(\x0b2D.grpc.gateway.protoc_gen_openapiv2.options.Operation.ExtensionsEntry\x1ae\n\x0eResponsesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12B\n\x05value\x18\x02 \x01(\x0b23.grpc.gateway.protoc_gen_openapiv2.options.Response:\x028\x01\x1aI\n\x0fExtensionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12%\n\x05value\x18\x02 \x01(\x0b2\x16.google.protobuf.Value:\x028\x01J\x04\x08\x08\x10\t"\xab\x01\n\x06Header\x12\x13\n\x0bdescription\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x0e\n\x06format\x18\x03 \x01(\t\x12\x0f\n\x07default\x18\x06 \x01(\t\x12\x0f\n\x07pattern\x18\r \x01(\tJ\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x07\x10\x08J\x04\x08\x08\x10\tJ\x04\x08\t\x10\nJ\x04\x08\n\x10\x0bJ\x04\x08\x0b\x10\x0cJ\x04\x08\x0c\x10\rJ\x04\x08\x0e\x10\x0fJ\x04\x08\x0f\x10\x10J\x04\x08\x10\x10\x11J\x04\x08\x11\x10\x12J\x04\x08\x12\x10\x13"\xc2\x04\n\x08Response\x12\x13\n\x0bdescription\x18\x01 \x01(\t\x12A\n\x06schema\x18\x02 \x01(\x0b21.grpc.gateway.protoc_gen_openapiv2.options.Schema\x12Q\n\x07headers\x18\x03 \x03(\x0b2@.grpc.gateway.protoc_gen_openapiv2.options.Response.HeadersEntry\x12S\n\x08examples\x18\x04 \x03(\x0b2A.grpc.gateway.protoc_gen_openapiv2.options.Response.ExamplesEntry\x12W\n\nextensions\x18\x05 \x03(\x0b2C.grpc.gateway.protoc_gen_openapiv2.options.Response.ExtensionsEntry\x1aa\n\x0cHeadersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12@\n\x05value\x18\x02 \x01(\x0b21.grpc.gateway.protoc_gen_openapiv2.options.Header:\x028\x01\x1a/\n\rExamplesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x028\x01\x1aI\n\x0fExtensionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12%\n\x05value\x18\x02 \x01(\x0b2\x16.google.protobuf.Value:\x028\x01"\xff\x02\n\x04Info\x12\r\n\x05title\x18\x01 \x01(\t\x12\x13\n\x0bdescription\x18\x02 \x01(\t\x12\x18\n\x10terms_of_service\x18\x03 \x01(\t\x12C\n\x07contact\x18\x04 \x01(\x0b22.grpc.gateway.protoc_gen_openapiv2.options.Contact\x12C\n\x07license\x18\x05 \x01(\x0b22.grpc.gateway.protoc_gen_openapiv2.options.License\x12\x0f\n\x07version\x18\x06 \x01(\t\x12S\n\nextensions\x18\x07 \x03(\x0b2?.grpc.gateway.protoc_gen_openapiv2.options.Info.ExtensionsEntry\x1aI\n\x0fExtensionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12%\n\x05value\x18\x02 \x01(\x0b2\x16.google.protobuf.Value:\x028\x01"3\n\x07Contact\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0b\n\x03url\x18\x02 \x01(\t\x12\r\n\x05email\x18\x03 \x01(\t"$\n\x07License\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0b\n\x03url\x18\x02 \x01(\t"9\n\x15ExternalDocumentation\x12\x13\n\x0bdescription\x18\x01 \x01(\t\x12\x0b\n\x03url\x18\x02 \x01(\t"\xee\x01\n\x06Schema\x12J\n\x0bjson_schema\x18\x01 \x01(\x0b25.grpc.gateway.protoc_gen_openapiv2.options.JSONSchema\x12\x15\n\rdiscriminator\x18\x02 \x01(\t\x12\x11\n\tread_only\x18\x03 \x01(\x08\x12W\n\rexternal_docs\x18\x05 \x01(\x0b2@.grpc.gateway.protoc_gen_openapiv2.options.ExternalDocumentation\x12\x0f\n\x07example\x18\x06 \x01(\tJ\x04\x08\x04\x10\x05"\xfc\x06\n\nJSONSchema\x12\x0b\n\x03ref\x18\x03 \x01(\t\x12\r\n\x05title\x18\x05 \x01(\t\x12\x13\n\x0bdescription\x18\x06 \x01(\t\x12\x0f\n\x07default\x18\x07 \x01(\t\x12\x11\n\tread_only\x18\x08 \x01(\x08\x12\x0f\n\x07example\x18\t \x01(\t\x12\x13\n\x0bmultiple_of\x18\n \x01(\x01\x12\x0f\n\x07maximum\x18\x0b \x01(\x01\x12\x19\n\x11exclusive_maximum\x18\x0c \x01(\x08\x12\x0f\n\x07minimum\x18\r \x01(\x01\x12\x19\n\x11exclusive_minimum\x18\x0e \x01(\x08\x12\x12\n\nmax_length\x18\x0f \x01(\x04\x12\x12\n\nmin_length\x18\x10 \x01(\x04\x12\x0f\n\x07pattern\x18\x11 \x01(\t\x12\x11\n\tmax_items\x18\x14 \x01(\x04\x12\x11\n\tmin_items\x18\x15 \x01(\x04\x12\x14\n\x0cunique_items\x18\x16 \x01(\x08\x12\x16\n\x0emax_properties\x18\x18 \x01(\x04\x12\x16\n\x0emin_properties\x18\x19 \x01(\x04\x12\x10\n\x08required\x18\x1a \x03(\t\x12\r\n\x05array\x18" \x03(\t\x12Y\n\x04type\x18# \x03(\x0e2K.grpc.gateway.protoc_gen_openapiv2.options.JSONSchema.JSONSchemaSimpleTypes\x12\x0e\n\x06format\x18$ \x01(\t\x12\x0c\n\x04enum\x18. \x03(\t\x12f\n\x13field_configuration\x18\xe9\x07 \x01(\x0b2H.grpc.gateway.protoc_gen_openapiv2.options.JSONSchema.FieldConfiguration\x1a-\n\x12FieldConfiguration\x12\x17\n\x0fpath_param_name\x18/ \x01(\t"w\n\x15JSONSchemaSimpleTypes\x12\x0b\n\x07UNKNOWN\x10\x00\x12\t\n\x05ARRAY\x10\x01\x12\x0b\n\x07BOOLEAN\x10\x02\x12\x0b\n\x07INTEGER\x10\x03\x12\x08\n\x04NULL\x10\x04\x12\n\n\x06NUMBER\x10\x05\x12\n\n\x06OBJECT\x10\x06\x12\n\n\x06STRING\x10\x07J\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03J\x04\x08\x04\x10\x05J\x04\x08\x12\x10\x13J\x04\x08\x13\x10\x14J\x04\x08\x17\x10\x18J\x04\x08\x1b\x10\x1cJ\x04\x08\x1c\x10\x1dJ\x04\x08\x1d\x10\x1eJ\x04\x08\x1e\x10"J\x04\x08%\x10*J\x04\x08*\x10+J\x04\x08+\x10."y\n\x03Tag\x12\x13\n\x0bdescription\x18\x02 \x01(\t\x12W\n\rexternal_docs\x18\x03 \x01(\x0b2@.grpc.gateway.protoc_gen_openapiv2.options.ExternalDocumentationJ\x04\x08\x01\x10\x02"\xe1\x01\n\x13SecurityDefinitions\x12^\n\x08security\x18\x01 \x03(\x0b2L.grpc.gateway.protoc_gen_openapiv2.options.SecurityDefinitions.SecurityEntry\x1aj\n\rSecurityEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12H\n\x05value\x18\x02 \x01(\x0b29.grpc.gateway.protoc_gen_openapiv2.options.SecurityScheme:\x028\x01"\xa0\x06\n\x0eSecurityScheme\x12L\n\x04type\x18\x01 \x01(\x0e2>.grpc.gateway.protoc_gen_openapiv2.options.SecurityScheme.Type\x12\x13\n\x0bdescription\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12H\n\x02in\x18\x04 \x01(\x0e2<.grpc.gateway.protoc_gen_openapiv2.options.SecurityScheme.In\x12L\n\x04flow\x18\x05 \x01(\x0e2>.grpc.gateway.protoc_gen_openapiv2.options.SecurityScheme.Flow\x12\x19\n\x11authorization_url\x18\x06 \x01(\t\x12\x11\n\ttoken_url\x18\x07 \x01(\t\x12A\n\x06scopes\x18\x08 \x01(\x0b21.grpc.gateway.protoc_gen_openapiv2.options.Scopes\x12]\n\nextensions\x18\t \x03(\x0b2I.grpc.gateway.protoc_gen_openapiv2.options.SecurityScheme.ExtensionsEntry\x1aI\n\x0fExtensionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12%\n\x05value\x18\x02 \x01(\x0b2\x16.google.protobuf.Value:\x028\x01"K\n\x04Type\x12\x10\n\x0cTYPE_INVALID\x10\x00\x12\x0e\n\nTYPE_BASIC\x10\x01\x12\x10\n\x0cTYPE_API_KEY\x10\x02\x12\x0f\n\x0bTYPE_OAUTH2\x10\x03"1\n\x02In\x12\x0e\n\nIN_INVALID\x10\x00\x12\x0c\n\x08IN_QUERY\x10\x01\x12\r\n\tIN_HEADER\x10\x02"j\n\x04Flow\x12\x10\n\x0cFLOW_INVALID\x10\x00\x12\x11\n\rFLOW_IMPLICIT\x10\x01\x12\x11\n\rFLOW_PASSWORD\x10\x02\x12\x14\n\x10FLOW_APPLICATION\x10\x03\x12\x14\n\x10FLOW_ACCESS_CODE\x10\x04"\xcd\x02\n\x13SecurityRequirement\x12u\n\x14security_requirement\x18\x01 \x03(\x0b2W.grpc.gateway.protoc_gen_openapiv2.options.SecurityRequirement.SecurityRequirementEntry\x1a)\n\x18SecurityRequirementValue\x12\r\n\x05scope\x18\x01 \x03(\t\x1a\x93\x01\n\x18SecurityRequirementEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12f\n\x05value\x18\x02 \x01(\x0b2W.grpc.gateway.protoc_gen_openapiv2.options.SecurityRequirement.SecurityRequirementValue:\x028\x01"\x83\x01\n\x06Scopes\x12K\n\x05scope\x18\x01 \x03(\x0b2<.grpc.gateway.protoc_gen_openapiv2.options.Scopes.ScopeEntry\x1a,\n\nScopeEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x028\x01*;\n\x06Scheme\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x08\n\x04HTTP\x10\x01\x12\t\n\x05HTTPS\x10\x02\x12\x06\n\x02WS\x10\x03\x12\x07\n\x03WSS\x10\x04BHZFgithub.com/grpc-ecosystem/grpc-gateway/v2/protoc-gen-openapiv2/optionsb\x06proto3')
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'protoc_gen_openapiv2.options.openapiv2_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'protoc_gen_openapiv2.options.openapiv2_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b'ZFgithub.com/grpc-ecosystem/grpc-gateway/v2/protoc-gen-openapiv2/options'
     _SWAGGER_RESPONSESENTRY._options = None
     _SWAGGER_RESPONSESENTRY._serialized_options = b'8\x01'
     _SWAGGER_EXTENSIONSENTRY._options = None
     _SWAGGER_EXTENSIONSENTRY._serialized_options = b'8\x01'
@@ -31,75 +32,75 @@
     _SECURITYDEFINITIONS_SECURITYENTRY._serialized_options = b'8\x01'
     _SECURITYSCHEME_EXTENSIONSENTRY._options = None
     _SECURITYSCHEME_EXTENSIONSENTRY._serialized_options = b'8\x01'
     _SECURITYREQUIREMENT_SECURITYREQUIREMENTENTRY._options = None
     _SECURITYREQUIREMENT_SECURITYREQUIREMENTENTRY._serialized_options = b'8\x01'
     _SCOPES_SCOPEENTRY._options = None
     _SCOPES_SCOPEENTRY._serialized_options = b'8\x01'
-    _SCHEME._serialized_start = 5781
-    _SCHEME._serialized_end = 5840
-    _SWAGGER._serialized_start = 122
-    _SWAGGER._serialized_end = 983
-    _SWAGGER_RESPONSESENTRY._serialized_start = 789
-    _SWAGGER_RESPONSESENTRY._serialized_end = 890
-    _SWAGGER_EXTENSIONSENTRY._serialized_start = 892
-    _SWAGGER_EXTENSIONSENTRY._serialized_end = 965
-    _OPERATION._serialized_start = 986
-    _OPERATION._serialized_end = 1728
-    _OPERATION_RESPONSESENTRY._serialized_start = 789
-    _OPERATION_RESPONSESENTRY._serialized_end = 890
-    _OPERATION_EXTENSIONSENTRY._serialized_start = 892
-    _OPERATION_EXTENSIONSENTRY._serialized_end = 965
-    _HEADER._serialized_start = 1731
-    _HEADER._serialized_end = 1902
-    _RESPONSE._serialized_start = 1905
-    _RESPONSE._serialized_end = 2483
-    _RESPONSE_HEADERSENTRY._serialized_start = 2262
-    _RESPONSE_HEADERSENTRY._serialized_end = 2359
-    _RESPONSE_EXAMPLESENTRY._serialized_start = 2361
-    _RESPONSE_EXAMPLESENTRY._serialized_end = 2408
-    _RESPONSE_EXTENSIONSENTRY._serialized_start = 892
-    _RESPONSE_EXTENSIONSENTRY._serialized_end = 965
-    _INFO._serialized_start = 2486
-    _INFO._serialized_end = 2869
-    _INFO_EXTENSIONSENTRY._serialized_start = 892
-    _INFO_EXTENSIONSENTRY._serialized_end = 965
-    _CONTACT._serialized_start = 2871
-    _CONTACT._serialized_end = 2922
-    _LICENSE._serialized_start = 2924
-    _LICENSE._serialized_end = 2960
-    _EXTERNALDOCUMENTATION._serialized_start = 2962
-    _EXTERNALDOCUMENTATION._serialized_end = 3019
-    _SCHEMA._serialized_start = 3022
-    _SCHEMA._serialized_end = 3260
-    _JSONSCHEMA._serialized_start = 3263
-    _JSONSCHEMA._serialized_end = 4155
-    _JSONSCHEMA_FIELDCONFIGURATION._serialized_start = 3911
-    _JSONSCHEMA_FIELDCONFIGURATION._serialized_end = 3956
-    _JSONSCHEMA_JSONSCHEMASIMPLETYPES._serialized_start = 3958
-    _JSONSCHEMA_JSONSCHEMASIMPLETYPES._serialized_end = 4077
-    _TAG._serialized_start = 4157
-    _TAG._serialized_end = 4278
-    _SECURITYDEFINITIONS._serialized_start = 4281
-    _SECURITYDEFINITIONS._serialized_end = 4506
-    _SECURITYDEFINITIONS_SECURITYENTRY._serialized_start = 4400
-    _SECURITYDEFINITIONS_SECURITYENTRY._serialized_end = 4506
-    _SECURITYSCHEME._serialized_start = 4509
-    _SECURITYSCHEME._serialized_end = 5309
-    _SECURITYSCHEME_EXTENSIONSENTRY._serialized_start = 892
-    _SECURITYSCHEME_EXTENSIONSENTRY._serialized_end = 965
-    _SECURITYSCHEME_TYPE._serialized_start = 5075
-    _SECURITYSCHEME_TYPE._serialized_end = 5150
-    _SECURITYSCHEME_IN._serialized_start = 5152
-    _SECURITYSCHEME_IN._serialized_end = 5201
-    _SECURITYSCHEME_FLOW._serialized_start = 5203
-    _SECURITYSCHEME_FLOW._serialized_end = 5309
-    _SECURITYREQUIREMENT._serialized_start = 5312
-    _SECURITYREQUIREMENT._serialized_end = 5645
-    _SECURITYREQUIREMENT_SECURITYREQUIREMENTVALUE._serialized_start = 5454
-    _SECURITYREQUIREMENT_SECURITYREQUIREMENTVALUE._serialized_end = 5495
-    _SECURITYREQUIREMENT_SECURITYREQUIREMENTENTRY._serialized_start = 5498
-    _SECURITYREQUIREMENT_SECURITYREQUIREMENTENTRY._serialized_end = 5645
-    _SCOPES._serialized_start = 5648
-    _SCOPES._serialized_end = 5779
-    _SCOPES_SCOPEENTRY._serialized_start = 5735
-    _SCOPES_SCOPEENTRY._serialized_end = 5779
+    _globals['_SCHEME']._serialized_start = 5781
+    _globals['_SCHEME']._serialized_end = 5840
+    _globals['_SWAGGER']._serialized_start = 122
+    _globals['_SWAGGER']._serialized_end = 983
+    _globals['_SWAGGER_RESPONSESENTRY']._serialized_start = 789
+    _globals['_SWAGGER_RESPONSESENTRY']._serialized_end = 890
+    _globals['_SWAGGER_EXTENSIONSENTRY']._serialized_start = 892
+    _globals['_SWAGGER_EXTENSIONSENTRY']._serialized_end = 965
+    _globals['_OPERATION']._serialized_start = 986
+    _globals['_OPERATION']._serialized_end = 1728
+    _globals['_OPERATION_RESPONSESENTRY']._serialized_start = 789
+    _globals['_OPERATION_RESPONSESENTRY']._serialized_end = 890
+    _globals['_OPERATION_EXTENSIONSENTRY']._serialized_start = 892
+    _globals['_OPERATION_EXTENSIONSENTRY']._serialized_end = 965
+    _globals['_HEADER']._serialized_start = 1731
+    _globals['_HEADER']._serialized_end = 1902
+    _globals['_RESPONSE']._serialized_start = 1905
+    _globals['_RESPONSE']._serialized_end = 2483
+    _globals['_RESPONSE_HEADERSENTRY']._serialized_start = 2262
+    _globals['_RESPONSE_HEADERSENTRY']._serialized_end = 2359
+    _globals['_RESPONSE_EXAMPLESENTRY']._serialized_start = 2361
+    _globals['_RESPONSE_EXAMPLESENTRY']._serialized_end = 2408
+    _globals['_RESPONSE_EXTENSIONSENTRY']._serialized_start = 892
+    _globals['_RESPONSE_EXTENSIONSENTRY']._serialized_end = 965
+    _globals['_INFO']._serialized_start = 2486
+    _globals['_INFO']._serialized_end = 2869
+    _globals['_INFO_EXTENSIONSENTRY']._serialized_start = 892
+    _globals['_INFO_EXTENSIONSENTRY']._serialized_end = 965
+    _globals['_CONTACT']._serialized_start = 2871
+    _globals['_CONTACT']._serialized_end = 2922
+    _globals['_LICENSE']._serialized_start = 2924
+    _globals['_LICENSE']._serialized_end = 2960
+    _globals['_EXTERNALDOCUMENTATION']._serialized_start = 2962
+    _globals['_EXTERNALDOCUMENTATION']._serialized_end = 3019
+    _globals['_SCHEMA']._serialized_start = 3022
+    _globals['_SCHEMA']._serialized_end = 3260
+    _globals['_JSONSCHEMA']._serialized_start = 3263
+    _globals['_JSONSCHEMA']._serialized_end = 4155
+    _globals['_JSONSCHEMA_FIELDCONFIGURATION']._serialized_start = 3911
+    _globals['_JSONSCHEMA_FIELDCONFIGURATION']._serialized_end = 3956
+    _globals['_JSONSCHEMA_JSONSCHEMASIMPLETYPES']._serialized_start = 3958
+    _globals['_JSONSCHEMA_JSONSCHEMASIMPLETYPES']._serialized_end = 4077
+    _globals['_TAG']._serialized_start = 4157
+    _globals['_TAG']._serialized_end = 4278
+    _globals['_SECURITYDEFINITIONS']._serialized_start = 4281
+    _globals['_SECURITYDEFINITIONS']._serialized_end = 4506
+    _globals['_SECURITYDEFINITIONS_SECURITYENTRY']._serialized_start = 4400
+    _globals['_SECURITYDEFINITIONS_SECURITYENTRY']._serialized_end = 4506
+    _globals['_SECURITYSCHEME']._serialized_start = 4509
+    _globals['_SECURITYSCHEME']._serialized_end = 5309
+    _globals['_SECURITYSCHEME_EXTENSIONSENTRY']._serialized_start = 892
+    _globals['_SECURITYSCHEME_EXTENSIONSENTRY']._serialized_end = 965
+    _globals['_SECURITYSCHEME_TYPE']._serialized_start = 5075
+    _globals['_SECURITYSCHEME_TYPE']._serialized_end = 5150
+    _globals['_SECURITYSCHEME_IN']._serialized_start = 5152
+    _globals['_SECURITYSCHEME_IN']._serialized_end = 5201
+    _globals['_SECURITYSCHEME_FLOW']._serialized_start = 5203
+    _globals['_SECURITYSCHEME_FLOW']._serialized_end = 5309
+    _globals['_SECURITYREQUIREMENT']._serialized_start = 5312
+    _globals['_SECURITYREQUIREMENT']._serialized_end = 5645
+    _globals['_SECURITYREQUIREMENT_SECURITYREQUIREMENTVALUE']._serialized_start = 5454
+    _globals['_SECURITYREQUIREMENT_SECURITYREQUIREMENTVALUE']._serialized_end = 5495
+    _globals['_SECURITYREQUIREMENT_SECURITYREQUIREMENTENTRY']._serialized_start = 5498
+    _globals['_SECURITYREQUIREMENT_SECURITYREQUIREMENTENTRY']._serialized_end = 5645
+    _globals['_SCOPES']._serialized_start = 5648
+    _globals['_SCOPES']._serialized_end = 5779
+    _globals['_SCOPES_SCOPEENTRY']._serialized_start = 5735
+    _globals['_SCOPES_SCOPEENTRY']._serialized_end = 5779
```

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/api_client/test_exabel_api_group.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/api_client/test_exabel_api_group.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/data_classes/test_data_set.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/data_classes/test_data_set.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/data_classes/test_derived_signal.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/data_classes/test_derived_signal.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/data_classes/test_entity_type.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/data_classes/test_entity_type.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/data_classes/test_folder.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/data_classes/test_folder.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/data_classes/test_folder_accessor.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/data_classes/test_folder_accessor.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/data_classes/test_folder_item.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/data_classes/test_folder_item.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/data_classes/test_group.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/data_classes/test_group.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/data_classes/test_prediction_model_run.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/data_classes/test_prediction_model_run.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/data_classes/test_relationship.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/data_classes/test_relationship.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/data_classes/test_relationship_type.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/data_classes/test_relationship_type.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/data_classes/test_request_error.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/data_classes/test_request_error.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/data_classes/test_signal.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/data_classes/test_signal.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/data_classes/test_tag.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/data_classes/test_tag.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/data_classes/test_time_series.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/data_classes/test_time_series.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/data_classes/test_user.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/data_classes/test_user.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/mock_entity_api.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/mock_entity_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/mock_relationship_api.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/mock_relationship_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/mock_resource_store.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/mock_resource_store.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/mock_signal_api.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/mock_signal_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/test_bulk_insert_import.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/test_bulk_insert_import.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/test_entity_api.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/test_entity_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/test_error_handler.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/test_error_handler.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/test_export_api.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/test_export_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/test_namespace_api.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/test_namespace_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/test_pageable_resource.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/test_pageable_resource.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/test_relationship_api.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/test_relationship_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/test_resource_creation_result.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/test_resource_creation_result.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/test_signal_api.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/test_signal_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/api/test_time_series_api.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/api/test_time_series_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/exabel_mock_client.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/exabel_mock_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/query/test_query.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/query/test_query.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/test_client_config.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/test_client_config.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/test_exabel_client.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/test_exabel_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/client/test_user_login.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/client/test_user_login.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/decorators.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/decorators.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/scripts/common_utils.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/scripts/common_utils.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/scripts/sql/test_read_snowflake.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/scripts/sql/test_read_snowflake.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/scripts/sql/test_sql_script.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/scripts/sql/test_sql_script.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/scripts/test_actions.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/scripts/test_actions.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/scripts/test_command_line_script.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/scripts/test_command_line_script.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/scripts/test_create_entity_mapping_from_csv.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/scripts/test_create_entity_mapping_from_csv.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/scripts/test_create_entity_type.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/scripts/test_create_entity_type.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/scripts/test_create_relationship_type.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/scripts/test_create_relationship_type.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/scripts/test_delete_entity_type.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/scripts/test_delete_entity_type.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/scripts/test_export_data.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/scripts/test_export_data.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/scripts/test_load_entities_from_csv.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/scripts/test_load_entities_from_csv.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/scripts/test_load_relationships_from_csv.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/scripts/test_load_relationships_from_csv.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/scripts/test_load_scripts.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/scripts/test_load_scripts.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/scripts/test_load_time_series_from_csv.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/scripts/test_load_time_series_from_csv.py`

 * *Files 3% similar despite different names*

```diff
@@ -507,56 +507,109 @@
             "--no-create-tag",
         ]
         script = LoadTimeSeriesFromFile(args)
         script.run_script(self.client, script.parse_arguments())
 
         call_args_list = self.client.time_series_api.bulk_upsert_time_series.call_args_list
         create_tag_status = call_args_list[0][1]["create_tag"]
-        self.assertEqual(False, create_tag_status)
+        self.assertFalse(create_tag_status)
 
     def test_valid_create_tag(self):
         args = common_args + [
             "--filename",
             "./exabel_data_sdk/tests/resources/data/timeseries_known_time.csv",
         ]
         script = LoadTimeSeriesFromFile(args)
         script.run_script(self.client, script.parse_arguments())
 
         call_args_list = self.client.time_series_api.bulk_upsert_time_series.call_args_list
         create_tag_status = call_args_list[0][1]["create_tag"]
-        self.assertEqual(True, create_tag_status)
+        self.assertTrue(create_tag_status)
 
     def test_valid_no_create_library_signal(self):
         args = common_args + [
             "--filename",
             "./exabel_data_sdk/tests/resources/data/timeseries_known_time.csv",
             "--create-missing-signals",
             "--no-create-library-signal",
         ]
         script = LoadTimeSeriesFromFile(args)
         self.client.namespace = "acme"
         script.run_script(self.client, script.parse_arguments())
 
         call_args_list = self.client.signal_api.create_signal.call_args_list
         create_library_signal_status = call_args_list[0][1]["create_library_signal"]
-        self.assertEqual(False, create_library_signal_status)
+        self.assertFalse(create_library_signal_status)
 
     def test_valid_create_library_signal(self):
         args = common_args + [
             "--filename",
             "./exabel_data_sdk/tests/resources/data/timeseries_known_time.csv",
             "--create-missing-signals",
         ]
         script = LoadTimeSeriesFromFile(args)
         self.client.namespace = "acme"
         script.run_script(self.client, script.parse_arguments())
 
         call_args_list = self.client.signal_api.create_signal.call_args_list
         create_library_signal_status = call_args_list[0][1]["create_library_signal"]
-        self.assertEqual(True, create_library_signal_status)
+        self.assertTrue(create_library_signal_status)
+
+    def test_valid_replace_existing_time_series(self):
+        args = common_args + [
+            "--filename",
+            "./exabel_data_sdk/tests/resources/data/timeseries_known_time.csv",
+            "--create-missing-signals",
+            "--replace-existing-time-series",
+        ]
+        script = LoadTimeSeriesFromFile(args)
+        self.client.namespace = "acme"
+        script.run_script(self.client, script.parse_arguments())
+
+        call_args_list = self.client.time_series_api.bulk_upsert_time_series.call_args_list
+        replace_existing_tine_series_status = call_args_list[0][1]["replace_existing_time_series"]
+        self.assertTrue(replace_existing_tine_series_status)
+
+    def test_replace_existing_time_series_accross_batches(self):
+        args = common_args + [
+            "--filename",
+            "./exabel_data_sdk/tests/resources/data/timeseries.csv",
+            "--create-missing-signals",
+            "--pit-offset",
+            "0",
+            "--replace-existing-time-series",
+            "--batch-size",
+            "3",
+        ]
+        script = LoadTimeSeriesFromFile(args)
+        self.client.namespace = "acme"
+        script.run_script(self.client, script.parse_arguments())
+
+        call_args_list = self.client.time_series_api.bulk_upsert_time_series.call_args_list
+        self.assertEqual(4, len(call_args_list))
+        self.assertTrue(call_args_list[0][1]["replace_existing_time_series"])
+        self.assertEqual(
+            "entityTypes/company/entities/company_A/signals/acme.signal1",
+            call_args_list[0][0][0][0].name,
+        )
+        self.assertFalse("replace_existing_time_series" in call_args_list[1][1])
+        self.assertEqual(
+            "entityTypes/company/entities/company_A/signals/acme.signal1",
+            call_args_list[1][0][0][0].name,
+        )
+        self.assertTrue(call_args_list[2][1]["replace_existing_time_series"])
+        self.assertEqual(
+            "entityTypes/company/entities/company_B/signals/acme.signal1",
+            call_args_list[2][0][0][0].name,
+        )
+        self.assertFalse("replace_existing_time_series" in call_args_list[3][1])
+        self.assertEqual(
+            "entityTypes/company/entities/company_B/signals/acme.signal1",
+            call_args_list[3][0][0][0].name,
+        )
 
     @property
     def _partial_load_time_series(self) -> Callable:
         parse_file_result = pd.DataFrame(
             data={
                 "entity": ["entity1", "entity1", "entity2"],
                 "date": ["2022-01-01", "2022-01-01", "2022-01-01"],
```

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/scripts/test_load_time_series_from_excel.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/scripts/test_load_time_series_from_excel.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/scripts/test_update_entity_type.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/scripts/test_update_entity_type.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/scripts/test_update_relationship_type.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/scripts/test_update_relationship_type.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/services/sql/test_athena_reader_configuration.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/services/sql/test_athena_reader_configuration.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/services/sql/test_bigquery_reader_configuration.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/services/sql/test_bigquery_reader_configuration.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/services/sql/test_snowflake_reader_configuration.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/services/sql/test_snowflake_reader_configuration.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/services/sql/test_sql_reader.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/services/sql/test_sql_reader.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/services/sql/test_sql_reader_configuration.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/services/sql/test_sql_reader_configuration.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/services/test_csv_entity_loader.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/services/test_csv_entity_loader.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/services/test_csv_reader.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/services/test_csv_reader.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/services/test_csv_relationship_loader.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/services/test_csv_relationship_loader.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/services/test_csv_time_series_loader.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/services/test_csv_time_series_loader.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/services/test_csv_writer.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/services/test_csv_writer.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/services/test_entity_mapping_file_reader.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/services/test_entity_mapping_file_reader.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/services/test_excel_writer.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/services/test_excel_writer.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/services/test_file_loading_result.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/services/test_file_loading_result.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/services/test_file_time_series_loader.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/services/test_file_time_series_loader.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/services/test_file_time_series_parser.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/services/test_file_time_series_parser.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/services/test_file_writer_provider.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/services/test_file_writer_provider.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/test_decorators.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/util/test_batcher.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/util/test_batcher.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/util/test_deprecate_arguments.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/util/test_deprecate_arguments.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/util/test_handle_missing_imports.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/util/test_handle_missing_imports.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/util/test_parse_property_columns.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/util/test_parse_property_columns.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/util/test_resource_name_normalization.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/util/test_resource_name_normalization.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/tests/util/test_type_converter.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/tests/util/test_type_converter.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/util/case_insensitive_column.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/util/case_insensitive_column.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/util/deprecate_arguments.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/util/deprecate_arguments.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/util/handle_missing_imports.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/util/handle_missing_imports.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/util/import_.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/util/import_.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/util/parse_property_columns.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/util/parse_property_columns.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/util/resource_name_normalization.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/util/resource_name_normalization.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk/util/type_converter.py` & `exabel-data-sdk-4.5.0/exabel_data_sdk/util/type_converter.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk.egg-info/PKG-INFO` & `exabel-data-sdk-4.5.0/exabel_data_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exabel-data-sdk
-Version: 4.4.0
+Version: 4.5.0
 Summary: Python SDK for the Exabel Data API
 Home-page: https://github.com/Exabel/python-sdk
 Author: Exabel
 Author-email: support@exabel.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Financial and Insurance Industry
```

### Comparing `exabel-data-sdk-4.4.0/exabel_data_sdk.egg-info/SOURCES.txt` & `exabel-data-sdk-4.5.0/exabel_data_sdk.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -316,14 +316,15 @@
 exabel_data_sdk/tests/scripts/__init__.py
 exabel_data_sdk/tests/scripts/common_utils.py
 exabel_data_sdk/tests/scripts/test_actions.py
 exabel_data_sdk/tests/scripts/test_command_line_script.py
 exabel_data_sdk/tests/scripts/test_create_entity_mapping_from_csv.py
 exabel_data_sdk/tests/scripts/test_create_entity_type.py
 exabel_data_sdk/tests/scripts/test_create_relationship_type.py
+exabel_data_sdk/tests/scripts/test_csv_script.py
 exabel_data_sdk/tests/scripts/test_delete_entity_type.py
 exabel_data_sdk/tests/scripts/test_export_data.py
 exabel_data_sdk/tests/scripts/test_load_entities_from_csv.py
 exabel_data_sdk/tests/scripts/test_load_relationships_from_csv.py
 exabel_data_sdk/tests/scripts/test_load_scripts.py
 exabel_data_sdk/tests/scripts/test_load_time_series_from_csv.py
 exabel_data_sdk/tests/scripts/test_load_time_series_from_excel.py
```

### Comparing `exabel-data-sdk-4.4.0/pyproject.toml` & `exabel-data-sdk-4.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.4.0/setup.py` & `exabel-data-sdk-4.5.0/setup.py`

 * *Files identical despite different names*

