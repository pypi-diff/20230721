# Comparing `tmp/rime_sdk-2.2.0rc2.tar.gz` & `tmp/rime_sdk-2.2.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rime_sdk-2.2.0rc2.tar", last modified: Wed Jul 12 00:30:35 2023, max compression
+gzip compressed data, was "rime_sdk-2.2.0rc3.tar", last modified: Thu Jul 20 04:41:45 2023, max compression
```

## Comparing `rime_sdk-2.2.0rc2.tar` & `rime_sdk-2.2.0rc3.tar`

### file list

```diff
@@ -1,502 +1,497 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:30:35.438487 rime_sdk-2.2.0rc2/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-12 00:29:56.000000 rime_sdk-2.2.0rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-12 00:30:35.438487 rime_sdk-2.2.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-12 00:29:56.000000 rime_sdk-2.2.0rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:30:35.386488 rime_sdk-2.2.0rc2/rime_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-12 00:29:56.000000 rime_sdk-2.2.0rc2/rime_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63997 2023-07-12 00:29:56.000000 rime_sdk-2.2.0rc2/rime_sdk/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12282 2023-07-12 00:29:56.000000 rime_sdk-2.2.0rc2/rime_sdk/data_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:30:35.386488 rime_sdk-2.2.0rc2/rime_sdk/data_format_check/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 00:29:56.000000 rime_sdk-2.2.0rc2/rime_sdk/data_format_check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-07-12 00:29:56.000000 rime_sdk-2.2.0rc2/rime_sdk/data_format_check/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-12 00:29:56.000000 rime_sdk-2.2.0rc2/rime_sdk/data_format_check/data_format_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     8642 2023-07-12 00:29:56.000000 rime_sdk-2.2.0rc2/rime_sdk/data_format_check/nlp_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-07-12 00:29:56.000000 rime_sdk-2.2.0rc2/rime_sdk/data_format_check/tabular_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-12 00:29:56.000000 rime_sdk-2.2.0rc2/rime_sdk/detection_event.py
--rw-r--r--   0 runner    (1001) docker     (123)    24664 2023-07-12 00:29:56.000000 rime_sdk-2.2.0rc2/rime_sdk/firewall.py
--rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-07-12 00:29:56.000000 rime_sdk-2.2.0rc2/rime_sdk/image_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:30:35.390488 rime_sdk-2.2.0rc2/rime_sdk/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 00:29:56.000000 rime_sdk-2.2.0rc2/rime_sdk/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15159 2023-07-12 00:29:56.000000 rime_sdk-2.2.0rc2/rime_sdk/internal/config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-12 00:29:56.000000 rime_sdk-2.2.0rc2/rime_sdk/internal/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-12 00:29:56.000000 rime_sdk-2.2.0rc2/rime_sdk/internal/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     9405 2023-07-12 00:29:56.000000 rime_sdk-2.2.0rc2/rime_sdk/internal/file_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-12 00:29:56.000000 rime_sdk-2.2.0rc2/rime_sdk/internal/rest_error_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-12 00:29:56.000000 rime_sdk-2.2.0rc2/rime_sdk/internal/security_config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9119 2023-07-12 00:29:56.000000 rime_sdk-2.2.0rc2/rime_sdk/internal/swagger_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-07-12 00:29:56.000000 rime_sdk-2.2.0rc2/rime_sdk/internal/swagger_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-12 00:29:56.000000 rime_sdk-2.2.0rc2/rime_sdk/internal/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-07-12 00:29:56.000000 rime_sdk-2.2.0rc2/rime_sdk/internal/throttle_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-07-12 00:29:56.000000 rime_sdk-2.2.0rc2/rime_sdk/internal/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18123 2023-07-12 00:29:56.000000 rime_sdk-2.2.0rc2/rime_sdk/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-07-12 00:29:56.000000 rime_sdk-2.2.0rc2/rime_sdk/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    71842 2023-07-12 00:29:56.000000 rime_sdk-2.2.0rc2/rime_sdk/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    27058 2023-07-12 00:29:56.000000 rime_sdk-2.2.0rc2/rime_sdk/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:30:35.390488 rime_sdk-2.2.0rc2/rime_sdk/swagger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 00:30:30.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:30:35.390488 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/
--rw-r--r--   0 runner    (1001) docker     (123)    48376 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:30:35.394487 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/api/
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35443 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/api/agent_manager_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/api/config_validator_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18019 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/api/customer_managed_key_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25195 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/api/data_collector_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11208 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/api/detection_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    22891 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/api/feature_flag_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8998 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/api/file_scanning_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18110 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/api/file_upload_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    22460 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/api/firewall_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    28286 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/api/image_registry_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26888 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/api/integration_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26961 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/api/job_reader_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    21630 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/api/model_card_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19271 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/api/model_testing_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29459 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/api/monitor_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19744 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/api/notification_setting_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    55813 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/api/project_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    57319 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/api/registry_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    72408 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/api/results_reader_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/api/rime_info_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    40185 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/api/user_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25498 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/api/validation_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    46002 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/api/workspace_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25179 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8286 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:30:35.438487 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/
--rw-r--r--   0 runner    (1001) docker     (123)    46235 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/configvalidator_config_type_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/continuoustests_firewall_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/create_agent_request_azure_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     8011 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/customermanagedkey_customer_managed_key_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/data_params_feature_intersection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/data_params_ranking_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    13500 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/data_profiling_column_type_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/data_profiling_feature_relationship_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/datacollector_datapoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/datacollector_datapoint_row.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/dataset_ct_dataset_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/dataset_ct_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    11792 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/dataset_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     8421 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/dataset_id_prediction_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/datastream_project_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    16260 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/detection_detection_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/detection_event_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/detection_event_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/detection_metric_degradation_event_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/detection_resolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     7745 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/detection_security_event_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/difference_from_target_difference.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/difference_from_target_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/digest_config_digest_frequency.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/featureflags_customer_name_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/filescanning_file_scan_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/filescanning_huggingface_model_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/filescanning_model_file_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/filescanning_pytorch_model_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/filescanning_security_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/filescanning_security_report_import_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     9982 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/firewall_firewall.py
--rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    11064 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5158 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/generativestresstests_project_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/googlerpc_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/heartbeat_agent_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/integration_integration_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/integration_integration_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/integration_integration_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/integrations_integration_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/job_data_continuous_incremental_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/job_data_stress_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/list_agents_request_list_agents_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/list_datasets_request_datasets_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/list_images_request_pip_library_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_aggregated_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metric_without_subsets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/list_models_request_model_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/list_monitors_request_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/list_notifications_request_list_notifications_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/list_prediction_sets_request_prediction_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/list_summary_tests_request_list_summary_tests_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/list_test_cases_request_list_test_cases_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/managed_image_package_requirement.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/managed_image_package_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/managed_image_pip_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/managed_image_pip_requirement.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/managed_image_role_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    10561 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/model_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/modelcards_model_card_model_card_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/monitor_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/monitor_aggregation_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/monitor_anomaly_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/monitor_artifact_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/monitor_difference_from_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/monitor_excluded_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/monitor_metric_degradation_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/monitor_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/monitor_monitor_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/monitor_threshold.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/monitor_threshold_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/monitor_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/monitoring_config_alert_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/monitors_monitor_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/notification_digest_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/notification_job_action_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/notification_monitoring_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9399 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/notification_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/notification_notification_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/notification_object_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/notification_webhook_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/notifsettings_notification_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/predictions_model_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/project_add_users_to_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11026 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/project_create_project_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/project_create_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/project_delete_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/project_get_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/project_get_project_url_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/project_get_workspace_roles_for_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/project_id_uuid_dataset_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/project_id_uuid_model_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/project_list_projects_request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/project_list_projects_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/project_list_users_of_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/project_owner_details.py
--rw-r--r--   0 runner    (1001) docker     (123)    17754 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/project_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/project_project_with_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/project_remove_user_from_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/project_update_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/project_update_user_of_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/project_update_workspace_roles_for_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/projects_project_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/protobuf_any.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/protobuf_null_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rca_feature_cause.py
--rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rca_rca_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rca_rca_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rca_test_case_cause.py
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rca_test_case_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/registry_connection_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/registry_data_collector_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/registry_data_file_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/registry_data_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/registry_data_loading_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    20573 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/registry_data_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/registry_data_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/registry_databricks_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/registry_hugging_face_data_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/registry_hugging_face_model_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/registry_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/registry_model_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/registry_model_path_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/registry_pred_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/registry_prediction_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/registry_validity_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    11606 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/registryprediction_prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_actor_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7904 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_agent_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_api_token_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_category_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    13366 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_category_test_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_config_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_configure_integration_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_continuous_test_run_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_agent_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_agent_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_api_token_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_api_token_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_image_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_image_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_model_card_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_model_card_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7142 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_notification_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_notification_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_user_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_user_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7061 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_workspace_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_deactivate_agent_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_delete_agent_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_delete_custom_monitor_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_delete_dataset_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_delete_firewall_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_delete_image_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_delete_integration_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_delete_model_card_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_delete_model_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_delete_prediction_set_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_delete_uploaded_file_url_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_failing_row.py
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     9233 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_feature_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_feature_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_float_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_customer_managed_key_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_feature_flag_jwt_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_feature_flags_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_firewall_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_image_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_integration_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_job_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_key_status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_latest_logs_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_limit_status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_model_card_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_model_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_monitor_result_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_prediction_set_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_predictions_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_project_id_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     8541 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_rime_info_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_test_run_id_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_url_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_user_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_validate_dataset_task_status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_validate_model_task_status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_validate_predictions_task_status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_heartbeat_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_image_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_int_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_integration_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_job_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    14784 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_job_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_job_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_job_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_language.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_license_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_license_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_limit_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_limit_status_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_agents_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_api_tokens_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_datasets_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    10179 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_enabled_features_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_file_scan_results_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_images_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_images_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_models_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_monitors_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_notifications_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_prediction_sets_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_project_tags_in_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_uploaded_file_urls_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_users_of_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_users_request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_users_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_workspace_integrations_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_long_description_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)    13132 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_managed_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_managed_image_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_model_card.py
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_model_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_model_with_owner_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_monitor_data_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_named_double.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_parent_role_subject_role_pair.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_register_data_stream_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_register_dataset_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_register_external_agent_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_register_internal_agent_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_register_model_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_register_prediction_set_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_remove_user_from_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_reset_password_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_resolve_detection_event_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_ri_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_safe_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_severity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_severity_counts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_sort_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_start_generative_stress_test_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_str_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_subject_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_suggestion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_sync_image_tag_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_table_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_table_column_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_test_case_monitor_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_test_case_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     9660 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_test_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py
--rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_test_task_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_test_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_time_interval.py
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_token_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_update_build_info_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_update_build_info_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_update_firewall_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_update_integration_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_update_model_card_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_update_monitor_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_update_notification_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_update_user_of_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_update_user_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_update_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_upsert_feature_flags_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_user_detail_with_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_user_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_user_with_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_user_write_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_validate_test_config_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7431 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_workspace_write_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rischemaintegration_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/riskscore_risk_category_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/riskscore_risk_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/role_users_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/role_workspace_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/schemamonitor_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/schemanotification_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/statedb_archived_job_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/statedb_job_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10280 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py
--rw-r--r--   0 runner    (1001) docker     (123)    10652 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrun_generative_test_run_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12809 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrun_ref_eval_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     8617 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     6759 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrun_test_suite_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_config_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_run_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_list_batch_results_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_list_feature_results_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_list_monitor_categories_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_list_summary_tests_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_cases_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_list_validation_categories_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_rename_test_run_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_result_summary_counts.py
--rw-r--r--   0 runner    (1001) docker     (123)    16684 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result_display.py
--rw-r--r--   0 runner    (1001) docker     (123)    13296 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_test_case_display.py
--rw-r--r--   0 runner    (1001) docker     (123)    13655 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result_display.py
--rw-r--r--   0 runner    (1001) docker     (123)    15198 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/user_favorite_projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/user_private_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/user_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     7844 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/user_user_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/users_user_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py
--rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py
--rw-r--r--   0 runner    (1001) docker     (123)    14608 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/v1betamonitorsmonitor_id_uuid_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11044 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py
--rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/v1notifsettingsnotification_id_uuid_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/v1projectsproject_id_uuidroleusersuser_user_id_uuid_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     8198 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/validation_validate_dataset_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/validation_validate_model_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/validation_validate_predictions_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    13063 2023-07-12 00:30:31.000000 rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-07-12 00:29:56.000000 rime_sdk-2.2.0rc2/rime_sdk/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)    14859 2023-07-12 00:29:56.000000 rime_sdk-2.2.0rc2/rime_sdk/test_run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:30:35.386488 rime_sdk-2.2.0rc2/rime_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-12 00:30:35.000000 rime_sdk-2.2.0rc2/rime_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    33350 2023-07-12 00:30:35.000000 rime_sdk-2.2.0rc2/rime_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 00:30:35.000000 rime_sdk-2.2.0rc2/rime_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-12 00:30:35.000000 rime_sdk-2.2.0rc2/rime_sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-12 00:30:35.000000 rime_sdk-2.2.0rc2/rime_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 00:30:35.000000 rime_sdk-2.2.0rc2/rime_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 00:30:35.438487 rime_sdk-2.2.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-12 00:29:56.000000 rime_sdk-2.2.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:41:45.720434 rime_sdk-2.2.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-20 04:41:45.720434 rime_sdk-2.2.0rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:41:45.676434 rime_sdk-2.2.0rc3/rime_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/rime_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63997 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/rime_sdk/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12282 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/rime_sdk/data_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:41:45.676434 rime_sdk-2.2.0rc3/rime_sdk/data_format_check/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/rime_sdk/data_format_check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/rime_sdk/data_format_check/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/rime_sdk/data_format_check/data_format_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8642 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/rime_sdk/data_format_check/nlp_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/rime_sdk/data_format_check/tabular_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/rime_sdk/detection_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26099 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/rime_sdk/firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/rime_sdk/image_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:41:45.676434 rime_sdk-2.2.0rc3/rime_sdk/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/rime_sdk/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15159 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/rime_sdk/internal/config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/rime_sdk/internal/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/rime_sdk/internal/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9405 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/rime_sdk/internal/file_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/rime_sdk/internal/rest_error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/rime_sdk/internal/security_config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9011 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/rime_sdk/internal/swagger_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/rime_sdk/internal/swagger_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/rime_sdk/internal/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/rime_sdk/internal/throttle_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/rime_sdk/internal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18064 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/rime_sdk/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/rime_sdk/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73004 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/rime_sdk/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27443 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/rime_sdk/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:41:45.676434 rime_sdk-2.2.0rc3/rime_sdk/swagger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:41:45.676434 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/
+-rw-r--r--   0 runner    (1001) docker     (123)    47967 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:41:45.680434 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35443 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/agent_manager_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/config_validator_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18019 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/customer_managed_key_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25195 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/data_collector_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11208 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/detection_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22891 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/feature_flag_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8998 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/file_scanning_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18110 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/file_upload_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22460 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/firewall_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28286 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/image_registry_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26888 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/integration_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26961 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/job_reader_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21630 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/model_card_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19271 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/model_testing_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29459 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/monitor_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19744 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/notification_setting_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55813 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/project_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57319 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/registry_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72408 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/results_reader_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/rime_info_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40185 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25498 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/validation_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46002 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/workspace_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25179 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8286 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:41:45.720434 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    45826 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/configvalidator_config_type_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/continuoustests_firewall_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/create_agent_request_azure_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8011 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/customermanagedkey_customer_managed_key_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/data_params_feature_intersection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/data_params_ranking_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13500 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/data_profiling_column_type_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/data_profiling_feature_relationship_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/datacollector_datapoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/datacollector_datapoint_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/dataset_ct_dataset_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/dataset_ct_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11792 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/dataset_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8421 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/dataset_id_prediction_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/datastream_project_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15539 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/detection_detection_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/detection_event_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/detection_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/detection_metric_degradation_event_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/detection_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7745 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/detection_security_event_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/difference_from_target_difference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/difference_from_target_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/digest_config_digest_frequency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/featureflags_customer_name_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/filescanning_file_scan_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/filescanning_huggingface_model_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/filescanning_model_file_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/filescanning_pytorch_model_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/filescanning_security_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/filescanning_security_report_import_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9982 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/firewall_firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11064 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5158 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/generativestresstests_project_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/googlerpc_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/heartbeat_agent_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/integration_integration_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/integration_integration_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/integration_integration_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/integrations_integration_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/job_data_continuous_incremental_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/job_data_stress_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/list_agents_request_list_agents_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/list_datasets_request_datasets_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/list_images_request_pip_library_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_aggregated_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metric_without_subsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/list_models_request_model_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/list_monitors_request_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/list_notifications_request_list_notifications_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/list_prediction_sets_request_prediction_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/list_summary_tests_request_list_summary_tests_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/list_test_cases_request_list_test_cases_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/managed_image_package_requirement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/managed_image_package_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/managed_image_pip_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/managed_image_pip_requirement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/managed_image_role_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11642 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/model_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/modelcards_model_card_model_card_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/monitor_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/monitor_aggregation_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/monitor_anomaly_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/monitor_artifact_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/monitor_difference_from_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/monitor_excluded_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/monitor_metric_degradation_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12705 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/monitor_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/monitor_monitor_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/monitor_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/monitor_threshold_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/monitor_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/monitoring_config_alert_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/monitors_monitor_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/notification_digest_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/notification_job_action_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/notification_monitoring_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9399 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/notification_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/notification_notification_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/notification_object_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/notification_webhook_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/notifsettings_notification_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/predictions_model_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_add_users_to_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11026 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_create_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_create_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_delete_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_get_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_get_project_url_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_get_workspace_roles_for_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_id_uuid_dataset_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10410 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_id_uuid_model_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_list_projects_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_list_projects_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_list_users_of_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_owner_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17754 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_project_with_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_remove_user_from_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_update_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_update_user_of_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_update_workspace_roles_for_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/projects_project_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/protobuf_any.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/protobuf_null_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_connection_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_data_collector_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_data_file_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_data_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_data_loading_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20609 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_data_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_databricks_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_hugging_face_data_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_hugging_face_model_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_model_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_model_path_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_pred_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_prediction_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_validity_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11606 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registryprediction_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_actor_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7904 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_agent_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_api_token_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_category_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13366 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_category_test_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_config_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_configure_integration_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_continuous_test_run_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_agent_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_agent_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5639 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_api_token_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_api_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_image_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_image_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_model_card_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_model_card_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7230 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_notification_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_notification_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_user_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7061 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_workspace_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_deactivate_agent_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_agent_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_custom_monitor_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_dataset_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_firewall_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_image_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_integration_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_model_card_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_prediction_set_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_uploaded_file_url_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_failing_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9233 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_feature_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_feature_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_float_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_customer_managed_key_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_feature_flag_jwt_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_feature_flags_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_firewall_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_image_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_integration_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_job_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_key_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_latest_logs_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_limit_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_model_card_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_monitor_result_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_prediction_set_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_predictions_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_project_id_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8541 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_rime_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_test_run_id_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_url_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_user_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_validate_dataset_task_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_validate_model_task_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_validate_predictions_task_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_heartbeat_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_image_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_int_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_integration_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_job_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14784 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_job_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_job_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_job_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_language.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_license_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_license_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_limit_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_limit_status_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_agents_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_api_tokens_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_datasets_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10179 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_enabled_features_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_file_scan_results_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_images_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_images_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_models_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_monitors_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_notifications_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_prediction_sets_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_project_tags_in_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_uploaded_file_urls_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_users_of_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_users_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_users_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_workspace_integrations_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_long_description_tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13132 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_managed_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_managed_image_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_model_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_model_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_model_with_owner_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_monitor_data_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_named_double.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_parent_role_subject_role_pair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_register_data_stream_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_register_dataset_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_register_external_agent_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_register_internal_agent_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_register_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_register_prediction_set_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_remove_user_from_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_reset_password_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_resolve_detection_event_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_ri_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_safe_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_severity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_severity_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_sort_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_generative_stress_test_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_str_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_subject_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_suggestion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_sync_image_tag_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_table_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_table_column_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_test_case_monitor_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_test_case_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9660 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_test_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_test_task_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_test_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_time_interval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_token_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_build_info_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_build_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_firewall_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_integration_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_model_card_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_monitor_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_notification_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_user_of_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_user_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_upsert_feature_flags_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_user_detail_with_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_user_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_user_with_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_user_write_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_validate_test_config_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7431 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_workspace_write_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rischemaintegration_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/riskscore_risk_category_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/riskscore_risk_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/role_users_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/role_workspace_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/schemamonitor_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/schemanotification_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/statedb_archived_job_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/statedb_job_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10280 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10652 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrun_generative_test_run_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12809 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrun_ref_eval_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8617 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6759 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrun_test_suite_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_config_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_run_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_list_batch_results_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_list_feature_results_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_list_monitor_categories_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_list_summary_tests_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_cases_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_list_validation_categories_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_rename_test_run_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_result_summary_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16800 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13296 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_case_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13655 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16128 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/user_favorite_projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/user_private_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/user_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7844 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/user_user_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/users_user_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13843 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/v1betamonitorsmonitor_id_uuid_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11044 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/v1notifsettingsnotification_id_uuid_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/v1projectsproject_id_uuidroleusersuser_user_id_uuid_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8198 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/validation_validate_dataset_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/validation_validate_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/validation_validate_predictions_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13063 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/rime_sdk/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14859 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/rime_sdk/test_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:41:45.676434 rime_sdk-2.2.0rc3/rime_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-20 04:41:45.000000 rime_sdk-2.2.0rc3/rime_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    33057 2023-07-20 04:41:45.000000 rime_sdk-2.2.0rc3/rime_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 04:41:45.000000 rime_sdk-2.2.0rc3/rime_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-20 04:41:45.000000 rime_sdk-2.2.0rc3/rime_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-20 04:41:45.000000 rime_sdk-2.2.0rc3/rime_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-20 04:41:45.000000 rime_sdk-2.2.0rc3/rime_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 04:41:45.720434 rime_sdk-2.2.0rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/setup.py
```

### Comparing `rime_sdk-2.2.0rc2/LICENSE` & `rime_sdk-2.2.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/PKG-INFO` & `rime_sdk-2.2.0rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rime_sdk
-Version: 2.2.0rc2
+Version: 2.2.0rc3
 Summary: Package to programmatically access a RIME deployment
 Home-page: UNKNOWN
 License: OSI Approved :: Apache Software License
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `rime_sdk-2.2.0rc2/README.md` & `rime_sdk-2.2.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/__init__.py` & `rime_sdk-2.2.0rc3/rime_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/client.py` & `rime_sdk-2.2.0rc3/rime_sdk/client.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/data_collector.py` & `rime_sdk-2.2.0rc3/rime_sdk/data_collector.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/data_format_check/cli.py` & `rime_sdk-2.2.0rc3/rime_sdk/data_format_check/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -93,22 +93,22 @@
             checker.check(
                 argps.ref_path,
                 argps.eval_path,
                 argps.task,
                 preds_ref_path=argps.preds_ref_path,
                 preds_eval_path=argps.preds_eval_path,
             )
-        except Exception as e:  # pylint: disable=broad-except
+        except Exception as e:
             pprint_exception(e)
     elif argps.tabular:
         checker = TabularDataFormatChecker()
         try:
             checker.check(
                 argps.ref_path,
                 argps.eval_path,
                 argps.task,
                 label_col_name=argps.label_col_name,
                 pred_col_name=argps.pred_col_name,
                 timestamp_col_name=argps.timestamp_col_name,
             )
-        except Exception as e:  # pylint: disable=broad-except
+        except Exception as e:
             pprint_exception(e)
```

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/data_format_check/data_format_checker.py` & `rime_sdk-2.2.0rc3/rime_sdk/data_format_check/data_format_checker.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/data_format_check/nlp_checker.py` & `rime_sdk-2.2.0rc3/rime_sdk/data_format_check/nlp_checker.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/data_format_check/tabular_checker.py` & `rime_sdk-2.2.0rc3/rime_sdk/data_format_check/tabular_checker.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/detection_event.py` & `rime_sdk-2.2.0rc3/rime_sdk/detection_event.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/firewall.py` & `rime_sdk-2.2.0rc3/rime_sdk/firewall.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Library defining the interface to firewall."""
 from datetime import timedelta
 from typing import Any, Dict, Iterator, List, Optional
 
 import pandas as pd
+from deprecated import deprecated
 
 from rime_sdk.internal.config_parser import (
     convert_single_data_info_to_swagger,
     convert_single_pred_info_to_swagger,
 )
 from rime_sdk.internal.constants import (
     MONITOR_TYPE_TO_SWAGGER,
@@ -38,21 +39,21 @@
 )
 from rime_sdk.swagger.swagger_client.api.detection_api import DetectionApi
 from rime_sdk.swagger.swagger_client.models import RimeJobMetadata
 from rime_sdk.swagger.swagger_client.models.detection_event_type import (
     DetectionEventType,
 )
 
-# 30 days in seconds
-# 1 day = 86400 seconds
-LIST_TEST_RUNS_INTERVAL_LENGTH_SECONDS = 30 * 86400
-
 
+@deprecated("Firewall class will not be supported from Robust Intelligence v2.4.")
 class Firewall:
-    """An interface to a RIME Firewall."""
+    """An interface to a RIME Firewall.
+
+    This class is deprecated in Robust Intelligence v2.2 and will be removed in v2.4.
+    """
 
     # A throttler that limits the number of model tests to roughly 20 every 5 minutes.
     # This is a static variable for Client.
     _throttler = ThrottleQueue(desired_events_per_epoch=20, epoch_duration_sec=300)
 
     def __init__(self, api_client: ApiClient, firewall_id: str) -> None:
         """Create a new Firewall object.
@@ -70,14 +71,17 @@
         """Check if this FWInstance is equivalent to 'obj'."""
         return isinstance(obj, Firewall) and self._firewall_id == obj._firewall_id
 
     def __repr__(self) -> str:
         """Return string representation of the object."""
         return f"Firewall({self._firewall_id})"
 
+    @deprecated(
+        "Firewall class methods will not be supported from Robust Intelligence v2.4."
+    )
     def update_firewall(
         self,
         model_id: Optional[str] = None,
         ref_data_id: Optional[str] = None,
         scheduled_ct_eval_data_integration_id: Optional[str] = None,
         scheduled_ct_eval_data_info: Optional[dict] = None,
         scheduled_ct_eval_pred_integration_id: Optional[str] = None,
@@ -181,14 +185,17 @@
             resp = api.firewall_service_update_firewall(
                 firewall_firewall_id_uuid=self._firewall_id,
                 body=req,
             )
         print(f"Firewall {self._firewall_id} updated successfully.")
         return resp
 
+    @deprecated(
+        "Firewall class methods will not be supported from Robust Intelligence v2.4."
+    )
     def activate_ct_scheduling(
         self,
         data_info: dict,
         data_integration_id: Optional[str] = None,
         pred_integration_id: Optional[str] = None,
         pred_info: Optional[dict] = None,
         rolling_window_size: Optional[timedelta] = None,
@@ -220,14 +227,17 @@
             scheduled_ct_eval_pred_info=pred_info,
             update_rolling_window=rolling_window_size is not None,
             scheduled_ct_rolling_window_size=rolling_window_size,
             disable_scheduled_ct=False,
         )
         print(f"Scheduled CT of Firewall {self._firewall_id} activated successfully.")
 
+    @deprecated(
+        "Firewall class methods will not be supported from Robust Intelligence v2.4."
+    )
     def update_scheduled_ct_info(
         self,
         data_integration_id: Optional[str] = None,
         data_info: Optional[dict] = None,
         pred_integration_id: Optional[str] = None,
         pred_info: Optional[dict] = None,
     ) -> None:
@@ -250,14 +260,17 @@
             scheduled_ct_eval_data_integration_id=data_integration_id,
             scheduled_ct_eval_data_info=data_info,
             scheduled_ct_eval_pred_integration_id=pred_integration_id,
             scheduled_ct_eval_pred_info=pred_info,
         )
         print(f"Location info of Firewall {self._firewall_id} updated successfully.")
 
+    @deprecated(
+        "Firewall class methods will not be supported from Robust Intelligence v2.4."
+    )
     def deactivate_ct_scheduling(self) -> None:
         """Deactivate scheduled CT."""
         if not self.is_scheduled_ct_enabled():
             raise ValueError("Scheduled CT is already disabled.")
         self.update_firewall(disable_scheduled_ct=True)
         print(f"Scheduled CT of Firewall {self._firewall_id} deactivated successfully.")
 
@@ -268,58 +281,79 @@
             "Link": make_link(
                 "https://" + self.get_link(),
                 link_text="Continuous Testing Overview Page",
             ),
         }
         return convert_dict_to_html(info)
 
+    @deprecated(
+        "Firewall class methods will not be supported from Robust Intelligence v2.4."
+    )
     def get_link(self) -> str:
         """Return a URL to the Firewall."""
         api = swagger_client.FirewallServiceApi(self._api_client)
         with RESTErrorHandler():
             resp = api.firewall_service_get_url(
                 firewall_id_uuid=self._firewall_id,
             )
         return resp.url.url
 
+    @deprecated(
+        "Firewall class methods will not be supported from Robust Intelligence v2.4."
+    )
     def get_bin_size(self) -> timedelta:
         """Return the bin size of this Firewall."""
         firewall = self._get_firewall()
         return rest_to_timedelta(firewall.bin_size)
 
+    @deprecated(
+        "Firewall class methods will not be supported from Robust Intelligence v2.4."
+    )
     def get_ref_data_id(self) -> str:
         """Return the ID of the Firewall's current reference set."""
         firewall = self._get_firewall()
         return firewall.ref_data_id
 
+    @deprecated(
+        "Firewall class methods will not be supported from Robust Intelligence v2.4."
+    )
     def get_model_id(self) -> str:
         """Return the ID of the Firewall's current model."""
         firewall = self._get_firewall()
         return firewall.model_id.uuid
 
+    @deprecated(
+        "Firewall class methods will not be supported from Robust Intelligence v2.4."
+    )
     def get_scheduled_ct_info(self) -> FirewallScheduledCTInfo:
         """Return the scheduled continuous testing info of this Firewall."""
         firewall = self._get_firewall()
         return firewall.scheduled_ct_info
 
+    @deprecated(
+        "Firewall class methods will not be supported from Robust Intelligence v2.4."
+    )
     def is_scheduled_ct_enabled(self) -> bool:
         """Return whether scheduled continuous testing is enabled for this Firewall."""
         firewall = self._get_firewall()
         is_enabled = firewall.scheduled_ct_info is not None
         is_enabled = is_enabled and not firewall.scheduled_ct_info.disable_scheduled_ct
         return is_enabled
 
     @property
     def project_id(self) -> str:
         """Return the ID of the parent project for this Firewall."""
         fw = self._get_firewall()
         return fw.project_id.uuid
 
+    @deprecated(
+        "Firewall class methods will not be supported from Robust Intelligence v2.4."
+    )
     @prompt_confirmation("Are you sure you want to delete this Firewall? (y/n) ")
-    def delete_firewall(  # pylint: disable=unused-argument
+    def delete_firewall(
         self,
         force: Optional[bool] = False,  # noqa: ARG002 (unused-method-argument)
     ) -> None:
         """Delete Firewall.
 
         Args:
             force: Optional[bool] = False
@@ -333,14 +367,17 @@
 
     def _get_firewall(self) -> FirewallFirewall:
         api = swagger_client.FirewallServiceApi(self._api_client)
         with RESTErrorHandler():
             res = api.firewall_service_get_firewall(firewall_id_uuid=self._firewall_id)
         return res.firewall
 
+    @deprecated(
+        "Firewall class methods will not be supported from Robust Intelligence v2.4."
+    )
     def get_events_df(
         self,
     ) -> pd.DataFrame:
         """Get a dataframe of Detected Events for the given Firewall.
 
         Monitors detect Events when degradations occur.
         For example, a Monitor for the metric "Accuracy" will detect an Event
@@ -367,14 +404,17 @@
                 )
                 next_page_token = res.next_page_token
                 has_more = res.has_more
                 all_events += res.events
         df = parse_events_to_df(all_events)
         return df
 
+    @deprecated(
+        "Firewall class methods will not be supported from Robust Intelligence v2.4."
+    )
     def list_monitors(
         self,
         monitor_types: Optional[List[str]] = None,
         risk_category_types: Optional[List[str]] = None,
     ) -> Iterator[Monitor]:
         """List Monitors for the given Firewall.
 
@@ -457,14 +497,17 @@
             for monitor in res.monitors:
                 yield Monitor(
                     self._api_client, monitor.id.uuid, self._firewall_id, project_id
                 )
             next_page_token = res.next_page_token
             has_more = res.has_more
 
+    @deprecated(
+        "Firewall class methods will not be supported from Robust Intelligence v2.4."
+    )
     def start_continuous_test(
         self,
         eval_data_id: str,
         override_existing_bins: bool = False,
         agent_id: Optional[str] = None,
         ram_request_megabytes: Optional[int] = None,
         cpu_request_millicores: Optional[int] = None,
@@ -551,26 +594,22 @@
             ),
             override_existing_bins=override_existing_bins,
             experimental_fields=exp_fields if exp_fields else None,
             agent_id=RimeUUID(agent_id) if agent_id else None,
         )
         if custom_image:
             req.test_run_incremental_config.run_time_info.custom_image = (
-                RuntimeinfoCustomImageType(  # pylint: disable=line-too-long
-                    custom_image=custom_image
-                )
+                RuntimeinfoCustomImageType(custom_image=custom_image)
             )
         if rime_managed_image:
             req.test_run_incremental_config.run_time_info.custom_image = (
-                RuntimeinfoCustomImageType(  # pylint: disable=line-too-long
-                    managed_image_name=rime_managed_image
-                )
+                RuntimeinfoCustomImageType(managed_image_name=rime_managed_image)
             )
         with RESTErrorHandler():
-            Firewall._throttler.throttle(  # pylint: disable=W0212
+            Firewall._throttler.throttle(
                 throttling_msg="Your request is throttled to limit # of model tests."
             )
             api = swagger_client.ModelTestingApi(self._api_client)
             job: RimeJobMetadata = api.model_testing_start_continuous_test(
                 body=req,
                 firewall_id_uuid=self._firewall_id,
             ).job
```

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/image_builder.py` & `rime_sdk-2.2.0rc3/rime_sdk/image_builder.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/internal/config_parser.py` & `rime_sdk-2.2.0rc3/rime_sdk/internal/config_parser.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/internal/constants.py` & `rime_sdk-2.2.0rc3/rime_sdk/internal/constants.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/internal/decorators.py` & `rime_sdk-2.2.0rc3/rime_sdk/internal/decorators.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/internal/file_upload.py` & `rime_sdk-2.2.0rc3/rime_sdk/internal/file_upload.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/internal/rest_error_handler.py` & `rime_sdk-2.2.0rc3/rime_sdk/internal/rest_error_handler.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,30 +12,32 @@
 
     Used so that we handle REST errors in a uniform way in the code base.
     """
 
     def __enter__(self) -> None:
         """Needed for context manager usage."""
 
-    def __exit__(  # pylint: disable=useless-return
+    def __exit__(
         self,
         exc_type: Optional[Type[BaseException]],
         exc: Optional[BaseException],
         traceback: Optional[TracebackType],
     ) -> Optional[bool]:
         """Handle exceptions in custom way on exit."""
         # Check if an exception was raised.
         if exc_type is not None:
             # For ApiException errors, we only raise the details.
             if isinstance(exc, ApiException):
                 if exc.body:
                     # Authentication (401) errors need to be handled separately as they are nginx messages
                     if exc.status == HTTPStatus.UNAUTHORIZED:
                         raise ValueError(
-                            f"{exc.reason}: Your API token is either invalid or expired. Please generate a new API token from the API Access Tokens page under Workspace Settings."  # pylint: disable=line-too-long
+                            f"{exc.reason}: Your API token is either invalid or "
+                            f"expired. Please generate a new API token from the API "
+                            f"Access Tokens page under Workspace Settings."
                         ) from None
                     else:
                         body_string = exc.body.decode("UTF-8")
                         # Safely interpret string as a python dict to pull out message
                         body_dict = ast.literal_eval(body_string)
                         raise ValueError(
                             f"{exc.reason}: {body_dict['message']}"
```

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/internal/security_config_parser.py` & `rime_sdk-2.2.0rc3/rime_sdk/internal/security_config_parser.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/internal/swagger_parser.py` & `rime_sdk-2.2.0rc3/rime_sdk/internal/swagger_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,15 +142,15 @@
     # to do this conversion.
     for key, value in DEFAULT_TEST_RUN_COLUMN_INFO.items():
         if value == "Int64":
             # Some nested fields such as `metrics.severity_counts.low` will be `None`
             # because MessageToDict does not populate nested primitive fields with
             # default values.
             # Since some columns may be `None`, we must convert to `float` first.
-            # https://stackoverflow.com/questions/60024262/error-converting-object-string-to-int32-typeerror-object-cannot-be-converted  # pylint: disable=line-too-long
+            # https://stackoverflow.com/questions/60024262/error-converting-object-string-to-int32-typeerror-object-cannot-be-converted
             full_df[key] = full_df[key].astype("float").astype("Int64")
 
     # Fix an order for the index of the df.
     non_default_cols = list(
         set(all_test_run_columns).difference(set(default_test_run_columns))
     )
     ordered_index = pd.Index(default_test_run_columns + sorted(non_default_cols))
@@ -175,15 +175,15 @@
     df = pd.json_normalize(result_dict, sep=DF_FLATTEN_SEPARATOR)
 
     for key in INT_TEST_BATCH_ATTRIBUTES:
         # Some nested fields such as `metrics.severity_counts.low` will be `None`
         # because MessageToDict does not populate nested primitive fields with
         # default values.
         # Since some columns may be `None`, we must convert to `float` first.
-        # https://stackoverflow.com/questions/60024262/error-converting-object-string-to-int32-typeerror-object-cannot-be-converted  # pylint: disable=line-too-long
+        # https://stackoverflow.com/questions/60024262/error-converting-object-string-to-int32-typeerror-object-cannot-be-converted
         df[key] = df[key].astype("float").astype("Int64")
 
     return df.squeeze(axis=0)
 
 
 def parse_test_case_result(
     raw_result: TestrunresultTestCase, unpack_metrics: bool = False
@@ -204,15 +204,15 @@
 
 
 def _add_metric_cols(
     result_dict: dict,
     raw_result: Union[TestrunresultTestCase, TestrunresultTestBatchResult],
 ) -> None:
     """Unpack test metrics into separate fields."""
-    if raw_result.metrics:  # pylint: disable=too-many-nested-blocks
+    if raw_result.metrics:
         for metric in raw_result.metrics:
             category_string = metric.category
             if category_string:
                 prefix = "TEST_METRIC_CATEGORY_"
                 category_string = category_string[len(prefix) :]
                 metric_value: Any = np.nan
                 if metric.empty:
```

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/internal/swagger_utils.py` & `rime_sdk-2.2.0rc3/rime_sdk/internal/swagger_utils.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/internal/test_helpers.py` & `rime_sdk-2.2.0rc3/rime_sdk/internal/test_helpers.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/internal/throttle_queue.py` & `rime_sdk-2.2.0rc3/rime_sdk/internal/throttle_queue.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/internal/utils.py` & `rime_sdk-2.2.0rc3/rime_sdk/internal/utils.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/job.py` & `rime_sdk-2.2.0rc3/rime_sdk/job.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,23 +18,22 @@
     RimeTestRunProgress,
     RimeTestTaskStatus,
     StatedbJobStatus,
 )
 from rime_sdk.swagger.swagger_client.rest import ApiException
 from rime_sdk.test_run import TestRun
 
-default_csv_header = ["test_name", "feature(s)", "status"]
-cancellable_job_types = [
+CANCELLABLE_JOB_TYPES = [
     RimeJobType.FIREWALL_BATCH_TEST,
     RimeJobType.MODEL_STRESS_TEST,
 ]
 # Format datetimes in user-readable format
-datetime_fields = ["creation_time", "start_time"]
+DATETIME_FIELDS = ["creation_time", "start_time"]
 # Removed if empty or overly verbose
-fields_to_be_removed = ["job_data", "archived_job_logs"]
+FIELDS_TO_BE_REMOVED = ["job_data", "archived_job_logs"]
 
 
 class BaseJob(ABC):
     """Abstract class for RIME Jobs.
 
     This object provides an interface for monitoring the status of a
     job in the RIME backend.
@@ -229,19 +228,19 @@
                 if e.status != HTTPStatus.NOT_FOUND:
                     raise ValueError(e.reason) from None
             # check for debug logs in the job
             print(f"Debug Logs: {self._get_debug_logs(job)}")
 
         job_dict = job.to_dict()
         # Hide job data and archived logs in the return value because it can get ugly.
-        for field in fields_to_be_removed:
+        for field in FIELDS_TO_BE_REMOVED:
             if field in job_dict:
                 del job_dict[field]
 
-        for field in datetime_fields:
+        for field in DATETIME_FIELDS:
             if field in job_dict and job_dict[field]:
                 job_dict[field] = job_dict[field].strftime("%H:%M %B %d, %Y")
 
         return job_dict
 
     @staticmethod
     def _format_logs(logs_string: str) -> str:
@@ -255,18 +254,18 @@
 
     def cancel(self) -> None:
         """Request to cancel the Job.
 
         The RIME cluster will mark the Job with "Cancellation Requested" and then clean
         up the Job.
         """
-        if self.job_type not in cancellable_job_types:
+        if self.job_type not in CANCELLABLE_JOB_TYPES:
             raise ValueError(
                 "Cancelling jobs is only supported for job types "
-                f"{cancellable_job_types}"
+                f"{CANCELLABLE_JOB_TYPES}"
             )
         api = swagger_client.JobReaderApi(self._api_client)
         with RESTErrorHandler():
             api.job_reader_cancel_job(job_id=self.job_id)
 
     def get_agent_id(self) -> str:
         """Return the Agent ID running the Job."""
```

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/monitor.py` & `rime_sdk-2.2.0rc3/rime_sdk/monitor.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/project.py` & `rime_sdk-2.2.0rc3/rime_sdk/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
     ProjectsProjectIdUuidBody,
     RimeActorRole,
     RimeCreateNotificationRequest,
     RimeJobType,
     RimeLicenseLimit,
     RimeLimitStatusStatus,
     RimeListNotificationsResponse,
+    RimeTestType,
     SchemanotificationConfig,
     StatedbJobStatus,
 )
 from rime_sdk.swagger.swagger_client.models.testrun_profiling_config import (
     TestrunProfilingConfig,
 )
 from rime_sdk.swagger.swagger_client.rest import ApiException
@@ -294,40 +295,57 @@
                 )
                 for job in res.jobs:
                     yield Job(self._api_client, job.job_id)
                 if not res.has_more:
                     break
                 page_token = res.next_page_token
 
-    def list_test_runs(self) -> Iterator[TestRun]:
-        """List the Stress Test Runs associated with this Project.
+    def list_test_runs(
+        self,
+        test_type: Optional[RimeTestType] = None,
+    ) -> Iterator[TestRun]:
+        """List the Test Runs associated with this Project.
+
+        Args:
+            test_type: Optional[RimeTestType] = None.
+                Filter for selecting test runs by RimeTestType.
+                If omitted, stress test runs are returned, excluding continuous test runs.
 
         Returns:
             Iterator[TestRun]:
                 An iterator of ``TestRun`` objects.
 
         Raises:
             ValueError
                 This error is generated when the request to the
                 ResultsReader Service fails.
 
         Example:
             .. code-block:: python
 
-                # List all test runs in the Project.
+                # List all stress test runs in the Project.
                 test_runs = project.list_test_runs()
-                # Get the IDs of all the test runs.
+                # Get the IDs of the test runs.
                 [test_run.test_run_id for test_run in test_runs]
+
+
+                # List all continuous test runs in the Project.
+                test_runs = project.list_test_runs(RimeTestType.CONTINUOUS_TESTING)
         """
         api = swagger_client.ResultsReaderApi(self._api_client)
         # Iterate through the pages of projects and break at the last page.
         page_token = ""
         while True:
             if page_token == "":
-                res = api.results_reader_list_test_runs(project_id=self._project_id)
+                res = api.results_reader_list_test_runs(
+                    first_page_query_project_id_uuid=self._project_id,
+                    first_page_query_testing_type=test_type
+                    if test_type is not None
+                    else RimeTestType.STRESS_TESTING_UNSPECIFIED,
+                )
             else:
                 res = api.results_reader_list_test_runs(page_token=page_token)
             if res.test_runs is not None:
                 for test_run in res.test_runs:
                     yield TestRun(self._api_client, test_run.test_run_id)
             # Advance to the next page of Test Cases.
             page_token = res.next_page_token
@@ -691,15 +709,14 @@
         if email is not None:
             notif_entry_str = "Email " + email
         elif webhook_config is not None:
             notif_entry_str = "Webhook " + webhook_config.webhook
         print(f"{notif_entry_str} not found for Notification type {notif_type_str}")
 
     def add_email(self, email: str, notif_type_str: str) -> None:
-        # pylint: disable=line-too-long
         """Add an email to the Notification settings for the specified Notification type.
 
         The valid Notification types are:
         ["Job_Action", "Monitoring", "Daily_Digest"]
 
         Example:
             .. code-block:: python
@@ -709,15 +726,14 @@
         if email == "":
             raise ValueError("Email must be a non-empty string")
         return self._add_notif_entry(
             notif_type_str=notif_type_str, email=email, webhook_config=None
         )
 
     def remove_email(self, email: str, notif_type_str: str) -> None:
-        # pylint: disable=line-too-long
         """Remove an email from the Notification settings for the specified Notification type.
 
         The valid Notification types are:
         ["Job_Action", "Monitoring", "Daily_Digest"]
 
         Example:
             .. code-block:: python
@@ -727,15 +743,14 @@
         if email == "":
             raise ValueError("Email must be a non-empty string")
         return self._remove_notif_entry(
             notif_type_str=notif_type_str, email=email, webhook_config=None
         )
 
     def add_webhook(self, webhook: str, notif_type_str: str) -> None:
-        # pylint: disable=line-too-long
         """Add a webhook to the Notification settings for the specified Notification type.
 
         The valid Notification types are:
         ["Job_Action", "Monitoring", "Daily_Digest"]
 
         Example:
             .. code-block:: python
@@ -746,15 +761,14 @@
             raise ValueError("Webhook must be a non empty string")
         webhook_config = NotificationWebhookConfig(webhook=webhook)
         return self._add_notif_entry(
             notif_type_str=notif_type_str, email=None, webhook_config=webhook_config
         )
 
     def remove_webhook(self, webhook: str, notif_type_str: str) -> None:
-        # pylint: disable=line-too-long,
         """Remove a webhook from the Notification settings for the specified Notification type.
 
         The valid Notification types are:
         ["Job_Action", "Monitoring", "Daily_Digest"]
 
         Example:
             .. code-block:: python
@@ -765,15 +779,15 @@
             raise ValueError("Webhook must be a non empty string")
         webhook_config = NotificationWebhookConfig(webhook=webhook)
         return self._remove_notif_entry(
             notif_type_str=notif_type_str, email=None, webhook_config=webhook_config
         )
 
     @prompt_confirmation("Are you sure you want to delete this Project? (y/n) ")
-    def delete(  # pylint: disable=unused-argument
+    def delete(
         self, force: Optional[bool] = False  # noqa: ARG002 (unused-method-argument)
     ) -> None:
         """Delete this Project.
 
         Args:
             force: Optional[bool] = False
                 When set to True, the Project will be deleted immediately. By default,
@@ -957,15 +971,15 @@
                 The chosen name of the dataset.
             file_path: Union[Path, str]
                 The local path to the dataset artifact, to be uploaded to Robust
                 Intelligence's blob store.
             upload_path: Optional[str] = None,
                 Name of the directory in the blob store file system. If omitted,
                 a unique random string will be the directory.
-            data_params: dict
+            data_params: Optional[dict] = None,
                 A dictionary that contains the data parameters.
                 The data parameters must match the API specification
                 of the `data_info.data_params` field in the `RegisterDataset` request.
             tags: Optional[List[str]] = None,
                 An optional list of tags to associate with the dataset.
             metadata: Optional[dict] = None,
                 An optional dictionary of metadata to associate with the dataset.
@@ -1015,14 +1029,15 @@
         self,
         name: str,
         model_config: Optional[dict] = None,
         tags: Optional[List[str]] = None,
         metadata: Optional[dict] = None,
         external_id: Optional[str] = None,
         integration_id: Optional[str] = None,
+        model_endpoint_integration_id: Optional[str] = None,
         skip_validation: Optional[bool] = False,
         agent_id: Optional[str] = None,
     ) -> str:
         """Register and validate a new model in this Project.
 
         Args:
             name: str
@@ -1036,15 +1051,18 @@
                 An optional list of tags to associate with the model.
             metadata: Optional[dict] = None,
                 An optional dictionary of metadata to associate with the model.
             external_id: Optional[str] = None,
                 An optional external ID that can be used to identify the model.
             integration_id: Optional[str] = None,
                 Provide the integration ID for models that require an
-                integration for access.
+                integration for accessing the model.
+            model_endpoint_integration_id: Optional[str] = None,
+                Provide the integration ID for models that require an
+                integration when running the model.
             skip_validation: Optional[bool] = False,
                 An optional boolean that indicates whether to skip validation.
                 Validation ensures that the model is valid for Robust
                 Intelligence's systems.
             agent_id: Optional[str] = None,
                 Agent for running validation. If omitted the workspace's default
                 agent will be used.
@@ -1085,26 +1103,28 @@
             self.project_id,
             name,
             model_config=model_config,
             tags=tags,
             metadata=metadata,
             external_id=external_id,
             integration_id=integration_id,
+            model_endpoint_integration_id=model_endpoint_integration_id,
             skip_validation=skip_validation,
             agent_id=agent_id,
         )
 
     def register_model_from_path(
         self,
         name: str,
         remote_path: str,
         tags: Optional[List[str]] = None,
         metadata: Optional[dict] = None,
         external_id: Optional[str] = None,
         integration_id: Optional[str] = None,
+        model_endpoint_integration_id: Optional[str] = None,
         skip_validation: Optional[bool] = False,
         agent_id: Optional[str] = None,
     ) -> str:
         """Register and validate a new model in this Project.
 
         Args:
             name: str
@@ -1116,14 +1136,17 @@
             metadata: Optional[dict] = None,
                 An optional dictionary of metadata to associate with the model.
             external_id: Optional[str] = None,
                 An optional external ID that can be used to identify the model.
             integration_id: Optional[str] = None,
                 Provide the integration ID for models that require an
                 integration for access.
+            model_endpoint_integration_id: Optional[str] = None,
+                Provide the integration ID for models that require an
+                integration when running the model.
             skip_validation: Optional[bool] = False,
                 An optional boolean that indicates whether to skip validation.
                 Validation ensures that the model is valid for Robust
                 Intelligence's systems.
             agent_id: Optional[str] = None,
                 Agent for running validation. If omitted the workspace's default
                 agent will be used.
@@ -1152,14 +1175,15 @@
             self.project_id,
             name,
             model_config,
             tags=tags,
             metadata=metadata,
             external_id=external_id,
             integration_id=integration_id,
+            model_endpoint_integration_id=model_endpoint_integration_id,
             skip_validation=skip_validation,
             agent_id=agent_id,
         )
 
     def upload_and_register_model_from_path(
         self,
         name: str,
```

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/registry.py` & `rime_sdk-2.2.0rc3/rime_sdk/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,14 +153,15 @@
         project_id: str,
         name: str,
         model_config: Optional[dict] = None,
         tags: Optional[List[str]] = None,
         metadata: Optional[dict] = None,
         external_id: Optional[str] = None,
         integration_id: Optional[str] = None,
+        model_endpoint_integration_id: Optional[str] = None,
         skip_validation: Optional[bool] = False,
         agent_id: Optional[str] = None,
     ) -> str:
         """Register and validate a new model in a Project.
 
         Args:
             project_id: str
@@ -177,14 +178,17 @@
             metadata: Optional[dict] = None,
                 An optional dictionary of metadata to associate with the model.
             external_id: Optional[str] = None,
                 An optional external ID that can be used to identify the model.
             integration_id: Optional[str] = None,
                 Provide the integration ID for models that require an
                 integration for access.
+            model_endpoint_integration_id: Optional[str] = None,
+                Provide the integration ID for models that require an
+                integration when running the model.
             skip_validation: Optional[bool] = False,
                 An optional boolean that indicates whether to skip validation.
                 Validation ensures that the model is valid for Robust
                 Intelligence's systems.
             agent_id: Optional[str] = None,
                 Agent for running validation. If omitted the workspace's default
                 agent will be used.
@@ -247,14 +251,18 @@
             metadata_str = json.dumps(metadata)
         if tags or metadata_str:
             req.metadata = RegistryMetadata(tags=tags, extra_info=metadata_str)
         if external_id:
             req.external_id = external_id
         if integration_id is not None:
             req.integration_id = RimeUUID(uuid=integration_id)
+        if model_endpoint_integration_id is not None:
+            req.model_endpoint_integration_id = RimeUUID(
+                uuid=model_endpoint_integration_id
+            )
 
         with RESTErrorHandler():
             api = swagger_client.RegistryServiceApi(self._api_client)
             res = api.registry_service_register_model(
                 body=req,
                 project_id_uuid=project_id,
             )
@@ -471,15 +479,14 @@
         if model_id is None and dataset_id is None:
             raise ValueError("Must specify either a model_id or dataset_id.")
         else:
             pass
         api = swagger_client.RegistryServiceApi(self._api_client)
         # Iterate through the pages of datasets and break at the last page.
         page_token = ""
-        # pylint: disable=line-too-long
         with RESTErrorHandler():
             while True:
                 if page_token == "":
                     if model_id is not None:
                         res: RimeListPredictionSetsResponse = (
                             api.registry_service_list_prediction_sets(
                                 project_id_uuid=project_id,
```

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/__init__.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,19 +164,14 @@
 from rime_sdk.swagger.swagger_client.models.project_remove_user_from_project_response import ProjectRemoveUserFromProjectResponse
 from rime_sdk.swagger.swagger_client.models.project_update_project_response import ProjectUpdateProjectResponse
 from rime_sdk.swagger.swagger_client.models.project_update_user_of_project_response import ProjectUpdateUserOfProjectResponse
 from rime_sdk.swagger.swagger_client.models.project_update_workspace_roles_for_project_response import ProjectUpdateWorkspaceRolesForProjectResponse
 from rime_sdk.swagger.swagger_client.models.projects_project_id_uuid_body import ProjectsProjectIdUuidBody
 from rime_sdk.swagger.swagger_client.models.protobuf_any import ProtobufAny
 from rime_sdk.swagger.swagger_client.models.protobuf_null_value import ProtobufNullValue
-from rime_sdk.swagger.swagger_client.models.rca_feature_cause import RcaFeatureCause
-from rime_sdk.swagger.swagger_client.models.rca_rca_result import RcaRCAResult
-from rime_sdk.swagger.swagger_client.models.rca_rca_role import RcaRCARole
-from rime_sdk.swagger.swagger_client.models.rca_test_case_cause import RcaTestCaseCause
-from rime_sdk.swagger.swagger_client.models.rca_test_case_id import RcaTestCaseID
 from rime_sdk.swagger.swagger_client.models.registry_connection_info import RegistryConnectionInfo
 from rime_sdk.swagger.swagger_client.models.registry_data_collector_info import RegistryDataCollectorInfo
 from rime_sdk.swagger.swagger_client.models.registry_data_file_info import RegistryDataFileInfo
 from rime_sdk.swagger.swagger_client.models.registry_data_info import RegistryDataInfo
 from rime_sdk.swagger.swagger_client.models.registry_data_loading_info import RegistryDataLoadingInfo
 from rime_sdk.swagger.swagger_client.models.registry_data_params import RegistryDataParams
 from rime_sdk.swagger.swagger_client.models.registry_data_type import RegistryDataType
```

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/api/__init__.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/api/agent_manager_api.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/agent_manager_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/api/config_validator_api.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/config_validator_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/api/customer_managed_key_service_api.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/customer_managed_key_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/api/data_collector_api.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/data_collector_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/api/detection_api.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/detection_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/api/feature_flag_api.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/feature_flag_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/api/file_scanning_api.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/file_scanning_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/api/file_upload_api.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/file_upload_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/api/firewall_service_api.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/firewall_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/api/image_registry_api.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/image_registry_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/api/integration_service_api.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/integration_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/api/job_reader_api.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/job_reader_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/api/model_card_service_api.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/model_card_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/api/model_testing_api.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/model_testing_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/api/monitor_service_api.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/monitor_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/api/notification_setting_api.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/notification_setting_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/api/project_service_api.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/project_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/api/registry_service_api.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/registry_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/api/results_reader_api.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/results_reader_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/api/rime_info_api.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/rime_info_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/api/user_api.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/user_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/api/validation_service_api.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/validation_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/api/workspace_service_api.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/workspace_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/api_client.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api_client.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/configuration.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/configuration.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/__init__.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,19 +136,14 @@
 from rime_sdk.swagger.swagger_client.models.project_remove_user_from_project_response import ProjectRemoveUserFromProjectResponse
 from rime_sdk.swagger.swagger_client.models.project_update_project_response import ProjectUpdateProjectResponse
 from rime_sdk.swagger.swagger_client.models.project_update_user_of_project_response import ProjectUpdateUserOfProjectResponse
 from rime_sdk.swagger.swagger_client.models.project_update_workspace_roles_for_project_response import ProjectUpdateWorkspaceRolesForProjectResponse
 from rime_sdk.swagger.swagger_client.models.projects_project_id_uuid_body import ProjectsProjectIdUuidBody
 from rime_sdk.swagger.swagger_client.models.protobuf_any import ProtobufAny
 from rime_sdk.swagger.swagger_client.models.protobuf_null_value import ProtobufNullValue
-from rime_sdk.swagger.swagger_client.models.rca_feature_cause import RcaFeatureCause
-from rime_sdk.swagger.swagger_client.models.rca_rca_result import RcaRCAResult
-from rime_sdk.swagger.swagger_client.models.rca_rca_role import RcaRCARole
-from rime_sdk.swagger.swagger_client.models.rca_test_case_cause import RcaTestCaseCause
-from rime_sdk.swagger.swagger_client.models.rca_test_case_id import RcaTestCaseID
 from rime_sdk.swagger.swagger_client.models.registry_connection_info import RegistryConnectionInfo
 from rime_sdk.swagger.swagger_client.models.registry_data_collector_info import RegistryDataCollectorInfo
 from rime_sdk.swagger.swagger_client.models.registry_data_file_info import RegistryDataFileInfo
 from rime_sdk.swagger.swagger_client.models.registry_data_info import RegistryDataInfo
 from rime_sdk.swagger.swagger_client.models.registry_data_loading_info import RegistryDataLoadingInfo
 from rime_sdk.swagger.swagger_client.models.registry_data_params import RegistryDataParams
 from rime_sdk.swagger.swagger_client.models.registry_data_type import RegistryDataType
```

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/configvalidator_config_type_body.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/configvalidator_config_type_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/continuoustests_firewall_id_uuid_body.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/continuoustests_firewall_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/create_agent_request_azure_config.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/create_agent_request_azure_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/customermanagedkey_customer_managed_key_config.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/customermanagedkey_customer_managed_key_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_provider.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_provider.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_status.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/data_params_feature_intersection.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/data_params_feature_intersection.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/data_params_ranking_info.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/data_params_ranking_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/data_profiling_column_type_info.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/data_profiling_column_type_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/data_profiling_feature_relationship_info.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/data_profiling_feature_relationship_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/datacollector_datapoint.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/datacollector_datapoint.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/datacollector_datapoint_row.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/datacollector_datapoint_row.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/dataset_ct_dataset_type.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/dataset_ct_dataset_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/dataset_ct_info.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/dataset_ct_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/dataset_dataset.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/dataset_dataset.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/dataset_id_prediction_body.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/dataset_id_prediction_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/datastream_project_id_uuid_body.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/datastream_project_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/detection_detection_event.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/detection_detection_event.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,16 +38,15 @@
         'event_time_range': 'RimeTimeInterval',
         'last_update_time': 'datetime',
         'risk_category_type': 'RiskscoreRiskCategoryType',
         'test_category': 'TestrunTestCategoryType',
         'description': 'str',
         'description_html': 'str',
         'resolution': 'DetectionResolution',
-        'detail': 'DetectionEventDetail',
-        'rca_role': 'RcaRCARole'
+        'detail': 'DetectionEventDetail'
     }
 
     attribute_map = {
         'id': 'id',
         'project_id': 'projectId',
         'firewall_id': 'firewallId',
         'event_type': 'eventType',
@@ -57,19 +56,18 @@
         'event_time_range': 'eventTimeRange',
         'last_update_time': 'lastUpdateTime',
         'risk_category_type': 'riskCategoryType',
         'test_category': 'testCategory',
         'description': 'description',
         'description_html': 'descriptionHtml',
         'resolution': 'resolution',
-        'detail': 'detail',
-        'rca_role': 'rcaRole'
+        'detail': 'detail'
     }
 
-    def __init__(self, id=None, project_id=None, firewall_id=None, event_type=None, severity=None, event_object_id=None, event_object_name=None, event_time_range=None, last_update_time=None, risk_category_type=None, test_category=None, description=None, description_html=None, resolution=None, detail=None, rca_role=None):  # noqa: E501
+    def __init__(self, id=None, project_id=None, firewall_id=None, event_type=None, severity=None, event_object_id=None, event_object_name=None, event_time_range=None, last_update_time=None, risk_category_type=None, test_category=None, description=None, description_html=None, resolution=None, detail=None):  # noqa: E501
         """DetectionDetectionEvent - a model defined in Swagger"""  # noqa: E501
         self._id = None
         self._project_id = None
         self._firewall_id = None
         self._event_type = None
         self._severity = None
         self._event_object_id = None
@@ -78,15 +76,14 @@
         self._last_update_time = None
         self._risk_category_type = None
         self._test_category = None
         self._description = None
         self._description_html = None
         self._resolution = None
         self._detail = None
-        self._rca_role = None
         self.discriminator = None
         if id is not None:
             self.id = id
         if project_id is not None:
             self.project_id = project_id
         if firewall_id is not None:
             self.firewall_id = firewall_id
@@ -110,16 +107,14 @@
             self.description = description
         if description_html is not None:
             self.description_html = description_html
         if resolution is not None:
             self.resolution = resolution
         if detail is not None:
             self.detail = detail
-        if rca_role is not None:
-            self.rca_role = rca_role
 
     @property
     def id(self):
         """Gets the id of this DetectionDetectionEvent.  # noqa: E501
 
 
         :return: The id of this DetectionDetectionEvent.  # noqa: E501
@@ -436,35 +431,14 @@
 
         :param detail: The detail of this DetectionDetectionEvent.  # noqa: E501
         :type: DetectionEventDetail
         """
 
         self._detail = detail
 
-    @property
-    def rca_role(self):
-        """Gets the rca_role of this DetectionDetectionEvent.  # noqa: E501
-
-
-        :return: The rca_role of this DetectionDetectionEvent.  # noqa: E501
-        :rtype: RcaRCARole
-        """
-        return self._rca_role
-
-    @rca_role.setter
-    def rca_role(self, rca_role):
-        """Sets the rca_role of this DetectionDetectionEvent.
-
-
-        :param rca_role: The rca_role of this DetectionDetectionEvent.  # noqa: E501
-        :type: RcaRCARole
-        """
-
-        self._rca_role = rca_role
-
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/detection_event_detail.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/detection_event_detail.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/detection_event_type.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/detection_event_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/detection_metric_degradation_event_details.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,87 +11,87 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class DetectionMetricDegradationEventDetails(object):
+class StreamResultOfRimeGetPredictionsResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'event_context_range': 'RimeTimeInterval',
-        'rca_result': 'RcaRCAResult'
+        'result': 'RimeGetPredictionsResponse',
+        'error': 'GooglerpcStatus'
     }
 
     attribute_map = {
-        'event_context_range': 'eventContextRange',
-        'rca_result': 'rcaResult'
+        'result': 'result',
+        'error': 'error'
     }
 
-    def __init__(self, event_context_range=None, rca_result=None):  # noqa: E501
-        """DetectionMetricDegradationEventDetails - a model defined in Swagger"""  # noqa: E501
-        self._event_context_range = None
-        self._rca_result = None
+    def __init__(self, result=None, error=None):  # noqa: E501
+        """StreamResultOfRimeGetPredictionsResponse - a model defined in Swagger"""  # noqa: E501
+        self._result = None
+        self._error = None
         self.discriminator = None
-        if event_context_range is not None:
-            self.event_context_range = event_context_range
-        if rca_result is not None:
-            self.rca_result = rca_result
+        if result is not None:
+            self.result = result
+        if error is not None:
+            self.error = error
 
     @property
-    def event_context_range(self):
-        """Gets the event_context_range of this DetectionMetricDegradationEventDetails.  # noqa: E501
+    def result(self):
+        """Gets the result of this StreamResultOfRimeGetPredictionsResponse.  # noqa: E501
 
 
-        :return: The event_context_range of this DetectionMetricDegradationEventDetails.  # noqa: E501
-        :rtype: RimeTimeInterval
+        :return: The result of this StreamResultOfRimeGetPredictionsResponse.  # noqa: E501
+        :rtype: RimeGetPredictionsResponse
         """
-        return self._event_context_range
+        return self._result
 
-    @event_context_range.setter
-    def event_context_range(self, event_context_range):
-        """Sets the event_context_range of this DetectionMetricDegradationEventDetails.
+    @result.setter
+    def result(self, result):
+        """Sets the result of this StreamResultOfRimeGetPredictionsResponse.
 
 
-        :param event_context_range: The event_context_range of this DetectionMetricDegradationEventDetails.  # noqa: E501
-        :type: RimeTimeInterval
+        :param result: The result of this StreamResultOfRimeGetPredictionsResponse.  # noqa: E501
+        :type: RimeGetPredictionsResponse
         """
 
-        self._event_context_range = event_context_range
+        self._result = result
 
     @property
-    def rca_result(self):
-        """Gets the rca_result of this DetectionMetricDegradationEventDetails.  # noqa: E501
+    def error(self):
+        """Gets the error of this StreamResultOfRimeGetPredictionsResponse.  # noqa: E501
 
 
-        :return: The rca_result of this DetectionMetricDegradationEventDetails.  # noqa: E501
-        :rtype: RcaRCAResult
+        :return: The error of this StreamResultOfRimeGetPredictionsResponse.  # noqa: E501
+        :rtype: GooglerpcStatus
         """
-        return self._rca_result
+        return self._error
 
-    @rca_result.setter
-    def rca_result(self, rca_result):
-        """Sets the rca_result of this DetectionMetricDegradationEventDetails.
+    @error.setter
+    def error(self, error):
+        """Sets the error of this StreamResultOfRimeGetPredictionsResponse.
 
 
-        :param rca_result: The rca_result of this DetectionMetricDegradationEventDetails.  # noqa: E501
-        :type: RcaRCAResult
+        :param error: The error of this StreamResultOfRimeGetPredictionsResponse.  # noqa: E501
+        :type: GooglerpcStatus
         """
 
-        self._rca_result = rca_result
+        self._error = error
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -106,15 +106,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(DetectionMetricDegradationEventDetails, dict):
+        if issubclass(StreamResultOfRimeGetPredictionsResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -122,15 +122,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, DetectionMetricDegradationEventDetails):
+        if not isinstance(other, StreamResultOfRimeGetPredictionsResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/detection_resolution.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/detection_resolution.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/detection_security_event_details.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/detection_security_event_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/difference_from_target_difference.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/difference_from_target_difference.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/difference_from_target_target.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/difference_from_target_target.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/digest_config_digest_frequency.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/digest_config_digest_frequency.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/featureflags_customer_name_body.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/featureflags_customer_name_body.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,16 +35,15 @@
         'signed_jwt_token_str': 'signedJwtTokenStr'
     }
 
     def __init__(self, signed_jwt_token_str=None):  # noqa: E501
         """FeatureflagsCustomerNameBody - a model defined in Swagger"""  # noqa: E501
         self._signed_jwt_token_str = None
         self.discriminator = None
-        if signed_jwt_token_str is not None:
-            self.signed_jwt_token_str = signed_jwt_token_str
+        self.signed_jwt_token_str = signed_jwt_token_str
 
     @property
     def signed_jwt_token_str(self):
         """Gets the signed_jwt_token_str of this FeatureflagsCustomerNameBody.  # noqa: E501
 
         This is the signed JWT token (with RI private key that we don't share). We embed the public key in FeatureFlag server on startup. The jwt token str is decode with public key, and only updates DB on successful decoding (means it was encoded with right private key).  # noqa: E501
 
@@ -58,14 +57,16 @@
         """Sets the signed_jwt_token_str of this FeatureflagsCustomerNameBody.
 
         This is the signed JWT token (with RI private key that we don't share). We embed the public key in FeatureFlag server on startup. The jwt token str is decode with public key, and only updates DB on successful decoding (means it was encoded with right private key).  # noqa: E501
 
         :param signed_jwt_token_str: The signed_jwt_token_str of this FeatureflagsCustomerNameBody.  # noqa: E501
         :type: str
         """
+        if signed_jwt_token_str is None:
+            raise ValueError("Invalid value for `signed_jwt_token_str`, must not be `None`")  # noqa: E501
 
         self._signed_jwt_token_str = signed_jwt_token_str
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/filescanning_file_scan_result.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/filescanning_file_scan_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/filescanning_huggingface_model_info.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/filescanning_huggingface_model_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/filescanning_model_file_info.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/filescanning_model_file_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/filescanning_pytorch_model_info.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/filescanning_pytorch_model_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/filescanning_security_report.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/filescanning_security_report.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/filescanning_security_report_import_result.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/filescanning_security_report_import_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/firewall_firewall.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/firewall_firewall.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/generativestresstests_project_id_uuid_body.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/generativestresstests_project_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/googlerpc_status.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/googlerpc_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/heartbeat_agent_id_uuid_body.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/heartbeat_agent_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/integration_integration_level.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/integration_integration_level.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/integration_integration_schema.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/integration_integration_schema.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/integration_integration_type.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/integration_integration_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/integrations_integration_id_uuid_body.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/integrations_integration_id_uuid_body.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,16 +40,15 @@
     def __init__(self, integration_id=None, variables=None):  # noqa: E501
         """IntegrationsIntegrationIdUuidBody - a model defined in Swagger"""  # noqa: E501
         self._integration_id = None
         self._variables = None
         self.discriminator = None
         if integration_id is not None:
             self.integration_id = integration_id
-        if variables is not None:
-            self.variables = variables
+        self.variables = variables
 
     @property
     def integration_id(self):
         """Gets the integration_id of this IntegrationsIntegrationIdUuidBody.  # noqa: E501
 
         Unique ID of an object in RIME.  # noqa: E501
 
@@ -84,14 +83,16 @@
     def variables(self, variables):
         """Sets the variables of this IntegrationsIntegrationIdUuidBody.
 
 
         :param variables: The variables of this IntegrationsIntegrationIdUuidBody.  # noqa: E501
         :type: list[RimeConfigureIntegrationRequestIntegrationVariable]
         """
+        if variables is None:
+            raise ValueError("Invalid value for `variables`, must not be `None`")  # noqa: E501
 
         self._variables = variables
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/job_data_continuous_incremental_test.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/job_data_continuous_incremental_test.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/job_data_stress_test.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/job_data_stress_test.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/list_agents_request_list_agents_query.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/list_agents_request_list_agents_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/list_datasets_request_datasets_query.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/list_datasets_request_datasets_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/list_images_request_pip_library_filter.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/list_images_request_pip_library_filter.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_aggregated_metric.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_aggregated_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metric_without_subsets.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metric_without_subsets.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metrics.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metrics.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metric.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metrics.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metrics.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/list_models_request_model_query.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/list_models_request_model_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/list_monitors_request_filter.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/list_monitors_request_filter.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/list_notifications_request_list_notifications_query.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/list_notifications_request_list_notifications_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/list_prediction_sets_request_prediction_query.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/list_prediction_sets_request_prediction_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/list_summary_tests_request_list_summary_tests_query.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/list_summary_tests_request_list_summary_tests_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/list_test_cases_request_list_test_cases_query.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/list_test_cases_request_list_test_cases_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/managed_image_package_requirement.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/managed_image_package_requirement.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/managed_image_package_type.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/managed_image_package_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/managed_image_pip_library.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/managed_image_pip_library.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/managed_image_pip_requirement.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/managed_image_pip_requirement.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/managed_image_role_type.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/managed_image_role_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/model_model.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/model_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,42 +33,45 @@
         'project_ids': 'list[RimeUUID]',
         'creator_id': 'RimeUUID',
         'creation_time': 'datetime',
         'external_id': 'str',
         'user_metadata': 'RegistryMetadata',
         'model_info': 'RegistryModelInfo',
         'validity_status': 'RegistryValidityStatus',
-        'integration_id': 'RimeUUID'
+        'integration_id': 'RimeUUID',
+        'model_endpoint_integration_id': 'RimeUUID'
     }
 
     attribute_map = {
         'name': 'name',
         'model_id': 'modelId',
         'project_ids': 'projectIds',
         'creator_id': 'creatorId',
         'creation_time': 'creationTime',
         'external_id': 'externalId',
         'user_metadata': 'userMetadata',
         'model_info': 'modelInfo',
         'validity_status': 'validityStatus',
-        'integration_id': 'integrationId'
+        'integration_id': 'integrationId',
+        'model_endpoint_integration_id': 'modelEndpointIntegrationId'
     }
 
-    def __init__(self, name=None, model_id=None, project_ids=None, creator_id=None, creation_time=None, external_id=None, user_metadata=None, model_info=None, validity_status=None, integration_id=None):  # noqa: E501
+    def __init__(self, name=None, model_id=None, project_ids=None, creator_id=None, creation_time=None, external_id=None, user_metadata=None, model_info=None, validity_status=None, integration_id=None, model_endpoint_integration_id=None):  # noqa: E501
         """ModelModel - a model defined in Swagger"""  # noqa: E501
         self._name = None
         self._model_id = None
         self._project_ids = None
         self._creator_id = None
         self._creation_time = None
         self._external_id = None
         self._user_metadata = None
         self._model_info = None
         self._validity_status = None
         self._integration_id = None
+        self._model_endpoint_integration_id = None
         self.discriminator = None
         if name is not None:
             self.name = name
         if model_id is not None:
             self.model_id = model_id
         if project_ids is not None:
             self.project_ids = project_ids
@@ -82,14 +85,16 @@
             self.user_metadata = user_metadata
         if model_info is not None:
             self.model_info = model_info
         if validity_status is not None:
             self.validity_status = validity_status
         if integration_id is not None:
             self.integration_id = integration_id
+        if model_endpoint_integration_id is not None:
+            self.model_endpoint_integration_id = model_endpoint_integration_id
 
     @property
     def name(self):
         """Gets the name of this ModelModel.  # noqa: E501
 
         Name and model_id are both enforced to be unique. Name is user specified. Model_id is internally generated.  # noqa: E501
 
@@ -299,14 +304,35 @@
 
         :param integration_id: The integration_id of this ModelModel.  # noqa: E501
         :type: RimeUUID
         """
 
         self._integration_id = integration_id
 
+    @property
+    def model_endpoint_integration_id(self):
+        """Gets the model_endpoint_integration_id of this ModelModel.  # noqa: E501
+
+
+        :return: The model_endpoint_integration_id of this ModelModel.  # noqa: E501
+        :rtype: RimeUUID
+        """
+        return self._model_endpoint_integration_id
+
+    @model_endpoint_integration_id.setter
+    def model_endpoint_integration_id(self, model_endpoint_integration_id):
+        """Sets the model_endpoint_integration_id of this ModelModel.
+
+
+        :param model_endpoint_integration_id: The model_endpoint_integration_id of this ModelModel.  # noqa: E501
+        :type: RimeUUID
+        """
+
+        self._model_endpoint_integration_id = model_endpoint_integration_id
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/modelcards_model_card_model_card_id_uuid_body.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/modelcards_model_card_model_card_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/monitor_aggregation.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/monitor_aggregation.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/monitor_aggregation_type.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/monitor_aggregation_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/monitor_anomaly_config.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/monitor_anomaly_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/monitor_artifact_identifier.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/monitor_artifact_identifier.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/monitor_difference_from_target.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/monitor_difference_from_target.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/monitor_excluded_transforms.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/monitor_excluded_transforms.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/monitor_metric_degradation_config.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/monitor_metric_degradation_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/monitor_monitor.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/monitor_monitor.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,14 @@
         'firewall_id': 'RimeUUID',
         'monitor_type': 'MonitorMonitorType',
         'risk_category_type': 'RiskscoreRiskCategoryType',
         'test_category': 'TestrunTestCategoryType',
         'artifact_identifier': 'MonitorArtifactIdentifier',
         'created_time': 'datetime',
         'notify': 'bool',
-        'rca_role': 'RcaRCARole',
         'config': 'SchemamonitorConfig',
         'excluded_transforms': 'MonitorExcludedTransforms',
         'pinned': 'bool'
     }
 
     attribute_map = {
         'id': 'id',
@@ -49,32 +48,30 @@
         'firewall_id': 'firewallId',
         'monitor_type': 'monitorType',
         'risk_category_type': 'riskCategoryType',
         'test_category': 'testCategory',
         'artifact_identifier': 'artifactIdentifier',
         'created_time': 'createdTime',
         'notify': 'notify',
-        'rca_role': 'rcaRole',
         'config': 'config',
         'excluded_transforms': 'excludedTransforms',
         'pinned': 'pinned'
     }
 
-    def __init__(self, id=None, name=None, firewall_id=None, monitor_type=None, risk_category_type=None, test_category=None, artifact_identifier=None, created_time=None, notify=None, rca_role=None, config=None, excluded_transforms=None, pinned=None):  # noqa: E501
+    def __init__(self, id=None, name=None, firewall_id=None, monitor_type=None, risk_category_type=None, test_category=None, artifact_identifier=None, created_time=None, notify=None, config=None, excluded_transforms=None, pinned=None):  # noqa: E501
         """MonitorMonitor - a model defined in Swagger"""  # noqa: E501
         self._id = None
         self._name = None
         self._firewall_id = None
         self._monitor_type = None
         self._risk_category_type = None
         self._test_category = None
         self._artifact_identifier = None
         self._created_time = None
         self._notify = None
-        self._rca_role = None
         self._config = None
         self._excluded_transforms = None
         self._pinned = None
         self.discriminator = None
         if id is not None:
             self.id = id
         if name is not None:
@@ -89,16 +86,14 @@
             self.test_category = test_category
         if artifact_identifier is not None:
             self.artifact_identifier = artifact_identifier
         if created_time is not None:
             self.created_time = created_time
         if notify is not None:
             self.notify = notify
-        if rca_role is not None:
-            self.rca_role = rca_role
         if config is not None:
             self.config = config
         if excluded_transforms is not None:
             self.excluded_transforms = excluded_transforms
         if pinned is not None:
             self.pinned = pinned
 
@@ -294,35 +289,14 @@
         :param notify: The notify of this MonitorMonitor.  # noqa: E501
         :type: bool
         """
 
         self._notify = notify
 
     @property
-    def rca_role(self):
-        """Gets the rca_role of this MonitorMonitor.  # noqa: E501
-
-
-        :return: The rca_role of this MonitorMonitor.  # noqa: E501
-        :rtype: RcaRCARole
-        """
-        return self._rca_role
-
-    @rca_role.setter
-    def rca_role(self, rca_role):
-        """Sets the rca_role of this MonitorMonitor.
-
-
-        :param rca_role: The rca_role of this MonitorMonitor.  # noqa: E501
-        :type: RcaRCARole
-        """
-
-        self._rca_role = rca_role
-
-    @property
     def config(self):
         """Gets the config of this MonitorMonitor.  # noqa: E501
 
 
         :return: The config of this MonitorMonitor.  # noqa: E501
         :rtype: SchemamonitorConfig
         """
```

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/monitor_monitor_type.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/monitor_monitor_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/monitor_threshold.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/monitor_threshold.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/monitor_threshold_type.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/monitor_threshold_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/monitor_transform.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/monitor_transform.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/monitoring_config_alert_level.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/monitoring_config_alert_level.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/monitors_monitor_id_uuid_body.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/monitors_monitor_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/notification_digest_config.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/notification_digest_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/notification_job_action_config.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/notification_job_action_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/notification_monitoring_config.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/notification_monitoring_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/notification_notification.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/notification_notification.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/notification_notification_type.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/notification_notification_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/notification_object_type.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/notification_object_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/notification_webhook_config.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/notification_webhook_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/notifsettings_notification_id_uuid_body.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/notifsettings_notification_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/predictions_model_id_uuid_body.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/predictions_model_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/project_add_users_to_project_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_add_users_to_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/project_create_project_request.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_create_project_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/project_create_project_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_create_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/project_delete_project_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_delete_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/project_get_project_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_get_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/project_get_project_url_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_get_project_url_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/project_get_workspace_roles_for_project_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_get_workspace_roles_for_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/project_id_uuid_dataset_body.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_id_uuid_dataset_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/project_id_uuid_model_body.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_id_uuid_model_body.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,38 +31,41 @@
         'project_id': 'object',
         'name': 'str',
         'metadata': 'RegistryMetadata',
         'external_id': 'str',
         'model_info': 'RegistryModelInfo',
         'integration_id': 'RimeUUID',
         'skip_validation': 'bool',
-        'agent_id': 'RimeUUID'
+        'agent_id': 'RimeUUID',
+        'model_endpoint_integration_id': 'RimeUUID'
     }
 
     attribute_map = {
         'project_id': 'projectId',
         'name': 'name',
         'metadata': 'metadata',
         'external_id': 'externalId',
         'model_info': 'modelInfo',
         'integration_id': 'integrationId',
         'skip_validation': 'skipValidation',
-        'agent_id': 'agentId'
+        'agent_id': 'agentId',
+        'model_endpoint_integration_id': 'modelEndpointIntegrationId'
     }
 
-    def __init__(self, project_id=None, name=None, metadata=None, external_id=None, model_info=None, integration_id=None, skip_validation=None, agent_id=None):  # noqa: E501
+    def __init__(self, project_id=None, name=None, metadata=None, external_id=None, model_info=None, integration_id=None, skip_validation=None, agent_id=None, model_endpoint_integration_id=None):  # noqa: E501
         """ProjectIdUuidModelBody - a model defined in Swagger"""  # noqa: E501
         self._project_id = None
         self._name = None
         self._metadata = None
         self._external_id = None
         self._model_info = None
         self._integration_id = None
         self._skip_validation = None
         self._agent_id = None
+        self._model_endpoint_integration_id = None
         self.discriminator = None
         if project_id is not None:
             self.project_id = project_id
         self.name = name
         if metadata is not None:
             self.metadata = metadata
         if external_id is not None:
@@ -71,14 +74,16 @@
             self.model_info = model_info
         if integration_id is not None:
             self.integration_id = integration_id
         if skip_validation is not None:
             self.skip_validation = skip_validation
         if agent_id is not None:
             self.agent_id = agent_id
+        if model_endpoint_integration_id is not None:
+            self.model_endpoint_integration_id = model_endpoint_integration_id
 
     @property
     def project_id(self):
         """Gets the project_id of this ProjectIdUuidModelBody.  # noqa: E501
 
         Uniquely specifies a Project.  # noqa: E501
 
@@ -250,14 +255,35 @@
 
         :param agent_id: The agent_id of this ProjectIdUuidModelBody.  # noqa: E501
         :type: RimeUUID
         """
 
         self._agent_id = agent_id
 
+    @property
+    def model_endpoint_integration_id(self):
+        """Gets the model_endpoint_integration_id of this ProjectIdUuidModelBody.  # noqa: E501
+
+
+        :return: The model_endpoint_integration_id of this ProjectIdUuidModelBody.  # noqa: E501
+        :rtype: RimeUUID
+        """
+        return self._model_endpoint_integration_id
+
+    @model_endpoint_integration_id.setter
+    def model_endpoint_integration_id(self, model_endpoint_integration_id):
+        """Sets the model_endpoint_integration_id of this ProjectIdUuidModelBody.
+
+
+        :param model_endpoint_integration_id: The model_endpoint_integration_id of this ProjectIdUuidModelBody.  # noqa: E501
+        :type: RimeUUID
+        """
+
+        self._model_endpoint_integration_id = model_endpoint_integration_id
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/project_list_projects_request_query.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_list_projects_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/project_list_projects_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_list_projects_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/project_list_users_of_project_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_list_users_of_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/project_owner_details.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_owner_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/project_project.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_project.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/project_project_with_details.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_project_with_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/project_remove_user_from_project_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_remove_user_from_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/project_update_project_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_update_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/project_update_user_of_project_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_update_user_of_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/project_update_workspace_roles_for_project_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_update_workspace_roles_for_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/projects_project_id_uuid_body.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/projects_project_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/protobuf_any.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/protobuf_any.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/protobuf_null_value.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/protobuf_null_value.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rca_rca_result.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_users_response.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,115 +11,113 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RcaRCAResult(object):
+class RimeListUsersResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'feature_causes': 'list[RcaFeatureCause]',
-        'description': 'str',
-        'description_html': 'str'
+        'users': 'list[UserUserDetail]',
+        'next_page_token': 'str',
+        'has_more': 'bool'
     }
 
     attribute_map = {
-        'feature_causes': 'featureCauses',
-        'description': 'description',
-        'description_html': 'descriptionHtml'
+        'users': 'users',
+        'next_page_token': 'nextPageToken',
+        'has_more': 'hasMore'
     }
 
-    def __init__(self, feature_causes=None, description=None, description_html=None):  # noqa: E501
-        """RcaRCAResult - a model defined in Swagger"""  # noqa: E501
-        self._feature_causes = None
-        self._description = None
-        self._description_html = None
+    def __init__(self, users=None, next_page_token=None, has_more=None):  # noqa: E501
+        """RimeListUsersResponse - a model defined in Swagger"""  # noqa: E501
+        self._users = None
+        self._next_page_token = None
+        self._has_more = None
         self.discriminator = None
-        if feature_causes is not None:
-            self.feature_causes = feature_causes
-        if description is not None:
-            self.description = description
-        if description_html is not None:
-            self.description_html = description_html
+        if users is not None:
+            self.users = users
+        if next_page_token is not None:
+            self.next_page_token = next_page_token
+        if has_more is not None:
+            self.has_more = has_more
 
     @property
-    def feature_causes(self):
-        """Gets the feature_causes of this RcaRCAResult.  # noqa: E501
+    def users(self):
+        """Gets the users of this RimeListUsersResponse.  # noqa: E501
 
-        Potentially problematic features that may have caused the MetricDegradationEvent. Sorted by confidence score.  # noqa: E501
 
-        :return: The feature_causes of this RcaRCAResult.  # noqa: E501
-        :rtype: list[RcaFeatureCause]
+        :return: The users of this RimeListUsersResponse.  # noqa: E501
+        :rtype: list[UserUserDetail]
         """
-        return self._feature_causes
+        return self._users
 
-    @feature_causes.setter
-    def feature_causes(self, feature_causes):
-        """Sets the feature_causes of this RcaRCAResult.
+    @users.setter
+    def users(self, users):
+        """Sets the users of this RimeListUsersResponse.
 
-        Potentially problematic features that may have caused the MetricDegradationEvent. Sorted by confidence score.  # noqa: E501
 
-        :param feature_causes: The feature_causes of this RcaRCAResult.  # noqa: E501
-        :type: list[RcaFeatureCause]
+        :param users: The users of this RimeListUsersResponse.  # noqa: E501
+        :type: list[UserUserDetail]
         """
 
-        self._feature_causes = feature_causes
+        self._users = users
 
     @property
-    def description(self):
-        """Gets the description of this RcaRCAResult.  # noqa: E501
+    def next_page_token(self):
+        """Gets the next_page_token of this RimeListUsersResponse.  # noqa: E501
 
 
-        :return: The description of this RcaRCAResult.  # noqa: E501
+        :return: The next_page_token of this RimeListUsersResponse.  # noqa: E501
         :rtype: str
         """
-        return self._description
+        return self._next_page_token
 
-    @description.setter
-    def description(self, description):
-        """Sets the description of this RcaRCAResult.
+    @next_page_token.setter
+    def next_page_token(self, next_page_token):
+        """Sets the next_page_token of this RimeListUsersResponse.
 
 
-        :param description: The description of this RcaRCAResult.  # noqa: E501
+        :param next_page_token: The next_page_token of this RimeListUsersResponse.  # noqa: E501
         :type: str
         """
 
-        self._description = description
+        self._next_page_token = next_page_token
 
     @property
-    def description_html(self):
-        """Gets the description_html of this RcaRCAResult.  # noqa: E501
+    def has_more(self):
+        """Gets the has_more of this RimeListUsersResponse.  # noqa: E501
 
 
-        :return: The description_html of this RcaRCAResult.  # noqa: E501
-        :rtype: str
+        :return: The has_more of this RimeListUsersResponse.  # noqa: E501
+        :rtype: bool
         """
-        return self._description_html
+        return self._has_more
 
-    @description_html.setter
-    def description_html(self, description_html):
-        """Sets the description_html of this RcaRCAResult.
+    @has_more.setter
+    def has_more(self, has_more):
+        """Sets the has_more of this RimeListUsersResponse.
 
 
-        :param description_html: The description_html of this RcaRCAResult.  # noqa: E501
-        :type: str
+        :param has_more: The has_more of this RimeListUsersResponse.  # noqa: E501
+        :type: bool
         """
 
-        self._description_html = description_html
+        self._has_more = has_more
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -134,15 +132,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RcaRCAResult, dict):
+        if issubclass(RimeListUsersResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -150,15 +148,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RcaRCAResult):
+        if not isinstance(other, RimeListUsersResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rca_rca_role.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_users_request_query.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,43 +11,34 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RcaRCARole(object):
+class RimeListUsersRequestQuery(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
-
-    """
-    allowed enum values
-    """
-    UNSPECIFIED = "RCAROLE_UNSPECIFIED"
-    EFFECT = "RCAROLE_EFFECT"
-    FEATURE_CAUSE = "RCAROLE_FEATURE_CAUSE"
-    TEST_CAUSE = "RCAROLE_TEST_CAUSE"
-    EXCLUDED = "RCAROLE_EXCLUDED"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """RcaRCARole - a model defined in Swagger"""  # noqa: E501
+        """RimeListUsersRequestQuery - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -63,15 +54,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RcaRCARole, dict):
+        if issubclass(RimeListUsersRequestQuery, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -79,15 +70,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RcaRCARole):
+        if not isinstance(other, RimeListUsersRequestQuery):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rca_test_case_cause.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_users_of_workspace_response.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,167 +11,139 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RcaTestCaseCause(object):
+class RimeListUsersOfWorkspaceResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'test_case_id': 'RcaTestCaseID',
-        'description': 'str',
-        'description_html': 'str',
-        'confidence_score': 'float',
-        'monitor_id': 'RimeUUID'
+        'workspace_id': 'RimeUUID',
+        'users': 'list[RimeUserDetailWithRole]',
+        'next_page_token': 'str',
+        'has_more': 'bool'
     }
 
     attribute_map = {
-        'test_case_id': 'testCaseId',
-        'description': 'description',
-        'description_html': 'descriptionHtml',
-        'confidence_score': 'confidenceScore',
-        'monitor_id': 'monitorId'
+        'workspace_id': 'workspaceId',
+        'users': 'users',
+        'next_page_token': 'nextPageToken',
+        'has_more': 'hasMore'
     }
 
-    def __init__(self, test_case_id=None, description=None, description_html=None, confidence_score=None, monitor_id=None):  # noqa: E501
-        """RcaTestCaseCause - a model defined in Swagger"""  # noqa: E501
-        self._test_case_id = None
-        self._description = None
-        self._description_html = None
-        self._confidence_score = None
-        self._monitor_id = None
+    def __init__(self, workspace_id=None, users=None, next_page_token=None, has_more=None):  # noqa: E501
+        """RimeListUsersOfWorkspaceResponse - a model defined in Swagger"""  # noqa: E501
+        self._workspace_id = None
+        self._users = None
+        self._next_page_token = None
+        self._has_more = None
         self.discriminator = None
-        if test_case_id is not None:
-            self.test_case_id = test_case_id
-        if description is not None:
-            self.description = description
-        if description_html is not None:
-            self.description_html = description_html
-        if confidence_score is not None:
-            self.confidence_score = confidence_score
-        if monitor_id is not None:
-            self.monitor_id = monitor_id
+        if workspace_id is not None:
+            self.workspace_id = workspace_id
+        if users is not None:
+            self.users = users
+        if next_page_token is not None:
+            self.next_page_token = next_page_token
+        if has_more is not None:
+            self.has_more = has_more
 
     @property
-    def test_case_id(self):
-        """Gets the test_case_id of this RcaTestCaseCause.  # noqa: E501
+    def workspace_id(self):
+        """Gets the workspace_id of this RimeListUsersOfWorkspaceResponse.  # noqa: E501
 
 
-        :return: The test_case_id of this RcaTestCaseCause.  # noqa: E501
-        :rtype: RcaTestCaseID
+        :return: The workspace_id of this RimeListUsersOfWorkspaceResponse.  # noqa: E501
+        :rtype: RimeUUID
         """
-        return self._test_case_id
+        return self._workspace_id
 
-    @test_case_id.setter
-    def test_case_id(self, test_case_id):
-        """Sets the test_case_id of this RcaTestCaseCause.
+    @workspace_id.setter
+    def workspace_id(self, workspace_id):
+        """Sets the workspace_id of this RimeListUsersOfWorkspaceResponse.
 
 
-        :param test_case_id: The test_case_id of this RcaTestCaseCause.  # noqa: E501
-        :type: RcaTestCaseID
+        :param workspace_id: The workspace_id of this RimeListUsersOfWorkspaceResponse.  # noqa: E501
+        :type: RimeUUID
         """
 
-        self._test_case_id = test_case_id
+        self._workspace_id = workspace_id
 
     @property
-    def description(self):
-        """Gets the description of this RcaTestCaseCause.  # noqa: E501
+    def users(self):
+        """Gets the users of this RimeListUsersOfWorkspaceResponse.  # noqa: E501
 
 
-        :return: The description of this RcaTestCaseCause.  # noqa: E501
-        :rtype: str
+        :return: The users of this RimeListUsersOfWorkspaceResponse.  # noqa: E501
+        :rtype: list[RimeUserDetailWithRole]
         """
-        return self._description
+        return self._users
 
-    @description.setter
-    def description(self, description):
-        """Sets the description of this RcaTestCaseCause.
+    @users.setter
+    def users(self, users):
+        """Sets the users of this RimeListUsersOfWorkspaceResponse.
 
 
-        :param description: The description of this RcaTestCaseCause.  # noqa: E501
-        :type: str
+        :param users: The users of this RimeListUsersOfWorkspaceResponse.  # noqa: E501
+        :type: list[RimeUserDetailWithRole]
         """
 
-        self._description = description
+        self._users = users
 
     @property
-    def description_html(self):
-        """Gets the description_html of this RcaTestCaseCause.  # noqa: E501
+    def next_page_token(self):
+        """Gets the next_page_token of this RimeListUsersOfWorkspaceResponse.  # noqa: E501
 
 
-        :return: The description_html of this RcaTestCaseCause.  # noqa: E501
+        :return: The next_page_token of this RimeListUsersOfWorkspaceResponse.  # noqa: E501
         :rtype: str
         """
-        return self._description_html
+        return self._next_page_token
 
-    @description_html.setter
-    def description_html(self, description_html):
-        """Sets the description_html of this RcaTestCaseCause.
+    @next_page_token.setter
+    def next_page_token(self, next_page_token):
+        """Sets the next_page_token of this RimeListUsersOfWorkspaceResponse.
 
 
-        :param description_html: The description_html of this RcaTestCaseCause.  # noqa: E501
+        :param next_page_token: The next_page_token of this RimeListUsersOfWorkspaceResponse.  # noqa: E501
         :type: str
         """
 
-        self._description_html = description_html
-
-    @property
-    def confidence_score(self):
-        """Gets the confidence_score of this RcaTestCaseCause.  # noqa: E501
-
-        Confidence that TestCaseCause explains the issue with the feature. Used to rank TestCaseCauses. In range [0,1].  # noqa: E501
-
-        :return: The confidence_score of this RcaTestCaseCause.  # noqa: E501
-        :rtype: float
-        """
-        return self._confidence_score
-
-    @confidence_score.setter
-    def confidence_score(self, confidence_score):
-        """Sets the confidence_score of this RcaTestCaseCause.
-
-        Confidence that TestCaseCause explains the issue with the feature. Used to rank TestCaseCauses. In range [0,1].  # noqa: E501
-
-        :param confidence_score: The confidence_score of this RcaTestCaseCause.  # noqa: E501
-        :type: float
-        """
-
-        self._confidence_score = confidence_score
+        self._next_page_token = next_page_token
 
     @property
-    def monitor_id(self):
-        """Gets the monitor_id of this RcaTestCaseCause.  # noqa: E501
+    def has_more(self):
+        """Gets the has_more of this RimeListUsersOfWorkspaceResponse.  # noqa: E501
 
 
-        :return: The monitor_id of this RcaTestCaseCause.  # noqa: E501
-        :rtype: RimeUUID
+        :return: The has_more of this RimeListUsersOfWorkspaceResponse.  # noqa: E501
+        :rtype: bool
         """
-        return self._monitor_id
+        return self._has_more
 
-    @monitor_id.setter
-    def monitor_id(self, monitor_id):
-        """Sets the monitor_id of this RcaTestCaseCause.
+    @has_more.setter
+    def has_more(self, has_more):
+        """Sets the has_more of this RimeListUsersOfWorkspaceResponse.
 
 
-        :param monitor_id: The monitor_id of this RcaTestCaseCause.  # noqa: E501
-        :type: RimeUUID
+        :param has_more: The has_more of this RimeListUsersOfWorkspaceResponse.  # noqa: E501
+        :type: bool
         """
 
-        self._monitor_id = monitor_id
+        self._has_more = has_more
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -186,15 +158,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RcaTestCaseCause, dict):
+        if issubclass(RimeListUsersOfWorkspaceResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -202,15 +174,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RcaTestCaseCause):
+        if not isinstance(other, RimeListUsersOfWorkspaceResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rca_test_case_id.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_agent_response.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,89 +11,89 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RcaTestCaseID(object):
+class RimeCreateAgentResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'test_batch_type': 'str',
-        'test_feature_name': 'str'
+        'config': 'str',
+        'agent_id': 'RimeUUID'
     }
 
     attribute_map = {
-        'test_batch_type': 'testBatchType',
-        'test_feature_name': 'testFeatureName'
+        'config': 'config',
+        'agent_id': 'agentId'
     }
 
-    def __init__(self, test_batch_type=None, test_feature_name=None):  # noqa: E501
-        """RcaTestCaseID - a model defined in Swagger"""  # noqa: E501
-        self._test_batch_type = None
-        self._test_feature_name = None
+    def __init__(self, config=None, agent_id=None):  # noqa: E501
+        """RimeCreateAgentResponse - a model defined in Swagger"""  # noqa: E501
+        self._config = None
+        self._agent_id = None
         self.discriminator = None
-        if test_batch_type is not None:
-            self.test_batch_type = test_batch_type
-        if test_feature_name is not None:
-            self.test_feature_name = test_feature_name
+        if config is not None:
+            self.config = config
+        if agent_id is not None:
+            self.agent_id = agent_id
 
     @property
-    def test_batch_type(self):
-        """Gets the test_batch_type of this RcaTestCaseID.  # noqa: E501
+    def config(self):
+        """Gets the config of this RimeCreateAgentResponse.  # noqa: E501
 
+        File that contains configuration values for installing the agent.  # noqa: E501
 
-        :return: The test_batch_type of this RcaTestCaseID.  # noqa: E501
+        :return: The config of this RimeCreateAgentResponse.  # noqa: E501
         :rtype: str
         """
-        return self._test_batch_type
+        return self._config
 
-    @test_batch_type.setter
-    def test_batch_type(self, test_batch_type):
-        """Sets the test_batch_type of this RcaTestCaseID.
+    @config.setter
+    def config(self, config):
+        """Sets the config of this RimeCreateAgentResponse.
 
+        File that contains configuration values for installing the agent.  # noqa: E501
 
-        :param test_batch_type: The test_batch_type of this RcaTestCaseID.  # noqa: E501
+        :param config: The config of this RimeCreateAgentResponse.  # noqa: E501
         :type: str
         """
 
-        self._test_batch_type = test_batch_type
+        self._config = config
 
     @property
-    def test_feature_name(self):
-        """Gets the test_feature_name of this RcaTestCaseID.  # noqa: E501
+    def agent_id(self):
+        """Gets the agent_id of this RimeCreateAgentResponse.  # noqa: E501
 
-        Can be empty string if no feature associated with this test case.  # noqa: E501
 
-        :return: The test_feature_name of this RcaTestCaseID.  # noqa: E501
-        :rtype: str
+        :return: The agent_id of this RimeCreateAgentResponse.  # noqa: E501
+        :rtype: RimeUUID
         """
-        return self._test_feature_name
+        return self._agent_id
 
-    @test_feature_name.setter
-    def test_feature_name(self, test_feature_name):
-        """Sets the test_feature_name of this RcaTestCaseID.
+    @agent_id.setter
+    def agent_id(self, agent_id):
+        """Sets the agent_id of this RimeCreateAgentResponse.
 
-        Can be empty string if no feature associated with this test case.  # noqa: E501
 
-        :param test_feature_name: The test_feature_name of this RcaTestCaseID.  # noqa: E501
-        :type: str
+        :param agent_id: The agent_id of this RimeCreateAgentResponse.  # noqa: E501
+        :type: RimeUUID
         """
 
-        self._test_feature_name = test_feature_name
+        self._agent_id = agent_id
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -108,15 +108,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RcaTestCaseID, dict):
+        if issubclass(RimeCreateAgentResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -124,15 +124,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RcaTestCaseID):
+        if not isinstance(other, RimeCreateAgentResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/registry_connection_info.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_connection_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/registry_data_collector_info.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_data_collector_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/registry_data_file_info.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_data_file_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/registry_data_info.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_data_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/registry_data_loading_info.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_data_loading_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,26 +50,26 @@
         if loader_kwargs_json is not None:
             self.loader_kwargs_json = loader_kwargs_json
 
     @property
     def path(self):
         """Gets the path of this RegistryDataLoadingInfo.  # noqa: E501
 
-        The path to the data file.  # noqa: E501
+        The path to the python file containing the data loading function.  # noqa: E501
 
         :return: The path of this RegistryDataLoadingInfo.  # noqa: E501
         :rtype: str
         """
         return self._path
 
     @path.setter
     def path(self, path):
         """Sets the path of this RegistryDataLoadingInfo.
 
-        The path to the data file.  # noqa: E501
+        The path to the python file containing the data loading function.  # noqa: E501
 
         :param path: The path of this RegistryDataLoadingInfo.  # noqa: E501
         :type: str
         """
         if path is None:
             raise ValueError("Invalid value for `path`, must not be `None`")  # noqa: E501
```

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/registry_data_params.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_data_params.py`

 * *Files 2% similar despite different names*

```diff
@@ -491,26 +491,26 @@
 
         self._feature_type_path = feature_type_path
 
     @property
     def image_load_path(self):
         """Gets the image_load_path of this RegistryDataParams.  # noqa: E501
 
-        Path to a CSV file that contains images to load for image_features.  # noqa: E501
+        Path to a python file containing a custom function for loading images in the dataset.  # noqa: E501
 
         :return: The image_load_path of this RegistryDataParams.  # noqa: E501
         :rtype: str
         """
         return self._image_load_path
 
     @image_load_path.setter
     def image_load_path(self, image_load_path):
         """Sets the image_load_path of this RegistryDataParams.
 
-        Path to a CSV file that contains images to load for image_features.  # noqa: E501
+        Path to a python file containing a custom function for loading images in the dataset.  # noqa: E501
 
         :param image_load_path: The image_load_path of this RegistryDataParams.  # noqa: E501
         :type: str
         """
 
         self._image_load_path = image_load_path
```

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/registry_data_type.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_data_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/registry_databricks_info.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_databricks_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/registry_hugging_face_data_info.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_hugging_face_data_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/registry_hugging_face_model_info.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_hugging_face_model_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/registry_metadata.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_metadata.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/registry_model_info.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_model_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/registry_model_path_info.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_model_path_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/registry_pred_info.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_pred_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/registry_prediction_params.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_prediction_params.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/registry_validity_status.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_validity_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/registryprediction_prediction.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registryprediction_prediction.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,16 +45,15 @@
         self._old_password = None
         self._new_password = None
         self.discriminator = None
         if user_id is not None:
             self.user_id = user_id
         if old_password is not None:
             self.old_password = old_password
-        if new_password is not None:
-            self.new_password = new_password
+        self.new_password = new_password
 
     @property
     def user_id(self):
         """Gets the user_id of this ResetpasswordUserIdUuidBody.  # noqa: E501
 
         Unique ID of an object in RIME.  # noqa: E501
 
@@ -110,14 +109,16 @@
     def new_password(self, new_password):
         """Sets the new_password of this ResetpasswordUserIdUuidBody.
 
 
         :param new_password: The new_password of this ResetpasswordUserIdUuidBody.  # noqa: E501
         :type: str
         """
+        if new_password is None:
+            raise ValueError("Invalid value for `new_password`, must not be `None`")  # noqa: E501
 
         self._new_password = new_password
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_actor_role.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_actor_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_agent.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_agent.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_agent_status.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_agent_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_api_token_info.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_api_token_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_category_metric.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_category_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_category_test_result.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_category_test_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_config_type.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_config_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_configure_integration_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_configure_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_continuous_test_run_progress.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_continuous_test_run_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_agent_request.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_agent_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_agent_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_image_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,89 +11,87 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeCreateAgentResponse(object):
+class RimeCreateImageResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'config': 'str',
-        'agent_id': 'RimeUUID'
+        'image': 'RimeManagedImage',
+        'job': 'RimeJobMetadata'
     }
 
     attribute_map = {
-        'config': 'config',
-        'agent_id': 'agentId'
+        'image': 'image',
+        'job': 'job'
     }
 
-    def __init__(self, config=None, agent_id=None):  # noqa: E501
-        """RimeCreateAgentResponse - a model defined in Swagger"""  # noqa: E501
-        self._config = None
-        self._agent_id = None
+    def __init__(self, image=None, job=None):  # noqa: E501
+        """RimeCreateImageResponse - a model defined in Swagger"""  # noqa: E501
+        self._image = None
+        self._job = None
         self.discriminator = None
-        if config is not None:
-            self.config = config
-        if agent_id is not None:
-            self.agent_id = agent_id
+        if image is not None:
+            self.image = image
+        if job is not None:
+            self.job = job
 
     @property
-    def config(self):
-        """Gets the config of this RimeCreateAgentResponse.  # noqa: E501
+    def image(self):
+        """Gets the image of this RimeCreateImageResponse.  # noqa: E501
 
-        File that contains configuration values for installing the agent.  # noqa: E501
 
-        :return: The config of this RimeCreateAgentResponse.  # noqa: E501
-        :rtype: str
+        :return: The image of this RimeCreateImageResponse.  # noqa: E501
+        :rtype: RimeManagedImage
         """
-        return self._config
+        return self._image
 
-    @config.setter
-    def config(self, config):
-        """Sets the config of this RimeCreateAgentResponse.
+    @image.setter
+    def image(self, image):
+        """Sets the image of this RimeCreateImageResponse.
 
-        File that contains configuration values for installing the agent.  # noqa: E501
 
-        :param config: The config of this RimeCreateAgentResponse.  # noqa: E501
-        :type: str
+        :param image: The image of this RimeCreateImageResponse.  # noqa: E501
+        :type: RimeManagedImage
         """
 
-        self._config = config
+        self._image = image
 
     @property
-    def agent_id(self):
-        """Gets the agent_id of this RimeCreateAgentResponse.  # noqa: E501
+    def job(self):
+        """Gets the job of this RimeCreateImageResponse.  # noqa: E501
 
 
-        :return: The agent_id of this RimeCreateAgentResponse.  # noqa: E501
-        :rtype: RimeUUID
+        :return: The job of this RimeCreateImageResponse.  # noqa: E501
+        :rtype: RimeJobMetadata
         """
-        return self._agent_id
+        return self._job
 
-    @agent_id.setter
-    def agent_id(self, agent_id):
-        """Sets the agent_id of this RimeCreateAgentResponse.
+    @job.setter
+    def job(self, job):
+        """Sets the job of this RimeCreateImageResponse.
 
 
-        :param agent_id: The agent_id of this RimeCreateAgentResponse.  # noqa: E501
-        :type: RimeUUID
+        :param job: The job of this RimeCreateImageResponse.  # noqa: E501
+        :type: RimeJobMetadata
         """
 
-        self._agent_id = agent_id
+        self._job = job
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -108,15 +106,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeCreateAgentResponse, dict):
+        if issubclass(RimeCreateImageResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -124,15 +122,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeCreateAgentResponse):
+        if not isinstance(other, RimeCreateImageResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_api_token_request.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_api_token_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,16 +44,15 @@
     def __init__(self, name=None, workspace_id=None, token_type=None, agent_id=None):  # noqa: E501
         """RimeCreateAPITokenRequest - a model defined in Swagger"""  # noqa: E501
         self._name = None
         self._workspace_id = None
         self._token_type = None
         self._agent_id = None
         self.discriminator = None
-        if name is not None:
-            self.name = name
+        self.name = name
         if workspace_id is not None:
             self.workspace_id = workspace_id
         if token_type is not None:
             self.token_type = token_type
         if agent_id is not None:
             self.agent_id = agent_id
 
@@ -73,14 +72,16 @@
         """Sets the name of this RimeCreateAPITokenRequest.
 
         Name of the API token.  # noqa: E501
 
         :param name: The name of this RimeCreateAPITokenRequest.  # noqa: E501
         :type: str
         """
+        if name is None:
+            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
 
         self._name = name
 
     @property
     def workspace_id(self):
         """Gets the workspace_id of this RimeCreateAPITokenRequest.  # noqa: E501
```

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_api_token_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_api_token_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_request.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_image_request.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_image_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_image_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_sync_image_tag_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeCreateImageResponse(object):
+class RimeSyncImageTagResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -34,60 +34,60 @@
 
     attribute_map = {
         'image': 'image',
         'job': 'job'
     }
 
     def __init__(self, image=None, job=None):  # noqa: E501
-        """RimeCreateImageResponse - a model defined in Swagger"""  # noqa: E501
+        """RimeSyncImageTagResponse - a model defined in Swagger"""  # noqa: E501
         self._image = None
         self._job = None
         self.discriminator = None
         if image is not None:
             self.image = image
         if job is not None:
             self.job = job
 
     @property
     def image(self):
-        """Gets the image of this RimeCreateImageResponse.  # noqa: E501
+        """Gets the image of this RimeSyncImageTagResponse.  # noqa: E501
 
 
-        :return: The image of this RimeCreateImageResponse.  # noqa: E501
+        :return: The image of this RimeSyncImageTagResponse.  # noqa: E501
         :rtype: RimeManagedImage
         """
         return self._image
 
     @image.setter
     def image(self, image):
-        """Sets the image of this RimeCreateImageResponse.
+        """Sets the image of this RimeSyncImageTagResponse.
 
 
-        :param image: The image of this RimeCreateImageResponse.  # noqa: E501
+        :param image: The image of this RimeSyncImageTagResponse.  # noqa: E501
         :type: RimeManagedImage
         """
 
         self._image = image
 
     @property
     def job(self):
-        """Gets the job of this RimeCreateImageResponse.  # noqa: E501
+        """Gets the job of this RimeSyncImageTagResponse.  # noqa: E501
 
 
-        :return: The job of this RimeCreateImageResponse.  # noqa: E501
+        :return: The job of this RimeSyncImageTagResponse.  # noqa: E501
         :rtype: RimeJobMetadata
         """
         return self._job
 
     @job.setter
     def job(self, job):
-        """Sets the job of this RimeCreateImageResponse.
+        """Sets the job of this RimeSyncImageTagResponse.
 
 
-        :param job: The job of this RimeCreateImageResponse.  # noqa: E501
+        :param job: The job of this RimeSyncImageTagResponse.  # noqa: E501
         :type: RimeJobMetadata
         """
 
         self._job = job
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -106,15 +106,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeCreateImageResponse, dict):
+        if issubclass(RimeSyncImageTagResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -122,15 +122,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeCreateImageResponse):
+        if not isinstance(other, RimeSyncImageTagResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_model_card_request.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_model_card_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_model_card_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_model_card_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_notification_request.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_notification_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,16 +49,15 @@
         self._object_id = None
         self._emails = None
         self._config = None
         self._webhooks = None
         self.discriminator = None
         if object_type is not None:
             self.object_type = object_type
-        if object_id is not None:
-            self.object_id = object_id
+        self.object_id = object_id
         if emails is not None:
             self.emails = emails
         if config is not None:
             self.config = config
         if webhooks is not None:
             self.webhooks = webhooks
 
@@ -99,14 +98,16 @@
         """Sets the object_id of this RimeCreateNotificationRequest.
 
         Uniquely specifies an object for the notification. This varies depending on the object type; for Projects, this should be the unique identifier of the project.  # noqa: E501
 
         :param object_id: The object_id of this RimeCreateNotificationRequest.  # noqa: E501
         :type: str
         """
+        if object_id is None:
+            raise ValueError("Invalid value for `object_id`, must not be `None`")  # noqa: E501
 
         self._object_id = object_id
 
     @property
     def emails(self):
         """Gets the emails of this RimeCreateNotificationRequest.  # noqa: E501
```

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_notification_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_notification_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_user_request.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_user_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,20 +44,17 @@
     def __init__(self, email=None, password=None, full_name=None, org_role=None):  # noqa: E501
         """RimeCreateUserRequest - a model defined in Swagger"""  # noqa: E501
         self._email = None
         self._password = None
         self._full_name = None
         self._org_role = None
         self.discriminator = None
-        if email is not None:
-            self.email = email
-        if password is not None:
-            self.password = password
-        if full_name is not None:
-            self.full_name = full_name
+        self.email = email
+        self.password = password
+        self.full_name = full_name
         if org_role is not None:
             self.org_role = org_role
 
     @property
     def email(self):
         """Gets the email of this RimeCreateUserRequest.  # noqa: E501
 
@@ -73,14 +70,16 @@
         """Sets the email of this RimeCreateUserRequest.
 
         The email address of the user.  # noqa: E501
 
         :param email: The email of this RimeCreateUserRequest.  # noqa: E501
         :type: str
         """
+        if email is None:
+            raise ValueError("Invalid value for `email`, must not be `None`")  # noqa: E501
 
         self._email = email
 
     @property
     def password(self):
         """Gets the password of this RimeCreateUserRequest.  # noqa: E501
 
@@ -96,14 +95,16 @@
         """Sets the password of this RimeCreateUserRequest.
 
         The password of the user. This password will be changed on the first login.  # noqa: E501
 
         :param password: The password of this RimeCreateUserRequest.  # noqa: E501
         :type: str
         """
+        if password is None:
+            raise ValueError("Invalid value for `password`, must not be `None`")  # noqa: E501
 
         self._password = password
 
     @property
     def full_name(self):
         """Gets the full_name of this RimeCreateUserRequest.  # noqa: E501
 
@@ -119,14 +120,16 @@
         """Sets the full_name of this RimeCreateUserRequest.
 
         The full name of the user.  # noqa: E501
 
         :param full_name: The full_name of this RimeCreateUserRequest.  # noqa: E501
         :type: str
         """
+        if full_name is None:
+            raise ValueError("Invalid value for `full_name`, must not be `None`")  # noqa: E501
 
         self._full_name = full_name
 
     @property
     def org_role(self):
         """Gets the org_role of this RimeCreateUserRequest.  # noqa: E501
```

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_user_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_user_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_workspace_request.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_workspace_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_workspace_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_deactivate_agent_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_deactivate_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_delete_agent_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_delete_custom_monitor_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_custom_monitor_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_delete_dataset_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_dataset_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_delete_firewall_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_firewall_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_delete_image_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_image_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_delete_integration_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_delete_model_card_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_model_card_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_delete_model_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_model_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_delete_prediction_set_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_prediction_set_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_delete_uploaded_file_url_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_uploaded_file_url_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_failing_row.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_failing_row.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_feature_flags.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_feature_flags.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_feature_type.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_feature_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_float_list.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_float_list.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_customer_managed_key_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_customer_managed_key_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_feature_flag_jwt_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_feature_flag_jwt_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_feature_flags_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_feature_flags_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_firewall_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_firewall_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_image_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_image_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_integration_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_job_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_job_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_key_status_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_key_status_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_latest_logs_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_latest_logs_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_limit_status_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_limit_status_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_model_card_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_model_card_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_model_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_model_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_monitor_result_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_monitor_result_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_prediction_set_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_prediction_set_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_predictions_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_predictions_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_project_id_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_project_id_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_rime_info_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_rime_info_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_test_run_id_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_test_run_id_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_url_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_url_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_user_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_user_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_validate_dataset_task_status_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_validate_dataset_task_status_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_validate_model_task_status_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_validate_model_task_status_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_validate_predictions_task_status_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_validate_predictions_task_status_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_workspace_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_heartbeat_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_heartbeat_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_image_reference.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_image_reference.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_int_list.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_int_list.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_integration_info.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_integration_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_job_data.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_job_data.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_job_metadata.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_job_metadata.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_job_type.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_job_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_job_view.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_job_view.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_language.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_language.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_license_feature.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_license_feature.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_license_limit.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_license_limit.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_limit_status.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_limit_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_limit_status_status.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_limit_status_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_agents_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_agents_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_api_tokens_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_api_tokens_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_datasets_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_datasets_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_request_query.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_enabled_features_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_enabled_features_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_file_scan_results_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_file_scan_results_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_images_request.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_images_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_images_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_images_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_request_query.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_models_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_models_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_monitors_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_monitors_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_notifications_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_notifications_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_prediction_sets_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_prediction_sets_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_project_tags_in_workspace_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_project_tags_in_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_uploaded_file_urls_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_uploaded_file_urls_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_users_of_workspace_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_user_role.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,139 +11,139 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeListUsersOfWorkspaceResponse(object):
+class RimeUserRole(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'workspace_id': 'RimeUUID',
-        'users': 'list[RimeUserDetailWithRole]',
-        'next_page_token': 'str',
-        'has_more': 'bool'
+        'subject_type': 'RimeSubjectType',
+        'subject_id': 'str',
+        'role': 'RimeActorRole',
+        'implicit_grant': 'bool'
     }
 
     attribute_map = {
-        'workspace_id': 'workspaceId',
-        'users': 'users',
-        'next_page_token': 'nextPageToken',
-        'has_more': 'hasMore'
+        'subject_type': 'subjectType',
+        'subject_id': 'subjectId',
+        'role': 'role',
+        'implicit_grant': 'implicitGrant'
     }
 
-    def __init__(self, workspace_id=None, users=None, next_page_token=None, has_more=None):  # noqa: E501
-        """RimeListUsersOfWorkspaceResponse - a model defined in Swagger"""  # noqa: E501
-        self._workspace_id = None
-        self._users = None
-        self._next_page_token = None
-        self._has_more = None
+    def __init__(self, subject_type=None, subject_id=None, role=None, implicit_grant=None):  # noqa: E501
+        """RimeUserRole - a model defined in Swagger"""  # noqa: E501
+        self._subject_type = None
+        self._subject_id = None
+        self._role = None
+        self._implicit_grant = None
         self.discriminator = None
-        if workspace_id is not None:
-            self.workspace_id = workspace_id
-        if users is not None:
-            self.users = users
-        if next_page_token is not None:
-            self.next_page_token = next_page_token
-        if has_more is not None:
-            self.has_more = has_more
+        if subject_type is not None:
+            self.subject_type = subject_type
+        if subject_id is not None:
+            self.subject_id = subject_id
+        if role is not None:
+            self.role = role
+        if implicit_grant is not None:
+            self.implicit_grant = implicit_grant
 
     @property
-    def workspace_id(self):
-        """Gets the workspace_id of this RimeListUsersOfWorkspaceResponse.  # noqa: E501
+    def subject_type(self):
+        """Gets the subject_type of this RimeUserRole.  # noqa: E501
 
 
-        :return: The workspace_id of this RimeListUsersOfWorkspaceResponse.  # noqa: E501
-        :rtype: RimeUUID
+        :return: The subject_type of this RimeUserRole.  # noqa: E501
+        :rtype: RimeSubjectType
         """
-        return self._workspace_id
+        return self._subject_type
 
-    @workspace_id.setter
-    def workspace_id(self, workspace_id):
-        """Sets the workspace_id of this RimeListUsersOfWorkspaceResponse.
+    @subject_type.setter
+    def subject_type(self, subject_type):
+        """Sets the subject_type of this RimeUserRole.
 
 
-        :param workspace_id: The workspace_id of this RimeListUsersOfWorkspaceResponse.  # noqa: E501
-        :type: RimeUUID
+        :param subject_type: The subject_type of this RimeUserRole.  # noqa: E501
+        :type: RimeSubjectType
         """
 
-        self._workspace_id = workspace_id
+        self._subject_type = subject_type
 
     @property
-    def users(self):
-        """Gets the users of this RimeListUsersOfWorkspaceResponse.  # noqa: E501
+    def subject_id(self):
+        """Gets the subject_id of this RimeUserRole.  # noqa: E501
 
 
-        :return: The users of this RimeListUsersOfWorkspaceResponse.  # noqa: E501
-        :rtype: list[RimeUserDetailWithRole]
+        :return: The subject_id of this RimeUserRole.  # noqa: E501
+        :rtype: str
         """
-        return self._users
+        return self._subject_id
 
-    @users.setter
-    def users(self, users):
-        """Sets the users of this RimeListUsersOfWorkspaceResponse.
+    @subject_id.setter
+    def subject_id(self, subject_id):
+        """Sets the subject_id of this RimeUserRole.
 
 
-        :param users: The users of this RimeListUsersOfWorkspaceResponse.  # noqa: E501
-        :type: list[RimeUserDetailWithRole]
+        :param subject_id: The subject_id of this RimeUserRole.  # noqa: E501
+        :type: str
         """
 
-        self._users = users
+        self._subject_id = subject_id
 
     @property
-    def next_page_token(self):
-        """Gets the next_page_token of this RimeListUsersOfWorkspaceResponse.  # noqa: E501
+    def role(self):
+        """Gets the role of this RimeUserRole.  # noqa: E501
 
 
-        :return: The next_page_token of this RimeListUsersOfWorkspaceResponse.  # noqa: E501
-        :rtype: str
+        :return: The role of this RimeUserRole.  # noqa: E501
+        :rtype: RimeActorRole
         """
-        return self._next_page_token
+        return self._role
 
-    @next_page_token.setter
-    def next_page_token(self, next_page_token):
-        """Sets the next_page_token of this RimeListUsersOfWorkspaceResponse.
+    @role.setter
+    def role(self, role):
+        """Sets the role of this RimeUserRole.
 
 
-        :param next_page_token: The next_page_token of this RimeListUsersOfWorkspaceResponse.  # noqa: E501
-        :type: str
+        :param role: The role of this RimeUserRole.  # noqa: E501
+        :type: RimeActorRole
         """
 
-        self._next_page_token = next_page_token
+        self._role = role
 
     @property
-    def has_more(self):
-        """Gets the has_more of this RimeListUsersOfWorkspaceResponse.  # noqa: E501
+    def implicit_grant(self):
+        """Gets the implicit_grant of this RimeUserRole.  # noqa: E501
 
 
-        :return: The has_more of this RimeListUsersOfWorkspaceResponse.  # noqa: E501
+        :return: The implicit_grant of this RimeUserRole.  # noqa: E501
         :rtype: bool
         """
-        return self._has_more
+        return self._implicit_grant
 
-    @has_more.setter
-    def has_more(self, has_more):
-        """Sets the has_more of this RimeListUsersOfWorkspaceResponse.
+    @implicit_grant.setter
+    def implicit_grant(self, implicit_grant):
+        """Sets the implicit_grant of this RimeUserRole.
 
 
-        :param has_more: The has_more of this RimeListUsersOfWorkspaceResponse.  # noqa: E501
+        :param implicit_grant: The implicit_grant of this RimeUserRole.  # noqa: E501
         :type: bool
         """
 
-        self._has_more = has_more
+        self._implicit_grant = implicit_grant
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -158,15 +158,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeListUsersOfWorkspaceResponse, dict):
+        if issubclass(RimeUserRole, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -174,15 +174,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeListUsersOfWorkspaceResponse):
+        if not isinstance(other, RimeUserRole):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_users_request_query.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeListUsersRequestQuery(object):
+class RimeSendRIEmailResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -30,15 +30,15 @@
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """RimeListUsersRequestQuery - a model defined in Swagger"""  # noqa: E501
+        """RimeSendRIEmailResponse - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -54,15 +54,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeListUsersRequestQuery, dict):
+        if issubclass(RimeSendRIEmailResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -70,15 +70,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeListUsersRequestQuery):
+        if not isinstance(other, RimeSendRIEmailResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_users_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,113 +11,89 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeListUsersResponse(object):
+class TestrunTestRunIncrementalConfig(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'users': 'list[UserUserDetail]',
-        'next_page_token': 'str',
-        'has_more': 'bool'
+        'eval_dataset_id': 'str',
+        'run_time_info': 'RuntimeinfoRunTimeInfo'
     }
 
     attribute_map = {
-        'users': 'users',
-        'next_page_token': 'nextPageToken',
-        'has_more': 'hasMore'
+        'eval_dataset_id': 'evalDatasetId',
+        'run_time_info': 'runTimeInfo'
     }
 
-    def __init__(self, users=None, next_page_token=None, has_more=None):  # noqa: E501
-        """RimeListUsersResponse - a model defined in Swagger"""  # noqa: E501
-        self._users = None
-        self._next_page_token = None
-        self._has_more = None
+    def __init__(self, eval_dataset_id=None, run_time_info=None):  # noqa: E501
+        """TestrunTestRunIncrementalConfig - a model defined in Swagger"""  # noqa: E501
+        self._eval_dataset_id = None
+        self._run_time_info = None
         self.discriminator = None
-        if users is not None:
-            self.users = users
-        if next_page_token is not None:
-            self.next_page_token = next_page_token
-        if has_more is not None:
-            self.has_more = has_more
+        if eval_dataset_id is not None:
+            self.eval_dataset_id = eval_dataset_id
+        if run_time_info is not None:
+            self.run_time_info = run_time_info
 
     @property
-    def users(self):
-        """Gets the users of this RimeListUsersResponse.  # noqa: E501
+    def eval_dataset_id(self):
+        """Gets the eval_dataset_id of this TestrunTestRunIncrementalConfig.  # noqa: E501
 
+        Uniquely specifies an evaluation Dataset.  # noqa: E501
 
-        :return: The users of this RimeListUsersResponse.  # noqa: E501
-        :rtype: list[UserUserDetail]
-        """
-        return self._users
-
-    @users.setter
-    def users(self, users):
-        """Sets the users of this RimeListUsersResponse.
-
-
-        :param users: The users of this RimeListUsersResponse.  # noqa: E501
-        :type: list[UserUserDetail]
-        """
-
-        self._users = users
-
-    @property
-    def next_page_token(self):
-        """Gets the next_page_token of this RimeListUsersResponse.  # noqa: E501
-
-
-        :return: The next_page_token of this RimeListUsersResponse.  # noqa: E501
+        :return: The eval_dataset_id of this TestrunTestRunIncrementalConfig.  # noqa: E501
         :rtype: str
         """
-        return self._next_page_token
+        return self._eval_dataset_id
 
-    @next_page_token.setter
-    def next_page_token(self, next_page_token):
-        """Sets the next_page_token of this RimeListUsersResponse.
+    @eval_dataset_id.setter
+    def eval_dataset_id(self, eval_dataset_id):
+        """Sets the eval_dataset_id of this TestrunTestRunIncrementalConfig.
 
+        Uniquely specifies an evaluation Dataset.  # noqa: E501
 
-        :param next_page_token: The next_page_token of this RimeListUsersResponse.  # noqa: E501
+        :param eval_dataset_id: The eval_dataset_id of this TestrunTestRunIncrementalConfig.  # noqa: E501
         :type: str
         """
 
-        self._next_page_token = next_page_token
+        self._eval_dataset_id = eval_dataset_id
 
     @property
-    def has_more(self):
-        """Gets the has_more of this RimeListUsersResponse.  # noqa: E501
+    def run_time_info(self):
+        """Gets the run_time_info of this TestrunTestRunIncrementalConfig.  # noqa: E501
 
 
-        :return: The has_more of this RimeListUsersResponse.  # noqa: E501
-        :rtype: bool
+        :return: The run_time_info of this TestrunTestRunIncrementalConfig.  # noqa: E501
+        :rtype: RuntimeinfoRunTimeInfo
         """
-        return self._has_more
+        return self._run_time_info
 
-    @has_more.setter
-    def has_more(self, has_more):
-        """Sets the has_more of this RimeListUsersResponse.
+    @run_time_info.setter
+    def run_time_info(self, run_time_info):
+        """Sets the run_time_info of this TestrunTestRunIncrementalConfig.
 
 
-        :param has_more: The has_more of this RimeListUsersResponse.  # noqa: E501
-        :type: bool
+        :param run_time_info: The run_time_info of this TestrunTestRunIncrementalConfig.  # noqa: E501
+        :type: RuntimeinfoRunTimeInfo
         """
 
-        self._has_more = has_more
+        self._run_time_info = run_time_info
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -132,15 +108,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeListUsersResponse, dict):
+        if issubclass(TestrunTestRunIncrementalConfig, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -148,15 +124,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeListUsersResponse):
+        if not isinstance(other, TestrunTestRunIncrementalConfig):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_workspace_integrations_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_workspace_integrations_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_request_query.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_long_description_tab.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_long_description_tab.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_managed_image.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_managed_image.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_managed_image_status.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_managed_image_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_model_card.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_model_card.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_model_task.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_model_task.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_model_with_owner_details.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_model_with_owner_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_monitor_data_point.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_monitor_data_point.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_named_double.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_named_double.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_order.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_order.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_parent_role_subject_role_pair.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_parent_role_subject_role_pair.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_register_data_stream_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_register_data_stream_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_register_dataset_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_register_dataset_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_register_external_agent_request.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_register_external_agent_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_register_internal_agent_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_register_internal_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_register_model_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_register_model_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_register_prediction_set_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_register_prediction_set_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_remove_user_from_workspace_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_remove_user_from_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_reset_password_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_reset_password_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_resolve_detection_event_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_resolve_detection_event_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_ri_plan.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_ri_plan.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_safe_url.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_safe_url.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeSendRIEmailResponse(object):
+class RimeStorePredictionsResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -30,15 +30,15 @@
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """RimeSendRIEmailResponse - a model defined in Swagger"""  # noqa: E501
+        """RimeStorePredictionsResponse - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -54,15 +54,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeSendRIEmailResponse, dict):
+        if issubclass(RimeStorePredictionsResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -70,15 +70,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeSendRIEmailResponse):
+        if not isinstance(other, RimeStorePredictionsResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_severity.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_severity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_severity_counts.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_severity_counts.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_sort_spec.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_sort_spec.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_start_generative_stress_test_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_generative_stress_test_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_request.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_request.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_request.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_str_list.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,35 +11,61 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeStorePredictionsResponse(object):
+class RimeStrList(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
+        'values': 'list[str]'
     }
 
     attribute_map = {
+        'values': 'values'
     }
 
-    def __init__(self):  # noqa: E501
-        """RimeStorePredictionsResponse - a model defined in Swagger"""  # noqa: E501
+    def __init__(self, values=None):  # noqa: E501
+        """RimeStrList - a model defined in Swagger"""  # noqa: E501
+        self._values = None
         self.discriminator = None
+        if values is not None:
+            self.values = values
+
+    @property
+    def values(self):
+        """Gets the values of this RimeStrList.  # noqa: E501
+
+
+        :return: The values of this RimeStrList.  # noqa: E501
+        :rtype: list[str]
+        """
+        return self._values
+
+    @values.setter
+    def values(self, values):
+        """Sets the values of this RimeStrList.
+
+
+        :param values: The values of this RimeStrList.  # noqa: E501
+        :type: list[str]
+        """
+
+        self._values = values
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -54,15 +80,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeStorePredictionsResponse, dict):
+        if issubclass(RimeStrList, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -70,15 +96,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeStorePredictionsResponse):
+        if not isinstance(other, RimeStrList):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_str_list.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_test_type.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,61 +11,41 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeStrList(object):
+class RimeTestType(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
+
+    """
+    allowed enum values
+    """
+    STRESS_TESTING_UNSPECIFIED = "TEST_TYPE_STRESS_TESTING_UNSPECIFIED"
+    CONTINUOUS_TESTING = "TEST_TYPE_CONTINUOUS_TESTING"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'values': 'list[str]'
     }
 
     attribute_map = {
-        'values': 'values'
     }
 
-    def __init__(self, values=None):  # noqa: E501
-        """RimeStrList - a model defined in Swagger"""  # noqa: E501
-        self._values = None
+    def __init__(self):  # noqa: E501
+        """RimeTestType - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
-        if values is not None:
-            self.values = values
-
-    @property
-    def values(self):
-        """Gets the values of this RimeStrList.  # noqa: E501
-
-
-        :return: The values of this RimeStrList.  # noqa: E501
-        :rtype: list[str]
-        """
-        return self._values
-
-    @values.setter
-    def values(self, values):
-        """Sets the values of this RimeStrList.
-
-
-        :param values: The values of this RimeStrList.  # noqa: E501
-        :type: list[str]
-        """
-
-        self._values = values
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -80,15 +60,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeStrList, dict):
+        if issubclass(RimeTestType, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -96,15 +76,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeStrList):
+        if not isinstance(other, RimeTestType):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_subject_type.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_subject_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_suggestion.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_suggestion.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_sync_image_tag_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/validation_validate_predictions_response.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,87 +11,87 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeSyncImageTagResponse(object):
+class ValidationValidatePredictionsResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'image': 'RimeManagedImage',
-        'job': 'RimeJobMetadata'
+        'is_valid': 'bool',
+        'error_message': 'str'
     }
 
     attribute_map = {
-        'image': 'image',
-        'job': 'job'
+        'is_valid': 'isValid',
+        'error_message': 'errorMessage'
     }
 
-    def __init__(self, image=None, job=None):  # noqa: E501
-        """RimeSyncImageTagResponse - a model defined in Swagger"""  # noqa: E501
-        self._image = None
-        self._job = None
+    def __init__(self, is_valid=None, error_message=None):  # noqa: E501
+        """ValidationValidatePredictionsResponse - a model defined in Swagger"""  # noqa: E501
+        self._is_valid = None
+        self._error_message = None
         self.discriminator = None
-        if image is not None:
-            self.image = image
-        if job is not None:
-            self.job = job
+        if is_valid is not None:
+            self.is_valid = is_valid
+        if error_message is not None:
+            self.error_message = error_message
 
     @property
-    def image(self):
-        """Gets the image of this RimeSyncImageTagResponse.  # noqa: E501
+    def is_valid(self):
+        """Gets the is_valid of this ValidationValidatePredictionsResponse.  # noqa: E501
 
 
-        :return: The image of this RimeSyncImageTagResponse.  # noqa: E501
-        :rtype: RimeManagedImage
+        :return: The is_valid of this ValidationValidatePredictionsResponse.  # noqa: E501
+        :rtype: bool
         """
-        return self._image
+        return self._is_valid
 
-    @image.setter
-    def image(self, image):
-        """Sets the image of this RimeSyncImageTagResponse.
+    @is_valid.setter
+    def is_valid(self, is_valid):
+        """Sets the is_valid of this ValidationValidatePredictionsResponse.
 
 
-        :param image: The image of this RimeSyncImageTagResponse.  # noqa: E501
-        :type: RimeManagedImage
+        :param is_valid: The is_valid of this ValidationValidatePredictionsResponse.  # noqa: E501
+        :type: bool
         """
 
-        self._image = image
+        self._is_valid = is_valid
 
     @property
-    def job(self):
-        """Gets the job of this RimeSyncImageTagResponse.  # noqa: E501
+    def error_message(self):
+        """Gets the error_message of this ValidationValidatePredictionsResponse.  # noqa: E501
 
 
-        :return: The job of this RimeSyncImageTagResponse.  # noqa: E501
-        :rtype: RimeJobMetadata
+        :return: The error_message of this ValidationValidatePredictionsResponse.  # noqa: E501
+        :rtype: str
         """
-        return self._job
+        return self._error_message
 
-    @job.setter
-    def job(self, job):
-        """Sets the job of this RimeSyncImageTagResponse.
+    @error_message.setter
+    def error_message(self, error_message):
+        """Sets the error_message of this ValidationValidatePredictionsResponse.
 
 
-        :param job: The job of this RimeSyncImageTagResponse.  # noqa: E501
-        :type: RimeJobMetadata
+        :param error_message: The error_message of this ValidationValidatePredictionsResponse.  # noqa: E501
+        :type: str
         """
 
-        self._job = job
+        self._error_message = error_message
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -106,15 +106,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeSyncImageTagResponse, dict):
+        if issubclass(ValidationValidatePredictionsResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -122,15 +122,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeSyncImageTagResponse):
+        if not isinstance(other, ValidationValidatePredictionsResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_table_column.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_table_column.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_table_column_type.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_table_column_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_test_case_monitor_info.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_test_case_monitor_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,38 +26,33 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'threshold': 'MonitorThreshold',
         'is_subset_metric': 'bool',
-        'rca_role': 'RcaRCARole',
         'excluded_transforms': 'MonitorExcludedTransforms'
     }
 
     attribute_map = {
         'threshold': 'threshold',
         'is_subset_metric': 'isSubsetMetric',
-        'rca_role': 'rcaRole',
         'excluded_transforms': 'excludedTransforms'
     }
 
-    def __init__(self, threshold=None, is_subset_metric=None, rca_role=None, excluded_transforms=None):  # noqa: E501
+    def __init__(self, threshold=None, is_subset_metric=None, excluded_transforms=None):  # noqa: E501
         """RimeTestCaseMonitorInfo - a model defined in Swagger"""  # noqa: E501
         self._threshold = None
         self._is_subset_metric = None
-        self._rca_role = None
         self._excluded_transforms = None
         self.discriminator = None
         if threshold is not None:
             self.threshold = threshold
         if is_subset_metric is not None:
             self.is_subset_metric = is_subset_metric
-        if rca_role is not None:
-            self.rca_role = rca_role
         if excluded_transforms is not None:
             self.excluded_transforms = excluded_transforms
 
     @property
     def threshold(self):
         """Gets the threshold of this RimeTestCaseMonitorInfo.  # noqa: E501
 
@@ -96,35 +91,14 @@
         :param is_subset_metric: The is_subset_metric of this RimeTestCaseMonitorInfo.  # noqa: E501
         :type: bool
         """
 
         self._is_subset_metric = is_subset_metric
 
     @property
-    def rca_role(self):
-        """Gets the rca_role of this RimeTestCaseMonitorInfo.  # noqa: E501
-
-
-        :return: The rca_role of this RimeTestCaseMonitorInfo.  # noqa: E501
-        :rtype: RcaRCARole
-        """
-        return self._rca_role
-
-    @rca_role.setter
-    def rca_role(self, rca_role):
-        """Sets the rca_role of this RimeTestCaseMonitorInfo.
-
-
-        :param rca_role: The rca_role of this RimeTestCaseMonitorInfo.  # noqa: E501
-        :type: RcaRCARole
-        """
-
-        self._rca_role = rca_role
-
-    @property
     def excluded_transforms(self):
         """Gets the excluded_transforms of this RimeTestCaseMonitorInfo.  # noqa: E501
 
 
         :return: The excluded_transforms of this RimeTestCaseMonitorInfo.  # noqa: E501
         :rtype: MonitorExcludedTransforms
         """
```

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_test_case_status.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_test_case_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_test_metric.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_test_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_test_task_status.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_test_task_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_test_type.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/user_role.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,40 +11,42 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeTestType(object):
+class UserRole(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    STRESS_TESTING_UNSPECIFIED = "TEST_TYPE_STRESS_TESTING_UNSPECIFIED"
-    CONTINUOUS_TESTING = "TEST_TYPE_CONTINUOUS_TESTING"
+    UNSPECIFIED = "ROLE_UNSPECIFIED"
+    ADMIN = "ROLE_ADMIN"
+    TRIAL_USER = "ROLE_TRIAL_USER"
+    SUPPORT = "ROLE_SUPPORT"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """RimeTestType - a model defined in Swagger"""  # noqa: E501
+        """UserRole - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -60,15 +62,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeTestType, dict):
+        if issubclass(UserRole, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -76,15 +78,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeTestType):
+        if not isinstance(other, UserRole):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_time_interval.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_time_interval.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_token_type.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_token_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_update_build_info_request.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_build_info_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_update_build_info_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_build_info_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_update_firewall_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_firewall_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_update_integration_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_update_model_card_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_model_card_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_update_monitor_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_monitor_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_update_notification_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_notification_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_update_user_of_workspace_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_user_of_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_update_user_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_user_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_update_workspace_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_upsert_feature_flags_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_upsert_feature_flags_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_user_detail_with_role.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_user_detail_with_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_user_role.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_response.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,139 +11,119 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeUserRole(object):
+class TestrunresultListTestRunsResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'subject_type': 'RimeSubjectType',
-        'subject_id': 'str',
-        'role': 'RimeActorRole',
-        'implicit_grant': 'bool'
+        'test_runs': 'list[TestrunresultTestRunDetail]',
+        'next_page_token': 'str',
+        'has_more': 'bool'
     }
 
     attribute_map = {
-        'subject_type': 'subjectType',
-        'subject_id': 'subjectId',
-        'role': 'role',
-        'implicit_grant': 'implicitGrant'
+        'test_runs': 'testRuns',
+        'next_page_token': 'nextPageToken',
+        'has_more': 'hasMore'
     }
 
-    def __init__(self, subject_type=None, subject_id=None, role=None, implicit_grant=None):  # noqa: E501
-        """RimeUserRole - a model defined in Swagger"""  # noqa: E501
-        self._subject_type = None
-        self._subject_id = None
-        self._role = None
-        self._implicit_grant = None
+    def __init__(self, test_runs=None, next_page_token=None, has_more=None):  # noqa: E501
+        """TestrunresultListTestRunsResponse - a model defined in Swagger"""  # noqa: E501
+        self._test_runs = None
+        self._next_page_token = None
+        self._has_more = None
         self.discriminator = None
-        if subject_type is not None:
-            self.subject_type = subject_type
-        if subject_id is not None:
-            self.subject_id = subject_id
-        if role is not None:
-            self.role = role
-        if implicit_grant is not None:
-            self.implicit_grant = implicit_grant
+        if test_runs is not None:
+            self.test_runs = test_runs
+        if next_page_token is not None:
+            self.next_page_token = next_page_token
+        if has_more is not None:
+            self.has_more = has_more
 
     @property
-    def subject_type(self):
-        """Gets the subject_type of this RimeUserRole.  # noqa: E501
+    def test_runs(self):
+        """Gets the test_runs of this TestrunresultListTestRunsResponse.  # noqa: E501
 
+        The details of the test runs.  # noqa: E501
 
-        :return: The subject_type of this RimeUserRole.  # noqa: E501
-        :rtype: RimeSubjectType
+        :return: The test_runs of this TestrunresultListTestRunsResponse.  # noqa: E501
+        :rtype: list[TestrunresultTestRunDetail]
         """
-        return self._subject_type
+        return self._test_runs
 
-    @subject_type.setter
-    def subject_type(self, subject_type):
-        """Sets the subject_type of this RimeUserRole.
+    @test_runs.setter
+    def test_runs(self, test_runs):
+        """Sets the test_runs of this TestrunresultListTestRunsResponse.
 
+        The details of the test runs.  # noqa: E501
 
-        :param subject_type: The subject_type of this RimeUserRole.  # noqa: E501
-        :type: RimeSubjectType
+        :param test_runs: The test_runs of this TestrunresultListTestRunsResponse.  # noqa: E501
+        :type: list[TestrunresultTestRunDetail]
         """
 
-        self._subject_type = subject_type
+        self._test_runs = test_runs
 
     @property
-    def subject_id(self):
-        """Gets the subject_id of this RimeUserRole.  # noqa: E501
+    def next_page_token(self):
+        """Gets the next_page_token of this TestrunresultListTestRunsResponse.  # noqa: E501
 
+        A token representing the next page from the list returned by a ListTestRuns query.  # noqa: E501
 
-        :return: The subject_id of this RimeUserRole.  # noqa: E501
+        :return: The next_page_token of this TestrunresultListTestRunsResponse.  # noqa: E501
         :rtype: str
         """
-        return self._subject_id
+        return self._next_page_token
 
-    @subject_id.setter
-    def subject_id(self, subject_id):
-        """Sets the subject_id of this RimeUserRole.
+    @next_page_token.setter
+    def next_page_token(self, next_page_token):
+        """Sets the next_page_token of this TestrunresultListTestRunsResponse.
 
+        A token representing the next page from the list returned by a ListTestRuns query.  # noqa: E501
 
-        :param subject_id: The subject_id of this RimeUserRole.  # noqa: E501
+        :param next_page_token: The next_page_token of this TestrunresultListTestRunsResponse.  # noqa: E501
         :type: str
         """
 
-        self._subject_id = subject_id
+        self._next_page_token = next_page_token
 
     @property
-    def role(self):
-        """Gets the role of this RimeUserRole.  # noqa: E501
+    def has_more(self):
+        """Gets the has_more of this TestrunresultListTestRunsResponse.  # noqa: E501
 
+        A Boolean that specifies whether there are more test runs to return.  # noqa: E501
 
-        :return: The role of this RimeUserRole.  # noqa: E501
-        :rtype: RimeActorRole
-        """
-        return self._role
-
-    @role.setter
-    def role(self, role):
-        """Sets the role of this RimeUserRole.
-
-
-        :param role: The role of this RimeUserRole.  # noqa: E501
-        :type: RimeActorRole
-        """
-
-        self._role = role
-
-    @property
-    def implicit_grant(self):
-        """Gets the implicit_grant of this RimeUserRole.  # noqa: E501
-
-
-        :return: The implicit_grant of this RimeUserRole.  # noqa: E501
+        :return: The has_more of this TestrunresultListTestRunsResponse.  # noqa: E501
         :rtype: bool
         """
-        return self._implicit_grant
+        return self._has_more
 
-    @implicit_grant.setter
-    def implicit_grant(self, implicit_grant):
-        """Sets the implicit_grant of this RimeUserRole.
+    @has_more.setter
+    def has_more(self, has_more):
+        """Sets the has_more of this TestrunresultListTestRunsResponse.
 
+        A Boolean that specifies whether there are more test runs to return.  # noqa: E501
 
-        :param implicit_grant: The implicit_grant of this RimeUserRole.  # noqa: E501
+        :param has_more: The has_more of this TestrunresultListTestRunsResponse.  # noqa: E501
         :type: bool
         """
 
-        self._implicit_grant = implicit_grant
+        self._has_more = has_more
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -158,15 +138,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeUserRole, dict):
+        if issubclass(TestrunresultListTestRunsResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -174,15 +154,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeUserRole):
+        if not isinstance(other, TestrunresultListTestRunsResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_user_with_role.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_user_with_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_user_write_mask.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_user_write_mask.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_uuid.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_uuid.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_validate_test_config_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_validate_test_config_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_workspace.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_workspace.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rime_workspace_write_mask.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_workspace_write_mask.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/rischemaintegration_integration.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rischemaintegration_integration.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/riskscore_risk_category_type.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/riskscore_risk_category_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/riskscore_risk_score.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/riskscore_risk_score.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/role_users_body.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/role_users_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/role_workspace_body.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/role_workspace_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/schemamonitor_config.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/schemamonitor_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/schemanotification_config.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/schemanotification_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/statedb_archived_job_logs.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/statedb_archived_job_logs.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/statedb_job_status.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/statedb_job_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrun_generative_test_run_config.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrun_generative_test_run_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrun_ref_eval_datasets.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrun_ref_eval_datasets.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,89 +11,89 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class TestrunTestRunIncrementalConfig(object):
+class UsersUserUserIdUuidBody(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'eval_dataset_id': 'str',
-        'run_time_info': 'RuntimeinfoRunTimeInfo'
+        'project_id': 'object',
+        'user': 'V1projectsprojectIdUuidroleusersuserUserIdUuidUser'
     }
 
     attribute_map = {
-        'eval_dataset_id': 'evalDatasetId',
-        'run_time_info': 'runTimeInfo'
+        'project_id': 'projectId',
+        'user': 'user'
     }
 
-    def __init__(self, eval_dataset_id=None, run_time_info=None):  # noqa: E501
-        """TestrunTestRunIncrementalConfig - a model defined in Swagger"""  # noqa: E501
-        self._eval_dataset_id = None
-        self._run_time_info = None
+    def __init__(self, project_id=None, user=None):  # noqa: E501
+        """UsersUserUserIdUuidBody - a model defined in Swagger"""  # noqa: E501
+        self._project_id = None
+        self._user = None
         self.discriminator = None
-        if eval_dataset_id is not None:
-            self.eval_dataset_id = eval_dataset_id
-        if run_time_info is not None:
-            self.run_time_info = run_time_info
+        if project_id is not None:
+            self.project_id = project_id
+        if user is not None:
+            self.user = user
 
     @property
-    def eval_dataset_id(self):
-        """Gets the eval_dataset_id of this TestrunTestRunIncrementalConfig.  # noqa: E501
+    def project_id(self):
+        """Gets the project_id of this UsersUserUserIdUuidBody.  # noqa: E501
 
-        Uniquely specifies an evaluation Dataset.  # noqa: E501
+        Uniquely specifies a Project.  # noqa: E501
 
-        :return: The eval_dataset_id of this TestrunTestRunIncrementalConfig.  # noqa: E501
-        :rtype: str
+        :return: The project_id of this UsersUserUserIdUuidBody.  # noqa: E501
+        :rtype: object
         """
-        return self._eval_dataset_id
+        return self._project_id
 
-    @eval_dataset_id.setter
-    def eval_dataset_id(self, eval_dataset_id):
-        """Sets the eval_dataset_id of this TestrunTestRunIncrementalConfig.
+    @project_id.setter
+    def project_id(self, project_id):
+        """Sets the project_id of this UsersUserUserIdUuidBody.
 
-        Uniquely specifies an evaluation Dataset.  # noqa: E501
+        Uniquely specifies a Project.  # noqa: E501
 
-        :param eval_dataset_id: The eval_dataset_id of this TestrunTestRunIncrementalConfig.  # noqa: E501
-        :type: str
+        :param project_id: The project_id of this UsersUserUserIdUuidBody.  # noqa: E501
+        :type: object
         """
 
-        self._eval_dataset_id = eval_dataset_id
+        self._project_id = project_id
 
     @property
-    def run_time_info(self):
-        """Gets the run_time_info of this TestrunTestRunIncrementalConfig.  # noqa: E501
+    def user(self):
+        """Gets the user of this UsersUserUserIdUuidBody.  # noqa: E501
 
 
-        :return: The run_time_info of this TestrunTestRunIncrementalConfig.  # noqa: E501
-        :rtype: RuntimeinfoRunTimeInfo
+        :return: The user of this UsersUserUserIdUuidBody.  # noqa: E501
+        :rtype: V1projectsprojectIdUuidroleusersuserUserIdUuidUser
         """
-        return self._run_time_info
+        return self._user
 
-    @run_time_info.setter
-    def run_time_info(self, run_time_info):
-        """Sets the run_time_info of this TestrunTestRunIncrementalConfig.
+    @user.setter
+    def user(self, user):
+        """Sets the user of this UsersUserUserIdUuidBody.
 
 
-        :param run_time_info: The run_time_info of this TestrunTestRunIncrementalConfig.  # noqa: E501
-        :type: RuntimeinfoRunTimeInfo
+        :param user: The user of this UsersUserUserIdUuidBody.  # noqa: E501
+        :type: V1projectsprojectIdUuidroleusersuserUserIdUuidUser
         """
 
-        self._run_time_info = run_time_info
+        self._user = user
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -108,15 +108,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(TestrunTestRunIncrementalConfig, dict):
+        if issubclass(UsersUserUserIdUuidBody, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -124,15 +124,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TestrunTestRunIncrementalConfig):
+        if not isinstance(other, UsersUserUserIdUuidBody):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrun_test_suite_config.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrun_test_suite_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_config_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_config_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_run_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_run_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_list_batch_results_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_list_batch_results_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_list_feature_results_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_list_feature_results_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_list_monitor_categories_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_list_monitor_categories_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_list_summary_tests_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_list_summary_tests_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_cases_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_cases_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_request_query.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_case_display.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,119 +11,117 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class TestrunresultListTestRunsResponse(object):
+class TestrunresultTestCaseDisplay(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'test_runs': 'list[TestrunresultTestRunDetail]',
-        'next_page_token': 'str',
-        'has_more': 'bool'
+        'table_info': 'str',
+        'details': 'str',
+        'details_layout': 'list[str]'
     }
 
     attribute_map = {
-        'test_runs': 'testRuns',
-        'next_page_token': 'nextPageToken',
-        'has_more': 'hasMore'
+        'table_info': 'tableInfo',
+        'details': 'details',
+        'details_layout': 'detailsLayout'
     }
 
-    def __init__(self, test_runs=None, next_page_token=None, has_more=None):  # noqa: E501
-        """TestrunresultListTestRunsResponse - a model defined in Swagger"""  # noqa: E501
-        self._test_runs = None
-        self._next_page_token = None
-        self._has_more = None
+    def __init__(self, table_info=None, details=None, details_layout=None):  # noqa: E501
+        """TestrunresultTestCaseDisplay - a model defined in Swagger"""  # noqa: E501
+        self._table_info = None
+        self._details = None
+        self._details_layout = None
         self.discriminator = None
-        if test_runs is not None:
-            self.test_runs = test_runs
-        if next_page_token is not None:
-            self.next_page_token = next_page_token
-        if has_more is not None:
-            self.has_more = has_more
+        if table_info is not None:
+            self.table_info = table_info
+        if details is not None:
+            self.details = details
+        if details_layout is not None:
+            self.details_layout = details_layout
 
     @property
-    def test_runs(self):
-        """Gets the test_runs of this TestrunresultListTestRunsResponse.  # noqa: E501
+    def table_info(self):
+        """Gets the table_info of this TestrunresultTestCaseDisplay.  # noqa: E501
 
-        The details of the test runs.  # noqa: E501
+        Table info contains information for displaying the test case in a table in the FE.  # noqa: E501
 
-        :return: The test_runs of this TestrunresultListTestRunsResponse.  # noqa: E501
-        :rtype: list[TestrunresultTestRunDetail]
+        :return: The table_info of this TestrunresultTestCaseDisplay.  # noqa: E501
+        :rtype: str
         """
-        return self._test_runs
+        return self._table_info
 
-    @test_runs.setter
-    def test_runs(self, test_runs):
-        """Sets the test_runs of this TestrunresultListTestRunsResponse.
+    @table_info.setter
+    def table_info(self, table_info):
+        """Sets the table_info of this TestrunresultTestCaseDisplay.
 
-        The details of the test runs.  # noqa: E501
+        Table info contains information for displaying the test case in a table in the FE.  # noqa: E501
 
-        :param test_runs: The test_runs of this TestrunresultListTestRunsResponse.  # noqa: E501
-        :type: list[TestrunresultTestRunDetail]
+        :param table_info: The table_info of this TestrunresultTestCaseDisplay.  # noqa: E501
+        :type: str
         """
 
-        self._test_runs = test_runs
+        self._table_info = table_info
 
     @property
-    def next_page_token(self):
-        """Gets the next_page_token of this TestrunresultListTestRunsResponse.  # noqa: E501
+    def details(self):
+        """Gets the details of this TestrunresultTestCaseDisplay.  # noqa: E501
 
-        A token representing the next page from the list returned by a ListTestRuns query.  # noqa: E501
+        Details includes ML-specified details for the test case. This can include graphs, HTML, etc.  # noqa: E501
 
-        :return: The next_page_token of this TestrunresultListTestRunsResponse.  # noqa: E501
+        :return: The details of this TestrunresultTestCaseDisplay.  # noqa: E501
         :rtype: str
         """
-        return self._next_page_token
+        return self._details
 
-    @next_page_token.setter
-    def next_page_token(self, next_page_token):
-        """Sets the next_page_token of this TestrunresultListTestRunsResponse.
+    @details.setter
+    def details(self, details):
+        """Sets the details of this TestrunresultTestCaseDisplay.
 
-        A token representing the next page from the list returned by a ListTestRuns query.  # noqa: E501
+        Details includes ML-specified details for the test case. This can include graphs, HTML, etc.  # noqa: E501
 
-        :param next_page_token: The next_page_token of this TestrunresultListTestRunsResponse.  # noqa: E501
+        :param details: The details of this TestrunresultTestCaseDisplay.  # noqa: E501
         :type: str
         """
 
-        self._next_page_token = next_page_token
+        self._details = details
 
     @property
-    def has_more(self):
-        """Gets the has_more of this TestrunresultListTestRunsResponse.  # noqa: E501
+    def details_layout(self):
+        """Gets the details_layout of this TestrunresultTestCaseDisplay.  # noqa: E501
 
-        A Boolean that specifies whether there are more test runs to return.  # noqa: E501
 
-        :return: The has_more of this TestrunresultListTestRunsResponse.  # noqa: E501
-        :rtype: bool
+        :return: The details_layout of this TestrunresultTestCaseDisplay.  # noqa: E501
+        :rtype: list[str]
         """
-        return self._has_more
+        return self._details_layout
 
-    @has_more.setter
-    def has_more(self, has_more):
-        """Sets the has_more of this TestrunresultListTestRunsResponse.
+    @details_layout.setter
+    def details_layout(self, details_layout):
+        """Sets the details_layout of this TestrunresultTestCaseDisplay.
 
-        A Boolean that specifies whether there are more test runs to return.  # noqa: E501
 
-        :param has_more: The has_more of this TestrunresultListTestRunsResponse.  # noqa: E501
-        :type: bool
+        :param details_layout: The details_layout of this TestrunresultTestCaseDisplay.  # noqa: E501
+        :type: list[str]
         """
 
-        self._has_more = has_more
+        self._details_layout = details_layout
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -138,15 +136,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(TestrunresultListTestRunsResponse, dict):
+        if issubclass(TestrunresultTestCaseDisplay, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -154,15 +152,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TestrunresultListTestRunsResponse):
+        if not isinstance(other, TestrunresultTestCaseDisplay):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_list_validation_categories_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_list_validation_categories_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_rename_test_run_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_rename_test_run_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_result_summary_counts.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_result_summary_counts.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -355,26 +355,26 @@
 
         self._metrics = metrics
 
     @property
     def show_in_test_comparisons(self):
         """Gets the show_in_test_comparisons of this TestrunresultTestBatchResult.  # noqa: E501
 
-        A Boolean that specifies whether to include the test batch in the test comparison page in the web UI.  # noqa: E501
+        A Boolean that specifies whether to include the test batch in the test comparison page in the web UI. This field is no longer used, and will be removed in 2.3.  # noqa: E501
 
         :return: The show_in_test_comparisons of this TestrunresultTestBatchResult.  # noqa: E501
         :rtype: bool
         """
         return self._show_in_test_comparisons
 
     @show_in_test_comparisons.setter
     def show_in_test_comparisons(self, show_in_test_comparisons):
         """Sets the show_in_test_comparisons of this TestrunresultTestBatchResult.
 
-        A Boolean that specifies whether to include the test batch in the test comparison page in the web UI.  # noqa: E501
+        A Boolean that specifies whether to include the test batch in the test comparison page in the web UI. This field is no longer used, and will be removed in 2.3.  # noqa: E501
 
         :param show_in_test_comparisons: The show_in_test_comparisons of this TestrunresultTestBatchResult.  # noqa: E501
         :type: bool
         """
 
         self._show_in_test_comparisons = show_in_test_comparisons
```

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result_display.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result_display.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_test_case.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_case.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result_display.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result_display.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_detail.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_detail.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,15 +38,16 @@
         'model_id': 'RimeUUID',
         'upload_time': 'datetime',
         'web_app_url': 'RimeSafeURL',
         'test_categories': 'list[TestrunTestCategoryType]',
         'metrics': 'TestrunresultTestRunMetrics',
         'status': 'RimeTestTaskStatus',
         'progress': 'str',
-        'rime_version': 'str'
+        'rime_version': 'str',
+        'bin_time_interval': 'RimeTimeInterval'
     }
 
     attribute_map = {
         'test_run_id': 'testRunId',
         'name': 'name',
         'project_id': 'projectId',
         'testing_type': 'testingType',
@@ -56,18 +57,19 @@
         'model_id': 'modelId',
         'upload_time': 'uploadTime',
         'web_app_url': 'webAppUrl',
         'test_categories': 'testCategories',
         'metrics': 'metrics',
         'status': 'status',
         'progress': 'progress',
-        'rime_version': 'rimeVersion'
+        'rime_version': 'rimeVersion',
+        'bin_time_interval': 'binTimeInterval'
     }
 
-    def __init__(self, test_run_id=None, name=None, project_id=None, testing_type=None, model_task=None, ref_data_id=None, eval_data_id=None, model_id=None, upload_time=None, web_app_url=None, test_categories=None, metrics=None, status=None, progress=None, rime_version=None):  # noqa: E501
+    def __init__(self, test_run_id=None, name=None, project_id=None, testing_type=None, model_task=None, ref_data_id=None, eval_data_id=None, model_id=None, upload_time=None, web_app_url=None, test_categories=None, metrics=None, status=None, progress=None, rime_version=None, bin_time_interval=None):  # noqa: E501
         """TestrunresultTestRunDetail - a model defined in Swagger"""  # noqa: E501
         self._test_run_id = None
         self._name = None
         self._project_id = None
         self._testing_type = None
         self._model_task = None
         self._ref_data_id = None
@@ -76,14 +78,15 @@
         self._upload_time = None
         self._web_app_url = None
         self._test_categories = None
         self._metrics = None
         self._status = None
         self._progress = None
         self._rime_version = None
+        self._bin_time_interval = None
         self.discriminator = None
         if test_run_id is not None:
             self.test_run_id = test_run_id
         if name is not None:
             self.name = name
         if project_id is not None:
             self.project_id = project_id
@@ -107,14 +110,16 @@
             self.metrics = metrics
         if status is not None:
             self.status = status
         if progress is not None:
             self.progress = progress
         if rime_version is not None:
             self.rime_version = rime_version
+        if bin_time_interval is not None:
+            self.bin_time_interval = bin_time_interval
 
     @property
     def test_run_id(self):
         """Gets the test_run_id of this TestrunresultTestRunDetail.  # noqa: E501
 
         Uniquely specifies a Test Run.  # noqa: E501
 
@@ -439,14 +444,35 @@
 
         :param rime_version: The rime_version of this TestrunresultTestRunDetail.  # noqa: E501
         :type: str
         """
 
         self._rime_version = rime_version
 
+    @property
+    def bin_time_interval(self):
+        """Gets the bin_time_interval of this TestrunresultTestRunDetail.  # noqa: E501
+
+
+        :return: The bin_time_interval of this TestrunresultTestRunDetail.  # noqa: E501
+        :rtype: RimeTimeInterval
+        """
+        return self._bin_time_interval
+
+    @bin_time_interval.setter
+    def bin_time_interval(self, bin_time_interval):
+        """Sets the bin_time_interval of this TestrunresultTestRunDetail.
+
+
+        :param bin_time_interval: The bin_time_interval of this TestrunresultTestRunDetail.  # noqa: E501
+        :type: RimeTimeInterval
+        """
+
+        self._bin_time_interval = bin_time_interval
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_metrics.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_metrics.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/user_favorite_projects.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/user_favorite_projects.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/user_private_info.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/user_private_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/user_role.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/detection_metric_degradation_event_details.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,42 +11,34 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class UserRole(object):
+class DetectionMetricDegradationEventDetails(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
-
-    """
-    allowed enum values
-    """
-    UNSPECIFIED = "ROLE_UNSPECIFIED"
-    ADMIN = "ROLE_ADMIN"
-    TRIAL_USER = "ROLE_TRIAL_USER"
-    SUPPORT = "ROLE_SUPPORT"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """UserRole - a model defined in Swagger"""  # noqa: E501
+        """DetectionMetricDegradationEventDetails - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -62,15 +54,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(UserRole, dict):
+        if issubclass(DetectionMetricDegradationEventDetails, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -78,15 +70,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, UserRole):
+        if not isinstance(other, DetectionMetricDegradationEventDetails):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/user_user_detail.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/user_user_detail.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/users_user_id_uuid_body.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/users_user_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,89 +11,92 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class UsersUserUserIdUuidBody(object):
+class WorkspaceIdUuidUsersBody(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'project_id': 'object',
-        'user': 'V1projectsprojectIdUuidroleusersuserUserIdUuidUser'
+        'workspace_id': 'object',
+        'users': 'list[RimeUserWithRole]'
     }
 
     attribute_map = {
-        'project_id': 'projectId',
-        'user': 'user'
+        'workspace_id': 'workspaceId',
+        'users': 'users'
     }
 
-    def __init__(self, project_id=None, user=None):  # noqa: E501
-        """UsersUserUserIdUuidBody - a model defined in Swagger"""  # noqa: E501
-        self._project_id = None
-        self._user = None
+    def __init__(self, workspace_id=None, users=None):  # noqa: E501
+        """WorkspaceIdUuidUsersBody - a model defined in Swagger"""  # noqa: E501
+        self._workspace_id = None
+        self._users = None
         self.discriminator = None
-        if project_id is not None:
-            self.project_id = project_id
-        if user is not None:
-            self.user = user
+        if workspace_id is not None:
+            self.workspace_id = workspace_id
+        self.users = users
 
     @property
-    def project_id(self):
-        """Gets the project_id of this UsersUserUserIdUuidBody.  # noqa: E501
+    def workspace_id(self):
+        """Gets the workspace_id of this WorkspaceIdUuidUsersBody.  # noqa: E501
 
-        Uniquely specifies a Project.  # noqa: E501
+        Unique ID of an object in RIME.  # noqa: E501
 
-        :return: The project_id of this UsersUserUserIdUuidBody.  # noqa: E501
+        :return: The workspace_id of this WorkspaceIdUuidUsersBody.  # noqa: E501
         :rtype: object
         """
-        return self._project_id
+        return self._workspace_id
 
-    @project_id.setter
-    def project_id(self, project_id):
-        """Sets the project_id of this UsersUserUserIdUuidBody.
+    @workspace_id.setter
+    def workspace_id(self, workspace_id):
+        """Sets the workspace_id of this WorkspaceIdUuidUsersBody.
 
-        Uniquely specifies a Project.  # noqa: E501
+        Unique ID of an object in RIME.  # noqa: E501
 
-        :param project_id: The project_id of this UsersUserUserIdUuidBody.  # noqa: E501
+        :param workspace_id: The workspace_id of this WorkspaceIdUuidUsersBody.  # noqa: E501
         :type: object
         """
 
-        self._project_id = project_id
+        self._workspace_id = workspace_id
 
     @property
-    def user(self):
-        """Gets the user of this UsersUserUserIdUuidBody.  # noqa: E501
+    def users(self):
+        """Gets the users of this WorkspaceIdUuidUsersBody.  # noqa: E501
 
+        List of Users to add to the Workspace.  # noqa: E501
 
-        :return: The user of this UsersUserUserIdUuidBody.  # noqa: E501
-        :rtype: V1projectsprojectIdUuidroleusersuserUserIdUuidUser
+        :return: The users of this WorkspaceIdUuidUsersBody.  # noqa: E501
+        :rtype: list[RimeUserWithRole]
         """
-        return self._user
+        return self._users
 
-    @user.setter
-    def user(self, user):
-        """Sets the user of this UsersUserUserIdUuidBody.
+    @users.setter
+    def users(self, users):
+        """Sets the users of this WorkspaceIdUuidUsersBody.
 
+        List of Users to add to the Workspace.  # noqa: E501
 
-        :param user: The user of this UsersUserUserIdUuidBody.  # noqa: E501
-        :type: V1projectsprojectIdUuidroleusersuserUserIdUuidUser
+        :param users: The users of this WorkspaceIdUuidUsersBody.  # noqa: E501
+        :type: list[RimeUserWithRole]
         """
+        if users is None:
+            raise ValueError("Invalid value for `users`, must not be `None`")  # noqa: E501
 
-        self._user = user
+        self._users = users
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -108,15 +111,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(UsersUserUserIdUuidBody, dict):
+        if issubclass(WorkspaceIdUuidUsersBody, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -124,15 +127,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, UsersUserUserIdUuidBody):
+        if not isinstance(other, WorkspaceIdUuidUsersBody):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/v1betamonitorsmonitor_id_uuid_monitor.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/v1betamonitorsmonitor_id_uuid_monitor.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,14 @@
         'firewall_id': 'RimeUUID',
         'monitor_type': 'MonitorMonitorType',
         'risk_category_type': 'RiskscoreRiskCategoryType',
         'test_category': 'TestrunTestCategoryType',
         'artifact_identifier': 'MonitorArtifactIdentifier',
         'created_time': 'datetime',
         'notify': 'bool',
-        'rca_role': 'RcaRCARole',
         'config': 'SchemamonitorConfig',
         'excluded_transforms': 'MonitorExcludedTransforms',
         'pinned': 'bool'
     }
 
     attribute_map = {
         'id': 'id',
@@ -49,32 +48,30 @@
         'firewall_id': 'firewallId',
         'monitor_type': 'monitorType',
         'risk_category_type': 'riskCategoryType',
         'test_category': 'testCategory',
         'artifact_identifier': 'artifactIdentifier',
         'created_time': 'createdTime',
         'notify': 'notify',
-        'rca_role': 'rcaRole',
         'config': 'config',
         'excluded_transforms': 'excludedTransforms',
         'pinned': 'pinned'
     }
 
-    def __init__(self, id=None, name=None, firewall_id=None, monitor_type=None, risk_category_type=None, test_category=None, artifact_identifier=None, created_time=None, notify=None, rca_role=None, config=None, excluded_transforms=None, pinned=None):  # noqa: E501
+    def __init__(self, id=None, name=None, firewall_id=None, monitor_type=None, risk_category_type=None, test_category=None, artifact_identifier=None, created_time=None, notify=None, config=None, excluded_transforms=None, pinned=None):  # noqa: E501
         """V1betamonitorsmonitorIdUuidMonitor - a model defined in Swagger"""  # noqa: E501
         self._id = None
         self._name = None
         self._firewall_id = None
         self._monitor_type = None
         self._risk_category_type = None
         self._test_category = None
         self._artifact_identifier = None
         self._created_time = None
         self._notify = None
-        self._rca_role = None
         self._config = None
         self._excluded_transforms = None
         self._pinned = None
         self.discriminator = None
         if id is not None:
             self.id = id
         if name is not None:
@@ -89,16 +86,14 @@
             self.test_category = test_category
         if artifact_identifier is not None:
             self.artifact_identifier = artifact_identifier
         if created_time is not None:
             self.created_time = created_time
         if notify is not None:
             self.notify = notify
-        if rca_role is not None:
-            self.rca_role = rca_role
         if config is not None:
             self.config = config
         if excluded_transforms is not None:
             self.excluded_transforms = excluded_transforms
         if pinned is not None:
             self.pinned = pinned
 
@@ -296,35 +291,14 @@
         :param notify: The notify of this V1betamonitorsmonitorIdUuidMonitor.  # noqa: E501
         :type: bool
         """
 
         self._notify = notify
 
     @property
-    def rca_role(self):
-        """Gets the rca_role of this V1betamonitorsmonitorIdUuidMonitor.  # noqa: E501
-
-
-        :return: The rca_role of this V1betamonitorsmonitorIdUuidMonitor.  # noqa: E501
-        :rtype: RcaRCARole
-        """
-        return self._rca_role
-
-    @rca_role.setter
-    def rca_role(self, rca_role):
-        """Sets the rca_role of this V1betamonitorsmonitorIdUuidMonitor.
-
-
-        :param rca_role: The rca_role of this V1betamonitorsmonitorIdUuidMonitor.  # noqa: E501
-        :type: RcaRCARole
-        """
-
-        self._rca_role = rca_role
-
-    @property
     def config(self):
         """Gets the config of this V1betamonitorsmonitorIdUuidMonitor.  # noqa: E501
 
 
         :return: The config of this V1betamonitorsmonitorIdUuidMonitor.  # noqa: E501
         :rtype: SchemamonitorConfig
         """
```

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/v1notifsettingsnotification_id_uuid_notification.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/v1notifsettingsnotification_id_uuid_notification.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/v1projectsproject_id_uuidroleusersuser_user_id_uuid_user.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/v1projectsproject_id_uuidroleusersuser_user_id_uuid_user.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/validation_validate_dataset_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/validation_validate_dataset_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/validation_validate_model_response.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/validation_validate_model_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/swagger/swagger_client/rest.py` & `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/rest.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/test_batch.py` & `rime_sdk-2.2.0rc3/rime_sdk/test_batch.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk/test_run.py` & `rime_sdk-2.2.0rc3/rime_sdk/test_run.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc2/rime_sdk.egg-info/PKG-INFO` & `rime_sdk-2.2.0rc3/rime_sdk.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rime-sdk
-Version: 2.2.0rc2
+Version: 2.2.0rc3
 Summary: Package to programmatically access a RIME deployment
 Home-page: UNKNOWN
 License: OSI Approved :: Apache Software License
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `rime_sdk-2.2.0rc2/rime_sdk.egg-info/SOURCES.txt` & `rime_sdk-2.2.0rc3/rime_sdk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -188,19 +188,14 @@
 rime_sdk/swagger/swagger_client/models/project_remove_user_from_project_response.py
 rime_sdk/swagger/swagger_client/models/project_update_project_response.py
 rime_sdk/swagger/swagger_client/models/project_update_user_of_project_response.py
 rime_sdk/swagger/swagger_client/models/project_update_workspace_roles_for_project_response.py
 rime_sdk/swagger/swagger_client/models/projects_project_id_uuid_body.py
 rime_sdk/swagger/swagger_client/models/protobuf_any.py
 rime_sdk/swagger/swagger_client/models/protobuf_null_value.py
-rime_sdk/swagger/swagger_client/models/rca_feature_cause.py
-rime_sdk/swagger/swagger_client/models/rca_rca_result.py
-rime_sdk/swagger/swagger_client/models/rca_rca_role.py
-rime_sdk/swagger/swagger_client/models/rca_test_case_cause.py
-rime_sdk/swagger/swagger_client/models/rca_test_case_id.py
 rime_sdk/swagger/swagger_client/models/registry_connection_info.py
 rime_sdk/swagger/swagger_client/models/registry_data_collector_info.py
 rime_sdk/swagger/swagger_client/models/registry_data_file_info.py
 rime_sdk/swagger/swagger_client/models/registry_data_info.py
 rime_sdk/swagger/swagger_client/models/registry_data_loading_info.py
 rime_sdk/swagger/swagger_client/models/registry_data_params.py
 rime_sdk/swagger/swagger_client/models/registry_data_type.py
```

### Comparing `rime_sdk-2.2.0rc2/setup.py` & `rime_sdk-2.2.0rc3/setup.py`

 * *Files identical despite different names*

